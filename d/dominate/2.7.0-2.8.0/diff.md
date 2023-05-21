# Comparing `tmp/dominate-2.7.0.tar.gz` & `tmp/dominate-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dominate-2.7.0.tar", last modified: Mon Jul 25 06:44:59 2022, max compression
+gzip compressed data, was "dominate-2.8.0.tar", last modified: Sun May 21 19:32:52 2023, max compression
```

## Comparing `dominate-2.7.0.tar` & `dominate-2.8.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 tom       (1001) tom       (1001)        0 2022-07-25 06:44:59.670655 dominate-2.7.0/
--rw-rw-r--   0 tom       (1001) tom       (1001)     7637 2018-09-25 02:45:41.000000 dominate-2.7.0/LICENSE.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)      112 2018-09-25 02:45:41.000000 dominate-2.7.0/MANIFEST.in
--rw-r--r--   0 tom       (1001) tom       (1001)    18389 2022-07-25 06:44:59.670655 dominate-2.7.0/PKG-INFO
--rw-r--r--   0 tom       (1001) tom       (1001)    12270 2022-07-25 06:39:55.000000 dominate-2.7.0/README.md
-drwxr-xr-x   0 tom       (1001) tom       (1001)        0 2022-07-25 06:44:59.670655 dominate-2.7.0/dominate/
--rw-rw-r--   0 tom       (1001) tom       (1001)       88 2018-09-25 02:45:41.000000 dominate-2.7.0/dominate/__init__.py
--rw-r--r--   0 tom       (1001) tom       (1001)       22 2022-07-25 06:39:55.000000 dominate-2.7.0/dominate/_version.py
--rw-r--r--   0 tom       (1001) tom       (1001)     2243 2022-07-25 06:39:55.000000 dominate-2.7.0/dominate/document.py
--rw-r--r--   0 tom       (1001) tom       (1001)     1734 2022-07-25 06:39:55.000000 dominate-2.7.0/dominate/dom1core.py
--rw-r--r--   0 tom       (1001) tom       (1001)    12662 2022-07-25 06:39:55.000000 dominate-2.7.0/dominate/dom_tag.py
--rw-r--r--   0 tom       (1001) tom       (1001)     9121 2022-07-25 06:39:55.000000 dominate-2.7.0/dominate/svg.py
--rw-r--r--   0 tom       (1001) tom       (1001)    28643 2022-07-25 06:39:55.000000 dominate-2.7.0/dominate/tags.py
--rw-r--r--   0 tom       (1001) tom       (1001)     4311 2022-07-25 06:39:55.000000 dominate-2.7.0/dominate/util.py
-drwxr-xr-x   0 tom       (1001) tom       (1001)        0 2022-07-25 06:44:59.670655 dominate-2.7.0/dominate.egg-info/
--rw-rw-r--   0 tom       (1001) tom       (1001)    18389 2022-07-25 06:44:59.000000 dominate-2.7.0/dominate.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1001) tom       (1001)      460 2022-07-25 06:44:59.000000 dominate-2.7.0/dominate.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)        1 2022-07-25 06:44:59.000000 dominate-2.7.0/dominate.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)        9 2022-07-25 06:44:59.000000 dominate-2.7.0/dominate.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)      106 2022-07-25 06:44:59.670655 dominate-2.7.0/setup.cfg
--rw-r--r--   0 tom       (1001) tom       (1001)     2403 2022-07-25 06:39:55.000000 dominate-2.7.0/setup.py
-drwxr-xr-x   0 tom       (1001) tom       (1001)        0 2022-07-25 06:44:59.670655 dominate-2.7.0/tests/
--rw-r--r--   0 tom       (1001) tom       (1001)     1759 2022-07-25 06:39:55.000000 dominate-2.7.0/tests/test_document.py
--rw-r--r--   0 tom       (1001) tom       (1001)      661 2022-07-25 06:39:55.000000 dominate-2.7.0/tests/test_dom1core.py
--rw-r--r--   0 tom       (1001) tom       (1001)      357 2022-07-25 06:39:55.000000 dominate-2.7.0/tests/test_dominate.py
--rw-r--r--   0 tom       (1001) tom       (1001)     7145 2022-07-25 06:39:55.000000 dominate-2.7.0/tests/test_html.py
--rw-rw-r--   0 tom       (1001) tom       (1001)    10000 2019-08-04 04:52:29.000000 dominate-2.7.0/tests/test_svg.py
--rw-r--r--   0 tom       (1001) tom       (1001)      994 2022-07-25 06:39:55.000000 dominate-2.7.0/tests/test_utils.py
+drwxr-xr-x   0 tom       (1001) tom       (1001)        0 2023-05-21 19:32:52.816259 dominate-2.8.0/
+-rw-rw-r--   0 tom       (1001) tom       (1001)     7637 2018-09-25 02:45:41.000000 dominate-2.8.0/LICENSE.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)      112 2018-09-25 02:45:41.000000 dominate-2.8.0/MANIFEST.in
+-rw-r--r--   0 tom       (1001) tom       (1001)    18389 2023-05-21 19:32:52.816259 dominate-2.8.0/PKG-INFO
+-rw-r--r--   0 tom       (1001) tom       (1001)    12270 2022-07-25 06:39:55.000000 dominate-2.8.0/README.md
+drwxr-xr-x   0 tom       (1001) tom       (1001)        0 2023-05-21 19:32:52.812259 dominate-2.8.0/dominate/
+-rw-rw-r--   0 tom       (1001) tom       (1001)       88 2018-09-25 02:45:41.000000 dominate-2.8.0/dominate/__init__.py
+-rw-r--r--   0 tom       (1001) tom       (1001)       22 2023-05-21 19:32:15.000000 dominate-2.8.0/dominate/_version.py
+-rw-r--r--   0 tom       (1001) tom       (1001)     2243 2022-07-25 06:39:55.000000 dominate-2.8.0/dominate/document.py
+-rw-r--r--   0 tom       (1001) tom       (1001)     1734 2022-07-25 06:39:55.000000 dominate-2.8.0/dominate/dom1core.py
+-rw-r--r--   0 tom       (1001) tom       (1001)    12704 2023-05-21 19:32:15.000000 dominate-2.8.0/dominate/dom_tag.py
+-rw-r--r--   0 tom       (1001) tom       (1001)     9121 2022-07-25 06:39:55.000000 dominate-2.8.0/dominate/svg.py
+-rw-r--r--   0 tom       (1001) tom       (1001)    28643 2022-07-25 06:39:55.000000 dominate-2.8.0/dominate/tags.py
+-rw-r--r--   0 tom       (1001) tom       (1001)     4311 2022-07-25 06:39:55.000000 dominate-2.8.0/dominate/util.py
+drwxr-xr-x   0 tom       (1001) tom       (1001)        0 2023-05-21 19:32:52.812259 dominate-2.8.0/dominate.egg-info/
+-rw-rw-r--   0 tom       (1001) tom       (1001)    18389 2023-05-21 19:32:52.000000 dominate-2.8.0/dominate.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1001) tom       (1001)      482 2023-05-21 19:32:52.000000 dominate-2.8.0/dominate.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)        1 2023-05-21 19:32:52.000000 dominate-2.8.0/dominate.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)        9 2023-05-21 19:32:52.000000 dominate-2.8.0/dominate.egg-info/top_level.txt
+-rw-rw-r--   0 tom       (1001) tom       (1001)      106 2023-05-21 19:32:52.816259 dominate-2.8.0/setup.cfg
+-rw-r--r--   0 tom       (1001) tom       (1001)     2403 2022-07-25 06:39:55.000000 dominate-2.8.0/setup.py
+drwxr-xr-x   0 tom       (1001) tom       (1001)        0 2023-05-21 19:32:52.816259 dominate-2.8.0/tests/
+-rw-r--r--   0 tom       (1001) tom       (1001)     1857 2023-03-05 21:15:17.000000 dominate-2.8.0/tests/test_document.py
+-rw-r--r--   0 tom       (1001) tom       (1001)      898 2023-03-05 21:15:17.000000 dominate-2.8.0/tests/test_dom1core.py
+-rw-r--r--   0 tom       (1001) tom       (1001)     1898 2023-05-21 19:32:15.000000 dominate-2.8.0/tests/test_dom_tag.py
+-rw-r--r--   0 tom       (1001) tom       (1001)      357 2023-05-21 19:32:15.000000 dominate-2.8.0/tests/test_dominate.py
+-rw-r--r--   0 tom       (1001) tom       (1001)     7145 2022-07-25 06:39:55.000000 dominate-2.8.0/tests/test_html.py
+-rw-rw-r--   0 tom       (1001) tom       (1001)    10000 2019-08-04 04:52:29.000000 dominate-2.8.0/tests/test_svg.py
+-rw-r--r--   0 tom       (1001) tom       (1001)      994 2022-07-25 06:39:55.000000 dominate-2.8.0/tests/test_utils.py
```

### Comparing `dominate-2.7.0/LICENSE.txt` & `dominate-2.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dominate-2.7.0/PKG-INFO` & `dominate-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dominate
-Version: 2.7.0
+Version: 2.8.0
 Summary: Dominate is a Python library for creating and manipulating HTML documents using an elegant DOM API.
 Home-page: https://github.com/Knio/dominate/
 Author: Tom Flanagan and Jake Wharton
 Author-email: tom@zkpq.ca
 License: LGPLv3
 Description: Dominate
         ========
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dominate Version: 2.7.0 Summary: Dominate is a
+Metadata-Version: 2.1 Name: dominate Version: 2.8.0 Summary: Dominate is a
 Python library for creating and manipulating HTML documents using an elegant
 DOM API. Home-page: https://github.com/Knio/dominate/ Author: Tom Flanagan and
 Jake Wharton Author-email: tom@zkpq.ca License: LGPLv3 Description: Dominate
 ======== `Dominate` is a Python library for creating and manipulating HTML
 documents using an elegant DOM API. It allows you to write HTML pages in pure
 Python very concisely, which eliminates the need to learn another template
 language, and lets you take advantage of the more powerful features of Python.
