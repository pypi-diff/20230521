# Comparing `tmp/tuneflow-devkit-py-0.8.3.tar.gz` & `tmp/tuneflow-devkit-py-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-devkit-py-0.8.3.tar", last modified: Fri May 19 15:34:58 2023, max compression
+gzip compressed data, was "tuneflow-devkit-py-0.8.4.tar", last modified: Sun May 21 00:58:35 2023, max compression
```

## Comparing `tuneflow-devkit-py-0.8.3.tar` & `tuneflow-devkit-py-0.8.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-19 15:34:58.735057 tuneflow-devkit-py-0.8.3/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.8.3/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-19 15:34:58.735057 tuneflow-devkit-py-0.8.3/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.8.3/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-05-19 15:34:32.000000 tuneflow-devkit-py-0.8.3/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-05-19 15:34:58.735057 tuneflow-devkit-py-0.8.3/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-19 15:34:58.735057 tuneflow-devkit-py-0.8.3/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-19 15:34:58.735057 tuneflow-devkit-py-0.8.3/src/tuneflow_devkit/
--rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.8.3/src/tuneflow_devkit/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     7078 2023-05-10 04:50:11.000000 tuneflow-devkit-py-0.8.3/src/tuneflow_devkit/debugger.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     8753 2023-05-19 15:24:13.000000 tuneflow-devkit-py-0.8.3/src/tuneflow_devkit/runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.8.3/src/tuneflow_devkit/translate_utils.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.8.3/src/tuneflow_devkit/validation_utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-19 15:34:58.735057 tuneflow-devkit-py-0.8.3/src/tuneflow_devkit_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-19 15:34:58.000000 tuneflow-devkit-py-0.8.3/src/tuneflow_devkit_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-05-19 15:34:58.000000 tuneflow-devkit-py-0.8.3/src/tuneflow_devkit_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-05-19 15:34:58.000000 tuneflow-devkit-py-0.8.3/src/tuneflow_devkit_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-05-19 15:34:58.000000 tuneflow-devkit-py-0.8.3/src/tuneflow_devkit_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-05-19 15:34:58.000000 tuneflow-devkit-py-0.8.3/src/tuneflow_devkit_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-19 15:34:58.735057 tuneflow-devkit-py-0.8.3/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4192 2023-03-30 01:44:09.000000 tuneflow-devkit-py-0.8.3/test/test_runner.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.8.3/test/test_validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-21 00:58:35.837463 tuneflow-devkit-py-0.8.4/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-01-11 08:37:26.000000 tuneflow-devkit-py-0.8.4/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-21 00:58:35.837463 tuneflow-devkit-py-0.8.4/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-03-29 06:56:17.000000 tuneflow-devkit-py-0.8.4/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1376 2023-05-21 00:53:55.000000 tuneflow-devkit-py-0.8.4/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-05-21 00:58:35.837463 tuneflow-devkit-py-0.8.4/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-21 00:58:35.827463 tuneflow-devkit-py-0.8.4/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-21 00:58:35.837463 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       88 2023-03-05 07:33:21.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     7078 2023-05-10 04:50:11.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/debugger.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     8679 2023-05-20 23:50:54.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      921 2023-02-28 00:11:56.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/translate_utils.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1280 2023-03-05 07:33:30.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/validation_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-21 00:58:35.837463 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2620 2023-05-21 00:58:35.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      484 2023-05-21 00:58:35.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-05-21 00:58:35.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      119 2023-05-21 00:58:35.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       16 2023-05-21 00:58:35.000000 tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-21 00:58:35.837463 tuneflow-devkit-py-0.8.4/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4192 2023-03-30 01:44:09.000000 tuneflow-devkit-py-0.8.4/test/test_runner.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2686 2023-03-05 07:52:40.000000 tuneflow-devkit-py-0.8.4/test/test_validation_utils.py
```

### Comparing `tuneflow-devkit-py-0.8.3/LICENSE` & `tuneflow-devkit-py-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.3/PKG-INFO` & `tuneflow-devkit-py-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.8.3
+Version: 0.8.4
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.8.3/README.md` & `tuneflow-devkit-py-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.3/pyproject.toml` & `tuneflow-devkit-py-0.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-devkit-py"
-version = "0.8.3"
+version = "0.8.4"
 authors = [{ name = "Andantei", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
     "AI",
     "music",
```

### Comparing `tuneflow-devkit-py-0.8.3/src/tuneflow_devkit/debugger.py` & `tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/debugger.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.3/src/tuneflow_devkit/runner.py` & `tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             return {
                 "status": "OK",
                 "song": song.serialize_to_bytestring()
             }
 
         async def run_plugin_async_task(plugin_class: Type[TuneflowPlugin], song, params, job_id: str, store_uploader):
             # TODO: Revisit to see if we can call run_plugin_task directly.
-            response = await asyncio.get_event_loop().run_in_executor(None,  functools.partial(run_plugin_task, plugin_class=plugin_class, song=song, params=params))
+            response = run_plugin_task(plugin_class=plugin_class, song=song, params=params)
             error = response["error"] if "error" in response else None
             if "error" in response:
                 del response["error"]
             response["jobId"] = job_id
             store_uploader(job_id, packb(response))
             if response["status"] == "ERROR" and error is not None and exception_handler is not None:
                 exception_handler(error)
```

### Comparing `tuneflow-devkit-py-0.8.3/src/tuneflow_devkit/translate_utils.py` & `tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/translate_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.3/src/tuneflow_devkit/validation_utils.py` & `tuneflow-devkit-py-0.8.4/src/tuneflow_devkit/validation_utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.3/src/tuneflow_devkit_py.egg-info/PKG-INFO` & `tuneflow-devkit-py-0.8.4/src/tuneflow_devkit_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-devkit-py
-Version: 0.8.3
+Version: 0.8.4
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: Andantei <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-devkit-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-devkit-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis,SDK,devkit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-devkit-py-0.8.3/test/test_runner.py` & `tuneflow-devkit-py-0.8.4/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `tuneflow-devkit-py-0.8.3/test/test_validation_utils.py` & `tuneflow-devkit-py-0.8.4/test/test_validation_utils.py`

 * *Files identical despite different names*

