# Comparing `tmp/toolforge-weld-0.2.0.tar.gz` & `tmp/toolforge-weld-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge-weld-0.2.0.tar", last modified: Thu May 11 20:08:21 2023, max compression
+gzip compressed data, was "toolforge-weld-0.2.1.tar", last modified: Sun May 21 12:26:23 2023, max compression
```

## Comparing `toolforge-weld-0.2.0.tar` & `toolforge-weld-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:08:21.475040 toolforge-weld-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)    34524 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-11 20:08:21.475040 toolforge-weld-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 20:08:21.475040 toolforge-weld-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      968 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:08:21.471040 toolforge-weld-0.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/tests/test_kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)     3540 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/tests/test_kubernetes_config.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:08:21.471040 toolforge-weld-0.2.0/toolforge_weld/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     7555 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)     2673 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/kubernetes_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:08:21.475040 toolforge-weld-0.2.0/toolforge_weld/logs/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/logs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2456 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/logs/kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/logs/source.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-11 18:14:37.000000 toolforge-weld-0.2.0/toolforge_weld/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 20:08:21.471040 toolforge-weld-0.2.0/toolforge_weld.egg-info/
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-11 20:08:21.000000 toolforge-weld-0.2.0/toolforge_weld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      597 2023-05-11 20:08:21.000000 toolforge-weld-0.2.0/toolforge_weld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 20:08:21.000000 toolforge-weld-0.2.0/toolforge_weld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-05-11 20:08:21.000000 toolforge-weld-0.2.0/toolforge_weld.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-11 20:08:21.000000 toolforge-weld-0.2.0/toolforge_weld.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:23.165054 toolforge-weld-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)    34524 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-21 12:26:23.165054 toolforge-weld-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 12:26:23.165054 toolforge-weld-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      968 2023-05-21 12:25:09.000000 toolforge-weld-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:23.161054 toolforge-weld-0.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/tests/test_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/tests/test_kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3540 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/tests/test_kubernetes_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:23.161054 toolforge-weld-0.2.1/toolforge_weld/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2498 2023-05-21 12:25:09.000000 toolforge-weld-0.2.1/toolforge_weld/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7555 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3021 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/kubernetes_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:23.165054 toolforge-weld-0.2.1/toolforge_weld/logs/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/logs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2456 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/logs/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/logs/source.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-21 11:06:29.000000 toolforge-weld-0.2.1/toolforge_weld/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 12:26:23.161054 toolforge-weld-0.2.1/toolforge_weld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-21 12:26:23.000000 toolforge-weld-0.2.1/toolforge_weld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      622 2023-05-21 12:26:23.000000 toolforge-weld-0.2.1/toolforge_weld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 12:26:23.000000 toolforge-weld-0.2.1/toolforge_weld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-05-21 12:26:23.000000 toolforge-weld-0.2.1/toolforge_weld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-21 12:26:23.000000 toolforge-weld-0.2.1/toolforge_weld.egg-info/top_level.txt
```

### Comparing `toolforge-weld-0.2.0/LICENSE` & `toolforge-weld-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.0/PKG-INFO` & `toolforge-weld-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforge-weld
-Version: 0.2.0
+Version: 0.2.1
 Summary: Shared Python code for Toolforge infrastructure components
 Author: Taavi Väänänen
 Author-email: hi@taavi.wtf
 License: AGPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `toolforge-weld-0.2.0/setup.py` & `toolforge-weld-0.2.1/setup.py`

 * *Files identical despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 
 setup(
     name="toolforge-weld",
-    version="0.2.0",
+    version="0.2.1",
     author="Taavi Väänänen",
     author_email="hi@taavi.wtf",
     license="AGPL-3.0-or-later",
     packages=find_packages(),
     package_data={"toolforge_weld": ["py.typed"]},
     description="Shared Python code for Toolforge infrastructure components",
     long_description=(this_directory / 'README.md').read_text(),
```

### Comparing `toolforge-weld-0.2.0/tests/test_kubernetes_config.py` & `toolforge-weld-0.2.1/tests/test_kubernetes_config.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.0/toolforge_weld/api_client.py` & `toolforge-weld-0.2.1/toolforge_weld/api_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict
+from typing import Any, Callable, Dict, Optional
 
 import requests
 import urllib3
 
 import toolforge_weld
 from toolforge_weld.kubernetes_config import Kubeconfig
 
@@ -13,15 +13,17 @@
     def __init__(
         self,
         *,
         server: str,
         kubeconfig: Kubeconfig,
         user_agent: str,
         timeout: int = 10,
+        exception_handler: Optional[Callable[..., BaseException]] = None,
     ):
+        self.exception_handler = exception_handler
         self.timeout = timeout
         self.server = server
         self.session = requests.Session()
 
         self.session.cert = (
             str(kubeconfig.client_cert_file),
             str(kubeconfig.client_key_file),
@@ -33,39 +35,47 @@
         # Kubernetes API endpoint
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
         self.session.headers[
             "User-Agent"
         ] = f"{user_agent} toolforge_weld/{toolforge_weld.__version__} python-requests/{requests.__version__}"
 
+    def _make_request(self, method: str, url: str, **kwargs) -> requests.Response:
+        try:
+            response = self.session.request(method, **self.make_kwargs(url, **kwargs))
+            response.raise_for_status()
+            return response
+        except requests.exceptions.HTTPError as e:
+            if self.exception_handler:
+                raise self.exception_handler(e)
+            raise e
+
     def make_kwargs(self, url: str, **kwargs) -> Dict[str, Any]:
         """Setup kwargs for a Requests request."""
-        kwargs["url"] = "{}/{}".format(self.server, url)
+        kwargs["url"] = "{}/{}".format(
+            self.server.removesuffix("/"), url.removeprefix("/")
+        )
 
         if "timeout" not in kwargs:
             kwargs["timeout"] = self.timeout
 
         return kwargs
 
     def get(self, url, **kwargs) -> Dict[str, Any]:
         """GET request."""
-        r = self.session.get(**self.make_kwargs(url, **kwargs))
-        r.raise_for_status()
+        r = self._make_request("GET", url, **kwargs)
         return r.json()
 
     def post(self, url, **kwargs) -> int:
         """POST request."""
-        r = self.session.post(**self.make_kwargs(url, **kwargs))
-        r.raise_for_status()
+        r = self._make_request("POST", url, **kwargs)
         return r.status_code
 
     def put(self, url, **kwargs) -> int:
         """PUT request."""
-        r = self.session.put(**self.make_kwargs(url, **kwargs))
-        r.raise_for_status()
+        r = self._make_request("PUT", url, **kwargs)
         return r.status_code
 
     def delete(self, url, **kwargs) -> int:
         """DELETE request."""
-        r = self.session.delete(**self.make_kwargs(url, **kwargs))
-        r.raise_for_status()
+        r = self._make_request("DELETE", url, **kwargs)
         return r.status_code
```

### Comparing `toolforge-weld-0.2.0/toolforge_weld/errors.py` & `toolforge-weld-0.2.1/toolforge_weld/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.0/toolforge_weld/kubernetes.py` & `toolforge-weld-0.2.1/toolforge_weld/kubernetes.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.0/toolforge_weld/kubernetes_config.py` & `toolforge-weld-0.2.1/toolforge_weld/kubernetes_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,7 +73,18 @@
 
 
 def _resolve_file_path(base: Path, input: str) -> Path:
     input_path = Path(input).expanduser()
     if input_path.is_absolute():
         return input_path
     return (base / input_path).resolve()
+
+
+def fake_kube_config() -> Kubeconfig:
+    """Creates a fake Kubeconfig object for testing purposes."""
+    return Kubeconfig(
+        path=Path("dummy/path"),
+        current_server="https://example.org/",
+        current_namespace="tool-test",
+        client_cert_file=Path("/tmp/fake.crt"),
+        client_key_file=Path("/tmp/fake.key"),
+    )
```

### Comparing `toolforge-weld-0.2.0/toolforge_weld/logs/__init__.py` & `toolforge-weld-0.2.1/toolforge_weld/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.0/toolforge_weld/logs/kubernetes.py` & `toolforge-weld-0.2.1/toolforge_weld/logs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.0/toolforge_weld/logs/source.py` & `toolforge-weld-0.2.1/toolforge_weld/logs/source.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.2.0/toolforge_weld.egg-info/PKG-INFO` & `toolforge-weld-0.2.1/toolforge_weld.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforge-weld
-Version: 0.2.0
+Version: 0.2.1
 Summary: Shared Python code for Toolforge infrastructure components
 Author: Taavi Väänänen
 Author-email: hi@taavi.wtf
 License: AGPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `toolforge-weld-0.2.0/toolforge_weld.egg-info/SOURCES.txt` & `toolforge-weld-0.2.1/toolforge_weld.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+tests/test_api_client.py
 tests/test_kubernetes.py
 tests/test_kubernetes_config.py
 tests/test_utils.py
 toolforge_weld/__init__.py
 toolforge_weld/api_client.py
 toolforge_weld/errors.py
 toolforge_weld/kubernetes.py
```

