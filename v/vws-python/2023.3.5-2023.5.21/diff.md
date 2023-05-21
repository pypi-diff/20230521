# Comparing `tmp/vws-python-2023.3.5.tar.gz` & `tmp/vws-python-2023.5.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vws-python-2023.3.5.tar", last modified: Sun Mar  5 10:07:00 2023, max compression
+gzip compressed data, was "vws-python-2023.5.21.tar", last modified: Sun May 21 19:03:44 2023, max compression
```

## Comparing `vws-python-2023.3.5.tar` & `vws-python-2023.5.21.tar`

### file list

```diff
@@ -1,68 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:07:00.799916 vws-python-2023.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-05 10:06:31.000000 vws-python-2023.3.5/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-05 10:06:31.000000 vws-python-2023.3.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:07:00.795916 vws-python-2023.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-05 10:06:31.000000 vws-python-2023.3.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:07:00.795916 vws-python-2023.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-05 10:06:31.000000 vws-python-2023.3.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-05 10:06:31.000000 vws-python-2023.3.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-05 10:06:31.000000 vws-python-2023.3.5/.github/workflows/windows-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-05 10:06:31.000000 vws-python-2023.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-05 10:06:34.000000 vws-python-2023.3.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-03-05 10:06:31.000000 vws-python-2023.3.5/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-03-05 10:06:31.000000 vws-python-2023.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-05 10:06:31.000000 vws-python-2023.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-05 10:06:31.000000 vws-python-2023.3.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-03-05 10:07:00.799916 vws-python-2023.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-03-05 10:06:31.000000 vws-python-2023.3.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-05 10:06:31.000000 vws-python-2023.3.5/codecov.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:07:00.795916 vws-python-2023.3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-05 10:06:31.000000 vws-python-2023.3.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:07:00.795916 vws-python-2023.3.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-05 10:06:31.000000 vws-python-2023.3.5/docs/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-05 10:06:31.000000 vws-python-2023.3.5/docs/source/api-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-05 10:06:31.000000 vws-python-2023.3.5/docs/source/changelog.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2359 2023-03-05 10:06:31.000000 vws-python-2023.3.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-05 10:06:31.000000 vws-python-2023.3.5/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-05 10:06:31.000000 vws-python-2023.3.5/docs/source/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-05 10:06:31.000000 vws-python-2023.3.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-05 10:06:31.000000 vws-python-2023.3.5/docs/source/release-process.rst
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-03-05 10:06:31.000000 vws-python-2023.3.5/lint.mk
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-03-05 10:06:31.000000 vws-python-2023.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-05 10:06:31.000000 vws-python-2023.3.5/readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:07:00.795916 vws-python-2023.3.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-05 10:06:31.000000 vws-python-2023.3.5/requirements/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-05 10:06:31.000000 vws-python-2023.3.5/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-05 10:06:31.000000 vws-python-2023.3.5/requirements/setup-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 10:07:00.799916 vws-python-2023.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-05 10:06:31.000000 vws-python-2023.3.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-05 10:06:31.000000 vws-python-2023.3.5/spelling_private_dict.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:07:00.791916 vws-python-2023.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:07:00.795916 vws-python-2023.3.5/src/vws/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-05 10:06:31.000000 vws-python-2023.3.5/src/vws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:07:00.795916 vws-python-2023.3.5/src/vws/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-05 10:06:31.000000 vws-python-2023.3.5/src/vws/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-05 10:06:31.000000 vws-python-2023.3.5/src/vws/exceptions/base_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-05 10:06:31.000000 vws-python-2023.3.5/src/vws/exceptions/cloud_reco_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-05 10:06:31.000000 vws-python-2023.3.5/src/vws/exceptions/custom_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-05 10:06:31.000000 vws-python-2023.3.5/src/vws/exceptions/vws_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-05 10:06:31.000000 vws-python-2023.3.5/src/vws/include_target_data.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 10:06:31.000000 vws-python-2023.3.5/src/vws/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-03-05 10:06:31.000000 vws-python-2023.3.5/src/vws/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-03-05 10:06:31.000000 vws-python-2023.3.5/src/vws/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    24701 2023-03-05 10:06:31.000000 vws-python-2023.3.5/src/vws/vws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:07:00.799916 vws-python-2023.3.5/src/vws_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-03-05 10:07:00.000000 vws-python-2023.3.5/src/vws_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-03-05 10:07:00.000000 vws-python-2023.3.5/src/vws_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 10:07:00.000000 vws-python-2023.3.5/src/vws_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 10:07:00.000000 vws-python-2023.3.5/src/vws_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-05 10:07:00.000000 vws-python-2023.3.5/src/vws_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-05 10:07:00.000000 vws-python-2023.3.5/src/vws_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 10:07:00.799916 vws-python-2023.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-05 10:06:31.000000 vws-python-2023.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-05 10:06:31.000000 vws-python-2023.3.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-03-05 10:06:31.000000 vws-python-2023.3.5/tests/test_cloud_reco_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-05 10:06:31.000000 vws-python-2023.3.5/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-03-05 10:06:31.000000 vws-python-2023.3.5/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-03-05 10:06:31.000000 vws-python-2023.3.5/tests/test_vws.py
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-03-05 10:06:31.000000 vws-python-2023.3.5/tests/test_vws_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:44.597975 vws-python-2023.5.21/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 19:03:28.000000 vws-python-2023.5.21/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-21 19:03:28.000000 vws-python-2023.5.21/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:44.589974 vws-python-2023.5.21/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-21 19:03:28.000000 vws-python-2023.5.21/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:44.589974 vws-python-2023.5.21/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-21 19:03:28.000000 vws-python-2023.5.21/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-21 19:03:28.000000 vws-python-2023.5.21/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-21 19:03:28.000000 vws-python-2023.5.21/.github/workflows/windows-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-21 19:03:28.000000 vws-python-2023.5.21/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:44.589974 vws-python-2023.5.21/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-21 19:03:28.000000 vws-python-2023.5.21/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-21 19:03:28.000000 vws-python-2023.5.21/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-21 19:03:30.000000 vws-python-2023.5.21/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-21 19:03:28.000000 vws-python-2023.5.21/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-21 19:03:28.000000 vws-python-2023.5.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-21 19:03:28.000000 vws-python-2023.5.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-21 19:03:28.000000 vws-python-2023.5.21/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-21 19:03:44.597975 vws-python-2023.5.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-21 19:03:28.000000 vws-python-2023.5.21/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-21 19:03:28.000000 vws-python-2023.5.21/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-21 19:03:28.000000 vws-python-2023.5.21/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:44.589974 vws-python-2023.5.21/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-21 19:03:28.000000 vws-python-2023.5.21/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:44.593974 vws-python-2023.5.21/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 19:03:28.000000 vws-python-2023.5.21/docs/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-21 19:03:28.000000 vws-python-2023.5.21/docs/source/api-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 19:03:28.000000 vws-python-2023.5.21/docs/source/changelog.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2374 2023-05-21 19:03:28.000000 vws-python-2023.5.21/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-21 19:03:28.000000 vws-python-2023.5.21/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-21 19:03:28.000000 vws-python-2023.5.21/docs/source/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-21 19:03:28.000000 vws-python-2023.5.21/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-21 19:03:28.000000 vws-python-2023.5.21/docs/source/release-process.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-21 19:03:28.000000 vws-python-2023.5.21/lint.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-21 19:03:28.000000 vws-python-2023.5.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-21 19:03:28.000000 vws-python-2023.5.21/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:03:44.597975 vws-python-2023.5.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-21 19:03:28.000000 vws-python-2023.5.21/spelling_private_dict.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:44.589974 vws-python-2023.5.21/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:44.593974 vws-python-2023.5.21/src/vws/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-21 19:03:28.000000 vws-python-2023.5.21/src/vws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:44.593974 vws-python-2023.5.21/src/vws/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 19:03:28.000000 vws-python-2023.5.21/src/vws/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-21 19:03:28.000000 vws-python-2023.5.21/src/vws/exceptions/base_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-21 19:03:28.000000 vws-python-2023.5.21/src/vws/exceptions/cloud_reco_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-21 19:03:28.000000 vws-python-2023.5.21/src/vws/exceptions/custom_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-21 19:03:28.000000 vws-python-2023.5.21/src/vws/exceptions/vws_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-21 19:03:28.000000 vws-python-2023.5.21/src/vws/include_target_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:28.000000 vws-python-2023.5.21/src/vws/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-21 19:03:28.000000 vws-python-2023.5.21/src/vws/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-21 19:03:28.000000 vws-python-2023.5.21/src/vws/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23430 2023-05-21 19:03:28.000000 vws-python-2023.5.21/src/vws/vws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:44.597975 vws-python-2023.5.21/src/vws_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-21 19:03:44.000000 vws-python-2023.5.21/src/vws_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-21 19:03:44.000000 vws-python-2023.5.21/src/vws_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:03:44.000000 vws-python-2023.5.21/src/vws_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:03:44.000000 vws-python-2023.5.21/src/vws_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-21 19:03:44.000000 vws-python-2023.5.21/src/vws_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-21 19:03:44.000000 vws-python-2023.5.21/src/vws_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:03:44.597975 vws-python-2023.5.21/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-21 19:03:28.000000 vws-python-2023.5.21/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-21 19:03:28.000000 vws-python-2023.5.21/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-21 19:03:28.000000 vws-python-2023.5.21/tests/test_cloud_reco_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-05-21 19:03:28.000000 vws-python-2023.5.21/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-05-21 19:03:28.000000 vws-python-2023.5.21/tests/test_vws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-05-21 19:03:28.000000 vws-python-2023.5.21/tests/test_vws_exceptions.py
```

### Comparing `vws-python-2023.3.5/.github/workflows/ci.yml` & `vws-python-2023.5.21/.github/workflows/ci.yml`

 * *Files 11% similar despite different names*

```diff
@@ -28,18 +28,15 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - uses: actions/cache@v3
         with:
           path: ~/.cache/pip
