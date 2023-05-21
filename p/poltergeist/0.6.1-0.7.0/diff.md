# Comparing `tmp/poltergeist-0.6.1.tar.gz` & `tmp/poltergeist-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poltergeist-0.6.1.tar", max compression
+gzip compressed data, was "poltergeist-0.7.0.tar", max compression
```

## Comparing `poltergeist-0.6.1.tar` & `poltergeist-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-01-22 19:42:26.781458 poltergeist-0.6.1/LICENSE
--rw-r--r--   0        0        0     2323 2023-01-22 19:42:26.781458 poltergeist-0.6.1/README.md
--rw-r--r--   0        0        0      143 2023-01-22 19:42:26.781458 poltergeist-0.6.1/poltergeist/__init__.py
--rw-r--r--   0        0        0     1186 2023-01-22 19:42:26.781458 poltergeist-0.6.1/poltergeist/decorator.py
--rw-r--r--   0        0        0        0 2023-01-22 19:42:26.781458 poltergeist-0.6.1/poltergeist/py.typed
--rw-r--r--   0        0        0     1811 2023-01-22 19:42:26.781458 poltergeist-0.6.1/poltergeist/result.py
--rw-r--r--   0        0        0     1151 2023-01-22 19:42:52.912247 poltergeist-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3045 1970-01-01 00:00:00.000000 poltergeist-0.6.1/setup.py
--rw-r--r--   0        0        0     3218 1970-01-01 00:00:00.000000 poltergeist-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-21 17:52:34.034860 poltergeist-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2465 2023-05-21 17:52:34.034860 poltergeist-0.7.0/README.md
+-rw-r--r--   0        0        0      143 2023-05-21 17:52:34.034860 poltergeist-0.7.0/poltergeist/__init__.py
+-rw-r--r--   0        0        0      612 2023-05-21 17:52:34.034860 poltergeist-0.7.0/poltergeist/decorator.py
+-rw-r--r--   0        0        0        0 2023-05-21 17:52:34.034860 poltergeist-0.7.0/poltergeist/py.typed
+-rw-r--r--   0        0        0     1811 2023-05-21 17:52:34.034860 poltergeist-0.7.0/poltergeist/result.py
+-rw-r--r--   0        0        0     1151 2023-05-21 17:52:53.379014 poltergeist-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 poltergeist-0.7.0/setup.py
+-rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 poltergeist-0.7.0/PKG-INFO
```

### Comparing `poltergeist-0.6.1/LICENSE` & `poltergeist-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poltergeist-0.6.1/README.md` & `poltergeist-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,16 @@
 ## Examples
 
 Use the `@poltergeist` decorator on any function:
 
 ```python
 from poltergeist import poltergeist
 
-# Handle an exception type potentially raised
-# within the function (Exception by default)
-@poltergeist(error=OSError)
+# Handle an exception type potentially raised within the function
+@poltergeist(OSError)
 def read_text(path: str) -> str:
     with open(path) as f:
         return f.read()
 
 # Returns an object of type Result[str, OSError]
 result = read_text("my_file.txt")
 ```
@@ -39,25 +38,14 @@
     try:
         with open(path) as f:
             return Ok(f.read())
     except OSError as e:
         return Err(e)
 ```
 
-It's also possible to wrap multiple exception types:
-
-```python
-def read_text(path: str) -> Result[str, OSError | UnicodeDecodeError]:
-    try:
-        with open(path) as f:
-            return Ok(f.read())
-    except (OSError, UnicodeDecodeError) as e:
-        return Err(e)
-```
-
 Then handle the result in a type-safe way:
 
 ```python
 # Get the Ok value or re-raise the Err exception
 content: str = result.unwrap()
 
 # Get the Ok value or a default if it's an Err
@@ -74,14 +62,34 @@
 match result:
     case Ok(content):
         print("Text in upper:", content.upper())
     case Err(FileNotFoundError() as e):
         print("File not found:", e.filename)
 ```
 
+It's also possible to wrap multiple exception types with the decorator:
+
+```python
+@poltergeist(OSError, UnicodeDecodeError)
+def read_text(path: str) -> str:
+    with open(path) as f:
+        return f.read()
+```
+
+Or manually:
+
+```python
+def read_text(path: str) -> Result[str, OSError | UnicodeDecodeError]:
+    try:
+        with open(path) as f:
+            return Ok(f.read())
+    except (OSError, UnicodeDecodeError) as e:
+        return Err(e)
+```
+
 ## Contributing
 
 Set up the project using [Poetry](https://python-poetry.org/):
 
 ```
 poetry install
 ```
```

