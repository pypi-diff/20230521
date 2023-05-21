# Comparing `tmp/ansible-lint-6.9.0.tar.gz` & `tmp/ansible-lint-6.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-lint-6.9.0.tar", last modified: Thu Nov 24 01:13:31 2022, max compression
+gzip compressed data, was "ansible-lint-6.9.1.tar", last modified: Sat Dec  3 21:00:15 2022, max compression
```

## Comparing `ansible-lint-6.9.0.tar` & `ansible-lint-6.9.1.tar`

### file list

```diff
@@ -1,701 +1,967 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.078473 ansible-lint-6.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3497 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.ansible-lint
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.010473 ansible-lint-6.9.0/.config/
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.config/ansible-lint.spec
--rw-r--r--   0 runner    (1001) docker     (121)     3189 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.darglint
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.010473 ansible-lint-6.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.010473 ansible-lint-6.9.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)     1851 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.010473 ansible-lint-6.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/workflows/redirects.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8986 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.packit.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6292 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     1282 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.010473 ansible-lint-6.9.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/DCO_1_1.md
--rw-r--r--   0 runner    (1001) docker     (121)     4348 2022-11-24 01:13:31.082473 ansible-lint-6.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2057 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     3542 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/_static/ansible-lint.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (121)    13320 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/_static/images/ansible-lint-512.png
--rw-r--r--   0 runner    (1001) docker     (121)    15406 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/_static/images/logo_invert.png
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (121)    10972 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/configuring.md
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (121)     4190 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/custom-rules.md
--rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/installing.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/docs/licenses/
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/licenses/LICENSE.mit.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5345 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/philosophy.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/docs/pkg/
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/pkg/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/redirects.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/docs/rules/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/rules/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/rules.md
--rw-r--r--   0 runner    (1001) docker     (121)     7522 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/docs/using-profiles.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/examples/.config/
--rw-r--r--   0 runner    (1001) docker     (121)     3497 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/.config/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/ansible-navigator.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/examples/broken/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/broken/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/broken/ansible-navigator.yml
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/broken/encoding.j2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/examples/broken/yaml-with-tabs/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/broken/yaml-with-tabs/invalid-due-tabs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.994473 ansible-lint-6.9.0/examples/broken_collection_meta_runtime/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/examples/broken_collection_meta_runtime/meta/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/broken_collection_meta_runtime/meta/runtime.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/examples/collection/
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/collection/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/examples/ee_broken/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/ee_broken/execution-environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/execution-environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/examples/group_vars/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/group_vars/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/examples/host_vars/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/host_vars/localhost.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/examples/inventory/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/inventory/broken_dev_inventory.yml
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/inventory/inventory.yml
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/inventory/production.yml
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/lineno.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/examples/meta/
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/meta/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/meta/runtime.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.014473 ansible-lint-6.9.0/examples/other/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/other/some.j2.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/other/some.yaml-too
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.026473 ansible-lint-6.9.0/examples/playbooks/
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/.ansible-lint-only-builtins-allow-collections
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/always-run-success.yml
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/become-user-without-become-failure.yml
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/become-user-without-become-success.yml
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/become.transformed.yml
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/become.yml
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/block.yml
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/blockincludes.yml
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/blockincludes2.yml
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/bracketsmatchtest.yml
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/command-check-failure.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/command-check-success.yml
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/common-include-1.yml
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/common-include-2.yml
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/conflicting_action.yml
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/contains_secrets.transformed.yml
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/contains_secrets.yml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/custom_module.yml
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/ematcher-rule.yml
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/empty_playbook.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/example.yml
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/extra_vars.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.026473 ansible-lint-6.9.0/examples/playbooks/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/handlers/included-handlers.yml
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/handlers/y.yml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/include-import-tasks-in-role.yml
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/include-in-block.yml
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/include.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3213 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/jinja-spacing.yml
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/jinja2-when-failure.yml
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/jinja2-when-success.yml
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/json-schema-fail.yml
--rw-r--r--   0 runner    (1001) docker     (121)    47347 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/lots_of_warnings.transformed.yml
--rw-r--r--   0 runner    (1001) docker     (121)    47347 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/lots_of_warnings.yml
--rw-r--r--   0 runner    (1001) docker     (121)      245 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/mocked_dependency.yml
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/multiline-brackets-do-not-match-test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/multiline-bracketsmatchtest.yml
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/name-templated.yml
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/no-prompting.yml
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/nomatches.yml
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/nomatchestest.transformed.yml
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/nomatchestest.yml
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/noqa-nested.yml
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/noqa.yml
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/norole.yml
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/norole2.yml
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/package-check-failure.yml
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/package-check-success.yml
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/pass-loop-var-prefix.yml
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/play-name-missing.yml
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/play.yml
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/play_miss_include.yml
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/playbook-imported.yml
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/playbook-parent.yml
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-avoid-implicit-fail.yml
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-avoid-implicit-pass.yml
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-fqcn-fail.yml
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-fqcn-pass.yml
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-jinja-invalid.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-jinja-valid.yml
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-key-order-fail.yml
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-no-free-form-fail.yml
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-no-free-form-pass.yml
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-no-handler-fail.yml
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-no-handler-pass.yml
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-no-tabs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-only-builtins.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-risky-file-permissions-fail.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-risky-file-permissions-pass.yml
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/rule-var-naming-fail.yml
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/run-once-fail.yml
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/run-once-pass.yml
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/schema-error-string.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/skiptasks.yml
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/strict-mode.yml
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/syntax-error-string.yml
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/syntax-error.yml
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/task-has-name-failure.yml
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/task-has-name-success.yml
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/task-name-lowercase.yml
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/taskimports.yml
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/taskincludes.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.026473 ansible-lint-6.9.0/examples/playbooks/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/tasks/conflicting-action-statements.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.026473 ansible-lint-6.9.0/examples/playbooks/tasks/directory with spaces/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/tasks/directory with spaces/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/tasks/empty_blocks.yml
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/tasks/include-in-block-inner.yml
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/tasks/included-with-lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/tasks/malformed.yml
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/tasks/nestedincludes.yml
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/tasks/passing_task.yml
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/tasks/simple_task.yml
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/tasks/varset.yml
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/tasks/varunset.yml
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/tasks/x.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.026473 ansible-lint-6.9.0/examples/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/templates/not-valid.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/test_import_with_conflicting_action_statements.yml
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/test_import_with_malformed.yml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/test_include_inplace.yml
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/test_include_relative.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/test_skip_inside_yaml.yml
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/unicode.transformed.yml
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/unicode.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/using-bare-variables-failure.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3984 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/using-bare-variables-success.yml
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/valid.yml
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/valid_with_alt_extension.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/playbooks/vars/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/vars/empty_vars.transformed.yml
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/vars/empty_vars.yml
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/vars/invalid_vars_schema.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/vars/jinja-spacing.yml
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/vars/not_decryptable.yml
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/vars/other.yml
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/vars/rule_jinja_vars.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/vars/strings.transformed.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/vars/strings.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/playbooks/vars/subfolder/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/vars/subfolder/settings.yml
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/with-skip-tag-id.yml
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/playbooks/with-umlaut-ä.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/reqs_v1/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/reqs_v1/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/reqs_v2/
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/reqs_v2/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/ansible-role-foo/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/ansible-role-foo/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/ansible-role-foo/tasks/main.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/bobbins/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/bobbins/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/bobbins/tasks/imported_tasks.yml
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/bobbins/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/broken_argument_specs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/broken_argument_specs/meta/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/broken_argument_specs/meta/argument_specs.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/dependency_in_meta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/dependency_in_meta/meta/
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/dependency_in_meta/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/hello/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/hello/meta/
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/hello/meta/argument_specs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/hello/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/include_in_the_place/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/include_in_the_place/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/include_in_the_place/tasks/included_file.yml
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/include_in_the_place/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/include_miss/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/include_miss/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/include_miss/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/include_relative/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/include_relative/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/include_relative/tasks/included_file.yml
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/include_relative/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/invalid-name/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/invalid-name/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/invalid-name/tasks/main.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/invalid_due_to_meta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/invalid_due_to_meta/meta/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/invalid_due_to_meta/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/invalid_due_to_meta/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/invalid_due_to_meta/tasks/main.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/invalid_meta_schema/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/invalid_meta_schema/meta/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/invalid_meta_schema/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/invalid_requirements_schema/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/invalid_requirements_schema/meta/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/invalid_requirements_schema/meta/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/invalud_meta_schema
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/loop_var_prefix/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/loop_var_prefix/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/loop_var_prefix/tasks/fail.yml
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/loop_var_prefix/tasks/pass.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/meta_noqa/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/meta_noqa/meta/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/meta_noqa/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/more_complex/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.030473 ansible-lint-6.9.0/examples/roles/more_complex/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/more_complex/handlers/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/more_complex/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/more_complex/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/role_for_no_same_owner/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/role_for_no_same_owner/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/role_for_no_same_owner/tasks/fail.yml
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/role_for_no_same_owner/tasks/pass.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/role_with_task_inclusions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/role_with_task_inclusions/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/role_with_task_inclusions/tasks/imported_tasks.yml
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/role_with_task_inclusions/tasks/included_tasks.yml
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/role_with_task_inclusions/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/subfolder/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/subfolder/other_role/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/subfolder/other_role/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/subfolder/other_role/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/template_lookup/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/template_lookup/files/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/template_lookup/files/a_file
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/template_lookup/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/template_lookup/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/template_lookup_missing/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/template_lookup_missing/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/template_lookup_missing/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/test-role/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/test-role/meta/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/test-role/meta/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/test-role/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/test-role/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/test-role/molecule/default/include-import-role.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/test-role/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/test-role/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/test-role/tasks/world.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/roles/valid-due-to-meta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/valid-due-to-meta/meta/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/valid-due-to-meta/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/valid-due-to-meta/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/valid-due-to-meta/tasks/debian/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/valid-due-to-meta/tasks/debian/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/valid-due-to-meta/tasks/main.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/var_naming_pattern/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/var_naming_pattern/.ansible-lint
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/roles/var_naming_pattern/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/roles/var_naming_pattern/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/rules/
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/rules/task_has_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:30.998473 ansible-lint-6.9.0/examples/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/templates/playbooks/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/templates/playbooks/playbook.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/examples/testproject/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/examples/testproject/roles/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/examples/testproject/roles/test-role/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.038473 ansible-lint-6.9.0/examples/testproject/roles/test-role/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/testproject/roles/test-role/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.042473 ansible-lint-6.9.0/examples/yamllint/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/yamllint/invalid.yml
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/yamllint/multi-document.yaml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/examples/yamllint/valid.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/playbook.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.042473 ansible-lint-6.9.0/plugins/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/plugins/modules/fake_module.py
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3732 2022-11-24 01:13:31.082473 ansible-lint-6.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.042473 ansible-lint-6.9.0/src/ansible_lint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4348 2022-11-24 01:13:30.000000 ansible-lint-6.9.0/src/ansible_lint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20054 2022-11-24 01:13:30.000000 ansible-lint-6.9.0/src/ansible_lint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-24 01:13:30.000000 ansible-lint-6.9.0/src/ansible_lint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-24 01:13:30.000000 ansible-lint-6.9.0/src/ansible_lint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-24 01:13:30.000000 ansible-lint-6.9.0/src/ansible_lint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-11-24 01:13:30.000000 ansible-lint-6.9.0/src/ansible_lint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-24 01:13:30.000000 ansible-lint-6.9.0/src/ansible_lint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.046473 ansible-lint-6.9.0/src/ansiblelint/
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15312 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.046473 ansible-lint-6.9.0/src/ansiblelint/_internal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/_internal/internal_error.md
--rw-r--r--   0 runner    (1001) docker     (121)     5832 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/_internal/rules.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/_internal/warning.md
--rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/_mockings.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-24 01:13:30.000000 ansible-lint-6.9.0/src/ansiblelint/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    13504 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/app.py
--rw-r--r--   0 runner    (1001) docker     (121)    19425 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4094 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/color.py
--rw-r--r--   0 runner    (1001) docker     (121)    10255 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3632 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.046473 ansible-lint-6.9.0/src/ansiblelint/data/
--rw-r--r--   0 runner    (1001) docker     (121)     4110 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/data/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5329 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    16390 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.046473 ansible-lint-6.9.0/src/ansiblelint/formatters/
--rw-r--r--   0 runner    (1001) docker     (121)    11052 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5492 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/generate_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.058473 ansible-lint-6.9.0/src/ansiblelint/rules/
--rw-r--r--   0 runner    (1001) docker     (121)    20039 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/avoid_implicit.md
--rw-r--r--   0 runner    (1001) docker     (121)     2149 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/avoid_implicit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/command_instead_of_module.md
--rw-r--r--   0 runner    (1001) docker     (121)     7511 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/command_instead_of_module.py
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/command_instead_of_shell.md
--rw-r--r--   0 runner    (1001) docker     (121)     5257 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/command_instead_of_shell.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.058473 ansible-lint-6.9.0/src/ansiblelint/rules/custom/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_bare_vars.md
--rw-r--r--   0 runner    (1001) docker     (121)     4093 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_bare_vars.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_command_syntax.md
--rw-r--r--   0 runner    (1001) docker     (121)     2755 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_command_syntax.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_local_action.md
--rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_local_action.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_module.md
--rw-r--r--   0 runner    (1001) docker     (121)     2045 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/empty_string_compare.md
--rw-r--r--   0 runner    (1001) docker     (121)     2865 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/empty_string_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     2731 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/fqcn.md
--rw-r--r--   0 runner    (1001) docker     (121)     5825 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/fqcn.py
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/galaxy.md
--rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/galaxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/ignore_errors.md
--rw-r--r--   0 runner    (1001) docker     (121)     3950 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/ignore_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/inline_env_var.md
--rw-r--r--   0 runner    (1001) docker     (121)     2664 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/inline_env_var.py
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/jinja.md
--rw-r--r--   0 runner    (1001) docker     (121)    26503 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/jinja.py
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/key_order.md
--rw-r--r--   0 runner    (1001) docker     (121)     4713 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/key_order.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/latest.md
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/latest.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/literal_compare.md
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/literal_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/loop_var_prefix.md
--rw-r--r--   0 runner    (1001) docker     (121)     3415 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/loop_var_prefix.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/meta_incorrect.md
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/meta_incorrect.py
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/meta_no_info.md
--rw-r--r--   0 runner    (1001) docker     (121)     2556 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/meta_no_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/meta_no_tags.md
--rw-r--r--   0 runner    (1001) docker     (121)     3344 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/meta_no_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/meta_video_links.md
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/meta_video_links.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/name.md
--rw-r--r--   0 runner    (1001) docker     (121)     5244 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/name.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_changed_when.md
--rw-r--r--   0 runner    (1001) docker     (121)     6945 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_changed_when.py
--rw-r--r--   0 runner    (1001) docker     (121)     1687 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_free_form.md
--rw-r--r--   0 runner    (1001) docker     (121)     4061 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_free_form.py
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_handler.md
--rw-r--r--   0 runner    (1001) docker     (121)     4912 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_jinja_when.md
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_jinja_when.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_log_password.md
--rw-r--r--   0 runner    (1001) docker     (121)     7770 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_log_password.py
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_prompting.md
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_prompting.py
--rw-r--r--   0 runner    (1001) docker     (121)     2677 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_relative_paths.md
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_relative_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_same_owner.md
--rw-r--r--   0 runner    (1001) docker     (121)     3456 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_same_owner.py
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_tabs.md
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/no_tabs.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/only_builtins.md
--rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/only_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/package_latest.md
--rw-r--r--   0 runner    (1001) docker     (121)     2619 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/package_latest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/partial_become.md
--rw-r--r--   0 runner    (1001) docker     (121)     5123 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/partial_become.py
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/playbook_extension.md
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/playbook_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/risky_file_permissions.md
--rw-r--r--   0 runner    (1001) docker     (121)     5677 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/risky_file_permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/risky_octal.md
--rw-r--r--   0 runner    (1001) docker     (121)     3789 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/risky_octal.py
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/risky_shell_pipe.md
--rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/risky_shell_pipe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/role_name.md
--rw-r--r--   0 runner    (1001) docker     (121)     4521 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/role_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/run_once.md
--rw-r--r--   0 runner    (1001) docker     (121)     2795 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/run_once.py
--rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/schema.md
--rw-r--r--   0 runner    (1001) docker     (121)     7309 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/syntax_check.md
--rw-r--r--   0 runner    (1001) docker     (121)     7952 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/syntax_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/var_naming.md
--rw-r--r--   0 runner    (1001) docker     (121)     9126 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/var_naming.py
--rw-r--r--   0 runner    (1001) docker     (121)     2033 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/yaml.md
--rw-r--r--   0 runner    (1001) docker     (121)     6197 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/rules/yaml_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     8821 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.058473 ansible-lint-6.9.0/src/ansiblelint/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2478 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/__store__.json
--rw-r--r--   0 runner    (1001) docker     (121)     4900 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/ansible-lint-config.json
--rw-r--r--   0 runner    (1001) docker     (121)    23497 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/ansible-navigator-config.json
--rw-r--r--   0 runner    (1001) docker     (121)     6401 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/arg_specs.json
--rw-r--r--   0 runner    (1001) docker     (121)     2139 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/execution-environment.json
--rw-r--r--   0 runner    (1001) docker     (121)    12674 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/galaxy.json
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/inventory.json
--rw-r--r--   0 runner    (1001) docker     (121)     3371 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     2893 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/meta-runtime.json
--rw-r--r--   0 runner    (1001) docker     (121)    32089 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/meta.json
--rw-r--r--   0 runner    (1001) docker     (121)    31636 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/playbook.json
--rw-r--r--   0 runner    (1001) docker     (121)     2957 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/requirements.json
--rw-r--r--   0 runner    (1001) docker     (121)    14107 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/tasks.json
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/schemas/vars.json
--rw-r--r--   0 runner    (1001) docker     (121)    10377 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/skip_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.058473 ansible-lint-6.9.0/src/ansiblelint/testing/
--rw-r--r--   0 runner    (1001) docker     (121)     4572 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2348 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/text.py
--rw-r--r--   0 runner    (1001) docker     (121)     5910 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)    32196 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    43645 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/src/ansiblelint/yaml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.066473 ansible-lint-6.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/bar.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.066473 ansible-lint-6.9.0/test/custom_rules/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/custom_rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.066473 ansible-lint-6.9.0/test/custom_rules/example_com/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/custom_rules/example_com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/custom_rules/example_com/example_com_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.066473 ansible-lint-6.9.0/test/custom_rules/example_inc/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/custom_rules/example_inc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/custom_rules/example_inc/custom_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.070473 ansible-lint-6.9.0/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/ansible-config-invalid.yml
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/ansible-config.yml
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/config-with-extra-vars.yml
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/config-with-relative-path.yml
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/config-with-write-all.yml
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/config-with-write-none.yml
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/config-with-write-subset.yml
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/exclude-paths-with-expands.yml
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/exclude-paths.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.070473 ansible-lint-6.9.0/test/fixtures/formatting-after/
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/formatting-after/fmt-1.yml
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/formatting-after/fmt-2.yml
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/formatting-after/fmt-3.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.070473 ansible-lint-6.9.0/test/fixtures/formatting-before/
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/formatting-before/fmt-1.yml
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/formatting-before/fmt-2.yml
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/formatting-before/fmt-3.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.070473 ansible-lint-6.9.0/test/fixtures/formatting-prettier/
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/formatting-prettier/fmt-1.yml
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/formatting-prettier/fmt-2.yml
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/formatting-prettier/fmt-3.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.070473 ansible-lint-6.9.0/test/fixtures/list-rules-tests/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/list-rules-tests/.yamllint
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/parseable.yml
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/quiet.yml
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/rulesdir-defaults.yml
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/rulesdir.yml
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/show-abspath.yml
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/show-relpath.yml
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/skip-tags.yml
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/strict.yml
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/tags.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/test_regenerate_formatting_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/unknown-type.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.070473 ansible-lint-6.9.0/test/fixtures/verbosity-tests/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/verbosity-tests/.yamllint
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/fixtures/verbosity.yml
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/foo.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.070473 ansible-lint-6.9.0/test/local-content/
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/test/local-content/collections/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/test/local-content/collections/ansible_collections/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/test/local-content/collections/ansible_collections/testns/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/collections/ansible_collections/testns/test_collection/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/collections/ansible_collections/testns/test_collection/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/test/local-content/collections/ansible_collections/testns/test_collection/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/collections/ansible_collections/testns/test_collection/plugins/filter/
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/collections/ansible_collections/testns/test_collection/plugins/filter/test_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/collections/ansible_collections/testns/test_collection/plugins/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/collections/ansible_collections/testns/test_collection/plugins/modules/test_module_2.py
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-collection.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-failed/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role1/library/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role1/library/test_module_1_failed.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role1/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role1/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role2/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role2/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role2/test_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role2/test_plugins/b_failed.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.006473 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role3/library/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role3/library/test_module_3_failed.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role3/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-failed/roles/role3/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-failed/test.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role1/library/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role1/library/test_module_1_failed_complete.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role1/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role1/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role2/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role2/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role2/test_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role2/test_plugins/b_failed_complete.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.002473 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role3/library/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role3/library/test_module_3_failed_complete.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role3/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-failed-complete/roles/role3/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.006473 ansible-lint-6.9.0/test/local-content/test-roles-success/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.006473 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.006473 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role1/library/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role1/library/test_module_1_success.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role1/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role1/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.006473 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role2/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role2/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role2/test_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role2/test_plugins/b_success.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.006473 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role3/library/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role3/library/test_module_3_success.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.074473 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role3/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/local-content/test-roles-success/roles/role3/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.078473 ansible-lint-6.9.0/test/rules/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.078473 ansible-lint-6.9.0/test/rules/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/fixtures/ematcher.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/fixtures/raw_task.md
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/fixtures/raw_task.py
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/fixtures/unset_variable_matcher.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_deprecated_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_inline_env_var.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_line_too_long.py
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_literal_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_meta_change_from_default.py
--rw-r--r--   0 runner    (1001) docker     (121)     2568 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_meta_no_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      972 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_meta_video_links.py
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_no_changed_when.py
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_no_jinja_when.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_no_relative_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     3197 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_octal_permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)      861 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_package_latest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_risky_shell_pipe.py
--rw-r--r--   0 runner    (1001) docker     (121)     2483 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_role_names.py
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_use_bare_variables.py
--rw-r--r--   0 runner    (1001) docker     (121)     1928 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/rules/test_use_handler_rather_than_when_changed.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_ansiblelintrule.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_ansiblesyntax.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_boot.py
--rw-r--r--   0 runner    (1001) docker     (121)     6456 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_cli_role_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     6899 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_commandline_invocations_same_as_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_dependencies_in_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_eco.py
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     3490 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_file_path_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (121)    14853 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_file_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2411 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_formatter_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_formatter_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     5486 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_formatter_sarif.py
--rw-r--r--   0 runner    (1001) docker     (121)     3775 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_import_include_role.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_import_playbook.py
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_import_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_include_miss_file_with_role.py
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_lint_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     2511 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_list_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_load_failure.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_local_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)     6586 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_matcherrror.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     2251 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_progressive.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_rule_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     6812 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_rules_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     5463 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_skip_import_playbook.py
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_skip_inside_yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_skip_playbook_items.py
--rw-r--r--   0 runner    (1001) docker     (121)     8399 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_skiputils.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_strict.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_task_includes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4677 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_transform_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     5566 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)    14673 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_verbosity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_with_skip_tagid.py
--rw-r--r--   0 runner    (1001) docker     (121)    28618 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/test/test_yaml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-24 01:13:31.078473 ansible-lint-6.9.0/tools/
--rwxr-xr-x   0 runner    (1001) docker     (121)      248 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/tools/get-version.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1183 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/tools/test-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      222 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/tools/update-version.sh
--rw-r--r--   0 runner    (1001) docker     (121)     6662 2022-11-24 01:13:09.000000 ansible-lint-6.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.816518 ansible-lint-6.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.ansible-lint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.664512 ansible-lint-6.9.1/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.config/ansible-lint.spec
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.darglint
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.664512 ansible-lint-6.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.664512 ansible-lint-6.9.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.664512 ansible-lint-6.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/workflows/redirects.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.packit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.668512 ansible-lint-6.9.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/DCO_1_1.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2022-12-03 21:00:15.816518 ansible-lint-6.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.668512 ansible-lint-6.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.668512 ansible-lint-6.9.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/_static/ansible-lint.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    13320 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/_static/images/ansible-lint-512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4280 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/_static/images/logo_invert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/configuring.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/custom-rules.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/installing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/docs/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/licenses/LICENSE.mit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/philosophy.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/docs/pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/pkg/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/redirects.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/docs/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/rules/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/rules.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/docs/using-profiles.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/examples/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/.config/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/ansible-navigator.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/examples/broken/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/broken/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/broken/ansible-navigator.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/broken/encoding.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/examples/broken/yaml-with-tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/broken/yaml-with-tabs/invalid-due-tabs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.632510 ansible-lint-6.9.1/examples/broken_collection_meta_runtime/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/examples/broken_collection_meta_runtime/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/broken_collection_meta_runtime/meta/runtime.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/examples/collection/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/collection/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/examples/ee_broken/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/ee_broken/execution-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/execution-environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/examples/group_vars/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/group_vars/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/examples/host_vars/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/host_vars/localhost.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.672512 ansible-lint-6.9.1/examples/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/inventory/broken_dev_inventory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/inventory/inventory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/inventory/production.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/lineno.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.676512 ansible-lint-6.9.1/examples/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/meta/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/meta/runtime.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.676512 ansible-lint-6.9.1/examples/other/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/other/some.j2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/other/some.yaml-too
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.692513 ansible-lint-6.9.1/examples/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/.ansible-lint-only-builtins-allow
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/always-run-success.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/become.transformed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/become.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/block.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/blockincludes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/blockincludes2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/bracketsmatchtest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/command-check-failure.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/command-check-success.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/common-include-1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/common-include-2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/conflicting_action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/contains_secrets.transformed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/contains_secrets.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/custom_module.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/ematcher-rule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/empty_playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/extra_vars.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.692513 ansible-lint-6.9.1/examples/playbooks/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/handlers/included-handlers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/handlers/y.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/include-import-tasks-in-role.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/include-in-block.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/include.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/jinja-spacing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/jinja2-when-failure.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/jinja2-when-success.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/json-schema-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    47347 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/lots_of_warnings.transformed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    47347 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/lots_of_warnings.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/mocked_dependency.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/multiline-brackets-do-not-match-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/multiline-bracketsmatchtest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/no-prompting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/nomatches.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/nomatchestest.transformed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/nomatchestest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/noqa-nested.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/noqa.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/norole.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/norole2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/package-check-failure.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/package-check-success.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/pass-loop-var-prefix.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/play.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/play_miss_include.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/playbook-imported.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/playbook-parent.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-avoid-implicit-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-avoid-implicit-pass.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-fqcn-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-fqcn-pass.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-jinja-invalid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-jinja-valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-key-order-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-name-casing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-name-missing-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-name-missing-pass.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-name-play-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-name-templated-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-no-free-form-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-no-free-form-pass.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-no-handler-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-no-handler-pass.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-no-tabs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-only-builtins.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-partial-become-without-become-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-partial-become-without-become-pass.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-risky-file-permissions-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-risky-file-permissions-pass.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-risky-octal-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-risky-octal-pass.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/rule-var-naming-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/run-once-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/run-once-pass.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/schema-error-string.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/skiptasks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/strict-mode.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/syntax-error-string.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/syntax-error.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/taskimports.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/taskincludes.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.696513 ansible-lint-6.9.1/examples/playbooks/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/tasks/conflicting-action-statements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.696513 ansible-lint-6.9.1/examples/playbooks/tasks/directory with spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/tasks/directory with spaces/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/tasks/empty_blocks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/tasks/include-in-block-inner.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/tasks/included-with-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/tasks/malformed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/tasks/nestedincludes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/tasks/passing_task.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/tasks/rule-name-prefix-fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/tasks/simple_task.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/tasks/varset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/tasks/varunset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/tasks/x.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.696513 ansible-lint-6.9.1/examples/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/templates/not-valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/test_import_with_conflicting_action_statements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/test_import_with_malformed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/test_include_inplace.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/test_include_relative.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/test_skip_inside_yaml.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/unicode.transformed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/unicode.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/using-bare-variables-failure.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/using-bare-variables-success.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/valid_with_alt_extension.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/playbooks/vars/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/vars/empty_vars.transformed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/vars/empty_vars.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/vars/invalid_vars_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/vars/jinja-spacing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/vars/not_decryptable.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/vars/other.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/vars/rule_jinja_vars.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/vars/strings.transformed.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/vars/strings.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/playbooks/vars/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/vars/subfolder/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/with-skip-tag-id.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/playbooks/with-umlaut-ä.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/reqs_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/reqs_v1/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/reqs_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/reqs_v2/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.632510 ansible-lint-6.9.1/examples/roles/ansible-role-foo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/roles/ansible-role-foo/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/ansible-role-foo/tasks/main.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.632510 ansible-lint-6.9.1/examples/roles/bobbins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/roles/bobbins/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/bobbins/tasks/imported_tasks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/bobbins/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.632510 ansible-lint-6.9.1/examples/roles/broken_argument_specs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/roles/broken_argument_specs/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/broken_argument_specs/meta/argument_specs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.632510 ansible-lint-6.9.1/examples/roles/dependency_in_meta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/roles/dependency_in_meta/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/dependency_in_meta/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/hello/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/roles/hello/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/hello/meta/argument_specs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/hello/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/include_in_the_place/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/roles/include_in_the_place/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/include_in_the_place/tasks/included_file.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/include_in_the_place/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/include_miss/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/roles/include_miss/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/include_miss/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/include_relative/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/roles/include_relative/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/include_relative/tasks/included_file.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/include_relative/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/invalid-name/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/roles/invalid-name/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/invalid-name/tasks/main.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/invalid_due_to_meta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/roles/invalid_due_to_meta/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/invalid_due_to_meta/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.700513 ansible-lint-6.9.1/examples/roles/invalid_due_to_meta/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/invalid_due_to_meta/tasks/main.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/invalid_meta_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/invalid_meta_schema/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/invalid_meta_schema/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/invalid_requirements_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/invalid_requirements_schema/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/invalid_requirements_schema/meta/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/invalud_meta_schema
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/loop_var_prefix/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/loop_var_prefix/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/loop_var_prefix/tasks/fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/loop_var_prefix/tasks/pass.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/meta_noqa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/meta_noqa/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/meta_noqa/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/more_complex/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/more_complex/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/more_complex/handlers/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/more_complex/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/more_complex/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/role_for_no_same_owner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/role_for_no_same_owner/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/role_for_no_same_owner/tasks/fail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/role_for_no_same_owner/tasks/pass.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/role_with_task_inclusions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/role_with_task_inclusions/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/role_with_task_inclusions/tasks/imported_tasks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/role_with_task_inclusions/tasks/included_tasks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/role_with_task_inclusions/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/subfolder/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/subfolder/other_role/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/subfolder/other_role/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/subfolder/other_role/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/template_lookup/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/template_lookup/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/template_lookup/files/a_file
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/template_lookup/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/template_lookup/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.636510 ansible-lint-6.9.1/examples/roles/template_lookup_missing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/template_lookup_missing/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/template_lookup_missing/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.640511 ansible-lint-6.9.1/examples/roles/test-role/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/test-role/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/test-role/meta/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.640511 ansible-lint-6.9.1/examples/roles/test-role/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/test-role/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/test-role/molecule/default/include-import-role.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/test-role/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/test-role/tasks/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/test-role/tasks/world.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.640511 ansible-lint-6.9.1/examples/roles/valid-due-to-meta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.704513 ansible-lint-6.9.1/examples/roles/valid-due-to-meta/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/valid-due-to-meta/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.708514 ansible-lint-6.9.1/examples/roles/valid-due-to-meta/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.708514 ansible-lint-6.9.1/examples/roles/valid-due-to-meta/tasks/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/valid-due-to-meta/tasks/debian/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/valid-due-to-meta/tasks/main.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.708514 ansible-lint-6.9.1/examples/roles/var_naming_pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/var_naming_pattern/.ansible-lint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.708514 ansible-lint-6.9.1/examples/roles/var_naming_pattern/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/roles/var_naming_pattern/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.708514 ansible-lint-6.9.1/examples/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/rules/task_has_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.640511 ansible-lint-6.9.1/examples/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.708514 ansible-lint-6.9.1/examples/templates/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/templates/playbooks/playbook.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.640511 ansible-lint-6.9.1/examples/testproject/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.640511 ansible-lint-6.9.1/examples/testproject/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.640511 ansible-lint-6.9.1/examples/testproject/roles/test-role/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.708514 ansible-lint-6.9.1/examples/testproject/roles/test-role/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/testproject/roles/test-role/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.708514 ansible-lint-6.9.1/examples/yamllint/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/yamllint/invalid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/yamllint/multi-document.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/examples/yamllint/valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/playbook.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.640511 ansible-lint-6.9.1/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.708514 ansible-lint-6.9.1/plugins/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/plugins/modules/fake_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2022-12-03 21:00:15.816518 ansible-lint-6.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.640511 ansible-lint-6.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.708514 ansible-lint-6.9.1/src/ansible_lint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2022-12-03 21:00:15.000000 ansible-lint-6.9.1/src/ansible_lint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31290 2022-12-03 21:00:15.000000 ansible-lint-6.9.1/src/ansible_lint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 21:00:15.000000 ansible-lint-6.9.1/src/ansible_lint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-03 21:00:15.000000 ansible-lint-6.9.1/src/ansible_lint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 21:00:14.000000 ansible-lint-6.9.1/src/ansible_lint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2022-12-03 21:00:15.000000 ansible-lint-6.9.1/src/ansible_lint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-03 21:00:15.000000 ansible-lint-6.9.1/src/ansible_lint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.716514 ansible-lint-6.9.1/src/ansiblelint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16009 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.716514 ansible-lint-6.9.1/src/ansiblelint/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/_internal/internal_error.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/_internal/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/_internal/warning.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/_mockings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-03 21:00:15.000000 ansible-lint-6.9.1/src/ansiblelint/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.716514 ansible-lint-6.9.1/src/ansiblelint/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/data/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16392 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.716514 ansible-lint-6.9.1/src/ansiblelint/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/generate_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.732515 ansible-lint-6.9.1/src/ansiblelint/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)    20000 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/avoid_implicit.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/avoid_implicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/command_instead_of_module.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/command_instead_of_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/command_instead_of_shell.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/command_instead_of_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.732515 ansible-lint-6.9.1/src/ansiblelint/rules/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_bare_vars.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_bare_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_command_syntax.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_command_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_local_action.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_local_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_module.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/empty_string_compare.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/empty_string_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/fqcn.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/fqcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/galaxy.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/ignore_errors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/ignore_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/inline_env_var.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/inline_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/jinja.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25951 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/key_order.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/key_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/latest.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/latest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/literal_compare.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/literal_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/loop_var_prefix.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/loop_var_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/meta_incorrect.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/meta_incorrect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/meta_no_info.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/meta_no_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/meta_no_tags.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/meta_no_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/meta_video_links.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/meta_video_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/name.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_changed_when.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_changed_when.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_free_form.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_free_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_handler.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_jinja_when.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_jinja_when.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_log_password.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_log_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_prompting.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_prompting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_relative_paths.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_relative_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_same_owner.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_same_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/no_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/only_builtins.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/only_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/package_latest.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/package_latest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/partial_become.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/partial_become.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/playbook_extension.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/playbook_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/risky_file_permissions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/risky_file_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/risky_octal.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/risky_octal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/risky_shell_pipe.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/risky_shell_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/role_name.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/role_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/run_once.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/run_once.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/schema.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/syntax_check.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/syntax_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/var_naming.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/var_naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/yaml.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/rules/yaml_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.736515 ansible-lint-6.9.1/src/ansiblelint/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/__store__.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/ansible-lint-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23497 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/ansible-navigator-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/ansible-navigator.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31263 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/ansible.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/arg_specs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/execution-environment.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12693 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/galaxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/inventory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/meta-runtime.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32108 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13840 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/molecule.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31728 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/playbook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/requirements.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14163 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/schemas/vars.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/skip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.736515 ansible-lint-6.9.1/src/ansiblelint/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32303 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44137 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/src/ansiblelint/yaml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.748515 ansible-lint-6.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/bar.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.748515 ansible-lint-6.9.1/test/custom_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/custom_rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.748515 ansible-lint-6.9.1/test/custom_rules/example_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/custom_rules/example_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/custom_rules/example_com/example_com_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.748515 ansible-lint-6.9.1/test/custom_rules/example_inc/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/custom_rules/example_inc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/custom_rules/example_inc/custom_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.752516 ansible-lint-6.9.1/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/ansible-config-invalid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/ansible-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/config-with-extra-vars.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/config-with-relative-path.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/config-with-write-all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/config-with-write-none.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/config-with-write-subset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/exclude-paths-with-expands.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/exclude-paths.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.752516 ansible-lint-6.9.1/test/fixtures/formatting-after/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/formatting-after/fmt-1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/formatting-after/fmt-2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/formatting-after/fmt-3.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.752516 ansible-lint-6.9.1/test/fixtures/formatting-before/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/formatting-before/fmt-1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/formatting-before/fmt-2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/formatting-before/fmt-3.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/fixtures/formatting-prettier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/formatting-prettier/fmt-1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/formatting-prettier/fmt-2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/formatting-prettier/fmt-3.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/fixtures/list-rules-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/list-rules-tests/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/parseable.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/quiet.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/rulesdir-defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/rulesdir.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/show-abspath.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/show-relpath.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/skip-tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/strict.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/test_regenerate_formatting_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/unknown-type.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/fixtures/verbosity-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/verbosity-tests/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/fixtures/verbosity.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/foo.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.644511 ansible-lint-6.9.1/test/local-content/collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.644511 ansible-lint-6.9.1/test/local-content/collections/ansible_collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.644511 ansible-lint-6.9.1/test/local-content/collections/ansible_collections/testns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/collections/ansible_collections/testns/test_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/collections/ansible_collections/testns/test_collection/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.644511 ansible-lint-6.9.1/test/local-content/collections/ansible_collections/testns/test_collection/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/collections/ansible_collections/testns/test_collection/plugins/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/collections/ansible_collections/testns/test_collection/plugins/filter/test_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/collections/ansible_collections/testns/test_collection/plugins/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/collections/ansible_collections/testns/test_collection/plugins/modules/test_module_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-collection.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/test-roles-failed/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.648511 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.644511 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role1/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role1/library/test_module_1_failed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role1/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role1/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.648511 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role2/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role2/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role2/test_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role2/test_plugins/b_failed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.648511 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.760516 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role3/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role3/library/test_module_3_failed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.760516 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role3/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-failed/roles/role3/tasks/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-failed/test.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.644511 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.644511 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.644511 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role1/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role1/library/test_module_1_failed_complete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role1/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role1/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.644511 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role2/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role2/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role2/test_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role2/test_plugins/b_failed_complete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.644511 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role3/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role3/library/test_module_3_failed_complete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.756516 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role3/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-failed-complete/roles/role3/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.648511 ansible-lint-6.9.1/test/local-content/test-roles-success/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.648511 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.648511 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.760516 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role1/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role1/library/test_module_1_success.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.760516 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role1/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role1/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.648511 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.760516 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role2/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role2/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.760516 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role2/test_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role2/test_plugins/b_success.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.648511 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.760516 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role3/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role3/library/test_module_3_success.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.760516 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role3/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/local-content/test-roles-success/roles/role3/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.768516 ansible-lint-6.9.1/test/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.768516 ansible-lint-6.9.1/test/rules/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/fixtures/ematcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/fixtures/raw_task.md
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/fixtures/raw_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/fixtures/unset_variable_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_deprecated_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_inline_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_line_too_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_literal_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_meta_change_from_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_meta_no_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_meta_video_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_no_changed_when.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_no_jinja_when.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_no_relative_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_package_latest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_risky_shell_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_role_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_use_bare_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/rules/test_use_handler_rather_than_when_changed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.772517 ansible-lint-6.9.1/test/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/.mocharc.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.772517 ansible-lint-6.9.1/test/schemas/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   204531 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/data/licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.648511 ansible-lint-6.9.1/test/schemas/negative_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.772517 ansible-lint-6.9.1/test/schemas/negative_test/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/inventory/broken_dev_inventory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/inventory/broken_dev_inventory.yml.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.648511 ansible-lint-6.9.1/test/schemas/negative_test/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.772517 ansible-lint-6.9.1/test/schemas/negative_test/molecule/platforms_children/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/molecule/platforms_children/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/molecule/platforms_children/molecule.yml.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.772517 ansible-lint-6.9.1/test/schemas/negative_test/molecule/platforms_networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/molecule/platforms_networks/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/molecule/platforms_networks/molecule.yml.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.784517 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/environment.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/failed_when.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/failed_when.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/gather_facts.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/gather_facts.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/gather_subset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/gather_subset.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/gather_subset2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/gather_subset2.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/gather_subset3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/gather_subset3.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/gather_subset4.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/gather_subset4.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/ignore_errors.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/ignore_errors.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/import_playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/import_playbook.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/import_playbook_exclusive.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/import_playbook_exclusive.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/invalid-failed-when.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/invalid-failed-when.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/invalid-serial.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/invalid-serial.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/invalid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/invalid.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/invalid_become.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/invalid_become.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/local_action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/local_action.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/loop.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/loop.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/loop2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/loop2.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/no_log_partial_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/no_log_partial_template.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/no_log_string.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/no_log_string.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/roles.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/roles.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/run_once_list.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/run_once_list.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tags-mapping.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tags-mapping.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tags-number.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tags-number.yml.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.792517 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/args_integer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/args_integer.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/args_string.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/args_string.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/become_method_untemplated.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/become_method_untemplated.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/ignore_errors.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/ignore_errors.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/invalid_block.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/invalid_block.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/local_action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/local_action.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/loop.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/loop.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/loop2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/loop2.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/no_log_number.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/no_log_number.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/no_log_string.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/no_log_string.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/tags-mapping.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/tags-mapping.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/tags-string.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/tags-string.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/when_integer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/when_integer.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/when_object.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/when_object.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/with_items_boolean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/with_items_boolean.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/with_items_untemplated_string.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks/with_items_untemplated_string.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/tasks.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/var_files_list_number.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/var_files_list_number.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/var_files_number.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/var_files_number.yml.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.796517 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/asterisk.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/asterisk.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/dash-in-var-name.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/dash-in-var-name.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/list.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/list.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/numeric-var-name.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/numeric-var-name.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/play-keyword.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/play-keyword.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/python-keyword.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/python-keyword.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/varname-numeric-prefix.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vars/varname-numeric-prefix.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vas_prompt.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/vas_prompt.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/with_cartesian.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/with_cartesian.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/with_filetree.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/with_filetree.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/with_flattened.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/playbooks/with_flattened.yml.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.648511 ansible-lint-6.9.1/test/schemas/negative_test/reqs3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.796517 ansible-lint-6.9.1/test/schemas/negative_test/reqs3/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/reqs3/meta/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/reqs3/meta/requirements.yml.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.652511 ansible-lint-6.9.1/test/schemas/negative_test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.796517 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta/argument_specs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta/argument_specs.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta/main.yml.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.652511 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta_invalid_collection/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.796517 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta_invalid_collection/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta_invalid_collection/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta_invalid_collection/meta/main.yml.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.652511 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta_invalid_collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.800518 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta_invalid_collections/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta_invalid_collections/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta_invalid_collections/meta/main.yml.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.652511 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta_invalid_role_namespace/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.800518 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta_invalid_role_namespace/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta_invalid_role_namespace/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/roles/meta_invalid_role_namespace/meta/main.yml.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.652511 ansible-lint-6.9.1/test/schemas/negative_test/roles/role_with_bad_deps_in_meta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.800518 ansible-lint-6.9.1/test/schemas/negative_test/roles/role_with_bad_deps_in_meta/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/roles/role_with_bad_deps_in_meta/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/negative_test/roles/role_with_bad_deps_in_meta/meta/main.yml.md
+-rw-r--r--   0 runner    (1001) docker     (123)    94991 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.800518 ansible-lint-6.9.1/test/schemas/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/src/rebuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/src/schema.spec.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.800518 ansible-lint-6.9.1/test/schemas/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/ansible-navigator.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/execution-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.800518 ansible-lint-6.9.1/test/schemas/test/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/inventory/inventory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/inventory/production.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/inventory.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.800518 ansible-lint-6.9.1/test/schemas/test/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/meta/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.652511 ansible-lint-6.9.1/test/schemas/test/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.800518 ansible-lint-6.9.1/test/schemas/test/molecule/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/molecule/cluster/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.804518 ansible-lint-6.9.1/test/schemas/test/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.804518 ansible-lint-6.9.1/test/schemas/test/molecule/vagrant/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/molecule/vagrant/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.808518 ansible-lint-6.9.1/test/schemas/test/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/block.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.808518 ansible-lint-6.9.1/test/schemas/test/playbooks/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/defaults/foo.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/failed_when.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/full-jinja.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/gather_facts.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/gather_subset.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/ignore_errors..yml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/import_playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/included.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/integers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/local_action_dict.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/local_action_string.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/loop.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/no_log.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/roles.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/run_once.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tags.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.812518 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/args.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/become_method.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/changed_when.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/diff.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/empty_tasks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/ignore_errors.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/local_action_dict.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/local_action_string.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/loop.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/no_log.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/notify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/run_once.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/some_tasks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/templated_become.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/templated_integers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/throttled.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/until.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/when.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks/with_items.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/tasks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/templated_become.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/user_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/var_files.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.812518 ansible-lint-6.9.1/test/schemas/test/playbooks/vars/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/vars/empty_vars.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/vars/encrypted.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/vars/myvars.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/vars_prompt.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/playbooks/with_.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.652511 ansible-lint-6.9.1/test/schemas/test/reqs2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.812518 ansible-lint-6.9.1/test/schemas/test/reqs2/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/reqs2/meta/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.652511 ansible-lint-6.9.1/test/schemas/test/reqs4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.812518 ansible-lint-6.9.1/test/schemas/test/reqs4/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/reqs4/meta/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.652511 ansible-lint-6.9.1/test/schemas/test/reqs5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.812518 ansible-lint-6.9.1/test/schemas/test/reqs5/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/reqs5/meta/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.656511 ansible-lint-6.9.1/test/schemas/test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.652511 ansible-lint-6.9.1/test/schemas/test/roles/empty-meta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.812518 ansible-lint-6.9.1/test/schemas/test/roles/empty-meta/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/roles/empty-meta/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.652511 ansible-lint-6.9.1/test/schemas/test/roles/foo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.812518 ansible-lint-6.9.1/test/schemas/test/roles/foo/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/roles/foo/meta/argument_specs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/roles/foo/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/roles/foo/meta/runtime.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.652511 ansible-lint-6.9.1/test/schemas/test/roles/maximum/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.812518 ansible-lint-6.9.1/test/schemas/test/roles/maximum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/roles/maximum/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.656511 ansible-lint-6.9.1/test/schemas/test/roles/meta-tags/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.812518 ansible-lint-6.9.1/test/schemas/test/roles/meta-tags/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/roles/meta-tags/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.656511 ansible-lint-6.9.1/test/schemas/test/roles/ns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.816518 ansible-lint-6.9.1/test/schemas/test/roles/ns/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/roles/ns/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.656511 ansible-lint-6.9.1/test/schemas/test/roles/v1_role/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.816518 ansible-lint-6.9.1/test/schemas/test/roles/v1_role/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/roles/v1_role/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.656511 ansible-lint-6.9.1/test/schemas/test/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.656511 ansible-lint-6.9.1/test/schemas/test/tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.656511 ansible-lint-6.9.1/test/schemas/test/tests/integration/rom_role/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.816518 ansible-lint-6.9.1/test/schemas/test/tests/integration/rom_role/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/test/tests/integration/rom_role/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/schemas/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_ansiblelintrule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_ansiblesyntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_boot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_cli_role_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_commandline_invocations_same_as_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_dependencies_in_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_eco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_file_path_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14853 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_formatter_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_formatter_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_formatter_sarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_import_include_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_import_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_import_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_include_miss_file_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_internal_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_lint_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_list_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_load_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_local_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_matcherrror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_progressive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_rule_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_rules_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_skip_import_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_skip_inside_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_skip_playbook_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_skiputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_strict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_task_includes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_transform_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14673 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_verbosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_with_skip_tagid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29443 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/test/test_yaml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 21:00:15.816518 ansible-lint-6.9.1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      248 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/tools/get-version.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1012 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/tools/test-setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      222 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/tools/update-version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2022-12-03 20:59:56.000000 ansible-lint-6.9.1/tox.ini
```

### Comparing `ansible-lint-6.9.0/.ansible-lint` & `ansible-lint-6.9.1/.ansible-lint`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # and not relative to the CWD of execution. CLI arguments passed to the --exclude
 # option are parsed relative to the CWD of execution.
 exclude_paths:
   - .cache/ # implicit unless exclude_paths is defined in config
   - .github/
   - test/fixtures/formatting-before/
   - test/fixtures/formatting-prettier/
+  - test/schemas/
 # parseable: true
 # quiet: true
 # strict: true
 # verbosity: 1
 
 # Mock modules or roles in order to pass ansible-playbook --syntax-check
 mock_modules:
@@ -29,15 +30,15 @@
 
 # Enable checking of loop variable prefixes in roles
 loop_var_prefix: "{role}_"
 
 # Enforce variable names to follow pattern below, in addition to Ansible own
 # requirements, like avoiding python identifiers. To disable add `var-naming`
 # to skip_list.
-# var_naming_pattern: "^[a-z_][a-z0-9_]*$"
+var_naming_pattern: "^[a-z_][a-z0-9_]*$"
 
 use_default_rules: true
 # Load custom rules from this specific folder
 # rulesdir:
 #   - ./rule/directory/
 
 # Ansible-lint completely ignores rules or tags listed below
@@ -46,14 +47,15 @@
 
 # Ansible-lint does not automatically load rules that have the 'opt-in' tag.
 # You must enable opt-in rules by listing each rule 'id' below.
 enable_list:
   - empty-string-compare # opt-in
   - no-log-password # opt-in
   - no-same-owner # opt-in
+  - name[prefix] # opt-in
   # add yaml here if you want to avoid ignoring yaml checks when yamllint
   # library is missing. Normally its absence just skips using that rule.
   - yaml
 # Report only a subset of tags and fully ignore any others
 # tags:
 #   - jinja[spacing]
 
@@ -97,7 +99,18 @@
 kinds:
   # - playbook: "**/examples/*.{yml,yaml}"
   # - galaxy: "**/folder/galaxy.yml"
   # - tasks: "**/tasks/*.yml"
   # - vars: "**/vars/*.yml"
   # - meta: "**/meta/main.yml"
   - yaml: "**/*.yaml-too"
+
+# List of additional collections to allow in only-builtins rule.
+# only_builtins_allow_collections:
+#   - example_ns.example_collection
+
+# List of additions modules to allow in only-builtins rule.
+# only_builtins_allow_modules:
+#   - example_module
+
+# Allow setting custom prefix for name[prefix] rule
+task_name_prefix: "{stem} | "
```

