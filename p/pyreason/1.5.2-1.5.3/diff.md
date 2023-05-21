# Comparing `tmp/pyreason-1.5.2.tar.gz` & `tmp/pyreason-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.5.2.tar", last modified: Wed May 17 09:42:38 2023, max compression
+gzip compressed data, was "pyreason-1.5.3.tar", last modified: Sun May 21 04:55:18 2023, max compression
```

## Comparing `pyreason-1.5.2.tar` & `pyreason-1.5.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.437632 pyreason-1.5.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-05-17 09:42:23.000000 pyreason-1.5.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-17 09:42:23.000000 pyreason-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-17 09:42:38.437632 pyreason-1.5.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-05-17 09:42:23.000000 pyreason-1.5.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.425632 pyreason-1.5.2/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.425632 pyreason-1.5.2/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.429632 pyreason-1.5.2/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    27119 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.429632 pyreason-1.5.2/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.429632 pyreason-1.5.2/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.429632 pyreason-1.5.2/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.433632 pyreason-1.5.2/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/facts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.433632 pyreason-1.5.2/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    70954 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.433632 pyreason-1.5.2/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.433632 pyreason-1.5.2/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.437632 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5992 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10901 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.437632 pyreason-1.5.2/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.437632 pyreason-1.5.2/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.437632 pyreason-1.5.2/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9056 2023-05-17 09:42:23.000000 pyreason-1.5.2/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 09:42:38.425632 pyreason-1.5.2/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-17 09:42:38.000000 pyreason-1.5.2/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-17 09:42:38.000000 pyreason-1.5.2/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 09:42:38.000000 pyreason-1.5.2/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 09:42:38.000000 pyreason-1.5.2/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 09:42:38.000000 pyreason-1.5.2/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 09:42:38.437632 pyreason-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-17 09:42:23.000000 pyreason-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.832931 pyreason-1.5.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-05-21 04:55:07.000000 pyreason-1.5.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-21 04:55:07.000000 pyreason-1.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-21 04:55:18.832931 pyreason-1.5.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-05-21 04:55:07.000000 pyreason-1.5.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.824931 pyreason-1.5.3/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.824931 pyreason-1.5.3/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.824931 pyreason-1.5.3/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27121 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/facts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    71082 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10909 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.828931 pyreason-1.5.3/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.832931 pyreason-1.5.3/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4564 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4233 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9058 2023-05-21 04:55:07.000000 pyreason-1.5.3/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:55:18.824931 pyreason-1.5.3/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-21 04:55:18.000000 pyreason-1.5.3/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-21 04:55:18.000000 pyreason-1.5.3/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 04:55:18.000000 pyreason-1.5.3/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-21 04:55:18.000000 pyreason-1.5.3/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 04:55:18.000000 pyreason-1.5.3/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 04:55:18.832931 pyreason-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-21 04:55:07.000000 pyreason-1.5.3/setup.py
```

### Comparing `pyreason-1.5.2/LICENSE.md` & `pyreason-1.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/PKG-INFO` & `pyreason-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.5.2
+Version: 1.5.3
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.5.2/README.md` & `pyreason-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/__init__.py` & `pyreason-1.5.3/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.5.3/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.5.3/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.5.3/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/pyreason.py` & `pyreason-1.5.3/pyreason/pyreason.py`

 * *Files 0% similar despite different names*

```diff
@@ -465,15 +465,15 @@
     bnd = interval.closed(1, 1)
     ann_fn = ''
     ann_label = label.Label('')
 
     weights = np.ones(len(body_predicates), dtype=np.float64)
     weights = np.append(weights, 0)
 
-    r = rule.Rule(name, target, target_criteria, numba.types.int8(0), neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges)
+    r = rule.Rule(name, target, target_criteria, numba.types.uint16(0), neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges)
 
     # Add to collection of rules
     if __rules is None:
         __rules = numba.typed.List.empty_list(rule.rule_type)
     __rules.append(r)
```

### Comparing `pyreason-1.5.2/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.5.3/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/args.py` & `pyreason-1.5.3/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/components/world.py` & `pyreason-1.5.3/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/diffuse.py` & `pyreason-1.5.3/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.5.3/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/facts/fact_node.py` & `pyreason-1.5.3/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.5.3/pyreason/scripts/interpretation/interpretation.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,26 +38,26 @@
 		self.prev_reasoning_data = numba.typed.List([0, 0])
 
 		# Initialize list of tuples for rules/facts to be applied, along with all the ground atoms that fired the rule. One to One correspondence between rules_to_be_applied_node and rules_to_be_applied_node_trace if atom_trace is true
 		self.rules_to_be_applied_node_trace = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), numba.types.string)))
 		self.rules_to_be_applied_edge_trace = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), numba.types.string)))
 		self.facts_to_be_applied_node_trace = numba.typed.List.empty_list(numba.types.string)
 		self.facts_to_be_applied_edge_trace = numba.typed.List.empty_list(numba.types.string)
-		self.rules_to_be_applied_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, node_type, label.label_type, interval.interval_type, numba.types.boolean)))
-		self.rules_to_be_applied_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, edge_type, label.label_type, interval.interval_type, numba.types.boolean)))
-		self.facts_to_be_applied_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, node_type, label.label_type, interval.interval_type, numba.types.boolean, numba.types.boolean)))
-		self.facts_to_be_applied_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, edge_type, label.label_type, interval.interval_type, numba.types.boolean, numba.types.boolean)))
+		self.rules_to_be_applied_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.uint16, node_type, label.label_type, interval.interval_type, numba.types.boolean)))
+		self.rules_to_be_applied_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.uint16, edge_type, label.label_type, interval.interval_type, numba.types.boolean)))
+		self.facts_to_be_applied_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.uint16, node_type, label.label_type, interval.interval_type, numba.types.boolean, numba.types.boolean)))
+		self.facts_to_be_applied_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.uint16, edge_type, label.label_type, interval.interval_type, numba.types.boolean, numba.types.boolean)))
 		self.edges_to_be_added_node_rule = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(node_type), numba.types.ListType(node_type), label.label_type)))
 		self.edges_to_be_added_edge_rule = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(node_type), numba.types.ListType(node_type), label.label_type)))
 
 		# Keep track of all the rules that have affected each node/edge at each timestep/fp operation, and all ground atoms that have affected the rules as well. Keep track of previous bounds and name of the rule/fact here
 		self.rule_trace_node_atoms = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), interval.interval_type, numba.types.string)))
 		self.rule_trace_edge_atoms = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), interval.interval_type, numba.types.string)))
