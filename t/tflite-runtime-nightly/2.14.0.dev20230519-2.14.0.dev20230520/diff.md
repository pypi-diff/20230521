# Comparing `tmp/tflite_runtime_nightly-2.14.0.dev20230519-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/tflite_runtime_nightly-2.14.0.dev20230520-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 2396297 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-May-20 04:51 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  6814248 b- defN 23-May-20 04:53 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-May-20 04:51 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-May-20 04:51 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-May-20 04:51 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-May-20 04:53 tflite_runtime_nightly-2.14.0.dev20230519.dist-info/METADATA
--rw-rw-r--  2.0 unx      111 b- defN 23-May-20 04:53 tflite_runtime_nightly-2.14.0.dev20230519.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-May-20 04:53 tflite_runtime_nightly-2.14.0.dev20230519.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-May-20 04:53 tflite_runtime_nightly-2.14.0.dev20230519.dist-info/RECORD
-9 files, 6859137 bytes uncompressed, 2394751 bytes compressed:  65.1%
+Zip file size: 2396295 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       80 b- defN 23-May-21 04:51 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  6814248 b- defN 23-May-21 04:53 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-May-21 04:51 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-May-21 04:51 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-May-21 04:51 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-May-21 04:53 tflite_runtime_nightly-2.14.0.dev20230520.dist-info/METADATA
+-rw-rw-r--  2.0 unx      111 b- defN 23-May-21 04:53 tflite_runtime_nightly-2.14.0.dev20230520.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-May-21 04:53 tflite_runtime_nightly-2.14.0.dev20230520.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-May-21 04:53 tflite_runtime_nightly-2.14.0.dev20230520.dist-info/RECORD
+9 files, 6859137 bytes uncompressed, 2394749 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230519.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.14.0.dev20230520.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230519.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.14.0.dev20230520.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230519.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.14.0.dev20230520.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.14.0.dev20230519.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.14.0.dev20230520.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.14.0dev20230519'
-__git_version__ = '0.6.0-148117-ge33c39ca354'
+__version__ = '2.14.0dev20230520'
+__git_version__ = '0.6.0-148124-gf8db9933945'
```

## Comparing `tflite_runtime_nightly-2.14.0.dev20230519.dist-info/METADATA` & `tflite_runtime_nightly-2.14.0.dev20230520.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.14.0.dev20230519
+Version: 2.14.0.dev20230520
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

