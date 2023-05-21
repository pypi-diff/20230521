# Comparing `tmp/cuke-0.1.2.tar.gz` & `tmp/cuke-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuke-0.1.2.tar", max compression
+gzip compressed data, was "cuke-0.1.3.tar", max compression
```

## Comparing `cuke-0.1.2.tar` & `cuke-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      405 2023-05-09 03:43:27.198481 cuke-0.1.2/README.md
--rw-r--r--   0        0        0    12131 2023-05-09 03:43:27.198481 cuke-0.1.2/cuke/__init__.py
--rw-r--r--   0        0        0      655 2023-05-09 03:43:27.198481 cuke-0.1.2/cuke/errors.py
--rw-r--r--   0        0        0     1702 2023-05-09 03:43:27.198481 cuke-0.1.2/cuke/util.py
--rw-r--r--   0        0        0      750 2023-05-09 03:43:27.198481 cuke-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 cuke-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      405 2023-05-21 00:39:44.202192 cuke-0.1.3/README.md
+-rw-r--r--   0        0        0    12966 2023-05-21 00:39:44.202192 cuke-0.1.3/cuke/__init__.py
+-rw-r--r--   0        0        0      655 2023-05-21 00:39:44.202192 cuke-0.1.3/cuke/errors.py
+-rw-r--r--   0        0        0     1702 2023-05-21 00:39:44.202192 cuke-0.1.3/cuke/util.py
+-rw-r--r--   0        0        0      775 2023-05-21 00:39:44.202192 cuke-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 cuke-0.1.3/PKG-INFO
```

### Comparing `cuke-0.1.2/cuke/__init__.py` & `cuke-0.1.3/cuke/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 import requests
 from requests.exceptions import HTTPError
 
 from cuke.errors import NoApiKey, NoPageYet, SetPageIdOnInitialization
 from cuke.util import add_header_to_function, get_function_body, make_request_in_api_key_order
 
 KEYS_TO_NOT_UPDATE = {"_dirty_set", "_instant_updates", "_vars", "_vars_lock", "_daemon",
-                      "_contributor_key", "_editor_key", "_page_id", "_page_slug"}
+                      "_contributor_key", "_editor_key", "_page_id", "_page_subslug", "_page_slug"}
 
 class Cuke:
     def __init__(self, url="https://cuke.cool", api_key=None, instant_updates=False,
-                 page_slug=None, page_id=None, contributor_key=None, editor_key=None,
-                 private=False, **kwargs):
+                 page_slug=None, page_subslug=None, page_id=None, contributor_key=None,
+                 editor_key=None, private=False, **kwargs):
         self._dirty_set = set()
         self._instant_updates = instant_updates
         self._vars = {}
         self._vars_lock = threading.Lock()
         self._daemon = None
         self._url = url
         self._api_key = api_key
@@ -34,14 +34,15 @@
             try:
                 self._api_key = open(".cuke").read()
             except:
                 pass
         
         self._user_agent = kwargs.get("user_agent", None)
         self._page_slug = page_slug or self._user_alias
+        self._page_subslug = page_subslug
         self._page_id = page_id
         self._contributor_key = contributor_key
         self._editor_key = editor_key
         
         self._webworker = None
         self._ui_thread_js_for_loop_output = None
         self._setup = None
@@ -59,15 +60,19 @@
         if self._page_id:
             self._initialize_vars()
         self._dirty_set = set()
 
 
     def _call_remote(self, key):
         """Remote version of function with name `key`."""
-        resp = requests.get(f"{self._url}/page/{self._page_slug}/{self._page_id}/execute/{key}", headers=self._headers(self._editor_key))
+        if self._page_subslug:
+            url = f"{self._url}/page/{self._page_slug}/{self._page_subslug}/{self._page_id}/execute/{key}"
+        else:
+            url = f"{self._url}/page/{self._page_slug}/{self._page_id}/execute/{key}"
+        resp = requests.get(url, headers=self._headers(self._editor_key))
         resp.raise_for_status()
         return resp.text
     
     class _CukeFun(object):
         """Function to be executed remotely."""
         def __init__(self, cuke, key):
             self._cuke = weakref.ref(cuke)
@@ -100,29 +105,33 @@
         else:
             super().__setattr__(key, val)
             if key not in KEYS_TO_NOT_UPDATE:
                 self._dirty_set.add(key)
                 if self._instant_updates:
                     self._update()
 
+    def __url_for(self, key):
+        if self._page_subslug:
+            return f"{self._url}/{key}/{self._page_slug}/{self._page_subslug}/{self._page_id}"
+        return f"{self._url}/{key}/{self._page_slug}/{self._page_id}"
+
     @property
     def _page_url(self):
-        return f"{self._url}/page/{self._page_slug}/{self._page_id}"
-
+        return self.__url_for("page")
 
     @property
     def _user_alias(self):
         if self._api_key is None:
             return None
         resp = requests.get(f"{self._url}/user/get_alias", headers=self._headers(self._api_key))
         resp.raise_for_status()
         return resp.json()["alias"]
 
     def _initialize_vars(self):