-		self.rule_trace_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, numba.types.int8, node_type, label.label_type, interval.interval_type)))
-		self.rule_trace_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, numba.types.int8, edge_type, label.label_type, interval.interval_type)))
+		self.rule_trace_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.uint16, numba.types.uint16, node_type, label.label_type, interval.interval_type)))
+		self.rule_trace_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.uint16, numba.types.uint16, edge_type, label.label_type, interval.interval_type)))
 
 		# Nodes and edges of the graph
 		self.nodes = numba.typed.List(self.graph.nodes())
 		self.edges = numba.typed.List(self.graph.edges())
 
 		# Make sure they are correct type
 		if len(self.available_labels_node)==0:
@@ -132,23 +132,23 @@
 	def _init_facts(facts_node, facts_edge, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, atom_trace):
 		max_time = 0
 		for fact in facts_node:
 			for t in range(fact.get_time_lower(), fact.get_time_upper() + 1):
 				max_time = max(max_time, t)
 				name = fact.get_name()
 				graph_attribute = True if name=='graph-attribute-fact' else False
-				facts_to_be_applied_node.append((numba.types.int8(t), fact.get_component(), fact.get_label(), fact.get_bound(), fact.static, graph_attribute))
+				facts_to_be_applied_node.append((numba.types.uint16(t), fact.get_component(), fact.get_label(), fact.get_bound(), fact.static, graph_attribute))
 				if atom_trace:
 					facts_to_be_applied_node_trace.append(fact.get_name())
 		for fact in facts_edge:
 			for t in range(fact.get_time_lower(), fact.get_time_upper() + 1):
 				max_time = max(max_time, t)
 				name = fact.get_name()
 				graph_attribute = True if name=='graph-attribute-fact' else False
-				facts_to_be_applied_edge.append((numba.types.int8(t), fact.get_component(), fact.get_label(), fact.get_bound(), fact.static, graph_attribute))
+				facts_to_be_applied_edge.append((numba.types.uint16(t), fact.get_component(), fact.get_label(), fact.get_bound(), fact.static, graph_attribute))
 				if atom_trace:
 					facts_to_be_applied_edge_trace.append(fact.get_name())
 		return max_time
 
 	def _start_fp(self, rules, max_facts_time, verbose):
 		fp_cnt, t = self.reason(self.interpretations_node, self.interpretations_edge, self.tmax, self.prev_reasoning_data, rules, self.nodes, self.edges, self.neighbors, self.rules_to_be_applied_node, self.rules_to_be_applied_edge, self.edges_to_be_added_node_rule, self.edges_to_be_added_edge_rule, self.rules_to_be_applied_node_trace, self.rules_to_be_applied_edge_trace, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.available_labels_node, self.available_labels_edge, self.specific_node_labels, self.specific_edge_labels, self.ipl, self.rule_trace_node, self.rule_trace_edge, self.rule_trace_node_atoms, self.rule_trace_edge_atoms, self.reverse_graph, self.atom_trace, self.save_graph_attributes_to_rule_trace, self.canonical, self.inconsistency_check, max_facts_time, self._convergence_mode, self._convergence_delta, verbose)
 		self.time = t - 1
@@ -214,24 +214,24 @@
 			for i in range(len(facts_to_be_applied_node)):
 				if facts_to_be_applied_node[i][0]==t:
 					comp, l, bnd, static, graph_attribute = facts_to_be_applied_node[i][1], facts_to_be_applied_node[i][2], facts_to_be_applied_node[i][3], facts_to_be_applied_node[i][4], facts_to_be_applied_node[i][5]
 					# Check if bnd is static. Then no need to update, just add to rule trace, check if graph attribute and add ipl complement to rule trace as well
 					if interpretations_node[comp].world[l].is_static():
 						# Inverse of this is: if not save_graph_attributes_to_rule_trace and graph_attribute
 						if save_graph_attributes_to_rule_trace or not graph_attribute:
-							rule_trace_node.append((numba.types.int8(t), numba.types.int8(fp_cnt), comp, l, bnd))
+							rule_trace_node.append((numba.types.uint16(t), numba.types.uint16(fp_cnt), comp, l, bnd))
 							if atom_trace:
 								_update_rule_trace(rule_trace_node_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), bnd, facts_to_be_applied_node_trace[i])
 							for p1, p2 in ipl:
 								if p1==l:
-									rule_trace_node.append((numba.types.int8(t), numba.types.int8(fp_cnt), comp, p2, interpretations_node[comp].world[p2]))
+									rule_trace_node.append((numba.types.uint16(t), numba.types.uint16(fp_cnt), comp, p2, interpretations_node[comp].world[p2]))
 									if atom_trace:
 										_update_rule_trace(rule_trace_node_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), interpretations_node[comp].world[p2], facts_to_be_applied_node_trace[i])
 								elif p2==l:
-									rule_trace_node.append((numba.types.int8(t), numba.types.int8(fp_cnt), comp, p1, interpretations_node[comp].world[p1]))
+									rule_trace_node.append((numba.types.uint16(t), numba.types.uint16(fp_cnt), comp, p1, interpretations_node[comp].world[p1]))
 									if atom_trace:
 										_update_rule_trace(rule_trace_node_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), interpretations_node[comp].world[p1], facts_to_be_applied_node_trace[i])
 							
 					else:
 						# Check for inconsistencies (multiple facts)
 						if check_consistent_node(interpretations_node, comp, (l, bnd)):
 							mode = 'graph-attribute-fact' if graph_attribute else 'fact'
@@ -255,36 +255,36 @@
 								# Update convergence params
 								if convergence_mode=='delta_bound':
 									bound_delta = max(bound_delta, changes)
 								else:
 									changes_cnt += changes
 
 					if static:
-						facts_to_be_applied_node[i] = (numba.types.int8(facts_to_be_applied_node[i][0]+1), comp, l, bnd, static, graph_attribute)
+						facts_to_be_applied_node[i] = (numba.types.uint16(facts_to_be_applied_node[i][0]+1), comp, l, bnd, static, graph_attribute)
 
 			# Deleting facts that have been applied is very inefficient
 			
 			# Edges
 			for i in range(len(facts_to_be_applied_edge)):
 				if facts_to_be_applied_edge[i][0]==t:
 					comp, l, bnd, static, graph_attribute = facts_to_be_applied_edge[i][1], facts_to_be_applied_edge[i][2], facts_to_be_applied_edge[i][3], facts_to_be_applied_edge[i][4], facts_to_be_applied_edge[i][5]
 					# Check if bnd is static. Then no need to update, just add to rule trace, check if graph attribute, and add ipl complement to rule trace as well
 					if interpretations_edge[comp].world[l].is_static():
 						# Inverse of this is: if not save_graph_attributes_to_rule_trace and graph_attribute
 						if save_graph_attributes_to_rule_trace or not graph_attribute:
