# Comparing `tmp/sqlite3-to-mysql-1.4.8.tar.gz` & `tmp/sqlite3-to-mysql-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite3-to-mysql-1.4.8.tar", last modified: Sun Oct 10 13:49:33 2021, max compression
+gzip compressed data, was "sqlite3-to-mysql-1.4.9.tar", last modified: Sun Dec 19 22:12:53 2021, max compression
```

## Comparing `sqlite3-to-mysql-1.4.8.tar` & `sqlite3-to-mysql-1.4.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 13:49:33.865462 sqlite3-to-mysql-1.4.8/
--rw-r--r--   0 klemen     (501) staff       (20)     5513 2021-09-19 12:10:28.000000 sqlite3-to-mysql-1.4.8/CODE-OF-CONDUCT.md
--rw-r--r--   0 klemen     (501) staff       (20)     1069 2021-02-13 11:00:12.000000 sqlite3-to-mysql-1.4.8/LICENSE
--rw-r--r--   0 klemen     (501) staff       (20)      166 2020-07-19 22:13:21.000000 sqlite3-to-mysql-1.4.8/MANIFEST.in
--rw-r--r--   0 klemen     (501) staff       (20)     5850 2021-10-10 13:49:33.865702 sqlite3-to-mysql-1.4.8/PKG-INFO
--rw-r--r--   0 klemen     (501) staff       (20)     4449 2021-09-19 12:11:52.000000 sqlite3-to-mysql-1.4.8/README.md
--rw-r--r--   0 klemen     (501) staff       (20)      288 2019-08-31 11:17:29.000000 sqlite3-to-mysql-1.4.8/pytest.ini
--rw-r--r--   0 klemen     (501) staff       (20)      729 2021-10-10 13:00:57.000000 sqlite3-to-mysql-1.4.8/requirements_dev.txt
--rw-r--r--   0 klemen     (501) staff       (20)      191 2021-10-10 13:49:33.867086 sqlite3-to-mysql-1.4.8/setup.cfg
--rw-r--r--   0 klemen     (501) staff       (20)     2492 2021-10-10 12:17:53.000000 sqlite3-to-mysql-1.4.8/setup.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 13:49:33.823866 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/
--rw-r--r--   0 klemen     (501) staff       (20)       96 2019-08-30 23:56:58.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)      363 2021-10-10 13:49:29.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/__version__.py
--rw-r--r--   0 klemen     (501) staff       (20)     5267 2021-09-15 21:38:13.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/cli.py
--rw-r--r--   0 klemen     (501) staff       (20)     2369 2021-04-18 12:23:41.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/click_utils.py
--rw-r--r--   0 klemen     (501) staff       (20)     3387 2020-08-31 11:57:01.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/debug_info.py
--rw-r--r--   0 klemen     (501) staff       (20)     2969 2021-09-18 22:11:02.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/mysql_utils.py
--rw-r--r--   0 klemen     (501) staff       (20)      378 2020-08-31 11:51:56.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/sixeptions.py
--rw-r--r--   0 klemen     (501) staff       (20)     1337 2021-09-15 13:46:49.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/sqlite_utils.py
--rw-r--r--   0 klemen     (501) staff       (20)    26111 2021-09-18 22:11:02.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/transporter.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 13:49:33.836732 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql.egg-info/
--rw-r--r--   0 klemen     (501) staff       (20)     5850 2021-10-10 13:49:33.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql.egg-info/PKG-INFO
--rw-r--r--   0 klemen     (501) staff       (20)      906 2021-10-10 13:49:33.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 klemen     (501) staff       (20)        1 2021-10-10 13:49:33.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 klemen     (501) staff       (20)       77 2021-10-10 13:49:33.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql.egg-info/entry_points.txt
--rw-r--r--   0 klemen     (501) staff       (20)        1 2019-08-29 21:34:48.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql.egg-info/not-zip-safe
--rw-r--r--   0 klemen     (501) staff       (20)      346 2021-10-10 13:49:33.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql.egg-info/requires.txt
--rw-r--r--   0 klemen     (501) staff       (20)       17 2021-10-10 13:49:33.000000 sqlite3-to-mysql-1.4.8/sqlite3_to_mysql.egg-info/top_level.txt
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 13:49:33.849736 sqlite3-to-mysql-1.4.8/tests/
--rw-r--r--   0 klemen     (501) staff       (20)        0 2019-08-25 00:15:14.000000 sqlite3-to-mysql-1.4.8/tests/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)    12906 2020-08-31 11:26:29.000000 sqlite3-to-mysql-1.4.8/tests/conftest.py
--rw-r--r--   0 klemen     (501) staff       (20)     1260 2019-09-02 14:03:22.000000 sqlite3-to-mysql-1.4.8/tests/database.py
--rw-r--r--   0 klemen     (501) staff       (20)     4023 2021-10-10 13:39:09.000000 sqlite3-to-mysql-1.4.8/tests/factories.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 13:49:33.860804 sqlite3-to-mysql-1.4.8/tests/func/
--rw-r--r--   0 klemen     (501) staff       (20)        0 2019-08-25 00:15:14.000000 sqlite3-to-mysql-1.4.8/tests/func/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)    19781 2021-10-10 13:16:37.000000 sqlite3-to-mysql-1.4.8/tests/func/sqlite3_to_mysql_test.py
--rw-r--r--   0 klemen     (501) staff       (20)    12717 2021-04-18 12:43:07.000000 sqlite3-to-mysql-1.4.8/tests/func/test_cli.py
--rw-r--r--   0 klemen     (501) staff       (20)     5974 2021-04-17 20:58:11.000000 sqlite3-to-mysql-1.4.8/tests/models.py
--rw-r--r--   0 klemen     (501) staff       (20)      246 2019-08-27 07:59:34.000000 sqlite3-to-mysql-1.4.8/tests/sixeptions.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 13:49:33.864119 sqlite3-to-mysql-1.4.8/tests/unit/
--rw-r--r--   0 klemen     (501) staff       (20)        0 2019-08-25 00:15:14.000000 sqlite3-to-mysql-1.4.8/tests/unit/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)    13223 2021-09-18 20:05:05.000000 sqlite3-to-mysql-1.4.8/tests/unit/sqlite3_to_mysql_test.py
+drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-12-19 22:12:53.733608 sqlite3-to-mysql-1.4.9/
+-rw-r--r--   0 klemen     (501) staff       (20)     5513 2021-09-19 12:10:28.000000 sqlite3-to-mysql-1.4.9/CODE-OF-CONDUCT.md
+-rw-r--r--   0 klemen     (501) staff       (20)     1069 2021-02-13 11:00:12.000000 sqlite3-to-mysql-1.4.9/LICENSE
+-rw-r--r--   0 klemen     (501) staff       (20)      166 2020-07-19 22:13:21.000000 sqlite3-to-mysql-1.4.9/MANIFEST.in
+-rw-r--r--   0 klemen     (501) staff       (20)     5850 2021-12-19 22:12:53.734417 sqlite3-to-mysql-1.4.9/PKG-INFO
+-rw-r--r--   0 klemen     (501) staff       (20)     4449 2021-09-19 12:11:52.000000 sqlite3-to-mysql-1.4.9/README.md
+-rw-r--r--   0 klemen     (501) staff       (20)      288 2019-08-31 11:17:29.000000 sqlite3-to-mysql-1.4.9/pytest.ini
+-rw-r--r--   0 klemen     (501) staff       (20)      729 2021-10-10 13:00:57.000000 sqlite3-to-mysql-1.4.9/requirements_dev.txt
+-rw-r--r--   0 klemen     (501) staff       (20)      191 2021-12-19 22:12:53.736088 sqlite3-to-mysql-1.4.9/setup.cfg
+-rw-r--r--   0 klemen     (501) staff       (20)     2492 2021-10-10 12:17:53.000000 sqlite3-to-mysql-1.4.9/setup.py
+drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-12-19 22:12:53.682585 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/
+-rw-r--r--   0 klemen     (501) staff       (20)       96 2019-08-30 23:56:58.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/__init__.py
+-rw-r--r--   0 klemen     (501) staff       (20)      363 2021-12-19 22:11:54.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/__version__.py
+-rw-r--r--   0 klemen     (501) staff       (20)     5267 2021-09-15 21:38:13.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/cli.py
+-rw-r--r--   0 klemen     (501) staff       (20)     2369 2021-04-18 12:23:41.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/click_utils.py
+-rw-r--r--   0 klemen     (501) staff       (20)     3387 2020-08-31 11:57:01.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/debug_info.py
+-rw-r--r--   0 klemen     (501) staff       (20)     2969 2021-09-18 22:11:02.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/mysql_utils.py
+-rw-r--r--   0 klemen     (501) staff       (20)      378 2020-08-31 11:51:56.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/sixeptions.py
+-rw-r--r--   0 klemen     (501) staff       (20)     1337 2021-09-15 13:46:49.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/sqlite_utils.py
+-rw-r--r--   0 klemen     (501) staff       (20)    26206 2021-12-19 22:06:09.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/transporter.py
+drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-12-19 22:12:53.691244 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/
+-rw-r--r--   0 klemen     (501) staff       (20)     5850 2021-12-19 22:12:53.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 klemen     (501) staff       (20)      906 2021-12-19 22:12:53.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 klemen     (501) staff       (20)        1 2021-12-19 22:12:53.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 klemen     (501) staff       (20)       77 2021-12-19 22:12:53.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/entry_points.txt
+-rw-r--r--   0 klemen     (501) staff       (20)        1 2019-08-29 21:34:48.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 klemen     (501) staff       (20)      346 2021-12-19 22:12:53.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/requires.txt
+-rw-r--r--   0 klemen     (501) staff       (20)       17 2021-12-19 22:12:53.000000 sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/top_level.txt
+drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-12-19 22:12:53.710607 sqlite3-to-mysql-1.4.9/tests/
+-rw-r--r--   0 klemen     (501) staff       (20)        0 2019-08-25 00:15:14.000000 sqlite3-to-mysql-1.4.9/tests/__init__.py
+-rw-r--r--   0 klemen     (501) staff       (20)    12906 2021-12-19 22:12:07.000000 sqlite3-to-mysql-1.4.9/tests/conftest.py
+-rw-r--r--   0 klemen     (501) staff       (20)     1260 2019-09-02 14:03:22.000000 sqlite3-to-mysql-1.4.9/tests/database.py
+-rw-r--r--   0 klemen     (501) staff       (20)     4023 2021-10-10 13:39:09.000000 sqlite3-to-mysql-1.4.9/tests/factories.py
+drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-12-19 22:12:53.723615 sqlite3-to-mysql-1.4.9/tests/func/
+-rw-r--r--   0 klemen     (501) staff       (20)        0 2019-08-25 00:15:14.000000 sqlite3-to-mysql-1.4.9/tests/func/__init__.py
+-rw-r--r--   0 klemen     (501) staff       (20)    19781 2021-10-10 13:16:37.000000 sqlite3-to-mysql-1.4.9/tests/func/sqlite3_to_mysql_test.py
+-rw-r--r--   0 klemen     (501) staff       (20)    12717 2021-04-18 12:43:07.000000 sqlite3-to-mysql-1.4.9/tests/func/test_cli.py
+-rw-r--r--   0 klemen     (501) staff       (20)     5974 2021-04-17 20:58:11.000000 sqlite3-to-mysql-1.4.9/tests/models.py
+-rw-r--r--   0 klemen     (501) staff       (20)      246 2019-08-27 07:59:34.000000 sqlite3-to-mysql-1.4.9/tests/sixeptions.py
+drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-12-19 22:12:53.730085 sqlite3-to-mysql-1.4.9/tests/unit/
+-rw-r--r--   0 klemen     (501) staff       (20)        0 2019-08-25 00:15:14.000000 sqlite3-to-mysql-1.4.9/tests/unit/__init__.py
+-rw-r--r--   0 klemen     (501) staff       (20)    13223 2021-09-18 20:05:05.000000 sqlite3-to-mysql-1.4.9/tests/unit/sqlite3_to_mysql_test.py
```

### Comparing `sqlite3-to-mysql-1.4.8/CODE-OF-CONDUCT.md` & `sqlite3-to-mysql-1.4.9/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/LICENSE` & `sqlite3-to-mysql-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/PKG-INFO` & `sqlite3-to-mysql-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite3-to-mysql
-Version: 1.4.8
+Version: 1.4.9
 Summary: A simple Python tool to transfer data from SQLite 3 to MySQL
 Home-page: https://github.com/techouse/sqlite3-to-mysql
 Author: Klemen Tusar
 Author-email: techouse@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/techouse/sqlite3-to-mysql
 Platform: UNKNOWN
