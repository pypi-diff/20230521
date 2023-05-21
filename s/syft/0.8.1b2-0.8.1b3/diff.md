# Comparing `tmp/syft-0.8.1b2.tar.gz` & `tmp/syft-0.8.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.1b2.tar", last modified: Sun May 14 12:45:01 2023, max compression
+gzip compressed data, was "syft-0.8.1b3.tar", last modified: Sun May 21 12:44:53 2023, max compression
```

## Comparing `syft-0.8.1b2.tar` & `syft-0.8.1b3.tar`

### file list

```diff
@@ -1,178 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:01.022682 syft-0.8.1b2/
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-05-14 12:42:01.000000 syft-0.8.1b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-14 12:42:01.000000 syft-0.8.1b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-14 12:45:01.022682 syft-0.8.1b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-14 12:42:01.000000 syft-0.8.1b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-14 12:42:01.000000 syft-0.8.1b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-14 12:45:01.026682 syft-0.8.1b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-14 12:42:01.000000 syft-0.8.1b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.922682 syft-0.8.1b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.938682 syft-0.8.1b2/src/syft/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-14 12:42:19.000000 syft-0.8.1b2/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-14 12:42:19.000000 syft-0.8.1b2/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.942682 syft-0.8.1b2/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.946682 syft-0.8.1b2/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24303 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.950682 syft-0.8.1b2/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.954682 syft-0.8.1b2/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15930 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.962682 syft-0.8.1b2/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    27103 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.970682 syft-0.8.1b2/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/serde/third_party.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.970682 syft-0.8.1b2/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.978682 syft-0.8.1b2/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    46598 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27045 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.982682 syft-0.8.1b2/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    21458 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.986682 syft-0.8.1b2/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.990682 syft-0.8.1b2/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.990682 syft-0.8.1b2/src/syft/service/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/message/message_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/message/message_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/message/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.994682 syft-0.8.1b2/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/metadata/metadata_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.994682 syft-0.8.1b2/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (123)    15290 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/network/network_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.994682 syft-0.8.1b2/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.998682 syft-0.8.1b2/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22709 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.998682 syft-0.8.1b2/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/queue/queue_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:01.002682 syft-0.8.1b2/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:01.006682 syft-0.8.1b2/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:01.010682 syft-0.8.1b2/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:01.018682 syft-0.8.1b2/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:01.022682 syft-0.8.1b2/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-14 12:42:01.000000 syft-0.8.1b2/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 12:45:00.942682 syft-0.8.1b2/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-14 12:45:00.000000 syft-0.8.1b2/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.624683 syft-0.8.1b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-05-21 12:41:56.000000 syft-0.8.1b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 12:41:56.000000 syft-0.8.1b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-21 12:44:53.624683 syft-0.8.1b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-21 12:41:55.000000 syft-0.8.1b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-21 12:41:56.000000 syft-0.8.1b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-21 12:44:53.628682 syft-0.8.1b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-21 12:41:56.000000 syft-0.8.1b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.588681 syft-0.8.1b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.592681 syft-0.8.1b3/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-21 12:42:13.000000 syft-0.8.1b3/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-21 12:42:13.000000 syft-0.8.1b3/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.596681 syft-0.8.1b3/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.596681 syft-0.8.1b3/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24303 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21133 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.588681 syft-0.8.1b3/src/syft/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.588681 syft-0.8.1b3/src/syft/core/node/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.596681 syft-0.8.1b3/src/syft/core/node/new/
+-rw-r--r--   0 runner    (1001) docker     (123)    26990 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/core/node/new/action_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.596681 syft-0.8.1b3/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.600682 syft-0.8.1b3/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15930 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.604682 syft-0.8.1b3/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.604682 syft-0.8.1b3/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/serde/third_party.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.604682 syft-0.8.1b3/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.608682 syft-0.8.1b3/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16617 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46598 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27045 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.608682 syft-0.8.1b3/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21458 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.612682 syft-0.8.1b3/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.612682 syft-0.8.1b3/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.612682 syft-0.8.1b3/src/syft/service/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/message/message_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/message/message_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/message/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.612682 syft-0.8.1b3/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/metadata/metadata_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.612682 syft-0.8.1b3/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20283 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/network/network_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.616682 syft-0.8.1b3/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.616682 syft-0.8.1b3/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22709 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.616682 syft-0.8.1b3/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.616682 syft-0.8.1b3/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.616682 syft-0.8.1b3/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.620682 syft-0.8.1b3/src/syft/service/vpn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/vpn/headscale_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/vpn/tailscale_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/service/vpn/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.620682 syft-0.8.1b3/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.624683 syft-0.8.1b3/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.624683 syft-0.8.1b3/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23269 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-21 12:41:56.000000 syft-0.8.1b3/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:44:53.596681 syft-0.8.1b3/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-21 12:44:53.000000 syft-0.8.1b3/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.1b2/LICENSE` & `syft-0.8.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/PKG-INFO` & `syft-0.8.1b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b2
+Version: 0.8.1b3
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b2 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b3 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.1b2/README.md` & `syft-0.8.1b3/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/setup.cfg` & `syft-0.8.1b3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.1-beta.2"
+version = attr: "0.8.1-beta.3"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -28,23 +28,25 @@
 	flax==0.5.3
 	forbiddenfruit==0.1.4
 	gevent==22.10.2
 	gipc==1.5.0
 	jax==0.3.14
 	jaxlib==0.3.14
 	loguru==0.7.0
+	networkx==2.8
 	numpy==1.24.2
 	opendp==0.6.2
 	packaging>=21.0
 	pandas==1.5.3
 	pyarrow==11.0.0
 	pycapnp==1.3.0
 	pydantic[email]==1.10.7
 	pymongo==4.3.3
 	pynacl==1.5.0
+	pyzmq==23.2.1
 	redis==4.5.4
 	requests==2.29.0
 	RestrictedPython==6.0
 	result==0.9.0
 	tqdm==4.65.0
 	typeguard==2.13.3
 	typing_extensions==4.5.0
```

### Comparing `syft-0.8.1b2/src/syft/VERSION` & `syft-0.8.1b3/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.1-beta.2"
+__version__ = "0.8.1-beta.3"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.1b2/src/syft/__init__.py` & `syft-0.8.1b3/src/syft/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.1-beta.2"
+__version__ = "0.8.1-beta.3"
 
 # stdlib
 from pathlib import Path
 import sys
 from typing import Any
 from typing import Callable
