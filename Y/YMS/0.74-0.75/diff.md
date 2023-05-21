# Comparing `tmp/YMS-0.74.tar.gz` & `tmp/YMS-0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YMS-0.74.tar", last modified: Tue May  9 22:19:41 2023, max compression
+gzip compressed data, was "YMS-0.75.tar", last modified: Sun May 21 12:28:16 2023, max compression
```

## Comparing `YMS-0.74.tar` & `YMS-0.75.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-09 22:19:41.555065 YMS-0.74/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-09 22:19:41.555065 YMS-0.74/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.74/README.md
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-09 22:19:41.555065 YMS-0.74/YMS.egg-info/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-09 22:19:41.000000 YMS-0.74/YMS.egg-info/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-09 22:19:41.000000 YMS-0.74/YMS.egg-info/SOURCES.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-09 22:19:41.000000 YMS-0.74/YMS.egg-info/dependency_links.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-09 22:19:41.000000 YMS-0.74/YMS.egg-info/entry_points.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-09 22:19:41.000000 YMS-0.74/YMS.egg-info/requires.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-09 22:19:41.000000 YMS-0.74/YMS.egg-info/top_level.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-09 22:19:41.555065 YMS-0.74/setup.cfg
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      476 2023-05-09 22:04:47.000000 YMS-0.74/setup.py
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-09 22:19:41.555065 YMS-0.74/yamas/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.74/yamas/__init__.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.74/yamas/config.json
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9581 2023-05-09 22:04:26.000000 YMS-0.74/yamas/create_visualization.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.74/yamas/dataset_downloading.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.74/yamas/export_data.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.74/yamas/utilities.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-21 12:28:16.043363 YMS-0.75/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-21 12:28:16.043363 YMS-0.75/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.75/README.md
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-21 12:28:16.043363 YMS-0.75/YMS.egg-info/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-21 12:28:15.000000 YMS-0.75/YMS.egg-info/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-21 12:28:16.000000 YMS-0.75/YMS.egg-info/SOURCES.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-21 12:28:16.000000 YMS-0.75/YMS.egg-info/dependency_links.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-21 12:28:16.000000 YMS-0.75/YMS.egg-info/entry_points.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-21 12:28:16.000000 YMS-0.75/YMS.egg-info/requires.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-21 12:28:16.000000 YMS-0.75/YMS.egg-info/top_level.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-21 12:28:16.043363 YMS-0.75/setup.cfg
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      476 2023-05-21 12:28:04.000000 YMS-0.75/setup.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-21 12:28:16.043363 YMS-0.75/yamas/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.75/yamas/__init__.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.75/yamas/config.json
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9562 2023-05-21 12:24:39.000000 YMS-0.75/yamas/create_visualization.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.75/yamas/dataset_downloading.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.75/yamas/export_data.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.75/yamas/utilities.py
```

### Comparing `YMS-0.74/README.md` & `YMS-0.75/README.md`

 * *Files identical despite different names*

### Comparing `YMS-0.74/yamas/__init__.py` & `YMS-0.75/yamas/__init__.py`

 * *Files identical despite different names*

### Comparing `YMS-0.74/yamas/create_visualization.py` & `YMS-0.75/yamas/create_visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,19 +131,18 @@
 def metaphlan_extraction(reads_data, dataset_id):
     fastq_path = os.path.join(reads_data.dir_path, "fastq")
     export_path = os.path.join(reads_data.dir_path, "export")
     run_cmd([f"mkdir {export_path}"])
     final_output_path = os.path.join(export_path, f'{dataset_id}_final.txt')
     run_cmd([f"touch {final_output_path}"])
     args = []
-    for fastq_file in tqdm(os.listdir(fastq_path)):
-        fastq, extension = os.path.splitext(fastq_file)
+    for fastq in tqdm([a for a in os.listdir(fastq_path) if a.split(".")[-1] == "fastq"]):
         input = os.path.join(fastq_path,fastq)
         output = os.path.join(os.path.join(reads_data.dir_path, 'qza'), f'{fastq}_profile.txt')
-        command = [f"metaphlan {input} --input_type fastq --nproc 16 > {output} "]
+        command = [f"metaphlan {input} --input_type fastq --nproc 1 > {output} "]
         run_cmd(command)
         args.append(output)
     merge(args, open(final_output_path, 'w'), gtdb=False)
 
 
 def visualization(acc_list, dataset_id, data_type, verbose_print, specific_location):
     verbose_print("\n")
```

### Comparing `YMS-0.74/yamas/dataset_downloading.py` & `YMS-0.75/yamas/dataset_downloading.py`

 * *Files identical despite different names*

### Comparing `YMS-0.74/yamas/export_data.py` & `YMS-0.75/yamas/export_data.py`

 * *Files identical despite different names*

### Comparing `YMS-0.74/yamas/utilities.py` & `YMS-0.75/yamas/utilities.py`

 * *Files identical despite different names*

