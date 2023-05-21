# Comparing `tmp/noise2read-0.0.99.tar.gz` & `tmp/noise2read-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noise2read-0.0.99.tar", last modified: Sat May 20 11:19:23 2023, max compression
+gzip compressed data, was "noise2read-0.1.0.tar", last modified: Sun May 21 07:25:03 2023, max compression
```

## Comparing `noise2read-0.0.99.tar` & `noise2read-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 11:19:23.204498 noise2read-0.0.99/
--rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.0.99/LICENSE
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-20 11:19:23.205778 noise2read-0.0.99/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.0.99/README.rst
--rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.0.99/pyproject.toml
--rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-20 11:19:23.209031 noise2read-0.0.99/setup.cfg
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 11:19:22.998820 noise2read-0.0.99/src/
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 11:19:23.115871 noise2read-0.0.99/src/noise2read/
--rw-r--r--   0 pping    (55472) Research  (5010)      182 2023-05-20 11:18:03.000000 noise2read-0.0.99/src/noise2read/__init__.py
--rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.0.99/src/noise2read/classifier.py
--rw-r--r--   0 pping    (55472) Research  (5010)    17347 2023-05-19 00:55:32.000000 noise2read-0.0.99/src/noise2read/config.py
--rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.0.99/src/noise2read/coverage.py
--rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.0.99/src/noise2read/data_analysis.py
--rw-r--r--   0 pping    (55472) Research  (5010)    56593 2023-05-20 11:17:32.000000 noise2read-0.0.99/src/noise2read/data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)    11534 2023-05-17 00:24:07.000000 noise2read-0.0.99/src/noise2read/data_preprocessing.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.0.99/src/noise2read/encoding.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30703 2023-05-18 23:59:43.000000 noise2read-0.0.99/src/noise2read/error_orrection.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.0.99/src/noise2read/isolates_correction.py
--rw-r--r--   0 pping    (55472) Research  (5010)    26351 2023-05-16 13:42:25.000000 noise2read-0.0.99/src/noise2read/noise2read.py
--rw-r--r--   0 pping    (55472) Research  (5010)    39127 2023-05-20 01:49:53.000000 noise2read-0.0.99/src/noise2read/reads2vectors.py
--rw-r--r--   0 pping    (55472) Research  (5010)    18547 2023-05-17 00:19:59.000000 noise2read-0.0.99/src/noise2read/simulation.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.0.99/src/noise2read/umitest.py
--rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.0.99/src/noise2read/utils.py
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 11:19:23.183814 noise2read-0.0.99/src/noise2read.egg-info/
--rw-r--r--   0 pping    (55472) Research  (5010)     5951 2023-05-20 11:19:22.000000 noise2read-0.0.99/src/noise2read.egg-info/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-20 11:19:22.000000 noise2read-0.0.99/src/noise2read.egg-info/SOURCES.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-20 11:19:22.000000 noise2read-0.0.99/src/noise2read.egg-info/dependency_links.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-20 11:19:22.000000 noise2read-0.0.99/src/noise2read.egg-info/entry_points.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.0.99/src/noise2read.egg-info/not-zip-safe
--rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-20 11:19:22.000000 noise2read-0.0.99/src/noise2read.egg-info/requires.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-20 11:19:22.000000 noise2read-0.0.99/src/noise2read.egg-info/top_level.txt
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-20 11:19:23.198973 noise2read-0.0.99/tests/
--rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.0.99/tests/test_data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.0.99/tests/test_reads2vector.py
--rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.0.99/tests/test_utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-21 07:25:03.836815 noise2read-0.1.0/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.1.0/LICENSE
+-rw-r--r--   0 pping    (55472) Research  (5010)     5950 2023-05-21 07:25:03.839256 noise2read-0.1.0/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.1.0/README.rst
+-rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.1.0/pyproject.toml
+-rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-21 07:25:03.846093 noise2read-0.1.0/setup.cfg
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-21 07:25:03.583385 noise2read-0.1.0/src/
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-21 07:25:03.735572 noise2read-0.1.0/src/noise2read/
+-rw-r--r--   0 pping    (55472) Research  (5010)      181 2023-05-21 00:25:03.000000 noise2read-0.1.0/src/noise2read/__init__.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.1.0/src/noise2read/classifier.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    17309 2023-05-21 04:58:20.000000 noise2read-0.1.0/src/noise2read/config.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.1.0/src/noise2read/coverage.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.1.0/src/noise2read/data_analysis.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    56606 2023-05-21 06:40:27.000000 noise2read-0.1.0/src/noise2read/data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    11566 2023-05-21 07:12:51.000000 noise2read-0.1.0/src/noise2read/data_preprocessing.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.1.0/src/noise2read/encoding.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30703 2023-05-18 23:59:43.000000 noise2read-0.1.0/src/noise2read/error_orrection.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.1.0/src/noise2read/isolates_correction.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    26118 2023-05-21 07:18:05.000000 noise2read-0.1.0/src/noise2read/noise2read.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    39127 2023-05-20 01:49:53.000000 noise2read-0.1.0/src/noise2read/reads2vectors.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    20359 2023-05-21 07:14:27.000000 noise2read-0.1.0/src/noise2read/simulation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.1.0/src/noise2read/umitest.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.1.0/src/noise2read/utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-21 07:25:03.799466 noise2read-0.1.0/src/noise2read.egg-info/
+-rw-r--r--   0 pping    (55472) Research  (5010)     5950 2023-05-21 07:25:03.000000 noise2read-0.1.0/src/noise2read.egg-info/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-21 07:25:03.000000 noise2read-0.1.0/src/noise2read.egg-info/SOURCES.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-21 07:25:03.000000 noise2read-0.1.0/src/noise2read.egg-info/dependency_links.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-21 07:25:03.000000 noise2read-0.1.0/src/noise2read.egg-info/entry_points.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.1.0/src/noise2read.egg-info/not-zip-safe
+-rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-21 07:25:03.000000 noise2read-0.1.0/src/noise2read.egg-info/requires.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-21 07:25:03.000000 noise2read-0.1.0/src/noise2read.egg-info/top_level.txt
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-21 07:25:03.829330 noise2read-0.1.0/tests/
+-rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.1.0/tests/test_data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.1.0/tests/test_reads2vector.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.1.0/tests/test_utils.py
```

### Comparing `noise2read-0.0.99/LICENSE` & `noise2read-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/PKG-INFO` & `noise2read-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.99
+Version: 0.1.0
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.99/README.rst` & `noise2read-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/setup.cfg` & `noise2read-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/src/noise2read/classifier.py` & `noise2read-0.1.0/src/noise2read/classifier.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/src/noise2read/config.py` & `noise2read-0.1.0/src/noise2read/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-19 10:56:38
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-19 10:55:32
+# @Last Modified time: 2023-05-21 14:58:20
 
 import configparser
 import os
 
 class Config(object):
     def __init__(self, config_file, logger):
         conf = configparser.ConfigParser()
