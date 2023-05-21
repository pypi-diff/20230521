# Comparing `tmp/sftp_uploader-1.0.4.tar.gz` & `tmp/sftp_uploader-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftp_uploader-1.0.4.tar", max compression
+gzip compressed data, was "sftp_uploader-1.0.5.tar", max compression
```

## Comparing `sftp_uploader-1.0.4.tar` & `sftp_uploader-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1065 2023-05-20 07:24:26.996978 sftp_uploader-1.0.4/LICENSE
--rw-r--r--   0        0        0      408 2023-05-21 05:57:54.673932 sftp_uploader-1.0.4/README.md
--rw-r--r--   0        0        0     1365 2023-05-21 20:53:02.033368 sftp_uploader-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      697 2023-05-21 12:50:31.918508 sftp_uploader-1.0.4/sftp_uploader/__init__.py
--rw-r--r--   0        0        0       42 2023-05-20 09:27:25.068533 sftp_uploader-1.0.4/sftp_uploader/applications/__init__.py
--rw-r--r--   0        0        0     2279 2023-05-20 14:10:57.521529 sftp_uploader-1.0.4/sftp_uploader/applications/dependency_container.py
--rw-r--r--   0        0        0     2135 2023-05-21 07:11:20.183796 sftp_uploader-1.0.4/sftp_uploader/applications/env_load.py
--rw-r--r--   0        0        0     4657 2023-05-21 12:37:31.948650 sftp_uploader-1.0.4/sftp_uploader/applications/git_manipulation.py
--rw-r--r--   0        0        0      705 2023-05-20 19:47:55.241332 sftp_uploader-1.0.4/sftp_uploader/applications/logs.py
--rw-r--r--   0        0        0      350 2023-05-21 13:19:09.740175 sftp_uploader-1.0.4/sftp_uploader/applications/poetry_post_install.py
--rw-r--r--   0        0        0      600 2023-05-21 12:44:39.776066 sftp_uploader-1.0.4/sftp_uploader/applications/pre_commit_actions.py
--rw-r--r--   0        0        0     4085 2023-05-21 07:19:21.887091 sftp_uploader-1.0.4/sftp_uploader/applications/sftp.py
--rw-r--r--   0        0        0     1442 2023-05-21 12:43:37.252590 sftp_uploader-1.0.4/sftp_uploader/applications/sftp_uploader.py
--rw-r--r--   0        0        0     2866 2023-05-20 13:41:17.047261 sftp_uploader-1.0.4/sftp_uploader/applications/ssh.py
--rw-r--r--   0        0        0      160 2023-05-20 13:46:09.134055 sftp_uploader-1.0.4/sftp_uploader/constants/applications/dependency_container.py
--rw-r--r--   0        0        0       38 2023-05-20 11:19:48.844840 sftp_uploader-1.0.4/sftp_uploader/constants/applications/env_load.py
--rw-r--r--   0        0        0      554 2023-05-21 13:01:23.892525 sftp_uploader-1.0.4/sftp_uploader/constants/applications/git_manipulation.py
--rw-r--r--   0        0        0      111 2023-05-20 19:48:34.639833 sftp_uploader-1.0.4/sftp_uploader/constants/applications/logs.py
--rw-r--r--   0        0        0       58 2023-05-20 09:37:11.920073 sftp_uploader-1.0.4/sftp_uploader/constants/applications/ssh.py
--rw-r--r--   0        0        0       38 2023-05-20 09:27:08.700932 sftp_uploader-1.0.4/sftp_uploader/services/__init__.py
--rw-r--r--   0        0        0      738 2023-05-21 12:27:50.714821 sftp_uploader-1.0.4/sftp_uploader/services/applications/git_manipulation.py
--rw-r--r--   0        0        0      338 2023-05-21 07:22:37.795342 sftp_uploader-1.0.4/sftp_uploader/services/applications/sftp_uploader.py
--rw-r--r--   0        0        0      151 2023-05-21 07:27:41.176725 sftp_uploader-1.0.4/sftp_uploader/services/exceptions/pre_commit_actions.py
--rw-r--r--   0        0        0      164 2023-05-20 13:20:59.757264 sftp_uploader-1.0.4/sftp_uploader/services/exceptions/sftp.py
--rw-r--r--   0        0        0       81 2023-05-20 13:20:16.751418 sftp_uploader-1.0.4/sftp_uploader/services/exceptions/ssh.py
--rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 sftp_uploader-1.0.4/setup.py
--rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 sftp_uploader-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-20 07:24:26.996978 sftp_uploader-1.0.5/LICENSE
+-rw-r--r--   0        0        0      408 2023-05-21 05:57:54.673932 sftp_uploader-1.0.5/README.md
+-rw-r--r--   0        0        0     1306 2023-05-21 20:55:20.089740 sftp_uploader-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      697 2023-05-21 12:50:31.918508 sftp_uploader-1.0.5/sftp_uploader/__init__.py
+-rw-r--r--   0        0        0       42 2023-05-20 09:27:25.068533 sftp_uploader-1.0.5/sftp_uploader/applications/__init__.py
+-rw-r--r--   0        0        0     2279 2023-05-20 14:10:57.521529 sftp_uploader-1.0.5/sftp_uploader/applications/dependency_container.py
+-rw-r--r--   0        0        0     2135 2023-05-21 07:11:20.183796 sftp_uploader-1.0.5/sftp_uploader/applications/env_load.py
+-rw-r--r--   0        0        0     4657 2023-05-21 12:37:31.948650 sftp_uploader-1.0.5/sftp_uploader/applications/git_manipulation.py
+-rw-r--r--   0        0        0      705 2023-05-20 19:47:55.241332 sftp_uploader-1.0.5/sftp_uploader/applications/logs.py
+-rw-r--r--   0        0        0      326 2023-05-21 20:55:10.806007 sftp_uploader-1.0.5/sftp_uploader/applications/post_install.py
+-rw-r--r--   0        0        0      600 2023-05-21 12:44:39.776066 sftp_uploader-1.0.5/sftp_uploader/applications/pre_commit_actions.py
+-rw-r--r--   0        0        0     4085 2023-05-21 07:19:21.887091 sftp_uploader-1.0.5/sftp_uploader/applications/sftp.py
+-rw-r--r--   0        0        0     1442 2023-05-21 12:43:37.252590 sftp_uploader-1.0.5/sftp_uploader/applications/sftp_uploader.py
+-rw-r--r--   0        0        0     2866 2023-05-20 13:41:17.047261 sftp_uploader-1.0.5/sftp_uploader/applications/ssh.py
+-rw-r--r--   0        0        0      160 2023-05-20 13:46:09.134055 sftp_uploader-1.0.5/sftp_uploader/constants/applications/dependency_container.py
+-rw-r--r--   0        0        0       38 2023-05-20 11:19:48.844840 sftp_uploader-1.0.5/sftp_uploader/constants/applications/env_load.py
+-rw-r--r--   0        0        0      554 2023-05-21 13:01:23.892525 sftp_uploader-1.0.5/sftp_uploader/constants/applications/git_manipulation.py
+-rw-r--r--   0        0        0      111 2023-05-20 19:48:34.639833 sftp_uploader-1.0.5/sftp_uploader/constants/applications/logs.py
+-rw-r--r--   0        0        0       58 2023-05-20 09:37:11.920073 sftp_uploader-1.0.5/sftp_uploader/constants/applications/ssh.py
+-rw-r--r--   0        0        0       38 2023-05-20 09:27:08.700932 sftp_uploader-1.0.5/sftp_uploader/services/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-21 12:27:50.714821 sftp_uploader-1.0.5/sftp_uploader/services/applications/git_manipulation.py
+-rw-r--r--   0        0        0      338 2023-05-21 07:22:37.795342 sftp_uploader-1.0.5/sftp_uploader/services/applications/sftp_uploader.py
+-rw-r--r--   0        0        0      151 2023-05-21 07:27:41.176725 sftp_uploader-1.0.5/sftp_uploader/services/exceptions/pre_commit_actions.py
+-rw-r--r--   0        0        0      164 2023-05-20 13:20:59.757264 sftp_uploader-1.0.5/sftp_uploader/services/exceptions/sftp.py
+-rw-r--r--   0        0        0       81 2023-05-20 13:20:16.751418 sftp_uploader-1.0.5/sftp_uploader/services/exceptions/ssh.py
+-rw-r--r--   0        0        0     1604 1970-01-01 00:00:00.000000 sftp_uploader-1.0.5/setup.py
+-rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 sftp_uploader-1.0.5/PKG-INFO
```

### Comparing `sftp_uploader-1.0.4/LICENSE` & `sftp_uploader-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.4/pyproject.toml` & `sftp_uploader-1.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sftp_uploader"
-version = "1.0.4"
+version = "1.0.5"
 description = "Package for upload data to sftp with different parametrs and with different methods"
 
 authors = ["Moonvent <moonvent@proton.me>"]
 
 license = "MIT"
 readme = "README.md"
 