-          # This is like the example but we use ``*requirements.txt`` rather
-          # than ``requirements.txt`` because we have multiple requirements
-          # files.
-          key: ${{ runner.os }}-pip-${{ hashFiles('**/*requirements.txt') }}
+          key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml') }}
           restore-keys: |
             ${{ runner.os }}-pip-
 
       - name: "Install dependencies"
         run: |
           python -m pip install --upgrade pip setuptools wheel
           # We use '--ignore-installed' to avoid GitHub's cache which can cause
@@ -49,11 +46,13 @@
 
       - name: "Lint"
         run: |
           make lint
 
       - name: "Run tests"
         run: |
-          pytest -s -vvv --cov-fail-under 100 --cov=src/ --cov=tests tests/ --cov-report=xml
+          # We run tests against "." and not the tests directory as we test the README
+          # and documentation.
+          pytest -s -vvv --cov-fail-under 100 --cov=src/ --cov=tests . --cov-report=xml
 
       - name: "Upload coverage to Codecov"
         uses: "codecov/codecov-action@v3"
```

### Comparing `vws-python-2023.3.5/.github/workflows/release.yml` & `vws-python-2023.5.21/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -66,11 +66,11 @@
           # Checkout the latest tag - the one we just created.
           git fetch --tags
           git checkout $(git describe --tags $(git rev-list --tags --max-count=1))
           python -m pip install build
           python -m build --sdist --wheel --outdir dist/ .
 
       - name: Publish distribution 📦 to PyPI
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
           verbose: true
```

### Comparing `vws-python-2023.3.5/.github/workflows/windows-ci.yml` & `vws-python-2023.5.21/.github/workflows/windows-ci.yml`

 * *Files 18% similar despite different names*

```diff
@@ -28,25 +28,24 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - uses: actions/cache@v3
         with:
           path: ~\AppData\Local\pip\Cache
-          # This is like the example but we use ``*requirements.txt`` rather
-          # than ``requirements.txt`` because we have multiple requirements
-          # files.
-          key: ${{ runner.os }}-pip-${{ hashFiles('**/*requirements.txt') }}
+          key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml') }}
           restore-keys: |
             ${{ runner.os }}-pip-
 
       - name: "Install dependencies"
         run: |
           python -m pip install --upgrade pip setuptools wheel
           # We use '--ignore-installed' to avoid GitHub's cache which can cause
           # issues - we have seen packages from this cache be cause trouble with
           # pip-extra-reqs.
           python -m pip install --ignore-installed --upgrade --editable .[dev]
 
       - name: "Run tests"
         run: |
-          pytest -s -vvv --cov-fail-under 100 --cov=src/ --cov=tests tests/ --cov-report=xml
+          # We run tests against "." and not the tests directory as we test the README
+          # and documentation.
+          pytest -s -vvv --cov-fail-under 100 --cov=src/ --cov=tests . --cov-report=xml
```

### Comparing `vws-python-2023.3.5/.gitignore` & `vws-python-2023.5.21/.gitignore`

 * *Files identical despite different names*

### Comparing `vws-python-2023.3.5/CHANGELOG.rst` & `vws-python-2023.5.21/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 Changelog
 =========
 
 Next
 ----
 
+2023.05.21
+------------
+
+* Breaking change: the ``vws.exceptions.custom_exceptions.ActiveMatchingTargetsDeleteProcessing`` exception has been removed as Vuforia no longer returns this error.
+
+2023.03.25
+------------
+
+* Support file-like objects in every method which accepts a file.
+
 2023.03.05
 ------------
 
 2021.03.28.2
 ------------
 
 2021.03.28.1
```

### Comparing `vws-python-2023.3.5/CODE_OF_CONDUCT.rst` & `vws-python-2023.5.21/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `vws-python-2023.3.5/LICENSE` & `vws-python-2023.5.21/LICENSE`

 * *Files identical despite different names*

### Comparing `vws-python-2023.3.5/Makefile` & `vws-python-2023.5.21/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     check-manifest \
     doc8 \
     linkcheck \
     mypy \
     ruff \
     pip-extra-reqs \
     pip-missing-reqs \
+    pyright \
     pyroma \
     spelling \
     vulture \
     pylint
 
 .PHONY: fix-lint
 fix-lint: \
```

### Comparing `vws-python-2023.3.5/PKG-INFO` & `vws-python-2023.5.21/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vws-python
-Version: 2023.3.5
+Version: 2023.5.21
 Summary: Interact with the Vuforia Web Services (VWS) API.
 Author-email: Adam Dangoor <adamdangoor@gmail.com>
 License: The MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,42 +28,72 @@
 Project-URL: Documentation, https://vws-python.readthedocs.io/en/latest/
 Keywords: vuforia,vws,client
 Classifier: Operating System :: POSIX
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 |Build Status| |codecov| |PyPI| |Documentation Status|
 
 vws-python
 ==========
 
-Python library for the Vuforia Web Services (VWS) API and the Vuforia Web Query API.
+Python library for the Vuforia Web Services (VWS) API and the Vuforia
+Web Query API.
 
 Installation
 ------------
 
 .. code:: sh
 
    pip install vws-python
 
-This is tested on Python 3.11+.
-Get in touch with ``adamdangoor@gmail.com`` if you would like to use this with another language.
+This is tested on Python 3.11+. Get in touch with
+``adamdangoor@gmail.com`` if you would like to use this with another
+language.
 
 Getting Started
 ---------------
 
-.. code:: python
+.. invisible-code-block: python
+
+   import contextlib
+   import pathlib
+   import shutil
+
+   import vws_test_fixtures
+   from mock_vws import MockVWS
+   from mock_vws.database import VuforiaDatabase
+
+   mock = MockVWS(real_http=False)
+   database = VuforiaDatabase(
+       server_access_key='[server-access-key]',
+       server_secret_key='[server-secret-key]',
+       client_access_key='[client-access-key]',
+       client_secret_key='[client-secret-key]',
+   )
+   mock.add_database(database=database)
+   stack = contextlib.ExitStack()
+   stack.enter_context(mock)
+
+   # We rely on implementation details of the fixtures package.
+   image = pathlib.Path(vws_test_fixtures.__path__[0]) / 'high_quality_image.jpg'
+   assert image.exists(), image.resolve()
+   new_image = pathlib.Path('high_quality_image.jpg')
+   shutil.copy(image, new_image)
 
-   import io
+
+.. code-block:: python
+
+   import pathlib
 
    from vws import VWS, CloudRecoService
 
    server_access_key = '[server-access-key]'
    server_secret_key = '[server-secret-key]'
    client_access_key = '[client-access-key]'
    client_secret_key = '[client-secret-key]'
@@ -74,37 +104,40 @@
    )
    cloud_reco_client = CloudRecoService(
        client_access_key=client_access_key,
        client_secret_key=client_secret_key,
    )
    name = 'my_image_name'
 
-   with open('/path/to/image.png', 'rb') as my_image_file:
-      my_image = io.BytesIO(my_image_file.read())
-
-   target_id = vws_client.add_target(
-       name=name,
-       width=1,
-       image=my_image,
-       active_flag=True,
-       application_metadata=None,
-   )
-   vws_client.wait_for_target_processed(target_id=target_id)
-   matching_targets = cloud_reco_client.query(image=my_image)
+   image = pathlib.Path('high_quality_image.jpg')
+   with image.open(mode='rb') as my_image_file:
+       target_id = vws_client.add_target(
+           name=name,
+           width=1,
+           image=my_image_file,
+           active_flag=True,
+           application_metadata=None,
+       )
+       vws_client.wait_for_target_processed(target_id=target_id)
+       matching_targets = cloud_reco_client.query(image=my_image_file)
 
    assert matching_targets[0].target_id == target_id
 
