# Comparing `tmp/ansible-compat-4.0.4.tar.gz` & `tmp/ansible-compat-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-compat-4.0.4.tar", last modified: Mon May 15 16:44:56 2023, max compression
+gzip compressed data, was "ansible-compat-4.0.5.tar", last modified: Sun May 21 12:32:44 2023, max compression
```

## Comparing `ansible-compat-4.0.4.tar` & `ansible-compat-4.0.5.tar`

### file list

```diff
@@ -1,115 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.000491 ansible-compat-4.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.004491 ansible-compat-4.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.004491 ansible-compat-4.0.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.004491 ansible-compat-4.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.004491 ansible-compat-4.0.4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.988491 ansible-compat-4.0.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.004491 ansible-compat-4.0.4/examples/reqs_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/examples/reqs_v1/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.004491 ansible-compat-4.0.4/examples/reqs_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/examples/reqs_v2/community-molecule-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/examples/reqs_v2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.988491 ansible-compat-4.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.012491 ansible-compat-4.0.4/src/ansible_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31718 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/src/ansible_compat/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.012491 ansible-compat-4.0.4/src/ansible_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 16:44:55.000000 ansible-compat-4.0.4/src/ansible_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-15 16:44:55.000000 ansible-compat-4.0.4/src/ansible_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:44:55.000000 ansible-compat-4.0.4/src/ansible_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-15 16:44:55.000000 ansible-compat-4.0.4/src/ansible_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 16:44:55.000000 ansible-compat-4.0.4/src/ansible_compat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.016491 ansible-compat-4.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.016491 ansible-compat-4.0.4/test/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/assets/requirements-invalid-collection.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/assets/requirements-invalid-role.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/assets/validate0_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/assets/validate0_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/assets/validate0_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/collections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/collections/acme.broken/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.broken/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/collections/acme.goodies/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/collections/acme.goodies/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/collections/acme.goodies/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/collections/acme.goodies/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/roles/baz/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/collections/acme.goodies/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/collections/acme.goodies/tests/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.020491 ansible-compat-4.0.4/test/roles/acme.missing_deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/test/roles/acme.missing_deps/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/roles/acme.missing_deps/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/roles/acme.missing_deps/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/roles/acme.sample2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/test/roles/acme.sample2/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/roles/acme.sample2/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/roles/ansible-role-sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/test/roles/ansible-role-sample/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/roles/ansible-role-sample/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.992491 ansible-compat-4.0.4/test/roles/sample3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/test/roles/sample3/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/roles/sample3/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:55.996491 ansible-compat-4.0.4/test/roles/sample4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:44:56.024491 ansible-compat-4.0.4/test/roles/sample4/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/roles/sample4/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_configuration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    25190 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_runtime_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/test/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-15 16:44:40.000000 ansible-compat-4.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/examples/reqs_broken/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/examples/reqs_broken/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/examples/reqs_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/examples/reqs_v1/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/examples/reqs_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/examples/reqs_v2/community-molecule-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/examples/reqs_v2/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/src/ansible_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31920 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/src/ansible_compat/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/src/ansible_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-21 12:32:44.000000 ansible-compat-4.0.5/src/ansible_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-21 12:32:44.000000 ansible-compat-4.0.5/src/ansible_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 12:32:44.000000 ansible-compat-4.0.5/src/ansible_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-21 12:32:44.000000 ansible-compat-4.0.5/src/ansible_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-21 12:32:44.000000 ansible-compat-4.0.5/src/ansible_compat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.492278 ansible-compat-4.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/assets/requirements-invalid-collection.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/assets/requirements-invalid-role.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/assets/validate0_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/assets/validate0_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/assets/validate0_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/test/collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/collections/acme.broken/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.broken/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/collections/acme.goodies/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/test/collections/acme.goodies/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/collections/acme.goodies/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/test/collections/acme.goodies/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.484278 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/roles/baz/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/collections/acme.goodies/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/collections/acme.goodies/tests/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/roles/acme.missing_deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/roles/acme.missing_deps/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/roles/acme.missing_deps/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/roles/acme.missing_deps/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/test/roles/acme.sample2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/roles/acme.sample2/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/roles/acme.sample2/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/test/roles/ansible-role-sample/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/roles/ansible-role-sample/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/roles/ansible-role-sample/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/test/roles/sample3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/roles/sample3/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/roles/sample3/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.488278 ansible-compat-4.0.5/test/roles/sample4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 12:32:44.496278 ansible-compat-4.0.5/test/roles/sample4/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/roles/sample4/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_configuration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25494 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_runtime_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/test/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-21 12:32:28.000000 ansible-compat-4.0.5/tox.ini
```

### Comparing `ansible-compat-4.0.4/.github/dependabot.yml` & `ansible-compat-4.0.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/.github/workflows/release.yml` & `ansible-compat-4.0.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/.github/workflows/tox.yml` & `ansible-compat-4.0.5/.github/workflows/tox.yml`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
           other_names: |
             lint
             docs
             pkg
             py39-ansible212
             py39-ansible213
             py39-ansible214
+            py39-ansible215
             py311-devel
           platforms: linux,macos
           macos: minmax
   build:
     name: ${{ matrix.name }}
     runs-on: ${{ matrix.os || 'ubuntu-22.04' }}
     needs: pre
```

