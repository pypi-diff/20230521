# Comparing `tmp/shinherpro-1.6.0.tar.gz` & `tmp/shinherpro-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.6.0.tar", last modified: Sun May 21 05:53:11 2023, max compression
+gzip compressed data, was "shinherpro-1.6.1.tar", last modified: Sun May 21 07:54:15 2023, max compression
```

## Comparing `shinherpro-1.6.0.tar` & `shinherpro-1.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 05:53:11.314465 shinherpro-1.6.0/
--rw-rw-rw-   0        0        0     3853 2023-05-21 05:53:11.313471 shinherpro-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     3673 2023-05-20 13:15:34.000000 shinherpro-1.6.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 05:53:11.314465 shinherpro-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-05-21 05:53:05.000000 shinherpro-1.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 05:53:11.301071 shinherpro-1.6.0/shinherpro/
--rw-rw-rw-   0        0        0    10582 2023-05-21 05:52:45.000000 shinherpro-1.6.0/shinherpro/TYAI.py
--rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.6.0/shinherpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 05:53:11.311984 shinherpro-1.6.0/shinherpro.egg-info/
--rw-rw-rw-   0        0        0     3853 2023-05-21 05:53:11.000000 shinherpro-1.6.0/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-21 05:53:11.000000 shinherpro-1.6.0/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 05:53:11.000000 shinherpro-1.6.0/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-21 05:53:11.000000 shinherpro-1.6.0/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-21 05:53:11.000000 shinherpro-1.6.0/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 07:54:15.325432 shinherpro-1.6.1/
+-rw-rw-rw-   0        0        0     4317 2023-05-21 07:54:15.324438 shinherpro-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4137 2023-05-21 07:54:09.000000 shinherpro-1.6.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 07:54:15.325432 shinherpro-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-05-21 07:25:51.000000 shinherpro-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 07:54:15.309063 shinherpro-1.6.1/shinherpro/
+-rw-rw-rw-   0        0        0    11190 2023-05-21 07:48:31.000000 shinherpro-1.6.1/shinherpro/TYAI.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.6.1/shinherpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 07:54:15.323447 shinherpro-1.6.1/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0     4317 2023-05-21 07:54:15.000000 shinherpro-1.6.1/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-21 07:54:15.000000 shinherpro-1.6.1/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 07:54:15.000000 shinherpro-1.6.1/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-21 07:54:15.000000 shinherpro-1.6.1/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-21 07:54:15.000000 shinherpro-1.6.1/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.6.0/PKG-INFO` & `shinherpro-1.6.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,8 @@
-Metadata-Version: 2.1
-Name: shinherpro
-Version: 1.6.0
-Summary: shinher-pro 1.6.0
-Author: Yihuan
-Author-email: ivan17.lai@gmail.com
-Description-Content-Type: text/markdown
-
-# Shinher-Pro V1.5.7
+# Shinher-Pro V1.6.1
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
 
 ## use
 ```
 from shinherpro import TYAI
 ```
@@ -34,36 +26,41 @@
 ```
 url = TYAI.urlGet() = "https://sai.tyai.tyc.edu.tw/online/"
 driver = TYAI.chrome_driver_setup(url,True)
 ```
 ## get grade
 ### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
