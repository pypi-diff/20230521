# Comparing `tmp/mlflow_tmp-2.2.9.tar.gz` & `tmp/mlflow_tmp-2.3.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_tmp-2.2.9.tar", last modified: Sun May 21 00:15:09 2023, max compression
+gzip compressed data, was "mlflow_tmp-2.3.3.dev0.tar", last modified: Fri May 19 04:30:58 2023, max compression
```

## Comparing `mlflow_tmp-2.2.9.tar` & `mlflow_tmp-2.3.3.dev0.tar`

### file list

```diff
@@ -1,440 +1,439 @@
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.956612 mlflow_tmp-2.2.9/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11382 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/LICENSE.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      562 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/MANIFEST.in
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10474 2023-05-21 00:15:09.956612 mlflow_tmp-2.2.9/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9767 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/README.rst
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      949 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/README_SKINNY.rst
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.932612 mlflow_tmp-2.2.9/mlflow/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6215 2023-05-18 22:57:23.000000 mlflow_tmp-2.2.9/mlflow/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       39 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/__main__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3668 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/_doctor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9428 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/_spark_autologging.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.932612 mlflow_tmp-2.2.9/mlflow/artifacts/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6485 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/artifacts/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.932612 mlflow_tmp-2.2.9/mlflow/azure/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/azure/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11647 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/azure/client.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    15140 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/catboost.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    23356 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/cli.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      407 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/client.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      881 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/db.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.932612 mlflow_tmp-2.2.9/mlflow/deployments/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3797 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/deployments/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    15572 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/deployments/base.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    15078 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/deployments/cli.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3825 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/deployments/interface.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5512 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/deployments/plugin_manager.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      556 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/deployments/utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    28178 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/diviner.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.932612 mlflow_tmp-2.2.9/mlflow/entities/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      948 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1414 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/_mlflow_object.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3510 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/experiment.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      887 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/experiment_tag.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1215 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/file_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1242 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/lifecycle_stage.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1418 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/metric.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.932612 mlflow_tmp-2.2.9/mlflow/entities/model_registry/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      529 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/model_registry/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      286 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/model_registry/_model_registry_entity.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6435 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/model_registry/model_version.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      831 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/model_registry/model_version_stages.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1533 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/model_registry/model_version_status.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      933 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/model_registry/model_version_tag.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4933 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/model_registry/registered_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1053 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/model_registry/registered_model_alias.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      948 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/model_registry/registered_model_tag.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1133 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/param.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1438 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/run.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3032 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/run_data.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6182 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/run_info.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1550 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/run_status.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      890 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/run_tag.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1212 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/source_type.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1826 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/entities/view_type.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10192 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/environment_variables.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4881 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/exceptions.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5080 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/experiments.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.932612 mlflow_tmp-2.2.9/mlflow/fastai/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    25354 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/fastai/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5757 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/fastai/callback.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.932612 mlflow_tmp-2.2.9/mlflow/gluon/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    19063 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/gluon/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2020 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/gluon/_autolog.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    14185 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/h2o.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10155 2023-05-20 03:22:38.000000 mlflow_tmp-2.2.9/mlflow/johnsnowlabs.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    36523 2023-05-21 00:10:12.000000 mlflow_tmp-2.2.9/mlflow/johnsnowlabs2.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      311 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/keras.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.932612 mlflow_tmp-2.2.9/mlflow/langchain/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    20905 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/langchain/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4846 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/langchain/api_request_parallel_processor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    35902 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/lightgbm.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      180 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/llm.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5575 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/ml_package_versions.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    13885 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/mleap.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.936612 mlflow_tmp-2.2.9/mlflow/models/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3627 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9803 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/cli.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.936612 mlflow_tmp-2.2.9/mlflow/models/container/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9387 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/container/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.936612 mlflow_tmp-2.2.9/mlflow/models/container/scoring_server/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/container/scoring_server/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      712 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/container/scoring_server/nginx.conf
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      131 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/container/scoring_server/wsgi.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9853 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/docker_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.936612 mlflow_tmp-2.2.9/mlflow/models/evaluation/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      491 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/evaluation/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3105 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/evaluation/_shap_patch.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6769 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/evaluation/artifacts.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    59488 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/evaluation/base.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    50976 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/evaluation/default_evaluator.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2036 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/evaluation/evaluator_registry.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6223 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/evaluation/lift_curve.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10946 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/evaluation/validation.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3420 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/flavor_backend.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2354 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/flavor_backend_registry.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    24148 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8634 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/signature.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    38161 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11707 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/models/wheeled_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    21826 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/onnx.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.936612 mlflow_tmp-2.2.9/mlflow/openai/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    23265 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/openai/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12309 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/openai/api_request_parallel_processor.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2936 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/openai/retry.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2088 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/openai/utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.936612 mlflow_tmp-2.2.9/mlflow/paddle/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    23859 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/paddle/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4792 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/paddle/_paddle_autolog.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    17616 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pmdarima.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.936612 mlflow_tmp-2.2.9/mlflow/projects/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    17396 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/projects/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11532 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/projects/_project_spec.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.936612 mlflow_tmp-2.2.9/mlflow/projects/backend/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      271 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/projects/backend/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2210 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/projects/backend/abstract_backend.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1079 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/projects/backend/loader.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    17240 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/projects/backend/local.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    20270 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/projects/databricks.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6394 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/projects/docker.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       94 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/projects/env_type.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6379 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/projects/kubernetes.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3574 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/projects/submitted_run.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    13432 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/projects/utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    14024 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/prophet.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.936612 mlflow_tmp-2.2.9/mlflow/protos/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/protos/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    17261 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/protos/databricks_artifacts_pb2.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    14095 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/protos/databricks_pb2.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    39471 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/protos/databricks_uc_registry_messages_pb2.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12471 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/protos/databricks_uc_registry_service_pb2.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    16146 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/protos/facet_feature_statistics_pb2.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8552 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/protos/mlflow_artifacts_pb2.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    54475 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/protos/model_registry_pb2.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.936612 mlflow_tmp-2.2.9/mlflow/protos/scalapb/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/protos/scalapb/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3307 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/protos/scalapb/scalapb_pb2.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    48593 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/protos/service_pb2.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/pyfunc/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    81412 2023-05-18 21:22:32.000000 mlflow_tmp-2.2.9/mlflow/pyfunc/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    16640 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pyfunc/backend.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      901 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pyfunc/mlserver.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    15392 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pyfunc/model.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/pyfunc/scoring_server/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    13910 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pyfunc/scoring_server/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4222 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pyfunc/scoring_server/client.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      175 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pyfunc/scoring_server/wsgi.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2124 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pyfunc/spark_model_cache.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1001 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pyfunc/stdin_server.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)  7197781 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pypi_package_index.json
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/pyspark/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       50 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pyspark/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/pyspark/ml/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    53458 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pyspark/ml/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2908 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pyspark/ml/_autolog.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1886 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pyspark/ml/log_model_allowlist.txt
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/pytorch/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    45379 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pytorch/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    17629 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pytorch/_lightning_autolog.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2654 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pytorch/_pytorch_autolog.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2090 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/pytorch/pickle_module.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/recipes/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1330 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6092 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/artifacts.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/recipes/cards/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10229 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/cards/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4780 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/cards/histogram_generator.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12548 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/cards/pandas_renderer.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/recipes/cards/templates/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/cards/templates/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3488 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/cards/templates/base.html
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/recipes/classification/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/classification/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/recipes/classification/v1/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      122 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/classification/v1/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    20462 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/classification/v1/recipe.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2917 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/cli.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    18431 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/dag_help_strings.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    17933 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/recipe.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/recipes/regression/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/regression/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/recipes/regression/v1/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      114 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/regression/v1/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    22495 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/regression/v1/recipe.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/recipes/resources/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12211 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/resources/recipe_dag_template.html
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    14988 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/step.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/recipes/steps/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/steps/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/recipes/steps/automl/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/steps/automl/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6269 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/steps/automl/flaml.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    20717 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/steps/evaluate.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/recipes/steps/ingest/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11137 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/steps/ingest/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    26446 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/steps/ingest/datasets.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12132 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/steps/predict.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     7680 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/steps/register.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    19541 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/steps/split.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    59789 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/steps/train.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10602 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/steps/transform.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/recipes/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6355 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    28468 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/utils/execution.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8990 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/utils/metrics.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     7392 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/utils/step.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12375 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/utils/tracking.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1748 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/recipes/utils/wrapped_recipe_model.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/rfunc/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1115 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/rfunc/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3643 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/rfunc/backend.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2519 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/runs.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.940612 mlflow_tmp-2.2.9/mlflow/sagemaker/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)   135097 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/sagemaker/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12986 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/sagemaker/cli.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.944612 mlflow_tmp-2.2.9/mlflow/server/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6460 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/server/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.944612 mlflow_tmp-2.2.9/mlflow/server/auth/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    24354 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/server/auth/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      575 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/server/auth/config.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3171 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/server/auth/entities.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2673 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/server/auth/logo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1267 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/server/auth/permissions.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12648 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/server/auth/sqlalchemy_store.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    68605 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/server/handlers.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      481 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/server/prometheus_exporter.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    26647 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/shap.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.944612 mlflow_tmp-2.2.9/mlflow/sklearn/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    82319 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/sklearn/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    37485 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/sklearn/utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    14351 2023-05-18 22:21:37.000000 mlflow_tmp-2.2.9/mlflow/spacy.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    44813 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/spark.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    24596 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/statsmodels.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.944612 mlflow_tmp-2.2.9/mlflow/store/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      227 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.944612 mlflow_tmp-2.2.9/mlflow/store/_unity_catalog/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/_unity_catalog/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.944612 mlflow_tmp-2.2.9/mlflow/store/_unity_catalog/registry/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/_unity_catalog/registry/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    27183 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/_unity_catalog/registry/rest_store.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5419 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/_unity_catalog/registry/utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.944612 mlflow_tmp-2.2.9/mlflow/store/artifact/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    15034 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5309 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/artifact_repository_registry.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8136 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/azure_blob_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5829 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/azure_data_lake_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5378 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/cli.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    31773 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/databricks_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6654 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/databricks_models_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10247 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/dbfs_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5234 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/ftp_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5873 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/gcs_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9684 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/hdfs_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3377 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/http_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5085 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/local_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3001 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/mlflow_artifacts_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6757 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/models_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6016 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/runs_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9442 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/s3_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5455 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/sftp_artifact_repo.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5592 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/unity_catalog_models_artifact_repo.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.944612 mlflow_tmp-2.2.9/mlflow/store/artifact/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3934 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/artifact/utils/models.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.944612 mlflow_tmp-2.2.9/mlflow/store/db/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       71 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db/base_sql_model.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      221 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db/db_types.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10592 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db/utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.944612 mlflow_tmp-2.2.9/mlflow/store/db_migrations/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1634 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/alembic.ini
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2768 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/env.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.948612 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1990 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      462 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/0c779009ac13_add_deleted_time_field_to_runs_table.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      924 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1059 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2624 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1375 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1433 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1201 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      940 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1014 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      476 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/84291f40a231_add_run_link_to_model_version.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5716 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1666 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      577 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      582 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      637 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1295 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      684 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2830 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      904 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.948612 mlflow_tmp-2.2.9/mlflow/store/entities/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       80 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/entities/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      479 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/entities/paged_list.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.948612 mlflow_tmp-2.2.9/mlflow/store/model_registry/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      605 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/model_registry/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    11022 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/model_registry/abstract_store.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1330 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/model_registry/base_rest_store.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.948612 mlflow_tmp-2.2.9/mlflow/store/model_registry/dbmodels/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/model_registry/dbmodels/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6341 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/model_registry/dbmodels/models.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    38833 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/model_registry/file_store.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    16920 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/model_registry/rest_store.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    50646 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/model_registry/sqlalchemy_store.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.948612 mlflow_tmp-2.2.9/mlflow/store/tracking/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1154 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/tracking/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    13042 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/tracking/abstract_store.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.948612 mlflow_tmp-2.2.9/mlflow/store/tracking/dbmodels/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/tracking/dbmodels/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8315 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/tracking/dbmodels/initial_models.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    15674 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/tracking/dbmodels/models.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    46363 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/tracking/file_store.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    12172 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/tracking/rest_store.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    67230 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/store/tracking/sqlalchemy_store.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.948612 mlflow_tmp-2.2.9/mlflow/tensorflow/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    57261 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tensorflow/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     8442 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tensorflow/_autolog.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.948612 mlflow_tmp-2.2.9/mlflow/tracking/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      995 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/__init__.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.948612 mlflow_tmp-2.2.9/mlflow/tracking/_model_registry/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       41 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/_model_registry/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    15534 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/_model_registry/client.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9641 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/_model_registry/fluent.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3152 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/_model_registry/registry.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     7008 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/_model_registry/utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.948612 mlflow_tmp-2.2.9/mlflow/tracking/_tracking_service/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/_tracking_service/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    23690 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/_tracking_service/client.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2335 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/_tracking_service/registry.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9517 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/_tracking_service/utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     7155 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/artifact_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)   130061 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/client.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.952612 mlflow_tmp-2.2.9/mlflow/tracking/context/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/context/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1076 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/context/abstract_context.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      520 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/context/databricks_cluster_context.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      561 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/context/databricks_command_context.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1965 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/context/databricks_job_context.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1713 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/context/databricks_notebook_context.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1952 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/context/databricks_repo_context.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1020 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/context/default_context.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      898 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/context/git_context.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3738 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/context/registry.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      443 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/context/system_environment_context.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.952612 mlflow_tmp-2.2.9/mlflow/tracking/default_experiment/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       28 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/default_experiment/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1703 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/default_experiment/abstract_context.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1718 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2300 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3173 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/default_experiment/registry.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    71082 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/fluent.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3404 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/llm_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2248 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/metric_value_conversion_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3515 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/registry.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.952612 mlflow_tmp-2.2.9/mlflow/tracking/request_header/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/request_header/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1077 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/request_header/abstract_request_header_provider.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1336 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/request_header/databricks_request_header_provider.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      486 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/request_header/default_request_header_provider.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2867 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/tracking/request_header/registry.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    96409 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/transformers.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.952612 mlflow_tmp-2.2.9/mlflow/types/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      299 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/types/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    13334 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/types/schema.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    17899 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/types/utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.956612 mlflow_tmp-2.2.9/mlflow/utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9389 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6270 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/_capture_modules.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6395 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/_spark_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     4906 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/annotations.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      400 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/arguments_utils.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.956612 mlflow_tmp-2.2.9/mlflow/utils/autologging_utils/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    27070 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/autologging_utils/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    15731 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/autologging_utils/client.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10937 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/autologging_utils/events.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    13381 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/autologging_utils/logging_and_warnings.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    47266 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/autologging_utils/safety.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3489 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/autologging_utils/versioning.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      215 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/class_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6431 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/cli_args.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    13002 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/conda.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      432 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/data_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    22596 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/databricks_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     9138 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/docstring_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      192 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/env.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      474 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/env_manager.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    21851 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/environment.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    25967 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/file_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2306 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/git_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    24166 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/gorilla.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.956612 mlflow_tmp-2.2.9/mlflow/utils/import_hooks/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    13489 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/import_hooks/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2597 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/logging_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1298 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/mime_type_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3839 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/mlflow_tags.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6208 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/model_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5873 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/name_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2412 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/nfs_on_spark.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      139 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/os.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     5799 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/process.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    19923 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/proto_json_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    18635 2023-05-20 03:04:12.000000 mlflow_tmp-2.2.9/mlflow/utils/requirements_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    16880 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/rest_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    56769 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/search_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2368 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/server_cli_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     3805 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/string_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      512 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/time_utils.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    13915 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/uri.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    16024 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/validation.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    16452 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/utils/virtualenv.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      152 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/version.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.956612 mlflow_tmp-2.2.9/mlflow/xgboost/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    34313 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/xgboost/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2908 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/mlflow/xgboost/_autolog.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.956612 mlflow_tmp-2.2.9/mlflow_tmp.egg-info/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    10474 2023-05-21 00:15:09.000000 mlflow_tmp-2.2.9/mlflow_tmp.egg-info/PKG-INFO
--rw-rw-r--   0 ckl       (1000) ckl       (1000)    13629 2023-05-21 00:15:09.000000 mlflow_tmp-2.2.9/mlflow_tmp.egg-info/SOURCES.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-05-21 00:15:09.000000 mlflow_tmp-2.2.9/mlflow_tmp.egg-info/dependency_links.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       92 2023-05-21 00:15:09.000000 mlflow_tmp-2.2.9/mlflow_tmp.egg-info/entry_points.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-05-19 04:30:57.000000 mlflow_tmp-2.2.9/mlflow_tmp.egg-info/not-zip-safe
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      865 2023-05-21 00:15:09.000000 mlflow_tmp-2.2.9/mlflow_tmp.egg-info/requires.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       22 2023-05-21 00:15:09.000000 mlflow_tmp-2.2.9/mlflow_tmp.egg-info/top_level.txt
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.956612 mlflow_tmp-2.2.9/pylint_plugins/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      521 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/pylint_plugins/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     2006 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/pylint_plugins/errors.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      856 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/pylint_plugins/print_function.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.956612 mlflow_tmp-2.2.9/pylint_plugins/pytest_raises_checker/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     1546 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/pylint_plugins/pytest_raises_checker/__init__.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      571 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/pylint_plugins/set_checker.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      878 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/pylint_plugins/string_checker.py
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      692 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/pylint_plugins/unittest_assert_raises.py
-drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-21 00:15:09.956612 mlflow_tmp-2.2.9/requirements/
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      609 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/requirements/core-requirements.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)      481 2023-05-18 21:19:46.000000 mlflow_tmp-2.2.9/requirements/skinny-requirements.txt
--rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-05-21 00:15:09.956612 mlflow_tmp-2.2.9/setup.cfg
--rw-rw-r--   0 ckl       (1000) ckl       (1000)     6756 2023-05-21 00:08:42.000000 mlflow_tmp-2.2.9/setup.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.069904 mlflow_tmp-2.3.3.dev0/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11382 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/LICENSE.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      562 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/MANIFEST.in
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10479 2023-05-19 04:30:58.069904 mlflow_tmp-2.3.3.dev0/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9767 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/README.rst
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      949 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/README_SKINNY.rst
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.049904 mlflow_tmp-2.3.3.dev0/mlflow/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6215 2023-05-18 22:57:23.000000 mlflow_tmp-2.3.3.dev0/mlflow/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       39 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/__main__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3668 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/_doctor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9428 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/_spark_autologging.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.049904 mlflow_tmp-2.3.3.dev0/mlflow/artifacts/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6485 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/artifacts/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.049904 mlflow_tmp-2.3.3.dev0/mlflow/azure/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/azure/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11647 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/azure/client.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    15140 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/catboost.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    23356 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/cli.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      407 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/client.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      881 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/db.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.049904 mlflow_tmp-2.3.3.dev0/mlflow/deployments/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3797 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/deployments/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    15572 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/deployments/base.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    15078 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/deployments/cli.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3825 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/deployments/interface.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5512 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/deployments/plugin_manager.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      556 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/deployments/utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    28178 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/diviner.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.049904 mlflow_tmp-2.3.3.dev0/mlflow/entities/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      948 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1414 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/_mlflow_object.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3510 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/experiment.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      887 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/experiment_tag.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1215 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/file_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1242 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/lifecycle_stage.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1418 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/metric.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.049904 mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      529 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      286 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/_model_registry_entity.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6435 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/model_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      831 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/model_version_stages.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1533 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/model_version_status.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      933 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/model_version_tag.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4933 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/registered_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1053 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/registered_model_alias.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      948 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/registered_model_tag.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1133 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/param.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1438 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/run.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3032 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/run_data.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6182 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/run_info.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1550 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/run_status.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      890 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/run_tag.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1212 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/source_type.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1826 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/entities/view_type.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10192 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/environment_variables.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4881 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/exceptions.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5080 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/experiments.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.049904 mlflow_tmp-2.3.3.dev0/mlflow/fastai/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    25354 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/fastai/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5757 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/fastai/callback.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.049904 mlflow_tmp-2.3.3.dev0/mlflow/gluon/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    19063 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/gluon/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2020 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/gluon/_autolog.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    14185 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/h2o.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8695 2023-05-19 03:35:20.000000 mlflow_tmp-2.3.3.dev0/mlflow/johnsnowlabs.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      311 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/keras.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.049904 mlflow_tmp-2.3.3.dev0/mlflow/langchain/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    20905 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/langchain/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4846 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/langchain/api_request_parallel_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    35902 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/lightgbm.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      180 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/llm.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5575 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/ml_package_versions.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    13885 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/mleap.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.049904 mlflow_tmp-2.3.3.dev0/mlflow/models/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3627 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9803 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/cli.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.049904 mlflow_tmp-2.3.3.dev0/mlflow/models/container/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9387 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/container/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.049904 mlflow_tmp-2.3.3.dev0/mlflow/models/container/scoring_server/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/container/scoring_server/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      712 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/container/scoring_server/nginx.conf
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      131 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/container/scoring_server/wsgi.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9853 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/docker_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.053904 mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      491 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3105 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/_shap_patch.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6769 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/artifacts.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    59488 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/base.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    50976 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/default_evaluator.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2036 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/evaluator_registry.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6223 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/lift_curve.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10946 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/validation.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3420 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/flavor_backend.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2354 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/flavor_backend_registry.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    24148 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8634 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/signature.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    38161 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11707 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/models/wheeled_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    21826 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/onnx.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.053904 mlflow_tmp-2.3.3.dev0/mlflow/openai/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    23265 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/openai/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12309 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/openai/api_request_parallel_processor.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2936 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/openai/retry.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2088 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/openai/utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.053904 mlflow_tmp-2.3.3.dev0/mlflow/paddle/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    23859 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/paddle/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4792 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/paddle/_paddle_autolog.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    17616 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pmdarima.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.053904 mlflow_tmp-2.3.3.dev0/mlflow/projects/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    17396 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/projects/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11532 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/projects/_project_spec.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.053904 mlflow_tmp-2.3.3.dev0/mlflow/projects/backend/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      271 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/projects/backend/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2210 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/projects/backend/abstract_backend.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1079 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/projects/backend/loader.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    17240 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/projects/backend/local.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    20270 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/projects/databricks.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6394 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/projects/docker.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       94 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/projects/env_type.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6379 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/projects/kubernetes.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3574 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/projects/submitted_run.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    13432 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/projects/utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    14024 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/prophet.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.053904 mlflow_tmp-2.3.3.dev0/mlflow/protos/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/protos/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    17261 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/protos/databricks_artifacts_pb2.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    14095 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/protos/databricks_pb2.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    39471 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/protos/databricks_uc_registry_messages_pb2.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12471 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/protos/databricks_uc_registry_service_pb2.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    16146 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/protos/facet_feature_statistics_pb2.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8552 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/protos/mlflow_artifacts_pb2.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    54475 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/protos/model_registry_pb2.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.053904 mlflow_tmp-2.3.3.dev0/mlflow/protos/scalapb/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/protos/scalapb/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3307 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/protos/scalapb/scalapb_pb2.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    48593 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/protos/service_pb2.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.053904 mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    81412 2023-05-18 21:22:32.000000 mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    16640 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/backend.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      901 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/mlserver.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    15392 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/model.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.053904 mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/scoring_server/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    13910 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/scoring_server/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4222 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/scoring_server/client.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      175 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/scoring_server/wsgi.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2124 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/spark_model_cache.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1001 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/stdin_server.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)  7197781 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pypi_package_index.json
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.053904 mlflow_tmp-2.3.3.dev0/mlflow/pyspark/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       50 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pyspark/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.053904 mlflow_tmp-2.3.3.dev0/mlflow/pyspark/ml/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    53458 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pyspark/ml/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2908 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pyspark/ml/_autolog.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1886 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pyspark/ml/log_model_allowlist.txt
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.053904 mlflow_tmp-2.3.3.dev0/mlflow/pytorch/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    45379 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pytorch/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    17629 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pytorch/_lightning_autolog.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2654 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pytorch/_pytorch_autolog.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2090 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/pytorch/pickle_module.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/recipes/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1330 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6092 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/artifacts.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/recipes/cards/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10229 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/cards/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4780 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/cards/histogram_generator.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12548 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/cards/pandas_renderer.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/recipes/cards/templates/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/cards/templates/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3488 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/cards/templates/base.html
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/recipes/classification/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/classification/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/recipes/classification/v1/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      122 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/classification/v1/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    20462 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/classification/v1/recipe.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2917 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/cli.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    18431 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/dag_help_strings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    17933 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/recipe.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/recipes/regression/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/regression/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/recipes/regression/v1/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      114 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/regression/v1/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    22495 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/regression/v1/recipe.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/recipes/resources/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12211 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/resources/recipe_dag_template.html
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    14988 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/step.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/automl/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/automl/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6269 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/automl/flaml.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    20717 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/evaluate.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/ingest/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11137 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/ingest/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    26446 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/ingest/datasets.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12132 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/predict.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     7680 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/register.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    19541 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/split.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    59789 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/train.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10602 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/transform.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/recipes/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6355 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    28468 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/utils/execution.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8990 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/utils/metrics.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     7392 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/utils/step.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12375 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/utils/tracking.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1748 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/recipes/utils/wrapped_recipe_model.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/rfunc/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1115 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/rfunc/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3643 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/rfunc/backend.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2519 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/runs.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/sagemaker/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)   135097 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/sagemaker/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12986 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/sagemaker/cli.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/server/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6460 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/server/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/server/auth/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    24354 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/server/auth/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      575 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/server/auth/config.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3171 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/server/auth/entities.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2673 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/server/auth/logo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1267 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/server/auth/permissions.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12648 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/server/auth/sqlalchemy_store.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    68605 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/server/handlers.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      481 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/server/prometheus_exporter.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    26647 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/shap.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/sklearn/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    82319 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/sklearn/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    37485 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/sklearn/utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    14351 2023-05-18 22:21:37.000000 mlflow_tmp-2.3.3.dev0/mlflow/spacy.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    44813 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/spark.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    24596 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/statsmodels.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/store/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      227 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/store/_unity_catalog/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/_unity_catalog/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.057904 mlflow_tmp-2.3.3.dev0/mlflow/store/_unity_catalog/registry/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/_unity_catalog/registry/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    27183 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/_unity_catalog/registry/rest_store.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5419 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/_unity_catalog/registry/utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.061904 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    15034 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5309 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/artifact_repository_registry.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8136 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/azure_blob_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5829 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/azure_data_lake_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5378 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/cli.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    31773 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/databricks_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6654 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/databricks_models_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10247 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/dbfs_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5234 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/ftp_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5873 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/gcs_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9684 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/hdfs_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3377 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/http_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5085 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/local_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3001 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/mlflow_artifacts_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6757 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/models_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6016 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/runs_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9442 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/s3_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5455 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/sftp_artifact_repo.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5592 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/unity_catalog_models_artifact_repo.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.061904 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3934 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/utils/models.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.061904 mlflow_tmp-2.3.3.dev0/mlflow/store/db/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       71 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db/base_sql_model.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      221 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db/db_types.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10592 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db/utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.061904 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1634 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/alembic.ini
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2768 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/env.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.061904 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1990 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      462 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/0c779009ac13_add_deleted_time_field_to_runs_table.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      924 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1059 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2624 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1375 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1433 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1201 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      940 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1014 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      476 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/84291f40a231_add_run_link_to_model_version.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5716 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1666 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      577 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      582 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      637 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1295 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      684 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2830 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      904 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.061904 mlflow_tmp-2.3.3.dev0/mlflow/store/entities/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       80 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/entities/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      479 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/entities/paged_list.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.061904 mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      605 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    11022 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/abstract_store.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1330 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/base_rest_store.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.061904 mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/dbmodels/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/dbmodels/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6341 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/dbmodels/models.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    38833 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/file_store.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    16920 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/rest_store.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    50646 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/sqlalchemy_store.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.061904 mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1154 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    13042 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/abstract_store.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.061904 mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/dbmodels/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/dbmodels/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8315 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/dbmodels/initial_models.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    15674 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/dbmodels/models.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    46363 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/file_store.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    12172 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/rest_store.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    67230 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/sqlalchemy_store.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.061904 mlflow_tmp-2.3.3.dev0/mlflow/tensorflow/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    57261 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tensorflow/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     8442 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tensorflow/_autolog.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.065904 mlflow_tmp-2.3.3.dev0/mlflow/tracking/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      995 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/__init__.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.065904 mlflow_tmp-2.3.3.dev0/mlflow/tracking/_model_registry/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       41 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/_model_registry/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    15534 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/_model_registry/client.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9641 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/_model_registry/fluent.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3152 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/_model_registry/registry.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     7008 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/_model_registry/utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.065904 mlflow_tmp-2.3.3.dev0/mlflow/tracking/_tracking_service/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/_tracking_service/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    23690 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/_tracking_service/client.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2335 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/_tracking_service/registry.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9517 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/_tracking_service/utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     7155 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/artifact_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)   130061 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/client.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.065904 mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1076 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/abstract_context.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      520 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/databricks_cluster_context.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      561 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/databricks_command_context.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1965 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/databricks_job_context.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1713 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/databricks_notebook_context.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1952 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/databricks_repo_context.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1020 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/default_context.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      898 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/git_context.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3738 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/registry.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      443 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/system_environment_context.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.065904 mlflow_tmp-2.3.3.dev0/mlflow/tracking/default_experiment/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       28 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/default_experiment/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1703 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/default_experiment/abstract_context.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1718 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2300 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3173 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/default_experiment/registry.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    71082 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/fluent.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3404 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/llm_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2248 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/metric_value_conversion_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3515 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/registry.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.065904 mlflow_tmp-2.3.3.dev0/mlflow/tracking/request_header/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        0 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/request_header/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1077 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/request_header/abstract_request_header_provider.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1336 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/request_header/databricks_request_header_provider.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      486 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/request_header/default_request_header_provider.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2867 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/tracking/request_header/registry.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    96409 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/transformers.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.065904 mlflow_tmp-2.3.3.dev0/mlflow/types/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      299 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/types/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    13334 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/types/schema.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    17899 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/types/utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.069904 mlflow_tmp-2.3.3.dev0/mlflow/utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9389 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6270 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/_capture_modules.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6395 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/_spark_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     4906 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/annotations.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      400 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/arguments_utils.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.069904 mlflow_tmp-2.3.3.dev0/mlflow/utils/autologging_utils/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    27070 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/autologging_utils/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    15731 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/autologging_utils/client.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10937 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/autologging_utils/events.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    13381 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/autologging_utils/logging_and_warnings.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    47266 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/autologging_utils/safety.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3489 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/autologging_utils/versioning.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      215 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/class_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6431 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/cli_args.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    13002 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/conda.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      432 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/data_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    22596 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/databricks_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     9138 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/docstring_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      192 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/env.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      474 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/env_manager.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    21851 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/environment.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    25967 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/file_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2306 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/git_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    24166 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/gorilla.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.069904 mlflow_tmp-2.3.3.dev0/mlflow/utils/import_hooks/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    13489 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/import_hooks/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2597 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/logging_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1298 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/mime_type_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3839 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/mlflow_tags.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6208 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/model_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5873 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/name_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2412 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/nfs_on_spark.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      139 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/os.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     5799 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/process.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    19923 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/proto_json_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    18679 2023-05-19 03:32:37.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/requirements_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    16880 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/rest_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    56769 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/search_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2368 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/server_cli_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     3805 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/string_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      512 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/time_utils.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    13915 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/uri.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    16024 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/validation.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    16452 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/utils/virtualenv.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      152 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/version.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.069904 mlflow_tmp-2.3.3.dev0/mlflow/xgboost/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    34313 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/xgboost/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2908 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/mlflow/xgboost/_autolog.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.069904 mlflow_tmp-2.3.3.dev0/mlflow_tmp.egg-info/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    10479 2023-05-19 04:30:57.000000 mlflow_tmp-2.3.3.dev0/mlflow_tmp.egg-info/PKG-INFO
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)    13605 2023-05-19 04:30:58.000000 mlflow_tmp-2.3.3.dev0/mlflow_tmp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-05-19 04:30:57.000000 mlflow_tmp-2.3.3.dev0/mlflow_tmp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       92 2023-05-19 04:30:57.000000 mlflow_tmp-2.3.3.dev0/mlflow_tmp.egg-info/entry_points.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)        1 2023-05-19 04:30:57.000000 mlflow_tmp-2.3.3.dev0/mlflow_tmp.egg-info/not-zip-safe
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      865 2023-05-19 04:30:57.000000 mlflow_tmp-2.3.3.dev0/mlflow_tmp.egg-info/requires.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       22 2023-05-19 04:30:57.000000 mlflow_tmp-2.3.3.dev0/mlflow_tmp.egg-info/top_level.txt
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.069904 mlflow_tmp-2.3.3.dev0/pylint_plugins/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      521 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/pylint_plugins/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     2006 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/pylint_plugins/errors.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      856 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/pylint_plugins/print_function.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.069904 mlflow_tmp-2.3.3.dev0/pylint_plugins/pytest_raises_checker/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     1546 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/pylint_plugins/pytest_raises_checker/__init__.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      571 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/pylint_plugins/set_checker.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      878 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/pylint_plugins/string_checker.py
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      692 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/pylint_plugins/unittest_assert_raises.py
+drwxrwxr-x   0 ckl       (1000) ckl       (1000)        0 2023-05-19 04:30:58.069904 mlflow_tmp-2.3.3.dev0/requirements/
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      609 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/requirements/core-requirements.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)      481 2023-05-18 21:19:46.000000 mlflow_tmp-2.3.3.dev0/requirements/skinny-requirements.txt
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)       38 2023-05-19 04:30:58.069904 mlflow_tmp-2.3.3.dev0/setup.cfg
+-rw-rw-r--   0 ckl       (1000) ckl       (1000)     6850 2023-05-19 04:30:56.000000 mlflow_tmp-2.3.3.dev0/setup.py
```

### Comparing `mlflow_tmp-2.2.9/LICENSE.txt` & `mlflow_tmp-2.3.3.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/MANIFEST.in` & `mlflow_tmp-2.3.3.dev0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/PKG-INFO` & `mlflow_tmp-2.3.3.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow_tmp
-Version: 2.2.9
+Version: 2.3.3.dev0
 Summary: MLflow: A Platform for ML Development and Productionization
 Home-page: https://mlflow.org/
 Author: Databricks
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mlflow/mlflow/issues
 Project-URL: Documentation, https://mlflow.org/docs/latest/index.html
 Project-URL: Source Code, https://github.com/mlflow/mlflow
