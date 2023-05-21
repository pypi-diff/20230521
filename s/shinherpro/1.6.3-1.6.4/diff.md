# Comparing `tmp/shinherpro-1.6.3.tar.gz` & `tmp/shinherpro-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.6.3.tar", last modified: Sun May 21 09:09:26 2023, max compression
+gzip compressed data, was "shinherpro-1.6.4.tar", last modified: Sun May 21 15:22:46 2023, max compression
```

## Comparing `shinherpro-1.6.3.tar` & `shinherpro-1.6.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 09:09:26.555323 shinherpro-1.6.3/
--rw-rw-rw-   0        0        0     4604 2023-05-21 09:09:26.554827 shinherpro-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     4424 2023-05-21 09:08:20.000000 shinherpro-1.6.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 09:09:26.555323 shinherpro-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-05-21 09:08:55.000000 shinherpro-1.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:09:26.542924 shinherpro-1.6.3/shinherpro/
--rw-rw-rw-   0        0        0     9212 2023-05-21 09:09:22.000000 shinherpro-1.6.3/shinherpro/TYAI.py
--rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.6.3/shinherpro/__init__.py
--rw-rw-rw-   0        0        0     1225 2023-05-21 09:03:22.000000 shinherpro-1.6.3/shinherpro/chormeDriver.py
--rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.6.3/shinherpro/vfcModel.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:09:26.553835 shinherpro-1.6.3/shinherpro.egg-info/
--rw-rw-rw-   0        0        0     4604 2023-05-21 09:09:26.000000 shinherpro-1.6.3/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-05-21 09:09:26.000000 shinherpro-1.6.3/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 09:09:26.000000 shinherpro-1.6.3/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-21 09:09:26.000000 shinherpro-1.6.3/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-21 09:09:26.000000 shinherpro-1.6.3/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 15:22:46.550748 shinherpro-1.6.4/
+-rw-rw-rw-   0        0        0     4623 2023-05-21 15:22:46.550251 shinherpro-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4443 2023-05-21 09:21:34.000000 shinherpro-1.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 15:22:46.551243 shinherpro-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-05-21 15:22:25.000000 shinherpro-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:22:46.532648 shinherpro-1.6.4/shinherpro/
+-rw-rw-rw-   0        0        0     9358 2023-05-21 15:22:31.000000 shinherpro-1.6.4/shinherpro/TYAI.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.6.4/shinherpro/__init__.py
+-rw-rw-rw-   0        0        0     1225 2023-05-21 09:03:22.000000 shinherpro-1.6.4/shinherpro/chormeDriver.py
+-rw-rw-rw-   0        0        0     2127 2023-05-21 08:58:49.000000 shinherpro-1.6.4/shinherpro/vfcModel.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:22:46.548266 shinherpro-1.6.4/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0     4623 2023-05-21 15:22:46.000000 shinherpro-1.6.4/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-05-21 15:22:46.000000 shinherpro-1.6.4/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 15:22:46.000000 shinherpro-1.6.4/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-21 15:22:46.000000 shinherpro-1.6.4/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-21 15:22:46.000000 shinherpro-1.6.4/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.6.3/PKG-INFO` & `shinherpro-1.6.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: shinherpro
-Version: 1.6.3
-Summary: shinher-pro 1.6.3
+Version: 1.6.4
+Summary: shinher-pro 1.6.4
 Author: Yihuan
 Author-email: ivan17.lai@gmail.com
 Description-Content-Type: text/markdown
 