-TYAI.getGrades(username, password, driver, model,examname):
+TYAI.getGrades(username, password, driver, model,examname,LowConfidence):
 ```
 ### driver、model 為提前初始化所取得的回傳值
+### username, password 為帳號密碼
+### exam 為考試列表需準確無誤
+### LowConfidence 非必填，預設為85，為驗證碼AI的準確度要求，若AI判斷本次驗證碼準確率低於指定值，則會重新整理網頁獲取新的驗證碼。
 ### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
 ### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
 
 ### 如果登入成功，成績查詢成功，則返回以下格式的json：
 ```
 {
     "code": 0,
     "考試標題": "考試標題",
     "學號": "學號",
     "姓名": "姓名",
     "班級": "班級",
     "考試科目成績": [
         {
             "考試科目": "科目1",
-            "考試成績": "成績1"
+            "考試成績": "成績1",
+            "全班平均": "平均1"
         },
         {
             "考試科目": "科目2",
-            "考試成績": "成績2"
+            "考試成績": "成績2",
+            "全班平均": "平均2"
         },
         ...
     ],
     "總分": "總分",
     "平均分數": "平均分數",
     "排名": "排名",
     "科別排名": "科別排名"
@@ -75,14 +72,18 @@
 {
     "code": 1,
     "reason": "帳號或密碼錯誤,請重新登入!"
 }
 ```
 ### 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
 ### 如果登入失敗次數過多，則返回以下格式的字典：
+{
+    "code": 2,
+    "reason": "帳號登入失敗次數過多，請於15分鐘後再嘗試登入!!"
+}
 ### 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
 ### 如果其他未知錯誤發生，則返回以下格式的字典：
 ```
 {
     "code": 3,
     "reason": "錯誤原因"
 }
```

### Comparing `shinherpro-1.6.0/README.md` & `shinherpro-1.6.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,16 @@
-# Shinher-Pro V1.5.7
+Metadata-Version: 2.1
+Name: shinherpro
+Version: 1.6.1
+Summary: shinher-pro 1.6.1
+Author: Yihuan
+Author-email: ivan17.lai@gmail.com
+Description-Content-Type: text/markdown
+
+# Shinher-Pro V1.6.1
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
 
 ## use
 ```
 from shinherpro import TYAI
 ```
@@ -26,36 +34,41 @@
 ```
 url = TYAI.urlGet() = "https://sai.tyai.tyc.edu.tw/online/"
 driver = TYAI.chrome_driver_setup(url,True)
 ```
 ## get grade
 ### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
-TYAI.getGrades(username, password, driver, model,examname):
+TYAI.getGrades(username, password, driver, model,examname,LowConfidence):
 ```
 ### driver、model 為提前初始化所取得的回傳值
+### username, password 為帳號密碼
+### exam 為考試列表需準確無誤
+### LowConfidence 非必填，預設為85，為驗證碼AI的準確度要求，若AI判斷本次驗證碼準確率低於指定值，則會重新整理網頁獲取新的驗證碼。
 ### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
 ### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
 
 ### 如果登入成功，成績查詢成功，則返回以下格式的json：
 ```
 {
     "code": 0,
     "考試標題": "考試標題",
     "學號": "學號",
     "姓名": "姓名",
     "班級": "班級",
     "考試科目成績": [
         {
             "考試科目": "科目1",
-            "考試成績": "成績1"
+            "考試成績": "成績1",
+            "全班平均": "平均1"
         },
         {
             "考試科目": "科目2",
-            "考試成績": "成績2"
+            "考試成績": "成績2",
+            "全班平均": "平均2"
         },
         ...
     ],
     "總分": "總分",
     "平均分數": "平均分數",
     "排名": "排名",
     "科別排名": "科別排名"
@@ -67,14 +80,18 @@
 {
     "code": 1,
     "reason": "帳號或密碼錯誤,請重新登入!"
 }
 ```
 ### 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
 ### 如果登入失敗次數過多，則返回以下格式的字典：
+{
+    "code": 2,
+    "reason": "帳號登入失敗次數過多，請於15分鐘後再嘗試登入!!"
+}
 ### 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
 ### 如果其他未知錯誤發生，則返回以下格式的字典：
 ```
 {
     "code": 3,
     "reason": "錯誤原因"
 }
```

### Comparing `shinherpro-1.6.0/setup.py` & `shinherpro-1.6.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from setuptools.command.install import install
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 class CustomInstallCommand(install):
     def run(self):
-        print("\033[93m 正在安裝shinher-pro...")
+        print("\033[98m 正在安裝shinher-pro...")
         install.run(self)
         print("shinherpro安裝完成！ \033[0m")
 
 setup(
     name='shinherpro',
-    version='1.6.0',
-    description='shinher-pro 1.6.0',
+    version='1.6.1',
+    description='shinher-pro 1.6.1',
     author='Yihuan',
     author_email='ivan17.lai@gmail.com',
     packages=['shinherpro'],
     install_requires=[
         'selenium',
         'beautifulsoup4',
         'keras',
```

### Comparing `shinherpro-1.6.0/shinherpro/TYAI.py` & `shinherpro-1.6.1/shinherpro/TYAI.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import requests
 import numpy as np
 import cv2
 import time
 import json
 import os
 
+
 ###################################################
 # V 1.5.7 By Yihuan Studio --> 2023/5/20/09:08:49  
 
 #############################################
 #  vfcCode AI model 5.1  x4307 picture
 ##  image enhancement algorithm V1 By Sam
 
@@ -35,16 +36,19 @@
 def official_model(Version):
     current_folder = os.path.dirname(os.path.abspath(__file__))
     print(current_folder)
     current_folder = os.path.dirname(os.path.abspath(__file__))
     model_path = os.path.join(current_folder, 'vfc_AiModel_5.1_VGG16_black.h5')
     print("vfc_AiModel_5.1_VGG16_black.h5 的完整路徑：", model_path)
     return model_path
+
 def urlGet():
+
     return "https://sai.tyai.tyc.edu.tw/online/"
+
 def chrome_driver_setup(url,view):
     print("chrome_options setup")
     chrome_options = Options()
     chrome_options.add_argument("--window-size=1280,960")
     if view==False :
         chrome_options.add_argument('--headless')
     driver = webdriver.Chrome(options=chrome_options)
@@ -82,111 +86,120 @@
 
     predictions = model.predict(image)
     predicted_label = np.argmax(predictions, axis=1)[0]
     confidence = predictions[0][predicted_label]
 
     return predicted_label, confidence
 
-
 def score_tolist(new_page_source):
+    
     html = new_page_source
     soup = BeautifulSoup(html, 'html.parser')
 
     # 提取考試科目成績
     subject_scores = []
     rows = soup.select('table.t02 tr.row')
     for row in rows:
         subject = row.select_one('td.top').text.strip()
-        score = row.select_one('td.top.right span').text.strip()
-        subject_scores.append({'考試科目': subject, '考試成績': score})
+        score_elements = row.select('td.top.right span')
+        if len(score_elements) >= 2:
+            user_score = score_elements[0].text.strip()
+            class_average = score_elements[1].text.strip()
+            subject_scores.append({'考試科目': subject, '個人成績': user_score, '全班平均': class_average})
 
     # 提取總分、平均分數、排名和科別排名
     total_score = soup.select_one('table.scoreTable-inline td.score').text.strip()
-    
-    average_score_element = soup.select_one('table.scoreTable-inline span.unpass')
-    average_score = average_score_element.text.strip() if average_score_element else "N/A"
+
+    average_score_elements = soup.select('table.scoreTable-inline td.score')
+    average_score = average_score_elements[1].text.strip() if len(average_score_elements) >= 3 else "N/A"
 
     ranking_elements = soup.select('table.scoreTable-inline td.score')
     ranking = ranking_elements[2].text.strip() if len(ranking_elements) >= 3 else "N/A"
     department_ranking = ranking_elements[3].text.strip() if len(ranking_elements) >= 4 else "N/A"
 
     # 建立包含所有資訊的字典
     result = {
-        'code':0,
+        'code': 0,
         '考試標題': soup.select_one('.center.pt-2 .bluetext').text.strip(),
         '學號': soup.select_one('.center.mobile-text-center .mr-3-ow:nth-of-type(1)').text.strip().replace('學號：', ''),
         '姓名': soup.select_one('.center.mobile-text-center .mr-3-ow:nth-of-type(2)').text.strip().replace('姓名：', ''),
         '班級': soup.select_one('.center.mobile-text-center .mr-3-ow:nth-of-type(3)').text.strip().replace('班級：', ''),
         '考試科目成績': subject_scores,
         '總分': total_score,
-        '平均分數': average_score,
+        '平均': average_score,
         '排名': ranking,
         '科別排名': department_ranking
     }
 
     return result
 
+def getGrades(username, password, driver, model,examname,LowConfidence=85):
 
-def getGrades(username, password, driver, model,examname):
-     
     RESET = "\033[0m"
     RED = "\033[31m"
     GREEN = "\033[32m"
     YELLOW = "\033[33m"
 
     loginScess = False
 
     while True:
-        vfc = ""
-        captcha_element = driver.find_element(By.XPATH, '//img[@id="imgvcode"]')
-
-        src = captcha_element.get_attribute('src')
-        print('Image source:', src)
-
-        screenshot_path = 'captcha.png'
-        driver.save_screenshot(screenshot_path)
-        location = captcha_element.location
-        size = captcha_element.size
-        captcha_image = Image.open(screenshot_path)
-        captcha_image = captcha_image.crop((location['x'], location['y'], location['x'] + size['width'], location['y'] + size['height']))
-        width, height = captcha_image.size
-
-        part_width = width // 4
-        captcha_images = []
-        for i in range(4):
-            left = i * part_width
-            right = (i + 1) * part_width
-            part = captcha_image.crop((left, 0, right, height))
-            part = vfcCodeFilter(part)
-            part_path = f'captcha_part{i}.png'
-            part.save(part_path)
-            captcha_images.append(part_path)
-
-        confidence_threshold_low = 50
-        confidence_threshold_medium = 80
-        
-        confidence = [0, 0, 0, 0]
-        count = 0
-
-        for captcha_image_path in captcha_images:
-            predicted_label, predicted_confidence = predict_image(captcha_image_path, captcha_image, model)
-            vfc += str(predicted_label)
-            predicted_confidence = predicted_confidence * 100
-            confidence[count] = predicted_confidence
-            count += 1
-
-            if predicted_confidence < confidence_threshold_low:
-                print(f"{RED}驗證碼: {predicted_label} 置信度: {predicted_confidence} %{RESET}")
-            elif predicted_confidence < confidence_threshold_medium:
-                print(f"{YELLOW}驗證碼: {predicted_label} 置信度: {predicted_confidence} %{RESET}")
-            else:
-                print(f"{GREEN}驗證碼: {predicted_label} 置信度: {predicted_confidence} %{RESET}")
+        allConfidence = 0
+        while allConfidence <= LowConfidence :
+            vfc = ""
+            captcha_element = driver.find_element(By.XPATH, '//img[@id="imgvcode"]')
+
+            src = captcha_element.get_attribute('src')
+            print('Image source:', src)
+
+            screenshot_path = 'captcha.png'
+            driver.save_screenshot(screenshot_path)
+            location = captcha_element.location
+            size = captcha_element.size
+            captcha_image = Image.open(screenshot_path)
+            captcha_image = captcha_image.crop((location['x'], location['y'], location['x'] + size['width'], location['y'] + size['height']))
+            width, height = captcha_image.size
+
+            part_width = width // 4
+            captcha_images = []
+            for i in range(4):
+                left = i * part_width
+                right = (i + 1) * part_width
+                part = captcha_image.crop((left, 0, right, height))
+                part = vfcCodeFilter(part)
+                part_path = f'captcha_part{i}.png'
+                part.save(part_path)
+                captcha_images.append(part_path)
+
+            confidence_threshold_low = 50
+            confidence_threshold_medium = 80
+            
+            confidence = [0, 0, 0, 0]
+            count = 0
+
+            for captcha_image_path in captcha_images:
+                predicted_label, predicted_confidence = predict_image(captcha_image_path, captcha_image, model)
+                vfc += str(predicted_label)
+                predicted_confidence = predicted_confidence * 100
+                confidence[count] = predicted_confidence
+                count += 1
+
+                if predicted_confidence < confidence_threshold_low:
+                    print(f"{RED}驗證碼: {predicted_label} 置信度: {predicted_confidence} %{RESET}")
+                elif predicted_confidence < confidence_threshold_medium:
+                    print(f"{YELLOW}驗證碼: {predicted_label} 置信度: {predicted_confidence} %{RESET}")
+                else:
+                    print(f"{GREEN}驗證碼: {predicted_label} 置信度: {predicted_confidence} %{RESET}")
+
+            allConfidence = confidence[0] * confidence[1] * confidence[2] * confidence[3] * 0.000001
+            print("\033[33m 驗證碼影像辨識:" + str(vfc) + "  本次準確率:" + str(allConfidence) + " % \033[0m")
+
+            if allConfidence <= LowConfidence :
+                driver.refresh()
+        print("\033[36m 驗證碼準確率達標 \033[0m")
 
-        allConfidence = confidence[0] * confidence[1] * confidence[2] * confidence[3] * 0.000001
-        print("驗證碼影像辨識:" + str(vfc) + "  本次準確率:" + str(allConfidence) + " %")
 
         vcode = vfc
         # login
         username_element = driver.find_element(By.ID, 'Loginid')
         username_element.send_keys(username)
         password_element = driver.find_element(By.ID, 'LoginPwd')
         password_element.send_keys(password)
```

### Comparing `shinherpro-1.6.0/shinherpro.egg-info/PKG-INFO` & `shinherpro-1.6.1/shinherpro.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: shinherpro
-Version: 1.6.0
-Summary: shinher-pro 1.6.0
+Version: 1.6.1
+Summary: shinher-pro 1.6.1
 Author: Yihuan
 Author-email: ivan17.lai@gmail.com
 Description-Content-Type: text/markdown
 
-# Shinher-Pro V1.5.7
+# Shinher-Pro V1.6.1
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
 
 ## use
 ```
 from shinherpro import TYAI
 ```
@@ -34,36 +34,41 @@
 ```
 url = TYAI.urlGet() = "https://sai.tyai.tyc.edu.tw/online/"
 driver = TYAI.chrome_driver_setup(url,True)
 ```
 ## get grade
 ### TYAI.getGrades() 函式用於獲取成績資訊。你需要提供(學號、密碼(身分證字號)、WebDriver對象、AI模型、考試名稱)作為輸入參數。函式內部進行驗證碼辨識、登入操作，然後切換到成績查詢頁面，獲取成績表格的 HTML 內容,並使用json格式回傳.
 ```
-TYAI.getGrades(username, password, driver, model,examname):
+TYAI.getGrades(username, password, driver, model,examname,LowConfidence):
 ```
 ### driver、model 為提前初始化所取得的回傳值
+### username, password 為帳號密碼
+### exam 為考試列表需準確無誤
+### LowConfidence 非必填，預設為85，為驗證碼AI的準確度要求，若AI判斷本次驗證碼準確率低於指定值，則會重新整理網頁獲取新的驗證碼。
 ### 可以根據 code 的值來判斷返回結果的狀態，並根據需要處理相應的資訊。
 ### code 0 正常回傳成績 , code 1 帳號密碼錯誤 , code 2 登入失敗次數過多 , code 3 未知的錯誤訊息 
 
 ### 如果登入成功，成績查詢成功，則返回以下格式的json：
 ```
 {
     "code": 0,
     "考試標題": "考試標題",
     "學號": "學號",
     "姓名": "姓名",
     "班級": "班級",
     "考試科目成績": [
         {
             "考試科目": "科目1",
-            "考試成績": "成績1"
+            "考試成績": "成績1",
+            "全班平均": "平均1"
         },
         {
             "考試科目": "科目2",
-            "考試成績": "成績2"
+            "考試成績": "成績2",
+            "全班平均": "平均2"
         },
         ...
     ],
     "總分": "總分",
     "平均分數": "平均分數",
     "排名": "排名",
     "科別排名": "科別排名"
@@ -75,14 +80,18 @@
 {
     "code": 1,
     "reason": "帳號或密碼錯誤,請重新登入!"
 }
 ```
 ### 其中，code 表示返回的狀態碼，1 表示帳號或密碼錯誤。reason 表示錯誤原因的描述。
 ### 如果登入失敗次數過多，則返回以下格式的字典：
+{
+    "code": 2,
+    "reason": "帳號登入失敗次數過多，請於15分鐘後再嘗試登入!!"
+}
 ### 其中，code 表示返回的狀態碼，2 表示登入失敗次數過多。reason 表示錯誤原因的描述。
 ### 如果其他未知錯誤發生，則返回以下格式的字典：
 ```
 {
     "code": 3,
     "reason": "錯誤原因"
 }
```

