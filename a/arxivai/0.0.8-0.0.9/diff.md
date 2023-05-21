# Comparing `tmp/arxivai-0.0.8.tar.gz` & `tmp/arxivai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxivai-0.0.8.tar", last modified: Tue May 16 21:54:58 2023, max compression
+gzip compressed data, was "arxivai-0.0.9.tar", last modified: Wed May 17 04:16:39 2023, max compression
```

## Comparing `arxivai-0.0.8.tar` & `arxivai-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:58.042760 arxivai-0.0.8/
--rw-rw-rw-   0        0        0     1090 2023-05-16 12:09:57.000000 arxivai-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      655 2023-05-16 21:54:58.041756 arxivai-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-05-16 12:09:49.000000 arxivai-0.0.8/README.md
--rw-rw-rw-   0        0        0      679 2023-05-16 21:54:26.000000 arxivai-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 21:54:58.042760 arxivai-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:58.010756 arxivai-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:58.020753 arxivai-0.0.8/src/arxivai/
--rw-rw-rw-   0        0        0       50 2023-05-16 21:54:11.000000 arxivai-0.0.8/src/arxivai/__init__.py
--rw-rw-rw-   0        0        0     4421 2023-05-16 20:22:48.000000 arxivai-0.0.8/src/arxivai/arxiv_api.py
--rw-rw-rw-   0        0        0      629 2023-05-16 21:49:58.000000 arxivai-0.0.8/src/arxivai/arxiv_pdf.py
-drwxrwxrwx   0        0        0        0 2023-05-16 21:54:58.039758 arxivai-0.0.8/src/arxivai.egg-info/
--rw-rw-rw-   0        0        0      655 2023-05-16 21:54:57.000000 arxivai-0.0.8/src/arxivai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-05-16 21:54:58.000000 arxivai-0.0.8/src/arxivai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 21:54:57.000000 arxivai-0.0.8/src/arxivai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 21:54:57.000000 arxivai-0.0.8/src/arxivai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 04:16:39.265067 arxivai-0.0.9/
+-rw-rw-rw-   0        0        0     1090 2023-05-16 12:09:57.000000 arxivai-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      655 2023-05-17 04:16:39.264066 arxivai-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-05-16 12:09:49.000000 arxivai-0.0.9/README.md
+-rw-rw-rw-   0        0        0      675 2023-05-17 04:14:22.000000 arxivai-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 04:16:39.266066 arxivai-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 04:16:39.221066 arxivai-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 04:16:39.245067 arxivai-0.0.9/src/arxivai/
+-rw-rw-rw-   0        0        0       50 2023-05-16 21:54:11.000000 arxivai-0.0.9/src/arxivai/__init__.py
+-rw-rw-rw-   0        0        0     5176 2023-05-17 04:13:40.000000 arxivai-0.0.9/src/arxivai/arxiv_api.py
+-rw-rw-rw-   0        0        0     1654 2023-05-17 04:15:04.000000 arxivai-0.0.9/src/arxivai/arxiv_pdf.py
+drwxrwxrwx   0        0        0        0 2023-05-17 04:16:39.262066 arxivai-0.0.9/src/arxivai.egg-info/
+-rw-rw-rw-   0        0        0      655 2023-05-17 04:16:39.000000 arxivai-0.0.9/src/arxivai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-17 04:16:39.000000 arxivai-0.0.9/src/arxivai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 04:16:39.000000 arxivai-0.0.9/src/arxivai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 04:16:39.000000 arxivai-0.0.9/src/arxivai.egg-info/top_level.txt
```

### Comparing `arxivai-0.0.8/LICENSE` & `arxivai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `arxivai-0.0.8/PKG-INFO` & `arxivai-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxivai
-Version: 0.0.8
+Version: 0.0.9
 Summary: A complete arXiv API wrapper for Python.
 Author-email: Bongsang Kim <happykbs@gmail.com>
 Project-URL: Homepage, https://github.com/bongsang/arxivai-pypi
 Project-URL: Bug Tracker, https://github.com/bongsang/arxivai-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arxivai-0.0.8/pyproject.toml` & `arxivai-0.0.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = [
   "setuptools",
   "requests",
-  "beautifulsoup4",
+  "feedparser",
   "google-cloud-storage",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arxivai"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Bongsang Kim", email="happykbs@gmail.com" },
 ]
 description = "A complete arXiv API wrapper for Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `arxivai-0.0.8/src/arxivai.egg-info/PKG-INFO` & `arxivai-0.0.9/src/arxivai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxivai
-Version: 0.0.8
+Version: 0.0.9
 Summary: A complete arXiv API wrapper for Python.
 Author-email: Bongsang Kim <happykbs@gmail.com>
 Project-URL: Homepage, https://github.com/bongsang/arxivai-pypi
 Project-URL: Bug Tracker, https://github.com/bongsang/arxivai-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

