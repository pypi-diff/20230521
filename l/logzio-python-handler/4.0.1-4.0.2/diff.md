# Comparing `tmp/logzio-python-handler-4.0.1.tar.gz` & `tmp/logzio-python-handler-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logzio-python-handler-4.0.1.tar", last modified: Thu Feb 16 09:25:17 2023, max compression
+gzip compressed data, was "logzio-python-handler-4.0.2.tar", last modified: Sun May 21 07:20:29 2023, max compression
```

## Comparing `logzio-python-handler-4.0.1.tar` & `logzio-python-handler-4.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:25:17.175371 logzio-python-handler-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-16 09:25:17.175371 logzio-python-handler-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:25:17.175371 logzio-python-handler-4.0.1/logzio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/logzio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/logzio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/logzio/flusher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/logzio/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/logzio/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/logzio/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:25:17.175371 logzio-python-handler-4.0.1/logzio_python_handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-16 09:25:17.000000 logzio-python-handler-4.0.1/logzio_python_handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-16 09:25:17.000000 logzio-python-handler-4.0.1/logzio_python_handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 09:25:17.000000 logzio-python-handler-4.0.1/logzio_python_handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-16 09:25:17.000000 logzio-python-handler-4.0.1/logzio_python_handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-16 09:25:17.000000 logzio-python-handler-4.0.1/logzio_python_handler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-16 09:25:17.175371 logzio-python-handler-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:25:17.175371 logzio-python-handler-4.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 09:25:17.175371 logzio-python-handler-4.0.1/tests/mockLogzioListener/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/tests/mockLogzioListener/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/tests/mockLogzioListener/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/tests/mockLogzioListener/logsList.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/tests/mockLogzioListener/persistentFlags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/tests/test_add_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/tests/test_logzioHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-02-16 09:25:03.000000 logzio-python-handler-4.0.1/tests/test_logzioSender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/logzio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/logzio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/logzio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/logzio/flusher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/logzio/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/logzio/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/logzio/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/logzio_python_handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-21 07:20:29.000000 logzio-python-handler-4.0.2/logzio_python_handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-21 07:20:29.000000 logzio-python-handler-4.0.2/logzio_python_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 07:20:29.000000 logzio-python-handler-4.0.2/logzio_python_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-21 07:20:29.000000 logzio-python-handler-4.0.2/logzio_python_handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-21 07:20:29.000000 logzio-python-handler-4.0.2/logzio_python_handler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:29.070340 logzio-python-handler-4.0.2/tests/mockLogzioListener/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/mockLogzioListener/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/mockLogzioListener/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/mockLogzioListener/logsList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/mockLogzioListener/persistentFlags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/test_add_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/test_logzioHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-21 07:20:22.000000 logzio-python-handler-4.0.2/tests/test_logzioSender.py
```

### Comparing `logzio-python-handler-4.0.1/LICENSE` & `logzio-python-handler-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.0.1/README.md` & `logzio-python-handler-4.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -251,28 +251,33 @@
     }
 }
 ```
 
 Please note that if you are using `python 3.8`, it is preferred to use the `logging.config.dictConfig` method, as mentioned in [python's documentation](https://docs.python.org/3/library/logging.config.html#configuration-file-format).
 
 ## Release Notes
+
+- 4.0.2
+  - Fix bug for logging exceptions ([#76](https://github.com/logzio/logzio-python-handler/pull/76))
 - 4.0.1
   - Updated `protobuf>=3.20.2`.
   - Added dependency `setuptools>=65.5.1`
   
 - 4.0.0
   - Add ability to automatically attach trace context to the logs.
 
-- 3.1.1
-  - Bug fixes (issue #68, exception message formatting)
-  - Added CI: Tests and Auto release 
 
 <details>
   <summary markdown="span"> Expand to check old versions </summary>
 
+
+- 3.1.1
+  - Bug fixes (issue #68, exception message formatting)
+  - Added CI: Tests and Auto release
+  
 - 3.1.0
     - Bug fixes
     - Retry number and timeout is now configurable
     
 - 3.0.0
     - Deprecated `python2.7` & `python3.4`
     - Changed log levels on `_flush_queue()` method (@hilsenrat)
```

