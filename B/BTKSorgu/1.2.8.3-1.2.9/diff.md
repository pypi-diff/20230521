# Comparing `tmp/BTKSorgu-1.2.8.3.tar.gz` & `tmp/BTKSorgu-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-1.2.8.3.tar", last modified: Sat May 20 22:01:03 2023, max compression
+gzip compressed data, was "BTKSorgu-1.2.9.tar", last modified: Sat May 20 21:15:05 2023, max compression
```

## Comparing `BTKSorgu-1.2.8.3.tar` & `BTKSorgu-1.2.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 22:01:03.186501 BTKSorgu-1.2.8.3/
-drwxrwxrwx   0        0        0        0 2023-05-20 22:01:03.142227 BTKSorgu-1.2.8.3/BTKSorgu/
--rw-rw-rw-   0        0        0     3424 2023-05-20 20:21:20.000000 BTKSorgu-1.2.8.3/BTKSorgu/Erisim_Engeli.py
--rw-rw-rw-   0        0        0     4157 2023-05-20 20:21:20.000000 BTKSorgu-1.2.8.3/BTKSorgu/KekikGUI.py
--rw-rw-rw-   0        0        0      123 2023-05-20 20:21:20.000000 BTKSorgu-1.2.8.3/BTKSorgu/__init__.py
--rw-rw-rw-   0        0        0      174 2023-05-20 20:21:20.000000 BTKSorgu-1.2.8.3/BTKSorgu/arayuz.py
--rw-rw-rw-   0        0        0      285 2023-05-20 20:21:20.000000 BTKSorgu-1.2.8.3/BTKSorgu/ekstra.py
--rw-rw-rw-   0        0        0      624 2023-05-20 20:21:20.000000 BTKSorgu-1.2.8.3/BTKSorgu/konsol.py
--rw-rw-rw-   0        0        0    10945 2023-05-20 20:21:20.000000 BTKSorgu-1.2.8.3/BTKSorgu/logo.png
-drwxrwxrwx   0        0        0        0 2023-05-20 22:01:03.173219 BTKSorgu-1.2.8.3/BTKSorgu.egg-info/
--rw-rw-rw-   0        0        0     9272 2023-05-20 22:01:03.000000 BTKSorgu-1.2.8.3/BTKSorgu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2023-05-20 22:01:03.000000 BTKSorgu-1.2.8.3/BTKSorgu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 22:01:03.000000 BTKSorgu-1.2.8.3/BTKSorgu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-05-20 22:01:03.000000 BTKSorgu-1.2.8.3/BTKSorgu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      100 2023-05-20 22:01:03.000000 BTKSorgu-1.2.8.3/BTKSorgu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 22:01:03.000000 BTKSorgu-1.2.8.3/BTKSorgu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-05-20 20:21:20.000000 BTKSorgu-1.2.8.3/LICENSE
--rw-rw-rw-   0        0        0       28 2023-05-20 20:21:20.000000 BTKSorgu-1.2.8.3/MANIFEST.in
--rw-rw-rw-   0        0        0     9272 2023-05-20 22:01:03.184185 BTKSorgu-1.2.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     8682 2023-05-20 20:21:20.000000 BTKSorgu-1.2.8.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 22:01:03.178671 BTKSorgu-1.2.8.3/Shared/
--rw-rw-rw-   0        0        0     3191 2023-05-20 21:12:18.000000 BTKSorgu-1.2.8.3/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
--rw-rw-rw-   0        0        0      326 2023-05-20 21:12:21.000000 BTKSorgu-1.2.8.3/Shared/org.KekikAkademi.BTKSorgu.desktop
--rw-rw-rw-   0        0        0     1868 2023-05-20 20:21:20.000000 BTKSorgu-1.2.8.3/Shared/org.KekikAkademi.BTKSorgu.svg
--rw-rw-rw-   0        0        0       42 2023-05-20 22:01:03.187571 BTKSorgu-1.2.8.3/setup.cfg
--rw-rw-rw-   0        0        0     4613 2023-05-20 22:00:35.000000 BTKSorgu-1.2.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/KekikGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/ekstra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/konsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/BTKSorgu/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 21:14:30.000000 BTKSorgu-1.2.9/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 21:15:05.226631 BTKSorgu-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-20 21:14:10.000000 BTKSorgu-1.2.9/setup.py
```

### Comparing `BTKSorgu-1.2.8.3/BTKSorgu/konsol.py` & `BTKSorgu-1.2.9/BTKSorgu/konsol.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
-
-from rich         import pretty, traceback
-from rich.console import Console
-pretty.install()
-traceback.install(show_locals=False)
-konsol = Console(log_path=False)
-
-from BTKSorgu  import BTKSorgu
-from sys       import argv
-
-def basla():
-    print()
-
-    if len(argv) != 2:
-        konsol.print("[bold yellow2][!] Lütfen Domain Girin..")
-        konsol.print("\n[turquoise2]Örn.: [pale_green1]BTKSorgu redtube.com\n")
-        return
-
-    konsol.print(f"[yellow]{BTKSorgu(argv[1])}\n")
-
-if __name__ == "__main__":
+# Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
+
+from rich         import pretty, traceback
+from rich.console import Console
+pretty.install()
+traceback.install(show_locals=False)
+konsol = Console(log_path=False)
+
+from BTKSorgu  import BTKSorgu
+from sys       import argv
+
+def basla():
+    print()
+
+    if len(argv) != 2:
+        konsol.print("[bold yellow2][!] Lütfen Domain Girin..")
+        konsol.print("\n[turquoise2]Örn.: [pale_green1]BTKSorgu redtube.com\n")
+        return
+
+    konsol.print(f"[yellow]{BTKSorgu(argv[1])}\n")
+
+if __name__ == "__main__":
     basla()