### Comparing `poltergeist-0.6.1/poltergeist/result.py` & `poltergeist-0.7.0/poltergeist/result.py`

 * *Files identical despite different names*

### Comparing `poltergeist-0.6.1/setup.py` & `poltergeist-0.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['poltergeist']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'poltergeist',
-    'version': '0.6.1',
+    'version': '0.7.0',
     'description': 'Rust-like error handling in Python, with type-safety in mind.',
-    'long_description': '# poltergeist\n\n[![pypi](https://img.shields.io/pypi/v/poltergeist.svg)](https://pypi.python.org/pypi/poltergeist)\n[![versions](https://img.shields.io/pypi/pyversions/poltergeist.svg)](https://github.com/alexandermalyga/poltergeist)\n\n[Rust-like error handling](https://doc.rust-lang.org/book/ch09-00-error-handling.html) in Python, with type-safety in mind.\n\n## Installation\n\n```\npip install poltergeist\n```\n\n## Examples\n\nUse the `@poltergeist` decorator on any function:\n\n```python\nfrom poltergeist import poltergeist\n\n# Handle an exception type potentially raised\n# within the function (Exception by default)\n@poltergeist(error=OSError)\ndef read_text(path: str) -> str:\n    with open(path) as f:\n        return f.read()\n\n# Returns an object of type Result[str, OSError]\nresult = read_text("my_file.txt")\n```\n\nOr wrap errors manually:\n\n```python\nfrom poltergeist import Result, Ok, Err\n\n# Equivalent to the decorated function above\ndef read_text(path: str) -> Result[str, OSError]:\n    try:\n        with open(path) as f:\n            return Ok(f.read())\n    except OSError as e:\n        return Err(e)\n```\n\nIt\'s also possible to wrap multiple exception types:\n\n```python\ndef read_text(path: str) -> Result[str, OSError | UnicodeDecodeError]:\n    try:\n        with open(path) as f:\n            return Ok(f.read())\n    except (OSError, UnicodeDecodeError) as e:\n        return Err(e)\n```\n\nThen handle the result in a type-safe way:\n\n```python\n# Get the Ok value or re-raise the Err exception\ncontent: str = result.unwrap()\n\n# Get the Ok value or a default if it\'s an Err\ncontent: str = result.unwrap_or("lorem ipsum")\ncontent: str | None = result.unwrap_or()\n\n# Get the Ok value or compute it from the exception\ncontent: str = result.unwrap_or_else(lambda e: f"The exception was: {e}")\n\n# Get the Err exception or None if it\'s an Ok\nerr: OSError | None = result.err()\n\n# Handle the result using structural pattern matching\nmatch result:\n    case Ok(content):\n        print("Text in upper:", content.upper())\n    case Err(FileNotFoundError() as e):\n        print("File not found:", e.filename)\n```\n\n## Contributing\n\nSet up the project using [Poetry](https://python-poetry.org/):\n\n```\npoetry install\n```\n\nFormat the code:\n\n```\nmake lint\n```\n\nRun tests:\n\n```\nmake test\n```\n\nCheck for typing and format issues:\n\n```\nmake check\n```\n',
+    'long_description': '# poltergeist\n\n[![pypi](https://img.shields.io/pypi/v/poltergeist.svg)](https://pypi.python.org/pypi/poltergeist)\n[![versions](https://img.shields.io/pypi/pyversions/poltergeist.svg)](https://github.com/alexandermalyga/poltergeist)\n\n[Rust-like error handling](https://doc.rust-lang.org/book/ch09-00-error-handling.html) in Python, with type-safety in mind.\n\n## Installation\n\n```\npip install poltergeist\n```\n\n## Examples\n\nUse the `@poltergeist` decorator on any function:\n\n```python\nfrom poltergeist import poltergeist\n\n# Handle an exception type potentially raised within the function\n@poltergeist(OSError)\ndef read_text(path: str) -> str:\n    with open(path) as f:\n        return f.read()\n\n# Returns an object of type Result[str, OSError]\nresult = read_text("my_file.txt")\n```\n\nOr wrap errors manually:\n\n```python\nfrom poltergeist import Result, Ok, Err\n\n# Equivalent to the decorated function above\ndef read_text(path: str) -> Result[str, OSError]:\n    try:\n        with open(path) as f:\n            return Ok(f.read())\n    except OSError as e:\n        return Err(e)\n```\n\nThen handle the result in a type-safe way:\n\n```python\n# Get the Ok value or re-raise the Err exception\ncontent: str = result.unwrap()\n\n# Get the Ok value or a default if it\'s an Err\ncontent: str = result.unwrap_or("lorem ipsum")\ncontent: str | None = result.unwrap_or()\n\n# Get the Ok value or compute it from the exception\ncontent: str = result.unwrap_or_else(lambda e: f"The exception was: {e}")\n\n# Get the Err exception or None if it\'s an Ok\nerr: OSError | None = result.err()\n\n# Handle the result using structural pattern matching\nmatch result:\n    case Ok(content):\n        print("Text in upper:", content.upper())\n    case Err(FileNotFoundError() as e):\n        print("File not found:", e.filename)\n```\n\nIt\'s also possible to wrap multiple exception types with the decorator:\n\n```python\n@poltergeist(OSError, UnicodeDecodeError)\ndef read_text(path: str) -> str:\n    with open(path) as f:\n        return f.read()\n```\n\nOr manually:\n\n```python\ndef read_text(path: str) -> Result[str, OSError | UnicodeDecodeError]:\n    try:\n        with open(path) as f:\n            return Ok(f.read())\n    except (OSError, UnicodeDecodeError) as e:\n        return Err(e)\n```\n\n## Contributing\n\nSet up the project using [Poetry](https://python-poetry.org/):\n\n```\npoetry install\n```\n\nFormat the code:\n\n```\nmake lint\n```\n\nRun tests:\n\n```\nmake test\n```\n\nCheck for typing and format issues:\n\n```\nmake check\n```\n',
     'author': 'Alexander Malyga',
     'author_email': 'alexander@malyga.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/alexandermalyga/poltergeist',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `poltergeist-0.6.1/PKG-INFO` & `poltergeist-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poltergeist
-Version: 0.6.1
+Version: 0.7.0
 Summary: Rust-like error handling in Python, with type-safety in mind.
 Home-page: https://github.com/alexandermalyga/poltergeist
 License: MIT
 Author: Alexander Malyga
 Author-email: alexander@malyga.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -36,17 +36,16 @@
 ## Examples
 
 Use the `@poltergeist` decorator on any function:
 
 ```python
 from poltergeist import poltergeist
 
