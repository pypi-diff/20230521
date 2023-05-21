# Comparing `tmp/shinherpro-1.5.8.tar.gz` & `tmp/shinherpro-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.5.8.tar", last modified: Sat May 20 13:12:13 2023, max compression
+gzip compressed data, was "shinherpro-1.5.9.tar", last modified: Sun May 21 04:37:47 2023, max compression
```

## Comparing `shinherpro-1.5.8.tar` & `shinherpro-1.5.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 13:12:13.177266 shinherpro-1.5.8/
--rw-rw-rw-   0        0        0     3841 2023-05-20 13:12:13.176769 shinherpro-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     3661 2023-05-20 13:10:07.000000 shinherpro-1.5.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 13:12:13.177266 shinherpro-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-05-20 13:12:07.000000 shinherpro-1.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 13:12:13.164371 shinherpro-1.5.8/shinherpro/
--rw-rw-rw-   0        0        0    10823 2023-05-20 13:08:34.000000 shinherpro-1.5.8/shinherpro/TYAI.py
--rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.5.8/shinherpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 13:12:13.175778 shinherpro-1.5.8/shinherpro.egg-info/
--rw-rw-rw-   0        0        0     3841 2023-05-20 13:12:13.000000 shinherpro-1.5.8/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-20 13:12:13.000000 shinherpro-1.5.8/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 13:12:13.000000 shinherpro-1.5.8/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-20 13:12:13.000000 shinherpro-1.5.8/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-20 13:12:13.000000 shinherpro-1.5.8/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 04:37:47.124395 shinherpro-1.5.9/
+-rw-rw-rw-   0        0        0     3853 2023-05-21 04:37:47.123899 shinherpro-1.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3673 2023-05-20 13:15:34.000000 shinherpro-1.5.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 04:37:47.125389 shinherpro-1.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-05-21 04:37:40.000000 shinherpro-1.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 04:37:47.112491 shinherpro-1.5.9/shinherpro/
+-rw-rw-rw-   0        0        0    10986 2023-05-21 04:36:45.000000 shinherpro-1.5.9/shinherpro/TYAI.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.5.9/shinherpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 04:37:47.122411 shinherpro-1.5.9/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0     3853 2023-05-21 04:37:46.000000 shinherpro-1.5.9/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-21 04:37:47.000000 shinherpro-1.5.9/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 04:37:46.000000 shinherpro-1.5.9/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-21 04:37:46.000000 shinherpro-1.5.9/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-21 04:37:46.000000 shinherpro-1.5.9/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.5.8/PKG-INFO` & `shinherpro-1.5.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: shinherpro
-Version: 1.5.8
-Summary: shinher-pro 1.5.8
+Version: 1.5.9
+Summary: shinher-pro 1.5.9
 Author: Yihuan
 Author-email: ivan17.lai@gmail.com
 Description-Content-Type: text/markdown
 
 # Shinher-Pro V1.5.7
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
@@ -37,15 +37,14 @@
 ```
 ## get grade
 ### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
 TYAI.getGrades(username, password, driver, model,examname):
 ```
 ### driver、model 為提前初始化所取得的回傳值
-
 ### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
 ### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
 
 ### 如果登入成功，成績查詢成功，則返回以下格式的json：
 ```
 {
     "code": 0,
@@ -66,27 +65,27 @@
     ],
     "總分": "總分",
     "平均分數": "平均分數",
     "排名": "排名",
     "科別排名": "科別排名"
 }
 ```
-# 其中，code 表示返回的狀態碼，0 表示成功。其他鍵值對表示成績資訊，包括考試標題、學號、姓名、班級、考試科目成績、總分、平均分數、排名和科別排名。考試科目成績 是一個列表，每個元素表示一個考試科目的成績，包括考試科目名稱和對應的成績。
-# 如果登入失敗，則返回以下格式的字典：
+### 其中，code 表示返回的狀態碼，0 表示成功。其他鍵值對表示成績資訊，包括考試標題、學號、姓名、班級、考試科目成績、總分、平均分數、排名和科別排名。考試科目成績 是一個列表，每個元素表示一個考試科目的成績，包括考試科目名稱和對應的成績。
+### 如果登入失敗，則返回以下格式的字典：
 ```
 {
     "code": 1,
     "reason": "帳號或密碼錯誤,請重新登入!"
 }
 ```
