# Comparing `tmp/semantic_counter-0.0.3.tar.gz` & `tmp/semantic_counter-0.0.4.tar.gz`

## Comparing `semantic_counter-0.0.3.tar` & `semantic_counter-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/requirements.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/test.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/src/semantic_counter/__init__.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/src/semantic_counter/semantic_vectorizer.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/LICENSE
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/README.md
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 semantic_counter-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 semantic_counter-0.0.4/requirements.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 semantic_counter-0.0.4/test.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 semantic_counter-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 semantic_counter-0.0.4/src/semantic_counter/__init__.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 semantic_counter-0.0.4/src/semantic_counter/semantic_vectorizer.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 semantic_counter-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 semantic_counter-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 semantic_counter-0.0.4/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 semantic_counter-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 semantic_counter-0.0.4/PKG-INFO
```

### Comparing `semantic_counter-0.0.3/requirements.txt` & `semantic_counter-0.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `semantic_counter-0.0.3/src/semantic_counter/semantic_vectorizer.py` & `semantic_counter-0.0.4/src/semantic_counter/semantic_vectorizer.py`

 * *Files identical despite different names*

### Comparing `semantic_counter-0.0.3/LICENSE` & `semantic_counter-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic_counter-0.0.3/README.md` & `semantic_counter-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `semantic_counter-0.0.3/pyproject.toml` & `semantic_counter-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "semantic_counter"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Deepak Dalakoti", email="deepakkdalakoti@gmail.com" },
 ]
 description = "A wrapper around CountVectorizer which counts semantically similar tokens"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `semantic_counter-0.0.3/PKG-INFO` & `semantic_counter-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic_counter
-Version: 0.0.3
+Version: 0.0.4
 Summary: A wrapper around CountVectorizer which counts semantically similar tokens
 Project-URL: Homepage, https://github.com/deepakdalakoti/SemanticVectorizer
 Project-URL: Bug Tracker, https://github.com/deepakdalakoti/SemanticVectorizer/issues
 Author-email: Deepak Dalakoti <deepakkdalakoti@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

