# Comparing `tmp/openapi_pydantic-0.1.1.tar.gz` & `tmp/openapi_pydantic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_pydantic-0.1.1.tar", max compression
+gzip compressed data, was "openapi_pydantic-0.2.0.tar", max compression
```

## Comparing `openapi_pydantic-0.1.1.tar` & `openapi_pydantic-0.2.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0     1896 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/LICENSE
--rw-r--r--   0        0        0     8079 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/README.md
--rw-r--r--   0        0        0     1290 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/__init__.py
--rw-r--r--   0        0        0       26 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/py.typed
--rw-r--r--   0        0        0     5464 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/util.py
--rw-r--r--   0        0        0     1335 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/__init__.py
--rw-r--r--   0        0        0     1603 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/README.md
--rw-r--r--   0        0        0     1898 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/__init__.py
--rw-r--r--   0        0        0      747 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/callback.py
--rw-r--r--   0        0        0     5491 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/components.py
--rw-r--r--   0        0        0      865 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/contact.py
--rw-r--r--   0        0        0      215 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/datatype.py
--rw-r--r--   0        0        0     1282 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/discriminator.py
--rw-r--r--   0        0        0     3141 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/encoding.py
--rw-r--r--   0        0        0     1554 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/example.py
--rw-r--r--   0        0        0      731 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/external_documentation.py
--rw-r--r--   0        0        0     1073 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/header.py
--rw-r--r--   0        0        0     1982 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/info.py
--rw-r--r--   0        0        0      645 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/license.py
--rw-r--r--   0        0        0     2958 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/link.py
--rw-r--r--   0        0        0     2980 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/media_type.py
--rw-r--r--   0        0        0     2125 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/oauth_flow.py
--rw-r--r--   0        0        0      835 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/oauth_flows.py
--rw-r--r--   0        0        0     2635 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/open_api.py
--rw-r--r--   0        0        0     6422 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/operation.py
--rw-r--r--   0        0        0     8047 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/parameter.py
--rw-r--r--   0        0        0     4930 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/path_item.py
--rw-r--r--   0        0        0     1017 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/paths.py
--rw-r--r--   0        0        0      894 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/reference.py
--rw-r--r--   0        0        0     3209 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/request_body.py
--rw-r--r--   0        0        0     3719 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/response.py
--rw-r--r--   0        0        0     2050 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/responses.py
--rw-r--r--   0        0        0    22285 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/schema.py
--rw-r--r--   0        0        0     1325 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/security_requirement.py
--rw-r--r--   0        0        0     3545 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/security_scheme.py
--rw-r--r--   0        0        0     1889 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/server.py
--rw-r--r--   0        0        0     1071 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/server_variable.py
--rw-r--r--   0        0        0      887 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/tag.py
--rw-r--r--   0        0        0     5464 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/util.py
--rw-r--r--   0        0        0     1850 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/xml.py
--rw-r--r--   0        0        0     1663 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/README.md
--rw-r--r--   0        0        0     1898 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/__init__.py
--rw-r--r--   0        0        0      806 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/callback.py
--rw-r--r--   0        0        0     5650 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/components.py
--rw-r--r--   0        0        0      861 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/contact.py
--rw-r--r--   0        0        0      238 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/datatype.py
--rw-r--r--   0        0        0     1282 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/discriminator.py
--rw-r--r--   0        0        0     3573 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/encoding.py
--rw-r--r--   0        0        0     1633 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/example.py
--rw-r--r--   0        0        0      729 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/external_documentation.py
--rw-r--r--   0        0        0     1076 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/header.py
--rw-r--r--   0        0        0     2112 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/info.py
--rw-r--r--   0        0        0     1028 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/license.py
--rw-r--r--   0        0        0     3038 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/link.py
--rw-r--r--   0        0        0     3060 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/media_type.py
--rw-r--r--   0        0        0     2306 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/oauth_flow.py
--rw-r--r--   0        0        0      835 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/oauth_flows.py
--rw-r--r--   0        0        0     3500 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/open_api.py
--rw-r--r--   0        0        0     6704 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/operation.py
--rw-r--r--   0        0        0     8049 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/parameter.py
--rw-r--r--   0        0        0     5010 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/path_item.py
--rw-r--r--   0        0        0     1040 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/paths.py
--rw-r--r--   0        0        0     1463 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/reference.py
--rw-r--r--   0        0        0     3209 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/request_body.py
--rw-r--r--   0        0        0     3545 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/response.py
--rw-r--r--   0        0        0     2048 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/responses.py
--rw-r--r--   0        0        0    38873 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/schema.py
--rw-r--r--   0        0        0     1434 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/security_requirement.py
--rw-r--r--   0        0        0     3932 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/security_scheme.py
--rw-r--r--   0        0        0     1890 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/server.py
--rw-r--r--   0        0        0     1069 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/server_variable.py
--rw-r--r--   0        0        0      887 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/tag.py
--rw-r--r--   0        0        0     1962 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/xml.py
--rw-r--r--   0        0        0     1222 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8948 1970-01-01 00:00:00.000000 openapi_pydantic-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1896 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8376 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/README.md
+-rw-r--r--   0        0        0     1329 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/__init__.py
+-rw-r--r--   0        0        0       26 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/py.typed
+-rw-r--r--   0        0        0     5464 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/util.py
+-rw-r--r--   0        0        0     1378 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/__init__.py
+-rw-r--r--   0        0        0      447 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/parser.py
+-rw-r--r--   0        0        0     1603 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/README.md
+-rw-r--r--   0        0        0     1898 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/__init__.py
+-rw-r--r--   0        0        0      747 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/callback.py
+-rw-r--r--   0        0        0     5491 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/components.py
+-rw-r--r--   0        0        0      865 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/contact.py
+-rw-r--r--   0        0        0      215 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/datatype.py
+-rw-r--r--   0        0        0     1282 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/discriminator.py
+-rw-r--r--   0        0        0     3141 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/encoding.py
+-rw-r--r--   0        0        0     1554 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/example.py
+-rw-r--r--   0        0        0      731 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/external_documentation.py
+-rw-r--r--   0        0        0     1073 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/header.py
+-rw-r--r--   0        0        0     1982 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/info.py
+-rw-r--r--   0        0        0      645 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/license.py
+-rw-r--r--   0        0        0     2958 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/link.py
+-rw-r--r--   0        0        0     2980 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/media_type.py
+-rw-r--r--   0        0        0     2125 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/oauth_flow.py
+-rw-r--r--   0        0        0      835 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/oauth_flows.py
+-rw-r--r--   0        0        0     2684 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/open_api.py
+-rw-r--r--   0        0        0     6422 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/operation.py
+-rw-r--r--   0        0        0     8047 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/parameter.py
+-rw-r--r--   0        0        0     4930 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/path_item.py
+-rw-r--r--   0        0        0     1017 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/paths.py
+-rw-r--r--   0        0        0      894 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/reference.py
+-rw-r--r--   0        0        0     3209 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/request_body.py
+-rw-r--r--   0        0        0     3719 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/response.py
+-rw-r--r--   0        0        0     2050 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/responses.py
+-rw-r--r--   0        0        0    22285 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/schema.py
+-rw-r--r--   0        0        0     1325 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/security_requirement.py
+-rw-r--r--   0        0        0     3545 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/security_scheme.py
+-rw-r--r--   0        0        0     1889 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/server.py
+-rw-r--r--   0        0        0     1071 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/server_variable.py
+-rw-r--r--   0        0        0      887 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/tag.py
+-rw-r--r--   0        0        0     5464 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/util.py
+-rw-r--r--   0        0        0     1850 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/xml.py
+-rw-r--r--   0        0        0     1663 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/README.md
+-rw-r--r--   0        0        0     1898 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/__init__.py
+-rw-r--r--   0        0        0      806 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/callback.py
+-rw-r--r--   0        0        0     5650 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/components.py
+-rw-r--r--   0        0        0      861 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/contact.py
+-rw-r--r--   0        0        0      238 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/datatype.py
+-rw-r--r--   0        0        0     1282 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/discriminator.py
+-rw-r--r--   0        0        0     3573 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/encoding.py
+-rw-r--r--   0        0        0     1633 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/example.py
+-rw-r--r--   0        0        0      729 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/external_documentation.py
+-rw-r--r--   0        0        0     1076 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/header.py
+-rw-r--r--   0        0        0     2112 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/info.py
+-rw-r--r--   0        0        0     1028 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/license.py
+-rw-r--r--   0        0        0     3038 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/link.py
+-rw-r--r--   0        0        0     3060 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/media_type.py
+-rw-r--r--   0        0        0     2306 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/oauth_flow.py
+-rw-r--r--   0        0        0      835 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/oauth_flows.py
+-rw-r--r--   0        0        0     3522 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/open_api.py
+-rw-r--r--   0        0        0     6704 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/operation.py
+-rw-r--r--   0        0        0     8049 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/parameter.py
+-rw-r--r--   0        0        0     5010 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/path_item.py
+-rw-r--r--   0        0        0     1040 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/paths.py
+-rw-r--r--   0        0        0     1463 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/reference.py
+-rw-r--r--   0        0        0     3209 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/request_body.py
+-rw-r--r--   0        0        0     3545 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/response.py
+-rw-r--r--   0        0        0     2048 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/responses.py
+-rw-r--r--   0        0        0    38873 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/schema.py
+-rw-r--r--   0        0        0     1434 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/security_requirement.py
+-rw-r--r--   0        0        0     3932 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/security_scheme.py
+-rw-r--r--   0        0        0     1890 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/server.py
+-rw-r--r--   0        0        0     1069 2023-05-21 18:57:52.003084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/server_variable.py
+-rw-r--r--   0        0        0      887 2023-05-21 18:57:52.007084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/tag.py
+-rw-r--r--   0        0        0     1962 2023-05-21 18:57:52.007084 openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/xml.py
+-rw-r--r--   0        0        0     1222 2023-05-21 18:57:52.007084 openapi_pydantic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9245 1970-01-01 00:00:00.000000 openapi_pydantic-0.2.0/PKG-INFO
```

### Comparing `openapi_pydantic-0.1.1/LICENSE` & `openapi_pydantic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/README.md` & `openapi_pydantic-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -70,17 +70,28 @@
 ## Take advantage of Pydantic
 
 Pydantic is a great tool, allow you to use object / dict / mixed data for for input.
 
 The following examples give the same OpenAPI result as above:
 
 ```python
-from openapi_pydantic import OpenAPI, PathItem, Response
+from openapi_pydantic import parse_obj, OpenAPI, PathItem, Response
 
-# Construct OpenAPI from dict
+# Construct OpenAPI from dict, inferring the correct schema version
+open_api = parse_obj({
+    "info": {"title": "My own API", "version": "v0.0.1"},
+    "paths": {
+        "/ping": {
+            "get": {"responses": {"200": {"description": "pong"}}}
+        }
+    },
+})
+
+
+# Construct OpenAPI v3.1.0 schema from dict
 open_api = OpenAPI.parse_obj({
     "info": {"title": "My own API", "version": "v0.0.1"},
     "paths": {
         "/ping": {
             "get": {"responses": {"200": {"description": "pong"}}}
         }
     },
```

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/__init__.py` & `openapi_pydantic-0.2.0/openapi_pydantic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,9 +27,10 @@
 from .v3 import Responses as Responses
 from .v3 import Schema as Schema
 from .v3 import SecurityRequirement as SecurityRequirement
 from .v3 import SecurityScheme as SecurityScheme
 from .v3 import Server as Server
 from .v3 import ServerVariable as ServerVariable
 from .v3 import Tag as Tag
