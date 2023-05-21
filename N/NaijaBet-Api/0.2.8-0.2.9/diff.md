# Comparing `tmp/NaijaBet_Api-0.2.8.tar.gz` & `tmp/NaijaBet_Api-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NaijaBet_Api-0.2.8.tar", last modified: Sat Aug 21 16:44:28 2021, max compression
+gzip compressed data, was "NaijaBet_Api-0.2.9.tar", last modified: Wed Sep  1 13:04:58 2021, max compression
```

## Comparing `NaijaBet_Api-0.2.8.tar` & `NaijaBet_Api-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-21 16:44:28.881654 NaijaBet_Api-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-21 16:44:28.877654 NaijaBet_Api-0.2.8/NaijaBet_Api/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/NaijaBet_Api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/NaijaBet_Api/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-21 16:44:28.881654 NaijaBet_Api-0.2.8/NaijaBet_Api/bookmakers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/NaijaBet_Api/bookmakers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/NaijaBet_Api/bookmakers/bet9ja.py
--rw-r--r--   0 runner    (1001) docker     (121)     1926 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/NaijaBet_Api/bookmakers/betking.py
--rw-r--r--   0 runner    (1001) docker     (121)     2159 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/NaijaBet_Api/bookmakers/nairabet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2871 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/NaijaBet_Api/id.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-21 16:44:28.881654 NaijaBet_Api-0.2.8/NaijaBet_Api/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/NaijaBet_Api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10896 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/NaijaBet_Api/utils/bet9ja_normalizer.json
--rw-r--r--   0 runner    (1001) docker     (121)    12435 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/NaijaBet_Api/utils/betking_normalizer.json
--rw-r--r--   0 runner    (1001) docker     (121)     2899 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/NaijaBet_Api/utils/jsonpaths.py
--rw-r--r--   0 runner    (1001) docker     (121)    14472 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/NaijaBet_Api/utils/nairabet_normalizer.json
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/NaijaBet_Api/utils/normalizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-21 16:44:28.881654 NaijaBet_Api-0.2.8/NaijaBet_Api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2021-08-21 16:44:28.000000 NaijaBet_Api-0.2.8/NaijaBet_Api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      647 2021-08-21 16:44:28.000000 NaijaBet_Api-0.2.8/NaijaBet_Api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-21 16:44:28.000000 NaijaBet_Api-0.2.8/NaijaBet_Api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-08-21 16:44:28.000000 NaijaBet_Api-0.2.8/NaijaBet_Api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2021-08-21 16:44:28.881654 NaijaBet_Api-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-08-21 16:44:12.000000 NaijaBet_Api-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-08-21 16:44:28.881654 NaijaBet_Api-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 13:04:58.914538 NaijaBet_Api-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 13:04:58.910538 NaijaBet_Api-0.2.9/NaijaBet_Api/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 13:04:58.914538 NaijaBet_Api-0.2.9/NaijaBet_Api/bookmakers/
+-rw-r--r--   0 runner    (1001) docker     (121)     3812 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/bookmakers/BaseClass.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/bookmakers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/bookmakers/bet9ja.py
+-rw-r--r--   0 runner    (1001) docker     (121)      717 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/bookmakers/betking.py
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/bookmakers/nairabet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2871 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/id.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 13:04:58.914538 NaijaBet_Api-0.2.9/NaijaBet_Api/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10896 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/utils/bet9ja_normalizer.json
+-rw-r--r--   0 runner    (1001) docker     (121)    12435 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/utils/betking_normalizer.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2899 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/utils/jsonpaths.py
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14472 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/utils/nairabet_normalizer.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1984 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/NaijaBet_Api/utils/normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-01 13:04:58.914538 NaijaBet_Api-0.2.9/NaijaBet_Api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2357 2021-09-01 13:04:58.000000 NaijaBet_Api-0.2.9/NaijaBet_Api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      717 2021-09-01 13:04:58.000000 NaijaBet_Api-0.2.9/NaijaBet_Api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-01 13:04:58.000000 NaijaBet_Api-0.2.9/NaijaBet_Api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-09-01 13:04:58.000000 NaijaBet_Api-0.2.9/NaijaBet_Api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2357 2021-09-01 13:04:58.914538 NaijaBet_Api-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1803 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2021-09-01 13:04:35.000000 NaijaBet_Api-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-09-01 13:04:58.914538 NaijaBet_Api-0.2.9/setup.cfg
```

### Comparing `NaijaBet_Api-0.2.8/LICENSE` & `NaijaBet_Api-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `NaijaBet_Api-0.2.8/NaijaBet_Api/id.py` & `NaijaBet_Api-0.2.9/NaijaBet_Api/id.py`

 * *Files identical despite different names*