```

### Comparing `mlflow_tmp-2.2.9/README.rst` & `mlflow_tmp-2.3.3.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/README_SKINNY.rst` & `mlflow_tmp-2.3.3.dev0/README_SKINNY.rst`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/_doctor.py` & `mlflow_tmp-2.3.3.dev0/mlflow/_doctor.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/_spark_autologging.py` & `mlflow_tmp-2.3.3.dev0/mlflow/_spark_autologging.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/artifacts/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/azure/client.py` & `mlflow_tmp-2.3.3.dev0/mlflow/azure/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/catboost.py` & `mlflow_tmp-2.3.3.dev0/mlflow/catboost.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/cli.py` & `mlflow_tmp-2.3.3.dev0/mlflow/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/db.py` & `mlflow_tmp-2.3.3.dev0/mlflow/db.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/deployments/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/deployments/base.py` & `mlflow_tmp-2.3.3.dev0/mlflow/deployments/base.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/deployments/cli.py` & `mlflow_tmp-2.3.3.dev0/mlflow/deployments/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/deployments/interface.py` & `mlflow_tmp-2.3.3.dev0/mlflow/deployments/interface.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/deployments/plugin_manager.py` & `mlflow_tmp-2.3.3.dev0/mlflow/deployments/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/deployments/utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/deployments/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/diviner.py` & `mlflow_tmp-2.3.3.dev0/mlflow/diviner.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/_mlflow_object.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/_mlflow_object.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/experiment.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/experiment.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/experiment_tag.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/experiment_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/file_info.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/file_info.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/lifecycle_stage.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/lifecycle_stage.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/metric.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/metric.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/model_registry/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/model_registry/model_version.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/model_version.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/model_registry/model_version_stages.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/model_version_stages.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/model_registry/model_version_status.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/model_version_status.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/model_registry/model_version_tag.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/model_version_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/model_registry/registered_model.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/registered_model.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/model_registry/registered_model_alias.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/registered_model_alias.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/model_registry/registered_model_tag.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/model_registry/registered_model_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/param.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/param.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/run.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/run.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/run_data.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/run_data.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/run_info.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/run_info.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/run_status.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/run_status.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/run_tag.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/run_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/source_type.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/source_type.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/entities/view_type.py` & `mlflow_tmp-2.3.3.dev0/mlflow/entities/view_type.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/environment_variables.py` & `mlflow_tmp-2.3.3.dev0/mlflow/environment_variables.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/exceptions.py` & `mlflow_tmp-2.3.3.dev0/mlflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/experiments.py` & `mlflow_tmp-2.3.3.dev0/mlflow/experiments.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/fastai/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/fastai/callback.py` & `mlflow_tmp-2.3.3.dev0/mlflow/fastai/callback.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/gluon/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/gluon/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/gluon/_autolog.py` & `mlflow_tmp-2.3.3.dev0/mlflow/gluon/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/h2o.py` & `mlflow_tmp-2.3.3.dev0/mlflow/h2o.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/johnsnowlabs.py` & `mlflow_tmp-2.3.3.dev0/mlflow/johnsnowlabs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,64 @@
-import json
 import sys
-from pathlib import Path
-import mlflow.spark
 
 from johnsnowlabs import nlp
-from johnsnowlabs.auto_install.jsl_home import get_install_suite_from_jsl_home
-from johnsnowlabs.py_models.jsl_secrets import JslSecrets
 from pyspark.ml import PipelineModel
 
 """
 The ``mlflow.spacy`` module provides an API for logging and loading spaCy models.
 This module exports spacy models with the following flavors:
 
 spaCy (native) format
     This is the main flavor that can be loaded back into spaCy.
 :py:mod:`mlflow.pyfunc`
     Produced for use by generic pyfunc-based deployment tools and batch inference, this
     flavor is created only if spaCy's model pipeline has at least one
     `TextCategorizer <https://spacy.io/api/textcategorizer>`_.
 """
+import os
+from mlflow.utils.model_utils import (
+    _get_flavor_configuration,
+    _add_code_from_conf_to_system_path,
+)
+
 import logging
 import os
+import pickle
+
+import mlflow
+import numpy as np
+import pandas as pd
+import yaml
+from mlflow import pyfunc
+from mlflow.exceptions import MlflowException
+from mlflow.models import Model
+from mlflow.models.model import MLMODEL_FILE_NAME
+from mlflow.models.utils import _save_example
+from mlflow.protos.databricks_pb2 import INTERNAL_ERROR, INVALID_PARAMETER_VALUE
+from mlflow.tracking._model_registry import DEFAULT_AWAIT_MAX_SLEEP_SECONDS
+from mlflow.tracking.artifact_utils import _download_artifact_from_uri
+from mlflow.utils.environment import (
+    _CONDA_ENV_FILE_NAME,
+    _CONSTRAINTS_FILE_NAME,
+    _PYTHON_ENV_FILE_NAME,
+    _REQUIREMENTS_FILE_NAME,
+    _mlflow_conda_env,
+    _process_conda_env,
+    _process_pip_requirements,
+    _PythonEnv,
+    _validate_env_arguments,
+)
+from mlflow.utils.file_utils import write_to
 from mlflow.utils.model_utils import (
     _add_code_from_conf_to_system_path,
     _get_flavor_configuration,
+    _validate_and_copy_code_paths,
+    _validate_and_prepare_target_save_path,
 )
+from mlflow.utils.requirements_utils import _get_pinned_requirement
 
 _logger = logging.getLogger(__name__)
 
 import yaml
 from mlflow.tracking.artifact_utils import _download_artifact_from_uri
 import mlflow
 from mlflow import pyfunc
@@ -47,84 +77,74 @@
 from mlflow.utils.file_utils import write_to
 from mlflow.utils.model_utils import (
     _validate_and_copy_code_paths,
 )
 from mlflow.utils.requirements_utils import _get_pinned_requirement
 
 
+# TODO HARDCODE I NTERNAL!!?
 def get_default_pip_requirements():
     """
     :return: A list of default pip requirements for MLflow Models produced by this flavor.
              Calls to :func:`save_model()` and :func:`log_model()` produce a pip environment
              that, at minimum, contains these requirements.
     """
     return [
         _get_pinned_requirement("johnsnowlabs"),
         "https://pypi.johnsnowlabs.com/4.4.2-f771e88dcf8e1535585c5531824a595e92c0305c/spark-nlp-jsl/spark_nlp_jsl-4.4.2-py3-none-any.whl",
-        'pyspark==3.2.1',
 
-    ]
+            ]
 
 
 FLAVOR_NAME = "johnsnowlabs"
 MLMODEL_FILE_NAME = "MLmodel"
 _MLFLOW_VERSION_KEY = "mlflow_version"
 
 
+
 class MyModel(mlflow.pyfunc.PythonModel):
-    def __init__(self, spell=None, pipe_path=None, jars_paths=None, license_path=None):
+    def __init__(self, spell=None, pipe_path=None):
         os.environ['PYSPARK_PYTHON'] = sys.executable
         os.environ['PYSPARK_DRIVER_PYTHON'] = sys.executable
 
-        # TODO check if jsl-hoome exists, if not check if we find jar in Artifacts
-        # TODO credentials?!
-        if jars_paths:
-            # load jar from disk
-            os.environ.update({k: str(v) for k, v in json.load(open(license_path)).items() if v is not None})
-            os.environ['JSL_NLP_LICENSE'] = json.load(open(license_path))['HC_LICENSE']
-            self.spark = nlp.start(nlp=False, spark_nlp=False, jar_paths=jars_paths, json_license_path=license_path)
-        else:
-            # load jar from web
-            if pipe_path:
-                if os.path.exists(os.path.join(pipe_path,'jars.jsl')):
-                    jars_paths, license_path = fetch_deps_from_path(pipe_path)
-                    os.environ.update({k: str(v) for k, v in json.load(open(license_path)).items() if v is not None})
-                    os.environ['JSL_NLP_LICENSE'] = json.load(open(license_path))['HC_LICENSE']
-
-                    self.spark = nlp.start(nlp=False, spark_nlp=False, jar_paths=jars_paths, json_license_path=license_path)
-            else:
-
-                self.spark = nlp.start()
+        self.spark = nlp.start()
         if pipe_path:
             print(f'loading from disk {pipe_path}')
             self.pipe = nlp.to_nlu_pipe(PipelineModel.load(pipe_path))
             print('loading from disk done')
+
+
         else:
             self.pipe = nlp.load(spell)
         self.pipe.predict('Init NLU')
 
-    def predict(self, model_input, output_level=None):
-        return self.pipe.predict(model_input, output_level=output_level)
+    def predict(self, model_input, groupy=None):
+        # return 1
+        return self.pipe.predict(model_input) #,groupy=groupy)
+
+
+
+
+
 
 
 def log_model(
         johnsnowlabs_model,
         artifact_path,
         conda_env=None,
         code_paths=None,
         registered_model_name=None,
         signature: ModelSignature = None,
         input_example: ModelInputExample = None,
         pip_requirements=None,
         extra_pip_requirements=None,
         metadata=None,
         **kwargs,
-):  # TOdo make sure log shows up
+):
     # todo make sure pass correct model type , its expected as kwarg in python_model
-    print("LOG FROM log_mode")
     return Model.log(
         artifact_path=artifact_path,
         flavor=mlflow.johnsnowlabs,
         registered_model_name=registered_model_name,
         python_model=johnsnowlabs_model,
         johnsnowlabs_model=johnsnowlabs_model,
         conda_env=conda_env,
@@ -134,38 +154,31 @@
         pip_requirements=pip_requirements,
         extra_pip_requirements=extra_pip_requirements,
         metadata=metadata,
         **kwargs,
     )
 
 
-def _load_pyfunc(path):
-    # todo load jars ?
-    print("LOAD FROM _load_pyfunc")
-    return MyModel(pipe_path=path)
 
 
-def fetch_deps_from_path(local_model_path):
-    local_model_path = os.path.join(local_model_path,  'jars.jsl', )
-    jar_paths = [os.path.join(local_model_path, file) for file in os.listdir(local_model_path) if '.jar' in file]
-    license_path = [os.path.join(local_model_path, file) for file in os.listdir(local_model_path) if '.json' in file]
-    license_path = license_path[0] if license_path else None
-    return jar_paths, license_path
+def _load_pyfunc(path): return MyModel(pipe_path=path)
+
 
 def load_model(model_uri):
-    print("LOAD FROM load_model")
     local_model_path = _download_artifact_from_uri(artifact_uri=model_uri, output_path=None)
-    jar_paths, license_path = fetch_deps_from_path(os.path.join(local_model_path,"model.jsl",))
-    print("Found jars ", jar_paths)
     flavor_conf = _get_flavor_configuration(model_path=local_model_path, flavor_name=FLAVOR_NAME)
     _add_code_from_conf_to_system_path(local_model_path, flavor_conf)
     # Flavor configurations for models saved in MLflow version <= 0.8.0 may not contain a
     # `data` key; in this case, we assume the model artifact path to be `model.spacy`
     spacy_model_file_path = os.path.join(local_model_path, flavor_conf.get("data", "model.jsl"))
-    return MyModel(pipe_path=spacy_model_file_path, jars_paths=jar_paths, license_path=license_path)
+    return MyModel(pipe_path=spacy_model_file_path)
+
+
+def _save_model(sk_model, output_path, serialization_format):
+    print('????SAVING!!')
 
 
 def save_model(
         johnsnowlabs_model=None,
         path=None,
         conda_env=None,
         code_paths=None,
@@ -181,37 +194,19 @@
         python_model=None,  # RM
         artifacts=None,  # RM
 ):
     print('Saving')
 
     model_data_subpath = "model.jsl"
     model_data_path = os.path.join(path, model_data_subpath)
-    deps_data_path = os.path.join(model_data_path, "jars.jsl")
-    Path(model_data_path).mkdir(parents=True, exist_ok=True)
-
-    if isinstance(python_model, MyModel):
+    os.makedirs(model_data_path)
+    code_dir_subpath = _validate_and_copy_code_paths(code_paths, path)
+    if isinstance(python_model,MyModel ):
         johnsnowlabs_model = python_model.pipe
     johnsnowlabs_model.vanilla_transformer_pipe.write().overwrite().save(model_data_path)
-    Path(deps_data_path).mkdir(parents=True, exist_ok=True)
-
-    from johnsnowlabs import nlp
-    nlp.start()  # ?
-    suite = get_install_suite_from_jsl_home(False)
-    import shutil
-    if suite.hc.get_java_path():
-        shutil.copyfile(suite.hc.get_java_path(), os.path.join(deps_data_path, 'hc_jar.jar'))
-    if suite.nlp.get_java_path():
-        shutil.copyfile(suite.nlp.get_java_path(), os.path.join(deps_data_path, 'os_jar.jar'))
-
-    secrets = JslSecrets.build_or_try_find_secrets()
-    if secrets.HC_LICENSE:
-        with open(os.path.join(deps_data_path, 'license.json'), 'w') as f:
-            f.write(secrets.json())
-
-    code_dir_subpath = _validate_and_copy_code_paths(code_paths, path)
 
     if mlflow_model is None:
         mlflow_model = Model()
     if signature is not None:
         mlflow_model.signature = signature
     if input_example is not None:
         _save_example(mlflow_model, input_example, path)
@@ -260,7 +255,11 @@
         write_to(os.path.join(path, _CONSTRAINTS_FILE_NAME), "\n".join(pip_constraints))
 
     # Save `requirements.txt`
     write_to(os.path.join(path, _REQUIREMENTS_FILE_NAME), "\n".join(pip_requirements))
 
     _PythonEnv.current().to_yaml(os.path.join(path, _PYTHON_ENV_FILE_NAME))
     mlflow_model.save(os.path.join(path, MLMODEL_FILE_NAME))
+
+
+
+url="https://pypi.johnsnowlabs.com/4.4.2-f771e88dcf8e1535585c5531824a595e92c0305c/spark-nlp-jsl/spark_nlp_jsl-4.4.2-py3-none-any.whl",
```

### Comparing `mlflow_tmp-2.2.9/mlflow/johnsnowlabs2.py` & `mlflow_tmp-2.3.3.dev0/mlflow/xgboost/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,175 +1,127 @@
 """
