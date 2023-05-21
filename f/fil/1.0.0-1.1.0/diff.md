# Comparing `tmp/fil-1.0.0.tar.gz` & `tmp/fil-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fil-1.0.0.tar", max compression
+gzip compressed data, was "fil-1.1.0.tar", max compression
```

## Comparing `fil-1.0.0.tar` & `fil-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      782 2023-05-02 15:39:14.592872 fil-1.0.0/README.md
--rw-r--r--   0        0        0     5353 2023-05-02 15:34:01.648332 fil-1.0.0/fil.py
--rw-r--r--   0        0        0      496 2023-05-02 15:39:39.873581 fil-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 fil-1.0.0/setup.py
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 fil-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      782 2023-05-02 15:39:14.592872 fil-1.1.0/README.md
+-rw-r--r--   0        0        0     5579 2023-05-21 10:49:57.389177 fil-1.1.0/fil.py
+-rw-r--r--   0        0        0      496 2023-05-21 10:50:21.836044 fil-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 fil-1.1.0/setup.py
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 fil-1.1.0/PKG-INFO
```

### Comparing `fil-1.0.0/README.md` & `fil-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fil-1.0.0/fil.py` & `fil-1.1.0/fil.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,39 +22,46 @@
     # Write an iterator to a JSON Line file
     dicts = ({'key': i} for i in range(10))
     fil.write(dicts, 'file.jsonl')
 """
 
 from functools import cached_property
 from pathlib import Path
-from typing import Dict, Iterator, List, Optional, Union
+from typing import Any, Dict, Iterator, List, Optional, Union
 import json
 import safer
 
 __all__ = 'read', 'write', 'SUFFIX_TO_CLASS'
 
 # JSON is the type used by JSON, TOML, or Yaml
 JSON = Union[Dict, List, None, bool, float, int, str]
 JSON_Lines = Iterator[JSON]
 FileData = Union[JSON, JSON_Lines]
 FilePath = Union[Path, str]
+_NONE = object()
 
 
-def read(path: FilePath) -> FileData:
+def read(path: FilePath, default: Any = _NONE) -> FileData:
     """
     Reads data from a file based on its suffix
 
     Returns:
        JSON, or an iterator of JSON records, if the file is JSON Lines
 
     Args:
       path: the string or path to the file to read
+      default: a default to return if there is any error in reading the file
     """
     p = Path(path)
-    return _get_class(p).read(p)
+    try:
+        return _get_class(p).read(p)
+    except Exception:
+        if default is _NONE:
+            raise
+        return default
 
 
 def write(
     data: FileData,
     path: FilePath,
     *,
     use_safer: Optional[bool] = None,
```

### Comparing `fil-1.0.0/setup.py` & `fil-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 modules = \
 ['fil']
 install_requires = \
 ['safer>=4.6.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'fil',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': '🏺 Read/write JSON/TOML/Yaml/txt 🏺',
     'long_description': "## Example 1: read a file\n\n    d1 = fil.read('file.json')   # Any Json\n    d2 = fil.read('file.toml')   # A dict\n    d3 = fil.read('file.yaml')   # Any JSON\n    d4 = fil.read('file.txt')    # A string\n\n    # Reading a JSON Line file returns an interator:\n    for record in fil.read('file.jsonl'):\n        print(record)  # A sequence of JSON\n\n## Example 2: write to a file\n\n    fil.write(d1, 'file.json')  # d1 can be any JSON\n    fil.write(d2, 'file.toml')  # d2 must be a dict\n    fil.write(d3, 'file.yaml')  # d3 can be any JSON\n    fil.write(d4, 'file.txt')   # d4 most be a str\n\n    # Write an iterator to a JSON Line file\n    dicts = ({'key': i} for i in range(10))\n    fil.write(dicts, 'file.jsonl')\n\n\n### [API Documentation](https://rec.github.io/fil#fil--api-documentation)\n",
     'author': 'Tom Ritchford',
     'author_email': 'tom@swirly.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fil-1.0.0/PKG-INFO` & `fil-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fil
-Version: 1.0.0
+Version: 1.1.0
 Summary: 🏺 Read/write JSON/TOML/Yaml/txt 🏺
 License: MIT
 Author: Tom Ritchford
 Author-email: tom@swirly.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

