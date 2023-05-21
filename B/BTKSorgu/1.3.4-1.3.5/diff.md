# Comparing `tmp/BTKSorgu-1.3.4.tar.gz` & `tmp/BTKSorgu-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.3.4.tar", last modified: Sun May 21 00:29:59 2023, max compression
+gzip compressed data, was "BTKSorgu-1.3.5.tar", last modified: Sun May 21 00:52:22 2023, max compression
```

## Comparing `BTKSorgu-1.3.4.tar` & `BTKSorgu-1.3.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.993704 BTKSorgu-1.3.4/BTKSorgu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/BTKSorgu/Assets/
--rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/BTKSorgu/Assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/BTKSorgu/GUI/
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/BTKSorgu/GUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/BTKSorgu/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/BTKSorgu/Libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/BTKSorgu/konsol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-21 00:29:58.000000 BTKSorgu-1.3.4/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-21 00:29:58.000000 BTKSorgu-1.3.4/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:29:58.000000 BTKSorgu-1.3.4/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-21 00:29:58.000000 BTKSorgu-1.3.4/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-21 00:29:58.000000 BTKSorgu-1.3.4/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 00:29:58.000000 BTKSorgu-1.3.4/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:52:22.865393 BTKSorgu-1.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:52:22.857392 BTKSorgu-1.3.5/BTKSorgu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:52:22.861392 BTKSorgu-1.3.5/BTKSorgu/Assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-21 00:51:53.000000 BTKSorgu-1.3.5/BTKSorgu/Assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:52:22.861392 BTKSorgu-1.3.5/BTKSorgu/GUI/
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-21 00:51:53.000000 BTKSorgu-1.3.5/BTKSorgu/GUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:52:22.861392 BTKSorgu-1.3.5/BTKSorgu/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-21 00:51:53.000000 BTKSorgu-1.3.5/BTKSorgu/Libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-21 00:51:53.000000 BTKSorgu-1.3.5/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-21 00:51:53.000000 BTKSorgu-1.3.5/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-21 00:51:53.000000 BTKSorgu-1.3.5/BTKSorgu/konsol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:52:22.861392 BTKSorgu-1.3.5/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-21 00:52:22.000000 BTKSorgu-1.3.5/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-21 00:52:22.000000 BTKSorgu-1.3.5/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:52:22.000000 BTKSorgu-1.3.5/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-21 00:52:22.000000 BTKSorgu-1.3.5/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-21 00:52:22.000000 BTKSorgu-1.3.5/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 00:52:22.000000 BTKSorgu-1.3.5/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 00:51:53.000000 BTKSorgu-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-21 00:51:53.000000 BTKSorgu-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-21 00:52:22.865393 BTKSorgu-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-05-21 00:51:53.000000 BTKSorgu-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:52:22.861392 BTKSorgu-1.3.5/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-21 00:51:53.000000 BTKSorgu-1.3.5/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-21 00:51:53.000000 BTKSorgu-1.3.5/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-21 00:51:53.000000 BTKSorgu-1.3.5/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:52:22.865393 BTKSorgu-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-21 00:51:53.000000 BTKSorgu-1.3.5/setup.py
```

### Comparing `BTKSorgu-1.3.4/BTKSorgu/Assets/logo.png` & `BTKSorgu-1.3.5/BTKSorgu/Assets/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.3.4/BTKSorgu/GUI/__init__.py` & `BTKSorgu-1.3.5/BTKSorgu/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.3.4/BTKSorgu/__init__.py` & `BTKSorgu-1.3.5/BTKSorgu/__init__.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.3.4/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.3.5/BTKSorgu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.3.4
+Version: 1.3.5
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/BTKSorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.3.4 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.3.5 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.3.4/LICENSE` & `BTKSorgu-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.3.4/PKG-INFO` & `BTKSorgu-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.3.4
+Version: 1.3.5
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/BTKSorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.3.4 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.3.5 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.3.4/README.md` & `BTKSorgu-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.3.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.3.5/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 0% similar despite different names*

#### Comparing `BTKSorgu-1.3.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.3.5/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -28,15 +28,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.3.4" date="2023-5-21">
+    <release version="1.3.5" date="2023-5-21">
       <description>
         <p>Çeşitli hatalar giderildi..</p>
         <p>Bkz.:</p>
         <ul>
           <li>Github CI/CD</li>
           <li>Tkinter CTRL+A</li>
           <li>tesseract Hata Çıktısı</li>
```

### Comparing `BTKSorgu-1.3.4/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.3.5/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.3.4/setup.py` & `BTKSorgu-1.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.3.4",
+    version      = "1.3.5",
     url          = "https://github.com/keyiflerolsun/BTKSorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -25,15 +25,14 @@
     packages         = ["BTKSorgu"],
     python_requires  = ">=3.10",
     install_requires = [
         "setuptools",
         "wheel",
         "install_freedesktop",
         "rich",
-        "Pygments",
         "requests",
         "parsel",
         "cssselect",
         "regex",
         "Pillow",
         "pytesseract",
         "sv_ttk"
```

