# Comparing `tmp/fastapi_jwt-0.1.7-py3-none-any.whl.zip` & `tmp/fastapi_jwt-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 6074 bytes, number of entries: 7
--rw-r--r--  2.0 unx       39 b- defN 21-Dec-06 19:59 fastapi_jwt/__init__.py
--rw-r--r--  2.0 unx    15630 b- defN 21-Dec-06 19:59 fastapi_jwt/jwt.py
--rw-r--r--  2.0 unx     1078 b- defN 21-Dec-06 20:00 fastapi_jwt-0.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     4565 b- defN 21-Dec-06 20:00 fastapi_jwt-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Dec-06 20:00 fastapi_jwt-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 21-Dec-06 20:00 fastapi_jwt-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      560 b- defN 21-Dec-06 20:00 fastapi_jwt-0.1.7.dist-info/RECORD
-7 files, 21976 bytes uncompressed, 5080 bytes compressed:  76.9%
+Zip file size: 6229 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       39 b- defN 22-Apr-26 10:21 fastapi_jwt/__init__.py
+-rw-r--r--  2.0 unx    15630 b- defN 22-Apr-26 10:21 fastapi_jwt/jwt.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Apr-26 10:21 fastapi_jwt/py.typed
+-rw-r--r--  2.0 unx     1078 b- defN 22-Apr-26 10:21 fastapi_jwt-0.1.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4545 b- defN 22-Apr-26 10:21 fastapi_jwt-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Apr-26 10:21 fastapi_jwt-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 22-Apr-26 10:21 fastapi_jwt-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      634 b- defN 22-Apr-26 10:21 fastapi_jwt-0.1.8.dist-info/RECORD
+8 files, 22030 bytes uncompressed, 5119 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: fastapi_jwt/__init__.py
 Comment: 
 
 Filename: fastapi_jwt/jwt.py
 Comment: 
 
-Filename: fastapi_jwt-0.1.7.dist-info/LICENSE
+Filename: fastapi_jwt/py.typed
 Comment: 
 
-Filename: fastapi_jwt-0.1.7.dist-info/METADATA
+Filename: fastapi_jwt-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: fastapi_jwt-0.1.7.dist-info/WHEEL
+Filename: fastapi_jwt-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: fastapi_jwt-0.1.7.dist-info/top_level.txt
+Filename: fastapi_jwt-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: fastapi_jwt-0.1.7.dist-info/RECORD
+Filename: fastapi_jwt-0.1.8.dist-info/top_level.txt
+Comment: 
+
+Filename: fastapi_jwt-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fastapi_jwt-0.1.7.dist-info/LICENSE` & `fastapi_jwt-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastapi_jwt-0.1.7.dist-info/METADATA` & `fastapi_jwt-0.1.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-jwt
-Version: 0.1.7
+Version: 0.1.8
 Summary: `FastAPI` extension for JTW Auth
 Home-page: https://github.com/k4black/fastapi-jwt
 Author: Konstantin Chernyshev
 Author-email: kdchernyshev@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -19,19 +19,19 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: <3.10,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fastapi (<0.80.0,>=0.50.0)
-Requires-Dist: python-jose[cryptography] (<4.0.0,>=3.3.0)
+Requires-Dist: fastapi (>=0.50.0)
+Requires-Dist: python-jose[cryptography] (>=3.3.0)
 Provides-Extra: docs
 Requires-Dist: mkdocs (<2.0.0,>=1.2.0) ; extra == 'docs'
 Requires-Dist: mkdocs-material (<9.0.0,>=8.0.0) ; extra == 'docs'
 Requires-Dist: MkAutoDoc (<1.0.0,>=0.1.0) ; extra == 'docs'
 Requires-Dist: lazydocs (<1.0.0,>=0.4.5) ; extra == 'docs'
 Requires-Dist: mkdocs-include-markdown-plugin (<4.0.0,>=3.2.0) ; extra == 'docs'
 Requires-Dist: mkdocs-awesome-pages-plugin (<3.0.0,>=2.6.0) ; extra == 'docs'
@@ -61,15 +61,15 @@
 **Documentation:** [k4black.github.io/fastapi-jwt](https://k4black.github.io/fastapi-jwt/)  
 **Source Code:** [github.com/k4black/fastapi-jwt](https://github.com/k4black/fastapi-jwt/)
 
 
 ## Features
 * OpenAPI schema generation 
 * Native integration with FastAPI
-* Access/Refresh JTW
+* Access/Refresh JWT
 * JTI
 * Cookie setting
 
 
 ## Installation
 You can access package [fastapi-jwt in pypi](https://pypi.org/project/fastapi-jwt/)
 ```shell
@@ -120,7 +120,8 @@
 There it is open and maintained [Pull Request #3305](https://github.com/tiangolo/fastapi/pull/3305) to the `fastapi` repo. Currently, not considered.
 
 ## Requirements 
 
 * `fastapi`
 * `python-jose[cryptography]`
 
+
```

