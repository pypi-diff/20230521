# Comparing `tmp/longalpha_utils-0.48.tar.gz` & `tmp/longalpha_utils-0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.48.tar", last modified: Sat May 20 19:58:30 2023, max compression
+gzip compressed data, was "longalpha_utils-0.49.tar", last modified: Sun May 21 00:14:52 2023, max compression
```

## Comparing `longalpha_utils-0.48.tar` & `longalpha_utils-0.49.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:58:30.236262 longalpha_utils-0.48/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 19:58:30.236262 longalpha_utils-0.48/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:58:30.236262 longalpha_utils-0.48/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-20 19:58:16.000000 longalpha_utils-0.48/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-20 19:58:16.000000 longalpha_utils-0.48/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-20 19:58:16.000000 longalpha_utils-0.48/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-05-20 19:58:16.000000 longalpha_utils-0.48/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-20 19:58:16.000000 longalpha_utils-0.48/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-20 19:58:16.000000 longalpha_utils-0.48/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 19:58:30.236262 longalpha_utils-0.48/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 19:58:30.000000 longalpha_utils-0.48/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-20 19:58:30.000000 longalpha_utils-0.48/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 19:58:30.000000 longalpha_utils-0.48/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-20 19:58:30.000000 longalpha_utils-0.48/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 19:58:30.000000 longalpha_utils-0.48/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 19:58:30.236262 longalpha_utils-0.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-20 19:58:16.000000 longalpha_utils-0.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:14:52.805338 longalpha_utils-0.49/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-21 00:14:52.805338 longalpha_utils-0.49/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:14:52.805338 longalpha_utils-0.49/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-21 00:14:42.000000 longalpha_utils-0.49/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 00:14:42.000000 longalpha_utils-0.49/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-21 00:14:42.000000 longalpha_utils-0.49/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-21 00:14:42.000000 longalpha_utils-0.49/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-21 00:14:42.000000 longalpha_utils-0.49/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-21 00:14:42.000000 longalpha_utils-0.49/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:14:52.805338 longalpha_utils-0.49/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-21 00:14:52.000000 longalpha_utils-0.49/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-21 00:14:52.000000 longalpha_utils-0.49/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:14:52.000000 longalpha_utils-0.49/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-21 00:14:52.000000 longalpha_utils-0.49/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-21 00:14:52.000000 longalpha_utils-0.49/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:14:52.805338 longalpha_utils-0.49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-21 00:14:42.000000 longalpha_utils-0.49/setup.py
```

### Comparing `longalpha_utils-0.48/longalpha_utils/messenger.py` & `longalpha_utils-0.49/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.48/longalpha_utils/transfers.py` & `longalpha_utils-0.49/longalpha_utils/transfers.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 from pyspark.sql import SparkSession, DataFrame
 from sqlalchemy import Engine
 from sqlalchemy import create_engine
 from sqlalchemy import text
 from minio.error import S3Error
 from datetime import date, timedelta
 from pyspark.sql.utils import AnalysisException
-from longalpha_utils.utils import  multi_union_by_name
+from longalpha_utils.utils import multi_union_by_name
+from tqdm import tqdm
+
+
 def init_spark(
     spark_executor_memory: str = "30g",
     spark_driver_memory: str = "90g",
     minio_endpoint: Optional[str] = None,
     minio_access_key: Optional[str] = None,
     minio_secret_key: Optional[str] = None,
 ) -> SparkSession:
@@ -62,14 +65,15 @@
         spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.endpoint", minio_endpoint)
         spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.access.key", minio_access_key)
         spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.secret.key", minio_secret_key)
         spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.connection.ssl.enabled", "false")
 
     return spark
 
+
 class MinioWrapper:
     def __init__(self, minio_url, minio_access_key, minio_secret_key):
         self.minio_client = Minio(
             endpoint=minio_url,
             access_key=minio_access_key,
             secret_key=minio_secret_key,
             secure=False,
@@ -172,43 +176,58 @@
         latest_obj = time_obj[latest_time]
         return self.get(bucket_name=bucket_name, object_name=latest_obj.object_name)
 
     def list(self, bucket_name: str) -> List[str]:
         return [i.object_name for i in self.minio_client.list_objects(bucket_name)]
 
 
-
-
 def get_s3_data_spark(
-        spark: SparkSession, start_date: date, end_date: date, bucket: str, subfolder: str,
+    spark: SparkSession,
+    start_date: date,
+    end_date: date,
+    bucket: str,
+    subfolder: str,
+    show_missing_dates: bool = False,
+    progress_bar: bool = True,
 ) -> Union[DataFrame, None]:
     """
     Get data from s3 for a given date range
     Args:
         spark: spark session
         start_date: start date to get options data for
         end_date: end date to get options data for
+        bucket: s3 bucket name
+        subfolder: subfolder in the s3 bucket
+        show_missing_dates: whether to print out missing dates
+        progress_bar: whether to show a progress bar
 
     Returns: a spark dataframe if data exists, None otherwise
 
     """
-    options = []
+    dates = []
     while start_date <= end_date:
-        file_s3_path = "s3a://" +os.path.join(bucket, f"{subfolder}/{start_date}.parquet")
+        dates.append(start_date)
+        start_date += timedelta(days=1)
+    if progress_bar:
+        dates = tqdm(dates)
+
+    options = []
+    for day in dates:
+        file_s3_path = "s3a://" + os.path.join(bucket, f"{subfolder}/{day}.parquet")
         try:
             option = spark.read.parquet(file_s3_path)
             options.append(option)
         except AnalysisException:
-            print(f"Options data for {start_date} does not exist.")
-        start_date += timedelta(days=1)
+            if show_missing_dates:
+                print(f"Options data for {start_date} does not exist.")
+            else:
+                pass
     if len(options) == 0:
         return None
-    unioned_options = multi_union_by_name(options)
-    return unioned_options
-
+    return multi_union_by_name(options)
 
 
 def spark_read_psql(
     spark: SparkSession, psql_url: str, psql_db: str, psql_table: str, psql_usr: str, psql_pwd: str
 ) -> DataFrame:
     """
     use spark to read psql
```

### Comparing `longalpha_utils-0.48/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.49/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.48/longalpha_utils/utils.py` & `longalpha_utils-0.49/longalpha_utils/utils.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.48/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.49/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.48/setup.py` & `longalpha_utils-0.49/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.48",
+    version="0.49",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

