# Comparing `tmp/konductor-0.0.2.tar.gz` & `tmp/konductor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konductor-0.0.2.tar", last modified: Fri Apr  7 02:16:34 2023, max compression
+gzip compressed data, was "konductor-0.0.3.tar", last modified: Sun May 21 04:53:33 2023, max compression
```

## Comparing `konductor-0.0.2.tar` & `konductor-0.0.3.tar`

### file list

```diff
@@ -1,128 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.360264 konductor-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-07 02:16:24.000000 konductor-0.0.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.344263 konductor-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.348264 konductor-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-07 02:16:24.000000 konductor-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-07 02:16:24.000000 konductor-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-07 02:16:24.000000 konductor-0.0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-07 02:16:24.000000 konductor-0.0.2/Dockerfile.pytorch
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-07 02:16:24.000000 konductor-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-04-07 02:16:34.360264 konductor-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-07 02:16:24.000000 konductor-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.352264 konductor-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:24.000000 konductor-0.0.2/docs/statistics.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:24.000000 konductor-0.0.2/docs/trainer.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:24.000000 konductor-0.0.2/docs/visualisation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.352264 konductor-0.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-07 02:16:24.000000 konductor-0.0.2/examples/kube-launch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-07 02:16:24.000000 konductor-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 02:16:34.360264 konductor-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-07 02:16:24.000000 konductor-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.348264 konductor-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.352264 konductor-0.0.2/src/konductor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.352264 konductor-0.0.2/src/konductor/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.352264 konductor-0.0.2/src/konductor/metadata/checkpointer/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/metadata/checkpointer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/metadata/checkpointer/_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/metadata/checkpointer/_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/metadata/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.352264 konductor-0.0.2/src/konductor/metadata/remotesync/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/metadata/remotesync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/metadata/remotesync/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/metadata/remotesync/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/metadata/remotesync/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.352264 konductor-0.0.2/src/konductor/metadata/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/metadata/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/metadata/statistics/perflogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/metadata/statistics/scalar_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/metadata/statistics/statistic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.352264 konductor-0.0.2/src/konductor/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.352264 konductor-0.0.2/src/konductor/modules/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.352264 konductor-0.0.2/src/konductor/modules/data/_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/data/_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/data/_pytorch/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/data/_pytorch/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/data/_pytorch/mnist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.352264 konductor-0.0.2/src/konductor/modules/data/_tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/data/_tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/data/_tensorflow/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/data/dali.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.356263 konductor-0.0.2/src/konductor/modules/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.356263 konductor-0.0.2/src/konductor/modules/losses/_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/losses/_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/losses/_pytorch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.356263 konductor-0.0.2/src/konductor/modules/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.356263 konductor-0.0.2/src/konductor/modules/models/_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/models/_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/models/_pytorch/encdec.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/models/_pytorch/torchvision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.356263 konductor-0.0.2/src/konductor/modules/models/_tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/models/_tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.356263 konductor-0.0.2/src/konductor/modules/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.356263 konductor-0.0.2/src/konductor/modules/optimizers/_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/optimizers/_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/optimizers/_pytorch/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/optimizers/_pytorch/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/optimizers/_pytorch/lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.356263 konductor-0.0.2/src/konductor/modules/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/modules/scheduler/_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.356263 konductor-0.0.2/src/konductor/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/trainer/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/trainer/pbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/trainer/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/trainer/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.356263 konductor-0.0.2/src/konductor/utilities/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.356263 konductor-0.0.2/src/konductor/utilities/comm/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/utilities/comm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/utilities/comm/_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/utilities/comm/_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/utilities/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/utilities/onnx_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.356263 konductor-0.0.2/src/konductor/webserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/webserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/webserver/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-07 02:16:24.000000 konductor-0.0.2/src/konductor/webserver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.352264 konductor-0.0.2/src/konductor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-04-07 02:16:34.000000 konductor-0.0.2/src/konductor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-07 02:16:34.000000 konductor-0.0.2/src/konductor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 02:16:34.000000 konductor-0.0.2/src/konductor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-07 02:16:34.000000 konductor-0.0.2/src/konductor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-07 02:16:34.000000 konductor-0.0.2/src/konductor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 02:16:34.000000 konductor-0.0.2/src/konductor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.360264 konductor-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/base.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.360264 konductor-0.0.2/tests/config_init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/config_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/config_init/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/init_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.360264 konductor-0.0.2/tests/remote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/remote/ssh_config
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/remote/test_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.360264 konductor-0.0.2/tests/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/statistics/test_checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/statistics/test_metamanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/statistics/test_perflogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/statistics/test_statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/statistics/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.360264 konductor-0.0.2/tests/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/trainer/test_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:34.360264 konductor-0.0.2/tests/webui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/webui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-07 02:16:24.000000 konductor-0.0.2/tests/webui/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-21 04:53:24.000000 konductor-0.0.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.805137 konductor-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-21 04:53:24.000000 konductor-0.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-21 04:53:24.000000 konductor-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-21 04:53:24.000000 konductor-0.0.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-21 04:53:24.000000 konductor-0.0.3/Dockerfile.pytorch
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-21 04:53:24.000000 konductor-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-05-21 04:53:33.817137 konductor-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-21 04:53:24.000000 konductor-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/docs/statistics.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/docs/trainer.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/docs/visualisation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-21 04:53:24.000000 konductor-0.0.3/examples/kube-launch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-21 04:53:24.000000 konductor-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 04:53:33.817137 konductor-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-21 04:53:24.000000 konductor-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.805137 konductor-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/src/konductor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/src/konductor/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/src/konductor/metadata/checkpointer/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/checkpointer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/checkpointer/_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/checkpointer/_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/src/konductor/metadata/remotesync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/remotesync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/remotesync/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/remotesync/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/remotesync/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/metadata/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/statistics/perflogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/statistics/scalar_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/statistics/statistic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/data/_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/_pytorch/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/_pytorch/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/_pytorch/mnist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/data/_tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/_tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/_tensorflow/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/dali.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/losses/_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/losses/_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/losses/_pytorch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/models/_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/models/_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/models/_pytorch/encdec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/models/_pytorch/torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/models/_tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/models/_tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/scheduler/_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/trainer/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/trainer/pbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/trainer/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/trainer/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/src/konductor/utilities/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/src/konductor/utilities/comm/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/utilities/comm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/utilities/comm/_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/utilities/comm/_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/utilities/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/utilities/onnx_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/src/konductor/webserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/src/konductor/webserver/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/pages/experiment_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/pages/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/pages/simple_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/src/konductor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-05-21 04:53:33.000000 konductor-0.0.3/src/konductor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-21 04:53:33.000000 konductor-0.0.3/src/konductor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 04:53:33.000000 konductor-0.0.3/src/konductor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-21 04:53:33.000000 konductor-0.0.3/src/konductor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-21 04:53:33.000000 konductor-0.0.3/src/konductor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 04:53:33.000000 konductor-0.0.3/src/konductor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/base.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/tests/config_init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/config_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/config_init/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/init_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/tests/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/remote/ssh_config
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/remote/test_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/tests/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/statistics/test_checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/statistics/test_metamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/statistics/test_perflogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/statistics/test_statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/statistics/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/tests/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/trainer/test_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/tests/webui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/webui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/webui/test_tree.py
```

### Comparing `konductor-0.0.2/.dockerignore` & `konductor-0.0.3/.dockerignore`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/.github/workflows/publish-to-pypi.yml` & `konductor-0.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/.gitignore` & `konductor-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/Dockerfile.pytorch` & `konductor-0.0.3/Dockerfile.pytorch`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 FROM nvidia/cuda:12.0.1-devel-ubuntu22.04
 
 # Basic Python Setup
 RUN apt update && apt install -y python3 python3-pip python3.10-venv git
 
 # Install Python Dependencies
 # Install PyTorch
