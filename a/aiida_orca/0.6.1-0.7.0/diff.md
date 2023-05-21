# Comparing `tmp/aiida_orca-0.6.1.tar.gz` & `tmp/aiida_orca-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_orca-0.6.1.tar", last modified: Thu Feb 16 21:15:53 2023, max compression
+gzip compressed data, was "aiida_orca-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_orca-0.6.1.tar` & `aiida_orca-0.7.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     2650 2023-02-16 21:15:49.454423 aiida_orca-0.6.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      711 2023-02-16 21:15:49.454423 aiida_orca-0.6.1/.github/workflows/publish_on_pypi.yml
--rw-r--r--   0        0        0     1203 2023-02-16 21:15:49.454423 aiida_orca-0.6.1/.gitignore
--rw-r--r--   0        0        0     1431 2023-02-16 21:15:49.454423 aiida_orca-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      119 2023-02-16 21:15:49.454423 aiida_orca-0.6.1/.readthedocs.yml
--rw-r--r--   0        0        0     1078 2023-02-16 21:15:49.454423 aiida_orca-0.6.1/LICENSE
--rw-r--r--   0        0        0       19 2023-02-16 21:15:49.454423 aiida_orca-0.6.1/MANIFEST.in
--rw-r--r--   0        0        0     5050 2023-02-16 21:15:49.454423 aiida_orca-0.6.1/README.md
--rw-r--r--   0        0        0       71 2023-02-16 21:15:49.454423 aiida_orca-0.6.1/aiida_orca/__init__.py
--rw-r--r--   0        0        0      128 2023-02-16 21:15:49.454423 aiida_orca-0.6.1/aiida_orca/calculations/__init__.py
--rw-r--r--   0        0        0     1319 2023-02-16 21:15:49.454423 aiida_orca-0.6.1/aiida_orca/calculations/orca_asa.py
--rw-r--r--   0        0        0     6181 2023-02-16 21:15:49.454423 aiida_orca-0.6.1/aiida_orca/calculations/orca_orca.py
--rw-r--r--   0        0        0     4710 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/aiida_orca/parsers/__init__.py
--rw-r--r--   0        0        0     1526 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/aiida_orca/parsers/cclib/LICENSE
--rw-r--r--   0        0        0       43 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/aiida_orca/parsers/cclib/__init__.py
--rw-r--r--   0        0        0     1009 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/aiida_orca/parsers/cclib/ccio.py
--rw-r--r--   0        0        0    21650 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/aiida_orca/parsers/cclib/data.py
--rw-r--r--   0        0        0    19078 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/aiida_orca/parsers/cclib/logfileparser.py
--rw-r--r--   0        0        0   103986 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/aiida_orca/parsers/cclib/orcaparser.py
--rw-r--r--   0        0        0     2237 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/aiida_orca/parsers/cclib/utils.py
--rw-r--r--   0        0        0      102 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/aiida_orca/utils/__init__.py
--rw-r--r--   0        0        0     1050 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/aiida_orca/utils/input_generator.py
--rw-r--r--   0        0        0       95 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/aiida_orca/workchains/__init__.py
--rw-r--r--   0        0        0     3377 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/aiida_orca/workchains/base.py
--rw-r--r--   0        0        0        7 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/docs/.gitignore
--rwxr-xr-x   0        0        0     1547 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/docs/Makefile
--rwxr-xr-x   0        0        0    11685 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/docs/source/conf.py
--rw-r--r--   0        0        0     1350 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/docs/source/developer_guide/index.rst
--rw-r--r--   0        0        0    76300 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/docs/source/images/AiiDA_transparent_logo.png
--rwxr-xr-x   0        0        0     1081 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/docs/source/index.rst
--rw-r--r--   0        0        0     2718 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/docs/source/rtd_settings.py
--rw-r--r--   0        0        0      624 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/docs/source/user_guide/get_started.rst
--rw-r--r--   0        0        0       94 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/docs/source/user_guide/index.rst
--rw-r--r--   0        0        0       93 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/docs/source/user_guide/tutorial.rst
--rw-r--r--   0        0        0      248 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/examples/ch4.xyz
--rw-r--r--   0        0        0      709 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/examples/conftest.py
--rw-r--r--   0        0        0     2584 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/examples/example_0.py
--rw-r--r--   0        0        0     3146 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/examples/example_1.py
--rw-r--r--   0        0        0     2784 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/examples/example_2.py
--rw-r--r--   0        0        0     3112 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/examples/example_3.py
--rw-r--r--   0        0        0     2977 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/examples/example_4.py
--rw-r--r--   0        0        0     2353 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/examples/example_5.py
--rw-r--r--   0        0        0      123 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/examples/h2co.xyz
--rw-r--r--   0        0        0       66 2023-02-16 21:15:49.458423 aiida_orca-0.6.1/examples/pytest.ini
--rw-r--r--   0        0        0   645627 2023-02-16 21:15:49.462423 aiida_orca-0.6.1/miscellaneous/ackn_logo.png
--rw-r--r--   0        0        0  1426431 2023-02-16 21:15:49.474423 aiida_orca-0.6.1/miscellaneous/aiida-orca_logo.png
--rw-r--r--   0        0        0     3540 2023-02-16 21:15:49.474423 aiida_orca-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2581 2023-02-16 21:15:49.474423 aiida_orca-0.6.1/tests/calculations/test_orca.py
--rw-r--r--   0        0        0      145 2023-02-16 21:15:49.474423 aiida_orca-0.6.1/tests/calculations/test_orca/test_default.in
--rw-r--r--   0        0        0     7218 2023-02-16 21:15:49.474423 aiida_orca-0.6.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-02-16 21:15:49.474423 aiida_orca-0.6.1/tests/parsers/__init__.py
--rw-r--r--   0        0        0   106842 2023-02-16 21:15:49.474423 aiida_orca-0.6.1/tests/parsers/fixtures/orca/default/aiida.out
--rw-r--r--   0        0        0      369 2023-02-16 21:15:49.474423 aiida_orca-0.6.1/tests/parsers/fixtures/orca/default/aiida.xyz
--rw-r--r--   0        0        0      369 2023-02-16 21:15:49.478423 aiida_orca-0.6.1/tests/parsers/fixtures/orca/missing_stdout/aiida.xyz
--rw-r--r--   0        0        0    47067 2023-02-16 21:15:49.478423 aiida_orca-0.6.1/tests/parsers/fixtures/orca/tddft/aiida.out
--rw-r--r--   0        0        0    54547 2023-02-16 21:15:49.478423 aiida_orca-0.6.1/tests/parsers/fixtures/orca/unrestricted/aiida.out
--rw-r--r--   0        0        0      172 2023-02-16 21:15:49.478423 aiida_orca-0.6.1/tests/parsers/fixtures/orca/unsuccessful/README
--rw-r--r--   0        0        0   106380 2023-02-16 21:15:49.478423 aiida_orca-0.6.1/tests/parsers/fixtures/orca/unsuccessful/aiida.out
--rw-r--r--   0        0        0      369 2023-02-16 21:15:49.478423 aiida_orca-0.6.1/tests/parsers/fixtures/orca/unsuccessful/aiida.xyz
--rw-r--r--   0        0        0     4738 2023-02-16 21:15:49.478423 aiida_orca-0.6.1/tests/parsers/test_orca.py
--rw-r--r--   0        0        0     8697 2023-02-16 21:15:49.478423 aiida_orca-0.6.1/tests/parsers/test_orca/test_orca_default.yml
--rw-r--r--   0        0        0     3663 2023-02-16 21:15:49.478423 aiida_orca-0.6.1/tests/parsers/test_orca/test_orca_tddft.yml
--rw-r--r--   0        0        0     5522 2023-02-16 21:15:49.478423 aiida_orca-0.6.1/tests/parsers/test_orca/test_orca_unrestricted.yml
--rw-r--r--   0        0        0     8698 2023-02-16 21:15:49.478423 aiida_orca-0.6.1/tests/parsers/test_orca/test_orca_unsuccessful.yml
--rw-r--r--   0        0        0     6636 1970-01-01 00:00:00.000000 aiida_orca-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     2650 2023-05-21 21:53:01.212263 aiida_orca-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      711 2023-05-21 21:53:01.212263 aiida_orca-0.7.0/.github/workflows/publish_on_pypi.yml
+-rw-r--r--   0        0        0     1203 2023-05-21 21:53:01.212263 aiida_orca-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1431 2023-05-21 21:53:01.212263 aiida_orca-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      119 2023-05-21 21:53:01.212263 aiida_orca-0.7.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1078 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/LICENSE
+-rw-r--r--   0        0        0       19 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/MANIFEST.in
+-rw-r--r--   0        0        0     5050 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/README.md
+-rw-r--r--   0        0        0       71 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/__init__.py
+-rw-r--r--   0        0        0      128 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/calculations/__init__.py
+-rw-r--r--   0        0        0     1319 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/calculations/orca_asa.py
+-rw-r--r--   0        0        0     5819 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/calculations/orca_orca.py
+-rw-r--r--   0        0        0     4680 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/parsers/__init__.py
+-rw-r--r--   0        0        0     1526 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/parsers/cclib/LICENSE
+-rw-r--r--   0        0        0       43 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/parsers/cclib/__init__.py
+-rw-r--r--   0        0        0     1009 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/parsers/cclib/ccio.py
+-rw-r--r--   0        0        0    21650 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/parsers/cclib/data.py
+-rw-r--r--   0        0        0    19078 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/parsers/cclib/logfileparser.py
+-rw-r--r--   0        0        0   103986 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/parsers/cclib/orcaparser.py
+-rw-r--r--   0        0        0     2237 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/parsers/cclib/utils.py
+-rw-r--r--   0        0        0      102 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/utils/__init__.py
+-rw-r--r--   0        0        0     1050 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/utils/input_generator.py
+-rw-r--r--   0        0        0       95 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/workchains/__init__.py
+-rw-r--r--   0        0        0     3377 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/aiida_orca/workchains/base.py
+-rw-r--r--   0        0        0        7 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/docs/.gitignore
+-rwxr-xr-x   0        0        0     1547 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/docs/Makefile
+-rwxr-xr-x   0        0        0    11685 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1350 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/docs/source/developer_guide/index.rst
+-rw-r--r--   0        0        0    76300 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/docs/source/images/AiiDA_transparent_logo.png
+-rwxr-xr-x   0        0        0     1081 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/docs/source/index.rst
+-rw-r--r--   0        0        0     2718 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/docs/source/rtd_settings.py
+-rw-r--r--   0        0        0      624 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/docs/source/user_guide/get_started.rst
+-rw-r--r--   0        0        0       94 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/docs/source/user_guide/index.rst
+-rw-r--r--   0        0        0       93 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/docs/source/user_guide/tutorial.rst
+-rw-r--r--   0        0        0      248 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/examples/ch4.xyz
+-rw-r--r--   0        0        0      709 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/examples/conftest.py
+-rw-r--r--   0        0        0     2654 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/examples/example_0.py
+-rw-r--r--   0        0        0     3146 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/examples/example_1.py
+-rw-r--r--   0        0        0     2784 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/examples/example_2.py
+-rw-r--r--   0        0        0     3112 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/examples/example_3.py
+-rw-r--r--   0        0        0     2977 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/examples/example_4.py
+-rw-r--r--   0        0        0     2353 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/examples/example_5.py
+-rw-r--r--   0        0        0      123 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/examples/h2co.xyz
+-rw-r--r--   0        0        0       66 2023-05-21 21:53:01.216263 aiida_orca-0.7.0/examples/pytest.ini
+-rw-r--r--   0        0        0   645627 2023-05-21 21:53:01.220263 aiida_orca-0.7.0/miscellaneous/ackn_logo.png
+-rw-r--r--   0        0        0  1426431 2023-05-21 21:53:01.232263 aiida_orca-0.7.0/miscellaneous/aiida-orca_logo.png
+-rw-r--r--   0        0        0     3540 2023-05-21 21:53:01.232263 aiida_orca-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2532 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/calculations/test_orca.py
+-rw-r--r--   0        0        0      145 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/calculations/test_orca/test_default.in
+-rw-r--r--   0        0        0     7218 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/__init__.py
+-rw-r--r--   0        0        0   106842 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/fixtures/orca/default/aiida.out
+-rw-r--r--   0        0        0      369 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/fixtures/orca/default/aiida.xyz
+-rw-r--r--   0        0        0      369 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/fixtures/orca/missing_stdout/aiida.xyz
+-rw-r--r--   0        0        0    47067 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/fixtures/orca/tddft/aiida.out
+-rw-r--r--   0        0        0    54547 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/fixtures/orca/unrestricted/aiida.out
+-rw-r--r--   0        0        0      172 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/fixtures/orca/unsuccessful/README
+-rw-r--r--   0        0        0   106380 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/fixtures/orca/unsuccessful/aiida.out
+-rw-r--r--   0        0        0      369 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/fixtures/orca/unsuccessful/aiida.xyz
+-rw-r--r--   0        0        0     4738 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/test_orca.py
+-rw-r--r--   0        0        0     8697 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/test_orca/test_orca_default.yml
+-rw-r--r--   0        0        0     3663 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/test_orca/test_orca_tddft.yml
+-rw-r--r--   0        0        0     5522 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/test_orca/test_orca_unrestricted.yml
+-rw-r--r--   0        0        0     8698 2023-05-21 21:53:01.236263 aiida_orca-0.7.0/tests/parsers/test_orca/test_orca_unsuccessful.yml
+-rw-r--r--   0        0        0     6636 1970-01-01 00:00:00.000000 aiida_orca-0.7.0/PKG-INFO
```

### Comparing `aiida_orca-0.6.1/.github/workflows/ci.yml` & `aiida_orca-0.7.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/.github/workflows/publish_on_pypi.yml` & `aiida_orca-0.7.0/.github/workflows/publish_on_pypi.yml`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/.gitignore` & `aiida_orca-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/.pre-commit-config.yaml` & `aiida_orca-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/LICENSE` & `aiida_orca-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/README.md` & `aiida_orca-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/aiida_orca/calculations/orca_asa.py` & `aiida_orca-0.7.0/aiida_orca/calculations/orca_asa.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/aiida_orca/calculations/orca_orca.py` & `aiida_orca-0.7.0/aiida_orca/calculations/orca_orca.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,17 +37,14 @@
         spec.input(
             'parameters',
             valid_type=Dict,
             serializer=to_aiida_type,
             required=True,
             help='Input parameters to generate the input file.'
         )
-        spec.input(
-            'settings', valid_type=Dict, serializer=to_aiida_type, required=False, help='Additional input parameters'
-        )
         spec.input_namespace(
             'file',
             valid_type=SinglefileData,
             required=False,
             help='Additional input files like gbw or hessian',
             dynamic=True
         )
@@ -91,19 +88,17 @@
 
         # create input structure
         self._write_structure(self.inputs.structure, folder, self._INPUT_COORDS_FILE)
 
         # create ORCA input file
         self._write_input_file(self.inputs.parameters, folder, self._INPUT_FILE)
 
-        settings = self.inputs.settings.get_dict() if 'settings' in self.inputs else {}
-
         # create code info
         codeinfo = CodeInfo()
-        codeinfo.cmdline_params = settings.pop('cmdline', []) + [self._INPUT_FILE]
+        codeinfo.cmdline_params = [self._INPUT_FILE]
         codeinfo.stdout_name = self._OUTPUT_FILE
         codeinfo.join_files = True
         codeinfo.code_uuid = self.inputs.code.uuid
 
         # create calc info
         calcinfo = CalcInfo()
         calcinfo.cmdline_params = codeinfo.cmdline_params
@@ -117,16 +112,15 @@
             for name, obj in self.inputs.file.items():
                 if name == 'gbw':
                     calcinfo.local_copy_list.append((obj.uuid, obj.filename, 'aiida_old.gbw'))
                 else:
                     calcinfo.local_copy_list.append((obj.uuid, obj.filename, obj.filename))
 
         # Retrieve list
-        calcinfo.retrieve_list = [self._OUTPUT_FILE, self._GBW_FILE, self._HESSIAN_FILE, self._RELAX_COORDS_FILE]
-        calcinfo.retrieve_list += settings.pop('additional_retrieve_list', [])
+        calcinfo.retrieve_list = [self._OUTPUT_FILE, self._HESSIAN_FILE, self._RELAX_COORDS_FILE]
         return calcinfo
 
     def _write_input_file(self, parameters: Dict, folder: Folder, filename: str) -> None:
         """Function that writes ORCA input file"""
         params = parameters.get_dict()
 
         charge = params.get('charge')
```