```

### Comparing `syft-0.8.1b2/src/syft/abstract_node.py` & `syft-0.8.1b3/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/client/api.py` & `syft-0.8.1b3/src/syft/client/api.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/client/client.py` & `syft-0.8.1b3/src/syft/client/client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/client/connection.py` & `syft-0.8.1b3/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/client/deploy.py` & `syft-0.8.1b3/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/client/registry.py` & `syft-0.8.1b3/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/client/search.py` & `syft-0.8.1b3/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/client/user_settings.py` & `syft-0.8.1b3/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/external/__init__.py` & `syft-0.8.1b3/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/external/oblv/__init__.py` & `syft-0.8.1b3/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/external/oblv/deployment.py` & `syft-0.8.1b3/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/external/oblv/deployment_client.py` & `syft-0.8.1b3/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/external/oblv/exceptions.py` & `syft-0.8.1b3/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.1b3/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.1b3/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/external/oblv/oblv_service.py` & `syft-0.8.1b3/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/gevent_patch.py` & `syft-0.8.1b3/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/node/credentials.py` & `syft-0.8.1b3/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/node/node.py` & `syft-0.8.1b3/src/syft/node/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from ..abstract_node import AbstractNode
 from ..abstract_node import NodeType
 from ..client.api import SignedSyftAPICall
 from ..client.api import SyftAPI
 from ..client.api import SyftAPICall
 from ..client.api import SyftAPIData
 from ..external import OBLV
+from ..serde import serialize
 from ..serde.deserialize import _deserialize
 from ..serde.serialize import _serialize
 from ..service.action.action_service import ActionService
 from ..service.action.action_store import DictActionStore
 from ..service.action.action_store import SQLiteActionStore
 from ..service.code.user_code_service import UserCodeService
 from ..service.context import AuthedServiceContext
@@ -53,16 +54,20 @@
 from ..service.metadata.metadata_service import MetadataService
 from ..service.metadata.metadata_stash import MetadataStash
 from ..service.metadata.node_metadata import NodeMetadata
 from ..service.network.network_service import NetworkService
 from ..service.policy.policy_service import PolicyService
 from ..service.project.project_service import NewProjectService
 from ..service.project.project_service import ProjectService
+from ..service.queue.queue import APICallMessageHandler
+from ..service.queue.queue import QueueManager
 from ..service.queue.queue_stash import QueueItem
 from ..service.queue.queue_stash import QueueStash
+from ..service.queue.zmq_queue import QueueConfig
+from ..service.queue.zmq_queue import ZMQQueueConfig
 from ..service.request.request_service import RequestService
 from ..service.response import SyftError
 from ..service.service import AbstractService
 from ..service.service import ServiceConfigRegistry
 from ..service.service import UserServiceConfigRegistry
 from ..service.user.user import User
 from ..service.user.user import UserCreate
@@ -99,27 +104,32 @@
 
 def gipc_decoder(obj_bytes):
     return _deserialize(obj_bytes, from_bytes=True)
 
 
 NODE_PRIVATE_KEY = "NODE_PRIVATE_KEY"
 NODE_UID = "NODE_UID"
+NODE_TYPE = "NODE_TYPE"
 
 DEFAULT_ROOT_EMAIL = "DEFAULT_ROOT_EMAIL"
 DEFAULT_ROOT_PASSWORD = "DEFAULT_ROOT_PASSWORD"  # nosec
 
 
 def get_env(key: str, default: Optional[Any] = None) -> Optional[str]:
     return os.environ.get(key, default)
 
 
 def get_private_key_env() -> Optional[str]:
     return get_env(NODE_PRIVATE_KEY)
 
 
+def get_node_type() -> Optional[str]:
+    return get_env(NODE_TYPE, "domain")
+
+
 def get_node_uid_env() -> Optional[str]:
     return get_env(NODE_UID)
 
 
 def get_default_root_email() -> Optional[str]:
     return get_env(DEFAULT_ROOT_EMAIL, "info@openmined.org")
 
@@ -152,14 +162,15 @@
         root_email: str = default_root_email,
         root_password: str = default_root_password,
         processes: int = 0,
         is_subprocess: bool = False,
         node_type: NodeType = NodeType.DOMAIN,
         local_db: bool = False,
         sqlite_path: Optional[str] = None,
+        queue_config: QueueConfig = ZMQQueueConfig,
     ):
         # 🟡 TODO 22: change our ENV variable format and default init args to make this
         # less horrible or add some convenience functions
         if node_uid_env is not None:
             self.id = UID.from_string(node_uid_env)
         else:
             if id is None:
@@ -228,14 +239,30 @@
             node=self,
         )
 
         self.client_cache = {}
         self.node_type = node_type
 
         self.post_init()