+from .v3 import parse_obj as parse_obj
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/util.py` & `openapi_pydantic-0.2.0/openapi_pydantic/util.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/__init__.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .parser import parse_obj as parse_obj
 from .v3_1_0 import XML as XML
 from .v3_1_0 import Callback as Callback
 from .v3_1_0 import Components as Components
 from .v3_1_0 import Contact as Contact
 from .v3_1_0 import Discriminator as Discriminator
 from .v3_1_0 import Encoding as Encoding
 from .v3_1_0 import Example as Example
```

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/README.md` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/README.md`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/__init__.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/callback.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/callback.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/components.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/components.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/contact.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/contact.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/discriminator.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/discriminator.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/encoding.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/encoding.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/example.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/example.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/external_documentation.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/external_documentation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/header.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/header.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/info.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/info.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/license.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/license.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/link.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/link.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/media_type.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/media_type.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/oauth_flow.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/oauth_flows.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/open_api.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/open_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Literal, Optional
 
 from pydantic import BaseModel, Extra
 
 from .components import Components
 from .external_documentation import ExternalDocumentation
 from .info import Info
 from .paths import Paths
@@ -10,15 +10,15 @@
 from .server import Server
 from .tag import Tag
 
 
 class OpenAPI(BaseModel):
     """This is the root document object of the OpenAPI document."""
 
-    openapi: str = "3.0.3"
+    openapi: Literal["3.0.3", "3.0.2", "3.0.1", "3.0.0"] = "3.0.3"
     """
     **REQUIRED**. This string MUST be the [semantic version number](https://semver.org/spec/v2.0.0.html)
     of the [OpenAPI Specification version](#versions) that the OpenAPI document uses. 
     The `openapi` field SHOULD be used by tooling specifications and clients to 
     interpret the OpenAPI document. This is *not* related to the API 
     [`info.version`](#infoVersion) string.
     """
```

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/operation.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/parameter.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/parameter.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/path_item.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/path_item.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/paths.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/paths.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/reference.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/reference.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/request_body.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/request_body.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/response.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/response.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/responses.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/responses.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/schema.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/schema.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/security_requirement.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/security_requirement.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/security_scheme.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/security_scheme.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/server.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/server.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/server_variable.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/server_variable.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/tag.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/tag.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/util.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/util.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/xml.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_0_3/xml.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/README.md` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/README.md`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/__init__.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/callback.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/callback.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/components.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/components.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/contact.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/contact.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/discriminator.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/discriminator.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/encoding.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/encoding.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/example.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/example.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/external_documentation.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/external_documentation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/header.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/header.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/info.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/info.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/license.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/license.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/link.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/link.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/media_type.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/media_type.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/oauth_flow.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/oauth_flows.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/open_api.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/open_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Literal, Optional, Union
 
 from pydantic import BaseModel, Extra
 
 from .components import Components
 from .external_documentation import ExternalDocumentation
 from .info import Info
 from .path_item import PathItem
