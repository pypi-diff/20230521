# Comparing `tmp/guacli-1.1.0.tar.gz` & `tmp/guacli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guacli-1.1.0.tar", last modified: Sun May 21 18:43:23 2023, max compression
+gzip compressed data, was "guacli-1.1.1.tar", last modified: Sun May 21 19:29:46 2023, max compression
```

## Comparing `guacli-1.1.0.tar` & `guacli-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 18:43:23.545627 guacli-1.1.0/
--rw-rw-rw-   0        0        0    11357 2022-11-14 15:57:40.000000 guacli-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1886 2023-05-21 18:43:23.545627 guacli-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1434 2023-02-01 11:22:42.000000 guacli-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 18:43:23.535733 guacli-1.1.0/guacli/
--rw-rw-rw-   0        0        0       23 2023-05-21 17:05:49.000000 guacli-1.1.0/guacli/__init__.py
--rw-rw-rw-   0        0        0    13902 2023-05-21 18:41:51.000000 guacli-1.1.0/guacli/cli.py
--rw-rw-rw-   0        0        0    12635 2023-05-21 18:25:39.000000 guacli-1.1.0/guacli/guacamoleClient.py
-drwxrwxrwx   0        0        0        0 2023-05-21 18:43:23.545627 guacli-1.1.0/guacli.egg-info/
--rw-rw-rw-   0        0        0     1886 2023-05-21 18:43:23.000000 guacli-1.1.0/guacli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-05-21 18:43:23.000000 guacli-1.1.0/guacli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 18:43:23.000000 guacli-1.1.0/guacli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-21 18:43:23.000000 guacli-1.1.0/guacli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-05-21 18:43:23.000000 guacli-1.1.0/guacli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 18:43:23.545627 guacli-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      719 2022-11-30 20:02:13.000000 guacli-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:29:46.054745 guacli-1.1.1/
+-rw-rw-rw-   0        0        0    11357 2022-11-14 15:57:40.000000 guacli-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1886 2023-05-21 19:29:46.054745 guacli-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1434 2023-02-01 11:22:42.000000 guacli-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 19:29:46.044926 guacli-1.1.1/guacli/
+-rw-rw-rw-   0        0        0       23 2023-05-21 19:15:36.000000 guacli-1.1.1/guacli/__init__.py
+-rw-rw-rw-   0        0        0    13902 2023-05-21 18:41:51.000000 guacli-1.1.1/guacli/cli.py
+-rw-rw-rw-   0        0        0    12705 2023-05-21 19:07:30.000000 guacli-1.1.1/guacli/guacamoleClient.py
+drwxrwxrwx   0        0        0        0 2023-05-21 19:29:46.054745 guacli-1.1.1/guacli.egg-info/
+-rw-rw-rw-   0        0        0     1886 2023-05-21 19:29:46.000000 guacli-1.1.1/guacli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-21 19:29:46.000000 guacli-1.1.1/guacli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 19:29:46.000000 guacli-1.1.1/guacli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-21 19:29:46.000000 guacli-1.1.1/guacli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-05-21 19:29:46.000000 guacli-1.1.1/guacli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 19:29:46.054745 guacli-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      719 2022-11-30 20:02:13.000000 guacli-1.1.1/setup.py
```

### Comparing `guacli-1.1.0/LICENSE` & `guacli-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `guacli-1.1.0/PKG-INFO` & `guacli-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guacli
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python client (library and CLI) for Apache Guacamole front-end REST API.
 Home-page: https://github.com/chaimeleon-eu/guacamole-python-client
 Author: Pau Lozano
 Author-email: 
 License: Apache 2.0
 Keywords: cli client guacamole api
 Description-Content-Type: text/markdown
```

### Comparing `guacli-1.1.0/README.md` & `guacli-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `guacli-1.1.0/guacli/cli.py` & `guacli-1.1.1/guacli/cli.py`

 * *Files identical despite different names*

### Comparing `guacli-1.1.0/guacli/guacamoleClient.py` & `guacli-1.1.1/guacli/guacamoleClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             raise GuacError("Error setting permissions for the user", res, msg)
 
     def changeUserPermissions(self, userName, operation: PermissionsOperation, permission: SystemPermissions): 
         self._changeUserPermissions(userName, "/systemPermissions", operation.value, permission.value)
 
     def changeUserAccessToConnection(self, userName, operation: PermissionsOperation, connectionId):
         self._changeUserPermissions(userName, "/connectionPermissions/"+connectionId, operation.value, ConnectionPermissions.READ.value)
-        
+
     def createConnectionGroup(self, connectionGroupName):
         newConnectionGroup = {
             "parentIdentifier": "ROOT",
             "name": connectionGroupName,
             "type": "ORGANIZATIONAL",
             "attributes":{
                 "max-connections":"",
@@ -243,14 +243,16 @@
         headers = {'Content-Type': 'application/json;charset=UTF-8'}
         self.connection.request("POST", self.path+"api/session/data/postgresql/connections?token="+self.token, payload, headers)
         res = self.connection.getresponse()
         httpStatusCode = res.status
         msg = res.read()  # whole response must be readed in order to do more requests using the same connection
         if httpStatusCode != 200:
             raise GuacError("Error creating the connection", res, msg)
+        response = json.loads(msg)
+        return str(response['identifier'])
 
     def getConnectionId(self, connectionName, connectionGroupId = "ROOT"):
         payload = ''
         headers = {}
         self.connection.request("GET", self.path+"api/session/data/postgresql/connectionGroups/"+connectionGroupId+"/tree?token="+self.token, payload, headers)
         res = self.connection.getresponse()
         httpStatusCode = res.status
```

### Comparing `guacli-1.1.0/guacli.egg-info/PKG-INFO` & `guacli-1.1.1/guacli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guacli
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python client (library and CLI) for Apache Guacamole front-end REST API.
 Home-page: https://github.com/chaimeleon-eu/guacamole-python-client
 Author: Pau Lozano
 Author-email: 
 License: Apache 2.0
 Keywords: cli client guacamole api
 Description-Content-Type: text/markdown
```

### Comparing `guacli-1.1.0/setup.py` & `guacli-1.1.1/setup.py`

 * *Files identical despite different names*

