# Comparing `tmp/tokendito-2.1.0.tar.gz` & `tmp/tokendito-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokendito-2.1.0.tar", last modified: Fri May 19 19:24:25 2023, max compression
+gzip compressed data, was "tokendito-2.1.1.tar", last modified: Sun May 21 00:35:26 2023, max compression
```

## Comparing `tokendito-2.1.0.tar` & `tokendito-2.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:25.433522 tokendito-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-19 19:24:15.000000 tokendito-2.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-19 19:24:15.000000 tokendito-2.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-19 19:24:15.000000 tokendito-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-19 19:24:25.429522 tokendito-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-19 19:24:15.000000 tokendito-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-19 19:24:15.000000 tokendito-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-19 19:24:15.000000 tokendito-2.1.0/requirements-dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-05-19 19:24:15.000000 tokendito-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 19:24:25.433522 tokendito-2.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2213 2023-05-19 19:24:15.000000 tokendito-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:25.429522 tokendito-2.1.0/tokendito/
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/duo.py
--rw-r--r--   0 runner    (1001) docker     (123)    21679 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/okta.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/tokendito.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)    42028 2023-05-19 19:24:15.000000 tokendito-2.1.0/tokendito/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:24:25.429522 tokendito-2.1.0/tokendito.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 19:24:25.000000 tokendito-2.1.0/tokendito.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:35:26.874058 tokendito-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-21 00:35:16.000000 tokendito-2.1.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-21 00:35:16.000000 tokendito-2.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-21 00:35:16.000000 tokendito-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-21 00:35:26.874058 tokendito-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-21 00:35:16.000000 tokendito-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-21 00:35:16.000000 tokendito-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-21 00:35:16.000000 tokendito-2.1.1/requirements-dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-05-21 00:35:16.000000 tokendito-2.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:35:26.874058 tokendito-2.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2213 2023-05-21 00:35:16.000000 tokendito-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:35:26.874058 tokendito-2.1.1/tokendito/
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/duo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21679 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/okta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/tokendito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41970 2023-05-21 00:35:16.000000 tokendito-2.1.1/tokendito/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:35:26.874058 tokendito-2.1.1/tokendito.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 00:35:26.000000 tokendito-2.1.1/tokendito.egg-info/top_level.txt
```

### Comparing `tokendito-2.1.0/LICENSE.txt` & `tokendito-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.0/PKG-INFO` & `tokendito-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokendito
-Version: 2.1.0
+Version: 2.1.1
 Summary: Get AWS STS tokens from Okta SSO
 Home-page: https://github.com/dowjones/tokendito
 Author: tokendito
 Author-email: tokendito@dowjones.com
 License: Apache 2.0
 Keywords: okta,aws,sts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `tokendito-2.1.0/README.md` & `tokendito-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.0/setup.py` & `tokendito-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.0/tokendito/__init__.py` & `tokendito-2.1.1/tokendito/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import os
 from os.path import expanduser
 import sys
 
 from platformdirs import user_config_dir
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 __title__ = "tokendito"
 __description__ = "Get AWS STS tokens from Okta SSO"
 __long_description_content_type__ = "text/markdown"
 __url__ = "https://github.com/dowjones/tokendito"
 __author__ = "tokendito"
 __author_email__ = "tokendito@dowjones.com"
 __license__ = "Apache 2.0"
```

### Comparing `tokendito-2.1.0/tokendito/__main__.py` & `tokendito-2.1.1/tokendito/__main__.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.0/tokendito/aws.py` & `tokendito-2.1.1/tokendito/aws.py`

 * *Files 6% similar despite different names*

```diff
@@ -200,22 +200,29 @@
 
     :param tiles: tiles metadata, list of tuples
     :return: tuple with AWS AssumeRoleWithSaml response and role name
     """
     authenticated_tiles = {}
     for url, saml_response, saml, label in tiles:
         roles_and_providers = user.extract_arns(saml)
+        if not roles_and_providers:
+            logger.warning(f"Skipping {url}, no valid roles or tile is misconfigured")
+            continue
         authenticated_tiles[url] = {
             "roles": list(roles_and_providers.keys()),
             "saml": saml,
             "saml_response_string": saml_response,
             "roles_and_providers": roles_and_providers,
             "label": label,
         }
 
+    if not authenticated_tiles:
+        logger.error("No roles found. Please check with your Okta admin.")
+        sys.exit(1)
+
     role_arn, _id = user.select_role_arn(authenticated_tiles)
     role_name = role_arn.split("/")[-1]
 
     assume_role_response = assume_role(
         role_arn,
         authenticated_tiles[_id]["roles_and_providers"][role_arn],
         authenticated_tiles[_id]["saml"],
```

### Comparing `tokendito-2.1.0/tokendito/duo.py` & `tokendito-2.1.1/tokendito/duo.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.0/tokendito/okta.py` & `tokendito-2.1.1/tokendito/okta.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.0/tokendito/tokendito.py` & `tokendito-2.1.1/tokendito/tokendito.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.0/tokendito/tool.py` & `tokendito-2.1.1/tokendito/tool.py`

 * *Files identical despite different names*

### Comparing `tokendito-2.1.0/tokendito/user.py` & `tokendito-2.1.1/tokendito/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,28 +451,26 @@
     """Extract arns from SAML decoded xml.
 
     :param saml: results saml decoded
     :return: Dict of Role and Provider ARNs
     """
     logger.debug("Decode response string as a SAML decoded value.")
 
+    roles_and_providers = {}
     arn_regex = ">(arn:aws:iam::.*?,arn:aws:iam::.*?)<"
 
     # find all provider and role pairs.
     arns = re.findall(arn_regex, saml)
-
-    if len(arns) == 0:
-        logger.error("No IAM roles found in SAML response.")
-        logger.debug(arns)
-        sys.exit(2)
+    logger.debug(f"found ARNs: {arns}")
 
     # stuff into dict, role is dict key.
-    roles_and_providers = {i.split(",")[1]: i.split(",")[0] for i in arns}
+    if arns:
+        roles_and_providers = {i.split(",")[1]: i.split(",")[0] for i in arns}
 
-    logger.debug(f"Collected ARNs: {json.dumps(roles_and_providers)}")
+    logger.debug(f"Collected ARNs: {roles_and_providers}")
 
     return roles_and_providers
 
 
 def validate_okta_org(input_url=None):
     """Validate whether a given URL is a valid AWS Org URL in Okta.
```

### Comparing `tokendito-2.1.0/tokendito.egg-info/PKG-INFO` & `tokendito-2.1.1/tokendito.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokendito
-Version: 2.1.0
+Version: 2.1.1
 Summary: Get AWS STS tokens from Okta SSO
 Home-page: https://github.com/dowjones/tokendito
 Author: tokendito
 Author-email: tokendito@dowjones.com
 License: Apache 2.0
 Keywords: okta,aws,sts
 Classifier: License :: OSI Approved :: Apache Software License
```