+.. invisible-code-block: python
+   new_image = pathlib.Path('high_quality_image.jpg')
+   new_image.unlink()
+   stack.close()
 
 Full Documentation
 ------------------
 
-See the `full documentation <https://vws-python.readthedocs.io/en/latest>`__.
+See the `full
+documentation <https://vws-python.readthedocs.io/en/latest>`__.
 
 .. |Build Status| image:: https://github.com/VWS-Python/vws-python/workflows/CI/badge.svg
    :target: https://github.com/VWS-Python/vws-python/actions
 .. |codecov| image:: https://codecov.io/gh/VWS-Python/vws-python/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/VWS-Python/vws-python
-.. |Documentation Status| image:: https://readthedocs.org/projects/vws-python/badge/?version=latest
-   :target: https://vws-python.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
 .. |PyPI| image:: https://badge.fury.io/py/VWS-Python.svg
    :target: https://badge.fury.io/py/VWS-Python
+.. |Documentation Status| image:: https://readthedocs.org/projects/vws-python/badge/?version=latest
+   :target: https://vws-python.readthedocs.io/en/latest/?badge=latest
```

### Comparing `vws-python-2023.3.5/docs/Makefile` & `vws-python-2023.5.21/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vws-python-2023.3.5/docs/source/conf.py` & `vws-python-2023.5.21/docs/source/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 """
 Configuration for Sphinx.
 """
 
 # pylint: disable=invalid-name
 
 import datetime
-
-from pkg_resources import get_distribution
+import importlib.metadata
 
 project = "VWS-Python"
 author = "Adam Dangoor"
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
@@ -29,17 +28,17 @@
 year = datetime.datetime.now(tz=datetime.UTC).year
 project_copyright = f"{year}, {author}"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-# Use ``pkg_resources`` as per
+# Use ``importlib.metadata.version`` as per
 # https://github.com/pypa/setuptools_scm#usage-from-sphinx.
-version = get_distribution(project).version
+version = importlib.metadata.version(distribution_name=project)
 _month, _day, _year, *_ = version.split(".")
 release = f"{_month}.{_day}.{_year}"
 
 language = "en"
 
 # The name of the syntax highlighting style to use.
 pygments_style = "sphinx"
```

### Comparing `vws-python-2023.3.5/docs/source/contributing.rst` & `vws-python-2023.5.21/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `vws-python-2023.3.5/docs/source/exceptions.rst` & `vws-python-2023.5.21/docs/source/exceptions.rst`

 * *Files identical despite different names*

### Comparing `vws-python-2023.3.5/docs/source/index.rst` & `vws-python-2023.5.21/tests/test_cloud_reco_exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,115 @@
-|project|
-=========
+"""
+Tests for exceptions raised when using the CloudRecoService.
+"""
+
+from __future__ import annotations
+
+import uuid
+from http import HTTPStatus
+from typing import TYPE_CHECKING
+
+import pytest
+from mock_vws import MockVWS
+from mock_vws.database import VuforiaDatabase
+from mock_vws.states import States
+from vws import CloudRecoService
+from vws.exceptions.base_exceptions import CloudRecoException
+from vws.exceptions.cloud_reco_exceptions import (
+    AuthenticationFailure,
+    BadImage,
+    InactiveProject,
+    MaxNumResultsOutOfRange,
+    RequestTimeTooSkewed,
+)
+from vws.exceptions.custom_exceptions import (
+    RequestEntityTooLarge,
+)
+
+if TYPE_CHECKING:
+    import io
+
+
+def test_too_many_max_results(
+    cloud_reco_client: CloudRecoService,
+    high_quality_image: io.BytesIO,
+) -> None:
+    """
+    A ``MaxNumResultsOutOfRange`` error is raised if the given
+    ``max_num_results`` is out of range.
+    """
+    with pytest.raises(MaxNumResultsOutOfRange) as exc:
+        cloud_reco_client.query(
+            image=high_quality_image,
+            max_num_results=51,
+        )
+
+    expected_value = (
+        "Integer out of range (51) in form data part 'max_result'. "
+        "Accepted range is from 1 to 50 (inclusive)."
+    )
+    assert str(exc.value) == exc.value.response.text == expected_value
+
+
+def test_image_too_large(
+    cloud_reco_client: CloudRecoService,
+    png_too_large: io.BytesIO,
+) -> None:
+    """
+    A ``RequestEntityTooLarge`` exception is raised if an image which is too
+    large is given.
+    """
+    with pytest.raises(RequestEntityTooLarge):
+        cloud_reco_client.query(image=png_too_large)
+
+
+def test_cloudrecoexception_inheritance() -> None:
+    """
+    CloudRecoService-specific exceptions inherit from CloudRecoException.
+    """
+    subclasses = [
+        MaxNumResultsOutOfRange,
+        InactiveProject,
+        BadImage,
+        AuthenticationFailure,
+        RequestTimeTooSkewed,
+    ]
+    for subclass in subclasses:
+        assert issubclass(subclass, CloudRecoException)
+
+
+def test_authentication_failure(high_quality_image: io.BytesIO) -> None:
+    """
+    An ``AuthenticationFailure`` exception is raised when the client access key
+    exists but the client secret key is incorrect.
+    """
+    database = VuforiaDatabase()
+    cloud_reco_client = CloudRecoService(
+        client_access_key=database.client_access_key,
+        client_secret_key=uuid.uuid4().hex,
+    )
+    with MockVWS() as mock:
+        mock.add_database(database=database)
+
+        with pytest.raises(AuthenticationFailure) as exc:
+            cloud_reco_client.query(image=high_quality_image)
+
+        assert exc.value.response.status_code == HTTPStatus.UNAUTHORIZED
+
+
+def test_inactive_project(high_quality_image: io.BytesIO) -> None:
+    """
+    An ``InactiveProject`` exception is raised when querying an inactive
+    database.
+    """
+    database = VuforiaDatabase(state=States.PROJECT_INACTIVE)
+    with MockVWS() as mock:
+        mock.add_database(database=database)
+        cloud_reco_client = CloudRecoService(
+            client_access_key=database.client_access_key,
+            client_secret_key=database.client_secret_key,
+        )
 
-Installation
-------------
+        with pytest.raises(InactiveProject) as exc:
+            cloud_reco_client.query(image=high_quality_image)
 
-.. prompt:: bash
-
-   pip3 install vws-python
-
-This is tested on Python 3.8+.
-Get in touch with ``adamdangoor@gmail.com`` if you would like to use this with another language.
-
-Usage
------
-
-See the :doc:`api-reference` for full usage details.
-
-.. code:: python
-
-   import io
-
-   from vws import VWS, CloudRecoService
-
-   server_access_key = '[server-access-key]'
-   server_secret_key = '[server-secret-key]'
-   client_access_key = '[client-access-key]'
-   client_secret_key = '[client-secret-key]'
-
-   vws_client = VWS(
-       server_access_key=server_access_key,
-       server_secret_key=server_secret_key,
-   )
-   cloud_reco_client = CloudRecoService(
-       client_access_key=client_access_key,
-       client_secret_key=client_secret_key,
-   )
-   name = 'my_image_name'
-
-   with open('/path/to/image.png', 'rb') as my_image_file:
-      my_image = io.BytesIO(my_image_file.read())
-
-   target_id = vws_client.add_target(
-       name=name,
-       width=1,
-       image=my_image,
-       active_flag=True,
-       application_metadata=None,
-   )
-   vws_client.wait_for_target_processed(target_id=target_id)
-   matching_targets = cloud_reco_client.query(image=my_image)
-
-   assert matching_targets[0].target_id == target_id
-
-Testing
--------
-
-To write unit tests for code which uses this library, without using your Vuforia quota, you can use the `VWS Python Mock`_ tool:
-
-.. prompt:: bash
-
-   pip3 install vws-python-mock
-
-.. code:: python
-
-   from mock_vws import MockVWS, VuforiaDatabase
-
-   with MockVWS() as mock:
-       database = VuforiaDatabase()
-       mock.add_database(database=database)
-       vws_client = VWS(
-           server_access_key=server_access_key,
-           server_secret_key=server_secret_key,
-       )
-       cloud_reco_client = CloudRecoService(
-           client_access_key=client_access_key,
-           client_secret_key=client_secret_key,
-       )
-
-       name = 'my_image_name'
-
-       with open('/path/to/image.png', 'rb') as my_image_file:
-           my_image = io.BytesIO(my_image_file.read())
-
-       target_id = vws_client.add_target(
-           name=name,
-           width=1,
-           image=my_image,
-       )
-
-There are some differences between the mock and the real Vuforia.
-See https://vws-python-mock.readthedocs.io/en/latest/differences-to-vws.html for details.
-
-.. _VWS Python Mock: https://github.com/VWS-Python/vws-python-mock
-
-
-Reference
----------
-
-.. toctree::
-   :maxdepth: 3
-
-   api-reference
-   exceptions
-   contributing
-   release-process
-   changelog
+        assert exc.value.response.status_code == HTTPStatus.FORBIDDEN
```

### Comparing `vws-python-2023.3.5/lint.mk` & `vws-python-2023.5.21/lint.mk`

 * *Files 20% similar despite different names*

```diff
@@ -28,28 +28,32 @@
 
 .PHONY: fix-ruff
 fix-ruff:
 	ruff --fix .
 
 .PHONY: pip-extra-reqs
 pip-extra-reqs:
-	pip-extra-reqs --requirements-file=requirements/requirements.txt src/
+	pip-extra-reqs --requirements-file=<(pdm export --pyproject) src/
 
 .PHONY: pip-missing-reqs
 pip-missing-reqs:
-	pip-missing-reqs --requirements-file=requirements/requirements.txt src/
+	pip-missing-reqs --requirements-file=<(pdm export --pyproject) src/
 
 .PHONY: pylint
 pylint:
 	pylint *.py src/ tests/ docs/
 
 .PHONY: pyroma
 pyroma:
 	pyroma --min 10 .
 
+.PHONY: pyright
+pyright:
+	pyright .
+
 .PHONY: vulture
 vulture:
 	vulture --min-confidence 100 --exclude _vendor --exclude .eggs .
 
 .PHONY: linkcheck
 linkcheck:
 	$(MAKE) -C docs/ linkcheck SPHINXOPTS=$(SPHINXOPTS)
```

### Comparing `vws-python-2023.3.5/pyproject.toml` & `vws-python-2023.5.21/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -88,14 +88,17 @@
 
 line-length = 79
 
 [tool.coverage.run]
 
 branch = true
 
+[tool.coverage.report]
+exclude_lines = ["pragma: no cover", "if TYPE_CHECKING:"]
+
 [tool.pytest.ini_options]
 
 xfail_strict = true
 log_cli = true
 
 [tool.check-manifest]
 
@@ -137,22 +140,28 @@
 [tool.mypy]
 
 strict = true
 
 [[tool.mypy.overrides]]
 
 module = [
-	"func_timeout",
-	"func_timeout.exceptions"
+    "sybil",
+    "sybil.parsers.rest",
 ]
 
 ignore_missing_imports = true
 
 [build-system]
-requires = ["setuptools", "pip", "wheel"]
+requires = [
+    "pip",
+    "setuptools",
+    "setuptools-scm-git-archive==1.4",
+    "setuptools_scm[toml]==7.1.0",
+    "wheel",
+]
 build-backend = "setuptools.build_meta"
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 [tool.ruff]
 select = ["ALL"]
@@ -164,38 +173,37 @@
     "C901",
     # Allow our chosen docstring line-style - no one-line summary.
     "D200",
     "D203",
     "D205",
     "D212",
     "D213",
-    # Allow backslashes in a docstring.
-    # See https://click.palletsprojects.com/en/8.0.x/documentation/#preventing-rewrapping.
-    "D301",
     # It is too much work to make every docstring imperative.
     "D401",
     # We ignore some docstyle errors which do not apply to Google style
     # docstrings.
     "D406",
     "D407",
     # We have an existing interface to support and so we do not want to change
     # exception names.
     "N818",
     # Ignore "too-many-*" errors as they seem to get in the way more than
     # helping.
-    "PLR0912",
     "PLR0913",
     # Allow 'assert' as we use it for tests.
     "S101",
-    # Allow imports which are only used for type checking to be outside type
-    # checking blocks.
-    "TCH002",
-    "TCH003",
+    # Allow simple random numbers as we are not using them for cryptography.
+    "S311",
 ]
 
+# Do not automatically remove commented out code.
+# We comment out code during development, and with VSCode auto-save, this code
+# is sometimes annoyingly removed.
+unfixable = ["ERA001"]
+
 [tool.ruff.per-file-ignores]
 "tests/test_*.py" = [
     # Do not require tests to have a one-line summary.
     "D205",
 ]
 
 [project]
@@ -210,20 +218,62 @@
 description = "Interact with the Vuforia Web Services (VWS) API."
 dynamic = ["version"]
 keywords = ["vuforia", "vws", "client"]
 license = { file = "LICENSE" }
 name = "vws-python"
 readme = { file = "README.rst", content-type = "text/x-rst"}
 requires-python = ">=3.10"
+dependencies = [
+    "VWS-Auth-Tools",
+    "requests",
+    "urllib3",
+]
+
+[project.optional-dependencies]
+dev = [
+    "PyYAML==6.0",
+    "Pygments==2.15.1",
+    "Sphinx-Substitution-Extensions==2022.2.16",
+    "Sphinx==7.0.1",
+    "VWS-Python-Mock==2023.5.21",
+    "VWS-Test-Fixtures==2023.3.5",
+    "black==23.3.0",
+    "check-manifest==0.49",
+    "doc8==1.1.1",
+    "dodgy==0.2.1",
+    "freezegun==1.2.2",
+    "furo==2023.5.20",
+    "mypy==1.3.0",
+    "pdm==2.6.1",
+    "pip_check_reqs==2.4.4",
+    "pydocstyle==6.3.0  ",
+    "pyenchant==3.2.2 ",
+    "pyright==1.1.309",
+    "pylint==2.17.4 ",
+    "pyroma==4.2",
+    "pytest-cov==4.0.0",
+    "pytest==7.3.1 ",
+    "ruff==0.0.269",
+    "sphinx-autodoc-typehints==1.23.0",
+    "sphinx-prompt==1.5.0",
+    "sphinxcontrib-spelling==8.0.0",
+    "sybil==5.0.2",
+    "types-requests==2.30.0.0",
+    "vulture==2.7",
+]
 
 [project.urls]
 Source = "https://github.com/VWS-Python/vws-python"
 Documentation = "https://vws-python.readthedocs.io/en/latest/"
 
 [tool.setuptools]
 zip-safe = false
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
 vws = ["py.typed"]
+
+[tool.setuptools_scm]
+
+[tool.pyright]
```

### Comparing `vws-python-2023.3.5/spelling_private_dict.txt` & `vws-python-2023.5.21/spelling_private_dict.txt`

 * *Files identical despite different names*

### Comparing `vws-python-2023.3.5/src/vws/exceptions/base_exceptions.py` & `vws-python-2023.5.21/src/vws/exceptions/base_exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """
 Base exceptions for errors returned by Vuforia Web Services or the Vuforia
 Cloud Recognition Web API.
 """
 
-from requests import Response
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from requests import Response
 
 
 class CloudRecoException(Exception):
     """
     Base class for Vuforia Cloud Recognition Web API exceptions.
     """
```

### Comparing `vws-python-2023.3.5/src/vws/exceptions/cloud_reco_exceptions.py` & `vws-python-2023.5.21/src/vws/exceptions/cloud_reco_exceptions.py`

 * *Files identical despite different names*

### Comparing `vws-python-2023.3.5/src/vws/exceptions/vws_exceptions.py` & `vws-python-2023.5.21/src/vws/exceptions/vws_exceptions.py`

 * *Files identical despite different names*

### Comparing `vws-python-2023.3.5/src/vws/query.py` & `vws-python-2023.5.21/src/vws/query.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 """
 Tools for interacting with the Vuforia Cloud Recognition Web APIs.
 """
 
 from __future__ import annotations
 
 import datetime
-import io
 from http import HTTPStatus
+from typing import Any, BinaryIO
 from urllib.parse import urljoin
 
 import requests
 from urllib3.filepost import encode_multipart_formdata
 from vws_auth_tools import authorization_header, rfc_1123_date
 
 from vws.exceptions.cloud_reco_exceptions import (
     AuthenticationFailure,
     BadImage,
     InactiveProject,
     MaxNumResultsOutOfRange,
     RequestTimeTooSkewed,
 )
 from vws.exceptions.custom_exceptions import (
-    ActiveMatchingTargetsDeleteProcessing,
     RequestEntityTooLarge,
 )
 from vws.include_target_data import CloudRecoIncludeTargetData
 from vws.reports import QueryResult, TargetData
 
 
