# Comparing `tmp/xiaomi-ble-0.9.2.tar.gz` & `tmp/xiaomi-ble-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaomi-ble-0.9.2.tar", max compression
+gzip compressed data, was "xiaomi-ble-0.9.3.tar", max compression
```

## Comparing `xiaomi-ble-0.9.2.tar` & `xiaomi-ble-0.9.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11345 2022-08-25 14:25:26.444233 xiaomi-ble-0.9.2/LICENSE
--rw-r--r--   0        0        0     3500 2022-08-25 14:25:26.444233 xiaomi-ble-0.9.2/README.md
--rw-r--r--   0        0        0     2575 2022-08-25 14:25:27.228237 xiaomi-ble-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      713 2022-08-25 14:25:27.184237 xiaomi-ble-0.9.2/src/xiaomi_ble/__init__.py
--rw-r--r--   0        0        0      193 2022-08-25 14:25:26.444233 xiaomi-ble-0.9.2/src/xiaomi_ble/const.py
--rw-r--r--   0        0        0     4613 2022-08-25 14:25:26.444233 xiaomi-ble-0.9.2/src/xiaomi_ble/devices.py
--rw-r--r--   0        0        0    44237 2022-08-25 14:25:26.444233 xiaomi-ble-0.9.2/src/xiaomi_ble/parser.py
--rw-r--r--   0        0        0        0 2022-08-25 14:25:26.444233 xiaomi-ble-0.9.2/src/xiaomi_ble/py.typed
--rw-r--r--   0        0        0     4615 2022-08-25 14:25:36.168923 xiaomi-ble-0.9.2/setup.py
--rw-r--r--   0        0        0     5028 2022-08-25 14:25:36.169398 xiaomi-ble-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11345 2022-09-12 13:57:42.536019 xiaomi-ble-0.9.3/LICENSE
+-rw-r--r--   0        0        0     3500 2022-09-12 13:57:42.536019 xiaomi-ble-0.9.3/README.md
+-rw-r--r--   0        0        0     2576 2022-09-12 13:57:43.620035 xiaomi-ble-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      713 2022-09-12 13:57:43.572034 xiaomi-ble-0.9.3/src/xiaomi_ble/__init__.py
+-rw-r--r--   0        0        0      193 2022-09-12 13:57:42.536019 xiaomi-ble-0.9.3/src/xiaomi_ble/const.py
+-rw-r--r--   0        0        0     4613 2022-09-12 13:57:42.536019 xiaomi-ble-0.9.3/src/xiaomi_ble/devices.py
+-rw-r--r--   0        0        0    44237 2022-09-12 13:57:42.536019 xiaomi-ble-0.9.3/src/xiaomi_ble/parser.py
+-rw-r--r--   0        0        0        0 2022-09-12 13:57:42.536019 xiaomi-ble-0.9.3/src/xiaomi_ble/py.typed
+-rw-r--r--   0        0        0     4620 1970-01-01 00:00:00.000000 xiaomi-ble-0.9.3/setup.py
+-rw-r--r--   0        0        0     5029 1970-01-01 00:00:00.000000 xiaomi-ble-0.9.3/PKG-INFO
```

### Comparing `xiaomi-ble-0.9.2/LICENSE` & `xiaomi-ble-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaomi-ble-0.9.2/README.md` & `xiaomi-ble-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `xiaomi-ble-0.9.2/pyproject.toml` & `xiaomi-ble-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xiaomi-ble"
-version = "0.9.2"
+version = "0.9.3"
 description = "Manage Xiaomi BLE devices"
 authors = ["John Carr <john.carr@unrouted.co.uk>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/xiaomi-ble"
 documentation = "https://xiaomi-ble.readthedocs.io"
 classifiers = [
@@ -29,15 +29,15 @@
 Sphinx = {version = "^5.0", optional = true}
 sphinx-rtd-theme = {version = "^1.0", optional = true}
 myst-parser = {version = "^0.18", optional = true}
 home-assistant-bluetooth = ">=1.3.0"
 sensor-state-data = ">=2.1.2"
 bluetooth-sensor-state-data = ">=1.5.0"
 pycryptodomex = ">=3.15.0"
-bleak-retry-connector = ">0.11.0"
+bleak-retry-connector = ">=1.14.0"
 bluetooth-data-tools = ">=0.1.2"
 
 [tool.poetry.extras]
 docs = [
     "myst-parser",
     "sphinx",
     "sphinx-rtd-theme",
```