@@ -48,9 +48,8 @@
 twine = "^4.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-post_install = "keks:run"
-# post_install = "sftp_uploader.applications.poetry_post_install:poetry_post_install_actions"
+post_install = "sftp_uploader.applications.post_install:run"
```

### Comparing `sftp_uploader-1.0.4/sftp_uploader/__init__.py` & `sftp_uploader-1.0.5/sftp_uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.4/sftp_uploader/applications/dependency_container.py` & `sftp_uploader-1.0.5/sftp_uploader/applications/dependency_container.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.4/sftp_uploader/applications/env_load.py` & `sftp_uploader-1.0.5/sftp_uploader/applications/env_load.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.4/sftp_uploader/applications/git_manipulation.py` & `sftp_uploader-1.0.5/sftp_uploader/applications/git_manipulation.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.4/sftp_uploader/applications/logs.py` & `sftp_uploader-1.0.5/sftp_uploader/applications/logs.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.4/sftp_uploader/applications/pre_commit_actions.py` & `sftp_uploader-1.0.5/sftp_uploader/applications/pre_commit_actions.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.4/sftp_uploader/applications/sftp.py` & `sftp_uploader-1.0.5/sftp_uploader/applications/sftp.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.4/sftp_uploader/applications/sftp_uploader.py` & `sftp_uploader-1.0.5/sftp_uploader/applications/sftp_uploader.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.4/sftp_uploader/applications/ssh.py` & `sftp_uploader-1.0.5/sftp_uploader/applications/ssh.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.4/sftp_uploader/constants/applications/git_manipulation.py` & `sftp_uploader-1.0.5/sftp_uploader/constants/applications/git_manipulation.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.4/sftp_uploader/services/applications/git_manipulation.py` & `sftp_uploader-1.0.5/sftp_uploader/services/applications/git_manipulation.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.4/setup.py` & `sftp_uploader-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 ['dependency-injector>=4.41.0,<5.0.0',
  'gitpython>=3.1.31,<4.0.0',
  'paramiko>=3.1.0,<4.0.0',
  'pydantic>=1.10.7,<2.0.0',
  'python-dotenv>=1.0.0,<2.0.0']
 
 entry_points = \
