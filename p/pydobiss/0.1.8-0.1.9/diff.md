# Comparing `tmp/pydobiss-0.1.8.tar.gz` & `tmp/pydobiss-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydobiss-0.1.8.tar", last modified: Mon Nov 16 09:30:41 2020, max compression
+gzip compressed data, was "dist/pydobiss-0.1.9.tar", last modified: Mon Nov 16 09:53:54 2020, max compression
```

## Comparing `pydobiss-0.1.8.tar` & `pydobiss-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kester     (501) staff       (20)        0 2020-11-16 09:30:41.119064 pydobiss-0.1.8/
--rw-r--r--   0 kester     (501) staff       (20)     1071 2020-11-14 09:47:16.000000 pydobiss-0.1.8/LICENSE
--rw-r--r--   0 kester     (501) staff       (20)       16 2020-11-14 09:47:16.000000 pydobiss-0.1.8/MANIFEST.in
--rw-r--r--   0 kester     (501) staff       (20)     2898 2020-11-16 09:30:41.119308 pydobiss-0.1.8/PKG-INFO
--rw-r--r--   0 kester     (501) staff       (20)     1878 2020-11-16 09:28:55.000000 pydobiss-0.1.8/README.md
-drwxr-xr-x   0 kester     (501) staff       (20)        0 2020-11-16 09:30:41.116104 pydobiss-0.1.8/dobissapi/
--rw-r--r--   0 kester     (501) staff       (20)       25 2020-11-14 09:47:16.000000 pydobiss-0.1.8/dobissapi/__init__.py
--rw-r--r--   0 kester     (501) staff       (20)    16659 2020-11-16 09:22:06.000000 pydobiss-0.1.8/dobissapi/dobissapi.py
-drwxr-xr-x   0 kester     (501) staff       (20)        0 2020-11-16 09:30:41.118574 pydobiss-0.1.8/pydobiss.egg-info/
--rw-r--r--   0 kester     (501) staff       (20)     2898 2020-11-16 09:30:40.000000 pydobiss-0.1.8/pydobiss.egg-info/PKG-INFO
--rw-r--r--   0 kester     (501) staff       (20)      252 2020-11-16 09:30:40.000000 pydobiss-0.1.8/pydobiss.egg-info/SOURCES.txt
--rw-r--r--   0 kester     (501) staff       (20)        1 2020-11-16 09:30:40.000000 pydobiss-0.1.8/pydobiss.egg-info/dependency_links.txt
--rw-r--r--   0 kester     (501) staff       (20)       22 2020-11-16 09:30:40.000000 pydobiss-0.1.8/pydobiss.egg-info/requires.txt
--rw-r--r--   0 kester     (501) staff       (20)       10 2020-11-16 09:30:40.000000 pydobiss-0.1.8/pydobiss.egg-info/top_level.txt
--rw-r--r--   0 kester     (501) staff       (20)       79 2020-11-16 09:30:41.119827 pydobiss-0.1.8/setup.cfg
--rw-r--r--   0 kester     (501) staff       (20)      657 2020-11-16 09:23:32.000000 pydobiss-0.1.8/setup.py
+drwxr-xr-x   0 kester     (501) staff       (20)        0 2020-11-16 09:53:54.297583 pydobiss-0.1.9/
+-rw-r--r--   0 kester     (501) staff       (20)     1071 2020-11-14 09:47:16.000000 pydobiss-0.1.9/LICENSE
+-rw-r--r--   0 kester     (501) staff       (20)       16 2020-11-14 09:47:16.000000 pydobiss-0.1.9/MANIFEST.in
+-rw-r--r--   0 kester     (501) staff       (20)     2898 2020-11-16 09:53:54.297805 pydobiss-0.1.9/PKG-INFO
+-rw-r--r--   0 kester     (501) staff       (20)     1878 2020-11-16 09:45:19.000000 pydobiss-0.1.9/README.md
+drwxr-xr-x   0 kester     (501) staff       (20)        0 2020-11-16 09:53:54.293404 pydobiss-0.1.9/dobissapi/
+-rw-r--r--   0 kester     (501) staff       (20)       25 2020-11-14 09:47:16.000000 pydobiss-0.1.9/dobissapi/__init__.py
+-rw-r--r--   0 kester     (501) staff       (20)    16773 2020-11-16 09:42:44.000000 pydobiss-0.1.9/dobissapi/dobissapi.py
+drwxr-xr-x   0 kester     (501) staff       (20)        0 2020-11-16 09:53:54.297095 pydobiss-0.1.9/pydobiss.egg-info/
+-rw-r--r--   0 kester     (501) staff       (20)     2898 2020-11-16 09:53:54.000000 pydobiss-0.1.9/pydobiss.egg-info/PKG-INFO
+-rw-r--r--   0 kester     (501) staff       (20)      252 2020-11-16 09:53:54.000000 pydobiss-0.1.9/pydobiss.egg-info/SOURCES.txt
+-rw-r--r--   0 kester     (501) staff       (20)        1 2020-11-16 09:53:54.000000 pydobiss-0.1.9/pydobiss.egg-info/dependency_links.txt
+-rw-r--r--   0 kester     (501) staff       (20)       22 2020-11-16 09:53:54.000000 pydobiss-0.1.9/pydobiss.egg-info/requires.txt
+-rw-r--r--   0 kester     (501) staff       (20)       10 2020-11-16 09:53:54.000000 pydobiss-0.1.9/pydobiss.egg-info/top_level.txt
+-rw-r--r--   0 kester     (501) staff       (20)       79 2020-11-16 09:53:54.298618 pydobiss-0.1.9/setup.cfg
+-rw-r--r--   0 kester     (501) staff       (20)      657 2020-11-16 09:45:37.000000 pydobiss-0.1.9/setup.py
```

### Comparing `pydobiss-0.1.8/LICENSE` & `pydobiss-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydobiss-0.1.8/PKG-INFO` & `pydobiss-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydobiss
-Version: 0.1.8
+Version: 0.1.9
 Summary: python interface to the dobiss developer api
 Home-page: https://github.com/kesteraernoudt/pydobiss
 Author: Kester Aernoudt
 Author-email: kesteraernoudt@yahoo.com
 License: MIT
 Description: pydobiss Module Repository
         ==========================
