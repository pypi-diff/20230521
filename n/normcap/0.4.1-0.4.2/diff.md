# Comparing `tmp/normcap-0.4.1.tar.gz` & `tmp/normcap-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "normcap-0.4.1.tar", max compression
+gzip compressed data, was "normcap-0.4.2.tar", max compression
```

## Comparing `normcap-0.4.1.tar` & `normcap-0.4.2.tar`

### file list

```diff
@@ -1,66 +1,65 @@
--rw-r--r--   0        0        0    13604 2023-05-01 12:30:54.612167 normcap-0.4.1/CHANGELOG
--rw-r--r--   0        0        0      724 2023-05-01 12:30:54.612167 normcap-0.4.1/LICENSE
--rw-r--r--   0        0        0     7062 2023-05-01 12:30:54.612167 normcap-0.4.1/README.md
--rw-r--r--   0        0        0       46 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/__init__.py
--rw-r--r--   0        0        0      113 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/__main__.py
--rw-r--r--   0        0        0     1659 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/app.py
--rw-r--r--   0        0        0      450 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/clipboard/__init__.py
--rw-r--r--   0        0        0     1187 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/clipboard/linux.py
--rw-r--r--   0        0        0      588 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/clipboard/macos.py
--rw-r--r--   0        0        0      284 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/clipboard/qt.py
--rw-r--r--   0        0        0     5885 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/clipboard/windows.py
--rw-r--r--   0        0        0        0 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/__init__.py
--rw-r--r--   0        0        0     8955 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/constants.py
--rw-r--r--   0        0        0     2356 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/downloader.py
--rw-r--r--   0        0        0     8359 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/language_manager.py
--rw-r--r--   0        0        0     2753 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/loading_indicator.py
--rw-r--r--   0        0        0    10006 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/menu_button.py
--rw-r--r--   0        0        0     3481 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/models.py
--rw-r--r--   0        0        0     3949 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/notifier.py
--rw-r--r--   0        0        0   217598 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/resources.py
--rw-r--r--   0        0        0     3552 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/settings.py
--rw-r--r--   0        0        0     6205 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/system_info.py
--rw-r--r--   0        0        0    20812 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/tray.py
--rw-r--r--   0        0        0     4568 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/update_check.py
--rw-r--r--   0        0        0      758 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/utils.py
--rw-r--r--   0        0        0    11944 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/gui/window.py
--rw-r--r--   0        0        0       93 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/__init__.py
--rw-r--r--   0        0        0     3603 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/enhance.py
--rw-r--r--   0        0        0       46 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/__init__.py
--rw-r--r--   0        0        0      870 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/base_magic.py
--rw-r--r--   0        0        0     1807 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/email_magic.py
--rw-r--r--   0        0        0     2463 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/magic.py
--rw-r--r--   0        0        0     1048 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/multi_line_magic.py
--rw-r--r--   0        0        0     1546 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/paragraph_magic.py
--rw-r--r--   0        0        0      964 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/single_line_magic.py
--rw-r--r--   0        0        0     2699 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/magics/url_magic.py
--rw-r--r--   0        0        0     5121 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/models.py
--rw-r--r--   0        0        0     1535 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/recognize.py
--rw-r--r--   0        0        0     3305 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/ocr/tesseract.py
--rw-r--r--   0        0        0        0 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/resources/__init__.py
--rw-r--r--   0        0        0    13773 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/resources/icons/normcap.png
--rw-r--r--   0        0        0    24936 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/resources/icons/normcap.svg
--rw-r--r--   0        0        0     9267 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/resources/icons/notification.png
--rw-r--r--   0        0        0    16576 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/resources/icons/notification.svg
--rw-r--r--   0        0        0     9267 2023-05-01 12:30:54.976166 normcap-0.4.1/normcap/resources/icons/parse.png
--rw-r--r--   0        0        0    16576 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/parse.svg
--rw-r--r--   0        0        0     2982 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/raw.png
--rw-r--r--   0        0        0    14953 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/raw.svg
--rw-r--r--   0        0        0      528 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/resources.qrc
--rw-r--r--   0        0        0    17968 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/settings.png
--rw-r--r--   0        0        0    13793 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/settings.svg
--rw-r--r--   0        0        0    17311 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/tray.png
--rw-r--r--   0        0        0    16523 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/icons/tray.svg
--rw-r--r--   0        0        0       79 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/tessdata/.keep
--rw-r--r--   0        0        0    11358 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/tessdata/LICENSE.txt
--rw-r--r--   0        0        0     1081 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/resources/tessdata/README.txt
--rw-r--r--   0        0        0     1623 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/screengrab/__init__.py
--rw-r--r--   0        0        0     7202 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/screengrab/dbus_portal.py
--rw-r--r--   0        0        0     4239 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/screengrab/dbus_portal_legacy.py
--rw-r--r--   0        0        0     1816 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/screengrab/dbus_shell.py
--rw-r--r--   0        0        0      461 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/screengrab/qt.py
--rw-r--r--   0        0        0     5512 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/screengrab/utils.py
--rw-r--r--   0        0        0     7463 2023-05-01 12:30:54.980166 normcap-0.4.1/normcap/utils.py
--rw-r--r--   0        0        0     7764 2023-05-01 12:30:54.980166 normcap-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     8263 1970-01-01 00:00:00.000000 normcap-0.4.1/setup.py
--rw-r--r--   0        0        0     8543 1970-01-01 00:00:00.000000 normcap-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    13806 2023-05-21 10:20:44.792297 normcap-0.4.2/CHANGELOG
+-rw-r--r--   0        0        0      724 2023-05-21 10:20:44.792297 normcap-0.4.2/LICENSE
+-rw-r--r--   0        0        0     6999 2023-05-21 10:20:44.792297 normcap-0.4.2/README.md
+-rw-r--r--   0        0        0       46 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/__init__.py
+-rw-r--r--   0        0        0      113 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/__main__.py
+-rw-r--r--   0        0        0     1659 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/app.py
+-rw-r--r--   0        0        0      450 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/clipboard/__init__.py
+-rw-r--r--   0        0        0     1440 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/clipboard/linux.py
+-rw-r--r--   0        0        0      588 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/clipboard/macos.py
+-rw-r--r--   0        0        0      284 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/clipboard/qt.py
+-rw-r--r--   0        0        0     5885 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/clipboard/windows.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/__init__.py
+-rw-r--r--   0        0        0     8955 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/constants.py
+-rw-r--r--   0        0        0     2356 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/downloader.py
+-rw-r--r--   0        0        0     8359 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/language_manager.py
+-rw-r--r--   0        0        0     2753 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/loading_indicator.py
+-rw-r--r--   0        0        0    10108 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/menu_button.py
+-rw-r--r--   0        0        0     3481 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/models.py
+-rw-r--r--   0        0        0     3949 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/notifier.py
+-rw-r--r--   0        0        0   217598 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/resources.py
+-rw-r--r--   0        0        0     3552 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/settings.py
+-rw-r--r--   0        0        0     6205 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/system_info.py
+-rw-r--r--   0        0        0    20841 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/tray.py
+-rw-r--r--   0        0        0     4568 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/update_check.py
+-rw-r--r--   0        0        0      758 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/utils.py
+-rw-r--r--   0        0        0    11944 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/gui/window.py
+-rw-r--r--   0        0        0       93 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/__init__.py
+-rw-r--r--   0        0        0     3603 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/enhance.py
+-rw-r--r--   0        0        0       46 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/__init__.py
+-rw-r--r--   0        0        0      870 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/base_magic.py
+-rw-r--r--   0        0        0     1807 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/email_magic.py
+-rw-r--r--   0        0        0     2463 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/magic.py
+-rw-r--r--   0        0        0     1048 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/multi_line_magic.py
+-rw-r--r--   0        0        0     1546 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/paragraph_magic.py
+-rw-r--r--   0        0        0      964 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/single_line_magic.py
+-rw-r--r--   0        0        0     2699 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/magics/url_magic.py
+-rw-r--r--   0        0        0     5121 2023-05-21 10:20:45.116303 normcap-0.4.2/normcap/ocr/models.py
+-rw-r--r--   0        0        0     1535 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/ocr/recognize.py
+-rw-r--r--   0        0        0     3321 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/ocr/tesseract.py
+-rw-r--r--   0        0        0        0 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/__init__.py
+-rw-r--r--   0        0        0    13773 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/normcap.png
+-rw-r--r--   0        0        0    24936 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/normcap.svg
+-rw-r--r--   0        0        0     9267 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/notification.png
+-rw-r--r--   0        0        0    16576 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/notification.svg
+-rw-r--r--   0        0        0     9267 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/parse.png
+-rw-r--r--   0        0        0    16576 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/parse.svg
+-rw-r--r--   0        0        0     2982 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/raw.png
+-rw-r--r--   0        0        0    14953 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/raw.svg
+-rw-r--r--   0        0        0      528 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/resources.qrc
+-rw-r--r--   0        0        0    17968 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/settings.png
+-rw-r--r--   0        0        0    13793 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/settings.svg
+-rw-r--r--   0        0        0    17311 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/tray.png
+-rw-r--r--   0        0        0    16523 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/icons/tray.svg
+-rw-r--r--   0        0        0       79 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/tessdata/.keep
+-rw-r--r--   0        0        0    11358 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/tessdata/LICENSE.txt
+-rw-r--r--   0        0        0     1081 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/resources/tessdata/README.txt
+-rw-r--r--   0        0        0     1242 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/screengrab/__init__.py
+-rw-r--r--   0        0        0     7202 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/screengrab/dbus_portal.py
+-rw-r--r--   0        0        0     1816 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/screengrab/dbus_shell.py
+-rw-r--r--   0        0        0      461 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/screengrab/qt.py
+-rw-r--r--   0        0        0     5512 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/screengrab/utils.py
+-rw-r--r--   0        0        0     7463 2023-05-21 10:20:45.120303 normcap-0.4.2/normcap/utils.py
+-rw-r--r--   0        0        0     7044 2023-05-21 10:20:45.124303 normcap-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     8174 1970-01-01 00:00:00.000000 normcap-0.4.2/setup.py
+-rw-r--r--   0        0        0     8440 1970-01-01 00:00:00.000000 normcap-0.4.2/PKG-INFO
```

### Comparing `normcap-0.4.1/CHANGELOG` & `normcap-0.4.2/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Changelog
 
