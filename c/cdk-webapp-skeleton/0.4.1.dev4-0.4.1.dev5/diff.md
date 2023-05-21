# Comparing `tmp/cdk_webapp_skeleton-0.4.1.dev4.tar.gz` & `tmp/cdk_webapp_skeleton-0.4.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_webapp_skeleton-0.4.1.dev4.tar", max compression
+gzip compressed data, was "cdk_webapp_skeleton-0.4.1.dev5.tar", max compression
```

## Comparing `cdk_webapp_skeleton-0.4.1.dev4.tar` & `cdk_webapp_skeleton-0.4.1.dev5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       64 2023-05-13 19:40:31.358782 cdk_webapp_skeleton-0.4.1.dev4/README.md
--rw-r--r--   0        0        0      449 2023-05-13 19:40:31.358782 cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/__init__.py
--rw-r--r--   0        0        0     3546 2023-05-13 19:40:31.358782 cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/auth_stack.py
--rw-r--r--   0        0        0     2159 2023-05-13 19:40:31.358782 cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/branch_cicd_pipeline.py
--rw-r--r--   0        0        0     2089 2023-05-13 19:40:31.358782 cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/branch_config.py
--rw-r--r--   0        0        0     3621 2023-05-13 19:40:31.358782 cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/monitored_lambda_function.py
--rw-r--r--   0        0        0     4725 2023-05-13 19:40:31.358782 cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/react_website.py
--rw-r--r--   0        0        0      344 2023-05-13 19:40:31.358782 cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/test_utils.py
--rw-r--r--   0        0        0     4466 2023-05-13 19:40:31.358782 cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/webapp_lambda.py
--rw-r--r--   0        0        0     1473 2023-05-13 19:40:58.083210 cdk_webapp_skeleton-0.4.1.dev4/pyproject.toml
--rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.4.1.dev4/PKG-INFO
+-rw-r--r--   0        0        0       64 2023-05-21 02:33:44.287497 cdk_webapp_skeleton-0.4.1.dev5/README.md
+-rw-r--r--   0        0        0      449 2023-05-21 02:33:44.287497 cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/__init__.py
+-rw-r--r--   0        0        0     3546 2023-05-21 02:33:44.287497 cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/auth_stack.py
+-rw-r--r--   0        0        0     2393 2023-05-21 02:33:44.287497 cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/branch_cicd_pipeline.py
+-rw-r--r--   0        0        0     2089 2023-05-21 02:33:44.287497 cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/branch_config.py
+-rw-r--r--   0        0        0     3621 2023-05-21 02:33:44.287497 cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/monitored_lambda_function.py
+-rw-r--r--   0        0        0     4725 2023-05-21 02:33:44.287497 cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/react_website.py
+-rw-r--r--   0        0        0      344 2023-05-21 02:33:44.287497 cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/test_utils.py
+-rw-r--r--   0        0        0     4466 2023-05-21 02:33:44.287497 cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/webapp_lambda.py
+-rw-r--r--   0        0        0     1473 2023-05-21 02:34:06.727686 cdk_webapp_skeleton-0.4.1.dev5/pyproject.toml
+-rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.4.1.dev5/PKG-INFO
```

### Comparing `cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/auth_stack.py` & `cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/auth_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/branch_cicd_pipeline.py` & `cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/branch_cicd_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,27 +17,35 @@
         cache_bucket = s3.Bucket(
             scope,
             "CacheBucket",
             removal_policy=cdk.RemovalPolicy.DESTROY,
             auto_delete_objects=True,
         )
 
+        artifact_bucket = s3.Bucket(
+            scope,
+            "ArtifactBucket",
+            removal_policy=cdk.RemovalPolicy.DESTROY,
+            auto_delete_objects=True,
+        )
+
         synth_step = pipelines.ShellStep(
             "Synth",
             input=branch_config.source,
             env={
                 "BRANCH": branch_config.branch_name,
             },
             commands=["./synth.sh"],
         )
 
         self.cdk_pipeline = pipelines.CodePipeline(
             scope,
             "Pipeline",  # Pipeline name gets the stack name prepended
             synth=synth_step,
+            artifact_bucket=artifact_bucket,
             code_build_defaults=pipelines.CodeBuildOptions(
                 build_environment=codebuild.BuildEnvironment(
                     compute_type=codebuild.ComputeType.SMALL
                 ),
                 cache=codebuild.Cache.bucket(cache_bucket),
             ),
             cross_account_keys=False,
```

### Comparing `cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/branch_config.py` & `cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/branch_config.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/monitored_lambda_function.py` & `cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/monitored_lambda_function.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/react_website.py` & `cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/react_website.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.4.1.dev4/cdk_webapp_skeleton/webapp_lambda.py` & `cdk_webapp_skeleton-0.4.1.dev5/cdk_webapp_skeleton/webapp_lambda.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.4.1.dev4/pyproject.toml` & `cdk_webapp_skeleton-0.4.1.dev5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdk-webapp-skeleton"
-version = "0.4.1.dev4"
+version = "0.4.1.dev5"
 description = ""
 authors = ["Ilya Nekhay <nekhayiv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cdk_webapp_skeleton"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `cdk_webapp_skeleton-0.4.1.dev4/PKG-INFO` & `cdk_webapp_skeleton-0.4.1.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-webapp-skeleton
-Version: 0.4.1.dev4
+Version: 0.4.1.dev5
 Summary: 
 Author: Ilya Nekhay
 Author-email: nekhayiv@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

