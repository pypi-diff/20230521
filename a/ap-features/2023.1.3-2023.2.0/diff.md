# Comparing `tmp/ap_features-2023.1.3.tar.gz` & `tmp/ap_features-2023.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ap_features-2023.1.3.tar", last modified: Wed Feb  8 10:13:51 2023, max compression
+gzip compressed data, was "ap_features-2023.2.0.tar", last modified: Sun May 21 09:31:42 2023, max compression
```

## Comparing `ap_features-2023.1.3.tar` & `ap_features-2023.2.0.tar`

### file list

```diff
@@ -1,65 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:13:51.012506 ap_features-2023.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-08 10:13:49.000000 ap_features-2023.1.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-02-08 10:13:49.000000 ap_features-2023.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-02-08 10:13:49.000000 ap_features-2023.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-08 10:13:49.000000 ap_features-2023.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-02-08 10:13:51.012506 ap_features-2023.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-02-08 10:13:49.000000 ap_features-2023.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:13:51.000506 ap_features-2023.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-02-08 10:13:49.000000 ap_features-2023.1.3/docs/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-02-08 10:13:49.000000 ap_features-2023.1.3/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-08 10:13:49.000000 ap_features-2023.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-02-08 10:13:51.012506 ap_features-2023.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-02-08 10:13:49.000000 ap_features-2023.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:13:50.996506 ap_features-2023.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:13:51.000506 ap_features-2023.1.3/src/c/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/c/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/c/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/c/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:13:51.000506 ap_features-2023.1.3/src/c/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/c/cmake/BuildType.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/c/common.h
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/c/cost_terms.c
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/c/cost_terms.h
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/c/cost_terms_main.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:13:50.996506 ap_features-2023.1.3/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:13:51.004506 ap_features-2023.1.3/src/python/ap_features/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/python/ap_features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/python/ap_features/_c.py
--rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/python/ap_features/_numba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/python/ap_features/average.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/python/ap_features/background.py
--rw-r--r--   0 runner    (1001) docker     (123)    37249 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/python/ap_features/beat.py
--rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/python/ap_features/chopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    28808 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/python/ap_features/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/python/ap_features/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/python/ap_features/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/python/ap_features/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-02-08 10:13:49.000000 ap_features-2023.1.3/src/python/ap_features/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:13:51.008506 ap_features-2023.1.3/src/python/ap_features.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-02-08 10:13:50.000000 ap_features-2023.1.3/src/python/ap_features.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-02-08 10:13:50.000000 ap_features-2023.1.3/src/python/ap_features.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 10:13:50.000000 ap_features-2023.1.3/src/python/ap_features.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 10:13:50.000000 ap_features-2023.1.3/src/python/ap_features.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-08 10:13:50.000000 ap_features-2023.1.3/src/python/ap_features.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-08 10:13:50.000000 ap_features-2023.1.3/src/python/ap_features.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:13:51.008506 ap_features-2023.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:13:50.996506 ap_features-2023.1.3/tests/baseline_images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 10:13:51.012506 ap_features-2023.1.3/tests/baseline_images/test_plot/
--rw-r--r--   0 runner    (1001) docker     (123)    61987 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/baseline_images/test_plot/beats.png
--rw-r--r--   0 runner    (1001) docker     (123)    79471 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/baseline_images/test_plot/beats_aligned.png
--rw-r--r--   0 runner    (1001) docker     (123)    47169 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/baseline_images/test_plot/poincare.png
--rw-r--r--   0 runner    (1001) docker     (123)    52868 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/baseline_images/test_plot/simple_beat.png
--rw-r--r--   0 runner    (1001) docker     (123)    61269 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/baseline_images/test_plot/simple_beat_with_background.png
--rw-r--r--   0 runner    (1001) docker     (123)    66463 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/baseline_images/test_plot/simple_beat_with_pacing.png
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/cost_terms.npy
--rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/data.npy
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/real_data.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/test_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/test_background.py
--rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/test_beat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/test_chopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-02-08 10:13:49.000000 ap_features-2023.1.3/tests/test_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:31:42.718766 ap_features-2023.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-21 09:30:59.000000 ap_features-2023.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-21 09:30:59.000000 ap_features-2023.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-21 09:30:59.000000 ap_features-2023.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-21 09:30:59.000000 ap_features-2023.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-21 09:31:42.714766 ap_features-2023.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-21 09:30:59.000000 ap_features-2023.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:31:42.706766 ap_features-2023.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-21 09:30:59.000000 ap_features-2023.2.0/docs/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-05-21 09:30:59.000000 ap_features-2023.2.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-21 09:30:59.000000 ap_features-2023.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 09:31:42.718766 ap_features-2023.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:31:42.702766 ap_features-2023.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:31:42.706766 ap_features-2023.2.0/src/c/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/c/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/c/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/c/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:31:42.706766 ap_features-2023.2.0/src/c/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/c/cmake/BuildType.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/c/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/c/cost_terms.c
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/c/cost_terms.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/c/cost_terms_main.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:31:42.702766 ap_features-2023.2.0/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:31:42.710766 ap_features-2023.2.0/src/python/ap_features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/python/ap_features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/python/ap_features/_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/python/ap_features/average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/python/ap_features/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37123 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/python/ap_features/beat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/python/ap_features/chopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28479 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/python/ap_features/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/python/ap_features/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/python/ap_features/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/python/ap_features/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-21 09:30:59.000000 ap_features-2023.2.0/src/python/ap_features/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:31:42.710766 ap_features-2023.2.0/src/python/ap_features.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-21 09:31:42.000000 ap_features-2023.2.0/src/python/ap_features.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-21 09:31:42.000000 ap_features-2023.2.0/src/python/ap_features.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 09:31:42.000000 ap_features-2023.2.0/src/python/ap_features.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-21 09:31:42.000000 ap_features-2023.2.0/src/python/ap_features.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 09:31:42.000000 ap_features-2023.2.0/src/python/ap_features.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:31:42.714766 ap_features-2023.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:31:42.702766 ap_features-2023.2.0/tests/baseline_images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 09:31:42.714766 ap_features-2023.2.0/tests/baseline_images/test_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)    61987 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/baseline_images/test_plot/beats.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79471 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/baseline_images/test_plot/beats_aligned.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47169 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/baseline_images/test_plot/poincare.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52868 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/baseline_images/test_plot/simple_beat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61269 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/baseline_images/test_plot/simple_beat_with_background.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66463 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/baseline_images/test_plot/simple_beat_with_pacing.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/cost_terms.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/data.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/real_data.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/test_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/test_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/test_beat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/test_chopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-21 09:30:59.000000 ap_features-2023.2.0/tests/test_plot.py
```

### Comparing `ap_features-2023.1.3/CONTRIBUTING.md` & `ap_features-2023.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/LICENSE` & `ap_features-2023.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/docs/INSTALL.md` & `ap_features-2023.2.0/docs/INSTALL.md`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,20 @@
 will always install the most recent stable release.
 
 If you don\'t have [pip](https://pip.pypa.io) installed, this [Python
 installation
 guide](http://docs.python-guide.org/en/latest/starting/installation/)
 can guide you through the process.
 
+## Conda
+You can also install `ap_features` using `conda`
+```
+conda install -c conda-forge ap_features
+```
+
 ## From sources
 
 The sources for Action Potential features can be downloaded from the
 [Github repo](https://github.com/ComputationalPhysiology/ap_features).
 
 You can either clone the public repository:
 
@@ -66,31 +72,25 @@
 
 Once you have a copy of the source, you can install it with:
 
 ```Shell
 $ python -m pip install .
 ```
 
-There is also a way to install the package using the Makefile, i.e
-
-```Shell
-$ make install
-```
 
 ### For developers
 
 If you plan to develop this package you should also make sure to install
 the development dependencies using the command
 
 ```Shell
 python -m pip install -e ".[dev]"
 ```
 
-In addition you should also make sure to install the pre-commit hook. All of this can be installed by
-executing the command
-
-```Shell
-$ make dev
-```
-
 Note that this will also install the main package in editable mode,
 which is nice when developing.
+
+In addition you should also make sure to install the pre-commit hook
+
+```
+pre-commit install
+```
```

