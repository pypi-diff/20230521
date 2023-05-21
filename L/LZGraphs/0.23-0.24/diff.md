# Comparing `tmp/LZGraphs-0.23.tar.gz` & `tmp/LZGraphs-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LZGraphs-0.23.tar", last modified: Tue Jan 17 13:09:17 2023, max compression
+gzip compressed data, was "LZGraphs-0.24.tar", last modified: Sun May 21 15:13:22 2023, max compression
```

## Comparing `LZGraphs-0.23.tar` & `LZGraphs-0.24.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-01-17 13:09:17.046453 LZGraphs-0.23/
--rw-rw-rw-   0        0        0     1079 2021-01-04 22:48:55.000000 LZGraphs-0.23/LICENSE
-drwxrwxrwx   0        0        0        0 2023-01-17 13:09:17.032784 LZGraphs-0.23/LZGraphs/
--rw-rw-rw-   0        0        0    27294 2023-01-16 14:08:57.000000 LZGraphs-0.23/LZGraphs/AminoAcidPositional.py
--rw-rw-rw-   0        0        0     4623 2023-01-17 13:07:44.000000 LZGraphs-0.23/LZGraphs/BOWEncoder.py
--rw-rw-rw-   0        0        0    34760 2023-01-16 09:36:36.000000 LZGraphs-0.23/LZGraphs/LZGraphBase.py
--rw-rw-rw-   0        0        0    27709 2022-11-18 08:20:03.000000 LZGraphs-0.23/LZGraphs/Naive.py
--rw-rw-rw-   0        0        0     6239 2023-01-17 10:12:21.000000 LZGraphs-0.23/LZGraphs/NodeEdgeSaturationProbe.py
--rw-rw-rw-   0        0        0    23786 2023-01-16 09:44:20.000000 LZGraphs-0.23/LZGraphs/NucleotideDoublePositional.py
--rw-rw-rw-   0        0        0     6934 2023-01-16 11:44:39.000000 LZGraphs-0.23/LZGraphs/Utilities.py
--rw-rw-rw-   0        0        0     6386 2023-01-12 07:25:58.000000 LZGraphs-0.23/LZGraphs/Visualize.py
--rw-rw-rw-   0        0        0      356 2023-01-17 13:03:13.000000 LZGraphs-0.23/LZGraphs/__init__.py
--rw-rw-rw-   0        0        0     1120 2023-01-15 16:46:30.000000 LZGraphs-0.23/LZGraphs/decomposition.py
--rw-rw-rw-   0        0        0     2378 2023-01-11 19:06:11.000000 LZGraphs-0.23/LZGraphs/misc.py
-drwxrwxrwx   0        0        0        0 2023-01-17 13:09:17.045957 LZGraphs-0.23/LZGraphs.egg-info/
--rw-rw-rw-   0        0        0     3988 2023-01-17 13:09:16.000000 LZGraphs-0.23/LZGraphs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2023-01-17 13:09:16.000000 LZGraphs-0.23/LZGraphs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-17 13:09:16.000000 LZGraphs-0.23/LZGraphs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-01-17 13:09:16.000000 LZGraphs-0.23/LZGraphs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-17 13:09:16.000000 LZGraphs-0.23/LZGraphs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2021-01-04 22:48:55.000000 LZGraphs-0.23/MANIFEST.in
--rw-rw-rw-   0        0        0     3988 2023-01-17 13:09:17.046949 LZGraphs-0.23/PKG-INFO
--rw-rw-rw-   0        0        0     3263 2023-01-17 11:28:03.000000 LZGraphs-0.23/README.md
--rw-rw-rw-   0        0        0       98 2021-01-04 22:48:55.000000 LZGraphs-0.23/pyproject.toml
--rw-rw-rw-   0        0        0      119 2023-01-17 13:09:17.047941 LZGraphs-0.23/setup.cfg
--rw-rw-rw-   0        0        0     1259 2023-01-17 13:09:08.000000 LZGraphs-0.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:13:22.636351 LZGraphs-0.24/
+-rw-rw-rw-   0        0        0     1079 2021-01-04 22:48:55.000000 LZGraphs-0.24/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-21 15:13:22.621471 LZGraphs-0.24/LZGraphs/
+-rw-rw-rw-   0        0        0    27294 2023-01-16 14:08:57.000000 LZGraphs-0.24/LZGraphs/AminoAcidPositional.py
+-rw-rw-rw-   0        0        0     4623 2023-01-17 13:07:44.000000 LZGraphs-0.24/LZGraphs/BOWEncoder.py
+-rw-rw-rw-   0        0        0    34791 2023-05-21 14:24:04.000000 LZGraphs-0.24/LZGraphs/LZGraphBase.py
+-rw-rw-rw-   0        0        0    28268 2023-05-21 08:25:24.000000 LZGraphs-0.24/LZGraphs/Naive.py
+-rw-rw-rw-   0        0        0     6615 2023-05-21 14:47:47.000000 LZGraphs-0.24/LZGraphs/NodeEdgeSaturationProbe.py
+-rw-rw-rw-   0        0        0    23781 2023-05-21 08:24:17.000000 LZGraphs-0.24/LZGraphs/NucleotideDoublePositional.py
+-rw-rw-rw-   0        0        0     6934 2023-01-16 11:44:39.000000 LZGraphs-0.24/LZGraphs/Utilities.py
+-rw-rw-rw-   0        0        0     6386 2023-01-12 07:25:58.000000 LZGraphs-0.24/LZGraphs/Visualize.py
+-rw-rw-rw-   0        0        0      356 2023-01-17 13:03:13.000000 LZGraphs-0.24/LZGraphs/__init__.py
+-rw-rw-rw-   0        0        0     1077 2023-05-17 13:52:35.000000 LZGraphs-0.24/LZGraphs/decomposition.py
+-rw-rw-rw-   0        0        0     2378 2023-01-11 19:06:11.000000 LZGraphs-0.24/LZGraphs/misc.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:13:22.635855 LZGraphs-0.24/LZGraphs.egg-info/
+-rw-rw-rw-   0        0        0     3939 2023-05-21 15:13:21.000000 LZGraphs-0.24/LZGraphs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2023-05-21 15:13:22.000000 LZGraphs-0.24/LZGraphs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 15:13:21.000000 LZGraphs-0.24/LZGraphs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-21 15:13:22.000000 LZGraphs-0.24/LZGraphs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-21 15:13:22.000000 LZGraphs-0.24/LZGraphs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2021-01-04 22:48:55.000000 LZGraphs-0.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     3939 2023-05-21 15:13:22.636351 LZGraphs-0.24/PKG-INFO
+-rw-rw-rw-   0        0        0     3263 2023-01-17 11:28:03.000000 LZGraphs-0.24/README.md
+-rw-rw-rw-   0        0        0       98 2021-01-04 22:48:55.000000 LZGraphs-0.24/pyproject.toml
+-rw-rw-rw-   0        0        0      119 2023-05-21 15:13:22.637342 LZGraphs-0.24/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2023-05-21 15:08:36.000000 LZGraphs-0.24/setup.py
```

### Comparing `LZGraphs-0.23/LICENSE` & `LZGraphs-0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.23/LZGraphs/AminoAcidPositional.py` & `LZGraphs-0.24/LZGraphs/AminoAcidPositional.py`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.23/LZGraphs/BOWEncoder.py` & `LZGraphs-0.24/LZGraphs/BOWEncoder.py`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.23/LZGraphs/LZGraphBase.py` & `LZGraphs-0.24/LZGraphs/LZGraphBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -688,16 +688,16 @@
         elif mode == 'max_product':
             return self._max_product_gene_prediction(walk, top_n=top_n)
         elif mode == 'sampling':
             return self._sampling_gene_prediction(walk, top_n=top_n)
         elif mode == 'full':
             return self._full_appearance_gene_prediction(walk, alpha)
 
