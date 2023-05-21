# Comparing `tmp/pywxdll-0.1.3.tar.gz` & `tmp/pywxdll-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywxdll-0.1.3.tar", last modified: Tue May  2 16:51:51 2023, max compression
+gzip compressed data, was "dist/pywxdll-0.1.4.tar", last modified: Sun May 21 13:12:26 2023, max compression
```

## Comparing `pywxdll-0.1.3.tar` & `pywxdll-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-02 16:51:51.000000 pywxdll-0.1.3/
--rw-r--r--   0 henryyang   (501) staff       (20)     1067 2023-04-30 06:33:02.000000 pywxdll-0.1.3/LICENSE
--rw-rw-r--   0 henryyang   (501) staff       (20)       26 2023-05-01 18:24:33.000000 pywxdll-0.1.3/MANIFEST.in
--rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-02 16:51:51.000000 pywxdll-0.1.3/PKG-INFO
--rw-r--r--   0 henryyang   (501) staff       (20)      577 2023-05-02 16:49:34.000000 pywxdll-0.1.3/README.md
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-02 16:51:51.000000 pywxdll-0.1.3/pywxdll/
--rw-r--r--   0 henryyang   (501) staff       (20)       74 2023-05-02 16:49:09.000000 pywxdll-0.1.3/pywxdll/__init__.py
--rw-r--r--   0 henryyang   (501) staff       (20)     7349 2023-05-02 16:34:24.000000 pywxdll-0.1.3/pywxdll/pywxdll.py
--rw-r--r--   0 henryyang   (501) staff       (20)     4000 2023-05-02 16:30:12.000000 pywxdll-0.1.3/pywxdll/pywxdll_json.py
-drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-02 16:51:51.000000 pywxdll-0.1.3/pywxdll.egg-info/
--rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-02 16:36:22.000000 pywxdll-0.1.3/pywxdll.egg-info/.gitignore
--rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-02 16:51:51.000000 pywxdll-0.1.3/pywxdll.egg-info/PKG-INFO
--rw-r--r--   0 henryyang   (501) staff       (20)      283 2023-05-02 16:51:51.000000 pywxdll-0.1.3/pywxdll.egg-info/SOURCES.txt
--rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-02 16:51:51.000000 pywxdll-0.1.3/pywxdll.egg-info/dependency_links.txt
--rw-r--r--   0 henryyang   (501) staff       (20)       26 2023-05-02 16:51:51.000000 pywxdll-0.1.3/pywxdll.egg-info/requires.txt
--rw-r--r--   0 henryyang   (501) staff       (20)        8 2023-05-02 16:51:51.000000 pywxdll-0.1.3/pywxdll.egg-info/top_level.txt
--rw-r--r--   0 henryyang   (501) staff       (20)       38 2023-05-02 16:51:51.000000 pywxdll-0.1.3/setup.cfg
--rw-r--r--   0 henryyang   (501) staff       (20)     3743 2023-05-02 16:50:27.000000 pywxdll-0.1.3/setup.py
+drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-21 13:12:26.000000 pywxdll-0.1.4/
+-rw-r--r--   0 henryyang   (501) staff       (20)     1067 2023-04-30 06:33:02.000000 pywxdll-0.1.4/LICENSE
+-rw-rw-r--   0 henryyang   (501) staff       (20)       26 2023-05-01 18:24:33.000000 pywxdll-0.1.4/MANIFEST.in
+-rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-21 13:12:26.000000 pywxdll-0.1.4/PKG-INFO
+-rw-r--r--   0 henryyang   (501) staff       (20)      577 2023-05-02 16:49:34.000000 pywxdll-0.1.4/README.md
+drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-21 13:12:26.000000 pywxdll-0.1.4/pywxdll/
+-rw-r--r--   0 henryyang   (501) staff       (20)       74 2023-05-02 16:49:09.000000 pywxdll-0.1.4/pywxdll/__init__.py
+-rw-r--r--   0 henryyang   (501) staff       (20)     7434 2023-05-21 13:11:18.000000 pywxdll-0.1.4/pywxdll/pywxdll.py
+-rw-r--r--   0 henryyang   (501) staff       (20)     4000 2023-05-02 16:30:12.000000 pywxdll-0.1.4/pywxdll/pywxdll_json.py
+drwxr-xr-x   0 henryyang   (501) staff       (20)        0 2023-05-21 13:12:26.000000 pywxdll-0.1.4/pywxdll.egg-info/
+-rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-02 16:36:22.000000 pywxdll-0.1.4/pywxdll.egg-info/.gitignore
+-rw-r--r--   0 henryyang   (501) staff       (20)      699 2023-05-21 13:12:26.000000 pywxdll-0.1.4/pywxdll.egg-info/PKG-INFO
+-rw-r--r--   0 henryyang   (501) staff       (20)      283 2023-05-21 13:12:26.000000 pywxdll-0.1.4/pywxdll.egg-info/SOURCES.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)        1 2023-05-21 13:12:26.000000 pywxdll-0.1.4/pywxdll.egg-info/dependency_links.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)       26 2023-05-21 13:12:26.000000 pywxdll-0.1.4/pywxdll.egg-info/requires.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)        8 2023-05-21 13:12:26.000000 pywxdll-0.1.4/pywxdll.egg-info/top_level.txt
+-rw-r--r--   0 henryyang   (501) staff       (20)       38 2023-05-21 13:12:26.000000 pywxdll-0.1.4/setup.cfg
+-rw-r--r--   0 henryyang   (501) staff       (20)     3743 2023-05-21 13:12:02.000000 pywxdll-0.1.4/setup.py
```

### Comparing `pywxdll-0.1.3/LICENSE` & `pywxdll-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pywxdll-0.1.3/PKG-INFO` & `pywxdll-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdll
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for wechat dll hook
 Home-page: https://github.com/HenryXiaoYang/pywxdll
 Author: HenryXiaoYang
 Author-email: henryyang666@hotmal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pywxdll-0.1.3/README.md` & `pywxdll-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pywxdll-0.1.3/pywxdll/pywxdll.py` & `pywxdll-0.1.4/pywxdll/pywxdll.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,15 +97,18 @@
             'wxid': 'null',
             'content': 'null',
             'nickname': 'null',
             'ext': 'null',
         }
         base_data.update(data)
         url = f'http://{self.ip}:{self.port}/{uri}'
-        rsp = requests.post(url, json={'para': base_data}, timeout=5)
+        try:
+            rsp = requests.post(url, json={'para': base_data})
+        except:
+            logger('发送信息失败！信息：',base_data)
         rsp = rsp.json()
         if 'content' in rsp and isinstance(rsp['content'], str):
             try:
                 rsp['content'] = json.loads(rsp['content'])
             except:
                 pass
         return rsp
```

### Comparing `pywxdll-0.1.3/pywxdll/pywxdll_json.py` & `pywxdll-0.1.4/pywxdll/pywxdll_json.py`

 * *Files identical despite different names*

### Comparing `pywxdll-0.1.3/pywxdll.egg-info/PKG-INFO` & `pywxdll-0.1.4/pywxdll.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywxdll
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for wechat dll hook
 Home-page: https://github.com/HenryXiaoYang/pywxdll
 Author: HenryXiaoYang
 Author-email: henryyang666@hotmal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pywxdll-0.1.3/setup.py` & `pywxdll-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pywxdll'
 DESCRIPTION = 'A Python package for wechat dll hook'
 URL = 'https://github.com/HenryXiaoYang/pywxdll'
 EMAIL = 'henryyang666@hotmal.com'
 AUTHOR = 'HenryXiaoYang'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = ['websocket-client', 'requests']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

