# Comparing `tmp/csv-embeddings-creator-1.0.4.tar.gz` & `tmp/csv-embeddings-creator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv-embeddings-creator-1.0.4.tar", last modified: Fri May 12 11:54:30 2023, max compression
+gzip compressed data, was "csv-embeddings-creator-1.0.5.tar", last modified: Sun May 21 18:52:52 2023, max compression
```

## Comparing `csv-embeddings-creator-1.0.4.tar` & `csv-embeddings-creator-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 11:54:30.646504 csv-embeddings-creator-1.0.4/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2910 2023-05-12 11:54:30.646407 csv-embeddings-creator-1.0.4/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     2802 2023-05-12 11:54:30.000000 csv-embeddings-creator-1.0.4/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-12 11:54:30.646237 csv-embeddings-creator-1.0.4/csv_embeddings_creator.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2910 2023-05-12 11:54:30.000000 csv-embeddings-creator-1.0.4/csv_embeddings_creator.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-05-12 11:54:30.000000 csv-embeddings-creator-1.0.4/csv_embeddings_creator.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-12 11:54:30.000000 csv-embeddings-creator-1.0.4/csv_embeddings_creator.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       71 2023-05-12 11:54:30.000000 csv-embeddings-creator-1.0.4/csv_embeddings_creator.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-05-12 11:54:30.000000 csv-embeddings-creator-1.0.4/csv_embeddings_creator.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-05-12 11:54:30.000000 csv-embeddings-creator-1.0.4/csv_embeddings_creator.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     2628 2023-05-12 11:54:30.000000 csv-embeddings-creator-1.0.4/csv_embeddings_creator.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-12 11:54:30.646535 csv-embeddings-creator-1.0.4/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-05-12 11:54:30.000000 csv-embeddings-creator-1.0.4/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 18:52:52.322108 csv-embeddings-creator-1.0.5/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3136 2023-05-21 18:52:52.321991 csv-embeddings-creator-1.0.5/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2956 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 18:52:52.321823 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3136 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      322 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       72 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       23 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3074 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/csv_embeddings_creator.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 18:52:52.322143 csv-embeddings-creator-1.0.5/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      552 2023-05-21 18:52:52.000000 csv-embeddings-creator-1.0.5/setup.py
```

### Comparing `csv-embeddings-creator-1.0.4/PKG-INFO` & `csv-embeddings-creator-1.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-Metadata-Version: 2.1
-Name: csv-embeddings-creator
-Version: 1.0.4
-Description-Content-Type: text/markdown
+# csv_embeddings_creator v1.0.4 by Bowen Chiu
 
-# csv_embeddings_creator
+這東西可以把 google sheet 或者任意 .csv 變成知識庫，未來就能拿 .pt 檔案群來做句子相似度比對了。
 
 `csv_embeddings_creator` 是一個 Python 套件，用於從 CSV 文件中創建句子嵌入。它使用 Hugging Face Transformers 的 `paraphrase-multilingual-MiniLM-L12-v2` 模型為文本生成嵌入。該套件將文本轉換為 txt 格式並將嵌入保存為 PyTorch 張量文件。
 
 ## 安裝
 
 在安裝 `csv_embeddings_creator` 之前，請確保您的系統已安裝 Python 3.6 或更高版本。
 
 要安裝 `csv_embeddings_creator`，請運行以下命令：
 
 ```bash
-pip install csv_embeddings_creator
+pip install csv-embeddings-creator
 ```
 
 ## 使用方法
 
 ### CLI 示範用法
 
 您可以通過以下 CLI 呼叫方法使用 `csv_embeddings_creator`：
```

### Comparing `csv-embeddings-creator-1.0.4/README.md` & `csv-embeddings-creator-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,30 @@
-# csv_embeddings_creator
+Metadata-Version: 2.1
+Name: csv-embeddings-creator
+Version: 1.0.5
+Summary: UNKNOWN
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
+# csv_embeddings_creator v1.0.4 by Bowen Chiu
+
+這東西可以把 google sheet 或者任意 .csv 變成知識庫，未來就能拿 .pt 檔案群來做句子相似度比對了。
 
 `csv_embeddings_creator` 是一個 Python 套件，用於從 CSV 文件中創建句子嵌入。它使用 Hugging Face Transformers 的 `paraphrase-multilingual-MiniLM-L12-v2` 模型為文本生成嵌入。該套件將文本轉換為 txt 格式並將嵌入保存為 PyTorch 張量文件。
 
 ## 安裝
 
 在安裝 `csv_embeddings_creator` 之前，請確保您的系統已安裝 Python 3.6 或更高版本。
 
 要安裝 `csv_embeddings_creator`，請運行以下命令：
 
 ```bash
-pip install csv_embeddings_creator
+pip install csv-embeddings-creator
 ```
 
 ## 使用方法
 
 ### CLI 示範用法
 
 您可以通過以下 CLI 呼叫方法使用 `csv_embeddings_creator`：
