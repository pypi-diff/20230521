# Comparing `tmp/vocabtrimmer-0.0.1.tar.gz` & `tmp/vocabtrimmer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocabtrimmer-0.0.1.tar", last modified: Sat Mar 11 09:20:22 2023, max compression
+gzip compressed data, was "vocabtrimmer-0.0.2.tar", last modified: Sun May 21 18:55:02 2023, max compression
```

## Comparing `vocabtrimmer-0.0.1.tar` & `vocabtrimmer-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-03-11 09:20:22.614832 vocabtrimmer-0.0.1/
--rw-r--r--   0 asahi      (501) staff       (20)     1560 2023-03-11 09:20:22.615079 vocabtrimmer-0.0.1/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)      756 2023-03-11 09:20:08.000000 vocabtrimmer-0.0.1/README.md
--rw-r--r--   0 asahi      (501) staff       (20)       38 2023-03-11 09:20:22.615758 vocabtrimmer-0.0.1/setup.cfg
--rw-r--r--   0 asahi      (501) staff       (20)     1767 2023-03-11 09:19:55.000000 vocabtrimmer-0.0.1/setup.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-03-11 09:20:22.608965 vocabtrimmer-0.0.1/vocabtrimmer/
--rw-r--r--   0 asahi      (501) staff       (20)       76 2023-03-01 17:54:43.000000 vocabtrimmer-0.0.1/vocabtrimmer/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)    14024 2023-03-04 11:29:34.000000 vocabtrimmer-0.0.1/vocabtrimmer/base_trimmer.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-03-11 09:20:22.613874 vocabtrimmer-0.0.1/vocabtrimmer/cl/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2023-02-27 12:02:07.000000 vocabtrimmer-0.0.1/vocabtrimmer/cl/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     2675 2023-03-04 11:29:42.000000 vocabtrimmer-0.0.1/vocabtrimmer/cl/trimming.py
--rw-r--r--   0 asahi      (501) staff       (20)      401 2023-03-01 15:27:53.000000 vocabtrimmer-0.0.1/vocabtrimmer/util.py
--rw-r--r--   0 asahi      (501) staff       (20)     9939 2023-03-04 11:29:23.000000 vocabtrimmer-0.0.1/vocabtrimmer/vocab_miner.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-03-11 09:20:22.612862 vocabtrimmer-0.0.1/vocabtrimmer.egg-info/
--rw-r--r--   0 asahi      (501) staff       (20)     1560 2023-03-11 09:20:22.000000 vocabtrimmer-0.0.1/vocabtrimmer.egg-info/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)      405 2023-03-11 09:20:22.000000 vocabtrimmer-0.0.1/vocabtrimmer.egg-info/SOURCES.txt
--rw-r--r--   0 asahi      (501) staff       (20)        1 2023-03-11 09:20:22.000000 vocabtrimmer-0.0.1/vocabtrimmer.egg-info/dependency_links.txt
--rw-r--r--   0 asahi      (501) staff       (20)       73 2023-03-11 09:20:22.000000 vocabtrimmer-0.0.1/vocabtrimmer.egg-info/entry_points.txt
--rw-r--r--   0 asahi      (501) staff       (20)       58 2023-03-11 09:20:22.000000 vocabtrimmer-0.0.1/vocabtrimmer.egg-info/requires.txt
--rw-r--r--   0 asahi      (501) staff       (20)       13 2023-03-11 09:20:22.000000 vocabtrimmer-0.0.1/vocabtrimmer.egg-info/top_level.txt
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-21 18:55:01.997465 vocabtrimmer-0.0.2/
+-rw-r--r--   0 asahi      (501) staff       (20)     1064 2023-05-21 13:09:58.000000 vocabtrimmer-0.0.2/LICENSE
+-rw-r--r--   0 asahi      (501) staff       (20)     6321 2023-05-21 18:55:01.997676 vocabtrimmer-0.0.2/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)     5495 2023-05-21 18:54:56.000000 vocabtrimmer-0.0.2/README.md
+-rw-r--r--   0 asahi      (501) staff       (20)       38 2023-05-21 18:55:01.998234 vocabtrimmer-0.0.2/setup.cfg
+-rw-r--r--   0 asahi      (501) staff       (20)     1776 2023-05-21 18:07:16.000000 vocabtrimmer-0.0.2/setup.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-21 18:55:01.992412 vocabtrimmer-0.0.2/vocabtrimmer/
+-rw-r--r--   0 asahi      (501) staff       (20)       76 2023-03-01 17:54:43.000000 vocabtrimmer-0.0.2/vocabtrimmer/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)    14669 2023-05-21 18:06:51.000000 vocabtrimmer-0.0.2/vocabtrimmer/base_trimmer.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-21 18:55:01.996608 vocabtrimmer-0.0.2/vocabtrimmer/cl/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2023-02-27 12:02:07.000000 vocabtrimmer-0.0.2/vocabtrimmer/cl/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2778 2023-03-14 17:05:00.000000 vocabtrimmer-0.0.2/vocabtrimmer/cl/trimming.py
+-rw-r--r--   0 asahi      (501) staff       (20)      401 2023-03-01 15:27:53.000000 vocabtrimmer-0.0.2/vocabtrimmer/util.py
+-rw-r--r--   0 asahi      (501) staff       (20)     4269 2023-03-14 17:01:50.000000 vocabtrimmer-0.0.2/vocabtrimmer/vocab_miner.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-21 18:55:01.996087 vocabtrimmer-0.0.2/vocabtrimmer.egg-info/
+-rw-r--r--   0 asahi      (501) staff       (20)     6321 2023-05-21 18:55:01.000000 vocabtrimmer-0.0.2/vocabtrimmer.egg-info/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)      413 2023-05-21 18:55:01.000000 vocabtrimmer-0.0.2/vocabtrimmer.egg-info/SOURCES.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        1 2023-05-21 18:55:01.000000 vocabtrimmer-0.0.2/vocabtrimmer.egg-info/dependency_links.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       73 2023-05-21 18:55:01.000000 vocabtrimmer-0.0.2/vocabtrimmer.egg-info/entry_points.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       58 2023-05-21 18:55:01.000000 vocabtrimmer-0.0.2/vocabtrimmer.egg-info/requires.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       13 2023-05-21 18:55:01.000000 vocabtrimmer-0.0.2/vocabtrimmer.egg-info/top_level.txt
```

### Comparing `vocabtrimmer-0.0.1/setup.py` & `vocabtrimmer-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 NAME = 'vocabtrimmer'
 LICENSE = 'MIT License'
 setup(
     name=NAME,
-    packages=find_packages(exclude=['tests', 'misc', 'asset', "experiments", "hf_operations", "metric_files"]),
+    packages=find_packages(exclude=['assets','tests', 'misc', 'asset', "experiments", "hf_operations", "metric_files"]),
     version=VERSION,
     license=LICENSE,
     description='Trimming vocabulary of pre-trained multilingual language models to language localization.',
     url='https://github.com/asahi417/lm-vocab-trmmer',
     download_url="https://github.com/asahi417/lm-vocab-trmmer/archive/v{}.tar.gz".format(VERSION),
     keywords=['language model', 't5', 'gpt3', 'bert' 'nlp', 'multilingual', 'efficient-model'],
     long_description=readme,
```

### Comparing `vocabtrimmer-0.0.1/vocabtrimmer/base_trimmer.py` & `vocabtrimmer-0.0.2/vocabtrimmer/base_trimmer.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 os.environ["OMP_NUM_THREADS"] = "1"  # to turn off warning message
 os.environ["TOKENIZERS_PARALLELISM"] = "false"  # to turn off warning message
 MBART_LANG_ID = ['ar_AR', 'cs_CZ', 'de_DE', 'en_XX', 'es_XX', 'et_EE', 'fi_FI', 'fr_XX', 'gu_IN', 'hi_IN', 'it_IT',
                  'ja_XX', 'kk_KZ', 'ko_KR', 'lt_LT', 'lv_LV', 'my_MM', 'ne_NP', 'nl_XX', 'ro_RO', 'ru_RU', 'si_LK',
                  'tr_TR', 'vi_VN', 'zh_CN']
 
 
-def show_parameter(target_model, log: bool = False, is_encoder_decoder: bool = True):
+def show_parameter(target_model, log: bool = False, double_embedding: bool = True):
     param_size_embedding = prod(target_model.get_input_embeddings().weight.shape)
-    if is_encoder_decoder:
+    if double_embedding:
         param_size_embedding = param_size_embedding * 2
     param_size_full = sum(p.numel() for p in target_model.parameters())
     vocab_size = len(target_model.get_input_embeddings().weight)
 
     func = logging.info if log else print
     func(f"PARAMETER SUMMARY")
     func(f"\t*parameter size (full) : {pretty(param_size_full)}")
@@ -86,33 +86,36 @@
     model.save_pretrained(path_to_save)
     tokenizer.save_pretrained(path_to_save)
 
 
 class VocabTrimmer:
     """ Vocabulary trimming for language localization of multilingual LM """
 
-    def __init__(self, model_name: str):
+    def __init__(self, model_name: str, double_embedding: bool = None):
         """ Vocabulary trimming for language localization of multilingual LM
 
         :param model_name: model name on huggingface or path to local model
+        :param double_embedding: (this is only for log) double the number of embedding or not
         """
         # load model
         self.model_name = model_name
         self.tokenizer = AutoTokenizer.from_pretrained(model_name)
         self.config = AutoConfig.from_pretrained(model_name)
+        if double_embedding is None:
+            self.double_embedding = True if self.config.model_type in ['mt5'] else False
+        else:
+            self.double_embedding = double_embedding
         if self.config.model_type in ['mt5', 'mbart']:
             logging.info("model is encoder-decoder LM")
-            self.is_encoder_decoder = True
             if self.config.model_type == 'mbart':
                 self.__model_class = MBartForConditionalGeneration
             else:
                 self.__model_class = MT5ForConditionalGeneration
         else:
             logging.info("model is masked LM")
-            self.is_encoder_decoder = False
             if self.config.architectures[0].endswith("TokenClassification"):
                 self.__model_class = AutoModelForTokenClassification
             elif self.config.architectures[0].endswith("SequenceClassification"):
                 self.__model_class = AutoModelForSequenceClassification
             elif self.config.architectures[0].endswith("MaskedLM"):
                 self.__model_class = AutoModelForMaskedLM
             else:
@@ -137,20 +140,20 @@
     def token_classification(self, input_text: str):
         return pipeline("token-classification", model=self.model, tokenizer=self.tokenizer)(input_text)
 
     def fill_mask(self, input_text: str):
         return pipeline("fill-mask", model=self.model, tokenizer=self.tokenizer)(input_text)
 
     def show_parameter(self, log: bool = False):
-        return show_parameter(self.model, is_encoder_decoder=self.is_encoder_decoder, log=log)
+        return show_parameter(self.model, double_embedding=self.double_embedding, log=log)
 
-    def trim_vocab(self, language: str, path_to_save: str, dataset: str = 'mc4', dataset_column: str = 'text',
-                   dataset_name: str = None, dataset_split: str = 'train', tokens_to_keep: List = None,
-                   target_vocab_size: int = None, min_frequency: int = 2, chunk: int = 1000,
-                   cache_file_vocab: str = None, cache_file_frequency: str = None):
+    def trim_vocab(self, language: str, path_to_save: str, dataset: str = 'vocabtrimmer/mc4_validation', dataset_column: str = 'text',
+                   dataset_name: str = None, dataset_split: str = 'validation', tokens_to_keep: List = None,
+                   target_vocab_size: int = None, min_frequency: int = 2, chunk: int = 500,
+                   cache_file_vocab: str = None, cache_file_frequency: str = None, overwrite: bool = False):
         """ Vocabulary trimming along with vocabulary mining on corpus
 
         :param path_to_save: directly to save model
         :param language: language code of tokens to keep
         :param dataset: huggingface dataset to be used for mining
         :param dataset_column: column of the dataset containing text for mining
         :param dataset_name: name of the dataset
@@ -172,15 +175,16 @@
             dataset_column=dataset_column,
             dataset_name=dataset_name,
             dataset_split=dataset_split,
             target_vocab_size=target_vocab_size,
             min_frequency=min_frequency,
             chunk=chunk,
             cache_file_frequency=cache_file_frequency,
-            cache_file_vocab=cache_file_vocab
+            cache_file_vocab=cache_file_vocab,
+            overwrite=overwrite
         )
 
         vocab = dict(zip(self.tokenizer.all_special_tokens, self.tokenizer.all_special_ids))
         vocab.update(new_vocab)
         if tokens_to_keep is not None:
             vocab.update({i: self.tokenizer.vocab[i] for i in tokens_to_keep})
         new_vocab_id = sorted(vocab.values())
@@ -242,15 +246,19 @@
         self.tokenizer.backend_tokenizer.model = model_class(**model_state)
 
         # update additional tokens (tokens added after pre-training won't be re-indexed above so need a dirty hack)
         additional_special_tokens = [i for i in self.tokenizer.additional_special_tokens if i not in MBART_LANG_ID]
         if len(additional_special_tokens) != 0:
             logging.info(f"updating additional_special_tokens of tokenizer")
             logging.info(f"num of add tokens: {len(additional_special_tokens)}")
-            last_id = len(self.tokenizer.vocab) - 1 - len(additional_special_tokens)
+            if self.config.model_type == 'mbart':  # lang_ids are added to tokenizer when it's instantiated
+                will_append_ids = [x for x in MBART_LANG_ID if x not in self.tokenizer.vocab]
+                last_id = len(self.tokenizer.vocab) - 1 - len(additional_special_tokens) + len(will_append_ids)
+            else:
+                last_id = len(self.tokenizer.vocab) - 1 - len(additional_special_tokens)
             new_sp_token_index = {v: n + last_id + 1 for n, v in enumerate(additional_special_tokens)}
             _, _, _, path_added_token, _ = self.tokenizer.save_pretrained(path_to_save)
             with open(path_added_token, 'w') as f:
                 json.dump(new_sp_token_index, f)
             self.tokenizer = AutoTokenizer.from_pretrained(path_to_save)
 
         # update config
```

### Comparing `vocabtrimmer-0.0.1/vocabtrimmer/cl/trimming.py` & `vocabtrimmer-0.0.2/vocabtrimmer/cl/trimming.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     parser.add_argument('-s', '--dataset-split', help='split of the dataset', default='validation', type=str)
     parser.add_argument('--dataset-column', help="column of the dataset containing text for mining", default='text', type=str)
     parser.add_argument('--cache-file-vocab', help="cache directly to save the mined vocab", default=None, type=str)
     parser.add_argument('--cache-file-frequency', help="cache directly to save the frequency over the corpus used for vocab mining", default=None, type=str)
     parser.add_argument('--min-frequency', help="min frequency of tokens", default=2, type=int)
     parser.add_argument('--tokens-to-keep', help='custom tokens to keep in vocabulary', nargs='+', default=None, type=str)
 
+    parser.add_argument('--overwrite', help='', action='store_true')
+
     opt = parser.parse_args()
 
     # trimming
     trimmer = vocabtrimmer.VocabTrimmer(opt.model)
     trimmer.trim_vocab(
         path_to_save=opt.path_to_save,
         language=opt.language,
@@ -39,14 +41,15 @@
         dataset_column=opt.dataset_column,
         dataset_name=opt.dataset_name,
         dataset_split=opt.dataset_split,
         target_vocab_size=opt.target_vocab_size,
         min_frequency=opt.min_frequency,
         chunk=opt.chunk,
         cache_file_vocab=opt.cache_file_vocab,
-        cache_file_frequency=opt.cache_file_frequency
+        cache_file_frequency=opt.cache_file_frequency,
+        overwrite=opt.overwrite
     )
 
     # push to huggingface
     if opt.repo_id is not None:
         logging.info(f"pushing to {opt.repo_id}")
         trimmer.push_to_hub(opt.repo_id)
```

