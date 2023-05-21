# Comparing `tmp/ldimbenchmark-0.2.5.tar.gz` & `tmp/ldimbenchmark-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldimbenchmark-0.2.5.tar", max compression
+gzip compressed data, was "ldimbenchmark-0.2.6.tar", max compression
```

## Comparing `ldimbenchmark-0.2.5.tar` & `ldimbenchmark-0.2.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     3330 2023-05-21 19:36:52.079241 ldimbenchmark-0.2.5/README.md
--rw-r--r--   0        0        0     2359 2023-05-21 19:37:03.783347 ldimbenchmark-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      158 2023-05-21 19:36:52.099241 ldimbenchmark-0.2.5/src/ldimbenchmark/__init__.py
--rw-r--r--   0        0        0       60 2023-05-21 19:36:52.099241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/__init__.py
--rw-r--r--   0        0        0    39257 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/benchmark.py
--rw-r--r--   0        0        0     2926 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/results.py
--rw-r--r--   0        0        0     6456 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py
--rw-r--r--   0        0        0     8649 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py
--rw-r--r--   0        0        0     3467 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py
--rw-r--r--   0        0        0     7945 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py
--rw-r--r--   0        0        0      195 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/__init__.py
--rw-r--r--   0        0        0     8177 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark_complexity.py
--rw-r--r--   0        0        0     6578 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark_evaluation.py
--rw-r--r--   0        0        0    10115 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/classes.py
--rw-r--r--   0        0        0     3928 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/cli.py
--rw-r--r--   0        0        0      176 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/constants.py
--rw-r--r--   0        0        0      211 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/__init__.py
--rw-r--r--   0        0        0    10884 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/analysis.py
--rw-r--r--   0        0        0    17897 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/classes.py
--rw-r--r--   0        0        0    11765 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/derivation.py
--rw-r--r--   0        0        0     1285 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/derivation_show.py
--rw-r--r--   0        0        0     2087 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/library.py
--rw-r--r--   0        0        0        0 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/loaders/__init__.py
--rw-r--r--   0        0        0     9939 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/loaders/load_battledim.py
--rw-r--r--   0        0        0      880 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/loaders/load_dataset_base.py
--rw-r--r--   0        0        0     1288 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/evaluation_metrics/__init__.py
--rw-r--r--   0        0        0     9680 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/generator/__init__.py
--rw-r--r--   0        0        0    12993 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/generator/dataset_generator.py
--rw-r--r--   0        0        0     6332 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/generator/poulakis_network.py
--rw-r--r--   0        0        0      158 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/__init__.py
--rw-r--r--   0        0        0    13338 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/dualmethod.py
--rw-r--r--   0        0        0    19401 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/lila.py
--rw-r--r--   0        0        0    10445 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/mnf.py
--rw-r--r--   0        0        0     1171 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/null.py
--rw-r--r--   0        0        0     2033 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/random.py
--rw-r--r--   0        0        0        0 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/utils/__init__.py
--rw-r--r--   0        0        0     5309 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/methods/utils/cusum.py
--rw-r--r--   0        0        0     8349 2023-05-21 19:36:52.103241 ldimbenchmark-0.2.5/src/ldimbenchmark/utilities.py
--rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.5/setup.py
--rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     3330 2023-05-21 21:06:14.399657 ldimbenchmark-0.2.6/README.md
+-rw-r--r--   0        0        0     2359 2023-05-21 21:06:24.699523 ldimbenchmark-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/__init__.py
+-rw-r--r--   0        0        0    38982 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/benchmark.py
+-rw-r--r--   0        0        0     2926 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/results.py
+-rw-r--r--   0        0        0     6456 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py
+-rw-r--r--   0        0        0     8649 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py
+-rw-r--r--   0        0        0     3467 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py
+-rw-r--r--   0        0        0     7945 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py
+-rw-r--r--   0        0        0      195 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/runners/__init__.py
+-rw-r--r--   0        0        0     8019 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark_complexity.py
+-rw-r--r--   0        0        0     6578 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark_evaluation.py
+-rw-r--r--   0        0        0    10115 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/classes.py
+-rw-r--r--   0        0        0     3928 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/cli.py
+-rw-r--r--   0        0        0      176 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/constants.py
+-rw-r--r--   0        0        0      211 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/__init__.py
+-rw-r--r--   0        0        0    10884 2023-05-21 21:06:14.419657 ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/analysis.py
+-rw-r--r--   0        0        0    18600 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/classes.py
+-rw-r--r--   0        0        0    11765 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/derivation.py
+-rw-r--r--   0        0        0     1285 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/derivation_show.py
+-rw-r--r--   0        0        0     2087 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/library.py
+-rw-r--r--   0        0        0        0 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/loaders/__init__.py
+-rw-r--r--   0        0        0     9939 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/loaders/load_battledim.py
+-rw-r--r--   0        0        0      880 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/loaders/load_dataset_base.py
+-rw-r--r--   0        0        0     1288 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/evaluation_metrics/__init__.py
+-rw-r--r--   0        0        0     9680 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/generator/__init__.py
+-rw-r--r--   0        0        0    12993 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/generator/dataset_generator.py
+-rw-r--r--   0        0        0     6332 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/generator/poulakis_network.py
+-rw-r--r--   0        0        0      158 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/methods/__init__.py
+-rw-r--r--   0        0        0    13338 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/methods/dualmethod.py
+-rw-r--r--   0        0        0    19401 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/methods/lila.py
+-rw-r--r--   0        0        0    10445 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/methods/mnf.py
+-rw-r--r--   0        0        0     1171 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/methods/null.py
+-rw-r--r--   0        0        0     2033 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/methods/random.py
+-rw-r--r--   0        0        0        0 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/methods/utils/__init__.py
+-rw-r--r--   0        0        0     5309 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/methods/utils/cusum.py
+-rw-r--r--   0        0        0     8349 2023-05-21 21:06:14.423657 ldimbenchmark-0.2.6/src/ldimbenchmark/utilities.py
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.6/setup.py
+-rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.6/PKG-INFO
```

### Comparing `ldimbenchmark-0.2.5/README.md` & `ldimbenchmark-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/pyproject.toml` & `ldimbenchmark-0.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ldimbenchmark"
-version = "0.2.5"
+version = "0.2.6"
 description = ""
 authors = ["DanielHabenicht <daniel-habenicht@outlook.de>"]
 readme = "README.md"
 exclude = [
     "tests",
     "experiments"
 ]
