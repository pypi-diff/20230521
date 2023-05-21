# Comparing `tmp/osw-0.7.2.tar.gz` & `tmp/osw-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osw-0.7.2.tar", last modified: Fri May 12 05:53:13 2023, max compression
+gzip compressed data, was "osw-0.8.0.tar", last modified: Sun May 21 16:06:29 2023, max compression
```

## Comparing `osw-0.7.2.tar` & `osw-0.8.0.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.970792 osw-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-12 05:52:40.000000 osw-0.7.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.958792 osw-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.962792 osw-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-12 05:52:40.000000 osw-0.7.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-12 05:52:40.000000 osw-0.7.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-12 05:52:40.000000 osw-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-12 05:52:40.000000 osw-0.7.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 05:52:40.000000 osw-0.7.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-12 05:52:40.000000 osw-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-12 05:52:40.000000 osw-0.7.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-12 05:52:40.000000 osw-0.7.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-12 05:52:40.000000 osw-0.7.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-12 05:52:40.000000 osw-0.7.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-05-12 05:52:40.000000 osw-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-05-12 05:52:40.000000 osw-0.7.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-12 05:53:13.970792 osw-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-12 05:52:40.000000 osw-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 05:52:40.000000 osw-0.7.2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.962792 osw-0.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-12 05:52:40.000000 osw-0.7.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.962792 osw-0.7.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 05:52:40.000000 osw-0.7.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-12 05:52:40.000000 osw-0.7.2/docs/auth.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 05:52:40.000000 osw-0.7.2/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-12 05:52:40.000000 osw-0.7.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-05-12 05:52:40.000000 osw-0.7.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 05:52:40.000000 osw-0.7.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-12 05:52:40.000000 osw-0.7.2/docs/controller.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 05:52:40.000000 osw-0.7.2/docs/dev.md
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-12 05:52:40.000000 osw-0.7.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-12 05:52:40.000000 osw-0.7.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 05:52:40.000000 osw-0.7.2/docs/model.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 05:52:40.000000 osw-0.7.2/docs/osw.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-12 05:52:40.000000 osw-0.7.2/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-12 05:52:40.000000 osw-0.7.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 05:52:40.000000 osw-0.7.2/docs/tools.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.962792 osw-0.7.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-12 05:52:40.000000 osw-0.7.2/examples/accounts.pwd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-12 05:52:40.000000 osw-0.7.2/examples/controller_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 05:52:40.000000 osw-0.7.2/examples/create_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-12 05:52:40.000000 osw-0.7.2/examples/create_page_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.962792 osw-0.7.2/examples/data_processing/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-12 05:52:40.000000 osw-0.7.2/examples/data_processing/local_jsonpath_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-12 05:52:40.000000 osw-0.7.2/examples/database_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-12 05:52:40.000000 osw-0.7.2/examples/entity_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-12 05:52:40.000000 osw-0.7.2/examples/load_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-05-12 05:52:40.000000 osw-0.7.2/examples/local_editing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-12 05:52:40.000000 osw-0.7.2/examples/ontology_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-05-12 05:52:40.000000 osw-0.7.2/examples/page_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-12 05:52:40.000000 osw-0.7.2/examples/register_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 05:52:40.000000 osw-0.7.2/examples/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-12 05:52:40.000000 osw-0.7.2/examples/store_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-12 05:52:40.000000 osw-0.7.2/examples/update_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-12 05:52:40.000000 osw-0.7.2/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.958792 osw-0.7.2/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.962792 osw-0.7.2/nb/quantities/
--rw-r--r--   0 runner    (1001) docker     (123)   123529 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/Quantities.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.966792 osw-0.7.2/nb/quantities/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   107607 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/broader.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59112 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/buildDictionaryTest.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   152865 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/httpRequest.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/idea.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/querys.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/searchRunaways.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.966792 osw-0.7.2/nb/translations/
--rw-r--r--   0 runner    (1001) docker     (123)   404547 2023-05-12 05:52:40.000000 osw-0.7.2/nb/translations/DeeplTranslate.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-12 05:52:40.000000 osw-0.7.2/nb/translations/JsObjectToJson.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-12 05:52:40.000000 osw-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-12 05:53:13.970792 osw-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-12 05:52:40.000000 osw-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.958792 osw-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.966792 osw-0.7.2/src/osw/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.966792 osw-0.7.2/src/osw/controller/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/controller/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/controller/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    22113 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.970792 osw-0.7.2/src/osw/model/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/model/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/model/page_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/model/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/sparql_client_smw.py
--rw-r--r--   0 runner    (1001) docker     (123)    37470 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/wiki_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    20859 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/wtsite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.966792 osw-0.7.2/src/osw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-12 05:53:13.000000 osw-0.7.2/src/osw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-12 05:53:13.000000 osw-0.7.2/src/osw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 05:53:13.000000 osw-0.7.2/src/osw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 05:53:13.000000 osw-0.7.2/src/osw.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-12 05:53:13.000000 osw-0.7.2/src/osw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 05:53:13.000000 osw-0.7.2/src/osw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.970792 osw-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-12 05:52:40.000000 osw-0.7.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-12 05:52:40.000000 osw-0.7.2/tests/controller_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.970792 osw-0.7.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-12 05:52:40.000000 osw-0.7.2/tests/integration/db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-12 05:52:40.000000 osw-0.7.2/tests/integration/login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-12 05:52:40.000000 osw-0.7.2/tests/integration/store_and_load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-12 05:52:40.000000 osw-0.7.2/tests/sparql_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-12 05:52:40.000000 osw-0.7.2/tests/test_credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-12 05:52:40.000000 osw-0.7.2/tests/test_osl.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-12 05:52:40.000000 osw-0.7.2/tests/test_wiki_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-12 05:52:40.000000 osw-0.7.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.906982 osw-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-21 16:05:56.000000 osw-0.8.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.874982 osw-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.886982 osw-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-21 16:05:56.000000 osw-0.8.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-21 16:05:56.000000 osw-0.8.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-21 16:05:56.000000 osw-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-21 16:05:56.000000 osw-0.8.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-21 16:05:56.000000 osw-0.8.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-21 16:05:56.000000 osw-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-21 16:05:56.000000 osw-0.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-21 16:05:56.000000 osw-0.8.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-21 16:05:56.000000 osw-0.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-21 16:05:56.000000 osw-0.8.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-05-21 16:05:56.000000 osw-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-05-21 16:05:56.000000 osw-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-21 16:06:29.906982 osw-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-21 16:05:56.000000 osw-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-21 16:05:56.000000 osw-0.8.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.894982 osw-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-21 16:05:56.000000 osw-0.8.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.894982 osw-0.8.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 16:05:56.000000 osw-0.8.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-21 16:05:56.000000 osw-0.8.0/docs/auth.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-21 16:05:56.000000 osw-0.8.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 16:05:56.000000 osw-0.8.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-05-21 16:05:56.000000 osw-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-21 16:05:56.000000 osw-0.8.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-21 16:05:56.000000 osw-0.8.0/docs/controller.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-21 16:05:56.000000 osw-0.8.0/docs/dev.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-21 16:05:56.000000 osw-0.8.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-21 16:05:56.000000 osw-0.8.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-21 16:05:56.000000 osw-0.8.0/docs/model.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 16:05:56.000000 osw-0.8.0/docs/osw.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-21 16:05:56.000000 osw-0.8.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-21 16:05:56.000000 osw-0.8.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-21 16:05:56.000000 osw-0.8.0/docs/tools.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.898982 osw-0.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-21 16:05:56.000000 osw-0.8.0/examples/accounts.pwd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-21 16:05:56.000000 osw-0.8.0/examples/controller_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-21 16:05:56.000000 osw-0.8.0/examples/create_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-21 16:05:56.000000 osw-0.8.0/examples/create_page_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.902982 osw-0.8.0/examples/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-21 16:05:56.000000 osw-0.8.0/examples/data_processing/local_jsonpath_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-21 16:05:56.000000 osw-0.8.0/examples/database_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-21 16:05:56.000000 osw-0.8.0/examples/entity_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-21 16:05:56.000000 osw-0.8.0/examples/load_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-05-21 16:05:56.000000 osw-0.8.0/examples/local_editing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-21 16:05:56.000000 osw-0.8.0/examples/ontology_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-05-21 16:05:56.000000 osw-0.8.0/examples/page_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-21 16:05:56.000000 osw-0.8.0/examples/register_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-21 16:05:56.000000 osw-0.8.0/examples/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-21 16:05:56.000000 osw-0.8.0/examples/store_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-21 16:05:56.000000 osw-0.8.0/examples/update_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-21 16:05:56.000000 osw-0.8.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.874982 osw-0.8.0/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.902982 osw-0.8.0/nb/quantities/
+-rw-r--r--   0 runner    (1001) docker     (123)   123529 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/Quantities.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.902982 osw-0.8.0/nb/quantities/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   107607 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/broader.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    59112 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/buildDictionaryTest.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   152865 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/httpRequest.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/idea.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/querys.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-05-21 16:05:56.000000 osw-0.8.0/nb/quantities/archive/searchRunaways.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.902982 osw-0.8.0/nb/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)   404547 2023-05-21 16:05:56.000000 osw-0.8.0/nb/translations/DeeplTranslate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-21 16:05:56.000000 osw-0.8.0/nb/translations/JsObjectToJson.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-21 16:05:56.000000 osw-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-21 16:06:29.910982 osw-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-21 16:05:56.000000 osw-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.878982 osw-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.902982 osw-0.8.0/src/osw/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.906982 osw-0.8.0/src/osw/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/controller/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/controller/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/controller/page_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22113 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.906982 osw-0.8.0/src/osw/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/model/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/model/page_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/model/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/sparql_client_smw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37510 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/wiki_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22013 2023-05-21 16:05:56.000000 osw-0.8.0/src/osw/wtsite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.906982 osw-0.8.0/src/osw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-21 16:06:29.000000 osw-0.8.0/src/osw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-21 16:06:29.000000 osw-0.8.0/src/osw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 16:06:29.000000 osw-0.8.0/src/osw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 16:06:29.000000 osw-0.8.0/src/osw.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-21 16:06:29.000000 osw-0.8.0/src/osw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-21 16:06:29.000000 osw-0.8.0/src/osw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.906982 osw-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-21 16:05:56.000000 osw-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-21 16:05:56.000000 osw-0.8.0/tests/controller_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:06:29.906982 osw-0.8.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-21 16:05:56.000000 osw-0.8.0/tests/integration/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-21 16:05:56.000000 osw-0.8.0/tests/integration/login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-21 16:05:56.000000 osw-0.8.0/tests/integration/store_and_load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-21 16:05:56.000000 osw-0.8.0/tests/sparql_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-21 16:05:56.000000 osw-0.8.0/tests/test_credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-21 16:05:56.000000 osw-0.8.0/tests/test_osl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-21 16:05:56.000000 osw-0.8.0/tests/test_wiki_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-21 16:05:56.000000 osw-0.8.0/tox.ini
```

### Comparing `osw-0.7.2/.coveragerc` & `osw-0.8.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/.github/workflows/ci.yml` & `osw-0.8.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/.github/workflows/docs.yml` & `osw-0.8.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/.gitignore` & `osw-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/.pre-commit-config.yaml` & `osw-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/CONTRIBUTING.md` & `osw-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/LICENSE.txt` & `osw-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/PKG-INFO` & `osw-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osw
-Version: 0.7.2
+Version: 0.8.0
 Summary: Python toolset for data processing, queries, wikicode generation and page manipulation
 Home-page: https://github.com/OpenSemanticLab/osw-python
 Author: "Simon Stier"
 Author-email: simon.stier@isc.fraunhofer.de
 License: AGPL-3.0-or-later
 Project-URL: Documentation, https://opensemanticlab.github.io/osw-python/
 Project-URL: Source, https://github.com/OpenSemanticLab/osw-python
