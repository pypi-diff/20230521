# Comparing `tmp/ondewo-vtsi-client-5.0.0.tar.gz` & `tmp/ondewo-vtsi-client-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-vtsi-client-5.0.0.tar", last modified: Thu Sep 15 11:08:04 2022, max compression
+gzip compressed data, was "ondewo-vtsi-client-6.0.0.tar", last modified: Sun May 21 19:37:12 2023, max compression
```

## Comparing `ondewo-vtsi-client-5.0.0.tar` & `ondewo-vtsi-client-6.0.0.tar`

### file list

```diff
@@ -1,68 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:08:04.716412 ondewo-vtsi-client-5.0.0/
--rw-rw-r--   0 root         (0) root         (0)    10257 2022-09-15 11:07:17.000000 ondewo-vtsi-client-5.0.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2022-09-15 11:07:17.000000 ondewo-vtsi-client-5.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1858 2022-09-15 11:08:04.716412 ondewo-vtsi-client-5.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1291 2022-09-15 11:07:17.000000 ondewo-vtsi-client-5.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:08:04.704412 ondewo-vtsi-client-5.0.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-15 11:07:17.000000 ondewo-vtsi-client-5.0.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:08:04.712412 ondewo-vtsi-client-5.0.0/ondewo/nlu/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-15 11:07:17.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    68859 2022-09-15 11:07:52.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/agent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    85379 2022-09-15 11:07:52.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/agent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    28680 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/aiservices_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16812 2022-09-15 11:07:52.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/aiservices_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     1600 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/common_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      158 2022-09-15 11:07:50.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/common_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    10369 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/context_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    14789 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/context_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    27186 2022-09-15 11:07:52.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/entity_type_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    28789 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/entity_type_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    71972 2022-09-15 11:07:53.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/intent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    59591 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/intent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3294 2022-09-15 11:07:50.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/operation_metadata_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      158 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/operation_metadata_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7908 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/operations_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    11373 2022-09-15 11:07:52.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/operations_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     9554 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/project_role_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    10650 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/project_role_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7470 2022-09-15 11:07:50.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/project_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16556 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/project_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3009 2022-09-15 11:07:50.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/server_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     6727 2022-09-15 11:07:50.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/server_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    35177 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/session_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    29018 2022-09-15 11:07:52.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/session_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    19689 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/user_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    27587 2022-09-15 11:07:52.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/user_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    20239 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/utility_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16902 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/utility_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     6369 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/webhook_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     6507 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/nlu/webhook_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:08:04.712412 ondewo-vtsi-client-5.0.0/ondewo/qa/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-15 11:07:17.000000 ondewo-vtsi-client-5.0.0/ondewo/qa/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11457 2022-09-15 11:07:52.000000 ondewo-vtsi-client-5.0.0/ondewo/qa/qa_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    13320 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/qa/qa_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:08:04.712412 ondewo-vtsi-client-5.0.0/ondewo/s2t/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-15 11:07:17.000000 ondewo-vtsi-client-5.0.0/ondewo/s2t/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    35052 2022-09-15 11:07:52.000000 ondewo-vtsi-client-5.0.0/ondewo/s2t/speech_to_text_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    30994 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/s2t/speech_to_text_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:08:04.712412 ondewo-vtsi-client-5.0.0/ondewo/sip/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-15 11:07:17.000000 ondewo-vtsi-client-5.0.0/ondewo/sip/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10727 2022-09-15 11:07:52.000000 ondewo-vtsi-client-5.0.0/ondewo/sip/sip_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    20740 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/sip/sip_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:08:04.716412 ondewo-vtsi-client-5.0.0/ondewo/t2s/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-15 11:07:17.000000 ondewo-vtsi-client-5.0.0/ondewo/t2s/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    31414 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/t2s/text_to_speech_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    33144 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/t2s/text_to_speech_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:08:04.716412 ondewo-vtsi-client-5.0.0/ondewo/vtsi/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-15 11:07:17.000000 ondewo-vtsi-client-5.0.0/ondewo/vtsi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5491 2022-09-15 11:07:17.000000 ondewo-vtsi-client-5.0.0/ondewo/vtsi/client.py
--rw-rw-r--   0 root         (0) root         (0)    41672 2022-09-15 11:07:52.000000 ondewo-vtsi-client-5.0.0/ondewo/vtsi/voip_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    32104 2022-09-15 11:07:51.000000 ondewo-vtsi-client-5.0.0/ondewo/vtsi/voip_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 11:08:04.716412 ondewo-vtsi-client-5.0.0/ondewo_vtsi_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1858 2022-09-15 11:08:04.000000 ondewo-vtsi-client-5.0.0/ondewo_vtsi_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1660 2022-09-15 11:08:04.000000 ondewo-vtsi-client-5.0.0/ondewo_vtsi_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-15 11:08:04.000000 ondewo-vtsi-client-5.0.0/ondewo_vtsi_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      198 2022-09-15 11:08:04.000000 ondewo-vtsi-client-5.0.0/ondewo_vtsi_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-09-15 11:08:04.000000 ondewo-vtsi-client-5.0.0/ondewo_vtsi_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2022-09-15 11:08:04.720412 ondewo-vtsi-client-5.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1225 2022-09-15 11:07:49.000000 ondewo-vtsi-client-5.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.332427 ondewo-vtsi-client-6.0.0/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9088 2023-05-21 19:37:12.332427 ondewo-vtsi-client-6.0.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8516 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.327427 ondewo-vtsi-client-6.0.0/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.330427 ondewo-vtsi-client-6.0.0/ondewo/nlu/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    73579 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/agent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    87204 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/agent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    28729 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/aiservices_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16826 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/aiservices_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     1600 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/common_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/common_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    10375 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/context_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    14789 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/context_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    29954 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/entity_type_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    36069 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/entity_type_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    72044 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/intent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    59591 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/intent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3366 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/operation_metadata_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/operation_metadata_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7908 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/operations_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    11374 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/operations_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     9554 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/project_role_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    10478 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/project_role_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7470 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/project_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16562 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/project_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3009 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/server_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     6634 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/server_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    66065 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/session_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    59122 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/session_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    19689 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/user_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    27124 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/user_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    20239 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/utility_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16902 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/utility_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     6369 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/webhook_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     6508 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/nlu/webhook_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.330427 ondewo-vtsi-client-6.0.0/ondewo/qa/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/qa/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11457 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/qa/qa_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    13389 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/qa/qa_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.330427 ondewo-vtsi-client-6.0.0/ondewo/s2t/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/s2t/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    38634 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/s2t/speech_to_text_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    30933 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/s2t/speech_to_text_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.330427 ondewo-vtsi-client-6.0.0/ondewo/sip/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/sip/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10727 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/sip/sip_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    20740 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/sip/sip_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.331427 ondewo-vtsi-client-6.0.0/ondewo/t2s/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/t2s/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    31414 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/t2s/text_to_speech_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    33144 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/t2s/text_to_speech_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.331427 ondewo-vtsi-client-6.0.0/ondewo/vtsi/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    42878 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/calls_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    29068 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/calls_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.331427 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      735 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      263 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.332427 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3734 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/services/calls.py
+-rw-rw-r--   0 root         (0) root         (0)     2153 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/services/projects.py
+-rw-rw-r--   0 root         (0) root         (0)      317 2023-05-21 19:35:42.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    13169 2023-05-21 19:36:56.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/projects_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    12545 2023-05-21 19:36:55.000000 ondewo-vtsi-client-6.0.0/ondewo/vtsi/projects_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:37:12.332427 ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9088 2023-05-21 19:37:12.000000 ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-05-21 19:37:12.000000 ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 19:37:12.000000 ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-21 19:37:12.000000 ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-21 19:37:12.000000 ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-05-21 19:37:12.333427 ondewo-vtsi-client-6.0.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1586 2023-05-21 19:37:00.000000 ondewo-vtsi-client-6.0.0/setup.py
```

### Comparing `ondewo-vtsi-client-5.0.0/LICENSE` & `ondewo-vtsi-client-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/agent_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/agent_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ondewo/nlu/agent.proto
 """Generated protocol buffer code."""
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from ondewo.nlu import session_pb2 as ondewo_dot_nlu_dot_session__pb2
 from ondewo.nlu import operations_pb2 as ondewo_dot_nlu_dot_operations__pb2
 from ondewo.nlu import project_role_pb2 as ondewo_dot_nlu_dot_project__role__pb2
 from ondewo.nlu import user_pb2 as ondewo_dot_nlu_dot_user__pb2
 from ondewo.nlu import intent_pb2 as ondewo_dot_nlu_dot_intent__pb2
 from ondewo.nlu import common_pb2 as ondewo_dot_nlu_dot_common__pb2
-from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
@@ -20,37 +20,58 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16ondewo/nlu/agent.proto\x12\nondewo.nlu\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x19google/protobuf/any.proto\x1a\x17ondewo/nlu/common.proto\x1a\x17ondewo/nlu/intent.proto\x1a\x15ondewo/nlu/user.proto\x1a\x1dondewo/nlu/project_role.proto\x1a\x1bondewo/nlu/operations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x91\x02\n\x05\x41gent\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x1d\n\x15\x64\x65\x66\x61ult_language_code\x18\x03 \x01(\t\x12 \n\x18supported_language_codes\x18\x04 \x03(\t\x12\x11\n\ttime_zone\x18\x05 \x01(\t\x12\x14\n\x0cnlu_platform\x18\x06 \x01(\t\x12(\n\x07\x63onfigs\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x10\n\x08owner_id\x18\x08 \x01(\t\x12\'\n\x06status\x18\t \x01(\x0e\x32\x17.ondewo.nlu.AgentStatus\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\"S\n\x0e\x41gentWithOwner\x12 \n\x05\x61gent\x18\x01 \x01(\x0b\x32\x11.ondewo.nlu.Agent\x12\x1f\n\x05owner\x18\x02 \x01(\x0b\x32\x10.ondewo.nlu.User\"{\n\x14\x41gentOfUserWithOwner\x12\x34\n\x10\x61gent_with_owner\x18\x01 \x01(\x0b\x32\x1a.ondewo.nlu.AgentWithOwner\x12-\n\x0cproject_role\x18\x02 \x01(\x0b\x32\x17.ondewo.nlu.ProjectRole\"a\n\x12\x43reateAgentRequest\x12 \n\x05\x61gent\x18\x01 \x01(\x0b\x32\x11.ondewo.nlu.Agent\x12)\n\nagent_view\x18\x02 \x01(\x0e\x32\x15.ondewo.nlu.AgentView\"\x92\x01\n\x12UpdateAgentRequest\x12 \n\x05\x61gent\x18\x01 \x01(\x0b\x32\x11.ondewo.nlu.Agent\x12)\n\nagent_view\x18\x02 \x01(\x0e\x32\x15.ondewo.nlu.AgentView\x12/\n\x0bupdate_mask\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"$\n\x12\x44\x65leteAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\"L\n\x0fGetAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12)\n\nagent_view\x18\x02 \x01(\x0e\x32\x15.ondewo.nlu.AgentView\"\x83\x01\n\x11ListAgentsRequest\x12)\n\nagent_view\x18\x01 \x01(\x0e\x32\x15.ondewo.nlu.AgentView\x12\x12\n\npage_token\x18\x02 \x01(\t\x12/\n\rsort_by_field\x18\x03 \x01(\x0b\x32\x18.ondewo.nlu.AgentSorting\"e\n\x12ListAgentsResponse\x12\x36\n\x12\x61gents_with_owners\x18\x01 \x03(\x0b\x32\x1a.ondewo.nlu.AgentWithOwner\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"y\n\x18ListAgentsOfUserResponse\x12\x44\n\x1a\x61gents_of_user_with_owners\x18\x01 \x03(\x0b\x32 .ondewo.nlu.AgentOfUserWithOwner\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"p\n\x11TrainAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\x12;\n\x13initiation_protocol\x18\x03 \x01(\x0e\x32\x1e.ondewo.nlu.InitiationProtocol\"3\n\x11\x42uildCacheRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\"R\n\x12\x45xportAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x11\n\tagent_uri\x18\x02 \x01(\t\x12\x19\n\x11\x63ompression_level\x18\x03 \x01(\x05\"L\n\x13\x45xportAgentResponse\x12\x13\n\tagent_uri\x18\x01 \x01(\tH\x00\x12\x17\n\ragent_content\x18\x02 \x01(\x0cH\x00\x42\x07\n\x05\x61gent\"\x85\x01\n\x1b\x45xportBenchmarkAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x19\n\x11\x63ompression_level\x18\x02 \x01(\x05\x12\x11\n\ttest_size\x18\x03 \x01(\x02\x12\x12\n\ntrain_size\x18\x04 \x01(\x02\x12\x14\n\x0crandom_state\x18\x05 \x01(\x05\"\xef\x01\n\x1c\x45xportBenchmarkAgentResponse\x12\x15\n\ragent_content\x18\x01 \x01(\x0c\x12W\n\x10training_phrases\x18\x02 \x03(\x0b\x32=.ondewo.nlu.ExportBenchmarkAgentResponse.TrainingPhrasesEntry\x1a_\n\x14TrainingPhrasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.ondewo.nlu.ListTrainingPhrasesResponse:\x02\x38\x01\"\xa1\x01\n\x1bOptimizeRankingMatchRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x16\n\x0elanguage_codes\x18\x02 \x03(\t\x12H\n\x14optimization_configs\x18\x03 \x03(\x0b\x32*.ondewo.nlu.RankingMatchOptimizationConfig\x12\x10\n\x08in_place\x18\x04 \x01(\x08\"\x93\x01\n\x1eRankingMatchOptimizationConfig\x12\x15\n\rlanguage_code\x18\x01 \x01(\t\x12\x10\n\x08n_splits\x18\x02 \x01(\x05\x12\x13\n\x0brandom_seed\x18\x03 \x01(\x05\x12\x33\n\x12initial_thresholds\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x8c\x01\n\x1cOptimizeRankingMatchResponse\x12\x32\n\x11optimization_info\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x38\n\x17optimized_ondewo_config\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\"[\n\x12ImportAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x13\n\tagent_uri\x18\x02 \x01(\tH\x00\x12\x17\n\ragent_content\x18\x03 \x01(\x0cH\x00\x42\x07\n\x05\x61gent\"\\\n\x13RestoreAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x13\n\tagent_uri\x18\x02 \x01(\tH\x00\x12\x17\n\ragent_content\x18\x03 \x01(\x0cH\x00\x42\x07\n\x05\x61gent\"\x92\x01\n\x19GetAgentStatisticsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12(\n\x06\x66ormat\x18\x02 \x01(\x0e\x32\x18.ondewo.nlu.ReportFormat\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12$\n\x04type\x18\x04 \x01(\x0e\x32\x16.ondewo.nlu.ReportType\"}\n\x1aGetAgentStatisticsResponse\x12\x0f\n\x07reports\x18\x01 \x01(\x0c\x12(\n\x06\x66ormat\x18\x02 \x01(\x0e\x32\x18.ondewo.nlu.ReportFormat\x12$\n\x04type\x18\x03 \x01(\x0e\x32\x16.ondewo.nlu.ReportType\"S\n\x17\x41\x64\x64UserToProjectRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x02 \x01(\t\x12\x17\n\x0fproject_role_id\x18\x04 \x01(\r\"?\n\x1cRemoveUserFromProjectRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x02 \x01(\t\"?\n\x19ListUsersInProjectRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x12\n\npage_token\x18\x02 \x01(\t\"P\n\rUserInProject\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x1e\n\x04user\x18\x02 \x01(\x0b\x32\x10.ondewo.nlu.User\x12\x0f\n\x07role_id\x18\x03 \x01(\r\"_\n\x1aListUsersInProjectResponse\x12(\n\x05users\x18\x01 \x03(\x0b\x32\x19.ondewo.nlu.UserInProject\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"?\n\x17GetPlatformInfoResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0b\x63ommit_hash\x18\x02 \x01(\t\"3\n\x1dListProjectPermissionsRequest\x12\x12\n\npage_token\x18\x01 \x01(\t\"N\n\x1eListProjectPermissionsResponse\x12\x13\n\x0bpermissions\x18\x01 \x03(\t\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"{\n\x15SetAgentStatusRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\'\n\x06status\x18\x02 \x01(\x0e\x32\x17.ondewo.nlu.AgentStatus\x12)\n\nagent_view\x18\x03 \x01(\x0e\x32\x15.ondewo.nlu.AgentView\"\xa3\x02\n\x0c\x41gentSorting\x12\x41\n\rsorting_field\x18\x01 \x01(\x0e\x32*.ondewo.nlu.AgentSorting.AgentSortingField\x12-\n\x0csorting_mode\x18\x02 \x01(\x0e\x32\x17.ondewo.nlu.SortingMode\"\xa0\x01\n\x11\x41gentSortingField\x12\x14\n\x10NO_AGENT_SORTING\x10\x00\x12\x16\n\x12SORT_AGENT_BY_NAME\x10\x01\x12\x1f\n\x1bSORT_AGENT_BY_CREATION_DATE\x10\x02\x12\x1e\n\x1aSORT_AGENT_BY_LAST_UPDATED\x10\x03\x12\x1c\n\x18SORT_AGENT_BY_OWNER_NAME\x10\x04\"o\n\x13SetResourcesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rresource_file\x18\x04 \x01(\x0c\x12\x15\n\rlanguage_code\x18\x05 \x01(\t\"[\n\x16\x44\x65leteResourcesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\"[\n\x16\x45xportResourcesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\"s\n\x17\x45xportResourcesResponse\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x15\n\rresource_file\x18\x05 \x01(\x0c\"k\n\x17GetModelStatusesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rcache_version\x18\x02 \x01(\x05\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12\x12\n\nmodel_name\x18\x04 \x01(\t\"\xc0\x02\n\x0bModelStatus\x12\x15\n\rcache_version\x18\x01 \x01(\x05\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\nmodel_name\x18\x03 \x01(\t\x12\x33\n\x0fstatus_set_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x63onfig\x18\x05 \x01(\t\x12\x32\n\x06status\x18\x06 \x01(\x0e\x32\".ondewo.nlu.ModelStatus.StatusName\"v\n\nStatusName\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0cINITIALIZING\x10\x01\x12\x0f\n\x0bINITIALIZED\x10\x02\x12\x10\n\x0cLOADING_DATA\x10\x03\x12\x0c\n\x08TRAINING\x10\x04\x12\x0b\n\x07TESTING\x10\x05\x12\x0b\n\x07TRAINED\x10\x06\"K\n\x18GetModelStatusesResponse\x12/\n\x0emodel_statuses\x18\x01 \x03(\x0b\x32\x17.ondewo.nlu.ModelStatus\"s\n\x12\x43ustomPlatformInfo\x12\x35\n\x08platform\x18\x01 \x01(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\r\"+\n\x19GetPlatformMappingRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\"X\n\x0fPlatformMapping\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x35\n\rplatform_info\x18\x02 \x03(\x0b\x32\x1e.ondewo.nlu.CustomPlatformInfo\"\x99\x03\n\x15\x46ullTextSearchRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x0c\n\x04term\x18\x03 \x01(\t\x12\x12\n\npage_token\x18\x04 \x01(\t\"\xb6\x02\n\tQueryType\x12\x07\n\x03\x41LL\x10\x00\x12\x15\n\x11OndewoEntityQuery\x10\x01\x12\x19\n\x15OndewoEntityTypeQuery\x10\x02\x12\x1c\n\x18OndewoEntitySynonymQuery\x10\x03\x12\x15\n\x11OndewoIntentQuery\x10\x04\x12\x1e\n\x1aOndewoIntentContextInQuery\x10\x05\x12\x1f\n\x1bOndewoIntentContextOutQuery\x10\x06\x12\x1d\n\x19OndewoIntentUsersaysQuery\x10\x07\x12\x19\n\x15OndewoIntentTagsQuery\x10\x08\x12\x1f\n\x1bOndewoIntentParametersQuery\x10\t\x12\x1d\n\x19OndewoIntentResponseQuery\x10\n\"\xc7\x02\n FullTextSearchResponseEntityType\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12`\n\x13\x65ntity_type_results\x18\x03 \x03(\x0b\x32\x43.ondewo.nlu.FullTextSearchResponseEntityType.EntityTypeSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1aN\n\x16\x45ntityTypeSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x10\n\x08language\x18\x03 \x01(\t\"\xcc\x02\n\x1c\x46ullTextSearchResponseEntity\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12S\n\x0e\x65ntity_results\x18\x03 \x03(\x0b\x32;.ondewo.nlu.FullTextSearchResponseEntity.EntitySearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a\x64\n\x12\x45ntitySearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x18\n\x10\x65ntity_type_name\x18\x03 \x01(\t\x12\x10\n\x08language\x18\x04 \x01(\t\"\x86\x03\n#FullTextSearchResponseEntitySynonym\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12i\n\x16\x65ntity_synonym_results\x18\x03 \x03(\x0b\x32I.ondewo.nlu.FullTextSearchResponseEntitySynonym.EntitySynonymSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a\x80\x01\n\x19\x45ntitySynonymSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x18\n\x10\x65ntity_type_name\x18\x03 \x01(\t\x12\x13\n\x0b\x65ntity_name\x18\x04 \x01(\t\x12\x10\n\x08language\x18\x05 \x01(\t\"\xc7\x02\n\x1c\x46ullTextSearchResponseIntent\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12S\n\x0eintent_results\x18\x03 \x03(\x0b\x32;.ondewo.nlu.FullTextSearchResponseIntent.IntentSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a_\n\x12IntentSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x13\n\x0b\x64omain_name\x18\x03 \x01(\t\x12\x10\n\x08language\x18\x04 \x01(\t\"\xe0\x02\n%FullTextSearchResponseIntentContextIn\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12p\n\x19intent_context_in_results\x18\x03 \x03(\x0b\x32M.ondewo.nlu.FullTextSearchResponseIntentContextIn.IntentContextInSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1aR\n\x1bIntentContextInSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bintent_name\x18\x02 \x01(\t\x12\x10\n\x08language\x18\x03 \x01(\t\"\xe5\x02\n&FullTextSearchResponseIntentContextOut\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12s\n\x1aintent_context_out_results\x18\x03 \x03(\x0b\x32O.ondewo.nlu.FullTextSearchResponseIntentContextOut.IntentContextOutSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1aS\n\x1cIntentContextOutSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bintent_name\x18\x02 \x01(\t\x12\x10\n\x08language\x18\x03 \x01(\t\"\xb4\x03\n$FullTextSearchResponseIntentUsersays\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12l\n\x17intent_usersays_results\x18\x03 \x03(\x0b\x32K.ondewo.nlu.FullTextSearchResponseIntentUsersays.IntentUsersaysSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a\xaa\x01\n\x1aIntentUsersaysSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x1c\n\x14text_as_entity_types\x18\x03 \x01(\t\x12\x1d\n\x15text_as_entity_values\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x13\n\x0bintent_name\x18\x06 \x01(\t\x12\x10\n\x08language\x18\x07 \x01(\t\"\xd4\x02\n FullTextSearchResponseIntentTags\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12`\n\x13intent_tags_results\x18\x03 \x03(\x0b\x32\x43.ondewo.nlu.FullTextSearchResponseIntentTags.IntentTagsSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a[\n\x16IntentTagsSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x13\n\x0bintent_name\x18\x03 \x01(\t\x12\x10\n\x08language\x18\x04 \x01(\t\"\x83\x03\n$FullTextSearchResponseIntentResponse\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12l\n\x17intent_response_results\x18\x03 \x03(\x0b\x32K.ondewo.nlu.FullTextSearchResponseIntentResponse.IntentResponseSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1az\n\x1aIntentResponseSearchResult\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x10\n\x08platform\x18\x02 \x01(\t\x12\x15\n\rresponse_type\x18\x03 \x01(\t\x12\x13\n\x0bintent_name\x18\x04 \x01(\t\x12\x10\n\x08language\x18\x05 \x01(\t\"\x8e\x03\n&FullTextSearchResponseIntentParameters\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12r\n\x19intent_parameters_results\x18\x03 \x03(\x0b\x32O.ondewo.nlu.FullTextSearchResponseIntentParameters.IntentParametersSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a}\n\x1cIntentParametersSearchResult\x12\x16\n\x0eparameter_name\x18\x01 \x01(\t\x12\x1e\n\x16parameter_display_name\x18\x02 \x01(\t\x12\x13\n\x0bintent_name\x18\x03 \x01(\t\x12\x10\n\x08language\x18\x04 \x01(\t\"|\n\x13ReindexAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\t\x12@\n\x0bindex_types\x18\x03 \x03(\x0e\x32+.ondewo.nlu.FullTextSearchRequest.QueryType*T\n\tAgentView\x12\x1a\n\x16\x41GENT_VIEW_UNSPECIFIED\x10\x00\x12\x13\n\x0f\x41GENT_VIEW_FULL\x10\x01\x12\x16\n\x12\x41GENT_VIEW_SHALLOW\x10\x02*J\n\x12InitiationProtocol\x12\x17\n\x13\x41S_SOON_AS_POSSIBLE\x10\x00\x12\x10\n\x0cWHEN_TRAINED\x10\x01\x12\t\n\x05NEVER\x10\x02*q\n\nReportType\x12\x07\n\x03\x41LL\x10\x00\x12\x17\n\x13INTENT_PER_LANGUAGE\x10\x01\x12\x17\n\x13\x45NTITY_PER_LANGUAGE\x10\x02\x12\x14\n\x10\x45NTITY_COLLISION\x10\x03\x12\x12\n\x0eINTENT_GENERAL\x10\x04*+\n\x0cReportFormat\x12\x07\n\x03\x43SV\x10\x00\x12\x08\n\x04HTML\x10\x01\x12\x08\n\x04JSON\x10\x02*\'\n\x0b\x41gentStatus\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08INACTIVE\x10\x01\x32\xe5#\n\x06\x41gents\x12Y\n\x0b\x43reateAgent\x12\x1e.ondewo.nlu.CreateAgentRequest\x1a\x11.ondewo.nlu.Agent\"\x17\x82\xd3\xe4\x93\x02\x11\"\x0c/v2/projects:\x01*\x12p\n\x0bUpdateAgent\x12\x1e.ondewo.nlu.UpdateAgentRequest\x1a\x11.ondewo.nlu.Agent\".\x82\xd3\xe4\x93\x02(2#/v2/{agent.parent=projects/*/agent}:\x01*\x12\x61\n\x08GetAgent\x12\x1b.ondewo.nlu.GetAgentRequest\x1a\x11.ondewo.nlu.Agent\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/v2/{parent=projects/*/agent}\x12l\n\x0b\x44\x65leteAgent\x12\x1e.ondewo.nlu.DeleteAgentRequest\x1a\x16.google.protobuf.Empty\"%\x82\xd3\xe4\x93\x02\x1f*\x1d/v2/{parent=projects/*/agent}\x12W\n\x0f\x44\x65leteAllAgents\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x14\x82\xd3\xe4\x93\x02\x0e*\x0c/v2/projects\x12\x61\n\nListAgents\x12\x1d.ondewo.nlu.ListAgentsRequest\x1a\x1e.ondewo.nlu.ListAgentsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v2/projects\x12m\n\x10ListAgentsOfUser\x12\x1d.ondewo.nlu.ListAgentsRequest\x1a$.ondewo.nlu.ListAgentsOfUserResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v2/projects\x12h\n\rListAllAgents\x12\x1d.ondewo.nlu.ListAgentsRequest\x1a\x1e.ondewo.nlu.ListAgentsResponse\"\x18\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/projects:all\x12\x8b\x01\n\x10\x41\x64\x64UserToProject\x12#.ondewo.nlu.AddUserToProjectRequest\x1a\x16.google.protobuf.Empty\":\x82\xd3\xe4\x93\x02\x34\"//v2/{parent=projects/*/agent}/users/{user_id=*}:\x01*\x12\x92\x01\n\x15RemoveUserFromProject\x12(.ondewo.nlu.RemoveUserFromProjectRequest\x1a\x16.google.protobuf.Empty\"7\x82\xd3\xe4\x93\x02\x31*//v2/{parent=projects/*/agent}/users/{user_id=*}\x12\x90\x01\n\x12ListUsersInProject\x12%.ondewo.nlu.ListUsersInProjectRequest\x1a&.ondewo.nlu.ListUsersInProjectResponse\"+\x82\xd3\xe4\x93\x02%\x12#/v2/{parent=projects/*/agent}/users\x12\x63\n\x0fGetPlatformInfo\x12\x16.google.protobuf.Empty\x1a#.ondewo.nlu.GetPlatformInfoResponse\"\x13\x82\xd3\xe4\x93\x02\r\x12\x0b/v2/version\x12\x90\x01\n\x16ListProjectPermissions\x12).ondewo.nlu.ListProjectPermissionsRequest\x1a*.ondewo.nlu.ListProjectPermissionsResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/v2/project_permissions\x12r\n\nTrainAgent\x12\x1d.ondewo.nlu.TrainAgentRequest\x1a\x15.ondewo.nlu.Operation\".\x82\xd3\xe4\x93\x02(\"#/v2/{parent=projects/*/agent}:train:\x01*\x12x\n\nBuildCache\x12\x1d.ondewo.nlu.BuildCacheRequest\x1a\x15.ondewo.nlu.Operation\"4\x82\xd3\xe4\x93\x02.\")/v2/{parent=projects/*/agent}:build_cache:\x01*\x12u\n\x0b\x45xportAgent\x12\x1e.ondewo.nlu.ExportAgentRequest\x1a\x15.ondewo.nlu.Operation\"/\x82\xd3\xe4\x93\x02)\"$/v2/{parent=projects/*/agent}:export:\x01*\x12\x91\x01\n\x14\x45xportBenchmarkAgent\x12\'.ondewo.nlu.ExportBenchmarkAgentRequest\x1a\x15.ondewo.nlu.Operation\"9\x82\xd3\xe4\x93\x02\x33\"./v2/{parent=projects/*/agent}:export_benchmark:\x01*\x12u\n\x0bImportAgent\x12\x1e.ondewo.nlu.ImportAgentRequest\x1a\x15.ondewo.nlu.Operation\"/\x82\xd3\xe4\x93\x02)\"$/v2/{parent=projects/*/agent}:import:\x01*\x12\x97\x01\n\x14OptimizeRankingMatch\x12\'.ondewo.nlu.OptimizeRankingMatchRequest\x1a\x15.ondewo.nlu.Operation\"?\x82\xd3\xe4\x93\x02\x39\"4/v2/{parent=projects/*/agent}:optimize_ranking_match:\x01*\x12x\n\x0cRestoreAgent\x12\x1f.ondewo.nlu.RestoreAgentRequest\x1a\x15.ondewo.nlu.Operation\"0\x82\xd3\xe4\x93\x02*\"%/v2/{parent=projects/*/agent}:restore:\x01*\x12\x95\x01\n\x12GetAgentStatistics\x12%.ondewo.nlu.GetAgentStatisticsRequest\x1a&.ondewo.nlu.GetAgentStatisticsResponse\"0\x82\xd3\xe4\x93\x02*\x12(/v2/{parent=projects/*/agent}:statistics\x12w\n\x0eSetAgentStatus\x12!.ondewo.nlu.SetAgentStatusRequest\x1a\x11.ondewo.nlu.Agent\"/\x82\xd3\xe4\x93\x02)\"$/v2/{parent=projects/*/agent}:status:\x01*\x12{\n\x0cSetResources\x12\x1f.ondewo.nlu.SetResourcesRequest\x1a\x16.google.protobuf.Empty\"2\x82\xd3\xe4\x93\x02,\"\'/v2/{parent=projects/*/agent}:resources:\x01*\x12~\n\x0f\x44\x65leteResources\x12\".ondewo.nlu.DeleteResourcesRequest\x1a\x16.google.protobuf.Empty\"/\x82\xd3\xe4\x93\x02)*\'/v2/{parent=projects/*/agent}:resources\x12\x8e\x01\n\x0f\x45xportResources\x12\".ondewo.nlu.ExportResourcesRequest\x1a#.ondewo.nlu.ExportResourcesResponse\"2\x82\xd3\xe4\x93\x02,\"\'/v2/{parent=projects/*/agent}:resources:\x01*\x12]\n\x10GetModelStatuses\x12#.ondewo.nlu.GetModelStatusesRequest\x1a$.ondewo.nlu.GetModelStatusesResponse\x12X\n\x12GetPlatformMapping\x12%.ondewo.nlu.GetPlatformMappingRequest\x1a\x1b.ondewo.nlu.PlatformMapping\x12N\n\x12SetPlatformMapping\x12\x1b.ondewo.nlu.PlatformMapping\x1a\x1b.ondewo.nlu.PlatformMapping\x12n\n\x1bGetFullTextSearchEntityType\x12!.ondewo.nlu.FullTextSearchRequest\x1a,.ondewo.nlu.FullTextSearchResponseEntityType\x12\x66\n\x17GetFullTextSearchEntity\x12!.ondewo.nlu.FullTextSearchRequest\x1a(.ondewo.nlu.FullTextSearchResponseEntity\x12t\n\x1eGetFullTextSearchEntitySynonym\x12!.ondewo.nlu.FullTextSearchRequest\x1a/.ondewo.nlu.FullTextSearchResponseEntitySynonym\x12\x66\n\x17GetFullTextSearchIntent\x12!.ondewo.nlu.FullTextSearchRequest\x1a(.ondewo.nlu.FullTextSearchResponseIntent\x12x\n GetFullTextSearchIntentContextIn\x12!.ondewo.nlu.FullTextSearchRequest\x1a\x31.ondewo.nlu.FullTextSearchResponseIntentContextIn\x12z\n!GetFullTextSearchIntentContextOut\x12!.ondewo.nlu.FullTextSearchRequest\x1a\x32.ondewo.nlu.FullTextSearchResponseIntentContextOut\x12v\n\x1fGetFullTextSearchIntentUsersays\x12!.ondewo.nlu.FullTextSearchRequest\x1a\x30.ondewo.nlu.FullTextSearchResponseIntentUsersays\x12n\n\x1bGetFullTextSearchIntentTags\x12!.ondewo.nlu.FullTextSearchRequest\x1a,.ondewo.nlu.FullTextSearchResponseIntentTags\x12v\n\x1fGetFullTextSearchIntentResponse\x12!.ondewo.nlu.FullTextSearchRequest\x1a\x30.ondewo.nlu.FullTextSearchResponseIntentResponse\x12z\n!GetFullTextSearchIntentParameters\x12!.ondewo.nlu.FullTextSearchRequest\x1a\x32.ondewo.nlu.FullTextSearchResponseIntentParameters\x12\x46\n\x0cReindexAgent\x12\x1f.ondewo.nlu.ReindexAgentRequest\x1a\x15.ondewo.nlu.Operationb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16ondewo/nlu/agent.proto\x12\nondewo.nlu\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x17ondewo/nlu/common.proto\x1a\x17ondewo/nlu/intent.proto\x1a\x15ondewo/nlu/user.proto\x1a\x1dondewo/nlu/project_role.proto\x1a\x1bondewo/nlu/operations.proto\x1a\x18ondewo/nlu/session.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x91\x02\n\x05\x41gent\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x1d\n\x15\x64\x65\x66\x61ult_language_code\x18\x03 \x01(\t\x12 \n\x18supported_language_codes\x18\x04 \x03(\t\x12\x11\n\ttime_zone\x18\x05 \x01(\t\x12\x14\n\x0cnlu_platform\x18\x06 \x01(\t\x12(\n\x07\x63onfigs\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x10\n\x08owner_id\x18\x08 \x01(\t\x12\'\n\x06status\x18\t \x01(\x0e\x32\x17.ondewo.nlu.AgentStatus\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\"S\n\x0e\x41gentWithOwner\x12 \n\x05\x61gent\x18\x01 \x01(\x0b\x32\x11.ondewo.nlu.Agent\x12\x1f\n\x05owner\x18\x02 \x01(\x0b\x32\x10.ondewo.nlu.User\"{\n\x14\x41gentOfUserWithOwner\x12\x34\n\x10\x61gent_with_owner\x18\x01 \x01(\x0b\x32\x1a.ondewo.nlu.AgentWithOwner\x12-\n\x0cproject_role\x18\x02 \x01(\x0b\x32\x17.ondewo.nlu.ProjectRole\"a\n\x12\x43reateAgentRequest\x12 \n\x05\x61gent\x18\x01 \x01(\x0b\x32\x11.ondewo.nlu.Agent\x12)\n\nagent_view\x18\x02 \x01(\x0e\x32\x15.ondewo.nlu.AgentView\"\x92\x01\n\x12UpdateAgentRequest\x12 \n\x05\x61gent\x18\x01 \x01(\x0b\x32\x11.ondewo.nlu.Agent\x12)\n\nagent_view\x18\x02 \x01(\x0e\x32\x15.ondewo.nlu.AgentView\x12/\n\x0bupdate_mask\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"$\n\x12\x44\x65leteAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\"L\n\x0fGetAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12)\n\nagent_view\x18\x02 \x01(\x0e\x32\x15.ondewo.nlu.AgentView\"\x83\x01\n\x11ListAgentsRequest\x12)\n\nagent_view\x18\x01 \x01(\x0e\x32\x15.ondewo.nlu.AgentView\x12\x12\n\npage_token\x18\x02 \x01(\t\x12/\n\rsort_by_field\x18\x03 \x01(\x0b\x32\x18.ondewo.nlu.AgentSorting\"e\n\x12ListAgentsResponse\x12\x36\n\x12\x61gents_with_owners\x18\x01 \x03(\x0b\x32\x1a.ondewo.nlu.AgentWithOwner\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"y\n\x18ListAgentsOfUserResponse\x12\x44\n\x1a\x61gents_of_user_with_owners\x18\x01 \x03(\x0b\x32 .ondewo.nlu.AgentOfUserWithOwner\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"p\n\x11TrainAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\x12;\n\x13initiation_protocol\x18\x03 \x01(\x0e\x32\x1e.ondewo.nlu.InitiationProtocol\"3\n\x11\x42uildCacheRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\"R\n\x12\x45xportAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x11\n\tagent_uri\x18\x02 \x01(\t\x12\x19\n\x11\x63ompression_level\x18\x03 \x01(\x05\"L\n\x13\x45xportAgentResponse\x12\x13\n\tagent_uri\x18\x01 \x01(\tH\x00\x12\x17\n\ragent_content\x18\x02 \x01(\x0cH\x00\x42\x07\n\x05\x61gent\"\x85\x01\n\x1b\x45xportBenchmarkAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x19\n\x11\x63ompression_level\x18\x02 \x01(\x05\x12\x11\n\ttest_size\x18\x03 \x01(\x02\x12\x12\n\ntrain_size\x18\x04 \x01(\x02\x12\x14\n\x0crandom_state\x18\x05 \x01(\x05\"\xef\x01\n\x1c\x45xportBenchmarkAgentResponse\x12\x15\n\ragent_content\x18\x01 \x01(\x0c\x12W\n\x10training_phrases\x18\x02 \x03(\x0b\x32=.ondewo.nlu.ExportBenchmarkAgentResponse.TrainingPhrasesEntry\x1a_\n\x14TrainingPhrasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.ondewo.nlu.ListTrainingPhrasesResponse:\x02\x38\x01\"\xa1\x01\n\x1bOptimizeRankingMatchRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x16\n\x0elanguage_codes\x18\x02 \x03(\t\x12H\n\x14optimization_configs\x18\x03 \x03(\x0b\x32*.ondewo.nlu.RankingMatchOptimizationConfig\x12\x10\n\x08in_place\x18\x04 \x01(\x08\"\x93\x01\n\x1eRankingMatchOptimizationConfig\x12\x15\n\rlanguage_code\x18\x01 \x01(\t\x12\x10\n\x08n_splits\x18\x02 \x01(\x05\x12\x13\n\x0brandom_seed\x18\x03 \x01(\x05\x12\x33\n\x12initial_thresholds\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x8c\x01\n\x1cOptimizeRankingMatchResponse\x12\x32\n\x11optimization_info\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x38\n\x17optimized_ondewo_config\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\"[\n\x12ImportAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x13\n\tagent_uri\x18\x02 \x01(\tH\x00\x12\x17\n\ragent_content\x18\x03 \x01(\x0cH\x00\x42\x07\n\x05\x61gent\"\\\n\x13RestoreAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x13\n\tagent_uri\x18\x02 \x01(\tH\x00\x12\x17\n\ragent_content\x18\x03 \x01(\x0cH\x00\x42\x07\n\x05\x61gent\"\x92\x01\n\x19GetAgentStatisticsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12(\n\x06\x66ormat\x18\x02 \x01(\x0e\x32\x18.ondewo.nlu.ReportFormat\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12$\n\x04type\x18\x04 \x01(\x0e\x32\x16.ondewo.nlu.ReportType\"}\n\x1aGetAgentStatisticsResponse\x12\x0f\n\x07reports\x18\x01 \x01(\x0c\x12(\n\x06\x66ormat\x18\x02 \x01(\x0e\x32\x18.ondewo.nlu.ReportFormat\x12$\n\x04type\x18\x03 \x01(\x0e\x32\x16.ondewo.nlu.ReportType\"\xe5\x02\n\x1cGetSessionsStatisticsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12(\n\x06\x66ormat\x18\x02 \x01(\x0e\x32\x18.ondewo.nlu.ReportFormat\x12,\n\x04type\x18\x03 \x01(\x0e\x32\x1e.ondewo.nlu.SessionsReportType\x12\x31\n\x0esession_filter\x18\x04 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\x12\x32\n\x0f\x63ontext_filters\x18\x05 \x03(\x0b\x32\x19.ondewo.nlu.ContextFilter\x12\r\n\x05limit\x18\x06 \x01(\x05\x12\x11\n\tgroup_bys\x18\x07 \x03(\t\x12\x11\n\torder_bys\x18\x08 \x03(\t\x12.\n\nfield_mask\x18\t \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12\x11\n\tsql_query\x18\n \x01(\t\"\x88\x01\n\x1dGetSessionsStatisticsResponse\x12\x0f\n\x07reports\x18\x01 \x01(\x0c\x12(\n\x06\x66ormat\x18\x02 \x01(\x0e\x32\x18.ondewo.nlu.ReportFormat\x12,\n\x04type\x18\x03 \x01(\x0e\x32\x1e.ondewo.nlu.SessionsReportType\"S\n\x17\x41\x64\x64UserToProjectRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x02 \x01(\t\x12\x17\n\x0fproject_role_id\x18\x04 \x01(\r\"?\n\x1cRemoveUserFromProjectRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x02 \x01(\t\"?\n\x19ListUsersInProjectRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x12\n\npage_token\x18\x02 \x01(\t\"P\n\rUserInProject\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x1e\n\x04user\x18\x02 \x01(\x0b\x32\x10.ondewo.nlu.User\x12\x0f\n\x07role_id\x18\x03 \x01(\r\"_\n\x1aListUsersInProjectResponse\x12(\n\x05users\x18\x01 \x03(\x0b\x32\x19.ondewo.nlu.UserInProject\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"?\n\x17GetPlatformInfoResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0b\x63ommit_hash\x18\x02 \x01(\t\"3\n\x1dListProjectPermissionsRequest\x12\x12\n\npage_token\x18\x01 \x01(\t\"N\n\x1eListProjectPermissionsResponse\x12\x13\n\x0bpermissions\x18\x01 \x03(\t\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"{\n\x15SetAgentStatusRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\'\n\x06status\x18\x02 \x01(\x0e\x32\x17.ondewo.nlu.AgentStatus\x12)\n\nagent_view\x18\x03 \x01(\x0e\x32\x15.ondewo.nlu.AgentView\"\xa3\x02\n\x0c\x41gentSorting\x12\x41\n\rsorting_field\x18\x01 \x01(\x0e\x32*.ondewo.nlu.AgentSorting.AgentSortingField\x12-\n\x0csorting_mode\x18\x02 \x01(\x0e\x32\x17.ondewo.nlu.SortingMode\"\xa0\x01\n\x11\x41gentSortingField\x12\x14\n\x10NO_AGENT_SORTING\x10\x00\x12\x16\n\x12SORT_AGENT_BY_NAME\x10\x01\x12\x1f\n\x1bSORT_AGENT_BY_CREATION_DATE\x10\x02\x12\x1e\n\x1aSORT_AGENT_BY_LAST_UPDATED\x10\x03\x12\x1c\n\x18SORT_AGENT_BY_OWNER_NAME\x10\x04\"o\n\x13SetResourcesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rresource_file\x18\x04 \x01(\x0c\x12\x15\n\rlanguage_code\x18\x05 \x01(\t\"[\n\x16\x44\x65leteResourcesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\"[\n\x16\x45xportResourcesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\"s\n\x17\x45xportResourcesResponse\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x15\n\rresource_file\x18\x05 \x01(\x0c\"k\n\x17GetModelStatusesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rcache_version\x18\x02 \x01(\x05\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12\x12\n\nmodel_name\x18\x04 \x01(\t\"\xc0\x02\n\x0bModelStatus\x12\x15\n\rcache_version\x18\x01 \x01(\x05\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\nmodel_name\x18\x03 \x01(\t\x12\x33\n\x0fstatus_set_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x63onfig\x18\x05 \x01(\t\x12\x32\n\x06status\x18\x06 \x01(\x0e\x32\".ondewo.nlu.ModelStatus.StatusName\"v\n\nStatusName\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0cINITIALIZING\x10\x01\x12\x0f\n\x0bINITIALIZED\x10\x02\x12\x10\n\x0cLOADING_DATA\x10\x03\x12\x0c\n\x08TRAINING\x10\x04\x12\x0b\n\x07TESTING\x10\x05\x12\x0b\n\x07TRAINED\x10\x06\"K\n\x18GetModelStatusesResponse\x12/\n\x0emodel_statuses\x18\x01 \x03(\x0b\x32\x17.ondewo.nlu.ModelStatus\"s\n\x12\x43ustomPlatformInfo\x12\x35\n\x08platform\x18\x01 \x01(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\r\"+\n\x19GetPlatformMappingRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\"X\n\x0fPlatformMapping\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x35\n\rplatform_info\x18\x02 \x03(\x0b\x32\x1e.ondewo.nlu.CustomPlatformInfo\"\x99\x03\n\x15\x46ullTextSearchRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x0c\n\x04term\x18\x03 \x01(\t\x12\x12\n\npage_token\x18\x04 \x01(\t\"\xb6\x02\n\tQueryType\x12\x07\n\x03\x41LL\x10\x00\x12\x15\n\x11OndewoEntityQuery\x10\x01\x12\x19\n\x15OndewoEntityTypeQuery\x10\x02\x12\x1c\n\x18OndewoEntitySynonymQuery\x10\x03\x12\x15\n\x11OndewoIntentQuery\x10\x04\x12\x1e\n\x1aOndewoIntentContextInQuery\x10\x05\x12\x1f\n\x1bOndewoIntentContextOutQuery\x10\x06\x12\x1d\n\x19OndewoIntentUsersaysQuery\x10\x07\x12\x19\n\x15OndewoIntentTagsQuery\x10\x08\x12\x1f\n\x1bOndewoIntentParametersQuery\x10\t\x12\x1d\n\x19OndewoIntentResponseQuery\x10\n\"\xc7\x02\n FullTextSearchResponseEntityType\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12`\n\x13\x65ntity_type_results\x18\x03 \x03(\x0b\x32\x43.ondewo.nlu.FullTextSearchResponseEntityType.EntityTypeSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1aN\n\x16\x45ntityTypeSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x10\n\x08language\x18\x03 \x01(\t\"\xef\x02\n\x1c\x46ullTextSearchResponseEntity\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12S\n\x0e\x65ntity_results\x18\x03 \x03(\x0b\x32;.ondewo.nlu.FullTextSearchResponseEntity.EntitySearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a\x86\x01\n\x12\x45ntitySearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x18\n\x10\x65ntity_type_name\x18\x03 \x01(\t\x12 \n\x18\x65ntity_type_display_name\x18\x04 \x01(\t\x12\x10\n\x08language\x18\x05 \x01(\t\"\xc5\x03\n#FullTextSearchResponseEntitySynonym\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12i\n\x16\x65ntity_synonym_results\x18\x03 \x03(\x0b\x32I.ondewo.nlu.FullTextSearchResponseEntitySynonym.EntitySynonymSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a\xbf\x01\n\x19\x45ntitySynonymSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x18\n\x10\x65ntity_type_name\x18\x03 \x01(\t\x12 \n\x18\x65ntity_type_display_name\x18\x04 \x01(\t\x12\x13\n\x0b\x65ntity_name\x18\x05 \x01(\t\x12\x1b\n\x13\x65ntity_display_name\x18\x06 \x01(\t\x12\x10\n\x08language\x18\x07 \x01(\t\"\xd5\x02\n\x1c\x46ullTextSearchResponseIntent\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12S\n\x0eintent_results\x18\x03 \x03(\x0b\x32;.ondewo.nlu.FullTextSearchResponseIntent.IntentSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1am\n\x12IntentSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x13\n\x0b\x64omain_name\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x10\n\x08language\x18\x05 \x01(\t\"\x8b\x03\n%FullTextSearchResponseIntentContextIn\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12p\n\x19intent_context_in_results\x18\x03 \x03(\x0b\x32M.ondewo.nlu.FullTextSearchResponseIntentContextIn.IntentContextInSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a}\n\x1bIntentContextInSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bintent_name\x18\x02 \x01(\t\x12\x1b\n\x13intent_display_name\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x10\n\x08language\x18\x05 \x01(\t\"\x90\x03\n&FullTextSearchResponseIntentContextOut\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12s\n\x1aintent_context_out_results\x18\x03 \x03(\x0b\x32O.ondewo.nlu.FullTextSearchResponseIntentContextOut.IntentContextOutSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a~\n\x1cIntentContextOutSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bintent_name\x18\x02 \x01(\t\x12\x1b\n\x13intent_display_name\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x10\n\x08language\x18\x05 \x01(\t\"\xdf\x03\n$FullTextSearchResponseIntentUsersays\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12l\n\x17intent_usersays_results\x18\x03 \x03(\x0b\x32K.ondewo.nlu.FullTextSearchResponseIntentUsersays.IntentUsersaysSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a\xd5\x01\n\x1aIntentUsersaysSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x1c\n\x14text_as_entity_types\x18\x03 \x01(\t\x12\x1d\n\x15text_as_entity_values\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x13\n\x0bintent_name\x18\x06 \x01(\t\x12\x1b\n\x13intent_display_name\x18\x07 \x01(\t\x12\x0c\n\x04tags\x18\x08 \x03(\t\x12\x10\n\x08language\x18\t \x01(\t\"\x80\x03\n FullTextSearchResponseIntentTags\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12`\n\x13intent_tags_results\x18\x03 \x03(\x0b\x32\x43.ondewo.nlu.FullTextSearchResponseIntentTags.IntentTagsSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a\x86\x01\n\x16IntentTagsSearchResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x13\n\x0bintent_name\x18\x03 \x01(\t\x12\x1b\n\x13intent_display_name\x18\x04 \x01(\t\x12\x0c\n\x04tags\x18\x05 \x03(\t\x12\x10\n\x08language\x18\x06 \x01(\t\"\xaf\x03\n$FullTextSearchResponseIntentResponse\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12l\n\x17intent_response_results\x18\x03 \x03(\x0b\x32K.ondewo.nlu.FullTextSearchResponseIntentResponse.IntentResponseSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a\xa5\x01\n\x1aIntentResponseSearchResult\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x10\n\x08platform\x18\x02 \x01(\t\x12\x15\n\rresponse_type\x18\x03 \x01(\t\x12\x13\n\x0bintent_name\x18\x04 \x01(\t\x12\x1b\n\x13intent_display_name\x18\x05 \x01(\t\x12\x0c\n\x04tags\x18\x06 \x03(\t\x12\x10\n\x08language\x18\x07 \x01(\t\"\xba\x03\n&FullTextSearchResponseIntentParameters\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12r\n\x19intent_parameters_results\x18\x03 \x03(\x0b\x32O.ondewo.nlu.FullTextSearchResponseIntentParameters.IntentParametersSearchResult\x12\x0c\n\x04term\x18\x04 \x01(\t\x12\x15\n\relastic_query\x18\x05 \x01(\t\x12\x0c\n\x04time\x18\x06 \x01(\x02\x12\x17\n\x0fnext_page_token\x18\x07 \x01(\t\x1a\xa8\x01\n\x1cIntentParametersSearchResult\x12\x16\n\x0eparameter_name\x18\x01 \x01(\t\x12\x1e\n\x16parameter_display_name\x18\x02 \x01(\t\x12\x13\n\x0bintent_name\x18\x03 \x01(\t\x12\x1b\n\x13intent_display_name\x18\x04 \x01(\t\x12\x0c\n\x04tags\x18\x05 \x03(\t\x12\x10\n\x08language\x18\x06 \x01(\t\"|\n\x13ReindexAgentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x13\n\x0b\x62ranch_name\x18\x02 \x01(\t\x12@\n\x0bindex_types\x18\x03 \x03(\x0e\x32+.ondewo.nlu.FullTextSearchRequest.QueryType*l\n\tAgentView\x12\x1a\n\x16\x41GENT_VIEW_UNSPECIFIED\x10\x00\x12\x13\n\x0f\x41GENT_VIEW_FULL\x10\x01\x12\x16\n\x12\x41GENT_VIEW_SHALLOW\x10\x02\x12\x16\n\x12\x41GENT_VIEW_MINIMUM\x10\x03*J\n\x12InitiationProtocol\x12\x17\n\x13\x41S_SOON_AS_POSSIBLE\x10\x00\x12\x10\n\x0cWHEN_TRAINED\x10\x01\x12\t\n\x05NEVER\x10\x02*q\n\nReportType\x12\x07\n\x03\x41LL\x10\x00\x12\x17\n\x13INTENT_PER_LANGUAGE\x10\x01\x12\x17\n\x13\x45NTITY_PER_LANGUAGE\x10\x02\x12\x14\n\x10\x45NTITY_COLLISION\x10\x03\x12\x12\n\x0eINTENT_GENERAL\x10\x04*\xfa\x03\n\x12SessionsReportType\x12\x0c\n\x08SESSIONS\x10\x00\x12\x11\n\rSESSION_STEPS\x10\x01\x12\x19\n\x15SESSION_TOP_X_INTENTS\x10\x02\x12\x1e\n\x1aSESSION_TOP_X_ENTITY_TYPES\x10\x03\x12\x1f\n\x1bSESSION_TOP_X_ENTITY_VALUES\x10\x04\x12\x17\n\x13SESSION_TOP_X_USERS\x10\x05\x12\x18\n\x14SESSION_TOP_X_LABELS\x10\x06\x12\x16\n\x12SESSION_TOP_X_TAGS\x10\x07\x12\x1f\n\x1bSESSION_TOP_X_PHONE_NUMBERS\x10\x08\x12\x1b\n\x17SESSION_HUMAN_HANDOVERS\x10\t\x12\x15\n\x11SESSION_SQL_QUERY\x10\n\x12\x1b\n\x17SESSION_LEAST_X_INTENTS\x10\x0b\x12 \n\x1cSESSION_LEAST_X_ENTITY_TYPES\x10\x0c\x12!\n\x1dSESSION_LEAST_X_ENTITY_VALUES\x10\r\x12\x19\n\x15SESSION_LEAST_X_USERS\x10\x0e\x12\x1a\n\x16SESSION_LEAST_X_LABELS\x10\x0f\x12\x18\n\x14SESSION_LEAST_X_TAGS\x10\x10\x12\x14\n\x10TOTAL_STATISTICS\x10\x11*+\n\x0cReportFormat\x12\x07\n\x03\x43SV\x10\x00\x12\x08\n\x04HTML\x10\x01\x12\x08\n\x04JSON\x10\x02*\'\n\x0b\x41gentStatus\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08INACTIVE\x10\x01\x32\x8e%\n\x06\x41gents\x12Y\n\x0b\x43reateAgent\x12\x1e.ondewo.nlu.CreateAgentRequest\x1a\x11.ondewo.nlu.Agent\"\x17\x82\xd3\xe4\x93\x02\x11\"\x0c/v2/projects:\x01*\x12p\n\x0bUpdateAgent\x12\x1e.ondewo.nlu.UpdateAgentRequest\x1a\x11.ondewo.nlu.Agent\".\x82\xd3\xe4\x93\x02(2#/v2/{agent.parent=projects/*/agent}:\x01*\x12\x61\n\x08GetAgent\x12\x1b.ondewo.nlu.GetAgentRequest\x1a\x11.ondewo.nlu.Agent\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/v2/{parent=projects/*/agent}\x12l\n\x0b\x44\x65leteAgent\x12\x1e.ondewo.nlu.DeleteAgentRequest\x1a\x16.google.protobuf.Empty\"%\x82\xd3\xe4\x93\x02\x1f*\x1d/v2/{parent=projects/*/agent}\x12W\n\x0f\x44\x65leteAllAgents\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x14\x82\xd3\xe4\x93\x02\x0e*\x0c/v2/projects\x12\x61\n\nListAgents\x12\x1d.ondewo.nlu.ListAgentsRequest\x1a\x1e.ondewo.nlu.ListAgentsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v2/projects\x12m\n\x10ListAgentsOfUser\x12\x1d.ondewo.nlu.ListAgentsRequest\x1a$.ondewo.nlu.ListAgentsOfUserResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v2/projects\x12h\n\rListAllAgents\x12\x1d.ondewo.nlu.ListAgentsRequest\x1a\x1e.ondewo.nlu.ListAgentsResponse\"\x18\x82\xd3\xe4\x93\x02\x12\x12\x10/v2/projects:all\x12\x8b\x01\n\x10\x41\x64\x64UserToProject\x12#.ondewo.nlu.AddUserToProjectRequest\x1a\x16.google.protobuf.Empty\":\x82\xd3\xe4\x93\x02\x34\"//v2/{parent=projects/*/agent}/users/{user_id=*}:\x01*\x12\x92\x01\n\x15RemoveUserFromProject\x12(.ondewo.nlu.RemoveUserFromProjectRequest\x1a\x16.google.protobuf.Empty\"7\x82\xd3\xe4\x93\x02\x31*//v2/{parent=projects/*/agent}/users/{user_id=*}\x12\x90\x01\n\x12ListUsersInProject\x12%.ondewo.nlu.ListUsersInProjectRequest\x1a&.ondewo.nlu.ListUsersInProjectResponse\"+\x82\xd3\xe4\x93\x02%\x12#/v2/{parent=projects/*/agent}/users\x12\x63\n\x0fGetPlatformInfo\x12\x16.google.protobuf.Empty\x1a#.ondewo.nlu.GetPlatformInfoResponse\"\x13\x82\xd3\xe4\x93\x02\r\x12\x0b/v2/version\x12\x90\x01\n\x16ListProjectPermissions\x12).ondewo.nlu.ListProjectPermissionsRequest\x1a*.ondewo.nlu.ListProjectPermissionsResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/v2/project_permissions\x12r\n\nTrainAgent\x12\x1d.ondewo.nlu.TrainAgentRequest\x1a\x15.ondewo.nlu.Operation\".\x82\xd3\xe4\x93\x02(\"#/v2/{parent=projects/*/agent}:train:\x01*\x12x\n\nBuildCache\x12\x1d.ondewo.nlu.BuildCacheRequest\x1a\x15.ondewo.nlu.Operation\"4\x82\xd3\xe4\x93\x02.\")/v2/{parent=projects/*/agent}:build_cache:\x01*\x12u\n\x0b\x45xportAgent\x12\x1e.ondewo.nlu.ExportAgentRequest\x1a\x15.ondewo.nlu.Operation\"/\x82\xd3\xe4\x93\x02)\"$/v2/{parent=projects/*/agent}:export:\x01*\x12\x91\x01\n\x14\x45xportBenchmarkAgent\x12\'.ondewo.nlu.ExportBenchmarkAgentRequest\x1a\x15.ondewo.nlu.Operation\"9\x82\xd3\xe4\x93\x02\x33\"./v2/{parent=projects/*/agent}:export_benchmark:\x01*\x12u\n\x0bImportAgent\x12\x1e.ondewo.nlu.ImportAgentRequest\x1a\x15.ondewo.nlu.Operation\"/\x82\xd3\xe4\x93\x02)\"$/v2/{parent=projects/*/agent}:import:\x01*\x12\x97\x01\n\x14OptimizeRankingMatch\x12\'.ondewo.nlu.OptimizeRankingMatchRequest\x1a\x15.ondewo.nlu.Operation\"?\x82\xd3\xe4\x93\x02\x39\"4/v2/{parent=projects/*/agent}:optimize_ranking_match:\x01*\x12x\n\x0cRestoreAgent\x12\x1f.ondewo.nlu.RestoreAgentRequest\x1a\x15.ondewo.nlu.Operation\"0\x82\xd3\xe4\x93\x02*\"%/v2/{parent=projects/*/agent}:restore:\x01*\x12\x95\x01\n\x12GetAgentStatistics\x12%.ondewo.nlu.GetAgentStatisticsRequest\x1a&.ondewo.nlu.GetAgentStatisticsResponse\"0\x82\xd3\xe4\x93\x02*\x12(/v2/{parent=projects/*/agent}:statistics\x12\xa6\x01\n\x15GetSessionsStatistics\x12(.ondewo.nlu.GetSessionsStatisticsRequest\x1a).ondewo.nlu.GetSessionsStatisticsResponse\"8\x82\xd3\xe4\x93\x02\x32\x12\x30/v2/{parent=projects/*/agent}:session_statistics\x12w\n\x0eSetAgentStatus\x12!.ondewo.nlu.SetAgentStatusRequest\x1a\x11.ondewo.nlu.Agent\"/\x82\xd3\xe4\x93\x02)\"$/v2/{parent=projects/*/agent}:status:\x01*\x12{\n\x0cSetResources\x12\x1f.ondewo.nlu.SetResourcesRequest\x1a\x16.google.protobuf.Empty\"2\x82\xd3\xe4\x93\x02,\"\'/v2/{parent=projects/*/agent}:resources:\x01*\x12~\n\x0f\x44\x65leteResources\x12\".ondewo.nlu.DeleteResourcesRequest\x1a\x16.google.protobuf.Empty\"/\x82\xd3\xe4\x93\x02)*\'/v2/{parent=projects/*/agent}:resources\x12\x8e\x01\n\x0f\x45xportResources\x12\".ondewo.nlu.ExportResourcesRequest\x1a#.ondewo.nlu.ExportResourcesResponse\"2\x82\xd3\xe4\x93\x02,\"\'/v2/{parent=projects/*/agent}:resources:\x01*\x12]\n\x10GetModelStatuses\x12#.ondewo.nlu.GetModelStatusesRequest\x1a$.ondewo.nlu.GetModelStatusesResponse\x12X\n\x12GetPlatformMapping\x12%.ondewo.nlu.GetPlatformMappingRequest\x1a\x1b.ondewo.nlu.PlatformMapping\x12N\n\x12SetPlatformMapping\x12\x1b.ondewo.nlu.PlatformMapping\x1a\x1b.ondewo.nlu.PlatformMapping\x12n\n\x1bGetFullTextSearchEntityType\x12!.ondewo.nlu.FullTextSearchRequest\x1a,.ondewo.nlu.FullTextSearchResponseEntityType\x12\x66\n\x17GetFullTextSearchEntity\x12!.ondewo.nlu.FullTextSearchRequest\x1a(.ondewo.nlu.FullTextSearchResponseEntity\x12t\n\x1eGetFullTextSearchEntitySynonym\x12!.ondewo.nlu.FullTextSearchRequest\x1a/.ondewo.nlu.FullTextSearchResponseEntitySynonym\x12\x66\n\x17GetFullTextSearchIntent\x12!.ondewo.nlu.FullTextSearchRequest\x1a(.ondewo.nlu.FullTextSearchResponseIntent\x12x\n GetFullTextSearchIntentContextIn\x12!.ondewo.nlu.FullTextSearchRequest\x1a\x31.ondewo.nlu.FullTextSearchResponseIntentContextIn\x12z\n!GetFullTextSearchIntentContextOut\x12!.ondewo.nlu.FullTextSearchRequest\x1a\x32.ondewo.nlu.FullTextSearchResponseIntentContextOut\x12v\n\x1fGetFullTextSearchIntentUsersays\x12!.ondewo.nlu.FullTextSearchRequest\x1a\x30.ondewo.nlu.FullTextSearchResponseIntentUsersays\x12n\n\x1bGetFullTextSearchIntentTags\x12!.ondewo.nlu.FullTextSearchRequest\x1a,.ondewo.nlu.FullTextSearchResponseIntentTags\x12v\n\x1fGetFullTextSearchIntentResponse\x12!.ondewo.nlu.FullTextSearchRequest\x1a\x30.ondewo.nlu.FullTextSearchResponseIntentResponse\x12z\n!GetFullTextSearchIntentParameters\x12!.ondewo.nlu.FullTextSearchRequest\x1a\x32.ondewo.nlu.FullTextSearchResponseIntentParameters\x12\x46\n\x0cReindexAgent\x12\x1f.ondewo.nlu.ReindexAgentRequest\x1a\x15.ondewo.nlu.Operationb\x06proto3')
 
 _AGENTVIEW = DESCRIPTOR.enum_types_by_name['AgentView']
 AgentView = enum_type_wrapper.EnumTypeWrapper(_AGENTVIEW)
 _INITIATIONPROTOCOL = DESCRIPTOR.enum_types_by_name['InitiationProtocol']
 InitiationProtocol = enum_type_wrapper.EnumTypeWrapper(_INITIATIONPROTOCOL)
 _REPORTTYPE = DESCRIPTOR.enum_types_by_name['ReportType']
 ReportType = enum_type_wrapper.EnumTypeWrapper(_REPORTTYPE)
+_SESSIONSREPORTTYPE = DESCRIPTOR.enum_types_by_name['SessionsReportType']
+SessionsReportType = enum_type_wrapper.EnumTypeWrapper(_SESSIONSREPORTTYPE)
 _REPORTFORMAT = DESCRIPTOR.enum_types_by_name['ReportFormat']
 ReportFormat = enum_type_wrapper.EnumTypeWrapper(_REPORTFORMAT)
 _AGENTSTATUS = DESCRIPTOR.enum_types_by_name['AgentStatus']
 AgentStatus = enum_type_wrapper.EnumTypeWrapper(_AGENTSTATUS)
 AGENT_VIEW_UNSPECIFIED = 0
 AGENT_VIEW_FULL = 1
 AGENT_VIEW_SHALLOW = 2
+AGENT_VIEW_MINIMUM = 3
 AS_SOON_AS_POSSIBLE = 0
 WHEN_TRAINED = 1
 NEVER = 2
 ALL = 0
 INTENT_PER_LANGUAGE = 1
 ENTITY_PER_LANGUAGE = 2
 ENTITY_COLLISION = 3
 INTENT_GENERAL = 4
+SESSIONS = 0
+SESSION_STEPS = 1
+SESSION_TOP_X_INTENTS = 2
+SESSION_TOP_X_ENTITY_TYPES = 3
+SESSION_TOP_X_ENTITY_VALUES = 4
+SESSION_TOP_X_USERS = 5
+SESSION_TOP_X_LABELS = 6
+SESSION_TOP_X_TAGS = 7
+SESSION_TOP_X_PHONE_NUMBERS = 8
+SESSION_HUMAN_HANDOVERS = 9
+SESSION_SQL_QUERY = 10
+SESSION_LEAST_X_INTENTS = 11
+SESSION_LEAST_X_ENTITY_TYPES = 12
+SESSION_LEAST_X_ENTITY_VALUES = 13
+SESSION_LEAST_X_USERS = 14
+SESSION_LEAST_X_LABELS = 15
+SESSION_LEAST_X_TAGS = 16
+TOTAL_STATISTICS = 17
 CSV = 0
 HTML = 1
 JSON = 2
 ACTIVE = 0
 INACTIVE = 1
 
 
@@ -74,14 +95,16 @@
 _OPTIMIZERANKINGMATCHREQUEST = DESCRIPTOR.message_types_by_name['OptimizeRankingMatchRequest']
 _RANKINGMATCHOPTIMIZATIONCONFIG = DESCRIPTOR.message_types_by_name['RankingMatchOptimizationConfig']
 _OPTIMIZERANKINGMATCHRESPONSE = DESCRIPTOR.message_types_by_name['OptimizeRankingMatchResponse']
 _IMPORTAGENTREQUEST = DESCRIPTOR.message_types_by_name['ImportAgentRequest']
 _RESTOREAGENTREQUEST = DESCRIPTOR.message_types_by_name['RestoreAgentRequest']
 _GETAGENTSTATISTICSREQUEST = DESCRIPTOR.message_types_by_name['GetAgentStatisticsRequest']
 _GETAGENTSTATISTICSRESPONSE = DESCRIPTOR.message_types_by_name['GetAgentStatisticsResponse']
+_GETSESSIONSSTATISTICSREQUEST = DESCRIPTOR.message_types_by_name['GetSessionsStatisticsRequest']
+_GETSESSIONSSTATISTICSRESPONSE = DESCRIPTOR.message_types_by_name['GetSessionsStatisticsResponse']
 _ADDUSERTOPROJECTREQUEST = DESCRIPTOR.message_types_by_name['AddUserToProjectRequest']
 _REMOVEUSERFROMPROJECTREQUEST = DESCRIPTOR.message_types_by_name['RemoveUserFromProjectRequest']
 _LISTUSERSINPROJECTREQUEST = DESCRIPTOR.message_types_by_name['ListUsersInProjectRequest']
 _USERINPROJECT = DESCRIPTOR.message_types_by_name['UserInProject']
 _LISTUSERSINPROJECTRESPONSE = DESCRIPTOR.message_types_by_name['ListUsersInProjectResponse']
 _GETPLATFORMINFORESPONSE = DESCRIPTOR.message_types_by_name['GetPlatformInfoResponse']
 _LISTPROJECTPERMISSIONSREQUEST = DESCRIPTOR.message_types_by_name['ListProjectPermissionsRequest']
@@ -287,14 +310,28 @@
 GetAgentStatisticsResponse = _reflection.GeneratedProtocolMessageType('GetAgentStatisticsResponse', (_message.Message,), {
     'DESCRIPTOR': _GETAGENTSTATISTICSRESPONSE,
     '__module__': 'ondewo.nlu.agent_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.nlu.GetAgentStatisticsResponse)
 })
 _sym_db.RegisterMessage(GetAgentStatisticsResponse)
 
+GetSessionsStatisticsRequest = _reflection.GeneratedProtocolMessageType('GetSessionsStatisticsRequest', (_message.Message,), {
+    'DESCRIPTOR': _GETSESSIONSSTATISTICSREQUEST,
+    '__module__': 'ondewo.nlu.agent_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.nlu.GetSessionsStatisticsRequest)
+})
+_sym_db.RegisterMessage(GetSessionsStatisticsRequest)
+
+GetSessionsStatisticsResponse = _reflection.GeneratedProtocolMessageType('GetSessionsStatisticsResponse', (_message.Message,), {
+    'DESCRIPTOR': _GETSESSIONSSTATISTICSRESPONSE,
+    '__module__': 'ondewo.nlu.agent_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.nlu.GetSessionsStatisticsResponse)
+})
+_sym_db.RegisterMessage(GetSessionsStatisticsResponse)
+
 AddUserToProjectRequest = _reflection.GeneratedProtocolMessageType('AddUserToProjectRequest', (_message.Message,), {
     'DESCRIPTOR': _ADDUSERTOPROJECTREQUEST,
     '__module__': 'ondewo.nlu.agent_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.nlu.AddUserToProjectRequest)
 })
 _sym_db.RegisterMessage(AddUserToProjectRequest)
 
@@ -629,166 +666,174 @@
     _AGENTS.methods_by_name['ImportAgent']._serialized_options = b'\202\323\344\223\002)\"$/v2/{parent=projects/*/agent}:import:\001*'
     _AGENTS.methods_by_name['OptimizeRankingMatch']._options = None
     _AGENTS.methods_by_name['OptimizeRankingMatch']._serialized_options = b'\202\323\344\223\0029\"4/v2/{parent=projects/*/agent}:optimize_ranking_match:\001*'
     _AGENTS.methods_by_name['RestoreAgent']._options = None
     _AGENTS.methods_by_name['RestoreAgent']._serialized_options = b'\202\323\344\223\002*\"%/v2/{parent=projects/*/agent}:restore:\001*'
     _AGENTS.methods_by_name['GetAgentStatistics']._options = None
     _AGENTS.methods_by_name['GetAgentStatistics']._serialized_options = b'\202\323\344\223\002*\022(/v2/{parent=projects/*/agent}:statistics'
+    _AGENTS.methods_by_name['GetSessionsStatistics']._options = None
+    _AGENTS.methods_by_name['GetSessionsStatistics']._serialized_options = b'\202\323\344\223\0022\0220/v2/{parent=projects/*/agent}:session_statistics'
     _AGENTS.methods_by_name['SetAgentStatus']._options = None
     _AGENTS.methods_by_name['SetAgentStatus']._serialized_options = b'\202\323\344\223\002)\"$/v2/{parent=projects/*/agent}:status:\001*'
     _AGENTS.methods_by_name['SetResources']._options = None
     _AGENTS.methods_by_name['SetResources']._serialized_options = b'\202\323\344\223\002,\"\'/v2/{parent=projects/*/agent}:resources:\001*'
     _AGENTS.methods_by_name['DeleteResources']._options = None
     _AGENTS.methods_by_name['DeleteResources']._serialized_options = b'\202\323\344\223\002)*\'/v2/{parent=projects/*/agent}:resources'
     _AGENTS.methods_by_name['ExportResources']._options = None
     _AGENTS.methods_by_name['ExportResources']._serialized_options = b'\202\323\344\223\002,\"\'/v2/{parent=projects/*/agent}:resources:\001*'
-    _AGENTVIEW._serialized_start = 9593
-    _AGENTVIEW._serialized_end = 9677
-    _INITIATIONPROTOCOL._serialized_start = 9679
-    _INITIATIONPROTOCOL._serialized_end = 9753
-    _REPORTTYPE._serialized_start = 9755
-    _REPORTTYPE._serialized_end = 9868
-    _REPORTFORMAT._serialized_start = 9870
-    _REPORTFORMAT._serialized_end = 9913
-    _AGENTSTATUS._serialized_start = 9915
-    _AGENTSTATUS._serialized_end = 9954
-    _AGENT._serialized_start = 355
-    _AGENT._serialized_end = 628
-    _AGENTWITHOWNER._serialized_start = 630
-    _AGENTWITHOWNER._serialized_end = 713
-    _AGENTOFUSERWITHOWNER._serialized_start = 715
-    _AGENTOFUSERWITHOWNER._serialized_end = 838
-    _CREATEAGENTREQUEST._serialized_start = 840
-    _CREATEAGENTREQUEST._serialized_end = 937
-    _UPDATEAGENTREQUEST._serialized_start = 940
-    _UPDATEAGENTREQUEST._serialized_end = 1086
-    _DELETEAGENTREQUEST._serialized_start = 1088
-    _DELETEAGENTREQUEST._serialized_end = 1124
-    _GETAGENTREQUEST._serialized_start = 1126
-    _GETAGENTREQUEST._serialized_end = 1202
-    _LISTAGENTSREQUEST._serialized_start = 1205
-    _LISTAGENTSREQUEST._serialized_end = 1336
-    _LISTAGENTSRESPONSE._serialized_start = 1338
-    _LISTAGENTSRESPONSE._serialized_end = 1439
-    _LISTAGENTSOFUSERRESPONSE._serialized_start = 1441
-    _LISTAGENTSOFUSERRESPONSE._serialized_end = 1562
-    _TRAINAGENTREQUEST._serialized_start = 1564
-    _TRAINAGENTREQUEST._serialized_end = 1676
-    _BUILDCACHEREQUEST._serialized_start = 1678
-    _BUILDCACHEREQUEST._serialized_end = 1729
-    _EXPORTAGENTREQUEST._serialized_start = 1731
-    _EXPORTAGENTREQUEST._serialized_end = 1813
-    _EXPORTAGENTRESPONSE._serialized_start = 1815
-    _EXPORTAGENTRESPONSE._serialized_end = 1891
-    _EXPORTBENCHMARKAGENTREQUEST._serialized_start = 1894
-    _EXPORTBENCHMARKAGENTREQUEST._serialized_end = 2027
-    _EXPORTBENCHMARKAGENTRESPONSE._serialized_start = 2030
-    _EXPORTBENCHMARKAGENTRESPONSE._serialized_end = 2269
-    _EXPORTBENCHMARKAGENTRESPONSE_TRAININGPHRASESENTRY._serialized_start = 2174
-    _EXPORTBENCHMARKAGENTRESPONSE_TRAININGPHRASESENTRY._serialized_end = 2269
-    _OPTIMIZERANKINGMATCHREQUEST._serialized_start = 2272
-    _OPTIMIZERANKINGMATCHREQUEST._serialized_end = 2433
-    _RANKINGMATCHOPTIMIZATIONCONFIG._serialized_start = 2436
-    _RANKINGMATCHOPTIMIZATIONCONFIG._serialized_end = 2583
-    _OPTIMIZERANKINGMATCHRESPONSE._serialized_start = 2586
-    _OPTIMIZERANKINGMATCHRESPONSE._serialized_end = 2726
-    _IMPORTAGENTREQUEST._serialized_start = 2728
-    _IMPORTAGENTREQUEST._serialized_end = 2819
-    _RESTOREAGENTREQUEST._serialized_start = 2821
-    _RESTOREAGENTREQUEST._serialized_end = 2913
-    _GETAGENTSTATISTICSREQUEST._serialized_start = 2916
-    _GETAGENTSTATISTICSREQUEST._serialized_end = 3062
-    _GETAGENTSTATISTICSRESPONSE._serialized_start = 3064
-    _GETAGENTSTATISTICSRESPONSE._serialized_end = 3189
-    _ADDUSERTOPROJECTREQUEST._serialized_start = 3191
-    _ADDUSERTOPROJECTREQUEST._serialized_end = 3274
-    _REMOVEUSERFROMPROJECTREQUEST._serialized_start = 3276
-    _REMOVEUSERFROMPROJECTREQUEST._serialized_end = 3339
-    _LISTUSERSINPROJECTREQUEST._serialized_start = 3341
-    _LISTUSERSINPROJECTREQUEST._serialized_end = 3404
-    _USERINPROJECT._serialized_start = 3406
-    _USERINPROJECT._serialized_end = 3486
-    _LISTUSERSINPROJECTRESPONSE._serialized_start = 3488
-    _LISTUSERSINPROJECTRESPONSE._serialized_end = 3583
-    _GETPLATFORMINFORESPONSE._serialized_start = 3585
-    _GETPLATFORMINFORESPONSE._serialized_end = 3648
-    _LISTPROJECTPERMISSIONSREQUEST._serialized_start = 3650
-    _LISTPROJECTPERMISSIONSREQUEST._serialized_end = 3701
-    _LISTPROJECTPERMISSIONSRESPONSE._serialized_start = 3703
-    _LISTPROJECTPERMISSIONSRESPONSE._serialized_end = 3781
-    _SETAGENTSTATUSREQUEST._serialized_start = 3783
-    _SETAGENTSTATUSREQUEST._serialized_end = 3906
-    _AGENTSORTING._serialized_start = 3909
-    _AGENTSORTING._serialized_end = 4200
-    _AGENTSORTING_AGENTSORTINGFIELD._serialized_start = 4040
-    _AGENTSORTING_AGENTSORTINGFIELD._serialized_end = 4200
-    _SETRESOURCESREQUEST._serialized_start = 4202
-    _SETRESOURCESREQUEST._serialized_end = 4313
-    _DELETERESOURCESREQUEST._serialized_start = 4315
-    _DELETERESOURCESREQUEST._serialized_end = 4406
-    _EXPORTRESOURCESREQUEST._serialized_start = 4408
-    _EXPORTRESOURCESREQUEST._serialized_end = 4499
-    _EXPORTRESOURCESRESPONSE._serialized_start = 4501
-    _EXPORTRESOURCESRESPONSE._serialized_end = 4616
-    _GETMODELSTATUSESREQUEST._serialized_start = 4618
-    _GETMODELSTATUSESREQUEST._serialized_end = 4725
-    _MODELSTATUS._serialized_start = 4728
-    _MODELSTATUS._serialized_end = 5048
-    _MODELSTATUS_STATUSNAME._serialized_start = 4930
-    _MODELSTATUS_STATUSNAME._serialized_end = 5048
-    _GETMODELSTATUSESRESPONSE._serialized_start = 5050
-    _GETMODELSTATUSESRESPONSE._serialized_end = 5125
-    _CUSTOMPLATFORMINFO._serialized_start = 5127
-    _CUSTOMPLATFORMINFO._serialized_end = 5242
-    _GETPLATFORMMAPPINGREQUEST._serialized_start = 5244
-    _GETPLATFORMMAPPINGREQUEST._serialized_end = 5287
-    _PLATFORMMAPPING._serialized_start = 5289
-    _PLATFORMMAPPING._serialized_end = 5377
-    _FULLTEXTSEARCHREQUEST._serialized_start = 5380
-    _FULLTEXTSEARCHREQUEST._serialized_end = 5789
-    _FULLTEXTSEARCHREQUEST_QUERYTYPE._serialized_start = 5479
-    _FULLTEXTSEARCHREQUEST_QUERYTYPE._serialized_end = 5789
-    _FULLTEXTSEARCHRESPONSEENTITYTYPE._serialized_start = 5792
-    _FULLTEXTSEARCHRESPONSEENTITYTYPE._serialized_end = 6119
-    _FULLTEXTSEARCHRESPONSEENTITYTYPE_ENTITYTYPESEARCHRESULT._serialized_start = 6041
-    _FULLTEXTSEARCHRESPONSEENTITYTYPE_ENTITYTYPESEARCHRESULT._serialized_end = 6119
-    _FULLTEXTSEARCHRESPONSEENTITY._serialized_start = 6122
-    _FULLTEXTSEARCHRESPONSEENTITY._serialized_end = 6454
-    _FULLTEXTSEARCHRESPONSEENTITY_ENTITYSEARCHRESULT._serialized_start = 6354
-    _FULLTEXTSEARCHRESPONSEENTITY_ENTITYSEARCHRESULT._serialized_end = 6454
-    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM._serialized_start = 6457
-    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM._serialized_end = 6847
-    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM_ENTITYSYNONYMSEARCHRESULT._serialized_start = 6719
-    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM_ENTITYSYNONYMSEARCHRESULT._serialized_end = 6847
-    _FULLTEXTSEARCHRESPONSEINTENT._serialized_start = 6850
-    _FULLTEXTSEARCHRESPONSEINTENT._serialized_end = 7177
-    _FULLTEXTSEARCHRESPONSEINTENT_INTENTSEARCHRESULT._serialized_start = 7082
-    _FULLTEXTSEARCHRESPONSEINTENT_INTENTSEARCHRESULT._serialized_end = 7177
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN._serialized_start = 7180
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN._serialized_end = 7532
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN_INTENTCONTEXTINSEARCHRESULT._serialized_start = 7450
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN_INTENTCONTEXTINSEARCHRESULT._serialized_end = 7532
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT._serialized_start = 7535
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT._serialized_end = 7892
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT_INTENTCONTEXTOUTSEARCHRESULT._serialized_start = 7809
-    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT_INTENTCONTEXTOUTSEARCHRESULT._serialized_end = 7892
-    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS._serialized_start = 7895
-    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS._serialized_end = 8331
-    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS_INTENTUSERSAYSSEARCHRESULT._serialized_start = 8161
-    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS_INTENTUSERSAYSSEARCHRESULT._serialized_end = 8331
-    _FULLTEXTSEARCHRESPONSEINTENTTAGS._serialized_start = 8334
-    _FULLTEXTSEARCHRESPONSEINTENTTAGS._serialized_end = 8674
-    _FULLTEXTSEARCHRESPONSEINTENTTAGS_INTENTTAGSSEARCHRESULT._serialized_start = 8583
-    _FULLTEXTSEARCHRESPONSEINTENTTAGS_INTENTTAGSSEARCHRESULT._serialized_end = 8674
-    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE._serialized_start = 8677
-    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE._serialized_end = 9064
-    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE_INTENTRESPONSESEARCHRESULT._serialized_start = 8942
-    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE_INTENTRESPONSESEARCHRESULT._serialized_end = 9064
-    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS._serialized_start = 9067
-    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS._serialized_end = 9465
-    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS_INTENTPARAMETERSSEARCHRESULT._serialized_start = 9340
-    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS_INTENTPARAMETERSSEARCHRESULT._serialized_end = 9465
-    _REINDEXAGENTREQUEST._serialized_start = 9467
-    _REINDEXAGENTREQUEST._serialized_end = 9591
-    _AGENTS._serialized_start = 9957
-    _AGENTS._serialized_end = 14538
+    _AGENTVIEW._serialized_start = 10464
+    _AGENTVIEW._serialized_end = 10572
+    _INITIATIONPROTOCOL._serialized_start = 10574
+    _INITIATIONPROTOCOL._serialized_end = 10648
+    _REPORTTYPE._serialized_start = 10650
+    _REPORTTYPE._serialized_end = 10763
+    _SESSIONSREPORTTYPE._serialized_start = 10766
+    _SESSIONSREPORTTYPE._serialized_end = 11272
+    _REPORTFORMAT._serialized_start = 11274
+    _REPORTFORMAT._serialized_end = 11317
+    _AGENTSTATUS._serialized_start = 11319
+    _AGENTSTATUS._serialized_end = 11358
+    _AGENT._serialized_start = 354
+    _AGENT._serialized_end = 627
+    _AGENTWITHOWNER._serialized_start = 629
+    _AGENTWITHOWNER._serialized_end = 712
+    _AGENTOFUSERWITHOWNER._serialized_start = 714
+    _AGENTOFUSERWITHOWNER._serialized_end = 837
+    _CREATEAGENTREQUEST._serialized_start = 839
+    _CREATEAGENTREQUEST._serialized_end = 936
+    _UPDATEAGENTREQUEST._serialized_start = 939
+    _UPDATEAGENTREQUEST._serialized_end = 1085
+    _DELETEAGENTREQUEST._serialized_start = 1087
+    _DELETEAGENTREQUEST._serialized_end = 1123
+    _GETAGENTREQUEST._serialized_start = 1125
+    _GETAGENTREQUEST._serialized_end = 1201
+    _LISTAGENTSREQUEST._serialized_start = 1204
+    _LISTAGENTSREQUEST._serialized_end = 1335
+    _LISTAGENTSRESPONSE._serialized_start = 1337
+    _LISTAGENTSRESPONSE._serialized_end = 1438
+    _LISTAGENTSOFUSERRESPONSE._serialized_start = 1440
+    _LISTAGENTSOFUSERRESPONSE._serialized_end = 1561
+    _TRAINAGENTREQUEST._serialized_start = 1563
+    _TRAINAGENTREQUEST._serialized_end = 1675
+    _BUILDCACHEREQUEST._serialized_start = 1677
+    _BUILDCACHEREQUEST._serialized_end = 1728
+    _EXPORTAGENTREQUEST._serialized_start = 1730
+    _EXPORTAGENTREQUEST._serialized_end = 1812
+    _EXPORTAGENTRESPONSE._serialized_start = 1814
+    _EXPORTAGENTRESPONSE._serialized_end = 1890
+    _EXPORTBENCHMARKAGENTREQUEST._serialized_start = 1893
+    _EXPORTBENCHMARKAGENTREQUEST._serialized_end = 2026
+    _EXPORTBENCHMARKAGENTRESPONSE._serialized_start = 2029
+    _EXPORTBENCHMARKAGENTRESPONSE._serialized_end = 2268
+    _EXPORTBENCHMARKAGENTRESPONSE_TRAININGPHRASESENTRY._serialized_start = 2173
+    _EXPORTBENCHMARKAGENTRESPONSE_TRAININGPHRASESENTRY._serialized_end = 2268
+    _OPTIMIZERANKINGMATCHREQUEST._serialized_start = 2271
+    _OPTIMIZERANKINGMATCHREQUEST._serialized_end = 2432
+    _RANKINGMATCHOPTIMIZATIONCONFIG._serialized_start = 2435
+    _RANKINGMATCHOPTIMIZATIONCONFIG._serialized_end = 2582
+    _OPTIMIZERANKINGMATCHRESPONSE._serialized_start = 2585
+    _OPTIMIZERANKINGMATCHRESPONSE._serialized_end = 2725
+    _IMPORTAGENTREQUEST._serialized_start = 2727
+    _IMPORTAGENTREQUEST._serialized_end = 2818
+    _RESTOREAGENTREQUEST._serialized_start = 2820
+    _RESTOREAGENTREQUEST._serialized_end = 2912
+    _GETAGENTSTATISTICSREQUEST._serialized_start = 2915
+    _GETAGENTSTATISTICSREQUEST._serialized_end = 3061
+    _GETAGENTSTATISTICSRESPONSE._serialized_start = 3063
+    _GETAGENTSTATISTICSRESPONSE._serialized_end = 3188
+    _GETSESSIONSSTATISTICSREQUEST._serialized_start = 3191
+    _GETSESSIONSSTATISTICSREQUEST._serialized_end = 3548
+    _GETSESSIONSSTATISTICSRESPONSE._serialized_start = 3551
+    _GETSESSIONSSTATISTICSRESPONSE._serialized_end = 3687
+    _ADDUSERTOPROJECTREQUEST._serialized_start = 3689
+    _ADDUSERTOPROJECTREQUEST._serialized_end = 3772
+    _REMOVEUSERFROMPROJECTREQUEST._serialized_start = 3774
+    _REMOVEUSERFROMPROJECTREQUEST._serialized_end = 3837
+    _LISTUSERSINPROJECTREQUEST._serialized_start = 3839
+    _LISTUSERSINPROJECTREQUEST._serialized_end = 3902
+    _USERINPROJECT._serialized_start = 3904
+    _USERINPROJECT._serialized_end = 3984
+    _LISTUSERSINPROJECTRESPONSE._serialized_start = 3986
+    _LISTUSERSINPROJECTRESPONSE._serialized_end = 4081
+    _GETPLATFORMINFORESPONSE._serialized_start = 4083
+    _GETPLATFORMINFORESPONSE._serialized_end = 4146
+    _LISTPROJECTPERMISSIONSREQUEST._serialized_start = 4148
+    _LISTPROJECTPERMISSIONSREQUEST._serialized_end = 4199
+    _LISTPROJECTPERMISSIONSRESPONSE._serialized_start = 4201
+    _LISTPROJECTPERMISSIONSRESPONSE._serialized_end = 4279
+    _SETAGENTSTATUSREQUEST._serialized_start = 4281
+    _SETAGENTSTATUSREQUEST._serialized_end = 4404
+    _AGENTSORTING._serialized_start = 4407
+    _AGENTSORTING._serialized_end = 4698
+    _AGENTSORTING_AGENTSORTINGFIELD._serialized_start = 4538
+    _AGENTSORTING_AGENTSORTINGFIELD._serialized_end = 4698
+    _SETRESOURCESREQUEST._serialized_start = 4700
+    _SETRESOURCESREQUEST._serialized_end = 4811
+    _DELETERESOURCESREQUEST._serialized_start = 4813
+    _DELETERESOURCESREQUEST._serialized_end = 4904
+    _EXPORTRESOURCESREQUEST._serialized_start = 4906
+    _EXPORTRESOURCESREQUEST._serialized_end = 4997
+    _EXPORTRESOURCESRESPONSE._serialized_start = 4999
+    _EXPORTRESOURCESRESPONSE._serialized_end = 5114
+    _GETMODELSTATUSESREQUEST._serialized_start = 5116
+    _GETMODELSTATUSESREQUEST._serialized_end = 5223
+    _MODELSTATUS._serialized_start = 5226
+    _MODELSTATUS._serialized_end = 5546
+    _MODELSTATUS_STATUSNAME._serialized_start = 5428
+    _MODELSTATUS_STATUSNAME._serialized_end = 5546
+    _GETMODELSTATUSESRESPONSE._serialized_start = 5548
+    _GETMODELSTATUSESRESPONSE._serialized_end = 5623
+    _CUSTOMPLATFORMINFO._serialized_start = 5625
+    _CUSTOMPLATFORMINFO._serialized_end = 5740
+    _GETPLATFORMMAPPINGREQUEST._serialized_start = 5742
+    _GETPLATFORMMAPPINGREQUEST._serialized_end = 5785
+    _PLATFORMMAPPING._serialized_start = 5787
+    _PLATFORMMAPPING._serialized_end = 5875
+    _FULLTEXTSEARCHREQUEST._serialized_start = 5878
+    _FULLTEXTSEARCHREQUEST._serialized_end = 6287
+    _FULLTEXTSEARCHREQUEST_QUERYTYPE._serialized_start = 5977
+    _FULLTEXTSEARCHREQUEST_QUERYTYPE._serialized_end = 6287
+    _FULLTEXTSEARCHRESPONSEENTITYTYPE._serialized_start = 6290
+    _FULLTEXTSEARCHRESPONSEENTITYTYPE._serialized_end = 6617
+    _FULLTEXTSEARCHRESPONSEENTITYTYPE_ENTITYTYPESEARCHRESULT._serialized_start = 6539
+    _FULLTEXTSEARCHRESPONSEENTITYTYPE_ENTITYTYPESEARCHRESULT._serialized_end = 6617
+    _FULLTEXTSEARCHRESPONSEENTITY._serialized_start = 6620
+    _FULLTEXTSEARCHRESPONSEENTITY._serialized_end = 6987
+    _FULLTEXTSEARCHRESPONSEENTITY_ENTITYSEARCHRESULT._serialized_start = 6853
+    _FULLTEXTSEARCHRESPONSEENTITY_ENTITYSEARCHRESULT._serialized_end = 6987
+    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM._serialized_start = 6990
+    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM._serialized_end = 7443
+    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM_ENTITYSYNONYMSEARCHRESULT._serialized_start = 7252
+    _FULLTEXTSEARCHRESPONSEENTITYSYNONYM_ENTITYSYNONYMSEARCHRESULT._serialized_end = 7443
+    _FULLTEXTSEARCHRESPONSEINTENT._serialized_start = 7446
+    _FULLTEXTSEARCHRESPONSEINTENT._serialized_end = 7787
+    _FULLTEXTSEARCHRESPONSEINTENT_INTENTSEARCHRESULT._serialized_start = 7678
+    _FULLTEXTSEARCHRESPONSEINTENT_INTENTSEARCHRESULT._serialized_end = 7787
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN._serialized_start = 7790
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN._serialized_end = 8185
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN_INTENTCONTEXTINSEARCHRESULT._serialized_start = 8060
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTIN_INTENTCONTEXTINSEARCHRESULT._serialized_end = 8185
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT._serialized_start = 8188
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT._serialized_end = 8588
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT_INTENTCONTEXTOUTSEARCHRESULT._serialized_start = 8462
+    _FULLTEXTSEARCHRESPONSEINTENTCONTEXTOUT_INTENTCONTEXTOUTSEARCHRESULT._serialized_end = 8588
+    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS._serialized_start = 8591
+    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS._serialized_end = 9070
+    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS_INTENTUSERSAYSSEARCHRESULT._serialized_start = 8857
+    _FULLTEXTSEARCHRESPONSEINTENTUSERSAYS_INTENTUSERSAYSSEARCHRESULT._serialized_end = 9070
+    _FULLTEXTSEARCHRESPONSEINTENTTAGS._serialized_start = 9073
+    _FULLTEXTSEARCHRESPONSEINTENTTAGS._serialized_end = 9457
+    _FULLTEXTSEARCHRESPONSEINTENTTAGS_INTENTTAGSSEARCHRESULT._serialized_start = 9323
+    _FULLTEXTSEARCHRESPONSEINTENTTAGS_INTENTTAGSSEARCHRESULT._serialized_end = 9457
+    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE._serialized_start = 9460
+    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE._serialized_end = 9891
+    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE_INTENTRESPONSESEARCHRESULT._serialized_start = 9726
+    _FULLTEXTSEARCHRESPONSEINTENTRESPONSE_INTENTRESPONSESEARCHRESULT._serialized_end = 9891
+    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS._serialized_start = 9894
+    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS._serialized_end = 10336
+    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS_INTENTPARAMETERSSEARCHRESULT._serialized_start = 10168
+    _FULLTEXTSEARCHRESPONSEINTENTPARAMETERS_INTENTPARAMETERSSEARCHRESULT._serialized_end = 10336
+    _REINDEXAGENTREQUEST._serialized_start = 10338
+    _REINDEXAGENTREQUEST._serialized_end = 10462
+    _AGENTS._serialized_start = 11361
+    _AGENTS._serialized_end = 16111
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/agent_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/agent_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,19 @@
             response_deserializer=ondewo_dot_nlu_dot_operations__pb2.Operation.FromString,
         )
         self.GetAgentStatistics = channel.unary_unary(
             '/ondewo.nlu.Agents/GetAgentStatistics',
             request_serializer=ondewo_dot_nlu_dot_agent__pb2.GetAgentStatisticsRequest.SerializeToString,
             response_deserializer=ondewo_dot_nlu_dot_agent__pb2.GetAgentStatisticsResponse.FromString,
         )
+        self.GetSessionsStatistics = channel.unary_unary(
+            '/ondewo.nlu.Agents/GetSessionsStatistics',
+            request_serializer=ondewo_dot_nlu_dot_agent__pb2.GetSessionsStatisticsRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_agent__pb2.GetSessionsStatisticsResponse.FromString,
+        )
         self.SetAgentStatus = channel.unary_unary(
             '/ondewo.nlu.Agents/SetAgentStatus',
             request_serializer=ondewo_dot_nlu_dot_agent__pb2.SetAgentStatusRequest.SerializeToString,
             response_deserializer=ondewo_dot_nlu_dot_agent__pb2.Agent.FromString,
         )
         self.SetResources = channel.unary_unary(
             '/ondewo.nlu.Agents/SetResources',
@@ -242,15 +247,15 @@
         """Creates the specified agent.
 
         <p>Examples:</p>
 
         <pre>
         grpcurl -plaintext -H 'cai-token: aimp' -d '{
         "agent": {
-        "display_name": "Pizza Bot",
+        "display_name": "My Pizza Bot",
         "default_language_code": "en",
         "supported_language_codes": ["en"],
         "time_zone": "Europe/Vienna",
         "nlu_platform": "ONDEWO"
         }
         }' localhost:50055 ondewo.nlu.Agents.CreateAgent
         </pre>
@@ -483,27 +488,30 @@
         """Removes a user with specified id from the project (agent)
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListUsersInProject(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Lists users in the project (agent)
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetPlatformInfo(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Gets information from the platform
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListProjectPermissions(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """List permissions from the project (agent)
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def TrainAgent(self, request, context):
         """Trains the specified agent.
 
@@ -553,15 +561,16 @@
         metadata: [google.protobuf.Struct][google.protobuf.Struct]>
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def OptimizeRankingMatch(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Runs optimize ranking match
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def RestoreAgent(self, request, context):
         """Restores the specified agent from a ZIP file.
 
@@ -572,39 +581,50 @@
         metadata: [google.protobuf.Struct][google.protobuf.Struct]>
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetAgentStatistics(self, request, context):
+        """Gets statistics for the agent
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetSessionsStatistics(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SetAgentStatus(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Sets status for the agent
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SetResources(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Sets resources
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteResources(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Deletes resources
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ExportResources(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Exports resources
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetModelStatuses(self, request, context):
         """Get statuses of models related to project
         """
@@ -623,70 +643,79 @@
         """Set platform name mappings for an Agent
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFullTextSearchEntityType(self, request, context):
-        """Full text search endpoint
+        """Full text search endpoint in entity types
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFullTextSearchEntity(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Full text search endpoint in entities
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFullTextSearchEntitySynonym(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Full text search endpoint in entity synonyms
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFullTextSearchIntent(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Full text search endpoint in intents
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFullTextSearchIntentContextIn(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Full text search endpoint in context ins of intents
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFullTextSearchIntentContextOut(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Full text search endpoint in context outs of intents
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFullTextSearchIntentUsersays(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Full text search endpoint in user says of intents
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFullTextSearchIntentTags(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Full text search endpoint in tags of intents
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFullTextSearchIntentResponse(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Full text search endpoint in responses of intents
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFullTextSearchIntentParameters(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Full text search endpoint in parameters of intents
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ReindexAgent(self, request, context):
         """Force reindexing Intent and Entity data of Agent
         """
@@ -798,14 +827,19 @@
             response_serializer=ondewo_dot_nlu_dot_operations__pb2.Operation.SerializeToString,
         ),
         'GetAgentStatistics': grpc.unary_unary_rpc_method_handler(
             servicer.GetAgentStatistics,
             request_deserializer=ondewo_dot_nlu_dot_agent__pb2.GetAgentStatisticsRequest.FromString,
             response_serializer=ondewo_dot_nlu_dot_agent__pb2.GetAgentStatisticsResponse.SerializeToString,
         ),
+        'GetSessionsStatistics': grpc.unary_unary_rpc_method_handler(
+            servicer.GetSessionsStatistics,
+            request_deserializer=ondewo_dot_nlu_dot_agent__pb2.GetSessionsStatisticsRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_agent__pb2.GetSessionsStatisticsResponse.SerializeToString,
+        ),
         'SetAgentStatus': grpc.unary_unary_rpc_method_handler(
             servicer.SetAgentStatus,
             request_deserializer=ondewo_dot_nlu_dot_agent__pb2.SetAgentStatusRequest.FromString,
             response_serializer=ondewo_dot_nlu_dot_agent__pb2.Agent.SerializeToString,
         ),
         'SetResources': grpc.unary_unary_rpc_method_handler(
             servicer.SetResources,
@@ -1268,14 +1302,31 @@
         return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Agents/GetAgentStatistics',
                                              ondewo_dot_nlu_dot_agent__pb2.GetAgentStatisticsRequest.SerializeToString,
                                              ondewo_dot_nlu_dot_agent__pb2.GetAgentStatisticsResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetSessionsStatistics(request,
+                              target,
+                              options=(),
+                              channel_credentials=None,
+                              call_credentials=None,
+                              insecure=False,
+                              compression=None,
+                              wait_for_ready=None,
+                              timeout=None,
+                              metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Agents/GetSessionsStatistics',
+                                             ondewo_dot_nlu_dot_agent__pb2.GetSessionsStatisticsRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_agent__pb2.GetSessionsStatisticsResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def SetAgentStatus(request,
                        target,
                        options=(),
                        channel_credentials=None,
                        call_credentials=None,
                        insecure=False,
                        compression=None,
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/aiservices_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/aiservices_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bondewo/nlu/aiservices.proto\x12\nondewo.nlu\x1a\x1cgoogle/api/annotations.proto\x1a\x17ondewo/nlu/intent.proto\x1a\x1condewo/nlu/entity_type.proto\"b\n\x16\x45xtractEntitiesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12\x13\n\x0bintent_name\x18\x04 \x01(\t\"\xac\x01\n\x1b\x45xtractEntitiesFuzzyRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12@\n\x12potential_entities\x18\x03 \x03(\x0b\x32$.ondewo.nlu.EntityTypeFuzzyNerConfig\x12\x15\n\rminimal_score\x18\x04 \x01(\x02\x12\x16\n\x0e\x61llow_overlaps\x18\x05 \x01(\x08\"\x83\x02\n\x18\x45ntityTypeFuzzyNerConfig\x12+\n\x0b\x65ntity_type\x18\x01 \x01(\x0b\x32\x16.ondewo.nlu.EntityType\x12\x15\n\rminimal_score\x18\x02 \x01(\x02\x12\x15\n\rentity_values\x18\x03 \x03(\t\x12I\n\talgorithm\x18\x04 \x01(\x0e\x32\x36.ondewo.nlu.EntityTypeFuzzyNerConfig.FuzzyNerAlgorithm\"A\n\x11\x46uzzyNerAlgorithm\x12\x19\n\x15PREFILTER_LEVENSHTEIN\x10\x00\x12\x11\n\rLOCAL_MAXIMUM\x10\x01\"t\n\x0e\x45ntityDetected\x12\x38\n\x06\x65ntity\x18\x01 \x01(\x0b\x32(.ondewo.nlu.Intent.TrainingPhrase.Entity\x12\x19\n\x11\x65xtraction_method\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x02\"^\n\x17\x45xtractEntitiesResponse\x12\x35\n\x11\x65ntities_detected\x18\x01 \x03(\x0b\x32\x1a.ondewo.nlu.EntityDetected\x12\x0c\n\x04text\x18\x02 \x01(\t\"\xbd\x01\n\x1eGetAlternativeSentencesRequest\x12\x30\n\x06\x63onfig\x18\x01 \x01(\x0b\x32 .ondewo.nlu.DataEnrichmentConfig\x12\x10\n\x08sentence\x18\x02 \x01(\t\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x0e\n\x06parent\x18\x05 \x01(\t\x12\x17\n\x0fprotected_words\x18\x06 \x03(\t\x12\x17\n\x0fwords_to_change\x18\x07 \x03(\t\"j\n\x17GenerateUserSaysRequest\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x0e\n\x06parent\x18\x05 \x01(\t\x12\x18\n\x10n_repeat_synonym\x18\x06 \x01(\x05\x12\x0e\n\x06\x62ranch\x18\x08 \x01(\t\"\x8c\x01\n\x18GenerateResponsesRequest\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x0e\n\x06parent\x18\x05 \x01(\t\x12\x18\n\x10n_repeat_synonym\x18\x07 \x01(\x05\x12\x0e\n\x06\x62ranch\x18\x08 \x01(\t\x12\x1f\n\x17\x64rop_unknown_parameters\x18\t \x01(\x08\"\xc9\x02\n$GetAlternativeTrainingPhrasesRequest\x12\x30\n\x06\x63onfig\x18\x01 \x01(\x0b\x32 .ondewo.nlu.DataEnrichmentConfig\x12:\n\x0ftraining_phrase\x18\x02 \x01(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\x12\x13\n\x0bintent_name\x18\x03 \x01(\t\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x0e\n\x06parent\x18\x05 \x01(\t\x12\x17\n\x0f\x64\x65tect_entities\x18\x06 \x01(\x08\x12\x1c\n\x14similarity_threshold\x18\x07 \x01(\x02\x12\x17\n\x0fprotected_words\x18\x08 \x03(\t\x12\x17\n\x0fwords_to_change\x18\t \x03(\t\x12\x0e\n\x06\x62ranch\x18\n \x01(\t\"{\n\x12GetSynonymsRequest\x12\x30\n\x06\x63onfig\x18\x01 \x01(\x0b\x32 .ondewo.nlu.DataEnrichmentConfig\x12\x0c\n\x04word\x18\x02 \x01(\t\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x0e\n\x06parent\x18\x05 \x01(\t\"<\n\x13GetSynonymsResponse\x12%\n\x08synonyms\x18\x01 \x03(\x0b\x32\x13.ondewo.nlu.Synonym\")\n\x07Synonym\x12\x0f\n\x07synonym\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x05\"Y\n\x1fGetAlternativeSentencesResponse\x12\x36\n\x15\x61lternative_sentences\x18\x01 \x03(\x0b\x32\x17.ondewo.nlu.AltSentence\".\n\x19GenerateResponsesResponse\x12\x11\n\tresponses\x18\x02 \x03(\t\"-\n\x18GenerateUserSaysResponse\x12\x11\n\tuser_says\x18\x02 \x03(\t\"l\n%GetAlternativeTrainingPhrasesResponse\x12\x43\n\x1c\x61lternative_training_phrases\x18\x01 \x03(\x0b\x32\x1d.ondewo.nlu.AltTrainingPhrase\".\n\x0b\x41ltSentence\x12\x10\n\x08sentence\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x02\"^\n\x11\x41ltTrainingPhrase\x12:\n\x0ftraining_phrase\x18\x01 \x01(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\x12\r\n\x05score\x18\x02 \x01(\x02\"\x98\x04\n\x14\x44\x61taEnrichmentConfig\x12=\n\x11\x65ntity_enrichment\x18\x01 \x01(\x0b\x32\".ondewo.nlu.EntityEnrichmentConfig\x12\x43\n\x14thesaurus_enrichment\x18\x02 \x01(\x0b\x32%.ondewo.nlu.ThesaurusEnrichmentConfig\x12\x41\n\x13word2vec_enrichment\x18\x03 \x01(\x0b\x32$.ondewo.nlu.Word2VecEnrichmentConfig\x12\x43\n\x13word_net_enrichment\x18\x04 \x01(\x0b\x32&.ondewo.nlu.WordNetAugEnrichmentConfig\x12\x39\n\x0fgpt2_enrichment\x18\x05 \x01(\x0b\x32 .ondewo.nlu.GPT2EnrichmentConfig\x12;\n\x10glove_enrichment\x18\x06 \x01(\x0b\x32!.ondewo.nlu.GloVeEnrichmentConfig\x12<\n\x0f\x62\x65rt_enrichment\x18\x08 \x01(\x0b\x32#.ondewo.nlu.BertAugEnrichmentConfig\x12>\n\x10xlnet_enrichment\x18\t \x01(\x0b\x32$.ondewo.nlu.XLNetAugEnrichmentConfig\"_\n\x16\x45ntityEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"b\n\x19ThesaurusEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"`\n\x17\x42\x65rtAugEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"^\n\x15GloVeEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"]\n\x14GPT2EnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"a\n\x18Word2VecEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"c\n\x1aWordNetAugEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"a\n\x18XLNetAugEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"\xcf\x01\n\x16\x43lassifyIntentsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12\x17\n\x0f\x61\x63tive_contexts\x18\x04 \x01(\x08\x12\x15\n\rcontext_names\x18\x05 \x03(\t\x12\x1e\n\x04mode\x18\x06 \x01(\x0e\x32\x10.ondewo.nlu.Mode\x12\x30\n\nalgorithms\x18\x07 \x03(\x0e\x32\x1c.ondewo.nlu.IntentAlgorithms\"g\n\x10IntentClassified\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12\x1b\n\x13intent_display_name\x18\x02 \x01(\t\x12\x12\n\nclassifier\x18\x03 \x01(\t\x12\r\n\x05score\x18\x04 \x01(\x02\"\x91\x01\n\x17\x43lassifyIntentsResponse\x12\x38\n\x12intents_classified\x18\x01 \x03(\x0b\x32\x1c.ondewo.nlu.IntentClassified\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x17\n\x0f\x61\x63tive_contexts\x18\x03 \x01(\x08\x12\x15\n\rcontext_names\x18\x04 \x03(\t*5\n\x04Mode\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\r\n\tEXCLUSIVE\x10\x01\x12\r\n\tINCLUSIVE\x10\x02*\x8c\x03\n\x10IntentAlgorithms\x12$\n OndewoIntentExactContextDetector\x10\x00\x12\x1a\n\x16OndewoIntentExactMatch\x10\x01\x12\x1f\n\x1bOndewoIntentNamedExactMatch\x10\x02\x12\x1f\n\x1bOndewoIntentSimilarityMatch\x10\x03\x12$\n OndewoIntentNamedSimilarityMatch\x10\x04\x12\x1e\n\x1aOndewoIntentBertClassifier\x10\x07\x12\x1e\n\x1aOndewoIntentMetaClassifier\x10\x08\x12\x16\n\x12IntentExitDetector\x10\n\x12\x1c\n\x18OndewoIntentRankingMatch\x10\x0b\x12\x1a\n\x16OndewoWeightedEnsemble\x10\r\x12\x1c\n\x18OndewoIntentExitDetector\x10\x0e\x12\x1e\n\x1aOndewoIntentParameterMatch\x10\x0f\x32\xf0\t\n\nAiServices\x12\x95\x01\n\x0f\x45xtractEntities\x12\".ondewo.nlu.ExtractEntitiesRequest\x1a#.ondewo.nlu.ExtractEntitiesResponse\"9\x82\xd3\xe4\x93\x02\x33\"./v2/{parent=projects/*/agent}/entities:extract:\x01*\x12\x9a\x01\n\x10GenerateUserSays\x12#.ondewo.nlu.GenerateUserSaysRequest\x1a$.ondewo.nlu.GenerateUserSaysResponse\";\x82\xd3\xe4\x93\x02\x35\"0/v2/{parent=projects/*/agent}/generate_user_says:\x01*\x12\x9d\x01\n\x11GenerateResponses\x12$.ondewo.nlu.GenerateResponsesRequest\x1a%.ondewo.nlu.GenerateResponsesResponse\";\x82\xd3\xe4\x93\x02\x35\"0/v2/{parent=projects/*/agent}/generate_responses:\x01*\x12\xb5\x01\n\x17GetAlternativeSentences\x12*.ondewo.nlu.GetAlternativeSentencesRequest\x1a+.ondewo.nlu.GetAlternativeSentencesResponse\"A\x82\xd3\xe4\x93\x02;\"6/v2/{parent=projects/*/agent}/get_alternative:sentence:\x01*\x12\xcf\x01\n\x1dGetAlternativeTrainingPhrases\x12\x30.ondewo.nlu.GetAlternativeTrainingPhrasesRequest\x1a\x31.ondewo.nlu.GetAlternativeTrainingPhrasesResponse\"I\x82\xd3\xe4\x93\x02\x43\">/v2/{parent=projects/*/agent}/get_alternative:training_phrases:\x01*\x12\x85\x01\n\x0bGetSynonyms\x12\x1e.ondewo.nlu.GetSynonymsRequest\x1a\x1f.ondewo.nlu.GetSynonymsResponse\"5\x82\xd3\xe4\x93\x02/\"*/v2/{parent=projects/*/agent}/get_synonyms:\x01*\x12\x94\x01\n\x0f\x43lassifyIntents\x12\".ondewo.nlu.ClassifyIntentsRequest\x1a#.ondewo.nlu.ClassifyIntentsResponse\"8\x82\xd3\xe4\x93\x02\x32\"-/v2/{parent=projects/*/agent}/classify_intent:\x01*\x12\x64\n\x14\x45xtractEntitiesFuzzy\x12\'.ondewo.nlu.ExtractEntitiesFuzzyRequest\x1a#.ondewo.nlu.ExtractEntitiesResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bondewo/nlu/aiservices.proto\x12\nondewo.nlu\x1a\x1cgoogle/api/annotations.proto\x1a\x17ondewo/nlu/intent.proto\x1a\x1condewo/nlu/entity_type.proto\"b\n\x16\x45xtractEntitiesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12\x13\n\x0bintent_name\x18\x04 \x01(\t\"\xac\x01\n\x1b\x45xtractEntitiesFuzzyRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12@\n\x12potential_entities\x18\x03 \x03(\x0b\x32$.ondewo.nlu.EntityTypeFuzzyNerConfig\x12\x15\n\rminimal_score\x18\x04 \x01(\x02\x12\x16\n\x0e\x61llow_overlaps\x18\x05 \x01(\x08\"\x9b\x02\n\x18\x45ntityTypeFuzzyNerConfig\x12+\n\x0b\x65ntity_type\x18\x01 \x01(\x0b\x32\x16.ondewo.nlu.EntityType\x12\x15\n\rminimal_score\x18\x02 \x01(\x02\x12\x15\n\rentity_values\x18\x03 \x03(\t\x12I\n\talgorithm\x18\x04 \x01(\x0e\x32\x36.ondewo.nlu.EntityTypeFuzzyNerConfig.FuzzyNerAlgorithm\x12\x16\n\x0e\x61llow_overlaps\x18\x05 \x01(\x08\"A\n\x11\x46uzzyNerAlgorithm\x12\x19\n\x15PREFILTER_LEVENSHTEIN\x10\x00\x12\x11\n\rLOCAL_MAXIMUM\x10\x01\"t\n\x0e\x45ntityDetected\x12\x38\n\x06\x65ntity\x18\x01 \x01(\x0b\x32(.ondewo.nlu.Intent.TrainingPhrase.Entity\x12\x19\n\x11\x65xtraction_method\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x02\"^\n\x17\x45xtractEntitiesResponse\x12\x35\n\x11\x65ntities_detected\x18\x01 \x03(\x0b\x32\x1a.ondewo.nlu.EntityDetected\x12\x0c\n\x04text\x18\x02 \x01(\t\"\xbd\x01\n\x1eGetAlternativeSentencesRequest\x12\x30\n\x06\x63onfig\x18\x01 \x01(\x0b\x32 .ondewo.nlu.DataEnrichmentConfig\x12\x10\n\x08sentence\x18\x02 \x01(\t\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x0e\n\x06parent\x18\x05 \x01(\t\x12\x17\n\x0fprotected_words\x18\x06 \x03(\t\x12\x17\n\x0fwords_to_change\x18\x07 \x03(\t\"j\n\x17GenerateUserSaysRequest\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x0e\n\x06parent\x18\x05 \x01(\t\x12\x18\n\x10n_repeat_synonym\x18\x06 \x01(\x05\x12\x0e\n\x06\x62ranch\x18\x08 \x01(\t\"\x8c\x01\n\x18GenerateResponsesRequest\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x0e\n\x06parent\x18\x05 \x01(\t\x12\x18\n\x10n_repeat_synonym\x18\x07 \x01(\x05\x12\x0e\n\x06\x62ranch\x18\x08 \x01(\t\x12\x1f\n\x17\x64rop_unknown_parameters\x18\t \x01(\x08\"\xc9\x02\n$GetAlternativeTrainingPhrasesRequest\x12\x30\n\x06\x63onfig\x18\x01 \x01(\x0b\x32 .ondewo.nlu.DataEnrichmentConfig\x12:\n\x0ftraining_phrase\x18\x02 \x01(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\x12\x13\n\x0bintent_name\x18\x03 \x01(\t\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x0e\n\x06parent\x18\x05 \x01(\t\x12\x17\n\x0f\x64\x65tect_entities\x18\x06 \x01(\x08\x12\x1c\n\x14similarity_threshold\x18\x07 \x01(\x02\x12\x17\n\x0fprotected_words\x18\x08 \x03(\t\x12\x17\n\x0fwords_to_change\x18\t \x03(\t\x12\x0e\n\x06\x62ranch\x18\n \x01(\t\"{\n\x12GetSynonymsRequest\x12\x30\n\x06\x63onfig\x18\x01 \x01(\x0b\x32 .ondewo.nlu.DataEnrichmentConfig\x12\x0c\n\x04word\x18\x02 \x01(\t\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x0e\n\x06parent\x18\x05 \x01(\t\"<\n\x13GetSynonymsResponse\x12%\n\x08synonyms\x18\x01 \x03(\x0b\x32\x13.ondewo.nlu.Synonym\")\n\x07Synonym\x12\x0f\n\x07synonym\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x05\"Y\n\x1fGetAlternativeSentencesResponse\x12\x36\n\x15\x61lternative_sentences\x18\x01 \x03(\x0b\x32\x17.ondewo.nlu.AltSentence\".\n\x19GenerateResponsesResponse\x12\x11\n\tresponses\x18\x01 \x03(\t\"-\n\x18GenerateUserSaysResponse\x12\x11\n\tuser_says\x18\x01 \x03(\t\"l\n%GetAlternativeTrainingPhrasesResponse\x12\x43\n\x1c\x61lternative_training_phrases\x18\x01 \x03(\x0b\x32\x1d.ondewo.nlu.AltTrainingPhrase\".\n\x0b\x41ltSentence\x12\x10\n\x08sentence\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x02\"^\n\x11\x41ltTrainingPhrase\x12:\n\x0ftraining_phrase\x18\x01 \x01(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\x12\r\n\x05score\x18\x02 \x01(\x02\"\x98\x04\n\x14\x44\x61taEnrichmentConfig\x12=\n\x11\x65ntity_enrichment\x18\x01 \x01(\x0b\x32\".ondewo.nlu.EntityEnrichmentConfig\x12\x43\n\x14thesaurus_enrichment\x18\x02 \x01(\x0b\x32%.ondewo.nlu.ThesaurusEnrichmentConfig\x12\x41\n\x13word2vec_enrichment\x18\x03 \x01(\x0b\x32$.ondewo.nlu.Word2VecEnrichmentConfig\x12\x43\n\x13word_net_enrichment\x18\x04 \x01(\x0b\x32&.ondewo.nlu.WordNetAugEnrichmentConfig\x12\x39\n\x0fgpt2_enrichment\x18\x05 \x01(\x0b\x32 .ondewo.nlu.GPT2EnrichmentConfig\x12;\n\x10glove_enrichment\x18\x06 \x01(\x0b\x32!.ondewo.nlu.GloVeEnrichmentConfig\x12<\n\x0f\x62\x65rt_enrichment\x18\x08 \x01(\x0b\x32#.ondewo.nlu.BertAugEnrichmentConfig\x12>\n\x10xlnet_enrichment\x18\t \x01(\x0b\x32$.ondewo.nlu.XLNetAugEnrichmentConfig\"_\n\x16\x45ntityEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"b\n\x19ThesaurusEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"`\n\x17\x42\x65rtAugEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"^\n\x15GloVeEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"]\n\x14GPT2EnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"a\n\x18Word2VecEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"c\n\x1aWordNetAugEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"a\n\x18XLNetAugEnrichmentConfig\x12\x11\n\tis_active\x18\x01 \x01(\x08\x12\x19\n\x11\x65nrichment_factor\x18\x02 \x01(\x05\x12\x17\n\x0f\x65xecution_order\x18\x03 \x01(\x05\"\xcf\x01\n\x16\x43lassifyIntentsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12\x17\n\x0f\x61\x63tive_contexts\x18\x04 \x01(\x08\x12\x15\n\rcontext_names\x18\x05 \x03(\t\x12\x1e\n\x04mode\x18\x06 \x01(\x0e\x32\x10.ondewo.nlu.Mode\x12\x30\n\nalgorithms\x18\x07 \x03(\x0e\x32\x1c.ondewo.nlu.IntentAlgorithms\"g\n\x10IntentClassified\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12\x1b\n\x13intent_display_name\x18\x02 \x01(\t\x12\x12\n\nclassifier\x18\x03 \x01(\t\x12\r\n\x05score\x18\x04 \x01(\x02\"\x91\x01\n\x17\x43lassifyIntentsResponse\x12\x38\n\x12intents_classified\x18\x01 \x03(\x0b\x32\x1c.ondewo.nlu.IntentClassified\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x17\n\x0f\x61\x63tive_contexts\x18\x03 \x01(\x08\x12\x15\n\rcontext_names\x18\x04 \x03(\t*5\n\x04Mode\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\r\n\tEXCLUSIVE\x10\x01\x12\r\n\tINCLUSIVE\x10\x02*\x8c\x03\n\x10IntentAlgorithms\x12$\n OndewoIntentExactContextDetector\x10\x00\x12\x1a\n\x16OndewoIntentExactMatch\x10\x01\x12\x1f\n\x1bOndewoIntentNamedExactMatch\x10\x02\x12\x1f\n\x1bOndewoIntentSimilarityMatch\x10\x03\x12$\n OndewoIntentNamedSimilarityMatch\x10\x04\x12\x1e\n\x1aOndewoIntentBertClassifier\x10\x07\x12\x1e\n\x1aOndewoIntentMetaClassifier\x10\x08\x12\x16\n\x12IntentExitDetector\x10\n\x12\x1c\n\x18OndewoIntentRankingMatch\x10\x0b\x12\x1a\n\x16OndewoWeightedEnsemble\x10\r\x12\x1c\n\x18OndewoIntentExitDetector\x10\x0e\x12\x1e\n\x1aOndewoIntentParameterMatch\x10\x0f\x32\xf0\t\n\nAiServices\x12\x95\x01\n\x0f\x45xtractEntities\x12\".ondewo.nlu.ExtractEntitiesRequest\x1a#.ondewo.nlu.ExtractEntitiesResponse\"9\x82\xd3\xe4\x93\x02\x33\"./v2/{parent=projects/*/agent}/entities:extract:\x01*\x12\x9a\x01\n\x10GenerateUserSays\x12#.ondewo.nlu.GenerateUserSaysRequest\x1a$.ondewo.nlu.GenerateUserSaysResponse\";\x82\xd3\xe4\x93\x02\x35\"0/v2/{parent=projects/*/agent}/generate_user_says:\x01*\x12\x9d\x01\n\x11GenerateResponses\x12$.ondewo.nlu.GenerateResponsesRequest\x1a%.ondewo.nlu.GenerateResponsesResponse\";\x82\xd3\xe4\x93\x02\x35\"0/v2/{parent=projects/*/agent}/generate_responses:\x01*\x12\xb5\x01\n\x17GetAlternativeSentences\x12*.ondewo.nlu.GetAlternativeSentencesRequest\x1a+.ondewo.nlu.GetAlternativeSentencesResponse\"A\x82\xd3\xe4\x93\x02;\"6/v2/{parent=projects/*/agent}/get_alternative:sentence:\x01*\x12\xcf\x01\n\x1dGetAlternativeTrainingPhrases\x12\x30.ondewo.nlu.GetAlternativeTrainingPhrasesRequest\x1a\x31.ondewo.nlu.GetAlternativeTrainingPhrasesResponse\"I\x82\xd3\xe4\x93\x02\x43\">/v2/{parent=projects/*/agent}/get_alternative:training_phrases:\x01*\x12\x85\x01\n\x0bGetSynonyms\x12\x1e.ondewo.nlu.GetSynonymsRequest\x1a\x1f.ondewo.nlu.GetSynonymsResponse\"5\x82\xd3\xe4\x93\x02/\"*/v2/{parent=projects/*/agent}/get_synonyms:\x01*\x12\x94\x01\n\x0f\x43lassifyIntents\x12\".ondewo.nlu.ClassifyIntentsRequest\x1a#.ondewo.nlu.ClassifyIntentsResponse\"8\x82\xd3\xe4\x93\x02\x32\"-/v2/{parent=projects/*/agent}/classify_intent:\x01*\x12\x64\n\x14\x45xtractEntitiesFuzzy\x12\'.ondewo.nlu.ExtractEntitiesFuzzyRequest\x1a#.ondewo.nlu.ExtractEntitiesResponseb\x06proto3')
 
 _MODE = DESCRIPTOR.enum_types_by_name['Mode']
 Mode = enum_type_wrapper.EnumTypeWrapper(_MODE)
 _INTENTALGORITHMS = DESCRIPTOR.enum_types_by_name['IntentAlgorithms']
 IntentAlgorithms = enum_type_wrapper.EnumTypeWrapper(_INTENTALGORITHMS)
 UNSPECIFIED = 0
 EXCLUSIVE = 1
@@ -294,76 +294,76 @@
     _AISERVICES.methods_by_name['GetAlternativeSentences']._serialized_options = b'\202\323\344\223\002;\"6/v2/{parent=projects/*/agent}/get_alternative:sentence:\001*'
     _AISERVICES.methods_by_name['GetAlternativeTrainingPhrases']._options = None
     _AISERVICES.methods_by_name['GetAlternativeTrainingPhrases']._serialized_options = b'\202\323\344\223\002C\">/v2/{parent=projects/*/agent}/get_alternative:training_phrases:\001*'
     _AISERVICES.methods_by_name['GetSynonyms']._options = None
     _AISERVICES.methods_by_name['GetSynonyms']._serialized_options = b'\202\323\344\223\002/\"*/v2/{parent=projects/*/agent}/get_synonyms:\001*'
     _AISERVICES.methods_by_name['ClassifyIntents']._options = None
     _AISERVICES.methods_by_name['ClassifyIntents']._serialized_options = b'\202\323\344\223\0022\"-/v2/{parent=projects/*/agent}/classify_intent:\001*'
-    _MODE._serialized_start = 4111
-    _MODE._serialized_end = 4164
-    _INTENTALGORITHMS._serialized_start = 4167
-    _INTENTALGORITHMS._serialized_end = 4563
+    _MODE._serialized_start = 4135
+    _MODE._serialized_end = 4188
+    _INTENTALGORITHMS._serialized_start = 4191
+    _INTENTALGORITHMS._serialized_end = 4587
     _EXTRACTENTITIESREQUEST._serialized_start = 128
     _EXTRACTENTITIESREQUEST._serialized_end = 226
     _EXTRACTENTITIESFUZZYREQUEST._serialized_start = 229
     _EXTRACTENTITIESFUZZYREQUEST._serialized_end = 401
     _ENTITYTYPEFUZZYNERCONFIG._serialized_start = 404
-    _ENTITYTYPEFUZZYNERCONFIG._serialized_end = 663
-    _ENTITYTYPEFUZZYNERCONFIG_FUZZYNERALGORITHM._serialized_start = 598
-    _ENTITYTYPEFUZZYNERCONFIG_FUZZYNERALGORITHM._serialized_end = 663
-    _ENTITYDETECTED._serialized_start = 665
-    _ENTITYDETECTED._serialized_end = 781
-    _EXTRACTENTITIESRESPONSE._serialized_start = 783
-    _EXTRACTENTITIESRESPONSE._serialized_end = 877
-    _GETALTERNATIVESENTENCESREQUEST._serialized_start = 880
-    _GETALTERNATIVESENTENCESREQUEST._serialized_end = 1069
-    _GENERATEUSERSAYSREQUEST._serialized_start = 1071
-    _GENERATEUSERSAYSREQUEST._serialized_end = 1177
-    _GENERATERESPONSESREQUEST._serialized_start = 1180
-    _GENERATERESPONSESREQUEST._serialized_end = 1320
-    _GETALTERNATIVETRAININGPHRASESREQUEST._serialized_start = 1323
-    _GETALTERNATIVETRAININGPHRASESREQUEST._serialized_end = 1652
-    _GETSYNONYMSREQUEST._serialized_start = 1654
-    _GETSYNONYMSREQUEST._serialized_end = 1777
-    _GETSYNONYMSRESPONSE._serialized_start = 1779
-    _GETSYNONYMSRESPONSE._serialized_end = 1839
-    _SYNONYM._serialized_start = 1841
-    _SYNONYM._serialized_end = 1882
-    _GETALTERNATIVESENTENCESRESPONSE._serialized_start = 1884
-    _GETALTERNATIVESENTENCESRESPONSE._serialized_end = 1973
-    _GENERATERESPONSESRESPONSE._serialized_start = 1975
-    _GENERATERESPONSESRESPONSE._serialized_end = 2021
-    _GENERATEUSERSAYSRESPONSE._serialized_start = 2023
-    _GENERATEUSERSAYSRESPONSE._serialized_end = 2068
-    _GETALTERNATIVETRAININGPHRASESRESPONSE._serialized_start = 2070
-    _GETALTERNATIVETRAININGPHRASESRESPONSE._serialized_end = 2178
-    _ALTSENTENCE._serialized_start = 2180
-    _ALTSENTENCE._serialized_end = 2226
-    _ALTTRAININGPHRASE._serialized_start = 2228
-    _ALTTRAININGPHRASE._serialized_end = 2322
-    _DATAENRICHMENTCONFIG._serialized_start = 2325
-    _DATAENRICHMENTCONFIG._serialized_end = 2861
-    _ENTITYENRICHMENTCONFIG._serialized_start = 2863
-    _ENTITYENRICHMENTCONFIG._serialized_end = 2958
-    _THESAURUSENRICHMENTCONFIG._serialized_start = 2960
-    _THESAURUSENRICHMENTCONFIG._serialized_end = 3058
-    _BERTAUGENRICHMENTCONFIG._serialized_start = 3060
-    _BERTAUGENRICHMENTCONFIG._serialized_end = 3156
-    _GLOVEENRICHMENTCONFIG._serialized_start = 3158
-    _GLOVEENRICHMENTCONFIG._serialized_end = 3252
-    _GPT2ENRICHMENTCONFIG._serialized_start = 3254
-    _GPT2ENRICHMENTCONFIG._serialized_end = 3347
-    _WORD2VECENRICHMENTCONFIG._serialized_start = 3349
-    _WORD2VECENRICHMENTCONFIG._serialized_end = 3446
-    _WORDNETAUGENRICHMENTCONFIG._serialized_start = 3448
-    _WORDNETAUGENRICHMENTCONFIG._serialized_end = 3547
-    _XLNETAUGENRICHMENTCONFIG._serialized_start = 3549
-    _XLNETAUGENRICHMENTCONFIG._serialized_end = 3646
-    _CLASSIFYINTENTSREQUEST._serialized_start = 3649
-    _CLASSIFYINTENTSREQUEST._serialized_end = 3856
-    _INTENTCLASSIFIED._serialized_start = 3858
-    _INTENTCLASSIFIED._serialized_end = 3961
-    _CLASSIFYINTENTSRESPONSE._serialized_start = 3964
-    _CLASSIFYINTENTSRESPONSE._serialized_end = 4109
-    _AISERVICES._serialized_start = 4566
-    _AISERVICES._serialized_end = 5830
+    _ENTITYTYPEFUZZYNERCONFIG._serialized_end = 687
+    _ENTITYTYPEFUZZYNERCONFIG_FUZZYNERALGORITHM._serialized_start = 622
+    _ENTITYTYPEFUZZYNERCONFIG_FUZZYNERALGORITHM._serialized_end = 687
+    _ENTITYDETECTED._serialized_start = 689
+    _ENTITYDETECTED._serialized_end = 805
+    _EXTRACTENTITIESRESPONSE._serialized_start = 807
+    _EXTRACTENTITIESRESPONSE._serialized_end = 901
+    _GETALTERNATIVESENTENCESREQUEST._serialized_start = 904
+    _GETALTERNATIVESENTENCESREQUEST._serialized_end = 1093
+    _GENERATEUSERSAYSREQUEST._serialized_start = 1095
+    _GENERATEUSERSAYSREQUEST._serialized_end = 1201
+    _GENERATERESPONSESREQUEST._serialized_start = 1204
+    _GENERATERESPONSESREQUEST._serialized_end = 1344
+    _GETALTERNATIVETRAININGPHRASESREQUEST._serialized_start = 1347
+    _GETALTERNATIVETRAININGPHRASESREQUEST._serialized_end = 1676
+    _GETSYNONYMSREQUEST._serialized_start = 1678
+    _GETSYNONYMSREQUEST._serialized_end = 1801
+    _GETSYNONYMSRESPONSE._serialized_start = 1803
+    _GETSYNONYMSRESPONSE._serialized_end = 1863
+    _SYNONYM._serialized_start = 1865
+    _SYNONYM._serialized_end = 1906
+    _GETALTERNATIVESENTENCESRESPONSE._serialized_start = 1908
+    _GETALTERNATIVESENTENCESRESPONSE._serialized_end = 1997
+    _GENERATERESPONSESRESPONSE._serialized_start = 1999
+    _GENERATERESPONSESRESPONSE._serialized_end = 2045
+    _GENERATEUSERSAYSRESPONSE._serialized_start = 2047
+    _GENERATEUSERSAYSRESPONSE._serialized_end = 2092
+    _GETALTERNATIVETRAININGPHRASESRESPONSE._serialized_start = 2094
+    _GETALTERNATIVETRAININGPHRASESRESPONSE._serialized_end = 2202
+    _ALTSENTENCE._serialized_start = 2204
+    _ALTSENTENCE._serialized_end = 2250
+    _ALTTRAININGPHRASE._serialized_start = 2252
+    _ALTTRAININGPHRASE._serialized_end = 2346
+    _DATAENRICHMENTCONFIG._serialized_start = 2349
+    _DATAENRICHMENTCONFIG._serialized_end = 2885
+    _ENTITYENRICHMENTCONFIG._serialized_start = 2887
+    _ENTITYENRICHMENTCONFIG._serialized_end = 2982
+    _THESAURUSENRICHMENTCONFIG._serialized_start = 2984
+    _THESAURUSENRICHMENTCONFIG._serialized_end = 3082
+    _BERTAUGENRICHMENTCONFIG._serialized_start = 3084
+    _BERTAUGENRICHMENTCONFIG._serialized_end = 3180
+    _GLOVEENRICHMENTCONFIG._serialized_start = 3182
+    _GLOVEENRICHMENTCONFIG._serialized_end = 3276
+    _GPT2ENRICHMENTCONFIG._serialized_start = 3278
+    _GPT2ENRICHMENTCONFIG._serialized_end = 3371
+    _WORD2VECENRICHMENTCONFIG._serialized_start = 3373
+    _WORD2VECENRICHMENTCONFIG._serialized_end = 3470
+    _WORDNETAUGENRICHMENTCONFIG._serialized_start = 3472
+    _WORDNETAUGENRICHMENTCONFIG._serialized_end = 3571
+    _XLNETAUGENRICHMENTCONFIG._serialized_start = 3573
+    _XLNETAUGENRICHMENTCONFIG._serialized_end = 3670
+    _CLASSIFYINTENTSREQUEST._serialized_start = 3673
+    _CLASSIFYINTENTSREQUEST._serialized_end = 3880
+    _INTENTCLASSIFIED._serialized_start = 3882
+    _INTENTCLASSIFIED._serialized_end = 3985
+    _CLASSIFYINTENTSRESPONSE._serialized_start = 3988
+    _CLASSIFYINTENTSRESPONSE._serialized_end = 4133
+    _AISERVICES._serialized_start = 4590
+    _AISERVICES._serialized_end = 5854
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/aiservices_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/aiservices_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,45 +65,51 @@
         """Processes a natural language query and returns detected entities
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GenerateUserSays(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Generates a list of training phrases
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GenerateResponses(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Generate responses from all intents using synonyms
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetAlternativeSentences(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Generates alternative phrase based on original phrase
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetAlternativeTrainingPhrases(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Generates alternative training phrase based on original training phrase
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSynonyms(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Generates synonyms for a certain word
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ClassifyIntents(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Preprocess text and detects intents in a sentence
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ExtractEntitiesFuzzy(self, request, context):
         """Processes a natural language query and returns detected entities
         """
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/common_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/context_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/context_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18ondewo/nlu/context.proto\x12\nondewo.nlu\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\"\xa9\x02\n\x07\x43ontext\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0elifespan_count\x18\x02 \x01(\x05\x12\x37\n\nparameters\x18\x03 \x03(\x0b\x32#.ondewo.nlu.Context.ParametersEntry\x12\x15\n\rlifespan_time\x18\x04 \x01(\x02\x1aV\n\tParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x16\n\x0evalue_original\x18\x04 \x01(\t\x1aP\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x1d.ondewo.nlu.Context.Parameter:\x02\x38\x01\"9\n\x13ListContextsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x12\n\npage_token\x18\x03 \x01(\t\"V\n\x14ListContextsResponse\x12%\n\x08\x63ontexts\x18\x01 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"!\n\x11GetContextRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"L\n\x14\x43reateContextRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12$\n\x07\x63ontext\x18\x02 \x01(\x0b\x32\x13.ondewo.nlu.Context\"m\n\x14UpdateContextRequest\x12$\n\x07\x63ontext\x18\x01 \x01(\x0b\x32\x13.ondewo.nlu.Context\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"$\n\x14\x44\x65leteContextRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"*\n\x18\x44\x65leteAllContextsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t2\xce\x06\n\x08\x43ontexts\x12\x8c\x01\n\x0cListContexts\x12\x1f.ondewo.nlu.ListContextsRequest\x1a .ondewo.nlu.ListContextsResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v2/{parent=projects/*/agent/sessions/*}/contexts\x12{\n\nGetContext\x12\x1d.ondewo.nlu.GetContextRequest\x1a\x13.ondewo.nlu.Context\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v2/{name=projects/*/agent/sessions/*/contexts/*}\x12\x8a\x01\n\rCreateContext\x12 .ondewo.nlu.CreateContextRequest\x1a\x13.ondewo.nlu.Context\"B\x82\xd3\xe4\x93\x02<\"1/v2/{parent=projects/*/agent/sessions/*}/contexts:\x07\x63ontext\x12\x92\x01\n\rUpdateContext\x12 .ondewo.nlu.UpdateContextRequest\x1a\x13.ondewo.nlu.Context\"J\x82\xd3\xe4\x93\x02\x44\x32\x39/v2/{context.name=projects/*/agent/sessions/*/contexts/*}:\x07\x63ontext\x12\x84\x01\n\rDeleteContext\x12 .ondewo.nlu.DeleteContextRequest\x1a\x16.google.protobuf.Empty\"9\x82\xd3\xe4\x93\x02\x33*1/v2/{name=projects/*/agent/sessions/*/contexts/*}\x12\x8c\x01\n\x11\x44\x65leteAllContexts\x12$.ondewo.nlu.DeleteAllContextsRequest\x1a\x16.google.protobuf.Empty\"9\x82\xd3\xe4\x93\x02\x33*1/v2/{parent=projects/*/agent/sessions/*}/contextsB\x9b\x01\n\x1e\x63om.google.cloud.dialogflow.v2B\x0c\x43ontextProtoP\x01ZDgoogle.golang.org/genproto/googleapis/cloud/dialogflow/v2;dialogflow\xf8\x01\x01\xa2\x02\x02\x44\x46\xaa\x02\x1aGoogle.Cloud.Dialogflow.V2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18ondewo/nlu/context.proto\x12\nondewo.nlu\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\"\xa9\x02\n\x07\x43ontext\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x16\n\x0elifespan_count\x18\x02 \x01(\x05\x12\x37\n\nparameters\x18\x03 \x03(\x0b\x32#.ondewo.nlu.Context.ParametersEntry\x12\x15\n\rlifespan_time\x18\x04 \x01(\x02\x1aV\n\tParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x16\n\x0evalue_original\x18\x04 \x01(\t\x1aP\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x1d.ondewo.nlu.Context.Parameter:\x02\x38\x01\"=\n\x13ListContextsRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x12\n\npage_token\x18\x03 \x01(\t\"V\n\x14ListContextsResponse\x12%\n\x08\x63ontexts\x18\x01 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"!\n\x11GetContextRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"P\n\x14\x43reateContextRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12$\n\x07\x63ontext\x18\x02 \x01(\x0b\x32\x13.ondewo.nlu.Context\"m\n\x14UpdateContextRequest\x12$\n\x07\x63ontext\x18\x01 \x01(\x0b\x32\x13.ondewo.nlu.Context\x12/\n\x0bupdate_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"$\n\x14\x44\x65leteContextRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\".\n\x18\x44\x65leteAllContextsRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t2\xce\x06\n\x08\x43ontexts\x12\x8c\x01\n\x0cListContexts\x12\x1f.ondewo.nlu.ListContextsRequest\x1a .ondewo.nlu.ListContextsResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v2/{parent=projects/*/agent/sessions/*}/contexts\x12{\n\nGetContext\x12\x1d.ondewo.nlu.GetContextRequest\x1a\x13.ondewo.nlu.Context\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v2/{name=projects/*/agent/sessions/*/contexts/*}\x12\x8a\x01\n\rCreateContext\x12 .ondewo.nlu.CreateContextRequest\x1a\x13.ondewo.nlu.Context\"B\x82\xd3\xe4\x93\x02<\"1/v2/{parent=projects/*/agent/sessions/*}/contexts:\x07\x63ontext\x12\x92\x01\n\rUpdateContext\x12 .ondewo.nlu.UpdateContextRequest\x1a\x13.ondewo.nlu.Context\"J\x82\xd3\xe4\x93\x02\x44\x32\x39/v2/{context.name=projects/*/agent/sessions/*/contexts/*}:\x07\x63ontext\x12\x84\x01\n\rDeleteContext\x12 .ondewo.nlu.DeleteContextRequest\x1a\x16.google.protobuf.Empty\"9\x82\xd3\xe4\x93\x02\x33*1/v2/{name=projects/*/agent/sessions/*/contexts/*}\x12\x8c\x01\n\x11\x44\x65leteAllContexts\x12$.ondewo.nlu.DeleteAllContextsRequest\x1a\x16.google.protobuf.Empty\"9\x82\xd3\xe4\x93\x02\x33*1/v2/{parent=projects/*/agent/sessions/*}/contextsB\x9b\x01\n\x1e\x63om.google.cloud.dialogflow.v2B\x0c\x43ontextProtoP\x01ZDgoogle.golang.org/genproto/googleapis/cloud/dialogflow/v2;dialogflow\xf8\x01\x01\xa2\x02\x02\x44\x46\xaa\x02\x1aGoogle.Cloud.Dialogflow.V2b\x06proto3')
 
 
 _CONTEXT = DESCRIPTOR.message_types_by_name['Context']
 _CONTEXT_PARAMETER = _CONTEXT.nested_types_by_name['Parameter']
 _CONTEXT_PARAMETERSENTRY = _CONTEXT.nested_types_by_name['ParametersEntry']
 _LISTCONTEXTSREQUEST = DESCRIPTOR.message_types_by_name['ListContextsRequest']
 _LISTCONTEXTSRESPONSE = DESCRIPTOR.message_types_by_name['ListContextsResponse']
@@ -120,23 +120,23 @@
     _CONTEXT._serialized_start = 134
     _CONTEXT._serialized_end = 431
     _CONTEXT_PARAMETER._serialized_start = 263
     _CONTEXT_PARAMETER._serialized_end = 349
     _CONTEXT_PARAMETERSENTRY._serialized_start = 351
     _CONTEXT_PARAMETERSENTRY._serialized_end = 431
     _LISTCONTEXTSREQUEST._serialized_start = 433
-    _LISTCONTEXTSREQUEST._serialized_end = 490
-    _LISTCONTEXTSRESPONSE._serialized_start = 492
-    _LISTCONTEXTSRESPONSE._serialized_end = 578
-    _GETCONTEXTREQUEST._serialized_start = 580
-    _GETCONTEXTREQUEST._serialized_end = 613
-    _CREATECONTEXTREQUEST._serialized_start = 615
-    _CREATECONTEXTREQUEST._serialized_end = 691
-    _UPDATECONTEXTREQUEST._serialized_start = 693
-    _UPDATECONTEXTREQUEST._serialized_end = 802
-    _DELETECONTEXTREQUEST._serialized_start = 804
-    _DELETECONTEXTREQUEST._serialized_end = 840
-    _DELETEALLCONTEXTSREQUEST._serialized_start = 842
-    _DELETEALLCONTEXTSREQUEST._serialized_end = 884
-    _CONTEXTS._serialized_start = 887
-    _CONTEXTS._serialized_end = 1733
+    _LISTCONTEXTSREQUEST._serialized_end = 494
+    _LISTCONTEXTSRESPONSE._serialized_start = 496
+    _LISTCONTEXTSRESPONSE._serialized_end = 582
+    _GETCONTEXTREQUEST._serialized_start = 584
+    _GETCONTEXTREQUEST._serialized_end = 617
+    _CREATECONTEXTREQUEST._serialized_start = 619
+    _CREATECONTEXTREQUEST._serialized_end = 699
+    _UPDATECONTEXTREQUEST._serialized_start = 701
+    _UPDATECONTEXTREQUEST._serialized_end = 810
+    _DELETECONTEXTREQUEST._serialized_start = 812
+    _DELETECONTEXTREQUEST._serialized_end = 848
+    _DELETEALLCONTEXTSREQUEST._serialized_start = 850
+    _DELETEALLCONTEXTSREQUEST._serialized_end = 896
+    _CONTEXTS._serialized_start = 899
+    _CONTEXTS._serialized_end = 1745
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/context_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/context_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/entity_type_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/entity_type_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,24 +14,25 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1condewo/nlu/entity_type.proto\x12\nondewo.nlu\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a\x17ondewo/nlu/common.proto\x1a\x1bondewo/nlu/operations.proto\"\x93\x05\n\nEntityType\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12)\n\x04kind\x18\x03 \x01(\x0e\x32\x1b.ondewo.nlu.EntityType.Kind\x12\x45\n\x13\x61uto_expansion_mode\x18\x04 \x01(\x0e\x32(.ondewo.nlu.EntityType.AutoExpansionMode\x12/\n\x08\x65ntities\x18\x06 \x03(\x0b\x32\x1d.ondewo.nlu.EntityType.Entity\x12\x17\n\x0fnext_page_token\x18\n \x01(\t\x12\x14\n\x0c\x65ntity_count\x18\x0b \x01(\x05\x12\x37\n\x06status\x18\x0c \x01(\x0e\x32\'.ondewo.nlu.EntityType.EntityTypeStatus\x12\x15\n\rsynonym_count\x18\r \x01(\x05\x1a{\n\x06\x45ntity\x12\r\n\x05value\x18\x01 \x01(\t\x12\x10\n\x08synonyms\x18\x02 \x03(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x04 \x01(\t\x12\x15\n\rsynonym_count\x18\x05 \x01(\x05\x12\x15\n\rlanguage_code\x18\x06 \x01(\t\"9\n\x04Kind\x12\x14\n\x10KIND_UNSPECIFIED\x10\x00\x12\x0c\n\x08KIND_MAP\x10\x01\x12\r\n\tKIND_LIST\x10\x02\",\n\x10\x45ntityTypeStatus\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08INACTIVE\x10\x01\"Y\n\x11\x41utoExpansionMode\x12#\n\x1f\x41UTO_EXPANSION_MODE_UNSPECIFIED\x10\x00\x12\x1f\n\x1b\x41UTO_EXPANSION_MODE_DEFAULT\x10\x01\"\xfb\x01\n\x16ListEntityTypesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x34\n\x10\x65ntity_type_view\x18\x05 \x01(\x0e\x32\x1a.ondewo.nlu.EntityTypeView\x12:\n\x12\x66ilter_by_category\x18\x06 \x01(\x0e\x32\x1e.ondewo.nlu.EntityTypeCategory\x12\x34\n\rsort_by_field\x18\x07 \x01(\x0b\x32\x1d.ondewo.nlu.EntityTypeSorting\"`\n\x17ListEntityTypesResponse\x12,\n\x0c\x65ntity_types\x18\x01 \x03(\x0b\x32\x16.ondewo.nlu.EntityType\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x85\x01\n\x14GetEntityTypeRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\npage_token\x18\x05 \x01(\t\x12\x34\n\x10\x65ntity_type_view\x18\x06 \x01(\x0e\x32\x1a.ondewo.nlu.EntityTypeView\"\xa3\x01\n\x17\x43reateEntityTypeRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12+\n\x0b\x65ntity_type\x18\x02 \x01(\x0b\x32\x16.ondewo.nlu.EntityType\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12\x34\n\x10\x65ntity_type_view\x18\x06 \x01(\x0e\x32\x1a.ondewo.nlu.EntityTypeView\"\xc4\x01\n\x17UpdateEntityTypeRequest\x12+\n\x0b\x65ntity_type\x18\x01 \x01(\x0b\x32\x16.ondewo.nlu.EntityType\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12/\n\x0bupdate_mask\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12\x34\n\x10\x65ntity_type_view\x18\x06 \x01(\x0e\x32\x1a.ondewo.nlu.EntityTypeView\"\'\n\x17\x44\x65leteEntityTypeRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xee\x01\n\x1d\x42\x61tchUpdateEntityTypesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x1f\n\x15\x65ntity_type_batch_uri\x18\x02 \x01(\tH\x00\x12?\n\x18\x65ntity_type_batch_inline\x18\x03 \x01(\x0b\x32\x1b.ondewo.nlu.EntityTypeBatchH\x00\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12/\n\x0bupdate_mask\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskB\x13\n\x11\x65ntity_type_batch\"N\n\x1e\x42\x61tchUpdateEntityTypesResponse\x12,\n\x0c\x65ntity_types\x18\x01 \x03(\x0b\x32\x16.ondewo.nlu.EntityType\"J\n\x1d\x42\x61tchDeleteEntityTypesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x19\n\x11\x65ntity_type_names\x18\x02 \x03(\t\"?\n\x0f\x45ntityTypeBatch\x12,\n\x0c\x65ntity_types\x18\x01 \x03(\x0b\x32\x16.ondewo.nlu.EntityType\"\x84\x03\n\x11\x45ntityTypeSorting\x12K\n\rsorting_field\x18\x01 \x01(\x0e\x32\x34.ondewo.nlu.EntityTypeSorting.EntityTypeSortingField\x12-\n\x0csorting_mode\x18\x02 \x01(\x0e\x32\x17.ondewo.nlu.SortingMode\"\xf2\x01\n\x16\x45ntityTypeSortingField\x12\x1a\n\x16NO_ENTITY_TYPE_SORTING\x10\x00\x12\x1c\n\x18SORT_ENTITY_TYPE_BY_NAME\x10\x01\x12%\n!SORT_ENTITY_TYPE_BY_CREATION_DATE\x10\x02\x12$\n SORT_ENTITY_TYPE_BY_LAST_UPDATED\x10\x03\x12*\n&SORT_ENTITY_TYPE_BY_ENTITY_VALUE_COUNT\x10\x04\x12%\n!SORT_ENTITY_TYPE_BY_SYNONYM_COUNT\x10\x05\"\xe2\x01\n\x15\x42\x61tchEntitiesResponse\x12G\n\x0f\x65ntity_statuses\x18\x01 \x03(\x0b\x32..ondewo.nlu.BatchEntitiesResponse.EntityStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\x1al\n\x0c\x45ntityStatus\x12/\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1d.ondewo.nlu.EntityType.EntityH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x12\n\x10\x65ntity_or_status\"\xd8\x01\n\x1a\x42\x61tchCreateEntitiesRequest\x12Z\n\x16\x63reate_entity_requests\x18\x01 \x03(\x0b\x32:.ondewo.nlu.BatchCreateEntitiesRequest.CreateEntityRequest\x1a^\n\x13\x43reateEntityRequest\x12\x18\n\x10\x65ntity_type_name\x18\x01 \x01(\t\x12-\n\x06\x65ntity\x18\x02 \x01(\x0b\x32\x1d.ondewo.nlu.EntityType.Entity\"M\n\x1a\x42\x61tchUpdateEntitiesRequest\x12/\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x1d.ondewo.nlu.EntityType.Entity\"(\n\x17\x42\x61tchGetEntitiesRequest\x12\r\n\x05names\x18\x01 \x03(\t\"+\n\x1a\x42\x61tchDeleteEntitiesRequest\x12\r\n\x05names\x18\x01 \x03(\t\"\xfe\x01\n\x1b\x42\x61tchDeleteEntitiesResponse\x12S\n\x0f\x64\x65lete_statuses\x18\x01 \x03(\x0b\x32:.ondewo.nlu.BatchDeleteEntitiesResponse.DeleteEntityStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\x1av\n\x12\x44\x65leteEntityStatus\x12\x36\n\x14successfully_deleted\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x0f\n\rdelete_status\"\xac\x01\n\x13ListEntitiesRequest\x12\x18\n\x10\x65ntity_type_name\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x35\n\rsort_by_field\x18\x05 \x01(\x0b\x32\x1e.ondewo.nlu.EntityValueSorting\x12\x19\n\x11search_by_pattern\x18\x06 \x01(\t\"`\n\x14ListEntitiesResponse\x12/\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x1d.ondewo.nlu.EntityType.Entity\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xba\x02\n\x12\x45ntityValueSorting\x12M\n\rsorting_field\x18\x07 \x01(\x0e\x32\x36.ondewo.nlu.EntityValueSorting.EntityValueSortingField\x12-\n\x0csorting_mode\x18\x08 \x01(\x0e\x32\x17.ondewo.nlu.SortingMode\"\xa5\x01\n\x17\x45ntityValueSortingField\x12\x1b\n\x17NO_ENTITY_VALUE_SORTING\x10\x00\x12%\n!SORT_ENTITY_VALUE_BY_DISPLAY_NAME\x10\x01\x12\x1e\n\x1aSORT_ENTITY_VALUE_BY_VALUE\x10\x02\x12&\n\"SORT_ENTITY_VALUE_BY_SYNONYM_COUNT\x10\x03*\x89\x01\n\x0e\x45ntityTypeView\x12 \n\x1c\x45NTITY_TYPE_VIEW_UNSPECIFIED\x10\x00\x12\x19\n\x15\x45NTITY_TYPE_VIEW_FULL\x10\x01\x12\x1c\n\x18\x45NTITY_TYPE_VIEW_PARTIAL\x10\x02\x12\x1c\n\x18\x45NTITY_TYPE_VIEW_SHALLOW\x10\x03*c\n\x12\x45ntityTypeCategory\x12\x14\n\x10\x41LL_ENTITY_TYPES\x10\x00\x12\x18\n\x14\x44\x45\x46\x41ULT_ENTITY_TYPES\x10\x01\x12\x1d\n\x19USER_DEFINED_ENTITY_TYPES\x10\x02\x32\xd5\x0b\n\x0b\x45ntityTypes\x12\x8d\x01\n\x0fListEntityTypes\x12\".ondewo.nlu.ListEntityTypesRequest\x1a#.ondewo.nlu.ListEntityTypesResponse\"1\x82\xd3\xe4\x93\x02+\x12)/v2/{parent=projects/*/agent}/entityTypes\x12|\n\rGetEntityType\x12 .ondewo.nlu.GetEntityTypeRequest\x1a\x16.ondewo.nlu.EntityType\"1\x82\xd3\xe4\x93\x02+\x12)/v2/{name=projects/*/agent/entityTypes/*}\x12\x85\x01\n\x10\x43reateEntityType\x12#.ondewo.nlu.CreateEntityTypeRequest\x1a\x16.ondewo.nlu.EntityType\"4\x82\xd3\xe4\x93\x02.\")/v2/{parent=projects/*/agent}/entityTypes:\x01*\x12\x91\x01\n\x10UpdateEntityType\x12#.ondewo.nlu.UpdateEntityTypeRequest\x1a\x16.ondewo.nlu.EntityType\"@\x82\xd3\xe4\x93\x02:25/v2/{entity_type.name=projects/*/agent/entityTypes/*}:\x01*\x12\x82\x01\n\x10\x44\x65leteEntityType\x12#.ondewo.nlu.DeleteEntityTypeRequest\x1a\x16.google.protobuf.Empty\"1\x82\xd3\xe4\x93\x02+*)/v2/{name=projects/*/agent/entityTypes/*}\x12\x9c\x01\n\x16\x42\x61tchUpdateEntityTypes\x12).ondewo.nlu.BatchUpdateEntityTypesRequest\x1a\x15.ondewo.nlu.Operation\"@\x82\xd3\xe4\x93\x02:\"5/v2/{parent=projects/*/agent}/entityTypes:batchUpdate:\x01*\x12\x9c\x01\n\x16\x42\x61tchDeleteEntityTypes\x12).ondewo.nlu.BatchDeleteEntityTypesRequest\x1a\x15.ondewo.nlu.Operation\"@\x82\xd3\xe4\x93\x02:\"5/v2/{parent=projects/*/agent}/entityTypes:batchDelete:\x01*\x12`\n\x13\x42\x61tchCreateEntities\x12&.ondewo.nlu.BatchCreateEntitiesRequest\x1a!.ondewo.nlu.BatchEntitiesResponse\x12`\n\x13\x42\x61tchUpdateEntities\x12&.ondewo.nlu.BatchUpdateEntitiesRequest\x1a!.ondewo.nlu.BatchEntitiesResponse\x12Z\n\x10\x42\x61tchGetEntities\x12#.ondewo.nlu.BatchGetEntitiesRequest\x1a!.ondewo.nlu.BatchEntitiesResponse\x12\x66\n\x13\x42\x61tchDeleteEntities\x12&.ondewo.nlu.BatchDeleteEntitiesRequest\x1a\'.ondewo.nlu.BatchDeleteEntitiesResponse\x12Q\n\x0cListEntities\x12\x1f.ondewo.nlu.ListEntitiesRequest\x1a .ondewo.nlu.ListEntitiesResponseB\x9e\x01\n\x1e\x63om.google.cloud.dialogflow.v2B\x0f\x45ntityTypeProtoP\x01ZDgoogle.golang.org/genproto/googleapis/cloud/dialogflow/v2;dialogflow\xf8\x01\x01\xa2\x02\x02\x44\x46\xaa\x02\x1aGoogle.Cloud.Dialogflow.V2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1condewo/nlu/entity_type.proto\x12\nondewo.nlu\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a\x17ondewo/nlu/common.proto\x1a\x1bondewo/nlu/operations.proto\"\x93\x05\n\nEntityType\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12)\n\x04kind\x18\x03 \x01(\x0e\x32\x1b.ondewo.nlu.EntityType.Kind\x12\x45\n\x13\x61uto_expansion_mode\x18\x04 \x01(\x0e\x32(.ondewo.nlu.EntityType.AutoExpansionMode\x12/\n\x08\x65ntities\x18\x06 \x03(\x0b\x32\x1d.ondewo.nlu.EntityType.Entity\x12\x17\n\x0fnext_page_token\x18\n \x01(\t\x12\x14\n\x0c\x65ntity_count\x18\x0b \x01(\x05\x12\x37\n\x06status\x18\x0c \x01(\x0e\x32\'.ondewo.nlu.EntityType.EntityTypeStatus\x12\x15\n\rsynonym_count\x18\r \x01(\x05\x1a{\n\x06\x45ntity\x12\r\n\x05value\x18\x01 \x01(\t\x12\x10\n\x08synonyms\x18\x02 \x03(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x04 \x01(\t\x12\x15\n\rsynonym_count\x18\x05 \x01(\x05\x12\x15\n\rlanguage_code\x18\x06 \x01(\t\"9\n\x04Kind\x12\x14\n\x10KIND_UNSPECIFIED\x10\x00\x12\x0c\n\x08KIND_MAP\x10\x01\x12\r\n\tKIND_LIST\x10\x02\",\n\x10\x45ntityTypeStatus\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08INACTIVE\x10\x01\"Y\n\x11\x41utoExpansionMode\x12#\n\x1f\x41UTO_EXPANSION_MODE_UNSPECIFIED\x10\x00\x12\x1f\n\x1b\x41UTO_EXPANSION_MODE_DEFAULT\x10\x01\"\xfb\x01\n\x16ListEntityTypesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x34\n\x10\x65ntity_type_view\x18\x05 \x01(\x0e\x32\x1a.ondewo.nlu.EntityTypeView\x12:\n\x12\x66ilter_by_category\x18\x06 \x01(\x0e\x32\x1e.ondewo.nlu.EntityTypeCategory\x12\x34\n\rsort_by_field\x18\x07 \x01(\x0b\x32\x1d.ondewo.nlu.EntityTypeSorting\"`\n\x17ListEntityTypesResponse\x12,\n\x0c\x65ntity_types\x18\x01 \x03(\x0b\x32\x16.ondewo.nlu.EntityType\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x85\x01\n\x14GetEntityTypeRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\npage_token\x18\x05 \x01(\t\x12\x34\n\x10\x65ntity_type_view\x18\x06 \x01(\x0e\x32\x1a.ondewo.nlu.EntityTypeView\"\xa3\x01\n\x17\x43reateEntityTypeRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12+\n\x0b\x65ntity_type\x18\x02 \x01(\x0b\x32\x16.ondewo.nlu.EntityType\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12\x34\n\x10\x65ntity_type_view\x18\x06 \x01(\x0e\x32\x1a.ondewo.nlu.EntityTypeView\"\xc4\x01\n\x17UpdateEntityTypeRequest\x12+\n\x0b\x65ntity_type\x18\x01 \x01(\x0b\x32\x16.ondewo.nlu.EntityType\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12/\n\x0bupdate_mask\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12\x34\n\x10\x65ntity_type_view\x18\x06 \x01(\x0e\x32\x1a.ondewo.nlu.EntityTypeView\"\'\n\x17\x44\x65leteEntityTypeRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xee\x01\n\x1d\x42\x61tchUpdateEntityTypesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x1f\n\x15\x65ntity_type_batch_uri\x18\x02 \x01(\tH\x00\x12?\n\x18\x65ntity_type_batch_inline\x18\x03 \x01(\x0b\x32\x1b.ondewo.nlu.EntityTypeBatchH\x00\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12/\n\x0bupdate_mask\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskB\x13\n\x11\x65ntity_type_batch\"N\n\x1e\x42\x61tchUpdateEntityTypesResponse\x12,\n\x0c\x65ntity_types\x18\x01 \x03(\x0b\x32\x16.ondewo.nlu.EntityType\"J\n\x1d\x42\x61tchDeleteEntityTypesRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x19\n\x11\x65ntity_type_names\x18\x02 \x03(\t\"?\n\x0f\x45ntityTypeBatch\x12,\n\x0c\x65ntity_types\x18\x01 \x03(\x0b\x32\x16.ondewo.nlu.EntityType\"\x84\x03\n\x11\x45ntityTypeSorting\x12K\n\rsorting_field\x18\x01 \x01(\x0e\x32\x34.ondewo.nlu.EntityTypeSorting.EntityTypeSortingField\x12-\n\x0csorting_mode\x18\x02 \x01(\x0e\x32\x17.ondewo.nlu.SortingMode\"\xf2\x01\n\x16\x45ntityTypeSortingField\x12\x1a\n\x16NO_ENTITY_TYPE_SORTING\x10\x00\x12\x1c\n\x18SORT_ENTITY_TYPE_BY_NAME\x10\x01\x12%\n!SORT_ENTITY_TYPE_BY_CREATION_DATE\x10\x02\x12$\n SORT_ENTITY_TYPE_BY_LAST_UPDATED\x10\x03\x12*\n&SORT_ENTITY_TYPE_BY_ENTITY_VALUE_COUNT\x10\x04\x12%\n!SORT_ENTITY_TYPE_BY_SYNONYM_COUNT\x10\x05\"l\n\x0c\x45ntityStatus\x12/\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1d.ondewo.nlu.EntityType.EntityH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x12\n\x10\x65ntity_or_status\"^\n\x15\x42\x61tchEntitiesResponse\x12\x31\n\x0f\x65ntity_statuses\x18\x01 \x03(\x0b\x32\x18.ondewo.nlu.EntityStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\"^\n\x13\x43reateEntityRequest\x12\x18\n\x10\x65ntity_type_name\x18\x01 \x01(\t\x12-\n\x06\x65ntity\x18\x02 \x01(\x0b\x32\x1d.ondewo.nlu.EntityType.Entity\"]\n\x1a\x42\x61tchCreateEntitiesRequest\x12?\n\x16\x63reate_entity_requests\x18\x01 \x03(\x0b\x32\x1f.ondewo.nlu.CreateEntityRequest\"M\n\x1a\x42\x61tchUpdateEntitiesRequest\x12/\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x1d.ondewo.nlu.EntityType.Entity\"D\n\x13UpdateEntityRequest\x12-\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x1d.ondewo.nlu.EntityType.Entity\" \n\x10GetEntityRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"(\n\x17\x42\x61tchGetEntitiesRequest\x12\r\n\x05names\x18\x01 \x03(\t\"+\n\x1a\x42\x61tchDeleteEntitiesRequest\x12\r\n\x05names\x18\x01 \x03(\t\"#\n\x13\x44\x65leteEntityRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"v\n\x12\x44\x65leteEntityStatus\x12\x36\n\x14successfully_deleted\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x0f\n\rdelete_status\"j\n\x1b\x42\x61tchDeleteEntitiesResponse\x12\x37\n\x0f\x64\x65lete_statuses\x18\x01 \x03(\x0b\x32\x1e.ondewo.nlu.DeleteEntityStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\"\xac\x01\n\x13ListEntitiesRequest\x12\x18\n\x10\x65ntity_type_name\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x35\n\rsort_by_field\x18\x05 \x01(\x0b\x32\x1e.ondewo.nlu.EntityValueSorting\x12\x19\n\x11search_by_pattern\x18\x06 \x01(\t\"`\n\x14ListEntitiesResponse\x12/\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x1d.ondewo.nlu.EntityType.Entity\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xba\x02\n\x12\x45ntityValueSorting\x12M\n\rsorting_field\x18\x07 \x01(\x0e\x32\x36.ondewo.nlu.EntityValueSorting.EntityValueSortingField\x12-\n\x0csorting_mode\x18\x08 \x01(\x0e\x32\x17.ondewo.nlu.SortingMode\"\xa5\x01\n\x17\x45ntityValueSortingField\x12\x1b\n\x17NO_ENTITY_VALUE_SORTING\x10\x00\x12%\n!SORT_ENTITY_VALUE_BY_DISPLAY_NAME\x10\x01\x12\x1e\n\x1aSORT_ENTITY_VALUE_BY_VALUE\x10\x02\x12&\n\"SORT_ENTITY_VALUE_BY_SYNONYM_COUNT\x10\x03*\xa7\x01\n\x0e\x45ntityTypeView\x12 \n\x1c\x45NTITY_TYPE_VIEW_UNSPECIFIED\x10\x00\x12\x19\n\x15\x45NTITY_TYPE_VIEW_FULL\x10\x01\x12\x1c\n\x18\x45NTITY_TYPE_VIEW_PARTIAL\x10\x02\x12\x1c\n\x18\x45NTITY_TYPE_VIEW_SHALLOW\x10\x03\x12\x1c\n\x18\x45NTITY_TYPE_VIEW_MINIMUM\x10\x04*c\n\x12\x45ntityTypeCategory\x12\x14\n\x10\x41LL_ENTITY_TYPES\x10\x00\x12\x18\n\x14\x44\x45\x46\x41ULT_ENTITY_TYPES\x10\x01\x12\x1d\n\x19USER_DEFINED_ENTITY_TYPES\x10\x02\x32\x9b\x10\n\x0b\x45ntityTypes\x12\x8d\x01\n\x0fListEntityTypes\x12\".ondewo.nlu.ListEntityTypesRequest\x1a#.ondewo.nlu.ListEntityTypesResponse\"1\x82\xd3\xe4\x93\x02+\x12)/v2/{parent=projects/*/agent}/entityTypes\x12|\n\rGetEntityType\x12 .ondewo.nlu.GetEntityTypeRequest\x1a\x16.ondewo.nlu.EntityType\"1\x82\xd3\xe4\x93\x02+\x12)/v2/{name=projects/*/agent/entityTypes/*}\x12\x85\x01\n\x10\x43reateEntityType\x12#.ondewo.nlu.CreateEntityTypeRequest\x1a\x16.ondewo.nlu.EntityType\"4\x82\xd3\xe4\x93\x02.\")/v2/{parent=projects/*/agent}/entityTypes:\x01*\x12\x91\x01\n\x10UpdateEntityType\x12#.ondewo.nlu.UpdateEntityTypeRequest\x1a\x16.ondewo.nlu.EntityType\"@\x82\xd3\xe4\x93\x02:25/v2/{entity_type.name=projects/*/agent/entityTypes/*}:\x01*\x12\x82\x01\n\x10\x44\x65leteEntityType\x12#.ondewo.nlu.DeleteEntityTypeRequest\x1a\x16.google.protobuf.Empty\"1\x82\xd3\xe4\x93\x02+*)/v2/{name=projects/*/agent/entityTypes/*}\x12\x9c\x01\n\x16\x42\x61tchUpdateEntityTypes\x12).ondewo.nlu.BatchUpdateEntityTypesRequest\x1a\x15.ondewo.nlu.Operation\"@\x82\xd3\xe4\x93\x02:\"5/v2/{parent=projects/*/agent}/entityTypes:batchUpdate:\x01*\x12\x9c\x01\n\x16\x42\x61tchDeleteEntityTypes\x12).ondewo.nlu.BatchDeleteEntityTypesRequest\x1a\x15.ondewo.nlu.Operation\"@\x82\xd3\xe4\x93\x02:\"5/v2/{parent=projects/*/agent}/entityTypes:batchDelete:\x01*\x12\x86\x01\n\tGetEntity\x12\x1c.ondewo.nlu.GetEntityRequest\x1a\x1d.ondewo.nlu.EntityType.Entity\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/v2/{name=projects/*/agent/entityTypes/*/entities/*}\x12\x90\x01\n\x0c\x43reateEntity\x12\x1f.ondewo.nlu.CreateEntityRequest\x1a\x1d.ondewo.nlu.EntityType.Entity\"@\x82\xd3\xe4\x93\x02:\"5/v2/{parent=projects/*/agent}/entityTypes/*/entities/:\x01*\x12\x97\x01\n\x0cUpdateEntity\x12\x1f.ondewo.nlu.UpdateEntityRequest\x1a\x1d.ondewo.nlu.EntityType.Entity\"G\x82\xd3\xe4\x93\x02\x41\x32</v2/{entity_.name=projects/*/agent/entityTypes/*/entities/*}:\x01*\x12\x8d\x01\n\x0c\x44\x65leteEntity\x12\x1f.ondewo.nlu.DeleteEntityRequest\x1a\x1e.ondewo.nlu.DeleteEntityStatus\"<\x82\xd3\xe4\x93\x02\x36*4/v2/{name=projects/*/agent/entityTypes/*/entities/*}\x12`\n\x13\x42\x61tchCreateEntities\x12&.ondewo.nlu.BatchCreateEntitiesRequest\x1a!.ondewo.nlu.BatchEntitiesResponse\x12`\n\x13\x42\x61tchUpdateEntities\x12&.ondewo.nlu.BatchUpdateEntitiesRequest\x1a!.ondewo.nlu.BatchEntitiesResponse\x12Z\n\x10\x42\x61tchGetEntities\x12#.ondewo.nlu.BatchGetEntitiesRequest\x1a!.ondewo.nlu.BatchEntitiesResponse\x12\x66\n\x13\x42\x61tchDeleteEntities\x12&.ondewo.nlu.BatchDeleteEntitiesRequest\x1a\'.ondewo.nlu.BatchDeleteEntitiesResponse\x12Q\n\x0cListEntities\x12\x1f.ondewo.nlu.ListEntitiesRequest\x1a .ondewo.nlu.ListEntitiesResponseB\x9e\x01\n\x1e\x63om.google.cloud.dialogflow.v2B\x0f\x45ntityTypeProtoP\x01ZDgoogle.golang.org/genproto/googleapis/cloud/dialogflow/v2;dialogflow\xf8\x01\x01\xa2\x02\x02\x44\x46\xaa\x02\x1aGoogle.Cloud.Dialogflow.V2b\x06proto3')
 
 _ENTITYTYPEVIEW = DESCRIPTOR.enum_types_by_name['EntityTypeView']
 EntityTypeView = enum_type_wrapper.EnumTypeWrapper(_ENTITYTYPEVIEW)
 _ENTITYTYPECATEGORY = DESCRIPTOR.enum_types_by_name['EntityTypeCategory']
 EntityTypeCategory = enum_type_wrapper.EnumTypeWrapper(_ENTITYTYPECATEGORY)
 ENTITY_TYPE_VIEW_UNSPECIFIED = 0
 ENTITY_TYPE_VIEW_FULL = 1
 ENTITY_TYPE_VIEW_PARTIAL = 2
 ENTITY_TYPE_VIEW_SHALLOW = 3
+ENTITY_TYPE_VIEW_MINIMUM = 4
 ALL_ENTITY_TYPES = 0
 DEFAULT_ENTITY_TYPES = 1
 USER_DEFINED_ENTITY_TYPES = 2
 
 
 _ENTITYTYPE = DESCRIPTOR.message_types_by_name['EntityType']
 _ENTITYTYPE_ENTITY = _ENTITYTYPE.nested_types_by_name['Entity']
@@ -42,23 +43,26 @@
 _UPDATEENTITYTYPEREQUEST = DESCRIPTOR.message_types_by_name['UpdateEntityTypeRequest']
 _DELETEENTITYTYPEREQUEST = DESCRIPTOR.message_types_by_name['DeleteEntityTypeRequest']
 _BATCHUPDATEENTITYTYPESREQUEST = DESCRIPTOR.message_types_by_name['BatchUpdateEntityTypesRequest']
 _BATCHUPDATEENTITYTYPESRESPONSE = DESCRIPTOR.message_types_by_name['BatchUpdateEntityTypesResponse']
 _BATCHDELETEENTITYTYPESREQUEST = DESCRIPTOR.message_types_by_name['BatchDeleteEntityTypesRequest']
 _ENTITYTYPEBATCH = DESCRIPTOR.message_types_by_name['EntityTypeBatch']
 _ENTITYTYPESORTING = DESCRIPTOR.message_types_by_name['EntityTypeSorting']
+_ENTITYSTATUS = DESCRIPTOR.message_types_by_name['EntityStatus']
 _BATCHENTITIESRESPONSE = DESCRIPTOR.message_types_by_name['BatchEntitiesResponse']
-_BATCHENTITIESRESPONSE_ENTITYSTATUS = _BATCHENTITIESRESPONSE.nested_types_by_name['EntityStatus']
+_CREATEENTITYREQUEST = DESCRIPTOR.message_types_by_name['CreateEntityRequest']
 _BATCHCREATEENTITIESREQUEST = DESCRIPTOR.message_types_by_name['BatchCreateEntitiesRequest']
-_BATCHCREATEENTITIESREQUEST_CREATEENTITYREQUEST = _BATCHCREATEENTITIESREQUEST.nested_types_by_name['CreateEntityRequest']
 _BATCHUPDATEENTITIESREQUEST = DESCRIPTOR.message_types_by_name['BatchUpdateEntitiesRequest']
+_UPDATEENTITYREQUEST = DESCRIPTOR.message_types_by_name['UpdateEntityRequest']
+_GETENTITYREQUEST = DESCRIPTOR.message_types_by_name['GetEntityRequest']
 _BATCHGETENTITIESREQUEST = DESCRIPTOR.message_types_by_name['BatchGetEntitiesRequest']
 _BATCHDELETEENTITIESREQUEST = DESCRIPTOR.message_types_by_name['BatchDeleteEntitiesRequest']
+_DELETEENTITYREQUEST = DESCRIPTOR.message_types_by_name['DeleteEntityRequest']
+_DELETEENTITYSTATUS = DESCRIPTOR.message_types_by_name['DeleteEntityStatus']
 _BATCHDELETEENTITIESRESPONSE = DESCRIPTOR.message_types_by_name['BatchDeleteEntitiesResponse']
-_BATCHDELETEENTITIESRESPONSE_DELETEENTITYSTATUS = _BATCHDELETEENTITIESRESPONSE.nested_types_by_name['DeleteEntityStatus']
 _LISTENTITIESREQUEST = DESCRIPTOR.message_types_by_name['ListEntitiesRequest']
 _LISTENTITIESRESPONSE = DESCRIPTOR.message_types_by_name['ListEntitiesResponse']
 _ENTITYVALUESORTING = DESCRIPTOR.message_types_by_name['EntityValueSorting']
 _ENTITYTYPE_KIND = _ENTITYTYPE.enum_types_by_name['Kind']
 _ENTITYTYPE_ENTITYTYPESTATUS = _ENTITYTYPE.enum_types_by_name['EntityTypeStatus']
 _ENTITYTYPE_AUTOEXPANSIONMODE = _ENTITYTYPE.enum_types_by_name['AutoExpansionMode']
 _ENTITYTYPESORTING_ENTITYTYPESORTINGFIELD = _ENTITYTYPESORTING.enum_types_by_name['EntityTypeSortingField']
@@ -150,76 +154,97 @@
 EntityTypeSorting = _reflection.GeneratedProtocolMessageType('EntityTypeSorting', (_message.Message,), {
     'DESCRIPTOR': _ENTITYTYPESORTING,
     '__module__': 'ondewo.nlu.entity_type_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.nlu.EntityTypeSorting)
 })
 _sym_db.RegisterMessage(EntityTypeSorting)
 
-BatchEntitiesResponse = _reflection.GeneratedProtocolMessageType('BatchEntitiesResponse', (_message.Message,), {
+EntityStatus = _reflection.GeneratedProtocolMessageType('EntityStatus', (_message.Message,), {
+    'DESCRIPTOR': _ENTITYSTATUS,
+    '__module__': 'ondewo.nlu.entity_type_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.nlu.EntityStatus)
+})
+_sym_db.RegisterMessage(EntityStatus)
 
-    'EntityStatus': _reflection.GeneratedProtocolMessageType('EntityStatus', (_message.Message,), {
-        'DESCRIPTOR': _BATCHENTITIESRESPONSE_ENTITYSTATUS,
-        '__module__': 'ondewo.nlu.entity_type_pb2'
-        # @@protoc_insertion_point(class_scope:ondewo.nlu.BatchEntitiesResponse.EntityStatus)
-    }),
+BatchEntitiesResponse = _reflection.GeneratedProtocolMessageType('BatchEntitiesResponse', (_message.Message,), {
     'DESCRIPTOR': _BATCHENTITIESRESPONSE,
     '__module__': 'ondewo.nlu.entity_type_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.nlu.BatchEntitiesResponse)
 })
 _sym_db.RegisterMessage(BatchEntitiesResponse)
-_sym_db.RegisterMessage(BatchEntitiesResponse.EntityStatus)
 
-BatchCreateEntitiesRequest = _reflection.GeneratedProtocolMessageType('BatchCreateEntitiesRequest', (_message.Message,), {
+CreateEntityRequest = _reflection.GeneratedProtocolMessageType('CreateEntityRequest', (_message.Message,), {
+    'DESCRIPTOR': _CREATEENTITYREQUEST,
+    '__module__': 'ondewo.nlu.entity_type_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.nlu.CreateEntityRequest)
+})
+_sym_db.RegisterMessage(CreateEntityRequest)
 
-    'CreateEntityRequest': _reflection.GeneratedProtocolMessageType('CreateEntityRequest', (_message.Message,), {
-        'DESCRIPTOR': _BATCHCREATEENTITIESREQUEST_CREATEENTITYREQUEST,
-        '__module__': 'ondewo.nlu.entity_type_pb2'
-        # @@protoc_insertion_point(class_scope:ondewo.nlu.BatchCreateEntitiesRequest.CreateEntityRequest)
-    }),
+BatchCreateEntitiesRequest = _reflection.GeneratedProtocolMessageType('BatchCreateEntitiesRequest', (_message.Message,), {
     'DESCRIPTOR': _BATCHCREATEENTITIESREQUEST,
     '__module__': 'ondewo.nlu.entity_type_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.nlu.BatchCreateEntitiesRequest)
 })
 _sym_db.RegisterMessage(BatchCreateEntitiesRequest)
-_sym_db.RegisterMessage(BatchCreateEntitiesRequest.CreateEntityRequest)
 
 BatchUpdateEntitiesRequest = _reflection.GeneratedProtocolMessageType('BatchUpdateEntitiesRequest', (_message.Message,), {
     'DESCRIPTOR': _BATCHUPDATEENTITIESREQUEST,
     '__module__': 'ondewo.nlu.entity_type_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.nlu.BatchUpdateEntitiesRequest)
 })
 _sym_db.RegisterMessage(BatchUpdateEntitiesRequest)
 
+UpdateEntityRequest = _reflection.GeneratedProtocolMessageType('UpdateEntityRequest', (_message.Message,), {
+    'DESCRIPTOR': _UPDATEENTITYREQUEST,
+    '__module__': 'ondewo.nlu.entity_type_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.nlu.UpdateEntityRequest)
+})
+_sym_db.RegisterMessage(UpdateEntityRequest)
+
+GetEntityRequest = _reflection.GeneratedProtocolMessageType('GetEntityRequest', (_message.Message,), {
+    'DESCRIPTOR': _GETENTITYREQUEST,
+    '__module__': 'ondewo.nlu.entity_type_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.nlu.GetEntityRequest)
+})
+_sym_db.RegisterMessage(GetEntityRequest)
+
 BatchGetEntitiesRequest = _reflection.GeneratedProtocolMessageType('BatchGetEntitiesRequest', (_message.Message,), {
     'DESCRIPTOR': _BATCHGETENTITIESREQUEST,
     '__module__': 'ondewo.nlu.entity_type_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.nlu.BatchGetEntitiesRequest)
 })
 _sym_db.RegisterMessage(BatchGetEntitiesRequest)
 
 BatchDeleteEntitiesRequest = _reflection.GeneratedProtocolMessageType('BatchDeleteEntitiesRequest', (_message.Message,), {
     'DESCRIPTOR': _BATCHDELETEENTITIESREQUEST,
     '__module__': 'ondewo.nlu.entity_type_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.nlu.BatchDeleteEntitiesRequest)
 })
 _sym_db.RegisterMessage(BatchDeleteEntitiesRequest)
 
-BatchDeleteEntitiesResponse = _reflection.GeneratedProtocolMessageType('BatchDeleteEntitiesResponse', (_message.Message,), {
+DeleteEntityRequest = _reflection.GeneratedProtocolMessageType('DeleteEntityRequest', (_message.Message,), {
+    'DESCRIPTOR': _DELETEENTITYREQUEST,
+    '__module__': 'ondewo.nlu.entity_type_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.nlu.DeleteEntityRequest)
+})
+_sym_db.RegisterMessage(DeleteEntityRequest)
 
-    'DeleteEntityStatus': _reflection.GeneratedProtocolMessageType('DeleteEntityStatus', (_message.Message,), {
-        'DESCRIPTOR': _BATCHDELETEENTITIESRESPONSE_DELETEENTITYSTATUS,
-        '__module__': 'ondewo.nlu.entity_type_pb2'
-        # @@protoc_insertion_point(class_scope:ondewo.nlu.BatchDeleteEntitiesResponse.DeleteEntityStatus)
-    }),
+DeleteEntityStatus = _reflection.GeneratedProtocolMessageType('DeleteEntityStatus', (_message.Message,), {
+    'DESCRIPTOR': _DELETEENTITYSTATUS,
+    '__module__': 'ondewo.nlu.entity_type_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.nlu.DeleteEntityStatus)
+})
+_sym_db.RegisterMessage(DeleteEntityStatus)
+
+BatchDeleteEntitiesResponse = _reflection.GeneratedProtocolMessageType('BatchDeleteEntitiesResponse', (_message.Message,), {
     'DESCRIPTOR': _BATCHDELETEENTITIESRESPONSE,
     '__module__': 'ondewo.nlu.entity_type_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.nlu.BatchDeleteEntitiesResponse)
 })
 _sym_db.RegisterMessage(BatchDeleteEntitiesResponse)
-_sym_db.RegisterMessage(BatchDeleteEntitiesResponse.DeleteEntityStatus)
 
 ListEntitiesRequest = _reflection.GeneratedProtocolMessageType('ListEntitiesRequest', (_message.Message,), {
     'DESCRIPTOR': _LISTENTITIESREQUEST,
     '__module__': 'ondewo.nlu.entity_type_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.nlu.ListEntitiesRequest)
 })
 _sym_db.RegisterMessage(ListEntitiesRequest)
@@ -253,18 +278,26 @@
     _ENTITYTYPES.methods_by_name['UpdateEntityType']._serialized_options = b'\202\323\344\223\002:25/v2/{entity_type.name=projects/*/agent/entityTypes/*}:\001*'
     _ENTITYTYPES.methods_by_name['DeleteEntityType']._options = None
     _ENTITYTYPES.methods_by_name['DeleteEntityType']._serialized_options = b'\202\323\344\223\002+*)/v2/{name=projects/*/agent/entityTypes/*}'
     _ENTITYTYPES.methods_by_name['BatchUpdateEntityTypes']._options = None
     _ENTITYTYPES.methods_by_name['BatchUpdateEntityTypes']._serialized_options = b'\202\323\344\223\002:\"5/v2/{parent=projects/*/agent}/entityTypes:batchUpdate:\001*'
     _ENTITYTYPES.methods_by_name['BatchDeleteEntityTypes']._options = None
     _ENTITYTYPES.methods_by_name['BatchDeleteEntityTypes']._serialized_options = b'\202\323\344\223\002:\"5/v2/{parent=projects/*/agent}/entityTypes:batchDelete:\001*'
-    _ENTITYTYPEVIEW._serialized_start = 4062
-    _ENTITYTYPEVIEW._serialized_end = 4199
-    _ENTITYTYPECATEGORY._serialized_start = 4201
-    _ENTITYTYPECATEGORY._serialized_end = 4300
+    _ENTITYTYPES.methods_by_name['GetEntity']._options = None
+    _ENTITYTYPES.methods_by_name['GetEntity']._serialized_options = b'\202\323\344\223\0026\0224/v2/{name=projects/*/agent/entityTypes/*/entities/*}'
+    _ENTITYTYPES.methods_by_name['CreateEntity']._options = None
+    _ENTITYTYPES.methods_by_name['CreateEntity']._serialized_options = b'\202\323\344\223\002:\"5/v2/{parent=projects/*/agent}/entityTypes/*/entities/:\001*'
+    _ENTITYTYPES.methods_by_name['UpdateEntity']._options = None
+    _ENTITYTYPES.methods_by_name['UpdateEntity']._serialized_options = b'\202\323\344\223\002A2</v2/{entity_.name=projects/*/agent/entityTypes/*/entities/*}:\001*'
+    _ENTITYTYPES.methods_by_name['DeleteEntity']._options = None
+    _ENTITYTYPES.methods_by_name['DeleteEntity']._serialized_options = b'\202\323\344\223\0026*4/v2/{name=projects/*/agent/entityTypes/*/entities/*}'
+    _ENTITYTYPEVIEW._serialized_start = 4123
+    _ENTITYTYPEVIEW._serialized_end = 4290
+    _ENTITYTYPECATEGORY._serialized_start = 4292
+    _ENTITYTYPECATEGORY._serialized_end = 4391
     _ENTITYTYPE._serialized_start = 192
     _ENTITYTYPE._serialized_end = 851
     _ENTITYTYPE_ENTITY._serialized_start = 532
     _ENTITYTYPE_ENTITY._serialized_end = 655
     _ENTITYTYPE_KIND._serialized_start = 657
     _ENTITYTYPE_KIND._serialized_end = 714
     _ENTITYTYPE_ENTITYTYPESTATUS._serialized_start = 716
@@ -291,36 +324,42 @@
     _BATCHDELETEENTITYTYPESREQUEST._serialized_end = 2142
     _ENTITYTYPEBATCH._serialized_start = 2144
     _ENTITYTYPEBATCH._serialized_end = 2207
     _ENTITYTYPESORTING._serialized_start = 2210
     _ENTITYTYPESORTING._serialized_end = 2598
     _ENTITYTYPESORTING_ENTITYTYPESORTINGFIELD._serialized_start = 2356
     _ENTITYTYPESORTING_ENTITYTYPESORTINGFIELD._serialized_end = 2598
-    _BATCHENTITIESRESPONSE._serialized_start = 2601
-    _BATCHENTITIESRESPONSE._serialized_end = 2827
-    _BATCHENTITIESRESPONSE_ENTITYSTATUS._serialized_start = 2719
-    _BATCHENTITIESRESPONSE_ENTITYSTATUS._serialized_end = 2827
-    _BATCHCREATEENTITIESREQUEST._serialized_start = 2830
-    _BATCHCREATEENTITIESREQUEST._serialized_end = 3046
-    _BATCHCREATEENTITIESREQUEST_CREATEENTITYREQUEST._serialized_start = 2952
-    _BATCHCREATEENTITIESREQUEST_CREATEENTITYREQUEST._serialized_end = 3046
-    _BATCHUPDATEENTITIESREQUEST._serialized_start = 3048
-    _BATCHUPDATEENTITIESREQUEST._serialized_end = 3125
-    _BATCHGETENTITIESREQUEST._serialized_start = 3127
-    _BATCHGETENTITIESREQUEST._serialized_end = 3167
-    _BATCHDELETEENTITIESREQUEST._serialized_start = 3169
-    _BATCHDELETEENTITIESREQUEST._serialized_end = 3212
-    _BATCHDELETEENTITIESRESPONSE._serialized_start = 3215
-    _BATCHDELETEENTITIESRESPONSE._serialized_end = 3469
-    _BATCHDELETEENTITIESRESPONSE_DELETEENTITYSTATUS._serialized_start = 3351
-    _BATCHDELETEENTITIESRESPONSE_DELETEENTITYSTATUS._serialized_end = 3469
-    _LISTENTITIESREQUEST._serialized_start = 3472
-    _LISTENTITIESREQUEST._serialized_end = 3644
-    _LISTENTITIESRESPONSE._serialized_start = 3646
-    _LISTENTITIESRESPONSE._serialized_end = 3742
-    _ENTITYVALUESORTING._serialized_start = 3745
-    _ENTITYVALUESORTING._serialized_end = 4059
-    _ENTITYVALUESORTING_ENTITYVALUESORTINGFIELD._serialized_start = 3894
-    _ENTITYVALUESORTING_ENTITYVALUESORTINGFIELD._serialized_end = 4059
-    _ENTITYTYPES._serialized_start = 4303
-    _ENTITYTYPES._serialized_end = 5796
+    _ENTITYSTATUS._serialized_start = 2600
+    _ENTITYSTATUS._serialized_end = 2708
+    _BATCHENTITIESRESPONSE._serialized_start = 2710
+    _BATCHENTITIESRESPONSE._serialized_end = 2804
+    _CREATEENTITYREQUEST._serialized_start = 2806
+    _CREATEENTITYREQUEST._serialized_end = 2900
+    _BATCHCREATEENTITIESREQUEST._serialized_start = 2902
+    _BATCHCREATEENTITIESREQUEST._serialized_end = 2995
+    _BATCHUPDATEENTITIESREQUEST._serialized_start = 2997
+    _BATCHUPDATEENTITIESREQUEST._serialized_end = 3074
+    _UPDATEENTITYREQUEST._serialized_start = 3076
+    _UPDATEENTITYREQUEST._serialized_end = 3144
+    _GETENTITYREQUEST._serialized_start = 3146
+    _GETENTITYREQUEST._serialized_end = 3178
+    _BATCHGETENTITIESREQUEST._serialized_start = 3180
+    _BATCHGETENTITIESREQUEST._serialized_end = 3220
+    _BATCHDELETEENTITIESREQUEST._serialized_start = 3222
+    _BATCHDELETEENTITIESREQUEST._serialized_end = 3265
+    _DELETEENTITYREQUEST._serialized_start = 3267
+    _DELETEENTITYREQUEST._serialized_end = 3302
+    _DELETEENTITYSTATUS._serialized_start = 3304
+    _DELETEENTITYSTATUS._serialized_end = 3422
+    _BATCHDELETEENTITIESRESPONSE._serialized_start = 3424
+    _BATCHDELETEENTITIESRESPONSE._serialized_end = 3530
+    _LISTENTITIESREQUEST._serialized_start = 3533
+    _LISTENTITIESREQUEST._serialized_end = 3705
+    _LISTENTITIESRESPONSE._serialized_start = 3707
+    _LISTENTITIESRESPONSE._serialized_end = 3803
+    _ENTITYVALUESORTING._serialized_start = 3806
+    _ENTITYVALUESORTING._serialized_end = 4120
+    _ENTITYVALUESORTING_ENTITYVALUESORTINGFIELD._serialized_start = 3955
+    _ENTITYVALUESORTING_ENTITYVALUESORTINGFIELD._serialized_end = 4120
+    _ENTITYTYPES._serialized_start = 4394
+    _ENTITYTYPES._serialized_end = 6469
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/entity_type_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/entity_type_pb2_grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,14 +74,34 @@
             response_deserializer=ondewo_dot_nlu_dot_operations__pb2.Operation.FromString,
         )
         self.BatchDeleteEntityTypes = channel.unary_unary(
             '/ondewo.nlu.EntityTypes/BatchDeleteEntityTypes',
             request_serializer=ondewo_dot_nlu_dot_entity__type__pb2.BatchDeleteEntityTypesRequest.SerializeToString,
             response_deserializer=ondewo_dot_nlu_dot_operations__pb2.Operation.FromString,
         )
+        self.GetEntity = channel.unary_unary(
+            '/ondewo.nlu.EntityTypes/GetEntity',
+            request_serializer=ondewo_dot_nlu_dot_entity__type__pb2.GetEntityRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_entity__type__pb2.EntityType.Entity.FromString,
+        )
+        self.CreateEntity = channel.unary_unary(
+            '/ondewo.nlu.EntityTypes/CreateEntity',
+            request_serializer=ondewo_dot_nlu_dot_entity__type__pb2.CreateEntityRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_entity__type__pb2.EntityType.Entity.FromString,
+        )
+        self.UpdateEntity = channel.unary_unary(
+            '/ondewo.nlu.EntityTypes/UpdateEntity',
+            request_serializer=ondewo_dot_nlu_dot_entity__type__pb2.UpdateEntityRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_entity__type__pb2.EntityType.Entity.FromString,
+        )
+        self.DeleteEntity = channel.unary_unary(
+            '/ondewo.nlu.EntityTypes/DeleteEntity',
+            request_serializer=ondewo_dot_nlu_dot_entity__type__pb2.DeleteEntityRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_entity__type__pb2.DeleteEntityStatus.FromString,
+        )
         self.BatchCreateEntities = channel.unary_unary(
             '/ondewo.nlu.EntityTypes/BatchCreateEntities',
             request_serializer=ondewo_dot_nlu_dot_entity__type__pb2.BatchCreateEntitiesRequest.SerializeToString,
             response_deserializer=ondewo_dot_nlu_dot_entity__type__pb2.BatchEntitiesResponse.FromString,
         )
         self.BatchUpdateEntities = channel.unary_unary(
             '/ondewo.nlu.EntityTypes/BatchUpdateEntities',
@@ -186,14 +206,42 @@
         Operation <response: [google.protobuf.Empty][google.protobuf.Empty],
         metadata: [google.protobuf.Struct][google.protobuf.Struct]>
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetEntity(self, request, context):
+        """Retrieves the specified entity .
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def CreateEntity(self, request, context):
+        """Creates an entity  in the specified agent.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def UpdateEntity(self, request, context):
+        """Updates the specified entity .
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DeleteEntity(self, request, context):
+        """Deletes the specified entity .
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def BatchCreateEntities(self, request, context):
         """Creates an entity value in an entity type.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -259,14 +307,34 @@
             response_serializer=ondewo_dot_nlu_dot_operations__pb2.Operation.SerializeToString,
         ),
         'BatchDeleteEntityTypes': grpc.unary_unary_rpc_method_handler(
             servicer.BatchDeleteEntityTypes,
             request_deserializer=ondewo_dot_nlu_dot_entity__type__pb2.BatchDeleteEntityTypesRequest.FromString,
             response_serializer=ondewo_dot_nlu_dot_operations__pb2.Operation.SerializeToString,
         ),
+        'GetEntity': grpc.unary_unary_rpc_method_handler(
+            servicer.GetEntity,
+            request_deserializer=ondewo_dot_nlu_dot_entity__type__pb2.GetEntityRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_entity__type__pb2.EntityType.Entity.SerializeToString,
+        ),
+        'CreateEntity': grpc.unary_unary_rpc_method_handler(
+            servicer.CreateEntity,
+            request_deserializer=ondewo_dot_nlu_dot_entity__type__pb2.CreateEntityRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_entity__type__pb2.EntityType.Entity.SerializeToString,
+        ),
+        'UpdateEntity': grpc.unary_unary_rpc_method_handler(
+            servicer.UpdateEntity,
+            request_deserializer=ondewo_dot_nlu_dot_entity__type__pb2.UpdateEntityRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_entity__type__pb2.EntityType.Entity.SerializeToString,
+        ),
+        'DeleteEntity': grpc.unary_unary_rpc_method_handler(
+            servicer.DeleteEntity,
+            request_deserializer=ondewo_dot_nlu_dot_entity__type__pb2.DeleteEntityRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_entity__type__pb2.DeleteEntityStatus.SerializeToString,
+        ),
         'BatchCreateEntities': grpc.unary_unary_rpc_method_handler(
             servicer.BatchCreateEntities,
             request_deserializer=ondewo_dot_nlu_dot_entity__type__pb2.BatchCreateEntitiesRequest.FromString,
             response_serializer=ondewo_dot_nlu_dot_entity__type__pb2.BatchEntitiesResponse.SerializeToString,
         ),
         'BatchUpdateEntities': grpc.unary_unary_rpc_method_handler(
             servicer.BatchUpdateEntities,
@@ -442,14 +510,82 @@
         return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.EntityTypes/BatchDeleteEntityTypes',
                                              ondewo_dot_nlu_dot_entity__type__pb2.BatchDeleteEntityTypesRequest.SerializeToString,
                                              ondewo_dot_nlu_dot_operations__pb2.Operation.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetEntity(request,
+                  target,
+                  options=(),
+                  channel_credentials=None,
+                  call_credentials=None,
+                  insecure=False,
+                  compression=None,
+                  wait_for_ready=None,
+                  timeout=None,
+                  metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.EntityTypes/GetEntity',
+                                             ondewo_dot_nlu_dot_entity__type__pb2.GetEntityRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_entity__type__pb2.EntityType.Entity.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CreateEntity(request,
+                     target,
+                     options=(),
+                     channel_credentials=None,
+                     call_credentials=None,
+                     insecure=False,
+                     compression=None,
+                     wait_for_ready=None,
+                     timeout=None,
+                     metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.EntityTypes/CreateEntity',
+                                             ondewo_dot_nlu_dot_entity__type__pb2.CreateEntityRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_entity__type__pb2.EntityType.Entity.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UpdateEntity(request,
+                     target,
+                     options=(),
+                     channel_credentials=None,
+                     call_credentials=None,
+                     insecure=False,
+                     compression=None,
+                     wait_for_ready=None,
+                     timeout=None,
+                     metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.EntityTypes/UpdateEntity',
+                                             ondewo_dot_nlu_dot_entity__type__pb2.UpdateEntityRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_entity__type__pb2.EntityType.Entity.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteEntity(request,
+                     target,
+                     options=(),
+                     channel_credentials=None,
+                     call_credentials=None,
+                     insecure=False,
+                     compression=None,
+                     wait_for_ready=None,
+                     timeout=None,
+                     metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.EntityTypes/DeleteEntity',
+                                             ondewo_dot_nlu_dot_entity__type__pb2.DeleteEntityRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_entity__type__pb2.DeleteEntityStatus.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def BatchCreateEntities(request,
                             target,
                             options=(),
                             channel_credentials=None,
                             call_credentials=None,
                             insecure=False,
                             compression=None,
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/intent_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/intent_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17ondewo/nlu/intent.proto\x12\nondewo.nlu\x1a\x1cgoogle/api/annotations.proto\x1a\x18ondewo/nlu/context.proto\x1a\x17ondewo/nlu/common.proto\x1a\x1bondewo/nlu/operations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a google/protobuf/field_mask.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xcf\'\n\x06Intent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x36\n\rwebhook_state\x18\x06 \x01(\x0e\x32\x1f.ondewo.nlu.Intent.WebhookState\x12\x10\n\x08priority\x18\x03 \x01(\x05\x12\x13\n\x0bis_fallback\x18\x04 \x01(\x08\x12\x13\n\x0bml_disabled\x18\x13 \x01(\x08\x12\x1b\n\x13input_context_names\x18\x07 \x03(\t\x12\x0e\n\x06\x65vents\x18\x08 \x03(\t\x12;\n\x10training_phrases\x18\t \x03(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\x12\x0e\n\x06\x61\x63tion\x18\n \x01(\t\x12,\n\x0foutput_contexts\x18\x0b \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x16\n\x0ereset_contexts\x18\x0c \x01(\x08\x12\x30\n\nparameters\x18\r \x03(\x0b\x32\x1c.ondewo.nlu.Intent.Parameter\x12,\n\x08messages\x18\x0e \x03(\x0b\x32\x1a.ondewo.nlu.Intent.Message\x12G\n\x1a\x64\x65\x66\x61ult_response_platforms\x18\x0f \x03(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\x12!\n\x19root_followup_intent_name\x18\x10 \x01(\t\x12#\n\x1bparent_followup_intent_name\x18\x11 \x01(\t\x12\x43\n\x14\x66ollowup_intent_info\x18\x12 \x03(\x0b\x32%.ondewo.nlu.Intent.FollowupIntentInfo\x12\x17\n\x0fnext_page_token\x18\x1e \x01(\t\x12\x13\n\x0b\x64omain_name\x18\x1f \x01(\t\x12\x1d\n\x15is_start_of_deviation\x18  \x01(\x08\x12\x1b\n\x13is_end_of_deviation\x18! \x01(\x08\x12\x1d\n\x15training_phrase_count\x18\" \x01(\x05\x12/\n\x06status\x18# \x01(\x0e\x32\x1f.ondewo.nlu.Intent.IntentStatus\x12.\n\nstart_date\x18$ \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_date\x18% \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04tags\x18& \x03(\t\x1a\xe2\x03\n\x0eTrainingPhrase\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x34\n\x04type\x18\x02 \x01(\x0e\x32&.ondewo.nlu.Intent.TrainingPhrase.Type\x12\x0c\n\x04text\x18\x03 \x01(\t\x12:\n\x08\x65ntities\x18\x04 \x03(\x0b\x32(.ondewo.nlu.Intent.TrainingPhrase.Entity\x12\x19\n\x11times_added_count\x18\x05 \x01(\x05\x12\x15\n\rlanguage_code\x18\x06 \x01(\t\x1a\xd6\x01\n\x06\x45ntity\x12\x18\n\x10\x65ntity_type_name\x18\x01 \x01(\t\x12 \n\x18\x65ntity_type_display_name\x18\x03 \x01(\t\x12\x19\n\x11\x65ntity_value_name\x18\x04 \x01(\t\x12!\n\x19\x65ntity_value_display_name\x18\x05 \x01(\t\x12\r\n\x05start\x18\x06 \x01(\x05\x12\x0b\n\x03\x65nd\x18\x07 \x01(\x05\x12\x16\n\x0eparameter_name\x18\x08 \x01(\t\x12\x1e\n\x16parameter_display_name\x18\t \x01(\t\"7\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0b\n\x07\x45XAMPLE\x10\x01\x12\x0c\n\x08TEMPLATE\x10\x02\x1a\xa8\x02\n\tParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x15\n\rdefault_value\x18\x04 \x01(\t\x12\x18\n\x10\x65ntity_type_name\x18\x05 \x01(\t\x12 \n\x18\x65ntity_type_display_name\x18\x06 \x01(\t\x12\x11\n\tmandatory\x18\x07 \x01(\x08\x12\x34\n\x07prompts\x18\x08 \x03(\x0b\x32#.ondewo.nlu.Intent.Parameter.Prompt\x12\x0f\n\x07is_list\x18\t \x01(\x08\x1a;\n\x06Prompt\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x1a\x87\x18\n\x07Message\x12\x0c\n\x04name\x18\x10 \x01(\t\x12\x15\n\rlanguage_code\x18\x11 \x01(\t\x12/\n\x04text\x18\x01 \x01(\x0b\x32\x1f.ondewo.nlu.Intent.Message.TextH\x00\x12\x31\n\x05image\x18\x02 \x01(\x0b\x32 .ondewo.nlu.Intent.Message.ImageH\x00\x12@\n\rquick_replies\x18\x03 \x01(\x0b\x32\'.ondewo.nlu.Intent.Message.QuickRepliesH\x00\x12/\n\x04\x63\x61rd\x18\x04 \x01(\x0b\x32\x1f.ondewo.nlu.Intent.Message.CardH\x00\x12*\n\x07payload\x18\x05 \x01(\x0b\x32\x17.google.protobuf.StructH\x00\x12\x46\n\x10simple_responses\x18\x07 \x01(\x0b\x32*.ondewo.nlu.Intent.Message.SimpleResponsesH\x00\x12:\n\nbasic_card\x18\x08 \x01(\x0b\x32$.ondewo.nlu.Intent.Message.BasicCardH\x00\x12=\n\x0bsuggestions\x18\t \x01(\x0b\x32&.ondewo.nlu.Intent.Message.SuggestionsH\x00\x12K\n\x13link_out_suggestion\x18\n \x01(\x0b\x32,.ondewo.nlu.Intent.Message.LinkOutSuggestionH\x00\x12<\n\x0blist_select\x18\x0b \x01(\x0b\x32%.ondewo.nlu.Intent.Message.ListSelectH\x00\x12\x44\n\x0f\x63\x61rousel_select\x18\x0c \x01(\x0b\x32).ondewo.nlu.Intent.Message.CarouselSelectH\x00\x12\x38\n\thtml_text\x18\r \x01(\x0b\x32#.ondewo.nlu.Intent.Message.HTMLTextH\x00\x12\x31\n\x05video\x18\x0e \x01(\x0b\x32 .ondewo.nlu.Intent.Message.VideoH\x00\x12\x31\n\x05\x61udio\x18\x0f \x01(\x0b\x32 .ondewo.nlu.Intent.Message.AudioH\x00\x12\x35\n\x08platform\x18\x06 \x01(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\x12\x11\n\tis_prompt\x18\x12 \x01(\x08\x1a\x14\n\x04Text\x12\x0c\n\x04text\x18\x01 \x03(\t\x1a\x36\n\x05Image\x12\x11\n\timage_uri\x18\x01 \x01(\t\x12\x1a\n\x12\x61\x63\x63\x65ssibility_text\x18\x02 \x01(\t\x1a\x34\n\x0cQuickReplies\x12\r\n\x05title\x18\x01 \x01(\t\x12\x15\n\rquick_replies\x18\x02 \x03(\t\x1a\x9d\x01\n\x04\x43\x61rd\x12\r\n\x05title\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x11\n\timage_uri\x18\x03 \x01(\t\x12\x37\n\x07\x62uttons\x18\x04 \x03(\x0b\x32&.ondewo.nlu.Intent.Message.Card.Button\x1a(\n\x06\x42utton\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x10\n\x08postback\x18\x02 \x01(\t\x1aL\n\x0eSimpleResponse\x12\x16\n\x0etext_to_speech\x18\x01 \x01(\t\x12\x0c\n\x04ssml\x18\x02 \x01(\t\x12\x14\n\x0c\x64isplay_text\x18\x03 \x01(\t\x1aV\n\x0fSimpleResponses\x12\x43\n\x10simple_responses\x18\x01 \x03(\x0b\x32).ondewo.nlu.Intent.Message.SimpleResponse\x1a\xbf\x02\n\tBasicCard\x12\r\n\x05title\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x16\n\x0e\x66ormatted_text\x18\x03 \x01(\t\x12/\n\x05image\x18\x04 \x01(\x0b\x32 .ondewo.nlu.Intent.Message.Image\x12<\n\x07\x62uttons\x18\x05 \x03(\x0b\x32+.ondewo.nlu.Intent.Message.BasicCard.Button\x1a\x89\x01\n\x06\x42utton\x12\r\n\x05title\x18\x01 \x01(\t\x12R\n\x0fopen_uri_action\x18\x02 \x01(\x0b\x32\x39.ondewo.nlu.Intent.Message.BasicCard.Button.OpenUriAction\x1a\x1c\n\rOpenUriAction\x12\x0b\n\x03uri\x18\x01 \x01(\t\x1a\x1b\n\nSuggestion\x12\r\n\x05title\x18\x01 \x01(\t\x1aI\n\x0bSuggestions\x12:\n\x0bsuggestions\x18\x01 \x03(\x0b\x32%.ondewo.nlu.Intent.Message.Suggestion\x1a:\n\x11LinkOutSuggestion\x12\x18\n\x10\x64\x65stination_name\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x1a\xed\x01\n\nListSelect\x12\r\n\x05title\x18\x01 \x01(\t\x12\x39\n\x05items\x18\x02 \x03(\x0b\x32*.ondewo.nlu.Intent.Message.ListSelect.Item\x1a\x94\x01\n\x04Item\x12\x37\n\x04info\x18\x01 \x01(\x0b\x32).ondewo.nlu.Intent.Message.SelectItemInfo\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12/\n\x05image\x18\x04 \x01(\x0b\x32 .ondewo.nlu.Intent.Message.Image\x1a\xe6\x01\n\x0e\x43\x61rouselSelect\x12=\n\x05items\x18\x01 \x03(\x0b\x32..ondewo.nlu.Intent.Message.CarouselSelect.Item\x1a\x94\x01\n\x04Item\x12\x37\n\x04info\x18\x01 \x01(\x0b\x32).ondewo.nlu.Intent.Message.SelectItemInfo\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12/\n\x05image\x18\x04 \x01(\x0b\x32 .ondewo.nlu.Intent.Message.Image\x1a\x18\n\x08HTMLText\x12\x0c\n\x04text\x18\x01 \x03(\t\x1a\x30\n\x05Video\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x1a\n\x12\x61\x63\x63\x65ssibility_text\x18\x02 \x01(\t\x1a\x30\n\x05\x41udio\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x1a\n\x12\x61\x63\x63\x65ssibility_text\x18\x02 \x01(\t\x1a/\n\x0eSelectItemInfo\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x10\n\x08synonyms\x18\x02 \x03(\t\"\x92\x04\n\x08Platform\x12\x18\n\x14PLATFORM_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x46\x41\x43\x45\x42OOK\x10\x01\x12\t\n\x05SLACK\x10\x02\x12\x0c\n\x08TELEGRAM\x10\x03\x12\x07\n\x03KIK\x10\x04\x12\t\n\x05SKYPE\x10\x05\x12\x08\n\x04LINE\x10\x06\x12\t\n\x05VIBER\x10\x07\x12\x15\n\x11\x41\x43TIONS_ON_GOOGLE\x10\x08\x12\x11\n\rPLACEHOLDER_1\x10\t\x12\x11\n\rPLACEHOLDER_2\x10\n\x12\x11\n\rPLACEHOLDER_3\x10\x0b\x12\x11\n\rPLACEHOLDER_4\x10\x0c\x12\x11\n\rPLACEHOLDER_5\x10\r\x12\x11\n\rPLACEHOLDER_6\x10\x0e\x12\x11\n\rPLACEHOLDER_7\x10\x0f\x12\x11\n\rPLACEHOLDER_8\x10\x10\x12\x11\n\rPLACEHOLDER_9\x10\x11\x12\x12\n\x0ePLACEHOLDER_10\x10\x12\x12\x12\n\x0ePLACEHOLDER_11\x10\x13\x12\x12\n\x0ePLACEHOLDER_12\x10\x14\x12\x12\n\x0ePLACEHOLDER_13\x10\x15\x12\x12\n\x0ePLACEHOLDER_14\x10\x16\x12\x12\n\x0ePLACEHOLDER_15\x10\x17\x12\x12\n\x0ePLACEHOLDER_16\x10\x18\x12\x12\n\x0ePLACEHOLDER_17\x10\x19\x12\x12\n\x0ePLACEHOLDER_18\x10\x1a\x12\x12\n\x0ePLACEHOLDER_19\x10\x1b\x12\x12\n\x0ePLACEHOLDER_20\x10\x1c\x42\t\n\x07message\x1aW\n\x12\x46ollowupIntentInfo\x12\x1c\n\x14\x66ollowup_intent_name\x18\x01 \x01(\t\x12#\n\x1bparent_followup_intent_name\x18\x02 \x01(\t\"(\n\x0cIntentStatus\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08INACTIVE\x10\x01\"t\n\x0cWebhookState\x12\x1d\n\x19WEBHOOK_STATE_UNSPECIFIED\x10\x00\x12\x19\n\x15WEBHOOK_STATE_ENABLED\x10\x01\x12*\n&WEBHOOK_STATE_ENABLED_FOR_SLOT_FILLING\x10\x02\"\xfe\x01\n\x12ListIntentsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12+\n\x0bintent_view\x18\x03 \x01(\x0e\x32\x16.ondewo.nlu.IntentView\x12\x12\n\npage_token\x18\x05 \x01(\t\x12\x36\n\x12\x66ilter_by_category\x18\x06 \x01(\x0e\x32\x1a.ondewo.nlu.IntentCategory\x12\x30\n\rsort_by_field\x18\x07 \x01(\x0b\x32\x19.ondewo.nlu.IntentSorting\x12\x16\n\x0e\x66ilter_by_tags\x18\x08 \x03(\t\"S\n\x13ListIntentsResponse\x12#\n\x07intents\x18\x01 \x03(\x0b\x32\x12.ondewo.nlu.Intent\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"x\n\x10GetIntentRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12+\n\x0bintent_view\x18\x03 \x01(\x0e\x32\x16.ondewo.nlu.IntentView\x12\x12\n\npage_token\x18\n \x01(\t\"\x8d\x01\n\x13\x43reateIntentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\"\n\x06intent\x18\x02 \x01(\x0b\x32\x12.ondewo.nlu.Intent\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12+\n\x0bintent_view\x18\x04 \x01(\x0e\x32\x16.ondewo.nlu.IntentView\"\xae\x01\n\x13UpdateIntentRequest\x12\"\n\x06intent\x18\x01 \x01(\x0b\x32\x12.ondewo.nlu.Intent\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12/\n\x0bupdate_mask\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12+\n\x0bintent_view\x18\x04 \x01(\x0e\x32\x16.ondewo.nlu.IntentView\"#\n\x13\x44\x65leteIntentRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x84\x02\n\x19\x42\x61tchUpdateIntentsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x1a\n\x10intent_batch_uri\x18\x02 \x01(\tH\x00\x12\x36\n\x13intent_batch_inline\x18\x03 \x01(\x0b\x32\x17.ondewo.nlu.IntentBatchH\x00\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12/\n\x0bupdate_mask\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12+\n\x0bintent_view\x18\x06 \x01(\x0e\x32\x16.ondewo.nlu.IntentViewB\x0e\n\x0cintent_batch\"A\n\x1a\x42\x61tchUpdateIntentsResponse\x12#\n\x07intents\x18\x01 \x03(\x0b\x32\x12.ondewo.nlu.Intent\"P\n\x19\x42\x61tchDeleteIntentsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12#\n\x07intents\x18\x02 \x03(\x0b\x32\x12.ondewo.nlu.Intent\"2\n\x0bIntentBatch\x12#\n\x07intents\x18\x01 \x03(\x0b\x32\x12.ondewo.nlu.Intent\"\xec\x02\n\rIntentSorting\x12\x43\n\rsorting_field\x18\x01 \x01(\x0e\x32,.ondewo.nlu.IntentSorting.IntentSortingField\x12-\n\x0csorting_mode\x18\x02 \x01(\x0e\x32\x17.ondewo.nlu.SortingMode\"\xe6\x01\n\x12IntentSortingField\x12\x15\n\x11NO_INTENT_SORTING\x10\x00\x12\x17\n\x13SORT_INTENT_BY_NAME\x10\x01\x12 \n\x1cSORT_INTENT_BY_CREATION_DATE\x10\x02\x12\x1f\n\x1bSORT_INTENT_BY_LAST_UPDATED\x10\x03\x12!\n\x1dSORT_INTENT_BY_USERSAYS_COUNT\x10\x04\x12\x1d\n\x19SORT_INTENT_BY_START_DATE\x10\x05\x12\x1b\n\x17SORT_INTENT_BY_END_DATE\x10\x06\"5\n\x10IntentTagRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12\x0c\n\x04tags\x18\x02 \x03(\t\"+\n\x14GetIntentTagsRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\",\n\x15GetIntentTagsResponse\x12\x13\n\x0bintent_tags\x18\x01 \x03(\t\")\n\x17GetAllIntentTagsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\"`\n!BatchUpdateTrainingPhrasesRequest\x12;\n\x10training_phrases\x18\x01 \x03(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\"\x81\x01\n\x14TrainingPhraseStatus\x12<\n\x0ftraining_phrase\x18\x01 \x01(\x0b\x32!.ondewo.nlu.Intent.TrainingPhraseH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x12\n\x10phrase_or_status\"|\n\"BatchTrainingPhrasesStatusResponse\x12\x42\n\x18training_phrase_statuses\x18\x01 \x03(\x0b\x32 .ondewo.nlu.TrainingPhraseStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\"\x80\x02\n!BatchCreateTrainingPhrasesRequest\x12k\n\x18training_phrase_requests\x18\x01 \x03(\x0b\x32I.ondewo.nlu.BatchCreateTrainingPhrasesRequest.CreateTrainingPhraseRequest\x1an\n\x1b\x43reateTrainingPhraseRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12:\n\x0ftraining_phrase\x18\x02 \x01(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\"/\n\x1e\x42\x61tchGetTrainingPhrasesRequest\x12\r\n\x05names\x18\x01 \x03(\t\"2\n!BatchDeleteTrainingPhrasesRequest\x12\r\n\x05names\x18\x01 \x03(\t\"\x9c\x02\n\"BatchDeleteTrainingPhrasesResponse\x12\x62\n\x0f\x64\x65lete_statuses\x18\x01 \x03(\x0b\x32I.ondewo.nlu.BatchDeleteTrainingPhrasesResponse.DeleteTrainingPhraseStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\x1a~\n\x1a\x44\x65leteTrainingPhraseStatus\x12\x36\n\x14successfully_deleted\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x0f\n\rdelete_status\"\\\n\x1aListTrainingPhrasesRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\npage_token\x18\x03 \x01(\t\"s\n\x1bListTrainingPhrasesResponse\x12;\n\x10training_phrases\x18\x01 \x03(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xa1\x02\n#BatchResponseMessagesStatusResponse\x12h\n\x19response_message_statuses\x18\x01 \x03(\x0b\x32\x45.ondewo.nlu.BatchResponseMessagesStatusResponse.ResponseMessageStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\x1a|\n\x15ResponseMessageStatus\x12\x36\n\x10response_message\x18\x01 \x01(\x0b\x32\x1a.ondewo.nlu.Intent.MessageH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x12\n\x10phrase_or_status\"\xff\x01\n\"BatchCreateResponseMessagesRequest\x12n\n\x19response_message_requests\x18\x01 \x03(\x0b\x32K.ondewo.nlu.BatchCreateResponseMessagesRequest.CreateResponseMessageRequest\x1ai\n\x1c\x43reateResponseMessageRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12\x34\n\x10response_message\x18\x02 \x01(\x0b\x32\x1a.ondewo.nlu.Intent.Message\"[\n\"BatchUpdateResponseMessagesRequest\x12\x35\n\x11response_messages\x18\x01 \x03(\x0b\x32\x1a.ondewo.nlu.Intent.Message\"0\n\x1f\x42\x61tchGetResponseMessagesRequest\x12\r\n\x05names\x18\x01 \x03(\t\"3\n\"BatchDeleteResponseMessagesRequest\x12\r\n\x05names\x18\x01 \x03(\t\"\xa0\x02\n#BatchDeleteResponseMessagesResponse\x12\x64\n\x0f\x64\x65lete_statuses\x18\x01 \x03(\x0b\x32K.ondewo.nlu.BatchDeleteResponseMessagesResponse.DeleteResponseMessageStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\x1a\x7f\n\x1b\x44\x65leteResponseMessageStatus\x12\x36\n\x14successfully_deleted\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x0f\n\rdelete_status\"]\n\x1bListResponseMessagesRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\npage_token\x18\x03 \x01(\t\"n\n\x1cListResponseMessagesResponse\x12\x35\n\x11response_messages\x18\x01 \x03(\x0b\x32\x1a.ondewo.nlu.Intent.Message\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xfd\x01\n\x1d\x42\x61tchParametersStatusResponse\x12U\n\x12parameter_statuses\x18\x01 \x03(\x0b\x32\x39.ondewo.nlu.BatchParametersStatusResponse.ParameterStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\x1aq\n\x0fParameterStatus\x12\x31\n\tparameter\x18\x01 \x01(\x0b\x32\x1c.ondewo.nlu.Intent.ParameterH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x12\n\x10phrase_or_status\"\xdb\x01\n\x1c\x42\x61tchCreateParametersRequest\x12[\n\x12parameter_requests\x18\x01 \x03(\x0b\x32?.ondewo.nlu.BatchCreateParametersRequest.CreateParameterRequest\x1a^\n\x16\x43reateParameterRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12/\n\tparameter\x18\x02 \x01(\x0b\x32\x1c.ondewo.nlu.Intent.Parameter\"P\n\x1c\x42\x61tchUpdateParametersRequest\x12\x30\n\nparameters\x18\x01 \x03(\x0b\x32\x1c.ondewo.nlu.Intent.Parameter\"*\n\x19\x42\x61tchGetParametersRequest\x12\r\n\x05names\x18\x01 \x03(\t\"-\n\x1c\x42\x61tchDeleteParametersRequest\x12\r\n\x05names\x18\x01 \x03(\t\"\x88\x02\n\x1d\x42\x61tchDeleteParametersResponse\x12X\n\x0f\x64\x65lete_statuses\x18\x01 \x03(\x0b\x32?.ondewo.nlu.BatchDeleteParametersResponse.DeleteParameterStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\x1ay\n\x15\x44\x65leteParameterStatus\x12\x36\n\x14successfully_deleted\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x0f\n\rdelete_status\"W\n\x15ListParametersRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\npage_token\x18\x03 \x01(\t\"c\n\x16ListParametersResponse\x12\x30\n\nparameters\x18\x01 \x03(\x0b\x32\x1c.ondewo.nlu.Intent.Parameter\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x82\x01\n1ListTrainingPhrasesofIntentsWithEnrichmentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\nintent_ids\x18\x03 \x03(\t\x12\x12\n\npage_token\x18\x04 \x01(\t\"g\n2ListTrainingPhrasesofIntentsWithEnrichmentResponse\x12\x18\n\x10training_phrases\x18\x01 \x03(\t\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t*q\n\nIntentView\x12\x1b\n\x17INTENT_VIEW_UNSPECIFIED\x10\x00\x12\x14\n\x10INTENT_VIEW_FULL\x10\x01\x12\x17\n\x13INTENT_VIEW_PARTIAL\x10\x02\x12\x17\n\x13INTENT_VIEW_SHALLOW\x10\x03*\x9e\x01\n\x0eIntentCategory\x12\x0f\n\x0b\x41LL_INTENTS\x10\x00\x12\x13\n\x0f\x44\x45\x46\x41ULT_INTENTS\x10\x01\x12\x18\n\x14USER_DEFINED_INTENTS\x10\x02\x12\x18\n\x14\x44\x41TE_EXPIRED_INTENTS\x10\x03\x12\x17\n\x13\x44\x41TE_ACTIVE_INTENTS\x10\x04\x12\x19\n\x15\x44\x41TE_UPCOMING_INTENTS\x10\x05\x32\xbe\x19\n\x07Intents\x12}\n\x0bListIntents\x12\x1e.ondewo.nlu.ListIntentsRequest\x1a\x1f.ondewo.nlu.ListIntentsResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/v2/{parent=projects/*/agent}/intents\x12l\n\tGetIntent\x12\x1c.ondewo.nlu.GetIntentRequest\x1a\x12.ondewo.nlu.Intent\"-\x82\xd3\xe4\x93\x02\'\x12%/v2/{name=projects/*/agent/intents/*}\x12u\n\x0c\x43reateIntent\x12\x1f.ondewo.nlu.CreateIntentRequest\x1a\x12.ondewo.nlu.Intent\"0\x82\xd3\xe4\x93\x02*\"%/v2/{parent=projects/*/agent}/intents:\x01*\x12|\n\x0cUpdateIntent\x12\x1f.ondewo.nlu.UpdateIntentRequest\x1a\x12.ondewo.nlu.Intent\"7\x82\xd3\xe4\x93\x02\x31\x32,/v2/{intent.name=projects/*/agent/intents/*}:\x01*\x12v\n\x0c\x44\x65leteIntent\x12\x1f.ondewo.nlu.DeleteIntentRequest\x1a\x16.google.protobuf.Empty\"-\x82\xd3\xe4\x93\x02\'*%/v2/{name=projects/*/agent/intents/*}\x12\x90\x01\n\x12\x42\x61tchUpdateIntents\x12%.ondewo.nlu.BatchUpdateIntentsRequest\x1a\x15.ondewo.nlu.Operation\"<\x82\xd3\xe4\x93\x02\x36\"1/v2/{parent=projects/*/agent}/intents:batchUpdate:\x01*\x12\x90\x01\n\x12\x42\x61tchDeleteIntents\x12%.ondewo.nlu.BatchDeleteIntentsRequest\x1a\x15.ondewo.nlu.Operation\"<\x82\xd3\xe4\x93\x02\x36\"1/v2/{parent=projects/*/agent}/intents:batchDelete:\x01*\x12}\n\tTagIntent\x12\x1c.ondewo.nlu.IntentTagRequest\x1a\x16.google.protobuf.Empty\":\x82\xd3\xe4\x93\x02\x34\"//v2/{parent=projects/*/agent}/intents:tagIntent:\x01*\x12\x89\x01\n\x0f\x44\x65leteIntentTag\x12\x1c.ondewo.nlu.IntentTagRequest\x1a\x16.google.protobuf.Empty\"@\x82\xd3\xe4\x93\x02:\"5/v2/{parent=projects/*/agent}/intents:deleteIntentTag:\x01*\x12V\n\rGetIntentTags\x12 .ondewo.nlu.GetIntentTagsRequest\x1a!.ondewo.nlu.GetIntentTagsResponse\"\x00\x12\\\n\x10GetAllIntentTags\x12#.ondewo.nlu.GetAllIntentTagsRequest\x1a!.ondewo.nlu.GetIntentTagsResponse\"\x00\x12{\n\x1a\x42\x61tchCreateTrainingPhrases\x12-.ondewo.nlu.BatchCreateTrainingPhrasesRequest\x1a..ondewo.nlu.BatchTrainingPhrasesStatusResponse\x12u\n\x17\x42\x61tchGetTrainingPhrases\x12*.ondewo.nlu.BatchGetTrainingPhrasesRequest\x1a..ondewo.nlu.BatchTrainingPhrasesStatusResponse\x12{\n\x1a\x42\x61tchUpdateTrainingPhrases\x12-.ondewo.nlu.BatchUpdateTrainingPhrasesRequest\x1a..ondewo.nlu.BatchTrainingPhrasesStatusResponse\x12{\n\x1a\x42\x61tchDeleteTrainingPhrases\x12-.ondewo.nlu.BatchDeleteTrainingPhrasesRequest\x1a..ondewo.nlu.BatchDeleteTrainingPhrasesResponse\x12\x66\n\x13ListTrainingPhrases\x12&.ondewo.nlu.ListTrainingPhrasesRequest\x1a\'.ondewo.nlu.ListTrainingPhrasesResponse\x12~\n\x1b\x42\x61tchCreateResponseMessages\x12..ondewo.nlu.BatchCreateResponseMessagesRequest\x1a/.ondewo.nlu.BatchResponseMessagesStatusResponse\x12x\n\x18\x42\x61tchGetResponseMessages\x12+.ondewo.nlu.BatchGetResponseMessagesRequest\x1a/.ondewo.nlu.BatchResponseMessagesStatusResponse\x12~\n\x1b\x42\x61tchUpdateResponseMessages\x12..ondewo.nlu.BatchUpdateResponseMessagesRequest\x1a/.ondewo.nlu.BatchResponseMessagesStatusResponse\x12~\n\x1b\x42\x61tchDeleteResponseMessages\x12..ondewo.nlu.BatchDeleteResponseMessagesRequest\x1a/.ondewo.nlu.BatchDeleteResponseMessagesResponse\x12i\n\x14ListResponseMessages\x12\'.ondewo.nlu.ListResponseMessagesRequest\x1a(.ondewo.nlu.ListResponseMessagesResponse\x12l\n\x15\x42\x61tchCreateParameters\x12(.ondewo.nlu.BatchCreateParametersRequest\x1a).ondewo.nlu.BatchParametersStatusResponse\x12\x66\n\x12\x42\x61tchGetParameters\x12%.ondewo.nlu.BatchGetParametersRequest\x1a).ondewo.nlu.BatchParametersStatusResponse\x12l\n\x15\x42\x61tchUpdateParameters\x12(.ondewo.nlu.BatchUpdateParametersRequest\x1a).ondewo.nlu.BatchParametersStatusResponse\x12l\n\x15\x42\x61tchDeleteParameters\x12(.ondewo.nlu.BatchDeleteParametersRequest\x1a).ondewo.nlu.BatchDeleteParametersResponse\x12W\n\x0eListParameters\x12!.ondewo.nlu.ListParametersRequest\x1a\".ondewo.nlu.ListParametersResponse\x12\xab\x01\n*ListTrainingPhrasesofIntentsWithEnrichment\x12=.ondewo.nlu.ListTrainingPhrasesofIntentsWithEnrichmentRequest\x1a>.ondewo.nlu.ListTrainingPhrasesofIntentsWithEnrichmentResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17ondewo/nlu/intent.proto\x12\nondewo.nlu\x1a\x1cgoogle/api/annotations.proto\x1a\x18ondewo/nlu/context.proto\x1a\x17ondewo/nlu/common.proto\x1a\x1bondewo/nlu/operations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a google/protobuf/field_mask.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xcf\'\n\x06Intent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x36\n\rwebhook_state\x18\x06 \x01(\x0e\x32\x1f.ondewo.nlu.Intent.WebhookState\x12\x10\n\x08priority\x18\x03 \x01(\x05\x12\x13\n\x0bis_fallback\x18\x04 \x01(\x08\x12\x13\n\x0bml_disabled\x18\x13 \x01(\x08\x12\x1b\n\x13input_context_names\x18\x07 \x03(\t\x12\x0e\n\x06\x65vents\x18\x08 \x03(\t\x12;\n\x10training_phrases\x18\t \x03(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\x12\x0e\n\x06\x61\x63tion\x18\n \x01(\t\x12,\n\x0foutput_contexts\x18\x0b \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x16\n\x0ereset_contexts\x18\x0c \x01(\x08\x12\x30\n\nparameters\x18\r \x03(\x0b\x32\x1c.ondewo.nlu.Intent.Parameter\x12,\n\x08messages\x18\x0e \x03(\x0b\x32\x1a.ondewo.nlu.Intent.Message\x12G\n\x1a\x64\x65\x66\x61ult_response_platforms\x18\x0f \x03(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\x12!\n\x19root_followup_intent_name\x18\x10 \x01(\t\x12#\n\x1bparent_followup_intent_name\x18\x11 \x01(\t\x12\x43\n\x14\x66ollowup_intent_info\x18\x12 \x03(\x0b\x32%.ondewo.nlu.Intent.FollowupIntentInfo\x12\x17\n\x0fnext_page_token\x18\x1e \x01(\t\x12\x13\n\x0b\x64omain_name\x18\x1f \x01(\t\x12\x1d\n\x15is_start_of_deviation\x18  \x01(\x08\x12\x1b\n\x13is_end_of_deviation\x18! \x01(\x08\x12\x1d\n\x15training_phrase_count\x18\" \x01(\x05\x12/\n\x06status\x18# \x01(\x0e\x32\x1f.ondewo.nlu.Intent.IntentStatus\x12.\n\nstart_date\x18$ \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_date\x18% \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04tags\x18& \x03(\t\x1a\xe2\x03\n\x0eTrainingPhrase\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x34\n\x04type\x18\x02 \x01(\x0e\x32&.ondewo.nlu.Intent.TrainingPhrase.Type\x12\x0c\n\x04text\x18\x03 \x01(\t\x12:\n\x08\x65ntities\x18\x04 \x03(\x0b\x32(.ondewo.nlu.Intent.TrainingPhrase.Entity\x12\x19\n\x11times_added_count\x18\x05 \x01(\x05\x12\x15\n\rlanguage_code\x18\x06 \x01(\t\x1a\xd6\x01\n\x06\x45ntity\x12\x18\n\x10\x65ntity_type_name\x18\x01 \x01(\t\x12 \n\x18\x65ntity_type_display_name\x18\x03 \x01(\t\x12\x19\n\x11\x65ntity_value_name\x18\x04 \x01(\t\x12!\n\x19\x65ntity_value_display_name\x18\x05 \x01(\t\x12\r\n\x05start\x18\x06 \x01(\x05\x12\x0b\n\x03\x65nd\x18\x07 \x01(\x05\x12\x16\n\x0eparameter_name\x18\x08 \x01(\t\x12\x1e\n\x16parameter_display_name\x18\t \x01(\t\"7\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0b\n\x07\x45XAMPLE\x10\x01\x12\x0c\n\x08TEMPLATE\x10\x02\x1a\xa8\x02\n\tParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x15\n\rdefault_value\x18\x04 \x01(\t\x12\x18\n\x10\x65ntity_type_name\x18\x05 \x01(\t\x12 \n\x18\x65ntity_type_display_name\x18\x06 \x01(\t\x12\x11\n\tmandatory\x18\x07 \x01(\x08\x12\x34\n\x07prompts\x18\x08 \x03(\x0b\x32#.ondewo.nlu.Intent.Parameter.Prompt\x12\x0f\n\x07is_list\x18\t \x01(\x08\x1a;\n\x06Prompt\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x1a\x87\x18\n\x07Message\x12\x0c\n\x04name\x18\x10 \x01(\t\x12\x15\n\rlanguage_code\x18\x11 \x01(\t\x12/\n\x04text\x18\x01 \x01(\x0b\x32\x1f.ondewo.nlu.Intent.Message.TextH\x00\x12\x31\n\x05image\x18\x02 \x01(\x0b\x32 .ondewo.nlu.Intent.Message.ImageH\x00\x12@\n\rquick_replies\x18\x03 \x01(\x0b\x32\'.ondewo.nlu.Intent.Message.QuickRepliesH\x00\x12/\n\x04\x63\x61rd\x18\x04 \x01(\x0b\x32\x1f.ondewo.nlu.Intent.Message.CardH\x00\x12*\n\x07payload\x18\x05 \x01(\x0b\x32\x17.google.protobuf.StructH\x00\x12\x46\n\x10simple_responses\x18\x07 \x01(\x0b\x32*.ondewo.nlu.Intent.Message.SimpleResponsesH\x00\x12:\n\nbasic_card\x18\x08 \x01(\x0b\x32$.ondewo.nlu.Intent.Message.BasicCardH\x00\x12=\n\x0bsuggestions\x18\t \x01(\x0b\x32&.ondewo.nlu.Intent.Message.SuggestionsH\x00\x12K\n\x13link_out_suggestion\x18\n \x01(\x0b\x32,.ondewo.nlu.Intent.Message.LinkOutSuggestionH\x00\x12<\n\x0blist_select\x18\x0b \x01(\x0b\x32%.ondewo.nlu.Intent.Message.ListSelectH\x00\x12\x44\n\x0f\x63\x61rousel_select\x18\x0c \x01(\x0b\x32).ondewo.nlu.Intent.Message.CarouselSelectH\x00\x12\x38\n\thtml_text\x18\r \x01(\x0b\x32#.ondewo.nlu.Intent.Message.HTMLTextH\x00\x12\x31\n\x05video\x18\x0e \x01(\x0b\x32 .ondewo.nlu.Intent.Message.VideoH\x00\x12\x31\n\x05\x61udio\x18\x0f \x01(\x0b\x32 .ondewo.nlu.Intent.Message.AudioH\x00\x12\x35\n\x08platform\x18\x06 \x01(\x0e\x32#.ondewo.nlu.Intent.Message.Platform\x12\x11\n\tis_prompt\x18\x12 \x01(\x08\x1a\x14\n\x04Text\x12\x0c\n\x04text\x18\x01 \x03(\t\x1a\x36\n\x05Image\x12\x11\n\timage_uri\x18\x01 \x01(\t\x12\x1a\n\x12\x61\x63\x63\x65ssibility_text\x18\x02 \x01(\t\x1a\x34\n\x0cQuickReplies\x12\r\n\x05title\x18\x01 \x01(\t\x12\x15\n\rquick_replies\x18\x02 \x03(\t\x1a\x9d\x01\n\x04\x43\x61rd\x12\r\n\x05title\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x11\n\timage_uri\x18\x03 \x01(\t\x12\x37\n\x07\x62uttons\x18\x04 \x03(\x0b\x32&.ondewo.nlu.Intent.Message.Card.Button\x1a(\n\x06\x42utton\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x10\n\x08postback\x18\x02 \x01(\t\x1aL\n\x0eSimpleResponse\x12\x16\n\x0etext_to_speech\x18\x01 \x01(\t\x12\x0c\n\x04ssml\x18\x02 \x01(\t\x12\x14\n\x0c\x64isplay_text\x18\x03 \x01(\t\x1aV\n\x0fSimpleResponses\x12\x43\n\x10simple_responses\x18\x01 \x03(\x0b\x32).ondewo.nlu.Intent.Message.SimpleResponse\x1a\xbf\x02\n\tBasicCard\x12\r\n\x05title\x18\x01 \x01(\t\x12\x10\n\x08subtitle\x18\x02 \x01(\t\x12\x16\n\x0e\x66ormatted_text\x18\x03 \x01(\t\x12/\n\x05image\x18\x04 \x01(\x0b\x32 .ondewo.nlu.Intent.Message.Image\x12<\n\x07\x62uttons\x18\x05 \x03(\x0b\x32+.ondewo.nlu.Intent.Message.BasicCard.Button\x1a\x89\x01\n\x06\x42utton\x12\r\n\x05title\x18\x01 \x01(\t\x12R\n\x0fopen_uri_action\x18\x02 \x01(\x0b\x32\x39.ondewo.nlu.Intent.Message.BasicCard.Button.OpenUriAction\x1a\x1c\n\rOpenUriAction\x12\x0b\n\x03uri\x18\x01 \x01(\t\x1a\x1b\n\nSuggestion\x12\r\n\x05title\x18\x01 \x01(\t\x1aI\n\x0bSuggestions\x12:\n\x0bsuggestions\x18\x01 \x03(\x0b\x32%.ondewo.nlu.Intent.Message.Suggestion\x1a:\n\x11LinkOutSuggestion\x12\x18\n\x10\x64\x65stination_name\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x1a\xed\x01\n\nListSelect\x12\r\n\x05title\x18\x01 \x01(\t\x12\x39\n\x05items\x18\x02 \x03(\x0b\x32*.ondewo.nlu.Intent.Message.ListSelect.Item\x1a\x94\x01\n\x04Item\x12\x37\n\x04info\x18\x01 \x01(\x0b\x32).ondewo.nlu.Intent.Message.SelectItemInfo\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12/\n\x05image\x18\x04 \x01(\x0b\x32 .ondewo.nlu.Intent.Message.Image\x1a\xe6\x01\n\x0e\x43\x61rouselSelect\x12=\n\x05items\x18\x01 \x03(\x0b\x32..ondewo.nlu.Intent.Message.CarouselSelect.Item\x1a\x94\x01\n\x04Item\x12\x37\n\x04info\x18\x01 \x01(\x0b\x32).ondewo.nlu.Intent.Message.SelectItemInfo\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12/\n\x05image\x18\x04 \x01(\x0b\x32 .ondewo.nlu.Intent.Message.Image\x1a\x18\n\x08HTMLText\x12\x0c\n\x04text\x18\x01 \x03(\t\x1a\x30\n\x05Video\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x1a\n\x12\x61\x63\x63\x65ssibility_text\x18\x02 \x01(\t\x1a\x30\n\x05\x41udio\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x1a\n\x12\x61\x63\x63\x65ssibility_text\x18\x02 \x01(\t\x1a/\n\x0eSelectItemInfo\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x10\n\x08synonyms\x18\x02 \x03(\t\"\x92\x04\n\x08Platform\x12\x18\n\x14PLATFORM_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x46\x41\x43\x45\x42OOK\x10\x01\x12\t\n\x05SLACK\x10\x02\x12\x0c\n\x08TELEGRAM\x10\x03\x12\x07\n\x03KIK\x10\x04\x12\t\n\x05SKYPE\x10\x05\x12\x08\n\x04LINE\x10\x06\x12\t\n\x05VIBER\x10\x07\x12\x15\n\x11\x41\x43TIONS_ON_GOOGLE\x10\x08\x12\x11\n\rPLACEHOLDER_1\x10\t\x12\x11\n\rPLACEHOLDER_2\x10\n\x12\x11\n\rPLACEHOLDER_3\x10\x0b\x12\x11\n\rPLACEHOLDER_4\x10\x0c\x12\x11\n\rPLACEHOLDER_5\x10\r\x12\x11\n\rPLACEHOLDER_6\x10\x0e\x12\x11\n\rPLACEHOLDER_7\x10\x0f\x12\x11\n\rPLACEHOLDER_8\x10\x10\x12\x11\n\rPLACEHOLDER_9\x10\x11\x12\x12\n\x0ePLACEHOLDER_10\x10\x12\x12\x12\n\x0ePLACEHOLDER_11\x10\x13\x12\x12\n\x0ePLACEHOLDER_12\x10\x14\x12\x12\n\x0ePLACEHOLDER_13\x10\x15\x12\x12\n\x0ePLACEHOLDER_14\x10\x16\x12\x12\n\x0ePLACEHOLDER_15\x10\x17\x12\x12\n\x0ePLACEHOLDER_16\x10\x18\x12\x12\n\x0ePLACEHOLDER_17\x10\x19\x12\x12\n\x0ePLACEHOLDER_18\x10\x1a\x12\x12\n\x0ePLACEHOLDER_19\x10\x1b\x12\x12\n\x0ePLACEHOLDER_20\x10\x1c\x42\t\n\x07message\x1aW\n\x12\x46ollowupIntentInfo\x12\x1c\n\x14\x66ollowup_intent_name\x18\x01 \x01(\t\x12#\n\x1bparent_followup_intent_name\x18\x02 \x01(\t\"(\n\x0cIntentStatus\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08INACTIVE\x10\x01\"t\n\x0cWebhookState\x12\x1d\n\x19WEBHOOK_STATE_UNSPECIFIED\x10\x00\x12\x19\n\x15WEBHOOK_STATE_ENABLED\x10\x01\x12*\n&WEBHOOK_STATE_ENABLED_FOR_SLOT_FILLING\x10\x02\"\xfe\x01\n\x12ListIntentsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12+\n\x0bintent_view\x18\x03 \x01(\x0e\x32\x16.ondewo.nlu.IntentView\x12\x12\n\npage_token\x18\x05 \x01(\t\x12\x36\n\x12\x66ilter_by_category\x18\x06 \x01(\x0e\x32\x1a.ondewo.nlu.IntentCategory\x12\x30\n\rsort_by_field\x18\x07 \x01(\x0b\x32\x19.ondewo.nlu.IntentSorting\x12\x16\n\x0e\x66ilter_by_tags\x18\x08 \x03(\t\"S\n\x13ListIntentsResponse\x12#\n\x07intents\x18\x01 \x03(\x0b\x32\x12.ondewo.nlu.Intent\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"x\n\x10GetIntentRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12+\n\x0bintent_view\x18\x03 \x01(\x0e\x32\x16.ondewo.nlu.IntentView\x12\x12\n\npage_token\x18\n \x01(\t\"\x8d\x01\n\x13\x43reateIntentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\"\n\x06intent\x18\x02 \x01(\x0b\x32\x12.ondewo.nlu.Intent\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12+\n\x0bintent_view\x18\x04 \x01(\x0e\x32\x16.ondewo.nlu.IntentView\"\xae\x01\n\x13UpdateIntentRequest\x12\"\n\x06intent\x18\x01 \x01(\x0b\x32\x12.ondewo.nlu.Intent\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12/\n\x0bupdate_mask\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12+\n\x0bintent_view\x18\x04 \x01(\x0e\x32\x16.ondewo.nlu.IntentView\"#\n\x13\x44\x65leteIntentRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x84\x02\n\x19\x42\x61tchUpdateIntentsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x1a\n\x10intent_batch_uri\x18\x02 \x01(\tH\x00\x12\x36\n\x13intent_batch_inline\x18\x03 \x01(\x0b\x32\x17.ondewo.nlu.IntentBatchH\x00\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12/\n\x0bupdate_mask\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12+\n\x0bintent_view\x18\x06 \x01(\x0e\x32\x16.ondewo.nlu.IntentViewB\x0e\n\x0cintent_batch\"A\n\x1a\x42\x61tchUpdateIntentsResponse\x12#\n\x07intents\x18\x01 \x03(\x0b\x32\x12.ondewo.nlu.Intent\"P\n\x19\x42\x61tchDeleteIntentsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12#\n\x07intents\x18\x02 \x03(\x0b\x32\x12.ondewo.nlu.Intent\"2\n\x0bIntentBatch\x12#\n\x07intents\x18\x01 \x03(\x0b\x32\x12.ondewo.nlu.Intent\"\xec\x02\n\rIntentSorting\x12\x43\n\rsorting_field\x18\x01 \x01(\x0e\x32,.ondewo.nlu.IntentSorting.IntentSortingField\x12-\n\x0csorting_mode\x18\x02 \x01(\x0e\x32\x17.ondewo.nlu.SortingMode\"\xe6\x01\n\x12IntentSortingField\x12\x15\n\x11NO_INTENT_SORTING\x10\x00\x12\x17\n\x13SORT_INTENT_BY_NAME\x10\x01\x12 \n\x1cSORT_INTENT_BY_CREATION_DATE\x10\x02\x12\x1f\n\x1bSORT_INTENT_BY_LAST_UPDATED\x10\x03\x12!\n\x1dSORT_INTENT_BY_USERSAYS_COUNT\x10\x04\x12\x1d\n\x19SORT_INTENT_BY_START_DATE\x10\x05\x12\x1b\n\x17SORT_INTENT_BY_END_DATE\x10\x06\"5\n\x10IntentTagRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12\x0c\n\x04tags\x18\x02 \x03(\t\"+\n\x14GetIntentTagsRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\",\n\x15GetIntentTagsResponse\x12\x13\n\x0bintent_tags\x18\x01 \x03(\t\")\n\x17GetAllIntentTagsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\"`\n!BatchUpdateTrainingPhrasesRequest\x12;\n\x10training_phrases\x18\x01 \x03(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\"\x81\x01\n\x14TrainingPhraseStatus\x12<\n\x0ftraining_phrase\x18\x01 \x01(\x0b\x32!.ondewo.nlu.Intent.TrainingPhraseH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x12\n\x10phrase_or_status\"|\n\"BatchTrainingPhrasesStatusResponse\x12\x42\n\x18training_phrase_statuses\x18\x01 \x03(\x0b\x32 .ondewo.nlu.TrainingPhraseStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\"\x80\x02\n!BatchCreateTrainingPhrasesRequest\x12k\n\x18training_phrase_requests\x18\x01 \x03(\x0b\x32I.ondewo.nlu.BatchCreateTrainingPhrasesRequest.CreateTrainingPhraseRequest\x1an\n\x1b\x43reateTrainingPhraseRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12:\n\x0ftraining_phrase\x18\x02 \x01(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\"/\n\x1e\x42\x61tchGetTrainingPhrasesRequest\x12\r\n\x05names\x18\x01 \x03(\t\"2\n!BatchDeleteTrainingPhrasesRequest\x12\r\n\x05names\x18\x01 \x03(\t\"\x9c\x02\n\"BatchDeleteTrainingPhrasesResponse\x12\x62\n\x0f\x64\x65lete_statuses\x18\x01 \x03(\x0b\x32I.ondewo.nlu.BatchDeleteTrainingPhrasesResponse.DeleteTrainingPhraseStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\x1a~\n\x1a\x44\x65leteTrainingPhraseStatus\x12\x36\n\x14successfully_deleted\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x0f\n\rdelete_status\"\\\n\x1aListTrainingPhrasesRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\npage_token\x18\x03 \x01(\t\"s\n\x1bListTrainingPhrasesResponse\x12;\n\x10training_phrases\x18\x01 \x03(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xa1\x02\n#BatchResponseMessagesStatusResponse\x12h\n\x19response_message_statuses\x18\x01 \x03(\x0b\x32\x45.ondewo.nlu.BatchResponseMessagesStatusResponse.ResponseMessageStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\x1a|\n\x15ResponseMessageStatus\x12\x36\n\x10response_message\x18\x01 \x01(\x0b\x32\x1a.ondewo.nlu.Intent.MessageH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x12\n\x10phrase_or_status\"\xff\x01\n\"BatchCreateResponseMessagesRequest\x12n\n\x19response_message_requests\x18\x01 \x03(\x0b\x32K.ondewo.nlu.BatchCreateResponseMessagesRequest.CreateResponseMessageRequest\x1ai\n\x1c\x43reateResponseMessageRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12\x34\n\x10response_message\x18\x02 \x01(\x0b\x32\x1a.ondewo.nlu.Intent.Message\"[\n\"BatchUpdateResponseMessagesRequest\x12\x35\n\x11response_messages\x18\x01 \x03(\x0b\x32\x1a.ondewo.nlu.Intent.Message\"0\n\x1f\x42\x61tchGetResponseMessagesRequest\x12\r\n\x05names\x18\x01 \x03(\t\"3\n\"BatchDeleteResponseMessagesRequest\x12\r\n\x05names\x18\x01 \x03(\t\"\xa0\x02\n#BatchDeleteResponseMessagesResponse\x12\x64\n\x0f\x64\x65lete_statuses\x18\x01 \x03(\x0b\x32K.ondewo.nlu.BatchDeleteResponseMessagesResponse.DeleteResponseMessageStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\x1a\x7f\n\x1b\x44\x65leteResponseMessageStatus\x12\x36\n\x14successfully_deleted\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x0f\n\rdelete_status\"]\n\x1bListResponseMessagesRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\npage_token\x18\x03 \x01(\t\"n\n\x1cListResponseMessagesResponse\x12\x35\n\x11response_messages\x18\x01 \x03(\x0b\x32\x1a.ondewo.nlu.Intent.Message\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xfd\x01\n\x1d\x42\x61tchParametersStatusResponse\x12U\n\x12parameter_statuses\x18\x01 \x03(\x0b\x32\x39.ondewo.nlu.BatchParametersStatusResponse.ParameterStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\x1aq\n\x0fParameterStatus\x12\x31\n\tparameter\x18\x01 \x01(\x0b\x32\x1c.ondewo.nlu.Intent.ParameterH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x12\n\x10phrase_or_status\"\xdb\x01\n\x1c\x42\x61tchCreateParametersRequest\x12[\n\x12parameter_requests\x18\x01 \x03(\x0b\x32?.ondewo.nlu.BatchCreateParametersRequest.CreateParameterRequest\x1a^\n\x16\x43reateParameterRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12/\n\tparameter\x18\x02 \x01(\x0b\x32\x1c.ondewo.nlu.Intent.Parameter\"P\n\x1c\x42\x61tchUpdateParametersRequest\x12\x30\n\nparameters\x18\x01 \x03(\x0b\x32\x1c.ondewo.nlu.Intent.Parameter\"*\n\x19\x42\x61tchGetParametersRequest\x12\r\n\x05names\x18\x01 \x03(\t\"-\n\x1c\x42\x61tchDeleteParametersRequest\x12\r\n\x05names\x18\x01 \x03(\t\"\x88\x02\n\x1d\x42\x61tchDeleteParametersResponse\x12X\n\x0f\x64\x65lete_statuses\x18\x01 \x03(\x0b\x32?.ondewo.nlu.BatchDeleteParametersResponse.DeleteParameterStatus\x12\x12\n\nhas_errors\x18\x02 \x01(\x08\x1ay\n\x15\x44\x65leteParameterStatus\x12\x36\n\x14successfully_deleted\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x12\x17\n\rerror_message\x18\x02 \x01(\tH\x00\x42\x0f\n\rdelete_status\"W\n\x15ListParametersRequest\x12\x13\n\x0bintent_name\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\npage_token\x18\x03 \x01(\t\"c\n\x16ListParametersResponse\x12\x30\n\nparameters\x18\x01 \x03(\x0b\x32\x1c.ondewo.nlu.Intent.Parameter\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x82\x01\n1ListTrainingPhrasesofIntentsWithEnrichmentRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x12\n\nintent_ids\x18\x03 \x03(\t\x12\x12\n\npage_token\x18\x04 \x01(\t\"g\n2ListTrainingPhrasesofIntentsWithEnrichmentResponse\x12\x18\n\x10training_phrases\x18\x01 \x03(\t\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t*\x8a\x01\n\nIntentView\x12\x1b\n\x17INTENT_VIEW_UNSPECIFIED\x10\x00\x12\x14\n\x10INTENT_VIEW_FULL\x10\x01\x12\x17\n\x13INTENT_VIEW_PARTIAL\x10\x02\x12\x17\n\x13INTENT_VIEW_SHALLOW\x10\x03\x12\x17\n\x13INTENT_VIEW_MINIMUM\x10\x04*\x9e\x01\n\x0eIntentCategory\x12\x0f\n\x0b\x41LL_INTENTS\x10\x00\x12\x13\n\x0f\x44\x45\x46\x41ULT_INTENTS\x10\x01\x12\x18\n\x14USER_DEFINED_INTENTS\x10\x02\x12\x18\n\x14\x44\x41TE_EXPIRED_INTENTS\x10\x03\x12\x17\n\x13\x44\x41TE_ACTIVE_INTENTS\x10\x04\x12\x19\n\x15\x44\x41TE_UPCOMING_INTENTS\x10\x05\x32\xbe\x19\n\x07Intents\x12}\n\x0bListIntents\x12\x1e.ondewo.nlu.ListIntentsRequest\x1a\x1f.ondewo.nlu.ListIntentsResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/v2/{parent=projects/*/agent}/intents\x12l\n\tGetIntent\x12\x1c.ondewo.nlu.GetIntentRequest\x1a\x12.ondewo.nlu.Intent\"-\x82\xd3\xe4\x93\x02\'\x12%/v2/{name=projects/*/agent/intents/*}\x12u\n\x0c\x43reateIntent\x12\x1f.ondewo.nlu.CreateIntentRequest\x1a\x12.ondewo.nlu.Intent\"0\x82\xd3\xe4\x93\x02*\"%/v2/{parent=projects/*/agent}/intents:\x01*\x12|\n\x0cUpdateIntent\x12\x1f.ondewo.nlu.UpdateIntentRequest\x1a\x12.ondewo.nlu.Intent\"7\x82\xd3\xe4\x93\x02\x31\x32,/v2/{intent.name=projects/*/agent/intents/*}:\x01*\x12v\n\x0c\x44\x65leteIntent\x12\x1f.ondewo.nlu.DeleteIntentRequest\x1a\x16.google.protobuf.Empty\"-\x82\xd3\xe4\x93\x02\'*%/v2/{name=projects/*/agent/intents/*}\x12\x90\x01\n\x12\x42\x61tchUpdateIntents\x12%.ondewo.nlu.BatchUpdateIntentsRequest\x1a\x15.ondewo.nlu.Operation\"<\x82\xd3\xe4\x93\x02\x36\"1/v2/{parent=projects/*/agent}/intents:batchUpdate:\x01*\x12\x90\x01\n\x12\x42\x61tchDeleteIntents\x12%.ondewo.nlu.BatchDeleteIntentsRequest\x1a\x15.ondewo.nlu.Operation\"<\x82\xd3\xe4\x93\x02\x36\"1/v2/{parent=projects/*/agent}/intents:batchDelete:\x01*\x12}\n\tTagIntent\x12\x1c.ondewo.nlu.IntentTagRequest\x1a\x16.google.protobuf.Empty\":\x82\xd3\xe4\x93\x02\x34\"//v2/{parent=projects/*/agent}/intents:tagIntent:\x01*\x12\x89\x01\n\x0f\x44\x65leteIntentTag\x12\x1c.ondewo.nlu.IntentTagRequest\x1a\x16.google.protobuf.Empty\"@\x82\xd3\xe4\x93\x02:\"5/v2/{parent=projects/*/agent}/intents:deleteIntentTag:\x01*\x12V\n\rGetIntentTags\x12 .ondewo.nlu.GetIntentTagsRequest\x1a!.ondewo.nlu.GetIntentTagsResponse\"\x00\x12\\\n\x10GetAllIntentTags\x12#.ondewo.nlu.GetAllIntentTagsRequest\x1a!.ondewo.nlu.GetIntentTagsResponse\"\x00\x12{\n\x1a\x42\x61tchCreateTrainingPhrases\x12-.ondewo.nlu.BatchCreateTrainingPhrasesRequest\x1a..ondewo.nlu.BatchTrainingPhrasesStatusResponse\x12u\n\x17\x42\x61tchGetTrainingPhrases\x12*.ondewo.nlu.BatchGetTrainingPhrasesRequest\x1a..ondewo.nlu.BatchTrainingPhrasesStatusResponse\x12{\n\x1a\x42\x61tchUpdateTrainingPhrases\x12-.ondewo.nlu.BatchUpdateTrainingPhrasesRequest\x1a..ondewo.nlu.BatchTrainingPhrasesStatusResponse\x12{\n\x1a\x42\x61tchDeleteTrainingPhrases\x12-.ondewo.nlu.BatchDeleteTrainingPhrasesRequest\x1a..ondewo.nlu.BatchDeleteTrainingPhrasesResponse\x12\x66\n\x13ListTrainingPhrases\x12&.ondewo.nlu.ListTrainingPhrasesRequest\x1a\'.ondewo.nlu.ListTrainingPhrasesResponse\x12~\n\x1b\x42\x61tchCreateResponseMessages\x12..ondewo.nlu.BatchCreateResponseMessagesRequest\x1a/.ondewo.nlu.BatchResponseMessagesStatusResponse\x12x\n\x18\x42\x61tchGetResponseMessages\x12+.ondewo.nlu.BatchGetResponseMessagesRequest\x1a/.ondewo.nlu.BatchResponseMessagesStatusResponse\x12~\n\x1b\x42\x61tchUpdateResponseMessages\x12..ondewo.nlu.BatchUpdateResponseMessagesRequest\x1a/.ondewo.nlu.BatchResponseMessagesStatusResponse\x12~\n\x1b\x42\x61tchDeleteResponseMessages\x12..ondewo.nlu.BatchDeleteResponseMessagesRequest\x1a/.ondewo.nlu.BatchDeleteResponseMessagesResponse\x12i\n\x14ListResponseMessages\x12\'.ondewo.nlu.ListResponseMessagesRequest\x1a(.ondewo.nlu.ListResponseMessagesResponse\x12l\n\x15\x42\x61tchCreateParameters\x12(.ondewo.nlu.BatchCreateParametersRequest\x1a).ondewo.nlu.BatchParametersStatusResponse\x12\x66\n\x12\x42\x61tchGetParameters\x12%.ondewo.nlu.BatchGetParametersRequest\x1a).ondewo.nlu.BatchParametersStatusResponse\x12l\n\x15\x42\x61tchUpdateParameters\x12(.ondewo.nlu.BatchUpdateParametersRequest\x1a).ondewo.nlu.BatchParametersStatusResponse\x12l\n\x15\x42\x61tchDeleteParameters\x12(.ondewo.nlu.BatchDeleteParametersRequest\x1a).ondewo.nlu.BatchDeleteParametersResponse\x12W\n\x0eListParameters\x12!.ondewo.nlu.ListParametersRequest\x1a\".ondewo.nlu.ListParametersResponse\x12\xab\x01\n*ListTrainingPhrasesofIntentsWithEnrichment\x12=.ondewo.nlu.ListTrainingPhrasesofIntentsWithEnrichmentRequest\x1a>.ondewo.nlu.ListTrainingPhrasesofIntentsWithEnrichmentResponseb\x06proto3')
 
 _INTENTVIEW = DESCRIPTOR.enum_types_by_name['IntentView']
 IntentView = enum_type_wrapper.EnumTypeWrapper(_INTENTVIEW)
 _INTENTCATEGORY = DESCRIPTOR.enum_types_by_name['IntentCategory']
 IntentCategory = enum_type_wrapper.EnumTypeWrapper(_INTENTCATEGORY)
 INTENT_VIEW_UNSPECIFIED = 0
 INTENT_VIEW_FULL = 1
 INTENT_VIEW_PARTIAL = 2
 INTENT_VIEW_SHALLOW = 3
+INTENT_VIEW_MINIMUM = 4
 ALL_INTENTS = 0
 DEFAULT_INTENTS = 1
 USER_DEFINED_INTENTS = 2
 DATE_EXPIRED_INTENTS = 3
 DATE_ACTIVE_INTENTS = 4
 DATE_UPCOMING_INTENTS = 5
 
@@ -686,18 +687,18 @@
     _INTENTS.methods_by_name['BatchUpdateIntents']._serialized_options = b'\202\323\344\223\0026\"1/v2/{parent=projects/*/agent}/intents:batchUpdate:\001*'
     _INTENTS.methods_by_name['BatchDeleteIntents']._options = None
     _INTENTS.methods_by_name['BatchDeleteIntents']._serialized_options = b'\202\323\344\223\0026\"1/v2/{parent=projects/*/agent}/intents:batchDelete:\001*'
     _INTENTS.methods_by_name['TagIntent']._options = None
     _INTENTS.methods_by_name['TagIntent']._serialized_options = b'\202\323\344\223\0024\"//v2/{parent=projects/*/agent}/intents:tagIntent:\001*'
     _INTENTS.methods_by_name['DeleteIntentTag']._options = None
     _INTENTS.methods_by_name['DeleteIntentTag']._serialized_options = b'\202\323\344\223\002:\"5/v2/{parent=projects/*/agent}/intents:deleteIntentTag:\001*'
-    _INTENTVIEW._serialized_start = 10995
-    _INTENTVIEW._serialized_end = 11108
-    _INTENTCATEGORY._serialized_start = 11111
-    _INTENTCATEGORY._serialized_end = 11269
+    _INTENTVIEW._serialized_start = 10996
+    _INTENTVIEW._serialized_end = 11134
+    _INTENTCATEGORY._serialized_start = 11137
+    _INTENTCATEGORY._serialized_end = 11295
     _INTENT._serialized_start = 276
     _INTENT._serialized_end = 5347
     _INTENT_TRAININGPHRASE._serialized_start = 1235
     _INTENT_TRAININGPHRASE._serialized_end = 1717
     _INTENT_TRAININGPHRASE_ENTITY._serialized_start = 1446
     _INTENT_TRAININGPHRASE_ENTITY._serialized_end = 1660
     _INTENT_TRAININGPHRASE_TYPE._serialized_start = 1662
@@ -856,10 +857,10 @@
     _LISTPARAMETERSREQUEST._serialized_end = 10654
     _LISTPARAMETERSRESPONSE._serialized_start = 10656
     _LISTPARAMETERSRESPONSE._serialized_end = 10755
     _LISTTRAININGPHRASESOFINTENTSWITHENRICHMENTREQUEST._serialized_start = 10758
     _LISTTRAININGPHRASESOFINTENTSWITHENRICHMENTREQUEST._serialized_end = 10888
     _LISTTRAININGPHRASESOFINTENTSWITHENRICHMENTRESPONSE._serialized_start = 10890
     _LISTTRAININGPHRASESOFINTENTSWITHENRICHMENTRESPONSE._serialized_end = 10993
-    _INTENTS._serialized_start = 11272
-    _INTENTS._serialized_end = 14534
+    _INTENTS._serialized_start = 11298
+    _INTENTS._serialized_end = 14560
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/intent_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/intent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/operation_metadata_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/operation_metadata_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#ondewo/nlu/operation_metadata.proto\x12\nondewo.nlu\x1a\x1fgoogle/protobuf/timestamp.proto\"\xee\x06\n\x11OperationMetadata\x12\x34\n\x06status\x18\x01 \x01(\x0e\x32$.ondewo.nlu.OperationMetadata.Status\x12\x1d\n\x15parent_operation_name\x18\x02 \x01(\t\x12\x1b\n\x13sub_operation_names\x18\x03 \x03(\t\x12/\n\x0b\x63reate_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12!\n\x19is_cancellation_requested\x18\x07 \x01(\x08\x12\x16\n\x0e\x63\x61ncel_command\x18\x08 \x01(\t\x12\x17\n\x0fuser_id_created\x18\t \x01(\t\x12\x19\n\x11user_id_cancelled\x18\n \x01(\t\x12\x16\n\x0eproject_parent\x18\x0b \x01(\t\x12\x43\n\x0eoperation_type\x18\x0c \x01(\x0e\x32+.ondewo.nlu.OperationMetadata.OperationType\x12\x11\n\thost_name\x18\r \x01(\t\x12\x12\n\nnum_reruns\x18\x0e \x01(\x05\x12\x16\n\x0emax_num_reruns\x18\x0f \x01(\x05\x12\x13\n\x0b\x64\x65scription\x18\x10 \x01(\t\"g\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bNOT_STARTED\x10\x01\x12\x0f\n\x0bIN_PROGRESS\x10\x02\x12\x08\n\x04\x44ONE\x10\x03\x12\r\n\tCANCELLED\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\"\xce\x01\n\rOperationType\x12\x1e\n\x1aOPERATION_TYPE_UNSPECIFIED\x10\x00\x12\x10\n\x0c\x43REATE_AGENT\x10\x01\x12\x10\n\x0cIMPORT_AGENT\x10\x02\x12\x10\n\x0c\x45XPORT_AGENT\x10\x03\x12\x10\n\x0c\x44\x45LETE_AGENT\x10\x04\x12\x11\n\rRESTORE_AGENT\x10\x05\x12\x15\n\x11\x42UILD_AGENT_CACHE\x10\x06\x12\x0f\n\x0bTRAIN_AGENT\x10\x07\x12\x1a\n\x16\x45XPORT_BENCHMARK_AGENT\x10\x08\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#ondewo/nlu/operation_metadata.proto\x12\nondewo.nlu\x1a\x1fgoogle/protobuf/timestamp.proto\"\x8e\x07\n\x11OperationMetadata\x12\x34\n\x06status\x18\x01 \x01(\x0e\x32$.ondewo.nlu.OperationMetadata.Status\x12\x1d\n\x15parent_operation_name\x18\x02 \x01(\t\x12\x1b\n\x13sub_operation_names\x18\x03 \x03(\t\x12/\n\x0b\x63reate_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12!\n\x19is_cancellation_requested\x18\x07 \x01(\x08\x12\x16\n\x0e\x63\x61ncel_command\x18\x08 \x01(\t\x12\x17\n\x0fuser_id_created\x18\t \x01(\t\x12\x19\n\x11user_id_cancelled\x18\n \x01(\t\x12\x16\n\x0eproject_parent\x18\x0b \x01(\t\x12\x43\n\x0eoperation_type\x18\x0c \x01(\x0e\x32+.ondewo.nlu.OperationMetadata.OperationType\x12\x11\n\thost_name\x18\r \x01(\t\x12\x12\n\nnum_reruns\x18\x0e \x01(\x05\x12\x16\n\x0emax_num_reruns\x18\x0f \x01(\x05\x12\x13\n\x0b\x64\x65scription\x18\x10 \x01(\t\x12\x0b\n\x03log\x18\x11 \x03(\t\x12\x11\n\tlog_limit\x18\x12 \x01(\x05\"g\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x0f\n\x0bNOT_STARTED\x10\x01\x12\x0f\n\x0bIN_PROGRESS\x10\x02\x12\x08\n\x04\x44ONE\x10\x03\x12\r\n\tCANCELLED\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\"\xce\x01\n\rOperationType\x12\x1e\n\x1aOPERATION_TYPE_UNSPECIFIED\x10\x00\x12\x10\n\x0c\x43REATE_AGENT\x10\x01\x12\x10\n\x0cIMPORT_AGENT\x10\x02\x12\x10\n\x0c\x45XPORT_AGENT\x10\x03\x12\x10\n\x0c\x44\x45LETE_AGENT\x10\x04\x12\x11\n\rRESTORE_AGENT\x10\x05\x12\x15\n\x11\x42UILD_AGENT_CACHE\x10\x06\x12\x0f\n\x0bTRAIN_AGENT\x10\x07\x12\x1a\n\x16\x45XPORT_BENCHMARK_AGENT\x10\x08\x62\x06proto3')
 
 
 _OPERATIONMETADATA = DESCRIPTOR.message_types_by_name['OperationMetadata']
 _OPERATIONMETADATA_STATUS = _OPERATIONMETADATA.enum_types_by_name['Status']
 _OPERATIONMETADATA_OPERATIONTYPE = _OPERATIONMETADATA.enum_types_by_name['OperationType']
 OperationMetadata = _reflection.GeneratedProtocolMessageType('OperationMetadata', (_message.Message,), {
     'DESCRIPTOR': _OPERATIONMETADATA,
@@ -26,13 +26,13 @@
 })
 _sym_db.RegisterMessage(OperationMetadata)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
     _OPERATIONMETADATA._serialized_start = 85
-    _OPERATIONMETADATA._serialized_end = 963
-    _OPERATIONMETADATA_STATUS._serialized_start = 651
-    _OPERATIONMETADATA_STATUS._serialized_end = 754
-    _OPERATIONMETADATA_OPERATIONTYPE._serialized_start = 757
-    _OPERATIONMETADATA_OPERATIONTYPE._serialized_end = 963
+    _OPERATIONMETADATA._serialized_end = 995
+    _OPERATIONMETADATA_STATUS._serialized_start = 683
+    _OPERATIONMETADATA_STATUS._serialized_end = 786
+    _OPERATIONMETADATA_OPERATIONTYPE._serialized_start = 789
+    _OPERATIONMETADATA_OPERATIONTYPE._serialized_end = 995
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/operations_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/operations_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/operations_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,19 +90,19 @@
 
     def CancelOperation(self, request, context):
         """Starts asynchronous cancellation on a long-running operation.  The server
         makes a best effort to cancel the operation, but success is not
         guaranteed.  If the server doesn't support this method, it returns
         `google.rpc.Code.UNIMPLEMENTED`.  Clients can use
         [Operations.GetOperation][ondewo.nlu.Operations.GetOperation] or
-        other methods to check whether the cancellation succeeded or whether the
+        other methods to verify whether the cancellation succeeded or whether the
         operation completed despite cancellation. On successful cancellation,
         the operation is not deleted; instead, it becomes an operation with
-        an [Operation.error][ondewo.nlu.Operation.error] value with a [google.rpc.Status.code][google.rpc.Status.code] of 1,
-        corresponding to `Code.CANCELLED`.
+        an [Operation.error][ondewo.nlu.Operation.error] value with a [google.rpc.Status.code][google.rpc.Status.code]
+        of 1, corresponding to `Code.CANCELLED`.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_OperationsServicer_to_server(servicer, server):
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/project_role_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/project_role_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/project_role_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/project_role_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import grpc
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from ondewo.nlu import project_role_pb2 as ondewo_dot_nlu_dot_project__role__pb2
 
 
 class ProjectRolesStub(object):
-    """Missing associated documentation comment in .proto file."""
+    """Project roles
+    """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
@@ -39,42 +40,48 @@
             '/ondewo.nlu.ProjectRoles/ListProjectRoles',
             request_serializer=ondewo_dot_nlu_dot_project__role__pb2.ListProjectRolesRequest.SerializeToString,
             response_deserializer=ondewo_dot_nlu_dot_project__role__pb2.ListProjectRolesResponse.FromString,
         )
 
 
 class ProjectRolesServicer(object):
-    """Missing associated documentation comment in .proto file."""
+    """Project roles
+    """
 
     def CreateProjectRole(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Creates a project role by creating the knowledge base master
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetProjectRole(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Creates a project role by getting the knowledge base master
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteProjectRole(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Deletes project role
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def UpdateProjectRole(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Updates project role
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListProjectRoles(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """List project roles
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_ProjectRolesServicer_to_server(servicer, server):
     rpc_method_handlers = {
@@ -108,15 +115,16 @@
         'ondewo.nlu.ProjectRoles', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
  # This class is part of an EXPERIMENTAL API.
 
 
 class ProjectRoles(object):
-    """Missing associated documentation comment in .proto file."""
+    """Project roles
+    """
 
     @staticmethod
     def CreateProjectRole(request,
                           target,
                           options=(),
                           channel_credentials=None,
                           call_credentials=None,
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/project_statistics_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/project_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/project_statistics_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/project_statistics_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import grpc
 
 from ondewo.nlu import common_pb2 as ondewo_dot_nlu_dot_common__pb2
 from ondewo.nlu import project_statistics_pb2 as ondewo_dot_nlu_dot_project__statistics__pb2
 
 
 class ProjectStatisticsStub(object):
-    """Missing associated documentation comment in .proto file."""
+    """Project Root Statistics
+    """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
@@ -54,63 +55,68 @@
             '/ondewo.nlu.ProjectStatistics/GetEntitySynonymCount',
             request_serializer=ondewo_dot_nlu_dot_project__statistics__pb2.GetProjectElementStatRequest.SerializeToString,
             response_deserializer=ondewo_dot_nlu_dot_common__pb2.StatResponse.FromString,
         )
 
 
 class ProjectStatisticsServicer(object):
-    """Missing associated documentation comment in .proto file."""
+    """Project Root Statistics
+    """
 
     def GetIntentCount(self, request, context):
-        """Project Root Statistics
+        """Returns the intent count within a project
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetEntityTypeCount(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Returns the entity types count within a project
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetUserCount(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Returns the users count within a project
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSessionCount(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Returns the sessions count within a project
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetTrainingPhraseCount(self, request, context):
-        """Intent Statistics
+        """Returns the training phrases count within a project
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetResponseCount(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Returns the responses count within a project
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetEntityValueCount(self, request, context):
-        """Entity Type Statistics
+        """Returns the entity value count within a project
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetEntitySynonymCount(self, request, context):
-        """Entity Value Statistics
+        """Returns the entity synonyms count within a project
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_ProjectStatisticsServicer_to_server(servicer, server):
@@ -160,15 +166,16 @@
         'ondewo.nlu.ProjectStatistics', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
  # This class is part of an EXPERIMENTAL API.
 
 
 class ProjectStatistics(object):
-    """Missing associated documentation comment in .proto file."""
+    """Project Root Statistics
+    """
 
     @staticmethod
     def GetIntentCount(request,
                        target,
                        options=(),
                        channel_credentials=None,
                        call_credentials=None,
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/server_statistics_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/server_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/server_statistics_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/server_statistics_pb2_grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from ondewo.nlu import common_pb2 as ondewo_dot_nlu_dot_common__pb2
 from ondewo.nlu import server_statistics_pb2 as ondewo_dot_nlu_dot_server__statistics__pb2
 
 
 class ServerStatisticsStub(object):
-    """Missing associated documentation comment in .proto file."""
+    """Server project statistics
+    """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
@@ -30,30 +31,34 @@
             '/ondewo.nlu.ServerStatistics/GetUserCount',
             request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             response_deserializer=ondewo_dot_nlu_dot_common__pb2.StatResponse.FromString,
         )
 
 
 class ServerStatisticsServicer(object):
-    """Missing associated documentation comment in .proto file."""
+    """Server project statistics
+    """
 
     def GetProjectCount(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Returns the count of projects in the CAI server
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetUserProjectCount(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Returns the count of projects of a user
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetUserCount(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Returns the users count within a project
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_ServerStatisticsServicer_to_server(servicer, server):
     rpc_method_handlers = {
@@ -77,15 +82,16 @@
         'ondewo.nlu.ServerStatistics', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
  # This class is part of an EXPERIMENTAL API.
 
 
 class ServerStatistics(object):
-    """Missing associated documentation comment in .proto file."""
+    """Server project statistics
+    """
 
     @staticmethod
     def GetProjectCount(request,
                         target,
                         options=(),
                         channel_credentials=None,
                         call_credentials=None,
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/session_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/t2s/text_to_speech_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,422 +1,455 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: ondewo/nlu/session.proto
+# source: ondewo/t2s/text-to-speech.proto
 """Generated protocol buffer code."""
-from ondewo.nlu import entity_type_pb2 as ondewo_dot_nlu_dot_entity__type__pb2
-from ondewo.nlu import intent_pb2 as ondewo_dot_nlu_dot_intent__pb2
-from ondewo.nlu import context_pb2 as ondewo_dot_nlu_dot_context__pb2
-from google.type import latlng_pb2 as google_dot_type_dot_latlng__pb2
-from google.rpc import status_pb2 as google_dot_rpc_dot_status__pb2
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18ondewo/nlu/session.proto\x12\nondewo.nlu\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x17google/rpc/status.proto\x1a\x18google/type/latlng.proto\x1a\x18ondewo/nlu/context.proto\x1a\x17ondewo/nlu/intent.proto\x1a\x1condewo/nlu/entity_type.proto\"\x9b\x01\n\x13\x44\x65tectIntentRequest\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x31\n\x0cquery_params\x18\x02 \x01(\x0b\x32\x1b.ondewo.nlu.QueryParameters\x12+\n\x0bquery_input\x18\x03 \x01(\x0b\x32\x16.ondewo.nlu.QueryInput\x12\x13\n\x0binput_audio\x18\x05 \x01(\x0c\"\x86\x01\n\x14\x44\x65tectIntentResponse\x12\x13\n\x0bresponse_id\x18\x01 \x01(\t\x12-\n\x0cquery_result\x18\x02 \x01(\x0b\x32\x17.ondewo.nlu.QueryResult\x12*\n\x0ewebhook_status\x18\x03 \x01(\x0b\x32\x12.google.rpc.Status\"\xb8\x01\n\x0fQueryParameters\x12\x11\n\ttime_zone\x18\x01 \x01(\t\x12)\n\x0cgeo_location\x18\x02 \x01(\x0b\x32\x13.google.type.LatLng\x12%\n\x08\x63ontexts\x18\x03 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x16\n\x0ereset_contexts\x18\x04 \x01(\x08\x12(\n\x07payload\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\"\x9b\x01\n\nQueryInput\x12\x34\n\x0c\x61udio_config\x18\x01 \x01(\x0b\x32\x1c.ondewo.nlu.InputAudioConfigH\x00\x12%\n\x04text\x18\x02 \x01(\x0b\x32\x15.ondewo.nlu.TextInputH\x00\x12\'\n\x05\x65vent\x18\x03 \x01(\x0b\x32\x16.ondewo.nlu.EventInputH\x00\x42\x07\n\x05input\"\x88\x04\n\x0bQueryResult\x12\x12\n\nquery_text\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x0f \x01(\t\x12%\n\x1dspeech_recognition_confidence\x18\x02 \x01(\x02\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x12+\n\nparameters\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12#\n\x1b\x61ll_required_params_present\x18\x05 \x01(\x08\x12\x18\n\x10\x66ulfillment_text\x18\x06 \x01(\t\x12\x38\n\x14\x66ulfillment_messages\x18\x07 \x03(\x0b\x32\x1a.ondewo.nlu.Intent.Message\x12\x16\n\x0ewebhook_source\x18\x08 \x01(\t\x12\x30\n\x0fwebhook_payload\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12,\n\x0foutput_contexts\x18\n \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\"\n\x06intent\x18\x0b \x01(\x0b\x32\x12.ondewo.nlu.Intent\x12#\n\x1bintent_detection_confidence\x18\x0c \x01(\x02\x12\x30\n\x0f\x64iagnostic_info\x18\x0e \x01(\x0b\x32\x17.google.protobuf.Struct\"\xbe\x01\n\x1cStreamingDetectIntentRequest\x12\x0f\n\x07session\x18\x01 \x01(\t\x12\x31\n\x0cquery_params\x18\x02 \x01(\x0b\x32\x1b.ondewo.nlu.QueryParameters\x12+\n\x0bquery_input\x18\x03 \x01(\x0b\x32\x16.ondewo.nlu.QueryInput\x12\x18\n\x10single_utterance\x18\x04 \x01(\x08\x12\x13\n\x0binput_audio\x18\x06 \x01(\x0c\"\xd3\x01\n\x1dStreamingDetectIntentResponse\x12\x13\n\x0bresponse_id\x18\x01 \x01(\t\x12\x42\n\x12recognition_result\x18\x02 \x01(\x0b\x32&.ondewo.nlu.StreamingRecognitionResult\x12-\n\x0cquery_result\x18\x03 \x01(\x0b\x32\x17.ondewo.nlu.QueryResult\x12*\n\x0ewebhook_status\x18\x04 \x01(\x0b\x32\x12.google.rpc.Status\"\xfa\x01\n\x1aStreamingRecognitionResult\x12H\n\x0cmessage_type\x18\x01 \x01(\x0e\x32\x32.ondewo.nlu.StreamingRecognitionResult.MessageType\x12\x12\n\ntranscript\x18\x02 \x01(\t\x12\x10\n\x08is_final\x18\x03 \x01(\x08\x12\x12\n\nconfidence\x18\x04 \x01(\x02\"X\n\x0bMessageType\x12\x1c\n\x18MESSAGE_TYPE_UNSPECIFIED\x10\x00\x12\x0e\n\nTRANSCRIPT\x10\x01\x12\x1b\n\x17\x45ND_OF_SINGLE_UTTERANCE\x10\x02\"\x8d\x01\n\x10InputAudioConfig\x12\x31\n\x0e\x61udio_encoding\x18\x01 \x01(\x0e\x32\x19.ondewo.nlu.AudioEncoding\x12\x19\n\x11sample_rate_hertz\x18\x02 \x01(\x05\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\x12\x14\n\x0cphrase_hints\x18\x04 \x03(\t\"0\n\tTextInput\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\"^\n\nEventInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\nparameters\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x15\n\rlanguage_code\x18\x03 \x01(\t\"\xba\x01\n\x07Session\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12.\n\rsession_steps\x18\x02 \x03(\x0b\x32\x17.ondewo.nlu.SessionStep\x12-\n\x0csession_info\x18\x03 \x01(\x0b\x32\x17.ondewo.nlu.SessionInfo\"<\n\x04View\x12\x14\n\x10VIEW_UNSPECIFIED\x10\x00\x12\r\n\tVIEW_FULL\x10\x01\x12\x0f\n\x0bVIEW_SPARSE\x10\x02\"\xb6\x01\n\x0bSessionStep\x12>\n\x15\x64\x65tect_intent_request\x18\x01 \x01(\x0b\x32\x1f.ondewo.nlu.DetectIntentRequest\x12@\n\x16\x64\x65tect_intent_response\x18\x02 \x01(\x0b\x32 .ondewo.nlu.DetectIntentResponse\x12%\n\x08\x63ontexts\x18\x03 \x03(\x0b\x32\x13.ondewo.nlu.Context\"\x8c\x01\n\x17TrackSessionStepRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12-\n\x0csession_step\x18\x02 \x01(\x0b\x32\x17.ondewo.nlu.SessionStep\x12.\n\x0csession_view\x18\x03 \x01(\x0e\x32\x18.ondewo.nlu.Session.View\"\x9c\x01\n\x13ListSessionsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12.\n\x0csession_view\x18\x02 \x01(\x0e\x32\x18.ondewo.nlu.Session.View\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x31\n\x0esession_filter\x18\x05 \x01(\x0b\x32\x19.ondewo.nlu.SessionFilter\"\xa1\x04\n\rSessionFilter\x12\x16\n\x0elanguage_codes\x18\x01 \x03(\t\x12+\n\x0fmatched_intents\x18\x02 \x03(\x0b\x32\x12.ondewo.nlu.Intent\x12\x34\n\x14matched_entity_types\x18\x03 \x03(\x0b\x32\x16.ondewo.nlu.EntityType\x12\"\n\x1amin_intents_confidence_min\x18\x04 \x01(\x02\x12\"\n\x1amin_intents_confidence_max\x18\x05 \x01(\x02\x12\'\n\x1fmin_entity_types_confidence_min\x18\x06 \x01(\x02\x12\'\n\x1fmin_entity_types_confidence_max\x18\x07 \x01(\x02\x12\x10\n\x08\x65\x61rliest\x18\x08 \x01(\x02\x12\x0e\n\x06latest\x18\t \x01(\x02\x12\x18\n\x10min_number_turns\x18\n \x01(\x05\x12\x18\n\x10max_number_turns\x18\x0b \x01(\x05\x12\x0e\n\x06labels\x18\x0c \x03(\t\x12\x10\n\x08user_ids\x18\r \x03(\t\x12\x13\n\x0bintent_tags\x18\x0e \x03(\t\x12\x13\n\x0bsession_ids\x18\x0f \x03(\t\x12+\n\x0einput_contexts\x18\x10 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12,\n\x0foutput_contexts\x18\x11 \x03(\x0b\x32\x13.ondewo.nlu.Context\"\xfa\x03\n\x0bSessionInfo\x12\x16\n\x0elanguage_codes\x18\x01 \x03(\t\x12+\n\x0fmatched_intents\x18\x02 \x03(\x0b\x32\x12.ondewo.nlu.Intent\x12\x34\n\x14matched_entity_types\x18\x03 \x03(\x0b\x32\x16.ondewo.nlu.EntityType\x12\x1e\n\x16min_intents_confidence\x18\x04 \x01(\x02\x12#\n\x1bmin_entity_types_confidence\x18\x05 \x01(\x02\x12\x10\n\x08\x65\x61rliest\x18\x06 \x01(\x02\x12\x0e\n\x06latest\x18\x07 \x01(\x02\x12\x14\n\x0cnumber_turns\x18\x08 \x01(\x05\x12\x0e\n\x06labels\x18\t \x03(\t\x12\x10\n\x08user_ids\x18\n \x03(\t\x12\x13\n\x0bintent_tags\x18\x0b \x03(\t\x12\x41\n\x13input_context_steps\x18\x0c \x03(\x0b\x32$.ondewo.nlu.SessionInfo.ContextSteps\x12\x42\n\x14output_context_steps\x18\r \x03(\x0b\x32$.ondewo.nlu.SessionInfo.ContextSteps\x1a\x35\n\x0c\x43ontextSteps\x12%\n\x08\x63ontexts\x18\x01 \x03(\x0b\x32\x13.ondewo.nlu.Context\"V\n\x14ListSessionsResponse\x12%\n\x08sessions\x18\x01 \x03(\x0b\x32\x13.ondewo.nlu.Session\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"W\n\x11GetSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12.\n\x0csession_view\x18\x02 \x01(\x0e\x32\x18.ondewo.nlu.Session.View\"<\n\x14\x43reateSessionRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\x12\x14\n\x0csession_uuid\x18\x02 \x01(\t\"*\n\x14\x44\x65leteSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"\xba\x01\n\x1a\x43reateSessionReviewRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x18\n\x10parent_review_id\x18\x02 \x01(\t\x12\x31\n\x0esession_review\x18\x03 \x01(\x0b\x32\x19.ondewo.nlu.SessionReview\x12;\n\x13session_review_view\x18\x04 \x01(\x0e\x32\x1e.ondewo.nlu.SessionReview.View\"\xa5\x01\n\rSessionReview\x12\x19\n\x11session_review_id\x18\x01 \x01(\t\x12;\n\x14session_review_steps\x18\x02 \x03(\x0b\x32\x1d.ondewo.nlu.SessionReviewStep\"<\n\x04View\x12\x14\n\x10VIEW_UNSPECIFIED\x10\x00\x12\r\n\tVIEW_FULL\x10\x01\x12\x0f\n\x0bVIEW_SPARSE\x10\x02\"\xf1\x01\n\x11SessionReviewStep\x12=\n\x12\x61nnotated_usersays\x18\x01 \x01(\x0b\x32!.ondewo.nlu.Intent.TrainingPhrase\x12\x15\n\rlanguage_code\x18\x02 \x01(\t\x12\x34\n\x10\x64\x65tected_intents\x18\x03 \x03(\x0b\x32\x1a.ondewo.nlu.DetectedIntent\x12%\n\x08\x63ontexts\x18\x04 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12)\n\x0c\x63ontexts_out\x18\x05 \x03(\x0b\x32\x13.ondewo.nlu.Context\"\xb0\x01\n\x0e\x44\x65tectedIntent\x12\"\n\x06intent\x18\x01 \x01(\x0b\x32\x12.ondewo.nlu.Intent\x12\r\n\x05score\x18\x02 \x01(\x02\x12\x11\n\talgorithm\x18\x03 \x01(\t\x12\x38\n\x14\x66ulfillment_messages\x18\x04 \x03(\x0b\x32\x1a.ondewo.nlu.Intent.Message\x12\x1e\n\x16required_param_missing\x18\x05 \x01(\x08\"*\n\x18ListSessionLabelsRequest\x12\x0e\n\x06parent\x18\x01 \x01(\t\"+\n\x19ListSessionLabelsResponse\x12\x0e\n\x06labels\x18\x01 \x03(\t\"m\n\x17\x41\x64\x64SessionLabelsRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0e\n\x06labels\x18\x02 \x03(\t\x12.\n\x0csession_view\x18\x03 \x01(\x0e\x32\x18.ondewo.nlu.Session.View\"p\n\x1aRemoveSessionLabelsRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x0e\n\x06labels\x18\x02 \x03(\t\x12.\n\x0csession_view\x18\x03 \x01(\x0e\x32\x18.ondewo.nlu.Session.View\"\x80\x01\n\x19ListSessionReviewsRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12;\n\x13session_review_view\x18\x02 \x01(\x0e\x32\x1e.ondewo.nlu.SessionReview.View\x12\x12\n\npage_token\x18\x04 \x01(\t\"i\n\x1aListSessionReviewsResponse\x12\x32\n\x0fsession_reviews\x18\x01 \x03(\x0b\x32\x19.ondewo.nlu.SessionReview\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"q\n\x17GetSessionReviewRequest\x12\x19\n\x11session_review_id\x18\x01 \x01(\t\x12;\n\x13session_review_view\x18\x02 \x01(\x0e\x32\x1e.ondewo.nlu.SessionReview.View\"p\n\x1dGetLatestSessionReviewRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12;\n\x13session_review_view\x18\x02 \x01(\x0e\x32\x1e.ondewo.nlu.SessionReview.View*\xfb\x01\n\rAudioEncoding\x12\x1e\n\x1a\x41UDIO_ENCODING_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x41UDIO_ENCODING_LINEAR_16\x10\x01\x12\x17\n\x13\x41UDIO_ENCODING_FLAC\x10\x02\x12\x18\n\x14\x41UDIO_ENCODING_MULAW\x10\x03\x12\x16\n\x12\x41UDIO_ENCODING_AMR\x10\x04\x12\x19\n\x15\x41UDIO_ENCODING_AMR_WB\x10\x05\x12\x1b\n\x17\x41UDIO_ENCODING_OGG_OPUS\x10\x06\x12)\n%AUDIO_ENCODING_SPEEX_WITH_HEADER_BYTE\x10\x07\x32\x8b\x10\n\x08Sessions\x12\x94\x01\n\x0c\x44\x65tectIntent\x12\x1f.ondewo.nlu.DetectIntentRequest\x1a .ondewo.nlu.DetectIntentResponse\"A\x82\xd3\xe4\x93\x02;\"6/v2/{session=projects/*/agent/sessions/*}:detectIntent:\x01*\x12p\n\x15StreamingDetectIntent\x12(.ondewo.nlu.StreamingDetectIntentRequest\x1a).ondewo.nlu.StreamingDetectIntentResponse(\x01\x30\x01\x12\x81\x01\n\x0cListSessions\x12\x1f.ondewo.nlu.ListSessionsRequest\x1a .ondewo.nlu.ListSessionsResponse\".\x82\xd3\xe4\x93\x02(\x12&/v2/{parent=projects/*/agent}/sessions\x12v\n\nGetSession\x12\x1d.ondewo.nlu.GetSessionRequest\x1a\x13.ondewo.nlu.Session\"4\x82\xd3\xe4\x93\x02.\x12,/v2/{session_id=projects/*/agent/sessions/*}\x12y\n\rCreateSession\x12 .ondewo.nlu.CreateSessionRequest\x1a\x13.ondewo.nlu.Session\"1\x82\xd3\xe4\x93\x02+\"&/v2/{parent=projects/*/agent}/sessions:\x01*\x12\x96\x01\n\x10TrackSessionStep\x12#.ondewo.nlu.TrackSessionStepRequest\x1a\x13.ondewo.nlu.Session\"H\x82\xd3\xe4\x93\x02\x42\"=/v2/{session_id=projects/*/agent/sessions/*}:trackSessionStep:\x01*\x12\x7f\n\rDeleteSession\x12 .ondewo.nlu.DeleteSessionRequest\x1a\x16.google.protobuf.Empty\"4\x82\xd3\xe4\x93\x02.*,/v2/{session_id=projects/*/agent/sessions/*}\x12\x97\x01\n\x11ListSessionLabels\x12$.ondewo.nlu.ListSessionLabelsRequest\x1a%.ondewo.nlu.ListSessionLabelsResponse\"5\x82\xd3\xe4\x93\x02/\x12-/v2/{parent=projects/*/agent}/sessions/labels\x12\x90\x01\n\x10\x41\x64\x64SessionLabels\x12#.ondewo.nlu.AddSessionLabelsRequest\x1a\x13.ondewo.nlu.Session\"B\x82\xd3\xe4\x93\x02<\"7/v2/{session_id=projects/*/agent/sessions/*}/labels:add:\x01*\x12\x99\x01\n\x13RemoveSessionLabels\x12&.ondewo.nlu.RemoveSessionLabelsRequest\x1a\x13.ondewo.nlu.Session\"E\x82\xd3\xe4\x93\x02?\":/v2/{session_id=projects/*/agent/sessions/*}/labels:remove:\x01*\x12\xa1\x01\n\x12ListSessionReviews\x12%.ondewo.nlu.ListSessionReviewsRequest\x1a&.ondewo.nlu.ListSessionReviewsResponse\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/v2/{session_id=projects/*/agent/sessions/*}/reviews\x12\x99\x01\n\x10GetSessionReview\x12#.ondewo.nlu.GetSessionReviewRequest\x1a\x19.ondewo.nlu.SessionReview\"E\x82\xd3\xe4\x93\x02?\x12=/v2/{session_review_id=projects/*/agent/sessions/*/reviews/*}\x12\xb3\x01\n\x16GetLatestSessionReview\x12).ondewo.nlu.GetLatestSessionReviewRequest\x1a\x19.ondewo.nlu.SessionReview\"S\x82\xd3\xe4\x93\x02M\x12K/v2/{session_id=projects/*/agent/sessions/*}/reviews:getLatestSessionReview\x12\xa5\x01\n\x13\x43reateSessionReview\x12&.ondewo.nlu.CreateSessionReviewRequest\x1a\x19.ondewo.nlu.SessionReview\"K\x82\xd3\xe4\x93\x02\x45\"@/v2/{session_id=projects/*/agent/sessions/*}:createSessionReview:\x01*B\x9b\x01\n\x1e\x63om.google.cloud.dialogflow.v2B\x0cSessionProtoP\x01ZDgoogle.golang.org/genproto/googleapis/cloud/dialogflow/v2;dialogflow\xf8\x01\x01\xa2\x02\x02\x44\x46\xaa\x02\x1aGoogle.Cloud.Dialogflow.V2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fondewo/t2s/text-to-speech.proto\x12\nondewo.t2s\x1a\x1bgoogle/protobuf/empty.proto\"L\n\x11SynthesizeRequest\x12\x0c\n\x04text\x18\x01 \x01(\t\x12)\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x19.ondewo.t2s.RequestConfig\"N\n\x16\x42\x61tchSynthesizeRequest\x12\x34\n\rbatch_request\x18\x01 \x03(\x0b\x32\x1d.ondewo.t2s.SynthesizeRequest\"Q\n\x17\x42\x61tchSynthesizeResponse\x12\x36\n\x0e\x62\x61tch_response\x18\x01 \x03(\x0b\x32\x1e.ondewo.t2s.SynthesizeResponse\"\xf3\x02\n\rRequestConfig\x12\x17\n\x0ft2s_pipeline_id\x18\x01 \x01(\t\x12\x16\n\x0clength_scale\x18\x02 \x01(\x02H\x00\x12\x15\n\x0bnoise_scale\x18\x03 \x01(\x02H\x01\x12\x15\n\x0bsample_rate\x18\x04 \x01(\x05H\x02\x12\x1e\n\x03pcm\x18\x05 \x01(\x0e\x32\x0f.ondewo.t2s.PcmH\x03\x12/\n\x0c\x61udio_format\x18\x06 \x01(\x0e\x32\x17.ondewo.t2s.AudioFormatH\x04\x12\x13\n\tuse_cache\x18\x07 \x01(\x08H\x05\x12\x14\n\nnormalizer\x18\x08 \x01(\tH\x06\x42\x14\n\x12oneof_length_scaleB\x13\n\x11oneof_noise_scaleB\x13\n\x11oneof_sample_rateB\x0b\n\toneof_PcmB\x13\n\x11oneof_AudioFormatB\x11\n\x0foneof_use_cacheB\x12\n\x10oneof_normalizer\"\xb8\x01\n\x12SynthesizeResponse\x12\x12\n\naudio_uuid\x18\x01 \x01(\t\x12\r\n\x05\x61udio\x18\x02 \x01(\x0c\x12\x17\n\x0fgeneration_time\x18\x03 \x01(\x02\x12\x14\n\x0c\x61udio_length\x18\x04 \x01(\x02\x12\x0c\n\x04text\x18\x05 \x01(\t\x12)\n\x06\x63onfig\x18\x06 \x01(\x0b\x32\x19.ondewo.t2s.RequestConfig\x12\x17\n\x0fnormalized_text\x18\x07 \x01(\t\"=\n\x14NormalizeTextRequest\x12\x17\n\x0ft2s_pipeline_id\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\"0\n\x15NormalizeTextResponse\x12\x17\n\x0fnormalized_text\x18\x01 \x01(\t\",\n\x19T2SGetServiceInfoResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"\x84\x01\n\x17ListT2sPipelinesRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x15\n\rspeaker_sexes\x18\x02 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x03 \x03(\t\x12\x15\n\rspeaker_names\x18\x04 \x03(\t\x12\x0f\n\x07\x64omains\x18\x05 \x03(\t\"L\n\x18ListT2sPipelinesResponse\x12\x30\n\tpipelines\x18\x01 \x03(\x0b\x32\x1d.ondewo.t2s.Text2SpeechConfig\"q\n\x17ListT2sLanguagesRequest\x12\x15\n\rspeaker_sexes\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\x12\x15\n\rspeaker_names\x18\x03 \x03(\t\x12\x0f\n\x07\x64omains\x18\x04 \x03(\t\"-\n\x18ListT2sLanguagesResponse\x12\x11\n\tlanguages\x18\x01 \x03(\t\"q\n\x15ListT2sDomainsRequest\x12\x15\n\rspeaker_sexes\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\x12\x15\n\rspeaker_names\x18\x03 \x03(\t\x12\x11\n\tlanguages\x18\x04 \x03(\t\")\n\x16ListT2sDomainsResponse\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\"\x1b\n\rT2sPipelineId\x12\n\n\x02id\x18\x01 \x01(\t\"\xf6\x01\n\x11Text2SpeechConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12/\n\x0b\x64\x65scription\x18\x02 \x01(\x0b\x32\x1a.ondewo.t2s.T2SDescription\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\x12+\n\tinference\x18\x04 \x01(\x0b\x32\x18.ondewo.t2s.T2SInference\x12\x33\n\rnormalization\x18\x05 \x01(\x0b\x32\x1c.ondewo.t2s.T2SNormalization\x12\x32\n\x0epostprocessing\x18\x06 \x01(\x0b\x32\x1a.ondewo.t2s.Postprocessing\"\x87\x01\n\x0eT2SDescription\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x13\n\x0bspeaker_sex\x18\x02 \x01(\t\x12\x16\n\x0epipeline_owner\x18\x03 \x01(\t\x12\x10\n\x08\x63omments\x18\x04 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x05 \x01(\t\x12\x0e\n\x06\x64omain\x18\x06 \x01(\t\"\x7f\n\x0cT2SInference\x12\x0c\n\x04type\x18\x01 \x01(\t\x12;\n\x13\x63omposite_inference\x18\x02 \x01(\x0b\x32\x1e.ondewo.t2s.CompositeInference\x12$\n\x07\x63\x61\x63hing\x18\x03 \x01(\x0b\x32\x13.ondewo.t2s.Caching\"f\n\x12\x43ompositeInference\x12&\n\x08text2mel\x18\x01 \x01(\x0b\x32\x14.ondewo.t2s.Text2Mel\x12(\n\tmel2audio\x18\x02 \x01(\x0b\x32\x15.ondewo.t2s.Mel2Audio\"s\n\x08Text2Mel\x12\x0c\n\x04type\x18\x01 \x01(\t\x12%\n\x08glow_tts\x18\x02 \x01(\x0b\x32\x13.ondewo.t2s.GlowTTS\x12\x32\n\x0fglow_tts_triton\x18\x03 \x01(\x0b\x32\x19.ondewo.t2s.GlowTTSTriton\"\x94\x01\n\x07GlowTTS\x12\x12\n\nbatch_size\x18\x01 \x01(\x03\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\x12\x14\n\x0clength_scale\x18\x03 \x01(\x02\x12\x13\n\x0bnoise_scale\x18\x04 \x01(\x02\x12\x0c\n\x04path\x18\x05 \x01(\t\x12\x10\n\x08\x63leaners\x18\x06 \x03(\t\x12\x19\n\x11param_config_path\x18\x07 \x01(\t\"\xaf\x01\n\rGlowTTSTriton\x12\x12\n\nbatch_size\x18\x01 \x01(\x03\x12\x14\n\x0clength_scale\x18\x02 \x01(\x02\x12\x13\n\x0bnoise_scale\x18\x03 \x01(\x02\x12\x10\n\x08\x63leaners\x18\x04 \x03(\t\x12\x17\n\x0fmax_text_length\x18\x05 \x01(\x03\x12\x19\n\x11param_config_path\x18\x06 \x01(\t\x12\x19\n\x11triton_model_name\x18\x07 \x01(\t\"\xaa\x01\n\tMel2Audio\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x34\n\x10mb_melgan_triton\x18\x02 \x01(\x0b\x32\x1a.ondewo.t2s.MbMelganTriton\x12%\n\x08hifi_gan\x18\x03 \x01(\x0b\x32\x13.ondewo.t2s.HiFiGan\x12\x32\n\x0fhifi_gan_triton\x18\x04 \x01(\x0b\x32\x19.ondewo.t2s.HiFiGanTriton\"W\n\x07HiFiGan\x12\x0f\n\x07use_gpu\x18\x01 \x01(\x08\x12\x12\n\nbatch_size\x18\x02 \x01(\x03\x12\x13\n\x0b\x63onfig_path\x18\x03 \x01(\t\x12\x12\n\nmodel_path\x18\x04 \x01(\t\"?\n\rHiFiGanTriton\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\"h\n\x0eMbMelganTriton\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x12\n\nstats_path\x18\x02 \x01(\t\x12\x19\n\x11triton_model_name\x18\x03 \x01(\t\x12\x12\n\ntriton_url\x18\x04 \x01(\t\"\x8f\x01\n\x07\x43\x61\x63hing\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x08\x12\x1d\n\x15memory_cache_max_size\x18\x02 \x01(\x03\x12\x15\n\rsampling_rate\x18\x03 \x01(\x03\x12\x12\n\nload_cache\x18\x04 \x01(\x08\x12\x12\n\nsave_cache\x18\x05 \x01(\x08\x12\x16\n\x0e\x63\x61\x63he_save_dir\x18\x06 \x01(\t\"\xe2\x01\n\x10T2SNormalization\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x10\n\x08pipeline\x18\x02 \x03(\t\x12\x1c\n\x14\x63ustom_phonemizer_id\x18\x03 \x01(\t\x12?\n\x14\x63ustom_length_scales\x18\x04 \x01(\x0b\x32!.ondewo.t2s.T2SCustomLengthScales\x12\x17\n\x0f\x61rpabet_mapping\x18\x05 \x01(\t\x12\x17\n\x0fnumeric_mapping\x18\x06 \x01(\t\x12\x19\n\x11\x63\x61llsigns_mapping\x18\x07 \x01(\t\"\xb0\x01\n\x0ePostprocessing\x12\x14\n\x0csilence_secs\x18\x01 \x01(\x02\x12\x10\n\x08pipeline\x18\x02 \x03(\t\x12$\n\x07logmmse\x18\x03 \x01(\x0b\x32\x13.ondewo.t2s.Logmnse\x12\"\n\x06wiener\x18\x04 \x01(\x0b\x32\x12.ondewo.t2s.Wiener\x12,\n\x0b\x61podization\x18\x05 \x01(\x0b\x32\x17.ondewo.t2s.Apodization\"N\n\x07Logmnse\x12\x15\n\rinitial_noise\x18\x01 \x01(\x03\x12\x13\n\x0bwindow_size\x18\x02 \x01(\x03\x12\x17\n\x0fnoise_threshold\x18\x03 \x01(\x02\"a\n\x06Wiener\x12\x11\n\tframe_len\x18\x01 \x01(\x03\x12\x11\n\tlpc_order\x18\x02 \x01(\x03\x12\x12\n\niterations\x18\x03 \x01(\x03\x12\r\n\x05\x61lpha\x18\x04 \x01(\x02\x12\x0e\n\x06thresh\x18\x05 \x01(\x02\"\'\n\x0b\x41podization\x12\x18\n\x10\x61podization_secs\x18\x01 \x01(\x02\"\xa8\x01\n\x15T2SCustomLengthScales\x12\x0c\n\x04text\x18\x01 \x01(\x02\x12\r\n\x05\x65mail\x18\x02 \x01(\x02\x12\x0b\n\x03url\x18\x03 \x01(\x02\x12\r\n\x05phone\x18\x04 \x01(\x02\x12\r\n\x05spell\x18\x05 \x01(\x02\x12\x18\n\x10spell_with_names\x18\x06 \x01(\x02\x12\x15\n\rcallsign_long\x18\x07 \x01(\x02\x12\x16\n\x0e\x63\x61llsign_short\x18\x08 \x01(\x02\"\x1a\n\x0cPhonemizerId\x12\n\n\x02id\x18\x01 \x01(\t\"B\n\x15\x43ustomPhonemizerProto\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1d\n\x04maps\x18\x02 \x03(\x0b\x32\x0f.ondewo.t2s.Map\"+\n\x03Map\x12\x0c\n\x04word\x18\x01 \x01(\t\x12\x16\n\x0ephoneme_groups\x18\x02 \x01(\t\"V\n\x1cListCustomPhonemizerResponse\x12\x36\n\x0bphonemizers\x18\x01 \x03(\x0b\x32!.ondewo.t2s.CustomPhonemizerProto\"3\n\x1bListCustomPhonemizerRequest\x12\x14\n\x0cpipeline_ids\x18\x01 \x03(\t\"\xd8\x01\n\x1dUpdateCustomPhonemizerRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12M\n\rupdate_method\x18\x02 \x01(\x0e\x32\x36.ondewo.t2s.UpdateCustomPhonemizerRequest.UpdateMethod\x12\x1d\n\x04maps\x18\x03 \x03(\x0b\x32\x0f.ondewo.t2s.Map\"=\n\x0cUpdateMethod\x12\x0f\n\x0b\x65xtend_hard\x10\x00\x12\x0f\n\x0b\x65xtend_soft\x10\x01\x12\x0b\n\x07replace\x10\x02\"N\n\x1d\x43reateCustomPhonemizerRequest\x12\x0e\n\x06prefix\x18\x01 \x01(\t\x12\x1d\n\x04maps\x18\x02 \x03(\x0b\x32\x0f.ondewo.t2s.Map*X\n\x03Pcm\x12\n\n\x06PCM_16\x10\x00\x12\n\n\x06PCM_24\x10\x01\x12\n\n\x06PCM_32\x10\x02\x12\n\n\x06PCM_S8\x10\x03\x12\n\n\x06PCM_U8\x10\x04\x12\t\n\x05\x46LOAT\x10\x05\x12\n\n\x06\x44OUBLE\x10\x06*M\n\x0b\x41udioFormat\x12\x07\n\x03wav\x10\x00\x12\x08\n\x04\x66lac\x10\x01\x12\x07\n\x03\x63\x61\x66\x10\x02\x12\x07\n\x03mp3\x10\x03\x12\x07\n\x03\x61\x61\x63\x10\x04\x12\x07\n\x03ogg\x10\x05\x12\x07\n\x03wma\x10\x06\x32\xb9\x07\n\x0bText2Speech\x12M\n\nSynthesize\x12\x1d.ondewo.t2s.SynthesizeRequest\x1a\x1e.ondewo.t2s.SynthesizeResponse\"\x00\x12\\\n\x0f\x42\x61tchSynthesize\x12\".ondewo.t2s.BatchSynthesizeRequest\x1a#.ondewo.t2s.BatchSynthesizeResponse\"\x00\x12V\n\rNormalizeText\x12 .ondewo.t2s.NormalizeTextRequest\x1a!.ondewo.t2s.NormalizeTextResponse\"\x00\x12L\n\x0eGetT2sPipeline\x12\x19.ondewo.t2s.T2sPipelineId\x1a\x1d.ondewo.t2s.Text2SpeechConfig\"\x00\x12O\n\x11\x43reateT2sPipeline\x12\x1d.ondewo.t2s.Text2SpeechConfig\x1a\x19.ondewo.t2s.T2sPipelineId\"\x00\x12H\n\x11\x44\x65leteT2sPipeline\x12\x19.ondewo.t2s.T2sPipelineId\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x11UpdateT2sPipeline\x12\x1d.ondewo.t2s.Text2SpeechConfig\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x10ListT2sPipelines\x12#.ondewo.t2s.ListT2sPipelinesRequest\x1a$.ondewo.t2s.ListT2sPipelinesResponse\"\x00\x12_\n\x10ListT2sLanguages\x12#.ondewo.t2s.ListT2sLanguagesRequest\x1a$.ondewo.t2s.ListT2sLanguagesResponse\"\x00\x12Y\n\x0eListT2sDomains\x12!.ondewo.t2s.ListT2sDomainsRequest\x1a\".ondewo.t2s.ListT2sDomainsResponse\"\x00\x12Q\n\x0eGetServiceInfo\x12\x16.google.protobuf.Empty\x1a%.ondewo.t2s.T2SGetServiceInfoResponse\"\x00\x32\xef\x03\n\x11\x43ustomPhonemizers\x12T\n\x13GetCustomPhonemizer\x12\x18.ondewo.t2s.PhonemizerId\x1a!.ondewo.t2s.CustomPhonemizerProto\"\x00\x12_\n\x16\x43reateCustomPhonemizer\x12).ondewo.t2s.CreateCustomPhonemizerRequest\x1a\x18.ondewo.t2s.PhonemizerId\"\x00\x12L\n\x16\x44\x65leteCustomPhonemizer\x12\x18.ondewo.t2s.PhonemizerId\x1a\x16.google.protobuf.Empty\"\x00\x12h\n\x16UpdateCustomPhonemizer\x12).ondewo.t2s.UpdateCustomPhonemizerRequest\x1a!.ondewo.t2s.CustomPhonemizerProto\"\x00\x12k\n\x14ListCustomPhonemizer\x12\'.ondewo.t2s.ListCustomPhonemizerRequest\x1a(.ondewo.t2s.ListCustomPhonemizerResponse\"\x00\x62\x06proto3')
 
-_AUDIOENCODING = DESCRIPTOR.enum_types_by_name['AudioEncoding']
-AudioEncoding = enum_type_wrapper.EnumTypeWrapper(_AUDIOENCODING)
-AUDIO_ENCODING_UNSPECIFIED = 0
-AUDIO_ENCODING_LINEAR_16 = 1
-AUDIO_ENCODING_FLAC = 2
-AUDIO_ENCODING_MULAW = 3
-AUDIO_ENCODING_AMR = 4
-AUDIO_ENCODING_AMR_WB = 5
-AUDIO_ENCODING_OGG_OPUS = 6
-AUDIO_ENCODING_SPEEX_WITH_HEADER_BYTE = 7
-
-
-_DETECTINTENTREQUEST = DESCRIPTOR.message_types_by_name['DetectIntentRequest']
-_DETECTINTENTRESPONSE = DESCRIPTOR.message_types_by_name['DetectIntentResponse']
-_QUERYPARAMETERS = DESCRIPTOR.message_types_by_name['QueryParameters']
-_QUERYINPUT = DESCRIPTOR.message_types_by_name['QueryInput']
-_QUERYRESULT = DESCRIPTOR.message_types_by_name['QueryResult']
-_STREAMINGDETECTINTENTREQUEST = DESCRIPTOR.message_types_by_name['StreamingDetectIntentRequest']
-_STREAMINGDETECTINTENTRESPONSE = DESCRIPTOR.message_types_by_name['StreamingDetectIntentResponse']
-_STREAMINGRECOGNITIONRESULT = DESCRIPTOR.message_types_by_name['StreamingRecognitionResult']
-_INPUTAUDIOCONFIG = DESCRIPTOR.message_types_by_name['InputAudioConfig']
-_TEXTINPUT = DESCRIPTOR.message_types_by_name['TextInput']
-_EVENTINPUT = DESCRIPTOR.message_types_by_name['EventInput']
-_SESSION = DESCRIPTOR.message_types_by_name['Session']
-_SESSIONSTEP = DESCRIPTOR.message_types_by_name['SessionStep']
-_TRACKSESSIONSTEPREQUEST = DESCRIPTOR.message_types_by_name['TrackSessionStepRequest']
-_LISTSESSIONSREQUEST = DESCRIPTOR.message_types_by_name['ListSessionsRequest']
-_SESSIONFILTER = DESCRIPTOR.message_types_by_name['SessionFilter']
-_SESSIONINFO = DESCRIPTOR.message_types_by_name['SessionInfo']
-_SESSIONINFO_CONTEXTSTEPS = _SESSIONINFO.nested_types_by_name['ContextSteps']
-_LISTSESSIONSRESPONSE = DESCRIPTOR.message_types_by_name['ListSessionsResponse']
-_GETSESSIONREQUEST = DESCRIPTOR.message_types_by_name['GetSessionRequest']
-_CREATESESSIONREQUEST = DESCRIPTOR.message_types_by_name['CreateSessionRequest']
-_DELETESESSIONREQUEST = DESCRIPTOR.message_types_by_name['DeleteSessionRequest']
-_CREATESESSIONREVIEWREQUEST = DESCRIPTOR.message_types_by_name['CreateSessionReviewRequest']
-_SESSIONREVIEW = DESCRIPTOR.message_types_by_name['SessionReview']
-_SESSIONREVIEWSTEP = DESCRIPTOR.message_types_by_name['SessionReviewStep']
-_DETECTEDINTENT = DESCRIPTOR.message_types_by_name['DetectedIntent']
-_LISTSESSIONLABELSREQUEST = DESCRIPTOR.message_types_by_name['ListSessionLabelsRequest']
-_LISTSESSIONLABELSRESPONSE = DESCRIPTOR.message_types_by_name['ListSessionLabelsResponse']
-_ADDSESSIONLABELSREQUEST = DESCRIPTOR.message_types_by_name['AddSessionLabelsRequest']
-_REMOVESESSIONLABELSREQUEST = DESCRIPTOR.message_types_by_name['RemoveSessionLabelsRequest']
-_LISTSESSIONREVIEWSREQUEST = DESCRIPTOR.message_types_by_name['ListSessionReviewsRequest']
-_LISTSESSIONREVIEWSRESPONSE = DESCRIPTOR.message_types_by_name['ListSessionReviewsResponse']
-_GETSESSIONREVIEWREQUEST = DESCRIPTOR.message_types_by_name['GetSessionReviewRequest']
-_GETLATESTSESSIONREVIEWREQUEST = DESCRIPTOR.message_types_by_name['GetLatestSessionReviewRequest']
-_STREAMINGRECOGNITIONRESULT_MESSAGETYPE = _STREAMINGRECOGNITIONRESULT.enum_types_by_name['MessageType']
-_SESSION_VIEW = _SESSION.enum_types_by_name['View']
-_SESSIONREVIEW_VIEW = _SESSIONREVIEW.enum_types_by_name['View']
-DetectIntentRequest = _reflection.GeneratedProtocolMessageType('DetectIntentRequest', (_message.Message,), {
-    'DESCRIPTOR': _DETECTINTENTREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.DetectIntentRequest)
-})
-_sym_db.RegisterMessage(DetectIntentRequest)
-
-DetectIntentResponse = _reflection.GeneratedProtocolMessageType('DetectIntentResponse', (_message.Message,), {
-    'DESCRIPTOR': _DETECTINTENTRESPONSE,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.DetectIntentResponse)
-})
-_sym_db.RegisterMessage(DetectIntentResponse)
-
-QueryParameters = _reflection.GeneratedProtocolMessageType('QueryParameters', (_message.Message,), {
-    'DESCRIPTOR': _QUERYPARAMETERS,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.QueryParameters)
-})
-_sym_db.RegisterMessage(QueryParameters)
-
-QueryInput = _reflection.GeneratedProtocolMessageType('QueryInput', (_message.Message,), {
-    'DESCRIPTOR': _QUERYINPUT,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.QueryInput)
-})
-_sym_db.RegisterMessage(QueryInput)
-
-QueryResult = _reflection.GeneratedProtocolMessageType('QueryResult', (_message.Message,), {
-    'DESCRIPTOR': _QUERYRESULT,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.QueryResult)
-})
-_sym_db.RegisterMessage(QueryResult)
-
-StreamingDetectIntentRequest = _reflection.GeneratedProtocolMessageType('StreamingDetectIntentRequest', (_message.Message,), {
-    'DESCRIPTOR': _STREAMINGDETECTINTENTREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.StreamingDetectIntentRequest)
-})
-_sym_db.RegisterMessage(StreamingDetectIntentRequest)
-
-StreamingDetectIntentResponse = _reflection.GeneratedProtocolMessageType('StreamingDetectIntentResponse', (_message.Message,), {
-    'DESCRIPTOR': _STREAMINGDETECTINTENTRESPONSE,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.StreamingDetectIntentResponse)
-})
-_sym_db.RegisterMessage(StreamingDetectIntentResponse)
-
-StreamingRecognitionResult = _reflection.GeneratedProtocolMessageType('StreamingRecognitionResult', (_message.Message,), {
-    'DESCRIPTOR': _STREAMINGRECOGNITIONRESULT,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.StreamingRecognitionResult)
-})
-_sym_db.RegisterMessage(StreamingRecognitionResult)
-
-InputAudioConfig = _reflection.GeneratedProtocolMessageType('InputAudioConfig', (_message.Message,), {
-    'DESCRIPTOR': _INPUTAUDIOCONFIG,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.InputAudioConfig)
-})
-_sym_db.RegisterMessage(InputAudioConfig)
-
-TextInput = _reflection.GeneratedProtocolMessageType('TextInput', (_message.Message,), {
-    'DESCRIPTOR': _TEXTINPUT,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.TextInput)
-})
-_sym_db.RegisterMessage(TextInput)
-
-EventInput = _reflection.GeneratedProtocolMessageType('EventInput', (_message.Message,), {
-    'DESCRIPTOR': _EVENTINPUT,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.EventInput)
-})
-_sym_db.RegisterMessage(EventInput)
-
-Session = _reflection.GeneratedProtocolMessageType('Session', (_message.Message,), {
-    'DESCRIPTOR': _SESSION,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.Session)
-})
-_sym_db.RegisterMessage(Session)
-
-SessionStep = _reflection.GeneratedProtocolMessageType('SessionStep', (_message.Message,), {
-    'DESCRIPTOR': _SESSIONSTEP,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.SessionStep)
-})
-_sym_db.RegisterMessage(SessionStep)
-
-TrackSessionStepRequest = _reflection.GeneratedProtocolMessageType('TrackSessionStepRequest', (_message.Message,), {
-    'DESCRIPTOR': _TRACKSESSIONSTEPREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.TrackSessionStepRequest)
-})
-_sym_db.RegisterMessage(TrackSessionStepRequest)
-
-ListSessionsRequest = _reflection.GeneratedProtocolMessageType('ListSessionsRequest', (_message.Message,), {
-    'DESCRIPTOR': _LISTSESSIONSREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.ListSessionsRequest)
-})
-_sym_db.RegisterMessage(ListSessionsRequest)
-
-SessionFilter = _reflection.GeneratedProtocolMessageType('SessionFilter', (_message.Message,), {
-    'DESCRIPTOR': _SESSIONFILTER,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.SessionFilter)
-})
-_sym_db.RegisterMessage(SessionFilter)
-
-SessionInfo = _reflection.GeneratedProtocolMessageType('SessionInfo', (_message.Message,), {
-
-    'ContextSteps': _reflection.GeneratedProtocolMessageType('ContextSteps', (_message.Message,), {
-        'DESCRIPTOR': _SESSIONINFO_CONTEXTSTEPS,
-        '__module__': 'ondewo.nlu.session_pb2'
-        # @@protoc_insertion_point(class_scope:ondewo.nlu.SessionInfo.ContextSteps)
-    }),
-    'DESCRIPTOR': _SESSIONINFO,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.SessionInfo)
-})
-_sym_db.RegisterMessage(SessionInfo)
-_sym_db.RegisterMessage(SessionInfo.ContextSteps)
-
-ListSessionsResponse = _reflection.GeneratedProtocolMessageType('ListSessionsResponse', (_message.Message,), {
-    'DESCRIPTOR': _LISTSESSIONSRESPONSE,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.ListSessionsResponse)
-})
-_sym_db.RegisterMessage(ListSessionsResponse)
-
-GetSessionRequest = _reflection.GeneratedProtocolMessageType('GetSessionRequest', (_message.Message,), {
-    'DESCRIPTOR': _GETSESSIONREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.GetSessionRequest)
-})
-_sym_db.RegisterMessage(GetSessionRequest)
-
-CreateSessionRequest = _reflection.GeneratedProtocolMessageType('CreateSessionRequest', (_message.Message,), {
-    'DESCRIPTOR': _CREATESESSIONREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.CreateSessionRequest)
-})
-_sym_db.RegisterMessage(CreateSessionRequest)
-
-DeleteSessionRequest = _reflection.GeneratedProtocolMessageType('DeleteSessionRequest', (_message.Message,), {
-    'DESCRIPTOR': _DELETESESSIONREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.DeleteSessionRequest)
-})
-_sym_db.RegisterMessage(DeleteSessionRequest)
-
-CreateSessionReviewRequest = _reflection.GeneratedProtocolMessageType('CreateSessionReviewRequest', (_message.Message,), {
-    'DESCRIPTOR': _CREATESESSIONREVIEWREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.CreateSessionReviewRequest)
-})
-_sym_db.RegisterMessage(CreateSessionReviewRequest)
-
-SessionReview = _reflection.GeneratedProtocolMessageType('SessionReview', (_message.Message,), {
-    'DESCRIPTOR': _SESSIONREVIEW,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.SessionReview)
-})
-_sym_db.RegisterMessage(SessionReview)
-
-SessionReviewStep = _reflection.GeneratedProtocolMessageType('SessionReviewStep', (_message.Message,), {
-    'DESCRIPTOR': _SESSIONREVIEWSTEP,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.SessionReviewStep)
-})
-_sym_db.RegisterMessage(SessionReviewStep)
-
-DetectedIntent = _reflection.GeneratedProtocolMessageType('DetectedIntent', (_message.Message,), {
-    'DESCRIPTOR': _DETECTEDINTENT,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.DetectedIntent)
-})
-_sym_db.RegisterMessage(DetectedIntent)
-
-ListSessionLabelsRequest = _reflection.GeneratedProtocolMessageType('ListSessionLabelsRequest', (_message.Message,), {
-    'DESCRIPTOR': _LISTSESSIONLABELSREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.ListSessionLabelsRequest)
-})
-_sym_db.RegisterMessage(ListSessionLabelsRequest)
-
-ListSessionLabelsResponse = _reflection.GeneratedProtocolMessageType('ListSessionLabelsResponse', (_message.Message,), {
-    'DESCRIPTOR': _LISTSESSIONLABELSRESPONSE,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.ListSessionLabelsResponse)
-})
-_sym_db.RegisterMessage(ListSessionLabelsResponse)
-
-AddSessionLabelsRequest = _reflection.GeneratedProtocolMessageType('AddSessionLabelsRequest', (_message.Message,), {
-    'DESCRIPTOR': _ADDSESSIONLABELSREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.AddSessionLabelsRequest)
-})
-_sym_db.RegisterMessage(AddSessionLabelsRequest)
-
-RemoveSessionLabelsRequest = _reflection.GeneratedProtocolMessageType('RemoveSessionLabelsRequest', (_message.Message,), {
-    'DESCRIPTOR': _REMOVESESSIONLABELSREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.RemoveSessionLabelsRequest)
-})
-_sym_db.RegisterMessage(RemoveSessionLabelsRequest)
-
-ListSessionReviewsRequest = _reflection.GeneratedProtocolMessageType('ListSessionReviewsRequest', (_message.Message,), {
-    'DESCRIPTOR': _LISTSESSIONREVIEWSREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.ListSessionReviewsRequest)
-})
-_sym_db.RegisterMessage(ListSessionReviewsRequest)
-
-ListSessionReviewsResponse = _reflection.GeneratedProtocolMessageType('ListSessionReviewsResponse', (_message.Message,), {
-    'DESCRIPTOR': _LISTSESSIONREVIEWSRESPONSE,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.ListSessionReviewsResponse)
-})
-_sym_db.RegisterMessage(ListSessionReviewsResponse)
-
-GetSessionReviewRequest = _reflection.GeneratedProtocolMessageType('GetSessionReviewRequest', (_message.Message,), {
-    'DESCRIPTOR': _GETSESSIONREVIEWREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.GetSessionReviewRequest)
-})
-_sym_db.RegisterMessage(GetSessionReviewRequest)
-
-GetLatestSessionReviewRequest = _reflection.GeneratedProtocolMessageType('GetLatestSessionReviewRequest', (_message.Message,), {
-    'DESCRIPTOR': _GETLATESTSESSIONREVIEWREQUEST,
-    '__module__': 'ondewo.nlu.session_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.nlu.GetLatestSessionReviewRequest)
+_PCM = DESCRIPTOR.enum_types_by_name['Pcm']
+Pcm = enum_type_wrapper.EnumTypeWrapper(_PCM)
+_AUDIOFORMAT = DESCRIPTOR.enum_types_by_name['AudioFormat']
+AudioFormat = enum_type_wrapper.EnumTypeWrapper(_AUDIOFORMAT)
+PCM_16 = 0
+PCM_24 = 1
+PCM_32 = 2
+PCM_S8 = 3
+PCM_U8 = 4
+FLOAT = 5
+DOUBLE = 6
+wav = 0
+flac = 1
+caf = 2
+mp3 = 3
+aac = 4
+ogg = 5
+wma = 6
+
+
+_SYNTHESIZEREQUEST = DESCRIPTOR.message_types_by_name['SynthesizeRequest']
+_BATCHSYNTHESIZEREQUEST = DESCRIPTOR.message_types_by_name['BatchSynthesizeRequest']
+_BATCHSYNTHESIZERESPONSE = DESCRIPTOR.message_types_by_name['BatchSynthesizeResponse']
+_REQUESTCONFIG = DESCRIPTOR.message_types_by_name['RequestConfig']
+_SYNTHESIZERESPONSE = DESCRIPTOR.message_types_by_name['SynthesizeResponse']
+_NORMALIZETEXTREQUEST = DESCRIPTOR.message_types_by_name['NormalizeTextRequest']
+_NORMALIZETEXTRESPONSE = DESCRIPTOR.message_types_by_name['NormalizeTextResponse']
+_T2SGETSERVICEINFORESPONSE = DESCRIPTOR.message_types_by_name['T2SGetServiceInfoResponse']
+_LISTT2SPIPELINESREQUEST = DESCRIPTOR.message_types_by_name['ListT2sPipelinesRequest']
+_LISTT2SPIPELINESRESPONSE = DESCRIPTOR.message_types_by_name['ListT2sPipelinesResponse']
+_LISTT2SLANGUAGESREQUEST = DESCRIPTOR.message_types_by_name['ListT2sLanguagesRequest']
+_LISTT2SLANGUAGESRESPONSE = DESCRIPTOR.message_types_by_name['ListT2sLanguagesResponse']
+_LISTT2SDOMAINSREQUEST = DESCRIPTOR.message_types_by_name['ListT2sDomainsRequest']
+_LISTT2SDOMAINSRESPONSE = DESCRIPTOR.message_types_by_name['ListT2sDomainsResponse']
+_T2SPIPELINEID = DESCRIPTOR.message_types_by_name['T2sPipelineId']
+_TEXT2SPEECHCONFIG = DESCRIPTOR.message_types_by_name['Text2SpeechConfig']
+_T2SDESCRIPTION = DESCRIPTOR.message_types_by_name['T2SDescription']
+_T2SINFERENCE = DESCRIPTOR.message_types_by_name['T2SInference']
+_COMPOSITEINFERENCE = DESCRIPTOR.message_types_by_name['CompositeInference']
+_TEXT2MEL = DESCRIPTOR.message_types_by_name['Text2Mel']
+_GLOWTTS = DESCRIPTOR.message_types_by_name['GlowTTS']
+_GLOWTTSTRITON = DESCRIPTOR.message_types_by_name['GlowTTSTriton']
+_MEL2AUDIO = DESCRIPTOR.message_types_by_name['Mel2Audio']
+_HIFIGAN = DESCRIPTOR.message_types_by_name['HiFiGan']
+_HIFIGANTRITON = DESCRIPTOR.message_types_by_name['HiFiGanTriton']
+_MBMELGANTRITON = DESCRIPTOR.message_types_by_name['MbMelganTriton']
+_CACHING = DESCRIPTOR.message_types_by_name['Caching']
+_T2SNORMALIZATION = DESCRIPTOR.message_types_by_name['T2SNormalization']
+_POSTPROCESSING = DESCRIPTOR.message_types_by_name['Postprocessing']
+_LOGMNSE = DESCRIPTOR.message_types_by_name['Logmnse']
+_WIENER = DESCRIPTOR.message_types_by_name['Wiener']
+_APODIZATION = DESCRIPTOR.message_types_by_name['Apodization']
+_T2SCUSTOMLENGTHSCALES = DESCRIPTOR.message_types_by_name['T2SCustomLengthScales']
+_PHONEMIZERID = DESCRIPTOR.message_types_by_name['PhonemizerId']
+_CUSTOMPHONEMIZERPROTO = DESCRIPTOR.message_types_by_name['CustomPhonemizerProto']
+_MAP = DESCRIPTOR.message_types_by_name['Map']
+_LISTCUSTOMPHONEMIZERRESPONSE = DESCRIPTOR.message_types_by_name['ListCustomPhonemizerResponse']
+_LISTCUSTOMPHONEMIZERREQUEST = DESCRIPTOR.message_types_by_name['ListCustomPhonemizerRequest']
+_UPDATECUSTOMPHONEMIZERREQUEST = DESCRIPTOR.message_types_by_name['UpdateCustomPhonemizerRequest']
+_CREATECUSTOMPHONEMIZERREQUEST = DESCRIPTOR.message_types_by_name['CreateCustomPhonemizerRequest']
+_UPDATECUSTOMPHONEMIZERREQUEST_UPDATEMETHOD = _UPDATECUSTOMPHONEMIZERREQUEST.enum_types_by_name['UpdateMethod']
+SynthesizeRequest = _reflection.GeneratedProtocolMessageType('SynthesizeRequest', (_message.Message,), {
+    'DESCRIPTOR': _SYNTHESIZEREQUEST,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.SynthesizeRequest)
+})
+_sym_db.RegisterMessage(SynthesizeRequest)
+
+BatchSynthesizeRequest = _reflection.GeneratedProtocolMessageType('BatchSynthesizeRequest', (_message.Message,), {
+    'DESCRIPTOR': _BATCHSYNTHESIZEREQUEST,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.BatchSynthesizeRequest)
+})
+_sym_db.RegisterMessage(BatchSynthesizeRequest)
+
+BatchSynthesizeResponse = _reflection.GeneratedProtocolMessageType('BatchSynthesizeResponse', (_message.Message,), {
+    'DESCRIPTOR': _BATCHSYNTHESIZERESPONSE,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.BatchSynthesizeResponse)
+})
+_sym_db.RegisterMessage(BatchSynthesizeResponse)
+
+RequestConfig = _reflection.GeneratedProtocolMessageType('RequestConfig', (_message.Message,), {
+    'DESCRIPTOR': _REQUESTCONFIG,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.RequestConfig)
+})
+_sym_db.RegisterMessage(RequestConfig)
+
+SynthesizeResponse = _reflection.GeneratedProtocolMessageType('SynthesizeResponse', (_message.Message,), {
+    'DESCRIPTOR': _SYNTHESIZERESPONSE,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.SynthesizeResponse)
+})
+_sym_db.RegisterMessage(SynthesizeResponse)
+
+NormalizeTextRequest = _reflection.GeneratedProtocolMessageType('NormalizeTextRequest', (_message.Message,), {
+    'DESCRIPTOR': _NORMALIZETEXTREQUEST,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.NormalizeTextRequest)
+})
+_sym_db.RegisterMessage(NormalizeTextRequest)
+
+NormalizeTextResponse = _reflection.GeneratedProtocolMessageType('NormalizeTextResponse', (_message.Message,), {
+    'DESCRIPTOR': _NORMALIZETEXTRESPONSE,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.NormalizeTextResponse)
+})
+_sym_db.RegisterMessage(NormalizeTextResponse)
+
+T2SGetServiceInfoResponse = _reflection.GeneratedProtocolMessageType('T2SGetServiceInfoResponse', (_message.Message,), {
+    'DESCRIPTOR': _T2SGETSERVICEINFORESPONSE,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.T2SGetServiceInfoResponse)
+})
+_sym_db.RegisterMessage(T2SGetServiceInfoResponse)
+
+ListT2sPipelinesRequest = _reflection.GeneratedProtocolMessageType('ListT2sPipelinesRequest', (_message.Message,), {
+    'DESCRIPTOR': _LISTT2SPIPELINESREQUEST,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.ListT2sPipelinesRequest)
+})
+_sym_db.RegisterMessage(ListT2sPipelinesRequest)
+
+ListT2sPipelinesResponse = _reflection.GeneratedProtocolMessageType('ListT2sPipelinesResponse', (_message.Message,), {
+    'DESCRIPTOR': _LISTT2SPIPELINESRESPONSE,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.ListT2sPipelinesResponse)
+})
+_sym_db.RegisterMessage(ListT2sPipelinesResponse)
+
+ListT2sLanguagesRequest = _reflection.GeneratedProtocolMessageType('ListT2sLanguagesRequest', (_message.Message,), {
+    'DESCRIPTOR': _LISTT2SLANGUAGESREQUEST,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.ListT2sLanguagesRequest)
+})
+_sym_db.RegisterMessage(ListT2sLanguagesRequest)
+
+ListT2sLanguagesResponse = _reflection.GeneratedProtocolMessageType('ListT2sLanguagesResponse', (_message.Message,), {
+    'DESCRIPTOR': _LISTT2SLANGUAGESRESPONSE,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.ListT2sLanguagesResponse)
+})
+_sym_db.RegisterMessage(ListT2sLanguagesResponse)
+
+ListT2sDomainsRequest = _reflection.GeneratedProtocolMessageType('ListT2sDomainsRequest', (_message.Message,), {
+    'DESCRIPTOR': _LISTT2SDOMAINSREQUEST,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.ListT2sDomainsRequest)
+})
+_sym_db.RegisterMessage(ListT2sDomainsRequest)
+
+ListT2sDomainsResponse = _reflection.GeneratedProtocolMessageType('ListT2sDomainsResponse', (_message.Message,), {
+    'DESCRIPTOR': _LISTT2SDOMAINSRESPONSE,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.ListT2sDomainsResponse)
+})
+_sym_db.RegisterMessage(ListT2sDomainsResponse)
+
+T2sPipelineId = _reflection.GeneratedProtocolMessageType('T2sPipelineId', (_message.Message,), {
+    'DESCRIPTOR': _T2SPIPELINEID,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.T2sPipelineId)
+})
+_sym_db.RegisterMessage(T2sPipelineId)
+
+Text2SpeechConfig = _reflection.GeneratedProtocolMessageType('Text2SpeechConfig', (_message.Message,), {
+    'DESCRIPTOR': _TEXT2SPEECHCONFIG,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.Text2SpeechConfig)
+})
+_sym_db.RegisterMessage(Text2SpeechConfig)
+
+T2SDescription = _reflection.GeneratedProtocolMessageType('T2SDescription', (_message.Message,), {
+    'DESCRIPTOR': _T2SDESCRIPTION,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.T2SDescription)
+})
+_sym_db.RegisterMessage(T2SDescription)
+
+T2SInference = _reflection.GeneratedProtocolMessageType('T2SInference', (_message.Message,), {
+    'DESCRIPTOR': _T2SINFERENCE,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.T2SInference)
+})
+_sym_db.RegisterMessage(T2SInference)
+
+CompositeInference = _reflection.GeneratedProtocolMessageType('CompositeInference', (_message.Message,), {
+    'DESCRIPTOR': _COMPOSITEINFERENCE,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.CompositeInference)
+})
+_sym_db.RegisterMessage(CompositeInference)
+
+Text2Mel = _reflection.GeneratedProtocolMessageType('Text2Mel', (_message.Message,), {
+    'DESCRIPTOR': _TEXT2MEL,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.Text2Mel)
+})
+_sym_db.RegisterMessage(Text2Mel)
+
+GlowTTS = _reflection.GeneratedProtocolMessageType('GlowTTS', (_message.Message,), {
+    'DESCRIPTOR': _GLOWTTS,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.GlowTTS)
+})
+_sym_db.RegisterMessage(GlowTTS)
+
+GlowTTSTriton = _reflection.GeneratedProtocolMessageType('GlowTTSTriton', (_message.Message,), {
+    'DESCRIPTOR': _GLOWTTSTRITON,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.GlowTTSTriton)
+})
+_sym_db.RegisterMessage(GlowTTSTriton)
+
+Mel2Audio = _reflection.GeneratedProtocolMessageType('Mel2Audio', (_message.Message,), {
+    'DESCRIPTOR': _MEL2AUDIO,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.Mel2Audio)
+})
+_sym_db.RegisterMessage(Mel2Audio)
+
+HiFiGan = _reflection.GeneratedProtocolMessageType('HiFiGan', (_message.Message,), {
+    'DESCRIPTOR': _HIFIGAN,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.HiFiGan)
+})
+_sym_db.RegisterMessage(HiFiGan)
+
+HiFiGanTriton = _reflection.GeneratedProtocolMessageType('HiFiGanTriton', (_message.Message,), {
+    'DESCRIPTOR': _HIFIGANTRITON,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.HiFiGanTriton)
+})
+_sym_db.RegisterMessage(HiFiGanTriton)
+
+MbMelganTriton = _reflection.GeneratedProtocolMessageType('MbMelganTriton', (_message.Message,), {
+    'DESCRIPTOR': _MBMELGANTRITON,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.MbMelganTriton)
+})
+_sym_db.RegisterMessage(MbMelganTriton)
+
+Caching = _reflection.GeneratedProtocolMessageType('Caching', (_message.Message,), {
+    'DESCRIPTOR': _CACHING,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.Caching)
+})
+_sym_db.RegisterMessage(Caching)
+
+T2SNormalization = _reflection.GeneratedProtocolMessageType('T2SNormalization', (_message.Message,), {
+    'DESCRIPTOR': _T2SNORMALIZATION,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.T2SNormalization)
+})
+_sym_db.RegisterMessage(T2SNormalization)
+
+Postprocessing = _reflection.GeneratedProtocolMessageType('Postprocessing', (_message.Message,), {
+    'DESCRIPTOR': _POSTPROCESSING,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.Postprocessing)
+})
+_sym_db.RegisterMessage(Postprocessing)
+
+Logmnse = _reflection.GeneratedProtocolMessageType('Logmnse', (_message.Message,), {
+    'DESCRIPTOR': _LOGMNSE,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.Logmnse)
+})
+_sym_db.RegisterMessage(Logmnse)
+
+Wiener = _reflection.GeneratedProtocolMessageType('Wiener', (_message.Message,), {
+    'DESCRIPTOR': _WIENER,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.Wiener)
+})
+_sym_db.RegisterMessage(Wiener)
+
+Apodization = _reflection.GeneratedProtocolMessageType('Apodization', (_message.Message,), {
+    'DESCRIPTOR': _APODIZATION,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.Apodization)
+})
+_sym_db.RegisterMessage(Apodization)
+
+T2SCustomLengthScales = _reflection.GeneratedProtocolMessageType('T2SCustomLengthScales', (_message.Message,), {
+    'DESCRIPTOR': _T2SCUSTOMLENGTHSCALES,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.T2SCustomLengthScales)
+})
+_sym_db.RegisterMessage(T2SCustomLengthScales)
+
+PhonemizerId = _reflection.GeneratedProtocolMessageType('PhonemizerId', (_message.Message,), {
+    'DESCRIPTOR': _PHONEMIZERID,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.PhonemizerId)
+})
+_sym_db.RegisterMessage(PhonemizerId)
+
+CustomPhonemizerProto = _reflection.GeneratedProtocolMessageType('CustomPhonemizerProto', (_message.Message,), {
+    'DESCRIPTOR': _CUSTOMPHONEMIZERPROTO,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.CustomPhonemizerProto)
+})
+_sym_db.RegisterMessage(CustomPhonemizerProto)
+
+Map = _reflection.GeneratedProtocolMessageType('Map', (_message.Message,), {
+    'DESCRIPTOR': _MAP,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.Map)
+})
+_sym_db.RegisterMessage(Map)
+
+ListCustomPhonemizerResponse = _reflection.GeneratedProtocolMessageType('ListCustomPhonemizerResponse', (_message.Message,), {
+    'DESCRIPTOR': _LISTCUSTOMPHONEMIZERRESPONSE,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.ListCustomPhonemizerResponse)
+})
+_sym_db.RegisterMessage(ListCustomPhonemizerResponse)
+
+ListCustomPhonemizerRequest = _reflection.GeneratedProtocolMessageType('ListCustomPhonemizerRequest', (_message.Message,), {
+    'DESCRIPTOR': _LISTCUSTOMPHONEMIZERREQUEST,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.ListCustomPhonemizerRequest)
+})
+_sym_db.RegisterMessage(ListCustomPhonemizerRequest)
+
+UpdateCustomPhonemizerRequest = _reflection.GeneratedProtocolMessageType('UpdateCustomPhonemizerRequest', (_message.Message,), {
+    'DESCRIPTOR': _UPDATECUSTOMPHONEMIZERREQUEST,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.UpdateCustomPhonemizerRequest)
+})
+_sym_db.RegisterMessage(UpdateCustomPhonemizerRequest)
+
+CreateCustomPhonemizerRequest = _reflection.GeneratedProtocolMessageType('CreateCustomPhonemizerRequest', (_message.Message,), {
+    'DESCRIPTOR': _CREATECUSTOMPHONEMIZERREQUEST,
+    '__module__': 'ondewo.t2s.text_to_speech_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.t2s.CreateCustomPhonemizerRequest)
 })
-_sym_db.RegisterMessage(GetLatestSessionReviewRequest)
+_sym_db.RegisterMessage(CreateCustomPhonemizerRequest)
 
-_SESSIONS = DESCRIPTOR.services_by_name['Sessions']
+_TEXT2SPEECH = DESCRIPTOR.services_by_name['Text2Speech']
+_CUSTOMPHONEMIZERS = DESCRIPTOR.services_by_name['CustomPhonemizers']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b'\n\036com.google.cloud.dialogflow.v2B\014SessionProtoP\001ZDgoogle.golang.org/genproto/googleapis/cloud/dialogflow/v2;dialogflow\370\001\001\242\002\002DF\252\002\032Google.Cloud.Dialogflow.V2'
-    _SESSIONS.methods_by_name['DetectIntent']._options = None
-    _SESSIONS.methods_by_name['DetectIntent']._serialized_options = b'\202\323\344\223\002;\"6/v2/{session=projects/*/agent/sessions/*}:detectIntent:\001*'
-    _SESSIONS.methods_by_name['ListSessions']._options = None
-    _SESSIONS.methods_by_name['ListSessions']._serialized_options = b'\202\323\344\223\002(\022&/v2/{parent=projects/*/agent}/sessions'
-    _SESSIONS.methods_by_name['GetSession']._options = None
-    _SESSIONS.methods_by_name['GetSession']._serialized_options = b'\202\323\344\223\002.\022,/v2/{session_id=projects/*/agent/sessions/*}'
-    _SESSIONS.methods_by_name['CreateSession']._options = None
-    _SESSIONS.methods_by_name['CreateSession']._serialized_options = b'\202\323\344\223\002+\"&/v2/{parent=projects/*/agent}/sessions:\001*'
-    _SESSIONS.methods_by_name['TrackSessionStep']._options = None
-    _SESSIONS.methods_by_name['TrackSessionStep']._serialized_options = b'\202\323\344\223\002B\"=/v2/{session_id=projects/*/agent/sessions/*}:trackSessionStep:\001*'
-    _SESSIONS.methods_by_name['DeleteSession']._options = None
-    _SESSIONS.methods_by_name['DeleteSession']._serialized_options = b'\202\323\344\223\002.*,/v2/{session_id=projects/*/agent/sessions/*}'
-    _SESSIONS.methods_by_name['ListSessionLabels']._options = None
-    _SESSIONS.methods_by_name['ListSessionLabels']._serialized_options = b'\202\323\344\223\002/\022-/v2/{parent=projects/*/agent}/sessions/labels'
-    _SESSIONS.methods_by_name['AddSessionLabels']._options = None
-    _SESSIONS.methods_by_name['AddSessionLabels']._serialized_options = b'\202\323\344\223\002<\"7/v2/{session_id=projects/*/agent/sessions/*}/labels:add:\001*'
-    _SESSIONS.methods_by_name['RemoveSessionLabels']._options = None
-    _SESSIONS.methods_by_name['RemoveSessionLabels']._serialized_options = b'\202\323\344\223\002?\":/v2/{session_id=projects/*/agent/sessions/*}/labels:remove:\001*'
-    _SESSIONS.methods_by_name['ListSessionReviews']._options = None
-    _SESSIONS.methods_by_name['ListSessionReviews']._serialized_options = b'\202\323\344\223\0026\0224/v2/{session_id=projects/*/agent/sessions/*}/reviews'
-    _SESSIONS.methods_by_name['GetSessionReview']._options = None
-    _SESSIONS.methods_by_name['GetSessionReview']._serialized_options = b'\202\323\344\223\002?\022=/v2/{session_review_id=projects/*/agent/sessions/*/reviews/*}'
-    _SESSIONS.methods_by_name['GetLatestSessionReview']._options = None
-    _SESSIONS.methods_by_name['GetLatestSessionReview']._serialized_options = b'\202\323\344\223\002M\022K/v2/{session_id=projects/*/agent/sessions/*}/reviews:getLatestSessionReview'
-    _SESSIONS.methods_by_name['CreateSessionReview']._options = None
-    _SESSIONS.methods_by_name['CreateSessionReview']._serialized_options = b'\202\323\344\223\002E\"@/v2/{session_id=projects/*/agent/sessions/*}:createSessionReview:\001*'
-    _AUDIOENCODING._serialized_start = 5952
-    _AUDIOENCODING._serialized_end = 6203
-    _DETECTINTENTREQUEST._serialized_start = 262
-    _DETECTINTENTREQUEST._serialized_end = 417
-    _DETECTINTENTRESPONSE._serialized_start = 420
-    _DETECTINTENTRESPONSE._serialized_end = 554
-    _QUERYPARAMETERS._serialized_start = 557
-    _QUERYPARAMETERS._serialized_end = 741
-    _QUERYINPUT._serialized_start = 744
-    _QUERYINPUT._serialized_end = 899
-    _QUERYRESULT._serialized_start = 902
-    _QUERYRESULT._serialized_end = 1422
-    _STREAMINGDETECTINTENTREQUEST._serialized_start = 1425
-    _STREAMINGDETECTINTENTREQUEST._serialized_end = 1615
-    _STREAMINGDETECTINTENTRESPONSE._serialized_start = 1618
-    _STREAMINGDETECTINTENTRESPONSE._serialized_end = 1829
-    _STREAMINGRECOGNITIONRESULT._serialized_start = 1832
-    _STREAMINGRECOGNITIONRESULT._serialized_end = 2082
-    _STREAMINGRECOGNITIONRESULT_MESSAGETYPE._serialized_start = 1994
-    _STREAMINGRECOGNITIONRESULT_MESSAGETYPE._serialized_end = 2082
-    _INPUTAUDIOCONFIG._serialized_start = 2085
-    _INPUTAUDIOCONFIG._serialized_end = 2226
-    _TEXTINPUT._serialized_start = 2228
-    _TEXTINPUT._serialized_end = 2276
-    _EVENTINPUT._serialized_start = 2278
-    _EVENTINPUT._serialized_end = 2372
-    _SESSION._serialized_start = 2375
-    _SESSION._serialized_end = 2561
-    _SESSION_VIEW._serialized_start = 2501
-    _SESSION_VIEW._serialized_end = 2561
-    _SESSIONSTEP._serialized_start = 2564
-    _SESSIONSTEP._serialized_end = 2746
-    _TRACKSESSIONSTEPREQUEST._serialized_start = 2749
-    _TRACKSESSIONSTEPREQUEST._serialized_end = 2889
-    _LISTSESSIONSREQUEST._serialized_start = 2892
-    _LISTSESSIONSREQUEST._serialized_end = 3048
-    _SESSIONFILTER._serialized_start = 3051
-    _SESSIONFILTER._serialized_end = 3596
-    _SESSIONINFO._serialized_start = 3599
-    _SESSIONINFO._serialized_end = 4105
-    _SESSIONINFO_CONTEXTSTEPS._serialized_start = 4052
-    _SESSIONINFO_CONTEXTSTEPS._serialized_end = 4105
-    _LISTSESSIONSRESPONSE._serialized_start = 4107
-    _LISTSESSIONSRESPONSE._serialized_end = 4193
-    _GETSESSIONREQUEST._serialized_start = 4195
-    _GETSESSIONREQUEST._serialized_end = 4282
-    _CREATESESSIONREQUEST._serialized_start = 4284
-    _CREATESESSIONREQUEST._serialized_end = 4344
-    _DELETESESSIONREQUEST._serialized_start = 4346
-    _DELETESESSIONREQUEST._serialized_end = 4388
-    _CREATESESSIONREVIEWREQUEST._serialized_start = 4391
-    _CREATESESSIONREVIEWREQUEST._serialized_end = 4577
-    _SESSIONREVIEW._serialized_start = 4580
-    _SESSIONREVIEW._serialized_end = 4745
-    _SESSIONREVIEW_VIEW._serialized_start = 2501
-    _SESSIONREVIEW_VIEW._serialized_end = 2561
-    _SESSIONREVIEWSTEP._serialized_start = 4748
-    _SESSIONREVIEWSTEP._serialized_end = 4989
-    _DETECTEDINTENT._serialized_start = 4992
-    _DETECTEDINTENT._serialized_end = 5168
-    _LISTSESSIONLABELSREQUEST._serialized_start = 5170
-    _LISTSESSIONLABELSREQUEST._serialized_end = 5212
-    _LISTSESSIONLABELSRESPONSE._serialized_start = 5214
-    _LISTSESSIONLABELSRESPONSE._serialized_end = 5257
-    _ADDSESSIONLABELSREQUEST._serialized_start = 5259
-    _ADDSESSIONLABELSREQUEST._serialized_end = 5368
-    _REMOVESESSIONLABELSREQUEST._serialized_start = 5370
-    _REMOVESESSIONLABELSREQUEST._serialized_end = 5482
-    _LISTSESSIONREVIEWSREQUEST._serialized_start = 5485
-    _LISTSESSIONREVIEWSREQUEST._serialized_end = 5613
-    _LISTSESSIONREVIEWSRESPONSE._serialized_start = 5615
-    _LISTSESSIONREVIEWSRESPONSE._serialized_end = 5720
-    _GETSESSIONREVIEWREQUEST._serialized_start = 5722
-    _GETSESSIONREVIEWREQUEST._serialized_end = 5835
-    _GETLATESTSESSIONREVIEWREQUEST._serialized_start = 5837
-    _GETLATESTSESSIONREVIEWREQUEST._serialized_end = 5949
-    _SESSIONS._serialized_start = 6206
-    _SESSIONS._serialized_end = 8265
+    _PCM._serialized_start = 4624
+    _PCM._serialized_end = 4712
+    _AUDIOFORMAT._serialized_start = 4714
+    _AUDIOFORMAT._serialized_end = 4791
+    _SYNTHESIZEREQUEST._serialized_start = 76
+    _SYNTHESIZEREQUEST._serialized_end = 152
+    _BATCHSYNTHESIZEREQUEST._serialized_start = 154
+    _BATCHSYNTHESIZEREQUEST._serialized_end = 232
+    _BATCHSYNTHESIZERESPONSE._serialized_start = 234
+    _BATCHSYNTHESIZERESPONSE._serialized_end = 315
+    _REQUESTCONFIG._serialized_start = 318
+    _REQUESTCONFIG._serialized_end = 689
+    _SYNTHESIZERESPONSE._serialized_start = 692
+    _SYNTHESIZERESPONSE._serialized_end = 876
+    _NORMALIZETEXTREQUEST._serialized_start = 878
+    _NORMALIZETEXTREQUEST._serialized_end = 939
+    _NORMALIZETEXTRESPONSE._serialized_start = 941
+    _NORMALIZETEXTRESPONSE._serialized_end = 989
+    _T2SGETSERVICEINFORESPONSE._serialized_start = 991
+    _T2SGETSERVICEINFORESPONSE._serialized_end = 1035
+    _LISTT2SPIPELINESREQUEST._serialized_start = 1038
+    _LISTT2SPIPELINESREQUEST._serialized_end = 1170
+    _LISTT2SPIPELINESRESPONSE._serialized_start = 1172
+    _LISTT2SPIPELINESRESPONSE._serialized_end = 1248
+    _LISTT2SLANGUAGESREQUEST._serialized_start = 1250
+    _LISTT2SLANGUAGESREQUEST._serialized_end = 1363
+    _LISTT2SLANGUAGESRESPONSE._serialized_start = 1365
+    _LISTT2SLANGUAGESRESPONSE._serialized_end = 1410
+    _LISTT2SDOMAINSREQUEST._serialized_start = 1412
+    _LISTT2SDOMAINSREQUEST._serialized_end = 1525
+    _LISTT2SDOMAINSRESPONSE._serialized_start = 1527
+    _LISTT2SDOMAINSRESPONSE._serialized_end = 1568
+    _T2SPIPELINEID._serialized_start = 1570
+    _T2SPIPELINEID._serialized_end = 1597
+    _TEXT2SPEECHCONFIG._serialized_start = 1600
+    _TEXT2SPEECHCONFIG._serialized_end = 1846
+    _T2SDESCRIPTION._serialized_start = 1849
+    _T2SDESCRIPTION._serialized_end = 1984
+    _T2SINFERENCE._serialized_start = 1986
+    _T2SINFERENCE._serialized_end = 2113
+    _COMPOSITEINFERENCE._serialized_start = 2115
+    _COMPOSITEINFERENCE._serialized_end = 2217
+    _TEXT2MEL._serialized_start = 2219
+    _TEXT2MEL._serialized_end = 2334
+    _GLOWTTS._serialized_start = 2337
+    _GLOWTTS._serialized_end = 2485
+    _GLOWTTSTRITON._serialized_start = 2488
+    _GLOWTTSTRITON._serialized_end = 2663
+    _MEL2AUDIO._serialized_start = 2666
+    _MEL2AUDIO._serialized_end = 2836
+    _HIFIGAN._serialized_start = 2838
+    _HIFIGAN._serialized_end = 2925
+    _HIFIGANTRITON._serialized_start = 2927
+    _HIFIGANTRITON._serialized_end = 2990
+    _MBMELGANTRITON._serialized_start = 2992
+    _MBMELGANTRITON._serialized_end = 3096
+    _CACHING._serialized_start = 3099
+    _CACHING._serialized_end = 3242
+    _T2SNORMALIZATION._serialized_start = 3245
+    _T2SNORMALIZATION._serialized_end = 3471
+    _POSTPROCESSING._serialized_start = 3474
+    _POSTPROCESSING._serialized_end = 3650
+    _LOGMNSE._serialized_start = 3652
+    _LOGMNSE._serialized_end = 3730
+    _WIENER._serialized_start = 3732
+    _WIENER._serialized_end = 3829
+    _APODIZATION._serialized_start = 3831
+    _APODIZATION._serialized_end = 3870
+    _T2SCUSTOMLENGTHSCALES._serialized_start = 3873
+    _T2SCUSTOMLENGTHSCALES._serialized_end = 4041
+    _PHONEMIZERID._serialized_start = 4043
+    _PHONEMIZERID._serialized_end = 4069
+    _CUSTOMPHONEMIZERPROTO._serialized_start = 4071
+    _CUSTOMPHONEMIZERPROTO._serialized_end = 4137
+    _MAP._serialized_start = 4139
+    _MAP._serialized_end = 4182
+    _LISTCUSTOMPHONEMIZERRESPONSE._serialized_start = 4184
+    _LISTCUSTOMPHONEMIZERRESPONSE._serialized_end = 4270
+    _LISTCUSTOMPHONEMIZERREQUEST._serialized_start = 4272
+    _LISTCUSTOMPHONEMIZERREQUEST._serialized_end = 4323
+    _UPDATECUSTOMPHONEMIZERREQUEST._serialized_start = 4326
+    _UPDATECUSTOMPHONEMIZERREQUEST._serialized_end = 4542
+    _UPDATECUSTOMPHONEMIZERREQUEST_UPDATEMETHOD._serialized_start = 4481
+    _UPDATECUSTOMPHONEMIZERREQUEST_UPDATEMETHOD._serialized_end = 4542
+    _CREATECUSTOMPHONEMIZERREQUEST._serialized_start = 4544
+    _CREATECUSTOMPHONEMIZERREQUEST._serialized_end = 4622
+    _TEXT2SPEECH._serialized_start = 4794
+    _TEXT2SPEECH._serialized_end = 5747
+    _CUSTOMPHONEMIZERS._serialized_start = 5750
+    _CUSTOMPHONEMIZERS._serialized_end = 6245
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/session_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/user_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,533 +1,545 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from ondewo.nlu import session_pb2 as ondewo_dot_nlu_dot_session__pb2
+from ondewo.nlu import user_pb2 as ondewo_dot_nlu_dot_user__pb2
 
 
-class SessionsStub(object):
-    """A session represents an interaction with a user. You retrieve user input
-    and pass it to the [DetectIntent][google.cloud.dialogflow.v2.Sessions.DetectIntent] (or
-    [StreamingDetectIntent][google.cloud.dialogflow.v2.Sessions.StreamingDetectIntent]) method to determine
-    user intent and respond.
-    """
+class UsersStub(object):
+    """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.DetectIntent = channel.unary_unary(
-            '/ondewo.nlu.Sessions/DetectIntent',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.DetectIntentRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_session__pb2.DetectIntentResponse.FromString,
-        )
-        self.StreamingDetectIntent = channel.stream_stream(
-            '/ondewo.nlu.Sessions/StreamingDetectIntent',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.StreamingDetectIntentRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_session__pb2.StreamingDetectIntentResponse.FromString,
-        )
-        self.ListSessions = channel.unary_unary(
-            '/ondewo.nlu.Sessions/ListSessions',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.ListSessionsRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_session__pb2.ListSessionsResponse.FromString,
-        )
-        self.GetSession = channel.unary_unary(
-            '/ondewo.nlu.Sessions/GetSession',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.GetSessionRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_session__pb2.Session.FromString,
-        )
-        self.CreateSession = channel.unary_unary(
-            '/ondewo.nlu.Sessions/CreateSession',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.CreateSessionRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_session__pb2.Session.FromString,
-        )
-        self.TrackSessionStep = channel.unary_unary(
-            '/ondewo.nlu.Sessions/TrackSessionStep',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.TrackSessionStepRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_session__pb2.Session.FromString,
-        )
-        self.DeleteSession = channel.unary_unary(
-            '/ondewo.nlu.Sessions/DeleteSession',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.DeleteSessionRequest.SerializeToString,
+        self.CreateUser = channel.unary_unary(
+            '/ondewo.nlu.Users/CreateUser',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.CreateUserRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_user__pb2.User.FromString,
+        )
+        self.GetUser = channel.unary_unary(
+            '/ondewo.nlu.Users/GetUser',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.GetUserRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_user__pb2.User.FromString,
+        )
+        self.GetUserInfo = channel.unary_unary(
+            '/ondewo.nlu.Users/GetUserInfo',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.GetUserRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_user__pb2.UserInfo.FromString,
+        )
+        self.DeleteUser = channel.unary_unary(
+            '/ondewo.nlu.Users/DeleteUser',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.GetUserRequest.SerializeToString,
             response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
         )
-        self.ListSessionLabels = channel.unary_unary(
-            '/ondewo.nlu.Sessions/ListSessionLabels',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.ListSessionLabelsRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_session__pb2.ListSessionLabelsResponse.FromString,
-        )
-        self.AddSessionLabels = channel.unary_unary(
-            '/ondewo.nlu.Sessions/AddSessionLabels',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.AddSessionLabelsRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_session__pb2.Session.FromString,
-        )
-        self.RemoveSessionLabels = channel.unary_unary(
-            '/ondewo.nlu.Sessions/RemoveSessionLabels',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.RemoveSessionLabelsRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_session__pb2.Session.FromString,
-        )
-        self.ListSessionReviews = channel.unary_unary(
-            '/ondewo.nlu.Sessions/ListSessionReviews',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.ListSessionReviewsRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_session__pb2.ListSessionReviewsResponse.FromString,
-        )
-        self.GetSessionReview = channel.unary_unary(
-            '/ondewo.nlu.Sessions/GetSessionReview',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.GetSessionReviewRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_session__pb2.SessionReview.FromString,
-        )
-        self.GetLatestSessionReview = channel.unary_unary(
-            '/ondewo.nlu.Sessions/GetLatestSessionReview',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.GetLatestSessionReviewRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_session__pb2.SessionReview.FromString,
+        self.UpdateUser = channel.unary_unary(
+            '/ondewo.nlu.Users/UpdateUser',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.UpdateUserRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_user__pb2.User.FromString,
+        )
+        self.ListUsers = channel.unary_unary(
+            '/ondewo.nlu.Users/ListUsers',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.ListUsersRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ListUsersResponse.FromString,
+        )
+        self.ListUserInfos = channel.unary_unary(
+            '/ondewo.nlu.Users/ListUserInfos',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.ListUsersRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ListUserInfosResponse.FromString,
+        )
+        self.CreateServerRole = channel.unary_unary(
+            '/ondewo.nlu.Users/CreateServerRole',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.CreateServerRoleRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ServerRole.FromString,
+        )
+        self.GetServerRole = channel.unary_unary(
+            '/ondewo.nlu.Users/GetServerRole',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.GetServerRoleRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ServerRole.FromString,
+        )
+        self.DeleteServerRole = channel.unary_unary(
+            '/ondewo.nlu.Users/DeleteServerRole',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.DeleteServerRoleRequest.SerializeToString,
+            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
         )
-        self.CreateSessionReview = channel.unary_unary(
-            '/ondewo.nlu.Sessions/CreateSessionReview',
-            request_serializer=ondewo_dot_nlu_dot_session__pb2.CreateSessionReviewRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_session__pb2.SessionReview.FromString,
+        self.UpdateServerRole = channel.unary_unary(
+            '/ondewo.nlu.Users/UpdateServerRole',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.UpdateServerRoleRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ServerRole.FromString,
+        )
+        self.ListServerRoles = channel.unary_unary(
+            '/ondewo.nlu.Users/ListServerRoles',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.ListServerRolesRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ListServerRolesResponse.FromString,
+        )
+        self.ListServerPermissions = channel.unary_unary(
+            '/ondewo.nlu.Users/ListServerPermissions',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.ListServerPermissionsRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ListServerPermissionsResponse.FromString,
+        )
+        self.Login = channel.unary_unary(
+            '/ondewo.nlu.Users/Login',
+            request_serializer=ondewo_dot_nlu_dot_user__pb2.LoginRequest.SerializeToString,
+            response_deserializer=ondewo_dot_nlu_dot_user__pb2.LoginResponse.FromString,
+        )
+        self.CheckLogin = channel.unary_unary(
+            '/ondewo.nlu.Users/CheckLogin',
+            request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
         )
 
 
-class SessionsServicer(object):
-    """A session represents an interaction with a user. You retrieve user input
-    and pass it to the [DetectIntent][google.cloud.dialogflow.v2.Sessions.DetectIntent] (or
-    [StreamingDetectIntent][google.cloud.dialogflow.v2.Sessions.StreamingDetectIntent]) method to determine
-    user intent and respond.
-    """
+class UsersServicer(object):
+    """Missing associated documentation comment in .proto file."""
 
-    def DetectIntent(self, request, context):
-        """Processes a natural language query and returns structured, actionable data
-        as a result. This method is not idempotent, because it may cause contexts
-        and session entity types to be updated, which in turn might affect
-        results of future queries.
+    def CreateUser(self, request, context):
+        """Creates user
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def StreamingDetectIntent(self, request_iterator, context):
-        """Processes a natural language query in audio format in a streaming fashion
-        and returns structured, actionable data as a result. This method is only
-        available via the gRPC API (not REST).
+    def GetUser(self, request, context):
+        """Gets user
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListSessions(self, request, context):
-        """*** SESSION RELATED ENDPOINTS *** //
-        ListSessions: returns list of sessions from ondewo-kb; by default returns only session IDs
+    def GetUserInfo(self, request, context):
+        """Gets user information
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetSession(self, request, context):
-        """GetSession: returns a session(=conversation) from ondewo-kb
+    def DeleteUser(self, request, context):
+        """Deletes user
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CreateSession(self, request, context):
-        """CreateSession: creates and returns a session(=conversation) from ondewo-kb
+    def UpdateUser(self, request, context):
+        """Updates user
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def TrackSessionStep(self, request, context):
-        """TrackSessionStep: append to an existing session; creates it if not existing
+    def ListUsers(self, request, context):
+        """Lists users
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeleteSession(self, request, context):
-        """DeleteSession: delete a session(=conversation) from ondewo-kb (for testing only)
+    def ListUserInfos(self, request, context):
+        """Lists users information
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListSessionLabels(self, request, context):
-        """*** SESSION-LABEL RELATED ENDPOINTS *** //
+    def CreateServerRole(self, request, context):
+        """Creates server role
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def AddSessionLabels(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetServerRole(self, request, context):
+        """Get server role
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def RemoveSessionLabels(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def DeleteServerRole(self, request, context):
+        """Deletes server role
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListSessionReviews(self, request, context):
-        """*** SESSION-REVIEW RELATED ENDPOINTS *** //
-        ListSessionReviews:
-        returns list of session reviews from ondewo-kb; by default only returns session review IDs
+    def UpdateServerRole(self, request, context):
+        """Updates server role
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetSessionReview(self, request, context):
-        """GetSessionReview:
-        returns a session-review from ondewo-kb or computes the first review if none exists
+    def ListServerRoles(self, request, context):
+        """Lists server roles
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetLatestSessionReview(self, request, context):
-        """GetLatestSessionReview:
-        returns a session-review from ondewo-kb or computes the first review if none exists
+    def ListServerPermissions(self, request, context):
+        """Lists server permissions
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CreateSessionReview(self, request, context):
-        """CreateSessionReview:
-        persist a session review in ondewo-kb
-        as a side effect: also update training data in ondewo-cai
+    def Login(self, request, context):
+        """Request to login
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def CheckLogin(self, request, context):
+        """Checks login
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
-def add_SessionsServicer_to_server(servicer, server):
+
+def add_UsersServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        'DetectIntent': grpc.unary_unary_rpc_method_handler(
-            servicer.DetectIntent,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.DetectIntentRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_session__pb2.DetectIntentResponse.SerializeToString,
-        ),
-        'StreamingDetectIntent': grpc.stream_stream_rpc_method_handler(
-            servicer.StreamingDetectIntent,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.StreamingDetectIntentRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_session__pb2.StreamingDetectIntentResponse.SerializeToString,
-        ),
-        'ListSessions': grpc.unary_unary_rpc_method_handler(
-            servicer.ListSessions,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.ListSessionsRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_session__pb2.ListSessionsResponse.SerializeToString,
-        ),
-        'GetSession': grpc.unary_unary_rpc_method_handler(
-            servicer.GetSession,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.GetSessionRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_session__pb2.Session.SerializeToString,
-        ),
-        'CreateSession': grpc.unary_unary_rpc_method_handler(
-            servicer.CreateSession,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.CreateSessionRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_session__pb2.Session.SerializeToString,
-        ),
-        'TrackSessionStep': grpc.unary_unary_rpc_method_handler(
-            servicer.TrackSessionStep,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.TrackSessionStepRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_session__pb2.Session.SerializeToString,
-        ),
-        'DeleteSession': grpc.unary_unary_rpc_method_handler(
-            servicer.DeleteSession,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.DeleteSessionRequest.FromString,
+        'CreateUser': grpc.unary_unary_rpc_method_handler(
+            servicer.CreateUser,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.CreateUserRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_user__pb2.User.SerializeToString,
+        ),
+        'GetUser': grpc.unary_unary_rpc_method_handler(
+            servicer.GetUser,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.GetUserRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_user__pb2.User.SerializeToString,
+        ),
+        'GetUserInfo': grpc.unary_unary_rpc_method_handler(
+            servicer.GetUserInfo,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.GetUserRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_user__pb2.UserInfo.SerializeToString,
+        ),
+        'DeleteUser': grpc.unary_unary_rpc_method_handler(
+            servicer.DeleteUser,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.GetUserRequest.FromString,
+            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+        ),
+        'UpdateUser': grpc.unary_unary_rpc_method_handler(
+            servicer.UpdateUser,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.UpdateUserRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_user__pb2.User.SerializeToString,
+        ),
+        'ListUsers': grpc.unary_unary_rpc_method_handler(
+            servicer.ListUsers,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.ListUsersRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_user__pb2.ListUsersResponse.SerializeToString,
+        ),
+        'ListUserInfos': grpc.unary_unary_rpc_method_handler(
+            servicer.ListUserInfos,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.ListUsersRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_user__pb2.ListUserInfosResponse.SerializeToString,
+        ),
+        'CreateServerRole': grpc.unary_unary_rpc_method_handler(
+            servicer.CreateServerRole,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.CreateServerRoleRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_user__pb2.ServerRole.SerializeToString,
+        ),
+        'GetServerRole': grpc.unary_unary_rpc_method_handler(
+            servicer.GetServerRole,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.GetServerRoleRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_user__pb2.ServerRole.SerializeToString,
+        ),
+        'DeleteServerRole': grpc.unary_unary_rpc_method_handler(
+            servicer.DeleteServerRole,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.DeleteServerRoleRequest.FromString,
             response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
         ),
-        'ListSessionLabels': grpc.unary_unary_rpc_method_handler(
-            servicer.ListSessionLabels,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.ListSessionLabelsRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_session__pb2.ListSessionLabelsResponse.SerializeToString,
-        ),
-        'AddSessionLabels': grpc.unary_unary_rpc_method_handler(
-            servicer.AddSessionLabels,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.AddSessionLabelsRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_session__pb2.Session.SerializeToString,
-        ),
-        'RemoveSessionLabels': grpc.unary_unary_rpc_method_handler(
-            servicer.RemoveSessionLabels,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.RemoveSessionLabelsRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_session__pb2.Session.SerializeToString,
-        ),
-        'ListSessionReviews': grpc.unary_unary_rpc_method_handler(
-            servicer.ListSessionReviews,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.ListSessionReviewsRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_session__pb2.ListSessionReviewsResponse.SerializeToString,
-        ),
-        'GetSessionReview': grpc.unary_unary_rpc_method_handler(
-            servicer.GetSessionReview,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.GetSessionReviewRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_session__pb2.SessionReview.SerializeToString,
-        ),
-        'GetLatestSessionReview': grpc.unary_unary_rpc_method_handler(
-            servicer.GetLatestSessionReview,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.GetLatestSessionReviewRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_session__pb2.SessionReview.SerializeToString,
-        ),
-        'CreateSessionReview': grpc.unary_unary_rpc_method_handler(
-            servicer.CreateSessionReview,
-            request_deserializer=ondewo_dot_nlu_dot_session__pb2.CreateSessionReviewRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_session__pb2.SessionReview.SerializeToString,
+        'UpdateServerRole': grpc.unary_unary_rpc_method_handler(
+            servicer.UpdateServerRole,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.UpdateServerRoleRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_user__pb2.ServerRole.SerializeToString,
+        ),
+        'ListServerRoles': grpc.unary_unary_rpc_method_handler(
+            servicer.ListServerRoles,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.ListServerRolesRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_user__pb2.ListServerRolesResponse.SerializeToString,
+        ),
+        'ListServerPermissions': grpc.unary_unary_rpc_method_handler(
+            servicer.ListServerPermissions,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.ListServerPermissionsRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_user__pb2.ListServerPermissionsResponse.SerializeToString,
+        ),
+        'Login': grpc.unary_unary_rpc_method_handler(
+            servicer.Login,
+            request_deserializer=ondewo_dot_nlu_dot_user__pb2.LoginRequest.FromString,
+            response_serializer=ondewo_dot_nlu_dot_user__pb2.LoginResponse.SerializeToString,
+        ),
+        'CheckLogin': grpc.unary_unary_rpc_method_handler(
+            servicer.CheckLogin,
+            request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        'ondewo.nlu.Sessions', rpc_method_handlers)
+        'ondewo.nlu.Users', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
  # This class is part of an EXPERIMENTAL API.
 
 
-class Sessions(object):
-    """A session represents an interaction with a user. You retrieve user input
-    and pass it to the [DetectIntent][google.cloud.dialogflow.v2.Sessions.DetectIntent] (or
-    [StreamingDetectIntent][google.cloud.dialogflow.v2.Sessions.StreamingDetectIntent]) method to determine
-    user intent and respond.
-    """
-
-    @staticmethod
-    def DetectIntent(request,
-                     target,
-                     options=(),
-                     channel_credentials=None,
-                     call_credentials=None,
-                     insecure=False,
-                     compression=None,
-                     wait_for_ready=None,
-                     timeout=None,
-                     metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Sessions/DetectIntent',
-                                             ondewo_dot_nlu_dot_session__pb2.DetectIntentRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_session__pb2.DetectIntentResponse.FromString,
+class Users(object):
+    """Missing associated documentation comment in .proto file."""
+
+    @staticmethod
+    def CreateUser(request,
+                   target,
+                   options=(),
+                   channel_credentials=None,
+                   call_credentials=None,
+                   insecure=False,
+                   compression=None,
+                   wait_for_ready=None,
+                   timeout=None,
+                   metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/CreateUser',
+                                             ondewo_dot_nlu_dot_user__pb2.CreateUserRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_user__pb2.User.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetUser(request,
+                target,
+                options=(),
+                channel_credentials=None,
+                call_credentials=None,
+                insecure=False,
+                compression=None,
+                wait_for_ready=None,
+                timeout=None,
+                metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/GetUser',
+                                             ondewo_dot_nlu_dot_user__pb2.GetUserRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_user__pb2.User.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetUserInfo(request,
+                    target,
+                    options=(),
+                    channel_credentials=None,
+                    call_credentials=None,
+                    insecure=False,
+                    compression=None,
+                    wait_for_ready=None,
+                    timeout=None,
+                    metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/GetUserInfo',
+                                             ondewo_dot_nlu_dot_user__pb2.GetUserRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_user__pb2.UserInfo.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def StreamingDetectIntent(request_iterator,
-                              target,
-                              options=(),
-                              channel_credentials=None,
-                              call_credentials=None,
-                              insecure=False,
-                              compression=None,
-                              wait_for_ready=None,
-                              timeout=None,
-                              metadata=None):
-        return grpc.experimental.stream_stream(request_iterator, target, '/ondewo.nlu.Sessions/StreamingDetectIntent',
-                                               ondewo_dot_nlu_dot_session__pb2.StreamingDetectIntentRequest.SerializeToString,
-                                               ondewo_dot_nlu_dot_session__pb2.StreamingDetectIntentResponse.FromString,
-                                               options, channel_credentials,
-                                               insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ListSessions(request,
-                     target,
-                     options=(),
-                     channel_credentials=None,
-                     call_credentials=None,
-                     insecure=False,
-                     compression=None,
-                     wait_for_ready=None,
-                     timeout=None,
-                     metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Sessions/ListSessions',
-                                             ondewo_dot_nlu_dot_session__pb2.ListSessionsRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_session__pb2.ListSessionsResponse.FromString,
+    def DeleteUser(request,
+                   target,
+                   options=(),
+                   channel_credentials=None,
+                   call_credentials=None,
+                   insecure=False,
+                   compression=None,
+                   wait_for_ready=None,
+                   timeout=None,
+                   metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/DeleteUser',
+                                             ondewo_dot_nlu_dot_user__pb2.GetUserRequest.SerializeToString,
+                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetSession(request,
+    def UpdateUser(request,
                    target,
                    options=(),
                    channel_credentials=None,
                    call_credentials=None,
                    insecure=False,
                    compression=None,
                    wait_for_ready=None,
                    timeout=None,
                    metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Sessions/GetSession',
-                                             ondewo_dot_nlu_dot_session__pb2.GetSessionRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_session__pb2.Session.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/UpdateUser',
+                                             ondewo_dot_nlu_dot_user__pb2.UpdateUserRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_user__pb2.User.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CreateSession(request,
+    def ListUsers(request,
+                  target,
+                  options=(),
+                  channel_credentials=None,
+                  call_credentials=None,
+                  insecure=False,
+                  compression=None,
+                  wait_for_ready=None,
+                  timeout=None,
+                  metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/ListUsers',
+                                             ondewo_dot_nlu_dot_user__pb2.ListUsersRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_user__pb2.ListUsersResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListUserInfos(request,
                       target,
                       options=(),
                       channel_credentials=None,
                       call_credentials=None,
                       insecure=False,
                       compression=None,
                       wait_for_ready=None,
                       timeout=None,
                       metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Sessions/CreateSession',
-                                             ondewo_dot_nlu_dot_session__pb2.CreateSessionRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_session__pb2.Session.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/ListUserInfos',
+                                             ondewo_dot_nlu_dot_user__pb2.ListUsersRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_user__pb2.ListUserInfosResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def TrackSessionStep(request,
+    def CreateServerRole(request,
                          target,
                          options=(),
                          channel_credentials=None,
                          call_credentials=None,
                          insecure=False,
                          compression=None,
                          wait_for_ready=None,
                          timeout=None,
                          metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Sessions/TrackSessionStep',
-                                             ondewo_dot_nlu_dot_session__pb2.TrackSessionStepRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_session__pb2.Session.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/CreateServerRole',
+                                             ondewo_dot_nlu_dot_user__pb2.CreateServerRoleRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_user__pb2.ServerRole.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def DeleteSession(request,
+    def GetServerRole(request,
                       target,
                       options=(),
                       channel_credentials=None,
                       call_credentials=None,
                       insecure=False,
                       compression=None,
                       wait_for_ready=None,
                       timeout=None,
                       metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Sessions/DeleteSession',
-                                             ondewo_dot_nlu_dot_session__pb2.DeleteSessionRequest.SerializeToString,
-                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/GetServerRole',
+                                             ondewo_dot_nlu_dot_user__pb2.GetServerRoleRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_user__pb2.ServerRole.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListSessionLabels(request,
-                          target,
-                          options=(),
-                          channel_credentials=None,
-                          call_credentials=None,
-                          insecure=False,
-                          compression=None,
-                          wait_for_ready=None,
-                          timeout=None,
-                          metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Sessions/ListSessionLabels',
-                                             ondewo_dot_nlu_dot_session__pb2.ListSessionLabelsRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_session__pb2.ListSessionLabelsResponse.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def AddSessionLabels(request,
+    def DeleteServerRole(request,
                          target,
                          options=(),
                          channel_credentials=None,
                          call_credentials=None,
                          insecure=False,
                          compression=None,
                          wait_for_ready=None,
                          timeout=None,
                          metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Sessions/AddSessionLabels',
-                                             ondewo_dot_nlu_dot_session__pb2.AddSessionLabelsRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_session__pb2.Session.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def RemoveSessionLabels(request,
-                            target,
-                            options=(),
-                            channel_credentials=None,
-                            call_credentials=None,
-                            insecure=False,
-                            compression=None,
-                            wait_for_ready=None,
-                            timeout=None,
-                            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Sessions/RemoveSessionLabels',
-                                             ondewo_dot_nlu_dot_session__pb2.RemoveSessionLabelsRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_session__pb2.Session.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ListSessionReviews(request,
-                           target,
-                           options=(),
-                           channel_credentials=None,
-                           call_credentials=None,
-                           insecure=False,
-                           compression=None,
-                           wait_for_ready=None,
-                           timeout=None,
-                           metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Sessions/ListSessionReviews',
-                                             ondewo_dot_nlu_dot_session__pb2.ListSessionReviewsRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_session__pb2.ListSessionReviewsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/DeleteServerRole',
+                                             ondewo_dot_nlu_dot_user__pb2.DeleteServerRoleRequest.SerializeToString,
+                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetSessionReview(request,
+    def UpdateServerRole(request,
                          target,
                          options=(),
                          channel_credentials=None,
                          call_credentials=None,
                          insecure=False,
                          compression=None,
                          wait_for_ready=None,
                          timeout=None,
                          metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Sessions/GetSessionReview',
-                                             ondewo_dot_nlu_dot_session__pb2.GetSessionReviewRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_session__pb2.SessionReview.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/UpdateServerRole',
+                                             ondewo_dot_nlu_dot_user__pb2.UpdateServerRoleRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_user__pb2.ServerRole.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListServerRoles(request,
+                        target,
+                        options=(),
+                        channel_credentials=None,
+                        call_credentials=None,
+                        insecure=False,
+                        compression=None,
+                        wait_for_ready=None,
+                        timeout=None,
+                        metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/ListServerRoles',
+                                             ondewo_dot_nlu_dot_user__pb2.ListServerRolesRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_user__pb2.ListServerRolesResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetLatestSessionReview(request,
-                               target,
-                               options=(),
-                               channel_credentials=None,
-                               call_credentials=None,
-                               insecure=False,
-                               compression=None,
-                               wait_for_ready=None,
-                               timeout=None,
-                               metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Sessions/GetLatestSessionReview',
-                                             ondewo_dot_nlu_dot_session__pb2.GetLatestSessionReviewRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_session__pb2.SessionReview.FromString,
+    def ListServerPermissions(request,
+                              target,
+                              options=(),
+                              channel_credentials=None,
+                              call_credentials=None,
+                              insecure=False,
+                              compression=None,
+                              wait_for_ready=None,
+                              timeout=None,
+                              metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/ListServerPermissions',
+                                             ondewo_dot_nlu_dot_user__pb2.ListServerPermissionsRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_user__pb2.ListServerPermissionsResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CreateSessionReview(request,
-                            target,
-                            options=(),
-                            channel_credentials=None,
-                            call_credentials=None,
-                            insecure=False,
-                            compression=None,
-                            wait_for_ready=None,
-                            timeout=None,
-                            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Sessions/CreateSessionReview',
-                                             ondewo_dot_nlu_dot_session__pb2.CreateSessionReviewRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_session__pb2.SessionReview.FromString,
+    def Login(request,
+              target,
+              options=(),
+              channel_credentials=None,
+              call_credentials=None,
+              insecure=False,
+              compression=None,
+              wait_for_ready=None,
+              timeout=None,
+              metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/Login',
+                                             ondewo_dot_nlu_dot_user__pb2.LoginRequest.SerializeToString,
+                                             ondewo_dot_nlu_dot_user__pb2.LoginResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CheckLogin(request,
+                   target,
+                   options=(),
+                   channel_credentials=None,
+                   call_credentials=None,
+                   insecure=False,
+                   compression=None,
+                   wait_for_ready=None,
+                   timeout=None,
+                   metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/CheckLogin',
+                                             google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/user_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/user_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/user_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/s2t/speech_to_text_pb2_grpc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,530 +1,552 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from ondewo.nlu import user_pb2 as ondewo_dot_nlu_dot_user__pb2
+from ondewo.s2t import speech_to_text_pb2 as ondewo_dot_s2t_dot_speech__to__text__pb2
 
 
-class UsersStub(object):
-    """Missing associated documentation comment in .proto file."""
+class Speech2TextStub(object):
+    """Speech-to-text service
+    """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.CreateUser = channel.unary_unary(
-            '/ondewo.nlu.Users/CreateUser',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.CreateUserRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_user__pb2.User.FromString,
-        )
-        self.GetUser = channel.unary_unary(
-            '/ondewo.nlu.Users/GetUser',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.GetUserRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_user__pb2.User.FromString,
-        )
-        self.GetUserInfo = channel.unary_unary(
-            '/ondewo.nlu.Users/GetUserInfo',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.GetUserRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_user__pb2.UserInfo.FromString,
-        )
-        self.DeleteUser = channel.unary_unary(
-            '/ondewo.nlu.Users/DeleteUser',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.GetUserRequest.SerializeToString,
+        self.TranscribeFile = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/TranscribeFile',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.TranscribeFileRequest.SerializeToString,
+            response_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.TranscribeFileResponse.FromString,
+        )
+        self.TranscribeStream = channel.stream_stream(
+            '/ondewo.s2t.Speech2Text/TranscribeStream',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.TranscribeStreamRequest.SerializeToString,
+            response_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.TranscribeStreamResponse.FromString,
+        )
+        self.GetS2tPipeline = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/GetS2tPipeline',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.S2tPipelineId.SerializeToString,
+            response_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.Speech2TextConfig.FromString,
+        )
+        self.CreateS2tPipeline = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/CreateS2tPipeline',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.Speech2TextConfig.SerializeToString,
+            response_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.S2tPipelineId.FromString,
+        )
+        self.DeleteS2tPipeline = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/DeleteS2tPipeline',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.S2tPipelineId.SerializeToString,
             response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
         )
-        self.UpdateUser = channel.unary_unary(
-            '/ondewo.nlu.Users/UpdateUser',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.UpdateUserRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_user__pb2.User.FromString,
-        )
-        self.ListUsers = channel.unary_unary(
-            '/ondewo.nlu.Users/ListUsers',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.ListUsersRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ListUsersResponse.FromString,
-        )
-        self.ListUserInfos = channel.unary_unary(
-            '/ondewo.nlu.Users/ListUserInfos',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.ListUsersRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ListUserInfosResponse.FromString,
-        )
-        self.CreateServerRole = channel.unary_unary(
-            '/ondewo.nlu.Users/CreateServerRole',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.CreateServerRoleRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ServerRole.FromString,
-        )
-        self.GetServerRole = channel.unary_unary(
-            '/ondewo.nlu.Users/GetServerRole',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.GetServerRoleRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ServerRole.FromString,
-        )
-        self.DeleteServerRole = channel.unary_unary(
-            '/ondewo.nlu.Users/DeleteServerRole',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.DeleteServerRoleRequest.SerializeToString,
+        self.UpdateS2tPipeline = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/UpdateS2tPipeline',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.Speech2TextConfig.SerializeToString,
             response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
         )
-        self.UpdateServerRole = channel.unary_unary(
-            '/ondewo.nlu.Users/UpdateServerRole',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.UpdateServerRoleRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ServerRole.FromString,
-        )
-        self.ListServerRoles = channel.unary_unary(
-            '/ondewo.nlu.Users/ListServerRoles',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.ListServerRolesRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ListServerRolesResponse.FromString,
-        )
-        self.ListServerPermissions = channel.unary_unary(
-            '/ondewo.nlu.Users/ListServerPermissions',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.ListServerPermissionsRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_user__pb2.ListServerPermissionsResponse.FromString,
-        )
-        self.Login = channel.unary_unary(
-            '/ondewo.nlu.Users/Login',
-            request_serializer=ondewo_dot_nlu_dot_user__pb2.LoginRequest.SerializeToString,
-            response_deserializer=ondewo_dot_nlu_dot_user__pb2.LoginResponse.FromString,
+        self.ListS2tPipelines = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/ListS2tPipelines',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tPipelinesRequest.SerializeToString,
+            response_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tPipelinesResponse.FromString,
+        )
+        self.ListS2tLanguages = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/ListS2tLanguages',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tLanguagesRequest.SerializeToString,
+            response_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tLanguagesResponse.FromString,
+        )
+        self.ListS2tDomains = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/ListS2tDomains',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tDomainsRequest.SerializeToString,
+            response_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tDomainsResponse.FromString,
         )
-        self.CheckLogin = channel.unary_unary(
-            '/ondewo.nlu.Users/CheckLogin',
+        self.GetServiceInfo = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/GetServiceInfo',
             request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            response_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.S2TGetServiceInfoResponse.FromString,
+        )
+        self.ListS2tLanguageModels = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/ListS2tLanguageModels',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tLanguageModelsRequest.SerializeToString,
+            response_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tLanguageModelsResponse.FromString,
+        )
+        self.CreateUserLanguageModel = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/CreateUserLanguageModel',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.CreateUserLanguageModelRequest.SerializeToString,
+            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        )
+        self.DeleteUserLanguageModel = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/DeleteUserLanguageModel',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.DeleteUserLanguageModelRequest.SerializeToString,
+            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        )
+        self.AddDataToUserLanguageModel = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/AddDataToUserLanguageModel',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.AddDataToUserLanguageModelRequest.SerializeToString,
+            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        )
+        self.TrainUserLanguageModel = channel.unary_unary(
+            '/ondewo.s2t.Speech2Text/TrainUserLanguageModel',
+            request_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.TrainUserLanguageModelRequest.SerializeToString,
             response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
         )
 
 
-class UsersServicer(object):
-    """Missing associated documentation comment in .proto file."""
+class Speech2TextServicer(object):
+    """Speech-to-text service
+    """
 
-    def CreateUser(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def TranscribeFile(self, request, context):
+        """Transcribes an audio file
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetUser(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def TranscribeStream(self, request_iterator, context):
+        """Transcribes an audio stream.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetUserInfo(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetS2tPipeline(self, request, context):
+        """Gets a speech to text pipeline corresponding to the id specified in S2tPipelineId. If no corresponding id is
+        found, raises ModuleNotFoundError in server.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeleteUser(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def CreateS2tPipeline(self, request, context):
+        """Creates a new speech to text pipeline from a Speech2TextConfig and registers the new pipeline in the server.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def UpdateUser(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def DeleteS2tPipeline(self, request, context):
+        """Deletes a pipeline corresponding to the id parsed in S2TPipelineId. If no corresponding id is
+        found, raises ModuleNotFoundError in server.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListUsers(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def UpdateS2tPipeline(self, request, context):
+        """Updates a pipeline with the id specified in Speech2TextConfig with the new config. If no corresponding id is
+        found, raises ModuleNotFoundError in server.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListUserInfos(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def ListS2tPipelines(self, request, context):
+        """Lists all speech to text pipelines.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CreateServerRole(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def ListS2tLanguages(self, request, context):
+        """Returns a message containing a list of all languages for which there exist pipelines.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetServerRole(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def ListS2tDomains(self, request, context):
+        """Returns a message containing a list of all domains for which there exist pipelines.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeleteServerRole(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetServiceInfo(self, request, context):
+        """Returns a message containing the version of the running speech to text server.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def UpdateServerRole(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def ListS2tLanguageModels(self, request, context):
+        """Given a list of pipeline ids, returns a list of LanguageModelPipelineId messages containing the pipeline
+        id and a list of the language models loaded in the pipeline.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListServerRoles(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def CreateUserLanguageModel(self, request, context):
+        """Create a user language model.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListServerPermissions(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def DeleteUserLanguageModel(self, request, context):
+        """Delete a user language model.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Login(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def AddDataToUserLanguageModel(self, request, context):
+        """Add data to a user language model.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CheckLogin(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def TrainUserLanguageModel(self, request, context):
+        """Train a user language model.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_UsersServicer_to_server(servicer, server):
+def add_Speech2TextServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        'CreateUser': grpc.unary_unary_rpc_method_handler(
-            servicer.CreateUser,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.CreateUserRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_user__pb2.User.SerializeToString,
-        ),
-        'GetUser': grpc.unary_unary_rpc_method_handler(
-            servicer.GetUser,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.GetUserRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_user__pb2.User.SerializeToString,
-        ),
-        'GetUserInfo': grpc.unary_unary_rpc_method_handler(
-            servicer.GetUserInfo,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.GetUserRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_user__pb2.UserInfo.SerializeToString,
-        ),
-        'DeleteUser': grpc.unary_unary_rpc_method_handler(
-            servicer.DeleteUser,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.GetUserRequest.FromString,
+        'TranscribeFile': grpc.unary_unary_rpc_method_handler(
+            servicer.TranscribeFile,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.TranscribeFileRequest.FromString,
+            response_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.TranscribeFileResponse.SerializeToString,
+        ),
+        'TranscribeStream': grpc.stream_stream_rpc_method_handler(
+            servicer.TranscribeStream,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.TranscribeStreamRequest.FromString,
+            response_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.TranscribeStreamResponse.SerializeToString,
+        ),
+        'GetS2tPipeline': grpc.unary_unary_rpc_method_handler(
+            servicer.GetS2tPipeline,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.S2tPipelineId.FromString,
+            response_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.Speech2TextConfig.SerializeToString,
+        ),
+        'CreateS2tPipeline': grpc.unary_unary_rpc_method_handler(
+            servicer.CreateS2tPipeline,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.Speech2TextConfig.FromString,
+            response_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.S2tPipelineId.SerializeToString,
+        ),
+        'DeleteS2tPipeline': grpc.unary_unary_rpc_method_handler(
+            servicer.DeleteS2tPipeline,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.S2tPipelineId.FromString,
             response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
         ),
-        'UpdateUser': grpc.unary_unary_rpc_method_handler(
-            servicer.UpdateUser,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.UpdateUserRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_user__pb2.User.SerializeToString,
-        ),
-        'ListUsers': grpc.unary_unary_rpc_method_handler(
-            servicer.ListUsers,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.ListUsersRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_user__pb2.ListUsersResponse.SerializeToString,
-        ),
-        'ListUserInfos': grpc.unary_unary_rpc_method_handler(
-            servicer.ListUserInfos,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.ListUsersRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_user__pb2.ListUserInfosResponse.SerializeToString,
-        ),
-        'CreateServerRole': grpc.unary_unary_rpc_method_handler(
-            servicer.CreateServerRole,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.CreateServerRoleRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_user__pb2.ServerRole.SerializeToString,
-        ),
-        'GetServerRole': grpc.unary_unary_rpc_method_handler(
-            servicer.GetServerRole,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.GetServerRoleRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_user__pb2.ServerRole.SerializeToString,
-        ),
-        'DeleteServerRole': grpc.unary_unary_rpc_method_handler(
-            servicer.DeleteServerRole,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.DeleteServerRoleRequest.FromString,
+        'UpdateS2tPipeline': grpc.unary_unary_rpc_method_handler(
+            servicer.UpdateS2tPipeline,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.Speech2TextConfig.FromString,
             response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
         ),
-        'UpdateServerRole': grpc.unary_unary_rpc_method_handler(
-            servicer.UpdateServerRole,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.UpdateServerRoleRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_user__pb2.ServerRole.SerializeToString,
-        ),
-        'ListServerRoles': grpc.unary_unary_rpc_method_handler(
-            servicer.ListServerRoles,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.ListServerRolesRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_user__pb2.ListServerRolesResponse.SerializeToString,
-        ),
-        'ListServerPermissions': grpc.unary_unary_rpc_method_handler(
-            servicer.ListServerPermissions,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.ListServerPermissionsRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_user__pb2.ListServerPermissionsResponse.SerializeToString,
-        ),
-        'Login': grpc.unary_unary_rpc_method_handler(
-            servicer.Login,
-            request_deserializer=ondewo_dot_nlu_dot_user__pb2.LoginRequest.FromString,
-            response_serializer=ondewo_dot_nlu_dot_user__pb2.LoginResponse.SerializeToString,
+        'ListS2tPipelines': grpc.unary_unary_rpc_method_handler(
+            servicer.ListS2tPipelines,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tPipelinesRequest.FromString,
+            response_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tPipelinesResponse.SerializeToString,
+        ),
+        'ListS2tLanguages': grpc.unary_unary_rpc_method_handler(
+            servicer.ListS2tLanguages,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tLanguagesRequest.FromString,
+            response_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tLanguagesResponse.SerializeToString,
+        ),
+        'ListS2tDomains': grpc.unary_unary_rpc_method_handler(
+            servicer.ListS2tDomains,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tDomainsRequest.FromString,
+            response_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tDomainsResponse.SerializeToString,
         ),
-        'CheckLogin': grpc.unary_unary_rpc_method_handler(
-            servicer.CheckLogin,
+        'GetServiceInfo': grpc.unary_unary_rpc_method_handler(
+            servicer.GetServiceInfo,
             request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            response_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.S2TGetServiceInfoResponse.SerializeToString,
+        ),
+        'ListS2tLanguageModels': grpc.unary_unary_rpc_method_handler(
+            servicer.ListS2tLanguageModels,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tLanguageModelsRequest.FromString,
+            response_serializer=ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tLanguageModelsResponse.SerializeToString,
+        ),
+        'CreateUserLanguageModel': grpc.unary_unary_rpc_method_handler(
+            servicer.CreateUserLanguageModel,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.CreateUserLanguageModelRequest.FromString,
+            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+        ),
+        'DeleteUserLanguageModel': grpc.unary_unary_rpc_method_handler(
+            servicer.DeleteUserLanguageModel,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.DeleteUserLanguageModelRequest.FromString,
+            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+        ),
+        'AddDataToUserLanguageModel': grpc.unary_unary_rpc_method_handler(
+            servicer.AddDataToUserLanguageModel,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.AddDataToUserLanguageModelRequest.FromString,
+            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+        ),
+        'TrainUserLanguageModel': grpc.unary_unary_rpc_method_handler(
+            servicer.TrainUserLanguageModel,
+            request_deserializer=ondewo_dot_s2t_dot_speech__to__text__pb2.TrainUserLanguageModelRequest.FromString,
             response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        'ondewo.nlu.Users', rpc_method_handlers)
+        'ondewo.s2t.Speech2Text', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
  # This class is part of an EXPERIMENTAL API.
 
 
-class Users(object):
-    """Missing associated documentation comment in .proto file."""
-
-    @staticmethod
-    def CreateUser(request,
-                   target,
-                   options=(),
-                   channel_credentials=None,
-                   call_credentials=None,
-                   insecure=False,
-                   compression=None,
-                   wait_for_ready=None,
-                   timeout=None,
-                   metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/CreateUser',
-                                             ondewo_dot_nlu_dot_user__pb2.CreateUserRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_user__pb2.User.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetUser(request,
-                target,
-                options=(),
-                channel_credentials=None,
-                call_credentials=None,
-                insecure=False,
-                compression=None,
-                wait_for_ready=None,
-                timeout=None,
-                metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/GetUser',
-                                             ondewo_dot_nlu_dot_user__pb2.GetUserRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_user__pb2.User.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetUserInfo(request,
-                    target,
-                    options=(),
-                    channel_credentials=None,
-                    call_credentials=None,
-                    insecure=False,
-                    compression=None,
-                    wait_for_ready=None,
-                    timeout=None,
-                    metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/GetUserInfo',
-                                             ondewo_dot_nlu_dot_user__pb2.GetUserRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_user__pb2.UserInfo.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def DeleteUser(request,
-                   target,
-                   options=(),
-                   channel_credentials=None,
-                   call_credentials=None,
-                   insecure=False,
-                   compression=None,
-                   wait_for_ready=None,
-                   timeout=None,
-                   metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/DeleteUser',
-                                             ondewo_dot_nlu_dot_user__pb2.GetUserRequest.SerializeToString,
-                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def UpdateUser(request,
-                   target,
-                   options=(),
-                   channel_credentials=None,
-                   call_credentials=None,
-                   insecure=False,
-                   compression=None,
-                   wait_for_ready=None,
-                   timeout=None,
-                   metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/UpdateUser',
-                                             ondewo_dot_nlu_dot_user__pb2.UpdateUserRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_user__pb2.User.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ListUsers(request,
-                  target,
-                  options=(),
-                  channel_credentials=None,
-                  call_credentials=None,
-                  insecure=False,
-                  compression=None,
-                  wait_for_ready=None,
-                  timeout=None,
-                  metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/ListUsers',
-                                             ondewo_dot_nlu_dot_user__pb2.ListUsersRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_user__pb2.ListUsersResponse.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+class Speech2Text(object):
+    """Speech-to-text service
+    """
 
     @staticmethod
-    def ListUserInfos(request,
-                      target,
-                      options=(),
-                      channel_credentials=None,
-                      call_credentials=None,
-                      insecure=False,
-                      compression=None,
-                      wait_for_ready=None,
-                      timeout=None,
-                      metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/ListUserInfos',
-                                             ondewo_dot_nlu_dot_user__pb2.ListUsersRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_user__pb2.ListUserInfosResponse.FromString,
+    def TranscribeFile(request,
+                       target,
+                       options=(),
+                       channel_credentials=None,
+                       call_credentials=None,
+                       insecure=False,
+                       compression=None,
+                       wait_for_ready=None,
+                       timeout=None,
+                       metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/TranscribeFile',
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.TranscribeFileRequest.SerializeToString,
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.TranscribeFileResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CreateServerRole(request,
+    def TranscribeStream(request_iterator,
                          target,
                          options=(),
                          channel_credentials=None,
                          call_credentials=None,
                          insecure=False,
                          compression=None,
                          wait_for_ready=None,
                          timeout=None,
                          metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/CreateServerRole',
-                                             ondewo_dot_nlu_dot_user__pb2.CreateServerRoleRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_user__pb2.ServerRole.FromString,
+        return grpc.experimental.stream_stream(request_iterator, target, '/ondewo.s2t.Speech2Text/TranscribeStream',
+                                               ondewo_dot_s2t_dot_speech__to__text__pb2.TranscribeStreamRequest.SerializeToString,
+                                               ondewo_dot_s2t_dot_speech__to__text__pb2.TranscribeStreamResponse.FromString,
+                                               options, channel_credentials,
+                                               insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetS2tPipeline(request,
+                       target,
+                       options=(),
+                       channel_credentials=None,
+                       call_credentials=None,
+                       insecure=False,
+                       compression=None,
+                       wait_for_ready=None,
+                       timeout=None,
+                       metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/GetS2tPipeline',
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.S2tPipelineId.SerializeToString,
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.Speech2TextConfig.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CreateS2tPipeline(request,
+                          target,
+                          options=(),
+                          channel_credentials=None,
+                          call_credentials=None,
+                          insecure=False,
+                          compression=None,
+                          wait_for_ready=None,
+                          timeout=None,
+                          metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/CreateS2tPipeline',
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.Speech2TextConfig.SerializeToString,
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.S2tPipelineId.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetServerRole(request,
-                      target,
-                      options=(),
-                      channel_credentials=None,
-                      call_credentials=None,
-                      insecure=False,
-                      compression=None,
-                      wait_for_ready=None,
-                      timeout=None,
-                      metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/GetServerRole',
-                                             ondewo_dot_nlu_dot_user__pb2.GetServerRoleRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_user__pb2.ServerRole.FromString,
+    def DeleteS2tPipeline(request,
+                          target,
+                          options=(),
+                          channel_credentials=None,
+                          call_credentials=None,
+                          insecure=False,
+                          compression=None,
+                          wait_for_ready=None,
+                          timeout=None,
+                          metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/DeleteS2tPipeline',
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.S2tPipelineId.SerializeToString,
+                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def DeleteServerRole(request,
+    def UpdateS2tPipeline(request,
+                          target,
+                          options=(),
+                          channel_credentials=None,
+                          call_credentials=None,
+                          insecure=False,
+                          compression=None,
+                          wait_for_ready=None,
+                          timeout=None,
+                          metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/UpdateS2tPipeline',
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.Speech2TextConfig.SerializeToString,
+                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListS2tPipelines(request,
                          target,
                          options=(),
                          channel_credentials=None,
                          call_credentials=None,
                          insecure=False,
                          compression=None,
                          wait_for_ready=None,
                          timeout=None,
                          metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/DeleteServerRole',
-                                             ondewo_dot_nlu_dot_user__pb2.DeleteServerRoleRequest.SerializeToString,
-                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/ListS2tPipelines',
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tPipelinesRequest.SerializeToString,
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tPipelinesResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def UpdateServerRole(request,
+    def ListS2tLanguages(request,
                          target,
                          options=(),
                          channel_credentials=None,
                          call_credentials=None,
                          insecure=False,
                          compression=None,
                          wait_for_ready=None,
                          timeout=None,
                          metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/UpdateServerRole',
-                                             ondewo_dot_nlu_dot_user__pb2.UpdateServerRoleRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_user__pb2.ServerRole.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/ListS2tLanguages',
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tLanguagesRequest.SerializeToString,
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tLanguagesResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListServerRoles(request,
-                        target,
-                        options=(),
-                        channel_credentials=None,
-                        call_credentials=None,
-                        insecure=False,
-                        compression=None,
-                        wait_for_ready=None,
-                        timeout=None,
-                        metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/ListServerRoles',
-                                             ondewo_dot_nlu_dot_user__pb2.ListServerRolesRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_user__pb2.ListServerRolesResponse.FromString,
+    def ListS2tDomains(request,
+                       target,
+                       options=(),
+                       channel_credentials=None,
+                       call_credentials=None,
+                       insecure=False,
+                       compression=None,
+                       wait_for_ready=None,
+                       timeout=None,
+                       metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/ListS2tDomains',
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tDomainsRequest.SerializeToString,
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tDomainsResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListServerPermissions(request,
+    def GetServiceInfo(request,
+                       target,
+                       options=(),
+                       channel_credentials=None,
+                       call_credentials=None,
+                       insecure=False,
+                       compression=None,
+                       wait_for_ready=None,
+                       timeout=None,
+                       metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/GetServiceInfo',
+                                             google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.S2TGetServiceInfoResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListS2tLanguageModels(request,
                               target,
                               options=(),
                               channel_credentials=None,
                               call_credentials=None,
                               insecure=False,
                               compression=None,
                               wait_for_ready=None,
                               timeout=None,
                               metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/ListServerPermissions',
-                                             ondewo_dot_nlu_dot_user__pb2.ListServerPermissionsRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_user__pb2.ListServerPermissionsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/ListS2tLanguageModels',
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tLanguageModelsRequest.SerializeToString,
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.ListS2tLanguageModelsResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Login(request,
-              target,
-              options=(),
-              channel_credentials=None,
-              call_credentials=None,
-              insecure=False,
-              compression=None,
-              wait_for_ready=None,
-              timeout=None,
-              metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/Login',
-                                             ondewo_dot_nlu_dot_user__pb2.LoginRequest.SerializeToString,
-                                             ondewo_dot_nlu_dot_user__pb2.LoginResponse.FromString,
+    def CreateUserLanguageModel(request,
+                                target,
+                                options=(),
+                                channel_credentials=None,
+                                call_credentials=None,
+                                insecure=False,
+                                compression=None,
+                                wait_for_ready=None,
+                                timeout=None,
+                                metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/CreateUserLanguageModel',
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.CreateUserLanguageModelRequest.SerializeToString,
+                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CheckLogin(request,
-                   target,
-                   options=(),
-                   channel_credentials=None,
-                   call_credentials=None,
-                   insecure=False,
-                   compression=None,
-                   wait_for_ready=None,
-                   timeout=None,
-                   metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.nlu.Users/CheckLogin',
-                                             google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+    def DeleteUserLanguageModel(request,
+                                target,
+                                options=(),
+                                channel_credentials=None,
+                                call_credentials=None,
+                                insecure=False,
+                                compression=None,
+                                wait_for_ready=None,
+                                timeout=None,
+                                metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/DeleteUserLanguageModel',
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.DeleteUserLanguageModelRequest.SerializeToString,
+                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def AddDataToUserLanguageModel(request,
+                                   target,
+                                   options=(),
+                                   channel_credentials=None,
+                                   call_credentials=None,
+                                   insecure=False,
+                                   compression=None,
+                                   wait_for_ready=None,
+                                   timeout=None,
+                                   metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/AddDataToUserLanguageModel',
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.AddDataToUserLanguageModelRequest.SerializeToString,
+                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def TrainUserLanguageModel(request,
+                               target,
+                               options=(),
+                               channel_credentials=None,
+                               call_credentials=None,
+                               insecure=False,
+                               compression=None,
+                               wait_for_ready=None,
+                               timeout=None,
+                               metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.s2t.Speech2Text/TrainUserLanguageModel',
+                                             ondewo_dot_s2t_dot_speech__to__text__pb2.TrainUserLanguageModelRequest.SerializeToString,
                                              google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/utility_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/utility_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/utility_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/utility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/webhook_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/webhook_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/nlu/webhook_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/nlu/webhook_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         context information can be changed by the webhook server
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Ping(self, request, context):
-        """send a Ping to the webhook server to check server health
+        """send a Ping to the webhook server to verify server health
         will return True if http status_code==200 is detected in the response
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/qa/qa_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/qa/qa_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/qa/qa_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/qa/qa_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import grpc
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from ondewo.qa import qa_pb2 as ondewo_dot_qa_dot_qa__pb2
 
 
 class QAStub(object):
-    """///// Services ///////
-
+    """///// Question Answering (QA) Services ///////
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -51,16 +50,15 @@
             '/ondewo.qa.QA/GetProjectConfig',
             request_serializer=ondewo_dot_qa_dot_qa__pb2.GetProjectConfigRequest.SerializeToString,
             response_deserializer=ondewo_dot_qa_dot_qa__pb2.GetProjectConfigResponse.FromString,
         )
 
 
 class QAServicer(object):
-    """///// Services ///////
-
+    """///// Question Answering (QA) Services ///////
     """
 
     def GetAnswer(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
@@ -144,16 +142,15 @@
         'ondewo.qa.QA', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
  # This class is part of an EXPERIMENTAL API.
 
 
 class QA(object):
-    """///// Services ///////
-
+    """///// Question Answering (QA) Services ///////
     """
 
     @staticmethod
     def GetAnswer(request,
                   target,
                   options=(),
                   channel_credentials=None,
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/s2t/speech_to_text_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/s2t/speech_to_text_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,45 +10,55 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fondewo/s2t/speech-to-text.proto\x12\nondewo.s2t\x1a\x1bgoogle/protobuf/empty.proto\"\xa1\x04\n\x17TranscribeRequestConfig\x12\x17\n\x0fs2t_pipeline_id\x18\x01 \x01(\t\x12-\n\x0c\x63tc_decoding\x18\x02 \x01(\x0e\x32\x17.ondewo.s2t.CTCDecoding\x12\x1d\n\x13language_model_name\x18\x03 \x01(\tH\x00\x12<\n\x0fpost_processing\x18\x04 \x01(\x0b\x32!.ondewo.s2t.PostProcessingOptionsH\x01\x12\x44\n\x13utterance_detection\x18\x05 \x01(\x0b\x32%.ondewo.s2t.UtteranceDetectionOptionsH\x02\x12(\n\x08pyannote\x18\x06 \x01(\x0b\x32\x14.ondewo.s2t.PyannoteH\x03\x12(\n\x08matchbox\x18\x07 \x01(\x0b\x32\x14.ondewo.s2t.MatchboxH\x03\x12@\n\x0ereturn_options\x18\x08 \x01(\x0b\x32&.ondewo.s2t.TranscriptionReturnOptionsH\x04\x42\x1b\n\x19oneof_language_model_nameB\x17\n\x15oneof_post_processingB\x1b\n\x19oneof_utterance_detectionB\x1a\n\x18voice_activity_detectionB\x16\n\x14oneof_return_options\"\xba\x01\n\x1aTranscriptionReturnOptions\x12\x1e\n\x16return_start_of_speech\x18\x01 \x01(\x08\x12\x14\n\x0creturn_audio\x18\x02 \x01(\x08\x12)\n!return_alternative_transcriptions\x18\x03 \x01(\x08\x12\x1f\n\x17return_confidence_score\x18\x04 \x01(\x08\x12\x1a\n\x12return_word_timing\x18\x08 \x01(\x08\"\xbf\x01\n\x19UtteranceDetectionOptions\x12\x1e\n\x14transcribe_not_final\x18\x01 \x01(\x08H\x00\x12$\n\x1cstart_of_utterance_threshold\x18\x02 \x01(\x02\x12\"\n\x1a\x65nd_of_utterance_threshold\x18\x03 \x01(\x02\x12\x1a\n\x12next_chunk_timeout\x18\x04 \x01(\x02\x42\x1c\n\x1aoneof_transcribe_not_final\"s\n\x15PostProcessingOptions\x12\x1b\n\x13spelling_correction\x18\x01 \x01(\x08\x12\x11\n\tnormalize\x18\x02 \x01(\x08\x12*\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessing\"\x8e\x01\n\x17TranscribeStreamRequest\x12\x13\n\x0b\x61udio_chunk\x18\x01 \x01(\x0c\x12\x15\n\rend_of_stream\x18\x02 \x01(\x08\x12\x33\n\x06\x63onfig\x18\x03 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\x12\x12\n\nmute_audio\x18\x04 \x01(\x08\"@\n\rTranscription\x12\x15\n\rtranscription\x18\x01 \x01(\t\x12\x18\n\x10\x63onfidence_score\x18\x02 \x01(\x02\"\x83\x02\n\x18TranscribeStreamResponse\x12\x31\n\x0etranscriptions\x18\x01 \x03(\x0b\x32\x19.ondewo.s2t.Transcription\x12\x0c\n\x04time\x18\x02 \x01(\x02\x12\r\n\x05\x66inal\x18\x03 \x01(\x08\x12\x14\n\x0creturn_audio\x18\x04 \x01(\x08\x12\r\n\x05\x61udio\x18\x05 \x01(\x0c\x12\x17\n\x0futterance_start\x18\x06 \x01(\x08\x12\x12\n\naudio_uuid\x18\x07 \x01(\t\x12\x35\n\x06\x63onfig\x18\x08 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfigH\x00\x42\x0e\n\x0coneof_config\"`\n\x15TranscribeFileRequest\x12\x12\n\naudio_file\x18\x01 \x01(\x0c\x12\x33\n\x06\x63onfig\x18\x02 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\"\x9a\x01\n\x16TranscribeFileResponse\x12\x31\n\x0etranscriptions\x18\x01 \x03(\x0b\x32\x19.ondewo.s2t.Transcription\x12\x0c\n\x04time\x18\x02 \x01(\x02\x12+\n\x0bword_timing\x18\x03 \x03(\x0b\x32\x16.ondewo.s2t.WordTiming\x12\x12\n\naudio_uuid\x18\x04 \x01(\t\"6\n\nWordTiming\x12\x0c\n\x04word\x18\x01 \x01(\t\x12\r\n\x05\x62\x65gin\x18\x02 \x01(\x05\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x05\"\x1b\n\rS2tPipelineId\x12\n\n\x02id\x18\x01 \x01(\t\"o\n\x17ListS2tPipelinesRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\x12\x0f\n\x07\x64omains\x18\x03 \x03(\t\x12\x17\n\x0fregistered_only\x18\x04 \x01(\x08\"S\n\x18ListS2tPipelinesResponse\x12\x37\n\x10pipeline_configs\x18\x01 \x03(\x0b\x32\x1d.ondewo.s2t.Speech2TextConfig\"C\n\x17ListS2tLanguagesRequest\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\"-\n\x18ListS2tLanguagesResponse\x12\x11\n\tlanguages\x18\x01 \x03(\t\"C\n\x15ListS2tDomainsRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\")\n\x16ListS2tDomainsResponse\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\",\n\x19S2TGetServiceInfoResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"\xe5\x02\n\x11Speech2TextConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12/\n\x0b\x64\x65scription\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.S2TDescription\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\x12+\n\tinference\x18\x04 \x01(\x0b\x32\x18.ondewo.s2t.S2TInference\x12\x35\n\x10streaming_server\x18\x05 \x01(\x0b\x32\x1b.ondewo.s2t.StreamingServer\x12\x44\n\x18voice_activity_detection\x18\x06 \x01(\x0b\x32\".ondewo.s2t.VoiceActivityDetection\x12\x33\n\x0fpost_processing\x18\x07 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessing\x12$\n\x07logging\x18\x08 \x01(\x0b\x32\x13.ondewo.s2t.Logging\"\\\n\x0eS2TDescription\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x16\n\x0epipeline_owner\x18\x02 \x01(\t\x12\x0e\n\x06\x64omain\x18\x03 \x01(\t\x12\x10\n\x08\x63omments\x18\x04 \x01(\t\"\x7f\n\x0cS2TInference\x12:\n\x13\x63tc_acoustic_models\x18\x01 \x01(\x0b\x32\x1d.ondewo.s2t.CtcAcousticModels\x12\x33\n\x0flanguage_models\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.LanguageModels\"\xdb\x01\n\x11\x43tcAcousticModels\x12\x0c\n\x04type\x18\x01 \x01(\t\x12(\n\tquartznet\x18\x02 \x01(\x0b\x32\x15.ondewo.s2t.Quartznet\x12\x35\n\x10quartznet_triton\x18\x03 \x01(\x0b\x32\x1b.ondewo.s2t.QuartznetTriton\x12$\n\x07wav2vec\x18\x04 \x01(\x0b\x32\x13.ondewo.s2t.Wav2Vec\x12\x31\n\x0ewav2vec_triton\x18\x05 \x01(\x0b\x32\x19.ondewo.s2t.Wav2VecTriton\".\n\x07Wav2Vec\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\"~\n\rWav2VecTriton\x12\x16\n\x0eprocessor_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\x12\x1c\n\x14triton_model_version\x18\x03 \x01(\t\x12\x1c\n\x14\x63heck_status_timeout\x18\x04 \x01(\x03\"\x94\x01\n\tQuartznet\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x11\n\tload_type\x18\x02 \x01(\t\x12%\n\x08pt_files\x18\x03 \x01(\x0b\x32\x13.ondewo.s2t.PtFiles\x12\'\n\tckpt_file\x18\x04 \x01(\x0b\x32\x14.ondewo.s2t.CkptFile\x12\x0f\n\x07use_gpu\x18\x05 \x01(\x08\"%\n\x07PtFiles\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0c\n\x04step\x18\x02 \x01(\t\"\x18\n\x08\x43kptFile\x12\x0c\n\x04path\x18\x01 \x01(\t\"P\n\x0fQuartznetTriton\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x12\n\ntriton_url\x18\x02 \x01(\t\x12\x14\n\x0ctriton_model\x18\x03 \x01(\t\"\x88\x01\n\x0eLanguageModels\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tbeam_size\x18\x02 \x01(\x03\x12\x12\n\ndefault_lm\x18\x03 \x01(\t\x12 \n\x18\x62\x65\x61m_search_scorer_alpha\x18\x04 \x01(\x02\x12\x1f\n\x17\x62\x65\x61m_search_scorer_beta\x18\x05 \x01(\x02\"\x91\x01\n\x0fStreamingServer\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x03\x12\x14\n\x0coutput_style\x18\x03 \x01(\t\x12L\n\x1cstreaming_speech_recognition\x18\x04 \x01(\x0b\x32&.ondewo.s2t.StreamingSpeechRecognition\"\xf2\x01\n\x1aStreamingSpeechRecognition\x12\x1c\n\x14transcribe_not_final\x18\x01 \x01(\x08\x12\x1b\n\x13\x63tc_decoding_method\x18\x02 \x01(\t\x12\x15\n\rsampling_rate\x18\x03 \x01(\x03\x12\x1c\n\x14min_audio_chunk_size\x18\x04 \x01(\x03\x12$\n\x1cstart_of_utterance_threshold\x18\x05 \x01(\x02\x12\"\n\x1a\x65nd_of_utterance_threshold\x18\x06 \x01(\x02\x12\x1a\n\x12next_chunk_timeout\x18\x07 \x01(\x02\"\x8f\x01\n\x16VoiceActivityDetection\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\t\x12\x15\n\rsampling_rate\x18\x02 \x01(\x03\x12&\n\x08pyannote\x18\x03 \x01(\x0b\x32\x14.ondewo.s2t.Pyannote\x12&\n\x08matchbox\x18\x04 \x01(\x0b\x32\x14.ondewo.s2t.Matchbox\"\xb0\x01\n\x08Pyannote\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x16\n\x0emin_audio_size\x18\x02 \x01(\x03\x12\x0e\n\x06offset\x18\x03 \x01(\x02\x12\r\n\x05onset\x18\x04 \x01(\x02\x12\x13\n\tlog_scale\x18\x05 \x01(\x08H\x00\x12\x18\n\x10min_duration_off\x18\x06 \x01(\x02\x12\x17\n\x0fmin_duration_on\x18\x07 \x01(\x02\x42\x11\n\x0foneof_log_scale\"L\n\x08Matchbox\x12\x14\n\x0cmodel_config\x18\x01 \x01(\t\x12\x14\n\x0c\x65ncoder_path\x18\x02 \x01(\t\x12\x14\n\x0c\x64\x65\x63oder_path\x18\x03 \x01(\t\"W\n\x0ePostProcessing\x12\x10\n\x08pipeline\x18\x01 \x03(\t\x12\x33\n\x0fpost_processors\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessors\"n\n\x0ePostProcessors\x12\'\n\tsym_spell\x18\x01 \x01(\x0b\x32\x14.ondewo.s2t.SymSpell\x12\x33\n\rnormalization\x18\x02 \x01(\x0b\x32\x1c.ondewo.s2t.S2TNormalization\"Z\n\x08SymSpell\x12\x11\n\tdict_path\x18\x01 \x01(\t\x12$\n\x1cmax_dictionary_edit_distance\x18\x02 \x01(\x03\x12\x15\n\rprefix_length\x18\x03 \x01(\x03\"$\n\x10S2TNormalization\x12\x10\n\x08language\x18\x01 \x01(\t\"%\n\x07Logging\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"+\n\x1cListS2tLanguageModelsRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"C\n\x17LanguageModelPipelineId\x12\x13\n\x0bpipeline_id\x18\x01 \x01(\t\x12\x13\n\x0bmodel_names\x18\x02 \x03(\t\"]\n\x1dListS2tLanguageModelsResponse\x12<\n\x0flm_pipeline_ids\x18\x01 \x03(\x0b\x32#.ondewo.s2t.LanguageModelPipelineId\"=\n\x1e\x43reateUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\"=\n\x1e\x44\x65leteUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\"U\n!AddDataToUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\x12\x13\n\x0bzipped_data\x18\x02 \x01(\x0c\"K\n\x1dTrainUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\x03*?\n\x0b\x43TCDecoding\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06GREEDY\x10\x01\x12\x17\n\x13\x42\x45\x41M_SEARCH_WITH_LM\x10\x02\x32\xec\n\n\x0bSpeech2Text\x12Y\n\x0eTranscribeFile\x12!.ondewo.s2t.TranscribeFileRequest\x1a\".ondewo.s2t.TranscribeFileResponse\"\x00\x12\x63\n\x10TranscribeStream\x12#.ondewo.s2t.TranscribeStreamRequest\x1a$.ondewo.s2t.TranscribeStreamResponse\"\x00(\x01\x30\x01\x12L\n\x0eGetS2tPipeline\x12\x19.ondewo.s2t.S2tPipelineId\x1a\x1d.ondewo.s2t.Speech2TextConfig\"\x00\x12O\n\x11\x43reateS2tPipeline\x12\x1d.ondewo.s2t.Speech2TextConfig\x1a\x19.ondewo.s2t.S2tPipelineId\"\x00\x12H\n\x11\x44\x65leteS2tPipeline\x12\x19.ondewo.s2t.S2tPipelineId\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x11UpdateS2tPipeline\x12\x1d.ondewo.s2t.Speech2TextConfig\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x10ListS2tPipelines\x12#.ondewo.s2t.ListS2tPipelinesRequest\x1a$.ondewo.s2t.ListS2tPipelinesResponse\"\x00\x12_\n\x10ListS2tLanguages\x12#.ondewo.s2t.ListS2tLanguagesRequest\x1a$.ondewo.s2t.ListS2tLanguagesResponse\"\x00\x12Y\n\x0eListS2tDomains\x12!.ondewo.s2t.ListS2tDomainsRequest\x1a\".ondewo.s2t.ListS2tDomainsResponse\"\x00\x12Q\n\x0eGetServiceInfo\x12\x16.google.protobuf.Empty\x1a%.ondewo.s2t.S2TGetServiceInfoResponse\"\x00\x12n\n\x15ListS2tLanguageModels\x12(.ondewo.s2t.ListS2tLanguageModelsRequest\x1a).ondewo.s2t.ListS2tLanguageModelsResponse\"\x00\x12_\n\x17\x43reateUserLanguageModel\x12*.ondewo.s2t.CreateUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x17\x44\x65leteUserLanguageModel\x12*.ondewo.s2t.DeleteUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x65\n\x1a\x41\x64\x64\x44\x61taToUserLanguageModel\x12-.ondewo.s2t.AddDataToUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12]\n\x16TrainUserLanguageModel\x12).ondewo.s2t.TrainUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fondewo/s2t/speech-to-text.proto\x12\nondewo.s2t\x1a\x1bgoogle/protobuf/empty.proto\"\x9a\x04\n\x17TranscribeRequestConfig\x12\x17\n\x0fs2t_pipeline_id\x18\x01 \x01(\t\x12&\n\x08\x64\x65\x63oding\x18\x02 \x01(\x0e\x32\x14.ondewo.s2t.Decoding\x12\x1d\n\x13language_model_name\x18\x03 \x01(\tH\x00\x12<\n\x0fpost_processing\x18\x04 \x01(\x0b\x32!.ondewo.s2t.PostProcessingOptionsH\x01\x12\x44\n\x13utterance_detection\x18\x05 \x01(\x0b\x32%.ondewo.s2t.UtteranceDetectionOptionsH\x02\x12(\n\x08pyannote\x18\x06 \x01(\x0b\x32\x14.ondewo.s2t.PyannoteH\x03\x12(\n\x08matchbox\x18\x07 \x01(\x0b\x32\x14.ondewo.s2t.MatchboxH\x03\x12@\n\x0ereturn_options\x18\x08 \x01(\x0b\x32&.ondewo.s2t.TranscriptionReturnOptionsH\x04\x42\x1b\n\x19oneof_language_model_nameB\x17\n\x15oneof_post_processingB\x1b\n\x19oneof_utterance_detectionB\x1a\n\x18voice_activity_detectionB\x16\n\x14oneof_return_options\"\xaf\x02\n\x1aTranscriptionReturnOptions\x12\x1e\n\x16return_start_of_speech\x18\x01 \x01(\x08\x12\x14\n\x0creturn_audio\x18\x02 \x01(\x08\x12\x1f\n\x17return_confidence_score\x18\x03 \x01(\x08\x12)\n!return_alternative_transcriptions\x18\x04 \x01(\x08\x12,\n$return_alternative_transcriptions_nr\x18\x05 \x01(\x05\x12 \n\x18return_alternative_words\x18\x06 \x01(\x08\x12#\n\x1breturn_alternative_words_nr\x18\x07 \x01(\x05\x12\x1a\n\x12return_word_timing\x18\x08 \x01(\x08\"\xbf\x01\n\x19UtteranceDetectionOptions\x12\x1e\n\x14transcribe_not_final\x18\x01 \x01(\x08H\x00\x12$\n\x1cstart_of_utterance_threshold\x18\x02 \x01(\x02\x12\"\n\x1a\x65nd_of_utterance_threshold\x18\x03 \x01(\x02\x12\x1a\n\x12next_chunk_timeout\x18\x04 \x01(\x02\x42\x1c\n\x1aoneof_transcribe_not_final\"s\n\x15PostProcessingOptions\x12\x1b\n\x13spelling_correction\x18\x01 \x01(\x08\x12\x11\n\tnormalize\x18\x02 \x01(\x08\x12*\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessing\"\xa3\x01\n\rTranscription\x12\x15\n\rtranscription\x18\x01 \x01(\t\x12\x18\n\x10\x63onfidence_score\x18\x02 \x01(\x02\x12%\n\x05words\x18\x03 \x03(\x0b\x32\x16.ondewo.s2t.WordDetail\x12:\n\x0c\x61lternatives\x18\x04 \x03(\x0b\x32$.ondewo.s2t.TranscriptionAlternative\"i\n\x18TranscriptionAlternative\x12\x12\n\ntranscript\x18\x01 \x01(\t\x12\x12\n\nconfidence\x18\x02 \x01(\x02\x12%\n\x05words\x18\x03 \x03(\x0b\x32\x16.ondewo.s2t.WordDetail\"\x8c\x01\n\nWordDetail\x12\x12\n\nstart_time\x18\x01 \x01(\x02\x12\x10\n\x08\x65nd_time\x18\x02 \x01(\x02\x12\x0c\n\x04word\x18\x03 \x01(\t\x12\x12\n\nconfidence\x18\x04 \x01(\x02\x12\x36\n\x11word_alternatives\x18\x05 \x03(\x0b\x32\x1b.ondewo.s2t.WordAlternative\"3\n\x0fWordAlternative\x12\x0c\n\x04word\x18\x01 \x01(\t\x12\x12\n\nconfidence\x18\x02 \x01(\x02\"\x8e\x01\n\x17TranscribeStreamRequest\x12\x13\n\x0b\x61udio_chunk\x18\x01 \x01(\x0c\x12\x15\n\rend_of_stream\x18\x02 \x01(\x08\x12\x33\n\x06\x63onfig\x18\x03 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\x12\x12\n\nmute_audio\x18\x04 \x01(\x08\"\x83\x02\n\x18TranscribeStreamResponse\x12\x31\n\x0etranscriptions\x18\x01 \x03(\x0b\x32\x19.ondewo.s2t.Transcription\x12\x0c\n\x04time\x18\x02 \x01(\x02\x12\r\n\x05\x66inal\x18\x03 \x01(\x08\x12\x14\n\x0creturn_audio\x18\x04 \x01(\x08\x12\r\n\x05\x61udio\x18\x05 \x01(\x0c\x12\x17\n\x0futterance_start\x18\x06 \x01(\x08\x12\x12\n\naudio_uuid\x18\x07 \x01(\t\x12\x35\n\x06\x63onfig\x18\x08 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfigH\x00\x42\x0e\n\x0coneof_config\"`\n\x15TranscribeFileRequest\x12\x12\n\naudio_file\x18\x01 \x01(\x0c\x12\x33\n\x06\x63onfig\x18\x02 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\"m\n\x16TranscribeFileResponse\x12\x31\n\x0etranscriptions\x18\x01 \x03(\x0b\x32\x19.ondewo.s2t.Transcription\x12\x0c\n\x04time\x18\x02 \x01(\x02\x12\x12\n\naudio_uuid\x18\x03 \x01(\t\"\x1b\n\rS2tPipelineId\x12\n\n\x02id\x18\x01 \x01(\t\"o\n\x17ListS2tPipelinesRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\x12\x0f\n\x07\x64omains\x18\x03 \x03(\t\x12\x17\n\x0fregistered_only\x18\x04 \x01(\x08\"S\n\x18ListS2tPipelinesResponse\x12\x37\n\x10pipeline_configs\x18\x01 \x03(\x0b\x32\x1d.ondewo.s2t.Speech2TextConfig\"C\n\x17ListS2tLanguagesRequest\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\"-\n\x18ListS2tLanguagesResponse\x12\x11\n\tlanguages\x18\x01 \x03(\t\"C\n\x15ListS2tDomainsRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\")\n\x16ListS2tDomainsResponse\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\",\n\x19S2TGetServiceInfoResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"\xe5\x02\n\x11Speech2TextConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12/\n\x0b\x64\x65scription\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.S2TDescription\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\x12+\n\tinference\x18\x04 \x01(\x0b\x32\x18.ondewo.s2t.S2TInference\x12\x35\n\x10streaming_server\x18\x05 \x01(\x0b\x32\x1b.ondewo.s2t.StreamingServer\x12\x44\n\x18voice_activity_detection\x18\x06 \x01(\x0b\x32\".ondewo.s2t.VoiceActivityDetection\x12\x33\n\x0fpost_processing\x18\x07 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessing\x12$\n\x07logging\x18\x08 \x01(\x0b\x32\x13.ondewo.s2t.Logging\"\\\n\x0eS2TDescription\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x16\n\x0epipeline_owner\x18\x02 \x01(\t\x12\x0e\n\x06\x64omain\x18\x03 \x01(\t\x12\x10\n\x08\x63omments\x18\x04 \x01(\t\"\xb1\x01\n\x0cS2TInference\x12\x33\n\x0f\x61\x63oustic_models\x18\x01 \x01(\x0b\x32\x1a.ondewo.s2t.AcousticModels\x12\x33\n\x0flanguage_models\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.LanguageModels\x12\x37\n\x11inference_backend\x18\x03 \x01(\x0e\x32\x1c.ondewo.s2t.InferenceBackend\"\xb1\x02\n\x0e\x41\x63ousticModels\x12\x0c\n\x04type\x18\x01 \x01(\t\x12(\n\tquartznet\x18\x02 \x01(\x0b\x32\x15.ondewo.s2t.Quartznet\x12\x35\n\x10quartznet_triton\x18\x03 \x01(\x0b\x32\x1b.ondewo.s2t.QuartznetTriton\x12$\n\x07wav2vec\x18\x04 \x01(\x0b\x32\x13.ondewo.s2t.Wav2Vec\x12\x31\n\x0ewav2vec_triton\x18\x05 \x01(\x0b\x32\x19.ondewo.s2t.Wav2VecTriton\x12$\n\x07whisper\x18\x06 \x01(\x0b\x32\x13.ondewo.s2t.Whisper\x12\x31\n\x0ewhisper_triton\x18\x07 \x01(\x0b\x32\x19.ondewo.s2t.WhisperTriton\"@\n\x07Whisper\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\x12\x10\n\x08language\x18\x03 \x01(\t\"~\n\rWhisperTriton\x12\x16\n\x0eprocessor_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\x12\x1c\n\x14triton_model_version\x18\x03 \x01(\t\x12\x1c\n\x14\x63heck_status_timeout\x18\x04 \x01(\x03\".\n\x07Wav2Vec\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\"~\n\rWav2VecTriton\x12\x16\n\x0eprocessor_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\x12\x1c\n\x14triton_model_version\x18\x03 \x01(\t\x12\x1c\n\x14\x63heck_status_timeout\x18\x04 \x01(\x03\"\x94\x01\n\tQuartznet\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x11\n\tload_type\x18\x02 \x01(\t\x12%\n\x08pt_files\x18\x03 \x01(\x0b\x32\x13.ondewo.s2t.PtFiles\x12\'\n\tckpt_file\x18\x04 \x01(\x0b\x32\x14.ondewo.s2t.CkptFile\x12\x0f\n\x07use_gpu\x18\x05 \x01(\x08\"%\n\x07PtFiles\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0c\n\x04step\x18\x02 \x01(\t\"\x18\n\x08\x43kptFile\x12\x0c\n\x04path\x18\x01 \x01(\t\"P\n\x0fQuartznetTriton\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x12\n\ntriton_url\x18\x02 \x01(\t\x12\x14\n\x0ctriton_model\x18\x03 \x01(\t\"\x88\x01\n\x0eLanguageModels\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tbeam_size\x18\x02 \x01(\x03\x12\x12\n\ndefault_lm\x18\x03 \x01(\t\x12 \n\x18\x62\x65\x61m_search_scorer_alpha\x18\x04 \x01(\x02\x12\x1f\n\x17\x62\x65\x61m_search_scorer_beta\x18\x05 \x01(\x02\"\x91\x01\n\x0fStreamingServer\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x03\x12\x14\n\x0coutput_style\x18\x03 \x01(\t\x12L\n\x1cstreaming_speech_recognition\x18\x04 \x01(\x0b\x32&.ondewo.s2t.StreamingSpeechRecognition\"\xee\x01\n\x1aStreamingSpeechRecognition\x12\x1c\n\x14transcribe_not_final\x18\x01 \x01(\x08\x12\x17\n\x0f\x64\x65\x63oding_method\x18\x02 \x01(\t\x12\x15\n\rsampling_rate\x18\x03 \x01(\x03\x12\x1c\n\x14min_audio_chunk_size\x18\x04 \x01(\x03\x12$\n\x1cstart_of_utterance_threshold\x18\x05 \x01(\x02\x12\"\n\x1a\x65nd_of_utterance_threshold\x18\x06 \x01(\x02\x12\x1a\n\x12next_chunk_timeout\x18\x07 \x01(\x02\"\x8f\x01\n\x16VoiceActivityDetection\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\t\x12\x15\n\rsampling_rate\x18\x02 \x01(\x03\x12&\n\x08pyannote\x18\x03 \x01(\x0b\x32\x14.ondewo.s2t.Pyannote\x12&\n\x08matchbox\x18\x04 \x01(\x0b\x32\x14.ondewo.s2t.Matchbox\"\xb0\x01\n\x08Pyannote\x12\x12\n\nmodel_path\x18\x01 \x01(\t\x12\x16\n\x0emin_audio_size\x18\x02 \x01(\x03\x12\x0e\n\x06offset\x18\x03 \x01(\x02\x12\r\n\x05onset\x18\x04 \x01(\x02\x12\x13\n\tlog_scale\x18\x05 \x01(\x08H\x00\x12\x18\n\x10min_duration_off\x18\x06 \x01(\x02\x12\x17\n\x0fmin_duration_on\x18\x07 \x01(\x02\x42\x11\n\x0foneof_log_scale\"L\n\x08Matchbox\x12\x14\n\x0cmodel_config\x18\x01 \x01(\t\x12\x14\n\x0c\x65ncoder_path\x18\x02 \x01(\t\x12\x14\n\x0c\x64\x65\x63oder_path\x18\x03 \x01(\t\"W\n\x0ePostProcessing\x12\x10\n\x08pipeline\x18\x01 \x03(\t\x12\x33\n\x0fpost_processors\x18\x02 \x01(\x0b\x32\x1a.ondewo.s2t.PostProcessors\"n\n\x0ePostProcessors\x12\'\n\tsym_spell\x18\x01 \x01(\x0b\x32\x14.ondewo.s2t.SymSpell\x12\x33\n\rnormalization\x18\x02 \x01(\x0b\x32\x1c.ondewo.s2t.S2TNormalization\"Z\n\x08SymSpell\x12\x11\n\tdict_path\x18\x01 \x01(\t\x12$\n\x1cmax_dictionary_edit_distance\x18\x02 \x01(\x03\x12\x15\n\rprefix_length\x18\x03 \x01(\x03\"$\n\x10S2TNormalization\x12\x10\n\x08language\x18\x01 \x01(\t\"%\n\x07Logging\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"+\n\x1cListS2tLanguageModelsRequest\x12\x0b\n\x03ids\x18\x01 \x03(\t\"C\n\x17LanguageModelPipelineId\x12\x13\n\x0bpipeline_id\x18\x01 \x01(\t\x12\x13\n\x0bmodel_names\x18\x02 \x03(\t\"]\n\x1dListS2tLanguageModelsResponse\x12<\n\x0flm_pipeline_ids\x18\x01 \x03(\x0b\x32#.ondewo.s2t.LanguageModelPipelineId\"=\n\x1e\x43reateUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\"=\n\x1e\x44\x65leteUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\"U\n!AddDataToUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\x12\x13\n\x0bzipped_data\x18\x02 \x01(\x0c\"K\n\x1dTrainUserLanguageModelRequest\x12\x1b\n\x13language_model_name\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\x03*M\n\x08\x44\x65\x63oding\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06GREEDY\x10\x01\x12\x17\n\x13\x42\x45\x41M_SEARCH_WITH_LM\x10\x02\x12\x0f\n\x0b\x42\x45\x41M_SEARCH\x10\x03*l\n\x10InferenceBackend\x12\x1d\n\x19INFERENCE_BACKEND_UNKNOWN\x10\x00\x12\x1d\n\x19INFERENCE_BACKEND_PYTORCH\x10\x01\x12\x1a\n\x16INFERENCE_BACKEND_FLAX\x10\x02\x32\xec\n\n\x0bSpeech2Text\x12Y\n\x0eTranscribeFile\x12!.ondewo.s2t.TranscribeFileRequest\x1a\".ondewo.s2t.TranscribeFileResponse\"\x00\x12\x63\n\x10TranscribeStream\x12#.ondewo.s2t.TranscribeStreamRequest\x1a$.ondewo.s2t.TranscribeStreamResponse\"\x00(\x01\x30\x01\x12L\n\x0eGetS2tPipeline\x12\x19.ondewo.s2t.S2tPipelineId\x1a\x1d.ondewo.s2t.Speech2TextConfig\"\x00\x12O\n\x11\x43reateS2tPipeline\x12\x1d.ondewo.s2t.Speech2TextConfig\x1a\x19.ondewo.s2t.S2tPipelineId\"\x00\x12H\n\x11\x44\x65leteS2tPipeline\x12\x19.ondewo.s2t.S2tPipelineId\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x11UpdateS2tPipeline\x12\x1d.ondewo.s2t.Speech2TextConfig\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x10ListS2tPipelines\x12#.ondewo.s2t.ListS2tPipelinesRequest\x1a$.ondewo.s2t.ListS2tPipelinesResponse\"\x00\x12_\n\x10ListS2tLanguages\x12#.ondewo.s2t.ListS2tLanguagesRequest\x1a$.ondewo.s2t.ListS2tLanguagesResponse\"\x00\x12Y\n\x0eListS2tDomains\x12!.ondewo.s2t.ListS2tDomainsRequest\x1a\".ondewo.s2t.ListS2tDomainsResponse\"\x00\x12Q\n\x0eGetServiceInfo\x12\x16.google.protobuf.Empty\x1a%.ondewo.s2t.S2TGetServiceInfoResponse\"\x00\x12n\n\x15ListS2tLanguageModels\x12(.ondewo.s2t.ListS2tLanguageModelsRequest\x1a).ondewo.s2t.ListS2tLanguageModelsResponse\"\x00\x12_\n\x17\x43reateUserLanguageModel\x12*.ondewo.s2t.CreateUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x17\x44\x65leteUserLanguageModel\x12*.ondewo.s2t.DeleteUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x65\n\x1a\x41\x64\x64\x44\x61taToUserLanguageModel\x12-.ondewo.s2t.AddDataToUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x12]\n\x16TrainUserLanguageModel\x12).ondewo.s2t.TrainUserLanguageModelRequest\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
 
-_CTCDECODING = DESCRIPTOR.enum_types_by_name['CTCDecoding']
-CTCDecoding = enum_type_wrapper.EnumTypeWrapper(_CTCDECODING)
+_DECODING = DESCRIPTOR.enum_types_by_name['Decoding']
+Decoding = enum_type_wrapper.EnumTypeWrapper(_DECODING)
+_INFERENCEBACKEND = DESCRIPTOR.enum_types_by_name['InferenceBackend']
+InferenceBackend = enum_type_wrapper.EnumTypeWrapper(_INFERENCEBACKEND)
 DEFAULT = 0
 GREEDY = 1
 BEAM_SEARCH_WITH_LM = 2
+BEAM_SEARCH = 3
+INFERENCE_BACKEND_UNKNOWN = 0
+INFERENCE_BACKEND_PYTORCH = 1
+INFERENCE_BACKEND_FLAX = 2
 
 
 _TRANSCRIBEREQUESTCONFIG = DESCRIPTOR.message_types_by_name['TranscribeRequestConfig']
 _TRANSCRIPTIONRETURNOPTIONS = DESCRIPTOR.message_types_by_name['TranscriptionReturnOptions']
 _UTTERANCEDETECTIONOPTIONS = DESCRIPTOR.message_types_by_name['UtteranceDetectionOptions']
 _POSTPROCESSINGOPTIONS = DESCRIPTOR.message_types_by_name['PostProcessingOptions']
-_TRANSCRIBESTREAMREQUEST = DESCRIPTOR.message_types_by_name['TranscribeStreamRequest']
 _TRANSCRIPTION = DESCRIPTOR.message_types_by_name['Transcription']
+_TRANSCRIPTIONALTERNATIVE = DESCRIPTOR.message_types_by_name['TranscriptionAlternative']
+_WORDDETAIL = DESCRIPTOR.message_types_by_name['WordDetail']
+_WORDALTERNATIVE = DESCRIPTOR.message_types_by_name['WordAlternative']
+_TRANSCRIBESTREAMREQUEST = DESCRIPTOR.message_types_by_name['TranscribeStreamRequest']
 _TRANSCRIBESTREAMRESPONSE = DESCRIPTOR.message_types_by_name['TranscribeStreamResponse']
 _TRANSCRIBEFILEREQUEST = DESCRIPTOR.message_types_by_name['TranscribeFileRequest']
 _TRANSCRIBEFILERESPONSE = DESCRIPTOR.message_types_by_name['TranscribeFileResponse']
-_WORDTIMING = DESCRIPTOR.message_types_by_name['WordTiming']
 _S2TPIPELINEID = DESCRIPTOR.message_types_by_name['S2tPipelineId']
 _LISTS2TPIPELINESREQUEST = DESCRIPTOR.message_types_by_name['ListS2tPipelinesRequest']
 _LISTS2TPIPELINESRESPONSE = DESCRIPTOR.message_types_by_name['ListS2tPipelinesResponse']
 _LISTS2TLANGUAGESREQUEST = DESCRIPTOR.message_types_by_name['ListS2tLanguagesRequest']
 _LISTS2TLANGUAGESRESPONSE = DESCRIPTOR.message_types_by_name['ListS2tLanguagesResponse']
 _LISTS2TDOMAINSREQUEST = DESCRIPTOR.message_types_by_name['ListS2tDomainsRequest']
 _LISTS2TDOMAINSRESPONSE = DESCRIPTOR.message_types_by_name['ListS2tDomainsResponse']
 _S2TGETSERVICEINFORESPONSE = DESCRIPTOR.message_types_by_name['S2TGetServiceInfoResponse']
 _SPEECH2TEXTCONFIG = DESCRIPTOR.message_types_by_name['Speech2TextConfig']
 _S2TDESCRIPTION = DESCRIPTOR.message_types_by_name['S2TDescription']
 _S2TINFERENCE = DESCRIPTOR.message_types_by_name['S2TInference']
-_CTCACOUSTICMODELS = DESCRIPTOR.message_types_by_name['CtcAcousticModels']
+_ACOUSTICMODELS = DESCRIPTOR.message_types_by_name['AcousticModels']
+_WHISPER = DESCRIPTOR.message_types_by_name['Whisper']
+_WHISPERTRITON = DESCRIPTOR.message_types_by_name['WhisperTriton']
 _WAV2VEC = DESCRIPTOR.message_types_by_name['Wav2Vec']
 _WAV2VECTRITON = DESCRIPTOR.message_types_by_name['Wav2VecTriton']
 _QUARTZNET = DESCRIPTOR.message_types_by_name['Quartznet']
 _PTFILES = DESCRIPTOR.message_types_by_name['PtFiles']
 _CKPTFILE = DESCRIPTOR.message_types_by_name['CkptFile']
 _QUARTZNETTRITON = DESCRIPTOR.message_types_by_name['QuartznetTriton']
 _LANGUAGEMODELS = DESCRIPTOR.message_types_by_name['LanguageModels']
@@ -93,28 +103,49 @@
 PostProcessingOptions = _reflection.GeneratedProtocolMessageType('PostProcessingOptions', (_message.Message,), {
     'DESCRIPTOR': _POSTPROCESSINGOPTIONS,
     '__module__': 'ondewo.s2t.speech_to_text_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.s2t.PostProcessingOptions)
 })
 _sym_db.RegisterMessage(PostProcessingOptions)
 
-TranscribeStreamRequest = _reflection.GeneratedProtocolMessageType('TranscribeStreamRequest', (_message.Message,), {
-    'DESCRIPTOR': _TRANSCRIBESTREAMREQUEST,
-    '__module__': 'ondewo.s2t.speech_to_text_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.s2t.TranscribeStreamRequest)
-})
-_sym_db.RegisterMessage(TranscribeStreamRequest)
-
 Transcription = _reflection.GeneratedProtocolMessageType('Transcription', (_message.Message,), {
     'DESCRIPTOR': _TRANSCRIPTION,
     '__module__': 'ondewo.s2t.speech_to_text_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.s2t.Transcription)
 })
 _sym_db.RegisterMessage(Transcription)
 
+TranscriptionAlternative = _reflection.GeneratedProtocolMessageType('TranscriptionAlternative', (_message.Message,), {
+    'DESCRIPTOR': _TRANSCRIPTIONALTERNATIVE,
+    '__module__': 'ondewo.s2t.speech_to_text_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.s2t.TranscriptionAlternative)
+})
+_sym_db.RegisterMessage(TranscriptionAlternative)
+
+WordDetail = _reflection.GeneratedProtocolMessageType('WordDetail', (_message.Message,), {
+    'DESCRIPTOR': _WORDDETAIL,
+    '__module__': 'ondewo.s2t.speech_to_text_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.s2t.WordDetail)
+})
+_sym_db.RegisterMessage(WordDetail)
+
+WordAlternative = _reflection.GeneratedProtocolMessageType('WordAlternative', (_message.Message,), {
+    'DESCRIPTOR': _WORDALTERNATIVE,
+    '__module__': 'ondewo.s2t.speech_to_text_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.s2t.WordAlternative)
+})
+_sym_db.RegisterMessage(WordAlternative)
+
+TranscribeStreamRequest = _reflection.GeneratedProtocolMessageType('TranscribeStreamRequest', (_message.Message,), {
+    'DESCRIPTOR': _TRANSCRIBESTREAMREQUEST,
+    '__module__': 'ondewo.s2t.speech_to_text_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.s2t.TranscribeStreamRequest)
+})
+_sym_db.RegisterMessage(TranscribeStreamRequest)
+
 TranscribeStreamResponse = _reflection.GeneratedProtocolMessageType('TranscribeStreamResponse', (_message.Message,), {
     'DESCRIPTOR': _TRANSCRIBESTREAMRESPONSE,
     '__module__': 'ondewo.s2t.speech_to_text_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.s2t.TranscribeStreamResponse)
 })
 _sym_db.RegisterMessage(TranscribeStreamResponse)
 
@@ -128,21 +159,14 @@
 TranscribeFileResponse = _reflection.GeneratedProtocolMessageType('TranscribeFileResponse', (_message.Message,), {
     'DESCRIPTOR': _TRANSCRIBEFILERESPONSE,
     '__module__': 'ondewo.s2t.speech_to_text_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.s2t.TranscribeFileResponse)
 })
 _sym_db.RegisterMessage(TranscribeFileResponse)
 
-WordTiming = _reflection.GeneratedProtocolMessageType('WordTiming', (_message.Message,), {
-    'DESCRIPTOR': _WORDTIMING,
-    '__module__': 'ondewo.s2t.speech_to_text_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.s2t.WordTiming)
-})
-_sym_db.RegisterMessage(WordTiming)
-
 S2tPipelineId = _reflection.GeneratedProtocolMessageType('S2tPipelineId', (_message.Message,), {
     'DESCRIPTOR': _S2TPIPELINEID,
     '__module__': 'ondewo.s2t.speech_to_text_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.s2t.S2tPipelineId)
 })
 _sym_db.RegisterMessage(S2tPipelineId)
 
@@ -212,20 +236,34 @@
 S2TInference = _reflection.GeneratedProtocolMessageType('S2TInference', (_message.Message,), {
     'DESCRIPTOR': _S2TINFERENCE,
     '__module__': 'ondewo.s2t.speech_to_text_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.s2t.S2TInference)
 })
 _sym_db.RegisterMessage(S2TInference)
 
-CtcAcousticModels = _reflection.GeneratedProtocolMessageType('CtcAcousticModels', (_message.Message,), {
-    'DESCRIPTOR': _CTCACOUSTICMODELS,
+AcousticModels = _reflection.GeneratedProtocolMessageType('AcousticModels', (_message.Message,), {
+    'DESCRIPTOR': _ACOUSTICMODELS,
+    '__module__': 'ondewo.s2t.speech_to_text_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.s2t.AcousticModels)
+})
+_sym_db.RegisterMessage(AcousticModels)
+
+Whisper = _reflection.GeneratedProtocolMessageType('Whisper', (_message.Message,), {
+    'DESCRIPTOR': _WHISPER,
+    '__module__': 'ondewo.s2t.speech_to_text_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.s2t.Whisper)
+})
+_sym_db.RegisterMessage(Whisper)
+
+WhisperTriton = _reflection.GeneratedProtocolMessageType('WhisperTriton', (_message.Message,), {
+    'DESCRIPTOR': _WHISPERTRITON,
     '__module__': 'ondewo.s2t.speech_to_text_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.s2t.CtcAcousticModels)
+    # @@protoc_insertion_point(class_scope:ondewo.s2t.WhisperTriton)
 })
-_sym_db.RegisterMessage(CtcAcousticModels)
+_sym_db.RegisterMessage(WhisperTriton)
 
 Wav2Vec = _reflection.GeneratedProtocolMessageType('Wav2Vec', (_message.Message,), {
     'DESCRIPTOR': _WAV2VEC,
     '__module__': 'ondewo.s2t.speech_to_text_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.s2t.Wav2Vec)
 })
 _sym_db.RegisterMessage(Wav2Vec)
@@ -391,104 +429,114 @@
 })
 _sym_db.RegisterMessage(TrainUserLanguageModelRequest)
 
 _SPEECH2TEXT = DESCRIPTOR.services_by_name['Speech2Text']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _CTCDECODING._serialized_start = 5492
-    _CTCDECODING._serialized_end = 5555
+    _DECODING._serialized_start = 6230
+    _DECODING._serialized_end = 6307
+    _INFERENCEBACKEND._serialized_start = 6309
+    _INFERENCEBACKEND._serialized_end = 6417
     _TRANSCRIBEREQUESTCONFIG._serialized_start = 77
-    _TRANSCRIBEREQUESTCONFIG._serialized_end = 622
-    _TRANSCRIPTIONRETURNOPTIONS._serialized_start = 625
-    _TRANSCRIPTIONRETURNOPTIONS._serialized_end = 811
-    _UTTERANCEDETECTIONOPTIONS._serialized_start = 814
-    _UTTERANCEDETECTIONOPTIONS._serialized_end = 1005
-    _POSTPROCESSINGOPTIONS._serialized_start = 1007
-    _POSTPROCESSINGOPTIONS._serialized_end = 1122
-    _TRANSCRIBESTREAMREQUEST._serialized_start = 1125
-    _TRANSCRIBESTREAMREQUEST._serialized_end = 1267
-    _TRANSCRIPTION._serialized_start = 1269
-    _TRANSCRIPTION._serialized_end = 1333
-    _TRANSCRIBESTREAMRESPONSE._serialized_start = 1336
-    _TRANSCRIBESTREAMRESPONSE._serialized_end = 1595
-    _TRANSCRIBEFILEREQUEST._serialized_start = 1597
-    _TRANSCRIBEFILEREQUEST._serialized_end = 1693
-    _TRANSCRIBEFILERESPONSE._serialized_start = 1696
-    _TRANSCRIBEFILERESPONSE._serialized_end = 1850
-    _WORDTIMING._serialized_start = 1852
-    _WORDTIMING._serialized_end = 1906
-    _S2TPIPELINEID._serialized_start = 1908
-    _S2TPIPELINEID._serialized_end = 1935
-    _LISTS2TPIPELINESREQUEST._serialized_start = 1937
-    _LISTS2TPIPELINESREQUEST._serialized_end = 2048
-    _LISTS2TPIPELINESRESPONSE._serialized_start = 2050
-    _LISTS2TPIPELINESRESPONSE._serialized_end = 2133
-    _LISTS2TLANGUAGESREQUEST._serialized_start = 2135
-    _LISTS2TLANGUAGESREQUEST._serialized_end = 2202
-    _LISTS2TLANGUAGESRESPONSE._serialized_start = 2204
-    _LISTS2TLANGUAGESRESPONSE._serialized_end = 2249
-    _LISTS2TDOMAINSREQUEST._serialized_start = 2251
-    _LISTS2TDOMAINSREQUEST._serialized_end = 2318
-    _LISTS2TDOMAINSRESPONSE._serialized_start = 2320
-    _LISTS2TDOMAINSRESPONSE._serialized_end = 2361
-    _S2TGETSERVICEINFORESPONSE._serialized_start = 2363
-    _S2TGETSERVICEINFORESPONSE._serialized_end = 2407
-    _SPEECH2TEXTCONFIG._serialized_start = 2410
-    _SPEECH2TEXTCONFIG._serialized_end = 2767
-    _S2TDESCRIPTION._serialized_start = 2769
-    _S2TDESCRIPTION._serialized_end = 2861
-    _S2TINFERENCE._serialized_start = 2863
-    _S2TINFERENCE._serialized_end = 2990
-    _CTCACOUSTICMODELS._serialized_start = 2993
-    _CTCACOUSTICMODELS._serialized_end = 3212
-    _WAV2VEC._serialized_start = 3214
-    _WAV2VEC._serialized_end = 3260
-    _WAV2VECTRITON._serialized_start = 3262
-    _WAV2VECTRITON._serialized_end = 3388
-    _QUARTZNET._serialized_start = 3391
-    _QUARTZNET._serialized_end = 3539
-    _PTFILES._serialized_start = 3541
-    _PTFILES._serialized_end = 3578
-    _CKPTFILE._serialized_start = 3580
-    _CKPTFILE._serialized_end = 3604
-    _QUARTZNETTRITON._serialized_start = 3606
-    _QUARTZNETTRITON._serialized_end = 3686
-    _LANGUAGEMODELS._serialized_start = 3689
-    _LANGUAGEMODELS._serialized_end = 3825
-    _STREAMINGSERVER._serialized_start = 3828
-    _STREAMINGSERVER._serialized_end = 3973
-    _STREAMINGSPEECHRECOGNITION._serialized_start = 3976
-    _STREAMINGSPEECHRECOGNITION._serialized_end = 4218
-    _VOICEACTIVITYDETECTION._serialized_start = 4221
-    _VOICEACTIVITYDETECTION._serialized_end = 4364
-    _PYANNOTE._serialized_start = 4367
-    _PYANNOTE._serialized_end = 4543
-    _MATCHBOX._serialized_start = 4545
-    _MATCHBOX._serialized_end = 4621
-    _POSTPROCESSING._serialized_start = 4623
-    _POSTPROCESSING._serialized_end = 4710
-    _POSTPROCESSORS._serialized_start = 4712
-    _POSTPROCESSORS._serialized_end = 4822
-    _SYMSPELL._serialized_start = 4824
-    _SYMSPELL._serialized_end = 4914
-    _S2TNORMALIZATION._serialized_start = 4916
-    _S2TNORMALIZATION._serialized_end = 4952
-    _LOGGING._serialized_start = 4954
-    _LOGGING._serialized_end = 4991
-    _LISTS2TLANGUAGEMODELSREQUEST._serialized_start = 4993
-    _LISTS2TLANGUAGEMODELSREQUEST._serialized_end = 5036
-    _LANGUAGEMODELPIPELINEID._serialized_start = 5038
-    _LANGUAGEMODELPIPELINEID._serialized_end = 5105
-    _LISTS2TLANGUAGEMODELSRESPONSE._serialized_start = 5107
-    _LISTS2TLANGUAGEMODELSRESPONSE._serialized_end = 5200
-    _CREATEUSERLANGUAGEMODELREQUEST._serialized_start = 5202
-    _CREATEUSERLANGUAGEMODELREQUEST._serialized_end = 5263
-    _DELETEUSERLANGUAGEMODELREQUEST._serialized_start = 5265
-    _DELETEUSERLANGUAGEMODELREQUEST._serialized_end = 5326
-    _ADDDATATOUSERLANGUAGEMODELREQUEST._serialized_start = 5328
-    _ADDDATATOUSERLANGUAGEMODELREQUEST._serialized_end = 5413
-    _TRAINUSERLANGUAGEMODELREQUEST._serialized_start = 5415
-    _TRAINUSERLANGUAGEMODELREQUEST._serialized_end = 5490
-    _SPEECH2TEXT._serialized_start = 5558
-    _SPEECH2TEXT._serialized_end = 6946
+    _TRANSCRIBEREQUESTCONFIG._serialized_end = 615
+    _TRANSCRIPTIONRETURNOPTIONS._serialized_start = 618
+    _TRANSCRIPTIONRETURNOPTIONS._serialized_end = 921
+    _UTTERANCEDETECTIONOPTIONS._serialized_start = 924
+    _UTTERANCEDETECTIONOPTIONS._serialized_end = 1115
+    _POSTPROCESSINGOPTIONS._serialized_start = 1117
+    _POSTPROCESSINGOPTIONS._serialized_end = 1232
+    _TRANSCRIPTION._serialized_start = 1235
+    _TRANSCRIPTION._serialized_end = 1398
+    _TRANSCRIPTIONALTERNATIVE._serialized_start = 1400
+    _TRANSCRIPTIONALTERNATIVE._serialized_end = 1505
+    _WORDDETAIL._serialized_start = 1508
+    _WORDDETAIL._serialized_end = 1648
+    _WORDALTERNATIVE._serialized_start = 1650
+    _WORDALTERNATIVE._serialized_end = 1701
+    _TRANSCRIBESTREAMREQUEST._serialized_start = 1704
+    _TRANSCRIBESTREAMREQUEST._serialized_end = 1846
+    _TRANSCRIBESTREAMRESPONSE._serialized_start = 1849
+    _TRANSCRIBESTREAMRESPONSE._serialized_end = 2108
+    _TRANSCRIBEFILEREQUEST._serialized_start = 2110
+    _TRANSCRIBEFILEREQUEST._serialized_end = 2206
+    _TRANSCRIBEFILERESPONSE._serialized_start = 2208
+    _TRANSCRIBEFILERESPONSE._serialized_end = 2317
+    _S2TPIPELINEID._serialized_start = 2319
+    _S2TPIPELINEID._serialized_end = 2346
+    _LISTS2TPIPELINESREQUEST._serialized_start = 2348
+    _LISTS2TPIPELINESREQUEST._serialized_end = 2459
+    _LISTS2TPIPELINESRESPONSE._serialized_start = 2461
+    _LISTS2TPIPELINESRESPONSE._serialized_end = 2544
+    _LISTS2TLANGUAGESREQUEST._serialized_start = 2546
+    _LISTS2TLANGUAGESREQUEST._serialized_end = 2613
+    _LISTS2TLANGUAGESRESPONSE._serialized_start = 2615
+    _LISTS2TLANGUAGESRESPONSE._serialized_end = 2660
+    _LISTS2TDOMAINSREQUEST._serialized_start = 2662
+    _LISTS2TDOMAINSREQUEST._serialized_end = 2729
+    _LISTS2TDOMAINSRESPONSE._serialized_start = 2731
+    _LISTS2TDOMAINSRESPONSE._serialized_end = 2772
+    _S2TGETSERVICEINFORESPONSE._serialized_start = 2774
+    _S2TGETSERVICEINFORESPONSE._serialized_end = 2818
+    _SPEECH2TEXTCONFIG._serialized_start = 2821
+    _SPEECH2TEXTCONFIG._serialized_end = 3178
+    _S2TDESCRIPTION._serialized_start = 3180
+    _S2TDESCRIPTION._serialized_end = 3272
+    _S2TINFERENCE._serialized_start = 3275
+    _S2TINFERENCE._serialized_end = 3452
+    _ACOUSTICMODELS._serialized_start = 3455
+    _ACOUSTICMODELS._serialized_end = 3760
+    _WHISPER._serialized_start = 3762
+    _WHISPER._serialized_end = 3826
+    _WHISPERTRITON._serialized_start = 3828
+    _WHISPERTRITON._serialized_end = 3954
+    _WAV2VEC._serialized_start = 3956
+    _WAV2VEC._serialized_end = 4002
+    _WAV2VECTRITON._serialized_start = 4004
+    _WAV2VECTRITON._serialized_end = 4130
+    _QUARTZNET._serialized_start = 4133
+    _QUARTZNET._serialized_end = 4281
+    _PTFILES._serialized_start = 4283
+    _PTFILES._serialized_end = 4320
+    _CKPTFILE._serialized_start = 4322
+    _CKPTFILE._serialized_end = 4346
+    _QUARTZNETTRITON._serialized_start = 4348
+    _QUARTZNETTRITON._serialized_end = 4428
+    _LANGUAGEMODELS._serialized_start = 4431
+    _LANGUAGEMODELS._serialized_end = 4567
+    _STREAMINGSERVER._serialized_start = 4570
+    _STREAMINGSERVER._serialized_end = 4715
+    _STREAMINGSPEECHRECOGNITION._serialized_start = 4718
+    _STREAMINGSPEECHRECOGNITION._serialized_end = 4956
+    _VOICEACTIVITYDETECTION._serialized_start = 4959
+    _VOICEACTIVITYDETECTION._serialized_end = 5102
+    _PYANNOTE._serialized_start = 5105
+    _PYANNOTE._serialized_end = 5281
+    _MATCHBOX._serialized_start = 5283
+    _MATCHBOX._serialized_end = 5359
+    _POSTPROCESSING._serialized_start = 5361
+    _POSTPROCESSING._serialized_end = 5448
+    _POSTPROCESSORS._serialized_start = 5450
+    _POSTPROCESSORS._serialized_end = 5560
+    _SYMSPELL._serialized_start = 5562
+    _SYMSPELL._serialized_end = 5652
+    _S2TNORMALIZATION._serialized_start = 5654
+    _S2TNORMALIZATION._serialized_end = 5690
+    _LOGGING._serialized_start = 5692
+    _LOGGING._serialized_end = 5729
+    _LISTS2TLANGUAGEMODELSREQUEST._serialized_start = 5731
+    _LISTS2TLANGUAGEMODELSREQUEST._serialized_end = 5774
+    _LANGUAGEMODELPIPELINEID._serialized_start = 5776
+    _LANGUAGEMODELPIPELINEID._serialized_end = 5843
+    _LISTS2TLANGUAGEMODELSRESPONSE._serialized_start = 5845
+    _LISTS2TLANGUAGEMODELSRESPONSE._serialized_end = 5938
+    _CREATEUSERLANGUAGEMODELREQUEST._serialized_start = 5940
+    _CREATEUSERLANGUAGEMODELREQUEST._serialized_end = 6001
+    _DELETEUSERLANGUAGEMODELREQUEST._serialized_start = 6003
+    _DELETEUSERLANGUAGEMODELREQUEST._serialized_end = 6064
+    _ADDDATATOUSERLANGUAGEMODELREQUEST._serialized_start = 6066
+    _ADDDATATOUSERLANGUAGEMODELREQUEST._serialized_end = 6151
+    _TRAINUSERLANGUAGEMODELREQUEST._serialized_start = 6153
+    _TRAINUSERLANGUAGEMODELREQUEST._serialized_end = 6228
+    _SPEECH2TEXT._serialized_start = 6420
+    _SPEECH2TEXT._serialized_end = 7808
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/sip/sip_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/sip/sip_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/sip/sip_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/sip/sip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/t2s/text_to_speech_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/t2s/text_to_speech_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/vtsi/voip_pb2.py` & `ondewo-vtsi-client-6.0.0/ondewo/vtsi/calls_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,589 +1,598 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: ondewo/vtsi/voip.proto
+# source: ondewo/vtsi/calls.proto
 """Generated protocol buffer code."""
 from ondewo.sip import sip_pb2 as ondewo_dot_sip_dot_sip__pb2
 from ondewo.t2s import text_to_speech_pb2 as ondewo_dot_t2s_dot_text__to__speech__pb2
 from ondewo.s2t import speech_to_text_pb2 as ondewo_dot_s2t_dot_speech__to__text__pb2
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from ondewo.nlu import context_pb2 as ondewo_dot_nlu_dot_context__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16ondewo/vtsi/voip.proto\x12\x0bondewo.vtsi\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x18ondewo/nlu/context.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1fondewo/s2t/speech-to-text.proto\x1a\x1fondewo/t2s/text-to-speech.proto\x1a\x14ondewo/sip/sip.proto\"t\n\x0eProjectConfigs\x12\x13\n\x0bmax_callers\x18\x01 \x01(\x05\x12\x15\n\rmax_listeners\x18\x02 \x01(\x05\x12\x36\n\x10\x61sterisk_configs\x18\x03 \x01(\x0b\x32\x1c.ondewo.vtsi.AsteriskConfigs\"\xc1\x01\n\x18\x41steriskConfigsVariables\x12\x1a\n\x12sip_trunk_username\x18\x01 \x01(\t\x12\x1a\n\x12sip_trunk_password\x18\x02 \x01(\t\x12\x16\n\x0esip_trunk_host\x18\x03 \x01(\t\x12\x17\n\x0ftransfer_number\x18\x04 \x01(\t\x12\x1c\n\x14transfer_number_host\x18\x05 \x01(\t\x12\x1e\n\x16sip_trunk_phone_number\x18\x06 \x01(\t\"\x9c\x01\n\x14\x41steriskConfigsFiles\x12\x1c\n\x14sip_conf_file_string\x18\x01 \x01(\t\x12#\n\x1b\x65xtensions_conf_file_string\x18\x02 \x01(\t\x12\x1f\n\x17queues_conf_file_string\x18\x03 \x01(\t\x12 \n\x18modules_conf_file_string\x18\x04 \x01(\t\"\x86\x02\n\x0f\x41steriskConfigs\x12K\n\x1a\x61sterisk_configs_variables\x18\x01 \x01(\x0b\x32%.ondewo.vtsi.AsteriskConfigsVariablesH\x00\x12\x43\n\x16\x61sterisk_configs_files\x18\x02 \x01(\x0b\x32!.ondewo.vtsi.AsteriskConfigsFilesH\x00\x12\x30\n&asterisk_configs_target_directory_name\x18\x03 \x01(\tH\x00\x12\x15\n\rasterisk_port\x18\x04 \x01(\x05\x42\x18\n\x16\x61sterisk_configs_oneof\"g\n\x1b\x43reateProjectConfigsRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x34\n\x0fproject_configs\x18\x02 \x01(\x0b\x32\x1b.ondewo.vtsi.ProjectConfigs\".\n\x18GetProjectConfigsRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\"\xa1\x01\n\x19GetProjectConfigsResponse\x12\x34\n\x0fproject_configs\x18\x01 \x01(\x0b\x32\x1b.ondewo.vtsi.ProjectConfigs\x12\x16\n\x0e\x65rror_messages\x18\x02 \x01(\t\x12\x36\n\x07request\x18\x03 \x01(\x0b\x32%.ondewo.vtsi.GetProjectConfigsRequest\"g\n\x1bUpdateProjectConfigsRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x34\n\x0fproject_configs\x18\x02 \x01(\x0b\x32\x1b.ondewo.vtsi.ProjectConfigs\"1\n\x1b\x44\x65leteProjectConfigsRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\"*\n\x14\x44\x65ployProjectRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\",\n\x16UndeployProjectRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\"B\n\x11\x42\x61seServiceConfig\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x11\n\tgrpc_cert\x18\x03 \x01(\t\"5\n\x0b\x43redentials\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"\xef\x01\n\tNLUConfig\x12\x33\n\x0b\x62\x61se_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\x12/\n\x0b\x63redentials\x18\x02 \x01(\x0b\x32\x18.ondewo.vtsi.CredentialsH\x00\x12\x14\n\nauth_token\x18\x03 \x01(\tH\x00\x12\x15\n\rlanguage_code\x18\x04 \x01(\t\x12\x16\n\x0einitial_intent\x18\x05 \x01(\t\x12%\n\x08\x63ontexts\x18\x06 \x03(\x0b\x32\x13.ondewo.nlu.ContextB\x10\n\x0e\x61uthentication\"o\n\tT2SConfig\x12\x33\n\x0b\x62\x61se_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\x12-\n\nt2s_config\x18\x02 \x01(\x0b\x32\x19.ondewo.t2s.RequestConfig\"y\n\tS2TConfig\x12\x33\n\x0b\x62\x61se_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\x12\x37\n\ns2t_config\x18\x02 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\"E\n\x0e\x41steriskConfig\x12\x33\n\x0b\x62\x61se_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\"\xfd\x01\n\x15\x43ommonServicesConfigs\x12\x34\n\x0f\x61sterisk_config\x18\x01 \x01(\x0b\x32\x1b.ondewo.vtsi.AsteriskConfig\x12*\n\ncai_config\x18\x02 \x01(\x0b\x32\x16.ondewo.vtsi.NLUConfig\x12*\n\nstt_config\x18\x03 \x01(\x0b\x32\x16.ondewo.vtsi.S2TConfig\x12*\n\ntts_config\x18\x04 \x01(\x0b\x32\x16.ondewo.vtsi.T2SConfig\x12*\n\ncsi_config\x18\x05 \x01(\x0b\x32\x16.ondewo.vtsi.CsiConfig\"(\n\rSIPBaseConfig\x12\x17\n\x0fsip_sim_version\x18\x01 \x01(\t\"\xc8\x01\n\x0fSIPCallerConfig\x12\x33\n\x0fsip_base_config\x18\x01 \x01(\x0b\x32\x1a.ondewo.vtsi.SIPBaseConfig\x12\x14\n\x0cphone_number\x18\x02 \x01(\t\x12:\n\x07headers\x18\x03 \x03(\x0b\x32).ondewo.vtsi.SIPCallerConfig.HeadersEntry\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xcf\x02\n\tCsiConfig\x12\x30\n\rs2t_callbacks\x18\x01 \x01(\x0b\x32\x19.ondewo.vtsi.S2tCallbacks\x12\x30\n\rnlu_callbacks\x18\x02 \x01(\x0b\x32\x19.ondewo.vtsi.NluCallbacks\x12\x30\n\rt2s_callbacks\x18\x03 \x01(\x0b\x32\x19.ondewo.vtsi.T2sCallbacks\x12H\n\x19\x61udio_object_store_config\x18\x04 \x01(\x0b\x32%.ondewo.vtsi.AudioObjectStorageConfig\x12?\n\x15message_broker_config\x18\x05 \x01(\x0b\x32 .ondewo.vtsi.MessageBrokerConfig\x12!\n\x19\x61\x63tivate_control_messages\x18\x06 \x01(\x08\"\xfd\x01\n\x18\x41udioObjectStorageConfig\x12%\n\x1d\x61\x63tivate_audio_object_storage\x18\x01 \x01(\x08\x12p\n/audio_object_storage_services_activation_config\x18\x02 \x01(\x0b\x32\x37.ondewo.vtsi.AudioObjectStorageServicesActivationConfig\x12\x30\n\x0cminio_config\x18\x03 \x01(\x0b\x32\x18.ondewo.vtsi.MinioConfigH\x00\x42\x16\n\x14\x61udio_storage_config\"X\n*AudioObjectStorageServicesActivationConfig\x12\x14\n\x0c\x61\x63tivate_s2t\x18\x01 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_t2s\x18\x02 \x01(\x08\"\xef\x01\n\x13MessageBrokerConfig\x12\x1f\n\x17\x61\x63tivate_message_broker\x18\x01 \x01(\x08\x12\x65\n)message_broker_services_activation_config\x18\x02 \x01(\x0b\x32\x32.ondewo.vtsi.MessageBrokerServicesActivationConfig\x12\x37\n\x10rabbit_mq_config\x18\x03 \x01(\x0b\x32\x1b.ondewo.vtsi.RabbitMqConfigH\x00\x42\x17\n\x15message_broker_config\"\x7f\n%MessageBrokerServicesActivationConfig\x12\x14\n\x0c\x61\x63tivate_s2t\x18\x01 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_nlu\x18\x02 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_t2s\x18\x03 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_sip\x18\x04 \x01(\x08\"\\\n\x0eRabbitMqConfig\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\t\x12\x0e\n\x06port_2\x18\x03 \x01(\t\x12\x0c\n\x04user\x18\x04 \x01(\t\x12\x10\n\x08password\x18\x05 \x01(\t\"&\n\x08\x45ndpoint\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\t\"\x85\x01\n\x0bMinioConfig\x12\'\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32\x15.ondewo.vtsi.Endpoint\x12\x12\n\naccess_key\x18\x02 \x01(\t\x12\x12\n\nsecret_key\x18\x03 \x01(\t\x12\x0e\n\x06secure\x18\x04 \x01(\x08\x12\x15\n\rsession_token\x18\x05 \x01(\t\"E\n\x0cS2tCallbacks\x12\x19\n\x11pre_s2t_callbacks\x18\x01 \x03(\t\x12\x1a\n\x12post_s2t_callbacks\x18\x02 \x03(\t\"E\n\x0cNluCallbacks\x12\x19\n\x11pre_nlu_callbacks\x18\x01 \x03(\t\x12\x1a\n\x12post_nlu_callbacks\x18\x02 \x03(\t\"E\n\x0cT2sCallbacks\x12\x19\n\x11pre_t2s_callbacks\x18\x01 \x03(\t\x12\x1a\n\x12post_t2s_callbacks\x18\x02 \x03(\t\"\x84\x01\n\x14StartListenerRequest\x12.\n\nsip_config\x18\x01 \x01(\x0b\x32\x1a.ondewo.vtsi.SIPBaseConfig\x12<\n\x10services_configs\x18\x02 \x01(\x0b\x32\".ondewo.vtsi.CommonServicesConfigs\"\x84\x01\n\x12StartCallerRequest\x12\x30\n\nsip_config\x18\x01 \x01(\x0b\x32\x1c.ondewo.vtsi.SIPCallerConfig\x12<\n\x10services_configs\x18\x02 \x01(\x0b\x32\".ondewo.vtsi.CommonServicesConfigs\"\x83\x01\n\x1bStartScheduledCallerRequest\x12\x30\n\x07request\x18\x01 \x01(\x0b\x32\x1f.ondewo.vtsi.StartCallerRequest\x12\x32\n\x0escheduled_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"`\n\x15StartListenersRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x33\n\x08requests\x18\x02 \x03(\x0b\x32!.ondewo.vtsi.StartListenerRequest\">\n\x16StartListenersResponse\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61ll_ids\x18\x02 \x03(\t\"\\\n\x13StartCallersRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x31\n\x08requests\x18\x02 \x03(\x0b\x32\x1f.ondewo.vtsi.StartCallerRequest\"<\n\x14StartCallersResponse\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61ll_ids\x18\x02 \x03(\t\"n\n\x1cStartScheduledCallersRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12:\n\x08requests\x18\x02 \x03(\x0b\x32(.ondewo.vtsi.StartScheduledCallerRequest\"8\n\x10StopCallsRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61ll_ids\x18\x02 \x03(\t\")\n\x13StopAllCallsRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\"P\n\x14TransferCallsRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61ll_id\x18\x02 \x03(\t\x12\x13\n\x0btransfer_id\x18\x03 \x03(\t\"y\n\x16GetVoipCallInfoRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61ll_id\x18\x02 \x01(\t\x12:\n\x13voip_call_info_view\x18\x03 \x01(\x0e\x32\x1d.ondewo.vtsi.VoipCallInfoView\"v\n\x17GetVoipCallInfoResponse\x12-\n\nactive_log\x18\x01 \x01(\x0b\x32\x19.ondewo.vtsi.VoipCallInfo\x12,\n\tdone_logs\x18\x02 \x03(\x0b\x32\x19.ondewo.vtsi.VoipCallInfo\"\xdc\x02\n\x0cVoipCallInfo\x12\x0f\n\x07\x63\x61ll_id\x18\x01 \x01(\t\x12\x13\n\x0bsip_account\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_name\x18\x03 \x01(\t\x12(\n\tcall_type\x18\x04 \x01(\x0e\x32\x15.ondewo.vtsi.CallType\x12\x14\n\x0cphone_number\x18\x05 \x01(\t\x12\x12\n\nstart_time\x18\x06 \x01(\x01\x12\x10\n\x08\x65nd_time\x18\x07 \x01(\x01\x12)\n\nsip_status\x18\x08 \x01(\x0b\x32\x15.ondewo.sip.SipStatus\x12@\n\x12sip_status_history\x18\t \x01(\x0b\x32$.ondewo.sip.SipStatusHistoryResponse\x12;\n\x11services_statuses\x18\n \x01(\x0b\x32 .ondewo.vtsi.AllServicesStatuses\"\x93\x01\n\x17ListVoipCallInfoRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12:\n\x13voip_call_info_view\x18\x02 \x01(\x0e\x32\x1d.ondewo.vtsi.VoipCallInfoView\x12(\n\tcall_type\x18\x03 \x01(\x0e\x32\x15.ondewo.vtsi.CallType\"H\n\x18ListVoipCallInfoResponse\x12,\n\tvoip_info\x18\x01 \x03(\x0b\x32\x19.ondewo.vtsi.VoipCallInfo\"\x8a\x02\n\x13\x41llServicesStatuses\x12.\n\nstatus_sip\x18\x01 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12\x33\n\x0fstatus_asterisk\x18\x02 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12.\n\nstatus_cai\x18\x03 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12.\n\nstatus_stt\x18\x04 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12.\n\nstatus_tts\x18\x05 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\"9\n\rServiceStatus\x12\x0f\n\x07healthy\x18\x01 \x01(\x08\x12\x17\n\x0f\x65rror_messsages\x18\x02 \x01(\t\"o\n\x13GetAudioFileRequest\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x13\n\x0bobject_name\x18\x02 \x01(\t\x12.\n\x0cminio_config\x18\x03 \x01(\x0b\x32\x18.ondewo.vtsi.MinioConfig\"%\n\x14GetAudioFileResponse\x12\r\n\x05\x61udio\x18\x01 \x01(\x0c\"\x80\x01\n#GetFullConversationAudioFileRequest\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x14\n\x0cobject_names\x18\x02 \x03(\t\x12.\n\x0cminio_config\x18\x03 \x01(\x0b\x32\x18.ondewo.vtsi.MinioConfig\"5\n$GetFullConversationAudioFileResponse\x12\r\n\x05\x61udio\x18\x01 \x01(\x0c*=\n\x10VoipCallInfoView\x12\x15\n\x11Info_VIEW_SHALLOW\x10\x00\x12\x12\n\x0eInfo_VIEW_FULL\x10\x01*.\n\x08\x43\x61llType\x12\x08\n\x04\x62oth\x10\x00\x12\x0c\n\x08listener\x10\x01\x12\n\n\x06\x63\x61ller\x10\x02\x32\xa0\x0b\n\x0cVoipSessions\x12X\n\x14\x43reateProjectConfigs\x12(.ondewo.vtsi.CreateProjectConfigsRequest\x1a\x16.google.protobuf.Empty\x12\x62\n\x11GetProjectConfigs\x12%.ondewo.vtsi.GetProjectConfigsRequest\x1a&.ondewo.vtsi.GetProjectConfigsResponse\x12X\n\x14UpdateProjectConfigs\x12(.ondewo.vtsi.UpdateProjectConfigsRequest\x1a\x16.google.protobuf.Empty\x12X\n\x14\x44\x65leteProjectConfigs\x12(.ondewo.vtsi.DeleteProjectConfigsRequest\x1a\x16.google.protobuf.Empty\x12J\n\rDeployProject\x12!.ondewo.vtsi.DeployProjectRequest\x1a\x16.google.protobuf.Empty\x12N\n\x0fUndeployProject\x12#.ondewo.vtsi.UndeployProjectRequest\x1a\x16.google.protobuf.Empty\x12Y\n\x0eStartListeners\x12\".ondewo.vtsi.StartListenersRequest\x1a#.ondewo.vtsi.StartListenersResponse\x12S\n\x0cStartCallers\x12 .ondewo.vtsi.StartCallersRequest\x1a!.ondewo.vtsi.StartCallersResponse\x12Z\n\x15StartScheduledCallers\x12).ondewo.vtsi.StartScheduledCallersRequest\x1a\x16.google.protobuf.Empty\x12\x42\n\tStopCalls\x12\x1d.ondewo.vtsi.StopCallsRequest\x1a\x16.google.protobuf.Empty\x12H\n\x0cStopAllCalls\x12 .ondewo.vtsi.StopAllCallsRequest\x1a\x16.google.protobuf.Empty\x12J\n\rTransferCalls\x12!.ondewo.vtsi.TransferCallsRequest\x1a\x16.google.protobuf.Empty\x12\\\n\x0fGetVoipCallInfo\x12#.ondewo.vtsi.GetVoipCallInfoRequest\x1a$.ondewo.vtsi.GetVoipCallInfoResponse\x12_\n\x10ListVoipCallInfo\x12$.ondewo.vtsi.ListVoipCallInfoRequest\x1a%.ondewo.vtsi.ListVoipCallInfoResponse\x12U\n\x0cGetAudioFile\x12 .ondewo.vtsi.GetAudioFileRequest\x1a!.ondewo.vtsi.GetAudioFileResponse\"\x00\x12\x85\x01\n\x1cGetFullConversationAudioFile\x12\x30.ondewo.vtsi.GetFullConversationAudioFileRequest\x1a\x31.ondewo.vtsi.GetFullConversationAudioFileResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17ondewo/vtsi/calls.proto\x12\x0bondewo.vtsi\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x18ondewo/nlu/context.proto\x1a\x1fondewo/s2t/speech-to-text.proto\x1a\x1fondewo/t2s/text-to-speech.proto\x1a\x14ondewo/sip/sip.proto\"B\n\x11\x42\x61seServiceConfig\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x11\n\tgrpc_cert\x18\x03 \x01(\t\"5\n\x0b\x43redentials\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"\xaa\x02\n\rNluVtsiConfig\x12\x37\n\x0fnlu_base_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\x12/\n\x0b\x63redentials\x18\x02 \x01(\x0b\x32\x18.ondewo.vtsi.CredentialsH\x00\x12\x14\n\nauth_token\x18\x03 \x01(\tH\x00\x12\x12\n\nagent_name\x18\x04 \x01(\t\x12\x15\n\rlanguage_code\x18\x05 \x01(\t\x12\x16\n\x0einitial_intent\x18\x06 \x01(\t\x12%\n\x08\x63ontexts\x18\x07 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x1d\n\x15http_basic_auth_token\x18\x08 \x01(\tB\x10\n\x0e\x61uthentication\"\x7f\n\rT2sVtsiConfig\x12\x37\n\x0ft2s_base_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\x12\x35\n\x12t2s_request_config\x18\x02 \x01(\x0b\x32\x19.ondewo.t2s.RequestConfig\"\x94\x01\n\rS2tVtsiConfig\x12\x37\n\x0fs2t_base_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\x12J\n\x1ds2t_transcribe_request_config\x18\x02 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\"N\n\x0e\x41steriskConfig\x12<\n\x14\x61sterisk_base_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\"\xea\x01\n\x14\x43ommonServicesConfig\x12\x33\n\x0fs2t_vtsi_config\x18\x01 \x01(\x0b\x32\x1a.ondewo.vtsi.S2tVtsiConfig\x12\x33\n\x0fnlu_vtsi_config\x18\x02 \x01(\x0b\x32\x1a.ondewo.vtsi.NluVtsiConfig\x12\x33\n\x0ft2s_vtsi_config\x18\x03 \x01(\x0b\x32\x1a.ondewo.vtsi.T2sVtsiConfig\x12\x33\n\x0f\x63si_vtsi_config\x18\x04 \x01(\x0b\x32\x1a.ondewo.vtsi.CsiVtsiConfig\"(\n\rSipBaseConfig\x12\x17\n\x0fsip_sim_version\x18\x01 \x01(\t\"\xcf\x01\n\x0fSipCallerConfig\x12\x33\n\x0fsip_base_config\x18\x01 \x01(\x0b\x32\x1a.ondewo.vtsi.SipBaseConfig\x12\x11\n\tcallee_id\x18\x02 \x01(\t\x12\x41\n\x0bsip_headers\x18\x03 \x03(\x0b\x32,.ondewo.vtsi.SipCallerConfig.SipHeadersEntry\x1a\x31\n\x0fSipHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xee\x02\n\rCsiVtsiConfig\x12\x39\n\x12s2t_vtsi_callbacks\x18\x01 \x01(\x0b\x32\x1d.ondewo.vtsi.S2tVtsiCallbacks\x12\x39\n\x12nlu_vtsi_callbacks\x18\x02 \x01(\x0b\x32\x1d.ondewo.vtsi.NluVtsiCallbacks\x12\x39\n\x12t2s_vtsi_callbacks\x18\x03 \x01(\x0b\x32\x1d.ondewo.vtsi.T2sVtsiCallbacks\x12H\n\x19\x61udio_object_store_config\x18\x04 \x01(\x0b\x32%.ondewo.vtsi.AudioObjectStorageConfig\x12?\n\x15message_broker_config\x18\x05 \x01(\x0b\x32 .ondewo.vtsi.MessageBrokerConfig\x12!\n\x19\x61\x63tivate_control_messages\x18\x06 \x01(\x08\"\xfd\x01\n\x18\x41udioObjectStorageConfig\x12%\n\x1d\x61\x63tivate_audio_object_storage\x18\x01 \x01(\x08\x12p\n/audio_object_storage_services_activation_config\x18\x02 \x01(\x0b\x32\x37.ondewo.vtsi.AudioObjectStorageServicesActivationConfig\x12\x30\n\x0cminio_config\x18\x03 \x01(\x0b\x32\x18.ondewo.vtsi.MinioConfigH\x00\x42\x16\n\x14\x61udio_storage_config\"X\n*AudioObjectStorageServicesActivationConfig\x12\x14\n\x0c\x61\x63tivate_s2t\x18\x01 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_t2s\x18\x02 \x01(\x08\"\xef\x01\n\x13MessageBrokerConfig\x12\x1f\n\x17\x61\x63tivate_message_broker\x18\x01 \x01(\x08\x12\x65\n)message_broker_services_activation_config\x18\x02 \x01(\x0b\x32\x32.ondewo.vtsi.MessageBrokerServicesActivationConfig\x12\x37\n\x10rabbit_mq_config\x18\x03 \x01(\x0b\x32\x1b.ondewo.vtsi.RabbitMqConfigH\x00\x42\x17\n\x15message_broker_config\"\x7f\n%MessageBrokerServicesActivationConfig\x12\x14\n\x0c\x61\x63tivate_s2t\x18\x01 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_nlu\x18\x02 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_t2s\x18\x03 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_sip\x18\x04 \x01(\x08\"\\\n\x0eRabbitMqConfig\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x0e\n\x06port_2\x18\x03 \x01(\x05\x12\x0c\n\x04user\x18\x04 \x01(\t\x12\x10\n\x08password\x18\x05 \x01(\t\"x\n\x0bMinioConfig\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x12\n\naccess_key\x18\x03 \x01(\t\x12\x12\n\nsecret_key\x18\x04 \x01(\t\x12\x0e\n\x06secure\x18\x05 \x01(\x08\x12\x15\n\rsession_token\x18\x06 \x01(\t\"I\n\x10S2tVtsiCallbacks\x12\x19\n\x11pre_s2t_callbacks\x18\x01 \x03(\t\x12\x1a\n\x12post_s2t_callbacks\x18\x02 \x03(\t\"I\n\x10NluVtsiCallbacks\x12\x19\n\x11pre_nlu_callbacks\x18\x01 \x03(\t\x12\x1a\n\x12post_nlu_callbacks\x18\x02 \x03(\t\"I\n\x10T2sVtsiCallbacks\x12\x19\n\x11pre_t2s_callbacks\x18\x01 \x03(\t\x12\x1a\n\x12post_t2s_callbacks\x18\x02 \x03(\t\"\xa3\x01\n\x08Listener\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x33\n\x0fsip_base_config\x18\x03 \x01(\x0b\x32\x1a.ondewo.vtsi.SipBaseConfig\x12\x41\n\x16\x63ommon_services_config\x18\x04 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\"\xa5\x01\n\x06\x43\x61ller\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x37\n\x11sip_caller_config\x18\x03 \x01(\x0b\x32\x1c.ondewo.vtsi.SipCallerConfig\x12\x41\n\x16\x63ommon_services_config\x18\x04 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\"\xa9\x01\n\x14StartListenerRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x33\n\x0fsip_base_config\x18\x02 \x01(\x0b\x32\x1a.ondewo.vtsi.SipBaseConfig\x12\x41\n\x16\x63ommon_services_config\x18\x03 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\"r\n\x15StartListenerResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\'\n\x08listener\x18\x02 \x01(\x0b\x32\x15.ondewo.vtsi.Listener\x12\x15\n\rerror_message\x18\x03 \x01(\t\"p\n\x15StartListenersRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12<\n\x11listener_requests\x18\x02 \x03(\x0b\x32!.ondewo.vtsi.StartListenerRequest\"\x8a\x01\n\x16StartListenersResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12>\n\x12listener_responses\x18\x02 \x03(\x0b\x32\".ondewo.vtsi.StartListenerResponse\x12\x15\n\rerror_message\x18\x03 \x01(\t\"\xab\x01\n\x12StartCallerRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x37\n\x11sip_caller_config\x18\x02 \x01(\x0b\x32\x1c.ondewo.vtsi.SipCallerConfig\x12\x41\n\x16\x63ommon_services_config\x18\x03 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\"l\n\x13StartCallerResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12#\n\x06\x63\x61ller\x18\x02 \x01(\x0b\x32\x13.ondewo.vtsi.Caller\x12\x15\n\rerror_message\x18\x03 \x01(\t\"j\n\x13StartCallersRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x38\n\x0f\x63\x61ller_requests\x18\x02 \x03(\x0b\x32\x1f.ondewo.vtsi.StartCallerRequest\"\x84\x01\n\x14StartCallersResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12:\n\x10\x63\x61ller_responses\x18\x02 \x03(\x0b\x32 .ondewo.vtsi.StartCallerResponse\x12\x15\n\rerror_message\x18\x03 \x01(\t\"\x9e\x01\n\x1bStartScheduledCallerRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x30\n\x07request\x18\x02 \x01(\x0b\x32\x1f.ondewo.vtsi.StartCallerRequest\x12\x32\n\x0escheduled_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x86\x01\n\x1cStartScheduledCallersRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12K\n\x19scheduled_caller_requests\x18\x02 \x03(\x0b\x32(.ondewo.vtsi.StartScheduledCallerRequest\"\x89\x01\n\x1dStartScheduledCallersResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12M\n\x1ascheduled_caller_responses\x18\x02 \x03(\x0b\x32).ondewo.vtsi.StartScheduledCallerResponse\"\x88\x01\n\x1cStartScheduledCallerResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x36\n\x10scheduled_caller\x18\x02 \x01(\x0b\x32\x1c.ondewo.vtsi.ScheduledCaller\x12\x15\n\rerror_message\x18\x03 \x01(\t\"\xd9\x01\n\x0fScheduledCaller\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12.\n\nsip_config\x18\x03 \x01(\x0b\x32\x1a.ondewo.vtsi.SipBaseConfig\x12\x41\n\x16\x63ommon_services_config\x18\x04 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\x12\x32\n\x0escheduled_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"?\n\x0fStopCallRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\"W\n\x10StopCallResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x15\n\rerror_message\x18\x03 \x01(\t\"A\n\x10StopCallsRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x12\n\ncall_names\x18\x02 \x03(\t\"f\n\x11StopCallsResponse\x12:\n\x13stop_call_responses\x18\x01 \x03(\x0b\x32\x1d.ondewo.vtsi.StopCallResponse\x12\x15\n\rerror_message\x18\x02 \x01(\t\"0\n\x13StopAllCallsRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\"X\n\x13TransferCallRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x13\n\x0btransfer_id\x18\x03 \x03(\t\"p\n\x14TransferCallResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x13\n\x0btransfer_id\x18\x03 \x01(\t\x12\x15\n\rerror_message\x18\x04 \x01(\t\"s\n\x14TransferCallsRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12@\n\x16transfer_call_requests\x18\x02 \x03(\x0b\x32 .ondewo.vtsi.TransferCallRequest\"\x8d\x01\n\x15TransferCallsResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x42\n\x17transfer_call_responses\x18\x02 \x03(\x0b\x32!.ondewo.vtsi.TransferCallResponse\x12\x15\n\rerror_message\x18\x03 \x01(\t\"u\n\x12GetCallInfoRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x31\n\x0e\x63\x61ll_info_view\x18\x03 \x01(\x0e\x32\x19.ondewo.vtsi.CallInfoView\"j\n\x13GetCallInfoResponse\x12)\n\nactive_log\x18\x01 \x01(\x0b\x32\x15.ondewo.vtsi.CallInfo\x12(\n\tdone_logs\x18\x02 \x03(\x0b\x32\x15.ondewo.vtsi.CallInfo\"\x92\x03\n\x08\x43\x61llInfo\x12\x11\n\tcall_name\x18\x01 \x01(\t\x12\x13\n\x0bsip_account\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_name\x18\x03 \x01(\t\x12(\n\tcall_type\x18\x04 \x01(\x0e\x32\x15.ondewo.vtsi.CallType\x12\x14\n\x0cphone_number\x18\x05 \x01(\t\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\nsip_status\x18\x08 \x01(\x0b\x32\x15.ondewo.sip.SipStatus\x12@\n\x12sip_status_history\x18\t \x01(\x0b\x32$.ondewo.sip.SipStatusHistoryResponse\x12;\n\x11services_statuses\x18\n \x01(\x0b\x32 .ondewo.vtsi.AllServicesStatuses\"\x8d\x01\n\x13ListCallInfoRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x31\n\x0e\x63\x61ll_info_view\x18\x02 \x01(\x0e\x32\x19.ondewo.vtsi.CallInfoView\x12(\n\tcall_type\x18\x03 \x01(\x0e\x32\x15.ondewo.vtsi.CallType\"A\n\x14ListCallInfoResponse\x12)\n\ncall_infos\x18\x01 \x03(\x0b\x32\x15.ondewo.vtsi.CallInfo\"\x8a\x02\n\x13\x41llServicesStatuses\x12.\n\nstatus_sip\x18\x01 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12\x33\n\x0fstatus_asterisk\x18\x02 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12.\n\nstatus_nlu\x18\x03 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12.\n\nstatus_stt\x18\x04 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12.\n\nstatus_tts\x18\x05 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\"7\n\rServiceStatus\x12\x0f\n\x07healthy\x18\x01 \x01(\x08\x12\x15\n\rerror_message\x18\x02 \x01(\t\"o\n\x13GetAudioFileRequest\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x13\n\x0bobject_name\x18\x02 \x01(\t\x12.\n\x0cminio_config\x18\x03 \x01(\x0b\x32\x18.ondewo.vtsi.MinioConfig\"%\n\x14GetAudioFileResponse\x12\r\n\x05\x61udio\x18\x01 \x01(\x0c\"\x80\x01\n#GetFullConversationAudioFileRequest\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x14\n\x0cobject_names\x18\x02 \x03(\t\x12.\n\x0cminio_config\x18\x03 \x01(\x0b\x32\x18.ondewo.vtsi.MinioConfig\"5\n$GetFullConversationAudioFileResponse\x12\r\n\x05\x61udio\x18\x01 \x01(\x0c*%\n\x0c\x43\x61llInfoView\x12\x0b\n\x07SHALLOW\x10\x00\x12\x08\n\x04\x46ULL\x10\x01*.\n\x08\x43\x61llType\x12\x08\n\x04\x62oth\x10\x00\x12\x0c\n\x08listener\x10\x01\x12\n\n\x06\x63\x61ller\x10\x02\x32\xd6\n\n\x05\x43\x61lls\x12P\n\x0bStartCaller\x12\x1f.ondewo.vtsi.StartCallerRequest\x1a .ondewo.vtsi.StartCallerResponse\x12S\n\x0cStartCallers\x12 .ondewo.vtsi.StartCallersRequest\x1a!.ondewo.vtsi.StartCallersResponse\x12V\n\rStartListener\x12!.ondewo.vtsi.StartListenerRequest\x1a\".ondewo.vtsi.StartListenerResponse\x12Y\n\x0eStartListeners\x12\".ondewo.vtsi.StartListenersRequest\x1a#.ondewo.vtsi.StartListenersResponse\x12k\n\x14StartScheduledCaller\x12(.ondewo.vtsi.StartScheduledCallerRequest\x1a).ondewo.vtsi.StartScheduledCallerResponse\x12n\n\x15StartScheduledCallers\x12).ondewo.vtsi.StartScheduledCallersRequest\x1a*.ondewo.vtsi.StartScheduledCallersResponse\x12G\n\x08StopCall\x12\x1c.ondewo.vtsi.StopCallRequest\x1a\x1d.ondewo.vtsi.StopCallResponse\x12J\n\tStopCalls\x12\x1d.ondewo.vtsi.StopCallsRequest\x1a\x1e.ondewo.vtsi.StopCallsResponse\x12P\n\x0cStopAllCalls\x12 .ondewo.vtsi.StopAllCallsRequest\x1a\x1e.ondewo.vtsi.StopCallsResponse\x12S\n\x0cTransferCall\x12 .ondewo.vtsi.TransferCallRequest\x1a!.ondewo.vtsi.TransferCallResponse\x12V\n\rTransferCalls\x12!.ondewo.vtsi.TransferCallsRequest\x1a\".ondewo.vtsi.TransferCallsResponse\x12P\n\x0bGetCallInfo\x12\x1f.ondewo.vtsi.GetCallInfoRequest\x1a .ondewo.vtsi.GetCallInfoResponse\x12S\n\x0cListCallInfo\x12 .ondewo.vtsi.ListCallInfoRequest\x1a!.ondewo.vtsi.ListCallInfoResponse\x12S\n\x0cGetAudioFile\x12 .ondewo.vtsi.GetAudioFileRequest\x1a!.ondewo.vtsi.GetAudioFileResponse\x12\x85\x01\n\x1cGetFullConversationAudioFile\x12\x30.ondewo.vtsi.GetFullConversationAudioFileRequest\x1a\x31.ondewo.vtsi.GetFullConversationAudioFileResponse\"\x00\x62\x06proto3')
 
-_VOIPCALLINFOVIEW = DESCRIPTOR.enum_types_by_name['VoipCallInfoView']
-VoipCallInfoView = enum_type_wrapper.EnumTypeWrapper(_VOIPCALLINFOVIEW)
+_CALLINFOVIEW = DESCRIPTOR.enum_types_by_name['CallInfoView']
+CallInfoView = enum_type_wrapper.EnumTypeWrapper(_CALLINFOVIEW)
 _CALLTYPE = DESCRIPTOR.enum_types_by_name['CallType']
 CallType = enum_type_wrapper.EnumTypeWrapper(_CALLTYPE)
-Info_VIEW_SHALLOW = 0
-Info_VIEW_FULL = 1
+SHALLOW = 0
+FULL = 1
 both = 0
 listener = 1
 caller = 2
 
 
-_PROJECTCONFIGS = DESCRIPTOR.message_types_by_name['ProjectConfigs']
-_ASTERISKCONFIGSVARIABLES = DESCRIPTOR.message_types_by_name['AsteriskConfigsVariables']
-_ASTERISKCONFIGSFILES = DESCRIPTOR.message_types_by_name['AsteriskConfigsFiles']
-_ASTERISKCONFIGS = DESCRIPTOR.message_types_by_name['AsteriskConfigs']
-_CREATEPROJECTCONFIGSREQUEST = DESCRIPTOR.message_types_by_name['CreateProjectConfigsRequest']
-_GETPROJECTCONFIGSREQUEST = DESCRIPTOR.message_types_by_name['GetProjectConfigsRequest']
-_GETPROJECTCONFIGSRESPONSE = DESCRIPTOR.message_types_by_name['GetProjectConfigsResponse']
-_UPDATEPROJECTCONFIGSREQUEST = DESCRIPTOR.message_types_by_name['UpdateProjectConfigsRequest']
-_DELETEPROJECTCONFIGSREQUEST = DESCRIPTOR.message_types_by_name['DeleteProjectConfigsRequest']
-_DEPLOYPROJECTREQUEST = DESCRIPTOR.message_types_by_name['DeployProjectRequest']
-_UNDEPLOYPROJECTREQUEST = DESCRIPTOR.message_types_by_name['UndeployProjectRequest']
 _BASESERVICECONFIG = DESCRIPTOR.message_types_by_name['BaseServiceConfig']
 _CREDENTIALS = DESCRIPTOR.message_types_by_name['Credentials']
-_NLUCONFIG = DESCRIPTOR.message_types_by_name['NLUConfig']
-_T2SCONFIG = DESCRIPTOR.message_types_by_name['T2SConfig']
-_S2TCONFIG = DESCRIPTOR.message_types_by_name['S2TConfig']
+_NLUVTSICONFIG = DESCRIPTOR.message_types_by_name['NluVtsiConfig']
+_T2SVTSICONFIG = DESCRIPTOR.message_types_by_name['T2sVtsiConfig']
+_S2TVTSICONFIG = DESCRIPTOR.message_types_by_name['S2tVtsiConfig']
 _ASTERISKCONFIG = DESCRIPTOR.message_types_by_name['AsteriskConfig']
-_COMMONSERVICESCONFIGS = DESCRIPTOR.message_types_by_name['CommonServicesConfigs']
-_SIPBASECONFIG = DESCRIPTOR.message_types_by_name['SIPBaseConfig']
-_SIPCALLERCONFIG = DESCRIPTOR.message_types_by_name['SIPCallerConfig']
-_SIPCALLERCONFIG_HEADERSENTRY = _SIPCALLERCONFIG.nested_types_by_name['HeadersEntry']
-_CSICONFIG = DESCRIPTOR.message_types_by_name['CsiConfig']
+_COMMONSERVICESCONFIG = DESCRIPTOR.message_types_by_name['CommonServicesConfig']
+_SIPBASECONFIG = DESCRIPTOR.message_types_by_name['SipBaseConfig']
+_SIPCALLERCONFIG = DESCRIPTOR.message_types_by_name['SipCallerConfig']
+_SIPCALLERCONFIG_SIPHEADERSENTRY = _SIPCALLERCONFIG.nested_types_by_name['SipHeadersEntry']
+_CSIVTSICONFIG = DESCRIPTOR.message_types_by_name['CsiVtsiConfig']
 _AUDIOOBJECTSTORAGECONFIG = DESCRIPTOR.message_types_by_name['AudioObjectStorageConfig']
 _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG = DESCRIPTOR.message_types_by_name['AudioObjectStorageServicesActivationConfig']
 _MESSAGEBROKERCONFIG = DESCRIPTOR.message_types_by_name['MessageBrokerConfig']
 _MESSAGEBROKERSERVICESACTIVATIONCONFIG = DESCRIPTOR.message_types_by_name['MessageBrokerServicesActivationConfig']
 _RABBITMQCONFIG = DESCRIPTOR.message_types_by_name['RabbitMqConfig']
-_ENDPOINT = DESCRIPTOR.message_types_by_name['Endpoint']
 _MINIOCONFIG = DESCRIPTOR.message_types_by_name['MinioConfig']
-_S2TCALLBACKS = DESCRIPTOR.message_types_by_name['S2tCallbacks']
-_NLUCALLBACKS = DESCRIPTOR.message_types_by_name['NluCallbacks']
-_T2SCALLBACKS = DESCRIPTOR.message_types_by_name['T2sCallbacks']
+_S2TVTSICALLBACKS = DESCRIPTOR.message_types_by_name['S2tVtsiCallbacks']
+_NLUVTSICALLBACKS = DESCRIPTOR.message_types_by_name['NluVtsiCallbacks']
+_T2SVTSICALLBACKS = DESCRIPTOR.message_types_by_name['T2sVtsiCallbacks']
+_LISTENER = DESCRIPTOR.message_types_by_name['Listener']
+_CALLER = DESCRIPTOR.message_types_by_name['Caller']
 _STARTLISTENERREQUEST = DESCRIPTOR.message_types_by_name['StartListenerRequest']
-_STARTCALLERREQUEST = DESCRIPTOR.message_types_by_name['StartCallerRequest']
-_STARTSCHEDULEDCALLERREQUEST = DESCRIPTOR.message_types_by_name['StartScheduledCallerRequest']
+_STARTLISTENERRESPONSE = DESCRIPTOR.message_types_by_name['StartListenerResponse']
 _STARTLISTENERSREQUEST = DESCRIPTOR.message_types_by_name['StartListenersRequest']
 _STARTLISTENERSRESPONSE = DESCRIPTOR.message_types_by_name['StartListenersResponse']
+_STARTCALLERREQUEST = DESCRIPTOR.message_types_by_name['StartCallerRequest']
+_STARTCALLERRESPONSE = DESCRIPTOR.message_types_by_name['StartCallerResponse']
 _STARTCALLERSREQUEST = DESCRIPTOR.message_types_by_name['StartCallersRequest']
 _STARTCALLERSRESPONSE = DESCRIPTOR.message_types_by_name['StartCallersResponse']
+_STARTSCHEDULEDCALLERREQUEST = DESCRIPTOR.message_types_by_name['StartScheduledCallerRequest']
 _STARTSCHEDULEDCALLERSREQUEST = DESCRIPTOR.message_types_by_name['StartScheduledCallersRequest']
+_STARTSCHEDULEDCALLERSRESPONSE = DESCRIPTOR.message_types_by_name['StartScheduledCallersResponse']
+_STARTSCHEDULEDCALLERRESPONSE = DESCRIPTOR.message_types_by_name['StartScheduledCallerResponse']
+_SCHEDULEDCALLER = DESCRIPTOR.message_types_by_name['ScheduledCaller']
+_STOPCALLREQUEST = DESCRIPTOR.message_types_by_name['StopCallRequest']
+_STOPCALLRESPONSE = DESCRIPTOR.message_types_by_name['StopCallResponse']
 _STOPCALLSREQUEST = DESCRIPTOR.message_types_by_name['StopCallsRequest']
+_STOPCALLSRESPONSE = DESCRIPTOR.message_types_by_name['StopCallsResponse']
 _STOPALLCALLSREQUEST = DESCRIPTOR.message_types_by_name['StopAllCallsRequest']
+_TRANSFERCALLREQUEST = DESCRIPTOR.message_types_by_name['TransferCallRequest']
+_TRANSFERCALLRESPONSE = DESCRIPTOR.message_types_by_name['TransferCallResponse']
 _TRANSFERCALLSREQUEST = DESCRIPTOR.message_types_by_name['TransferCallsRequest']
-_GETVOIPCALLINFOREQUEST = DESCRIPTOR.message_types_by_name['GetVoipCallInfoRequest']
-_GETVOIPCALLINFORESPONSE = DESCRIPTOR.message_types_by_name['GetVoipCallInfoResponse']
-_VOIPCALLINFO = DESCRIPTOR.message_types_by_name['VoipCallInfo']
-_LISTVOIPCALLINFOREQUEST = DESCRIPTOR.message_types_by_name['ListVoipCallInfoRequest']
-_LISTVOIPCALLINFORESPONSE = DESCRIPTOR.message_types_by_name['ListVoipCallInfoResponse']
+_TRANSFERCALLSRESPONSE = DESCRIPTOR.message_types_by_name['TransferCallsResponse']
+_GETCALLINFOREQUEST = DESCRIPTOR.message_types_by_name['GetCallInfoRequest']
+_GETCALLINFORESPONSE = DESCRIPTOR.message_types_by_name['GetCallInfoResponse']
+_CALLINFO = DESCRIPTOR.message_types_by_name['CallInfo']
+_LISTCALLINFOREQUEST = DESCRIPTOR.message_types_by_name['ListCallInfoRequest']
+_LISTCALLINFORESPONSE = DESCRIPTOR.message_types_by_name['ListCallInfoResponse']
 _ALLSERVICESSTATUSES = DESCRIPTOR.message_types_by_name['AllServicesStatuses']
 _SERVICESTATUS = DESCRIPTOR.message_types_by_name['ServiceStatus']
 _GETAUDIOFILEREQUEST = DESCRIPTOR.message_types_by_name['GetAudioFileRequest']
 _GETAUDIOFILERESPONSE = DESCRIPTOR.message_types_by_name['GetAudioFileResponse']
 _GETFULLCONVERSATIONAUDIOFILEREQUEST = DESCRIPTOR.message_types_by_name['GetFullConversationAudioFileRequest']
 _GETFULLCONVERSATIONAUDIOFILERESPONSE = DESCRIPTOR.message_types_by_name['GetFullConversationAudioFileResponse']
-ProjectConfigs = _reflection.GeneratedProtocolMessageType('ProjectConfigs', (_message.Message,), {
-    'DESCRIPTOR': _PROJECTCONFIGS,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ProjectConfigs)
-})
-_sym_db.RegisterMessage(ProjectConfigs)
-
-AsteriskConfigsVariables = _reflection.GeneratedProtocolMessageType('AsteriskConfigsVariables', (_message.Message,), {
-    'DESCRIPTOR': _ASTERISKCONFIGSVARIABLES,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.AsteriskConfigsVariables)
-})
-_sym_db.RegisterMessage(AsteriskConfigsVariables)
-
-AsteriskConfigsFiles = _reflection.GeneratedProtocolMessageType('AsteriskConfigsFiles', (_message.Message,), {
-    'DESCRIPTOR': _ASTERISKCONFIGSFILES,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.AsteriskConfigsFiles)
-})
-_sym_db.RegisterMessage(AsteriskConfigsFiles)
-
-AsteriskConfigs = _reflection.GeneratedProtocolMessageType('AsteriskConfigs', (_message.Message,), {
-    'DESCRIPTOR': _ASTERISKCONFIGS,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.AsteriskConfigs)
-})
-_sym_db.RegisterMessage(AsteriskConfigs)
-
-CreateProjectConfigsRequest = _reflection.GeneratedProtocolMessageType('CreateProjectConfigsRequest', (_message.Message,), {
-    'DESCRIPTOR': _CREATEPROJECTCONFIGSREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.CreateProjectConfigsRequest)
-})
-_sym_db.RegisterMessage(CreateProjectConfigsRequest)
-
-GetProjectConfigsRequest = _reflection.GeneratedProtocolMessageType('GetProjectConfigsRequest', (_message.Message,), {
-    'DESCRIPTOR': _GETPROJECTCONFIGSREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetProjectConfigsRequest)
-})
-_sym_db.RegisterMessage(GetProjectConfigsRequest)
-
-GetProjectConfigsResponse = _reflection.GeneratedProtocolMessageType('GetProjectConfigsResponse', (_message.Message,), {
-    'DESCRIPTOR': _GETPROJECTCONFIGSRESPONSE,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetProjectConfigsResponse)
-})
-_sym_db.RegisterMessage(GetProjectConfigsResponse)
-
-UpdateProjectConfigsRequest = _reflection.GeneratedProtocolMessageType('UpdateProjectConfigsRequest', (_message.Message,), {
-    'DESCRIPTOR': _UPDATEPROJECTCONFIGSREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.UpdateProjectConfigsRequest)
-})
-_sym_db.RegisterMessage(UpdateProjectConfigsRequest)
-
-DeleteProjectConfigsRequest = _reflection.GeneratedProtocolMessageType('DeleteProjectConfigsRequest', (_message.Message,), {
-    'DESCRIPTOR': _DELETEPROJECTCONFIGSREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.DeleteProjectConfigsRequest)
-})
-_sym_db.RegisterMessage(DeleteProjectConfigsRequest)
-
-DeployProjectRequest = _reflection.GeneratedProtocolMessageType('DeployProjectRequest', (_message.Message,), {
-    'DESCRIPTOR': _DEPLOYPROJECTREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.DeployProjectRequest)
-})
-_sym_db.RegisterMessage(DeployProjectRequest)
-
-UndeployProjectRequest = _reflection.GeneratedProtocolMessageType('UndeployProjectRequest', (_message.Message,), {
-    'DESCRIPTOR': _UNDEPLOYPROJECTREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.UndeployProjectRequest)
-})
-_sym_db.RegisterMessage(UndeployProjectRequest)
-
 BaseServiceConfig = _reflection.GeneratedProtocolMessageType('BaseServiceConfig', (_message.Message,), {
     'DESCRIPTOR': _BASESERVICECONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.BaseServiceConfig)
 })
 _sym_db.RegisterMessage(BaseServiceConfig)
 
 Credentials = _reflection.GeneratedProtocolMessageType('Credentials', (_message.Message,), {
     'DESCRIPTOR': _CREDENTIALS,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.Credentials)
 })
 _sym_db.RegisterMessage(Credentials)
 
-NLUConfig = _reflection.GeneratedProtocolMessageType('NLUConfig', (_message.Message,), {
-    'DESCRIPTOR': _NLUCONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.NLUConfig)
-})
-_sym_db.RegisterMessage(NLUConfig)
-
-T2SConfig = _reflection.GeneratedProtocolMessageType('T2SConfig', (_message.Message,), {
-    'DESCRIPTOR': _T2SCONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.T2SConfig)
-})
-_sym_db.RegisterMessage(T2SConfig)
-
-S2TConfig = _reflection.GeneratedProtocolMessageType('S2TConfig', (_message.Message,), {
-    'DESCRIPTOR': _S2TCONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.S2TConfig)
+NluVtsiConfig = _reflection.GeneratedProtocolMessageType('NluVtsiConfig', (_message.Message,), {
+    'DESCRIPTOR': _NLUVTSICONFIG,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.NluVtsiConfig)
+})
+_sym_db.RegisterMessage(NluVtsiConfig)
+
+T2sVtsiConfig = _reflection.GeneratedProtocolMessageType('T2sVtsiConfig', (_message.Message,), {
+    'DESCRIPTOR': _T2SVTSICONFIG,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.T2sVtsiConfig)
+})
+_sym_db.RegisterMessage(T2sVtsiConfig)
+
+S2tVtsiConfig = _reflection.GeneratedProtocolMessageType('S2tVtsiConfig', (_message.Message,), {
+    'DESCRIPTOR': _S2TVTSICONFIG,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.S2tVtsiConfig)
 })
-_sym_db.RegisterMessage(S2TConfig)
+_sym_db.RegisterMessage(S2tVtsiConfig)
 
 AsteriskConfig = _reflection.GeneratedProtocolMessageType('AsteriskConfig', (_message.Message,), {
     'DESCRIPTOR': _ASTERISKCONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.AsteriskConfig)
 })
 _sym_db.RegisterMessage(AsteriskConfig)
 
-CommonServicesConfigs = _reflection.GeneratedProtocolMessageType('CommonServicesConfigs', (_message.Message,), {
-    'DESCRIPTOR': _COMMONSERVICESCONFIGS,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.CommonServicesConfigs)
+CommonServicesConfig = _reflection.GeneratedProtocolMessageType('CommonServicesConfig', (_message.Message,), {
+    'DESCRIPTOR': _COMMONSERVICESCONFIG,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.CommonServicesConfig)
 })
-_sym_db.RegisterMessage(CommonServicesConfigs)
+_sym_db.RegisterMessage(CommonServicesConfig)
 
-SIPBaseConfig = _reflection.GeneratedProtocolMessageType('SIPBaseConfig', (_message.Message,), {
+SipBaseConfig = _reflection.GeneratedProtocolMessageType('SipBaseConfig', (_message.Message,), {
     'DESCRIPTOR': _SIPBASECONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.SIPBaseConfig)
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.SipBaseConfig)
 })
-_sym_db.RegisterMessage(SIPBaseConfig)
+_sym_db.RegisterMessage(SipBaseConfig)
 
-SIPCallerConfig = _reflection.GeneratedProtocolMessageType('SIPCallerConfig', (_message.Message,), {
+SipCallerConfig = _reflection.GeneratedProtocolMessageType('SipCallerConfig', (_message.Message,), {
 
-    'HeadersEntry': _reflection.GeneratedProtocolMessageType('HeadersEntry', (_message.Message,), {
-        'DESCRIPTOR': _SIPCALLERCONFIG_HEADERSENTRY,
-        '__module__': 'ondewo.vtsi.voip_pb2'
-        # @@protoc_insertion_point(class_scope:ondewo.vtsi.SIPCallerConfig.HeadersEntry)
+    'SipHeadersEntry': _reflection.GeneratedProtocolMessageType('SipHeadersEntry', (_message.Message,), {
+        'DESCRIPTOR': _SIPCALLERCONFIG_SIPHEADERSENTRY,
+        '__module__': 'ondewo.vtsi.calls_pb2'
+        # @@protoc_insertion_point(class_scope:ondewo.vtsi.SipCallerConfig.SipHeadersEntry)
     }),
     'DESCRIPTOR': _SIPCALLERCONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.SIPCallerConfig)
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.SipCallerConfig)
 })
-_sym_db.RegisterMessage(SIPCallerConfig)
-_sym_db.RegisterMessage(SIPCallerConfig.HeadersEntry)
+_sym_db.RegisterMessage(SipCallerConfig)
+_sym_db.RegisterMessage(SipCallerConfig.SipHeadersEntry)
 
-CsiConfig = _reflection.GeneratedProtocolMessageType('CsiConfig', (_message.Message,), {
-    'DESCRIPTOR': _CSICONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.CsiConfig)
+CsiVtsiConfig = _reflection.GeneratedProtocolMessageType('CsiVtsiConfig', (_message.Message,), {
+    'DESCRIPTOR': _CSIVTSICONFIG,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.CsiVtsiConfig)
 })
-_sym_db.RegisterMessage(CsiConfig)
+_sym_db.RegisterMessage(CsiVtsiConfig)
 
 AudioObjectStorageConfig = _reflection.GeneratedProtocolMessageType('AudioObjectStorageConfig', (_message.Message,), {
     'DESCRIPTOR': _AUDIOOBJECTSTORAGECONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.AudioObjectStorageConfig)
 })
 _sym_db.RegisterMessage(AudioObjectStorageConfig)
 
 AudioObjectStorageServicesActivationConfig = _reflection.GeneratedProtocolMessageType('AudioObjectStorageServicesActivationConfig', (_message.Message,), {
     'DESCRIPTOR': _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.AudioObjectStorageServicesActivationConfig)
 })
 _sym_db.RegisterMessage(AudioObjectStorageServicesActivationConfig)
 
 MessageBrokerConfig = _reflection.GeneratedProtocolMessageType('MessageBrokerConfig', (_message.Message,), {
     'DESCRIPTOR': _MESSAGEBROKERCONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.MessageBrokerConfig)
 })
 _sym_db.RegisterMessage(MessageBrokerConfig)
 
 MessageBrokerServicesActivationConfig = _reflection.GeneratedProtocolMessageType('MessageBrokerServicesActivationConfig', (_message.Message,), {
     'DESCRIPTOR': _MESSAGEBROKERSERVICESACTIVATIONCONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.MessageBrokerServicesActivationConfig)
 })
 _sym_db.RegisterMessage(MessageBrokerServicesActivationConfig)
 
 RabbitMqConfig = _reflection.GeneratedProtocolMessageType('RabbitMqConfig', (_message.Message,), {
     'DESCRIPTOR': _RABBITMQCONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.RabbitMqConfig)
 })
 _sym_db.RegisterMessage(RabbitMqConfig)
 
-Endpoint = _reflection.GeneratedProtocolMessageType('Endpoint', (_message.Message,), {
-    'DESCRIPTOR': _ENDPOINT,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.Endpoint)
-})
-_sym_db.RegisterMessage(Endpoint)
-
 MinioConfig = _reflection.GeneratedProtocolMessageType('MinioConfig', (_message.Message,), {
     'DESCRIPTOR': _MINIOCONFIG,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.MinioConfig)
 })
 _sym_db.RegisterMessage(MinioConfig)
 
-S2tCallbacks = _reflection.GeneratedProtocolMessageType('S2tCallbacks', (_message.Message,), {
-    'DESCRIPTOR': _S2TCALLBACKS,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.S2tCallbacks)
-})
-_sym_db.RegisterMessage(S2tCallbacks)
-
-NluCallbacks = _reflection.GeneratedProtocolMessageType('NluCallbacks', (_message.Message,), {
-    'DESCRIPTOR': _NLUCALLBACKS,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.NluCallbacks)
-})
-_sym_db.RegisterMessage(NluCallbacks)
-
-T2sCallbacks = _reflection.GeneratedProtocolMessageType('T2sCallbacks', (_message.Message,), {
-    'DESCRIPTOR': _T2SCALLBACKS,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.T2sCallbacks)
+S2tVtsiCallbacks = _reflection.GeneratedProtocolMessageType('S2tVtsiCallbacks', (_message.Message,), {
+    'DESCRIPTOR': _S2TVTSICALLBACKS,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.S2tVtsiCallbacks)
 })
-_sym_db.RegisterMessage(T2sCallbacks)
+_sym_db.RegisterMessage(S2tVtsiCallbacks)
+
+NluVtsiCallbacks = _reflection.GeneratedProtocolMessageType('NluVtsiCallbacks', (_message.Message,), {
+    'DESCRIPTOR': _NLUVTSICALLBACKS,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.NluVtsiCallbacks)
+})
+_sym_db.RegisterMessage(NluVtsiCallbacks)
+
+T2sVtsiCallbacks = _reflection.GeneratedProtocolMessageType('T2sVtsiCallbacks', (_message.Message,), {
+    'DESCRIPTOR': _T2SVTSICALLBACKS,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.T2sVtsiCallbacks)
+})
+_sym_db.RegisterMessage(T2sVtsiCallbacks)
+
+Listener = _reflection.GeneratedProtocolMessageType('Listener', (_message.Message,), {
+    'DESCRIPTOR': _LISTENER,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.Listener)
+})
+_sym_db.RegisterMessage(Listener)
+
+Caller = _reflection.GeneratedProtocolMessageType('Caller', (_message.Message,), {
+    'DESCRIPTOR': _CALLER,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.Caller)
+})
+_sym_db.RegisterMessage(Caller)
 
 StartListenerRequest = _reflection.GeneratedProtocolMessageType('StartListenerRequest', (_message.Message,), {
     'DESCRIPTOR': _STARTLISTENERREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartListenerRequest)
 })
 _sym_db.RegisterMessage(StartListenerRequest)
 
-StartCallerRequest = _reflection.GeneratedProtocolMessageType('StartCallerRequest', (_message.Message,), {
-    'DESCRIPTOR': _STARTCALLERREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartCallerRequest)
-})
-_sym_db.RegisterMessage(StartCallerRequest)
-
-StartScheduledCallerRequest = _reflection.GeneratedProtocolMessageType('StartScheduledCallerRequest', (_message.Message,), {
-    'DESCRIPTOR': _STARTSCHEDULEDCALLERREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartScheduledCallerRequest)
+StartListenerResponse = _reflection.GeneratedProtocolMessageType('StartListenerResponse', (_message.Message,), {
+    'DESCRIPTOR': _STARTLISTENERRESPONSE,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartListenerResponse)
 })
-_sym_db.RegisterMessage(StartScheduledCallerRequest)
+_sym_db.RegisterMessage(StartListenerResponse)
 
 StartListenersRequest = _reflection.GeneratedProtocolMessageType('StartListenersRequest', (_message.Message,), {
     'DESCRIPTOR': _STARTLISTENERSREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartListenersRequest)
 })
 _sym_db.RegisterMessage(StartListenersRequest)
 
 StartListenersResponse = _reflection.GeneratedProtocolMessageType('StartListenersResponse', (_message.Message,), {
     'DESCRIPTOR': _STARTLISTENERSRESPONSE,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartListenersResponse)
 })
 _sym_db.RegisterMessage(StartListenersResponse)
 
+StartCallerRequest = _reflection.GeneratedProtocolMessageType('StartCallerRequest', (_message.Message,), {
+    'DESCRIPTOR': _STARTCALLERREQUEST,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartCallerRequest)
+})
+_sym_db.RegisterMessage(StartCallerRequest)
+
+StartCallerResponse = _reflection.GeneratedProtocolMessageType('StartCallerResponse', (_message.Message,), {
+    'DESCRIPTOR': _STARTCALLERRESPONSE,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartCallerResponse)
+})
+_sym_db.RegisterMessage(StartCallerResponse)
+
 StartCallersRequest = _reflection.GeneratedProtocolMessageType('StartCallersRequest', (_message.Message,), {
     'DESCRIPTOR': _STARTCALLERSREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartCallersRequest)
 })
 _sym_db.RegisterMessage(StartCallersRequest)
 
 StartCallersResponse = _reflection.GeneratedProtocolMessageType('StartCallersResponse', (_message.Message,), {
     'DESCRIPTOR': _STARTCALLERSRESPONSE,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartCallersResponse)
 })
 _sym_db.RegisterMessage(StartCallersResponse)
 
+StartScheduledCallerRequest = _reflection.GeneratedProtocolMessageType('StartScheduledCallerRequest', (_message.Message,), {
+    'DESCRIPTOR': _STARTSCHEDULEDCALLERREQUEST,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartScheduledCallerRequest)
+})
+_sym_db.RegisterMessage(StartScheduledCallerRequest)
+
 StartScheduledCallersRequest = _reflection.GeneratedProtocolMessageType('StartScheduledCallersRequest', (_message.Message,), {
     'DESCRIPTOR': _STARTSCHEDULEDCALLERSREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartScheduledCallersRequest)
 })
 _sym_db.RegisterMessage(StartScheduledCallersRequest)
 
+StartScheduledCallersResponse = _reflection.GeneratedProtocolMessageType('StartScheduledCallersResponse', (_message.Message,), {
+    'DESCRIPTOR': _STARTSCHEDULEDCALLERSRESPONSE,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartScheduledCallersResponse)
+})
+_sym_db.RegisterMessage(StartScheduledCallersResponse)
+
+StartScheduledCallerResponse = _reflection.GeneratedProtocolMessageType('StartScheduledCallerResponse', (_message.Message,), {
+    'DESCRIPTOR': _STARTSCHEDULEDCALLERRESPONSE,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartScheduledCallerResponse)
+})
+_sym_db.RegisterMessage(StartScheduledCallerResponse)
+
+ScheduledCaller = _reflection.GeneratedProtocolMessageType('ScheduledCaller', (_message.Message,), {
+    'DESCRIPTOR': _SCHEDULEDCALLER,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ScheduledCaller)
+})
+_sym_db.RegisterMessage(ScheduledCaller)
+
+StopCallRequest = _reflection.GeneratedProtocolMessageType('StopCallRequest', (_message.Message,), {
+    'DESCRIPTOR': _STOPCALLREQUEST,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.StopCallRequest)
+})
+_sym_db.RegisterMessage(StopCallRequest)
+
+StopCallResponse = _reflection.GeneratedProtocolMessageType('StopCallResponse', (_message.Message,), {
+    'DESCRIPTOR': _STOPCALLRESPONSE,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.StopCallResponse)
+})
+_sym_db.RegisterMessage(StopCallResponse)
+
 StopCallsRequest = _reflection.GeneratedProtocolMessageType('StopCallsRequest', (_message.Message,), {
     'DESCRIPTOR': _STOPCALLSREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.StopCallsRequest)
 })
 _sym_db.RegisterMessage(StopCallsRequest)
 
+StopCallsResponse = _reflection.GeneratedProtocolMessageType('StopCallsResponse', (_message.Message,), {
+    'DESCRIPTOR': _STOPCALLSRESPONSE,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.StopCallsResponse)
+})
+_sym_db.RegisterMessage(StopCallsResponse)
+
 StopAllCallsRequest = _reflection.GeneratedProtocolMessageType('StopAllCallsRequest', (_message.Message,), {
     'DESCRIPTOR': _STOPALLCALLSREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.StopAllCallsRequest)
 })
 _sym_db.RegisterMessage(StopAllCallsRequest)
 
+TransferCallRequest = _reflection.GeneratedProtocolMessageType('TransferCallRequest', (_message.Message,), {
+    'DESCRIPTOR': _TRANSFERCALLREQUEST,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.TransferCallRequest)
+})
+_sym_db.RegisterMessage(TransferCallRequest)
+
+TransferCallResponse = _reflection.GeneratedProtocolMessageType('TransferCallResponse', (_message.Message,), {
+    'DESCRIPTOR': _TRANSFERCALLRESPONSE,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.TransferCallResponse)
+})
+_sym_db.RegisterMessage(TransferCallResponse)
+
 TransferCallsRequest = _reflection.GeneratedProtocolMessageType('TransferCallsRequest', (_message.Message,), {
     'DESCRIPTOR': _TRANSFERCALLSREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.TransferCallsRequest)
 })
 _sym_db.RegisterMessage(TransferCallsRequest)
 
-GetVoipCallInfoRequest = _reflection.GeneratedProtocolMessageType('GetVoipCallInfoRequest', (_message.Message,), {
-    'DESCRIPTOR': _GETVOIPCALLINFOREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetVoipCallInfoRequest)
+TransferCallsResponse = _reflection.GeneratedProtocolMessageType('TransferCallsResponse', (_message.Message,), {
+    'DESCRIPTOR': _TRANSFERCALLSRESPONSE,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.TransferCallsResponse)
+})
+_sym_db.RegisterMessage(TransferCallsResponse)
+
+GetCallInfoRequest = _reflection.GeneratedProtocolMessageType('GetCallInfoRequest', (_message.Message,), {
+    'DESCRIPTOR': _GETCALLINFOREQUEST,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetCallInfoRequest)
 })
-_sym_db.RegisterMessage(GetVoipCallInfoRequest)
+_sym_db.RegisterMessage(GetCallInfoRequest)
 
-GetVoipCallInfoResponse = _reflection.GeneratedProtocolMessageType('GetVoipCallInfoResponse', (_message.Message,), {
-    'DESCRIPTOR': _GETVOIPCALLINFORESPONSE,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetVoipCallInfoResponse)
+GetCallInfoResponse = _reflection.GeneratedProtocolMessageType('GetCallInfoResponse', (_message.Message,), {
+    'DESCRIPTOR': _GETCALLINFORESPONSE,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetCallInfoResponse)
 })
-_sym_db.RegisterMessage(GetVoipCallInfoResponse)
+_sym_db.RegisterMessage(GetCallInfoResponse)
 
-VoipCallInfo = _reflection.GeneratedProtocolMessageType('VoipCallInfo', (_message.Message,), {
-    'DESCRIPTOR': _VOIPCALLINFO,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.VoipCallInfo)
+CallInfo = _reflection.GeneratedProtocolMessageType('CallInfo', (_message.Message,), {
+    'DESCRIPTOR': _CALLINFO,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.CallInfo)
 })
-_sym_db.RegisterMessage(VoipCallInfo)
+_sym_db.RegisterMessage(CallInfo)
 
-ListVoipCallInfoRequest = _reflection.GeneratedProtocolMessageType('ListVoipCallInfoRequest', (_message.Message,), {
-    'DESCRIPTOR': _LISTVOIPCALLINFOREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ListVoipCallInfoRequest)
+ListCallInfoRequest = _reflection.GeneratedProtocolMessageType('ListCallInfoRequest', (_message.Message,), {
+    'DESCRIPTOR': _LISTCALLINFOREQUEST,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ListCallInfoRequest)
 })
-_sym_db.RegisterMessage(ListVoipCallInfoRequest)
+_sym_db.RegisterMessage(ListCallInfoRequest)
 
-ListVoipCallInfoResponse = _reflection.GeneratedProtocolMessageType('ListVoipCallInfoResponse', (_message.Message,), {
-    'DESCRIPTOR': _LISTVOIPCALLINFORESPONSE,
-    '__module__': 'ondewo.vtsi.voip_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ListVoipCallInfoResponse)
+ListCallInfoResponse = _reflection.GeneratedProtocolMessageType('ListCallInfoResponse', (_message.Message,), {
+    'DESCRIPTOR': _LISTCALLINFORESPONSE,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ListCallInfoResponse)
 })
-_sym_db.RegisterMessage(ListVoipCallInfoResponse)
+_sym_db.RegisterMessage(ListCallInfoResponse)
 
 AllServicesStatuses = _reflection.GeneratedProtocolMessageType('AllServicesStatuses', (_message.Message,), {
     'DESCRIPTOR': _ALLSERVICESSTATUSES,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.AllServicesStatuses)
 })
 _sym_db.RegisterMessage(AllServicesStatuses)
 
 ServiceStatus = _reflection.GeneratedProtocolMessageType('ServiceStatus', (_message.Message,), {
     'DESCRIPTOR': _SERVICESTATUS,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.ServiceStatus)
 })
 _sym_db.RegisterMessage(ServiceStatus)
 
 GetAudioFileRequest = _reflection.GeneratedProtocolMessageType('GetAudioFileRequest', (_message.Message,), {
     'DESCRIPTOR': _GETAUDIOFILEREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetAudioFileRequest)
 })
 _sym_db.RegisterMessage(GetAudioFileRequest)
 
 GetAudioFileResponse = _reflection.GeneratedProtocolMessageType('GetAudioFileResponse', (_message.Message,), {
     'DESCRIPTOR': _GETAUDIOFILERESPONSE,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetAudioFileResponse)
 })
 _sym_db.RegisterMessage(GetAudioFileResponse)
 
 GetFullConversationAudioFileRequest = _reflection.GeneratedProtocolMessageType('GetFullConversationAudioFileRequest', (_message.Message,), {
     'DESCRIPTOR': _GETFULLCONVERSATIONAUDIOFILEREQUEST,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetFullConversationAudioFileRequest)
 })
 _sym_db.RegisterMessage(GetFullConversationAudioFileRequest)
 
 GetFullConversationAudioFileResponse = _reflection.GeneratedProtocolMessageType('GetFullConversationAudioFileResponse', (_message.Message,), {
     'DESCRIPTOR': _GETFULLCONVERSATIONAUDIOFILERESPONSE,
-    '__module__': 'ondewo.vtsi.voip_pb2'
+    '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetFullConversationAudioFileResponse)
 })
 _sym_db.RegisterMessage(GetFullConversationAudioFileResponse)
 
-_VOIPSESSIONS = DESCRIPTOR.services_by_name['VoipSessions']
+_CALLS = DESCRIPTOR.services_by_name['Calls']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _SIPCALLERCONFIG_HEADERSENTRY._options = None
-    _SIPCALLERCONFIG_HEADERSENTRY._serialized_options = b'8\001'
-    _VOIPCALLINFOVIEW._serialized_start = 6788
-    _VOIPCALLINFOVIEW._serialized_end = 6849
-    _CALLTYPE._serialized_start = 6851
-    _CALLTYPE._serialized_end = 6897
-    _PROJECTCONFIGS._serialized_start = 275
-    _PROJECTCONFIGS._serialized_end = 391
-    _ASTERISKCONFIGSVARIABLES._serialized_start = 394
-    _ASTERISKCONFIGSVARIABLES._serialized_end = 587
-    _ASTERISKCONFIGSFILES._serialized_start = 590
-    _ASTERISKCONFIGSFILES._serialized_end = 746
-    _ASTERISKCONFIGS._serialized_start = 749
-    _ASTERISKCONFIGS._serialized_end = 1011
-    _CREATEPROJECTCONFIGSREQUEST._serialized_start = 1013
-    _CREATEPROJECTCONFIGSREQUEST._serialized_end = 1116
-    _GETPROJECTCONFIGSREQUEST._serialized_start = 1118
-    _GETPROJECTCONFIGSREQUEST._serialized_end = 1164
-    _GETPROJECTCONFIGSRESPONSE._serialized_start = 1167
-    _GETPROJECTCONFIGSRESPONSE._serialized_end = 1328
-    _UPDATEPROJECTCONFIGSREQUEST._serialized_start = 1330
-    _UPDATEPROJECTCONFIGSREQUEST._serialized_end = 1433
-    _DELETEPROJECTCONFIGSREQUEST._serialized_start = 1435
-    _DELETEPROJECTCONFIGSREQUEST._serialized_end = 1484
-    _DEPLOYPROJECTREQUEST._serialized_start = 1486
-    _DEPLOYPROJECTREQUEST._serialized_end = 1528
-    _UNDEPLOYPROJECTREQUEST._serialized_start = 1530
-    _UNDEPLOYPROJECTREQUEST._serialized_end = 1574
-    _BASESERVICECONFIG._serialized_start = 1576
-    _BASESERVICECONFIG._serialized_end = 1642
-    _CREDENTIALS._serialized_start = 1644
-    _CREDENTIALS._serialized_end = 1697
-    _NLUCONFIG._serialized_start = 1700
-    _NLUCONFIG._serialized_end = 1939
-    _T2SCONFIG._serialized_start = 1941
-    _T2SCONFIG._serialized_end = 2052
-    _S2TCONFIG._serialized_start = 2054
-    _S2TCONFIG._serialized_end = 2175
-    _ASTERISKCONFIG._serialized_start = 2177
-    _ASTERISKCONFIG._serialized_end = 2246
-    _COMMONSERVICESCONFIGS._serialized_start = 2249
-    _COMMONSERVICESCONFIGS._serialized_end = 2502
-    _SIPBASECONFIG._serialized_start = 2504
-    _SIPBASECONFIG._serialized_end = 2544
-    _SIPCALLERCONFIG._serialized_start = 2547
-    _SIPCALLERCONFIG._serialized_end = 2747
-    _SIPCALLERCONFIG_HEADERSENTRY._serialized_start = 2701
-    _SIPCALLERCONFIG_HEADERSENTRY._serialized_end = 2747
-    _CSICONFIG._serialized_start = 2750
-    _CSICONFIG._serialized_end = 3085
-    _AUDIOOBJECTSTORAGECONFIG._serialized_start = 3088
-    _AUDIOOBJECTSTORAGECONFIG._serialized_end = 3341
-    _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG._serialized_start = 3343
-    _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG._serialized_end = 3431
-    _MESSAGEBROKERCONFIG._serialized_start = 3434
-    _MESSAGEBROKERCONFIG._serialized_end = 3673
-    _MESSAGEBROKERSERVICESACTIVATIONCONFIG._serialized_start = 3675
-    _MESSAGEBROKERSERVICESACTIVATIONCONFIG._serialized_end = 3802
-    _RABBITMQCONFIG._serialized_start = 3804
-    _RABBITMQCONFIG._serialized_end = 3896
-    _ENDPOINT._serialized_start = 3898
-    _ENDPOINT._serialized_end = 3936
-    _MINIOCONFIG._serialized_start = 3939
-    _MINIOCONFIG._serialized_end = 4072
-    _S2TCALLBACKS._serialized_start = 4074
-    _S2TCALLBACKS._serialized_end = 4143
-    _NLUCALLBACKS._serialized_start = 4145
-    _NLUCALLBACKS._serialized_end = 4214
-    _T2SCALLBACKS._serialized_start = 4216
-    _T2SCALLBACKS._serialized_end = 4285
-    _STARTLISTENERREQUEST._serialized_start = 4288
-    _STARTLISTENERREQUEST._serialized_end = 4420
-    _STARTCALLERREQUEST._serialized_start = 4423
-    _STARTCALLERREQUEST._serialized_end = 4555
-    _STARTSCHEDULEDCALLERREQUEST._serialized_start = 4558
-    _STARTSCHEDULEDCALLERREQUEST._serialized_end = 4689
-    _STARTLISTENERSREQUEST._serialized_start = 4691
-    _STARTLISTENERSREQUEST._serialized_end = 4787
-    _STARTLISTENERSRESPONSE._serialized_start = 4789
-    _STARTLISTENERSRESPONSE._serialized_end = 4851
-    _STARTCALLERSREQUEST._serialized_start = 4853
-    _STARTCALLERSREQUEST._serialized_end = 4945
-    _STARTCALLERSRESPONSE._serialized_start = 4947
-    _STARTCALLERSRESPONSE._serialized_end = 5007
-    _STARTSCHEDULEDCALLERSREQUEST._serialized_start = 5009
-    _STARTSCHEDULEDCALLERSREQUEST._serialized_end = 5119
-    _STOPCALLSREQUEST._serialized_start = 5121
-    _STOPCALLSREQUEST._serialized_end = 5177
-    _STOPALLCALLSREQUEST._serialized_start = 5179
-    _STOPALLCALLSREQUEST._serialized_end = 5220
-    _TRANSFERCALLSREQUEST._serialized_start = 5222
-    _TRANSFERCALLSREQUEST._serialized_end = 5302
-    _GETVOIPCALLINFOREQUEST._serialized_start = 5304
-    _GETVOIPCALLINFOREQUEST._serialized_end = 5425
-    _GETVOIPCALLINFORESPONSE._serialized_start = 5427
-    _GETVOIPCALLINFORESPONSE._serialized_end = 5545
-    _VOIPCALLINFO._serialized_start = 5548
-    _VOIPCALLINFO._serialized_end = 5896
-    _LISTVOIPCALLINFOREQUEST._serialized_start = 5899
-    _LISTVOIPCALLINFOREQUEST._serialized_end = 6046
-    _LISTVOIPCALLINFORESPONSE._serialized_start = 6048
-    _LISTVOIPCALLINFORESPONSE._serialized_end = 6120
-    _ALLSERVICESSTATUSES._serialized_start = 6123
-    _ALLSERVICESSTATUSES._serialized_end = 6389
-    _SERVICESTATUS._serialized_start = 6391
-    _SERVICESTATUS._serialized_end = 6448
-    _GETAUDIOFILEREQUEST._serialized_start = 6450
-    _GETAUDIOFILEREQUEST._serialized_end = 6561
-    _GETAUDIOFILERESPONSE._serialized_start = 6563
-    _GETAUDIOFILERESPONSE._serialized_end = 6600
-    _GETFULLCONVERSATIONAUDIOFILEREQUEST._serialized_start = 6603
-    _GETFULLCONVERSATIONAUDIOFILEREQUEST._serialized_end = 6731
-    _GETFULLCONVERSATIONAUDIOFILERESPONSE._serialized_start = 6733
-    _GETFULLCONVERSATIONAUDIOFILERESPONSE._serialized_end = 6786
-    _VOIPSESSIONS._serialized_start = 6900
-    _VOIPSESSIONS._serialized_end = 8340
+    _SIPCALLERCONFIG_SIPHEADERSENTRY._options = None
+    _SIPCALLERCONFIG_SIPHEADERSENTRY._serialized_options = b'8\001'
+    _CALLINFOVIEW._serialized_start = 7594
+    _CALLINFOVIEW._serialized_end = 7631
+    _CALLTYPE._serialized_start = 7633
+    _CALLTYPE._serialized_end = 7679
+    _BASESERVICECONFIG._serialized_start = 246
+    _BASESERVICECONFIG._serialized_end = 312
+    _CREDENTIALS._serialized_start = 314
+    _CREDENTIALS._serialized_end = 367
+    _NLUVTSICONFIG._serialized_start = 370
+    _NLUVTSICONFIG._serialized_end = 668
+    _T2SVTSICONFIG._serialized_start = 670
+    _T2SVTSICONFIG._serialized_end = 797
+    _S2TVTSICONFIG._serialized_start = 800
+    _S2TVTSICONFIG._serialized_end = 948
+    _ASTERISKCONFIG._serialized_start = 950
+    _ASTERISKCONFIG._serialized_end = 1028
+    _COMMONSERVICESCONFIG._serialized_start = 1031
+    _COMMONSERVICESCONFIG._serialized_end = 1265
+    _SIPBASECONFIG._serialized_start = 1267
+    _SIPBASECONFIG._serialized_end = 1307
+    _SIPCALLERCONFIG._serialized_start = 1310
+    _SIPCALLERCONFIG._serialized_end = 1517
+    _SIPCALLERCONFIG_SIPHEADERSENTRY._serialized_start = 1468
+    _SIPCALLERCONFIG_SIPHEADERSENTRY._serialized_end = 1517
+    _CSIVTSICONFIG._serialized_start = 1520
+    _CSIVTSICONFIG._serialized_end = 1886
+    _AUDIOOBJECTSTORAGECONFIG._serialized_start = 1889
+    _AUDIOOBJECTSTORAGECONFIG._serialized_end = 2142
+    _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG._serialized_start = 2144
+    _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG._serialized_end = 2232
+    _MESSAGEBROKERCONFIG._serialized_start = 2235
+    _MESSAGEBROKERCONFIG._serialized_end = 2474
+    _MESSAGEBROKERSERVICESACTIVATIONCONFIG._serialized_start = 2476
+    _MESSAGEBROKERSERVICESACTIVATIONCONFIG._serialized_end = 2603
+    _RABBITMQCONFIG._serialized_start = 2605
+    _RABBITMQCONFIG._serialized_end = 2697
+    _MINIOCONFIG._serialized_start = 2699
+    _MINIOCONFIG._serialized_end = 2819
+    _S2TVTSICALLBACKS._serialized_start = 2821
+    _S2TVTSICALLBACKS._serialized_end = 2894
+    _NLUVTSICALLBACKS._serialized_start = 2896
+    _NLUVTSICALLBACKS._serialized_end = 2969
+    _T2SVTSICALLBACKS._serialized_start = 2971
+    _T2SVTSICALLBACKS._serialized_end = 3044
+    _LISTENER._serialized_start = 3047
+    _LISTENER._serialized_end = 3210
+    _CALLER._serialized_start = 3213
+    _CALLER._serialized_end = 3378
+    _STARTLISTENERREQUEST._serialized_start = 3381
+    _STARTLISTENERREQUEST._serialized_end = 3550
+    _STARTLISTENERRESPONSE._serialized_start = 3552
+    _STARTLISTENERRESPONSE._serialized_end = 3666
+    _STARTLISTENERSREQUEST._serialized_start = 3668
+    _STARTLISTENERSREQUEST._serialized_end = 3780
+    _STARTLISTENERSRESPONSE._serialized_start = 3783
+    _STARTLISTENERSRESPONSE._serialized_end = 3921
+    _STARTCALLERREQUEST._serialized_start = 3924
+    _STARTCALLERREQUEST._serialized_end = 4095
+    _STARTCALLERRESPONSE._serialized_start = 4097
+    _STARTCALLERRESPONSE._serialized_end = 4205
+    _STARTCALLERSREQUEST._serialized_start = 4207
+    _STARTCALLERSREQUEST._serialized_end = 4313
+    _STARTCALLERSRESPONSE._serialized_start = 4316
+    _STARTCALLERSRESPONSE._serialized_end = 4448
+    _STARTSCHEDULEDCALLERREQUEST._serialized_start = 4451
+    _STARTSCHEDULEDCALLERREQUEST._serialized_end = 4609
+    _STARTSCHEDULEDCALLERSREQUEST._serialized_start = 4612
+    _STARTSCHEDULEDCALLERSREQUEST._serialized_end = 4746
+    _STARTSCHEDULEDCALLERSRESPONSE._serialized_start = 4749
+    _STARTSCHEDULEDCALLERSRESPONSE._serialized_end = 4886
+    _STARTSCHEDULEDCALLERRESPONSE._serialized_start = 4889
+    _STARTSCHEDULEDCALLERRESPONSE._serialized_end = 5025
+    _SCHEDULEDCALLER._serialized_start = 5028
+    _SCHEDULEDCALLER._serialized_end = 5245
+    _STOPCALLREQUEST._serialized_start = 5247
+    _STOPCALLREQUEST._serialized_end = 5310
+    _STOPCALLRESPONSE._serialized_start = 5312
+    _STOPCALLRESPONSE._serialized_end = 5399
+    _STOPCALLSREQUEST._serialized_start = 5401
+    _STOPCALLSREQUEST._serialized_end = 5466
+    _STOPCALLSRESPONSE._serialized_start = 5468
+    _STOPCALLSRESPONSE._serialized_end = 5570
+    _STOPALLCALLSREQUEST._serialized_start = 5572
+    _STOPALLCALLSREQUEST._serialized_end = 5620
+    _TRANSFERCALLREQUEST._serialized_start = 5622
+    _TRANSFERCALLREQUEST._serialized_end = 5710
+    _TRANSFERCALLRESPONSE._serialized_start = 5712
+    _TRANSFERCALLRESPONSE._serialized_end = 5824
+    _TRANSFERCALLSREQUEST._serialized_start = 5826
+    _TRANSFERCALLSREQUEST._serialized_end = 5941
+    _TRANSFERCALLSRESPONSE._serialized_start = 5944
+    _TRANSFERCALLSRESPONSE._serialized_end = 6085
+    _GETCALLINFOREQUEST._serialized_start = 6087
+    _GETCALLINFOREQUEST._serialized_end = 6204
+    _GETCALLINFORESPONSE._serialized_start = 6206
+    _GETCALLINFORESPONSE._serialized_end = 6312
+    _CALLINFO._serialized_start = 6315
+    _CALLINFO._serialized_end = 6717
+    _LISTCALLINFOREQUEST._serialized_start = 6720
+    _LISTCALLINFOREQUEST._serialized_end = 6861
+    _LISTCALLINFORESPONSE._serialized_start = 6863
+    _LISTCALLINFORESPONSE._serialized_end = 6928
+    _ALLSERVICESSTATUSES._serialized_start = 6931
+    _ALLSERVICESSTATUSES._serialized_end = 7197
+    _SERVICESTATUS._serialized_start = 7199
+    _SERVICESTATUS._serialized_end = 7254
+    _GETAUDIOFILEREQUEST._serialized_start = 7256
+    _GETAUDIOFILEREQUEST._serialized_end = 7367
+    _GETAUDIOFILERESPONSE._serialized_start = 7369
+    _GETAUDIOFILERESPONSE._serialized_end = 7406
+    _GETFULLCONVERSATIONAUDIOFILEREQUEST._serialized_start = 7409
+    _GETFULLCONVERSATIONAUDIOFILEREQUEST._serialized_end = 7537
+    _GETFULLCONVERSATIONAUDIOFILERESPONSE._serialized_start = 7539
+    _GETFULLCONVERSATIONAUDIOFILERESPONSE._serialized_end = 7592
+    _CALLS._serialized_start = 7682
+    _CALLS._serialized_end = 9048
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo/vtsi/voip_pb2_grpc.py` & `ondewo-vtsi-client-6.0.0/ondewo/vtsi/calls_pb2_grpc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,613 +1,553 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from ondewo.vtsi import voip_pb2 as ondewo_dot_vtsi_dot_voip__pb2
+from ondewo.vtsi import calls_pb2 as ondewo_dot_vtsi_dot_calls__pb2
 
 
-class VoipSessionsStub(object):
-    """session manager for phone calls.
-    endpoints of voip server that manages instances of ondewo-sip, which handle individual calls
-    /////////
-    Projects //
-    /////////
+class CallsStub(object):
+    """ONDEWO VTSI API
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.CreateProjectConfigs = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/CreateProjectConfigs',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.CreateProjectConfigsRequest.SerializeToString,
-            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-        )
-        self.GetProjectConfigs = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/GetProjectConfigs',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.GetProjectConfigsRequest.SerializeToString,
-            response_deserializer=ondewo_dot_vtsi_dot_voip__pb2.GetProjectConfigsResponse.FromString,
-        )
-        self.UpdateProjectConfigs = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/UpdateProjectConfigs',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.UpdateProjectConfigsRequest.SerializeToString,
-            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-        )
-        self.DeleteProjectConfigs = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/DeleteProjectConfigs',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.DeleteProjectConfigsRequest.SerializeToString,
-            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-        )
-        self.DeployProject = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/DeployProject',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.DeployProjectRequest.SerializeToString,
-            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-        )
-        self.UndeployProject = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/UndeployProject',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.UndeployProjectRequest.SerializeToString,
-            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-        )
-        self.StartListeners = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/StartListeners',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.StartListenersRequest.SerializeToString,
-            response_deserializer=ondewo_dot_vtsi_dot_voip__pb2.StartListenersResponse.FromString,
+        self.StartCaller = channel.unary_unary(
+            '/ondewo.vtsi.Calls/StartCaller',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallerRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallerResponse.FromString,
         )
         self.StartCallers = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/StartCallers',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.StartCallersRequest.SerializeToString,
-            response_deserializer=ondewo_dot_vtsi_dot_voip__pb2.StartCallersResponse.FromString,
+            '/ondewo.vtsi.Calls/StartCallers',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallersRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallersResponse.FromString,
+        )
+        self.StartListener = channel.unary_unary(
+            '/ondewo.vtsi.Calls/StartListener',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenerRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenerResponse.FromString,
+        )
+        self.StartListeners = channel.unary_unary(
+            '/ondewo.vtsi.Calls/StartListeners',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenersRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenersResponse.FromString,
+        )
+        self.StartScheduledCaller = channel.unary_unary(
+            '/ondewo.vtsi.Calls/StartScheduledCaller',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallerRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallerResponse.FromString,
         )
         self.StartScheduledCallers = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/StartScheduledCallers',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.StartScheduledCallersRequest.SerializeToString,
-            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            '/ondewo.vtsi.Calls/StartScheduledCallers',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallersRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallersResponse.FromString,
+        )
+        self.StopCall = channel.unary_unary(
+            '/ondewo.vtsi.Calls/StopCall',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.StopCallRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StopCallResponse.FromString,
         )
         self.StopCalls = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/StopCalls',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.StopCallsRequest.SerializeToString,
-            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            '/ondewo.vtsi.Calls/StopCalls',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.StopCallsRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StopCallsResponse.FromString,
         )
         self.StopAllCalls = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/StopAllCalls',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.StopAllCallsRequest.SerializeToString,
-            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            '/ondewo.vtsi.Calls/StopAllCalls',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.StopAllCallsRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StopCallsResponse.FromString,
+        )
+        self.TransferCall = channel.unary_unary(
+            '/ondewo.vtsi.Calls/TransferCall',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallResponse.FromString,
         )
         self.TransferCalls = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/TransferCalls',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.TransferCallsRequest.SerializeToString,
-            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-        )
-        self.GetVoipCallInfo = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/GetVoipCallInfo',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.GetVoipCallInfoRequest.SerializeToString,
-            response_deserializer=ondewo_dot_vtsi_dot_voip__pb2.GetVoipCallInfoResponse.FromString,
-        )
-        self.ListVoipCallInfo = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/ListVoipCallInfo',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.ListVoipCallInfoRequest.SerializeToString,
-            response_deserializer=ondewo_dot_vtsi_dot_voip__pb2.ListVoipCallInfoResponse.FromString,
+            '/ondewo.vtsi.Calls/TransferCalls',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallsRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallsResponse.FromString,
+        )
+        self.GetCallInfo = channel.unary_unary(
+            '/ondewo.vtsi.Calls/GetCallInfo',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.GetCallInfoRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.GetCallInfoResponse.FromString,
+        )
+        self.ListCallInfo = channel.unary_unary(
+            '/ondewo.vtsi.Calls/ListCallInfo',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallInfoRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallInfoResponse.FromString,
         )
         self.GetAudioFile = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/GetAudioFile',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.GetAudioFileRequest.SerializeToString,
-            response_deserializer=ondewo_dot_vtsi_dot_voip__pb2.GetAudioFileResponse.FromString,
+            '/ondewo.vtsi.Calls/GetAudioFile',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.GetAudioFileRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.GetAudioFileResponse.FromString,
         )
         self.GetFullConversationAudioFile = channel.unary_unary(
-            '/ondewo.vtsi.VoipSessions/GetFullConversationAudioFile',
-            request_serializer=ondewo_dot_vtsi_dot_voip__pb2.GetFullConversationAudioFileRequest.SerializeToString,
-            response_deserializer=ondewo_dot_vtsi_dot_voip__pb2.GetFullConversationAudioFileResponse.FromString,
+            '/ondewo.vtsi.Calls/GetFullConversationAudioFile',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.GetFullConversationAudioFileRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.GetFullConversationAudioFileResponse.FromString,
         )
 
 
-class VoipSessionsServicer(object):
-    """session manager for phone calls.
-    endpoints of voip server that manages instances of ondewo-sip, which handle individual calls
-    /////////
-    Projects //
-    /////////
+class CallsServicer(object):
+    """ONDEWO VTSI API
     """
 
-    def CreateProjectConfigs(self, request, context):
-        """Create an NLU project with configs.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
+    def StartCaller(self, request, context):
+        """////////////////////////////////////////////////////////////////////////////
+        Caller and Listener endpoints
+        ////////////////////////////////////////////////////////////////////////////
 
-    def GetProjectConfigs(self, request, context):
-        """Get an NLU project with configs.
+        start single caller instance for a specific nlu-project.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def UpdateProjectConfigs(self, request, context):
-        """Update an NLU project with configs.
+    def StartCallers(self, request, context):
+        """start multiple ondewo-sip callers instances for a specific nlu-project.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeleteProjectConfigs(self, request, context):
-        """Delete an NLU project with configs.
+    def StartListener(self, request, context):
+        """start single listener instance for a specific nlu-project.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeployProject(self, request, context):
-        """/////////
-        Asterisk //
-        /////////
-
+    def StartListeners(self, request, context):
+        """start multiple ondewo-sip listeners instances for a specific nlu-project.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def UndeployProject(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def StartListeners(self, request, context):
-        """/////////
-        CALLS //
-        /////////
-
-        start multiple ondewo-sip listeners instances for a specific nlu-project.
+    def StartScheduledCaller(self, request, context):
+        """start multiple ondewo-sip callers instances with schedules
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def StartCallers(self, request, context):
-        """start multiple ondewo-sip callers instances for a specific nlu-project.
+    def StartScheduledCallers(self, request, context):
+        """start multiple ondewo-sip callers instances with schedules
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def StartScheduledCallers(self, request, context):
-        """start multiple ondewo-sip callers instances with schedules
+    def StopCall(self, request, context):
+        """stop/kill a ondewo-sip listener or caller instance for a specific vtsi-project.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def StopCalls(self, request, context):
-        """stop/kill a list of ondewo-sip listener or caller instances for a specific nlu-project.
+        """stop/kill a list of ondewo-sip listener or caller instances for a specific vtsi-project.
         "stops both Listener and Caller calls"
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def StopAllCalls(self, request, context):
         """stop/kill all ondewo-sip listener or caller instance for a specific nlu-project.
         "stops all Listener and Caller calls"
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def TransferCalls(self, request, context):
-        """Transfer a call from a listener to another number for a specific nlu-project.
+    def TransferCall(self, request, context):
+        """Transfer a call from a listener to another
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetVoipCallInfo(self, request, context):
-        """ConferenceCall .. to be added in the future
-        rpc ConferenceCall (ConferenceCallRequest) returns (google.protobuf.Empty);
-
-        //////////
-        STATUS //
-        //////////
+    def TransferCalls(self, request, context):
+        """Transfer a call from a listener to another
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
-        get call log for single call instance
+    def GetCallInfo(self, request, context):
+        """get call log for single call instance
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListVoipCallInfo(self, request, context):
+    def ListCallInfo(self, request, context):
         """get call log for all call instances
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetAudioFile(self, request, context):
-        """///////////////////////
-        Retrieving Audio files //
-        //////////////////////////
-
-        Get a s2t or t2s audio file for this conversation if it exists in Minio
+        """Get a s2t or t2s audio file for this conversation if it exists in Minio
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetFullConversationAudioFile(self, request, context):
         """Get The whole conversation in an audio file
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_VoipSessionsServicer_to_server(servicer, server):
+def add_CallsServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        'CreateProjectConfigs': grpc.unary_unary_rpc_method_handler(
-            servicer.CreateProjectConfigs,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.CreateProjectConfigsRequest.FromString,
-            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-        ),
-        'GetProjectConfigs': grpc.unary_unary_rpc_method_handler(
-            servicer.GetProjectConfigs,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.GetProjectConfigsRequest.FromString,
-            response_serializer=ondewo_dot_vtsi_dot_voip__pb2.GetProjectConfigsResponse.SerializeToString,
-        ),
-        'UpdateProjectConfigs': grpc.unary_unary_rpc_method_handler(
-            servicer.UpdateProjectConfigs,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.UpdateProjectConfigsRequest.FromString,
-            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-        ),
-        'DeleteProjectConfigs': grpc.unary_unary_rpc_method_handler(
-            servicer.DeleteProjectConfigs,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.DeleteProjectConfigsRequest.FromString,
-            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-        ),
-        'DeployProject': grpc.unary_unary_rpc_method_handler(
-            servicer.DeployProject,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.DeployProjectRequest.FromString,
-            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
-        ),
-        'UndeployProject': grpc.unary_unary_rpc_method_handler(
-            servicer.UndeployProject,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.UndeployProjectRequest.FromString,
-            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+        'StartCaller': grpc.unary_unary_rpc_method_handler(
+            servicer.StartCaller,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallerRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallerResponse.SerializeToString,
+        ),
+        'StartCallers': grpc.unary_unary_rpc_method_handler(
+            servicer.StartCallers,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallersRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallersResponse.SerializeToString,
+        ),
+        'StartListener': grpc.unary_unary_rpc_method_handler(
+            servicer.StartListener,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenerRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenerResponse.SerializeToString,
         ),
         'StartListeners': grpc.unary_unary_rpc_method_handler(
             servicer.StartListeners,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.StartListenersRequest.FromString,
-            response_serializer=ondewo_dot_vtsi_dot_voip__pb2.StartListenersResponse.SerializeToString,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenersRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenersResponse.SerializeToString,
         ),
-        'StartCallers': grpc.unary_unary_rpc_method_handler(
-            servicer.StartCallers,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.StartCallersRequest.FromString,
-            response_serializer=ondewo_dot_vtsi_dot_voip__pb2.StartCallersResponse.SerializeToString,
+        'StartScheduledCaller': grpc.unary_unary_rpc_method_handler(
+            servicer.StartScheduledCaller,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallerRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallerResponse.SerializeToString,
         ),
         'StartScheduledCallers': grpc.unary_unary_rpc_method_handler(
             servicer.StartScheduledCallers,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.StartScheduledCallersRequest.FromString,
-            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallersRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallersResponse.SerializeToString,
+        ),
+        'StopCall': grpc.unary_unary_rpc_method_handler(
+            servicer.StopCall,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StopCallRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StopCallResponse.SerializeToString,
         ),
         'StopCalls': grpc.unary_unary_rpc_method_handler(
             servicer.StopCalls,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.StopCallsRequest.FromString,
-            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StopCallsRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StopCallsResponse.SerializeToString,
         ),
         'StopAllCalls': grpc.unary_unary_rpc_method_handler(
             servicer.StopAllCalls,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.StopAllCallsRequest.FromString,
-            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StopAllCallsRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StopCallsResponse.SerializeToString,
+        ),
+        'TransferCall': grpc.unary_unary_rpc_method_handler(
+            servicer.TransferCall,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallResponse.SerializeToString,
         ),
         'TransferCalls': grpc.unary_unary_rpc_method_handler(
             servicer.TransferCalls,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.TransferCallsRequest.FromString,
-            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallsRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallsResponse.SerializeToString,
         ),
-        'GetVoipCallInfo': grpc.unary_unary_rpc_method_handler(
-            servicer.GetVoipCallInfo,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.GetVoipCallInfoRequest.FromString,
-            response_serializer=ondewo_dot_vtsi_dot_voip__pb2.GetVoipCallInfoResponse.SerializeToString,
-        ),
-        'ListVoipCallInfo': grpc.unary_unary_rpc_method_handler(
-            servicer.ListVoipCallInfo,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.ListVoipCallInfoRequest.FromString,
-            response_serializer=ondewo_dot_vtsi_dot_voip__pb2.ListVoipCallInfoResponse.SerializeToString,
+        'GetCallInfo': grpc.unary_unary_rpc_method_handler(
+            servicer.GetCallInfo,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.GetCallInfoRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.GetCallInfoResponse.SerializeToString,
+        ),
+        'ListCallInfo': grpc.unary_unary_rpc_method_handler(
+            servicer.ListCallInfo,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallInfoRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallInfoResponse.SerializeToString,
         ),
         'GetAudioFile': grpc.unary_unary_rpc_method_handler(
             servicer.GetAudioFile,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.GetAudioFileRequest.FromString,
-            response_serializer=ondewo_dot_vtsi_dot_voip__pb2.GetAudioFileResponse.SerializeToString,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.GetAudioFileRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.GetAudioFileResponse.SerializeToString,
         ),
         'GetFullConversationAudioFile': grpc.unary_unary_rpc_method_handler(
             servicer.GetFullConversationAudioFile,
-            request_deserializer=ondewo_dot_vtsi_dot_voip__pb2.GetFullConversationAudioFileRequest.FromString,
-            response_serializer=ondewo_dot_vtsi_dot_voip__pb2.GetFullConversationAudioFileResponse.SerializeToString,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.GetFullConversationAudioFileRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.GetFullConversationAudioFileResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        'ondewo.vtsi.VoipSessions', rpc_method_handlers)
+        'ondewo.vtsi.Calls', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
  # This class is part of an EXPERIMENTAL API.
 
 
-class VoipSessions(object):
-    """session manager for phone calls.
-    endpoints of voip server that manages instances of ondewo-sip, which handle individual calls
-    /////////
-    Projects //
-    /////////
+class Calls(object):
+    """ONDEWO VTSI API
     """
 
     @staticmethod
-    def CreateProjectConfigs(request,
-                             target,
-                             options=(),
-                             channel_credentials=None,
-                             call_credentials=None,
-                             insecure=False,
-                             compression=None,
-                             wait_for_ready=None,
-                             timeout=None,
-                             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/CreateProjectConfigs',
-                                             ondewo_dot_vtsi_dot_voip__pb2.CreateProjectConfigsRequest.SerializeToString,
-                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def GetProjectConfigs(request,
-                          target,
-                          options=(),
-                          channel_credentials=None,
-                          call_credentials=None,
-                          insecure=False,
-                          compression=None,
-                          wait_for_ready=None,
-                          timeout=None,
-                          metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/GetProjectConfigs',
-                                             ondewo_dot_vtsi_dot_voip__pb2.GetProjectConfigsRequest.SerializeToString,
-                                             ondewo_dot_vtsi_dot_voip__pb2.GetProjectConfigsResponse.FromString,
+    def StartCaller(request,
+                    target,
+                    options=(),
+                    channel_credentials=None,
+                    call_credentials=None,
+                    insecure=False,
+                    compression=None,
+                    wait_for_ready=None,
+                    timeout=None,
+                    metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/StartCaller',
+                                             ondewo_dot_vtsi_dot_calls__pb2.StartCallerRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.StartCallerResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def UpdateProjectConfigs(request,
-                             target,
-                             options=(),
-                             channel_credentials=None,
-                             call_credentials=None,
-                             insecure=False,
-                             compression=None,
-                             wait_for_ready=None,
-                             timeout=None,
-                             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/UpdateProjectConfigs',
-                                             ondewo_dot_vtsi_dot_voip__pb2.UpdateProjectConfigsRequest.SerializeToString,
-                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def DeleteProjectConfigs(request,
-                             target,
-                             options=(),
-                             channel_credentials=None,
-                             call_credentials=None,
-                             insecure=False,
-                             compression=None,
-                             wait_for_ready=None,
-                             timeout=None,
-                             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/DeleteProjectConfigs',
-                                             ondewo_dot_vtsi_dot_voip__pb2.DeleteProjectConfigsRequest.SerializeToString,
-                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+    def StartCallers(request,
+                     target,
+                     options=(),
+                     channel_credentials=None,
+                     call_credentials=None,
+                     insecure=False,
+                     compression=None,
+                     wait_for_ready=None,
+                     timeout=None,
+                     metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/StartCallers',
+                                             ondewo_dot_vtsi_dot_calls__pb2.StartCallersRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.StartCallersResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def DeployProject(request,
+    def StartListener(request,
                       target,
                       options=(),
                       channel_credentials=None,
                       call_credentials=None,
                       insecure=False,
                       compression=None,
                       wait_for_ready=None,
                       timeout=None,
                       metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/DeployProject',
-                                             ondewo_dot_vtsi_dot_voip__pb2.DeployProjectRequest.SerializeToString,
-                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def UndeployProject(request,
-                        target,
-                        options=(),
-                        channel_credentials=None,
-                        call_credentials=None,
-                        insecure=False,
-                        compression=None,
-                        wait_for_ready=None,
-                        timeout=None,
-                        metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/UndeployProject',
-                                             ondewo_dot_vtsi_dot_voip__pb2.UndeployProjectRequest.SerializeToString,
-                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/StartListener',
+                                             ondewo_dot_vtsi_dot_calls__pb2.StartListenerRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.StartListenerResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def StartListeners(request,
                        target,
                        options=(),
                        channel_credentials=None,
                        call_credentials=None,
                        insecure=False,
                        compression=None,
                        wait_for_ready=None,
                        timeout=None,
                        metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/StartListeners',
-                                             ondewo_dot_vtsi_dot_voip__pb2.StartListenersRequest.SerializeToString,
-                                             ondewo_dot_vtsi_dot_voip__pb2.StartListenersResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/StartListeners',
+                                             ondewo_dot_vtsi_dot_calls__pb2.StartListenersRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.StartListenersResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def StartCallers(request,
-                     target,
-                     options=(),
-                     channel_credentials=None,
-                     call_credentials=None,
-                     insecure=False,
-                     compression=None,
-                     wait_for_ready=None,
-                     timeout=None,
-                     metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/StartCallers',
-                                             ondewo_dot_vtsi_dot_voip__pb2.StartCallersRequest.SerializeToString,
-                                             ondewo_dot_vtsi_dot_voip__pb2.StartCallersResponse.FromString,
+    def StartScheduledCaller(request,
+                             target,
+                             options=(),
+                             channel_credentials=None,
+                             call_credentials=None,
+                             insecure=False,
+                             compression=None,
+                             wait_for_ready=None,
+                             timeout=None,
+                             metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/StartScheduledCaller',
+                                             ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallerRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallerResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def StartScheduledCallers(request,
                               target,
                               options=(),
                               channel_credentials=None,
                               call_credentials=None,
                               insecure=False,
                               compression=None,
                               wait_for_ready=None,
                               timeout=None,
                               metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/StartScheduledCallers',
-                                             ondewo_dot_vtsi_dot_voip__pb2.StartScheduledCallersRequest.SerializeToString,
-                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/StartScheduledCallers',
+                                             ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallersRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallersResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def StopCall(request,
+                 target,
+                 options=(),
+                 channel_credentials=None,
+                 call_credentials=None,
+                 insecure=False,
+                 compression=None,
+                 wait_for_ready=None,
+                 timeout=None,
+                 metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/StopCall',
+                                             ondewo_dot_vtsi_dot_calls__pb2.StopCallRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.StopCallResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def StopCalls(request,
                   target,
                   options=(),
                   channel_credentials=None,
                   call_credentials=None,
                   insecure=False,
                   compression=None,
                   wait_for_ready=None,
                   timeout=None,
                   metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/StopCalls',
-                                             ondewo_dot_vtsi_dot_voip__pb2.StopCallsRequest.SerializeToString,
-                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/StopCalls',
+                                             ondewo_dot_vtsi_dot_calls__pb2.StopCallsRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.StopCallsResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def StopAllCalls(request,
                      target,
                      options=(),
                      channel_credentials=None,
                      call_credentials=None,
                      insecure=False,
                      compression=None,
                      wait_for_ready=None,
                      timeout=None,
                      metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/StopAllCalls',
-                                             ondewo_dot_vtsi_dot_voip__pb2.StopAllCallsRequest.SerializeToString,
-                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/StopAllCalls',
+                                             ondewo_dot_vtsi_dot_calls__pb2.StopAllCallsRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.StopCallsResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def TransferCall(request,
+                     target,
+                     options=(),
+                     channel_credentials=None,
+                     call_credentials=None,
+                     insecure=False,
+                     compression=None,
+                     wait_for_ready=None,
+                     timeout=None,
+                     metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/TransferCall',
+                                             ondewo_dot_vtsi_dot_calls__pb2.TransferCallRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.TransferCallResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def TransferCalls(request,
                       target,
                       options=(),
                       channel_credentials=None,
                       call_credentials=None,
                       insecure=False,
                       compression=None,
                       wait_for_ready=None,
                       timeout=None,
                       metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/TransferCalls',
-                                             ondewo_dot_vtsi_dot_voip__pb2.TransferCallsRequest.SerializeToString,
-                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/TransferCalls',
+                                             ondewo_dot_vtsi_dot_calls__pb2.TransferCallsRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.TransferCallsResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetVoipCallInfo(request,
-                        target,
-                        options=(),
-                        channel_credentials=None,
-                        call_credentials=None,
-                        insecure=False,
-                        compression=None,
-                        wait_for_ready=None,
-                        timeout=None,
-                        metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/GetVoipCallInfo',
-                                             ondewo_dot_vtsi_dot_voip__pb2.GetVoipCallInfoRequest.SerializeToString,
-                                             ondewo_dot_vtsi_dot_voip__pb2.GetVoipCallInfoResponse.FromString,
+    def GetCallInfo(request,
+                    target,
+                    options=(),
+                    channel_credentials=None,
+                    call_credentials=None,
+                    insecure=False,
+                    compression=None,
+                    wait_for_ready=None,
+                    timeout=None,
+                    metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/GetCallInfo',
+                                             ondewo_dot_vtsi_dot_calls__pb2.GetCallInfoRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.GetCallInfoResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListVoipCallInfo(request,
-                         target,
-                         options=(),
-                         channel_credentials=None,
-                         call_credentials=None,
-                         insecure=False,
-                         compression=None,
-                         wait_for_ready=None,
-                         timeout=None,
-                         metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/ListVoipCallInfo',
-                                             ondewo_dot_vtsi_dot_voip__pb2.ListVoipCallInfoRequest.SerializeToString,
-                                             ondewo_dot_vtsi_dot_voip__pb2.ListVoipCallInfoResponse.FromString,
+    def ListCallInfo(request,
+                     target,
+                     options=(),
+                     channel_credentials=None,
+                     call_credentials=None,
+                     insecure=False,
+                     compression=None,
+                     wait_for_ready=None,
+                     timeout=None,
+                     metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/ListCallInfo',
+                                             ondewo_dot_vtsi_dot_calls__pb2.ListCallInfoRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.ListCallInfoResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetAudioFile(request,
                      target,
                      options=(),
                      channel_credentials=None,
                      call_credentials=None,
                      insecure=False,
                      compression=None,
                      wait_for_ready=None,
                      timeout=None,
                      metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/GetAudioFile',
-                                             ondewo_dot_vtsi_dot_voip__pb2.GetAudioFileRequest.SerializeToString,
-                                             ondewo_dot_vtsi_dot_voip__pb2.GetAudioFileResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/GetAudioFile',
+                                             ondewo_dot_vtsi_dot_calls__pb2.GetAudioFileRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.GetAudioFileResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetFullConversationAudioFile(request,
                                      target,
                                      options=(),
                                      channel_credentials=None,
                                      call_credentials=None,
                                      insecure=False,
                                      compression=None,
                                      wait_for_ready=None,
                                      timeout=None,
                                      metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.VoipSessions/GetFullConversationAudioFile',
-                                             ondewo_dot_vtsi_dot_voip__pb2.GetFullConversationAudioFileRequest.SerializeToString,
-                                             ondewo_dot_vtsi_dot_voip__pb2.GetFullConversationAudioFileResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/GetFullConversationAudioFile',
+                                             ondewo_dot_vtsi_dot_calls__pb2.GetFullConversationAudioFileRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.GetFullConversationAudioFileResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `ondewo-vtsi-client-5.0.0/ondewo_vtsi_client.egg-info/SOURCES.txt` & `ondewo-vtsi-client-6.0.0/ondewo_vtsi_client.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -44,15 +44,23 @@
 ondewo/sip/__init__.py
 ondewo/sip/sip_pb2.py
 ondewo/sip/sip_pb2_grpc.py
 ondewo/t2s/__init__.py
 ondewo/t2s/text_to_speech_pb2.py
 ondewo/t2s/text_to_speech_pb2_grpc.py
 ondewo/vtsi/__init__.py
-ondewo/vtsi/client.py
-ondewo/vtsi/voip_pb2.py
-ondewo/vtsi/voip_pb2_grpc.py
+ondewo/vtsi/calls_pb2.py
+ondewo/vtsi/calls_pb2_grpc.py
+ondewo/vtsi/projects_pb2.py
+ondewo/vtsi/projects_pb2_grpc.py
+ondewo/vtsi/client/__init__.py
+ondewo/vtsi/client/client.py
+ondewo/vtsi/client/client_config.py
+ondewo/vtsi/client/services_container.py
+ondewo/vtsi/client/services/__init__.py
+ondewo/vtsi/client/services/calls.py
+ondewo/vtsi/client/services/projects.py
 ondewo_vtsi_client.egg-info/PKG-INFO
 ondewo_vtsi_client.egg-info/SOURCES.txt
 ondewo_vtsi_client.egg-info/dependency_links.txt
 ondewo_vtsi_client.egg-info/requires.txt
 ondewo_vtsi_client.egg-info/top_level.txt
```

### Comparing `ondewo-vtsi-client-5.0.0/setup.py` & `ondewo-vtsi-client-6.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import setuptools
+from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 with open("requirements.txt") as f:
     requires = []
     for line in f:
@@ -10,31 +10,42 @@
         if "#egg=" in req:
             req_url, req_name = req.split("#egg=")
             req_str = f"{req_name} @ {req_url}"
         else:
             req_str = req
         requires.append(req_str)
 
-setuptools.setup(
+setup(
     name="ondewo-vtsi-client",
-    version='5.0.0',
-    author="ONDEWO GbmH",
-    author_email="info@ondewo.com",
+    version='6.0.0',
+    author="Ondewo GbmH",
+    author_email="office@ondewo.com",
     description="exposes the ondewo-vtsi endpoints in a user-friendly way",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ondewo/ondewo-vtsi-client-python",
     packages=[
-        np for np in filter(lambda n: n.startswith("ondewo.") or n == "ondewo", setuptools.find_packages())
+        np
+        for np in filter(
+            lambda n: n.startswith('ondewo.') or n == 'ondewo',
+            find_packages()
+        )
     ],
+    include_package_data=True,
     package_data={
-        'ondewo.vtsi': ['py.typed']
+        'ondewo.vtsi': ['py.typed', '*.pyi'],
+        'ondewo.nlu': ['py.typed', '*.pyi'],
+        'ondewo.qa': ['py.typed', '*.pyi'],
+        'ondewo.s2t': ['py.typed', '*.pyi'],
+        'ondewo.t2s': ['py.typed', '*.pyi'],
+        'ondewo.csi': ['py.typed', '*.pyi'],
+        'ondewo.sip': ['py.typed', '*.pyi'],
     },
     classifiers=[
-        "Programming Language :: Python :: 3",
-        "Operating System :: OS Independent",
-        "Development Status :: 3 - Alpha",
-        "Topic :: Software Development :: Libraries",
+        'Programming Language :: Python :: 3.8',
+        'Operating System :: OS Independent',
+        'Development Status :: 5 - Production/Stable',
+        'Topic :: Software Development :: Libraries',
     ],
-    python_requires=">=2.7, !=3.0.1",
+    python_requires='>=3',
     install_requires=requires,
 )
```

