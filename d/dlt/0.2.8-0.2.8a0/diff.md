# Comparing `tmp/dlt-0.2.8.tar.gz` & `tmp/dlt-0.2.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.2.8.tar", max compression
+gzip compressed data, was "dlt-0.2.8a0.tar", max compression
```

## Comparing `dlt-0.2.8.tar` & `dlt-0.2.8a0.tar`

### file list

```diff
@@ -1,208 +1,209 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.2.8/LICENSE.txt
--rw-r--r--   0        0        0     4214 2023-04-30 21:17:44.388805 dlt-0.2.8/README.md
--rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.2.8/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.2.8/dlt/cli/__init__.py
--rw-r--r--   0        0        0    15909 2023-05-07 23:03:04.659469 dlt-0.2.8/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3858 2023-05-07 23:03:04.659469 dlt-0.2.8/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    16665 2023-05-14 20:33:31.539348 dlt-0.2.8/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.2.8/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18827 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10489 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9422 2023-05-14 20:33:31.539348 dlt-0.2.8/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4505 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-04-22 20:26:30.632198 dlt-0.2.8/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     3757 2023-04-30 21:17:44.388805 dlt-0.2.8/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.2.8/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      428 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5078 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3469 2023-05-07 23:03:04.659469 dlt-0.2.8/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     5884 2023-04-22 20:26:30.632198 dlt-0.2.8/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.2.8/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.2.8/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      306 2023-05-07 23:03:04.659469 dlt-0.2.8/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0     1108 2023-05-19 14:44:37.212613 dlt-0.2.8/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.2.8/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.2.8/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.2.8/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     8349 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1306 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0     6560 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    17262 2023-05-14 20:33:31.539348 dlt-0.2.8/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0      912 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.2.8/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0    13108 2023-05-20 17:49:45.908821 dlt-0.2.8/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     5521 2023-05-14 20:33:31.539348 dlt-0.2.8/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     2792 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1818 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.2.8/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.2.8/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6026 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.2.8/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     5893 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2395 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0       97 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.2.8/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    10682 2023-04-24 11:35:34.867759 dlt-0.2.8/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6451 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/git.py
--rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.2.8/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.2.8/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.2.8/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.2.8/dlt/common/jsonpath.py
--rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.2.8/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.2.8/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.2.8/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.2.8/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.2.8/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/pendulum.py
--rw-r--r--   0        0        0    19121 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.2.8/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.2.8/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.2.8/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.2.8/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      705 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.2.8/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.2.8/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13441 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.2.8/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.2.8/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.2.8/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.2.8/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25175 2023-04-09 16:39:04.593180 dlt-0.2.8/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.2.8/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23087 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1467 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/source.py
--rw-r--r--   0        0        0      554 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1649 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     2804 2023-04-03 18:50:36.893525 dlt-0.2.8/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    10891 2023-05-14 20:33:31.539348 dlt-0.2.8/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2690 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21812 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2409 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8434 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.2.8/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.2.8/dlt/common/typing.py
--rw-r--r--   0        0        0    12696 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.2.8/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    12347 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10342 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.2.8/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7008 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.2.8/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.2.8/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4975 2023-04-24 11:35:34.867759 dlt-0.2.8/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.2.8/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     4983 2023-04-05 08:03:40.638919 dlt-0.2.8/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    15625 2023-05-18 22:16:41.982767 dlt-0.2.8/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.2.8/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.2.8/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0     1232 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     6074 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.2.8/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.2.8/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     7110 2023-04-29 12:58:55.953219 dlt-0.2.8/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    10101 2023-04-09 16:39:04.593180 dlt-0.2.8/dlt/destinations/sql_merge_job.py
--rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.2.8/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.8/dlt/extract/__init__.py
--rw-r--r--   0        0        0    26199 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12645 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     8451 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/extract/extract.py
--rw-r--r--   0        0        0    14954 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/extract/incremental.py
--rw-r--r--   0        0        0    31737 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-04-22 20:26:30.632198 dlt-0.2.8/dlt/extract/schema.py
--rw-r--r--   0        0        0    34714 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/extract/source.py
--rw-r--r--   0        0        0     4350 2023-04-22 20:26:30.632198 dlt-0.2.8/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.2.8/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.2.8/dlt/helpers/__init__.py
--rw-r--r--   0        0        0      267 2023-05-14 20:33:31.539348 dlt-0.2.8/dlt/helpers/airflow.py
--rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.2.8/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2490 2023-05-14 20:33:31.539348 dlt-0.2.8/dlt/helpers/pandas.py
--rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.2.8/dlt/helpers/parquet.py
--rw-r--r--   0        0        0    13371 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/helpers/streamlit.py
--rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.2.8/dlt/load/__init__.py
--rw-r--r--   0        0        0     1005 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.2.8/dlt/load/exceptions.py
--rw-r--r--   0        0        0    19928 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.2.8/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1101 2023-05-21 19:00:09.602319 dlt-0.2.8/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.8/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    16538 2023-05-21 19:00:09.612319 dlt-0.2.8/dlt/normalize/normalize.py
--rw-r--r--   0        0        0     1880 2023-03-23 14:48:32.571618 dlt-0.2.8/dlt/pipeline/README.md
--rw-r--r--   0        0        0    13138 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      379 2023-05-21 19:00:09.612319 dlt-0.2.8/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.2.8/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     2891 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8764 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.2.8/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    56483 2023-05-21 19:00:09.612319 dlt-0.2.8/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.2.8/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4200 2023-04-10 08:12:53.769595 dlt-0.2.8/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.2.8/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     4563 2023-04-03 18:50:36.903525 dlt-0.2.8/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.2.8/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.2.8/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.8/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.2.8/dlt/reflection/names.py
--rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.2.8/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/sources/__init__.py
--rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.2.8/dlt/sources/credentials.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.8/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.2.8/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0     9106 2023-05-14 20:33:31.539348 dlt-0.2.8/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.2.8/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.2.8/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.2.8/dlt/version.py
--rw-r--r--   0        0        0     4054 2023-05-21 19:00:09.612319 dlt-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     7369 1970-01-01 00:00:00.000000 dlt-0.2.8/setup.py
--rw-r--r--   0        0        0     7321 1970-01-01 00:00:00.000000 dlt-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.2.8a0/LICENSE.txt
+-rw-r--r--   0        0        0     4214 2023-04-30 21:17:44.388805 dlt-0.2.8a0/README.md
+-rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.2.8a0/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.2.8a0/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    15909 2023-05-07 23:03:04.659469 dlt-0.2.8a0/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3858 2023-05-07 23:03:04.659469 dlt-0.2.8a0/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    16665 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.2.8a0/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18832 2023-05-18 22:16:30.462767 dlt-0.2.8a0/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10489 2023-05-18 22:16:30.462767 dlt-0.2.8a0/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9422 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4510 2023-05-18 22:16:30.462767 dlt-0.2.8a0/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-04-22 20:26:30.632198 dlt-0.2.8a0/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     3757 2023-04-30 21:17:44.388805 dlt-0.2.8a0/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.2.8a0/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      428 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     4243 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3469 2023-05-07 23:03:04.659469 dlt-0.2.8a0/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     5884 2023-04-22 20:26:30.632198 dlt-0.2.8a0/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.2.8a0/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      306 2023-05-07 23:03:04.659469 dlt-0.2.8a0/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0     1108 2023-04-26 11:34:23.292768 dlt-0.2.8a0/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.2.8a0/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.2.8a0/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.2.8a0/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     9441 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1108 2023-05-07 23:03:04.659469 dlt-0.2.8a0/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0     5237 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    17262 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0     1176 2023-05-07 23:03:04.659469 dlt-0.2.8a0/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.2.8a0/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0    13108 2023-05-07 23:03:04.659469 dlt-0.2.8a0/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     5521 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     2792 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1798 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.2.8a0/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0      556 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/configuration/specs/load_volume_configuration.py
+-rw-r--r--   0        0        0      417 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/configuration/specs/normalize_volume_configuration.py
+-rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.2.8a0/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0      944 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/configuration/specs/schema_volume_configuration.py
+-rw-r--r--   0        0        0     6026 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.2.8a0/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     5893 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2395 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0       97 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.2.8a0/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    10682 2023-04-24 11:35:34.867759 dlt-0.2.8a0/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6121 2023-05-18 22:16:30.462767 dlt-0.2.8a0/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/git.py
+-rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.2.8a0/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.2.8a0/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.2.8a0/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.2.8a0/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.2.8a0/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.2.8a0/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.2.8a0/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    16937 2023-05-18 22:16:30.462767 dlt-0.2.8a0/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.2.8a0/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.2.8a0/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.2.8a0/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.2.8a0/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      508 2023-04-30 21:17:44.388805 dlt-0.2.8a0/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.2.8a0/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.2.8a0/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13441 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.2.8a0/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.2.8a0/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25175 2023-04-09 16:39:04.593180 dlt-0.2.8a0/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.2.8a0/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    23087 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0      410 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     2804 2023-04-03 18:50:36.893525 dlt-0.2.8a0/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    10891 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2685 2023-04-13 08:33:43.967587 dlt-0.2.8a0/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21806 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2414 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8508 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.2.8a0/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.2.8a0/dlt/common/typing.py
+-rw-r--r--   0        0        0    12669 2023-05-18 22:16:41.982767 dlt-0.2.8a0/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.2.8a0/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    12347 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10342 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.2.8a0/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7008 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.2.8a0/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.2.8a0/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4975 2023-04-24 11:35:34.867759 dlt-0.2.8a0/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.2.8a0/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     4983 2023-04-05 08:03:40.638919 dlt-0.2.8a0/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    15625 2023-05-18 22:16:41.982767 dlt-0.2.8a0/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.2.8a0/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.2.8a0/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0     1232 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     6074 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.2.8a0/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.2.8a0/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     7110 2023-04-29 12:58:55.953219 dlt-0.2.8a0/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10101 2023-04-09 16:39:04.593180 dlt-0.2.8a0/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.2.8a0/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.8a0/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    22830 2023-05-18 22:16:30.462767 dlt-0.2.8a0/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12645 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     8449 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/extract/extract.py
+-rw-r--r--   0        0        0    14956 2023-05-18 22:16:30.462767 dlt-0.2.8a0/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    31567 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-04-22 20:26:30.632198 dlt-0.2.8a0/dlt/extract/schema.py
+-rw-r--r--   0        0        0    34195 2023-05-18 22:16:30.462767 dlt-0.2.8a0/dlt/extract/source.py
+-rw-r--r--   0        0        0     4350 2023-04-22 20:26:30.632198 dlt-0.2.8a0/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.2.8a0/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.2.8a0/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0      267 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/helpers/airflow.py
+-rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.2.8a0/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2490 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/helpers/pandas.py
+-rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.2.8a0/dlt/helpers/parquet.py
+-rw-r--r--   0        0        0    13371 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/helpers/streamlit.py
+-rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.2.8a0/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1019 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.2.8a0/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    19928 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.2.8a0/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1098 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.8a0/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    16576 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0     1880 2023-03-23 14:48:32.571618 dlt-0.2.8a0/dlt/pipeline/README.md
+-rw-r--r--   0        0        0    13138 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      363 2023-05-18 22:16:30.462767 dlt-0.2.8a0/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.2.8a0/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     2891 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8764 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.2.8a0/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    56518 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.2.8a0/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4200 2023-04-10 08:12:53.769595 dlt-0.2.8a0/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.2.8a0/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4563 2023-04-03 18:50:36.903525 dlt-0.2.8a0/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.2.8a0/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.2.8a0/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.8a0/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.2.8a0/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.2.8a0/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.2.8a0/dlt/sources/credentials.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.8a0/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.2.8a0/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0     9106 2023-05-14 20:33:31.539348 dlt-0.2.8a0/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.2.8a0/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.2.8a0/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.2.8a0/dlt/version.py
+-rw-r--r--   0        0        0     4056 2023-05-18 22:16:41.992767 dlt-0.2.8a0/pyproject.toml
+-rw-r--r--   0        0        0     7371 1970-01-01 00:00:00.000000 dlt-0.2.8a0/setup.py
+-rw-r--r--   0        0        0     7323 1970-01-01 00:00:00.000000 dlt-0.2.8a0/PKG-INFO
```

### Comparing `dlt-0.2.8/LICENSE.txt` & `dlt-0.2.8a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/README.md` & `dlt-0.2.8a0/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/__init__.py` & `dlt-0.2.8a0/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/cli/_dlt.py` & `dlt-0.2.8a0/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/cli/config_toml_writer.py` & `dlt-0.2.8a0/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/cli/deploy_command.py` & `dlt-0.2.8a0/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/cli/echo.py` & `dlt-0.2.8a0/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/cli/init_command.py` & `dlt-0.2.8a0/dlt/cli/init_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 from dlt.common import git
 from dlt.common.configuration.paths import get_dlt_settings_dir, make_dlt_settings_path
 from dlt.common.configuration.specs import known_sections
 from dlt.common.configuration.providers import CONFIG_TOML, SECRETS_TOML, ConfigTomlProvider, SecretsTomlProvider
 from dlt.common.normalizers import default_normalizers, import_normalizers
 from dlt.common.pipeline import get_dlt_repos_dir