### Comparing `ansible-compat-4.0.4/.gitignore` & `ansible-compat-4.0.5/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -123,7 +123,8 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 .test-results
+*.lcov
```

### Comparing `ansible-compat-4.0.4/.pre-commit-config.yaml` & `ansible-compat-4.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/.readthedocs.yml` & `ansible-compat-4.0.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/.vscode/settings.json` & `ansible-compat-4.0.5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/LICENSE` & `ansible-compat-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/PKG-INFO` & `ansible-compat-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.0.4
+Version: 4.0.5
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.0.4/README.md` & `ansible-compat-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/docs/images/favicon.ico` & `ansible-compat-4.0.5/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/docs/images/logo.png` & `ansible-compat-4.0.5/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/docs/images/logo.svg` & `ansible-compat-4.0.5/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/examples/reqs_v2/community-molecule-0.1.0.tar.gz` & `ansible-compat-4.0.5/examples/reqs_v2/community-molecule-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/mkdocs.yml` & `ansible-compat-4.0.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/pyproject.toml` & `ansible-compat-4.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,19 @@
 
 [project.optional-dependencies]
 docs = ["argparse-manpage", "black", "mkdocs-ansible[lock]>=0.1.2"]
 test = ["coverage", "pip-tools", "pytest>=7.2.0", "pytest-mock", "pytest-plus"]
 
 [tool.coverage.run]
 source = ["src"]
-branch = true
+# Do not use branch until bug is fixes:
+# https://github.com/nedbat/coveragepy/issues/605
+branch = false
+parallel = true
+concurrency = ["multiprocessing", "thread"]
 
 [tool.coverage.report]
 exclude_lines = ["pragma: no cover", "if TYPE_CHECKING:"]
 fail_under = 93
 skip_covered = true
 show_missing = true
```

### Comparing `ansible-compat-4.0.4/requirements.txt` & `ansible-compat-4.0.5/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --extra=docs --extra=test --output-file=requirements.txt --resolver=backtracking --strip-extras --unsafe-package=ansible-core --unsafe-package=resolvelib --unsafe-package=typing_extensions pyproject.toml
 #
-argparse-manpage==4.1
+argparse-manpage==4.2
     # via ansible-compat (pyproject.toml)
 attrs==23.1.0
     # via jsonschema
 beautifulsoup4==4.12.1
     # via
     #   mkdocs-ansible
     #   mkdocs-htmlproofer-plugin
@@ -42,15 +42,15 @@
     #   mkdocs-ansible
     #   pip-tools
 colorama==0.4.6
     # via
     #   griffe
     #   mkdocs-ansible
     #   mkdocs-material