### Comparing `NaijaBet_Api-0.2.8/NaijaBet_Api/utils/bet9ja_normalizer.json` & `NaijaBet_Api-0.2.9/NaijaBet_Api/utils/bet9ja_normalizer.json`

 * *Files identical despite different names*

### Comparing `NaijaBet_Api-0.2.8/NaijaBet_Api/utils/betking_normalizer.json` & `NaijaBet_Api-0.2.9/NaijaBet_Api/utils/betking_normalizer.json`

 * *Files identical despite different names*

### Comparing `NaijaBet_Api-0.2.8/NaijaBet_Api/utils/jsonpaths.py` & `NaijaBet_Api-0.2.9/NaijaBet_Api/utils/jsonpaths.py`

 * *Files identical despite different names*

### Comparing `NaijaBet_Api-0.2.8/NaijaBet_Api/utils/nairabet_normalizer.json` & `NaijaBet_Api-0.2.9/NaijaBet_Api/utils/nairabet_normalizer.json`

 * *Files identical despite different names*

### Comparing `NaijaBet_Api-0.2.8/NaijaBet_Api.egg-info/PKG-INFO` & `NaijaBet_Api-0.2.9/NaijaBet_Api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NaijaBet-Api
-Version: 0.2.8
+Version: 0.2.9
 Summary: A wrapper around the API of Nigerias major betting sites
 Home-page: https://github.com/jayteealao/Naijabet_Api
 Author: graphitenerd
 Author-email: jayteealao@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jayteealao/Naijabet_Api/issues
 Platform: UNKNOWN
```

### Comparing `NaijaBet_Api-0.2.8/NaijaBet_Api.egg-info/SOURCES.txt` & `NaijaBet_Api-0.2.9/NaijaBet_Api.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 ./NaijaBet_Api/__init__.py
 ./NaijaBet_Api/__main__.py
 ./NaijaBet_Api/id.py
+./NaijaBet_Api/bookmakers/BaseClass.py
 ./NaijaBet_Api/bookmakers/__init__.py
 ./NaijaBet_Api/bookmakers/bet9ja.py
 ./NaijaBet_Api/bookmakers/betking.py
 ./NaijaBet_Api/bookmakers/nairabet.py
 ./NaijaBet_Api/utils/__init__.py
 ./NaijaBet_Api/utils/bet9ja_normalizer.json
 ./NaijaBet_Api/utils/betking_normalizer.json
 ./NaijaBet_Api/utils/jsonpaths.py
+./NaijaBet_Api/utils/logger.py
 ./NaijaBet_Api/utils/nairabet_normalizer.json
 ./NaijaBet_Api/utils/normalizer.py
 NaijaBet_Api.egg-info/PKG-INFO
 NaijaBet_Api.egg-info/SOURCES.txt
 NaijaBet_Api.egg-info/dependency_links.txt
 NaijaBet_Api.egg-info/top_level.txt
```

### Comparing `NaijaBet_Api-0.2.8/PKG-INFO` & `NaijaBet_Api-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NaijaBet_Api
-Version: 0.2.8
+Version: 0.2.9
 Summary: A wrapper around the API of Nigerias major betting sites
 Home-page: https://github.com/jayteealao/Naijabet_Api
 Author: graphitenerd
 Author-email: jayteealao@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jayteealao/Naijabet_Api/issues
 Platform: UNKNOWN
```

### Comparing `NaijaBet_Api-0.2.8/README.md` & `NaijaBet_Api-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `NaijaBet_Api-0.2.8/setup.cfg` & `NaijaBet_Api-0.2.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = NaijaBet_Api
-version = 0.2.8
+version = 0.2.9
 author = graphitenerd
 author_email = jayteealao@gmail.com
 description = A wrapper around the API of Nigerias major betting sites
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jayteealao/Naijabet_Api
 project_urls =
```