```

### Comparing `BTKSorgu-1.2.8.3/BTKSorgu/logo.png` & `BTKSorgu-1.2.9/BTKSorgu/logo.png`

 * *Files identical despite different names*

### Comparing `BTKSorgu-1.2.8.3/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.2.9/BTKSorgu.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,209 +1,209 @@
-Metadata-Version: 2.1
-Name: BTKSorgu
-Version: 1.2.8.3
-Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
-Home-page: https://github.com/keyiflerolsun/BTKSorgu
-Author: keyiflerolsun
-Author-email: keyiflerolsun@gmail.com
-License: GPLv3+
-Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/org.KekikAkademi.BTKSorgu.svg"></a> BTKSorgu
-
-[![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)](#)
-[![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
-<a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
-
-[![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/releases)
-[![PyPi Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
-[![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
-
-[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
-[![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
-
-[![PyPi](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://pypi.org/project/BTKSorgu)
-[![PyPi - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
-[![PyPi - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
-
-[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white&label=Python)](#)
-[![Lisans](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#)
-[![Durum](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#)
-
-*Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
-
-[![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
-
-[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
-
-## 🚀 Kurulum
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPi (Lib - CLI - UI)
-
-```bash
-# Yüklemek
-pip install BTKSorgu
-
-# Güncellemek
-pip install -U BTKSorgu
-```
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"></a> FlatHub (UI)
-
-```bash
-# Yüklemek
-flatpak install flathub org.KekikAkademi.BTKSorgu
-
-# Çalıştırmak
-flatpak run org.KekikAkademi.BTKSorgu
-```
-
-## 📝 Kullanım
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Lib
-
-```python
-from BTKSorgu import BTKSorgu
-from time     import time
-
-basla = time()
-print(BTKSorgu("redtube.com"))
-    # » redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
-print(BTKSorgu("kekikakademi.org"))
-    # » Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
-print(BTKSorgu("xnxx.com"))
-    # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
-bitir = time()
-
-print(bitir-basla)
-    # » 8.352766513824463
-```
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"></a> CLI
-
-```bash
-BTKSorgu keyiflerolsun.dev
-
-# > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
-```
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"></a> UI
-
-```bash
-BTKSorguGUI
-
-# veya
-
-flatpak run org.KekikAkademi.BTKSorgu
-```
-
----
-
-<details>
-    <summary style="font-weight: bold; font-size: 20px">
-      <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"></a> <b>Kendiniz Paketlemek İsterseniz</b>
-      <i>(genişletmek için tıklayın!)</i>
-    </summary>
-    <br/>
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Python
-
-```bash
-# Depoyu Çek
-https://github.com/keyiflerolsun/BTKSorgu.git
-cd BTKSorgu
-
-# Gerekli Ortamları Kur
-pip install -U pip setuptools wheel twine
-
-# Paketi Yükle
-pip install .
-
-# Artıkları Temizle
-rm -rf build *.egg-info
-
-# Çalıştır
-BTKSorgu     # CLI
-BTKSorguGUI  # GUI
-
-# Paketi Kaldır
-pip uninstall BTKSorgu
-```
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"></a> FlatPak
-
-```bash
-# Depoyu Çek
-git clone https://github.com/keyiflerolsun/BTKSorgu.git
-cd BTKSorgu
-
-# Gerekli Dosyaları Al
-mv Shared/*.yml . && mv Shared/SRC .
-
-# Gerekli Ortamları Kur
-flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
-flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
-flatpak update && flatpak upgrade
-flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
-
-# Paketle
-flatpak-builder --user --install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml
-
-# Artıkları Temizle
-rm -rf .flatpak* .vscode build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf
-
-# Çalıştır
-flatpak run org.KekikAkademi.BTKSorgu
-
-# Paketi Kaldır
-flatpak uninstall org.KekikAkademi.BTKSorgu
-```
-
-</details>
-
----
-
-## 🔖 Program Akış Şeması
-
-1. *Oturum Başlat,*
-2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
-3. *Dönen kaynak kodundan doğrulama resmini indir,*
-4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
-5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
-6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
-
-> Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
-
-> Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
-
-> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
-
-## 📝 Proje İlerlemesi
-
-- ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
-- ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
-- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
-- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
-
-## 🌐 Telif Hakkı ve Lisans
-
-* *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
-* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
-
-## ♻️ İletişim
-
-*Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
-
-## 💸 Bağış Yap
-
-**[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
-
-***
-
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
+Metadata-Version: 2.1
+Name: BTKSorgu
+Version: 1.2.9
+Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
+Home-page: https://github.com/keyiflerolsun/BTKSorgu
+Author: keyiflerolsun
+Author-email: keyiflerolsun@gmail.com
+License: GPLv3+
+Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/org.KekikAkademi.BTKSorgu.svg"></a> BTKSorgu
+
+[![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)](#)
+[![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
+<a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
+
+[![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/releases)
+[![PyPi Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
+[![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
+
+[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+[![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+
+[![PyPi](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://pypi.org/project/BTKSorgu)
+[![PyPi - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
+[![PyPi - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white&label=Python)](#)
+[![Lisans](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#)
+[![Durum](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#)
+
+*Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
+
+[![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
+
+[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
+
+## 🚀 Kurulum
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPi (Lib - CLI - UI)
+
+```bash
+# Yüklemek
+pip install BTKSorgu
+
+# Güncellemek
+pip install -U BTKSorgu
+```
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"></a> FlatHub (UI)
+
+```bash
+# Yüklemek
+flatpak install flathub org.KekikAkademi.BTKSorgu
+
+# Çalıştırmak
+flatpak run org.KekikAkademi.BTKSorgu
+```
+
+## 📝 Kullanım
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Lib
+
+```python
+from BTKSorgu import BTKSorgu
+from time     import time
+
+basla = time()
+print(BTKSorgu("redtube.com"))
+    # » redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
+print(BTKSorgu("kekikakademi.org"))
+    # » Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
+print(BTKSorgu("xnxx.com"))
+    # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
+bitir = time()
+
+print(bitir-basla)
+    # » 8.352766513824463
+```
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"></a> CLI
+
+```bash
+BTKSorgu keyiflerolsun.dev
+
+# > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
+```
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"></a> UI
+
+```bash
+BTKSorguGUI
+
+# veya
+
+flatpak run org.KekikAkademi.BTKSorgu
+```
+
+---
+
+<details>
+    <summary style="font-weight: bold; font-size: 20px">
+      <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"></a> <b>Kendiniz Paketlemek İsterseniz</b>
+      <i>(genişletmek için tıklayın!)</i>
+    </summary>
+    <br/>
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Python
+
+```bash
+# Depoyu Çek
+https://github.com/keyiflerolsun/BTKSorgu.git
+cd BTKSorgu
+
+# Gerekli Ortamları Kur
+pip install -U pip setuptools wheel twine
+
+# Paketi Yükle
+pip install .
+
+# Artıkları Temizle
+rm -rf build *.egg-info
+
+# Çalıştır
+BTKSorgu     # CLI
+BTKSorguGUI  # GUI
+
+# Paketi Kaldır
+pip uninstall BTKSorgu
+```
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"></a> FlatPak
+
+```bash
+# Depoyu Çek
+git clone https://github.com/keyiflerolsun/BTKSorgu.git
+cd BTKSorgu
+
+# Gerekli Dosyaları Al
+mv Shared/*.yml . && mv Shared/SRC .
+
+# Gerekli Ortamları Kur
+flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
+flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
+flatpak update && flatpak upgrade
+flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
+
+# Paketle
+flatpak-builder --user --install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml
+
+# Artıkları Temizle
+rm -rf .flatpak* .vscode build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf
+
+# Çalıştır
+flatpak run org.KekikAkademi.BTKSorgu
+
+# Paketi Kaldır
+flatpak uninstall org.KekikAkademi.BTKSorgu
+```
+
+</details>
+
+---
+
+## 🔖 Program Akış Şeması
+
+1. *Oturum Başlat,*
+2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
+3. *Dönen kaynak kodundan doğrulama resmini indir,*
+4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
+5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
+6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
+
+> Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
+
+> Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
+
+> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
+
+## 📝 Proje İlerlemesi
+
+- ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
+- ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
+- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
+- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
+
+## 🌐 Telif Hakkı ve Lisans
+
+* *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
+* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
+
+## ♻️ İletişim
+
+*Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
+
+## 💸 Bağış Yap
+
+**[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
+
+***
+
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.8.3 Summary: Hedef
-websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://
-github.com/keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.9 Summary: Hedef websitesinin
+BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
+keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/
 Shared/org.KekikAkademi.BTKSorgu.svg] BTKSorgu [![Boyut](https://
```

### Comparing `BTKSorgu-1.2.8.3/LICENSE` & `BTKSorgu-1.2.9/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `BTKSorgu-1.2.8.3/PKG-INFO` & `BTKSorgu-1.2.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,209 +1,209 @@
-Metadata-Version: 2.1
-Name: BTKSorgu
-Version: 1.2.8.3
-Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
-Home-page: https://github.com/keyiflerolsun/BTKSorgu
-Author: keyiflerolsun
-Author-email: keyiflerolsun@gmail.com
-License: GPLv3+
-Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/org.KekikAkademi.BTKSorgu.svg"></a> BTKSorgu
-
-[![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)](#)
-[![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
-<a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
-
-[![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/releases)
-[![PyPi Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
-[![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
-
-[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
-[![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
-
-[![PyPi](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://pypi.org/project/BTKSorgu)
-[![PyPi - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
-[![PyPi - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
-
-[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white&label=Python)](#)
-[![Lisans](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#)
-[![Durum](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#)
-
-*Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
-
-[![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
-
-[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
-
-## 🚀 Kurulum
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPi (Lib - CLI - UI)
-
-```bash
-# Yüklemek
-pip install BTKSorgu
-
-# Güncellemek
-pip install -U BTKSorgu
-```
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"></a> FlatHub (UI)
-
-```bash
-# Yüklemek
-flatpak install flathub org.KekikAkademi.BTKSorgu
-
-# Çalıştırmak
-flatpak run org.KekikAkademi.BTKSorgu
-```
-
-## 📝 Kullanım
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Lib
-
-```python
-from BTKSorgu import BTKSorgu
-from time     import time
-
-basla = time()
-print(BTKSorgu("redtube.com"))
-    # » redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
-print(BTKSorgu("kekikakademi.org"))
-    # » Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
-print(BTKSorgu("xnxx.com"))
-    # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
-bitir = time()
-
-print(bitir-basla)
-    # » 8.352766513824463
-```
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"></a> CLI
-
-```bash
-BTKSorgu keyiflerolsun.dev
-
-# > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
-```
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"></a> UI
-
-```bash
-BTKSorguGUI
-
-# veya
-
-flatpak run org.KekikAkademi.BTKSorgu
-```
-
----
-
-<details>
-    <summary style="font-weight: bold; font-size: 20px">
-      <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"></a> <b>Kendiniz Paketlemek İsterseniz</b>
-      <i>(genişletmek için tıklayın!)</i>
-    </summary>
-    <br/>
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Python
-
-```bash
-# Depoyu Çek
-https://github.com/keyiflerolsun/BTKSorgu.git
-cd BTKSorgu
-
-# Gerekli Ortamları Kur
-pip install -U pip setuptools wheel twine
-
-# Paketi Yükle
-pip install .
-
-# Artıkları Temizle
-rm -rf build *.egg-info
-
-# Çalıştır
-BTKSorgu     # CLI
-BTKSorguGUI  # GUI
-
-# Paketi Kaldır
-pip uninstall BTKSorgu
-```
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"></a> FlatPak
-
-```bash
-# Depoyu Çek
-git clone https://github.com/keyiflerolsun/BTKSorgu.git
-cd BTKSorgu
-
-# Gerekli Dosyaları Al
-mv Shared/*.yml . && mv Shared/SRC .
-
-# Gerekli Ortamları Kur
-flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
-flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
-flatpak update && flatpak upgrade
-flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
-
-# Paketle
-flatpak-builder --user --install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml
-
-# Artıkları Temizle
-rm -rf .flatpak* .vscode build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf
-
-# Çalıştır
-flatpak run org.KekikAkademi.BTKSorgu
-
-# Paketi Kaldır
-flatpak uninstall org.KekikAkademi.BTKSorgu
-```
-
-</details>
-
----
-
-## 🔖 Program Akış Şeması
-
-1. *Oturum Başlat,*
-2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
-3. *Dönen kaynak kodundan doğrulama resmini indir,*
-4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
-5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
-6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
-
-> Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
-
-> Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
-
-> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
-
-## 📝 Proje İlerlemesi
-
-- ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
-- ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
-- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
-- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
-
-## 🌐 Telif Hakkı ve Lisans
-
-* *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
-* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
-
-## ♻️ İletişim
-
-*Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
-
-## 💸 Bağış Yap
-
-**[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
-
-***
-
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
+Metadata-Version: 2.1
+Name: BTKSorgu
+Version: 1.2.9
+Summary: Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
+Home-page: https://github.com/keyiflerolsun/BTKSorgu
+Author: keyiflerolsun
+Author-email: keyiflerolsun@gmail.com
+License: GPLv3+
+Keywords: BTKSorgu,KekikAkademi,keyiflerolsun
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/org.KekikAkademi.BTKSorgu.svg"></a> BTKSorgu
+
+[![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)](#)
+[![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
+<a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
+
+[![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/releases)
+[![PyPi Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
+[![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
+
+[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+[![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+
+[![PyPi](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://pypi.org/project/BTKSorgu)
+[![PyPi - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
+[![PyPi - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white&label=Python)](#)
+[![Lisans](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#)
+[![Durum](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#)
+
+*Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
+
+[![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
+
+[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
+
+## 🚀 Kurulum
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPi (Lib - CLI - UI)
+
+```bash
+# Yüklemek
+pip install BTKSorgu
+
+# Güncellemek
+pip install -U BTKSorgu
+```
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"></a> FlatHub (UI)
+
+```bash
+# Yüklemek
+flatpak install flathub org.KekikAkademi.BTKSorgu
+
+# Çalıştırmak
+flatpak run org.KekikAkademi.BTKSorgu
+```
+
+## 📝 Kullanım
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Lib
+
+```python
+from BTKSorgu import BTKSorgu
+from time     import time
+
+basla = time()
+print(BTKSorgu("redtube.com"))
+    # » redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
+print(BTKSorgu("kekikakademi.org"))
+    # » Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
+print(BTKSorgu("xnxx.com"))
+    # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
+bitir = time()
+
+print(bitir-basla)
+    # » 8.352766513824463
+```
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"></a> CLI
+
+```bash
+BTKSorgu keyiflerolsun.dev
+
+# > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
+```
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"></a> UI
+
+```bash
+BTKSorguGUI
+
+# veya
+
+flatpak run org.KekikAkademi.BTKSorgu
+```
+
+---
+
+<details>
+    <summary style="font-weight: bold; font-size: 20px">
+      <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"></a> <b>Kendiniz Paketlemek İsterseniz</b>
+      <i>(genişletmek için tıklayın!)</i>
+    </summary>
+    <br/>
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Python
+
+```bash
+# Depoyu Çek
+https://github.com/keyiflerolsun/BTKSorgu.git
+cd BTKSorgu
+
+# Gerekli Ortamları Kur
+pip install -U pip setuptools wheel twine
+
+# Paketi Yükle
+pip install .
+
+# Artıkları Temizle
+rm -rf build *.egg-info
+
+# Çalıştır
+BTKSorgu     # CLI
+BTKSorguGUI  # GUI
+
+# Paketi Kaldır
+pip uninstall BTKSorgu
+```
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"></a> FlatPak
+
+```bash
+# Depoyu Çek
+git clone https://github.com/keyiflerolsun/BTKSorgu.git
+cd BTKSorgu
+
+# Gerekli Dosyaları Al
+mv Shared/*.yml . && mv Shared/SRC .
+
+# Gerekli Ortamları Kur
+flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
+flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
+flatpak update && flatpak upgrade
+flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
+
+# Paketle
+flatpak-builder --user --install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml
+
+# Artıkları Temizle
+rm -rf .flatpak* .vscode build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf
+
+# Çalıştır
+flatpak run org.KekikAkademi.BTKSorgu
+
+# Paketi Kaldır
+flatpak uninstall org.KekikAkademi.BTKSorgu
+```
+
+</details>
+
+---
+
+## 🔖 Program Akış Şeması
+
+1. *Oturum Başlat,*
+2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
+3. *Dönen kaynak kodundan doğrulama resmini indir,*
+4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
+5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
+6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
+
+> Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
+
+> Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
+
+> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
+
+## 📝 Proje İlerlemesi
+
+- ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
+- ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
+- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
+- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
+
+## 🌐 Telif Hakkı ve Lisans
+
+* *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
+* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
+
+## ♻️ İletişim
+
+*Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
+
+## 💸 Bağış Yap
+
+**[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
+
+***
+
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.8.3 Summary: Hedef
-websitesinin BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://
-github.com/keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
+Metadata-Version: 2.1 Name: BTKSorgu Version: 1.2.9 Summary: Hedef websitesinin
+BTK TarafÄ±ndan EriÅim Engeli Sorgusu Home-page: https://github.com/
+keyiflerolsun/BTKSorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 BTKSorgu,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # [https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/
 Shared/org.KekikAkademi.BTKSorgu.svg] BTKSorgu [![Boyut](https://
```

### Comparing `BTKSorgu-1.2.8.3/README.md` & `BTKSorgu-1.2.9/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-# <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/org.KekikAkademi.BTKSorgu.svg"></a> BTKSorgu
-
-[![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)](#)
-[![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
-<a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
-
-[![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/releases)
-[![PyPi Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
-[![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
-
-[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
-[![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
-
-[![PyPi](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://pypi.org/project/BTKSorgu)
-[![PyPi - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
-[![PyPi - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
-
-[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white&label=Python)](#)
-[![Lisans](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#)
-[![Durum](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#)
-
-*Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
-
-[![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
-
-[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
-
-## 🚀 Kurulum
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPi (Lib - CLI - UI)
-
-```bash
-# Yüklemek
-pip install BTKSorgu
-
-# Güncellemek
-pip install -U BTKSorgu
-```
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"></a> FlatHub (UI)
-
-```bash
-# Yüklemek
-flatpak install flathub org.KekikAkademi.BTKSorgu
-
-# Çalıştırmak
-flatpak run org.KekikAkademi.BTKSorgu
-```
-
-## 📝 Kullanım
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Lib
-
-```python
-from BTKSorgu import BTKSorgu
-from time     import time
-
-basla = time()
-print(BTKSorgu("redtube.com"))
-    # » redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
-print(BTKSorgu("kekikakademi.org"))
-    # » Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
-print(BTKSorgu("xnxx.com"))
-    # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
-bitir = time()
-
-print(bitir-basla)
-    # » 8.352766513824463
-```
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"></a> CLI
-
-```bash
-BTKSorgu keyiflerolsun.dev
-
-# > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
-```
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"></a> UI
-
-```bash
-BTKSorguGUI
-
-# veya
-
-flatpak run org.KekikAkademi.BTKSorgu
-```
-
----
-
-<details>
-    <summary style="font-weight: bold; font-size: 20px">
-      <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"></a> <b>Kendiniz Paketlemek İsterseniz</b>
-      <i>(genişletmek için tıklayın!)</i>
-    </summary>
-    <br/>
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Python
-
-```bash
-# Depoyu Çek
-https://github.com/keyiflerolsun/BTKSorgu.git
-cd BTKSorgu
-
-# Gerekli Ortamları Kur
-pip install -U pip setuptools wheel twine
-
-# Paketi Yükle
-pip install .
-
-# Artıkları Temizle
-rm -rf build *.egg-info
-
-# Çalıştır
-BTKSorgu     # CLI
-BTKSorguGUI  # GUI
-
-# Paketi Kaldır
-pip uninstall BTKSorgu
-```
-
-### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"></a> FlatPak
-
-```bash
-# Depoyu Çek
-git clone https://github.com/keyiflerolsun/BTKSorgu.git
-cd BTKSorgu
-
-# Gerekli Dosyaları Al
-mv Shared/*.yml . && mv Shared/SRC .
-
-# Gerekli Ortamları Kur
-flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
-flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
-flatpak update && flatpak upgrade
-flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
-
-# Paketle
-flatpak-builder --user --install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml
-
-# Artıkları Temizle
-rm -rf .flatpak* .vscode build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf
-
-# Çalıştır
-flatpak run org.KekikAkademi.BTKSorgu
-
-# Paketi Kaldır
-flatpak uninstall org.KekikAkademi.BTKSorgu
-```
-
-</details>
-
----
-
-## 🔖 Program Akış Şeması
-
-1. *Oturum Başlat,*
-2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
-3. *Dönen kaynak kodundan doğrulama resmini indir,*
-4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
-5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
-6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
-
-> Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
-
-> Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
-
-> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
-
-## 📝 Proje İlerlemesi
-
-- ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
-- ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
-- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
-- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
-
-## 🌐 Telif Hakkı ve Lisans
-
-* *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
-* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
-
-## ♻️ İletişim
-
-*Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
-
-## 💸 Bağış Yap
-
-**[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
-
-***
-
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
+# <a href="#"><img width="32" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/Shared/org.KekikAkademi.BTKSorgu.svg"></a> BTKSorgu
+
+[![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/BTKSorgu?logo=git&logoColor=white&label=Boyut)](#)
+[![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/BTKSorgu&title=Görüntülenme)](#)
+<a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
+
+[![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/BTKSorgu?logo=github&label=GitHub)](https://github.com/keyiflerolsun/BTKSorgu/releases)
+[![PyPi Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/pypiYukle.yml?label=PyPi%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/pypiYukle.yml)
+[![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/BTKSorgu/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/BTKSorgu/actions/workflows/flatpakYukle.yml)
+
+[![FlatHub](https://img.shields.io/flathub/v/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=FlatHub)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+[![FlatHub - Yüklenme](https://img.shields.io/flathub/downloads/org.KekikAkademi.BTKSorgu?logo=flathub&logoColor=white&label=Yüklenme)](https://flathub.org/tr/apps/org.KekikAkademi.BTKSorgu)
+
+[![PyPi](https://img.shields.io/pypi/v/BTKSorgu?logo=pypi&logoColor=white&label=PyPi)](https://pypi.org/project/BTKSorgu)
+[![PyPi - Yüklenme](https://img.shields.io/pypi/dm/BTKSorgu?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/BTKSorgu)
+[![PyPi - Wheel](https://img.shields.io/pypi/wheel/BTKSorgu?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/BTKSorgu)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/BTKSorgu?logo=python&logoColor=white&label=Python)](#)
+[![Lisans](https://img.shields.io/pypi/l/BTKSorgu?logo=gnu&logoColor=white&label=Lisans)](#)
+[![Durum](https://img.shields.io/pypi/status/BTKSorgu?logo=windowsterminal&logoColor=white&label=Durum)](#)
+
+*Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu..*
+
+[![BTKSorgu](https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/SS.png)](#)
+
+[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
+
+## 🚀 Kurulum
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/pypi.svg"></a> PyPi (Lib - CLI - UI)
+
+```bash
+# Yüklemek
+pip install BTKSorgu
+
+# Güncellemek
+pip install -U BTKSorgu
+```
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flathub.svg"></a> FlatHub (UI)
+
+```bash
+# Yüklemek
+flatpak install flathub org.KekikAkademi.BTKSorgu
+
+# Çalıştırmak
+flatpak run org.KekikAkademi.BTKSorgu
+```
+
+## 📝 Kullanım
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Lib
+
+```python
+from BTKSorgu import BTKSorgu
+from time     import time
+
+basla = time()
+print(BTKSorgu("redtube.com"))
+    # » redtube.com, 30/01/2008 tarihli ve 410.01.02.2008-028105 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
+print(BTKSorgu("kekikakademi.org"))
+    # » Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
+print(BTKSorgu("xnxx.com"))
+    # » xnxx.com, 23/02/2008 tarihli ve 410.01.02.2008-054003 sayılı Telekomünikasyon İletişim Başkanlığı kararıyla erişime engellenmiştir.
+bitir = time()
+
+print(bitir-basla)
+    # » 8.352766513824463
+```
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/iterm2.svg"></a> CLI
+
+```bash
+BTKSorgu keyiflerolsun.dev
+
+# > Bilgi Teknolojileri ve İletişim Kurumu tarafından uygulanan bir karar bulunamadı.
+```
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/freedesktop.svg"></a> UI
+
+```bash
+BTKSorguGUI
+
+# veya
+
+flatpak run org.KekikAkademi.BTKSorgu
+```
+
+---
+
+<details>
+    <summary style="font-weight: bold; font-size: 20px">
+      <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/buddy.svg"></a> <b>Kendiniz Paketlemek İsterseniz</b>
+      <i>(genişletmek için tıklayın!)</i>
+    </summary>
+    <br/>
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/python.svg"></a> Python
+
+```bash
+# Depoyu Çek
+https://github.com/keyiflerolsun/BTKSorgu.git
+cd BTKSorgu
+
+# Gerekli Ortamları Kur
+pip install -U pip setuptools wheel twine
+
+# Paketi Yükle
+pip install .
+
+# Artıkları Temizle
+rm -rf build *.egg-info
+
+# Çalıştır
+BTKSorgu     # CLI
+BTKSorguGUI  # GUI
+
+# Paketi Kaldır
+pip uninstall BTKSorgu
+```
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/BTKSorgu/main/.github/icons/flatpak.svg"></a> FlatPak
+
+```bash
+# Depoyu Çek
+git clone https://github.com/keyiflerolsun/BTKSorgu.git
+cd BTKSorgu
+
+# Gerekli Dosyaları Al
+mv Shared/*.yml . && mv Shared/SRC .
+
+# Gerekli Ortamları Kur
+flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
+flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
+flatpak update && flatpak upgrade
+flatpak install flathub org.freedesktop.{Platform,Sdk}//22.08
+
+# Paketle
+flatpak-builder --user --install --force-clean build-dir org.KekikAkademi.BTKSorgu.yml
+
+# Artıkları Temizle
+rm -rf .flatpak* .vscode build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf
+
+# Çalıştır
+flatpak run org.KekikAkademi.BTKSorgu
+
+# Paketi Kaldır
+flatpak uninstall org.KekikAkademi.BTKSorgu
+```
+
+</details>
+
+---
+
+## 🔖 Program Akış Şeması
+
+1. *Oturum Başlat,*
+2. *[https://internet2.btk.gov.tr](https://internet2.btk.gov.tr/) adresine yönlendirmeleri kabul ederek git: kurabiyeleri ye,*
+3. *Dönen kaynak kodundan doğrulama resmini indir,*
+4. *Doğrulama resmini OCR ile harflere dönüştür, boşlukları sil,*
+5. *Sorgu adresini okuduğun doğrulama koduyla birlikte post at,*
+6. *Dönen yanıtı ayrıştırıp edip geri döndür..*
+
+> Bu programın yazılma ve açık kaynak kodlu olarak paylaşılma amacı: *Tarayıcı Otomasyonlarının sebep olduğu  **gereksiz kaynak tüketimi** ve  **zaman kaybının**  önüne geçmeye teşvik etmektir…*
+
+> Tarayıcı Otomasyonu : *[Selenium IDE](https://www.selenium.dev/selenium-ide/)* **-** *[Katalon Automation Recorder](https://www.katalon.com/resources-center/blog/katalon-automation-recorder/)* **-** *[BrowserAutomationStudio](https://bablosoft.com/shop/BrowserAutomationStudio)*
+
+> Karşılaştırması : **[Selenium VS Requests](https://www.r10.net/off-topic/2751612-selenium-vs-requests.html)**
+
+## 📝 Proje İlerlemesi
+
+- ✅ **[@raifpy](https://github.com/raifpy)** *tarafından kodlanmış projenin hantal bir bileşeni itinayla `dızz 🐍`'lanmıştır..*
+- ✅ **Selenium** *bağımlılığından dolayı hantal çalışan kod yapısı tamamen ayıklanıp bütün iş* `requests`*'e yaptırılıp ciddi miktarda kaynak ve zaman tasarrufu ettirilmiştir..*
+- ✅ *Kolay erişilebilir olması ve ilham yaratması için* **pypi** *depolarına yüklenmiştir..*
+- ✅ **Tkinter** *ile basit bir arayüz tasarlanmıştır ve eğitim amacıyla Depolara yüklenmiştir..*
+
+## 🌐 Telif Hakkı ve Lisans
+
+* *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
+* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/BTKSorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
+
+## ♻️ İletişim
+
+*Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
+
+## 💸 Bağış Yap
+
+**[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
+
+***
+
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

### Comparing `BTKSorgu-1.2.8.3/Shared/org.KekikAkademi.BTKSorgu.svg` & `BTKSorgu-1.2.9/Shared/org.KekikAkademi.BTKSorgu.svg`

 * *Files 3% similar despite different names*

```diff
@@ -4,114 +4,114 @@
 00000030: 2077 6964 7468 3d22 3530 7078 2220 6865   width="50px" he
 00000040: 6967 6874 3d22 3530 7078 2220 7072 6573  ight="50px" pres
 00000050: 6572 7665 4173 7065 6374 5261 7469 6f3d  erveAspectRatio=
 00000060: 226e 6f6e 6522 2076 6965 7742 6f78 3d22  "none" viewBox="
 00000070: 352e 3632 3920 372e 3734 3120 3230 3020  5.629 7.741 200 
 00000080: 3230 3022 2078 6d6c 6e73 3d22 6874 7470  200" xmlns="http
 00000090: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
-000000a0: 3030 2f73 7667 223e 0d0a 2020 3c64 6566  00/svg">..  <def
-000000b0: 733e 3c2f 6465 6673 3e0d 0a20 203c 6720  s></defs>..  <g 
-000000c0: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
-000000d0: 7828 312c 2030 2c20 302c 2031 2c20 2d36  x(1, 0, 0, 1, -6
-000000e0: 342e 3731 3537 3539 2c20 2d33 312e 3630  4.715759, -31.60
-000000f0: 3435 3039 2922 3e0d 0a20 2020 203c 706f  4509)">..    <po
-00000100: 6c79 676f 6e20 706f 696e 7473 3d22 3139  lygon points="19
-00000110: 392e 3339 3620 3134 362e 3838 3120 3138  9.396 146.881 18
-00000120: 382e 3235 3520 3134 322e 3634 3720 3138  8.255 142.647 18
-00000130: 382e 3832 3820 3133 302e 3733 3720 3138  8.828 130.737 18
-00000140: 312e 3338 3220 3134 302e 3037 3320 3137  1.382 140.073 17
-00000150: 302e 3230 3420 3133 352e 3833 3820 3137  0.204 135.838 17
-00000160: 362e 3733 3420 3134 352e 3830 3420 3136  6.734 145.804 16
-00000170: 392e 3330 3920 3135 352e 3135 3320 3138  9.309 155.153 18
-00000180: 302e 3833 3720 3135 312e 3935 3620 3138  0.837 151.956 18
-00000190: 372e 3335 3520 3136 312e 3932 2031 3837  7.355 161.92 187
-000001a0: 2e39 3132 2031 3439 2e39 3932 2220 7374  .912 149.992" st
-000001b0: 796c 653d 2222 3e3c 2f70 6f6c 7967 6f6e  yle=""></polygon
-000001c0: 3e0d 0a20 2020 203c 706f 6c79 676f 6e20  >..    <polygon 
-000001d0: 706f 696e 7473 3d22 3138 302e 3230 3620  points="180.206 
-000001e0: 3837 2e38 3437 2031 3730 2e36 3331 2039  87.847 170.631 9
-000001f0: 382e 3138 2031 3730 2e36 3331 2031 3333  8.18 170.631 133
-00000200: 2e38 3938 2031 3830 2e32 3036 2031 3234  .898 180.206 124
-00000210: 2e37 3738 2220 7374 796c 653d 2222 3e3c  .778" style=""><
-00000220: 2f70 6f6c 7967 6f6e 3e0d 0a20 2020 203c  /polygon>..    <
-00000230: 706f 6c79 676f 6e20 706f 696e 7473 3d22  polygon points="
-00000240: 3132 382e 3038 3420 3631 2e32 3238 2031  128.084 61.228 1
-00000250: 3238 2e30 3834 2031 3438 2e39 3838 2031  28.084 148.988 1
-00000260: 3337 2e36 3539 2031 3538 2e31 3039 2031  37.659 158.109 1
-00000270: 3337 2e36 3539 2037 312e 3536 3122 2073  37.659 71.561" s
-00000280: 7479 6c65 3d22 223e 3c2f 706f 6c79 676f  tyle=""></polygo
-00000290: 6e3e 0d0a 2020 2020 3c70 6174 6820 643d  n>..    <path d=
-000002a0: 224d 2031 3531 2e33 3631 2038 322e 3339  "M 151.361 82.39
-000002b0: 3520 4c20 3134 312e 3731 3420 3732 2e34  5 L 141.714 72.4
-000002c0: 3638 204c 2031 3431 2e37 3134 2037 382e  68 L 141.714 78.
-000002d0: 3031 3720 4c20 3134 312e 3731 3420 3133  017 L 141.714 13
-000002e0: 312e 3137 3720 4c20 3134 312e 3731 3120  1.177 L 141.711 
-000002f0: 3133 312e 3137 3720 4c20 3134 312e 3731  131.177 L 141.71
-00000300: 3120 3133 362e 3732 3720 4c20 3134 312e  1 136.727 L 141.
-00000310: 3731 3120 3136 362e 3731 3220 4c20 3134  711 166.712 L 14
-00000320: 312e 3731 3120 3137 322e 3236 3220 4c20  1.711 172.262 L 
-00000330: 3134 312e 3731 3420 3137 322e 3236 3220  141.714 172.262 
-00000340: 4c20 3134 312e 3731 3420 3137 322e 3238  L 141.714 172.28
-00000350: 3220 4c20 3134 312e 3731 3420 3137 362e  2 L 141.714 176.
-00000360: 3639 3920 4320 3134 312e 3732 3920 3137  699 C 141.729 17
-00000370: 372e 3033 3620 3134 312e 3735 3920 3137  7.036 141.759 17
-00000380: 372e 3337 2031 3431 2e37 3833 2031 3737  7.37 141.783 177
-00000390: 2e37 3034 204c 2031 3431 2e38 3431 2031  .704 L 141.841 1
-000003a0: 3832 2e32 3438 2043 2031 3432 2e32 3238  82.248 C 142.228
-000003b0: 2031 3931 2e30 3532 2031 3435 2e37 3639   191.052 145.769
-000003c0: 2031 3939 2e30 3334 2031 3531 2e33 3631   199.034 151.361
-000003d0: 2032 3035 2e30 3937 204c 2031 3531 2e33   205.097 L 151.3
-000003e0: 3631 2038 322e 3339 3520 5a22 2073 7479  61 82.395 Z" sty
-000003f0: 6c65 3d22 223e 3c2f 7061 7468 3e0d 0a20  le=""></path>.. 
-00000400: 2020 203c 7061 7468 2064 3d22 4d20 3136     <path d="M 16
-00000410: 352e 3735 2031 3631 2e38 3835 204c 2031  5.75 161.885 L 1
-00000420: 3635 2e38 3531 2031 3631 2e38 3835 204c  65.851 161.885 L
-00000430: 2031 3635 2e38 3531 2031 3339 2e39 3332   165.851 139.932
-00000440: 204c 2031 3635 2e38 3531 2031 3334 2e33   L 165.851 134.3
-00000450: 3832 204c 2031 3635 2e38 3420 3133 342e  82 L 165.84 134.
-00000460: 3339 3320 4c20 3136 352e 3834 2039 372e  393 L 165.84 97.
-00000470: 3239 3720 4c20 3135 362e 3336 2038 372e  297 L 156.36 87.
-00000480: 3534 3120 4c20 3135 362e 3336 2032 3039  541 L 156.36 209
-00000490: 2e36 2043 2031 3539 2e31 3434 2032 3131  .6 C 159.144 211
-000004a0: 2e36 3732 2031 3632 2e32 3336 2032 3133  .672 162.236 213
-000004b0: 2e33 3535 2031 3635 2e35 3536 2032 3134  .355 165.556 214
-000004c0: 2e35 3633 2043 2031 3635 2e36 3231 2032  .563 C 165.621 2
-000004d0: 3134 2e35 3932 2031 3635 2e36 3836 2032  14.592 165.686 2
-000004e0: 3134 2e36 3137 2031 3635 2e37 3531 2032  14.617 165.751 2
-000004f0: 3134 2e36 3435 204c 2031 3635 2e37 3531  14.645 L 165.751
-00000500: 2031 3631 2e38 3835 204c 2031 3635 2e37   161.885 L 165.7
-00000510: 3520 3136 312e 3838 3520 5a22 2073 7479  5 161.885 Z" sty
-00000520: 6c65 3d22 223e 3c2f 7061 7468 3e0d 0a20  le=""></path>.. 
-00000530: 2020 203c 7061 7468 2064 3d22 4d20 3231     <path d="M 21
-00000540: 312e 3934 3120 3137 372e 3331 3720 4320  1.941 177.317 C 
-00000550: 3230 392e 3531 3720 3136 352e 3631 3220  209.517 165.612 
-00000560: 3230 312e 3336 3920 3135 362e 3634 3220  201.369 156.642 
-00000570: 3139 302e 3939 3820 3135 322e 3639 3920  190.998 152.699 
-00000580: 4320 3139 322e 3134 3620 3135 332e 3337  C 192.146 153.37
-00000590: 3720 3139 332e 3234 3420 3135 342e 3134  7 193.244 154.14
-000005a0: 3120 3139 342e 3238 3420 3135 342e 3938  1 194.284 154.98
-000005b0: 3220 4320 3139 372e 3935 3220 3135 382e  2 C 197.952 158.
-000005c0: 3236 3920 3230 302e 3331 3120 3136 332e  269 200.311 163.
-000005d0: 3032 3920 3230 302e 3334 3520 3136 382e  029 200.345 168.
-000005e0: 3337 3120 4320 3230 302e 3432 3320 3137  371 C 200.423 17
-000005f0: 382e 3336 3520 3139 322e 3335 3520 3138  8.365 192.355 18
-00000600: 362e 3533 3320 3138 322e 3336 3820 3138  6.533 182.368 18
-00000610: 362e 3538 3720 4320 3137 372e 3734 3820  6.587 C 177.748 
-00000620: 3138 362e 3633 3120 3137 332e 3836 2031  186.631 173.86 1
-00000630: 3834 2e38 3534 2031 3731 2e30 3037 2031  84.854 171.007 1
-00000640: 3831 2e39 3433 204c 2031 3731 2e30 3037  81.943 L 171.007
-00000650: 2032 3136 2e34 3437 2043 2031 3735 2e37   216.447 C 175.7
-00000660: 3120 3231 372e 3633 3420 3138 302e 3734  1 217.634 180.74
-00000670: 3120 3231 372e 3832 3220 3138 352e 3830  1 217.822 185.80
-00000680: 3920 3231 362e 3739 3320 4320 3139 362e  9 216.793 C 196.
-00000690: 3634 3720 3231 342e 3538 3420 3230 352e  647 214.584 205.
-000006a0: 3136 3920 3230 372e 3336 3120 3230 392e  169 207.361 209.
-000006b0: 3439 2031 3938 2e30 3434 2043 2032 3039  49 198.044 C 209
-000006c0: 2e36 3434 2031 3937 2e37 3634 2032 3039  .644 197.764 209
-000006d0: 2e37 3938 2031 3937 2e34 3834 2032 3039  .798 197.484 209
-000006e0: 2e39 3435 2031 3937 2e32 204c 2032 3039  .945 197.2 L 209
-000006f0: 2e38 3634 2031 3937 2e32 2043 2032 3132  .864 197.2 C 212
-00000700: 2e34 3735 2031 3931 2e31 3432 2032 3133  .475 191.142 213
-00000710: 2e33 3420 3138 342e 3236 2032 3131 2e39  .34 184.26 211.9
-00000720: 3431 2031 3737 2e33 3137 2220 7374 796c  41 177.317" styl
-00000730: 653d 2222 3e3c 2f70 6174 683e 0d0a 2020  e=""></path>..  
-00000740: 3c2f 673e 0d0a 3c2f 7376 673e            </g>..</svg>
+000000a0: 3030 2f73 7667 223e 0a20 203c 6465 6673  00/svg">.  <defs
+000000b0: 3e3c 2f64 6566 733e 0a20 203c 6720 7472  ></defs>.  <g tr
+000000c0: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
+000000d0: 312c 2030 2c20 302c 2031 2c20 2d36 342e  1, 0, 0, 1, -64.
+000000e0: 3731 3537 3539 2c20 2d33 312e 3630 3435  715759, -31.6045
+000000f0: 3039 2922 3e0a 2020 2020 3c70 6f6c 7967  09)">.    <polyg
+00000100: 6f6e 2070 6f69 6e74 733d 2231 3939 2e33  on points="199.3
+00000110: 3936 2031 3436 2e38 3831 2031 3838 2e32  96 146.881 188.2
+00000120: 3535 2031 3432 2e36 3437 2031 3838 2e38  55 142.647 188.8
+00000130: 3238 2031 3330 2e37 3337 2031 3831 2e33  28 130.737 181.3
+00000140: 3832 2031 3430 2e30 3733 2031 3730 2e32  82 140.073 170.2
+00000150: 3034 2031 3335 2e38 3338 2031 3736 2e37  04 135.838 176.7
+00000160: 3334 2031 3435 2e38 3034 2031 3639 2e33  34 145.804 169.3
+00000170: 3039 2031 3535 2e31 3533 2031 3830 2e38  09 155.153 180.8
+00000180: 3337 2031 3531 2e39 3536 2031 3837 2e33  37 151.956 187.3
+00000190: 3535 2031 3631 2e39 3220 3138 372e 3931  55 161.92 187.91
+000001a0: 3220 3134 392e 3939 3222 2073 7479 6c65  2 149.992" style
+000001b0: 3d22 223e 3c2f 706f 6c79 676f 6e3e 0a20  =""></polygon>. 
+000001c0: 2020 203c 706f 6c79 676f 6e20 706f 696e     <polygon poin
+000001d0: 7473 3d22 3138 302e 3230 3620 3837 2e38  ts="180.206 87.8
+000001e0: 3437 2031 3730 2e36 3331 2039 382e 3138  47 170.631 98.18
+000001f0: 2031 3730 2e36 3331 2031 3333 2e38 3938   170.631 133.898
+00000200: 2031 3830 2e32 3036 2031 3234 2e37 3738   180.206 124.778
+00000210: 2220 7374 796c 653d 2222 3e3c 2f70 6f6c  " style=""></pol
+00000220: 7967 6f6e 3e0a 2020 2020 3c70 6f6c 7967  ygon>.    <polyg
+00000230: 6f6e 2070 6f69 6e74 733d 2231 3238 2e30  on points="128.0
+00000240: 3834 2036 312e 3232 3820 3132 382e 3038  84 61.228 128.08
+00000250: 3420 3134 382e 3938 3820 3133 372e 3635  4 148.988 137.65
+00000260: 3920 3135 382e 3130 3920 3133 372e 3635  9 158.109 137.65
+00000270: 3920 3731 2e35 3631 2220 7374 796c 653d  9 71.561" style=
+00000280: 2222 3e3c 2f70 6f6c 7967 6f6e 3e0a 2020  ""></polygon>.  
+00000290: 2020 3c70 6174 6820 643d 224d 2031 3531    <path d="M 151
+000002a0: 2e33 3631 2038 322e 3339 3520 4c20 3134  .361 82.395 L 14
+000002b0: 312e 3731 3420 3732 2e34 3638 204c 2031  1.714 72.468 L 1
+000002c0: 3431 2e37 3134 2037 382e 3031 3720 4c20  41.714 78.017 L 
+000002d0: 3134 312e 3731 3420 3133 312e 3137 3720  141.714 131.177 
+000002e0: 4c20 3134 312e 3731 3120 3133 312e 3137  L 141.711 131.17
+000002f0: 3720 4c20 3134 312e 3731 3120 3133 362e  7 L 141.711 136.
+00000300: 3732 3720 4c20 3134 312e 3731 3120 3136  727 L 141.711 16
+00000310: 362e 3731 3220 4c20 3134 312e 3731 3120  6.712 L 141.711 
+00000320: 3137 322e 3236 3220 4c20 3134 312e 3731  172.262 L 141.71
+00000330: 3420 3137 322e 3236 3220 4c20 3134 312e  4 172.262 L 141.
+00000340: 3731 3420 3137 322e 3238 3220 4c20 3134  714 172.282 L 14
+00000350: 312e 3731 3420 3137 362e 3639 3920 4320  1.714 176.699 C 
+00000360: 3134 312e 3732 3920 3137 372e 3033 3620  141.729 177.036 
+00000370: 3134 312e 3735 3920 3137 372e 3337 2031  141.759 177.37 1
+00000380: 3431 2e37 3833 2031 3737 2e37 3034 204c  41.783 177.704 L
+00000390: 2031 3431 2e38 3431 2031 3832 2e32 3438   141.841 182.248
+000003a0: 2043 2031 3432 2e32 3238 2031 3931 2e30   C 142.228 191.0
+000003b0: 3532 2031 3435 2e37 3639 2031 3939 2e30  52 145.769 199.0
+000003c0: 3334 2031 3531 2e33 3631 2032 3035 2e30  34 151.361 205.0
+000003d0: 3937 204c 2031 3531 2e33 3631 2038 322e  97 L 151.361 82.
+000003e0: 3339 3520 5a22 2073 7479 6c65 3d22 223e  395 Z" style="">
+000003f0: 3c2f 7061 7468 3e0a 2020 2020 3c70 6174  </path>.    <pat
+00000400: 6820 643d 224d 2031 3635 2e37 3520 3136  h d="M 165.75 16
+00000410: 312e 3838 3520 4c20 3136 352e 3835 3120  1.885 L 165.851 
+00000420: 3136 312e 3838 3520 4c20 3136 352e 3835  161.885 L 165.85
+00000430: 3120 3133 392e 3933 3220 4c20 3136 352e  1 139.932 L 165.
+00000440: 3835 3120 3133 342e 3338 3220 4c20 3136  851 134.382 L 16
+00000450: 352e 3834 2031 3334 2e33 3933 204c 2031  5.84 134.393 L 1
+00000460: 3635 2e38 3420 3937 2e32 3937 204c 2031  65.84 97.297 L 1
+00000470: 3536 2e33 3620 3837 2e35 3431 204c 2031  56.36 87.541 L 1
+00000480: 3536 2e33 3620 3230 392e 3620 4320 3135  56.36 209.6 C 15
+00000490: 392e 3134 3420 3231 312e 3637 3220 3136  9.144 211.672 16
+000004a0: 322e 3233 3620 3231 332e 3335 3520 3136  2.236 213.355 16
+000004b0: 352e 3535 3620 3231 342e 3536 3320 4320  5.556 214.563 C 
+000004c0: 3136 352e 3632 3120 3231 342e 3539 3220  165.621 214.592 
+000004d0: 3136 352e 3638 3620 3231 342e 3631 3720  165.686 214.617 
+000004e0: 3136 352e 3735 3120 3231 342e 3634 3520  165.751 214.645 
+000004f0: 4c20 3136 352e 3735 3120 3136 312e 3838  L 165.751 161.88
+00000500: 3520 4c20 3136 352e 3735 2031 3631 2e38  5 L 165.75 161.8
+00000510: 3835 205a 2220 7374 796c 653d 2222 3e3c  85 Z" style=""><
+00000520: 2f70 6174 683e 0a20 2020 203c 7061 7468  /path>.    <path
+00000530: 2064 3d22 4d20 3231 312e 3934 3120 3137   d="M 211.941 17
+00000540: 372e 3331 3720 4320 3230 392e 3531 3720  7.317 C 209.517 
+00000550: 3136 352e 3631 3220 3230 312e 3336 3920  165.612 201.369 
+00000560: 3135 362e 3634 3220 3139 302e 3939 3820  156.642 190.998 
+00000570: 3135 322e 3639 3920 4320 3139 322e 3134  152.699 C 192.14
+00000580: 3620 3135 332e 3337 3720 3139 332e 3234  6 153.377 193.24
+00000590: 3420 3135 342e 3134 3120 3139 342e 3238  4 154.141 194.28
+000005a0: 3420 3135 342e 3938 3220 4320 3139 372e  4 154.982 C 197.
+000005b0: 3935 3220 3135 382e 3236 3920 3230 302e  952 158.269 200.
+000005c0: 3331 3120 3136 332e 3032 3920 3230 302e  311 163.029 200.
+000005d0: 3334 3520 3136 382e 3337 3120 4320 3230  345 168.371 C 20
+000005e0: 302e 3432 3320 3137 382e 3336 3520 3139  0.423 178.365 19
+000005f0: 322e 3335 3520 3138 362e 3533 3320 3138  2.355 186.533 18
+00000600: 322e 3336 3820 3138 362e 3538 3720 4320  2.368 186.587 C 
+00000610: 3137 372e 3734 3820 3138 362e 3633 3120  177.748 186.631 
+00000620: 3137 332e 3836 2031 3834 2e38 3534 2031  173.86 184.854 1
+00000630: 3731 2e30 3037 2031 3831 2e39 3433 204c  71.007 181.943 L
+00000640: 2031 3731 2e30 3037 2032 3136 2e34 3437   171.007 216.447
+00000650: 2043 2031 3735 2e37 3120 3231 372e 3633   C 175.71 217.63
+00000660: 3420 3138 302e 3734 3120 3231 372e 3832  4 180.741 217.82
+00000670: 3220 3138 352e 3830 3920 3231 362e 3739  2 185.809 216.79
+00000680: 3320 4320 3139 362e 3634 3720 3231 342e  3 C 196.647 214.
+00000690: 3538 3420 3230 352e 3136 3920 3230 372e  584 205.169 207.
+000006a0: 3336 3120 3230 392e 3439 2031 3938 2e30  361 209.49 198.0
+000006b0: 3434 2043 2032 3039 2e36 3434 2031 3937  44 C 209.644 197
+000006c0: 2e37 3634 2032 3039 2e37 3938 2031 3937  .764 209.798 197
+000006d0: 2e34 3834 2032 3039 2e39 3435 2031 3937  .484 209.945 197
+000006e0: 2e32 204c 2032 3039 2e38 3634 2031 3937  .2 L 209.864 197
+000006f0: 2e32 2043 2032 3132 2e34 3735 2031 3931  .2 C 212.475 191
+00000700: 2e31 3432 2032 3133 2e33 3420 3138 342e  .142 213.34 184.
+00000710: 3236 2032 3131 2e39 3431 2031 3737 2e33  26 211.941 177.3
+00000720: 3137 2220 7374 796c 653d 2222 3e3c 2f70  17" style=""></p
+00000730: 6174 683e 0a20 203c 2f67 3e0a 3c2f 7376  ath>.  </g>.</sv
+00000740: 673e                                     g>
```