```

### Comparing `osw-0.7.2/README.md` & `osw-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/docs/Makefile` & `osw-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/docs/conf.py` & `osw-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/docs/index.md` & `osw-0.8.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/examples/controller_logic.py` & `osw-0.8.0/examples/controller_logic.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/examples/data_processing/local_jsonpath_queries.py` & `osw-0.8.0/examples/data_processing/local_jsonpath_queries.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/examples/database_access.py` & `osw-0.8.0/examples/database_access.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/examples/entity_manipulation.py` & `osw-0.8.0/examples/entity_manipulation.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/examples/load_entity.py` & `osw-0.8.0/examples/load_entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/examples/local_editing.py` & `osw-0.8.0/examples/local_editing.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/examples/ontology_import.py` & `osw-0.8.0/examples/ontology_import.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/examples/page_manipulation.py` & `osw-0.8.0/examples/page_manipulation.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/examples/register_model.py` & `osw-0.8.0/examples/register_model.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/examples/settings.json` & `osw-0.8.0/examples/settings.json`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/examples/store_entity.py` & `osw-0.8.0/examples/store_entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/examples/update_local_model.py` & `osw-0.8.0/examples/update_local_model.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/nb/quantities/Quantities.ipynb` & `osw-0.8.0/nb/quantities/Quantities.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb` & `osw-0.8.0/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/nb/quantities/archive/broader.ipynb` & `osw-0.8.0/nb/quantities/archive/broader.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/nb/quantities/archive/buildDictionaryTest.ipynb` & `osw-0.8.0/nb/quantities/archive/buildDictionaryTest.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/nb/quantities/archive/httpRequest.ipynb` & `osw-0.8.0/nb/quantities/archive/httpRequest.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/nb/quantities/archive/idea.ipynb` & `osw-0.8.0/nb/quantities/archive/idea.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/nb/quantities/archive/querys.ipynb` & `osw-0.8.0/nb/quantities/archive/querys.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/nb/quantities/archive/searchRunaways.ipynb` & `osw-0.8.0/nb/quantities/archive/searchRunaways.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/nb/translations/DeeplTranslate.ipynb` & `osw-0.8.0/nb/translations/DeeplTranslate.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/nb/translations/JsObjectToJson.ipynb` & `osw-0.8.0/nb/translations/JsObjectToJson.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/setup.cfg` & `osw-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/setup.py` & `osw-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/src/osw/auth.py` & `osw-0.8.0/src/osw/auth.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/src/osw/controller/database.py` & `osw-0.8.0/src/osw/controller/database.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/src/osw/core.py` & `osw-0.8.0/src/osw/core.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/src/osw/model/entity.py` & `osw-0.8.0/src/osw/model/entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/src/osw/model/page_package.py` & `osw-0.8.0/src/osw/model/page_package.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 from typing import List, Optional, Union
 
 from pydantic import BaseModel
 
 
 class PagePackagePageSlot(BaseModel):
     url: Optional[str]
@@ -160,18 +161,20 @@
 
 
 class PagePackageConfig(BaseModel):
     """A config for a page package"""
 
     name: str
     """The name (label) of the package."""
-    config_path: str
-    """The path of the generated json file (package.json)."""
-    content_path: Optional[str] = ""
-    """The directory where the content (pages, files) is stored."""
+    config_path: Union[str, Path]
+    """The path of the generated json file (package.json).
+    Will be created automatically if not existing"""
+    content_path: Optional[Union[str, Path]] = ""
+    """The directory where the content (pages, files) is stored.
+    Will be created automatically if not existing."""
     titles: List[str]
     """List of page titles."""
     # replace: Optional[bool] = False
     bundle: PagePackageBundle
     """Bund of pages."""
     skip_slot_suffix_for_main: Optional[bool] = False
     include_files: Optional[bool] = True
@@ -183,7 +186,57 @@
         no __post_init__ method will be available until Pydantic v2. Then an
         analogous function will be implemented and any in a BaseModel class defined
         method named 'model_post_init(self, **kwargs)' will be called after
         init."""
         super().__init__(**data)
         if self.content_path == "":
             self.content_path = os.path.dirname(self.config_path)
+
+
+class PagePackageMetaData(BaseModel):
+    """Metadata for a page package. This data needed to create a page package and
+    included in the page package."""
+
+    name: str
+    """The name (label) of the page package."""
+    repo: str
+    """Page package repository name - usually the GitHub repository name"""
+    id: str
+    """Page package ID - usually the same as package_repo"""
+    subdir: str
+    """Page package subdirectory - usually resembling parts of the package name"""
+    branch: str
+    """Page package branch - usually 'main'."""
+    repo_org: str
+    """(GitHub) Organization hosting the package repository"""
+    description: str
+    """Page package description"""
+    language: str = "en"
+    """Page package language - usually the two-letter IETF language tag for that
+    language"""
+    version = "0.2.1"
+    """Page package version - use semantic versioning"""
+    author: List[str]
+    """Author(s) of the page package"""
+    publisher: str
+    """Publisher of the page package."""
+    page_titles: List[str]
+    """List of the page titles (full page titles with namespace, e.g. 'Category:Entity')
+     to be packaged."""
+
+
+# Special namespace mappings (default is namespace_const = "NS_" + namespace.upper())
+NAMESPACE_CONST_TO_NAMESPACE_MAPPING = {
+    # SMW: https://github.com/SemanticMediaWiki/SemanticMediaWiki/blob/ebb03c1537810f4ee8c1a25198b8d2e243cc38a1/src/NamespaceManager.php#L119
+    "SMW_NS_PROPERTY": "Property",
+    "SMW_NS_PROPERTY_TALK": "Property_talk",
+    "SMW_NS_CONCEPT": "Concept",
+    "SMW_NS_CONCEPT_TALK": "Concept_talk",
+    "SMW_NS_SCHEMA": "smw/schema",
+    "SMW_NS_SCHEMA_TALK": "smw/schema_talk",
+    "SMW_NS_RULE": "Rule",
+    "SMW_NS_RULE_TALK": "Rule_talk",
+}
+# inverse
+NAMESPACE_TO_NAMESPACE_CONST_MAPPING = {
+    v: k for k, v in NAMESPACE_CONST_TO_NAMESPACE_MAPPING.items()
+}
```