-							rule_trace_edge.append((numba.types.int8(t), numba.types.int8(fp_cnt), comp, l, interpretations_edge[comp].world[l]))
+							rule_trace_edge.append((numba.types.uint16(t), numba.types.uint16(fp_cnt), comp, l, interpretations_edge[comp].world[l]))
 							if atom_trace:
 								_update_rule_trace(rule_trace_edge_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), bnd, facts_to_be_applied_edge_trace[i])
 							for p1, p2 in ipl:
 								if p1==l:
-									rule_trace_edge.append((numba.types.int8(t), numba.types.int8(fp_cnt), comp, p2, interpretations_edge[comp].world[p2]))
+									rule_trace_edge.append((numba.types.uint16(t), numba.types.uint16(fp_cnt), comp, p2, interpretations_edge[comp].world[p2]))
 									if atom_trace:
 										_update_rule_trace(rule_trace_edge_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), interpretations_edge[comp].world[p2], facts_to_be_applied_edge_trace[i])
 								elif p2==l:
-									rule_trace_edge.append((numba.types.int8(t), numba.types.int8(fp_cnt), comp, p1, interpretations_edge[comp].world[p1]))
+									rule_trace_edge.append((numba.types.uint16(t), numba.types.uint16(fp_cnt), comp, p1, interpretations_edge[comp].world[p1]))
 									if atom_trace:
 										_update_rule_trace(rule_trace_edge_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), interpretations_edge[comp].world[p1], facts_to_be_applied_edge_trace[i])
 					else:
 						# Check for inconsistencies
 						if check_consistent_edge(interpretations_edge, comp, (l, bnd)):
 							mode = 'graph-attribute-fact' if graph_attribute else 'fact'
 							u, changes = _update_edge(interpretations_edge, comp, (l, bnd), ipl, rule_trace_edge, fp_cnt, t, static, convergence_mode, atom_trace, save_graph_attributes_to_rule_trace, rules_to_be_applied_edge_trace, i, facts_to_be_applied_edge_trace, rule_trace_edge_atoms, mode=mode)
@@ -307,15 +307,15 @@
 								# Update convergence params
 								if convergence_mode=='delta_bound':
 									bound_delta = max(bound_delta, changes)
 								else:
 									changes_cnt += changes
 
 					if static:
-						facts_to_be_applied_edge[i] = (numba.types.int8(facts_to_be_applied_edge[i][0]+1), comp, l, bnd, static, graph_attribute)
+						facts_to_be_applied_edge[i] = (numba.types.uint16(facts_to_be_applied_edge[i][0]+1), comp, l, bnd, static, graph_attribute)
 
 			# Deleting facts that have been applied is very inefficient
 
 			in_loop = True
 			while in_loop:
 				# This will become true only if delta_t = 0 for some rule, otherwise we go to the next timestep
 				in_loop = False
@@ -383,15 +383,15 @@
 									# Update convergence params
 									if convergence_mode=='delta_bound':
 										bound_delta = max(bound_delta, changes)
 									else:
 										changes_cnt += changes
 
 						# Delete rules that have been applied from list by changing t to -1
-						rules_to_be_applied_node[idx] = (numba.types.int8(-1), comp, l, bnd, False)
+						rules_to_be_applied_node[idx] = (numba.types.uint16(-1), comp, l, bnd, False)
 
 						# Break out of the apply rules loop if a rule is immediate. Then we go to the fp operator and check for other applicable rules then come back
 						if immediate:
 							# If delta_t=0 we want to apply one rule and go back to the fp operator
 							# If delta_t>0 we want to come back here and apply the rest of the rules
 							if immediate_edge_rule_fire:
 								break
@@ -465,15 +465,15 @@
 									# Update convergence params
 									if convergence_mode=='delta_bound':
 										bound_delta = max(bound_delta, changes)
 									else:
 										changes_cnt += changes
 
 						# Delete rules that have been applied from list by changing t to -1
-						rules_to_be_applied_edge[idx] = (numba.types.int8(-1), comp, l, bnd, False)
+						rules_to_be_applied_edge[idx] = (numba.types.uint16(-1), comp, l, bnd, False)
 
 						# Break out of the apply rules loop if a rule is immediate. Then we go to the fp operator and check for other applicable rules then come back
 						if immediate:
 							# If t=0 we want to apply one rule and go back to the fp operator
 							# If t>0 we want to come back here and apply the rest of the rules
 							if immediate_edge_rule_fire:
 								break
@@ -505,15 +505,15 @@
 								target_criteria_satisfaction = are_satisfied_node(interpretations_node, n, rule.get_target_criteria())
 								if (target_criteria_satisfaction and is_satisfied_node(interpretations_node, n, (rule.get_target(), interval.closed(0,1)))) or (target_criteria_satisfaction and rule.get_target().value==''):
 									result, annotations, qualified_nodes, qualified_edges, edges_to_add = _is_rule_applicable(interpretations_node, interpretations_edge, neighbors, n, rule.get_neigh_criteria(), rule.get_thresholds(), reverse_graph, rule.get_annotation_function(), rule.get_annotation_label(), rule.get_edges(), atom_trace)
 									if (result and rule.get_target().value=='') or (result and not interpretations_node[n].world[rule.get_target()].is_static()):
 										bnd = influence(rule, annotations, rule.get_weights())
 										max_rules_time = max(max_rules_time, t+delta_t)
 										edges_to_be_added_node_rule.append(edges_to_add)
-										rules_to_be_applied_node.append((numba.types.int8(t+delta_t), n, rule.get_target(), bnd, immediate_rule))
+										rules_to_be_applied_node.append((numba.types.uint16(t+delta_t), n, rule.get_target(), bnd, immediate_rule))
 										if atom_trace:
 											rules_to_be_applied_node_trace.append((qualified_nodes, qualified_edges, rule.get_name()))
 
 										# We apply a rule on a node/edge only once in each timestep to prevent it from being added to the to_be_added list continuously (this will improve performance
 										nodes_to_skip.append((i, j))
 
 										# Handle loop parameters for the next (maybe) fp operation