@@ -269,30 +269,30 @@
             if conf.has_option("Simulation", "substations"):
                 self.substations = conf.getboolean("Simulation", "substations")
             else:
                 self.substations = True
             if conf.has_option("Simulation", "indels"):
                 self.indels = conf.getboolean("Simulation", "indels")
             else:
-                self.indels = True
+                self.indels = False
 
             if conf.has_option("Simulation", "error_rate1"):
                 self.error_rate1 = conf.getfloat("Simulation", "error_rate1")
             else:
                 self.error_rate1 = 0.03 # default
 
             if conf.has_option("Simulation", "error_rate2"):
                 self.error_rate2 = conf.getfloat("Simulation", "error_rate2")
             else:
                 self.error_rate2 = 0.005 # default
 
-            if conf.has_option("Simulation", "sim_random_state"):
-                self.sim_random_state = conf.getint("Simulation", "sim_random_state")
+            if conf.has_option("Simulation", "sim_seed"):
+                self.sim_seed = conf.getint("Simulation", "sim_seed")
             else:
-                self.sim_random_state = 42 # default
+                self.sim_seed = 42 # default
                 
             # # Evaluation
             # if conf.has_option("Evaluation", "delta"):
             #     self.delta = conf.getint("Evaluation", "delta")
             # else:
             #     self.delta = 10 # default
 
