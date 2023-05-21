# Comparing `tmp/ldimbenchmark-0.2.2.tar.gz` & `tmp/ldimbenchmark-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldimbenchmark-0.2.2.tar", max compression
+gzip compressed data, was "ldimbenchmark-0.2.3.tar", max compression
```

## Comparing `ldimbenchmark-0.2.2.tar` & `ldimbenchmark-0.2.3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     3330 2023-05-20 17:38:31.891433 ldimbenchmark-0.2.2/README.md
--rw-r--r--   0        0        0     2359 2023-05-20 17:38:43.263574 ldimbenchmark-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      158 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/__init__.py
--rw-r--r--   0        0        0       60 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark/__init__.py
--rw-r--r--   0        0        0    40659 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark/benchmark.py
--rw-r--r--   0        0        0     6456 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py
--rw-r--r--   0        0        0     8655 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py
--rw-r--r--   0        0        0     3467 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py
--rw-r--r--   0        0        0     7945 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py
--rw-r--r--   0        0        0      195 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark/runners/__init__.py
--rw-r--r--   0        0        0     5440 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark_complexity.py
--rw-r--r--   0        0        0     6578 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark_evaluation.py
--rw-r--r--   0        0        0    10115 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/classes.py
--rw-r--r--   0        0        0     3928 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/cli.py
--rw-r--r--   0        0        0      176 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/constants.py
--rw-r--r--   0        0        0      211 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/__init__.py
--rw-r--r--   0        0        0    10884 2023-05-20 17:38:31.911434 ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/analysis.py
--rw-r--r--   0        0        0    17897 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/classes.py
--rw-r--r--   0        0        0    11765 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/derivation.py
--rw-r--r--   0        0        0     1285 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/derivation_show.py
--rw-r--r--   0        0        0     2087 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/library.py
--rw-r--r--   0        0        0        0 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/loaders/__init__.py
--rw-r--r--   0        0        0     9939 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/loaders/load_battledim.py
--rw-r--r--   0        0        0      880 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/loaders/load_dataset_base.py
--rw-r--r--   0        0        0     1288 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/evaluation_metrics/__init__.py
--rw-r--r--   0        0        0     9680 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/generator/__init__.py
--rw-r--r--   0        0        0    12993 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/generator/dataset_generator.py
--rw-r--r--   0        0        0     6332 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/generator/poulakis_network.py
--rw-r--r--   0        0        0      158 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/methods/__init__.py
--rw-r--r--   0        0        0    13338 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/methods/dualmethod.py
--rw-r--r--   0        0        0    19401 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/methods/lila.py
--rw-r--r--   0        0        0    10445 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/methods/mnf.py
--rw-r--r--   0        0        0     1171 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/methods/null.py
--rw-r--r--   0        0        0     2033 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/methods/random.py
--rw-r--r--   0        0        0        0 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/methods/utils/__init__.py
--rw-r--r--   0        0        0     5309 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/methods/utils/cusum.py
--rw-r--r--   0        0        0     8229 2023-05-20 17:38:31.915434 ldimbenchmark-0.2.2/src/ldimbenchmark/utilities.py
--rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.2/setup.py
--rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3330 2023-05-21 15:03:38.439758 ldimbenchmark-0.2.3/README.md
+-rw-r--r--   0        0        0     2359 2023-05-21 15:03:49.324260 ldimbenchmark-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark/__init__.py
+-rw-r--r--   0        0        0    39257 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark/benchmark.py
+-rw-r--r--   0        0        0     2930 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark/results.py
+-rw-r--r--   0        0        0     6456 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py
+-rw-r--r--   0        0        0     8649 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py
+-rw-r--r--   0        0        0     3467 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py
+-rw-r--r--   0        0        0     7945 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py
+-rw-r--r--   0        0        0      195 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark/runners/__init__.py
+-rw-r--r--   0        0        0     7388 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark_complexity.py
+-rw-r--r--   0        0        0     6578 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark_evaluation.py
+-rw-r--r--   0        0        0    10115 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/classes.py
+-rw-r--r--   0        0        0     3928 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/cli.py
+-rw-r--r--   0        0        0      176 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/constants.py
+-rw-r--r--   0        0        0      211 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/__init__.py
+-rw-r--r--   0        0        0    10884 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/analysis.py
+-rw-r--r--   0        0        0    17897 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/classes.py
+-rw-r--r--   0        0        0    11765 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/derivation.py
+-rw-r--r--   0        0        0     1285 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/derivation_show.py
+-rw-r--r--   0        0        0     2087 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/library.py
+-rw-r--r--   0        0        0        0 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/loaders/__init__.py
+-rw-r--r--   0        0        0     9939 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/loaders/load_battledim.py
+-rw-r--r--   0        0        0      880 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/loaders/load_dataset_base.py
+-rw-r--r--   0        0        0     1288 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/evaluation_metrics/__init__.py
+-rw-r--r--   0        0        0     9680 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/generator/__init__.py
+-rw-r--r--   0        0        0    12993 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/generator/dataset_generator.py
+-rw-r--r--   0        0        0     6332 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/generator/poulakis_network.py
+-rw-r--r--   0        0        0      158 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/methods/__init__.py
+-rw-r--r--   0        0        0    13338 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/methods/dualmethod.py
+-rw-r--r--   0        0        0    19401 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/methods/lila.py
+-rw-r--r--   0        0        0    10445 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/methods/mnf.py
+-rw-r--r--   0        0        0     1171 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/methods/null.py
+-rw-r--r--   0        0        0     2033 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/methods/random.py
+-rw-r--r--   0        0        0        0 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/methods/utils/__init__.py
+-rw-r--r--   0        0        0     5309 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/methods/utils/cusum.py
+-rw-r--r--   0        0        0     8349 2023-05-21 15:03:38.459758 ldimbenchmark-0.2.3/src/ldimbenchmark/utilities.py
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.3/setup.py
+-rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.3/PKG-INFO
```

### Comparing `ldimbenchmark-0.2.2/README.md` & `ldimbenchmark-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/pyproject.toml` & `ldimbenchmark-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ldimbenchmark"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["DanielHabenicht <daniel-habenicht@outlook.de>"]
 readme = "README.md"
 exclude = [
     "tests",
     "experiments"
 ]
