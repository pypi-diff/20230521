# Comparing `tmp/pip-licenses-4.3.1.tar.gz` & `tmp/pip-licenses-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pip-licenses-4.3.1.tar", last modified: Thu May  4 02:33:00 2023, max compression
+gzip compressed data, was "dist/pip-licenses-4.3.2.tar", last modified: Sun May 21 02:56:34 2023, max compression
```

## Comparing `pip-licenses-4.3.1.tar` & `pip-licenses-4.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-05-04 02:33:00.846429 pip-licenses-4.3.1/
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     5499 2023-05-04 02:29:28.000000 pip-licenses-4.3.1/CHANGELOG.md
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1063 2020-12-06 15:11:59.000000 pip-licenses-4.3.1/LICENSE
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)      129 2022-12-04 03:57:54.000000 pip-licenses-4.3.1/MANIFEST.in
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    31115 2023-05-04 02:33:00.846429 pip-licenses-4.3.1/PKG-INFO
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    21661 2023-04-25 08:07:16.000000 pip-licenses-4.3.1/README.md
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-05-04 02:33:00.846429 pip-licenses-4.3.1/pip_licenses.egg-info/
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    31115 2023-05-04 02:33:00.000000 pip-licenses-4.3.1/pip_licenses.egg-info/PKG-INFO
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)      361 2023-05-04 02:33:00.000000 pip-licenses-4.3.1/pip_licenses.egg-info/SOURCES.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)        1 2023-05-04 02:33:00.000000 pip-licenses-4.3.1/pip_licenses.egg-info/dependency_links.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       51 2023-05-04 02:33:00.000000 pip-licenses-4.3.1/pip_licenses.egg-info/entry_points.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       85 2023-05-04 02:33:00.000000 pip-licenses-4.3.1/pip_licenses.egg-info/requires.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       12 2023-05-04 02:33:00.000000 pip-licenses-4.3.1/pip_licenses.egg-info/top_level.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    33206 2023-05-04 02:26:34.000000 pip-licenses-4.3.1/piplicenses.py
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)        0 2022-12-04 03:57:54.000000 pip-licenses-4.3.1/py.typed
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1367 2023-05-04 02:33:00.846429 pip-licenses-4.3.1/setup.cfg
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     2347 2022-12-04 03:57:54.000000 pip-licenses-4.3.1/setup.py
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    35764 2023-05-04 02:22:44.000000 pip-licenses-4.3.1/test_piplicenses.py
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-05-04 02:33:00.846429 pip-licenses-4.3.1/tests/
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-05-04 02:33:00.846429 pip-licenses-4.3.1/tests/fixtures/
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       16 2020-12-06 15:11:59.000000 pip-licenses-4.3.1/tests/fixtures/unicode_characters.txt
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-05-21 02:56:34.430612 pip-licenses-4.3.2/
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     5564 2023-05-21 02:52:57.000000 pip-licenses-4.3.2/CHANGELOG.md
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1063 2020-12-06 15:11:59.000000 pip-licenses-4.3.2/LICENSE
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)      129 2022-12-04 03:57:54.000000 pip-licenses-4.3.2/MANIFEST.in
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    31195 2023-05-21 02:56:34.430612 pip-licenses-4.3.2/PKG-INFO
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    21661 2023-04-25 08:07:16.000000 pip-licenses-4.3.2/README.md
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-05-21 02:56:34.430612 pip-licenses-4.3.2/pip_licenses.egg-info/
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    31195 2023-05-21 02:56:34.000000 pip-licenses-4.3.2/pip_licenses.egg-info/PKG-INFO
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)      361 2023-05-21 02:56:34.000000 pip-licenses-4.3.2/pip_licenses.egg-info/SOURCES.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)        1 2023-05-21 02:56:34.000000 pip-licenses-4.3.2/pip_licenses.egg-info/dependency_links.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       51 2023-05-21 02:56:34.000000 pip-licenses-4.3.2/pip_licenses.egg-info/entry_points.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       85 2023-05-21 02:56:34.000000 pip-licenses-4.3.2/pip_licenses.egg-info/requires.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       12 2023-05-21 02:56:34.000000 pip-licenses-4.3.2/pip_licenses.egg-info/top_level.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    33275 2023-05-21 02:51:05.000000 pip-licenses-4.3.2/piplicenses.py
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)        0 2022-12-04 03:57:54.000000 pip-licenses-4.3.2/py.typed
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1367 2023-05-21 02:56:34.430612 pip-licenses-4.3.2/setup.cfg
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     2347 2022-12-04 03:57:54.000000 pip-licenses-4.3.2/setup.py
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    36224 2023-05-21 02:50:40.000000 pip-licenses-4.3.2/test_piplicenses.py
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-05-21 02:56:34.420612 pip-licenses-4.3.2/tests/
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-05-21 02:56:34.430612 pip-licenses-4.3.2/tests/fixtures/
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       16 2020-12-06 15:11:59.000000 pip-licenses-4.3.2/tests/fixtures/unicode_characters.txt
```

### Comparing `pip-licenses-4.3.1/CHANGELOG.md` & `pip-licenses-4.3.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ## CHANGELOG
 
