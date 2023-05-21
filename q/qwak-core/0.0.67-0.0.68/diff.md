# Comparing `tmp/qwak_core-0.0.67.tar.gz` & `tmp/qwak_core-0.0.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.67.tar", max compression
+gzip compressed data, was "qwak_core-0.0.68.tar", max compression
```

## Comparing `qwak_core-0.0.67.tar` & `qwak_core-0.0.68.tar`

### file list

```diff
@@ -1,582 +1,582 @@
--rw-r--r--   0        0        0      264 2023-05-21 11:46:05.104022 qwak_core-0.0.67/README.md
--rw-r--r--   0        0        0        0 2023-05-21 11:47:47.088438 qwak_core-0.0.67/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-21 11:47:47.112439 qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-21 11:47:26.456353 qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.112439 qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-21 11:47:47.108438 qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-21 11:47:26.088351 qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.108438 qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-21 11:47:47.108438 qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-21 11:47:26.272352 qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.108438 qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-21 11:47:47.100438 qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-21 11:47:25.536349 qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-21 11:47:47.100438 qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-21 11:47:47.104438 qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-21 11:47:25.716350 qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.104438 qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-21 11:47:47.104438 qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-21 11:47:25.900350 qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.104438 qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-21 11:47:47.088438 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-21 11:47:25.356348 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-21 11:47:47.088438 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-21 11:47:47.088438 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-21 11:47:26.724354 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.092438 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-21 11:47:47.092438 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-21 11:47:27.096356 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.096438 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-21 11:47:47.096438 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-21 11:47:27.280356 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-21 11:47:47.096438 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-21 11:47:47.092438 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-21 11:47:26.908355 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.092438 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-21 11:47:47.096438 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-21 11:47:27.468357 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.100438 qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-21 11:47:47.140439 qwak_core-0.0.67/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-21 11:47:30.156368 qwak_core-0.0.67/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.140439 qwak_core-0.0.67/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-21 11:47:47.144439 qwak_core-0.0.67/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-21 11:47:30.340369 qwak_core-0.0.67/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-21 11:47:47.144439 qwak_core-0.0.67/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-21 11:47:47.212439 qwak_core-0.0.67/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-21 11:47:35.516390 qwak_core-0.0.67/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.212439 qwak_core-0.0.67/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-21 11:47:47.212439 qwak_core-0.0.67/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-21 11:47:35.696391 qwak_core-0.0.67/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-21 11:47:47.216439 qwak_core-0.0.67/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-21 11:47:47.216439 qwak_core-0.0.67/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-21 11:47:36.616395 qwak_core-0.0.67/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-21 11:47:47.220439 qwak_core-0.0.67/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-21 11:47:47.216439 qwak_core-0.0.67/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-21 11:47:36.436394 qwak_core-0.0.67/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.216439 qwak_core-0.0.67/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-05-21 11:47:47.220439 qwak_core-0.0.67/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-05-21 11:47:36.800396 qwak_core-0.0.67/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.220439 qwak_core-0.0.67/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-21 11:47:47.220439 qwak_core-0.0.67/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-21 11:47:36.980396 qwak_core-0.0.67/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-21 11:47:47.224439 qwak_core-0.0.67/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-21 11:47:47.312439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-21 11:47:44.808429 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.312439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-05-21 11:47:47.308439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-05-21 11:47:44.444427 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.308439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-21 11:47:47.312439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-21 11:47:44.620428 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.312439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-21 11:47:47.304439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-21 11:47:44.072426 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-21 11:47:47.304439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-21 11:47:47.308439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-21 11:47:44.260427 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.308439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-21 11:47:47.320439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-21 11:47:45.352431 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.320439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-21 11:47:47.316439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-21 11:47:45.176430 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.316439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-21 11:47:47.316439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-21 11:47:44.988430 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.316439 qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-21 11:47:47.300439 qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-21 11:47:43.868425 qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.304439 qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-21 11:47:47.296439 qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-21 11:47:43.488423 qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.300439 qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-21 11:47:47.300439 qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-21 11:47:43.684424 qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-21 11:47:47.300439 qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-21 11:47:47.248439 qwak_core-0.0.67/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-21 11:47:38.836404 qwak_core-0.0.67/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-21 11:47:47.248439 qwak_core-0.0.67/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-21 11:47:47.244439 qwak_core-0.0.67/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-21 11:47:38.656403 qwak_core-0.0.67/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.248439 qwak_core-0.0.67/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-21 11:47:47.236439 qwak_core-0.0.67/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-21 11:47:38.284402 qwak_core-0.0.67/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.236439 qwak_core-0.0.67/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-21 11:47:47.240439 qwak_core-0.0.67/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-21 11:47:38.468402 qwak_core-0.0.67/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.240439 qwak_core-0.0.67/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-21 11:47:47.240439 qwak_core-0.0.67/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-21 11:47:39.020405 qwak_core-0.0.67/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-21 11:47:47.244439 qwak_core-0.0.67/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-21 11:47:47.244439 qwak_core-0.0.67/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-21 11:47:39.416406 qwak_core-0.0.67/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-21 11:47:47.244439 qwak_core-0.0.67/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-21 11:47:47.256439 qwak_core-0.0.67/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-21 11:47:39.796408 qwak_core-0.0.67/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.256439 qwak_core-0.0.67/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-21 11:47:47.256439 qwak_core-0.0.67/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-21 11:47:39.980409 qwak_core-0.0.67/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-21 11:47:47.256439 qwak_core-0.0.67/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-21 11:47:47.232439 qwak_core-0.0.67/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-21 11:47:37.736400 qwak_core-0.0.67/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.232439 qwak_core-0.0.67/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-21 11:47:47.232439 qwak_core-0.0.67/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-21 11:47:37.916400 qwak_core-0.0.67/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-21 11:47:47.232439 qwak_core-0.0.67/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-21 11:47:47.228439 qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-21 11:47:37.360398 qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.228439 qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-21 11:47:47.224439 qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-21 11:47:37.176397 qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.224439 qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-21 11:47:47.228439 qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-21 11:47:37.552399 qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-21 11:47:47.228439 qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-21 11:47:47.128439 qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-21 11:47:29.240364 qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.132439 qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-21 11:47:47.132439 qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-21 11:47:29.424365 qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.132439 qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-21 11:47:47.132439 qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-21 11:47:29.612366 qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-21 11:47:47.136438 qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-21 11:47:47.192439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-21 11:47:34.432386 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.192439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-21 11:47:47.188439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-21 11:47:34.248385 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-21 11:47:47.192439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-21 11:47:47.172439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-21 11:47:32.564378 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.172439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-21 11:47:47.168439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-21 11:47:32.384377 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.168439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-21 11:47:47.160439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-21 11:47:31.816375 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.164439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-21 11:47:47.168439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-21 11:47:32.200377 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-21 11:47:47.168439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-21 11:47:47.172439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-21 11:47:32.748379 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.172439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-21 11:47:47.176439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-21 11:47:32.932380 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-21 11:47:47.176439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25222 2023-05-21 11:47:47.164439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37429 2023-05-21 11:47:32.008376 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.164439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-21 11:47:47.176439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-21 11:47:33.112380 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.180439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     7284 2023-05-21 11:47:47.180439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0     8518 2023-05-21 11:47:33.296381 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.180439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-21 11:47:47.196439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-21 11:47:46.636436 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.196439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-21 11:47:47.196439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-21 11:47:46.820437 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-21 11:47:47.196439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-21 11:47:47.200439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-21 11:47:34.976388 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.200439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-21 11:47:47.200439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-21 11:47:35.156389 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-21 11:47:47.200439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-21 11:47:47.204439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-21 11:47:35.336389 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.204439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-21 11:47:47.208439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-21 11:47:36.064392 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.208439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-21 11:47:47.204439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-21 11:47:35.880392 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-21 11:47:47.204439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-21 11:47:47.208439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-21 11:47:36.252393 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.208439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-21 11:47:47.180439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-21 11:47:33.476382 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.184439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-21 11:47:47.184439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-21 11:47:33.660383 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.184439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-21 11:47:47.184439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-21 11:47:33.844383 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-21 11:47:47.188439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-21 11:47:47.188439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-21 11:47:34.064384 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.188439 qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-21 11:47:47.320439 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-21 11:47:45.536432 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.320439 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-21 11:47:47.324439 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-21 11:47:45.716433 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-21 11:47:47.324439 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-21 11:47:47.324439 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-21 11:47:45.896433 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.328439 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-21 11:47:47.328439 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-21 11:47:46.080434 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-21 11:47:47.328439 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-21 11:47:47.328439 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-21 11:47:46.268435 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-21 11:47:47.332439 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-21 11:47:47.332439 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-21 11:47:46.452436 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.332439 qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-21 11:47:47.260439 qwak_core-0.0.67/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-21 11:47:40.160410 qwak_core-0.0.67/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.260439 qwak_core-0.0.67/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-21 11:47:47.260439 qwak_core-0.0.67/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-21 11:47:40.344410 qwak_core-0.0.67/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-21 11:47:47.260439 qwak_core-0.0.67/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-21 11:47:47.148439 qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-21 11:47:31.080372 qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.148439 qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-21 11:47:47.152438 qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-21 11:47:31.260372 qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.152438 qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-21 11:47:47.156439 qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-21 11:47:31.440373 qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-21 11:47:47.156439 qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-21 11:47:47.160439 qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-21 11:47:31.628374 qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.160439 qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-21 11:47:47.236439 qwak_core-0.0.67/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-21 11:47:38.100401 qwak_core-0.0.67/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-21 11:47:47.236439 qwak_core-0.0.67/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-05-21 11:47:47.264439 qwak_core-0.0.67/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-05-21 11:47:40.528411 qwak_core-0.0.67/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.264439 qwak_core-0.0.67/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-05-21 11:47:47.264439 qwak_core-0.0.67/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-05-21 11:47:40.712412 qwak_core-0.0.67/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-05-21 11:47:47.264439 qwak_core-0.0.67/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-21 11:47:47.276439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-21 11:47:41.808416 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.280439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-21 11:47:47.280439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-21 11:47:41.992417 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.280439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-21 11:47:47.280439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-21 11:47:42.176418 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.284439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-21 11:47:47.284439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-21 11:47:42.360419 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.284439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-21 11:47:47.288439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-21 11:47:42.552420 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.288439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-21 11:47:47.288439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-21 11:47:42.752420 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-21 11:47:47.288439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-21 11:47:47.292439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-21 11:47:42.932421 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.292439 qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-21 11:47:47.268439 qwak_core-0.0.67/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-21 11:47:41.076413 qwak_core-0.0.67/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.272439 qwak_core-0.0.67/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-21 11:47:47.276439 qwak_core-0.0.67/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-21 11:47:41.620416 qwak_core-0.0.67/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.276439 qwak_core-0.0.67/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-21 11:47:47.272439 qwak_core-0.0.67/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-21 11:47:41.256414 qwak_core-0.0.67/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-21 11:47:47.272439 qwak_core-0.0.67/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-05-21 11:47:47.272439 qwak_core-0.0.67/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-05-21 11:47:41.440415 qwak_core-0.0.67/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.276439 qwak_core-0.0.67/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-21 11:47:47.252439 qwak_core-0.0.67/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-21 11:47:39.616407 qwak_core-0.0.67/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-21 11:47:47.252439 qwak_core-0.0.67/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-21 11:47:47.124438 qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-21 11:47:30.712370 qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-21 11:47:47.128439 qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-21 11:47:47.124438 qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-21 11:47:30.524370 qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.124438 qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-21 11:47:47.128439 qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-21 11:47:30.896371 qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-21 11:47:47.128439 qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-21 11:47:47.252439 qwak_core-0.0.67/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-21 11:47:39.212406 qwak_core-0.0.67/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-21 11:47:47.252439 qwak_core-0.0.67/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-21 11:47:47.268439 qwak_core-0.0.67/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-21 11:47:40.896412 qwak_core-0.0.67/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-21 11:47:47.268439 qwak_core-0.0.67/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-21 11:47:47.120438 qwak_core-0.0.67/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-21 11:47:28.488361 qwak_core-0.0.67/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.124438 qwak_core-0.0.67/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-21 11:47:47.120438 qwak_core-0.0.67/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-21 11:47:28.304360 qwak_core-0.0.67/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-21 11:47:47.120438 qwak_core-0.0.67/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-21 11:47:47.112439 qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-21 11:47:27.652358 qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.112439 qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-21 11:47:47.116438 qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-21 11:47:27.932359 qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.116438 qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-21 11:47:47.116438 qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-21 11:47:28.120360 qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-21 11:47:47.116438 qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-21 11:47:47.296439 qwak_core-0.0.67/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-21 11:47:43.304422 qwak_core-0.0.67/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-21 11:47:47.296439 qwak_core-0.0.67/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-21 11:47:47.292439 qwak_core-0.0.67/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-21 11:47:43.116422 qwak_core-0.0.67/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.292439 qwak_core-0.0.67/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-21 11:47:47.136438 qwak_core-0.0.67/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    15881 2023-05-21 11:47:29.792367 qwak_core-0.0.67/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.136438 qwak_core-0.0.67/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-21 11:47:47.140439 qwak_core-0.0.67/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-21 11:47:29.972367 qwak_core-0.0.67/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-21 11:47:47.140439 qwak_core-0.0.67/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-21 11:47:48.548444 qwak_core-0.0.67/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-21 11:47:48.548444 qwak_core-0.0.67/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    18744 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14847 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-21 11:46:05.104022 qwak_core-0.0.67/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-21 11:46:05.108022 qwak_core-0.0.67/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-21 11:46:05.112022 qwak_core-0.0.67/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.67/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.67/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-21 13:17:24.735218 qwak_core-0.0.68/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 13:19:06.779656 qwak_core-0.0.68/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-21 13:19:06.803656 qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-21 13:18:45.667565 qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.807656 qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-21 13:19:06.799656 qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-21 13:18:45.303563 qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.803656 qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-21 13:19:06.803656 qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-21 13:18:45.483564 qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.803656 qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-21 13:19:06.795656 qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-21 13:18:44.723561 qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-21 13:19:06.795656 qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-21 13:19:06.795656 qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-21 13:18:44.923562 qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.799656 qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-21 13:19:06.799656 qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-21 13:18:45.123563 qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.799656 qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-21 13:19:06.783656 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-21 13:18:44.543560 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-21 13:19:06.783656 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-21 13:19:06.783656 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-21 13:18:45.851566 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.783656 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-21 13:19:06.787656 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-21 13:18:46.215567 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.787656 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-21 13:19:06.791656 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-21 13:18:46.403568 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-21 13:19:06.791656 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-21 13:19:06.787656 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-21 13:18:46.031567 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.787656 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-21 13:19:06.791656 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-21 13:18:46.595569 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.795656 qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-21 13:19:06.835656 qwak_core-0.0.68/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-21 13:18:49.219580 qwak_core-0.0.68/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.835656 qwak_core-0.0.68/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-21 13:19:06.835656 qwak_core-0.0.68/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-21 13:18:49.399581 qwak_core-0.0.68/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-21 13:19:06.839656 qwak_core-0.0.68/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-21 13:19:06.903656 qwak_core-0.0.68/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-21 13:18:54.551603 qwak_core-0.0.68/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.903656 qwak_core-0.0.68/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-21 13:19:06.907656 qwak_core-0.0.68/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-21 13:18:54.735604 qwak_core-0.0.68/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-21 13:19:06.907656 qwak_core-0.0.68/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-21 13:19:06.911656 qwak_core-0.0.68/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-21 13:18:55.719608 qwak_core-0.0.68/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-21 13:19:06.911656 qwak_core-0.0.68/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-21 13:19:06.907656 qwak_core-0.0.68/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-21 13:18:55.515607 qwak_core-0.0.68/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.907656 qwak_core-0.0.68/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-05-21 13:19:06.911656 qwak_core-0.0.68/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-05-21 13:18:55.919609 qwak_core-0.0.68/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.911656 qwak_core-0.0.68/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-21 13:19:06.915656 qwak_core-0.0.68/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-21 13:18:56.115610 qwak_core-0.0.68/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-21 13:19:06.915656 qwak_core-0.0.68/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-21 13:19:07.003656 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-21 13:19:04.487646 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:07.007656 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-05-21 13:19:06.999657 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-05-21 13:19:04.115644 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:07.003656 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-21 13:19:07.003656 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-21 13:19:04.295645 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:07.003656 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-21 13:19:06.995657 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-21 13:19:03.731643 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-21 13:19:06.995657 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-21 13:19:06.999657 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-21 13:19:03.931643 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.999657 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-21 13:19:07.011657 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-21 13:19:05.031648 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:07.011657 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-21 13:19:07.007656 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-21 13:19:04.851647 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:07.011657 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-21 13:19:07.007656 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-21 13:19:04.671646 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:07.007656 qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-21 13:19:06.995657 qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-21 13:19:03.531642 qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.995657 qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-21 13:19:06.991656 qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-21 13:19:03.091640 qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.991656 qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-21 13:19:06.991656 qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-21 13:19:03.307641 qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-21 13:19:06.991656 qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-05-21 13:19:06.939656 qwak_core-0.0.68/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-05-21 13:18:58.375620 qwak_core-0.0.68/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-05-21 13:19:06.943656 qwak_core-0.0.68/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-21 13:19:06.939656 qwak_core-0.0.68/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-21 13:18:58.151619 qwak_core-0.0.68/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.939656 qwak_core-0.0.68/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-21 13:19:06.931656 qwak_core-0.0.68/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-21 13:18:57.695617 qwak_core-0.0.68/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.931656 qwak_core-0.0.68/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-21 13:19:06.931656 qwak_core-0.0.68/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-21 13:18:57.911618 qwak_core-0.0.68/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.931656 qwak_core-0.0.68/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-21 13:19:06.935656 qwak_core-0.0.68/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-21 13:18:58.579620 qwak_core-0.0.68/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-21 13:19:06.935656 qwak_core-0.0.68/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-21 13:19:06.935656 qwak_core-0.0.68/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-21 13:18:58.983622 qwak_core-0.0.68/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-21 13:19:06.935656 qwak_core-0.0.68/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-21 13:19:06.947656 qwak_core-0.0.68/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-21 13:18:59.363624 qwak_core-0.0.68/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.947656 qwak_core-0.0.68/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-21 13:19:06.947656 qwak_core-0.0.68/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-21 13:18:59.547624 qwak_core-0.0.68/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-21 13:19:06.951656 qwak_core-0.0.68/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-21 13:19:06.923656 qwak_core-0.0.68/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-21 13:18:57.023614 qwak_core-0.0.68/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.923656 qwak_core-0.0.68/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-21 13:19:06.923656 qwak_core-0.0.68/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-21 13:18:57.251615 qwak_core-0.0.68/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-21 13:19:06.927656 qwak_core-0.0.68/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-21 13:19:06.919656 qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-21 13:18:56.579612 qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.919656 qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-21 13:19:06.915656 qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-21 13:18:56.355611 qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.919656 qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-21 13:19:06.919656 qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-21 13:18:56.803613 qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-21 13:19:06.923656 qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-21 13:19:06.823656 qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-21 13:18:48.287576 qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.827656 qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-21 13:19:06.827656 qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-21 13:18:48.475577 qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.827656 qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-21 13:19:06.827656 qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-21 13:18:48.667578 qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-21 13:19:06.831656 qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-21 13:19:06.883656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-21 13:18:53.463599 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.887656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-21 13:19:06.883656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-21 13:18:53.283598 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-21 13:19:06.883656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-21 13:19:06.863656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-21 13:18:51.631591 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.863656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-21 13:19:06.859656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-21 13:18:51.447590 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.863656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-21 13:19:06.855656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-21 13:18:50.879588 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.855656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-21 13:19:06.859656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-21 13:18:51.267589 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-21 13:19:06.859656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-21 13:19:06.863656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-21 13:18:51.815591 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.867656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-21 13:19:06.867656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-21 13:18:51.999592 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-21 13:19:06.867656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25222 2023-05-21 13:19:06.855656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37429 2023-05-21 13:18:51.071588 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.859656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-21 13:19:06.871656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-21 13:18:52.183593 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.871656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     7284 2023-05-21 13:19:06.871656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0     8518 2023-05-21 13:18:52.363594 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.871656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-21 13:19:06.887656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-21 13:19:06.331654 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.887656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-21 13:19:06.887656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-21 13:19:06.511654 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-21 13:19:06.891656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-21 13:19:06.891656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-21 13:18:54.003601 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.891656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-21 13:19:06.891656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-21 13:18:54.187602 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-21 13:19:06.895656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-21 13:19:06.895656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-21 13:18:54.367602 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.895656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-21 13:19:06.899656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-21 13:18:55.107606 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.899656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-21 13:19:06.895656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-21 13:18:54.919605 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-21 13:19:06.899656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-21 13:19:06.903656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-21 13:18:55.311607 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.903656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-21 13:19:06.875656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-21 13:18:52.551595 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.875656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-21 13:19:06.875656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-21 13:18:52.735595 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.875656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-21 13:19:06.879656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-21 13:18:52.923596 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-21 13:19:06.879656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-21 13:19:06.879656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-21 13:18:53.103597 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.879656 qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-21 13:19:07.011657 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-21 13:19:05.219649 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:07.015657 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-21 13:19:07.015657 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-21 13:19:05.403650 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-21 13:19:07.015657 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-21 13:19:07.019657 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-21 13:19:05.587650 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:07.019657 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-21 13:19:07.019657 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-21 13:19:05.775651 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-21 13:19:07.019657 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-21 13:19:07.023657 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-21 13:19:05.971652 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-21 13:19:07.023657 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-21 13:19:07.023657 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-21 13:19:06.151653 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:07.023657 qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-21 13:19:06.951656 qwak_core-0.0.68/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-21 13:18:59.735625 qwak_core-0.0.68/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.951656 qwak_core-0.0.68/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-21 13:19:06.951656 qwak_core-0.0.68/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-21 13:18:59.919626 qwak_core-0.0.68/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-21 13:19:06.955656 qwak_core-0.0.68/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-21 13:19:06.839656 qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-21 13:18:50.139584 qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.843656 qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-21 13:19:06.843656 qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-21 13:18:50.323585 qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.847656 qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-21 13:19:06.847656 qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-21 13:18:50.503586 qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-21 13:19:06.851656 qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-21 13:19:06.851656 qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-21 13:18:50.687587 qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.851656 qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-21 13:19:06.927656 qwak_core-0.0.68/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-21 13:18:57.475616 qwak_core-0.0.68/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-21 13:19:06.927656 qwak_core-0.0.68/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-05-21 13:19:06.955656 qwak_core-0.0.68/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-05-21 13:19:00.099627 qwak_core-0.0.68/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.955656 qwak_core-0.0.68/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-05-21 13:19:06.959656 qwak_core-0.0.68/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-05-21 13:19:00.279628 qwak_core-0.0.68/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-05-21 13:19:06.959656 qwak_core-0.0.68/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-21 13:19:06.971656 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-21 13:19:01.371632 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.971656 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-21 13:19:06.971656 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-21 13:19:01.555633 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.971656 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-21 13:19:06.975656 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-21 13:19:01.747634 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.975656 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-21 13:19:06.975656 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-21 13:19:01.935635 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.979656 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-21 13:19:06.979656 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-21 13:19:02.127636 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.979656 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-21 13:19:06.979656 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-21 13:19:02.327637 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-21 13:19:06.983657 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-21 13:19:06.983657 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-21 13:19:02.511637 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.983657 qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-21 13:19:06.963656 qwak_core-0.0.68/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-21 13:19:00.643629 qwak_core-0.0.68/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.963656 qwak_core-0.0.68/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-21 13:19:06.967656 qwak_core-0.0.68/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-21 13:19:01.187632 qwak_core-0.0.68/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.967656 qwak_core-0.0.68/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-21 13:19:06.963656 qwak_core-0.0.68/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-21 13:19:00.823630 qwak_core-0.0.68/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-21 13:19:06.963656 qwak_core-0.0.68/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-05-21 13:19:06.967656 qwak_core-0.0.68/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-05-21 13:19:01.007631 qwak_core-0.0.68/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.967656 qwak_core-0.0.68/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-21 13:19:06.943656 qwak_core-0.0.68/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-21 13:18:59.179623 qwak_core-0.0.68/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-21 13:19:06.947656 qwak_core-0.0.68/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-21 13:19:06.819656 qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-21 13:18:49.775583 qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-21 13:19:06.819656 qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-21 13:19:06.819656 qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-21 13:18:49.587582 qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.819656 qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-21 13:19:06.823656 qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-21 13:18:49.959583 qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-21 13:19:06.823656 qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-21 13:19:06.943656 qwak_core-0.0.68/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-21 13:18:58.779621 qwak_core-0.0.68/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-21 13:19:06.943656 qwak_core-0.0.68/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-21 13:19:06.959656 qwak_core-0.0.68/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-21 13:19:00.459628 qwak_core-0.0.68/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-21 13:19:06.959656 qwak_core-0.0.68/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-21 13:19:06.815656 qwak_core-0.0.68/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-21 13:18:47.519573 qwak_core-0.0.68/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.815656 qwak_core-0.0.68/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-21 13:19:06.815656 qwak_core-0.0.68/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-21 13:18:47.335572 qwak_core-0.0.68/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-21 13:19:06.815656 qwak_core-0.0.68/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-21 13:19:06.807656 qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-21 13:18:46.783570 qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.807656 qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-21 13:19:06.811656 qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-21 13:18:46.963571 qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.811656 qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-21 13:19:06.811656 qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-21 13:18:47.147571 qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-21 13:19:06.811656 qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-21 13:19:06.987656 qwak_core-0.0.68/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-21 13:19:02.907639 qwak_core-0.0.68/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-21 13:19:06.987656 qwak_core-0.0.68/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-21 13:19:06.983657 qwak_core-0.0.68/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-21 13:19:02.715638 qwak_core-0.0.68/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.987656 qwak_core-0.0.68/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-21 13:19:06.831656 qwak_core-0.0.68/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    15881 2023-05-21 13:18:48.851579 qwak_core-0.0.68/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.831656 qwak_core-0.0.68/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-21 13:19:06.831656 qwak_core-0.0.68/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-21 13:18:49.031580 qwak_core-0.0.68/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-21 13:19:06.835656 qwak_core-0.0.68/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-21 13:19:08.583663 qwak_core-0.0.68/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-21 13:19:08.583663 qwak_core-0.0.68/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    18744 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14847 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-21 13:17:24.739218 qwak_core-0.0.68/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-21 13:17:24.743218 qwak_core-0.0.68/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.68/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.68/PKG-INFO
```

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,29 +11,33 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%qwak/automation/v1/auto_scaling.proto\x12\x12qwak.automation.v1\"\xad\x01\n\x11\x41utoScalingConfig\x12\x19\n\x11min_replica_count\x18\x01 \x01(\x05\x12\x19\n\x11max_replica_count\x18\x02 \x01(\x05\x12\x18\n\x10polling_interval\x18\x03 \x01(\x05\x12\x18\n\x10\x63ool_down_period\x18\x04 \x01(\x05\x12.\n\x08triggers\x18\x05 \x01(\x0b\x32\x1c.qwak.automation.v1.Triggers\">\n\x08Triggers\x12\x32\n\x08triggers\x18\x01 \x03(\x0b\x32 .qwak.automation.v1.ScaleTrigger\"n\n\x0cScaleTrigger\x12N\n\x12prometheus_trigger\x18\x01 \x01(\x0b\x32\x30.qwak.automation.v1.AutoScalingPrometheusTriggerH\x00\x42\x0e\n\x0ctrigger_type\"d\n\x1c\x41utoScalingPrometheusTrigger\x12\x31\n\nquery_spec\x18\x01 \x01(\x0b\x32\x1d.qwak.automation.v1.QuerySpec\x12\x11\n\tthreshold\x18\x02 \x01(\x05\"\xaa\x01\n\tQuerySpec\x12>\n\x0bmetric_type\x18\x01 \x01(\x0e\x32).qwak.automation.v1.AutoScalingMetricType\x12H\n\x10\x61ggregation_type\x18\x02 \x01(\x0e\x32..qwak.automation.v1.AutoScalingAggregationType\x12\x13\n\x0btime_period\x18\x03 \x01(\x05*x\n\x15\x41utoScalingMetricType\x12\x19\n\x15METRIC_TYPE_NOT_VALID\x10\x00\x12\x13\n\x0fMETRIC_TYPE_CPU\x10\x01\x12\x16\n\x12METRIC_TYPE_MEMORY\x10\x02\x12\x17\n\x13METRIC_TYPE_LATENCY\x10\x03*\xa8\x01\n\x1a\x41utoScalingAggregationType\x12\x1e\n\x1a\x41GGREGATION_TYPE_NOT_VALID\x10\x00\x12\x18\n\x14\x41GGREGATION_TYPE_MIN\x10\x01\x12\x18\n\x14\x41GGREGATION_TYPE_MAX\x10\x02\x12\x1c\n\x18\x41GGREGATION_TYPE_AVERAGE\x10\x03\x12\x18\n\x14\x41GGREGATION_TYPE_SUM\x10\x04\x42!\n\x1d\x63om.qwak.ai.automation.api.v1P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%qwak/automation/v1/auto_scaling.proto\x12\x12qwak.automation.v1\"\xad\x01\n\x11\x41utoScalingConfig\x12\x19\n\x11min_replica_count\x18\x01 \x01(\x05\x12\x19\n\x11max_replica_count\x18\x02 \x01(\x05\x12\x18\n\x10polling_interval\x18\x03 \x01(\x05\x12\x18\n\x10\x63ool_down_period\x18\x04 \x01(\x05\x12.\n\x08triggers\x18\x05 \x01(\x0b\x32\x1c.qwak.automation.v1.Triggers\">\n\x08Triggers\x12\x32\n\x08triggers\x18\x01 \x03(\x0b\x32 .qwak.automation.v1.ScaleTrigger\"n\n\x0cScaleTrigger\x12N\n\x12prometheus_trigger\x18\x01 \x01(\x0b\x32\x30.qwak.automation.v1.AutoScalingPrometheusTriggerH\x00\x42\x0e\n\x0ctrigger_type\"d\n\x1c\x41utoScalingPrometheusTrigger\x12\x31\n\nquery_spec\x18\x01 \x01(\x0b\x32\x1d.qwak.automation.v1.QuerySpec\x12\x11\n\tthreshold\x18\x02 \x01(\x05\"\xaa\x01\n\tQuerySpec\x12>\n\x0bmetric_type\x18\x01 \x01(\x0e\x32).qwak.automation.v1.AutoScalingMetricType\x12H\n\x10\x61ggregation_type\x18\x02 \x01(\x0e\x32..qwak.automation.v1.AutoScalingAggregationType\x12\x13\n\x0btime_period\x18\x03 \x01(\x05*x\n\x15\x41utoScalingMetricType\x12\x19\n\x15METRIC_TYPE_NOT_VALID\x10\x00\x12\x13\n\x0fMETRIC_TYPE_CPU\x10\x01\x12\x16\n\x12METRIC_TYPE_MEMORY\x10\x02\x12\x17\n\x13METRIC_TYPE_LATENCY\x10\x03*\x90\x02\n\x1a\x41utoScalingAggregationType\x12\x1e\n\x1a\x41GGREGATION_TYPE_NOT_VALID\x10\x00\x12\x18\n\x14\x41GGREGATION_TYPE_MIN\x10\x01\x12\x18\n\x14\x41GGREGATION_TYPE_MAX\x10\x02\x12\x1c\n\x18\x41GGREGATION_TYPE_AVERAGE\x10\x03\x12\x18\n\x14\x41GGREGATION_TYPE_SUM\x10\x04\x12\x18\n\x14\x41GGREGATION_TYPE_P50\x10\x05\x12\x18\n\x14\x41GGREGATION_TYPE_P90\x10\x06\x12\x18\n\x14\x41GGREGATION_TYPE_P95\x10\x07\x12\x18\n\x14\x41GGREGATION_TYPE_P99\x10\x08\x42!\n\x1d\x63om.qwak.ai.automation.api.v1P\x01\x62\x06proto3')
 
 _AUTOSCALINGMETRICTYPE = DESCRIPTOR.enum_types_by_name['AutoScalingMetricType']
 AutoScalingMetricType = enum_type_wrapper.EnumTypeWrapper(_AUTOSCALINGMETRICTYPE)
 _AUTOSCALINGAGGREGATIONTYPE = DESCRIPTOR.enum_types_by_name['AutoScalingAggregationType']
 AutoScalingAggregationType = enum_type_wrapper.EnumTypeWrapper(_AUTOSCALINGAGGREGATIONTYPE)
 METRIC_TYPE_NOT_VALID = 0
 METRIC_TYPE_CPU = 1
 METRIC_TYPE_MEMORY = 2
 METRIC_TYPE_LATENCY = 3
 AGGREGATION_TYPE_NOT_VALID = 0
 AGGREGATION_TYPE_MIN = 1
 AGGREGATION_TYPE_MAX = 2
 AGGREGATION_TYPE_AVERAGE = 3
 AGGREGATION_TYPE_SUM = 4
+AGGREGATION_TYPE_P50 = 5
+AGGREGATION_TYPE_P90 = 6
+AGGREGATION_TYPE_P95 = 7
+AGGREGATION_TYPE_P99 = 8
 
 
 _AUTOSCALINGCONFIG = DESCRIPTOR.message_types_by_name['AutoScalingConfig']
 _TRIGGERS = DESCRIPTOR.message_types_by_name['Triggers']
 _SCALETRIGGER = DESCRIPTOR.message_types_by_name['ScaleTrigger']
 _AUTOSCALINGPROMETHEUSTRIGGER = DESCRIPTOR.message_types_by_name['AutoScalingPrometheusTrigger']
 _QUERYSPEC = DESCRIPTOR.message_types_by_name['QuerySpec']
@@ -75,15 +79,15 @@
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\035com.qwak.ai.automation.api.v1P\001'
   _AUTOSCALINGMETRICTYPE._serialized_start=688
   _AUTOSCALINGMETRICTYPE._serialized_end=808
   _AUTOSCALINGAGGREGATIONTYPE._serialized_start=811
-  _AUTOSCALINGAGGREGATIONTYPE._serialized_end=979
+  _AUTOSCALINGAGGREGATIONTYPE._serialized_end=1083
   _AUTOSCALINGCONFIG._serialized_start=62
   _AUTOSCALINGCONFIG._serialized_end=235
   _TRIGGERS._serialized_start=237
   _TRIGGERS._serialized_end=299
   _SCALETRIGGER._serialized_start=301
   _SCALETRIGGER._serialized_end=411
   _AUTOSCALINGPROMETHEUSTRIGGER._serialized_start=413
```

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -44,22 +44,30 @@
 class _AutoScalingAggregationTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_AutoScalingAggregationType.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     AGGREGATION_TYPE_NOT_VALID: _AutoScalingAggregationType.ValueType  # 0
     AGGREGATION_TYPE_MIN: _AutoScalingAggregationType.ValueType  # 1
     AGGREGATION_TYPE_MAX: _AutoScalingAggregationType.ValueType  # 2
     AGGREGATION_TYPE_AVERAGE: _AutoScalingAggregationType.ValueType  # 3
     AGGREGATION_TYPE_SUM: _AutoScalingAggregationType.ValueType  # 4
