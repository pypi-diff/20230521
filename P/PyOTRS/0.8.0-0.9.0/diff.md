# Comparing `tmp/PyOTRS-0.8.0.tar.gz` & `tmp/PyOTRS-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyOTRS-0.8.0.tar", last modified: Fri Apr 17 11:21:16 2020, max compression
+gzip compressed data, was "dist/PyOTRS-0.9.0.tar", last modified: Thu Apr 23 21:35:13 2020, max compression
```

## Comparing `PyOTRS-0.8.0.tar` & `PyOTRS-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-17 11:21:16.000000 PyOTRS-0.8.0/
--rw-rw-r--   0 robbie    (1000) robbie    (1000)      131 2020-04-17 11:21:16.000000 PyOTRS-0.8.0/setup.cfg
--rw-rw-r--   0 robbie    (1000) robbie    (1000)      235 2017-07-12 19:07:34.000000 PyOTRS-0.8.0/MANIFEST.in
-drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-17 11:21:16.000000 PyOTRS-0.8.0/webservices_templates/
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     2154 2017-03-04 20:30:10.000000 PyOTRS-0.8.0/webservices_templates/GenericLinkConnectorREST.yml
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     1739 2017-03-04 20:30:10.000000 PyOTRS-0.8.0/webservices_templates/GenericTicketConnectorREST.yml
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     1338 2017-03-04 21:03:17.000000 PyOTRS-0.8.0/webservices_templates/GenericFAQConnectorREST.yml
--rw-rw-r--   0 robbie    (1000) robbie    (1000)    16295 2020-04-17 11:21:16.000000 PyOTRS-0.8.0/PKG-INFO
-drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-17 11:21:16.000000 PyOTRS-0.8.0/pyotrs/
--rw-rw-r--   0 robbie    (1000) robbie    (1000)      273 2020-04-17 11:16:56.000000 PyOTRS-0.8.0/pyotrs/version.py
--rw-rw-r--   0 robbie    (1000) robbie    (1000)    70849 2020-04-06 11:16:28.000000 PyOTRS-0.8.0/pyotrs/lib.py
--rw-rw-r--   0 robbie    (1000) robbie    (1000)      690 2020-03-12 20:20:18.000000 PyOTRS-0.8.0/pyotrs/__init__.py
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     2132 2020-04-17 11:19:49.000000 PyOTRS-0.8.0/setup.py
--rw-rw-r--   0 robbie    (1000) robbie    (1000)    11093 2020-04-06 11:17:23.000000 PyOTRS-0.8.0/README.rst
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     1088 2020-04-06 11:16:28.000000 PyOTRS-0.8.0/LICENSE
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     3534 2020-04-17 11:16:46.000000 PyOTRS-0.8.0/CHANGELOG.rst
-drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-17 11:21:16.000000 PyOTRS-0.8.0/PyOTRS.egg-info/
--rw-rw-r--   0 robbie    (1000) robbie    (1000)    16295 2020-04-17 11:21:16.000000 PyOTRS-0.8.0/PyOTRS.egg-info/PKG-INFO
--rw-rw-r--   0 robbie    (1000) robbie    (1000)        1 2020-04-17 11:21:16.000000 PyOTRS-0.8.0/PyOTRS.egg-info/dependency_links.txt
--rw-rw-r--   0 robbie    (1000) robbie    (1000)       11 2020-04-17 11:21:16.000000 PyOTRS-0.8.0/PyOTRS.egg-info/top_level.txt
--rw-rw-r--   0 robbie    (1000) robbie    (1000)      509 2020-04-17 11:21:16.000000 PyOTRS-0.8.0/PyOTRS.egg-info/SOURCES.txt
--rw-rw-r--   0 robbie    (1000) robbie    (1000)        1 2017-10-03 11:22:46.000000 PyOTRS-0.8.0/PyOTRS.egg-info/not-zip-safe
--rw-rw-r--   0 robbie    (1000) robbie    (1000)       43 2020-04-17 11:21:16.000000 PyOTRS-0.8.0/PyOTRS.egg-info/requires.txt
--rw-rw-r--   0 robbie    (1000) robbie    (1000)       61 2020-04-17 11:21:16.000000 PyOTRS-0.8.0/PyOTRS.egg-info/entry_points.txt
-drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-17 11:21:16.000000 PyOTRS-0.8.0/cli/
--rw-rw-r--   0 robbie    (1000) robbie    (1000)     5188 2017-05-23 18:12:06.000000 PyOTRS-0.8.0/cli/PyOTRS.py
--rw-rw-r--   0 robbie    (1000) robbie    (1000)        0 2016-04-16 20:46:18.000000 PyOTRS-0.8.0/cli/__init__.py
+drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)      131 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/setup.cfg
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)      235 2017-07-12 19:07:34.000000 PyOTRS-0.9.0/MANIFEST.in
+drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/webservices_templates/
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)     2154 2017-03-04 20:30:10.000000 PyOTRS-0.9.0/webservices_templates/GenericLinkConnectorREST.yml
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)     1745 2020-04-23 20:54:54.000000 PyOTRS-0.9.0/webservices_templates/GenericTicketConnectorREST.yml
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)     1338 2017-03-04 21:03:17.000000 PyOTRS-0.9.0/webservices_templates/GenericFAQConnectorREST.yml
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)    17191 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/PKG-INFO
+drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/pyotrs/
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)      273 2020-04-23 21:07:39.000000 PyOTRS-0.9.0/pyotrs/version.py
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)    71254 2020-04-23 20:54:54.000000 PyOTRS-0.9.0/pyotrs/lib.py
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)      690 2020-03-12 20:20:18.000000 PyOTRS-0.9.0/pyotrs/__init__.py
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)     2052 2020-04-17 15:35:36.000000 PyOTRS-0.9.0/setup.py
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)    11787 2020-04-23 21:21:51.000000 PyOTRS-0.9.0/README.rst
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)     1088 2020-04-06 11:16:28.000000 PyOTRS-0.9.0/LICENSE
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)     3633 2020-04-23 21:07:39.000000 PyOTRS-0.9.0/CHANGELOG.rst
+drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/PyOTRS.egg-info/
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)    17191 2020-04-23 21:35:12.000000 PyOTRS-0.9.0/PyOTRS.egg-info/PKG-INFO
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)        1 2020-04-23 21:35:12.000000 PyOTRS-0.9.0/PyOTRS.egg-info/dependency_links.txt
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)       11 2020-04-23 21:35:12.000000 PyOTRS-0.9.0/PyOTRS.egg-info/top_level.txt
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)      509 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/PyOTRS.egg-info/SOURCES.txt
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)        1 2020-04-23 19:25:53.000000 PyOTRS-0.9.0/PyOTRS.egg-info/not-zip-safe
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)       43 2020-04-23 21:35:12.000000 PyOTRS-0.9.0/PyOTRS.egg-info/requires.txt
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)       61 2020-04-23 21:35:12.000000 PyOTRS-0.9.0/PyOTRS.egg-info/entry_points.txt
+drwxrwxr-x   0 robbie    (1000) robbie    (1000)        0 2020-04-23 21:35:13.000000 PyOTRS-0.9.0/cli/
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)     5331 2020-04-17 15:35:36.000000 PyOTRS-0.9.0/cli/PyOTRS.py
+-rw-rw-r--   0 robbie    (1000) robbie    (1000)        0 2016-04-16 20:46:18.000000 PyOTRS-0.9.0/cli/__init__.py
```

### Comparing `PyOTRS-0.8.0/webservices_templates/GenericLinkConnectorREST.yml` & `PyOTRS-0.9.0/webservices_templates/GenericLinkConnectorREST.yml`

 * *Files identical despite different names*

### Comparing `PyOTRS-0.8.0/webservices_templates/GenericTicketConnectorREST.yml` & `PyOTRS-0.9.0/webservices_templates/GenericTicketConnectorREST.yml`

 * *Files 1% similar despite different names*

```diff
@@ -55,19 +55,18 @@
           Route: /Ticket/:TicketID
         TicketGetList:
           RequestMethod:
           - GET
           Route: /TicketList
         TicketSearch:
           RequestMethod:
-          - GET
-          Route: /Ticket
+          - POST
+          Route: /TicketSearch
         TicketUpdate:
           RequestMethod:
           - PATCH
           Route: /Ticket/:TicketID
     Type: HTTP::REST
 RemoteSystem: ''
 Requester:
   Transport:
     Type: ''
-
```

### Comparing `PyOTRS-0.8.0/webservices_templates/GenericFAQConnectorREST.yml` & `PyOTRS-0.9.0/webservices_templates/GenericFAQConnectorREST.yml`

 * *Files identical despite different names*

### Comparing `PyOTRS-0.8.0/PKG-INFO` & `PyOTRS-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOTRS
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python wrapper for OTRS (using REST API)
 Home-page: https://gitlab.com/rhab/PyOTRS
 Author: Robert Habermann
 Author-email: mail@rhab.de
 Maintainer: Robert Habermann
 License: The MIT License (MIT)
 
@@ -54,32 +54,40 @@
             :target: https://gitlab.com/rhab/PyOTRS/-/blob/master/LICENSE
             :alt: MIT licensed
         
         .. |PythonVersions| image:: https://img.shields.io/badge/python-2.7%2C%203.4%2C%203.5%2C%203.6%2C%203.7%2C%203.8-blue.svg
             :alt: python: 2.7, 3.4, 3.5, 3.6, 3.7, 3.8
         
         