```

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark/benchmark.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark/benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from concurrent.futures import ThreadPoolExecutor, as_completed
 import itertools
 
 from numpy import timedelta64
+from ldimbenchmark.benchmark.results import load_result
 from ldimbenchmark.benchmark.runners import DockerMethodRunner, LocalMethodRunner
 from ldimbenchmark.benchmark.runners.BaseMethodRunner import MethodRunner
 from ldimbenchmark.datasets import Dataset
 import pandas as pd
 import numpy as np
 from typing import Dict, Literal, TypedDict, Union, List, Callable
 import os
 import logging
 from ldimbenchmark.constants import CPU_COUNT, LDIM_BENCHMARK_CACHE_DIR
 from glob import glob
-from ldimbenchmark.benchmark_evaluation import evaluate_leakages
 from tabulate import tabulate
 from ldimbenchmark.benchmark_complexity import run_benchmark_complexity
 import matplotlib.pyplot as plt
 import enlighten
 from ldimbenchmark.evaluation_metrics import (
     precision,
     recall,
@@ -30,14 +30,16 @@
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 from matplotlib import patches
 import ast
 import seaborn as sns
 from matplotlib.ticker import FormatStrFormatter
 
+from ldimbenchmark.utilities import get_method_name_from_docker_image
+
 
 def execute_experiment(experiment: MethodRunner):
     """
     Private method for running an experiment in a separate process.
     """
     return experiment.run()
 
@@ -242,52 +244,14 @@
     # Put a legend to the right of the current axis
     # ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
     fig.suptitle(name)
     fig.savefig(os.path.join(out_dir, name + ".png"))
     plt.close(fig)
 
 
-def load_result(folder: str) -> Dict:
-    folder = os.path.join(folder, "")
-    detected_leaks_file = os.path.join(folder, "detected_leaks.csv")
-    if not os.path.exists(detected_leaks_file):
-        return {}
-
-    detected_leaks = pd.read_csv(
-        detected_leaks_file,
-        parse_dates=True,
-        date_parser=lambda x: pd.to_datetime(x, utc=True),
-    )
-
-    evaluation_dataset_leakages = pd.read_csv(
-        os.path.join(folder, "should_have_detected_leaks.csv"),
-        parse_dates=True,
-        date_parser=lambda x: pd.to_datetime(x, utc=True),
-    )
-
-    run_info = pd.read_csv(os.path.join(folder, "run_info.csv")).iloc[0]
-
-    # TODO: Ignore Detections outside of the evaluation period
-    (evaluation_results, matched_list) = evaluate_leakages(
-        evaluation_dataset_leakages, detected_leaks
-    )
-    evaluation_results["method"] = run_info["method"]
-    evaluation_results["method_version"] = run_info.get("method_version", None)
-    evaluation_results["dataset"] = run_info["dataset"]
-    evaluation_results["dataset_part"] = run_info.get("dataset_part", None)
-    evaluation_results["dataset_id"] = run_info["dataset_id"]
-    evaluation_results["dataset_derivations"] = run_info["dataset_options"]
-    evaluation_results["hyperparameters"] = run_info["hyperparameters"]
-    evaluation_results["matched_leaks_list"] = matched_list
-    evaluation_results["_folder"] = os.path.basename(os.path.dirname(folder))
-    evaluation_results["executed_at"] = run_info.get("executed_at", None)
-
-    return evaluation_results
-
-
 def create_plots(
     results: pd.DataFrame,
     method: str,
     dataset: str,
     hyperparameters: List[str],
     performance_metric: str,
     out_folder,
@@ -534,15 +498,17 @@
         methods,
         style: Literal["time", "junctions"],
     ):
         complexity_results_path = os.path.join(self.complexity_results_dir, style)
         os.makedirs(complexity_results_path, exist_ok=True)
         hyperparameters_map = self._get_hyperparameters_for_methods_and_datasets(
             hyperparameters=self.hyperparameters,
-            method_ids=[lmethod.name for lmethod in methods],
+            method_ids=[
+                get_method_name_from_docker_image(lmethod) for lmethod in methods
+            ],
             dataset_base_ids=[],
         )
         if style == "time":
             return run_benchmark_complexity(
                 methods,
                 cache_dir=os.path.join(self.cache_dir, "datagen"),
                 out_folder=complexity_results_path,
@@ -583,15 +549,16 @@
             raise ValueError("Cannot run local and docker methods at the same time")
 
         logging.info("Starting Benchmark")
         logging.info("Preparing Hyperparameters")
         hyperparameters_map = self._get_hyperparameters_for_methods_and_datasets(
             hyperparameters=self.hyperparameters,
             method_ids=[
-                dmethod.split(":")[0].split("/")[-1] for dmethod in self.methods_docker
+                get_method_name_from_docker_image(dmethod)
+                for dmethod in self.methods_docker
             ]
             + [lmethod.name for lmethod in self.methods_local],
             dataset_base_ids=[dataset.id for dataset in self.datasets],
         )
 
         # TODO: Move to parallel step execution step in run_benchmark, but still validate at least once
         for dataset in self.datasets:
```

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,16 +178,16 @@
             status = container.wait()
             if status["StatusCode"] != 0:
                 killEvent.set()
                 thread.join()
                 logging.error(
                     f"Runner {self.id} errored with status code {status['StatusCode']}!"
                 )