-The ``mlflow.spark`` module provides an API for logging and loading Spark MLlib models. This module
-exports Spark MLlib models with the following flavors:
+The ``mlflow.xgboost`` module provides an API for logging and loading XGBoost models.
+This module exports XGBoost models with the following flavors:
 
-Spark MLlib (native) format
-    Allows models to be loaded as Spark Transformers for scoring in a Spark session.
-    Models with this flavor can be loaded as PySpark PipelineModel objects in Python.
-    This is the main flavor and is always produced.
+XGBoost (native) format
+    This is the main flavor that can be loaded back into XGBoost.
 :py:mod:`mlflow.pyfunc`
-    Supports deployment outside of Spark by instantiating a SparkContext and reading
-    input data as a Spark DataFrame prior to scoring. Also supports deployment in Spark
-    as a Spark UDF. Models with this flavor can be loaded as Python functions
-    for performing inference. This flavor is always produced.
-:py:mod:`mlflow.mleap`
-    Enables high-performance deployment outside of Spark by leveraging MLeap's
-    custom dataframe and pipeline representations. Models with this flavor *cannot* be loaded
-    back as Python objects. Rather, they must be deserialized in Java using the
-    ``mlflow/java`` package. This flavor is produced only if you specify
-    MLeap-compatible arguments.
+    Produced for use by generic pyfunc-based deployment tools and batch inference.
+
+.. _xgboost.Booster:
+    https://xgboost.readthedocs.io/en/latest/python/python_api.html#xgboost.Booster
+.. _xgboost.Booster.save_model:
+    https://xgboost.readthedocs.io/en/latest/python/python_api.html#xgboost.Booster.save_model
+.. _xgboost.train:
+    https://xgboost.readthedocs.io/en/latest/python/python_api.html#xgboost.train
+.. _scikit-learn API:
+    https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn
 """
-import json
-import logging
 import os
-import posixpath
 import shutil
-import sys
-from pathlib import Path
-
+import json
 import yaml
-from johnsnowlabs import nlp
-from johnsnowlabs.auto_install.jsl_home import get_install_suite_from_jsl_home
-from johnsnowlabs.py_models.jsl_secrets import JslSecrets
+import tempfile
+import logging
+from copy import deepcopy
 
 import mlflow
-from mlflow import pyfunc, mleap
-from mlflow.environment_variables import MLFLOW_DFS_TMP
-from mlflow.exceptions import MlflowException
-from mlflow.models import Model
+from mlflow import pyfunc
+from mlflow.models import Model, ModelInputExample, infer_signature
 from mlflow.models.model import MLMODEL_FILE_NAME
 from mlflow.models.signature import ModelSignature
-from mlflow.models.utils import ModelInputExample, _save_example
-from mlflow.spark import _mlflowdbfs_path, _HadoopFileSystem, _should_use_mlflowdbfs, _validate_model, _maybe_save_model
-from mlflow.store.artifact.databricks_artifact_repo import DatabricksArtifactRepository
-from mlflow.tracking._model_registry import DEFAULT_AWAIT_MAX_SLEEP_SECONDS
-from mlflow.tracking.artifact_utils import (
-    _download_artifact_from_uri,
-    _get_root_uri_and_artifact_path,
-)
-from mlflow.utils import databricks_utils
-from mlflow.utils.autologging_utils import autologging_integration, safe_patch
-from mlflow.utils.docstring_utils import format_docstring, LOG_MODEL_PARAM_DOCS
+from mlflow.models.utils import _save_example
+from mlflow.tracking.artifact_utils import _download_artifact_from_uri
+from mlflow.utils import _get_fully_qualified_class_name
 from mlflow.utils.environment import (
     _mlflow_conda_env,
     _validate_env_arguments,
     _process_pip_requirements,
     _process_conda_env,
     _CONDA_ENV_FILE_NAME,
     _REQUIREMENTS_FILE_NAME,
     _CONSTRAINTS_FILE_NAME,
     _PYTHON_ENV_FILE_NAME,
     _PythonEnv,
 )
-from mlflow.utils.file_utils import TempDir, write_to, shutil_copytree_without_file_permissions
+from mlflow.utils.class_utils import _get_class_from_string
+from mlflow.utils.requirements_utils import _get_pinned_requirement
+from mlflow.utils.file_utils import write_to
 from mlflow.utils.model_utils import (
-    _get_flavor_configuration_from_uri,
+    _get_flavor_configuration,
     _validate_and_copy_code_paths,
     _add_code_from_conf_to_system_path,
+    _validate_and_prepare_target_save_path,
 )
-from mlflow.utils.requirements_utils import _get_pinned_requirement
-from mlflow.utils.uri import (
-    is_local_uri,
-    append_to_uri_path,
-    dbfs_hdfs_uri_to_fuse_path,
-    is_valid_dbfs_uri,
-    get_databricks_profile_uri_from_artifact_uri,
-    generate_tmp_dfs_path,
+from mlflow.utils.docstring_utils import format_docstring, LOG_MODEL_PARAM_DOCS
+from mlflow.utils.arguments_utils import _get_arg_names
+from mlflow.utils.autologging_utils import (
+    autologging_integration,
+    safe_patch,
+    picklable_exception_safe_function,
+    get_mlflow_run_params_for_fn_args,
+    INPUT_EXAMPLE_SAMPLE_ROWS,
+    resolve_input_example_and_signature,
+    InputExampleInfo,
+    ENSURE_AUTOLOGGING_ENABLED_TEXT,
+    batch_metrics_logger,
+    MlflowAutologgingQueueingClient,
+    get_autologging_config,
 )
 
-FLAVOR_NAME = "johnsnowlabs2"
+from mlflow.tracking._model_registry import DEFAULT_AWAIT_MAX_SLEEP_SECONDS
+from mlflow.sklearn import _SklearnTrainingSession
 
-_JOHNSNOWLABS_MODEL_PATH_SUB = "jsl-model"
-_MLFLOWDBFS_SCHEME = "mlflowdbfs"
+FLAVOR_NAME = "xgboost"
 
 _logger = logging.getLogger(__name__)
 
 
 def get_default_pip_requirements():
     """
     :return: A list of default pip requirements for MLflow Models produced by this flavor.
              Calls to :func:`save_model()` and :func:`log_model()` produce a pip environment
              that, at minimum, contains these requirements.
     """
-    # todo pandas <=2
-    return [
-        _get_pinned_requirement("johnsnowlabs"),
-        "https://pypi.johnsnowlabs.com/4.4.2-f771e88dcf8e1535585c5531824a595e92c0305c/spark-nlp-jsl/spark_nlp_jsl-4.4.2-py3-none-any.whl",
-        'pyspark==3.2.1',
-
-    ]
+    return [_get_pinned_requirement("xgboost")]
 
 
 def get_default_conda_env():
     """
     :return: The default Conda environment for MLflow Models produced by calls to
