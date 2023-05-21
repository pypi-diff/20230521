# Comparing `tmp/sequana_rnaseq-0.9.8.tar.gz` & `tmp/sequana_rnaseq-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_rnaseq-0.9.8.tar", last modified: Tue Jan 28 12:34:32 2020, max compression
+gzip compressed data, was "dist/sequana_rnaseq-0.9.9.tar", last modified: Sat Feb  1 22:11:58 2020, max compression
```

## Comparing `sequana_rnaseq-0.9.8.tar` & `sequana_rnaseq-0.9.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      252 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/setup.cfg
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/sequana_rnaseq.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      902 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/sequana_rnaseq.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2019-12-02 16:35:02.000000 sequana_rnaseq-0.9.8/sequana_rnaseq.egg-info/not-zip-safe
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6542 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/sequana_rnaseq.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/sequana_rnaseq.egg-info/top_level.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/sequana_rnaseq.egg-info/dependency_links.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      133 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/sequana_rnaseq.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        8 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/sequana_rnaseq.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6542 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2799 2020-01-28 12:28:19.000000 sequana_rnaseq-0.9.8/setup.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/test/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1025 2020-01-28 12:30:05.000000 sequana_rnaseq-0.9.8/test/test_main.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/sequana_pipelines/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      111 2019-12-05 14:31:43.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/requirements.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5239 2020-01-22 17:07:12.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/schema.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4480 2019-12-23 13:33:04.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/multiqc_config.yaml
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)    71698 2019-12-03 16:49:42.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/dag.png
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/data/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)  1000897 2020-01-28 12:17:51.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/data/WT_R1_.mapped.fastq.gz
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2019-12-02 16:09:48.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/data/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)  1000897 2020-01-28 12:17:56.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/data/KO_R1_.mapped.fastq.gz
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-01-28 12:34:32.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/data/Saccer3/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2020-01-28 12:27:09.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/data/Saccer3/__init__.py
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      260 2019-12-02 19:46:22.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/cluster_config.json
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    22610 2020-01-27 22:27:16.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/rnaseq.rules
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     8174 2020-01-28 12:06:41.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/main.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      124 2020-01-28 11:02:07.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3519 2019-12-05 16:07:38.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/fastq_screen.conf
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    12222 2020-01-27 21:19:39.000000 sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4420 2020-01-28 12:28:33.000000 sequana_rnaseq-0.9.8/README.rst
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-02-01 22:11:58.000000 sequana_rnaseq-0.9.9/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      252 2020-02-01 22:11:58.000000 sequana_rnaseq-0.9.9/setup.cfg
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-02-01 22:11:58.000000 sequana_rnaseq-0.9.9/sequana_rnaseq.egg-info/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      902 2020-02-01 22:11:57.000000 sequana_rnaseq-0.9.9/sequana_rnaseq.egg-info/SOURCES.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2019-12-02 16:35:02.000000 sequana_rnaseq-0.9.9/sequana_rnaseq.egg-info/not-zip-safe
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6672 2020-02-01 22:11:57.000000 sequana_rnaseq-0.9.9/sequana_rnaseq.egg-info/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2020-02-01 22:11:57.000000 sequana_rnaseq-0.9.9/sequana_rnaseq.egg-info/top_level.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2020-02-01 22:11:57.000000 sequana_rnaseq-0.9.9/sequana_rnaseq.egg-info/dependency_links.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      133 2020-02-01 22:11:57.000000 sequana_rnaseq-0.9.9/sequana_rnaseq.egg-info/entry_points.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        8 2020-02-01 22:11:57.000000 sequana_rnaseq-0.9.9/sequana_rnaseq.egg-info/requires.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6672 2020-02-01 22:11:58.000000 sequana_rnaseq-0.9.9/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2799 2020-02-01 22:11:08.000000 sequana_rnaseq-0.9.9/setup.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-02-01 22:11:58.000000 sequana_rnaseq-0.9.9/test/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1025 2020-02-01 21:59:04.000000 sequana_rnaseq-0.9.9/test/test_main.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-02-01 22:11:57.000000 sequana_rnaseq-0.9.9/sequana_pipelines/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-02-01 22:11:57.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      111 2020-02-01 21:55:37.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/requirements.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5186 2020-02-01 21:58:35.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/schema.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4631 2020-02-01 16:18:21.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/multiqc_config.yaml
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)    71698 2019-12-03 16:49:42.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/dag.png
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-02-01 22:11:58.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/data/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)  1000897 2020-01-28 12:17:51.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/data/WT_R1_.mapped.fastq.gz
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2019-12-02 16:09:48.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/data/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)  1000897 2020-01-28 12:17:56.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/data/KO_R1_.mapped.fastq.gz
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-02-01 22:11:58.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/data/Saccer3/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2020-01-28 12:27:09.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/data/Saccer3/__init__.py
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      260 2019-12-02 19:46:22.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/cluster_config.json
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    23708 2020-02-01 21:55:03.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/rnaseq.rules
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     8488 2020-02-01 21:59:52.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/main.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      124 2020-01-28 11:02:07.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3519 2019-12-05 16:07:38.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/fastq_screen.conf
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    12309 2020-02-01 21:59:21.000000 sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/config.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4534 2020-02-01 22:10:37.000000 sequana_rnaseq-0.9.9/README.rst
```

### Comparing `sequana_rnaseq-0.9.8/sequana_rnaseq.egg-info/SOURCES.txt` & `sequana_rnaseq-0.9.9/sequana_rnaseq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sequana_rnaseq-0.9.8/sequana_rnaseq.egg-info/PKG-INFO` & `sequana_rnaseq-0.9.9/sequana_rnaseq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sequana-rnaseq
-Version: 0.9.8
+Version: 0.9.9
 Summary: A RNAseq pipeline from raw reads to feature counts
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -87,14 +87,16 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        0.9.9     * Fix RNAseQC rule, which is now available. 
+                  * Fix ability to use existing rRNA file as input
         0.9.8     * Fix indexing for bowtie1 to not be done if aligner is different
                   * add new options: --feature-counts-options and --do-rnaseq-qc,
                     --rRNA-feature
                   * Based on the input GFF, we now check the validity of the rRNA
                     feature and feature counts options to check whether the feature 
                     exists in the GFF
                   * schema is now used to check the config file values
```

### Comparing `sequana_rnaseq-0.9.8/PKG-INFO` & `sequana_rnaseq-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sequana_rnaseq
-Version: 0.9.8
+Version: 0.9.9
 Summary: A RNAseq pipeline from raw reads to feature counts
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -87,14 +87,16 @@
         
         Changelog
         ~~~~~~~~~
         
         ========= ====================================================================
         Version   Description
         ========= ====================================================================
+        0.9.9     * Fix RNAseQC rule, which is now available. 
+                  * Fix ability to use existing rRNA file as input
         0.9.8     * Fix indexing for bowtie1 to not be done if aligner is different
                   * add new options: --feature-counts-options and --do-rnaseq-qc,
                     --rRNA-feature
                   * Based on the input GFF, we now check the validity of the rRNA
                     feature and feature counts options to check whether the feature 
                     exists in the GFF
                   * schema is now used to check the config file values
```

### Comparing `sequana_rnaseq-0.9.8/setup.py` & `sequana_rnaseq-0.9.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # License: 3-clause BSD
 __revision__ = "$Id: $" # for the SVN Id
 from setuptools import setup, find_namespace_packages
 
 _MAJOR               = 0
 _MINOR               = 9