```

### Comparing `sqlite3-to-mysql-1.4.8/README.md` & `sqlite3-to-mysql-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/requirements_dev.txt` & `sqlite3-to-mysql-1.4.9/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/setup.py` & `sqlite3-to-mysql-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/cli.py` & `sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/cli.py`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/click_utils.py` & `sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/click_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/debug_info.py` & `sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/debug_info.py`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/mysql_utils.py` & `sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/mysql_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/sqlite_utils.py` & `sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/sqlite3_to_mysql/transporter.py` & `sqlite3-to-mysql-1.4.9/sqlite3_to_mysql/transporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,25 +297,26 @@
 
         rows = self._sqlite_cur.fetchall()
         compound_primary_key = (
             len(tuple(True for row in rows if dict(row)["pk"] > 0)) > 1
         )
         for row in rows:
             column = dict(row)
-            sql += " `{name}` {type} {notnull} {auto_increment}, ".format(
+            sql += " `{name}` {type} {notnull} {dflt} {auto_increment}, ".format(
                 name=safe_identifier_length(column["name"]),
                 type=self._translate_type_from_sqlite_to_mysql(column["type"]),
                 notnull="NOT NULL" if column["notnull"] or column["pk"] else "NULL",
                 auto_increment="AUTO_INCREMENT"
                 if column["pk"] > 0
                 and self._translate_type_from_sqlite_to_mysql(
                     column["type"]
                 ).startswith(("INT", "BIGINT"))
                 and not compound_primary_key
                 else "",
+                dflt="DEFAULT " + column["dflt_value"] if column["dflt_value"] else "",
             )
             if column["pk"] > 0:
                 primary_key = {
                     "column": safe_identifier_length(column["name"]),
                     "length": "",
                 }
                 # In case we have a non-numeric primary key
```

### Comparing `sqlite3-to-mysql-1.4.8/sqlite3_to_mysql.egg-info/PKG-INFO` & `sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite3-to-mysql
-Version: 1.4.8
+Version: 1.4.9
 Summary: A simple Python tool to transfer data from SQLite 3 to MySQL
 Home-page: https://github.com/techouse/sqlite3-to-mysql
 Author: Klemen Tusar
 Author-email: techouse@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/techouse/sqlite3-to-mysql
 Platform: UNKNOWN
```

### Comparing `sqlite3-to-mysql-1.4.8/sqlite3_to_mysql.egg-info/SOURCES.txt` & `sqlite3-to-mysql-1.4.9/sqlite3_to_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/tests/conftest.py` & `sqlite3-to-mysql-1.4.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/tests/database.py` & `sqlite3-to-mysql-1.4.9/tests/database.py`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/tests/factories.py` & `sqlite3-to-mysql-1.4.9/tests/factories.py`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/tests/func/sqlite3_to_mysql_test.py` & `sqlite3-to-mysql-1.4.9/tests/func/sqlite3_to_mysql_test.py`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/tests/func/test_cli.py` & `sqlite3-to-mysql-1.4.9/tests/func/test_cli.py`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/tests/models.py` & `sqlite3-to-mysql-1.4.9/tests/models.py`

 * *Files identical despite different names*

### Comparing `sqlite3-to-mysql-1.4.8/tests/unit/sqlite3_to_mysql_test.py` & `sqlite3-to-mysql-1.4.9/tests/unit/sqlite3_to_mysql_test.py`

 * *Files identical despite different names*

