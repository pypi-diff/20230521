# Comparing `tmp/guacli-1.0.3.tar.gz` & `tmp/guacli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guacli-1.0.3.tar", last modified: Wed Feb  1 11:27:51 2023, max compression
+gzip compressed data, was "guacli-1.1.0.tar", last modified: Sun May 21 18:43:23 2023, max compression
```

## Comparing `guacli-1.0.3.tar` & `guacli-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-01 11:27:51.279850 guacli-1.0.3/
--rw-rw-rw-   0        0        0    11357 2022-11-14 15:57:40.000000 guacli-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1886 2023-02-01 11:27:51.279850 guacli-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1434 2023-02-01 11:22:42.000000 guacli-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-01 11:27:51.264105 guacli-1.0.3/guacli/
--rw-rw-rw-   0        0        0       23 2023-02-01 11:06:53.000000 guacli-1.0.3/guacli/__init__.py
--rw-rw-rw-   0        0        0    13621 2023-02-01 10:49:16.000000 guacli-1.0.3/guacli/cli.py
--rw-rw-rw-   0        0        0    11902 2023-02-01 10:28:35.000000 guacli-1.0.3/guacli/guacamoleClient.py
-drwxrwxrwx   0        0        0        0 2023-02-01 11:27:51.274968 guacli-1.0.3/guacli.egg-info/
--rw-rw-rw-   0        0        0     1886 2023-02-01 11:27:51.000000 guacli-1.0.3/guacli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-02-01 11:27:51.000000 guacli-1.0.3/guacli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-01 11:27:51.000000 guacli-1.0.3/guacli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-02-01 11:27:51.000000 guacli-1.0.3/guacli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-02-01 11:27:51.000000 guacli-1.0.3/guacli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-01 11:27:51.280492 guacli-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      719 2022-11-30 20:02:13.000000 guacli-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 18:43:23.545627 guacli-1.1.0/
+-rw-rw-rw-   0        0        0    11357 2022-11-14 15:57:40.000000 guacli-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1886 2023-05-21 18:43:23.545627 guacli-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1434 2023-02-01 11:22:42.000000 guacli-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 18:43:23.535733 guacli-1.1.0/guacli/
+-rw-rw-rw-   0        0        0       23 2023-05-21 17:05:49.000000 guacli-1.1.0/guacli/__init__.py
+-rw-rw-rw-   0        0        0    13902 2023-05-21 18:41:51.000000 guacli-1.1.0/guacli/cli.py
+-rw-rw-rw-   0        0        0    12635 2023-05-21 18:25:39.000000 guacli-1.1.0/guacli/guacamoleClient.py
+drwxrwxrwx   0        0        0        0 2023-05-21 18:43:23.545627 guacli-1.1.0/guacli.egg-info/
+-rw-rw-rw-   0        0        0     1886 2023-05-21 18:43:23.000000 guacli-1.1.0/guacli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-21 18:43:23.000000 guacli-1.1.0/guacli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 18:43:23.000000 guacli-1.1.0/guacli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-21 18:43:23.000000 guacli-1.1.0/guacli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-05-21 18:43:23.000000 guacli-1.1.0/guacli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 18:43:23.545627 guacli-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      719 2022-11-30 20:02:13.000000 guacli-1.1.0/setup.py
```

### Comparing `guacli-1.0.3/LICENSE` & `guacli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `guacli-1.0.3/PKG-INFO` & `guacli-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guacli
-Version: 1.0.3
+Version: 1.1.0
 Summary: Python client (library and CLI) for Apache Guacamole front-end REST API.
 Home-page: https://github.com/chaimeleon-eu/guacamole-python-client
 Author: Pau Lozano
 Author-email: 
 License: Apache 2.0
 Keywords: cli client guacamole api
 Description-Content-Type: text/markdown
```

