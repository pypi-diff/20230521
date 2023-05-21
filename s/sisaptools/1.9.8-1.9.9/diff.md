# Comparing `tmp/sisaptools-1.9.8.tar.gz` & `tmp/sisaptools-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sisaptools-1.9.8.tar", last modified: Tue Jun 15 08:51:09 2021, max compression
+gzip compressed data, was "dist/sisaptools-1.9.9.tar", last modified: Tue Jun 15 09:27:20 2021, max compression
```

## Comparing `sisaptools-1.9.8.tar` & `sisaptools-1.9.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sisap     (1000) sisap     (1000)        0 2021-06-15 08:51:09.000000 sisaptools-1.9.8/
-drwxrwxr-x   0 sisap     (1000) sisap     (1000)        0 2021-06-15 08:51:09.000000 sisaptools-1.9.8/sisaptools/
--rw-rw-r--   0 sisap     (1000) sisap     (1000)     2194 2021-05-09 08:56:11.000000 sisaptools-1.9.8/sisaptools/mail.py
--rw-rw-r--   0 sisap     (1000) sisap     (1000)    23889 2021-06-15 08:50:16.000000 sisaptools-1.9.8/sisaptools/database.py
--rw-rw-r--   0 sisap     (1000) sisap     (1000)      451 2021-05-09 08:56:11.000000 sisaptools-1.9.8/sisaptools/services.py
--rw-rw-r--   0 sisap     (1000) sisap     (1000)     2192 2021-05-09 08:56:11.000000 sisaptools-1.9.8/sisaptools/ssh.py
--rw-rw-r--   0 sisap     (1000) sisap     (1000)     1864 2021-05-09 08:56:11.000000 sisaptools-1.9.8/sisaptools/aes.py
--rw-rw-r--   0 sisap     (1000) sisap     (1000)     1158 2021-05-09 08:56:11.000000 sisaptools-1.9.8/sisaptools/textfile.py
--rw-rw-r--   0 sisap     (1000) sisap     (1000)      638 2021-05-09 08:56:11.000000 sisaptools-1.9.8/sisaptools/redis.py
--rw-rw-r--   0 sisap     (1000) sisap     (1000)      908 2021-05-09 08:56:11.000000 sisaptools-1.9.8/sisaptools/constants.py
--rw-rw-r--   0 sisap     (1000) sisap     (1000)     3244 2021-05-09 08:56:11.000000 sisaptools-1.9.8/sisaptools/__init__.py
--rw-rw-r--   0 sisap     (1000) sisap     (1000)    16113 2021-05-09 09:12:39.000000 sisaptools-1.9.8/sisaptools/services.json
--rw-rw-r--   0 sisap     (1000) sisap     (1000)       38 2021-06-15 08:51:09.000000 sisaptools-1.9.8/setup.cfg
--rw-rw-r--   0 sisap     (1000) sisap     (1000)      732 2021-06-15 08:51:09.000000 sisaptools-1.9.8/PKG-INFO
--rw-rw-r--   0 sisap     (1000) sisap     (1000)     1290 2021-06-15 08:51:00.000000 sisaptools-1.9.8/setup.py
-drwxrwxr-x   0 sisap     (1000) sisap     (1000)        0 2021-06-15 08:51:09.000000 sisaptools-1.9.8/sisaptools.egg-info/
--rw-rw-r--   0 sisap     (1000) sisap     (1000)       11 2021-06-15 08:51:09.000000 sisaptools-1.9.8/sisaptools.egg-info/top_level.txt
--rw-rw-r--   0 sisap     (1000) sisap     (1000)      403 2021-06-15 08:51:09.000000 sisaptools-1.9.8/sisaptools.egg-info/SOURCES.txt
--rw-rw-r--   0 sisap     (1000) sisap     (1000)      732 2021-06-15 08:51:09.000000 sisaptools-1.9.8/sisaptools.egg-info/PKG-INFO
--rw-rw-r--   0 sisap     (1000) sisap     (1000)       79 2021-06-15 08:51:09.000000 sisaptools-1.9.8/sisaptools.egg-info/requires.txt
--rw-rw-r--   0 sisap     (1000) sisap     (1000)        1 2021-06-15 08:51:09.000000 sisaptools-1.9.8/sisaptools.egg-info/dependency_links.txt
--rw-rw-r--   0 sisap     (1000) sisap     (1000)     3398 2021-05-09 08:56:11.000000 sisaptools-1.9.8/README.md
+drwxrwxr-x   0 sisap     (1000) sisap     (1000)        0 2021-06-15 09:27:20.000000 sisaptools-1.9.9/
+drwxrwxr-x   0 sisap     (1000) sisap     (1000)        0 2021-06-15 09:27:20.000000 sisaptools-1.9.9/sisaptools/
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)     2194 2021-05-09 08:56:11.000000 sisaptools-1.9.9/sisaptools/mail.py
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)    23933 2021-06-15 09:26:52.000000 sisaptools-1.9.9/sisaptools/database.py
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)      451 2021-05-09 08:56:11.000000 sisaptools-1.9.9/sisaptools/services.py
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)     2192 2021-05-09 08:56:11.000000 sisaptools-1.9.9/sisaptools/ssh.py
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)     1864 2021-05-09 08:56:11.000000 sisaptools-1.9.9/sisaptools/aes.py
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)     1158 2021-05-09 08:56:11.000000 sisaptools-1.9.9/sisaptools/textfile.py
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)      638 2021-05-09 08:56:11.000000 sisaptools-1.9.9/sisaptools/redis.py
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)      908 2021-05-09 08:56:11.000000 sisaptools-1.9.9/sisaptools/constants.py
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)     3244 2021-05-09 08:56:11.000000 sisaptools-1.9.9/sisaptools/__init__.py
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)    16113 2021-05-09 09:12:39.000000 sisaptools-1.9.9/sisaptools/services.json
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)       38 2021-06-15 09:27:20.000000 sisaptools-1.9.9/setup.cfg
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)      732 2021-06-15 09:27:20.000000 sisaptools-1.9.9/PKG-INFO
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)     1290 2021-06-15 09:27:16.000000 sisaptools-1.9.9/setup.py
+drwxrwxr-x   0 sisap     (1000) sisap     (1000)        0 2021-06-15 09:27:20.000000 sisaptools-1.9.9/sisaptools.egg-info/
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)       11 2021-06-15 09:27:20.000000 sisaptools-1.9.9/sisaptools.egg-info/top_level.txt
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)      403 2021-06-15 09:27:20.000000 sisaptools-1.9.9/sisaptools.egg-info/SOURCES.txt
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)      732 2021-06-15 09:27:20.000000 sisaptools-1.9.9/sisaptools.egg-info/PKG-INFO
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)       79 2021-06-15 09:27:20.000000 sisaptools-1.9.9/sisaptools.egg-info/requires.txt
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)        1 2021-06-15 09:27:20.000000 sisaptools-1.9.9/sisaptools.egg-info/dependency_links.txt
+-rw-rw-r--   0 sisap     (1000) sisap     (1000)     3398 2021-05-09 08:56:11.000000 sisaptools-1.9.9/README.md
```

### Comparing `sisaptools-1.9.8/sisaptools/mail.py` & `sisaptools-1.9.9/sisaptools/mail.py`

 * *Files identical despite different names*

### Comparing `sisaptools-1.9.8/sisaptools/database.py` & `sisaptools-1.9.9/sisaptools/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,15 +455,16 @@
                 ('ora', 'DATETIME', 'ora', 'query'): column,
                 ('ora', 'TIMESTAMP(6)', 'my', 'create'): '{column} datetime',
                 ('ora', 'TIMESTAMP(6)', 'my', 'query'):
                     "to_char({column}, 'YYYY-MM-DD HH24:MI:SS')",
                 ('ora', 'TIMESTAMP(6)', 'ora', 'create'): '{column} date',
                 ('ora', 'TIMESTAMP(6)', 'ora', 'query'): column,
                 ('ora', 'NUMBER', 'my', 'create'):
