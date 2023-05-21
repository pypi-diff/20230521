# Comparing `tmp/runcitadel-1.0.0a0.tar.gz` & `tmp/runcitadel-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runcitadel-1.0.0a0.tar", max compression
+gzip compressed data, was "runcitadel-2.0.0.tar", max compression
```

## Comparing `runcitadel-1.0.0a0.tar` & `runcitadel-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1077 2023-03-15 09:37:56.646433 runcitadel-1.0.0a0/LICENSE
--rw-r--r--   0        0        0      920 2023-03-15 11:53:00.789948 runcitadel-1.0.0a0/README.md
--rw-r--r--   0        0        0      482 2023-05-20 11:27:46.410583 runcitadel-1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0      139 2023-03-15 09:37:56.646433 runcitadel-1.0.0a0/src/runcitadel/__init__.py
--rw-r--r--   0        0        0    12218 2023-05-20 11:18:40.040663 runcitadel-1.0.0a0/src/runcitadel/runcitadel.py
--rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 runcitadel-1.0.0a0/setup.py
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 runcitadel-1.0.0a0/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-03-15 09:37:56.646433 runcitadel-2.0.0/LICENSE
+-rw-r--r--   0        0        0      920 2023-03-15 11:53:00.789948 runcitadel-2.0.0/README.md
+-rw-r--r--   0        0        0      480 2023-05-21 16:14:15.045533 runcitadel-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-03-15 09:37:56.646433 runcitadel-2.0.0/src/runcitadel/__init__.py
+-rw-r--r--   0        0        0    12223 2023-05-21 16:12:50.087751 runcitadel-2.0.0/src/runcitadel/runcitadel.py
+-rw-r--r--   0        0        0     1681 1970-01-01 00:00:00.000000 runcitadel-2.0.0/setup.py
+-rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 runcitadel-2.0.0/PKG-INFO
```

### Comparing `runcitadel-1.0.0a0/LICENSE` & `runcitadel-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runcitadel-1.0.0a0/README.md` & `runcitadel-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `runcitadel-1.0.0a0/src/runcitadel/runcitadel.py` & `runcitadel-2.0.0/src/runcitadel/runcitadel.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 
 
 def validate_params_schema(data):
     FIELD_MINLENGTH = 1
     FIELD_MAXLENGTH = 30
     VALUE_MAXLENGTH = 100
 
+    return True
+
     if (len(data) > 10):
         raise ValueError("Start params length must be max 10")
 
     schema = {
         "type": "array",
         "description": "Start parameters schema",
         "items": {
@@ -328,15 +330,15 @@
             'senderID': key,
             'type': 'registerSimulator',
             'messageSource': 'simulator',
             'receiverType': 'server',
             'receiverID': 'server',
             'payload': {
                 'apikey': key,
-                'params': json.dumps(startParams),
+                'params': startParams,
                 'validator': has_schema,
                 'title': title,
             }
         }))
 
         while (1):
             response = await websocket.recv()
```

### Comparing `runcitadel-1.0.0a0/setup.py` & `runcitadel-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['jsonschema>=4.17.3,<5.0.0', 'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'runcitadel',
-    'version': '1.0.0a0',
+    'version': '2.0.0',
     'description': 'A package for developing and running citadel simulations.',
     'long_description': '# runcitadel\n\nA package for developing and running citadel simulations.\n\n## Installation\n\n```bash\n$ pip install runcitadel\n```\n\n## Usage\n\n`runcitadel` can be used to connect a local simulation to a citadel session to perform\ninteractive computation on graphs. For usage examples, see the examples notebook in /docs/.\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`runcitadel` was created by Miles van der Lely. It is licensed under the terms of the MIT license.\n\n## Credits\n\n`runcitadel` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n\nDeveloped in the Visualisation Lab at the University of Amsterdam (UvA).\n',
     'author': 'Miles van der Lely',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `runcitadel-1.0.0a0/PKG-INFO` & `runcitadel-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runcitadel
-Version: 1.0.0a0
+Version: 2.0.0
 Summary: A package for developing and running citadel simulations.
 License: MIT
 Author: Miles van der Lely
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