@@ -543,15 +543,15 @@
 								if (target_criteria_satisfaction and is_satisfied_node(interpretations_edge, e, (rule.get_target(), interval.closed(0,1)))) or (target_criteria_satisfaction and rule.get_target().value==''):
 									# Find out if rule is applicable. returns list of list, of qualified nodes and qualified edges. one for each clause
 									result, annotations, qualified_nodes, qualified_edges, edges_to_add = _is_rule_applicable_edge(interpretations_node, interpretations_edge, neighbors, e, rule.get_neigh_criteria(), rule.get_thresholds(), reverse_graph, rule.get_annotation_function(), rule.get_annotation_label(), rule.get_edges(), atom_trace)
 									if (result and rule.get_target().value=='') or (result and not interpretations_edge[e].world[rule.get_target()].is_static()):
 										bnd = influence(rule, annotations, rule.get_weights())
 										max_rules_time = max(max_rules_time, t+delta_t)
 										edges_to_be_added_edge_rule.append(edges_to_add)
-										rules_to_be_applied_edge.append((numba.types.int8(t+delta_t), e, rule.get_target(), bnd, immediate_rule))
+										rules_to_be_applied_edge.append((numba.types.uint16(t+delta_t), e, rule.get_target(), bnd, immediate_rule))
 										if atom_trace:
 											rules_to_be_applied_edge_trace.append((qualified_nodes, qualified_edges, rule.get_name()))
 
 										# We apply a rule on a node/edge only once in each timestep to prevent it from being added to the to_be_added list continuously (this will improve performance
 										edges_to_skip.append((i, j))
 
 										# Handle loop parameters for the next (maybe) fp operation
@@ -933,15 +933,15 @@
 		world.world[l].set_static(static)
 		if world.world[l]!=prev_bnd:
 			updated = True
 			updated_bnds.append(world.world[l])
 
 			# Add to rule trace if update happened and add to atom trace if necessary
 			if save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact':
-				rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, l, world.world[l].copy()))
+				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, l, world.world[l].copy()))
 				if atom_trace:
 					# Mode can be fact or rule, updation of trace will happen accordingly
 					if mode=='fact' or mode=='graph-attribute-fact':
 						qn = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
 						qe = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
 						name = facts_to_be_applied_trace[idx]
 						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
@@ -958,25 +958,25 @@
 						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p2], f'IPL: {l.get_value()}')
 					lower = max(world.world[p2].lower, 1 - world.world[p1].upper)
 					upper = min(world.world[p2].upper, 1 - world.world[p1].lower)
 					world.world[p2].set_lower_upper(lower, upper)
 					world.world[p2].set_static(static)
 					ip_update_cnt += 1
 					updated_bnds.append(world.world[p2])
-					rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, p2, interval.closed(lower, upper)))
+					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(lower, upper)))
 				if p2==l:
 					if atom_trace:
 						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p1], f'IPL: {l.get_value()}')
 					lower = max(world.world[p1].lower, 1 - world.world[p2].upper)
 					upper = min(world.world[p1].upper, 1 - world.world[p2].lower)
 					world.world[p1].set_lower_upper(lower, upper)
 					world.world[p1].set_static(static)
 					ip_update_cnt += 1
 					updated_bnds.append(world.world[p1])
-					rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, p1, interval.closed(lower, upper)))
+					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(lower, upper)))
 		
 		# Gather convergence data
 		change = 0
 		if updated:
 			# Find out if it has changed from previous interp
 			current_bnd = world.world[l]
 			prev_t_bnd = interval.closed(world.world[l].prev_lower, world.world[l].prev_upper)
@@ -1011,15 +1011,15 @@
 		world.world[l].set_static(static)
 		if world.world[l]!=prev_bnd:
 			updated = True
 			updated_bnds.append(world.world[l])
 
 			# Add to rule trace if update happened and add to atom trace if necessary
 			if save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact':
-				rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, l, world.world[l].copy()))
+				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, l, world.world[l].copy()))
 				if atom_trace:
 					# Mode can be fact or rule, updation of trace will happen accordingly
 					if mode=='fact' or mode=='graph-attribute-fact':
 						qn = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
 						qe = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
 						name = facts_to_be_applied_trace[idx]
 						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
@@ -1037,25 +1037,25 @@
 						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p2], f'IPL: {l.get_value()}')
 					lower = max(world.world[p2].lower, 1 - world.world[p1].upper)
 					upper = min(world.world[p2].upper, 1 - world.world[p1].lower)
 					world.world[p2].set_lower_upper(lower, upper)
 					world.world[p2].set_static(static)
 					ip_update_cnt += 1
 					updated_bnds.append(world.world[p2])
-					rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, p2, interval.closed(lower, upper)))
+					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(lower, upper)))
 				if p2==l:
 					if atom_trace:
 						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p1], f'IPL: {l.get_value()}')
 					lower = max(world.world[p1].lower, 1 - world.world[p2].upper)
 					upper = min(world.world[p1].upper, 1 - world.world[p2].lower)
 					world.world[p1].set_lower_upper(lower, upper)
 					world.world[p1].set_static(static)
 					ip_update_cnt += 1
 					updated_bnds.append(world.world[p1])
-					rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, p1, interval.closed(lower, upper)))
+					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(lower, upper)))
 		
 		# Gather convergence data
 		change = 0
 		if updated:
 			# Find out if it has changed from previous interp
 			current_bnd = world.world[l]
 			prev_t_bnd = interval.closed(world.world[l].prev_lower, world.world[l].prev_upper)
@@ -1090,15 +1090,15 @@
 		world.world[l].set_static(static)
 		if world.world[l]!=prev_bnd:
 			updated = True
 			updated_bnds.append(world.world[l])
 
 			# Add to rule trace if update happened and add to atom trace if necessary
 			if save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact':
-				rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, l, world.world[l].copy()))
+				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, l, world.world[l].copy()))
 				if atom_trace:
 					# Mode can be fact or rule, updation of trace will happen accordingly
 					if mode=='fact' or mode=='graph-attribute-fact':
 						qn = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
 						qe = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
 						name = facts_to_be_applied_trace[idx]
 						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
@@ -1115,25 +1115,25 @@
 						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p2], f'IPL: {l.get_value()}')
 					lower = max(world.world[p2].lower, 1 - world.world[p1].upper)
 					upper = min(world.world[p2].upper, 1 - world.world[p1].lower)
 					world.world[p2].set_lower_upper(lower, upper)
 					world.world[p2].set_static(static)
 					ip_update_cnt += 1
 					updated_bnds.append(world.world[p2])
-					rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, p2, interval.closed(lower, upper)))
+					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(lower, upper)))
 				if p2==l:
 					if atom_trace:
 						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p1], f'IPL: {l.get_value()}')
 					lower = max(world.world[p1].lower, 1 - world.world[p2].upper)
 					upper = min(world.world[p1].upper, 1 - world.world[p2].lower)
 					world.world[p1].set_lower_upper(lower, upper)
 					world.world[p1].set_static(static)
 					ip_update_cnt += 1
 					updated_bnds.append(world.world[p2])