-RUN pip3 install --index-url https://download.pytorch.org/whl/cu118 torch==2.0.0 torchvision==0.15.1 torchaudio==2.0.1 torchdata==0.6.0
+RUN pip3 install --index-url https://download.pytorch.org/whl/cu118 \
+    torch==2.0.0 torchvision==0.15.1 torchaudio==2.0.1 torchdata==0.6.0
 
 # Install DALI
-RUN pip3 install --extra-index-url https://developer.download.nvidia.com/compute/redist nvidia-dali-cuda120==1.23.0
+RUN pip3 install --extra-index-url https://developer.download.nvidia.com/compute/redist \
+    nvidia-dali-cuda120==1.23.0
 
 # Install other Python Packages
 RUN pip3 install \
     pyarrow==10.0.1 \
     paramiko==3.0.0 \
     minio==7.1.12 \
     pandas==1.3.5 \
```

### Comparing `konductor-0.0.2/LICENSE` & `konductor-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/PKG-INFO` & `konductor-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konductor
-Version: 0.0.2
+Version: 0.0.3
 Summary: Framework for training generic ml models
 Author-email: Bryce Ferenczi <frenzi@hotmail.com.au>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `konductor-0.0.2/README.rst` & `konductor-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/examples/kube-launch.yml` & `konductor-0.0.3/examples/kube-launch.yml`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/pyproject.toml` & `konductor-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
   "colorama",
   "pyyaml",
   "typer"
 ]
 
 [project.scripts]
 konduct-metadata = "konductor.utilities.metadata:app"
