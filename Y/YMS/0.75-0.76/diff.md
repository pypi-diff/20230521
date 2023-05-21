# Comparing `tmp/YMS-0.75.tar.gz` & `tmp/YMS-0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YMS-0.75.tar", last modified: Sun May 21 12:28:16 2023, max compression
+gzip compressed data, was "YMS-0.76.tar", last modified: Sun May 21 14:06:55 2023, max compression
```

## Comparing `YMS-0.75.tar` & `YMS-0.76.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-21 12:28:16.043363 YMS-0.75/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-21 12:28:16.043363 YMS-0.75/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.75/README.md
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-21 12:28:16.043363 YMS-0.75/YMS.egg-info/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-21 12:28:15.000000 YMS-0.75/YMS.egg-info/PKG-INFO
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-21 12:28:16.000000 YMS-0.75/YMS.egg-info/SOURCES.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-21 12:28:16.000000 YMS-0.75/YMS.egg-info/dependency_links.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-21 12:28:16.000000 YMS-0.75/YMS.egg-info/entry_points.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-21 12:28:16.000000 YMS-0.75/YMS.egg-info/requires.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-21 12:28:16.000000 YMS-0.75/YMS.egg-info/top_level.txt
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-21 12:28:16.043363 YMS-0.75/setup.cfg
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      476 2023-05-21 12:28:04.000000 YMS-0.75/setup.py
-drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-21 12:28:16.043363 YMS-0.75/yamas/
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.75/yamas/__init__.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.75/yamas/config.json
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9562 2023-05-21 12:24:39.000000 YMS-0.75/yamas/create_visualization.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.75/yamas/dataset_downloading.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.75/yamas/export_data.py
--rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.75/yamas/utilities.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-21 14:06:55.911554 YMS-0.76/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-21 14:06:55.911554 YMS-0.76/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     2003 2023-04-02 09:28:26.000000 YMS-0.76/README.md
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-21 14:06:55.907554 YMS-0.76/YMS.egg-info/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      156 2023-05-21 14:06:55.000000 YMS-0.76/YMS.egg-info/PKG-INFO
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      317 2023-05-21 14:06:55.000000 YMS-0.76/YMS.egg-info/SOURCES.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        1 2023-05-21 14:06:55.000000 YMS-0.76/YMS.egg-info/dependency_links.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       37 2023-05-21 14:06:55.000000 YMS-0.76/YMS.egg-info/entry_points.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       15 2023-05-21 14:06:55.000000 YMS-0.76/YMS.egg-info/requires.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)        6 2023-05-21 14:06:55.000000 YMS-0.76/YMS.egg-info/top_level.txt
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       38 2023-05-21 14:06:55.911554 YMS-0.76/setup.cfg
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)      476 2023-05-21 14:06:48.000000 YMS-0.76/setup.py
+drwxrwxr-x   0 yarinbekor  (1000) yarinbekor  (1000)        0 2023-05-21 14:06:55.911554 YMS-0.76/yamas/
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1942 2023-05-09 16:55:03.000000 YMS-0.76/yamas/__init__.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)       30 2023-03-26 09:25:23.000000 YMS-0.76/yamas/config.json
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)    11186 2023-05-21 14:06:05.000000 YMS-0.76/yamas/create_visualization.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1015 2023-05-09 16:55:03.000000 YMS-0.76/yamas/dataset_downloading.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     9100 2023-04-02 11:41:02.000000 YMS-0.76/yamas/export_data.py
+-rw-rw-r--   0 yarinbekor  (1000) yarinbekor  (1000)     1183 2023-03-09 09:50:30.000000 YMS-0.76/yamas/utilities.py
```

### Comparing `YMS-0.75/README.md` & `YMS-0.76/README.md`

 * *Files identical despite different names*

### Comparing `YMS-0.75/yamas/__init__.py` & `YMS-0.76/yamas/__init__.py`

 * *Files identical despite different names*

### Comparing `YMS-0.75/yamas/create_visualization.py` & `YMS-0.76/yamas/create_visualization.py`

 * *Files 19% similar despite different names*

```diff
@@ -134,19 +134,54 @@
     run_cmd([f"mkdir {export_path}"])
     final_output_path = os.path.join(export_path, f'{dataset_id}_final.txt')
     run_cmd([f"touch {final_output_path}"])
     args = []
     for fastq in tqdm([a for a in os.listdir(fastq_path) if a.split(".")[-1] == "fastq"]):
         input = os.path.join(fastq_path,fastq)
         output = os.path.join(os.path.join(reads_data.dir_path, 'qza'), f'{fastq}_profile.txt')