-coverage==7.2.4
+coverage==7.2.5
     # via ansible-compat (pyproject.toml)
 cryptography==40.0.2
     # via ansible-core
 csscompressor==0.9.5
     # via
     #   mkdocs-ansible
     #   mkdocs-minify-plugin
@@ -81,14 +81,16 @@
     #   mkdocs-ansible
     #   requests
 importlib-metadata==6.1.0
     # via
     #   markdown
     #   mkdocs
     #   mkdocs-ansible
+importlib-resources==5.0.7
+    # via ansible-core
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via
     #   ansible-core
     #   mkdocs
     #   mkdocs-ansible
@@ -178,15 +180,15 @@
     #   mkdocs-ansible
 pip==23.1.2
     # via pip-tools
 pip-tools==6.13.0
     # via ansible-compat (pyproject.toml)
 pipdeptree==2.7.0
     # via mkdocs-ansible
-platformdirs==3.5.0
+platformdirs==3.5.1
     # via black
 pluggy==1.0.0
     # via pytest
 pycparser==2.21
     # via
     #   cffi
     #   mkdocs-ansible
@@ -259,14 +261,16 @@
     #   mkdocs-ansible
     #   python-slugify
 tinycss2==1.2.1
     # via
     #   cairosvg
     #   cssselect2
     #   mkdocs-ansible
+toml==0.10.2
+    # via argparse-manpage
 tomli==2.0.1
     # via
     #   black
     #   build
     #   pyproject-hooks
     #   pytest
 typing-extensions==4.5.0 ; python_version < "3.10"
```

### Comparing `ansible-compat-4.0.4/src/ansible_compat/config.py` & `ansible-compat-4.0.5/src/ansible_compat/config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/src/ansible_compat/constants.py` & `ansible-compat-4.0.5/src/ansible_compat/constants.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 """Constants used by ansible_compat."""
 
 
+REQUIREMENT_LOCATIONS = [
+    "requirements.yml",
+    "roles/requirements.yml",
+    "collections/requirements.yml",
+    # These is more of less the official way to store test requirements in collections so far, comments shows number of repos using this reported by https://sourcegraph.com/ at the time of writing
+    "tests/requirements.yml",  # 170
+    "tests/integration/requirements.yml",  # 3
+    "tests/unit/requirements.yml",  # 1
+]
+
 # Minimal version of Ansible we support for runtime
 ANSIBLE_MIN_VERSION = "2.12"
 
 # Based on https://docs.ansible.com/ansible/latest/reference_appendices/config.html
 ANSIBLE_DEFAULT_ROLES_PATH = (
     "~/.ansible/roles:/usr/share/ansible/roles:/etc/ansible/roles"
 )
```

### Comparing `ansible-compat-4.0.4/src/ansible_compat/errors.py` & `ansible-compat-4.0.5/src/ansible_compat/errors.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/src/ansible_compat/loaders.py` & `ansible-compat-4.0.5/src/ansible_compat/loaders.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/src/ansible_compat/prerun.py` & `ansible-compat-4.0.5/src/ansible_compat/prerun.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/src/ansible_compat/runtime.py` & `ansible-compat-4.0.5/src/ansible_compat/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 from packaging.version import Version
 
 from ansible_compat.config import (
     AnsibleConfig,
     ansible_collections_path,
     parse_ansible_version,
 )
-from ansible_compat.constants import MSG_INVALID_FQRL, RC_ANSIBLE_OPTIONS_ERROR
+from ansible_compat.constants import (
+    MSG_INVALID_FQRL,
+    RC_ANSIBLE_OPTIONS_ERROR,
+    REQUIREMENT_LOCATIONS,
+)
 from ansible_compat.errors import (
     AnsibleCommandError,
     AnsibleCompatError,
     InvalidPrerequisiteError,
     MissingAnsibleError,
 )
 from ansible_compat.loaders import colpath_from_path, yaml_from_file
