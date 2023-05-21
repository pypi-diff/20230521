# Comparing `tmp/ondewo-csi-client-3.1.1.tar.gz` & `tmp/ondewo-csi-client-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-csi-client-3.1.1.tar", last modified: Tue Apr 18 09:43:05 2023, max compression
+gzip compressed data, was "ondewo-csi-client-3.2.0.tar", last modified: Sun May 21 18:24:11 2023, max compression
```

## Comparing `ondewo-csi-client-3.1.1.tar` & `ondewo-csi-client-3.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:43:05.197585 ondewo-csi-client-3.1.1/
--rw-rw-r--   0 root         (0) root         (0)    10257 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7365 2023-04-18 09:43:05.197585 ondewo-csi-client-3.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     6526 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:43:05.196585 ondewo-csi-client-3.1.1/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:43:05.196585 ondewo-csi-client-3.1.1/ondewo/csi/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:43:05.196585 ondewo-csi-client-3.1.1/ondewo/csi/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1370 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      872 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:43:05.196585 ondewo-csi-client-3.1.1/ondewo/csi/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3151 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/client/services/conversations.py
--rw-rw-r--   0 root         (0) root         (0)      879 2023-01-24 18:48:24.000000 ondewo-csi-client-3.1.1/ondewo/csi/client/services_container.py
--rw-rw-r--   0 root         (0) root         (0)    16188 2023-04-18 09:39:40.000000 ondewo-csi-client-3.1.1/ondewo/csi/conversation_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    19025 2023-04-18 09:39:40.000000 ondewo-csi-client-3.1.1/ondewo/csi/conversation_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 09:43:05.197585 ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7365 2023-04-18 09:43:05.000000 ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      577 2023-04-18 09:43:05.000000 ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 09:43:05.000000 ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      202 2023-04-18 09:43:05.000000 ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-18 09:43:05.000000 ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2023-04-18 09:43:05.197585 ondewo-csi-client-3.1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1902 2023-04-18 09:39:44.000000 ondewo-csi-client-3.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:24:11.726235 ondewo-csi-client-3.2.0/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-05-21 18:24:11.726235 ondewo-csi-client-3.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6526 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:24:11.725235 ondewo-csi-client-3.2.0/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:24:11.725235 ondewo-csi-client-3.2.0/ondewo/csi/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:24:11.725235 ondewo-csi-client-3.2.0/ondewo/csi/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1370 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      872 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:24:11.725235 ondewo-csi-client-3.2.0/ondewo/csi/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3151 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/client/services/conversations.py
+-rw-rw-r--   0 root         (0) root         (0)      879 2023-05-21 18:21:29.000000 ondewo-csi-client-3.2.0/ondewo/csi/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    16188 2023-05-21 18:22:50.000000 ondewo-csi-client-3.2.0/ondewo/csi/conversation_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    19025 2023-05-21 18:22:50.000000 ondewo-csi-client-3.2.0/ondewo/csi/conversation_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 18:24:11.726235 ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-05-21 18:24:11.000000 ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      577 2023-05-21 18:24:11.000000 ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 18:24:11.000000 ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-21 18:24:11.000000 ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-21 18:24:11.000000 ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-05-21 18:24:11.726235 ondewo-csi-client-3.2.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1902 2023-05-21 18:22:54.000000 ondewo-csi-client-3.2.0/setup.py
```

### Comparing `ondewo-csi-client-3.1.1/LICENSE` & `ondewo-csi-client-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.1/PKG-INFO` & `ondewo-csi-client-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-csi-client
-Version: 3.1.1
+Version: 3.2.0
 Summary: Provides endpoints and messages for gRPC communication to the ONDEWO CSI server
 Home-page: https://github.com/ondewo/ondewo-csi-client-python
 Author: ONDEWO GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-csi-client Version: 3.1.1 Summary: Provides
+Metadata-Version: 2.1 Name: ondewo-csi-client Version: 3.2.0 Summary: Provides
 endpoints and messages for gRPC communication to the ONDEWO CSI server Home-
 page: https://github.com/ondewo/ondewo-csi-client-python Author: ONDEWO GbmH
 Author-email: office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `ondewo-csi-client-3.1.1/README.md` & `ondewo-csi-client-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.1/ondewo/csi/client/client.py` & `ondewo-csi-client-3.2.0/ondewo/csi/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.1/ondewo/csi/client/client_config.py` & `ondewo-csi-client-3.2.0/ondewo/csi/client/client_config.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.1/ondewo/csi/client/services/conversations.py` & `ondewo-csi-client-3.2.0/ondewo/csi/client/services/conversations.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.1/ondewo/csi/client/services_container.py` & `ondewo-csi-client-3.2.0/ondewo/csi/client/services_container.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.1/ondewo/csi/conversation_pb2.py` & `ondewo-csi-client-3.2.0/ondewo/csi/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.1/ondewo/csi/conversation_pb2_grpc.py` & `ondewo-csi-client-3.2.0/ondewo/csi/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/PKG-INFO` & `ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-csi-client
-Version: 3.1.1
+Version: 3.2.0
 Summary: Provides endpoints and messages for gRPC communication to the ONDEWO CSI server
 Home-page: https://github.com/ondewo/ondewo-csi-client-python
 Author: ONDEWO GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-csi-client Version: 3.1.1 Summary: Provides
+Metadata-Version: 2.1 Name: ondewo-csi-client Version: 3.2.0 Summary: Provides
 endpoints and messages for gRPC communication to the ONDEWO CSI server Home-
 page: https://github.com/ondewo/ondewo-csi-client-python Author: ONDEWO GbmH
 Author-email: office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `ondewo-csi-client-3.1.1/ondewo_csi_client.egg-info/SOURCES.txt` & `ondewo-csi-client-3.2.0/ondewo_csi_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ondewo-csi-client-3.1.1/setup.py` & `ondewo-csi-client-3.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 long_description: str = read_file('README.md')
 requires: List[str] = read_requirements('requirements.txt')
 
 setup(
     name="ondewo-csi-client",
-    version='3.1.1',
+    version='3.2.0',
     author="ONDEWO GbmH",
     author_email="office@ondewo.com",
     description="Provides endpoints and messages for gRPC communication to the ONDEWO CSI server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ondewo/ondewo-csi-client-python",
     packages=[
```