+def _get_image_data(image: BinaryIO) -> bytes:
+    original_tell = image.tell()
+    image.seek(0)
+    image_data = image.read()
+    image.seek(original_tell)
+    return image_data
+
+
 class CloudRecoService:
     """
     An interface to the Vuforia Cloud Recognition Web APIs.
     """
 
     def __init__(
         self,
@@ -47,15 +54,15 @@
         """
         self._client_access_key = client_access_key
         self._client_secret_key = client_secret_key
         self._base_vwq_url = base_vwq_url
 
     def query(
         self,
-        image: io.BytesIO,
+        image: BinaryIO,
         max_num_results: int = 1,
         include_target_data: CloudRecoIncludeTargetData = (
             CloudRecoIncludeTargetData.TOP
         ),
     ) -> list[QueryResult]:
         """
         Use the Vuforia Web Query API to make an Image Recognition Query.
@@ -83,38 +90,31 @@
             ~vws.exceptions.cloud_reco_exceptions.RequestTimeTooSkewed: There
                 is an error with the time sent to Vuforia.
             ~vws.exceptions.cloud_reco_exceptions.BadImage: There is a problem
                 with the given image.  For example, it must be a JPEG or PNG
                 file in the grayscale or RGB color space.
             ~vws.exceptions.custom_exceptions.RequestEntityTooLarge: The given
                 image is too large.
-            ~vws.exceptions.custom_exceptions.ActiveMatchingTargetsDeleteProcessing:
-                The given image matches a target which was recently deleted.
 
         Returns:
             An ordered list of target details of matching targets.
         """
-        image_content = image.getvalue()
-        body = {
+        image_content = _get_image_data(image=image)
+        body: dict[str, Any] = {
             "image": ("image.jpeg", image_content, "image/jpeg"),
             "max_num_results": (None, int(max_num_results), "text/plain"),
             "include_target_data": (
                 None,
                 include_target_data.value,
                 "text/plain",
             ),
         }
         date = rfc_1123_date()
         request_path = "/v1/query"
-        (
-            content,
-            content_type_header,
-        ) = encode_multipart_formdata(  # type:ignore[no-untyped-call]
-            fields=body,
-        )
+        content, content_type_header = encode_multipart_formdata(fields=body)
         method = "POST"
 
         authorization_string = authorization_header(
             access_key=self._client_access_key,
             secret_key=self._client_secret_key,
             method=method,
             content=content,
@@ -141,28 +141,25 @@
 
         if response.status_code == HTTPStatus.REQUEST_ENTITY_TOO_LARGE:
             raise RequestEntityTooLarge
 
         if "Integer out of range" in response.text:
             raise MaxNumResultsOutOfRange(response=response)
 
-        if "No content to map due to end-of-input" in response.text:
-            raise ActiveMatchingTargetsDeleteProcessing
-
         result_code = response.json()["result_code"]
         if result_code != "Success":
             exception = {
                 "AuthenticationFailure": AuthenticationFailure,
                 "BadImage": BadImage,
                 "InactiveProject": InactiveProject,
                 "RequestTimeTooSkewed": RequestTimeTooSkewed,
             }[result_code]
             raise exception(response=response)
 
-        result = []
+        result: list[QueryResult] = []
         result_list = list(response.json()["results"])
         for item in result_list:
             target_data: TargetData | None = None
             if "target_data" in item:
                 target_data_dict = item["target_data"]
                 metadata = target_data_dict["application_metadata"]
                 timestamp_string = target_data_dict["target_timestamp"]
```

### Comparing `vws-python-2023.3.5/src/vws/reports.py` & `vws-python-2023.5.21/src/vws/reports.py`

 * *Files identical despite different names*

### Comparing `vws-python-2023.3.5/src/vws/vws.py` & `vws-python-2023.5.21/src/vws/vws.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """
 Tools for interacting with Vuforia APIs.
 """
 
 from __future__ import annotations
 
 import base64
-import io
 import json
+import time
 from datetime import date
-from time import sleep
+from typing import TYPE_CHECKING, BinaryIO
 from urllib.parse import urljoin
 
 import requests
-from func_timeout import func_set_timeout
-from func_timeout.exceptions import FunctionTimedOut
 from requests import Response
 from vws_auth_tools import authorization_header, rfc_1123_date
 
 from vws.exceptions.custom_exceptions import (
     TargetProcessingTimeout,
     UnknownVWSErrorPossiblyBadName,
 )
@@ -43,14 +41,25 @@
     DatabaseSummaryReport,
     TargetRecord,
     TargetStatusAndRecord,
     TargetStatuses,
     TargetSummaryReport,
 )
 
+if TYPE_CHECKING:
+    import io
+
+
+def _get_image_data(image: BinaryIO) -> bytes:
+    original_tell = image.tell()
+    image.seek(0)
+    image_data = image.read()
+    image.seek(original_tell)
+    return image_data
+
 
 def _target_api_request(
     server_access_key: str,
     server_secret_key: str,
     method: str,
     content: bytes,
     request_path: str,
@@ -197,15 +206,15 @@
 
         raise exception(response=response)
 
     def add_target(
         self,
         name: str,
         width: int | float,
-        image: io.BytesIO,
+        image: BinaryIO,
         application_metadata: str | None,
         *,
         active_flag: bool,
     ) -> str:
         """
         Add a target to a Vuforia Web Services database.
 
@@ -248,15 +257,15 @@
             ~vws.exceptions.vws_exceptions.RequestTimeTooSkewed: There is an
                 error with the time sent to Vuforia.
             ~vws.exceptions.custom_exceptions.UnknownVWSErrorPossiblyBadName:
                 Vuforia returns an HTML page with the text "Oops, an error
                 occurred". This has been seen to happen when the given name
                 includes a bad character.
         """
-        image_data = image.getvalue()
+        image_data = _get_image_data(image=image)
         image_data_encoded = base64.b64encode(image_data).decode("ascii")
 
         data = {
             "name": name,
             "width": width,
             "image": image_data_encoded,
             "active_flag": active_flag,
@@ -317,67 +326,33 @@
             reco_rating=target_record_dict["reco_rating"],
         )
         return TargetStatusAndRecord(
             status=status,
             target_record=target_record,
         )
 
-    def _wait_for_target_processed(
-        self,
-        target_id: str,
-        seconds_between_requests: float,
-    ) -> None:
-        """
-        Wait indefinitely for a target to get past the processing stage.
-
-        Args:
-            target_id: The ID of the target to wait for.
-            seconds_between_requests: The number of seconds to wait between
-                requests made while polling the target status.
-
-        Raises:
-            ~vws.exceptions.vws_exceptions.AuthenticationFailure: The secret
-                key is not correct.
-            ~vws.exceptions.vws_exceptions.Fail: There was an error with the
-                request. For example, the given access key does not match a
-                known database.
-            TimeoutError: The target remained in the processing stage for more
-                than five minutes.
-            ~vws.exceptions.vws_exceptions.UnknownTarget: The given target ID
-                does not match a target in the database.
-            ~vws.exceptions.vws_exceptions.RequestTimeTooSkewed: There is an
-                error with the time sent to Vuforia.
-        """
-        while True:
-            report = self.get_target_summary_report(target_id=target_id)
-            if report.status != TargetStatuses.PROCESSING:
-                return
-
-            sleep(seconds_between_requests)
-
     def wait_for_target_processed(
         self,
         target_id: str,
         seconds_between_requests: float = 0.2,
-        timeout_seconds: float | None = 60 * 5,
+        timeout_seconds: float = 60 * 5,
     ) -> None:
         """
         Wait up to five minutes (arbitrary) for a target to get past the
         processing stage.
 
         Args:
             target_id: The ID of the target to wait for.
             seconds_between_requests: The number of seconds to wait between
                 requests made while polling the target status.
                 We wait 0.2 seconds by default, rather than less, than that to
                 decrease the number of calls made to the API, to decrease the
                 likelihood of hitting the request quota.
             timeout_seconds: The maximum number of seconds to wait for the
-                target to be processed. If ``None`` is given, no maximum is
-                applied.
+                target to be processed.
 
         Raises:
             ~vws.exceptions.vws_exceptions.AuthenticationFailure: The secret
                 key is not correct.
             ~vws.exceptions.vws_exceptions.Fail: There was an error with the
                 request. For example, the given access key does not match a
                 known database.
@@ -385,27 +360,25 @@
                 target remained in the processing stage for more than
                 ``timeout_seconds`` seconds.
             ~vws.exceptions.vws_exceptions.UnknownTarget: The given target ID
                 does not match a target in the database.
             ~vws.exceptions.vws_exceptions.RequestTimeTooSkewed: There is an
                 error with the time sent to Vuforia.
         """
+        start_time = time.monotonic()
+        while True:
+            report = self.get_target_summary_report(target_id=target_id)
+            if report.status != TargetStatuses.PROCESSING:
+                return
+
+            elapsed_time = time.monotonic() - start_time
+            if elapsed_time > timeout_seconds:  # pragma: no cover
+                raise TargetProcessingTimeout
 
-        # func_timeout does not have type hints.
-        @func_set_timeout(timeout=timeout_seconds)  # type: ignore[misc]
-        def decorated() -> None:
-            self._wait_for_target_processed(
-                target_id=target_id,
-                seconds_between_requests=seconds_between_requests,
-            )
-
-        try:
-            decorated()
-        except FunctionTimedOut as exc:
-            raise TargetProcessingTimeout from exc
+            time.sleep(seconds_between_requests)
 
     def list_targets(self) -> list[str]:
         """
         List target IDs.
 
         See
         https://library.vuforia.com/articles/Solution/How-To-Use-the-Vuforia-Web-Services-API#How-To-Get-a-Target-List-for-a-Cloud-Database.
@@ -637,15 +610,15 @@
         if name is not None:
             data["name"] = name
 
         if width is not None:
             data["width"] = width
 
         if image is not None:
-            image_data = image.getvalue()
+            image_data = _get_image_data(image=image)
             image_data_encoded = base64.b64encode(image_data).decode("ascii")
             data["image"] = image_data_encoded
 
         if active_flag is not None:
             data["active_flag"] = active_flag
 
         if application_metadata is not None:
```

### Comparing `vws-python-2023.3.5/src/vws_python.egg-info/PKG-INFO` & `vws-python-2023.5.21/src/vws_python.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vws-python
-Version: 2023.3.5
+Version: 2023.5.21
 Summary: Interact with the Vuforia Web Services (VWS) API.
 Author-email: Adam Dangoor <adamdangoor@gmail.com>
 License: The MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,42 +28,72 @@
 Project-URL: Documentation, https://vws-python.readthedocs.io/en/latest/
 Keywords: vuforia,vws,client
 Classifier: Operating System :: POSIX
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 |Build Status| |codecov| |PyPI| |Documentation Status|
 
 vws-python
 ==========
 
-Python library for the Vuforia Web Services (VWS) API and the Vuforia Web Query API.
+Python library for the Vuforia Web Services (VWS) API and the Vuforia
+Web Query API.
 
 Installation
 ------------
 
 .. code:: sh
 
    pip install vws-python
 
-This is tested on Python 3.11+.
-Get in touch with ``adamdangoor@gmail.com`` if you would like to use this with another language.
+This is tested on Python 3.11+. Get in touch with
+``adamdangoor@gmail.com`` if you would like to use this with another
+language.
 
 Getting Started
 ---------------
 
-.. code:: python
+.. invisible-code-block: python
+
+   import contextlib
+   import pathlib
+   import shutil
+
+   import vws_test_fixtures
+   from mock_vws import MockVWS
+   from mock_vws.database import VuforiaDatabase
+
+   mock = MockVWS(real_http=False)
+   database = VuforiaDatabase(
+       server_access_key='[server-access-key]',
+       server_secret_key='[server-secret-key]',
+       client_access_key='[client-access-key]',
+       client_secret_key='[client-secret-key]',
+   )
+   mock.add_database(database=database)
+   stack = contextlib.ExitStack()
+   stack.enter_context(mock)
+
+   # We rely on implementation details of the fixtures package.
+   image = pathlib.Path(vws_test_fixtures.__path__[0]) / 'high_quality_image.jpg'
+   assert image.exists(), image.resolve()
+   new_image = pathlib.Path('high_quality_image.jpg')
+   shutil.copy(image, new_image)
 
-   import io
+
+.. code-block:: python
+
+   import pathlib
 
    from vws import VWS, CloudRecoService
 
    server_access_key = '[server-access-key]'
    server_secret_key = '[server-secret-key]'
    client_access_key = '[client-access-key]'
    client_secret_key = '[client-secret-key]'
@@ -74,37 +104,40 @@
    )
    cloud_reco_client = CloudRecoService(
        client_access_key=client_access_key,
        client_secret_key=client_secret_key,
    )
    name = 'my_image_name'
 