-from dlt.common.source import _SOURCES
 from dlt.version import DLT_PKG_NAME, __version__
 from dlt.common.destination.reference import DestinationReference
 from dlt.common.reflection.utils import rewrite_python_script
 from dlt.common.schema.exceptions import InvalidSchemaName
 from dlt.common.storages.file_storage import FileStorage
 
+from dlt.extract.decorators import _SOURCES
 import dlt.reflection.names as n
 from dlt.reflection.script_inspector import inspect_pipeline_script, load_script_module
 
 from dlt.cli import echo as fmt, pipeline_files as files_ops, source_detection
 from dlt.cli import utils
 from dlt.cli.config_toml_writer import WritableConfigValue, write_values
 from dlt.cli.pipeline_files import PipelineFiles, TPipelineFileEntry, TPipelineFileIndex
```

### Comparing `dlt-0.2.8/dlt/cli/pipeline_command.py` & `dlt-0.2.8a0/dlt/cli/pipeline_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import yaml
 from typing import Any
 import dlt
 from dlt.cli.exceptions import CliCommandException
 
 from dlt.common import json
-from dlt.common.pipeline import resource_state, get_dlt_pipelines_dir, TSourceState
+from dlt.common.pipeline import _resource_state, get_dlt_pipelines_dir, TSourceState
 from dlt.common.destination.reference import TDestinationReferenceArg
 from dlt.common.runners import Venv
 from dlt.common.runners.stdout import iter_stdout
 from dlt.common.schema.utils import group_tables_by_resource, remove_defaults
 from dlt.common.storages.file_storage import FileStorage
 from dlt.common.typing import DictStrAny
 from dlt.pipeline.helpers import DropCommand
@@ -93,16 +93,16 @@
                 schema = p.schemas[schema_name]
                 data_tables = {t["name"]: t for t in schema.data_tables()}
                 for resource_name, tables in group_tables_by_resource(data_tables).items():
                     res_state_slots = 0
                     if sources_state:
                         source_state = next(iter(sources_state.items()))[1] if is_single_schema else sources_state.get(schema_name)
                         if source_state:
-                            resource_state_ = resource_state(resource_name, source_state)
-                            res_state_slots = len(resource_state_)
+                            resource_state = _resource_state(resource_name, source_state)
+                            res_state_slots = len(resource_state)
                     fmt.echo("%s with %s table(s) and %s resource state slot(s)" % (fmt.bold(resource_name), fmt.bold(str(len(tables))), fmt.bold(str(res_state_slots))))
         fmt.echo()
         fmt.echo("Working dir content:")
         extracted_files = p.list_extracted_resources()
         if extracted_files:
             fmt.echo("Has %s extracted files ready to be normalized" % fmt.bold(str(len(extracted_files))))
         norm_packages = p.list_normalized_load_packages()
```

### Comparing `dlt-0.2.8/dlt/cli/pipeline_files.py` & `dlt-0.2.8a0/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/cli/source_detection.py` & `dlt-0.2.8a0/dlt/cli/source_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from astunparse import unparse
 from typing import Dict, Tuple, Set, List
 
 from dlt.common.configuration import is_secret_hint
 from dlt.common.configuration.specs import BaseConfiguration
 from dlt.common.reflection.utils import creates_func_def_name_node
 from dlt.common.typing import is_optional_type
-from dlt.common.source import SourceInfo
 
 from dlt.cli.config_toml_writer import WritableConfigValue
 from dlt.cli.exceptions import CliCommandException
+from dlt.extract.decorators import SourceInfo
 from dlt.reflection.script_visitor import PipelineScriptVisitor
 
 
 def find_call_arguments_to_replace(visitor: PipelineScriptVisitor, replace_nodes: List[Tuple[str, str]], init_script_name: str) -> List[Tuple[ast.AST, ast.AST]]:
     # the input tuple (call argument name, replacement value)
     # the returned tuple (node, replacement value, node type)
     transformed_nodes: List[Tuple[ast.AST, ast.AST]] = []
```

### Comparing `dlt-0.2.8/dlt/cli/telemetry_command.py` & `dlt-0.2.8a0/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/cli/utils.py` & `dlt-0.2.8a0/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/arithmetics.py` & `dlt-0.2.8a0/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/accessors.py` & `dlt-0.2.8a0/dlt/common/configuration/accessors.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,19 +22,14 @@
         if value is None:
             raise ConfigFieldMissingException("Any", {field: traces})
         if isinstance(value, str):
             return auto_cast(value)
         else:
             return value
 
-    def __setitem__(self, field: str, value: Any) -> None:
-        sections = field.split(".")
-        key = sections.pop()
-        self.writable_provider.set_value(key, value, None, *sections)
-
     def get(self, field: str, expected_type: Type[TConfigAny] = None) -> TConfigAny:
         value: TConfigAny
         value, _ = self._get_value(field, expected_type)
         if value is None:
             return None
         # cast to required type
         if expected_type:
@@ -48,19 +43,14 @@
         pass
 
     @property
     @abc.abstractmethod
     def default_type(self) -> AnyType:
         pass
 
-    @property
-    @abc.abstractmethod
-    def writable_provider(self) -> ConfigProvider:
-        pass
-
     def _get_providers_from_context(self) -> Sequence[ConfigProvider]:
         return Container()[ConfigProvidersContext].providers
 
     def _get_value(self, field: str, type_hint: Type[Any] = None) -> Tuple[Any, List[LookupTrace]]:
         # get default hint type, in case of dlt.secrets it it TSecretValue
         type_hint = type_hint or self.default_type
         # split field into sections and a key
@@ -93,19 +83,14 @@
         """Return a list of config providers, in lookup order"""
         return [p for p in self._get_providers_from_context()]
 
     @property
     def default_type(self) -> AnyType:
         return AnyType
 
-    @property
-    def writable_provider(self) -> ConfigProvider:
-        """find first writable provider that does not support secrets - should be config.toml"""
-        return next(p for p in self._get_providers_from_context() if p.is_writable and not p.supports_secrets)
-
     value: ClassVar[None] = ConfigValue
     "A placeholder that tells dlt to replace it with actual config value during the call to a source or resource decorated function."
 
 
 class _SecretsAccessor(_Accessor):
     """Provides direct access to secrets."""
 
@@ -114,19 +99,14 @@
         """Return a list of config providers that can hold secrets, in lookup order"""
         return [p for p in self._get_providers_from_context() if p.supports_secrets]
 
     @property
     def default_type(self) -> AnyType:
         return TSecretValue
 
-    @property
-    def writable_provider(self) -> ConfigProvider:
-        """find first writable provider that supports secrets - should be secrets.toml"""
-        return next(p for p in self._get_providers_from_context() if p.is_writable and p.supports_secrets)
-
     value: ClassVar[None] = ConfigValue
     "A placeholder that tells dlt to replace it with actual secret during the call to a source or resource decorated function."
 
 
 config = _ConfigAccessor()
 """Dictionary-like access to all config values to dlt"""
```

### Comparing `dlt-0.2.8/dlt/common/configuration/container.py` & `dlt-0.2.8a0/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/exceptions.py` & `dlt-0.2.8a0/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/inject.py` & `dlt-0.2.8a0/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/paths.py` & `dlt-0.2.8a0/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/providers/airflow.py` & `dlt-0.2.8a0/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/providers/context.py` & `dlt-0.2.8a0/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/providers/dictionary.py` & `dlt-0.2.8a0/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/providers/environ.py` & `dlt-0.2.8a0/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.2.8a0/dlt/common/configuration/providers/google_secrets.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,15 +134,44 @@
     def _update_from_vault(self, full_key: str, key: str, hint: type, pipeline_name: str, sections: Tuple[str, ...]) -> None:
         if full_key in self._vault_lookups:
             return
         # print(f"tries '{key}' {pipeline_name} | {sections} at '{full_key}'")
         secret = self._look_vault(full_key, hint)
         self._vault_lookups[full_key] = pendulum.now()
         if secret is not None:
-            self.set_value(key, auto_cast(secret), pipeline_name, *sections)
+            self._add_node(secret, key, pipeline_name, sections)
+
+    def _add_node(self, secret: str, key: str, pipeline_name: str, sections: Tuple[str, ...]) -> None:
+        if pipeline_name:
+            sections = (pipeline_name, ) + sections
+
+        doc: Any = auto_cast(secret)
+        if isinstance(doc, TOMLContainer):
+            if key is None:
+                self._toml = doc
+            else:
+                # always update the top document
+                update_dict_nested(self._toml, doc)
+        else:
+            if key is None:
+                raise ValueError("dlt_secrets_toml must contain toml document")
+
+            master: TOMLContainer
+            # descend from root, create tables if necessary
+            master = self._toml
+            for k in sections:
+                if not isinstance(master, dict):
+                    raise KeyError(k)
+                if k not in master:
+                    master[k] = tomlkit.table()
+                master = master[k]  # type: ignore
+            if isinstance(doc, dict):
+                update_dict_nested(master[key], doc)  # type: ignore
+            else:
+                master[key] = doc
 
     @property
     def is_empty(self) -> bool:
         return False
 
     # def _verify_secret_access(self) -> None:
     #     try:
```

### Comparing `dlt-0.2.8/dlt/common/configuration/providers/provider.py` & `dlt-0.2.8a0/dlt/common/configuration/providers/provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 
 class ConfigProvider(abc.ABC):
 
     @abc.abstractmethod
     def get_value(self, key: str, hint: Type[Any], pipeline_name: str, *sections: str) -> Tuple[Optional[Any], str]:
         pass
 