+        if not (self.is_subprocess or self.processes == 0):
+            self.init_queue_manager(queue_config=queue_config)
+
+    def init_queue_manager(self, queue_config: QueueConfig):
+        MessageHandlers = [APICallMessageHandler]
+
+        self.queue_manager = QueueManager(queue_config)
+        for message_handler in MessageHandlers:
+            queue_name = message_handler.queue_name
+            producer = self.queue_manager.create_producer(
+                queue_name=queue_name,
+            )
+            consumer = self.queue_manager.create_consumer(
+                message_handler, producer.address
+            )
+            consumer.run()
 
     @classmethod
     def named(
         cls,
         name: str,
         processes: int = 0,
         reset: bool = False,
@@ -323,15 +350,14 @@
             # why would we do this?
             # print(f"> {self}")
 
         def reload_user_code() -> None:
             user_code_service.load_user_code(context=context)
 
         CODE_RELOADER[thread_ident()] = reload_user_code
-        # super().post_init()
 
     def init_stores(
         self,
         document_store_config: Optional[StoreConfig] = None,
         action_store_config: Optional[StoreConfig] = None,
     ):
         if document_store_config is None:
@@ -464,16 +490,18 @@
             return False
 
         if self.id != other.id:
             return False
 
         return True
 
-    def resolve_future(self, uid: UID) -> Union[Optional[QueueItem], SyftError]:
-        result = self.queue_stash.pop(uid)
+    def resolve_future(
+        self, credentials: SyftVerifyKey, uid: UID
+    ) -> Union[Optional[QueueItem], SyftError]:
+        result = self.queue_stash.pop_on_complete(credentials, uid)
         if result.is_ok():
             return result.ok()
         return result.err()
 
     def forward_message(
         self, api_call: Union[SyftAPICall, SignedSyftAPICall]
     ) -> Result[Union[QueueItem, SyftObject], Err]:
@@ -531,21 +559,25 @@
             if not api_call.is_valid:
                 return SyftError(message="Your message signature is invalid")  # type: ignore
 
         if api_call.message.node_uid != self.id:
             return self.forward_message(api_call=api_call)
 
         if api_call.message.path == "queue":
-            return self.resolve_future(uid=api_call.message.kwargs["uid"])
+            return self.resolve_future(
+                credentials=api_call.credentials, uid=api_call.message.kwargs["uid"]
+            )
 
         if api_call.message.path == "metadata":
             return self.metadata
 
         result = None
-        if self.is_subprocess or self.processes == 0:
+        is_blocking = api_call.message.blocking
+
+        if is_blocking or self.is_subprocess or self.processes == 0:
             credentials: SyftVerifyKey = api_call.credentials
             api_call = api_call.message
 
             role = self.get_role_for_credentials(credentials=credentials)
             context = AuthedServiceContext(
                 node=self, credentials=credentials, role=role
             )
@@ -566,44 +598,28 @@
             try:
                 result = method(context, *api_call.args, **api_call.kwargs)
             except Exception:
                 result = SyftError(
                     message=f"Exception calling {api_call.path}. {traceback.format_exc()}"
                 )
         else:
-            worker_settings = WorkerSettings(
-                id=self.id,
-                name=self.name,
-                signing_key=self.signing_key,
-                document_store_config=self.document_store_config,
-                action_store_config=self.action_store_config,
-            )
-
             task_uid = UID()
             item = QueueItem(id=task_uid, node_uid=self.id)
             # 🟡 TODO 36: Needs distributed lock
-            # self.queue_stash.set_placeholder(item)
-            # self.queue_stash.partition.commit()
-            thread = gevent.spawn(
-                queue_task,
-                api_call,
-                worker_settings,
-                task_uid,
-                api_call.message.blocking,
-            )
-            if api_call.message.blocking:
-                gevent.joinall([thread])
-                signed_result = thread.value
+            self.queue_stash.set_placeholder(self.verify_key, item)
 
-                if not signed_result.is_valid:
-                    return SyftError(message="The result signature is invalid")  # type: ignore
+            # Publisher system which pushes to a Queue
+            worker_settings = WorkerSettings.from_node(node=self)
 
-                result = signed_result.message.data
-            else:
-                result = item
+            message_bytes = serialize._serialize(
+                [task_uid, api_call, worker_settings], to_bytes=True
+            )
+            self.queue_manager.send(message=message_bytes, queue_name="api_call")
+
+            return item
         return result
 
     def get_api(self, for_user: Optional[SyftVerifyKey] = None) -> SyftAPI:
         return SyftAPI.for_user(node=self, user_verify_key=for_user)
 
     def get_method_with_context(
         self, function: Callable, context: NodeServiceContext
```

### Comparing `syft-0.8.1b2/src/syft/node/routes.py` & `syft-0.8.1b3/src/syft/node/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         context = NodeServiceContext(node=node)
         method = node.get_method_with_context(UserService.register, context)
 
         result = method(new_user=user_create)
 
         if isinstance(result, SyftError):
             logger.bind(payload={"user": user_create}).error(result.message)
-            response = SyftError(message=f"User Registration failed: {result.message}")
+            response = SyftError(message=f"{result.message}")
         else:
             response = result
 
         return Response(
             serialize(response, to_bytes=True),
             media_type="application/octet-stream",
         )
```

### Comparing `syft-0.8.1b2/src/syft/node/run.py` & `syft-0.8.1b3/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/node/server.py` & `syft-0.8.1b3/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/node/worker_settings.py` & `syft-0.8.1b3/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/serde/array.py` & `syft-0.8.1b3/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/serde/arrow.py` & `syft-0.8.1b3/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/serde/deserialize.py` & `syft-0.8.1b3/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/serde/lib_permissions.py` & `syft-0.8.1b3/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/serde/lib_service_registry.py` & `syft-0.8.1b3/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/serde/recursive.py` & `syft-0.8.1b3/src/syft/serde/recursive.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,34 +68,35 @@
         ]
         attribute_list.update(pydantic_fields)
 
     if serialize_attrs:
         # If serialize_attrs is provided, append it to our attr list
         attribute_list.update(serialize_attrs)
 
-    if exclude_attrs:
-        attribute_list = attribute_list - set(exclude_attrs)
-
     if issubclass(cls, Enum):
         attribute_list.update(["value"])
 
+    exclude_attrs = [] if exclude_attrs is None else exclude_attrs
+    attribute_list = attribute_list - set(exclude_attrs)
+
     if inheritable_attrs and attribute_list and not is_pydantic:
         # only set __syft_serializable__ for non-pydantic classes because
         # pydantic objects inherit by default
         setattr(cls, "__syft_serializable__", attribute_list)
 
     attributes = set(list(attribute_list)) if attribute_list else None
     serde_overrides = getattr(cls, "__serde_overrides__", {})
 
     # without fqn duplicate class names overwrite
     TYPE_BANK[fqn] = (
         nonrecursive,
         _serialize,
         _deserialize,
         attributes,
+        exclude_attrs,
         serde_overrides,
         cls,
     )
 
 
 def chunk_bytes(
     data: bytes, field_name: Union[str, int], builder: _DynamicStructBuilder
@@ -132,14 +133,15 @@
 
     msg.fullyQualifiedName = fqn
     (
         nonrecursive,
         serialize,
         deserialize,
         attribute_list,
+        exclude_attrs_list,
         serde_overrides,
         cls,
     ) = TYPE_BANK[fqn]
 
     if nonrecursive or is_type:
         if serialize is None:
             raise Exception(
@@ -147,14 +149,16 @@
             )
         chunk_bytes(serialize(self), "nonrecursiveBlob", msg)
         return msg
 
     if attribute_list is None:
         attribute_list = self.__dict__.keys()
 
+    attribute_list = set(attribute_list) - set(exclude_attrs_list)
+
     msg.init("fieldsName", len(attribute_list))
     msg.init("fieldsData", len(attribute_list))
 
     for idx, attr_name in enumerate(sorted(attribute_list)):
         if not hasattr(self, attr_name):
             raise ValueError(
                 f"{attr_name} on {type(self)} does not exist, serialization aborted!"
@@ -221,14 +225,15 @@
     # however simply getting the class from the TYPE_BANK doesn't always work and
     # causes some errors so it seems like we want to get the local one where possible
     (
         nonrecursive,
         serialize,
         deserialize,
         attribute_list,
+        exclude_attrs_list,
         serde_overrides,
         cls,
     ) = TYPE_BANK[proto.fullyQualifiedName]
 
     if class_type == type(None):
         # yes this looks stupid but it works and the opposite breaks
         class_type = cls
@@ -240,21 +245,22 @@
             )
 
         return deserialize(combine_bytes(proto.nonrecursiveBlob))
 
     kwargs = {}
 
     for attr_name, attr_bytes_list in zip(proto.fieldsName, proto.fieldsData):
-        attr_bytes = combine_bytes(attr_bytes_list)
-        attr_value = _deserialize(attr_bytes, from_bytes=True)
-        transforms = serde_overrides.get(attr_name, None)
-
-        if transforms is not None:
-            attr_value = transforms[1](attr_value)
-        kwargs[attr_name] = attr_value
+        if attr_name != "":
+            attr_bytes = combine_bytes(attr_bytes_list)
+            attr_value = _deserialize(attr_bytes, from_bytes=True)
+            transforms = serde_overrides.get(attr_name, None)
+
+            if transforms is not None:
+                attr_value = transforms[1](attr_value)
+            kwargs[attr_name] = attr_value
 
     if hasattr(class_type, "serde_constructor"):
         return getattr(class_type, "serde_constructor")(kwargs)
 
     if issubclass(class_type, Enum) and "value" in kwargs:
         obj = class_type.__new__(class_type, kwargs["value"])  # type: ignore
     elif issubclass(class_type, BaseModel):
```

### Comparing `syft-0.8.1b2/src/syft/serde/recursive_primitives.py` & `syft-0.8.1b3/src/syft/serde/recursive_primitives.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from typing import Mapping
 from typing import Optional
 from typing import TypeVar
 from typing import Union
 from typing import _GenericAlias
 from typing import _SpecialForm
 from typing import cast
+import weakref
 
 # relative
 from .capnp import get_capnp_schema
 from .recursive import chunk_bytes
 from .recursive import combine_bytes
 from .recursive import recursive_serde_register
 
@@ -225,14 +226,20 @@
 recursive_serde_register(
     set,
     serialize=serialize_iterable,
     deserialize=functools.partial(deserialize_iterable, set),
 )
 
 recursive_serde_register(
+    weakref.WeakSet,
+    serialize=serialize_iterable,
+    deserialize=functools.partial(deserialize_iterable, weakref.WeakSet),
+)
+
+recursive_serde_register(
     frozenset,
     serialize=serialize_iterable,
     deserialize=functools.partial(deserialize_iterable, frozenset),
 )
 
 recursive_serde_register(
     complex,
```

### Comparing `syft-0.8.1b2/src/syft/serde/serializable.py` & `syft-0.8.1b3/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/serde/signature.py` & `syft-0.8.1b3/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/serde/third_party.py` & `syft-0.8.1b3/src/syft/serde/third_party.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,28 @@
 from dateutil import parser
 import flax
 from flax.core.frozen_dict import FrozenDict
 from jax import numpy as jnp
 from jaxlib.xla_extension import DeviceArray
 from nacl.signing import SigningKey
 from nacl.signing import VerifyKey
+import networkx as nx
+from networkx import DiGraph
 import numpy as np
 from pandas import DataFrame
 from pandas import Series
 from pandas._libs.tslibs.timestamps import Timestamp
 import pyarrow as pa
 import pyarrow.parquet as pq
 import pydantic
 from pymongo.collection import Collection
 from result import Err
 from result import Ok
 from result import Result
+import zmq.green as zmq
 
 # relative
 from .deserialize import _deserialize as deserialize
 from .recursive_primitives import recursive_serde_register
 from .recursive_primitives import recursive_serde_register_type
 from .serialize import _serialize as serialize
 
@@ -159,9 +162,37 @@
         flax.serialization.from_state_dict(FrozenDict, deserialize(x, from_bytes=True))
     ),
 )
 
 # unsure why we have to register the object not the type but this works
 recursive_serde_register(np.core._ufunc_config._unspecified())
 
+recursive_serde_register(
+    zmq._Socket,
+    serialize_attrs=[
+        "_shadow",
+        "_monitor_socket",
+        "_type_name",
+    ],
+)
+recursive_serde_register(zmq._Context)
+
 # how else do you import a relative file to execute it?
 NOTHING = None
+
+
+# TODO: debug serializing after updating a node
+def serialize_networkx_graph(graph: DiGraph) -> bytes:
+    graph_dict: dict = nx.node_link_data(graph)
+    return serialize(graph_dict, to_bytes=True)
+
+
+def deserialize_networkx_graph(buf: bytes) -> DiGraph:
+    graph_dict: dict = deserialize(buf, from_bytes=True)
+    return nx.node_link_graph(graph_dict)
+
+
+recursive_serde_register(
+    DiGraph,
+    serialize=serialize_networkx_graph,
+    deserialize=deserialize_networkx_graph,
+)
```

### Comparing `syft-0.8.1b2/src/syft/service/action/action_object.py` & `syft-0.8.1b3/src/syft/service/action/action_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -833,26 +833,26 @@
             if HOOK_ALWAYS in self._syft_pre_hooks__:
                 for hook in self._syft_pre_hooks__[HOOK_ALWAYS]:
                     result = hook(context, *result_args, **result_kwargs)
                     if result.is_ok():
                         context, result_args, result_kwargs = result.ok()
                     else:
                         msg = result.err().replace("\\n", "\n")
-                        print(f"Pre-hook failed with {msg}")
+                        debug(f"Pre-hook failed with {msg}")
 
         if self.is_pointer:
             if name not in self._syft_dont_wrap_attrs():
                 if HOOK_ALWAYS in self._syft_pre_hooks__:
                     for hook in self._syft_pre_hooks__[HOOK_ON_POINTERS]:
                         result = hook(context, *result_args, **result_kwargs)
                         if result.is_ok():
                             context, result_args, result_kwargs = result.ok()
                         else:
                             msg = result.err().replace("\\n", "\n")
-                            print(f"Pre-hook failed with {msg}")
+                            debug(f"Pre-hook failed with {msg}")
 
         return context, result_args, result_kwargs
 
     def _syft_run_post_hooks__(
         self, context: PreHookContext, name: str, result: Any
     ) -> Any:
         """Hooks executed after the actual call"""
```

### Comparing `syft-0.8.1b2/src/syft/service/action/action_permissions.py` & `syft-0.8.1b3/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/action/action_service.py` & `syft-0.8.1b3/src/syft/service/action/action_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/action/action_store.py` & `syft-0.8.1b3/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/action/action_types.py` & `syft-0.8.1b3/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/action/numpy.py` & `syft-0.8.1b3/src/syft/service/action/numpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 class NumpyArrayObject(ActionObject, np.lib.mixins.NDArrayOperatorsMixin):
     __canonical_name__ = "NumpyArrayObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     syft_internal_type: ClassVar[Type[Any]] = np.ndarray
     syft_pointer_type = NumpyArrayObjectPointer
     syft_passthrough_attrs = BASE_PASSTHROUGH_ATTRS
-    syft_dont_wrap_attrs = ["dtype"]
+    syft_dont_wrap_attrs = ["dtype", "shape"]
 
     # def __eq__(self, other: Any) -> bool:
     #     # 🟡 TODO 8: move __eq__ to a Data / Serdeable type interface on ActionObject
     #     if isinstance(other, NumpyArrayObject):
     #         return (
     #             numpy_like_eq(self.syft_action_data, other.syft_action_data)
     #             and self.syft_pointer_type == other.syft_pointer_type
@@ -84,28 +84,28 @@
 @serializable()
 class NumpyScalarObject(ActionObject, np.lib.mixins.NDArrayOperatorsMixin):
     __canonical_name__ = "NumpyScalarObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     syft_internal_type = np.number
     syft_passthrough_attrs = BASE_PASSTHROUGH_ATTRS
-    syft_dont_wrap_attrs = ["dtype"]
+    syft_dont_wrap_attrs = ["dtype", "shape"]
 
     def __float__(self) -> float:
         return float(self.syft_action_data)
 
 
 @serializable()
 class NumpyBoolObject(ActionObject, np.lib.mixins.NDArrayOperatorsMixin):
     __canonical_name__ = "NumpyBoolObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     syft_internal_type = np.bool_
     syft_passthrough_attrs = BASE_PASSTHROUGH_ATTRS
-    syft_dont_wrap_attrs = ["dtype"]
+    syft_dont_wrap_attrs = ["dtype", "shape"]
 
 
 np_array = np.array([1, 2, 3])
 action_types[type(np_array)] = NumpyArrayObject
 
 
 SUPPORTED_BOOL_TYPES = [np.bool_]
```

### Comparing `syft-0.8.1b2/src/syft/service/action/pandas.py` & `syft-0.8.1b3/src/syft/service/action/pandas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # stdlib
 from typing import Any
 from typing import ClassVar
+from typing import Optional
 from typing import Type
 
 # third party
 from pandas import DataFrame
 from pandas import Series
 
 # relative
@@ -18,14 +19,15 @@
 @serializable()
 class PandasDataFrameObject(ActionObject):
     __canonical_name__ = "PandasDataframeObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     syft_internal_type: ClassVar[Type[Any]] = DataFrame
     syft_passthrough_attrs = BASE_PASSTHROUGH_ATTRS
+    # this is added for instance checks for dataframes
     # syft_dont_wrap_attrs = ["shape"]
 
     def __dataframe__(self, *args: Any, **kwargs: Any) -> Any:
         return self.__dataframe__(*args, **kwargs)
 
     def __getattribute__(self, name: str) -> Any:
         return super().__getattribute__(name)
@@ -42,14 +44,17 @@
 
 @serializable()
 class PandasSeriesObject(ActionObject):
     __canonical_name__ = "PandasSeriesObject"
     __version__ = SYFT_OBJECT_VERSION_1
 
     syft_internal_type = Series
+    syft_passthrough_attrs = BASE_PASSTHROUGH_ATTRS
+
+    name: Optional[str] = None
     # syft_dont_wrap_attrs = ["shape"]
 
     def __getattribute__(self, name: str) -> Any:
         return super().__getattribute__(name)
 
     def syft_get_property(self, obj: Any, method: str) -> Any:
         return getattr(self.syft_action_data, method)
```

### Comparing `syft-0.8.1b2/src/syft/service/action/plan.py` & `syft-0.8.1b3/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/action/verification.py` & `syft-0.8.1b3/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/code/unparse.py` & `syft-0.8.1b3/src/syft/service/code/unparse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/code/user_code.py` & `syft-0.8.1b3/src/syft/service/code/user_code.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/code/user_code_parse.py` & `syft-0.8.1b3/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/code/user_code_service.py` & `syft-0.8.1b3/src/syft/service/code/user_code_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/code/user_code_stash.py` & `syft-0.8.1b3/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/context.py` & `syft-0.8.1b3/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/data_subject/data_subject.py` & `syft-0.8.1b3/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.1b3/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.1b3/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.1b3/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/dataset/dataset.py` & `syft-0.8.1b3/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/dataset/dataset_service.py` & `syft-0.8.1b3/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.1b3/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/message/message_service.py` & `syft-0.8.1b3/src/syft/service/message/message_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/message/message_stash.py` & `syft-0.8.1b3/src/syft/service/message/message_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/message/messages.py` & `syft-0.8.1b3/src/syft/service/message/messages.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/metadata/metadata_service.py` & `syft-0.8.1b3/src/syft/service/metadata/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/metadata/metadata_stash.py` & `syft-0.8.1b3/src/syft/service/metadata/metadata_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/metadata/node_metadata.py` & `syft-0.8.1b3/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/network/network_service.py` & `syft-0.8.1b3/src/syft/service/network/network_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -41,14 +41,20 @@
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user_roles import GUEST_ROLE_LEVEL
+from ..vpn.headscale_client import HeadscaleAuthToken
+from ..vpn.headscale_client import HeadscaleClient
+from ..vpn.tailscale_client import TailscaleClient
+from ..vpn.tailscale_client import TailscaleState
+from ..vpn.tailscale_client import TailscaleStatus
+from ..vpn.tailscale_client import get_vpn_client
 
 VerifyKeyPartitionKey = PartitionKey(key="verify_key", type_=SyftVerifyKey)
 
 
 class NodeRoute:
     def client_with_context(self, context: NodeServiceContext) -> SyftClient:
         connection = route_to_connection(route=self, context=context)
@@ -140,14 +146,16 @@
     # version
     __canonical_name__ = "NodePeer"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: Optional[UID]
     name: str
     verify_key: SyftVerifyKey
+    is_vpn: bool = False
+    vpn_auth_key: Optional[str] = None
     node_routes: List[NodeRoute] = []
 
     __attr_searchable__ = ["name"]
     __attr_unique__ = ["verify_key"]
     __attr_repr_cols__ = ["name"]
 
     def __hash__(self) -> int:
@@ -275,15 +283,15 @@
 
     def update_peer(
         self, credentials: SyftVerifyKey, peer: NodePeer
     ) -> Result[NodePeer, str]:
         valid = self.check_type(peer, NodePeer)
         if valid.is_err():
             return SyftError(message=valid.err())
-        existing = self.get_by_uid(credentials, peer.id)
+        existing = self.get_by_uid(credentials=credentials, uid=peer.id)
         if existing.is_ok() and existing.ok():
             existing = existing.ok()
             existing.update_routes(peer.node_routes)
             result = self.update(credentials, existing)
             return result
         else:
             result = self.set(credentials, peer)
@@ -339,15 +347,15 @@
                 (
                     f"Response from remote peer {remote_peer_metadata} "
                     f"does not match initial peer {remote_peer}"
                 )
             )
 
         # save the remote peer for later