### Comparing `ansible-lint-6.9.0/.config/ansible-lint.spec` & `ansible-lint-6.9.1/.config/ansible-lint.spec`

 * *Files 26% similar despite different names*

```diff
@@ -7,81 +7,66 @@
 %bcond_with     privileged_tests
 
 Name:           ansible-lint
 Version:        VERSION_PLACEHOLDER
 Release:        1%{?dist}
 Summary:        Ansible-lint checks ansible content for common mistakes
 
-License:        MIT
+License:        GPL-3.0-or-later AND MIT
 URL:            https://github.com/ansible/ansible-lint
 Source0:        %{pypi_source}
 
 BuildArch:      noarch
 
-BuildRequires:  pyproject-rpm-macros
-BuildRequires:  python%{python3_pkgversion}-build
 BuildRequires:  python%{python3_pkgversion}-devel
-BuildRequires:  python%{python3_pkgversion}-pip
-BuildRequires:  python%{python3_pkgversion}-setuptools
-BuildRequires:  python%{python3_pkgversion}-setuptools_scm
-BuildRequires:  python%{python3_pkgversion}-wheel
 %if %{with check}
 # These are required for tests:
-BuildRequires:  python%{python3_pkgversion}-pyyaml
 BuildRequires:  python%{python3_pkgversion}-pytest
 BuildRequires:  python%{python3_pkgversion}-pytest-xdist
 BuildRequires:  python%{python3_pkgversion}-libselinux
-BuildRequires:  git
+BuildRequires:  git-core
 %endif
-# Named based on fedora 35:
-Requires:       ansible-core >= 2.12.0
-Requires:       python3-packaging
-Requires:       python3-pyyaml
-Requires:       python3-rich
-Requires:       python3-ruamel-yaml
-Requires:       python3-ruamel-yaml-clib
-Requires:       python3-wcmatch
-Requires:       yamllint
 
-# generate_buildrequires
-# pyproject_buildrequires
 
 %description
 Ansible-lint checks ansible content for practices and behaviors that could
 potentially be improved.
 
 %prep
 %autosetup
 
 
+%generate_buildrequires
+%pyproject_buildrequires
+
+
 %build
 %pyproject_wheel
 
 
 %install
 %pyproject_install
+%pyproject_save_files ansiblelint
 
 
-%if %{with check}
 %check
-PYTHONPATH=%{buildroot}%{python3_sitelib} \
-  pytest-3 \
+# Don't try to import tests that import pytest which isn't available at runtime
+%pyproject_check_import -e 'ansiblelint.testing*' -e 'ansiblelint.rules.conftest'
+%if %{with check}
+%pytest \
   -v \
   --disable-pytest-warnings \
   --numprocesses=auto \
 %if %{with privileged_tests}
   tests
 %else
   tests/unit
 %endif
 %endif
 
 
-%files
-%{python3_sitelib}/ansiblelint/
-%{python3_sitelib}/ansible_lint-*.dist-info/
+%files -f %{pyproject_files}
 %{_bindir}/ansible-lint
-%license COPYING
-%doc docs/* README.md
+%license COPYING docs/licenses/LICENSE.mit.txt
+%doc docs/ README.md
 
 %changelog
-Available at https://github.com/ansible/ansible-lint/releases
```