-        resp = make_request_in_api_key_order(requests.get, self, f"{self._url}/retrieve/{self._page_slug}/{self._page_id}",
+        resp = make_request_in_api_key_order(requests.get, self, self.__url_for("retrieve"),
                                              anonymous_error_msg="because you're trying to connect to an existing page, but without authentication.")
         if resp.status_code == 404:
             return False
         
         resp = resp.json()
         
         self._template = resp.pop("__template__")
@@ -212,15 +221,16 @@
                     update[k] = {"type": "error", "value": f"Could not serialize. {e}" }
         # TODO this needs error handling or it kills the thread
         if os.environ.get("CUKE_PIPELINE_STAGE", None):
             headers = {"X-Cuke-Pipeline-Stage": os.environ["CUKE_PIPELINE_STAGE"]}
         else:
             headers = {}
         try:
-            resp = make_request_in_api_key_order(requests.post, self, f"{self._url}/store/{self._page_slug}/{self._page_id}", json=update, additional_headers=headers)
+            qwe = self.__url_for("store")
+            resp = make_request_in_api_key_order(requests.post, self, self.__url_for("store"), json=update, additional_headers=headers)
             resp.raise_for_status()
         except HTTPError as e:
             if resp.status_code == 404:
                 raise NoPageYet()
             else:
                 raise e
         self._dirty_set = set()
@@ -276,15 +286,15 @@
         Store a template. If basic_auth is provided - a dict with keys username and password - that will set the page up with
         HTTP basic auth.
         """
         if self._page_id is None and self._api_key is not None:
             raise SetPageIdOnInitialization()
         username = self._basic_auth.get("username", None)
         password = self._basic_auth.get("password", None)
-        page_id = self._page_id or ""
+        page_id = self._page_id or None
 
         code = {}
         code["webworker"] = self._webworker
         code["ui_thread_js_for_loop_input"] = None
         # TODO i should probably add this. For example, in the setInterval call:
         # postMessage(`run_the_users_ui_input_code`) ... <user's code is run on ui thread; ui thread sends back a message>
         # onMessage(`from_ui_thread`, data => for key, val in data: pyodide.globals.set(key, val))
@@ -295,26 +305,32 @@
             code["setup"] = inspect.getsource(self._setup).strip()
         if self._loop:
             code["loop"] = inspect.getsource(self._loop).strip()
         if self._event:
             code["event"] = inspect.getsource(self._event).strip()
         code["packages"] = self._packages
         
-        resp = make_request_in_api_key_order(requests.post, self, f"{self._url}/store_template/{page_id}",
-                                             json={"template": template, "username": username, 
-                                             "password": password, "code": code}, allow_anonymous=True)
+        resp = make_request_in_api_key_order(requests.post, self, f"{self._url}/store_template",
+                                             json={"template": template, "username": username,
+                                                   "page_subslug": self._page_subslug, "page_id": page_id, 
+                                                   "password": password, "code": code}, allow_anonymous=True)
 
         resp.raise_for_status()
 
         self._template = template
 
-        url = resp.json()["url"]
+        response = resp.json()
+        url = response["url"]
         if not self._api_key:
-            _, _, self._page_slug, self._page_id = url.split("/")
+            #_, _, self._page_slug, self._page_id = url.split("/")
+            self._page_slug, self._page_subslug, self._page_id = response["page_slug"], response["page_subslug"], response["page_id"]
         if not self._page_id:
-            _, _, _, self._page_id = url.split("/")
+            #_, _, _, self._page_id = url.split("/")
+            self._page_id = response["page_id"]
+        if not self._page_subslug:
+            self._page_subslug = response["page_subslug"]
         if not self._page_slug:
-            _, _, self._page_slug, _ = url.split("/")
+            self._page_slug = response["page_slug"]
         self._contributor_key = resp.json()["contributor_key"]
         self._editor_key = resp.json()["editor_key"]
         
         return resp.json()
```

### Comparing `cuke-0.1.2/cuke/errors.py` & `cuke-0.1.3/cuke/errors.py`

 * *Files identical despite different names*

### Comparing `cuke-0.1.2/cuke/util.py` & `cuke-0.1.3/cuke/util.py`

 * *Files identical despite different names*

### Comparing `cuke-0.1.2/pyproject.toml` & `cuke-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cuke"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python client for cuke.cool"
 authors = ["tomgrek <tom.grek@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cuke"}]
 homepage = "https://cuke.cool"
 repository = "https://github.com/tomgrek/cuke.cool"
 documentation = "https://docs.cuke.cool"
@@ -16,14 +16,15 @@
 requests = "^2.30.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.12.0"
 jupyterlab = "^3.6.2"
 pytest = "^7.2.2"
 pytest-playwright = "^0.3.2"
+pytest-dotenv = "^0.5.2"
 
 [tool.pytest.ini_options]
 pythonpath = "cuke"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cuke-0.1.2/PKG-INFO` & `cuke-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuke
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client for cuke.cool
 Home-page: https://cuke.cool
 Keywords: publishing,faas,serverless,webpage,python
 Author: tomgrek
 Author-email: tom.grek@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

