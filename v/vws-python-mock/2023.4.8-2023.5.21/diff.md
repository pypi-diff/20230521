# Comparing `tmp/vws-python-mock-2023.4.8.tar.gz` & `tmp/vws-python-mock-2023.5.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vws-python-mock-2023.4.8.tar", last modified: Sat Apr  8 18:21:20 2023, max compression
+gzip compressed data, was "vws-python-mock-2023.5.21.tar", last modified: Sun May 21 17:56:14 2023, max compression
```

## Comparing `vws-python-mock-2023.4.8.tar` & `vws-python-mock-2023.5.21.tar`

### file list

```diff
@@ -1,158 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.432574 vws-python-mock-2023.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.408573 vws-python-mock-2023.4.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.408573 vws-python-mock-2023.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.github/workflows/docker-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.github/workflows/windows-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.408573 vws-python-mock-2023.4.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-08 18:21:02.000000 vws-python-mock-2023.4.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-08 18:21:20.432574 vws-python-mock-2023.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.408573 vws-python-mock-2023.4.8/ci/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/ci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/ci/custom_linters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/ci/decrypt_secret.sh
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/ci/set_secrets_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/doc8.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.408573 vws-python-mock-2023.4.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.412573 vws-python-mock-2023.4.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/basic-example.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/ci-setup.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2569 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/differences-to-vws.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/docker.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/mock-api-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/release-process.rst
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/versioning-and-api-stability.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/lint.mk
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/secrets.tar.gpg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 18:21:20.432574 vws-python-mock-2023.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/spelling_private_dict.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.404573 vws-python-mock-2023.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.416574 vws-python-mock-2023.4.8/src/mock_vws/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_base64_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_database_matchers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.416574 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.404573 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.416574 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/target_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/target_manager/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.416574 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/vwq/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/vwq/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.416574 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/vws/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/vws/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/target_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/vwq.py
--rw-r--r--   0 runner    (1001) docker     (123)    20085 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/vws.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_mock_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.420574 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/accept_header_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/auth_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/content_length_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/content_type_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/date_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    23346 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/fields_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/image_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/include_target_data_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/num_results_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/project_state_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.420574 vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/mock_web_query_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25025 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/mock_web_services_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.424574 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/active_flag_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/auth_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/content_length_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/content_type_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/date_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17325 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/image_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/json_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/key_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/metadata_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/name_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/project_state_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/target_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/width_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/image_matchers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.424574 vws-python-mock-2023.4.8/src/mock_vws/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/resources/deleted_target_matched_response.html
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/resources/oops_error_occurred_response.html
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/target_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/target_raters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.424574 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-08 18:21:20.000000 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-08 18:21:20.000000 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:21:20.000000 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:21:19.000000 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-08 18:21:20.000000 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-08 18:21:20.000000 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.424574 vws-python-mock-2023.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.428574 vws-python-mock-2023.4.8/tests/mock_vws/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.428574 vws-python-mock-2023.4.8/tests/mock_vws/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/fixtures/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/fixtures/prepared_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/fixtures/vuforia_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/jetty_error_deletion_not_complete.html
--rw-r--r--   0 runner    (1001) docker     (123)    32560 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_add_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_authorization_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_content_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    13101 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_database_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_date_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_delete_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_flask_app_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_get_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_get_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_invalid_given_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_invalid_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    69389 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    28210 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_requests_mock_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_target_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_target_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_unexpected_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    29397 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_update_target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.432574 vws-python-mock-2023.4.8/tests/mock_vws/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/utils/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/utils/usage_test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/vuforia_secrets.env.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.276282 vws-python-mock-2023.5.21/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.248282 vws-python-mock-2023.5.21/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.248282 vws-python-mock-2023.5.21/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/.github/workflows/docker-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/.github/workflows/windows-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.248282 vws-python-mock-2023.5.21/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-21 17:56:00.000000 vws-python-mock-2023.5.21/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-21 17:56:14.276282 vws-python-mock-2023.5.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.248282 vws-python-mock-2023.5.21/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/ci/custom_linters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/ci/decrypt_secret.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/ci/set_secrets_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/doc8.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.252282 vws-python-mock-2023.5.21/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.252282 vws-python-mock-2023.5.21/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/basic-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/ci-setup.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2569 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/differences-to-vws.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/mock-api-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/release-process.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/docs/source/versioning-and-api-stability.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/lint.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/secrets.tar.gpg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 17:56:14.276282 vws-python-mock-2023.5.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/spelling_private_dict.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.240282 vws-python-mock-2023.5.21/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.256282 vws-python-mock-2023.5.21/src/mock_vws/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_base64_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_database_matchers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.256282 vws-python-mock-2023.5.21/src/mock_vws/_flask_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_flask_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.240282 vws-python-mock-2023.5.21/src/mock_vws/_flask_server/dockerfiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.260282 vws-python-mock-2023.5.21/src/mock_vws/_flask_server/dockerfiles/target_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_flask_server/dockerfiles/target_manager/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.260282 vws-python-mock-2023.5.21/src/mock_vws/_flask_server/dockerfiles/vwq/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_flask_server/dockerfiles/vwq/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.260282 vws-python-mock-2023.5.21/src/mock_vws/_flask_server/dockerfiles/vws/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_flask_server/dockerfiles/vws/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_flask_server/target_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_flask_server/vwq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_flask_server/vws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_mock_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_query_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.264282 vws-python-mock-2023.5.21/src/mock_vws/_query_validators/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_query_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_query_validators/accept_header_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_query_validators/auth_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_query_validators/content_length_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_query_validators/content_type_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_query_validators/date_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21805 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_query_validators/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_query_validators/fields_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_query_validators/image_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_query_validators/include_target_data_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_query_validators/num_results_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_query_validators/project_state_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.264282 vws-python-mock-2023.5.21/src/mock_vws/_requests_mock_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_requests_mock_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_requests_mock_server/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_requests_mock_server/mock_web_query_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25025 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_requests_mock_server/mock_web_services_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.268282 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/active_flag_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/auth_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/content_length_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/content_type_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/date_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17325 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/image_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/json_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/key_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/metadata_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/name_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/project_state_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/target_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/_services_validators/width_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/image_matchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.268282 vws-python-mock-2023.5.21/src/mock_vws/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/resources/deleted_target_matched_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/resources/oops_error_occurred_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/target_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/src/mock_vws/target_raters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.268282 vws-python-mock-2023.5.21/src/vws_python_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-21 17:56:14.000000 vws-python-mock-2023.5.21/src/vws_python_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-21 17:56:14.000000 vws-python-mock-2023.5.21/src/vws_python_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:56:14.000000 vws-python-mock-2023.5.21/src/vws_python_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:56:13.000000 vws-python-mock-2023.5.21/src/vws_python_mock.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-21 17:56:14.000000 vws-python-mock-2023.5.21/src/vws_python_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 17:56:14.000000 vws-python-mock-2023.5.21/src/vws_python_mock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.272282 vws-python-mock-2023.5.21/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.276282 vws-python-mock-2023.5.21/tests/mock_vws/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.276282 vws-python-mock-2023.5.21/tests/mock_vws/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/fixtures/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/fixtures/prepared_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/fixtures/vuforia_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32560 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_add_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_authorization_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_content_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13101 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_database_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_date_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_delete_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_flask_app_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_get_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_get_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_invalid_given_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_invalid_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65910 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23244 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_requests_mock_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_target_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_target_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_unexpected_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29397 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/test_update_target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:14.276282 vws-python-mock-2023.5.21/tests/mock_vws/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/utils/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/tests/mock_vws/utils/usage_test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-21 17:55:58.000000 vws-python-mock-2023.5.21/vuforia_secrets.env.example
```

### Comparing `vws-python-mock-2023.4.8/.github/workflows/ci.yml` & `vws-python-mock-2023.5.21/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/.github/workflows/docker-build.yml` & `vws-python-mock-2023.5.21/.github/workflows/docker-build.yml`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/.github/workflows/lint.yml` & `vws-python-mock-2023.5.21/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/.github/workflows/release.yml` & `vws-python-mock-2023.5.21/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/.github/workflows/windows-ci.yml` & `vws-python-mock-2023.5.21/.github/workflows/windows-ci.yml`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/.gitignore` & `vws-python-mock-2023.5.21/.gitignore`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/CHANGELOG.rst` & `vws-python-mock-2023.5.21/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Changelog
 =========
 
 Next
 ----
 
+2023.05.21
+------------
+
 2023.04.08
 ------------
 
 2023.03.26
 ------------
 
 2023.03.05
```

