# Comparing `tmp/t_python_markdown-1.4.0.tar.gz` & `tmp/t_python_markdown-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t_python_markdown-1.4.0.tar", last modified: Sat May 13 19:29:16 2023, max compression
+gzip compressed data, was "t_python_markdown-1.4.1.tar", last modified: Sun May 21 12:26:46 2023, max compression
```

## Comparing `t_python_markdown-1.4.0.tar` & `t_python_markdown-1.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 19:29:16.875731 t_python_markdown-1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-05-13 19:28:57.000000 t_python_markdown-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4225 2023-05-13 19:29:16.875731 t_python_markdown-1.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2351 2023-05-13 19:28:57.000000 t_python_markdown-1.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-05-13 19:28:57.000000 t_python_markdown-1.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-13 19:29:16.875731 t_python_markdown-1.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 19:29:16.873731 t_python_markdown-1.4.0/t_python_markdown/
--rw-rw-rw-   0 root         (0) root         (0)      789 2023-05-13 19:28:57.000000 t_python_markdown-1.4.0/t_python_markdown/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 19:29:16.875731 t_python_markdown-1.4.0/t_python_markdown/extensions/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-13 19:28:57.000000 t_python_markdown-1.4.0/t_python_markdown/extensions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1666 2023-05-13 19:28:57.000000 t_python_markdown-1.4.0/t_python_markdown/extensions/mkdocs.py
--rw-rw-rw-   0 root         (0) root         (0)    11048 2023-05-13 19:28:57.000000 t_python_markdown-1.4.0/t_python_markdown/t_python_markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 19:29:16.874731 t_python_markdown-1.4.0/t_python_markdown.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4225 2023-05-13 19:29:16.000000 t_python_markdown-1.4.0/t_python_markdown.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      385 2023-05-13 19:29:16.000000 t_python_markdown-1.4.0/t_python_markdown.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-13 19:29:16.000000 t_python_markdown-1.4.0/t_python_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-05-13 19:29:16.000000 t_python_markdown-1.4.0/t_python_markdown.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-13 19:29:16.000000 t_python_markdown-1.4.0/t_python_markdown.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:46.497961 t_python_markdown-1.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-05-21 12:26:27.000000 t_python_markdown-1.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4351 2023-05-21 12:26:46.496961 t_python_markdown-1.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-05-21 12:26:27.000000 t_python_markdown-1.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-05-21 12:26:27.000000 t_python_markdown-1.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 12:26:46.497961 t_python_markdown-1.4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:46.495961 t_python_markdown-1.4.1/t_python_markdown/
+-rw-rw-rw-   0 root         (0) root         (0)      789 2023-05-21 12:26:27.000000 t_python_markdown-1.4.1/t_python_markdown/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:46.496961 t_python_markdown-1.4.1/t_python_markdown/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-21 12:26:27.000000 t_python_markdown-1.4.1/t_python_markdown/extensions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1666 2023-05-21 12:26:27.000000 t_python_markdown-1.4.1/t_python_markdown/extensions/mkdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)    11086 2023-05-21 12:26:27.000000 t_python_markdown-1.4.1/t_python_markdown/t_python_markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:46.496961 t_python_markdown-1.4.1/t_python_markdown.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4351 2023-05-21 12:26:46.000000 t_python_markdown-1.4.1/t_python_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      385 2023-05-21 12:26:46.000000 t_python_markdown-1.4.1/t_python_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 12:26:46.000000 t_python_markdown-1.4.1/t_python_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-05-21 12:26:46.000000 t_python_markdown-1.4.1/t_python_markdown.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-21 12:26:46.000000 t_python_markdown-1.4.1/t_python_markdown.egg-info/top_level.txt
```

### Comparing `t_python_markdown-1.4.0/LICENSE` & `t_python_markdown-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `t_python_markdown-1.4.0/PKG-INFO` & `t_python_markdown-1.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_python_markdown
-Version: 1.4.0
+Version: 1.4.1
 Summary: A simple to use markdown generator for Python.
 Author-email: t-python-markdown <t-python-markdown@toyne.cix.co.uk>
 Maintainer-email: t-python-markdown <t-python-markdown@toyne.cix.co.uk>
 License: MIT License
         
         Copyright (c) 2023 Toyne
         
@@ -110,14 +110,17 @@
 
 
 ## Usage
 For usage, see https://www.cix.co.uk/~toyne/t-python-markdown/usage/
 
 
 ## Recent Changelog
+**1.4.1**  
+- Resolve issue where embedding tables in lists in tables in lists in tables (etc...) would not render correctly
+
 **1.4.0**  
 - Improve support for embedded lists and tables. Now able to wrap child items in other markdown elements
 
 **1.3.2**  
 - Add support for attribute lists when processing embedded lists
 
 **1.3.1**
```

