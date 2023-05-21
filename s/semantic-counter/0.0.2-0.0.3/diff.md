# Comparing `tmp/semantic_counter-0.0.2.tar.gz` & `tmp/semantic_counter-0.0.3.tar.gz`

## Comparing `semantic_counter-0.0.2.tar` & `semantic_counter-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 semantic_counter-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semantic_counter-0.0.2/src/semantic_counter/__init__.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 semantic_counter-0.0.2/src/semantic_counter/semantic_vectorizer.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 semantic_counter-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 semantic_counter-0.0.2/LICENSE
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 semantic_counter-0.0.2/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 semantic_counter-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 semantic_counter-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/test.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/src/semantic_counter/__init__.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/src/semantic_counter/semantic_vectorizer.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/PKG-INFO
```

### Comparing `semantic_counter-0.0.2/requirements.txt` & `semantic_counter-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `semantic_counter-0.0.2/src/semantic_counter/semantic_vectorizer.py` & `semantic_counter-0.0.3/src/semantic_counter/semantic_vectorizer.py`

 * *Files identical despite different names*

### Comparing `semantic_counter-0.0.2/LICENSE` & `semantic_counter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic_counter-0.0.2/README.md` & `semantic_counter-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 ### Wrapper around CountVectorizer to count phrases based on semantic similarity
 ---
 SemanticCountVectorizer extends CountVectorizer by counting the frequency of semantically similar tokens. This is useful when searching for frequency of similar but not exact terms.
 
 SemanticCountVectorizer uses sentence_transformers to compute embedding of n-grams and then clusters similar terms using Agglomerative Clustering using cosine similarity as the similarity metric
 
 ---
+
+### Installation
+
+`pip install semantic_counter`
+
+
 ### Usage
 
 ```
-from semantic_vectorizer import SemanticCountVectorizer 
+from semantic_counter.semantic_vectorizer import SemanticCountVectorizer 
 sentences = ['this is a test sentences','this is another test sentence']
-svect = SemanticVectorizer(embedding_model_name='all-MiniLM-L6-v2', similarity_threshold=0.7, ngram_range=(3,3))
+svect = SemanticCountVectorizer(embedding_model_name='all-MiniLM-L6-v2', similarity_threshold=0.7, ngram_range=(3,3))
 counts=svect.fit_transform(sentences)
 ```
 
 ### Arguments
 - embedding_model_name: Name of the sentence_transformer pretrained model to use. Refer to [package website](https://www.sbert.net/docs/pretrained_models.html) for a list of available models
 - similarity_threshold: value between 0-1 which indicates minimum cosine similarity needed to group tokens.
 - Arguments of sklearn's CountVectorizer as listed [here](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.html)
```

### Comparing `semantic_counter-0.0.2/pyproject.toml` & `semantic_counter-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "semantic_counter"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Deepak Dalakoti", email="deepakkdalakoti@gmail.com" },
 ]
 description = "A wrapper around CountVectorizer which counts semantically similar tokens"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `semantic_counter-0.0.2/PKG-INFO` & `semantic_counter-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic_counter
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wrapper around CountVectorizer which counts semantically similar tokens
 Project-URL: Homepage, https://github.com/deepakdalakoti/SemanticVectorizer
 Project-URL: Bug Tracker, https://github.com/deepakdalakoti/SemanticVectorizer/issues
 Author-email: Deepak Dalakoti <deepakkdalakoti@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,20 +15,26 @@
 ### Wrapper around CountVectorizer to count phrases based on semantic similarity
 ---
 SemanticCountVectorizer extends CountVectorizer by counting the frequency of semantically similar tokens. This is useful when searching for frequency of similar but not exact terms.
 
 SemanticCountVectorizer uses sentence_transformers to compute embedding of n-grams and then clusters similar terms using Agglomerative Clustering using cosine similarity as the similarity metric
 
 ---
+
+### Installation
+
+`pip install semantic_counter`
+
+
 ### Usage
 
 ```
-from semantic_vectorizer import SemanticCountVectorizer 
+from semantic_counter.semantic_vectorizer import SemanticCountVectorizer 
 sentences = ['this is a test sentences','this is another test sentence']
-svect = SemanticVectorizer(embedding_model_name='all-MiniLM-L6-v2', similarity_threshold=0.7, ngram_range=(3,3))
+svect = SemanticCountVectorizer(embedding_model_name='all-MiniLM-L6-v2', similarity_threshold=0.7, ngram_range=(3,3))
 counts=svect.fit_transform(sentences)
 ```
 
 ### Arguments
 - embedding_model_name: Name of the sentence_transformer pretrained model to use. Refer to [package website](https://www.sbert.net/docs/pretrained_models.html) for a list of available models
 - similarity_threshold: value between 0-1 which indicates minimum cosine similarity needed to group tokens.
 - Arguments of sklearn's CountVectorizer as listed [here](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.html)
```