-        PyOTRS is a Python wrapper for accessing `OTRS <https://www.otrs.com/>`_ (Version 5, 6, 7 or 8) using the
+        PyOTRS is a Python wrapper for accessing `OTRS <https://www.otrs.com/>`_ (Version 5, 6, 7) using the
         (GenericInterface) REST API.
         
         Warning
         =======
         
-            Please upgrade PyOTRS to atleast version 0.7.1 if you are using OTRS 6.0.27, 7.0.16 or
-            newer. See `issue 27 <https://gitlab.com/rhab/PyOTRS/-/issues/27>`_ for more details.
+            Please upgrade PyOTRS to at least version 0.7.1 if you are using OTRS 6.0.27, 7.0.16 or
+            newer. See `issue 27 <https://gitlab.com/rhab/PyOTRS/-/issues/27>`_ and
+            `issue 29 <https://gitlab.com/rhab/PyOTRS/-/issues/29>`_ for more details.
+        
+            OTRS has introduced a new API in version 8 and with this also changed the API endpoint from
+            "Session::SessionCreate" to "AccessToken::Create". At the moment PyOTRS does not support
+            OTRS v8. See `issue 28 <https://gitlab.com/rhab/PyOTRS/-/issues/28>`_ for progress and
+            discussions.
+        
         
         Features
         ========
         
         Access an OTRS instance to::
         
             * create a new Ticket
             * get the data of a specific Ticket
             * search for Tickets
             * update existing Tickets
+            * access as a "Customer User"
         
         Some of the most notable methods provided are::
         
             * Client.session_create (Use credentials to "log in")
             * Client.ticket_create
             * Client.ticket_get_by_list  (takes a list)
             * Client.ticket_get_by_id  (takes an int)
@@ -103,16 +111,18 @@
         ------------
         
         *Dependencies are installed automatically*
         
         pip::
         
             - python-requests
-            - click (for PyOTRS Shell CLI)
-            - colorama (for colors in PyOTRS Shell CLI)
+        
+        
+        There also is a (completely optional and rudimentary) *interactive* CLI which requires `click`. This
+        dependency can be installed by calling `pip install PyOTRS[cli]`.
         
         Install
         -------
         
         install::
         
             pip install PyOTRS
