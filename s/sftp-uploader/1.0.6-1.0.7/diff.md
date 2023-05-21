# Comparing `tmp/sftp_uploader-1.0.6.tar.gz` & `tmp/sftp_uploader-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftp_uploader-1.0.6.tar", max compression
+gzip compressed data, was "sftp_uploader-1.0.7.tar", last modified: Sun May 21 21:16:36 2023, max compression
```

## Comparing `sftp_uploader-1.0.6.tar` & `sftp_uploader-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,32 @@
--rw-r--r--   0        0        0     1065 2023-05-20 07:24:26.996978 sftp_uploader-1.0.6/LICENSE
--rw-r--r--   0        0        0      408 2023-05-21 05:57:54.673932 sftp_uploader-1.0.6/README.md
--rw-r--r--   0        0        0     1293 2023-05-21 21:02:12.056605 sftp_uploader-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      697 2023-05-21 12:50:31.918508 sftp_uploader-1.0.6/sftp_uploader/__init__.py
--rw-r--r--   0        0        0       42 2023-05-20 09:27:25.068533 sftp_uploader-1.0.6/sftp_uploader/applications/__init__.py
--rw-r--r--   0        0        0     2279 2023-05-20 14:10:57.521529 sftp_uploader-1.0.6/sftp_uploader/applications/dependency_container.py
--rw-r--r--   0        0        0     2135 2023-05-21 07:11:20.183796 sftp_uploader-1.0.6/sftp_uploader/applications/env_load.py
--rw-r--r--   0        0        0     4657 2023-05-21 12:37:31.948650 sftp_uploader-1.0.6/sftp_uploader/applications/git_manipulation.py
--rw-r--r--   0        0        0      705 2023-05-20 19:47:55.241332 sftp_uploader-1.0.6/sftp_uploader/applications/logs.py
--rw-r--r--   0        0        0      600 2023-05-21 12:44:39.776066 sftp_uploader-1.0.6/sftp_uploader/applications/pre_commit_actions.py
--rw-r--r--   0        0        0     4085 2023-05-21 07:19:21.887091 sftp_uploader-1.0.6/sftp_uploader/applications/sftp.py
--rw-r--r--   0        0        0     1442 2023-05-21 12:43:37.252590 sftp_uploader-1.0.6/sftp_uploader/applications/sftp_uploader.py
--rw-r--r--   0        0        0     2866 2023-05-20 13:41:17.047261 sftp_uploader-1.0.6/sftp_uploader/applications/ssh.py
--rw-r--r--   0        0        0      160 2023-05-20 13:46:09.134055 sftp_uploader-1.0.6/sftp_uploader/constants/applications/dependency_container.py
--rw-r--r--   0        0        0       38 2023-05-20 11:19:48.844840 sftp_uploader-1.0.6/sftp_uploader/constants/applications/env_load.py
--rw-r--r--   0        0        0      554 2023-05-21 13:01:23.892525 sftp_uploader-1.0.6/sftp_uploader/constants/applications/git_manipulation.py
--rw-r--r--   0        0        0      111 2023-05-20 19:48:34.639833 sftp_uploader-1.0.6/sftp_uploader/constants/applications/logs.py
--rw-r--r--   0        0        0       58 2023-05-20 09:37:11.920073 sftp_uploader-1.0.6/sftp_uploader/constants/applications/ssh.py
--rw-r--r--   0        0        0      326 2023-05-21 21:00:53.610182 sftp_uploader-1.0.6/sftp_uploader/post_install.py
--rw-r--r--   0        0        0       38 2023-05-20 09:27:08.700932 sftp_uploader-1.0.6/sftp_uploader/services/__init__.py
--rw-r--r--   0        0        0      738 2023-05-21 12:27:50.714821 sftp_uploader-1.0.6/sftp_uploader/services/applications/git_manipulation.py
--rw-r--r--   0        0        0      338 2023-05-21 07:22:37.795342 sftp_uploader-1.0.6/sftp_uploader/services/applications/sftp_uploader.py
--rw-r--r--   0        0        0      151 2023-05-21 07:27:41.176725 sftp_uploader-1.0.6/sftp_uploader/services/exceptions/pre_commit_actions.py
--rw-r--r--   0        0        0      164 2023-05-20 13:20:59.757264 sftp_uploader-1.0.6/sftp_uploader/services/exceptions/sftp.py
--rw-r--r--   0        0        0       81 2023-05-20 13:20:16.751418 sftp_uploader-1.0.6/sftp_uploader/services/exceptions/ssh.py
--rw-r--r--   0        0        0     1567 1970-01-01 00:00:00.000000 sftp_uploader-1.0.6/setup.py
--rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 sftp_uploader-1.0.6/PKG-INFO
+drwxr-xr-x   0 nikitakurkurin   (501) staff       (20)        0 2023-05-21 21:16:36.661273 sftp_uploader-1.0.7/
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)     1065 2023-05-20 07:24:26.000000 sftp_uploader-1.0.7/LICENSE
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)      202 2023-05-21 21:16:36.661116 sftp_uploader-1.0.7/PKG-INFO
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)      408 2023-05-21 05:57:54.000000 sftp_uploader-1.0.7/README.md
+drwxr-xr-x   0 nikitakurkurin   (501) staff       (20)        0 2023-05-21 21:16:36.656075 sftp_uploader-1.0.7/docs/
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)       29 2023-05-20 08:08:28.000000 sftp_uploader-1.0.7/docs/__init__.py
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)      333 2023-05-21 21:16:09.000000 sftp_uploader-1.0.7/post_install.py
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)     1293 2023-05-21 21:02:12.000000 sftp_uploader-1.0.7/pyproject.toml
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)       38 2023-05-21 21:16:36.661323 sftp_uploader-1.0.7/setup.cfg
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)      407 2023-05-21 21:15:42.000000 sftp_uploader-1.0.7/setup.py
+drwxr-xr-x   0 nikitakurkurin   (501) staff       (20)        0 2023-05-21 21:16:36.656661 sftp_uploader-1.0.7/sftp_uploader/
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)      697 2023-05-21 12:50:31.000000 sftp_uploader-1.0.7/sftp_uploader/__init__.py
+drwxr-xr-x   0 nikitakurkurin   (501) staff       (20)        0 2023-05-21 21:16:36.660248 sftp_uploader-1.0.7/sftp_uploader/applications/
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)       42 2023-05-20 09:27:25.000000 sftp_uploader-1.0.7/sftp_uploader/applications/__init__.py
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)     2279 2023-05-20 14:10:57.000000 sftp_uploader-1.0.7/sftp_uploader/applications/dependency_container.py
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)     2135 2023-05-21 07:11:20.000000 sftp_uploader-1.0.7/sftp_uploader/applications/env_load.py
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)     4657 2023-05-21 12:37:31.000000 sftp_uploader-1.0.7/sftp_uploader/applications/git_manipulation.py
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)      705 2023-05-20 19:47:55.000000 sftp_uploader-1.0.7/sftp_uploader/applications/logs.py
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)      600 2023-05-21 12:44:39.000000 sftp_uploader-1.0.7/sftp_uploader/applications/pre_commit_actions.py
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)     4085 2023-05-21 07:19:21.000000 sftp_uploader-1.0.7/sftp_uploader/applications/sftp.py
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)     1442 2023-05-21 12:43:37.000000 sftp_uploader-1.0.7/sftp_uploader/applications/sftp_uploader.py
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)     2866 2023-05-20 13:41:17.000000 sftp_uploader-1.0.7/sftp_uploader/applications/ssh.py
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)      326 2023-05-21 21:00:53.000000 sftp_uploader-1.0.7/sftp_uploader/post_install.py
+drwxr-xr-x   0 nikitakurkurin   (501) staff       (20)        0 2023-05-21 21:16:36.660523 sftp_uploader-1.0.7/sftp_uploader/services/
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)       38 2023-05-20 09:27:08.000000 sftp_uploader-1.0.7/sftp_uploader/services/__init__.py
+drwxr-xr-x   0 nikitakurkurin   (501) staff       (20)        0 2023-05-21 21:16:36.657282 sftp_uploader-1.0.7/sftp_uploader.egg-info/
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)      202 2023-05-21 21:16:36.000000 sftp_uploader-1.0.7/sftp_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)      704 2023-05-21 21:16:36.000000 sftp_uploader-1.0.7/sftp_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)        1 2023-05-21 21:16:36.000000 sftp_uploader-1.0.7/sftp_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)       25 2023-05-21 21:16:36.000000 sftp_uploader-1.0.7/sftp_uploader.egg-info/top_level.txt
+drwxr-xr-x   0 nikitakurkurin   (501) staff       (20)        0 2023-05-21 21:16:36.660783 sftp_uploader-1.0.7/tests/
+-rw-r--r--   0 nikitakurkurin   (501) staff       (20)       26 2023-05-20 08:08:31.000000 sftp_uploader-1.0.7/tests/__init__.py
```

### Comparing `sftp_uploader-1.0.6/LICENSE` & `sftp_uploader-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.6/pyproject.toml` & `sftp_uploader-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.6/sftp_uploader/__init__.py` & `sftp_uploader-1.0.7/sftp_uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.6/sftp_uploader/applications/dependency_container.py` & `sftp_uploader-1.0.7/sftp_uploader/applications/dependency_container.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.6/sftp_uploader/applications/env_load.py` & `sftp_uploader-1.0.7/sftp_uploader/applications/env_load.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.6/sftp_uploader/applications/git_manipulation.py` & `sftp_uploader-1.0.7/sftp_uploader/applications/git_manipulation.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.6/sftp_uploader/applications/logs.py` & `sftp_uploader-1.0.7/sftp_uploader/applications/logs.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.6/sftp_uploader/applications/pre_commit_actions.py` & `sftp_uploader-1.0.7/sftp_uploader/applications/pre_commit_actions.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.6/sftp_uploader/applications/sftp.py` & `sftp_uploader-1.0.7/sftp_uploader/applications/sftp.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.6/sftp_uploader/applications/sftp_uploader.py` & `sftp_uploader-1.0.7/sftp_uploader/applications/sftp_uploader.py`

 * *Files identical despite different names*

### Comparing `sftp_uploader-1.0.6/sftp_uploader/applications/ssh.py` & `sftp_uploader-1.0.7/sftp_uploader/applications/ssh.py`

 * *Files identical despite different names*

