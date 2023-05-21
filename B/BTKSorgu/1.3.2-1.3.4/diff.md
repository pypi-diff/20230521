# Comparing `tmp/BTKSorgu-1.3.2.tar.gz` & `tmp/BTKSorgu-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.3.2.tar", last modified: Sat May 20 23:45:00 2023, max compression
+gzip compressed data, was "BTKSorgu-1.3.4.tar", last modified: Sun May 21 00:29:59 2023, max compression
```

## Comparing `BTKSorgu-1.3.2.tar` & `BTKSorgu-1.3.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:45:00.790547 BTKSorgu-1.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:45:00.786547 BTKSorgu-1.3.2/BTKSorgu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:45:00.790547 BTKSorgu-1.3.2/BTKSorgu/GUI/
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-20 23:44:25.000000 BTKSorgu-1.3.2/BTKSorgu/GUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:45:00.790547 BTKSorgu-1.3.2/BTKSorgu/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-20 23:44:25.000000 BTKSorgu-1.3.2/BTKSorgu/Libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-20 23:44:25.000000 BTKSorgu-1.3.2/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-20 23:44:25.000000 BTKSorgu-1.3.2/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-20 23:44:25.000000 BTKSorgu-1.3.2/BTKSorgu/konsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-20 23:44:25.000000 BTKSorgu-1.3.2/BTKSorgu/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:45:00.790547 BTKSorgu-1.3.2/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-20 23:45:00.000000 BTKSorgu-1.3.2/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-20 23:45:00.000000 BTKSorgu-1.3.2/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 23:45:00.000000 BTKSorgu-1.3.2/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 23:45:00.000000 BTKSorgu-1.3.2/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 23:45:00.000000 BTKSorgu-1.3.2/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 23:45:00.000000 BTKSorgu-1.3.2/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 23:44:25.000000 BTKSorgu-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 23:44:25.000000 BTKSorgu-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-20 23:45:00.790547 BTKSorgu-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-05-20 23:44:25.000000 BTKSorgu-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:45:00.790547 BTKSorgu-1.3.2/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-20 23:44:25.000000 BTKSorgu-1.3.2/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-20 23:44:25.000000 BTKSorgu-1.3.2/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-20 23:44:25.000000 BTKSorgu-1.3.2/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 23:45:00.790547 BTKSorgu-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-20 23:44:25.000000 BTKSorgu-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.993704 BTKSorgu-1.3.4/BTKSorgu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/BTKSorgu/Assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/BTKSorgu/Assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/BTKSorgu/GUI/
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/BTKSorgu/GUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/BTKSorgu/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/BTKSorgu/Libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/BTKSorgu/konsol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-21 00:29:58.000000 BTKSorgu-1.3.4/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-21 00:29:58.000000 BTKSorgu-1.3.4/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:29:58.000000 BTKSorgu-1.3.4/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-21 00:29:58.000000 BTKSorgu-1.3.4/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-21 00:29:58.000000 BTKSorgu-1.3.4/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 00:29:58.000000 BTKSorgu-1.3.4/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:29:58.997704 BTKSorgu-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-21 00:29:29.000000 BTKSorgu-1.3.4/setup.py
```

### Comparing `BTKSorgu-1.3.2/BTKSorgu/GUI/__init__.py` & `BTKSorgu-1.3.4/BTKSorgu/GUI/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class KekikGUI(tk.Tk):
     def __init__(self):
         super().__init__()
         set_theme("dark")
         self.title("BTK Sorgu")
 
-        logo_b64 = encodebytes(open(file=dosya_ver("logo.png", ust_dizin=2), mode="rb").read())
+        logo_b64 = encodebytes(open(file=dosya_ver("Assets/logo.png", ust_dizin=2), mode="rb").read())
         favicon  = tk.PhotoImage(data=logo_b64)
         self.iconphoto(False, favicon)
 
         self.p_genislik  = max(self.winfo_width(), 400)
         self.p_yukseklik = max(self.winfo_height(), 250)
         self.minsize(width=self.p_genislik, height=self.p_yukseklik)
```

### Comparing `BTKSorgu-1.3.2/BTKSorgu/__init__.py` & `BTKSorgu-1.3.4/BTKSorgu/__init__.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.3.2/BTKSorgu/logo.png` & `BTKSorgu-1.3.4/BTKSorgu/Assets/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.3.2/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.3.4/BTKSorgu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.3.2
+Version: 1.3.4
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
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.3.2 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.3.4 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.3.2/LICENSE` & `BTKSorgu-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.3.2/PKG-INFO` & `BTKSorgu-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.3.2
+Version: 1.3.4
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
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.3.2 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.3.4 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `BTKSorgu-1.3.2/README.md` & `BTKSorgu-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.3.2/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.3.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 8% similar despite different names*

#### Comparing `BTKSorgu-1.3.2/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.3.4/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -28,23 +28,23 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.3.2" date="2023-5-21">
+    <release version="1.3.4" date="2023-5-21">
       <description>
         <p>Çeşitli hatalar giderildi..</p>
         <p>Bkz.:</p>
         <ul>
           <li>Github CI/CD</li>
           <li>Tkinter CTRL+A</li>
           <li>tesseract Hata Çıktısı</li>
         </ul>
       </description>
     </release>
     <release version="1.1.4" date="2023-5-18"/>
-    <release version="1.0.5" date="2023-5-17"/>
+    <release version="0.0.1" date="2021-3-13"/>
   </releases>
   <content_rating type="oars-1.1"/>
 </component>
```

### Comparing `BTKSorgu-1.3.2/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.3.4/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.3.2/setup.py` & `BTKSorgu-1.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.3.2",
+    version      = "1.3.4",
     url          = "https://github.com/keyiflerolsun/BTKSorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -25,14 +25,15 @@
     packages         = ["BTKSorgu"],
     python_requires  = ">=3.10",
     install_requires = [
         "setuptools",
         "wheel",
         "install_freedesktop",
         "rich",
+        "Pygments",
         "requests",
         "parsel",
         "cssselect",
         "regex",
         "Pillow",
         "pytesseract",
         "sv_ttk"
```