-             :func:`save_model()` and :func:`log_model()`. This Conda environment
-             contains the current version of PySpark that is installed on the caller's
-             system. ``dev`` versions of PySpark are replaced with stable versions in
-             the resulting Conda environment (e.g., if you are running PySpark version
-             ``2.4.5.dev0``, invoking this method produces a Conda environment with a
-             dependency on PySpark version ``2.4.5``).
+             :func:`save_model()` and :func:`log_model()`.
     """
     return _mlflow_conda_env(additional_pip_deps=get_default_pip_requirements())
 
 
-@format_docstring(LOG_MODEL_PARAM_DOCS.format(package_name="johnsnowlabs"))
-def log_model(
-        spark_model,
-        artifact_path,
-        conda_env=None,
-        code_paths=None,
-        dfs_tmpdir=None,
-        sample_input=None,
-        registered_model_name=None,
-        signature: ModelSignature = None,
-        input_example: ModelInputExample = None,
-        await_registration_for=DEFAULT_AWAIT_MAX_SLEEP_SECONDS,
-        pip_requirements=None,
-        extra_pip_requirements=None,
-        metadata=None,
+@format_docstring(LOG_MODEL_PARAM_DOCS.format(package_name=FLAVOR_NAME))
+def save_model(
+    xgb_model,
+    path,
+    conda_env=None,
+    code_paths=None,
+    mlflow_model=None,
+    signature: ModelSignature = None,
+    input_example: ModelInputExample = None,
+    pip_requirements=None,
+    extra_pip_requirements=None,
+    model_format="xgb",
+    metadata=None,
 ):
     """
-    Log a Spark MLlib model as an MLflow artifact for the current run. This uses the
-    MLlib persistence format and produces an MLflow Model with the Spark flavor.
-
-    Note: If no run is active, it will instantiate a run to obtain a run_id.
+    Save an XGBoost model to a path on the local file system.
 
-    :param spark_model: Spark model to be saved - MLflow can only save descendants of
-                        pyspark.ml.Model or pyspark.ml.Transformer which implement
-                        MLReadable and MLWritable.
-    :param artifact_path: Run relative artifact path.
-    :param conda_env: Either a dictionary representation of a Conda environment or the path to a
-                      Conda environment yaml file. If provided, this decsribes the environment
-                      this model should be run in. At minimum, it should specify the dependencies
-                      contained in :func:`get_default_conda_env()`. If `None`, the default
-                      :func:`get_default_conda_env()` environment is added to the model.
-                      The following is an *example* dictionary representation of a Conda
-                      environment::
-
-                        {
-                            'name': 'mlflow-env',
-                            'channels': ['defaults'],
-                            'dependencies': [
-                                'python=3.8.15',
-                                'pyspark=2.3.0'
-                            ]
-                        }
-    :param dfs_tmpdir: Temporary directory path on Distributed (Hadoop) File System (DFS) or local
-                       filesystem if running in local mode. The model is written in this
-                       destination and then copied into the model's artifact directory. This is
-                       necessary as Spark ML models read from and write to DFS if running on a
-                       cluster. If this operation completes successfully, all temporary files
-                       created on the DFS are removed. Defaults to ``/tmp/mlflow``.
-    :param sample_input: A sample input used to add the MLeap flavor to the model.
-                         This must be a PySpark DataFrame that the model can evaluate. If
-                         ``sample_input`` is ``None``, the MLeap flavor is not added.
-    :param registered_model_name: If given, create a model version under
-                                  ``registered_model_name``, also creating a registered model if one
-                                  with the given name does not exist.
+    :param xgb_model: XGBoost model (an instance of `xgboost.Booster`_ or
+                      models that implement the `scikit-learn API`_) to be saved.
+    :param path: Local path where the model is to be saved.
+    :param conda_env: {{ conda_env }}
+    :param code_paths: A list of local filesystem paths to Python file dependencies (or directories
+                       containing file dependencies). These files are *prepended* to the system
+                       path when the model is loaded.
+    :param mlflow_model: :py:mod:`mlflow.models.Model` this flavor is being added to.
 
     :param signature: :py:class:`ModelSignature <mlflow.models.ModelSignature>`
                       describes model input and output :py:class:`Schema <mlflow.types.Schema>`.
                       The model signature can be :py:func:`inferred <mlflow.models.infer_signature>`
                       from datasets with valid model input (e.g. the training dataset with target
                       column omitted) and valid model output (e.g. model predictions generated on
                       the training dataset), for example:
@@ -182,291 +134,125 @@
                         predictions = ...  # compute model predictions
                         signature = infer_signature(train, predictions)
     :param input_example: Input example provides one or several instances of valid
                           model input. The example can be used as a hint of what data to feed the
                           model. The given example will be converted to a Pandas DataFrame and then
                           serialized to json using the Pandas split-oriented format. Bytes are
                           base64-encoded.
-    :param await_registration_for: Number of seconds to wait for the model version to finish
-                            being created and is in ``READY`` status. By default, the function
-                            waits for five minutes. Specify 0 or None to skip waiting.
     :param pip_requirements: {{ pip_requirements }}
     :param extra_pip_requirements: {{ extra_pip_requirements }}
+    :param model_format: File format in which the model is to be saved.
     :param metadata: Custom metadata dictionary passed to the model and stored in the MLmodel file.
 
                      .. Note:: Experimental: This parameter may change or be removed in a future
                                              release without warning.
-    :return: A :py:class:`ModelInfo <mlflow.models.model.ModelInfo>` instance that contains the
-             metadata of the logged model.
-
-    .. code-block:: python
-        :caption: Example
-
-        from pyspark.ml import Pipeline
-        from pyspark.ml.classification import LogisticRegression
-        from pyspark.ml.feature import HashingTF, Tokenizer
-
-        training = spark.createDataFrame(
-            [
-                (0, "a b c d e spark", 1.0),
-                (1, "b d", 0.0),
-                (2, "spark f g h", 1.0),
-                (3, "hadoop mapreduce", 0.0),
-            ],
-            ["id", "text", "label"],
-        )
-        tokenizer = Tokenizer(inputCol="text", outputCol="words")
-        hashingTF = HashingTF(inputCol=tokenizer.getOutputCol(), outputCol="features")
-        lr = LogisticRegression(maxIter=10, regParam=0.001)
-        pipeline = Pipeline(stages=[tokenizer, hashingTF, lr])
-        model = pipeline.fit(training)
-        mlflow.spark.log_model(model, "spark-model")
-    """
-    # TODO add optional "jar loc" arg , if set we use those jars instead of from jsl home
-    # _validate_model(spark_model)
-
-    # TODO nlu pipe vs light vs etc
-
-    run_id = mlflow.tracking.fluent._get_or_start_run().info.run_id
-    run_root_artifact_uri = mlflow.get_artifact_uri()
-    remote_model_path = None
-    if _should_use_mlflowdbfs(run_root_artifact_uri):
-        # TODO WTF?
-        remote_model_path = append_to_uri_path(
-            run_root_artifact_uri, artifact_path, _JOHNSNOWLABS_MODEL_PATH_SUB
-        )
-        mlflowdbfs_path = _mlflowdbfs_path(run_id, artifact_path)
-        with databricks_utils.MlflowCredentialContext(
-                get_databricks_profile_uri_from_artifact_uri(run_root_artifact_uri)
-        ):
-            try:
-                # TODO NLU Save
-                _unpack_and_save_model(spark_model, mlflowdbfs_path)
-
-            except Exception as e:
-                raise MlflowException("failed to save spark model via mlflowdbfs") from e
+    """
+    import xgboost as xgb
 
