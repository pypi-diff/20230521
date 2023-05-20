# Comparing `tmp/textagon-0.1.8.tar.gz` & `tmp/textagon-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textagon-0.1.8.tar", last modified: Sat May 20 04:00:06 2023, max compression
+gzip compressed data, was "textagon-0.1.9.tar", last modified: Sat May 20 04:45:47 2023, max compression
```

## Comparing `textagon-0.1.8.tar` & `textagon-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 04:00:06.172123 textagon-0.1.8/
--rw-rw-rw-   0        0        0      181 2023-05-20 04:00:06.172123 textagon-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-20 04:00:06.172123 textagon-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-05-20 03:59:47.000000 textagon-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 04:00:06.143119 textagon-0.1.8/textagon/
--rw-rw-rw-   0        0        0      218 2023-05-20 01:44:59.000000 textagon-0.1.8/textagon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 04:00:06.134112 textagon-0.1.8/textagon/external/
-drwxrwxrwx   0        0        0        0 2023-05-20 04:00:06.134112 textagon-0.1.8/textagon/external/extracted/
-drwxrwxrwx   0        0        0        0 2023-05-20 04:00:06.158120 textagon-0.1.8/textagon/external/extracted/WNAffect-master/
--rw-rw-rw-   0        0        0    33762 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/WNAffect-master/README.md
--rw-rw-rw-   0        0        0     2953 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/WNAffect-master/emotion.py
--rw-rw-rw-   0        0        0     3454 2023-05-20 03:59:40.000000 textagon-0.1.8/textagon/external/extracted/WNAffect-master/wnaffect.py
-drwxrwxrwx   0        0        0        0 2023-05-20 04:00:06.164120 textagon-0.1.8/textagon/external/extracted/wn-domains/
--rw-rw-rw-   0        0        0    84063 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wn-domains/Coling-04-ws-WDH.pdf
--rw-rw-rw-   0        0        0     2247 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wn-domains/README
--rw-rw-rw-   0        0        0    47416 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wn-domains/WDH-old-new-comparison.pdf
--rw-rw-rw-   0        0        0     8688 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wn-domains/WDH-revision-summary.pdf
--rw-rw-rw-   0        0        0    39740 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wn-domains/WDH-to-DDC-map.pdf
--rw-rw-rw-   0        0        0    51492 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wn-domains/WORDNET-DOMAINS-2.0-TR.pdf
--rw-rw-rw-   0        0        0     2278 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wn-domains/version-history.txt
--rw-rw-rw-   0        0        0  2213039 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wn-domains/wn-domains-2.0-20050210
--rw-rw-rw-   0        0        0  2543843 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wn-domains/wn-domains-3.2-20070223
-drwxrwxrwx   0        0        0        0 2023-05-20 04:00:06.170111 textagon-0.1.8/textagon/external/extracted/wordnet-1.6/
--rw-rw-rw-   0        0        0     3788 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wordnet-1.6/CHANGES
--rw-rw-rw-   0        0        0     6176 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wordnet-1.6/INSTALL
--rw-rw-rw-   0        0        0     1625 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wordnet-1.6/LICENSE
--rw-rw-rw-   0        0        0     7217 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wordnet-1.6/Makefile
--rw-rw-rw-   0        0        0    11453 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wordnet-1.6/README
--rw-rw-rw-   0        0        0     1996 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wordnet-1.6/README.ml
--rw-rw-rw-   0        0        0     1612 2023-05-19 15:50:31.000000 textagon-0.1.8/textagon/external/extracted/wordnet-1.6/README.tcltk
-drwxrwxrwx   0        0        0        0 2023-05-20 04:00:06.171118 textagon-0.1.8/textagon/external/lexicons/
--rw-rw-rw-   0        0        0   477716 2023-05-19 15:50:35.000000 textagon-0.1.8/textagon/external/lexicons/Lexicons_v5.zip
--rw-rw-rw-   0        0        0    43255 2023-05-19 15:50:35.000000 textagon-0.1.8/textagon/external/lexicons/exclusions.txt
--rw-rw-rw-   0        0        0      197 2023-05-19 15:50:30.000000 textagon-0.1.8/textagon/install-dependencies.py
--rw-rw-rw-   0        0        0      309 2023-05-19 22:15:17.000000 textagon-0.1.8/textagon/post_install.py
--rw-rw-rw-   0        0        0    60290 2023-05-19 15:50:30.000000 textagon-0.1.8/textagon/process-text.py
--rw-rw-rw-   0        0        0    26116 2023-05-20 03:57:47.000000 textagon-0.1.8/textagon/textagon.py
-drwxrwxrwx   0        0        0        0 2023-05-20 04:00:06.150115 textagon-0.1.8/textagon.egg-info/
--rw-rw-rw-   0        0        0      181 2023-05-20 04:00:06.000000 textagon-0.1.8/textagon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2023-05-20 04:00:06.000000 textagon-0.1.8/textagon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 04:00:06.000000 textagon-0.1.8/textagon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-20 04:00:06.000000 textagon-0.1.8/textagon.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2023-05-20 04:00:06.000000 textagon-0.1.8/textagon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 04:00:06.000000 textagon-0.1.8/textagon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 04:45:47.619692 textagon-0.1.9/
+-rw-rw-rw-   0        0        0      181 2023-05-20 04:45:47.618690 textagon-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-20 04:45:47.619692 textagon-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-05-20 04:45:23.000000 textagon-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 04:45:47.597340 textagon-0.1.9/textagon/
+-rw-rw-rw-   0        0        0      218 2023-05-20 01:44:59.000000 textagon-0.1.9/textagon/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 04:45:47.586334 textagon-0.1.9/textagon/external/
+drwxrwxrwx   0        0        0        0 2023-05-20 04:45:47.586334 textagon-0.1.9/textagon/external/extracted/
+drwxrwxrwx   0        0        0        0 2023-05-20 04:45:47.606476 textagon-0.1.9/textagon/external/extracted/WNAffect-master/
+-rw-rw-rw-   0        0        0    33762 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/WNAffect-master/README.md
+-rw-rw-rw-   0        0        0     2953 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/WNAffect-master/emotion.py
+-rw-rw-rw-   0        0        0     3454 2023-05-20 03:59:40.000000 textagon-0.1.9/textagon/external/extracted/WNAffect-master/wnaffect.py
+drwxrwxrwx   0        0        0        0 2023-05-20 04:45:47.612699 textagon-0.1.9/textagon/external/extracted/wn-domains/
+-rw-rw-rw-   0        0        0    84063 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wn-domains/Coling-04-ws-WDH.pdf
+-rw-rw-rw-   0        0        0     2247 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wn-domains/README
+-rw-rw-rw-   0        0        0    47416 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wn-domains/WDH-old-new-comparison.pdf
+-rw-rw-rw-   0        0        0     8688 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wn-domains/WDH-revision-summary.pdf
+-rw-rw-rw-   0        0        0    39740 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wn-domains/WDH-to-DDC-map.pdf
+-rw-rw-rw-   0        0        0    51492 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wn-domains/WORDNET-DOMAINS-2.0-TR.pdf
+-rw-rw-rw-   0        0        0     2278 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wn-domains/version-history.txt
+-rw-rw-rw-   0        0        0  2213039 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wn-domains/wn-domains-2.0-20050210
+-rw-rw-rw-   0        0        0  2543843 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wn-domains/wn-domains-3.2-20070223
+drwxrwxrwx   0        0        0        0 2023-05-20 04:45:47.617692 textagon-0.1.9/textagon/external/extracted/wordnet-1.6/
+-rw-rw-rw-   0        0        0     3788 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wordnet-1.6/CHANGES
+-rw-rw-rw-   0        0        0     6176 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wordnet-1.6/INSTALL
+-rw-rw-rw-   0        0        0     1625 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wordnet-1.6/LICENSE
+-rw-rw-rw-   0        0        0     7217 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wordnet-1.6/Makefile
+-rw-rw-rw-   0        0        0    11453 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wordnet-1.6/README
+-rw-rw-rw-   0        0        0     1996 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wordnet-1.6/README.ml
+-rw-rw-rw-   0        0        0     1612 2023-05-19 15:50:31.000000 textagon-0.1.9/textagon/external/extracted/wordnet-1.6/README.tcltk
+drwxrwxrwx   0        0        0        0 2023-05-20 04:45:47.618690 textagon-0.1.9/textagon/external/lexicons/
+-rw-rw-rw-   0        0        0   477716 2023-05-19 15:50:35.000000 textagon-0.1.9/textagon/external/lexicons/Lexicons_v5.zip
+-rw-rw-rw-   0        0        0    43255 2023-05-19 15:50:35.000000 textagon-0.1.9/textagon/external/lexicons/exclusions.txt
+-rw-rw-rw-   0        0        0      197 2023-05-19 15:50:30.000000 textagon-0.1.9/textagon/install-dependencies.py
+-rw-rw-rw-   0        0        0      309 2023-05-19 22:15:17.000000 textagon-0.1.9/textagon/post_install.py
+-rw-rw-rw-   0        0        0    60290 2023-05-19 15:50:30.000000 textagon-0.1.9/textagon/process-text.py
+-rw-rw-rw-   0        0        0    26764 2023-05-20 04:45:16.000000 textagon-0.1.9/textagon/textagon.py
+drwxrwxrwx   0        0        0        0 2023-05-20 04:45:47.604337 textagon-0.1.9/textagon.egg-info/
+-rw-rw-rw-   0        0        0      181 2023-05-20 04:45:47.000000 textagon-0.1.9/textagon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1465 2023-05-20 04:45:47.000000 textagon-0.1.9/textagon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 04:45:47.000000 textagon-0.1.9/textagon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-20 04:45:47.000000 textagon-0.1.9/textagon.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2023-05-20 04:45:47.000000 textagon-0.1.9/textagon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-20 04:45:47.000000 textagon-0.1.9/textagon.egg-info/top_level.txt
```

### Comparing `textagon-0.1.8/setup.py` & `textagon-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'textagon',
-    version = '0.1.8',
+    version = '0.1.9',
     packages = find_packages(),
     description = 'Start building textagon',
     author = 'Mendoza',
     classifiers=[
         "License :: OSI Approved :: Python Software Foundation License"
     ],
     install_requires=[
```

### Comparing `textagon-0.1.8/textagon/external/extracted/WNAffect-master/README.md` & `textagon-0.1.9/textagon/external/extracted/WNAffect-master/README.md`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/WNAffect-master/emotion.py` & `textagon-0.1.9/textagon/external/extracted/WNAffect-master/emotion.py`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/WNAffect-master/wnaffect.py` & `textagon-0.1.9/textagon/external/extracted/WNAffect-master/wnaffect.py`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wn-domains/Coling-04-ws-WDH.pdf` & `textagon-0.1.9/textagon/external/extracted/wn-domains/Coling-04-ws-WDH.pdf`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wn-domains/README` & `textagon-0.1.9/textagon/external/extracted/wn-domains/README`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wn-domains/WDH-old-new-comparison.pdf` & `textagon-0.1.9/textagon/external/extracted/wn-domains/WDH-old-new-comparison.pdf`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wn-domains/WDH-revision-summary.pdf` & `textagon-0.1.9/textagon/external/extracted/wn-domains/WDH-revision-summary.pdf`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wn-domains/WDH-to-DDC-map.pdf` & `textagon-0.1.9/textagon/external/extracted/wn-domains/WDH-to-DDC-map.pdf`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wn-domains/WORDNET-DOMAINS-2.0-TR.pdf` & `textagon-0.1.9/textagon/external/extracted/wn-domains/WORDNET-DOMAINS-2.0-TR.pdf`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wn-domains/version-history.txt` & `textagon-0.1.9/textagon/external/extracted/wn-domains/version-history.txt`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wn-domains/wn-domains-2.0-20050210` & `textagon-0.1.9/textagon/external/extracted/wn-domains/wn-domains-2.0-20050210`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wn-domains/wn-domains-3.2-20070223` & `textagon-0.1.9/textagon/external/extracted/wn-domains/wn-domains-3.2-20070223`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wordnet-1.6/CHANGES` & `textagon-0.1.9/textagon/external/extracted/wordnet-1.6/CHANGES`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wordnet-1.6/INSTALL` & `textagon-0.1.9/textagon/external/extracted/wordnet-1.6/INSTALL`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wordnet-1.6/LICENSE` & `textagon-0.1.9/textagon/external/extracted/wordnet-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wordnet-1.6/Makefile` & `textagon-0.1.9/textagon/external/extracted/wordnet-1.6/Makefile`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wordnet-1.6/README` & `textagon-0.1.9/textagon/external/extracted/wordnet-1.6/README`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wordnet-1.6/README.ml` & `textagon-0.1.9/textagon/external/extracted/wordnet-1.6/README.ml`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/extracted/wordnet-1.6/README.tcltk` & `textagon-0.1.9/textagon/external/extracted/wordnet-1.6/README.tcltk`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/lexicons/Lexicons_v5.zip` & `textagon-0.1.9/textagon/external/lexicons/Lexicons_v5.zip`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/external/lexicons/exclusions.txt` & `textagon-0.1.9/textagon/external/lexicons/exclusions.txt`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/process-text.py` & `textagon-0.1.9/textagon/process-text.py`

 * *Files identical despite different names*

### Comparing `textagon-0.1.8/textagon/textagon.py` & `textagon-0.1.9/textagon/textagon.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,24 +57,24 @@
 
 ### Setup NLP Tools ###
 
 # SentiWN #
 from nltk.corpus import sentiwordnet as swn
 swn.ensure_loaded()
 
-import pkg_resources
+# import pkg_resources
 
-wnaffect_path = pkg_resources.resource_filename('textagon', 'external/extracted/WNAffect-master')
-wordnet_path = nltk.data.find('corpora/wordnet').path
-wn_domains_path = pkg_resources.resource_filename('textagon', 'external/extracted/wn-domains')
-
-sys.path.append(wnaffect_path)
-from wnaffect import WNAffect
-from emotion import Emotion
-wna = WNAffect(wordnet_path, wn_domains_path)
+# wnaffect_path = pkg_resources.resource_filename('textagon', 'external/extracted/WNAffect-master')
+# wordnet_path = nltk.data.find('corpora/wordnet').path
+# wn_domains_path = pkg_resources.resource_filename('textagon', 'external/extracted/wn-domains')
+
+# sys.path.append(wnaffect_path)
+# from wnaffect import WNAffect
+# from emotion import Emotion
+# wna = WNAffect(wordnet_path, wn_domains_path)
 
 # VADER #
 from nltk.sentiment.vader import SentimentIntensityAnalyzer
 
 # spaCy #
 import spacy
 nlp = spacy.load('en_core_web_sm', exclude = ['lemmatizer'])
@@ -275,431 +275,431 @@
     print("Reading raw text...")
     pure_chunck = SanityCheck(dataPath=path, override_original_file=False)
     classLabels = list(pure_chunck['samples_per_class'].keys())
     raw = [x[1] for x in pure_chunck['raw_data']]
     print("Reading raw text completed.")
     return({'corpus': raw, 'classLabels': classLabels})
 
-def TextToFeatures (textData, debug = False, lexicons = None, wnaReturnLevel = 5, useSpellChecker = True, provideMisspellingDetailed = True, useCores = 1):
+# def TextToFeatures (textData, debug = False, lexicons = None, wnaReturnLevel = 5, useSpellChecker = True, provideMisspellingDetailed = True, useCores = 1):
 
-    if lexicons == None:
-        lexicons = ReadAllLexicons()
-    else:
-        if isinstance(lexicons, str):
-            if os.path.exists(lexicons):
-                lexicons = ReadAllLexicons(lexiconFileFullPath=lexicons)
-        elif isinstance(lexicons, collections.OrderedDict):
-            pass
-        else:
-            print('Lexicons must be a path to lexicon zip file or an well-done lexicon OrderedDict.')
-            return None
-
-    spellcheckerLibrary, exclusionsFileFullPath, exclusionsLength, spellchecker = setSpellChecking(exclusionsFileFullPath=exclusionsFileFullPath)
-
-    textData = pd.DataFrame({
-        'InitialSentence': textData
-        })
-
-    def BasicTextCleanup (sentence, debug = False):
-
-        if debug:
-            print('\nInitial Sentence:', sentence)
-
-        # note: need to add exception handler (e.g., non-English issues)
-
-        # Basic Cleaning
-        initialSentenceLength = len(sentence)
-
-        # Strip html
-        sentence = BS(sentence, 'html.parser').get_text()
-        htmlStripLength = initialSentenceLength - len(sentence)
-
-        # Strip all excessive whitespace (after html to ensure no additional spaces result from html stripping)
-        sentence = ' '.join(sentence.split())
-        whitespaceStripLength = initialSentenceLength - htmlStripLength - len(sentence)
-
-        # Spellchecking
-        spellingCorrectionDetailsSentences = []
-        spellingCorrectionDetailsWords = []
-        spellingCorrectionDetailsSuggestions = []
-        spellingCorrectionDetailsChosenSuggestion = []
-        spellingCorrectionDetailsChangesWord = []
-        spellingCorrectionDetailsReplacementLength = []
-        spellingCorrectionCount = 0
+#     if lexicons == None:
+#         lexicons = ReadAllLexicons()
+#     else:
+#         if isinstance(lexicons, str):
+#             if os.path.exists(lexicons):
+#                 lexicons = ReadAllLexicons(lexiconFileFullPath=lexicons)
+#         elif isinstance(lexicons, collections.OrderedDict):
+#             pass
+#         else:
+#             print('Lexicons must be a path to lexicon zip file or an well-done lexicon OrderedDict.')
+#             return None
+
+#     spellcheckerLibrary, exclusionsFileFullPath, exclusionsLength, spellchecker = setSpellChecking(exclusionsFileFullPath=exclusionsFileFullPath)
+
+#     textData = pd.DataFrame({
+#         'InitialSentence': textData
+#         })
+
+#     def BasicTextCleanup (sentence, debug = False):
+
+#         if debug:
+#             print('\nInitial Sentence:', sentence)
+
+#         # note: need to add exception handler (e.g., non-English issues)
+
+#         # Basic Cleaning
+#         initialSentenceLength = len(sentence)
+
+#         # Strip html
+#         sentence = BS(sentence, 'html.parser').get_text()
+#         htmlStripLength = initialSentenceLength - len(sentence)
+
+#         # Strip all excessive whitespace (after html to ensure no additional spaces result from html stripping)
+#         sentence = ' '.join(sentence.split())
+#         whitespaceStripLength = initialSentenceLength - htmlStripLength - len(sentence)
+
+#         # Spellchecking
+#         spellingCorrectionDetailsSentences = []
+#         spellingCorrectionDetailsWords = []
+#         spellingCorrectionDetailsSuggestions = []
+#         spellingCorrectionDetailsChosenSuggestion = []
+#         spellingCorrectionDetailsChangesWord = []
+#         spellingCorrectionDetailsReplacementLength = []
+#         spellingCorrectionCount = 0
+
+#         spellchecker = enchant.DictWithPWL(spellcheckerLibrary, pwl = exclusionsFileFullPath, broker = b)
+#         chkr = SpellChecker(spellchecker, sentence, filters = [EmailFilter, URLFilter])
+
+#         collectMisspellingDetails = {
+#             'Word': [], 
+#             'Substitution': [], 
+#             'SubstitutionText': []
+#             }
+
+#         for err in chkr:
+
+#             #print('\nSpellcheck Word:', err.word)
+#             matchedWord = False
+
+#             word = err.word
+
+#             if lexicons is not None and provideMisspellingDetailed:
+
+#                 appendLexiconLabel = ''
+
+#                 for lexicon, tagTokenPairs in lexicons.items():
+
+#                     lexiconName = '|_|' + lexicon.upper() + '&'
+
+#                     matchedWord = False  # note: we want to capture in multiple lexicons (but only once per lexicon)
+
+#                     for tag, tokens in tagTokenPairs.items():
+
+#                         if matchedWord:
+#                             break
+
+#                         elif any('*' in s for s in tokens):
+#                             # regex mode
+#                             nonmatching = [s for s in tokens if not s.endswith('*')]
+#                             if word.lower() in nonmatching:
+#                                 appendLexiconLabel += lexiconName + tag.upper()
+#                                 matchedWord = True
+#                             else:
+#                                 matching = [s for s in tokens if s.endswith('*')]
+#                                 for eachToken in matching:
+#                                     startString = eachToken[:-1]
+#                                     startStringUnique = set(startString)
+#                                     if startStringUnique != set('*'):
+#                                         if word.lower().startswith(startString):
+
+#                                             appendLexiconLabel += lexiconName + tag.upper()
+#                                             matchedWord = True
+#                                     else:
+#                                         if eachToken == word.lower():
+
+#                                             appendLexiconLabel += lexiconName + tag.upper()
+#                                             matchedWord = True
+
+#                         elif word.lower() in tokens:
+
+#                             appendLexiconLabel += lexiconName + tag.upper()
+#                             matchedWord = True
+
+#                 collectMisspellingDetails['SubstitutionText'].append('MISSPELLING' + appendLexiconLabel)
+
+#             #print(appendLexiconLabel)
+#             collectMisspellingDetails['Word'].append(err.word)
+#             collectMisspellingDetails['Substitution'].append('ABCMISSPELLING' + str(len(collectMisspellingDetails['Word'])) + 'XYZ')
+
+#             if (len(err.suggest()) == 0):
+#                 spellingCorrectionDetailsSentences.append(sentence)
+#                 spellingCorrectionDetailsChangesWord.append('True')
+#                 spellingCorrectionDetailsWords.append(err.word)
+#                 spellingCorrectionDetailsSuggestions.append(' | '.join(err.suggest()))
+#                 spellingCorrectionDetailsChosenSuggestion.append('NA')
+#                 spellingCorrectionDetailsReplacementLength.append('NA')
+#             else: # no need to count case corrections (e.g., i'm = I'm), but go ahead and perform them
+#                 spellingCorrectionDetailsSentences.append(sentence)
+#                 spellingCorrectionDetailsWords.append(err.word)
+#                 spellingCorrectionDetailsSuggestions.append(' | '.join(err.suggest()))
+#                 if err.word.lower() != err.suggest()[0].lower():
+#                     spellingCorrectionDetailsChangesWord.append('True')
+#                     spellingCorrectionCount += 1
+#                 else:
+#                     spellingCorrectionDetailsChangesWord.append('False')
+
+#                 finalSuggestions = err.suggest()
+
+#                 err.replace(finalSuggestions[0])
+#                 spellingCorrectionDetailsChosenSuggestion.append(finalSuggestions[0])
+#                 spellingCorrectionDetailsReplacementLength.append(len(finalSuggestions[0].split()))
+
+#         sentenceMisspelling = sentence
+#         #print('\nRaw:', sentenceMisspelling)
+
+#         for i, word in enumerate(collectMisspellingDetails['Word']):
+
+#             replacementLength = spellingCorrectionDetailsReplacementLength[i]
+#             # if there is no suggested replacement
+#             if replacementLength == 'NA':
+#                 replacementLength = 1
+
+#             sentenceMisspelling = re.sub('(?<=[^a-zA-Z0-9])' + word + '(?![a-zA-Z0-9])', ' '.join([collectMisspellingDetails['Substitution'][i]] * replacementLength), sentenceMisspelling, count = 1)
+
+#         MisspellingRaw = ' '.join(spaCyTOK(sentenceMisspelling)).lower()
+
+#         Misspelling = re.sub('ABCMISSPELLING[0-9]+XYZ'.lower(), 'MISSPELLING', MisspellingRaw)
+
+#         if provideMisspellingDetailed == True:
+
+#             MisspellingDetailed = MisspellingRaw
+
+#             for i, word in enumerate(collectMisspellingDetails['Word']):
+
+#                 replacementLength = spellingCorrectionDetailsReplacementLength[i]
+#                 # if there is no suggested replacement
+#                 if replacementLength == 'NA':
+#                     replacementLength = 1
+
+#                 MisspellingDetailed = MisspellingDetailed.replace(collectMisspellingDetails['Substitution'][i].lower(), collectMisspellingDetails['SubstitutionText'][i], replacementLength)
+
+
+#             MisspellingDetailed = MisspellingDetailed
+
+#         #print('\nMISSPELLING Representation:', Misspelling)
+#         #print('\nMISSPELLINGDETAILED Representation:', MisspellingDetailed)
+
+#         if useSpellChecker:
+#             sentence = chkr.get_text()
+#             correctedSentence = sentence
+#         else:
+#             correctedSentence = chkr.get_text()
+
+#         #print('\nCorrected Sentence:', correctedSentence)
+
+#         checkLength = [
+#             len(spellingCorrectionDetailsSentences),
+#             len(spellingCorrectionDetailsWords),
+#             len(spellingCorrectionDetailsChangesWord),
+#             len(spellingCorrectionDetailsReplacementLength),
+#             len(spellingCorrectionDetailsSuggestions),
+#             len(spellingCorrectionDetailsChosenSuggestion)
+#             ]
+
+#         if debug:
+#             print('correctionDF:', checkLength)
+
+#         if not all(x == checkLength[0] for x in checkLength):
+#             print('\nProblem detected with the following text (spellchecker):', '\n')
+#             print(sentence)
+#             print(spellingCorrectionDetailsSuggestions)
+#             print(spellingCorrectionDetailsChosenSuggestion)
+#             print(spellingCorrectionDetailsReplacementLength)
+
+#         correctionDF = pd.DataFrame({
+#             #'RawInput': spellingCorrectionDetailsSentences,
+#             'RawWord': spellingCorrectionDetailsWords,
+#             'ChangesWord': spellingCorrectionDetailsChangesWord,
+#             'ReplacementLength': spellingCorrectionDetailsReplacementLength,
+#             'Suggestions': spellingCorrectionDetailsSuggestions,
+#             'ChosenSuggestion': spellingCorrectionDetailsChosenSuggestion
+#             })
+
+#         if debug:
+#             print('CorrectedSentence:', correctedSentence)
+#             print('CountStrippedWhitespaceChars:', whitespaceStripLength)
+#             print('CountStrippedHTMLChars:', htmlStripLength)
+#             print('CountSpellingCorrections', spellingCorrectionCount)
+#             print(correctionDF)
+
+#         resReturn = pd.DataFrame({
+#             'Sentence': sentence, 
+#             'Feature_Misspelling': Misspelling,
+#             'Spellchecker_CorrectedSentence': correctedSentence,
+#             'Spellchecker_CountStrippedWhitespaceChars': whitespaceStripLength,
+#             'Spellchecker_CountStrippedHTMLChars': htmlStripLength,
+#             'Spellchecker_CountSpellingCorrections': spellingCorrectionCount
+#             }, index = [0])
+
+#         if provideMisspellingDetailed:
+#             resReturn['Feature_MisspellingDetailed'] = MisspellingDetailed
+
+#         return([resReturn, correctionDF])
+
+#     # Basic Text Cleanup
+#     print('# Performing Basic Text Cleanup #\n')
+#     res = textData['InitialSentence'].mapply(BasicTextCleanup, debug = debug)
+#     resZip = list(zip(*res))
 
-        spellchecker = enchant.DictWithPWL(spellcheckerLibrary, pwl = exclusionsFileFullPath, broker = b)
-        chkr = SpellChecker(spellchecker, sentence, filters = [EmailFilter, URLFilter])
-
-        collectMisspellingDetails = {
-            'Word': [], 
-            'Substitution': [], 
-            'SubstitutionText': []
-            }
-
-        for err in chkr:
-
-            #print('\nSpellcheck Word:', err.word)
-            matchedWord = False
-
-            word = err.word
-
-            if lexicons is not None and provideMisspellingDetailed:
-
-                appendLexiconLabel = ''
-
-                for lexicon, tagTokenPairs in lexicons.items():
-
-                    lexiconName = '|_|' + lexicon.upper() + '&'
-
-                    matchedWord = False  # note: we want to capture in multiple lexicons (but only once per lexicon)
-
-                    for tag, tokens in tagTokenPairs.items():
-
-                        if matchedWord:
-                            break
-
-                        elif any('*' in s for s in tokens):
-                            # regex mode
-                            nonmatching = [s for s in tokens if not s.endswith('*')]
-                            if word.lower() in nonmatching:
-                                appendLexiconLabel += lexiconName + tag.upper()
-                                matchedWord = True
-                            else:
-                                matching = [s for s in tokens if s.endswith('*')]
-                                for eachToken in matching:
-                                    startString = eachToken[:-1]
-                                    startStringUnique = set(startString)
-                                    if startStringUnique != set('*'):
-                                        if word.lower().startswith(startString):
-
-                                            appendLexiconLabel += lexiconName + tag.upper()
-                                            matchedWord = True
-                                    else:
-                                        if eachToken == word.lower():
-
-                                            appendLexiconLabel += lexiconName + tag.upper()
-                                            matchedWord = True
-
-                        elif word.lower() in tokens:
-
-                            appendLexiconLabel += lexiconName + tag.upper()
-                            matchedWord = True
-
-                collectMisspellingDetails['SubstitutionText'].append('MISSPELLING' + appendLexiconLabel)
-
-            #print(appendLexiconLabel)
-            collectMisspellingDetails['Word'].append(err.word)
-            collectMisspellingDetails['Substitution'].append('ABCMISSPELLING' + str(len(collectMisspellingDetails['Word'])) + 'XYZ')
-
-            if (len(err.suggest()) == 0):
-                spellingCorrectionDetailsSentences.append(sentence)
-                spellingCorrectionDetailsChangesWord.append('True')
-                spellingCorrectionDetailsWords.append(err.word)
-                spellingCorrectionDetailsSuggestions.append(' | '.join(err.suggest()))
-                spellingCorrectionDetailsChosenSuggestion.append('NA')
-                spellingCorrectionDetailsReplacementLength.append('NA')
-            else: # no need to count case corrections (e.g., i'm = I'm), but go ahead and perform them
-                spellingCorrectionDetailsSentences.append(sentence)
-                spellingCorrectionDetailsWords.append(err.word)
-                spellingCorrectionDetailsSuggestions.append(' | '.join(err.suggest()))
-                if err.word.lower() != err.suggest()[0].lower():
-                    spellingCorrectionDetailsChangesWord.append('True')
-                    spellingCorrectionCount += 1
-                else:
-                    spellingCorrectionDetailsChangesWord.append('False')
-
-                finalSuggestions = err.suggest()
-
-                err.replace(finalSuggestions[0])
-                spellingCorrectionDetailsChosenSuggestion.append(finalSuggestions[0])
-                spellingCorrectionDetailsReplacementLength.append(len(finalSuggestions[0].split()))
-
-        sentenceMisspelling = sentence
-        #print('\nRaw:', sentenceMisspelling)
-
-        for i, word in enumerate(collectMisspellingDetails['Word']):
-
-            replacementLength = spellingCorrectionDetailsReplacementLength[i]
-            # if there is no suggested replacement
-            if replacementLength == 'NA':
-                replacementLength = 1
-
-            sentenceMisspelling = re.sub('(?<=[^a-zA-Z0-9])' + word + '(?![a-zA-Z0-9])', ' '.join([collectMisspellingDetails['Substitution'][i]] * replacementLength), sentenceMisspelling, count = 1)
-
-        MisspellingRaw = ' '.join(spaCyTOK(sentenceMisspelling)).lower()
-
-        Misspelling = re.sub('ABCMISSPELLING[0-9]+XYZ'.lower(), 'MISSPELLING', MisspellingRaw)
-
-        if provideMisspellingDetailed == True:
-
-            MisspellingDetailed = MisspellingRaw
-
-            for i, word in enumerate(collectMisspellingDetails['Word']):
-
-                replacementLength = spellingCorrectionDetailsReplacementLength[i]
-                # if there is no suggested replacement
-                if replacementLength == 'NA':
-                    replacementLength = 1
-
-                MisspellingDetailed = MisspellingDetailed.replace(collectMisspellingDetails['Substitution'][i].lower(), collectMisspellingDetails['SubstitutionText'][i], replacementLength)
-
-
-            MisspellingDetailed = MisspellingDetailed
-
-        #print('\nMISSPELLING Representation:', Misspelling)
-        #print('\nMISSPELLINGDETAILED Representation:', MisspellingDetailed)
-
-        if useSpellChecker:
-            sentence = chkr.get_text()
-            correctedSentence = sentence
-        else:
-            correctedSentence = chkr.get_text()
-
-        #print('\nCorrected Sentence:', correctedSentence)
-
-        checkLength = [
-            len(spellingCorrectionDetailsSentences),
-            len(spellingCorrectionDetailsWords),
-            len(spellingCorrectionDetailsChangesWord),
-            len(spellingCorrectionDetailsReplacementLength),
-            len(spellingCorrectionDetailsSuggestions),
-            len(spellingCorrectionDetailsChosenSuggestion)
-            ]
-
-        if debug:
-            print('correctionDF:', checkLength)
-
-        if not all(x == checkLength[0] for x in checkLength):
-            print('\nProblem detected with the following text (spellchecker):', '\n')
-            print(sentence)
-            print(spellingCorrectionDetailsSuggestions)
-            print(spellingCorrectionDetailsChosenSuggestion)
-            print(spellingCorrectionDetailsReplacementLength)
-
-        correctionDF = pd.DataFrame({
-            #'RawInput': spellingCorrectionDetailsSentences,
-            'RawWord': spellingCorrectionDetailsWords,
-            'ChangesWord': spellingCorrectionDetailsChangesWord,
-            'ReplacementLength': spellingCorrectionDetailsReplacementLength,
-            'Suggestions': spellingCorrectionDetailsSuggestions,
-            'ChosenSuggestion': spellingCorrectionDetailsChosenSuggestion
-            })
-
-        if debug:
-            print('CorrectedSentence:', correctedSentence)
-            print('CountStrippedWhitespaceChars:', whitespaceStripLength)
-            print('CountStrippedHTMLChars:', htmlStripLength)
-            print('CountSpellingCorrections', spellingCorrectionCount)
-            print(correctionDF)
-
-        resReturn = pd.DataFrame({
-            'Sentence': sentence, 
-            'Feature_Misspelling': Misspelling,
-            'Spellchecker_CorrectedSentence': correctedSentence,
-            'Spellchecker_CountStrippedWhitespaceChars': whitespaceStripLength,
-            'Spellchecker_CountStrippedHTMLChars': htmlStripLength,
-            'Spellchecker_CountSpellingCorrections': spellingCorrectionCount
-            }, index = [0])
-
-        if provideMisspellingDetailed:
-            resReturn['Feature_MisspellingDetailed'] = MisspellingDetailed
-
-        return([resReturn, correctionDF])
-
-    # Basic Text Cleanup
-    print('# Performing Basic Text Cleanup #\n')
-    res = textData['InitialSentence'].mapply(BasicTextCleanup, debug = debug)
-    resZip = list(zip(*res))
-
-    textData = pd.concat([textData, pd.concat(resZip[0], ignore_index = True)], axis = 1)
-    corrections = pd.concat(resZip[1], ignore_index = True)
+#     textData = pd.concat([textData, pd.concat(resZip[0], ignore_index = True)], axis = 1)
+#     corrections = pd.concat(resZip[1], ignore_index = True)
     
-    # Process Text with spaCy
-    print('\n# Processing Text Representations #\n')
-    def ProcessText (doc, debug = debug):
-
-        doc = nlp(doc)
-
-        all_word = []
-        all_word_lower = []
-        all_pos = []
-        all_word_pos = []
-        all_ner = []
-        all_word_ner = []
-        all_bounds = []
-
-        for token in doc:
-
-            word = token.text
-            pos = token.pos_
-
-            all_word.append(word)
-            all_word_lower.append(token.lower_)
-            all_pos.append(pos)
-            all_word_pos.append(token.lower_ + '|_|' + pos)
-
-            if token.ent_iob_ == "O":
-                ner = token.lower_
-                all_word_ner.append(token.lower_)
-            else:
-                ner = token.ent_type_
-                all_word_ner.append(token.lower_ + '|_|' + token.ent_type_)
-
-            all_ner.append(ner)
-
-        sents = doc.sents
-
-        for eachSent in sents:
-            sentBounds = ['-'] * len([token.text for token in eachSent])
-            sentBounds[-1] = 'S'
-            all_bounds += sentBounds
-
-        all_bounds = np.array(all_bounds)
-        all_bounds[np.where(np.array(all_word) == '|||')] = 'D'
-
-        # Vars
-        Word        = all_word_lower
-        POS         = all_pos
-        Word_POS    = all_word_pos
-        NER         = all_ner
-        Word_NER    = all_word_ner
-        Boundaries  = all_bounds
-
-        # Word Sense Disambiguation
-        tempWS = disambiguate(' '.join(all_word), algorithm = adapted_lesk, tokenizer = splitWS)
-        tempWSRaw = [x[1] for x in tempWS]
-
-        # Hypernym, Sentiment, Affect
-        Hypernym = []
-        Sentiment = []
-        Affect = []
-        Word_Sense = []
-
-        # for WNAffect
-        POSTreeBank = nltk.pos_tag(all_word)
-
-        for i, each in enumerate(Word):
-
-            try:
-                wnaRes = str(wna.get_emotion(Word[i], POSTreeBank[i][1]).get_level(wnaReturnLevel))
-                Affect.append(wnaRes.upper())
-            except:
-                Affect.append(Word[i])
-
-            if (str(tempWSRaw[i]) != 'None'):
-
-                Word_Sense.append(Word[i] + '|_|' + tempWS[i][1].name().split('.')[-1:][0])
-
-                hypernyms = tempWS[i][1].hypernyms()
-
-                if len(hypernyms) > 0:
-                    Hypernym.append(hypernyms[0].name().split('.')[0].upper())
-                else:
-                    Hypernym.append(Word[i])
-
-                swnScores = swn.senti_synset(tempWS[i][1].name())
-
-                wordSentiment = ''
-
-                if swnScores.pos_score() > 2/3:
-                    wordSentiment += 'HPOS'
-                elif swnScores.pos_score() > 1/3:
-                    wordSentiment += 'MPOS'
-                else:
-                    wordSentiment += 'LPOS'
-
-                if swnScores.neg_score() > 2/3:
-                    wordSentiment += 'HNEG'
-                elif swnScores.neg_score() > 1/3:
-                    wordSentiment += 'MNEG'
-                else:
-                    wordSentiment += 'LNEG'
-
-                Sentiment.append(wordSentiment)
-
-            else:
-                Word_Sense.append(Word[i])
-                Hypernym.append(Word[i])
-                Sentiment.append(Word[i])
-
-        res = {
-            'Feature_Word': all_word_lower,
-            'Feature_POS': all_pos,
-            'Feature_Word&POS': all_word_pos,
-            'Feature_NER': all_ner,
-            'Feature_Word&NER': all_word_ner,
-            'Feature_Boundaries': all_bounds,
-            'Feature_Affect': Affect,
-            'Feature_Word&Sense': Word_Sense,
-            'Feature_Hypernym': Hypernym,
-            'Feature_Sentiment': Sentiment,
-            }
+#     # Process Text with spaCy
+#     print('\n# Processing Text Representations #\n')
+#     def ProcessText (doc, debug = debug):
+
+#         doc = nlp(doc)
+
+#         all_word = []
+#         all_word_lower = []
+#         all_pos = []
+#         all_word_pos = []
+#         all_ner = []
+#         all_word_ner = []
+#         all_bounds = []
+
+#         for token in doc:
+
+#             word = token.text
+#             pos = token.pos_
+
+#             all_word.append(word)
+#             all_word_lower.append(token.lower_)
+#             all_pos.append(pos)
+#             all_word_pos.append(token.lower_ + '|_|' + pos)
+
+#             if token.ent_iob_ == "O":
+#                 ner = token.lower_
+#                 all_word_ner.append(token.lower_)
+#             else:
+#                 ner = token.ent_type_
+#                 all_word_ner.append(token.lower_ + '|_|' + token.ent_type_)
+
+#             all_ner.append(ner)
+
+#         sents = doc.sents
+
+#         for eachSent in sents:
+#             sentBounds = ['-'] * len([token.text for token in eachSent])
+#             sentBounds[-1] = 'S'
+#             all_bounds += sentBounds
+
+#         all_bounds = np.array(all_bounds)
+#         all_bounds[np.where(np.array(all_word) == '|||')] = 'D'
+
+#         # Vars
+#         Word        = all_word_lower
+#         POS         = all_pos
+#         Word_POS    = all_word_pos
+#         NER         = all_ner
+#         Word_NER    = all_word_ner
+#         Boundaries  = all_bounds
+
+#         # Word Sense Disambiguation
+#         tempWS = disambiguate(' '.join(all_word), algorithm = adapted_lesk, tokenizer = splitWS)
+#         tempWSRaw = [x[1] for x in tempWS]
+
+#         # Hypernym, Sentiment, Affect
+#         Hypernym = []
+#         Sentiment = []
+#         Affect = []
+#         Word_Sense = []
+
+#         # for WNAffect
+#         POSTreeBank = nltk.pos_tag(all_word)
+
+#         for i, each in enumerate(Word):
+
+#             try:
+#                 wnaRes = str(wna.get_emotion(Word[i], POSTreeBank[i][1]).get_level(wnaReturnLevel))
+#                 Affect.append(wnaRes.upper())
+#             except:
+#                 Affect.append(Word[i])
+
+#             if (str(tempWSRaw[i]) != 'None'):
+
+#                 Word_Sense.append(Word[i] + '|_|' + tempWS[i][1].name().split('.')[-1:][0])
+
+#                 hypernyms = tempWS[i][1].hypernyms()
+
+#                 if len(hypernyms) > 0:
+#                     Hypernym.append(hypernyms[0].name().split('.')[0].upper())
+#                 else:
+#                     Hypernym.append(Word[i])
+
+#                 swnScores = swn.senti_synset(tempWS[i][1].name())
+
+#                 wordSentiment = ''
+
+#                 if swnScores.pos_score() > 2/3:
+#                     wordSentiment += 'HPOS'
+#                 elif swnScores.pos_score() > 1/3:
+#                     wordSentiment += 'MPOS'
+#                 else:
+#                     wordSentiment += 'LPOS'
+
+#                 if swnScores.neg_score() > 2/3:
+#                     wordSentiment += 'HNEG'
+#                 elif swnScores.neg_score() > 1/3:
+#                     wordSentiment += 'MNEG'
+#                 else:
+#                     wordSentiment += 'LNEG'
+
+#                 Sentiment.append(wordSentiment)
+
+#             else:
+#                 Word_Sense.append(Word[i])
+#                 Hypernym.append(Word[i])
+#                 Sentiment.append(Word[i])
+
+#         res = {
+#             'Feature_Word': all_word_lower,
+#             'Feature_POS': all_pos,
+#             'Feature_Word&POS': all_word_pos,
+#             'Feature_NER': all_ner,
+#             'Feature_Word&NER': all_word_ner,
+#             'Feature_Boundaries': all_bounds,
+#             'Feature_Affect': Affect,
+#             'Feature_Word&Sense': Word_Sense,
+#             'Feature_Hypernym': Hypernym,
+#             'Feature_Sentiment': Sentiment,
+#             }
         
-        # Generate separate lexicon features (if available)
-        LexiconFeatures = {}
+#         # Generate separate lexicon features (if available)
+#         LexiconFeatures = {}
 
-        if lexicons is not None:
+#         if lexicons is not None:
 
-            for lexicon, tagTokenPairs in lexicons.items():
+#             for lexicon, tagTokenPairs in lexicons.items():
 
-                lexiconName = 'Feature_Lexicon' + lexicon.upper()
-                LexiconFeatures[lexiconName] = []
-
-                for i, word in enumerate(Word):
-
-                    LexiconFeatures[lexiconName].append(word)
-                    wordReplaced = False
-
-                    for tag, tokens in tagTokenPairs.items():
-                        if wordReplaced:
-                            break
-                        elif any('*' in s for s in tokens):
-                            # regex mode
-                            nonmatching = [s for s in tokens if not s.endswith('*')]
-                            if word.lower() in nonmatching:
-                                LexiconFeatures[lexiconName][i] = tag.upper()
-                                wordReplaced = True
-                            else:
-                                matching = [s for s in tokens if s.endswith('*')]
-                                for eachToken in matching:
-                                    startString = eachToken[:-1]
-                                    startStringUnique = set(startString)
-                                    if startStringUnique != set('*'):
-                                        if word.lower().startswith(startString):
-                                            LexiconFeatures[lexiconName][i] = tag.upper()
-                                            matchedWord = True
-                                    else:
-                                        if eachToken == word.lower():
-                                            LexiconFeatures[lexiconName][i] = tag.upper()
-                                            matchedWord = True
-
-                        elif word.lower() in tokens:
-
-                            LexiconFeatures[lexiconName][i] = tag.upper()
-                            wordReplaced = True
-
-        if lexicons is not None:
-            res.update(LexiconFeatures)
-
-        checkLength = [len(res[each]) for each in res]
-
-        if len(set(checkLength)) != 1:
-            print('Check Length:', checkLength)
-            print('Problem detected with the following text:')
-            print(sentence)
-
-        # Rejoin features
-        for each in res.keys():
-            res[each] = ' '.join(res[each])
+#                 lexiconName = 'Feature_Lexicon' + lexicon.upper()
+#                 LexiconFeatures[lexiconName] = []
+
+#                 for i, word in enumerate(Word):
+
+#                     LexiconFeatures[lexiconName].append(word)
+#                     wordReplaced = False
+
+#                     for tag, tokens in tagTokenPairs.items():
+#                         if wordReplaced:
+#                             break
+#                         elif any('*' in s for s in tokens):
+#                             # regex mode
+#                             nonmatching = [s for s in tokens if not s.endswith('*')]
+#                             if word.lower() in nonmatching:
+#                                 LexiconFeatures[lexiconName][i] = tag.upper()
+#                                 wordReplaced = True
+#                             else:
+#                                 matching = [s for s in tokens if s.endswith('*')]
+#                                 for eachToken in matching:
+#                                     startString = eachToken[:-1]
+#                                     startStringUnique = set(startString)
+#                                     if startStringUnique != set('*'):
+#                                         if word.lower().startswith(startString):
+#                                             LexiconFeatures[lexiconName][i] = tag.upper()
+#                                             matchedWord = True
+#                                     else:
+#                                         if eachToken == word.lower():
+#                                             LexiconFeatures[lexiconName][i] = tag.upper()
+#                                             matchedWord = True
+
+#                         elif word.lower() in tokens:
+
+#                             LexiconFeatures[lexiconName][i] = tag.upper()
+#                             wordReplaced = True
+
+#         if lexicons is not None:
+#             res.update(LexiconFeatures)
+
+#         checkLength = [len(res[each]) for each in res]
+
+#         if len(set(checkLength)) != 1:
+#             print('Check Length:', checkLength)
+#             print('Problem detected with the following text:')
+#             print(sentence)
+
+#         # Rejoin features
+#         for each in res.keys():
+#             res[each] = ' '.join(res[each])
 
-        return(res)
+#         return(res)
 
-    res = textData['Sentence'].mapply(ProcessText)
-    textData = pd.concat([textData, pd.DataFrame(res.values.tolist())], axis = 1)
+#     res = textData['Sentence'].mapply(ProcessText)
+#     textData = pd.concat([textData, pd.DataFrame(res.values.tolist())], axis = 1)
 
-    return([textData, corrections])
+#     return([textData, corrections])
```

### Comparing `textagon-0.1.8/textagon.egg-info/SOURCES.txt` & `textagon-0.1.9/textagon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