@@ -407,14 +411,20 @@
         if not Path(requirement).exists():
             return
         reqs_yaml = yaml_from_file(Path(requirement))
         if not isinstance(reqs_yaml, (dict, list)):
             msg = f"{requirement} file is not a valid Ansible requirements file."
             raise InvalidPrerequisiteError(msg)
 
+        if isinstance(reqs_yaml, dict):
+            for key in reqs_yaml:
+                if key not in ("roles", "collections"):
+                    msg = f"{requirement} file is not a valid Ansible requirements file. Only 'roles' and 'collections' keys are allowed at root level. Recognized valid locations are: {', '.join(REQUIREMENT_LOCATIONS)}"
+                    raise InvalidPrerequisiteError(msg)
+
         if isinstance(reqs_yaml, list) or "roles" in reqs_yaml:
             cmd = [
                 "ansible-galaxy",
                 "role",
                 "install",
                 "-vr",
                 f"{requirement}",
@@ -481,21 +491,15 @@
         if required_collections is None:
             required_collections = {}
 
         # first one is standard for collection layout repos and the last two
         # are part of Tower specification
         # https://docs.ansible.com/ansible-tower/latest/html/userguide/projects.html#ansible-galaxy-support
         # https://docs.ansible.com/ansible-tower/latest/html/userguide/projects.html#collections-support
-        for req_file in [
-            "requirements.yml",
-            "roles/requirements.yml",
-            "collections/requirements.yml",
-            # These is more of less the official way to store test requirements in collections so far:
-            "tests/requirements.yml",
-        ]:
+        for req_file in REQUIREMENT_LOCATIONS:
             self.install_requirements(Path(req_file), retry=retry, offline=offline)
 
         galaxy_path = Path("galaxy.yml")
         if galaxy_path.exists():
             data = yaml_from_file(galaxy_path)
             if isinstance(data, dict) and "dependencies" in data:
                 for name, required_version in data["dependencies"].items():
```

### Comparing `ansible-compat-4.0.4/src/ansible_compat/schema.py` & `ansible-compat-4.0.5/src/ansible_compat/schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/src/ansible_compat/types.py` & `ansible-compat-4.0.5/src/ansible_compat/types.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/src/ansible_compat.egg-info/PKG-INFO` & `ansible-compat-4.0.5/src/ansible_compat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.0.4
+Version: 4.0.5
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.0.4/src/ansible_compat.egg-info/SOURCES.txt` & `ansible-compat-4.0.5/src/ansible_compat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 .vscode/extensions.json
 .vscode/settings.json
 docs/api.md
 docs/index.md
 docs/images/favicon.ico
 docs/images/logo.png
 docs/images/logo.svg
+examples/reqs_broken/requirements.yml
 examples/reqs_v1/requirements.yml
 examples/reqs_v2/community-molecule-0.1.0.tar.gz
 examples/reqs_v2/requirements.yml
 src/ansible_compat/__init__.py
 src/ansible_compat/config.py
 src/ansible_compat/constants.py
 src/ansible_compat/errors.py
```

### Comparing `ansible-compat-4.0.4/test/assets/validate0_expected.json` & `ansible-compat-4.0.5/test/assets/validate0_expected.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/test/collections/acme.goodies/galaxy.yml` & `ansible-compat-4.0.5/test/collections/acme.goodies/galaxy.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/test/conftest.py` & `ansible-compat-4.0.5/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/test/test_config.py` & `ansible-compat-4.0.5/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/test/test_runtime.py` & `ansible-compat-4.0.5/test/test_runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,21 @@
         )
         assert any(
             msg.startswith("Running ansible-galaxy collection install")
             for msg in caplog.messages
         )
 
 
+def test_prerun_reqs_broken(runtime: Runtime) -> None:
+    """Checks that the we report invalid requirements.yml file."""
+    path = (Path(__file__).parent.parent / "examples" / "reqs_broken").resolve()
+    with cwd(path), pytest.raises(InvalidPrerequisiteError):
+        runtime.prepare_environment()
+
+
 def test__update_env_no_old_value_no_default_no_value(monkeypatch: MonkeyPatch) -> None:
     """Make sure empty value does not touch environment."""
     monkeypatch.delenv("DUMMY_VAR", raising=False)
 
     runtime = Runtime()
     runtime._update_env("DUMMY_VAR", [])
