# Comparing `tmp/succulent-0.1.0.tar.gz` & `tmp/succulent-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "succulent-0.1.0.tar", max compression
+gzip compressed data, was "succulent-0.1.1.tar", max compression
```

## Comparing `succulent-0.1.0.tar` & `succulent-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-05-19 11:57:25.374491 succulent-0.1.0/LICENSE
--rw-r--r--   0        0        0     1155 2023-05-19 11:57:25.374491 succulent-0.1.0/README.md
--rw-r--r--   0        0        0      669 2023-05-19 11:59:25.308631 succulent-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      107 2023-05-19 11:57:25.374491 succulent-0.1.0/succulent/__init__.py
--rw-r--r--   0        0        0     1323 2023-05-19 11:57:25.374491 succulent-0.1.0/succulent/api.py
--rw-r--r--   0        0        0      343 2023-05-19 11:57:25.374491 succulent-0.1.0/succulent/configuration.py
--rw-r--r--   0        0        0     1812 2023-05-19 11:57:25.374491 succulent-0.1.0/succulent/processing.py
--rw-r--r--   0        0        0     1858 2023-05-19 11:59:30.753174 succulent-0.1.0/setup.py
--rw-r--r--   0        0        0     1889 2023-05-19 11:59:30.753385 succulent-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-21 15:50:22.668905 succulent-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2399 2023-05-21 15:50:22.668905 succulent-0.1.1/README.md
+-rw-r--r--   0        0        0      669 2023-05-21 15:50:22.668905 succulent-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-05-21 15:50:22.668905 succulent-0.1.1/succulent/__init__.py
+-rw-r--r--   0        0        0     1367 2023-05-21 15:50:22.668905 succulent-0.1.1/succulent/api.py
+-rw-r--r--   0        0        0      335 2023-05-21 15:50:22.668905 succulent-0.1.1/succulent/configuration.py
+-rw-r--r--   0        0        0      102 2023-05-21 15:50:22.668905 succulent-0.1.1/succulent/configuration.yml
+-rw-r--r--   0        0        0     1998 2023-05-21 15:50:22.668905 succulent-0.1.1/succulent/processing.py
+-rw-r--r--   0        0        0     3108 2023-05-21 15:50:29.580088 succulent-0.1.1/setup.py
+-rw-r--r--   0        0        0     3118 2023-05-21 15:50:29.580277 succulent-0.1.1/PKG-INFO
```

### Comparing `succulent-0.1.0/LICENSE` & `succulent-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `succulent-0.1.0/pyproject.toml` & `succulent-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "succulent"
-version = "0.1.0"
+version = "0.1.1"
 description = "Collect POST requests easily"
 license = "MIT"
 authors = ["Iztok Fister Jr. <iztok@iztok-jr-fister.eu>", "Tadej Lahovnik <lahovnik.tadej@gmail.com>"]
 keywords = ['data collection', 'data science', 'sensor measurements']
 homepage = "https://github.com/firefly-cpp/succulent"
 repository = "https://github.com/firefly-cpp/succulent"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+pandas = "^2.0.1"
 pyyaml = "^6.0"
-pandas = "^2.0.0"
-flask = "^2.2.3"
+flask = "^2.3.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
 sphinx = "^7.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `succulent-0.1.0/succulent/api.py` & `succulent-0.1.1/succulent/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from flask import Flask, jsonify, request
 from succulent.configuration import Configuration
 from succulent.processing import Processing
 
 class SucculentAPI:
-    def __init__(self, host, port, config):
+    def __init__(self, host, port, config, format='csv'):
         self.host = host
         self.port = port
+        self.format = format
 
         # Configuration file
         conf = Configuration(config)
         self.config = conf.load_config()
 
         # Initialise processing
-        self.processing = Processing(self.config)
+        self.processing = Processing(self.config, self.format)
 
         # Initialise Flask
         self.app = Flask(__name__)
         self.app.add_url_rule('/measure', 'url', self.url, methods=['GET'])
         self.app.add_url_rule('/measure', 'measure', self.measure, methods=['POST'])
 
     def url(self):
@@ -28,14 +29,14 @@
 
     def measure(self):
         try:
             # Process request
             self.processing.process(request)
         except ValueError:
             # Invalid file type
-            return jsonify({'message': f'Invalid file type: {self.config["filetype"]}. Supported file types: csv, json'}), 400
+            return jsonify({'message': f'Invalid file type: {self.format}. Supported file types: csv, json'}), 400
 
         # Send response
         return jsonify({'message': 'Data stored'}), 200
 
     def start(self):
         self.app.run(host=self.host, port=self.port)
