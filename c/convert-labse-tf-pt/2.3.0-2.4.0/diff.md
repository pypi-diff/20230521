# Comparing `tmp/convert_labse_tf_pt-2.3.0.tar.gz` & `tmp/convert_labse_tf_pt-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert_labse_tf_pt-2.3.0.tar", max compression
+gzip compressed data, was "convert_labse_tf_pt-2.4.0.tar", max compression
```

## Comparing `convert_labse_tf_pt-2.3.0.tar` & `convert_labse_tf_pt-2.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-05-21 08:41:13.624773 convert_labse_tf_pt-2.3.0/LICENSE
--rw-r--r--   0        0        0     1384 2023-05-21 08:41:13.624773 convert_labse_tf_pt-2.3.0/README.md
--rw-r--r--   0        0        0     1175 2023-05-21 08:41:13.624773 convert_labse_tf_pt-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      315 2023-05-21 08:41:13.624773 convert_labse_tf_pt-2.3.0/src/convert_labse_tf_pt/__init__.py
--rw-r--r--   0        0        0     2081 2023-05-21 08:41:13.624773 convert_labse_tf_pt-2.3.0/src/convert_labse_tf_pt/configurations.py
--rw-r--r--   0        0        0    17891 2023-05-21 08:41:13.624773 convert_labse_tf_pt-2.3.0/src/convert_labse_tf_pt/convert.py
--rw-r--r--   0        0        0  5220781 2023-05-21 08:41:13.664774 convert_labse_tf_pt-2.3.0/src/convert_labse_tf_pt/data/labse_vocab/cased_vocab.txt
--rw-r--r--   0        0        0  1469057 2023-05-21 08:41:13.676774 convert_labse_tf_pt-2.3.0/src/convert_labse_tf_pt/data/smaller_vocab/vocab-en-fr-es-de-zh-ar-zh_classical-it-ja-ko-nl-pl-pt-th-tr-ru.txt
--rw-r--r--   0        0        0     2280 1970-01-01 00:00:00.000000 convert_labse_tf_pt-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-21 08:41:17.652723 convert_labse_tf_pt-2.4.0/LICENSE
+-rw-r--r--   0        0        0     1384 2023-05-21 08:41:17.652723 convert_labse_tf_pt-2.4.0/README.md
+-rw-r--r--   0        0        0     1198 2023-05-21 08:41:17.656723 convert_labse_tf_pt-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      315 2023-05-21 08:41:17.656723 convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/__init__.py
+-rw-r--r--   0        0        0     2081 2023-05-21 08:41:17.656723 convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/configurations.py
+-rw-r--r--   0        0        0    18478 2023-05-21 08:41:17.656723 convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/convert.py
+-rw-r--r--   0        0        0  5220781 2023-05-21 08:41:17.700724 convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/data/labse_vocab/cased_vocab.txt
+-rw-r--r--   0        0        0  1469057 2023-05-21 08:41:17.708724 convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/data/smaller_vocab/vocab-en-fr-es-de-zh-ar-zh_classical-it-ja-ko-nl-pl-pt-th-tr-ru.txt
+-rw-r--r--   0        0        0     2324 1970-01-01 00:00:00.000000 convert_labse_tf_pt-2.4.0/PKG-INFO
```

### Comparing `convert_labse_tf_pt-2.3.0/LICENSE` & `convert_labse_tf_pt-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `convert_labse_tf_pt-2.3.0/README.md` & `convert_labse_tf_pt-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `convert_labse_tf_pt-2.3.0/pyproject.toml` & `convert_labse_tf_pt-2.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "convert-labse-tf-pt"
-version = "2.3.0"
+version = "2.4.0"
 description = "Convert LaBSE model from TensorFlow to PyTorch."
 license = "MIT"
 authors = ["Setu Shah <setu+labse@setu.me>"]
 readme = "README.md"
 homepage = "https://github.com/setu4993/convert-labse-tf-pt"
 repository = "https://github.com/setu4993/convert-labse-tf-pt"
 keywords = ["transformers", "bert", "labse", "pytorch", "tensorflow"]