### Comparing `guacli-1.0.3/README.md` & `guacli-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `guacli-1.0.3/guacli/cli.py` & `guacli-1.1.0/guacli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,59 +18,59 @@
         epilog='Example of use: \n'
             + os.path.basename(__file__)+' --url "https://example.com/guacamole" --user guacadmin create user james-smith')
     create_user_parser.add_argument('NEW_USER_NAME', type=str, help='Name of the user to create')
     create_user_parser.add_argument('--new-user-password', type=str, default='..........', 
                                     help='Password for the user to create. (if this parameter is not set, it will be interactively asked)')
     create_user_parser.add_argument('--can-create-connections', action='store_true', help='The user will be able to create connections.')
 
-def create_user_and_private_connection_group(client, args, newUserPassword):
+def create_user_and_private_connection_group(client: guac.GuacamoleClient, args, newUserPassword):
     newUserName = args.NEW_USER_NAME
     # if client.existsUser(newUserName):
     #     print('The user '+newUserName+' already exists. Changing the password')
-    #     client.changePasswordToUser(newUserName, newUserPassword)
+    #     client.changeUserPassword(newUserName, newUserPassword)
     # else:
     print('Creating user: '+newUserName)
     client.createUser(newUserName, newUserPassword)
     
     if args.can_create_connections:
         print('Adding permission to create connections')
-        client.changePermissionToUser(newUserName, 'add', 'CREATE_CONNECTION')
+        client.changeUserPermissions(newUserName, guac.PermissionsOperation.ADD, guac.SystemPermissions.CREATE_CONNECTION)
         
     ret = client.existsConnectionGroup(newUserName)
     if ret: 
         print('The connection group for the user already exists.')
         exit(code=7)
     
     #NOTE: The connection group must be created by the user because only the creator (or an admin) can create connections in the group. 
     #      If a connection group is created by an admin, only admins will be able to create connections in it.
 
     print('Adding permission to create connection groups to the user')
-    client.changePermissionToUser(newUserName, 'add', 'CREATE_CONNECTION_GROUP')
+    client.changeUserPermissions(newUserName, guac.PermissionsOperation.ADD, guac.SystemPermissions.CREATE_CONNECTION_GROUP)
     
     adminToken = client.token   # save admin token
     print('Login with the user... ', end='')
     client.login(newUserName, newUserPassword)
     print('OK.')
     
     print('Creating connection group: '+newUserName)
     client.createConnectionGroup(newUserName)
     
     print('Removing permission to create connection groups')
     client.token = adminToken     # restore admin token
-    client.changePermissionToUser(newUserName, 'remove', 'CREATE_CONNECTION_GROUP')
+    client.changeUserPermissions(newUserName, guac.PermissionsOperation.REMOVE, guac.SystemPermissions.CREATE_CONNECTION_GROUP)
     
 
 def delete_user_parser(create_subparsers):
     create_user_parser = create_subparsers.add_parser('user', help='Deletes a user.', 
         description='This operation deletes a user in guacamole database and the private connection group with the same name of the user.',
         epilog='Example of use: \n'
             + os.path.basename(__file__)+' --url "https://example.com/guacamole" --user guacadmin delete user james-smith')
     create_user_parser.add_argument('USER_TO_DELETE', type=str, help='Name of the user to delete')
 
-def delete_user_and_private_connection_group(client, args):
+def delete_user_and_private_connection_group(client: guac.GuacamoleClient, args):
     userToDelete = args.USER_TO_DELETE
     print('Deleting user: '+userToDelete)
     client.deleteUser(userToDelete)
     
     ret = client.getConnectionGroupId(userToDelete)
     if ret is None: 
         print('Connection group "'+userToDelete+'" not found.')
@@ -105,15 +105,15 @@
                                               +'If sftp-user provided, the password for the VNC service will be used also for sftp.')
     create_connection_parser.add_argument('--sftp-disable-file-uploads', action='store_true')
     create_connection_parser.add_argument('--sftp-disable-file-downloads', action='store_true')
 
     create_connection_parser.add_argument('--disable-clipboard-copy', action='store_true', help='Disable copy from the remote clipboard.')
     create_connection_parser.add_argument('--disable-clipboard-paste', action='store_true', help='Disable paste into the remote clipboard.')
 