-        result = self.stash.update_peer(context.credentials, remote_peer)
+        result = self.stash.update_peer(context.node.verify_key, remote_peer)
         if result.is_err():
             return SyftError(message=str(result.err()))
 
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="Credentials Exchanged")
 
@@ -417,15 +425,15 @@
             return SyftError(
                 message=(
                     f"verify_key: {metadata.verify_key} at route {route} "
                     f"does not match listed peer: {peer}"
                 )
             )
         peer.update_routes([route])
-        result = self.stash.update_peer(context.credentials, peer)
+        result = self.stash.update_peer(context.node.verify_key, peer)
         if result.is_err():
             return SyftError(message=str(result.err()))
         return SyftSuccess(message="Network Route Verified")
 
     @service_method(path="network.get_all_peers", name="get_all_peers")
     def get_all_peers(
         self, context: AuthedServiceContext
@@ -433,10 +441,166 @@
         """Get all Peers"""
         result = self.stash.get_all(context.credentials)
         if result.is_ok():
             peers = result.ok()
             return peers
         return SyftError(message=result.err())
 
+    @service_method(path="network.join_vpn", name="join_vpn")
+    def join_vpn(
+        self,
+        context: AuthedServiceContext,
+        peer: Optional[NodePeer] = None,
+        client: Optional[SyftClient] = None,
+    ) -> Union[SyftSuccess, SyftError]:
+        """Join a VPN Service"""
+
+        if isinstance(client, SyftClient):
+            remote_peer = NodePeer.from_client(client)
+        else:
+            remote_peer = peer
+        if remote_peer is None:
+            return SyftError("join_vpn requires peer or client")
+
+        result = self.stash.get_by_uid(
+            credentials=context.node.verify_key, uid=remote_peer.id
+        )
+
+        if result.is_err():
+            return SyftError(message=f"{result.err()}")
+
+        if result.ok() is not None:
+            return SyftError(
+                message=f"Already connected to VPN Peer: {remote_peer.name}"
+            )
+
+        # tell the remote peer our details
+        if not context.node:
+            return SyftError(message=f"{type(context)} has no node")
+
+        # switch to the nodes signing key
+        client = remote_peer.client_with_context(context=context)
+
+        auth_token = client.api.services.network.register_to_vpn()
+
+        if isinstance(auth_token, SyftError):
+            return auth_token
+
+        result = get_vpn_client(TailscaleClient)
+
+        if result.is_err():
+            return SyftError(message=result.err())
+
+        tailscale_client = result.ok()
+
+        result = tailscale_client.disconnect()
+
+        if isinstance(result, SyftError):
+            return result
+
+        # TODO: move this url information /vpn stuff to the client
+        vpn_url = GridURL.from_url(client.connection.url).with_path(path="/vpn")
+
+        result = tailscale_client.connect(
+            headscale_host=vpn_url,
+            headscale_auth_token=auth_token.key,
+        )
+
+        if isinstance(result, SyftError):
+            return result
+
+        # save vpn token information to peer
+        remote_peer.vpn_auth_key = auth_token.key
+        remote_peer.is_vpn = True
+
+        # save the remote peer for later
+        result = self.stash.update_peer(
+            credentials=context.node.verify_key, peer=remote_peer
+        )
+        if result.is_err():
+            return SyftError(message=str(result.err()))
+
+        if result.is_err():
+            return SyftError(message=str(result.err()))
+
+        return SyftSuccess(
+            message=f"Successfully joined {remote_peer.name} via VPN !!!"
+        )
+
+    @service_method(path="network.vpn_status", name="vpn_status")
+    def get_vpn_status(
+        self,
+        context: AuthedServiceContext,
+    ) -> Union[TailscaleStatus, SyftError]:
+        """Join a VPN Service"""
+        result = get_vpn_client(TailscaleClient)
+
+        if result.is_err():
+            return SyftError(message=result.err())
+
+        tailscale_client = result.ok()
+
+        return tailscale_client.status()
+
+    @service_method(
+        path="network.register_to_vpn",
+        name="register_to_vpn",
+        roles=GUEST_ROLE_LEVEL,
+    )
+    def register_to_vpn(
+        self,
+        context: AuthedServiceContext,
+    ) -> Union[HeadscaleAuthToken, SyftError]:
+        """Register node to the VPN."""
+
+        result = get_vpn_client(HeadscaleClient)
+
+        if result.is_err():
+            return SyftError(message=result.err())
+
+        headscale_client = result.ok()
+
+        token = headscale_client.generate_token()
+
+        return token
+
+    def connect_self(
+        self, context: AuthedServiceContext
+    ) -> Union[SyftSuccess, SyftError]:
+        tailscale_status = self.get_vpn_status(context=context)
+
+        if isinstance(tailscale_status, SyftError):
+            return tailscale_status
+
+        if tailscale_status.state is TailscaleState.RUNNING.value:
+            return SyftSuccess(message="Connection already established !!")
+
+        auth_token = self.register_to_vpn(context=context)
+
+        if isinstance(auth_token, SyftError):
+            return auth_token
+
+        result = get_vpn_client(TailscaleClient)
+
+        if result.is_err():
+            return SyftError(message=result.err())
+
+        tailscale_client = result.ok()
+
+        result = tailscale_client.disconnect()
+
+        if isinstance(result, SyftError):
+            return result
+
+        result = tailscale_client.connect(
+            headscale_host="http://headscale:8080",
+            headscale_auth_token=auth_token.key,
+        )
+
+        if isinstance(result, SyftError):
+            return result
+
+        return SyftSuccess(message="Successfully joined VPN !!!")
+
 
 TYPE_TO_SERVICE[NodePeer] = NetworkService
 SERVICE_TO_TYPES[NetworkService].update({NodePeer})
```

### Comparing `syft-0.8.1b2/src/syft/service/policy/policy.py` & `syft-0.8.1b3/src/syft/service/policy/policy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/policy/policy_service.py` & `syft-0.8.1b3/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.1b3/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/project/project.py` & `syft-0.8.1b3/src/syft/service/project/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/project/project_service.py` & `syft-0.8.1b3/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/project/project_stash.py` & `syft-0.8.1b3/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/queue/queue_stash.py` & `syft-0.8.1b3/src/syft/service/queue/queue_stash.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # stdlib
+from enum import Enum
 from typing import Any
 from typing import List
 from typing import Optional
 from typing import Union
 
 # third party
 from result import Ok
@@ -25,36 +26,47 @@
 from ..action.action_permissions import ActionObjectPermission
 from ..response import SyftError
 from ..response import SyftNotReady
 from ..response import SyftSuccess
 
 
 @serializable()
+class Status(str, Enum):
+    CREATED = "created"
+    PROCESSING = "processing"
+    ERRORED = "errored"
+    COMPLETED = "completed"
+
+
+@serializable()
 class QueueItem(SyftObject):
     __canonical_name__ = "QueueItem"
     __version__ = SYFT_OBJECT_VERSION_1
 
     id: UID
     node_uid: UID
     result: Optional[Any]
     resolved: bool = False
+    status: Status = Status.CREATED
 
     def fetch(self) -> None:
         api = APIRegistry.api_for(node_uid=self.node_uid)
         call = SyftAPICall(
             node_uid=self.node_uid,
             path="queue",
             args=[],
             kwargs={"uid": self.id},
             blocking=True,
         )
         result = api.make_call(call)
         if isinstance(result, QueueItem) and result.resolved:
             self.resolved = True
             self.result = result.result
+            self.status = result.status
+        return result
 
     @property
     def resolve(self) -> Union[Any, SyftNotReady]:
         if not self.resolved:
             self.fetch()
 
         if self.resolved:
@@ -79,26 +91,26 @@
         item: QueueItem,
         add_permissions: Optional[List[ActionObjectPermission]] = None,
     ) -> Result[Optional[QueueItem], str]:
         if item.resolved:
             valid = self.check_type(item, self.object_type)
             if valid.is_err():
                 return SyftError(message=valid.err())