@@ -12,15 +12,15 @@
 from .server import Server
 from .tag import Tag
 
 
 class OpenAPI(BaseModel):
     """This is the root document object of the OpenAPI document."""
 
-    openapi: str = "3.1.0"
+    openapi: Literal["3.1.0"] = "3.1.0"
     """
     **REQUIRED**. This string MUST be the [version number](#versions)
     of the OpenAPI Specification that the OpenAPI document uses.
     The `openapi` field SHOULD be used by tooling to interpret the OpenAPI document.
     This is *not* related to the API [`info.version`](#infoVersion) string.
     """
```

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/operation.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/parameter.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/parameter.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/path_item.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/path_item.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/paths.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/paths.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/reference.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/reference.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/request_body.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/request_body.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/response.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/response.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/responses.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/responses.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/schema.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/schema.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/security_requirement.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/security_requirement.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/security_scheme.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/security_scheme.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/server.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/server.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/server_variable.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/server_variable.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/tag.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/tag.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/xml.py` & `openapi_pydantic-0.2.0/openapi_pydantic/v3/v3_1_0/xml.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.1/pyproject.toml` & `openapi_pydantic-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-pydantic"
-version = "0.1.1"
+version = "0.2.0"
 description = "Pydantic OpenAPI schema implementation"
 authors = ["Mike Oakley <mike-oakley@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/mike-oakley/openapi-pydantic"
 license = "MIT"
 keywords = [
   "openapi",
```