-        command = [f"metaphlan {input} --input_type fastq --nproc 1 > {output} "]
+        command = [f"metaphlan {input} --input_type fastq --nproc 16 > {output} "]
         run_cmd(command)
         args.append(output)
     merge(args, open(final_output_path, 'w'), gtdb=False)
+    # profiles = [os.listdir(os.path.join(reads_data.dir_path, 'qza'))
+    # merge(profiles)
 
+def metaphlan_txt_csv(reads_data, dataset_id):
+    export_path = os.path.join(reads_data.dir_path, "export")
+    input_file = os.path.join(export_path,f"{dataset_id}_final.txt")
+    data = []
+
+    with open(input_file, 'r') as file:
+        lines = file.readlines()
+
+        for line in lines:
+            line = line.strip()
+
+            if line.startswith('#') or line.startswith('SampleID') or line.startswith('clade_name'):
+                continue
+
+            fields = line.split('\t')
+
+            if len(fields) >= 4:
+                bacteria = fields[0]
+                relative_abundance = fields[2]
+                data.append([bacteria, relative_abundance])
+
+    total_abundance = sum(float(row[1]) for row in data)
+
+    for row in data:
+        relative_abundance = float(row[1])
+        percentage = (relative_abundance / total_abundance) * 100
+        row[1] = f'{percentage:.2f}%'
+    output_file = os.path.join(export_path, f'{dataset_id}_table.csv')
+    run_cmd([f"touch {output_file}"])
+    with open(output_file, 'w', newline='') as file:
+        writer = csv.writer(file)
+        writer.writerow(['Bacteria', 'Percentage'])
+        writer.writerows(data)
 
 def visualization(acc_list, dataset_id, data_type, verbose_print, specific_location):
     verbose_print("\n")
     verbose_print(datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S'))
     dir_name = f"{dataset_id}-{datetime.datetime.now().strftime('%d-%m-%Y_%H-%M-%S')}"
     verbose_print("Starting conversion to VIS file")
 
@@ -203,13 +238,17 @@
             print(f"Note: The data has only a forward read.\n"
                   f"Therefore, you must give the parameters 'trim' and 'trunc' of export() "
                   f"exactly one integers value which is related to the forward read.")
 
         return reads_data.dir_path
     else:
         verbose_print("\n")
-        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start metaphlan extraction (3/3)")
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start metaphlan extraction (3/4)")
         metaphlan_extraction(reads_data, dataset_id)
-        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish metaphlan extraction (3/3)")
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish metaphlan extraction (3/4)")
+        verbose_print("\n")
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Start metaphlan extraction (4/4)")
+        metaphlan_txt_csv(reads_data, dataset_id)
+        verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finish metaphlan extraction (4/4)")
         verbose_print(f"{datetime.datetime.now().strftime('%d/%m/%Y %H:%M:%S')} -- Finished downloading.\n")
```

### Comparing `YMS-0.75/yamas/dataset_downloading.py` & `YMS-0.76/yamas/dataset_downloading.py`

 * *Files identical despite different names*

### Comparing `YMS-0.75/yamas/export_data.py` & `YMS-0.76/yamas/export_data.py`

 * *Files identical despite different names*

### Comparing `YMS-0.75/yamas/utilities.py` & `YMS-0.76/yamas/utilities.py`

 * *Files identical despite different names*