-					rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, p1, interval.closed(lower, upper)))
+					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(lower, upper)))
 	
 		# Gather convergence data
 		change = 0
 		if updated:
 			# Find out if it has changed from previous interp
 			current_bnd = world.world[l]
 			prev_t_bnd = interval.closed(world.world[l].prev_lower, world.world[l].prev_upper)
@@ -1167,15 +1167,15 @@
 		world.world[l].set_static(static)
 		if world.world[l]!=prev_bnd:
 			updated = True
 			updated_bnds.append(world.world[l])
 
 			# Add to rule trace if update happened and add to atom trace if necessary
 			if save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact':
-				rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, l, world.world[l].copy()))
+				rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, l, world.world[l].copy()))
 				if atom_trace:
 					# Mode can be fact or rule, updation of trace will happen accordingly
 					if mode=='fact' or mode=='graph-attribute-fact':
 						qn = numba.typed.List.empty_list(numba.typed.List.empty_list(node_type))
 						qe = numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type))
 						name = facts_to_be_applied_trace[idx]
 						_update_rule_trace(rule_trace_atoms, qn, qe, prev_bnd, name)
@@ -1192,25 +1192,25 @@
 						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p2], f'IPL: {l.get_value()}')
 					lower = max(world.world[p2].lower, 1 - world.world[p1].upper)
 					upper = min(world.world[p2].upper, 1 - world.world[p1].lower)
 					world.world[p2].set_lower_upper(lower, upper)
 					world.world[p2].set_static(static)
 					ip_update_cnt += 1
 					updated_bnds.append(world.world[p2])
-					rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, p2, interval.closed(lower, upper)))
+					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(lower, upper)))
 				if p2==l:
 					if atom_trace:
 						_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p1], f'IPL: {l.get_value()}')
 					lower = max(world.world[p1].lower, 1 - world.world[p2].upper)
 					upper = min(world.world[p1].upper, 1 - world.world[p2].lower)
 					world.world[p1].set_lower_upper(lower, upper)
 					world.world[p1].set_static(static)
 					ip_update_cnt += 1
 					updated_bnds.append(world.world[p2])
-					rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, p1, interval.closed(lower, upper)))
+					rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(lower, upper)))
 	
 		# Gather convergence data
 		change = 0
 		if updated:
 			# Find out if it has changed from previous interp
 			current_bnd = world.world[l]
 			prev_t_bnd = interval.closed(world.world[l].prev_lower, world.world[l].prev_upper)
@@ -1314,60 +1314,60 @@
 	else:
 		return True
 
 
 @numba.njit(cache=True)
 def resolve_inconsistency_node(interpretations, comp, na, ipl, t_cnt, fp_cnt, atom_trace, rule_trace, rule_trace_atoms):
 	world = interpretations[comp]
-	rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, na[0], interval.closed(0,1)))
+	rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, na[0], interval.closed(0,1)))
 	if atom_trace:
 		_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[na[0]], 'Inconsistency')
 	# Resolve inconsistency and set static
 	world.world[na[0]].set_lower_upper(0, 1)
 	world.world[na[0]].set_static(True)
 	for p1, p2 in ipl:
 		if p1==na[0]:
 			if atom_trace:
 				_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p2], 'Inconsistency')
 			world.world[p2].set_lower_upper(0, 1)
 			world.world[p2].set_static(True)
-			rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, p2, interval.closed(0,1)))
+			rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(0,1)))
 
 		if p2==na[0]:
 			if atom_trace:
 				_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p1], 'Inconsistency')
 			world.world[p1].set_lower_upper(0, 1)
 			world.world[p1].set_static(True)
-			rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, p1, interval.closed(0,1)))
+			rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(0,1)))
 	# Add inconsistent predicates to a list 
 
 
 @numba.njit(cache=True)
 def resolve_inconsistency_edge(interpretations, comp, na, ipl, t_cnt, fp_cnt, atom_trace, rule_trace, rule_trace_atoms):
 	world = interpretations[comp]
-	rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, na[0], interval.closed(0,1)))
+	rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, na[0], interval.closed(0,1)))
 	if atom_trace:
 		_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[na[0]], 'Inconsistency')
 	# Resolve inconsistency and set static
 	world.world[na[0]].set_lower_upper(0, 1)
 	world.world[na[0]].set_static(True)
 	for p1, p2 in ipl:
 		if p1==na[0]:
 			if atom_trace:
 				_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p2], 'Inconsistency')
 			world.world[p2].set_lower_upper(0, 1)
 			world.world[p2].set_static(True)
-			rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, p2, interval.closed(0,1)))
+			rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p2, interval.closed(0,1)))
 
 		if p2==na[0]:
 			if atom_trace:
 				_update_rule_trace(rule_trace_atoms, numba.typed.List.empty_list(numba.typed.List.empty_list(node_type)), numba.typed.List.empty_list(numba.typed.List.empty_list(edge_type)), world.world[p1], 'Inconsistency')
 			world.world[p1].set_lower_upper(0, 1)
 			world.world[p1].set_static(True)
-			rule_trace.append((numba.types.int8(t_cnt), numba.types.int8(fp_cnt), comp, p1, interval.closed(0,1)))
+			rule_trace.append((numba.types.uint16(t_cnt), numba.types.uint16(fp_cnt), comp, p1, interval.closed(0,1)))
 
 
 @numba.njit(cache=True)
 def _add_node(node, neighbors, nodes, interpretations_node):
 	nodes.append(node)
 	neighbors[node] = numba.typed.List.empty_list(node_type)
 	interpretations_node[node] = world.World(numba.typed.List.empty_list(label.label_type))
```

### Comparing `pyreason-1.5.2/pyreason/scripts/interval/interval.py` & `pyreason-1.5.3/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 class FactModel(models.StructModel):
     def __init__(self, dmm, fe_type):
         members = [
             ('name', numba.types.string),
             ('component', numba.types.Tuple((numba.types.string, numba.types.string))),
             ('l', label.label_type),
             ('bnd', interval.interval_type),
-            ('t_lower', numba.types.int8),
-            ('t_upper', numba.types.int8),
+            ('t_lower', numba.types.uint16),
+            ('t_upper', numba.types.uint16),
             ('static', numba.types.boolean)
             ]
         models.StructModel.__init__(self, dmm, fe_type, members)
 
 
 # Expose datamodel attributes
 make_attribute_wrapper(FactType, 'name', 'name')