-    def eigenvector_centrality(self):
-        return nx.algorithms.eigenvector_centrality(self.graph, weight='weight')
+    def eigenvector_centrality(self,max_iter=500):
+        return nx.algorithms.eigenvector_centrality(self.graph, weight='weight',max_iter=max_iter)
 
     def isolates(self):
         """
            A function that returns the list of all isolates in the graph.
            an isolate is a node that is connected to 0 edges (unseen sub-pattern).
 
                    Parameters:
```

### Comparing `LZGraphs-0.23/LZGraphs/Naive.py` & `LZGraphs-0.24/LZGraphs/Naive.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,14 +277,30 @@
     def nodes(self):
         return self.graph.nodes
 
     @property
     def edges(self):
         return self.graph.edges
 
+    @staticmethod
+    def encode_sequence(cdr3):
+        """
+              given a sequence of nucleotides this function will encode it into the following format:
+              {lz_subpattern}
+              matching the requirement of the NaiveLZGraph.
+
+
+                      Parameters:
+                              cdr3 (str): a string to encode into the NDPLZGraph format
+
+                      Returns:
+                              list : a list of unique sub-patterns in the NDPLZGraph format
+       """
+        return lempel_ziv_decomposition(cdr3)
+
     def __derive_terminal_state_map(self):
         """
             This function derives a mapping between each terminal state and all terminal state that could
             be reached from it
           """
         terminal_state_map = np.zeros((len(self.terminal_states), len(self.terminal_states)))
         for pos_1, terminal_1 in enumerate(self.terminal_states.index):
```

### Comparing `LZGraphs-0.23/LZGraphs/NodeEdgeSaturationProbe.py` & `LZGraphs-0.24/LZGraphs/NodeEdgeSaturationProbe.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,7 +143,14 @@
                 np.random.shuffle(sequence_list)
                 self.test_sequences(random.sample(sequence_list, sample_size), log_every, n)
                 # save logs
                 # reset aux
                 result.append(self.log_memory.copy())
                 self._reset()
         return result
+
+def get_k1000_diversity(list_of_sequences,lzgraph_encoding_function,draws=25):
+    # sample 1000 unique sequences
+    NESP = NodeEdgeSaturationProbe(node_function=lzgraph_encoding_function)
+    result = NESP.resampling_test(list(set(list_of_sequences)),n_tests=draws,sample_size=1000)
+    K_tests = [list(i.values())[-1]['nodes'] for i in result]
+    return np.mean(K_tests)
```

### Comparing `LZGraphs-0.23/LZGraphs/NucleotideDoublePositional.py` & `LZGraphs-0.24/LZGraphs/NucleotideDoublePositional.py`

 * *Files 0% similar despite different names*

```diff
@@ -483,15 +483,15 @@
         """
         given a sequence this function will return 2 list,
         the first is the lz-subpattern path through the graph and the second list is the number
         of possible choices that can be made at each sub-pattern
         :param cdr3_sample:
         :return:
         """
-        encoded = self.self.encode_sequence(cdr3_sample)
+        encoded = self.encode_sequence(cdr3_sample)
         curve = [self.graph.out_degree(i) for i in encoded]
         return encoded,curve
 
     def path_gene_table(self,cdr3_sample,threshold=None):
         """
         the function will return two tables of all possible v and j genes
             that colud be used to generate the sequence given by "cdr3_sample"
