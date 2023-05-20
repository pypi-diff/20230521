# Comparing `tmp/BTKSorgu-1.2.9.tar.gz` & `tmp/BTKSorgu-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.2.9.tar", last modified: Sat May 20 21:15:05 2023, max compression
+gzip compressed data, was "BTKSorgu-1.3.1.tar", last modified: Sat May 20 23:04:53 2023, max compression
```

## Comparing `BTKSorgu-1.2.9.tar` & `BTKSorgu-1.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/BTKSorgu/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/ekstra.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/konsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/BTKSorgu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:04:53.899836 BTKSorgu-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:04:53.895836 BTKSorgu-1.3.1/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/BTKSorgu/ekstra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:04:53.899836 BTKSorgu-1.3.1/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-20 23:04:53.000000 BTKSorgu-1.3.1/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-20 23:04:53.000000 BTKSorgu-1.3.1/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 23:04:53.000000 BTKSorgu-1.3.1/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 23:04:53.000000 BTKSorgu-1.3.1/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 23:04:53.000000 BTKSorgu-1.3.1/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 23:04:53.000000 BTKSorgu-1.3.1/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-05-20 23:04:53.899836 BTKSorgu-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:04:53.899836 BTKSorgu-1.3.1/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 23:04:53.899836 BTKSorgu-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-20 23:04:27.000000 BTKSorgu-1.3.1/setup.py
```

### Comparing `BTKSorgu-1.2.9/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.3.1/BTKSorgu/Erisim_Engeli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
+from rich         import pretty, traceback
+from rich.console import Console
+pretty.install()
+traceback.install(show_locals=False)
+konsol = Console(log_path=False)
+
 from requests import Session
 from parsel   import Selector
 
 from shutil      import copyfileobj
 from pytesseract import image_to_string 
 from PIL         import Image
 from re          import search
@@ -15,40 +21,45 @@
     BTKSorgu : Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 
     Dönüş
     ----------
         (str):
             {domain}, {karar} Karar Bulunamadı.
     """
-    def __init__(self, sorgu_url:str, arka_plan:bool=False):
+    def __init__(self, sorgu_url:str):
         """Karar Döndürür"""
-        self.arka_plan      = arka_plan
         self.ana_sayfa      = "https://internet2.btk.gov.tr"
         self.sorgu_sayfasi  = "https://internet2.btk.gov.tr/sitesorgu/"
         self.sorgu_url      = search(r"(?:https?://)?(?:www\.)?([^/]+)", sorgu_url).group(1)
         self._gecici_gorsel = "captcha.png"
 
         self.oturum = Session()
 
-    @property
-    def captcha_ver(self):
+    def __captcha_ver(self):
         """Captcha görselini indirip OCR ile okur"""
         ilk_bakis    = self.oturum.get(self.sorgu_sayfasi, allow_redirects=True)
         captcha_yolu = Selector(ilk_bakis.text).xpath("//div[@class='arama_captcha']/img/@src").get()
 
         captcha_data = self.oturum.get(f"{self.ana_sayfa}{captcha_yolu}", stream=True)
         with open(self._gecici_gorsel, "wb") as captcha_gorsel:
             copyfileobj(captcha_data.raw, captcha_gorsel)
 
-        return image_to_string(Image.open(self._gecici_gorsel)).strip().replace(" ", "")
+        try:
+            captcha_harfleri = image_to_string(Image.open(self._gecici_gorsel)).strip().replace(" ", "")
+        except Exception as hata:
+            konsol.print(f"[bold red]Hata: {hata}\n\n")
+            return None
+
+        return captcha_harfleri
 
-    @property
-    def karar(self):
+    def karar_ver(self):
         """Captcha ile birlikte sorgu sitesini POST eder"""
-        captcha = self.captcha_ver
+        captcha = self.__captcha_ver()
+        if not captcha:
+            return "Muhtemelen Sisteminizde 'tesseract-ocr' Yüklü Değil!"
 
         karar_sayfasi = self.oturum.post(
             url     = self.sorgu_sayfasi,
             headers = {
                 "Content-Type" : "application/x-www-form-urlencoded",
                 "Host"         : "internet2.btk.gov.tr",
                 "Origin"       : self.ana_sayfa,
@@ -67,27 +78,18 @@
         )
 
         # print(karar_sayfasi.text)
         secici     = Selector(karar_sayfasi.text)
         hatali_kod = secici.xpath("//div[@class='icerik']/ul/li/text()").get()
         erisim_var = secici.xpath("//div[@class='yazi2']/text()").get()
         erisim_yok = secici.xpath("//span[@class='yazi2_2']/text()").get()
-        karar      = hatali_kod or erisim_var or erisim_yok or ""
-
-        if self.arka_plan:
-            print(f"""
-
-            # Sorgu   : {self.sorgu_url}
-            # Captcha : {captcha}
-            # Karar   : {karar}
 