### Comparing `aiida_orca-0.6.1/aiida_orca/parsers/__init__.py` & `aiida_orca-0.7.0/aiida_orca/parsers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 """AiiDA-ORCA output parser"""
 import pathlib
-import shutil
-import tempfile
 import traceback
 
 import ase.io
 import numpy as np
 
 from aiida.parsers import Parser
 from aiida.common import OutputParsingError, NotExistent
```

### Comparing `aiida_orca-0.6.1/aiida_orca/parsers/cclib/LICENSE` & `aiida_orca-0.7.0/aiida_orca/parsers/cclib/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/aiida_orca/parsers/cclib/ccio.py` & `aiida_orca-0.7.0/aiida_orca/parsers/cclib/ccio.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/aiida_orca/parsers/cclib/data.py` & `aiida_orca-0.7.0/aiida_orca/parsers/cclib/data.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/aiida_orca/parsers/cclib/logfileparser.py` & `aiida_orca-0.7.0/aiida_orca/parsers/cclib/logfileparser.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/aiida_orca/parsers/cclib/orcaparser.py` & `aiida_orca-0.7.0/aiida_orca/parsers/cclib/orcaparser.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/aiida_orca/parsers/cclib/utils.py` & `aiida_orca-0.7.0/aiida_orca/parsers/cclib/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/aiida_orca/utils/input_generator.py` & `aiida_orca-0.7.0/aiida_orca/utils/input_generator.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/aiida_orca/workchains/base.py` & `aiida_orca-0.7.0/aiida_orca/workchains/base.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/docs/Makefile` & `aiida_orca-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/docs/source/conf.py` & `aiida_orca-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/docs/source/developer_guide/index.rst` & `aiida_orca-0.7.0/docs/source/developer_guide/index.rst`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/docs/source/images/AiiDA_transparent_logo.png` & `aiida_orca-0.7.0/docs/source/images/AiiDA_transparent_logo.png`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/docs/source/index.rst` & `aiida_orca-0.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/docs/source/rtd_settings.py` & `aiida_orca-0.7.0/docs/source/rtd_settings.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/docs/source/user_guide/get_started.rst` & `aiida_orca-0.7.0/docs/source/user_guide/get_started.rst`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/examples/conftest.py` & `aiida_orca-0.7.0/examples/conftest.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/examples/example_0.py` & `aiida_orca-0.7.0/examples/example_0.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     # Construct process builder
     builder = OrcaCalculation.get_builder()
 
     builder.structure = structure
     builder.parameters = parameters
     builder.code = orca_code
 
+    builder.metadata.options.additional_retrieve_list = ['aiida.gbw']
     # 'withmpi' needs to be always set to False even for parallel
     # calculations, because ORCA uses mpirun internally.
     builder.metadata.options.withmpi = False
     builder.metadata.options.resources = {
         'num_machines': 1,
         'num_mpiprocs_per_machine': nproc,
     }
```