-{'console_scripts': ['post_install = keks:run']}
+{'console_scripts': ['post_install = '
+                     'sftp_uploader.applications.post_install:run']}
 
 setup_kwargs = {
     'name': 'sftp-uploader',
-    'version': '1.0.4',
+    'version': '1.0.5',
     'description': 'Package for upload data to sftp with different parametrs and with different methods',
     'long_description': '# TODO\n\n[ ] Make title, description, which problem is solve, metter of this project description\n\n[ ] Add more [classifiers](https://pypi.org/classifiers/)\n\n[ ] Add tests\n\n[ ] Add additional links to project conf\n\n[ ] Add poetry scripts and pre-commit scripts\n\n[ ] Add poetry post install, if git exists andd to gitignore and setup pre commit hook, and setup config module, if not exists, create and setup it\n',
     'author': 'Moonvent',
     'author_email': 'moonvent@proton.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/moonvent/sftp_uploader/',
```

### Comparing `sftp_uploader-1.0.4/PKG-INFO` & `sftp_uploader-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftp-uploader
-Version: 1.0.4
+Version: 1.0.5
 Summary: Package for upload data to sftp with different parametrs and with different methods
 Home-page: https://github.com/moonvent/sftp_uploader/
 License: MIT
 Keywords: sftp,git
 Author: Moonvent
 Author-email: moonvent@proton.me
 Requires-Python: >=3.11,<4.0
```

