# Comparing `tmp/krxreader-0.0.dev1.tar.gz` & `tmp/krxreader-0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krxreader-0.0.dev1.tar", last modified: Tue Aug 23 05:02:18 2022, max compression
+gzip compressed data, was "krxreader-0.0.dev2.tar", last modified: Sun May 21 08:16:18 2023, max compression
```

## Comparing `krxreader-0.0.dev1.tar` & `krxreader-0.0.dev2.tar`

### file list

```diff
@@ -1,18 +1,28 @@
-drwxr-xr-x   0 gunhoon    (501) staff       (20)        0 2022-08-23 05:02:18.283616 krxreader-0.0.dev1/
--rw-r--r--   0 gunhoon    (501) staff       (20)     1068 2022-08-23 05:00:24.000000 krxreader-0.0.dev1/LICENSE
--rw-r--r--   0 gunhoon    (501) staff       (20)     1939 2022-08-23 05:02:18.283243 krxreader-0.0.dev1/PKG-INFO
--rw-r--r--   0 gunhoon    (501) staff       (20)      120 2022-08-23 05:00:24.000000 krxreader-0.0.dev1/README.md
--rw-r--r--   0 gunhoon    (501) staff       (20)      676 2022-08-23 05:00:24.000000 krxreader-0.0.dev1/pyproject.toml
--rw-r--r--   0 gunhoon    (501) staff       (20)       38 2022-08-23 05:02:18.283763 krxreader-0.0.dev1/setup.cfg
-drwxr-xr-x   0 gunhoon    (501) staff       (20)        0 2022-08-23 05:02:18.278203 krxreader-0.0.dev1/src/
-drwxr-xr-x   0 gunhoon    (501) staff       (20)        0 2022-08-23 05:02:18.281227 krxreader-0.0.dev1/src/krxreader/
--rw-r--r--   0 gunhoon    (501) staff       (20)        0 2022-08-23 05:00:24.000000 krxreader-0.0.dev1/src/krxreader/__init__.py
--rw-r--r--   0 gunhoon    (501) staff       (20)      628 2022-08-23 05:00:24.000000 krxreader-0.0.dev1/src/krxreader/_calendar.py
--rw-r--r--   0 gunhoon    (501) staff       (20)     1217 2022-08-23 05:00:24.000000 krxreader-0.0.dev1/src/krxreader/_krx.py
--rw-r--r--   0 gunhoon    (501) staff       (20)     1797 2022-08-23 05:00:24.000000 krxreader-0.0.dev1/src/krxreader/index.py
--rw-r--r--   0 gunhoon    (501) staff       (20)     1478 2022-08-23 05:00:24.000000 krxreader-0.0.dev1/src/krxreader/stock.py
-drwxr-xr-x   0 gunhoon    (501) staff       (20)        0 2022-08-23 05:02:18.282718 krxreader-0.0.dev1/src/krxreader.egg-info/
--rw-r--r--   0 gunhoon    (501) staff       (20)     1939 2022-08-23 05:02:18.000000 krxreader-0.0.dev1/src/krxreader.egg-info/PKG-INFO
--rw-r--r--   0 gunhoon    (501) staff       (20)      301 2022-08-23 05:02:18.000000 krxreader-0.0.dev1/src/krxreader.egg-info/SOURCES.txt
--rw-r--r--   0 gunhoon    (501) staff       (20)        1 2022-08-23 05:02:18.000000 krxreader-0.0.dev1/src/krxreader.egg-info/dependency_links.txt
--rw-r--r--   0 gunhoon    (501) staff       (20)       10 2022-08-23 05:02:18.000000 krxreader-0.0.dev1/src/krxreader.egg-info/top_level.txt
+drwxr-xr-x   0 gunhoon    (501) staff       (20)        0 2023-05-21 08:16:18.442472 krxreader-0.0.dev2/
+-rw-r--r--   0 gunhoon    (501) staff       (20)     1068 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/LICENSE
+-rw-r--r--   0 gunhoon    (501) staff       (20)     1939 2023-05-21 08:16:18.441879 krxreader-0.0.dev2/PKG-INFO
+-rw-r--r--   0 gunhoon    (501) staff       (20)      120 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/README.md
+-rw-r--r--   0 gunhoon    (501) staff       (20)      714 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/pyproject.toml
+-rw-r--r--   0 gunhoon    (501) staff       (20)       38 2023-05-21 08:16:18.442654 krxreader-0.0.dev2/setup.cfg
+drwxr-xr-x   0 gunhoon    (501) staff       (20)        0 2023-05-21 08:16:18.430667 krxreader-0.0.dev2/src/
+drwxr-xr-x   0 gunhoon    (501) staff       (20)        0 2023-05-21 08:16:18.435818 krxreader-0.0.dev2/src/krxreader/
+-rw-r--r--   0 gunhoon    (501) staff       (20)        0 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/src/krxreader/__init__.py
+-rw-r--r--   0 gunhoon    (501) staff       (20)      628 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/src/krxreader/_calendar.py
+-rw-r--r--   0 gunhoon    (501) staff       (20)     1094 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/src/krxreader/base.py
+-rw-r--r--   0 gunhoon    (501) staff       (20)     1259 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/src/krxreader/bond.py
+-rw-r--r--   0 gunhoon    (501) staff       (20)      627 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/src/krxreader/fetch.py
+-rw-r--r--   0 gunhoon    (501) staff       (20)     2129 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/src/krxreader/index.py
+-rw-r--r--   0 gunhoon    (501) staff       (20)       29 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/src/krxreader/sample.py
+-rw-r--r--   0 gunhoon    (501) staff       (20)     1232 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/src/krxreader/stock.py
+drwxr-xr-x   0 gunhoon    (501) staff       (20)        0 2023-05-21 08:16:18.438326 krxreader-0.0.dev2/src/krxreader.egg-info/
+-rw-r--r--   0 gunhoon    (501) staff       (20)     1939 2023-05-21 08:16:18.000000 krxreader-0.0.dev2/src/krxreader.egg-info/PKG-INFO
+-rw-r--r--   0 gunhoon    (501) staff       (20)      506 2023-05-21 08:16:18.000000 krxreader-0.0.dev2/src/krxreader.egg-info/SOURCES.txt
+-rw-r--r--   0 gunhoon    (501) staff       (20)        1 2023-05-21 08:16:18.000000 krxreader-0.0.dev2/src/krxreader.egg-info/dependency_links.txt
+-rw-r--r--   0 gunhoon    (501) staff       (20)        9 2023-05-21 08:16:18.000000 krxreader-0.0.dev2/src/krxreader.egg-info/requires.txt
+-rw-r--r--   0 gunhoon    (501) staff       (20)       10 2023-05-21 08:16:18.000000 krxreader-0.0.dev2/src/krxreader.egg-info/top_level.txt
+drwxr-xr-x   0 gunhoon    (501) staff       (20)        0 2023-05-21 08:16:18.441142 krxreader-0.0.dev2/tests/
+-rw-r--r--   0 gunhoon    (501) staff       (20)      827 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/tests/test_base.py
+-rw-r--r--   0 gunhoon    (501) staff       (20)      923 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/tests/test_fetch.py
+-rw-r--r--   0 gunhoon    (501) staff       (20)      413 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/tests/test_index.py
+-rw-r--r--   0 gunhoon    (501) staff       (20)       74 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/tests/test_sample.py
+-rw-r--r--   0 gunhoon    (501) staff       (20)      912 2023-05-21 08:12:21.000000 krxreader-0.0.dev2/tests/test_stock.py
```

### Comparing `krxreader-0.0.dev1/LICENSE` & `krxreader-0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `krxreader-0.0.dev1/PKG-INFO` & `krxreader-0.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krxreader
-Version: 0.0.dev1
+Version: 0.0.dev2
 Summary: KRXReader is a library for scraping financial data from the KRX(Korea Exchange) Market Data System.
 Author-email: Gunhoon Lee <gunhoon@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Gunhoon Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `krxreader-0.0.dev1/pyproject.toml` & `krxreader-0.0.dev2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
 [project]
 name = "krxreader"