### Comparing `osw-0.7.2/src/osw/model/static.py` & `osw-0.8.0/src/osw/model/static.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/src/osw/sparql_client_smw.py` & `osw-0.8.0/src/osw/sparql_client_smw.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/src/osw/wiki_tools.py` & `osw-0.8.0/src/osw/wiki_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import copy
 import getpass
-from pathlib import Path
 from typing import Dict, List, Tuple, Union
 
 import mwclient
 import mwparserfromhell
 import numpy as np
 import yaml
 from jsonpath_ng.ext import parse
+from pydantic import FilePath
 
 
 def read_domains_from_credentials_file(
-    credentials_file_path: Union[str, Path]
+    credentials_file_path: Union[str, FilePath]
 ) -> Tuple[List[str], Dict[str, Dict[str, str]]]:
     """Reads domains and credentials from a yaml file
 
     Parameters
     ----------
     credentials_file_path
         Path to the yaml file with the credentials
@@ -32,15 +32,15 @@
                 raise ValueError("No domain found in accounts.pwd.yaml!")
             return domains_list, accounts_dict
         except yaml.YAMLError as exc_:
             print(exc_)
 
 
 def read_credentials_from_yaml(
-    password_file: Union[str, Path], domain: str = None
+    password_file: Union[str, FilePath], domain: str = None
 ) -> dict:
     """Reads credentials from a yaml file
 
     Parameters
     ----------
     password_file :
         Path to the yaml file with the credentials.
