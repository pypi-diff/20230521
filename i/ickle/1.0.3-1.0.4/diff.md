# Comparing `tmp/ickle-1.0.3.tar.gz` & `tmp/ickle-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ickle-1.0.3.tar", last modified: Sat Mar 25 10:30:07 2023, max compression
+gzip compressed data, was "ickle-1.0.4.tar", last modified: Sun May 21 14:10:11 2023, max compression
```

## Comparing `ickle-1.0.3.tar` & `ickle-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 10:30:07.362382 ickle-1.0.3/
--rw-rw-rw-   0        0        0     1091 2022-11-17 11:52:28.000000 ickle-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2815 2023-03-25 10:30:07.360381 ickle-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2160 2022-11-17 11:52:28.000000 ickle-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-25 10:30:07.320381 ickle-1.0.3/ickle/
--rw-rw-rw-   0        0        0    37587 2023-03-25 10:25:50.000000 ickle-1.0.3/ickle/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 10:30:07.343389 ickle-1.0.3/ickle.egg-info/
--rw-rw-rw-   0        0        0     2815 2023-03-25 10:30:07.000000 ickle-1.0.3/ickle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-03-25 10:30:07.000000 ickle-1.0.3/ickle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 10:30:07.000000 ickle-1.0.3/ickle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-25 10:30:07.000000 ickle-1.0.3/ickle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-25 10:30:07.000000 ickle-1.0.3/ickle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-25 10:30:07.363381 ickle-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-03-25 10:25:50.000000 ickle-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-25 10:30:07.356382 ickle-1.0.3/tests/
--rw-rw-rw-   0        0        0      381 2022-11-17 11:52:28.000000 ickle-1.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0    32630 2023-03-25 10:25:50.000000 ickle-1.0.3/tests/test_dataframe.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:10:11.912359 ickle-1.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-05-21 14:08:30.000000 ickle-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2815 2023-05-21 14:10:11.911356 ickle-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2160 2023-05-21 14:08:30.000000 ickle-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 14:10:11.858450 ickle-1.0.4/ickle/
+-rw-rw-rw-   0        0        0    38421 2023-05-21 14:08:30.000000 ickle-1.0.4/ickle/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:10:11.901837 ickle-1.0.4/ickle.egg-info/
+-rw-rw-rw-   0        0        0     2815 2023-05-21 14:10:11.000000 ickle-1.0.4/ickle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-05-21 14:10:11.000000 ickle-1.0.4/ickle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 14:10:11.000000 ickle-1.0.4/ickle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-21 14:10:11.000000 ickle-1.0.4/ickle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-21 14:10:11.000000 ickle-1.0.4/ickle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 14:10:11.912359 ickle-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-05-21 14:08:30.000000 ickle-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:10:11.907434 ickle-1.0.4/tests/
+-rw-rw-rw-   0        0        0      381 2023-05-21 14:08:30.000000 ickle-1.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0    33147 2023-05-21 14:08:30.000000 ickle-1.0.4/tests/test_dataframe.py
```

### Comparing `ickle-1.0.3/LICENSE` & `ickle-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ickle-1.0.3/PKG-INFO` & `ickle-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ickle
-Version: 1.0.3
+Version: 1.0.4
 Summary: 🔍 Experimental DataFrame, statistics and analysis library for Python
 Home-page: https://github.com/karishmashuklaa/ickle
 Author: Karishma Shukla
 Author-email: karishmashuklaa@gmail.com
 License: MIT
 Keywords: data-analysis,numpy,data,python,library,pandas,ickle,datascience
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ickle Version: 1.0.3 Summary: ð Experimental
+Metadata-Version: 2.1 Name: ickle Version: 1.0.4 Summary: ð Experimental
 DataFrame, statistics and analysis library for Python Home-page: https://
 github.com/karishmashuklaa/ickle Author: Karishma Shukla Author-email:
 karishmashuklaa@gmail.com License: MIT Keywords: data-
 analysis,numpy,data,python,library,pandas,ickle,datascience Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