@@ -61,59 +61,65 @@
 make_attribute_wrapper(FactType, 'bnd', 'bnd')
 make_attribute_wrapper(FactType, 't_lower', 't_lower')
 make_attribute_wrapper(FactType, 't_upper', 't_upper')
 make_attribute_wrapper(FactType, 'static', 'static')
 
 
 # Implement constructor
-@lower_builtin(Fact, numba.types.string, numba.types.Tuple((numba.types.string, numba.types.string)), label.label_type, interval.interval_type, numba.types.int8, numba.types.int8, numba.types.boolean)
+@lower_builtin(Fact, numba.types.string, numba.types.Tuple((numba.types.string, numba.types.string)), label.label_type, interval.interval_type, numba.types.uint16, numba.types.uint16, numba.types.boolean)
 def impl_fact(context, builder, sig, args):
     typ = sig.return_type
     name, component, l, bnd, t_lower, t_upper, static = args
     fact = cgutils.create_struct_proxy(typ)(context, builder)
     fact.name = name
     fact.component = component
     fact.l = l
     fact.bnd = bnd
     fact.t_lower = t_lower
     fact.t_upper = t_upper
     fact.static = static
     return fact._getvalue()
 
+
 # Expose properties
 @overload_method(FactType, "get_name")
 def get_name(fact):
     def getter(fact):
         return fact.name
     return getter
 
+
 @overload_method(FactType, "get_component")
 def get_component(fact):
     def getter(fact):
         return fact.component
     return getter
 
+
 @overload_method(FactType, "get_label")
 def get_label(fact):
     def getter(fact):
         return fact.l
     return getter
 
+
 @overload_method(FactType, "get_bound")
 def get_bound(fact):
     def getter(fact):
         return fact.bnd
     return getter
 
+
 @overload_method(FactType, "get_time_lower")
 def get_time_lower(fact):
     def getter(fact):
         return fact.t_lower
     return getter
 
+
 @overload_method(FactType, "get_time_upper")
 def get_time_lower(fact):
     def getter(fact):
         return fact.t_upper
     return getter
 
 
@@ -128,39 +134,38 @@
     t_upper_obj = c.pyapi.object_getattr_string(obj, "_t_upper")
     static_obj = c.pyapi.object_getattr_string(obj, "_static")
     fact = cgutils.create_struct_proxy(typ)(c.context, c.builder)
     fact.name = c.unbox(numba.types.string, name_obj).value
     fact.component = c.unbox(numba.types.Tuple((numba.types.string, numba.types.string)), component_obj).value
     fact.l = c.unbox(label.label_type, l_obj).value
     fact.bnd = c.unbox(interval.interval_type, bnd_obj).value
-    fact.t_lower = c.unbox(numba.types.int8, t_lower_obj).value
-    fact.t_upper = c.unbox(numba.types.int8, t_upper_obj).value
+    fact.t_lower = c.unbox(numba.types.uint16, t_lower_obj).value
+    fact.t_upper = c.unbox(numba.types.uint16, t_upper_obj).value
     fact.static = c.unbox(numba.types.boolean, static_obj).value
     c.pyapi.decref(name_obj)
     c.pyapi.decref(component_obj)
     c.pyapi.decref(l_obj)
     c.pyapi.decref(bnd_obj)
     c.pyapi.decref(t_lower_obj)
     c.pyapi.decref(t_upper_obj)
     c.pyapi.decref(static_obj)
     is_error = cgutils.is_not_null(c.builder, c.pyapi.err_occurred())
     return NativeValue(fact._getvalue(), is_error=is_error)
 
 
-
 @box(FactType)
 def box_fact(typ, val, c):
     fact = cgutils.create_struct_proxy(typ)(c.context, c.builder, value=val)
     class_obj = c.pyapi.unserialize(c.pyapi.serialize_object(Fact))
     name_obj = c.box(numba.types.string, fact.name)
     component_obj = c.box(numba.types.Tuple((numba.types.string, numba.types.string)), fact.component)
     l_obj = c.box(label.label_type, fact.l)
     bnd_obj = c.box(interval.interval_type, fact.bnd)
-    t_lower_obj = c.box(numba.types.int8, fact.t_lower)
-    t_upper_obj = c.box(numba.types.int8, fact.t_upper)
+    t_lower_obj = c.box(numba.types.uint16, fact.t_lower)
+    t_upper_obj = c.box(numba.types.uint16, fact.t_upper)
     static_obj = c.box(numba.types.boolean, fact.static)
     res = c.pyapi.call_function_objargs(class_obj, (name_obj, component_obj, l_obj, bnd_obj, t_lower_obj, t_upper_obj, static_obj))
     c.pyapi.decref(name_obj)
     c.pyapi.decref(component_obj)
     c.pyapi.decref(l_obj)
     c.pyapi.decref(bnd_obj)
     c.pyapi.decref(t_lower_obj)
```

### Comparing `pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 
 # Create new numba type
 class FactType(types.Type):
     def __init__(self):
         super(FactType, self).__init__(name='FactNode')
 
+
 fact_type = FactType()
 
 
 # Type inference
 @typeof_impl.register(Fact)
 def typeof_fact(val, c):
     return fact_type
@@ -42,16 +43,16 @@
 class FactModel(models.StructModel):
     def __init__(self, dmm, fe_type):
         members = [
             ('name', numba.types.string),
             ('component', numba.types.string),
             ('l', label.label_type),
             ('bnd', interval.interval_type),
-            ('t_lower', numba.types.int8),
-            ('t_upper', numba.types.int8),
+            ('t_lower', numba.types.uint16),
+            ('t_upper', numba.types.uint16),
             ('static', numba.types.boolean)
             ]
         models.StructModel.__init__(self, dmm, fe_type, members)
 
 
 # Expose datamodel attributes
 make_attribute_wrapper(FactType, 'name', 'name')
@@ -60,59 +61,65 @@
 make_attribute_wrapper(FactType, 'bnd', 'bnd')
 make_attribute_wrapper(FactType, 't_lower', 't_lower')
 make_attribute_wrapper(FactType, 't_upper', 't_upper')
 make_attribute_wrapper(FactType, 'static', 'static')
 
 
 # Implement constructor
-@lower_builtin(Fact, numba.types.string, numba.types.string, label.label_type, interval.interval_type, numba.types.int8, numba.types.int8, numba.types.boolean)
+@lower_builtin(Fact, numba.types.string, numba.types.string, label.label_type, interval.interval_type, numba.types.uint16, numba.types.uint16, numba.types.boolean)
 def impl_fact(context, builder, sig, args):
     typ = sig.return_type
     name, component, l, bnd, t_lower, t_upper, static = args
     fact = cgutils.create_struct_proxy(typ)(context, builder)
     fact.name = name
     fact.component = component
     fact.l = l
     fact.bnd = bnd
     fact.t_lower = t_lower
     fact.t_upper = t_upper
     fact.static = static
     return fact._getvalue()
 