### Comparing `ansible-lint-6.9.0/.config/dictionary.txt` & `ansible-lint-6.9.1/.config/dictionary.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,95 @@
+Adrián
 Autobuild
 CLICOLOR
 CODENOTIFY
 CODEOWNERS
 CTYPE
+Cacqueray
+Chamoulaud
+DISTRO
 DOTGLOB
 ENVVAR
 EPIPE # linux
+Fimport
 Jython
 MYTAG
+PYTHONBREAKPOINT
 PYTHONIOENCODING
-Representer
+PYTHONPYCACHEPREFIX
 REQPASS
 RULEDIRS
 RUNLEVEL
+Representer
 SRCROOT
+Sbarnea
+Sorin
 Sshell
 TOXENV
 TYPECHECK
+Tsukinowa
+Tóth
 WSLENV
 aarch64
 abspath
 addoption
 addopts
 ansiblelint
 apidoc
 apport
 argparsing
 argspecs
+arxcruz
 auditd
 autobuild
 autoclass
 autodetected
 autodiscovery
 autodoc
 autofix
 autoupdate
+awcrosby
 backports
 backticks
 bdist
 becomeuserabove
 bindep
 blockincludes
 blockinfile
 bools
 boto
 bracketsmatchtest
 bracketsmatchtestfile
 buildinfo
 buildset
 builtins
+cachier
 capfd
 caplog
 capsys
 cffi
 chdir
 chgrp
 chkconfig
 chunksize
 codeclimate
 codecov
-codeql
 codenotify
+codeql
 codespell
 colorama
 colsystem
 commandline
 commitlint
 commonmark
 compat
 conftest
 coveragerc
+cpus
+cpuset
 createfile
 darglint
 dataclasses
 dbservers
 deannotate
 debops
 decryptable
@@ -82,71 +98,89 @@
 denormalize
 deps
 devel
 dharmabumstead
 dirhtml
 dists
 distutils
+doas
 docstrings
 doctest
 doctrees
 docutils
 dotconfig
 dotslash
+drybjed
+dzdo
 ematcher
 ematchtestfile
+envrc
 execnet
 extlinks
+facter
 fakerole
 fileglob
 filelock
 filesspot
 filetree
+fips
+firewalld
 formatstr
 formetting
 formsyntax
 fqcn
 fqrn
 fulltoc
 fullwidth
+gecos
+geerlingguy
 getmatches
 globbing
 globmatch
+groupname
 hostkey
 hostnames
 hostvars
 htmldir
 htpasswd
 hwchksum
 hwcksum
 idempotency
 importlib
 iniconfig
 insertafter
 intersphinx
 ipwrap
 isclass
+iscsi
 isdir
 isdisjoint
 iskeyword
 isort
+jsonfile
 jsonschema
 junitxml
 keepends
+konstruktoid
 kubernetes
+kubevirt
+languageservice
 letsencrypt
 levelname
+libbzip
 libera
 libyaml
 lineinfile
 linkcheck
 lintable
 lintables
 literalinclude
 localectl
+machinectl
+markdownlint
 matchdir
 matcherror
 matchlines
 matchtask
 matchtasks
 matchvar
 matchyaml
@@ -161,42 +195,45 @@
 modindex
 moduleauthor
 mypy
 myrole
 namedtempfile
 nestedincludes
 netcommon
+nilashishc
 nitpicky
 nocolor
 nodeps
 noexist
 nomatches
 nomatchestest
 noqa
 norole
 nostderr
 notest
+nxos
 opensearch
 openshift
 outdir
 outlen
 pageview
 parseable
 pathex
 pathlib
 pathspec
+pbrun
+pfexec
 pickleable
 pipdeptree
 pipefail
 piptools
 pipx
 pkgcache  # linux
 pkgs
 placefolder
-playholder
 pluggy
 pluginmanager
 podman
 prerun
 prettierignore
 programoutput
 psutil
@@ -221,25 +258,29 @@
 releasenotes
 relpath
 reportversion
 representer
 reqs
 returncode
 rmtree
+robertdebock
 rolepath
 roundtrip
 ruamel
 ruledirs
 rulesdir
 rulesdirs
+runas
 sarif
 scalarint
+schemafile
 sdist
 sdists
 sectionauthor
+seealso
 setenv
 setuptools
 shortdesc
 showlocals
 shutil
 signoff
 simpletask
@@ -247,44 +288,50 @@
 skiptasks
 skiputils
 slaveinput
 sortfunc
 sourcegraph
 sphinxcontrib
 srpm
+ssbarnea
 stylesheet
 subdir
 subelements
 subresults
+subschema
+subschemas
 substrs
 subtest
 supervisorctl
 synchronize
 sysvinit
 taskhandler
 taskimports
 taskincludes
 taskshandlers
 templatevars
 templating
+testinfra
 testmon
 testns
 testpath
 testpaths
 testproject
 testpypi
 testrun
 timesyncd
+tmpfs
 toctree
 toidentifier
 tomli
 toolset
 tripleo
 typehint
 typehints
+ulimits
 uncook
 ungrouped
 unignored
 unimported
 unindented
 uninstallation
 unjinja
@@ -293,46 +340,29 @@
 unskippable
 unspaced
 unsubscriptable
 untemplated
 userbase
 uwsgi
 validable
+varname
 varnotset
 varset
 varsfile
 varstring
 varunset
 venv
 viewcode
 virtnet
 virtualenv
 virtualenvs
 wcmatch
 webserver
 webservers
+willthames
 workdir
 worktree
 xdist
 xfail
 xunit
-zuul
-
-# names and usernames
-Adrián
-Cacqueray
-Chamoulaud
-Sbarnea
-Sorin
-Tsukinowa
-Tóth
-arxcruz
-awcrosby
-drybjed
-geerlingguy
-konstruktoid
-nilashishc
-nxos
-robertdebock
-ssbarnea
-willthames
 yatesr
+zuul
```

### Comparing `ansible-lint-6.9.0/.flake8` & `ansible-lint-6.9.1/.flake8`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,27 @@
 
 # The only allowed ignores are related to black and isort
 # https://black.readthedocs.io/en/stable/the_black_code_style.html#line-length
 # "H" are generated by hacking plugin, which is not black compatible
 extend-ignore =
   E203,
   E501,
-  C901, # complexity is also measured by pylint: too-many-branches
-  DAR104,  # We use type annotations instead
-  DAR301,  # https://github.com/terrencepreilly/darglint/issues/165
-  F401,  # duplicate of pylint W0611 (unused-import)
-  F821,  # duplicate of pylint E0602 (undefined-variable)
-  F841,  # duplicate of pylint W0612 (unused-variable)
+  # complexity is also measured by pylint: too-many-branches
+  C901,
+  # We use type annotations instead
+  DAR101,
+  DAR104,
+  # https://github.com/terrencepreilly/darglint/issues/165
+  DAR301,
+  # duplicate of pylint W0611 (unused-import)
+  F401,
+  # duplicate of pylint E0602 (undefined-variable)
+  F821,
+  # duplicate of pylint W0612 (unused-variable)
+  F841,
   H,
 
 # Allow certain violations in certain files:
 per-file-ignores =
   # FIXME: D102 Missing docstring in public method
   src/ansiblelint/cli.py: D102
   src/ansiblelint/formatters/__init__.py: D102
```

### Comparing `ansible-lint-6.9.0/.github/CONTRIBUTING.md` & `ansible-lint-6.9.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ansible-lint-6.9.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 ---
 name: Bug report
 about: >
-  Create a bug report. Please test against the main branch before
-  submitting it. For anything else, please use discussions
-  link below.
+  Create a bug report. Ensure that it does reproduce on the main branch with
+  python >=3.9.  For anything else, please use the discussion link below.
 labels: bug, new
 ---
 
 <!--- Verify first that your issue is not already reported on GitHub -->
 <!--- Also test if the latest release and main branch are affected too -->
 
 ##### Summary
 
 <!--- Explain the problem briefly below -->
 
 ##### Issue Type
 
 - Bug Report
 
-##### Ansible and Ansible Lint details
+##### OS / ENVIRONMENT
 
 <!--- Paste verbatim output between triple backticks -->
 
 ```console (paste below)
-ansible --version
-
 ansible-lint --version
-
 ```
 
+<!--- Provide all relevant information below, e.g. target OS versions, network
+ device firmware, etc. -->
+
 - ansible installation method: one of source, pip, OS package
 - ansible-lint installation method: one of source, pip, OS package
 
-##### OS / ENVIRONMENT
-
-<!--- Provide all relevant information below, e.g. target OS versions, network device firmware, etc. -->
-
 ##### STEPS TO REPRODUCE
 
-<!--- Describe exactly how to reproduce the problem, using a minimal test-case -->
+<!--- Describe exactly how to reproduce the problem, using a minimal test case -->
 
 <!--- Paste example playbooks or commands between triple backticks below -->
 
 ```console (paste below)
 
 ```
 
@@ -52,22 +47,22 @@
 
 <!--- Describe what you expected to happen when running the steps above -->
 
 Possible security bugs should be reported via email to `security@ansible.com`
 
 ##### Actual Behavior
 
-<!--- Describe what actually happened. If possible run with extra verbosity (-vvvv) -->
+<!--- Describe what happened. If possible run with extra verbosity (-vvvv) -->
 
-Please give some details of what is actually happening.
+Please give some details of what is happening.
 Include a [minimum complete verifiable example] with:
 
-- playbook
-- output of running ansible-lint
-- if you're getting a stack trace, output of
+- minimized playbook to reproduce the error
+- the output of running ansible-lint including the command line used
+- if you're getting a stack trace, also the output of
   `ansible-playbook --syntax-check playbook`
 
 <!--- Paste verbatim command output between triple backticks -->
 
 ```paste below
 
 ```
```

### Comparing `ansible-lint-6.9.0/.github/ISSUE_TEMPLATE/config.yml` & `ansible-lint-6.9.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/.github/ISSUE_TEMPLATE.md` & `ansible-lint-6.9.1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/.github/SECURITY.md` & `ansible-lint-6.9.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/.github/dependabot.yml` & `ansible-lint-6.9.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/.github/workflows/redirects.yml` & `ansible-lint-6.9.1/.github/workflows/redirects.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/.github/workflows/tox.yml` & `ansible-lint-6.9.1/.github/workflows/tox.yml`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,16 @@
   create: # is used for publishing to PyPI and TestPyPI
     tags: # any tag regardless of its name, no branches
       - "**"
   push: # only publishes pushes to the main branch to TestPyPI
     branches: # any integration branch but not tag
       - "main"
   pull_request:
+    branches:
+      - "main"
   release:
     types:
       - published # It seems that you can publish directly without creating
   schedule:
     - cron: 1 0 * * * # Run daily at 0:01 UTC
   # Run every Friday at 18:02 UTC
   # https://crontab.guru/#2_18_*_*_5
@@ -21,153 +23,68 @@
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.sha }}
   cancel-in-progress: true
 
 env:
   FORCE_COLOR: 1 # tox, pytest, ansible-lint
   PY_COLORS: 1
-  TOX_PARALLEL_NO_SPINNER: 1
 
 jobs:
-  linters:
-    name: >-
-      ${{ matrix.env.TOXENV }}
-    runs-on: ${{ matrix.os }}
-    strategy:
-      fail-fast: false
-      matrix:
-        python-version:
-          - 3.9
-        os:
-          - ubuntu-20.04
-        env:
-          - TOXENV: lint
-          - TOXENV: docs
-          - TOXENV: eco
-          - TOXENV: packaging
-          - TOXENV: validate-hook
-
-    steps:
-      - name: Check out src from Git
-        uses: actions/checkout@v3
-        with:
-          fetch-depth: 0 # needed by setuptools-scm
-      - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python-version }}
-          cache: "pip"
-      # - name: set PY_SHA256
-      #   run: echo "::set-env name=PY_SHA256::$(python -VV | sha256sum | cut -d' ' -f1)"
-      # - name: Pre-commit cache
-      #   uses: actions/cache@v1
-      #   with:
-      #     path: ~/.cache/pre-commit
-      #     key: ${{ runner.os }}-pre-commit-${{ env.PY_SHA256 }}-${{ hashFiles('setup.cfg') }}-${{ hashFiles('tox.ini') }}-${{ hashFiles('pyproject.toml') }}-${{ hashFiles('.pre-commit-config.yaml') }}-${{ hashFiles('pytest.ini') }}
-      # - name: Pip cache
-      #   uses: actions/cache@v1
-      #   with:
-      #     path: ~/.cache/pip
-      #     key: ${{ runner.os }}-pip-${{ env.PY_SHA256 }}-${{ hashFiles('setup.cfg') }}-${{ hashFiles('tox.ini') }}-${{ hashFiles('pyproject.toml') }}-${{ hashFiles('.pre-commit-config.yaml') }}-${{ hashFiles('pytest.ini') }}
-      #     restore-keys: |
-      #       ${{ runner.os }}-pip-
-      #       ${{ runner.os }}-
-      - name: Install tox
-        run: |
-          python3 -m pip install --upgrade pip
-          python3 -m pip install --upgrade tox
-      - name: Log installed dists
-        run: >-
-          python -m pip freeze --all
-      - name: Initialize tox envs
-        run: >-
-          python -m
-          tox
-          --parallel auto
-          --parallel-live
-          --notest
-          --skip-missing-interpreters false
-          -vv
-        env: ${{ matrix.env }}
-      - name: Test with tox
-        run: |
-          python -m tox --parallel auto --parallel-live
-        env: ${{ matrix.env }}
-      - name: Archive logs
-        uses: actions/upload-artifact@v3
-        with:
-          name: logs.zip
-          path: .tox/**/log/
-
-  unit:
+  build:
     name: ${{ matrix.name || matrix.tox_env }}
-    runs-on: ${{ matrix.os }}
+    runs-on: ${{ matrix.os || 'ubuntu-22.04' }}
     defaults:
       run:
         shell: ${{ matrix.shell || 'bash'}}
     strategy:
       fail-fast: false
       # max-parallel: 5
       # The matrix testing goal is to cover the *most likely* environments
       # which are expected to be used by users in production. Avoid adding a
       # combination unless there are good reasons to test it, like having
       # proof that we failed to catch a bug by not running it. Using
       # distribution should be preferred instead of custom builds.
       matrix:
-        name:
-          - py38
-        tox_env:
-          - py38
-        python-version:
-          - 3.8
-        os:
-          # https://help.github.com/en/actions/reference/virtual-environments-for-github-hosted-runners
-          - ubuntu-20.04
-        # - windows-latest
-        # - windows-2016
+        # https://help.github.com/en/actions/reference/virtual-environments-for-github-hosted-runners
         include:
           # keep list sorted as it determines UI order too
           # linux
-          # py38 is first and comes from matrix
-          - tox_env: py38 # no devel for 3.8 as core dropped support for it
-            os: ubuntu-20.04
-            python-version: 3.8
+          - tox_env: lint
+          - tox_env: pkg,hook,docs
+          - tox_env: schemas
+          - tox_env: eco # slow, keep separated
           - tox_env: py39,py39-devel
-            os: ubuntu-20.04
             python-version: 3.9
           - tox_env: py310
-            os: ubuntu-20.04
             python-version: "3.10"
           - tox_env: py311,py311-devel
-            os: ubuntu-20.04
             python-version: "3.11"
           # macos
-          - name: py38 (macos)
-            tox_env: py38
+          - name: py39 (macos)
+            tox_env: py39,py39-devel
             os: macOS-latest
-            python-version: 3.8
-            devel: false # ansible 2.14 removed support for py38
+            python-version: 3.9
           - name: py311 (macos)
             tox_env: py311,py311-devel
             os: macOS-latest
             python-version: "3.11"
           # windows-2022 WSL does timeout running tests, likely caused but some
           # extreme (>10x) performance degradation compared with windows-2019
           # https://github.com/actions/virtual-environments/issues/4856
           - name: py39 (wsl)
             tox_env: py39
             os: windows-2019
             shell: "wsl-bash {0}"
 
     env:
       # vars safe to be passed to wsl:
-      WSLENV: FORCE_COLOR:PYTEST_REQPASS:TOXENV:TOX_PARALLEL_NO_SPINNER
+      WSLENV: FORCE_COLOR:PYTEST_REQPASS:TOXENV
       # Number of expected test passes, safety measure for accidental skip of
       # tests. Update value if you add/remove tests.
-      PYTEST_REQPASS: 717
+      PYTEST_REQPASS: 725
 
     steps:
       - name: Activate WSL1
         if: "contains(matrix.shell, 'wsl')"
         uses: Vampire/setup-wsl@v1
 
       - name: MacOS workaround for https://github.com/actions/virtual-environments/issues/1187
@@ -176,55 +93,63 @@
           sudo sysctl -w net.link.generic.system.hwcksum_tx=0
           sudo sysctl -w net.link.generic.system.hwcksum_rx=0
 
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0 # needed by setuptools-scm
 
-      - name: Set cache for galaxy
+      - name: Set caches
         uses: actions/cache@v3
         with:
           path: |
             ~/.ansible/galaxy_cache
             ~/.ansible/collections/ansible_collections
             ~/.ansible/roles/
-          key: galaxy-${{ matrix.name }}-${{ hashFiles('requirements.yml') }}
+            ~/.cache/pre-commit
+          key: galaxy-${{ matrix.name }}-${{ hashFiles('requirements.yml', '.pre-commit-config.yaml', 'pyproject.toml') }}
 
-      - name: Set up Python ${{ matrix.python-version }}
+      - name: Set up Python ${{ matrix.python-version || '3.9' }}
         if: "!contains(matrix.shell, 'wsl')"
         uses: actions/setup-python@v4
         with:
           cache: pip
-          python-version: ${{ matrix.python-version }}
+          python-version: ${{ matrix.python-version || '3.9' }}
+
+      - uses: actions/setup-node@v3
+        with:
+          node-version: 18
+          cache: "npm"
+          cache-dependency-path: test/schemas/package-lock.json
 
       - name: Run ./tools/test-setup.sh
         run: ./tools/test-setup.sh
 
       - name: Install tox
         run: |
           python3 -m pip install --upgrade pip
-          python3 -m pip install --upgrade tox tox-extra
+          python3 -m pip install --upgrade "tox>=4.0.0rc1"
 
       - name: Log installed dists
         run: python3 -m pip freeze --all
 
       - name: Initialize tox envs ${{ matrix.tox_env }}
         run: python3 -m tox --notest --skip-missing-interpreters false -vv -e ${{ matrix.tox_env }}
         timeout-minutes: 5 # average is under 1, but macos can be over 3
 
       # sequential run improves browsing experience (almost no speed impact)
-      - name: "Test with tox: ${{ matrix.tox_env }}"
+      - name: tox -e ${{ matrix.tox_env }}
         run: python3 -m tox -e ${{ matrix.tox_env }}
 
       - name: Combine coverage data
+        if: ${{ startsWith(matrix.tox_env, 'py') }}
         # produce a single .coverage file at repo root
         run: tox -e coverage
 
       - name: Upload coverage data
-        if: "runner.os == 'Linux'"
+        if: ${{ startsWith(matrix.tox_env, 'py') }}
         uses: codecov/codecov-action@v3
         with:
           name: ${{ matrix.tox_env }}
           fail_ci_if_error: false # see https://github.com/codecov/codecov-action/issues/598
           token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true # optional (default = false)
 
@@ -232,29 +157,67 @@
         uses: actions/upload-artifact@v3
         with:
           name: logs.zip
           path: .tox/**/log/
         # https://github.com/actions/upload-artifact/issues/123
         continue-on-error: true
 
-      - name: Report junit failures
-        # cspell:disable-next-line
-        uses: shyim/junit-report-annotations-action@3d2e5374f2b13e70f6f3209a21adfdbc42c466ae
+      - name: Report failure if git reports dirty status
+        run: |
+          if [[ -n $(git status -s) ]]; then
+            # shellcheck disable=SC2016
+            echo -n '::error file=git-status::'
+            printf '### Failed as git reported modified and/or untracked files\n```\n%s\n```\n' "$(git status -s)" | tee -a "$GITHUB_STEP_SUMMARY"
+            exit 99
+          fi
+        # https://github.com/actions/toolkit/issues/193
+  codeql:
+    name: codeql
+    runs-on: ubuntu-latest
+    permissions:
+      actions: read
+      contents: read
+      security-events: write
+
+    strategy:
+      fail-fast: false
+      matrix:
+        language: ["python"]
+
+    steps:
+      - name: Checkout repository
+        uses: actions/checkout@v3
+
+      # Initializes the CodeQL tools for scanning.
+      - name: Initialize CodeQL
+        uses: github/codeql-action/init@v2
+        with:
+          languages: ${{ matrix.language }}
+          # If you wish to specify custom queries, you can do so here or in a config file.
+          # By default, queries listed here will override any specified in a config file.
+          # Prefix the list here with "+" to use these queries and those in the config file.
+
+          # Details on CodeQL's query packs refer to : https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/configuring-code-scanning#using-queries-in-ql-packs
+          # queries: security-extended,security-and-quality
+
+      - name: Autobuild
+        uses: github/codeql-action/autobuild@v2
+
+      - name: Perform CodeQL Analysis
+        uses: github/codeql-action/analyze@v2
         with:
-          path: .tox/junit.*.xml
-        if: always()
+          category: "/language:${{matrix.language}}"
 
   check: # This job does nothing and is only used for the branch protection
     if: always()
     permissions:
       pull-requests: write # allow codenotify to comment on pull-request
 
     needs:
-      - linters
-      - unit
+      - build
 
     runs-on: ubuntu-latest
 
     steps:
       - name: Decide whether the needed jobs succeeded or failed
         uses: re-actors/alls-green@release/v1
         with:
```

