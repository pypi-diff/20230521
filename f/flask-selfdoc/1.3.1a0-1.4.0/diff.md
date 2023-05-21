# Comparing `tmp/flask-selfdoc-1.3.1a0.tar.gz` & `tmp/flask_selfdoc-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-selfdoc-1.3.1a0.tar", max compression
+gzip compressed data, was "flask_selfdoc-1.4.0.tar", max compression
```

## Comparing `flask-selfdoc-1.3.1a0.tar` & `flask_selfdoc-1.4.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1080 2022-03-01 13:44:24.991679 flask-selfdoc-1.3.1a0/LICENSE
--rw-r--r--   0        0        0      135 2022-03-01 13:44:24.991679 flask-selfdoc-1.3.1a0/flask_selfdoc/__init__.py
--rw-r--r--   0        0        0     8458 2022-03-01 13:44:24.991679 flask-selfdoc-1.3.1a0/flask_selfdoc/autodoc.py
--rw-r--r--   0        0        0     2624 2022-03-01 13:44:24.991679 flask-selfdoc-1.3.1a0/flask_selfdoc/templates/autodoc_default.html
--rw-r--r--   0        0        0      574 2022-03-01 13:44:24.991679 flask-selfdoc-1.3.1a0/pyproject.toml
--rw-r--r--   0        0        0      951 2022-03-01 13:45:08.241252 flask-selfdoc-1.3.1a0/setup.py
--rw-r--r--   0        0        0      581 2022-03-01 13:45:08.241596 flask-selfdoc-1.3.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-21 09:35:05.839376 flask_selfdoc-1.4.0/LICENSE
+-rw-r--r--   0        0        0      135 2023-05-21 09:35:05.839376 flask_selfdoc-1.4.0/flask_selfdoc/__init__.py
+-rw-r--r--   0        0        0    11999 2023-05-21 09:35:05.839376 flask_selfdoc-1.4.0/flask_selfdoc/autodoc.py
+-rw-r--r--   0        0        0     2624 2023-05-21 09:35:05.839376 flask_selfdoc-1.4.0/flask_selfdoc/templates/autodoc_default.html
+-rw-r--r--   0        0        0      703 2023-05-21 09:35:05.839376 flask_selfdoc-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 flask_selfdoc-1.4.0/PKG-INFO
```

### Comparing `flask-selfdoc-1.3.1a0/LICENSE` & `flask_selfdoc-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-selfdoc-1.3.1a0/flask_selfdoc/templates/autodoc_default.html` & `flask_selfdoc-1.4.0/flask_selfdoc/templates/autodoc_default.html`

 * *Files identical despite different names*

### Comparing `flask-selfdoc-1.3.1a0/pyproject.toml` & `flask_selfdoc-1.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [tool.poetry]
 name = "flask-selfdoc"
-version = "1.3.1-alpha.0"
+version = "1.4.0"
 description = "Documentation generator for flask"
 authors = ["Jack Grahl <jack.grahl@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.6"
-Flask = "^1.0"
+Flask = [
+    {python = "~3.6", version = ">=1.0, <2.1"},
+    {python = ">=3.7, <3.10", version = ">=1.0"},
+    {python = "~3.10", version = ">=1.1"}
+]
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 requests = "^2.26.0"
 
 [tool.poetry.scripts]
 test = 'run_tests:test'
```