+
 # Expose properties
 @overload_method(FactType, "get_name")
 def get_name(fact):
     def getter(fact):
         return fact.name
     return getter
 
+
 @overload_method(FactType, "get_component")
 def get_component(fact):
     def getter(fact):
         return fact.component
     return getter
 
+
 @overload_method(FactType, "get_label")
 def get_label(fact):
     def getter(fact):
         return fact.l
     return getter
 
+
 @overload_method(FactType, "get_bound")
 def get_bound(fact):
     def getter(fact):
         return fact.bnd
     return getter
 
+
 @overload_method(FactType, "get_time_lower")
 def get_time_lower(fact):
     def getter(fact):
         return fact.t_lower
     return getter
 
+
 @overload_method(FactType, "get_time_upper")
 def get_time_lower(fact):
     def getter(fact):
         return fact.t_upper
     return getter
 
 
@@ -127,16 +134,16 @@
     t_upper_obj = c.pyapi.object_getattr_string(obj, "_t_upper")
     static_obj = c.pyapi.object_getattr_string(obj, "_static")
     fact = cgutils.create_struct_proxy(typ)(c.context, c.builder)
     fact.name = c.unbox(numba.types.string, name_obj).value
     fact.component = c.unbox(numba.types.string, component_obj).value
     fact.l = c.unbox(label.label_type, l_obj).value
     fact.bnd = c.unbox(interval.interval_type, bnd_obj).value
-    fact.t_lower = c.unbox(numba.types.int8, t_lower_obj).value
-    fact.t_upper = c.unbox(numba.types.int8, t_upper_obj).value
+    fact.t_lower = c.unbox(numba.types.uint16, t_lower_obj).value
+    fact.t_upper = c.unbox(numba.types.uint16, t_upper_obj).value
     fact.static = c.unbox(numba.types.boolean, static_obj).value
     c.pyapi.decref(name_obj)
     c.pyapi.decref(component_obj)
     c.pyapi.decref(l_obj)
     c.pyapi.decref(bnd_obj)
     c.pyapi.decref(t_lower_obj)
     c.pyapi.decref(t_upper_obj)
@@ -150,16 +157,16 @@
 def box_fact(typ, val, c):
     fact = cgutils.create_struct_proxy(typ)(c.context, c.builder, value=val)
     class_obj = c.pyapi.unserialize(c.pyapi.serialize_object(Fact))
     name_obj = c.box(numba.types.string, fact.name)
     component_obj = c.box(numba.types.string, fact.component)
     l_obj = c.box(label.label_type, fact.l)
     bnd_obj = c.box(interval.interval_type, fact.bnd)
-    t_lower_obj = c.box(numba.types.int8, fact.t_lower)
-    t_upper_obj = c.box(numba.types.int8, fact.t_upper)
+    t_lower_obj = c.box(numba.types.uint16, fact.t_lower)
+    t_upper_obj = c.box(numba.types.uint16, fact.t_upper)
     static_obj = c.box(numba.types.boolean, fact.static)
     res = c.pyapi.call_function_objargs(class_obj, (name_obj, component_obj, l_obj, bnd_obj, t_lower_obj, t_upper_obj, static_obj))
     c.pyapi.decref(name_obj)
     c.pyapi.decref(component_obj)
     c.pyapi.decref(l_obj)
     c.pyapi.decref(bnd_obj)
     c.pyapi.decref(t_lower_obj)
```

### Comparing `pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 @register_model(RuleType)
 class RuleModel(models.StructModel):
     def __init__(self, dmm, fe_type):
         members = [
             ('name', types.string),
             ('target', label.label_type),
             ('target_criteria', types.ListType(types.Tuple((label.label_type, interval.interval_type)))),
-            ('delta', types.int8),
+            ('delta', types.uint16),
             ('neigh_criteria', types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), label.label_type, interval.interval_type)))),
             ('bnd', interval.interval_type),
             ('thresholds', types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64)))),
             ('ann_fn', types.string),
             ('ann_label', label.label_type),
             ('weights', types.float64[::1]),
             ('edges', types.Tuple((types.string, types.string, label.label_type))),
@@ -71,15 +71,15 @@
 make_attribute_wrapper(RuleType, 'ann_label', 'ann_label')
 make_attribute_wrapper(RuleType, 'weights', 'weights')
 make_attribute_wrapper(RuleType, 'edges', 'edges')
 make_attribute_wrapper(RuleType, 'immediate_rule', 'immediate_rule')
 
 
 # Implement constructor
-@lower_builtin(Rule, types.string, label.label_type, types.ListType(types.Tuple((label.label_type, interval.interval_type))), types.int8, types.ListType(types.Tuple((types.string, label.label_type, interval.interval_type))), interval.interval_type, types.ListType(types.ListType(types.Tuple((types.string, types.string, types.float64)))), types.string, label.label_type, types.float64[::1], types.Tuple((types.string, types.string, label.label_type)), types.boolean)
+@lower_builtin(Rule, types.string, label.label_type, types.ListType(types.Tuple((label.label_type, interval.interval_type))), types.uint16, types.ListType(types.Tuple((types.string, label.label_type, interval.interval_type))), interval.interval_type, types.ListType(types.ListType(types.Tuple((types.string, types.string, types.float64)))), types.string, label.label_type, types.float64[::1], types.Tuple((types.string, types.string, label.label_type)), types.boolean)
 def impl_rule(context, builder, sig, args):
     typ = sig.return_type
     name, target, target_criteria, delta, neigh_criteria, bnd, thresholds, ann_fn, ann_label, weights, edges, immediate_rule = args
     context.nrt.incref(builder, types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), label.label_type, interval.interval_type))), neigh_criteria)
     context.nrt.incref(builder, types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64))), thresholds)
     rule = cgutils.create_struct_proxy(typ)(context, builder)
     rule.name = name
@@ -197,15 +197,15 @@
     weights_obj = c.pyapi.object_getattr_string(obj, "_weights")
     edges_obj = c.pyapi.object_getattr_string(obj, "_edges")
     immediate_rule_obj = c.pyapi.object_getattr_string(obj, "_immediate_rule")
     rule = cgutils.create_struct_proxy(typ)(c.context, c.builder)
     rule.name = c.unbox(types.string, name_obj).value
     rule.target = c.unbox(label.label_type, target_obj).value
     rule.target_criteria = c.unbox(types.ListType(types.Tuple((label.label_type, interval.interval_type))), tc_obj).value
