# Comparing `tmp/shinherpro-1.5.9.tar.gz` & `tmp/shinherpro-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinherpro-1.5.9.tar", last modified: Sun May 21 04:37:47 2023, max compression
+gzip compressed data, was "shinherpro-1.6.0.tar", last modified: Sun May 21 05:53:11 2023, max compression
```

## Comparing `shinherpro-1.5.9.tar` & `shinherpro-1.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 04:37:47.124395 shinherpro-1.5.9/
--rw-rw-rw-   0        0        0     3853 2023-05-21 04:37:47.123899 shinherpro-1.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     3673 2023-05-20 13:15:34.000000 shinherpro-1.5.9/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 04:37:47.125389 shinherpro-1.5.9/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-05-21 04:37:40.000000 shinherpro-1.5.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 04:37:47.112491 shinherpro-1.5.9/shinherpro/
--rw-rw-rw-   0        0        0    10986 2023-05-21 04:36:45.000000 shinherpro-1.5.9/shinherpro/TYAI.py
--rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.5.9/shinherpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 04:37:47.122411 shinherpro-1.5.9/shinherpro.egg-info/
--rw-rw-rw-   0        0        0     3853 2023-05-21 04:37:46.000000 shinherpro-1.5.9/shinherpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-05-21 04:37:47.000000 shinherpro-1.5.9/shinherpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 04:37:46.000000 shinherpro-1.5.9/shinherpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-21 04:37:46.000000 shinherpro-1.5.9/shinherpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-21 04:37:46.000000 shinherpro-1.5.9/shinherpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 05:53:11.314465 shinherpro-1.6.0/
+-rw-rw-rw-   0        0        0     3853 2023-05-21 05:53:11.313471 shinherpro-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3673 2023-05-20 13:15:34.000000 shinherpro-1.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 05:53:11.314465 shinherpro-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-05-21 05:53:05.000000 shinherpro-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 05:53:11.301071 shinherpro-1.6.0/shinherpro/
+-rw-rw-rw-   0        0        0    10582 2023-05-21 05:52:45.000000 shinherpro-1.6.0/shinherpro/TYAI.py
+-rw-rw-rw-   0        0        0        0 2023-05-18 14:47:36.000000 shinherpro-1.6.0/shinherpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 05:53:11.311984 shinherpro-1.6.0/shinherpro.egg-info/
+-rw-rw-rw-   0        0        0     3853 2023-05-21 05:53:11.000000 shinherpro-1.6.0/shinherpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-21 05:53:11.000000 shinherpro-1.6.0/shinherpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 05:53:11.000000 shinherpro-1.6.0/shinherpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-21 05:53:11.000000 shinherpro-1.6.0/shinherpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-21 05:53:11.000000 shinherpro-1.6.0/shinherpro.egg-info/top_level.txt
```

### Comparing `shinherpro-1.5.9/PKG-INFO` & `shinherpro-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: shinherpro
-Version: 1.5.9
-Summary: shinher-pro 1.5.9
+Version: 1.6.0
+Summary: shinher-pro 1.6.0
 Author: Yihuan
 Author-email: ivan17.lai@gmail.com
 Description-Content-Type: text/markdown
 
 # Shinher-Pro V1.5.7
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
```

### Comparing `shinherpro-1.5.9/README.md` & `shinherpro-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `shinherpro-1.5.9/setup.py` & `shinherpro-1.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     def run(self):
         print("\033[93m 正在安裝shinher-pro...")
         install.run(self)
         print("shinherpro安裝完成！ \033[0m")
 
 setup(
     name='shinherpro',
-    version='1.5.9',
-    description='shinher-pro 1.5.9',
+    version='1.6.0',
+    description='shinher-pro 1.6.0',
     author='Yihuan',
     author_email='ivan17.lai@gmail.com',
     packages=['shinherpro'],
     install_requires=[
         'selenium',
         'beautifulsoup4',
         'keras',
```

### Comparing `shinherpro-1.5.9/shinherpro/TYAI.py` & `shinherpro-1.6.0/shinherpro/TYAI.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,19 +259,8 @@
     new_page_source = driver.page_source
     # 成績表格分析
     result = score_tolist(new_page_source)
     loginScess = True
 
     driver.delete_all_cookies()
     driver.refresh()
-    return result
-
-
-# for test
-if True:
-    model1 = model_setup("E:\\project\\vfc_AiModel_5.1_VGG16_black.h5")
-
-    driver1 = chrome_driver_setup(urlGet(),False)
-
-    print(getGrades(username="013333",password="B123742969",driver=driver1,model=model1,examname='[111下] 111下第1次段考'))
-    #print(getGrades(username="",password="",driver=driver1,model=model1,examname='[111下] 111下第2次段考'))
- 
+    return result
```

### Comparing `shinherpro-1.5.9/shinherpro.egg-info/PKG-INFO` & `shinherpro-1.6.0/shinherpro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: shinherpro
-Version: 1.5.9
-Summary: shinher-pro 1.5.9
+Version: 1.6.0
+Summary: shinher-pro 1.6.0
 Author: Yihuan
 Author-email: ivan17.lai@gmail.com
 Description-Content-Type: text/markdown
 
 # Shinher-Pro V1.5.7
 
 ### 這個程式是一個自動化的成績查詢工具，它使用 Selenium 和 BeautifulSoup 套件來模擬網頁瀏覽和解析 HTML 內容，並使用 Keras 加載自訓練的 AI 模型進行圖形驗證碼自動辨識。它可以自動登入到支援的成績查詢網站，通常是欣河線上查詢系統，只需輸入帳號密碼，程序會自動操作到成績業面並返回成績，跳過原先繁雜的操作。
```