-    def set_value(self, key: str, value: Any, pipeline_name: str, *sections: str) -> None:
-        raise NotImplementedError()
-
     @property
     @abc.abstractmethod
     def supports_secrets(self) -> bool:
         pass
 
     @property
     @abc.abstractmethod
@@ -28,17 +25,14 @@
     def name(self) -> str:
         pass
 
     @property
     def is_empty(self) -> bool:
         return False
 
-    @property
-    def is_writable(self) -> bool:
-        return False
 
 
 def get_key_name(key: str, separator: str, /, *sections: str) -> str:
     if sections:
         sections = filter(lambda x: bool(x), sections)  # type: ignore
         env_key = separator.join((*sections, key))
     else:
```

### Comparing `dlt-0.2.8/dlt/common/configuration/providers/toml.py` & `dlt-0.2.8a0/dlt/common/configuration/providers/toml.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,43 +32,14 @@
                     raise KeyError(k)
                 node = node[k]
             rv = node.unwrap() if isinstance(node, (TOMLContainer, TOMLItem)) else node
             return rv, full_key
         except KeyError:
             return None, full_key
 
-    def set_value(self, key: str, value: Any, pipeline_name: str, *sections: str) -> None:
-        if pipeline_name:
-            sections = (pipeline_name, ) + sections
-
-        if isinstance(value, TOMLContainer):
-            if key is None:
-                self._toml = value
-            else:
-                # always update the top document
-                # TODO: verify that value contains only the elements under key
-                update_dict_nested(self._toml, value)
-        else:
-            if key is None:
-                raise ValueError("dlt_secrets_toml must contain toml document")
-
-            master: TOMLContainer
-            # descend from root, create tables if necessary
-            master = self._toml
-            for k in sections:
-                if not isinstance(master, dict):
-                    raise KeyError(k)
-                if k not in master:
-                    master[k] = tomlkit.table()
-                master = master[k]  # type: ignore
-            if isinstance(value, dict) and isinstance(master.get(key), dict):
-                update_dict_nested(master[key], value)  # type: ignore
-            else:
-                master[key] = value
-
     @property
     def supports_sections(self) -> bool:
         return True
 
     @property
     def is_empty(self) -> bool:
         return len(self._toml.body) == 0
@@ -135,17 +106,14 @@
     def name(self) -> str:
         return CONFIG_TOML
 
     @property
     def supports_secrets(self) -> bool:
         return False
 
-    @property
-    def is_writable(self) -> bool:
-        return True
 
 
 class SecretsTomlProvider(TomlFileProvider):
 
     def __init__(self, project_dir: str = None, add_global_config: bool = False) -> None:
         super().__init__(SECRETS_TOML, project_dir=project_dir, add_global_config=add_global_config)
 
@@ -153,18 +121,14 @@
     def name(self) -> str:
         return SECRETS_TOML
 
     @property
     def supports_secrets(self) -> bool:
         return True
 
-    @property
-    def is_writable(self) -> bool:
-        return True
-
 
 class TomlProviderReadException(ConfigProviderException):
     def __init__(self, provider_name: str, file_name: str, full_path: str, toml_exception: str) -> None:
         self.file_name = file_name
         self.full_path = full_path
         msg = f"A problem encountered when loading {provider_name} from {full_path}:\n"
         msg += toml_exception
```

### Comparing `dlt-0.2.8/dlt/common/configuration/resolve.py` & `dlt-0.2.8a0/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/specs/__init__.py` & `dlt-0.2.8a0/dlt/common/configuration/specs/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from .run_configuration import RunConfiguration  # noqa: F401
 from .base_configuration import BaseConfiguration, CredentialsConfiguration, CredentialsWithDefault, ContainerInjectableContext, extract_inner_hint, is_base_configuration_inner_hint, configspec  # noqa: F401
+from .normalize_volume_configuration import NormalizeVolumeConfiguration  # noqa: F401
+from .load_volume_configuration import LoadVolumeConfiguration  # noqa: F401
+from .schema_volume_configuration import SchemaVolumeConfiguration, TSchemaFileFormat  # noqa: F401
 from .config_section_context import ConfigSectionContext  # noqa: F401
 
 from .gcp_credentials import GcpServiceAccountCredentialsWithoutDefaults, GcpServiceAccountCredentials, GcpOAuthCredentialsWithoutDefaults, GcpOAuthCredentials, GcpCredentials  # noqa: F401
 from .connection_string_credentials import ConnectionStringCredentials  # noqa: F401
 from .api_credentials import OAuth2Credentials  # noqa: F401
```

### Comparing `dlt-0.2.8/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.2.8a0/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.2.8a0/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.2.8a0/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.2.8a0/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.2.8a0/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     database: str = None
     password: Optional[TSecretValue] = None
     username: str = None
     host: Optional[str] = None
     port: Optional[int] = None
     query: Optional[Dict[str, str]] = None
 
-    __config_gen_annotations__: ClassVar[List[str]] = ["port", "password", "host"]
+    __config_gen_annotations__: ClassVar[List[str]] = ["port"]
 
     def parse_native_representation(self, native_value: Any) -> None:
         if not isinstance(native_value, str):
             raise InvalidConnectionString(self.__class__, native_value, self.drivername)
         try:
             url = make_url(native_value)
             # update only values that are not None
```

### Comparing `dlt-0.2.8/dlt/common/configuration/specs/exceptions.py` & `dlt-0.2.8a0/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.2.8a0/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/specs/known_sections.py` & `dlt-0.2.8a0/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.2.8a0/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/configuration/utils.py` & `dlt-0.2.8a0/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/data_types/type_helpers.py` & `dlt-0.2.8a0/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/data_writers/buffered.py` & `dlt-0.2.8a0/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/data_writers/escape.py` & `dlt-0.2.8a0/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/data_writers/exceptions.py` & `dlt-0.2.8a0/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/data_writers/writers.py` & `dlt-0.2.8a0/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/destination/capabilities.py` & `dlt-0.2.8a0/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/destination/reference.py` & `dlt-0.2.8a0/dlt/common/destination/reference.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/exceptions.py` & `dlt-0.2.8a0/dlt/common/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,17 +150,11 @@
         else:
             msg = "The resource you called requested the access to pipeline state but no pipeline is active right now."
         msg += " Call dlt.pipeline(...) before you call the @dlt.source or  @dlt.resource decorated function."
         self.source_name = source_name
         super().__init__(None, msg)
 
 
-class ResourceNameNotAvailable(PipelineException):
-    def __init__(self) -> None:
-        super().__init__(None,
-            "A resource state was requested but no resource marked callable was found in the call stack. Resource state may be only requested from @dlt.resource decorated function or with explicit resource name.")
-
-
 class SourceSectionNotAvailable(PipelineException):
     def __init__(self) -> None:
         msg = "Access to state was requested without source section active. State should be requested from within the @dlt.source and @dlt.resource decorated function."
         super().__init__(None, msg)
```

### Comparing `dlt-0.2.8/dlt/common/git.py` & `dlt-0.2.8a0/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/json/__init__.py` & `dlt-0.2.8a0/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/json/_orjson.py` & `dlt-0.2.8a0/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/json/_simplejson.py` & `dlt-0.2.8a0/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/jsonpath.py` & `dlt-0.2.8a0/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/normalizers/configuration.py` & `dlt-0.2.8a0/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/normalizers/json/__init__.py` & `dlt-0.2.8a0/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/normalizers/json/relational.py` & `dlt-0.2.8a0/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/normalizers/naming/direct.py` & `dlt-0.2.8a0/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.2.8a0/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.2.8a0/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/normalizers/naming/naming.py` & `dlt-0.2.8a0/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.2.8a0/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/normalizers/utils.py` & `dlt-0.2.8a0/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/pipeline.py` & `dlt-0.2.8a0/dlt/common/pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import os
 import datetime  # noqa: 251
 import humanize
-import inspect
 import contextlib
 from typing import Any, Callable, ClassVar, Dict, List, NamedTuple, Optional, Protocol, Sequence, TYPE_CHECKING, Tuple, TypedDict
 
-from dlt.common import pendulum, logger
+from dlt.common import pendulum
 from dlt.common.configuration import configspec
 from dlt.common.configuration import known_sections
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.exceptions import ContextDefaultCannotBeCreated
 from dlt.common.configuration.specs import ContainerInjectableContext
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.configuration.paths import get_dlt_data_dir
 from dlt.common.configuration.specs import RunConfiguration
 from dlt.common.destination.reference import DestinationReference, TDestinationReferenceArg
-from dlt.common.exceptions import DestinationHasFailedJobs, PipelineStateNotAvailable, ResourceNameNotAvailable, SourceSectionNotAvailable
+from dlt.common.exceptions import DestinationHasFailedJobs, PipelineStateNotAvailable, SourceSectionNotAvailable
 from dlt.common.schema import Schema
 from dlt.common.schema.typing import TColumnKey, TColumnSchema, TWriteDisposition
-from dlt.common.source import get_current_pipe_name
 from dlt.common.storages.load_storage import LoadPackageInfo
 from dlt.common.typing import DictStrAny, REPattern
 from dlt.common.jsonpath import delete_matches, TAnyJsonPath
 
 
 class ExtractInfo(NamedTuple):
     """A tuple holding information on extracted data items. Returned by pipeline `extract` method."""
@@ -290,26 +288,46 @@
 
     # allow inspection of last returned full state
     _last_full_state = state
     return sources_state_
 
 
 def source_state() -> DictStrAny:
-    """Returns a dictionary with the source-scoped state. Source-scoped state may be shared across the resources of a particular source. Please avoid using source scoped state. Check
-    the `resource_state` function for resource-scoped state that is visible within particular resource. Dlt state is preserved across pipeline runs and may be used to implement incremental loads.
+    """Returns a dictionary with the source state. Such state is preserved across pipeline runs and may be used to implement incremental loads.
 
     ### Summary
-    The source state is a python dictionary-like object that is available within the `@dlt.source` and `@dlt.resource` decorated functions and may be read and written to.
+    The state is a python dictionary-like object that is available within the `@dlt.source` and `@dlt.resource` decorated functions and may be read and written to.
     The data within the state is loaded into destination together with any other extracted data and made automatically available to the source/resource extractor functions when they are run next time.
     When using the state:
     * The source state is scoped to a section of the source. The source section is set by default to the module name in which source function is defined.
     * If the `section` argument when decorating source function is not specified, all sources in the module will share the state
     * Any JSON-serializable values can be written and the read from the state. `dlt` dumps and restores instances of Python bytes, DateTime, Date and Decimal types.
     * The state available in the source decorated function is read only and any changes will be discarded.
     * The state available in the resource decorated function is writable and written values will be available on the next pipeline run