@@ -13,14 +13,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.11"
 transformers = { extras = ["flax", "sentencepiece", "torch", "tf"], version = "^4.29.0" }
 tensorflow-hub = "^0.12.0"
 ipywidgets = "^7.6.3"
 loguru = "^0.6.0"
+safetensors = "^0.3.1"
 
 [tool.poetry.scripts]
 convert_labse = "convert_labse_tf_pt.convert:convert_labse"
 convert_lealla = "convert_labse_tf_pt.convert:convert_lealla"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.0"
```

### Comparing `convert_labse_tf_pt-2.3.0/src/convert_labse_tf_pt/configurations.py` & `convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/configurations.py`

 * *Files identical despite different names*

### Comparing `convert_labse_tf_pt-2.3.0/src/convert_labse_tf_pt/convert.py` & `convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     )
 
 
 def save_labse_models(
     model: BertModel,
     tokenizer: BertTokenizerFast,
     output_path: PATH,
+    save_safe_tensor: bool = True,
     save_tokenizer: bool = True,
     save_tf: bool = True,
     save_flax: bool = True,
     huggingface_path: bool = False,
 ):
     output_path = Path(output_path) if isinstance(output_path, str) else output_path
 
@@ -78,14 +79,24 @@
 
     if save_tokenizer:
         tokenizer_output_path = output_path.joinpath("tokenizer") if not huggingface_path else output_path
         tokenizer_output_path.mkdir(exist_ok=True, parents=True)
         tokenizer.save_pretrained(tokenizer_output_path)
         logger.info(f"Saved tokenizer to {tokenizer_output_path}.")
 
+    if save_safe_tensor:
+        logger.info(f"Loading HuggingFace compatible PyTorch LaBSE model from {pt_output_path}.")
+        pt_output_path = output_path.joinpath("pt_safe") if not huggingface_path else output_path
+        pt_model = BertModel.from_pretrained(pt_output_path)
+        for parameter in pt_model.parameters():
+            parameter = parameter.contiguous()
+        pt_model.save_pretrained(pt_output_path, safe_serialization=True)
+        del pt_model
+        logger.info(f"Saved PyTorch `safetensors` model to {pt_output_path}.")
+
     if save_tf:
         tf_output_path = output_path.joinpath("tf") if not huggingface_path else output_path
         tf_output_path.mkdir(exist_ok=True, parents=True)
         logger.info(f"Loading HuggingFace compatible TF LaBSE model from {pt_output_path}.")
         tf_model = TFBertModel.from_pretrained(pt_output_path, from_pt=True)
         tf_model.save_pretrained(tf_output_path)
         del tf_model
```

### Comparing `convert_labse_tf_pt-2.3.0/src/convert_labse_tf_pt/data/labse_vocab/cased_vocab.txt` & `convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/data/labse_vocab/cased_vocab.txt`

 * *Files identical despite different names*

### Comparing `convert_labse_tf_pt-2.3.0/src/convert_labse_tf_pt/data/smaller_vocab/vocab-en-fr-es-de-zh-ar-zh_classical-it-ja-ko-nl-pl-pt-th-tr-ru.txt` & `convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/data/smaller_vocab/vocab-en-fr-es-de-zh-ar-zh_classical-it-ja-ko-nl-pl-pt-th-tr-ru.txt`

 * *Files identical despite different names*

### Comparing `convert_labse_tf_pt-2.3.0/PKG-INFO` & `convert_labse_tf_pt-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: convert-labse-tf-pt
-Version: 2.3.0
+Version: 2.4.0
 Summary: Convert LaBSE model from TensorFlow to PyTorch.
 Home-page: https://github.com/setu4993/convert-labse-tf-pt
 License: MIT
 Keywords: transformers,bert,labse,pytorch,tensorflow
 Author: Setu Shah
 Author-email: setu+labse@setu.me
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: ipywidgets (>=7.6.3,<8.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: safetensors (>=0.3.1,<0.4.0)
 Requires-Dist: tensorflow-hub (>=0.12.0,<0.13.0)
 Requires-Dist: transformers[flax,sentencepiece,tf,torch] (>=4.29.0,<5.0.0)
 Project-URL: Repository, https://github.com/setu4993/convert-labse-tf-pt
 Description-Content-Type: text/markdown
 
 # LaBSE
```