-    rule.delta = c.unbox(types.int8, delta_obj).value
+    rule.delta = c.unbox(types.uint16, delta_obj).value
     rule.neigh_criteria = c.unbox(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), label.label_type, interval.interval_type))), neigh_criteria_obj).value
     rule.bnd = c.unbox(interval.interval_type, bnd_obj).value
     rule.thresholds = c.unbox(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64))), thresholds_obj).value
     rule.ann_fn = c.unbox(types.string, ann_fn_obj).value
     rule.ann_label = c.unbox(label.label_type, ann_label_obj).value
     rule.weights = c.unbox(types.float64[::1], weights_obj).value
     rule.edges = c.unbox(types.Tuple((types.string, types.string, label.label_type)), edges_obj).value
@@ -229,15 +229,15 @@
 @box(RuleType)
 def box_rule(typ, val, c):
     rule = cgutils.create_struct_proxy(typ)(c.context, c.builder, value=val)
     class_obj = c.pyapi.unserialize(c.pyapi.serialize_object(Rule))
     name_obj = c.box(types.string, rule.name)
     target_obj = c.box(label.label_type, rule.target)
     tc_obj = c.box(types.ListType(types.Tuple((label.label_type, interval.interval_type))), rule.target_criteria)
-    delta_obj = c.box(types.int8, rule.delta)
+    delta_obj = c.box(types.uint16, rule.delta)
     neigh_criteria_obj = c.box(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), label.label_type, interval.interval_type))), rule.neigh_criteria)
     bnd_obj = c.box(interval.interval_type, rule.bnd)
     thresholds_obj = c.box(types.ListType(types.Tuple((types.string, types.UniTuple(types.string, 2), types.float64))), rule.thresholds)
     ann_fn_obj = c.box(types.string, rule.ann_fn)
     ann_label_obj = c.box(label.label_type, rule.ann_label)
     weights_obj = c.box(types.float64[::1], rule.weights)
     edges_obj = c.box(types.Tuple((types.string, types.string, label.label_type)), rule.edges)
```

### Comparing `pyreason-1.5.2/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.5.3/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/program/program.py` & `pyreason-1.5.3/pyreason/scripts/program/program.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/rules/rule.py` & `pyreason-1.5.3/pyreason/scripts/rules/rule.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/utils/filter.py` & `pyreason-1.5.3/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.5.3/pyreason/scripts/utils/graphml_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,27 +28,27 @@
             for key, value in self.graph.nodes[n].items():
                 # IF attribute is a float or int and it is less than 1, then make it a bound, else make it a label
                 if isinstance(value, (float, int)) and value<=1 and value>=0:
                     l = str(key)
                     l_bnd = float(value)
                     u_bnd = 1
                 else:
-                    l = l = f'{key}-{value}'
+                    l = f'{key}-{value}'
                     l_bnd = 1
                     u_bnd = 1
                 if isinstance(value, str):
-                    l = str(key)
                     bnd_str = value.split(',')
                     if len(bnd_str)==2:
                         try:
                             low = int(bnd_str[0])
                             up = int(bnd_str[1])
                             if low<=1 and low>=0 and up<=1 and up>=0:
                                 l_bnd = low
                                 u_bnd = up
+                                l = str(key)
                         except:
                             pass
                 
                 if label.Label(l) not in specific_node_labels.keys():
                     specific_node_labels[label.Label(l)] = numba.typed.List.empty_list(numba.types.string)
                 specific_node_labels[label.Label(l)].append(n)
                 f = fact_node.Fact('graph-attribute-fact', n, label.Label(l), interval.closed(l_bnd, u_bnd), 0, 0, static=static_facts)
@@ -57,27 +57,27 @@
             for key, value in self.graph.edges[e].items():
                 # IF attribute is a float or int and it is less than 1, then make it a bound, else make it a label
                 if isinstance(value, (float, int)) and value<=1 and value>=0:
                     l = str(key)
                     l_bnd = float(value)
                     u_bnd = 1
                 else:
-                    l = l = f'{key}-{value}'
+                    l = f'{key}-{value}'
                     l_bnd = 1
                     u_bnd = 1
                 if isinstance(value, str):
-                    l = str(key)
                     bnd_str = value.split(',')
                     if len(bnd_str)==2:
                         try:
                             low = int(bnd_str[0])
                             up = int(bnd_str[1])
                             if low<=1 and low>=0 and up<=1 and up>=0:
                                 l_bnd = low
                                 u_bnd = up
+                                l = str(key)
                         except:
                             pass
 
                 if label.Label(l) not in specific_edge_labels.keys():
                     specific_edge_labels[label.Label(l)] = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.string)))
                 specific_edge_labels[label.Label(l)].append((e[0], e[1]))
                 f = fact_edge.Fact('graph-attribute-fact', (e[0], e[1]), label.Label(l), interval.closed(l_bnd, u_bnd), 0, 0, static=static_facts)
```

### Comparing `pyreason-1.5.2/pyreason/scripts/utils/output.py` & `pyreason-1.5.3/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/utils/plotter.py` & `pyreason-1.5.3/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/utils/visuals.py` & `pyreason-1.5.3/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.5.3/pyreason/scripts/utils/yaml_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         # Set rule target criteria
         target_criteria = numba.typed.List.empty_list(numba.types.Tuple((label.label_type, interval.interval_type)))
         if values['target_criteria'] is not None:
             for tc in values['target_criteria']:
                 target_criteria.append((label.Label(tc[0]), interval.closed(tc[1], tc[2])))
 
         # Set delta t
-        delta_t = numba.types.int8(values['delta_t'])
+        delta_t = numba.types.uint16(values['delta_t'])
 
         # neigh_criteria = [c1, c2, c3, c4]
         # thresholds = [t1, t2, t3, t4]
 
         # Array of thresholds to keep track of for each neighbor criterion. Form [(comparison, (number/percent, total/available), thresh)]
         thresholds = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.UniTuple(numba.types.string, 2), numba.types.float64)))
```

### Comparing `pyreason-1.5.2/pyreason.egg-info/PKG-INFO` & `pyreason-1.5.3/pyreason.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.5.2
+Version: 1.5.3
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.5.2/pyreason.egg-info/SOURCES.txt` & `pyreason-1.5.3/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.5.2/setup.py` & `pyreason-1.5.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name = 'pyreason',
-    version = '1.5.2',
+    version = '1.5.3',
     author = 'Dyuman Aditya',
     author_email = 'dyuman.aditya@gmail.com',
     description = 'An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/lab-v2/pyreason',
     license = 'BSD 3-clause',
```

