# Comparing `tmp/text2phonemesequence-0.0.5.tar.gz` & `tmp/text2phonemesequence-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/text2phonemesequence-0.0.5.tar", last modified: Sat May 20 04:32:27 2023, max compression
+gzip compressed data, was "dist/text2phonemesequence-0.0.6.tar", last modified: Sun May 21 16:58:08 2023, max compression
```

## Comparing `text2phonemesequence-0.0.5.tar` & `text2phonemesequence-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-20 04:32:27.000000 text2phonemesequence-0.0.5/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2640 2023-05-20 04:32:27.000000 text2phonemesequence-0.0.5/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1777 2023-05-19 09:33:26.000000 text2phonemesequence-0.0.5/README.md
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-05-20 04:32:27.000000 text2phonemesequence-0.0.5/setup.cfg
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.0.5/setup.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-20 04:32:27.000000 text2phonemesequence-0.0.5/text2phonemesequence/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-05-19 10:20:06.000000 text2phonemesequence-0.0.5/text2phonemesequence/__init__.py
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     7125 2023-05-20 04:30:22.000000 text2phonemesequence-0.0.5/text2phonemesequence/text2phonemesequence.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-20 04:32:27.000000 text2phonemesequence-0.0.5/text2phonemesequence.egg-info/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2640 2023-05-20 04:32:26.000000 text2phonemesequence-0.0.5/text2phonemesequence.egg-info/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-05-20 04:32:26.000000 text2phonemesequence-0.0.5/text2phonemesequence.egg-info/SOURCES.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-05-20 04:32:26.000000 text2phonemesequence-0.0.5/text2phonemesequence.egg-info/dependency_links.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-05-20 04:32:26.000000 text2phonemesequence-0.0.5/text2phonemesequence.egg-info/requires.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-05-20 04:32:26.000000 text2phonemesequence-0.0.5/text2phonemesequence.egg-info/top_level.txt
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2640 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1777 2023-05-20 04:58:56.000000 text2phonemesequence-0.0.6/README.md
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/setup.cfg
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.0.6/setup.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-05-21 16:57:44.000000 text2phonemesequence-0.0.6/text2phonemesequence/__init__.py
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     7251 2023-05-21 16:52:00.000000 text2phonemesequence-0.0.6/text2phonemesequence/text2phonemesequence.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence.egg-info/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2640 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence.egg-info/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence.egg-info/requires.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence.egg-info/top_level.txt
```

### Comparing `text2phonemesequence-0.0.5/PKG-INFO` & `text2phonemesequence-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
@@ -22,15 +22,15 @@
         ## Usage example <a name="example"></a>
         The library uses CharsiuG2P to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
         
         ```python
         from text2phonemesequence import Text2PhonemeSequence
         
         # Load Text2PhonemeSequence
-        model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-uk', is_cuda=False)
+        model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
         
         
         # Convert a raw corpus
         model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
         
         # Convert a raw sentence
         model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
```

### Comparing `text2phonemesequence-0.0.5/README.md` & `text2phonemesequence-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ## Usage example <a name="example"></a>
 The library uses CharsiuG2P to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
 
 ```python
 from text2phonemesequence import Text2PhonemeSequence
 
 # Load Text2PhonemeSequence
-model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-uk', is_cuda=False)
+model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
 
 
 # Convert a raw corpus
 model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
 
 # Convert a raw sentence
 model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
```

### Comparing `text2phonemesequence-0.0.5/setup.py` & `text2phonemesequence-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.0.5/text2phonemesequence/text2phonemesequence.py` & `text2phonemesequence-0.0.6/text2phonemesequence/text2phonemesequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from transformers import T5ForConditionalGeneration, AutoTokenizer
 from segments import Tokenizer
 import os
 from tqdm import tqdm
 
-
-
 class Text2PhonemeSequence:
     def __init__(self, pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='vie-c', is_cuda=True):
         self.tokenizer = AutoTokenizer.from_pretrained('google/byt5-small')
         self.model = T5ForConditionalGeneration.from_pretrained(pretrained_g2p_model)
         self.is_cuda = is_cuda
         if self.is_cuda:
             self.model = model.cuda()
@@ -34,15 +32,15 @@
     def infer_dataset(self, input_file='', seperate_syllabel_token= "_", output_file=""):
         f = open(input_file, 'r')
         list_lines = f.readlines()
         f.close()
         list_words = []
         print("Building vocabulary!")
         for line in list_lines:
-            words = line.strip().split(" ")
+            words = line.strip().split("|")[-1].split(" ")
             for w in words:
                 w = w.replace(seperate_syllabel_token, " ").lower()
                 if w not in self.phone_dict.keys():
                     list_words.append(w)
         list_words_p = ['<' + self.language + '>: ' + i for i in list_words]
         out = self.tokenizer(list_words_p, padding=True, add_special_tokens=False, return_tensors='pt')
         if self.is_cuda:
@@ -65,18 +63,20 @@
             self.phone_dict[w].append(segmented_phone)
         
         f = open(input_file, 'r')
         list_lines = f.readlines()
         f.close()
         f = open(output_file, 'w')
         for line in tqdm(list_lines):
-            line = line.strip().split(" ")
-            for i in range(len(line)):
-                line[i] = self.phone_dict[line[i].replace(seperate_syllabel_token, " ").lower()][1]
-            f.write(" ▁ ".join(line))
+            line = line.strip().split("|")
+            prefix = line[0]
+            list_words = line[-1].split(" ")
+            for i in range(len(list_words)):
+                list_words[i] = self.phone_dict[list_words[i].replace(seperate_syllabel_token, " ").lower()][1]
+            f.write(prefix + "|" + " ▁ ".join(list_words))
             f.write("\n")
         f.close()
     
     def infer_sentence(self, sentence="", seperate_syllabel_token="_"):
         list_words = sentence.split(" ")
         list_phones = []
         for i in range(len(list_words)):
```

### Comparing `text2phonemesequence-0.0.5/text2phonemesequence.egg-info/PKG-INFO` & `text2phonemesequence-0.0.6/text2phonemesequence.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
@@ -22,15 +22,15 @@
         ## Usage example <a name="example"></a>
         The library uses CharsiuG2P to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
         
         ```python
         from text2phonemesequence import Text2PhonemeSequence
         
         # Load Text2PhonemeSequence
-        model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-uk', is_cuda=False)
+        model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
         
         
         # Convert a raw corpus
         model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
         
         # Convert a raw sentence
         model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
```