```

### Comparing `ansible-compat-4.0.4/test/test_runtime_example.py` & `ansible-compat-4.0.5/test/test_runtime_example.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/test/test_schema.py` & `ansible-compat-4.0.5/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.0.4/tox.ini` & `ansible-compat-4.0.5/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 [tox]
 minversion = 4.0.0
 envlist =
   lint
   pkg
   docs
   # matrix assumed current (implicit) is 2.13:
-  py{39,310,311}{,-devel,-ansible212,-ansible213,-ansible214}
+  py{39,310,311}{,-devel,-ansible212,-ansible213,-ansible214,-ansible215}
 isolated_build = true
 skip_missing_interpreters = True
 skipsdist = true
 
 [testenv]
 description =
   Run the tests with {basepython}
   devel: ansible devel branch
   ansible212: ansible-core 2.12
   ansible213: ansible-core 2.13
   ansible214: ansible-core 2.14
+  ansible215: ansible-core 2.15
 
 deps =
   ansible212: ansible-core>=2.12,<2.13
   ansible213: ansible-core>=2.13,<2.14
   ansible214: ansible-core>=2.14,<2.15
+  ansible215: ansible-core>=2.15,<2.16
 
   devel: ansible-core @ git+https://github.com/ansible/ansible.git  # GPLv3+
   # avoid installing ansible-core on -devel envs:
   !devel: ansible-core
   --editable .[test]
 
 commands =
   sh -c "ansible --version | head -n 1"
   # We add coverage options but not making them mandatory as we do not want to force
   # pytest users to run coverage when they just want to run a single test with `pytest -k test`
   coverage run -m pytest {posargs:}
-  sh -c "coverage xml || true && coverage report"
+  sh -c "coverage combine -a -q --data-file=.coverage {toxworkdir}/.coverage.*"
+  # needed for upload to codecov.io
+  -sh -c "COVERAGE_FILE= coverage xml --ignore-errors -q --fail-under=0"
+  # needed for vscode integration due to https://github.com/ryanluker/vscode-coverage-gutters/issues/403
+  -sh -c "COVERAGE_FILE= coverage lcov --ignore-errors -q --fail-under=0"
+  sh -c "COVERAGE_FILE= coverage report"
   # We fail if files are modified at the end
   git diff --exit-code
+
 commands_pre =
   # safety measure to assure we do not accidentally run tests with broken dependencies
   {envpython} -m pip check
+  # cleaning needed to prevent errors between runs
+  sh -c "rm -f .coverage {toxworkdir}/.coverage.* 2>/dev/null || true"
 passenv =
   CURL_CA_BUNDLE  # https proxies, https://github.com/tox-dev/tox/issues/1437
   FORCE_COLOR
   HOME
   NO_COLOR
   PYTEST_*  # allows developer to define their own preferences
   PY_COLORS
@@ -50,18 +60,19 @@
   SSL_CERT_FILE  # https proxies
   LANG
   LC_ALL
   LC_CTYPE
 setenv =
   ANSIBLE_DEVEL_WARNING='false'
   COVERAGE_FILE = {env:COVERAGE_FILE:{toxworkdir}/.coverage.{envname}}
+  COVERAGE_PROCESS_START={toxinidir}/pyproject.toml
   PIP_DISABLE_PIP_VERSION_CHECK = 1
   PIP_CONSTRAINT = {toxinidir}/requirements.txt
   PRE_COMMIT_COLOR = always
-  PYTEST_REQPASS = 80
+  PYTEST_REQPASS = 81
   FORCE_COLOR = 1
 allowlist_externals =
   ansible
   git
   sh
 
 [testenv:lint]
```

