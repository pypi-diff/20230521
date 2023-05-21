# Comparing `tmp/BingImageCreator-0.2.0.tar.gz` & `tmp/BingImageCreator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BingImageCreator-0.2.0.tar", last modified: Wed May 17 01:32:01 2023, max compression
+gzip compressed data, was "BingImageCreator-0.2.1.tar", last modified: Sun May 21 10:53:55 2023, max compression
```

## Comparing `BingImageCreator-0.2.0.tar` & `BingImageCreator-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:32:01.094792 BingImageCreator-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-17 01:31:39.000000 BingImageCreator-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-17 01:32:01.094792 BingImageCreator-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-17 01:31:39.000000 BingImageCreator-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 01:32:01.098792 BingImageCreator-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-17 01:31:39.000000 BingImageCreator-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:32:01.094792 BingImageCreator-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:32:01.094792 BingImageCreator-0.2.0/src/BingImageCreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-17 01:32:01.000000 BingImageCreator-0.2.0/src/BingImageCreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-17 01:32:01.000000 BingImageCreator-0.2.0/src/BingImageCreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 01:32:01.000000 BingImageCreator-0.2.0/src/BingImageCreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 01:32:01.000000 BingImageCreator-0.2.0/src/BingImageCreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 01:32:01.000000 BingImageCreator-0.2.0/src/BingImageCreator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-05-17 01:31:39.000000 BingImageCreator-0.2.0/src/BingImageCreator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 01:32:01.094792 BingImageCreator-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-17 01:31:39.000000 BingImageCreator-0.2.0/test/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:53:55.302250 BingImageCreator-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-21 10:53:33.000000 BingImageCreator-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-21 10:53:55.302250 BingImageCreator-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-21 10:53:33.000000 BingImageCreator-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 10:53:55.302250 BingImageCreator-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-21 10:53:33.000000 BingImageCreator-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:53:55.302250 BingImageCreator-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:53:55.302250 BingImageCreator-0.2.1/src/BingImageCreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-21 10:53:55.000000 BingImageCreator-0.2.1/src/BingImageCreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-21 10:53:55.000000 BingImageCreator-0.2.1/src/BingImageCreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 10:53:55.000000 BingImageCreator-0.2.1/src/BingImageCreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 10:53:55.000000 BingImageCreator-0.2.1/src/BingImageCreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-21 10:53:55.000000 BingImageCreator-0.2.1/src/BingImageCreator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14630 2023-05-21 10:53:33.000000 BingImageCreator-0.2.1/src/BingImageCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:53:55.302250 BingImageCreator-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-21 10:53:33.000000 BingImageCreator-0.2.1/test/test_example.py
```

### Comparing `BingImageCreator-0.2.0/LICENSE` & `BingImageCreator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.2.0/PKG-INFO` & `BingImageCreator-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.2.0
+Version: 0.2.1
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.2.0/README.md` & `BingImageCreator-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.2.0/setup.py` & `BingImageCreator-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="BingImageCreator",
-    version="0.2.0",
+    version="0.2.1",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="High quality image generation by Microsoft. Reverse engineered API.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/BingImageCreator",
```

### Comparing `BingImageCreator-0.2.0/src/BingImageCreator.egg-info/PKG-INFO` & `BingImageCreator-0.2.1/src/BingImageCreator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.2.0
+Version: 0.2.1
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.2.0/src/BingImageCreator.py` & `BingImageCreator-0.2.1/src/BingImageCreator.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,19 +58,26 @@
     """
     Image generation by Microsoft Bing
     Parameters:3
         auth_cookie: str
     """
 
     def __init__(
-        self, auth_cookie: str, debug_file: Union[str, None] = None, quiet: bool = False
+        self,
+        auth_cookie: str,
+        debug_file: Union[str, None] = None,
+        quiet: bool = False,
+        all_cookies: list[dict] = None,
     ) -> None:
         self.session: requests.Session = requests.Session()
         self.session.headers = HEADERS
         self.session.cookies.set("_U", auth_cookie)
+        if all_cookies:
+            for cookie in all_cookies:
+                self.session.cookies.set(cookie["name"], cookie["value"])
         self.quiet = quiet
         self.debug_file = debug_file
         if self.debug_file:
             self.debug = partial(debug, self.debug_file)
 
     def get_images(self, prompt: str) -> list:
         """
@@ -366,28 +373,28 @@
     args = parser.parse_args()
 
     if args.version:
         print(pkg_resources.get_distribution("BingImageCreator").version)
         sys.exit()
 
     # Load auth cookie
-    with contextlib.suppress(Exception):
-        with open(args.cookie_file, encoding="utf-8") as file:
-            cookie_json = json.load(file)
-            for cookie in cookie_json:
-                if cookie.get("name") == "_U":
-                    args.U = cookie.get("value")
-                    break
+    cookie_json = None
+    if args.cookie_file is not None:
+        with contextlib.suppress(Exception):
+            with open(args.cookie_file, encoding="utf-8") as file:
+                cookie_json = json.load(file)
 
     if args.U is None and args.cookie_file is None:
         raise Exception("Could not find auth cookie")
 
     if not args.asyncio:
         # Create image generator
-        image_generator = ImageGen(args.U, args.debug_file, args.quiet)
+        image_generator = ImageGen(
+            args.U, args.debug_file, args.quiet, all_cookies=cookie_json
+        )
         image_generator.save_images(
             image_generator.get_images(args.prompt),
             output_dir=args.output_dir,
         )
     else:
         asyncio.run(async_image_gen(args))
```

### Comparing `BingImageCreator-0.2.0/test/test_example.py` & `BingImageCreator-0.2.1/test/test_example.py`

 * *Files identical despite different names*