### Comparing `ap_features-2023.1.3/docs/logo.png` & `ap_features-2023.2.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/src/c/.clang-format` & `ap_features-2023.2.0/src/c/.clang-format`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/src/c/CMakeLists.txt` & `ap_features-2023.2.0/src/c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/src/c/cmake/BuildType.cmake` & `ap_features-2023.2.0/src/c/cmake/BuildType.cmake`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/src/c/cost_terms.c` & `ap_features-2023.2.0/src/c/cost_terms.c`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/src/c/cost_terms_main.c` & `ap_features-2023.2.0/src/c/cost_terms_main.c`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/src/python/ap_features/__init__.py` & `ap_features-2023.2.0/src/python/ap_features/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,38 +6,40 @@
 
 from . import (
     background,
     chopping,
     features,
     average,
     filters,
-    lib,
     utils,
-    _c,
     _numba,
     plot,
+    testing,
 )
-from ._c import NUM_COST_TERMS
+
 from ._numba import transpose_trace_array
 from .beat import Beat, Beats, Trace, BeatCollection, StateCollection, State
 from .features import all_cost_terms, apd, apd_up_xy, cost_terms, cost_terms_trace
-from .utils import Backend, list_cost_function_terms, list_cost_function_terms_trace
+from .utils import (
+    Backend,
+    list_cost_function_terms,
+    list_cost_function_terms_trace,
+    NUM_COST_TERMS,
+)
 from .average import average_and_interpolate
 from .background import BackgroundCorrection as BC
 
 
 def set_log_level(level=_logging.INFO):
     for logger in [
-        _c.logger,
         _numba.logger,
         background.logger,
         chopping.logger,
         features.logger,
         filters.logger,
-        lib.logger,
         utils.logger,
     ]:
         logger.setLevel(level)
 
 
 set_log_level()
 