### Comparing `openapi_pydantic-0.1.1/PKG-INFO` & `openapi_pydantic-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-pydantic
-Version: 0.1.1
+Version: 0.2.0
 Summary: Pydantic OpenAPI schema implementation
 Home-page: https://github.com/mike-oakley/openapi-pydantic
 License: MIT
 Keywords: openapi,schema,parser,pydantic,validation
 Author: Mike Oakley
 Author-email: mike-oakley@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
@@ -92,17 +92,28 @@
 ## Take advantage of Pydantic
 
 Pydantic is a great tool, allow you to use object / dict / mixed data for for input.
 
 The following examples give the same OpenAPI result as above:
 
 ```python
-from openapi_pydantic import OpenAPI, PathItem, Response
+from openapi_pydantic import parse_obj, OpenAPI, PathItem, Response
 
-# Construct OpenAPI from dict
+# Construct OpenAPI from dict, inferring the correct schema version
+open_api = parse_obj({
+    "info": {"title": "My own API", "version": "v0.0.1"},
+    "paths": {
+        "/ping": {
+            "get": {"responses": {"200": {"description": "pong"}}}
+        }
+    },
+})
+
+
+# Construct OpenAPI v3.1.0 schema from dict
 open_api = OpenAPI.parse_obj({
     "info": {"title": "My own API", "version": "v0.0.1"},
     "paths": {
         "/ping": {
             "get": {"responses": {"200": {"description": "pong"}}}
         }
     },
```

