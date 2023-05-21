# Comparing `tmp/tcoi-0.2.4.tar.gz` & `tmp/tcoi-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcoi-0.2.4.tar", last modified: Wed Feb 22 18:25:28 2023, max compression
+gzip compressed data, was "tcoi-0.2.5.tar", last modified: Sun May 21 02:49:02 2023, max compression
```

## Comparing `tcoi-0.2.4.tar` & `tcoi-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 qurashiakh  (1000) qurashiakh  (1000)        0 2023-02-22 18:25:28.640349 tcoi-0.2.4/
--rw-r--r--   0 qurashiakh  (1000) qurashiakh  (1000)    35149 2023-02-08 16:26:09.000000 tcoi-0.2.4/LICENSE
--rw-r--r--   0 qurashiakh  (1000) qurashiakh  (1000)     6555 2023-02-22 18:25:28.630349 tcoi-0.2.4/PKG-INFO
--rw-r--r--   0 qurashiakh  (1000) qurashiakh  (1000)     5985 2023-02-22 17:37:34.000000 tcoi-0.2.4/README.md
--rw-r--r--   0 qurashiakh  (1000) qurashiakh  (1000)      639 2023-02-22 18:22:16.000000 tcoi-0.2.4/pyproject.toml
--rw-r--r--   0 qurashiakh  (1000) qurashiakh  (1000)       38 2023-02-22 18:25:28.640349 tcoi-0.2.4/setup.cfg
-drwxr-xr-x   0 qurashiakh  (1000) qurashiakh  (1000)        0 2023-02-22 18:25:28.630349 tcoi-0.2.4/src/
-drwxr-xr-x   0 qurashiakh  (1000) qurashiakh  (1000)        0 2023-02-22 18:25:28.630349 tcoi-0.2.4/src/tcoi/
--rw-r--r--   0 qurashiakh  (1000) qurashiakh  (1000)       88 2023-02-08 19:41:59.000000 tcoi-0.2.4/src/tcoi/__init__.py
--rw-r--r--   0 qurashiakh  (1000) qurashiakh  (1000)     4685 2023-02-22 18:20:40.000000 tcoi-0.2.4/src/tcoi/classes.py
--rw-r--r--   0 qurashiakh  (1000) qurashiakh  (1000)       37 2023-02-08 16:10:46.000000 tcoi-0.2.4/src/tcoi/errors.py
-drwxr-xr-x   0 qurashiakh  (1000) qurashiakh  (1000)        0 2023-02-22 18:25:28.630349 tcoi-0.2.4/src/tcoi.egg-info/
--rw-r--r--   0 qurashiakh  (1000) qurashiakh  (1000)     6555 2023-02-22 18:25:28.000000 tcoi-0.2.4/src/tcoi.egg-info/PKG-INFO
--rw-r--r--   0 qurashiakh  (1000) qurashiakh  (1000)      220 2023-02-22 18:25:28.000000 tcoi-0.2.4/src/tcoi.egg-info/SOURCES.txt
--rw-r--r--   0 qurashiakh  (1000) qurashiakh  (1000)        1 2023-02-22 18:25:28.000000 tcoi-0.2.4/src/tcoi.egg-info/dependency_links.txt
--rw-r--r--   0 qurashiakh  (1000) qurashiakh  (1000)        5 2023-02-22 18:25:28.000000 tcoi-0.2.4/src/tcoi.egg-info/top_level.txt
+drwxr-xr-x   0 husayn    (1000) husayn    (1000)        0 2023-05-21 02:49:02.032160 tcoi-0.2.5/
+-rwx------   0 husayn    (1000) husayn    (1000)    35149 2023-03-06 11:19:03.000000 tcoi-0.2.5/LICENSE
+-rw-r--r--   0 husayn    (1000) husayn    (1000)     6546 2023-05-21 02:49:02.032160 tcoi-0.2.5/PKG-INFO
+-rwx------   0 husayn    (1000) husayn    (1000)     5985 2023-03-06 11:19:03.000000 tcoi-0.2.5/README.md
+-rwx------   0 husayn    (1000) husayn    (1000)      630 2023-05-21 02:48:20.000000 tcoi-0.2.5/pyproject.toml
+-rw-r--r--   0 husayn    (1000) husayn    (1000)       38 2023-05-21 02:49:02.032160 tcoi-0.2.5/setup.cfg
+drwxr-xr-x   0 husayn    (1000) husayn    (1000)        0 2023-05-21 02:49:02.028827 tcoi-0.2.5/src/
+drwxr-xr-x   0 husayn    (1000) husayn    (1000)        0 2023-05-21 02:49:02.032160 tcoi-0.2.5/src/tcoi/
+-rwx------   0 husayn    (1000) husayn    (1000)       88 2023-03-06 11:19:02.000000 tcoi-0.2.5/src/tcoi/__init__.py
+-rwx------   0 husayn    (1000) husayn    (1000)     4685 2023-03-06 11:19:02.000000 tcoi-0.2.5/src/tcoi/classes.py
+-rwx------   0 husayn    (1000) husayn    (1000)       37 2023-03-06 11:19:02.000000 tcoi-0.2.5/src/tcoi/errors.py
+drwxr-xr-x   0 husayn    (1000) husayn    (1000)        0 2023-05-21 02:49:02.032160 tcoi-0.2.5/src/tcoi.egg-info/
+-rwx------   0 husayn    (1000) husayn    (1000)     6546 2023-05-21 02:49:02.000000 tcoi-0.2.5/src/tcoi.egg-info/PKG-INFO
+-rwx------   0 husayn    (1000) husayn    (1000)      220 2023-05-21 02:49:02.000000 tcoi-0.2.5/src/tcoi.egg-info/SOURCES.txt
+-rwx------   0 husayn    (1000) husayn    (1000)        1 2023-05-21 02:49:02.000000 tcoi-0.2.5/src/tcoi.egg-info/dependency_links.txt
+-rwx------   0 husayn    (1000) husayn    (1000)        5 2023-05-21 02:49:02.000000 tcoi-0.2.5/src/tcoi.egg-info/top_level.txt
```

### Comparing `tcoi-0.2.4/LICENSE` & `tcoi-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tcoi-0.2.4/PKG-INFO` & `tcoi-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tcoi
-Version: 0.2.4
+Version: 0.2.5
 Summary: A New Form of Decentralised Hashing.