@@ -63,8 +65,9 @@
     "StateCollection",
     "State",
     "average",
     "average_and_interpolate",
     "filters",
     "BC",
     "plot",
+    "testing",
 ]
```

### Comparing `ap_features-2023.1.3/src/python/ap_features/average.py` & `ap_features-2023.2.0/src/python/ap_features/average.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/src/python/ap_features/background.py` & `ap_features-2023.2.0/src/python/ap_features/background.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,15 @@
         corrected=corrected,
         background=bkg,
         F0=F0,
         method=method,
     )
 
 
-def full_background_correction(
-    x: Array, y: Array, filter_kernel_size=0, **kwargs
-) -> Background:
+def full_background_correction(x: Array, y: Array, filter_kernel_size=0, **kwargs) -> Background:
     r"""Perform at background correction.
     First estimate background :math:`b`, and let
     :math:`F_0 = b(0)`. The corrected background is
     then :math:`\frac{y - b}{F_0}`. Additional argument
     can be passed to background corrected algorithm as
     keyword arguments.
```

### Comparing `ap_features-2023.1.3/src/python/ap_features/beat.py` & `ap_features-2023.2.0/src/python/ap_features/beat.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     __slots__ = ("_t", "_y", "_pacing", "_backend")
 
     def __init__(
         self,
         y: Array,
         t: Optional[Array],
         pacing: Optional[Array] = None,
-        backend: Backend = Backend.c,
+        backend: Backend = Backend.numba,
     ) -> None:
         if t is None:
             t = np.arange(len(y))
         self._t = utils.numpyfy(t)
         self._y = utils.numpyfy(y)
         if pacing is None:
             pacing = np.zeros_like(self._t)  # type: ignore
@@ -171,15 +171,15 @@
     def __init__(
         self,
         y: Array,
         t: Array,
         pacing: Optional[Array] = None,
         y_rest: Optional[float] = None,
         parent: Optional["Beats"] = None,
-        backend: Backend = Backend.c,
+        backend: Backend = Backend.numba,
         beat_number: Optional[int] = None,
     ) -> None:
         super().__init__(y, t, pacing=pacing, backend=backend)
         msg = (
             "Expected shape of 't' and 'y' to be the same. got "
             f"{self._t.shape}(t) and {self._y.shape}(y)"
         )
@@ -556,17 +556,14 @@
 
         Arguments
         ---------
         factor_x: int
             First APD line (value between 0 and 100)
         factor_y: int
             Second APD line (value between 0 and 100)
-        backend : utils.Backend, optional
-            Which backend to use by default Backend.python.
-            Choices, 'python', 'c', 'numba'
 
         Returns
         -------
         float:
             The time between `factor_x` to `factor_y`
 
         """
@@ -594,19 +591,15 @@
     if len(beats) == 0:
         return beats
 
     apd_points = [b.apd_point(apd_point) for b in beats]
     bad_beats = [np.isclose(*p) for p in apd_points]
 
     # Make sure all beats start at time zero
-    xs = [
-        beat.t - ap[0]
-        for (beat, ap, bad) in zip(beats, apd_points, bad_beats)
-        if not bad
-    ]
+    xs = [beat.t - ap[0] for (beat, ap, bad) in zip(beats, apd_points, bad_beats) if not bad]
     ys = [beat.y for (beat, bad) in zip(beats, bad_beats) if not bad]
 
     # Make them start at zero
     min_x = np.min([np.min(xi) for xi in xs])
     xs = [xi - min_x for xi in xs]
 
     return [Beat(yi, xi, parent=parent) for (yi, xi) in zip(ys, xs)]