```

### Comparing `dominate-2.7.0/README.md` & `dominate-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dominate-2.7.0/dominate/document.py` & `dominate-2.8.0/dominate/document.py`

 * *Files identical despite different names*

### Comparing `dominate-2.7.0/dominate/dom1core.py` & `dominate-2.8.0/dominate/dom1core.py`

 * *Files identical despite different names*

### Comparing `dominate-2.7.0/dominate/dom_tag.py` & `dominate-2.8.0/dominate/dom_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 from collections import defaultdict, namedtuple
 from functools import wraps
 import threading
 
 try:
   # Python 3
   from collections.abc import Callable
-except ImportError:
+except ImportError: # pragma: no cover
   # Python 2.7
   from collections import Callable
 
 try:
   basestring = basestring
-except NameError: # py3
+except NameError: # py3 # pragma: no cover
   basestring = str
   unicode = str
 
 
 try:
   import greenlet
 except ImportError:
@@ -187,17 +187,17 @@
         obj = str(obj)
 
       if isinstance(obj, basestring):
         obj = util.escape(obj)
         self.children.append(obj)
 
       elif isinstance(obj, dom_tag):
-        stack = dom_tag._with_contexts.get(_get_thread_context())
-        if stack:
-          stack[-1].used.add(obj)
+        stack = dom_tag._with_contexts.get(_get_thread_context(), [])
+        for s in stack:
+          s.used.add(obj)
         self.children.append(obj)
         obj.parent = self
 
       elif isinstance(obj, dict):
         for attr, value in obj.items():
           self.set_attribute(*dom_tag.clean_pair(attr, value))
 