-# Shinher-Pro V1.6.1
+# Shinher-Pro V1.6.3
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
 
 [![PyPI Version](https://img.shields.io/pypi/v/shinherpro.svg)](https://pypi.org/project/shinherpro/1.6.1/)
 
 ## use
 ```
@@ -19,43 +19,43 @@
 from shinherpro import chormeDriver  # 模擬遊覽器模組
 ```
 ## setup model
 #### model_setup(file.h5) 用於載入模型,回傳的內容將作為get grade()使用的必要引數.
 ```
 model = vfcModel.setup(model_path)
 ```
-### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(尚在開發中)
+#### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(尚在開發中)
 ```
 model_path = vfcModel.official_model(5.1)
 model = model_setup(model_path)
 ```
 ## setup chrome driver
-### chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
+#### chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
 ```
 driver = chormeDriver.setup(url,view)
 ```
-### url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
-### TYAI中的.urlGet() 提供了TYAI的成績查詢連結
+#### url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
+#### TYAI中的.urlGet() 提供了TYAI的成績查詢連結
 ```
 url = TYAI.urlGet() = "https://sai.tyai.tyc.edu.tw/online/"
 driver = chormeDriver.setup(url,True)
 ```
 ## get grade
-### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
+#### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
 TYAI.getGrades(username, password, driver, model,examname,LowConfidence):
 ```
-### driver、model 為提前初始化所取得的回傳值
-### username, password 為帳號密碼
-### exam 為考試列表需準確無誤
-### LowConfidence 非必填，預設為85，為驗證碼AI的準確度要求，若AI判斷本次驗證碼準確率低於指定值，則會重新整理網頁獲取新的驗證碼。
-### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
-### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
+#### driver、model 為提前初始化所取得的回傳值
+#### username, password 為帳號密碼
+#### exam 為考試列表需準確無誤
+#### LowConfidence 非必填，預設為85，為驗證碼AI的準確度要求，若AI判斷本次驗證碼準確率低於指定值，則會重新整理網頁獲取新的驗證碼。
+#### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
+#### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
 
-### 如果登入成功，成績查詢成功，則返回以下格式的json：
+#### 如果登入成功，成績查詢成功，則返回以下格式的json：
 ```
 {
     "code": 0,
     "考試標題": "考試標題",
     "學號": "學號",
     "姓名": "姓名",
     "班級": "班級",
@@ -74,33 +74,33 @@
     ],
     "總分": "總分",
     "平均分數": "平均分數",
     "排名": "排名",
     "科別排名": "科別排名"
 }
 ```
-### 其中，code 表示返回的狀態碼，0 表示成功。其他鍵值對表示成績資訊，包括考試標題、學號、姓名、班級、考試科目成績、總分、平均分數、排名和科別排名。考試科目成績 是一個列表，每個元素表示一個考試科目的成績，包括考試科目名稱和對應的成績。
-### 如果登入失敗，則返回以下格式的字典：
+#### 其中，code 表示返回的狀態碼，0 表示成功。其他鍵值對表示成績資訊，包括考試標題、學號、姓名、班級、考試科目成績、總分、平均分數、排名和科別排名。考試科目成績 是一個列表，每個元素表示一個考試科目的成績，包括考試科目名稱和對應的成績。
+#### 如果登入失敗，則返回以下格式的字典：
 ```
 {
     "code": 1,
     "reason": "帳號或密碼錯誤,請重新登入!"
 }
 ```
-### 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
-### 如果登入失敗次數過多，則返回以下格式的字典：
+#### 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
+#### 如果登入失敗次數過多，則返回以下格式的字典：
 ```
 {
     "code": 2,
     "reason": "帳號登入失敗次數過多，請於15分鐘後再嘗試登入!!"
 }
 ```
-### 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
-### 如果其他未知錯誤發生，則返回以下格式的字典：
+#### 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
+#### 如果其他未知錯誤發生，則返回以下格式的字典：
 ```
 {
     "code": 3,
     "reason": "錯誤原因"
 }
 ```
-### 其中，code 表示返回的狀態碼，3 表示未知錯誤。reason 表示錯誤原因的描述。
+#### 其中，code 表示返回的狀態碼，3 表示未知錯誤。reason 表示錯誤原因的描述。
```

### Comparing `shinherpro-1.6.3/README.md` & `shinherpro-1.6.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Shinher-Pro V1.6.1
+# Shinher-Pro V1.6.3
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
 
 [![PyPI Version](https://img.shields.io/pypi/v/shinherpro.svg)](https://pypi.org/project/shinherpro/1.6.1/)
 
 ## use
 ```
@@ -11,43 +11,43 @@
 from shinherpro import chormeDriver  # 模擬遊覽器模組
 ```
 ## setup model
 #### model_setup(file.h5) 用於載入模型,回傳的內容將作為get grade()使用的必要引數.
 ```
 model = vfcModel.setup(model_path)
 ```
-### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(尚在開發中)
+#### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(尚在開發中)
 ```
 model_path = vfcModel.official_model(5.1)
 model = model_setup(model_path)
 ```
 ## setup chrome driver
-### chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
+#### chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
 ```
 driver = chormeDriver.setup(url,view)
 ```
-### url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
-### TYAI中的.urlGet() 提供了TYAI的成績查詢連結
+#### url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
+#### TYAI中的.urlGet() 提供了TYAI的成績查詢連結
 ```
 url = TYAI.urlGet() = "https://sai.tyai.tyc.edu.tw/online/"
 driver = chormeDriver.setup(url,True)
 ```
 ## get grade
-### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
+#### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
 TYAI.getGrades(username, password, driver, model,examname,LowConfidence):
 ```
-### driver、model 為提前初始化所取得的回傳值
-### username, password 為帳號密碼
-### exam 為考試列表需準確無誤
-### LowConfidence 非必填，預設為85，為驗證碼AI的準確度要求，若AI判斷本次驗證碼準確率低於指定值，則會重新整理網頁獲取新的驗證碼。
-### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
-### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
+#### driver、model 為提前初始化所取得的回傳值
+#### username, password 為帳號密碼
+#### exam 為考試列表需準確無誤
+#### LowConfidence 非必填，預設為85，為驗證碼AI的準確度要求，若AI判斷本次驗證碼準確率低於指定值，則會重新整理網頁獲取新的驗證碼。
+#### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
+#### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
 
-### 如果登入成功，成績查詢成功，則返回以下格式的json：
+#### 如果登入成功，成績查詢成功，則返回以下格式的json：
 ```
 {
     "code": 0,
     "考試標題": "考試標題",
     "學號": "學號",
     "姓名": "姓名",
     "班級": "班級",
@@ -66,33 +66,33 @@
     ],
     "總分": "總分",
     "平均分數": "平均分數",
     "排名": "排名",
     "科別排名": "科別排名"
 }
 ```
-### 其中，code 表示返回的狀態碼，0 表示成功。其他鍵值對表示成績資訊，包括考試標題、學號、姓名、班級、考試科目成績、總分、平均分數、排名和科別排名。考試科目成績 是一個列表，每個元素表示一個考試科目的成績，包括考試科目名稱和對應的成績。
-### 如果登入失敗，則返回以下格式的字典：
+#### 其中，code 表示返回的狀態碼，0 表示成功。其他鍵值對表示成績資訊，包括考試標題、學號、姓名、班級、考試科目成績、總分、平均分數、排名和科別排名。考試科目成績 是一個列表，每個元素表示一個考試科目的成績，包括考試科目名稱和對應的成績。
+#### 如果登入失敗，則返回以下格式的字典：
 ```
 {
     "code": 1,
     "reason": "帳號或密碼錯誤,請重新登入!"
 }
 ```
-### 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
-### 如果登入失敗次數過多，則返回以下格式的字典：
+#### 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
+#### 如果登入失敗次數過多，則返回以下格式的字典：
 ```
 {
     "code": 2,
     "reason": "帳號登入失敗次數過多，請於15分鐘後再嘗試登入!!"
 }
 ```
-### 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
-### 如果其他未知錯誤發生，則返回以下格式的字典：
+#### 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
+#### 如果其他未知錯誤發生，則返回以下格式的字典：
 ```
 {
     "code": 3,
     "reason": "錯誤原因"
 }
 ```
-### 其中，code 表示返回的狀態碼，3 表示未知錯誤。reason 表示錯誤原因的描述。
+#### 其中，code 表示返回的狀態碼，3 表示未知錯誤。reason 表示錯誤原因的描述。
```

### Comparing `shinherpro-1.6.3/setup.py` & `shinherpro-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     def run(self):
         print("\033[98m 正在安裝shinher-pro...")
         install.run(self)
         print("shinherpro安裝完成！ \033[0m")
 
 setup(
     name='shinherpro',
-    version='1.6.3',
-    description='shinher-pro 1.6.3',
+    version='1.6.4',
+    description='shinher-pro 1.6.4',
     author='Yihuan',
     author_email='ivan17.lai@gmail.com',
     packages=['shinherpro'],
     install_requires=[
         'selenium',
         'beautifulsoup4',
         'keras',
```

### Comparing `shinherpro-1.6.3/shinherpro/TYAI.py` & `shinherpro-1.6.4/shinherpro/TYAI.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import json
 import os
 from shinherpro import vfcModel
 from shinherpro import chormeDriver
 
 
 ###################################################
-# V 1.6.3 By Yihuan Studio --> 2023/5/21/05:09:19
+# V 1.6.4 By Yihuan Studio --> 2023/5/21/05:09:19
 
 #############################################
 #  vfcCode AI model 5.1  x4307 picture
 ##  image enhancement algorithm V1 By Sam
 
 def urlGet():
     return "https://sai.tyai.tyc.edu.tw/online/"
@@ -83,15 +83,20 @@
 
     loginScess = False
 
     while True:
         allConfidence = 0
         while allConfidence <= LowConfidence :
             vfc = ""
-            captcha_element = driver.find_element(By.XPATH, '//img[@id="imgvcode"]')
+            while(True):
+                try:
+                    captcha_element = driver.find_element(By.XPATH, '//img[@id="imgvcode"]')
+                    break
+                except:
+                    driver.refresh()
 
             src = captcha_element.get_attribute('src')
             print('Image source:', src)
 
             screenshot_path = 'captcha.png'
             driver.save_screenshot(screenshot_path)
             location = captcha_element.location
```

### Comparing `shinherpro-1.6.3/shinherpro/chormeDriver.py` & `shinherpro-1.6.4/shinherpro/chormeDriver.py`

 * *Files identical despite different names*

### Comparing `shinherpro-1.6.3/shinherpro/vfcModel.py` & `shinherpro-1.6.4/shinherpro/vfcModel.py`

 * *Files identical despite different names*

### Comparing `shinherpro-1.6.3/shinherpro.egg-info/PKG-INFO` & `shinherpro-1.6.4/shinherpro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: shinherpro
-Version: 1.6.3
-Summary: shinher-pro 1.6.3
+Version: 1.6.4
+Summary: shinher-pro 1.6.4
 Author: Yihuan
 Author-email: ivan17.lai@gmail.com
 Description-Content-Type: text/markdown
 
-# Shinher-Pro V1.6.1
+# Shinher-Pro V1.6.3
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
 
 [![PyPI Version](https://img.shields.io/pypi/v/shinherpro.svg)](https://pypi.org/project/shinherpro/1.6.1/)
 
 ## use
 ```
@@ -19,43 +19,43 @@
 from shinherpro import chormeDriver  # 模擬遊覽器模組
 ```
 ## setup model
 #### model_setup(file.h5) 用於載入模型,回傳的內容將作為get grade()使用的必要引數.
 ```
 model = vfcModel.setup(model_path)
 ```
-### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(尚在開發中)
+#### official_model(Version) 提供了官方的驗證碼辨識模型,目前僅支持5.1版本(尚在開發中)
 ```
 model_path = vfcModel.official_model(5.1)
 model = model_setup(model_path)
 ```
 ## setup chrome driver
-### chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
+#### chrome_driver_setup(url,view) 用於打開chrome driver 並開啟指定網址,,回傳的內容將作為get grade()使用的必要引數.
 ```
 driver = chormeDriver.setup(url,view)
 ```
-### url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
-### TYAI中的.urlGet() 提供了TYAI的成績查詢連結
+#### url為指定的網址,view可指定模擬遊覽器執行時是否要顯示實體頁面.
+#### TYAI中的.urlGet() 提供了TYAI的成績查詢連結
 ```
 url = TYAI.urlGet() = "https://sai.tyai.tyc.edu.tw/online/"
 driver = chormeDriver.setup(url,True)
 ```
 ## get grade
-### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
+#### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
 TYAI.getGrades(username, password, driver, model,examname,LowConfidence):
 ```
-### driver、model 為提前初始化所取得的回傳值
-### username, password 為帳號密碼
-### exam 為考試列表需準確無誤
-### LowConfidence 非必填，預設為85，為驗證碼AI的準確度要求，若AI判斷本次驗證碼準確率低於指定值，則會重新整理網頁獲取新的驗證碼。
-### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
-### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
+#### driver、model 為提前初始化所取得的回傳值
+#### username, password 為帳號密碼
+#### exam 為考試列表需準確無誤
+#### LowConfidence 非必填，預設為85，為驗證碼AI的準確度要求，若AI判斷本次驗證碼準確率低於指定值，則會重新整理網頁獲取新的驗證碼。
+#### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
+#### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
 
-### 如果登入成功，成績查詢成功，則返回以下格式的json：
+#### 如果登入成功，成績查詢成功，則返回以下格式的json：
 ```
 {
     "code": 0,
     "考試標題": "考試標題",
     "學號": "學號",
     "姓名": "姓名",
     "班級": "班級",
@@ -74,33 +74,33 @@
     ],
     "總分": "總分",
     "平均分數": "平均分數",
     "排名": "排名",
     "科別排名": "科別排名"
 }
 ```
-### 其中，code 表示返回的狀態碼，0 表示成功。其他鍵值對表示成績資訊，包括考試標題、學號、姓名、班級、考試科目成績、總分、平均分數、排名和科別排名。考試科目成績 是一個列表，每個元素表示一個考試科目的成績，包括考試科目名稱和對應的成績。
-### 如果登入失敗，則返回以下格式的字典：
+#### 其中，code 表示返回的狀態碼，0 表示成功。其他鍵值對表示成績資訊，包括考試標題、學號、姓名、班級、考試科目成績、總分、平均分數、排名和科別排名。考試科目成績 是一個列表，每個元素表示一個考試科目的成績，包括考試科目名稱和對應的成績。
+#### 如果登入失敗，則返回以下格式的字典：
 ```
 {
     "code": 1,
     "reason": "帳號或密碼錯誤,請重新登入!"
 }
 ```
-### 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
-### 如果登入失敗次數過多，則返回以下格式的字典：
+#### 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
+#### 如果登入失敗次數過多，則返回以下格式的字典：
 ```
 {
     "code": 2,
     "reason": "帳號登入失敗次數過多，請於15分鐘後再嘗試登入!!"
 }
 ```
-### 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
-### 如果其他未知錯誤發生，則返回以下格式的字典：
+#### 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
+#### 如果其他未知錯誤發生，則返回以下格式的字典：
 ```
 {
     "code": 3,
     "reason": "錯誤原因"
 }
 ```
-### 其中，code 表示返回的狀態碼，3 表示未知錯誤。reason 表示錯誤原因的描述。
+#### 其中，code 表示返回的狀態碼，3 表示未知錯誤。reason 表示錯誤原因的描述。
```