-            return super().set(credentials, item, add_permissions)
+            return super().update(credentials, item, add_permissions)
         return None
 
     def set_placeholder(
         self,
         credentials: SyftVerifyKey,
         item: QueueItem,
         add_permissions: Optional[List[ActionObjectPermission]] = None,
     ) -> Result[QueueItem, str]:
         # 🟡 TODO 36: Needs distributed lock
         if not item.resolved:
-            exists = self.get_by_uid(item.id)
+            exists = self.get_by_uid(credentials, item.id)
             if exists.is_ok() and exists.ok() is None:
                 valid = self.check_type(item, self.object_type)
                 if valid.is_err():
                     return SyftError(message=valid.err())
                 return super().set(credentials, item, add_permissions)
         return item
 
@@ -112,14 +124,24 @@
     def pop(
         self, credentials: SyftVerifyKey, uid: UID
     ) -> Result[Optional[QueueItem], str]:
         item = self.get_by_uid(credentials=credentials, uid=uid)
         self.delete_by_uid(credentials=credentials, uid=uid)
         return item
 
+    def pop_on_complete(
+        self, credentials: SyftVerifyKey, uid: UID
+    ) -> Result[Optional[QueueItem], str]:
+        item = self.get_by_uid(credentials=credentials, uid=uid)
+        if item.is_ok():
+            queue_item = item.ok()
+            if queue_item.status == Status.COMPLETED:
+                self.delete_by_uid(credentials=credentials, uid=uid)
+        return item
+
     def delete_by_uid(
         self, credentials: SyftVerifyKey, uid: UID
     ) -> Result[SyftSuccess, str]:
         qk = UIDPartitionKey.with_obj(uid)
         result = super().delete(credentials=credentials, qk=qk)
         if result.is_ok():
             return Ok(SyftSuccess(message=f"ID: {uid} deleted"))