+
+    ### Example
+    The most typical use case for the state is to implement incremental load.
+    >>> @dlt.resource(write_disposition="append")
+    >>> def players_games(chess_url, players, start_month=None, end_month=None):
+    >>>     checked_archives = dlt.current.state().setdefault("archives", [])
+    >>>     archives = players_archives(chess_url, players)
+    >>>     for url in archives:
+    >>>         if url in checked_archives:
+    >>>             print(f"skipping archive {url}")
+    >>>             continue
+    >>>         else:
+    >>>             print(f"getting archive {url}")
+    >>>             checked_archives.append(url)
+    >>>         # get the filtered archive
+    >>>         r = requests.get(url)
+    >>>         r.raise_for_status()
+    >>>         yield r.json().get("games", [])
+
+    Here we store all the urls with game archives in the state and we skip loading them on next run. The archives are immutable. The state will grow with the coming months (and more players).
+    Up to few thousand archives we should be good though.
     """
     global _last_full_state
 
     container = Container()
 
     # get the source name from the section context
     source_section: str = None
@@ -337,64 +355,19 @@
     """Remove one or more key from the source state.
     The `key` can be any number of keys and/or json paths to be removed.
     """
     state_ = source_state() if source_state_ is None else source_state_
     delete_matches(key, state_)
 
 
-def resource_state(resource_name: str = None, source_state_: Optional[DictStrAny] = None, /) -> DictStrAny:
-    """Returns a dictionary with the resource-scoped state. Resource-scoped state is visible only to resource requesting the access. Dlt state is preserved across pipeline runs and may be used to implement incremental loads.
-
-    Note that this function accepts the resource name as optional argument. There are rare cases when `dlt` is not able to resolve resource name due to requesting function
-    working in different thread than the main. You'll need to pass the name explicitly when you request resource_state from async functions or functions decorated with @defer.
-
-    ### Summary
-    The resource state is a python dictionary-like object that is available within the `@dlt.resource` decorated functions and may be read and written to.
-    The data within the state is loaded into destination together with any other extracted data and made automatically available to the source/resource extractor functions when they are run next time.
-    When using the state:
-    * The resource state is scoped to a particular resource requesting it.
-    * Any JSON-serializable values can be written and the read from the state. `dlt` dumps and restores instances of Python bytes, DateTime, Date and Decimal types.
-    * The state available in the resource decorated function is writable and written values will be available on the next pipeline run
-
-    ### Example
-    The most typical use case for the state is to implement incremental load.
-    >>> @dlt.resource(write_disposition="append")
-    >>> def players_games(chess_url, players, start_month=None, end_month=None):
-    >>>     checked_archives = dlt.current.resource_state().setdefault("archives", [])
-    >>>     archives = players_archives(chess_url, players)
-    >>>     for url in archives:
-    >>>         if url in checked_archives:
-    >>>             print(f"skipping archive {url}")
-    >>>             continue
-    >>>         else:
-    >>>             print(f"getting archive {url}")
-    >>>             checked_archives.append(url)
-    >>>         # get the filtered archive
-    >>>         r = requests.get(url)
-    >>>         r.raise_for_status()
-    >>>         yield r.json().get("games", [])
-
-    Here we store all the urls with game archives in the state and we skip loading them on next run. The archives are immutable. The state will grow with the coming months (and more players).
-    Up to few thousand archives we should be good though.
-    Args:
-        resource_name (str, optional): forces to use state for a resource with this name. Defaults to None.
-        source_state_ (Optional[DictStrAny], optional): Alternative source state. Defaults to None.
-
-    Raises:
-        ResourceNameNotAvailable: Raise if used outside of resource context or from a different thread than main
-
-    Returns:
-        DictStrAny: State dictionary
+def _resource_state(resource_name: str, source_state_: Optional[DictStrAny] = None, /) -> DictStrAny:
+    """Alpha version of the resource state, the signature will change.
+    Returns resource-scoped state.
     """
     state_ = source_state() if source_state_ is None else source_state_
