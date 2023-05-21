# Comparing `tmp/ldimbenchmark-0.2.4.tar.gz` & `tmp/ldimbenchmark-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldimbenchmark-0.2.4.tar", max compression
+gzip compressed data, was "ldimbenchmark-0.2.5.tar", max compression
```

## Comparing `ldimbenchmark-0.2.4.tar` & `ldimbenchmark-0.2.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     3330 2023-05-21 16:33:16.625824 ldimbenchmark-0.2.4/README.md
--rw-r--r--   0        0        0     2359 2023-05-21 16:33:27.878261 ldimbenchmark-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      158 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/__init__.py
--rw-r--r--   0        0        0       60 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/__init__.py
--rw-r--r--   0        0        0    39257 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/benchmark.py
--rw-r--r--   0        0        0     2926 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/results.py
--rw-r--r--   0        0        0     6456 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py
--rw-r--r--   0        0        0     8649 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py
--rw-r--r--   0        0        0     3467 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py
--rw-r--r--   0        0        0     7945 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py
--rw-r--r--   0        0        0      195 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/runners/__init__.py
--rw-r--r--   0        0        0     7388 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark_complexity.py
--rw-r--r--   0        0        0     6578 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark_evaluation.py
--rw-r--r--   0        0        0    10115 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/classes.py
--rw-r--r--   0        0        0     3928 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/cli.py
--rw-r--r--   0        0        0      176 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/constants.py
--rw-r--r--   0        0        0      211 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/__init__.py
--rw-r--r--   0        0        0    10884 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/analysis.py
--rw-r--r--   0        0        0    17897 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/classes.py
--rw-r--r--   0        0        0    11765 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/derivation.py
--rw-r--r--   0        0        0     1285 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/derivation_show.py
--rw-r--r--   0        0        0     2087 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/library.py
--rw-r--r--   0        0        0        0 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/loaders/__init__.py
--rw-r--r--   0        0        0     9939 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/loaders/load_battledim.py
--rw-r--r--   0        0        0      880 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/loaders/load_dataset_base.py
--rw-r--r--   0        0        0     1288 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/evaluation_metrics/__init__.py
--rw-r--r--   0        0        0     9680 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/generator/__init__.py
--rw-r--r--   0        0        0    12993 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/generator/dataset_generator.py
--rw-r--r--   0        0        0     6332 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/generator/poulakis_network.py
--rw-r--r--   0        0        0      158 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/methods/__init__.py
--rw-r--r--   0        0        0    13338 2023-05-21 16:33:16.645825 ldimbenchmark-0.2.4/src/ldimbenchmark/methods/dualmethod.py
--rw-r--r--   0        0        0    19401 2023-05-21 16:33:16.649825 ldimbenchmark-0.2.4/src/ldimbenchmark/methods/lila.py
--rw-r--r--   0        0        0    10445 2023-05-21 16:33:16.649825 ldimbenchmark-0.2.4/src/ldimbenchmark/methods/mnf.py
--rw-r--r--   0        0        0     1171 2023-05-21 16:33:16.649825 ldimbenchmark-0.2.4/src/ldimbenchmark/methods/null.py
--rw-r--r--   0        0        0     2033 2023-05-21 16:33:16.649825 ldimbenchmark-0.2.4/src/ldimbenchmark/methods/random.py
--rw-r--r--   0        0        0        0 2023-05-21 16:33:16.649825 ldimbenchmark-0.2.4/src/ldimbenchmark/methods/utils/__init__.py
--rw-r--r--   0        0        0     5309 2023-05-21 16:33:16.649825 ldimbenchmark-0.2.4/src/ldimbenchmark/methods/utils/cusum.py
--rw-r--r--   0        0        0     8349 2023-05-21 16:33:16.649825 ldimbenchmark-0.2.4/src/ldimbenchmark/utilities.py
--rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.4/setup.py
--rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     3330 2023-05-21 19:36:52.079241 ldimbenchmark-0.2.5/README.md
+-rw-r--r--   0        0        0     2359 2023-05-21 19:37:03.783347 ldimbenchmark-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-05-21 19:36:52.099241 ldimbenchmark-0.2.5/src/ldimbenchmark/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-21 19:36:52.099241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/__init__.py
+-rw-r--r--   0        0        0    39257 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/benchmark.py
+-rw-r--r--   0        0        0     2926 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/results.py
+-rw-r--r--   0        0        0     6456 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py
+-rw-r--r--   0        0        0     8649 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py
+-rw-r--r--   0        0        0     3467 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py
+-rw-r--r--   0        0        0     7945 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py
+-rw-r--r--   0        0        0      195 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/__init__.py
+-rw-r--r--   0        0        0     8177 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark_complexity.py
+-rw-r--r--   0        0        0     6578 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark_evaluation.py
+-rw-r--r--   0        0        0    10115 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/classes.py
+-rw-r--r--   0        0        0     3928 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/cli.py
+-rw-r--r--   0        0        0      176 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/constants.py
+-rw-r--r--   0        0        0      211 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/__init__.py
+-rw-r--r--   0        0        0    10884 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/analysis.py
+-rw-r--r--   0        0        0    17897 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/classes.py
+-rw-r--r--   0        0        0    11765 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/derivation.py
+-rw-r--r--   0        0        0     1285 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/derivation_show.py
+-rw-r--r--   0        0        0     2087 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/library.py
+-rw-r--r--   0        0        0        0 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/loaders/__init__.py
+-rw-r--r--   0        0        0     9939 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/loaders/load_battledim.py
+-rw-r--r--   0        0        0      880 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/loaders/load_dataset_base.py
+-rw-r--r--   0        0        0     1288 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/evaluation_metrics/__init__.py
+-rw-r--r--   0        0        0     9680 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/generator/__init__.py
+-rw-r--r--   0        0        0    12993 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/generator/dataset_generator.py
+-rw-r--r--   0        0        0     6332 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/generator/poulakis_network.py
+-rw-r--r--   0        0        0      158 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/__init__.py
+-rw-r--r--   0        0        0    13338 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/dualmethod.py
+-rw-r--r--   0        0        0    19401 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/lila.py
+-rw-r--r--   0        0        0    10445 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/mnf.py
+-rw-r--r--   0        0        0     1171 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/null.py
+-rw-r--r--   0        0        0     2033 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/random.py
+-rw-r--r--   0        0        0        0 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/utils/__init__.py
+-rw-r--r--   0        0        0     5309 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/utils/cusum.py
+-rw-r--r--   0        0        0     8349 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/utilities.py
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.5/setup.py
+-rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.5/PKG-INFO
```

### Comparing `ldimbenchmark-0.2.4/README.md` & `ldimbenchmark-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/pyproject.toml` & `ldimbenchmark-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ldimbenchmark"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["DanielHabenicht <daniel-habenicht@outlook.de>"]
 readme = "README.md"
 exclude = [
     "tests",
     "experiments"
 ]
