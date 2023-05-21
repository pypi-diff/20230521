# Comparing `tmp/audit_logging_pepsico-0.0.5.tar.gz` & `tmp/audit_logging_pepsico-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audit_logging_pepsico-0.0.5.tar", last modified: Mon Feb  6 10:27:52 2023, max compression
+gzip compressed data, was "audit_logging_pepsico-0.0.6.tar", last modified: Sun May 21 21:14:09 2023, max compression
```

## Comparing `audit_logging_pepsico-0.0.5.tar` & `audit_logging_pepsico-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-02-06 10:27:52.070746 audit_logging_pepsico-0.0.5/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 audit_logging_pepsico-0.0.5/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1500 2023-02-06 10:27:52.070367 audit_logging_pepsico-0.0.5/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 audit_logging_pepsico-0.0.5/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-02-06 10:27:52.066207 audit_logging_pepsico-0.0.5/audit_logging_pepsico/
--rw-r--r--   0 jatintalati   (501) staff       (20)     3001 2023-01-19 18:16:00.000000 audit_logging_pepsico-0.0.5/audit_logging_pepsico/audit.py
--rw-r--r--   0 jatintalati   (501) staff       (20)     2970 2023-02-03 11:33:41.000000 audit_logging_pepsico-0.0.5/audit_logging_pepsico/audit_config.py
--rw-r--r--   0 jatintalati   (501) staff       (20)      152 2023-01-19 18:09:47.000000 audit_logging_pepsico-0.0.5/audit_logging_pepsico/constants.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-02-06 10:27:52.069689 audit_logging_pepsico-0.0.5/audit_logging_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1500 2023-02-06 10:27:52.000000 audit_logging_pepsico-0.0.5/audit_logging_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      360 2023-02-06 10:27:52.000000 audit_logging_pepsico-0.0.5/audit_logging_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-02-06 10:27:52.000000 audit_logging_pepsico-0.0.5/audit_logging_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       62 2023-02-06 10:27:52.000000 audit_logging_pepsico-0.0.5/audit_logging_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       22 2023-02-06 10:27:52.000000 audit_logging_pepsico-0.0.5/audit_logging_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      684 2023-02-03 11:42:43.000000 audit_logging_pepsico-0.0.5/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-02-06 10:27:52.070877 audit_logging_pepsico-0.0.5/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-21 21:14:09.753518 audit_logging_pepsico-0.0.6/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 audit_logging_pepsico-0.0.6/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-05-21 21:14:09.752870 audit_logging_pepsico-0.0.6/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 audit_logging_pepsico-0.0.6/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-21 21:14:09.748998 audit_logging_pepsico-0.0.6/audit_logging_pepsico/
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     2059 2023-05-21 21:09:26.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico/Kafka_log.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     3021 2023-05-17 06:47:52.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico/audit.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     2978 2023-05-17 06:46:50.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico/audit_config.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)      152 2023-05-02 11:42:24.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico/constants.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     4901 2023-05-18 10:09:56.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico/kafka_utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-05-21 21:14:09.751963 audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-05-21 21:14:09.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      436 2023-05-21 21:14:09.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-05-21 21:14:09.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       88 2023-05-21 21:14:09.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       22 2023-05-21 21:14:09.000000 audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      742 2023-05-21 21:11:33.000000 audit_logging_pepsico-0.0.6/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-05-21 21:14:09.753790 audit_logging_pepsico-0.0.6/setup.cfg
```

### Comparing `audit_logging_pepsico-0.0.5/LICENSE` & `audit_logging_pepsico-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.5/PKG-INFO` & `audit_logging_pepsico-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: audit_logging_pepsico
-Version: 0.0.5
+Version: 0.0.6
 Summary: A logging package which allows users to log in pepsico format. Specially write logs for request and response.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