+    AGGREGATION_TYPE_P50: _AutoScalingAggregationType.ValueType  # 5
+    AGGREGATION_TYPE_P90: _AutoScalingAggregationType.ValueType  # 6
+    AGGREGATION_TYPE_P95: _AutoScalingAggregationType.ValueType  # 7
+    AGGREGATION_TYPE_P99: _AutoScalingAggregationType.ValueType  # 8
 
 class AutoScalingAggregationType(_AutoScalingAggregationType, metaclass=_AutoScalingAggregationTypeEnumTypeWrapper): ...
 
 AGGREGATION_TYPE_NOT_VALID: AutoScalingAggregationType.ValueType  # 0
 AGGREGATION_TYPE_MIN: AutoScalingAggregationType.ValueType  # 1
 AGGREGATION_TYPE_MAX: AutoScalingAggregationType.ValueType  # 2
 AGGREGATION_TYPE_AVERAGE: AutoScalingAggregationType.ValueType  # 3
 AGGREGATION_TYPE_SUM: AutoScalingAggregationType.ValueType  # 4
+AGGREGATION_TYPE_P50: AutoScalingAggregationType.ValueType  # 5
+AGGREGATION_TYPE_P90: AutoScalingAggregationType.ValueType  # 6
+AGGREGATION_TYPE_P95: AutoScalingAggregationType.ValueType  # 7
+AGGREGATION_TYPE_P99: AutoScalingAggregationType.ValueType  # 8
 global___AutoScalingAggregationType = AutoScalingAggregationType
 
 class AutoScalingConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MIN_REPLICA_COUNT_FIELD_NUMBER: builtins.int
     MAX_REPLICA_COUNT_FIELD_NUMBER: builtins.int
