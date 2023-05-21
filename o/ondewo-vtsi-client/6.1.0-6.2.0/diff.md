# Comparing `tmp/ondewo-vtsi-client-6.1.0.tar.gz` & `tmp/ondewo-vtsi-client-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-vtsi-client-6.1.0.tar", last modified: Sun May 21 20:27:27 2023, max compression
+gzip compressed data, was "ondewo-vtsi-client-6.2.0.tar", last modified: Sun May 21 21:03:21 2023, max compression
```

## Comparing `ondewo-vtsi-client-6.1.0.tar` & `ondewo-vtsi-client-6.2.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.082217 ondewo-vtsi-client-6.1.0/
--rw-rw-r--   0 root         (0) root         (0)    10257 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9088 2023-05-21 20:27:27.082217 ondewo-vtsi-client-6.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8516 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.077217 ondewo-vtsi-client-6.1.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.079217 ondewo-vtsi-client-6.1.0/ondewo/nlu/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    73579 2023-05-21 20:27:11.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/agent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    87204 2023-05-21 20:27:11.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/agent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    28729 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/aiservices_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16826 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/aiservices_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     1600 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/common_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      158 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/common_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    10375 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/context_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    14789 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/context_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    29954 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/entity_type_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    36069 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/entity_type_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    72044 2023-05-21 20:27:11.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/intent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    59591 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/intent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3366 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/operation_metadata_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      158 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/operation_metadata_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7908 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/operations_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    11374 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/operations_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     9554 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/project_role_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    10478 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/project_role_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7470 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/project_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16562 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/project_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3009 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/server_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     6634 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/server_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    66065 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/session_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    59122 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/session_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    19689 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/user_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    27124 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/user_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    20239 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/utility_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16902 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/utility_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     6369 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/webhook_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     6508 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/webhook_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.080217 ondewo-vtsi-client-6.1.0/ondewo/qa/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/qa/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11457 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/qa/qa_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    13389 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/qa/qa_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.080217 ondewo-vtsi-client-6.1.0/ondewo/s2t/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/s2t/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    38634 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/s2t/speech_to_text_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    30933 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/s2t/speech_to_text_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.080217 ondewo-vtsi-client-6.1.0/ondewo/sip/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/sip/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10727 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/sip/sip_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    20740 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/sip/sip_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.081217 ondewo-vtsi-client-6.1.0/ondewo/t2s/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/t2s/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    31414 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/t2s/text_to_speech_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    33144 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/t2s/text_to_speech_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.081217 ondewo-vtsi-client-6.1.0/ondewo/vtsi/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    42878 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/calls_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    29068 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/calls_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.081217 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      735 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      263 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.081217 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3734 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services/calls.py
--rw-rw-r--   0 root         (0) root         (0)     2153 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services/projects.py
--rw-rw-r--   0 root         (0) root         (0)      317 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services_container.py
--rw-rw-r--   0 root         (0) root         (0)    13169 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/projects_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    12545 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/projects_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.082217 ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9088 2023-05-21 20:27:27.000000 ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1955 2023-05-21 20:27:27.000000 ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 20:27:27.000000 ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-21 20:27:27.000000 ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-21 20:27:27.000000 ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2023-05-21 20:27:27.082217 ondewo-vtsi-client-6.1.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1586 2023-05-21 20:27:15.000000 ondewo-vtsi-client-6.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.467772 ondewo-vtsi-client-6.2.0/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9088 2023-05-21 21:03:21.467772 ondewo-vtsi-client-6.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8516 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.461773 ondewo-vtsi-client-6.2.0/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.464773 ondewo-vtsi-client-6.2.0/ondewo/nlu/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    73579 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/agent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    87204 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/agent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    28729 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/aiservices_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16826 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/aiservices_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     1600 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/common_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/common_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    10375 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/context_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    14789 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/context_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    29954 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/entity_type_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    36069 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/entity_type_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    72044 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/intent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    59591 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/intent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3366 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/operation_metadata_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/operation_metadata_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7908 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/operations_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    11374 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/operations_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     9554 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/project_role_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    10478 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/project_role_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7470 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/project_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16562 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/project_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3009 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/server_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     6634 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/server_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    66065 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/session_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    59122 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/session_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    19689 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/user_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    27124 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/user_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    20239 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/utility_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16902 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/utility_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     6369 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/webhook_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     6508 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/nlu/webhook_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.465772 ondewo-vtsi-client-6.2.0/ondewo/qa/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/qa/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11457 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/qa/qa_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    13389 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/qa/qa_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.465772 ondewo-vtsi-client-6.2.0/ondewo/s2t/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/s2t/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    38634 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/s2t/speech_to_text_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    30933 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/s2t/speech_to_text_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.465772 ondewo-vtsi-client-6.2.0/ondewo/sip/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/sip/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11001 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/sip/sip_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    21323 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/sip/sip_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.466772 ondewo-vtsi-client-6.2.0/ondewo/t2s/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/t2s/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    31414 2023-05-21 21:03:06.000000 ondewo-vtsi-client-6.2.0/ondewo/t2s/text_to_speech_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    33144 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/t2s/text_to_speech_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.466772 ondewo-vtsi-client-6.2.0/ondewo/vtsi/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    42878 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/calls_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    29068 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/calls_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.467772 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      735 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      263 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.467772 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3734 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services/calls.py
+-rw-rw-r--   0 root         (0) root         (0)     2153 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services/projects.py
+-rw-rw-r--   0 root         (0) root         (0)      317 2023-05-21 21:01:48.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    13169 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/projects_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    12545 2023-05-21 21:03:05.000000 ondewo-vtsi-client-6.2.0/ondewo/vtsi/projects_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 21:03:21.467772 ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9088 2023-05-21 21:03:21.000000 ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-05-21 21:03:21.000000 ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 21:03:21.000000 ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-21 21:03:21.000000 ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-21 21:03:21.000000 ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-05-21 21:03:21.468772 ondewo-vtsi-client-6.2.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1586 2023-05-21 21:03:09.000000 ondewo-vtsi-client-6.2.0/setup.py
```

### Comparing `ondewo-vtsi-client-6.1.0/LICENSE` & `ondewo-vtsi-client-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/PKG-INFO` & `ondewo-vtsi-client-6.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-vtsi-client
-Version: 6.1.0
+Version: 6.2.0
 Summary: exposes the ondewo-vtsi endpoints in a user-friendly way
 Home-page: https://github.com/ondewo/ondewo-vtsi-client-python
 Author: Ondewo GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.1.0 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.2.0 Summary: exposes
 the ondewo-vtsi endpoints in a user-friendly way Home-page: https://github.com/
 ondewo/ondewo-vtsi-client-python Author: Ondewo GbmH Author-email:
 office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3.8 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Software Development :: Libraries Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-vtsi-client-6.1.0/README.md` & `ondewo-vtsi-client-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/agent_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/agent_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/aiservices_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/aiservices_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/aiservices_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/aiservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/common_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/context_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/context_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/context_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/context_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/entity_type_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/entity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/entity_type_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/entity_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/intent_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/intent_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/intent_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/intent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/operation_metadata_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/operation_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/operations_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/operations_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/project_role_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/project_role_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/project_role_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/project_role_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/project_statistics_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/project_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/project_statistics_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/project_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/server_statistics_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/server_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/server_statistics_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/server_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/session_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/session_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/session_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/user_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/user_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/user_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/utility_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/utility_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/utility_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/utility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/webhook_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/webhook_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/nlu/webhook_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/nlu/webhook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/qa/qa_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/qa/qa_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/qa/qa_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/qa/qa_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/s2t/speech_to_text_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/s2t/speech_to_text_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/s2t/speech_to_text_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/s2t/speech_to_text_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/sip/sip_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/sip/sip_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,77 +10,77 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14ondewo/sip/sip.proto\x12\nondewo.sip\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"%\n\x0e\x45ndCallRequest\x12\x13\n\x0bhard_hangup\x18\x01 \x01(\x08\"\x91\x01\n\x10StartCallRequest\x12\x11\n\tcallee_id\x18\x01 \x01(\t\x12:\n\x07headers\x18\x02 \x03(\x0b\x32).ondewo.sip.StartCallRequest.HeadersEntry\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"o\n\x16RegisterAccountRequest\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x15\n\rauth_username\x18\x03 \x01(\t\x12\x16\n\x0eoutbound_proxy\x18\x04 \x01(\t\"I\n\x13StartSessionRequest\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x1c\n\x14\x61uto_answer_interval\x18\x02 \x01(\x05\"\x99\x01\n\x13TransferCallRequest\x12\x13\n\x0btransfer_id\x18\x01 \x01(\t\x12=\n\x07headers\x18\x02 \x03(\x0b\x32,.ondewo.sip.TransferCallRequest.HeadersEntry\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x97\x07\n\tSipStatus\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x0bstatus_type\x18\x03 \x01(\x0e\x32 .ondewo.sip.SipStatus.StatusType\x12\x11\n\tcallee_id\x18\x04 \x01(\t\x12\x18\n\x10transfer_call_id\x18\x05 \x01(\t\x12\x33\n\x07headers\x18\x06 \x03(\x0b\x32\".ondewo.sip.SipStatus.HeadersEntry\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x16\n\x0e\x65xception_name\x18\x08 \x01(\t\x12\x1b\n\x13\x65xception_traceback\x18\t \x01(\t\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb1\x04\n\nStatusType\x12\x0e\n\nNO_SESSION\x10\x00\x12\x0e\n\nREGISTERED\x10\x01\x12\t\n\x05READY\x10\x02\x12\x1b\n\x17INCOMING_CALL_INITIATED\x10\x03\x12\x1b\n\x17OUTGOING_CALL_INITIATED\x10\x04\x12\x1b\n\x17OUTGOING_CALL_CONNECTED\x10\x05\x12\x1b\n\x17INCOMING_CALL_CONNECTED\x10\x06\x12\x1b\n\x17TRANSFER_CALL_INITIATED\x10\x07\x12\x19\n\x15SOFT_HANGUP_INITIATED\x10\x08\x12\x19\n\x15HARD_HANGUP_INITIATED\x10\t\x12\x18\n\x14INCOMING_CALL_FAILED\x10\n\x12\x18\n\x14OUTGOING_CALL_FAILED\x10\x0b\x12\x1a\n\x16INCOMING_CALL_FINISHED\x10\x0c\x12\x1a\n\x16OUTGOING_CALL_FINISHED\x10\r\x12\x1f\n\x1bSESSION_REGISTRATION_FAILED\x10\x0e\x12\x13\n\x0fSESSION_STARTED\x10\x0f\x12\x11\n\rSESSION_ENDED\x10\x10\x12\x18\n\x14TRANSFER_CALL_FAILED\x10\x11\x12\x14\n\x10MICROPHONE_MUTED\x10\x12\x12\x16\n\x12MICROPHONE_UNMUTED\x10\x13\x12\x1f\n\x1bMICROPHONE_WAV_FILES_PLAYED\x10\x14\x12\x13\n\x0fNO_ONGOING_CALL\x10\x15\"I\n\x18SipStatusHistoryResponse\x12-\n\x0estatus_history\x18\x01 \x03(\x0b\x32\x15.ondewo.sip.SipStatus\"(\n\x13PlayWavFilesRequest\x12\x11\n\twav_files\x18\x01 \x03(\x0c\x32\x82\x06\n\x03Sip\x12H\n\x0cStartSession\x12\x1f.ondewo.sip.StartSessionRequest\x1a\x15.ondewo.sip.SipStatus\"\x00\x12=\n\nEndSession\x12\x16.google.protobuf.Empty\x1a\x15.ondewo.sip.SipStatus\"\x00\x12\x42\n\tStartCall\x12\x1c.ondewo.sip.StartCallRequest\x1a\x15.ondewo.sip.SipStatus\"\x00\x12>\n\x07\x45ndCall\x12\x1a.ondewo.sip.EndCallRequest\x1a\x15.ondewo.sip.SipStatus\"\x00\x12H\n\x0cTransferCall\x12\x1f.ondewo.sip.TransferCallRequest\x1a\x15.ondewo.sip.SipStatus\"\x00\x12N\n\x0fRegisterAccount\x12\".ondewo.sip.RegisterAccountRequest\x1a\x15.ondewo.sip.SipStatus\"\x00\x12?\n\x0cGetSipStatus\x12\x16.google.protobuf.Empty\x1a\x15.ondewo.sip.SipStatus\"\x00\x12U\n\x13GetSipStatusHistory\x12\x16.google.protobuf.Empty\x1a$.ondewo.sip.SipStatusHistoryResponse\"\x00\x12H\n\x0cPlayWavFiles\x12\x1f.ondewo.sip.PlayWavFilesRequest\x1a\x15.ondewo.sip.SipStatus\"\x00\x12\x37\n\x04Mute\x12\x16.google.protobuf.Empty\x1a\x15.ondewo.sip.SipStatus\"\x00\x12\x39\n\x06UnMute\x12\x16.google.protobuf.Empty\x1a\x15.ondewo.sip.SipStatus\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14ondewo/sip/sip.proto\x12\nondewo.sip\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"(\n\x11SipEndCallRequest\x12\x13\n\x0bhard_hangup\x18\x01 \x01(\x08\"\x97\x01\n\x13SipStartCallRequest\x12\x11\n\tcallee_id\x18\x01 \x01(\t\x12=\n\x07headers\x18\x02 \x03(\x0b\x32,.ondewo.sip.SipStartCallRequest.HeadersEntry\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x19SipRegisterAccountRequest\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x15\n\rauth_username\x18\x03 \x01(\t\x12\x16\n\x0eoutbound_proxy\x18\x04 \x01(\t\"L\n\x16SipStartSessionRequest\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x1c\n\x14\x61uto_answer_interval\x18\x02 \x01(\x05\"\x9f\x01\n\x16SipTransferCallRequest\x12\x13\n\x0btransfer_id\x18\x01 \x01(\t\x12@\n\x07headers\x18\x02 \x03(\x0b\x32/.ondewo.sip.SipTransferCallRequest.HeadersEntry\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x97\x07\n\tSipStatus\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x0bstatus_type\x18\x03 \x01(\x0e\x32 .ondewo.sip.SipStatus.StatusType\x12\x11\n\tcallee_id\x18\x04 \x01(\t\x12\x18\n\x10transfer_call_id\x18\x05 \x01(\t\x12\x33\n\x07headers\x18\x06 \x03(\x0b\x32\".ondewo.sip.SipStatus.HeadersEntry\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x16\n\x0e\x65xception_name\x18\x08 \x01(\t\x12\x1b\n\x13\x65xception_traceback\x18\t \x01(\t\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb1\x04\n\nStatusType\x12\x0e\n\nNO_SESSION\x10\x00\x12\x0e\n\nREGISTERED\x10\x01\x12\t\n\x05READY\x10\x02\x12\x1b\n\x17INCOMING_CALL_INITIATED\x10\x03\x12\x1b\n\x17OUTGOING_CALL_INITIATED\x10\x04\x12\x1b\n\x17OUTGOING_CALL_CONNECTED\x10\x05\x12\x1b\n\x17INCOMING_CALL_CONNECTED\x10\x06\x12\x1b\n\x17TRANSFER_CALL_INITIATED\x10\x07\x12\x19\n\x15SOFT_HANGUP_INITIATED\x10\x08\x12\x19\n\x15HARD_HANGUP_INITIATED\x10\t\x12\x18\n\x14INCOMING_CALL_FAILED\x10\n\x12\x18\n\x14OUTGOING_CALL_FAILED\x10\x0b\x12\x1a\n\x16INCOMING_CALL_FINISHED\x10\x0c\x12\x1a\n\x16OUTGOING_CALL_FINISHED\x10\r\x12\x1f\n\x1bSESSION_REGISTRATION_FAILED\x10\x0e\x12\x13\n\x0fSESSION_STARTED\x10\x0f\x12\x11\n\rSESSION_ENDED\x10\x10\x12\x18\n\x14TRANSFER_CALL_FAILED\x10\x11\x12\x14\n\x10MICROPHONE_MUTED\x10\x12\x12\x16\n\x12MICROPHONE_UNMUTED\x10\x13\x12\x1f\n\x1bMICROPHONE_WAV_FILES_PLAYED\x10\x14\x12\x13\n\x0fNO_ONGOING_CALL\x10\x15\"I\n\x18SipStatusHistoryResponse\x12-\n\x0estatus_history\x18\x01 \x03(\x0b\x32\x15.ondewo.sip.SipStatus\"+\n\x16SipPlayWavFilesRequest\x12\x11\n\twav_files\x18\x01 \x03(\x0c\x32\xb5\x06\n\x03Sip\x12N\n\x0fSipStartSession\x12\".ondewo.sip.SipStartSessionRequest\x1a\x15.ondewo.sip.SipStatus\"\x00\x12@\n\rSipEndSession\x12\x16.google.protobuf.Empty\x1a\x15.ondewo.sip.SipStatus\"\x00\x12H\n\x0cSipStartCall\x12\x1f.ondewo.sip.SipStartCallRequest\x1a\x15.ondewo.sip.SipStatus\"\x00\x12\x44\n\nSipEndCall\x12\x1d.ondewo.sip.SipEndCallRequest\x1a\x15.ondewo.sip.SipStatus\"\x00\x12N\n\x0fSipTransferCall\x12\".ondewo.sip.SipTransferCallRequest\x1a\x15.ondewo.sip.SipStatus\"\x00\x12T\n\x12SipRegisterAccount\x12%.ondewo.sip.SipRegisterAccountRequest\x1a\x15.ondewo.sip.SipStatus\"\x00\x12\x42\n\x0fSipGetSipStatus\x12\x16.google.protobuf.Empty\x1a\x15.ondewo.sip.SipStatus\"\x00\x12X\n\x16SipGetSipStatusHistory\x12\x16.google.protobuf.Empty\x1a$.ondewo.sip.SipStatusHistoryResponse\"\x00\x12N\n\x0fSipPlayWavFiles\x12\".ondewo.sip.SipPlayWavFilesRequest\x1a\x15.ondewo.sip.SipStatus\"\x00\x12:\n\x07SipMute\x12\x16.google.protobuf.Empty\x1a\x15.ondewo.sip.SipStatus\"\x00\x12<\n\tSipUnMute\x12\x16.google.protobuf.Empty\x1a\x15.ondewo.sip.SipStatus\"\x00\x62\x06proto3')
 
 
-_ENDCALLREQUEST = DESCRIPTOR.message_types_by_name['EndCallRequest']
-_STARTCALLREQUEST = DESCRIPTOR.message_types_by_name['StartCallRequest']
-_STARTCALLREQUEST_HEADERSENTRY = _STARTCALLREQUEST.nested_types_by_name['HeadersEntry']
-_REGISTERACCOUNTREQUEST = DESCRIPTOR.message_types_by_name['RegisterAccountRequest']
-_STARTSESSIONREQUEST = DESCRIPTOR.message_types_by_name['StartSessionRequest']
-_TRANSFERCALLREQUEST = DESCRIPTOR.message_types_by_name['TransferCallRequest']
-_TRANSFERCALLREQUEST_HEADERSENTRY = _TRANSFERCALLREQUEST.nested_types_by_name['HeadersEntry']
+_SIPENDCALLREQUEST = DESCRIPTOR.message_types_by_name['SipEndCallRequest']
+_SIPSTARTCALLREQUEST = DESCRIPTOR.message_types_by_name['SipStartCallRequest']
+_SIPSTARTCALLREQUEST_HEADERSENTRY = _SIPSTARTCALLREQUEST.nested_types_by_name['HeadersEntry']
+_SIPREGISTERACCOUNTREQUEST = DESCRIPTOR.message_types_by_name['SipRegisterAccountRequest']
+_SIPSTARTSESSIONREQUEST = DESCRIPTOR.message_types_by_name['SipStartSessionRequest']
+_SIPTRANSFERCALLREQUEST = DESCRIPTOR.message_types_by_name['SipTransferCallRequest']
+_SIPTRANSFERCALLREQUEST_HEADERSENTRY = _SIPTRANSFERCALLREQUEST.nested_types_by_name['HeadersEntry']
 _SIPSTATUS = DESCRIPTOR.message_types_by_name['SipStatus']
 _SIPSTATUS_HEADERSENTRY = _SIPSTATUS.nested_types_by_name['HeadersEntry']
 _SIPSTATUSHISTORYRESPONSE = DESCRIPTOR.message_types_by_name['SipStatusHistoryResponse']
-_PLAYWAVFILESREQUEST = DESCRIPTOR.message_types_by_name['PlayWavFilesRequest']
+_SIPPLAYWAVFILESREQUEST = DESCRIPTOR.message_types_by_name['SipPlayWavFilesRequest']
 _SIPSTATUS_STATUSTYPE = _SIPSTATUS.enum_types_by_name['StatusType']
-EndCallRequest = _reflection.GeneratedProtocolMessageType('EndCallRequest', (_message.Message,), {
-    'DESCRIPTOR': _ENDCALLREQUEST,
+SipEndCallRequest = _reflection.GeneratedProtocolMessageType('SipEndCallRequest', (_message.Message,), {
+    'DESCRIPTOR': _SIPENDCALLREQUEST,
     '__module__': 'ondewo.sip.sip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.sip.EndCallRequest)
+    # @@protoc_insertion_point(class_scope:ondewo.sip.SipEndCallRequest)
 })
-_sym_db.RegisterMessage(EndCallRequest)
+_sym_db.RegisterMessage(SipEndCallRequest)
 
-StartCallRequest = _reflection.GeneratedProtocolMessageType('StartCallRequest', (_message.Message,), {
+SipStartCallRequest = _reflection.GeneratedProtocolMessageType('SipStartCallRequest', (_message.Message,), {
 
     'HeadersEntry': _reflection.GeneratedProtocolMessageType('HeadersEntry', (_message.Message,), {
-        'DESCRIPTOR': _STARTCALLREQUEST_HEADERSENTRY,
+        'DESCRIPTOR': _SIPSTARTCALLREQUEST_HEADERSENTRY,
         '__module__': 'ondewo.sip.sip_pb2'
-        # @@protoc_insertion_point(class_scope:ondewo.sip.StartCallRequest.HeadersEntry)
+        # @@protoc_insertion_point(class_scope:ondewo.sip.SipStartCallRequest.HeadersEntry)
     }),
-    'DESCRIPTOR': _STARTCALLREQUEST,
+    'DESCRIPTOR': _SIPSTARTCALLREQUEST,
     '__module__': 'ondewo.sip.sip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.sip.StartCallRequest)
+    # @@protoc_insertion_point(class_scope:ondewo.sip.SipStartCallRequest)
 })
-_sym_db.RegisterMessage(StartCallRequest)
-_sym_db.RegisterMessage(StartCallRequest.HeadersEntry)
+_sym_db.RegisterMessage(SipStartCallRequest)
+_sym_db.RegisterMessage(SipStartCallRequest.HeadersEntry)
 
-RegisterAccountRequest = _reflection.GeneratedProtocolMessageType('RegisterAccountRequest', (_message.Message,), {
-    'DESCRIPTOR': _REGISTERACCOUNTREQUEST,
+SipRegisterAccountRequest = _reflection.GeneratedProtocolMessageType('SipRegisterAccountRequest', (_message.Message,), {
+    'DESCRIPTOR': _SIPREGISTERACCOUNTREQUEST,
     '__module__': 'ondewo.sip.sip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.sip.RegisterAccountRequest)
+    # @@protoc_insertion_point(class_scope:ondewo.sip.SipRegisterAccountRequest)
 })
-_sym_db.RegisterMessage(RegisterAccountRequest)
+_sym_db.RegisterMessage(SipRegisterAccountRequest)
 
-StartSessionRequest = _reflection.GeneratedProtocolMessageType('StartSessionRequest', (_message.Message,), {
-    'DESCRIPTOR': _STARTSESSIONREQUEST,
+SipStartSessionRequest = _reflection.GeneratedProtocolMessageType('SipStartSessionRequest', (_message.Message,), {
+    'DESCRIPTOR': _SIPSTARTSESSIONREQUEST,
     '__module__': 'ondewo.sip.sip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.sip.StartSessionRequest)
+    # @@protoc_insertion_point(class_scope:ondewo.sip.SipStartSessionRequest)
 })
-_sym_db.RegisterMessage(StartSessionRequest)
+_sym_db.RegisterMessage(SipStartSessionRequest)
 
-TransferCallRequest = _reflection.GeneratedProtocolMessageType('TransferCallRequest', (_message.Message,), {
+SipTransferCallRequest = _reflection.GeneratedProtocolMessageType('SipTransferCallRequest', (_message.Message,), {
 
     'HeadersEntry': _reflection.GeneratedProtocolMessageType('HeadersEntry', (_message.Message,), {
-        'DESCRIPTOR': _TRANSFERCALLREQUEST_HEADERSENTRY,
+        'DESCRIPTOR': _SIPTRANSFERCALLREQUEST_HEADERSENTRY,
         '__module__': 'ondewo.sip.sip_pb2'
-        # @@protoc_insertion_point(class_scope:ondewo.sip.TransferCallRequest.HeadersEntry)
+        # @@protoc_insertion_point(class_scope:ondewo.sip.SipTransferCallRequest.HeadersEntry)
     }),
-    'DESCRIPTOR': _TRANSFERCALLREQUEST,
+    'DESCRIPTOR': _SIPTRANSFERCALLREQUEST,
     '__module__': 'ondewo.sip.sip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.sip.TransferCallRequest)
+    # @@protoc_insertion_point(class_scope:ondewo.sip.SipTransferCallRequest)
 })
-_sym_db.RegisterMessage(TransferCallRequest)
-_sym_db.RegisterMessage(TransferCallRequest.HeadersEntry)
+_sym_db.RegisterMessage(SipTransferCallRequest)
+_sym_db.RegisterMessage(SipTransferCallRequest.HeadersEntry)
 
 SipStatus = _reflection.GeneratedProtocolMessageType('SipStatus', (_message.Message,), {
 
     'HeadersEntry': _reflection.GeneratedProtocolMessageType('HeadersEntry', (_message.Message,), {
         'DESCRIPTOR': _SIPSTATUS_HEADERSENTRY,
         '__module__': 'ondewo.sip.sip_pb2'
         # @@protoc_insertion_point(class_scope:ondewo.sip.SipStatus.HeadersEntry)
@@ -95,51 +95,51 @@
 SipStatusHistoryResponse = _reflection.GeneratedProtocolMessageType('SipStatusHistoryResponse', (_message.Message,), {
     'DESCRIPTOR': _SIPSTATUSHISTORYRESPONSE,
     '__module__': 'ondewo.sip.sip_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.sip.SipStatusHistoryResponse)
 })
 _sym_db.RegisterMessage(SipStatusHistoryResponse)
 
-PlayWavFilesRequest = _reflection.GeneratedProtocolMessageType('PlayWavFilesRequest', (_message.Message,), {
-    'DESCRIPTOR': _PLAYWAVFILESREQUEST,
+SipPlayWavFilesRequest = _reflection.GeneratedProtocolMessageType('SipPlayWavFilesRequest', (_message.Message,), {
+    'DESCRIPTOR': _SIPPLAYWAVFILESREQUEST,
     '__module__': 'ondewo.sip.sip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.sip.PlayWavFilesRequest)
+    # @@protoc_insertion_point(class_scope:ondewo.sip.SipPlayWavFilesRequest)
 })
-_sym_db.RegisterMessage(PlayWavFilesRequest)
+_sym_db.RegisterMessage(SipPlayWavFilesRequest)
 
 _SIP = DESCRIPTOR.services_by_name['Sip']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _STARTCALLREQUEST_HEADERSENTRY._options = None
-    _STARTCALLREQUEST_HEADERSENTRY._serialized_options = b'8\001'
-    _TRANSFERCALLREQUEST_HEADERSENTRY._options = None
-    _TRANSFERCALLREQUEST_HEADERSENTRY._serialized_options = b'8\001'
+    _SIPSTARTCALLREQUEST_HEADERSENTRY._options = None
+    _SIPSTARTCALLREQUEST_HEADERSENTRY._serialized_options = b'8\001'
+    _SIPTRANSFERCALLREQUEST_HEADERSENTRY._options = None
+    _SIPTRANSFERCALLREQUEST_HEADERSENTRY._serialized_options = b'8\001'
     _SIPSTATUS_HEADERSENTRY._options = None
     _SIPSTATUS_HEADERSENTRY._serialized_options = b'8\001'
-    _ENDCALLREQUEST._serialized_start = 98
-    _ENDCALLREQUEST._serialized_end = 135
-    _STARTCALLREQUEST._serialized_start = 138
-    _STARTCALLREQUEST._serialized_end = 283
-    _STARTCALLREQUEST_HEADERSENTRY._serialized_start = 237
-    _STARTCALLREQUEST_HEADERSENTRY._serialized_end = 283
-    _REGISTERACCOUNTREQUEST._serialized_start = 285
-    _REGISTERACCOUNTREQUEST._serialized_end = 396
-    _STARTSESSIONREQUEST._serialized_start = 398
-    _STARTSESSIONREQUEST._serialized_end = 471
-    _TRANSFERCALLREQUEST._serialized_start = 474
-    _TRANSFERCALLREQUEST._serialized_end = 627
-    _TRANSFERCALLREQUEST_HEADERSENTRY._serialized_start = 237
-    _TRANSFERCALLREQUEST_HEADERSENTRY._serialized_end = 283
-    _SIPSTATUS._serialized_start = 630
-    _SIPSTATUS._serialized_end = 1549
-    _SIPSTATUS_HEADERSENTRY._serialized_start = 237
-    _SIPSTATUS_HEADERSENTRY._serialized_end = 283
-    _SIPSTATUS_STATUSTYPE._serialized_start = 988
-    _SIPSTATUS_STATUSTYPE._serialized_end = 1549
-    _SIPSTATUSHISTORYRESPONSE._serialized_start = 1551
-    _SIPSTATUSHISTORYRESPONSE._serialized_end = 1624
-    _PLAYWAVFILESREQUEST._serialized_start = 1626
-    _PLAYWAVFILESREQUEST._serialized_end = 1666
-    _SIP._serialized_start = 1669
-    _SIP._serialized_end = 2439
+    _SIPENDCALLREQUEST._serialized_start = 98
+    _SIPENDCALLREQUEST._serialized_end = 138
+    _SIPSTARTCALLREQUEST._serialized_start = 141
+    _SIPSTARTCALLREQUEST._serialized_end = 292
+    _SIPSTARTCALLREQUEST_HEADERSENTRY._serialized_start = 246
+    _SIPSTARTCALLREQUEST_HEADERSENTRY._serialized_end = 292
+    _SIPREGISTERACCOUNTREQUEST._serialized_start = 294
+    _SIPREGISTERACCOUNTREQUEST._serialized_end = 408
+    _SIPSTARTSESSIONREQUEST._serialized_start = 410
+    _SIPSTARTSESSIONREQUEST._serialized_end = 486
+    _SIPTRANSFERCALLREQUEST._serialized_start = 489
+    _SIPTRANSFERCALLREQUEST._serialized_end = 648
+    _SIPTRANSFERCALLREQUEST_HEADERSENTRY._serialized_start = 246
+    _SIPTRANSFERCALLREQUEST_HEADERSENTRY._serialized_end = 292
+    _SIPSTATUS._serialized_start = 651
+    _SIPSTATUS._serialized_end = 1570
+    _SIPSTATUS_HEADERSENTRY._serialized_start = 246
+    _SIPSTATUS_HEADERSENTRY._serialized_end = 292
+    _SIPSTATUS_STATUSTYPE._serialized_start = 1009
+    _SIPSTATUS_STATUSTYPE._serialized_end = 1570
+    _SIPSTATUSHISTORYRESPONSE._serialized_start = 1572
+    _SIPSTATUSHISTORYRESPONSE._serialized_end = 1645
+    _SIPPLAYWAVFILESREQUEST._serialized_start = 1647
+    _SIPPLAYWAVFILESREQUEST._serialized_end = 1690
+    _SIP._serialized_start = 1693
+    _SIP._serialized_end = 2514
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/sip/sip_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/sip/sip_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,209 +13,209 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.StartSession = channel.unary_unary(
-            '/ondewo.sip.Sip/StartSession',
-            request_serializer=ondewo_dot_sip_dot_sip__pb2.StartSessionRequest.SerializeToString,
+        self.SipStartSession = channel.unary_unary(
+            '/ondewo.sip.Sip/SipStartSession',
+            request_serializer=ondewo_dot_sip_dot_sip__pb2.SipStartSessionRequest.SerializeToString,
             response_deserializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
         )
-        self.EndSession = channel.unary_unary(
-            '/ondewo.sip.Sip/EndSession',
+        self.SipEndSession = channel.unary_unary(
+            '/ondewo.sip.Sip/SipEndSession',
             request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             response_deserializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
         )
-        self.StartCall = channel.unary_unary(
-            '/ondewo.sip.Sip/StartCall',
-            request_serializer=ondewo_dot_sip_dot_sip__pb2.StartCallRequest.SerializeToString,
+        self.SipStartCall = channel.unary_unary(
+            '/ondewo.sip.Sip/SipStartCall',
+            request_serializer=ondewo_dot_sip_dot_sip__pb2.SipStartCallRequest.SerializeToString,
             response_deserializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
         )
-        self.EndCall = channel.unary_unary(
-            '/ondewo.sip.Sip/EndCall',
-            request_serializer=ondewo_dot_sip_dot_sip__pb2.EndCallRequest.SerializeToString,
+        self.SipEndCall = channel.unary_unary(
+            '/ondewo.sip.Sip/SipEndCall',
+            request_serializer=ondewo_dot_sip_dot_sip__pb2.SipEndCallRequest.SerializeToString,
             response_deserializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
         )
-        self.TransferCall = channel.unary_unary(
-            '/ondewo.sip.Sip/TransferCall',
-            request_serializer=ondewo_dot_sip_dot_sip__pb2.TransferCallRequest.SerializeToString,
+        self.SipTransferCall = channel.unary_unary(
+            '/ondewo.sip.Sip/SipTransferCall',
+            request_serializer=ondewo_dot_sip_dot_sip__pb2.SipTransferCallRequest.SerializeToString,
             response_deserializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
         )
-        self.RegisterAccount = channel.unary_unary(
-            '/ondewo.sip.Sip/RegisterAccount',
-            request_serializer=ondewo_dot_sip_dot_sip__pb2.RegisterAccountRequest.SerializeToString,
+        self.SipRegisterAccount = channel.unary_unary(
+            '/ondewo.sip.Sip/SipRegisterAccount',
+            request_serializer=ondewo_dot_sip_dot_sip__pb2.SipRegisterAccountRequest.SerializeToString,
             response_deserializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
         )
-        self.GetSipStatus = channel.unary_unary(
-            '/ondewo.sip.Sip/GetSipStatus',
+        self.SipGetSipStatus = channel.unary_unary(
+            '/ondewo.sip.Sip/SipGetSipStatus',
             request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             response_deserializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
         )
-        self.GetSipStatusHistory = channel.unary_unary(
-            '/ondewo.sip.Sip/GetSipStatusHistory',
+        self.SipGetSipStatusHistory = channel.unary_unary(
+            '/ondewo.sip.Sip/SipGetSipStatusHistory',
             request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             response_deserializer=ondewo_dot_sip_dot_sip__pb2.SipStatusHistoryResponse.FromString,
         )
-        self.PlayWavFiles = channel.unary_unary(
-            '/ondewo.sip.Sip/PlayWavFiles',
-            request_serializer=ondewo_dot_sip_dot_sip__pb2.PlayWavFilesRequest.SerializeToString,
+        self.SipPlayWavFiles = channel.unary_unary(
+            '/ondewo.sip.Sip/SipPlayWavFiles',
+            request_serializer=ondewo_dot_sip_dot_sip__pb2.SipPlayWavFilesRequest.SerializeToString,
             response_deserializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
         )
-        self.Mute = channel.unary_unary(
-            '/ondewo.sip.Sip/Mute',
+        self.SipMute = channel.unary_unary(
+            '/ondewo.sip.Sip/SipMute',
             request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             response_deserializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
         )
-        self.UnMute = channel.unary_unary(
-            '/ondewo.sip.Sip/UnMute',
+        self.SipUnMute = channel.unary_unary(
+            '/ondewo.sip.Sip/SipUnMute',
             request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             response_deserializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
         )
 
 
 class SipServicer(object):
     """ONDEWO-SIP API available at <a href="https://github.com/ondewo/ondewo-sip-api>">GitHub</a>
     SIP LifeCycle is explained at <a href="https://thanhloi2603.wordpress.com/2017/06/10/sip-lifecycle-overview/">here</a>
     """
 
-    def StartSession(self, request, context):
+    def SipStartSession(self, request, context):
         """Starts a new SIP session for an account registered at a SIP server. <code>RegisterAccount</code> need to be called before.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def EndSession(self, request, context):
+    def SipEndSession(self, request, context):
         """Ends a SIP session for an account registered at a SIP server
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def StartCall(self, request, context):
+    def SipStartCall(self, request, context):
         """Starts a call in an active SIP session for an account registered at a SIP server
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def EndCall(self, request, context):
+    def SipEndCall(self, request, context):
         """Ends a call in an active SIP session for an account registered at a SIP server
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def TransferCall(self, request, context):
+    def SipTransferCall(self, request, context):
         """Transfers a call in an active SIP session for an account registered at a SIP server to
         another SIP account or phone number specified by <code>transfer_id</code>
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def RegisterAccount(self, request, context):
+    def SipRegisterAccount(self, request, context):
         """Registers s SIP account at a SIP server
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetSipStatus(self, request, context):
+    def SipGetSipStatus(self, request, context):
         """Gets the current SIP status
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetSipStatusHistory(self, request, context):
+    def SipGetSipStatusHistory(self, request, context):
         """Gets the history of SIP status
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def PlayWavFiles(self, request, context):
+    def SipPlayWavFiles(self, request, context):
         """Plays wav files during an ongoing call of an active SIP session
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Mute(self, request, context):
+    def SipMute(self, request, context):
         """Mutes the microphone in an ongoing call of an active SIP session
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def UnMute(self, request, context):
-        """Unmutes the microphone in an ongoing call of an active SIP session
+    def SipUnMute(self, request, context):
+        """Un-mutes the microphone in an ongoing call of an active SIP session
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_SipServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        'StartSession': grpc.unary_unary_rpc_method_handler(
-            servicer.StartSession,
-            request_deserializer=ondewo_dot_sip_dot_sip__pb2.StartSessionRequest.FromString,
+        'SipStartSession': grpc.unary_unary_rpc_method_handler(
+            servicer.SipStartSession,
+            request_deserializer=ondewo_dot_sip_dot_sip__pb2.SipStartSessionRequest.FromString,
             response_serializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.SerializeToString,
         ),
-        'EndSession': grpc.unary_unary_rpc_method_handler(
-            servicer.EndSession,
+        'SipEndSession': grpc.unary_unary_rpc_method_handler(
+            servicer.SipEndSession,
             request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             response_serializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.SerializeToString,
         ),
-        'StartCall': grpc.unary_unary_rpc_method_handler(
-            servicer.StartCall,
-            request_deserializer=ondewo_dot_sip_dot_sip__pb2.StartCallRequest.FromString,
+        'SipStartCall': grpc.unary_unary_rpc_method_handler(
+            servicer.SipStartCall,
+            request_deserializer=ondewo_dot_sip_dot_sip__pb2.SipStartCallRequest.FromString,
             response_serializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.SerializeToString,
         ),
-        'EndCall': grpc.unary_unary_rpc_method_handler(
-            servicer.EndCall,
-            request_deserializer=ondewo_dot_sip_dot_sip__pb2.EndCallRequest.FromString,
+        'SipEndCall': grpc.unary_unary_rpc_method_handler(
+            servicer.SipEndCall,
+            request_deserializer=ondewo_dot_sip_dot_sip__pb2.SipEndCallRequest.FromString,
             response_serializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.SerializeToString,
         ),
-        'TransferCall': grpc.unary_unary_rpc_method_handler(
-            servicer.TransferCall,
-            request_deserializer=ondewo_dot_sip_dot_sip__pb2.TransferCallRequest.FromString,
+        'SipTransferCall': grpc.unary_unary_rpc_method_handler(
+            servicer.SipTransferCall,
+            request_deserializer=ondewo_dot_sip_dot_sip__pb2.SipTransferCallRequest.FromString,
             response_serializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.SerializeToString,
         ),
-        'RegisterAccount': grpc.unary_unary_rpc_method_handler(
-            servicer.RegisterAccount,
-            request_deserializer=ondewo_dot_sip_dot_sip__pb2.RegisterAccountRequest.FromString,
+        'SipRegisterAccount': grpc.unary_unary_rpc_method_handler(
+            servicer.SipRegisterAccount,
+            request_deserializer=ondewo_dot_sip_dot_sip__pb2.SipRegisterAccountRequest.FromString,
             response_serializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.SerializeToString,
         ),
-        'GetSipStatus': grpc.unary_unary_rpc_method_handler(
-            servicer.GetSipStatus,
+        'SipGetSipStatus': grpc.unary_unary_rpc_method_handler(
+            servicer.SipGetSipStatus,
             request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             response_serializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.SerializeToString,
         ),
-        'GetSipStatusHistory': grpc.unary_unary_rpc_method_handler(
-            servicer.GetSipStatusHistory,
+        'SipGetSipStatusHistory': grpc.unary_unary_rpc_method_handler(
+            servicer.SipGetSipStatusHistory,
             request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             response_serializer=ondewo_dot_sip_dot_sip__pb2.SipStatusHistoryResponse.SerializeToString,
         ),
-        'PlayWavFiles': grpc.unary_unary_rpc_method_handler(
-            servicer.PlayWavFiles,
-            request_deserializer=ondewo_dot_sip_dot_sip__pb2.PlayWavFilesRequest.FromString,
+        'SipPlayWavFiles': grpc.unary_unary_rpc_method_handler(
+            servicer.SipPlayWavFiles,
+            request_deserializer=ondewo_dot_sip_dot_sip__pb2.SipPlayWavFilesRequest.FromString,
             response_serializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.SerializeToString,
         ),
-        'Mute': grpc.unary_unary_rpc_method_handler(
-            servicer.Mute,
+        'SipMute': grpc.unary_unary_rpc_method_handler(
+            servicer.SipMute,
             request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             response_serializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.SerializeToString,
         ),
-        'UnMute': grpc.unary_unary_rpc_method_handler(
-            servicer.UnMute,
+        'SipUnMute': grpc.unary_unary_rpc_method_handler(
+            servicer.SipUnMute,
             request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             response_serializer=ondewo_dot_sip_dot_sip__pb2.SipStatus.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
         'ondewo.sip.Sip', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
@@ -225,192 +225,192 @@
 
 class Sip(object):
     """ONDEWO-SIP API available at <a href="https://github.com/ondewo/ondewo-sip-api>">GitHub</a>
     SIP LifeCycle is explained at <a href="https://thanhloi2603.wordpress.com/2017/06/10/sip-lifecycle-overview/">here</a>
     """
 
     @staticmethod
-    def StartSession(request,
+    def SipStartSession(request,
+                        target,
+                        options=(),
+                        channel_credentials=None,
+                        call_credentials=None,
+                        insecure=False,
+                        compression=None,
+                        wait_for_ready=None,
+                        timeout=None,
+                        metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/SipStartSession',
+                                             ondewo_dot_sip_dot_sip__pb2.SipStartSessionRequest.SerializeToString,
+                                             ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SipEndSession(request,
+                      target,
+                      options=(),
+                      channel_credentials=None,
+                      call_credentials=None,
+                      insecure=False,
+                      compression=None,
+                      wait_for_ready=None,
+                      timeout=None,
+                      metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/SipEndSession',
+                                             google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                                             ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SipStartCall(request,
                      target,
                      options=(),
                      channel_credentials=None,
                      call_credentials=None,
                      insecure=False,
                      compression=None,
                      wait_for_ready=None,
                      timeout=None,
                      metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/StartSession',
-                                             ondewo_dot_sip_dot_sip__pb2.StartSessionRequest.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/SipStartCall',
+                                             ondewo_dot_sip_dot_sip__pb2.SipStartCallRequest.SerializeToString,
                                              ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def EndSession(request,
+    def SipEndCall(request,
                    target,
                    options=(),
                    channel_credentials=None,
                    call_credentials=None,
                    insecure=False,
                    compression=None,
                    wait_for_ready=None,
                    timeout=None,
                    metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/EndSession',
-                                             google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-                                             ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def StartCall(request,
-                  target,
-                  options=(),
-                  channel_credentials=None,
-                  call_credentials=None,
-                  insecure=False,
-                  compression=None,
-                  wait_for_ready=None,
-                  timeout=None,
-                  metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/StartCall',
-                                             ondewo_dot_sip_dot_sip__pb2.StartCallRequest.SerializeToString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/SipEndCall',
+                                             ondewo_dot_sip_dot_sip__pb2.SipEndCallRequest.SerializeToString,
                                              ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def EndCall(request,
-                target,
-                options=(),
-                channel_credentials=None,
-                call_credentials=None,
-                insecure=False,
-                compression=None,
-                wait_for_ready=None,
-                timeout=None,
-                metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/EndCall',
-                                             ondewo_dot_sip_dot_sip__pb2.EndCallRequest.SerializeToString,
+    def SipTransferCall(request,
+                        target,
+                        options=(),
+                        channel_credentials=None,
+                        call_credentials=None,
+                        insecure=False,
+                        compression=None,
+                        wait_for_ready=None,
+                        timeout=None,
+                        metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/SipTransferCall',
+                                             ondewo_dot_sip_dot_sip__pb2.SipTransferCallRequest.SerializeToString,
                                              ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def TransferCall(request,
-                     target,
-                     options=(),
-                     channel_credentials=None,
-                     call_credentials=None,
-                     insecure=False,
-                     compression=None,
-                     wait_for_ready=None,
-                     timeout=None,
-                     metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/TransferCall',
-                                             ondewo_dot_sip_dot_sip__pb2.TransferCallRequest.SerializeToString,
+    def SipRegisterAccount(request,
+                           target,
+                           options=(),
+                           channel_credentials=None,
+                           call_credentials=None,
+                           insecure=False,
+                           compression=None,
+                           wait_for_ready=None,
+                           timeout=None,
+                           metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/SipRegisterAccount',
+                                             ondewo_dot_sip_dot_sip__pb2.SipRegisterAccountRequest.SerializeToString,
                                              ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def RegisterAccount(request,
+    def SipGetSipStatus(request,
                         target,
                         options=(),
                         channel_credentials=None,
                         call_credentials=None,
                         insecure=False,
                         compression=None,
                         wait_for_ready=None,
                         timeout=None,
                         metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/RegisterAccount',
-                                             ondewo_dot_sip_dot_sip__pb2.RegisterAccountRequest.SerializeToString,
-                                             ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetSipStatus(request,
-                     target,
-                     options=(),
-                     channel_credentials=None,
-                     call_credentials=None,
-                     insecure=False,
-                     compression=None,
-                     wait_for_ready=None,
-                     timeout=None,
-                     metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/GetSipStatus',
+        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/SipGetSipStatus',
                                              google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                                              ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetSipStatusHistory(request,
-                            target,
-                            options=(),
-                            channel_credentials=None,
-                            call_credentials=None,
-                            insecure=False,
-                            compression=None,
-                            wait_for_ready=None,
-                            timeout=None,
-                            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/GetSipStatusHistory',
+    def SipGetSipStatusHistory(request,
+                               target,
+                               options=(),
+                               channel_credentials=None,
+                               call_credentials=None,
+                               insecure=False,
+                               compression=None,
+                               wait_for_ready=None,
+                               timeout=None,
+                               metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/SipGetSipStatusHistory',
                                              google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                                              ondewo_dot_sip_dot_sip__pb2.SipStatusHistoryResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def PlayWavFiles(request,
-                     target,
-                     options=(),
-                     channel_credentials=None,
-                     call_credentials=None,
-                     insecure=False,
-                     compression=None,
-                     wait_for_ready=None,
-                     timeout=None,
-                     metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/PlayWavFiles',
-                                             ondewo_dot_sip_dot_sip__pb2.PlayWavFilesRequest.SerializeToString,
+    def SipPlayWavFiles(request,
+                        target,
+                        options=(),
+                        channel_credentials=None,
+                        call_credentials=None,
+                        insecure=False,
+                        compression=None,
+                        wait_for_ready=None,
+                        timeout=None,
+                        metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/SipPlayWavFiles',
+                                             ondewo_dot_sip_dot_sip__pb2.SipPlayWavFilesRequest.SerializeToString,
                                              ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Mute(request,
-             target,
-             options=(),
-             channel_credentials=None,
-             call_credentials=None,
-             insecure=False,
-             compression=None,
-             wait_for_ready=None,
-             timeout=None,
-             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/Mute',
+    def SipMute(request,
+                target,
+                options=(),
+                channel_credentials=None,
+                call_credentials=None,
+                insecure=False,
+                compression=None,
+                wait_for_ready=None,
+                timeout=None,
+                metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/SipMute',
                                              google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                                              ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def UnMute(request,
-               target,
-               options=(),
-               channel_credentials=None,
-               call_credentials=None,
-               insecure=False,
-               compression=None,
-               wait_for_ready=None,
-               timeout=None,
-               metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/UnMute',
+    def SipUnMute(request,
+                  target,
+                  options=(),
+                  channel_credentials=None,
+                  call_credentials=None,
+                  insecure=False,
+                  compression=None,
+                  wait_for_ready=None,
+                  timeout=None,
+                  metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.sip.Sip/SipUnMute',
                                              google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                                              ondewo_dot_sip_dot_sip__pb2.SipStatus.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/t2s/text_to_speech_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/t2s/text_to_speech_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/t2s/text_to_speech_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/t2s/text_to_speech_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/vtsi/calls_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/vtsi/calls_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/vtsi/calls_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/vtsi/calls_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/client.py` & `ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services/calls.py` & `ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services/calls.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services/projects.py` & `ondewo-vtsi-client-6.2.0/ondewo/vtsi/client/services/projects.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/vtsi/projects_pb2.py` & `ondewo-vtsi-client-6.2.0/ondewo/vtsi/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo/vtsi/projects_pb2_grpc.py` & `ondewo-vtsi-client-6.2.0/ondewo/vtsi/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/PKG-INFO` & `ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-vtsi-client
-Version: 6.1.0
+Version: 6.2.0
 Summary: exposes the ondewo-vtsi endpoints in a user-friendly way
 Home-page: https://github.com/ondewo/ondewo-vtsi-client-python
 Author: Ondewo GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.1.0 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.2.0 Summary: exposes
 the ondewo-vtsi endpoints in a user-friendly way Home-page: https://github.com/
 ondewo/ondewo-vtsi-client-python Author: Ondewo GbmH Author-email:
 office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3.8 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Software Development :: Libraries Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/SOURCES.txt` & `ondewo-vtsi-client-6.2.0/ondewo_vtsi_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.1.0/setup.py` & `ondewo-vtsi-client-6.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             req_str = f"{req_name} @ {req_url}"
         else:
             req_str = req
         requires.append(req_str)
 
 setup(
     name="ondewo-vtsi-client",
-    version='6.1.0',
+    version='6.2.0',
     author="Ondewo GbmH",
     author_email="office@ondewo.com",
     description="exposes the ondewo-vtsi endpoints in a user-friendly way",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ondewo/ondewo-vtsi-client-python",
     packages=[
```