@@ -140,29 +150,38 @@
         More Examples
         -------------
         
         - instantiate a ``Client`` object called **client**
         - create a session ("login") on **client**
         - get the ``Ticket`` with ID 1
         
-        >>> from pyotrs import Article, Client, Ticket
+        >>> from pyotrs import Article, Client, DynamicField, Ticket
         >>> client = Client("http://otrs.example.com", "root@localhost", "password")
         >>> client.session_create()
         True
         
         >>> my_ticket = client.ticket_get_by_id(1)
         >>> my_ticket
         <Ticket: 1>
         
         >>> my_ticket.field_get("TicketNumber")
         u'2010080210123456'
         >>> my_ticket.field_get("Title")
         u'Welcome to OTRS!'
         >>> my_ticket.to_dct()  # Show complete ticket
         
+        
+        - access as a CustomerUser
+        
+        >>> from pyotrs import Client
+        >>> client = Client("http://otrs.example.com", "user@customer.example.com", "password", customer_user=True)
+        >>> client.session_create()
+        True
+        
+        
         - add an ``Article`` to ``Ticket`` with ID 1
         
         >>> my_article = Article({"Subject": "Subj", "Body": "New Body"})
         >>> client.ticket_update(1, article=my_article)
         {u'ArticleID': u'3',
          u'TicketID': u'1',
          u'TicketNumber': u'2010080210123456'}
@@ -249,15 +268,15 @@
         
         Search for Tickets
         ------------------
         
         - get list of Tickets created before a date (e.g. Jan 01, 2011)
         
         >>> from datetime import datetime
-        >>> client.ticket_search(TicketCreateTimeOlderDate=datetime(2011, 01, 01))
+        >>> client.ticket_search(TicketCreateTimeOlderDate=datetime(2011, 1, 1))
         [u'1']
         
         
         - get list of Tickets created less than a certain time ago (e.g. younger than 1 week)
         
         >>> from datetime import datetime
         >>> from datetime import timedelta
@@ -420,13 +439,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Documentation :: Sphinx
 Provides-Extra: cli
```

### Comparing `PyOTRS-0.8.0/pyotrs/lib.py` & `PyOTRS-0.9.0/pyotrs/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -805,15 +805,15 @@
         # TODO 2016-04-23 (RH): check this
         if not SessionStore._validate_file_owner_and_permissions(self.file_path):
             raise IOError("Race condition: Something happened to file during the run!")
 
         return True
 
     def delete(self):
-        """remove session id file (e.g. when it only contains an invalid session id
+        """remove session id file (e.g. when it only contains an invalid session id)
 
         Raises:
             NotImplementedError
 
         Returns:
             **bool**: **True** if successful, otherwise **False**.
 
@@ -841,15 +841,15 @@
             return False
 
         if not file_lstat.st_mode & 0o777 == 384:
             """ check for unix permission User R+W only (0600)
             >>> oct(384)
             '0600' Python 2
             >>> oct(384)
-            '0o600'  Python 3  """
+            '0o600' Python 3  """
             return False
 
         return True
 
 
 class Client(object):
     """PyOTRS Client class - includes Session handling
@@ -869,14 +869,16 @@
             more information - default to no proxies
         https_verify (bool): Should HTTPS certificates be verified (defaults to True)
         ca_cert_bundle (str): file path - if specified overrides python/system default for
             Root CA bundle that will be used.
         auth (tuple): e.g. ("user", "pass") - see requests documentation ("auth") for details
         client_auth_cert (str): file path containing both certificate and key (unencrypted) in
             PEM format to use for TLS client authentication (passed to requests as "cert")
