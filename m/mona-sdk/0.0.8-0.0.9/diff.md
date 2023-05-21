# Comparing `tmp/mona_sdk-0.0.8.tar.gz` & `tmp/mona_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/anatbarsinai/workspace/mona-sdk/dist/tmpm78j72zd/mona_sdk-0.0.8.tar", last modified: Sun May  2 08:41:49 2021, max compression
+gzip compressed data, was "/Users/anatbarsinai/workspace/mona-sdk/dist/tmp5zi304lm/mona_sdk-0.0.9.tar", last modified: Sun May  2 09:15:13 2021, max compression
```

## Comparing `mona_sdk-0.0.8.tar` & `mona_sdk-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anatbarsinai   (501) staff       (20)        0 2021-05-02 08:41:49.422168 mona_sdk-0.0.8/
--rw-r--r--   0 anatbarsinai   (501) staff       (20)    11357 2021-04-08 11:18:22.000000 mona_sdk-0.0.8/LICENSE
--rw-r--r--   0 anatbarsinai   (501) staff       (20)     7604 2021-05-02 08:41:49.421864 mona_sdk-0.0.8/PKG-INFO
--rw-r--r--   0 anatbarsinai   (501) staff       (20)     5939 2021-05-02 08:41:03.000000 mona_sdk-0.0.8/README.md
-drwxr-xr-x   0 anatbarsinai   (501) staff       (20)        0 2021-05-02 08:41:49.412275 mona_sdk-0.0.8/mona_sdk/
--rw-r--r--   0 anatbarsinai   (501) staff       (20)      109 2021-04-14 11:24:00.000000 mona_sdk-0.0.8/mona_sdk/__init__.py
--rw-r--r--   0 anatbarsinai   (501) staff       (20)    12296 2021-05-02 08:41:03.000000 mona_sdk-0.0.8/mona_sdk/authentication.py
--rw-r--r--   0 anatbarsinai   (501) staff       (20)    12973 2021-05-02 08:41:03.000000 mona_sdk-0.0.8/mona_sdk/client.py
--rw-r--r--   0 anatbarsinai   (501) staff       (20)      229 2021-05-02 08:41:03.000000 mona_sdk-0.0.8/mona_sdk/client_exceptions.py
--rw-r--r--   0 anatbarsinai   (501) staff       (20)      334 2021-04-14 11:24:00.000000 mona_sdk-0.0.8/mona_sdk/client_util.py
--rw-r--r--   0 anatbarsinai   (501) staff       (20)     1436 2021-04-14 11:24:00.000000 mona_sdk-0.0.8/mona_sdk/logger.py
--rw-r--r--   0 anatbarsinai   (501) staff       (20)     3292 2021-04-14 11:24:00.000000 mona_sdk-0.0.8/mona_sdk/validation.py
-drwxr-xr-x   0 anatbarsinai   (501) staff       (20)        0 2021-05-02 08:41:49.421335 mona_sdk-0.0.8/mona_sdk.egg-info/
--rw-r--r--   0 anatbarsinai   (501) staff       (20)     7604 2021-05-02 08:41:49.000000 mona_sdk-0.0.8/mona_sdk.egg-info/PKG-INFO
--rw-r--r--   0 anatbarsinai   (501) staff       (20)      363 2021-05-02 08:41:49.000000 mona_sdk-0.0.8/mona_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 anatbarsinai   (501) staff       (20)        1 2021-05-02 08:41:49.000000 mona_sdk-0.0.8/mona_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 anatbarsinai   (501) staff       (20)       53 2021-05-02 08:41:49.000000 mona_sdk-0.0.8/mona_sdk.egg-info/requires.txt
--rw-r--r--   0 anatbarsinai   (501) staff       (20)        9 2021-05-02 08:41:49.000000 mona_sdk-0.0.8/mona_sdk.egg-info/top_level.txt
--rw-r--r--   0 anatbarsinai   (501) staff       (20)      104 2021-04-14 11:37:05.000000 mona_sdk-0.0.8/pyproject.toml
--rw-r--r--   0 anatbarsinai   (501) staff       (20)       38 2021-05-02 08:41:49.422266 mona_sdk-0.0.8/setup.cfg
--rw-r--r--   0 anatbarsinai   (501) staff       (20)      803 2021-05-02 08:41:03.000000 mona_sdk-0.0.8/setup.py
+drwxr-xr-x   0 anatbarsinai   (501) staff       (20)        0 2021-05-02 09:15:13.211681 mona_sdk-0.0.9/
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)    11357 2021-04-08 11:18:22.000000 mona_sdk-0.0.9/LICENSE
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)     7665 2021-05-02 09:15:13.211420 mona_sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)     5992 2021-05-02 08:57:27.000000 mona_sdk-0.0.9/README.md
+drwxr-xr-x   0 anatbarsinai   (501) staff       (20)        0 2021-05-02 09:15:13.201618 mona_sdk-0.0.9/mona_sdk/
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)      109 2021-04-14 11:24:00.000000 mona_sdk-0.0.9/mona_sdk/__init__.py
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)    12296 2021-05-02 08:41:03.000000 mona_sdk-0.0.9/mona_sdk/authentication.py
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)    12953 2021-05-02 08:57:27.000000 mona_sdk-0.0.9/mona_sdk/client.py
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)      229 2021-05-02 08:41:03.000000 mona_sdk-0.0.9/mona_sdk/client_exceptions.py
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)      334 2021-04-14 11:24:00.000000 mona_sdk-0.0.9/mona_sdk/client_util.py
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)     1436 2021-04-14 11:24:00.000000 mona_sdk-0.0.9/mona_sdk/logger.py
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)     3292 2021-04-14 11:24:00.000000 mona_sdk-0.0.9/mona_sdk/validation.py
+drwxr-xr-x   0 anatbarsinai   (501) staff       (20)        0 2021-05-02 09:15:13.210968 mona_sdk-0.0.9/mona_sdk.egg-info/
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)     7665 2021-05-02 09:15:13.000000 mona_sdk-0.0.9/mona_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)      363 2021-05-02 09:15:13.000000 mona_sdk-0.0.9/mona_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)        1 2021-05-02 09:15:13.000000 mona_sdk-0.0.9/mona_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)       53 2021-05-02 09:15:13.000000 mona_sdk-0.0.9/mona_sdk.egg-info/requires.txt
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)        9 2021-05-02 09:15:13.000000 mona_sdk-0.0.9/mona_sdk.egg-info/top_level.txt
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)      104 2021-04-14 11:37:05.000000 mona_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)       38 2021-05-02 09:15:13.211768 mona_sdk-0.0.9/setup.cfg
+-rw-r--r--   0 anatbarsinai   (501) staff       (20)      803 2021-05-02 09:12:58.000000 mona_sdk-0.0.9/setup.py
```

### Comparing `mona_sdk-0.0.8/LICENSE` & `mona_sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mona_sdk-0.0.8/PKG-INFO` & `mona_sdk-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mona_sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: SDK for communicating with Mona's servers
 Home-page: https://github.com/monalabs/mona-sdk
 Author: MonaLabs
 Author-email: sdk@monalabs.io
 License: UNKNOWN
 Download-URL: http://pypi.python.org/pypi/mona-sdk/
 Description: # Mona Python SDK