### Comparing `vws-python-mock-2023.4.8/CODE_OF_CONDUCT.rst` & `vws-python-mock-2023.5.21/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/LICENSE` & `vws-python-mock-2023.5.21/LICENSE`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/Makefile` & `vws-python-mock-2023.5.21/Makefile`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/PKG-INFO` & `vws-python-mock-2023.5.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vws-python-mock
-Version: 2023.4.8
+Version: 2023.5.21
 Summary: A mock for the Vuforia Web Services (VWS) API.
 Author-email: Adam Dangoor <adamdangoor@gmail.com>
 License: The MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `vws-python-mock-2023.4.8/README.rst` & `vws-python-mock-2023.5.21/README.rst`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/ci/custom_linters.py` & `vws-python-mock-2023.5.21/ci/custom_linters.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/ci/set_secrets_file.py` & `vws-python-mock-2023.5.21/ci/set_secrets_file.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/docs/Makefile` & `vws-python-mock-2023.5.21/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/docs/source/basic-example.rst` & `vws-python-mock-2023.5.21/docs/source/basic-example.rst`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/docs/source/ci-setup.rst` & `vws-python-mock-2023.5.21/docs/source/ci-setup.rst`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/docs/source/conf.py` & `vws-python-mock-2023.5.21/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/docs/source/contributing.rst` & `vws-python-mock-2023.5.21/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/docs/source/differences-to-vws.rst` & `vws-python-mock-2023.5.21/docs/source/differences-to-vws.rst`

 * *Files 8% similar despite different names*

```diff
@@ -33,29 +33,14 @@
 This is customizable with the :paramref:`~mock_vws.MockVWS.target_tracking_rater` parameter.
 
 Image targets which are not suited to detection are given 'failed' statuses.
 The criteria for these images is not defined by the Vuforia documentation.
 The mock is more forgiving than the real Vuforia Web Services.
 Therefore, an image given a 'success' status by the mock may not be given a 'success' status by the real Vuforia Web Services.
 
-Matching targets in the processing state
-----------------------------------------
-
-Matching a target which is in the processing state sometimes returns a successful response with no results.
-Sometimes a 500 (``INTERNAL SERVER ERROR``) response is given.
-The mock always gives a 500 response.
-
-Matching deleted targets
-------------------------
-
-Matching a target which has been deleted returns a 500 (``INTERNAL SERVER ERROR``) response within the first few seconds.
-This time frame is not consistent on the real Vuforia Web Services.
-On the mock, this time frame is three seconds by default.
-:py:class:`~mock_vws.MockVWS` takes a parameter :paramref:`~mock_vws.MockVWS.query_processes_deletion_seconds` to change this.
-
 Accepted date formats for the Query API
 ---------------------------------------
 
 The Query API documentation is not clear on which date formats are expected exactly in the ``Date`` header.
 The mock is strict.
 That is, it accepts only a few date formats, and rejects all others.
 If you find a date format which is accepted by the real Query API but rejected by the mock, please create a GitHub issue.
```

### Comparing `vws-python-mock-2023.4.8/docs/source/docker.rst` & `vws-python-mock-2023.5.21/docs/source/docker.rst`

 * *Files 4% similar despite different names*

```diff
@@ -114,28 +114,14 @@
    * ``random``: The rating is random.
 
    Default: ``brisque``
 
 Query container
 ~~~~~~~~~~~~~~~
 
-.. envvar:: DELETION_PROCESSING_SECONDS
-
-   The number of seconds after a target deletion is recognized that the
-   query endpoint will return a 500 response on a match.
-
-   Default: 3.0
-
-.. envvar:: DELETION_RECOGNITION_SECONDS
-
-   The number of seconds after a target has been deleted that the query
-   endpoint will still recognize the target for.
-
-   Default: 2.0
-
 .. envvar:: QUERY_IMAGE_MATCHER
 
    The matcher to use for the query endpoint.
 
    Options include:
 
    * ``exact``: The images must be exactly the same to match.
```

### Comparing `vws-python-mock-2023.4.8/docs/source/index.rst` & `vws-python-mock-2023.5.21/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/docs/source/mock-api-reference.rst` & `vws-python-mock-2023.5.21/docs/source/mock-api-reference.rst`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/lint.mk` & `vws-python-mock-2023.5.21/lint.mk`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/pyproject.toml` & `vws-python-mock-2023.5.21/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,21 @@
 
 line-length = 79
 
 [tool.coverage.run]
 
 branch = true
 
+[tool.coverage.report]
+
+exclude_lines =  [
+  "pragma: no cover",
+  "if TYPE_CHECKING:",
+]
+
 [tool.pytest.ini_options]
 
 xfail_strict = true
 log_cli = true
 addopts = ["--strict-markers"]
 markers = ["requires_docker_build"]
 
@@ -140,14 +147,15 @@
 [[tool.mypy.overrides]]
 
 module = [
     "brisque",
     "cv2",
     "docker",
     "docker.errors",
+    "docker.models.containers",
     "docker.models.networks",
     "multipart",
     "sybil",
     "sybil.parsers.rest",
 ]
 
 ignore_missing_imports = true
@@ -207,14 +215,15 @@
     "D407",
     # We have an existing interface to support and so we do not want to change
     # exception names.
     "N818",
     # Ignore "too-many-*" errors as they seem to get in the way more than
     # helping.
     "PLR0913",
+    "PLR0915",
     # Allow 'assert' in tests as it is the standard for pytest.
     # Also, allow 'assert' in other code as it is the standard for Python type hint
     # narrowing - see
     # https://mypy.readthedocs.io/en/stable/type_narrowing.html#type-narrowing-expressions.
     "S101",
     # Allow `random` as we are not implementing something which needs cryptographic safety.
     "S311",
@@ -264,57 +273,59 @@
     "numpy",
     "opencv-python",
     "pydantic",
     "requests",
     "requests-mock",
     "tzdata; sys_platform == 'win32'",
     "vws-auth-tools",
-    "werkzeug",
 ]
 
 [project.optional-dependencies]
 dev = [
     "PyYAML==6.0",
     "Sphinx-Substitution-Extensions==2022.2.16",
-    "Sphinx==6.1.3",
+    "Sphinx==7.0.1",
     "VWS-Test-Fixtures==2023.3.5",
     "black==23.3.0",
     "check-manifest==0.49",
-    "dirty-equals==0.5.0",
+    "dirty-equals==0.6.0",
     # We pin to an old doc8 to avoid version conflicts with sphinx_toolbox.
     # When we bump this, we can remove doc8.ini.
     "doc8==0.11.2",
-    "docker==6.0.1",
+    "docker==6.1.2",
     "dodgy==0.2.1",
     "enum-tools[sphinx]==0.9.0.post1",
     "freezegun==1.2.2",
-    "furo==2023.3.27",
-    "mypy==1.2.0",
-    "pdm==2.4.9",
+    "furo==2023.5.20",
+    "mypy==1.3.0",
+    "pdm==2.6.1",
     "pip_check_reqs==2.4.4",
     "pydocstyle==6.3.0",
     "pyenchant==3.2.2",
-    "pylint==2.17.2",
-    "pyright==1.1.302",
+    "pylint==2.17.4",
+    "pyright==1.1.309",
     "pyroma==4.2",
     "pytest-cov==4.0.0",
-    "pytest==7.2.2",
-    "requests-mock-flask==2023.3.5.1",
-    "ruff==0.0.261",
-    "sphinx-autodoc-typehints==1.22",
+    "pytest==7.3.1",
+    "requests-mock-flask==2023.5.14",
+    "ruff==0.0.269",
+    "sphinx-autodoc-typehints==1.23.0",
     "sphinx-prompt==1.5.0",
     "sphinx_paramlinks==0.5.4",
     "sphinxcontrib-httpdomain==1.8.1",
     "sphinxcontrib-spelling==8.0.0",
     "sphinx-toolbox==3.4.0",
-    "sybil==5.0.0",
+    "sybil==5.0.2",
     "types-PyYAML==6.0.12.9",
-    "types-Pillow==9.4.0.19",
-    "types-requests==2.28.11.17",
-    "types-urllib3==1.26.25.10",
+    "types-Pillow==9.5.0.4",
+    "types-requests==2.30.0.0",
+    # We need urllib3 < 2.0.0 for pdm to work.
+    # After we can bump urllib3, we can remove types-urllib.
+    "types-urllib3==1.26.25.13",
+    "urllib3<2.0.0",
     "vulture==2.7",
     "vws-python==2023.3.25",
 ]
 
 [project.urls]
 Source = "https://github.com/VWS-Python/vws-python-mock"
 Documentation = "https://vws-python-mock.readthedocs.io"
