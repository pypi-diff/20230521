# Comparing `tmp/shinherpro-1.6.2.tar.gz` & `tmp/shinherpro-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.6.2.tar", last modified: Sun May 21 09:03:34 2023, max compression
+gzip compressed data, was "shinherpro-1.6.3.tar", last modified: Sun May 21 09:09:26 2023, max compression
```

## Comparing `shinherpro-1.6.2.tar` & `shinherpro-1.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 09:03:34.833543 shinherpro-1.6.2/
--rw-rw-rw-   0        0        0     4438 2023-05-21 09:03:34.832549 shinherpro-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     4258 2023-05-21 08:20:16.000000 shinherpro-1.6.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 09:03:34.833543 shinherpro-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-05-21 08:59:00.000000 shinherpro-1.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:03:34.818180 shinherpro-1.6.2/shinherpro/
--rw-rw-rw-   0        0        0     9214 2023-05-21 09:03:27.000000 shinherpro-1.6.2/shinherpro/TYAI.py
--rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.6.2/shinherpro/__init__.py
--rw-rw-rw-   0        0        0     1225 2023-05-21 09:03:22.000000 shinherpro-1.6.2/shinherpro/chormeDriver.py
--rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.6.2/shinherpro/vfcModel.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:03:34.831558 shinherpro-1.6.2/shinherpro.egg-info/
--rw-rw-rw-   0        0        0     4438 2023-05-21 09:03:34.000000 shinherpro-1.6.2/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-05-21 09:03:34.000000 shinherpro-1.6.2/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 09:03:34.000000 shinherpro-1.6.2/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-21 09:03:34.000000 shinherpro-1.6.2/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-21 09:03:34.000000 shinherpro-1.6.2/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 09:09:26.555323 shinherpro-1.6.3/
+-rw-rw-rw-   0        0        0     4604 2023-05-21 09:09:26.554827 shinherpro-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4424 2023-05-21 09:08:20.000000 shinherpro-1.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 09:09:26.555323 shinherpro-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-05-21 09:08:55.000000 shinherpro-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 09:09:26.542924 shinherpro-1.6.3/shinherpro/
+-rw-rw-rw-   0        0        0     9212 2023-05-21 09:09:22.000000 shinherpro-1.6.3/shinherpro/TYAI.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.6.3/shinherpro/__init__.py
+-rw-rw-rw-   0        0        0     1225 2023-05-21 09:03:22.000000 shinherpro-1.6.3/shinherpro/chormeDriver.py
+-rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.6.3/shinherpro/vfcModel.py
+drwxrwxrwx   0        0        0        0 2023-05-21 09:09:26.553835 shinherpro-1.6.3/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0     4604 2023-05-21 09:09:26.000000 shinherpro-1.6.3/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-05-21 09:09:26.000000 shinherpro-1.6.3/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 09:09:26.000000 shinherpro-1.6.3/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-21 09:09:26.000000 shinherpro-1.6.3/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-21 09:09:26.000000 shinherpro-1.6.3/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.6.2/PKG-INFO` & `shinherpro-1.6.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,39 @@
-Metadata-Version: 2.1
-Name: shinherpro
-Version: 1.6.2
-Summary: shinher-pro 1.6.2
-Author: Yihuan
-Author-email: ivan17.lai@gmail.com
-Description-Content-Type: text/markdown
-
 # Shinher-Pro V1.6.1
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
 
 [![PyPI Version](https://img.shields.io/pypi/v/shinherpro.svg)](https://pypi.org/project/shinherpro/1.6.1/)
 
 ## use
 ```
-from shinherpro import TYAI
+from shinherpro import TYAI          # 指定學校專用模組
+from shinherpro import vfcModel      # 驗證碼辨識模組
+from shinherpro import chormeDriver  # 模擬遊覽器模組
 ```
 ## setup model
 #### model_setup(file.h5) 用於載入模型,回傳的內容將作為get grade()使用的必要引數.
 ```
-model = TYAI.model_setup(model_path)
+model = vfcModel.setup(model_path)
 ```
-### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(開發中功能)
+### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(尚在開發中)
 ```
-model_path = official_model(5.1)
+model_path = vfcModel.official_model(5.1)
 model = model_setup(model_path)
 ```
 ## setup chrome driver
 ### chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
 ```
-driver = TYAI.chrome_driver_setup(url,view)
+driver = chormeDriver.setup(url,view)
 ```
 ### url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
-### urlGet() 提供了TYAI的成績查詢連結
+### TYAI中的.urlGet() 提供了TYAI的成績查詢連結
 ```
 url = TYAI.urlGet() = "https://sai.tyai.tyc.edu.tw/online/"
-driver = TYAI.chrome_driver_setup(url,True)
+driver = chormeDriver.setup(url,True)
 ```
 ## get grade
 ### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
 TYAI.getGrades(username, password, driver, model,examname,LowConfidence):
 ```
 ### driver、model 為提前初始化所取得的回傳值
```

### Comparing `shinherpro-1.6.2/README.md` & `shinherpro-1.6.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,47 @@
+Metadata-Version: 2.1
+Name: shinherpro
+Version: 1.6.3
+Summary: shinher-pro 1.6.3
+Author: Yihuan
+Author-email: ivan17.lai@gmail.com
+Description-Content-Type: text/markdown
+
 # Shinher-Pro V1.6.1
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
 
 [![PyPI Version](https://img.shields.io/pypi/v/shinherpro.svg)](https://pypi.org/project/shinherpro/1.6.1/)
 
 ## use
 ```
-from shinherpro import TYAI
+from shinherpro import TYAI          # 指定學校專用模組
+from shinherpro import vfcModel      # 驗證碼辨識模組
+from shinherpro import chormeDriver  # 模擬遊覽器模組
 ```
 ## setup model
 #### model_setup(file.h5) 用於載入模型,回傳的內容將作為get grade()使用的必要引數.
 ```
-model = TYAI.model_setup(model_path)
+model = vfcModel.setup(model_path)
 ```
-### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(開發中功能)
+### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(尚在開發中)
 ```
-model_path = official_model(5.1)
+model_path = vfcModel.official_model(5.1)
 model = model_setup(model_path)
 ```
 ## setup chrome driver
 ### chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
 ```
-driver = TYAI.chrome_driver_setup(url,view)
+driver = chormeDriver.setup(url,view)
 ```
 ### url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
-### urlGet() 提供了TYAI的成績查詢連結
+### TYAI中的.urlGet() 提供了TYAI的成績查詢連結
 ```
 url = TYAI.urlGet() = "https://sai.tyai.tyc.edu.tw/online/"
-driver = TYAI.chrome_driver_setup(url,True)
+driver = chormeDriver.setup(url,True)
 ```
 ## get grade
 ### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
 TYAI.getGrades(username, password, driver, model,examname,LowConfidence):
 ```
 ### driver、model 為提前初始化所取得的回傳值
```

### Comparing `shinherpro-1.6.2/setup.py` & `shinherpro-1.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     def run(self):
         print("\033[98m 正在安裝shinher-pro...")
         install.run(self)
         print("shinherpro安裝完成！ \033[0m")
 
 setup(
     name='shinherpro',
-    version='1.6.2',
-    description='shinher-pro 1.6.2',
+    version='1.6.3',
+    description='shinher-pro 1.6.3',
     author='Yihuan',
     author_email='ivan17.lai@gmail.com',
     packages=['shinherpro'],
     install_requires=[
         'selenium',
         'beautifulsoup4',
         'keras',
```

### Comparing `shinherpro-1.6.2/shinherpro/TYAI.py` & `shinherpro-1.6.3/shinherpro/TYAI.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import json
 import os
 from shinherpro import vfcModel
 from shinherpro import chormeDriver
 
 
 ###################################################
-# V 1.5.7 By Yihuan Studio --> 2023/5/20/09:08:49  
+# V 1.6.3 By Yihuan Studio --> 2023/5/21/05:09:19
 
 #############################################
 #  vfcCode AI model 5.1  x4307 picture
 ##  image enhancement algorithm V1 By Sam
 
 def urlGet():
     return "https://sai.tyai.tyc.edu.tw/online/"
```

### Comparing `shinherpro-1.6.2/shinherpro/chormeDriver.py` & `shinherpro-1.6.3/shinherpro/chormeDriver.py`

 * *Files identical despite different names*

### Comparing `shinherpro-1.6.2/shinherpro/vfcModel.py` & `shinherpro-1.6.3/shinherpro/vfcModel.py`

 * *Files identical despite different names*

### Comparing `shinherpro-1.6.2/shinherpro.egg-info/PKG-INFO` & `shinherpro-1.6.3/shinherpro.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 Metadata-Version: 2.1
 Name: shinherpro
-Version: 1.6.2
-Summary: shinher-pro 1.6.2
+Version: 1.6.3
+Summary: shinher-pro 1.6.3
 Author: Yihuan
 Author-email: ivan17.lai@gmail.com
 Description-Content-Type: text/markdown
 
 # Shinher-Pro V1.6.1
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
 
 [![PyPI Version](https://img.shields.io/pypi/v/shinherpro.svg)](https://pypi.org/project/shinherpro/1.6.1/)
 
 ## use
 ```
-from shinherpro import TYAI
+from shinherpro import TYAI          # 指定學校專用模組
+from shinherpro import vfcModel      # 驗證碼辨識模組
+from shinherpro import chormeDriver  # 模擬遊覽器模組
 ```
 ## setup model
 #### model_setup(file.h5) 用於載入模型,回傳的內容將作為get grade()使用的必要引數.
 ```
-model = TYAI.model_setup(model_path)
+model = vfcModel.setup(model_path)
 ```
-### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(開發中功能)
+### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(尚在開發中)
 ```
-model_path = official_model(5.1)
+model_path = vfcModel.official_model(5.1)
 model = model_setup(model_path)
 ```
 ## setup chrome driver
 ### chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
 ```
-driver = TYAI.chrome_driver_setup(url,view)
+driver = chormeDriver.setup(url,view)
 ```
 ### url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
-### urlGet() 提供了TYAI的成績查詢連結
+### TYAI中的.urlGet() 提供了TYAI的成績查詢連結
 ```
 url = TYAI.urlGet() = "https://sai.tyai.tyc.edu.tw/online/"
-driver = TYAI.chrome_driver_setup(url,True)
+driver = chormeDriver.setup(url,True)
 ```
 ## get grade
 ### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
 TYAI.getGrades(username, password, driver, model,examname,LowConfidence):
 ```
 ### driver、model 為提前初始化所取得的回傳值
```

