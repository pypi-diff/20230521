# Comparing `tmp/gb2seq-0.2.6.tar.gz` & `tmp/gb2seq-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gb2seq-0.2.6.tar", last modified: Sun May 21 14:18:29 2023, max compression
+gzip compressed data, was "gb2seq-0.2.7.tar", last modified: Sun May 21 14:24:44 2023, max compression
```

## Comparing `gb2seq-0.2.6.tar` & `gb2seq-0.2.7.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:18:29.961735 gb2seq-0.2.6/
--rw-rw-r--   0 terry      (501) staff       (20)       82 2022-08-03 22:54:17.000000 gb2seq-0.2.6/AUTHORS
--rw-rw-r--   0 terry      (501) staff       (20)       39 2023-05-20 21:53:46.000000 gb2seq-0.2.6/MANIFEST.in
--rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 14:18:29.961277 gb2seq-0.2.6/PKG-INFO
--rw-rw-r--   0 terry      (501) staff       (20)    26621 2023-05-21 12:53:46.000000 gb2seq-0.2.6/README.md
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:18:29.947806 gb2seq-0.2.6/bin/
--rwxrwxr-x   0 terry      (501) staff       (20)     1933 2022-08-04 07:08:53.000000 gb2seq-0.2.6/bin/annotate-genome.py
--rwxrwxr-x   0 terry      (501) staff       (20)     7257 2023-05-21 10:01:54.000000 gb2seq-0.2.6/bin/describe-feature.py
--rwxrwxr-x   0 terry      (501) staff       (20)    15353 2023-05-20 07:09:01.000000 gb2seq-0.2.6/bin/describe-genome.py
--rwxrwxr-x   0 terry      (501) staff       (20)     6171 2023-05-21 10:32:17.000000 gb2seq-0.2.6/bin/describe-site.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:18:29.952612 gb2seq-0.2.6/gb2seq/
--rw-rw-r--   0 terry      (501) staff       (20)       93 2023-05-21 13:47:53.000000 gb2seq-0.2.6/gb2seq/__init__.py
--rw-rw-r--   0 terry      (501) staff       (20)    41849 2023-05-21 12:40:54.000000 gb2seq-0.2.6/gb2seq/alignment.py
--rw-rw-r--   0 terry      (501) staff       (20)     7745 2023-03-24 11:55:34.000000 gb2seq-0.2.6/gb2seq/annotate.py
--rw-rw-r--   0 terry      (501) staff       (20)     1701 2022-08-03 22:54:17.000000 gb2seq-0.2.6/gb2seq/change.py
--rw-rw-r--   0 terry      (501) staff       (20)     1961 2022-08-03 22:54:17.000000 gb2seq-0.2.6/gb2seq/checker.py
--rw-rw-r--   0 terry      (501) staff       (20)    27532 2023-05-21 14:02:33.000000 gb2seq-0.2.6/gb2seq/features.py
--rw-rw-r--   0 terry      (501) staff       (20)      558 2022-08-03 22:54:17.000000 gb2seq-0.2.6/gb2seq/genome.py
--rw-rw-r--   0 terry      (501) staff       (20)     2457 2023-03-24 11:55:34.000000 gb2seq-0.2.6/gb2seq/sars2.py
--rw-rw-r--   0 terry      (501) staff       (20)    20485 2023-05-21 07:41:44.000000 gb2seq-0.2.6/gb2seq/translate.py
--rw-rw-r--   0 terry      (501) staff       (20)     2049 2022-08-03 22:56:02.000000 gb2seq-0.2.6/gb2seq/variants.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:18:29.954893 gb2seq-0.2.6/gb2seq.egg-info/
--rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 14:18:29.000000 gb2seq-0.2.6/gb2seq.egg-info/PKG-INFO
--rw-rw-r--   0 terry      (501) staff       (20)      648 2023-05-21 14:18:29.000000 gb2seq-0.2.6/gb2seq.egg-info/SOURCES.txt
--rw-rw-r--   0 terry      (501) staff       (20)        1 2023-05-21 14:18:29.000000 gb2seq-0.2.6/gb2seq.egg-info/dependency_links.txt
--rw-rw-r--   0 terry      (501) staff       (20)       20 2023-05-21 14:18:29.000000 gb2seq-0.2.6/gb2seq.egg-info/requires.txt
--rw-rw-r--   0 terry      (501) staff       (20)        7 2023-05-21 14:18:29.000000 gb2seq-0.2.6/gb2seq.egg-info/top_level.txt
--rw-rw-r--   0 terry      (501) staff       (20)      539 2023-05-20 13:31:27.000000 gb2seq-0.2.6/pyproject.toml
--rw-rw-r--   0 terry      (501) staff       (20)       38 2023-05-21 14:18:29.961870 gb2seq-0.2.6/setup.cfg
--rw-rw-r--   0 terry      (501) staff       (20)     2079 2023-05-21 13:34:44.000000 gb2seq-0.2.6/setup.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:18:29.960564 gb2seq-0.2.6/test/
--rw-rw-r--   0 terry      (501) staff       (20)    66686 2023-05-21 13:39:01.000000 gb2seq-0.2.6/test/test_alignment.py
--rw-rw-r--   0 terry      (501) staff       (20)     1903 2022-08-03 23:06:40.000000 gb2seq-0.2.6/test/test_change.py
--rw-rw-r--   0 terry      (501) staff       (20)     5116 2023-05-21 13:39:38.000000 gb2seq-0.2.6/test/test_checker.py
--rw-rw-r--   0 terry      (501) staff       (20)    12860 2023-03-24 11:55:34.000000 gb2seq-0.2.6/test/test_features.py
--rw-rw-r--   0 terry      (501) staff       (20)    17090 2023-05-21 13:40:07.000000 gb2seq-0.2.6/test/test_genomes.py
--rw-rw-r--   0 terry      (501) staff       (20)      414 2022-08-03 23:08:39.000000 gb2seq-0.2.6/test/test_sars2.py
--rw-rw-r--   0 terry      (501) staff       (20)    21028 2023-05-21 12:34:49.000000 gb2seq-0.2.6/test/test_translate.py
--rw-rw-r--   0 terry      (501) staff       (20)     1075 2023-05-21 13:47:12.000000 gb2seq-0.2.6/test/test_variants.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:24:44.189385 gb2seq-0.2.7/
+-rw-rw-r--   0 terry      (501) staff       (20)       82 2022-08-03 22:54:17.000000 gb2seq-0.2.7/AUTHORS
+-rw-rw-r--   0 terry      (501) staff       (20)       39 2023-05-20 21:53:46.000000 gb2seq-0.2.7/MANIFEST.in
+-rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 14:24:44.188997 gb2seq-0.2.7/PKG-INFO
+-rw-rw-r--   0 terry      (501) staff       (20)    26621 2023-05-21 12:53:46.000000 gb2seq-0.2.7/README.md
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:24:44.175412 gb2seq-0.2.7/bin/
+-rwxrwxr-x   0 terry      (501) staff       (20)     1933 2022-08-04 07:08:53.000000 gb2seq-0.2.7/bin/annotate-genome.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     7257 2023-05-21 10:01:54.000000 gb2seq-0.2.7/bin/describe-feature.py
+-rwxrwxr-x   0 terry      (501) staff       (20)    15353 2023-05-20 07:09:01.000000 gb2seq-0.2.7/bin/describe-genome.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     6171 2023-05-21 10:32:17.000000 gb2seq-0.2.7/bin/describe-site.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:24:44.181634 gb2seq-0.2.7/gb2seq/
+-rw-rw-r--   0 terry      (501) staff       (20)       93 2023-05-21 14:24:28.000000 gb2seq-0.2.7/gb2seq/__init__.py
+-rw-rw-r--   0 terry      (501) staff       (20)    41849 2023-05-21 12:40:54.000000 gb2seq-0.2.7/gb2seq/alignment.py
+-rw-rw-r--   0 terry      (501) staff       (20)     7745 2023-03-24 11:55:34.000000 gb2seq-0.2.7/gb2seq/annotate.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1701 2022-08-03 22:54:17.000000 gb2seq-0.2.7/gb2seq/change.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1961 2022-08-03 22:54:17.000000 gb2seq-0.2.7/gb2seq/checker.py
+-rw-rw-r--   0 terry      (501) staff       (20)    27532 2023-05-21 14:02:33.000000 gb2seq-0.2.7/gb2seq/features.py
+-rw-rw-r--   0 terry      (501) staff       (20)      558 2022-08-03 22:54:17.000000 gb2seq-0.2.7/gb2seq/genome.py
+-rw-rw-r--   0 terry      (501) staff       (20)     2457 2023-03-24 11:55:34.000000 gb2seq-0.2.7/gb2seq/sars2.py
+-rw-rw-r--   0 terry      (501) staff       (20)    20485 2023-05-21 07:41:44.000000 gb2seq-0.2.7/gb2seq/translate.py
+-rw-rw-r--   0 terry      (501) staff       (20)     2049 2022-08-03 22:56:02.000000 gb2seq-0.2.7/gb2seq/variants.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:24:44.183766 gb2seq-0.2.7/gb2seq.egg-info/
+-rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 14:24:43.000000 gb2seq-0.2.7/gb2seq.egg-info/PKG-INFO
+-rw-rw-r--   0 terry      (501) staff       (20)      633 2023-05-21 14:24:44.000000 gb2seq-0.2.7/gb2seq.egg-info/SOURCES.txt
+-rw-rw-r--   0 terry      (501) staff       (20)        1 2023-05-21 14:24:43.000000 gb2seq-0.2.7/gb2seq.egg-info/dependency_links.txt
+-rw-rw-r--   0 terry      (501) staff       (20)       20 2023-05-21 14:24:43.000000 gb2seq-0.2.7/gb2seq.egg-info/requires.txt
+-rw-rw-r--   0 terry      (501) staff       (20)        7 2023-05-21 14:24:43.000000 gb2seq-0.2.7/gb2seq.egg-info/top_level.txt
+-rw-rw-r--   0 terry      (501) staff       (20)       38 2023-05-21 14:24:44.189456 gb2seq-0.2.7/setup.cfg
+-rw-rw-r--   0 terry      (501) staff       (20)     2079 2023-05-21 13:34:44.000000 gb2seq-0.2.7/setup.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:24:44.188370 gb2seq-0.2.7/test/
+-rw-rw-r--   0 terry      (501) staff       (20)    66686 2023-05-21 13:39:01.000000 gb2seq-0.2.7/test/test_alignment.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1903 2022-08-03 23:06:40.000000 gb2seq-0.2.7/test/test_change.py
+-rw-rw-r--   0 terry      (501) staff       (20)     5116 2023-05-21 13:39:38.000000 gb2seq-0.2.7/test/test_checker.py
+-rw-rw-r--   0 terry      (501) staff       (20)    12860 2023-03-24 11:55:34.000000 gb2seq-0.2.7/test/test_features.py
+-rw-rw-r--   0 terry      (501) staff       (20)    17090 2023-05-21 13:40:07.000000 gb2seq-0.2.7/test/test_genomes.py
+-rw-rw-r--   0 terry      (501) staff       (20)      414 2022-08-03 23:08:39.000000 gb2seq-0.2.7/test/test_sars2.py
+-rw-rw-r--   0 terry      (501) staff       (20)    21028 2023-05-21 12:34:49.000000 gb2seq-0.2.7/test/test_translate.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1075 2023-05-21 13:47:12.000000 gb2seq-0.2.7/test/test_variants.py
```

### Comparing `gb2seq-0.2.6/PKG-INFO` & `gb2seq-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gb2seq
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python library and scripts for working with unannotated sequences based on an annotated reference genome provided by a GenBank file.
 Home-page: https://github.com/virologycharite/gb2seq
 Download-URL: https://github.com/virologycharite/gb2seq
 Author: Terry C. Jones
 Author-email: terence.jones@charite.de
 Maintainer: Terry C. Jones
 Maintainer-email: terence.jones@charite.de