```

### Comparing `vws-python-mock-2023.4.8/secrets.tar.gpg` & `vws-python-mock-2023.5.21/secrets.tar.gpg`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/spelling_private_dict.txt` & `vws-python-mock-2023.5.21/spelling_private_dict.txt`

 * *Files 14% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 pytest
 readme
 readthedocs
 recognitions
 refactoring
 regex
 reimplementation
+reportGeneralTypeIssues
 repr
 reqheader
 reqjson
 reqjsonarr
 resheader
 resjson
 resjsonarr
```

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_base64_decoding.py` & `vws-python-mock-2023.5.21/src/mock_vws/_base64_decoding.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_constants.py` & `vws-python-mock-2023.5.21/src/mock_vws/_constants.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_database_matchers.py` & `vws-python-mock-2023.5.21/src/mock_vws/_database_matchers.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_flask_server/target_manager.py` & `vws-python-mock-2023.5.21/src/mock_vws/_flask_server/target_manager.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_flask_server/vwq.py` & `vws-python-mock-2023.5.21/src/mock_vws/_flask_server/vwq.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,23 +8,20 @@
 import email.utils
 from enum import StrEnum, auto
 from http import HTTPStatus
 
 import requests
 from flask import Flask, Response, request
 from pydantic import BaseSettings
-from werkzeug.datastructures import Headers
 
 from mock_vws._query_tools import (
-    ActiveMatchingTargetsDeleteProcessing,
     get_query_match_response_text,
 )
 from mock_vws._query_validators import run_query_validators
 from mock_vws._query_validators.exceptions import (
-    DeletedTargetMatched,
     ValidatorException,
 )
 from mock_vws.database import VuforiaDatabase
 from mock_vws.image_matchers import (
     AverageHashMatcher,
     ExactMatcher,
     ImageMatcher,
@@ -51,16 +48,14 @@
 
 
 class VWQSettings(BaseSettings):
     """Settings for the VWQ Flask app."""
 
     vwq_host: str = ""
     target_manager_base_url: str
-    deletion_processing_seconds: float = 3.0
-    deletion_recognition_seconds: float = 2.0
     query_image_matcher: _ImageMatcherChoice = _ImageMatcherChoice.AVERAGE_HASH
 
 
 def get_all_databases() -> set[VuforiaDatabase]:
     """
     Get all database objects from the target manager back-end.
     """
@@ -78,41 +73,39 @@
 @CLOUDRECO_FLASK_APP.before_request
 def set_terminate_wsgi_input() -> None:
     """
     We set ``wsgi.input_terminated`` to ``True`` when going through
     ``requests``, so that requests have the given ``Content-Length`` headers
     and the given data in ``request.headers`` and ``request.data``.
 
-    We set this to ``False`` when running an application as standalone.
+    We do not set this at all when running an application as standalone.
     This is because when running the Flask application, if this is set,
     reading ``request.data`` hangs.
 
     Therefore, when running the real Flask application, the behavior is not the
     same as the real Vuforia.
     This is documented as a difference in the documentation for this package.
     """
-    terminate_wsgi_input = CLOUDRECO_FLASK_APP.config.get(
-        "TERMINATE_WSGI_INPUT",
-        False,
-    )
-    request.environ["wsgi.input_terminated"] = terminate_wsgi_input
+    if CLOUDRECO_FLASK_APP.config.get("TERMINATE_WSGI_INPUT") is True:
+        request.environ["wsgi.input_terminated"] = True
 
 
 @CLOUDRECO_FLASK_APP.errorhandler(ValidatorException)
 def handle_exceptions(exc: ValidatorException) -> Response:
     """
     Return the error response associated with the given exception.
     """
     response = Response(
         status=exc.status_code.value,
         response=exc.response_text,
         headers=exc.headers,
     )
 
-    response.headers = Headers(exc.headers)
+    response.headers.clear()
+    response.headers.extend(exc.headers)
     return response
 
 
 @CLOUDRECO_FLASK_APP.route("/v1/query", methods=["POST"])
 def query() -> Response:
     """
     Perform an image recognition query.
@@ -127,29 +120,22 @@
         request_body=request_body,
         request_method=request.method,
         request_path=request.path,
         databases=databases,
     )
     date = email.utils.formatdate(None, localtime=False, usegmt=True)
 
-    try:
-        response_text = get_query_match_response_text(
-            request_headers=dict(request.headers),
-            request_body=request_body,
-            request_method=request.method,
-            request_path=request.path,
-            databases=databases,
-            query_processes_deletion_seconds=settings.deletion_processing_seconds,
-            query_recognizes_deletion_seconds=(
-                settings.deletion_recognition_seconds
-            ),
-            query_match_checker=query_match_checker,
-        )
-    except ActiveMatchingTargetsDeleteProcessing as exc:
-        raise DeletedTargetMatched from exc
+    response_text = get_query_match_response_text(
+        request_headers=dict(request.headers),
+        request_body=request_body,
+        request_method=request.method,
+        request_path=request.path,
+        databases=databases,
+        query_match_checker=query_match_checker,
+    )
 
     headers = {
         "Content-Type": "application/json",
         "Date": date,
         "Connection": "keep-alive",
         "Server": "nginx",
     }
```

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_flask_server/vws.py` & `vws-python-mock-2023.5.21/src/mock_vws/_flask_server/vws.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import uuid
 from enum import StrEnum, auto
 from http import HTTPStatus
 
 import requests
 from flask import Flask, Response, request
 from pydantic import BaseSettings