-_MICRO               = 8
+_MICRO               = 9
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 metainfo = {
     'authors': {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
     'version': version,
     'license' : 'new BSD',
```

### Comparing `sequana_rnaseq-0.9.8/test/test_main.py` & `sequana_rnaseq-0.9.9/test/test_main.py`

 * *Files identical despite different names*

### Comparing `sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/schema.yaml` & `sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/schema.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -187,23 +187,21 @@
     'igvtools':
         type: map
         mapping:
             "do":
                 type: bool
             "chrom_sizes_file":
                 type: str
-    'RNAseQC':
+    'rnaseqc2':
         type: map
         mapping:
             "do":
                 type: bool
             "gtf_file":
                 type: str
-            "BWArRNA_file":
-                type: str
             "options":
                 type: str
     'bowtie2_mapping_ref':
         type: map
         mapping:
             "options":
                 type: str
```

### Comparing `sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/multiqc_config.yaml` & `sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/multiqc_config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -43,238 +43,248 @@
 000002a0: 0a23 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .#--------------
 000002b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000002c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000002d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000002e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000002f0: 2d0a 0a23 2054 6974 6c65 2074 6f20 7573  -..# Title to us
 00000300: 6520 666f 7220 7468 6520 7265 706f 7274  e for the report
-00000310: 2e0a 7469 746c 653a 2022 5072 6f6a 6563  ..title: "Projec
-00000320: 7420 4e61 6d65 220a 7375 6274 6974 6c65  t Name".subtitle
-00000330: 3a20 2254 6974 7265 2064 6520 6c27 616e  : "Titre de l'an
-00000340: 616c 7973 6522 2020 2020 2020 2020 2020  alyse"          
-00000350: 2023 2047 7265 7920 7465 7874 2062 656c   # Grey text bel
-00000360: 6f77 2074 6974 6c65 0a69 6e74 726f 5f74  ow title.intro_t
-00000370: 6578 743a 2022 4d75 6c74 6951 4320 7265  ext: "MultiQC re
-00000380: 706f 7274 7320 7375 6d6d 6172 6973 6520  ports summarise 
-00000390: 616e 616c 7973 6973 2072 6573 756c 7473  analysis results
-000003a0: 2070 726f 6475 6365 6420 7769 7468 2052   produced with R
-000003b0: 4e41 2d73 6571 2073 6571 7561 6e61 2070  NA-seq sequana p
-000003c0: 6970 656c 696e 6520 2220 2020 2020 2020  ipeline "       
-000003d0: 2020 2023 2053 6574 2079 6f75 7220 6f77     # Set your ow
-000003e0: 6e20 7465 7874 0a0a 2320 4164 6420 6765  n text..# Add ge
-000003f0: 6e65 7269 6320 696e 666f 726d 6174 696f  neric informatio
-00000400: 6e20 746f 2074 6865 2074 6f70 206f 6620  n to the top of 
-00000410: 7265 706f 7274 730a 7265 706f 7274 5f68  reports.report_h
-00000420: 6561 6465 725f 696e 666f 3a0a 232d 2045  eader_info:.#- E
-00000430: 7861 6d70 6c65 2043 6f6e 6669 673a 3a20  xample Config:: 
-00000440: 2754 6869 7320 6973 2061 7262 6974 7261  'This is arbitra
-00000450: 7279 270a 232d 2041 6e6f 7468 6572 2066  ry'.#- Another f
-00000460: 6965 6c64 3a3a 2027 4c6f 6164 6564 2066  ield:: 'Loaded f
-00000470: 726f 6d20 3c63 6f64 653e 6d75 6c74 6971  rom <code>multiq
-00000480: 635f 636f 6e66 6967 5f65 7861 6d70 6c65  c_config_example
-00000490: 2e79 616d 6c3c 2f63 6f64 653e 270a 2020  .yaml</code>'.  
-000004a0: 2020 2d20 436f 6e74 6163 7420 452d 6d61    - Contact E-ma
-000004b0: 696c 3a20 273c 6c6f 6769 6e3e 4065 7861  il: '<login>@exa
-000004c0: 6d70 6c65 2e63 6f6d 270a 2020 2020 2d20  mple.com'.    - 
-000004d0: 4170 706c 6963 6174 696f 6e20 5479 7065  Application Type
-000004e0: 3a20 2753 7472 616e 6465 6420 524e 412d  : 'Stranded RNA-
-000004f0: 7365 7127 0a20 2020 202d 2050 726f 6a65  seq'.    - Proje
-00000500: 6374 2054 7970 653a 2027 4469 6666 6572  ct Type: 'Differ
-00000510: 656e 7469 616c 2067 656e 6520 6578 7072  ential gene expr
-00000520: 6573 7369 6f6e 270a 2020 2020 2d20 5365  ession'.    - Se
-00000530: 7175 656e 6369 6e67 2050 6c61 7466 6f72  quencing Platfor
-00000540: 6d3a 2027 4869 5365 7120 3235 3030 2048  m: 'HiSeq 2500 H
-00000550: 6967 6820 4f75 7470 7574 2056 3427 0a20  igh Output V4'. 
-00000560: 2020 202d 2053 6571 7565 6e63 696e 6720     - Sequencing 
-00000570: 5365 7475 703a 2027 5352 3635 270a 2020  Setup: 'SR65'.  
-00000580: 2020 2d20 4c69 6272 6172 7920 7479 7065    - Library type
-00000590: 203a 2027 496c 6c75 6d69 6e61 2054 7275   : 'Illumina Tru
-000005a0: 5365 7127 0a0a 232d 2d2d 2d2d 2d2d 2d2d  Seq'..#---------
-000005b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000005f0: 2d2d 2d2d 2d2d 0a0a 0a23 2053 7065 6369  ------...# Speci
-00000600: 6679 2061 2063 7573 746f 6d20 6c6f 676f  fy a custom logo
-00000610: 2074 6f20 6164 6420 746f 2072 6570 6f72   to add to repor
-00000620: 7473 2028 756e 636f 6d6d 656e 7420 746f  ts (uncomment to
-00000630: 2075 7365 290a 2363 7573 746f 6d5f 6c6f   use).#custom_lo
-00000640: 676f 3a20 2720 2020 2020 2020 2020 2320  go: '         # 
-00000650: 272f 7061 7468 2f74 6f2f 6c6f 676f 2e70  '/path/to/logo.p
-00000660: 6e67 270a 2363 7573 746f 6d5f 6c6f 676f  ng'.#custom_logo
-00000670: 5f75 726c 3a20 2727 2020 2020 2320 2768  _url: ''    # 'h
-00000680: 7474 7073 3a2f 2f77 7777 2e65 7861 6d70  ttps://www.examp
-00000690: 6c65 2e63 6f6d 270a 2363 7573 746f 6d5f  le.com'.#custom_
-000006a0: 6c6f 676f 5f74 6974 6c65 3a20 2727 2020  logo_title: ''  
-000006b0: 2320 274f 7572 2049 6e73 7469 7475 7465  # 'Our Institute
-000006c0: 204e 616d 6527 0a0a 0a0a 0a0a 2320 5072   Name'......# Pr
-000006d0: 6570 656e 6420 7361 6d70 6c65 206e 616d  epend sample nam
-000006e0: 6573 2077 6974 6820 7468 6569 7220 6469  es with their di
-000006f0: 7265 6374 6f72 792e 2055 7365 6675 6c20  rectory. Useful 
-00000700: 6966 2061 6e61 6c79 7369 6e67 2074 6865  if analysing the
-00000710: 0a23 2073 616d 706c 6520 7361 6d70 6c65  .# sample sample
-00000720: 7320 7769 7468 2064 6966 6665 7265 6e74  s with different
-00000730: 2070 6172 616d 6574 6572 732e 0a70 7265   parameters..pre
-00000740: 7065 6e64 5f64 6972 733a 2046 616c 7365  pend_dirs: False
-00000750: 0a0a 2320 4465 6661 756c 7420 6f75 7470  ..# Default outp
-00000760: 7574 2066 696c 656e 616d 6573 0a6f 7574  ut filenames.out
-00000770: 7075 745f 666e 5f6e 616d 653a 206d 756c  put_fn_name: mul
-00000780: 7469 7163 5f72 6570 6f72 742e 6874 6d6c  tiqc_report.html
-00000790: 0a64 6174 615f 6469 725f 6e61 6d65 3a20  .data_dir_name: 
-000007a0: 6d75 6c74 6971 635f 6461 7461 0a0a 2320  multiqc_data..# 
-000007b0: 5768 6574 6865 7220 746f 2063 7265 6174  Whether to creat
-000007c0: 6520 7468 6520 7061 7273 6564 2064 6174  e the parsed dat
-000007d0: 6120 6469 7265 6374 6f72 7920 696e 2061  a directory in a
-000007e0: 6464 6974 696f 6e20 746f 2074 6865 2072  ddition to the r
-000007f0: 6570 6f72 740a 6d61 6b65 5f64 6174 615f  eport.make_data_
-00000800: 6469 723a 2054 7275 650a 0a23 2043 6c65  dir: True..# Cle
-00000810: 616e 696e 6720 6f70 7469 6f6e 7320 666f  aning options fo
-00000820: 7220 7361 6d70 6c65 206e 616d 6573 2e20  r sample names. 
-00000830: 5479 7069 6361 6c6c 792c 2073 616d 706c  Typically, sampl
-00000840: 6520 6e61 6d65 7320 6172 6520 6465 7465  e names are dete
-00000850: 6374 6564 0a23 2066 726f 6d20 616e 2069  cted.# from an i
-00000860: 6e70 7574 2066 696c 656e 616d 652e 2049  nput filename. I
-00000870: 6620 616e 7920 6f66 2074 6865 7365 2073  f any of these s
-00000880: 7472 696e 6773 2061 7265 2066 6f75 6e64  trings are found
-00000890: 2c20 7468 6579 2061 6e64 2061 6e79 0a23  , they and any.#
-000008a0: 2074 6578 7420 746f 2074 6865 6972 2072   text to their r
-000008b0: 6967 6874 2077 696c 6c20 6265 2064 6973  ight will be dis
-000008c0: 6361 7264 6564 2e0a 2320 466f 7220 6578  carded..# For ex
-000008d0: 616d 706c 6520 2d20 6669 6c65 312e 6671  ample - file1.fq
-000008e0: 2e67 7a5f 7472 696d 6d65 642e 6261 6d5f  .gz_trimmed.bam_
-000008f0: 6465 6475 706c 6963 6174 6564 5f66 6173  deduplicated_fas
-00000900: 7471 632e 7a69 700a 2320 776f 756c 6420  tqc.zip.# would 
-00000910: 6265 2063 6c65 616e 6564 2074 6f20 2766  be cleaned to 'f
-00000920: 696c 6531 270a 2320 5477 6f20 6f70 7469  ile1'.# Two opti
-00000930: 6f6e 7320 6865 7265 202d 2066 6e5f 636c  ons here - fn_cl
-00000940: 6561 6e5f 6578 7473 2077 696c 6c20 7265  ean_exts will re
-00000950: 706c 6163 6520 7468 6520 6465 6661 756c  place the defaul
-00000960: 7473 2c0a 2320 6578 7472 615f 666e 5f63  ts,.# extra_fn_c
-00000970: 6c65 616e 5f65 7874 7320 7769 6c6c 2061  lean_exts will a
-00000980: 7070 656e 6420 746f 2074 6865 2064 6566  ppend to the def
-00000990: 6175 6c74 730a 6578 7472 615f 666e 5f63  aults.extra_fn_c
-000009a0: 6c65 616e 5f65 7874 733a 0a20 2020 202d  lean_exts:.    -
-000009b0: 202e 677a 0a20 2020 202d 202e 6661 7374   .gz.    - .fast
-000009c0: 710a 2020 2020 2d20 5f52 315f 2e63 7574  q.    - _R1_.cut
-000009d0: 6164 6170 740a 2020 2020 2d20 5f52 325f  adapt.    - _R2_
-000009e0: 2e63 7574 6164 6170 740a 2020 2020 2d20  .cutadapt.    - 
-000009f0: 5f52 325f 3030 310a 2020 2020 2d20 5f52  _R2_001.    - _R
-00000a00: 315f 3030 310a 2020 2020 2d20 2e65 7272  1_001.    - .err
-00000a10: 0a20 2020 202d 2074 7970 653a 2072 656d  .    - type: rem
-00000a20: 6f76 650a 2020 2020 2020 7061 7474 6572  ove.      patter
-00000a30: 6e3a 2027 2e73 6f72 7465 6427 0a20 2020  n: '.sorted'.   
-00000a40: 202d 2074 7970 653a 2072 6567 6578 0a20   - type: regex. 
-00000a50: 2020 2020 2070 6174 7465 726e 3a20 275e       pattern: '^
-00000a60: 5361 6d70 6c65 5f5c 642b 270a 0a0a 2320  Sample_\d+'...# 
-00000a70: 4967 6e6f 7265 2074 6865 7365 2066 696c  Ignore these fil
-00000a80: 6573 202f 2064 6972 6563 746f 7269 6573  es / directories
-00000a90: 202f 2070 6174 6873 2077 6865 6e20 7365   / paths when se
-00000aa0: 6172 6368 696e 6720 666f 7220 6c6f 6773  arching for logs
-00000ab0: 0a66 6e5f 6967 6e6f 7265 5f66 696c 6573  .fn_ignore_files
-00000ac0: 3a0a 2020 2020 2d20 2e44 535f 5374 6f72  :.    - .DS_Stor
-00000ad0: 650a 666e 5f69 676e 6f72 655f 6469 7273  e.fn_ignore_dirs
-00000ae0: 3a0a 2020 2020 2d20 616e 6e6f 7969 6e67  :.    - annoying
-00000af0: 5f64 6972 6e61 6d65 0a66 6e5f 6967 6e6f  _dirname.fn_igno
-00000b00: 7265 5f70 6174 6873 3a0a 2020 2020 2d20  re_paths:.    - 
-00000b10: 272a 2f70 6174 682f 746f 2f2a 5f66 696c  '*/path/to/*_fil
-00000b20: 6573 2f27 0a0a 2320 4967 6e6f 7265 2066  es/'..# Ignore f
-00000b30: 696c 6573 206c 6172 6765 7220 7468 616e  iles larger than
-00000b40: 2074 6869 7320 7768 656e 2073 6561 7263   this when searc
-00000b50: 696e 6720 666f 7220 6c6f 6773 2028 6279  ing for logs (by
-00000b60: 7465 7329 0a6c 6f67 5f66 696c 6573 697a  tes).log_filesiz
-00000b70: 655f 6c69 6d69 743a 2035 3030 3030 3030  e_limit: 5000000
-00000b80: 0a0a 2320 4d75 6c74 6951 4320 736b 6970  ..# MultiQC skip
-00000b90: 7320 6120 636f 7570 6c65 206f 6620 6465  s a couple of de
-00000ba0: 6275 6720 6d65 7373 6167 6573 2077 6865  bug messages whe
-00000bb0: 6e20 7365 6172 6368 696e 6720 6669 6c65  n searching file
-00000bc0: 7320 6173 2074 6865 0a23 206c 6f67 2063  s as the.# log c
-00000bd0: 616e 2067 6574 2076 6572 7920 7665 7262  an get very verb
-00000be0: 6f73 6520 6f74 6865 7277 6973 652e 2052  ose otherwise. R
-00000bf0: 652d 656e 6162 6c65 2068 6572 6520 746f  e-enable here to
-00000c00: 2068 656c 7020 6465 6275 6767 696e 672e   help debugging.
-00000c10: 0a72 6570 6f72 745f 7265 6164 6572 726f  .report_readerro
-00000c20: 7273 3a20 4661 6c73 650a 7265 706f 7274  rs: False.report
-00000c30: 5f69 6d67 736b 6970 733a 2046 616c 7365  _imgskips: False
-00000c40: 0a0a 2320 4f70 742d 6f75 7420 6f66 2072  ..# Opt-out of r
-00000c50: 656d 6f74 656c 7920 6368 6563 6b69 6e67  emotely checking
-00000c60: 2074 6861 7420 796f 7527 7265 2072 756e   that you're run
-00000c70: 6e69 6e67 2074 6865 206c 6174 6573 7420  ning the latest 
-00000c80: 7665 7273 696f 6e0a 6e6f 5f76 6572 7369  version.no_versi
-00000c90: 6f6e 5f63 6865 636b 3a20 4661 6c73 650a  on_check: False.
-00000ca0: 0a23 2048 6f77 2074 6f20 706c 6f74 2067  .# How to plot g
-00000cb0: 7261 7068 732e 2044 6966 6665 7265 6e74  raphs. Different
-00000cc0: 2074 656d 706c 6174 6573 2063 616e 206f   templates can o
-00000cd0: 7665 7272 6964 6520 7468 6573 6520 7365  verride these se
-00000ce0: 7474 696e 6773 2c20 6275 740a 2320 7468  ttings, but.# th
-00000cf0: 6520 6465 6661 756c 7420 7465 6d70 6c61  e default templa
-00000d00: 7465 2063 616e 2075 7365 2069 6e74 6572  te can use inter
-00000d10: 6163 7469 7665 2070 6c6f 7473 2028 4a61  active plots (Ja
-00000d20: 7661 7363 7269 7074 2075 7369 6e67 2048  vascript using H
-00000d30: 6967 6843 6861 7274 7329 0a23 206f 7220  ighCharts).# or 
-00000d40: 666c 6174 2070 6c6f 7473 2028 696d 6167  flat plots (imag
-00000d50: 6573 2c20 7573 696e 6720 4d61 7450 6c6f  es, using MatPlo
-00000d60: 744c 6962 292e 2057 6974 6820 696e 7465  tLib). With inte
-00000d70: 7261 6374 6976 6520 706c 6f74 732c 2074  ractive plots, t
-00000d80: 6865 2072 6570 6f72 740a 2320 6361 6e20  he report.# can 
-00000d90: 7072 6576 656e 7420 6175 746f 6d61 7469  prevent automati
-00000da0: 6361 6c6c 7920 7265 6e64 6572 696e 6720  cally rendering 
-00000db0: 616c 6c20 6772 6170 6873 2069 6620 7468  all graphs if th
-00000dc0: 6572 6520 6172 6520 6c6f 7473 206f 6620  ere are lots of 
-00000dd0: 7361 6d70 6c65 730a 2320 746f 2070 7265  samples.# to pre
-00000de0: 7665 6e74 2074 6865 2062 726f 7773 6572  vent the browser
-00000df0: 2062 6569 6e67 206c 6f63 6b65 6420 7570   being locked up
-00000e00: 2077 6865 6e20 7468 6520 7265 706f 7274   when the report
-00000e10: 206f 7065 6e73 2e0a 706c 6f74 735f 666f   opens..plots_fo
-00000e20: 7263 655f 666c 6174 3a20 4661 6c73 6520  rce_flat: False 
-00000e30: 2020 2020 2020 2020 2023 2054 7279 2074           # Try t
-00000e40: 6f20 7573 6520 6f6e 6c79 2066 6c61 7420  o use only flat 
-00000e50: 696d 6167 6520 6772 6170 6873 0a70 6c6f  image graphs.plo
-00000e60: 7473 5f66 6f72 6365 5f69 6e74 6572 6163  ts_force_interac
-00000e70: 7469 7665 3a20 4661 6c73 6520 2020 2320  tive: False   # 
-00000e80: 5472 7920 746f 2075 7365 206f 6e6c 7920  Try to use only 
-00000e90: 696e 7465 7261 6374 6976 6520 6a61 7661  interactive java
-00000ea0: 7363 7269 7074 2067 7261 7068 730a 706c  script graphs.pl
-00000eb0: 6f74 735f 666c 6174 5f6e 756d 7365 7269  ots_flat_numseri
-00000ec0: 6573 3a20 3130 3020 2020 2020 2020 2023  es: 100        #
-00000ed0: 2049 6620 6e65 6974 6865 7220 6f66 2074   If neither of t
-00000ee0: 6865 2061 626f 7665 2c20 7573 6520 666c  he above, use fl
-00000ef0: 6174 2069 6620 3e20 7468 6973 206e 756d  at if > this num
-00000f00: 6265 7220 6f66 2064 6174 6173 6574 730a  ber of datasets.
-00000f10: 6e75 6d5f 6461 7461 7365 7473 5f70 6c6f  num_datasets_plo
-00000f20: 745f 6c69 6d69 743a 2035 3020 2020 2020  t_limit: 50     
-00000f30: 2023 2049 6620 696e 7465 7261 6374 6976   # If interactiv
-00000f40: 652c 2064 6f6e 2774 2070 6c6f 7420 6f6e  e, don't plot on
-00000f50: 206c 6f61 6420 6966 203e 2074 6869 7320   load if > this 
-00000f60: 6e75 6d62 6572 206f 6620 6461 7461 7365  number of datase
-00000f70: 7473 0a6d 6178 5f74 6162 6c65 5f72 6f77  ts.max_table_row
-00000f80: 733a 2035 3030 2020 2020 2020 2020 2020  s: 500          
-00000f90: 2020 2020 2320 5377 6170 2074 6162 6c65      # Swap table
-00000fa0: 7320 666f 7220 6120 6265 6573 7761 726d  s for a beeswarm
-00000fb0: 2070 6c6f 7420 6162 6f76 6520 7468 6973   plot above this
-00000fc0: 0a0a 2320 4f76 6572 7772 6974 6520 6d6f  ..# Overwrite mo
-00000fd0: 6475 6c65 2066 696c 656e 616d 6520 7365  dule filename se
-00000fe0: 6172 6368 2070 6174 7465 726e 732e 2053  arch patterns. S
-00000ff0: 6565 206d 756c 7469 7163 2f75 7469 6c73  ee multiqc/utils
-00001000: 2f73 6561 7263 685f 7061 7474 6572 6e73  /search_patterns
-00001010: 2e79 616d 6c0a 2320 666f 7220 7468 6520  .yaml.# for the 
-00001020: 6465 6661 756c 7473 2e20 5265 6d6f 7665  defaults. Remove
-00001030: 2061 2064 6566 6175 6c74 2062 7920 7365   a default by se
-00001040: 7474 696e 6720 6974 2074 6f20 6e75 6c6c  tting it to null
-00001050: 2e0a 7370 3a0a 2020 2020 7374 6172 3a0a  ..sp:.    star:.
-00001060: 2020 2020 2020 2020 666e 3a20 272a 4c6f          fn: '*Lo
-00001070: 672e 6669 6e61 6c2e 6f75 7427 0a20 2020  g.final.out'.   
-00001080: 2074 7269 6d6d 6f6d 6174 6963 3a0a 2020   trimmomatic:.  
-00001090: 2020 2020 2020 636f 6e74 656e 7473 3a20        contents: 
-000010a0: 2754 7269 6d6d 6f6d 6174 6963 270a 2020  'Trimmomatic'.  
-000010b0: 2020 6375 7461 6461 7074 3a0a 2020 2020    cutadapt:.    
-000010c0: 2020 2020 666e 3a20 2763 7574 6164 6170      fn: 'cutadap
-000010d0: 742e 7478 7427 0a0a 0a0a 2320 4f76 6572  t.txt'....# Over
-000010e0: 7772 6974 6520 7468 6520 6465 6661 756c  write the defaul
-000010f0: 7473 206f 6620 7768 6963 6820 7461 626c  ts of which tabl
-00001100: 6520 636f 6c75 6d6e 7320 6172 6520 7669  e columns are vi
-00001110: 7369 626c 6520 6279 2064 6566 6175 6c74  sible by default
-00001120: 0a74 6162 6c65 5f63 6f6c 756d 6e73 5f76  .table_columns_v
-00001130: 6973 6962 6c65 3a0a 2020 2020 4661 7374  isible:.    Fast
-00001140: 5143 3a0a 2020 2020 2020 2020 7065 7263  QC:.        perc
-00001150: 656e 745f 6661 696c 733a 2046 616c 7365  ent_fails: False
-00001160: 0a20 2020 2020 2020 2074 6f74 616c 5f73  .        total_s
-00001170: 6571 7565 6e63 6573 3a20 5472 7565 0a0a  equences: True..
+00000310: 2e0a 7469 746c 653a 2022 4258 5858 220a  ..title: "BXXX".
+00000320: 7375 6274 6974 6c65 3a20 2252 4e41 2d73  subtitle: "RNA-s
+00000330: 6571 2061 6e61 6c79 7369 7322 200a 696e  eq analysis" .in
+00000340: 7472 6f5f 7465 7874 3a20 2252 6570 6f72  tro_text: "Repor
+00000350: 7420 7375 6d6d 6172 6973 696e 6720 636c  t summarising cl
+00000360: 6561 6e69 6e67 2028 6375 7461 6461 7074  eaning (cutadapt
+00000370: 2073 6563 7469 6f6e 2920 616e 6420 6d61   section) and ma
+00000380: 7070 696e 6720 2873 7461 742f 626f 7774  pping (stat/bowt
+00000390: 6965 2073 6563 7469 6f6e 7329 206f 6620  ie sections) of 
+000003a0: 796f 7572 2046 6173 7451 2066 696c 6573  your FastQ files
+000003b0: 2c20 6173 2077 656c 6c20 6173 2066 6561  , as well as fea
+000003c0: 7475 7265 2063 6f75 6e74 7320 2866 6561  ture counts (fea
+000003d0: 7475 7265 436f 756e 7473 2073 6563 7469  tureCounts secti
+000003e0: 6f6e 2920 616e 6420 7175 6963 6b20 636f  on) and quick co
+000003f0: 6e74 616d 696e 616e 7420 7365 6172 6368  ntaminant search
+00000400: 2028 6661 7374 7120 7363 7265 656e 2073   (fastq screen s
+00000410: 6563 7469 6f6e 2922 0a0a 2320 4164 6420  ection)"..# Add 
+00000420: 6765 6e65 7269 6320 696e 666f 726d 6174  generic informat
+00000430: 696f 6e20 746f 2074 6865 2074 6f70 206f  ion to the top o
+00000440: 6620 7265 706f 7274 730a 7265 706f 7274  f reports.report
+00000450: 5f68 6561 6465 725f 696e 666f 3a0a 2020  _header_info:.  
+00000460: 202d 2041 7574 686f 7273 3a20 273c 6120   - Authors: '<a 
+00000470: 6872 6566 3d22 6874 7470 3a2f 2f67 6974  href="http://git
+00000480: 6875 622e 636f 6d2f 7365 7175 616e 612f  hub.com/sequana/
+00000490: 7365 7175 616e 6122 3e53 6571 7561 6e61  sequana">Sequana
+000004a0: 2064 6576 656c 6f70 6572 733c 2f61 3e27   developers</a>'
+000004b0: 0a20 2020 2d20 5761 6e74 2074 6f20 6b6e  .   - Want to kn
+000004c0: 6f77 206d 6f72 653f 3a20 2753 6565 2074  ow more?: 'See t
+000004d0: 6865 203c 6120 6872 6566 3d22 6874 7470  he <a href="http
+000004e0: 3a2f 2f73 6571 7561 6e61 2e72 6561 6474  ://sequana.readt
+000004f0: 6865 646f 6373 2e69 6f22 2074 6172 6765  hedocs.io" targe
+00000500: 743d 225f 626c 616e 6b22 3e53 6571 7561  t="_blank">Sequa
+00000510: 6e61 3c2f 613e 2061 6e64 203c 6120 6872  na</a> and <a hr
+00000520: 6566 3d22 6874 7470 3a2f 2f67 6974 6875  ef="http://githu
+00000530: 622e 636f 6d2f 7365 7175 616e 612f 7365  b.com/sequana/se
+00000540: 7175 616e 615f 726e 6173 6571 2f22 2074  quana_rnaseq/" t
+00000550: 6172 6765 743d 225f 626c 616e 6b22 3e20  arget="_blank"> 
+00000560: 7365 7175 616e 615f 726e 6173 6571 2070  sequana_rnaseq p
+00000570: 6970 656c 696e 653c 2f61 3e20 646f 6375  ipeline</a> docu
+00000580: 6d65 6e74 6174 696f 6e2e 270a 2020 202d  mentation.'.   -
+00000590: 2043 6974 6174 696f 6e73 3a20 2749 6620   Citations: 'If 
+000005a0: 796f 7520 7573 6564 2053 6571 7561 6e69  you used Sequani
+000005b0: 782c 2053 6571 7561 6e61 2c20 5365 7175  x, Sequana, Sequ
+000005c0: 616e 615f 636f 7665 7261 6765 2074 6f6f  ana_coverage too
+000005d0: 6c2c 206f 7220 616e 7920 5365 7175 616e  l, or any Sequan
+000005e0: 6120 7069 7065 6c69 6e65 732c 2070 6c65  a pipelines, ple
+000005f0: 6173 6520 7365 6520 3c61 2068 7265 663d  ase see <a href=
+00000600: 2268 7474 703a 2f20 2020 202f 7365 7175  "http:/    /sequ
+00000610: 616e 612e 7265 6164 7468 6564 6f63 732e  ana.readthedocs.
+00000620: 696f 223e 486f 7720 746f 2063 6974 6520  io">How to cite 
+00000630: 3f3c 2f61 3e20 7365 6374 696f 6e2e 2049  ?</a> section. I
+00000640: 6e20 7061 7274 6963 756c 6172 2c20 6966  n particular, if
+00000650: 2079 6f75 2075 7365 2074 6869 7320 7265   you use this re
+00000660: 706f 7274 2069 6e20 6120 7075 626c 6963  port in a public
+00000670: 6174 696f 6e2c 2070 6c65 6173 6520 6369  ation, please ci
+00000680: 7465 2053 6571 7561 6e61 2e27 0a20 2020  te Sequana.'.   
+00000690: 2d20 436f 6e74 6163 7420 452d 6d61 696c  - Contact E-mail
+000006a0: 3a20 2727 0a23 2020 202d 2050 726f 6a65  : ''.#   - Proje
+000006b0: 6374 2054 7970 653a 2027 4469 6666 6572  ct Type: 'Differ
+000006c0: 656e 7469 616c 2067 656e 6520 6578 7072  ential gene expr
+000006d0: 6573 7369 6f6e 270a 0a0a 232d 2d2d 2d2d  ession'...#-----
+000006e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000006f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000720: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 0a0a 2320  ----------....# 
+00000730: 5072 6570 656e 6420 7361 6d70 6c65 206e  Prepend sample n
+00000740: 616d 6573 2077 6974 6820 7468 6569 7220  ames with their 
+00000750: 6469 7265 6374 6f72 792e 2055 7365 6675  directory. Usefu
+00000760: 6c20 6966 2061 6e61 6c79 7369 6e67 2074  l if analysing t
+00000770: 6865 0a23 2073 616d 706c 6520 7361 6d70  he.# sample samp
+00000780: 6c65 7320 7769 7468 2064 6966 6665 7265  les with differe
+00000790: 6e74 2070 6172 616d 6574 6572 732e 0a70  nt parameters..p
+000007a0: 7265 7065 6e64 5f64 6972 733a 2046 616c  repend_dirs: Fal
+000007b0: 7365 0a0a 2320 4465 6661 756c 7420 6f75  se..# Default ou
+000007c0: 7470 7574 2066 696c 656e 616d 6573 0a6f  tput filenames.o
+000007d0: 7574 7075 745f 666e 5f6e 616d 653a 206d  utput_fn_name: m
+000007e0: 756c 7469 7163 5f72 6570 6f72 742e 6874  ultiqc_report.ht
+000007f0: 6d6c 0a64 6174 615f 6469 725f 6e61 6d65  ml.data_dir_name
+00000800: 3a20 6d75 6c74 6971 635f 6461 7461 0a0a  : multiqc_data..
+00000810: 2320 5768 6574 6865 7220 746f 2063 7265  # Whether to cre
+00000820: 6174 6520 7468 6520 7061 7273 6564 2064  ate the parsed d
+00000830: 6174 6120 6469 7265 6374 6f72 7920 696e  ata directory in
+00000840: 2061 6464 6974 696f 6e20 746f 2074 6865   addition to the
+00000850: 2072 6570 6f72 740a 6d61 6b65 5f64 6174   report.make_dat
+00000860: 615f 6469 723a 2054 7275 650a 0a23 2043  a_dir: True..# C
+00000870: 6c65 616e 696e 6720 6f70 7469 6f6e 7320  leaning options 
+00000880: 666f 7220 7361 6d70 6c65 206e 616d 6573  for sample names
+00000890: 2e20 5479 7069 6361 6c6c 792c 2073 616d  . Typically, sam
+000008a0: 706c 6520 6e61 6d65 7320 6172 6520 6465  ple names are de
+000008b0: 7465 6374 6564 0a23 2066 726f 6d20 616e  tected.# from an
+000008c0: 2069 6e70 7574 2066 696c 656e 616d 652e   input filename.
+000008d0: 2049 6620 616e 7920 6f66 2074 6865 7365   If any of these
+000008e0: 2073 7472 696e 6773 2061 7265 2066 6f75   strings are fou
+000008f0: 6e64 2c20 7468 6579 2061 6e64 2061 6e79  nd, they and any
+00000900: 0a23 2074 6578 7420 746f 2074 6865 6972  .# text to their
+00000910: 2072 6967 6874 2077 696c 6c20 6265 2064   right will be d
+00000920: 6973 6361 7264 6564 2e0a 2320 466f 7220  iscarded..# For 
+00000930: 6578 616d 706c 6520 2d20 6669 6c65 312e  example - file1.
+00000940: 6671 2e67 7a5f 7472 696d 6d65 642e 6261  fq.gz_trimmed.ba
+00000950: 6d5f 6465 6475 706c 6963 6174 6564 5f66  m_deduplicated_f
+00000960: 6173 7471 632e 7a69 700a 2320 776f 756c  astqc.zip.# woul
+00000970: 6420 6265 2063 6c65 616e 6564 2074 6f20  d be cleaned to 
+00000980: 2766 696c 6531 270a 2320 5477 6f20 6f70  'file1'.# Two op
+00000990: 7469 6f6e 7320 6865 7265 202d 2066 6e5f  tions here - fn_
+000009a0: 636c 6561 6e5f 6578 7473 2077 696c 6c20  clean_exts will 
+000009b0: 7265 706c 6163 6520 7468 6520 6465 6661  replace the defa
+000009c0: 756c 7473 2c0a 2320 6578 7472 615f 666e  ults,.# extra_fn
+000009d0: 5f63 6c65 616e 5f65 7874 7320 7769 6c6c  _clean_exts will
+000009e0: 2061 7070 656e 6420 746f 2074 6865 2064   append to the d
+000009f0: 6566 6175 6c74 730a 6578 7472 615f 666e  efaults.extra_fn
+00000a00: 5f63 6c65 616e 5f65 7874 733a 0a20 2020  _clean_exts:.   
+00000a10: 202d 202e 677a 0a20 2020 202d 202e 6661   - .gz.    - .fa
+00000a20: 7374 710a 2020 2020 2d20 5f52 315f 2e63  stq.    - _R1_.c
+00000a30: 7574 6164 6170 740a 2020 2020 2d20 5f52  utadapt.    - _R
+00000a40: 325f 2e63 7574 6164 6170 740a 2020 2020  2_.cutadapt.    
+00000a50: 2d20 5f52 325f 3030 310a 2020 2020 2d20  - _R2_001.    - 
+00000a60: 5f52 315f 3030 310a 2020 2020 2d20 2e65  _R1_001.    - .e
+00000a70: 7272 0a20 2020 202d 2074 7970 653a 2072  rr.    - type: r
+00000a80: 656d 6f76 650a 2020 2020 2020 7061 7474  emove.      patt
+00000a90: 6572 6e3a 2027 2e73 6f72 7465 6427 0a20  ern: '.sorted'. 
+00000aa0: 2020 202d 2074 7970 653a 2072 6567 6578     - type: regex
+00000ab0: 0a20 2020 2020 2070 6174 7465 726e 3a20  .      pattern: 
+00000ac0: 275e 5361 6d70 6c65 5f5c 642b 270a 0a0a  '^Sample_\d+'...
+00000ad0: 2320 4967 6e6f 7265 2074 6865 7365 2066  # Ignore these f
+00000ae0: 696c 6573 202f 2064 6972 6563 746f 7269  iles / directori
+00000af0: 6573 202f 2070 6174 6873 2077 6865 6e20  es / paths when 
+00000b00: 7365 6172 6368 696e 6720 666f 7220 6c6f  searching for lo
+00000b10: 6773 0a66 6e5f 6967 6e6f 7265 5f66 696c  gs.fn_ignore_fil
+00000b20: 6573 3a0a 2020 2020 2d20 2e44 535f 5374  es:.    - .DS_St
+00000b30: 6f72 650a 666e 5f69 676e 6f72 655f 6469  ore.fn_ignore_di
+00000b40: 7273 3a0a 2020 2020 2d20 616e 6e6f 7969  rs:.    - annoyi
+00000b50: 6e67 5f64 6972 6e61 6d65 0a66 6e5f 6967  ng_dirname.fn_ig
+00000b60: 6e6f 7265 5f70 6174 6873 3a0a 2020 2020  nore_paths:.    
+00000b70: 2d20 272a 2f70 6174 682f 746f 2f2a 5f66  - '*/path/to/*_f
+00000b80: 696c 6573 2f27 0a0a 2320 4967 6e6f 7265  iles/'..# Ignore
+00000b90: 2066 696c 6573 206c 6172 6765 7220 7468   files larger th
+00000ba0: 616e 2074 6869 7320 7768 656e 2073 6561  an this when sea
+00000bb0: 7263 696e 6720 666f 7220 6c6f 6773 2028  rcing for logs (
+00000bc0: 6279 7465 7329 0a6c 6f67 5f66 696c 6573  bytes).log_files
+00000bd0: 697a 655f 6c69 6d69 743a 2035 3030 3030  ize_limit: 50000
+00000be0: 3030 0a0a 2320 4d75 6c74 6951 4320 736b  00..# MultiQC sk
+00000bf0: 6970 7320 6120 636f 7570 6c65 206f 6620  ips a couple of 
+00000c00: 6465 6275 6720 6d65 7373 6167 6573 2077  debug messages w
+00000c10: 6865 6e20 7365 6172 6368 696e 6720 6669  hen searching fi
+00000c20: 6c65 7320 6173 2074 6865 0a23 206c 6f67  les as the.# log
+00000c30: 2063 616e 2067 6574 2076 6572 7920 7665   can get very ve
+00000c40: 7262 6f73 6520 6f74 6865 7277 6973 652e  rbose otherwise.
+00000c50: 2052 652d 656e 6162 6c65 2068 6572 6520   Re-enable here 
+00000c60: 746f 2068 656c 7020 6465 6275 6767 696e  to help debuggin
+00000c70: 672e 0a72 6570 6f72 745f 7265 6164 6572  g..report_reader
+00000c80: 726f 7273 3a20 4661 6c73 650a 7265 706f  rors: False.repo
+00000c90: 7274 5f69 6d67 736b 6970 733a 2046 616c  rt_imgskips: Fal
+00000ca0: 7365 0a0a 2320 4f70 742d 6f75 7420 6f66  se..# Opt-out of
+00000cb0: 2072 656d 6f74 656c 7920 6368 6563 6b69   remotely checki
+00000cc0: 6e67 2074 6861 7420 796f 7527 7265 2072  ng that you're r
+00000cd0: 756e 6e69 6e67 2074 6865 206c 6174 6573  unning the lates
+00000ce0: 7420 7665 7273 696f 6e0a 6e6f 5f76 6572  t version.no_ver
+00000cf0: 7369 6f6e 5f63 6865 636b 3a20 4661 6c73  sion_check: Fals
+00000d00: 650a 0a23 2048 6f77 2074 6f20 706c 6f74  e..# How to plot
+00000d10: 2067 7261 7068 732e 2044 6966 6665 7265   graphs. Differe
+00000d20: 6e74 2074 656d 706c 6174 6573 2063 616e  nt templates can
+00000d30: 206f 7665 7272 6964 6520 7468 6573 6520   override these 
+00000d40: 7365 7474 696e 6773 2c20 6275 740a 2320  settings, but.# 
+00000d50: 7468 6520 6465 6661 756c 7420 7465 6d70  the default temp
+00000d60: 6c61 7465 2063 616e 2075 7365 2069 6e74  late can use int
+00000d70: 6572 6163 7469 7665 2070 6c6f 7473 2028  eractive plots (
+00000d80: 4a61 7661 7363 7269 7074 2075 7369 6e67  Javascript using
+00000d90: 2048 6967 6843 6861 7274 7329 0a23 206f   HighCharts).# o
+00000da0: 7220 666c 6174 2070 6c6f 7473 2028 696d  r flat plots (im
+00000db0: 6167 6573 2c20 7573 696e 6720 4d61 7450  ages, using MatP
+00000dc0: 6c6f 744c 6962 292e 2057 6974 6820 696e  lotLib). With in
+00000dd0: 7465 7261 6374 6976 6520 706c 6f74 732c  teractive plots,
+00000de0: 2074 6865 2072 6570 6f72 740a 2320 6361   the report.# ca
+00000df0: 6e20 7072 6576 656e 7420 6175 746f 6d61  n prevent automa
+00000e00: 7469 6361 6c6c 7920 7265 6e64 6572 696e  tically renderin
+00000e10: 6720 616c 6c20 6772 6170 6873 2069 6620  g all graphs if 
+00000e20: 7468 6572 6520 6172 6520 6c6f 7473 206f  there are lots o
+00000e30: 6620 7361 6d70 6c65 730a 2320 746f 2070  f samples.# to p
+00000e40: 7265 7665 6e74 2074 6865 2062 726f 7773  revent the brows
+00000e50: 6572 2062 6569 6e67 206c 6f63 6b65 6420  er being locked 
+00000e60: 7570 2077 6865 6e20 7468 6520 7265 706f  up when the repo
+00000e70: 7274 206f 7065 6e73 2e0a 706c 6f74 735f  rt opens..plots_
+00000e80: 666f 7263 655f 666c 6174 3a20 4661 6c73  force_flat: Fals
+00000e90: 6520 2020 2020 2020 2020 2023 2054 7279  e          # Try
+00000ea0: 2074 6f20 7573 6520 6f6e 6c79 2066 6c61   to use only fla
+00000eb0: 7420 696d 6167 6520 6772 6170 6873 0a70  t image graphs.p
+00000ec0: 6c6f 7473 5f66 6f72 6365 5f69 6e74 6572  lots_force_inter
+00000ed0: 6163 7469 7665 3a20 4661 6c73 6520 2020  active: False   
+00000ee0: 2320 5472 7920 746f 2075 7365 206f 6e6c  # Try to use onl
+00000ef0: 7920 696e 7465 7261 6374 6976 6520 6a61  y interactive ja
+00000f00: 7661 7363 7269 7074 2067 7261 7068 730a  vascript graphs.
+00000f10: 706c 6f74 735f 666c 6174 5f6e 756d 7365  plots_flat_numse
+00000f20: 7269 6573 3a20 3130 3020 2020 2020 2020  ries: 100       
+00000f30: 2023 2049 6620 6e65 6974 6865 7220 6f66   # If neither of
+00000f40: 2074 6865 2061 626f 7665 2c20 7573 6520   the above, use 
+00000f50: 666c 6174 2069 6620 3e20 7468 6973 206e  flat if > this n
+00000f60: 756d 6265 7220 6f66 2064 6174 6173 6574  umber of dataset
+00000f70: 730a 6e75 6d5f 6461 7461 7365 7473 5f70  s.num_datasets_p
+00000f80: 6c6f 745f 6c69 6d69 743a 2035 3020 2020  lot_limit: 50   
+00000f90: 2020 2023 2049 6620 696e 7465 7261 6374     # If interact
+00000fa0: 6976 652c 2064 6f6e 2774 2070 6c6f 7420  ive, don't plot 
+00000fb0: 6f6e 206c 6f61 6420 6966 203e 2074 6869  on load if > thi
+00000fc0: 7320 6e75 6d62 6572 206f 6620 6461 7461  s number of data
+00000fd0: 7365 7473 0a6d 6178 5f74 6162 6c65 5f72  sets.max_table_r
+00000fe0: 6f77 733a 2035 3030 2020 2020 2020 2020  ows: 500        
+00000ff0: 2020 2020 2020 2320 5377 6170 2074 6162        # Swap tab
+00001000: 6c65 7320 666f 7220 6120 6265 6573 7761  les for a beeswa
+00001010: 726d 2070 6c6f 7420 6162 6f76 6520 7468  rm plot above th
+00001020: 6973 0a0a 2320 4f76 6572 7772 6974 6520  is..# Overwrite 
+00001030: 6d6f 6475 6c65 2066 696c 656e 616d 6520  module filename 
+00001040: 7365 6172 6368 2070 6174 7465 726e 732e  search patterns.
+00001050: 2053 6565 206d 756c 7469 7163 2f75 7469   See multiqc/uti
+00001060: 6c73 2f73 6561 7263 685f 7061 7474 6572  ls/search_patter
+00001070: 6e73 2e79 616d 6c0a 2320 666f 7220 7468  ns.yaml.# for th
+00001080: 6520 6465 6661 756c 7473 2e20 5265 6d6f  e defaults. Remo
+00001090: 7665 2061 2064 6566 6175 6c74 2062 7920  ve a default by 
+000010a0: 7365 7474 696e 6720 6974 2074 6f20 6e75  setting it to nu
+000010b0: 6c6c 2e0a 7370 3a0a 2020 2020 7374 6172  ll..sp:.    star
+000010c0: 3a0a 2020 2020 2020 2020 666e 3a20 272a  :.        fn: '*
+000010d0: 4c6f 672e 6669 6e61 6c2e 6f75 7427 0a20  Log.final.out'. 
+000010e0: 2020 2074 7269 6d6d 6f6d 6174 6963 3a0a     trimmomatic:.
+000010f0: 2020 2020 2020 2020 636f 6e74 656e 7473          contents
+00001100: 3a20 2754 7269 6d6d 6f6d 6174 6963 270a  : 'Trimmomatic'.
+00001110: 2020 2020 6375 7461 6461 7074 3a0a 2020      cutadapt:.  
+00001120: 2020 2020 2020 666e 3a20 2763 7574 6164        fn: 'cutad
+00001130: 6170 742e 7478 7427 0a0a 0a0a 2320 4f76  apt.txt'....# Ov
+00001140: 6572 7772 6974 6520 7468 6520 6465 6661  erwrite the defa
+00001150: 756c 7473 206f 6620 7768 6963 6820 7461  ults of which ta
+00001160: 626c 6520 636f 6c75 6d6e 7320 6172 6520  ble columns are 
+00001170: 7669 7369 626c 6520 6279 2064 6566 6175  visible by defau
+00001180: 6c74 0a74 6162 6c65 5f63 6f6c 756d 6e73  lt.table_columns
+00001190: 5f76 6973 6962 6c65 3a0a 2020 2020 4661  _visible:.    Fa
+000011a0: 7374 5143 3a0a 2020 2020 2020 2020 7065  stQC:.        pe
+000011b0: 7263 656e 745f 6661 696c 733a 2046 616c  rcent_fails: Fal
+000011c0: 7365 0a20 2020 2020 2020 2074 6f74 616c  se.        total
+000011d0: 5f73 6571 7565 6e63 6573 3a20 5472 7565  _sequences: True
+000011e0: 0a23 6661 7374 7163 5f63 6f6e 6669 673a  .#fastqc_config:
+000011f0: 0a23 6661 7374 7163 5f74 6865 6f72 6574  .#fastqc_theoret
+00001200: 6963 616c 5f67 633a 2027 6d6d 3130 5f67  ical_gc: 'mm10_g
+00001210: 656e 6f6d 6527 0a                        enome'.
```

### Comparing `sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/dag.png` & `sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/data/WT_R1_.mapped.fastq.gz` & `sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/data/WT_R1_.mapped.fastq.gz`

 * *Files identical despite different names*

### Comparing `sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/data/KO_R1_.mapped.fastq.gz` & `sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/data/KO_R1_.mapped.fastq.gz`

 * *Files identical despite different names*

### Comparing `sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/rnaseq.rules` & `sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/rnaseq.rules`

 * *Files 10% similar despite different names*

```diff
@@ -87,40 +87,40 @@
         __bowtie1_index_ref__log           = "logs/indexing/bowtie_genome.log"
         include: bowtie1_index_dynamic("ref")
     elif os.path.exists(__bowtie1_index_ref__output_done) and do_indexing and force_indexing is False:
         error(msg_error_indexing_exists.format("bowtie1", __bowtie1_index_ref__output_done))
     elif os.path.exists(__bowtie1_index_ref__output_done) is False and do_indexing is False:
         error(msg_error_indexing_notfound.format("bowtie1", __bowtie1_index_ref__output_done))
 
+if manager.config.general.rRNA_file and manager.config.general.rRNA_feature:
+    error("Either set rRNA_file or rRNA_feature in the config file, not both.")
 
 # =========================================================================== rRNA genome
 if manager.config.general.rRNA_file:
-    __bowtie1_index_rna__fasta =            __prefix_name + config["general"]["rRNA_file"]
-    __bowtie1_index_rna__output_done =      __prefix_name__ + "_rRNA.1.ebwt"
-    __bowtie1_index_rna__output_prefix =    __prefix_name__ + "_rRNA"
-    __bowtie1_index_rna__log = "logs/indexing/bowtie_rRNA.log"
-    __RNA_index__ = __bowtie1_index_rna__output_prefix
+    __bowtie1_index_rna__fasta = config['general']["genome_directory"] + os.sep + config["general"]["rRNA_file"]
+    if os.path.exists(__bowtie1_index_rna__fasta) is False:
+        error("File {} does not exists. Check your config file".format(__bowtie1_index_rna__fasta))
 else:
     # extract rRNA feature from GFF and get corresponding fasta
     # and gff. if no match for rRNA, save empty fasta as AAAAAAAAAAA
     __extract_fasta_from_bed__input =       __fasta_file__
     __extract_fasta_from_bed__gff =         __gff_file__
     __extract_fasta_from_bed__feature =     config["general"]["rRNA_feature"]
     __extract_fasta_from_bed__output =          __prefix_name__ + "_rRNA.fa"
     __extract_fasta_from_bed__output_features = __prefix_name__ + "_rRNA.gff"
     __extract_fasta_from_bed__log =             "logs/indexing/get_rRNA.log"
     include: sm.modules["extract_fasta_from_bed"]
 
     # This is fast, so we do it again
     __bowtie1_index_rna__fasta = __extract_fasta_from_bed__output
-    __bowtie1_index_rna__output_done = __prefix_name__ + "_rRNA.1.ebwt"
-    __bowtie1_index_rna__output_prefix = __prefix_name__ + "_rRNA"
-    __bowtie1_index_rna__log = "logs/indexing/bowtie_rRNA.log"
-    include: bowtie1_index_dynamic("rna")
-    __RNA_index__ = __bowtie1_index_rna__output_prefix
+__bowtie1_index_rna__output_done = __prefix_name__ + "_rRNA.1.ebwt"
+__bowtie1_index_rna__output_prefix = __prefix_name__ + "_rRNA"
+__bowtie1_index_rna__log = "logs/indexing/bowtie_rRNA.log"
+include: bowtie1_index_dynamic("rna")
+__RNA_index__ = __bowtie1_index_rna__output_prefix
 
 # ============================================================================ bowtie2 index
 
 if manager.config.general.aligner == "bowtie2":
     __bowtie2_index_ref__output_done   = __prefix_name__ + ".1.bt2"
     __bowtie2_index__ = __prefix_name__
     if os.path.exists(__bowtie2_index_ref__output_done) and do_indexing is False:
@@ -384,38 +384,49 @@
     __mark_duplicates_ref__metrics = manager.getname("mark_duplicates", ".metrics")
     __mark_duplicates_ref__log_std = "%s/logs/mark_duplicates/stdout.logs" % manager.sample
     __mark_duplicates_ref__log_err =  "%s/logs/mark_duplicates/stderr.logs" % manager.sample
     include: mark_duplicates_dynamic("ref", manager)
     expected_output.extend(expand(__mark_duplicates_ref__output, sample=manager.samples))
 
 
-if config["RNAseQC"]["do"]:
+# FIXME do we need the mark_duplicates for RNASEQC2 ? is it compulsary ?
+if config["rnaseqc2"]["do"]:
     if config["mark_duplicates"]['do']:
         __reorderSam__input_sam = __mark_duplicates_ref__output
     else:
         __reorderSam__input_sam = __add_read_group__output
 
     __reorderSam__input_genome = __fasta_file__
     __reorderSam__logs = manager.getname("reorderSam", ".logs")
     __reorderSam__output = manager.getname("reorderSam", "_reorder.bam")
     include: sm.modules["reorderSam"]
-    expected_output.extend(expand(__reorderSam__output, sample=manager.samples))
+    #expected_output.extend(expand(__reorderSam__output, sample=manager.samples))
 
-    __RNAseQC__input_bam = expand(__mark_duplicates_ref__output, sample=manager.samples)
-    __RNAseQC__input_genome = __fasta_file__
-    if os.path.exists(config['RNAseQC']['gtf_file']):
-        __RNAseQC__input_gtf = config['RNAseQC']['gtf_file']
+    # Define input of the rnaseqc2 rule.
+    if config["mark_duplicates"]['do']:
+        __rnaseqc2__input_bam = __mark_duplicates_ref__output
+    else:
+        __rnaseqc2__input_bam = __reorderSam__input_sam
+
+    #__rnaseqc2__input_genome = __fasta_file__
+    if os.path.exists(config['rnaseqc2']['gtf_file']):
+        __rnaseqc2__input_gtf = config['rnaseqc2']['gtf_file']
+    elif os.path.exists(genome_directory + os.sep + config['rnaseqc2']['gtf_file']):
+        __rnaseqc2__input_gtf = genome_directory + os.sep + config['RNAseQC']['gtf_file']
     else:
-        __RNAseQC__input_gtf = genome_directory + os.sep + config['RNAseQC']['gtf_file']
-    __RNAseQC__params_directory = "RNAseQC"
-    __RNAseQC__logs = "RNAseQC/RNAseQC.log"
-    __RNAseQC__output_conf = "RNAseQC/sample_index.txt"
-    __RNAseQC__output_figure =  "RNAseQC/Transcript-associated_Reads_metrics.svg"
-    include: sm.modules["RNAseQC"]
-    expected_output.extend([__RNAseQC__output_figure])
+        error("Could not find {} locally or in {}".format(
+            config['rnaseqc2']['gtf_file'],
+            config['general']['genome_directory']
+        ))
+    __rnaseqc2__params_directory = "{sample}/rnaseqc2"
+    __rnaseqc2__logs = "{sample}/rnaseqc2/{sample}.log"
+    __rnaseqc2__params_sample = "{sample}"
+    __rnaseqc2__output_metrics = "{sample}/rnaseqc2/{sample}.metrics.tsv"
+    include: sm.modules["rnaseqc2"]
+    expected_output.extend(expand(__rnaseqc2__output_metrics, sample=manager.samples))
 
 
 # !Reset expected_output variable after multiqc
 # Hack while waiting for a more general multiqc rules
 
 # Multiqc rule
 __multiqc__input = expected_output
@@ -473,15 +484,15 @@
 
 onsuccess:
     import os
     # Create plots about stats
     sm.plot_stats(N=len(manager.samples))
 
     # Main directory
-    report_dir_format = "%(proj)s/report_rnaseq_%(proj)s"
+    report_dir_format = "%(proj)s/report_rnaseq"
     for proj in manager.samples.keys():
         report_dir = report_dir_format % {"proj": proj}
         try:os.mkdir(report_dir)
         except:pass
 
         shell("cp %s %s" % (__snakefile__, report_dir))
         #shell("cp rulegraph.svg %s/rulegraph.svg" % (report_dir))
@@ -495,12 +506,32 @@
     tocopy = expand(__feature_counts__output_count, sample=manager.samples)
     try:os.mkdir("feature_counts")
     except:pass
     shell("cp {} ./feature_counts/ ".format(" ".join(tocopy)))
 
     sm.OnSuccess()() # create instance to create main cleanup
 
+    with open(__multiqc__output, "r") as fin:
+        with open(__multiqc__output+"2", "w") as fout:
+            line = fin.readline()
+            while line:
+                if """<a href="http://multiqc.info" target="_blank">""" in line:
+                    line = fin.readline() # read the image
+                    line = fin.readline() # read the ending </a> tag
+                else:
+                    fout.write(line)
+                line = fin.readline() # read the next line
+    shell("mv {} {}".format(__multiqc__output +"2", __multiqc__output))
 
 onerror:
     print("An error occurred. See message above.")
 
 
+
+
+
+
+
+
+
+
+
```

### Comparing `sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/main.py` & `sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,20 @@
 feature type, -g by a valid attribute name and -s  by the value 0 (unstranded),
 1( stranded) or 2 (reversely stranded)""")
 
         pipeline_group = self.add_argument_group("pipeline_others")
         pipeline_group.add_argument('--do-igvtools', action="store_true")
         pipeline_group.add_argument('--do-bam-coverage', action="store_true")
         pipeline_group.add_argument('--do-mark-duplicates', action="store_true")
-        pipeline_group.add_argument('--do-rnaseq-qc', action="store_true",
-            help="not yet implemented")
+
+        pipeline_group = self.add_argument_group("pipeline_RNAseQC")
+        pipeline_group.add_argument('--do-rnaseqc', action="store_true",
+            help="do RNA-seq QC using RNAseQC v2")
+        pipeline_group.add_argument('--rnaseqc-gtf-file',
+            help="The GTF file to be used")
 
 
 def main(args=None):
 
     if args is None:
         args = sys.argv
 
@@ -149,23 +153,26 @@
     # ----------------------------------------------------- feature counts
     cfg.feature_counts.options = options.feature_counts_options
 
     # ------------------------------------------------------ optional
     cfg.igvtools.do = options.do_igvtools
     cfg.coverage.do = options.do_bam_coverage
     cfg.mark_duplicates.do = options.do_mark_duplicates
-    cfg.RNAseQC.do = options.do_rnaseq_qc
+
+    # -------------------------------------------------------- RNAseqQC
+    cfg.rnaseqc2.do = options.do_rnaseqc
+    cfg.rnaseqc2.gtf_file = options.rnaseqc_gtf_file
 
     # ----------------------------------------------------- fastq_screen conf
     if options.do_fastq_screen:
         cfg.fastq_screen.do = True
         manager.exists(options.fastq_screen_conf)
         cfg.fastq_screen_conf = os.path.abspath(options.fastq_screen_conf)
         # copy the fastq_screen.conf input or default file
-        shutil.copy(fastq_screen_conf, manager.workdir)
+        shutil.copy(options.fastq_screen_conf, manager.workdir)
     else:
         cfg.fastq_screen.do = False
         # copy the default fastq_screen conf file 
         import sequana_pipelines.rnaseq
         shutil.copy(os.path.join(sequana_pipelines.rnaseq.__path__[0] ,
             "fastq_screen.conf"), manager.workdir)
```

### Comparing `sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/fastq_screen.conf` & `sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/fastq_screen.conf`

 * *Files identical despite different names*

### Comparing `sequana_rnaseq-0.9.8/sequana_pipelines/rnaseq/config.yaml` & `sequana_rnaseq-0.9.9/sequana_pipelines/rnaseq/config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -3,42 +3,44 @@
 #
 # ==================[ Sections for the users ]================================
 #
 # One of input_directory, input_pattern and input_samples must be provided
 # If input_directory provided, use it otherwise if input_pattern provided,
 # use it, otherwise use input_samples.
 # ============================================================================
-input_directory: /home/cokelaer/Work/github/sequana_rnaseq/test
+input_directory: /home/cokelaer/Work/github/sequana_rnaseq/sequana_pipelines/rnaseq/data
 input_readtag: _R[12]_
 input_pattern: '*fastq.gz'
 # =========================================== Sections for the users
 
 #############################################################################
 # Genome section:
 #
 # :Parameters:
 #
 # - aligner: either star, bowtie or bowtie2. fastq_screen, if checked, uses
 #        either bowtie2 by default.
 # - genome_directory: directory where all indexes are written.
-# - rRNA_file: path to fasta file for ribosomal RNA if provided (to be found in
+# - rRNA_file: path to an existing fasta file for ribosomal RNA (to be found in
 #   genome_directory)
-# - rRNA_feature: if rRNA_fasta not provided, ribosomal RNA will be extract
-#     from GFF using this feature
+# - rRNA_feature: if rRNA_file is not provided, ribosomal RNA will be extract
+#     from GFF using this feature name. It must be found. 
 # - indexing: if indexing is set to True, the index for bowtie1 will be done as
 #   well as the indexing of the aligner provided. If the files exists already, not
 #   indexing is performed. If you want to force the index building despite the
 #   presence of the index files, then, use the force_indexing parameter and set
 #   it to True. Indexing is followed by force_indexing to make sure we do not
 #   erase the index files, which may be large.
 general:
-    aligner: bowtie2
+    aligner: star
     genome_directory: /home/cokelaer/Work/github/sequana_rnaseq/test/Saccer3
-    rRNA_file: ''
-    rRNA_feature: rRNA
+    #rRNA_file: 'Saccer3_rRNA.fa'
+    rRNA_file: ""
+    rRNA_feature: rRNA_gene
+    #rRNA_feature:
     indexing: false
     force_indexing: false
 
 
 
 ######################
 # if files are required for a pipeline and are within sequana or should
@@ -287,16 +289,16 @@
 # - do: if unchecked, this rule is ignored. Mandatory for RNA-SeQC tool.
 # - remove: If true do not write duplicates to the output file instead of writing them with
 #            appropriate flags set.  Default value: false. This option can be set to 'null' to clear
 #            the default value. Possible values: {true, false}
 # - tmpdir: write tempory file on this directory (default TMP_DIR=/tmp/, but could be "TMP_DIR=/local/scratch/")
 #
 mark_duplicates:
-    do: false
-    remove: False ## may be True
+    do: true
+    remove: false ## may be True
     tmpdir: /tmp/
     threads: 4
 
 
 
 #############################################################################
 # RNA-SeQC allows to compute a series of quality control metrics for RNA-seq data
@@ -306,19 +308,18 @@
 # - do: if unchecked, this rule is ignored
 # - ref: Reference Genome in fasta format
 # - gtf: GTF File defining transcripts (must end in '.gtf')
 # - BWArRNA: Use an on the fly BWA alignment for estimating
 #            rRNA content. The value should be the rRNA
 #            reference fasta.
 # - options: any options recognised by RNA-seQC tool
-RNAseQC:
-    do: false
-    gtf_file: file.gtf
-    BWArRNA_file: file_rRNA.fasta
-    options: ''
+rnaseqc2:
+    do: true
+    gtf_file: Saccer3.gtf
+    options: ' --coverage '
 
 
 #############################################################################
 #   MultiQC aggregates results from bioinformatics analyses across many
 #   samples into a single report.
 #
 # :Parameters:
```

### Comparing `sequana_rnaseq-0.9.8/README.rst` & `sequana_rnaseq-0.9.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,16 @@
 
 Changelog
 ~~~~~~~~~
 
 ========= ====================================================================
 Version   Description
 ========= ====================================================================
+0.9.9     * Fix RNAseQC rule, which is now available. 
+          * Fix ability to use existing rRNA file as input
 0.9.8     * Fix indexing for bowtie1 to not be done if aligner is different
           * add new options: --feature-counts-options and --do-rnaseq-qc,
             --rRNA-feature
           * Based on the input GFF, we now check the validity of the rRNA
             feature and feature counts options to check whether the feature 
             exists in the GFF
           * schema is now used to check the config file values
```