```

### Comparing `syft-0.8.1b2/src/syft/service/request/request.py` & `syft-0.8.1b3/src/syft/service/request/request.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/request/request_service.py` & `syft-0.8.1b3/src/syft/service/request/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/request/request_stash.py` & `syft-0.8.1b3/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/response.py` & `syft-0.8.1b3/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/service.py` & `syft-0.8.1b3/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/user/user.py` & `syft-0.8.1b3/src/syft/service/user/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 @serializable()
 class UserUpdate(PartialSyftObject):
     __canonical_name__ = "UserUpdate"
     __version__ = SYFT_OBJECT_VERSION_1
 
     @pydantic.validator("email", pre=True)
     def make_email(cls, v: EmailStr) -> Optional[EmailStr]:
-        return EmailStr(v) if v is not None else v
+        return EmailStr(v) if isinstance(v, str) else v
 
     email: EmailStr
     name: str
     role: ServiceRole  # make sure role cant be set without uid
     password: str
     password_verify: str
     verify_key: SyftVerifyKey
```

### Comparing `syft-0.8.1b2/src/syft/service/user/user_roles.py` & `syft-0.8.1b3/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/service/user/user_service.py` & `syft-0.8.1b3/src/syft/service/user/user_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
                 ),
             ],
         )
         if result.is_err():
             return SyftError(message=str(result.err()))
 
         user = result.ok()
