# Comparing `tmp/ros2_easy_test-0.1.0.tar.gz` & `tmp/ros2_easy_test-0.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ros2_easy_test-0.1.0.tar", last modified: Tue Apr 11 21:40:54 2023, max compression
+gzip compressed data, was "ros2_easy_test-0.2.0.post1.tar", last modified: Sun May 21 16:21:28 2023, max compression
```

## Comparing `ros2_easy_test-0.1.0.tar` & `ros2_easy_test-0.2.0.post1.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.091895 ros2_easy_test-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.083895 ros2_easy_test-0.1.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.083895 ros2_easy_test-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.083895 ros2_easy_test-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/.github/workflows/python-package.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/.github/workflows/python-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.083895 ros2_easy_test-0.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-04-11 21:40:54.091895 ros2_easy_test-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.083895 ros2_easy_test-0.1.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.087895 ros2_easy_test-0.1.0/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/doc/source/decorators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/doc/source/design_and_limits.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/doc/source/env.rst
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.087895 ros2_easy_test-0.1.0/ros2_easy_test/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/ros2_easy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16332 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/ros2_easy_test/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/ros2_easy_test/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/ros2_easy_test/launch_file.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/ros2_easy_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.087895 ros2_easy_test-0.1.0/ros2_easy_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-04-11 21:40:54.000000 ros2_easy_test-0.1.0/ros2_easy_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-11 21:40:54.000000 ros2_easy_test-0.1.0/ros2_easy_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:40:54.000000 ros2_easy_test-0.1.0/ros2_easy_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-11 21:40:54.000000 ros2_easy_test-0.1.0/ros2_easy_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 21:40:54.000000 ros2_easy_test-0.1.0/ros2_easy_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 21:40:54.091895 ros2_easy_test-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.087895 ros2_easy_test-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.087895 ros2_easy_test-0.1.0/tests/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/demo/fixture_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/demo/hypothesis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/demo/reuse_decorator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.091895 ros2_easy_test-0.1.0/tests/example_launch_files/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/example_launch_files/adder.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/example_launch_files/echo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/example_launch_files/raise_in_init.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/example_launch_files/raise_in_timer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/example_launch_files/raise_on_request.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/example_launch_files/talker.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/example_launch_files/talker.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:40:54.091895 ros2_easy_test-0.1.0/tests/example_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/example_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/example_nodes/failing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/example_nodes/run_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/example_nodes/well_behaved.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/test_env_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/test_failing_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-04-11 21:40:41.000000 ros2_easy_test-0.1.0/tests/test_interactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:28.761924 ros2_easy_test-0.2.0.post1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:28.753924 ros2_easy_test-0.2.0.post1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:28.753924 ros2_easy_test-0.2.0.post1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:28.753924 ros2_easy_test-0.2.0.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/.github/workflows/python-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/.github/workflows/python-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:28.753924 ros2_easy_test-0.2.0.post1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-21 16:21:28.757924 ros2_easy_test-0.2.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:28.753924 ros2_easy_test-0.2.0.post1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:28.753924 ros2_easy_test-0.2.0.post1/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/doc/source/decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/doc/source/design_and_limits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/doc/source/env.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:28.757924 ros2_easy_test-0.2.0.post1/ros2_easy_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/ros2_easy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18441 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/ros2_easy_test/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/ros2_easy_test/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/ros2_easy_test/launch_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/ros2_easy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:28.757924 ros2_easy_test-0.2.0.post1/ros2_easy_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-21 16:21:28.000000 ros2_easy_test-0.2.0.post1/ros2_easy_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-21 16:21:28.000000 ros2_easy_test-0.2.0.post1/ros2_easy_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 16:21:28.000000 ros2_easy_test-0.2.0.post1/ros2_easy_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-21 16:21:28.000000 ros2_easy_test-0.2.0.post1/ros2_easy_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-21 16:21:28.000000 ros2_easy_test-0.2.0.post1/ros2_easy_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 16:21:28.761924 ros2_easy_test-0.2.0.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:28.757924 ros2_easy_test-0.2.0.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:28.757924 ros2_easy_test-0.2.0.post1/tests/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/demo/coroutine_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/demo/fixture_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/demo/hypothesis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/demo/reuse_decorator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:28.757924 ros2_easy_test-0.2.0.post1/tests/example_launch_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/example_launch_files/adder.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/example_launch_files/echo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/example_launch_files/raise_in_init.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/example_launch_files/raise_in_timer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/example_launch_files/raise_on_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/example_launch_files/talker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/example_launch_files/talker.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 16:21:28.757924 ros2_easy_test-0.2.0.post1/tests/example_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/example_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/example_nodes/failing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/example_nodes/run_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/example_nodes/well_behaved.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/test_env_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/test_failing_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/test_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-21 16:21:14.000000 ros2_easy_test-0.2.0.post1/tests/test_timeouts.py
```

### Comparing `ros2_easy_test-0.1.0/.github/workflows/python-package.yaml` & `ros2_easy_test-0.2.0.post1/.github/workflows/python-package.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -22,25 +22,34 @@
       run:
         shell: bash
     steps:
       - 
         name: Checkout repository
         uses: actions/checkout@v3
       -
-        name: Install dependencies and the pakage
+        name: Install dependencies and the package
         run: |
           apt-get update -q && apt-get install -qy python3-pip python-is-python3 ros-$ROS_DISTRO-example-interfaces
           pip install --upgrade pip setuptools
           python -m pip install -e '.[dev]'
       -
         name: Format (with black)
         run: |
           black --check .
       -
         name: Lint (with ruff)
         run: |
           ruff check .
       -
+        name: Type check main code (with mypy)
+        run: |
+          mypy ros2_easy_test
+      -
+        name: Type check tests (with mypy)
+        continue-on-error: true  # We do not want to fail the build if the type checker fails on the tests
+        run: |
+          mypy tests
+      -
         name: Testing (with pytest)
         run: |
           source /opt/ros/$ROS_DISTRO/setup.bash  # Activate ROS
           python -m pytest
```

### Comparing `ros2_easy_test-0.1.0/.github/workflows/python-release.yaml` & `ros2_easy_test-0.2.0.post1/.github/workflows/python-release.yaml`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/.gitignore` & `ros2_easy_test-0.2.0.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/Dockerfile` & `ros2_easy_test-0.2.0.post1/Dockerfile`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/LICENSE` & `ros2_easy_test-0.2.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/PKG-INFO` & `ros2_easy_test-0.2.0.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros2_easy_test
-Version: 0.1.0
+Version: 0.2.0.post1
 Summary: A Python test framework for ROS2 allowing simple and expressive assertions based on message interactions.
 Author-email: Felix Divo <felix.divo@sailingteam.tu-darmstadt.de>
 Project-URL: Homepage, https://github.com/felixdivo/ros2-easy-test
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
@@ -17,39 +17,40 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 # ROS2 easy-test
 
