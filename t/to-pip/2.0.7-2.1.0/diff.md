# Comparing `tmp/to-pip-2.0.7.tar.gz` & `tmp/to-pip-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to-pip-2.0.7.tar", last modified: Sun May 21 00:19:43 2023, max compression
+gzip compressed data, was "to-pip-2.1.0.tar", last modified: Sun May 21 06:14:53 2023, max compression
```

## Comparing `to-pip-2.0.7.tar` & `to-pip-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 00:19:43.773320 to-pip-2.0.7/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-21 00:19:43.773210 to-pip-2.0.7/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     2121 2023-05-21 00:19:43.000000 to-pip-2.0.7/README.md
--rwxr-xr-x   0 chiubowen   (501) staff       (20)       66 2023-05-21 00:19:43.000000 to-pip-2.0.7/hi.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 00:19:43.773353 to-pip-2.0.7/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      508 2023-05-21 00:19:43.000000 to-pip-2.0.7/setup.py
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 00:19:43.773059 to-pip-2.0.7/to_pip.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      216 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       54 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)      103 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       10 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     4483 2023-05-21 00:19:43.000000 to-pip-2.0.7/to_pip.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 06:14:53.953327 to-pip-2.1.0/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-21 06:14:53.953207 to-pip-2.1.0/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2121 2023-05-21 06:14:53.000000 to-pip-2.1.0/README.md
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-05-21 06:14:53.953387 to-pip-2.1.0/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      488 2023-05-21 06:14:53.000000 to-pip-2.1.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-05-21 06:14:53.953046 to-pip-2.1.0/to_pip.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2285 2023-05-21 06:14:53.000000 to-pip-2.1.0/to_pip.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      210 2023-05-21 06:14:53.000000 to-pip-2.1.0/to_pip.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-05-21 06:14:53.000000 to-pip-2.1.0/to_pip.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       40 2023-05-21 06:14:53.000000 to-pip-2.1.0/to_pip.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)      103 2023-05-21 06:14:53.000000 to-pip-2.1.0/to_pip.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        7 2023-05-21 06:14:53.000000 to-pip-2.1.0/to_pip.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     4805 2023-05-21 06:14:53.000000 to-pip-2.1.0/to_pip.py
```

### Comparing `to-pip-2.0.7/PKG-INFO` & `to-pip-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-pip
-Version: 2.0.7
+Version: 2.1.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # to-pip
```

### Comparing `to-pip-2.0.7/README.md` & `to-pip-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `to-pip-2.0.7/to_pip.egg-info/PKG-INFO` & `to-pip-2.1.0/to_pip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-pip
-Version: 2.0.7
+Version: 2.1.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # to-pip
```

### Comparing `to-pip-2.0.7/to_pip.py` & `to-pip-2.1.0/to_pip.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/usr/bin/env python
-# to_pip.py
 import argparse
 import os
 import shutil
 import sys
-import tempfile
 
 
 def usage():
     print(
         f"Usage: python -m to_pip -n <package_name> -v <package_version> [-u <pypi_username> -p <pypi_password>] <python_files>"
     )
     sys.exit(1)
@@ -21,17 +19,16 @@
     parser.add_argument("-u", "--pypi_username", help="PyPI username", default="")
     parser.add_argument("-p", "--pypi_password", help="PyPI password", default="")
     parser.add_argument("python_files", nargs="*", help="Python files to include")
     return parser.parse_args()
 
 
 def create_package_dir(package_name, package_version, python_files):
-    tmp_dir = tempfile.mkdtemp()
-    package_dir = os.path.join(tmp_dir, f"{package_name}-{package_version}")
-    os.makedirs(package_dir)
+    package_dir = os.path.join(os.getcwd(), f"{package_name}-{package_version}")
+    os.makedirs(package_dir, exist_ok=True)
 
     for file in python_files:
         file_name = os.path.basename(file)
         if os.path.exists(os.path.join(package_dir, file_name)):
             print(f"Error: File {file_name} already exists in the package directory.")
             sys.exit(1)
         with open(file) as src, open(os.path.join(package_dir, file_name), "w") as dest:
@@ -74,14 +71,20 @@
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',)
 """
 
     with open(os.path.join(package_dir, "setup.py"), "w") as f:
         f.write(setup_py)
 
+    # Copy setup.py to the root directory
+    shutil.copy(os.path.join(package_dir, "setup.py"), "setup.py")
+    print("Successfully generated setup.py file")
+    print("To install the package from your GitHub repository, use the following command:")
+    print("pip install git+https://github.com/your_username/your_repo.git")
+
 
 def handle_readme(package_dir, package_name):
     if os.path.exists("README.md"):
         shutil.copy("README.md", os.path.join(package_dir, "README.md"))
     else:
         with open(os.path.join(package_dir, "README.md"), "w") as f:
             f.write(f"# {package_name}\n\nThis is a placeholder README.md file.")
@@ -116,16 +119,15 @@
     # Build the package before uploading
     build_exit_code = os.system(f"cd {package_dir} && python setup.py sdist bdist_wheel")
     if build_exit_code != 0:
         print("Error: Failed to build the package.")
         sys.exit(1)
     exit_code = os.system(f"cd {package_dir} && twine upload --config-file ~/.pypirc dist/*")
     if exit_code != 0:
-        print("Error: Failed to upload the package.")
-        sys.exit(1)
+        print("Error: Failed to upload the package. The package installation from GitHub is still possible.")
 
 
 def to_pip_args():
     args = parse_args()
 
     if not args.python_files:
         usage()
```