-# 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
-# 如果登入失敗次數過多，則返回以下格式的字典：
-# 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
-# 如果其他未知錯誤發生，則返回以下格式的字典：
+### 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
+### 如果登入失敗次數過多，則返回以下格式的字典：
+### 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
+### 如果其他未知錯誤發生，則返回以下格式的字典：
 ```
 {
     "code": 3,
     "reason": "錯誤原因"
 }
 ```
-# 其中，code 表示返回的狀態碼，3 表示未知錯誤。reason 表示錯誤原因的描述。
+### 其中，code 表示返回的狀態碼，3 表示未知錯誤。reason 表示錯誤原因的描述。
```

### Comparing `shinherpro-1.5.8/README.md` & `shinherpro-1.5.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 ```
 ## get grade
 ### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
 TYAI.getGrades(username, password, driver, model,examname):
 ```
 ### driver、model 為提前初始化所取得的回傳值
-
 ### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
 ### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
 
 ### 如果登入成功，成績查詢成功，則返回以下格式的json：
 ```
 {
     "code": 0,
@@ -58,27 +57,27 @@
     ],
     "總分": "總分",
     "平均分數": "平均分數",
     "排名": "排名",
     "科別排名": "科別排名"
 }
 ```
-# 其中，code 表示返回的狀態碼，0 表示成功。其他鍵值對表示成績資訊，包括考試標題、學號、姓名、班級、考試科目成績、總分、平均分數、排名和科別排名。考試科目成績 是一個列表，每個元素表示一個考試科目的成績，包括考試科目名稱和對應的成績。
-# 如果登入失敗，則返回以下格式的字典：
+### 其中，code 表示返回的狀態碼，0 表示成功。其他鍵值對表示成績資訊，包括考試標題、學號、姓名、班級、考試科目成績、總分、平均分數、排名和科別排名。考試科目成績 是一個列表，每個元素表示一個考試科目的成績，包括考試科目名稱和對應的成績。
+### 如果登入失敗，則返回以下格式的字典：
 ```
 {
     "code": 1,
     "reason": "帳號或密碼錯誤,請重新登入!"
 }
 ```
-# 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
-# 如果登入失敗次數過多，則返回以下格式的字典：
-# 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
-# 如果其他未知錯誤發生，則返回以下格式的字典：
+### 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
+### 如果登入失敗次數過多，則返回以下格式的字典：
+### 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
+### 如果其他未知錯誤發生，則返回以下格式的字典：
 ```
 {
     "code": 3,
     "reason": "錯誤原因"
 }
 ```