@@ -70,15 +70,15 @@
     else:
         user = input("Enter bot username (username@botname)")
         password = getpass.getpass("Enter bot password")
     return {"username": user, "password": password}
 
 
 def create_site_object(
-    domain: str, password_file: Union[str, Path] = "", credentials: dict = None
+    domain: str, password_file: Union[str, FilePath] = "", credentials: dict = None
 ) -> mwclient.client.Site:
     """
     Parameters
     ----------
     domain :
         Domain of the OSW instance, as specifed in the yaml file
     password_file :
@@ -377,16 +377,17 @@
             exists = False
             for rel1 in r1:
                 all_params_equal = True
                 for p in rel2.params:
                     if rel1.has(p.name):
                         if not rel1.get(p.name).value.matches(rel2.get(p.name).value):
                             all_params_equal = False
-                        # print("Compare {}:{} with :{} -> res={}".format(p.name, rel1.get(p.name).value,rel2.get(p.name).value,
-                        #                                                rel1.get(p.name).value.matches(rel2.get(p.name).value)))
+                        # print("Compare {}:{} with :{} -> res={}".format(p.name,
+                        #       rel1.get(p.name).value,rel2.get(p.name).value,
+                        #       rel1.get(p.name).value.matches(rel2.get(p.name).value)))
                     else:
                         all_params_equal = False
                 if all_params_equal:
                     exists = True
             if not exists:
                 r1.append(rel2)
         r1string = ""
@@ -527,15 +528,16 @@
                     wt += get_wikitext_from_flat_content_dict(element)
                     # wt += "\n{{" + element
                     # wt += get_wikitext_from_dict(element)
                     # wt += "\n}}"
                 else:
                     if string_index != index:
                         print(
-                            f"Warning: template param '{key}' has mixed template/string values: {value}"
+                            f"Warning: template param '{key}' has mixed template/"
+                            f"string values: {value}"
                         )
                     if string_index > 0 and element and not element.strip().isspace():
                         wt += ";"
                     wt += element
                     string_index += 1
         else:
             # print("literal")
```

### Comparing `osw-0.7.2/src/osw/wtsite.py` & `osw-0.8.0/src/osw/wtsite.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from pprint import pprint
 from time import sleep
 from typing import Dict, Optional, Union
 
 import mwclient
 from jsonpath_ng.ext import parse
-from pydantic import BaseModel
+from pydantic import BaseModel, FilePath
 
 import osw.model.page_package as package
 import osw.wiki_tools as wt
 from osw.model.entity import _basemodel_decorator
 
 # Definition of constants
 SLOTS = {
@@ -41,27 +41,27 @@
         self._page_cache = {}
         self._cache_enabled = False
 
     @classmethod
     def from_domain(
         cls,
         domain: str = None,
-        password_file: Union[str, Path] = None,
+        password_file: Union[str, FilePath] = None,
         credentials: dict = None,
     ):
         if credentials is None:
             site = wt.create_site_object(domain, password_file)
         else:
             site = wt.create_site_object(domain, "", credentials)
         return cls(site)
 
     @classmethod
     def from_credentials(
         cls,
-        credentials: Union[Dict[str, Dict[str, str]], str, Path],
+        credentials: Union[Dict[str, Dict[str, str]], str, FilePath],
         key: Union[str, int] = 0,
     ):
         """
 
         Parameters
         ----------
         credentials:
@@ -356,15 +356,15 @@
         d = dict(
             zip(range(len(self._dict)), self._dict)
         )  # convert list to dict with index
         for match in jsonpath_expr.find(d):
             res.append(match.value)
         return res
 
-    def update_dict(combined: dict, update: dict) -> None:
+    def update_dict(self, combined: dict, update: dict) -> None:
         for k, v in update.items():
             if isinstance(v, dict):
                 WtPage.combine_into(v, combined.setdefault(k, {}))
             else:
                 combined[k] = v
 
     def set_value(self, jsonpath_match, value, replace=False):
@@ -392,18 +392,19 @@
         return self
 
     def edit(self, comment: str = None, mode="action-multislot"):
         """creates / updates the content of all page slots in the wiki site
 
         Parameters
         ----------
-        comment, optional
-            edit comment for the page history, by default None
-        mode, optional
-            single API call ('action-multislot') or multiple ('action-singleslot'), by default 'action-multislot' (faster)
+        comment:
+            (optional) edit comment for the page history, by default None
+        mode:
+            (optional) single API call ('action-multislot') or multiple (
+            'action-singleslot'), by default 'action-multislot' (faster)
         """
         retry = 0
         max_retry = 5
         while retry < max_retry:
             try:
                 return self._edit(comment, mode)
             except Exception as e:
@@ -469,31 +470,56 @@
     def get_last_changed_time(self):
         return datetime.fromisoformat(
             self._current_revision["timestamp"].replace("Z", "+00:00")
         )
 
     @_basemodel_decorator
     class PageDumpConfig(BaseModel):
+        """Configuration to dump wiki pages to the file system"""
+
         target_dir: Union[str, Path]
+        """Directory to dump all contents.
+        Will be created automatically if not existing"""
         namespace_as_folder: Optional[bool] = True
+        """Store page contents in subfolders named according to their namespaces"""
         skip_slot_suffix_for_main: Optional[bool] = False
+        """If true, do not include 'main' in the generated content file.
+        Useful for pages / wikis using only the main slot."""
         dump_empty_slots: Optional[bool] = False
+        """If true, dump all configured slots even empty ones.
+        Useful to create initial content in these slots."""
         page_name_as_filename: Optional[bool] = False
+        """Use the (human readable) name of a page also for the file naming.
+        Useful to identify dumped files manually. The mapping to the page title/id
+        (in general a UUID) is ensured anyway through package.json meta data."""
 
         class Config:
             arbitrary_types_allowed = True  # necessary to allow e.g. np.array as type
 
-    def dump(self, config: PageDumpConfig):
+    def dump(self, config: PageDumpConfig) -> package.PagePackagePage:
+        """Dump this page to the file system
+
+        Parameters
+        ----------
+        config
+            see WtPage.PageDumpConfig
+
+        Returns
+        -------
+            Metadata of the generated dump
+        """
         page_name = self.title.split(":")[-1]
         if ":" in self.title:
             namespace = self.title.split(":")[0]
         else:
             namespace = "Main"