@@ -261,15 +261,15 @@
     Returns the stored value of the specified attribute or child
     (if it exists).
     '''
     if isinstance(key, int):
       # Children are accessed using integers
       try:
         return object.__getattribute__(self, 'children')[key]
-      except KeyError:
+      except IndexError:
         raise IndexError('Child with index "%s" does not exist.' % key)
     elif isinstance(key, basestring):
       # Attributes are accessed using strings
       try:
         return object.__getattribute__(self, 'attributes')[key]
       except KeyError:
         raise AttributeError('Attribute "%s" does not exist.' % key)
```

### Comparing `dominate-2.7.0/dominate/svg.py` & `dominate-2.8.0/dominate/svg.py`

 * *Files identical despite different names*

### Comparing `dominate-2.7.0/dominate/tags.py` & `dominate-2.8.0/dominate/tags.py`

 * *Files identical despite different names*

### Comparing `dominate-2.7.0/dominate/util.py` & `dominate-2.8.0/dominate/util.py`

 * *Files identical despite different names*

### Comparing `dominate-2.7.0/dominate.egg-info/PKG-INFO` & `dominate-2.8.0/dominate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dominate
-Version: 2.7.0
+Version: 2.8.0
 Summary: Dominate is a Python library for creating and manipulating HTML documents using an elegant DOM API.
 Home-page: https://github.com/Knio/dominate/
 Author: Tom Flanagan and Jake Wharton
 Author-email: tom@zkpq.ca
 License: LGPLv3
 Description: Dominate
         ========
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dominate Version: 2.7.0 Summary: Dominate is a
+Metadata-Version: 2.1 Name: dominate Version: 2.8.0 Summary: Dominate is a
 Python library for creating and manipulating HTML documents using an elegant
 DOM API. Home-page: https://github.com/Knio/dominate/ Author: Tom Flanagan and
 Jake Wharton Author-email: tom@zkpq.ca License: LGPLv3 Description: Dominate
 ======== `Dominate` is a Python library for creating and manipulating HTML
 documents using an elegant DOM API. It allows you to write HTML pages in pure
 Python very concisely, which eliminates the need to learn another template
 language, and lets you take advantage of the more powerful features of Python.
```

### Comparing `dominate-2.7.0/setup.py` & `dominate-2.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `dominate-2.7.0/tests/test_document.py` & `dominate-2.8.0/tests/test_document.py`

 * *Files 12% similar despite different names*

```diff
@@ -106,11 +106,14 @@
   d = document(title=None, doctype=None, lang='en')
   assert d.render() == \
 '''<html lang="en">
   <head></head>
   <body></body>
 </html>'''
 
+def test_repr():
+  d = document(title='foo')
+  assert d.__repr__() == '<dominate.document "foo">'
 
 if __name__ == '__main__':
   # test_doc()
   test_decorator()
```

### Comparing `dominate-2.7.0/tests/test_dom1core.py` & `dominate-2.8.0/tests/test_dom1core.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,19 +9,26 @@
     s2 = span('World', id='span2')
 
   s3 = span('foobar', id='span3')
   dom.appendChild(s3)
   assert container.getElementById('base') is dom
   assert container.getElementById('span1') is s1
   assert container.getElementById('span3') is s3
+  assert container.getElementById('foo') is None
   assert container.getElementsByTagName('span') == [s1, s2, s3]
   assert container.getElementsByTagName('SPAN') == [s1, s2, s3]
-
+  assert container.getElementsByTagName(1234) is None
 
 def test_element():
   d = div(
     span(id='a'),
     span(id='a'),
   )
   with pytest.raises(ValueError):
     d.getElementById('a')
 
+def test_parent_node():
+  parent = div(id='parent')
+  child = div(id='child')
+  parent.add(child)
+
+  assert child.parentNode is parent
```

### Comparing `dominate-2.7.0/tests/test_html.py` & `dominate-2.8.0/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `dominate-2.7.0/tests/test_svg.py` & `dominate-2.8.0/tests/test_svg.py`

 * *Files identical despite different names*

### Comparing `dominate-2.7.0/tests/test_utils.py` & `dominate-2.8.0/tests/test_utils.py`

 * *Files identical despite different names*

