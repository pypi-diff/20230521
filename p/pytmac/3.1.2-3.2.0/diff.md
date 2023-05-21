# Comparing `tmp/pytmac-3.1.2.tar.gz` & `tmp/pytmac-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytmac-3.1.2.tar", last modified: Tue May 16 20:26:27 2023, max compression
+gzip compressed data, was "pytmac-3.2.0.tar", last modified: Sun May 21 09:51:11 2023, max compression
```

## Comparing `pytmac-3.1.2.tar` & `pytmac-3.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:26:27.930061 pytmac-3.1.2/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-05-16 20:26:24.000000 pytmac-3.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5018 2023-05-16 20:26:27.930061 pytmac-3.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4905 2023-05-16 20:26:24.000000 pytmac-3.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 20:26:25.000000 pytmac-3.1.2/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:26:27.930061 pytmac-3.1.2/bin/
--rw-r--r--   0 root         (0) root         (0)     2719 2023-05-16 20:26:24.000000 pytmac-3.1.2/bin/get_config.py
--rw-r--r--   0 root         (0) root         (0)     6326 2023-05-16 20:26:24.000000 pytmac-3.1.2/bin/input_validator.py
--rw-r--r--   0 root         (0) root         (0)     2766 2023-05-16 20:26:24.000000 pytmac-3.1.2/bin/resource_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:26:27.930061 pytmac-3.1.2/docs/
--rw-r--r--   0 root         (0) root         (0)      241 2023-05-16 20:26:24.000000 pytmac-3.1.2/docs/config.yaml
--rw-r--r--   0 root         (0) root         (0)     2089 2023-05-16 20:26:24.000000 pytmac-3.1.2/docs/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-16 20:26:24.000000 pytmac-3.1.2/docs/resources.yaml
--rw-r--r--   0 root         (0) root         (0)     7555 2023-05-16 20:26:24.000000 pytmac-3.1.2/docs/security_checks.yaml
--rw-r--r--   0 root         (0) root         (0)     1474 2023-05-16 20:26:24.000000 pytmac-3.1.2/docs/swagger.json
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-16 20:26:24.000000 pytmac-3.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)    18768 2023-05-16 20:26:27.000000 pytmac-3.1.2/pytmac
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:26:27.930061 pytmac-3.1.2/pytmac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5018 2023-05-16 20:26:27.000000 pytmac-3.1.2/pytmac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-16 20:26:27.000000 pytmac-3.1.2/pytmac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 20:26:27.000000 pytmac-3.1.2/pytmac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-16 20:26:27.000000 pytmac-3.1.2/pytmac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 20:26:27.000000 pytmac-3.1.2/pytmac.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 20:26:27.930061 pytmac-3.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      868 2023-05-16 20:26:24.000000 pytmac-3.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 09:51:11.212516 pytmac-3.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-21 09:51:08.000000 pytmac-3.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5233 2023-05-21 09:51:11.212516 pytmac-3.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5120 2023-05-21 09:51:08.000000 pytmac-3.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-21 09:51:09.000000 pytmac-3.2.0/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 09:51:11.208516 pytmac-3.2.0/bin/
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-05-21 09:51:08.000000 pytmac-3.2.0/bin/get_config.py
+-rw-r--r--   0 root         (0) root         (0)     6326 2023-05-21 09:51:08.000000 pytmac-3.2.0/bin/input_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-05-21 09:51:08.000000 pytmac-3.2.0/bin/resource_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 09:51:11.208516 pytmac-3.2.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-05-21 09:51:08.000000 pytmac-3.2.0/docs/config.yaml
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-05-21 09:51:08.000000 pytmac-3.2.0/docs/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-21 09:51:08.000000 pytmac-3.2.0/docs/resources.yaml
+-rw-r--r--   0 root         (0) root         (0)     7555 2023-05-21 09:51:08.000000 pytmac-3.2.0/docs/security_checks.yaml
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-05-21 09:51:08.000000 pytmac-3.2.0/docs/swagger.json
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-21 09:51:08.000000 pytmac-3.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-05-21 09:51:11.000000 pytmac-3.2.0/pytmac
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 09:51:11.212516 pytmac-3.2.0/pytmac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5233 2023-05-21 09:51:11.000000 pytmac-3.2.0/pytmac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-21 09:51:11.000000 pytmac-3.2.0/pytmac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 09:51:11.000000 pytmac-3.2.0/pytmac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-21 09:51:11.000000 pytmac-3.2.0/pytmac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-21 09:51:11.000000 pytmac-3.2.0/pytmac.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 09:51:11.212516 pytmac-3.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      868 2023-05-21 09:51:08.000000 pytmac-3.2.0/setup.py
```

### Comparing `pytmac-3.1.2/LICENSE` & `pytmac-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.2/PKG-INFO` & `pytmac-3.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: pytmac
-Version: 3.1.2
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
 ![Workflow Unit Tests](https://github.com/tjtharrison/pytmac/actions/workflows/pr-tests.yaml/badge.svg)
 ![Workflow CodeQL](https://github.com/tjtharrison/pytmac/actions/workflows/pr-codeql.yaml/badge.svg)
 
@@ -21,17 +15,19 @@
 Python based threat modelling as code tool (Python T.M.A.C).
 
 # Installation
 
 pytmac is available via PyPi, and can be installed with pip:
 
 ```
-pip install pytmac
+pip3 install pytmac
 ```
 
+In order for DFD diagrams to be generated, [plantuml](https://plantuml.com/) must be installed on the system. If it is not installed, pytmac will continue to execute but the output will not include a DFD diagram.
+
 # Usage
 
 Once installed, pytmac can be called from the command line with an array of arguments which are described in the help page:
 
 ```
 pytmac --help
```

### Comparing `pytmac-3.1.2/README.md` & `pytmac-3.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: pytmac
+Version: 3.2.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
 ![Workflow Unit Tests](https://github.com/tjtharrison/pytmac/actions/workflows/pr-tests.yaml/badge.svg)
 ![Workflow CodeQL](https://github.com/tjtharrison/pytmac/actions/workflows/pr-codeql.yaml/badge.svg)
 
@@ -15,17 +21,19 @@
 Python based threat modelling as code tool (Python T.M.A.C).
 
 # Installation
 
 pytmac is available via PyPi, and can be installed with pip:
 
 ```
-pip install pytmac
+pip3 install pytmac
 ```
 
+In order for DFD diagrams to be generated, [plantuml](https://plantuml.com/) must be installed on the system. If it is not installed, pytmac will continue to execute but the output will not include a DFD diagram.
+
 # Usage
 
 Once installed, pytmac can be called from the command line with an array of arguments which are described in the help page:
 
 ```
 pytmac --help
```

### Comparing `pytmac-3.1.2/bin/get_config.py` & `pytmac-3.2.0/bin/get_config.py`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.2/bin/input_validator.py` & `pytmac-3.2.0/bin/input_validator.py`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.2/bin/resource_validator.py` & `pytmac-3.2.0/bin/resource_validator.py`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.2/docs/defaults.yaml` & `pytmac-3.2.0/docs/defaults.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.2/docs/resources.yaml` & `pytmac-3.2.0/docs/resources.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.2/docs/security_checks.yaml` & `pytmac-3.2.0/docs/security_checks.yaml`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.2/docs/swagger.json` & `pytmac-3.2.0/docs/swagger.json`

 * *Files identical despite different names*

### Comparing `pytmac-3.1.2/pytmac` & `pytmac-3.2.0/pytmac`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 Python based programmatic threat modelling tool tmacs
 """
 import argparse
 import json
 import logging
 import os
+import subprocess
 import sys
 from copy import deepcopy
 from datetime import date
 
 import yaml
 
 from _version import __version__
@@ -158,14 +159,25 @@
                 elif isinstance(
                     resources_yaml["resources"][config_yaml["swagger_resource_type"]],
                     list,
                 ):
                     resources_yaml["resources"][
                         config_yaml["swagger_resource_type"]
                     ].append(swagger_path_detail)
+
+    # Check if plantuml is callable
+    try:
+        # Check if plantuml executable is available
+        subprocess.run(["plantuml", "-version"], stdout=subprocess.DEVNULL)
+        logging.info("Plantuml executable found, will generate diagrams")
+        plantuml_available = True
+    except FileNotFoundError:
+        plantuml_available = False
+        logging.error("Plantuml executable not found, unable to generate diagram")
+
     output_file_dir = output_dir
     output_file_name = "report-" + str(date.today())
 
     with open(
         output_file_dir + "/" + output_file_name + ".md", "w+", encoding="UTF-8"
     ) as output_file:
         # Build out json report
@@ -380,15 +392,16 @@
                     + res_links["description"]
                     + '")'
                     + "\n"
                 )
             output_file.write("@enduml\n")
             output_file.write("```\n")
             output_file.write("\n")
-            output_file.write("![Diagram](./" + output_file_name + ".svg)")
+            if plantuml_available:
+                output_file.write("![Diagram](./" + output_file_name + ".svg)")
 
             # Print final json
             yaml.dump(output_yaml_report, output_yaml)
 
             # Insecure resources
             insecure_resources = resource_validator.main(
                 security_checks_yaml, output_yaml_report
@@ -414,14 +427,23 @@
                         + response["check_query"]
                         + " | "
                         + str(response["severity"])
                         + " | "
                         + "\n"
                     )
                     output_file.write(response_detail)
+
+    if plantuml_available:
+        # Generate diagram
+        subprocess.run(
+            ["plantuml", "-tsvg", output_file_name + ".md"],
+            stdout=subprocess.DEVNULL,
+        )
+        logging.info("DFD diagram generated")
+
     return True
 
 
 if __name__ == "__main__":
     if args.version:
         print(VERSION)
     elif args.demo:
```

### Comparing `pytmac-3.1.2/pytmac.egg-info/PKG-INFO` & `pytmac-3.2.0/pytmac.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmac
-Version: 3.1.2
+Version: 3.2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B37707%2Fgit%40github.com%3Atjtharrison%2Ftmac.git?ref=badge_shield)
 ![Workflow Actionlint](https://github.com/tjtharrison/pytmac/actions/workflows/pr-actionlint.yaml/badge.svg)
 ![Workflow Checkov](https://github.com/tjtharrison/pytmac/actions/workflows/pr-checkov.yaml/badge.svg)
 ![Workflow Linting](https://github.com/tjtharrison/pytmac/actions/workflows/pr-linting.yaml/badge.svg)
@@ -21,17 +21,19 @@
 Python based threat modelling as code tool (Python T.M.A.C).
 
 # Installation
 
 pytmac is available via PyPi, and can be installed with pip:
 
 ```
-pip install pytmac
+pip3 install pytmac
 ```
 
+In order for DFD diagrams to be generated, [plantuml](https://plantuml.com/) must be installed on the system. If it is not installed, pytmac will continue to execute but the output will not include a DFD diagram.
+
 # Usage
 
 Once installed, pytmac can be called from the command line with an array of arguments which are described in the help page:
 
 ```
 pytmac --help
```

### Comparing `pytmac-3.1.2/setup.py` & `pytmac-3.2.0/setup.py`

 * *Files identical despite different names*