-    # backtrace to find the shallowest resource
-    if not resource_name:
-        resource_name = get_current_pipe_name()
-    if not resource_name:
-        raise ResourceNameNotAvailable()
     return state_.setdefault('resources', {}).setdefault(resource_name, {})  # type: ignore
 
 
 def _reset_resource_state(resource_name: str, source_state_: Optional[DictStrAny] = None, /) -> None:
     """Alpha version of the resource state. Resets the resource state
 
     Args:
```

### Comparing `dlt-0.2.8/dlt/common/reflection/spec.py` & `dlt-0.2.8a0/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/reflection/utils.py` & `dlt-0.2.8a0/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runners/pool_runner.py` & `dlt-0.2.8a0/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runners/runnable.py` & `dlt-0.2.8a0/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runners/stdout.py` & `dlt-0.2.8a0/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runners/synth_pickle.py` & `dlt-0.2.8a0/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runners/venv.py` & `dlt-0.2.8a0/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runtime/collector.py` & `dlt-0.2.8a0/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runtime/exec_info.py` & `dlt-0.2.8a0/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runtime/init.py` & `dlt-0.2.8a0/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runtime/logger.py` & `dlt-0.2.8a0/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runtime/prometheus.py` & `dlt-0.2.8a0/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runtime/segment.py` & `dlt-0.2.8a0/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runtime/sentry.py` & `dlt-0.2.8a0/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runtime/signals.py` & `dlt-0.2.8a0/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runtime/slack.py` & `dlt-0.2.8a0/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/runtime/telemetry.py` & `dlt-0.2.8a0/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/schema/detections.py` & `dlt-0.2.8a0/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/schema/exceptions.py` & `dlt-0.2.8a0/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/schema/schema.py` & `dlt-0.2.8a0/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/schema/typing.py` & `dlt-0.2.8a0/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/schema/utils.py` & `dlt-0.2.8a0/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/storages/configuration.py` & `dlt-0.2.8a0/dlt/common/configuration/specs/schema_volume_configuration.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,19 @@
-from typing import TYPE_CHECKING, Literal, Optional, get_args
+from typing import Optional, Literal, TYPE_CHECKING, get_args
 
-from dlt.common.configuration.specs import BaseConfiguration, configspec
+from dlt.common.configuration.specs.base_configuration import BaseConfiguration, configspec
 
 TSchemaFileFormat = Literal["json", "yaml"]
 SchemaFileExtensions = get_args(TSchemaFileFormat)
 
 
 @configspec(init=True)
-class SchemaStorageConfiguration(BaseConfiguration):
+class SchemaVolumeConfiguration(BaseConfiguration):
     schema_volume_path: str = None  # path to volume with default schemas
     import_schema_path: Optional[str] = None  # import schema from external location
     export_schema_path: Optional[str] = None  # export schema to external location
     external_schema_format: TSchemaFileFormat = "yaml"  # format in which to expect external schema
     external_schema_format_remove_defaults: bool = True  # remove default values when exporting schema
 
     if TYPE_CHECKING:
         def __init__(self, schema_volume_path: str = None, import_schema_path: str = None, export_schema_path: str = None) -> None:
             ...
-
-
-@configspec(init=True)
-class NormalizeStorageConfiguration(BaseConfiguration):
-    normalize_volume_path: str = None  # path to volume where normalized loader files will be stored
-
-    if TYPE_CHECKING:
-        def __init__(self, normalize_volume_path: str = None) -> None:
-            ...
-
-
-@configspec(init=True)
-class LoadStorageConfiguration(BaseConfiguration):
-    load_volume_path: str = None  # path to volume where files to be loaded to analytical storage are stored
-    delete_completed_jobs: bool = False  # if set to true the folder with completed jobs will be deleted
-
-    if TYPE_CHECKING:
-        def __init__(self, load_volume_path: str = None, delete_completed_jobs: bool = None) -> None:
-            ...
```

### Comparing `dlt-0.2.8/dlt/common/storages/data_item_storage.py` & `dlt-0.2.8a0/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/storages/exceptions.py` & `dlt-0.2.8a0/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/storages/file_storage.py` & `dlt-0.2.8a0/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/storages/live_schema_storage.py` & `dlt-0.2.8a0/dlt/common/storages/live_schema_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Dict
 
 from dlt.common.schema.schema import Schema
-from dlt.common.configuration.accessors import config
 from dlt.common.storages.schema_storage import SchemaStorage
-from dlt.common.storages.configuration import SchemaStorageConfiguration
+from dlt.common.configuration.specs import SchemaVolumeConfiguration
+from dlt.common.configuration.accessors import config
 
 
 class LiveSchemaStorage(SchemaStorage):
 
-    def __init__(self, config: SchemaStorageConfiguration = config.value, makedirs: bool = False) -> None:
+    def __init__(self, config: SchemaVolumeConfiguration = config.value, makedirs: bool = False) -> None:
         self.live_schemas: Dict[str, Schema] = {}
         super().__init__(config, makedirs)
 
     def __getitem__(self, name: str) -> Schema:
         if name in self.live_schemas:
             schema = self.live_schemas[name]
         else:
```

### Comparing `dlt-0.2.8/dlt/common/storages/load_storage.py` & `dlt-0.2.8a0/dlt/common/storages/load_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 from dlt.common import json, pendulum
 from dlt.common.configuration import known_sections
 from dlt.common.configuration.inject import with_config
 from dlt.common.typing import DictStrAny, StrAny
 from dlt.common.storages.file_storage import FileStorage
 from dlt.common.data_writers import TLoaderFileFormat, DataWriter
+from dlt.common.configuration.specs import LoadVolumeConfiguration
 from dlt.common.configuration.accessors import config
 from dlt.common.exceptions import TerminalValueError
 from dlt.common.schema import Schema, TSchemaTables, TTableSchemaColumns
-from dlt.common.storages.configuration import LoadStorageConfiguration
 from dlt.common.storages.versioned_storage import VersionedStorage
 from dlt.common.storages.data_item_storage import DataItemStorage
 from dlt.common.storages.exceptions import JobWithUnsupportedWriterException, LoadPackageNotFound
 from dlt.common.utils import flatten_list_or_items
 
 
 # folders to manage load jobs in a single load package
@@ -136,21 +136,21 @@
     SCHEMA_UPDATES_FILE_NAME = "schema_updates.json"  # updates to the tables in schema created by normalizer
     APPLIED_SCHEMA_UPDATES_FILE_NAME = "applied_" + "schema_updates.json"  # updates applied to the destination
     SCHEMA_FILE_NAME = "schema.json"  # package schema
     PACKAGE_COMPLETED_FILE_NAME = "package_completed.json"  # completed package marker file, currently only to store data with os.stat
 
     ALL_SUPPORTED_FILE_FORMATS: Set[TLoaderFileFormat] = set(get_args(TLoaderFileFormat))
 
-    @with_config(spec=LoadStorageConfiguration, sections=(known_sections.LOAD,))
+    @with_config(spec=LoadVolumeConfiguration, sections=(known_sections.LOAD,))
     def __init__(
         self,
         is_owner: bool,
         preferred_file_format: TLoaderFileFormat,
         supported_file_formats: Iterable[TLoaderFileFormat],
-        config: LoadStorageConfiguration = config.value
+        config: LoadVolumeConfiguration = config.value
     ) -> None:
         if not LoadStorage.ALL_SUPPORTED_FILE_FORMATS.issuperset(supported_file_formats):
             raise TerminalValueError(supported_file_formats)
         if preferred_file_format not in supported_file_formats:
             raise TerminalValueError(preferred_file_format)
         self.supported_file_formats = supported_file_formats
         self.config = config
```

### Comparing `dlt-0.2.8/dlt/common/storages/normalize_storage.py` & `dlt-0.2.8a0/dlt/common/storages/normalize_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from typing import ClassVar, Sequence, NamedTuple
+from typing import ClassVar, Sequence, NamedTuple, overload
 from itertools import groupby
 from pathlib import Path
 
-from dlt.common.configuration import with_config, known_sections
-from dlt.common.configuration.accessors import config
 from dlt.common.storages.file_storage import FileStorage
-from dlt.common.storages.configuration import NormalizeStorageConfiguration
+from dlt.common.configuration import with_config, known_sections
+from dlt.common.configuration.specs import NormalizeVolumeConfiguration
 from dlt.common.storages.versioned_storage import VersionedStorage
+from dlt.common.configuration.accessors import config
+
 
 class TParsedNormalizeFileName(NamedTuple):
     schema_name: str
     table_name: str
     file_id: str
 
 
 class NormalizeStorage(VersionedStorage):
 
     STORAGE_VERSION: ClassVar[str] = "1.0.0"
     EXTRACTED_FOLDER: ClassVar[str] = "extracted"  # folder within the volume where extracted files to be normalized are stored
 
-    @with_config(spec=NormalizeStorageConfiguration, sections=(known_sections.NORMALIZE,))
-    def __init__(self, is_owner: bool, config: NormalizeStorageConfiguration = config.value) -> None:
+    @with_config(spec=NormalizeVolumeConfiguration, sections=(known_sections.NORMALIZE,))
+    def __init__(self, is_owner: bool, config: NormalizeVolumeConfiguration = config.value) -> None:
         super().__init__(NormalizeStorage.STORAGE_VERSION, is_owner, FileStorage(config.normalize_volume_path, "t", makedirs=is_owner))
         self.config = config
         if is_owner:
             self.initialize_storage()
 
     def initialize_storage(self) -> None:
         self.storage.create_folder(NormalizeStorage.EXTRACTED_FOLDER, exists_ok=True)
```

### Comparing `dlt-0.2.8/dlt/common/storages/schema_storage.py` & `dlt-0.2.8a0/dlt/common/storages/schema_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import yaml
-from typing import Iterator, List, Mapping, Tuple
+from typing import Iterator, List, Mapping, Tuple, overload
 
 from dlt.common import json, logger
 from dlt.common.configuration import with_config
+from dlt.common.configuration.specs import SchemaVolumeConfiguration, TSchemaFileFormat
+from dlt.common.configuration.specs.schema_volume_configuration import SchemaFileExtensions
 from dlt.common.configuration.accessors import config
-from dlt.common.storages.configuration import SchemaStorageConfiguration, TSchemaFileFormat, SchemaFileExtensions
 from dlt.common.storages.file_storage import FileStorage
 from dlt.common.schema import Schema, verify_schema_hash
 from dlt.common.typing import DictStrAny
 
 from dlt.common.storages.exceptions import InStorageSchemaModified, SchemaNotFoundError
 
 
 class SchemaStorage(Mapping[str, Schema]):
 
     SCHEMA_FILE_NAME = "schema.%s"
     NAMED_SCHEMA_FILE_PATTERN = f"%s.{SCHEMA_FILE_NAME}"
 
-    @with_config(spec=SchemaStorageConfiguration, sections=("schema",))
-    def __init__(self, config: SchemaStorageConfiguration = config.value, makedirs: bool = False) -> None:
+    @with_config(spec=SchemaVolumeConfiguration, sections=("schema",))
+    def __init__(self, config: SchemaVolumeConfiguration = config.value, makedirs: bool = False) -> None:
         self.config = config
         self.storage = FileStorage(config.schema_volume_path, makedirs=makedirs)
 
     def load_schema(self, name: str) -> Schema:
         # loads a schema from a store holding many schemas
         schema_file = self._file_name_in_store(name, "json")
         storage_schema: DictStrAny = None
```

### Comparing `dlt-0.2.8/dlt/common/storages/versioned_storage.py` & `dlt-0.2.8a0/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/time.py` & `dlt-0.2.8a0/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/typing.py` & `dlt-0.2.8a0/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/utils.py` & `dlt-0.2.8a0/dlt/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 
 def reveal_pseudo_secret(obfuscated_secret: str, pseudo_key: bytes) -> str:
     return bytes([_a ^ _b for _a, _b in zip(base64.b64decode(obfuscated_secret.encode("ascii"), validate=True), pseudo_key*250)]).decode("utf-8")
 
 
 def get_module_name(m: ModuleType) -> str:
     """Gets module name from module with a fallback for executing module __main__"""
-    if m.__name__ == "__main__" and hasattr(m, "__file__"):
+    if m.__name__ == "__main__":
         module_file = os.path.basename(m.__file__)
         module_name, _ = os.path.splitext(module_file)
         return module_name
     return m.__name__.split(".")[-1]
 
 
 def derives_from_class_of_name(o: object, name: str) -> bool:
```

### Comparing `dlt-0.2.8/dlt/common/validation.py` & `dlt-0.2.8a0/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/common/wei.py` & `dlt-0.2.8a0/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/bigquery/__init__.py` & `dlt-0.2.8a0/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/bigquery/bigquery.py` & `dlt-0.2.8a0/dlt/destinations/bigquery/bigquery.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/bigquery/sql_client.py` & `dlt-0.2.8a0/dlt/destinations/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/duckdb/__init__.py` & `dlt-0.2.8a0/dlt/destinations/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/duckdb/configuration.py` & `dlt-0.2.8a0/dlt/destinations/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/duckdb/duck.py` & `dlt-0.2.8a0/dlt/destinations/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/duckdb/sql_client.py` & `dlt-0.2.8a0/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/dummy/__init__.py` & `dlt-0.2.8a0/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/dummy/configuration.py` & `dlt-0.2.8a0/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/dummy/dummy.py` & `dlt-0.2.8a0/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/exceptions.py` & `dlt-0.2.8a0/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/insert_job_client.py` & `dlt-0.2.8a0/dlt/destinations/insert_job_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/job_client_impl.py` & `dlt-0.2.8a0/dlt/destinations/job_client_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/job_impl.py` & `dlt-0.2.8a0/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/postgres/__init__.py` & `dlt-0.2.8a0/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/postgres/configuration.py` & `dlt-0.2.8a0/dlt/destinations/postgres/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/postgres/postgres.py` & `dlt-0.2.8a0/dlt/destinations/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/postgres/sql_client.py` & `dlt-0.2.8a0/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/redshift/README.md` & `dlt-0.2.8a0/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/redshift/__init__.py` & `dlt-0.2.8a0/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/redshift/configuration.py` & `dlt-0.2.8a0/dlt/destinations/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/redshift/redshift.py` & `dlt-0.2.8a0/dlt/destinations/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/sql_client.py` & `dlt-0.2.8a0/dlt/destinations/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/sql_merge_job.py` & `dlt-0.2.8a0/dlt/destinations/sql_merge_job.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/destinations/typing.py` & `dlt-0.2.8a0/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/extract/decorators.py` & `dlt-0.2.8a0/dlt/extract/decorators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import os
 import inspect
 from types import ModuleType
 from functools import wraps
-from typing import TYPE_CHECKING, Any, Callable, ClassVar, Iterator, List, Optional, Tuple, Type, TypeVar, Union, cast, overload
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Dict, Iterator, List, NamedTuple, Optional, Tuple, Type, TypeVar, Union, cast, overload
 
 from dlt.common.configuration import with_config, get_fun_spec, known_sections, configspec
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.exceptions import ContextDefaultCannotBeCreated
 from dlt.common.configuration.resolve import inject_section
 from dlt.common.configuration.specs import BaseConfiguration, ContainerInjectableContext
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.exceptions import ArgumentsOverloadException
 from dlt.common.pipeline import PipelineContext
-from dlt.common.source import _SOURCES, SourceInfo
 from dlt.common.schema.schema import Schema
-from dlt.common.schema.typing import TColumnKey, TTableSchemaColumns, TWriteDisposition
+from dlt.common.schema.typing import TColumnKey, TColumnName, TTableSchemaColumns, TWriteDisposition
 from dlt.common.storages.exceptions import SchemaNotFoundError
 from dlt.common.storages.schema_storage import SchemaStorage
 from dlt.common.typing import AnyFun, ParamSpec, Concatenate, TDataItem, TDataItems
 from dlt.common.utils import get_callable_name, get_module_name, is_inner_callable
 from dlt.extract.exceptions import InvalidTransformerDataTypeGeneratorFunctionRequired, ResourceFunctionExpected, ResourceInnerCallableConfigWrapDisallowed, SourceDataIsNone, SourceIsAClassTypeError, SourceNotAFunction, SourceSchemaNotAvailable
 from dlt.extract.incremental import IncrementalResourceWrapper
 
@@ -34,14 +33,25 @@
 
     can_create_default: ClassVar[bool] = False
 
     if TYPE_CHECKING:
         def __init__(self, schema: Schema = None) -> None:
             ...
 
+
+class SourceInfo(NamedTuple):
+    """Runtime information on the source/resource"""
+    SPEC: Type[BaseConfiguration]
+    f: AnyFun
+    module: ModuleType
+
+
+_SOURCES: Dict[str, SourceInfo] = {}
+"""A registry of all the decorated sources and resources discovered when importing modules"""
+
 TSourceFunParams = ParamSpec("TSourceFunParams")
 TResourceFunParams = ParamSpec("TResourceFunParams")
 
 
 @overload
 def source(
     func: Callable[TSourceFunParams, Any],
@@ -210,14 +220,16 @@
     primary_key: TTableHintTemplate[TColumnKey] = None,
     merge_key: TTableHintTemplate[TColumnKey] = None,
     selected: bool = True,
     spec: Type[BaseConfiguration] = None
 ) -> Callable[[Callable[TResourceFunParams, Any]], DltResource]:
     ...
 
+
+
 @overload
 def resource(
     data: Union[List[Any], Tuple[Any], Iterator[Any]],
     /,
     name: str = None,
     table_name: TTableHintTemplate[str] = None,
     write_disposition: TTableHintTemplate[TWriteDisposition] = None,
@@ -354,123 +366,53 @@
         # we're called with parens.
         return decorator
 
     if callable(data):
         return decorator(data)
     else:
         # take name from the generator
-        source_section: str = None
         if inspect.isgenerator(data):
             name = name or get_callable_name(data)  # type: ignore
-            func_module = inspect.getmodule(data.gi_frame)
-            source_section = _get_source_section_name(func_module)
-
-        return make_resource(name, source_section, data)
+        return make_resource(name, None, data)
 
 
-@overload
-def transformer(
-    f: None = ...,
-    /,
-    data_from: TUnboundDltResource = DltResource.Empty,
-    name: str = None,
-    table_name: TTableHintTemplate[str] = None,
-    write_disposition: TTableHintTemplate[TWriteDisposition] = None,
-    columns: TTableHintTemplate[TTableSchemaColumns] = None,
-    primary_key: TTableHintTemplate[TColumnKey] = None,
-    merge_key: TTableHintTemplate[TColumnKey] = None,
-    selected: bool = True,
-    spec: Type[BaseConfiguration] = None
-) -> Callable[[Callable[Concatenate[TDataItem, TResourceFunParams], Any]], Callable[TResourceFunParams, DltResource]]:
-    ...
-
-@overload
 def transformer(
-    f: Callable[Concatenate[TDataItem, TResourceFunParams], Any],
-    /,
-    data_from: TUnboundDltResource = DltResource.Empty,
-    name: str = None,
-    table_name: TTableHintTemplate[str] = None,
-    write_disposition: TTableHintTemplate[TWriteDisposition] = None,
-    columns: TTableHintTemplate[TTableSchemaColumns] = None,
-    primary_key: TTableHintTemplate[TColumnKey] = None,
-    merge_key: TTableHintTemplate[TColumnKey] = None,
-    selected: bool = True,
-    spec: Type[BaseConfiguration] = None
-) -> Callable[TResourceFunParams, DltResource]:
-    ...
-
-def transformer(  # type: ignore
-    f: Optional[Callable[Concatenate[TDataItem, TResourceFunParams], Any]] = None,
-    /,
     data_from: TUnboundDltResource = DltResource.Empty,
     name: str = None,
     table_name: TTableHintTemplate[str] = None,
     write_disposition: TTableHintTemplate[TWriteDisposition] = None,
     columns: TTableHintTemplate[TTableSchemaColumns] = None,
     primary_key: TTableHintTemplate[TColumnKey] = None,
     merge_key: TTableHintTemplate[TColumnKey] = None,
     selected: bool = True,
     spec: Type[BaseConfiguration] = None
 ) -> Callable[[Callable[Concatenate[TDataItem, TResourceFunParams], Any]], Callable[TResourceFunParams, DltResource]]:
-    """A form of `dlt resource` that takes input from other resources via `data_from` argument in order to enrich or transform the data.
-
-    The decorated function `f` must take at least one argument of type TDataItems (a single item or list of items depending on the resource `data_from`). `dlt` will pass
-    metadata associated with the data item if argument with name `meta` is present. Otherwise, transformer function may take more arguments and be parametrized
-    like the resources.
-
-    You can bind the transformer early by specifying resource in `data_from` when the transformer is created or create dynamic bindings later with | operator
-    which is demonstrated in example below:
+    """A form of `dlt resource` that takes input from other resources in order to enrich or transform the data.
 
     ### Example
     >>> @dlt.resource
     >>> def players(title, chess_url=dlt.config.value):
     >>>     r = requests.get(f"{chess_url}titled/{title}")
     >>>     yield r.json()["players"]  # returns list of player names
     >>>
     >>> # this resource takes data from players and returns profiles
-    >>> @dlt.transformer(write_disposition="replace")
+    >>> @dlt.transformer(data_from=players, write_disposition="replace")
     >>> def player_profile(player: Any) -> Iterator[TDataItems]:
     >>>     r = requests.get(f"{chess_url}player/{player}")
     >>>     r.raise_for_status()
     >>>     yield r.json()
     >>>
-    >>> # pipes the data from players into player profile to produce a list of player profiles
-    >>> list(players("GM") | player_profile)
-
-    ### Args:
-        f: (Callable): a function taking minimum one argument of TDataItems type which will receive data yielded from `data_from` resource.
-
-        data_from (Callable | Any, optional): a resource that will send data to the decorated function `f`
-
-        name (str, optional): A name of the resource that by default also becomes the name of the table to which the data is loaded.
-        If not present, the name of the decorated function will be used.
-
-        table_name (TTableHintTemplate[str], optional): An table name, if different from `name`.
-        This argument also accepts a callable that is used to dynamically create tables for stream-like resources yielding many datatypes.
-
-        write_disposition (Literal["skip", "append", "replace", "merge"], optional): Controls how to write data to a table. `append` will always add new data at the end of the table. `replace` will replace existing data with new data. `skip` will prevent data from loading. "merge" will deduplicate and merge data based on "primary_key" and "merge_key" hints. Defaults to "append".
-        This argument also accepts a callable that is used to dynamically create tables for stream-like resources yielding many datatypes.
-
-        columns (Sequence[TColumnSchema], optional): A list of column schemas. Typed dictionary describing column names, data types, write disposition and performance hints that gives you full control over the created table schema.
-        This argument also accepts a callable that is used to dynamically create tables for stream-like resources yielding many datatypes.
+    >>> list(players("GM") | player_profile)  # pipes the data from players into player profile to produce a list of player profiles
 
-        primary_key (str | Sequence[str]): A column name or a list of column names that comprise a private key. Typically used with "merge" write disposition to deduplicate loaded data.
-        This argument also accepts a callable that is used to dynamically create tables for stream-like resources yielding many datatypes.
-
-        merge_key (str | Sequence[str]): A column name or a list of column names that define a merge key. Typically used with "merge" write disposition to remove overlapping data ranges ie. to keep a single record for a given day.
-        This argument also accepts a callable that is used to dynamically create tables for stream-like resources yielding many datatypes.
-
-        selected (bool, optional): When `True` `dlt pipeline` will extract and load this resource, if `False`, the resource will be ignored.
-
-        spec (Type[BaseConfiguration], optional): A specification of configuration and secret values required by the source.
     """