-def create_connection(client, args):
+def create_connection(client: guac.GuacamoleClient, args):
     if args.connection_group != None:
         ret = client.getConnectionGroupId(args.connection_group)
         if ret is None: 
             print('Connection group "'+args.connection_group+'" not found.')
             exit(code=2)
         print('The ID of connection group "'+args.connection_group+'" is '+ret+'.')
         connectionGroupId = ret
@@ -145,15 +145,15 @@
                 + os.path.basename(__file__)+' --url "https://example.com/guacamole" --user guacadmin delete connection some-connection')
     create_connection_parser.add_argument('CONNECTION_NAME', type=str, 
                                           help='Name of the connection to delete.')
     create_connection_parser.add_argument('--connection-group', type=str, default=None, 
                                           help='Optional name of the conection group where the connection is. '
                                               +'If not provided, it will be deleted from the root group.')
     
-def delete_connection(client, args):
+def delete_connection(client: guac.GuacamoleClient, args):
     if args.connection_group != None:
         ret = client.getConnectionGroupId(args.connection_group)
         if ret is None: 
             print('Connection group "'+args.connection_group+'" not found.')
             exit(code=2)
         print('Id of connection group "'+args.connection_group+'" is '+ret+'.')
         connectionGroupId = ret
@@ -203,14 +203,15 @@
     parser.add_argument('--debug', action='store_true', help='Write debug details in the standard output')
 
     args = parser.parse_args()
     DEBUG = args.debug
     
     # Parse Common arguments
     url = urllib.parse.urlparse(args.url)
+    if url.hostname is None: print('Wrong url.'); exit(code=1)
     port = url.port
     if url.scheme == 'http':
         if port == None: port = 80
         connection = http.client.HTTPConnection(url.hostname, port) 
     else:
         if port == None: port = 443
         connection = http.client.HTTPSConnection(url.hostname, port)
```

### Comparing `guacli-1.0.3/guacli/guacamoleClient.py` & `guacli-1.1.0/guacli/guacamoleClient.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 #!/usr/bin/python
 
 import json
 import urllib.parse
 import http.client
+from enum import Enum
 
 DEBUG = False
 
 class GuacError(Exception):
     def __init__(self, short_msg, http_response, msg):
         super().__init__('%s. httpCode: %d %s' % (short_msg, http_response.status, http_response.reason) + '\n' + msg.decode())
 
+class PermissionsOperation(Enum):
+    ADD = "add"
+    REMOVE = "remove"
+
+class SystemPermissions(Enum):
+    CREATE_CONNECTION = "CREATE_CONNECTION"
+    CREATE_CONNECTION_GROUP = "CREATE_CONNECTION_GROUP"
+
+class ConnectionPermissions(Enum):
+    READ = "READ"
+
+
 class GuacamoleClient:
 
     def __init__(self, connection: "http.client.HTTPConnection | http.client.HTTPSConnection", path: str):
         self.connection = connection
         if not path.endswith('/'): path += '/'
         self.path = path
         self.token = ''
@@ -90,15 +103,15 @@
         self.connection.request("DELETE", self.path+"api/session/data/postgresql/users/"+userName+"?token="+self.token, payload, headers)
         res = self.connection.getresponse()
         httpStatusCode = res.status
         msg = res.read()  # whole response must be readed in order to do more requests using the same connection
         if httpStatusCode != 204:
             raise GuacError("Error deleting the user", res, msg)
 
