# Comparing `tmp/pyjaws-0.1.2.tar.gz` & `tmp/pyjaws-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjaws-0.1.2.tar", last modified: Fri May 19 08:09:33 2023, max compression
+gzip compressed data, was "pyjaws-0.1.3.tar", last modified: Sun May 21 14:07:33 2023, max compression
```

## Comparing `pyjaws-0.1.2.tar` & `pyjaws-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.412507 pyjaws-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-19 08:09:33.412507 pyjaws-0.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.408507 pyjaws-0.1.2/pyjaws/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.412507 pyjaws-0.1.2/pyjaws/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.412507 pyjaws-0.1.2/pyjaws/api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.412507 pyjaws-0.1.2/pyjaws/api/templates/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/templates/macros/cluster.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/templates/macros/task.j2
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/api/templates/workflow.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.412507 pyjaws-0.1.2/pyjaws/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyjaws/client/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:09:33.408507 pyjaws-0.1.2/pyjaws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-19 08:09:33.000000 pyjaws-0.1.2/pyjaws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-19 08:09:33.000000 pyjaws-0.1.2/pyjaws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 08:09:33.000000 pyjaws-0.1.2/pyjaws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 08:09:33.000000 pyjaws-0.1.2/pyjaws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-19 08:09:33.000000 pyjaws-0.1.2/pyjaws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 08:09:33.000000 pyjaws-0.1.2/pyjaws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-19 08:09:24.000000 pyjaws-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 08:09:33.412507 pyjaws-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-19 08:09:24.000000 pyjaws-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:07:33.894963 pyjaws-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-21 14:07:33.894963 pyjaws-0.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:07:33.894963 pyjaws-0.1.3/pyjaws/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-21 14:07:19.000000 pyjaws-0.1.3/pyjaws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:07:33.894963 pyjaws-0.1.3/pyjaws/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:07:19.000000 pyjaws-0.1.3/pyjaws/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-21 14:07:19.000000 pyjaws-0.1.3/pyjaws/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-21 14:07:19.000000 pyjaws-0.1.3/pyjaws/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-21 14:07:19.000000 pyjaws-0.1.3/pyjaws/api/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-21 14:07:19.000000 pyjaws-0.1.3/pyjaws/api/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:07:33.894963 pyjaws-0.1.3/pyjaws/api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:07:33.894963 pyjaws-0.1.3/pyjaws/api/templates/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-21 14:07:19.000000 pyjaws-0.1.3/pyjaws/api/templates/macros/cluster.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-21 14:07:19.000000 pyjaws-0.1.3/pyjaws/api/templates/macros/task.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-21 14:07:19.000000 pyjaws-0.1.3/pyjaws/api/templates/workflow.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:07:33.894963 pyjaws-0.1.3/pyjaws/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 14:07:19.000000 pyjaws-0.1.3/pyjaws/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-21 14:07:19.000000 pyjaws-0.1.3/pyjaws/client/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:07:33.894963 pyjaws-0.1.3/pyjaws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-21 14:07:33.000000 pyjaws-0.1.3/pyjaws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-21 14:07:33.000000 pyjaws-0.1.3/pyjaws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:07:33.000000 pyjaws-0.1.3/pyjaws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-21 14:07:33.000000 pyjaws-0.1.3/pyjaws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-21 14:07:33.000000 pyjaws-0.1.3/pyjaws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 14:07:33.000000 pyjaws-0.1.3/pyjaws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-21 14:07:19.000000 pyjaws-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 14:07:33.894963 pyjaws-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-21 14:07:19.000000 pyjaws-0.1.3/setup.py
```

### Comparing `pyjaws-0.1.2/PKG-INFO` & `pyjaws-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyjaws
-Version: 0.1.2
+Version: 0.1.3
 Author: Rafael Pierre
 Description-Content-Type: text/markdown
 
 # PyJaws: A Pythonic Way to Define Databricks Jobs and Workflows
 
 <p align="center">
         <img src="https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/pyjaws.png" class="align-center" />
     </a>
 </p>
 
 <hr />
 