```

### Comparing `pydobiss-0.1.8/README.md` & `pydobiss-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pydobiss-0.1.8/dobissapi/dobissapi.py` & `pydobiss-0.1.9/dobissapi/dobissapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,30 +268,33 @@
         return self._session
 
     def start_session(self):
         if not self._session or self._session.closed:
             self._session = aiohttp.ClientSession(raise_for_status=True)
         return self._session
 
-    def end_session(self):
-        if self._session and not self.session.closed:
-            self._session.close()
+    async def end_session(self):
+        if self._session:
+            if not self.session.closed:
+                await self._session.close()
             self._session = None
         return self._session
 
     async def auth_check(self):
         headers = { 'Authorization': 'Bearer ' + self.get_token() }
         auth_ok = False
         try:
             self.start_session()
             async with self._session.get(self._url + 'status', headers=headers) as response:
                 if response and response.status == 200:
                     auth_ok = True
         except:
             logger.exception("Äuthenticating Dobiss failed")
+        finally:
+            await self._session.close()
         return auth_ok
 
     def get_token(self):
         """ Request a token to use in a request to the Dobiss server """
         if self._exp_time < datetime.now() + timedelta(hours=20):
             # get new token
             self._token = (jwt.encode({'name': 'my_application'}, self._secret, headers={'expiresIn': "24h" })).decode("utf-8")
@@ -341,14 +344,15 @@
     async def status(self, address = None, channel = None):
         data = {}
         if address != None:
             data["address"] = address
         if channel != None:
             data["channel"] = channel
         headers = { 'Authorization': 'Bearer ' + self.get_token() }
+        self.start_session()
         return await self._session.get(self._url + 'status', headers=headers, json=data)
 
     async def action(self, address, channel, action, option1 = None):
         writedata = { 'address': address, 'channel': channel, 'action': action }
         if option1 != None:
             writedata["option1"] = option1
         headers = { 'Authorization': 'Bearer ' + self.get_token() }
```

### Comparing `pydobiss-0.1.8/pydobiss.egg-info/PKG-INFO` & `pydobiss-0.1.9/pydobiss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydobiss
-Version: 0.1.8
+Version: 0.1.9
 Summary: python interface to the dobiss developer api
 Home-page: https://github.com/kesteraernoudt/pydobiss
 Author: Kester Aernoudt
 Author-email: kesteraernoudt@yahoo.com
 License: MIT
 Description: pydobiss Module Repository
         ==========================
```

### Comparing `pydobiss-0.1.8/setup.py` & `pydobiss-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='pydobiss',
-    version='0.1.8',
+    version='0.1.9',
     description='python interface to the dobiss developer api',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Kester Aernoudt',
     author_email='kesteraernoudt@yahoo.com',
     url='https://github.com/kesteraernoudt/pydobiss',
     license='MIT',
```