### Comparing `ansible-lint-6.9.0/.gitignore` & `ansible-lint-6.9.1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 .sandbox
 
 # pyenv
 .python-version
 
 # Coverage artifacts
 .coverage
-coverage.xml
+coverage*.xml
 pip-wheel-metadata
 .test-results/
 
 # mypy
 .mypy_cache
 
 # .cache is used by progressive mode
@@ -61,7 +61,9 @@
 .idea
 src/ansiblelint/_version.py
 *.tar.gz
 .pytest_cache
 test/eco/CODENOTIFY.html
 test/eco
 docs/profiles.md
+test/schemas/node_modules
+.envrc
```

### Comparing `ansible-lint-6.9.0/.packit.yaml` & `ansible-lint-6.9.1/.packit.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -11,24 +11,30 @@
   post-upstream-clone:
     - ./tools/update-version.sh
 srpm_build_deps:
   - python3-build
   - python3-setuptools_scm
 jobs:
   - job: copr_build
-    metadata:
-      targets:
-        # See https://packit.dev/docs/configuration/#aliases
-        # API to get available targets: https://api.dev.testing-farm.io/v0.1/composes/public
-        - fedora-stable
-        - fedora-development
-        # Missing python3-build see https://bugzilla.redhat.com/show_bug.cgi?id=2129071
-        # - centos-stream-9-aarch64
-        # - centos-stream-9-x86_64
+    targets:
+      - fedora-rawhide-aarch64 # one on PR should be enough
     trigger: pull_request
+  - job: copr_build
+    trigger: commit
+    branch: main
+    targets:
+      # See https://packit.dev/docs/configuration/#aliases
+      # API to get available targets: https://api.dev.testing-farm.io/v0.1/composes/public
+      - fedora-rawhide-x86_64
+      - fedora-rawhide-aarch64
+      - fedora-37-x86_64
+      - fedora-37-aarch64
+      # Missing python3-build see https://bugzilla.redhat.com/show_bug.cgi?id=2129071
+      # - centos-stream-9-aarch64
+      # - centos-stream-9-x86_64
   # - job: tests
   #   trigger: pull_request
   #   metadata:
   #     targets:
   #     - fedora-all
   # - job: propose_downstream
   #   trigger: release
```

### Comparing `ansible-lint-6.9.0/.pre-commit-config.yaml` & `ansible-lint-6.9.1/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -6,59 +6,68 @@
   autofix_commit_msg: |
     chore: auto fixes from pre-commit.com hooks
 
     for more information, see https://pre-commit.ci
   skip:
     # https://github.com/pre-commit-ci/issues/issues/55
     - pip-compile
-    - pip-compile-upgrade
     - schemas
-default_language_version:
-  python: python3.9
 exclude: >
   (?x)^(
     .vscode/extensions.json|
     .vscode/settings.json|
+    test/schemas/data/licenses.json|
+    test/schemas/package-lock.json|
+    test/schemas/negative_test|
     examples/broken/yaml-with-tabs/invalid-due-tabs.yaml
   )$
 repos:
+  - repo: meta
+    hooks:
+      - id: check-useless-excludes
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
     rev: v3.0.0-alpha.4
     hooks:
       - id: prettier
         # Temporary excludes so we can gradually normalize the formatting
         exclude: >
           (?x)^(
+            .*\.md$|
             examples/other/some.j2.yaml|
             examples/playbooks/example.yml|
             examples/playbooks/multiline-brackets.*|
             examples/playbooks/templates/not-valid.yaml|
             examples/playbooks/with-umlaut-.*|
             examples/playbooks/with-skip-tag-id.yml|
             examples/yamllint/.*|
             test/fixtures/formatting-before/.*|
-            src/ansiblelint/schemas/.*
+            test/schemas/data/.*|
+            test/schemas/(negative_test|test)/.*\.md|
+            src/ansiblelint/schemas/(molecule|tasks|playbook).json|
+            src/ansiblelint/schemas/ansible-navigator-config.json
           )$
+        always_run: true
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
+          - prettier-plugin-sort-json
   - repo: https://github.com/streetsidesoftware/cspell-cli
-    rev: v6.14.0
+    rev: v6.15.0
     hooks:
       - id: cspell
         # entry: codespell --relative
         args: [--relative, --no-progress, --no-summary]
         name: Spell check with cspell
   - repo: https://github.com/sirosen/check-jsonschema