```

### Comparing `ickle-1.0.3/README.md` & `ickle-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ickle-1.0.3/ickle/__init__.py` & `ickle-1.0.4/ickle/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import csv
+import openpyxl
 import sqlalchemy
 from sqlalchemy.engine import URL
 
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 
 class DataFrame:
 
     def __init__(self, data):
         """
         A DataFrame holds two dimensional heterogenous data.
         Create it by passing a dictionary of NumPy arrays to the values parameter.
@@ -1182,7 +1183,40 @@
         except ValueError:
             try:
                 new_data[col] = np.array(vals, dtype='float')
             except ValueError:
                 new_data[col] = np.array(vals, dtype='O')
     return DataFrame(new_data)
 
+def read_excel(file_path, sheet_name=None):
+    """
+    Read a simple Excel file as a DataFrame
+
+    Parameters
+    ----------
+    file_path: str of the path to the Excel file that you want to read
+    sheet_name: str of sheet name
+
+    Returns
+    -------
+    A DataFrame
+    """
+    workbook = openpyxl.load_workbook(filename=file_path, read_only=True)
+    if sheet_name is not None:
+        worksheet = workbook[sheet_name]
+    else:
+        worksheet = workbook.active
+    
+    data = []
+    for row in worksheet.iter_rows(values_only=True):
+        data.append(row)
+    
+    data = np.array(data)
+    
+    headers = data[0]
+    records = data[1:]
+
+    columns = {}
+    for i, header in enumerate(headers):
+        columns[header] = records[:, i]
+    
+    return DataFrame(columns)
```

### Comparing `ickle-1.0.3/ickle.egg-info/PKG-INFO` & `ickle-1.0.4/ickle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ickle
-Version: 1.0.3
+Version: 1.0.4
 Summary: 🔍 Experimental DataFrame, statistics and analysis library for Python
 Home-page: https://github.com/karishmashuklaa/ickle
 Author: Karishma Shukla
 Author-email: karishmashuklaa@gmail.com
 License: MIT
 Keywords: data-analysis,numpy,data,python,library,pandas,ickle,datascience
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ickle Version: 1.0.3 Summary: ð Experimental
+Metadata-Version: 2.1 Name: ickle Version: 1.0.4 Summary: ð Experimental
 DataFrame, statistics and analysis library for Python Home-page: https://
 github.com/karishmashuklaa/ickle Author: Karishma Shukla Author-email:
 karishmashuklaa@gmail.com License: MIT Keywords: data-
 analysis,numpy,data,python,library,pandas,ickle,datascience Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
```

### Comparing `ickle-1.0.3/setup.py` & `ickle-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 def readme():
     with open('README.md') as f:
         README = f.read()
     return README
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = '🔍 Experimental DataFrame, statistics and analysis library for Python'
 
 setup(
     name="ickle",
     version=VERSION,
     author="Karishma Shukla",
     author_email="karishmashuklaa@gmail.com",
```

### Comparing `ickle-1.0.3/tests/test_dataframe.py` & `ickle-1.0.4/tests/test_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -887,8 +887,23 @@
     def test_sql_dataframe(self, db_session, valid_author):
         db_session.add(valid_author)
         db_session.commit()
         sql = 'SELECT id, firstname, lastname, email FROM authors'
         df = ick.read_sql(sql,url)
         assert df["firstname"] == "John"
         assert df["lastname"] == "Doe"
-        assert df["email"] == "upchh@example.com"
+        assert df["email"] == "upchh@example.com"
+
+class TestReadExcel:
+    def test_read_excel(self):
+        file_path = 'dataset/Book1.xlsx'
+        sheet_name = 'Sheet1'
+        df = ick.read_excel(file_path, sheet_name)
+
+        expected_data = {
+            'Name': np.array(['John', 'Sam', 'Max'], dtype='O'),
+            'Age': np.array(['54', '23', '44'], dtype='O'),
+            'Country': np.array(['USA', 'UK', 'Pakistan'], dtype='O'),
+        }
+        expected_df = ick.DataFrame(expected_data)
+
+        assert_df_equals(df, expected_df)
```