+### 4.3.2
+
+* Better Handling extracting URLs from `Project-URL`
+
 ### 4.3.1
 
 * Fix to treat package names as normalized as in [PEP 503](https://peps.python.org/pep-0503/) with `--packages` and `--ignore-packages` option
 
 ### 4.3.0
 
 * Implement new option `--no-version`
```

### Comparing `pip-licenses-4.3.1/LICENSE` & `pip-licenses-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.3.1/PKG-INFO` & `pip-licenses-4.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-licenses
-Version: 4.3.1
+Version: 4.3.2
 Summary: Dump the software license list of Python packages installed with pip.
 Home-page: https://github.com/raimon49/pip-licenses
 Author: raimon
 Author-email: raimon49@hotmail.com
 License: MIT
 Project-URL: Releases, https://github.com/raimon49/pip-licenses/releases
 Project-URL: Issues, https://github.com/raimon49/pip-licenses/issues
@@ -825,14 +825,21 @@
 .. |PyPI - Downloads| image:: https://img.shields.io/pypi/dm/pip-licenses
    :target: https://pypistats.org/packages/pip-licenses
 
 
 CHANGELOG
 ---------
 
+.. _432:
+
+4.3.2
+~~~~~
+
+-  Better Handling extracting URLs from ``Project-URL``
+
 .. _431:
 
 4.3.1
 ~~~~~
 
 -  Fix to treat package names as normalized as in `PEP
    503 <https://peps.python.org/pep-0503/>`__ with ``--packages`` and
```

### Comparing `pip-licenses-4.3.1/README.md` & `pip-licenses-4.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.3.1/pip_licenses.egg-info/PKG-INFO` & `pip-licenses-4.3.2/pip_licenses.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-licenses
-Version: 4.3.1
+Version: 4.3.2
 Summary: Dump the software license list of Python packages installed with pip.
 Home-page: https://github.com/raimon49/pip-licenses
 Author: raimon
 Author-email: raimon49@hotmail.com
 License: MIT
 Project-URL: Releases, https://github.com/raimon49/pip-licenses/releases
 Project-URL: Issues, https://github.com/raimon49/pip-licenses/issues
@@ -825,14 +825,21 @@
 .. |PyPI - Downloads| image:: https://img.shields.io/pypi/dm/pip-licenses
    :target: https://pypistats.org/packages/pip-licenses
 
 
 CHANGELOG
 ---------
 
+.. _432:
+
+4.3.2
+~~~~~
+
+-  Better Handling extracting URLs from ``Project-URL``
+
 .. _431:
 
 4.3.1
 ~~~~~
 
 -  Fix to treat package names as normalized as in `PEP
    503 <https://peps.python.org/pep-0503/>`__ with ``--packages`` and
```

### Comparing `pip-licenses-4.3.1/piplicenses.py` & `pip-licenses-4.3.2/piplicenses.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     from email.message import Message
     from typing import Callable, Dict, Iterator, Optional, Sequence
 
 
 open = open  # allow monkey patching
 
 __pkgname__ = "pip-licenses"
-__version__ = "4.3.1"
+__version__ = "4.3.2"
 __author__ = "raimon"
 __license__ = "MIT"
 __summary__ = (
     "Dump the software license list of Python packages installed with pip."
 )
 __url__ = "https://github.com/raimon49/pip-licenses"
 
@@ -116,17 +116,23 @@
     if homepage is not None:
         return homepage
 
     candidates: Dict[str, str] = {}
 
     for entry in metadata.get_all("Project-URL", []):
         key, value = entry.split(",", 1)
-        candidates[key.strip()] = value.strip()
+        candidates[key.strip().lower()] = value.strip()
 
-    for priority_key in ["Homepage", "Source", "Changelog", "Bug Tracker"]:
+    for priority_key in [
+        "homepage",
+        "source",
+        "repository",
+        "changelog",
+        "bug tracker",
+    ]:
         if priority_key in candidates:
             return candidates[priority_key]
 
     return None
 
 
 PATTERN_DELIMITER = re.compile(r"[-_.]+")
```

### Comparing `pip-licenses-4.3.1/setup.cfg` & `pip-licenses-4.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.3.1/setup.py` & `pip-licenses-4.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.3.1/test_piplicenses.py` & `pip-licenses-4.3.2/test_piplicenses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1000,7 +1000,22 @@
     metadata.get.return_value = None
     metadata.get_all.return_value = []
 
     assert None is extract_homepage(metadata=metadata)  # type: ignore
 
     metadata.get.assert_called_once_with("home-page", None)
     metadata.get_all.assert_called_once_with("Project-URL", [])
+
+
+def test_extract_homepage_project_uprl_fallback_capitalisation() -> None:
+    metadata = MagicMock()
+    metadata.get.return_value = None
+
+    # `homepage` is still prioritized higher than `Source` (capitalisation)
+    metadata.get_all.return_value = [
+        "Source, source",
+        "homepage, homepage",
+    ]
+
+    assert "homepage" == extract_homepage(metadata=metadata)  # type: ignore
+
+    metadata.get_all.assert_called_once_with("Project-URL", [])
```