```

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/benchmark.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,42 +493,38 @@
 
         self.methods_docker = self.methods_docker + methods
 
     def run_complexity_analysis(
         self,
         methods,
         style: Literal["time", "junctions"],
+        n_repeats=3,
+        n_measures=10,
+        n_max=91,
     ):
         complexity_results_path = os.path.join(self.complexity_results_dir, style)
         os.makedirs(complexity_results_path, exist_ok=True)
         hyperparameters_map = self._get_hyperparameters_for_methods_and_datasets(
             hyperparameters=self.hyperparameters,
             method_ids=[
                 get_method_name_from_docker_image(lmethod) for lmethod in methods
             ],
             dataset_base_ids=[],
         )
-        if style == "time":
-            return run_benchmark_complexity(
-                methods,
-                cache_dir=os.path.join(self.cache_dir, "datagen"),
-                out_folder=complexity_results_path,
-                style="time",
-                additionalOutput=self.debug,
-                hyperparameters=hyperparameters_map,
-            )
-        if style == "junctions":
-            return run_benchmark_complexity(
-                methods,
-                cache_dir=os.path.join(self.cache_dir, "datagen"),
-                out_folder=complexity_results_path,
-                style="junctions",
-                additionalOutput=self.debug,
-                hyperparameters=hyperparameters_map,
-            )
+        return run_benchmark_complexity(
+            methods,
+            cache_dir=os.path.join(self.cache_dir, "datagen"),
+            out_folder=complexity_results_path,
+            style=style,
+            additionalOutput=self.debug,
+            hyperparameters=hyperparameters_map,
+            n_repeats=n_repeats,
+            n_measures=n_measures,
+            n_max=n_max,
+        )
 
     def run_benchmark(
         self,
         evaluation_mode: Union["training", "evaluation"],
         use_cached=True,
         parallel=False,
         parallel_max_workers=0,
```

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/results.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/results.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark_complexity.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark_complexity.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,36 +43,42 @@
 def run_benchmark_complexity(
     methods: List[str],
     hyperparameters,
     cache_dir=os.path.join(LDIM_BENCHMARK_CACHE_DIR, "datagen"),
     out_folder="out/complexity",
     style=None,
     additionalOutput=False,
+    n_repeats=3,
+    n_measures=10,
+    n_max=91,
 ):
     """
     Run the benchmark for the given methods and datasets.
     :param methods: List of methods to run (only supports LocalMethodRunner currently)
     """
 
     if not os.path.exists(out_folder):
         os.mkdir(out_folder)
     logging.info("Complexity Analysis:")
     logging.info(" > Generating Datasets")
     if style == "time":
         datasets_dir = os.path.join(cache_dir, "synthetic-days")