-Keywords: logging,audit,pepsico
+Keywords: logging,audit,pepsico,kafka,couchbase
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `audit_logging_pepsico-0.0.5/README.md` & `audit_logging_pepsico-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-0.0.5/audit_logging_pepsico/audit.py` & `audit_logging_pepsico-0.0.6/audit_logging_pepsico/audit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import audit_logging_pepsico.constants as con
 class Audit:
     serialVersionUID = 1
 
     def __init__(self, id, channelId, systemId, ipAddress, userId, customerId, createdDate, url, interfaceName,
-                 operationName, orderId, coRelationId, sourceOrderNumber, externalId, requestHeader, responseCode, type,
+                 operationName, orderId, coRelationId, sourceOrderNumber, externalId, requestHeader, responseCode, log_type,
                  documentType, componentName, methodName, requestInput, responseOutput, gpid, route):
 
         self.prefix = con.PREFIX
         self.id = id
         self.channelId = channelId
         self.systemId = systemId
         self.ipAddress = ipAddress
@@ -19,15 +19,15 @@
         self.operationName = operationName
         self.orderId = orderId
         self.coRelationId = coRelationId
         self.sourceOrderNumber = sourceOrderNumber
         self.externalId = externalId
         self.requestHeader = requestHeader
         self.responseCode = responseCode
-        self.type = type
+        self.log_type = log_type
         self.documentType = documentType
         self.componentName = componentName
         self.methodName = methodName
         self.requestInput = requestInput
         self.responseOutput = responseOutput
         self.gpid = gpid
         self.route = route
@@ -53,15 +53,15 @@
             ", operationName='" + str(self.operationName) + '\'' + \
             ", orderId='" + str(self.orderId) + '\'' + \
             ", coRelationId='" + str(self.coRelationId) + '\'' + \
             ", sourceOrderNumber='" + str(self.sourceOrderNumber) + '\'' + \
             ", externalId='" + str(self.externalId) + '\'' + \
             ", requestHeader='" + str(self.requestHeader) + '\'' + \
             ", responseCode=" + str(self.responseCode) + \
-            ", type='" + str(self.type) + '\'' + \
+            ", log_type='" + str(self.log_type) + '\'' + \
             ", documentType='" + str(self.documentType) + '\'' + \
             ", componentName='" + str(self.componentName) + '\'' + \
             ", methodName='" + str(self.methodName) + '\'' + \
             ", requestInput=" + str(self.requestInput) + \
             ", responseOutput=" + str(self.responseOutput) + \
             ", gpid='" + str(self.gpid) + '\'' + \
             ", route='" + str(self.route) + '\'' + \
```

### Comparing `audit_logging_pepsico-0.0.5/audit_logging_pepsico/audit_config.py` & `audit_logging_pepsico-0.0.6/audit_logging_pepsico/audit_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,19 @@
                   componentName=None, methodName=None, requestInput=None, responseOutput=None, gpid=None, route=None,
                   write_to_blob=False, block_blob_client=None):
         try:
             ip_addr = ip_address
             id = con.AUDIT_PRIFIX + con.ID_DELIMITER + str(uuid.uuid4())
             createdDate = datetime.now()
             interfaceName = con.INTERFACE_NAME
-            type = con.AUDIT_SERVICE
+            log_type = con.AUDIT_SERVICE
             audit_obj = Audit(id, channelId, systemId, ip_addr,
                               userId, customerId, createdDate, url, interfaceName, operationName, orderId,
                               coRelationId, sourceOrderNumber,
-                              externalId, requestHeader, responseCode, type, documentType, componentName,
+                              externalId, requestHeader, responseCode, log_type, documentType, componentName,
                               methodName, requestInput, responseOutput, gpid, route)
             logs = audit_obj.__str__()
             if not write_to_blob:
                 logger.debug(logs)
             else:
                 block_blob_client.append_block(logs, length=len(logs))
         except:
```

### Comparing `audit_logging_pepsico-0.0.5/audit_logging_pepsico.egg-info/PKG-INFO` & `audit_logging_pepsico-0.0.6/audit_logging_pepsico.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: audit-logging-pepsico
-Version: 0.0.5
+Version: 0.0.6
 Summary: A logging package which allows users to log in pepsico format. Specially write logs for request and response.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
-Keywords: logging,audit,pepsico
+Keywords: logging,audit,pepsico,kafka,couchbase
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