```

### Comparing `LZGraphs-0.23/LZGraphs/Utilities.py` & `LZGraphs-0.24/LZGraphs/Utilities.py`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.23/LZGraphs/Visualize.py` & `LZGraphs-0.24/LZGraphs/Visualize.py`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.23/LZGraphs/decomposition.py` & `LZGraphs-0.24/LZGraphs/decomposition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from collections import OrderedDict
 from typing import List
-from numba import jit
 
-#@jit(nopython=True)
 def lempel_ziv_decomposition(sequence:str) -> List[str]:
     """
           an implementation of the LZ76 compression algorithm,
           Given a string the function will return all unique sub-patterns derived from the input string
 
                   Args:
                           sequence (str): a string from which to derive sub-patterns
```

### Comparing `LZGraphs-0.23/LZGraphs/misc.py` & `LZGraphs-0.24/LZGraphs/misc.py`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.23/LZGraphs.egg-info/PKG-INFO` & `LZGraphs-0.24/LZGraphs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: LZGraphs
-Version: 0.23
+Version: 0.24
 Summary: An Implementation of LZ76 Based Graphs for Repertoire Representation
 Home-page: https://github.com/MuteJester/LZGraph
-Download-URL: https://github.com/MuteJester/LZGraphs/archive/refs/tags/V2.tar.gz
+Download-URL: https://github.com/MuteJester/LZGraphs/archive/refs/tags/V2.2.tar.gz
 Author: Thomas Konstantinovsky
 Author-email: thomaskon90@gmail.com
 License: MIT
 Keywords: Graph Theory,Immunology,analytics,biology,tcell,repertoire,cdr3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 .. raw:: html
 
    <p align="center">
```

### Comparing `LZGraphs-0.23/PKG-INFO` & `LZGraphs-0.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: LZGraphs
-Version: 0.23
+Version: 0.24
 Summary: An Implementation of LZ76 Based Graphs for Repertoire Representation
 Home-page: https://github.com/MuteJester/LZGraph
-Download-URL: https://github.com/MuteJester/LZGraphs/archive/refs/tags/V2.tar.gz
+Download-URL: https://github.com/MuteJester/LZGraphs/archive/refs/tags/V2.2.tar.gz
 Author: Thomas Konstantinovsky
 Author-email: thomaskon90@gmail.com
 License: MIT
 Keywords: Graph Theory,Immunology,analytics,biology,tcell,repertoire,cdr3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 .. raw:: html
 
    <p align="center">
```

### Comparing `LZGraphs-0.23/README.md` & `LZGraphs-0.24/README.md`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.23/setup.py` & `LZGraphs-0.24/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,31 +5,33 @@
 except ImportError:
     print("warning: pypandoc module not found, could not convert Markdown to RST")
     read_md = lambda f: open(f, 'r').read()
 
 setup(
   name = 'LZGraphs',
   packages = ['LZGraphs'],
-  version = '0.23',
+  version = '0.24',
   license='MIT',
   description='An Implementation of LZ76 Based Graphs for Repertoire Representation',
   long_description_content_type="text/markdown",
   long_description=read_md('README.md'),
   author = 'Thomas Konstantinovsky',
   author_email = 'thomaskon90@gmail.com',
   url='https://github.com/MuteJester/LZGraph',
-  download_url='https://github.com/MuteJester/LZGraphs/archive/refs/tags/V2.tar.gz',
+  download_url='https://github.com/MuteJester/LZGraphs/archive/refs/tags/V2.2.tar.gz',
   keywords = ['Graph Theory','Immunology',
               'analytics,biology','tcell','repertoire','cdr3'],   # Keywords that define your package best
     install_requires=[
         'tqdm',
-        'pandas'
+        'pandas',
+        'networkx==2.8.4',
+        'matplotlib==3.5.1',
+        'seaborn==0.12.1'
     ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Information Analysis',
     'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.8'
   ],
 )
```