-    def changePasswordToUser(self, userName, password):
+    def changeUserPassword(self, userName, password):
         user = {
             "username": userName,
             "password": password,
             "attributes": {
                 # "guac-email-address":None,
                 # "guac-organizational-role":None,
                 # "guac-full-name":None,
@@ -119,14 +132,32 @@
         self.connection.request("PUT", self.path+"api/session/data/postgresql/users/"+userName+"?token="+self.token, payload, headers)
         res = self.connection.getresponse()
         httpStatusCode = res.status
         msg = res.read()  # whole response must be readed in order to do more requests using the same connection
         if httpStatusCode != 204:
             raise GuacError("Error modifying the user", res, msg)
             
+    def _changeUserPermissions(self, userName: str, path: str, operation: str, permission: str):
+        permissions = [{"op": operation, "path": path, "value": permission }]
+        payload = json.dumps(permissions)
+        if DEBUG: print(payload)
+        headers = {'Content-Type': 'application/json;charset=UTF-8'}
+        self.connection.request("PATCH", self.path+"api/session/data/postgresql/users/"+userName+"/permissions?token="+self.token, payload, headers)
+        res = self.connection.getresponse()
+        httpStatusCode = res.status
+        msg = res.read()  # whole response must be readed in order to do more requests using the same connection
+        if httpStatusCode != 204:
+            raise GuacError("Error setting permissions for the user", res, msg)
+
+    def changeUserPermissions(self, userName, operation: PermissionsOperation, permission: SystemPermissions): 
+        self._changeUserPermissions(userName, "/systemPermissions", operation.value, permission.value)
+
+    def changeUserAccessToConnection(self, userName, operation: PermissionsOperation, connectionId):
+        self._changeUserPermissions(userName, "/connectionPermissions/"+connectionId, operation.value, ConnectionPermissions.READ.value)
+        
     def createConnectionGroup(self, connectionGroupName):
         newConnectionGroup = {
             "parentIdentifier": "ROOT",
             "name": connectionGroupName,
             "type": "ORGANIZATIONAL",
             "attributes":{
                 "max-connections":"",
@@ -150,26 +181,14 @@
         self.connection.request("DELETE", self.path+"api/session/data/postgresql/connectionGroups/"+connectionGroupId+"?token="+self.token, payload, headers)
         res = self.connection.getresponse()
         httpStatusCode = res.status
         msg = res.read()  # whole response must be readed in order to do more requests using the same connection
         if httpStatusCode != 204:
             raise GuacError("Error deleting the connection group", res, msg)
             
-    def changePermissionToUser(self, userName, operation, permissionName): 
-        permissions = [{"op": operation, "path":"/systemPermissions", "value": permissionName }]
-        payload = json.dumps(permissions)
-        if DEBUG: print(payload)
-        headers = {'Content-Type': 'application/json;charset=UTF-8'}
-        self.connection.request("PATCH", self.path+"api/session/data/postgresql/users/"+userName+"/permissions?token="+self.token, payload, headers)
-        res = self.connection.getresponse()
-        httpStatusCode = res.status
-        msg = res.read()  # whole response must be readed in order to do more requests using the same connection
-        if httpStatusCode != 204:
-            raise GuacError("Error setting permissions for the user", res, msg)
-            
     def createVncConnection(self, connectionName, connectionGroupId, guacd_hostname, vnc_host, vnc_port, vnc_password, 
                             sftp_user = None, sftp_password = None, sftp_port = "22", sftp_disable_download = False, sftp_disable_upload = False,
                             disable_clipboard_copy = False, disable_clipboard_paste = False):
         newConnection = {
             "name": connectionName,
             "parentIdentifier": connectionGroupId,
             "protocol": "vnc",
```

### Comparing `guacli-1.0.3/guacli.egg-info/PKG-INFO` & `guacli-1.1.0/guacli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guacli
-Version: 1.0.3
+Version: 1.1.0
 Summary: Python client (library and CLI) for Apache Guacamole front-end REST API.
 Home-page: https://github.com/chaimeleon-eu/guacamole-python-client
 Author: Pau Lozano
 Author-email: 
 License: Apache 2.0
 Keywords: cli client guacamole api
 Description-Content-Type: text/markdown
```

### Comparing `guacli-1.0.3/setup.py` & `guacli-1.1.0/setup.py`

 * *Files identical despite different names*