-""")
-        return karar
+        return hatali_kod or erisim_var or erisim_yok or ""
 
     def __repr__(self) -> str:
         """Kararı Döndürür"""
         hatalar = ["Lütfen güvenlik kodunu giriniz.", "Güvenlik kodunu yanlış girdiniz. Lütfen Güvenlik Kodunu resimde gördüğünüz şekilde giriniz."]
         while True:
-            karar = self.karar
+            karar = self.karar_ver()
             if karar not in hatalar:
                 remove(self._gecici_gorsel)
                 return karar
```

### Comparing `BTKSorgu-1.2.9/BTKSorgu/KekikGUI.py` & `BTKSorgu-1.3.1/BTKSorgu/KekikGUI.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.9/BTKSorgu/konsol.py` & `BTKSorgu-1.3.1/BTKSorgu/konsol.py`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.9/BTKSorgu/logo.png` & `BTKSorgu-1.3.1/BTKSorgu/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.9/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.3.1/BTKSorgu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.2.9
+Version: 1.3.1
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/BTKSorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,38 +17,38 @@
 # <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/org.KekikAkademi.BTKSorgu.svg"></a> BTKSorgu
 
 [![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)](#)
 [![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
 [![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/releases)
-[![PyPi Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
+[![PyPI Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
 [![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
 
 [![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 [![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 
-[![PyPi](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://pypi.org/project/BTKSorgu)
-[![PyPi - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
-[![PyPi - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
+[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/BTKSorgu)
+[![PyPI - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
 
 [![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white&label=Python)](#)
 [![Lisans](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
 [![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPi (Lib - CLI - UI)
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPI (Lib - CLI - UI)
 
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
@@ -116,15 +116,15 @@
 
 ```bash
 # Depoyu Çek
 https://github.com/keyiflerolsun/BTKSorgu.git
 cd BTKSorgu
 
 # Gerekli Ortamları Kur
-pip install -U pip setuptools wheel twine
+pip install -U pip setuptools wheel
 
 # Paketi Yükle
 pip install .
 
 # Artıkları Temizle
 rm -rf build *.egg-info
 
@@ -184,16 +184,17 @@
 
 > Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
 
 ## 📝 Proje İlerlemesi
 
 - ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
 - ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
-- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
+- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **PyPI** *depolarına yüklenmiştir..*
 - ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
+- ✅ *İlham yaratması için* **FlatHub** *depolarına yüklenmiştir..*
 
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.9 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.3.1 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -10,45 +10,45 @@
 Shared/org.KekikAkademi.BTKSorgu.svg] BTKSorgu [![Boyut](https://
 img.shields.io/github/repo-size/keyiflerolsun/
 BTKSorgu?logo=git&logoColor=white&label=Boyut)](#) [![GÃ¶rÃ¼ntÃ¼lenme](https://
 hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
 keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/
 badge/âï¸-Kahve_Ismarla-ffdd00] [![GitHub](https://img.shields.io/github/v/
 release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/
-keyiflerolsun/BTKSorgu/releases) [![PyPi YÃ¼kleyici](https://img.shields.io/
+keyiflerolsun/BTKSorgu/releases) [![PyPI YÃ¼kleyici](https://img.shields.io/
 github/actions/workflow/status/keyiflerolsun/BTKSorgu/
-pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/
+pypiYukle.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/
 keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml) [![Flatpak YÃ¼kleyici]
 (https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/
 flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://
 github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml) [!
 [FlatHub](https://img.shields.io/flathub/v/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://
 flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - YÃ¼klenme](https://
 img.shields.io/flathub/downloads/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=YÃ¼klenme)](https:
-//flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![PyPi](https://
-img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://
-pypi.org/project/BTKSorgu) [![PyPi - YÃ¼klenme](https://img.shields.io/pypi/dm/
+//flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![PyPI](https://
+img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPI)](https://
+pypi.org/project/BTKSorgu) [![PyPI - YÃ¼klenme](https://img.shields.io/pypi/dm/
 BTKSorgu?logo=pypi&logoColor=white&label=YÃ¼klenme)](https://pypi.org/project/
-BTKSorgu) [![PyPi - Wheel](https://img.shields.io/pypi/wheel/
+BTKSorgu) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/
 BTKSorgu) [![Python Version](https://img.shields.io/pypi/pyversions/
 BTKSorgu?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
 img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#) [!
 [Durum](https://img.shields.io/pypi/status/
 BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#) *Hedef
 websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* [![BTKSorgu](https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-
 with-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love]
 (https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
 GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
-PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
+PyPI (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
 pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
 YÃ¼klemek flatpak install flathub org.KekikAkademi.BTKSorgu # ÃalÄ±ÅtÄ±rmak
 flatpak run org.KekikAkademi.BTKSorgu ``` ## ð KullanÄ±m ### [https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg]
 Lib ```python from BTKSorgu import BTKSorgu from time import time basla = time
 () print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve
@@ -65,51 +65,51 @@
 main/.github/icons/freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
 org.KekikAkademi.BTKSorgu ``` ---   [https://raw.githubusercontent.com/
 keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg] Kendiniz Paketlemek
 Ä°sterseniz (geniÅletmek iÃ§in tÄ±klayÄ±n!)
 ### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/
 icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
 keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli OrtamlarÄ± Kur pip install -
-U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
-Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI
-# Paketi KaldÄ±r pip uninstall BTKSorgu ``` ### [https://
-raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/
-flatpak.svg] FlatPak ```bash # Depoyu Ãek git clone https://github.com/
-keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli DosyalarÄ± Al mv Shared/*.yml
-. && mv Shared/SRC . # Gerekli OrtamlarÄ± Kur flatpak remote-add --if-not-
-exists flathub https://flathub.org/repo/flathub.flatpakrepo flatpak remote-add
---if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-
-beta.flatpakrepo flatpak update && flatpak upgrade flatpak install flathub
-org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --
-install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ±
-Temizle rm -rf .flatpak* .vscode build-dir && find . | grep -E "
-(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf # ÃalÄ±ÅtÄ±r flatpak run
-org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r flatpak uninstall
-org.KekikAkademi.BTKSorgu ```  --- ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
-BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
-) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
-kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
-harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
-doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
-geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
-paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu **gereksiz
-kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
+U pip setuptools wheel # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ± Temizle rm -
+rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI # Paketi
+KaldÄ±r pip uninstall BTKSorgu ``` ### [https://raw.githubusercontent.com/
+keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg] FlatPak ```bash # Depoyu
+Ãek git clone https://github.com/keyiflerolsun/BTKSorgu.git cd BTKSorgu #
+Gerekli DosyalarÄ± Al mv Shared/*.yml . && mv Shared/SRC . # Gerekli OrtamlarÄ±
+Kur flatpak remote-add --if-not-exists flathub https://flathub.org/repo/
+flathub.flatpakrepo flatpak remote-add --if-not-exists flathub-beta https://
+flathub.org/beta-repo/flathub-beta.flatpakrepo flatpak update && flatpak
+upgrade flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08 # Paketle
+flatpak-builder --user --install --force-clean build-dir
+org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ± Temizle rm -rf .flatpak* .vscode
+build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf #
+ÃalÄ±ÅtÄ±r flatpak run org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r flatpak
+uninstall org.KekikAkademi.BTKSorgu ```  --- ## ð Program AkÄ±Å ÅemasÄ± 1.
+*Oturum BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://
+internet2.btk.gov.tr/) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri
+ye,* 3. *DÃ¶nen kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama
+resmini OCR ile harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini
+okuduÄun doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ±
+ayrÄ±ÅtÄ±rÄ±p edip geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak
+kodlu olarak paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu
+**gereksiz kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
 etmektirâ¦* > TarayÄ±cÄ± Otomasyonu : *[Selenium IDE](https://
 www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://
 www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *
 [BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 > KarÅÄ±laÅtÄ±rmasÄ± : **[Selenium VS Requests](https://www.r10.net/off-
 topic/2751612-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
 [@raifpy](https://github.com/raifpy)** *tarafÄ±ndan kodlanmÄ±Å projenin hantal
 bir bileÅeni itinayla `dÄ±zz ð`'lanmÄ±ÅtÄ±r..* - â **Selenium**
 *baÄÄ±mlÄ±lÄ±ÄÄ±ndan dolayÄ± hantal Ã§alÄ±Åan kod yapÄ±sÄ± tamamen
 ayÄ±klanÄ±p bÃ¼tÃ¼n iÅ* `requests`*'e yaptÄ±rÄ±lÄ±p ciddi miktarda kaynak ve
 zaman tasarrufu ettirilmiÅtir..* - â *Kolay eriÅilebilir olmasÄ± ve ilham
-yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
+yaratmasÄ± iÃ§in* **PyPI** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
 *ile basit bir arayÃ¼z tasarlanmÄ±ÅtÄ±r ve eÄitim amacÄ±yla Depolara
+yÃ¼klenmiÅtir..* - â *Ä°lham yaratmasÄ± iÃ§in* **FlatHub** *depolarÄ±na
 yÃ¼klenmiÅtir..* ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
 [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
 PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
 BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
 â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
 mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
 ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
```

### Comparing `BTKSorgu-1.2.9/LICENSE` & `BTKSorgu-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.9/PKG-INFO` & `BTKSorgu-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BTKSorgu
-Version: 1.2.9
+Version: 1.3.1
 Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 Home-page: https://github.com/keyiflerolsun/BTKSorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,38 +17,38 @@
 # <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/org.KekikAkademi.BTKSorgu.svg"></a> BTKSorgu
 
 [![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)](#)
 [![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
 [![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/releases)
-[![PyPi Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
+[![PyPI Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
 [![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
 
 [![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 [![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 
-[![PyPi](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://pypi.org/project/BTKSorgu)
-[![PyPi - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
-[![PyPi - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
+[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/BTKSorgu)
+[![PyPI - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
 
 [![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white&label=Python)](#)
 [![Lisans](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
 [![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPi (Lib - CLI - UI)
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPI (Lib - CLI - UI)
 
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
@@ -116,15 +116,15 @@
 
 ```bash
 # Depoyu Çek
 https://github.com/keyiflerolsun/BTKSorgu.git
 cd BTKSorgu
 
 # Gerekli Ortamları Kur
-pip install -U pip setuptools wheel twine
+pip install -U pip setuptools wheel
 
 # Paketi Yükle
 pip install .
 
 # Artıkları Temizle
 rm -rf build *.egg-info
 
@@ -184,16 +184,17 @@
 
 > Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
 
 ## 📝 Proje İlerlemesi
 
 - ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
 - ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
-- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
+- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **PyPI** *depolarına yüklenmiştir..*
 - ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
+- ✅ *İlham yaratması için* **FlatHub** *depolarına yüklenmiştir..*
 
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.9 Summary: Hedef websitesinin
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.3.1 Summary: Hedef websitesinin
 BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
 keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -10,45 +10,45 @@
 Shared/org.KekikAkademi.BTKSorgu.svg] BTKSorgu [![Boyut](https://
 img.shields.io/github/repo-size/keyiflerolsun/
 BTKSorgu?logo=git&logoColor=white&label=Boyut)](#) [![GÃ¶rÃ¼ntÃ¼lenme](https://
 hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
 keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/
 badge/âï¸-Kahve_Ismarla-ffdd00] [![GitHub](https://img.shields.io/github/v/
 release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/
-keyiflerolsun/BTKSorgu/releases) [![PyPi YÃ¼kleyici](https://img.shields.io/
+keyiflerolsun/BTKSorgu/releases) [![PyPI YÃ¼kleyici](https://img.shields.io/
 github/actions/workflow/status/keyiflerolsun/BTKSorgu/
-pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/
+pypiYukle.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/
 keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml) [![Flatpak YÃ¼kleyici]
 (https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/
 flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://
 github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml) [!
 [FlatHub](https://img.shields.io/flathub/v/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://
 flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - YÃ¼klenme](https://
 img.shields.io/flathub/downloads/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=YÃ¼klenme)](https:
-//flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![PyPi](https://
-img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://
-pypi.org/project/BTKSorgu) [![PyPi - YÃ¼klenme](https://img.shields.io/pypi/dm/
+//flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![PyPI](https://
+img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPI)](https://
+pypi.org/project/BTKSorgu) [![PyPI - YÃ¼klenme](https://img.shields.io/pypi/dm/
 BTKSorgu?logo=pypi&logoColor=white&label=YÃ¼klenme)](https://pypi.org/project/
-BTKSorgu) [![PyPi - Wheel](https://img.shields.io/pypi/wheel/
+BTKSorgu) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/
 BTKSorgu) [![Python Version](https://img.shields.io/pypi/pyversions/
 BTKSorgu?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
 img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#) [!
 [Durum](https://img.shields.io/pypi/status/
 BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#) *Hedef
 websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* [![BTKSorgu](https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-
 with-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love]
 (https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
 GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
-PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
+PyPI (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
 pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
 YÃ¼klemek flatpak install flathub org.KekikAkademi.BTKSorgu # ÃalÄ±ÅtÄ±rmak
 flatpak run org.KekikAkademi.BTKSorgu ``` ## ð KullanÄ±m ### [https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg]
 Lib ```python from BTKSorgu import BTKSorgu from time import time basla = time
 () print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve
@@ -65,51 +65,51 @@
 main/.github/icons/freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
 org.KekikAkademi.BTKSorgu ``` ---   [https://raw.githubusercontent.com/
 keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg] Kendiniz Paketlemek
 Ä°sterseniz (geniÅletmek iÃ§in tÄ±klayÄ±n!)
 ### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/
 icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
 keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli OrtamlarÄ± Kur pip install -
-U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
-Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI
-# Paketi KaldÄ±r pip uninstall BTKSorgu ``` ### [https://
-raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/
-flatpak.svg] FlatPak ```bash # Depoyu Ãek git clone https://github.com/
-keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli DosyalarÄ± Al mv Shared/*.yml
-. && mv Shared/SRC . # Gerekli OrtamlarÄ± Kur flatpak remote-add --if-not-
-exists flathub https://flathub.org/repo/flathub.flatpakrepo flatpak remote-add
---if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-
-beta.flatpakrepo flatpak update && flatpak upgrade flatpak install flathub
-org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --
-install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ±
-Temizle rm -rf .flatpak* .vscode build-dir && find . | grep -E "
-(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf # ÃalÄ±ÅtÄ±r flatpak run
-org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r flatpak uninstall
-org.KekikAkademi.BTKSorgu ```  --- ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
-BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
-) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
-kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
-harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
-doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
-geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
-paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu **gereksiz
-kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
+U pip setuptools wheel # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ± Temizle rm -
+rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI # Paketi
+KaldÄ±r pip uninstall BTKSorgu ``` ### [https://raw.githubusercontent.com/
+keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg] FlatPak ```bash # Depoyu
+Ãek git clone https://github.com/keyiflerolsun/BTKSorgu.git cd BTKSorgu #
+Gerekli DosyalarÄ± Al mv Shared/*.yml . && mv Shared/SRC . # Gerekli OrtamlarÄ±
+Kur flatpak remote-add --if-not-exists flathub https://flathub.org/repo/
+flathub.flatpakrepo flatpak remote-add --if-not-exists flathub-beta https://
+flathub.org/beta-repo/flathub-beta.flatpakrepo flatpak update && flatpak
+upgrade flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08 # Paketle
+flatpak-builder --user --install --force-clean build-dir
+org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ± Temizle rm -rf .flatpak* .vscode
+build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf #
+ÃalÄ±ÅtÄ±r flatpak run org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r flatpak
+uninstall org.KekikAkademi.BTKSorgu ```  --- ## ð Program AkÄ±Å ÅemasÄ± 1.
+*Oturum BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://
+internet2.btk.gov.tr/) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri
+ye,* 3. *DÃ¶nen kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama
+resmini OCR ile harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini
+okuduÄun doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ±
+ayrÄ±ÅtÄ±rÄ±p edip geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak
+kodlu olarak paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu
+**gereksiz kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
 etmektirâ¦* > TarayÄ±cÄ± Otomasyonu : *[Selenium IDE](https://
 www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://
 www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *
 [BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 > KarÅÄ±laÅtÄ±rmasÄ± : **[Selenium VS Requests](https://www.r10.net/off-
 topic/2751612-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
 [@raifpy](https://github.com/raifpy)** *tarafÄ±ndan kodlanmÄ±Å projenin hantal
 bir bileÅeni itinayla `dÄ±zz ð`'lanmÄ±ÅtÄ±r..* - â **Selenium**
 *baÄÄ±mlÄ±lÄ±ÄÄ±ndan dolayÄ± hantal Ã§alÄ±Åan kod yapÄ±sÄ± tamamen
 ayÄ±klanÄ±p bÃ¼tÃ¼n iÅ* `requests`*'e yaptÄ±rÄ±lÄ±p ciddi miktarda kaynak ve
 zaman tasarrufu ettirilmiÅtir..* - â *Kolay eriÅilebilir olmasÄ± ve ilham
-yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
+yaratmasÄ± iÃ§in* **PyPI** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
 *ile basit bir arayÃ¼z tasarlanmÄ±ÅtÄ±r ve eÄitim amacÄ±yla Depolara
+yÃ¼klenmiÅtir..* - â *Ä°lham yaratmasÄ± iÃ§in* **FlatHub** *depolarÄ±na
 yÃ¼klenmiÅtir..* ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
 [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
 PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
 BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
 â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
 mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
 ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
```

### Comparing `BTKSorgu-1.2.9/README.md` & `BTKSorgu-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/org.KekikAkademi.BTKSorgu.svg"></a> BTKSorgu
 
 [![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)](#)
 [![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
 [![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/releases)
-[![PyPi Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
+[![PyPI Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
 [![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
 
 [![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 [![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
 
-[![PyPi](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://pypi.org/project/BTKSorgu)
-[![PyPi - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
-[![PyPi - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
+[![PyPI](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/BTKSorgu)
+[![PyPI - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
 
 [![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white&label=Python)](#)
 [![Lisans](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#)
 
 *Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
 
 [![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPi (Lib - CLI - UI)
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPI (Lib - CLI - UI)
 
 ```bash
 # Yüklemek
 pip install BTKSorgu
 
 # Güncellemek
 pip install -U BTKSorgu
@@ -100,15 +100,15 @@
 
 ```bash
 # Depoyu Çek
 https://github.com/keyiflerolsun/BTKSorgu.git
 cd BTKSorgu
 
 # Gerekli Ortamları Kur
-pip install -U pip setuptools wheel twine
+pip install -U pip setuptools wheel
 
 # Paketi Yükle
 pip install .
 
 # Artıkları Temizle
 rm -rf build *.egg-info
 
@@ -168,16 +168,17 @@
 
 > Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
 
 ## 📝 Proje İlerlemesi
 
 - ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
 - ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
-- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
+- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **PyPI** *depolarına yüklenmiştir..*
 - ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
+- ✅ *İlham yaratması için* **FlatHub** *depolarına yüklenmiştir..*
 
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
@@ -186,8 +187,8 @@
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ***
 
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -2,45 +2,45 @@
 org.KekikAkademi.BTKSorgu.svg] BTKSorgu [![Boyut](https://img.shields.io/
 github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)]
 (#) [![GÃ¶rÃ¼ntÃ¼lenme](https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=GÃ¶rÃ¼ntÃ¼lenme)]
 (#) [https://img.shields.io/badge/âï¸-Kahve_Ismarla-ffdd00] [![GitHub]
 (https://img.shields.io/github/v/release/keyiflerolsun/
 BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/
-releases) [![PyPi YÃ¼kleyici](https://img.shields.io/github/actions/workflow/
+releases) [![PyPI YÃ¼kleyici](https://img.shields.io/github/actions/workflow/
 status/keyiflerolsun/BTKSorgu/
-pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/
+pypiYukle.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/
 keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml) [![Flatpak YÃ¼kleyici]
 (https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/
 flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://
 github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml) [!
 [FlatHub](https://img.shields.io/flathub/v/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://
 flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![FlatHub - YÃ¼klenme](https://
 img.shields.io/flathub/downloads/
 org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=YÃ¼klenme)](https:
-//flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![PyPi](https://
-img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://
-pypi.org/project/BTKSorgu) [![PyPi - YÃ¼klenme](https://img.shields.io/pypi/dm/
+//flathub.org/tr/apps/org.KekikAkademi.BTKSorgu) [![PyPI](https://
+img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPI)](https://
+pypi.org/project/BTKSorgu) [![PyPI - YÃ¼klenme](https://img.shields.io/pypi/dm/
 BTKSorgu?logo=pypi&logoColor=white&label=YÃ¼klenme)](https://pypi.org/project/
-BTKSorgu) [![PyPi - Wheel](https://img.shields.io/pypi/wheel/
+BTKSorgu) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
 BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/
 BTKSorgu) [![Python Version](https://img.shields.io/pypi/pyversions/
 BTKSorgu?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
 img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#) [!
 [Durum](https://img.shields.io/pypi/status/
 BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#) *Hedef
 websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu..* [![BTKSorgu](https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-
 with-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love]
 (https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
 GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg]
-PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
+PyPI (Lib - CLI - UI) ```bash # YÃ¼klemek pip install BTKSorgu # GÃ¼ncellemek
 pip install -U BTKSorgu ``` ### [https://raw.githubusercontent.com/
 keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg] FlatHub (UI) ```bash #
 YÃ¼klemek flatpak install flathub org.KekikAkademi.BTKSorgu # ÃalÄ±ÅtÄ±rmak
 flatpak run org.KekikAkademi.BTKSorgu ``` ## ð KullanÄ±m ### [https://
 raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg]
 Lib ```python from BTKSorgu import BTKSorgu from time import time basla = time
 () print(BTKSorgu("redtube.com")) # Â» redtube.com, 30/01/2008 tarihli ve
@@ -57,51 +57,51 @@
 main/.github/icons/freedesktop.svg] UI ```bash BTKSorguGUI # veya flatpak run
 org.KekikAkademi.BTKSorgu ``` ---   [https://raw.githubusercontent.com/
 keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg] Kendiniz Paketlemek
 Ä°sterseniz (geniÅletmek iÃ§in tÄ±klayÄ±n!)
 ### [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/
 icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
 keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli OrtamlarÄ± Kur pip install -
-U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
-Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI
-# Paketi KaldÄ±r pip uninstall BTKSorgu ``` ### [https://
-raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/
-flatpak.svg] FlatPak ```bash # Depoyu Ãek git clone https://github.com/
-keyiflerolsun/BTKSorgu.git cd BTKSorgu # Gerekli DosyalarÄ± Al mv Shared/*.yml
-. && mv Shared/SRC . # Gerekli OrtamlarÄ± Kur flatpak remote-add --if-not-
-exists flathub https://flathub.org/repo/flathub.flatpakrepo flatpak remote-add
---if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-
-beta.flatpakrepo flatpak update && flatpak upgrade flatpak install flathub
-org.freedesktop.{Platform,Sdk}//22.08 # Paketle flatpak-builder --user --
-install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ±
-Temizle rm -rf .flatpak* .vscode build-dir && find . | grep -E "
-(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf # ÃalÄ±ÅtÄ±r flatpak run
-org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r flatpak uninstall
-org.KekikAkademi.BTKSorgu ```  --- ## ð Program AkÄ±Å ÅemasÄ± 1. *Oturum
-BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/
-) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri ye,* 3. *DÃ¶nen
-kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama resmini OCR ile
-harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini okuduÄun
-doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ± ayrÄ±ÅtÄ±rÄ±p edip
-geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak kodlu olarak
-paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu **gereksiz
-kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
+U pip setuptools wheel # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ± Temizle rm -
+rf build *.egg-info # ÃalÄ±ÅtÄ±r BTKSorgu # CLI BTKSorguGUI # GUI # Paketi
+KaldÄ±r pip uninstall BTKSorgu ``` ### [https://raw.githubusercontent.com/
+keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg] FlatPak ```bash # Depoyu
+Ãek git clone https://github.com/keyiflerolsun/BTKSorgu.git cd BTKSorgu #
+Gerekli DosyalarÄ± Al mv Shared/*.yml . && mv Shared/SRC . # Gerekli OrtamlarÄ±
+Kur flatpak remote-add --if-not-exists flathub https://flathub.org/repo/
+flathub.flatpakrepo flatpak remote-add --if-not-exists flathub-beta https://
+flathub.org/beta-repo/flathub-beta.flatpakrepo flatpak update && flatpak
+upgrade flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08 # Paketle
+flatpak-builder --user --install --force-clean build-dir
+org.KekikAkademi.BTKSorgu.yml # ArtÄ±klarÄ± Temizle rm -rf .flatpak* .vscode
+build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf #
+ÃalÄ±ÅtÄ±r flatpak run org.KekikAkademi.BTKSorgu # Paketi KaldÄ±r flatpak
+uninstall org.KekikAkademi.BTKSorgu ```  --- ## ð Program AkÄ±Å ÅemasÄ± 1.
+*Oturum BaÅlat,* 2. *[https://internet2.btk.gov.tr](https://
+internet2.btk.gov.tr/) adresine yÃ¶nlendirmeleri kabul ederek git: kurabiyeleri
+ye,* 3. *DÃ¶nen kaynak kodundan doÄrulama resmini indir,* 4. *DoÄrulama
+resmini OCR ile harflere dÃ¶nÃ¼ÅtÃ¼r, boÅluklarÄ± sil,* 5. *Sorgu adresini
+okuduÄun doÄrulama koduyla birlikte post at,* 6. *DÃ¶nen yanÄ±tÄ±
+ayrÄ±ÅtÄ±rÄ±p edip geri dÃ¶ndÃ¼r..* > Bu programÄ±n yazÄ±lma ve aÃ§Ä±k kaynak
+kodlu olarak paylaÅÄ±lma amacÄ±: *TarayÄ±cÄ± OtomasyonlarÄ±nÄ±n sebep olduÄu
+**gereksiz kaynak tÃ¼ketimi** ve **zaman kaybÄ±nÄ±n** Ã¶nÃ¼ne geÃ§meye teÅvik
 etmektirâ¦* > TarayÄ±cÄ± Otomasyonu : *[Selenium IDE](https://
 www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://
 www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *
 [BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
 > KarÅÄ±laÅtÄ±rmasÄ± : **[Selenium VS Requests](https://www.r10.net/off-
 topic/2751612-selenium-vs-requests.html)** ## ð Proje Ä°lerlemesi - â **
 [@raifpy](https://github.com/raifpy)** *tarafÄ±ndan kodlanmÄ±Å projenin hantal
 bir bileÅeni itinayla `dÄ±zz ð`'lanmÄ±ÅtÄ±r..* - â **Selenium**
 *baÄÄ±mlÄ±lÄ±ÄÄ±ndan dolayÄ± hantal Ã§alÄ±Åan kod yapÄ±sÄ± tamamen
 ayÄ±klanÄ±p bÃ¼tÃ¼n iÅ* `requests`*'e yaptÄ±rÄ±lÄ±p ciddi miktarda kaynak ve
 zaman tasarrufu ettirilmiÅtir..* - â *Kolay eriÅilebilir olmasÄ± ve ilham
-yaratmasÄ± iÃ§in* **pypi** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
+yaratmasÄ± iÃ§in* **PyPI** *depolarÄ±na yÃ¼klenmiÅtir..* - â **Tkinter**
 *ile basit bir arayÃ¼z tasarlanmÄ±ÅtÄ±r ve eÄitim amacÄ±yla Depolara
+yÃ¼klenmiÅtir..* - â *Ä°lham yaratmasÄ± iÃ§in* **FlatHub** *depolarÄ±na
 yÃ¼klenmiÅtir..* ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
 [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
 PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
 BTKSorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
 â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
 mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
 ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
```

### Comparing `BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.3.1/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

 * *Files 17% similar despite different names*

#### Comparing `BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.appdata.xml` & `BTKSorgu-1.3.1/Shared/org.KekikAkademi.BTKSorgu.appdata.xml`

```diff
@@ -28,51 +28,23 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.2.9" date="2023-5-20">
-      <description>
-        <p>`tess_yukle()` fonksiyonu eklendi..</p>
-      </description>
-    </release>
-    <release version="1.2.2" date="2023-5-20">
-      <description>
-        <p>Tk Tabanı Güncellendi..</p>
-      </description>
-    </release>
-    <release version="1.1.8" date="2023-5-19">
+    <release version="1.3.1" date="2023-5-21">
       <description>
         <p>Çeşitli hatalar giderildi..</p>
         <p>Bkz.:</p>
         <ul>
           <li>Github CI/CD</li>
           <li>Tkinter CTRL+A</li>
-          <li>Tesseract Çöp Temizliği ile paket boyutunun düşürülmesi</li>
+          <li>tesseract Hata Çıktısı</li>
         </ul>
       </description>
     </release>
-    <release version="1.1.4" date="2023-5-18">
-      <description>
-        <p>Github aksiyonlarıyla otomatik paketlenme ve yayınlama eklendi..</p>
-      </description>
-    </release>
-    <release version="1.1.2" date="2023-5-18">
-      <description>
-        <p>Readme Genişletildi ve Manuel Paketleme Aşamaları Eklendi..</p>
-      </description>
-    </release>
-    <release version="1.0.8" date="2023-5-17">
-      <description>
-        <p>Readme Düzenlendi..</p>
-      </description>
-    </release>
-    <release version="1.0.5" date="2023-5-17">
-      <description>
-        <p>Proje Başlangıcı</p>
-      </description>
-    </release>
+    <release version="1.1.4" date="2023-5-18"/>
+    <release version="1.0.5" date="2023-5-17"/>
   </releases>
   <content_rating type="oars-1.1"/>
 </component>
```

### Comparing `BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.3.1/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.9/setup.py` & `BTKSorgu-1.3.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
 from setuptools import setup
 from io         import open
-from tess_yukle import TesseractYukle
 
 setup(
     # ? Genel Bilgiler
     name         = "BTKSorgu",
-    version      = "1.2.9",
+    version      = "1.3.1",
     url          = "https://github.com/keyiflerolsun/BTKSorgu",
     description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
     keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -35,32 +34,27 @@
         "cssselect",
         "regex",
         "Pillow",
         "pytesseract",
         "sv_ttk"
     ],
 
-    # ? Dışarıdan Yüklenenler
-    cmdclass = {
-        "install" : TesseractYukle
-    },
-
     # ? Konsoldan Çalıştırılabilir
     entry_points = {
         "console_scripts": [
             "BTKSorgu    = BTKSorgu.konsol:basla",
             "BTKSorguGUI = BTKSorgu.arayuz:basla"
         ]
     },
 
     # ? Masaüstü Paketi
     setup_requires = ["install_freedesktop"],
     data_files     = [
-        ("share/applications",                ["Shared/org.KekikAkademi.BTKSorgu.desktop"]),
         ("share/appdata",                     ["Shared/org.KekikAkademi.BTKSorgu.appdata.xml"]),
+        ("share/applications",                ["Shared/org.KekikAkademi.BTKSorgu.desktop"]),
         ("share/icons/hicolor/scalable/apps", ["Shared/org.KekikAkademi.BTKSorgu.svg"])
     ],
 
     # ? PyPI Bilgileri
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True
```