### Comparing `aiida_orca-0.6.1/examples/example_1.py` & `aiida_orca-0.7.0/examples/example_1.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/examples/example_2.py` & `aiida_orca-0.7.0/examples/example_2.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/examples/example_3.py` & `aiida_orca-0.7.0/examples/example_3.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/examples/example_4.py` & `aiida_orca-0.7.0/examples/example_4.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/examples/example_5.py` & `aiida_orca-0.7.0/examples/example_5.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/miscellaneous/ackn_logo.png` & `aiida_orca-0.7.0/miscellaneous/ackn_logo.png`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/miscellaneous/aiida-orca_logo.png` & `aiida_orca-0.7.0/miscellaneous/aiida-orca_logo.png`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/pyproject.toml` & `aiida_orca-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/tests/calculations/test_orca.py` & `aiida_orca-0.7.0/tests/calculations/test_orca.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,15 @@
     entry_point_name = 'orca.orca'
 
     inputs = generate_inputs_orca()
     calc_info, dirpath = generate_calc_job(entry_point_name, inputs)
 
     # pylint: disable=protected-access
     cmdline_params = [OrcaCalculation._INPUT_FILE]
-    retrieve_list = [
-        OrcaCalculation._OUTPUT_FILE, OrcaCalculation._GBW_FILE, OrcaCalculation._HESSIAN_FILE,
-        OrcaCalculation._RELAX_COORDS_FILE
-    ]
+    retrieve_list = [OrcaCalculation._OUTPUT_FILE, OrcaCalculation._HESSIAN_FILE, OrcaCalculation._RELAX_COORDS_FILE]
     filenames_written = [OrcaCalculation._INPUT_FILE, OrcaCalculation._INPUT_COORDS_FILE]
 
     # Check the attributes of the returned `CalcInfo`
     assert isinstance(calc_info, datastructures.CalcInfo)
     assert isinstance(calc_info.codes_info[0], datastructures.CodeInfo)
     assert sorted(calc_info.codes_info[0].cmdline_params) == cmdline_params
     assert sorted(calc_info.retrieve_list) == sorted(retrieve_list)
