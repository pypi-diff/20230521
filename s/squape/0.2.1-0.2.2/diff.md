# Comparing `tmp/squape-0.2.1.tar.gz` & `tmp/squape-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squape-0.2.1.tar", last modified: Wed May 17 20:10:44 2023, max compression
+gzip compressed data, was "squape-0.2.2.tar", last modified: Sun May 21 20:22:10 2023, max compression
```

## Comparing `squape-0.2.1.tar` & `squape-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 20:10:44.171819 squape-0.2.1/
--rw-rw-rw-   0        0        0      183 2023-03-26 19:20:26.000000 squape-0.2.1/.flake8
--rw-rw-rw-   0        0        0      227 2023-03-26 19:19:42.000000 squape-0.2.1/.gitignore
--rw-rw-rw-   0        0        0     1214 2023-05-02 09:48:54.000000 squape-0.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      974 2023-05-17 18:52:47.000000 squape-0.2.1/HISTORY.md
--rw-rw-rw-   0        0        0     1541 2023-03-26 19:19:01.000000 squape-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2185 2023-05-17 20:10:44.170287 squape-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1548 2023-05-03 08:14:02.000000 squape-0.2.1/README.md
--rw-rw-rw-   0        0        0      847 2023-05-17 18:53:20.000000 squape-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       10 2023-03-26 19:20:26.000000 squape-0.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 20:10:44.172145 squape-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-17 20:10:44.154720 squape-0.2.1/squape/
--rw-rw-rw-   0        0        0      220 2023-04-17 17:33:50.000000 squape-0.2.1/squape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 20:10:44.167276 squape-0.2.1/squape/internal/
--rw-rw-rw-   0        0        0      220 2023-05-02 09:42:03.000000 squape-0.2.1/squape/internal/__init__.py
--rw-rw-rw-   0        0        0      468 2023-05-02 09:42:03.000000 squape-0.2.1/squape/internal/exceptions.py
--rw-rw-rw-   0        0        0     8426 2023-05-17 18:49:29.000000 squape-0.2.1/squape/report.py
-drwxrwxrwx   0        0        0        0 2023-05-17 20:10:44.169287 squape-0.2.1/squape/resources/
--rw-rw-rw-   0        0        0    10904 2023-05-02 09:48:54.000000 squape-0.2.1/squape/resources/empty_video_with_message.mp4
--rw-rw-rw-   0        0        0    10797 2023-05-02 09:48:54.000000 squape-0.2.1/squape/settings.py
--rw-rw-rw-   0        0        0     3882 2023-05-02 09:48:54.000000 squape-0.2.1/squape/video.py
--rw-rw-rw-   0        0        0     1179 2023-05-02 09:48:54.000000 squape-0.2.1/squape/vps.py
-drwxrwxrwx   0        0        0        0 2023-05-17 20:10:44.161454 squape-0.2.1/squape.egg-info/
--rw-rw-rw-   0        0        0     2185 2023-05-17 20:10:43.000000 squape-0.2.1/squape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-05-17 20:10:44.000000 squape-0.2.1/squape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 20:10:43.000000 squape-0.2.1/squape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-17 20:10:43.000000 squape-0.2.1/squape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 20:22:10.634861 squape-0.2.2/
+-rw-rw-rw-   0        0        0      183 2023-03-26 19:20:26.000000 squape-0.2.2/.flake8
+-rw-rw-rw-   0        0        0      227 2023-03-26 19:19:42.000000 squape-0.2.2/.gitignore
+-rw-rw-rw-   0        0        0     1214 2023-05-02 09:48:54.000000 squape-0.2.2/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1138 2023-05-21 20:19:23.000000 squape-0.2.2/HISTORY.md
+-rw-rw-rw-   0        0        0     1541 2023-03-26 19:19:01.000000 squape-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2185 2023-05-21 20:22:10.634861 squape-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1548 2023-05-03 08:14:02.000000 squape-0.2.2/README.md
+-rw-rw-rw-   0        0        0      847 2023-05-21 20:19:23.000000 squape-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       10 2023-03-26 19:20:26.000000 squape-0.2.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 20:22:10.635852 squape-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 20:22:10.617385 squape-0.2.2/squape/
+-rw-rw-rw-   0        0        0      220 2023-04-17 17:33:50.000000 squape-0.2.2/squape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:22:10.630361 squape-0.2.2/squape/internal/
+-rw-rw-rw-   0        0        0      220 2023-05-02 09:42:03.000000 squape-0.2.2/squape/internal/__init__.py
+-rw-rw-rw-   0        0        0      468 2023-05-02 09:42:03.000000 squape-0.2.2/squape/internal/exceptions.py
+-rw-rw-rw-   0        0        0     8524 2023-05-21 20:19:23.000000 squape-0.2.2/squape/report.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:22:10.632542 squape-0.2.2/squape/resources/
+-rw-rw-rw-   0        0        0    10904 2023-05-02 09:48:54.000000 squape-0.2.2/squape/resources/empty_video_with_message.mp4
+-rw-rw-rw-   0        0        0    10797 2023-05-02 09:48:54.000000 squape-0.2.2/squape/settings.py
+-rw-rw-rw-   0        0        0     3882 2023-05-02 09:48:54.000000 squape-0.2.2/squape/video.py
+-rw-rw-rw-   0        0        0     1179 2023-05-02 09:48:54.000000 squape-0.2.2/squape/vps.py
+drwxrwxrwx   0        0        0        0 2023-05-21 20:22:10.622919 squape-0.2.2/squape.egg-info/
+-rw-rw-rw-   0        0        0     2185 2023-05-21 20:22:10.000000 squape-0.2.2/squape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-05-21 20:22:10.000000 squape-0.2.2/squape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 20:22:10.000000 squape-0.2.2/squape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-21 20:22:10.000000 squape-0.2.2/squape.egg-info/top_level.txt
```

### Comparing `squape-0.2.1/.pre-commit-config.yaml` & `squape-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `squape-0.2.1/LICENSE` & `squape-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `squape-0.2.1/PKG-INFO` & `squape-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squape
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python utilities for the Squish GUI Tester
 Author-email: Cyber Alpaca <contact@cyberalpaca.com>
 Project-URL: Homepage, https://github.com/CyberAlpaca/squish-api-python-extension
 Project-URL: Cyber Alpaca, https://cyberalpaca.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `squape-0.2.1/README.md` & `squape-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `squape-0.2.1/pyproject.toml` & `squape-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["squape"]
 namespaces = false
 
 [project]
 name = "squape"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     { name="Cyber Alpaca", email="contact@cyberalpaca.com" },
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 description = "Python utilities for the Squish GUI Tester"
 classifiers = [
```

### Comparing `squape-0.2.1/squape/report.py` & `squape-0.2.2/squape/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,20 @@
        set_level(report.LogLevel.WARNING)
        set_level("FAIL")
     """
     global LOGLEVEL
     LOGLEVEL = __translate_Level(level)
 
 
-LOGLEVEL = set_level(LogLevel.LOG)
+set_level(LogLevel.LOG)
+
+_test_log = test.log
+_test_warning = test.warning
+_test_fail = test.fail
+_test_fatal = test.fatal
 
 
 def __is_level_enabled(level: LogLevel) -> bool:
     """Checks the given log level against the currently set LOGLEVEL
 
     Args:
         level (LogLevel): log level to check
@@ -90,15 +95,15 @@
 
     Returns:
         None
     """
     if __is_level_enabled(LogLevel.DEBUG):
         test.fixateResultContext(1)
         try:
-            test.log(f"[DEBUG] {msg}", details)
+            _test_log(f"[DEBUG] {msg}", details)
         finally:
             test.restoreResultContext()
 
 
 def log(msg: str, details: str = "") -> None:
     """Adds a log entry with the given message and details to a test report.
 
@@ -115,15 +120,15 @@
 
     Returns:
         None
     """
     if __is_level_enabled(LogLevel.LOG):
         test.fixateResultContext(1)
         try:
-            test.log(msg, details)
+            _test_log(msg, details)
         finally:
             test.restoreResultContext()
 
 
 def warning(msg: str, details: str = "") -> None:
     """Adds a warning entry with the given message and details to a test report.
 
@@ -141,15 +146,15 @@
 
     Returns:
         None
     """
     if __is_level_enabled(LogLevel.WARNING):
         test.fixateResultContext(1)
         try:
-            test.warning(msg, details)
+            _test_warning(msg, details)
         finally:
             test.restoreResultContext()
 
 
 def fail(msg: str, details: str = "") -> None:
     """Adds a fail entry with the given message and details to a test report.
 
@@ -166,15 +171,15 @@
 
     Returns:
         None
     """
     if __is_level_enabled(LogLevel.FAIL):
         test.fixateResultContext(1)
         try:
-            test.fail(msg, details)
+            _test_fail(msg, details)
         finally:
             test.restoreResultContext()
 
 
 def fatal(msg: str, details: str = "") -> None:
     """Adds a fatal entry with the given message and details to a test report,
     then aborts the test case execution.
@@ -195,15 +200,15 @@
     Returns:
         None
     """
     if __is_level_enabled(LogLevel.FATAL):
         test.fixateResultContext(1)
         try:
             squish.testSettings.throwOnFailure = True
-            test.fatal(msg, details)
+            _test_fatal(msg, details)
         finally:
             test.restoreResultContext()
 
 
 def enable_loglevel_in_test_module():
     """Adds support for log levels to the Squish 'test' module.
```

### Comparing `squape-0.2.1/squape/resources/empty_video_with_message.mp4` & `squape-0.2.2/squape/resources/empty_video_with_message.mp4`

 * *Files identical despite different names*

### Comparing `squape-0.2.1/squape/settings.py` & `squape-0.2.2/squape/settings.py`

 * *Files identical despite different names*

### Comparing `squape-0.2.1/squape/video.py` & `squape-0.2.2/squape/video.py`

 * *Files identical despite different names*

### Comparing `squape-0.2.1/squape/vps.py` & `squape-0.2.2/squape/vps.py`

 * *Files identical despite different names*

### Comparing `squape-0.2.1/squape.egg-info/PKG-INFO` & `squape-0.2.2/squape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squape
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python utilities for the Squish GUI Tester
 Author-email: Cyber Alpaca <contact@cyberalpaca.com>
 Project-URL: Homepage, https://github.com/CyberAlpaca/squish-api-python-extension
 Project-URL: Cyber Alpaca, https://cyberalpaca.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
```

