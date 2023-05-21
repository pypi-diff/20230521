# Comparing `tmp/mosek_license_server-0.1.1.tar.gz` & `tmp/mosek_license_server-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosek_license_server-0.1.1.tar", max compression
+gzip compressed data, was "mosek_license_server-0.1.2.tar", max compression
```

## Comparing `mosek_license_server-0.1.1.tar` & `mosek_license_server-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-21 04:33:23.366391 mosek_license_server-0.1.1/mosek_license/__init__.py
--rw-r--r--   0        0        0      499 2023-05-21 04:33:23.366391 mosek_license_server-0.1.1/mosek_license/license.py
--rw-r--r--   0        0        0      470 2023-05-21 04:33:39.190631 mosek_license_server-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1982 2023-05-21 04:33:23.366391 mosek_license_server-0.1.1/readme.md
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 mosek_license_server-0.1.1/setup.py
--rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 mosek_license_server-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-21 05:39:44.781663 mosek_license_server-0.1.2/mosek_license/__init__.py
+-rw-r--r--   0        0        0      499 2023-05-21 05:39:44.785663 mosek_license_server-0.1.2/mosek_license/license.py
+-rw-r--r--   0        0        0      533 2023-05-21 05:40:02.209895 mosek_license_server-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1982 2023-05-21 05:39:44.785663 mosek_license_server-0.1.2/readme.md
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 mosek_license_server-0.1.2/setup.py
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 mosek_license_server-0.1.2/PKG-INFO
```

### Comparing `mosek_license_server-0.1.1/readme.md` & `mosek_license_server-0.1.2/readme.md`

 * *Files identical despite different names*

### Comparing `mosek_license_server-0.1.1/setup.py` & `mosek_license_server-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['urllib3']
 
 setup_kwargs = {
     'name': 'mosek-license-server',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Expose a mosek license via a nginx server',
     'long_description': "# Mosek License Server\n\n[![PyPI version](https://badge.fury.io/py/mosek-license-server.svg)](https://badge.fury.io/py/mosek-license-server)\n[![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/tschm/mosek-license-server/blob/main/LICENSE)\n[![PyPI download month](https://img.shields.io/pypi/dm/mosek-license-server.svg)](https://pypi.python.org/pypi/mosek-license-server/)\n\nUsing a [nginx image](https://hub.docker.com/_/nginx/) we expose a Mosek license\non a server to be accessible from various research machines without sharing the actual\nlicense file in the underlying repositories.\n\nThis repository serves two purposes. It exposes the server but it is also the home\nfor a little Python package to inject the license into your programs.\n\nWe solve a common problem here. Assume $20$ researchers work on $50$ different strategies.\nUsing local copies of the same license file is a tedious exercise as the file needs to get \nupdated once a year. \nRather, each strategy would connect to the server to fetch a license using the mosek_license\nPython package. Once the strategy expires we only need to update the server.\nNo change for the strategies is required.\n\n## License server\n\n### Copy your license file into folder \n\nCopy the license file you have received (from Mosek) into the license folder.\nName it `mosek'.\n\n\n### Start the nginx server\n\nShare the license folder (after you have copied your personal Mosek license into)\nvia\n\n```bash\ndocker run --name mosek -v $PWD/license:/usr/share/nginx/html:ro -p 8080:80 -d nginx\n```\n\nThe license will now be exposed via http://localhost:8080\n\nAs an alternative you can run the script\n\n```bash\n./license_server.sh\n```\n\n## The mosek_license module\n\nInstall via\n\n```bash\npip install mosek-license-server\n```\nand then\n\n```python\nfrom mosek_license import license\n\n# It's important to upsert the license before you import mosek\nlicense.upsert()\n\n# only now import mosek\nimport mosek\n```\n\n",
     'author': 'Thomas Schmelzer',
     'author_email': 'thomas.schmelzer@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tschm/mosek-license-server',
```

### Comparing `mosek_license_server-0.1.1/PKG-INFO` & `mosek_license_server-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosek-license-server
-Version: 0.1.1
+Version: 0.1.2
 Summary: Expose a mosek license via a nginx server
 Home-page: https://github.com/tschm/mosek-license-server
 License: Apache 2.0
 Author: Thomas Schmelzer
 Author-email: thomas.schmelzer@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: Other/Proprietary License
```