```

### Comparing `succulent-0.1.0/setup.py` & `succulent-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['succulent']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['flask>=2.2.3,<3.0.0', 'pandas>=2.0.0,<3.0.0', 'pyyaml>=6.0,<7.0']
+['flask>=2.3.2,<3.0.0', 'pandas>=2.0.1,<3.0.0', 'pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'succulent',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Collect POST requests easily',
-    'long_description': "---\n\n# succulent - Collect POST requests easily\n\n---\n\n## About\n\nsucculent is a pure Python framework that simplifies the configuration, management, collection, and preprocessing of data collected via POST requests. The inspiration for the framework comes from the practical data collection challenges in smart agriculture. The main idea of the framework was to speed up the process of configuring different collected parameters and providing several useful functions for data transformations.\n\n## Detailed insights\nThe current version includes (but is not limited to) the following functions:\n\n- Request URL generation for data collection\n- Data collection from POST requests\n\n## Installation\n\n### pip\n\nInstall succulent with pip:\n\n```sh\npip install succulent\n```\n\n## Usage\n\n### Example\n\n```python\nfrom succulent.api import SucculentAPI\napi = SucculentAPI(host='0.0.0.0', port=8080, config='configuration.yml')\napi.start()\n```\n\n## Configuration\nIn the root directory, create a file named `configuration.yml` and define the following:\n```yml\nfiletype: # File type (csv or json)\n\ndata:\n  - name: # Measure name\n```",
+    'long_description': '---\n\n# succulent - Collect POST requests easily\n\n---\n![PyPI Version](https://img.shields.io/pypi/v/succulent.svg)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/succulent.svg)\n[![Downloads](https://pepy.tech/badge/succulent)](https://pepy.tech/project/succulent)\n![GitHub repo size](https://img.shields.io/github/repo-size/firefly-cpp/succulent?style=flat-square)\n[![GitHub license](https://img.shields.io/github/license/firefly-cpp/succulent.svg)](https://github.com/firefly-cpp/succulent/blob/master/LICENSE)\n![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/succulent.svg)\n[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Average time to resolve an issue")\n[![Percentage of issues still open](http://isitmaintained.com/badge/open/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Percentage of issues still open")\n\n## About\n\nsucculent is a pure Python framework that simplifies the configuration, management, collection, and preprocessing of data collected via POST requests. The inspiration for the framework comes from the practical data collection challenges in smart agriculture. The main idea of the framework was to speed up the process of configuring different collected parameters and providing several useful functions for data transformations.\n\n## Detailed insights\nThe current version includes (but is not limited to) the following functions:\n\n- Request URL generation for data collection\n- Data collection from POST requests\n\n## Installation\n\n### pip\n\nInstall succulent with pip:\n\n```sh\npip install succulent\n```\n\n## Usage\n\n### Example\n\n```python\nfrom succulent.api import SucculentAPI\napi = SucculentAPI(host=\'0.0.0.0\', port=8080, config=\'configuration.yml\', format=\'csv\')\napi.start()\n```\n\n## Configuration\nIn the root directory, create a file named `configuration.yml` and define the following:\n```yml\ndata:\n  - name: # Measure name\n```\n\n## License\n\nThis package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.\n\n## Disclaimer\n\nThis framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!\n',
     'author': 'Iztok Fister Jr.',
     'author_email': 'iztok@iztok-jr-fister.eu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/firefly-cpp/succulent',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `succulent-0.1.0/PKG-INFO` & `succulent-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 Metadata-Version: 2.1
 Name: succulent
-Version: 0.1.0
+Version: 0.1.1
 Summary: Collect POST requests easily
 Home-page: https://github.com/firefly-cpp/succulent
 License: MIT
 Keywords: data collection,data science,sensor measurements
 Author: Iztok Fister Jr.
 Author-email: iztok@iztok-jr-fister.eu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: flask (>=2.2.3,<3.0.0)
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: flask (>=2.3.2,<3.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/firefly-cpp/succulent
 Description-Content-Type: text/markdown
 
 ---
 
 # succulent - Collect POST requests easily
 
 ---
+![PyPI Version](https://img.shields.io/pypi/v/succulent.svg)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/succulent.svg)
+[![Downloads](https://pepy.tech/badge/succulent)](https://pepy.tech/project/succulent)
+![GitHub repo size](https://img.shields.io/github/repo-size/firefly-cpp/succulent?style=flat-square)
+[![GitHub license](https://img.shields.io/github/license/firefly-cpp/succulent.svg)](https://github.com/firefly-cpp/succulent/blob/master/LICENSE)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/firefly-cpp/succulent.svg)
+[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Average time to resolve an issue")
+[![Percentage of issues still open](http://isitmaintained.com/badge/open/firefly-cpp/succulent.svg)](http://isitmaintained.com/project/firefly-cpp/succulent "Percentage of issues still open")
 
 ## About
 
 succulent is a pure Python framework that simplifies the configuration, management, collection, and preprocessing of data collected via POST requests. The inspiration for the framework comes from the practical data collection challenges in smart agriculture. The main idea of the framework was to speed up the process of configuring different collected parameters and providing several useful functions for data transformations.
 
 ## Detailed insights
 The current version includes (but is not limited to) the following functions:
@@ -47,19 +55,26 @@
 
 ## Usage
 
 ### Example
 
 ```python
 from succulent.api import SucculentAPI
-api = SucculentAPI(host='0.0.0.0', port=8080, config='configuration.yml')
+api = SucculentAPI(host='0.0.0.0', port=8080, config='configuration.yml', format='csv')
 api.start()
 ```
 
 ## Configuration
 In the root directory, create a file named `configuration.yml` and define the following:
 ```yml
-filetype: # File type (csv or json)
-
 data:
   - name: # Measure name
 ```
+
+## License
+
+This package is distributed under the MIT License. This license can be found online at <http://www.opensource.org/licenses/MIT>.
+
+## Disclaimer
+
+This framework is provided as-is, and there are no guarantees that it fits your purposes or that it is bug-free. Use it at your own risk!
+
```