-# Handle an exception type potentially raised
-# within the function (Exception by default)
-@poltergeist(error=OSError)
+# Handle an exception type potentially raised within the function
+@poltergeist(OSError)
 def read_text(path: str) -> str:
     with open(path) as f:
         return f.read()
 
 # Returns an object of type Result[str, OSError]
 result = read_text("my_file.txt")
 ```
@@ -61,25 +60,14 @@
     try:
         with open(path) as f:
             return Ok(f.read())
     except OSError as e:
         return Err(e)
 ```
 
-It's also possible to wrap multiple exception types:
-
-```python
-def read_text(path: str) -> Result[str, OSError | UnicodeDecodeError]:
-    try:
-        with open(path) as f:
-            return Ok(f.read())
-    except (OSError, UnicodeDecodeError) as e:
-        return Err(e)
-```
-
 Then handle the result in a type-safe way:
 
 ```python
 # Get the Ok value or re-raise the Err exception
 content: str = result.unwrap()
 
 # Get the Ok value or a default if it's an Err
@@ -96,14 +84,34 @@
 match result:
     case Ok(content):
         print("Text in upper:", content.upper())
     case Err(FileNotFoundError() as e):
         print("File not found:", e.filename)
 ```
 
+It's also possible to wrap multiple exception types with the decorator:
+
+```python
+@poltergeist(OSError, UnicodeDecodeError)
+def read_text(path: str) -> str:
+    with open(path) as f:
+        return f.read()
+```
+
+Or manually:
+
+```python
+def read_text(path: str) -> Result[str, OSError | UnicodeDecodeError]:
+    try:
+        with open(path) as f:
+            return Ok(f.read())
+    except (OSError, UnicodeDecodeError) as e:
+        return Err(e)
+```
+
 ## Contributing
 
 Set up the project using [Poetry](https://python-poetry.org/):
 
 ```
 poetry install
 ```
```