+konduct-review = "konductor.webserver.app:app.run"
 
 [project.optional-dependencies]
 REMOTE = [
   "paramiko",
   "minio"
 ]
 WEBUI = [
```

### Comparing `konductor-0.0.2/src/konductor/metadata/__init__.py` & `konductor-0.0.3/src/konductor/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/metadata/checkpointer/__init__.py` & `konductor-0.0.3/src/konductor/metadata/checkpointer/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/metadata/checkpointer/_pytorch.py` & `konductor-0.0.3/src/konductor/metadata/checkpointer/_pytorch.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/metadata/manager.py` & `konductor-0.0.3/src/konductor/trainer/trainer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-"""
+from abc import ABC, abstractmethod
+from dataclasses import dataclass
+from logging import getLogger
+from typing import Any, Callable, Dict, List, Sequence, TypeVar
 
-"""
+from konductor.metadata import MetadataManager
 
-from datetime import datetime, timedelta
-from dataclasses import dataclass
-from pathlib import Path
-from typing import Any, Dict
 
-from .checkpointer import Checkpointer
-from .statistics.perflogger import PerfLogger
-from .remotesync import _RemoteSyncrhoniser
-from ..utilities import comm
+@dataclass
+class TrainerModules:
+    """Holds all common training Modules"""
 
+    model: Any  # Model to train
+    criterion: List[Any]  # List of loss functions
+    optimizer: Any  # Optimizer
+    scheduler: Any  # Learning rate scheduler
+    trainloader: Sequence
+    valloader: Sequence
+
+    def __post_init__(self):
+        # Remove list wrapper if only one model/dataset etc
+        for field in self.__dataclass_fields__:
+            if field == "criterion":
+                continue  # don't unwrap criterion
+            obj = getattr(self, field)
+            if isinstance(obj, list) and len(obj) == 1:
+                setattr(self, field, obj[0])
 
-class _Timer:
-    """
-    Basic timer that keeps track of elapsed time from creation or reset
-    """
 
-    def __init__(self):
-        self.start_time = datetime.now()
+@dataclass
+class TrainerConfig:
+    # Function to run for monitoring issues with the value
+    # of the loss, does absolutely nothing by default
+    loss_monitor: Callable[[Dict[str, Any]], None] = lambda x: None
 
-    def elapsed(self):
-        """Returns the elapsed time since the timer was created or last reset"""
-        return datetime.now() - self.start_time
-
-    def reset(self):
-        """Resets the Timer"""
-        self.start_time = datetime.now()
+    pbar: Callable | None = None  # Enable Console Progress
+    optimizer_interval: int = 1  # interval to call optimizer.step()
 
 
-@dataclass
-class MetadataManager:
-    """Manages the lifecycle for statistics, checkpoints and any other relevant logs during training"""
+class TrainingError(RuntimeError):
+    """Exception raised by user in their training loop"""
 
-    perflog: PerfLogger
-    checkpointer: Checkpointer
-    checkpoint_interval: int = 0
-    remote_sync: _RemoteSyncrhoniser | None = None
-    sync_interval: timedelta = timedelta(hours=1)
-    epoch: int = 0
-    iteration: int = 0
-
-    def __post_init__(self) -> None:
-        self.perflog.set_iteration(0)
-        if self.remote_sync is not None:
-            self.remote_timer = _Timer()
-
-    @property
-    def workspace(self):
-        """Directory where data is stored"""
-        return self.checkpointer.rootdir
-
-    @workspace.setter
-    def workspace(self, path: Path):
-        assert path.exists(), f"New workspace folder does not exist: {path}"
-        self.checkpointer.rootdir = path
-        self.perflog.config.write_path = path
-
-    def resume(self) -> Dict[str, Any] | None:
-        """Resume if available, pull from remote if necessary"""
-        self._remote_resume()
-        extras = self.checkpointer.resume()
-        if extras is not None:
-            self.epoch = extras["epoch"]
-            self.iteration = extras["iteration"]
-            self.perflog.set_iteration(self.iteration)
-
-        return extras
-
-    def epoch_step(self) -> None:
-        """Step every epoch"""
-        self.epoch += 1
 
-        if self.checkpoint_interval > 0 and self.epoch % self.checkpoint_interval == 0:
-            ckpt_name = f"epoch_{self.epoch}.pt"
+class BaseTrainer(ABC):
+    """
+    Base class that various trainer types inherit from that
+    contains basic train loops which they can implement
+    """
+
+    modules = TrainerModules
+
+    def __init__(
+        self,
+        config: TrainerConfig,
+        modules: TrainerModules,
+        data_manager: MetadataManager,
+    ):
+        self.modules = modules
+        self.data_manager = data_manager
+        self._logger = getLogger(type(self).__name__)
+        self._config = config
+
+        extra = self.data_manager.resume()
+        if extra is not None and "epoch" in extra:
+            self._logger.info(f"Resuming from epoch {extra['epoch']}")
         else:
-            ckpt_name = "latest.pt"
+            self._logger.info(f"Unable to load checkpont, starting from scatch")
 
-        # Only save checkpoint on local rank zero
-        if comm.get_local_rank() == 0:
-            self.checkpointer.save(
-                ckpt_name, epoch=self.epoch, iteration=self.iteration
+        if config.pbar is not None:
+            self._train = config.pbar(self._train, total=len(self.modules.trainloader))
+            self._validate = config.pbar(
+                self._validate, total=len(self.modules.valloader)
             )
-        self.perflog.flush()
-        self._remote_push()
 
-    def iter_step(self) -> None:
-        """Step every iteration"""
-        self.iteration += 1
-        self.perflog.set_iteration(self.iteration)
-
-    def _remote_push(self) -> None:
-        """Push latest checkpoint and metadata to remote"""
-        if self.remote_sync is None:
-            return
-        comm.synchronize()  # Sync potential push
-        if self.remote_timer.elapsed() > self.sync_interval:
-            if comm.is_main_process():  # Main rank pushes all data (logs + weights)
-                self.remote_sync.push_all()
-            elif comm.get_local_rank() == 0:  # Rank0 of dist machines push logs
-                self.remote_sync.push_select([r".*\.parquet", "events.out.tfevents.*"])
-            self.remote_timer.reset()
-        comm.synchronize()
-
-    def _remote_resume(self) -> None:
-        """Pulls latest checkpoint and configuration files from remote"""
-        if self.remote_sync is None:
-            return
-        if comm.get_local_rank() == 0:
-            self.remote_sync.pull_select([r".*\.yaml", r".*\.yml", "latest.pt"])
-        comm.synchronize()
+    def run_epoch(self) -> None:
+        """Complete one epoch with training and validation epoch"""
+        self._logger.info(f"Training epoch {self.data_manager.epoch}")
+        self._train()
+        self._logger.info(f"Validating epoch {self.data_manager.epoch}")
+        self._validate()
+        self._logger.info(f"Epoch {self.data_manager.epoch} complete")
+        self.data_manager.epoch_step()
+
+    def data_transform(self, data: Any) -> Any:
+        """Apply any post motifications to data after loading
+        before being passed to [train|val]_step, no-op by default"""
+        return data
+
+    def training_exception(self, err: Exception, data: Any) -> None:
+        """This function is run when an runtime exception is thrown
+        during training iteration, useful for logging the state of the
+        model and the data used in the training iteration"""
+        raise err
+
+    @abstractmethod
+    def _accumulate_losses(self, losses: Dict[str, Any]) -> Any:
+        """Accumulate losses into single number hook, good idea to put a
+        grad scaler here if using amp"""
+
+    @abstractmethod
+    def _maybe_step_optimiser(self, iter_: int) -> None:
+        """Step optimizer if iteration is divisible by subbatch number"""
+
+    @abstractmethod
+    def _train(self) -> None:
+        """Train for one epoch over the dataset"""
+
+    @abstractmethod
+    def _validate(self) -> None:
+        """Validate one epoch over the dataset"""
+
+
+TrainerT = TypeVar("TrainerT", bound=BaseTrainer)
```

### Comparing `konductor-0.0.2/src/konductor/metadata/remotesync/__init__.py` & `konductor-0.0.3/src/konductor/metadata/remotesync/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/metadata/remotesync/_base.py` & `konductor-0.0.3/src/konductor/metadata/remotesync/_base.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/metadata/remotesync/minio.py` & `konductor-0.0.3/src/konductor/metadata/remotesync/minio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Synchronise workspace with minio s3 bucket
 """
 import os
 from dataclasses import dataclass
 from typing import Any, Dict
 from pathlib import Path
+from datetime import datetime
 
 from minio import Minio, S3Error
 
 from . import REGISTRY, RemoteConfig, ExperimentInitConfig
 from ._base import _RemoteSyncrhoniser
 from ...utilities.comm import is_main_process
 
@@ -74,63 +75,73 @@
         self.bucket_name = self._host_path.name if bucket_name is None else bucket_name
 
         self.logger.info("Checking bucket existance %s", self.bucket_name)
         if is_main_process() and not self.client.bucket_exists(self.bucket_name):
             self.logger.info("Creating bucket %s", self.bucket_name)
             self.client.make_bucket(self.bucket_name)
 
-    def _local_is_newer(self, filename: str) -> bool:
-        """Whether the file on the host was the last modified file (is newer).
-        Return false if the file doesn't exist on the host
-        Return true if the file doesn't exist on the remote"""
-        local = self._host_path / filename
-        if not local.exists():  # Not found on host
-            return False
+    def _remote_exists(self, filename: str) -> bool:
+        """Test if the file exists on the remote"""
         try:
-            remote_modified = self.client.stat_object(
-                self.bucket_name, filename
-            ).last_modified.timestamp()
-        except S3Error:  # Not found on remote
+            self.client.stat_object(self.bucket_name, filename)
+        except S3Error:
+            return False
+        else:
             return True
-        local_modified = local.stat().st_mtime
-        return local_modified > remote_modified
+
+    def _remote_ts(self, filename: str) -> float:
+        """Get remote last motified time"""
+        ts: datetime = self.client.stat_object(self.bucket_name, filename).last_modified
+        return ts.timestamp()
 
     def pull(self, filename: str, force: bool = False) -> None:
-        if self._local_is_newer(filename) and not force:
+        """Pull file from bucket, will not pull if local version is
+        newer unless forced to"""
+        local = self._host_path / filename
+
+        local_is_newer = local.exists() and local.stat().st_mtime >= self._remote_ts(
+            filename
+        )
+
+        if local_is_newer and not force:
             self.logger.info("Skipping file pull from remote: %s", filename)
             return
 
-        local = self._host_path / filename
         if local.exists():
             self.logger.info("Pulling file from remote and overwriting: %s", filename)
         else:
             self.logger.info("Pulling new file from remote: %s", filename)
 
         self.client.fget_object(self.bucket_name, filename, str(local))
 
         # Change local time to remote last modified
-        remote_modified = self.client.stat_object(
-            self.bucket_name, filename
-        ).last_modified.timestamp()
+        remote_modified = self._remote_ts(filename)
         os.utime(str(local), (remote_modified, remote_modified))
 
     def pull_all(self, force: bool = False) -> None:
         super().pull_all(force)
         for filename in self.file_list:
             self.pull(filename, force)
 
     def push(self, filename: str, force: bool = False) -> None:
-        if not self._local_is_newer(filename) and not force:
+        """Push file to bucket, will not push to bucket if it
+        has a newer version unless forced to"""
+        local = self._host_path / filename
+
+        remote_is_newer = (
+            self._remote_exists(filename)
+            and self._remote_ts(filename) >= local.stat().st_mtime
+        )
+
+        if remote_is_newer and not force:
             self.logger.info("Skipping file push to remote: %s", filename)
             return
 
         self.logger.info("Pushing file to remote: %s", filename)
-        self.client.fput_object(
-            self.bucket_name, filename, str(self._host_path / filename)
-        )
+        self.client.fput_object(self.bucket_name, filename, str(local))
 
         # Doesn't seem like I can change last modified on object?
         # local_modified = (self._host_path / filename).stat().st_mtime
 
     def push_all(self, force: bool = False) -> None:
         super().push_all(force)
         for filename in self.file_list:
```

### Comparing `konductor-0.0.2/src/konductor/metadata/remotesync/ssh.py` & `konductor-0.0.3/src/konductor/metadata/remotesync/ssh.py`

 * *Files 12% similar despite different names*

```diff
@@ -136,28 +136,24 @@
 
         if not self.remote_existance() and is_main_process():
             self.logger.info("Creating directory on remote %s", remote_path)
             _, _, stderr = self._session.exec_command(f"mkdir -p {remote_path}")
             for line in stderr:
                 self.logger.error(line.strip("\n"))
 
-    @staticmethod
-    def _local_is_newer(local: Path, remote: Path, sftp: paramiko.SFTPClient) -> bool:
-        """Whether the file on the host was the last modified file (is newer).
-        Return false if the file doesn't exist on the host
-        Return true if the file doesn't exist on the remote"""
-        if not local.exists():  # Not found on host
-            return False
+    def _remote_exists(self, filename: str, sftp: paramiko.SFTPClient) -> bool:
+        """Test if the file exists on the remote by stat'ing it"""
         try:
-            remote_modified = sftp.stat(str(remote)).st_mtime
-            assert remote_modified is not None
-        except FileNotFoundError:  # Not found on remote
-            return True
-        local_modified = local.stat().st_mtime
-        return local_modified > remote_modified
+            sftp.stat(str(self._remote_path / filename))
+        except FileNotFoundError:
+            exists = False
+        else:
+            exists = True
+
+        return exists
 
     def _get_local_remote(self, filename: str):
         """Return local and remote path pair"""
         return self._host_path / filename, self._remote_path / filename
 
     def _match_checksum(self, host: Path, remote: Path) -> bool:
         """md5 checksum of host and remote files match"""
@@ -172,18 +168,25 @@
     @retry_connection
     def push(
         self,
         filename: str,
         force: bool = False,
         sftp: paramiko.SFTPClient | None = None,
     ) -> None:
+        """scp file from local to the remote, will not do this if
+        the remote has a newer version unless forced"""
         local, remote = self._get_local_remote(filename)
         sftp_ = self._session.open_sftp() if sftp is None else sftp
 
-        if not self._local_is_newer(local, remote, sftp_) and not force:
+        remote_is_newer = (
+            self._remote_exists(remote.name, sftp_)
+            and sftp_.stat(str(remote)).st_mtime >= local.stat().st_mtime
+        )
+
+        if remote_is_newer and not force:
             self.logger.info("Skipping file push to remote: %s", filename)
             return
 
         # Copy local to the remote
         self.logger.info("Pushing file to remote: %s", filename)
         tmp_remote = remote.with_suffix(".tmp")
         sftp_.put(str(local), str(tmp_remote))
@@ -218,18 +221,24 @@
     @retry_connection
     def pull(
         self,
         filename: str,
         force: bool = False,
         sftp: paramiko.SFTPClient | None = None,
     ) -> None:
+        """Pull file from the remote to local, will not pull
+        if the local copy is newer unless forced to"""
         local, remote = self._get_local_remote(filename)
         sftp_ = self._session.open_sftp() if sftp is None else sftp
 
-        if self._local_is_newer(local, remote, sftp_) and not force:
+        local_is_newer = (
+            local.exists() and local.stat().st_mtime >= sftp_.stat(str(remote)).st_mtime
+        )
+
+        if local_is_newer and not force:
             self.logger.info("Skipping file pull from remote: %s", filename)
             return
 
         self.logger.info(
             "Pulling file from remote and overwriting existing: %s"
             if local.exists()
             else "Pulling new file from remote: %s",
```

### Comparing `konductor-0.0.2/src/konductor/metadata/statistics/perflogger.py` & `konductor-0.0.3/src/konductor/metadata/statistics/perflogger.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/metadata/statistics/scalar_dict.py` & `konductor-0.0.3/src/konductor/metadata/statistics/scalar_dict.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/metadata/statistics/statistic.py` & `konductor-0.0.3/src/konductor/metadata/statistics/statistic.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/__init__.py` & `konductor-0.0.3/src/konductor/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/data/__init__.py` & `konductor-0.0.3/src/konductor/modules/data/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/data/_pytorch/cityscapes.py` & `konductor-0.0.3/src/konductor/modules/data/_pytorch/cityscapes.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/data/_pytorch/dataloader.py` & `konductor-0.0.3/src/konductor/modules/data/_pytorch/dataloader.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/data/dali.py` & `konductor-0.0.3/src/konductor/modules/data/dali.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/init.py` & `konductor-0.0.3/src/konductor/modules/init.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,29 +75,31 @@
 
 @dataclass
 class ExperimentInitConfig:
     """
     Configuration for all the modules for training
     """
 
-    work_dir: Path
+    brief: str  # Short description for experiment
+    work_dir: Path  # Directory for saving everything
     model: List[ModelInitConfig]
     data: List[DatasetInitConfig]
     criterion: List[ModuleInitConfig]
     remote_sync: ModuleInitConfig | None = None
     logger_kwargs: Dict[str, Any] = field(default_factory=dict)
 
     @classmethod
     def from_yaml(cls, parsed_dict: Dict[str, Any]):
         if "remote_sync" in parsed_dict:
             remote_sync = ModuleInitConfig(**parsed_dict["remote_sync"])
         else:
             remote_sync = None
 
         return cls(
+            brief=parsed_dict.get("brief", ""),
             model=[ModelInitConfig.from_yaml(cfg) for cfg in parsed_dict["model"]],
             data=[DatasetInitConfig.from_yaml(cfg) for cfg in parsed_dict["dataset"]],
             criterion=[
                 ModuleInitConfig(**crit_dict) for crit_dict in parsed_dict["criterion"]
             ],
             work_dir=parsed_dict["work_dir"],
             remote_sync=remote_sync,
```

### Comparing `konductor-0.0.2/src/konductor/modules/losses/__init__.py` & `konductor-0.0.3/src/konductor/modules/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/losses/_pytorch/base.py` & `konductor-0.0.3/src/konductor/modules/losses/_pytorch/base.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/models/__init__.py` & `konductor-0.0.3/src/konductor/modules/models/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/models/_pytorch/__init__.py` & `konductor-0.0.3/src/konductor/modules/models/_pytorch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         if self.pretrained is not None:
             ckpt_path = (
                 Path(os.environ.get("PRETRAINED_ROOT", Path.cwd())) / self.pretrained
             )
             logger = getLogger()
             logger.info(f"Loading pretrained checkpoint from {ckpt_path}")
-            checkpoint = load(ckpt_path)
+            checkpoint = load(ckpt_path, map_location="cpu")
             if "model" in checkpoint:
                 missing, unused = model.load_state_dict(
                     checkpoint["model"], strict=False
                 )
             else:
                 # Assume direct loading
                 missing, unused = model.load_state_dict(checkpoint, strict=False)
```

### Comparing `konductor-0.0.2/src/konductor/modules/models/_pytorch/encdec.py` & `konductor-0.0.3/src/konductor/modules/models/_pytorch/encdec.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/models/_pytorch/torchvision.py` & `konductor-0.0.3/src/konductor/modules/models/_pytorch/torchvision.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/optimizers/__init__.py` & `konductor-0.0.3/src/konductor/modules/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/optimizers/_pytorch/base.py` & `konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/base.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/optimizers/_pytorch/common.py` & `konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/common.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/optimizers/_pytorch/lamb.py` & `konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/lamb.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/registry.py` & `konductor-0.0.3/src/konductor/modules/registry.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/scheduler/__init__.py` & `konductor-0.0.3/src/konductor/modules/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/modules/scheduler/_pytorch.py` & `konductor-0.0.3/src/konductor/modules/scheduler/_pytorch.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/trainer/init.py` & `konductor-0.0.3/src/konductor/trainer/init.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ 
 Initialisation methods for Training/Validation etc.
 """
 import argparse
-from typing import Dict, Type
+from typing import Any, Dict, Type
 from pathlib import Path
 import yaml
 import hashlib
+from io import StringIO
 
 from .trainer import TrainerConfig, TrainerModules, TrainerT
 from ..modules import (
     get_model,
     get_training_model,
     get_criterion,
     get_optimizer,
@@ -52,45 +53,45 @@
     parser.add_argument(
         "-s",
         "--workspace",
         type=Path,
         default=Path.cwd() / "checkpoints",
         help="The base directory where checkpoints are stored",
     )
-
-    # Remote configuration
     parser.add_argument(
-        "-r",
-        "--remote",
-        type=Path,
-        required=False,
-        help="Path to configuration file for remote synchronisation",
+        "--workers", type=int, default=0, help="Number of dataloader workers"
     )
 
 
 def get_training_parser() -> argparse.ArgumentParser:
     """Parses arguments used for training"""
     parser = argparse.ArgumentParser("Training Script")
     parser_add_common_args(parser)
+
     parser.add_argument(
         "-k",
         "--extra_checkpoints",
         type=float,
         default=None,
         help="Save intermediate checkpoints at defined time interval (sec)",
     )
     parser.add_argument(
-        "-w",
-        "--workers",
-        type=int,
-        default=0,
-        help="Number of dataloader workers",
+        "-e", "--epochs", type=int, default=1, help="Max epoch to train to"
     )
     parser.add_argument(
-        "-e", "--epochs", type=int, default=1, help="Max epoch to train to"
+        "--brief", type=str, default="", help="Brief description to give experiment"
+    )
+
+    # Remote configuration
+    parser.add_argument(
+        "-r",
+        "--remote",
+        type=Path,
+        required=False,
+        help="Path to configuration file for remote synchronisation",
     )
 
     # Configruation for torch.distributed training
     parser.add_argument("-g", "--gpu", type=int, required=False, default=0)
     parser.add_argument("-b", "--backend", type=str, required=False, default="nccl")
     parser.add_argument(
         "-d",
@@ -114,14 +115,25 @@
         action="store_true",
         help="Enable Tensorboard Profiler (Runs only once if trace.json is not present)",
     )
 
     return parser
 
 
+def hash_from_config(config: Dict[str, Any]) -> str:
+    """Return hashed version of the config file loaded as a dict
+    This simulates writing config to a file which prevents issues
+    with changing orders and formatting between the written config
+    and original config"""
+    ss = StringIO()
+    yaml.safe_dump(config, ss)
+    ss.seek(0)
+    return hashlib.md5(ss.read().encode("utf-8")).hexdigest()
+
+
 def get_experiment_cfg(
     workspace: Path, config_file: Path | None = None, run_hash: str | None = None
 ) -> ExperimentInitConfig:
     """
     Returns a model config and its savepath given a list of directorys to search for the model.\n
     Uses argparse for seraching for the model or config argument.
     """
@@ -131,15 +143,15 @@
         with open(exp_path / "train_config.yml", "r", encoding="utf-8") as conf_f:
             exp_cfg = yaml.safe_load(conf_f)
 
     elif config_file is not None:
         with open(config_file, "r", encoding="utf-8") as conf_f:
             exp_cfg = yaml.safe_load(conf_f)
 
-        train_hash = hashlib.md5(str(exp_cfg).encode("utf-8")).hexdigest()
+        train_hash = hash_from_config(exp_cfg)
         exp_path: Path = workspace / train_hash
 
         if not exp_path.exists():
             print(f"Creating experiment directory {exp_path}")
             exp_path.mkdir(parents=True)
         else:
             print(f"Using experiment directory {exp_path}")
@@ -170,14 +182,15 @@
     ]
     train_loaders = [get_dataloader(cfg, "train") for cfg in dataset_cfgs]
     val_loaders = [get_dataloader(cfg, "val") for cfg in dataset_cfgs]
 
     modules = [
         get_training_model(exp_config, idx) for idx in range(len(exp_config.model))
     ]
+    # Unpack tuple into each category
     models = [m[0] for m in modules]
     optims = [m[1] for m in modules]
     scheds = [m[2] for m in modules]
 
     criterion = get_criterion(exp_config)
 
     return train_module_cls(
@@ -207,55 +220,62 @@
 
     remote_sync = (
         None
         if exp_config.remote_sync is None
         else get_remote_config(exp_config).get_instance()
     )
 
-    return get_metadata_manager(
+    manager = get_metadata_manager(
         log_config,
         remote_sync=remote_sync,
         model=train_modules.model,
         optim=train_modules.optimizer,
         scheduler=train_modules.scheduler,
     )
 
+    manager.write_brief(exp_config.brief)
+
+    return manager
+
 
 def cli_init_config(cli_args: argparse.Namespace):
     """
     Parse cli args to generate the experiment configuration
     """
     exp_config = get_experiment_cfg(
         cli_args.workspace, cli_args.config_file, cli_args.run_hash
     )
 
-    if cli_args.remote:
+    if hasattr(cli_args, "brief"):
+        exp_config.brief = cli_args.brief  # Add brief to experiment cfg
+
+    if getattr(cli_args, "remote", False):
         with open(cli_args.remote, "r", encoding="utf-8") as f:
             cfg = yaml.safe_load(f)
         exp_config.remote_sync = ModuleInitConfig(**cfg)
 
-    if hasattr(cli_args, "workers"):
-        for data in exp_config.data:  # Divide workers evenly among datasets
-            data.val_loader.args["workers"] = cli_args.workers // len(exp_config.data)
-            data.train_loader.args["workers"] = cli_args.workers // len(exp_config.data)
+    for data in exp_config.data:  # Divide workers evenly among datasets
+        data.val_loader.args["workers"] = cli_args.workers // len(exp_config.data)
+        data.train_loader.args["workers"] = cli_args.workers // len(exp_config.data)
 
     return exp_config
 
 
 def init_training(
     exp_config: ExperimentInitConfig,
     trainer_cls: Type[TrainerT],
     trainer_config: TrainerConfig,
     statistics: Dict[str, type[Statistic]],
     train_module_cls: Type[TrainerModules] = TrainerModules,
     perf_log_cfg_cls: Type[PerfLoggerConfig] = PerfLoggerConfig,
 ) -> TrainerT:
     """Initialize training manager class + distributed setup"""
-    comm.initialize()
+    comm.initialize()  # Init distributed if required
 
+    # Making the big assumption that step interval is same for all optimizers
     trainer_config.optimizer_interval = exp_config.model[0].optimizer.args.pop(
         "step_interval", 1
     )
 
     train_modules = init_training_modules(exp_config, train_module_cls)
     data_manager = init_data_manager(
         exp_config, train_modules, statistics, perf_log_cfg_cls
```

### Comparing `konductor-0.0.2/src/konductor/trainer/pbar.py` & `konductor-0.0.3/src/konductor/trainer/pbar.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/trainer/profiler.py` & `konductor-0.0.3/src/konductor/trainer/profiler.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/trainer/pytorch.py` & `konductor-0.0.3/src/konductor/trainer/pytorch.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/utilities/comm/__init__.py` & `konductor-0.0.3/src/konductor/utilities/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/utilities/comm/_pytorch.py` & `konductor-0.0.3/src/konductor/utilities/comm/_pytorch.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/utilities/comm/_tensorflow.py` & `konductor-0.0.3/src/konductor/utilities/comm/_tensorflow.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/utilities/onnx_export.py` & `konductor-0.0.3/src/konductor/utilities/onnx_export.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/src/konductor/webserver/app.py` & `konductor-0.0.3/src/konductor/webserver/pages/experiment_summary.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,139 +1,155 @@
-# Run this app with `python app.py` and
-# visit http://127.0.0.1:8050/ in your web browser.
-
-from argparse import ArgumentParser
 from pathlib import Path
 from typing import List
 
+
 import pandas as pd
-from dash import Dash, html, dcc, Input, Output
+import dash
+from dash import html, dcc, Input, Output, callback
 from dash.exceptions import PreventUpdate
 import dash_bootstrap_components as dbc
 import plotly.graph_objects as go
 
-try:
-    from .utils import Experiment, OptionTree
-except ImportError:
-    from utils import Experiment, OptionTree
-
-app = Dash(__name__, external_stylesheets=[dbc.themes.BOOTSTRAP])
-
-
-def get_experiments(root_dir: Path) -> List[Experiment]:
-    experiments = []
-    for p in root_dir.iterdir():
-        e = Experiment.from_path(p)
-        if e is not None:
-            experiments.append(e)
-    return experiments
-
-
-def get_option_tree(exp: List[Experiment]) -> OptionTree:
-    tree = OptionTree.make_root()
-    for s in list(s for e in exp for s in e.stats):
-        tree.add(s)
-    return tree
-
+from konductor.webserver.utils import (
+    fill_experiments,
+    fill_option_tree,
+    OptionTree,
+    Experiment,
+)
 
-parser = ArgumentParser()
-parser.add_argument("--root", type=Path, default=Path.cwd())
-args = parser.parse_args()
+dash.register_page(__name__, path="/experiment-summary")
 
-experiments = get_experiments(args.root)
-stat_tree = get_option_tree(experiments)
-exp_hashes = list(e.name for e in experiments)
+EXPERIMENTS: List[Experiment] = []
+OPTION_TREE = OptionTree.make_root()
 
-app.layout = html.Div(
+layout = html.Div(
     children=[
-        html.H1(children="Konduct-Review"),
+        html.H2(children="Experiment Summary"),
+        html.Div(dcc.Dropdown(id="summary-exp-select")),
+        html.Div(id="summary-exp-hash"),
         dbc.Row(
             [
                 dbc.Col(
                     [
-                        dbc.ModalTitle("Split"),
-                        dcc.Dropdown(stat_tree.keys, id="stat-split"),
+                        html.H4("Group", style={"text-align": "center"}),
+                        dcc.Dropdown(id="summary-stat-group"),
+                    ]
+                ),
+                dbc.Col(
+                    [
+                        dbc.ModalTitle("Statistic", style={"text-align": "center"}),
+                        dcc.Dropdown(id="summary-stat-name"),
                     ]
                 ),
-                dbc.Col([dbc.ModalTitle("Group"), dcc.Dropdown(id="stat-group")]),
-                dbc.Col([dbc.ModalTitle("Statistic"), dcc.Dropdown(id="stat-name")]),
             ],
         ),
+        dbc.Row(dcc.Graph(id="summary-graph")),
         dbc.Row(
             [
-                dbc.ModalTitle("Select Runs"),
-                html.Div(dcc.Dropdown(exp_hashes, id="enable-exp", multi=True)),
+                dbc.Col(
+                    [
+                        html.H4("Metadata", style={"text-align": "center"}),
+                        dcc.Textarea(
+                            id="summary-metadata-txt",
+                            readOnly=True,
+                            style={"width": "100%", "height": 300},
+                        ),
+                    ]
+                ),
+                dbc.Col(
+                    [
+                        html.H4("Training Config", style={"text-align": "center"}),
+                        dcc.Textarea(
+                            id="summary-traincfg-txt",
+                            readOnly=True,
+                            style={"width": "100%", "height": 300},
+                        ),
+                    ]
+                ),
             ]
         ),
-        dcc.Graph(id="line-graph"),
     ]
 )
 
 
-@app.callback(
-    Output("stat-group", "options"),
-    Output("stat-group", "value"),
-    Input("stat-split", "value"),
-)
-def update_stat_group(split: str):
-    if not split:
-        return [], None
-    return stat_tree[split].keys, None  # Deselect
-
-
-@app.callback(
-    Output("stat-name", "options"),
-    Output("stat-name", "value"),
-    Input("stat-split", "value"),
-    Input("stat-group", "value"),
-)
-def update_stat_name(split: str, group: str):
-    if split and group:
-        search_value = "/".join([split, group])
-        return stat_tree[search_value].keys, None
-    return [], None  # Deselect and clear
-
-
-@app.callback(
-    Output("enable-exp", "options"),
-    Input("stat-split", "value"),
-    Input("stat-group", "value"),
-    Input("stat-name", "value"),
-)
-def filter_experiments(split: str, group: str, name: str):
-    if split and group and name:
-        search = "/".join([split, group, name])
-        return [e.name for e in experiments if search in e.stats]
-    raise PreventUpdate  # Don't deselect/mess with things
-
-
-@app.callback(
-    Output("line-graph", "figure"),
-    Input("enable-exp", "value"),
-    Input("stat-split", "value"),
-    Input("stat-group", "value"),
-    Input("stat-name", "value"),
+@callback(
+    Output("summary-exp-select", "options"),
+    Input("root-dir", "data"),
 )
-def update_graph(exp_list: List[str], split: str, group: str, name: str):
-    if not (split and group and name and exp_list):
-        raise PreventUpdate
+def init_exp(root_dir: str):
+    if len(EXPERIMENTS) == 0:
+        fill_experiments(Path(root_dir), EXPERIMENTS)
+    return [e.name for e in EXPERIMENTS]
 
-    stat_path = "/".join([split, group, name])
-    exps: List[pd.Series] = [
-        e[stat_path].rename(e.name).sort_index()
-        for e in experiments
-        if e.name in exp_list and stat_path in e
-    ]
-    if len(exps) == 0:
+
+@callback(
+    Output("summary-stat-group", "options"),
+    Output("summary-stat-group", "value"),
+    Output("summary-traincfg-txt", "value"),
+    Output("summary-metadata-txt", "value"),
+    Output("summary-exp-hash", "children"),
+    Input("summary-exp-select", "value"),
+)
+def selected_experiment(exp_name: str):
+    """Return new statistic group and deselect previous value,
+    also initialize the training cfg and metadata text boxes"""
+    if not exp_name:
+        return [], None, "", "", ""
+    OPTION_TREE.children = {}
+
+    exp = next(e for e in EXPERIMENTS if e.name == exp_name)
+    fill_option_tree([exp], OPTION_TREE)
+
+    stat_groups = set()  # Gather all groups
+    for split in OPTION_TREE.keys:
+        stat_groups.update(OPTION_TREE[split].keys)
+
+    cfg_txt = (exp.root / "train_config.yml").read_text()
+    meta_txt = (exp.root / "metadata.yaml").read_text()
+
+    return sorted(stat_groups), None, cfg_txt, meta_txt, exp.root.name
+
+
+@callback(
+    Output("summary-stat-name", "options"),
+    Output("summary-stat-name", "value"),
+    Input("summary-stat-group", "value"),
+)
+def update_stat_name(group: str):
+    if not group:
+        return [], None  # Deselect and clear
+
+    stat_names = set()  # Gather all groups
+    for split in OPTION_TREE.keys:
+        stat_path = f"{split}/{group}"
+        if stat_path in OPTION_TREE:
+            stat_names.update(OPTION_TREE[stat_path].keys)
+
+    return sorted(stat_names), None
+
+
+@callback(
+    Output("summary-graph", "figure"),
+    Input("summary-exp-select", "value"),
+    Input("summary-stat-group", "value"),
+    Input("summary-stat-name", "value"),
+)
+def update_graph(exp_name: str, group: str, name: str):
+    if not (exp_name and group and name):
         raise PreventUpdate
 
+    exp = next(e for e in EXPERIMENTS if e.name == exp_name)
+
+    data: List[pd.Series] = []
+    for split in OPTION_TREE.keys:
+        stat_path = "/".join([split, group, name])
+        if stat_path not in exp:
+            continue
+        data.append(exp[stat_path].rename(split).sort_index())
+
     fig = go.Figure()
-    for exp in exps:
+    for sample in data:
         fig.add_trace(
-            go.Scatter(x=exp.index, y=exp.values, mode="lines", name=exp.name)
+            go.Scatter(x=sample.index, y=sample.values, mode="lines", name=sample.name)
         )
 
     return fig
-
-
-if __name__ == "__main__":
-    app.run(debug=True)
```

### Comparing `konductor-0.0.2/src/konductor/webserver/utils.py` & `konductor-0.0.3/src/konductor/webserver/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from pathlib import Path
 from dataclasses import dataclass
+from datetime import datetime
 from collections import deque
 import re
 from typing import List, Deque
 
+import yaml
 import pandas as pd
 from pyarrow import parquet as pq
 from konductor.utilities.metadata import _PQ_REDUCED_RE
 
+from logging import debug
+
 
 @dataclass
 class Experiment:
     root: Path
+    name: str
+    last_train: datetime
     stats: List[str]
 
     @staticmethod
     def get_keys(file: Path) -> List[str]:
         """Get statistics keys from file"""
         keys = pq.read_metadata(file)
         keys = [k for k in keys.schema.names if k not in {"timestamp", "iteration"}]
@@ -23,36 +29,53 @@
 
     @classmethod
     def from_path(cls, root: Path):
         assert not root.is_file(), "Experiment root should be a folder"
         log_files = [f for f in root.iterdir() if re.match(_PQ_REDUCED_RE, f.name)]
 
         if len(log_files) == 0:
-            print(f"Skipping {root.name}")
+            debug(f"Skipping {root.name}")
             return None
 
         keys: List[str] = []
         for log_file in log_files:
             split, name = log_file.stem.split("_")[:2]
             keys.extend([f"{split}/{name}/{k}" for k in Experiment.get_keys(log_file)])
 
-        return cls(root, keys)
-
-    @property
-    def name(self):
-        return self.root.name
-
-    def __getitem__(self, stat: str) -> pd.Series:
-        """Read from disk {split}/{statistic}/{key} and average by iteration for plotting"""
-        split, name, key = stat.split("/")
-        filename = self.root / f"{split}_{name}.parquet"
+        try:
+            with open(root / "metadata.yaml", "r", encoding="utf-8") as f:
+                mdata = yaml.safe_load(f)
+            name: str = mdata.get("brief", mdata["notes"][:30])
+            ts = mdata.get("train_last", datetime(1, 1, 1))
+        except FileNotFoundError:
+            name = ""
+            ts = datetime(1, 1, 1)
+
+        if len(name) == 0:  # rename to exp hash if brief/note empty
+            name = root.name
+
+        return cls(root, name, ts, keys)
+
+    def _get_group_data(self, split: str, group: str) -> pd.DataFrame:
+        """Return all statistics within a group with averaged iteration"""
+        filename = self.root / f"{split}_{group}.parquet"
         data: pd.DataFrame = pq.read_table(
             filename, pre_buffer=False, memory_map=True, use_threads=True
         ).to_pandas()
-        return data.groupby("iteration")[key].mean()
+        return data.groupby("iteration").mean()
+
+    def __getitem__(self, stat: str) -> pd.Series:
+        """Read from disk {split}/{statistic}/{key} and return data by iteration"""
+        split, name, key = stat.split("/")
+        return self._get_group_data(split, name)[key]
+
+    def get_group_latest(self, split: str, group: str) -> pd.DataFrame:
+        """Read all statistics within a group and get data from latest iteration"""
+        data = self._get_group_data(split, group)
+        return data.query("iteration == iteration.max()")
 
     def __contains__(self, stat: str) -> bool:
         return stat in self.stats
 
 
 class OptionTree:
     """Option tree enables creating recursive chains of options
@@ -92,14 +115,23 @@
         """Helper class that continues to pop items off the queue
         until we reach the depth of the node we're after"""
         if len(option) == 0:
             return self
         nxt_key = option.popleft()
         return self.children[nxt_key]._get_helper(option)
 
+    def __contains__(self, option: str) -> bool:
+        """Check if option path exists in tree"""
+        try:
+            self.__getitem__(option)
+        except KeyError:
+            return False
+        else:
+            return True
+
     def __getitem__(self, option: str):
         """Returns node of requested option string foo/bar/baz"""
         return self._get_helper(deque(option.split("/")))
 
     def add(self, option: str):
         """Add a new node to the tree"""
         self._add_helper(deque(option.split("/")))
@@ -111,7 +143,25 @@
             return
         nxt_key = option[0]
         if nxt_key in self.keys:
             option.popleft()
             self.children[nxt_key]._add_helper(option)
         else:
             self.children[nxt_key] = OptionTree(option)
+
+
+def fill_experiments(root_dir: Path, experiments: List[Experiment]):
+    """Add experiments in root directory to experiment folder"""
+    for p in root_dir.iterdir():
+        if not p.is_dir():
+            continue
+        e = Experiment.from_path(p)
+        if e is not None:
+            experiments.append(e)
+
+    experiments.sort(key=lambda e: e.last_train)
+
+
+def fill_option_tree(exp: List[Experiment], tree: OptionTree):
+    """Add experiments to the option tree"""
+    for s in list(s for e in exp for s in e.stats):
+        tree.add(s)
```

### Comparing `konductor-0.0.2/src/konductor.egg-info/PKG-INFO` & `konductor-0.0.3/src/konductor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konductor
-Version: 0.0.2
+Version: 0.0.3
 Summary: Framework for training generic ml models
 Author-email: Bryce Ferenczi <frenzi@hotmail.com.au>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `konductor-0.0.2/src/konductor.egg-info/SOURCES.txt` & `konductor-0.0.3/src/konductor.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -64,17 +64,22 @@
 src/konductor/trainer/pytorch.py
 src/konductor/trainer/trainer.py
 src/konductor/utilities/metadata.py
 src/konductor/utilities/onnx_export.py
 src/konductor/utilities/comm/__init__.py
 src/konductor/utilities/comm/_pytorch.py
 src/konductor/utilities/comm/_tensorflow.py
+src/konductor/webserver/README.md
 src/konductor/webserver/__init__.py
 src/konductor/webserver/app.py
 src/konductor/webserver/utils.py
+src/konductor/webserver/pages/__init__.py
+src/konductor/webserver/pages/experiment_summary.py
+src/konductor/webserver/pages/home.py
+src/konductor/webserver/pages/simple_comparison.py
 tests/__init__.py
 tests/base.yml
 tests/init_config.py
 tests/test_registry.py
 tests/config_init/__init__.py
 tests/config_init/test_pytorch.py
 tests/remote/__init__.py
```

### Comparing `konductor-0.0.2/tests/config_init/test_pytorch.py` & `konductor-0.0.3/tests/config_init/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/tests/remote/test_remote.py` & `konductor-0.0.3/tests/remote/test_remote.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/tests/statistics/test_checkpointer.py` & `konductor-0.0.3/tests/statistics/test_checkpointer.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/tests/statistics/test_metamanager.py` & `konductor-0.0.3/tests/statistics/test_metamanager.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/tests/statistics/test_perflogger.py` & `konductor-0.0.3/tests/statistics/test_perflogger.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/tests/statistics/test_statistic.py` & `konductor-0.0.3/tests/statistics/test_statistic.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/tests/test_registry.py` & `konductor-0.0.3/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/tests/trainer/test_pytorch.py` & `konductor-0.0.3/tests/trainer/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.2/tests/webui/test_tree.py` & `konductor-0.0.3/tests/webui/test_tree.py`

 * *Files identical despite different names*