-Author-email: Husayn al-Qurashi <husayn@dnmx.org>
+Author-email: Husayn Haras <husayn@dnmx.org>
 Project-URL: Homepage, https://qurashiakh.dev/the-code-of-ishaq.html
-Project-URL: Bug Tracker, https://github.com/qurashiakh/tcoi/issues
+Project-URL: Bug Tracker, https://github.com/hharas/tcoi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Utilities
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tcoi-0.2.4/README.md` & `tcoi-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tcoi-0.2.4/pyproject.toml` & `tcoi-0.2.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tcoi"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
-  { name="Husayn al-Qurashi", email="husayn@dnmx.org" },
+  { name="Husayn Haras", email="husayn@dnmx.org" },
 ]
 description = "A New Form of Decentralised Hashing."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Topic :: Utilities",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://qurashiakh.dev/the-code-of-ishaq.html"
-"Bug Tracker" = "https://github.com/qurashiakh/tcoi/issues"
+"Bug Tracker" = "https://github.com/hharas/tcoi/issues"
```

### Comparing `tcoi-0.2.4/src/tcoi/classes.py` & `tcoi-0.2.5/src/tcoi/classes.py`

 * *Files identical despite different names*

### Comparing `tcoi-0.2.4/src/tcoi.egg-info/PKG-INFO` & `tcoi-0.2.5/src/tcoi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tcoi
-Version: 0.2.4
+Version: 0.2.5
 Summary: A New Form of Decentralised Hashing.
-Author-email: Husayn al-Qurashi <husayn@dnmx.org>
+Author-email: Husayn Haras <husayn@dnmx.org>
 Project-URL: Homepage, https://qurashiakh.dev/the-code-of-ishaq.html
-Project-URL: Bug Tracker, https://github.com/qurashiakh/tcoi/issues
+Project-URL: Bug Tracker, https://github.com/hharas/tcoi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Utilities
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