+        customer_user (bool): flag to indicate that the username is for a "CustomerUser"
+           (defaults to False)
         user_agent (str): optional HTTP UserAgent string
         webservice_path (str): OTRS REST Web Service Path part - defaults to
             "/otrs/nph-genericinterface.pl/Webservice/"
 
     """
 
     def __init__(self,
@@ -890,14 +892,15 @@
                  webservice_config_faq=None,
                  webservice_config_link=None,
                  proxies=None,
                  https_verify=True,
                  ca_cert_bundle=None,
                  auth=None,
                  client_auth_cert=None,
+                 customer_user=False,
                  user_agent=None,
                  webservice_path="/otrs/nph-genericinterface.pl/Webservice/"):
 
         if not baseurl:
             raise ArgumentMissingError("baseurl")
         self.baseurl = baseurl.rstrip("/")
         self.webservice_path = webservice_path
@@ -958,14 +961,16 @@
                 self.https_verify = ca_certs
         else:
             self.https_verify = False
 
         self.auth = auth
         self.client_auth_cert = client_auth_cert
 
+        self.customer_user = customer_user
+
         self.user_agent = user_agent
 
         # credentials
         self.username = username
         self.password = password
 
         # dummy initialization
@@ -980,15 +985,15 @@
         * session_restore_or_set_up_new  # try to get session_id from a (json) file on disc
     """
 
     def session_check_is_valid(self, session_id=None):
         """check whether session_id is currently valid
 
         Args:
-            session_id (str): optional If set overrides the self.session_id
+            session_id (str): optional if set overrides the self.session_id
 
         Raises:
             ArgumentMissingError: if session_id is not set
 
         Returns:
             **bool**: **True** if valid, otherwise **False**.
 
@@ -1017,18 +1022,24 @@
 
         .. note::
             Uses HTTP Method: POST
 
         """
         self.operation = "SessionCreate"
 
-        payload = {
-            "UserLogin": self.username,
-            "Password": self.password
-        }
+        if self.customer_user:
+            payload = {
+                "CustomerUserLogin": self.username,
+                "Password": self.password
+            }
+        else:
+            payload = {
+                "UserLogin": self.username,
+                "Password": self.password
+            }
 
         if not self._parse_and_validate_response(self._send_request(payload)):
             return False
 
         self.session_id_store.value = self.result_json['SessionID']
         return True
 
@@ -1055,15 +1066,16 @@
             # got one.. check whether it's still valid
             try:
                 if self.session_check_is_valid(self.session_id_store.value):
                     log.info("Using valid Session ID "
                              "from ({0})".format(self.session_id_store.file_path))
                     return True
             except APIError:
-                """most likely invalid session_id so pass. Remove clear session_id_store.."""
+                """Most likely invalid session_id. Remove it from session_id_store."""
+                pass
 
         # got no (valid) session_id; clean store
         self.session_id_store.write("")
 
         # and try to create new one
         if not self.session_create():
             raise SessionCreateError("Failed to create a Session ID!")
@@ -1959,15 +1971,15 @@
 
         Args:
             response (requests.Response): result of _send_request
 
         Raises:
             OTRSAPIError
             NotImplementedError
