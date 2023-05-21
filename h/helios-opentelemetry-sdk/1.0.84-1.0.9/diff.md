# Comparing `tmp/helios-opentelemetry-sdk-1.0.84.tar.gz` & `tmp/helios-opentelemetry-sdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helios-opentelemetry-sdk-1.0.84.tar", last modified: Sun May 21 08:46:21 2023, max compression
+gzip compressed data, was "helios-opentelemetry-sdk-1.0.9.tar", last modified: Wed Jul 20 15:11:28 2022, max compression
```

## Comparing `helios-opentelemetry-sdk-1.0.84.tar` & `helios-opentelemetry-sdk-1.0.9.tar`

### file list

```diff
@@ -1,122 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.445466 helios-opentelemetry-sdk-1.0.84/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-21 08:46:21.445466 helios-opentelemetry-sdk-1.0.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.437466 helios-opentelemetry-sdk-1.0.84/helios/
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.437466 helios-opentelemetry-sdk-1.0.84/helios/aiosmtplib_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/aiosmtplib_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.437466 helios-opentelemetry-sdk-1.0.84/helios/aiosmtplib_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/aiosmtplib_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.437466 helios-opentelemetry-sdk-1.0.84/helios/aiosmtplib_instrumentation/src/aiosmtplib/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.437466 helios-opentelemetry-sdk-1.0.84/helios/base/
--rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.437466 helios-opentelemetry-sdk-1.0.84/helios/base/data_obfuscator/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/base/data_obfuscator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/base/data_obfuscator/base_data_obfuscator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/base/data_obfuscator/redis_data_obfuscator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.437466 helios-opentelemetry-sdk-1.0.84/helios/base/span_attribute_dropper/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/base/span_attribute_dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/base/span_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.437466 helios-opentelemetry-sdk-1.0.84/helios/base/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/base/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.437466 helios-opentelemetry-sdk-1.0.84/helios/base/tracing/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/base/tracing/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/base/tracing/export/conditional_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/base/tracing/export/fork_process_otlp_span_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/base/tracing/export/hooked_batch_span_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/base/tracing/export/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/base/tracing/suppress_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/helios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/helios_test_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/aio_pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/aiosmtplib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/base_http_instrumentor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/ses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/sqs_message_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/confluent_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/helios_asgi_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/pika.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/pyspark.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/raven.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/instrumentation/urllib3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/kafka_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/kafka_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/kafka_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/kafka_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/kafka_instrumentation/src/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/kafka_instrumentation/src/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/kafka_instrumentation/src/kafka/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/kafka_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/kafka_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/kafka_instrumentation/tests/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/pyspark_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/pyspark_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/pyspark_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/pyspark_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/pyspark_instrumentation/src/pyspark/
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/pyspark_instrumentation/src/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/pyspark_instrumentation/src/pyspark/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/pyspark_instrumentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/pyspark_instrumentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/pyspark_instrumentation/tests/test_pyspark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/src/raven/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/src/raven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/src/raven/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/src/sentry/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/src/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/src/sentry/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.441466 helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/helios/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.445466 helios-opentelemetry-sdk-1.0.84/helios_opentelemetry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-21 08:46:21.000000 helios-opentelemetry-sdk-1.0.84/helios_opentelemetry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-21 08:46:21.000000 helios-opentelemetry-sdk-1.0.84/helios_opentelemetry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 08:46:21.000000 helios-opentelemetry-sdk-1.0.84/helios_opentelemetry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-21 08:46:21.000000 helios-opentelemetry-sdk-1.0.84/helios_opentelemetry_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-21 08:46:21.000000 helios-opentelemetry-sdk-1.0.84/helios_opentelemetry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-21 08:46:21.000000 helios-opentelemetry-sdk-1.0.84/helios_opentelemetry_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:21.445466 helios-opentelemetry-sdk-1.0.84/hstest/
--rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/hstest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/hstest/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-21 08:46:21.445466 helios-opentelemetry-sdk-1.0.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-21 08:46:03.000000 helios-opentelemetry-sdk-1.0.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/
+-rw-r--r--   0 runner    (1001) docker     (121)     7073 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/src/aiosmtplib/
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/base/
+-rw-r--r--   0 runner    (1001) docker     (121)    14478 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8873 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/data_obfuscator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/span_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.113333 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/conditional_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/fork_process_otlp_span_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/hooked_batch_span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/base/tracing/suppress_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7594 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/helios.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5191 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/helios_test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (121)     3757 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/aiosmtplib.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2402 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2555 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/base_http_instrumentor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/
+-rw-r--r--   0 runner    (1001) docker     (121)     4055 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2059 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/consts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/s3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/ses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/sns.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4192 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/sqs_message_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      908 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5970 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/django.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2289 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8605 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/helios_asgi_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2562 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/pika.py
+-rw-r--r--   0 runner    (1001) docker     (121)      577 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/raven.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/redis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/requests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2845 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3549 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/urllib.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2064 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/instrumentation/urllib3.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/src/kafka/
+-rw-r--r--   0 runner    (1001) docker     (121)     9882 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/src/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/src/kafka/package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8440 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/tests/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/src/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (121)    10635 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/src/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/src/pyspark/package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7585 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/tests/test_pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.117333 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/raven/
+-rw-r--r--   0 runner    (1001) docker     (121)     2170 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/raven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/raven/package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/sentry/
+-rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/sentry/package.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/helios/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-07-20 15:11:28.000000 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-07-20 15:11:28.000000 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-20 15:11:28.000000 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-07-20 15:11:28.000000 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-07-20 15:11:28.000000 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-20 15:11:28.000000 helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/hstest/
+-rw-r--r--   0 runner    (1001) docker     (121)     9810 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/hstest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/hstest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-20 15:11:28.121333 helios-opentelemetry-sdk-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-07-20 15:11:09.000000 helios-opentelemetry-sdk-1.0.9/setup.py
```

### Comparing `helios-opentelemetry-sdk-1.0.84/LICENSE` & `helios-opentelemetry-sdk-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/PKG-INFO` & `helios-opentelemetry-sdk-1.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.84
+Version: 1.0.9
 Summary: Helios OpenTelemetry SDK
