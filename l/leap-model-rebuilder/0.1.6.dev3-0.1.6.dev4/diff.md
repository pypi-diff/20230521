# Comparing `tmp/leap_model_rebuilder-0.1.6.dev3.tar.gz` & `tmp/leap_model_rebuilder-0.1.6.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_model_rebuilder-0.1.6.dev3.tar", max compression
+gzip compressed data, was "leap_model_rebuilder-0.1.6.dev4.tar", max compression
```

## Comparing `leap_model_rebuilder-0.1.6.dev3.tar` & `leap_model_rebuilder-0.1.6.dev4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2022-02-09 09:13:42.448536 leap_model_rebuilder-0.1.6.dev3/LICENSE
--rw-r--r--   0        0        0       88 2022-02-09 09:13:42.448767 leap_model_rebuilder-0.1.6.dev3/README.md
--rw-r--r--   0        0        0       51 2022-02-09 09:13:42.448923 leap_model_rebuilder-0.1.6.dev3/leap_model_rebuilder/__init__.py
--rw-r--r--   0        0        0     1430 2023-04-30 15:05:40.258520 leap_model_rebuilder-0.1.6.dev3/leap_model_rebuilder/api.py
--rw-r--r--   0        0        0     7049 2023-04-30 15:05:40.259255 leap_model_rebuilder-0.1.6.dev3/leap_model_rebuilder/modelexpander.py
--rw-r--r--   0        0        0     2037 2023-04-30 15:05:40.259907 leap_model_rebuilder-0.1.6.dev3/leap_model_rebuilder/utils.py
--rw-r--r--   0        0        0      905 2023-05-07 07:04:55.716843 leap_model_rebuilder-0.1.6.dev3/pyproject.toml
--rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 leap_model_rebuilder-0.1.6.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-02-09 09:13:42.448536 leap_model_rebuilder-0.1.6.dev4/LICENSE
+-rw-r--r--   0        0        0       88 2022-02-09 09:13:42.448767 leap_model_rebuilder-0.1.6.dev4/README.md
+-rw-r--r--   0        0        0       51 2022-02-09 09:13:42.448923 leap_model_rebuilder-0.1.6.dev4/leap_model_rebuilder/__init__.py
+-rw-r--r--   0        0        0     1430 2023-04-30 15:05:40.258520 leap_model_rebuilder-0.1.6.dev4/leap_model_rebuilder/api.py
+-rw-r--r--   0        0        0     7049 2023-04-30 15:05:40.259255 leap_model_rebuilder-0.1.6.dev4/leap_model_rebuilder/modelexpander.py
+-rw-r--r--   0        0        0     2037 2023-04-30 15:05:40.259907 leap_model_rebuilder-0.1.6.dev4/leap_model_rebuilder/utils.py
+-rw-r--r--   0        0        0      904 2023-05-21 12:59:57.607851 leap_model_rebuilder-0.1.6.dev4/pyproject.toml
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 leap_model_rebuilder-0.1.6.dev4/PKG-INFO
```

### Comparing `leap_model_rebuilder-0.1.6.dev3/LICENSE` & `leap_model_rebuilder-0.1.6.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_model_rebuilder-0.1.6.dev3/leap_model_rebuilder/api.py` & `leap_model_rebuilder-0.1.6.dev4/leap_model_rebuilder/api.py`

 * *Files identical despite different names*

### Comparing `leap_model_rebuilder-0.1.6.dev3/leap_model_rebuilder/modelexpander.py` & `leap_model_rebuilder-0.1.6.dev4/leap_model_rebuilder/modelexpander.py`

 * *Files identical despite different names*

### Comparing `leap_model_rebuilder-0.1.6.dev3/leap_model_rebuilder/utils.py` & `leap_model_rebuilder-0.1.6.dev4/leap_model_rebuilder/utils.py`

 * *Files identical despite different names*

### Comparing `leap_model_rebuilder-0.1.6.dev3/pyproject.toml` & `leap_model_rebuilder-0.1.6.dev4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 [tool.poetry]
 name = "leap-model-rebuilder"
-version = "0.1.6.dev3"
+version = "0.1.6.dev4"
 description = ""
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/leap-model-rebuilder"
 homepage = "https://github.com/tensorleap/leap-model-rebuilder"
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
-protobuf = "^4.21.0"
+protobuf = "3.20.3"
 tensorflow = {version = "2.12.0", markers = "platform_machine  == 'x86_64'"}
 tensorflow-macos = {version = "2.12.0", markers = "platform_machine  == 'arm64'"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 grappa = "^1.0.1"
 pylint-pytest = "^1.1.2"
```

### Comparing `leap_model_rebuilder-0.1.6.dev3/PKG-INFO` & `leap_model_rebuilder-0.1.6.dev4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: leap-model-rebuilder
-Version: 0.1.6.dev3
+Version: 0.1.6.dev4
 Summary: 
 Home-page: https://github.com/tensorleap/leap-model-rebuilder
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: protobuf (>=4.21.0,<5.0.0)
+Requires-Dist: protobuf (==3.20.3)
 Requires-Dist: tensorflow (==2.12.0) ; platform_machine == "x86_64"
 Requires-Dist: tensorflow-macos (==2.12.0) ; platform_machine == "arm64"
 Project-URL: Repository, https://github.com/tensorleap/leap-model-rebuilder
 Description-Content-Type: text/markdown
 
 # leap-model-rebuilder
 Keras model rebuilder tool for model rebuilding with alterations
```