-                    '{column} double' if scale or column.upper() == "GMA_IND_CMPLX"  # noqa
+                    '{column} double' if scale
+                    else '{column} decimal' if column.upper() == "GMA_IND_CMPLX"  # noqa
                     else '{column} int' if not precision or precision < 10
                     else '{column} bigint',
                 ('ora', 'NUMBER', 'my', 'query'): column,
                 ('ora', 'NUMBER', 'ora', 'create'):
                     '{column} number({precision}, {scale})' if scale
                     else '{column} number',
                 ('ora', 'NUMBER', 'ora', 'query'): column,
```

### Comparing `sisaptools-1.9.8/sisaptools/ssh.py` & `sisaptools-1.9.9/sisaptools/ssh.py`

 * *Files identical despite different names*

### Comparing `sisaptools-1.9.8/sisaptools/aes.py` & `sisaptools-1.9.9/sisaptools/aes.py`

 * *Files identical despite different names*

### Comparing `sisaptools-1.9.8/sisaptools/textfile.py` & `sisaptools-1.9.9/sisaptools/textfile.py`

 * *Files identical despite different names*

### Comparing `sisaptools-1.9.8/sisaptools/redis.py` & `sisaptools-1.9.9/sisaptools/redis.py`

 * *Files identical despite different names*

### Comparing `sisaptools-1.9.8/sisaptools/constants.py` & `sisaptools-1.9.9/sisaptools/constants.py`

 * *Files identical despite different names*

### Comparing `sisaptools-1.9.8/sisaptools/__init__.py` & `sisaptools-1.9.9/sisaptools/__init__.py`

 * *Files identical despite different names*

### Comparing `sisaptools-1.9.8/sisaptools/services.json` & `sisaptools-1.9.9/sisaptools/services.json`

 * *Files identical despite different names*

### Comparing `sisaptools-1.9.8/PKG-INFO` & `sisaptools-1.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sisaptools
-Version: 1.9.8
+Version: 1.9.9
 Summary: Eines comunes de SISAP
 Home-page: https://github.com/sisap-ics/sisaptools
 Author: SISAP
 Author-email: sisap@gencat.cat
 License: MIT
 Description: Eines comunes per a l'execució de SISAP i SIDIAP.                       Per a més informació veure                       https://github.com/sisap-ics/sisaptools/
 Keywords: sisap database development
```

### Comparing `sisaptools-1.9.8/setup.py` & `sisaptools-1.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='sisaptools',
-    version='1.9.8',
+    version='1.9.9',
     description='Eines comunes de SISAP',
     long_description='Eines comunes per a l\'execució de SISAP i SIDIAP. \
                       Per a més informació veure \
                       https://github.com/sisap-ics/sisaptools/',
     url='https://github.com/sisap-ics/sisaptools',
     author='SISAP',
     author_email='sisap@gencat.cat',
```

### Comparing `sisaptools-1.9.8/sisaptools.egg-info/PKG-INFO` & `sisaptools-1.9.9/sisaptools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sisaptools
-Version: 1.9.8
+Version: 1.9.9
 Summary: Eines comunes de SISAP
 Home-page: https://github.com/sisap-ics/sisaptools
 Author: SISAP
 Author-email: sisap@gencat.cat
 License: MIT
 Description: Eines comunes per a l'execució de SISAP i SIDIAP.                       Per a més informació veure                       https://github.com/sisap-ics/sisaptools/
 Keywords: sisap database development
```

### Comparing `sisaptools-1.9.8/README.md` & `sisaptools-1.9.9/README.md`

 * *Files identical despite different names*

