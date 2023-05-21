# Comparing `tmp/ondewo-vtsi-client-6.0.0.tar.gz` & `tmp/ondewo-vtsi-client-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-vtsi-client-6.0.0.tar", last modified: Sun May 21 19:37:12 2023, max compression
+gzip compressed data, was "ondewo-vtsi-client-6.1.0.tar", last modified: Sun May 21 20:27:27 2023, max compression
```

## Comparing `ondewo-vtsi-client-6.0.0.tar` & `ondewo-vtsi-client-6.1.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.332427 ondewo-vtsi-client-6.0.0/
--rw-rw-r--   0 root         (0) root         (0)    10257 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9088 2023-05-21 19:37:12.332427 ondewo-vtsi-client-6.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8516 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.327427 ondewo-vtsi-client-6.0.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.330427 ondewo-vtsi-client-6.0.0/ondewo/nlu/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    73579 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/agent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    87204 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/agent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    28729 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/aiservices_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16826 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/aiservices_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     1600 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/common_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      158 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/common_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    10375 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/context_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    14789 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/context_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    29954 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/entity_type_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    36069 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/entity_type_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    72044 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/intent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    59591 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/intent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3366 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/operation_metadata_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      158 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/operation_metadata_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7908 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/operations_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    11374 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/operations_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     9554 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/project_role_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    10478 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/project_role_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7470 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/project_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16562 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/project_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3009 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/server_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     6634 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/server_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    66065 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/session_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    59122 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/session_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    19689 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/user_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    27124 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/user_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    20239 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/utility_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16902 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/utility_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     6369 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/webhook_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     6508 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/webhook_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.330427 ondewo-vtsi-client-6.0.0/ondewo/qa/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/qa/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11457 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/qa/qa_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    13389 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/qa/qa_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.330427 ondewo-vtsi-client-6.0.0/ondewo/s2t/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/s2t/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    38634 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/s2t/speech_to_text_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    30933 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/s2t/speech_to_text_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.330427 ondewo-vtsi-client-6.0.0/ondewo/sip/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/sip/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10727 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/sip/sip_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    20740 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/sip/sip_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.331427 ondewo-vtsi-client-6.0.0/ondewo/t2s/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/t2s/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    31414 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/t2s/text_to_speech_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    33144 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/t2s/text_to_speech_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.331427 ondewo-vtsi-client-6.0.0/ondewo/vtsi/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    42878 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/calls_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    29068 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/calls_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.331427 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      735 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      263 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.332427 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3734 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/services/calls.py
--rw-rw-r--   0 root         (0) root         (0)     2153 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/services/projects.py
--rw-rw-r--   0 root         (0) root         (0)      317 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/services_container.py
--rw-rw-r--   0 root         (0) root         (0)    13169 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/projects_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    12545 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/projects_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.332427 ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9088 2023-05-21 19:37:12.000000 ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1955 2023-05-21 19:37:12.000000 ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 19:37:12.000000 ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-21 19:37:12.000000 ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-21 19:37:12.000000 ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2023-05-21 19:37:12.333427 ondewo-vtsi-client-6.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1586 2023-05-21 19:37:00.000000 ondewo-vtsi-client-6.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.082217 ondewo-vtsi-client-6.1.0/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9088 2023-05-21 20:27:27.082217 ondewo-vtsi-client-6.1.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8516 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.077217 ondewo-vtsi-client-6.1.0/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.079217 ondewo-vtsi-client-6.1.0/ondewo/nlu/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    73579 2023-05-21 20:27:11.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/agent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    87204 2023-05-21 20:27:11.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/agent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    28729 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/aiservices_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16826 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/aiservices_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     1600 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/common_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/common_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    10375 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/context_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    14789 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/context_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    29954 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/entity_type_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    36069 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/entity_type_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    72044 2023-05-21 20:27:11.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/intent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    59591 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/intent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3366 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/operation_metadata_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/operation_metadata_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7908 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/operations_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    11374 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/operations_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     9554 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/project_role_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    10478 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/project_role_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7470 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/project_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16562 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/project_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3009 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/server_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     6634 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/server_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    66065 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/session_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    59122 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/session_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    19689 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/user_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    27124 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/user_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    20239 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/utility_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16902 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/utility_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     6369 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/webhook_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     6508 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/nlu/webhook_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.080217 ondewo-vtsi-client-6.1.0/ondewo/qa/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/qa/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11457 2023-05-21 20:27:09.000000 ondewo-vtsi-client-6.1.0/ondewo/qa/qa_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    13389 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/qa/qa_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.080217 ondewo-vtsi-client-6.1.0/ondewo/s2t/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/s2t/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    38634 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/s2t/speech_to_text_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    30933 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/s2t/speech_to_text_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.080217 ondewo-vtsi-client-6.1.0/ondewo/sip/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/sip/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10727 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/sip/sip_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    20740 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/sip/sip_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.081217 ondewo-vtsi-client-6.1.0/ondewo/t2s/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/t2s/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    31414 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/t2s/text_to_speech_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    33144 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/t2s/text_to_speech_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.081217 ondewo-vtsi-client-6.1.0/ondewo/vtsi/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    42878 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/calls_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    29068 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/calls_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.081217 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      735 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      263 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.081217 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3734 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services/calls.py
+-rw-rw-r--   0 root         (0) root         (0)     2153 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services/projects.py
+-rw-rw-r--   0 root         (0) root         (0)      317 2023-05-21 20:25:59.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    13169 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/projects_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    12545 2023-05-21 20:27:10.000000 ondewo-vtsi-client-6.1.0/ondewo/vtsi/projects_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 20:27:27.082217 ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9088 2023-05-21 20:27:27.000000 ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-05-21 20:27:27.000000 ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 20:27:27.000000 ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-21 20:27:27.000000 ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-21 20:27:27.000000 ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-05-21 20:27:27.082217 ondewo-vtsi-client-6.1.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1586 2023-05-21 20:27:15.000000 ondewo-vtsi-client-6.1.0/setup.py
```

### Comparing `ondewo-vtsi-client-6.0.0/LICENSE` & `ondewo-vtsi-client-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/PKG-INFO` & `ondewo-vtsi-client-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-vtsi-client
-Version: 6.0.0
+Version: 6.1.0
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
-Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.0.0 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.1.0 Summary: exposes
 the ondewo-vtsi endpoints in a user-friendly way Home-page: https://github.com/
 ondewo/ondewo-vtsi-client-python Author: Ondewo GbmH Author-email:
 office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3.8 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Software Development :: Libraries Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-vtsi-client-6.0.0/README.md` & `ondewo-vtsi-client-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/agent_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/agent_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/aiservices_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/aiservices_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/aiservices_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/aiservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/common_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/context_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/context_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/context_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/context_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/entity_type_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/entity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/entity_type_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/entity_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/intent_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/intent_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/intent_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/intent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/operation_metadata_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/operation_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/operations_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/operations_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/project_role_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/project_role_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/project_role_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/project_role_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/project_statistics_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/project_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/project_statistics_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/project_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/server_statistics_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/server_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/server_statistics_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/server_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/session_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/session_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/session_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/user_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/user_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/user_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/utility_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/utility_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/utility_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/utility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/webhook_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/webhook_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/nlu/webhook_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/nlu/webhook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/qa/qa_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/qa/qa_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/qa/qa_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/qa/qa_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/s2t/speech_to_text_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/s2t/speech_to_text_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/s2t/speech_to_text_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/s2t/speech_to_text_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/sip/sip_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/sip/sip_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/sip/sip_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/sip/sip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/t2s/text_to_speech_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/t2s/text_to_speech_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/t2s/text_to_speech_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/t2s/text_to_speech_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/vtsi/calls_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/vtsi/calls_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/vtsi/calls_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/vtsi/calls_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/client.py` & `ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/services/calls.py` & `ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services/calls.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/services/projects.py` & `ondewo-vtsi-client-6.1.0/ondewo/vtsi/client/services/projects.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/vtsi/projects_pb2.py` & `ondewo-vtsi-client-6.1.0/ondewo/vtsi/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo/vtsi/projects_pb2_grpc.py` & `ondewo-vtsi-client-6.1.0/ondewo/vtsi/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/PKG-INFO` & `ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-vtsi-client
-Version: 6.0.0
+Version: 6.1.0
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
-Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.0.0 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.1.0 Summary: exposes
 the ondewo-vtsi endpoints in a user-friendly way Home-page: https://github.com/
 ondewo/ondewo-vtsi-client-python Author: Ondewo GbmH Author-email:
 office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3.8 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Software Development :: Libraries Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/SOURCES.txt` & `ondewo-vtsi-client-6.1.0/ondewo_vtsi_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.0.0/setup.py` & `ondewo-vtsi-client-6.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             req_str = f"{req_name} @ {req_url}"
         else:
             req_str = req
         requires.append(req_str)
 
 setup(
     name="ondewo-vtsi-client",
-    version='6.0.0',
+    version='6.1.0',
     author="Ondewo GbmH",
     author_email="office@ondewo.com",
     description="exposes the ondewo-vtsi endpoints in a user-friendly way",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ondewo/ondewo-vtsi-client-python",
     packages=[
```