-                # for line in e.container.logs().decode().split("\n"):
-                #     logging.error(f"Container[{self.image}]: " + line)
+                for line in container.logs().decode().split("\n"):
+                    logging.error(f"Container[{self.image}]: " + line)
                 if status["StatusCode"] == 137:
                     logging.error("Process in container was killed.")
                     logging.error(
                         "This might be due to a memory limit. Try increasing the memory limit or reduce the amount of parallel processes."
                     )
                 if not self.debug:
                     container.remove()
```

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark_complexity.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark_complexity.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor, as_completed
 import importlib
 import os
 import time
 from datetime import datetime
 from glob import glob
 import logging
+import docker
 
 import enlighten
+from ldimbenchmark.benchmark.results import load_result
+from ldimbenchmark.benchmark.runners import DockerMethodRunner
 from ldimbenchmark.constants import LDIM_BENCHMARK_CACHE_DIR
 from ldimbenchmark.datasets import Dataset
 from ldimbenchmark.generator import (
     generateDatasetsForTimespan,
     generateDatasetsForJunctions,
 )
 from ldimbenchmark.classes import LDIMMethodBase
@@ -18,27 +21,31 @@
 import pandas as pd
 import wntr
 import yaml
 import big_o
 import matplotlib as mpl
 from typing import List
 
+from ldimbenchmark.utilities import get_method_name_from_docker_image
+
 
 def loadDataset_local(dataset_path):
-    dataset = Dataset(dataset_path).loadData().loadBenchmarkData()
+    dataset = Dataset(dataset_path)  # .loadData().loadBenchmarkData()
+    # dataset.is_valid()
     number = int(os.path.basename(os.path.normpath(dataset_path)).split("-")[-1])
     return (
         number,
-        dataset.getTrainingBenchmarkData(),
-        dataset.getEvaluationBenchmarkData(),
+        dataset
+        # dataset.getTrainingBenchmarkData(),
+        # dataset.getEvaluationBenchmarkData(),
     )
 
 
 def run_benchmark_complexity(
-    methods: List[LDIMMethodBase],
+    methods: List[str],
     hyperparameters,
     cache_dir=os.path.join(LDIM_BENCHMARK_CACHE_DIR, "datagen"),
     out_folder="out/complexity",
     style=None,
     additionalOutput=False,
 ):
     """
@@ -61,93 +68,132 @@
 
     manager = enlighten.get_manager()
     bar_loading_data = manager.counter(
         total=len(dataset_dirs), desc="Loading data", unit="datasets"
     )
     bar_loading_data.update(incr=0)
 
-    logging.info(" > Loading Data")
+    # logging.info(" > Loading Data")
     datasets = {}
     try:
         with ThreadPoolExecutor(max_workers=os.cpu_count()) as executor:
             # submit all tasks and get future objects
             futures = [
                 executor.submit(loadDataset_local, dataset_dir)
                 for dataset_dir in dataset_dirs
             ]
             # process results from tasks in order of task completion
             for future in as_completed(futures):
-                dataset_id, training, evaluation = future.result()
-                datasets[dataset_id] = {}
-                datasets[dataset_id]["training"] = training
-                datasets[dataset_id]["evaluation"] = evaluation
+                dataset_id, dataset = future.result()
+                datasets[dataset_id] = dataset
                 bar_loading_data.update()
     except KeyboardInterrupt:
         manager.stop()
         executor._processes.clear()
         os.kill(os.getpid(), 9)
     bar_loading_data.close()
 
-    results = {}
+    results = {"time": {}, "ram": {}}
     result_measures = []
 
     bar_running_analysis = manager.counter(
         total=len(methods), desc="Running Analysis", unit="methods"
     )
     logging.info(" > Starting Complexity analysis")
     for method in methods:
-        logging.info(f" - {method.name}")
+        method_name = get_method_name_from_docker_image(method)
+        logging.info(f" - {method_name}")
+        complexity_benchmark_result_folder = os.path.join(
+            out_folder, "runs", method_name, "1"
+        )
+        client = docker.from_env()
 
-        if additionalOutput:
-            method.init_with_benchmark_params(
-                additional_output_path=os.path.join(
-                    out_folder, "additional_output_path"
-                ),
-                hyperparameters=hyperparameters[method.name],
+        try:
+            image = client.images.get(method)
+        except docker.errors.ImageNotFound:
+            logging.info("Image does not exist. Pulling it...")
+            client.images.pull(method)
+
+        min_n = 4
+        max_n = len(dataset_dirs)
+        n_measures = 10
+        n_repeats = 3
+        n_samples = np.linspace(min_n, max_n, n_measures).astype("int64")
+
+        for i, n in enumerate(n_samples):
+            for r in range(n_repeats):
+                complexity_benchmark_result_folder_run = os.path.join(
+                    complexity_benchmark_result_folder, str(r)
+                )
+            runner = DockerMethodRunner(
+                method,
+                datasets[n],
+                "evaluation",
+                hyperparameters[method_name],
+                resultsFolder=complexity_benchmark_result_folder,
+                debug=additionalOutput,
             )
+            runner.run()
+
+        bar_running_analysis.close()
+        manager.stop()
+
+        parallel = True
+        result_folders = glob(os.path.join(complexity_benchmark_result_folder, "*"))
+        run_results = []
+        if parallel == True:
+            with ProcessPoolExecutor() as executor:
+                # submit all tasks and get future objects
+                futures = [
+                    executor.submit(load_result, folder, try_load_docker_stats=True)
+                    for folder in result_folders
+                ]
+                # process results from tasks in order of task completion
+                for future in as_completed(futures):
+                    result = future.result()
+                    run_results.append(result)
         else:
-            method.init_with_benchmark_params(
-                additional_output_path=None,
-                hyperparameters=hyperparameters[method.name],
-            )
+            for experiment_result in result_folders:
+                run_results.append(load_result(experiment_result, True))
 
-        def runAlgorithmWithNetwork(n):
-            method.prepare(datasets[n]["training"])
-            method.detect_offline(datasets[n]["evaluation"])
-
-        # Run Big-O
-        best, others = big_o.big_o(
-            runAlgorithmWithNetwork,
-            big_o.datagen.n_,
-            min_n=4,
-            max_n=len(dataset_dirs),
-            n_measures=10,
-            n_repeats=3,
-            return_raw_data=True,
+        run_results = pd.DataFrame(run_results)
+        run_results["number"] = run_results["dataset"].str.split("-").str[2].astype(int)
+        sorted_results = run_results.sort_values(by=["number"])
+        best_cpu, rest = big_o.infer_big_o_class(
+            sorted_results["number"], sorted_results["method_time"]
+        )
+        best_ram, rest = big_o.infer_big_o_class(
+            sorted_results["number"], sorted_results["memory_avg"]
         )
-        results[method.name] = best
 
-        measures = pd.DataFrame({"times": others["times"]}, index=others["measures"])
-        result_measures.append(measures.rename(columns={"times": method.name}))
-        measures.to_csv(os.path.join(out_folder, "measures_raw.csv"))
-        pd.DataFrame(list(others.items())[1:8]).to_csv(
-            os.path.join(out_folder, "big_o.csv"), header=False, index=False
+        results["time"][method] = best_cpu
+        results["ram"][method] = best_ram
+
+        measures = pd.DataFrame(
+            {
+                f"time_{method_name}": sorted_results["method_time"].to_list(),
+                f"ram_{method_name}": sorted_results["memory_max"].to_list(),
+            },
+            index=sorted_results["number"].to_list(),
         )
+        result_measures.append(measures)
+        # measures.to_csv(os.path.join(out_folder, "measures_raw.csv"))
+        # pd.DataFrame(list(others.items())[1:8]).to_csv(
+        #     os.path.join(out_folder, "big_o.csv"), header=False, index=False
+        # )
         bar_running_analysis.update()
         # Cooldown for 10 seconds
         time.sleep(10)
 
-    bar_running_analysis.close()
-    manager.stop()
-
     logging.info(f"Exporting results to {out_folder}")
     results = pd.DataFrame(
         {
-            "Leakage Detection Method": results.keys(),
-            "Time Complexity": results.values(),
+            "Leakage Detection Method": results["time"].keys(),
+            "Time Complexity": results["time"].values(),
+            "RAM Complexity": results["ram"].values(),
         }
     )
     results.to_csv(os.path.join(out_folder, "results.csv"), index=False)
 
     # TODO: Escape complexity formula into math mode
     results.style.hide(axis="index").to_latex(os.path.join(out_folder, "results.tex"))
```

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/benchmark_evaluation.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/benchmark_evaluation.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/classes.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/classes.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/cli.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/cli.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/analysis.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/analysis.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/classes.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/classes.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/derivation.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/derivation.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/derivation_show.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/derivation_show.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/library.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/library.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/loaders/load_battledim.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/loaders/load_battledim.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/datasets/loaders/load_dataset_base.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/datasets/loaders/load_dataset_base.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/evaluation_metrics/__init__.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/evaluation_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/generator/__init__.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/generator/dataset_generator.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/generator/dataset_generator.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/generator/poulakis_network.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/generator/poulakis_network.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/methods/dualmethod.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/methods/dualmethod.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/methods/lila.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/methods/lila.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/methods/mnf.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/methods/mnf.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/methods/null.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/methods/null.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/methods/random.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/methods/random.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/methods/utils/cusum.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/methods/utils/cusum.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.2.2/src/ldimbenchmark/utilities.py` & `ldimbenchmark-0.2.3/src/ldimbenchmark/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,7 +248,11 @@
 
 
 def _reduce_hash(hashlist, hashfunc):
     hasher = hashfunc()
     for hashvalue in sorted(hashlist):
         hasher.update(hashvalue.encode("utf-8"))
     return hasher.hexdigest()
