# Comparing `tmp/creative-namer-1.1.0.tar.gz` & `tmp/creative-namer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creative-namer-1.1.0.tar", last modified: Sun May 21 04:18:47 2023, max compression
+gzip compressed data, was "creative-namer-1.1.1.tar", last modified: Sun May 21 04:22:16 2023, max compression
```

## Comparing `creative-namer-1.1.0.tar` & `creative-namer-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 04:18:47.156767 creative-namer-1.1.0/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2477 2023-05-21 04:18:47.156583 creative-namer-1.1.0/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     2305 2023-05-21 04:18:47.000000 creative-namer-1.1.0/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 04:18:47.156402 creative-namer-1.1.0/creative_namer.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2477 2023-05-21 04:18:47.000000 creative-namer-1.1.0/creative_namer.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      266 2023-05-21 04:18:47.000000 creative-namer-1.1.0/creative_namer.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 04:18:47.000000 creative-namer-1.1.0/creative_namer.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       56 2023-05-21 04:18:47.000000 creative-namer-1.1.0/creative_namer.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       19 2023-05-21 04:18:47.000000 creative-namer-1.1.0/creative_namer.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       15 2023-05-21 04:18:47.000000 creative-namer-1.1.0/creative_namer.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     3450 2023-05-21 04:18:47.000000 creative-namer-1.1.0/creative_namer.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 04:18:47.156808 creative-namer-1.1.0/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      520 2023-05-21 04:18:47.000000 creative-namer-1.1.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 04:22:16.446238 creative-namer-1.1.1/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2477 2023-05-21 04:22:16.446035 creative-namer-1.1.1/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2305 2023-05-21 04:22:16.000000 creative-namer-1.1.1/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 04:22:16.445839 creative-namer-1.1.1/creative_namer.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2477 2023-05-21 04:22:16.000000 creative-namer-1.1.1/creative_namer.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      266 2023-05-21 04:22:16.000000 creative-namer-1.1.1/creative_namer.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 04:22:16.000000 creative-namer-1.1.1/creative_namer.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       56 2023-05-21 04:22:16.000000 creative-namer-1.1.1/creative_namer.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       19 2023-05-21 04:22:16.000000 creative-namer-1.1.1/creative_namer.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       15 2023-05-21 04:22:16.000000 creative-namer-1.1.1/creative_namer.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     3372 2023-05-21 04:22:16.000000 creative-namer-1.1.1/creative_namer.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 04:22:16.446280 creative-namer-1.1.1/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      520 2023-05-21 04:22:16.000000 creative-namer-1.1.1/setup.py
```

### Comparing `creative-namer-1.1.0/PKG-INFO` & `creative-namer-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creative-namer
-Version: 1.1.0
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Creative Namer
```

### Comparing `creative-namer-1.1.0/README.md` & `creative-namer-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `creative-namer-1.1.0/creative_namer.egg-info/PKG-INFO` & `creative-namer-1.1.1/creative_namer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creative-namer
-Version: 1.1.0
+Version: 1.1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Creative Namer
```

### Comparing `creative-namer-1.1.0/creative_namer.py` & `creative-namer-1.1.1/creative_namer.py`

 * *Files 9% similar despite different names*

```diff
@@ -82,14 +82,13 @@
     parser.add_argument("--n", type=int, default=DEFAULT_N, help="生成英文專案名稱的數量")
     parser.add_argument("--user", default=DEFAULT_USER, help="使用者的電子郵件地址")
     return parser
 
 
 def main():
     args = get_args_parser().parse_args()
-    json_str = creative_namer(args.project_description, n=args.n, user=args.user, start_tag=args.start_tag,
-                              end_tag=args.end_tag)
+    json_str = creative_namer(args.project_description, n=args.n, user=args.user)
     print('\n--creative_namer.py,main(),json_str:\n', json_str)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `creative-namer-1.1.0/setup.py` & `creative-namer-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="creative-namer",
-    version="1.1.0",
+    version="1.1.1",
     packages=find_packages(),
     py_modules=['creative_namer'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'creative_namer = creative_namer:main',
         ],
```

