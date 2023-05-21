# Comparing `tmp/spalah-1.0.0.tar.gz` & `tmp/spalah-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spalah-1.0.0.tar", max compression
+gzip compressed data, was "spalah-1.0.1.tar", max compression
```

## Comparing `spalah-1.0.0.tar` & `spalah-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1217 2022-07-09 12:46:46.000000 spalah-1.0.0/LICENSE
--rw-r--r--   0        0        0     5356 2023-05-20 17:48:37.703026 spalah-1.0.0/README.md
--rw-r--r--   0        0        0     1312 2023-05-20 17:50:57.279488 spalah-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      118 2022-07-09 12:46:46.000000 spalah-1.0.0/spalah/__init__.py
--rw-r--r--   0        0        0      177 2023-05-20 17:33:36.517825 spalah-1.0.0/spalah/dataframe/__init__.py
--rw-r--r--   0        0        0    23329 2023-05-20 17:33:36.518032 spalah-1.0.0/spalah/dataframe/dataframe.py
--rw-r--r--   0        0        0     8813 2023-05-20 17:33:36.518182 spalah-1.0.0/spalah/dataset/DeltaProperty.py
--rw-r--r--   0        0        0      144 2023-05-20 17:33:36.518286 spalah-1.0.0/spalah/dataset/__init__.py
--rw-r--r--   0        0        0      999 2023-05-20 17:33:36.518399 spalah-1.0.0/spalah/dataset/dbfs.py
--rw-r--r--   0        0        0       58 2023-05-20 17:33:36.518507 spalah-1.0.0/spalah/shared/__init__.py
--rw-r--r--   0        0        0      407 2023-05-20 17:33:36.518606 spalah-1.0.0/spalah/shared/logging.py
--rw-r--r--   0        0        0     6663 1970-01-01 00:00:00.000000 spalah-1.0.0/setup.py
--rw-r--r--   0        0        0     6741 1970-01-01 00:00:00.000000 spalah-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1217 2022-07-09 12:46:46.000000 spalah-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5356 2023-05-20 17:48:37.703026 spalah-1.0.1/README.md
+-rw-r--r--   0        0        0     1376 2023-05-21 15:07:41.772148 spalah-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      118 2022-07-09 12:46:46.000000 spalah-1.0.1/spalah/__init__.py
+-rw-r--r--   0        0        0      177 2023-05-20 17:33:36.517825 spalah-1.0.1/spalah/dataframe/__init__.py
+-rw-r--r--   0        0        0    23329 2023-05-20 17:33:36.518032 spalah-1.0.1/spalah/dataframe/dataframe.py
+-rw-r--r--   0        0        0     8813 2023-05-20 17:33:36.518182 spalah-1.0.1/spalah/dataset/DeltaProperty.py
+-rw-r--r--   0        0        0      144 2023-05-20 17:33:36.518286 spalah-1.0.1/spalah/dataset/__init__.py
+-rw-r--r--   0        0        0      999 2023-05-20 17:33:36.518399 spalah-1.0.1/spalah/dataset/dbfs.py
+-rw-r--r--   0        0        0       58 2023-05-20 17:33:36.518507 spalah-1.0.1/spalah/shared/__init__.py
+-rw-r--r--   0        0        0      407 2023-05-20 17:33:36.518606 spalah-1.0.1/spalah/shared/logging.py
+-rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 spalah-1.0.1/setup.py
+-rw-r--r--   0        0        0     6328 1970-01-01 00:00:00.000000 spalah-1.0.1/PKG-INFO
```

### Comparing `spalah-1.0.0/LICENSE` & `spalah-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spalah-1.0.0/README.md` & `spalah-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `spalah-1.0.0/pyproject.toml` & `spalah-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 
 [tool.poetry]
 name = "spalah"
-version = "1.0.0"
+version = "1.0.1"
 description = "Spalah is a set of PySpark dataframe helpers"
 homepage = "https://github.com/avolok/spalah"
 authors = ["Alex Volok <alexandr.volok@gmail.com>"]
 license = "MIT license"
 keywords = ["spalah"]
 classifiers = ["Intended Audience :: Developers", "License :: OSI Approved :: MIT License", "Natural Language :: English", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3.10"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
-black = "==22.3.0"
-bump2version = "==1.0.1"
-coverage = "==6.4.1"
-delta-spark = "==2.1.0"
+pyspark = ">=3.2.0,<4"
+delta-spark = ">=2.1.0,<2.4"
+
+[tool.poetry.dev-dependencies]
+black = ">=22.3.0"
+bump2version = ">=1.0.1,<7"
+coverage = ">=6.4.1"
 flake8 = "==6.0.0"
 packaging = "*"
 pip = "*"
-pre-commit = "==2.19.0"
-pyspark = "==3.3.0"
-pytest = "==7.1.2"
-pytest-cov = "==3.0.0"
+pre-commit = ">=2.19.0,<3"
+pytest = ">=7.1.2,<7.2"
+pytest-cov = ">=3.0.0,<4"
 ruff = "*"
-tox = "==3.25.0"
+tox = ">=3.25.0,<4"
 twine = "==4.0.1"
 watchdog = "==2.1.9"
 wheel = "*"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1.13"
 mkdocstrings = {extras = ["python"], version = "^0.20.0"}
-mkdocs = ">=1.4.3"
+mkdocs = ">=1.4.3,<1.5.0"
 termynal = ">=0.2.1"
 
 [tool.semantic_release]
 version_variable = [    
     "pyproject.toml:version"
 ]
 build_command = "pip install poetry && poetry build"
```