+
+
+def get_method_name_from_docker_image(docker_image: str) -> str:
+    return docker_image.split(":")[0].split("/")[-1]
```

### Comparing `ldimbenchmark-0.2.2/setup.py` & `ldimbenchmark-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
  'wntr>=0.5.0,<0.6.0']
 
 entry_points = \
 {'console_scripts': ['ldimbenchmark = ldimbenchmark.cli:cli']}
 
 setup_kwargs = {
     'name': 'ldimbenchmark',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': '',
     'long_description': '[![ldimbenchmark version](https://badgen.net/pypi/v/ldimbenchmark/)](https://pypi.org/project/ldimbenchmark)\n[![Documentation badge](https://img.shields.io/badge/Documentation-here!-GREEN.svg)](https://tumt2022.github.io/LDIMBench/)\n\n# LDIMBenchmark\n\nLeakage Detection and Isolation Methods Benchmark\n\n> Instead of collecting all the different dataset to benchmark different methods on. We wanted to create a Benchmarking Tool which makes it easy to reproduce the results of the different methods locally on your own dataset.\n\nIt provides a close to real-world conditions environment and forces researchers to provide a reproducible method implementation, which is supposed to run automated on any input dataset, thus hindering custom solutions which work well in one specific case.\n\n## Usage\n\n### Installation\n\n```bash\npip install ldimbenchmark\n```\n\n### Python\n\n```python\nfrom ldimbenchmark.datasets import DatasetLibrary, DATASETS\nfrom ldimbenchmark import (\n    LDIMBenchmark,\n    BenchmarkData,\n    BenchmarkLeakageResult,\n)\nfrom ldimbenchmark.classes import LDIMMethodBase\nfrom typing import List\n\nclass YourCustomLDIMMethod(LDIMMethodBase):\n    def __init__(self):\n        super().__init__(\n            name="YourCustomLDIMMethod",\n            version="0.1.0"\n        )\n\n    def train(self, data: BenchmarkData):\n        pass\n\n    def detect(self, data: BenchmarkData) -> List[BenchmarkLeakageResult]:\n        return [\n            {\n                "leak_start": "2020-01-01",\n                "leak_end": "2020-01-02",\n                "leak_area": 0.2,\n                "pipe_id": "test",\n            }\n        ]\n\n    def detect_datapoint(self, evaluation_data) -> BenchmarkLeakageResult:\n        return {}\n\n\ndatasets = DatasetLibrary("datasets").download(DATASETS.BATTLEDIM)\n\nlocal_methods = [YourCustomLDIMMethod()]\n\nhyperparameters = {}\n\nbenchmark = LDIMBenchmark(\n    hyperparameters, datasets, results_dir="./benchmark-results"\n)\nbenchmark.add_local_methods(local_methods)\n\nbenchmark.run_benchmark()\n\nbenchmark.evaluate()\n```\n\n### CLI\n\n```bash\nldimbenchmark --help\n```\n\n## Roadmap\n\n- v1: Just Leakage Detection\n- v2: Provides Benchmark of Isolation Methods\n\nhttps://mathspp.com/blog/how-to-create-a-python-package-in-2022\n\n## Development\n\nhttps://python-poetry.org/docs/basic-usage/\n\n```bash\n# python 3.10\n# Use Environment\npoetry config virtualenvs.in-project true\npoetry shell\npoetry install --without ci # --with ci\n\n\n# Test\npoetry build\ncp -r dist tests/dist\ncd tests\ndocker build . -t testmethod\npytest -s -o log_cli=true\npytest tests/test_derivation.py -k \'test_mything\'\npytest --testmon\npytest --snapshot-update\n\n# Pytest watch\nptw\nptw -- --testmon\n\n# Watch a file during development\nnpm install -g nodemon\nnodemon -L experiments/auto_hyperparameter.py\n\n# Test-Publish\npoetry config repositories.testpypi https://test.pypi.org/legacy/\npoetry config http-basic.testpypi __token__ pypi-your-api-token-here\npoetry build\npoetry publish -r testpypi\n\n# Real Publish\npoetry config pypi-token.pypi pypi-your-token-here\n```\n\n### Documentation\n\nhttps://squidfunk.github.io/mkdocs-material/\nhttps://click.palletsprojects.com/en/8.1.x/\n\n```\nmkdocs serve\n```\n\n# TODO\n\nLDIMBenchmark:\nData Cleansing before working with them\n\n- per sensor type, e.g. waterflow (cut of at 0)\n- removing datapoints which are clearly a malfunction\n',
     'author': 'DanielHabenicht',
     'author_email': 'daniel-habenicht@outlook.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ldimbenchmark-0.2.2/PKG-INFO` & `ldimbenchmark-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldimbenchmark
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: DanielHabenicht
 Author-email: daniel-habenicht@outlook.de
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

