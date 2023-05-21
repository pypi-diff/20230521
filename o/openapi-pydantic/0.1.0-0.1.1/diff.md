# Comparing `tmp/openapi_pydantic-0.1.0.tar.gz` & `tmp/openapi_pydantic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_pydantic-0.1.0.tar", max compression
+gzip compressed data, was "openapi_pydantic-0.1.1.tar", max compression
```

## Comparing `openapi_pydantic-0.1.0.tar` & `openapi_pydantic-0.1.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1896 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/LICENSE
--rw-r--r--   0        0        0     8079 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/README.md
--rw-r--r--   0        0        0     1290 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/__init__.py
--rw-r--r--   0        0        0       26 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/py.typed
--rw-r--r--   0        0        0     5464 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/util.py
--rw-r--r--   0        0        0     1335 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/__init__.py
--rw-r--r--   0        0        0     1603 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/README.md
--rw-r--r--   0        0        0     1828 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/__init__.py
--rw-r--r--   0        0        0      747 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/callback.py
--rw-r--r--   0        0        0     5491 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/components.py
--rw-r--r--   0        0        0      876 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/contact.py
--rw-r--r--   0        0        0      215 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/datatype.py
--rw-r--r--   0        0        0     1282 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/discriminator.py
--rw-r--r--   0        0        0     3141 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/encoding.py
--rw-r--r--   0        0        0     1554 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/example.py
--rw-r--r--   0        0        0      742 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/external_documentation.py
--rw-r--r--   0        0        0     1073 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/header.py
--rw-r--r--   0        0        0     1993 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/info.py
--rw-r--r--   0        0        0      656 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/license.py
--rw-r--r--   0        0        0     2958 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/link.py
--rw-r--r--   0        0        0     2980 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/media_type.py
--rw-r--r--   0        0        0     2185 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/oauth_flow.py
--rw-r--r--   0        0        0      835 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/oauth_flows.py
--rw-r--r--   0        0        0     2635 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/open_api.py
--rw-r--r--   0        0        0     6422 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/operation.py
--rw-r--r--   0        0        0     8047 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/parameter.py
--rw-r--r--   0        0        0     4930 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/path_item.py
--rw-r--r--   0        0        0     1017 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/paths.py
--rw-r--r--   0        0        0      894 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/reference.py
--rw-r--r--   0        0        0     3209 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/request_body.py
--rw-r--r--   0        0        0     3719 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/response.py
--rw-r--r--   0        0        0     2050 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/responses.py
--rw-r--r--   0        0        0    22285 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/schema.py
--rw-r--r--   0        0        0     1325 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/security_requirement.py
--rw-r--r--   0        0        0     3575 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/security_scheme.py
--rw-r--r--   0        0        0     1889 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/server.py
--rw-r--r--   0        0        0     1071 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/server_variable.py
--rw-r--r--   0        0        0      887 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/tag.py
--rw-r--r--   0        0        0     5464 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/util.py
--rw-r--r--   0        0        0     1850 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/xml.py
--rw-r--r--   0        0        0     1663 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/README.md
--rw-r--r--   0        0        0     1827 2023-05-21 14:25:26.296289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/__init__.py
--rw-r--r--   0        0        0      806 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/callback.py
--rw-r--r--   0        0        0     5650 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/components.py
--rw-r--r--   0        0        0      872 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/contact.py
--rw-r--r--   0        0        0      238 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/datatype.py
--rw-r--r--   0        0        0     1282 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/discriminator.py
--rw-r--r--   0        0        0     3573 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/encoding.py
--rw-r--r--   0        0        0     1633 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/example.py
--rw-r--r--   0        0        0      740 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/external_documentation.py
--rw-r--r--   0        0        0     1076 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/header.py
--rw-r--r--   0        0        0     2123 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/info.py
--rw-r--r--   0        0        0     1039 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/license.py
--rw-r--r--   0        0        0     3038 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/link.py
--rw-r--r--   0        0        0     3060 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/media_type.py
--rw-r--r--   0        0        0     2366 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/oauth_flow.py
--rw-r--r--   0        0        0      835 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/oauth_flows.py
--rw-r--r--   0        0        0     3500 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/open_api.py
--rw-r--r--   0        0        0     6704 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/operation.py
--rw-r--r--   0        0        0     8049 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/parameter.py
--rw-r--r--   0        0        0     5010 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/path_item.py
--rw-r--r--   0        0        0     1040 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/paths.py
--rw-r--r--   0        0        0     1463 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/reference.py
--rw-r--r--   0        0        0     3209 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/request_body.py
--rw-r--r--   0        0        0     3545 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/response.py
--rw-r--r--   0        0        0     2048 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/responses.py
--rw-r--r--   0        0        0    38873 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/schema.py
--rw-r--r--   0        0        0     1434 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/security_requirement.py
--rw-r--r--   0        0        0     3962 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/security_scheme.py
--rw-r--r--   0        0        0     1890 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/server.py
--rw-r--r--   0        0        0     1069 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/server_variable.py
--rw-r--r--   0        0        0      887 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/tag.py
--rw-r--r--   0        0        0     1962 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/xml.py
--rw-r--r--   0        0        0     1222 2023-05-21 14:25:26.304289 openapi_pydantic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8948 1970-01-01 00:00:00.000000 openapi_pydantic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1896 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8079 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/README.md
+-rw-r--r--   0        0        0     1290 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/__init__.py
+-rw-r--r--   0        0        0       26 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/py.typed
+-rw-r--r--   0        0        0     5464 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/util.py
+-rw-r--r--   0        0        0     1335 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/__init__.py
+-rw-r--r--   0        0        0     1603 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/README.md
+-rw-r--r--   0        0        0     1898 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/__init__.py
+-rw-r--r--   0        0        0      747 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/callback.py
+-rw-r--r--   0        0        0     5491 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/components.py
+-rw-r--r--   0        0        0      865 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/contact.py
+-rw-r--r--   0        0        0      215 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/datatype.py
+-rw-r--r--   0        0        0     1282 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/discriminator.py
+-rw-r--r--   0        0        0     3141 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/encoding.py
+-rw-r--r--   0        0        0     1554 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/example.py
+-rw-r--r--   0        0        0      731 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/external_documentation.py
+-rw-r--r--   0        0        0     1073 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/header.py
+-rw-r--r--   0        0        0     1982 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/info.py
+-rw-r--r--   0        0        0      645 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/license.py
+-rw-r--r--   0        0        0     2958 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/link.py
+-rw-r--r--   0        0        0     2980 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/media_type.py
+-rw-r--r--   0        0        0     2125 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/oauth_flow.py
+-rw-r--r--   0        0        0      835 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/oauth_flows.py
+-rw-r--r--   0        0        0     2635 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/open_api.py
+-rw-r--r--   0        0        0     6422 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/operation.py
+-rw-r--r--   0        0        0     8047 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/parameter.py
+-rw-r--r--   0        0        0     4930 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/path_item.py
+-rw-r--r--   0        0        0     1017 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/paths.py
+-rw-r--r--   0        0        0      894 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/reference.py
+-rw-r--r--   0        0        0     3209 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/request_body.py
+-rw-r--r--   0        0        0     3719 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/response.py
+-rw-r--r--   0        0        0     2050 2023-05-21 16:07:20.035070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/responses.py
+-rw-r--r--   0        0        0    22285 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/schema.py
+-rw-r--r--   0        0        0     1325 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/security_requirement.py
+-rw-r--r--   0        0        0     3545 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/security_scheme.py
+-rw-r--r--   0        0        0     1889 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/server.py
+-rw-r--r--   0        0        0     1071 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/server_variable.py
+-rw-r--r--   0        0        0      887 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/tag.py
+-rw-r--r--   0        0        0     5464 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/util.py
+-rw-r--r--   0        0        0     1850 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/xml.py
+-rw-r--r--   0        0        0     1663 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/README.md
+-rw-r--r--   0        0        0     1898 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/__init__.py
+-rw-r--r--   0        0        0      806 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/callback.py
+-rw-r--r--   0        0        0     5650 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/components.py
+-rw-r--r--   0        0        0      861 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/contact.py
+-rw-r--r--   0        0        0      238 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/datatype.py
+-rw-r--r--   0        0        0     1282 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/discriminator.py
+-rw-r--r--   0        0        0     3573 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/encoding.py
+-rw-r--r--   0        0        0     1633 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/example.py
+-rw-r--r--   0        0        0      729 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/external_documentation.py
+-rw-r--r--   0        0        0     1076 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/header.py
+-rw-r--r--   0        0        0     2112 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/info.py
+-rw-r--r--   0        0        0     1028 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/license.py
+-rw-r--r--   0        0        0     3038 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/link.py
+-rw-r--r--   0        0        0     3060 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/media_type.py
+-rw-r--r--   0        0        0     2306 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/oauth_flow.py
+-rw-r--r--   0        0        0      835 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/oauth_flows.py
+-rw-r--r--   0        0        0     3500 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/open_api.py
+-rw-r--r--   0        0        0     6704 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/operation.py
+-rw-r--r--   0        0        0     8049 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/parameter.py
+-rw-r--r--   0        0        0     5010 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/path_item.py
+-rw-r--r--   0        0        0     1040 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/paths.py
+-rw-r--r--   0        0        0     1463 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/reference.py
+-rw-r--r--   0        0        0     3209 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/request_body.py
+-rw-r--r--   0        0        0     3545 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/response.py
+-rw-r--r--   0        0        0     2048 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/responses.py
+-rw-r--r--   0        0        0    38873 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/schema.py
+-rw-r--r--   0        0        0     1434 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/security_requirement.py
+-rw-r--r--   0        0        0     3932 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/security_scheme.py
+-rw-r--r--   0        0        0     1890 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/server.py
+-rw-r--r--   0        0        0     1069 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/server_variable.py
+-rw-r--r--   0        0        0      887 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/tag.py
+-rw-r--r--   0        0        0     1962 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/xml.py
+-rw-r--r--   0        0        0     1222 2023-05-21 16:07:20.039070 openapi_pydantic-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8948 1970-01-01 00:00:00.000000 openapi_pydantic-0.1.1/PKG-INFO
```

### Comparing `openapi_pydantic-0.1.0/LICENSE` & `openapi_pydantic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/README.md` & `openapi_pydantic-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/__init__.py` & `openapi_pydantic-0.1.1/openapi_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/util.py` & `openapi_pydantic-0.1.1/openapi_pydantic/util.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/__init__.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/README.md` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/README.md`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/__init__.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,42 +2,43 @@
 OpenAPI v3.0.3 schema types, created according to the specification:
 https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.3.md
 
 The type orders are according to the contents of the specification:
 https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.3.md#table-of-contents
 """
 
-from .open_api import OpenAPI as OpenAPI
-from .info import Info as Info
-from .contact import Contact as Contact
-from .license import License as License
-from .server import Server as Server
-from .server_variable import ServerVariable as ServerVariable
+from .callback import Callback as Callback
 from .components import Components as Components
-from .paths import Paths as Paths
-from .path_item import PathItem as PathItem
-from .operation import Operation as Operation
-from .external_documentation import ExternalDocumentation as ExternalDocumentation
-from .parameter import Parameter as Parameter, ParameterLocation as ParameterLocation
-from .request_body import RequestBody as RequestBody
-from .media_type import MediaType as MediaType
+from .contact import Contact as Contact
+from .discriminator import Discriminator as Discriminator
 from .encoding import Encoding as Encoding
-from .responses import Responses as Responses
-from .response import Response as Response
-from .callback import Callback as Callback
 from .example import Example as Example
-from .link import Link as Link
+from .external_documentation import ExternalDocumentation as ExternalDocumentation
 from .header import Header as Header
-from .tag import Tag as Tag
+from .info import Info as Info
+from .license import License as License
+from .link import Link as Link
+from .media_type import MediaType as MediaType
+from .oauth_flow import OAuthFlow as OAuthFlow
+from .oauth_flows import OAuthFlows as OAuthFlows
+from .open_api import OpenAPI as OpenAPI
+from .operation import Operation as Operation
+from .parameter import Parameter as Parameter
+from .parameter import ParameterLocation as ParameterLocation
+from .path_item import PathItem as PathItem
+from .paths import Paths as Paths
 from .reference import Reference as Reference
+from .request_body import RequestBody as RequestBody
+from .response import Response as Response
+from .responses import Responses as Responses
 from .schema import Schema as Schema
-from .discriminator import Discriminator as Discriminator
-from .xml import XML as XML
-from .security_scheme import SecurityScheme as SecurityScheme
-from .oauth_flows import OAuthFlows as OAuthFlows
-from .oauth_flow import OAuthFlow as OAuthFlow
 from .security_requirement import SecurityRequirement as SecurityRequirement
-
+from .security_scheme import SecurityScheme as SecurityScheme
+from .server import Server as Server
+from .server_variable import ServerVariable as ServerVariable
+from .tag import Tag as Tag
+from .xml import XML as XML
 
 # resolve forward references
 Encoding.update_forward_refs(Header=Header)
 Schema.update_forward_refs()
+Operation.update_forward_refs(PathItem=PathItem)
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/callback.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/callback.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/components.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/components.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/contact.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/contact.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Optional
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import BaseModel, Extra
 
 
 class Contact(BaseModel):
     """
     Contact information for the exposed API.
     """
 
     name: Optional[str] = None
     """
     The identifying name of the contact person/organization.
     """
 
-    url: Optional[AnyUrl] = None
+    url: Optional[str] = None
     """
     The URL pointing to the contact information.
     MUST be in the format of a URL.
     """
 
     email: Optional[str] = None
     """
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/discriminator.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/discriminator.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/encoding.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/encoding.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/example.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/example.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/external_documentation.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/external_documentation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Optional
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import BaseModel, Extra
 
 
 class ExternalDocumentation(BaseModel):
     """Allows referencing an external resource for extended documentation."""
 
     description: Optional[str] = None
     """
     A short description of the target documentation.
     [CommonMark syntax](https://spec.commonmark.org/) MAY be used for rich text 
     representation.
     """
 