@@ -755,15 +748,15 @@
         self,
         y: Array,
         t: Array,
         pacing: Optional[Array] = None,
         background_correction_method: BC = BC.none,
         zero_index: Optional[int] = None,
         background_correction_kernel: int = 0,
-        backend: Backend = Backend.c,
+        backend: Backend = Backend.numba,
         intervals: Optional[List[chopping.Interval]] = None,
         chopping_options: Optional[Dict[str, float]] = None,
     ) -> None:
         """Initializer for `Beats` class
 
         Parameters
         ----------
@@ -781,16 +774,16 @@
             See `ap_features.background.correct_background` for more info.
         zero_index : Optional[int], optional
             Index where the value should be forced to be zero, by default None.
             This will make sure that the array at the given index is zero, and
             by subtracting the value at that index from all other values in the
             array.
         backend : Backend, optional
-            Backend to use for heavy computations, by default Backend.c.
-            Possible options are "c", "numba" and "python". Note that
+            Backend to use for heavy computations, by default Backend.numba.
+            Possible options are "numba" and "python". Note that
             most functions will be implemented in python / numpy anyway.
         intervals : Optional[List[chopping.Interval]], optional
             Optional ist of tuples containing start and ends of each beat
             to be used for chopping, by default None.
         chopping_options : Optional[Dict[str, float]], optional
             Parameters to be used for chopping trace into individual beats,
             by default None. See `ap_features.chopping.chop_data_without_pacing`
@@ -1091,26 +1084,24 @@
     def __init__(
         self,
         y: Array,
         t: Array,
         pacing: Optional[Array] = None,
         mask: Optional[Array] = None,
         parent: Optional["BeatSeriesCollection"] = None,
-        backend: Backend = Backend.c,
+        backend: Backend = Backend.numba,
     ) -> None:
         super().__init__(y, t, pacing=pacing, backend=backend)
         self._parent = parent
         msg = (
             "Expected first dimension of 'y' to be the same as shape of 't' "
             f", got {self._t.size}(t) and {self._y.shape[0]}(y)"
         )
         assert self.t.size == self.y.shape[0], msg
-        assert (
-            len(self.y.shape) == 2
-        ), f"Expected shape of y to be 2D, got {len(self.y.shape)}D"
+        assert len(self.y.shape) == 2, f"Expected shape of y to be 2D, got {len(self.y.shape)}D"
 
     @property
     def num_traces(self):
         return self.y.shape[-1]
 
     @property
     def parent(self) -> Optional["BeatSeriesCollection"]:
@@ -1161,40 +1152,43 @@
 
 class State(Trace):
     def __init__(
         self,
         y: Array,
         t: Optional[Array],
         pacing: Optional[Array] = None,
-        backend: Backend = Backend.c,
+        backend: Backend = Backend.numba,
     ) -> None:
         super().__init__(y, t, pacing=pacing, backend=backend)
 
         msg = (
             "Expected first dimension of 'y' to be the same as shape of 't' "
             f", got {self._t.size}(t) and {self._y.shape[0]}(y)"
         )
         assert self.t.size == self.y.shape[0], msg
-        assert (
-            len(self.y.shape) == 2
-        ), f"Expected shape of y to be D, got {len(self.y.shape)}D"
+        assert len(self.y.shape) == 2, f"Expected shape of y to be D, got {len(self.y.shape)}D"
 
     @property
     def num_states(self):
         return self.y.shape[1]
 
     def __getitem__(self, k):
         return self.y[:, k]
 
     @property
     def cost_terms(self):
         if self.num_states != 2:
             raise NotImplementedError
 
-        return features.cost_terms(v=self[0], ca=self[1], t_v=self.t, t_ca=self.t)
+        return features.cost_terms(
+            v=np.ascontiguousarray(self[0]),
+            ca=np.ascontiguousarray(self[1]),
+            t_v=self.t,
+            t_ca=self.t,
+        )
 
 
 class StateCollection(Trace):
     def __init__(
         self,
         y: Array,
         t: Array,
@@ -1207,17 +1201,15 @@
         self._parent = parent
 
         msg = (
             "Expected first dimension of 'y' to be the same as shape of 't' "
             f", got {self._t.size}(t) and {self._y.shape[0]}(y)"
         )
         assert self.t.size == self.y.shape[0], msg
-        assert (
-            len(self.y.shape) == 3
-        ), f"Expected shape of y to be 3D, got {len(self.y.shape)}D"
+        assert len(self.y.shape) == 3, f"Expected shape of y to be 3D, got {len(self.y.shape)}D"
         self.mask = mask
 
     @property
     def mask(self) -> Optional[Array]:
         return self._mask
 
     @mask.setter
```

### Comparing `ap_features-2023.1.3/src/python/ap_features/chopping.py` & `ap_features-2023.2.0/src/python/ap_features/chopping.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/src/python/ap_features/features.py` & `ap_features-2023.2.0/src/python/ap_features/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 
 import numpy as np
 from scipy.interpolate import UnivariateSpline
 
-from . import _c
 from . import _numba
 from . import utils
 from .utils import _check_factor
 from .utils import Array
 from .utils import Backend
 from .utils import numpyfy
 
@@ -58,15 +57,15 @@
     v_r : Optional[float], optional
         Resting value, by default None. Only applicable for python Backend.
     use_spline : bool, optional
         Use spline interpolation, by default True.
         Only applicable for python Backend.
     backend : utils.Backend, optional
         Which backend to use by default Backend.python.
-        Choices, 'python', 'c', 'numba'
+        Choices, 'python', 'numba'
 
 
 
     Returns
     -------
     float
         The triangulation
@@ -115,15 +114,15 @@
     v_r : Optional[float], optional
         Resting value, by default None. Only applicable for python Backend.
     use_spline : bool, optional
         Use spline interpolation, by default True.
         Only applicable for python Backend.
     backend : utils.Backend, optional
         Which backend to use by default Backend.python.
-        Choices, 'python', 'c', 'numba'
+        Choices, 'python', 'numba'
 
 
     Returns
     -------
     float
         The action potential duration
 
@@ -188,18 +187,15 @@
     if backend == Backend.python:
         try:
             x1, x2 = apd_point(factor=factor, V=y, t=x, v_r=v_r, use_spline=use_spline)
         except RuntimeError:
             # Return a number that indicate that something went wrong
             return -1
         return x2 - x1
-    elif backend == Backend.c:
-        return _c.apd(y=y, t=x, factor=factor)
     else:
-        _numba.check_numba()
         return _numba.apd(V=y, T=x, factor=factor)
 
 
 def sign_change(y: np.ndarray) -> np.ndarray:
     s = np.sign(y)
 
     # If we have many zero values just use these instead
@@ -337,15 +333,15 @@
         The time stamps
     y : Array
         The signal
     a : float, optional
         The value for which you want to estimate the time decay, by default 0.75
     backend : utils.Backend, optional
         Which backend to use by default Backend.python.
-        Choices, 'python', 'c', 'numba'
+        Choices, 'python', 'numba'
 
     Returns
     -------
     float
         Decay time
 
     """