```

### Comparing `aiida_orca-0.6.1/tests/conftest.py` & `aiida_orca-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/tests/parsers/fixtures/orca/default/aiida.out` & `aiida_orca-0.7.0/tests/parsers/fixtures/orca/default/aiida.out`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/tests/parsers/fixtures/orca/tddft/aiida.out` & `aiida_orca-0.7.0/tests/parsers/fixtures/orca/tddft/aiida.out`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/tests/parsers/fixtures/orca/unrestricted/aiida.out` & `aiida_orca-0.7.0/tests/parsers/fixtures/orca/unrestricted/aiida.out`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/tests/parsers/fixtures/orca/unsuccessful/aiida.out` & `aiida_orca-0.7.0/tests/parsers/fixtures/orca/unsuccessful/aiida.out`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/tests/parsers/test_orca.py` & `aiida_orca-0.7.0/tests/parsers/test_orca.py`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/tests/parsers/test_orca/test_orca_default.yml` & `aiida_orca-0.7.0/tests/parsers/test_orca/test_orca_default.yml`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/tests/parsers/test_orca/test_orca_tddft.yml` & `aiida_orca-0.7.0/tests/parsers/test_orca/test_orca_tddft.yml`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/tests/parsers/test_orca/test_orca_unrestricted.yml` & `aiida_orca-0.7.0/tests/parsers/test_orca/test_orca_unrestricted.yml`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/tests/parsers/test_orca/test_orca_unsuccessful.yml` & `aiida_orca-0.7.0/tests/parsers/test_orca/test_orca_unsuccessful.yml`

 * *Files identical despite different names*

### Comparing `aiida_orca-0.6.1/PKG-INFO` & `aiida_orca-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida_orca
-Version: 0.6.1
+Version: 0.7.0
 Summary: AiiDA-Orca plugin
 Keywords: aiida,orca
 Author-email: Pezhman Zarabadi-Poor <pzarabadip@gmail.com>, Daniel Hollas <danekhollas@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
```