-Home-page: https://docs.gethelios.dev/docs/python
+Home-page: https://github.com/helios/python-sdk
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Pytest
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -31,8 +32,10 @@
 Navigate to your project's root directory, and install the latest Helios OpenTelemetry SDK:
 ```
 pip install helios-opentelemetry-sdk
 ```
 [Read more](https://docs.gethelios.dev/)
 
 ## Requirements
-Unless otherwise noted, all published artifacts support Python 3.7 or higher.
+Unless otherwise noted, all published artifacts support Python 3.6 or higher.
+
+
```

### Comparing `helios-opentelemetry-sdk-1.0.84/README.md` & `helios-opentelemetry-sdk-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Helios OpenTelemetry SDK
 
 This page describes the Helios OpenTelemetry SDK implementation.
 
 ### Requirements
-Unless otherwise noted, all published artifacts support Python 3.7 or higher.
+Unless otherwise noted, all published artifacts support Python 3.6 or higher.
 
 ### Getting started
 
 #### Installing
 The SDK package is available on the Python Package Index (PyPI). You can install it via pip with the following commands:
 
 `pip install helios-opentelemetry-sdk`
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/base/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/base/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,79 @@
 import os
+import re
 import logging
-import sys
 
 from abc import ABC, abstractmethod
 from logging import getLogger, DEBUG, CRITICAL
 from typing import Dict, List, Optional, Union
 
-from opentelemetry import trace, metrics
-from opentelemetry.sdk.metrics import MeterProvider
+from opentelemetry import trace
 from opentelemetry.baggage import get_baggage, set_baggage
 from opentelemetry.context import Context, attach
 from opentelemetry.propagate import extract
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
-from opentelemetry.sdk.trace import (ReadableSpan, Span, SpanProcessor, TracerProvider)
+from opentelemetry.sdk.trace import (
+    ReadableSpan, Span, SpanProcessor, TracerProvider)
 from opentelemetry.sdk.trace.export import SpanExporter
+
 from helios.base.data_obfuscator import DataObfuscator, DataObfuscatorConfiguration
-from helios.base.span_attribute_dropper import SpanAttributeDropper
 from helios.base.tracing.export.fork_process_otlp_span_exporter import ForkProcessOTLPSpanExporter
 from helios.base.tracing.export.hooked_batch_span_processor import (
     HookedBatchSpanProcessor, HookedBatchSpanProcessorConfig)
 from helios.base.tracing.export.conditional_span_processor import (
     ConditionalSpanProcessor, ConditionalSpanProcessorConfig)
-from helios.utils import Configurations
 
 _LOG = getLogger(__name__)
 
 
 class HeliosTags(object):
     TEST_TRIGGERED_TRACE = 'hs-triggered-test'
 
 
 class HeliosBase(ABC):
     HS_COLLECTOR_ENDPOINT_ENV_VAR = 'HS_COLLECTOR_ENDPOINT'
-    HS_COLLECTOR_METRICS_ENDPOINT_ENV_VAR = 'HS_COLLECTOR_METRICS_ENDPOINT'
     HS_TEST_COLLECTOR_ENDPOINT_ENV_VAR = 'HS_TEST_COLLECTOR_ENDPOINT'
     HS_DEFAULT_COLLECTOR = 'https://collector.heliosphere.io/traces'
-    HS_DEFAULT_METRICS_COLLECTOR = 'https://collector.heliosphere.io/v1/metrics'
     HS_DEFAULT_TEST_COLLECTOR = 'https://collector.heliosphere.io/tests'
 
     def __init__(
         self,
         api_token: str,
         service_name: str,
         collector_endpoint: Optional[str] = None,
-        collector_metrics_endpoint: Optional[str] = None,
         test_collector_endpoint: Optional[str] = None,
         sampling_ratio: Optional[Union[float, int, str]] = 1.0,
         environment: Optional[str] = None,
-        service_namespace: Optional[str] = None,
         commit_hash: Optional[str] = None,
         max_queue_size: Optional[int] = None,
         resource_tags: Optional[Dict[str, Union[bool, float, int, str]]] = None,
         debug: Optional[bool] = False,
         data_obfuscation: Optional[DataObfuscatorConfiguration] = None,
         excluded_urls: Optional[str] = None,
-        excluded_grpc_methods: Optional[str] = None,
-        metadata_only: Optional[bool] = False,
-        disable_metrics_collection: Optional[bool] = False,
-        lambda_step_function_mode: Optional[bool] = False,
         **kwargs
     ):
         if debug:
-            otel_logger = logging.getLogger('opentelemetry')
-            otel_logger.setLevel(DEBUG)
-            otel_logger.addHandler(logging.StreamHandler(sys.stdout))
-            helios_logger = logging.getLogger('helios')
-            helios_logger.setLevel(DEBUG)
-            helios_logger.addHandler(logging.StreamHandler(sys.stdout))
+            logging.getLogger('opentelemetry').setLevel(DEBUG)
+            logging.getLogger('helios').setLevel(DEBUG)
         else:
             logging.getLogger('opentelemetry').setLevel(CRITICAL)
 
         self.api_token = api_token
         self.auto_init = kwargs.get('auto_init', False)
         self.collector_endpoint = collector_endpoint
-        self.collector_metrics_endpoint = collector_metrics_endpoint
         self.test_collector_endpoint = test_collector_endpoint
         self.environment = environment
-        self.service_namespace = service_namespace
         self.commit_hash = commit_hash
         self.resource_tags = resource_tags
         self.max_queue_size = self._extract_max_queue_size(max_queue_size)
         self.service_name = service_name.strip()
         self._validate_service_name()
         self.sampling_ratio = self._validate_sampling_ratio_and_convert_to_float(sampling_ratio)
         self.data_obfuscation = data_obfuscation
         self.excluded_urls = excluded_urls
-        self.excluded_grpc_methods = excluded_grpc_methods
-        self.metadata_only = metadata_only
-        self.disable_metrics_collection = disable_metrics_collection
-        if lambda_step_function_mode:
-            Configurations.STEP_FUNCTION_MODE = True
 
         self.id_generator = kwargs.get('id_generator', None)
         self.custom_sampler = kwargs.get('sampler', None)
 
         # Enable overwriting the default span exporter through kwargs (mainly for testing purposes).
         span_exporter = kwargs.get('span_exporter', None)
         test_span_exporter = kwargs.get('test_span_exporter', None)
@@ -113,37 +93,22 @@
         _LOG.debug('Extracting test span processor')
         self.test_span_processor: SpanProcessor = self.init_test_span_processor()
 
         self.tracer_provider.add_span_processor(self.span_processor)
         self.tracer_provider.add_span_processor(self.test_span_processor)
         self.instrumentations = self.get_instrumentations()
 
-        self.meter_provider = None
-        if not self.disable_metrics_collection:
-            self.meter_provider = self.init_metrics_provider()
-            metrics.set_meter_provider(self.meter_provider)
-
         _LOG.debug('Registering instrumentations')
 
-        instrumentor_config = {
-            'tracer_provider': self.tracer_provider,
-            'excluded_urls': self.excluded_urls,
-            'excluded_grpc_methods': self.excluded_grpc_methods,
-            'fastapi_custom_attributes_hook': kwargs.get('fastapi_custom_attributes_hook'),
-        }
-
-        if self.meter_provider is not None:
-            instrumentor_config['meter_provider'] = self.meter_provider
-
         for instrumentor in self.instrumentations:
-            instrumentor.instrument(**instrumentor_config)
+            instrumentor.instrument(tracer_provider=self.tracer_provider, excluded_urls=self.excluded_urls)
 
         trace.set_tracer_provider(self.tracer_provider)
 
-        print(f'Helios tracing initialized (service: {self.service_name}, token: {self.api_token[0:3] if self.api_token is not None else "NOT PROVIDED"}*****, environment: {self.environment})')
+        _LOG.info(f'Helios tracing initialized (service: {self.service_name}, token: {self.api_token[0:3]}*****, environment: {self.environment})')
 
         if self.is_running_in_databricks():
             try:
                 self.extract_context_from_databricks()
             except Exception as err:
                 _LOG.warning("Failed to extract context from databricks: %s", err)
                 None
@@ -151,29 +116,26 @@
         if self.is_running_in_k8s():
             try:
                 self.extract_context_k8s_job()
             except Exception as err:
                 _LOG.warning("Failed to extract context from k8s job: %s", err)
                 None
 
-        self.send_debug_span()
+        if debug:
+            self.send_debug_span()
 
     def uninstrument(self) -> None:
         for instrumentor in self.instrumentations:
             instrumentor.uninstrument()
 
     @abstractmethod
     def init_tracer_provider(self) -> TracerProvider:
         """Get Trace Provider"""
 
     @abstractmethod
-    def init_metrics_provider(self) -> MeterProvider:
-        """Get Meter Provider"""
-
-    @abstractmethod
     def get_instrumentations(self) -> List[BaseInstrumentor]:
         """Get Instrumentor list"""
 
     def init_span_exporter(self, span_exporter) -> SpanExporter:
         if span_exporter:
             return span_exporter
 
@@ -204,20 +166,18 @@
 
     def init_span_processor(self) -> SpanProcessor:
         if not self.span_exporter:
             error_message = 'Missing Span Exporter.'
             _LOG.error(error_message)
             raise ValueError(error_message)
 
-        if self.metadata_only:
-            on_end_hook = SpanAttributeDropper().drop_non_metadata_attributes
-        elif self.data_obfuscation is not None:
-            on_end_hook = DataObfuscator(self.data_obfuscation).obfuscate_data
-        else:
+        if self.data_obfuscation is None:
             on_end_hook = None
+        else:
+            on_end_hook = DataObfuscator(self.data_obfuscation).obfuscate_data
 
         return HookedBatchSpanProcessor(
             self.span_exporter,
             HookedBatchSpanProcessorConfig(
                 on_start_hook=HeliosBase.on_start_hook,
                 on_end_hook=on_end_hook,
                 max_queue_size=self.max_queue_size
@@ -333,40 +293,40 @@
             HeliosBase.set_span_as_triggered_by_helios_test(span)
         HeliosBase.push_operation_name_attribute(span)
         HeliosBase.push_jaeger_attributes(span)
 
     @staticmethod
     def is_context_of_helios_test(parent_context: Optional[Context]) -> bool:
         baggage_value = get_baggage(HeliosTags.TEST_TRIGGERED_TRACE, parent_context)
-        return baggage_value in [HeliosTags.TEST_TRIGGERED_TRACE, 'true']
+        return baggage_value == HeliosTags.TEST_TRIGGERED_TRACE
 
     @staticmethod
     def is_span_triggered_by_helios_test(span: ReadableSpan) -> bool:
         test_triggered_trace = HeliosTags.TEST_TRIGGERED_TRACE
-        return span.attributes and span.attributes.get(test_triggered_trace) in [test_triggered_trace, 'true']
+        return span.attributes and span.attributes.get(test_triggered_trace) == test_triggered_trace
 
     @staticmethod
     def set_span_as_triggered_by_helios_test(span: Span) -> None:
         test_triggered_trace = HeliosTags.TEST_TRIGGERED_TRACE
-        span.set_attribute(test_triggered_trace, 'true')
+        span.set_attribute(test_triggered_trace, test_triggered_trace)
 
     @staticmethod
     def set_test_triggered_baggage(context: Optional[Context] = None) -> Context:
         test_triggered_trace = HeliosTags.TEST_TRIGGERED_TRACE
-        return set_baggage(test_triggered_trace, 'true', context)
+        return set_baggage(test_triggered_trace, test_triggered_trace, context)
 
     @staticmethod
     def push_jaeger_attributes(span: Span) -> None:
         if span.kind:
             span.set_attribute('span.kind', span.kind.name.lower())
 
-        if span.instrumentation_scope:
-            name = span.instrumentation_scope.name
+        if span.instrumentation_info:
+            name = span.instrumentation_info.name
             span.set_attribute('otel.library.name', name) if name else None
-            version = span.instrumentation_scope.version
+            version = span.instrumentation_info.version
             span.set_attribute('otel.library.version', version) if version else None
 
     @staticmethod
     def push_operation_name_attribute(span: Span) -> None:
         span.set_attribute('span.operation', span.name)
 
     def _extract_max_queue_size(self, max_queue_size: Optional[int]):
@@ -383,14 +343,21 @@
         except Exception:
             _LOG.warning(f'Unable to parse max_queue_size from {max_queue_size}')
 
     def _validate_service_name(self) -> None:
         if not self.service_name:
             raise ValueError('Service name cannot be empty')
 
+        service_name_regex = '^[a-zA-Z0-9][a-zA-Z0-9-_]{1,62}[a-zA-Z0-9]$'
+        compiled_regex = re.compile(service_name_regex)
+        if not compiled_regex.match(self.service_name):
+            raise ValueError(f'Service name must contain letters, digits,\
+                               hyphens and underscores only. It may range\
+                               between 3 to 64 characters. got {self.service_name}')
+
     def _validate_sampling_ratio_and_convert_to_float(
             self, sampling_ratio: Optional[Union[float, int, str]]
     ) -> Optional[float]:
         if sampling_ratio is None or sampling_ratio == "":
             sampling_ratio = 1.0
 
         try:
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/base/data_obfuscator/base_data_obfuscator.py` & `helios-opentelemetry-sdk-1.0.9/helios/base/data_obfuscator.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,86 +4,83 @@
 from json import JSONDecodeError, dumps, loads
 from logging import getLogger
 from typing import Any, List, Optional, Tuple, Union
 
 from jsonpath_ng.ext import parse
 from jsonpath_ng.jsonpath import DatumInContext, JSONPath
 from opentelemetry.sdk.trace import ReadableSpan
-from opentelemetry.util.types import AttributeValue, Attributes
+from opentelemetry.util.types import AttributeValue
 
 from helios.base.span_attributes import SpanAttributes
 
 _LOG = getLogger(__name__)
+DATA_TO_DROP = [SpanAttributes.HTTP_RESPONSE_BODY]
 DATA_TO_OBFUSCATE = [
     SpanAttributes.DB_QUERY_RESULT,
     SpanAttributes.DB_STATEMENT,
     SpanAttributes.HTTP_REQUEST_BODY,
-    SpanAttributes.HTTP_RESPONSE_BODY,
     SpanAttributes.MESSAGING_PAYLOAD,
 ]
-HTTP_HEADERS_ATTRIBUTE_KEYS = [SpanAttributes.HTTP_REQUEST_HEADERS, SpanAttributes.HTTP_RESPONSE_HEADERS]
 IS_DATA_OBFUSCATED_KEY = 'hs_data_obfuscated'
 
 ExpectedValueType = Optional[Union[str, float, int, bool]]
 Mode = Optional[str]
 Rules = Optional[List[Union[Tuple[str, ExpectedValueType], str]]]
 
 
 @dataclass
 class DataObfuscatorConfiguration:
     hmac_key: str
     mode: Mode
     rules: Rules
-    http_headers_mode: Mode
-    http_headers_rules: Optional[List[str]]
 
 
-class BaseDataObfuscator:
+class DataObfuscator:
     _hmac_key: str
     _mode: Mode
     _global_rules: List[Tuple[JSONPath, ExpectedValueType]]
     _local_rules: List[JSONPath]
-    _http_headers_mode: Mode
-    _http_headers_rules: List[str]
 
     def __init__(self, data_obfuscator_configuration: DataObfuscatorConfiguration):
         self._hmac_key = data_obfuscator_configuration.hmac_key
         self._mode = data_obfuscator_configuration.mode
-        self._http_headers_mode = data_obfuscator_configuration.http_headers_mode
         global_rules: List[Tuple[str, ExpectedValueType]] = []
         local_rules: List[str] = []
-        http_headers_rules: List[str] = []
 
         if data_obfuscator_configuration.rules is not None:
             for rule in data_obfuscator_configuration.rules:
-                if BaseDataObfuscator._is_global_rule(rule):
+                if DataObfuscator._is_global_rule(rule):
                     global_rules.append(rule)
                 elif isinstance(rule, str):
                     local_rules.append(rule)
                 else:
                     _LOG.debug(f'Ignoring invalid rule {rule}.')
 
-        if data_obfuscator_configuration.http_headers_rules is not None:
-            for http_header_key in data_obfuscator_configuration.http_headers_rules:
-                http_headers_rules.append(http_header_key.lower())
-
-        _LOG.debug(f'Data obfuscation mode: {self._mode}, global rules: {global_rules}, local rules: {local_rules}.')
-        _LOG.debug(f'HTTP headers obfuscation mode: {self._http_headers_mode}, rules: {http_headers_rules}.')
-        self._global_rules = BaseDataObfuscator._parse_global_rules(global_rules)
-        self._local_rules = BaseDataObfuscator._parse_local_rules(local_rules)
-        self._http_headers_rules = http_headers_rules
+        self._global_rules = DataObfuscator._parse_global_rules(global_rules)
+        self._local_rules = DataObfuscator._parse_local_rules(local_rules)
+
+    def obfuscate_data(self, span: ReadableSpan) -> None:
+        # noinspection PyProtectedMember
+        attributes = span._attributes
+
+        if attributes is None:
+            return
+
+        self._inject_data_obfuscation_flag(span)
+
+        for datum_to_drop in DATA_TO_DROP:
+            if datum_to_drop in attributes:
+                # noinspection PyUnresolvedReferences
+                del attributes[datum_to_drop]
 
-    def obfuscate_data(self, attributes: Attributes, span_id: str) -> None:
         for datum_to_obfuscate in DATA_TO_OBFUSCATE:
             if datum_to_obfuscate in attributes:
                 value = attributes[datum_to_obfuscate]
                 # noinspection PyUnresolvedReferences
-                attributes[datum_to_obfuscate] = self._obfuscate_datum(value, span_id)
-
-        self._obfuscate_http_headers(attributes)
+                attributes[datum_to_obfuscate] = self._obfuscate_datum(value)
 
     @staticmethod
     def hash(key: str, msg: Any, length: int = 8) -> str:
         return hmac.new(key.encode(), str(msg).encode(), hashlib.sha256).hexdigest()[:length]
 
     @staticmethod
     def _is_global_rule(rule: Tuple[str, ExpectedValueType]) -> bool:
@@ -100,83 +97,77 @@
             global_rules: List[Tuple[str, ExpectedValueType]]
     ) -> List[Tuple[JSONPath, ExpectedValueType]]:
         parsed_global_rules: List[Tuple[JSONPath, ExpectedValueType]] = []
 
         for path_expression, expected_value in global_rules:
             try:
                 parsed_path_expression = parse(path_expression)
-                _LOG.debug(f'Added global rule: {path_expression}')
             except Exception as exception:
-                _LOG.debug(f'Ignoring invalid path expression {path_expression}: {exception}')
+                _LOG.debug(f'Ignoring invalid path expression {path_expression}.', exception)
                 parsed_path_expression = None
 
             if parsed_path_expression is not None:
                 parsed_global_rules.append((parsed_path_expression, expected_value))
 
         return parsed_global_rules
 
     @staticmethod
     def _parse_local_rules(local_rules: List[str]) -> List[JSONPath]:
         parsed_local_rules: List[JSONPath] = []
 
         for path_expression in local_rules:
             try:
                 parsed_local_rules.append(parse(path_expression))
-                _LOG.debug(f'Added local rule: {path_expression}')
             except Exception as exception:
-                _LOG.debug(f'Ignoring invalid path expression {path_expression}: {exception}')
+                _LOG.debug(f'Ignoring invalid path expression {path_expression}.', exception)
 
         return parsed_local_rules
 
     @staticmethod
-    def inject_data_obfuscation_flag(span: ReadableSpan) -> None:
+    def _inject_data_obfuscation_flag(span: ReadableSpan) -> None:
         try:
             # noinspection PyProtectedMember, PyUnresolvedReferences
             span.resource.attributes._dict[IS_DATA_OBFUSCATED_KEY] = True
         except Exception as exception:
             _LOG.debug('Cannot inject data obfuscation flag.', exception)
 
-    def _obfuscate_datum(self, value: AttributeValue, span_id: str) -> AttributeValue:
-        _LOG.debug(f'global rules for span_id {span_id} are {self._global_rules}')
-        _LOG.debug(f'local rules for span_id {span_id} are {self._local_rules}')
-        _LOG.debug(f'mode for span_id {span_id} are {self._mode}')
+    def _obfuscate_datum(self, value: AttributeValue) -> AttributeValue:
         if isinstance(value, str):
             dict_or_list: Optional[Union[dict, list]]
 
             try:
                 dict_or_list = loads(value)
             except JSONDecodeError:
                 dict_or_list = None
 
             if dict_or_list is not None:
-                if self._mode == 'allowlist':
+                if self._mode is None or self._mode == 'allowlist':
                     return self._obfuscate_dict_or_list_in_allowlist_mode(value, dict_or_list)
-                elif self._mode is None or self._mode == 'blocklist':
-                    return self._obfuscate_dict_or_list_in_blocklist_mode(dict_or_list, span_id)
+                elif self._mode == 'blocklist':
+                    return self._obfuscate_dict_or_list_in_blocklist_mode(dict_or_list)
                 else:
                     raise ValueError(f'Unsupported mode {self._mode}.')
 
         return self._obfuscate_primitive(value)
 
     def _obfuscate_dict_or_list_in_allowlist_mode(self, value: str, dict_or_list: Union[dict, list]) -> str:
         if self._match_global_rules(dict_or_list):
             return value
         else:
             nodes = self._extract_nodes(dict_or_list)
             obfuscated_dict_or_list = self._obfuscate_object(dict_or_list)
             self._insert_nodes(obfuscated_dict_or_list, nodes, False)
             return dumps(obfuscated_dict_or_list)
 
-    def _obfuscate_dict_or_list_in_blocklist_mode(self, dict_or_list: Union[dict, list], span_id: str) -> str:
+    def _obfuscate_dict_or_list_in_blocklist_mode(self, dict_or_list: Union[dict, list]) -> str:
         if self._match_global_rules(dict_or_list):
             obfuscated_dict_or_list = self._obfuscate_object(dict_or_list)
             return dumps(obfuscated_dict_or_list)
         else:
             nodes = self._extract_nodes(dict_or_list)
-            _LOG.debug(f'number of nodes to be obfuscated: {len(nodes)} for span_id: {span_id}')
             self._insert_nodes(dict_or_list, nodes, True)
             return dumps(dict_or_list)
 
     def _match_global_rules(self, dict_or_list: Union[dict, list]) -> bool:
         for parsed_path_expression, expected_value in self._global_rules:
             try:
                 nodes = parsed_path_expression.find(dict_or_list)
@@ -202,15 +193,15 @@
         return nodes
 
     def _insert_nodes(
             self, dict_or_list: Union[dict, list], nodes: List[DatumInContext], obfuscate_values: bool
     ) -> None:
         for node in nodes:
             try:
-                node.full_path.update(
+                parse(str(node.full_path)).update(
                     dict_or_list, self._obfuscate_object(node.value) if obfuscate_values else node.value
                 )
             except Exception as exception:
                 _LOG.debug(f'Cannot insert node {node} into dictionary or list.', exception)
 
     def _obfuscate_object(self, object_to_obfuscate: Any) -> Any:
         if isinstance(object_to_obfuscate, dict):
@@ -221,52 +212,11 @@
             return self._obfuscate_primitive(object_to_obfuscate)
 
     def _obfuscate_primitive(self, primitive: Any) -> Any:
         if primitive is None or isinstance(primitive, bool):
             return primitive
 
         try:
-            return BaseDataObfuscator.hash(self._hmac_key, primitive)
+            return DataObfuscator.hash(self._hmac_key, primitive)
         except Exception as exception:
             _LOG.debug(f'Cannot hash primitive {primitive}.', exception)
             return '********'
-
-    def _obfuscate_http_headers(self, attributes: Attributes) -> None:
-        if self._skip_http_headers_obfuscation():
-            return
-
-        for http_headers_attribute_key in HTTP_HEADERS_ATTRIBUTE_KEYS:
-            http_headers: Optional[dict]
-
-            try:
-                http_headers = loads(attributes[http_headers_attribute_key])
-            except (JSONDecodeError, KeyError):
-                http_headers = None
-
-            if http_headers is not None:
-                for http_header_key in http_headers.keys():
-                    http_header_key_in_lowercase = http_header_key.lower()
-
-                    if self._obfuscate_http_header(http_header_key_in_lowercase):
-                        http_header_value = http_headers[http_header_key]
-                        http_headers[http_header_key] = self._obfuscate_primitive(http_header_value)
-
-                # noinspection PyUnresolvedReferences
-                attributes[http_headers_attribute_key] = dumps(http_headers)
-
-    def _skip_http_headers_obfuscation(self) -> bool:
-        if self._http_headers_mode is None or self._http_headers_mode == 'blocklist':
-            if len(self._http_headers_rules) == 0:
-                return True
-
-        return False
-
-    def _obfuscate_http_header(self, http_header_key_in_lowercase: str) -> bool:
-        if self._http_headers_mode == 'allowlist':
-            if http_header_key_in_lowercase not in self._http_headers_rules:
-                return True
-
-        if self._http_headers_mode is None or self._http_headers_mode == 'blocklist':
-            if http_header_key_in_lowercase in self._http_headers_rules:
-                return True
-
-        return False
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/base/tracing/export/conditional_span_processor.py` & `helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/conditional_span_processor.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/base/tracing/export/fork_process_otlp_span_exporter.py` & `helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/fork_process_otlp_span_exporter.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from logging import getLogger
 
 import requests
 
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.trace.export import SpanExportResult
 from opentelemetry.exporter.otlp.proto.http import Compression
+from opentelemetry.exporter.otlp.proto.http.trace_exporter.encoder import (
+    _ProtobufEncoder,
+)
 
 _LOG = getLogger(__name__)
 
 
 class ForkProcessOTLPSpanExporter(OTLPSpanExporter):
     def __init__(
             self,
@@ -28,20 +31,20 @@
         try:
             curr_process_id = os.getpid()
             if self.process_id != curr_process_id:
                 _LOG.info('restarting Session object')
                 self.process_id = curr_process_id
                 self.init_session()
         except Exception as err:
-            _LOG.debug('error restarting Session object', err)
+            _LOG.error('error restarting Session object', err)
         return super().export(spans)
 
     def init_session(self):
         self._session = requests.Session()
         self._session.headers.update(self._headers)
         self._session.headers.update(
-            {"Content-Type": "application/x-protobuf"}
+            {"Content-Type": _ProtobufEncoder._CONTENT_TYPE}
         )
         if self._compression is not Compression.NoCompression:
             self._session.headers.update(
                 {"Content-Encoding": self._compression.value}
             )
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/base/tracing/export/hooked_batch_span_processor.py` & `helios-opentelemetry-sdk-1.0.9/helios/base/tracing/export/hooked_batch_span_processor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -47,20 +47,20 @@
             except Exception as err:
                 _LOG.error('error running onStart hook', err)
 
     def on_end(self, span: ReadableSpan) -> None:
         if SuppressTracing.is_tracing_suppressed():
             return
 
+        super().on_end(span)
         if self.on_end_hook:
             try:
                 self.on_end_hook(span)
             except Exception as err:
                 _LOG.error('error running onEnd hook', err)
-        super().on_end(span)
 
         if self.flush_on_end:
             try:
                 if self.flush_on_end(span):
                     self.force_flush()
             except Exception as err:
                 _LOG.error('Error evaluating flushOnSpanEnd predicate', err)
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/helios.py` & `helios-opentelemetry-sdk-1.0.9/helios/helios.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import os
 from logging import getLogger
 from typing import Callable, Dict, List, Optional, Union
 
 from helios import DataObfuscatorConfiguration, HeliosBase, version
 from helios.instrumentation import get_instrumentation_list
-from opentelemetry.metrics import set_meter_provider
-from opentelemetry.sdk.metrics import MeterProvider
-from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
-from opentelemetry.exporter.otlp.proto.http.metric_exporter import OTLPMetricExporter
+
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.util import types
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.semconv.resource import ResourceAttributes
 from opentelemetry.trace.status import Status, StatusCode
 from opentelemetry.trace import set_span_in_context
@@ -34,138 +31,87 @@
     @staticmethod
     def init(
         api_token: str,
         service_name: str,
         enabled: bool = False,
         collector_endpoint: Optional[str] = None,
         test_collector_endpoint: Optional[str] = None,
-        collector_metrics_endpoint: Optional[str] = None,
         sampling_ratio: Optional[Union[float, int, str]] = 1.0,
         environment: Optional[str] = None,
         commit_hash: Optional[str] = None,
         max_queue_size: Optional[int] = None,
         resource_tags: Optional[Dict[str, Union[bool, float, int, str]]] = None,
         debug: Optional[bool] = False,
         data_obfuscation: Optional[DataObfuscatorConfiguration] = None,
-        excluded_urls: Optional[str] = None, # comma-separated regex string
-        excluded_grpc_methods: Optional[str] = None, # comma-separated regex string
-        metadata_only: Optional[bool] = False,
-        disable_metrics_collection: Optional[bool] = False,
-        lambda_step_function_mode: Optional[bool] = False,
+        excluded_urls: Optional[str] = None,  # comma-separated regex string
         **kwargs
     ):
 
         if os.environ.get(Helios.HS_DISABLED_ENV_VAR) in ['True', 'true']:
             _LOG.warning(f'Helios instrumentation disabled by {Helios.HS_DISABLED_ENV_VAR} env var')
             return None
 
         if not enabled:
             _LOG.warning("Helios instrumentation disabled by 'enabled' initialization flag set to False")
             return None
 
-        if service_name is None:
-            service_name = os.environ.get('HS_SERVICE_NAME') or os.environ.get('AWS_LAMBDA_FUNCTION_NAME')
-
         return Helios(
             api_token=api_token,
             service_name=service_name,
             collector_endpoint=collector_endpoint,
             test_collector_endpoint=test_collector_endpoint,
-            collector_metrics_endpoint=collector_metrics_endpoint,
             sampling_ratio=sampling_ratio,
             environment=environment,
             commit_hash=commit_hash,
             max_queue_size=max_queue_size,
             resource_tags=resource_tags,
             debug=debug,
             data_obfuscation=data_obfuscation,
             excluded_urls=excluded_urls,
-            excluded_grpc_methods=excluded_grpc_methods,
-            metadata_only=metadata_only,
-            disable_metrics_collection=disable_metrics_collection,
-            lambda_step_function_mode=lambda_step_function_mode,
             **kwargs
         )
 
     @staticmethod
     def get_instance(*args, **kwargs):
         if Helios.__instance is None:
             Helios.__instance = Helios.init(*args, **kwargs)
         return Helios.__instance
 
     @staticmethod
     def has_instance() -> bool:
         return Helios.__instance is not None
 
-    def _get_resource(self) -> Resource:
+    def init_tracer_provider(self) -> TracerProvider:
         if self.resource_tags:
             resource_tags = self.resource_tags.copy()
         else:
             resource_tags = dict()
-        tags = {
+        resource_tags.update({
             ResourceAttributes.DEPLOYMENT_ENVIRONMENT:
                 self.get_deployment_environment(),
             ResourceAttributes.SERVICE_NAME:
                 self.service_name,
             ResourceAttributes.SERVICE_VERSION:
                 self.get_commit_hash(),
             ResourceAttributes.TELEMETRY_SDK_VERSION:
                 _OPENTELEMETRY_SDK_VERSION,
             ResourceAttributes.TELEMETRY_SDK_NAME:
                 'helios-opentelemetry-sdk',
             SAMPLING_RATIO_RESOURCE_ATTRIBUTE_NAME:
                 self.sampling_ratio
-        }
-
-        service_namespace = self.get_service_namespace()
-        if service_namespace:
-            tags[ResourceAttributes.SERVICE_NAMESPACE] = service_namespace
-
-        awsLambdaFunctionName = os.environ.get('AWS_LAMBDA_FUNCTION_NAME')
-        if awsLambdaFunctionName:
-            tags[ResourceAttributes.FAAS_NAME] = awsLambdaFunctionName
-
-        awsRegion = os.environ.get('AWS_REGION')
-        if awsRegion:
-            tags[ResourceAttributes.CLOUD_REGION] = awsRegion
-
-        resource_tags.update(tags)
-
-        return Resource.create(resource_tags)
+        })
 
-    def init_tracer_provider(self) -> TracerProvider:
-        resource = self._get_resource()
         set_global_response_propagator(TraceResponsePropagator())
 
         return TracerProvider(
             id_generator=self.id_generator,
             sampler=self.get_sampler(),
-            resource=resource,
+            resource=Resource.create(resource_tags),
         )
 
-    def init_metrics_provider(self):
-        try:
-            from opentelemetry.instrumentation.system_metrics import SystemMetricsInstrumentor
-        except Exception as e:
-            # Lambda functions required psutil to be included with its compiled linux binaries
-            # See https://repost.aws/knowledge-center/lambda-python-package-compatible
-            _LOG.error(f"Unable to import SystemMetricsInstrumentor: {e}")
-            return
-
-        resource = self._get_resource()
-        collector_endpoint = (self.collector_metrics_endpoint
-                              or os.environ.get(self.HS_COLLECTOR_METRICS_ENDPOINT_ENV_VAR)
-                              or self.HS_DEFAULT_METRICS_COLLECTOR
-                              )
-        exporter = OTLPMetricExporter(endpoint=collector_endpoint, headers={'Authorization': self.api_token})
-        provider = MeterProvider([PeriodicExportingMetricReader(exporter)], resource=resource)
-        set_meter_provider(provider)
-        SystemMetricsInstrumentor().instrument()
-        return provider
-
     def get_deployment_environment(self) -> str:
         if self.environment:
             return self.environment
 
         environment = None
         if os.environ.get('CI'):
             environment = self.get_ci_environment()
@@ -176,26 +122,14 @@
         if not environment and self.resource_tags:
             environment = \
                 self.resource_tags.get(
                     ResourceAttributes.DEPLOYMENT_ENVIRONMENT)
 
         return environment or os.environ.get('HS_ENVIRONMENT', os.environ.get('DEPLOYMENT_ENV', ''))
 
-    def get_service_namespace(self) -> str:
-        if self.service_namespace:
-            return self.service_namespace
-
-        service_namespace = None
-        if self.resource_tags:
-            service_namespace = \
-                self.resource_tags.get(
-                    ResourceAttributes.SERVICE_NAMESPACE)
-
-        return service_namespace or os.environ.get('HS_SERVICE_NAMESPACE')
-
     def get_ci_environment(self) -> str:
         if os.environ.get('GITHUB_ACTIONS'):
             return 'Github Actions'
 
         if os.environ.get('BITBUCKET_BUILD_NUMBER'):
             return 'Bitbucket Pipeline'
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/helios_test_trace.py` & `helios-opentelemetry-sdk-1.0.9/helios/helios_test_trace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import os
 import requests
 import time
 
 from contextlib import contextmanager
 from opentelemetry import context, trace
-from opentelemetry import baggage
-from opentelemetry.propagate import inject
 from opentelemetry.semconv.resource import ResourceAttributes
 from opentelemetry.instrumentation.utils import _SUPPRESS_INSTRUMENTATION_KEY
 from requests.adapters import HTTPAdapter, RetryError
 from requests.packages.urllib3.util.retry import Retry
 
-from helios import HeliosTags
 from helios.defaults import DEFAULT_HS_API_ENDPOINT
 from helios.utils import encode_id_as_hex_string
 
 HS_TOKEN_ENV_VAR = 'HS_TOKEN'
 
 
 class SpanResult():
@@ -50,28 +47,14 @@
 
                 if response.status_code == 200:
                     return response.json()
 
             except RetryError:
                 return None
 
-    def instrument_playwright(self, page):
-        baggaged_ctx = baggage.set_value(HeliosTags.TEST_TRIGGERED_TRACE, 'true', context.get_current())
-        test_span = trace.get_current_span()
-        test_span.set_attribute('testLibrary', 'playwright')
-
-        def handle_request(route, request):
-            headers = {
-                **request.headers,
-            }
-            inject(headers, baggaged_ctx)
-            route.continue_(headers=headers)
-
-        page.route('**/*', handle_request)
-
     @contextmanager
     def suppress_instrumentation():
         try:
             context_token = context.attach(context.set_value(_SUPPRESS_INSTRUMENTATION_KEY, True))
             yield
         finally:
             if context_token:
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from helios.instrumentation.aiosmtplib import HeliosAiosmtplibInstrumentor
 from helios.instrumentation.base import HeliosBaseInstrumentor
 from helios.instrumentation.botocore import HeliosBotocoreInstrumentor
 from helios.instrumentation.django import HeliosDjangoInstrumentor
 from helios.instrumentation.elasticsearch import HeliosElasticsearchInstrumentor
 from helios.instrumentation.fastapi import HeliosFastAPIInstrumentor
 from helios.instrumentation.flask import HeliosFlaskInstrumentor
-from helios.instrumentation.grpc import HeliosGrpcAioClientInstrumentor, HeliosGrpcAioServerInstrumentor, \
-    HeliosGrpcClientInstrumentor, HeliosGrpcServerInstrumentor
 from helios.instrumentation.httpx import HeliosHttpxInstrumentor
 from helios.instrumentation.kafka import HeliosKafkaInstrumentor
 from helios.instrumentation.logging import HeliosLoggingInstrumentor
 from helios.instrumentation.pika import HeliosPikaInstrumentor
 from helios.instrumentation.psycopg2 import HeliosPsycopg2Instrumentor
 from helios.instrumentation.pymongo import HeliosPymongoInstrumentor
 from helios.instrumentation.pyspark import HeliosPySparkInstrumentor
@@ -19,16 +17,15 @@
 from helios.instrumentation.redis import HeliosRedisInstrumentor
 from helios.instrumentation.requests import HeliosRequestsInstrumentor
 from helios.instrumentation.sentry import HeliosSentryInstrumentor
 from helios.instrumentation.starlette import HeliosStarletteInstrumentor
 from helios.instrumentation.tornado import HeliosTornadoInstrumentor
 from helios.instrumentation.urllib import HeliosUrllibInstrumentor
 from helios.instrumentation.urllib3 import HeliosUrllib3Instrumentor
-from helios.instrumentation.aio_pika import HeliosAioPikaInstrumentor
-from helios.instrumentation.confluent_kafka import HeliosConfluentKafkaInstrumentor
+from helios.instrumentation.grpc import HeliosGrpcClientInstrumentor, HeliosGrpcServerInstrumentor
 
 instrumentation_list = None
 
 
 def get_instrumentation_list():
 
     global instrumentation_list
@@ -37,33 +34,29 @@
         return instrumentation_list
 
     instrumentor_names = [
         ('opentelemetry.instrumentation.aiopg', 'AiopgInstrumentor'),
         ('opentelemetry.instrumentation.asyncpg', 'AsyncPGInstrumentor'),
         ('opentelemetry.instrumentation.boto', 'BotoInstrumentor'),
         ('opentelemetry.instrumentation.celery', 'CeleryInstrumentor'),
-        ('opentelemetry.instrumentation.confluent_kafka', 'ConfluentKafkaInstrumentor'),
         ('opentelemetry.instrumentation.mysql', 'MySQLInstrumentor'),
         ('opentelemetry.instrumentation.pymemcache', 'PymemcacheInstrumentor'),
         ('opentelemetry.instrumentation.pymysql', 'PyMySQLInstrumentor'),
         ('opentelemetry.instrumentation.sqlalchemy', 'SQLAlchemyInstrumentor'),
-        # ('opentelemetry.instrumentation.sqlite3', 'SQLite3Instrumentor'),
+        ('opentelemetry.instrumentation.sqlite3', 'SQLite3Instrumentor'),
     ]
 
     instrumentation_list = [
         HeliosAiohttpInstrumentor(),
-        HeliosAioPikaInstrumentor(),
         HeliosAiosmtplibInstrumentor(),
         HeliosBotocoreInstrumentor(),
         HeliosDjangoInstrumentor(),
         HeliosElasticsearchInstrumentor(),
         HeliosFastAPIInstrumentor(),
         HeliosFlaskInstrumentor(),
-        HeliosGrpcAioClientInstrumentor(),
-        HeliosGrpcAioServerInstrumentor(),
         HeliosGrpcClientInstrumentor(),
         HeliosGrpcServerInstrumentor(),
         HeliosHttpxInstrumentor(),
         HeliosKafkaInstrumentor(),
         HeliosLoggingInstrumentor(),
         HeliosPikaInstrumentor(),
         HeliosPsycopg2Instrumentor(),
@@ -73,15 +66,14 @@
         HeliosRedisInstrumentor(),
         HeliosRequestsInstrumentor(),
         HeliosSentryInstrumentor(),
         HeliosStarletteInstrumentor(),
         HeliosTornadoInstrumentor(),
         HeliosUrllib3Instrumentor(),
         HeliosUrllibInstrumentor(),
-        HeliosConfluentKafkaInstrumentor(),
     ]
 
     for module_name, instrumentor_name in instrumentor_names:
         instrumentor = HeliosBaseInstrumentor.init_instrumentor(module_name, instrumentor_name)
         if instrumentor is not None:
             instrumentation_list.append(instrumentor)
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/aio_pika.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/fastapi.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,58 @@
 from logging import getLogger
 
-from opentelemetry.propagate import extract
-from opentelemetry.context import attach, detach, get_current
-from opentelemetry.trace import get_tracer_provider, set_span_in_context
-from opentelemetry.semconv.trace import (
-    MessagingOperationValues,
-)
+import wrapt
 
-from helios.instrumentation.base import HeliosBaseInstrumentor
+from helios.instrumentation.base_http_instrumentor import HeliosBaseHttpInstrumentor
+from helios.instrumentation.helios_asgi_middleware import HeliosAsgiMiddleware
 
 _LOG = getLogger(__name__)
 
 
-class HeliosAioPikaInstrumentor(HeliosBaseInstrumentor):
-    MODULE_NAME = 'opentelemetry.instrumentation.aio_pika'
-    INSTRUMENTOR_NAME = 'AioPikaInstrumentor'
+class HeliosFastAPIInstrumentor(HeliosBaseHttpInstrumentor):
+    MODULE_NAME = 'opentelemetry.instrumentation.fastapi'
+    INSTRUMENTOR_NAME = 'FastAPIInstrumentor'
 
     def __init__(self):
         super().__init__(self.MODULE_NAME, self.INSTRUMENTOR_NAME)
+        self.tracer_provider = None
+        self.instrumented_apps = set()
 
     def instrument(self, tracer_provider=None, **kwargs):
         if self.get_instrumentor() is None:
             return
+        self.tracer_provider = tracer_provider
+        self.excluded_urls = kwargs.get('excluded_urls')
 
-        self.get_instrumentor().instrument(tracer_provider=tracer_provider)
+        wrapt.wrap_function_wrapper('opentelemetry.instrumentation.fastapi', '_get_route_details', HeliosAsgiMiddleware.get_span_details_wrapper)
+        wrapt.wrap_function_wrapper('fastapi', 'FastAPI.__init__', self.fastapi_instrument_and_init)
 
-
-class AioPikaMessageContext:
-    def __init__(self, message, queue=None):
-        self._message = message
-        self._queue = queue
-        self._span = None
-        self._token = None
-
-    def __enter__(self):
-        from opentelemetry.instrumentation import aio_pika
-        from opentelemetry.instrumentation.aio_pika.span_builder import SpanBuilder
-
-        headers = self._message.headers or {}
-        ctx = extract(headers)
-        if not ctx:
-            ctx = get_current()
-
-        tracer = get_tracer_provider().get_tracer(aio_pika.__name__)
-        builder = SpanBuilder(tracer)
-        builder.set_as_consumer()
-        builder.set_operation(MessagingOperationValues.RECEIVE)
-        builder.set_destination(self._message.exchange or self._message.routing_key)
-        builder.set_channel(self._queue.channel) if self._queue else None
-        builder.set_message(self._message)
-        token = attach(ctx)
-        try:
-            span = builder.build()
-        finally:
-            detach(token)
-
-        if not span or not span.is_recording():
+    def uninstrument(self):
+        if self.get_instrumentor() is None:
             return
 
-        self._span = span
-        self._token = attach(set_span_in_context(self._span))
+        for app in self.instrumented_apps:
+            self.get_instrumentor().uninstrument_app(app)
+        self.instrumented_apps = set()
+
+    def fastapi_instrument_and_init(self, wrapped, instance, args, kwargs):
+        init_response = wrapped(*args, **kwargs)
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        if self._span is not None:
-            self._span.end()
+        try:
+            if instance not in self.instrumented_apps:
+                self.instrumented_apps.add(instance)
+                self.get_instrumentor().instrument_app(
+                    instance,
+                    tracer_provider=self.tracer_provider,
+                    excluded_urls=self.excluded_urls
+                )
+                get_span_details = HeliosBaseHttpInstrumentor.import_attribute(self.MODULE_NAME, '_get_route_details')
+                instance.add_middleware(
+                    HeliosAsgiMiddleware,
+                    tracer=self.tracer_provider.get_tracer(self.MODULE_NAME),
+                    excluded_urls=self.excluded_urls,
+                    get_span_details=get_span_details
+                )
+        except Exception as error:
+            _LOG.debug('fastapi __init__ instrumentation error: %s.', error)
 
-        if self._token is not None:
-            detach(self._token)
+        return init_response
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/aiohttp.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/aiohttp.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/aiosmtplib.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/aiosmtplib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/base.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from opentelemetry.trace import Span
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 
 _LOG = getLogger(__name__)
 
 
 class HeliosBaseInstrumentor(object):
+
     MAX_PAYLOAD_SIZE = os.environ.get('HS_MAX_PAYLOAD_SIZE', 65536)
     DB_QUERY_RESULT_ATTRIBUTE_NAME = "db.query_result"
 
     def __init__(self, module_name: str, class_name: str):
         self._instrumentor = self.init_instrumentor(module_name, class_name)
 
     @staticmethod
@@ -38,15 +39,15 @@
             mod = importlib.import_module(module_name)
             return getattr(mod, attribute_name, None)
         except Exception as err:
             _LOG.debug(err)
             return None
 
     @staticmethod
-    def should_truncate_payload_by_length(content_length: int) -> bool:
+    def should_drop_payload_by_length(content_length: int) -> bool:
         if HeliosBaseInstrumentor.MAX_PAYLOAD_SIZE == '-1':
             return False
         return content_length is not None and content_length > int(HeliosBaseInstrumentor.MAX_PAYLOAD_SIZE)
 
     @staticmethod
     def byte_size(i: any) -> Optional[int]:
         try:
@@ -58,13 +59,11 @@
         except Exception as err:
             _LOG.debug(err)
         return None
 
     @staticmethod
     def set_payload_attribute(span: Span, attribute: str, payload: any, payload_size=None):
         if payload:
-            if HeliosBaseInstrumentor.should_truncate_payload_by_length(
-                    payload_size or HeliosBaseInstrumentor.byte_size(payload)):
-                span.set_attribute(attribute + '.truncated', True)
-                span.set_attribute(attribute, payload[0:int(HeliosBaseInstrumentor.MAX_PAYLOAD_SIZE)])
+            if HeliosBaseInstrumentor.should_drop_payload_by_length(payload_size or HeliosBaseInstrumentor.byte_size(payload)):
+                span.set_attribute(attribute + '.dropped', True)
             else:
                 span.set_attribute(attribute, payload)
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/base_http_instrumentor.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/base_http_instrumentor.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace import Span
 
 from helios.instrumentation.base import HeliosBaseInstrumentor
 
 
 class HeliosBaseHttpInstrumentor(HeliosBaseInstrumentor):
+
     HTTP_REQUEST_BODY_ATTRIBUTE_NAME = 'http.request.body'
     HTTP_REQUEST_HEADERS_ATTRIBUTE_NAME = 'http.request.headers'
     HTTP_RESPONSE_BODY_ATTRIBUTE_NAME = 'http.response.body'
     HTTP_RESPONSE_HEADERS_ATTRIBUTE_NAME = 'http.response.headers'
     DEFAULT_IGNORED_HOSTNAMES = [
         '.epsagon.com',
         'ingest.sentry.io',
@@ -22,39 +23,29 @@
     ]
 
     def __init__(self, module_name: str, class_name: str, ignored_hostnames: Iterable[str] = None):
         super().__init__(module_name, class_name)
         self.ignored_hostnames = ignored_hostnames or self.DEFAULT_IGNORED_HOSTNAMES
 
     @staticmethod
-    def extract_content_length(headers: Dict) -> int:
-        try:
-            for header_key in headers.keys():
-                if header_key.lower() == 'content-length':
-                    return int(headers[header_key])
-        except Exception:
-            return None
-        return None
-
-    @staticmethod
     def base_hook(
-            span: Span, headers_attribute_name: str, payload_attribute_name: str, headers: Dict, payload: Optional[str]
+        span: Span, headers_attribute_name: str, payload_attribute_name: str, headers: Dict, payload: Optional[str]
     ) -> None:
         span.set_attribute(headers_attribute_name, json.dumps(dict(headers), default=str))
-        content_length = HeliosBaseHttpInstrumentor.extract_content_length(dict(headers))
-        HeliosBaseInstrumentor.set_payload_attribute(span, payload_attribute_name, payload, content_length)
+        HeliosBaseInstrumentor.set_payload_attribute(span, payload_attribute_name, payload)
 
     @staticmethod
     def base_response_hook(span: Span, response_headers: Dict, response_payload: Optional[str]) -> None:
         HeliosBaseHttpInstrumentor.base_hook(
             span,
             HeliosBaseHttpInstrumentor.HTTP_RESPONSE_HEADERS_ATTRIBUTE_NAME,
             HeliosBaseHttpInstrumentor.HTTP_RESPONSE_BODY_ATTRIBUTE_NAME,
             response_headers,
-            response_payload)
+            response_payload
+        )
 
     @staticmethod
     def base_request_hook(span: Span, request_headers: Dict, request_payload: Optional[str]) -> None:
         url = span.attributes.get(SpanAttributes.HTTP_URL)
         target = span.attributes.get(SpanAttributes.HTTP_TARGET)
 
         if target is None and url is not None:
@@ -67,8 +58,9 @@
             span.set_attribute(SpanAttributes.HTTP_TARGET, target) if target is not None else None
 
         HeliosBaseHttpInstrumentor.base_hook(
             span,
             HeliosBaseHttpInstrumentor.HTTP_REQUEST_HEADERS_ATTRIBUTE_NAME,
             HeliosBaseHttpInstrumentor.HTTP_REQUEST_BODY_ATTRIBUTE_NAME,
             request_headers,
-            request_payload)
+            request_payload
+        )
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/consts.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/consts.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/dynamodb.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/dynamodb.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/s3.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/s3.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from helios.instrumentation.base import HeliosBaseInstrumentor
 from opentelemetry.semconv.trace import SpanAttributes
 
 from helios.instrumentation.botocore.consts import AwsParam, AwsAttribute, AwsService
 
 
 class S3Instrumentor(object):
 
@@ -10,33 +11,31 @@
 
     def request_hook(self, span, operation_name, api_params):
         if api_params is None:
             return
 
         bucket = api_params.get(AwsParam.BUCKET)
         key = api_params.get(AwsParam.KEY)
+        value = api_params.get(AwsParam.BODY)
 
         attributes = dict({
             SpanAttributes.DB_SYSTEM: AwsService.S3
         })
         if bucket:
             attributes[AwsAttribute.S3_BUCKET] = bucket
         if key:
             attributes[AwsAttribute.S3_KEY] = key
+        if value and type(value) == bytes:
+            HeliosBaseInstrumentor.set_payload_attribute(span, AwsAttribute.DB_QUERY_RESULT, value.decode())
 
         span.set_attributes(attributes)
 
     def response_hook(self, span, operation_name, result):
         attributes = dict({
             SpanAttributes.DB_SYSTEM: AwsService.S3
         })
         # TODO: fix how we read the body. The code below drains it and so customers get an empty body
         # https://botocore.amazonaws.com/v1/documentation/api/latest/reference/response.html#botocore.response.StreamingBody
-        body_stream = result.get(AwsParam.BODY)
-        if body_stream:
-            content_length = getattr(body_stream, '_content_length', None)
-            if type(content_length) == int:
-                attributes[SpanAttributes.MESSAGING_MESSAGE_PAYLOAD_SIZE_BYTES] = content_length
-            elif type(content_length) == str and content_length.isdigit():
-                attributes[SpanAttributes.MESSAGING_MESSAGE_PAYLOAD_SIZE_BYTES] = int(content_length)
-
+        # body_stream = result.get(AwsParam.BODY)
+        # if body_stream:
+        #    HeliosBaseInstrumentor.set_payload_attribute(span, AwsAttribute.DB_QUERY_RESULT, body_stream.read())
         span.set_attributes(attributes)
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/ses.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/ses.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/sns.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/sns.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/sqs.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/sqs.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/sqs_message_context.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/sqs_message_context.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/botocore/utils.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/botocore/utils.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/django.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/django.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import importlib
 from logging import getLogger
+from sys import modules
 
 from opentelemetry.trace import Span
 from opentelemetry.semconv.trace import SpanAttributes
+from opentelemetry.util.http import parse_excluded_urls
 
 from helios.instrumentation.base_http_instrumentor import HeliosBaseHttpInstrumentor
 
 _LOG = getLogger(__name__)
 
 
 class HeliosDjangoInstrumentor(HeliosBaseHttpInstrumentor):
@@ -28,19 +30,21 @@
             except Exception as err:
                 _LOG.warning(err)
 
     def instrument(self, tracer_provider=None, **kwargs):
         if self.get_instrumentor() is None:
             return
 
-        self.get_instrumentor().instrument(
-            tracer_provider=tracer_provider,
-            response_hook=self.response_hook,
-            excluded_urls=kwargs.get('excluded_urls')
-        )
+        # django instrumentation middleware holds excluded_urls as a class var rather than taking in an arg to instrument()
+        if modules[HeliosDjangoInstrumentor.MODULE_NAME] is not None:
+            middleware = getattr(modules[HeliosDjangoInstrumentor.MODULE_NAME], HeliosDjangoInstrumentor.MIDDLEWARE_NAME, None)
+            if middleware is not None:
+                setattr(middleware, '_excluded_urls', parse_excluded_urls(kwargs.get('excluded_urls')))
+
+        self.get_instrumentor().instrument(tracer_provider=tracer_provider, response_hook=self.response_hook)
 
     @staticmethod
     def extract_old_request_http_headers(request):
         if request.META is None or request.META.items() is None:
             return {}
         return dict((h.replace('HTTP_', ''), v) for (h, v) in request.META.items() if h.startswith('HTTP_'))
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/elasticsearch.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/fastapi.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/starlette.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,68 @@
+from sys import modules
 from logging import getLogger
 
 import wrapt
 
+from opentelemetry.util.http import parse_excluded_urls
+
 from helios.instrumentation.base_http_instrumentor import HeliosBaseHttpInstrumentor
 from helios.instrumentation.helios_asgi_middleware import HeliosAsgiMiddleware
 
 _LOG = getLogger(__name__)
 
 
-class HeliosFastAPIInstrumentor(HeliosBaseHttpInstrumentor):
-    MODULE_NAME = 'opentelemetry.instrumentation.fastapi'
-    INSTRUMENTOR_NAME = 'FastAPIInstrumentor'
+class HeliosStarletteInstrumentor(HeliosBaseHttpInstrumentor):
+    MODULE_NAME = 'opentelemetry.instrumentation.starlette'
+    INSTRUMENTOR_NAME = 'StarletteInstrumentor'
 
     def __init__(self):
         super().__init__(self.MODULE_NAME, self.INSTRUMENTOR_NAME)
         self.tracer_provider = None
         self.instrumented_apps = set()
-        self.excluded_urls = None
-        self.custom_attributes_hook = None
 
     def instrument(self, tracer_provider=None, **kwargs):
         if self.get_instrumentor() is None:
             return
+
         self.tracer_provider = tracer_provider
         self.excluded_urls = kwargs.get('excluded_urls')
-        self.custom_attributes_hook = kwargs.get('fastapi_custom_attributes_hook')
 
-        wrapt.wrap_function_wrapper('opentelemetry.instrumentation.fastapi', '_get_route_details', HeliosAsgiMiddleware.get_span_details_wrapper)
-        wrapt.wrap_function_wrapper('fastapi', 'FastAPI.__init__', self.fastapi_instrument_and_init)
+        wrapt.wrap_function_wrapper('opentelemetry.instrumentation.starlette', '_get_route_details', HeliosAsgiMiddleware.get_span_details_wrapper)
+        wrapt.wrap_function_wrapper('starlette.applications', 'Starlette.__init__', self.starlette_instrument_and_run)
 
     def uninstrument(self):
         if self.get_instrumentor() is None:
             return
 
         for app in self.instrumented_apps:
-            self.get_instrumentor().uninstrument_app(app)
+            self.get_instrumentor().uninstrument()
         self.instrumented_apps = set()
 
-    def fastapi_instrument_and_init(self, wrapped, instance, args, kwargs):
-        init_response = wrapped(*args, **kwargs)
+    def starlette_instrument_and_run(self, wrapped, instance, args, kwargs):
+        res = wrapped(*args, **kwargs)
+
+        # starlette instrumentation holds excluded_urls as a module var rather than taking in an arg to instrument()
+        if modules[HeliosStarletteInstrumentor.MODULE_NAME] is not None:
+            setattr(modules[HeliosStarletteInstrumentor.MODULE_NAME], '_excluded_urls', parse_excluded_urls(self.excluded_urls))
 
         try:
             if instance not in self.instrumented_apps:
                 self.instrumented_apps.add(instance)
                 self.get_instrumentor().instrument_app(
                     instance,
-                    tracer_provider=self.tracer_provider,
-                    excluded_urls=self.excluded_urls
+                    # server_request_hook=self.server_request_hook,
+                    # client_request_hook=self.client_request_hook,
+                    # client_response_hook=self.client_response_hook,
+                    tracer_provider=self.tracer_provider
                 )
                 get_span_details = HeliosBaseHttpInstrumentor.import_attribute(self.MODULE_NAME, '_get_route_details')
-                attributes_hook = self.custom_attributes_hook
-                if callable(attributes_hook):
-                    @instance.middleware('http')
-                    async def custom_span_middleware_hook(request, call_next):
-                        try:
-                            attributes = attributes_hook(request)
-                            from helios import create_custom_span
-                            create_custom_span('helios_fastapi_middleware', attributes)
-                        except Exception:
-                            # Protect the hook
-                            pass
-                        return await call_next(request)
-
                 instance.add_middleware(
                     HeliosAsgiMiddleware,
                     tracer=self.tracer_provider.get_tracer(self.MODULE_NAME),
                     excluded_urls=self.excluded_urls,
                     get_span_details=get_span_details
                 )
         except Exception as error:
-            _LOG.debug('fastapi __init__ instrumentation error: %s.', error)
+            _LOG.debug('starlette __init__ instrumentation error: %s.', error)
 
-        return init_response
+        return res
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/flask.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/flask.py`

 * *Files 15% similar despite different names*

```diff
@@ -82,66 +82,53 @@
                 request_body = request.environ['wsgi.input'].read(length)
                 request.environ['request_body_copy'] = request_body
                 request.environ['wsgi.input'] = BytesIO(request_body)
         except Exception as error:
             _LOG.debug('flask request instrumentation error: %s.', error)
 
     @staticmethod
-    def extract_request_body(request):
-        if HeliosFlaskInstrumentor._has_multipart_content_type(request):
-            try:
-                return bytearray(request.environ['request_body_copy'])
-            except Exception:
-                return None
-
-        try:
-            # Protect with try/catch to avoid cases where json could not be parsed, causing an exception
-            request_body = request.json
-            if request_body:
-                return request_body
-        except Exception as e:
-            _LOG.debug('Could not extract json bodyL %s', e)
-
-        return request.data
-
-    @staticmethod
-    def handle_request_attributes(span: Span, request):
-        if request:
-            url = request.url
-            request_body = HeliosFlaskInstrumentor.extract_request_body(request)
-        else:
-            url = None
-            request_body = None
-
-        span.set_attribute(SpanAttributes.HTTP_URL, url) if url else None
-        HeliosFlaskInstrumentor.base_request_hook(span, dict(request.headers), request_body)
-
-    @staticmethod
     def response_hook(span: Span, status: str, response_headers: List[Tuple[str]]) -> None:
         try:
             if span is None:
                 return
 
             request = getattr(span, REQUEST_ATTRIBUTE)
-            HeliosFlaskInstrumentor.handle_request_attributes(span, request)
+            if request:
+                url = request.url
+                request_body = None
+                if HeliosFlaskInstrumentor._has_multipart_content_type(request):
+                    try:
+                        request_body = bytearray(request.environ['request_body_copy'])
+                    except Exception:
+                        request_body = None
+                elif request.json:
+                    request_body = request.json
+                else:
+                    request_body = request.data
+            else:
+                url = None
+                request_body = None
+
+            span.set_attribute(SpanAttributes.HTTP_URL, url) if url else None
+            HeliosFlaskInstrumentor.base_request_hook(span, dict(request.headers), request_body)
 
-            response_body = None
+            body = None
             resp_headers = dict()
 
             for header in response_headers:
                 if len(header) != 2:
                     continue
                 key, value = header
                 if key == HeliosFlaskInstrumentor.RESPONSE_BODY_HEADER_NAME:
-                    response_body = value
+                    body = value
                     response_headers.remove(header)
                 else:
                     resp_headers[key] = value
 
-            HeliosFlaskInstrumentor.base_response_hook(span, resp_headers, response_body)
+            HeliosFlaskInstrumentor.base_response_hook(span, resp_headers, body)
         except Exception as error:
             _LOG.debug('flask response instrumentation error: %s.', error)
 
     @staticmethod
     def flask_response_callback(response):
         try:
             if response is None:
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/helios_asgi_middleware.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/helios_asgi_middleware.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from opentelemetry.context import attach, detach
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace.status import Status
 from opentelemetry.util.http import parse_excluded_urls
 from opentelemetry.instrumentation.utils import http_status_to_status_code
 
 from helios.instrumentation.base_http_instrumentor import HeliosBaseHttpInstrumentor
-from helios.utils import inject_span_to_exception
 
 _LOG = getLogger(__name__)
 
 
 class ASGISetter(Setter):
 
     def set(self, carrier: dict, key: str, value: str) -> None:
@@ -107,16 +106,14 @@
 
         try:
             attributes[HeliosBaseHttpInstrumentor.HTTP_REQUEST_HEADERS_ATTRIBUTE_NAME] = json.dumps(request_headers)
         except Exception as error:
             _LOG.debug('asgi instrumentation __call__ error: %s.', error)
 
         token = attach(propagated_context)
-
-        # noinspection PyBroadException
         try:
             with self.tracer.start_as_current_span(
                     f"{span_name}", kind=trace.SpanKind.SERVER, context=propagated_context
             ) as span:
                 span.set_attributes(attributes)
 
                 async def wrapped_send(message):
@@ -128,16 +125,15 @@
                         if 'headers' in message:
                             response_headers = HeliosAsgiMiddleware.extract_headers(message.get('headers'))
                             self.add_headers_to_span(span, response_headers)
 
                         if 'body' in message:
                             body = message.get('body')
                             body_attr = HeliosBaseHttpInstrumentor.HTTP_RESPONSE_BODY_ATTRIBUTE_NAME
-                            if body is not None and type(body) in (str, bytes) and len(body) != 0:
-                                span.set_attribute(body_attr, body)
+                            span.set_attribute(body_attr, body) if body is not None else None
                     except Exception as sendError:
                         _LOG.debug('asgi send instrumentation error: %s.', sendError)
 
                     return await send(message)
 
                 async def wrapped_receive():
                     message = await receive()
@@ -146,31 +142,25 @@
                         if 'status' in message:
                             status_code = message.get("status")
                             self.set_status_code(span, status_code)
 
                         if 'body' in message:
                             body = message.get('body')
                             body_attr = HeliosBaseHttpInstrumentor.HTTP_REQUEST_BODY_ATTRIBUTE_NAME
-                            if span.attributes.get(body_attr) is None or span.attributes.get(body_attr) == "":
-                                span.set_attribute(body_attr, body) if body is not None and body != "" else None
+                            span.set_attribute(body_attr, body) if body is not None else None
                     except Exception as receiveError:
                         _LOG.debug('asgi receive instrumentation error: %s.', receiveError)
 
                     return message
 
                 inject(scope, setter=asgi_setter)
                 return await self.app(scope, wrapped_receive, wrapped_send)
-        except Exception as exception:
-            span_injected_exception = inject_span_to_exception(exception, span)
         finally:
             detach(token)
 
-        if span_injected_exception is not None:
-            raise span_injected_exception
-
     @staticmethod
     def extract_headers(headers: Optional[List]) -> Optional[Dict]:
         if headers is None:
             return None
 
         try:
             return {
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/httpx.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/httpx.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,14 @@
             else:
                 payload = request.stream.read().decode('utf-8')
 
             HeliosBaseHttpInstrumentor.base_request_hook(span, self.parse_headers(request.headers), payload)
             return _noop_def()
         except Exception as error:
             _LOG.debug('httpx request instrumentation error: %s.', error)
-            return _noop_def()
 
     def response_hook(self, span: Span, _request, response):
         try:
             payload = None
 
             # TODO: Do not extract the response body, as it drains the data and makes it inaccessible later.
             # for member in response.stream:
@@ -52,15 +51,14 @@
             #     else:
             #         payload += member.decode('utf-8')
 
             HeliosBaseHttpInstrumentor.base_response_hook(span, self.parse_headers(response.headers), payload)
             return _noop_def()
         except Exception as error:
             _LOG.debug('httpx response instrumentation error: %s.', error)
-            return _noop_def()
 
     @staticmethod
     def parse_headers(headers: Optional[List[Tuple[bytes, bytes]]]):
         if headers is None:
             return None
         else:
             return {
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/kafka.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/kafka.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/logging.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/logging.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from helios.defaults import DEFAULT_HS_API_ENDPOINT
 from helios.instrumentation.base import HeliosBaseInstrumentor
 import logging
 import json
 import copy
 
-from traceback import format_exception
-from opentelemetry.trace import INVALID_SPAN, INVALID_SPAN_CONTEXT, get_current_span
-from helios.utils import extract_span_from_exc_info, get_trace_vis_url, inject_span_context_to_log_record
+from opentelemetry.trace import (
+    INVALID_SPAN,
+    INVALID_SPAN_CONTEXT,
+    get_current_span,
+)
 
 
 class HeliosLoggingInstrumentor(HeliosBaseInstrumentor):
     MODULE_NAME = 'opentelemetry.instrumentation.logging'
     INSTRUMENTOR_NAME = 'LoggingInstrumentor'
 
     _old_factory = None
@@ -37,71 +40,52 @@
         self.get_instrumentor().uninstrument(tracer_provider=tracer_provider)
 
     def _inject_context_to_record_message(self):
         old_factory = logging.getLogRecordFactory()
         self._old_factory = old_factory
 
         def _collect_error_log(level, record, span):
-            if not isinstance(level, int) or level < logging.ERROR:
-                return
-
-            message = None
-            stack = None
-
-            # noinspection PyBroadException
-            try:
-                if isinstance(record.msg, str):
-                    message = record.msg
-                elif isinstance(record.msg, dict):
-                    message = json.dumps(record.msg)
-            except Exception:
-                pass
-
             # noinspection PyBroadException
             try:
-                exc_info_type, exc_info_exception, exc_info_traceback = record.exc_info
-                stack = ''.join(format_exception(exc_info_type, exc_info_exception, exc_info_traceback)).strip()
+                if level >= logging.ERROR:
+                    if type(record.msg) is dict:
+                        span.add_event('error_log', record.msg)
+                    elif isinstance(record.msg, str):
+                        span.add_event('error_log', {'message': record.msg})
             except Exception:
                 pass
 
-            if message is not None or stack is not None:
-                span.add_event('error_log', {'message': message, 'stack': stack})
-
         def _mark_instrumentation_indicator(span):
             if not span or not span.is_recording() or self._log_instrumented_indicator:
                 return
 
             span.set_attribute('heliosLogInstrumented', True)
             self._log_instrumented_indicator = True
 
         def _inject_go_to_helios_url_to_record(record):
             if hasattr(record, 'otelTraceID'):
                 span_id = getattr(record, 'otelSpanID')
-                record.go_to_helios = get_trace_vis_url(record.otelTraceID, 'logging', span_id)
+                record.go_to_helios = f'{DEFAULT_HS_API_ENDPOINT}?actionTraceId={record.otelTraceID}&spanId={span_id}&source=logging'
 
         def _inject_context_to_record_msg(record, msg_as_json):
-            if 'go_to_helios' not in msg_as_json and hasattr(record, 'go_to_helios'):
+            if 'go_to_helio' not in msg_as_json and hasattr(record, 'go_to_helios'):
                 msg_as_json.setdefault('go_to_helios', record.go_to_helios)
             if 'otelServiceName' not in msg_as_json and hasattr(record, 'otelServiceName'):
                 msg_as_json.setdefault('otelServiceName', record.otelServiceName)
             if 'otelSpanID' not in msg_as_json and hasattr(record, 'otelSpanID'):
                 msg_as_json.setdefault('otelSpanID', record.otelSpanID)
             if 'otelTraceID' not in msg_as_json and hasattr(record, 'otelTraceID'):
                 msg_as_json.setdefault('otelTraceID', record.otelTraceID)
             return msg_as_json
 
         def record_factory(*args, **kwargs):
             record = old_factory(*args, **kwargs)
-            span = get_current_span()
-
-            if span is None or span == INVALID_SPAN:
-                span = extract_span_from_exc_info(None if record is None else record.exc_info)
-                inject_span_context_to_log_record(record, span)
 
-            if span is not None and span != INVALID_SPAN:
+            span = get_current_span()
+            if span != INVALID_SPAN:
                 _collect_error_log(args[1], record, span)
                 ctx = span.get_span_context()
                 if ctx != INVALID_SPAN_CONTEXT:
                     # noinspection PyBroadException
                     try:
                         _mark_instrumentation_indicator(span)
                         _inject_go_to_helios_url_to_record(record)
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/pika.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/pika.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 import json
 from logging import getLogger
-
-from opentelemetry.context import attach, detach, get_current
-from opentelemetry.propagate import extract
-from opentelemetry.semconv.trace import SpanAttributes
-from opentelemetry.trace import Span, SpanKind, get_tracer_provider, set_span_in_context
-
 from helios.instrumentation.base import HeliosBaseInstrumentor
+from opentelemetry.trace import Span
+from opentelemetry.semconv.trace import SpanAttributes
 
 _LOG = getLogger(__name__)
 
 
 class PikaSpanAttributes:
     MESSAGING_PAYLOAD = 'messaging.payload'
     RABBIT_MQ_HEADERS = 'rabbitmq.headers'
-    RECEIVE_NAME = 'rabbitmq.receiveMessage'
     SEND_NAME = 'rabbitmq.sendMessage'
+    RECEIVE_NAME = 'rabbitmq.receiveMessage'
 
 
 class HeliosPikaInstrumentor(HeliosBaseInstrumentor):
     MODULE_NAME = 'opentelemetry.instrumentation.pika'
     INSTRUMENTOR_NAME = 'PikaInstrumentor'
 
     def __init__(self):
@@ -28,83 +24,40 @@
     def instrument(self, tracer_provider=None, **kwargs):
         if self.get_instrumentor() is None:
             return
 
         self.get_instrumentor().instrument(tracer_provider=tracer_provider, publish_hook=self.publish_hook,
                                            consume_hook=self.consume_hook)
 
-    def publish_hook(self, span: Span, body: bytes, properties):
+    def publish_hook(self, span: Span, body: bytes, properties: dict):
         try:
             span.update_name(PikaSpanAttributes.SEND_NAME)
-            HeliosPikaInstrumentor.set_common_attributes(span, body, properties.headers)
+            self.set_common_attributes(span, body, properties)
             span.set_attribute('span.operation', PikaSpanAttributes.SEND_NAME)
         except Exception as error:
             _LOG.debug('pika publish instrumentation error: %s.', error)
 
     def consume_hook(self, span: Span, body: bytes, properties):
-        HeliosPikaInstrumentor.adjust_span_properties(span, body, properties.headers)
-
-    @staticmethod
-    def adjust_span_properties(span: Span, body: bytes, headers):
         try:
             span.update_name(PikaSpanAttributes.RECEIVE_NAME)
-            HeliosPikaInstrumentor.set_common_attributes(span, body, headers)
+            self.set_common_attributes(span, body, properties)
             span.set_attribute('span.operation', PikaSpanAttributes.RECEIVE_NAME)
         except Exception as error:
             _LOG.debug('pika consume instrumentation error: %s.', error)
 
-    @staticmethod
-    def set_common_attributes(span: Span, body: bytes, headers):
+    def set_common_attributes(self, span: Span, body: bytes, properties):
         string_body = None
         if type(body) == str:
             string_body = body
         elif type(body) == bytes:
             string_body = body.decode()
         else:
             _LOG.debug('Cannot parse body')
         span.set_attribute(PikaSpanAttributes.MESSAGING_PAYLOAD, string_body) if string_body else None
-        span.set_attribute(PikaSpanAttributes.RABBIT_MQ_HEADERS, json.dumps(headers))
+        span.set_attribute(PikaSpanAttributes.RABBIT_MQ_HEADERS, json.dumps(properties.headers))
         messaging_url = span.attributes.get(SpanAttributes.NET_PEER_NAME, None)
         span.set_attribute(SpanAttributes.MESSAGING_URL, messaging_url) if messaging_url else None
         routing_key = span.attributes['span.operation'].split()[0]
         span.set_attribute(SpanAttributes.MESSAGING_RABBITMQ_ROUTING_KEY, routing_key) if routing_key else None
-        span.set_attribute(SpanAttributes.MESSAGING_SYSTEM, 'rabbitmq')
         span.set_attribute(SpanAttributes.MESSAGING_DESTINATION, 'amq.topic')
         span.set_attribute(SpanAttributes.MESSAGING_DESTINATION_KIND, 'topic')
         span.set_attribute(SpanAttributes.MESSAGING_PROTOCOL, 'amqp')
-
-
-class RabbitMqMessageContext:
-    def __init__(self, method, headers, payload):
-        self._exchange = method.exchange if method else ''
-        self._routing_key = method.routing_key if method else ''
-        self._headers = headers
-        self._payload = payload
-        self._span = None
-        self._token = None
-
-    def __enter__(self):
-        from opentelemetry.instrumentation.pika import pika_instrumentor
-        from opentelemetry.instrumentation.pika.utils import _PikaGetter
-
-        headers = self._headers.headers if self._headers is not None and self._headers.headers is not None else {}
-        context = extract(headers, getter=_PikaGetter())
-
-        if not context:
-            context = get_current()
-
-        tracer = get_tracer_provider().get_tracer(pika_instrumentor.__name__)
-        span_name = f"{self._exchange if self._exchange else self._routing_key}"
-        span = tracer.start_span(span_name, context=context, kind=SpanKind.CONSUMER)
-        if not span.is_recording():
-            return
-
-        self._span = span
-        self._token = attach(set_span_in_context(self._span))
-        HeliosPikaInstrumentor.adjust_span_properties(self._span, self._payload, headers)
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        if self._span is not None:
-            self._span.end()
-
-        if self._token is not None:
-            detach(self._token)
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/psycopg2.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/psycopg2.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/pymongo.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/pymongo.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/pyspark.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/raven.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/raven.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/requests.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 
         default_excluded_urls = ','.join(self.ignored_hostnames)
         custom_excluded_urls = kwargs.get('excluded_urls')
         excluded_urls = ((default_excluded_urls or '') + ',' + (custom_excluded_urls or '')).strip(',')
 
         self.get_instrumentor().instrument(
             tracer_provider=tracer_provider,
-            response_hook=self.response_hook,
+            span_callback=self.span_callback,
             excluded_urls=excluded_urls
         )
 
     @staticmethod
-    def response_hook(span: Span, request, result) -> None:
+    def span_callback(span: Span, result) -> None:
         # result is an object of type requests.Response
         if result is None:
             return
 
         try:
             request = result.request
             if request is not None:
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/sentry.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/sentry.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/starlette.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/urllib3.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,52 @@
-from sys import modules
 from logging import getLogger
-
-import wrapt
-
-from opentelemetry.util.http import parse_excluded_urls
+from typing import Dict
+from opentelemetry.trace import Span
 
 from helios.instrumentation.base_http_instrumentor import HeliosBaseHttpInstrumentor
-from helios.instrumentation.helios_asgi_middleware import HeliosAsgiMiddleware
+from opentelemetry.instrumentation.requests import _SUPPRESS_HTTP_INSTRUMENTATION_KEY
+from opentelemetry import context
 
 _LOG = getLogger(__name__)
 
 
-class HeliosStarletteInstrumentor(HeliosBaseHttpInstrumentor):
-    MODULE_NAME = 'opentelemetry.instrumentation.starlette'
-    INSTRUMENTOR_NAME = 'StarletteInstrumentor'
+class HeliosUrllib3Instrumentor(HeliosBaseHttpInstrumentor):
+    MODULE_NAME = 'opentelemetry.instrumentation.urllib3'
+    INSTRUMENTOR_NAME = 'URLLib3Instrumentor'
 
     def __init__(self):
         super().__init__(self.MODULE_NAME, self.INSTRUMENTOR_NAME)
-        self.tracer_provider = None
-        self.instrumented_apps = set()
 
     def instrument(self, tracer_provider=None, **kwargs):
         if self.get_instrumentor() is None:
             return
 
-        self.tracer_provider = tracer_provider
-        self.excluded_urls = kwargs.get('excluded_urls')
+        self.get_instrumentor().instrument(
+            tracer_provider=tracer_provider, response_hook=self.response_hook, request_hook=self.request_hook)
 
-        wrapt.wrap_function_wrapper('opentelemetry.instrumentation.starlette', '_get_route_details', HeliosAsgiMiddleware.get_span_details_wrapper)
-        wrapt.wrap_function_wrapper('starlette.applications', 'Starlette.__init__', self.starlette_instrument_and_run)
+    @staticmethod
+    def is_instrumented_by_requests():
+        return context.get_value(_SUPPRESS_HTTP_INSTRUMENTATION_KEY)
 
-    def uninstrument(self):
-        if self.get_instrumentor() is None:
-            return
+    @staticmethod
+    def request_hook(span: Span, connection_pool, headers: Dict, body: str) -> None:
+        try:
+            if HeliosUrllib3Instrumentor.is_instrumented_by_requests():
+                return
 
-        for app in self.instrumented_apps:
-            self.get_instrumentor().uninstrument()
-        self.instrumented_apps = set()
-
-    def starlette_instrument_and_run(self, wrapped, instance, args, kwargs):
-        res = wrapped(*args, **kwargs)
-
-        # starlette instrumentation holds excluded_urls as a module var rather than taking in an arg to instrument()
-        if modules[HeliosStarletteInstrumentor.MODULE_NAME] is not None:
-            setattr(modules[HeliosStarletteInstrumentor.MODULE_NAME], '_excluded_urls', parse_excluded_urls(self.excluded_urls))
+            HeliosUrllib3Instrumentor.base_request_hook(span, headers, body)
+        except Exception as error:
+            _LOG.debug('urllib3 request instrumentation error: %s.', error)
 
+    @staticmethod
+    def response_hook(span: Span, connection_pool, response) -> None:
         try:
-            if instance not in self.instrumented_apps:
-                self.instrumented_apps.add(instance)
-                self.get_instrumentor().instrument_app(
-                    instance,
-                    # server_request_hook=self.server_request_hook,
-                    # client_request_hook=self.client_request_hook,
-                    # client_response_hook=self.client_response_hook,
-                    tracer_provider=self.tracer_provider
-                )
-                get_span_details = HeliosBaseHttpInstrumentor.import_attribute(self.MODULE_NAME, '_get_route_details')
-                instance.add_middleware(
-                    HeliosAsgiMiddleware,
-                    tracer=self.tracer_provider.get_tracer(self.MODULE_NAME),
-                    excluded_urls=self.excluded_urls,
-                    get_span_details=get_span_details
-                )
+            # connection_pool is an object of type urllib3.connectionpool.HTTPConnectionPool
+            # response is an object of type urllib3.response.HTTPResponse
+            if HeliosUrllib3Instrumentor.is_instrumented_by_requests():
+                return
+
+            response_headers = response.getheaders()
+            response_payload = response.data
+            HeliosUrllib3Instrumentor.base_response_hook(span, response_headers, response_payload)
         except Exception as error:
-            _LOG.debug('starlette __init__ instrumentation error: %s.', error)
-
-        return res
+            _LOG.debug('urllib3 response instrumentation error: %s.', error)
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/tornado.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/tornado.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/instrumentation/urllib.py` & `helios-opentelemetry-sdk-1.0.9/helios/instrumentation/urllib.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/kafka_instrumentation/src/kafka/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/src/kafka/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 def _serialize_headers(headers):
     if type(headers) == list:
         headers_dict = {}
         for headers_tuple in headers:
             if type(headers_tuple) == tuple and len(headers_tuple) == 2:
                 value = headers_tuple[1].decode() if type(headers_tuple[1]) == bytes else headers_tuple[1]
                 headers_dict[headers_tuple[0]] = value
-        return json.dumps(headers_dict)
+        return f"{headers_dict}"
     return None
 
 
 def _set_span_attributes(span, topic, partition, value, headers, bootstrap_servers):
     if span.is_recording():
         span.set_attribute(SpanAttributes.MESSAGING_SYSTEM, 'kafka')
         span.set_attribute(SpanAttributes.MESSAGING_PROTOCOL, 'kafka')
@@ -233,38 +233,32 @@
         return func(*args, **kwargs)
 
     wrap_function_wrapper("kafka", "KafkaProducer.send", _traced_send)
     wrap_function_wrapper("kafka", "KafkaConsumer.__next__", _traced_next)
     wrap_function_wrapper("kafka", "KafkaConsumer.commit", _traced_commit)
 
 
-def _is_supported():
-    # Older, unsupported versions of kafka don't have this property
-    return hasattr(kafka, '__version__')
-
-
 class KafkaInstrumentor(BaseInstrumentor):
     """An instrumentor for kafka module
     See `BaseInstrumentor`
     """
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
 
     def _instrument(self, **kwargs):
-        if not _is_supported():
-            return
+        """Instruments the kafka module
 
+        Args:
+            **kwargs: Optional arguments
+                ``tracer_provider``: a TracerProvider, defaults to global.
+        """
         tracer_provider = kwargs.get("tracer_provider")
         tracer = trace.get_tracer(
             'opentelemetry.instrumentation.kafka_python', __version__, tracer_provider=tracer_provider
         )
-
         _instrument(tracer)
 
     def _uninstrument(self, **kwargs):
-        if not _is_supported():
-            return
-
         unwrap(kafka.KafkaProducer, "send")
         unwrap(kafka.KafkaConsumer, "__next__")
         unwrap(kafka.KafkaConsumer, "commit")
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/kafka_instrumentation/tests/test_kafka.py` & `helios-opentelemetry-sdk-1.0.9/helios/kafka_instrumentation/tests/test_kafka.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
             value = header[1]
             value = value.decode() if type(value) == bytes else None
             result[header[0]] = value
         return result
 
     def assert_producer_attributes(self, span_operation, span_headers, expected_headers):
         self.assertEqual('send', span_operation)
-        self.assertEqual(json.dumps(self.convert_span_headers(expected_headers)), span_headers)
+        self.assertEqual(f"{self.convert_span_headers(expected_headers)}", span_headers)
 
     def assert_consumer_attributes(self, span_operation, span_headers):
         self.assertEqual('process', span_operation)
         self.assertNotEqual("", span_headers)
         self.assertIsNotNone(span_headers)
 
     def assert_common_attributes(self, span_system, span_topic, span_url, span_payload, expected_payload):
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/pyspark_instrumentation/src/pyspark/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/src/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/pyspark_instrumentation/tests/test_pyspark.py` & `helios-opentelemetry-sdk-1.0.9/helios/pyspark_instrumentation/tests/test_pyspark.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/sampler.py` & `helios-opentelemetry-sdk-1.0.9/helios/sampler.py`

 * *Files identical despite different names*

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/src/raven/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/raven/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import os
 import raven
 from logging import getLogger
 from typing import Collection
 from wrapt import wrap_function_wrapper
 
 from opentelemetry import trace
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation.utils import unwrap
 
+from helios.defaults import DEFAULT_HS_API_ENDPOINT
 from helios.sentry_instrumentation.src.sentry.package import _instruments
-from helios.utils import encode_id_as_hex_string, get_trace_vis_url
+from helios.utils import encode_id_as_hex_string
 
+HS_API_ENDPOINT = os.environ.get('HS_API_ENDPOINT') or DEFAULT_HS_API_ENDPOINT
 _LOG = getLogger(__name__)
 
 
 def has_helios_context(sentry_client):
     if not hasattr(sentry_client, 'context'):
         return False
 
@@ -33,15 +36,15 @@
         try:
             span_context = span.get_span_context()
             trace_id = encode_id_as_hex_string(span_context.trace_id)
             span_id = encode_id_as_hex_string(span_context.span_id, 8)
             if 'user' not in instance.context.data:
                 instance.context.data['user'] = {}
             instance.context.data['user']['Helios'] = {
-                'Trace visualization': get_trace_vis_url(trace_id, 'raven', span_id)
+                'Trace visualization': f'{HS_API_ENDPOINT}?actionTraceId={trace_id}&spanId={span_id}&source=raven'
             }
         except Exception as error:
             _LOG.debug('raven instrumentation wrap_capture_call error: %s.', error)
 
         result = func(*args, **kwargs)
         if has_helios_context(instance):
             del instance.context.data['user']['Helios']
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios/sentry_instrumentation/src/sentry/__init__.py` & `helios-opentelemetry-sdk-1.0.9/helios/sentry_instrumentation/src/sentry/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+import os
 import sentry_sdk
 
 from logging import getLogger
 from typing import Collection
 from wrapt import wrap_function_wrapper
 
 from opentelemetry import trace
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation.utils import unwrap
 
+from helios.defaults import DEFAULT_HS_API_ENDPOINT
 from helios.sentry_instrumentation.src.sentry.package import _instruments
-from helios.utils import encode_id_as_hex_string, get_trace_vis_url
+from helios.utils import encode_id_as_hex_string
 
+HS_API_ENDPOINT = os.environ.get('HS_API_ENDPOINT') or DEFAULT_HS_API_ENDPOINT
 _LOG = getLogger(__name__)
 
 
 def _instrument():
     def wrap_capture_call(func, instance, args, kwargs):
         span = trace.get_current_span()
 
@@ -27,15 +30,15 @@
                 trace_id = encode_id_as_hex_string(span_context.trace_id)
                 span_id = encode_id_as_hex_string(span_context.span_id, 8)
             except Exception as error:
                 _LOG.debug('sentry instrumentation wrap_capture_call error: %s.', error)
 
             with sentry_sdk.push_scope() as scope:
                 try:
-                    scope.set_context('Helios', {'Trace visualization': get_trace_vis_url(trace_id, 'sentry', span_id)})
+                    scope.set_context('Helios', {'Trace visualization': f'{HS_API_ENDPOINT}&actionTraceId={trace_id}?spanId={span_id}&source=sentry'})
                     scope.set_tag('helios-trace-id', trace_id)
                 except Exception as error:
                     _LOG.debug('sentry instrumentation wrap_capture_call error: %s.', error)
 
                 return func(*args, **kwargs)
 
         return func(*args, **kwargs)
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios_opentelemetry_sdk.egg-info/PKG-INFO` & `helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: helios-opentelemetry-sdk
-Version: 1.0.84
+Version: 1.0.9
 Summary: Helios OpenTelemetry SDK
-Home-page: https://docs.gethelios.dev/docs/python
+Home-page: https://github.com/helios/python-sdk
 Author: Helios
 Author-email: support@gethelios.dev
 License: Apache License 2.0
 Keywords: helios,heliosphere,microservices,tracing,distributed-tracing,debugging,testing
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Pytest
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -31,8 +32,10 @@
 Navigate to your project's root directory, and install the latest Helios OpenTelemetry SDK:
 ```
 pip install helios-opentelemetry-sdk
 ```
 [Read more](https://docs.gethelios.dev/)
 
 ## Requirements
-Unless otherwise noted, all published artifacts support Python 3.7 or higher.
+Unless otherwise noted, all published artifacts support Python 3.6 or higher.
+
+
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios_opentelemetry_sdk.egg-info/SOURCES.txt` & `helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,34 +11,28 @@
 helios/utils.py
 helios/version.py
 helios/aiosmtplib_instrumentation/__init__.py
 helios/aiosmtplib_instrumentation/src/__init__.py
 helios/aiosmtplib_instrumentation/src/aiosmtplib/__init__.py
 helios/aiosmtplib_instrumentation/src/aiosmtplib/package.py
 helios/base/__init__.py
+helios/base/data_obfuscator.py
 helios/base/span_attributes.py
-helios/base/data_obfuscator/__init__.py
-helios/base/data_obfuscator/base_data_obfuscator.py
-helios/base/data_obfuscator/redis_data_obfuscator.py
-helios/base/span_attribute_dropper/__init__.py
 helios/base/tracing/__init__.py
 helios/base/tracing/suppress_tracing.py
 helios/base/tracing/export/__init__.py
 helios/base/tracing/export/conditional_span_processor.py
 helios/base/tracing/export/fork_process_otlp_span_exporter.py
 helios/base/tracing/export/hooked_batch_span_processor.py
 helios/base/tracing/export/utils.py
 helios/instrumentation/__init__.py
-helios/instrumentation/aio_pika.py
 helios/instrumentation/aiohttp.py
 helios/instrumentation/aiosmtplib.py
-helios/instrumentation/aws_lambda.py
 helios/instrumentation/base.py
 helios/instrumentation/base_http_instrumentor.py
-helios/instrumentation/confluent_kafka.py
 helios/instrumentation/django.py
 helios/instrumentation/elasticsearch.py
 helios/instrumentation/fastapi.py
 helios/instrumentation/flask.py
 helios/instrumentation/grpc.py
 helios/instrumentation/helios_asgi_middleware.py
 helios/instrumentation/httpx.py
```

### Comparing `helios-opentelemetry-sdk-1.0.84/helios_opentelemetry_sdk.egg-info/requires.txt` & `helios-opentelemetry-sdk-1.0.9/helios_opentelemetry_sdk.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 autowrapt==1.0
 jsonpath-ng==1.5.3
-opentelemetry-api==1.18.0
-opentelemetry-exporter-otlp-proto-http==1.18.0
-opentelemetry-instrumentation-aio-pika==0.39b0
-opentelemetry-instrumentation-aiohttp-client==0.39b0
-opentelemetry-instrumentation-aiopg==0.39b0
-opentelemetry-instrumentation-asyncpg==0.39b0
-opentelemetry-instrumentation-aws-lambda==0.39b0
-opentelemetry-instrumentation-boto==0.39b0
-opentelemetry-instrumentation-botocore==0.39b0
-opentelemetry-instrumentation-celery==0.39b0
-opentelemetry-instrumentation-confluent-kafka==0.39b0
-opentelemetry-instrumentation-django==0.39b0
-opentelemetry-instrumentation-elasticsearch==0.39b0
-opentelemetry-instrumentation-fastapi==0.39b0
-opentelemetry-instrumentation-flask==0.39b0
-opentelemetry-instrumentation-grpc==0.39b0
-opentelemetry-instrumentation-httpx==0.39b0
-opentelemetry-instrumentation-logging==0.39b0
-opentelemetry-instrumentation-mysql==0.39b0
-opentelemetry-instrumentation-pika==0.39b0
-opentelemetry-instrumentation-psycopg2==0.39b0
-opentelemetry-instrumentation-pymemcache==0.39b0
-opentelemetry-instrumentation-pymongo==0.39b0
-opentelemetry-instrumentation-pymysql==0.39b0
-opentelemetry-instrumentation-redis==0.39b0
-opentelemetry-instrumentation-requests==0.39b0
-opentelemetry-instrumentation-sqlalchemy==0.39b0
-opentelemetry-instrumentation-sqlite3==0.39b0
-opentelemetry-instrumentation-starlette==0.39b0
-opentelemetry-instrumentation-tornado==0.39b0
-opentelemetry-instrumentation-urllib==0.39b0
-opentelemetry-instrumentation-urllib3==0.39b0
-opentelemetry-instrumentation-system-metrics==0.39b0
-opentelemetry-instrumentation==0.39b0
-opentelemetry-sdk==1.18.0
+opentelemetry-api==1.11.0
+opentelemetry-exporter-otlp-proto-http==1.11.0
+opentelemetry-instrumentation-aiohttp-client==0.30b0
+opentelemetry-instrumentation-aiopg==0.30b0
+opentelemetry-instrumentation-asyncpg==0.30b0
+opentelemetry-instrumentation-boto==0.30b0
+opentelemetry-instrumentation-botocore==0.30b0
+opentelemetry-instrumentation-celery==0.30b0
+opentelemetry-instrumentation-django==0.30b0
+opentelemetry-instrumentation-elasticsearch==0.30b0
+opentelemetry-instrumentation-fastapi==0.30b0
+opentelemetry-instrumentation-flask==0.30b0
+opentelemetry-instrumentation-grpc==0.30b0
+opentelemetry-instrumentation-httpx==0.30b0
+opentelemetry-instrumentation-logging==0.30b0
+opentelemetry-instrumentation-mysql==0.30b0
+opentelemetry-instrumentation-pika==0.30b0
+opentelemetry-instrumentation-psycopg2==0.30b0
+opentelemetry-instrumentation-pymemcache==0.30b0
+opentelemetry-instrumentation-pymongo==0.30b0
+opentelemetry-instrumentation-pymysql==0.30b0
+opentelemetry-instrumentation-redis==0.30b0
+opentelemetry-instrumentation-requests==0.30b0
+opentelemetry-instrumentation-sqlalchemy==0.30b0
+opentelemetry-instrumentation-sqlite3==0.30b0
+opentelemetry-instrumentation-starlette==0.30b0
+opentelemetry-instrumentation-tornado==0.30b0
+opentelemetry-instrumentation-urllib==0.30b0
+opentelemetry-instrumentation-urllib3==0.30b0
+opentelemetry-instrumentation==0.30b0
+opentelemetry-sdk==1.11.0
 requests~=2.22
-protobuf!=3.20.0,!=3.20.1,<5.0,>=3.19
+protobuf==3.20.1
```

### Comparing `helios-opentelemetry-sdk-1.0.84/hstest/__init__.py` & `helios-opentelemetry-sdk-1.0.9/hstest/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,17 @@
 import os
-import sys
+
 import pytest
 import json
-import logging
-
 from opentelemetry.sdk.trace.export.in_memory_span_exporter import InMemorySpanExporter
 from opentelemetry.trace.status import StatusCode
 from opentelemetry import context
 
-from helios.utils import get_trace_vis_url
-
-_LOG = logging.getLogger(__name__)
-_LOG.addHandler(logging.StreamHandler(sys.stdout))
-_LOG.setLevel(logging.INFO)
-
 SERVICE_NAME = 'hs_test'
 ROOT_SPAN_NAME = 'test_root'
-INSTRUMENTATION_LIB = 'opentelemetry.instrumentation.pytest'
 
 self_test = False
 span_exporter = None
 test_span_exporter = None
 active_span = None
 tracer_provider = None
 tracer = None
@@ -84,19 +75,15 @@
         environment=environment,
         enabled=hs_test_enabled,
         span_exporter=span_exporter,
         test_span_exporter=test_span_exporter
     )
 
     tracer_provider = hs.get_tracer_provider()
-    tracer = tracer_provider.get_tracer(INSTRUMENTATION_LIB)
-
-    if self_test:
-        span_exporter.clear()
-        test_span_exporter.clear()
+    tracer = tracer_provider.get_tracer(__name__)
 
 
 @pytest.hookimpl
 def pytest_sessionfinish():
     if tracer_provider is not None:
         tracer_provider.force_flush()
 
@@ -140,76 +127,59 @@
             elif span.name == ROOT_SPAN_NAME:
                 test_span = span
 
         test_span_ids = [x.context.span_id for x in test_span_exporter.get_finished_spans()]
         assert span_ids == test_span_ids
 
     assert test_span is not None
-    assert test_span.attributes.get('otel.library.name') == INSTRUMENTATION_LIB
     assert test_span.attributes.get(PytestSpanAttributes.NAME) == item.location[-1]
     assert test_span.attributes.get(PytestSpanAttributes.STATUS) == (
         StatusCode.ERROR.value if expected_status != 'passed' else StatusCode.OK.value)
     if expected_status == 'passed':
         assert test_span.attributes.get(PytestSpanAttributes.ERROR_MESSAGE, None) is None
     else:
         assert test_span.attributes.get(PytestSpanAttributes.ERROR_MESSAGE) is not None
 
     if child_span_name:
         assert child_span is not None
         assert child_span.parent.span_id == test_span.context.span_id
         headers = json.loads(child_span.attributes['http.request.headers'])
         from helios import HeliosTags
-        assert headers['baggage'] == f'{HeliosTags.TEST_TRIGGERED_TRACE}=true'
-
-
-def _extract_error_message(result):
-    longrerp = getattr(result, 'longrepr', None)
-    reprcrash = getattr(longrerp, 'reprcrash', None)
-    message = getattr(reprcrash, 'message', None)
-    return message if message else 'Unknown failure'
+        assert headers['baggage'] == f'{HeliosTags.TEST_TRIGGERED_TRACE}={HeliosTags.TEST_TRIGGERED_TRACE}'
 
 
 @pytest.hookimpl(hookwrapper=True)
 def pytest_runtest_makereport(item, call):
     # returns to test execution
     outcome = yield
 
     # when test is done, do nothing if hs_test not enabled
     if not hs_test_enabled:
         return
 
     # when test is done, extract the attributes from the test report
     result = outcome.get_result()
-    if result.when != 'call' or not active_span:
-        return
-
-    try:
-        test_name = result.location[-1]
-        test_skipped = result.outcome == 'skipped'
-        test_successful = result.outcome == 'passed'
-        test_failed = not test_successful and not test_skipped
-        err_msg = _extract_error_message(result) if test_failed else None
-        active_span.set_attributes({
-            PytestSpanAttributes.LIBRARY: 'pytest',
-            PytestSpanAttributes.NAME: test_name,
-            PytestSpanAttributes.STATUS: StatusCode.ERROR.value if test_failed else StatusCode.OK.value
-        })
-        if os.environ.get('CI'):
-            ci_attributes = get_ci_run_parameters()
-            active_span.set_attributes(ci_attributes) if ci_attributes else None
-        active_span.set_attribute(PytestSpanAttributes.ERROR_MESSAGE, err_msg) if err_msg else None
-
-        if not test_skipped:
+    if result.when == 'call':
+        if active_span:
+            test_name = result.location[-1]
+            test_successful = result.outcome == 'passed'
+            err_msg = result.longrepr.reprcrash.message if not test_successful else None
+            active_span.set_attributes({
+                PytestSpanAttributes.LIBRARY: 'pytest',
+                PytestSpanAttributes.NAME: test_name,
+                PytestSpanAttributes.STATUS: StatusCode.OK.value if test_successful else StatusCode.ERROR.value
+            })
+            if os.environ.get('CI'):
+                ci_attributes = get_ci_run_parameters()
+                active_span.set_attributes(ci_attributes) if ci_attributes else None
+            active_span.set_attribute(PytestSpanAttributes.ERROR_MESSAGE, err_msg) if err_msg else None
             # \u2713 is a "v" sign, \u2717 is an "x" sign.
-            _LOG.info('\n\n%s %s:' % ('\u2713' if test_successful else '\u2717', test_name))
-            print_highlighted(
-                'View complete test run in Helios >' if test_successful else 'Investigate test failure in Helios >')
+            print('\n\n%s %s:' % ('\u2713' if test_successful else '\u2717', test_name))
+            print_highlighted('View complete test run in Helios >' if test_successful else 'Investigate test failure in Helios >')
             print_highlighted(get_action_trace_string(active_span.context.trace_id, test_successful))
-    except Exception as e:
-        _LOG.warning('Failed reporting test result status: %s', e)
 
 
 def get_ci_run_parameters():
     env = os.environ
     env_detected = False
     job_name = None
     job_id = None
@@ -266,24 +236,26 @@
         return ci_attributes
 
 
 def get_action_trace_string(trace_id, success):
     x = '\u2715'
     v = '\u2713'
     icon = v if success else x
+    from helios.defaults import DEFAULT_HS_API_ENDPOINT
     from helios.utils import encode_id_as_hex_string
+    hs_api_endpoint = os.environ.get('HS_API_ENDPOINT') or DEFAULT_HS_API_ENDPOINT
     trace_id = encode_id_as_hex_string(trace_id)
-    return f'{icon} {get_trace_vis_url(trace_id, source="pytest")}'
+    return f'{icon} {hs_api_endpoint}?actionTraceId={trace_id}&source=pytest'
 
 
 def print_highlighted(text):
     cyan_bg = '\x1b[46m'
     reset_colors = '\x1b[0m'
     black_text = '\x1b[30m'
-    _LOG.info(f'{cyan_bg}{black_text} {text} {reset_colors}')
+    print(f'{cyan_bg}{black_text} {text} {reset_colors}')
 
 
 def pytest_addoption(parser):
     parser.addoption('--hs_enabled', help="enable instrumented tests", default=None)
     parser.addoption('--hs_access_token', help='access token for Helios', default=None)
     parser.addoption('--environment', help='name of the environment where the tests are running', default='')
     parser.addoption('--collector_endpoint', help='OTEL collector endpoint',
```

### Comparing `helios-opentelemetry-sdk-1.0.84/setup.py` & `helios-opentelemetry-sdk-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     version=PACKAGE_INFO["__version__"],
     description='Helios OpenTelemetry SDK',
     license="Apache License 2.0",
     long_description=open('README_PUBLIC.md').read(),
     long_description_content_type='text/markdown',
     author='Helios',
     author_email='support@gethelios.dev',
-    url='https://docs.gethelios.dev/docs/python',
+    url='https://github.com/helios/python-sdk',
     package_data={
         'helios': ['py.typed'],
         'hstest': ['py.typed'],
     },
     packages=find_packages(exclude=["tests.*", "tests"]),
     install_requires=reqs,
     setup_requires=['pytest-runner', 'flake8'],
@@ -42,17 +42,17 @@
         "helios": ["string = helios:auto_initialize"],
     },
     classifiers=[
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
         "Framework :: Pytest",
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Typing :: Typed'
     ]
 )
```