@@ -75,15 +75,16 @@
                 )
                 
         export_result = my_mona_client.export_batch(messages_batch_to_mona)
         ```
         ### Uploading a new configuration
         Mona's sdk provides a simple way to upload a new Mona configuration, using Client.upload_config():
         ```
-        new_configuration = {"YOUR_COMPANY_TENANT_ID": <Your new Mona configuration>}
+        # Note: no need to add your tenant_id as the key, just the configuration itself.
+        new_configuration = <Your new Mona configuration>
         upload_result = my_client.upload_config(new_configuration, "My commit message")
         
         # the return value format will be:
         # upload_result == {
         #    "success": <was the upload successful>, (bool)
         #    "new_config_id": <the new configuration ID> (str)
         #}
```

### Comparing `mona_sdk-0.0.8/README.md` & `mona_sdk-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,16 @@
         )
         
 export_result = my_mona_client.export_batch(messages_batch_to_mona)
 ```
 ### Uploading a new configuration
 Mona's sdk provides a simple way to upload a new Mona configuration, using Client.upload_config():
 ```
-new_configuration = {"YOUR_COMPANY_TENANT_ID": <Your new Mona configuration>}
+# Note: no need to add your tenant_id as the key, just the configuration itself.
+new_configuration = <Your new Mona configuration>
 upload_result = my_client.upload_config(new_configuration, "My commit message")
 
 # the return value format will be:
 # upload_result == {
 #    "success": <was the upload successful>, (bool)
 #    "new_config_id": <the new configuration ID> (str)
 #}