### Comparing `t_python_markdown-1.4.0/README.md` & `t_python_markdown-1.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,17 @@
 
 
 ## Usage
 For usage, see https://www.cix.co.uk/~toyne/t-python-markdown/usage/
 
 
 ## Recent Changelog
+**1.4.1**  
+- Resolve issue where embedding tables in lists in tables in lists in tables (etc...) would not render correctly
+
 **1.4.0**  
 - Improve support for embedded lists and tables. Now able to wrap child items in other markdown elements
 
 **1.3.2**  
 - Add support for attribute lists when processing embedded lists
 
 **1.3.1**
```

### Comparing `t_python_markdown-1.4.0/pyproject.toml` & `t_python_markdown-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "t_python_markdown"
 description = "A simple to use markdown generator for Python."
 readme = "README.md"
-version = "1.4.0"
+version = "1.4.1"
 license = {file = "LICENSE"}
 keywords = ["markdown"]
 authors = [
     { name="t-python-markdown", email="t-python-markdown@toyne.cix.co.uk" },
 ]
 maintainers = [
     { name="t-python-markdown", email="t-python-markdown@toyne.cix.co.uk" },
```

### Comparing `t_python_markdown-1.4.0/t_python_markdown/__init__.py` & `t_python_markdown-1.4.1/t_python_markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `t_python_markdown-1.4.0/t_python_markdown/extensions/mkdocs.py` & `t_python_markdown-1.4.1/t_python_markdown/extensions/mkdocs.py`

 * *Files identical despite different names*

### Comparing `t_python_markdown-1.4.0/t_python_markdown/t_python_markdown.py` & `t_python_markdown-1.4.1/t_python_markdown/t_python_markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
 
   def _render_item_complete(self, _parent, _s):
     if isinstance(_parent, (List)):
       return "\n".join(_s)
     return "\n" + "\n".join(_s) + "\n"
 
   def __check_indent(self, _o, _count=0):
-    if _o._parent:  # pylint: disable=W0212
+    if _o._parent and not isinstance(_o._parent, Table):  # pylint: disable=W0212
       _c = _count + 1 if isinstance(_o._parent, List) else _count  # pylint: disable=W0212
       return self.__check_indent(_o._parent, _c)  # pylint: disable=W0212
     return _count
 
 
 class UnorderedList(List):
   """Represents markdown unordered list"""
```

### Comparing `t_python_markdown-1.4.0/t_python_markdown.egg-info/PKG-INFO` & `t_python_markdown-1.4.1/t_python_markdown.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t-python-markdown
-Version: 1.4.0
+Version: 1.4.1
 Summary: A simple to use markdown generator for Python.
 Author-email: t-python-markdown <t-python-markdown@toyne.cix.co.uk>
 Maintainer-email: t-python-markdown <t-python-markdown@toyne.cix.co.uk>
 License: MIT License
         
         Copyright (c) 2023 Toyne
         
@@ -110,14 +110,17 @@
 
 
 ## Usage
 For usage, see https://www.cix.co.uk/~toyne/t-python-markdown/usage/
 
 
 ## Recent Changelog
+**1.4.1**  
+- Resolve issue where embedding tables in lists in tables in lists in tables (etc...) would not render correctly
+
 **1.4.0**  
 - Improve support for embedded lists and tables. Now able to wrap child items in other markdown elements
 
 **1.3.2**  
 - Add support for attribute lists when processing embedded lists
 
 **1.3.1**
```