-            ResponseJSONParseError
+            ResponseParseError
 
         Returns:
             **bool**: **True** if successful
 
         """
 
         if not isinstance(response, requests.models.Response):
```

### Comparing `PyOTRS-0.8.0/pyotrs/__init__.py` & `PyOTRS-0.9.0/pyotrs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyOTRS-0.8.0/setup.py` & `PyOTRS-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,27 +24,23 @@
     include_package_data=True,
     zip_safe=False,
     license=LICENSE,
     install_requires=[
         'requests', 'deprecation',
     ],
     extras_require={
-    "cli": ['click', 'colorama'],
+        "cli": ['click', 'colorama'],
     },
     entry_points='''
         [console_scripts]
         pyotrs=cli.PyOTRS:cli
     ''',
     test_suite='unittest2.collector',
     tests_require=['tox', 'coverage', 'unittest2', 'mock', 'responses'],
     classifiers=[
-        # How mature is this project? Common values are
-        #   3 - Alpha
-        #   4 - Beta
-        #   5 - Production/Stable
         'Development Status :: 4 - Beta',
 
         'Environment :: Console',
         'Environment :: Web Environment',
 
         'Framework :: Pytest',
         'Framework :: Sphinx',
@@ -59,14 +55,15 @@
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
 
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
 
         'Topic :: Documentation :: Sphinx',
     ],
```

### Comparing `PyOTRS-0.8.0/README.rst` & `PyOTRS-0.9.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -24,32 +24,40 @@
     :target: https://gitlab.com/rhab/PyOTRS/-/blob/master/LICENSE
     :alt: MIT licensed
 
 .. |PythonVersions| image:: https://img.shields.io/badge/python-2.7%2C%203.4%2C%203.5%2C%203.6%2C%203.7%2C%203.8-blue.svg
     :alt: python: 2.7, 3.4, 3.5, 3.6, 3.7, 3.8
 
 
-PyOTRS is a Python wrapper for accessing `OTRS <https://www.otrs.com/>`_ (Version 5, 6, 7 or 8) using the
+PyOTRS is a Python wrapper for accessing `OTRS <https://www.otrs.com/>`_ (Version 5, 6, 7) using the
 (GenericInterface) REST API.
 
 Warning
 =======
 
-    Please upgrade PyOTRS to atleast version 0.7.1 if you are using OTRS 6.0.27, 7.0.16 or
-    newer. See `issue 27 <https://gitlab.com/rhab/PyOTRS/-/issues/27>`_ for more details.
+    Please upgrade PyOTRS to at least version 0.7.1 if you are using OTRS 6.0.27, 7.0.16 or
+    newer. See `issue 27 <https://gitlab.com/rhab/PyOTRS/-/issues/27>`_ and
+    `issue 29 <https://gitlab.com/rhab/PyOTRS/-/issues/29>`_ for more details.
+
+    OTRS has introduced a new API in version 8 and with this also changed the API endpoint from
+    "Session::SessionCreate" to "AccessToken::Create". At the moment PyOTRS does not support
+    OTRS v8. See `issue 28 <https://gitlab.com/rhab/PyOTRS/-/issues/28>`_ for progress and
+    discussions.
+
 
 Features
 ========
 
 Access an OTRS instance to::
 
     * create a new Ticket
     * get the data of a specific Ticket
     * search for Tickets
     * update existing Tickets
+    * access as a "Customer User"
 
 Some of the most notable methods provided are::
 
     * Client.session_create (Use credentials to "log in")
     * Client.ticket_create
     * Client.ticket_get_by_list  (takes a list)
     * Client.ticket_get_by_id  (takes an int)
@@ -73,16 +81,18 @@
 ------------
 
 *Dependencies are installed automatically*
 
 pip::
 
     - python-requests
-    - click (for PyOTRS Shell CLI)
-    - colorama (for colors in PyOTRS Shell CLI)
+
+
+There also is a (completely optional and rudimentary) *interactive* CLI which requires `click`. This
+dependency can be installed by calling `pip install PyOTRS[cli]`.
 
 Install
 -------
 
 install::
 
     pip install PyOTRS
@@ -110,29 +120,38 @@
 More Examples
 -------------
 
 - instantiate a ``Client`` object called **client**
 - create a session ("login") on **client**
 - get the ``Ticket`` with ID 1
 
->>> from pyotrs import Article, Client, Ticket
+>>> from pyotrs import Article, Client, DynamicField, Ticket
 >>> client = Client("http://otrs.example.com", "root@localhost", "password")
 >>> client.session_create()
 True
 
 >>> my_ticket = client.ticket_get_by_id(1)
 >>> my_ticket
 <Ticket: 1>
 
 >>> my_ticket.field_get("TicketNumber")
 u'2010080210123456'
 >>> my_ticket.field_get("Title")
 u'Welcome to OTRS!'
 >>> my_ticket.to_dct()  # Show complete ticket
 
+
+- access as a CustomerUser
+
+>>> from pyotrs import Client
+>>> client = Client("http://otrs.example.com", "user@customer.example.com", "password", customer_user=True)
+>>> client.session_create()
+True
+
+
 - add an ``Article`` to ``Ticket`` with ID 1
 
 >>> my_article = Article({"Subject": "Subj", "Body": "New Body"})
 >>> client.ticket_update(1, article=my_article)
 {u'ArticleID': u'3',
  u'TicketID': u'1',
  u'TicketNumber': u'2010080210123456'}
@@ -219,15 +238,15 @@
 
 Search for Tickets
 ------------------
 
 - get list of Tickets created before a date (e.g. Jan 01, 2011)
 
 >>> from datetime import datetime
->>> client.ticket_search(TicketCreateTimeOlderDate=datetime(2011, 01, 01))
+>>> client.ticket_search(TicketCreateTimeOlderDate=datetime(2011, 1, 1))
 [u'1']
 
 
 - get list of Tickets created less than a certain time ago (e.g. younger than 1 week)
 
 >>> from datetime import datetime
 >>> from datetime import timedelta
```

### Comparing `PyOTRS-0.8.0/LICENSE` & `PyOTRS-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOTRS-0.8.0/CHANGELOG.rst` & `PyOTRS-0.9.0/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Change Log
 ==========
 
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/).
 
-0.9.x - 2020-xx-yy (unreleased)
--------------------------------
+0.10.x - 2020-xx-yy (unreleased)
+--------------------------------
+
+0.9.0 - 2020-04-23
+------------------
+
+- add: implement !23 (fix #31) adding support for CustomerUser
 
 
 0.8.0 - 2020-04-17
 ------------------
 
-- fix # : remove click and colorama from core dependencies
+- remove:  click and colorama from core dependencies
 
 0.7.1 - 2020-04-06
 ------------------
 
 - fix #27: GET must not contain a body (OTRS: #14203)
 
 0.6.0 - 2020-03-13
```

### Comparing `PyOTRS-0.8.0/PyOTRS.egg-info/PKG-INFO` & `PyOTRS-0.9.0/PyOTRS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOTRS
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python wrapper for OTRS (using REST API)
 Home-page: https://gitlab.com/rhab/PyOTRS
 Author: Robert Habermann
 Author-email: mail@rhab.de
 Maintainer: Robert Habermann
 License: The MIT License (MIT)
 
@@ -54,32 +54,40 @@
             :target: https://gitlab.com/rhab/PyOTRS/-/blob/master/LICENSE
             :alt: MIT licensed
         
         .. |PythonVersions| image:: https://img.shields.io/badge/python-2.7%2C%203.4%2C%203.5%2C%203.6%2C%203.7%2C%203.8-blue.svg
             :alt: python: 2.7, 3.4, 3.5, 3.6, 3.7, 3.8
         
         
-        PyOTRS is a Python wrapper for accessing `OTRS <https://www.otrs.com/>`_ (Version 5, 6, 7 or 8) using the
+        PyOTRS is a Python wrapper for accessing `OTRS <https://www.otrs.com/>`_ (Version 5, 6, 7) using the
         (GenericInterface) REST API.
         
         Warning
         =======
         
-            Please upgrade PyOTRS to atleast version 0.7.1 if you are using OTRS 6.0.27, 7.0.16 or
-            newer. See `issue 27 <https://gitlab.com/rhab/PyOTRS/-/issues/27>`_ for more details.
+            Please upgrade PyOTRS to at least version 0.7.1 if you are using OTRS 6.0.27, 7.0.16 or
+            newer. See `issue 27 <https://gitlab.com/rhab/PyOTRS/-/issues/27>`_ and
+            `issue 29 <https://gitlab.com/rhab/PyOTRS/-/issues/29>`_ for more details.
+        
+            OTRS has introduced a new API in version 8 and with this also changed the API endpoint from
+            "Session::SessionCreate" to "AccessToken::Create". At the moment PyOTRS does not support
+            OTRS v8. See `issue 28 <https://gitlab.com/rhab/PyOTRS/-/issues/28>`_ for progress and
+            discussions.
+        
         
         Features
         ========
         
         Access an OTRS instance to::
         
             * create a new Ticket
             * get the data of a specific Ticket
             * search for Tickets
             * update existing Tickets
+            * access as a "Customer User"
         
         Some of the most notable methods provided are::
         
             * Client.session_create (Use credentials to "log in")
             * Client.ticket_create
             * Client.ticket_get_by_list  (takes a list)
             * Client.ticket_get_by_id  (takes an int)
@@ -103,16 +111,18 @@
         ------------
         
         *Dependencies are installed automatically*
         
         pip::
         
             - python-requests
-            - click (for PyOTRS Shell CLI)
-            - colorama (for colors in PyOTRS Shell CLI)
+        
+        
+        There also is a (completely optional and rudimentary) *interactive* CLI which requires `click`. This
+        dependency can be installed by calling `pip install PyOTRS[cli]`.
         
         Install
         -------
         
         install::
         
             pip install PyOTRS
@@ -140,29 +150,38 @@
         More Examples
         -------------
         
         - instantiate a ``Client`` object called **client**
         - create a session ("login") on **client**
         - get the ``Ticket`` with ID 1
         
-        >>> from pyotrs import Article, Client, Ticket
+        >>> from pyotrs import Article, Client, DynamicField, Ticket
         >>> client = Client("http://otrs.example.com", "root@localhost", "password")
         >>> client.session_create()
         True
         
         >>> my_ticket = client.ticket_get_by_id(1)
         >>> my_ticket
         <Ticket: 1>
         
         >>> my_ticket.field_get("TicketNumber")
         u'2010080210123456'
         >>> my_ticket.field_get("Title")
         u'Welcome to OTRS!'
         >>> my_ticket.to_dct()  # Show complete ticket
         
+        
+        - access as a CustomerUser
+        
+        >>> from pyotrs import Client
+        >>> client = Client("http://otrs.example.com", "user@customer.example.com", "password", customer_user=True)
+        >>> client.session_create()
+        True
+        
+        
         - add an ``Article`` to ``Ticket`` with ID 1
         
         >>> my_article = Article({"Subject": "Subj", "Body": "New Body"})
         >>> client.ticket_update(1, article=my_article)
         {u'ArticleID': u'3',
          u'TicketID': u'1',
          u'TicketNumber': u'2010080210123456'}
@@ -249,15 +268,15 @@
         
         Search for Tickets
         ------------------
         
         - get list of Tickets created before a date (e.g. Jan 01, 2011)
         
         >>> from datetime import datetime
-        >>> client.ticket_search(TicketCreateTimeOlderDate=datetime(2011, 01, 01))
+        >>> client.ticket_search(TicketCreateTimeOlderDate=datetime(2011, 1, 1))
         [u'1']
         
         
         - get list of Tickets created less than a certain time ago (e.g. younger than 1 week)
         
         >>> from datetime import datetime
         >>> from datetime import timedelta
@@ -420,13 +439,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Documentation :: Sphinx
 Provides-Extra: cli
```

### Comparing `PyOTRS-0.8.0/cli/PyOTRS.py` & `PyOTRS-0.9.0/cli/PyOTRS.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # -*- coding: utf-8 -*-
 """ cli """
 
 import os
 import stat
-import click
+try:
+    import click
+except ImportError:
+    raise ImportError("Please install Python dependencies: "
+                      "click, colorama (optional).")
 import tempfile
 
 from pyotrs.version import __version__
 from pyotrs.lib import Client
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
```

