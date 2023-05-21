# Comparing `tmp/convert_labse_tf_pt-2.4.0.tar.gz` & `tmp/convert_labse_tf_pt-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert_labse_tf_pt-2.4.0.tar", max compression
+gzip compressed data, was "convert_labse_tf_pt-2.4.1.tar", max compression
```

## Comparing `convert_labse_tf_pt-2.4.0.tar` & `convert_labse_tf_pt-2.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-05-21 08:41:17.652723 convert_labse_tf_pt-2.4.0/LICENSE
--rw-r--r--   0        0        0     1384 2023-05-21 08:41:17.652723 convert_labse_tf_pt-2.4.0/README.md
--rw-r--r--   0        0        0     1198 2023-05-21 08:41:17.656723 convert_labse_tf_pt-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      315 2023-05-21 08:41:17.656723 convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/__init__.py
--rw-r--r--   0        0        0     2081 2023-05-21 08:41:17.656723 convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/configurations.py
--rw-r--r--   0        0        0    18478 2023-05-21 08:41:17.656723 convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/convert.py
--rw-r--r--   0        0        0  5220781 2023-05-21 08:41:17.700724 convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/data/labse_vocab/cased_vocab.txt
--rw-r--r--   0        0        0  1469057 2023-05-21 08:41:17.708724 convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/data/smaller_vocab/vocab-en-fr-es-de-zh-ar-zh_classical-it-ja-ko-nl-pl-pt-th-tr-ru.txt
--rw-r--r--   0        0        0     2324 1970-01-01 00:00:00.000000 convert_labse_tf_pt-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-21 08:45:20.478669 convert_labse_tf_pt-2.4.1/LICENSE
+-rw-r--r--   0        0        0     1384 2023-05-21 08:45:20.478669 convert_labse_tf_pt-2.4.1/README.md
+-rw-r--r--   0        0        0     1230 2023-05-21 08:45:20.478669 convert_labse_tf_pt-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0      314 2023-05-21 08:45:20.478669 convert_labse_tf_pt-2.4.1/src/convert_labse_tf_pt/__init__.py
+-rw-r--r--   0        0        0     2080 2023-05-21 08:45:20.478669 convert_labse_tf_pt-2.4.1/src/convert_labse_tf_pt/configurations.py
+-rw-r--r--   0        0        0    18504 2023-05-21 08:45:20.478669 convert_labse_tf_pt-2.4.1/src/convert_labse_tf_pt/convert.py
+-rw-r--r--   0        0        0  5220781 2023-05-21 08:45:20.522669 convert_labse_tf_pt-2.4.1/src/convert_labse_tf_pt/data/labse_vocab/cased_vocab.txt
+-rw-r--r--   0        0        0  1469057 2023-05-21 08:45:20.530669 convert_labse_tf_pt-2.4.1/src/convert_labse_tf_pt/data/smaller_vocab/vocab-en-fr-es-de-zh-ar-zh_classical-it-ja-ko-nl-pl-pt-th-tr-ru.txt
+-rw-r--r--   0        0        0     2324 1970-01-01 00:00:00.000000 convert_labse_tf_pt-2.4.1/PKG-INFO
```

### Comparing `convert_labse_tf_pt-2.4.0/LICENSE` & `convert_labse_tf_pt-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `convert_labse_tf_pt-2.4.0/README.md` & `convert_labse_tf_pt-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `convert_labse_tf_pt-2.4.0/pyproject.toml` & `convert_labse_tf_pt-2.4.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "convert-labse-tf-pt"
-version = "2.4.0"
+version = "2.4.1"
 description = "Convert LaBSE model from TensorFlow to PyTorch."
 license = "MIT"
 authors = ["Setu Shah <setu+labse@setu.me>"]
 readme = "README.md"
 homepage = "https://github.com/setu4993/convert-labse-tf-pt"
 repository = "https://github.com/setu4993/convert-labse-tf-pt"
 keywords = ["transformers", "bert", "labse", "pytorch", "tensorflow"]
@@ -31,12 +31,15 @@
 pre-commit = "^2.21.0"
 ipython = "^8.7.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.black]
+line-length = 120
+
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 pythonpath = ["./src/"]
```

### Comparing `convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/configurations.py` & `convert_labse_tf_pt-2.4.1/src/convert_labse_tf_pt/configurations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from dataclasses import dataclass, asdict
-from typing import Dict
-
+from dataclasses import asdict, dataclass
 from pathlib import Path
+from typing import Dict
 
 
 @dataclass
 class LaBSE:
     repo: str = "LaBSE"
 
     # Attributes from `BertConfig`.
```

### Comparing `convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/convert.py` & `convert_labse_tf_pt-2.4.1/src/convert_labse_tf_pt/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,29 +8,36 @@
 This script is adapted from HuggingFace's BERT conversion script: https://github.com/huggingface/transformers/blob/master/src/transformers/models/bert/convert_bert_original_tf2_checkpoint_to_pytorch.py
 """
 from argparse import ArgumentParser
 from pathlib import Path
 from re import match
 from typing import List, Tuple, Union
 
-import torch.nn.functional as F
 import tensorflow_text  # noqa: F401
+import torch.nn.functional as F
 from loguru import logger
 from tensorflow_hub import load
 from torch import from_numpy, matmul, no_grad
 from transformers import (
     BertConfig,
     BertModel,
     BertTokenizerFast,
-    PretrainedConfig,
     FlaxBertModel,
+    PretrainedConfig,
     TFBertModel,
 )
 from transformers.modeling_outputs import BaseModelOutputWithPoolingAndCrossAttentions
-from convert_labse_tf_pt.configurations import LEALLABase, LEALLALarge, LEALLASmall, LaBSE, SmallerLaBSE
+
+from convert_labse_tf_pt.configurations import (
+    LaBSE,
+    LEALLABase,
+    LEALLALarge,
+    LEALLASmall,
+    SmallerLaBSE,
+)
 
 PATH = Union[str, Path]
 MODEL_TOKENIZER = Tuple[BertModel, BertTokenizerFast]
 
 
 def load_tf_model(tf_saved_model: PATH = LaBSE().tf_hub_link):
     tf_saved_model = tf_saved_model
```

### Comparing `convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/data/labse_vocab/cased_vocab.txt` & `convert_labse_tf_pt-2.4.1/src/convert_labse_tf_pt/data/labse_vocab/cased_vocab.txt`

 * *Files identical despite different names*

### Comparing `convert_labse_tf_pt-2.4.0/src/convert_labse_tf_pt/data/smaller_vocab/vocab-en-fr-es-de-zh-ar-zh_classical-it-ja-ko-nl-pl-pt-th-tr-ru.txt` & `convert_labse_tf_pt-2.4.1/src/convert_labse_tf_pt/data/smaller_vocab/vocab-en-fr-es-de-zh-ar-zh_classical-it-ja-ko-nl-pl-pt-th-tr-ru.txt`

 * *Files identical despite different names*

### Comparing `convert_labse_tf_pt-2.4.0/PKG-INFO` & `convert_labse_tf_pt-2.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-labse-tf-pt
-Version: 2.4.0
+Version: 2.4.1
 Summary: Convert LaBSE model from TensorFlow to PyTorch.
 Home-page: https://github.com/setu4993/convert-labse-tf-pt
 License: MIT
 Keywords: transformers,bert,labse,pytorch,tensorflow
 Author: Setu Shah
 Author-email: setu+labse@setu.me
 Requires-Python: >=3.8,<3.11
```