```

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.68/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.68/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.68/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/pyproject.toml` & `qwak_core-0.0.68/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.67"
+version = "0.0.68"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.67/qwak/automations/__init__.py` & `qwak_core-0.0.68/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/automations/automation_executions.py` & `qwak_core-0.0.68/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/automations/automations.py` & `qwak_core-0.0.68/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.68/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.68/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/automations/common.py` & `qwak_core-0.0.68/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.68/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.68/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.68/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.68/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.68/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/alert_management/client.py` & `qwak_core-0.0.68/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/analytics/client.py` & `qwak_core-0.0.68/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/audience/client.py` & `qwak_core-0.0.68/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/automation_management/client.py` & `qwak_core-0.0.68/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.68/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.68/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.68/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.68/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/build_management/client.py` & `qwak_core-0.0.68/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.68/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.68/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/deployment/client.py` & `qwak_core-0.0.68/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.68/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.68/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.68/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.68/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/instance_template/client.py` & `qwak_core-0.0.68/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.68/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/logging_client/client.py` & `qwak_core-0.0.68/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/model_management/client.py` & `qwak_core-0.0.68/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/project/client.py` & `qwak_core-0.0.68/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/secret_service/client.py` & `qwak_core-0.0.68/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.68/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.68/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.68/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.68/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.68/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.68/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.68/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.68/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.68/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.68/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.68/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.68/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.68/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.68/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.68/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/offline/client.py` & `qwak_core-0.0.68/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/feature_store/online/client.py` & `qwak_core-0.0.68/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/inner/const.py` & `qwak_core-0.0.68/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.68/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.68/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.68/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.68/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/inner/singleton_meta.py` & `qwak_core-0.0.68/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/inner/tool/auth.py` & `qwak_core-0.0.68/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.68/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.68/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.68/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.68/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/adapters/__init__.py` & `qwak_core-0.0.68/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.68/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.68/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.68/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.68/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.68/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/base.py` & `qwak_core-0.0.68/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/decorators/api.py` & `qwak_core-0.0.68/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.68/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/experiment_tracking.py` & `qwak_core-0.0.68/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/schema.py` & `qwak_core-0.0.68/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/schema_entities.py` & `qwak_core-0.0.68/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.68/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.68/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.68/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.68/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.68/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.68/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.68/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.68/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.68/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.68/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.68/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.68/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.68/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.68/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.68/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.68/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.68/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.68/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.68/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/qwak_client/client.py` & `qwak_core-0.0.68/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.68/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/qwak_client/models/model.py` & `qwak_core-0.0.68/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.68/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.68/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/tools/logger/logger.py` & `qwak_core-0.0.68/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak/tools/logger/logging.yml` & `qwak_core-0.0.68/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.68/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/qwak_services_mock/services_mock.py` & `qwak_core-0.0.68/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.67/setup.py` & `qwak_core-0.0.68/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.67',
+    'version': '0.0.68',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.67/PKG-INFO` & `qwak_core-0.0.68/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.67
+Version: 0.0.68
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