-    # If the artifact URI is a local filesystem path, defer to Model.log() to persist the model,
-    # since Spark may not be able to write directly to the driver's filesystem. For example,
-    # writing to `file:/uri` will write to the local filesystem from each executor, which will
-    # be incorrect on multi-node clusters.
-    # If the artifact URI is not a local filesystem path we attempt to write directly to the
-    # artifact repo via Spark. If this fails, we defer to Model.log().
-    elif is_local_uri(run_root_artifact_uri) or not _maybe_save_model(
-            spark_model,
-            append_to_uri_path(run_root_artifact_uri, artifact_path),
-    ):
-        return Model.log(
-            artifact_path=artifact_path,
-            # flavor=mlflow.spark,  # TODO LOG JSL FLAVOR?!
-            flavor=mlflow.johnsnowlabs2,  # TODO LOG JSL FLAVOR?!
-            spark_model=spark_model,
-            conda_env=conda_env,
-            code_paths=code_paths,
-            dfs_tmpdir=dfs_tmpdir,
-            sample_input=sample_input,
-            registered_model_name=registered_model_name,
-            signature=signature,
-            input_example=input_example,
-            await_registration_for=await_registration_for,
-            pip_requirements=pip_requirements,
-            extra_pip_requirements=extra_pip_requirements,
-            metadata=metadata,
-        )
-    # Otherwise, override the default model log behavior and save model directly to artifact repo
-    mlflow_model = Model(artifact_path=artifact_path, run_id=run_id)
-    with TempDir() as tmp:
-        tmp_model_metadata_dir = tmp.path()
-        _save_model_metadata(
-            tmp_model_metadata_dir,
-            spark_model,
-            mlflow_model,
-            sample_input,
-            conda_env,
-            code_paths,
-            signature=signature,
-            input_example=input_example,
-            pip_requirements=pip_requirements,
-            extra_pip_requirements=extra_pip_requirements,
-            remote_model_path=remote_model_path,
-        )
-        mlflow.tracking.fluent.log_artifacts(tmp_model_metadata_dir, artifact_path)
-        mlflow.tracking.fluent._record_logged_model(mlflow_model)
-        if registered_model_name is not None:
-            mlflow.register_model(
-                f"runs:/{run_id}/{artifact_path}",
-                registered_model_name,
-                await_registration_for,
-            )
-        return mlflow_model.get_model_info()
+    _validate_env_arguments(conda_env, pip_requirements, extra_pip_requirements)
 
+    path = os.path.abspath(path)
+    _validate_and_prepare_target_save_path(path)
+    code_dir_subpath = _validate_and_copy_code_paths(code_paths, path)
 
-def _save_model_metadata(
-        dst_dir,
-        spark_model,
-        mlflow_model,
-        sample_input,
-        conda_env,
-        code_paths,
-        signature=None,
-        input_example=None,
-        pip_requirements=None,
-        extra_pip_requirements=None,
-        remote_model_path=None,
-):
-    """
-    Saves model metadata into the passed-in directory.
-    If mlflowdbfs is not used, the persisted metadata assumes that a model can be
-    loaded from a relative path to the metadata file (currently hard-coded to "sparkml").
-    If mlflowdbfs is used, remote_model_path should be provided, and the model needs to
-    be loaded from the remote_model_path.
-    """
-    import pyspark
-
-    if sample_input is not None:
-        mleap.add_to_model(
-            mlflow_model=mlflow_model,
-            path=dst_dir,
-            spark_model=spark_model,
-            sample_input=sample_input,
-        )
+    if mlflow_model is None:
+        mlflow_model = Model()
     if signature is not None:
         mlflow_model.signature = signature
     if input_example is not None:
-        _save_example(mlflow_model, input_example, dst_dir)
+        _save_example(mlflow_model, input_example, path)
+    if metadata is not None:
+        mlflow_model.metadata = metadata
+    model_data_subpath = f"model.{model_format}"
+    model_data_path = os.path.join(path, model_data_subpath)
 
-    code_dir_subpath = _validate_and_copy_code_paths(code_paths, dst_dir)
-    mlflow_model.add_flavor(
-        FLAVOR_NAME,
-        pyspark_version=pyspark.__version__,
-        model_data=_JOHNSNOWLABS_MODEL_PATH_SUB,
-        code=code_dir_subpath,
-    )
+    # Save an XGBoost model
+    xgb_model.save_model(model_data_path)
+    xgb_model_class = _get_fully_qualified_class_name(xgb_model)
     pyfunc.add_to_model(
         mlflow_model,
-        loader_module="mlflow.spark",
-        data=_JOHNSNOWLABS_MODEL_PATH_SUB,
+        loader_module="mlflow.xgboost",
+        data=model_data_subpath,
         conda_env=_CONDA_ENV_FILE_NAME,
         python_env=_PYTHON_ENV_FILE_NAME,
         code=code_dir_subpath,
     )
-    mlflow_model.save(os.path.join(dst_dir, MLMODEL_FILE_NAME))
+    mlflow_model.add_flavor(
+        FLAVOR_NAME,
+        xgb_version=xgb.__version__,
+        data=model_data_subpath,
+        model_class=xgb_model_class,
+        model_format=model_format,
+        code=code_dir_subpath,
+    )
+    mlflow_model.save(os.path.join(path, MLMODEL_FILE_NAME))
 
     if conda_env is None:
         if pip_requirements is None:
             default_reqs = get_default_pip_requirements()
-            if remote_model_path:
-                _logger.info(
-                    "Inferring pip requirements by reloading the logged model from the databricks "
-                    "artifact repository, which can be time-consuming. To speed up, explicitly "
-                    "specify the conda_env or pip_requirements when calling log_model()."
-                )
             # To ensure `_load_pyfunc` can successfully load the model during the dependency
             # inference, `mlflow_model.save` must be called beforehand to save an MLmodel file.
             inferred_reqs = mlflow.models.infer_pip_requirements(
-                remote_model_path or dst_dir,
+                path,
                 FLAVOR_NAME,
                 fallback=default_reqs,
             )
             default_reqs = sorted(set(inferred_reqs).union(default_reqs))
         else:
             default_reqs = None
         conda_env, pip_requirements, pip_constraints = _process_pip_requirements(
             default_reqs,
             pip_requirements,
             extra_pip_requirements,
         )
     else:
         conda_env, pip_requirements, pip_constraints = _process_conda_env(conda_env)
 
-    with open(os.path.join(dst_dir, _CONDA_ENV_FILE_NAME), "w") as f:
+    with open(os.path.join(path, _CONDA_ENV_FILE_NAME), "w") as f:
         yaml.safe_dump(conda_env, stream=f, default_flow_style=False)
 
     # Save `constraints.txt` if necessary
     if pip_constraints:
-        write_to(os.path.join(dst_dir, _CONSTRAINTS_FILE_NAME), "\n".join(pip_constraints))
+        write_to(os.path.join(path, _CONSTRAINTS_FILE_NAME), "\n".join(pip_constraints))
 
     # Save `requirements.txt`
-    write_to(os.path.join(dst_dir, _REQUIREMENTS_FILE_NAME), "\n".join(pip_requirements))
-
-    _PythonEnv.current().to_yaml(os.path.join(dst_dir, _PYTHON_ENV_FILE_NAME))
-
-    # TODO JARS and LIC
-    save_jars_and_lic(dst_dir)
-
-def save_jars_and_lic(dst_dir):
-        deps_data_path = os.path.join(dst_dir,_JOHNSNOWLABS_MODEL_PATH_SUB, "jars.jsl")
-        Path(deps_data_path).mkdir(parents=True, exist_ok=True)
+    write_to(os.path.join(path, _REQUIREMENTS_FILE_NAME), "\n".join(pip_requirements))
 
-        from johnsnowlabs import nlp
-        import shutil
-        suite = get_install_suite_from_jsl_home(False)
-        if suite.hc.get_java_path():
-            shutil.copyfile(suite.hc.get_java_path(), os.path.join(deps_data_path, 'hc_jar.jar'))
-        if suite.nlp.get_java_path():
-            shutil.copyfile(suite.nlp.get_java_path(), os.path.join(deps_data_path, 'os_jar.jar'))
+    _PythonEnv.current().to_yaml(os.path.join(path, _PYTHON_ENV_FILE_NAME))
 
-        secrets = JslSecrets.build_or_try_find_secrets()
-        if secrets.HC_LICENSE:
-            with open(os.path.join(deps_data_path, 'license.json'), 'w') as f:
-                f.write(secrets.json())
 