@@ -368,18 +368,18 @@
             self.amplicon_threshold_proba = 0.85
             # self.amplicon_error_node_degree = 4
 
             # simulation
             self.min_freq = 4
             self.min_read_count = 30
             self.substations = True
-            self.indels = True
+            self.indels = False
             self.error_rate1 = 0.03
             self.error_rate2 = 0.005
-            self.sim_random_state = 42
+            self.sim_seed = 42
 
             # # Evaluation
             # self.delta = 1
 
             # # coverage
             # self.library_layout = 'PE'
             # self.Alignment = '--local' # '--end-to-end'
```

### Comparing `noise2read-0.0.99/src/noise2read/coverage.py` & `noise2read-0.1.0/src/noise2read/coverage.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/src/noise2read/data_analysis.py` & `noise2read-0.1.0/src/noise2read/data_analysis.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/src/noise2read/data_generation.py` & `noise2read-0.1.0/src/noise2read/data_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-16 15:52:44
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-20 21:17:32
+# @Last Modified time: 2023-05-21 16:40:27
 
 import editdistance
 import networkx as nx
 import os
 import csv
 from tqdm import tqdm
 from noise2read.utils import *
@@ -40,18 +40,18 @@
                 config.high_ambiguous (bool, optional): If true, noise2read will predict high ambiguous errors. Defaults to False.
                 config.min_iters (int, optional): Minimum progress display update interval in iterations for the module tqdm. Defaults to 100.
                 config.verbose (bool, optional): If true, noise2read will save the genuine, ambiguous errors and negative reads to csv.
         """
         self.logger = logger
         self.config = config
         if os.path.exists(self.config.result_dir):
-            self.logger.warning("Directory '% s' already exists, noise2read will use it." % self.config.result_dir)
+            self.logger.warning("Directory '%s' already exists, noise2read will use it." % self.config.result_dir)
         else:
             os.makedirs(self.config.result_dir)
-            self.logger.info("Directory '% s' created" % self.config.result_dir)
+            self.logger.info("Directory '%s' created" % self.config.result_dir)
         
         self.file_type = parse_file_type(self.config.input_file)
         if ".gz" in self.file_type:
             self.out_file_tye = self.file_type.split(".gz")[0] 
         else:
             self.out_file_tye = self.file_type
 
@@ -205,15 +205,15 @@
         """
         extract genuine errors from umi graph
 
         Returns:
             DataFrame: one pandas dataframe saving genuine errors
         """
         graph, seqs_lens_lst, seqs2id_dict, unique_seqs = self.generate_graph(self.config.input_file, edit_dis=1)
-        subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph) ]#if len(c) >= 2
+        subgraphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph) if len(c) >= 2 ]#
 
         chunk_size = len(subgraphs) // self.config.chunks_num
         if chunk_size > 0:
             groups = [subgraphs[i:i+chunk_size] for i in range(0, len(subgraphs), chunk_size)]
         else:
             groups = subgraphs
 
@@ -234,25 +234,25 @@
             nx.write_gexf(group_G, file_name)
             gexf_files.append(file_name)
 
         del groups, subgraphs, graph
 
         genuine_lst = []
         for gexf_file in gexf_files:
-            graph = nx.read_gexf(gexf_file)
-            sub_graphs = [graph.subgraph(c).copy() for c in nx.connected_components(graph)]
+            cur_graph = nx.read_gexf(gexf_file)
+            sub_graphs = [cur_graph.subgraph(c).copy() for c in nx.connected_components(cur_graph)]
             
             subgraph_num = len(sub_graphs)
             with WorkerPool(self.config.num_workers, shared_objects=sub_graphs, start_method='fork') as pool:
                 cur_genuine_lsts = pool.imap(self.extract_umi_genuine_errs_subgraph, range(subgraph_num))
             for item in cur_genuine_lsts:
                 genuine_lst.extend(item)
 
             os.remove(gexf_file)
-            del graph, sub_graphs
+            del cur_graph, sub_graphs
 
         genuine_df = pd.DataFrame(genuine_lst, columns=["StartRead","StartReadCount", "StartDegree", "ErrorTye","ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"])
 
         if self.config.verbose:
             genuine_csv = os.path.join(self.config.result_dir, "umi_gnuine.csv")
             genuine_df.to_csv(genuine_csv, index=False) 
         return genuine_df
@@ -706,18 +706,18 @@
         # save graphs
         if self.config.graph_visualization or self.config.save_graph:
             if edit_dis == 1:
                 subdir = self.config.result_dir + "graph1/"                
             elif edit_dis == 2:
                 subdir = self.config.result_dir + "graph2/"
             if os.path.exists(subdir):
-                self.logger.info("Directory '% s' already exists" % subdir)
+                self.logger.info("Directory '%s' already exists" % subdir)
             else:
                 os.makedirs(subdir)
-                self.logger.info("Directory '% s' created" % subdir)
+                self.logger.info("Directory '%s' created" % subdir)
         if self.config.save_graph:
             graph_filename = subdir + 'graph.gexf'
             nx.write_gexf(graph, graph_filename)
             self.logger.info("Graph file *.gexf saved!")
         if self.config.graph_visualization:
             self.draw_graph(graph, subdir, self.config.drawing_graph_num)
             self.logger.info("Graph file *.png saved!")
```

### Comparing `noise2read-0.0.99/src/noise2read/data_preprocessing.py` & `noise2read-0.1.0/src/noise2read/data_preprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-17 10:24:07
+# @Last Modified time: 2023-05-21 17:12:51
 
 import collections
 from Bio import SeqIO
 from Bio.SeqRecord import SeqRecord
 import os
 from noise2read.utils import *
 from noise2read.data_generation import DataGneration
@@ -19,23 +19,23 @@
 class DataProcessing():
     # def __init__(self, logger, num_workers, output_dir, umi_start=None, umi_end=None, non_umi_start=None):
     def __init__(self, logger, config):
         self.logger = logger
         self.config = config
         
         if os.path.exists(self.config.result_dir):
-            self.logger.info("Directory '% s' already exists" % self.config.result_dir)
+            self.logger.info("Directory '%s' already exists" % self.config.result_dir)
         else:
             os.makedirs(self.config.result_dir)
         if os.path.exists(self.config.result_dir + 'raw/'):
-            self.logger.info("Directory '% s' already exists" % self.config.result_dir + 'raw/')
+            self.logger.info(f"Directory {self.config.result_dir}raw/ already exists")
         else:
             os.makedirs(self.config.result_dir + 'raw/')       
         if os.path.exists(self.config.result_dir + 'true/'):
-            self.logger.info("Directory '% s' already exists" % self.config.result_dir + 'true/')
+            self.logger.info(f"Directory {self.config.result_dir}true/ already exists")
         else:
             os.makedirs(self.config.result_dir + 'true/') 
                
     def extract_umis(self, original_data, umi_start, umi_end, non_umi_start):
         record_iterator, ff_type = parse_data(original_data) 
         self.logger.info("Read Data")
         umi_records = []
@@ -58,16 +58,16 @@
                 elif ff_type == "fasta":
                     umi_rec = SeqRecord(Seq(seq[umi_start:umi_end]), id=item.id, description=umi_desc)        
                     non_umi_rec = SeqRecord(Seq(seq[non_umi_start:]), id=item.id, description=non_umi_desc)  
                 umi_records.append(umi_rec)
                 non_umi_records.append(non_umi_rec)        
         self.logger.info("Rewrite umi and non-umi Data")
         raw_base_name = original_data.split('/')[-1]
-        umi_raw_dataset = self.output_dir + "umi_" + raw_base_name
-        non_umi_raw_dataset = self.output_dir + "non_umi_" + raw_base_name
+        umi_raw_dataset = self.config.result_dir + "umi_" + raw_base_name
+        non_umi_raw_dataset = self.config.result_dir + "umi_in_name_" + raw_base_name
         with open(umi_raw_dataset, "w") as handle:
             SeqIO.write(umi_records, handle, ff_type)        
         with open(non_umi_raw_dataset, "w") as handle:
             SeqIO.write(non_umi_records, handle, ff_type) 
         self.logger.info("Split umi and non-umis completed.") 
         return umi_raw_dataset, non_umi_raw_dataset
 
@@ -93,15 +93,15 @@
         genuine_df = DG.extract_umi_genuine_errs()
         # ##############################################################
         EC = ErrorCorrection(self.logger, self.config)
         # EC = ErrorCorrection(
         #     self.logger,
         #     self.num_workers,
         #     umi_raw_dataset,
-        #     self.output_dir,
+        #     self.config.result_dir,
         #     read_max_len = self.umi_end - self.umi_start,
         #     entropy_kmer=3, 
         #     entropy_q=2, 
         #     kmer_freq=3,
         #     read_type="DNA",
         #     iso_change_detail=False,
         #     min_iters=100)
@@ -162,16 +162,16 @@
                             # true_records.append(true_rec)
                             tmp_raw_rec.append(raw_rec)
                             tmp_true_rec.append(true_rec)
                     # if n >= 10:
                     raw_records.extend(tmp_raw_rec)
                     true_records.extend(tmp_true_rec)                    
         self.logger.info("Write raw and true data to file")
-        raw_file = self.output_dir + "raw/" + non_umi_f.split('/')[-1]
-        true_file = self.output_dir + "true/" + non_umi_f.split('/')[-1]
+        raw_file = self.config.result_dir + "raw/" + non_umi_f.split('/')[-1]
+        true_file = self.config.result_dir + "true/" + non_umi_f.split('/')[-1]
         with open(raw_file, "w") as handle:
             SeqIO.write(raw_records, handle, ori_file_type)        
         with open(true_file, "w") as handle:
             SeqIO.write(true_records, handle, ori_file_type) 
         self.logger.info("Real umi data processing completed.")                 
 
         return raw_file, true_file
@@ -208,16 +208,16 @@
             elif true_file_type == "fasta":
                 true_rec = SeqRecord(true_records_dict[name].seq, id=true_records_dict[name].id, description=true_des)        
                 raw_rec = SeqRecord(raw_records_dict[name].seq, id=raw_records_dict[name].id, description=raw_des)  
             raw_records.append(raw_rec)
             true_records.append(true_rec)
         raw_base_name = raw_dataset.split('/')[-1]
         true_base_name = true_dataset.split('/')[-1]
-        umi_raw_dataset = self.output_dir + "raw/" + "umi_" + raw_base_name
-        umi_true_dataset = self.output_dir + "true/" + "umi_"  + true_base_name
+        umi_raw_dataset = self.config.result_dir + "raw/" + "umi_" + raw_base_name
+        umi_true_dataset = self.config.result_dir + "true/" + "umi_"  + true_base_name
         self.logger.info("Rewrite Data")
         with open(umi_raw_dataset, "w") as handle:
             SeqIO.write(raw_records, handle, raw_file_type)        
         with open(umi_true_dataset, "w") as handle:
             SeqIO.write(true_records, handle, true_file_type) 
         self.logger.info("Mimic_umi preprocessing completed.") 
         return umi_raw_dataset, umi_true_dataset
```

### Comparing `noise2read-0.0.99/src/noise2read/encoding.py` & `noise2read-0.1.0/src/noise2read/encoding.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/src/noise2read/error_orrection.py` & `noise2read-0.1.0/src/noise2read/error_orrection.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/src/noise2read/isolates_correction.py` & `noise2read-0.1.0/src/noise2read/isolates_correction.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/src/noise2read/noise2read.py` & `noise2read-0.1.0/src/noise2read/noise2read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2022-12-29 23:04:12
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-16 23:42:25
+# @Last Modified time: 2023-05-21 17:18:05
 
 from noise2read.config import Config
 import sys, getopt
 from noise2read.data_generation import DataGneration
 from noise2read.error_orrection import ErrorCorrection
 from noise2read.data_analysis import DataAnalysis
 import os
@@ -316,21 +316,15 @@
 
                     if config.num_workers <= 0:
                         config.num_workers = available_cpu_cores
                     if config.num_workers > available_cpu_cores:
                         logger.error(f"Only {available_cpu_cores} available to use.") 
                         config.num_workers = available_cpu_cores
                 #############################################################
-                    DP = DataProcessing( 
-                        logger,
-                        config.num_workers,
-                        config.result_dir,
-                        config.umi_start,
-                        config.umi_end,
-                        config.non_umi_start)
+                    DP = DataProcessing(logger, config)
                     DP.write_mimic_umis(config.input_file, config.ground_truth_data)
 ############################################################################################################################
                 elif module_arg == "real_umi":   
                     if i_lst:
                         config = Config(None, logger)  
                         config.input_file = opts_dict[i_lst[0]]
                         if not os.path.exists(config.input_file):
```

### Comparing `noise2read-0.0.99/src/noise2read/reads2vectors.py` & `noise2read-0.1.0/src/noise2read/reads2vectors.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/src/noise2read/simulation.py` & `noise2read-0.1.0/src/noise2read/simulation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:04:45
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-17 10:19:59
+# @Last Modified time: 2023-05-21 17:14:27
 
 import collections
 from Bio import SeqIO
 # import gzip
 from Bio.SeqRecord import SeqRecord
 from Bio.Seq import Seq
 from tqdm import tqdm
@@ -118,16 +118,16 @@
                 raw_seq.insert(i, b)
                 editdis1_list.append(''.join(raw_seq))
         return set(editdis1_list)
         
     def read2err_read(self, read):
         possible_seqs = self.enumerate_ed1_seqs(read)
         num = len(possible_seqs)
-        # random.seed(self.config.indels)
-        random.shuffle(possible_seqs)
+        random.seed(self.config.sim_seed)
+        # random.shuffle(possible_seqs)
         idx = random.randint(0, num-1)
         return possible_seqs[idx]
 
     def error_correction(self, config):
         DG = DataGneration(self.logger, config)
         if config.high_ambiguous:
             isolates_file, non_isolates_file, unique_seqs, read_max_len, read_min_len, genuine_df, negative_df, ambiguous_df, high_ambiguous_df = DG.data_files(edit_dis=1)
@@ -153,16 +153,15 @@
         # step 1 correct errors using noise2read
         corrected_data = self.error_correction(self.config)
         # inject errors
         raw_data, true_data = self.error_injection(corrected_data)
         # raw_data, true_data = self.error_injection(self.config.input_file)
         DP = DataProcessing( 
             self.logger,
-            self.config.num_workers,
-            self.config.result_dir)
+            self.config)
         umi_raw_dataset, umi_true_dataset = DP.write_mimic_umis(raw_data, true_data)
         return umi_raw_dataset, umi_true_dataset
 
     def error_injection(self, data_set):
         records_dict, file_type = parse_data_dict(data_set)
         id_lst = list(records_dict.keys())
 
@@ -173,58 +172,67 @@
             seq2id_dict.setdefault(seq, []).append(item)
             total_seqs_lst.append(seq)
             # total_bases += len(seq)
             # total_reads += 1
 
         read2counts = collections.Counter(total_seqs_lst)
         select_id_lst = []
-        total_bases = 0
+        # total_bases = 0
         total_reads = 0
         new_read2counts = {}
         for read, count in read2counts.items():
             # if count >= 5:
-            if count > self.min_freq:
+            if count > self.config.min_freq:
                 select_id_lst.extend(seq2id_dict[read])
             if count > self.config.min_read_count:
                 new_read2counts[read] = count
                 total_reads += count
-                total_bases += len(read) * count
+                # total_bases += len(read) * count
                 
         # one base error
-        err_1_base_num = round(total_bases * self.config.error_rate1)
+        err_1_base_num = round(total_reads * self.config.error_rate1)
         if total_reads > err_1_base_num:
             per_num =  err_1_base_num / total_reads
-        err_1_id_lst = []
-        for read, count in new_read2counts.items():
-            random_num = round(count * per_num)
-            name_lst = seq2id_dict[read]
-            # random.shuffle(name_lst)
-            np.random.seed(self.config.sim_random_state)
-            indices = np.random.permutation(len(name_lst), size=random_num, replace=False)
-            err_1_id_lst.extend(name_lst[indices])
+            err_1_id_lst = []
+            for read, count in new_read2counts.items():
+                random_num = round(count * per_num)
+                name_lst = seq2id_dict[read]
+
+                rng = np.random.default_rng(seed=self.config.sim_seed)
+                indices = rng.permutation(len(name_lst))[:random_num]
+                # print(indices)
+                err_1_id_lst.extend(name_lst[i] for i in indices)
+                # print(err_1_id_lst)
+        else:
+            self.logger.error("1 base error reads number is larger than the total reads number!")
+            sys.exit(1)
 
         # two base errors
         if self.config.error_rate2 > 0:
             err_2_id_lst = []
-            err_2_base_num = round((total_bases-err_1_base_num) * self.config.error_rate2)
-
             cur_total_reads = total_reads - len(err_1_id_lst)
+            err_2_base_num = round(cur_total_reads * self.config.error_rate2)
+
             if cur_total_reads > err_2_base_num:
                 per_num_2base =  err_2_base_num / (cur_total_reads * 2)
-            for read, count in new_read2counts.items():
-                random_num_2base = round(count * per_num_2base)
-                cur_name_lst = list(set(seq2id_dict[read]) - set(err_1_id_lst))
-                # random.shuffle(name_lst)
-                np.random.seed(self.config.sim_random_state)
-                indices = np.random.permutation(len(cur_name_lst), size=random_num_2base, replace=False)
-                err_2_id_lst.extend(cur_name_lst[indices])
-            self.logger.info(f"total bases: {total_bases}, total reads: {total_reads}, 1 base error rate: {self.config.error_rate1}, 1 base error contained reads number: {len(err_1_id_lst)}, 2 bases error rate: {self.config.error_rate2}, 2 bases error contained reads number: {len(err_2_id_lst)}")
+                for read, count in new_read2counts.items():
+                    random_num_2base = round(count * per_num_2base)
+                    cur_name_lst = list(set(seq2id_dict[read]) - set(err_1_id_lst))
+
+                    rng = np.random.default_rng(seed=self.config.sim_seed)
+                    indices = rng.permutation(len(cur_name_lst))[:random_num_2base]
+                    err_2_id_lst.extend(cur_name_lst[i] for i in indices)
+                    
+                self.logger.info(f"Total reads: {total_reads}, 1 base error per read error rate: {self.config.error_rate1}, 1 base error reads number: {len(err_1_id_lst)}, 2 bases per read error rate: {self.config.error_rate2}, 2 bases error reads number: {len(err_2_id_lst)}")
+            else:
+                self.logger.error("2 bases error reads number is larger than the total reads number!")
+                sys.exit(1)
         else:
             # err_reads_num = round(total_bases * self.config.error_rate / total_reads)
-            self.logger.info(f"total bases: {total_bases}, total reads: {total_reads}, 1 base error rate: {self.config.error_rate1}, 1 base error contained reads number: {len(err_1_id_lst)}")
+            self.logger.info(f"Total reads: {total_reads}, 1 base error per read error rate: {self.config.error_rate1}, 1 base error reads number: {len(err_1_id_lst)}")
 
         err_1base_records = []
         shared_objects = records_dict, file_type
         with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
             for tmp_rec in pool.imap(self.mutate_seq, err_1_id_lst, progress_bar=self.config.verbose):
                 err_1base_records.append(tmp_rec)
 
@@ -253,19 +261,53 @@
         ##################################################################################
         err_free_subdataset_2 = self.config.result_dir + "err_free_subdataset2" + file_type
         extract_records(self.config.result_dir, err_id_lst, data_set, err_free_subdataset_2)
         true_data = self.config.result_dir + "simulated_true_" + file_name + file_type  
         os.system("cat %s %s > %s" % (err_free_subdataset_2, err_free_subdataset, true_data))     
         return raw_data, true_data
 
+    def find_first_diff_char(self, string1, string2):
+        min_len = min(len(string1), len(string2))
+
+        for i in range(min_len):
+            if string1[i] != string2[i]:
+                return i
+
+        # If all characters in the shorter string match the corresponding characters in the longer string
+        # and the shorter string is a prefix of the longer string, return the length of the shorter string
+        if len(string1) != len(string2):
+            return min_len
+
+        # If both strings are identical
+        return -1
+
     def mutate_seq(self, shared_objects, idx):
         records_dict, file_type = shared_objects
         ori_seq = str(records_dict[idx].seq)
         mutation_seq = self.read2err_read(ori_seq)
         if file_type == "fastq":
+            dis = editdistance.eval(ori_seq, mutation_seq)
+            if dis == 0:
+                pass
+            elif dis == 1:
+                indel_idx = self.find_first_diff_char(ori_seq, mutation_seq)
+                # Get the quality scores list from letter_annotations
+                quality_scores = records_dict[idx].letter_annotations["phred_quality"]
+                if len(ori_seq) < len(mutation_seq):
+                    # Calculate the average score
+                    min_score = min(quality_scores)
+                    # Insert the average score at the specified index
+                    quality_scores.insert(indel_idx, min_score)
+                    records_dict[idx].letter_annotations["phred_quality"] = quality_scores
+                elif len(ori_seq) > len(mutation_seq):
+                    quality_scores.pop(indel_idx)
+                    records_dict[idx].letter_annotations["phred_quality"] = quality_scores
+            else:
+                self.logger.error("Generate non 1-base error read.")
+                sys.exit(1)
             return SeqRecord(Seq(mutation_seq), id=records_dict[idx].id, description=records_dict[idx].description, letter_annotations=records_dict[idx].letter_annotations)
         elif file_type == "fasta":
             return SeqRecord(Seq(mutation_seq).seq, id=records_dict[idx].id, description=records_dict[idx].description)     
 
     def mutate_2base_seq(self, shared_objects, idx):
         records_dict, file_type = shared_objects
         ori_seq = str(records_dict[idx].seq)
@@ -274,26 +316,25 @@
             return SeqRecord(Seq(mutation_seq), id=records_dict[idx].id, description=records_dict[idx].description, letter_annotations=records_dict[idx].letter_annotations)
         elif file_type == "fasta":
             return SeqRecord(Seq(mutation_seq).seq, id=records_dict[idx].id, description=records_dict[idx].description)  
 
     def read2_2baseerr_read(self, read):
         possible_seqs = self.enumerate_ed2_seqs(read)
         num = len(possible_seqs)
-        # random.seed(self.config.indels)
-        random.shuffle(possible_seqs)
+        random.seed(self.config.sim_seed)
+        # random.shuffle(possible_seqs)
         idx = random.randint(0, num-1)
         return possible_seqs[idx]
 
-    def enumerate_ed2_seqs(read):
-        # possible_ed1 = self.enumerate_ed1_seqs(read)
+    def enumerate_ed2_seqs(self, read):
         possible_ed1 = seq2substitution(read)
         possible_ed2 = []
         for seq in possible_ed1:
             possible_ed2.extend(list(set(seq2substitution(seq)) - possible_ed1))
-        return set(possible_ed2)
+        return list(set(possible_ed2))
 
     '''
     def extract_seq(self, shared_objects, name):
         records_dict, file_type = shared_objects
         if file_type == "fastq":
             return SeqRecord(records_dict[name].seq, id=records_dict[name].id, description=records_dict[name].description, letter_annotations=records_dict[name].letter_annotations)
         elif file_type == "fasta":
```

### Comparing `noise2read-0.0.99/src/noise2read/umitest.py` & `noise2read-0.1.0/src/noise2read/umitest.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/src/noise2read/utils.py` & `noise2read-0.1.0/src/noise2read/utils.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/src/noise2read.egg-info/PKG-INFO` & `noise2read-0.1.0/src/noise2read.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.0.99
+Version: 0.1.0
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.0.99/src/noise2read.egg-info/SOURCES.txt` & `noise2read-0.1.0/src/noise2read.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/tests/test_data_generation.py` & `noise2read-0.1.0/tests/test_data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/tests/test_reads2vector.py` & `noise2read-0.1.0/tests/test_reads2vector.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.0.99/tests/test_utils.py` & `noise2read-0.1.0/tests/test_utils.py`

 * *Files identical despite different names*