-    url: AnyUrl
+    url: str
     """
     **REQUIRED**. The URL for the target documentation.
     Value MUST be in the format of a URL.
     """
 
     class Config:
         extra = Extra.allow
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/header.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/header.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/info.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import BaseModel, Extra
 
 from .contact import Contact
 from .license import License
 
 
 class Info(BaseModel):
     """
@@ -21,15 +21,15 @@
     description: Optional[str] = None
     """
     A short description of the API.
     [CommonMark syntax](https://spec.commonmark.org/) MAY be used for rich text 
     representation.
     """
 
-    termsOfService: Optional[AnyUrl] = None
+    termsOfService: Optional[str] = None
     """
     A URL to the Terms of Service for the API.
     MUST be in the format of a URL.
     """
 
     contact: Optional[Contact] = None
     """
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/license.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/license.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Optional
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import BaseModel, Extra
 
 
 class License(BaseModel):
     """
     License information for the exposed API.
     """
 
     name: str
     """
     **REQUIRED**. The license name used for the API.
     """
 
-    url: Optional[AnyUrl] = None
+    url: Optional[str] = None
     """
     A URL to the license used for the API.
     MUST be in the format of a URL.
     """
 
     class Config:
         extra = Extra.allow
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/link.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/link.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/media_type.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/media_type.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/oauth_flow.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/oauth_flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from typing import Dict, Optional, Union
+from typing import Dict, Optional
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import BaseModel, Extra
 
 
 class OAuthFlow(BaseModel):
     """
     Configuration details for a supported OAuth Flow
     """
 
-    authorizationUrl: Optional[Union[AnyUrl, str]] = None
+    authorizationUrl: Optional[str] = None
     """
     **REQUIRED** for `oauth2 ("implicit", "authorizationCode")`.
     The authorization URL to be used for this flow.
     This MUST be in the form of a URL.
     """
 
-    tokenUrl: Optional[Union[AnyUrl, str]] = None
+    tokenUrl: Optional[str] = None
     """
     **REQUIRED** for `oauth2 ("password", "clientCredentials", "authorizationCode")`.
     The token URL to be used for this flow.
     This MUST be in the form of a URL.
     """
 
-    refreshUrl: Optional[Union[AnyUrl, str]] = None
+    refreshUrl: Optional[str] = None
     """
     The URL to be used for obtaining refresh tokens. This MUST be in the form of a URL.
     """
 
     scopes: Dict[str, str]
     """
     **REQUIRED**. The available scopes for the OAuth2 security scheme.
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/oauth_flows.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/open_api.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/open_api.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/operation.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/parameter.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/parameter.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/path_item.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/path_item.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/paths.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/paths.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/reference.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/reference.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/request_body.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/request_body.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/response.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/response.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/responses.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/responses.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/schema.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/schema.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/security_requirement.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/security_requirement.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/security_scheme.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/security_scheme.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Optional, Union
+from typing import Optional
 
-from pydantic import AnyUrl, BaseModel, Extra, Field
+from pydantic import BaseModel, Extra, Field
 
 from .oauth_flows import OAuthFlows
 
 
 class SecurityScheme(BaseModel):
     """
     Defines a security scheme that can be used by the operations.
@@ -59,15 +59,15 @@
 
     flows: Optional[OAuthFlows] = None
     """
     **REQUIRED** for `oauth2`. An object containing configuration information for the 
     flow types supported.
     """
 
-    openIdConnectUrl: Optional[Union[AnyUrl, str]] = None
+    openIdConnectUrl: Optional[str] = None
     """
     **REQUIRED** for `openIdConnect`. OpenId Connect URL to discover OAuth2 
     configuration values. This MUST be in the form of a URL.
     """
 
     class Config:
         extra = Extra.allow
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/server.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/server.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/server_variable.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/server_variable.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/tag.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/tag.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/util.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/util.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_0_3/xml.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_0_3/xml.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/README.md` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/README.md`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/__init__.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,41 +2,43 @@
 OpenAPI v3.1.0 schema types, created according to the specification:
 https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.1.0.md
 
 The type orders are according to the contents of the specification:
 https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.1.0.md#table-of-contents
 """
 
-from .open_api import OpenAPI as OpenAPI
-from .info import Info as Info
-from .contact import Contact as Contact
-from .license import License as License
-from .server import Server as Server
-from .server_variable import ServerVariable as ServerVariable
+from .callback import Callback as Callback
 from .components import Components as Components
-from .paths import Paths as Paths
-from .path_item import PathItem as PathItem
-from .operation import Operation as Operation
-from .external_documentation import ExternalDocumentation as ExternalDocumentation
-from .parameter import Parameter as Parameter, ParameterLocation as ParameterLocation
-from .request_body import RequestBody as RequestBody
-from .media_type import MediaType as MediaType
+from .contact import Contact as Contact
+from .discriminator import Discriminator as Discriminator
 from .encoding import Encoding as Encoding
-from .responses import Responses as Responses
-from .response import Response as Response
-from .callback import Callback as Callback
 from .example import Example as Example
-from .link import Link as Link
+from .external_documentation import ExternalDocumentation as ExternalDocumentation
 from .header import Header as Header
-from .tag import Tag as Tag
+from .info import Info as Info
+from .license import License as License
+from .link import Link as Link
+from .media_type import MediaType as MediaType
+from .oauth_flow import OAuthFlow as OAuthFlow
+from .oauth_flows import OAuthFlows as OAuthFlows
+from .open_api import OpenAPI as OpenAPI
+from .operation import Operation as Operation
+from .parameter import Parameter as Parameter
+from .parameter import ParameterLocation as ParameterLocation
+from .path_item import PathItem as PathItem
+from .paths import Paths as Paths
 from .reference import Reference as Reference
+from .request_body import RequestBody as RequestBody
+from .response import Response as Response
+from .responses import Responses as Responses
 from .schema import Schema as Schema
-from .discriminator import Discriminator as Discriminator
-from .xml import XML as XML
-from .security_scheme import SecurityScheme as SecurityScheme
-from .oauth_flows import OAuthFlows as OAuthFlows
-from .oauth_flow import OAuthFlow as OAuthFlow
 from .security_requirement import SecurityRequirement as SecurityRequirement
+from .security_scheme import SecurityScheme as SecurityScheme
+from .server import Server as Server
+from .server_variable import ServerVariable as ServerVariable
+from .tag import Tag as Tag
+from .xml import XML as XML
 
 # resolve forward references
 Encoding.update_forward_refs(Header=Header)
 Schema.update_forward_refs()
+Operation.update_forward_refs(PathItem=PathItem)
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/callback.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/callback.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/components.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/components.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/contact.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/contact.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Optional
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import BaseModel, Extra
 
 
 class Contact(BaseModel):
     """
     Contact information for the exposed API.
     """
 
     name: Optional[str] = None
     """
     The identifying name of the contact person/organization.
     """
 
-    url: Optional[AnyUrl] = None
+    url: Optional[str] = None
     """
     The URL pointing to the contact information.
     MUST be in the form of a URL.
     """
 
     email: Optional[str] = None
     """
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/discriminator.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/discriminator.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/encoding.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/encoding.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/example.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/example.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/external_documentation.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/external_documentation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Optional
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import BaseModel, Extra
 
 
 class ExternalDocumentation(BaseModel):
     """Allows referencing an external resource for extended documentation."""
 
     description: Optional[str] = None
     """
     A short description of the target documentation.
     [CommonMark syntax](https://spec.commonmark.org/) MAY be used for rich text 
     representation.
     """
 
-    url: AnyUrl
+    url: str
     """
     **REQUIRED**. The URL for the target documentation.
     Value MUST be in the form of a URL.
     """
 
     class Config:
         extra = Extra.allow
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/header.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/header.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/info.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import BaseModel, Extra
 
 from .contact import Contact
 from .license import License
 
 
 class Info(BaseModel):
     """
@@ -26,15 +26,15 @@
     description: Optional[str] = None
     """
     A description of the API.
     [CommonMark syntax](https://spec.commonmark.org/) MAY be used for rich text 
     representation.
     """
 
-    termsOfService: Optional[AnyUrl] = None
+    termsOfService: Optional[str] = None
     """
     A URL to the Terms of Service for the API.
     MUST be in the form of a URL.
     """
 
     contact: Optional[Contact] = None
     """
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/license.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/license.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import BaseModel, Extra
 
 
 class License(BaseModel):
     """
     License information for the exposed API.
     """
 
@@ -16,15 +16,15 @@
     identifier: Optional[str] = None
     """
     An [SPDX](https://spdx.org/spdx-specification-21-web-version#h.jxpfx0ykyb60) 
     license expression for the API. The `identifier` field is mutually exclusive of the 
     `url` field.
     """
 
-    url: Optional[AnyUrl] = None
+    url: Optional[str] = None
     """
     A URL to the license used for the API.
     This MUST be in the form of a URL.
     The `url` field is mutually exclusive of the `identifier` field.
     """
 
     class Config:
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/link.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/link.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/media_type.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/media_type.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/oauth_flow.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/oauth_flow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from typing import Dict, Optional, Union
+from typing import Dict, Optional
 
-from pydantic import AnyUrl, BaseModel, Extra
+from pydantic import BaseModel, Extra
 
 
 class OAuthFlow(BaseModel):
     """
     Configuration details for a supported OAuth Flow
     """
 
-    authorizationUrl: Optional[Union[AnyUrl, str]] = None
+    authorizationUrl: Optional[str] = None
     """
     **REQUIRED** for `oauth2 ("implicit", "authorizationCode")`.
     The authorization URL to be used for this flow.
     This MUST be in the form of a URL.
     The OAuth2 standard requires the use of TLS.
     """
 
-    tokenUrl: Optional[Union[AnyUrl, str]] = None
+    tokenUrl: Optional[str] = None
     """
     **REQUIRED** for `oauth2 ("password", "clientCredentials", "authorizationCode")`.
     The token URL to be used for this flow.
     This MUST be in the form of a URL.
     The OAuth2 standard requires the use of TLS.
     """
 
-    refreshUrl: Optional[Union[AnyUrl, str]] = None
+    refreshUrl: Optional[str] = None
     """
     The URL to be used for obtaining refresh tokens.
     This MUST be in the form of a URL.
     The OAuth2 standard requires the use of TLS.
     """
 
     scopes: Optional[Dict[str, str]] = None
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/oauth_flows.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/open_api.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/open_api.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/operation.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/parameter.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/parameter.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/path_item.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/path_item.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/paths.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/paths.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/reference.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/reference.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/request_body.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/request_body.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/response.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/response.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/responses.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/responses.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/schema.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/schema.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/security_requirement.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/security_requirement.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/security_scheme.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/security_scheme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Optional, Union
+from typing import Optional
 
-from pydantic import AnyUrl, BaseModel, Extra, Field
+from pydantic import BaseModel, Extra, Field
 
 from .oauth_flows import OAuthFlows
 
 
 class SecurityScheme(BaseModel):
     """
     Defines a security scheme that can be used by the operations.
@@ -65,15 +65,15 @@
 
     flows: Optional[OAuthFlows] = None
     """
     **REQUIRED** for `oauth2`. An object containing configuration information for the 
     flow types supported.
     """
 
-    openIdConnectUrl: Optional[Union[AnyUrl, str]] = None
+    openIdConnectUrl: Optional[str] = None
     """
     **REQUIRED** for `openIdConnect`. OpenId Connect URL to discover OAuth2 
     configuration values. This MUST be in the form of a URL. The OpenID Connect 
     standard requires the use of TLS.
     """
 
     class Config:
```

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/server.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/server.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/server_variable.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/server_variable.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/tag.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/tag.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/openapi_pydantic/v3/v3_1_0/xml.py` & `openapi_pydantic-0.1.1/openapi_pydantic/v3/v3_1_0/xml.py`

 * *Files identical despite different names*

### Comparing `openapi_pydantic-0.1.0/pyproject.toml` & `openapi_pydantic-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-pydantic"
-version = "0.1.0"
+version = "0.1.1"
 description = "Pydantic OpenAPI schema implementation"
 authors = ["Mike Oakley <mike-oakley@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/mike-oakley/openapi-pydantic"
 license = "MIT"
 keywords = [
   "openapi",
```

### Comparing `openapi_pydantic-0.1.0/PKG-INFO` & `openapi_pydantic-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-pydantic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pydantic OpenAPI schema implementation
 Home-page: https://github.com/mike-oakley/openapi-pydantic
 License: MIT
 Keywords: openapi,schema,parser,pydantic,validation
 Author: Mike Oakley
 Author-email: mike-oakley@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

