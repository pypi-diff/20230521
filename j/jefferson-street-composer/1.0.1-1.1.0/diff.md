# Comparing `tmp/jefferson-street-composer-1.0.1.tar.gz` & `tmp/jefferson-street-composer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jefferson-street-composer-1.0.1.tar", max compression
+gzip compressed data, was "jefferson-street-composer-1.1.0.tar", max compression
```

## Comparing `jefferson-street-composer-1.0.1.tar` & `jefferson-street-composer-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-04-19 00:26:26.692765 jefferson-street-composer-1.0.1/README.md
--rw-r--r--   0        0        0       99 2023-04-19 00:26:26.693182 jefferson-street-composer-1.0.1/jefferson_street_composer/__init__.py
--rw-r--r--   0        0        0      115 2023-04-19 00:26:26.693492 jefferson-street-composer-1.0.1/jefferson_street_composer/services/__init__.py
--rw-r--r--   0        0        0      131 2023-04-19 00:26:26.693835 jefferson-street-composer-1.0.1/jefferson_street_composer/services/specifications/__init__.py
--rw-r--r--   0        0        0     2360 2023-04-24 04:54:25.836326 jefferson-street-composer-1.0.1/jefferson_street_composer/services/specifications/base_ingest_dag.py
--rw-r--r--   0        0        0      526 2023-04-24 04:54:23.523340 jefferson-street-composer-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 jefferson-street-composer-1.0.1/setup.py
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 jefferson-street-composer-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-19 00:26:26.692765 jefferson-street-composer-1.1.0/README.md
+-rw-r--r--   0        0        0       99 2023-04-19 00:26:26.693182 jefferson-street-composer-1.1.0/jefferson_street_composer/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-19 00:26:26.693492 jefferson-street-composer-1.1.0/jefferson_street_composer/services/__init__.py
+-rw-r--r--   0        0        0      131 2023-04-19 00:26:26.693835 jefferson-street-composer-1.1.0/jefferson_street_composer/services/specifications/__init__.py
+-rw-r--r--   0        0        0     2089 2023-05-21 00:43:58.781144 jefferson-street-composer-1.1.0/jefferson_street_composer/services/specifications/base_ingest_dag.py
+-rw-r--r--   0        0        0      526 2023-05-21 00:49:54.344014 jefferson-street-composer-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 jefferson-street-composer-1.1.0/setup.py
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 jefferson-street-composer-1.1.0/PKG-INFO
```

### Comparing `jefferson-street-composer-1.0.1/jefferson_street_composer/services/specifications/base_ingest_dag.py` & `jefferson-street-composer-1.1.0/jefferson_street_composer/services/specifications/base_ingest_dag.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,29 +6,23 @@
 from airflow.providers.cncf.kubernetes.operators.kubernetes_pod import KubernetesPodOperator
 from airflow import DAG
 
 @dataclass
 class DagDefaultArgs():
     owner: str =  'Jefferson Street Technologies'
     description: str =  "Ingest DAG for Jefferson Street Technologies"
-    depends_on_past: bool =  False
-    start_date: datetime = datetime.now()
-    email_on_failure: bool =  False
-    email_on_retry: bool = False
+    start_date: datetime = datetime.utcnow()
     retries: int =  5
     retries_delay: timedelta = timedelta(minutes=2)
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "owner": self.owner,
             "description": self.description,
-            "depends_on_past": self.depends_on_past,
             "start_date": self.start_date,
-            "email_on_failure": self.email_on_failure,
-            "email_on_retry": self.email_on_retry,
             "retries": self.retries,
             "retries_delay": self.retries_delay,
         }
 
 class JeffersonStreetBaseIngestDag():
     def __init__(
         self,
@@ -51,15 +45,15 @@
     @property
     def image(self) -> str:
         return f"gcr.io/jefferson-street-cloud/ingests/{self.image_name}"
 
     def run(self):
         dag_default_args = DagDefaultArgs()
 
-        with DAG(self.name, default_args=dag_default_args.to_dict(), schedule_interval=self.schedule_interval, catchup=False) as dag:
+        with DAG(self.name, default_args=dag_default_args.to_dict(), schedule_interval='0 0 * * 0', catchup=False) as dag:
             t1 = BashOperator(task_id='print_start', bash_command='echo "start"')
 
             t2 = KubernetesPodOperator(
                 task_id=self.task_id,
                 name=self.name,
                 image=self.image,
                 namespace=self.namespace,
```

### Comparing `jefferson-street-composer-1.0.1/pyproject.toml` & `jefferson-street-composer-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jefferson-street-composer"
-version = "1.0.1"
+version = "1.1.0"
 description = "Library for Jefferson Street Technologies Composer Configuration"
 authors = ["Nikolai McFall <nikolai@jeffersonst.io>"]
 readme = "README.md"
 packages = [{include = "jefferson_street_composer"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `jefferson-street-composer-1.0.1/setup.py` & `jefferson-street-composer-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 install_requires = \
 ['apache-airflow-providers-cncf-kubernetes==5.0.0',
  'apache-airflow==2.4.3',
  'google-cloud-orchestration-airflow==1.4.1']
 
 setup_kwargs = {
     'name': 'jefferson-street-composer',
-    'version': '1.0.1',
+    'version': '1.1.0',
     'description': 'Library for Jefferson Street Technologies Composer Configuration',
     'long_description': '',
     'author': 'Nikolai McFall',
     'author_email': 'nikolai@jeffersonst.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `jefferson-street-composer-1.0.1/PKG-INFO` & `jefferson-street-composer-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jefferson-street-composer
-Version: 1.0.1
+Version: 1.1.0
 Summary: Library for Jefferson Street Technologies Composer Configuration
 Author: Nikolai McFall
 Author-email: nikolai@jeffersonst.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