### Comparing `logzio-python-handler-4.0.1/logzio/flusher.py` & `logzio-python-handler-4.0.2/logzio/flusher.py`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.0.1/logzio/handler.py` & `logzio-python-handler-4.0.2/logzio/handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,14 +75,16 @@
 
     def flush(self):
         self.logzio_sender.flush()
 
     def format(self, record):
         message = super(LogzioHandler, self).format(record)
         try:
+            if record.exc_info:
+                message = message.split("\n")[0]  # only keep the original formatted message part
             return json.loads(message)
         except (TypeError, ValueError):
             return message
 
     def format_exception(self, exc_info):
         return '\n'.join(traceback.format_exception(*exc_info))
```

### Comparing `logzio-python-handler-4.0.1/logzio/sender.py` & `logzio-python-handler-4.0.2/logzio/sender.py`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.0.1/logzio_python_handler.egg-info/SOURCES.txt` & `logzio-python-handler-4.0.2/logzio_python_handler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.0.1/setup.py` & `logzio-python-handler-4.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 setup(
     name="logzio-python-handler",
-    version='4.0.1',
+    version='4.0.2',
     description="Logging handler to send logs to your Logz.io account with bulk SSL",
     keywords="logging handler logz.io bulk https",
     author="roiravhon",
     maintainer="tamir-michaeli",
     mail="tamir.michaeli@logz.io",
     url="https://github.com/logzio/logzio-python-handler/",
     license="Apache License 2",
```

### Comparing `logzio-python-handler-4.0.1/tests/mockLogzioListener/listener.py` & `logzio-python-handler-4.0.2/tests/mockLogzioListener/listener.py`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.0.1/tests/test_add_context.py` & `logzio-python-handler-4.0.2/tests/test_add_context.py`

 * *Files identical despite different names*

### Comparing `logzio-python-handler-4.0.1/tests/test_logzioHandler.py` & `logzio-python-handler-4.0.2/tests/test_logzioHandler.py`

 * *Files 7% similar despite different names*

```diff
@@ -133,15 +133,18 @@
                 'logger': 'my-logger',
                 'message': 'this is a test: moo.',
                 'path_name': 'handler_test.py',
                 'type': 'python'
             }
         )
 
-    def test_exc(self):
+    def test_exception(self):
+        formatter = logging.Formatter('{"tags": ["staging", "experimental"], "appname": "my-service"}', validate=False)
+        self.handler.setFormatter(formatter)
+        
         try:
             raise ValueError("oops.")
         except:
             exc_info = sys.exc_info()
 
         record = logging.LogRecord(
             name='my-logger',
@@ -159,17 +162,19 @@
 
         formatted_message["exception"] = formatted_message["exception"].replace(os.path.abspath(__file__), "")
         formatted_message["exception"] = re.sub(r", line \d+", "", formatted_message["exception"])
 
         self.assertDictEqual(
             {
                 '@timestamp': None,
+                'appname': 'my-service',
                 'line_number': 10,
                 'log_level': 'NOTSET',
                 'logger': 'my-logger',
                 'message': 'exception test:',
-                'exception': 'Traceback (most recent call last):\n\n  File "", in test_exc\n    raise ValueError("oops.")\n\nValueError: oops.\n',
+                'exception': 'Traceback (most recent call last):\n\n  File "", in test_exception\n    raise ValueError("oops.")\n\nValueError: oops.\n',
                 'path_name': 'handler_test.py',
-                'type': 'python'
+                'type': 'python',
+                'tags': ['staging', 'experimental']
             },
             formatted_message
         )
```

### Comparing `logzio-python-handler-4.0.1/tests/test_logzioSender.py` & `logzio-python-handler-4.0.2/tests/test_logzioSender.py`

 * *Files identical despite different names*