-        msg = SyftSuccess(message=f"{user.email} User successfully registered !!!")
+        msg = SyftSuccess(message="User successfully registered!")
         return tuple([msg, user.to(UserPrivateKey)])
 
     def user_verify_key(self, email: str) -> Union[SyftVerifyKey, SyftError]:
         # we are bypassing permissions here, so dont use to return a result directly to the user
         credentials = self.admin_verify_key()
         result = self.stash.get_by_email(credentials=credentials, email=email)
         if result.is_ok():
```

### Comparing `syft-0.8.1b2/src/syft/service/user/user_stash.py` & `syft-0.8.1b3/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/store/dict_document_store.py` & `syft-0.8.1b3/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/store/document_store.py` & `syft-0.8.1b3/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/store/kv_document_store.py` & `syft-0.8.1b3/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/store/linked_obj.py` & `syft-0.8.1b3/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/store/locks.py` & `syft-0.8.1b3/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/store/mongo_client.py` & `syft-0.8.1b3/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/store/mongo_codecs.py` & `syft-0.8.1b3/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/store/mongo_document_store.py` & `syft-0.8.1b3/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/store/sqlite_document_store.py` & `syft-0.8.1b3/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/types/datetime.py` & `syft-0.8.1b3/src/syft/types/datetime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # stdlib
 from datetime import datetime
+from typing import Optional
 
 # third party
 from typing_extensions import Self
 
 # relative
 from ..serde.serializable import serializable
 from .syft_object import SYFT_OBJECT_VERSION_1
 from .syft_object import SyftObject
+from .uid import UID
 
 
 @serializable()
 class DateTime(SyftObject):
     __canonical_name__ = "DateTime"
     __version__ = SYFT_OBJECT_VERSION_1
 
+    id: Optional[UID]
     utc_timestamp: float
 
     @staticmethod
     def now() -> Self:
         return DateTime(utc_timestamp=datetime.utcnow().timestamp())
 
     def __str__(self) -> str:
```

### Comparing `syft-0.8.1b2/src/syft/types/grid_url.py` & `syft-0.8.1b3/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/types/syft_metaclass.py` & `syft-0.8.1b3/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/types/syft_object.py` & `syft-0.8.1b3/src/syft/types/syft_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -490,16 +490,31 @@
         super().__init__(*args_, **kwargs_)
 
         fields_with_default = set()
         for _field_name, _field in self.__fields__.items():
             if _field.default or _field.allow_none:
                 fields_with_default.add(_field_name)
 
+        # Fields whose values are set via a validator hook
+        fields_set_via_validator = []
+
+        for _field_name in self.__validators__.keys():
+            _field = self.__fields__[_field_name]
+            if self.__dict__[_field_name] is None:
+                # Since all fields are None, only allow None
+                # where either none is allowed or default is None
+                if _field.allow_none or _field.default is None:
+                    fields_set_via_validator.append(_field)
+
         # Exclude unset fields