@@ -67,8 +78,10 @@
 
 ### Q: 句子嵌入的尺寸是多少？
 
 A: 使用 `paraphrase-multilingual-MiniLM-L12-v2` 模型生成的句子嵌入的尺寸為 384。不同的 Transformer 模型可能具有不同的嵌入尺寸。
 
 ## 貢獻
 
-我們歡迎您為 `csv_embeddings_creator` 做出貢獻！如果您有任何建議、改進或修復錯誤，請在 GitHub 存儲庫中創建一個 Pull 請求。
+我們歡迎您為 `csv_embeddings_creator` 做出貢獻！如果您有任何建議、改進或修復錯誤，請在 GitHub 存儲庫中創建一個 Pull 請求。
+
+
```

### Comparing `csv-embeddings-creator-1.0.4/csv_embeddings_creator.egg-info/PKG-INFO` & `csv-embeddings-creator-1.0.5/csv_embeddings_creator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: csv-embeddings-creator
-Version: 1.0.4
+Version: 1.0.5
+Summary: UNKNOWN
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-# csv_embeddings_creator
+# csv_embeddings_creator v1.0.4 by Bowen Chiu
+
+這東西可以把 google sheet 或者任意 .csv 變成知識庫，未來就能拿 .pt 檔案群來做句子相似度比對了。
 
 `csv_embeddings_creator` 是一個 Python 套件，用於從 CSV 文件中創建句子嵌入。它使用 Hugging Face Transformers 的 `paraphrase-multilingual-MiniLM-L12-v2` 模型為文本生成嵌入。該套件將文本轉換為 txt 格式並將嵌入保存為 PyTorch 張量文件。
 
 ## 安裝
 
 在安裝 `csv_embeddings_creator` 之前，請確保您的系統已安裝 Python 3.6 或更高版本。
 
 要安裝 `csv_embeddings_creator`，請運行以下命令：
 
 ```bash
-pip install csv_embeddings_creator
+pip install csv-embeddings-creator
 ```
 
 ## 使用方法
 
 ### CLI 示範用法
 
 您可以通過以下 CLI 呼叫方法使用 `csv_embeddings_creator`：
@@ -73,7 +79,9 @@
 ### Q: 句子嵌入的尺寸是多少？
 
 A: 使用 `paraphrase-multilingual-MiniLM-L12-v2` 模型生成的句子嵌入的尺寸為 384。不同的 Transformer 模型可能具有不同的嵌入尺寸。
 
 ## 貢獻
 
 我們歡迎您為 `csv_embeddings_creator` 做出貢獻！如果您有任何建議、改進或修復錯誤，請在 GitHub 存儲庫中創建一個 Pull 請求。
+
+
```

### Comparing `csv-embeddings-creator-1.0.4/csv_embeddings_creator.py` & `csv-embeddings-creator-1.0.5/csv_embeddings_creator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 #!/usr/bin/env python
 # csv_embeddings_creator.py
 import argparse
 import csv
 import glob
 import os
-
+import re
 import torch
 from sentence_transformers import SentenceTransformer
 
 
 def create_embeddings(input_folder, output_txt_folder, output_embeddings_folder, force=False):
     model = SentenceTransformer('paraphrase-multilingual-MiniLM-L12-v2')
 
     os.makedirs(output_txt_folder, exist_ok=True)
     os.makedirs(output_embeddings_folder, exist_ok=True)
 
     csv_files = glob.glob(os.path.join(input_folder, '**/*.csv'), recursive=True)
+    embedding_files = glob.glob(os.path.join(output_embeddings_folder, '**/*.pt'), recursive=True)
+
+    # 跳過已經做完的
+    dic_doc_id = {}
+    for path in embedding_files:
+        doc_id = re.findall('doc-id_(.*?)_spreadsheet', path)[0]
+        dic_doc_id[doc_id] = True
 
+    i = 0
     for csv_file in csv_files:
+        doc_id = re.findall('doc-id_(.*?)_spreadsheet', csv_file)[0]
+        if doc_id in dic_doc_id:
+            continue
+
         file_base_name = os.path.splitext(os.path.basename(csv_file))[0]
         existing_txt_files = glob.glob(os.path.join(output_txt_folder, f"{file_base_name}_*.txt"))
 
         if not force and existing_txt_files:
             continue
 
         with open(csv_file, 'r', encoding='utf-8') as f:
             reader = csv.reader(f)
             next(reader)  # Skip header
 
             for idx, row in enumerate(reader):
+                i += 1
                 folder_txt = os.path.join(output_txt_folder, f"{file_base_name}")
                 os.makedirs(folder_txt, exist_ok=True)
                 txt_file = os.path.join(folder_txt, f"{file_base_name}_{idx + 1}.txt")
                 with open(txt_file, 'w', encoding='utf-8') as txt_f:
                     txt_f.write('"' + '","'.join(row) + '"')
 
                 embeddings = model.encode('"' + '","'.join(row) + '"')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `csv-embeddings-creator-1.0.4/setup.py` & `csv-embeddings-creator-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="csv-embeddings-creator",
-    version="1.0.4",
+    version="1.0.5",
     packages=find_packages(),
     py_modules=['csv_embeddings_creator'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'csv_embeddings_creator = csv_embeddings_creator:main',
         ],
```