-   with open('/path/to/image.png', 'rb') as my_image_file:
-      my_image = io.BytesIO(my_image_file.read())
-
-   target_id = vws_client.add_target(
-       name=name,
-       width=1,
-       image=my_image,
-       active_flag=True,
-       application_metadata=None,
-   )
-   vws_client.wait_for_target_processed(target_id=target_id)
-   matching_targets = cloud_reco_client.query(image=my_image)
+   image = pathlib.Path('high_quality_image.jpg')
+   with image.open(mode='rb') as my_image_file:
+       target_id = vws_client.add_target(
+           name=name,
+           width=1,
+           image=my_image_file,
+           active_flag=True,
+           application_metadata=None,
+       )
+       vws_client.wait_for_target_processed(target_id=target_id)
+       matching_targets = cloud_reco_client.query(image=my_image_file)
 
    assert matching_targets[0].target_id == target_id
 
+.. invisible-code-block: python
+   new_image = pathlib.Path('high_quality_image.jpg')
+   new_image.unlink()
+   stack.close()
 
 Full Documentation
 ------------------
 
-See the `full documentation <https://vws-python.readthedocs.io/en/latest>`__.
+See the `full
+documentation <https://vws-python.readthedocs.io/en/latest>`__.
 
 .. |Build Status| image:: https://github.com/VWS-Python/vws-python/workflows/CI/badge.svg
    :target: https://github.com/VWS-Python/vws-python/actions
 .. |codecov| image:: https://codecov.io/gh/VWS-Python/vws-python/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/VWS-Python/vws-python
-.. |Documentation Status| image:: https://readthedocs.org/projects/vws-python/badge/?version=latest
-   :target: https://vws-python.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
 .. |PyPI| image:: https://badge.fury.io/py/VWS-Python.svg
    :target: https://badge.fury.io/py/VWS-Python
+.. |Documentation Status| image:: https://readthedocs.org/projects/vws-python/badge/?version=latest
+   :target: https://vws-python.readthedocs.io/en/latest/?badge=latest
```

### Comparing `vws-python-2023.3.5/src/vws_python.egg-info/SOURCES.txt` & `vws-python-2023.5.21/src/vws_python.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,35 +4,34 @@
 CHANGELOG.rst
 CODE_OF_CONDUCT.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 codecov.yaml
+conftest.py
 lint.mk
 pyproject.toml
 readthedocs.yaml
-setup.py
 spelling_private_dict.txt
 .github/dependabot.yml
 .github/workflows/ci.yml
 .github/workflows/release.yml
 .github/workflows/windows-ci.yml
+.vscode/extensions.json
+.vscode/settings.json
 docs/Makefile
 docs/source/__init__.py
 docs/source/api-reference.rst
 docs/source/changelog.rst
 docs/source/conf.py
 docs/source/contributing.rst
 docs/source/exceptions.rst
 docs/source/index.rst
 docs/source/release-process.rst
-requirements/dev-requirements.txt
-requirements/requirements.txt
-requirements/setup-requirements.txt
 src/vws/__init__.py
 src/vws/include_target_data.py
 src/vws/py.typed
 src/vws/query.py
 src/vws/reports.py
 src/vws/vws.py
 src/vws/exceptions/__init__.py
@@ -45,11 +44,10 @@
 src/vws_python.egg-info/dependency_links.txt
 src/vws_python.egg-info/not-zip-safe
 src/vws_python.egg-info/requires.txt
 src/vws_python.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_cloud_reco_exceptions.py
-tests/test_meta.py
 tests/test_query.py
 tests/test_vws.py
 tests/test_vws_exceptions.py
```

### Comparing `vws-python-2023.3.5/src/vws_python.egg-info/requires.txt` & `vws-python-2023.5.21/src/vws_python.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 VWS-Auth-Tools
-func-timeout
 requests
 urllib3
 
 [dev]
 PyYAML==6.0
-Pygments==2.14.0
+Pygments==2.15.1
 Sphinx-Substitution-Extensions==2022.2.16
-Sphinx==6.1.3
-VWS-Python-Mock==2021.12.27.3
-VWS-Test-Fixtures==2022.1.3
-black==23.1.0
+Sphinx==7.0.1
+VWS-Python-Mock==2023.5.21
+VWS-Test-Fixtures==2023.3.5
+black==23.3.0
 check-manifest==0.49
 doc8==1.1.1
 dodgy==0.2.1
 freezegun==1.2.2
-furo==2022.12.7
-mypy==1.0.1
+furo==2023.5.20
+mypy==1.3.0
+pdm==2.6.1
 pip_check_reqs==2.4.4
 pydocstyle==6.3.0
 pyenchant==3.2.2
-pylint==2.15.5
+pyright==1.1.309
+pylint==2.17.4
 pyroma==4.2
 pytest-cov==4.0.0
-pytest==7.2.2
-ruff==0.0.254
-sphinx-autodoc-typehints==1.22
+pytest==7.3.1
+ruff==0.0.269
+sphinx-autodoc-typehints==1.23.0
 sphinx-prompt==1.5.0
 sphinxcontrib-spelling==8.0.0
-types-freezegun==1.1.10
-types-requests==2.28.11.15
-types-setuptools==67.4.0.3
+sybil==5.0.2
+types-requests==2.30.0.0
 vulture==2.7