-## v0.4.1 (2023-05-01)
+## v0.4.2 (2023-05-21)
+
+- Fix quotes in detected text can result in wrong detection.
+  ([#446](https://github.com/dynobo/normcap/issues/446))
+- Update AppImage base image from Ubuntu 18.04 (deprected) to 20.04.
 
-**All:**
+## v0.4.1 (2023-05-01)
 
 - Enlarge settings button a bit to make it easier to spot.
   ([#254](https://github.com/dynobo/normcap/issues/254))
 - Prevent running multiple instances and start capture in original instance instead.
   ([#306](https://github.com/dynobo/normcap/issues/306))
 - Fix unintended re-capture if tray icon is disabled.
   ([#254](https://github.com/dynobo/normcap/issues/254))
```

### Comparing `normcap-0.4.1/LICENSE` & `normcap-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/README.md` & `normcap-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 [![Screencast](https://user-images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/assets/normcap.gif)
 
 ## Quickstart
 
 Install a prebuilt release:
 
 - **Windows**:
-  [NormCap-0.4.1-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-0.4.1-x86_64-Windows.msi)
+  [NormCap-0.4.2-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64-Windows.msi)
 - **Linux**:
-  [NormCap-0.4.1-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-0.4.1-x86_64.AppImage)
+  [NormCap-0.4.2-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64.AppImage)
 - **macOS** (x86) ¹:
-  [NormCap-0.4.1-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-0.4.1-x86_64-macOS.dmg)
+  [NormCap-0.4.2-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64-macOS.dmg)
 - **macOS** (M1) ¹·²:
-  [NormCap-0.4.1-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-0.4.1-arm64-macOS.dmg)
+  [NormCap-0.4.2-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-arm64-macOS.dmg)
   \
   <sub>1: On macOS, allow the unsigned application on first start: "System
   Preferences" → "Security & Privacy" → "General" → "Open anyway". You might also need
   to allow NormCap to take screenshots.
   [#135](https://github.com/dynobo/normcap/issues/135)<br> 2: Might be available a bit
   delayed, as it is currently build manually. (Thx,
   [@Takrin](https://github.com/Takrin)!)</sub>
@@ -164,15 +164,14 @@
 ```
 
 ## Credits
 
 This project uses the following non-standard libraries:
 
 - [pyside6](https://pypi.org/project/PySide6/) _- bindings for Qt UI Framework_
-- [jeepney](https://pypi.org/project/jeepney/) _- DBUS client_
 
 And it depends on external software:
 
 - [tesseract](https://github.com/tesseract-ocr/tesseract) - _OCR engine_
 - [wl-clipboard](https://github.com/bugaevc/wl-clipboard) - _Wayland clipboard
   utilities_
```

#### html2text {}

```diff
@@ -19,22 +19,22 @@
 (https://github.com/dynobo/normcap) | [Documentation](https://dynobo.github.io/
 normcap/) | [FAQs](https://dynobo.github.io/normcap/#faqs) | [Releases](https:/
 /github.com/dynobo/normcap/releases) | [Changelog](https://github.com/dynobo/
 normcap/blob/main/CHANGELOG) [![Screencast](https://user-
 images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-
 cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/
 assets/normcap.gif) ## Quickstart Install a prebuilt release: - **Windows**:
-[NormCap-0.4.1-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/
-download/v0.4.1/NormCap-0.4.1-x86_64-Windows.msi) - **Linux**: [NormCap-0.4.1-
-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.1/
-NormCap-0.4.1-x86_64.AppImage) - **macOS** (x86) Â¹: [NormCap-0.4.1-x86_64-
-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-
-0.4.1-x86_64-macOS.dmg) - **macOS** (M1) Â¹Â·Â²: [NormCap-0.4.1-arm64-
-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-
-0.4.1-arm64-macOS.dmg) \ 1: On macOS, allow the unsigned application on first
+[NormCap-0.4.2-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/
+download/v0.4.2/NormCap-0.4.2-x86_64-Windows.msi) - **Linux**: [NormCap-0.4.2-
+x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.2/
+NormCap-0.4.2-x86_64.AppImage) - **macOS** (x86) Â¹: [NormCap-0.4.2-x86_64-
+macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-
+0.4.2-x86_64-macOS.dmg) - **macOS** (M1) Â¹Â·Â²: [NormCap-0.4.2-arm64-
+macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-
+0.4.2-arm64-macOS.dmg) \ 1: On macOS, allow the unsigned application on first
 start: "System Preferences" â "Security & Privacy" â "General" â "Open
 anyway". You might also need to allow NormCap to take screenshots. [#135]
 (https://github.com/dynobo/normcap/issues/135)
 2: Might be available a bit delayed, as it is currently build manually. (Thx,
 [@Takrin](https://github.com/Takrin)!) Install from repositories: -
 **Windows**: Install from [Microsoft Store](https://apps.microsoft.com/store/
 detail/normcap/XPDLJNB4B6C2ZR). - **Arch / Manjaro**: Install the [`normcap`]
@@ -68,22 +68,21 @@
 Prerequisites for setting up a development environment are: **Python >=3.9**,
 **Poetry>=1.3.2** and **Tesseract** (incl. **language data**). ```sh # Clone
 repository git clone https://github.com/dynobo/normcap.git # Change into
 project directory cd normcap # Create virtual env and install dependencies
 poetry install # Register pre-commit hook poetry run pre-commit install # Run
 NormCap in virtual env poetry run python -m normcap ``` ## Credits This project
 uses the following non-standard libraries: - [pyside6](https://pypi.org/
-project/PySide6/) _- bindings for Qt UI Framework_ - [jeepney](https://
-pypi.org/project/jeepney/) _- DBUS client_ And it depends on external software:
-- [tesseract](https://github.com/tesseract-ocr/tesseract) - _OCR engine_ - [wl-
-clipboard](https://github.com/bugaevc/wl-clipboard) - _Wayland clipboard
-utilities_ Packaging is done with: - [briefcase](https://pypi.org/project/
-briefcase/) _- converting Python projects into_ _standalone apps_ Thanks to the
-maintainers of those nice tools! ## Similar open source tools If NormCap
-doesn't fit your needs, try those alternatives (no particular order): -
+project/PySide6/) _- bindings for Qt UI Framework_ And it depends on external
+software: - [tesseract](https://github.com/tesseract-ocr/tesseract) - _OCR
+engine_ - [wl-clipboard](https://github.com/bugaevc/wl-clipboard) - _Wayland
+clipboard utilities_ Packaging is done with: - [briefcase](https://pypi.org/
+project/briefcase/) _- converting Python projects into_ _standalone apps_
+Thanks to the maintainers of those nice tools! ## Similar open source tools If
+NormCap doesn't fit your needs, try those alternatives (no particular order): -
 [TextSnatcher](https://github.com/RajSolai/TextSnatcher) (Linux) - [GreenShot]
 (https://getgreenshot.org/) (Linux, macOS) - [TextShot](https://github.com/
 ianzhao05/textshot) (Windows) - [gImageReader](https://github.com/manisandro/
 gImageReader) (Linux, Windows) - [Capture2Text](https://sourceforge.net/
 projects/capture2text) (Windows) - [Frog](https://github.com/TenderOwl/Frog)
 (Linux) - [Textinator](https://github.com/RhetTbull/textinator) (macOS) -
 [Text-Grab](https://github.com/TheJoeFin/Text-Grab) (Windows) - [dpScreenOCR]
```

### Comparing `normcap-0.4.1/normcap/app.py` & `normcap-0.4.2/normcap/app.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/clipboard/macos.py` & `normcap-0.4.2/normcap/clipboard/macos.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/clipboard/windows.py` & `normcap-0.4.2/normcap/clipboard/windows.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/gui/constants.py` & `normcap-0.4.2/normcap/gui/constants.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/gui/downloader.py` & `normcap-0.4.2/normcap/gui/downloader.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/gui/language_manager.py` & `normcap-0.4.2/normcap/gui/language_manager.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/gui/loading_indicator.py` & `normcap-0.4.2/normcap/gui/loading_indicator.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/gui/menu_button.py` & `normcap-0.4.2/normcap/gui/menu_button.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,17 @@
         radius: 0.55,
         stop: 0 rgba(0,0,0,0) stop: 0.25 rgba(255,255,255,120) stop: 0.95 rgba(0,0,0,0)
     );
 }
 QToolButton::menu-indicator { image: none; }
 """
 
+# TODO: Add translations
+# https://doc.qt.io/qtforpython-6/tutorials/basictutorial/translations.html
+
 
 class Communicate(QtCore.QObject):
     """SettingsMenu' communication bus."""
 
     on_open_url = QtCore.Signal(str)
     on_close_in_settings = QtCore.Signal(str)
     on_manage_languages = QtCore.Signal()
```

### Comparing `normcap-0.4.1/normcap/gui/models.py` & `normcap-0.4.2/normcap/gui/models.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/gui/notifier.py` & `normcap-0.4.2/normcap/gui/notifier.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/gui/resources.py` & `normcap-0.4.2/normcap/gui/resources.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/gui/settings.py` & `normcap-0.4.2/normcap/gui/settings.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/gui/system_info.py` & `normcap-0.4.2/normcap/gui/system_info.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/gui/tray.py` & `normcap-0.4.2/normcap/gui/tray.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from normcap.gui.update_check import UpdateChecker
 from normcap.gui.window import Window
 
 logger = logging.getLogger(__name__)
 
 UPDATE_CHECK_INTERVAL_DAYS = 7
 
+# TODO: Add tutorial screen
+
 
 class Communicate(QtCore.QObject):
     """TrayMenus' communication bus."""
 
     on_close_or_exit = QtCore.Signal(str)
     on_copied_to_clipboard = QtCore.Signal()
     on_image_cropped = QtCore.Signal()
```

### Comparing `normcap-0.4.1/normcap/gui/update_check.py` & `normcap-0.4.2/normcap/gui/update_check.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/gui/utils.py` & `normcap-0.4.2/normcap/gui/utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/gui/window.py` & `normcap-0.4.2/normcap/gui/window.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/ocr/enhance.py` & `normcap-0.4.2/normcap/ocr/enhance.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/ocr/magics/base_magic.py` & `normcap-0.4.2/normcap/ocr/magics/base_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/ocr/magics/email_magic.py` & `normcap-0.4.2/normcap/ocr/magics/email_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/ocr/magics/magic.py` & `normcap-0.4.2/normcap/ocr/magics/magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/ocr/magics/multi_line_magic.py` & `normcap-0.4.2/normcap/ocr/magics/multi_line_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/ocr/magics/paragraph_magic.py` & `normcap-0.4.2/normcap/ocr/magics/paragraph_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/ocr/magics/single_line_magic.py` & `normcap-0.4.2/normcap/ocr/magics/single_line_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/ocr/magics/url_magic.py` & `normcap-0.4.2/normcap/ocr/magics/url_magic.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/ocr/models.py` & `normcap-0.4.2/normcap/ocr/models.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/ocr/recognize.py` & `normcap-0.4.2/normcap/ocr/recognize.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/ocr/tesseract.py` & `normcap-0.4.2/normcap/ocr/tesseract.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             input_image_path,  # will be suffixed with .tsv
             "-c",
             "tessedit_create_tsv=1",
             *args,
         ]
         _ = _run_command(cmd_args=cmd_args)
         with Path(output_tsv_path).open() as fh:
-            tsv_file = csv.reader(fh, delimiter="\t")
+            tsv_file = csv.reader(fh, delimiter="\t", quotechar=None)
             lines = list(tsv_file)
     finally:
         Path(input_image_path).unlink(missing_ok=True)
         Path(output_tsv_path).unlink(missing_ok=True)
 
     return lines
```

### Comparing `normcap-0.4.1/normcap/resources/icons/normcap.png` & `normcap-0.4.2/normcap/resources/icons/normcap.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/icons/normcap.svg` & `normcap-0.4.2/normcap/resources/icons/normcap.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/icons/notification.png` & `normcap-0.4.2/normcap/resources/icons/notification.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/icons/notification.svg` & `normcap-0.4.2/normcap/resources/icons/notification.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/icons/parse.png` & `normcap-0.4.2/normcap/resources/icons/parse.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/icons/parse.svg` & `normcap-0.4.2/normcap/resources/icons/parse.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/icons/raw.png` & `normcap-0.4.2/normcap/resources/icons/raw.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/icons/raw.svg` & `normcap-0.4.2/normcap/resources/icons/raw.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/icons/resources.qrc` & `normcap-0.4.2/normcap/resources/icons/resources.qrc`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/icons/settings.png` & `normcap-0.4.2/normcap/resources/icons/settings.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/icons/settings.svg` & `normcap-0.4.2/normcap/resources/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/icons/tray.png` & `normcap-0.4.2/normcap/resources/icons/tray.png`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/icons/tray.svg` & `normcap-0.4.2/normcap/resources/icons/tray.svg`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/tessdata/LICENSE.txt` & `normcap-0.4.2/normcap/resources/tessdata/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/resources/tessdata/README.txt` & `normcap-0.4.2/normcap/resources/tessdata/README.txt`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/screengrab/__init__.py` & `normcap-0.4.2/normcap/screengrab/dbus_shell.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,64 @@
-import logging
-import sys
-from typing import Callable
-
-from normcap.screengrab import utils
-from normcap.screengrab.utils import (
-    has_screenshot_permission,
-    macos_open_privacy_settings,
-    macos_request_screenshot_permission,
-    macos_reset_screenshot_permission,
-)
-
-
-class ScreenshotError(Exception):
-    ...
+"""Capture screenshot of all screens using DBUS org.gnome.Shell.Screenshot."""
 
+import logging
+import os
+import tempfile
+from pathlib import Path
+from typing import Union
 
-class ScreenshotResponseError(ScreenshotError):
-    ...
+from PySide6 import QtGui
 
+try:
+    from PySide6 import QtDBus
 
-class ScreenshotRequestError(ScreenshotError):
-    ...
+    HAS_QTDBUS = True
+except ImportError:
+    HAS_QTDBUS = False
 
+from normcap.screengrab.utils import split_full_desktop_to_screens
 
 logger = logging.getLogger(__name__)
 
 
-def _is_pyside6_64plus() -> bool:
-    import PySide6
-
-    version_tuple = PySide6.__version__.split(".")
-    return version_tuple[0] >= "6" and version_tuple[1] >= "4"
-
+def _get_screenshot_interface():  # noqa: ANN202
+    if not HAS_QTDBUS:
+        raise ModuleNotFoundError("QtDBUS not available.")
+
+    item = "org.gnome.Shell.Screenshot"
+    interface = "org.gnome.Shell.Screenshot"
+    path = "/org/gnome/Shell/Screenshot"
+
+    bus = QtDBus.QDBusConnection.sessionBus()
+    if not bus.isConnected():
+        logger.error("Not connected to dbus!")
+    return QtDBus.QDBusInterface(item, path, interface, bus)
+
+
+def _fullscreen_to_file(filename: Union[os.PathLike, str]) -> None:
+    """Capture full screen and store it in file."""
+    if not HAS_QTDBUS:
+        raise ModuleNotFoundError("QtDBUS not available.")
+
+    screenshot_interface = _get_screenshot_interface()
+    if screenshot_interface.isValid():
+        x = screenshot_interface.call("Screenshot", True, False, filename)
+        if x.errorName():
+            logger.error("Failed move Window!")
+            logger.error(x.errorMessage())
+    else:
+        logger.error("Invalid dbus interface")
+
+
+def capture() -> list[QtGui.QImage]:
+    """Capture screenshots for all screens using org.gnome.Shell.Screenshot.
+
+    This methods works gnome-shell < v41 and wayland.
+    """
+    _, temp_file = tempfile.mkstemp(prefix="normcap")
+    try:
+        _fullscreen_to_file(temp_file)
+        image = QtGui.QImage(temp_file)
+    finally:
+        Path(temp_file).unlink()
 
-def get_capture_func() -> Callable:
-    # fmt: off
-    if sys.platform != "linux" or not utils.has_wayland_display_manager():
-        logger.debug("Select capture method QT")
-        from normcap.screengrab import qt
-        return qt.capture
-
-    if utils.has_dbus_portal_support():
-        if _is_pyside6_64plus():
-            logger.debug("Select capture method DBUS portal")
-            from normcap.screengrab import dbus_portal
-            return dbus_portal.capture
-
-        logger.debug("Select capture method DBUS portal legacy")
-        from normcap.screengrab import dbus_portal_legacy
-        return dbus_portal_legacy.capture
-
-    logger.debug("Select capture method DBUS shell")
-    from normcap.screengrab import dbus_shell
-
-    return dbus_shell.capture
-    # fmt: on
-
-
-__all__ = [
-    "has_screenshot_permission",
-    "macos_open_privacy_settings",
-    "macos_request_screenshot_permission",
-    "macos_reset_screenshot_permission",
-    "get_capture_func",
-]
+    return split_full_desktop_to_screens(image)
```

### Comparing `normcap-0.4.1/normcap/screengrab/dbus_portal.py` & `normcap-0.4.2/normcap/screengrab/dbus_portal.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/screengrab/utils.py` & `normcap-0.4.2/normcap/screengrab/utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/normcap/utils.py` & `normcap-0.4.2/normcap/utils.py`

 * *Files identical despite different names*

### Comparing `normcap-0.4.1/pyproject.toml` & `normcap-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "normcap"
-version = "0.4.1"
+version = "0.4.2"
 description = "OCR-powered screen-capture tool to capture information instead of images."
 keywords = ["screenshot", "ocr", "capture", "clipboard"]
 license = "GPLv3"
 authors = ["dynobo <dynobo@mailbox.org>"]
 readme = "README.md"
 homepage = "https://dynobo.github.io/normcap/"
 repository = "https://github.com/dynobo/normcap"
@@ -42,45 +42,43 @@
 
 [tool.poetry.scripts]
 normcap = "normcap.app:main"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 PySide6-Essentials = "6.4.2"
-jeepney = "^0.8.0"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.1.0"
 briefcase = "0.3.14"
 coverage = { extras = ["toml"], version = "^6.4.2" }
 coveralls = ">=3.3.1"
-Levenshtein = ">=0.20.1"
 mdformat-gfm = ">=0.3.5"
-mypy = ">=0.991"
+mypy = ">=1.3.0"
 pre-commit = ">=3.0.2"
 pydeps = ">=1.11.0"
 pytest = ">=7.2.1"
 pytest-cov = ">=4.0.0"
 pytest-qt = ">=4.2.0"
 pytest-xvfb = "^2.0.0"
 rope = ">=1.7.0"
 ruff = ">=0.0.239"
 tbump = ">=6.9.0"
 toml = ">=0.10.2"
 types-toml = ">=0.10.8.1"
-typing-extensions = "^4.4.0"
-pip-audit = "^2.4.14"
+typing-extensions = ">=4.4.0"
+pip-audit = ">=2.5.5"
 
 [tool.poetry.group.analysis]
 optional = true
 
 [tool.poetry.group.analysis.dependencies]
 radon = ">=5.1.0"
 viztracer = ">=0.15.3"
-vulture = "^2.4"
+vulture = ">=2.4"
 
 [tool.black]
 line-length = 88
 include = '''
 (
     ^/tests/.*py
   | ^/normcap/.*py
@@ -150,93 +148,72 @@
   "gui: tests which require a graphical interface to run",
   "skip_on_gh: tests which are not supported during CI/CD on github",
 ]
 
 [tool.coverage.run]
 source = ["normcap"]
 
+[tool.pydeps]
+cluster = true
+max_cluster_size = 1
+no_show = true
+
 [tool.briefcase]
 project_name = "NormCap"
 bundle = "eu.dynobo"
-version = "0.4.1"
+version = "0.4.2"
 url = "https://github.com/dynobo/normcap"
 license = "GPLv3"
 author = 'dynobo'
 author_email = "dynobo@mailbox.org"
 
 [tool.briefcase.app.normcap]
 formal_name = "NormCap"
 description = "OCR-powered screen-capture tool to capture information instead of images"
 sources = ["normcap"]
 icon = "bundle/imgs/normcap"
 installer_icon = "bundle/imgs/normcap_install"
 installer_background = "bundle/imgs/normcap_install_bg"
-# ONHOLD: Switch to pyside6-essentials, once build works with Ubuntu 20.04+
-requires = ["pyside6", "jeepney"]
+requires = ["PySide6-Essentials==6.4.2"]
 cleanup_paths = [
   # Globs
   "**/[pP]y[sS]ide6/*[qQ]t*[oO]pen[gG][lL]*",
   "**/*.debug",
-  "**/*[bB]odymovin*",
   "**/*[lL]abs*",
   "**/*[qQ]t[xX]ml*",
-  "**/*[qQ]t*[bB]luetooth*",
-  "**/*[qQ]t*[cC]harts*",
-  "**/*[qQ]t*[dD]ata[vV]isualization*",
   "**/*[qQ]t*[dD]esigner*",
   "**/*[qQ]t*[hH]elp*",
-  "**/*[qQ]t*[mM]ultimedia*",
-  "**/*[qQ]t*[pP]ositioning*",
   "**/*[qQ]t*[pP]df*",
   "**/*[qQ]t*[pP]rint[sS]upport*",
-  "**/*[qQ]t*[rR]emote[oO]bjects*",
-  "**/*[qQ]t*[sS]ensor*",
-  "**/*[qQ]t*[sS]erial*",
-  "**/*[qQ]t*[sS]hader[tT]ools*",
   "**/*[qQ]t*[sS]ql*",
   "**/*[qQ]t*[sS]tate[mM]achine*",
   "**/*[qQ]t*[tT]est*",
-  "**/*[qQ]t*[wW]eb[cC]hannel*",
-  "**/*[qQ]t*[wW]eb[eE]ngine*",
+  "**/*[qQ]t*[lL]anguage[sS]erver*",
   "**/*[qQ]t*[wW]eb[sS]ockets*",
-  "**/*[qQ]t*3[dD]*",
   "**/*[qQ]uick*",
   "**/*[sS]cene*",
-  "**/*[sS]cxml*",
   "**/*[uU]i[tT]ools*",
   "**/*[vV]irtual[kK]eyboard*",
-  "**/*[wW]eb[vV]iew*",
   "**/*QtQml*",
   "**/bin/pyside6-*",
-  "**/libQt6Nfc*",
-  "**/render*",
   "**/PySide6/[aA]ssistant*",
   "**/PySide6/[dD]esigner*",
   "**/PySide6/[lL]inguist*",
   # Folders
   "**/__pycache__",
-  "**/docs",
-  "**/examples",
   "**/libexec",
-  "**/plugins/assetimporters",
-  "**/plugins/canbus",
   "**/plugins/designer",
   "**/plugins/printsupport",
   "**/plugins/qmltooling",
-  "**/plugins/sceneparsers",
-  "**/plugins/sensors",
   "**/plugins/sqldrivers",
-  "**/PySide6/Examples",
   "**/Qt/qml/QtQml",
-  "**/Qt/resources",
   "**/Qt/translations",
   "**/tests",
   "**/typesystems",
   # Files
-  "**/icudtl.dat",
   "**/PySide6/lrelease",
   "**/PySide6/lupdate",
 ]
 [tool.briefcase.app.normcap.macOS]
 requires = ["std-nslog==1.0.0"]
 
 [tool.briefcase.app.normcap.linux]
@@ -247,51 +224,50 @@
   "build-essential",
   "libtiff-dev",
   "libpng-dev",
   "libjpeg-dev",
   "libfuse2",
   "libwayland-dev",
   "wayland-protocols",
-  "meson",
-  "git",
   "software-properties-common", # required for apt-add-repository
-  # "wl-clipboard", Only available on Ubuntu 20.04+
+  "wl-clipboard",
 ]
 dockerfile_extra_content = """
 USER root
 
 # Upgrade Tesseract 4 to 5
-RUN apt-add-repository ppa:alex-p/tesseract-ocr-devel
-RUN apt-get update -y && apt-get upgrade --with-new-pkgs -y
-
-# Build wl-clipboard
-RUN git clone https://github.com/bugaevc/wl-clipboard.git
-RUN meson build wl-clipboard && ninja -C build
-RUN mv build/src/wl-copy /usr/bin/ && rm -rf wl-clipboard
+RUN apt-add-repository ppa:alex-p/tesseract-ocr-devel \
+  && apt-get update -y \
+  && apt-get upgrade --with-new-pkgs -y \
+  && apt-get autoremove -y
 
 USER brutus
 """
 
+[tool.briefcase.app.normcap.linux.appimage]
+template = "https://github.com/dynobo/briefcase-linux-appimage-template"
+template_branch = "main"
+
 [tool.briefcase.app.normcap.windows]
 
 [tool.tbump]
 
 [tool.tbump.version]
-current = "0.4.1"
+current = "0.4.2"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   ((?P<extra>.+))?
   '''
 
 [tool.tbump.git]
-message_template = "Bump to {new_version}"
+message_template = "build(release): bump to {new_version}"
 tag_template = "v{new_version}"
 
 [[tool.tbump.file]]
 # Poetry version and Briefcase version
 src = "pyproject.toml"
 search = 'version = "{current_version}"'
```

### Comparing `normcap-0.4.1/setup.py` & `normcap-0.4.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,24 +10,24 @@
  'normcap.resources',
  'normcap.screengrab']
 
 package_data = \
 {'': ['*'], 'normcap.resources': ['icons/*', 'tessdata/*']}
 
 install_requires = \
-['PySide6-Essentials==6.4.2', 'jeepney>=0.8.0,<0.9.0']
+['PySide6-Essentials==6.4.2']
 
 entry_points = \
 {'console_scripts': ['normcap = normcap.app:main']}
 
 setup_kwargs = {
     'name': 'normcap',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'OCR-powered screen-capture tool to capture information instead of images.',
-    'long_description': '<!-- markdownlint-disable MD013 MD026 MD033 -->\n\n# NormCap\n\n**_OCR powered screen-capture tool to capture information instead of images. For Linux,\nmacOS and Windows._**\n\n[![Build](https://img.shields.io/github/actions/workflow/status/dynobo/normcap/python.yaml?branch=main)](https://github.com/dynobo/normcap/releases)\n[![Coverage Status](https://img.shields.io/coverallsCoverage/github/dynobo/normcap?label=Test%20coverage&branch=main)](https://coveralls.io/github/dynobo/normcap)\n[![CodeQL](https://img.shields.io/github/actions/workflow/status/dynobo/normcap/codeql-analysis.yml?branch=main&label=CodeQL)](https://github.com/dynobo/normcap/actions/workflows/codeql-analysis.yml)\n\n[![GitHub](https://img.shields.io/github/downloads/dynobo/normcap/total?label=Github%20downloads&color=blue)](https://github.com/dynobo/normcap/releases)\n[![PyPi](https://img.shields.io/pypi/dm/normcap?label=PyPi%20downloads&color=blue)](https://pypi.org/project/normcap)\n[![Flathub](https://img.shields.io/flathub/downloads/com.github.dynobo.normcap?label=Flathub%20downloads&color=blue)](https://flathub.org/apps/details/com.github.dynobo.normcap)\n[![AUR](https://img.shields.io/aur/votes/normcap?label=AUR%20votes&color=blue)](https://aur.archlinux.org/packages/normcap)\n\n<a href="https://www.buymeacoffee.com/dynobo" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 40px !important;" ></a>\n\n**Links:** [Source Code](https://github.com/dynobo/normcap) |\n[Documentation](https://dynobo.github.io/normcap/) |\n[FAQs](https://dynobo.github.io/normcap/#faqs) |\n[Releases](https://github.com/dynobo/normcap/releases) |\n[Changelog](https://github.com/dynobo/normcap/blob/main/CHANGELOG)\n\n[![Screencast](https://user-images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/assets/normcap.gif)\n\n## Quickstart\n\nInstall a prebuilt release:\n\n- **Windows**:\n  [NormCap-0.4.1-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-0.4.1-x86_64-Windows.msi)\n- **Linux**:\n  [NormCap-0.4.1-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-0.4.1-x86_64.AppImage)\n- **macOS** (x86) ¹:\n  [NormCap-0.4.1-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-0.4.1-x86_64-macOS.dmg)\n- **macOS** (M1) ¹·²:\n  [NormCap-0.4.1-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-0.4.1-arm64-macOS.dmg)\n  \\\n  <sub>1: On macOS, allow the unsigned application on first start: "System\n  Preferences" → "Security & Privacy" → "General" → "Open anyway". You might also need\n  to allow NormCap to take screenshots.\n  [#135](https://github.com/dynobo/normcap/issues/135)<br> 2: Might be available a bit\n  delayed, as it is currently build manually. (Thx,\n  [@Takrin](https://github.com/Takrin)!)</sub>\n\nInstall from repositories:\n\n- **Windows**: Install from\n  [Microsoft Store](https://apps.microsoft.com/store/detail/normcap/XPDLJNB4B6C2ZR).\n- **Arch / Manjaro**: Install the\n  [`normcap`](https://aur.archlinux.org/packages/normcap) package from AUR.\n- **FlatPak (Linux)**: Install\n  [com.github.dynobo.normcap](https://flathub.org/apps/details/com.github.dynobo.normcap)\n  from FlatHub.\n\nIf you experience issues please look at the\n[FAQs](https://dynobo.github.io/normcap/#faqs) or\n[open an issue](https://github.com/dynobo/normcap/issues).\n\n## Python package\n\nAs an _alternative_ to a prebuilt package you can install the\n[NormCap Python package](https://pypi.org/project/normcap/) for **Python >=3.9**:\n\n#### On Linux\n\n```sh\n# Install dependencies (Ubuntu/Debian)\nsudo apt install build-essential tesseract-ocr tesseract-ocr-eng libtesseract-dev libleptonica-dev wl-clipboard\n\n## Install dependencies (Arch)\nsudo pacman -S tesseract tesseract-data-eng wl-clipboard\n\n## Install dependencies (Fedora)\nsudo dnf install tesseract wl-clipboard\n\n## Install dependencies (openSUSE)\nsudo zypper install python3-devel tesseract-ocr tesseract-ocr-devel wl-clipboard\n\n# Install normcap\npip install normcap\n\n# Run\n./normcap\n```\n\n#### On macOS\n\n```sh\n# Install dependencies\nbrew install tesseract tesseract-lang\n\n# Install normcap\npip install normcap\n\n# Run\n./normcap\n```\n\n#### On Windows\n\n1\\. Install `Tesseract 5` by using the\n[installer provided by UB Mannheim](https://github.com/UB-Mannheim/tesseract/wiki).\n\n2\\. Adjust environment variables:\n\n- Create an environment variable `TESSDATA_PREFIX` and set it to Tesseract\'s data\n  folder, e.g.:\n\n  ```cmd\n  setx TESSDATA_PREFIX "C:\\Program Files\\Tesseract-OCR\\tessdata"\n  ```\n\n- Append Tesseract\'s location to the environment variable `Path`, e.g.:\n\n  ```cmd\n  setx Path "%Path%;C:\\Program Files\\Tesseract-OCR"\n  ```\n\n- Make sure to close and reopen your current terminal window to apply the new variables.\n  Test it by running:\n\n  ```cmd\n  tesseract --list-langs\n  ```\n\n3\\. Install and run NormCap:\n\n```bash\n# Install normcap\npip install normcap\n\n# Run\nnormcap\n```\n\n## Why "NormCap"?\n\nSee [XKCD](https://xkcd.com):\n\n[![Comic](https://imgs.xkcd.com/comics/norm_normal_file_format.png)](https://xkcd.com/2116/)\n\n## Development\n\nPrerequisites for setting up a development environment are: **Python >=3.9**,\n**Poetry>=1.3.2** and **Tesseract** (incl. **language data**).\n\n```sh\n# Clone repository\ngit clone https://github.com/dynobo/normcap.git\n\n# Change into project directory\ncd normcap\n\n# Create virtual env and install dependencies\npoetry install\n\n# Register pre-commit hook\npoetry run pre-commit install\n\n# Run NormCap in virtual env\npoetry run python -m normcap\n```\n\n## Credits\n\nThis project uses the following non-standard libraries:\n\n- [pyside6](https://pypi.org/project/PySide6/) _- bindings for Qt UI Framework_\n- [jeepney](https://pypi.org/project/jeepney/) _- DBUS client_\n\nAnd it depends on external software:\n\n- [tesseract](https://github.com/tesseract-ocr/tesseract) - _OCR engine_\n- [wl-clipboard](https://github.com/bugaevc/wl-clipboard) - _Wayland clipboard\n  utilities_\n\nPackaging is done with:\n\n- [briefcase](https://pypi.org/project/briefcase/) _- converting Python projects into_\n  _standalone apps_\n\nThanks to the maintainers of those nice tools!\n\n## Similar open source tools\n\nIf NormCap doesn\'t fit your needs, try those alternatives (no particular order):\n\n- [TextSnatcher](https://github.com/RajSolai/TextSnatcher) (Linux)\n- [GreenShot](https://getgreenshot.org/) (Linux, macOS)\n- [TextShot](https://github.com/ianzhao05/textshot) (Windows)\n- [gImageReader](https://github.com/manisandro/gImageReader) (Linux, Windows)\n- [Capture2Text](https://sourceforge.net/projects/capture2text) (Windows)\n- [Frog](https://github.com/TenderOwl/Frog) (Linux)\n- [Textinator](https://github.com/RhetTbull/textinator) (macOS)\n- [Text-Grab](https://github.com/TheJoeFin/Text-Grab) (Windows)\n- [dpScreenOCR](https://danpla.github.io/dpscreenocr/) (Linux, Windows)\n\n## Certification\n\n![WOMM](https://raw.githubusercontent.com/dynobo/lmdiag/master/badge.png)\n',
+    'long_description': '<!-- markdownlint-disable MD013 MD026 MD033 -->\n\n# NormCap\n\n**_OCR powered screen-capture tool to capture information instead of images. For Linux,\nmacOS and Windows._**\n\n[![Build](https://img.shields.io/github/actions/workflow/status/dynobo/normcap/python.yaml?branch=main)](https://github.com/dynobo/normcap/releases)\n[![Coverage Status](https://img.shields.io/coverallsCoverage/github/dynobo/normcap?label=Test%20coverage&branch=main)](https://coveralls.io/github/dynobo/normcap)\n[![CodeQL](https://img.shields.io/github/actions/workflow/status/dynobo/normcap/codeql-analysis.yml?branch=main&label=CodeQL)](https://github.com/dynobo/normcap/actions/workflows/codeql-analysis.yml)\n\n[![GitHub](https://img.shields.io/github/downloads/dynobo/normcap/total?label=Github%20downloads&color=blue)](https://github.com/dynobo/normcap/releases)\n[![PyPi](https://img.shields.io/pypi/dm/normcap?label=PyPi%20downloads&color=blue)](https://pypi.org/project/normcap)\n[![Flathub](https://img.shields.io/flathub/downloads/com.github.dynobo.normcap?label=Flathub%20downloads&color=blue)](https://flathub.org/apps/details/com.github.dynobo.normcap)\n[![AUR](https://img.shields.io/aur/votes/normcap?label=AUR%20votes&color=blue)](https://aur.archlinux.org/packages/normcap)\n\n<a href="https://www.buymeacoffee.com/dynobo" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 40px !important;" ></a>\n\n**Links:** [Source Code](https://github.com/dynobo/normcap) |\n[Documentation](https://dynobo.github.io/normcap/) |\n[FAQs](https://dynobo.github.io/normcap/#faqs) |\n[Releases](https://github.com/dynobo/normcap/releases) |\n[Changelog](https://github.com/dynobo/normcap/blob/main/CHANGELOG)\n\n[![Screencast](https://user-images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/assets/normcap.gif)\n\n## Quickstart\n\nInstall a prebuilt release:\n\n- **Windows**:\n  [NormCap-0.4.2-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64-Windows.msi)\n- **Linux**:\n  [NormCap-0.4.2-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64.AppImage)\n- **macOS** (x86) ¹:\n  [NormCap-0.4.2-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64-macOS.dmg)\n- **macOS** (M1) ¹·²:\n  [NormCap-0.4.2-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-arm64-macOS.dmg)\n  \\\n  <sub>1: On macOS, allow the unsigned application on first start: "System\n  Preferences" → "Security & Privacy" → "General" → "Open anyway". You might also need\n  to allow NormCap to take screenshots.\n  [#135](https://github.com/dynobo/normcap/issues/135)<br> 2: Might be available a bit\n  delayed, as it is currently build manually. (Thx,\n  [@Takrin](https://github.com/Takrin)!)</sub>\n\nInstall from repositories:\n\n- **Windows**: Install from\n  [Microsoft Store](https://apps.microsoft.com/store/detail/normcap/XPDLJNB4B6C2ZR).\n- **Arch / Manjaro**: Install the\n  [`normcap`](https://aur.archlinux.org/packages/normcap) package from AUR.\n- **FlatPak (Linux)**: Install\n  [com.github.dynobo.normcap](https://flathub.org/apps/details/com.github.dynobo.normcap)\n  from FlatHub.\n\nIf you experience issues please look at the\n[FAQs](https://dynobo.github.io/normcap/#faqs) or\n[open an issue](https://github.com/dynobo/normcap/issues).\n\n## Python package\n\nAs an _alternative_ to a prebuilt package you can install the\n[NormCap Python package](https://pypi.org/project/normcap/) for **Python >=3.9**:\n\n#### On Linux\n\n```sh\n# Install dependencies (Ubuntu/Debian)\nsudo apt install build-essential tesseract-ocr tesseract-ocr-eng libtesseract-dev libleptonica-dev wl-clipboard\n\n## Install dependencies (Arch)\nsudo pacman -S tesseract tesseract-data-eng wl-clipboard\n\n## Install dependencies (Fedora)\nsudo dnf install tesseract wl-clipboard\n\n## Install dependencies (openSUSE)\nsudo zypper install python3-devel tesseract-ocr tesseract-ocr-devel wl-clipboard\n\n# Install normcap\npip install normcap\n\n# Run\n./normcap\n```\n\n#### On macOS\n\n```sh\n# Install dependencies\nbrew install tesseract tesseract-lang\n\n# Install normcap\npip install normcap\n\n# Run\n./normcap\n```\n\n#### On Windows\n\n1\\. Install `Tesseract 5` by using the\n[installer provided by UB Mannheim](https://github.com/UB-Mannheim/tesseract/wiki).\n\n2\\. Adjust environment variables:\n\n- Create an environment variable `TESSDATA_PREFIX` and set it to Tesseract\'s data\n  folder, e.g.:\n\n  ```cmd\n  setx TESSDATA_PREFIX "C:\\Program Files\\Tesseract-OCR\\tessdata"\n  ```\n\n- Append Tesseract\'s location to the environment variable `Path`, e.g.:\n\n  ```cmd\n  setx Path "%Path%;C:\\Program Files\\Tesseract-OCR"\n  ```\n\n- Make sure to close and reopen your current terminal window to apply the new variables.\n  Test it by running:\n\n  ```cmd\n  tesseract --list-langs\n  ```\n\n3\\. Install and run NormCap:\n\n```bash\n# Install normcap\npip install normcap\n\n# Run\nnormcap\n```\n\n## Why "NormCap"?\n\nSee [XKCD](https://xkcd.com):\n\n[![Comic](https://imgs.xkcd.com/comics/norm_normal_file_format.png)](https://xkcd.com/2116/)\n\n## Development\n\nPrerequisites for setting up a development environment are: **Python >=3.9**,\n**Poetry>=1.3.2** and **Tesseract** (incl. **language data**).\n\n```sh\n# Clone repository\ngit clone https://github.com/dynobo/normcap.git\n\n# Change into project directory\ncd normcap\n\n# Create virtual env and install dependencies\npoetry install\n\n# Register pre-commit hook\npoetry run pre-commit install\n\n# Run NormCap in virtual env\npoetry run python -m normcap\n```\n\n## Credits\n\nThis project uses the following non-standard libraries:\n\n- [pyside6](https://pypi.org/project/PySide6/) _- bindings for Qt UI Framework_\n\nAnd it depends on external software:\n\n- [tesseract](https://github.com/tesseract-ocr/tesseract) - _OCR engine_\n- [wl-clipboard](https://github.com/bugaevc/wl-clipboard) - _Wayland clipboard\n  utilities_\n\nPackaging is done with:\n\n- [briefcase](https://pypi.org/project/briefcase/) _- converting Python projects into_\n  _standalone apps_\n\nThanks to the maintainers of those nice tools!\n\n## Similar open source tools\n\nIf NormCap doesn\'t fit your needs, try those alternatives (no particular order):\n\n- [TextSnatcher](https://github.com/RajSolai/TextSnatcher) (Linux)\n- [GreenShot](https://getgreenshot.org/) (Linux, macOS)\n- [TextShot](https://github.com/ianzhao05/textshot) (Windows)\n- [gImageReader](https://github.com/manisandro/gImageReader) (Linux, Windows)\n- [Capture2Text](https://sourceforge.net/projects/capture2text) (Windows)\n- [Frog](https://github.com/TenderOwl/Frog) (Linux)\n- [Textinator](https://github.com/RhetTbull/textinator) (macOS)\n- [Text-Grab](https://github.com/TheJoeFin/Text-Grab) (Windows)\n- [dpScreenOCR](https://danpla.github.io/dpscreenocr/) (Linux, Windows)\n\n## Certification\n\n![WOMM](https://raw.githubusercontent.com/dynobo/lmdiag/master/badge.png)\n',
     'author': 'dynobo',
     'author_email': 'dynobo@mailbox.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://dynobo.github.io/normcap/',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['normcap',
 'normcap.clipboard', 'normcap.gui', 'normcap.ocr', 'normcap.ocr.magics',
 'normcap.resources', 'normcap.screengrab'] package_data = \ {'': ['*'],
 'normcap.resources': ['icons/*', 'tessdata/*']} install_requires = \ ['PySide6-
-Essentials==6.4.2', 'jeepney>=0.8.0,<0.9.0'] entry_points = \
-{'console_scripts': ['normcap = normcap.app:main']} setup_kwargs = { 'name':
-'normcap', 'version': '0.4.1', 'description': 'OCR-powered screen-capture tool
-to capture information instead of images.', 'long_description': '\n\n#
-NormCap\n\n**_OCR powered screen-capture tool to capture information instead of
-images. For Linux,\nmacOS and Windows._**\n\n[![Build](https://img.shields.io/
-github/actions/workflow/status/dynobo/normcap/python.yaml?branch=main)](https:/
-/github.com/dynobo/normcap/releases)\n[![Coverage Status](https://
-img.shields.io/coverallsCoverage/github/dynobo/
-normcap?label=Test%20coverage&branch=main)](https://coveralls.io/github/dynobo/
-normcap)\n[![CodeQL](https://img.shields.io/github/actions/workflow/status/
-dynobo/normcap/codeql-analysis.yml?branch=main&label=CodeQL)](https://
+Essentials==6.4.2'] entry_points = \ {'console_scripts': ['normcap =
+normcap.app:main']} setup_kwargs = { 'name': 'normcap', 'version': '0.4.2',
+'description': 'OCR-powered screen-capture tool to capture information instead
+of images.', 'long_description': '\n\n# NormCap\n\n**_OCR powered screen-
+capture tool to capture information instead of images. For Linux,\nmacOS and
+Windows._**\n\n[![Build](https://img.shields.io/github/actions/workflow/status/
+dynobo/normcap/python.yaml?branch=main)](https://github.com/dynobo/normcap/
+releases)\n[![Coverage Status](https://img.shields.io/coverallsCoverage/github/
+dynobo/normcap?label=Test%20coverage&branch=main)](https://coveralls.io/github/
+dynobo/normcap)\n[![CodeQL](https://img.shields.io/github/actions/workflow/
+status/dynobo/normcap/codeql-analysis.yml?branch=main&label=CodeQL)](https://
 github.com/dynobo/normcap/actions/workflows/codeql-analysis.yml)\n\n[![GitHub]
 (https://img.shields.io/github/downloads/dynobo/normcap/
 total?label=Github%20downloads&color=blue)](https://github.com/dynobo/normcap/
 releases)\n[![PyPi](https://img.shields.io/pypi/dm/
 normcap?label=PyPi%20downloads&color=blue)](https://pypi.org/project/normcap)\n
 [![Flathub](https://img.shields.io/flathub/downloads/
 com.github.dynobo.normcap?label=Flathub%20downloads&color=blue)](https://
@@ -27,22 +26,22 @@
 Code](https://github.com/dynobo/normcap) |\n[Documentation](https://
 dynobo.github.io/normcap/) |\n[FAQs](https://dynobo.github.io/normcap/#faqs)
 |\n[Releases](https://github.com/dynobo/normcap/releases) |\n[Changelog](https:
 //github.com/dynobo/normcap/blob/main/CHANGELOG)\n\n[![Screencast](https://
 user-images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-
 cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/
 assets/normcap.gif)\n\n## Quickstart\n\nInstall a prebuilt release:\n\n-
-**Windows**:\n [NormCap-0.4.1-x86_64-Windows.msi](https://github.com/dynobo/
-normcap/releases/download/v0.4.1/NormCap-0.4.1-x86_64-Windows.msi)\n-
-**Linux**:\n [NormCap-0.4.1-x86_64.AppImage](https://github.com/dynobo/normcap/
-releases/download/v0.4.1/NormCap-0.4.1-x86_64.AppImage)\n- **macOS** (x86) Â¹:
-\n [NormCap-0.4.1-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/
-download/v0.4.1/NormCap-0.4.1-x86_64-macOS.dmg)\n- **macOS** (M1) Â¹Â·Â²:\n
-[NormCap-0.4.1-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/
-download/v0.4.1/NormCap-0.4.1-arm64-macOS.dmg)\n \\\n 1: On macOS, allow the
+**Windows**:\n [NormCap-0.4.2-x86_64-Windows.msi](https://github.com/dynobo/
+normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64-Windows.msi)\n-
+**Linux**:\n [NormCap-0.4.2-x86_64.AppImage](https://github.com/dynobo/normcap/
+releases/download/v0.4.2/NormCap-0.4.2-x86_64.AppImage)\n- **macOS** (x86) Â¹:
+\n [NormCap-0.4.2-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/
+download/v0.4.2/NormCap-0.4.2-x86_64-macOS.dmg)\n- **macOS** (M1) Â¹Â·Â²:\n
+[NormCap-0.4.2-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/
+download/v0.4.2/NormCap-0.4.2-arm64-macOS.dmg)\n \\\n 1: On macOS, allow the
 unsigned application on first start: "System\n Preferences" â "Security &
 Privacy" â "General" â "Open anyway". You might also need\n to allow
 NormCap to take screenshots.\n [#135](https://github.com/dynobo/normcap/issues/
 135)
 2: Might be available a bit\n delayed, as it is currently build manually.
 (Thx,\n [@Takrin](https://github.com/Takrin)!)\n\nInstall from repositories:
 \n\n- **Windows**: Install from\n [Microsoft Store](https://apps.microsoft.com/
@@ -80,18 +79,17 @@
 **Python >=3.9**,\n**Poetry>=1.3.2** and **Tesseract** (incl. **language
 data**).\n\n```sh\n# Clone repository\ngit clone https://github.com/dynobo/
 normcap.git\n\n# Change into project directory\ncd normcap\n\n# Create virtual
 env and install dependencies\npoetry install\n\n# Register pre-commit
 hook\npoetry run pre-commit install\n\n# Run NormCap in virtual env\npoetry run
 python -m normcap\n```\n\n## Credits\n\nThis project uses the following non-
 standard libraries:\n\n- [pyside6](https://pypi.org/project/PySide6/) _-
-bindings for Qt UI Framework_\n- [jeepney](https://pypi.org/project/jeepney/
-) _- DBUS client_\n\nAnd it depends on external software:\n\n- [tesseract]
-(https://github.com/tesseract-ocr/tesseract) - _OCR engine_\n- [wl-clipboard]
-(https://github.com/bugaevc/wl-clipboard) - _Wayland clipboard\n
+bindings for Qt UI Framework_\n\nAnd it depends on external software:\n\n-
+[tesseract](https://github.com/tesseract-ocr/tesseract) - _OCR engine_\n- [wl-
+clipboard](https://github.com/bugaevc/wl-clipboard) - _Wayland clipboard\n
 utilities_\n\nPackaging is done with:\n\n- [briefcase](https://pypi.org/
 project/briefcase/) _- converting Python projects into_\n _standalone
 apps_\n\nThanks to the maintainers of those nice tools!\n\n## Similar open
 source tools\n\nIf NormCap doesn\'t fit your needs, try those alternatives (no
 particular order):\n\n- [TextSnatcher](https://github.com/RajSolai/
 TextSnatcher) (Linux)\n- [GreenShot](https://getgreenshot.org/) (Linux,
 macOS)\n- [TextShot](https://github.com/ianzhao05/textshot) (Windows)\n-
```

### Comparing `normcap-0.4.1/PKG-INFO` & `normcap-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: normcap
-Version: 0.4.1
+Version: 0.4.2
 Summary: OCR-powered screen-capture tool to capture information instead of images.
 Home-page: https://dynobo.github.io/normcap/
 License: GPLv3
 Keywords: screenshot,ocr,capture,clipboard
 Author: dynobo
 Author-email: dynobo@mailbox.org
 Requires-Python: >=3.9,<3.12
@@ -22,15 +22,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Screen Capture
 Classifier: Topic :: Utilities
 Requires-Dist: PySide6-Essentials (==6.4.2)
-Requires-Dist: jeepney (>=0.8.0,<0.9.0)
 Project-URL: FAQs, https://dynobo.github.io/normcap/#faqs
 Project-URL: Issues, https://github.com/dynobo/normcap/issues
 Project-URL: Repository, https://github.com/dynobo/normcap
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD013 MD026 MD033 -->
 
@@ -59,21 +58,21 @@
 [![Screencast](https://user-images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/assets/normcap.gif)
 
 ## Quickstart
 
 Install a prebuilt release:
 
 - **Windows**:
-  [NormCap-0.4.1-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-0.4.1-x86_64-Windows.msi)
+  [NormCap-0.4.2-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64-Windows.msi)
 - **Linux**:
-  [NormCap-0.4.1-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-0.4.1-x86_64.AppImage)
+  [NormCap-0.4.2-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64.AppImage)
 - **macOS** (x86) ¹:
-  [NormCap-0.4.1-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-0.4.1-x86_64-macOS.dmg)
+  [NormCap-0.4.2-x86_64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-x86_64-macOS.dmg)
 - **macOS** (M1) ¹·²:
-  [NormCap-0.4.1-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-0.4.1-arm64-macOS.dmg)
+  [NormCap-0.4.2-arm64-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-0.4.2-arm64-macOS.dmg)
   \
   <sub>1: On macOS, allow the unsigned application on first start: "System
   Preferences" → "Security & Privacy" → "General" → "Open anyway". You might also need
   to allow NormCap to take screenshots.
   [#135](https://github.com/dynobo/normcap/issues/135)<br> 2: Might be available a bit
   delayed, as it is currently build manually. (Thx,
   [@Takrin](https://github.com/Takrin)!)</sub>
@@ -198,15 +197,14 @@
 ```
 
 ## Credits
 
 This project uses the following non-standard libraries:
 
 - [pyside6](https://pypi.org/project/PySide6/) _- bindings for Qt UI Framework_
-- [jeepney](https://pypi.org/project/jeepney/) _- DBUS client_
 
 And it depends on external software:
 
 - [tesseract](https://github.com/tesseract-ocr/tesseract) - _OCR engine_
 - [wl-clipboard](https://github.com/bugaevc/wl-clipboard) - _Wayland clipboard
   utilities_
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: normcap Version: 0.4.1 Summary: OCR-powered screen-
+Metadata-Version: 2.1 Name: normcap Version: 0.4.2 Summary: OCR-powered screen-
 capture tool to capture information instead of images. Home-page: https://
 dynobo.github.io/normcap/ License: GPLv3 Keywords:
 screenshot,ocr,capture,clipboard Author: dynobo Author-email:
 dynobo@mailbox.org Requires-Python: >=3.9,<3.12 Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: End Users/Desktop Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 License :: Other/Proprietary License Classifier: Operating System :: MacOS
@@ -10,28 +10,27 @@
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
 Multimedia :: Graphics :: Capture :: Screen Capture Classifier: Topic ::
-Utilities Requires-Dist: PySide6-Essentials (==6.4.2) Requires-Dist: jeepney
-(>=0.8.0,<0.9.0) Project-URL: FAQs, https://dynobo.github.io/normcap/#faqs
-Project-URL: Issues, https://github.com/dynobo/normcap/issues Project-URL:
-Repository, https://github.com/dynobo/normcap Description-Content-Type: text/
-markdown  # NormCap **_OCR powered screen-capture tool to capture information
-instead of images. For Linux, macOS and Windows._** [![Build](https://
-img.shields.io/github/actions/workflow/status/dynobo/normcap/
-python.yaml?branch=main)](https://github.com/dynobo/normcap/releases) [!
-[Coverage Status](https://img.shields.io/coverallsCoverage/github/dynobo/
-normcap?label=Test%20coverage&branch=main)](https://coveralls.io/github/dynobo/
-normcap) [![CodeQL](https://img.shields.io/github/actions/workflow/status/
-dynobo/normcap/codeql-analysis.yml?branch=main&label=CodeQL)](https://
-github.com/dynobo/normcap/actions/workflows/codeql-analysis.yml) [![GitHub]
-(https://img.shields.io/github/downloads/dynobo/normcap/
+Utilities Requires-Dist: PySide6-Essentials (==6.4.2) Project-URL: FAQs, https:
+//dynobo.github.io/normcap/#faqs Project-URL: Issues, https://github.com/
+dynobo/normcap/issues Project-URL: Repository, https://github.com/dynobo/
+normcap Description-Content-Type: text/markdown  # NormCap **_OCR powered
+screen-capture tool to capture information instead of images. For Linux, macOS
+and Windows._** [![Build](https://img.shields.io/github/actions/workflow/
+status/dynobo/normcap/python.yaml?branch=main)](https://github.com/dynobo/
+normcap/releases) [![Coverage Status](https://img.shields.io/coverallsCoverage/
+github/dynobo/normcap?label=Test%20coverage&branch=main)](https://coveralls.io/
+github/dynobo/normcap) [![CodeQL](https://img.shields.io/github/actions/
+workflow/status/dynobo/normcap/codeql-analysis.yml?branch=main&label=CodeQL)]
+(https://github.com/dynobo/normcap/actions/workflows/codeql-analysis.yml) [!
+[GitHub](https://img.shields.io/github/downloads/dynobo/normcap/
 total?label=Github%20downloads&color=blue)](https://github.com/dynobo/normcap/
 releases) [![PyPi](https://img.shields.io/pypi/dm/
 normcap?label=PyPi%20downloads&color=blue)](https://pypi.org/project/normcap)
 [![Flathub](https://img.shields.io/flathub/downloads/
 com.github.dynobo.normcap?label=Flathub%20downloads&color=blue)](https://
 flathub.org/apps/details/com.github.dynobo.normcap) [![AUR](https://
 img.shields.io/aur/votes/normcap?label=AUR%20votes&color=blue)](https://
@@ -39,22 +38,22 @@
 (https://github.com/dynobo/normcap) | [Documentation](https://dynobo.github.io/
 normcap/) | [FAQs](https://dynobo.github.io/normcap/#faqs) | [Releases](https:/
 /github.com/dynobo/normcap/releases) | [Changelog](https://github.com/dynobo/
 normcap/blob/main/CHANGELOG) [![Screencast](https://user-
 images.githubusercontent.com/11071876/189767585-8bc45c18-8392-411d-84dc-
 cef1cb5dbc47.gif)](https://raw.githubusercontent.com/dynobo/normcap/main/
 assets/normcap.gif) ## Quickstart Install a prebuilt release: - **Windows**:
-[NormCap-0.4.1-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/
-download/v0.4.1/NormCap-0.4.1-x86_64-Windows.msi) - **Linux**: [NormCap-0.4.1-
-x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.1/
-NormCap-0.4.1-x86_64.AppImage) - **macOS** (x86) Â¹: [NormCap-0.4.1-x86_64-
-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-
-0.4.1-x86_64-macOS.dmg) - **macOS** (M1) Â¹Â·Â²: [NormCap-0.4.1-arm64-
-macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.1/NormCap-
-0.4.1-arm64-macOS.dmg) \ 1: On macOS, allow the unsigned application on first
+[NormCap-0.4.2-x86_64-Windows.msi](https://github.com/dynobo/normcap/releases/
+download/v0.4.2/NormCap-0.4.2-x86_64-Windows.msi) - **Linux**: [NormCap-0.4.2-
+x86_64.AppImage](https://github.com/dynobo/normcap/releases/download/v0.4.2/
+NormCap-0.4.2-x86_64.AppImage) - **macOS** (x86) Â¹: [NormCap-0.4.2-x86_64-
+macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-
+0.4.2-x86_64-macOS.dmg) - **macOS** (M1) Â¹Â·Â²: [NormCap-0.4.2-arm64-
+macOS.dmg](https://github.com/dynobo/normcap/releases/download/v0.4.2/NormCap-
+0.4.2-arm64-macOS.dmg) \ 1: On macOS, allow the unsigned application on first
 start: "System Preferences" â "Security & Privacy" â "General" â "Open
 anyway". You might also need to allow NormCap to take screenshots. [#135]
 (https://github.com/dynobo/normcap/issues/135)
 2: Might be available a bit delayed, as it is currently build manually. (Thx,
 [@Takrin](https://github.com/Takrin)!) Install from repositories: -
 **Windows**: Install from [Microsoft Store](https://apps.microsoft.com/store/
 detail/normcap/XPDLJNB4B6C2ZR). - **Arch / Manjaro**: Install the [`normcap`]
@@ -88,22 +87,21 @@
 Prerequisites for setting up a development environment are: **Python >=3.9**,
 **Poetry>=1.3.2** and **Tesseract** (incl. **language data**). ```sh # Clone
 repository git clone https://github.com/dynobo/normcap.git # Change into
 project directory cd normcap # Create virtual env and install dependencies
 poetry install # Register pre-commit hook poetry run pre-commit install # Run
 NormCap in virtual env poetry run python -m normcap ``` ## Credits This project
 uses the following non-standard libraries: - [pyside6](https://pypi.org/
-project/PySide6/) _- bindings for Qt UI Framework_ - [jeepney](https://
-pypi.org/project/jeepney/) _- DBUS client_ And it depends on external software:
-- [tesseract](https://github.com/tesseract-ocr/tesseract) - _OCR engine_ - [wl-
-clipboard](https://github.com/bugaevc/wl-clipboard) - _Wayland clipboard
-utilities_ Packaging is done with: - [briefcase](https://pypi.org/project/
-briefcase/) _- converting Python projects into_ _standalone apps_ Thanks to the
-maintainers of those nice tools! ## Similar open source tools If NormCap
-doesn't fit your needs, try those alternatives (no particular order): -
+project/PySide6/) _- bindings for Qt UI Framework_ And it depends on external
+software: - [tesseract](https://github.com/tesseract-ocr/tesseract) - _OCR
+engine_ - [wl-clipboard](https://github.com/bugaevc/wl-clipboard) - _Wayland
+clipboard utilities_ Packaging is done with: - [briefcase](https://pypi.org/
+project/briefcase/) _- converting Python projects into_ _standalone apps_
+Thanks to the maintainers of those nice tools! ## Similar open source tools If
+NormCap doesn't fit your needs, try those alternatives (no particular order): -
 [TextSnatcher](https://github.com/RajSolai/TextSnatcher) (Linux) - [GreenShot]
 (https://getgreenshot.org/) (Linux, macOS) - [TextShot](https://github.com/
 ianzhao05/textshot) (Windows) - [gImageReader](https://github.com/manisandro/
 gImageReader) (Linux, Windows) - [Capture2Text](https://sourceforge.net/
 projects/capture2text) (Windows) - [Frog](https://github.com/TenderOwl/Frog)
 (Linux) - [Textinator](https://github.com/RhetTbull/textinator) (macOS) -
 [Text-Grab](https://github.com/TheJoeFin/Text-Grab) (Windows) - [dpScreenOCR]
```