-        unset_fields = set(self.__fields__) - set(self.__fields_set__)
+        unset_fields = (
+            set(self.__fields__)
+            - set(self.__fields_set__)
+            - set(fields_set_via_validator)
+        )
 
         empty_fields = unset_fields - fields_with_default
         for field_name in empty_fields:
             self.__dict__[field_name] = Empty
 
 
 recursive_serde_register_type(PartialSyftObject)
```

### Comparing `syft-0.8.1b2/src/syft/types/transforms.py` & `syft-0.8.1b3/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/types/twin_object.py` & `syft-0.8.1b3/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/types/uid.py` & `syft-0.8.1b3/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/util/autoreload.py` & `syft-0.8.1b3/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/util/decorators.py` & `syft-0.8.1b3/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/util/experimental_flags.py` & `syft-0.8.1b3/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/util/filterwarnings.py` & `syft-0.8.1b3/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/util/logger.py` & `syft-0.8.1b3/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/util/telemetry.py` & `syft-0.8.1b3/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/util/trace_decorator.py` & `syft-0.8.1b3/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft/util/util.py` & `syft-0.8.1b3/src/syft/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 # relative
 from ..serde.serialize import _serialize
 from .logger import critical
 from .logger import debug
 from .logger import error
 from .logger import traceback_and_raise
 
+DATASETS_URL = "https://raw.githubusercontent.com/OpenMined/datasets/main"
+PANDAS_DATA = f"{DATASETS_URL}/pandas_cookbook"
+
 
 def full_name_with_qualname(klass: type) -> str:
     """Returns the klass module name + klass qualname."""
     try:
         if not hasattr(klass, "__module__"):
             return f"builtins.{get_qualname_for(klass)}"
         return f"{klass.__module__}.{get_qualname_for(klass)}"
```

### Comparing `syft-0.8.1b2/src/syft/util/version_compare.py` & `syft-0.8.1b3/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.1b2/src/syft.egg-info/PKG-INFO` & `syft-0.8.1b3/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.1b2
+Version: 0.8.1b3
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syft Version: 0.8.1b2 Summary: Perform numpy-like
+Metadata-Version: 2.1 Name: syft Version: 0.8.1b3 Summary: Perform numpy-like
 analysis on data that remains in someone elses server Home-page: https://
 openmined.github.io/PySyft/ Author: OpenMined Author-email: info@openmined.org
 License: Apache-2.0 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Requires-Python: >=3.9 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Provides-Extra: dev Provides-Extra: test_plugins
```

### Comparing `syft-0.8.1b2/src/syft.egg-info/SOURCES.txt` & `syft-0.8.1b3/src/syft.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/syft/client/api.py
 src/syft/client/client.py
 src/syft/client/connection.py
 src/syft/client/deploy.py
 src/syft/client/registry.py
 src/syft/client/search.py
 src/syft/client/user_settings.py
+src/syft/core/node/new/action_object.py
 src/syft/external/__init__.py
 src/syft/external/oblv/__init__.py
 src/syft/external/oblv/auth.py
 src/syft/external/oblv/constants.py
 src/syft/external/oblv/deployment.py
 src/syft/external/oblv/deployment_client.py
 src/syft/external/oblv/exceptions.py
@@ -51,26 +52,29 @@
 src/syft/serde/__init__.py
 src/syft/serde/array.py
 src/syft/serde/arrow.py
 src/syft/serde/capnp.py
 src/syft/serde/deserialize.py
 src/syft/serde/lib_permissions.py
 src/syft/serde/lib_service_registry.py
+src/syft/serde/mock.py
 src/syft/serde/recursive.py
 src/syft/serde/recursive_primitives.py
 src/syft/serde/serializable.py
 src/syft/serde/serialize.py
 src/syft/serde/signature.py
 src/syft/serde/third_party.py
 src/syft/service/__init__.py
 src/syft/service/context.py
 src/syft/service/response.py
 src/syft/service/service.py
 src/syft/service/action/__init__.py
 src/syft/service/action/action_data_empty.py
+src/syft/service/action/action_graph.py
+src/syft/service/action/action_graph_service.py
 src/syft/service/action/action_object.py
 src/syft/service/action/action_permissions.py
 src/syft/service/action/action_service.py
 src/syft/service/action/action_store.py
 src/syft/service/action/action_types.py
 src/syft/service/action/numpy.py
 src/syft/service/action/pandas.py
@@ -104,25 +108,31 @@
 src/syft/service/policy/policy.py
 src/syft/service/policy/policy_service.py
 src/syft/service/policy/user_policy_stash.py
 src/syft/service/project/__init__.py
 src/syft/service/project/project.py
 src/syft/service/project/project_service.py
 src/syft/service/project/project_stash.py
+src/syft/service/queue/base_queue.py
+src/syft/service/queue/queue.py
 src/syft/service/queue/queue_stash.py
+src/syft/service/queue/zmq_queue.py
 src/syft/service/request/__init__.py
 src/syft/service/request/request.py
 src/syft/service/request/request_service.py
 src/syft/service/request/request_stash.py
 src/syft/service/user/__init__.py
 src/syft/service/user/roles.py
 src/syft/service/user/user.py
 src/syft/service/user/user_roles.py
 src/syft/service/user/user_service.py
 src/syft/service/user/user_stash.py
+src/syft/service/vpn/headscale_client.py
+src/syft/service/vpn/tailscale_client.py
+src/syft/service/vpn/vpn.py
 src/syft/store/__init__.py
 src/syft/store/dict_document_store.py
 src/syft/store/document_store.py
 src/syft/store/kv_document_store.py
 src/syft/store/linked_obj.py
 src/syft/store/locks.py
 src/syft/store/mongo_client.py
```

### Comparing `syft-0.8.1b2/src/syft.egg-info/requires.txt` & `syft-0.8.1b3/src/syft.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 flax==0.5.3
 forbiddenfruit==0.1.4
 gevent==22.10.2
 gipc==1.5.0
 jax==0.3.14
 jaxlib==0.3.14
 loguru==0.7.0
+networkx==2.8
 numpy==1.24.2
 opendp==0.6.2
 packaging>=21.0
 pandas==1.5.3
 pyarrow==11.0.0
 pycapnp==1.3.0
 pydantic[email]==1.10.7
 pymongo==4.3.3
 pynacl==1.5.0
+pyzmq==23.2.1
 redis==4.5.4
 requests==2.29.0
 RestrictedPython==6.0
 result==0.9.0
 tqdm==4.65.0
 typeguard==2.13.3
 typing_extensions==4.5.0
```