+
         namespace_const = "NS_" + namespace.upper()
-        # namespace_id = self._page.namespace
+        if namespace in package.NAMESPACE_TO_NAMESPACE_CONST_MAPPING:
+            namespace_const = package.NAMESPACE_TO_NAMESPACE_CONST_MAPPING[namespace]
 
         package_page = package.PagePackagePage(
             name=page_name, namespace=namespace_const, slots={}
         )
         name_in_json_data = False
         if "jsondata" in self._slots and "name" in self._slots["jsondata"]:
             package_page.label = self._slots["jsondata"]["name"]
```

### Comparing `osw-0.7.2/src/osw.egg-info/PKG-INFO` & `osw-0.8.0/src/osw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osw
-Version: 0.7.2
+Version: 0.8.0
 Summary: Python toolset for data processing, queries, wikicode generation and page manipulation
 Home-page: https://github.com/OpenSemanticLab/osw-python
 Author: "Simon Stier"
 Author-email: simon.stier@isc.fraunhofer.de
 License: AGPL-3.0-or-later
 Project-URL: Documentation, https://opensemanticlab.github.io/osw-python/
 Project-URL: Source, https://github.com/OpenSemanticLab/osw-python
```

### Comparing `osw-0.7.2/src/osw.egg-info/SOURCES.txt` & `osw-0.8.0/src/osw.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 src/osw.egg-info/dependency_links.txt
 src/osw.egg-info/not-zip-safe
 src/osw.egg-info/requires.txt
 src/osw.egg-info/top_level.txt
 src/osw/controller/__init__.py
 src/osw/controller/database.py
 src/osw/controller/entity.py
+src/osw/controller/page_package.py
 src/osw/model/__init__.py
 src/osw/model/entity.py
 src/osw/model/page_package.py
 src/osw/model/static.py
 tests/conftest.py
 tests/controller_mixin.py
 tests/sparql_client_test.py
```

### Comparing `osw-0.7.2/tests/conftest.py` & `osw-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/tests/controller_mixin.py` & `osw-0.8.0/tests/controller_mixin.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/tests/integration/db_test.py` & `osw-0.8.0/tests/integration/db_test.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/tests/integration/store_and_load_test.py` & `osw-0.8.0/tests/integration/store_and_load_test.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/tests/sparql_client_test.py` & `osw-0.8.0/tests/sparql_client_test.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/tests/test_credential_manager.py` & `osw-0.8.0/tests/test_credential_manager.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.2/tox.ini` & `osw-0.8.0/tox.ini`

 * *Files identical despite different names*