-[![pypi](https://img.shields.io/badge/pypi-0.1.1-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
+[![pypi](https://img.shields.io/badge/pypi-0.1.2-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black) ![downloads](https://img.shields.io/pypi/dm/pyjaws?style=for-the-badge)
 
 <hr />
 
 * **PyJaws** enables declaring [Databricks Jobs and Workflows](https://docs.databricks.com/workflows/index.html) as Python code, allowing for:
   * Code Linting
   * Formatting
   * Parameter Validation
@@ -116,17 +116,50 @@
 
 workflow = Workflow(
     name = "my_workflow",
     tasks = [ingest_task, transform_task]
 )
 ```
 
-### Sample Results
+### Extra Features
 
-Running `pyjaws create examples/simple_workflow` will result in the following Workflow being deployed to Databricks:
+* **Context Manager** for **Cluster** declarations:
+
+```python
+# cluster created with context manager
+with Cluster(
+    job_cluster_key="mycluster_2",
+    spark_version=Runtime.DBR_13_ML,
+    node_type_id="Standard_E4ds_v4",
+    num_workers=3,
+) as cluster_2:
+    task_2 = SparkPythonTask(
+        key="task_2",
+        cluster=cluster_2,
+        python_file="/Workspace/Repos/bob@mail.com/utils/task_2.py",
+        source=Source.WORKSPACE,
+    )
+```
+
+* **Workflow preview/visualization** on notebooks:
+
+```python
+display(workflow)
+```
+Result:
+
+![preview](https://github.com/rafaelpierre/pyjaws/blob/main/img/preview.png?raw=true "Preview")
+
+## Deploying Jobs
+
+If you have a folder containing multiple workflow definition files written in Python with **PyJaws**, it is quite simple to deploy all of them to your Databricks Workspace with a one liner:
+
+`pyjaws create examples/simple_workflow`
+
+This would result in the following Workflow being deployed to your workspace:
 
 ![workflow](https://github.com/rafaelpierre/pyjaws/blob/main/img/workflow.png?raw=true "Workflow")
 
 By default, **pyjaws** also includes some useful tags into the workflows indicating which Git Repo hosts the Python definition, commit hash and when the workflow was last updated. For example:
 
 ![workflow](https://github.com/rafaelpierre/pyjaws/blob/main/img/tags.png?raw=true "Workflow")
```

### Comparing `pyjaws-0.1.2/pyjaws/api/base.py` & `pyjaws-0.1.3/pyjaws/api/base.py`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.2/pyjaws/api/jobs.py` & `pyjaws-0.1.3/pyjaws/api/jobs.py`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.2/pyjaws/api/tasks.py` & `pyjaws-0.1.3/pyjaws/api/tasks.py`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.2/pyjaws/api/templates/macros/cluster.j2` & `pyjaws-0.1.3/pyjaws/api/templates/macros/cluster.j2`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.2/pyjaws/api/templates/macros/task.j2` & `pyjaws-0.1.3/pyjaws/api/templates/macros/task.j2`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.2/pyjaws/api/templates/workflow.j2` & `pyjaws-0.1.3/pyjaws/api/templates/workflow.j2`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.2/pyjaws/client/entrypoint.py` & `pyjaws-0.1.3/pyjaws/client/entrypoint.py`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.2/pyjaws.egg-info/PKG-INFO` & `pyjaws-0.1.3/pyjaws.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyjaws
-Version: 0.1.2
+Version: 0.1.3
 Author: Rafael Pierre
 Description-Content-Type: text/markdown
 
 # PyJaws: A Pythonic Way to Define Databricks Jobs and Workflows
 
 <p align="center">
         <img src="https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/pyjaws.png" class="align-center" />
     </a>
 </p>
 
 <hr />
 
-[![pypi](https://img.shields.io/badge/pypi-0.1.1-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black)
+[![pypi](https://img.shields.io/badge/pypi-0.1.2-brightgreen?style=for-the-badge)](https://pypi.org/project/pyjaws/) ![black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge) ![ruff](https://img.shields.io/badge/lint-ruff-gold?style=for-the-badge) ![cov](https://raw.githubusercontent.com/rafaelpierre/pyjaws/main/img/coverage.svg) ![databricks](https://img.shields.io/badge/Databricks-FF3621.svg?style=for-the-badge&logo=Databricks&logoColor=white) ![Jinja](https://img.shields.io/badge/jinja-white.svg?style=for-the-badge&logo=jinja&logoColor=black) ![downloads](https://img.shields.io/pypi/dm/pyjaws?style=for-the-badge)
 
 <hr />
 
 * **PyJaws** enables declaring [Databricks Jobs and Workflows](https://docs.databricks.com/workflows/index.html) as Python code, allowing for:
   * Code Linting
   * Formatting
   * Parameter Validation
@@ -116,17 +116,50 @@
 
 workflow = Workflow(
     name = "my_workflow",
     tasks = [ingest_task, transform_task]
 )
 ```
 
-### Sample Results
+### Extra Features
 
-Running `pyjaws create examples/simple_workflow` will result in the following Workflow being deployed to Databricks:
+* **Context Manager** for **Cluster** declarations:
+
+```python
+# cluster created with context manager
+with Cluster(
+    job_cluster_key="mycluster_2",
+    spark_version=Runtime.DBR_13_ML,
+    node_type_id="Standard_E4ds_v4",
+    num_workers=3,
+) as cluster_2:
+    task_2 = SparkPythonTask(
+        key="task_2",
+        cluster=cluster_2,
+        python_file="/Workspace/Repos/bob@mail.com/utils/task_2.py",
+        source=Source.WORKSPACE,
+    )
+```
+
+* **Workflow preview/visualization** on notebooks:
+
+```python
+display(workflow)
+```
+Result:
+
+![preview](https://github.com/rafaelpierre/pyjaws/blob/main/img/preview.png?raw=true "Preview")
+
+## Deploying Jobs
+
+If you have a folder containing multiple workflow definition files written in Python with **PyJaws**, it is quite simple to deploy all of them to your Databricks Workspace with a one liner:
+
+`pyjaws create examples/simple_workflow`
+
+This would result in the following Workflow being deployed to your workspace:
 
 ![workflow](https://github.com/rafaelpierre/pyjaws/blob/main/img/workflow.png?raw=true "Workflow")
 
 By default, **pyjaws** also includes some useful tags into the workflows indicating which Git Repo hosts the Python definition, commit hash and when the workflow was last updated. For example:
 
 ![workflow](https://github.com/rafaelpierre/pyjaws/blob/main/img/tags.png?raw=true "Workflow")
```

### Comparing `pyjaws-0.1.2/pyproject.toml` & `pyjaws-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjaws-0.1.2/setup.py` & `pyjaws-0.1.3/setup.py`

 * *Files identical despite different names*