### Comparing `spalah-1.0.0/spalah/dataframe/dataframe.py` & `spalah-1.0.1/spalah/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `spalah-1.0.0/spalah/dataset/DeltaProperty.py` & `spalah-1.0.1/spalah/dataset/DeltaProperty.py`

 * *Files identical despite different names*

### Comparing `spalah-1.0.0/spalah/dataset/dbfs.py` & `spalah-1.0.1/spalah/dataset/dbfs.py`

 * *Files identical despite different names*

### Comparing `spalah-1.0.0/setup.py` & `spalah-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,34 +4,19 @@
 packages = \
 ['spalah', 'spalah.dataframe', 'spalah.dataset', 'spalah.shared']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['black==22.3.0',
- 'bump2version==1.0.1',
- 'coverage==6.4.1',
- 'delta-spark==2.1.0',
- 'flake8==6.0.0',
- 'packaging',
- 'pip',
- 'pre-commit==2.19.0',
- 'pyspark==3.3.0',
- 'pytest-cov==3.0.0',
- 'pytest==7.1.2',
- 'ruff',
- 'tox==3.25.0',
- 'twine==4.0.1',
- 'watchdog==2.1.9',
- 'wheel']
+['delta-spark>=2.1.0,<2.4', 'pyspark>=3.2.0,<4']
 
 setup_kwargs = {
     'name': 'spalah',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'Spalah is a set of PySpark dataframe helpers',
     'long_description': '# spalah\n\nSpalah is a set of python helpers to deal with PySpark dataframes, transformations, schemas and Delta Tables.\n\nThe word "spalah" means "spark" in Ukrainian 🇺🇦 \n\n# Installation\n\nUse the package manager [pip](https://pip.pypa.io/en/stable/) to install spalah.\n\n```bash\npip install spalah\n```\n\n# Examples of use\nSpalah currently has two different groups of helpers: `dataframe` and `datalake`.\n\n## spalah.dataframe\n\n### slice_dataframe\n\n```python\nfrom spalah.dataframe import slice_dataframe\n\ndf = spark.sql(\n    \'SELECT 1 as ID, "John" AS Name, struct("line1" AS Line1, "line2" AS Line2) AS Address\'\n)\ndf.printSchema()\n\n""" output:\nroot\n |-- ID: integer (nullable = false)\n |-- Name: string (nullable = false)\n |-- Address: struct (nullable = false)\n |    |-- Line1: string (nullable = false)\n |    |-- Line2: string (nullable = false)\n"""\n\n# Create a new dataframe by cutting of root and nested attributes\ndf_result = slice_dataframe(\n    input_dataframe=df,\n    columns_to_include=["Name", "Address"],\n    columns_to_exclude=["Address.Line2"]\n)\ndf_result.printSchema()\n\n""" output:\nroot\n |-- Name: string (nullable = false)\n |-- Address: struct (nullable = false)\n |    |-- Line1: string (nullable = false)\n"""\n```\n\nBeside of nested regular structs it also supported slicing of structs in arrays, including multiple levels of nesting\n\n\n### flatten_schema\n\n```python\nfrom spalah.dataframe import flatten_schema\n\n# Pass the sample dataframe to get the list of all attributes as single dimension list\nflatten_schema(df_complex_schema.schema)\n\n""" output:\n[\'ID\', \'Name\', \'Address.Line1\', \'Address.Line2\']\n"""\n\n\n# Alternatively, the function can return data types of the attributes\nflatten_schema(\n    schema=df_complex_schema.schema,\n    include_datatype=True\n)\n\n""" output:\n[\n    (\'ID\', \'IntegerType\'),\n    (\'Name\', \'StringType\'),\n    (\'Address.Line1\', \'StringType\'),\n    (\'Address.Line2\', \'StringType\')\n]\n"""\n```\n\n### script_dataframe\n\n```python\nfrom spalah.dataframe import script_dataframe\n\nscript = script_dataframe(df)\n\nprint(script)\n\n""" output:\nfrom pyspark.sql import Row\nimport datetime\nfrom decimal import Decimal\nfrom pyspark.sql.types import *\n\n# Scripted data and schema:\n__data = [Row(ID=1, Name=\'John\', Address=Row(Line1=\'line1\', Line2=\'line2\'))]\n\n__schema = {\'type\': \'struct\', \'fields\': [{\'name\': \'ID\', \'type\': \'integer\', \'nullable\': False, \'metadata\': {}}, {\'name\': \'Name\', \'type\': \'string\', \'nullable\': False, \'metadata\': {}}, {\'name\': \'Address\', \'type\': {\'type\': \'struct\', \'fields\': [{\'name\': \'Line1\', \'type\': \'string\', \'nullable\': False, \'metadata\': {}}, {\'name\': \'Line2\', \'type\': \'string\', \'nullable\': False, \'metadata\': {}}]}, \'nullable\': False, \'metadata\': {}}]}\n\noutcome_dataframe = spark.createDataFrame(__data, StructType.fromJson(__schema))\n"""\n```\n\n### SchemaComparer\n\n```python\nfrom spalah.dataframe import SchemaComparer\n\nschema_comparer = SchemaComparer(\n    source_schema = df_source.schema,\n    target_schema = df_target.schema\n)\n\nschema_comparer.compare()\n\n# The comparison results are stored in the class instance properties `matched` and `not_matched`\n\n# Contains a list of matched columns:\nschema_comparer.matched\n\n""" output:\n[MatchedColumn(name=\'Address.Line1\',  data_type=\'StringType\')]\n"""\n\n# Contains a list of all not matched columns with a reason as description of non-match:\nschema_comparer.not_matched\n\n""" output:\n[\n    NotMatchedColumn(\n        name=\'name\', \n        data_type=\'StringType\', \n        reason="The column exists in source and target schemas but it\'s name is case-mismatched"\n    ),\n    NotMatchedColumn(\n        name=\'ID\', \n        data_type=\'IntegerType <=> StringType\', \n        reason=\'The column exists in source and target schemas but it is not matched by a data type\'\n    ),\n    NotMatchedColumn(\n        name=\'Address.Line2\', \n        data_type=\'StringType\', \n        reason=\'The column exists only in the source schema\'\n    )\n]\n"""\n```\n\n## spalah.dataset\n\n### Get delta table properties\n\n```python\nfrom spalah.dataset import DeltaProperty\n\ndp = DeltaProperty(table_path="/path/dataset")\n\nprint(dp.properties) \n\n# output: \n# {\'delta.deletedFileRetentionDuration\': \'interval 15 days\'}\n```\n\n### Set delta table properties\n\n```python\nrom spalah.dataset import DeltaProperty\n\ndp = DeltaProperty(table_path="/path/dataset")\n\ndp.properties = {\n    "delta.logRetentionDuration": "interval 10 days",\n    "delta.deletedFileRetentionDuration": "interval 15 days"\n}\n\n```\nand the standard output is:\n\n```\n2023-05-20 18:27:42,070 INFO      Applying check constraints on \'delta.`/tmp/nested_schema_dataset`\':\n2023-05-20 18:27:42,071 INFO      Checking if constraint \'id_is_not_null\' was already set on delta.`/tmp/nested_schema_dataset`\n2023-05-20 18:27:42,433 INFO      The constraint id_is_not_null has been successfully added to \'delta.`/tmp/nested_schema_dataset`\n```\n\nPlease note that check constraints can be retrieved and set using property: `.check_constraints`\n\nCheck for more information in [examples: dataframe](docs/examples/dataframe.md), [examples: datalake](docs/examples/dataset.md) pages and related [notebook](docs/usage.ipynb)\n\n## Contributing\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n## License\n[MIT](https://choosealicense.com/licenses/mit/)\n',
     'author': 'Alex Volok',
     'author_email': 'alexandr.volok@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/avolok/spalah',
```

### Comparing `spalah-1.0.0/PKG-INFO` & `spalah-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spalah
-Version: 1.0.0
+Version: 1.0.1
 Summary: Spalah is a set of PySpark dataframe helpers
 Home-page: https://github.com/avolok/spalah
 License: MIT
 Keywords: spalah
 Author: Alex Volok
 Author-email: alexandr.volok@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -16,30 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: black (==22.3.0)
-Requires-Dist: bump2version (==1.0.1)
-Requires-Dist: coverage (==6.4.1)
-Requires-Dist: delta-spark (==2.1.0)
-Requires-Dist: flake8 (==6.0.0)
-Requires-Dist: packaging
-Requires-Dist: pip
-Requires-Dist: pre-commit (==2.19.0)
-Requires-Dist: pyspark (==3.3.0)
-Requires-Dist: pytest (==7.1.2)
-Requires-Dist: pytest-cov (==3.0.0)
-Requires-Dist: ruff
-Requires-Dist: tox (==3.25.0)
-Requires-Dist: twine (==4.0.1)
-Requires-Dist: watchdog (==2.1.9)
-Requires-Dist: wheel
+Requires-Dist: delta-spark (>=2.1.0,<2.4)
+Requires-Dist: pyspark (>=3.2.0,<4)
 Description-Content-Type: text/markdown
 
 # spalah
 
 Spalah is a set of python helpers to deal with PySpark dataframes, transformations, schemas and Delta Tables.
 
 The word "spalah" means "spark" in Ukrainian 🇺🇦
```