-        generateDatasetsForTimespan(1, 91, datasets_dir)
+        generateDatasetsForTimespan(1, n_max, datasets_dir)
     if style == "junctions":
         datasets_dir = os.path.join(cache_dir, "synthetic-junctions")
-        generateDatasetsForJunctions(4, 59, datasets_dir)
+        generateDatasetsForJunctions(4, n_max, datasets_dir)
 
     dataset_dirs = glob(datasets_dir + "/*/")
+    min_n = 4
+    max_n = len(dataset_dirs)
+    n_samples = np.linspace(min_n, max_n, n_measures).astype("int64")
 
     manager = enlighten.get_manager()
     bar_loading_data = manager.counter(
-        total=len(dataset_dirs), desc="Loading data", unit="datasets"
+        total=len(dataset_dirs), desc="Validating data", unit="datasets"
     )
     bar_loading_data.update(incr=0)
 
     # logging.info(" > Loading Data")
     datasets = {}
     try:
         with ThreadPoolExecutor(max_workers=os.cpu_count()) as executor:
@@ -109,70 +115,62 @@
 
         try:
             image = client.images.get(method)
         except docker.errors.ImageNotFound:
             logging.info("Image does not exist. Pulling it...")
             client.images.pull(method)
 
-        min_n = 4
-        max_n = len(dataset_dirs)
-        n_measures = 10
-        n_repeats = 3
-        n_samples = np.linspace(min_n, max_n, n_measures).astype("int64")
-
-        for i, n in enumerate(n_samples):
-            summed_results = {"time": [], "ram": []}
-            for r in range(n_repeats):
+        summed_results = {"time": [], "ram": []}
+        for r in range(n_repeats):
+            for i, n in enumerate(n_samples):
                 complexity_benchmark_result_folder_run = os.path.join(
                     complexity_benchmark_result_folder, str(r)
                 )
                 runner = DockerMethodRunner(
                     method,
                     datasets[n],
                     "evaluation",
                     hyperparameters[method_name],
                     resultsFolder=complexity_benchmark_result_folder_run,
                     debug=additionalOutput,
                 )
-                runner.run()
+                runner.run(cpu_count=1, mem_limit="20g")
 