-from werkzeug.datastructures import Headers
 
 from mock_vws._constants import ResultCodes, TargetStatuses
 from mock_vws._database_matchers import get_database_matching_server_keys
 from mock_vws._mock_common import json_dump
 from mock_vws._services_validators import run_services_validators
 from mock_vws._services_validators.exceptions import (
     Fail,
@@ -92,27 +91,24 @@
 @VWS_FLASK_APP.before_request
 def set_terminate_wsgi_input() -> None:
     """
     We set ``wsgi.input_terminated`` to ``True`` when going through
     ``requests``, so that requests have the given ``Content-Length`` headers
     and the given data in ``request.headers`` and ``request.data``.
 
-    We set this to ``False`` when running an application as standalone.
+    We do not set this at all when running an application as standalone.
     This is because when running the Flask application, if this is set,
     reading ``request.data`` hangs.
 
     Therefore, when running the real Flask application, the behavior is not the
     same as the real Vuforia.
     This is documented as a difference in the documentation for this package.
     """
-    terminate_wsgi_input = VWS_FLASK_APP.config.get(
-        "TERMINATE_WSGI_INPUT",
-        False,
-    )
-    request.environ["wsgi.input_terminated"] = terminate_wsgi_input
+    if VWS_FLASK_APP.config.get("TERMINATE_WSGI_INPUT") is True:
+        request.environ["wsgi.input_terminated"] = True
 
 
 @VWS_FLASK_APP.before_request
 def validate_request() -> None:
     """
     Run validators on the request.
     """
@@ -133,15 +129,16 @@
     """
     response = Response(
         status=exc.status_code.value,
         response=exc.response_text,
         headers=exc.headers,
     )
 
-    response.headers = Headers(exc.headers)
+    response.headers.clear()
+    response.headers.extend(exc.headers)
     return response
 
 
 @VWS_FLASK_APP.route("/targets", methods=["POST"])
 def add_target() -> Response:
     """
     Add a target.
```

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_mock_common.py` & `vws-python-mock-2023.5.21/src/mock_vws/_mock_common.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/__init__.py` & `vws-python-mock-2023.5.21/src/mock_vws/_query_validators/__init__.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/accept_header_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_query_validators/accept_header_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/auth_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_query_validators/auth_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/content_length_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_query_validators/content_length_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/content_type_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_query_validators/content_type_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/date_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_query_validators/date_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/exceptions.py` & `vws-python-mock-2023.5.21/src/mock_vws/_query_validators/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Exceptions to raise from validators.
 """
 
 import email.utils
 import textwrap
 import uuid
 from http import HTTPStatus
-from pathlib import Path
 
 from mock_vws._constants import ResultCodes
 from mock_vws._mock_common import json_dump
 
 
 class ValidatorException(Exception):
     """
@@ -624,53 +623,14 @@
             "Date": date,
             "Server": "nginx",
             "Content-Type": "text/html",
             "Content-Length": str(len(self.response_text)),
         }
 
 
-class DeletedTargetMatched(ValidatorException):
-    """
-    Exception raised when target which was recently deleted is matched.
-    """
-
-    def __init__(self) -> None:
-        """
-        Attributes:
-            status_code: The status code to use in a response if this is
-                raised.
-            response_text: The response text to use in a response if this is
-                raised.
-        """
-        super().__init__()
-        self.status_code = HTTPStatus.INTERNAL_SERVER_ERROR
-        date = email.utils.formatdate(None, localtime=False, usegmt=True)
-        # We return an example 500 response.
-        # Each response given by Vuforia is different.
-        #
-        # Sometimes Vuforia will ignore matching targets with the
-        # processing status, but we choose to:
-        # * Do the most unexpected thing.
-        # * Be consistent with every response.
-        resources_dir = Path(__file__).parent.parent / "resources"
-        filename = "deleted_target_matched_response.html"
-        deleted_target_matched_resp_file = resources_dir / filename
-        self.response_text = Path(deleted_target_matched_resp_file).read_text(
-            encoding="utf-8",
-        )
-        self.headers = {
-            "Connection": "keep-alive",
-            "Content-Type": "text/html;charset=iso-8859-1",
-            "Server": "nginx",
-            "Cache-Control": "must-revalidate,no-cache,no-store",
-            "Date": date,
-            "Content-Length": str(len(self.response_text)),
-        }
-
-
 class NoContentType(ValidatorException):
     """
     Exception raised when a content type is either not given or is empty.
     """
 
     def __init__(self) -> None:
         """
```

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/fields_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_query_validators/fields_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/image_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_query_validators/image_validators.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,25 +63,27 @@
     body_file = io.BytesIO(request_body)
 
     email_message = EmailMessage()
     email_message["content-type"] = request_headers["Content-Type"]
     boundary = email_message.get_boundary()
     assert isinstance(boundary, str)
     parsed = multipart.MultipartParser(stream=body_file, boundary=boundary)
-    image = parsed.get("image").raw
+    image_part = parsed.get("image")
+    assert image_part is not None
+    image_value = image_part.raw
 
     # This is the documented maximum size of a PNG as per.
     # https://library.vuforia.com/web-api/vuforia-query-web-api.
     # However, the tests show that this maximum size also applies to JPEG
     # files.
     max_bytes = 2 * 1024 * 1024
     # Ignore coverage on this as there is a bug in urllib3 which means that we
     # do not trigger this exception.
     # See https://github.com/urllib3/urllib3/issues/2733.
-    if len(image) > max_bytes:  # pragma: no cover
+    if len(image_value) > max_bytes:  # pragma: no cover
         _LOGGER.warning(msg="The image file size is too large.")
         raise RequestEntityTooLarge
 
 
 def validate_image_dimensions(
     request_headers: dict[str, str],
     request_body: bytes,
@@ -100,16 +102,18 @@
     body_file = io.BytesIO(request_body)
 
     email_message = EmailMessage()
     email_message["content-type"] = request_headers["Content-Type"]
     boundary = email_message.get_boundary()
     assert isinstance(boundary, str)
     parsed = multipart.MultipartParser(stream=body_file, boundary=boundary)
-    image = parsed.get("image").raw
-    image_file = io.BytesIO(image)
+    image_part = parsed.get("image")
+    assert image_part is not None
+    image_value = image_part.raw
+    image_file = io.BytesIO(image_value)
     pil_image = Image.open(image_file)
     max_width = 30000
     max_height = 30000
     if pil_image.height <= max_height and pil_image.width <= max_width:
         return
 
     _LOGGER.warning(msg="The image dimensions are too large.")
@@ -133,17 +137,19 @@
     body_file = io.BytesIO(request_body)
 
     email_message = EmailMessage()
     email_message["content-type"] = request_headers["Content-Type"]
     boundary = email_message.get_boundary()
     assert isinstance(boundary, str)
     parsed = multipart.MultipartParser(stream=body_file, boundary=boundary)
-    image = parsed.get("image").raw
+    image_part = parsed.get("image")
+    assert image_part is not None
+    image_value = image_part.raw
 
-    image_file = io.BytesIO(image)
+    image_file = io.BytesIO(image_value)
     pil_image = Image.open(image_file)
 
     if pil_image.format in {"PNG", "JPEG"}:
         return
 
     _LOGGER.warning(msg="The image format is not PNG or JPEG.")
     raise BadImage
@@ -166,16 +172,18 @@
     body_file = io.BytesIO(request_body)
 
     email_message = EmailMessage()
     email_message["content-type"] = request_headers["Content-Type"]
     boundary = email_message.get_boundary()
     assert isinstance(boundary, str)
     parsed = multipart.MultipartParser(stream=body_file, boundary=boundary)
-    image = parsed.get("image").raw
+    image_part = parsed.get("image")
+    assert image_part is not None
+    image_value = image_part.raw
 
-    image_file = io.BytesIO(image)
+    image_file = io.BytesIO(image_value)
 
     try:
         Image.open(image_file)
     except OSError as exc:
         _LOGGER.warning(msg="The image is not an image file.")
         raise BadImage from exc
```

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/include_target_data_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_query_validators/include_target_data_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/num_results_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_query_validators/num_results_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/project_state_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_query_validators/project_state_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/decorators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_requests_mock_server/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,16 +39,14 @@
     def __init__(
         self,
         base_vws_url: str = "https://vws.vuforia.com",
         base_vwq_url: str = "https://cloudreco.vuforia.com",
         duplicate_match_checker: ImageMatcher = _AVERAGE_HASH_MATCHER,
         query_match_checker: ImageMatcher = _AVERAGE_HASH_MATCHER,
         processing_time_seconds: int | float = 2,
-        query_recognizes_deletion_seconds: int | float = 2,
-        query_processes_deletion_seconds: int | float = 3,
         target_tracking_rater: TargetTrackingRater = _BRISQUE_TRACKING_RATER,
         *,
         real_http: bool = False,
     ) -> None:
         """
         Route requests to Vuforia's Web Service APIs to fakes of those APIs.
 
@@ -58,20 +56,14 @@
                 See
                 https://requests-mock.readthedocs.io/en/latest/mocker.html#real-http-requests.
             processing_time_seconds: The number of seconds to process each
                 image for.
                 In the real Vuforia Web Services, this is not deterministic.
             base_vwq_url: The base URL for the VWQ API.
             base_vws_url: The base URL for the VWS API.
-            query_recognizes_deletion_seconds: The number
-                of seconds after a target has been deleted that the query
-                endpoint will still recognize the target for.
-            query_processes_deletion_seconds: The number of
-                seconds after a target deletion is recognized that the query
-                endpoint will return a 500 response on a match.
             query_match_checker: A callable which takes two image values and
                 returns whether they will match in a query request.
             duplicate_match_checker: A callable which takes two image values
                 and returns whether they are duplicates.
             target_tracking_rater: A callable for rating targets for tracking.
 
         Raises:
@@ -100,20 +92,14 @@
             processing_time_seconds=processing_time_seconds,
             duplicate_match_checker=duplicate_match_checker,
             target_tracking_rater=target_tracking_rater,
         )
 
         self._mock_vwq_api = MockVuforiaWebQueryAPI(
             target_manager=self._target_manager,
-            query_processes_deletion_seconds=(
-                query_processes_deletion_seconds
-            ),
-            query_recognizes_deletion_seconds=(
-                query_recognizes_deletion_seconds
-            ),
             query_match_checker=query_match_checker,
         )
 
     def add_database(self, database: VuforiaDatabase) -> None:
         """
         Add a cloud database.
```

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/mock_web_query_api.py` & `vws-python-mock-2023.5.21/src/mock_vws/_requests_mock_server/mock_web_query_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 import email.utils
 from typing import TYPE_CHECKING
 
 from requests_mock import POST
 
 from mock_vws._mock_common import Route
 from mock_vws._query_tools import (
-    ActiveMatchingTargetsDeleteProcessing,
     get_query_match_response_text,
 )
 from mock_vws._query_validators import run_query_validators
 from mock_vws._query_validators.exceptions import (
-    DeletedTargetMatched,
     ValidatorException,
 )
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
     from requests_mock.request import _RequestObjectProxy
@@ -78,41 +76,27 @@
 
     This implementation is tied to the implementation of `requests_mock`.
     """
 
     def __init__(
         self,
         target_manager: TargetManager,
-        query_recognizes_deletion_seconds: int | float,
-        query_processes_deletion_seconds: int | float,
         query_match_checker: ImageMatcher,
     ) -> None:
         """
         Args:
             target_manager: The target manager which holds all databases.
-            query_recognizes_deletion_seconds: The number of seconds after a
-                target has been deleted that the query endpoint will still
-                recognize the target for.
-            query_processes_deletion_seconds: The number of seconds after a
-                target deletion is recognized that the query endpoint will
-                return a 500 response on a match.
             query_match_checker: A callable which takes two image values and
                 returns whether they match.
 
         Attributes:
             routes: The `Route`s to be used in the mock.
         """
         self.routes: set[Route] = _ROUTES
         self._target_manager = target_manager
-        self._query_processes_deletion_seconds = (
-            query_processes_deletion_seconds
-        )
-        self._query_recognizes_deletion_seconds = (
-            query_recognizes_deletion_seconds
-        )
         self._query_match_checker = query_match_checker
 
     @route(path_pattern="/v1/query", http_methods={POST})
     def query(
         self,
         request: _RequestObjectProxy,
         context: _Context,
@@ -129,34 +113,22 @@
                 databases=self._target_manager.databases,
             )
         except ValidatorException as exc:
             context.headers = exc.headers
             context.status_code = exc.status_code
             return exc.response_text
 
-        try:
-            response_text = get_query_match_response_text(
-                request_headers=request.headers,
-                request_body=request.body,
-                request_method=request.method,
-                request_path=request.path,
-                databases=self._target_manager.databases,
-                query_processes_deletion_seconds=(
-                    self._query_processes_deletion_seconds
-                ),
-                query_recognizes_deletion_seconds=(
-                    self._query_recognizes_deletion_seconds
-                ),
-                query_match_checker=self._query_match_checker,
-            )
-        except ActiveMatchingTargetsDeleteProcessing:
-            deleted_target_matched_exception = DeletedTargetMatched()
-            context.headers = deleted_target_matched_exception.headers
-            context.status_code = deleted_target_matched_exception.status_code
-            return deleted_target_matched_exception.response_text
+        response_text = get_query_match_response_text(
+            request_headers=request.headers,
+            request_body=request.body,
+            request_method=request.method,
+            request_path=request.path,
+            databases=self._target_manager.databases,
+            query_match_checker=self._query_match_checker,
+        )
 
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         context.headers = {
             "Connection": "keep-alive",
             "Content-Type": "application/json",
             "Server": "nginx",
             "Date": date,
```

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/mock_web_services_api.py` & `vws-python-mock-2023.5.21/src/mock_vws/_requests_mock_server/mock_web_services_api.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/__init__.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/__init__.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/active_flag_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/active_flag_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/auth_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/auth_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/content_length_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/content_length_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/content_type_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/content_type_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/date_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/date_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/exceptions.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/exceptions.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/image_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/image_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/json_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/json_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/key_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/key_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/metadata_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/metadata_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/name_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/name_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/project_state_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/project_state_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/target_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/target_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/width_validators.py` & `vws-python-mock-2023.5.21/src/mock_vws/_services_validators/width_validators.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/database.py` & `vws-python-mock-2023.5.21/src/mock_vws/database.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/image_matchers.py` & `vws-python-mock-2023.5.21/src/mock_vws/image_matchers.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/resources/deleted_target_matched_response.html` & `vws-python-mock-2023.5.21/src/mock_vws/resources/deleted_target_matched_response.html`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/resources/oops_error_occurred_response.html` & `vws-python-mock-2023.5.21/src/mock_vws/resources/oops_error_occurred_response.html`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/target.py` & `vws-python-mock-2023.5.21/src/mock_vws/target.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/target_manager.py` & `vws-python-mock-2023.5.21/src/mock_vws/target_manager.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/src/mock_vws/target_raters.py` & `vws-python-mock-2023.5.21/src/mock_vws/target_raters.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from typing import Protocol, runtime_checkable
 
 import brisque
 import cv2
 import numpy as np
 from PIL import Image
 
+# cv2 errors cannot be inferred without type stubs.
+# See https://github.com/opencv/opencv/issues/14590.
+_CV2_ERROR = (
+    cv2.error  # pyright: ignore[reportGeneralTypeIssues] # noqa: E501 # pylint: disable=no-member
+)
+
 
 @functools.cache
 def _get_brisque_target_tracking_rating(image_content: bytes) -> int:
     """
     Get a target tracking rating based on a BRISQUE score.
 
     This is a rough approximation of the quality score used by Vuforia, but is
@@ -28,15 +34,15 @@
     image = Image.open(fp=image_file)
     image_array = np.asarray(a=image)
     brisque_obj = brisque.BRISQUE(url=False)
     # We avoid a barrage of warnings from the BRISQUE library.
     with np.errstate(divide="ignore", invalid="ignore"):
         try:
             score = brisque_obj.score(img=image_array)
-        except (cv2.error, ValueError):  # pylint: disable=no-member
+        except (_CV2_ERROR, ValueError):
             return 0
     if math.isnan(score):
         return 0
     brisque_max_score = 100
     tracking_rating_max = 5
     return int(score / (brisque_max_score / tracking_rating_max))
```

### Comparing `vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/PKG-INFO` & `vws-python-mock-2023.5.21/src/vws_python_mock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vws-python-mock
-Version: 2023.4.8
+Version: 2023.5.21
 Summary: A mock for the Vuforia Web Services (VWS) API.
 Author-email: Adam Dangoor <adamdangoor@gmail.com>
 License: The MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/SOURCES.txt` & `vws-python-mock-2023.5.21/src/vws_python_mock.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,14 @@
 src/vws_python_mock.egg-info/dependency_links.txt
 src/vws_python_mock.egg-info/not-zip-safe
 src/vws_python_mock.egg-info/requires.txt
 src/vws_python_mock.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/mock_vws/__init__.py
-tests/mock_vws/jetty_error_deletion_not_complete.html
 tests/mock_vws/test_add_target.py
 tests/mock_vws/test_authorization_header.py
 tests/mock_vws/test_content_length.py
 tests/mock_vws/test_database_summary.py
 tests/mock_vws/test_date_header.py
 tests/mock_vws/test_delete_target.py
 tests/mock_vws/test_docker.py
```

### Comparing `vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/requires.txt` & `vws-python-mock-2023.5.21/src/vws_python_mock.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -5,51 +5,51 @@
 multipart
 numpy
 opencv-python
 pydantic
 requests
 requests-mock
 vws-auth-tools
-werkzeug
 
 [:sys_platform == "win32"]
 tzdata
 
 [dev]
 PyYAML==6.0
 Sphinx-Substitution-Extensions==2022.2.16
-Sphinx==6.1.3
+Sphinx==7.0.1
 VWS-Test-Fixtures==2023.3.5
 black==23.3.0
 check-manifest==0.49
-dirty-equals==0.5.0
+dirty-equals==0.6.0
 doc8==0.11.2
-docker==6.0.1
+docker==6.1.2
 dodgy==0.2.1
 enum-tools[sphinx]==0.9.0.post1
 freezegun==1.2.2
-furo==2023.3.27
-mypy==1.2.0
-pdm==2.4.9
+furo==2023.5.20
+mypy==1.3.0
+pdm==2.6.1
 pip_check_reqs==2.4.4
 pydocstyle==6.3.0
 pyenchant==3.2.2
-pylint==2.17.2
-pyright==1.1.302
+pylint==2.17.4
+pyright==1.1.309
 pyroma==4.2
 pytest-cov==4.0.0
-pytest==7.2.2
-requests-mock-flask==2023.3.5.1
-ruff==0.0.261
-sphinx-autodoc-typehints==1.22
+pytest==7.3.1
+requests-mock-flask==2023.5.14
+ruff==0.0.269
+sphinx-autodoc-typehints==1.23.0
 sphinx-prompt==1.5.0
 sphinx_paramlinks==0.5.4
 sphinxcontrib-httpdomain==1.8.1
 sphinxcontrib-spelling==8.0.0
 sphinx-toolbox==3.4.0
-sybil==5.0.0
+sybil==5.0.2
 types-PyYAML==6.0.12.9
-types-Pillow==9.4.0.19
-types-requests==2.28.11.17
-types-urllib3==1.26.25.10
+types-Pillow==9.5.0.4
+types-requests==2.30.0.0
+types-urllib3==1.26.25.13
+urllib3<2.0.0
 vulture==2.7
 vws-python==2023.3.25
```

### Comparing `vws-python-mock-2023.4.8/tests/conftest.py` & `vws-python-mock-2023.5.21/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/fixtures/credentials.py` & `vws-python-mock-2023.5.21/tests/mock_vws/fixtures/credentials.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/fixtures/prepared_requests.py` & `vws-python-mock-2023.5.21/tests/mock_vws/fixtures/prepared_requests.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/fixtures/vuforia_backends.py` & `vws-python-mock-2023.5.21/tests/mock_vws/fixtures/vuforia_backends.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_add_target.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_add_target.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_authorization_header.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_authorization_header.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_content_length.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_content_length.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_database_summary.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_database_summary.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_date_header.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_date_header.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_delete_target.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_delete_target.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_docker.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_docker.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 from http import HTTPStatus
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import docker
 import pytest
 import requests
-from docker.errors import BuildError
+from docker.errors import BuildError, NotFound
+from docker.models.containers import Container
+from docker.models.networks import Network
 from mock_vws.database import VuforiaDatabase
 from vws import VWS, CloudRecoService
 
 if TYPE_CHECKING:
     import io
     from collections.abc import Iterator
 
-    from docker.models.networks import Network
-
 
 # We do not cover this function because hitting particular branches depends on
 # timing.
 def wait_for_flask_app_to_start(base_url: str) -> None:  # pragma: no cover
     """
     Wait for a server to start.
 
@@ -68,21 +68,23 @@
     """
     client = docker.from_env()
     try:
         network = client.networks.create(
             name="test-vws-bridge-" + uuid.uuid4().hex,
             driver="bridge",
         )
-    except docker.errors.NotFound:
+    except NotFound:
         # On Windows the "bridge" network driver is not available and we use
         # the "nat" driver instead.
         network = client.networks.create(
             name="test-vws-bridge-" + uuid.uuid4().hex,
             driver="nat",
         )
+
+    assert isinstance(network, Network)
     try:
         yield network
     finally:
         network.reload()
         for container in network.containers:
             network.disconnect(container=container)
             container.stop()
@@ -111,15 +113,15 @@
 
     random = uuid.uuid4().hex
     target_manager_tag = f"vws-mock-target-manager:latest-{random}"
     vws_tag = f"vws-mock-vws:latest-{random}"
     vwq_tag = f"vws-mock-vwq:latest-{random}"
 
     try:
-        target_manager_image, _ = client.images.build(
+        target_manager_build_result = client.images.build(
             path=str(repository_root),
             dockerfile=str(target_manager_dockerfile),
             tag=target_manager_tag,
         )
     except BuildError as exc:
         full_log = "\n".join(
             [item["stream"] for item in exc.build_log if "stream" in item],
@@ -129,24 +131,31 @@
         if (
             "no matching manifest for windows/amd64" not in exc.msg
         ):  # pragma: no cover
             raise AssertionError(full_log) from exc
         reason = "We do not currently support using Windows containers."
         pytest.skip(reason)
 
-    vws_image, _ = client.images.build(
+    assert isinstance(target_manager_build_result, tuple)
+    target_manager_image, _ = target_manager_build_result
+
+    vws_build_result = client.images.build(
         path=str(repository_root),
         dockerfile=str(vws_dockerfile),
         tag=vws_tag,
     )
-    vwq_image, _ = client.images.build(
+    assert isinstance(vws_build_result, tuple)
+    vws_image, _ = vws_build_result
+    vwq_build_result = client.images.build(
         path=str(repository_root),
         dockerfile=str(vwq_dockerfile),
         tag=vwq_tag,
     )
+    assert isinstance(vwq_build_result, tuple)
+    vwq_image, _ = vwq_build_result
 
     database = VuforiaDatabase()
     target_manager_container_name = "vws-mock-target-manager-" + random
     target_manager_internal_base_url = (
         f"http://{target_manager_container_name}:5000"
     )
 
@@ -174,29 +183,38 @@
         publish_all_ports=True,
         network=custom_bridge_network.name,
         environment={
             "TARGET_MANAGER_BASE_URL": target_manager_internal_base_url,
         },
     )
 
+    assert isinstance(target_manager_container, Container)
+    assert isinstance(vws_container, Container)
+    assert isinstance(vwq_container, Container)
     for container in (target_manager_container, vws_container, vwq_container):
         container.reload()
 
+    assert isinstance(target_manager_container.attrs, dict)
+    target_manager_port_attrs = target_manager_container.attrs[
+        "NetworkSettings"
+    ]["Ports"]
     target_manager_port_attrs = target_manager_container.attrs[
         "NetworkSettings"
     ]["Ports"]
     task_manager_host_ip = target_manager_port_attrs["5000/tcp"][0]["HostIp"]
     task_manager_host_port = target_manager_port_attrs["5000/tcp"][0][
         "HostPort"
     ]
 
+    assert isinstance(vws_container.attrs, dict)
     vws_port_attrs = vws_container.attrs["NetworkSettings"]["Ports"]
     vws_host_ip = vws_port_attrs["5000/tcp"][0]["HostIp"]
     vws_host_port = vws_port_attrs["5000/tcp"][0]["HostPort"]
 
+    assert isinstance(vwq_container.attrs, dict)
     vwq_port_attrs = vwq_container.attrs["NetworkSettings"]["Ports"]
     vwq_host_ip = vwq_port_attrs["5000/tcp"][0]["HostIp"]
     vwq_host_port = vwq_port_attrs["5000/tcp"][0]["HostPort"]
 
     base_vws_url = f"http://{vws_host_ip}:{vws_host_port}"
     base_vwq_url = f"http://{vwq_host_ip}:{vwq_host_port}"
     base_task_manager_url = (
```

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_flask_app_usage.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_flask_app_usage.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 from mock_vws._flask_server.vws import VWS_FLASK_APP
 from mock_vws.database import VuforiaDatabase
 from PIL import Image
 from requests_mock_flask import add_flask_app_to_mock
 from vws import VWS, CloudRecoService
 
 from tests.mock_vws.utils.usage_test_helpers import (
-    process_deletion_seconds,
     processing_time_seconds,
-    recognize_deletion_seconds,
 )
 
 if TYPE_CHECKING:
     from requests_mock import Mocker
 
 _EXAMPLE_URL_FOR_TARGET_MANAGER = "http://" + uuid.uuid4().hex + ".com"
 
@@ -112,154 +110,14 @@
             image=image_file_failed_state,
         )
 
         expected = seconds
         assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
 
 
-class TestCustomQueryRecognizesDeletionSeconds:
-    """
-    Tests for setting the amount of time after a target has been deleted
-    until it is not recognized by the query endpoint.
-    """
-
-    LEEWAY = 0.5
-
-    def test_default(
-        self,
-        high_quality_image: io.BytesIO,
-        monkeypatch: pytest.MonkeyPatch,
-    ) -> None:
-        """
-        By default it takes 2 seconds for the Query API on the mock to
-        recognize that a target has been deleted.
-
-        The real Query API takes between zero and two seconds.
-        See ``test_query`` for more information.
-        """
-        database = VuforiaDatabase()
-        # Use the "exact" matcher, as it is the fastest.
-        monkeypatch.setenv(name="QUERY_IMAGE_MATCHER", value="exact")
-        # Use the fastest tracking rater.
-        monkeypatch.setenv(name="TARGET_RATER", value="perfect")
-        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
-        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
-        time_taken = recognize_deletion_seconds(
-            high_quality_image=high_quality_image,
-            vuforia_database=database,
-        )
-
-        expected = 2
-        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
-
-    @pytest.mark.parametrize(
-        argnames=["seconds"],
-        # We include 0 because it exercises some otherwise untouched code.
-        argvalues=[(0,), (5,)],
-    )
-    def test_custom(
-        self,
-        high_quality_image: io.BytesIO,
-        monkeypatch: pytest.MonkeyPatch,
-        seconds: int | float,
-    ) -> None:
-        """
-        It is possible to use set a custom amount of time that it takes for the
-        Query API on the mock to recognize that a target has been deleted.
-        """
-        database = VuforiaDatabase()
-        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
-        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
-        monkeypatch.setenv(
-            name="DELETION_RECOGNITION_SECONDS",
-            value=str(seconds),
-        )
-        # Use the "exact" matcher, as it is the fastest.
-        monkeypatch.setenv(name="QUERY_IMAGE_MATCHER", value="exact")
-        time_taken = recognize_deletion_seconds(
-            high_quality_image=high_quality_image,
-            vuforia_database=database,
-        )
-
-        expected = seconds
-        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
-
-
-class TestCustomQueryProcessDeletionSeconds:
-    """
-    Tests for setting the amount of time after a target has been deleted
-    until it is not processed by the query endpoint.
-    """
-
-    # There is a race condition in this test type - if tests start to
-    # fail, consider increasing the leeway.
-    LEEWAY = 0.5
-
-    def test_default(
-        self,
-        high_quality_image: io.BytesIO,
-        monkeypatch: pytest.MonkeyPatch,
-    ) -> None:
-        """
-        By default it takes three seconds for the Query API on the mock to
-        process that a target has been deleted.
-
-        The real Query API takes between seven and thirty seconds.
-        See ``test_query`` for more information.
-        """
-        # Use the "exact" matcher, as it is the fastest.
-        monkeypatch.setenv(name="QUERY_IMAGE_MATCHER", value="exact")
-        # Use the fastest tracking rater.
-        monkeypatch.setenv(name="TARGET_RATER", value="perfect")
-        database = VuforiaDatabase()
-        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
-        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
-        time_taken = process_deletion_seconds(
-            high_quality_image=high_quality_image,
-            vuforia_database=database,
-        )
-
-        expected = 3
-        # We minus the leeway because we might start the timer after the
-        # deletion processing has started.
-        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
-
-    def test_custom(
-        self,
-        high_quality_image: io.BytesIO,
-        monkeypatch: pytest.MonkeyPatch,
-    ) -> None:
-        """
-        It is possible to use set a custom amount of time that it takes for the
-        Query API on the mock to process that a target has been deleted.
-        """
-        # Use the "exact" matcher, as it is the fastest.
-        monkeypatch.setenv(name="QUERY_IMAGE_MATCHER", value="exact")
-        # Use the fastest tracking rater.
-        monkeypatch.setenv(name="TARGET_RATER", value="perfect")
-        # We choose a low time for a quick test.
-        query_processes_deletion = 5
-        database = VuforiaDatabase()
-        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
-        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
-        monkeypatch.setenv(
-            name="DELETION_PROCESSING_SECONDS",
-            value=str(query_processes_deletion),
-        )
-        time_taken = process_deletion_seconds(
-            high_quality_image=high_quality_image,
-            vuforia_database=database,
-        )
-
-        expected = query_processes_deletion
-        # We minus the leeway because we might start the timer after the
-        # deletion processing has started.
-        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
-
-
 class TestAddDatabase:
     """
     Tests for adding databases to the mock.
     """
 
     @staticmethod
     def test_duplicate_keys() -> None:
```

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_get_duplicates.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_get_duplicates.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_get_target.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_get_target.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_invalid_given_id.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_invalid_given_id.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_invalid_json.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_invalid_json.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_query.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import datetime
 import io
 import sys
 import textwrap
 import time
 import uuid
 from http import HTTPStatus
-from pathlib import Path
 from typing import TYPE_CHECKING, Any
 from urllib.parse import urljoin
 from zoneinfo import ZoneInfo
 
 import pytest
 import requests
 from mock_vws._constants import ResultCodes
@@ -73,21 +72,14 @@
     <center><h1>413 Request Entity Too Large</h1></center>\r
     <hr><center>nginx</center>\r
     </body>\r
     </html>\r
     """,
 )
 
-_JETTY_ERROR_DELETION_NOT_COMPLETE_START_PATH = (
-    Path(__file__).parent / "jetty_error_deletion_not_complete.html"
-)
-_JETTY_ERROR_DELETION_NOT_COMPLETE = (
-    _JETTY_ERROR_DELETION_NOT_COMPLETE_START_PATH.read_text()
-)
-
 
 def query(
     vuforia_database: VuforiaDatabase,
     body: dict[str, Any],
 ) -> requests.Response:
     """
     Make a request to the endpoint to make an image recognition query.
@@ -864,15 +856,15 @@
             "image": ("image.jpeg", image_content, "image/jpeg"),
             "max_num_results": (None, num_results, "text/plain"),
         }
 
         response = query(vuforia_database=vuforia_database, body=body)
 
         expected_text = (
-            f"Integer out of range ({repr(num_results)}) in form data part "
+            f"Integer out of range ({num_results}) in form data part "
             "'max_result'. Accepted range is from 1 to 50 (inclusive)."
         )
         assert response.text == expected_text
         assert_vwq_failure(
             response=response,
             content_type="application/json",
             status_code=HTTPStatus.BAD_REQUEST,
@@ -1846,117 +1838,31 @@
     @staticmethod
     def test_deleted(
         high_quality_image: io.BytesIO,
         vuforia_database: VuforiaDatabase,
         vws_client: VWS,
     ) -> None:
         """
-        Within approximately 7 seconds of deleting a target, querying for its
-        image results in an ``INTERNAL_SERVER_ERROR``.
+        Deleted targets are not matched.
         """
         image_content = high_quality_image.getvalue()
         target_id = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
             image=high_quality_image,
             active_flag=True,
             application_metadata=None,
         )
         vws_client.wait_for_target_processed(target_id=target_id)
         vws_client.delete_target(target_id=target_id)
 
         body = {"image": ("image.jpeg", image_content, "image/jpeg")}
 
-        while True:
-            response = query(vuforia_database=vuforia_database, body=body)
-            # Sometimes the first response(s) include the old target.
-            try:
-                assert_query_success(response=response)
-            except AssertionError:
-                assert response.text.startswith(
-                    _JETTY_ERROR_DELETION_NOT_COMPLETE,
-                )
-                assert_vwq_failure(
-                    response=response,
-                    content_type="text/html;charset=iso-8859-1",
-                    status_code=HTTPStatus.INTERNAL_SERVER_ERROR,
-                    cache_control="must-revalidate,no-cache,no-store",
-                    www_authenticate=None,
-                    connection="keep-alive",
-                )
-
-                return
-
-    @staticmethod
-    def test_deleted_and_wait(
-        high_quality_image: io.BytesIO,
-        vuforia_database: VuforiaDatabase,
-        vws_client: VWS,
-    ) -> None:
-        """
-        After waiting approximately 7 seconds (we wait more to be safer), a
-        deleted target is not found when its image is queried for.
-        """
-        image_content = high_quality_image.getvalue()
-        target_id = vws_client.add_target(
-            name=uuid.uuid4().hex,
-            width=1,
-            image=high_quality_image,
-            active_flag=True,
-            application_metadata=None,
-        )
-        vws_client.wait_for_target_processed(target_id=target_id)
-        vws_client.delete_target(target_id=target_id)
-
-        body = {"image": ("image.jpeg", image_content, "image/jpeg")}
-
-        # In practice, we have seen a delay of up to 30 seconds between
-        # deleting a target and getting a valid response which has a result
-        # array without the deleted item.
-        total_waited = 0
-
-        # We wait up to 60 seconds to be safe to avoid indefinite waits and
-        # using up our quota.
-        max_wait_seconds = 60
-
-        # We do not want to retry immediately else we risk using our request
-        # quota.
-        sleep_seconds = 2
-
-        server_error_seen = False
-
-        while True:
-            response = query(vuforia_database=vuforia_database, body=body)
-
-            try:
-                assert_query_success(response=response)
-            except AssertionError:
-                server_error_seen = True
-                assert response.text.startswith(
-                    _JETTY_ERROR_DELETION_NOT_COMPLETE,
-                )
-                time.sleep(sleep_seconds)
-                total_waited += sleep_seconds
-            else:
-                if response.json()["results"]:
-                    (result,) = response.json()["results"]
-                    assert result["target_id"] == target_id
-                    # We never see the target ID after having seen the server
-                    # error.
-                    assert not server_error_seen
-                    time.sleep(sleep_seconds)
-                    total_waited += sleep_seconds
-                else:
-                    assert response.json()["results"] == []
-                    break
-
-            assert total_waited < max_wait_seconds
-
-        # The deletion never takes effect immediately.
-        assert total_waited
+        response = query(vuforia_database=vuforia_database, body=body)
+        assert response.json()["results"] == []
 
     @staticmethod
     def test_deleted_inactive(
         high_quality_image: io.BytesIO,
         vuforia_database: VuforiaDatabase,
         vws_client: VWS,
     ) -> None:
```

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_requests_mock_usage.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_requests_mock_usage.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,25 +12,22 @@
 import pytest
 import requests
 from freezegun import freeze_time
 from mock_vws import MockVWS
 from mock_vws.database import VuforiaDatabase
 from mock_vws.image_matchers import AverageHashMatcher, ExactMatcher
 from mock_vws.target import Target
-from mock_vws.target_raters import HardcodedTargetTrackingRater
 from PIL import Image
 from requests.exceptions import MissingSchema
 from requests_mock.exceptions import NoMockAddress
 from vws import VWS, CloudRecoService
 from vws_auth_tools import rfc_1123_date
 
 from tests.mock_vws.utils.usage_test_helpers import (
-    process_deletion_seconds,
     processing_time_seconds,
-    recognize_deletion_seconds,
 )
 
 
 def _not_exact_matcher(
     first_image_content: bytes,
     second_image_content: bytes,
 ) -> bool:
@@ -242,149 +239,14 @@
         expected = (
             'Invalid URL "vuforia.vwq.example.com": No scheme supplied. '
             'Perhaps you meant "https://vuforia.vwq.example.com".'
         )
         assert str(vwq_exc.value) == expected
 
 
-class TestCustomQueryRecognizesDeletionSeconds:
-    """
-    Tests for setting the amount of time after a target has been deleted
-    until it is not recognized by the query endpoint.
-    """
-
-    LEEWAY = 0.5
-
-    def test_default(
-        self,
-        high_quality_image: io.BytesIO,
-    ) -> None:
-        """
-        By default it takes 2 seconds for the Query API on the mock to
-        recognize that a target has been deleted.
-
-        The real Query API takes between zero and two seconds.
-        See ``test_query`` for more information.
-        """
-        database = VuforiaDatabase()
-        with MockVWS(
-            # Use the fastest available matcher.
-            query_match_checker=ExactMatcher(),
-            # Use the fastest available tracker.
-            target_tracking_rater=HardcodedTargetTrackingRater(rating=5),
-        ) as mock:
-            mock.add_database(database=database)
-            time_taken = recognize_deletion_seconds(
-                high_quality_image=high_quality_image,
-                vuforia_database=database,
-            )
-
-        expected = 2
-        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
-
-    @pytest.mark.parametrize(
-        argnames=["seconds"],
-        # We include 0 because it exercises some otherwise untouched code.
-        argvalues=[(0,), (5,)],
-    )
-    def test_custom(
-        self,
-        high_quality_image: io.BytesIO,
-        seconds: int | float,
-    ) -> None:
-        """
-        It is possible to use set a custom amount of time that it takes for the
-        Query API on the mock to recognize that a target has been deleted.
-        """
-        database = VuforiaDatabase()
-        with MockVWS(
-            # Use the fastest available matcher.
-            query_match_checker=ExactMatcher(),
-            query_recognizes_deletion_seconds=seconds,
-        ) as mock:
-            mock.add_database(database=database)
-            time_taken = recognize_deletion_seconds(
-                high_quality_image=high_quality_image,
-                vuforia_database=database,
-            )
-
-        expected = seconds
-        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
-
-
-class TestCustomQueryProcessDeletionSeconds:
-    """
-    Tests for setting the amount of time after a target has been deleted
-    until it is not processed by the query endpoint.
-    """
-
-    # There is a race condition in this test type - if tests start to
-    # fail, consider increasing the leeway.
-    LEEWAY = 0.5
-
-    def test_default(
-        self,
-        high_quality_image: io.BytesIO,
-    ) -> None:
-        """
-        By default it takes three seconds for the Query API on the mock to
-        process that a target has been deleted.
-
-        The real Query API takes between seven and thirty seconds.
-        See ``test_query`` for more information.
-        """
-        database = VuforiaDatabase()
-        with MockVWS(
-            # Use the fastest available matcher.
-            query_match_checker=ExactMatcher(),
-            # Use the fastest available tracker.
-            target_tracking_rater=HardcodedTargetTrackingRater(rating=5),
-        ) as mock:
-            mock.add_database(database=database)
-            time_taken = process_deletion_seconds(
-                high_quality_image=high_quality_image,
-                vuforia_database=database,
-            )
-
-        expected = 3
-        # We minus the leeway because we might start the timer after the
-        # deletion processing has started.
-        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
-
-    def test_custom(
-        self,
-        high_quality_image: io.BytesIO,
-    ) -> None:
-        """
-        It is possible to use set a custom amount of time that it takes for the
-        Query API on the mock to process that a target has been deleted.
-        """
-        # We choose a low time for a quick test.
-        # We choose a time high enough that the leeway won't be a problem.
-        query_processes_deletion = 5
-        database = VuforiaDatabase()
-        with MockVWS(
-            query_processes_deletion_seconds=query_processes_deletion,
-            # Use the fastest available matcher.
-            query_match_checker=ExactMatcher(),
-            # Use the fastest available tracker.
-            target_tracking_rater=HardcodedTargetTrackingRater(rating=5),
-        ) as mock:
-            mock.add_database(database=database)
-            time_taken = process_deletion_seconds(
-                high_quality_image=high_quality_image,
-                vuforia_database=database,
-            )
-
-        expected = query_processes_deletion
-        # We minus the leeway because we might start the timer after the
-        # deletion processing has started.
-        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
-
-
 class TestTargets:
     """
     Tests for target representations.
     """
 
     @staticmethod
     def test_to_dict(high_quality_image: io.BytesIO) -> None:
```

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_target_list.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_target_list.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_target_summary.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_target_summary.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_unexpected_json.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_unexpected_json.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/test_update_target.py` & `vws-python-mock-2023.5.21/tests/mock_vws/test_update_target.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/utils/__init__.py` & `vws-python-mock-2023.5.21/tests/mock_vws/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/tests/mock_vws/utils/assertions.py` & `vws-python-mock-2023.5.21/tests/mock_vws/utils/assertions.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.4.8/vuforia_secrets.env.example` & `vws-python-mock-2023.5.21/vuforia_secrets.env.example`

 * *Files identical despite different names*