-    if isinstance(f, DltResource):
-        raise ValueError("Please pass `data_from=` argument as keyword argument. The only positional argument to transformer is the decorated function")
-
+    f: AnyFun = None
+    # if data_from is a function we are called without parens
+    if inspect.isfunction(data_from):
+        f = data_from
+        data_from = DltResource.Empty
     return resource(  # type: ignore
         f,
         name=name,
         table_name=table_name,
         write_disposition=write_disposition,
         columns=columns,
         primary_key=primary_key,
@@ -489,30 +431,56 @@
         if file:
             return SchemaStorage.load_schema_file(os.path.dirname(file), name)
     except SchemaNotFoundError:
         pass
     return None
 
 
+def _get_source_for_inner_function(f: AnyFun) -> Optional[SourceInfo]:
+    # find source function
+    parts = get_callable_name(f, "__qualname__").split(".")
+    parent_fun = ".".join(parts[:-2])
+    return _SOURCES.get(parent_fun)
+
+
 def _get_source_section_name(m: ModuleType) -> str:
-    if m is None:
-        return None
     if hasattr(m, "__source_name__"):
         return cast(str, m.__source_name__)
     return get_module_name(m)
 
 
 def get_source_schema() -> Schema:
     """When executed from the function decorated with @dlt.source, returns a writable source Schema"""
     try:
         return Container()[SourceSchemaInjectableContext].schema
     except ContextDefaultCannotBeCreated:
         raise SourceSchemaNotAvailable()
 
 
+# def with_retry(max_retries: int = 3, retry_sleep: float = 1.0) -> Callable[[Callable[_TFunParams, TBoundItem]], Callable[_TFunParams, TBoundItem]]:
+
+#     def decorator(f: Callable[_TFunParams, TBoundItem]) -> Callable[_TFunParams, TBoundItem]:
+
+#         def _wrap(*args: Any, **kwargs: Any) -> TBoundItem:
+#             attempts = 0
+#             while True:
+#                 try:
+#                     return f(*args, **kwargs)
+#                 except Exception as exc:
+#                     if attempts == max_retries:
+#                         raise
+#                     attempts += 1
+#                     logger.warning(f"Exception {exc} in iterator, retrying {attempts} / {max_retries}")
+#                     sleep(retry_sleep)
+
+#         return _wrap
+
+#     return decorator
+
+
 TBoundItems = TypeVar("TBoundItems", bound=TDataItems)
 TDeferred = Callable[[], TBoundItems]
 TDeferredFunParams = ParamSpec("TDeferredFunParams")
 
 
 def defer(f: Callable[TDeferredFunParams, TBoundItems]) -> Callable[TDeferredFunParams, TDeferred[TBoundItems]]:
```

### Comparing `dlt-0.2.8/dlt/extract/exceptions.py` & `dlt-0.2.8a0/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/extract/extract.py` & `dlt-0.2.8a0/dlt/extract/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 from dlt.common.pipeline import _reset_resource_state
 
 from dlt.common.runtime import signals
 from dlt.common.runtime.collector import Collector, NULL_COLLECTOR
 from dlt.common.utils import uniq_id
 from dlt.common.typing import TDataItems, TDataItem
 from dlt.common.schema import Schema, utils, TSchemaUpdate
-from dlt.common.storages import NormalizeStorageConfiguration, NormalizeStorage, DataItemStorage
-from dlt.common.configuration.specs import known_sections
+from dlt.common.storages import NormalizeStorage, DataItemStorage
+from dlt.common.configuration.specs import NormalizeVolumeConfiguration, known_sections
 
 from dlt.extract.decorators import SourceSchemaInjectableContext
 from dlt.extract.exceptions import DataItemRequiredForDynamicTableHints
 from dlt.extract.pipe import PipeIterator
 from dlt.extract.source import DltResource, DltSource
 from dlt.extract.typing import TableNameMeta
 
 
 class ExtractorStorage(DataItemStorage, NormalizeStorage):
     EXTRACT_FOLDER: ClassVar[str] = "extract"
 
-    def __init__(self, C: NormalizeStorageConfiguration) -> None:
+    def __init__(self, C: NormalizeVolumeConfiguration) -> None:
         # data item storage with jsonl with pua encoding
         super().__init__("puae-jsonl", True, C)
         self.storage.create_folder(ExtractorStorage.EXTRACT_FOLDER, exists_ok=True)
 
     def create_extract_id(self) -> str:
         extract_id = uniq_id()
         self.storage.create_folder(self._get_extract_path(extract_id))
```

### Comparing `dlt-0.2.8/dlt/extract/incremental.py` & `dlt-0.2.8a0/dlt/extract/incremental.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import dlt
 from dlt.common.json import json
 from dlt.common.jsonpath import compile_path, find_values, JSONPath
 from dlt.common.typing import TDataItem, TDataItems, TFun, extract_inner_type, is_optional_type
 from dlt.common.schema.typing import TColumnKey
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import BaseConfiguration
-from dlt.common.pipeline import resource_state
+from dlt.common.pipeline import _resource_state
 from dlt.common.utils import digest128
 from dlt.extract.exceptions import IncrementalUnboundError, PipeException
 from dlt.extract.pipe import Pipe
 from dlt.extract.utils import resolve_column_value
 from dlt.extract.typing import FilterItem, SupportsPipe, TTableHintTemplate
 from dlt.common import pendulum
 
@@ -141,15 +141,15 @@
                     'unique_hashes': []
                 }
             )
         return self._cached_state
 
     @staticmethod
     def _get_state(resource_name: str, cursor_path: str) -> IncrementalColumnState:
-        state: IncrementalColumnState = resource_state(resource_name).setdefault('incremental', {}).setdefault(cursor_path, {})
+        state: IncrementalColumnState = _resource_state(resource_name).setdefault('incremental', {}).setdefault(cursor_path, {})
         # if state params is empty
         return state
 
     @property
     def last_value(self) -> Optional[TCursorValue]:
         s = self.get_state()
         return s['last_value']  # type: ignore
```

### Comparing `dlt-0.2.8/dlt/extract/pipe.py` & `dlt-0.2.8a0/dlt/extract/pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from typing import Any, ContextManager, Optional, Sequence, Union, Callable, Iterable, Iterator, List, NamedTuple, Awaitable, Tuple, Type, TYPE_CHECKING
 
 from dlt.common import sleep
 from dlt.common.configuration import configspec
 from dlt.common.configuration.inject import with_config
 from dlt.common.configuration.specs import BaseConfiguration
 from dlt.common.exceptions import PipelineException
-from dlt.common.source import unset_current_pipe_name, set_current_pipe_name
 from dlt.common.typing import AnyFun, AnyType, TDataItems
 from dlt.common.utils import get_callable_name
 
 from dlt.extract.exceptions import CreatePipeException, DltSourceException, ExtractorException, InvalidResourceDataTypeFunctionNotAGenerator, InvalidStepFunctionArguments, InvalidTransformerGeneratorFunction, ParametrizedResourceUnbound, PipeException, PipeItemProcessingError, PipeNotBoundToData, ResourceExtractionError
 from dlt.extract.typing import DataItemWithMeta, ItemTransform, SupportsPipe, TPipedDataItems
 
 if TYPE_CHECKING:
@@ -548,38 +547,34 @@
                     raise PipeItemProcessingError(
                         pipe_item.pipe.name, f"Pipe item at step {pipe_item.step} was not fully evaluated and is of type {type(pipe_item.item).__name__}. This is internal error or you are yielding something weird from resources ie. functions or awaitables.")
                 # mypy not able to figure out that item was resolved
                 return pipe_item  # type: ignore
 
             # advance to next step
             step = pipe_item.pipe[pipe_item.step + 1]
+            assert callable(step)
             try:
-                set_current_pipe_name(pipe_item.pipe.name)
                 next_meta = pipe_item.meta
                 next_item = step(item, meta=pipe_item.meta)  # type: ignore
                 if isinstance(next_item, DataItemWithMeta):
                     next_meta = next_item.meta
                     next_item = next_item.data
             except TypeError as ty_ex:
-                assert callable(step)
                 raise InvalidStepFunctionArguments(pipe_item.pipe.name, get_callable_name(step), inspect.signature(step), str(ty_ex))
             except (PipelineException, ExtractorException, DltSourceException, PipeException):
                 raise
             except Exception as ex:
                 raise ResourceExtractionError(pipe_item.pipe.name, step, str(ex), "transform") from ex
             # create next pipe item if a value was returned. A None means that item was consumed/filtered out and should not be further processed
             if next_item is not None:
                 pipe_item = ResolvablePipeItem(next_item, pipe_item.step + 1, pipe_item.pipe, next_meta)
             else:
                 pipe_item = None
 
     def close(self) -> None:
-        # unregister the pipe name right after execution of gen stopped
-        unset_current_pipe_name()
-
         def stop_background_loop(loop: asyncio.AbstractEventLoop) -> None:
             loop.stop()
 
         # stop all futures
         for f, _, _, _ in self._futures:
             if not f.done():
                 f.cancel()
@@ -668,16 +663,16 @@
         # no more sources to iterate
         if len(self._sources) == 0:
             return None
 
         # get items from last added iterator, this makes the overall Pipe as close to FIFO as possible
         gen, step, pipe, meta = self._sources[-1]
         # print(f"got {pipe.name} {pipe._pipe_id}")
-        # register current pipe name during the execution of gen
-        set_current_pipe_name(pipe.name)
+        # TODO: count items coming of the generator and stop the generator if reached. that allows for sampling the beginning of a stream
+        # _counts(id(gen)).setdefault(0) + 1
         try:
             item = next(gen)
             # full pipe item may be returned, this is used by ForkPipe step
             # to redirect execution of an item to another pipe
             if isinstance(item, ResolvablePipeItem):
                 return item
             else:
```

### Comparing `dlt-0.2.8/dlt/extract/schema.py` & `dlt-0.2.8a0/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/extract/source.py` & `dlt-0.2.8a0/dlt/extract/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from dlt.common.configuration.specs import known_sections
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.normalizers.json.relational import DataItemNormalizer as RelationalNormalizer, RelationalNormalizerConfigPropagation
 from dlt.common.schema import Schema
 from dlt.common.schema.typing import TColumnName
 from dlt.common.typing import AnyFun, StrAny, TDataItem, TDataItems, NoneType
 from dlt.common.configuration.container import Container