@@ -355,25 +351,24 @@
     Y = UnivariateSpline(x, utils.normalize_signal(y) - a, s=0, k=3)
     t_max = x[int(np.argmax(y))]
     r = Y.roots()
     if len(r) >= 2:
         t_a = r[1]
     elif len(r) == 1:
         logger.warning(
-            (
-                "Only one zero was found when computing tau{}. " "Result might be wrong"
-            ).format(int(a * 100)),
+            ("Only one zero was found when computing tau{}. " "Result might be wrong").format(
+                int(a * 100),
+            ),
         )
         t_a = r[0]
     else:
         logger.warning(
-            (
-                "No zero found when computing tau{}. "
-                "Return the value of time to peak"
-            ).format(int(a * 100)),
+            ("No zero found when computing tau{}. " "Return the value of time to peak").format(
+                int(a * 100),
+            ),
         )
         t_a = x[0]
 
     return t_a - t_max
 
 
 def time_to_peak(
@@ -394,15 +389,15 @@
         The signal
     x : Array
         The time stamps
     pacing : Optional[Array], optional
         The pacing amplitude, by default None
     backend : utils.Backend, optional
         Which backend to use by default Backend.python.
-        Choices, 'python', 'c', 'numba'
+        Choices, 'python', 'numba'
 
     Returns
     -------
     float
         Time to peak
 
     """
@@ -422,20 +417,15 @@
 
     t_max = x[int(np.argmax(y))]
     if pacing is None:
         t_start = x[0]
     else:
         try:
             start_idx = (
-                next(
-                    i
-                    for i, p in enumerate(np.diff(np.array(pacing).astype(float)))
-                    if p > 0
-                )
-                + 1
+                next(i for i, p in enumerate(np.diff(np.array(pacing).astype(float))) if p > 0) + 1
             )
         except StopIteration:
             start_idx = 0
     t_start = x[start_idx]
 
     return t_max - t_start
 
@@ -457,15 +447,15 @@
         The time stamps
     y : Array
         The signal
     a : float, optional
         Fraction of signal amplitude, by default 0.8
     backend : utils.Backend, optional
         Which backend to use by default Backend.python.
-        Choices, 'python', 'c', 'numba'
+        Choices, 'python', 'numba'
 
     Returns
     -------
     float
         The upstroke value
 
     Raises
@@ -482,25 +472,23 @@
     Y = UnivariateSpline(x, utils.normalize_signal(y) - (1 - a), s=0, k=3)
     t_max = x[int(np.argmax(y))]
     r = Y.roots()
     if len(r) >= 1:
         if len(r) == 1:
             logger.warning(
                 (
-                    "Only one zero was found when computing upstroke{}. "
-                    "Result might be wrong"
+                    "Only one zero was found when computing upstroke{}. " "Result might be wrong"
                 ).format(int(a * 100)),
             )
         t_a = r[0]
     else:
         logger.warning(
-            (
-                "No zero found when computing upstroke{}. "
-                "Return the value of time to peak"
-            ).format(int(a * 100)),
+            ("No zero found when computing upstroke{}. " "Return the value of time to peak").format(
+                int(a * 100),
+            ),
         )
         t_a = x[0]
 
     return t_max - t_a
 
 
 def beating_frequency(times: List[Array], unit: str = "ms") -> float:
@@ -613,15 +601,15 @@
         The trace
     from_APD: int
         First APD line (value between 0 and 100)
     to_APD: int
         Second APD line (value between 0 and 100)
     backend : utils.Backend, optional
         Which backend to use by default Backend.python.
-        Choices, 'python', 'c', 'numba'
+        Choices, 'python', 'numba'
 
     Returns
     -------
     float:
         The time between `factor_x` to `factor_y`
 
 
@@ -629,18 +617,15 @@
     """
     _check_factor(factor_x)
     _check_factor(factor_y)
 
     y = numpyfy(y)
     t = numpyfy(t)
 
-    if backend == Backend.c:
-        return _c.apd_up_xy(y=y, t=t, factor_x=factor_x, factor_y=factor_y)
     if backend == Backend.numba:
-        _numba.check_numba()
         return _numba.apd_up_xy(y=y, t=t, factor_x=factor_x, factor_y=factor_y)
 
     y_norm = utils.normalize_signal(y)
 
     y_from = UnivariateSpline(t, y_norm - factor_x / 100, s=0, k=3)
     t_from = y_from.roots()[0]
 
@@ -1007,61 +992,65 @@
 
     y_smooth = gaussian_filter1d(y_tmp / np.max(y_tmp), sigma)
     peaks, props = find_peaks(y_smooth, prominence=prominence_level)
 
     return len(peaks) > 0, None if len(peaks) == 0 else int(peaks[0] + idx_max)
 
 
-def cost_terms_trace(y: Array, t: Array, backend: Backend = Backend.c) -> np.ndarray:
+def cost_terms_trace(
+    y: Array,
+    t: Array,
+    backend: Backend = Backend.numba,
+) -> np.ndarray:
     y = numpyfy(y)
     t = numpyfy(t)
 
     if backend == Backend.python:
         logger.warning(
             "Method currently not implemented for python backend (and will probably not be)",
         )
 
     if backend == Backend.numba:
-        _numba.check_numba()
         return _numba.cost_terms_trace(y=y, t=t)
 
-    # Use C backend
-    return _c.cost_terms_trace(y=y, t=t)
+    raise ValueError(f"Unknown backend {backend}")
+    # # Use C backend
+    # return _c.cost_terms_trace(y=y, t=t)
 
 
 def cost_terms(
     v: Array,
     ca: Array,
     t_v: Array,
     t_ca: Array,
-    backend: Backend = Backend.c,
+    backend: Backend = Backend.numba,
 ) -> np.ndarray:
     v = numpyfy(v)
     t_v = numpyfy(t_v)
     ca = numpyfy(ca)
     t_ca = numpyfy(t_ca)
 
     if backend == Backend.python:
         logger.warning(
             "Method currently not implemented for python backend (and will probably not be)",
         )
 
     if backend == Backend.numba:
-        _numba.check_numba()
         return _numba.cost_terms(v=v, ca=ca, t_v=t_v, t_ca=t_ca)
 
     # Use C backend
-    return _c.cost_terms(v=v, ca=ca, t_v=t_v, t_ca=t_ca)
+    # return _c.cost_terms(v=v, ca=ca, t_v=t_v, t_ca=t_ca)
+    raise ValueError(f"Unknown backend {backend}")
 
 
 def all_cost_terms(
     arr: np.ndarray,
     t: np.ndarray,
     mask: Optional[np.ndarray] = None,
-    backend: Backend = Backend.c,
+    backend: Backend = Backend.numba,
     normalize_time: bool = True,
 ) -> np.ndarray:
     arr = numpyfy(arr)
     t = numpyfy(t)
     if not isinstance(arr, np.ndarray):
         raise TypeError(f"Expected 'arr' to be of type numpy.ndarray got {type(arr)}")
     if not isinstance(t, np.ndarray):
@@ -1073,13 +1062,14 @@
     if normalize_time:
         t = t - t[0]
 
     if backend == Backend.python:
         logger.warning(
             "Method currently not implemented for python backend (and will probably not be)",
         )
+
     if backend == Backend.numba:
-        _numba.check_numba()
         return _numba.all_cost_terms(arr=arr, t=t, mask=mask)
 
     # Use C backend
-    return _c.all_cost_terms(arr=arr, t=t, mask=mask)
+    # return _c.all_cost_terms(arr=arr, t=t, mask=mask)
+    raise ValueError(f"Unknown backend {backend}")
```

### Comparing `ap_features-2023.1.3/src/python/ap_features/filters.py` & `ap_features-2023.2.0/src/python/ap_features/filters.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/src/python/ap_features/plot.py` & `ap_features-2023.2.0/src/python/ap_features/plot.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/src/python/ap_features/utils.py` & `ap_features-2023.2.0/src/python/ap_features/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 import numpy as np
 from scipy.interpolate import UnivariateSpline
 
 logger = logging.getLogger(__name__)
 
 Array = Union[np.ndarray, List[float], Sequence[float]]
 
+NUM_COST_TERMS = 60
+
 
 class Backend(str, Enum):
-    c = "c"
+    # c = "c"
     numba = "numba"
     python = "python"
 
 
 def _check_factor(factor: float) -> None:
     if not 0 < factor < 100:
         raise ValueError(f"Factor has to be between 0 and 100, got {factor}")
```

### Comparing `ap_features-2023.1.3/src/python/ap_features.egg-info/SOURCES.txt` & `ap_features-2023.2.0/src/python/ap_features.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 AUTHORS.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 docs/INSTALL.md
 docs/logo.png
 src/c/.clang-format
 src/c/CMakeLists.txt
 src/c/Makefile
 src/c/common.h
 src/c/cost_terms.c
 src/c/cost_terms.h
 src/c/cost_terms_main.c
 src/c/cmake/BuildType.cmake
 src/python/ap_features/__init__.py
-src/python/ap_features/_c.py
 src/python/ap_features/_numba.py
 src/python/ap_features/average.py
 src/python/ap_features/background.py
 src/python/ap_features/beat.py
 src/python/ap_features/chopping.py
 src/python/ap_features/features.py
 src/python/ap_features/filters.py
-src/python/ap_features/lib.py
 src/python/ap_features/plot.py
+src/python/ap_features/testing.py
 src/python/ap_features/utils.py
 src/python/ap_features.egg-info/PKG-INFO
 src/python/ap_features.egg-info/SOURCES.txt
 src/python/ap_features.egg-info/dependency_links.txt
-src/python/ap_features.egg-info/not-zip-safe
 src/python/ap_features.egg-info/requires.txt
 src/python/ap_features.egg-info/top_level.txt
 tests/conftest.py
 tests/cost_terms.npy
 tests/data.npy
 tests/real_data.npy
 tests/test_average.py
```

### Comparing `ap_features-2023.1.3/tests/baseline_images/test_plot/beats.png` & `ap_features-2023.2.0/tests/baseline_images/test_plot/beats.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/baseline_images/test_plot/beats_aligned.png` & `ap_features-2023.2.0/tests/baseline_images/test_plot/beats_aligned.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/baseline_images/test_plot/poincare.png` & `ap_features-2023.2.0/tests/baseline_images/test_plot/poincare.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/baseline_images/test_plot/simple_beat.png` & `ap_features-2023.2.0/tests/baseline_images/test_plot/simple_beat.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/baseline_images/test_plot/simple_beat_with_background.png` & `ap_features-2023.2.0/tests/baseline_images/test_plot/simple_beat_with_background.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/baseline_images/test_plot/simple_beat_with_pacing.png` & `ap_features-2023.2.0/tests/baseline_images/test_plot/simple_beat_with_pacing.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/cost_terms.npy` & `ap_features-2023.2.0/tests/cost_terms.npy`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/data.npy` & `ap_features-2023.2.0/tests/data.npy`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/real_data.npy` & `ap_features-2023.2.0/tests/real_data.npy`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/test_average.py` & `ap_features-2023.2.0/tests/test_average.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/test_background.py` & `ap_features-2023.2.0/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/test_beat.py` & `ap_features-2023.2.0/tests/test_beat.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/test_chopping.py` & `ap_features-2023.2.0/tests/test_chopping.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/test_features.py` & `ap_features-2023.2.0/tests/test_features.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,62 +108,42 @@
         ([0, 0, 1, 0], [0, 1, 2, 3], [0, 0, 0, 0], 2),
     ],
 )
 def test_time_to_peak_with_pacing(y, x, p, expected_ttp):
     assert apf.features.time_to_peak(y, x, pacing=p) == expected_ttp
 
 
-@pytest.mark.parametrize("backend", ("c", "numba"))
-def test_all_cost_terms(synthetic_data, backend):
+def test_all_cost_terms(synthetic_data):
     arr, t, expected_cost = synthetic_data
     arrs = np.expand_dims(arr, axis=0)
-    cost = apf.all_cost_terms(arrs.T, t, backend=backend).squeeze()
+
+    cost = apf.all_cost_terms(
+        np.ascontiguousarray(arrs.T),
+        t,
+        backend="numba",
+    ).squeeze()
 
     lst = apf.list_cost_function_terms()
     up_inds = np.where(["APD_up" in item or "CaD_up" in item for item in lst])[0]
     cost = np.delete(cost, up_inds)
 
     assert np.all(cost - expected_cost < 1e-10)
 
 
-def test_cost_terms_trace(synthetic_data):
-    arr, t, expected_cost = synthetic_data
-    V = np.ascontiguousarray(arr[0, :])
-
-    cost_terms_c = apf.cost_terms_trace(V, t, backend="c")
-    cost_terms_py = apf.cost_terms_trace(V, t, backend="numba")
-
-    lst = apf.list_cost_function_terms_trace()
-    inds = np.where(["int_30" in item for item in lst])[0]
-    x = np.delete(np.arange(len(lst)), inds)
-
-    assert np.all(np.abs(cost_terms_c[x] - cost_terms_py[x]) < 1e-10)
-
-
-@pytest.mark.parametrize("factor, backend", it.product((40, 60, 80), ("c", "numba")))
+@pytest.mark.parametrize("factor, backend", it.product((40, 60, 80), ("numba",)))
 def test_apd_equivalence(factor, backend, synthetic_data):
     arr, t, expected_cost = synthetic_data
     V = np.ascontiguousarray(arr[0, :])
     apd_py = apf.apd(V=V, t=t, factor=factor, backend="python")
     apd_x = apf.apd(V=V, t=t, factor=factor, backend=backend)
 
     # We expect some difference here, but no more than 1ms
     assert abs(apd_x - apd_py) < 1
 
 
-@pytest.mark.parametrize("factor", (40, 60, 80))
-def test_apd_equivalence_c_numba(factor, synthetic_data):
-    arr, t, expected_cost = synthetic_data
-    V = np.ascontiguousarray(arr[0, :])
-    apd_numba = apf.apd(V=V, t=t, factor=factor, backend="numba")
-    apd_c = apf.apd(V=V, t=t, factor=factor, backend="c")
-
-    assert abs(apd_c - apd_numba) < 1e-10
-
-
 @pytest.mark.parametrize(
     "key, index0, index4",
     (("", "max", "APD10"), ("V", "V_max", "APD10"), ("Ca", "Ca_max", "CaD10")),
 )
 def test_list_cost_function_terms_trace(key, index0, index4):
     lst = apf.list_cost_function_terms_trace(key)
     assert lst[0] == index0
```

### Comparing `ap_features-2023.1.3/tests/test_filters.py` & `ap_features-2023.2.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.1.3/tests/test_plot.py` & `ap_features-2023.2.0/tests/test_plot.py`

 * *Files identical despite different names*