-                parallel = True
-                result_folders = glob(
-                    os.path.join(complexity_benchmark_result_folder_run, "*")
-                )
-                run_results = []
-                if parallel == True:
-                    with ProcessPoolExecutor() as executor:
-                        # submit all tasks and get future objects
-                        futures = [
-                            executor.submit(
-                                load_result, folder, try_load_docker_stats=True
-                            )
-                            for folder in result_folders
-                        ]
-                        # process results from tasks in order of task completion
-                        for future in as_completed(futures):
-                            result = future.result()
-                            run_results.append(result)
-                else:
-                    for experiment_result in result_folders:
-                        run_results.append(load_result(experiment_result, True))
-
-                run_results = pd.DataFrame(run_results)
-                run_results["number"] = (
-                    run_results["dataset"].str.split("-").str[2].astype(int)
-                )
-                sorted_results = run_results.sort_values(by=["number"])
-
-                summed_results["time"] = np.append(
-                    summed_results["time"], sorted_results["method_time"]
-                )
-                summed_results["ram"] = np.append(
-                    summed_results["ram"], sorted_results["memory_max"]
-                )
+            parallel = True
+            result_folders = glob(
+                os.path.join(complexity_benchmark_result_folder_run, "*")
+            )
+            run_results = []
+            if parallel == True:
+                with ProcessPoolExecutor() as executor:
+                    # submit all tasks and get future objects
+                    futures = [
+                        executor.submit(load_result, folder, try_load_docker_stats=True)
+                        for folder in result_folders
+                    ]
+                    # process results from tasks in order of task completion
+                    for future in as_completed(futures):
+                        result = future.result()
+                        run_results.append(result)
+            else:
+                for experiment_result in result_folders:
+                    run_results.append(load_result(experiment_result, True))
+
+            run_results = pd.DataFrame(run_results)
+            run_results["number"] = (
+                run_results["dataset"].str.split("-").str[2].astype(int)
+            )
+            sorted_results = run_results.sort_values(by=["number"])
+
+            summed_results["time"] = np.append(
+                summed_results["time"], sorted_results["method_time"]
+            )
+            summed_results["ram"] = np.append(
+                summed_results["ram"], sorted_results["memory_max"]
+            )
 
         best_cpu, rest = big_o.infer_big_o_class(
             sorted_results["number"],
             np.sum(summed_results["time"].reshape((len(n_samples), n_repeats)), axis=1),
         )
         best_ram, rest = big_o.infer_big_o_class(
             sorted_results["number"],
```

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/benchmark_evaluation.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/benchmark_evaluation.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/classes.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/classes.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/cli.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/cli.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/analysis.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/analysis.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/classes.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,16 @@
 
     def __init__(self, path):
         """
         :param path: Path to the dataset folder
         """
         self.path = path
         self.__pickle_path = os.path.join(self.path, "dataset.pickle")
-        self.__timestamp_path = os.path.join(self.path, ".timestamp")
+        self.__validation_file_name = ".validation"
+        self.__validation_path = os.path.join(self.path, self.__validation_file_name)
         path_to_dataset_info = os.path.join(self.path, "dataset_info.yaml")
         # Read dataset_info.yaml
         if os.path.isfile(path_to_dataset_info):
             # file exists
             with open(path_to_dataset_info) as f:
                 self.info: DatasetInfo = yaml.safe_load(f)
                 training_start = pd.to_datetime(
@@ -237,45 +238,59 @@
             # file exists
             with open(dma_path, "r") as f:
                 self.dmas = json.load(f)
         else:
             logging.warning("No dmas.json file found. Skipping loading of DMAs.")
             self.dmas = None
 
-    def _update_id(self):
+    def _update_id(self, force=False):
         """
         Sets the id (hash) according to the information in "dataset_info.yaml"
         """
+
+        derivations_hash = (
+            "-"
+            + hashlib.md5(
+                json.dumps(self.info, sort_keys=True, default=str).encode("utf-8")
+            ).hexdigest()
+        )
+        self.id = self.info["name"] + derivations_hash
+
+    def _generate_dataset_hash(self, folder: str):
+        new_hash = dirhash(folder, "md5", ignore_hidden=True)
+        with open(os.path.join(folder, self.__validation_file_name), "w") as f:
+            f.write(str(pd.to_datetime(datetime.now(), utc=True)) + "\n" + new_hash)
+
+    def is_valid(self) -> bool:
         # Check the has of the whole dataset from time to time by writing the last timestamp
         # to a file and retrieving it before running the expensive hash function
-
         md5hash = None
         try:
-            with open(self.__timestamp_path, "r") as f:
+            with open(self.__validation_path, "r") as f:
                 timestamp_file = f.readlines()
                 last_timestamp = pd.to_datetime(timestamp_file[0], utc=True)
                 md5hash = timestamp_file[1]
         except (FileNotFoundError, IndexError):
+            logging.warn("Dataset had no hashes for validation.")
             last_timestamp = None
 
         if last_timestamp is None or last_timestamp < pd.to_datetime(
             datetime.now(), utc=True
         ) - pd.Timedelta("24 hour"):
             logging.info("Checking dataset consistency...")
             new_hash = dirhash(self.path, "md5", ignore_hidden=True)
             if md5hash != None and md5hash != new_hash:
                 logging.info(
                     "Dataset hash changed! Check the consistency of the dataset!"
                 )
+                return False
             md5hash = new_hash
-            with open(self.__timestamp_path, "w") as f:
+            with open(self.__validation_path, "w") as f:
                 f.write(str(pd.to_datetime(datetime.now(), utc=True)) + "\n" + md5hash)
-
-        derivations_hash = "-" + md5hash
-        self.id = self.info["name"] + derivations_hash
+        return True
 
     ######
     # Getters and Setters with direct lazy loading because they
     ######
 
     @property
     def pressures(self) -> DataFrame:
@@ -424,14 +439,15 @@
 
         with open(os.path.join(folder, f"dataset_info.yaml"), "w") as f:
             yaml.dump(
                 self.info, f, sort_keys=False, default_flow_style=None, Dumper=TSDumper
             )
         if os.path.exists(self.__pickle_path):
             os.remove(self.__pickle_path)
+        self._generate_dataset_hash(folder)
 
 
 def getTimeSliceOfDataset(
     dataset: Dict[str, DataFrame],
     start: datetime,
     end: datetime,
     logging_dataset_name: str,
```

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/derivation.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/derivation.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/derivation_show.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/derivation_show.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/library.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/library.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/loaders/load_battledim.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/loaders/load_battledim.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/datasets/loaders/load_dataset_base.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/datasets/loaders/load_dataset_base.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/evaluation_metrics/__init__.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/evaluation_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/generator/__init__.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/generator/dataset_generator.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/generator/dataset_generator.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/generator/poulakis_network.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/generator/poulakis_network.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/methods/dualmethod.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/methods/dualmethod.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/methods/lila.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/methods/lila.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/methods/mnf.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/methods/mnf.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/methods/null.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/methods/null.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/methods/random.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/methods/random.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/methods/utils/cusum.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/methods/utils/cusum.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/src/ldimbenchmark/utilities.py` & `ldimbenchmark-0.2.6/src/ldimbenchmark/utilities.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.5/setup.py` & `ldimbenchmark-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
  'wntr>=0.5.0,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['ldimbenchmark = ldimbenchmark.cli:cli']}
 
 setup_kwargs = {
     'name': 'ldimbenchmark',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': '',
     'long_description': '[![ldimbenchmark version](https://badgen.net/pypi/v/ldimbenchmark/)](https://pypi.org/project/ldimbenchmark)\n[![Documentation badge](https://img.shields.io/badge/Documentation-here!-GREEN.svg)](https://tumt2022.github.io/LDIMBench/)\n\n# LDIMBenchmark\n\nLeakage Detection and Isolation Methods Benchmark\n\n> Instead of collecting all the different dataset to benchmark different methods on. We wanted to create a Benchmarking Tool which makes it easy to reproduce the results of the different methods locally on your own dataset.\n\nIt provides a close to real-world conditions environment and forces researchers to provide a reproducible method implementation, which is supposed to run automated on any input dataset, thus hindering custom solutions which work well in one specific case.\n\n## Usage\n\n### Installation\n\n```bash\npip install ldimbenchmark\n```\n\n### Python\n\n```python\nfrom ldimbenchmark.datasets import DatasetLibrary, DATASETS\nfrom ldimbenchmark import (\n    LDIMBenchmark,\n    BenchmarkData,\n    BenchmarkLeakageResult,\n)\nfrom ldimbenchmark.classes import LDIMMethodBase\nfrom typing import List\n\nclass YourCustomLDIMMethod(LDIMMethodBase):\n    def __init__(self):\n        super().__init__(\n            name="YourCustomLDIMMethod",\n            version="0.1.0"\n        )\n\n    def train(self, data: BenchmarkData):\n        pass\n\n    def detect(self, data: BenchmarkData) -> List[BenchmarkLeakageResult]:\n        return [\n            {\n                "leak_start": "2020-01-01",\n                "leak_end": "2020-01-02",\n                "leak_area": 0.2,\n                "pipe_id": "test",\n            }\n        ]\n\n    def detect_datapoint(self, evaluation_data) -> BenchmarkLeakageResult:\n        return {}\n\n\ndatasets = DatasetLibrary("datasets").download(DATASETS.BATTLEDIM)\n\nlocal_methods = [YourCustomLDIMMethod()]\n\nhyperparameters = {}\n\nbenchmark = LDIMBenchmark(\n    hyperparameters, datasets, results_dir="./benchmark-results"\n)\nbenchmark.add_local_methods(local_methods)\n\nbenchmark.run_benchmark()\n\nbenchmark.evaluate()\n```\n\n### CLI\n\n```bash\nldimbenchmark --help\n```\n\n## Roadmap\n\n- v1: Just Leakage Detection\n- v2: Provides Benchmark of Isolation Methods\n\nhttps://mathspp.com/blog/how-to-create-a-python-package-in-2022\n\n## Development\n\nhttps://python-poetry.org/docs/basic-usage/\n\n```bash\n# python 3.10\n# Use Environment\npoetry config virtualenvs.in-project true\npoetry shell\npoetry install --without ci # --with ci\n\n\n# Test\npoetry build\ncp -r dist tests/dist\ncd tests\ndocker build . -t testmethod\npytest -s -o log_cli=true\npytest tests/test_derivation.py -k \'test_mything\'\npytest --testmon\npytest --snapshot-update\n\n# Pytest watch\nptw\nptw -- --testmon\n\n# Watch a file during development\nnpm install -g nodemon\nnodemon -L experiments/auto_hyperparameter.py\n\n# Test-Publish\npoetry config repositories.testpypi https://test.pypi.org/legacy/\npoetry config http-basic.testpypi __token__ pypi-your-api-token-here\npoetry build\npoetry publish -r testpypi\n\n# Real Publish\npoetry config pypi-token.pypi pypi-your-token-here\n```\n\n### Documentation\n\nhttps://squidfunk.github.io/mkdocs-material/\nhttps://click.palletsprojects.com/en/8.1.x/\n\n```\nmkdocs serve\n```\n\n# TODO\n\nLDIMBenchmark:\nData Cleansing before working with them\n\n- per sensor type, e.g. waterflow (cut of at 0)\n- removing datapoints which are clearly a malfunction\n',
     'author': 'DanielHabenicht',
     'author_email': 'daniel-habenicht@outlook.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ldimbenchmark-0.2.5/PKG-INFO` & `ldimbenchmark-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldimbenchmark
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 Author: DanielHabenicht
 Author-email: daniel-habenicht@outlook.de
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