```

### Comparing `vws-python-2023.3.5/tests/test_query.py` & `vws-python-2023.5.21/tests/test_query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 """
 Tests for the ``CloudRecoService`` querying functionality.
 """
 
-import io
+from __future__ import annotations
+
 import uuid
+from typing import TYPE_CHECKING
 
 from mock_vws import MockVWS
 from mock_vws.database import VuforiaDatabase
 from vws import VWS, CloudRecoService
 from vws.include_target_data import CloudRecoIncludeTargetData
 
+if TYPE_CHECKING:
+    import io
+
 
 class TestQuery:
     """
     Tests for making image queries.
     """
 
     @staticmethod
     def test_no_matches(
         cloud_reco_client: CloudRecoService,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         An empty list is returned if there are no matches.
         """
-        result = cloud_reco_client.query(image=high_quality_image)
+        result = cloud_reco_client.query(image=image)
         assert result == []
 
     @staticmethod
     def test_match(
         vws_client: VWS,
         cloud_reco_client: CloudRecoService,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         Details of matching targets are returned.
         """
         target_id = vws_client.add_target(
             name="x",
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         vws_client.wait_for_target_processed(target_id=target_id)
-        [matching_target] = cloud_reco_client.query(image=high_quality_image)
+        [matching_target] = cloud_reco_client.query(image=image)
         assert matching_target.target_id == target_id
 
 
 class TestCustomBaseVWQURL:
     """
     Tests for using a custom base VWQ URL.
     """
 
     @staticmethod
-    def test_custom_base_url(high_quality_image: io.BytesIO) -> None:
+    def test_custom_base_url(image: io.BytesIO) -> None:
         """
         It is possible to use query a target to a database under a custom VWQ
         URL.
         """
         base_vwq_url = "http://example.com"
         with MockVWS(base_vwq_url=base_vwq_url) as mock:
             database = VuforiaDatabase()
@@ -67,238 +72,238 @@
                 server_access_key=database.server_access_key,
                 server_secret_key=database.server_secret_key,
             )
 
             target_id = vws_client.add_target(
                 name="x",
                 width=1,
-                image=high_quality_image,
+                image=image,
                 active_flag=True,
                 application_metadata=None,
             )
 
             vws_client.wait_for_target_processed(target_id=target_id)
 
             cloud_reco_client = CloudRecoService(
                 client_access_key=database.client_access_key,
                 client_secret_key=database.client_secret_key,
                 base_vwq_url=base_vwq_url,
             )
 
-            matches = cloud_reco_client.query(image=high_quality_image)
+            matches = cloud_reco_client.query(image=image)
             assert len(matches) == 1
             match = matches[0]
             assert match.target_id == target_id
 
 
 class TestMaxNumResults:
     """
     Tests for the ``max_num_results`` parameter of ``query``.
     """
 
     @staticmethod
     def test_default(
         vws_client: VWS,
         cloud_reco_client: CloudRecoService,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         By default the maximum number of results is 1.
         """
         target_id = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         target_id_2 = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         vws_client.wait_for_target_processed(target_id=target_id)
         vws_client.wait_for_target_processed(target_id=target_id_2)
-        matches = cloud_reco_client.query(image=high_quality_image)
+        matches = cloud_reco_client.query(image=image)
         assert len(matches) == 1
 
     @staticmethod
     def test_custom(
         vws_client: VWS,
         cloud_reco_client: CloudRecoService,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         It is possible to set a custom ``max_num_results``.
         """
         target_id = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         target_id_2 = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         target_id_3 = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         vws_client.wait_for_target_processed(target_id=target_id)
         vws_client.wait_for_target_processed(target_id=target_id_2)
         vws_client.wait_for_target_processed(target_id=target_id_3)
         max_num_results = 2
         matches = cloud_reco_client.query(
-            image=high_quality_image,
+            image=image,
             max_num_results=max_num_results,
         )
         assert len(matches) == max_num_results
 
 
 class TestIncludeTargetData:
     """
     Tests for the ``include_target_data`` parameter of ``query``.
     """
 
     @staticmethod
     def test_default(
         vws_client: VWS,
         cloud_reco_client: CloudRecoService,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         By default, target data is only returned in the top match.
         """
         target_id = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         target_id_2 = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         vws_client.wait_for_target_processed(target_id=target_id)
         vws_client.wait_for_target_processed(target_id=target_id_2)
         top_match, second_match = cloud_reco_client.query(
-            image=high_quality_image,
+            image=image,
             max_num_results=2,
         )
         assert top_match.target_data is not None
         assert second_match.target_data is None
 
     @staticmethod
     def test_top(
         vws_client: VWS,
         cloud_reco_client: CloudRecoService,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         When ``CloudRecoIncludeTargetData.TOP`` is given, target data is only
         returned in the top match.
         """
         target_id = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         target_id_2 = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         vws_client.wait_for_target_processed(target_id=target_id)
         vws_client.wait_for_target_processed(target_id=target_id_2)
         top_match, second_match = cloud_reco_client.query(
-            image=high_quality_image,
+            image=image,
             max_num_results=2,
             include_target_data=CloudRecoIncludeTargetData.TOP,
         )
         assert top_match.target_data is not None
         assert second_match.target_data is None
 
     @staticmethod
     def test_none(
         vws_client: VWS,
         cloud_reco_client: CloudRecoService,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         When ``CloudRecoIncludeTargetData.NONE`` is given, target data is not
         returned in any match.
         """
         target_id = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         target_id_2 = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         vws_client.wait_for_target_processed(target_id=target_id)
         vws_client.wait_for_target_processed(target_id=target_id_2)
         top_match, second_match = cloud_reco_client.query(
-            image=high_quality_image,
+            image=image,
             max_num_results=2,
             include_target_data=CloudRecoIncludeTargetData.NONE,
         )
         assert top_match.target_data is None
         assert second_match.target_data is None
 
     @staticmethod
     def test_all(
         vws_client: VWS,
         cloud_reco_client: CloudRecoService,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         When ``CloudRecoIncludeTargetData.ALL`` is given, target data is
         returned in all matches.
         """
         target_id = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         target_id_2 = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         vws_client.wait_for_target_processed(target_id=target_id)
         vws_client.wait_for_target_processed(target_id=target_id_2)
         top_match, second_match = cloud_reco_client.query(
-            image=high_quality_image,
+            image=image,
             max_num_results=2,
             include_target_data=CloudRecoIncludeTargetData.ALL,
         )
         assert top_match.target_data is not None
         assert second_match.target_data is not None
```

### Comparing `vws-python-2023.3.5/tests/test_vws.py` & `vws-python-2023.5.21/tests/test_vws.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,43 +2,46 @@
 Tests for helper functions for managing a Vuforia database.
 """
 
 from __future__ import annotations
 
 import base64
 import datetime
-import io
 import random
 import uuid
+from typing import TYPE_CHECKING, BinaryIO
 
 import pytest
 from freezegun import freeze_time
 from mock_vws import MockVWS
 from mock_vws.database import VuforiaDatabase
 from vws import VWS, CloudRecoService
 from vws.exceptions.custom_exceptions import TargetProcessingTimeout
 from vws.reports import (
     DatabaseSummaryReport,
     TargetRecord,
     TargetStatuses,
     TargetSummaryReport,
 )
 
+if TYPE_CHECKING:
+    import io
+
 
 class TestAddTarget:
     """
     Tests for adding a target.
     """
 
     @staticmethod
     @pytest.mark.parametrize("application_metadata", [None, b"a"])
     @pytest.mark.parametrize("active_flag", [True, False])
     def test_add_target(
         vws_client: VWS,
-        high_quality_image: io.BytesIO,
+        image: BinaryIO,
         application_metadata: bytes | None,
         cloud_reco_client: CloudRecoService,
         *,
         active_flag: bool,
     ) -> None:
         """
         No exception is raised when adding one target.
@@ -50,62 +53,62 @@
         else:
             encoded_metadata_bytes = base64.b64encode(application_metadata)
             encoded_metadata = encoded_metadata_bytes.decode("utf-8")
 
         target_id = vws_client.add_target(
             name=name,
             width=width,
-            image=high_quality_image,
+            image=image,
             application_metadata=encoded_metadata,
             active_flag=active_flag,
         )
         target_record = vws_client.get_target_record(
             target_id=target_id,
         ).target_record
         assert target_record.name == name
         assert target_record.width == width
         assert target_record.active_flag is active_flag
         vws_client.wait_for_target_processed(target_id=target_id)
-        matching_targets = cloud_reco_client.query(image=high_quality_image)
+        matching_targets = cloud_reco_client.query(image=image)
         if active_flag:
             [matching_target] = matching_targets
             assert matching_target.target_id == target_id
             assert matching_target.target_data is not None
             query_metadata = matching_target.target_data.application_metadata
             assert query_metadata == encoded_metadata
         else:
             assert matching_targets == []
 
     @staticmethod
     def test_add_two_targets(
         vws_client: VWS,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         No exception is raised when adding two targets with different names.
 
         This demonstrates that the image seek position is not changed.
         """
         for name in ("a", "b"):
             vws_client.add_target(
                 name=name,
                 width=1,
-                image=high_quality_image,
+                image=image,
                 active_flag=True,
                 application_metadata=None,
             )
 
 
 class TestCustomBaseVWSURL:
     """
     Tests for using a custom base VWS URL.
     """
 
     @staticmethod
-    def test_custom_base_url(high_quality_image: io.BytesIO) -> None:
+    def test_custom_base_url(image: io.BytesIO) -> None:
         """
         It is possible to use add a target to a database under a custom VWS
         URL.
         """
         base_vws_url = "http://example.com"
         with MockVWS(base_vws_url=base_vws_url) as mock:
             database = VuforiaDatabase()
@@ -115,67 +118,67 @@
                 server_secret_key=database.server_secret_key,
                 base_vws_url=base_vws_url,
             )
 
             vws_client.add_target(
                 name="x",
                 width=1,
-                image=high_quality_image,
+                image=image,
                 active_flag=True,
                 application_metadata=None,
             )
 
 
 class TestListTargets:
     """
     Tests for listing targets.
     """
 
     @staticmethod
     def test_list_targets(
         vws_client: VWS,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         It is possible to get a list of target IDs.
         """
         id_1 = vws_client.add_target(
             name="x",
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         id_2 = vws_client.add_target(
             name="a",
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         assert sorted(vws_client.list_targets()) == sorted([id_1, id_2])
 
 
 class TestDelete:
     """
     Test for deleting a target.
     """
 
     @staticmethod
     def test_delete_target(
         vws_client: VWS,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         It is possible to delete a target.
         """
         target_id = vws_client.add_target(
             name="x",
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
 
         vws_client.wait_for_target_processed(target_id=target_id)
         assert target_id in vws_client.list_targets()
         vws_client.delete_target(target_id=target_id)
@@ -186,26 +189,26 @@
     """
     Tests for getting a summary report for a target.
     """
 
     @staticmethod
     def test_get_target_summary_report(
         vws_client: VWS,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         Details of a target are returned by ``get_target_summary_report``.
         """
         date = "2018-04-25"
         target_name = uuid.uuid4().hex
         with freeze_time(date):
             target_id = vws_client.add_target(
                 name=target_name,
                 width=1,
-                image=high_quality_image,
+                image=image,
                 active_flag=True,
                 application_metadata=None,
             )
 
         result = vws_client.get_target_summary_report(target_id=target_id)
 
         expected_report = TargetSummaryReport(
@@ -255,23 +258,23 @@
     """
     Tests for getting a record of a target.
     """
 
     @staticmethod
     def test_get_target_record(
         vws_client: VWS,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         Details of a target are returned by ``get_target_record``.
         """
         target_id = vws_client.add_target(
             name="x",
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
 
         result = vws_client.get_target_record(target_id=target_id)
         expected_target_record = TargetRecord(
             target_id=target_id,
@@ -290,35 +293,35 @@
     """
     Tests for waiting for a target to be processed.
     """
 
     @staticmethod
     def test_wait_for_target_processed(
         vws_client: VWS,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         It is possible to wait until a target is processed.
         """
         target_id = vws_client.add_target(
             name="x",
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         report = vws_client.get_target_summary_report(target_id=target_id)
         assert report.status == TargetStatuses.PROCESSING
         vws_client.wait_for_target_processed(target_id=target_id)
         report = vws_client.get_target_summary_report(target_id=target_id)
         assert report.status != TargetStatuses.PROCESSING
 
     @staticmethod
     def test_default_seconds_between_requests(
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         By default, 0.2 seconds are waited between polling requests.
         """
         with MockVWS(processing_time_seconds=0.5) as mock:
             database = VuforiaDatabase()
             mock.add_database(database=database)
@@ -326,15 +329,15 @@
                 server_access_key=database.server_access_key,
                 server_secret_key=database.server_secret_key,
             )
 
             target_id = vws_client.add_target(
                 name="x",
                 width=1,
-                image=high_quality_image,
+                image=image,
                 active_flag=True,
                 application_metadata=None,
             )
 
             vws_client.wait_for_target_processed(target_id=target_id)
             report = vws_client.get_database_summary_report()
             expected_requests = (
@@ -362,15 +365,15 @@
             # At the time of writing there is a bug which prevents request
             # usage from being tracked so we cannot track this.
             expected_requests = 0
             assert report.request_usage == expected_requests
 
     @staticmethod
     def test_custom_seconds_between_requests(
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         It is possible to customize the time waited between polling requests.
         """
         with MockVWS(processing_time_seconds=0.5) as mock:
             database = VuforiaDatabase()
             mock.add_database(database=database)
@@ -378,15 +381,15 @@
                 server_access_key=database.server_access_key,
                 server_secret_key=database.server_secret_key,
             )
 
             target_id = vws_client.add_target(
                 name="x",
                 width=1,
-                image=high_quality_image,
+                image=image,
                 active_flag=True,
                 application_metadata=None,
             )
 
             vws_client.wait_for_target_processed(
                 target_id=target_id,
                 seconds_between_requests=0.3,
@@ -413,30 +416,30 @@
             )
             # At the time of writing there is a bug which prevents request
             # usage from being tracked so we cannot track this.
             expected_requests = 0
             assert report.request_usage == expected_requests
 
     @staticmethod
-    def test_custom_timeout(high_quality_image: io.BytesIO) -> None:
+    def test_custom_timeout(image: io.BytesIO) -> None:
         """
         It is possible to set a maximum timeout.
         """
         with MockVWS(processing_time_seconds=0.5) as mock:
             database = VuforiaDatabase()
             mock.add_database(database=database)
             vws_client = VWS(
                 server_access_key=database.server_access_key,
                 server_secret_key=database.server_secret_key,
             )
 
             target_id = vws_client.add_target(
                 name="x",
                 width=1,
-                image=high_quality_image,
+                image=image,
                 active_flag=True,
                 application_metadata=None,
             )
 
             report = vws_client.get_target_summary_report(target_id=target_id)
             assert report.status == TargetStatuses.PROCESSING
             with pytest.raises(TargetProcessingTimeout):
@@ -457,30 +460,30 @@
     """
     Tests for getting duplicate targets.
     """
 
     @staticmethod
     def test_get_duplicate_targets(
         vws_client: VWS,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         It is possible to get the IDs of similar targets.
         """
         target_id = vws_client.add_target(
             name="x",
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         similar_target_id = vws_client.add_target(
             name="a",
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
 
         vws_client.wait_for_target_processed(target_id=target_id)
         vws_client.wait_for_target_processed(target_id=similar_target_id)
         duplicates = vws_client.get_duplicate_targets(target_id=target_id)
@@ -491,32 +494,32 @@
     """
     Tests for updating a target.
     """
 
     @staticmethod
     def test_update_target(
         vws_client: VWS,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
         different_high_quality_image: io.BytesIO,
         cloud_reco_client: CloudRecoService,
     ) -> None:
         """
         It is possible to update a target.
         """
         old_name = uuid.uuid4().hex
         old_width = random.uniform(a=0.01, b=50)
         target_id = vws_client.add_target(
             name=old_name,
             width=old_width,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         vws_client.wait_for_target_processed(target_id=target_id)
-        [matching_target] = cloud_reco_client.query(image=high_quality_image)
+        [matching_target] = cloud_reco_client.query(image=image)
         assert matching_target.target_id == target_id
         query_target_data = matching_target.target_data
         assert query_target_data is not None
         query_metadata = query_target_data.application_metadata
         assert query_metadata is None
 
         new_name = uuid.uuid4().hex
@@ -550,21 +553,21 @@
         assert target_details.target_record.name == new_name
         assert target_details.target_record.width == new_width
         assert not target_details.target_record.active_flag
 
     @staticmethod
     def test_no_fields_given(
         vws_client: VWS,
-        high_quality_image: io.BytesIO,
+        image: io.BytesIO,
     ) -> None:
         """
         It is possible to give no update fields.
         """
         target_id = vws_client.add_target(
             name="x",
             width=1,
-            image=high_quality_image,
+            image=image,
             active_flag=True,
             application_metadata=None,
         )
         vws_client.wait_for_target_processed(target_id=target_id)
         vws_client.update_target(target_id=target_id)
```

### Comparing `vws-python-2023.3.5/tests/test_vws_exceptions.py` & `vws-python-2023.5.21/tests/test_vws_exceptions.py`

 * *Files identical despite different names*

