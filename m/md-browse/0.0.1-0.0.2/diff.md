# Comparing `tmp/md-browse-0.0.1.tar.gz` & `tmp/md-browse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md-browse-0.0.1.tar", last modified: Sat Apr  8 12:53:51 2023, max compression
+gzip compressed data, was "md-browse-0.0.2.tar", last modified: Sun May 21 06:46:55 2023, max compression
```

## Comparing `md-browse-0.0.1.tar` & `md-browse-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 12:53:51.898704 md-browse-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-04-08 07:04:20.000000 md-browse-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      739 2023-04-08 12:53:51.897489 md-browse-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-04-08 07:09:37.000000 md-browse-0.0.1/README.md
--rw-rw-rw-   0        0        0      775 2023-04-08 07:36:32.000000 md-browse-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 12:53:51.898704 md-browse-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       92 2023-04-08 07:04:20.000000 md-browse-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 12:53:51.850764 md-browse-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 12:53:51.872566 md-browse-0.0.1/src/md_browse/
--rw-rw-rw-   0        0        0       50 2023-04-08 12:32:46.000000 md-browse-0.0.1/src/md_browse/__init__.py
--rw-rw-rw-   0        0        0     1480 2023-04-03 12:11:56.000000 md-browse-0.0.1/src/md_browse/clean.py
--rw-rw-rw-   0        0        0      358 2023-04-03 12:11:56.000000 md-browse-0.0.1/src/md_browse/converttomarkdown.py
--rw-rw-rw-   0        0        0     1528 2023-04-08 12:33:11.000000 md-browse-0.0.1/src/md_browse/md_browse.py
-drwxrwxrwx   0        0        0        0 2023-04-08 12:53:51.893334 md-browse-0.0.1/src/md_browse.egg-info/
--rw-rw-rw-   0        0        0      739 2023-04-08 12:53:51.000000 md-browse-0.0.1/src/md_browse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-04-08 12:53:51.000000 md-browse-0.0.1/src/md_browse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 12:53:51.000000 md-browse-0.0.1/src/md_browse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-08 12:53:51.000000 md-browse-0.0.1/src/md_browse.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2023-04-08 12:53:51.000000 md-browse-0.0.1/src/md_browse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-08 12:53:51.000000 md-browse-0.0.1/src/md_browse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 06:46:55.126084 md-browse-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-04-08 07:04:20.000000 md-browse-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      739 2023-05-21 06:46:55.126084 md-browse-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-04-08 07:09:37.000000 md-browse-0.0.2/README.md
+-rw-rw-rw-   0        0        0      780 2023-05-21 06:45:11.000000 md-browse-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 06:46:55.126084 md-browse-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       92 2023-04-08 07:04:20.000000 md-browse-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 06:46:55.072086 md-browse-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-21 06:46:55.098085 md-browse-0.0.2/src/md_browse/
+-rw-rw-rw-   0        0        0       50 2023-04-08 12:32:46.000000 md-browse-0.0.2/src/md_browse/__init__.py
+-rw-rw-rw-   0        0        0     1480 2023-04-03 12:11:56.000000 md-browse-0.0.2/src/md_browse/clean.py
+-rw-rw-rw-   0        0        0      358 2023-04-03 12:11:56.000000 md-browse-0.0.2/src/md_browse/converttomarkdown.py
+-rw-rw-rw-   0        0        0     1528 2023-04-08 12:33:11.000000 md-browse-0.0.2/src/md_browse/md_browse.py
+drwxrwxrwx   0        0        0        0 2023-05-21 06:46:55.125084 md-browse-0.0.2/src/md_browse.egg-info/
+-rw-rw-rw-   0        0        0      739 2023-05-21 06:46:55.000000 md-browse-0.0.2/src/md_browse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-05-21 06:46:55.000000 md-browse-0.0.2/src/md_browse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 06:46:55.000000 md-browse-0.0.2/src/md_browse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-21 06:46:55.000000 md-browse-0.0.2/src/md_browse.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2023-05-21 06:46:55.000000 md-browse-0.0.2/src/md_browse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-21 06:46:55.000000 md-browse-0.0.2/src/md_browse.egg-info/top_level.txt
```

### Comparing `md-browse-0.0.1/LICENSE` & `md-browse-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `md-browse-0.0.1/PKG-INFO` & `md-browse-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md-browse
-Version: 0.0.1
+Version: 0.0.2
 Summary: Returns HTML from a web request as cleaned markdown.
 Author-email: Emil Kloeden <emilkloeden@gmail.com>
 Project-URL: Homepage, https://github.com/emilkloeden/md-browse
 Project-URL: Bug Tracker, https://github.com/emilkloeden/md-browse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `md-browse-0.0.1/pyproject.toml` & `md-browse-0.0.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "md-browse"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Emil Kloeden", email="emilkloeden@gmail.com" },
 ]
 description = "Returns HTML from a web request as cleaned markdown."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -19,8 +19,8 @@
 dependencies = ["beautifulsoup4==4.12.2","requests==2.28.2", "markdownify==0.11.6"]
 
 [project.urls]
 "Homepage" = "https://github.com/emilkloeden/md-browse"
 "Bug Tracker" = "https://github.com/emilkloeden/md-browse/issues"
 
 [project.scripts]
-"md-browse" = "md_browse.main:main" 
+"md-browse" = "md_browse.md_browse:main"
```

### Comparing `md-browse-0.0.1/src/md_browse/clean.py` & `md-browse-0.0.2/src/md_browse/clean.py`

 * *Files identical despite different names*

### Comparing `md-browse-0.0.1/src/md_browse/md_browse.py` & `md-browse-0.0.2/src/md_browse/md_browse.py`

 * *Files identical despite different names*

### Comparing `md-browse-0.0.1/src/md_browse.egg-info/PKG-INFO` & `md-browse-0.0.2/src/md_browse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md-browse
-Version: 0.0.1
+Version: 0.0.2
 Summary: Returns HTML from a web request as cleaned markdown.
 Author-email: Emil Kloeden <emilkloeden@gmail.com>
 Project-URL: Homepage, https://github.com/emilkloeden/md-browse
 Project-URL: Bug Tracker, https://github.com/emilkloeden/md-browse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

