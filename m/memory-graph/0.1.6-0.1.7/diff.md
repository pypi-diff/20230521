# Comparing `tmp/memory_graph-0.1.6.tar.gz` & `tmp/memory_graph-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_graph-0.1.6.tar", last modified: Sat May 20 19:00:01 2023, max compression
+gzip compressed data, was "memory_graph-0.1.7.tar", last modified: Sun May 21 17:25:36 2023, max compression
```

## Comparing `memory_graph-0.1.6.tar` & `memory_graph-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 19:00:01.019402 memory_graph-0.1.6/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.6/LICENSE.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.6/MANIFEST.in
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4941 2023-05-20 19:00:01.019402 memory_graph-0.1.6/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4366 2023-05-20 18:13:48.000000 memory_graph-0.1.6/README.md
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 19:00:01.019402 memory_graph-0.1.6/memory_graph/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.6/memory_graph/Node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1190 2023-05-20 18:58:23.000000 memory_graph-0.1.6/memory_graph/__init__.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3696 2023-05-20 17:04:40.000000 memory_graph-0.1.6/memory_graph/graphviz_nodes.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4498 2023-05-20 18:49:23.000000 memory_graph-0.1.6/memory_graph/rewrite.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1142 2023-05-20 17:02:48.000000 memory_graph-0.1.6/memory_graph/rewrite_to_node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.6/memory_graph/rewrite_to_string.py
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-20 19:00:01.019402 memory_graph-0.1.6/memory_graph.egg-info/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4941 2023-05-20 19:00:01.000000 memory_graph-0.1.6/memory_graph.egg-info/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      388 2023-05-20 19:00:01.000000 memory_graph-0.1.6/memory_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-20 19:00:01.000000 memory_graph-0.1.6/memory_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-20 19:00:01.000000 memory_graph-0.1.6/memory_graph.egg-info/requires.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-20 19:00:01.000000 memory_graph-0.1.6/memory_graph.egg-info/top_level.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-20 19:00:01.019402 memory_graph-0.1.6/setup.cfg
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-20 18:58:32.000000 memory_graph-0.1.6/setup.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-21 17:25:36.443849 memory_graph-0.1.7/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.7/LICENSE.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.7/MANIFEST.in
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4941 2023-05-21 17:25:36.443849 memory_graph-0.1.7/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4366 2023-05-20 18:13:48.000000 memory_graph-0.1.7/README.md
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-21 17:25:36.443849 memory_graph-0.1.7/memory_graph/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.7/memory_graph/Node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1190 2023-05-21 17:24:25.000000 memory_graph-0.1.7/memory_graph/__init__.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5216 2023-05-21 17:18:14.000000 memory_graph-0.1.7/memory_graph/graphviz_nodes.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4498 2023-05-20 18:49:23.000000 memory_graph-0.1.7/memory_graph/rewrite.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1142 2023-05-20 17:02:48.000000 memory_graph-0.1.7/memory_graph/rewrite_to_node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.7/memory_graph/rewrite_to_string.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-21 17:25:36.443849 memory_graph-0.1.7/memory_graph.egg-info/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4941 2023-05-21 17:25:36.000000 memory_graph-0.1.7/memory_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      388 2023-05-21 17:25:36.000000 memory_graph-0.1.7/memory_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-21 17:25:36.000000 memory_graph-0.1.7/memory_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-21 17:25:36.000000 memory_graph-0.1.7/memory_graph.egg-info/requires.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-21 17:25:36.000000 memory_graph-0.1.7/memory_graph.egg-info/top_level.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-21 17:25:36.443849 memory_graph-0.1.7/setup.cfg
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-21 17:24:38.000000 memory_graph-0.1.7/setup.py
```

### Comparing `memory_graph-0.1.6/LICENSE.txt` & `memory_graph-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.6/PKG-INFO` & `memory_graph-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory_graph
-Version: 0.1.6
+Version: 0.1.7
 Summary: Draw a graph of your data to see the structure of its references.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `memory_graph-0.1.6/README.md` & `memory_graph-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.6/memory_graph/Node.py` & `memory_graph-0.1.7/memory_graph/Node.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.6/memory_graph/__init__.py` & `memory_graph-0.1.7/memory_graph/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from memory_graph import rewrite
 from memory_graph import Node
 from memory_graph import rewrite_to_node
 from memory_graph import graphviz_nodes
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 __author__ = 'Bas Terwijn'
 
 def create_graph(data):
     all_nodes=rewrite_to_node.rewrite_data(data)
     return graphviz_nodes.create_graph(all_nodes)
 
 def show(data,block=False):
```

### Comparing `memory_graph-0.1.6/memory_graph/rewrite.py` & `memory_graph-0.1.7/memory_graph/rewrite.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.6/memory_graph/rewrite_to_node.py` & `memory_graph-0.1.7/memory_graph/rewrite_to_node.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.6/memory_graph/rewrite_to_string.py` & `memory_graph-0.1.7/memory_graph/rewrite_to_string.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.6/memory_graph.egg-info/PKG-INFO` & `memory_graph-0.1.7/memory_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-graph
-Version: 0.1.6
+Version: 0.1.7
 Summary: Draw a graph of your data to see the structure of its references.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `memory_graph-0.1.6/setup.py` & `memory_graph-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description_from_readme = (this_directory / "README.md").read_text()
 
 setup(
     name = 'memory_graph',
-    version = '0.1.6',
+    version = '0.1.7',
     description = 'Draw a graph of your data to see the structure of its references.',
     long_description = long_description_from_readme,
     long_description_content_type = 'text/markdown',
     readme = 'README.md',
     url = 'https://github.com/bterwijn/memory_graph',
     author = 'Bas Terwijn',
     author_email = 'bterwijn@gmail.com',
```