```

### Comparing `gb2seq-0.2.6/README.md` & `gb2seq-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/bin/annotate-genome.py` & `gb2seq-0.2.7/bin/annotate-genome.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/bin/describe-feature.py` & `gb2seq-0.2.7/bin/describe-feature.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/bin/describe-genome.py` & `gb2seq-0.2.7/bin/describe-genome.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/bin/describe-site.py` & `gb2seq-0.2.7/bin/describe-site.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/gb2seq/alignment.py` & `gb2seq-0.2.7/gb2seq/alignment.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/gb2seq/annotate.py` & `gb2seq-0.2.7/gb2seq/annotate.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/gb2seq/change.py` & `gb2seq-0.2.7/gb2seq/change.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/gb2seq/checker.py` & `gb2seq-0.2.7/gb2seq/checker.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/gb2seq/features.py` & `gb2seq-0.2.7/gb2seq/features.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/gb2seq/genome.py` & `gb2seq-0.2.7/gb2seq/genome.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/gb2seq/sars2.py` & `gb2seq-0.2.7/gb2seq/sars2.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/gb2seq/translate.py` & `gb2seq-0.2.7/gb2seq/translate.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/gb2seq/variants.py` & `gb2seq-0.2.7/gb2seq/variants.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/gb2seq.egg-info/PKG-INFO` & `gb2seq-0.2.7/gb2seq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gb2seq
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python library and scripts for working with unannotated sequences based on an annotated reference genome provided by a GenBank file.
 Home-page: https://github.com/virologycharite/gb2seq
 Download-URL: https://github.com/virologycharite/gb2seq
 Author: Terry C. Jones
 Author-email: terence.jones@charite.de
 Maintainer: Terry C. Jones
 Maintainer-email: terence.jones@charite.de
```

### Comparing `gb2seq-0.2.6/gb2seq.egg-info/SOURCES.txt` & `gb2seq-0.2.7/gb2seq.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 AUTHORS
 MANIFEST.in
 README.md
-pyproject.toml
 setup.py
 bin/annotate-genome.py
 bin/describe-feature.py
 bin/describe-genome.py
 bin/describe-site.py
 gb2seq/__init__.py
 gb2seq/alignment.py
```

### Comparing `gb2seq-0.2.6/setup.py` & `gb2seq-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/test/test_alignment.py` & `gb2seq-0.2.7/test/test_alignment.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/test/test_change.py` & `gb2seq-0.2.7/test/test_change.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/test/test_checker.py` & `gb2seq-0.2.7/test/test_checker.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/test/test_features.py` & `gb2seq-0.2.7/test/test_features.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/test/test_genomes.py` & `gb2seq-0.2.7/test/test_genomes.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/test/test_translate.py` & `gb2seq-0.2.7/test/test_translate.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.6/test/test_variants.py` & `gb2seq-0.2.7/test/test_variants.py`

 * *Files identical despite different names*