-    rev: 0.18.4
+    rev: 0.19.2
     hooks:
       - id: check-github-workflows
   - repo: https://github.com/pre-commit/pre-commit-hooks.git
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: end-of-file-fixer
         # ignore formatting-prettier to have an accurate prettier comparison
         exclude: >
           (?x)^(
             test/eco/.*.result|
             examples/yamllint/.*|
@@ -82,14 +91,17 @@
         language_version: python3
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.2
     hooks:
       - id: codespell
         exclude: >
           (?x)^(
+            .config/dictionary.txt|
+            test/schemas/negative_test/.*|
+            test/schemas/test/.*|
             src/ansiblelint/schemas/.*\.json
           )$
   - repo: https://github.com/PyCQA/doc8
     rev: v1.0.0
     hooks:
       - id: doc8
   - repo: https://github.com/adrienverge/yamllint.git
@@ -115,43 +127,43 @@
           - --filter-files
   - repo: https://github.com/psf/black
     rev: 22.10.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pycqa/flake8.git
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         language_version: python3
         additional_dependencies:
           - flake8-2020>=1.6.0
           # - flake8-black>=0.1.1
           - flake8-docstrings>=1.5.0
           - flake8-pytest-style>=1.2.2
           - flake8-future-annotations>=0.0.3
   - repo: https://github.com/asottile/pyupgrade
     # keep it after flake8
-    rev: v3.2.0
+    rev: v3.2.3
     hooks:
       - id: pyupgrade
         args: ["--py38-plus"]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.982
+    rev: v0.991
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
         args: [--strict]
         additional_dependencies:
-          - ansible-compat>=2.2.5
-          - ansible-core
-          - black
+          - ansible-compat>=2.2.6
+          - ansible-core>=2.14.0
+          - black>=22.10.0
           - filelock
           - flaky
-          - pytest
+          - pytest>=7.2.0
           - rich>=11.0.0
           - ruamel.yaml
           - sphinx>=4.4.0
           - types-dataclasses
           - types-docutils
           - types-jsonschema>=4.4.2
           - types-pkg_resources
@@ -160,48 +172,54 @@
           - yamllint
         exclude: >
           (?x)^(
             test/local-content/.*|
             plugins/.*
           )$
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.15.7
     hooks:
       - id: pylint
         additional_dependencies:
-          - ansible-compat>=2.2.5
-          - ansible-core
-          - black
+          - ansible-compat>=2.2.6
+          - ansible-core>=2.14.0
+          - black>=22.10.0
           - docutils
           - filelock
           - flaky
           - jsonschema>=4.9.0
-          - pytest
+          - pytest>=7.2.0
           - pyyaml
           - rich>=11.0.0
           - ruamel.yaml
           - sphinx
           - typing_extensions
           - wcmatch
           - yamllint
+  - repo: https://github.com/jazzband/pip-tools
+    rev: 6.11.0
+    hooks:
+      - id: pip-compile
+        entry: pip-compile --resolver=backtracking -q --no-annotate --output-file=requirements.txt setup.cfg --extra docs --extra test --strip-extras --unsafe-package ansible-core
+        language: python
+        files: ^(requirements\.txt|pyproject\.toml)$
+        alias: deps
+        language_version: "3.9" # minimal we support officially
+        additional_dependencies:
+          - pip>=22.3.1
+      - id: pip-compile
+        entry: pip-compile --resolver=backtracking -q --no-annotate --output-file=requirements.txt setup.cfg --extra docs --extra test --strip-extras --unsafe-package ansible-core --upgrade
+        language: python
+        files: ^(requirements\.txt|pyproject\.toml)$
+        alias: up
+        stages: [manual]
+        language_version: "3.9" # minimal we support officially
+        additional_dependencies:
+          - pip>=22.3.1
   - # keep at bottom as these are slower
     repo: local
     hooks:
       - id: schemas
         name: update json schemas
         entry: python3 src/ansiblelint/schemas/__main__.py
         language: python
         stages: [manual]
-      - id: pip-compile
-        name: pip-compile
-        entry: python3.9 -m piptools compile -q --no-annotate --output-file=requirements.txt setup.cfg --extra docs --extra test --strip-extras --unsafe-package ansible-core
-        language: system
-        files: ^(setup\.cfg|=constraints\.txt)$
-        pass_filenames: false
-        stages: [manual]
-      - id: pip-compile-upgrade
-        name: pip-compile-upgrade
-        entry: python3.9 -m piptools compile -q --upgrade --no-annotate --output-file=requirements.txt setup.cfg --extra docs --extra test --strip-extras --unsafe-package ansible-core
-        language: system
-        files: ^(setup\.cfg|=constraints\.txt)$
-        pass_filenames: false
-        stages: [manual]
```

### Comparing `ansible-lint-6.9.0/.pre-commit-hooks.yaml` & `ansible-lint-6.9.1/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/.prettierignore` & `ansible-lint-6.9.1/.prettierignore`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 .sandbox
 
 # pyenv
 .python-version
 
 # Coverage artifacts
 .coverage
-coverage.xml
+coverage*.xml
 pip-wheel-metadata
 .test-results/
 
 # mypy
 .mypy_cache
 
 # .cache is used by progressive mode
@@ -61,7 +61,9 @@
 .idea
 src/ansiblelint/_version.py
 *.tar.gz
 .pytest_cache
 test/eco/CODENOTIFY.html
 test/eco
 docs/profiles.md
+test/schemas/node_modules
+.envrc
```

### Comparing `ansible-lint-6.9.0/.pylintrc` & `ansible-lint-6.9.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/.readthedocs.yml` & `ansible-lint-6.9.1/.readthedocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -25,25 +25,25 @@
 submodules:
   include: all # []
   exclude: []
   recursive: true
 
 build:
   # when using pre_build, "image:" is not supported and os and tools are required
-  os: ubuntu-20.04
+  os: ubuntu-22.04
   tools:
     python: "3.10"
   jobs:
     pre_build:
       - pip install '.[docs,test]'
       - ansible-lint -L -f docs
 # Optionally set the version of Python and requirements required
 # to build docs
 # python:
-#   version: "3.8"
+#   version: "3.9"
 #   install:
 #     # On https://readthedocs.org/dashboard/ansible-lint/environmentvariables/ we
 #     # do have PIP_CONSTRAINTS=requirements.txt which ensures we install only
 #     # pinned requirements that that we know to be working.
 #     - method: pip
 #       path: .
 #       extra_requirements:
```

### Comparing `ansible-lint-6.9.0/.vscode/settings.json` & `ansible-lint-6.9.1/.vscode/settings.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954545454545454%*

 * *Differences: {"'files.exclude'": "{'build': True}"}*

```diff
@@ -3,15 +3,16 @@
         "editor.defaultFormatter": "esbenp.prettier-vscode"
     },
     "evenBetterToml.formatter.allowedBlankLines": 2,
     "files.exclude": {
         "*.egg-info": true,
         ".pytest_cache": true,
         ".tox": true,
-        "__pycache__": true
+        "__pycache__": true,
+        "build": true
     },
     "git.ignoreLimitWarning": true,
     "grammarly.domain": "technical",
     "grammarly.files.include": [
         "**/*.txt",
         "**/*.md"
     ],
```

### Comparing `ansible-lint-6.9.0/COPYING` & `ansible-lint-6.9.1/COPYING`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/DCO_1_1.md` & `ansible-lint-6.9.1/DCO_1_1.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/PKG-INFO` & `ansible-lint-6.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 Metadata-Version: 2.1
 Name: ansible-lint
-Version: 6.9.0
+Version: 6.9.1
 Summary: Checks playbooks for practices and behavior that could potentially be improved
 Home-page: https://github.com/ansible/ansible-lint
 Author: Will Thames
 Author-email: will@thames.id.au
 Maintainer: Ansible by Red Hat
 Maintainer-email: info@ansible.com
-License: GPLv3
+License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/ansible/ansible-lint/issues
 Project-URL: Release Management, https://github.com/ansible/ansible-lint/releases
 Project-URL: CI: GitHub, https://github.com/ansible/ansible-lint/actions?query=workflow:tox+branch:main+event:push
 Project-URL: Code of Conduct, https://docs.ansible.com/ansible/latest/community/code_of_conduct.html
 Project-URL: Documentation, https://ansible-lint.readthedocs.io/
 Project-URL: Mailing lists, https://docs.ansible.com/ansible/latest/community/communication.html#asking-questions-over-email
 Project-URL: Source Code, https://github.com/ansible/ansible-lint
 Keywords: ansible,lint
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: Jython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Software Development :: Bug Tracking
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: COPYING
 License-File: docs/licenses/LICENSE.mit.txt
 
 [![PyPI version](https://img.shields.io/pypi/v/ansible-lint.svg)](https://pypi.org/project/ansible-lint)
-[![Ansible-lint rules explanation](https://img.shields.io/badge/Ansible--lint-rules%20table-blue.svg)](https://ansible-lint.readthedocs.io/default_rules)
+[![Ansible-lint rules explanation](https://img.shields.io/badge/Ansible--lint-rules-blue.svg)](https://ansible-lint.readthedocs.io/rules/)
 [![Discussions](https://img.shields.io/badge/Discussions-gray.svg)](https://github.com/ansible/ansible-lint/discussions)
 [![GitHub Actions CI/CD](https://github.com/ansible/ansible-lint/workflows/gh/badge.svg)](https://github.com/ansible/ansible-lint/actions?query=workflow%3Agh+branch%3Amain+event%3Apush)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/ansible/ansible-lint.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/ansible-community/ansible-lint/context:python)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 # Ansible-lint
```

### Comparing `ansible-lint-6.9.0/README.md` & `ansible-lint-6.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![PyPI version](https://img.shields.io/pypi/v/ansible-lint.svg)](https://pypi.org/project/ansible-lint)
-[![Ansible-lint rules explanation](https://img.shields.io/badge/Ansible--lint-rules%20table-blue.svg)](https://ansible-lint.readthedocs.io/default_rules)
+[![Ansible-lint rules explanation](https://img.shields.io/badge/Ansible--lint-rules-blue.svg)](https://ansible-lint.readthedocs.io/rules/)
 [![Discussions](https://img.shields.io/badge/Discussions-gray.svg)](https://github.com/ansible/ansible-lint/discussions)
 [![GitHub Actions CI/CD](https://github.com/ansible/ansible-lint/workflows/gh/badge.svg)](https://github.com/ansible/ansible-lint/actions?query=workflow%3Agh+branch%3Amain+event%3Apush)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/ansible/ansible-lint.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/ansible-community/ansible-lint/context:python)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 # Ansible-lint
```

### Comparing `ansible-lint-6.9.0/conftest.py` & `ansible-lint-6.9.1/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/_static/ansible-lint.svg` & `ansible-lint-6.9.1/docs/_static/ansible-lint.svg`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/_static/images/ansible-lint-512.png` & `ansible-lint-6.9.1/docs/_static/images/ansible-lint-512.png`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/_static/images/favicon.ico` & `ansible-lint-6.9.1/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/_static/images/logo_invert.png` & `ansible-lint-6.9.1/docs/_static/images/logo_invert.png`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/_static/theme_overrides.css` & `ansible-lint-6.9.1/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/conf.py` & `ansible-lint-6.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/configuring.md` & `ansible-lint-6.9.1/docs/configuring.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/contributing.md` & `ansible-lint-6.9.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/custom-rules.md` & `ansible-lint-6.9.1/docs/custom-rules.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/index.md` & `ansible-lint-6.9.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/installing.md` & `ansible-lint-6.9.1/docs/installing.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/licenses/LICENSE.mit.txt` & `ansible-lint-6.9.1/docs/licenses/LICENSE.mit.txt`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/philosophy.md` & `ansible-lint-6.9.1/docs/philosophy.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/usage.md` & `ansible-lint-6.9.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/docs/using-profiles.md` & `ansible-lint-6.9.1/docs/using-profiles.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/.config/ansible-lint.yml` & `ansible-lint-6.9.1/examples/.config/ansible-lint.yml`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # and not relative to the CWD of execution. CLI arguments passed to the --exclude
 # option are parsed relative to the CWD of execution.
 exclude_paths:
   - .cache/ # implicit unless exclude_paths is defined in config
   - .github/
   - test/fixtures/formatting-before/
   - test/fixtures/formatting-prettier/
+  - test/schemas/
 # parseable: true
 # quiet: true
 # strict: true
 # verbosity: 1
 
 # Mock modules or roles in order to pass ansible-playbook --syntax-check
 mock_modules:
@@ -29,15 +30,15 @@
 
 # Enable checking of loop variable prefixes in roles
 loop_var_prefix: "{role}_"
 
 # Enforce variable names to follow pattern below, in addition to Ansible own
 # requirements, like avoiding python identifiers. To disable add `var-naming`
 # to skip_list.
-# var_naming_pattern: "^[a-z_][a-z0-9_]*$"
+var_naming_pattern: "^[a-z_][a-z0-9_]*$"
 
 use_default_rules: true
 # Load custom rules from this specific folder
 # rulesdir:
 #   - ./rule/directory/
 
 # Ansible-lint completely ignores rules or tags listed below
@@ -46,14 +47,15 @@
 
 # Ansible-lint does not automatically load rules that have the 'opt-in' tag.
 # You must enable opt-in rules by listing each rule 'id' below.
 enable_list:
   - empty-string-compare # opt-in
   - no-log-password # opt-in
   - no-same-owner # opt-in
+  - name[prefix] # opt-in
   # add yaml here if you want to avoid ignoring yaml checks when yamllint
   # library is missing. Normally its absence just skips using that rule.
   - yaml
 # Report only a subset of tags and fully ignore any others
 # tags:
 #   - jinja[spacing]
 
@@ -97,7 +99,18 @@
 kinds:
   # - playbook: "**/examples/*.{yml,yaml}"
   # - galaxy: "**/folder/galaxy.yml"
   # - tasks: "**/tasks/*.yml"
   # - vars: "**/vars/*.yml"
   # - meta: "**/meta/main.yml"
   - yaml: "**/*.yaml-too"
+
+# List of additional collections to allow in only-builtins rule.
+# only_builtins_allow_collections:
+#   - example_ns.example_collection
+
+# List of additions modules to allow in only-builtins rule.
+# only_builtins_allow_modules:
+#   - example_module
+
+# Allow setting custom prefix for name[prefix] rule
+task_name_prefix: "{stem} | "
```

### Comparing `ansible-lint-6.9.0/examples/inventory/inventory.yml` & `ansible-lint-6.9.1/examples/inventory/inventory.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/inventory/production.yml` & `ansible-lint-6.9.1/examples/inventory/production.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/become-user-without-become-failure.yml` & `ansible-lint-6.9.1/examples/playbooks/rule-partial-become-without-become-fail.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/become-user-without-become-success.yml` & `ansible-lint-6.9.1/examples/playbooks/rule-partial-become-without-become-pass.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/block.yml` & `ansible-lint-6.9.1/examples/playbooks/block.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/blockincludes.yml` & `ansible-lint-6.9.1/examples/playbooks/blockincludes.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/blockincludes2.yml` & `ansible-lint-6.9.1/examples/playbooks/blockincludes2.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/command-check-success.yml` & `ansible-lint-6.9.1/examples/playbooks/command-check-success.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/contains_secrets.transformed.yml` & `ansible-lint-6.9.1/examples/playbooks/contains_secrets.transformed.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/contains_secrets.yml` & `ansible-lint-6.9.1/examples/playbooks/contains_secrets.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/example.yml` & `ansible-lint-6.9.1/examples/playbooks/example.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/jinja-spacing.yml` & `ansible-lint-6.9.1/examples/playbooks/jinja-spacing.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/lots_of_warnings.transformed.yml` & `ansible-lint-6.9.1/examples/playbooks/lots_of_warnings.transformed.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/lots_of_warnings.yml` & `ansible-lint-6.9.1/examples/playbooks/lots_of_warnings.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/multiline-brackets-do-not-match-test.yml` & `ansible-lint-6.9.1/examples/playbooks/multiline-brackets-do-not-match-test.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/multiline-bracketsmatchtest.yml` & `ansible-lint-6.9.1/examples/playbooks/multiline-bracketsmatchtest.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/no-prompting.yml` & `ansible-lint-6.9.1/examples/playbooks/no-prompting.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/rule-jinja-valid.yml` & `ansible-lint-6.9.1/examples/playbooks/rule-jinja-valid.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/rule-key-order-fail.yml` & `ansible-lint-6.9.1/examples/playbooks/rule-key-order-fail.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/rule-no-free-form-pass.yml` & `ansible-lint-6.9.1/examples/playbooks/rule-no-free-form-pass.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/rule-risky-file-permissions-fail.yml` & `ansible-lint-6.9.1/examples/playbooks/rule-risky-file-permissions-fail.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/rule-risky-file-permissions-pass.yml` & `ansible-lint-6.9.1/examples/playbooks/rule-risky-file-permissions-pass.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/rule-var-naming-fail.yml` & `ansible-lint-6.9.1/examples/playbooks/rule-var-naming-fail.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/skiptasks.yml` & `ansible-lint-6.9.1/examples/playbooks/skiptasks.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/test_skip_inside_yaml.yml` & `ansible-lint-6.9.1/examples/playbooks/test_skip_inside_yaml.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/using-bare-variables-failure.yml` & `ansible-lint-6.9.1/examples/playbooks/using-bare-variables-failure.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/using-bare-variables-success.yml` & `ansible-lint-6.9.1/examples/playbooks/using-bare-variables-success.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/vars/jinja-spacing.yml` & `ansible-lint-6.9.1/examples/playbooks/vars/jinja-spacing.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/vars/not_decryptable.yml` & `ansible-lint-6.9.1/examples/playbooks/vars/not_decryptable.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/vars/strings.transformed.yml` & `ansible-lint-6.9.1/examples/playbooks/vars/strings.transformed.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/playbooks/vars/strings.yml` & `ansible-lint-6.9.1/examples/playbooks/vars/strings.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/roles/dependency_in_meta/meta/main.yml` & `ansible-lint-6.9.1/examples/roles/dependency_in_meta/meta/main.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/roles/hello/meta/argument_specs.yml` & `ansible-lint-6.9.1/examples/roles/hello/meta/argument_specs.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/examples/roles/loop_var_prefix/tasks/fail.yml` & `ansible-lint-6.9.1/examples/roles/loop_var_prefix/tasks/fail.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 ---
 # 5 expected loop-var-prefix failures at 3, 9, 19, 26, 33
-- name: That should trigger loop-var-prefix
+- name: fail | That should trigger loop-var-prefix
   ansible.builtin.debug:
     var: item
   loop:
     - foo
     - bar
-- name: That should fail due to wrong prefix
+- name: fail | That should fail due to wrong prefix
   ansible.builtin.debug:
     var: zz_item
   loop:
     - foo
     - bar
   loop_control:
     loop_var: zz_item
-- name: Using a block
+- name: fail | Using a block
   block:
-    - name: That should also not pass
+    - name: fail | That should also not pass
       ansible.builtin.debug:
         var: item
       loop:
         - apples
         - oranges
   rescue:
-    - name: That should also not pass
+    - name: fail | That should also not pass
       ansible.builtin.debug:
         var: item
       loop:
         - avocados
         - kiwis
   always:
-    - name: That should also not pass
+    - name: fail | That should also not pass
       ansible.builtin.debug:
         var: item
       loop:
         - bananas
         - muscats
```

### Comparing `ansible-lint-6.9.0/examples/roles/role_for_no_same_owner/tasks/fail.yml` & `ansible-lint-6.9.1/examples/roles/role_for_no_same_owner/tasks/pass.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,32 @@
 ---
-- name: Block
-  block:
-    - name: Synchronize-in-block
-      ansible.posix.synchronize:
-        src: dummy
-        dest: dummy
-
-- name: Synchronize
+- name: pass | Synchronize-delegate
   ansible.posix.synchronize:
     src: dummy
     dest: dummy
-
-- name: Nested-block
-  block:
-    - name: Synchronize
-      block:
-        - name: Synchronize-in-deep-block
-          ansible.posix.synchronize:
-            src: dummy
-            dest: dummy
-  rescue:
-    - name: Synchronize-in-rescue
-      ansible.posix.synchronize:
-        src: dummy
-        dest: dummy
-  always:
-    - name: Synchronize-in-always
-      ansible.posix.synchronize:
-        src: dummy
-        dest: dummy
-
-- name: Unarchive-bz2
-  ansible.builtin.unarchive:
-    src: "{{ file }}.tar.bz2"
-    dest: dummy
-
-- name: Unarchive delegated
-  ansible.builtin.unarchive:
-    src: "{{ file }}.tar.bz2"
-    dest: dummy
   delegate_to: localhost
 
-- name: Unarchive-gz
-  ansible.builtin.unarchive:
-    src: "{{ file }}.tar.gz"
-    dest: dummy
-
-- name: Unarchive-tar
-  ansible.builtin.unarchive:
-    src: "{{ file }}.tar"
+- name: pass | Synchronize-no-same-owner
+  ansible.posix.synchronize:
+    src: dummy
     dest: dummy
+    owner: false
+    group: false
 
-- name: Unarchive-xz
+- name: pass | Unarchive-no-same-owner
   ansible.builtin.unarchive:
-    src: "{{ file }}.tar.xz"
+    src: "{{ file }}.tar.gz"
     dest: dummy
+    extra_opts:
+      - --no-same-owner
 
-- name: Unarchive-zip
+- name: pass | Unarchive-remote-src
   ansible.builtin.unarchive:
-    src: "{{ file }}.zip"
+    src: "{{ file }}.tar.gz"
     dest: dummy
     extra_opts:
-      - -X
+      - --no-same-owner
 
-- name: Unarchive-zip-same-owner
+- name: pass | Unarchive-unknown-file-ending
   ansible.builtin.unarchive:
-    src: "{{ file }}.zip"
+    src: "{{ file }}"
     dest: dummy
-    extra_opts:
-      - -X
```

### Comparing `ansible-lint-6.9.0/examples/rules/task_has_tag.py` & `ansible-lint-6.9.1/examples/rules/task_has_tag.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/mypy.ini` & `ansible-lint-6.9.1/mypy.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [mypy]
-python_version = 3.8
+python_version = 3.9
 color_output = True
 error_summary = True
 disallow_untyped_calls = True
 disallow_untyped_defs = True
 disallow_any_generics = True
 ; disallow_any_unimported = True
 ; warn_redundant_casts = True
```

### Comparing `ansible-lint-6.9.0/pyproject.toml` & `ansible-lint-6.9.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -11,21 +11,25 @@
 target-version = ["py38"]
 
 [tool.coverage.run]
 source_pkgs = ["ansiblelint"]
 branch = true
 parallel = true
 concurrency = ["multiprocessing", "thread"]
+data_file = ".tox/.coverage"
 
 [tool.coverage.paths]
 source = ["src", ".tox/*/site-packages"]
 
 [tool.coverage.report]
 exclude_lines = ["pragma: no cover", "if TYPE_CHECKING:"]
 omit = ["*/src/ansible_compat/*", "test/*"]
+fail_under = 88
+skip_covered = true
+skip_empty = true
 
 [tool.isort]
 profile = "black"
 add_imports = "from __future__ import annotations"
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
```

### Comparing `ansible-lint-6.9.0/pytest.ini` & `ansible-lint-6.9.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/requirements.txt` & `ansible-lint-6.9.1/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
-#    pip-compile --extra=docs --extra=test --no-annotate --output-file=requirements.txt --strip-extras --unsafe-package=ansible-core setup.cfg
+#    pip-compile --extra=docs --extra=test --no-annotate --output-file=requirements.txt --resolver=backtracking --strip-extras --unsafe-package=ansible-core setup.cfg
 #
 alabaster==0.7.12
-ansible-compat==2.2.5
+ansible-compat==2.2.6
 ansible-pygments==0.1.1
-astroid==2.12.12
+astroid==2.12.13
 attrs==22.1.0
 babel==2.11.0
 black==22.10.0
 bracex==2.3.post1
 certifi==2022.9.24
 cffi==1.15.1
 charset-normalizer==2.1.1
 click==8.1.3
 commonmark==0.9.1
 coverage==6.5.0
 coverage-enable-subprocess==1.0
-cryptography==38.0.3
+cryptography==38.0.4
 dill==0.3.6
 docutils==0.17.1
 exceptiongroup==1.0.4
 execnet==1.9.0
 filelock==3.8.0
-flake8==5.0.4
+flake8==6.0.0
 flake8-future-annotations==1.0.0
 flaky==3.7.0
 idna==3.4
 imagesize==1.4.1
-importlib-metadata==5.0.0
+importlib-metadata==5.1.0
 iniconfig==1.1.1
 isort==5.10.1
 jinja2==3.1.2
-jsonschema==4.17.0
+jsonschema==4.17.3
 lazy-object-proxy==1.8.0
 markdown-it-py==2.1.0
 markupsafe==2.1.1
 mccabe==0.7.0
 mdit-py-plugins==0.3.1
 mdurl==0.1.2
 more-itertools==9.0.0
@@ -48,25 +48,25 @@
 packaging==21.3
 pathspec==0.10.2
 pbr==5.11.0
 pipdeptree==2.3.3
 platformdirs==2.5.4
 pluggy==1.0.0
 psutil==5.9.4
-pycodestyle==2.9.1
+pycodestyle==2.10.0
 pycparser==2.21
-pyflakes==2.5.0
+pyflakes==3.0.1
 pygments==2.13.0
-pylint==2.15.5
+pylint==2.15.7
 pyparsing==3.0.9
 pyrsistent==0.19.2
 pytest==7.2.0
 pytest-mock==3.10.0
 pytest-plus==0.2
-pytest-xdist==3.0.2
+pytest-xdist==3.1.0
 pytz==2022.6
 pyyaml==6.0
 requests==2.28.1
 resolvelib==0.8.1
 rich==12.6.0
 ruamel-yaml==0.17.21
 ruamel-yaml-clib==0.2.7
@@ -78,19 +78,19 @@
 sphinxcontrib-applehelp==1.0.2
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.0
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-programoutput2==2.0a1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-subprocess-tee==0.3.5
+subprocess-tee==0.4.0
 tomli==2.0.1
 tomlkit==0.11.6
 typing-extensions==4.4.0
-urllib3==1.26.12
+urllib3==1.26.13
 wcmatch==8.4.1
 wrapt==1.14.1
 yamllint==1.28.0
-zipp==3.10.0
+zipp==3.11.0
 
 # The following packages are considered to be unsafe in a requirements file:
 # ansible-core
```

### Comparing `ansible-lint-6.9.0/requirements.yml` & `ansible-lint-6.9.1/requirements.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/setup.cfg` & `ansible-lint-6.9.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -12,46 +12,37 @@
 description = Checks playbooks for practices and behavior that could potentially be improved
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Will Thames
 author_email = will@thames.id.au
 maintainer = Ansible by Red Hat
 maintainer_email = info@ansible.com
-license = GPLv3
+license = GPLv3+
 license_files = 
 	COPYING
 	docs/licenses/LICENSE*.*
 classifiers = 
 	Development Status :: 5 - Production/Stable
-	
 	Environment :: Console
-	
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
-	
-	Operating System :: OS Independent
-	
-	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-	
+	Operating System :: MacOS
+	Operating System :: POSIX
+	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+	Natural Language :: English
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
-	Programming Language :: Python :: Implementation
-	Programming Language :: Python :: Implementation :: CPython
-	Programming Language :: Python :: Implementation :: Jython
-	Programming Language :: Python :: Implementation :: PyPy
-	
-	Topic :: Software Development :: Bug Tracking
+	Programming Language :: Python :: 3 :: Only
 	Topic :: Software Development :: Quality Assurance
 	Topic :: Software Development :: Testing
-	
 	Topic :: Utilities
 keywords = 
 	ansible
 	lint
 
 [options]
 use_scm_version = True
@@ -60,24 +51,24 @@
 	= src
 packages = find:
 zip_safe = False
 install_requires = 
 	will-not-work-on-windows-try-from-wsl-instead; platform_system=="Windows"
 	ansible-core>=2.12.0,<2.14.0; python_version<"3.9"  # GPLv3
 	ansible-core>=2.12.0; python_version>="3.9"  # GPLv3
-	ansible-compat>=2.2.5  # GPLv3
+	ansible-compat>=2.2.6  # GPLv3
 	black>=22.8.0  # MIT
-	filelock>=3.8.0  # The Unlicense
-	jsonschema>=4.17.0  # MIT, version needed for improved errors
+	filelock>=3.3.0  # The Unlicense
+	jsonschema>=4.10.0  # MIT, version needed for improved errors
 	packaging>=21.3  # Apache-2.0,BSD-2-Clause
 	pyyaml>=5.4.1  # MIT (centos 9 has 5.3.1)
 	rich>=12.0.0  # MIT
 	ruamel.yaml >= 0.17.21, < 0.18  # MIT, next version is planned to have breaking changes
 	yamllint >= 1.26.3  # GPLv3
-	wcmatch>=8.3.2  # MIT
+	wcmatch>=8.1.2  # MIT
 
 [options.entry_points]
 console_scripts = 
 	ansible-lint = ansiblelint.__main__:_run_cli_entrypoint
 
 [options.extras_require]
 docs =
```

### Comparing `ansible-lint-6.9.0/src/ansible_lint.egg-info/PKG-INFO` & `ansible-lint-6.9.1/src/ansible_lint.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 Metadata-Version: 2.1
 Name: ansible-lint
-Version: 6.9.0
+Version: 6.9.1
 Summary: Checks playbooks for practices and behavior that could potentially be improved
 Home-page: https://github.com/ansible/ansible-lint
 Author: Will Thames
 Author-email: will@thames.id.au
 Maintainer: Ansible by Red Hat
 Maintainer-email: info@ansible.com
-License: GPLv3
+License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/ansible/ansible-lint/issues
 Project-URL: Release Management, https://github.com/ansible/ansible-lint/releases
 Project-URL: CI: GitHub, https://github.com/ansible/ansible-lint/actions?query=workflow:tox+branch:main+event:push
 Project-URL: Code of Conduct, https://docs.ansible.com/ansible/latest/community/code_of_conduct.html
 Project-URL: Documentation, https://ansible-lint.readthedocs.io/
 Project-URL: Mailing lists, https://docs.ansible.com/ansible/latest/community/communication.html#asking-questions-over-email
 Project-URL: Source Code, https://github.com/ansible/ansible-lint
 Keywords: ansible,lint
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: Jython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Software Development :: Bug Tracking
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: COPYING
 License-File: docs/licenses/LICENSE.mit.txt
 
 [![PyPI version](https://img.shields.io/pypi/v/ansible-lint.svg)](https://pypi.org/project/ansible-lint)
-[![Ansible-lint rules explanation](https://img.shields.io/badge/Ansible--lint-rules%20table-blue.svg)](https://ansible-lint.readthedocs.io/default_rules)
+[![Ansible-lint rules explanation](https://img.shields.io/badge/Ansible--lint-rules-blue.svg)](https://ansible-lint.readthedocs.io/rules/)
 [![Discussions](https://img.shields.io/badge/Discussions-gray.svg)](https://github.com/ansible/ansible-lint/discussions)
 [![GitHub Actions CI/CD](https://github.com/ansible/ansible-lint/workflows/gh/badge.svg)](https://github.com/ansible/ansible-lint/actions?query=workflow%3Agh+branch%3Amain+event%3Apush)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/ansible/ansible-lint.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/ansible-community/ansible-lint/context:python)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 # Ansible-lint
```

### Comparing `ansible-lint-6.9.0/src/ansible_lint.egg-info/requires.txt` & `ansible-lint-6.9.1/src/ansible_lint.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-ansible-compat>=2.2.5
+ansible-compat>=2.2.6
 black>=22.8.0
-filelock>=3.8.0
-jsonschema>=4.17.0
+filelock>=3.3.0
+jsonschema>=4.10.0
 packaging>=21.3
 pyyaml>=5.4.1
 rich>=12.0.0
 ruamel.yaml<0.18,>=0.17.21
 yamllint>=1.26.3
-wcmatch>=8.3.2
+wcmatch>=8.1.2
 
 [:platform_system == "Windows"]
 will-not-work-on-windows-try-from-wsl-instead
 
 [:python_version < "3.9"]
 ansible-core<2.14.0,>=2.12.0
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/__init__.py` & `ansible-lint-6.9.1/src/ansiblelint/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/__main__.py` & `ansible-lint-6.9.1/src/ansiblelint/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,21 @@
 from ansible_compat.config import ansible_version
 from ansible_compat.prerun import get_cache_dir
 from filelock import FileLock, Timeout
 
 from ansiblelint import cli
 from ansiblelint._mockings import _perform_mockings_cleanup
 from ansiblelint.app import get_app
-from ansiblelint.color import console, console_options, reconfigure, render_yaml
+from ansiblelint.color import (
+    console,
+    console_options,
+    console_stderr,
+    reconfigure,
+    render_yaml,
+)
 from ansiblelint.config import get_version_warning, options
 from ansiblelint.constants import EXIT_CONTROL_C_RC, LOCK_TIMEOUT_RC
 from ansiblelint.file_utils import abspath, cwd, normpath
 from ansiblelint.skip_utils import normalize_tag
 from ansiblelint.version import __version__
 
 if TYPE_CHECKING:
@@ -107,22 +113,22 @@
     os.makedirs(options.cache_dir, exist_ok=True)
 
     options.cache_dir_lock = None
     if not options.offline:
         options.cache_dir_lock = FileLock(f"{options.cache_dir}/.lock")
         try:
             options.cache_dir_lock.acquire(timeout=180)
-        except Timeout:
+        except Timeout:  # pragma: no cover
             _logger.error(
                 "Timeout waiting for another instance of ansible-lint to release the lock."
             )
             sys.exit(LOCK_TIMEOUT_RC)
 
     # Avoid extra output noise from Ansible about using devel versions
-    if "ANSIBLE_DEVEL_WARNING" not in os.environ:
+    if "ANSIBLE_DEVEL_WARNING" not in os.environ:  # pragma: no branch
         os.environ["ANSIBLE_DEVEL_WARNING"] = "false"
 
 
 def _do_list(rules: RulesCollection) -> int:
     # On purpose lazy-imports to avoid pre-loading Ansible
     # pylint: disable=import-outside-toplevel
     from ansiblelint.generate_docs import (
@@ -166,14 +172,24 @@
 
     transformer = Transformer(result, options)
 
     # this will mark any matches as fixed if the transforms repaired the issue
     transformer.run()
 
 
+def support_banner() -> None:
+    """Display support banner when running on unsupported platform."""
+    if sys.version_info < (3, 9, 0):
+        prefix = "::warning::" if "GITHUB_ACTION" in os.environ else "WARNING: "
+        console_stderr.print(
+            f"{prefix}ansible-lint is no longer tested under Python {sys.version_info.major}.{sys.version_info.minor} and will soon require 3.9. Do not report bugs for this version.",
+            style="bold red",
+        )
+
+
 # pylint: disable=too-many-branches,too-many-statements
 def main(argv: list[str] | None = None) -> int:  # noqa: C901
     """Linter CLI entry point."""
     # alter PATH if needed (venv support)
     path_inject()
 
     if argv is None:
@@ -186,15 +202,18 @@
     if options.version:
         console.print(
             f"ansible-lint [repr.number]{__version__}[/] using ansible [repr.number]{ansible_version()}[/]"
         )
         msg = get_version_warning()
         if msg:
             console.print(msg)
+        support_banner()
         sys.exit(0)
+    else:
+        support_banner()
 
     initialize_logger(options.verbosity)
     _logger.debug("Options: %s", options)
     _logger.debug(os.getcwd())
 
     if not options.offline:
         # refresh schemas must happen before loading rules
@@ -324,19 +343,19 @@
 
     This function also processes the runtime exceptions.
     """
     try:
         sys.exit(main(sys.argv))
     except OSError as exc:
         # NOTE: Only "broken pipe" is acceptable to ignore
-        if exc.errno != errno.EPIPE:
+        if exc.errno != errno.EPIPE:  # pragma: no cover
             raise
-    except KeyboardInterrupt:
+    except KeyboardInterrupt:  # pragma: no cover
         sys.exit(EXIT_CONTROL_C_RC)
-    except RuntimeError as exc:
+    except RuntimeError as exc:  # pragma: no cover
         raise SystemExit(exc) from exc
 
 
 def path_inject() -> None:
     """Add python interpreter path to top of PATH to fix outside venv calling."""
     # This make it possible to call ansible-lint that was installed inside a
     # virtualenv without having to pre-activate it. Otherwise subprocess will
@@ -393,15 +412,15 @@
     if isinstance(value, str):
         value = value.lower()
     if value in ("yes", "on", "1", "true", 1):
         return True
     return False
 
 
-def should_do_markup(stream: TextIO = sys.stdout) -> bool:
+def should_do_markup(stream: TextIO = sys.stdout) -> bool:  # pragma: no cover
     """Decide about use of ANSI colors."""
     py_colors = None
 
     # https://xkcd.com/927/
     for env_var in ["PY_COLORS", "CLICOLOR", "FORCE_COLOR", "ANSIBLE_FORCE_COLOR"]:
         value = os.environ.get(env_var, None)
         if value is not None:
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/_internal/internal_error.md` & `ansible-lint-6.9.1/src/ansiblelint/_internal/internal_error.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/_internal/rules.py` & `ansible-lint-6.9.1/src/ansiblelint/_internal/rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import TYPE_CHECKING, Any
 
 from ansiblelint.constants import RULE_DOC_URL
 
 if TYPE_CHECKING:
     from ansiblelint.errors import MatchError
     from ansiblelint.file_utils import Lintable
+    from ansiblelint.rules import RulesCollection
 
 _logger = logging.getLogger(__name__)
 LOAD_FAILURE_MD = """\
 # load-failure
 
 Linter failed to process a YAML file, probably because it is either:
 
@@ -44,14 +45,16 @@
     needs_raw_task: bool = False
     # We use _order to sort rules and to ensure that some run before others,
     # _order 0 for internal rules
     # _order 1 for rules that check that data can be loaded
     # _order 5 implicit for normal rules
     _order: int = 5
     _help: str | None = None
+    # Added when a rule is registered into a collection, gives access to options
+    _collection: RulesCollection | None = None
 
     @property
     def help(self) -> str:
         """Return a help markdown string for the rule."""
         if self._help is None:
             self._help = ""
             md_file = (
@@ -61,15 +64,20 @@
             if md_file.exists():
                 self._help = md_file.read_text(encoding="utf-8")
         return self._help
 
     @property
     def url(self) -> str:
         """Return rule documentation url."""
-        return self.link or RULE_DOC_URL + self.id + "/"
+        url = self.link
+        if not url:
+            url = RULE_DOC_URL
+            if self.id:
+                url += self.id + "/"
+        return url
 
     @property
     def shortdesc(self) -> str:
         """Return the short description of the rule, basically the docstring."""
         return self.__doc__ or ""
 
     def getmatches(self, file: Lintable) -> list[MatchError]:
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/_internal/warning.md` & `ansible-lint-6.9.1/src/ansiblelint/_internal/warning.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/_mockings.py` & `ansible-lint-6.9.1/src/ansiblelint/_mockings.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/app.py` & `ansible-lint-6.9.1/src/ansiblelint/app.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/cli.py` & `ansible-lint-6.9.1/src/ansiblelint/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,14 +458,15 @@
         "skip_list": [],
         "tags": [],
         "warn_list": DEFAULT_WARN_LIST,
         "mock_modules": [],
         "mock_roles": [],
         "enable_list": [],
         "only_builtins_allow_collections": [],
+        "only_builtins_allow_modules": [],
         # do not include "write_list" here. See special logic below.
     }
 
     scalar_map = {
         "loop_var_prefix": None,
         "project_dir": ".",
         "profile": None,
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/color.py` & `ansible-lint-6.9.1/src/ansiblelint/color.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/config.py` & `ansible-lint-6.9.1/src/ansiblelint/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Store configuration options as a singleton."""
 from __future__ import annotations
 
 import json
 import logging
 import os
-import re
 import sys
 import time
 import urllib.request
 import warnings
 from argparse import Namespace
 from functools import lru_cache
 from pathlib import Path
@@ -31,14 +30,15 @@
     "avoid-implicit",
     "experimental",
     "fqcn[action]",
     "fqcn[redirect]",
     "jinja[spacing]",  # warning until we resolve all reported false-positives
     "name[casing]",
     "name[play]",
+    "name[prefix]",
     "role-name",
     "warning[empty-playbook]",  # because ansible considers it warning only
     "role-name[path]",  # too new
 ]
 
 DEFAULT_KINDS = [
     # Do not sort this list, order matters.
@@ -119,65 +119,55 @@
     warn_list=[],
     kinds=DEFAULT_KINDS,
     mock_filters=[],
     mock_modules=[],
     mock_roles=[],
     loop_var_prefix=None,
     only_builtins_allow_collections=[],
+    only_builtins_allow_modules=[],
     var_naming_pattern=None,
     offline=False,
     project_dir=".",  # default should be valid folder (do not use None here)
     extra_vars=None,
     enable_list=[],
     skip_action_validation=True,
     strict=False,
     rules={},  # Placeholder to set and keep configurations for each rule.
     profile=None,
+    task_name_prefix="{stem} | ",
 )
 
 # Used to store detected tag deprecations
 used_old_tags: dict[str, str] = {}
 
 # Used to store collection list paths (with mock paths if needed)
 collection_list: list[str] = []
 
 
 def get_rule_config(rule_id: str) -> dict[str, Any]:
     """Get configurations for the rule ``rule_id``."""
     rule_config = options.rules.get(rule_id, {})
-    if not isinstance(rule_config, dict):
+    if not isinstance(rule_config, dict):  # pragma: no branch
         raise RuntimeError(f"Invalid rule config for {rule_id}: {rule_config}")
     return rule_config
 
 
 @lru_cache
 def ansible_collections_path() -> str:
     """Return collection path variable for current version of Ansible."""
     # respect Ansible behavior, which is to load old name if present
-    for env_var in ["ANSIBLE_COLLECTIONS_PATHS", "ANSIBLE_COLLECTIONS_PATH"]:
+    for env_var in [
+        "ANSIBLE_COLLECTIONS_PATHS",
+        "ANSIBLE_COLLECTIONS_PATH",
+    ]:  # pragma: no cover
         if env_var in os.environ:
             return env_var
     return "ANSIBLE_COLLECTIONS_PATH"
 
 
-def parse_ansible_version(stdout: str) -> tuple[str, str | None]:
-    """Parse output of 'ansible --version'."""
-    # Ansible can produce extra output before displaying version in debug mode.
-
-    # ansible-core 2.11+: 'ansible [core 2.11.3]'
-    match = re.search(r"^ansible \[(?:core|base) ([^\]]+)\]", stdout, re.MULTILINE)
-    if match:
-        return match.group(1), None
-    # ansible-base 2.10 and Ansible 2.9: 'ansible 2.x.y'
-    match = re.search(r"^ansible ([^\s]+)", stdout, re.MULTILINE)
-    if match:
-        return match.group(1), None
-    return "", f"FATAL: Unable parse ansible cli version: {stdout}"
-
-
 def in_venv() -> bool:
     """Determine whether Python is running from a venv."""
     if hasattr(sys, "real_prefix") or os.environ.get("CONDA_EXE", None) is not None:
         return True
 
     pfx = getattr(sys, "base_prefix", sys.prefix)
     return pfx != sys.prefix
@@ -228,22 +218,22 @@
     # We only want to recommend pip for upgrade if it looks safe to do so.
     return pip if use_pip else ""
 
 
 def get_version_warning() -> str:
     """Display warning if current version is outdated."""
     # 0.1dev1 is special fallback version
-    if __version__ == "0.1.dev1":
+    if __version__ == "0.1.dev1":  # pragma: no cover
         return ""
 
     msg = ""
     data = {}
     current_version = Version(__version__)
 
-    if not os.path.exists(CACHE_DIR):
+    if not os.path.exists(CACHE_DIR):  # pragma: no cover
         os.makedirs(CACHE_DIR)
     cache_file = f"{CACHE_DIR}/latest.json"
     refresh = True
     if os.path.exists(cache_file):
         age = time.time() - os.path.getmtime(cache_file)
         if age < 24 * 60 * 60:
             refresh = False
@@ -255,15 +245,15 @@
             "https://api.github.com/repos/ansible/ansible-lint/releases/latest"
         )
         try:
             with urllib.request.urlopen(release_url) as url:
                 data = json.load(url)
                 with open(cache_file, "w", encoding="utf-8") as f:
                     json.dump(data, f)
-        except (URLError, HTTPError) as exc:
+        except (URLError, HTTPError) as exc:  # pragma: no cover
             _logger.debug(
                 "Unable to fetch latest version from %s due to: %s", release_url, exc
             )
             return ""
 
     html_url = data["html_url"]
     new_version = Version(data["tag_name"][1:])  # removing v prefix from tag
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/constants.py` & `ansible-lint-6.9.1/src/ansiblelint/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     "rescue",
 ]
 
 # Keys that are used internally when parsing YAML/JSON files
 SKIPPED_RULES_KEY = "__skipped_rules__"
 LINE_NUMBER_KEY = "__line__"
 FILENAME_KEY = "__file__"
-
+ANNOTATION_KEYS = [FILENAME_KEY, LINE_NUMBER_KEY, SKIPPED_RULES_KEY]
 
 INCLUSION_ACTION_NAMES = {
     "include",
     "include_tasks",
     "import_playbook",
     "import_tasks",
     "ansible.builtin.include",
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/data/profiles.yml` & `ansible-lint-6.9.1/src/ansiblelint/data/profiles.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/errors.py` & `ansible-lint-6.9.1/src/ansiblelint/errors.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/file_utils.py` & `ansible-lint-6.9.1/src/ansiblelint/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         # if the lintable is part of a role, we save role folder name
         self.role = ""
         parts = self.path.parent.parts
         if "roles" in parts:
             role = self.path
             while role.parent.name != "roles" and role.name:
                 role = role.parent
-            if role.exists:
+            if role.exists():
                 self.role = role.name
 
         if str(self.path) in ["/dev/stdin", "-"]:
             # pylint: disable=consider-using-with
             self.file = NamedTemporaryFile(mode="w+", suffix="playbook.yml")
             self.filename = self.file.name
             self._content = sys.stdin.read()
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/formatters/__init__.py` & `ansible-lint-6.9.1/src/ansiblelint/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/generate_docs.py` & `ansible-lint-6.9.1/src/ansiblelint/generate_docs.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/loaders.py` & `ansible-lint-6.9.1/src/ansiblelint/loaders.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/__init__.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,14 @@
         if not match.details:
             match.details = "Task/Handler: " + ansiblelint.utils.task_to_str(task)
         if match.linenumber < task[LINE_NUMBER_KEY]:
             match.linenumber = task[LINE_NUMBER_KEY]
 
     def matchlines(self, file: Lintable) -> list[MatchError]:
         matches: list[MatchError] = []
-        if not self.match:
-            return matches
         # arrays are 0-based, line numbers are 1-based
         # so use prev_line_no as the counter
         for (prev_line_no, line) in enumerate(file.content.split("\n")):
             if line.lstrip().startswith("#"):
                 continue
 
             rule_id_list = ansiblelint.skip_utils.get_rule_skips_from_line(line)
@@ -147,16 +145,15 @@
 
         Most rules will never need to override matchtasks because its main
         purpose is to call matchtask for each task/handlers in the same file,
         and to aggregate the results.
         """
         matches: list[MatchError] = []
         if (
-            not self.matchtask
-            or file.kind not in ["handlers", "tasks", "playbook"]
+            file.kind not in ["handlers", "tasks", "playbook"]
             or str(file.base_kind) != "text/yaml"
         ):
             return matches
 
         tasks_iterator = ansiblelint.yaml_utils.iter_tasks_in_file(file)
         for raw_task, task, skipped_tags, error in tasks_iterator:
             if error is not None:
@@ -204,15 +201,15 @@
 
             self._enrich_matcherror_with_task_details(match, task)
             matches.append(match)
         return matches
 
     def matchyaml(self, file: Lintable) -> list[MatchError]:
         matches: list[MatchError] = []
-        if not self.matchplay or str(file.base_kind) != "text/yaml":
+        if str(file.base_kind) != "text/yaml":
             return matches
 
         yaml = file.data
         # yaml returned can be an AnsibleUnicode (a string) when the yaml
         # file contains a single string. YAML spec allows this but we consider
         # this an fatal error.
         if isinstance(yaml, str):
@@ -411,14 +408,15 @@
                 self.profile,  # when profile is used we load all rules and filter later
                 "opt-in" not in obj.tags,
                 obj.id in self.options.enable_list,
                 self.options.list_rules,
                 self.options.list_tags,
             ]
         ):
+            obj._collection = self  # pylint: disable=protected-access
             self.rules.append(obj)
 
     def __iter__(self) -> Iterator[BaseRule]:
         """Return the iterator over the rules in the RulesCollection."""
         return iter(sorted(self.rules))
 
     def alphabetical(self) -> Iterator[BaseRule]:
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/avoid_implicit.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/avoid_implicit.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/avoid_implicit.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/avoid_implicit.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/command_instead_of_module.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/command_instead_of_module.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/command_instead_of_module.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/command_instead_of_module.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/command_instead_of_shell.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/command_instead_of_shell.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/command_instead_of_shell.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/command_instead_of_shell.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_bare_vars.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_bare_vars.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_bare_vars.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_bare_vars.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_command_syntax.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_command_syntax.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_command_syntax.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_command_syntax.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_local_action.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_local_action.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_module.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_module.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/deprecated_module.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/deprecated_module.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/empty_string_compare.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/empty_string_compare.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/empty_string_compare.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/empty_string_compare.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/fqcn.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/fqcn.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/fqcn.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/fqcn.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/galaxy.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/galaxy.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/galaxy.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/galaxy.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/ignore_errors.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/ignore_errors.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/ignore_errors.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/ignore_errors.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/inline_env_var.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/inline_env_var.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/inline_env_var.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/inline_env_var.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/jinja.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/jinja.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/jinja.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/jinja.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,43 +14,25 @@
 from jinja2.exceptions import TemplateSyntaxError
 
 from ansiblelint.constants import LINE_NUMBER_KEY
 from ansiblelint.file_utils import Lintable
 from ansiblelint.rules import AnsibleLintRule
 from ansiblelint.skip_utils import get_rule_skips_from_line
 from ansiblelint.utils import parse_yaml_from_file, template
-from ansiblelint.yaml_utils import nested_items_path
+from ansiblelint.yaml_utils import deannotate, nested_items_path
 
 if TYPE_CHECKING:
     from ansiblelint.errors import MatchError
 
 
 _logger = logging.getLogger(__package__)
 KEYWORDS_WITH_IMPLICIT_TEMPLATE = ("changed_when", "failed_when", "until", "when")
 
 Token = namedtuple("Token", "lineno token_type value")
 
-DEANNOTATE_KEYS = ("__file__", "__line__", "__start_line__", "__end_line__")
-
-
-def deannotate(data: Any) -> Any:
-    """Remove our annotations like __file__ and __line__ and return a JSON serializable object."""
-    if isinstance(data, dict):
-        result = data.copy()
-        for key, value in data.items():
-            if key in DEANNOTATE_KEYS:
-                del result[key]
-            elif isinstance(value, list):
-                for i, item in enumerate(value):
-                    value[i] = deannotate(item)
-            elif isinstance(value, dict):
-                result[key] = deannotate(value)
-        return result
-    return result
-
 
 class JinjaRule(AnsibleLintRule):
     """Rule that looks inside jinja2 templates."""
 
     id = "jinja"
     severity = "LOW"
     tags = ["formatting"]
@@ -220,14 +202,15 @@
     # pylint: disable=too-many-branches,too-many-statements,too-many-locals
     def check_whitespace(  # noqa: max-complexity: 13
         self, text: str, key: str, lintable: Lintable | None = None
     ) -> tuple[str, str, str]:
         """Check spacing inside given jinja2 template string.
 
         We aim to match Python Black formatting rules.
+        :raises NotImplementedError: On few cases where valid jinja is not valid Python.
 
         :returns: (string, string, string)  reformatted text, detailed error, error tag
         """
 
         def cook(value: str, implicit: bool = False) -> str:
             """Prepare an implicit string for jinja parsing when needed."""
             if not implicit:
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/key_order.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/key_order.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/key_order.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/key_order.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/latest.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/latest.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/latest.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/latest.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/literal_compare.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/literal_compare.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/literal_compare.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/literal_compare.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/loop_var_prefix.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/loop_var_prefix.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/loop_var_prefix.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/loop_var_prefix.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/meta_incorrect.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/meta_incorrect.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/meta_incorrect.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/meta_incorrect.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/meta_no_info.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/meta_no_info.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/meta_no_info.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/meta_no_info.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/meta_no_tags.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/meta_no_tags.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/meta_video_links.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/meta_video_links.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/meta_video_links.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/meta_video_links.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/name.py` & `ansible-lint-6.9.1/test/test_runner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,149 +1,159 @@
-"""Implementation of NameRule."""
+"""Tests for runner submodule."""
+# Copyright (c) 2013-2014 Will Thames <will@thames.id.au>
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+# THE SOFTWARE.
 from __future__ import annotations
 
-import re
-import sys
-from typing import TYPE_CHECKING, Any
+import os
+from typing import Any
 
-from ansiblelint.constants import LINE_NUMBER_KEY
-from ansiblelint.errors import MatchError
-from ansiblelint.rules import AnsibleLintRule
+import pytest
 
-if TYPE_CHECKING:
-    from ansiblelint.file_utils import Lintable
+from ansiblelint import formatters
+from ansiblelint.file_utils import Lintable, abspath
+from ansiblelint.rules import RulesCollection
+from ansiblelint.runner import Runner
+
+LOTS_OF_WARNINGS_PLAYBOOK = abspath(
+    "examples/playbooks/lots_of_warnings.yml", os.getcwd()
+)
+
+
+@pytest.mark.parametrize(
+    ("playbook", "exclude", "length"),
+    (
+        pytest.param("examples/playbooks/nomatchestest.yml", [], 0, id="nomatchestest"),
+        pytest.param("examples/playbooks/unicode.yml", [], 1, id="unicode"),
+        pytest.param(
+            LOTS_OF_WARNINGS_PLAYBOOK,
+            [LOTS_OF_WARNINGS_PLAYBOOK],
+            0,
+            id="lots_of_warnings",
+        ),
+        pytest.param("examples/playbooks/become.yml", [], 0, id="become"),
+        pytest.param(
+            "examples/playbooks/contains_secrets.yml", [], 0, id="contains_secrets"
+        ),
+    ),
+)
+def test_runner(
+    default_rules_collection: RulesCollection,
+    playbook: str,
+    exclude: list[str],
+    length: int,
+) -> None:
+    """Test that runner can go through any corner cases."""
+    runner = Runner(playbook, rules=default_rules_collection, exclude_paths=exclude)
+
+    matches = runner.run()
+
+    assert len(matches) == length
+
+
+def test_runner_exclude_paths(default_rules_collection: RulesCollection) -> None:
+    """Test that exclude paths do work."""
+    runner = Runner(
+        "examples/playbooks/example.yml",
+        rules=default_rules_collection,
+        exclude_paths=["examples/"],
+    )
+
+    matches = runner.run()
+    assert len(matches) == 0
+
+
+@pytest.mark.parametrize(("exclude_path"), ("**/playbooks/*.yml",))
+def test_runner_exclude_globs(
+    default_rules_collection: RulesCollection, exclude_path: str
+) -> None:
+    """Test that globs work."""
+    runner = Runner(
+        "examples/playbooks",
+        rules=default_rules_collection,
+        exclude_paths=[exclude_path],
+    )
+
+    matches = runner.run()
+    # we expect to find one error from the only .yaml file we have there.
+    assert len(matches) == 1
+
+
+@pytest.mark.parametrize(
+    ("formatter_cls"),
+    (
+        pytest.param(formatters.Formatter, id="Formatter-plain"),
+        pytest.param(formatters.ParseableFormatter, id="ParseableFormatter-colored"),
+        pytest.param(formatters.QuietFormatter, id="QuietFormatter-colored"),
+        pytest.param(formatters.Formatter, id="Formatter-colored"),
+    ),
+)
+def test_runner_unicode_format(
+    default_rules_collection: RulesCollection,
+    formatter_cls: type[formatters.BaseFormatter[Any]],
+) -> None:
+    """Check that all formatters are unicode-friendly."""
+    formatter = formatter_cls(os.getcwd(), display_relative_path=True)
+    runner = Runner(
+        Lintable("examples/playbooks/unicode.yml", kind="playbook"),
+        rules=default_rules_collection,
+    )
 
+    matches = runner.run()
 
-class NameRule(AnsibleLintRule):
-    """Rule for checking task and play names."""
+    formatter.format(matches[0])
 
-    id = "name"
-    description = (
-        "All tasks and plays should have a distinct name for readability "
-        "and for ``--start-at-task`` to work"
+
+@pytest.mark.parametrize("directory_name", ("test/", os.path.abspath("test")))
+def test_runner_with_directory(
+    default_rules_collection: RulesCollection, directory_name: str
+) -> None:
+    """Check that runner detects a directory as role."""
+    runner = Runner(directory_name, rules=default_rules_collection)
+
+    expected = Lintable(name=directory_name, kind="role")
+    assert expected in runner.lintables
+
+
+def test_files_not_scanned_twice(default_rules_collection: RulesCollection) -> None:
+    """Ensure that lintables aren't double-checked."""
+    checked_files: set[Lintable] = set()
+
+    filename = os.path.abspath("examples/playbooks/common-include-1.yml")
+    runner = Runner(
+        filename,
+        rules=default_rules_collection,
+        verbosity=0,
+        checked_files=checked_files,
+    )
+    run1 = runner.run()
+    assert len(runner.checked_files) == 2
+    assert len(run1) == 1
+
+    filename = os.path.abspath("examples/playbooks/common-include-2.yml")
+    runner = Runner(
+        filename,
+        rules=default_rules_collection,
+        verbosity=0,
+        checked_files=checked_files,
     )
-    severity = "MEDIUM"
-    tags = ["idiom"]
-    version_added = "v6.5.0 (last update)"
-    _re_templated_inside = re.compile(r".*\{\{.*\}\}(.+)$")
-
-    def matchplay(self, file: Lintable, data: dict[str, Any]) -> list[MatchError]:
-        """Return matches found for a specific play (entry in playbook)."""
-        results = []
-        if file.kind != "playbook":
-            return []
-        if "name" not in data:
-            return [
-                self.create_matcherror(
-                    message="All plays should be named.",
-                    linenumber=data[LINE_NUMBER_KEY],
-                    tag="name[play]",
-                    filename=file,
-                )
-            ]
-        results.extend(
-            self._check_name(
-                data["name"], lintable=file, linenumber=data[LINE_NUMBER_KEY]
-            )
-        )
-        return results
-
-    def matchtask(
-        self, task: dict[str, Any], file: Lintable | None = None
-    ) -> list[MatchError]:
-        results = []
-        name = task.get("name")
-        if not name:
-            results.append(
-                self.create_matcherror(
-                    message="All tasks should be named.",
-                    linenumber=task[LINE_NUMBER_KEY],
-                    tag="name[missing]",
-                    filename=file,
-                )
-            )
-        else:
-            results.extend(
-                self._check_name(name, lintable=file, linenumber=task[LINE_NUMBER_KEY])
-            )
-        return results
-
-    def _check_name(
-        self, name: str, lintable: Lintable | None, linenumber: int
-    ) -> list[MatchError]:
-        # This rules applies only to languages that do have uppercase and
-        # lowercase letter, so we ignore anything else. On Unicode isupper()
-        # is not necessarily the opposite of islower()
-        results = []
-        if name[0].isalpha() and name[0].islower() and not name[0].isupper():
-            results.append(
-                self.create_matcherror(
-                    message="All names should start with an uppercase letter.",
-                    linenumber=linenumber,
-                    tag="name[casing]",
-                    filename=lintable,
-                )
-            )
-        if self._re_templated_inside.match(name):
-            results.append(
-                self.create_matcherror(
-                    message="Jinja templates should only be at the end of 'name'",
-                    linenumber=linenumber,
-                    tag="name[template]",
-                    filename=lintable,
-                )
-            )
-        return results
-
-
-if "pytest" in sys.modules:  # noqa: C901
-
-    from ansiblelint.rules import RulesCollection
-    from ansiblelint.runner import Runner
-
-    def test_file_positive() -> None:
-        """Positive test for unnamed-task."""
-        collection = RulesCollection()
-        collection.register(NameRule())
-        success = "examples/playbooks/task-has-name-success.yml"
-        good_runner = Runner(success, rules=collection)
-        assert [] == good_runner.run()
-
-    def test_file_negative() -> None:
-        """Negative test for unnamed-task."""
-        collection = RulesCollection()
-        collection.register(NameRule())
-        failure = "examples/playbooks/task-has-name-failure.yml"
-        bad_runner = Runner(failure, rules=collection)
-        errs = bad_runner.run()
-        assert len(errs) == 5
-
-    def test_rule_name_lowercase() -> None:
-        """Negative test for a task that starts with lowercase."""
-        collection = RulesCollection()
-        collection.register(NameRule())
-        failure = "examples/playbooks/task-name-lowercase.yml"
-        bad_runner = Runner(failure, rules=collection)
-        errs = bad_runner.run()
-        assert len(errs) == 1
-        assert errs[0].tag == "name[casing]"
-        assert errs[0].rule.id == "name"
-
-    def test_name_play() -> None:
-        """Positive test for name[play]."""
-        collection = RulesCollection()
-        collection.register(NameRule())
-        success = "examples/playbooks/play-name-missing.yml"
-        errs = Runner(success, rules=collection).run()
-        assert len(errs) == 1
-        assert errs[0].tag == "name[play]"
-        assert errs[0].rule.id == "name"
-
-    def test_name_template() -> None:
-        """Negative test for name[templated]."""
-        collection = RulesCollection()
-        collection.register(NameRule())
-        failure = "examples/playbooks/name-templated.yml"
-        bad_runner = Runner(failure, rules=collection)
-        errs = bad_runner.run()
-        assert len(errs) == 1
-        assert errs[0].tag == "name[template]"
+    run2 = runner.run()
+    assert len(runner.checked_files) == 3
+    # this second run should return 0 because the included filed was already
+    # processed and added to checked_files, which acts like a bypass list.
+    assert len(run2) == 0
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_changed_when.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_changed_when.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_changed_when.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_changed_when.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_free_form.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_free_form.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_free_form.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_free_form.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_handler.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_handler.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_handler.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_handler.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_jinja_when.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_jinja_when.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_jinja_when.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_jinja_when.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_log_password.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_log_password.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_log_password.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_log_password.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_prompting.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_prompting.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_prompting.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_prompting.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_relative_paths.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_relative_paths.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_relative_paths.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_relative_paths.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_same_owner.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_same_owner.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_same_owner.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_same_owner.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_tabs.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_tabs.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/no_tabs.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/no_tabs.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/only_builtins.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/only_builtins.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/only_builtins.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/only_builtins.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 import sys
 from typing import Any
 
 from ansiblelint.config import options
 from ansiblelint.file_utils import Lintable
 from ansiblelint.rules import AnsibleLintRule
-
-# fqcn_builtins was added in 5.1.0 as FQCNBuiltinsRule, renamed to fqcn_builtins in 6.0.0
 from ansiblelint.rules.fqcn import builtins
 from ansiblelint.skip_utils import is_nested_task
 
 
 class OnlyBuiltinsRule(AnsibleLintRule):
     """Use only builtin actions."""
 
@@ -22,22 +20,26 @@
     tags = ["opt-in", "experimental"]
 
     def matchtask(
         self, task: dict[str, Any], file: Lintable | None = None
     ) -> bool | str:
         module = task["action"]["__ansible_module_original__"]
 
-        is_builtin = module.startswith("ansible.builtin.") or module in builtins
-
-        is_manually_allowed = any(
-            module.startswith(f"{prefix}.")
-            for prefix in options.only_builtins_allow_collections
+        allowed_collections = [
+            "ansible.builtin",
+            "ansible.legacy",
+        ] + options.only_builtins_allow_collections
+        allowed_modules = builtins + options.only_builtins_allow_modules
+
+        is_allowed = (
+            any(module.startswith(f"{prefix}.") for prefix in allowed_collections)
+            or module in allowed_modules
         )
 
-        return not is_builtin and not is_manually_allowed and not is_nested_task(task)
+        return not is_allowed and not is_nested_task(task)
 
 
 # testing code to be loaded only with pytest or when executed the rule file
 if "pytest" in sys.modules:
 
     # pylint: disable=ungrouped-imports
     import pytest
@@ -48,33 +50,35 @@
     SUCCESS_PLAY = """
 - hosts: localhost
   tasks:
   - name: A block
     block:
     - name: Shell (fqcn)
       ansible.builtin.shell: echo This rule should not get matched by the only-builtins rule
+    - name: Command with legacy FQCN
+      ansible.legacy.command: echo This rule should not get matched by the only-builtins rule
     """
 
     def test_only_builtins_fail() -> None:
         """Test rule matches."""
         result = run_ansible_lint(
             "--strict",
             "--warn-list=",
             "--enable-list",
             "only-builtins",
             "examples/playbooks/rule-only-builtins.yml",
         )
         assert result.returncode == VIOLATIONS_FOUND_RC
         assert "Failed" in result.stderr
-        assert "1 warning(s)" in result.stderr
+        assert "2 warning(s)" in result.stderr
         assert "only-builtins: Use only builtin actions" in result.stdout
 
-    def test_only_builtins_allow_collections() -> None:
+    def test_only_builtins_allow() -> None:
         """Test rule doesn't match."""
-        conf_path = "examples/playbooks/.ansible-lint-only-builtins-allow-collections"
+        conf_path = "examples/playbooks/.ansible-lint-only-builtins-allow"
         result = run_ansible_lint(
             f"--config-file={conf_path}",
             "--strict",
             "--warn-list=",
             "--enable-list",
             "only-builtins",
             "examples/playbooks/rule-only-builtins.yml",
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/package_latest.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/package_latest.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/package_latest.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/package_latest.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/partial_become.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/partial_become.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/partial_become.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/partial_become.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,19 +116,19 @@
     from ansiblelint.rules import RulesCollection  # pylint: disable=ungrouped-imports
     from ansiblelint.runner import Runner  # pylint: disable=ungrouped-imports
 
     def test_partial_become_positive() -> None:
         """Positive test for partial-become."""
         collection = RulesCollection()
         collection.register(BecomeUserWithoutBecomeRule())
-        success = "examples/playbooks/become-user-without-become-success.yml"
+        success = "examples/playbooks/rule-partial-become-without-become-pass.yml"
         good_runner = Runner(success, rules=collection)
         assert [] == good_runner.run()
 
     def test_partial_become_negative() -> None:
         """Negative test for partial-become."""
         collection = RulesCollection()
         collection.register(BecomeUserWithoutBecomeRule())
-        failure = "examples/playbooks/become-user-without-become-failure.yml"
+        failure = "examples/playbooks/rule-partial-become-without-become-fail.yml"
         bad_runner = Runner(failure, rules=collection)
         errs = bad_runner.run()
         assert len(errs) == 3
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/playbook_extension.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/playbook_extension.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/playbook_extension.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/playbook_extension.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/risky_file_permissions.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/risky_file_permissions.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/risky_file_permissions.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/risky_file_permissions.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/risky_shell_pipe.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/risky_shell_pipe.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/risky_shell_pipe.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/risky_shell_pipe.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/role_name.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/role_name.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/role_name.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/role_name.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/run_once.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/run_once.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/run_once.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/run_once.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/schema.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/schema.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,16 @@
 
 - `schema[ansible-lint-config]` validates [ansible-lint configuration](https://github.com/ansible/ansible-lint/blob/main/src/ansiblelint/schemas/ansible-lint-config.json)
 
 Maintained in the [ansible-navigator](https://github.com/ansible/ansible-navigator) project:
 
 - `schema[ansible-navigator]` validates [ansible-navigator configuration](https://github.com/ansible/ansible-navigator/blob/main/src/ansible_navigator/data/ansible-navigator.json)
 
-Maintained in the Ansible [schemas](https://github.com/ansible/schemas) project:
-
 - `schema[arg_specs]` validates [module argument specs](https://docs.ansible.com/ansible/latest/dev_guide/developing_program_flow_modules.html#argument-spec)
-- `schema[execution-environment]` validates [execution environments](https://docs.ansible.com/automation-controller/latest/html/userguide/execution_environments.html#ees)
+- `schema[execution-environment]` validates [execution environments](https://docs.ansible.com/automation-controller/latest/html/userguide/execution_environments.html)
 - `schema[galaxy]` validates [collection metadata](https://docs.ansible.com/ansible/latest/dev_guide/collections_galaxy_meta.html).
 - `schema[inventory]` validates [inventory files](https://docs.ansible.com/ansible/latest/user_guide/intro_inventory.html) that match `inventory/*.yml`.
 - `schema[meta-runtime]` validates [runtime information](https://docs.ansible.com/ansible/devel/dev_guide/developing_collections_structure.html#meta-directory-and-runtime-yml) that matches `meta/runtime.yml`
 - `schema[meta]` validates metadata for roles that match `meta/main.yml`. See [role-dependencies](https://docs.ansible.com/ansible/latest/user_guide/playbooks_reuse_roles.html#role-dependencies) or [role/metadata.py](https://github.com/ansible/ansible/blob/devel/lib/ansible/playbook/role/metadata.py#L79)) for details.
 - `schema[playbook]` validates Ansible playbooks.
 - `schema[requirements]` validates Ansible [requirements](https://docs.ansible.com/ansible/latest/galaxy/user_guide.html#install-multiple-collections-with-a-requirements-file) files that match `requirements.yml`.
 - `schema[tasks]` validates Ansible task files that match `tasks/**/*.yml`.
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/schema.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,14 @@
 
 DESCRIPTION_MD = """ Returned errors will not include exact line numbers, but they will mention
 the schema name being used as a tag, like ``schema[playbook]``,
 ``schema[tasks]``.
 
 This rule is not skippable and stops further processing of the file.
 
-Schema bugs should be reported towards [schemas](https://github.com/ansible/schemas) project instead of ansible-lint.
-
 If incorrect schema was picked, you might want to either:
 
 * move the file to standard location, so its file is detected correctly.
 * use ``kinds:`` option in linter config to help it pick correct file type.
 """
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/syntax_check.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/syntax_check.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/syntax_check.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/syntax_check.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/var_naming.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/var_naming.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/var_naming.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/var_naming.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/yaml.md` & `ansible-lint-6.9.1/src/ansiblelint/rules/yaml.md`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/rules/yaml_rule.py` & `ansible-lint-6.9.1/src/ansiblelint/rules/yaml_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/runner.py` & `ansible-lint-6.9.1/src/ansiblelint/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
                 try:
                     for child in ansiblelint.utils.find_children(lintable):
                         if self.is_excluded(child):
                             continue
                         self.lintables.add(child)
                         files.append(child)
                 except MatchError as exc:
-                    if not exc.filename:
+                    if not exc.filename:  # pragma: no branch
                         exc.filename = str(lintable.path)
                     exc.rule = LoadingFailureRule()
                     yield exc
                 except AttributeError:
                     yield MatchError(filename=lintable, rule=LoadingFailureRule())
                 visited.add(lintable)
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/__store__.json` & `ansible-lint-6.9.1/src/ansiblelint/schemas/__store__.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6346153846153846%*

 * *Differences: {"'arg_specs'": "{'url': "*

 * *                "'https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/arg_specs.json', "*

 * *                "delete: ['etag']}",*

 * * "'execution-environment'": "{'url': "*

 * *                            "'https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/execution-environment.json', "*

 * *                            "delete: ['etag']}",*

 * * "'galaxy'": "{'url': "*

 * *             "'https://raw.githubusercontent.com/ansible/ansible-lint/ […]*

```diff
@@ -3,47 +3,40 @@
         "url": "https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/ansible-lint-config.json"
     },
     "ansible-navigator-config": {
         "etag": "259a168c473dc88b5def7ea8c7ed28365e46a8abf894cd08fcd57613508e1f26",
         "url": "https://raw.githubusercontent.com/ansible/ansible-navigator/main/src/ansible_navigator/data/ansible-navigator.json"
     },
     "arg_specs": {
-        "etag": "cf3e180b9f9a1980ce491905db37bae4968be10bd0e45fb2096e0e360d4a4912",
-        "url": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-argument-specs.json"
+        "url": "https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/arg_specs.json"
     },
     "execution-environment": {
-        "etag": "b2c0e183aabbef8fd83e61e26af2fb1d9a2c8f6549599a24ebf7ccada4c11a81",
-        "url": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-ee.json"
+        "url": "https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/execution-environment.json"
     },
     "galaxy": {
-        "etag": "2bf1bc8df72c9063463daabddcb707e9ec6923633e4b66343237e39be102f63b",
-        "url": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-galaxy.json"
+        "url": "https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/galaxy.json"
     },
     "inventory": {
-        "etag": "4bf635a87d034c9316c441ab441ef63689059bf96ecd652339ee86200a707f0f",
-        "url": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-inventory.json"
+        "url": "https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/inventory.json"
     },
     "meta": {
-        "etag": "ffa1e3f48e1f3dbc2b6a0f18fd27676980bac4c94b39e6c072d55ee5ec27449e",
-        "url": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-meta.json"
+        "url": "https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/meta.json"
     },
     "meta-runtime": {
-        "etag": "21c8e4c37930a1c9b135101fcac6c4ef52cfbfe5a724d27612e7ec067cfc5a6a",
-        "url": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-meta-runtime.json"
+        "url": "https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/meta-runtime.json"
+    },
+    "molecule": {
+        "url": "https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/molecule.json"
     },
     "playbook": {
-        "etag": "3d3d803a7bba95bb159ad65c2b22c8961264308ef32c7e379d9d30ba3efeecae",
-        "url": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-playbook.json"
+        "url": "https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/playbook.json"
     },
     "requirements": {
-        "etag": "9805cd5cc2eb54de699fb9bc7a81db6321ab916d068bdd04e98ea58c8a7855e5",
-        "url": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-requirements.json"
+        "url": "https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/requirements.json"
     },
     "tasks": {
-        "etag": "68f5b5e1a568199617f777438c434006d9d6cfcd468a0f8b6bf8d1ce8d74af70",
-        "url": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-tasks.json"
+        "url": "https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/tasks.json"
     },
     "vars": {
-        "etag": "91faa0cc8adc0adf365a095efa948f8df21fcfc86ac742013b3429d5ea9a6092",
-        "url": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-vars.json"
+        "url": "https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/vars.json"
     }
 }
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/ansible-lint-config.json` & `ansible-lint-6.9.1/src/ansiblelint/schemas/ansible-lint-config.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9927884615384616%*

 * *Differences: {"'properties'": "{'only_builtins_allow_modules': OrderedDict([('items', OrderedDict([('type', "*

 * *                 "'string')])), ('title', 'Only Builtins Allow Modules'), ('type', 'array')]), "*

 * *                 "'task_name_prefix': OrderedDict([('default', '{stem} | '), ('title', 'Allow "*

 * *                 "custom prefix for task[prefix]'), ('type', 'string')]), 'var_naming_pattern': "*

 * *                 "OrderedDict([('default', '^[a-z_][a-z0-9_]*$'), ('title', 'Regex used to verify "*

 * *                 "variab […]*

```diff
@@ -76,14 +76,21 @@
         "only_builtins_allow_collections": {
             "items": {
                 "type": "string"
             },
             "title": "Only Builtins Allow Collections",
             "type": "array"
         },
+        "only_builtins_allow_modules": {
+            "items": {
+                "type": "string"
+            },
+            "title": "Only Builtins Allow Modules",
+            "type": "array"
+        },
         "parseable": {
             "default": true,
             "title": "Parseable",
             "type": "boolean"
         },
         "profile": {
             "enum": [
@@ -196,19 +203,29 @@
         "tags": {
             "items": {
                 "type": "string"
             },
             "title": "Tags",
             "type": "array"
         },
+        "task_name_prefix": {
+            "default": "{stem} | ",
+            "title": "Allow custom prefix for task[prefix]",
+            "type": "string"
+        },
         "use_default_rules": {
             "default": true,
             "title": "Use Default Rules",
             "type": "boolean"
         },
+        "var_naming_pattern": {
+            "default": "^[a-z_][a-z0-9_]*$",
+            "title": "Regex used to verify variable names",
+            "type": "string"
+        },
         "verbosity": {
             "default": 0,
             "title": "Verbosity",
             "type": "integer"
         },
         "warn_list": {
             "items": {
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/ansible-navigator-config.json` & `ansible-lint-6.9.1/src/ansiblelint/schemas/ansible-navigator-config.json`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/arg_specs.json` & `ansible-lint-6.9.1/src/ansiblelint/schemas/arg_specs.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/ansible/ansiblelint/main/src/ansiblelint/schemas/ansible-argument-specs.json'"}*

```diff
@@ -245,15 +245,15 @@
             },
             "removed_in_version": {
                 "type": "string"
             },
             "title": "Option"
         }
     },
-    "$id": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-argument-specs.json",
+    "$id": "https://raw.githubusercontent.com/ansible/ansiblelint/main/src/ansiblelint/schemas/ansible-argument-specs.json",
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": false,
     "examples": [
         "meta/argument_specs.yml"
     ],
     "markdownDescription": "Add entry point, usually `main`.\nSee [role-argument-validation](https://docs.ansible.com/ansible/latest/user_guide/playbooks_reuse_roles.html#role-argument-validation)",
     "properties": {
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/execution-environment.json` & `ansible-lint-6.9.1/src/ansiblelint/schemas/execution-environment.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/ansible-ee.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-ee.json",
+    "$id": "https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/ansible-ee.json",
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": false,
     "description": "See https://docs.ansible.com/automation-controller/latest/html/userguide/ee_reference.html",
     "examples": [
         "execution-environment.yml"
     ],
     "properties": {
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/galaxy.json` & `ansible-lint-6.9.1/src/ansiblelint/schemas/galaxy.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/ansible-galaxy.json'"}*

```diff
@@ -442,15 +442,15 @@
                 "xinetd",
                 "xpp",
                 "zlib-acknowledgement"
             ],
             "title": "SPDXLicenseEnum"
         }
     },
-    "$id": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-galaxy.json",
+    "$id": "https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/ansible-galaxy.json",
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": false,
     "examples": [
         "galaxy.yml"
     ],
     "properties": {
         "authors": {
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/inventory.json` & `ansible-lint-6.9.1/src/ansiblelint/schemas/inventory.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/ansible-inventory.json'"}*

```diff
@@ -59,15 +59,15 @@
                         "null"
                     ]
                 }
             },
             "type": "object"
         }
     },
-    "$id": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-inventory.json",
+    "$id": "https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/ansible-inventory.json",
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": true,
     "description": "Ansible Inventory Schema",
     "examples": [
         "inventory.yaml",
         "inventory.yml",
         "inventory/*.yml",
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/main.py` & `ansible-lint-6.9.1/src/ansiblelint/schemas/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,24 +23,25 @@
     """Refresh JSON schemas by downloading latest versions.
 
     Returns number of changed schemas.
     """
     age = int(time.time() - store_file.stat().st_mtime)
 
     # never check for updated schemas more than once a day
-    if min_age_seconds < age:
+    if min_age_seconds > age:
         return 0
     if not os.access(store_file, os.W_OK):
         _logger.debug(
             "Skipping schema update due to lack of writing rights on %s", store_file
         )
-        return 0
+        return -1
     _logger.debug("Checking for updated schemas...")
 
     changed = 0
+    # breakpoint()
     for kind, data in JSON_SCHEMAS.items():
         url = data["url"]
         if "#" in url:
             raise RuntimeError(
                 f"Schema URLs cannot contain # due to python-jsonschema limitation: {url}"
             )
         if url.startswith("https://raw.githubusercontent.com/ansible/ansible-lint"):
@@ -57,26 +58,21 @@
             request.add_header("If-None-Match", f'"{data.get("etag")}"')
         try:
             with urllib.request.urlopen(request) as response:
                 if response.status == 200:
                     content = response.read().decode("utf-8")
                     etag = response.headers["etag"].strip('"')
                     if etag != data.get("etag", ""):
-                        data["etag"] = etag
+                        JSON_SCHEMAS[kind]["etag"] = etag
                         changed += 1
-                        print(etag)
-                with open(f"{path}", "r+", encoding="utf-8") as f_out:
-                    _logger.info("Schema %s was updated", kind)
-                    if f_out.read() != content:
-                        f_out.seek(0)
+                    with open(f"{path}", "w", encoding="utf-8") as f_out:
+                        _logger.info("Schema %s was updated", kind)
                         f_out.write(content)
                         f_out.truncate()
-                    else:
-                        path.touch()
-                    changed += 1
+                        os.fsync(f_out.fileno())
         except urllib.error.HTTPError as exc:
             if exc.code == 304:
                 _logger.debug("Schema %s is not modified", url)
                 continue
             _logger.warning(
                 "Skipped schema refresh due to unexpected exception: %s", exc
             )
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/meta-runtime.json` & `ansible-lint-6.9.1/src/ansiblelint/schemas/meta-runtime.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/ansible-meta-runtime.json'"}*

```diff
@@ -34,15 +34,15 @@
                 "redirect": {
                     "type": "string"
                 }
             },
             "type": "object"
         }
     },
-    "$id": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-meta-runtime.json",
+    "$id": "https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/ansible-meta-runtime.json",
     "$schema": "http://json-schema.org/draft-07/schema",
     "additionalProperties": false,
     "description": "See https://docs.ansible.com/ansible/devel/dev_guide/developing_collections_structure.html#meta-directory",
     "examples": [
         "**/meta/runtime.yml"
     ],
     "properties": {
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/meta.json` & `ansible-lint-6.9.1/src/ansiblelint/schemas/meta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/meta.json'"}*

```diff
@@ -1475,15 +1475,15 @@
                     "type": "array"
                 }
             },
             "title": "vSpherePlatformModel",
             "type": "object"
         }
     },
-    "$id": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-meta.json",
+    "$id": "https://raw.githubusercontent.com/ansible/ansible-lint/main/src/ansiblelint/schemas/meta.json",
     "$schema": "http://json-schema.org/draft-07/schema",
     "examples": [
         "meta/main.yml"
     ],
     "properties": {
         "additionalProperties": false,
         "allow_duplicates": {
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/playbook.json` & `ansible-lint-6.9.1/src/ansiblelint/schemas/playbook.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9370584401472375%*

 * *Differences: {"'$defs'": "{'block': {'properties': {'diff': {'$ref': '#/$defs/templated-boolean', delete: "*

 * *            "['type']}}}, 'full-jinja': {'pattern': '^\\\\{\\\\{(.|[\\r\\n])*\\\\}\\\\}$'}, "*

 * *            "'play': {'properties': {'diff': {'$ref': '#/$defs/templated-boolean', delete: "*

 * *            "['type']}}}, 'play-role': {'properties': {'diff': {'$ref': "*

 * *            "'#/$defs/templated-boolean', delete: ['type']}}}, 'task': {'properties': {'diff': "*

 * *            "{'$ref': '#/$defs/templated-boolean', delete:  […]*

```diff
@@ -150,16 +150,16 @@
                     "type": "boolean"
                 },
                 "delegate_to": {
                     "title": "Delegate To",
                     "type": "string"
                 },
                 "diff": {
-                    "title": "Diff",
-                    "type": "boolean"
+                    "$ref": "#/$defs/templated-boolean",
+                    "title": "Diff"
                 },
                 "environment": {
                     "$ref": "#/$defs/environment"
                 },
                 "ignore_errors": {
                     "$ref": "#/$defs/ignore_errors"
                 },
@@ -255,15 +255,15 @@
                 {
                     "$ref": "#/$defs/full-jinja"
                 }
             ],
             "title": "Environment"
         },
         "full-jinja": {
-            "pattern": "^\\{\\{.*\\}\\}$",
+            "pattern": "^\\{\\{(.|[\r\n])*\\}\\}$",
             "type": "string"
         },
         "ignore_errors": {
             "$ref": "#/$defs/templated-boolean",
             "markdownDescription": "See [ignore_errors](https://docs.ansible.com/ansible/latest/user_guide/playbooks_error_handling.html#ignoring-failed-commands)",
             "title": "Ignore Errors"
         },
@@ -330,16 +330,16 @@
                     "type": "string"
                 },
                 "debugger": {
                     "title": "Debugger",
                     "type": "string"
                 },
                 "diff": {
-                    "title": "Diff",
-                    "type": "boolean"
+                    "$ref": "#/$defs/templated-boolean",
+                    "title": "Diff"
                 },
                 "environment": {
                     "$ref": "#/$defs/environment"
                 },
                 "fact_path": {
                     "title": "Fact Path",
                     "type": "string"
@@ -702,16 +702,16 @@
                     "type": "string"
                 },
                 "delegate_to": {
                     "title": "Delegate To",
                     "type": "string"
                 },
                 "diff": {
-                    "title": "Diff",
-                    "type": "boolean"
+                    "$ref": "#/$defs/templated-boolean",
+                    "title": "Diff"
                 },
                 "environment": {
                     "$ref": "#/$defs/environment"
                 },
                 "ignore_errors": {
                     "$ref": "#/$defs/ignore_errors"
                 },
@@ -911,16 +911,16 @@
                     "type": "boolean"
                 },
                 "delegate_to": {
                     "title": "Delegate To",
                     "type": "string"
                 },
                 "diff": {
-                    "title": "Diff",
-                    "type": "boolean"
+                    "$ref": "#/$defs/templated-boolean",
+                    "title": "Diff"
                 },
                 "environment": {
                     "$ref": "#/$defs/environment"
                 },
                 "failed_when": {
                     "$ref": "#/$defs/complex_conditional",
                     "title": "Failed When"
@@ -1210,15 +1210,15 @@
             "required": [
                 "name",
                 "prompt"
             ],
             "type": "object"
         }
     },
-    "$id": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-playbook.json",
+    "$id": "https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/playbook.json",
     "$schema": "http://json-schema.org/draft-07/schema",
     "examples": [
         "playbooks/*.yml",
         "playbooks/*.yaml"
     ],
     "items": {
         "oneOf": [
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/requirements.json` & `ansible-lint-6.9.1/src/ansiblelint/schemas/requirements.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/ansible-requirements.json'"}*

```diff
@@ -123,15 +123,15 @@
                     "type": "string"
                 }
             },
             "title": "Role",
             "type": "object"
         }
     },
-    "$id": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-requirements.json",
+    "$id": "https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/ansible-requirements.json",
     "$schema": "http://json-schema.org/draft-07/schema",
     "anyOf": [
         {
             "items": {
                 "anyOf": [
                     {
                         "$ref": "#/$defs/RoleModel"
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/tasks.json` & `ansible-lint-6.9.1/src/ansiblelint/schemas/tasks.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9368425575196409%*

 * *Differences: {"'$defs'": "{'block': {'properties': {'diff': {'$ref': '#/$defs/templated-boolean', delete: "*

 * *            "['type']}}}, 'full-jinja': {'pattern': '^\\\\{\\\\{(.|[\\r\\n])*\\\\}\\\\}$'}, "*

 * *            "'task': {'properties': {'diff': {'$ref': '#/$defs/templated-boolean', delete: "*

 * *            "['type']}}}}",*

 * * "'$id'": "'https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/tasks.json'"}*

```diff
@@ -102,16 +102,16 @@
                     "type": "boolean"
                 },
                 "delegate_to": {
                     "title": "Delegate To",
                     "type": "string"
                 },
                 "diff": {
-                    "title": "Diff",
-                    "type": "boolean"
+                    "$ref": "#/$defs/templated-boolean",
+                    "title": "Diff"
                 },
                 "environment": {
                     "$ref": "#/$defs/environment"
                 },
                 "ignore_errors": {
                     "$ref": "#/$defs/ignore_errors"
                 },
@@ -207,15 +207,15 @@
                 {
                     "$ref": "#/$defs/full-jinja"
                 }
             ],
             "title": "Environment"
         },
         "full-jinja": {
-            "pattern": "^\\{\\{.*\\}\\}$",
+            "pattern": "^\\{\\{(.|[\r\n])*\\}\\}$",
             "type": "string"
         },
         "ignore_errors": {
             "$ref": "#/$defs/templated-boolean",
             "markdownDescription": "See [ignore_errors](https://docs.ansible.com/ansible/latest/user_guide/playbooks_error_handling.html#ignoring-failed-commands)",
             "title": "Ignore Errors"
         },
@@ -363,16 +363,16 @@
                     "type": "boolean"
                 },
                 "delegate_to": {
                     "title": "Delegate To",
                     "type": "string"
                 },
                 "diff": {
-                    "title": "Diff",
-                    "type": "boolean"
+                    "$ref": "#/$defs/templated-boolean",
+                    "title": "Diff"
                 },
                 "environment": {
                     "$ref": "#/$defs/environment"
                 },
                 "failed_when": {
                     "$ref": "#/$defs/complex_conditional",
                     "title": "Failed When"
@@ -560,15 +560,15 @@
                 {
                     "$ref": "#/$defs/full-jinja",
                     "type": "string"
                 }
             ]
         }
     },
-    "$id": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-tasks.json",
+    "$id": "https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/tasks.json",
     "$schema": "http://json-schema.org/draft-07/schema",
     "examples": [
         "tasks/*.yml",
         "handlers/*.yml"
     ],
     "items": {
         "anyOf": [
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/schemas/vars.json` & `ansible-lint-6.9.1/src/ansiblelint/schemas/vars.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'$id'": "'https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/ansible-vars.json'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "$id": "https://raw.githubusercontent.com/ansible/schemas/main/f/ansible-vars.json",
+    "$id": "https://raw.githubusercontent.com/ansible-lint/main/src/ansiblelint/schemas/ansible-vars.json",
     "$schema": "http://json-schema.org/draft-07/schema",
     "anyOf": [
         {
             "additionalProperties": false,
             "patternProperties": {
                 "^(?!(False|None|True|and|any_errors_fatal|as|assert|async|await|become|become_exe|become_flags|become_method|become_user|break|check_mode|class|collections|connection|continue|debugger|def|del|diff|elif|else|environment|except|fact_path|finally|for|force_handlers|from|gather_facts|gather_subset|gather_timeout|global|handlers|hosts|if|ignore_errors|ignore_unreachable|import|in|is|lambda|max_fail_percentage|module_defaults|name|no_log|nonlocal|not|or|order|pass|port|post_tasks|pre_tasks|raise|remote_user|return|roles|run_once|serial|strategy|tags|tasks|throttle|timeout|try|vars|vars_files|vars_prompt|while|with|yield)$)[a-zA-Z_][\\w]*$": {}
             },
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/skip_utils.py` & `ansible-lint-6.9.1/src/ansiblelint/skip_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/stats.py` & `ansible-lint-6.9.1/src/ansiblelint/stats.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/testing/__init__.py` & `ansible-lint-6.9.1/src/ansiblelint/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/testing/fixtures.py` & `ansible-lint-6.9.1/src/ansiblelint/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/src/ansiblelint/text.py` & `ansible-lint-6.9.1/src/ansiblelint/text.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 def strip_ansi_escape(data: str | bytes) -> str:
     """Remove all ANSI escapes from string or bytes.
 
     If bytes is passed instead of string, it will be converted to string
     using UTF-8.
     """
-    if isinstance(data, bytes):
+    if isinstance(data, bytes):  # pragma: no branch
         data = data.decode("utf-8")
 
     return re.sub(r"\x1b[^m]*m", "", data)
 
 
 def toidentifier(text: str) -> str:
     """Convert unsafe chars to ones allowed in variables."""
     result = re.sub(r"[\s-]+", "_", text)
-    if not result.isidentifier:
+    if not result.isidentifier():
         raise RuntimeError(
             f"Unable to convert role name '{text}' to valid variable name."
         )
     return result
 
 
 # https://www.python.org/dev/peps/pep-0616/
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/transformer.py` & `ansible-lint-6.9.1/src/ansiblelint/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,14 @@
     def __init__(self, result: LintResult, options: Namespace):
         """Initialize a Transformer instance."""
         self.write_set = self.effective_write_set(options.write_list)
 
         self.matches: list[MatchError] = result.matches
         self.files: set[Lintable] = result.files
 
-        file: Lintable
-        # pylint: disable=undefined-variable
         lintables: dict[str, Lintable] = {file.filename: file for file in result.files}
         self.matches_per_file: dict[Lintable, list[MatchError]] = {
             file: [] for file in result.files
         }
 
         for match in self.matches:
             try:
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/utils.py` & `ansible-lint-6.9.1/src/ansiblelint/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,15 @@
     basedir: str, k: str, v: Any, parent_type: FileType
 ) -> list[Lintable]:
     # handle special case include_tasks: name=filename.yml
     if k in INCLUSION_ACTION_NAMES and isinstance(v, dict) and "file" in v:
         v = v["file"]
 
     # we cannot really parse any jinja2 in includes, so we ignore them
-    if "{{" in v:
+    if "{{" in v:  # pragma: no branch
         return []
 
     if "import_playbook" in k and COLLECTION_PLAY_RE.match(v):
         # Any import_playbooks from collections should be ignored as ansible
         # own syntax check will handle them.
         return []
 
@@ -398,15 +398,15 @@
 
     # Include the FQCN task names as this happens before normalize
     for task_handler_key in INCLUSION_ACTION_NAMES:
 
         with contextlib.suppress(KeyError):
 
             # ignore empty tasks
-            if not task_handler:
+            if not task_handler:  # pragma: no branch
                 continue
 
             file_name = task_handler[task_handler_key]
             if isinstance(file_name, Mapping) and file_name.get("file", None):
                 file_name = file_name["file"]
 
             f = path_dwim(basedir, file_name)
@@ -474,31 +474,31 @@
 
     for loc in get_app().runtime.config.default_roles_path:
         loc = os.path.expanduser(loc)
         possible_paths.append(path_dwim(loc, role))
 
     possible_paths.append(path_dwim(basedir, ""))
 
-    for path_option in possible_paths:
+    for path_option in possible_paths:  # pragma: no branch
         if os.path.isdir(path_option):
             role_path = path_option
             break
 
-    if role_path:
+    if role_path:  # pragma: no branch
         add_all_plugin_dirs(role_path)
 
     return role_path
 
 
 def _look_for_role_files(
     basedir: str, role: str, main: str | None = "main"
 ) -> list[Lintable]:
     # pylint: disable=unused-argument # main
     role_path = _rolepath(basedir, role)
-    if not role_path:
+    if not role_path:  # pragma: no branch
         return []
 
     results = []
 
     for kind in ["tasks", "meta", "handlers", "vars", "defaults"]:
         current_path = os.path.join(role_path, kind)
         for folder, _, files in os.walk(current_path):
@@ -876,15 +876,15 @@
     """Detect roles among lintables and adds them to the list."""
     for lintable in lintables:
         parts = lintable.path.parent.parts
         if "roles" in parts:
             role = lintable.path
             while role.parent.name != "roles" and role.name:
                 role = role.parent
-            if role.exists and not role.is_file():
+            if role.exists() and not role.is_file():
                 lintable = Lintable(role, kind="role")
                 if lintable not in lintables:
                     _logger.debug("Added role: %s", lintable)
                     lintables.append(lintable)
 
 
 def convert_to_boolean(value: Any) -> bool:
```

### Comparing `ansible-lint-6.9.0/src/ansiblelint/yaml_utils.py` & `ansible-lint-6.9.1/src/ansiblelint/yaml_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from ruamel.yaml.nodes import ScalarNode
 from ruamel.yaml.representer import RoundTripRepresenter
 from ruamel.yaml.scalarint import ScalarInt
 from ruamel.yaml.tokens import CommentToken
 from yamllint.config import YamlLintConfig
 
 from ansiblelint.constants import (
+    ANNOTATION_KEYS,
     NESTED_TASK_KEYS,
     PLAYBOOK_TASK_KEYWORDS,
     SKIPPED_RULES_KEY,
 )
 from ansiblelint.errors import MatchError
 from ansiblelint.file_utils import Lintable
 from ansiblelint.utils import get_action_tasks, normalize_task
@@ -65,14 +66,29 @@
   # and we are trying not to fight other linters.
   braces:
     min-spaces-inside: 0  # yamllint defaults to 0
     max-spaces-inside: 1  # yamllint defaults to 0
 """
 
 
+def deannotate(data: Any) -> Any:
+    """Remove our annotations like __file__ and __line__ and return a JSON serializable object."""
+    if isinstance(data, dict):
+        result = data.copy()
+        for key, value in data.items():
+            if key in ANNOTATION_KEYS:
+                del result[key]
+            else:
+                result[key] = deannotate(value)
+        return result
+    if isinstance(data, list):
+        return [deannotate(item) for item in data if item not in ANNOTATION_KEYS]
+    return data
+
+
 @functools.lru_cache(maxsize=1)
 def load_yamllint_config() -> YamlLintConfig:
     """Load our default yamllint config and any customized override file."""
     config = YamlLintConfig(content=YAMLLINT_CONFIG)
     # if we detect local yamllint config we use it but raise a warning
     # as this is likely to get out of sync with our internal config.
     for file in [
@@ -563,25 +579,25 @@
         )
         return super().expect_document_root()
 
     # NB: mypy does not support overriding attributes with properties yet:
     #     https://github.com/python/mypy/issues/4125
     #     To silence we have to ignore[override] both the @property and the method.
 
-    @property  # type: ignore[override]
+    @property
     def best_sequence_indent(self) -> int:
         """Return the configured sequence_indent or 2 for root level."""
         return 2 if self._is_root_level_sequence else self._sequence_indent
 
     @best_sequence_indent.setter
     def best_sequence_indent(self, value: int) -> None:
         """Configure how many columns to indent each sequence item (including the '-')."""
         self._sequence_indent = value
 
-    @property  # type: ignore[override]
+    @property
     def sequence_dash_offset(self) -> int:
         """Return the configured sequence_dash_offset or 0 for root level."""
         return 0 if self._is_root_level_sequence else self._sequence_dash_offset
 
     @sequence_dash_offset.setter
     def sequence_dash_offset(self, value: int) -> None:
         """Configure how many spaces to put before each sequence item's '-'."""
```

### Comparing `ansible-lint-6.9.0/test/conftest.py` & `ansible-lint-6.9.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/custom_rules/example_com/example_com_rule.py` & `ansible-lint-6.9.1/test/custom_rules/example_com/example_com_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/custom_rules/example_inc/custom_rule.py` & `ansible-lint-6.9.1/test/custom_rules/example_inc/custom_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/fixtures/formatting-after/fmt-1.yml` & `ansible-lint-6.9.1/test/fixtures/formatting-after/fmt-1.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/fixtures/formatting-before/fmt-1.yml` & `ansible-lint-6.9.1/test/fixtures/formatting-before/fmt-1.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/fixtures/formatting-before/fmt-3.yml` & `ansible-lint-6.9.1/test/fixtures/formatting-before/fmt-3.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/fixtures/formatting-prettier/fmt-1.yml` & `ansible-lint-6.9.1/test/fixtures/formatting-prettier/fmt-1.yml`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/fixtures/test_regenerate_formatting_fixtures.py` & `ansible-lint-6.9.1/test/fixtures/test_regenerate_formatting_fixtures.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/fixtures/raw_task.py` & `ansible-lint-6.9.1/test/rules/fixtures/raw_task.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_deprecated_module.py` & `ansible-lint-6.9.1/test/rules/test_deprecated_module.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_inline_env_var.py` & `ansible-lint-6.9.1/test/rules/test_inline_env_var.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_line_too_long.py` & `ansible-lint-6.9.1/test/rules/test_line_too_long.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_literal_compare.py` & `ansible-lint-6.9.1/test/rules/test_literal_compare.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_meta_change_from_default.py` & `ansible-lint-6.9.1/test/rules/test_meta_change_from_default.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_meta_no_info.py` & `ansible-lint-6.9.1/test/rules/test_meta_no_info.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_meta_video_links.py` & `ansible-lint-6.9.1/test/rules/test_meta_video_links.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_no_changed_when.py` & `ansible-lint-6.9.1/test/rules/test_no_changed_when.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_no_jinja_when.py` & `ansible-lint-6.9.1/test/rules/test_no_jinja_when.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_no_relative_paths.py` & `ansible-lint-6.9.1/test/rules/test_no_relative_paths.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_package_latest.py` & `ansible-lint-6.9.1/test/rules/test_package_latest.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_risky_shell_pipe.py` & `ansible-lint-6.9.1/test/rules/test_risky_shell_pipe.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_role_names.py` & `ansible-lint-6.9.1/test/rules/test_role_names.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_use_bare_variables.py` & `ansible-lint-6.9.1/test/rules/test_use_bare_variables.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/rules/test_use_handler_rather_than_when_changed.py` & `ansible-lint-6.9.1/test/rules/test_use_handler_rather_than_when_changed.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_ansiblelintrule.py` & `ansible-lint-6.9.1/test/test_ansiblelintrule.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_ansiblesyntax.py` & `ansible-lint-6.9.1/test/test_ansiblesyntax.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_boot.py` & `ansible-lint-6.9.1/test/test_boot.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_cli_role_paths.py` & `ansible-lint-6.9.1/test/test_cli_role_paths.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_commandline_invocations_same_as_config.py` & `ansible-lint-6.9.1/test/test_commandline_invocations_same_as_config.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_eco.py` & `ansible-lint-6.9.1/test/test_eco.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     # consistent results regardless on its location.
     for step in ["before", "after"]:
 
         args = ["-f", "pep8"]
         executable = (
             "ansible-lint"
             if step == "after"
-            else f"{pathlib.Path(__file__).parent.parent}/.tox/eco-main/bin/ansible-lint"
+            else f"{pathlib.Path(__file__).parent.parent}/.tox/venv/bin/ansible-lint"
         )
         result = run_ansible_lint(
             *args,
             executable=executable,
             cwd=f"{cache_dir}/{repo}",
         )
```

### Comparing `ansible-lint-6.9.0/test/test_examples.py` & `ansible-lint-6.9.1/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_file_path_evaluation.py` & `ansible-lint-6.9.1/test/test_file_path_evaluation.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,36 +20,36 @@
             - name: From main import task 1
               ansible.builtin.import_tasks: tasks/task_1.yml
         """
     ),
     "tasks/task_1.yml": textwrap.dedent(
         """\
         ---
-        - name: From task 1 import task 2
+        - name: task_1 | From task 1 import task 2
           ansible.builtin.import_tasks: tasks/task_2.yml
         """
     ),
     "tasks/task_2.yml": textwrap.dedent(
         """\
         ---
-        - name: From task 2 import subtask 1
+        - name: task_2 | From task 2 import subtask 1
           ansible.builtin.import_tasks: tasks/subtasks/subtask_1.yml
         """
     ),
     "tasks/subtasks/subtask_1.yml": textwrap.dedent(
         """\
         ---
-        - name: From subtask 1 import subtask 2
+        - name: subtask_1 | From subtask 1 import subtask 2
           ansible.builtin.import_tasks: tasks/subtasks/subtask_2.yml
         """
     ),
     "tasks/subtasks/subtask_2.yml": textwrap.dedent(
         """\
         ---
-        - name: From subtask 2 do something
+        - name: subtask_2 | From subtask 2 do something
           debug:  # <-- expected to raise fqcn[action-core]
             msg: |
               Something...
         """
     ),
 }
 
@@ -64,36 +64,36 @@
             - name: From main import task 1
               ansible.builtin.include_tasks: tasks/task_1.yml
         """
     ),
     "tasks/task_1.yml": textwrap.dedent(
         """\
         ---
-        - name: From task 1 import task 2
+        - name: task_1 | From task 1 import task 2
           ansible.builtin.include_tasks: tasks/task_2.yml
         """
     ),
     "tasks/task_2.yml": textwrap.dedent(
         """\
         ---
-        - name: From task 2 import subtask 1
+        - name: task_2 | From task 2 import subtask 1
           ansible.builtin.include_tasks: tasks/subtasks/subtask_1.yml
         """
     ),
     "tasks/subtasks/subtask_1.yml": textwrap.dedent(
         """\
         ---
-        - name: From subtask 1 import subtask 2
+        - name: subtask_1 | From subtask 1 import subtask 2
           ansible.builtin.include_tasks: tasks/subtasks/subtask_2.yml
         """
     ),
     "tasks/subtasks/subtask_2.yml": textwrap.dedent(
         """\
         ---
-        - name: From subtask 2 do something
+        - name: subtask_2 | From subtask 2 do something
           debug:  # <-- expected to raise fqcn[action-core]
             msg: |
               Something...
         """
     ),
 }
```

### Comparing `ansible-lint-6.9.0/test/test_file_utils.py` & `ansible-lint-6.9.1/test/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_formatter.py` & `ansible-lint-6.9.1/test/test_formatter.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_formatter_base.py` & `ansible-lint-6.9.1/test/test_formatter_base.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_formatter_json.py` & `ansible-lint-6.9.1/test/test_formatter_json.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_formatter_sarif.py` & `ansible-lint-6.9.1/test/test_formatter_sarif.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_import_include_role.py` & `ansible-lint-6.9.1/test/test_import_include_role.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_import_playbook.py` & `ansible-lint-6.9.1/test/test_import_playbook.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_import_tasks.py` & `ansible-lint-6.9.1/test/test_import_tasks.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_include_miss_file_with_role.py` & `ansible-lint-6.9.1/test/test_include_miss_file_with_role.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_lint_rule.py` & `ansible-lint-6.9.1/test/test_lint_rule.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_list_rules.py` & `ansible-lint-6.9.1/test/test_list_rules.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_load_failure.py` & `ansible-lint-6.9.1/test/test_load_failure.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_main.py` & `ansible-lint-6.9.1/test/test_main.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_matcherrror.py` & `ansible-lint-6.9.1/test/test_matcherrror.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_profiles.py` & `ansible-lint-6.9.1/test/test_profiles.py`

 * *Files 26% similar despite different names*

```diff
@@ -34,8 +34,11 @@
     result = subprocess.run(cmd, check=False).returncode
     assert result == 0
 
     out, err = capfd.readouterr()
 
     # Confirmation that it runs in auto-detect mode
     assert "command-instead-of-module" in out
-    assert err == ""
+    if sys.version_info < (3, 9):
+        assert "ansible-lint is no longer tested" in err
+    else:
+        assert err == ""
```

### Comparing `ansible-lint-6.9.0/test/test_progressive.py` & `ansible-lint-6.9.1/test/test_progressive.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_rules_collection.py` & `ansible-lint-6.9.1/test/test_rules_collection.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_skip_import_playbook.py` & `ansible-lint-6.9.1/test/test_skip_import_playbook.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_skip_inside_yaml.py` & `ansible-lint-6.9.1/test/test_skip_inside_yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_skip_playbook_items.py` & `ansible-lint-6.9.1/test/test_skip_playbook_items.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_skiputils.py` & `ansible-lint-6.9.1/test/test_skiputils.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_strict.py` & `ansible-lint-6.9.1/test/test_strict.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_task_includes.py` & `ansible-lint-6.9.1/test/test_task_includes.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,11 +36,12 @@
     default_rules_collection: RulesCollection,
     filename: str,
     file_count: int,
     match_count: int,
 ) -> None:
     """Check if number of loaded files is correct."""
     lintable = Lintable(filename)
+    default_rules_collection.options.enable_list = ["name[prefix]"]
     runner = Runner(lintable, rules=default_rules_collection)
     result = runner.run()
     assert len(runner.lintables) == file_count
     assert len(result) == match_count
```

### Comparing `ansible-lint-6.9.0/test/test_transform_mixin.py` & `ansible-lint-6.9.1/test/test_transform_mixin.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_transformer.py` & `ansible-lint-6.9.1/test/test_transformer.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_utils.py` & `ansible-lint-6.9.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_verbosity.py` & `ansible-lint-6.9.1/test/test_verbosity.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_with_skip_tagid.py` & `ansible-lint-6.9.1/test/test_with_skip_tagid.py`

 * *Files identical despite different names*

### Comparing `ansible-lint-6.9.0/test/test_yaml_utils.py` & `ansible-lint-6.9.1/test/test_yaml_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -329,93 +329,93 @@
         pytest.param(
             "examples/playbooks/become.yml",
             100,
             [0],
             id="1_play_playbook-line_after_eof",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             1,
             [],
             id="4_play_playbook-line_before_play_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             2,
             [0],
             id="4_play_playbook-first_line_in_play_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             5,
             [0],
             id="4_play_playbook-middle_line_in_play_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             9,
             [0],
             id="4_play_playbook-last_line_in_play_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             10,
             [1],
             id="4_play_playbook-first_line_in_play_2",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             14,
             [1],
             id="4_play_playbook-middle_line_in_play_2",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             18,
             [1],
             id="4_play_playbook-last_line_in_play_2",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             19,
             [2],
             id="4_play_playbook-first_line_in_play_3",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             23,
             [2],
             id="4_play_playbook-middle_line_in_play_3",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             27,
             [2],
             id="4_play_playbook-last_line_in_play_3",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             28,
             [3],
             id="4_play_playbook-first_line_in_play_4",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             31,
             [3],
             id="4_play_playbook-middle_line_in_play_4",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             35,
             [3],
             id="4_play_playbook-last_line_in_play_4",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             100,
             [3],
             id="4_play_playbook-line_after_eof",
         ),
         pytest.param(
             "examples/playbooks/playbook-parent.yml",
             1,
@@ -548,117 +548,117 @@
         pytest.param(
             "examples/playbooks/become.yml",
             100,
             [0, "tasks", 0],
             id="1_task_playbook-line_after_eof_without_anything_after_task",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             1,
             [],
             id="4_play_playbook-play_1_line_before_tasks",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             7,
             [0, "tasks", 0],
             id="4_play_playbook-play_1_first_line_task_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             9,
             [0, "tasks", 0],
             id="4_play_playbook-play_1_last_line_task_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             10,
             [],
             id="4_play_playbook-play_2_line_before_tasks",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             12,
             [],
             id="4_play_playbook-play_2_line_before_tasks",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             13,
             [1, "tasks", 0],
             id="4_play_playbook-play_2_first_line_task_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             18,
             [1, "tasks", 0],
             id="4_play_playbook-play_2_middle_line_task_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             18,
             [1, "tasks", 0],
             id="4_play_playbook-play_2_last_line_task_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             19,
             [],
             id="4_play_playbook-play_3_line_before_tasks",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             22,
             [],
             id="4_play_playbook-play_3_line_before_tasks",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             23,
             [2, "tasks", 0],
             id="4_play_playbook-play_3_first_line_task_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             25,
             [2, "tasks", 0],
             id="4_play_playbook-play_3_middle_line_task_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             27,
             [2, "tasks", 0],
             id="4_play_playbook-play_3_last_line_task_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             28,
             [],
             id="4_play_playbook-play_4_line_before_tasks",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             31,
             [],
             id="4_play_playbook-play_4_line_before_tasks",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             32,
             [3, "tasks", 0],
             id="4_play_playbook-play_4_first_line_task_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             33,
             [3, "tasks", 0],
             id="4_play_playbook-play_4_middle_line_task_1",
         ),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             35,
             [3, "tasks", 0],
             id="4_play_playbook-play_4_last_line_task_1",
         ),
         # playbook with multiple tasks + tasks blocks in a play
         pytest.param(
             # must have at least one key after one of the tasks blocks
@@ -846,15 +846,15 @@
 
 
 @pytest.mark.parametrize(
     ("file_path", "line_number"),
     (
         pytest.param("examples/playbooks/become.yml", 0, id="1_play_playbook"),
         pytest.param(
-            "examples/playbooks/become-user-without-become-success.yml",
+            "examples/playbooks/rule-partial-become-without-become-pass.yml",
             0,
             id="4_play_playbook",
         ),
         pytest.param("examples/playbooks/playbook-parent.yml", 0, id="import_playbook"),
         pytest.param("examples/playbooks/become.yml", 0, id="1_task_playbook"),
     ),
 )
@@ -880,7 +880,27 @@
     ruamel_data: CommentedMap | CommentedSeq,
 ) -> None:
     """Ensure ``get_task_to_play`` raises ValueError for line_number < 1."""
     with pytest.raises(
         ValueError, match=f"expected line_number >= 1, got {line_number}"
     ):
         ansiblelint.yaml_utils.get_path_to_task(lintable, line_number, ruamel_data)
+
+
+@pytest.mark.parametrize(
+    ("before", "after"),
+    (
+        pytest.param(None, None, id="1"),
+        pytest.param(1, 1, id="2"),
+        pytest.param({}, {}, id="3"),
+        pytest.param({"__file__": 1}, {}, id="simple"),
+        pytest.param({"foo": {"__file__": 1}}, {"foo": {}}, id="nested"),
+        pytest.param([{"foo": {"__file__": 1}}], [{"foo": {}}], id="nested-in-lint"),
+        pytest.param({"foo": [{"__file__": 1}]}, {"foo": [{}]}, id="nested-in-lint"),
+    ),
+)
+def test_deannotate(
+    before: Any,
+    after: Any,
+) -> None:
+    """Ensure deannotate works as intended."""
+    assert ansiblelint.yaml_utils.deannotate(before) == after
```

### Comparing `ansible-lint-6.9.0/tools/test-setup.sh` & `ansible-lint-6.9.1/tools/test-setup.sh`

 * *Files 15% similar despite different names*

```diff
@@ -17,20 +17,13 @@
     # avoid outdated ansible and pipx
     sudo apt-get remove -y ansible pipx || true
     # cspell:disable-next-line
     sudo apt-get install -y --no-install-recommends -o=Dpkg::Use-Pty=0 \
         gcc git python3-venv python3-pip python3-dev libyaml-dev
     # Some of these might be needed for compiling packages that do not yet
     # a binary for current platform, like pyyaml on py311
-    pip3 install -v --no-binary :all: --user pyyaml
+    # pip3 install -v --no-binary :all: --user pyyaml
 fi
 
-which pipx || python3 -m pip install --user pipx
-which -a pipx
-which pre-commit || pipx install pre-commit
-which tox || pipx install tox
-
 # Log some useful info in case of unexpected failures:
 uname
 python3 --version
-tox --version
-pre-commit --version
```

### Comparing `ansible-lint-6.9.0/tox.ini` & `ansible-lint-6.9.1/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # spell-checker:ignore linkcheck basepython changedir envdir envlist envname envsitepackagesdir passenv setenv testenv toxinidir toxworkdir usedevelop doctrees envpython posargs
 [tox]
-minversion = 3.16.1
+minversion = 4.0.0rc1
 envlist =
   lint
-  packaging
+  pkg
+  hook
   docs
+  schemas
   py
   py-devel
+  eco
 isolated_build = true
-requires =
-  setuptools >= 41.4.0
-  pip >= 19.3.0
-  # tox-extra ensure non-zero exit code if git reports dirty after test run
-  tox-extra >= 0.3.0
 skip_missing_interpreters = True
 
 [testenv]
 description =
   Run the tests under {basepython} and
   devel: ansible devel branch
 deps =
@@ -39,21 +37,21 @@
 passenv =
   CURL_CA_BUNDLE  # https proxies, https://github.com/tox-dev/tox/issues/1437
   FORCE_COLOR
   HOME
   NO_COLOR
   PYTEST_*  # allows developer to define their own preferences
   PYTEST_REQPASS  # needed for CI
+  PYTHON*  # PYTHONPYCACHEPREFIX, PYTHONIOENCODING, PYTHONBREAKPOINT,...
   PY_COLORS
   RTD_TOKEN
   REQUESTS_CA_BUNDLE  # https proxies
   SSL_CERT_FILE  # https proxies
   LANG
-  LC_ALL
-  LC_CTYPE
+  LC_*
 # recreate = True
 setenv =
   # Avoid runtime warning that might affect our devel testing
   devel: ANSIBLE_DEVEL_WARNING = false
   COVERAGE_FILE = {env:COVERAGE_FILE:{toxworkdir}/.coverage.{envname}}
   COVERAGE_PROCESS_START={toxinidir}/pyproject.toml
   PIP_CONSTRAINT = {toxinidir}/requirements.txt
@@ -62,74 +60,70 @@
   PRE_COMMIT_COLOR = always
   FORCE_COLOR = 1
 allowlist_externals =
   git
   sh
   tox
   rm
+  pwd
 # both options needed to workaround https://github.com/tox-dev/tox/issues/2197
 usedevelop = false
 skip_install = true
 
 [testenv:lint]
 description = Run all linters
 # pip compile includes python version in output constraints, so we want to
 # be sure that version does not change randomly.
 basepython = python3.9
 deps =
   pre-commit>=2.6.0
-  pip-tools>=6.8.0
   setuptools>=51.1.1
   pytest>=7.2.0  # to updated schemas
 skip_install = true
 commands =
   {envpython} -m pre_commit run --all-files --show-diff-on-failure {posargs:}
-  # manual hook as they are unlikely to work outside tox
-  {envpython} -m pre_commit run --all-files --show-diff-on-failure --hook-stage manual pip-compile
-
 passenv =
   {[testenv]passenv}
   PRE_COMMIT_HOME
 setenv =
   {[testenv]setenv}
   # avoid messing pre-commit with out own constraints
   PIP_CONSTRAINT=
 
-[testenv:validate-hook]
+[testenv:hook]
 description = Validate pre-commit hook definition
 deps = pre-commit
-changedir = {toxworkdir}/x
 commands =
-  git init --initial-branch=main
-  python3 -m pre_commit try-repo -v {toxinidir} ansible-lint
+  sh -c "mkdir -p .tox/x && cd .tox/x && git init && python3 -m pre_commit try-repo -v {toxinidir} ansible-lint"
 setenv =
-  PIP_CONSTRAINT = /dev/null
+  PIP_CONSTRAINT=/dev/null
 
 [testenv:deps]
 description = Bump all test dependencies
 # we reuse the lint environment
 envdir = {toxworkdir}/lint
 skip_install = true
 basepython = python3.9
 deps =
   {[testenv:lint]deps}
 setenv =
   # without his upgrade would likely not do anything
   PIP_CONSTRAINT = /dev/null
 commands =
+  pre-commit run --all-files --show-diff-on-failure --hook-stage manual up
   pre-commit run --all-files --show-diff-on-failure --hook-stage manual schemas
-  pre-commit run --all-files --show-diff-on-failure --hook-stage manual pip-compile-upgrade
   # Update pre-commit hooks
   pre-commit autoupdate
+  # Update npm deps
+  bash -c "cd src/schemas && npm run deps"
   # We fail if files are modified at the end
   git diff --exit-code
 
 [testenv:docs]
 description = Builds docs
-basepython = python3
 deps =
   --editable .[docs,test]
 setenv =
   PIP_CONSTRAINT = {toxinidir}/requirements.txt
 commands =
   # regenerate docs for rules
   sh -c "cd {toxinidir} && ansible-lint -L -f docs"
@@ -168,67 +162,74 @@
 description = Update documentation redirections for readthedocs
 deps =
   readthedocs-cli
 commands =
   # This assumes you loaded RTD_TOKEN in your environment
   rtd projects ansible-lint redirects sync -f docs/redirects.yml --wet-run
 
+[testenv:schemas]
+description = Rebuild and test JSON Schemas
+deps =
+  check-jsonschema
+skip_install = true
+changedir = test/schemas
+commands_pre =
+  npm install
+commands =
+  npm test
+allowlist_externals =
+  npm
+
 [testenv:eco]
 description = Perform ecosystem impact (downstream testing) https://github.com/ansible/ansible-lint/discussions/1403
 skip_install = true
 deps =
   {[testenv]deps}
 commands =
-  # installs ansible-lint@main in separated venv, to be used as reference
-  tox --notest -qq -e eco-main
+  python -m venv .tox/venv
+  .tox/venv/bin/pip install -q git+https://github.com/ansible/ansible-lint@main
   pytest -n auto --durations=3 -m eco
+allowlist_externals =
+  .tox/venv/bin/pip
+setenv =
+  PYTEST_REQPASS=9
 
-[testenv:eco-main]
-# that is used by eco to install @main version and produce reference eco
-# results, ones that we will compare with current change.
-skip_install = true
-deps =
-  ansible-lint @ git+https://github.com/ansible/ansible-lint@main
-commands =
-  ansible-lint --version
-
-[testenv:packaging]
-basepython = python3
+[testenv:pkg]
 description =
   Build package, verify metadata, install package and assert behavior when ansible is missing.
 deps =
-  build >= 0.7.0, < 0.8.0
-  twine
+  build >= 0.9.0
+  twine >= 4.0.1
 skip_install = true
 # Ref: https://twitter.com/di_codes/status/1044358639081975813
 commands =
   # build wheel and sdist using PEP-517
   {envpython} -c 'import os.path, shutil, sys; \
   dist_dir = os.path.join("{toxinidir}", "dist"); \
   os.path.isdir(dist_dir) or sys.exit(0); \
   print("Removing \{!s\} contents...".format(dist_dir), file=sys.stderr); \
   shutil.rmtree(dist_dir)'
-  {envpython} -m build \
-    --outdir {toxinidir}/dist/ \
-    {toxinidir}
+  {envpython} -m build --outdir {toxinidir}/dist/ {toxinidir}
   # Validate metadata using twine
   twine check --strict {toxinidir}/dist/*
   # Install the wheel
   sh -c "python3 -m pip install {toxinidir}/dist/*.whl"
+  # Uninstall it
+  python3 -m pip uninstall -y ansible-lint
 
 [testenv:clean]
 skip_install = true
 deps =
 commands =
   find . -type f -name '*.py[co]' -delete -o -type d -name __pycache__
   rm -rf .mypy_cache
 
 [testenv:coverage]
 description = Combines and displays coverage results
 commands =
-  sh -c "coverage combine .tox/.coverage.*"
+  sh -c "coverage combine -q .tox/.coverage.*"
   # needed by codecov github actions:
   coverage xml
   # just for humans running it:
-  coverage report --skip-covered --fail-under=88
+  coverage report
 deps =
   coverage[toml]
```