```

### Comparing `mona_sdk-0.0.8/mona_sdk/authentication.py` & `mona_sdk-0.0.9/mona_sdk/authentication.py`

 * *Files identical despite different names*

### Comparing `mona_sdk-0.0.8/mona_sdk/client.py` & `mona_sdk-0.0.9/mona_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,28 +258,25 @@
         """
         Uploads a new configuration, as a json-serializable dict.
         The configuration file enables you to define how the exported data should be
         aggregated and analyzed in Mona, as well as your insight and alerting
         preferences.
         Find more information on creating your configuration at:
         https://docs.monalabs.io/.
-        :param config: (dict)
-            json-serializable dict of the following format:
-            {
-            "YOUR_COMPANY_TENANT_ID": <your_new_configuration>
-            }
+        :param config: (dict) your configuration, no need for your tenant id as key,
+        first layer of keys should be the context classes.
         :param commit_message: (str)
         :return: A dict holding the upload data:
         {
             "success": <was the upload successful>, (bool)
             "new_config_id": <the new configuration ID> (str)
         }
         """
         config_to_upload = {
-            "config": config,
+            "config": {self._user_id: config},
             "author": self._api_key,
             "commit_message": commit_message,
             "user_id": self._user_id,
         }
         upload_output = {"success": False, "new_config_id": ""}
         try:
             upload_response = requests.post(
```

### Comparing `mona_sdk-0.0.8/mona_sdk/logger.py` & `mona_sdk-0.0.9/mona_sdk/logger.py`

 * *Files identical despite different names*

### Comparing `mona_sdk-0.0.8/mona_sdk/validation.py` & `mona_sdk-0.0.9/mona_sdk/validation.py`

 * *Files identical despite different names*

### Comparing `mona_sdk-0.0.8/mona_sdk.egg-info/PKG-INFO` & `mona_sdk-0.0.9/mona_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mona-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: SDK for communicating with Mona's servers
 Home-page: https://github.com/monalabs/mona-sdk
 Author: MonaLabs
 Author-email: sdk@monalabs.io
 License: UNKNOWN
 Download-URL: http://pypi.python.org/pypi/mona-sdk/
 Description: # Mona Python SDK
@@ -75,15 +75,16 @@
                 )
                 
         export_result = my_mona_client.export_batch(messages_batch_to_mona)
         ```
         ### Uploading a new configuration
         Mona's sdk provides a simple way to upload a new Mona configuration, using Client.upload_config():
         ```
-        new_configuration = {"YOUR_COMPANY_TENANT_ID": <Your new Mona configuration>}
+        # Note: no need to add your tenant_id as the key, just the configuration itself.
+        new_configuration = <Your new Mona configuration>
         upload_result = my_client.upload_config(new_configuration, "My commit message")
         
         # the return value format will be:
         # upload_result == {
         #    "success": <was the upload successful>, (bool)
         #    "new_config_id": <the new configuration ID> (str)
         #}
```

### Comparing `mona_sdk-0.0.8/setup.py` & `mona_sdk-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mona_sdk",
-    version="0.0.8",
+    version="0.0.9",
     author="MonaLabs",
     author_email="sdk@monalabs.io",
     description="SDK for communicating with Mona's servers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/monalabs/mona-sdk",
     download_url='http://pypi.python.org/pypi/mona-sdk/',
```