### Comparing `xiaomi-ble-0.9.2/src/xiaomi_ble/__init__.py` & `xiaomi-ble-0.9.3/src/xiaomi_ble/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     SensorUpdate,
     SensorValue,
     Units,
 )
 
 from .parser import XiaomiBluetoothDeviceData
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 __all__ = [
     "XiaomiBluetoothDeviceData",
     "SensorDescription",
     "SensorDeviceInfo",
     "DeviceClass",
     "DeviceKey",
```

### Comparing `xiaomi-ble-0.9.2/src/xiaomi_ble/devices.py` & `xiaomi-ble-0.9.3/src/xiaomi_ble/devices.py`

 * *Files identical despite different names*

### Comparing `xiaomi-ble-0.9.2/src/xiaomi_ble/parser.py` & `xiaomi-ble-0.9.3/src/xiaomi_ble/parser.py`

 * *Files identical despite different names*

### Comparing `xiaomi-ble-0.9.2/setup.py` & `xiaomi-ble-0.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,35 +7,35 @@
 packages = \
 ['xiaomi_ble']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bleak-retry-connector>0.11.0',
+['bleak-retry-connector>=1.14.0',
  'bluetooth-data-tools>=0.1.2',
  'bluetooth-sensor-state-data>=1.5.0',
  'home-assistant-bluetooth>=1.3.0',
  'pycryptodomex>=3.15.0',
  'sensor-state-data>=2.1.2']
 
 extras_require = \
 {'docs': ['Sphinx>=5.0,<6.0',
           'sphinx-rtd-theme>=1.0,<2.0',
           'myst-parser>=0.18,<0.19']}
 
 setup_kwargs = {
     'name': 'xiaomi-ble',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'Manage Xiaomi BLE devices',
     'long_description': '# Xiaomi BLE\n\n<p align="center">\n  <a href="https://github.com/bluetooth-devices/xiaomi-ble/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bluetooth-devices/xiaomi-ble/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://xiaomi-ble.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/xiaomi-ble.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bluetooth-devices/xiaomi-ble">\n    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/xiaomi-ble.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/xiaomi-ble/">\n    <img src="https://img.shields.io/pypi/v/xiaomi-ble.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/xiaomi-ble.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/xiaomi-ble.svg?style=flat-square" alt="License">\n</p>\n\nManage Xiaomi BLE devices\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install xiaomi-ble`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
     'author': 'John Carr',
     'author_email': 'john.carr@unrouted.co.uk',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/bluetooth-devices/xiaomi-ble',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.9,<4.0',
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['xiaomi_ble'] package_data = \ {'': ['*']}
-install_requires = \ ['bleak-retry-connector>0.11.0', 'bluetooth-data-
+install_requires = \ ['bleak-retry-connector>=1.14.0', 'bluetooth-data-
 tools>=0.1.2', 'bluetooth-sensor-state-data>=1.5.0', 'home-assistant-
 bluetooth>=1.3.0', 'pycryptodomex>=3.15.0', 'sensor-state-data>=2.1.2']
 extras_require = \ {'docs': ['Sphinx>=5.0,<6.0', 'sphinx-rtd-theme>=1.0,<2.0',
 'myst-parser>=0.18,<0.19']} setup_kwargs = { 'name': 'xiaomi-ble', 'version':
-'0.9.2', 'description': 'Manage Xiaomi BLE devices', 'long_description': '#
+'0.9.3', 'description': 'Manage Xiaomi BLE devices', 'long_description': '#
 Xiaomi BLE\n\n
      \n \n_[CI_Status]\n\n \n_[Documentation_Status]\n\n \n_[Test_coverage
                                 percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
@@ -18,12 +18,12 @@
 â¨\n\nThanks goes to these wonderful people ([emoji key](https://
 allcontributors.org/docs/en/emoji-key)):\n\n\n\n\n\n\n\n\nThis project follows
 the [all-contributors](https://github.com/all-contributors/all-contributors)
 specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package
 was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and
 the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/
 cookiecutter-pypackage)\nproject template.\n', 'author': 'John Carr',
-'author_email': 'john.carr@unrouted.co.uk', 'maintainer': None,
-'maintainer_email': None, 'url': 'https://github.com/bluetooth-devices/xiaomi-
-ble', 'package_dir': package_dir, 'packages': packages, 'package_data':
+'author_email': 'john.carr@unrouted.co.uk', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'https://github.com/bluetooth-devices/
+xiaomi-ble', 'package_dir': package_dir, 'packages': packages, 'package_data':
 package_data, 'install_requires': install_requires, 'extras_require':
 extras_require, 'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
```

### Comparing `xiaomi-ble-0.9.2/PKG-INFO` & `xiaomi-ble-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: xiaomi-ble
-Version: 0.9.2
+Version: 0.9.3
 Summary: Manage Xiaomi BLE devices
 Home-page: https://github.com/bluetooth-devices/xiaomi-ble
 License: Apache Software License 2.0
 Author: John Carr
 Author-email: john.carr@unrouted.co.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=5.0,<6.0); extra == "docs"
-Requires-Dist: bleak-retry-connector (>0.11.0)
+Requires-Dist: bleak-retry-connector (>=1.14.0)
 Requires-Dist: bluetooth-data-tools (>=0.1.2)
 Requires-Dist: bluetooth-sensor-state-data (>=1.5.0)
 Requires-Dist: home-assistant-bluetooth (>=1.3.0)
 Requires-Dist: myst-parser (>=0.18,<0.19); extra == "docs"
 Requires-Dist: pycryptodomex (>=3.15.0)
 Requires-Dist: sensor-state-data (>=2.1.2)
 Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0); extra == "docs"
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: xiaomi-ble Version: 0.9.2 Summary: Manage Xiaomi
+Metadata-Version: 2.1 Name: xiaomi-ble Version: 0.9.3 Summary: Manage Xiaomi
 BLE devices Home-page: https://github.com/bluetooth-devices/xiaomi-ble License:
 Apache Software License 2.0 Author: John Carr Author-email:
 john.carr@unrouted.co.uk Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: Other/Proprietary License Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Topic :: Software Development
-:: Libraries Provides-Extra: docs Requires-Dist: Sphinx (>=5.0,<6.0); extra ==
-"docs" Requires-Dist: bleak-retry-connector (>0.11.0) Requires-Dist: bluetooth-
-data-tools (>=0.1.2) Requires-Dist: bluetooth-sensor-state-data (>=1.5.0)
-Requires-Dist: home-assistant-bluetooth (>=1.3.0) Requires-Dist: myst-parser
-(>=0.18,<0.19); extra == "docs" Requires-Dist: pycryptodomex (>=3.15.0)
-Requires-Dist: sensor-state-data (>=2.1.2) Requires-Dist: sphinx-rtd-theme
-(>=1.0,<2.0); extra == "docs" Project-URL: Bug Tracker, https://github.com/
-bluetooth-devices/xiaomi-ble/issues Project-URL: Changelog, https://github.com/
-bluetooth-devices/xiaomi-ble/blob/main/CHANGELOG.md Project-URL: Documentation,
-https://xiaomi-ble.readthedocs.io Project-URL: Repository, https://github.com/
-bluetooth-devices/xiaomi-ble Description-Content-Type: text/markdown # Xiaomi
-BLE
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Topic :: Software
+Development :: Libraries Provides-Extra: docs Requires-Dist: Sphinx
+(>=5.0,<6.0); extra == "docs" Requires-Dist: bleak-retry-connector (>=1.14.0)
+Requires-Dist: bluetooth-data-tools (>=0.1.2) Requires-Dist: bluetooth-sensor-
+state-data (>=1.5.0) Requires-Dist: home-assistant-bluetooth (>=1.3.0)
+Requires-Dist: myst-parser (>=0.18,<0.19); extra == "docs" Requires-Dist:
+pycryptodomex (>=3.15.0) Requires-Dist: sensor-state-data (>=2.1.2) Requires-
+Dist: sphinx-rtd-theme (>=1.0,<2.0); extra == "docs" Project-URL: Bug Tracker,
+https://github.com/bluetooth-devices/xiaomi-ble/issues Project-URL: Changelog,
+https://github.com/bluetooth-devices/xiaomi-ble/blob/main/CHANGELOG.md Project-
+URL: Documentation, https://xiaomi-ble.readthedocs.io Project-URL: Repository,
+https://github.com/bluetooth-devices/xiaomi-ble Description-Content-Type: text/
+markdown # Xiaomi BLE
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 Manage Xiaomi BLE devices ## Installation Install this via pip (or your
 favourite package manager): `pip install xiaomi-ble` ## Contributors â¨ Thanks
 goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
 en/emoji-key)):       This project follows the [all-contributors](https://
```