-# 其中，code 表示返回的狀態碼，3 表示未知錯誤。reason 表示錯誤原因的描述。
+### 其中，code 表示返回的狀態碼，3 表示未知錯誤。reason 表示錯誤原因的描述。
```

### Comparing `shinherpro-1.5.8/setup.py` & `shinherpro-1.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     def run(self):
         print("\033[93m 正在安裝shinher-pro...")
         install.run(self)
         print("shinherpro安裝完成！ \033[0m")
 
 setup(
     name='shinherpro',
-    version='1.5.8',
-    description='shinher-pro 1.5.8',
+    version='1.5.9',
+    description='shinher-pro 1.5.9',
     author='Yihuan',
     author_email='ivan17.lai@gmail.com',
     packages=['shinherpro'],
     install_requires=[
         'selenium',
         'beautifulsoup4',
         'keras',
```

### Comparing `shinherpro-1.5.8/shinherpro/TYAI.py` & `shinherpro-1.5.9/shinherpro/TYAI.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,14 +200,16 @@
             popup_text = alert.text
             print(popup_text)
             alert.dismiss()
             if popup_text == "帳號或密碼錯誤,請重新登入!":
                 return {'code':1,'reason':"帳號或密碼錯誤,請重新登入!"}
             elif popup_text == "帳號登入失敗次數過多，請於15分鐘後再嘗試登入!!":
                 return {'code':2,'reason':"帳號登入失敗次數過多，請於15分鐘後再嘗試登入!!"}
+            elif popup_text == "驗證碼輸入錯誤，請重新輸入。":
+                print("驗證碼輸入錯誤,重新嘗試")
             else:
                 reason = popup_text
                 return {'code':3,'reason':reason}
             
  
         except:
             print(f"{GREEN}密碼正確.{RESET}",end="")
@@ -261,15 +263,15 @@
 
     driver.delete_all_cookies()
     driver.refresh()
     return result
 
 
 # for test
-if False:
+if True:
     model1 = model_setup("E:\\project\\vfc_AiModel_5.1_VGG16_black.h5")
 
-    driver1 = chrome_driver_setup(False)
+    driver1 = chrome_driver_setup(urlGet(),False)
 
-    print(getGrades(username="",password="",driver=driver1,model=model1,examname='[111下] 111下第1次段考'))
+    print(getGrades(username="013333",password="B123742969",driver=driver1,model=model1,examname='[111下] 111下第1次段考'))
     #print(getGrades(username="",password="",driver=driver1,model=model1,examname='[111下] 111下第2次段考'))
```

### Comparing `shinherpro-1.5.8/shinherpro.egg-info/PKG-INFO` & `shinherpro-1.5.9/shinherpro.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: shinherpro
-Version: 1.5.8
-Summary: shinher-pro 1.5.8
+Version: 1.5.9
+Summary: shinher-pro 1.5.9
 Author: Yihuan
 Author-email: ivan17.lai@gmail.com
 Description-Content-Type: text/markdown
 
 # Shinher-Pro V1.5.7
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
@@ -37,15 +37,14 @@
 ```
 ## get grade
 ### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
 TYAI.getGrades(username, password, driver, model,examname):
 ```
 ### driver、model 為提前初始化所取得的回傳值
-
 ### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
 ### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
 
 ### 如果登入成功，成績查詢成功，則返回以下格式的json：
 ```
 {
     "code": 0,
@@ -66,27 +65,27 @@
     ],
     "總分": "總分",
     "平均分數": "平均分數",
     "排名": "排名",
     "科別排名": "科別排名"
 }
 ```
-# 其中，code 表示返回的狀態碼，0 表示成功。其他鍵值對表示成績資訊，包括考試標題、學號、姓名、班級、考試科目成績、總分、平均分數、排名和科別排名。考試科目成績 是一個列表，每個元素表示一個考試科目的成績，包括考試科目名稱和對應的成績。
-# 如果登入失敗，則返回以下格式的字典：
+### 其中，code 表示返回的狀態碼，0 表示成功。其他鍵值對表示成績資訊，包括考試標題、學號、姓名、班級、考試科目成績、總分、平均分數、排名和科別排名。考試科目成績 是一個列表，每個元素表示一個考試科目的成績，包括考試科目名稱和對應的成績。
+### 如果登入失敗，則返回以下格式的字典：
 ```
 {
     "code": 1,
     "reason": "帳號或密碼錯誤,請重新登入!"
 }
 ```
-# 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
-# 如果登入失敗次數過多，則返回以下格式的字典：
-# 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
-# 如果其他未知錯誤發生，則返回以下格式的字典：
+### 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
+### 如果登入失敗次數過多，則返回以下格式的字典：
+### 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
+### 如果其他未知錯誤發生，則返回以下格式的字典：
 ```
 {
     "code": 3,
     "reason": "錯誤原因"
 }
 ```
-# 其中，code 表示返回的狀態碼，3 表示未知錯誤。reason 表示錯誤原因的描述。
+### 其中，code 表示返回的狀態碼，3 表示未知錯誤。reason 表示錯誤原因的描述。
```