-from dlt.common.pipeline import PipelineContext, StateInjectableContext, SupportsPipelineRun, resource_state, source_state, pipeline_state
+from dlt.common.pipeline import PipelineContext, StateInjectableContext, SupportsPipelineRun, _resource_state, source_state, pipeline_state
 from dlt.common.utils import flatten_list_or_items, get_callable_name, multi_context_manager, uniq_id
 
 from dlt.extract.typing import DataItemWithMeta, ItemTransformFunc, ItemTransformFunctionWithMeta, TableNameMeta, FilterItem, MapItem, YieldMapItem
 from dlt.extract.pipe import Pipe, ManagedPipeIterator, TPipeStep
 from dlt.extract.schema import DltResourceSchema, TTableSchemaTemplate
 from dlt.extract.incremental import Incremental, IncrementalResourceWrapper
 from dlt.extract.exceptions import (
@@ -292,15 +292,15 @@
             self._bound = True
         return self
 
     @property
     def state(self) -> StrAny:
         """Gets resource-scoped state from the existing pipeline context. If pipeline context is not available, PipelineStateNotAvailable is raised"""
         with self._get_config_section_context():
-            return resource_state(self.name)
+            return _resource_state(self.name)
 
     def __call__(self, *args: Any, **kwargs: Any) -> "DltResource":
         """Binds the parametrized resources to passed arguments. Creates and returns a bound resource. Generators and iterators are not evaluated."""
         if self._bound:
             raise TypeError("Bound DltResource object is not callable")
         r = DltResource.from_data(self._pipe._clone(keep_pipe_id=False), self._name, self.section, self._table_schema_template, self.selected, self._pipe.parent)
         return r.bind(*args, **kwargs)
@@ -332,27 +332,25 @@
             return [
                 self._get_config_section_context(),
                 Container().injectable_context(StateInjectableContext(state=state))
             ]
 
         # managed pipe iterator will remove injected contexts when closing
         with multi_context_manager(_get_context()):
-            pipe_iterator: ManagedPipeIterator = ManagedPipeIterator.from_pipes([self._pipe])  # type: ignore
+            pipe_iterator: ManagedPipeIterator = ManagedPipeIterator.from_pipe(self._pipe)  # type: ignore
 
         pipe_iterator.set_context_manager(multi_context_manager(_get_context()))
         _iter = map(lambda item: item.item, pipe_iterator)
         return flatten_list_or_items(_iter)
 
     def _get_config_section_context(self) -> ContextManager[ConfigSectionContext]:
         container = Container()
         proxy = container[PipelineContext]
         pipeline_name = None if not proxy.is_active() else proxy.pipeline().pipeline_name
-        return inject_section(
-            ConfigSectionContext(pipeline_name=pipeline_name, sections=(known_sections.SOURCES, self.section or pipeline_name or uniq_id(), self._name))
-        )
+        return inject_section(ConfigSectionContext(pipeline_name=pipeline_name, sections=(known_sections.SOURCES, self.section or pipeline_name or uniq_id(), self._name)))
 
     def __str__(self) -> str:
         info = f"DltResource {self._name}"
         if self.section:
             info += f" in section {self.section}:"
         else:
             info += ":"
@@ -509,15 +507,14 @@
     The instance of this class is created whenever you call the `dlt.source` decorated function. It automates several functions for you:
     * You can pass this instance to `dlt` `run` method in order to load all data present in the `dlt resources`.
     * You can select and deselect resources that you want to load via `with_resources` method
     * You can access the resources (which are `DltResource` instances) as source attributes
     * It implements `Iterable` interface so you can get all the data from the resources yourself and without dlt pipeline present.
     * You can get the `schema` for the source and all the resources within it.
     * You can use a `run` method to load the data with a default instance of dlt pipeline.
-    * You can get source read only state for the currently active Pipeline instance
     """
     def __init__(self, name: str, section: str, schema: Schema, resources: Sequence[DltResource] = None) -> None:
         self.name = name
         self.section = section
         self.exhausted = False
         """Tells if iterator associated with a source is exhausted"""
         self._schema = schema
@@ -601,18 +598,17 @@
             # names must be normalized here
             with contextlib.suppress(DataItemRequiredForDynamicTableHints):
                 partial_table = self._schema.normalize_table_identifiers(r.table_schema(item))
                 schema.update_schema(partial_table)
         return schema
 
     def with_resources(self, *resource_names: str) -> "DltSource":
-        """A convenience method to select one of more resources to be loaded. Returns a clone of the original source with the specified resources selected."""
-        source = self.clone()
-        source._resources.select(*resource_names)
-        return source
+        """A convenience method to select one of more resources to be loaded. Returns a source with the specified resources selected."""
+        self._resources.select(*resource_names)
+        return self
 
 
     def add_limit(self, max_items: int) -> "DltSource":  # noqa: A003
         """Adds a limit `max_items` yielded from all selected resources in the source that are not transformers.
 
         This is useful for testing, debugging and generating sample datasets for experimentation. You can easily get your test dataset in a few minutes, when otherwise
         you'd need to wait hours for the full loading to complete.
@@ -634,19 +630,14 @@
 
     @property
     def state(self) -> StrAny:
         """Gets source-scoped state from the existing pipeline context. If pipeline context is not available, PipelineStateNotAvailable is raised"""
         with self._get_config_section_context():
             return source_state()
 
-    def clone(self) -> "DltSource":
-        """Creates a deep copy of the source where copies of schema, resources and pipes are created"""
-        # mind that resources and pipes are cloned when added to the DltResourcesDict in the source constructor
-        return DltSource(self.name, self.section, self.schema.clone(), list(self._resources.values()))
-
     def __iter__(self) -> Iterator[TDataItem]:
         """Opens iterator that yields the data items from all the resources within the source in the same order as in Pipeline class.
 
             A read-only state is provided, initialized from active pipeline state. The state is discarded after the iterator is closed.
 
             A source config section is injected to allow secrets/config injection as during regular extraction.
         """
```

### Comparing `dlt-0.2.8/dlt/extract/typing.py` & `dlt-0.2.8a0/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/extract/utils.py` & `dlt-0.2.8a0/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/helpers/dbt/__init__.py` & `dlt-0.2.8a0/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/helpers/dbt/configuration.py` & `dlt-0.2.8a0/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.2.8a0/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/helpers/dbt/exceptions.py` & `dlt-0.2.8a0/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/helpers/dbt/profiles.yml` & `dlt-0.2.8a0/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/helpers/dbt/runner.py` & `dlt-0.2.8a0/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/helpers/pandas.py` & `dlt-0.2.8a0/dlt/helpers/pandas.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/helpers/parquet.py` & `dlt-0.2.8a0/dlt/helpers/parquet.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/helpers/streamlit.py` & `dlt-0.2.8a0/dlt/helpers/streamlit.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/load/configuration.py` & `dlt-0.2.8a0/dlt/load/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from dlt.common.configuration import configspec
-from dlt.common.storages import LoadStorageConfiguration
+from dlt.common.configuration.specs import LoadVolumeConfiguration
 from dlt.common.runners.configuration import PoolRunnerConfiguration, TPoolType
 
 
 @configspec(init=True)
 class LoaderConfiguration(PoolRunnerConfiguration):
     workers: int = 20
     """how many parallel loads can be executed"""
     pool_type: TPoolType = "thread"  # mostly i/o (upload) so may be thread pool
     raise_on_failed_jobs: bool = False
     """when True, raises on terminally failed jobs immediately"""
     raise_on_max_retries: int = 5
     """When gt 0 will raise when job reaches raise_on_max_retries"""
-    _load_storage_config: LoadStorageConfiguration = None
+    _load_storage_config: LoadVolumeConfiguration = None
 
     if TYPE_CHECKING:
         def __init__(
             self,
-            pool_type: TPoolType = "thread",
+            pool_type: TPoolType = None,
             workers: int = None,
             raise_on_failed_jobs: bool = False,
-            _load_storage_config: LoadStorageConfiguration = None
+            _load_storage_config: LoadVolumeConfiguration = None
         ) -> None:
             ...
```

### Comparing `dlt-0.2.8/dlt/load/exceptions.py` & `dlt-0.2.8a0/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/load/load.py` & `dlt-0.2.8a0/dlt/load/load.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/normalize/configuration.py` & `dlt-0.2.8a0/dlt/normalize/configuration.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import TYPE_CHECKING
 
 from dlt.common.configuration import configspec
+from dlt.common.configuration.specs import LoadVolumeConfiguration, NormalizeVolumeConfiguration, SchemaVolumeConfiguration
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.runners.configuration import PoolRunnerConfiguration, TPoolType
-from dlt.common.storages import LoadStorageConfiguration, NormalizeStorageConfiguration, SchemaStorageConfiguration
 
 
 @configspec(init=True)
 class NormalizeConfiguration(PoolRunnerConfiguration):
     pool_type: TPoolType = "process"
     destination_capabilities: DestinationCapabilitiesContext = None  # injectable
-    _schema_storage_config: SchemaStorageConfiguration
-    _normalize_storage_config: NormalizeStorageConfiguration
-    _load_storage_config: LoadStorageConfiguration
+    _schema_storage_config: SchemaVolumeConfiguration
+    _normalize_storage_config: NormalizeVolumeConfiguration
+    _load_storage_config: LoadVolumeConfiguration
 
     if TYPE_CHECKING:
         def __init__(
             self,
-            pool_type: TPoolType = "process",
+            pool_type: TPoolType = None,
             workers: int = None,
-            _schema_storage_config: SchemaStorageConfiguration = None,
-            _normalize_storage_config: NormalizeStorageConfiguration = None,
-            _load_storage_config: LoadStorageConfiguration = None
+            _schema_storage_config: SchemaVolumeConfiguration = None,
+            _normalize_storage_config: NormalizeVolumeConfiguration = None,
+            _load_storage_config: LoadVolumeConfiguration = None
         ) -> None:
             ...
```

### Comparing `dlt-0.2.8/dlt/normalize/normalize.py` & `dlt-0.2.8a0/dlt/normalize/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 from typing import Any, Callable, List, Dict, Sequence, Tuple
 from multiprocessing.pool import AsyncResult, Pool as ProcessPool
 
 from dlt.common import pendulum, json, logger, sleep
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
 from dlt.common.configuration.container import Container
+from dlt.common.configuration.specs import LoadVolumeConfiguration, NormalizeVolumeConfiguration
 from dlt.common.destination import DestinationCapabilitiesContext, TLoaderFileFormat
 from dlt.common.json import custom_pua_decode
 from dlt.common.runners import TRunMetrics, Runnable
 from dlt.common.runtime import signals
 from dlt.common.runtime.collector import Collector, NULL_COLLECTOR
 from dlt.common.schema.typing import TStoredSchema, TTableSchemaColumns
 from dlt.common.schema.utils import merge_schema_updates
 from dlt.common.storages.exceptions import SchemaNotFoundError
-from dlt.common.storages import NormalizeStorage, SchemaStorage, LoadStorage, LoadStorageConfiguration, NormalizeStorageConfiguration
+from dlt.common.storages import NormalizeStorage, SchemaStorage, LoadStorage
 from dlt.common.typing import TDataItem
 from dlt.common.schema import TSchemaUpdate, Schema
 from dlt.common.schema.exceptions import CannotCoerceColumnException
 from dlt.common.utils import chunks
 
 from dlt.normalize.configuration import NormalizeConfiguration
 
@@ -61,16 +62,16 @@
         except SchemaNotFoundError:
             schema = Schema(schema_name)
             logger.info(f"Created new schema with name {schema_name}")
         return schema
 
     @staticmethod
     def w_normalize_files(
-            normalize_storage_config: NormalizeStorageConfiguration,
-            loader_storage_config: LoadStorageConfiguration,
+            normalize_storage_config: NormalizeVolumeConfiguration,
+            loader_storage_config: LoadVolumeConfiguration,
             destination_caps: DestinationCapabilitiesContext,
             stored_schema: TStoredSchema,
             load_id: str,
             extracted_items_files: Sequence[str]
         ) -> TWorkerRV:
 
         schema_updates: List[TSchemaUpdate] = []
```

### Comparing `dlt-0.2.8/dlt/pipeline/README.md` & `dlt-0.2.8a0/dlt/pipeline/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/pipeline/__init__.py` & `dlt-0.2.8a0/dlt/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/pipeline/configuration.py` & `dlt-0.2.8a0/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/pipeline/dbt.py` & `dlt-0.2.8a0/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/pipeline/exceptions.py` & `dlt-0.2.8a0/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/pipeline/helpers.py` & `dlt-0.2.8a0/dlt/pipeline/helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/pipeline/pipeline.py` & `dlt-0.2.8a0/dlt/pipeline/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,31 +5,32 @@
 from functools import wraps
 from collections.abc import Sequence as C_Sequence
 from typing import Any, Callable, ClassVar, List, Iterator, Optional, Sequence, Tuple, cast, get_type_hints, ContextManager
 
 from dlt import version
 from dlt.common import json, logger, pendulum
 from dlt.common.configuration import inject_section, known_sections
-from dlt.common.configuration.specs import RunConfiguration, CredentialsConfiguration
+from dlt.common.configuration.specs import RunConfiguration, NormalizeVolumeConfiguration, SchemaVolumeConfiguration, LoadVolumeConfiguration, CredentialsConfiguration
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.exceptions import ConfigFieldMissingException, ContextDefaultCannotBeCreated
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.normalizers import default_normalizers, import_normalizers
 from dlt.common.runtime import signals, initialize_runtime
 from dlt.common.schema.exceptions import InvalidDatasetName
 from dlt.common.schema.typing import TColumnSchema, TSchemaTables, TWriteDisposition
-from dlt.common.storages.load_storage import LoadJobInfo, LoadPackageInfo
+from dlt.common.storages.load_storage import LoadJobInfo, LoadPackageInfo, LoadStorage
 from dlt.common.typing import TFun, TSecretValue
 from dlt.common.runners import pool_runner as runner
-from dlt.common.storages import LiveSchemaStorage, NormalizeStorage, LoadStorage, SchemaStorage, FileStorage, NormalizeStorageConfiguration, SchemaStorageConfiguration, LoadStorageConfiguration
+from dlt.common.storages import LiveSchemaStorage, NormalizeStorage, SchemaStorage
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import DestinationReference, JobClientBase, DestinationClientConfiguration, DestinationClientDwhConfiguration, TDestinationReferenceArg
 from dlt.common.pipeline import ExtractInfo, LoadInfo, NormalizeInfo, SupportsPipeline, TPipelineLocalState, TPipelineState, StateInjectableContext
 from dlt.common.schema import Schema
+from dlt.common.storages.file_storage import FileStorage
 from dlt.common.utils import is_interactive
 
 from dlt.destinations.exceptions import DatabaseUndefinedRelation
 
 from dlt.extract.exceptions import DataItemRequiredForDynamicTableHints, SourceExhausted
 from dlt.extract.extract import ExtractorStorage, extract_with_schema
 from dlt.extract.source import DltResource, DltSource
@@ -194,17 +195,17 @@
         self.full_refresh = full_refresh
         self.collector = progress or _NULL_COLLECTOR
 
         self._container = Container()
         self._pipeline_instance_id = self._create_pipeline_instance_id()
         self._pipeline_storage: FileStorage = None
         self._schema_storage: LiveSchemaStorage = None
-        self._schema_storage_config: SchemaStorageConfiguration = None
-        self._normalize_storage_config: NormalizeStorageConfiguration = None
-        self._load_storage_config: LoadStorageConfiguration = None
+        self._schema_storage_config: SchemaVolumeConfiguration = None
+        self._normalize_storage_config: NormalizeVolumeConfiguration = None
+        self._load_storage_config: LoadVolumeConfiguration = None
         self._trace: PipelineTrace = None
         self._last_trace: PipelineTrace = None
         self._state_restored: bool = False
 
         initialize_runtime(self.runtime_config)
         # initialize pipeline working dir
         self._init_working_dir(pipeline_name, pipelines_dir)
@@ -655,22 +656,22 @@
         self._pipeline_storage = FileStorage(self.working_dir, makedirs=False)
         # if full refresh was requested, wipe out all data from working folder, if exists
         if self.full_refresh:
             self._wipe_working_folder()
 
     def _configure(self, import_schema_path: str, export_schema_path: str, must_attach_to_local_pipeline: bool) -> None:
         # create schema storage and folders
-        self._schema_storage_config = SchemaStorageConfiguration(
+        self._schema_storage_config = SchemaVolumeConfiguration(
             schema_volume_path=os.path.join(self.working_dir, "schemas"),
             import_schema_path=import_schema_path,
             export_schema_path=export_schema_path
         )
         # create default configs
-        self._normalize_storage_config = NormalizeStorageConfiguration(normalize_volume_path=os.path.join(self.working_dir, "normalize"))
-        self._load_storage_config = LoadStorageConfiguration(load_volume_path=os.path.join(self.working_dir, "load"),)
+        self._normalize_storage_config = NormalizeVolumeConfiguration(normalize_volume_path=os.path.join(self.working_dir, "normalize"))
+        self._load_storage_config = LoadVolumeConfiguration(load_volume_path=os.path.join(self.working_dir, "load"),)
 
         # are we running again?
         has_state = self._pipeline_storage.has_file(Pipeline.STATE_FILE)
         if must_attach_to_local_pipeline and not has_state:
             raise CannotRestorePipelineException(self.pipeline_name, self.pipelines_dir, f"the pipeline was not found in {self.working_dir}.")
 
         self.must_attach_to_local_pipeline = must_attach_to_local_pipeline
```

### Comparing `dlt-0.2.8/dlt/pipeline/progress.py` & `dlt-0.2.8a0/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/pipeline/state_sync.py` & `dlt-0.2.8a0/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/pipeline/trace.py` & `dlt-0.2.8a0/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/pipeline/track.py` & `dlt-0.2.8a0/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/reflection/names.py` & `dlt-0.2.8a0/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/reflection/script_inspector.py` & `dlt-0.2.8a0/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/reflection/script_visitor.py` & `dlt-0.2.8a0/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/sources/helpers/requests/__init__.py` & `dlt-0.2.8a0/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/sources/helpers/requests/retry.py` & `dlt-0.2.8a0/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/sources/helpers/requests/session.py` & `dlt-0.2.8a0/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/sources/helpers/transform.py` & `dlt-0.2.8a0/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/dlt/version.py` & `dlt-0.2.8a0/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.8/pyproject.toml` & `dlt-0.2.8a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.2.8"
+version = "0.2.8a0"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
```

### Comparing `dlt-0.2.8/setup.py` & `dlt-0.2.8a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
  'redshift:platform_python_implementation == "PyPy"': ['psycopg2cffi>=2.9.0']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.2.8',
+    'version': '0.2.8a0',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
     'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Pipelines and Destinations\n\nExplore ready to use pipelines (e.g. Google Sheets) in the [Pipelines docs](https://dlthub.com/docs/pipelines/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Pipelines**: Pipelines are data processing steps that help move and transform data between various sources and destinations. Contribute your custom pipelines to the [dlt-hub/pipelines](https://github.com/dlt-hub/pipelines) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
```

### Comparing `dlt-0.2.8/PKG-INFO` & `dlt-0.2.8a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.2.8
+Version: 0.2.8a0
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
```

