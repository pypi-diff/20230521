# Comparing `tmp/bytez-0.1.94.tar.gz` & `tmp/bytez-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytez-0.1.94.tar", last modified: Sat May 20 23:25:39 2023, max compression
+gzip compressed data, was "bytez-0.1.95.tar", last modified: Sat May 20 23:35:11 2023, max compression
```

## Comparing `bytez-0.1.94.tar` & `bytez-0.1.95.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.940312 bytez-0.1.94/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-20 23:25:39.940312 bytez-0.1.94/PKG-INFO
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       73 2023-03-26 07:05:33.000000 bytez-0.1.94/README.md
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.936313 bytez-0.1.94/bytez/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-14 20:59:27.000000 bytez-0.1.94/bytez/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)   106246 2023-05-20 23:25:39.000000 bytez-0.1.94/bytez/exports.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1152 2023-05-17 01:52:53.000000 bytez-0.1.94/bytez/model.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.940312 bytez-0.1.94/bytez/tasks/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:00:59.000000 bytez-0.1.94/bytez/tasks/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.940312 bytez-0.1.94/bytez/tasks/language_modelling/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:55:06.000000 bytez-0.1.94/bytez/tasks/language_modelling/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.940312 bytez-0.1.94/bytez/tasks/language_modelling/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:55:06.000000 bytez-0.1.94/bytez/tasks/language_modelling/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1356 2023-05-20 01:55:06.000000 bytez-0.1.94/bytez/tasks/language_modelling/_models/blinkdl_rwkv_lm.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1438 2023-05-17 01:53:53.000000 bytez-0.1.94/bytez/tasks/language_modelling/_models/hazyresearch_h3.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      357 2023-05-20 01:50:51.000000 bytez-0.1.94/bytez/tasks/language_modelling/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.940312 bytez-0.1.94/bytez/tasks/style_transfer/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:57.000000 bytez-0.1.94/bytez/tasks/style_transfer/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.940312 bytez-0.1.94/bytez/tasks/style_transfer/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:59.000000 bytez-0.1.94/bytez/tasks/style_transfer/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      761 2023-05-14 20:47:16.000000 bytez-0.1.94/bytez/tasks/style_transfer/_models/cmd_style_transfer.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      686 2023-05-14 20:47:16.000000 bytez-0.1.94/bytez/tasks/style_transfer/_models/fast_style_transfer.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      706 2023-05-14 20:47:16.000000 bytez-0.1.94/bytez/tasks/style_transfer/_models/tensorflow_fast_style.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      547 2023-05-14 20:47:16.000000 bytez-0.1.94/bytez/tasks/style_transfer/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.940312 bytez-0.1.94/bytez/tasks/super_resolution/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:01:49.000000 bytez-0.1.94/bytez/tasks/super_resolution/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.940312 bytez-0.1.94/bytez/tasks/super_resolution/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:22.000000 bytez-0.1.94/bytez/tasks/super_resolution/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     2478 2023-05-14 20:58:15.000000 bytez-0.1.94/bytez/tasks/super_resolution/_models/holmes_alan_dsrvae.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      224 2023-05-14 20:58:15.000000 bytez-0.1.94/bytez/tasks/super_resolution/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.940312 bytez-0.1.94/bytez/tasks/text_summarization/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.000000 bytez-0.1.94/bytez/tasks/text_summarization/__init__.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.940312 bytez-0.1.94/bytez/tasks/text_summarization/_models/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.000000 bytez-0.1.94/bytez/tasks/text_summarization/_models/__init__.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      803 2023-05-14 21:13:12.000000 bytez-0.1.94/bytez/tasks/text_summarization/_models/chriskhanhtran_bert_extractive_summarization.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1079 2023-05-15 21:02:31.000000 bytez-0.1.94/bytez/tasks/text_summarization/_models/dmmiller612_bert_extractive_summarizer.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     2239 2023-05-20 23:25:39.000000 bytez-0.1.94/bytez/tasks/text_summarization/_models/hhousen_docsum.py
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      701 2023-05-20 20:52:40.000000 bytez-0.1.94/bytez/tasks/text_summarization/models.py
-drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:25:39.940312 bytez-0.1.94/bytez.egg-info/
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-20 23:25:39.000000 bytez-0.1.94/bytez.egg-info/PKG-INFO
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1333 2023-05-20 23:25:39.000000 bytez-0.1.94/bytez.egg-info/SOURCES.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        1 2023-05-20 23:25:39.000000 bytez-0.1.94/bytez.egg-info/dependency_links.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       70 2023-05-20 23:25:39.000000 bytez-0.1.94/bytez.egg-info/requires.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        6 2023-05-20 23:25:39.000000 bytez-0.1.94/bytez.egg-info/top_level.txt
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-20 23:25:39.940312 bytez-0.1.94/setup.cfg
--rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      663 2023-05-20 23:25:39.000000 bytez-0.1.94/setup.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:11.078801 bytez-0.1.95/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-20 23:35:11.078801 bytez-0.1.95/PKG-INFO
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       73 2023-03-26 07:05:33.000000 bytez-0.1.95/README.md
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:11.078801 bytez-0.1.95/bytez/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-14 20:59:27.000000 bytez-0.1.95/bytez/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)   106246 2023-05-20 23:35:10.000000 bytez-0.1.95/bytez/exports.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1152 2023-05-17 01:52:53.000000 bytez-0.1.95/bytez/model.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:11.078801 bytez-0.1.95/bytez/tasks/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:00:59.000000 bytez-0.1.95/bytez/tasks/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:11.078801 bytez-0.1.95/bytez/tasks/language_modelling/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:55:06.000000 bytez-0.1.95/bytez/tasks/language_modelling/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:11.078801 bytez-0.1.95/bytez/tasks/language_modelling/_models/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 01:55:06.000000 bytez-0.1.95/bytez/tasks/language_modelling/_models/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1356 2023-05-20 01:55:06.000000 bytez-0.1.95/bytez/tasks/language_modelling/_models/blinkdl_rwkv_lm.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1438 2023-05-17 01:53:53.000000 bytez-0.1.95/bytez/tasks/language_modelling/_models/hazyresearch_h3.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      357 2023-05-20 01:50:51.000000 bytez-0.1.95/bytez/tasks/language_modelling/models.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:11.078801 bytez-0.1.95/bytez/tasks/style_transfer/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:57.000000 bytez-0.1.95/bytez/tasks/style_transfer/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:11.078801 bytez-0.1.95/bytez/tasks/style_transfer/_models/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:59.000000 bytez-0.1.95/bytez/tasks/style_transfer/_models/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      761 2023-05-14 20:47:16.000000 bytez-0.1.95/bytez/tasks/style_transfer/_models/cmd_style_transfer.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      686 2023-05-14 20:47:16.000000 bytez-0.1.95/bytez/tasks/style_transfer/_models/fast_style_transfer.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      706 2023-05-14 20:47:16.000000 bytez-0.1.95/bytez/tasks/style_transfer/_models/tensorflow_fast_style.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      547 2023-05-14 20:47:16.000000 bytez-0.1.95/bytez/tasks/style_transfer/models.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:11.078801 bytez-0.1.95/bytez/tasks/super_resolution/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:01:49.000000 bytez-0.1.95/bytez/tasks/super_resolution/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:11.078801 bytez-0.1.95/bytez/tasks/super_resolution/_models/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-14 21:02:22.000000 bytez-0.1.95/bytez/tasks/super_resolution/_models/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     2478 2023-05-14 20:58:15.000000 bytez-0.1.95/bytez/tasks/super_resolution/_models/holmes_alan_dsrvae.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      224 2023-05-14 20:58:15.000000 bytez-0.1.95/bytez/tasks/super_resolution/models.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:11.078801 bytez-0.1.95/bytez/tasks/text_summarization/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:10.000000 bytez-0.1.95/bytez/tasks/text_summarization/__init__.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:11.078801 bytez-0.1.95/bytez/tasks/text_summarization/_models/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:10.000000 bytez-0.1.95/bytez/tasks/text_summarization/_models/__init__.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      803 2023-05-14 21:13:12.000000 bytez-0.1.95/bytez/tasks/text_summarization/_models/chriskhanhtran_bert_extractive_summarization.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1079 2023-05-15 21:02:31.000000 bytez-0.1.95/bytez/tasks/text_summarization/_models/dmmiller612_bert_extractive_summarizer.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     2221 2023-05-20 23:35:10.000000 bytez-0.1.95/bytez/tasks/text_summarization/_models/hhousen_docsum.py
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      701 2023-05-20 20:52:40.000000 bytez-0.1.95/bytez/tasks/text_summarization/models.py
+drwxrwxr-x   0 inf3rnus  (1000) inf3rnus  (1000)        0 2023-05-20 23:35:11.078801 bytez-0.1.95/bytez.egg-info/
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      409 2023-05-20 23:35:11.000000 bytez-0.1.95/bytez.egg-info/PKG-INFO
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)     1333 2023-05-20 23:35:11.000000 bytez-0.1.95/bytez.egg-info/SOURCES.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        1 2023-05-20 23:35:11.000000 bytez-0.1.95/bytez.egg-info/dependency_links.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       70 2023-05-20 23:35:11.000000 bytez-0.1.95/bytez.egg-info/requires.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)        6 2023-05-20 23:35:11.000000 bytez-0.1.95/bytez.egg-info/top_level.txt
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)       38 2023-05-20 23:35:11.078801 bytez-0.1.95/setup.cfg
+-rw-rw-r--   0 inf3rnus  (1000) inf3rnus  (1000)      663 2023-05-20 23:35:10.000000 bytez-0.1.95/setup.py
```

### Comparing `bytez-0.1.94/bytez/exports.py` & `bytez-0.1.95/bytez/exports.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.94/bytez/model.py` & `bytez-0.1.95/bytez/model.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.94/bytez/tasks/language_modelling/_models/blinkdl_rwkv_lm.py` & `bytez-0.1.95/bytez/tasks/language_modelling/_models/blinkdl_rwkv_lm.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.94/bytez/tasks/language_modelling/_models/hazyresearch_h3.py` & `bytez-0.1.95/bytez/tasks/language_modelling/_models/hazyresearch_h3.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.94/bytez/tasks/style_transfer/_models/cmd_style_transfer.py` & `bytez-0.1.95/bytez/tasks/style_transfer/_models/cmd_style_transfer.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.94/bytez/tasks/style_transfer/_models/fast_style_transfer.py` & `bytez-0.1.95/bytez/tasks/style_transfer/_models/fast_style_transfer.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.94/bytez/tasks/style_transfer/_models/tensorflow_fast_style.py` & `bytez-0.1.95/bytez/tasks/style_transfer/_models/tensorflow_fast_style.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.94/bytez/tasks/style_transfer/models.py` & `bytez-0.1.95/bytez/tasks/style_transfer/models.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.94/bytez/tasks/super_resolution/_models/holmes_alan_dsrvae.py` & `bytez-0.1.95/bytez/tasks/super_resolution/_models/holmes_alan_dsrvae.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.94/bytez/tasks/text_summarization/_models/chriskhanhtran_bert_extractive_summarization.py` & `bytez-0.1.95/bytez/tasks/text_summarization/_models/chriskhanhtran_bert_extractive_summarization.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.94/bytez/tasks/text_summarization/_models/dmmiller612_bert_extractive_summarizer.py` & `bytez-0.1.95/bytez/tasks/text_summarization/_models/dmmiller612_bert_extractive_summarizer.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.94/bytez/tasks/text_summarization/_models/hhousen_docsum.py` & `bytez-0.1.95/bytez/tasks/text_summarization/_models/hhousen_docsum.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 
 Returns:
 
 - Dict[str, str]: The output of the summarization. This is a dictionary of chapter and headings to summarized text.
         """
 
         request_params = {
-    "input_pdf": "input_pdf",
-    "preprocess": "preprocess",
-    "model": "model",
-    "bart_checkpoint": "bart_checkpoint",
-    "bart_state_dict_key": "bart_state_dict_key",
-    "bart_fairseq": "bart_fairseq",
-    "chapter_heading_font": "chapter_heading_font",
-    "body_heading_font": "body_heading_font",
-    "body_font": "body_font"
+    "input_pdf": input_pdf,
+    "preprocess": preprocess,
+    "model": model,
+    "bart_checkpoint": bart_checkpoint,
+    "bart_state_dict_key": bart_state_dict_key,
+    "bart_fairseq": bart_fairseq,
+    "chapter_heading_font": chapter_heading_font,
+    "body_heading_font": body_heading_font,
+    "body_font": body_font
 }
 
         url = 'https://hhousen-docsum-tfhmsoxnpq-uc.a.run.app'
 
         return self._Model__inference(url=url, request_params=request_params)
```

### Comparing `bytez-0.1.94/bytez/tasks/text_summarization/models.py` & `bytez-0.1.95/bytez/tasks/text_summarization/models.py`

 * *Files identical despite different names*

### Comparing `bytez-0.1.94/bytez.egg-info/SOURCES.txt` & `bytez-0.1.95/bytez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytez-0.1.94/setup.py` & `bytez-0.1.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 packages = find_packages()
 
 
 setup(
     name='bytez',
-    version='0.1.94',
+    version='0.1.95',
     packages=packages,
     install_requires=[
         'charset-normalizer==3.1.0',
         'idna==3.4',
         'requests==2.28.2',
         'urllib3==1.26.15',
     ],
```