-[![PyPI version](https://img.shields.io/pypi/v/ros2-easy-test.svg)](https://pypi.org/project/ros2-easy-test/)
-[![license](https://img.shields.io/pypi/l/ros2-easy-test.svg)](https://github.com/felixdivo/ros2-easy-test/blob/main/LICENSE)
+[![PyPI version](https://img.shields.io/pypi/v/ros2-easy-test.svg?color=blue)](https://pypi.org/project/ros2-easy-test/)
+[![license](https://img.shields.io/pypi/l/ros2-easy-test.svg?color=blue)](https://github.com/felixdivo/ros2-easy-test/blob/main/LICENSE)
 [![ros2 version](https://img.shields.io/badge/ROS2-Foxy%20Fitzroy+%20(see%20limitations)-blue)](https://docs.ros.org/en/rolling/Releases.html)
-[![python version](https://img.shields.io/badge/python-3.8+%20(matching%20ROS)-blue)](https://devguide.python.org/versions/)
+[![Python version](https://img.shields.io/badge/python-3.8+%20(matching%20ROS)-blue)](https://devguide.python.org/versions/)
 
 [![CI status](https://github.com/felixdivo/ros2-easy-test/actions/workflows/python-package.yaml/badge.svg)](https://github.com/felixdivo/ros2-easy-test/actions/workflows/python-package.yaml)
-[![Doc status](https://readthedocs.org/projects/ros2-easy-test/badge/)](https://ros2-easy-test.readthedocs.io/en/latest/)
+[![documentation status](https://readthedocs.org/projects/ros2-easy-test/badge/)](https://ros2-easy-test.readthedocs.io/en/latest/)
 [![code style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 [![linter](https://img.shields.io/badge/linter-ruff-black)](https://github.com/charliermarsh/ruff)
+[![static type checker](https://img.shields.io/badge/static%20typing-mypy-black)](https://mypy-lang.org/)
 
 A Python test framework for [ROS2](https://ros.org/) allowing for:
-- simple and expressive assertions based on message/service interactions (black box testing)
+- simple and expressive assertions based on message and service interactions (black box testing)
 - easy integration of existing nodes and launch files
 - testing of nodes implemented in any programming language (C++, Python, ...)
 - works with and without tools like `colcon test` and `pytest`
 - is minimalistic and has [very few dependencies](https://github.com/felixdivo/ros2-easy-test/blob/main/pyproject.toml)
-- is tested, used in practice, [documented](https://ros2-easy-test.readthedocs.io/en/latest/), and maintained
+- is typed and [documented](https://ros2-easy-test.readthedocs.io/en/latest/)
+- is tested, used in practice, and maintained
 
 ## Installation
 
-At the moment, you can run the following to install this package.
+Just run:
 ```shell
-pip install git+git://github.com/felixdivo/ros2-easy-test
+pip install ros2-easy-test
 ```
-In the future, we intend to publish this repository to be easily installed with rosdep and via PyPI.
 
 ## Examples
 
 The following two examples show off the usage of the Python decorators `@with_single_node` and `@with_launch_file`, which provide the core functionality of this package.
 To get a better grasp of their inner workings, have a look at their implementation [here](ros2_easy_test/decorators.py).
 Besides the simple examples here, you can embed everything in `unittest.TestCase` as well. 
 To check out how, have a look at the provided [tests/](tests/) for some advanced examples.
@@ -98,24 +99,24 @@
 
 ### How you can interact with the node(s)
 
 Using `ROS2TestEnvironment`, you can call:
 - `publish(topic: str, message: RosMessage) -> None`
 - `listen_for_messages(topic: str, time_span: float) -> List[RosMessage]`
 - `clear_messages(topic: str) -> None` to forget all messages that have been received so far.
+- `call_service(name: str, request: Request, timeout_availability: Optional[float], timeout_call: Optional[float]) -> Response`
 
 Note that `ROS2TestEnvironment` is a `rclpy.node.Node` and thus has all the methods of a ROS2 node. 
-As an example, you can create a service by `env.create_service(...)` and then use it with `env.call(...)`.
 In addition, nothing stops you from using any other means of interacting with ROS2 that would work otherwise.
 
 ### What you can test (recommended way of obtaining messages)
 
 Using `ROS2TestEnvironment`, you can assert:
-- `assert_message_published(topic: str, timeout: float) -> RosMessage`
-- `assert_no_message_published(topic: str, timeout: float) -> None`
+- `assert_message_published(topic: str, timeout: Optional[float]) -> RosMessage`
+- `assert_no_message_published(topic: str, timeout: Optional[float]) -> None`
 - `assert_messages_published(topic: str, number: int, ...) -> List[RosMessage]`
 
 Generally, you can always test that no exceptions are thrown, e.g., when nodes are initialized (see limitations below).
 
 ### Combining with other tools
 
 Some hints:
@@ -146,18 +147,17 @@
 # open build/html/index.html in you browser
 
 # You can also run a small webserver to serve the static files with
 cd build/html
 python -m http.server
 ```
 
+## Changelog
+
+See [Releases](https://github.com/felixdivo/ros2-easy-test/releases).
+
 ## License
 
 See [LICENSE](LICENSE).
 
 Initially developed by [Felix Divo](https://github.com/felixdivo) at [*Sailing Team Darmstadt e. V.*](https://www.st-darmstadt.de/), a student group devoted to robotic sailing based in Darmstadt, Germany.
 Thanks to [Simon Kohaut](https://github.com/simon-kohaut) for his kind and nuanced feedback.
-
-## TODOs
-
-- spread the word
-- push to PyPI
```

### Comparing `ros2_easy_test-0.1.0/README.md` & `ros2_easy_test-0.2.0.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # ROS2 easy-test
 
-[![PyPI version](https://img.shields.io/pypi/v/ros2-easy-test.svg)](https://pypi.org/project/ros2-easy-test/)
-[![license](https://img.shields.io/pypi/l/ros2-easy-test.svg)](https://github.com/felixdivo/ros2-easy-test/blob/main/LICENSE)
+[![PyPI version](https://img.shields.io/pypi/v/ros2-easy-test.svg?color=blue)](https://pypi.org/project/ros2-easy-test/)
+[![license](https://img.shields.io/pypi/l/ros2-easy-test.svg?color=blue)](https://github.com/felixdivo/ros2-easy-test/blob/main/LICENSE)
 [![ros2 version](https://img.shields.io/badge/ROS2-Foxy%20Fitzroy+%20(see%20limitations)-blue)](https://docs.ros.org/en/rolling/Releases.html)
-[![python version](https://img.shields.io/badge/python-3.8+%20(matching%20ROS)-blue)](https://devguide.python.org/versions/)
+[![Python version](https://img.shields.io/badge/python-3.8+%20(matching%20ROS)-blue)](https://devguide.python.org/versions/)
 
 [![CI status](https://github.com/felixdivo/ros2-easy-test/actions/workflows/python-package.yaml/badge.svg)](https://github.com/felixdivo/ros2-easy-test/actions/workflows/python-package.yaml)
-[![Doc status](https://readthedocs.org/projects/ros2-easy-test/badge/)](https://ros2-easy-test.readthedocs.io/en/latest/)
+[![documentation status](https://readthedocs.org/projects/ros2-easy-test/badge/)](https://ros2-easy-test.readthedocs.io/en/latest/)
 [![code style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 [![linter](https://img.shields.io/badge/linter-ruff-black)](https://github.com/charliermarsh/ruff)
+[![static type checker](https://img.shields.io/badge/static%20typing-mypy-black)](https://mypy-lang.org/)
 
 A Python test framework for [ROS2](https://ros.org/) allowing for:
-- simple and expressive assertions based on message/service interactions (black box testing)
+- simple and expressive assertions based on message and service interactions (black box testing)
 - easy integration of existing nodes and launch files
 - testing of nodes implemented in any programming language (C++, Python, ...)
 - works with and without tools like `colcon test` and `pytest`
 - is minimalistic and has [very few dependencies](https://github.com/felixdivo/ros2-easy-test/blob/main/pyproject.toml)
-- is tested, used in practice, [documented](https://ros2-easy-test.readthedocs.io/en/latest/), and maintained
+- is typed and [documented](https://ros2-easy-test.readthedocs.io/en/latest/)
+- is tested, used in practice, and maintained
 
 ## Installation
 
-At the moment, you can run the following to install this package.
+Just run:
 ```shell
-pip install git+git://github.com/felixdivo/ros2-easy-test
+pip install ros2-easy-test
 ```
-In the future, we intend to publish this repository to be easily installed with rosdep and via PyPI.
 
 ## Examples
 
 The following two examples show off the usage of the Python decorators `@with_single_node` and `@with_launch_file`, which provide the core functionality of this package.
 To get a better grasp of their inner workings, have a look at their implementation [here](ros2_easy_test/decorators.py).
 Besides the simple examples here, you can embed everything in `unittest.TestCase` as well. 
 To check out how, have a look at the provided [tests/](tests/) for some advanced examples.
@@ -77,24 +78,24 @@
 
 ### How you can interact with the node(s)
 
 Using `ROS2TestEnvironment`, you can call:
 - `publish(topic: str, message: RosMessage) -> None`
 - `listen_for_messages(topic: str, time_span: float) -> List[RosMessage]`
 - `clear_messages(topic: str) -> None` to forget all messages that have been received so far.
+- `call_service(name: str, request: Request, timeout_availability: Optional[float], timeout_call: Optional[float]) -> Response`
 
 Note that `ROS2TestEnvironment` is a `rclpy.node.Node` and thus has all the methods of a ROS2 node. 
-As an example, you can create a service by `env.create_service(...)` and then use it with `env.call(...)`.
 In addition, nothing stops you from using any other means of interacting with ROS2 that would work otherwise.
 
 ### What you can test (recommended way of obtaining messages)
 
 Using `ROS2TestEnvironment`, you can assert:
-- `assert_message_published(topic: str, timeout: float) -> RosMessage`
-- `assert_no_message_published(topic: str, timeout: float) -> None`
+- `assert_message_published(topic: str, timeout: Optional[float]) -> RosMessage`
+- `assert_no_message_published(topic: str, timeout: Optional[float]) -> None`
 - `assert_messages_published(topic: str, number: int, ...) -> List[RosMessage]`
 
 Generally, you can always test that no exceptions are thrown, e.g., when nodes are initialized (see limitations below).
 
 ### Combining with other tools
 
 Some hints:
@@ -125,18 +126,17 @@
 # open build/html/index.html in you browser
 
 # You can also run a small webserver to serve the static files with
 cd build/html
 python -m http.server
 ```
 
+## Changelog
+
+See [Releases](https://github.com/felixdivo/ros2-easy-test/releases).
+
 ## License
 
 See [LICENSE](LICENSE).
 
 Initially developed by [Felix Divo](https://github.com/felixdivo) at [*Sailing Team Darmstadt e. V.*](https://www.st-darmstadt.de/), a student group devoted to robotic sailing based in Darmstadt, Germany.
 Thanks to [Simon Kohaut](https://github.com/simon-kohaut) for his kind and nuanced feedback.
-
-## TODOs
-
-- spread the word
-- push to PyPI
```

### Comparing `ros2_easy_test-0.1.0/doc/Makefile` & `ros2_easy_test-0.2.0.post1/doc/Makefile`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
-SPHINXOPTS    ?= -W --keep-going
+SPHINXOPTS    ?= --keep-going
 SPHINXBUILD   ?= sphinx-build
 SOURCEDIR     = source
 BUILDDIR      = build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `ros2_easy_test-0.1.0/doc/make.bat` & `ros2_easy_test-0.2.0.post1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/doc/source/conf.py` & `ros2_easy_test-0.2.0.post1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/doc/source/design_and_limits.rst` & `ros2_easy_test-0.2.0.post1/doc/source/design_and_limits.rst`

 * *Files 9% similar despite different names*

```diff
@@ -18,22 +18,23 @@
   `not supported in ROS2 <https://discourse.ros.org/t/what-is-the-expected-behavior-of-rclcpp-in-case-of-an-exception-raised-in-a-user-callback/27527>`__.
   It will probably still fail because some expected message is not detected by the test.
   In those cases, you will have to look for messages like ``The following exception was never retrieved: [...]`` in the stderr output of pytest.
   It will probably be mixed in with other messages if you view it on the console.
 - Similar "silent" crashes can occur in other places, including timers and services.
   See ``tests/test_failing_nodes.py`` for unit tests on that behavior.
   A lot of them are marked with a ``TODO:``, since it is currently not straightforward to detect such issues.
-- A failing service might deadlock a test. Consider calling services asynchronously with timeouts.
+- A failing service might deadlock a test. Consider calling services asynchronously with timeouts, e.g. with
+  :meth:`~ros2_easy_test.env.ROS2TestEnvironment.call_service` or :meth:`~ros2_easy_test.env.ROS2TestEnvironment.await_future`.
 - It takes some time to set up the test environment each time, particularly when using ``@with_launch_file``.
   Also, some nodes or complex launch scenarios might need considerable time to process information.
   You may wish to append ``--durations=0 --durations-min=1.0`` to your pytest call to show the slowest tests
   (`more info <https://docs.pytest.org/en/latest/how-to/usage.html#profiling-test-execution-duration>`__).
   It might be possible to reduce the required ``warmup_time``,
   since it is unclear why setting it too low breaks *all* message exchanges and maybe there is a solvable bug causing it.
-- Currently, using services only works from ROS2 version Humble onwards, and not on Foxy.
+- Currently, interacting via services only works from ROS2 version Humble onwards, and not on Foxy.
   Similarly, a few of the tests seem to freeze sometimes.
   I do not intend to investigate further, sice `that version will reach end of life very soon <https://endoflife.date/ros2>`__.
 
 Design Considerations
 ---------------------
 
 These were the initial design considerations. Over time, this may shift.
@@ -51,16 +52,17 @@
   <https://docs.ros.org/en/rolling/The-ROS2-Project/Contributing/Developer-Guide.html#testing>`__).
 - Be well-documented and easy to get started.
 - Support the most widely used platforms (that have not reached end of life yet). Be pragmatic.
 
 Constraints
 ~~~~~~~~~~~
 
-- Be easy to maintain by needing only a few lines of code (below a thousand). Thus, actions and services are
-  currently not supported. Also, only use public APIs wherever possible.
+- Be easy to maintain by needing only a few lines of code (below a thousand).
+  Thus, actions are currently not supported.
+  Also, we only use public APIs wherever possible.
 - Don't reinvent the wheel and benefit from future improvements: Use existing functionality of Python and
   ROS2. This includes: :mod:`unittest`, :mod:`pytest`, and the
   `ROS2 launch system <https://design.ros2.org/articles/roslaunch.html>`__.
 - Efficiency is not a primary concern as this mini-framework is intended to only be used for testing
   and not in a real robot deployment, where performance is much more of a concern.
 - Must work with ``colcon test`` (see `here <https://colcon.readthedocs.io/en/released/reference/verb/test.html>`__) and also with just *pytest* alone (for simpler IDE integration).
```

### Comparing `ros2_easy_test-0.1.0/pyproject.toml` & `ros2_easy_test-0.2.0.post1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # The package is discovered automatically (including the py.typed file):
 # https://setuptools.pypa.io/en/latest/userguide/package_discovery.html#flat-layout
 
 [project.optional-dependencies]
 dev = [
   "black~=23.1",
   "ruff",
+  "mypy~=1.3.0",
   "pytest",
   "pytest-cov",
   "pytest-sugar",
   "hypothesis",  # To demonstrate how it works with this
 ]
 doc = [
   "sphinx",
@@ -66,7 +67,20 @@
 select = ["E", "F", "W", "I", "N", "UP"]
 
 # Same as Black
 line-length = 110
 
 # The lowest supported version
 target-version = "py38"
+
+[tool.mypy]
+warn_return_any = true
+warn_unused_configs = true
+
+[[tool.mypy.overrides]]
+module = [
+    "rclpy.*",  # For the CI pipeline to work
+    "launch.*",
+    "example_interfaces.*",
+    "std_msgs.*",
+]
+ignore_missing_imports = true
```

### Comparing `ros2_easy_test-0.1.0/ros2_easy_test/decorators.py` & `ros2_easy_test-0.2.0.post1/ros2_easy_test/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,18 @@
 
 # Standard library
 from functools import wraps
 from inspect import signature
 from pathlib import Path
 from signal import SIGINT
 from subprocess import Popen, TimeoutExpired
-from threading import Thread
 from time import sleep
 
 # Typing
-from typing import Any, Callable, Dict, Optional, Type, Union
+from typing import Any, Callable, Coroutine, Dict, Optional, Type, TypeVar, Union
 
 # ROS
 from rclpy.context import Context
 from rclpy.executors import MultiThreadedExecutor
 from rclpy.node import InvalidHandle, Node
 from rclpy.parameter import Parameter
 
@@ -34,26 +33,29 @@
 
 
 __all__ = ["with_launch_file", "with_single_node"]
 
 
 # From python 3.10+ on, we should make these typing.TypeAlias'es
 # Currently not possible to type the following any better
-TestFunctionBefore = Callable[..., None]
-TestFunctionAfter = Callable[..., None]  # The same but taking one kwarg less (the env)
+_TestReturnType = TypeVar("_TestReturnType", None, Coroutine[Any, Any, None])
+TestFunctionBefore = Callable[..., _TestReturnType]
+# The same but taking one kwarg less (the env), which we can't statically type
+TestFunctionAfter = Callable[..., _TestReturnType]
 
 
 #: The time to give a node for a successful shutdown.
 _DEFAULT_SHUTDOWN_TIMEOUT: float = 2
 
 
 def with_single_node(
     node_class: Type[Node],
     *,
     parameters: Optional[Dict[str, Any]] = None,
+    time_limit: Optional[float] = 60,
     shutdown_timeout=_DEFAULT_SHUTDOWN_TIMEOUT,
     **kwargs,
 ) -> Callable[[TestFunctionBefore], TestFunctionAfter]:
     """Marks a test case that shall be wrapped by a ROS2 context and be given an environment to interact.
 
     This function is not fundamentally restricted to one node, but more are simply not implemented as of
     now. See :func:`~with_launch_file` for more complex scenarios.
@@ -70,14 +72,19 @@
         ``super().__init__("node name", **kwargs)``.
 
     Args:
         node_class:
             Class of the node to instantiate. Assumed to accept no extra parameters besides **any** keyword
             arguments that are passed along to :class:`rclpy.node.Node`.
         parameters: The parameters to be set for the node as ``("key", value)`` pairs
+        time_limit:
+            The time in seconds to give the test case to complete.
+            This only applies to the test function, not the node setup etc.
+            If it takes longer than this, the test will fail.
+            Set to ``None`` to disable the timeout.
         shutdown_timeout:
             The time to give a node for a successful shutdown. If it takes longer than this,
             the test will fail.
         kwargs: Passed to the :class:`ros2_easy_test.env.ROS2TestEnvironment`
 
     See Also:
         :func:`~with_launch_file`
@@ -94,17 +101,19 @@
                 parameters_tuples = parameters or {}
                 ros_parameters = [
                     Parameter(name=name, value=value) for name, value in parameters_tuples.items()
                 ]
 
                 node: Node
                 if ros_parameters:
-                    node = node_class(parameter_overrides=ros_parameters, context=context)
+                    node = node_class(  # type: ignore[call-arg]
+                        parameter_overrides=ros_parameters, context=context
+                    )
                 else:
-                    node = node_class(context=context)
+                    node = node_class(context=context)  # type: ignore[call-arg]
 
                 # We need at least two threads: One to spin() and one to execute the test case (as the latter
                 # blocks). We better provide 4, since more nodes/tasks might get spun up by some tests and
                 # threads are rather cheap.
                 executor = MultiThreadedExecutor(num_threads=4, context=context)
 
                 try:
@@ -115,21 +124,28 @@
                     environment = ROS2TestEnvironment(context=context, **kwargs)
                     assert executor.add_node(environment), "Failed to add environment."
 
                     # Finally, we want to launch the actual test and wait for it to complete (indefinitely)
                     test_function_task = executor.create_task(
                         test_function, *args_inner, env=environment, **kwargs_inner
                     )
-                    thread = Thread(
-                        target=executor.spin_until_future_complete,
-                        args=(test_function_task,),
-                        daemon=True,
+                    # The type ignore is needed due to a bug in ROS2 Humble+
+                    executor.spin_until_future_complete(
+                        test_function_task, timeout_sec=time_limit  # type: ignore[arg-type]
                     )
-                    thread.start()
-                    thread.join()
+
+                    test_function_exception = test_function_task.exception()
+                    if not test_function_task.done():
+                        # Then test_function_exception can only be None, so we can overwrite it
+                        test_function_exception = TimeoutError(
+                            f"The test case did not complete in time ({time_limit} seconds). "
+                            "Consider passing a higher time_limit or setting it to None to disable it."
+                        )
+                        # Then, make sure to kill the test function as cleanup
+                        test_function_task.cancel()
 
                 finally:
                     for running_node in executor.get_nodes():
                         running_node.destroy_node()
 
                     has_finished = executor.shutdown(shutdown_timeout)
                     assert has_finished, f"Executor shutdown did not complete in {shutdown_timeout} seconds."
@@ -151,17 +167,16 @@
                     pass  # This is what we expect to happen
                 else:  # pragma: no cover
                     raise Exception("The Environment did not properly shut down after test.")
 
                 assert not executor.get_nodes(), "The executor still holds some nodes."
 
                 # Raise the exception that the test case might have raised, e.g. due to asserts
-                exception = test_function_task.exception()
-                if exception is not None:
-                    raise exception from None
+                if test_function_exception is not None:
+                    raise test_function_exception from None
 
                 # TODO: We should also raise exceptions that are raised in callbacks, but that's tricky
                 # because executor.spin_until_future_complete will not raise them.
                 # Currently, we can just point the users to look at the console for a
                 # "The following exception was never retrieved: [...]" message.
 
             finally:
@@ -169,25 +184,28 @@
 
             # Make sure that the context is freed afterwards. This sanity check should never fail.
             assert not context.ok(), "Context did not properly shut down after test."
 
         # This is required to make pytest fixtures work
         # In principle, we could make the parameter name easily adjustable,
         # but that is probably a rare use case
-        wrapper.__signature__ = remove_signature_parameters(signature(test_function), "env")
+        wrapper.__signature__ = remove_signature_parameters(  # type: ignore[attr-defined]
+            signature(test_function), "env"
+        )
         return wrapper
 
     return decorator
 
 
 def with_launch_file(  # noqa: C901
     launch_file: Union[Path, str],
     *,
     debug_launch_file: bool = False,
-    warmup_time: float = 5,
+    warmup_time: float = 2,
+    time_limit: Optional[float] = 60,
     shutdown_timeout=_DEFAULT_SHUTDOWN_TIMEOUT,
     **kwargs,
 ) -> Callable[[TestFunctionBefore], TestFunctionAfter]:
     """Marks a test case that shall be wrapped by a ROS2 context and be given an environment to interact.
 
     Note:
         Your test function *must* accept the environment as a keyword-parameter called ``env``,
@@ -202,14 +220,19 @@
             However, it might also cause sudden failures, therefore the default is ``False``.
         warmup_time:
             The time to sleep while letting the ROS2 system spin up. Must be zero or larger.
             Strange bugs will occur when this value is set too low: No messages can be exchanged,
             independently of how long the test waits.
             The default should suffice on most computers,
             it is rather conservative and higher numbers will slow down each test case even more.
+        time_limit:
+            The time in seconds to give the test case to complete.
+            This only applies to the test function, not the node setup etc.
+            If it takes longer than this, the test will fail.
+            Set to ``None`` to disable the timeout.
         shutdown_timeout:
             The time to give a node for a successful shutdown. If it takes longer than this,
             the test will fail.
             It applies individually to both shutting down the environment and the launch process.
         kwargs: Passed to the :class:`ros2_easy_test.env.ROS2TestEnvironment`
 
     See Also:
@@ -241,43 +264,49 @@
                     # We need at least two threads: One to spin() and one to execute the test case
                     # (as the latter blocks). We better provide 4, since more nodes/tasks might get spun up
                     # by some tests and threads are rather cheap.
                     executor = MultiThreadedExecutor(num_threads=4, context=context)
 
                     try:
                         # We first start the environment, such that any topics that are watched can be
-                        # captured rigth from the start
+                        # captured right from the start
                         environment = ROS2TestEnvironment(context=context, **kwargs)
                         assert executor.add_node(environment), "failed to add environment"
 
-                        # We should not need any warmp time here, as the environment is fully ready once the
+                        # We should not need any warmup time here, as the environment is fully ready once the
                         # node class (the environment) is instantiated.
-                        # TODO: However, this warmup and cleaing seems to suppress some rather rare errors.
+                        # TODO: However, this warmup and cleaning seems to suppress some rather rare errors.
                         executor.spin_until_future_complete(executor.create_task(sleep, 2))
                         environment.clear_messages()
 
                         # Now, we are ready to start the system under test using "ros2 launch"
                         ros2_process = Popen(ros2_parameters)
 
                         # Give the launch process time to start up. Otherwise, the timeouts on the first
                         # test asserts will be off and the system wil generally behave strangely.
                         # TODO: Ususally, this shouldn't need to be this high. Reducing it would be awesome.
                         executor.spin_until_future_complete(executor.create_task(sleep, warmup_time))
 
                         test_function_task = executor.create_task(
                             test_function, *args_inner, env=environment, **kwargs_inner
                         )
-
-                        thread = Thread(
-                            target=executor.spin_until_future_complete,
-                            args=(test_function_task,),
-                            daemon=True,
+                        # The type ignore is needed due to a bug in ROS2 Humble+
+                        executor.spin_until_future_complete(
+                            test_function_task, timeout_sec=time_limit  # type: ignore[arg-type]
                         )
-                        thread.start()
-                        thread.join()
+
+                        test_function_exception = test_function_task.exception()
+                        if not test_function_task.done():
+                            # Then test_function_exception can only be None, so we can overwrite it
+                            test_function_exception = TimeoutError(
+                                f"The test case did not complete in time ({time_limit} seconds). "
+                                "Consider passing a higher time_limit or setting it to None to disable it."
+                            )
+                            # Then, make sure to kill the test function as cleanup
+                            test_function_task.cancel()
 
                     finally:
                         # This should only kill the environment, no other node is registered
                         for node in executor.get_nodes():
                             node.destroy_node()
 
                         has_finished = executor.shutdown(shutdown_timeout)
@@ -318,32 +347,33 @@
                         except TimeoutExpired:  # pragma: no cover
                             ros2_process.terminate()
                             # return_code will be larger than 130
                             return_code = ros2_process.wait(timeout=shutdown_timeout / 2)
 
                 # Both SUCCESS (0) or the result code of SIGINT (130) are acceptable
                 return_code_problematic = return_code not in {0, 130}
-                test_function_exception = test_function_task.exception()
 
                 if return_code_problematic:
                     if test_function_exception is None:
                         raise AssertionError(
                             f"The ROS launch process FAILED with exit code {return_code} "
                             "(please inspect stdout and stderr) BUT the test case SUCCEEDED."
-                        )
+                        ) from None
 
                     raise AssertionError(
                         f"The ROS launch process FAILED with exit code {return_code} "
                         "(please inspect stdout and stderr) AND the test FAILED with "
                         f'exception: "{test_function_exception}".'
                     ) from test_function_exception
 
                 if test_function_exception is not None:
                     raise test_function_exception from None
 
         # This is required to make pytest fixtures work
         # In principle, we could make the parameter name easily adjustable,
         # but that is probably a rare use case
-        wrapper.__signature__ = remove_signature_parameters(signature(test_function), "env")
+        wrapper.__signature__ = remove_signature_parameters(  # type: ignore[attr-defined]
+            signature(test_function), "env"
+        )
         return wrapper
 
     return decorator
```

### Comparing `ros2_easy_test-0.1.0/ros2_easy_test/env.py` & `ros2_easy_test-0.2.0.post1/ros2_easy_test/env.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """This module provides the environment by which tests can interact with nodes."""
 
 # Standard library
+from importlib import import_module
 from queue import Empty, SimpleQueue
 from threading import RLock
-from time import sleep, time
+from time import monotonic, sleep
 
 # Typing
-from typing import Any, Dict, List, Mapping, Optional, Type
+from typing import Any, Dict, List, Mapping, Optional, Type, cast
 
 # ROS
+from rclpy.client import Client, SrvTypeRequest, SrvTypeResponse
 from rclpy.node import Node
 from rclpy.publisher import Publisher
 from rclpy.qos import QoSHistoryPolicy, QoSProfile
+from rclpy.task import Future
 
 RosMessage = Any  # We can't be more specific for now
 
 __all__ = ["ROS2TestEnvironment"]
 
 #: The normal timeout for asserts, like waiting for messages. This has to be surprisingly high.
 _DEFAULT_TIMEOUT: Optional[float] = 2
@@ -28,24 +31,25 @@
     However, one must ensure that the type of the message that is published stays the same across each test.
 
     For **subscribers**, the topics and their types must be declared at the instantiation via the
     ``watch_topics`` argument. This cannot be avoided due to how *rclpy* works.
     Then, a mailbox is created for each topic and incoming messages are collected each (without a limit).
     This is performed in the background, meaning that for example :meth:`~assert_message_published` may return
     a message that was collected before the method was called.
-    To prevent this from happening, one might use:meth:`clear_messages` (although the concurrency is often the
-    desired behaviour).
+    To prevent this from happening, one might use :meth:`~clear_messages`
+    (although the concurrency is often the desired behaviour).
     Also, mind the ``timeout`` / ``time_span`` arguments as they determine how long to wait while checking the
     assertion (default: ``1`` second).
     Asserting that a message is sent or failing to assert that no message is sent will return early.
 
+    **Services** are handled similarly to publishers, being created on the fly when used for the first time.
+
     Note:
         The :class:`ROS2TestEnvironment` is a :class:`rclpy.node.Node` too, which allows to implement custom
-        functionality too. In particular, one can simply call services using code similar to:
-        ``client = env.create_client(GetLocalTangentPoint, "/service/get_local_tangent_point")``.
+        functionality too.
 
     Note:
         Timings and timeouts in this class are only approximate.
 
     Args:
         watch_topics: The topics (and their type) to watch for incoming messages.
             You may pass ``None`` to not watch any topic.
@@ -74,14 +78,18 @@
             # After the mailboxes are set up, we can start receiving messages
             self.create_subscription(message_type, topic, callback, self._qos_profile)
 
         # Prepare to collect publishers; these are set up on the fly when used the first time in `publish()`
         self._registered_publishers_lock = RLock()
         self._registered_publishers: Dict[str, Publisher] = {}
 
+        # Similarly for services
+        self._registered_services_lock = RLock()
+        self._registered_services: Dict[str, Client] = {}
+
     def _get_mailbox_for(self, topic: str) -> "SimpleQueue[RosMessage]":
         """Checks that a topic is watched for and returns the appropriate mailbox. Handles synchronization.
 
         Args:
             topic: The topic to check and fetch the mailbox of
 
         Returns:
@@ -94,36 +102,36 @@
         with self._subscriber_mailboxes_lock:
             assert (
                 topic in self._subscriber_mailboxes
             ), f"topic {topic} it not being watched: please specify it in the constructor"
 
             return self._subscriber_mailboxes[topic]
 
+    def _get_publisher(self, topic: str, msg_type: Type) -> Publisher:
+        """Get or else create the correct publisher and cache it."""
+        with self._registered_publishers_lock:
+            try:
+                return self._registered_publishers[topic]
+            except KeyError:
+                publisher = self.create_publisher(msg_type, topic, self._qos_profile)
+                self._registered_publishers[topic] = publisher
+                return publisher
+
     def publish(self, topic: str, message: RosMessage) -> None:
         """Publish the message on the topic.
 
         This method creates the publisher internally if required and caches it.
         Nothing needs to be done manually.
 
         Args:
             topic: The topic to publish on
             message: The message to be sent. It's type must match the one of all other messages sent on this
                 ``topic`` before and after.
         """
-
-        # Get or else create the correct publisher and cache it
-        publisher: Publisher
-        with self._registered_publishers_lock:
-            try:
-                publisher = self._registered_publishers[topic]
-            except KeyError:
-                publisher = self.create_publisher(type(message), topic, self._qos_profile)
-                self._registered_publishers[topic] = publisher
-
-        publisher.publish(message)
+        self._get_publisher(topic, type(message)).publish(message)
 
     def assert_no_message_published(self, topic: str, time_span: float = 0.5) -> None:
         """Asserts that no message is published on the given topic within the given time.
 
         Args:
             topic: The topic to listen on
             time_span:
@@ -203,25 +211,25 @@
                 timeout = max_total_timeout
 
         remaining_time = timeout
         count = 0
         collected_messages: List[RosMessage] = []
 
         while count < number:
-            start = time()
+            start = monotonic()
             try:
                 collected_messages.append(self.assert_message_published(topic, timeout=remaining_time))
             except AssertionError:
                 raise AssertionError(
                     f"Only {count} messages out of {number} expected ones were published on "
                     f"topic {topic} after a total timeout of {timeout} seconds"
                 ) from None
             else:
                 if remaining_time is not None:
-                    remaining_time = max(0.0, remaining_time - (time() - start))
+                    remaining_time = max(0.0, remaining_time - (monotonic() - start))
                 count += 1
 
         assert len(collected_messages) == number, "internal counting error"
         return collected_messages
 
     def listen_for_messages(
         self, topic: str, time_span: Optional[float] = _DEFAULT_TIMEOUT
@@ -264,7 +272,82 @@
             with self._subscriber_mailboxes_lock:  # This is reentrant
                 for topic in self._subscriber_mailboxes.keys():
                     self.clear_messages(topic=topic)
 
         else:
             # There is not clear() in SimpleQueue
             self.listen_for_messages(topic, time_span=None)  # ignore the result
+
+    def await_future(self, future: Future, timeout: Optional[float] = 10) -> Any:
+        """Waits for the given future to complete.
+
+        Args:
+            future: The future to wait for
+            timeout: The timeout to wait for the future
+
+        Raises:
+            TimeoutError: If the future did not complete within the timeout
+            Exception: If the future completed with an exception
+
+        Returns:
+            The result of the future
+        """
+
+        # This does not work with the default executor, so we use the one from the node
+        assert self.executor, "executor is not set"
+        # The type ignore is needed due to a bug in ROS2 Humble+
+        self.executor.spin_until_future_complete(future, timeout_sec=timeout)  # type: ignore[arg-type]
+
+        if future.done():
+            return future.result()
+        else:
+            raise TimeoutError(f"Future did not complete within {timeout} seconds")
+
+    def _get_service_client(self, name: str, request_class: Type) -> Client:
+        """Returns the service client for the given service name."""
+
+        with self._registered_services_lock:
+            try:
+                return self._registered_services[name]
+            except KeyError:
+                # Get the type of the service
+                # This is a bit tricky but relieves the user from passing it explicitly
+                module = import_module(request_class.__module__)
+                # We cut away the trailing "_Request" from the type name, which has length 8
+                base_type_name = request_class.__name__[:-8]
+                base_type_class: Type = getattr(module, base_type_name)
+
+                client = self.create_client(base_type_class, name)
+                self._registered_services[name] = client
+                return client
+
+    def call_service(
+        self,
+        name: str,
+        request: SrvTypeRequest,
+        timeout_availability: Optional[float] = 1,
+        timeout_call: Optional[float] = 10,
+    ) -> SrvTypeResponse:  # type: ignore[type-var]
+        """Calls the given service with the given request once available and returns the response.
+
+        The service type if inferred automatically from the request type.
+
+        Args:
+            name: The name of the service
+            request: The request to send to the service
+            timeout_availability: The timeout to wait for the service to be available
+            timeout_call: The timeout to wait for the service to respond
+
+        Returns:
+            The response of the service
+
+        Raises:
+            TimeoutError: If the service did not respond within the timeout
+        """
+        client = self._get_service_client(name, type(request))
+        # The type ignore is needed due to a bug in ROS2 Humble+
+        is_ready = client.wait_for_service(timeout_availability)  # type: ignore[arg-type]
+        if not is_ready:
+            raise TimeoutError(f"Service {name} did not become ready within {timeout_availability} seconds")
+
+        future = client.call_async(request)
+        return cast(SrvTypeResponse, self.await_future(future, timeout=timeout_call))
```

### Comparing `ros2_easy_test-0.1.0/ros2_easy_test/launch_file.py` & `ros2_easy_test-0.2.0.post1/ros2_easy_test/launch_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
     def __enter__(self) -> Path:
         if self.is_path:
             launch_file_path = self._launch_file
             if not isinstance(launch_file_path, Path):
                 launch_file_path = Path(self._launch_file)
         else:
+            assert isinstance(self._launch_file, str)
             directory = TemporaryDirectory()
             self._exit_list.append(cast(ContextManager[str], directory))
             directory_name = Path(directory.__enter__())
             launch_file_path = directory_name / "launch_file"
             with open(launch_file_path, "w", encoding="utf-8") as file:
                 file.write(self._launch_file)
```

### Comparing `ros2_easy_test-0.1.0/ros2_easy_test.egg-info/PKG-INFO` & `ros2_easy_test-0.2.0.post1/ros2_easy_test.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros2-easy-test
-Version: 0.1.0
+Version: 0.2.0.post1
 Summary: A Python test framework for ROS2 allowing simple and expressive assertions based on message interactions.
 Author-email: Felix Divo <felix.divo@sailingteam.tu-darmstadt.de>
 Project-URL: Homepage, https://github.com/felixdivo/ros2-easy-test
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
@@ -17,39 +17,40 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 # ROS2 easy-test
 
-[![PyPI version](https://img.shields.io/pypi/v/ros2-easy-test.svg)](https://pypi.org/project/ros2-easy-test/)
-[![license](https://img.shields.io/pypi/l/ros2-easy-test.svg)](https://github.com/felixdivo/ros2-easy-test/blob/main/LICENSE)
+[![PyPI version](https://img.shields.io/pypi/v/ros2-easy-test.svg?color=blue)](https://pypi.org/project/ros2-easy-test/)
+[![license](https://img.shields.io/pypi/l/ros2-easy-test.svg?color=blue)](https://github.com/felixdivo/ros2-easy-test/blob/main/LICENSE)
 [![ros2 version](https://img.shields.io/badge/ROS2-Foxy%20Fitzroy+%20(see%20limitations)-blue)](https://docs.ros.org/en/rolling/Releases.html)
-[![python version](https://img.shields.io/badge/python-3.8+%20(matching%20ROS)-blue)](https://devguide.python.org/versions/)
+[![Python version](https://img.shields.io/badge/python-3.8+%20(matching%20ROS)-blue)](https://devguide.python.org/versions/)
 
 [![CI status](https://github.com/felixdivo/ros2-easy-test/actions/workflows/python-package.yaml/badge.svg)](https://github.com/felixdivo/ros2-easy-test/actions/workflows/python-package.yaml)
-[![Doc status](https://readthedocs.org/projects/ros2-easy-test/badge/)](https://ros2-easy-test.readthedocs.io/en/latest/)
+[![documentation status](https://readthedocs.org/projects/ros2-easy-test/badge/)](https://ros2-easy-test.readthedocs.io/en/latest/)
 [![code style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 [![linter](https://img.shields.io/badge/linter-ruff-black)](https://github.com/charliermarsh/ruff)
+[![static type checker](https://img.shields.io/badge/static%20typing-mypy-black)](https://mypy-lang.org/)
 
 A Python test framework for [ROS2](https://ros.org/) allowing for:
-- simple and expressive assertions based on message/service interactions (black box testing)
+- simple and expressive assertions based on message and service interactions (black box testing)
 - easy integration of existing nodes and launch files
 - testing of nodes implemented in any programming language (C++, Python, ...)
 - works with and without tools like `colcon test` and `pytest`
 - is minimalistic and has [very few dependencies](https://github.com/felixdivo/ros2-easy-test/blob/main/pyproject.toml)
-- is tested, used in practice, [documented](https://ros2-easy-test.readthedocs.io/en/latest/), and maintained
+- is typed and [documented](https://ros2-easy-test.readthedocs.io/en/latest/)
+- is tested, used in practice, and maintained
 
 ## Installation
 
-At the moment, you can run the following to install this package.
+Just run:
 ```shell
-pip install git+git://github.com/felixdivo/ros2-easy-test
+pip install ros2-easy-test
 ```
-In the future, we intend to publish this repository to be easily installed with rosdep and via PyPI.
 
 ## Examples
 
 The following two examples show off the usage of the Python decorators `@with_single_node` and `@with_launch_file`, which provide the core functionality of this package.
 To get a better grasp of their inner workings, have a look at their implementation [here](ros2_easy_test/decorators.py).
 Besides the simple examples here, you can embed everything in `unittest.TestCase` as well. 
 To check out how, have a look at the provided [tests/](tests/) for some advanced examples.
@@ -98,24 +99,24 @@
 
 ### How you can interact with the node(s)
 
 Using `ROS2TestEnvironment`, you can call:
 - `publish(topic: str, message: RosMessage) -> None`
 - `listen_for_messages(topic: str, time_span: float) -> List[RosMessage]`
 - `clear_messages(topic: str) -> None` to forget all messages that have been received so far.
+- `call_service(name: str, request: Request, timeout_availability: Optional[float], timeout_call: Optional[float]) -> Response`
 
 Note that `ROS2TestEnvironment` is a `rclpy.node.Node` and thus has all the methods of a ROS2 node. 
-As an example, you can create a service by `env.create_service(...)` and then use it with `env.call(...)`.
 In addition, nothing stops you from using any other means of interacting with ROS2 that would work otherwise.
 
 ### What you can test (recommended way of obtaining messages)
 
 Using `ROS2TestEnvironment`, you can assert:
-- `assert_message_published(topic: str, timeout: float) -> RosMessage`
-- `assert_no_message_published(topic: str, timeout: float) -> None`
+- `assert_message_published(topic: str, timeout: Optional[float]) -> RosMessage`
+- `assert_no_message_published(topic: str, timeout: Optional[float]) -> None`
 - `assert_messages_published(topic: str, number: int, ...) -> List[RosMessage]`
 
 Generally, you can always test that no exceptions are thrown, e.g., when nodes are initialized (see limitations below).
 
 ### Combining with other tools
 
 Some hints:
@@ -146,18 +147,17 @@
 # open build/html/index.html in you browser
 
 # You can also run a small webserver to serve the static files with
 cd build/html
 python -m http.server
 ```
 
+## Changelog
+
+See [Releases](https://github.com/felixdivo/ros2-easy-test/releases).
+
 ## License
 
 See [LICENSE](LICENSE).
 
 Initially developed by [Felix Divo](https://github.com/felixdivo) at [*Sailing Team Darmstadt e. V.*](https://www.st-darmstadt.de/), a student group devoted to robotic sailing based in Darmstadt, Germany.
 Thanks to [Simon Kohaut](https://github.com/simon-kohaut) for his kind and nuanced feedback.
-
-## TODOs
-
-- spread the word
-- push to PyPI
```

### Comparing `ros2_easy_test-0.1.0/ros2_easy_test.egg-info/SOURCES.txt` & `ros2_easy_test-0.2.0.post1/ros2_easy_test.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 ros2_easy_test.egg-info/dependency_links.txt
 ros2_easy_test.egg-info/requires.txt
 ros2_easy_test.egg-info/top_level.txt
 tests/__init__.py
 tests/test_env_coverage.py
 tests/test_failing_nodes.py
 tests/test_interactions.py
+tests/test_timeouts.py
 tests/demo/__init__.py
+tests/demo/coroutine_test.py
 tests/demo/fixture_test.py
 tests/demo/hypothesis_test.py
 tests/demo/reuse_decorator_test.py
 tests/example_launch_files/adder.yaml
 tests/example_launch_files/echo.yaml
 tests/example_launch_files/raise_in_init.yaml
 tests/example_launch_files/raise_in_timer.yaml
```

### Comparing `ros2_easy_test-0.1.0/tests/demo/fixture_test.py` & `ros2_easy_test-0.2.0.post1/tests/demo/fixture_test.py`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/tests/demo/hypothesis_test.py` & `ros2_easy_test-0.2.0.post1/tests/demo/hypothesis_test.py`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/tests/demo/reuse_decorator_test.py` & `ros2_easy_test-0.2.0.post1/tests/demo/reuse_decorator_test.py`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/tests/example_launch_files/talker.py` & `ros2_easy_test-0.2.0.post1/tests/example_launch_files/talker.py`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/tests/example_nodes/failing.py` & `ros2_easy_test-0.2.0.post1/tests/example_nodes/failing.py`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/tests/example_nodes/run_node.py` & `ros2_easy_test-0.2.0.post1/tests/example_nodes/run_node.py`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/tests/example_nodes/well_behaved.py` & `ros2_easy_test-0.2.0.post1/tests/example_nodes/well_behaved.py`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/tests/test_env_coverage.py` & `ros2_easy_test-0.2.0.post1/tests/test_env_coverage.py`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/tests/test_failing_nodes.py` & `ros2_easy_test-0.2.0.post1/tests/test_failing_nodes.py`

 * *Files identical despite different names*

### Comparing `ros2_easy_test-0.1.0/tests/test_interactions.py` & `ros2_easy_test-0.2.0.post1/tests/test_interactions.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,42 +44,57 @@
 
         # Do the same with env.listen_for_messages
         env.publish("/ear", String(data="Guude"))
         all_messages: List[String] = env.listen_for_messages("/mouth")
         self.assertSequenceEqual(all_messages, [String(data="Guude")])
 
     def test_service(self, env: ROS2TestEnvironment) -> None:
+        # Set up the request
+        request = AddTwoInts.Request(a=-500, b=73)
+        desired_sum = -500 + 73
+
+        # Call the service asynchronously
+        result: int = env.call_service("add_two_ints", request).sum
+        self.assertEqual(result, desired_sum)
+
+    def test_service_manual(self, env: ROS2TestEnvironment) -> None:
         # Set up the service
         adder = env.create_client(AddTwoInts, "add_two_ints")
         self.assertTrue(adder.wait_for_service(timeout_sec=5))
 
         # Set up the request
         request = AddTwoInts.Request(a=-500, b=73)
         desired_sum = -500 + 73
 
         # Call the service synchronously
         result: int = adder.call(request).sum
         self.assertEqual(result, desired_sum)
 
-        # Call the service asynchronously
+        # Call the service asynchronously with a helper
         future = adder.call_async(request)
+        result: int = env.await_future(future, timeout=2).sum
+        self.assertEqual(result, desired_sum)
+
+        # Call the service asynchronously completely manually
+        future = adder.call_async(request)
+        # This needs to be done via the executor of the node, see ROS2TestEnvironment::await_future
         env.executor.spin_until_future_complete(future, timeout_sec=2)
         self.assertIsNone(future.exception())
         result: int = future.result().sum
         self.assertEqual(result, desired_sum)
 
     def test_multiple_messages(self, env: ROS2TestEnvironment, count: int = 5) -> None:
         for identifier in range(count):
             env.publish("/ear", String(data=f"Hi #{identifier}"))
 
         # This text also tests the message order, which *is* relevant!
         all_messages: List[String] = env.assert_messages_published(
             "/mouth",
             number=count,
-            max_total_timeout=10,
+            max_total_timeout=5 + count * 0.05,
         )
         expected = [String(data=f"Hi #{identifier}") for identifier in range(count)]
         self.assertListEqual(all_messages, expected)
 
 
 class TestSingleNode(SharedTestCases, TestCase):
     """This test case uses the ``with_single_node`` decorator to set up the test environment."""
@@ -97,14 +112,19 @@
     def test_subscriber_and_publisher(self, env: ROS2TestEnvironment) -> None:
         super().test_subscriber_and_publisher(env)
 
     @with_single_node(AddTwoIntsServer)
     def test_service(self, env: ROS2TestEnvironment) -> None:
         super().test_service(env)
 
+    @mark.xfail(raises=ValueError, reason="See https://github.com/ros2/rclpy/pull/1129")
+    @with_single_node(AddTwoIntsServer)
+    def test_service_manual(self, env: ROS2TestEnvironment) -> None:
+        super().test_service_manual(env)
+
     @with_single_node(EchoNode, watch_topics={"/mouth": String})
     def test_multiple_messages(self, env: ROS2TestEnvironment) -> None:
         super().test_multiple_messages(env)
 
     @with_single_node(EchoNode, watch_topics={"/mouth": String})
     def test_multiple_messages_stress_test(self, env: ROS2TestEnvironment) -> None:
         super().test_multiple_messages(env, count=1000)
@@ -142,14 +162,19 @@
     def test_subscriber_and_publisher(self, env: ROS2TestEnvironment) -> None:
         super().test_subscriber_and_publisher(env)
 
     @with_launch_file(LAUNCH_FILES / "adder.yaml", warmup_time=2)
     def test_service(self, env: ROS2TestEnvironment) -> None:
         super().test_service(env)
 
+    @mark.xfail(raises=ValueError, reason="See https://github.com/ros2/rclpy/pull/1129")
+    @with_launch_file(LAUNCH_FILES / "adder.yaml", warmup_time=2)
+    def test_service_manual(self, env: ROS2TestEnvironment) -> None:
+        super().test_service_manual(env)
+
     @with_launch_file(LAUNCH_FILES / "echo.yaml", watch_topics={"/mouth": String})
     def test_multiple_messages(self, env: ROS2TestEnvironment) -> None:
         super().test_multiple_messages(env)
 
     @with_launch_file(LAUNCH_FILES / "echo.yaml", watch_topics={"/mouth": String})
     def test_multiple_messages_stress_test(self, env: ROS2TestEnvironment) -> None:
         super().test_multiple_messages(env, count=1000)
```