```

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/benchmark.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/results.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/results.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark_complexity.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark_complexity.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         total=len(methods), desc="Running Analysis", unit="methods"
     )
     logging.info(" > Starting Complexity analysis")
     for method in methods:
         method_name = get_method_name_from_docker_image(method)
         logging.info(f" - {method_name}")
         complexity_benchmark_result_folder = os.path.join(
-            out_folder, "runs", method_name, "1"
+            out_folder, "runs", method_name
         )
         client = docker.from_env()
 
         try:
             image = client.images.get(method)
         except docker.errors.ImageNotFound:
             logging.info("Image does not exist. Pulling it...")
@@ -116,57 +116,71 @@
         min_n = 4
         max_n = len(dataset_dirs)
         n_measures = 10
         n_repeats = 3
         n_samples = np.linspace(min_n, max_n, n_measures).astype("int64")
 
         for i, n in enumerate(n_samples):
+            summed_results = {"time": [], "ram": []}
             for r in range(n_repeats):
                 complexity_benchmark_result_folder_run = os.path.join(
                     complexity_benchmark_result_folder, str(r)
                 )
-            runner = DockerMethodRunner(
-                method,
-                datasets[n],
-                "evaluation",
-                hyperparameters[method_name],
-                resultsFolder=complexity_benchmark_result_folder,
-                debug=additionalOutput,
-            )
-            runner.run()
-
-        bar_running_analysis.close()
-        manager.stop()
-
-        parallel = True
-        result_folders = glob(os.path.join(complexity_benchmark_result_folder, "*"))
-        run_results = []
-        if parallel == True:
-            with ProcessPoolExecutor() as executor:
-                # submit all tasks and get future objects
-                futures = [
-                    executor.submit(load_result, folder, try_load_docker_stats=True)
-                    for folder in result_folders
-                ]
-                # process results from tasks in order of task completion
-                for future in as_completed(futures):
-                    result = future.result()
-                    run_results.append(result)
-        else:
-            for experiment_result in result_folders:
-                run_results.append(load_result(experiment_result, True))
-
-        run_results = pd.DataFrame(run_results)
-        run_results["number"] = run_results["dataset"].str.split("-").str[2].astype(int)
-        sorted_results = run_results.sort_values(by=["number"])
+                runner = DockerMethodRunner(
+                    method,
+                    datasets[n],
+                    "evaluation",
+                    hyperparameters[method_name],
+                    resultsFolder=complexity_benchmark_result_folder_run,
+                    debug=additionalOutput,
+                )
+                runner.run()
+
+                parallel = True
+                result_folders = glob(
+                    os.path.join(complexity_benchmark_result_folder_run, "*")
+                )
+                run_results = []
+                if parallel == True:
+                    with ProcessPoolExecutor() as executor:
+                        # submit all tasks and get future objects
+                        futures = [
+                            executor.submit(
+                                load_result, folder, try_load_docker_stats=True
+                            )
+                            for folder in result_folders
+                        ]
+                        # process results from tasks in order of task completion
+                        for future in as_completed(futures):
+                            result = future.result()
+                            run_results.append(result)
+                else:
+                    for experiment_result in result_folders:
+                        run_results.append(load_result(experiment_result, True))
+
+                run_results = pd.DataFrame(run_results)
+                run_results["number"] = (
+                    run_results["dataset"].str.split("-").str[2].astype(int)
+                )
+                sorted_results = run_results.sort_values(by=["number"])
+
+                summed_results["time"] = np.append(
+                    summed_results["time"], sorted_results["method_time"]
+                )
+                summed_results["ram"] = np.append(
+                    summed_results["ram"], sorted_results["memory_max"]
+                )
+
         best_cpu, rest = big_o.infer_big_o_class(
-            sorted_results["number"], sorted_results["method_time"]
+            sorted_results["number"],
+            np.sum(summed_results["time"].reshape((len(n_samples), n_repeats)), axis=1),
         )
         best_ram, rest = big_o.infer_big_o_class(
-            sorted_results["number"], sorted_results["memory_avg"]
+            sorted_results["number"],
+            np.sum(summed_results["ram"].reshape((len(n_samples), n_repeats)), axis=1),
         )
 
         results["time"][method] = best_cpu
         results["ram"][method] = best_ram
 
         measures = pd.DataFrame(
             {
@@ -177,17 +191,20 @@
         )
         result_measures.append(measures)
         # measures.to_csv(os.path.join(out_folder, "measures_raw.csv"))
         # pd.DataFrame(list(others.items())[1:8]).to_csv(
         #     os.path.join(out_folder, "big_o.csv"), header=False, index=False
         # )
         bar_running_analysis.update()
+
         # Cooldown for 10 seconds
         time.sleep(10)
 
+    bar_running_analysis.close()
+    manager.stop()
     logging.info(f"Exporting results to {out_folder}")
     results = pd.DataFrame(
         {
             "Leakage Detection Method": results["time"].keys(),
             "Time Complexity": results["time"].values(),
             "RAM Complexity": results["ram"].values(),
         }
```

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/benchmark_evaluation.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark_evaluation.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/classes.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/classes.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/cli.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/cli.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/analysis.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/analysis.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/classes.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/derivation.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/derivation.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/derivation_show.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/derivation_show.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/library.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/library.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/loaders/load_battledim.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/loaders/load_battledim.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/datasets/loaders/load_dataset_base.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/loaders/load_dataset_base.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/evaluation_metrics/__init__.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/evaluation_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/generator/__init__.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/generator/dataset_generator.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/generator/dataset_generator.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/generator/poulakis_network.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/generator/poulakis_network.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/methods/dualmethod.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/methods/dualmethod.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/methods/lila.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/methods/lila.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/methods/mnf.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/methods/mnf.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/methods/null.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/methods/null.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/methods/random.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/methods/random.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/methods/utils/cusum.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/methods/utils/cusum.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/src/ldimbenchmark/utilities.py` & `ldimbenchmark-0.2.5/src/ldimbenchmark/utilities.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.4/setup.py` & `ldimbenchmark-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
  'wntr>=0.5.0,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['ldimbenchmark = ldimbenchmark.cli:cli']}
 
 setup_kwargs = {
     'name': 'ldimbenchmark',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': '',
     'long_description': '[![ldimbenchmark version](https://badgen.net/pypi/v/ldimbenchmark/)](https://pypi.org/project/ldimbenchmark)\n[![Documentation badge](https://img.shields.io/badge/Documentation-here!-GREEN.svg)](https://tumt2022.github.io/LDIMBench/)\n\n# LDIMBenchmark\n\nLeakage Detection and Isolation Methods Benchmark\n\n> Instead of collecting all the different dataset to benchmark different methods on. We wanted to create a Benchmarking Tool which makes it easy to reproduce the results of the different methods locally on your own dataset.\n\nIt provides a close to real-world conditions environment and forces researchers to provide a reproducible method implementation, which is supposed to run automated on any input dataset, thus hindering custom solutions which work well in one specific case.\n\n## Usage\n\n### Installation\n\n```bash\npip install ldimbenchmark\n```\n\n### Python\n\n```python\nfrom ldimbenchmark.datasets import DatasetLibrary, DATASETS\nfrom ldimbenchmark import (\n    LDIMBenchmark,\n    BenchmarkData,\n    BenchmarkLeakageResult,\n)\nfrom ldimbenchmark.classes import LDIMMethodBase\nfrom typing import List\n\nclass YourCustomLDIMMethod(LDIMMethodBase):\n    def __init__(self):\n        super().__init__(\n            name="YourCustomLDIMMethod",\n            version="0.1.0"\n        )\n\n    def train(self, data: BenchmarkData):\n        pass\n\n    def detect(self, data: BenchmarkData) -> List[BenchmarkLeakageResult]:\n        return [\n            {\n                "leak_start": "2020-01-01",\n                "leak_end": "2020-01-02",\n                "leak_area": 0.2,\n                "pipe_id": "test",\n            }\n        ]\n\n    def detect_datapoint(self, evaluation_data) -> BenchmarkLeakageResult:\n        return {}\n\n\ndatasets = DatasetLibrary("datasets").download(DATASETS.BATTLEDIM)\n\nlocal_methods = [YourCustomLDIMMethod()]\n\nhyperparameters = {}\n\nbenchmark = LDIMBenchmark(\n    hyperparameters, datasets, results_dir="./benchmark-results"\n)\nbenchmark.add_local_methods(local_methods)\n\nbenchmark.run_benchmark()\n\nbenchmark.evaluate()\n```\n\n### CLI\n\n```bash\nldimbenchmark --help\n```\n\n## Roadmap\n\n- v1: Just Leakage Detection\n- v2: Provides Benchmark of Isolation Methods\n\nhttps://mathspp.com/blog/how-to-create-a-python-package-in-2022\n\n## Development\n\nhttps://python-poetry.org/docs/basic-usage/\n\n```bash\n# python 3.10\n# Use Environment\npoetry config virtualenvs.in-project true\npoetry shell\npoetry install --without ci # --with ci\n\n\n# Test\npoetry build\ncp -r dist tests/dist\ncd tests\ndocker build . -t testmethod\npytest -s -o log_cli=true\npytest tests/test_derivation.py -k \'test_mything\'\npytest --testmon\npytest --snapshot-update\n\n# Pytest watch\nptw\nptw -- --testmon\n\n# Watch a file during development\nnpm install -g nodemon\nnodemon -L experiments/auto_hyperparameter.py\n\n# Test-Publish\npoetry config repositories.testpypi https://test.pypi.org/legacy/\npoetry config http-basic.testpypi __token__ pypi-your-api-token-here\npoetry build\npoetry publish -r testpypi\n\n# Real Publish\npoetry config pypi-token.pypi pypi-your-token-here\n```\n\n### Documentation\n\nhttps://squidfunk.github.io/mkdocs-material/\nhttps://click.palletsprojects.com/en/8.1.x/\n\n```\nmkdocs serve\n```\n\n# TODO\n\nLDIMBenchmark:\nData Cleansing before working with them\n\n- per sensor type, e.g. waterflow (cut of at 0)\n- removing datapoints which are clearly a malfunction\n',
     'author': 'DanielHabenicht',
     'author_email': 'daniel-habenicht@outlook.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ldimbenchmark-0.2.4/PKG-INFO` & `ldimbenchmark-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldimbenchmark
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: DanielHabenicht
 Author-email: daniel-habenicht@outlook.de
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

