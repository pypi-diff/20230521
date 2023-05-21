# Comparing `tmp/prompt_optimizer-0.2.0.tar.gz` & `tmp/prompt_optimizer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_optimizer-0.2.0.tar", max compression
+gzip compressed data, was "prompt_optimizer-0.2.1.tar", max compression
```

## Comparing `prompt_optimizer-0.2.0.tar` & `prompt_optimizer-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-09 00:01:22.989764 prompt_optimizer-0.2.0/LICENSE
--rw-r--r--   0        0        0     5307 2023-05-19 19:11:38.420996 prompt_optimizer-0.2.0/README.md
--rw-r--r--   0        0        0      609 2023-05-19 03:03:11.410726 prompt_optimizer-0.2.0/prompt_optimizer/__init__.py
--rw-r--r--   0        0        0      234 2023-04-08 22:38:34.428079 prompt_optimizer-0.2.0/prompt_optimizer/metric/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-18 08:41:28.963678 prompt_optimizer-0.2.0/prompt_optimizer/metric/base.py
--rw-r--r--   0        0        0     2007 2023-05-19 02:42:52.321714 prompt_optimizer-0.2.0/prompt_optimizer/metric/bertscore_metric.py
--rw-r--r--   0        0        0     1925 2023-05-19 03:03:01.423169 prompt_optimizer-0.2.0/prompt_optimizer/metric/token_metric.py
--rw-r--r--   0        0        0     1027 2023-05-18 23:02:51.540434 prompt_optimizer-0.2.0/prompt_optimizer/poptim/__init__.py
--rw-r--r--   0        0        0     1709 2023-05-19 03:03:01.415647 prompt_optimizer-0.2.0/prompt_optimizer/poptim/autocorrect_optim.py
--rw-r--r--   0        0        0     5997 2023-05-18 23:01:02.911660 prompt_optimizer-0.2.0/prompt_optimizer/poptim/base.py
--rw-r--r--   0        0        0     5122 2023-05-19 03:03:01.454647 prompt_optimizer-0.2.0/prompt_optimizer/poptim/entropy_optim.py
--rw-r--r--   0        0        0     2109 2023-05-19 03:03:01.455363 prompt_optimizer-0.2.0/prompt_optimizer/poptim/lemmatizer_optim.py
--rw-r--r--   0        0        0      550 2023-05-18 22:59:18.835561 prompt_optimizer-0.2.0/prompt_optimizer/poptim/logger.py
--rw-r--r--   0        0        0     5180 2023-05-19 03:03:01.459575 prompt_optimizer-0.2.0/prompt_optimizer/poptim/name_replace_optim.py
--rw-r--r--   0        0        0     2583 2023-05-19 03:03:01.433793 prompt_optimizer-0.2.0/prompt_optimizer/poptim/pulp_optim.py
--rw-r--r--   0        0        0     1397 2023-05-19 03:03:01.427258 prompt_optimizer-0.2.0/prompt_optimizer/poptim/punctuation_optim.py
--rw-r--r--   0        0        0     1447 2023-05-18 23:01:02.902907 prompt_optimizer-0.2.0/prompt_optimizer/poptim/sequential.py
--rw-r--r--   0        0        0     1427 2023-05-19 03:03:01.438454 prompt_optimizer-0.2.0/prompt_optimizer/poptim/stemmer_optim.py
--rw-r--r--   0        0        0     1683 2023-05-19 03:03:01.444802 prompt_optimizer-0.2.0/prompt_optimizer/poptim/stop_word_optim.py
--rw-r--r--   0        0        0     3162 2023-05-19 03:03:01.465816 prompt_optimizer-0.2.0/prompt_optimizer/poptim/synonym_replace_optim.py
--rw-r--r--   0        0        0     6164 2023-05-18 23:01:03.800340 prompt_optimizer-0.2.0/prompt_optimizer/poptim/utils.py
--rw-r--r--   0        0        0       93 2023-05-18 08:28:30.775249 prompt_optimizer-0.2.0/prompt_optimizer/visualize/__init__.py
--rw-r--r--   0        0        0     1033 2023-05-18 08:36:23.277116 prompt_optimizer-0.2.0/prompt_optimizer/visualize/stringdiffer.py
--rw-r--r--   0        0        0     1691 2023-05-19 19:33:43.305769 prompt_optimizer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6059 1970-01-01 00:00:00.000000 prompt_optimizer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-09 00:01:22.989764 prompt_optimizer-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5307 2023-05-19 19:11:38.420996 prompt_optimizer-0.2.1/README.md
+-rw-r--r--   0        0        0      609 2023-05-21 01:28:58.617356 prompt_optimizer-0.2.1/prompt_optimizer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 22:21:06.683584 prompt_optimizer-0.2.1/prompt_optimizer/cli/__init__.py
+-rw-r--r--   0        0        0     6908 2023-05-21 01:27:23.766988 prompt_optimizer-0.2.1/prompt_optimizer/cli/main.py
+-rw-r--r--   0        0        0      234 2023-04-08 22:38:34.428079 prompt_optimizer-0.2.1/prompt_optimizer/metric/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-18 08:41:28.963678 prompt_optimizer-0.2.1/prompt_optimizer/metric/base.py
+-rw-r--r--   0        0        0     2007 2023-05-19 02:42:52.321714 prompt_optimizer-0.2.1/prompt_optimizer/metric/bertscore_metric.py
+-rw-r--r--   0        0        0     1925 2023-05-19 03:03:01.423169 prompt_optimizer-0.2.1/prompt_optimizer/metric/token_metric.py
+-rw-r--r--   0        0        0     1027 2023-05-18 23:02:51.540434 prompt_optimizer-0.2.1/prompt_optimizer/poptim/__init__.py
+-rw-r--r--   0        0        0     1709 2023-05-19 03:03:01.415647 prompt_optimizer-0.2.1/prompt_optimizer/poptim/autocorrect_optim.py
+-rw-r--r--   0        0        0     5997 2023-05-18 23:01:02.911660 prompt_optimizer-0.2.1/prompt_optimizer/poptim/base.py
+-rw-r--r--   0        0        0     5122 2023-05-19 03:03:01.454647 prompt_optimizer-0.2.1/prompt_optimizer/poptim/entropy_optim.py
+-rw-r--r--   0        0        0     2109 2023-05-19 03:03:01.455363 prompt_optimizer-0.2.1/prompt_optimizer/poptim/lemmatizer_optim.py
+-rw-r--r--   0        0        0      550 2023-05-18 22:59:18.835561 prompt_optimizer-0.2.1/prompt_optimizer/poptim/logger.py
+-rw-r--r--   0        0        0     5180 2023-05-19 03:03:01.459575 prompt_optimizer-0.2.1/prompt_optimizer/poptim/name_replace_optim.py
+-rw-r--r--   0        0        0     2583 2023-05-19 03:03:01.433793 prompt_optimizer-0.2.1/prompt_optimizer/poptim/pulp_optim.py
+-rw-r--r--   0        0        0     1397 2023-05-19 03:03:01.427258 prompt_optimizer-0.2.1/prompt_optimizer/poptim/punctuation_optim.py
+-rw-r--r--   0        0        0     1468 2023-05-21 01:27:23.656964 prompt_optimizer-0.2.1/prompt_optimizer/poptim/sequential.py
+-rw-r--r--   0        0        0     1427 2023-05-19 03:03:01.438454 prompt_optimizer-0.2.1/prompt_optimizer/poptim/stemmer_optim.py
+-rw-r--r--   0        0        0     1683 2023-05-19 03:03:01.444802 prompt_optimizer-0.2.1/prompt_optimizer/poptim/stop_word_optim.py
+-rw-r--r--   0        0        0     3162 2023-05-19 03:03:01.465816 prompt_optimizer-0.2.1/prompt_optimizer/poptim/synonym_replace_optim.py
+-rw-r--r--   0        0        0     6164 2023-05-18 23:01:03.800340 prompt_optimizer-0.2.1/prompt_optimizer/poptim/utils.py
+-rw-r--r--   0        0        0       93 2023-05-18 08:28:30.775249 prompt_optimizer-0.2.1/prompt_optimizer/visualize/__init__.py
+-rw-r--r--   0        0        0     1033 2023-05-18 08:36:23.277116 prompt_optimizer-0.2.1/prompt_optimizer/visualize/stringdiffer.py
+-rw-r--r--   0        0        0     1774 2023-05-21 01:30:22.995007 prompt_optimizer-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6059 1970-01-01 00:00:00.000000 prompt_optimizer-0.2.1/PKG-INFO
```

### Comparing `prompt_optimizer-0.2.0/LICENSE` & `prompt_optimizer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/README.md` & `prompt_optimizer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/__init__.py` & `prompt_optimizer-0.2.1/prompt_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/metric/base.py` & `prompt_optimizer-0.2.1/prompt_optimizer/metric/base.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/metric/bertscore_metric.py` & `prompt_optimizer-0.2.1/prompt_optimizer/metric/bertscore_metric.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/metric/token_metric.py` & `prompt_optimizer-0.2.1/prompt_optimizer/metric/token_metric.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/__init__.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/autocorrect_optim.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/autocorrect_optim.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/base.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/base.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/entropy_optim.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/entropy_optim.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/lemmatizer_optim.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/lemmatizer_optim.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/logger.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/logger.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/name_replace_optim.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/name_replace_optim.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/pulp_optim.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/pulp_optim.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/punctuation_optim.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/punctuation_optim.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/sequential.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/sequential.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 
 class Sequential:
     """
     Sequential is a class that represents a sequential composition of prompt optimization techniques.
 
     It applies a series of optimization techniques in sequence to the prompt.
 
-    Usage:
-    ```
-    optim1 = SomeOptimizationTechnique()
-    optim2 = AnotherOptimizationTechnique()
-    seq = Sequential(optim1, optim2)
-    optimized_prompt = seq(prompt)
-    ```
+
+
+
+    Example:
+        >>> optim1 = SomeOptimizationTechnique()
+        >>> optim2 = AnotherOptimizationTechnique()
+        >>> seq = Sequential(optim1, optim2)
+        >>> optimized_prompt = seq(prompt)
 
     Args:
         *optims: Variable-length argument list of prompt optimization techniques.
 
     Attributes:
         optims (list): A list of prompt optimization techniques.
```

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/stemmer_optim.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/stemmer_optim.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/stop_word_optim.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/stop_word_optim.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/synonym_replace_optim.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/synonym_replace_optim.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/poptim/utils.py` & `prompt_optimizer-0.2.1/prompt_optimizer/poptim/utils.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/prompt_optimizer/visualize/stringdiffer.py` & `prompt_optimizer-0.2.1/prompt_optimizer/visualize/stringdiffer.py`

 * *Files identical despite different names*

### Comparing `prompt_optimizer-0.2.0/pyproject.toml` & `prompt_optimizer-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [tool.poetry]
 name = "prompt-optimizer"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Vaibhav Kumar <34630911+TimeTraveller-San@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "prompt_optimizer"}]
 
+[tool.poetry.scripts]
+prompt-optimizer = "prompt_optimizer.cli.main:main"
+
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 transformers = "^4.27.4"
 torch = "^2.0.0"
 pulp = "^2.7.0"
 nltk = "^3.8.1"
 tiktoken = "^0.3.3"
@@ -51,15 +54,15 @@
 select = [
   "E",  # pycodestyle
   "F",  # pyflakes
   "I",  # isort
 ]
 line-length = 88
 fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
-ignore = ["E501"]
+ignore = ["E501", "F403"]
 
 
 [tool.mypy]
 ignore_missing_imports = "True"
 disallow_untyped_defs = "True"
 exclude = ["notebooks"]
```

### Comparing `prompt_optimizer-0.2.0/PKG-INFO` & `prompt_optimizer-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-optimizer
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Vaibhav Kumar
 Author-email: 34630911+TimeTraveller-San@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