-version = "0.0.dev1"
-authors = [
-  { name="Gunhoon Lee", email="gunhoon@gmail.com" },
-]
+version = "0.0.dev2"
 description = "KRXReader is a library for scraping financial data from the KRX(Korea Exchange) Market Data System."
 readme = "README.md"
-license = { file="LICENSE" }
 requires-python = ">=3.7"
+license = {file = "LICENSE"}
+authors = [
+    {name = "Gunhoon Lee", email = "gunhoon@gmail.com"}
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "requests",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/gunhoon/krxreader"
 "Bug Tracker" = "https://github.com/gunhoon/krxreader/issues"
+
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
```

### Comparing `krxreader-0.0.dev1/src/krxreader/_calendar.py` & `krxreader-0.0.dev2/src/krxreader/_calendar.py`

 * *Files identical despite different names*

### Comparing `krxreader-0.0.dev1/src/krxreader/_krx.py` & `krxreader-0.0.dev2/tests/test_fetch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,42 @@
-import requests
+import pytest
 
+from krxreader.fetch import get_json_data
+from krxreader.fetch import download_csv
 
-def get_json_data(data):
-    url = 'http://data.krx.co.kr/comm/bldAttendant/getJsonData.cmd'
 
-    r = requests.post(url=url, data=data)
-    dic = r.json()
-
-    return dic
-
-
-def download_csv(data):
-    # 1. Generate OTP
-    generate_url = 'http://data.krx.co.kr/comm/fileDn/GenerateOTP/generate.cmd'
-
-    r = requests.post(url=generate_url, data=data)
-    otp = {
-        'code': r.text
-    }
-
-    # 2. Download CSV
-    download_url = 'http://data.krx.co.kr/comm/fileDn/download_csv/download.cmd'
-
-    r = requests.post(url=download_url, data=otp)
-    csv = r.content.decode(encoding='euc_kr')
-
-    return csv
-
-
-if __name__ == '__main__':
-    params = {
+@pytest.fixture
+def params():
+    """[11001] 지수 > 주가지수 > 전체지수 시세
+    :return: dictionary
+    """
+    return {
         'bld': 'dbms/MDC/STAT/standard/MDCSTAT00101',
         'locale': 'ko_KR',
         'idxIndMidclssCd': '01',
-        'trdDd': '20220822',
+        'trdDd': '20230519',
         'share': '2',
         'money': '3',
         'csvxls_isNo': 'false'
     }
 
-    d = get_json_data(params)
 
-    print('=======================================')
-    print(type(d))
-    print(d)
+def test_get_json_data(params):
+    json = get_json_data(params)
+    data = json['output']
 
+    assert data[0]['IDX_NM'] == 'KRX 300'
+    assert data[0]['CLSPRC_IDX'] == '1,533.13'
+
+
+def test_download_csv(params):
+    bld = params.pop('bld')
     params['name'] = 'fileDown'
-    params['url'] = params['bld']
-    del params['bld']
+    params['url'] = bld
+
+    csv = download_csv(params)
 
-    c = download_csv(params)
+    lines = csv.splitlines()
+    first = lines[1].split(',')
 
-    print('=======================================')
-    print(type(c))
-    print(c)
+    assert first[0] == '"KRX 300"'
+    assert first[1] == '"1533.13"'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `krxreader-0.0.dev1/src/krxreader.egg-info/PKG-INFO` & `krxreader-0.0.dev2/src/krxreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krxreader
-Version: 0.0.dev1
+Version: 0.0.dev2
 Summary: KRXReader is a library for scraping financial data from the KRX(Korea Exchange) Market Data System.
 Author-email: Gunhoon Lee <gunhoon@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Gunhoon Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