-
-@format_docstring(LOG_MODEL_PARAM_DOCS.format(package_name="pyspark"))
-def save_model(
-        spark_model,
-        path,
-        mlflow_model=None,
-        conda_env=None,
-        code_paths=None,
-        dfs_tmpdir=None,
-        sample_input=None,
-        signature: ModelSignature = None,
-        input_example: ModelInputExample = None,
-        pip_requirements=None,
-        extra_pip_requirements=None,
-        metadata=None,
+@format_docstring(LOG_MODEL_PARAM_DOCS.format(package_name=FLAVOR_NAME))
+def log_model(
+    xgb_model,
+    artifact_path,
+    conda_env=None,
+    code_paths=None,
+    registered_model_name=None,
+    signature: ModelSignature = None,
+    input_example: ModelInputExample = None,
+    await_registration_for=DEFAULT_AWAIT_MAX_SLEEP_SECONDS,
+    pip_requirements=None,
+    extra_pip_requirements=None,
+    model_format="xgb",
+    metadata=None,
+    **kwargs,
 ):
     """
-    Save a Spark MLlib Model to a local path.
+    Log an XGBoost model as an MLflow artifact for the current run.
 
-    By default, this function saves models using the Spark MLlib persistence mechanism.
-    Additionally, if a sample input is specified using the ``sample_input`` parameter, the model
-    is also serialized in MLeap format and the MLeap flavor is added.
-
-    :param spark_model: Spark model to be saved - MLflow can only save descendants of
-                        pyspark.ml.Model or pyspark.ml.Transformer which implement
-                        MLReadable and MLWritable.
-    :param path: Local path where the model is to be saved.
-    :param mlflow_model: MLflow model config this flavor is being added to.
-    :param conda_env: Either a dictionary representation of a Conda environment or the path to a
-                      Conda environment yaml file. If provided, this decsribes the environment
-                      this model should be run in. At minimum, it should specify the dependencies
-                      contained in :func:`get_default_conda_env()`. If `None`, the default
-                      :func:`get_default_conda_env()` environment is added to the model.
-                      The following is an *example* dictionary representation of a Conda
-                      environment::
-
-                        {
-                            'name': 'mlflow-env',
-                            'channels': ['defaults'],
-                            'dependencies': [
-                                'python=3.8.15',
-                                'pyspark=2.3.0'
-                            ]
-                        }
-    :param dfs_tmpdir: Temporary directory path on Distributed (Hadoop) File System (DFS) or local
-                       filesystem if running in local mode. The model is be written in this
-                       destination and then copied to the requested local path. This is necessary
-                       as Spark ML models read from and write to DFS if running on a cluster. All
-                       temporary files created on the DFS are removed if this operation
-                       completes successfully. Defaults to ``/tmp/mlflow``.
-    :param sample_input: A sample input that is used to add the MLeap flavor to the model.
-                         This must be a PySpark DataFrame that the model can evaluate. If
-                         ``sample_input`` is ``None``, the MLeap flavor is not added.
+    :param xgb_model: XGBoost model (an instance of `xgboost.Booster`_ or
+                      models that implement the `scikit-learn API`_) to be saved.
+    :param artifact_path: Run-relative artifact path.
+    :param conda_env: {{ conda_env }}
+    :param code_paths: A list of local filesystem paths to Python file dependencies (or directories
+                       containing file dependencies). These files are *prepended* to the system
+                       path when the model is loaded.
+    :param registered_model_name: If given, create a model version under
+                                  ``registered_model_name``, also creating a registered model if one
+                                  with the given name does not exist.
 
     :param signature: :py:class:`ModelSignature <mlflow.models.ModelSignature>`
                       describes model input and output :py:class:`Schema <mlflow.types.Schema>`.
                       The model signature can be :py:func:`inferred <mlflow.models.infer_signature>`
                       from datasets with valid model input (e.g. the training dataset with target
                       column omitted) and valid model output (e.g. model predictions generated on
                       the training dataset), for example:
@@ -479,325 +265,495 @@
                         predictions = ...  # compute model predictions
                         signature = infer_signature(train, predictions)
     :param input_example: Input example provides one or several instances of valid
                           model input. The example can be used as a hint of what data to feed the
                           model. The given example will be converted to a Pandas DataFrame and then
                           serialized to json using the Pandas split-oriented format. Bytes are
                           base64-encoded.
+    :param await_registration_for: Number of seconds to wait for the model version to finish
+                            being created and is in ``READY`` status. By default, the function
+                            waits for five minutes. Specify 0 or None to skip waiting.
     :param pip_requirements: {{ pip_requirements }}
     :param extra_pip_requirements: {{ extra_pip_requirements }}
+    :param model_format: File format in which the model is to be saved.
     :param metadata: Custom metadata dictionary passed to the model and stored in the MLmodel file.
 
                      .. Note:: Experimental: This parameter may change or be removed in a future
                                              release without warning.
-
-    .. code-block:: python
-        :caption: Example
-
-        from mlflow import spark
-        from pyspark.ml.pipeline import PipelineModel
-
-        # your pyspark.ml.pipeline.PipelineModel type
-        model = ...
-        mlflow.spark.save_model(model, "spark-model")
+    :param kwargs: kwargs to pass to `xgboost.Booster.save_model`_ method.
+    :return: A :py:class:`ModelInfo <mlflow.models.model.ModelInfo>` instance that contains the
+             metadata of the logged model.
     """
-    # _validate_model(spark_model)
-    # _validate_env_arguments(conda_env, pip_requirements, extra_pip_requirements)
-
-    if mlflow_model is None:
-        mlflow_model = Model()
-    if metadata is not None:
-        mlflow_model.metadata = metadata
-    # Spark ML stores the model on DFS if running on a cluster
-    # Save it to a DFS temp dir first and copy it to local path
-    if dfs_tmpdir is None:
-        dfs_tmpdir = MLFLOW_DFS_TMP.get()
-    tmp_path = generate_tmp_dfs_path(dfs_tmpdir)
-
-    # Spark Session already is running if we have a model, so no need to check or create
-    _unpack_and_save_model(spark_model, tmp_path)
-    sparkml_data_path = os.path.abspath(os.path.join(path, _JOHNSNOWLABS_MODEL_PATH_SUB))
-    # We're copying the Spark model from DBFS to the local filesystem if (a) the temporary DFS URI
-    # we saved the Spark model to is a DBFS URI ("dbfs:/my-directory"), or (b) if we're running
-    # on a Databricks cluster and the URI is schemeless (e.g. looks like a filesystem absolute path
-    # like "/my-directory")
-    copying_from_dbfs = is_valid_dbfs_uri(tmp_path) or (
-            databricks_utils.is_in_cluster() and posixpath.abspath(tmp_path) == tmp_path
-    )
-    if copying_from_dbfs and databricks_utils.is_dbfs_fuse_available():
-        tmp_path_fuse = dbfs_hdfs_uri_to_fuse_path(tmp_path)
-        shutil.move(src=tmp_path_fuse, dst=sparkml_data_path)
-    else:
-        _HadoopFileSystem.copy_to_local_file(tmp_path, sparkml_data_path, remove_src=True)
-    _save_model_metadata(
-        dst_dir=path,
-        spark_model=spark_model,
-        mlflow_model=mlflow_model,
-        sample_input=sample_input,
+    return Model.log(
+        artifact_path=artifact_path,
+        flavor=mlflow.xgboost,
+        registered_model_name=registered_model_name,
+        xgb_model=xgb_model,
+        model_format=model_format,
         conda_env=conda_env,
         code_paths=code_paths,
         signature=signature,
         input_example=input_example,
+        await_registration_for=await_registration_for,
         pip_requirements=pip_requirements,
         extra_pip_requirements=extra_pip_requirements,
+        metadata=metadata,
+        **kwargs,
     )
 
 
-def _load_model_databricks(dfs_tmpdir, local_model_path):
-    # Spark ML expects the model to be stored on DFS
-    # Copy the model to a temp DFS location first. We cannot delete this file, as
-    # Spark may read from it at any point.
-    fuse_dfs_tmpdir = dbfs_hdfs_uri_to_fuse_path(dfs_tmpdir)
-    os.makedirs(fuse_dfs_tmpdir)
-    # Workaround for inability to use shutil.copytree with DBFS FUSE due to permission-denied
-    # errors on passthrough-enabled clusters when attempting to copy permission bits for directories
-    shutil_copytree_without_file_permissions(src_dir=local_model_path, dst_dir=fuse_dfs_tmpdir)
-    return nlp.load(dfs_tmpdir)
-
-
-def _load_model(model_uri, dfs_tmpdir_base=None, local_model_path=None):
-    dfs_tmpdir = generate_tmp_dfs_path(dfs_tmpdir_base or MLFLOW_DFS_TMP.get())
-    if databricks_utils.is_in_cluster() and databricks_utils.is_dbfs_fuse_available():
-        return _load_model_databricks(
-            dfs_tmpdir, local_model_path or _download_artifact_from_uri(model_uri)
-        )
-    # TODO use uri??? Not Supported
-    # model_uri = _HadoopFileSystem.maybe_copy_from_uri(model_uri, dfs_tmpdir, local_model_path)
-    # Make sure spark session is running before we try loading
+def _load_model(path):
+    """
+    Load Model Implementation.
 
+    :param path: Local filesystem path to
+                    the MLflow Model with the ``xgboost`` flavor (MLflow < 1.22.0) or
+                    the top-level MLflow Model directory (MLflow >= 1.22.0).
+    """
+    model_dir = os.path.dirname(path) if os.path.isfile(path) else path
+    flavor_conf = _get_flavor_configuration(model_path=model_dir, flavor_name=FLAVOR_NAME)
+
+    # XGBoost models saved in MLflow >=1.22.0 have `model_class`
+    # in the XGBoost flavor configuration to specify its XGBoost model class.
+    # When loading models, we first get the XGBoost model from
+    # its flavor configuration and then create an instance based on its class.
+    model_class = flavor_conf.get("model_class", "xgboost.core.Booster")
+    xgb_model_path = os.path.join(model_dir, flavor_conf.get("data"))
+
+    model = _get_class_from_string(model_class)()
+    model.load_model(xgb_model_path)
+    return model
 
-    if model_uri and not local_model_path :
-        local_model_path = _download_artifact_from_uri(model_uri)
-    get_or_create_sparksession(local_model_path)
-    # return nlp.load(model_uri)
-    return nlp.load(path=local_model_path)
+
+def _load_pyfunc(path):
+    """
+    Load PyFunc implementation. Called by ``pyfunc.load_model``.
+
+    :param path: Local filesystem path to the MLflow Model with the ``xgboost`` flavor.
+    """
+    return _XGBModelWrapper(_load_model(path))
 
 
-def load_model(model_uri, dfs_tmpdir=None, dst_path=None):
+def load_model(model_uri, dst_path=None):
     """
-    Load the Spark MLlib model from the path.
+    Load an XGBoost model from a local file or a run.
 
-    :param model_uri: The location, in URI format, of the MLflow model, for example:
+    :param model_uri: The location, in URI format, of the MLflow model. For example:
 
                       - ``/Users/me/path/to/local/model``
                       - ``relative/path/to/local/model``
                       - ``s3://my_bucket/path/to/model``
                       - ``runs:/<mlflow_run_id>/run-relative/path/to/model``
-                      - ``models:/<model_name>/<model_version>``
-                      - ``models:/<model_name>/<stage>``
 
                       For more information about supported URI schemes, see
-                      `Referencing Artifacts <https://www.mlflow.org/docs/latest/concepts.html#
+                      `Referencing Artifacts <https://www.mlflow.org/docs/latest/tracking.html#
                       artifact-locations>`_.
-    :param dfs_tmpdir: Temporary directory path on Distributed (Hadoop) File System (DFS) or local
-                       filesystem if running in local mode. The model is loaded from this
-                       destination. Defaults to ``/tmp/mlflow``.
     :param dst_path: The local filesystem path to which to download the model artifact.
                      This directory must already exist. If unspecified, a local output
                      path will be created.
-    :return: pyspark.ml.pipeline.PipelineModel
-
-    .. code-block:: python
-        :caption: Example
-
-        from mlflow import spark
 
-        model = mlflow.spark.load_model("spark-model")
-        # Prepare test documents, which are unlabeled (id, text) tuples.
-        test = spark.createDataFrame(
-            [(4, "spark i j k"), (5, "l m n"), (6, "spark hadoop spark"), (7, "apache hadoop")],
-            ["id", "text"],
-        )
-        # Make predictions on test documents
-        prediction = model.transform(test)
+    :return: An XGBoost model. An instance of either `xgboost.Booster`_ or XGBoost scikit-learn
+             models, depending on the saved model class specification.
     """
-    # This MUST be called prior to appending the model flavor to `model_uri` in order
-    # for `artifact_path` to take on the correct value for model loading via mlflowdbfs.
-    root_uri, artifact_path = _get_root_uri_and_artifact_path(model_uri)
-
-    flavor_conf = _get_flavor_configuration_from_uri(model_uri, FLAVOR_NAME, _logger)
-    local_mlflow_model_path = _download_artifact_from_uri(
-        artifact_uri=model_uri, output_path=dst_path
-    )
-    _add_code_from_conf_to_system_path(local_mlflow_model_path, flavor_conf)
+    local_model_path = _download_artifact_from_uri(artifact_uri=model_uri, output_path=dst_path)
+    flavor_conf = _get_flavor_configuration(local_model_path, FLAVOR_NAME)
+    _add_code_from_conf_to_system_path(local_model_path, flavor_conf)
+    return _load_model(path=local_model_path)
 
-    if _should_use_mlflowdbfs(model_uri):
-        from pyspark.ml.pipeline import PipelineModel
-
-        mlflowdbfs_path = _mlflowdbfs_path(
-            DatabricksArtifactRepository._extract_run_id(model_uri), artifact_path
-        )
-        with databricks_utils.MlflowCredentialContext(
-                get_databricks_profile_uri_from_artifact_uri(root_uri)
-        ):
-            return PipelineModel.load(mlflowdbfs_path)
-
-    sparkml_model_uri = append_to_uri_path(model_uri, flavor_conf["model_data"])
-    local_sparkml_model_path = os.path.join(local_mlflow_model_path, flavor_conf["model_data"])
-    return _load_model(
-        model_uri=sparkml_model_uri,
-        dfs_tmpdir_base=dfs_tmpdir,
-        local_model_path=local_sparkml_model_path,
-    )
 
+class _XGBModelWrapper:
+    def __init__(self, xgb_model):
+        self.xgb_model = xgb_model
 
-def _load_pyfunc(path):
-    """
-    Load PyFunc implementation. Called by ``pyfunc.load_model``.
-    :param path: Local filesystem path to the MLflow Model with the ``spark`` flavor.
-    """
-    # spark = _create_local_spark_session_for_loading_spark_model()
-    print(f"LOAD MODEL FROM ",path)
-    return _PyFuncModelWrapper(_load_model(model_uri=path), get_or_create_sparksession(path))
-
-
-def get_or_create_sparksession(model_path=None):
-    """
-    1. Check if SparkSession running and get it
-    2. If none exists, create a new one using jars in model_path
-    3. If model_path not defined, rely on nlp.start() to create a new
-    one using johnsnowlabs Jar resolution method
-    See https://nlp.johnsnowlabs.com/docs/en/jsl/start-a-sparksession
-    and https://nlp.johnsnowlabs.com/docs/en/jsl/install_advanced
-    :param model_path:
-    :return:
-    """
-
-    from mlflow.utils._spark_utils import _get_active_spark_session
-    spark = _get_active_spark_session()
-    if spark:
-        print(f'SPARKSESSIOON ALREADY ACTIIIIIIIVE!!!')
-    if spark is None:
-        os.environ['PYSPARK_PYTHON'] = sys.executable
-        os.environ['PYSPARK_DRIVER_PYTHON'] = sys.executable
-
-        if model_path:
-            jar_paths, license_path = fetch_deps_from_path(os.path.join(model_path ))
-            if license_path:
-                os.environ.update({k: str(v) for k, v in json.load(open(license_path)).items() if v is not None})
-                os.environ['JSL_NLP_LICENSE'] = json.load(open(license_path))['HC_LICENSE']
+    def predict(self, dataframe):
+        import xgboost as xgb
 
-            spark = nlp.start(nlp=False, spark_nlp=False, jar_paths=jar_paths, json_license_path=license_path)
+        if isinstance(self.xgb_model, xgb.Booster):
+            return self.xgb_model.predict(xgb.DMatrix(dataframe))
         else:
-            spark = nlp.start()
-    return spark
-
+            return self.xgb_model.predict(dataframe)
 
-def fetch_deps_from_path(local_model_path):
-    local_model_path = os.path.join(local_model_path, 'jars.jsl', )
-    jar_paths = [os.path.join(local_model_path, file) for file in os.listdir(local_model_path) if '.jar' in file]
-    license_path = [os.path.join(local_model_path, file) for file in os.listdir(local_model_path) if '.json' in file]
-    license_path = license_path[0] if license_path else None
-    return jar_paths, license_path
 
+@autologging_integration(FLAVOR_NAME)
+def autolog(
+    importance_types=None,
+    log_input_examples=False,
+    log_model_signatures=True,
+    log_models=True,
+    disable=False,
+    exclusive=False,
+    disable_for_unsupported_versions=False,
+    silent=False,
+    registered_model_name=None,
+    model_format="xgb",
+):  # pylint: disable=W0102,unused-argument
+    """
+    Enables (or disables) and configures autologging from XGBoost to MLflow. Logs the following:
+
+    - parameters specified in `xgboost.train`_.
+    - metrics on each iteration (if ``evals`` specified).
+    - metrics at the best iteration (if ``early_stopping_rounds`` specified).
+    - feature importance as JSON files and plots.
+    - trained model, including:
+        - an example of valid input.
+        - inferred signature of the inputs and outputs of the model.
+
+    Note that the `scikit-learn API`_ is now supported.
+
+    :param importance_types: Importance types to log. If unspecified, defaults to ``["weight"]``.
+    :param log_input_examples: If ``True``, input examples from training datasets are collected and
+                               logged along with XGBoost model artifacts during training. If
+                               ``False``, input examples are not logged.
+                               Note: Input examples are MLflow model attributes
+                               and are only collected if ``log_models`` is also ``True``.
+    :param log_model_signatures: If ``True``,
+                                 :py:class:`ModelSignatures <mlflow.models.ModelSignature>`
+                                 describing model inputs and outputs are collected and logged along
+                                 with XGBoost model artifacts during training. If ``False``,
+                                 signatures are not logged.
+                                 Note: Model signatures are MLflow model attributes
+                                 and are only collected if ``log_models`` is also ``True``.
+    :param log_models: If ``True``, trained models are logged as MLflow model artifacts.
+                       If ``False``, trained models are not logged.
+                       Input examples and model signatures, which are attributes of MLflow models,
+                       are also omitted when ``log_models`` is ``False``.
+    :param disable: If ``True``, disables the XGBoost autologging integration. If ``False``,
+                    enables the XGBoost autologging integration.
+    :param exclusive: If ``True``, autologged content is not logged to user-created fluent runs.
+                      If ``False``, autologged content is logged to the active fluent run,
+                      which may be user-created.
+    :param disable_for_unsupported_versions: If ``True``, disable autologging for versions of
+                      xgboost that have not been tested against this version of the MLflow client
+                      or are incompatible.
+    :param silent: If ``True``, suppress all event logs and warnings from MLflow during XGBoost
+                   autologging. If ``False``, show all events and warnings during XGBoost
+                   autologging.
+    :param registered_model_name: If given, each time a model is trained, it is registered as a
+                                  new model version of the registered model with this name.
+                                  The registered model is created if it does not already exist.
+    :param model_format: File format in which the model is to be saved.
+    """
+    import functools
+    import xgboost
+    import numpy as np
+
+    if importance_types is None:
+        importance_types = ["weight"]
+
+    # Patching this function so we can get a copy of the data given to DMatrix.__init__
+    #   to use as an input example and for inferring the model signature.
+    #   (there is no way to get the data back from a DMatrix object)
+    # We store it on the DMatrix object so the train function is able to read it.
+    def __init__(original, self, *args, **kwargs):
+        data = args[0] if len(args) > 0 else kwargs.get("data")
 
-def _unpack_and_save_model(spark_model, dst):
-    if isinstance(spark_model, _PyFuncModelWrapper):
-        spark_model = spark_model.spark_model
-    spark_model.vanilla_transformer_pipe.write().overwrite().save(dst)
-
+        if data is not None:
+            try:
+                if isinstance(data, str):
+                    raise Exception(
+                        "cannot gather example input when dataset is loaded from a file."
+                    )
 
+                input_example_info = InputExampleInfo(
+                    input_example=deepcopy(data[:INPUT_EXAMPLE_SAMPLE_ROWS])
+                )
+            except Exception as e:
+                input_example_info = InputExampleInfo(error_msg=str(e))
 
-class _PyFuncModelWrapper:
-    """
-    Wrapper around Spark MLlib PipelineModel providing interface for scoring pandas DataFrame.
-    """
+            self.input_example_info = input_example_info
 
-    def __init__(self, spark_model, spark=None, ):
-        # we have this ternary, so we support _PyFuncModelWrapper(nlu_ref)
-        self.spark = spark if spark else nlp.start()
-        self.spark_model = spark_model
+        original(self, *args, **kwargs)
 
-    def predict(self, text, output_level=None):
-        """
-        Generate predictions given input data in a pandas DataFrame.
+    def train_impl(_log_models, original, *args, **kwargs):
+        def record_eval_results(eval_results, metrics_logger):
+            """
+            Create a callback function that records evaluation results.
+            """
+            # TODO: Remove `replace("SNAPSHOT", "dev")` once the following issue is addressed:
+            #       https://github.com/dmlc/xgboost/issues/6984
+            from mlflow.xgboost._autolog import IS_TRAINING_CALLBACK_SUPPORTED
+
+            if IS_TRAINING_CALLBACK_SUPPORTED:
+                from mlflow.xgboost._autolog import AutologCallback
+
+                # In xgboost >= 1.3.0, user-defined callbacks should inherit
+                # `xgboost.callback.TrainingCallback`:
+                # https://xgboost.readthedocs.io/en/latest/python/callbacks.html#defining-your-own-callback
+                return AutologCallback(metrics_logger, eval_results)
+            else:
+                from mlflow.xgboost._autolog import autolog_callback
+
+                return picklable_exception_safe_function(
+                    functools.partial(
+                        autolog_callback, metrics_logger=metrics_logger, eval_results=eval_results
+                    )
+                )
 
-        :param output_level:
-        :param text: pandas DataFrame containing input data.
-        :return: List with model predictions.
-        """
-        return self.spark_model.predict(text, output_level=output_level).to_json()
+        def log_feature_importance_plot(features, importance, importance_type):
+            """
+            Log feature importance plot.
+            """
+            import matplotlib.pyplot as plt
+            from cycler import cycler
+
+            features = np.array(features)
+
+            # Structure the supplied `importance` values as a `num_features`-by-`num_classes` matrix
+            importances_per_class_by_feature = np.array(importance)
+            if importances_per_class_by_feature.ndim <= 1:
+                # In this case, the supplied `importance` values are not given per class. Rather,
+                # one importance value is given per feature. For consistency with the assumed
+                # `num_features`-by-`num_classes` matrix structure, we coerce the importance
+                # values to a `num_features`-by-1 matrix
+                indices = np.argsort(importance)
+                # Sort features and importance values by magnitude during transformation to a
+                # `num_features`-by-`num_classes` matrix
+                features = features[indices]
+                importances_per_class_by_feature = np.array(
+                    [[importance] for importance in importances_per_class_by_feature[indices]]
+                )
+                # In this case, do not include class labels on the feature importance plot because
+                # only one importance value has been provided per feature, rather than an
+                # one importance value for each class per feature
+                label_classes_on_plot = False
+            else:
+                importance_value_magnitudes = np.abs(importances_per_class_by_feature).sum(axis=1)
+                indices = np.argsort(importance_value_magnitudes)
+                features = features[indices]
+                importances_per_class_by_feature = importances_per_class_by_feature[indices]
+                label_classes_on_plot = True
+
+            num_classes = importances_per_class_by_feature.shape[1]
+            num_features = len(features)
+
+            # If num_features > 10, increase the figure height to prevent the plot
+            # from being too dense.
+            w, h = [6.4, 4.8]  # matplotlib's default figure size
+            h = h + 0.1 * num_features if num_features > 10 else h
+            h = h + 0.1 * num_classes if num_classes > 1 else h
+            fig, ax = plt.subplots(figsize=(w, h))
+            # When importance values are provided for each class per feature, we want to ensure
+            # that the same color is used for all bars in the bar chart that have the same class
+            colors_to_cycle = plt.rcParams["axes.prop_cycle"].by_key()["color"][:num_classes]
+            color_cycler = cycler(color=colors_to_cycle)
+            ax.set_prop_cycle(color_cycler)
+
+            # The following logic operates on one feature at a time, adding a bar to the bar chart
+            # for each class that reflects the importance of the feature to predictions of that
+            # class
+            feature_ylocs = np.arange(num_features)
+            # Define offsets on the y-axis that are used to evenly space the bars for each class
+            # around the y-axis position of each feature
+            offsets_per_yloc = np.linspace(-0.5, 0.5, num_classes) / 2 if num_classes > 1 else [0]
+            for feature_idx, (feature_yloc, importances_per_class) in enumerate(
+                zip(feature_ylocs, importances_per_class_by_feature)
+            ):
+                for class_idx, (offset, class_importance) in enumerate(
+                    zip(offsets_per_yloc, importances_per_class)
+                ):
+                    (bar,) = ax.barh(
+                        feature_yloc + offset,
+                        class_importance,
+                        align="center",
+                        # Set the bar height such that importance value bars for a particular
+                        # feature are spaced properly relative to each other (no overlap or gaps)
+                        # and relative to importance value bars for other features
+                        height=(0.5 / max(num_classes - 1, 1)),
+                    )
+                    if label_classes_on_plot and feature_idx == 0:
+                        # Only set a label the first time a bar for a particular class is plotted to
+                        # avoid duplicate legend entries. If we were to set a label for every bar,
+                        # the legend would contain `num_features` labels for each class.
+                        bar.set_label(f"Class {class_idx}")
+
+            ax.set_yticks(feature_ylocs)
+            ax.set_yticklabels(features)
+            ax.set_xlabel("Importance")
+            ax.set_title(f"Feature Importance ({importance_type})")
+            if label_classes_on_plot:
+                ax.legend()
+            fig.tight_layout()
 
+            tmpdir = tempfile.mkdtemp()
+            try:
+                # pylint: disable=undefined-loop-variable
+                filepath = os.path.join(tmpdir, f"feature_importance_{imp_type}.png")
+                fig.savefig(filepath)
+                mlflow.log_artifact(filepath)
+            finally:
+                plt.close(fig)
+                shutil.rmtree(tmpdir)
+
+        autologging_client = MlflowAutologgingQueueingClient()
+        # logging booster params separately to extract key/value pairs and make it easier to
+        # compare them across runs.
+        booster_params = args[0] if len(args) > 0 else kwargs["params"]
+        autologging_client.log_params(run_id=mlflow.active_run().info.run_id, params=booster_params)
+
+        unlogged_params = [
+            "params",
+            "dtrain",
+            "evals",
+            "obj",
+            "feval",
+            "evals_result",
+            "xgb_model",
+            "callbacks",
+            "learning_rates",
+        ]
+        params_to_log_for_fn = get_mlflow_run_params_for_fn_args(
+            original, args, kwargs, unlogged_params
+        )
+        autologging_client.log_params(
+            run_id=mlflow.active_run().info.run_id, params=params_to_log_for_fn
+        )
+
+        param_logging_operations = autologging_client.flush(synchronous=False)
+
+        all_arg_names = _get_arg_names(original)
+        num_pos_args = len(args)
+
+        # adding a callback that records evaluation results.
+        eval_results = []
+        callbacks_index = all_arg_names.index("callbacks")
+
+        run_id = mlflow.active_run().info.run_id
+        with batch_metrics_logger(run_id) as metrics_logger:
+            callback = record_eval_results(eval_results, metrics_logger)
+            if num_pos_args >= callbacks_index + 1:
+                tmp_list = list(args)
+                tmp_list[callbacks_index] += [callback]
+                args = tuple(tmp_list)
+            elif "callbacks" in kwargs and kwargs["callbacks"] is not None:
+                kwargs["callbacks"] += [callback]
+            else:
+                kwargs["callbacks"] = [callback]
+
+            # training model
+            model = original(*args, **kwargs)
+
+            # If early_stopping_rounds is present, logging metrics at the best iteration
+            # as extra metrics with the max step + 1.
+            early_stopping_index = all_arg_names.index("early_stopping_rounds")
+            early_stopping = num_pos_args >= early_stopping_index + 1 or kwargs.get(
+                "early_stopping_rounds"
+            )
+            if early_stopping:
+                extra_step = len(eval_results)
+                autologging_client.log_metrics(
+                    run_id=mlflow.active_run().info.run_id,
+                    metrics={
+                        "stopped_iteration": extra_step - 1,
+                        "best_iteration": model.best_iteration,
+                    },
+                )
+                autologging_client.log_metrics(
+                    run_id=mlflow.active_run().info.run_id,
+                    metrics=eval_results[model.best_iteration],
+                    step=extra_step,
+                )
+                early_stopping_logging_operations = autologging_client.flush(synchronous=False)
 
-@autologging_integration(FLAVOR_NAME)
-def autolog(disable=False, silent=False):  # pylint: disable=unused-argument
-    """
-    Enables (or disables) and configures logging of Spark datasource paths, versions
-    (if applicable), and formats when they are read. This method is not threadsafe and assumes a
-    `SparkSession
-    <https://spark.apache.org/docs/latest/api/python/pyspark.sql.html#pyspark.sql.SparkSession>`_
-    already exists with the
-    `mlflow-spark JAR
-    <http://mlflow.org/docs/latest/tracking.html#automatic-logging-from-spark-experimental>`_
-    attached. It should be called on the Spark driver, not on the executors (i.e. do not call
-    this method within a function parallelized by Spark). This API requires Spark 3.0 or above.
-
-    Datasource information is cached in memory and logged to all subsequent MLflow runs,
-    including the active MLflow run (if one exists when the data is read). Note that autologging of
-    Spark ML (MLlib) models is not currently supported via this API. Datasource autologging is
-    best-effort, meaning that if Spark is under heavy load or MLflow logging fails for any reason
-    (e.g., if the MLflow server is unavailable), logging may be dropped.
-
-    For any unexpected issues with autologging, check Spark driver and executor logs in addition
-    to stderr & stdout generated from your MLflow code - datasource information is pulled from
-    Spark, so logs relevant to debugging may show up amongst the Spark logs.
-
-    .. code-block:: python
-        :caption: Example
-
-        import mlflow.spark
-        import os
-        import shutil
-        from pyspark.sql import SparkSession
-
-        # Create and persist some dummy data
-        # Note: On environments like Databricks with pre-created SparkSessions,
-        # ensure the org.mlflow:mlflow-spark:1.11.0 is attached as a library to
-        # your cluster
-        spark = (
-            SparkSession.builder.config("spark.jars.packages", "org.mlflow:mlflow-spark:1.11.0")
-            .master("local[*]")
-            .getOrCreate()
-        )
-        df = spark.createDataFrame(
-            [(4, "spark i j k"), (5, "l m n"), (6, "spark hadoop spark"), (7, "apache hadoop")],
-            ["id", "text"],
-        )
-        import tempfile
+        # logging feature importance as artifacts.
+        for imp_type in importance_types:
+            imp = None
+            try:
+                imp = model.get_score(importance_type=imp_type)
+                features, importance = zip(*imp.items())
+                log_feature_importance_plot(features, importance, imp_type)
+            except Exception:
+                _logger.exception(
+                    "Failed to log feature importance plot. XGBoost autologging "
+                    "will ignore the failure and continue. Exception: "
+                )
 
-        tempdir = tempfile.mkdtemp()
-        df.write.csv(os.path.join(tempdir, "my-data-path"), header=True)
-        # Enable Spark datasource autologging.
-        mlflow.spark.autolog()
-        loaded_df = spark.read.csv(
-            os.path.join(tempdir, "my-data-path"), header=True, inferSchema=True
-        )
-        # Call toPandas() to trigger a read of the Spark datasource. Datasource info
-        # (path and format) is logged to the current active run, or the
-        # next-created MLflow run if no run is currently active
-        with mlflow.start_run() as active_run:
-            pandas_df = loaded_df.toPandas()
-
-    :param disable: If ``True``, disables the Spark datasource autologging integration.
-                    If ``False``, enables the Spark datasource autologging integration.
-    :param silent: If ``True``, suppress all event logs and warnings from MLflow during Spark
-                   datasource autologging. If ``False``, show all events and warnings during Spark
-                   datasource autologging.
-    """
-    from mlflow.utils._spark_utils import _get_active_spark_session
-    from mlflow._spark_autologging import _listen_for_spark_activity
-    from pyspark.sql import SparkSession
-    from pyspark import SparkContext
+            if imp is not None:
+                tmpdir = tempfile.mkdtemp()
+                try:
+                    filepath = os.path.join(tmpdir, f"feature_importance_{imp_type}.json")
+                    with open(filepath, "w") as f:
+                        json.dump(imp, f)
+                    mlflow.log_artifact(filepath)
+                finally:
+                    shutil.rmtree(tmpdir)
+
+        # dtrain must exist as the original train function already ran successfully
+        dtrain = args[1] if len(args) > 1 else kwargs.get("dtrain")
+
+        # it is possible that the dataset was constructed before the patched
+        #   constructor was applied, so we cannot assume the input_example_info exists
+        input_example_info = getattr(dtrain, "input_example_info", None)
+
+        def get_input_example():
+            if input_example_info is None:
+                raise Exception(ENSURE_AUTOLOGGING_ENABLED_TEXT)
+            if input_example_info.error_msg is not None:
+                raise Exception(input_example_info.error_msg)
+            return input_example_info.input_example
+
+        def infer_model_signature(input_example):
+            model_output = model.predict(xgboost.DMatrix(input_example))
+            model_signature = infer_signature(input_example, model_output)
+            return model_signature
+
+        # Only log the model if the autolog() param log_models is set to True.
+        if _log_models:
+            # Will only resolve `input_example` and `signature` if `log_models` is `True`.
+            input_example, signature = resolve_input_example_and_signature(
+                get_input_example,
+                infer_model_signature,
+                log_input_examples,
+                log_model_signatures,
+                _logger,
+            )
 
-    def __init__(original, self, *args, **kwargs):
-        original(self, *args, **kwargs)
+            registered_model_name = get_autologging_config(
+                FLAVOR_NAME, "registered_model_name", None
+            )
+            log_model(
+                model,
+                artifact_path="model",
+                signature=signature,
+                input_example=input_example,
+                registered_model_name=registered_model_name,
+                model_format=model_format,
+            )
 
-        _listen_for_spark_activity(self._sc)
+        param_logging_operations.await_completion()
+        if early_stopping:
+            early_stopping_logging_operations.await_completion()
+
+        return model
+
+    def train(_log_models, original, *args, **kwargs):
+        current_sklearn_session = _SklearnTrainingSession.get_current_session()
+        if current_sklearn_session is None or current_sklearn_session.should_log():
+            return train_impl(_log_models, original, *args, **kwargs)
+        else:
+            return original(*args, **kwargs)
 
-    safe_patch(FLAVOR_NAME, SparkSession, "__init__", __init__, manage_run=False)
+    safe_patch(FLAVOR_NAME, xgboost, "train", functools.partial(train, log_models), manage_run=True)
+    # The `train()` method logs XGBoost models as Booster objects. When using XGBoost
+    # scikit-learn models, we want to save / log models as their model classes. So we turn
+    # off the log_models functionality in the `train()` method patched to `xgboost.sklearn`.
+    # Instead the model logging is handled in `fit_mlflow_sklearn()` in `mlflow.sklearn._autolog()`,
+    # where models are logged as XGBoost scikit-learn models after the `fit()` method returns.
+    safe_patch(
+        FLAVOR_NAME, xgboost.sklearn, "train", functools.partial(train, False), manage_run=True
+    )
+    safe_patch(FLAVOR_NAME, xgboost.DMatrix, "__init__", __init__)
 
-    active_session = _get_active_spark_session()
-    if active_session is not None:
-        # We know SparkContext exists here already, so get it
-        sc = SparkContext.getOrCreate()
+    # enable xgboost scikit-learn estimators autologging
+    import mlflow.sklearn
 
-        _listen_for_spark_activity(sc)
+    mlflow.sklearn._autolog(
+        flavor_name=FLAVOR_NAME,
+        log_input_examples=log_input_examples,
+        log_model_signatures=log_model_signatures,
+        log_models=log_models,
+        disable=disable,
+        exclusive=exclusive,
+        disable_for_unsupported_versions=disable_for_unsupported_versions,
+        silent=silent,
+        max_tuning_runs=None,
+        log_post_training_metrics=True,
+    )
```

### Comparing `mlflow_tmp-2.2.9/mlflow/langchain/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/langchain/api_request_parallel_processor.py` & `mlflow_tmp-2.3.3.dev0/mlflow/langchain/api_request_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/lightgbm.py` & `mlflow_tmp-2.3.3.dev0/mlflow/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/ml_package_versions.py` & `mlflow_tmp-2.3.3.dev0/mlflow/ml_package_versions.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/mleap.py` & `mlflow_tmp-2.3.3.dev0/mlflow/mleap.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/cli.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/container/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/container/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/container/scoring_server/nginx.conf` & `mlflow_tmp-2.3.3.dev0/mlflow/models/container/scoring_server/nginx.conf`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/docker_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/docker_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/evaluation/_shap_patch.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/_shap_patch.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/evaluation/artifacts.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/artifacts.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/evaluation/base.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/evaluation/default_evaluator.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/default_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/evaluation/evaluator_registry.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/evaluator_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/evaluation/lift_curve.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/lift_curve.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/evaluation/validation.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/evaluation/validation.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/flavor_backend.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/flavor_backend.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/flavor_backend_registry.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/flavor_backend_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/model.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/model.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/signature.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/signature.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/models/wheeled_model.py` & `mlflow_tmp-2.3.3.dev0/mlflow/models/wheeled_model.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/onnx.py` & `mlflow_tmp-2.3.3.dev0/mlflow/onnx.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/openai/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/openai/api_request_parallel_processor.py` & `mlflow_tmp-2.3.3.dev0/mlflow/openai/api_request_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/openai/retry.py` & `mlflow_tmp-2.3.3.dev0/mlflow/openai/retry.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/openai/utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/openai/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/paddle/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/paddle/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/paddle/_paddle_autolog.py` & `mlflow_tmp-2.3.3.dev0/mlflow/paddle/_paddle_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pmdarima.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pmdarima.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/projects/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/projects/_project_spec.py` & `mlflow_tmp-2.3.3.dev0/mlflow/projects/_project_spec.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/projects/backend/abstract_backend.py` & `mlflow_tmp-2.3.3.dev0/mlflow/projects/backend/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/projects/backend/loader.py` & `mlflow_tmp-2.3.3.dev0/mlflow/projects/backend/loader.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/projects/backend/local.py` & `mlflow_tmp-2.3.3.dev0/mlflow/projects/backend/local.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/projects/databricks.py` & `mlflow_tmp-2.3.3.dev0/mlflow/projects/databricks.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/projects/docker.py` & `mlflow_tmp-2.3.3.dev0/mlflow/projects/docker.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/projects/kubernetes.py` & `mlflow_tmp-2.3.3.dev0/mlflow/projects/kubernetes.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/projects/submitted_run.py` & `mlflow_tmp-2.3.3.dev0/mlflow/projects/submitted_run.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/projects/utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/projects/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/prophet.py` & `mlflow_tmp-2.3.3.dev0/mlflow/prophet.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/protos/databricks_artifacts_pb2.py` & `mlflow_tmp-2.3.3.dev0/mlflow/protos/databricks_artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/protos/databricks_pb2.py` & `mlflow_tmp-2.3.3.dev0/mlflow/protos/databricks_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/protos/databricks_uc_registry_messages_pb2.py` & `mlflow_tmp-2.3.3.dev0/mlflow/protos/databricks_uc_registry_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/protos/databricks_uc_registry_service_pb2.py` & `mlflow_tmp-2.3.3.dev0/mlflow/protos/databricks_uc_registry_service_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/protos/facet_feature_statistics_pb2.py` & `mlflow_tmp-2.3.3.dev0/mlflow/protos/facet_feature_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/protos/mlflow_artifacts_pb2.py` & `mlflow_tmp-2.3.3.dev0/mlflow/protos/mlflow_artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/protos/model_registry_pb2.py` & `mlflow_tmp-2.3.3.dev0/mlflow/protos/model_registry_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/protos/scalapb/scalapb_pb2.py` & `mlflow_tmp-2.3.3.dev0/mlflow/protos/scalapb/scalapb_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/protos/service_pb2.py` & `mlflow_tmp-2.3.3.dev0/mlflow/protos/service_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pyfunc/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pyfunc/backend.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/backend.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pyfunc/mlserver.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/mlserver.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pyfunc/model.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/model.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pyfunc/scoring_server/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/scoring_server/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pyfunc/scoring_server/client.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/scoring_server/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pyfunc/spark_model_cache.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/spark_model_cache.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pyfunc/stdin_server.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pyfunc/stdin_server.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pypi_package_index.json` & `mlflow_tmp-2.3.3.dev0/mlflow/pypi_package_index.json`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pyspark/ml/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pyspark/ml/_autolog.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pyspark/ml/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pyspark/ml/log_model_allowlist.txt` & `mlflow_tmp-2.3.3.dev0/mlflow/pyspark/ml/log_model_allowlist.txt`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pytorch/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pytorch/_lightning_autolog.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pytorch/_lightning_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pytorch/_pytorch_autolog.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pytorch/_pytorch_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/pytorch/pickle_module.py` & `mlflow_tmp-2.3.3.dev0/mlflow/pytorch/pickle_module.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/artifacts.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/artifacts.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/cards/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/cards/histogram_generator.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/cards/histogram_generator.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/cards/pandas_renderer.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/cards/pandas_renderer.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/cards/templates/base.html` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/cards/templates/base.html`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/classification/v1/recipe.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/classification/v1/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/cli.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/dag_help_strings.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/dag_help_strings.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/recipe.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/regression/v1/recipe.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/regression/v1/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/resources/recipe_dag_template.html` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/resources/recipe_dag_template.html`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/step.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/step.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/steps/automl/flaml.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/automl/flaml.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/steps/evaluate.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/evaluate.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/steps/ingest/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/steps/ingest/datasets.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/ingest/datasets.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/steps/predict.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/predict.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/steps/register.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/register.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/steps/split.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/split.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/steps/train.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/train.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/steps/transform.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/steps/transform.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/utils/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/utils/execution.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/utils/execution.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/utils/metrics.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/utils/step.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/utils/step.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/utils/tracking.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/recipes/utils/wrapped_recipe_model.py` & `mlflow_tmp-2.3.3.dev0/mlflow/recipes/utils/wrapped_recipe_model.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/rfunc/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/rfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/rfunc/backend.py` & `mlflow_tmp-2.3.3.dev0/mlflow/rfunc/backend.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/runs.py` & `mlflow_tmp-2.3.3.dev0/mlflow/runs.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/sagemaker/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/sagemaker/cli.py` & `mlflow_tmp-2.3.3.dev0/mlflow/sagemaker/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/server/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/server/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/server/auth/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/server/auth/config.py` & `mlflow_tmp-2.3.3.dev0/mlflow/server/auth/config.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/server/auth/entities.py` & `mlflow_tmp-2.3.3.dev0/mlflow/server/auth/entities.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/server/auth/logo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/server/auth/logo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/server/auth/permissions.py` & `mlflow_tmp-2.3.3.dev0/mlflow/server/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/server/auth/sqlalchemy_store.py` & `mlflow_tmp-2.3.3.dev0/mlflow/server/auth/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/server/handlers.py` & `mlflow_tmp-2.3.3.dev0/mlflow/server/handlers.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/shap.py` & `mlflow_tmp-2.3.3.dev0/mlflow/shap.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/sklearn/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/sklearn/utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/sklearn/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/spacy.py` & `mlflow_tmp-2.3.3.dev0/mlflow/spacy.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/spark.py` & `mlflow_tmp-2.3.3.dev0/mlflow/spark.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/statsmodels.py` & `mlflow_tmp-2.3.3.dev0/mlflow/statsmodels.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/_unity_catalog/registry/rest_store.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/_unity_catalog/registry/rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/_unity_catalog/registry/utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/_unity_catalog/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/artifact_repository_registry.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/artifact_repository_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/azure_blob_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/azure_blob_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/azure_data_lake_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/azure_data_lake_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/cli.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/databricks_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/databricks_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/databricks_models_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/databricks_models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/dbfs_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/dbfs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/ftp_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/ftp_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/gcs_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/gcs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/hdfs_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/hdfs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/http_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/http_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/local_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/local_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/mlflow_artifacts_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/mlflow_artifacts_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/models_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/runs_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/runs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/s3_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/s3_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/sftp_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/sftp_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/unity_catalog_models_artifact_repo.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/unity_catalog_models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/artifact/utils/models.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/artifact/utils/models.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db/utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/alembic.ini` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/env.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/env.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/model_registry/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/model_registry/abstract_store.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/abstract_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/model_registry/base_rest_store.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/base_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/model_registry/dbmodels/models.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/dbmodels/models.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/model_registry/file_store.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/file_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/model_registry/rest_store.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/model_registry/sqlalchemy_store.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/model_registry/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/tracking/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/tracking/abstract_store.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/abstract_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/tracking/dbmodels/initial_models.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/dbmodels/initial_models.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/tracking/dbmodels/models.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/dbmodels/models.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/tracking/file_store.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/file_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/tracking/rest_store.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/store/tracking/sqlalchemy_store.py` & `mlflow_tmp-2.3.3.dev0/mlflow/store/tracking/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tensorflow/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tensorflow/_autolog.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tensorflow/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/_model_registry/client.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/_model_registry/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/_model_registry/fluent.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/_model_registry/fluent.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/_model_registry/registry.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/_model_registry/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/_model_registry/utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/_model_registry/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/_tracking_service/client.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/_tracking_service/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/_tracking_service/registry.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/_tracking_service/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/_tracking_service/utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/_tracking_service/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/artifact_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/client.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/context/abstract_context.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/abstract_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/context/databricks_cluster_context.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/databricks_cluster_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/context/databricks_command_context.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/databricks_command_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/context/databricks_job_context.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/databricks_job_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/context/databricks_notebook_context.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/databricks_notebook_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/context/databricks_repo_context.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/databricks_repo_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/context/default_context.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/default_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/context/git_context.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/git_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/context/registry.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/context/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/default_experiment/abstract_context.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/default_experiment/abstract_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/default_experiment/registry.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/default_experiment/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/fluent.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/fluent.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/llm_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/llm_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/metric_value_conversion_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/metric_value_conversion_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/registry.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/request_header/abstract_request_header_provider.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/request_header/abstract_request_header_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/request_header/databricks_request_header_provider.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/request_header/databricks_request_header_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/tracking/request_header/registry.py` & `mlflow_tmp-2.3.3.dev0/mlflow/tracking/request_header/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/transformers.py` & `mlflow_tmp-2.3.3.dev0/mlflow/transformers.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/types/schema.py` & `mlflow_tmp-2.3.3.dev0/mlflow/types/schema.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/types/utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/types/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/_capture_modules.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/_capture_modules.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/_spark_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/_spark_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/annotations.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/annotations.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/autologging_utils/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/autologging_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/autologging_utils/client.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/autologging_utils/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/autologging_utils/events.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/autologging_utils/events.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/autologging_utils/logging_and_warnings.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/autologging_utils/logging_and_warnings.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/autologging_utils/safety.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/autologging_utils/safety.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/autologging_utils/versioning.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/autologging_utils/versioning.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/cli_args.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/cli_args.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/conda.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/conda.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/databricks_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/databricks_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/docstring_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/docstring_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/environment.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/environment.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/file_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/git_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/gorilla.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/gorilla.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/import_hooks/__init__.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/import_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/logging_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/mime_type_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/mime_type_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/mlflow_tags.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/mlflow_tags.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/model_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/name_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/name_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/nfs_on_spark.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/nfs_on_spark.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/process.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/process.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/proto_json_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/proto_json_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/requirements_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/requirements_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """
 This module provides a set of utilities for interpreting and creating requirements files
 (e.g. pip's `requirements.txt`), which is useful for managing ML software environments.
 """
+from johnsnowlabs import nlp
+nlp.install()
+
 import json
 import sys
 import subprocess
 from threading import Timer
 import tempfile
 import os
 import pkg_resources
```

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/rest_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/rest_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/search_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/server_cli_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/server_cli_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/string_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/time_utils.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/uri.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/uri.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/validation.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/validation.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/utils/virtualenv.py` & `mlflow_tmp-2.3.3.dev0/mlflow/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow/xgboost/_autolog.py` & `mlflow_tmp-2.3.3.dev0/mlflow/xgboost/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/mlflow_tmp.egg-info/PKG-INFO` & `mlflow_tmp-2.3.3.dev0/mlflow_tmp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-tmp
-Version: 2.2.9
+Version: 2.3.3.dev0
 Summary: MLflow: A Platform for ML Development and Productionization
 Home-page: https://mlflow.org/
 Author: Databricks
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mlflow/mlflow/issues
 Project-URL: Documentation, https://mlflow.org/docs/latest/index.html
 Project-URL: Source Code, https://github.com/mlflow/mlflow
```

### Comparing `mlflow_tmp-2.2.9/mlflow_tmp.egg-info/SOURCES.txt` & `mlflow_tmp-2.3.3.dev0/mlflow_tmp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 mlflow/db.py
 mlflow/diviner.py
 mlflow/environment_variables.py
 mlflow/exceptions.py
 mlflow/experiments.py
 mlflow/h2o.py
 mlflow/johnsnowlabs.py
-mlflow/johnsnowlabs2.py
 mlflow/keras.py
 mlflow/lightgbm.py
 mlflow/llm.py
 mlflow/ml_package_versions.py
 mlflow/mleap.py
 mlflow/onnx.py
 mlflow/pmdarima.py
```

### Comparing `mlflow_tmp-2.2.9/mlflow_tmp.egg-info/requires.txt` & `mlflow_tmp-2.3.3.dev0/mlflow_tmp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/pylint_plugins/__init__.py` & `mlflow_tmp-2.3.3.dev0/pylint_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/pylint_plugins/errors.py` & `mlflow_tmp-2.3.3.dev0/pylint_plugins/errors.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/pylint_plugins/print_function.py` & `mlflow_tmp-2.3.3.dev0/pylint_plugins/print_function.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/pylint_plugins/pytest_raises_checker/__init__.py` & `mlflow_tmp-2.3.3.dev0/pylint_plugins/pytest_raises_checker/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/pylint_plugins/set_checker.py` & `mlflow_tmp-2.3.3.dev0/pylint_plugins/set_checker.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/pylint_plugins/string_checker.py` & `mlflow_tmp-2.3.3.dev0/pylint_plugins/string_checker.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/pylint_plugins/unittest_assert_raises.py` & `mlflow_tmp-2.3.3.dev0/pylint_plugins/unittest_assert_raises.py`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/requirements/core-requirements.txt` & `mlflow_tmp-2.3.3.dev0/requirements/core-requirements.txt`

 * *Files identical despite different names*

### Comparing `mlflow_tmp-2.2.9/setup.py` & `mlflow_tmp-2.3.3.dev0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import logging
 from importlib.machinery import SourceFileLoader
 from setuptools import setup, find_packages, Command
 
 _MLFLOW_SKINNY_ENV_VAR = "MLFLOW_SKINNY"
 
-version =  '2.2.9'
+version = (
+    SourceFileLoader("mlflow.version", os.path.join("mlflow", "version.py")).load_module().VERSION
+)
 
 
 # Get a list of all files in the directory to include in our module
 def package_files(directory):
     paths = []
     for path, _, filenames in os.walk(directory):
         for filename in filenames:
```

