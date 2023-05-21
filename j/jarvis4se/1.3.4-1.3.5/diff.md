# Comparing `tmp/jarvis4se-1.3.4.tar.gz` & `tmp/jarvis4se-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarvis4se-1.3.4.tar", last modified: Mon Mar  6 16:10:53 2023, max compression
+gzip compressed data, was "jarvis4se-1.3.5.tar", last modified: Sun May 21 16:51:56 2023, max compression
```

## Comparing `jarvis4se-1.3.4.tar` & `jarvis4se-1.3.5.tar`

### file list

```diff
@@ -1,54 +1,60 @@
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-03-06 16:10:53.932497 jarvis4se-1.3.4/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1105 2022-11-01 17:13:00.000000 jarvis4se-1.3.4/LICENSE
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2497 2023-03-06 16:10:53.932497 jarvis4se-1.3.4/PKG-INFO
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1783 2022-11-01 17:13:00.000000 jarvis4se-1.3.4/README.md
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      188 2022-11-01 17:13:00.000000 jarvis4se-1.3.4/pyproject.toml
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      793 2023-03-06 16:10:53.932497 jarvis4se-1.3.4/setup.cfg
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1100 2023-03-06 16:06:20.000000 jarvis4se-1.3.4/setup.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-03-06 16:10:53.919165 jarvis4se-1.3.4/src/
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-03-06 16:10:53.922498 jarvis4se-1.3.4/src/datamodel/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      900 2023-02-21 11:54:41.000000 jarvis4se-1.3.4/src/datamodel/__init__.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    30237 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/datamodel/datamodel.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      235 2023-02-21 11:54:41.000000 jarvis4se-1.3.4/src/datamodel/setup.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1441 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/datamodel/util.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-03-06 16:10:53.922498 jarvis4se-1.3.4/src/jarvis/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      598 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/jarvis/__init__.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    12721 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/jarvis/command_parser.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    64973 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/jarvis/diagram_generator.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    31221 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/jarvis/functional_orchestrator.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     4701 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/jarvis/jarvis.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    34208 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/jarvis/question_answer.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    60199 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/jarvis/shared_orchestrator.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    12157 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/jarvis/viewpoint_orchestrator.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-03-06 16:10:53.925831 jarvis4se-1.3.4/src/jarvis4se.egg-info/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2497 2023-03-06 16:10:53.000000 jarvis4se-1.3.4/src/jarvis4se.egg-info/PKG-INFO
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1177 2023-03-06 16:10:53.000000 jarvis4se-1.3.4/src/jarvis4se.egg-info/SOURCES.txt
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)        1 2023-03-06 16:10:53.000000 jarvis4se-1.3.4/src/jarvis4se.egg-info/dependency_links.txt
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)       74 2023-03-06 16:10:53.000000 jarvis4se-1.3.4/src/jarvis4se.egg-info/requires.txt
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)       52 2023-03-06 16:10:53.000000 jarvis4se-1.3.4/src/jarvis4se.egg-info/top_level.txt
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-03-06 16:10:53.925831 jarvis4se-1.3.4/src/plantuml_adapter/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1433 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/plantuml_adapter/__init__.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    41341 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/plantuml_adapter/plantuml_adapter.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      206 2022-11-01 17:13:00.000000 jarvis4se-1.3.4/src/plantuml_adapter/setup.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    19978 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/plantuml_adapter/util.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-03-06 16:10:53.925831 jarvis4se-1.3.4/src/tools/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      551 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/tools/__init__.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2158 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/tools/config.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2825 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/tools/console.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2558 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/tools/logger.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1536 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/tools/magic_tools.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      304 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/src/tools/util.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-03-06 16:10:53.929164 jarvis4se-1.3.4/src/xml_adapter/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      165 2022-11-01 17:13:00.000000 jarvis4se-1.3.4/src/xml_adapter/__init__.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)      191 2022-11-01 17:13:00.000000 jarvis4se-1.3.4/src/xml_adapter/setup.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    19903 2023-03-06 15:44:42.000000 jarvis4se-1.3.4/src/xml_adapter/xml_parser.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    30093 2023-02-21 11:54:41.000000 jarvis4se-1.3.4/src/xml_adapter/xml_writer.py
-drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-03-06 16:10:53.932497 jarvis4se-1.3.4/tests/
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    16095 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/tests/test_context_diagrams.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    12226 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/tests/test_decomposition_diagrams.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    11251 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/tests/test_input_cell.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2785 2022-11-08 19:33:28.000000 jarvis4se-1.3.4/tests/test_magic_tools.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2318 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/tests/test_question_answer.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2935 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/tests/test_sequence_diagrams.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1158 2023-03-06 15:44:42.000000 jarvis4se-1.3.4/tests/test_state_obj.py
--rw-r--r--   0 not2behere  (1000) not2behere  (1000)    18507 2023-03-06 15:56:04.000000 jarvis4se-1.3.4/tests/test_xml_file.py
+drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.875665 jarvis4se-1.3.5/
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1105 2022-11-01 17:13:00.000000 jarvis4se-1.3.5/LICENSE
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2497 2023-05-21 16:51:56.875665 jarvis4se-1.3.5/PKG-INFO
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1783 2022-11-01 17:13:00.000000 jarvis4se-1.3.5/README.md
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      188 2022-11-01 17:13:00.000000 jarvis4se-1.3.5/pyproject.toml
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      793 2023-05-21 16:51:56.878998 jarvis4se-1.3.5/setup.cfg
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1100 2023-05-21 16:49:17.000000 jarvis4se-1.3.5/setup.py
+drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.865665 jarvis4se-1.3.5/src/
+drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.868998 jarvis4se-1.3.5/src/datamodel/
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      900 2023-02-21 11:54:41.000000 jarvis4se-1.3.5/src/datamodel/__init__.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    30237 2023-03-06 15:56:04.000000 jarvis4se-1.3.5/src/datamodel/datamodel.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      235 2023-02-21 11:54:41.000000 jarvis4se-1.3.5/src/datamodel/setup.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1494 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/datamodel/util.py
+drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.868998 jarvis4se-1.3.5/src/jarvis/
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      684 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/__init__.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    12938 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/command_parser.py
+drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.868998 jarvis4se-1.3.5/src/jarvis/diagram/
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      229 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/diagram/__init__.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    38387 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/diagram/diagram_generator.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     4862 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/diagram/diagram_generator_chain.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     5869 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/diagram/diagram_generator_fana.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    10784 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/diagram/diagram_generator_farch.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    19998 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/diagram/util.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     4433 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/jarvis.py
+drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.872332 jarvis4se-1.3.5/src/jarvis/orchestrator/
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      109 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/orchestrator/__init__.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    33057 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/orchestrator/functional_orchestrator.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    60025 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/orchestrator/shared_orchestrator.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    12291 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/orchestrator/viewpoint_orchestrator.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    34208 2023-03-06 15:56:04.000000 jarvis4se-1.3.5/src/jarvis/question_answer.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1721 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/jarvis/util.py
+drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.872332 jarvis4se-1.3.5/src/jarvis4se.egg-info/
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2497 2023-05-21 16:51:56.000000 jarvis4se-1.3.5/src/jarvis4se.egg-info/PKG-INFO
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1368 2023-05-21 16:51:56.000000 jarvis4se-1.3.5/src/jarvis4se.egg-info/SOURCES.txt
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)        1 2023-05-21 16:51:56.000000 jarvis4se-1.3.5/src/jarvis4se.egg-info/dependency_links.txt
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)       74 2023-05-21 16:51:56.000000 jarvis4se-1.3.5/src/jarvis4se.egg-info/requires.txt
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)       52 2023-05-21 16:51:56.000000 jarvis4se-1.3.5/src/jarvis4se.egg-info/top_level.txt
+drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.872332 jarvis4se-1.3.5/src/plantuml_adapter/
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1433 2023-03-06 15:56:04.000000 jarvis4se-1.3.5/src/plantuml_adapter/__init__.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    47455 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/plantuml_adapter/plantuml_adapter.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      206 2022-11-01 17:13:00.000000 jarvis4se-1.3.5/src/plantuml_adapter/setup.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    20036 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/plantuml_adapter/util.py
+drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.875665 jarvis4se-1.3.5/src/tools/
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      551 2023-03-06 15:56:04.000000 jarvis4se-1.3.5/src/tools/__init__.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     3071 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/tools/config.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2708 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/tools/console.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     3014 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/tools/logger.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     1575 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/tools/magic_tools.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      362 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/tools/util.py
+drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.875665 jarvis4se-1.3.5/src/xml_adapter/
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      142 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/xml_adapter/__init__.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      191 2022-11-01 17:13:00.000000 jarvis4se-1.3.5/src/xml_adapter/setup.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    25934 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/xml_adapter/xml_parser.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    32240 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/src/xml_adapter/xml_writer.py
+drwxr-xr-x   0 not2behere  (1000) not2behere  (1000)        0 2023-05-21 16:51:56.875665 jarvis4se-1.3.5/tests/
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     9338 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/tests/test_input_cell.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      911 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/tests/test_lib.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)     2669 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/tests/test_magic_tools.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)      227 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/tests/test_question_answer.py
+-rw-r--r--   0 not2behere  (1000) not2behere  (1000)    12564 2023-05-21 16:45:17.000000 jarvis4se-1.3.5/tests/test_xml_file.py
```

### Comparing `jarvis4se-1.3.4/LICENSE` & `jarvis4se-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jarvis4se-1.3.4/PKG-INFO` & `jarvis4se-1.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis4se
-Version: 1.3.4
+Version: 1.3.5
 Summary: Jarvis 4 Systems Engineers
 Home-page: https://github.com/rcasteran/jarvis4se
 Author: Justin ANCELOT
 Author-email: not2behere@gmx.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rcasteran/jarvis4se/issues
 Project-URL: Gitbook, https://regis-casteran.gitbook.io/jarvis4se/
```

### Comparing `jarvis4se-1.3.4/README.md` & `jarvis4se-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `jarvis4se-1.3.4/setup.cfg` & `jarvis4se-1.3.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jarvis4se
-version = 1.3.4
+version = 1.3.5
 author = Justin ANCELOT
 author_email = not2behere@gmx.fr
 description = Jarvis 4 Systems Engineers
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rcasteran/jarvis4se
 project_urls =
```

### Comparing `jarvis4se-1.3.4/setup.py` & `jarvis4se-1.3.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 # jarvis4se version
-VERSION = "1.3.4"
+VERSION = "1.3.5"
 
 
 def readme():
     """print long description"""
     with open('README.md', "r", encoding="utf-8") as f:
         return f.read()
```

### Comparing `jarvis4se-1.3.4/src/datamodel/__init__.py` & `jarvis4se-1.3.5/src/datamodel/__init__.py`

 * *Files identical despite different names*

### Comparing `jarvis4se-1.3.4/src/datamodel/datamodel.py` & `jarvis4se-1.3.5/src/datamodel/datamodel.py`

 * *Files identical despite different names*

### Comparing `jarvis4se-1.3.4/src/datamodel/util.py` & `jarvis4se-1.3.5/src/datamodel/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""@defgroup datamodel
+Module for 3SE datamodel
+"""
+
 class Point:
     """@ingroup datamodel
     @anchor Point
     Basic type for diagram coordinates
     """
     def __init__(self, p_x='', p_y=''):
         """
```

### Comparing `jarvis4se-1.3.4/src/jarvis/__init__.py` & `jarvis4se-1.3.5/src/jarvis/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-"""An example magic"""
+""" @package jarvis
+Jarvis module
+
+Contains IPython Magic Class with magic cell as entry point of Jarvis
+"""
 __version__ = '0.0.1'
 from . import command_parser
 from .jarvis import MagicJarvis, greet_user, clean_folders
 from tools import MagicTools, Config
 from plantuml_adapter import PlantUmlGen
```

### Comparing `jarvis4se-1.3.4/src/jarvis/command_parser.py` & `jarvis4se-1.3.5/src/jarvis/command_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # Libraries
 import re
 import uuid
-import pathlib
 import os
 import requests
 from IPython.display import display, HTML, Markdown
 
 
 # Modules
-from . import viewpoint_orchestrator
-from . import functional_orchestrator
-from . import shared_orchestrator
+from jarvis.orchestrator import functional_orchestrator, shared_orchestrator, viewpoint_orchestrator
 from .question_answer import get_object_list, get_pandas_table, find_question
-from .diagram_generator import filter_show_command
+from jarvis.diagram import diagram_generator
 from tools import get_hyperlink
 from tools import Config
 from tools import Logger
 
 
 class CmdParser:
     def __init__(self, generator):
@@ -36,49 +33,57 @@
 
             (r"consider ([^.|\n]*)", matched_consider),
 
             (r"([^. |\n][^.|\n]*) is composed of ([^.|\n]*)", matched_composition),
 
             (r"([^. |\n][^.|\n]*) composes ([^.|\n]*)", matched_composition),
 
+            (r"([^. |\n][^.|\n]*) compose ([^.|\n]*)", matched_composition),
+
             (r"([^. |\n][^.|\n]*) consumes ([^.|\n]*)", matched_consumer),
 
             (r"([^. |\n][^.|\n]*) is an input of ([^.|\n]*)", matched_consumer),
 
             (r"([^. |\n][^.|\n]*) produces ([^.|\n]*)", matched_producer),
 
             (r"([^. |\n][^.|\n]*) is an output of ([^.|\n]*)", matched_producer),
 
             (r"([^. |\n][^.|\n]*) exposes ([^.|\n]*)", matched_exposes),
 
+            (r"([^. |\n][^.|\n]*) expose ([^.|\n]*)", matched_exposes),
+
             (r"([^. |\n][^.|\n]*) is allocated to ([^.|\n]*)", matched_allocation),
 
             (r"([^. |\n][^.|\n]*) allocates ([^.|\n]*)", matched_allocation),
 
             (r"delete ([^.|\n]*)", matched_delete),
 
             (r"The type of (.*?) is ([^.|\n]*)", matched_type),
 
             (r"([^. |\n][^.|\n]*) implies ([^.|\n]*)", matched_implies),
 
+            (r"([^. |\n][^.|\n]*) imply ([^.|\n]*)", matched_implies),
+
             (r"Condition for (.*?) is:([^.|\n]*)", matched_condition),
 
             (r"The (source|destination) of (.*?) is ([^.|\n]*)", matched_src_dest),
 
             (r"show ([^.|\n]*)", self.matched_show),
 
             (r"(.*?)\?", matched_question_mark),
 
             (r"list (input|output|child|data|function|transition|interface) ([^.|\n]*)",
              matched_list),
 
             (r"The ((?!type|alias|source|destination).*) of (.*?) is ([^.|\n]*)",
              matched_described_attribute),
         ]
+
         self.reverse = (r"([^. |\n][^.|\n]*) composes ([^.|\n]*)",
+                        r"([^. |\n][^.|\n]*) compose ([^.|\n]*)",
                         r"([^. |\n][^.|\n]*) consumes ([^.|\n]*)",
                         r"([^. |\n][^.|\n]*) produces ([^.|\n]*)",
                         r"([^. |\n][^.|\n]*) is allocated to ([^.|\n]*)")
 
         self.generator = generator
 
     def lookup_table(self, string, **kwargs):
@@ -96,15 +101,15 @@
                 result = re.search(regex, string, re.MULTILINE)
             else:
                 # Transform to avoid duplicated function's declaration within cells input
                 result = []
                 [result.append(x) for x in re.findall(regex, string, re.MULTILINE) if x not in result]
 
             if result and not result_chain:
-                # self.reverse : ("composes", "consumes", "produces", "is allocated to")
+                # self.reverse
                 if regex in self.reverse:
                     result = reverse(result)
                 update = method(result, **kwargs)
 
             elif result_chain:
                 string = ''
                 update = self.matched_under(result_chain, **kwargs)
@@ -127,27 +132,27 @@
         if 1 in out:
             return 1
 
         return 0
 
     def matched_show(self, diagram_name_str, **kwargs):
         """Get "show" declaration"""
-        out = filter_show_command(diagram_name_str, **kwargs)
+        out = diagram_generator.filter_show_command(diagram_name_str, **kwargs)
         if out:
             if Config.is_diagram_file:
                 url = self.generator.get_diagram_url(out)
                 # Generate and set unique identifier of length 10 integers
                 identi = uuid.uuid4()
                 identi = str(identi.int)[:10]
 
                 if not os.path.isdir("diagrams"):
                     os.makedirs("diagrams")
 
+                current_file_path = str('./diagrams/Diagram' + identi + '.svg')
                 try:
-                    current_file_path = str('./diagrams/Diagram' + identi + '.svg')
                     response = requests.get(url)
                     with open(current_file_path, "wb") as file_writer:
                         file_writer.write(response.content)
                     url = current_file_path
                 except EnvironmentError as ex:
                     Logger.set_error(__name__,
                                      f"Unable to write the diagram {current_file_path}: {str(ex)}")
```

### Comparing `jarvis4se-1.3.4/src/jarvis/diagram_generator.py` & `jarvis4se-1.3.5/src/plantuml_adapter/plantuml_adapter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,1386 +1,1142 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""Module with methods relative to Diagram generation for filtering objects before passing
-them to plantuml_adapter.py"""
-# Libraries
-import re
+"""@defgroup plantuml_adapter
+Plantuml adapter module
+"""
 
 # Modules
-import plantuml_adapter
-from datamodel import FunctionalElement
-from .question_answer import check_parentality, get_objects_names, check_get_object, switch_data, \
-    get_children, check_not_family, switch_fun_elem_interface, get_allocation_object
-from .shared_orchestrator import childs_inheritance, reset_childs_inheritance, \
-    attribute_inheritance, reset_attribute_inheritance, view_inheritance, reset_view_inheritance, \
-    allocation_inheritance, reset_alloc_inheritance
+import datamodel
+from .util import ObjDiagram, StateDiagram, SequenceDiagram
 from tools import Logger
 
 
-def filter_show_command(diagram_name_str, **kwargs):
-    """Entry point for all diagrams (i.e. 'show' command) from command_parser.py"""
-    plantuml_string = None
-    wanted_diagram_str = diagram_name_str[0].strip()
-    regex = r"(decomposition|context|chain|sequence|state|function|state sequence)\s(.*)"
-    specific_diagram_str = re.search(regex, wanted_diagram_str, re.MULTILINE)
-    if specific_diagram_str:
-        if 'sequence' not in specific_diagram_str.group(2):
-            diagram_type_str = specific_diagram_str.group(1)
-            diagram_object_str = specific_diagram_str.group(2)
+def write_function_child(string_obj, function, input_flow_list, output_flow_list,
+                         xml_attribute_list):
+    """@ingroup plantuml_adapter
+    Construct PlantUml text recursively
+    @param[in,out] string_obj current PlantUml text
+    @param[in] function
+    @param[in] input_flow_list
+    @param[in] output_flow_list
+    @param[in] xml_attribute_list
+    @return None
+    """
+
+    function_input_port = []
+    function_output_port = []
+    external_input_port = []
+    external_output_port = []
+    parent_function_port = []
+    count = 1
+    nb_component = count_composed_component(function, count)
+
+    # TODO: Create get_port_lists() and optimize
+    for p in input_flow_list:
+        if p[0][0] == function.name.lower():
+            function_input_port.append(p)
+        if p[0][0] is None and function.parent is None:
+            external_input_port.append(p)
+            if p[0][1] == function.name.lower():
+                parent_function_port.append(p)
+
+    for q in output_flow_list:
+        if q[0][0] == function.name.lower():
+            function_output_port.append(q)
+        if q[0][0] is None and function.parent is None:
+            external_output_port.append(q)
+            if q[0][1] == function.name.lower():
+                parent_function_port.append(q)
+
+    Logger.set_debug(__name__, f"Function name: {function.name}")
+    Logger.set_debug(__name__, f"Input port list: {function_input_port}")
+    Logger.set_debug(__name__, f"Output port list: {function_input_port}")
+    Logger.set_debug(__name__, f"Parent function port list: {parent_function_port}")
+    Logger.set_debug(__name__, f"External input port list: {external_input_port}")
+    Logger.set_debug(__name__, f"External output port list: {external_output_port}")
+
+    string_obj.create_port(function_input_port, "in")
+    string_obj.create_port(function_output_port, "out")
+    string_obj.create_port(parent_function_port, 'None')
+
+    child_with_no_child_list = []
+    child_with_child_list = []
+    # Create a child list for each parent function
+    for child_function in function.child_list:
+        Logger.set_debug(__name__, f"{child_function.name} check as child of {function.name}")
+        if child_function.child_list:
+            child_with_child_list.append(child_function)
         else:
-            diagram_type_str = specific_diagram_str.group(1) + ' sequence'
-            diagram_object_str = specific_diagram_str.group(2).replace("sequence ", "")
+            child_with_no_child_list.append(child_function)
 
-        plantuml_string = switch_show_filter(diagram_type_str=diagram_type_str,
-                                             diagram_object_str=diagram_object_str,
-                                             **kwargs)
-    else:
-        Logger.set_warning(__name__,
-                          f"Jarvis does not understand the command {wanted_diagram_str}")
+    # For child that has no child: create object
+    for fun in child_with_no_child_list:
+        string_obj.create_object(fun, xml_attribute_list)
+
+    for child in child_with_child_list:
+        string_obj.create_component(child)
+        write_function_child(string_obj, child, input_flow_list, output_flow_list,
+                             xml_attribute_list)
+        nb_component -= 1
+
+    # Close all the brackets depending on the number of component within highest parent
+    for i in range(nb_component):
+        string_obj.append_string('}\n')
+
+    for component in child_with_child_list:
+        string_obj.create_component_attribute(component, xml_attribute_list)
+
+    whole_child_list = child_with_child_list + child_with_no_child_list
+    for fun in whole_child_list:
+        for i in input_flow_list:
+            if i[0][0] == fun.name.lower():
+                string_obj.create_port(input_flow_list, "in")
+        for j in output_flow_list:
+            if j[0][0] == fun.name.lower():
+                string_obj.create_port(output_flow_list, "out")
+
+    string_obj.create_port(external_input_port, "in")
+    string_obj.create_port(external_output_port, "out")
+
+
+def count_composed_component(function, count):
+    """@ingroup plantuml_adapter
+    Count the number of composed function within the higher function
+    @param[in] function function to check
+    @param[in] count number of component
+    @return number of component
+    """
+
+    for elem in function.child_list:
+        if elem.child_list:
+            count += 1
+            count_composed_component(elem, count)
+            continue
+    return count
 
-    return plantuml_string
 
+def write_function_object(string_obj, function, input_flow_list, output_flow_list, check,
+                          xml_attribute_list, component_obj=None, compo_diagram=False):
+    """@ingroup plantuml_adapter
+    Construct the PlantUml text for a function object with associated ports for flow lists.
+    @param[in,out] string_obj current PlantUml text
+    @param[in] function
+    @param[in] input_flow_list
+    @param[in] output_flow_list
+    @param[in] check
+    @param[in] xml_attribute_list
+    @param[in] component_obj
+    @param[in] compo_diagram
+    @return PlantUml text for the function object
+    """
 
-def switch_show_filter(**kwargs):
-    """Switch case between diagram types"""
-    switch = {
-        "function": case_function_diagram,
-        "context": case_context_diagram,
-        "decomposition": case_decomposition_diagram,
-        "chain": case_chain_diagram,
-        "sequence": case_sequence_diagram,
-        "state": case_state_diagram,
-        "state sequence": case_state_sequence_diagram
-    }
-    get_diagram = switch.get(kwargs['diagram_type_str'], case_no_diagram)
-    return get_diagram(**kwargs)
-
-
-def case_function_diagram(**kwargs):
-    """Case for 'show function <functional_element>'"""
-    plantuml_string = None
-    xml_fun_elem_name_list = get_objects_names(kwargs['xml_fun_elem_list'])
-    if kwargs['diagram_object_str'] in xml_fun_elem_name_list:
-        plantuml_string = show_fun_elem_function(kwargs['diagram_object_str'],
-                                                 kwargs['xml_fun_elem_list'],
-                                                 kwargs['xml_function_list'],
-                                                 kwargs['xml_consumer_function_list'],
-                                                 kwargs['xml_producer_function_list'],
-                                                 kwargs['xml_type_list'])
+    string_obj.create_object(function, xml_attribute_list)
 
-    else:
-        Logger.set_warning(__name__,
-                          f"Jarvis does not know the functional Element {kwargs['diagram_object_str']}")
+    if check:
+        string_obj.append_string('}\n')
+        if component_obj:
+            string_obj.create_component_attribute(component_obj, xml_attribute_list)
+
+    for p in input_flow_list:
+        if compo_diagram:
+            if p[0][0] == function.name.lower():
+                string_obj.create_port(input_flow_list, "in")
+        else:
+            if p[0][0] == function.name.lower() or p[0][1] == function.name.lower():
+                string_obj.create_port(input_flow_list, "in")
+    for q in output_flow_list:
+        if compo_diagram:
+            if q[0][0] == function.name.lower():
+                string_obj.create_port(output_flow_list, "out")
+        else:
+            if q[0][0] == function.name.lower() or q[0][1] == function.name.lower():
+                string_obj.create_port(output_flow_list, "out")
 
-    return plantuml_string
 
+def get_function_diagrams(function_list, fun_elem_list, consumer_function_list, producer_function_list,
+                          parent_child_dict, data_list, xml_type_list, xml_attribute_list):
+    """@ingroup plantuml_adapter
+    @anchor get_function_diagrams
+    Construct the PlantUml text and url for the requested diagram between one of the following:
+    - context of function
+    - decomposition of function
+    - chain of function
+    @param[in] function_list
+    @param[in] consumer_function_list
+    @param[in] producer_function_list
+    @param[in] parent_child_dict
+    @param[in] data_list
+    @param[in] xml_type_list
+    @param[in] xml_attribute_list
+    @return PlantUml text and url of the diagram
+    """
 
-def case_context_diagram(**kwargs):
-    """Case for 'show context <functional_element>/<function>'"""
-    plantuml_string = None
-    xml_function_name_list = get_objects_names(kwargs['xml_function_list'])
-    xml_state_name_list = get_objects_names(kwargs['xml_state_list'])
-    xml_fun_elem_name_list = get_objects_names(kwargs['xml_fun_elem_list'])
-
-    if kwargs['diagram_object_str'] in xml_function_name_list:
-        plantuml_string = show_function_context(kwargs['diagram_object_str'],
-                                                kwargs['xml_function_list'],
-                                                kwargs['xml_consumer_function_list'],
-                                                kwargs['xml_producer_function_list'],
-                                                kwargs['xml_data_list'],
-                                                kwargs['xml_attribute_list'],
-                                                kwargs['xml_type_list'])
-
-    elif kwargs['diagram_object_str'] in xml_state_name_list:
-        plantuml_string = show_states_chain([kwargs['diagram_object_str']],
-                                            kwargs['xml_state_list'],
-                                            kwargs['xml_transition_list'])
-
-    elif kwargs['diagram_object_str'] in xml_fun_elem_name_list:
-        plantuml_string = show_fun_elem_context(kwargs['diagram_object_str'],
-                                                kwargs['xml_fun_elem_list'],
-                                                kwargs['xml_function_list'],
-                                                kwargs['xml_consumer_function_list'],
-                                                kwargs['xml_producer_function_list'],
-                                                kwargs['xml_attribute_list'],
-                                                kwargs['xml_fun_inter_list'],
-                                                kwargs['xml_data_list'])
-    else:
-        Logger.set_warning(__name__,
-                          f"Jarvis does not know the function {kwargs['diagram_object_str']} or "
-                          f"{kwargs['diagram_object_str']} is not a valid "
-                          f"Function/State/Functional Element name/alias")
-
-    return plantuml_string
-
-
-def case_decomposition_diagram(**kwargs):
-    """Case for 'show decomposition <functional_element>/<function>'"""
-    plantuml_string = None
-
-    if ' at level ' in kwargs['diagram_object_str']:
-        splitted_str = re.split(" at level ", kwargs['diagram_object_str'])
-        diagram_object_str = splitted_str[0]
-        try:
-            diagram_level = int(splitted_str[1])
-            if diagram_level == 0:
-                Logger.set_error(__name__,
-                                "Invalid level, please choose a valid level >= 1")
-                return plantuml_string
-        except ValueError:
-            Logger.set_error(__name__,
-                            "Invalid level, please choose a valid level >= 1")
-            return plantuml_string
+    string_obj = ObjDiagram()
+    # Filter output flows
+    output_flow_list = get_output_flows(consumer_function_list, producer_function_list,
+                                        concatenate=True)
+    # Filter input flows
+    input_flow_list = get_input_flows(consumer_function_list, producer_function_list,
+                                      concatenate=True)
+
+    # Filter consumers and producers list in order to create data flow
+    data_flow_list = get_exchanged_flows(consumer_function_list, producer_function_list,
+                                         parent_child_dict, concatenate=True)
+
+    Logger.set_debug(__name__, f"Output flows list: {output_flow_list}")
+    Logger.set_debug(__name__, f"Input flows list: {input_flow_list}")
+    Logger.set_debug(__name__, f'Exchanged flows list: {data_flow_list}')
+
+    if data_list:
+        per_message_data_flow_list = get_exchanged_flows(consumer_function_list,
+                                                         producer_function_list,
+                                                         parent_child_dict)
+        if len(data_list) == len(per_message_data_flow_list):
+            ordered_function_list, ordered_message_list = order_list(per_message_data_flow_list,
+                                                                     data_list)
+            if per_message_data_flow_list != ordered_message_list:
+                for idx, i in enumerate(ordered_message_list):
+                    for j in data_flow_list:
+                        for k in j[1]:
+                            if i[2] == k and i[3]:
+                                new = str(idx + 1) + ":" + k
+                                j[1].remove(k)
+                                j[1].append(new)
+
+    # Loop in order to filter functions and write in output's file, see write_function_child()
+    if parent_child_dict:
+        if fun_elem_list:
+            for fun_elem in fun_elem_list:
+                string_obj.create_component(fun_elem)
+                check_function = False
+                for f in function_list:
+                    if any(a == f.id for a in fun_elem.allocated_function_list):
+                        if len(fun_elem.allocated_function_list) > 1:
+                            check_function = False
+                        else:
+                            check_function = True
+                        write_function_object(string_obj, f, input_flow_list, output_flow_list,
+                                              check_function, xml_attribute_list, component_obj=fun_elem)
+                if not check_function:
+                    string_obj.append_string('}\n')
+                    string_obj.create_component_attribute(fun_elem, xml_attribute_list)
+        else:
+            for function in function_list:
+                if function.id not in parent_child_dict.keys():
+                    if function.id in parent_child_dict.values():
+                        # Function is a parent
+                        string_obj.create_component(function)
+                        write_function_child(string_obj, function, input_flow_list, output_flow_list,
+                                             xml_attribute_list)
+                    else:
+                        # Function is not a parent:
+                        write_function_object(string_obj, function, input_flow_list, output_flow_list,
+                                              False, xml_attribute_list, compo_diagram=True)
+                # Else do nothing : done as children of function parent
     else:
-        diagram_object_str = kwargs['diagram_object_str']
-        diagram_level = None
+        for function in function_list:
+            write_function_object(string_obj, function, input_flow_list, output_flow_list, False,
+                                  xml_attribute_list)
 
-    v_inheritance = view_inheritance(kwargs['xml_view_list'],
-                                     kwargs['xml_function_list'],
-                                     kwargs['xml_fun_elem_list'])
-
-    # Check view if activated and filter allocated item,
-    # if not activated then no item filtered
-    # if not any item under view return string for user's message
-    function_list = get_object_list_from_view(diagram_object_str,
-                                              kwargs['xml_function_list'],
-                                              kwargs['xml_view_list'])
-
-    # TODO : why this print ?
-    if isinstance(function_list, str):
-        print(function_list)
-        return None
-
-    if diagram_object_str in get_objects_names(kwargs['xml_function_list']):
-        consumer_list, producer_list = get_cons_prod_from_view_allocated_data(
-            kwargs['xml_data_list'],
-            kwargs['xml_view_list'],
-            kwargs['xml_consumer_function_list'],
-            kwargs['xml_producer_function_list'],
-            function_list)
-
-        plantuml_string = show_function_decomposition(diagram_object_str,
-                                                      function_list,
-                                                      consumer_list,
-                                                      producer_list,
-                                                      kwargs['xml_attribute_list'],
-                                                      kwargs['xml_type_list'],
-                                                      diagram_level=diagram_level)
-
-    elif diagram_object_str in get_objects_names(kwargs['xml_fun_elem_list']):
-        fun_elem_list = get_object_list_from_view(diagram_object_str,
-                                                  kwargs['xml_fun_elem_list'],
-                                                  kwargs['xml_view_list'])
-        consumer_list, producer_list = get_cons_prod_from_view_allocated_data(
-            kwargs['xml_data_list'],
-            kwargs['xml_view_list'],
-            kwargs['xml_consumer_function_list'],
-            kwargs['xml_producer_function_list'],
-            function_list)
-
-        plantuml_string = show_fun_elem_decomposition(diagram_object_str,
-                                                      function_list,
-                                                      consumer_list,
-                                                      producer_list,
-                                                      fun_elem_list,
-                                                      kwargs['xml_attribute_list'],
-                                                      kwargs['xml_data_list'],
-                                                      kwargs['xml_fun_inter_list'],
-                                                      diagram_level)
+    string_obj.create_input_flow(input_flow_list)
+    string_obj.create_output_flow(output_flow_list)
+    string_obj.create_data_flow(data_flow_list)
+
+    return string_obj.string
+
+
+def get_fun_elem_context_diagram(function_list, consumer_function_list, producer_function_list,
+                                 data_list, xml_attribute_list, fun_elem_list, fun_inter_list):
+    """@ingroup plantuml_adapter
+    @anchor get_fun_elem_context_diagram
+    Construct the PlantUml text and url for the context diagram for functional elements
+    @param[in] function_list TBD
+    @param[in] consumer_function_list TBD
+    @param[in] producer_function_list TBD
+    @param[in] data_list TBD
+    @param[in] xml_attribute_list TBD
+    @param[in] fun_elem_list TBD
+    @param[in] fun_inter_list TBD
+    @return PlantUml text and url of the diagram
+    """
 
-    else:
-        Logger.set_warning(__name__,
-                          f"Jarvis does not know the object {diagram_object_str}"
-                          f"(i.e. it is not a function, nor a functional element)")
-
-    reset_view_inheritance(kwargs['xml_view_list'], v_inheritance)
-
-    return plantuml_string
-
-
-def get_cons_prod_from_view_allocated_data(xml_data_list, xml_view_list, xml_consumer_function_list,
-                                           xml_producer_function_list, function_list):
-    """If a view is activated, returns filtered consumer/producer lists"""
-    new_consumer_list = []
-    new_producer_list = []
-    new_data_list = filter_allocated_item_from_view(xml_data_list, xml_view_list)
-
-    if len(new_data_list) == len(xml_data_list):
-        for prod in xml_producer_function_list:
-            if any(item == prod[1] for item in function_list):
-                new_producer_list.append(prod)
-
-        for cons in xml_consumer_function_list:
-            if any(item == cons[1] for item in function_list):
-                new_consumer_list.append(cons)
+    string_obj = ObjDiagram()
+    interface_list = None
 
-    else:
-        for cons in xml_consumer_function_list:
-            if any(item.name == cons[0] for item in new_data_list) and \
-                    any(item == cons[1] for item in function_list):
-                new_consumer_list.append(cons)
-
-        for prod in xml_producer_function_list:
-            if any(item.name == prod[0] for item in new_data_list) and \
-                    any(item == prod[1] for item in function_list):
-                new_producer_list.append(prod)
-
-    return new_consumer_list, new_producer_list
-
-
-def get_object_list_from_view(obj_str, xml_obj_list, xml_view_list):
-    """Returns current object's list by checking view"""
-    output_list = filter_allocated_item_from_view(xml_obj_list, xml_view_list)
-    if isinstance(output_list, str):
-        return output_list
-
-    if len(xml_obj_list) == len(output_list):
-        return xml_obj_list
-
-    if isinstance(obj_str, str):
-        for obj in xml_obj_list:
-            if obj_str in (obj.name, obj.alias) and not any(item == obj for item in output_list):
-                output_list.append(obj)
-    elif isinstance(obj_str, list):
-        for object_name in obj_str:
-            for obj in xml_obj_list:
-                if object_name in (obj.name, obj.alias) and \
-                        not any(item == obj for item in output_list):
-                    output_list.append(obj)
-
-    for new_obj in output_list:
-        child_list = set()
-        for child in new_obj.child_list:
-            if child in output_list:
-                child_list.add(child)
-        new_obj.child_list.clear()
-        new_obj.child_list = child_list
+    if fun_inter_list:
 
-    return output_list
+        unmerged_data_list = get_exchanged_flows(consumer_function_list, producer_function_list, {})
+        interface_list, data_flow_list = get_interface_list(fun_inter_list,
+                                                            data_list,
+                                                            unmerged_data_list,
+                                                            function_list,
+                                                            fun_elem_list,
+                                                            is_decomposition=False)
 
+        data_flow_list = concatenate_flows(data_flow_list)
 
-def case_chain_diagram(**kwargs):
-    """Case for 'show chain <states>/<functions>'"""
-    plantuml_string = None
-    xml_function_name_list = get_objects_names(kwargs['xml_function_list'])
-    xml_state_name_list = get_objects_names(kwargs['xml_state_list'])
-    object_list_str = re.split(r',(?![^[]*\])', kwargs['diagram_object_str'].replace(" ", ""))
-    if len(object_list_str) > 0:
-        result_function = all(t in xml_function_name_list for t in object_list_str)
-        result_state = all(t in xml_state_name_list for t in object_list_str)
-        if not result_function and not result_state:
-            for i in object_list_str:
-                if len(i) > 0:
-                    if not any(i in s for s in [*xml_function_name_list,
-                                                *xml_state_name_list]):
-                        Logger.set_error(__name__,
-                                        f"The object {i} does not exist, "
-                                        f"not a function/state's name nor an alias")
+    else:
+
+        # Filter consumers and producers list in order to create data flow
+        data_flow_list = get_exchanged_flows(consumer_function_list, producer_function_list,
+                                             {}, concatenate=True)
+
+    # Filter output flows
+    output_flow_list = get_output_flows(consumer_function_list, producer_function_list,
+                                        concatenate=True)
+    # Filter input flows
+    input_flow_list = get_input_flows(consumer_function_list, producer_function_list,
+                                      concatenate=True)
+
+    # Write external functions
+    external_function_list = []
+    for function in function_list:
+        is_external = True
+        for fun_elem in fun_elem_list:
+            if any(a == function.id for a in fun_elem.allocated_function_list):
+                is_external = False
+
+        if is_external:
+            external_function_list.append(function)
+
+    for function in external_function_list:
+        string_obj.create_object(function, xml_attribute_list)
+
+    for fun_elem in fun_elem_list:
+        string_obj.create_component(fun_elem)
+        check_function = False
+        for f in function_list:
+            if any(a == f.id for a in fun_elem.allocated_function_list):
+                if len(fun_elem.allocated_function_list) > 1:
+                    check_function = False
                 else:
-                    Logger.set_error(__name__,
-                                    f"{kwargs['diagram_object_str']} is not a valid chain")
+                    check_function = True
+                write_function_object(string_obj, f, input_flow_list, output_flow_list,
+                                      check_function, xml_attribute_list, component_obj=fun_elem)
+        if not check_function:
+            string_obj.append_string('}\n')
+            string_obj.create_component_attribute(fun_elem, xml_attribute_list)
+
+    string_obj.create_input_flow(input_flow_list)
+    string_obj.create_output_flow(output_flow_list)
+    string_obj.create_data_flow(data_flow_list)
+
+    if interface_list:
+        string_obj.create_interface(interface_list)
+
+    return string_obj.string
+
+
+def get_interface_list(fun_inter_list, data_list, data_flow_list, function_list, fun_elem_list,
+                       is_decomposition=True):
+    """@ingroup plantuml_adapter
+    Get list of functional interfaces with the functional elements exposing them.
+    Functional interface is returned only when specifed data is allocated to it
+    @param[in] fun_inter_list TBD
+    @param[in] data_list TBD
+    @param[in] data_flow_list TBD
+    @param[in] function_list TBD
+    @param[in] fun_elem_list TBD
+    @param[in] is_decomposition indicates if decomposition is required (True) or not (False)
+    @return functional interfaces list
+    """
 
-        elif result_function or result_state:
-            if result_function:
-                # Check view if activated and filter allocated item,
-                # if not activated then no item filtered
-                # if not any item under view return string
-                function_list = get_object_list_from_view(object_list_str,
-                                                          kwargs['xml_function_list'],
-                                                          kwargs['xml_view_list'])
-
-                # TODO : why this print ?
-                if isinstance(function_list, str):
-                    print(function_list)
-                    return None
-
-                consumer_list, producer_list = get_cons_prod_from_view_allocated_data(
-                    kwargs['xml_data_list'],
-                    kwargs['xml_view_list'],
-                    kwargs['xml_consumer_function_list'],
-                    kwargs['xml_producer_function_list'],
-                    function_list)
-                plantuml_string = show_functions_chain(object_list_str,
-                                                       function_list,
-                                                       consumer_list,
-                                                       producer_list,
-                                                       kwargs['xml_type_list'])
-            elif result_state:
-                # See above after "if result_function"
-                state_list = get_object_list_from_view(object_list_str,
-                                                       kwargs['xml_state_list'],
-                                                       kwargs['xml_view_list'])
-
-                #TODO : why this print ?
-                if isinstance(state_list, str):
-                    print(state_list)
-                    return None
-
-                transition_list = filter_allocated_item_from_view(kwargs['xml_transition_list'],
-                                                                  kwargs['xml_view_list'])
-                plantuml_string = show_states_chain(object_list_str, state_list, transition_list)
+    interface_list = []
+    removed_data_flow_list = []
+    initial_data = list(data_flow_list)
+    idx = 0
+    # Get all fun_inter with allocated data within data_flow_list and create interface list
+    # [[producer, consumer, fun_inter]...]
+    for fun_inter in fun_inter_list:
+        Logger.set_debug(__name__, f"Interface {fun_inter.name}, allocated data {fun_inter.allocated_data_list}")
+        if fun_inter.allocated_data_list:
+            for data_id in fun_inter.allocated_data_list:
+                for data in data_list:
+                    if data_id == data.id:
+                        for data_flow in data_flow_list.copy():
+                            if data.name == data_flow[2]:
+                                first_fun = None
+                                second_fun = None
+                                for fun in function_list:
+                                    if data_flow[0] == fun.name.lower():
+                                        first_fun = fun
+                                    if data_flow[1] == fun.name.lower():
+                                        second_fun = fun
+
+                                if first_fun or second_fun:
+                                    # Need to check consistency between [elem1, elem2, fun_inter] and [fun1, fun2, data]
+                                    # before adding to the list
+                                    is_first_fun_elem = False
+                                    is_second_fun_elem = False
+                                    for fun_elem in fun_elem_list:
+                                        if any(exposed_fun_inter_id == fun_inter.id for exposed_fun_inter_id in
+                                               fun_elem.exposed_interface_list):
+                                            if first_fun and not is_first_fun_elem:
+                                                is_first_fun_elem = any(allocated_fun_id ==
+                                                                        first_fun.id for allocated_fun_id
+                                                                        in fun_elem.allocated_function_list)
+                                            if second_fun and not is_second_fun_elem:
+                                                is_second_fun_elem = any(allocated_fun_id ==
+                                                                         second_fun.id for allocated_fun_id
+                                                                         in fun_elem.allocated_function_list)
+
+                                    if (first_fun and is_first_fun_elem and not second_fun) or \
+                                            (second_fun and is_second_fun_elem and not first_fun) or \
+                                            (first_fun and is_first_fun_elem and second_fun and is_second_fun_elem):
+                                        Logger.set_debug(__name__, f"[{first_fun}, {second_fun}, {fun_inter}] added")
+                                        interface_list.insert(idx, [first_fun, second_fun, fun_inter])
+                                        removed_data_flow_list.insert(idx, data_flow)
+                                        data_flow_list.remove(data_flow)
+                                        idx += 1
+                                        break
         else:
-            Logger.set_error(__name__,
-                            f"{kwargs['diagram_object_str']} is not a valid chain")
+            Logger.set_info(__name__, f"{fun_inter.name} does not have any allocated data (no display)")
 
-    return plantuml_string
+    output_list, interface_list = get_fun_elem_from_fun_inter(interface_list, fun_elem_list, is_decomposition)
 
+    if not output_list:
+        return None, initial_data
 
-def case_sequence_diagram(**kwargs):
-    """Case for 'show sequence <functional_elements>/<functions>/<functional_interface>'"""
-    plantuml_string = None
-    object_list_str = re.split(r',(?![^[]*\])', kwargs['diagram_object_str'].replace(", ", ","))
-    object_list_str = [s.rstrip() for s in object_list_str]
-    if object_list_str:
-        if len(object_list_str) == 1 and \
-                any(s == object_list_str[0] for s in get_objects_names(kwargs['xml_fun_inter_list'])):
-            plantuml_string = get_fun_inter_sequence_diagram(object_list_str.pop(), **kwargs)
-        elif len(object_list_str) >= 1:
-            # Check view if activated and filter allocated item,
-            # if not activated then no item filtered
-            # if not any item under view return string
-            xml_data_list = filter_allocated_item_from_view(kwargs['xml_data_list'],
-                                                            kwargs['xml_view_list'])
-
-            #TODO : why this print ?
-            if isinstance(xml_data_list, str):
-                print(xml_data_list)
-                return None
-
-            if all(i in get_objects_names(kwargs['xml_function_list']) for i in object_list_str):
-
-                if len(xml_data_list) != len(kwargs['xml_data_list']):
-                    xml_cons = [i for i in kwargs['xml_consumer_function_list']
-                                if any(a == i[0] for a in [d.name for d in xml_data_list])]
-                    xml_prod = [i for i in kwargs['xml_producer_function_list']
-                                if any(a == i[0] for a in [d.name for d in xml_data_list])]
+    # (re)Add [producer, consumer, data_name] to data_flow_list if no interface exposed
+    if any(isinstance(s, list) for s in interface_list):
+        for idx, rest_inter in enumerate(interface_list):
+            if isinstance(rest_inter, list):
+                data_flow_list.append(removed_data_flow_list[idx])
+
+    return output_list, data_flow_list
+
+
+def get_fun_elem_from_fun_inter(interface_list, fun_elem_list, is_decomposition=True):
+    """@ingroup plantuml_adapter
+    Get list of functional interfaces with the functional elements exposing them from interface_list =
+    [[producer, consumer, fun_inter]...] and put value to False if (first, second, interface)
+    have been added to output_list (i.e. fun_elem_1/fun_elem_2 have been found for a fun_inter)
+    @param[in] interface_list TBD
+    @param[in] fun_elem_list TBD
+    @param[in] is_decomposition indicates if decomposition is required (True) or not (False)
+    @return functional interfaces list
+    """
+
+    output_list = []
+    for ix, (first, second, interface) in enumerate(interface_list):
+        fun_elem_1 = None
+        fun_elem_2 = None
+        if first:
+            for elem_1 in fun_elem_list:
+                if any(s == interface.id for s in elem_1.exposed_interface_list):
+                    if is_decomposition:
+                        if not elem_1.child_list:
+                            fun_elem_1 = elem_1
+                        else:
+                            check = True
+                            for child in elem_1.child_list:
+                                if any(s == interface.id for s in child.exposed_interface_list):
+                                    check = False
+                            if check:
+                                fun_elem_1 = elem_1
+                    else:
+                        fun_elem_1 = elem_1
+
+        if second:
+            for elem_2 in fun_elem_list:
+                if not first:
+                    if is_decomposition:
+                        if any(s == interface.id for s in elem_2.exposed_interface_list):
+                            if not elem_2.child_list:
+                                fun_elem_2 = elem_2
+                            else:
+                                check = True
+                                for child in elem_2.child_list:
+                                    if any(s == interface.id for s in child.exposed_interface_list):
+                                        check = False
+                                if check:
+                                    fun_elem_2 = elem_2
+                    else:
+                        fun_elem_2 = elem_2
                 else:
-                    xml_cons = kwargs['xml_consumer_function_list']
-                    xml_prod = kwargs['xml_producer_function_list']
-                plantuml_string = show_functions_sequence(object_list_str,
-                                                          kwargs['xml_function_list'],
-                                                          xml_cons,
-                                                          xml_prod,
-                                                          xml_data_list)
-
-            elif all(i in get_objects_names(kwargs['xml_fun_elem_list']) for i in object_list_str):
-                if len(xml_data_list) != len(kwargs['xml_data_list']):
-                    kwargs['xml_consumer_function_list'] = \
-                        [i for i in kwargs['xml_consumer_function_list']
-                         if any(a == i[0] for a in [d.name for d in xml_data_list])]
-                    kwargs['xml_producer_function_list'] = \
-                        [i for i in kwargs['xml_producer_function_list']
-                         if any(a == i[0] for a in [d.name for d in xml_data_list])]
-                kwargs['xml_data_list'] = xml_data_list
-                plantuml_string = get_fun_elem_sequence_diagram(object_list_str, **kwargs)
-
-            else:
-                Logger.set_error(__name__,
-                                f"{kwargs['diagram_object_str']} is not a valid sequence, available sequences "
-                                f"are:\n"
-                                f"- show sequence Function_A, Function_B, ...\n"
-                                f"- show sequence Functional_element_A, Functional_element_B, ...\n"
-                                f"- show sequence Functional_interface\n")
-    return plantuml_string
-
-
-def case_state_diagram(**kwargs):
-    """Case for 'show state <functional_element>'"""
-    plantuml_string = None
-    xml_fun_elem_name_list = get_objects_names(kwargs['xml_fun_elem_list'])
-    if kwargs['diagram_object_str'] in xml_fun_elem_name_list:
-        plantuml_string = show_fun_elem_state_machine(kwargs['diagram_object_str'],
-                                                      kwargs['xml_state_list'],
-                                                      kwargs['xml_transition_list'],
-                                                      kwargs['xml_fun_elem_list'])
+                    if any(s == interface.id for s in elem_2.exposed_interface_list) and \
+                            elem_2 != fun_elem_1:
+                        if is_decomposition:
+                            if not elem_2.child_list:
+                                fun_elem_2 = elem_2
+                            else:
+                                check = True
+                                for child in elem_2.child_list:
+                                    if any(s == interface.id for s in child.exposed_interface_list):
+                                        check = False
+
+                                if check:
+                                    fun_elem_2 = elem_2
+                        else:
+                            fun_elem_2 = elem_2
+
+        if not (not fun_elem_1 and not fun_elem_2):
+            if [fun_elem_1, fun_elem_2, interface] not in output_list:
+                output_list.append([fun_elem_1, fun_elem_2, interface])
+            interface_list[ix] = False
+
+    return output_list, interface_list
+
+
+def check_child_allocation(string_obj, fun_elem, function_list, xml_attribute_list):
+    """@ingroup plantuml_adapter
+    Check for each function allocated to a functional element if not allocated to any
+    functional element child: in that case => write function object string.
+    @param[in,out] string_obj current PlantUml text
+    @param[in] fun_elem functional element to check
+    @param[in] function_list list of functions
+    @param[in] xml_attribute_list xml list of attributes
+    @return None
+    """
+
+    for function in function_list:
+        if function.id in fun_elem.allocated_function_list:
+            fun_elem_child_allocated_function_list = []
+            for c in fun_elem.child_list:
+                for j in c.allocated_function_list:
+                    fun_elem_child_allocated_function_list.append(j)
+
+            if not any(s == function.id for s in fun_elem_child_allocated_function_list):
+                write_function_object(string_obj, function, [], [], False, xml_attribute_list)
+
+
+def recursive_decomposition(string_obj, main_fun_elem, function_list, xml_attribute_list,
+                            first_iter=False):
+    """@ingroup plantuml_adapter
+    Create PlantUml text for functional elements recursively
+    @param[in,out] string_obj current PlantUml text
+    @param[in] main_fun_elem
+    @param[in] function_list list of functions
+    @param[in] xml_attribute_list xml list of attributes
+    @param[in] first_iter
+    @return None
+    """
+
+    if first_iter is True:
+        string_obj.create_component(main_fun_elem)
+        check_child_allocation(string_obj, main_fun_elem, function_list, xml_attribute_list)
+        if main_fun_elem.child_list:
+            recursive_decomposition(string_obj, main_fun_elem, function_list, xml_attribute_list)
     else:
-        Logger.set_error(__name__,
-                        f"Jarvis does not know the functional Element {kwargs['diagram_object_str']}")
+        for c in main_fun_elem.child_list:
+            string_obj.create_component(c)
+            check_child_allocation(string_obj, c, function_list, xml_attribute_list)
+            if c.child_list:
+                recursive_decomposition(string_obj, c, function_list, xml_attribute_list)
+            string_obj.append_string('}\n')
+            string_obj.create_component_attribute(c, xml_attribute_list)
+        string_obj.create_component_attribute(main_fun_elem, xml_attribute_list)
+
+
+def get_fun_elem_decomposition(main_fun_elem, fun_elem_list, allocated_function_list, consumer_list,
+                               producer_list, external_function_list, xml_attribute_list,
+                               data_list, fun_inter_list):
+    """@ingroup plantuml_adapter
+    @anchor get_fun_elem_decomposition
+    Construct the PlantUml text for the functional element decomposition diagram
+    @param[in] main_fun_elem main functional element
+    @param[in] fun_elem_list functional element list
+    @param[in] allocated_function_list list of allocated functions to main functional element
+    @param[in] consumer_list filtered consumers list
+    @param[in] producer_list filtered producers list
+    @param[in] external_function_list filtered external functions list
+    @param[in] xml_attribute_list xml list of attributes
+    @param[in] data_list data list
+    @param[in] fun_inter_list functional interface list
+    @return PlantUml text of the diagram
+    """
+
+    string_obj = ObjDiagram()
+    interface_list = None
 
-    return plantuml_string
+    if fun_inter_list:
+        unmerged_data_list = get_exchanged_flows(consumer_list, producer_list, {})
+        interface_list, data_flow_list = get_interface_list(fun_inter_list,
+                                                            data_list,
+                                                            unmerged_data_list,
+                                                            allocated_function_list.
+                                                            union(external_function_list),
+                                                            fun_elem_list,
+                                                            is_decomposition=True)
 
+        data_flow_list = concatenate_flows(data_flow_list)
 
-def case_state_sequence_diagram(**kwargs):
-    """Case for 'show state sequence <state>'"""
-    plantuml_string = None
-    xml_state_name_list = get_objects_names(kwargs['xml_state_list'])
-    if kwargs['diagram_object_str'] in xml_state_name_list:
-        plantuml_string = show_state_allocated_function(kwargs['diagram_object_str'],
-                                                        kwargs['xml_state_list'],
-                                                        kwargs['xml_function_list'],
-                                                        kwargs['xml_consumer_function_list'],
-                                                        kwargs['xml_producer_function_list'],
-                                                        kwargs['xml_data_list'])
     else:
-        Logger.set_error(__name__,
-                        f"Jarvis does not know the State {kwargs['diagram_object_str']}")
+        # Filter consumers and producers list in order to create data flow
+        data_flow_list = get_exchanged_flows(consumer_list, producer_list, {}, concatenate=True)
 
-    return plantuml_string
+    # Write external functions that are not already allocated to external components
+    external_function_not_allocated_list = []
+    for function in external_function_list:
+        is_external = True
+        for fun_elem in fun_elem_list:
+            if any(a == function.id for a in fun_elem.allocated_function_list):
+                is_external = False
+
+        if is_external:
+            external_function_not_allocated_list.append(function)
+
+    for function in external_function_not_allocated_list:
+        string_obj.create_object(function, xml_attribute_list)
+
+    # Write functional element decompo recursively and add allocated functions
+    recursive_decomposition(string_obj, main_fun_elem, allocated_function_list, xml_attribute_list,
+                            first_iter=True)
+    string_obj.append_string('}\n')
+    string_obj.create_component_attribute(main_fun_elem, xml_attribute_list)
+    # Write external fun_elem
+    for elem in fun_elem_list:
+        if elem != main_fun_elem and elem.parent is None:
+            recursive_decomposition(string_obj, elem, external_function_list, xml_attribute_list,
+                                    first_iter=True)
+            string_obj.append_string('}\n')
+            string_obj.create_component_attribute(elem, xml_attribute_list)
+
+    # Write data flows
+    string_obj.create_data_flow(data_flow_list)
+    if interface_list:
+        string_obj.create_interface(interface_list)
+
+    return string_obj.string
+
+
+def get_sequence_diagram(function_list, consumer_function_list, producer_function_list,
+                         parent_child_dict, data_list, str_out=False):
+    """@ingroup plantuml_adapter
+    @anchor get_sequence_diagram
+    Construct the PlantUml text for the sequence diagrams
+    @param[in] function_list TBD
+    @param[in] consumer_function_list TBD
+    @param[in] producer_function_list TBD
+    @param[in] parent_child_dict TBD
+    @param[in] data_list TBD
+    @return PlantUml text of the diagram
+    """
 
+    seq_obj_string = SequenceDiagram()
 
-def case_no_diagram(**kwargs):
-    """Default Case when no command has been found"""
-    Logger.set_warning(__name__,
-                      f"Jarvis does not understand the command {kwargs['diagram_type_str']}")
+    message_list = get_exchanged_flows(consumer_function_list, producer_function_list,
+                                       parent_child_dict)
+    ordered_function_list, ordered_message_list = order_list(message_list, data_list)
+
+    if ordered_function_list:
+        for fun_name in ordered_function_list:
+            for f in function_list:
+                if fun_name == f.name.lower():
+                    seq_obj_string.create_participant(f)
+    else:
+        for f in function_list:
+            seq_obj_string.create_participant(f)
+
+    seq_obj_string.create_sequence_message(ordered_message_list)
+
+    return seq_obj_string.string
+
+
+def get_predecessor_list(data):
+    """@ingroup plantuml_adapter
+    Get the predecessor's list for a Data object
+    @param[in] data data object
+    @return predecessor list
+    """
 
+    predecessor_list = set()
+    if data.predecessor_list:
+        for predecessor in data.predecessor_list:
+            predecessor_list.add(predecessor)
+
+    return predecessor_list
+
+
+def check_sequence(predecessor_list, sequence):
+    """@ingroup plantuml_adapter
+    Check if predecessors of a data are in a sequence
+    @param[in] predecessor_list predecessor list
+    @param[in] sequence sequence
+    @return TRUE (predecessors are in the sequence) or FALSE
+    """
 
-def check_level_0_allocated_child(fun_elem, function):
-    """Returns True if the function can be "shown" by the functional element (i.e. no function
-    children allocated to fun_elem children => TODO: Clean 2 below methods"""
     check = False
-    if fun_elem.child_list == set():
-        check = True
-        return check
-    if function.child_list == set() and function.parent.id not in fun_elem.allocated_function_list:
-        check = True
+    if predecessor_list == set():
+        check = None
         return check
 
-    allocated_function_id_list = []
-    for fun_elem_child in fun_elem.child_list:
-        for elem in fun_elem_child.allocated_function_list:
-            allocated_function_id_list.append(elem)
-    child_list, _ = get_children(function)
-    child_id_list = [elem.id for elem in child_list]
-    if any(t in child_id_list for t in allocated_function_id_list) or not child_id_list:
-        check = False
-        return check
+    pred_set = set()
+    seq_set = set()
+    for pred in predecessor_list:
+        pred_set.add(pred.name)
+    for elem in sequence:
+        seq_set.add(elem[2].name)
 
-    if function.parent is not None:
-        if function.parent.id not in fun_elem.allocated_function_list:
-            check = True
-            return check
-    else:
+    if pred_set.issubset(seq_set):
         check = True
+        return check
 
     return check
 
 
-def get_level_0_function(fun_elem, function_list, allocated_function_list=None):
-    """Recursively get functions allocated to main_fun_elem and its descendant"""
-    if allocated_function_list is None:
-        allocated_function_list = set()
-        if fun_elem.child_list == set():
-            return allocated_function_list
-    for function_id in fun_elem.allocated_function_list:
-        for function in function_list:
-            if function.id == function_id and function not in allocated_function_list:
-                if check_level_0_allocated_child(fun_elem, function) is True:
-                    allocated_function_list.add(function)
-                if fun_elem.child_list != set():
-                    for child in fun_elem.child_list:
-                        get_level_0_function(child, function_list, allocated_function_list)
-
-    return allocated_function_list
-
-
-def show_fun_elem_decomposition(fun_elem_str, xml_function_list, xml_consumer_function_list,
-                                xml_producer_function_list, xml_fun_elem_list, xml_attribute_list,
-                                xml_data_list, xml_fun_inter_list, diagram_level=None):
-    """Creates lists with desired objects for <functional_element> decomposition, send them to
-    plantuml_adapter.py then returns plantuml_text"""
-    plantuml_text = None
-    main_fun_elem = check_get_object(fun_elem_str, **{'xml_fun_elem_list': xml_fun_elem_list})
-    if not main_fun_elem:
-        return plantuml_text
-    main_fun_elem.parent = None
-
-    c_inheritance = childs_inheritance(xml_function_list, xml_fun_elem_list, level=diagram_level)
-    attrib_inheritance = attribute_inheritance(xml_attribute_list,
-                                               xml_function_list,
-                                               xml_fun_elem_list,
-                                               xml_fun_inter_list)
-
-    func_alloc_inheritance = allocation_inheritance(xml_fun_elem_list, xml_function_list)
-    fun_inter_alloc_inheritance = allocation_inheritance(xml_fun_inter_list, xml_data_list)
-
-    if diagram_level:
-        xml_function_list, xml_fun_elem_list = filter_fun_elem_with_level(main_fun_elem,
-                                                                          diagram_level,
-                                                                          xml_function_list,
-                                                                          xml_fun_elem_list)
-
-    allocated_function_list = get_level_0_function(main_fun_elem, xml_function_list)
-
-    if allocated_function_list:
-        external_function_list, new_consumer_list, new_producer_list = \
-            get_cons_prod_from_allocated_functions(
-                allocated_function_list,
-                xml_producer_function_list,
-                xml_consumer_function_list)
-
-        for fun in external_function_list:
-            for child in fun.child_list.copy():
-                if not any(t == child for t in external_function_list):
-                    fun.child_list.remove(child)
-    else:
-        external_function_list, xml_fun_elem_list = set(), set()
-        new_consumer_list, new_producer_list = [], []
+def clean_predecessor_list(message_object_list):
+    """@ingroup plantuml_adapter
+    Delete predecessor if not in the message's list
+    @param[in] message_object_list TBD
+    @return updated message list
+    """
 
-    plantuml_text = plantuml_adapter.get_fun_elem_decomposition(main_fun_elem, xml_fun_elem_list,
-                                                                allocated_function_list,
-                                                                new_consumer_list,
-                                                                new_producer_list,
-                                                                external_function_list,
-                                                                xml_attribute_list,
-                                                                xml_data_list,
-                                                                xml_fun_inter_list)
-
-    reset_childs_inheritance(xml_function_list, xml_fun_elem_list, derived_child_id=c_inheritance[2])
-    reset_attribute_inheritance(xml_attribute_list, attrib_inheritance)
-    reset_alloc_inheritance(func_alloc_inheritance)
-    reset_alloc_inheritance(fun_inter_alloc_inheritance)
-
-    Logger.set_info(__name__,
-                   f"Decomposition Diagram for {fun_elem_str} generated")
-
-    return plantuml_text
-
-
-def filter_fun_elem_with_level(main_fun_elem, diagram_level, xml_function_list, xml_fun_elem_list):
-    """Clean unwanted fun_elem and functions from xml_lists then returns them"""
-    main_fun_elem_list, _ = get_children(main_fun_elem, level=diagram_level)
-    # Remove (child) elements from xml lists that are below the level asked
-    for unwanted_fun_elem in xml_fun_elem_list.symmetric_difference(main_fun_elem_list):
-        if not check_not_family(unwanted_fun_elem, main_fun_elem):
-            for fun in xml_function_list.copy():
-                if fun.id in unwanted_fun_elem.allocated_function_list:
-                    xml_function_list.remove(fun)
-            xml_fun_elem_list.remove(unwanted_fun_elem)
-    # Remove (child) elements from external fun_elem (main_fun_elem point of view)
-    for unwanted_fun_elem in xml_fun_elem_list.symmetric_difference(main_fun_elem_list):
-        if check_not_family(unwanted_fun_elem, main_fun_elem) and \
-                unwanted_fun_elem.parent is None:
-            curr_fun_elem_list, _ = get_children(unwanted_fun_elem, level=diagram_level)
-            for un_fun_elem in xml_fun_elem_list.symmetric_difference(curr_fun_elem_list):
-                if not check_not_family(unwanted_fun_elem, un_fun_elem):
-                    xml_fun_elem_list.remove(un_fun_elem)
-
-    return xml_function_list, xml_fun_elem_list
-
-
-def get_cons_prod_from_allocated_functions(allocated_function_list,
-                                           xml_producer_function_list,
-                                           xml_consumer_function_list):
-    """Get consumers/producers from function's allocated to main_fun_elem (and its descendant)"""
-    new_producer_list = []
-    new_consumer_list = []
-    for allocated_function in allocated_function_list:
-        allocated_function.child_list.clear()
-        allocated_function.parent = None
-        for elem in xml_producer_function_list:
-            if allocated_function in elem:
-                new_producer_list.append(elem)
-        for elem in xml_consumer_function_list:
-            if allocated_function in elem:
-                new_consumer_list.append(elem)
-
-    external_function_list, new_consumer_list, new_producer_list = get_ext_cons_prod(
-        new_producer_list,
-        new_consumer_list,
-        xml_producer_function_list,
-        xml_consumer_function_list)
-
-    return external_function_list, new_consumer_list, new_producer_list
-
-
-def get_ext_cons_prod(producer_list, consumer_list, xml_producer_function_list,
-                      xml_consumer_function_list):
-    """Get external cons/prod associated to main_fun_elem allocated functions"""
-    external_function_list = set()
-    for elem in consumer_list:
-        if not any(elem[0] in s for s in producer_list):
-            for prod in xml_producer_function_list:
-                if prod[0] == elem[0] and prod[1].parent is None:
-                    external_function_list.add(prod[1])
-                    if prod not in producer_list:
-                        producer_list.append(prod)
-
-    for elem in producer_list:
-        if not any(elem[0] in s for s in consumer_list):
-            for cons in xml_consumer_function_list:
-                if cons[0] == elem[0] and cons[1].parent is None:
-                    external_function_list.add(cons[1])
-                    if cons not in consumer_list:
-                        consumer_list.append(cons)
-
-    return external_function_list, consumer_list, producer_list
-
-
-def show_state_allocated_function(state_str, state_list, function_list, xml_consumer_function_list,
-                                  xml_producer_function_list, xml_data_list):
-    """Creates lists with desired objects for <state> function's allocation, send them to
-    plantuml_adapter.py then returns plantuml_text"""
-    allocated_function_id_list = set()
-    state_name = ''
-    for state in state_list:
-        if state_str in (state.name, state.alias):
-            if not state.allocated_function_list:
-                Logger.set_info(__name__,
-                               f"No function allocated to {state.name} (no display)")
-                return None
-
-            state_name = state.name
-            for fun_id in state.allocated_function_list:
-                allocated_function_id_list.add(fun_id)
+    for message in message_object_list:
+        pred_list = get_predecessor_list(message[2])
+        for pred in pred_list:
+            if not any(pred in s for s in message_object_list):
+                message[2].predecessor_list.remove(pred)
+
+    return message_object_list
+
+
+def get_sequence(message, message_object_list, sequence_list, sequence=None, index=None):
+    """@ingroup plantuml_adapter
+    Return a sequence for a given message
+    @param[in] message TBD
+    @param[in] message_object_list TBD
+    @param[in] sequence_list TBD
+    @param[in] sequence TBD
+    @param[in] index TBD
+    @return sequence
+    """
+    if not sequence:
+        sequence = []
+        index = 0
+    if message not in sequence and not any(message in s for s in sequence_list) is True:
+        message[3] = True
+        sequence.insert(index, message)
+        index += 1
+        for mess in message_object_list:
+            if message[2] in mess[2].predecessor_list:
+                get_sequence(mess, message_object_list, sequence_list, sequence, index)
+
+    return sequence
+
+
+def get_sequences(message_object_list):
+    """@ingroup plantuml_adapter
+    Group all sequences into a sequence list
+    @param[in] message_object_list
+    @return sequence list
+    """
 
-    for function in function_list:
-        if function.id in allocated_function_id_list.copy():
-            allocated_function_id_list.remove(function.id)
-            allocated_function_id_list.add(function.name)
-
-    diagram_str = show_functions_sequence(allocated_function_id_list, function_list,
-                                          xml_consumer_function_list, xml_producer_function_list,
-                                          xml_data_list, True)
-
-    diagram_str = f'box "{state_name}"\n{diagram_str}end box\n'
-
-    Logger.set_info(__name__,
-                   f"Function Sequence Diagram for {state_str} generated")
-
-    return diagram_str
-
-
-def show_fun_elem_function(fun_elem_str, xml_fun_elem_list, xml_function_list,
-                           xml_consumer_function_list, xml_producer_function_list, xml_type_list):
-    """Creates lists with desired objects for <functional_element> function's allocation,
-    send them to plantuml_adapter.py then returns plantuml_text"""
-    plantuml_text = None
-
-    main_fun_elem = check_get_object(fun_elem_str, **{'xml_fun_elem_list': xml_fun_elem_list})
-    if not main_fun_elem:
-        return plantuml_text
-
-    if not main_fun_elem.allocated_function_list:
-        Logger.set_info(__name__,
-                       f"No function allocated to {main_fun_elem.name} (no display)")
-        return plantuml_text
-
-    main_fun_elem.parent = None
-    main_fun_elem.child_list.clear()
-    new_function_list = {f for f in xml_function_list
-                         if f.id in main_fun_elem.allocated_function_list and f.parent is None}
-
-    if not new_function_list:
-        Logger.set_info(__name__,
-                       f"No parent function allocated to {main_fun_elem.name} (no display)")
-        return plantuml_text
-
-    new_consumer_list = get_cons_or_prod_paired(new_function_list,
-                                                xml_consumer_function_list,
-                                                xml_producer_function_list)
-
-    new_producer_list = get_cons_or_prod_paired(new_function_list,
-                                                xml_producer_function_list,
-                                                xml_consumer_function_list)
-
-    plantuml_text = plantuml_adapter.get_function_diagrams(new_function_list,
-                                                           new_consumer_list,
-                                                           new_producer_list,
-                                                           {}, None, xml_type_list)
-
-    Logger.set_info(__name__,
-                   f"Function Diagram for {fun_elem_str} generated")
-
-    return plantuml_text
-
-
-def get_cons_or_prod_paired(function_list, xml_flow_list, xml_opposite_flow_list):
-    """Get flow list if opposite flow is existing: e.g. if flow A is consumed and produced by
-    function within function_list => Add it"""
-    new_flow_list = []
-    for func in function_list:
-        # Flow = [Data_name, Function]
-        for flow in xml_flow_list:
-            if func in flow and flow not in new_flow_list:
-                # Oppo = [Data_name, Function]
-                for oppo in xml_opposite_flow_list:
-                    if oppo[0] == flow[0] and oppo[1] in function_list:
-                        new_flow_list.append(flow)
-                        break
-    return new_flow_list
-
-
-def show_fun_elem_context(fun_elem_str, xml_fun_elem_list, xml_function_list,
-                          xml_consumer_function_list, xml_producer_function_list,
-                          xml_attribute_list, xml_fun_inter_list, xml_data_list):
-    """Creates lists with desired objects for <functional_element> context, send them to
-    plantuml_adapter.py then returns plantuml_text"""
-
-    main_fun_elem = check_get_object(fun_elem_str, **{'xml_fun_elem_list': xml_fun_elem_list})
-    if not main_fun_elem:
-        return None
-
-    c_inheritance = childs_inheritance(xml_function_list, xml_fun_elem_list, level=None)
-    attrib_inheritance = attribute_inheritance(xml_attribute_list,
-                                               xml_function_list,
-                                               xml_fun_elem_list,
-                                               xml_fun_inter_list)
-    func_alloc_inheritance = allocation_inheritance(xml_fun_elem_list, xml_function_list)
-    fun_inter_alloc_inheritance = allocation_inheritance(xml_fun_inter_list, xml_data_list)
-
-    # Get allocated function to main_fun_elem
-    allocated_function_list = {f for f in xml_function_list
-                               if f.id in main_fun_elem.allocated_function_list}
-
-    new_function_list, cons, prod = get_allocated_function_context_lists(
-        allocated_function_list,
-        xml_consumer_function_list,
-        xml_producer_function_list)
-
-    fun_elem_list, interface_list, fun_elem_inter_list = get_fun_inter_for_fun_elem_context(
-        main_fun_elem, xml_fun_inter_list, xml_fun_elem_list)
-
-    for fun in new_function_list:
-        for elem in xml_fun_elem_list:
-            if any(z == fun.id for z in elem.allocated_function_list) and elem not in fun_elem_list:
-                fun_elem_list.add(elem)
-
-    for elem in fun_elem_list.copy():
-        for str_id in elem.allocated_function_list.copy():
-            if str_id not in [i.id for i in new_function_list]:
-                elem.allocated_function_list.remove(str_id)
-        if any(a == elem for a in main_fun_elem.child_list):
-            fun_elem_list.remove(elem)
-
-    plantuml_text = plantuml_adapter.get_fun_elem_context_diagram(new_function_list,
-                                                                  cons,
-                                                                  prod,
-                                                                  xml_data_list,
-                                                                  xml_attribute_list,
-                                                                  fun_elem_list,
-                                                                  interface_list,
-                                                                  fun_elem_inter_list)
-    
-    reset_childs_inheritance(xml_function_list, xml_fun_elem_list, derived_child_id=c_inheritance[2])
-    reset_attribute_inheritance(xml_attribute_list, attrib_inheritance)                            
-    reset_alloc_inheritance(func_alloc_inheritance)
-    reset_alloc_inheritance(fun_inter_alloc_inheritance)
-
-    Logger.set_info(__name__,
-                   f"Context Diagram for {fun_elem_str} generated")
-
-    return plantuml_text
-
-
-def get_allocated_function_context_lists(allocated_function_list,
-                                         xml_consumer_function_list,
-                                         xml_producer_function_list):
-    """For each function within allocated_function_list, asks the context of the function then
-    adds returned list from show_function_context() to current lists"""
-    new_function_list = set()
-    cons = []
-    prod = []
-    for fun in allocated_function_list:
-        if fun.parent is None:
-            returned_list = show_function_context(fun.name, allocated_function_list,
-                                                  xml_consumer_function_list,
-                                                  xml_producer_function_list, set(),
-                                                  set(), set(), list_out=True)
-            for k in returned_list[0]:
-                new_function_list.add(k)
-            for i in returned_list[1]:
-                if i not in cons:
-                    cons.append(i)
-            for j in returned_list[2]:
-                if j not in prod:
-                    prod.append(j)
-
-    return new_function_list, cons, prod
-
-
-def get_fun_inter_for_fun_elem_context(main_fun_elem, xml_fun_inter_list, xml_fun_elem_list):
-    """Get functional interfaces and associated functional elements"""
-    fun_elem_list = set()
-    interface_list = set()
-    fun_elem_inter_list = []
-
-    # Add main_fun_elem to filtered fun_elem_list and remove it from xml_fun_elem_list
-    fun_elem_list.add(main_fun_elem)
-    xml_fun_elem_list.remove(main_fun_elem)
-
-    # Get exposed interfaces of fun_elem
-    for interface in xml_fun_inter_list:
-        if any(i == interface.id for i in main_fun_elem.exposed_interface_list):
-            interface_list.add(interface)
-
-    # Get fun_elem pair for fun_inter
-    for fun_inter in interface_list:
-        for fun_elem in xml_fun_elem_list:
-            if any(i == fun_inter.id for i in fun_elem.exposed_interface_list):
-                if get_highest_fun_elem_exposing_fun_inter(fun_inter, fun_elem) and \
-                        check_not_family(main_fun_elem, fun_elem):
-                    fun_elem_list.add(fun_elem)
-                    if [main_fun_elem, fun_elem, fun_inter] not in fun_elem_inter_list:
-                        fun_elem_inter_list.append([main_fun_elem, fun_elem, fun_inter])
+    sequence_list = []
+    for message in message_object_list:
+        if not message[2].predecessor_list:
+            sequence = get_sequence(message, message_object_list, sequence_list)
+            sequence_list.append(sequence)
+
+    return sequence_list
 
-    return fun_elem_list, interface_list, fun_elem_inter_list
 
+def post_check_sequence(sequence_list):
+    """@ingroup plantuml_adapter
+    Check if message isn't missing in sequence, insert it at the good place and loop if not
+    well ordered (predecessor after each one)
+    @param[in] sequence_list TBD
+    @return sequence list ordered
+    """
 
-def get_highest_fun_elem_exposing_fun_inter(fun_inter, fun_elem):
-    """Retruns True if it's highest fun_elem exposing fun_inter"""
-    check = False
-    if not fun_elem.parent:
-        check = True
-    elif not any(a == fun_inter.id for a in fun_elem.parent.exposed_interface_list):
-        check = True
+    for (idx, i) in enumerate(sequence_list):
+        pred = i[2].predecessor_list
+        if check_sequence(pred, sequence_list[:idx]) is True:
+            pass
+        elif check_sequence(pred, sequence_list[:idx]) is False:
+            for (index, elem) in enumerate(sequence_list.copy()):
+                curr_pred = elem[2].predecessor_list
+                if check_sequence(curr_pred, sequence_list[:index]) is True:
+                    sequence_list.remove(i)
+                    sequence_list.insert(index + 1, i)
+                    index += 1
+                else:
+                    continue
+        elif check_sequence(pred, sequence_list[:idx]) is None:
+            pass
+        idx += 1
+
+    for (new_idx, message) in enumerate(sequence_list):
+        new_pred = message[2].predecessor_list
+        if check_sequence(new_pred, sequence_list[:new_idx]) is False:
+            post_check_sequence(sequence_list)
+
+    return sequence_list
+
+
+def get_sequence_list(message_object_list):
+    """@ingroup plantuml_adapter
+    Call for sequences then clean_up and post_check
+    @param[in] message_object_list TBD
+    @return sequence list
+    """
+    sequence_list = get_sequences(message_object_list)
 
-    return check
+    sequence_list = sorted(sequence_list, key=lambda x: len(x), reverse=True)
+    # Could be possible to implement this part within post_check_sequence()
+    for (index, i) in enumerate(sequence_list):
+        main_list = sequence_list[0]
+        if index > 0:
+            start = 0
+            for j in i.copy():
+                if not j[2].predecessor_list:
+                    i.remove(j)
+                    main_list.insert(start, j)
+                    start += 1
+
+    sequence_list = [item for sub in sequence_list for item in sub]
+    sequence_list = post_check_sequence(sequence_list)
+
+    return sequence_list
+
+
+def order_list(message_list, data_list):
+    """@ingroup plantuml_adapter
+    Order functions and messages
+    @param[in] message_list TBD
+    @param[in] data_list TBD
+    @return ordered message list and ordered function list
+    """
 
+    ordered_message_list = []
+    ordered_function_list = []
+    message_object_list = []
+
+    for i in message_list:
+        for data in data_list:
+            if i[2] == data.name:
+                message_object_list.append([i[0], i[1], data, False])
+
+    message_object_list = clean_predecessor_list(message_object_list)
+    ordored_message_object_list = get_sequence_list(message_object_list)
+
+    # Add index for each item within the list
+    for idx, t in enumerate(ordored_message_object_list):
+        ordered_message_list.insert(idx, [t[0], t[1], t[2].name, t[3]])
+
+    # Create the ordered(from ordered message list) function's list
+    # Starting with producers
+    for idx, m in enumerate(ordered_message_list):
+        if m[0] not in ordered_function_list:
+            ordered_function_list.insert(idx, m[0])
+    # Finishing with consumers
+    for j in message_list:
+        if j[1] not in ordered_function_list:
+            ordered_function_list.append(j[1])
+
+    return ordered_function_list, ordered_message_list
+
+
+def get_exchanged_flows(consumer_function_list, producer_function_list, parent_child_dict,
+                        concatenate=False):
+    """@ingroup plantuml_adapter
+    Return list of exchanged flows [[producer, consumer, data]], i.e. data that have
+    producer and consumer
+    @param[in] consumer_function_list TBD
+    @param[in] producer_function_list TBD
+    @param[in] parent_child_dict TBD
+    @param[in] concatenate TBD
+    @return list of exchanged flows
+    """
 
-def show_fun_elem_state_machine(fun_elem_str, xml_state_list, xml_transition_list,
-                                xml_fun_elem_list):
-    """Creates lists with desired objects for <functional_element> state, send them to
-    plantuml_adapter.py then returns plantuml_text"""
-    new_fun_elem_list = set()
-
-    main_fun_elem = check_get_object(fun_elem_str, **{'xml_fun_elem_list': xml_fun_elem_list})
-    if not main_fun_elem:
-        # TODO error message
-        return None
-
-    if not main_fun_elem.allocated_state_list:
-        Logger.set_error(__name__,
-                        f"No state allocated to {main_fun_elem.name} (no display)")
-        return None
-
-    new_fun_elem_list.add(main_fun_elem)
-
-    new_state_list = {s for s in xml_state_list if s.id in main_fun_elem.allocated_state_list}
-
-    new_transition_list = get_transitions(new_state_list, xml_transition_list)
-
-    plantuml_text = plantuml_adapter.get_state_machine_diagram(new_state_list,
-                                                               new_transition_list,
-                                                               xml_fun_elem_list)
-
-    Logger.set_info(__name__,
-                   f"State Machine Diagram for {fun_elem_str} generated")
-
-    return plantuml_text
-
-
-def get_transitions(state_list, xml_transition_list):
-    """Get transitions if state(s) from state_list are source/destination"""
-    new_transition_list = set()
-    for new_state in state_list:
-        for transition in xml_transition_list:
-            if new_state.id == transition.source:
-                new_transition_list.add(transition)
-            if new_state.id == transition.destination:
-                new_transition_list.add(transition)
-
-    return new_transition_list
-
-
-def show_states_chain(state_list_str, xml_state_list, xml_transition_list):
-    """Creates lists with desired objects for <states> chain, send them to plantuml_adapter.py
-    then returns plantuml_text"""
-    new_state_list = set()
-    for state_str in state_list_str:
-        for state in xml_state_list:
-            if state_str in (state.name, state.alias):
-                state.child_list.clear()
-                state.set_parent(None)
-                new_state_list.add(state)
-
-    new_transition_list = get_transitions(new_state_list, xml_transition_list)
-
-    plantuml_text = plantuml_adapter.get_state_machine_diagram(new_state_list,
-                                                               new_transition_list)
-    spaced_state_list = ", ".join(state_list_str)
-    if len(state_list_str) == 1:
-        Logger.set_info(__name__,
-                       f"Context Diagram {str(spaced_state_list)} generated")
-    else:
-        Logger.set_info(__name__,
-                       f"Chain Diagram {str(spaced_state_list)} generated")
+    output_list = []
 
-    return plantuml_text
+    for producer_flow, producer_function in producer_function_list:
+        Logger.set_debug(__name__, f'Producer flow: {producer_flow}; '
+                                   f'function: {producer_function.id}, {producer_function.name}')
+        if not producer_function.child_list or not parent_child_dict:
+            for cons_flow, consumer_function in consumer_function_list:
+                Logger.set_debug(__name__, f'Consumer flow: {cons_flow}; '
+                                           f'function: {consumer_function.id}, {consumer_function.name}')
+                if (not consumer_function.child_list or not parent_child_dict) and cons_flow == producer_flow:
+                    output_list.append(
+                        [producer_function.name.lower(), consumer_function.name.lower(),
+                         producer_flow])
 
+    if concatenate:
+        output_list = concatenate_flows(output_list)
 
-def show_functions_sequence(function_list_str, xml_function_list, xml_consumer_function_list,
-                            xml_producer_function_list, xml_data_list, str_out=False):
-    """Creates lists with desired objects for <functions> sequence, send them to plantuml_adapter.py
-    then returns plantuml_text"""
-    new_function_list = set()
+    return output_list
 
-    for i in function_list_str:
-        fun = check_get_object(i, **{'xml_function_list': xml_function_list})
-        if not fun:
-            continue
-        fun.child_list.clear()
-        new_function_list.add(fun)
 
-    new_consumer_list = get_cons_or_prod_paired(new_function_list,
-                                                xml_consumer_function_list,
-                                                xml_producer_function_list)
-
-    new_producer_list = get_cons_or_prod_paired(new_function_list,
-                                                xml_producer_function_list,
-                                                xml_consumer_function_list)
-    # (Re)Filter data_list with only produced(same data in consumed since paired) and functions
-    # asked for sequence i.e. new_function_list used in get_cons_or_prod_paired()
-    # => TBC/TBT
-    new_data_list = {s for s in xml_data_list if any(s.name in j for j in new_producer_list)}
-
-    for new_data in new_data_list:
-        for pred in new_data.predecessor_list.copy():
-            if pred not in new_data_list:
-                new_data.predecessor_list.remove(pred)
-
-    plantuml_text = plantuml_adapter.get_sequence_diagram(new_function_list,
-                                                          new_consumer_list,
-                                                          new_producer_list,
-                                                          {},
-                                                          new_data_list, str_out)
-    if not str_out:
-        Logger.set_info(__name__,
-                       "Sequence Diagram " + str(", ".join(function_list_str)) + " generated")
-
-    return plantuml_text
-
-
-def show_functions_chain(function_list_str, xml_function_list, xml_consumer_function_list,
-                         xml_producer_function_list, xml_type_list):
-    new_function_list = set()
-    new_parent_dict = {}
-    new_producer_list = []
-    new_consumer_list = []
-    for i in function_list_str:
-        for fun in xml_function_list:
-            if i == fun.name or i == fun.alias:
-                new_function_list.add(fun)
-                if fun.parent:
-                    new_parent_dict[fun.id] = fun.parent.id
-                    if fun.parent not in new_function_list:
-                        new_function_list.add(fun.parent)
-                        fun.parent.child_list.clear()
-                    fun.parent.add_child(fun)
-                for xml_consumer_flow, xml_consumer in xml_consumer_function_list:
-                    if fun == xml_consumer:
-                        fun.child_list.clear()
-                        if [xml_consumer_flow, fun] not in new_consumer_list and \
-                                [xml_consumer_flow, fun] not in xml_producer_function_list:
-                            new_consumer_list.append([xml_consumer_flow, fun])
-                for xml_producer_flow, xml_producer in xml_producer_function_list:
-                    if fun == xml_producer:
-                        fun.child_list.clear()
-                        if [xml_producer_flow, fun] not in new_producer_list and \
-                                [xml_producer_flow, fun] not in xml_consumer_function_list:
-                            new_producer_list.append([xml_producer_flow, fun])
-
-    plantuml_text = plantuml_adapter.get_function_diagrams(new_function_list,
-                                                           new_consumer_list,
-                                                           new_producer_list,
-                                                           new_parent_dict,
-                                                           None,
-                                                           xml_type_list)
-
-    Logger.set_info(__name__,
-                   f'Chain Diagram {str(", ".join(function_list_str))} generated')
-
-    return plantuml_text
-
-
-# TODO: Clean-up once inheritance has been validated (Create method for Function and others
-#  objects?)
-def show_function_decomposition(diagram_function_str, xml_function_list, xml_consumer_function_list,
-                                xml_producer_function_list, xml_attribute_list, xml_type_list,
-                                diagram_level=None):
-    """Create necessary lists then returns plantuml text for decomposition of function"""
-    main_fun = check_get_object(diagram_function_str, **{'xml_function_list': xml_function_list})
-    if not main_fun:
-        return
-    main_parent = main_fun.parent
-
-    c_inheritance = childs_inheritance(xml_function_list, level=diagram_level)
-    a_inheritance = attribute_inheritance(xml_attribute_list, xml_function_list)
-
-    if diagram_level:
-        full_fun_list, _ = get_children(main_fun)
-        main_function_list, main_parent_dict = get_children(main_fun, level=diagram_level)
-        # derived = childs_inheritance(main_fun, level=diagram_level)
-        # if derived:
-        #     main_function_list = main_function_list.union(derived[0])
-        #     main_parent_dict.update(derived[1])
-
-        for k in full_fun_list.symmetric_difference(main_function_list):
-            for cons in xml_consumer_function_list.copy():
-                if k in cons:
-                    xml_consumer_function_list.remove(cons)
-                    if [cons[0], k.parent] in xml_consumer_function_list:
-                        xml_consumer_function_list.remove([cons[0], k.parent])
-
-            for prod in xml_producer_function_list.copy():
-                if k in prod:
-                    xml_producer_function_list.remove(prod)
-                    if [prod[0], k.parent] in xml_producer_function_list:
-                        xml_producer_function_list.remove([prod[0], k.parent])
-    else:
-        main_function_list, main_parent_dict = get_children(main_fun)
-        # derived = childs_inheritance(main_fun)
-        # if derived:
-        #     main_function_list = main_function_list.union(derived[0])
-        #     main_parent_dict.update(derived[1])
-
-    main_consumer_list = check_get_child_flows(main_function_list, xml_consumer_function_list)
-    main_producer_list = check_get_child_flows(main_function_list, xml_producer_function_list)
-
-    ext_prod_fun_list, ext_producer_list, ext_prod_parent_dict = get_external_flow_with_level(
-        main_consumer_list, main_function_list, main_fun, xml_producer_function_list, diagram_level)
-
-    ext_cons_fun_list, ext_consumer_list, ext_cons_parent_dict = get_external_flow_with_level(
-        main_producer_list, main_function_list, main_fun, xml_consumer_function_list, diagram_level)
-
-    new_function_list = main_function_list.union(ext_prod_fun_list).union(ext_cons_fun_list)
-    new_consumer_list = main_consumer_list + ext_consumer_list
-    new_producer_list = main_producer_list + ext_producer_list
-    new_parent_dict = {**main_parent_dict, **ext_cons_parent_dict, **ext_prod_parent_dict}
-
-    for function in new_function_list:
-        if main_parent and function.parent is main_parent:
-            function.parent = None
-        if function.child_list:
-            for j in function.child_list.copy():
-                if j not in new_function_list:
-                    function.child_list.remove(j)
-
-    plantuml_text = plantuml_adapter.get_function_diagrams(new_function_list,
-                                                           new_consumer_list,
-                                                           new_producer_list,
-                                                           new_parent_dict,
-                                                           None,
-                                                           xml_type_list,
-                                                           xml_attribute_list=xml_attribute_list)
-
-    reset_childs_inheritance(xml_function_list, derived_child_id=c_inheritance[2])
-    reset_attribute_inheritance(xml_attribute_list, a_inheritance)
-
-    Logger.set_info(__name__,
-                   f"Decomposition Diagram {diagram_function_str} generated")
-
-    return plantuml_text
-
-
-def get_external_flow_with_level(main_flow_list, main_function_list, main_fun, xml_flow_list,
-                                 level):
-    """Returns external functions list, flow lists and parent dict"""
-    ext_flow_fun_list = set()
-    ext_flow_list = []
-    ext_flow_parent_dict = {}
-    for flow, _ in main_flow_list:
-        for xml_flow, xml_fun in xml_flow_list:
-            if flow == xml_flow and xml_fun.parent == main_fun.parent:
-                ext_flow_fun_list.add(xml_fun)
-            elif flow == xml_flow and check_not_family(main_fun, xml_fun) and \
-                    xml_fun.parent is None:
-                ext_flow_fun_list.add(xml_fun)
-            elif flow == xml_flow and not check_parentality(xml_fun, main_fun) and \
-                    [xml_flow, xml_fun.parent] not in xml_flow_list:
-                ext_flow_fun_list.add(xml_fun)
-
-    for fun in ext_flow_fun_list.copy():
-        if fun.child_list:
-            function_list_dict = get_children(fun, level=level)
-            ext_flow_fun_list.update(function_list_dict[0])
-            ext_flow_parent_dict.update(function_list_dict[1])
-
-    for flow, _ in main_flow_list:
-        for xml_flow, xml_fun in xml_flow_list:
-            if flow == xml_flow and xml_fun in ext_flow_fun_list and \
-                    xml_fun not in main_function_list:
-                # ext_flow_list.append([xml_flow, xml_fun])
-                if not xml_fun.child_list:
-                    if [xml_flow, xml_fun] not in ext_flow_list:
-                        ext_flow_list.append([xml_flow, xml_fun])
-                else:
-                    temp = []
-                    for k in xml_fun.child_list:
-                        temp.append([xml_flow, k])
-                    if not any(t in temp for t in xml_flow_list):
-                        if [xml_flow, xml_fun] not in ext_flow_list:
-                            ext_flow_list.append([xml_flow, xml_fun])
-
-    for fun in ext_flow_fun_list.copy():
-        if not any(a == fun for a in [i[1] for i in ext_flow_list]) and not fun.child_list:
-            ext_flow_fun_list.remove(fun)
-    for fun in ext_flow_fun_list.copy():
-        if not any(a == fun for a in [i[1] for i in ext_flow_list]) and \
-                not any(i in fun.child_list for i in ext_flow_fun_list) and \
-                fun != main_fun:
-            ext_flow_fun_list.remove(fun)
-
-    return ext_flow_fun_list, ext_flow_list, ext_flow_parent_dict
-
-
-def check_get_child_flows(function_list, xml_flow_list, new_flow_list=None):
-    """Get flow_list associated with function_list and xml_flow_list"""
-    if new_flow_list is None:
-        new_flow_list = []
-    for f in function_list:
-        for xml_flow, xml_function in xml_flow_list:
-            if f == xml_function:
-                if not xml_function.child_list:
-                    if [xml_flow, xml_function] not in new_flow_list:
-                        new_flow_list.append([xml_flow, xml_function])
-                else:
-                    temp_list = []
-                    for c in xml_function.child_list:
-                        if [xml_flow, c] in xml_flow_list:
-                            temp_list.append([xml_flow, c])
-
-                    if not any(xml_flow in s for s in temp_list):
-                        if [xml_flow, xml_function] not in new_flow_list:
-                            new_flow_list.append([xml_flow, xml_function])
-
-    return new_flow_list
-
-
-def show_function_context(diagram_function_str, xml_function_list, xml_consumer_function_list,
-                          xml_producer_function_list, xml_data_list, xml_attribute_list,
-                          xml_type_list, list_out=False):
-    """Create necessary lists then returns plantuml text for context of function"""
-    new_function_list = set()
-    new_parent_dict = {}
-    new_producer_list = []
-    new_consumer_list = []
-    main = None
-
-    c_inheritance = childs_inheritance(xml_function_list)
-    a_inheritance = attribute_inheritance(xml_attribute_list, xml_function_list)
-
-    for fun in xml_function_list:
-        if diagram_function_str in (fun.name, fun.alias):
-            new_function_list.add(fun)
-            main = fun
-            for xml_producer_flow, xml_producer in xml_producer_function_list:
-                if fun == xml_producer:
-                    check = False
-                    for flow, consumer in xml_consumer_function_list:
-                        if xml_producer_flow == flow:
-                            if consumer.parent is None:
-                                current_func, current_dict = get_children(fun)
-                                parent_check = check_parentality(consumer, main)
-                                if consumer not in current_func and parent_check is False:
-                                    new_consumer_list.append([xml_producer_flow, consumer])
-                                    new_function_list.add(consumer)
-                                    check = True
-                            elif main.parent == consumer.parent and consumer != main:
-                                new_consumer_list.append([flow, consumer])
-                                new_function_list.add(consumer)
-                                check = True
-                    if check:
-                        if [xml_producer_flow, xml_producer] not in new_producer_list:
-                            new_producer_list.append([xml_producer_flow, xml_producer])
-
-                    if not any(xml_producer_flow in s for s in xml_consumer_function_list):
-                        if [xml_producer_flow, xml_producer] not in new_producer_list:
-                            new_producer_list.append([xml_producer_flow, xml_producer])
-
-    if main is not None:
-        for xml_consumer_flow, xml_consumer in xml_consumer_function_list:
-            if xml_consumer == main:
-                check = False
-                for flow, producer in xml_producer_function_list:
-                    if flow == xml_consumer_flow:
-                        if producer.parent is None:
-                            current_func, current_dict = get_children(producer)
-                            if main not in current_func:
-                                new_producer_list.append([flow, producer])
-                                new_function_list.add(producer)
-                                check = True
-                        elif main.parent == producer.parent and producer != main:
-                            new_producer_list.append([flow, producer])
-                            new_function_list.add(producer)
-                            check = True
-                if check:
-                    if [xml_consumer_flow, xml_consumer] not in new_consumer_list:
-                        new_consumer_list.append([xml_consumer_flow, xml_consumer])
-
-                if not any(xml_consumer_flow in s for s in xml_producer_function_list):
-                    if [xml_consumer_flow, xml_consumer] not in new_consumer_list:
-                        new_consumer_list.append([xml_consumer_flow, xml_consumer])
+def get_output_flows(consumer_function_list, producer_function_list, concatenate=False):
+    """@ingroup plantuml_adapter
+    Return list of output flows [[None/parent_name, producer, data]], i.e. data that
+    have only producer
+    @param[in] consumer_function_list TBD
+    @param[in] producer_function_list TBD
+    @param[in] concatenate TBD
+    @return list of output flows
+    """
+    flow_consumer_name_list = []
+    flow_child_consumer_list = []
+    temp_input_list = []
+    output_list = []
+
+    for flow, cons in consumer_function_list:
+        flow_consumer_name_list.append([flow, cons.name.lower()])
+        if cons.child_list is not None:
+            for child in cons.child_list:
+                flow_child = [flow, child.name.lower()]
+                if [flow, child] in consumer_function_list:
+                    flow_child_consumer_list.append(flow_child)
+
+    for consumer_flow, consumer_function in consumer_function_list:
+        if len(consumer_function.child_list) > 0:
+            if len(flow_child_consumer_list) > 0:
+                if not any(consumer_flow in sublist for sublist in flow_child_consumer_list):
+                    temp_input_list.append([consumer_function.name.lower(), consumer_flow])
+            if len(flow_child_consumer_list) == 0:
+                temp_input_list.append([consumer_function.name.lower(), consumer_flow])
+
+    for producer_flow, producer_function in producer_function_list:
+        # TODO to be checked because returns flow with both producer and consumer (same output as get_exchanged_flows)
+        # for name, flow in temp_input_list:
+        #     if producer_flow == flow:
+        #         flow_child_consumer_list = [name, producer_function.name.lower(), producer_flow]
+        #         output_list.append(flow_child_consumer_list)
+
+        # Looking for outputs (i.e. flow with only producer's function)
+        if not any(producer_flow in sublist for sublist in flow_consumer_name_list):
+            if not any(producer_flow in sub for sub in output_list):
+                output_list.append([None, producer_function.name.lower(), producer_flow])
 
-    for f in new_function_list:
-        f.child_list.clear()
+    if concatenate:
+        output_list = concatenate_flows(output_list)
 
-    if list_out:
-        out = new_function_list, new_consumer_list, new_producer_list
-    else:
-        out = plantuml_adapter.get_function_diagrams(
-            new_function_list,
-            new_consumer_list,
-            new_producer_list,
-            new_parent_dict,
-            xml_data_list,
-            xml_type_list,
-            xml_attribute_list=xml_attribute_list)
+    return output_list
 
-        Logger.set_info(__name__,
-                       f"Context Diagram {diagram_function_str} generated")
 
-    reset_childs_inheritance(xml_function_list, derived_child_id=c_inheritance[2])
-    reset_attribute_inheritance(xml_attribute_list, a_inheritance)
+def get_input_flows(consumer_function_list, producer_function_list, concatenate=False):
+    """@ingroup plantuml_adapter
+    Return list of input flow [[None/parent_name, consumer, data]], i.e. data that
+    have only consumer
+    @param[in] consumer_function_list TBD
+    @param[in] producer_function_list TBD
+    @param[in] concatenate TBD
+    @return list of input flows
+    """
 
-    return out
+    flow_producer_name_list = []
+    flow_child_producer_list = []
+    temp_input_list = []
+    output_list = []
+
+    for flow, prod in producer_function_list:
+        flow_producer_name_list.append([flow, prod.name.lower()])
+        if prod.child_list is not None:
+            for child in prod.child_list:
+                flow_child = [flow, child.name.lower()]
+                if [flow, child] in producer_function_list:
+                    flow_child_producer_list.append(flow_child)
+
+    for producer_flow, producer_function in producer_function_list:
+        if len(producer_function.child_list) > 0:
+            if len(flow_child_producer_list) > 0:
+                if not any(producer_flow in sublist for sublist in flow_child_producer_list):
+                    temp_input_list.append([producer_function.name.lower(), producer_flow])
+            if len(flow_child_producer_list) == 0:
+                temp_input_list.append([producer_function.name.lower(), producer_flow])
+
+    for cons_flow, consumer_fun in consumer_function_list:
+        # TODO to be checked because returns flow with both producer and consumer (same output as get_exchanged_flows)
+        # for name, flow in temp_input_list:
+        #     if cons_flow == flow:
+        #         flow_child_producer_list = [name, consumer_fun.name.lower(), cons_flow]
+        #         output_list.append(flow_child_producer_list)
+
+        if not any(cons_flow in sublist for sublist in flow_producer_name_list):
+            if not any(cons_flow in sublist for sublist in output_list):
+                output_list.append([None, consumer_fun.name.lower(), cons_flow])
+
+    if concatenate:
+        output_list = concatenate_flows(output_list)
+    return output_list
 
 
-def get_fun_inter_sequence_diagram(fun_inter_str, **kwargs):
+def concatenate_flows(input_list):
+    """@ingroup plantuml_adapter
+    Concatenate the flows with same consumer and producer: from [[cons=A, prod=B, flow_1],
+    [cons=A, prod=B, flow_2]] to [[cons=A, prod=B, [flow_1, flow_2]].
+    Adaptation for flow notation in PlantUml
+    @param[in] input_list
+    @return list of output flows
     """
-    Check and get all "show sequence Fun_inter" strings, find Fun_inter obj and then get/filter
-    needed lists for plantuml_adapter.
-    Args:
-        fun_inter_str: functional interface name/alias from input cell
-        **kwargs: whole lists
-
-    Returns:
-        plantuml_text (str) : plantuml text
-    """
-    new_consumer_list = []
-    new_producer_list = []
-    new_fun_elem_list = set()
-    fun_inter = check_get_object(
-        fun_inter_str, **{'xml_fun_inter_list': kwargs['xml_fun_inter_list']})
-
-    if fun_inter:
-        data_list_fun_inter = switch_data(fun_inter, None, **kwargs)['data']
-        for elem in data_list_fun_inter:
-            fun_elem_cons = check_get_object(
-                elem['Last consumer Functional element(s)'].pop(),
-                **{'xml_fun_elem_list': kwargs['xml_fun_elem_list']})
-            fun_elem_prod = check_get_object(
-                elem['Last producer Functional element(s)'].pop(),
-                **{'xml_fun_elem_list': kwargs['xml_fun_elem_list']})
-            if fun_elem_cons and fun_elem_prod:
-                new_consumer_list.append([elem['Data'], fun_elem_cons])
-                new_producer_list.append([elem['Data'], fun_elem_prod])
-                new_fun_elem_list.add(fun_elem_cons)
-                new_fun_elem_list.add(fun_elem_prod)
-
-    if new_consumer_list and new_producer_list:
-        plantuml_text = plantuml_adapter.get_sequence_diagram(new_fun_elem_list,
-                                                              new_consumer_list,
-                                                              new_producer_list,
-                                                              {},
-                                                              kwargs['xml_data_list'])
 
-        return plantuml_text
+    output_list = []
+    per_function_name_filtered_list = set(map(lambda x: (x[0], x[1]), input_list))
+    per_flow_filtered_list = [[y[2] for y in input_list if y[0] == x and y[1] == z] for x, z in
+                              per_function_name_filtered_list]
+    for idx, function in enumerate(per_function_name_filtered_list):
+        output_list.append([function, per_flow_filtered_list[idx]])
 
-    else:
-        Logger.set_warning(__name__,
-                          f"No data found for {fun_inter.name}")
+    return output_list
 
 
-def get_fun_elem_sequence_diagram(fun_elem_str, **kwargs):
+def get_state_machine_diagram(xml_state_list, xml_transition_list, fun_elem_list=None):
+    """@ingroup plantuml_adapter
+    @anchor get_state_machine_diagram
+    Construct  the PlantUml text and url for state machine diagrams
+    @param[in] xml_state_list TBD
+    @param[in] xml_transition_list TBD
+    @param[in] fun_elem_list TBD
+    @return PlantUml text and url diagram for state machine diagram
     """
-    Check and get all "show sequence Fun_elem_A, Fun_elem_B, ..." strings, find objects and
-    then get/filter needed lists for plantuml_adapter.
-    Args:
-        fun_elem_str: functional elements name/alias from input cell
-        **kwargs: dict with whole lists/sets
-
-    Returns:
-        plantuml_text (str) : plantuml_text
-    """
-    new_consumer_list = []
-    new_producer_list = []
-
-    new_fun_elem_list = {
-        check_get_object(i, **{'xml_fun_elem_list': kwargs['xml_fun_elem_list']}) 
-        for i in fun_elem_str
-        }
-
-    for fun_elem in new_fun_elem_list:
-        temp_fun_set = get_allocation_object(
-            fun_elem, 
-            kwargs['xml_function_list']
-            )
-
-        if isinstance(fun_elem.derived, FunctionalElement):
-            get_derived_if_in_view = filter_allocated_item_from_view(
-                {fun_elem.derived}, kwargs['xml_view_list']
-                )
-            # If type(list) has been returned from activated View()
-            # then add it's allocated func
-            if isinstance(get_derived_if_in_view, list):
-                alloc_derived_func_set = get_allocation_object(
-                    fun_elem.derived, 
-                    kwargs['xml_function_list']
-                    )
-                if alloc_derived_func_set is not None and temp_fun_set is not None:
-                        allocated_fun_set.update(alloc_derived_func_set)
-                    
-
-        if temp_fun_set is not None:
-            for fun in temp_fun_set:
-                new_consumer_list.extend(
-                    get_fun_elem_for_cons_prod_lists(
-                    fun_elem, fun, kwargs['xml_consumer_function_list']
-                    )
-                )
-                new_producer_list.extend(
-                    get_fun_elem_for_cons_prod_lists(
-                    fun_elem, fun, kwargs['xml_producer_function_list']
-                    )
-                )
-
-        fun_elem.child_list.clear()
-        fun_elem.parent = None
-
-    if new_consumer_list and new_producer_list:
-
-        for i in new_consumer_list:
-            if not any(i[0] in s for s in new_producer_list):
-                new_consumer_list.remove(i)
-        
-        for j in new_producer_list:
-            if not any(j[0] in s for s in new_consumer_list):
-                new_producer_list.remove(j)
-
-    if new_consumer_list and new_producer_list:
-        plantuml_text = plantuml_adapter.get_sequence_diagram(new_fun_elem_list,
-                                                              new_consumer_list,
-                                                              new_producer_list,
-                                                              {},
-                                                              kwargs['xml_data_list'])
 
-        return plantuml_text
+    state_obj_string = StateDiagram()
+    objects_conditions_list = get_objects_conditions_list(xml_state_list, xml_transition_list)
+    already_added_state_id_list = []
+    for state in xml_state_list:
+        if not state.parent and state.child_list:
+            check = False
+            if fun_elem_list:
+                for fun_elem in fun_elem_list:
+                    if state.id in fun_elem.allocated_state_list:
+                        if fun_elem.parent is None:
+                            check = True
+                            state_obj_string.create_state(fun_elem, True)
 
-    else:
-        Logger.set_warning(__name__,
-                          f"Not any data allocated to interfaces exposed by {', '.join(fun_elem_str)}")
+            write_composed_state(state_obj_string, state, already_added_state_id_list,
+                                 objects_conditions_list)
+            if check:
+                state_obj_string.append_string('}\n')
+
+    for s in xml_state_list:
+        if s.id not in already_added_state_id_list:
+            check = False
+            if fun_elem_list:
+                for fun_elem in fun_elem_list:
+                    if s.id in fun_elem.allocated_state_list:
+                        if fun_elem.parent is None:
+                            check = True
+                            state_obj_string.create_state(fun_elem, True)
+            write_state(state_obj_string, s, already_added_state_id_list, objects_conditions_list)
+            if check:
+                state_obj_string.append_string('}\n')
+
+    for p in objects_conditions_list.copy():
+        if (p[0].id and not p[1].id) or (not p[0].id and p[1].id):
+            state_obj_string.create_transition([p])
+            objects_conditions_list.remove(p)
+
+    return state_obj_string.string
+
+
+def get_objects_conditions_list(xml_state_list, xml_transition_list):
+    """@ingroup plantuml_adapter
+    Return all conditions associated to a list of state within a list of transition
+    @param[in] xml_state_list TBD
+    @param[in] xml_transition_list TBD
+    @return conditions list
+    """
 
+    objects_conditions_list = []
+    formatted_transition_list = []
+    # Create transition's list [src_id, dest_id, [conditions]]
+    for i in xml_transition_list:
+        formatted_transition_list.append([i.source, i.destination, i.condition_list])
+
+    # Create transition's list [src_state_obj, dest_state_obj, [conditions]]
+    for j in formatted_transition_list:
+        result = match_transition_states(j, xml_state_list)
+        if result:
+            objects_conditions_list.append(result)
+
+    return objects_conditions_list
+
+
+def write_state(state_obj_string, state, new, objects_conditions_list):
+    """@ingroup plantuml_adapter
+    Returns simple state string for PlantUml text
+    @param[in, out] state_obj_string TBD
+    @param[in] state TBD
+    @param[in] new TBD
+    @param[in, out] objects_conditions_list TBD
+    @return None
+    """
 
-def get_fun_elem_for_cons_prod_lists(fun_elem, func_obj, cons_or_prod_list):
+    if not state.parent and not state.child_list:
+        state_obj_string.create_state(state)
+        new.append(state.id)
+
+    for j in objects_conditions_list:
+        if all(x in new for x in [j[0].id, j[1].id]):
+            state_obj_string.create_transition([j])
+            objects_conditions_list.remove(j)
+
+
+def write_composed_state(state_obj_string, state, new, objects_conditions_list, output_str='',
+                         count=0):
+    """@ingroup plantuml_adapter
+    Returns composed state string for PlantUml text
+    @param[in, out] state_obj_string TBD
+    @param[in] state TBD
+    @param[in] new TBD
+    @param[in, out] objects_conditions_list TBD
+    @param[in] output_str TBD
+    @param[in] count TBD
+    @return None
     """
-    From cons or prod list [[data_1, function_1_str], [data_2, function_2_str], ...]
-    returns [[data_1, Function(1)], [data_2, Function(2)], ...]
+
+    state_obj_string.create_state(state, parent=True)
+    new.insert(count, state.id)
+    count += 1
+    for i in state.child_list:
+        if not i.child_list:
+            state_obj_string.create_state(i)
+            new.insert(count + 1, i.id)
+        else:
+            write_composed_state(state_obj_string, i, new, objects_conditions_list, output_str,
+                                 count)
+
+    for j in objects_conditions_list:
+        if all(x in new for x in [j[0].id, j[1].id]):
+            state_obj_string.create_transition([j])
+            objects_conditions_list.remove(j)
+
+    state_obj_string.append_string("}\n" * count)
+
+
+def match_transition_states(transition, xml_state_list):
+    """@ingroup plantuml_adapter
+    Return transition with associated state.
+    If not, create default ENTRY or EXIT if one is missing
+    @param[in] transition TBD
+    @param[in] xml_state_list TBD
+    @return transition
     """
-    output = []
-    for cons_or_prod in cons_or_prod_list:
-        if cons_or_prod[1] == func_obj:
-            output.append([cons_or_prod[0], fun_elem])
+    out = None
+    source_state, destination_state = get_source_and_dest(transition, xml_state_list)
 
-    return output
+    if source_state is not None and destination_state is not None:
+        out = [source_state, destination_state, transition[2]]
+    elif source_state is not None and destination_state is None:
+        n = datamodel.State()
+        n.set_name('EXIT')
+        xml_state_list.add(n)
+        out = [source_state, n, transition[2]]
+    elif source_state is None and destination_state is not None:
+        n = datamodel.State()
+        n.set_name('ENTRY')
+        xml_state_list.add(n)
+        out = [n, destination_state, transition[2]]
 
+    return out
 
-def filter_allocated_item_from_view(xml_item_list, xml_view_list):
-    """For a type of item from xml, check if a View is activated and if the item is in its
-    allocated item's list"""
-    if not any(j.activated for j in xml_view_list):
-        return xml_item_list
 
-    filtered_items_list = []
-    activated_view = ''
-    for view in xml_view_list:
-        if view.activated:
-            activated_view = view.name
-            for item in xml_item_list:
-                if item.id in view.allocated_item_list:
-                    filtered_items_list.append(item)
+def get_source_and_dest(transition, xml_state_list):
+    """@ingroup plantuml_adapter
+    Iterate over states id to get source and destination objects
+    @param[in] transition TBD
+    @param[in] xml_state_list TBD
+    @return source and destination objects
+    """
+    source_state = None
+    destination_state = None
 
-    if filtered_items_list:
-        return filtered_items_list
-    if view.allocated_item_list and not filtered_items_list:
-        return xml_item_list
+    for a, b in zip(xml_state_list, xml_state_list):
+        if transition[0] == a.id:
+            source_state = a
+        if transition[1] == b.id:
+            destination_state = b
+        if destination_state and source_state:
+            return source_state, destination_state
 
-    return f"View {activated_view} does not contain any elements"
+    return source_state, destination_state
```

### Comparing `jarvis4se-1.3.4/src/jarvis/functional_orchestrator.py` & `jarvis4se-1.3.5/src/jarvis/orchestrator/functional_orchestrator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """Module with methods relative to Functional section"""
 # Libraries
-import re
 
 # Modules
 import datamodel
 from . import shared_orchestrator
-from .question_answer import get_objects_names, get_children, check_get_object, check_parentality
+from jarvis import question_answer
+from jarvis import util
 from tools import Logger
 
 
 def check_add_predecessor(data_predecessor_str_set, xml_data_list, xml_view_list, output_xml):
     """
     Check if each string in data_predecessor_str_set is corresponding to an actual Data object,
     create new [Data, predecessor] objects lists for object's type : Data.
     Send lists to add_predecessor() to write them within xml and then returns update_list from it.
 
         Parameters:
             data_predecessor_str_set ([str]) : Lists of string from jarvis cell
             xml_data_list ([Data]) : Data list from xml parsing
             xml_view_list ([View]) : View list from xml parsing
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             update ([0/1]) : 1 if update, else 0
     """
     data_predecessor_list = []
 
     allocated_item_list = []
     # Filter input string
-    data_predecessor_str_list = shared_orchestrator.cut_string_list(data_predecessor_str_set)
+    data_predecessor_str_list = util.cut_tuple_list(data_predecessor_str_set)
 
     # Create data names list already in xml
-    xml_data_name_list = get_objects_names(xml_data_list)
+    xml_data_name_list = question_answer.get_objects_names(xml_data_list)
 
     for elem in data_predecessor_str_list:
         is_elem_found = True
         if elem[0] not in xml_data_name_list:
             is_elem_found = False
             if elem[1] not in xml_data_name_list:
                 Logger.set_error(__name__,
-                                f"{elem[0]} and {elem[1]} do not exist")
+                                 f"{elem[0]} and {elem[1]} do not exist")
             else:
                 Logger.set_error(__name__,
-                                f"{elem[0]} does not exist")
+                                 f"{elem[0]} does not exist")
 
         if elem[0] in xml_data_name_list:
             if elem[1] not in xml_data_name_list:
                 is_elem_found = False
                 Logger.set_error(__name__,
-                                f"{elem[1]} does not exist")
+                                 f"{elem[1]} does not exist")
 
         if is_elem_found:
             predecessor = None
             selected_data = None
             existing_predecessor_id_list = []
             for data in xml_data_list:
                 if elem[0] == data.name:
@@ -62,19 +62,21 @@
                     for existing_predecessor in data.predecessor_list:
                         existing_predecessor_id_list.append(existing_predecessor.id)
             for da in xml_data_list:
                 if elem[1] == da.name and da.id not in existing_predecessor_id_list:
                     predecessor = da
             if predecessor is not None and selected_data is not None:
                 data_predecessor_list.append([selected_data, predecessor])
+
             allocation_chain_1 = shared_orchestrator.check_add_allocated_item(elem[0],
                                                                               xml_data_list,
                                                                               xml_view_list)
             if allocation_chain_1:
                 allocated_item_list.append(allocation_chain_1)
+
             allocation_chain_2 = shared_orchestrator.check_add_allocated_item(elem[1],
                                                                               xml_data_list,
                                                                               xml_view_list)
             if allocation_chain_2:
                 allocated_item_list.append(allocation_chain_2)
 
     update = add_predecessor(data_predecessor_list, xml_data_list, output_xml)
@@ -88,32 +90,34 @@
     Check if input lists is not empty, write in xml for each list and return update list if some
     updates has been made
 
         Parameters:
             predecessor_list ([Data, Data(predecessor)]) : Data object to set new predessor and
             predecessor Data
             xml_data_list ([Data]) : Data list from xml parsing
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
     """
 
     if not predecessor_list:
         return 0
 
-    output_xml.write_predecessor(predecessor_list)
-    # Warn the user once added within xml
+    output_xml.write_data_predecessor(predecessor_list)
+
     for data_predecessor in predecessor_list:
         for d in xml_data_list:
             if data_predecessor[0].id == d.id:
                 d.add_predecessor(data_predecessor[1])
-                Logger.set_info(__name__,
-                               f"{data_predecessor[1].name} predecessor for "
-                               f"{data_predecessor[0].name}")
+
+        Logger.set_info(__name__,
+                        f"{data_predecessor[1].name} predecessor for "
+                        f"{data_predecessor[0].name}")
+
     return 1
 
 
 def check_add_consumer_function(consumer_str_list, xml_consumer_function_list,
                                 xml_producer_function_list, xml_function_list, xml_data_list,
                                 output_xml):
     """
@@ -126,203 +130,221 @@
             consumer_str_list ([str]) : Lists of string from jarvis cell
             xml_consumer_function_list ([Data_name_str, Function]) : Data's name and consumer's
             function list from xml
             xml_producer_function_list ([Data_name_str, Function]) : Data's name and producer's
             function list from xml
             xml_function_list ([Function]) : Function list from xml parsing
             xml_data_list ([Data]) : Data list from xml parsing
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
     """
     new_consumer_list = []
     # Create object names/aliases list and data's name
-    xml_function_name_list = get_objects_names(xml_function_list)
-    xml_data_name_list = get_objects_names(xml_data_list)
+    xml_function_name_list = question_answer.get_objects_names(xml_function_list)
+    xml_data_name_list = question_answer.get_objects_names(xml_data_list)
     # Loop to filter consumer and create a new list
     for elem in consumer_str_list:
         is_elem_found = True
         if not any(item == elem[1] for item in xml_function_name_list) and \
                 not any(item == elem[0] for item in xml_data_name_list):
             is_elem_found = False
             Logger.set_error(__name__,
-                            f"{elem[1]} and {elem[0]} do not exist")
+                             f"{elem[1]} and {elem[0]} do not exist")
         elif not any(item == elem[1] for item in xml_function_name_list) or \
                 not any(item == elem[0] for item in xml_data_name_list):
             is_elem_found = False
             if any(item == elem[1] for item in xml_function_name_list) and \
                     not any(item == elem[0] for item in xml_data_name_list):
                 Logger.set_error(__name__,
-                                f"{elem[0]} does not exist")
+                                 f"{elem[0]} does not exist")
             elif any(item == elem[0] for item in xml_data_name_list) and \
                     not any(item == elem[1] for item in xml_function_name_list):
                 Logger.set_error(__name__,
-                                f"{elem[1]} does not exist")
+                                 f"{elem[1]} does not exist")
 
         if is_elem_found:
+            Logger.set_debug(__name__, f"[{elem[0]}, {elem[1]}] check")
             # Loop to filter consumer and create a new list
             for function in xml_function_list:
                 if elem[1] == function.name or elem[1] == function.alias:
                     if [elem[0], function] not in xml_consumer_function_list:
-                        if [elem[0], function] not in xml_producer_function_list:
-                            new_consumer_list.append([elem[0], function])
-                            parent = add_parent_recursively(elem[0], function,
-                                                            xml_consumer_function_list,
-                                                            xml_producer_function_list,
-                                                            new_consumer_list,
-                                                            output_xml, "consumer")
-
-                            if parent is not None:
-                                for par in parent:
-                                    if par:
-                                        new_consumer_list.append(par)
-                        elif [elem[0], function] in xml_producer_function_list:
-                            pass
+                        add_producer_consumer_flow_recursively(elem[0],
+                                                               function,
+                                                               xml_consumer_function_list,
+                                                               xml_producer_function_list,
+                                                               new_consumer_list,
+                                                               output_xml,
+                                                               "consumer")
+                    break
 
+    Logger.set_debug(__name__, f"{consumer_str_list}: {new_consumer_list}")
     update = add_consumer_function(new_consumer_list, xml_consumer_function_list, output_xml)
 
     return update
 
 
 def add_consumer_function(new_consumer_list, xml_consumer_function_list, output_xml):
     """
     Check if input list is not empty, write in xml for each element and return update list if some
     updates has been made
 
         Parameters:
             new_consumer_list ([Data_name_str, Function]) : Data's name and consumer's function list
             xml_consumer_function_list ([Data_name_str, Function]) : Data's name and consumer's
             function list from xml
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
     """
 
     if not new_consumer_list:
         return 0
 
-    output_xml.write_consumer(new_consumer_list)
+    # TODO : new_producer_list to be [data, function] and not [data_name, function]
+    output_xml.write_data_consumer(new_consumer_list)
+
     # Warn the user once added within xml
     for consumer in new_consumer_list:
         xml_consumer_function_list.append(consumer)
         Logger.set_info(__name__,
-                       f"{consumer[1].name} consumes {consumer[0]}")
+                        f"{consumer[1].name} consumes {consumer[0]}")
 
     return 1
 
 
-def add_parent_recursively(flow, function, current_list, opposite_list, new_list, output_xml,
-                           relationship_str, out=False):
+def add_producer_consumer_flow_recursively(flow, function, current_list, opposite_list, new_list, output_xml,
+                                           relationship_str):
     """
-    Recursive method around add_parent_for_data().
+    Recursive method to add producer / consumer function for a flow.
         Parameters:
             flow (Data_name_str) : Data's name
             function (Function) : Current function's parent
             current_list ([Data_name_str, function_name_str]) : 'Current' list (producer/consumer)
             opposite_list ([Data_name_str, function_name_str]) : Opposite list from current
             new_list ([Data_name_str, Function]) : Data's name and consumer/producer's function list
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
             relationship_str (str) : "consumer" or "producer"
             out (bool) : List for recursivity
         Returns:
             elem ([data, Function]) : Return parent
 
     """
-    if not out:
-        out = []
-    parent = add_parent_for_data(flow, function,
-                                 current_list,
-                                 opposite_list,
-                                 new_list,
-                                 output_xml, relationship_str)
-
-    if parent is not None:
-        out.append(parent)
-        return add_parent_recursively(flow, function.parent, current_list, opposite_list, new_list,
-                                      output_xml,
-                                      relationship_str, out)
+    # Prevent function.parent to be added twice
+    if [flow, function] not in new_list and [flow, function] not in current_list:
+        new_list.append([flow, function])
+        Logger.set_debug(__name__, f"[{flow}, {function.name}] added")
+
+        # Check that parent opposite flow is present (if any)
+        is_opposite = False
+        for [opposite_flow, opposite_function] in opposite_list:
+            if opposite_flow == flow:
+                is_opposite = True
+                if opposite_function.parent is not None and opposite_function.parent != function and \
+                        opposite_function.parent != function.parent:
+                    if [opposite_flow, opposite_function.parent] not in opposite_list:
+                        add_producer_consumer_opposite(flow, opposite_function.parent, opposite_list, output_xml,
+                                                       relationship_str)
+
+        if not is_opposite:
+            if relationship_str == "consumer":
+                Logger.set_warning(__name__, f"No producer found for {flow}")
+            elif relationship_str == "producer":
+                Logger.set_warning(__name__, f"No consumer found for {flow}")
+            else:
+                Logger.set_error(__name__, f"Unsupported data relationship type: {relationship_str}")
+
+    if function.parent is not None:
+        parent_child_list, parent_child_dict = question_answer.get_children(function.parent)
 
-    return out
+        if not any([flow, parent_child] in opposite_list for parent_child in parent_child_list):
+            add_producer_consumer_flow_recursively(flow, function.parent, current_list, opposite_list, new_list,
+                                                   output_xml,
+                                                   relationship_str)
+        elif [flow, function.parent] in opposite_list:
+            # Check that no other function needs the flow before removing it
+            ext_function_list = []
+            for [current_flow, current_function] in current_list:
+                if current_flow == flow:
+                    Logger.set_debug(__name__, f"[{current_flow}, {current_function.name}] "
+                                               f"added in external function list")
+                    ext_function_list.append([current_flow, current_function])
+
+            for parent_child in parent_child_list:
+                if [flow, parent_child] in ext_function_list:
+                    ext_function_list.remove([flow, parent_child])
+
+            if len(ext_function_list) == 0:
+                remove_producer_consumer_opposite(flow, function.parent, opposite_list, output_xml, relationship_str)
+            else:
+                Logger.set_debug(__name__, f"[{flow}, {function.parent.name}] still needed")
 
 
-def add_parent_for_data(flow, function, current_list, opposite_list, new_list, output_xml,
-                        relationship_str):
+def add_producer_consumer_opposite(flow, function, flow_function_list, output_xml, relationship_type):
     """
-    Adds direct parent's function of consumer/producer and delete internal flow if the case
+    Add specific consumer/producer relationship within xml's file.
 
         Parameters:
             flow (Data_name_str) : Data's name
-            function (Function) : Current function's parent
-            current_list ([Data_name_str, function_name_str]) : 'Current' list (producer/consumer)
-            opposite_list ([Data_name_str, function_name_str]) : Opposite list from current
-            new_list ([Data_name_str, Function]) : Data's name and consumer/producer's function list
-            output_xml (GenerateXML object) : XML's file object
-            relationship_str (str) : "consumer" or "producer"
+            function (Function) : Current Function object
+            flow_function_list : list of [flow, function]
+            output_xml (XmlWriter3SE object) : XML's file object
+            relationship_type (str) : Type of relationship (i.e. consumer or producer)
         Returns:
-            elem ([data, Function]) : Return parent
+            None
     """
-    elem = [flow, function.parent]
-    temp_set = set()
-    check = False
-
-    if function.parent is not None and elem not in [*current_list, *new_list]:
-        parent_child_list, parent_child_dict = get_children(function.parent)
-
-        current_loop_check = False
-        for current_loop_data in [*current_list, *new_list]:
-            if current_loop_data[0] == flow and current_loop_data[1] not in parent_child_list:
-                current_loop_check = True
-        for data_function in opposite_list:
-            if data_function[0] == flow:
-                temp_set.add(data_function[1])
-        length = len(temp_set)
-        if temp_set == set():
-            check = True
-        else:
-            for fun in temp_set:
-                if fun not in parent_child_list:
-                    check = True
-                    if any(s == [flow, function.parent] for s in opposite_list):
-                        delete_opposite(flow, function.parent, output_xml, relationship_str)
-                if fun in parent_child_list:
-                    length -= 1
-        if length == 0 and not current_loop_check and temp_set != set():
-            delete_opposite(flow, function.parent, output_xml, relationship_str)
-    if check:
-        return elem
+    flow_function_list.append([flow, function])
+
+    if relationship_type == "producer":
+        output_xml.write_data_relationship([flow, function],
+                                           "consumer")
+        Logger.set_info(__name__,
+                        f"{function.name} consumes {flow} due to one of its children")
+    elif relationship_type == "consumer":
+
+        output_xml.write_data_relationship([flow, function],
+                                           "producer")
+        Logger.set_info(__name__,
+                        f"{function.name} produces {flow} due to one of its children")
 
+    if function.parent:
+        add_producer_consumer_opposite(flow, function.parent, flow_function_list, output_xml, relationship_type)
 
-def delete_opposite(data, function, output_xml, relationship_type):
+
+def remove_producer_consumer_opposite(flow, function, flow_function_list, output_xml, relationship_type):
     """
     Delete specific consumer/producer relationship within xml's file.
 
         Parameters:
-            data (Data_name_str) : Data's name
+            flow (Data_name_str) : Data's name
             function (Function) : Current Function object
-            output_xml (GenerateXML object) : XML's file object
+            flow_function_list : list of [flow, function]
+            output_xml (XmlWriter3SE object) : XML's file object
             relationship_type (str) : Type of relationship (i.e. consumer or producer)
         Returns:
             None
     """
+    flow_function_list.remove([flow, function])
 
     if relationship_type == "producer":
-        output_xml.delete_single_consumer_producer(data,
-                                                   function,
-                                                   "consumer")
+        output_xml.delete_data_relationship([flow, function],
+                                            "consumer")
         Logger.set_info(__name__,
-                       f"{function.name} does not consume {data} anymore")
+                        f"{function.name} does not consume {flow} anymore")
     elif relationship_type == "consumer":
 
-        output_xml.delete_single_consumer_producer(data,
-                                                   function,
-                                                   "producer")
+        output_xml.delete_data_relationship([flow, function],
+                                            "producer")
         Logger.set_info(__name__,
-                       f"{function.name} does not produce {data} anymore")
+                        f"{function.name} does not produce {flow} anymore")
+
+    if function.parent and [flow, function.parent] in flow_function_list:
+        remove_producer_consumer_opposite(flow, function.parent, flow_function_list, output_xml, relationship_type)
 
 
 def check_add_producer_function(producer_str_list, xml_consumer_function_list,
                                 xml_producer_function_list, xml_function_list, xml_data_list,
                                 output_xml):
     """
     Check if each string in consumer_str_list are corresponding to an actual object, create new
@@ -333,119 +355,116 @@
             producer_str_list ([str]) : List of string from jarvis cell
             xml_consumer_function_list ([Data_name_str, Function]) : Data's name and consumer's
             function list from xml
             xml_producer_function_list ([Data_name_str, Function]) : Data's name and producer's
             function list from xml
             xml_function_list ([Function]) : Function list from xml parsing
             xml_data_list ([Data]) : Data list from xml parsing
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
     """
     new_producer_list = []
     # Create object names/aliases list
-    xml_function_name_list = get_objects_names(xml_function_list)
-    xml_data_name_list = get_objects_names(xml_data_list)
+    xml_function_name_list = question_answer.get_objects_names(xml_function_list)
+    xml_data_name_list = question_answer.get_objects_names(xml_data_list)
     # Loop to filter producer and create a new list
     for elem in producer_str_list:
         is_elem_found = True
         if not any(item == elem[1] for item in xml_function_name_list) and \
                 not any(item == elem[0] for item in xml_data_name_list):
             is_elem_found = False
             Logger.set_error(__name__,
-                            f"{elem[1]} and {elem[0]} do not exist")
+                             f"{elem[1]} and {elem[0]} do not exist")
         elif not any(item == elem[1] for item in xml_function_name_list) or \
                 not any(item == elem[0] for item in xml_data_name_list):
             is_elem_found = False
             if any(item == elem[1] for item in xml_function_name_list) and \
                     not any(item == elem[0] for item in xml_data_name_list):
                 Logger.set_error(__name__,
-                                f"{elem[0]} does not exist")
+                                 f"{elem[0]} does not exist")
             elif any(item == elem[0] for item in xml_data_name_list) and \
                     not any(item == elem[1] for item in xml_function_name_list):
                 Logger.set_error(__name__,
-                                f"{elem[1]} does not exist")
+                                 f"{elem[1]} does not exist")
 
         if is_elem_found:
+            Logger.set_debug(__name__, f"[{elem[0]}, {elem[1]}] check")
             # Loop to filter consumer and create a new list
             for function in xml_function_list:
                 if elem[1] == function.name or elem[1] == function.alias:
                     if [elem[0], function] not in xml_producer_function_list:
-                        if [elem[0], function] not in xml_consumer_function_list:
-                            new_producer_list.append([elem[0], function])
-                            parent = add_parent_recursively(elem[0], function,
-                                                            xml_producer_function_list,
-                                                            xml_consumer_function_list,
-                                                            new_producer_list, output_xml,
-                                                            "producer")
-                            if parent is not None:
-                                for par in parent:
-                                    if par:
-                                        new_producer_list.append(par)
-
-                        elif [elem[0], function] in xml_consumer_function_list:
-                            pass
+                        add_producer_consumer_flow_recursively(elem[0],
+                                                               function,
+                                                               xml_producer_function_list,
+                                                               xml_consumer_function_list,
+                                                               new_producer_list,
+                                                               output_xml,
+                                                               "producer")
+                    break
 
+    Logger.set_debug(__name__, f"{producer_str_list}: {new_producer_list}")
     update = add_producer_function(new_producer_list, xml_producer_function_list, output_xml)
 
     return update
 
 
 def add_producer_function(new_producer_list, xml_producer_function_list, output_xml):
     """
     Check if input list is not empty, write in xml for each element and return update list if some
     updates has been made
 
         Parameters:
             new_producer_list ([Data_name_str, Function]) : Data's name and producer's function list
             xml_producer_function_list ([Data_name_str, Function]) : Data's name and producer's
             function list from xml
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
     """
     if not new_producer_list:
         return 0
 
-    output_xml.write_producer(new_producer_list)
+    # TODO : new_producer_list to be [data, function] and not [data_name, function]
+    output_xml.write_data_producer(new_producer_list)
     # Warn the user once added within xml
     for producer in new_producer_list:
         xml_producer_function_list.append(producer)
         Logger.set_info(__name__,
-                       f"{producer[1].name} produces {producer[0]}")
+                        f"{producer[1].name} produces {producer[0]}")
     return 1
 
 
 # TODO: Check condition_str on data and (add LogicalType, ArithmeticType in datamodel.py)
 def check_add_transition_condition(trans_condition_str_list, xml_transition_list, output_xml):
     """
     Check if each string in trans_condition_str_list is corresponding to an actual Transition
     object, create new [Transition, condition_str] objects lists for object's type : Transition.
     Send lists to add_transition_condition() to write them within xml and then returns update_list
     from it.
 
         Parameters:
             trans_condition_str_list ([str]) : Lists of string from jarvis cell
             xml_transition_list ([Transition]) : Transition list from xml parsing
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
     """
     condition_list = []
     # Create a list with all transition names/aliases already in the xml
-    xml_transition_name_list = get_objects_names(xml_transition_list)
+    xml_transition_name_list = question_answer.get_objects_names(xml_transition_list)
     for transition_str, condition_str in trans_condition_str_list:
         is_elem_found = True
         if not any(transition_str in s for s in xml_transition_name_list):
             is_elem_found = False
             Logger.set_error(__name__,
-                            f"The transition {transition_str} does not exist")
+                             f"The transition {transition_str} does not exist")
 
         if is_elem_found:
             for transition in xml_transition_list:
                 if transition_str == transition.name or transition_str == transition.alias:
                     if not condition_str.lstrip(' ') in transition.condition_list:
                         condition_list.append([transition, condition_str.lstrip(' ')])
 
@@ -457,95 +476,95 @@
 def add_transition_condition(condition_list, output_xml):
     """
     Check if input list is not empty, write in xml for each list and return update list if some
     updates has been made
 
         Parameters:
             condition_list ([Transition, condition_str]) : Transition object and conditions as str
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
     """
     if not condition_list:
         return 0
 
     output_xml.write_transition_condition(condition_list)
     for elem in condition_list:
         elem[0].add_condition(elem[1])
         Logger.set_info(__name__,
-                       f"Condition for {elem[0].name} : {elem[1]}")
+                        f"Condition for {elem[0].name} : {elem[1]}")
     return 1
 
 
 def check_add_src_dest(src_dest_str, xml_transition_list, xml_state_list, output_xml):
     """
     Check if each string in src_dest_str is corresponding to an actual Transition and State object,
     create new [Transition, State] objects lists.
     Send lists to add_src_dest() to write them within xml and then returns update_list from it.
 
         Parameters:
             src_dest_str ([str]) : Lists of string from jarvis cell
             xml_transition_list ([Transition]) : Transition list from xml parsing
             xml_state_list ([State]) : State list from xml parsing
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
     """
     new_src_list = []
     new_dest_list = []
     # Create lists with all object names/aliases already in the xml
-    xml_transition_name_list = get_objects_names(xml_transition_list)
-    xml_state_name_list = get_objects_names(xml_state_list)
+    xml_transition_name_list = question_answer.get_objects_names(xml_transition_list)
+    xml_state_name_list = question_answer.get_objects_names(xml_state_list)
 
     concatenated_lists = [*xml_transition_name_list, *xml_state_name_list]
 
     # elem = [source/destination, transition_name, state_name]
     for elem in src_dest_str:
         is_elem_found = True
         if not all(t in concatenated_lists for t in [elem[1], elem[2]]):
             is_elem_found = False
             if any(elem[1] in s for s in xml_transition_name_list) and not any(
                     elem[2] in j for j in xml_state_name_list):
                 Logger.set_error(__name__,
-                                f"{elem[2]} state does not exist")
+                                 f"{elem[2]} state does not exist")
             elif any(elem[2] in s for s in xml_state_name_list) and not any(
                     elem[1] in j for j in xml_transition_name_list):
                 Logger.set_error(__name__,
-                                f"{elem[1]} transition does not exist")
+                                 f"{elem[1]} transition does not exist")
             else:
                 Logger.set_error(__name__,
-                                f"{elem[1]} transition and {elem[2]} state do not exist")
+                                 f"{elem[1]} transition and {elem[2]} state do not exist")
 
         if is_elem_found:
             if elem[0] == "source":
                 for transition in xml_transition_list:
                     if elem[1] == transition.name or elem[1] == transition.alias:
                         for state in xml_state_list:
                             if elem[2] == state.name or elem[2] == state.alias:
                                 if not isinstance(state.type, datamodel.BaseType):
-                                    if 'EXIT' in state.type.name: 
+                                    if 'EXIT' in state.type.name:
                                         Logger.set_error(__name__,
-                                                        f"{elem[2]} is typed as EXIT state, "
-                                                        f"it cannot be put as source's transition (not added)")
+                                                         f"{elem[2]} is typed as EXIT state, "
+                                                         f"it cannot be put as source's transition (not added)")
                                 else:
                                     if transition.source != state.id:
                                         new_src_list.append([transition, state])
 
             elif elem[0] == "destination":
                 for transition in xml_transition_list:
                     if elem[1] == transition.name or elem[1] == transition.alias:
                         for state in xml_state_list:
                             if elem[2] == state.name or elem[2] == state.alias:
                                 if not isinstance(state.type, datamodel.BaseType):
                                     if 'ENTRY' in state.type.name:
                                         Logger.set_error(__name__,
-                                                        f"{elem[2]} is typed as ENTRY state, it cannot be "
-                                                        f"put as destination's transition (not added)")
+                                                         f"{elem[2]} is typed as ENTRY state, it cannot be "
+                                                         f"put as destination's transition (not added)")
                                 else:
                                     if transition.destination != state.id:
                                         new_dest_list.append([transition, state])
 
     src_dest_lists = [new_src_list, new_dest_list]
     update = add_src_dest(src_dest_lists, output_xml)
 
@@ -556,37 +575,37 @@
     """
     Check if input lists are not empty, write in xml for each list and return update list if some
     updates has been made
 
         Parameters:
             src_dest_lists ([Transition, State(Source)],[Transition, State(Destination)]) :
             Transition object and Source/Destination
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
     """
     if any(src_dest_lists):
         new_src_list = src_dest_lists[0]
         new_dest_list = src_dest_lists[1]
         if new_src_list:
-            output_xml.write_source(new_src_list)
+            output_xml.write_transition_source(new_src_list)
             # Warn the user once writtent and added within xml
             for source in new_src_list:
                 source[0].set_source(source[1].id)
                 Logger.set_info(__name__,
-                               f"{source[1].name} source for {source[0].name}")
+                                f"{source[1].name} source for {source[0].name}")
 
         if new_dest_list:
-            output_xml.write_destination(new_dest_list)
+            output_xml.write_transition_destination(new_dest_list)
             # Warn the user once writtent and added within xml
             for destination in new_dest_list:
                 destination[0].set_destination(destination[1].id)
                 Logger.set_info(__name__,
-                               f"{destination[1].name} destination for {destination[0].name}")
+                                f"{destination[1].name} destination for {destination[0].name}")
         return 1
 
     return 0
 
 
 def check_add_exposes(exposes_str_list, xml_fun_elem_list, xml_fun_inter_list, xml_data_list,
                       output_xml):
@@ -594,35 +613,37 @@
     Check and get all "Fun_elem exposes Fun_inter" strings, if Fun_inter is not exposed yet
     (or parentality relationship) => add it to Fun_elem object and as exposedInterface within xml.
     Args:
         exposes_str_list ([strings]): list of strings
         xml_fun_elem_list ([Fun Elem]) : Functional Element list from xml parsing
         xml_fun_inter_list ([FunctionalInterface]) : FunctionalInterface list from xml parsing
         xml_data_list ([Data]) : Data list from xml parsing
-        output_xml (GenerateXML object) : XML's file object
+        output_xml (XmlWriter3SE object) : XML's file object
 
     Returns:
         [0/1] : if update has been made
     """
+    # TODO : add physical interface support (see write_element_exposed_interface())
     output = False
-    for exposes_str in exposes_str_list:
-        fun_elem = check_get_object(exposes_str[0], **{'xml_fun_elem_list': xml_fun_elem_list})
-        fun_inter = check_get_object(exposes_str[1], **{'xml_fun_inter_list': xml_fun_inter_list})
+    cleaned_exposes_str_list = util.cut_tuple_list(exposes_str_list)
+    for exposes_str in cleaned_exposes_str_list:
+        fun_elem = question_answer.check_get_object(exposes_str[0], **{'xml_fun_elem_list': xml_fun_elem_list})
+        fun_inter = question_answer.check_get_object(exposes_str[1], **{'xml_fun_inter_list': xml_fun_inter_list})
 
         check_print_wrong_pair_object((exposes_str[0], fun_elem, 'Functional Element'),
                                       (exposes_str[1], fun_inter, 'Functional Interface'),
                                       'exposes')
         if fun_elem and fun_inter:
             check_rule = check_fun_elem_inter_families(fun_elem, fun_inter, xml_fun_elem_list)
             if fun_inter.id not in fun_elem.exposed_interface_list and check_rule:
                 output = True
                 fun_elem.add_exposed_interface(fun_inter.id)
-                output_xml.write_exposed_interface([[fun_elem, fun_inter]])
+                output_xml.write_element_exposed_interface([[fun_elem, fun_inter]])
                 Logger.set_info(__name__,
-                               f"{fun_elem.name} exposes {fun_inter.name}")
+                                f"{fun_elem.name} exposes {fun_inter.name}")
 
     if output:
         return 1
 
     return 0
 
 
@@ -637,24 +658,24 @@
             exposed_fun_elem_list.add(xml_fun_elem)
 
     if not exposed_fun_elem_list:
         return check
 
     opposite_fun_elem_list = []
     for elem in exposed_fun_elem_list:
-        if check_parentality(elem, fun_elem) or \
-                check_parentality(fun_elem, elem):
+        if question_answer.check_parentality(elem, fun_elem) or \
+                question_answer.check_parentality(fun_elem, elem):
             return check
         else:
             opposite_fun_elem_list.append(elem)
 
-    for idx in range(0, len(opposite_fun_elem_list)-1):
-        if not check_parentality(
-                opposite_fun_elem_list[idx], opposite_fun_elem_list[idx+1]) and \
-                not check_parentality(opposite_fun_elem_list[idx+1], opposite_fun_elem_list[idx]):
+    for idx in range(0, len(opposite_fun_elem_list) - 1):
+        if not question_answer.check_parentality(
+                opposite_fun_elem_list[idx], opposite_fun_elem_list[idx + 1]) and \
+                not question_answer.check_parentality(opposite_fun_elem_list[idx + 1], opposite_fun_elem_list[idx]):
             check = False
             return check
 
     return check
 
 
 def check_print_wrong_pair_object(object_a, object_b, relationship_type):
@@ -666,21 +687,21 @@
         e.g. (exposes_str[0], fun_elem, 'Functional Element')
         object_b: (exposes_str[1], fun_inter, 'Functional Interface')
         relationship_type: e.g. 'exposes'
 
     """
     if object_a[1] == object_b[1] is None:
         Logger.set_error(__name__,
-                        f"{object_a[0]} and {object_b[0]} do not exist, choose valid names/aliases for: "
-                        f"'{object_a[2]}' {relationship_type} "
-                        f"'{object_b[2]}'")
+                         f"{object_a[0]} and {object_b[0]} do not exist, choose valid names/aliases for: "
+                         f"'{object_a[2]}' {relationship_type} "
+                         f"'{object_b[2]}'")
     elif object_a[1] is None or object_b[1] is None:
         if object_a[1] is None and object_b[1]:
             Logger.set_error(__name__,
-                            f"{object_a[0]} does not exist, choose a valid name/alias for: "
-                            f"'{object_a[2]}' {relationship_type} "
-                            f"{object_b[1].name}")
+                             f"{object_a[0]} does not exist, choose a valid name/alias for: "
+                             f"'{object_a[2]}' {relationship_type} "
+                             f"{object_b[1].name}")
         elif object_b[1] is None and object_a[1]:
             Logger.set_error(__name__,
-                            f"{object_b[0]} does not exist, choose a valid name/alias for: "
-                            f"{object_a[1].name} {relationship_type} "
-                            f"'{object_b[2]}'")
+                             f"{object_b[0]} does not exist, choose a valid name/alias for: "
+                             f"{object_a[1].name} {relationship_type} "
+                             f"'{object_b[2]}'")
```

### Comparing `jarvis4se-1.3.4/src/jarvis/jarvis.py` & `jarvis4se-1.3.5/src/jarvis/jarvis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""Notebook interface, this module contains ipython Magic class with cell_magic as entry point of
-jarvi4se"""
+"""@defgroup jarvis
+Jarvis module
+"""
 # Libraries
 import re
 import os
 import getpass
 import shutil
 from datetime import datetime
 from io import StringIO
-
 from IPython.core.magic import (Magics, magics_class, cell_magic)
 
 # Modules
-from xml_adapter import GenerateXML, XmlParser3SE
+from xml_adapter import XmlWriter3SE, XmlParser3SE
 from tools import Logger
 
 
 # The class MUST call this class decorator at creation time
 @magics_class
 class MagicJarvis(Magics):
     """Magic iPython class"""
@@ -44,35 +42,29 @@
         # Get model's declaration, need a space after "with" otherwise print a message
         xml_name_str = re.match(r"^with (.*)(?=.|\n)", input_str, re.MULTILINE)
         if xml_name_str:
             xml_name = xml_name_str.group(1)
             # If the model(i.e. file) already exists, parse it to extract lists
             if os.path.isfile(f"{xml_name}.xml"):
                 obj_dict = xml_parser.parse_xml(f"{xml_name}.xml")
-
-                # TODO : why this print ?
-                if isinstance(obj_dict, str):
-                    print(obj_dict)
-                    return
-
                 Logger.set_info(__name__,
                                 f"{xml_name}.xml parsed")
-                output_xml = GenerateXML(f"{xml_name}.xml")
+                output_xml = XmlWriter3SE(f"{xml_name}.xml")
             # Else create an empty xml_lists
             # or will be named by default "Outpout"
             else:
                 if len(xml_name) > 1:
                     Logger.set_info(__name__,
                                     f"Creating {xml_name}.xml !")
 
-                    output_xml = GenerateXML(f"{xml_name}.xml")
+                    output_xml = XmlWriter3SE(f"{xml_name}.xml")
                 else:
                     Logger.set_info(__name__,
                                     "Xml's file does not exists, creating it ('output.xml' by default) !")
-                    output_xml = GenerateXML("")
+                    output_xml = XmlWriter3SE("")
                 output_xml.write()
 
             obj_dict['output_xml'] = output_xml
             update = self.parser.lookup_table(input_str, **obj_dict)
 
             if not update:
                 return
```

### Comparing `jarvis4se-1.3.4/src/jarvis/question_answer.py` & `jarvis4se-1.3.5/src/jarvis/question_answer.py`

 * *Files identical despite different names*

### Comparing `jarvis4se-1.3.4/src/jarvis/shared_orchestrator.py` & `jarvis4se-1.3.5/src/jarvis/orchestrator/shared_orchestrator.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,44 +3,19 @@
 """Module containing methods shared between objects/orchestrator"""
 # Libraries
 import re
 import uuid
 
 # Modules
 import datamodel
-from .question_answer import (get_object_type, check_get_object, get_allocation_object,
-                              check_not_family, get_objects_names, get_children, get_objects_name_lists)
+from jarvis import question_answer
+from jarvis import util
 from tools import Logger
 
 
-def cut_string_list(string_tuple_list):
-    """From set of input command strings e.g for composition with input list as
-    {(Function_name, Function_name_A), (Function_name, [Function_name_B, Function_name_C])} : this
-    methods returns {(Function_name, Function_name_A), (Function_name, Function_name_B),
-    (Function_name, Function_name_C)}
-
-        Parameters:
-            string_tuple_list ([(str, str), ...]) : Lists of string tuple from jarvis cell
-        Returns:
-            output_list ([0/1]) : output list
-    """
-
-    output_list = []
-    for parent, child in string_tuple_list:
-        if "," in child:
-            child_str = child.replace(" ", "")
-            child_list_str = re.split(r',(?![^[]*\])', child_str)
-            for elem in child_list_str:
-                output_list.append((parent, elem))
-        else:
-            output_list.append((parent, child))
-
-    return output_list
-
-
 def check_add_child(parent_child_name_str_list, **kwargs):
     """
     Check if each string in parent_child_name_str_list are corresponding to an actual object,
     create new [parent, child] objects lists for object's type : State/Function/FunctionalElement.
     Send lists to add_child() to write them within xml and then returns update_list from it.
 
         Parameters:
@@ -50,34 +25,34 @@
 
         Returns:
             update ([0/1]) : 1 if update, else 0
     """
 
     parent_child_lists = [[] for _ in range(4)]
     available_objects = (datamodel.Function, datamodel.State,
-                         datamodel.FunctionalElement,  datamodel.PhysicalElement)
+                         datamodel.FunctionalElement, datamodel.PhysicalElement)
 
-    cleaned_parent_child_list_str = cut_string_list(parent_child_name_str_list)
+    cleaned_parent_child_list_str = util.cut_tuple_list(parent_child_name_str_list)
     for elem in cleaned_parent_child_list_str:
-        parent_object = check_get_object(elem[0], **kwargs)
-        child_object = check_get_object(elem[1], **kwargs)
+        parent_object = question_answer.check_get_object(elem[0], **kwargs)
+        child_object = question_answer.check_get_object(elem[1], **kwargs)
         if parent_object is None:
             if child_object is None:
                 Logger.set_error(__name__,
-                                f"{elem[0]} and {elem[1]} are not Function/State/FunctionalElement"
-                                f"/PhysicalElement or the object does not exist")
+                                 f"{elem[0]} and {elem[1]} are not Function/State/FunctionalElement"
+                                 f"/PhysicalElement or the object does not exist")
             else:
                 Logger.set_error(__name__,
-                                f"{elem[0]} is not Function/State/FunctionalElement"
-                                f"/PhysicalElement or the object does not exist")
+                                 f"{elem[0]} is not Function/State/FunctionalElement"
+                                 f"/PhysicalElement or the object does not exist")
             continue
         if child_object is None:
             Logger.set_error(__name__,
-                            f"{elem[1]} is not Function/State/FunctionalElement"
-                            f"/PhysicalElement or the object does not exist")
+                             f"{elem[1]} is not Function/State/FunctionalElement"
+                             f"/PhysicalElement or the object does not exist")
             continue
         check_pair = None
         for idx, obj_type in enumerate(available_objects):
             if isinstance(parent_object, obj_type) and isinstance(child_object, obj_type):
                 check_pair = idx
                 break
         if isinstance(check_pair, int):
@@ -100,26 +75,26 @@
     Check if input lists are not empty, write in xml for each list and return update list if some
     updates has been made
 
         Parameters:
             parent_child_lists ([Parent, Child]) : [[Function],[State],[FunctionalElement],
             [PhysicalElement]]
             xml_fun_elem_list ([FunctionalElement]) : functional element list from xml parsing
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             update_list ([0/1]) : Add 1 to list if any update, otherwise 0 is added
     """
     if any(parent_child_lists):
         for i in range(4):
             if parent_child_lists[i]:
                 output_xml.write_object_child(parent_child_lists[i])
                 for k in parent_child_lists[i]:
                     Logger.set_info(__name__,
-                                   f"{k[0].name} is composed of {k[1].name}")
+                                    f"{k[0].name} is composed of {k[1].name}")
                     if i in (0, 1):
                         for fun_elem in xml_fun_elem_list:
                             if k[0].id in fun_elem.allocated_function_list:
                                 recursive_allocation([fun_elem, k[1]], output_xml)
         return 1
 
     return 0
@@ -173,26 +148,26 @@
 
         Returns:
             update ([0/1]) : 1 if update, else 0
     """
     to_be_deleted_obj_lists = [[] for _ in range(10)]
     # Check if the wanted to delete object exists and can be deleted
     for obj_str in delete_str_list:
-        object_to_del = check_get_object(obj_str, **kwargs)
+        object_to_del = question_answer.check_get_object(obj_str, **kwargs)
         if object_to_del is None:
             Logger.set_error(__name__,
-                            f"{obj_str} does not exist")
+                             f"{obj_str} does not exist")
             continue
 
         check, list_idx = check_relationship_before_delete(object_to_del, **kwargs)
         if check:
             to_be_deleted_obj_lists[list_idx].append(object_to_del)
         else:
             Logger.set_error(__name__,
-                            f"{object_to_del.name} can not be deleted")
+                             f"{object_to_del.name} can not be deleted")
 
     update = delete_objects(to_be_deleted_obj_lists, kwargs['output_xml'])
 
     return update
 
 
 def check_relationship_before_delete(object_to_del, **kwargs):
@@ -293,68 +268,68 @@
         check = True
     return check
 
 
 def check_function(object_to_del, **kwargs):
     """Checks for Function's object"""
     check = False
-    check_list = [False]*6
+    check_list = [False] * 6
     check_list[0] = check_object_no_parent_and_child(object_to_del)
     if not check_list[0]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has composition relationship(s)")
+                        f"{object_to_del.name} has composition relationship(s)")
 
     check_list[1] = check_object_not_allocated(object_to_del, kwargs['xml_state_list'])
     check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_fun_elem_list'])
     if not check_list[1] or not check_list[2]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has allocation relationship(s)")
+                        f"{object_to_del.name} has allocation relationship(s)")
 
     check_list[3] = check_object_not_in_prod_cons(object_to_del,
                                                   kwargs['xml_consumer_function_list'],
                                                   kwargs['xml_producer_function_list'])
     if not check_list[3]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has production/consumption relationship(s)")
+                        f"{object_to_del.name} has production/consumption relationship(s)")
 
     check_list[4] = check_object_no_attribute(object_to_del, kwargs['xml_attribute_list'])
     if not check_list[4]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has attribute(s) set")
+                        f"{object_to_del.name} has attribute(s) set")
 
     check_list[5] = check_object_not_allocated(object_to_del, kwargs['xml_view_list'])
     if not check_list[5]:
         Logger.set_info(__name__, f"{object_to_del.name} has chain relationship(s)")
 
     if all(check_list):
         check = True
         kwargs['xml_function_list'].remove(object_to_del)
     return check
 
 
 def check_data(object_to_del, **kwargs):
     """Checks for Data's object"""
     check = False
-    check_list = [False]*3
+    check_list = [False] * 3
     check_list[0] = check_object_not_in_prod_cons(object_to_del.name,
                                                   kwargs['xml_consumer_function_list'],
                                                   kwargs['xml_producer_function_list'])
     if not check_list[0]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has production/consumption relationship(s)")
+                        f"{object_to_del.name} has production/consumption relationship(s)")
 
     check_list[1] = check_object_not_allocated(object_to_del, kwargs['xml_view_list'])
     if not check_list[1]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has chain relationship(s)")
+                        f"{object_to_del.name} has chain relationship(s)")
 
     check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_fun_inter_list'])
     if not check_list[2]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has allocation relationship(s)")
+                        f"{object_to_del.name} has allocation relationship(s)")
 
     if all(check_list):
         check = True
         kwargs['xml_data_list'].remove(object_to_del)
     return check
 
 
@@ -362,42 +337,42 @@
     """Checks for State's object"""
     check = False
     check_list = [False] * 4
 
     check_list[0] = check_object_no_parent_and_child(object_to_del)
     if not check_list[0]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has composition relationship(s)")
+                        f"{object_to_del.name} has composition relationship(s)")
 
     check_list[1] = not object_to_del.allocated_function_list
     check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_fun_elem_list'])
     if not check_list[1] or not check_list[2]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has allocation relationship(s)")
+                        f"{object_to_del.name} has allocation relationship(s)")
 
     check_list[3] = not any(object_to_del.id in (trans.source, trans.destination)
                             for trans in kwargs['xml_transition_list'])
     if not check_list[3]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has transition relationship(s)")
+                        f"{object_to_del.name} has transition relationship(s)")
     if all(check_list):
         check = True
         kwargs['xml_state_list'].remove(object_to_del)
     return check
 
 
 def check_transition(object_to_del, **kwargs):
     """Checks for State's object"""
     check = False
     check_list = [False] * 1
 
     check_list[0] = object_to_del.source is None and object_to_del.destination is None
     if not check_list[0]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has source/destination relationship(s)")
+                        f"{object_to_del.name} has source/destination relationship(s)")
 
     if all(check_list):
         check = True
         kwargs['xml_transition_list'].remove(object_to_del)
     return check
 
 
@@ -405,27 +380,27 @@
     """Checks for Functional Element's object"""
     check = False
     check_list = [False] * 4
 
     check_list[0] = check_object_no_parent_and_child(object_to_del)
     if not check_list[0]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has composition relationship(s)")
+                        f"{object_to_del.name} has composition relationship(s)")
 
     check_list[1] = (not object_to_del.allocated_function_list and
                      not object_to_del.allocated_state_list)
     check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_phy_elem_list'])
     if not check_list[1] or not check_list[2]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has allocation relationship(s)")
+                        f"{object_to_del.name} has allocation relationship(s)")
 
     check_list[3] = not object_to_del.exposed_interface_list
     if not check_list[3]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has interface relationship(s)")
+                        f"{object_to_del.name} has interface relationship(s)")
 
     if all(check_list):
         check = True
         kwargs['xml_fun_elem_list'].remove(object_to_del)
 
     return check
 
@@ -434,15 +409,15 @@
     """Checks for View's object"""
     check = False
     check_list = [False] * 1
 
     check_list[0] = not object_to_del.allocated_item_list
     if not check_list[0]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has allocation relationship(s)")
+                        f"{object_to_del.name} has allocation relationship(s)")
 
     if all(check_list):
         check = True
         kwargs['xml_view_list'].remove(object_to_del)
 
     return check
 
@@ -451,15 +426,15 @@
     """Checks for Attribute's object"""
     check = False
     check_list = [False] * 1
 
     check_list[0] = not object_to_del.described_item_list
     if not check_list[0]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has attribute relationship(s)")
+                        f"{object_to_del.name} has attribute relationship(s)")
 
     if all(check_list):
         check = True
         kwargs['xml_attribute_list'].remove(object_to_del)
 
     return check
 
@@ -470,15 +445,15 @@
     check_list = [False] * 3
 
     check_list[0] = not object_to_del.allocated_data_list
     check_list[1] = check_object_not_allocated(object_to_del, kwargs['xml_fun_elem_list'])
     check_list[2] = check_object_not_allocated(object_to_del, kwargs['xml_phy_inter_list'])
     if not check_list[0] or not check_list[1] or not check_list[2]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has allocation relationship(s)")
+                        f"{object_to_del.name} has allocation relationship(s)")
 
     if all(check_list):
         check = True
         kwargs['xml_fun_inter_list'].remove(object_to_del)
 
     return check
 
@@ -487,25 +462,25 @@
     """Checks for Physical Element's object"""
     check = False
     check_list = [False] * 3
 
     check_list[0] = check_object_no_parent_and_child(object_to_del)
     if not check_list[0]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has composition relationship(s)")
+                        f"{object_to_del.name} has composition relationship(s)")
 
     check_list[1] = not object_to_del.allocated_fun_elem_list
     if not check_list[1]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has allocation relationship(s)")
+                        f"{object_to_del.name} has allocation relationship(s)")
 
     check_list[2] = not object_to_del.exposed_interface_list
     if not check_list[2]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has interface relationship(s)")
+                        f"{object_to_del.name} has interface relationship(s)")
 
     if all(check_list):
         check = True
         kwargs['xml_phy_elem_list'].remove(object_to_del)
 
     return check
 
@@ -514,20 +489,20 @@
     """Checks for Physical Interface's object"""
     check = False
     check_list = [False] * 2
 
     check_list[0] = not object_to_del.allocated_fun_inter_list
     if not check_list[0]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has allocation relationship(s)")
+                        f"{object_to_del.name} has allocation relationship(s)")
 
     check_list[1] = check_object_not_allocated(object_to_del, kwargs['xml_phy_elem_list'])
     if not check_list[1]:
         Logger.set_info(__name__,
-                       f"{object_to_del.name} has interface relationship(s)")
+                        f"{object_to_del.name} has interface relationship(s)")
 
     if all(check_list):
         check = True
         kwargs['xml_phy_inter_list'].remove(object_to_del)
 
     return check
 
@@ -535,26 +510,26 @@
 def delete_objects(object_lists, output_xml):
     """
     Check if input lists are not empty, write in xml for each list and return update list if some
     updates has been made
 
         Parameters:
             object_lists : see order in get_basetype_and_idx()
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             1 if update, else 0
     """
     if any(object_lists):
         for i in range(10):
             if object_lists[i]:
                 output_xml.delete_object(object_lists[i])
                 for object_type in object_lists[i]:
                     Logger.set_info(__name__,
-                                   f"{object_type.name} deleted")
+                                    f"{object_type.name} deleted")
         return 1
     return 0
 
 
 def check_set_object_type(type_str_list, **kwargs):
     """
     Check if each string in type_str_list are corresponding to an actual object's name/alias, create
@@ -569,18 +544,18 @@
 
         Returns:
             update ([0/1]) : 1 if update, else 0
     """
     object_type_lists = [[] for _ in range(10)]
     # Check if the wanted object exists and the type can be set
     for object_str, type_name in type_str_list:
-        object_to_set = check_get_object(object_str, **kwargs)
+        object_to_set = question_answer.check_get_object(object_str, **kwargs)
         if object_to_set is None:
             Logger.set_error(__name__,
-                           f"{object_str} does not exist")
+                             f"{object_str} does not exist")
             continue
         if object_to_set.type == type_name:
             continue
         check, basetype_idx = check_new_type(object_to_set, type_name, kwargs['xml_type_list'])
         if check:
             object_type_lists[basetype_idx].append(object_to_set)
 
@@ -596,28 +571,28 @@
     obj_base_type = get_basetype_and_idx(object_to_set)
     # print(specific_obj_type_list, list_idx)
     if obj_base_type and type_name != object_to_set.type:
         if type_name.capitalize().replace("_", " ") in [str(i) for i in datamodel.BaseType]:
             basetype_idx = obj_base_type.value
             check = True
             object_to_set.set_type(obj_base_type)
-        elif any(t == type_name for t in get_objects_names(xml_type_list)):
-            obj_type = check_get_object(type_name, **{'xml_type_list': xml_type_list})
+        elif any(t == type_name for t in question_answer.get_objects_names(xml_type_list)):
+            obj_type = question_answer.check_get_object(type_name, **{'xml_type_list': xml_type_list})
             check = check_type_recursively(obj_type)
             if not check:
                 Logger.set_info(__name__,
-                               f"{obj_type.name} is not base type: "
-                               f"{str(obj_base_type)}")
+                                f"{obj_type.name} is not base type: "
+                                f"{str(obj_base_type)}")
             else:
                 basetype_idx = obj_base_type.value
                 object_to_set.set_type(obj_type)
         else:
             Logger.set_error(__name__,
-                            f"The type {type_name} does not exist, available types are "
-                            f": {', '.join([str(i) for i in datamodel.BaseType])}.")
+                             f"The type {type_name} does not exist, available types are "
+                             f": {', '.join([str(i) for i in datamodel.BaseType])}.")
 
     return check, basetype_idx
 
 
 def check_type_recursively(obj_type):
     """Checks type.base recursively if it within specific_obj_type_list"""
     check = False
@@ -629,16 +604,16 @@
     return check
 
 
 def get_basetype_and_idx(object_to_set):
     """Return BaseType according to object's type"""
     # Tuple order is same as datamodel.BaseType(Enum)
     class_obj_tuple = (datamodel.Data, datamodel.Function, datamodel.FunctionalElement,
-    datamodel.FunctionalInterface, datamodel.PhysicalElement, datamodel.PhysicalInterface,
-    datamodel.State, datamodel.Transition, datamodel.Attribute, datamodel.View)
+                       datamodel.FunctionalInterface, datamodel.PhysicalElement, datamodel.PhysicalInterface,
+                       datamodel.State, datamodel.Transition, datamodel.Attribute, datamodel.View)
 
     for idx, i in enumerate(class_obj_tuple):
         if isinstance(object_to_set, i):
             return datamodel.BaseType(idx)
 
     return None
 
@@ -646,30 +621,30 @@
 def set_object_type(object_lists, output_xml):
     """
     Check if input lists are not empty, write in xml for each list and return update list if some
     updates has been made
 
         Parameters:
             object_lists : see order in get_basetype_and_idx()
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             1 if update, else 0
     """
     if any(object_lists):
         for i in range(10):
             if object_lists[i]:
                 output_xml.write_object_type(object_lists[i])
                 for object_type in object_lists[i]:
                     if isinstance(object_type.type, datamodel.BaseType):
                         type_name = str(object_type.type)
                     else:
                         type_name = object_type.type.name
                     Logger.set_info(__name__,
-                                   f"The type of {object_type.name} is {type_name}")
+                                    f"The type of {object_type.name} is {type_name}")
         return 1
     return 0
 
 
 def check_set_object_alias(alias_str_list, **kwargs):
     """
     Check if each string in alias_str_list are corresponding to an actual object's name/alias,
@@ -684,18 +659,18 @@
 
         Returns:
             update ([0/1]) : 1 if update, else 0
     """
     object_lists = [[] for _ in range(9)]
     # Check if the wanted to object exists and the type can be set
     for object_to_set_alias, alias_str in alias_str_list:
-        object_to_set = check_get_object(object_to_set_alias, **kwargs)
+        object_to_set = question_answer.check_get_object(object_to_set_alias, **kwargs)
         if object_to_set is None:
             Logger.set_error(__name__,
-                            f"{object_to_set_alias} does not exist")
+                             f"{object_to_set_alias} does not exist")
             continue
 
         idx = check_new_alias(object_to_set, alias_str)
         if isinstance(idx, int):
             object_lists[idx].append(object_to_set)
 
     update = set_object_alias(object_lists, kwargs['output_xml'])
@@ -716,39 +691,39 @@
     if isinstance(object_to_set, datamodel.Type):
         object_to_set.set_alias(alias_str)
         return 0
 
     base_type = get_base_type_recursively(object_to_set.type)
     if isinstance(base_type, datamodel.BaseType):
         # Data() and View() do not have aliases attributes
-        if base_type.value not in (0,9):
+        if base_type.value not in (0, 9):
             object_to_set.set_alias(alias_str)
             return base_type.value
 
     return check
 
 
 def set_object_alias(object_lists, output_xml):
     """
     Check if input lists are not empty, write in xml for each list and return update if some
     updates has been made.
         Parameters:
             object_lists ([Object]) : object with new alias
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             1 if update, else 0
     """
     if any(object_lists):
         for i in range(9):
             if object_lists[i]:
                 output_xml.write_object_alias(object_lists[i])
                 for object_alias in object_lists[i]:
                     Logger.set_info(__name__,
-                                   f"The alias for {object_alias.name} is {object_alias.alias}")
+                                    f"The alias for {object_alias.name} is {object_alias.alias}")
 
         return 1
 
     return 0
 
 
 def check_add_allocation(allocation_str_list, **kwargs):
@@ -772,28 +747,28 @@
         2: [],  # [FunctionalInterface, Data]
         3: [],  # [PhysicalElement, FunctionalElement]
         4: [],  # [PhysicalInterface, FunctionalInterface]
         # 5: [],  [View, Object] in other modules or [Fun_elem_Parent, Function/State] in
         # check_parent_allocation() it's just a key with no recursivety
     }
     for elem in allocation_str_list:
-        alloc_obj = check_get_object(elem[0],
-                                     **{'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
-                                        'xml_state_list': kwargs['xml_state_list'],
-                                        'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
-                                        'xml_phy_elem_list': kwargs['xml_phy_elem_list'],
-                                        'xml_phy_inter_list': kwargs['xml_phy_inter_list'],
-                                        })
-        obj_to_alloc = check_get_object(elem[1],
-                                        **{'xml_function_list': kwargs['xml_function_list'],
-                                            'xml_state_list': kwargs['xml_state_list'],
-                                           'xml_data_list': kwargs['xml_data_list'],
-                                           'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
-                                           'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
-                                           })
+        alloc_obj = question_answer.check_get_object(elem[0],
+                                                     **{'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
+                                                        'xml_state_list': kwargs['xml_state_list'],
+                                                        'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
+                                                        'xml_phy_elem_list': kwargs['xml_phy_elem_list'],
+                                                        'xml_phy_inter_list': kwargs['xml_phy_inter_list'],
+                                                        })
+        obj_to_alloc = question_answer.check_get_object(elem[1],
+                                                        **{'xml_function_list': kwargs['xml_function_list'],
+                                                           'xml_state_list': kwargs['xml_state_list'],
+                                                           'xml_data_list': kwargs['xml_data_list'],
+                                                           'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
+                                                           'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
+                                                           })
         check_obj = check_allocation_objects_types(alloc_obj, obj_to_alloc, elem)
         if not check_obj:
             continue
         check_rule, alloc = check_allocation_rules(alloc_obj, obj_to_alloc, **kwargs)
         if check_rule and alloc:
             new_allocation[alloc[0]].append(alloc[1])
 
@@ -826,20 +801,20 @@
     if isinstance(obj_str, tuple):
         name_str = f"Objects {obj_str[0]} and {obj_str[1]}"
     else:
         name_str = f"Object {obj_str}"
 
     Logger.set_error(__name__,
                      name_str + " not found or can not be allocated, "
-                               "available allocations are: \n"                     
-                               "(Functional Element allocates State/Function) OR \n"
-                               "(State allocates Function) OR \n"
-                               "(Functional Interface allocates Data) OR \n"
-                               "(Physical Element allocates Functional Element) OR \n"
-                               "(Physical Interface allocates Functional Interface)\n")
+                                "available allocations are: \n"
+                                "(Functional Element allocates State/Function) OR \n"
+                                "(State allocates Function) OR \n"
+                                "(Functional Interface allocates Data) OR \n"
+                                "(Physical Element allocates Functional Element) OR \n"
+                                "(Physical Interface allocates Functional Interface)\n")
 
 
 def check_allocation_rules(alloc_obj, obj_to_alloc, **kwargs):
     """Check "good" combinations, trigger specific check and then return check and new tuple
     allocation"""
     check = False
     new_alloc = None
@@ -881,20 +856,20 @@
     return check, new_alloc
 
 
 def check_fun_elem_allocation(fun_elem, obj_to_alloc, fun_elem_list):
     """Check allocation rules for fun_elem then returns objects if check"""
     count = None
     out = None
-    check_allocation = get_allocation_object(obj_to_alloc, fun_elem_list)
+    check_allocation = question_answer.get_allocation_object(obj_to_alloc, fun_elem_list)
     if check_allocation is not None:
         count = len(check_allocation)
         for item in check_allocation:
             # Checks if they are in the same family
-            if not check_not_family(item, fun_elem) and item != fun_elem:
+            if not question_answer.check_not_family(item, fun_elem) and item != fun_elem:
                 count -= 1
 
     if count in (None, 0):
         if isinstance(obj_to_alloc, datamodel.State):
             fun_elem.add_allocated_state(obj_to_alloc.id)
         else:
             fun_elem.add_allocated_function(obj_to_alloc.id)
@@ -902,59 +877,59 @@
 
     return out
 
 
 def check_state_allocation(state, function, state_list):
     """Check allocation rules for state then returns objects if check"""
     out = None
-    check_allocation = get_allocation_object(function, state_list)
+    check_allocation = question_answer.get_allocation_object(function, state_list)
     if check_allocation is None:
         state.add_allocated_function(function.id)
         out = [state, function]
     else:
         if state not in check_allocation:
             state.add_allocated_function(function.id)
             out = [state, function]
 
     return out
 
 
 def check_fun_inter_allocation(fun_inter, data, **kwargs):
     """Check allocation rules for fun_inter then returns objects if check"""
     out = None
-    check_allocation_fun_inter = get_allocation_object(data, kwargs['xml_fun_inter_list'])
+    check_allocation_fun_inter = question_answer.get_allocation_object(data, kwargs['xml_fun_inter_list'])
     if check_allocation_fun_inter is None:
         check_fe = check_fun_elem_data_consumption(
             data, fun_inter,
             kwargs['xml_fun_elem_list'],
             kwargs['xml_function_list'],
             kwargs['xml_consumer_function_list'],
             kwargs['xml_producer_function_list'])
         if all(i for i in check_fe):
             out = [fun_inter, data]
             fun_inter.add_allocated_data(data.id)
         elif True in check_fe:
             if check_fe[0] is True:
                 Logger.set_error(__name__,
-                               f"Data {data.name} has only consumer(s) "                      
-                               f"allocated to a functional element exposing "
-                               f"{fun_inter.name}, {data.name} not "
-                               f"allocated to {fun_inter.name}")
+                                 f"Data {data.name} has only consumer(s) "
+                                 f"allocated to a functional element exposing "
+                                 f"{fun_inter.name}, {data.name} not "
+                                 f"allocated to {fun_inter.name}")
             elif check_fe[1] is True:
                 Logger.set_error(__name__,
-                               f"Data {data.name} has only producer(s) "                      
-                               f"allocated to a functional element exposing "
-                               f"{fun_inter.name}, {data.name} not "
-                               f"allocated to {fun_inter.name}")
+                                 f"Data {data.name} has only producer(s) "
+                                 f"allocated to a functional element exposing "
+                                 f"{fun_inter.name}, {data.name} not "
+                                 f"allocated to {fun_inter.name}")
         else:
             Logger.set_error(__name__,
-                            f"Data {data.name} has no producer(s) nor "
-                            f"consumer(s) allocated to functional elements "
-                            f"exposing {fun_inter.name}, {data.name} not "
-                            f"allocated to {fun_inter.name}")
+                             f"Data {data.name} has no producer(s) nor "
+                             f"consumer(s) allocated to functional elements "
+                             f"exposing {fun_inter.name}, {data.name} not "
+                             f"allocated to {fun_inter.name}")
 
     return out
 
 
 def check_fun_elem_data_consumption(data, fun_inter, fun_elem_list, function_list,
                                     xml_consumer_function_list, xml_producer_function_list):
     """Check if for a fun_inter, the fun_elem exposing it has allocated functions producing and
@@ -981,28 +956,28 @@
 def add_allocation(allocation_dict, output_xml):
     """
     Check if allocation_lists is not empty, write in xml for each list and return 0/1
     if some update has been made.
 
         Parameters:
             allocation_dict : Containing all allocation to write within xml
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             1 if update, else 0
     """
     if any(allocation_dict.values()):
         for _, k in enumerate(allocation_dict):
             if allocation_dict[k]:
-                output_xml.write_objects_allocation(allocation_dict[k])
+                output_xml.write_object_allocation(allocation_dict[k])
                 # Warn the user once added within xml
                 for elem in allocation_dict[k]:
                     Logger.set_info(__name__,
-                                   f"{elem[1].__class__.__name__} {elem[1].name} is allocated to "
-                                   f"{elem[0].__class__.__name__} {elem[0].name}")
+                                    f"{elem[1].__class__.__name__} {elem[1].name} is allocated to "
+                                    f"{elem[0].__class__.__name__} {elem[0].name}")
                     # Check the dict length, if this method is called from viewpoint_orchestrator
                     # or functional_orchestrator for View => Only key[0] and no recursion wanted
                     if k in (0, 1):
                         recursive_allocation(elem, output_xml)
         return 1
     return 0
 
@@ -1030,22 +1005,22 @@
                 else:
                     fun_elem_parent.add_allocated_function(object_parent.id)
 
                 add_allocation({5: [[fun_elem_parent, object_parent]]}, output_xml)
                 check_parent_allocation([fun_elem_parent, object_parent], output_xml)
             else:
                 Logger.set_error(__name__,
-                                f"{object_parent.name} is not allocated despite at least one "
-                                f"of its child is")
+                                 f"{object_parent.name} is not allocated despite at least one "
+                                 f"of its child is")
 
 
 def recursive_allocation(elem, output_xml):
     """Recursive allocation for childs of State/Function"""
     check_parent_allocation(elem, output_xml)
-    object_type = get_object_type(elem[1])
+    object_type = question_answer.get_object_type(elem[1])
     if elem[1].child_list:
         for i in elem[1].child_list:
             parent_child = [elem[1], i]
             allocated_child_list = get_allocated_child(parent_child, [elem[0]])
             if allocated_child_list:
                 for item in allocated_child_list:
                     if isinstance(elem[1], datamodel.State):
@@ -1055,21 +1030,21 @@
                 # We want recursivety so it trigger for (0, 1) keys in the dict
                 add_allocation({0: allocated_child_list}, output_xml)
     else:
         # TBT/TBC
         if object_type == "state" and elem[1].id not in elem[0].allocated_state_list:
             elem[0].add_allocated_state(elem[1].id)
             Logger.set_info(__name__,
-                           f"State {elem[1].name} is allocated to functional "
-                           f"element {elem[0].name}")
+                            f"State {elem[1].name} is allocated to functional "
+                            f"element {elem[0].name}")
         elif object_type == "function" and elem[1].id not in elem[0].allocated_function_list:
             elem[0].add_allocated_function(elem[1].id)
             Logger.set_info(__name__,
-                           f"Function {elem[1].name} is allocated to functional "
-                           f"element {elem[0].name}")
+                            f"Function {elem[1].name} is allocated to functional "
+                            f"element {elem[0].name}")
 
 
 def get_allocated_child(elem, xml_fun_elem_list):
     """
     Check if the parent state/function is already allocated to a fun elem and create list to add
     its child also (if not already allocated)
 
@@ -1113,40 +1088,40 @@
 
         Returns:
             update ([0/1]) : 1 if update, else 0
     """
     new_list = []
     for elem in inherit_str_list:
         # elem_0: inheriting object
-        elem_0 = check_get_object(elem[0],
-                                  **{'xml_function_list': kwargs['xml_function_list'],
-                                     'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
-                                     'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
-                                     'xml_phy_elem_list': kwargs['xml_phy_elem_list'],
-                                     'xml_phy_inter_list': kwargs['xml_phy_inter_list'],
-                                     })
+        elem_0 = question_answer.check_get_object(elem[0],
+                                                  **{'xml_function_list': kwargs['xml_function_list'],
+                                                     'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
+                                                     'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
+                                                     'xml_phy_elem_list': kwargs['xml_phy_elem_list'],
+                                                     'xml_phy_inter_list': kwargs['xml_phy_inter_list'],
+                                                     })
         # elem_1: object to inherit from
-        elem_1 = check_get_object(elem[1],
-                                  **{'xml_function_list': kwargs['xml_function_list'],
-                                     'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
-                                     'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
-                                     'xml_phy_elem_list': kwargs['xml_phy_elem_list'],
-                                     'xml_phy_inter_list': kwargs['xml_phy_inter_list'],
-                                     })
+        elem_1 = question_answer.check_get_object(elem[1],
+                                                  **{'xml_function_list': kwargs['xml_function_list'],
+                                                     'xml_fun_elem_list': kwargs['xml_fun_elem_list'],
+                                                     'xml_fun_inter_list': kwargs['xml_fun_inter_list'],
+                                                     'xml_phy_elem_list': kwargs['xml_phy_elem_list'],
+                                                     'xml_phy_inter_list': kwargs['xml_phy_inter_list'],
+                                                     })
         if not elem_0 or not elem_1:
             if not elem_0 and not elem_1:
                 print_wrong_object_inheritance(elem[0], elem[1])
             elif not elem_0:
                 print_wrong_object_inheritance(elem[0])
             else:
                 print_wrong_object_inheritance(elem[1])
             continue
         if elem_0 == elem_1:
             Logger.set_warning(__name__,
-                              f"Same object {elem_0.name}")
+                               f"Same object {elem_0.name}")
             continue
         if elem_0.derived == elem_1:
             continue
 
         check_obj = check_inheritance(elem_0, elem_1)
         if not check_obj:
             continue
@@ -1163,20 +1138,20 @@
     """Prints wrong object(s) message for inheritance from input string"""
     if len(obj) == 2:
         user_message = f"{obj[0]} and {obj[1]}"
     else:
         user_message = f"{obj[0]}"
 
     Logger.set_error(__name__,
-                    f"{user_message} not found, available objects for inheritance are:\n"
-                    "- Function\n"
-                    "- Functional element\n"
-                    "- Functional interface\n"
-                    "- Physical element\n"
-                    "- Physical element\n")
+                     f"{user_message} not found, available objects for inheritance are:\n"
+                     "- Function\n"
+                     "- Functional element\n"
+                     "- Functional interface\n"
+                     "- Physical element\n"
+                     "- Physical element\n")
 
 
 def check_inheritance(elem_0, elem_1):
     """Returns check if pair are compatible and object list have been updated"""
     inheritance_type_list = [datamodel.Function, datamodel.FunctionalElement,
                              datamodel.FunctionalInterface, datamodel.PhysicalElement,
                              datamodel.PhysicalInterface]
@@ -1185,45 +1160,48 @@
     for idx, inheritance_type in enumerate(inheritance_type_list):
         if isinstance(elem_0, inheritance_type) and isinstance(elem_1, inheritance_type):
             type_found = idx
             break
 
     if type_found is None:
         Logger.set_error(__name__,
-                        f"{elem_0.__class__.__name__} and {elem_1.__class__.__name__} "
-                        f"are not of the same type")
+                         f"{elem_0.__class__.__name__} and {elem_1.__class__.__name__} "
+                         f"are not of the same type")
         return False
 
     elem_0.set_derived(elem_1)
     return True
 
 
 def add_derived(object_list, output_xml):
     """
     Check if input lists are not empty, write in xml for each list and return update if some
     updates has been made.
         Parameters:
             object_list ([Object]) : object with new derived
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             1 if update, else 0
     """
     if any(object_list):
-        output_xml.write_derived(object_list)
+        output_xml.write_object_derived(object_list)
         for obj in object_list:
             Logger.set_info(__name__,
-                           f"{obj.name} inherited from {obj.derived.name}")
+                            f"{obj.name} inherited from {obj.derived.name}")
         return 1
     return 0
 
+
 class CreateObjInstance:
     def __init__(self, obj_str, base_type, specific_obj_type=None, **kwargs):
         self.specific_obj_type = specific_obj_type
         self.base_type = base_type
+        self.base_type_idx = datamodel.BaseType.get_enum(
+            str(self.base_type)).value
         self.new_obj = self.create_obj(obj_str)
         # Data() and View() do not have aliases
         if not isinstance(self.new_obj, (datamodel.Data, datamodel.View)):
             self.create_alias(obj_str)
         self.add_obj_to_xml_set(**kwargs)
 
     def create_obj(self, obj_str):
@@ -1264,16 +1242,16 @@
         return call(self.new_obj)
 
     def return_obj(self):
         return self.new_obj, self.base_type_idx
 
 
 xml_str_lists = ['xml_function_list', 'xml_data_list', 'xml_state_list', 'xml_fun_elem_list',
-                    'xml_transition_list', 'xml_fun_inter_list', 'xml_phy_elem_list',
-                    'xml_phy_inter_list', 'xml_attribute_list', 'xml_view_list', 'xml_type_list']
+                 'xml_transition_list', 'xml_fun_inter_list', 'xml_phy_elem_list',
+                 'xml_phy_inter_list', 'xml_attribute_list', 'xml_view_list', 'xml_type_list']
 
 
 def check_add_specific_obj_by_type(obj_type_str_list, **kwargs):
     """
     Check if each string in obj_type_str_list are corresponding to an actual object's name/alias,
     set_derive, create object_lists with list per obj. Send lists to add_obj_to_xml()
     write them within xml and then returns update from it.
@@ -1289,27 +1267,27 @@
     for elem in obj_type_str_list:
         spec_obj_type = None
         base_type = None
         if elem[1].capitalize() in [str(i) for i in datamodel.BaseType]:
             base_type = next((i for i in [str(i) for i in datamodel.BaseType]
                               if i == elem[1].capitalize()))
         else:
-            spec_obj_type = check_get_object(elem[1],
-                                             **{'xml_type_list': kwargs['xml_type_list']})
+            spec_obj_type = question_answer.check_get_object(elem[1],
+                                                             **{'xml_type_list': kwargs['xml_type_list']})
             if not spec_obj_type:
                 Logger.set_error(__name__,
-                                f"No valid type found for {elem[1]}")
+                                 f"No valid type found for {elem[1]}")
                 continue
             base_type = get_base_type_recursively(spec_obj_type)
         if base_type is None:
             Logger.set_error(__name__,
-                            f"No valid base type found for {elem[1]}")
+                             f"No valid base type found for {elem[1]}")
             continue
 
-        xml_names_list = get_objects_name_lists(
+        xml_names_list = question_answer.get_objects_name_lists(
             **{key: value for (key, value) in kwargs.items() if key in xml_str_lists})
         flat_names_list = [item for sublist in xml_names_list for item in sublist]
         if any(n == elem[0] for n in flat_names_list):
             # Maybe we can warn user
             continue
         new_obj, base_type_idx = CreateObjInstance(
             elem[0],
@@ -1319,15 +1297,15 @@
         ).return_obj()
         if isinstance(new_obj.type, datamodel.BaseType):
             type_name = str(new_obj.type)
         else:
             type_name = new_obj.type.name
 
         Logger.set_info(__name__,
-                       f"{new_obj.name} is a {type_name}")
+                        f"{new_obj.name} is a {type_name}")
 
         object_lists[base_type_idx].append(new_obj)
 
     if any(object_lists):
         return add_obj_to_xml(object_lists, kwargs['output_xml'])
     return 0
 
@@ -1344,15 +1322,15 @@
 def get_unique_id():
     """Generate and set unique identifier of length 10 integers"""
     identifier = uuid.uuid4()
     return str(identifier.int)[:10]
 
 
 def add_obj_to_xml(object_lists, output_xml):
-    """Send lists object to respective methods of GenerateXML, returns 1 if at least one obj has
+    """Send lists object to respective methods of XmlWriter3SE, returns 1 if at least one obj has
     been written"""
     switch_write_obj = {
         0: output_xml.write_data,
         1: output_xml.write_function,
         2: output_xml.write_functional_element,
         3: output_xml.write_functional_interface,
         4: output_xml.write_physical_element,
@@ -1399,15 +1377,15 @@
 
     [obj.add_child(c) for c in obj.derived.child_list
      if c.parent == obj.derived]
     [c.set_parent(obj) for c in obj.derived.child_list
      if c.parent == obj.derived]
     for child in obj.derived.child_list:
         derived_parent_dict[str(child.id)] = str(obj.id)
-    derived_child_set = get_children(obj.derived, level=level)[0]
+    derived_child_set = question_answer.get_children(obj.derived, level=level)[0]
     derived_child_id_list = {c.id for c in obj.derived.child_list}
     obj.derived.child_list.clear()
     derived_child_set.remove(obj.derived)
 
     return derived_child_set, derived_parent_dict, derived_child_id_list
 
 
@@ -1478,28 +1456,28 @@
 def allocation_inheritance(xml_obj_set, xml_allocated_obj_set):
     """Allocation Inheritance"""
     alloc_to_reset = []
     for elem in xml_obj_set:
         if elem.derived:
             if isinstance(elem, datamodel.FunctionalElement):
                 pair = [elem, {i for i in elem.derived.allocated_function_list
-                                  if i not in elem.allocated_function_list}]
+                               if i not in elem.allocated_function_list}]
                 elem.allocated_function_list = elem.allocated_function_list.union(
                     elem.derived.allocated_function_list)
                 alloc_to_reset.append(pair)
             if isinstance(elem, datamodel.FunctionalInterface):
                 pair = [elem, {i for i in elem.derived.allocated_data_list
-                                  if i not in elem.allocated_data_list}]
+                               if i not in elem.allocated_data_list}]
                 elem.allocated_data_list = elem.allocated_data_list.union(
                     elem.derived.allocated_data_list)
                 alloc_to_reset.append(pair)
 
     return alloc_to_reset
 
 
 def reset_alloc_inheritance(pairs_to_reset):
     """Reset Allocation Inheritance"""
     for pair in pairs_to_reset:
         if isinstance(pair[0], datamodel.FunctionalElement):
             [pair[0].allocated_function_list.remove(fun_id) for fun_id in pair[1]]
         if isinstance(pair[0], datamodel.FunctionalInterface):
-            [pair[0].allocated_data_list.remove(data_id) for data_id in pair[1]]
+            [pair[0].allocated_data_list.remove(data_id) for data_id in pair[1]]
```

### Comparing `jarvis4se-1.3.4/src/jarvis/viewpoint_orchestrator.py` & `jarvis4se-1.3.5/src/jarvis/orchestrator/viewpoint_orchestrator.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 """Module with methods relative to Viewpoint section"""
 # Libraries
 import re
 
 # Modules
 import datamodel
 from . import shared_orchestrator
-from .question_answer import get_objects_names, check_get_object
+from jarvis import question_answer
 from tools import Logger
 
 
 def add_view(view_name_str, xml_view_list, output_xml):
     """
         Check if each string in view_name_str is not already corresponding to an actual
         object's name, create new View() object, instantiate it, write it within XML and
         then returns update_list.
 
             Parameters:
                 view_name_str ([str]) : Lists of string from jarvis cell
                 xml_view_list ([Function]) : view list from xml parsing
-                output_xml (GenerateXML object) : XML's file object
+                output_xml (XmlWriter3SE object) : XML's file object
 
             Returns:
                 1 if update, else 0
         """
     view_list = []
     # Create a list with all view names already in the xml
-    xml_view_name_list = get_objects_names(xml_view_list)
+    xml_view_name_list = question_answer.get_objects_names(xml_view_list)
     # Loop on the list and create set for functions
     if view_name_str not in xml_view_name_list:
         # Instantiate view class
         view = datamodel.View(name=view_name_str, uid=shared_orchestrator.get_unique_id())
         # Add view to new set() and existing et() from xml
         xml_view_list.add(view)
         view_list.append(view)
@@ -66,24 +66,24 @@
     the current view => add it to View object and as allocatedItem within xml
     Args:
         consider_str_list ([strings]): list of strings (separated by comma is possible)
         xml_function_list ([Function]) : Function list from xml parsing
         xml_fun_elem_list ([Fun Elem]) : Functional Element list from xml parsing
         xml_data_list ([Data]) : Data list from xml parsing
         xml_view_list ([View]) : View list from xml parsing
-        output_xml (GenerateXML object) : XML's file object
+        output_xml (XmlWriter3SE object) : XML's file object
 
     Returns:
         update ([0/1]) : 1 if update, else 0
     """
     allocated_item_list = []
     # Create lists with all object names/aliases already in the xml
-    xml_fun_elem_name_list = get_objects_names(xml_fun_elem_list)
-    xml_function_name_list = get_objects_names(xml_function_list)
-    xml_data_name_list = get_objects_names(xml_data_list)
+    xml_fun_elem_name_list = question_answer.get_objects_names(xml_fun_elem_list)
+    xml_function_name_list = question_answer.get_objects_names(xml_function_list)
+    xml_data_name_list = question_answer.get_objects_names(xml_data_list)
 
     consider_str_list = split_chain_from_string(consider_str_list)
 
     for consider_str in consider_str_list:
         if consider_str not in [*xml_fun_elem_name_list, *xml_function_name_list,
                                 *xml_data_name_list]:
             Logger.set_warning(__name__,
@@ -133,22 +133,22 @@
     Check if each string in xml_attribute_list is not already corresponding to an actual object's
     name/alias, create new Attribute() object, instantiate it, write it within XML and then returns
     update_list.
 
         Parameters:
             attribute_str_list ([str]) : Lists of string from jarvis cell
             xml_attribute_list ([Attribute]) : Attribute list from xml parsing
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             1 if update, else 0
     """
     new_attribute_list = []
     # Create attribute names list already in xml
-    xml_attribute_name_list = get_objects_names(xml_attribute_list)
+    xml_attribute_name_list = question_answer.get_objects_names(xml_attribute_list)
     # Filter attribute_list, keeping only the the ones not already in the xml
     for attribute_name in attribute_str_list:
         if attribute_name not in xml_attribute_name_list:
             new_attribute = datamodel.Attribute()
             new_attribute.set_name(str(attribute_name))
             # Generate and set unique identifier of length 10 integers
             new_attribute.set_id(shared_orchestrator.get_unique_id())
@@ -178,23 +178,23 @@
             xml_attribute_list ([Attribute]) : Attribute's list from xml
 
         Returns:
             update ([0/1]) : 1 if update, else 0
     """
     new_described_attribute_list = []
     for elem in described_attribute_list:
-        obj_to_set = check_get_object(
+        obj_to_set = question_answer.check_get_object(
             elem[1], 
             **{'xml_function_list': xml_dict_sets['xml_function_list'],
             'xml_fun_elem_list': xml_dict_sets['xml_fun_elem_list'],
             'xml_fun_inter_list': xml_dict_sets['xml_fun_inter_list'],
             'xml_phy_elem_list': xml_dict_sets['xml_phy_elem_list'],
             'xml_phy_inter_list': xml_dict_sets['xml_phy_inter_list'],
             })
-        attribute_wanted = check_get_object(
+        attribute_wanted = question_answer.check_get_object(
             elem[0], 
             **{'xml_attribute_list': xml_dict_sets['xml_attribute_list'],
             })
         if obj_to_set is None and attribute_wanted is None:
             print(f"{elem[0]:s} do not exist and {elem[1]:s} neither or {elem[1]:s} is not a:\n"
             "- Function\n"
             "- Functional element\n"
@@ -219,23 +219,23 @@
 def add_object_attribute(new_obj_attribute_list, output_xml):
     """
     Check if input list is not empty, write in xml for each element and return update list if some
     updates has been made
 
         Parameters:
             new_obj_attribute_list ([Attribute, (Object, value)]) : New described attributes
-            output_xml (GenerateXML object) : XML's file object
+            output_xml (XmlWriter3SE object) : XML's file object
 
         Returns:
             1 if update, else 0
     """
     if not new_obj_attribute_list:
         return 0
 
-    output_xml.write_described_attribute_item(new_obj_attribute_list)
+    output_xml.write_attribute_described_item(new_obj_attribute_list)
     # Warn the user once added within xml
     for described_attribute in new_obj_attribute_list:
         described_attribute[0].add_described_item(described_attribute[1])
         Logger.set_info(__name__,
                        f"Attribute {described_attribute[0].name} for {described_attribute[1][0].name} "
                        f"with value {described_attribute[1][1]}")
     return 1
@@ -253,15 +253,15 @@
 
         Returns:
             update ([0/1]) : 1 if update, else 0
     """
     new_type_list = []
     # Capitalyze the reference type for datamodel matching
     for elem in extends_str_list:
-        if any(t == elem[0] for t in get_objects_names(xml_type_list)):
+        if any(t == elem[0] for t in question_answer.get_objects_names(xml_type_list)):
             # print(f"{elem[0]} already exists")
             continue
         type_to_extend = check_get_type_to_extend(elem[1], xml_type_list)
         if not type_to_extend:
             Logger.set_error(__name__,
                             f"Unable to find referenced type '{elem[1]}'")
             continue
@@ -295,12 +295,12 @@
     """Checks if type_str is within BaseType or xml_type_list, then return Basetype or
     type object"""
     check = None
     formated_type_str = type_str.upper().replace(" ", "_")
     if any(a == formated_type_str for a in [i.name for i in datamodel.BaseType]):
         return datamodel.BaseType[formated_type_str]
 
-    if any(a == type_str for a in get_objects_names(xml_type_list)):
-        check = check_get_object(type_str, **{'xml_type_list': xml_type_list})
+    if any(a == type_str for a in question_answer.get_objects_names(xml_type_list)):
+        check = question_answer.check_get_object(type_str, **{'xml_type_list': xml_type_list})
         return check
 
     return check
```

### Comparing `jarvis4se-1.3.4/src/jarvis4se.egg-info/PKG-INFO` & `jarvis4se-1.3.5/src/jarvis4se.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis4se
-Version: 1.3.4
+Version: 1.3.5
 Summary: Jarvis 4 Systems Engineers
 Home-page: https://github.com/rcasteran/jarvis4se
 Author: Justin ANCELOT
 Author-email: not2behere@gmx.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rcasteran/jarvis4se/issues
 Project-URL: Gitbook, https://regis-casteran.gitbook.io/jarvis4se/
```

### Comparing `jarvis4se-1.3.4/src/plantuml_adapter/__init__.py` & `jarvis4se-1.3.5/src/plantuml_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `jarvis4se-1.3.4/src/plantuml_adapter/util.py` & `jarvis4se-1.3.5/src/plantuml_adapter/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""@defgroup plantuml_adapter
+Plantuml adapter module
+"""
 # Libraries
 import os
 import re
 import inspect
 import pathlib
 import subprocess
```

### Comparing `jarvis4se-1.3.4/src/tools/__init__.py` & `jarvis4se-1.3.5/src/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `jarvis4se-1.3.4/src/tools/config.py` & `jarvis4se-1.3.5/src/tools/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""@defgroup tools
+Tooling module
+"""
+
 # Libraries
 import os
 
 
 # Modules
 
 
@@ -9,14 +13,15 @@
     """@ingroup tools
     @anchor Config
     Jarvis configurator
     """
 
     is_log_file = False
     is_diagram_file = False
+    verbose_level = 1
 
     @classmethod
     def read(cls):
         """ Read the configuration file if any
         @return None
         """
         try:
@@ -34,14 +39,26 @@
                                     # Logger depends from Config. Thus simple print
                                     print("Log file storage activated")
                             elif lines[0].strip() == 'diagram':
                                 if 'True' == lines[1].strip() or '1' == lines[1].strip():
                                     cls.is_diagram_file = True
                                     # Logger depends from Config. Thus simple print
                                     print("Diagram file storage activated")
+                            elif lines[0].strip() == 'verbose':
+                                if lines[1].strip().isnumeric():
+                                    cls.verbose_level = int(lines[1].strip())
+                                    # Logger depends from Config. Thus simple print
+                                    if cls.verbose_level == 0:
+                                        print(f"ERROR and WARNING messages display activated")
+                                    elif cls.verbose_level == 1:
+                                        print(f"ERROR, WARNING and INFO messages display activated")
+                                    else:
+                                        print(f"ERROR, WARNING, INFO and DEBUG messages display activated")
+                                else:
+                                    error = True
                             else:
                                 error = True
                         else:
                             error = True
                         line = file_reader.readline()
 
                     if error:
```

### Comparing `jarvis4se-1.3.4/src/tools/console.py` & `jarvis4se-1.3.5/src/tools/console.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Libraries
 import re
 import os
 
 # Modules
 from jarvis.command_parser import CmdParser
 from plantuml_adapter import PlantUmlGen
-from xml_adapter import GenerateXML, XmlParser3SE
+from xml_adapter import XmlWriter3SE, XmlParser3SE
 
 
 def main():
     """@ingroup tools
     @anchor main
     Jarvis console
     @return None
@@ -45,28 +45,25 @@
             # Get model's declaration, need a space after "with" otherwise print a message
             xml_name_str = re.match(r"^with (.*)(?=.|\n)", input_str, re.MULTILINE)
             if xml_name_str:
                 xml_name = xml_name_str.group(1)
                 # If the model(i.e. file) already exists, parse it to extract lists
                 if os.path.isfile(f"{xml_name}.xml"):
                     obj_dict = xml_parser.parse_xml(f"{xml_name}.xml")
-                    if isinstance(obj_dict, str):
-                        print(obj_dict)
-                        return
                     print(f"{xml_name}.xml parsed")
-                    output_xml = GenerateXML(f"{xml_name}.xml")
+                    output_xml = XmlWriter3SE(f"{xml_name}.xml")
                 # Else create an empty xml_lists
                 # or will be named by default "Output"
                 else:
                     if len(xml_name) > 1:
                         print(f"Creating {xml_name}.xml !")
-                        output_xml = GenerateXML(f"{xml_name}.xml")
+                        output_xml = XmlWriter3SE(f"{xml_name}.xml")
                     else:
                         print("Xml's file does not exists, creating it('output.xml' by default) !")
-                        output_xml = GenerateXML("")
+                        output_xml = XmlWriter3SE("")
                     output_xml.write()
 
                 obj_dict['output_xml'] = output_xml
             elif len(xml_name) > 0:
                 update = parser.lookup_table(input_str, **obj_dict)
 
                 if 1 in update:
```

### Comparing `jarvis4se-1.3.4/src/tools/logger.py` & `jarvis4se-1.3.5/src/tools/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""@defgroup tools
+Tooling module
+"""
+
 # Libraries
 from datetime import datetime
 import os
 
 
 # Modules
 from . import Config
@@ -12,47 +16,57 @@
     @anchor Logger
     Jarvis logger
     """
 
     @classmethod
     def set_debug(cls, module_name, msg):
         """Format DEBUG message
+
+        DEBUG message are displayed with verbosity level greater than or equal to 2
         @param[in] module_name module name responsible for the message
         @param[in] msg message to be formatted
         @return None
         """
-        print("[DEBUG] " + msg)
-        if Config.is_log_file:
-            cls.write("DEBUG", module_name, msg)
+        if Config.verbose_level >= 2:
+            print("[DEBUG] " + msg)
+            if Config.is_log_file:
+                cls.write("DEBUG", module_name, msg)
 
     @classmethod
     def set_info(cls, module_name, msg):
         """Format INFO message
+
+        INFO message are displayed with verbosity level greater than 1
         @param[in] module_name module name responsible for the message
         @param[in] msg message to be formatted
         @return None
         """
-        print(msg)
-        if Config.is_log_file:
-            cls.write("INFO", module_name, msg)
+        if Config.verbose_level >= 1:
+            print(msg)
+            if Config.is_log_file:
+                cls.write("INFO", module_name, msg)
 
     @classmethod
     def set_warning(cls, module_name, msg):
         """Format WARNING message
+
+        WARNING message are always displayed (no verbosity level consideration)
         @param[in] module_name module name responsible for the message
         @param[in] msg message to be formatted
         @return None
         """
         print("[WARNING] " + msg)
         if Config.is_log_file:
             cls.write("WARNING", module_name, msg)
 
     @classmethod
     def set_error(cls, module_name, msg):
         """Format ERROR message
+
+        ERROR message are always displayed (no verbosity level consideration)
         @param[in] module_name module name responsible for the message
         @param[in] msg message to be formatted
         @return None
         """
         print("[ERROR] " + msg)
         if Config.is_log_file:
             cls.write("ERROR", module_name, msg)
```

### Comparing `jarvis4se-1.3.4/src/tools/magic_tools.py` & `jarvis4se-1.3.5/src/tools/magic_tools.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""@defgroup tools
+Tooling module
+"""
+
 # Libraries
 from sys import version as py_ver
 from importlib.metadata import version
 from IPython.core.magic import (Magics, magics_class, cell_magic, line_magic)
 from IPython.display import display, HTML, Markdown
 
 # Modules
```

### Comparing `jarvis4se-1.3.4/src/xml_adapter/xml_parser.py` & `jarvis4se-1.3.5/src/xml_adapter/xml_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,32 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""Module for xml parsing"""
+"""@defgroup xml_adapter
+Module for 3SE xml parsing and writing
+"""
 # Libraries
 from lxml import etree
 
 # Modules
 import datamodel
+from tools import Logger
 
 
 class XmlParser3SE:
-    """Class for xml parsing"""
+    """@ingroup xml_adapter
+    @anchor XmlParser3SE
+    3SE XML parser
+    """
+
     def __init__(self):
+        """ @var xml_dict
+        XML dictionary
+
+        @var root
+        Reference to the XML root object
+        """
+
         self.xml_dict = {'xml_function_list': set(),
                          'xml_consumer_function_list': [],
                          'xml_producer_function_list': [],
                          'xml_data_list': set(),
                          'xml_state_list': set(),
                          'xml_transition_list': set(),
                          'xml_fun_elem_list': set(),
@@ -23,426 +35,505 @@
                          'xml_fun_inter_list': set(),
                          'xml_phy_elem_list': set(),
                          'xml_phy_inter_list': set(),
                          'xml_type_list': set()}
         self.root = None
 
     def parse_xml(self, input_filename):
-        """Parses the whole xml then returns lists of objects/relationship"""
+        """Parse the XML file and returns the XML dictionary
+        @param[in] input_filename : XML file name
+        @return XML dictionary
+        """
         # To speed up parsing (see lxml doc) : TBC if can be extended to xml_writer
         parser = etree.XMLParser(collect_ids=False)
         # Parse the XML file
         tree = etree.parse(input_filename, parser)
         # Get the XML tree
         self.root = tree.getroot()
         # Check xml root tag
-        if not check_xml(self.root):
-            user_msg = f"Xml's file structure has changed, please delete {input_filename} " \
-                       f"and re-execute your whole notebook"
-            return user_msg
-
-        self.xml_dict = {'xml_type_list': get_type_list(self.root),
-                         'xml_function_list': get_functions(self.root),
-                         'xml_state_list': get_state(self.root),
-                         'xml_transition_list': get_transition(self.root),
-                         'xml_fun_elem_list': get_functional_element(self.root),
-                         'xml_view_list': get_views(self.root),
-                         'xml_attribute_list': get_attributes(self.root),
-                         'xml_fun_inter_list': get_functional_interface(self.root),
-                         'xml_phy_elem_list': get_physical_element(self.root),
-                         'xml_phy_inter_list': get_physical_interface(self.root),
-                         }
-        # Create data(and set predecessors), consumers, producers lists
-        self.xml_dict['xml_data_list'], self.xml_dict['xml_producer_function_list'], self.xml_dict[
-            'xml_consumer_function_list'] = get_data(self.root, self.xml_dict['xml_function_list'])
-
-        get_type_obj_from_str(self.xml_dict)
+        if self.check_xml():
+            # First retrieve extended types
+            self.xml_dict['xml_type_list'] = self.parse_type_list()
+            self.xml_dict['xml_function_list'] = self.parse_function_list()
+            self.xml_dict['xml_state_list'] = self.parse_state_list()
+            self.xml_dict['xml_transition_list'] = self.parse_transition_list()
+            self.xml_dict['xml_fun_elem_list'] = self.parse_functional_element_list()
+            self.xml_dict['xml_view_list'] = self.parse_view_list()
+            self.xml_dict['xml_attribute_list'] = self.parse_attribute_list()
+            self.xml_dict['xml_fun_inter_list'] = self.parse_functional_interface_list()
+            self.xml_dict['xml_phy_elem_list'] = self.parse_physical_element_list()
+            self.xml_dict['xml_phy_inter_list'] = self.parse_physical_interface_list()
+
+            # Then create data(and set predecessors), consumers, producers lists
+            self.xml_dict['xml_data_list'], self.xml_dict['xml_producer_function_list'], self.xml_dict[
+                'xml_consumer_function_list'] = self.parse_data_list()
+
+            # Finally update object types
+            self.update_object_type()
+        else:
+            Logger.set_error(__name__,
+                             f"Xml's file structure has changed, please delete {input_filename} "
+                             f"and re-execute your whole notebook")
 
         return self.xml_dict
 
+    def check_xml(self):
+        """Check XML file structure
 
-def check_xml(root):
-    """Check xml file root, since jarvis4se version 1.3 it's <systemAnalysis>"""
-    if root.tag == "systemAnalysis":
-        return True
-    else:
-        return False
-
-
-def get_functions(root):
-    """Get Function objects"""
-    function_list = set()
-    parent_list = {}
-    xml_function_list = root.iter('function')
-    for xml_function in xml_function_list:
-        # Instantiate functions and add them to a list
-        function = datamodel.Function(p_id=xml_function.get('id'), p_name=xml_function.get('name'),
-                                      p_alias=xml_function.get('alias'),
-                                      p_type=xml_function.get('type'),
-                                      p_derived=xml_function.get('derived'))
-        function.set_operand()
-
-        function_list.add(function)
-        # Looking for functions with "functionalPart" i.e childs and create a list
-        xml_function_part_list = xml_function.iter('functionPart')
-        for xml_function_part in xml_function_part_list:
-            parent_list[xml_function_part.get('id')] = function.id
-
-    # Loop to set parent() and add_child() to functions
-    for child_id in parent_list:
-        for child_function in function_list:
-            if child_function.id == child_id:
-                for parent_function in function_list:
-                    if parent_function.id == parent_list[child_id]:
-                        child_function.set_parent(parent_function)
-                        parent_function.add_child(child_function)
-                        break
-                break
-
-    for elem in function_list:
-        for derived in function_list:
-            if elem.derived == derived.id:
-                elem.derived = derived
-                break
-
-    return function_list
-
-
-def get_data(root, function_list):
-    """Get Data objects"""
-    data_list = set()
-    consumer_function_list = []
-    producer_function_list = []
-
-    xml_data_list = root.iter('data')
-    for xml_data in xml_data_list:
-        # Instantiate data and add it to a list
-        data = datamodel.Data(p_id=xml_data.get('id'),
-                              p_name=xml_data.get('name'),
-                              p_type=xml_data.get('type'))
-        data_list.add(data)
-        # looking for all elements with tag "consumer" and create a list [flow, consumer_function]
-        xml_consumer_list = xml_data.iter('consumer')
-        for xml_consumer in xml_consumer_list:
-            for function in function_list:
-                if xml_consumer.get('id') == function.id:
-                    consumer_function_list.append([xml_data.get('name'), function])
-                    if xml_consumer.get('role') != 'none':
-                        function.set_input_role(xml_data.get('name'))
-                    # Avoid to reset the input role once already set
-                    elif function.input_role is None:
-                        function.set_input_role(None)
-
-        # looking for all elements with tag "producer" and create a list [flow, producer_function]
-        xml_producer_list = xml_data.iter('producer')
-        for xml_producer in xml_producer_list:
-            for function in function_list:
-                if xml_producer.get('id') == function.id:
-                    producer_function_list.append([xml_data.get('name'), function])
-
-    # Loop on the data_list once created to find the predecessor and add it to list
-    for d in data_list:
-        xml_data_list = root.iter('data')
-        for xml_data in xml_data_list:
-            if xml_data.get('id') == d.id:
-                # looking for all elements with tag "predecessor" and create a
-                # list [flow, producer_function]
-                xml_predecessor_list = xml_data.iter('predecessor')
-                for xml_predecessor in xml_predecessor_list:
-                    for dodo in data_list:
-                        if xml_predecessor.get('id') == dodo.id:
-                            d.add_predecessor(dodo)
-
-    return data_list, producer_function_list, consumer_function_list
-
-
-def get_state(root):
-    """Get State objects"""
-    state_list = set()
-    state_parent_dict = {}
-    xml_state_list = root.iter('state')
-    for xml_state in xml_state_list:
-        # Instantiate states and add them to a list
-        state = datamodel.State(p_id=xml_state.get('id'),
-                                p_name=xml_state.get('name'),
-                                p_alias=xml_state.get('alias'),
-                                p_type=xml_state.get('type'))
-        state_list.add(state)
-        # Looking for states with "statePart" i.e child and create a list
-        xml_state_part_list = xml_state.iter('statePart')
-        for xml_state_part in xml_state_part_list:
-            state_parent_dict[xml_state_part.get('id')] = state.id
-
-        # Looking for allocated functions and add them to the state
-        xml_allocated_function_list = xml_state.iter('allocatedFunction')
-        for xml_allo_fun in xml_allocated_function_list:
-            state.add_allocated_function(xml_allo_fun.get("id"))
-
-    # Loop to set parent() and add_child() to states
-    for child_id in state_parent_dict:
-        for child_state in state_list:
-            if child_state.id == child_id:
-                for parent_state in state_list:
-                    if parent_state.id == state_parent_dict[child_id]:
-                        child_state.set_parent(parent_state)
-                        parent_state.add_child(child_state)
-                        break
-                break
-
-    return state_list
-
+        Since jarvis4se version 1.3 XML root element is <systemAnalysis>
+        @return XML file is well-structured (True) or not (FALSE
+        """
+        if self.root.tag == "systemAnalysis":
+            return True
+        else:
+            return False
+
+    @staticmethod
+    def update_parental_relationship(parent_id_list, element_list):
+        """Update parental relationship between two elements
+
+        The elements must implement the following methods:
+        - set_parent()
+        - add_child()
+
+        @param[in] parent_id_list : list of parent element identifiers
+        @param[in] element_list : list of element
+        @return None
+        """
+        for child_id in parent_id_list:
+            for element in element_list:
+                if element.id == child_id:
+                    # We have the child element, now search for the parent element
+                    for parent_elem in element_list:
+                        if parent_elem.id == parent_id_list[child_id]:
+                            element.set_parent(parent_elem)
+                            parent_elem.add_child(element)
+
+                            Logger.set_debug(__name__, f"Element [{parent_elem.id}, {parent_elem.name}]"
+                                                       f" is parent of "
+                                                       f"element [{element.id}, {element.name}]")
+                            break
+                    break
 
-def get_transition(root):
-    """Get Transition objects"""
-    transition_list = set()
-    xml_transition_list = root.iter('transition')
-    for xml_transition in xml_transition_list:
-        # Instantiate transitions and add them to a list
-        transition = datamodel.Transition(p_id=xml_transition.get('id'),
-                                          p_name=xml_transition.get('name'),
-                                          p_alias=xml_transition.get('alias'),
-                                          p_type=xml_transition.get('type'),
-                                          p_source=xml_transition.get('source'),
-                                          p_destination=xml_transition.get('destination'))
-        # Looking for conditions and add them to the transition
-        xml_transition_condition_list = xml_transition.iter('condition')
-        for xml_condition in xml_transition_condition_list:
-            transition.add_condition(xml_condition.get("text"))
-
-        transition_list.add(transition)
-
-    return transition_list
-
-
-def get_functional_element(root):
-    """Get Functional Element objects"""
-    functional_element_list = set()
-    fun_elem_parent_dict = {}
-    xml_functional_element_list = root.iter('functionalElement')
-    for xml_func_elem in xml_functional_element_list:
-        # Instantiate functional element and add them to a list
-        fun_elem = datamodel.FunctionalElement(p_id=xml_func_elem.get('id'),
-                                               p_name=xml_func_elem.get('name'),
-                                               p_alias=xml_func_elem.get('alias'),
-                                               p_type=xml_func_elem.get('type'),
-                                               p_derived=xml_func_elem.get('derived'))
-        functional_element_list.add(fun_elem)
-        # Looking for "functionalElementPart" i.e child and create a list
-        xml_functional_part_list = xml_func_elem.iter('functionalElementPart')
-        for xml_state_part in xml_functional_part_list:
-            fun_elem_parent_dict[xml_state_part.get('id')] = fun_elem.id
-
-        # Looking for allocated states and add them to the functional element
-        xml_allocated_state_list = xml_func_elem.iter('allocatedState')
-        for xml_allo_state in xml_allocated_state_list:
-            fun_elem.add_allocated_state(xml_allo_state.get("id"))
-
-        # Looking for allocated functions and add them to the functional element
-        xml_allocated_function_list = xml_func_elem.iter('allocatedFunction')
-        for xml_allo_fun in xml_allocated_function_list:
-            fun_elem.add_allocated_function(xml_allo_fun.get("id"))
-
-        # Looking for exposed interface and add them to the functional element
-        xml_exposed_interface_list = xml_func_elem.iter('exposedInterface')
-        for xml_exp_inter in xml_exposed_interface_list:
-            fun_elem.add_exposed_interface(xml_exp_inter.get("id"))
-
-    # Loop to set parent() and add_child() to fun elem
-    for child_id in fun_elem_parent_dict:
-        for child_state in functional_element_list:
-            if child_state.id == child_id:
-                for parent_state in functional_element_list:
-                    if parent_state.id == fun_elem_parent_dict[child_id]:
-                        child_state.set_parent(parent_state)
-                        parent_state.add_child(child_state)
-                        break
-                break
+    @staticmethod
+    def update_derived_object(element_list):
+        """Update derived objects of an element list based on their identifiers
+
+        @param[in] element_list : list of element
+        @return None
+        """
+        for elem in element_list:
+            for derived in element_list:
+                if elem.derived == derived.id:
+                    elem.derived = derived
+                    break
+
+    def parse_function_list(self):
+        """Parse XML function list
+        @return function list
+        """
+        function_list = set()
+        parent_list = {}
+        xml_function_list = self.root.iter('function')
+        for xml_function in xml_function_list:
+            # Instantiate functions and add them to a list
+            function = datamodel.Function(p_id=xml_function.get('id'), p_name=xml_function.get('name'),
+                                          p_alias=xml_function.get('alias'),
+                                          p_type=xml_function.get('type'),
+                                          p_derived=xml_function.get('derived'))
+            function.set_operand()
+
+            function_list.add(function)
+
+            # Looking for functions with "functionalPart" i.e childs and create a list
+            xml_part_list = xml_function.iter('functionPart')
+            for xml_part in xml_part_list:
+                parent_list[xml_part.get('id')] = function.id
+
+        # Loop to set parent and child to functions
+        self.update_parental_relationship(parent_list, function_list)
+
+        # Loop to update derived functions according to their ids
+        self.update_derived_object(function_list)
+
+        return function_list
+
+    def parse_data_list(self):
+        """Parse XML data list
+        @return data list, producer function list, consumer function list
+        """
+        data_list = set()
+        consumer_function_list = []
+        producer_function_list = []
 
-    for elem in functional_element_list:
-        for derived in functional_element_list:
-            if elem.derived == derived.id:
-                elem.derived = derived
-                break
-
-    return functional_element_list
-
-
-def get_views(root):
-    """Get View objects"""
-    view_list = set()
-    xml_view_list = root.iter('view')
-    for xml_view in xml_view_list:
-        # Instantiate view and add them to a list
-        view = datamodel.View(uid=xml_view.get('id'),
-                              name=xml_view.get('name'),
-                              v_type=xml_view.get('type'))
-        # Looking for allocated items and add them to the view
-        xml_allocated_item_list = xml_view.iter('allocatedItem')
-        for xml_allo_item in xml_allocated_item_list:
-            view.add_allocated_item(xml_allo_item.get("id"))
-
-        view_list.add(view)
-
-    return view_list
-
-
-def get_attributes(root):
-    """Get Attribute objects"""
-    attribute_list = set()
-    xml_attribute_list = root.iter('attribute')
-    for xml_attribute in xml_attribute_list:
-        # Instantiate Attribute and add them to a list
-        attribute = datamodel.Attribute(p_id=xml_attribute.get('id'),
-                                        p_name=xml_attribute.get('name'),
-                                        p_alias=xml_attribute.get('alias'),
-                                        p_type=xml_attribute.get('type'))
-        # Looking for described items and add them to the attribute
-        xml_described_item_list = xml_attribute.iter('describedItem')
-        for xml_described_item in xml_described_item_list:
-            attribute.add_described_item((xml_described_item.get("id"),
-                                          xml_described_item.get("value")))
-
-        attribute_list.add(attribute)
-
-    return attribute_list
-
-
-def get_functional_interface(root):
-    """Get Functional Interface objects"""
-    functional_interface_list = set()
-    xml_fun_inter_list = root.iter('functionalInterface')
-    for xml_fun_inter in xml_fun_inter_list:
-        # Instantiate fun_inter and add them to a list
-        fun_inter = datamodel.FunctionalInterface(p_id=xml_fun_inter.get('id'),
-                                                  p_name=xml_fun_inter.get('name'),
-                                                  p_alias=xml_fun_inter.get('alias'),
-                                                  p_type=xml_fun_inter.get('type'),
-                                                  p_derived=xml_fun_inter.get('derived'))
-        # Looking for allocated data and add them to the fun inter
-        xml_allocated_data_list = xml_fun_inter.iter('allocatedData')
-        for xml_allo_data in xml_allocated_data_list:
-            fun_inter.add_allocated_data(xml_allo_data.get("id"))
-
-        functional_interface_list.add(fun_inter)
-
-    for elem in functional_interface_list:
-        for derived in functional_interface_list:
-            if elem.derived == derived.id:
-                elem.derived = derived
-                break
-
-    return functional_interface_list
-
-
-def get_physical_element(root):
-    """Get Physical Element objects"""
-    physical_element_list = set()
-    phy_elem_parent_dict = {}
-    xml_physical_element_list = root.iter('physicalElement')
-    for xml_phy_elem in xml_physical_element_list:
-        # Instantiate functional element and add them to a list
-        phy_elem = datamodel.PhysicalElement(p_id=xml_phy_elem.get('id'),
-                                             p_name=xml_phy_elem.get('name'),
-                                             p_alias=xml_phy_elem.get('alias'),
-                                             p_type=xml_phy_elem.get('type'),
-                                             p_derived=xml_phy_elem.get('derived'))
-        physical_element_list.add(phy_elem)
-        # Looking for "physicalPart" i.e child and create a list
-        xml_functional_part_list = xml_phy_elem.iter('physicalElementPart')
-        for xml_state_part in xml_functional_part_list:
-            phy_elem_parent_dict[xml_state_part.get('id')] = phy_elem.id
-
-        # Looking for allocated functions and add them to the functional element
-        xml_allocated_fun_elem_list = xml_phy_elem.iter('allocatedFunctionalElement')
-        for xml_allo_fun_elem in xml_allocated_fun_elem_list:
-            phy_elem.add_allocated_fun_elem(xml_allo_fun_elem.get("id"))
-
-        # Looking for exposed interface and add them to the functional element
-        xml_exposed_interface_list = xml_phy_elem.iter('exposedInterface')
-        for xml_exp_inter in xml_exposed_interface_list:
-            phy_elem.add_exposed_interface(xml_exp_inter.get("id"))
-
-    # Loop to set parent() and add_child() to fun elem
-    for child_id in phy_elem_parent_dict:
-        for child_state in physical_element_list:
-            if child_state.id == child_id:
-                for parent_state in physical_element_list:
-                    if parent_state.id == phy_elem_parent_dict[child_id]:
-                        child_state.set_parent(parent_state)
-                        parent_state.add_child(child_state)
+        xml_data_list = self.root.iter('data')
+        for xml_data in xml_data_list:
+            # Instantiate data and add it to a list
+            data = datamodel.Data(p_id=xml_data.get('id'),
+                                  p_name=xml_data.get('name'),
+                                  p_type=xml_data.get('type'))
+            data_list.add(data)
+
+            # looking for all elements with tag "consumer" and create a list [flow_name, consumer_function]
+            xml_consumer_list = xml_data.iter('consumer')
+            for xml_consumer in xml_consumer_list:
+                for function in self.xml_dict['xml_function_list']:
+                    if xml_consumer.get('id') == function.id:
+                        consumer_function_list.append([xml_data.get('name'), function])
+                        Logger.set_debug(__name__, f"Data [{xml_data.get('id')}, {xml_data.get('name')}]"
+                                                   f" is consumed by "
+                                                   f"function [{function.id}, {function.name}]")
+
+                        if xml_consumer.get('role') != 'none':
+                            function.set_input_role(xml_data.get('name'))
+                        # Avoid to reset the input role once already set
+                        elif function.input_role is None:
+                            function.set_input_role(None)
+
+            # looking for all elements with tag "producer" and create a list [flow_name, producer_function]
+            xml_producer_list = xml_data.iter('producer')
+            for xml_producer in xml_producer_list:
+                for function in self.xml_dict['xml_function_list']:
+                    if xml_producer.get('id') == function.id:
+                        producer_function_list.append([xml_data.get('name'), function])
+                        Logger.set_debug(__name__, f"Data [{xml_data.get('id')}, {xml_data.get('name')}]"
+                                                   f" is produced by "
+                                                   f"function [{function.id}, {function.name}]")
+
+        # Loop on the data_list once created to find the predecessor and add it to list
+        for object_data in data_list:
+            xml_data_list = self.root.iter('data')
+            for xml_data in xml_data_list:
+                if xml_data.get('id') == object_data.id:
+                    # looking for all elements with tag "predecessor"
+                    xml_predecessor_list = xml_data.iter('predecessor')
+                    for xml_predecessor in xml_predecessor_list:
+                        for dodo in data_list:
+                            if xml_predecessor.get('id') == dodo.id:
+                                object_data.add_predecessor(dodo)
+
+                                Logger.set_debug(__name__, f"Data [{dodo.id, dodo.name}]"
+                                                           f" is predecessor of "
+                                                           f"data [{object_data.id, object_data.name}]")
+
+        return data_list, producer_function_list, consumer_function_list
+
+    def parse_state_list(self):
+        """Parse XML state list
+        @return state list
+        """
+        state_list = set()
+        parent_list = {}
+        xml_state_list = self.root.iter('state')
+        for xml_state in xml_state_list:
+            # Instantiate states and add them to a list
+            state = datamodel.State(p_id=xml_state.get('id'),
+                                    p_name=xml_state.get('name'),
+                                    p_alias=xml_state.get('alias'),
+                                    p_type=xml_state.get('type'))
+            state_list.add(state)
+
+            # Looking for states with "statePart" i.e child and create a list
+            xml_part_list = xml_state.iter('statePart')
+            for xml_part in xml_part_list:
+                parent_list[xml_part.get('id')] = state.id
+
+            # Looking for allocated functions and add them to the state
+            xml_allocated_function_list = xml_state.iter('allocatedFunction')
+            for xml_function in xml_allocated_function_list:
+                state.add_allocated_function(xml_function.get("id"))
+
+                Logger.set_debug(__name__, f"Function [{xml_function.get('id')}]"
+                                           f" is allocated to "
+                                           f"state [{state.id}, {state.name}]")
+
+        # Loop to set parent and child to states
+        self.update_parental_relationship(parent_list, state_list)
+
+        return state_list
+
+    def parse_transition_list(self):
+        """Parse XML transition list
+        @return transition list
+        """
+        transition_list = set()
+        xml_transition_list = self.root.iter('transition')
+        for xml_transition in xml_transition_list:
+            # Instantiate transitions and add them to a list
+            transition = datamodel.Transition(p_id=xml_transition.get('id'),
+                                              p_name=xml_transition.get('name'),
+                                              p_alias=xml_transition.get('alias'),
+                                              p_type=xml_transition.get('type'),
+                                              p_source=xml_transition.get('source'),
+                                              p_destination=xml_transition.get('destination'))
+
+            transition_list.add(transition)
+
+            # Looking for conditions and add them to the transition
+            xml_transition_condition_list = xml_transition.iter('condition')
+            for xml_condition in xml_transition_condition_list:
+                transition.add_condition(xml_condition.get("text"))
+
+        return transition_list
+
+    def parse_functional_element_list(self):
+        """Parse XML functional element list
+        @return functional element list
+        """
+        functional_element_list = set()
+        parent_list = {}
+        xml_functional_element_list = self.root.iter('functionalElement')
+        for xml_func_elem in xml_functional_element_list:
+            # Instantiate functional element and add them to a list
+            fun_elem = datamodel.FunctionalElement(p_id=xml_func_elem.get('id'),
+                                                   p_name=xml_func_elem.get('name'),
+                                                   p_alias=xml_func_elem.get('alias'),
+                                                   p_type=xml_func_elem.get('type'),
+                                                   p_derived=xml_func_elem.get('derived'))
+            functional_element_list.add(fun_elem)
+
+            # Looking for "functionalElementPart" i.e child and create a list
+            xml_part_list = xml_func_elem.iter('functionalElementPart')
+            for xml_part in xml_part_list:
+                parent_list[xml_part.get('id')] = fun_elem.id
+
+            # Looking for allocated states and add them to the functional element
+            xml_allocated_state_list = xml_func_elem.iter('allocatedState')
+            for xml_state in xml_allocated_state_list:
+                fun_elem.add_allocated_state(xml_state.get("id"))
+                Logger.set_debug(__name__, f"State [{xml_state.get('id')}]"
+                                           f" is allocated to "
+                                           f"functional element [{fun_elem.id}, {fun_elem.name}]")
+
+            # Looking for allocated functions and add them to the functional element
+            xml_allocated_function_list = xml_func_elem.iter('allocatedFunction')
+            for xml_fun in xml_allocated_function_list:
+                fun_elem.add_allocated_function(xml_fun.get("id"))
+                Logger.set_debug(__name__, f"Function [{xml_fun.get('id')}]"
+                                           f" is allocated to "
+                                           f"functional element [{fun_elem.id}, {fun_elem.name}]")
+
+            # Looking for exposed interface and add them to the functional element
+            xml_exposed_interface_list = xml_func_elem.iter('exposedInterface')
+            for xml_exp_inter in xml_exposed_interface_list:
+                fun_elem.add_exposed_interface(xml_exp_inter.get("id"))
+                Logger.set_debug(__name__, f"Functional interface [{xml_exp_inter.get('id')}]"
+                                           f" is exposed by "
+                                           f"functional element [{fun_elem.id}, {fun_elem.name}]")
+
+        # Loop to set parent and child to functional elements
+        self.update_parental_relationship(parent_list, functional_element_list)
+
+        # Loop to update derived functional elements according to their ids
+        self.update_derived_object(functional_element_list)
+
+        return functional_element_list
+
+    def parse_view_list(self):
+        """Parse XML view list
+        @return view list
+        """
+        view_list = set()
+        xml_view_list = self.root.iter('view')
+        for xml_view in xml_view_list:
+            # Instantiate view and add them to a list
+            view = datamodel.View(uid=xml_view.get('id'),
+                                  name=xml_view.get('name'),
+                                  v_type=xml_view.get('type'))
+
+            view_list.add(view)
+
+            # Looking for allocated items and add them to the view
+            xml_allocated_item_list = xml_view.iter('allocatedItem')
+            for xml_item in xml_allocated_item_list:
+                view.add_allocated_item(xml_item.get("id"))
+                Logger.set_debug(__name__, f"Element [{xml_item.get('id')}]"
+                                           f" is allocated to "
+                                           f"view [{view.id}, {view.name}]")
+
+        return view_list
+
+    def parse_attribute_list(self):
+        """Parse XML attribute list
+        @return attribute list
+        """
+        attribute_list = set()
+        xml_attribute_list = self.root.iter('attribute')
+        for xml_attribute in xml_attribute_list:
+            # Instantiate Attribute and add them to a list
+            attribute = datamodel.Attribute(p_id=xml_attribute.get('id'),
+                                            p_name=xml_attribute.get('name'),
+                                            p_alias=xml_attribute.get('alias'),
+                                            p_type=xml_attribute.get('type'))
+
+            attribute_list.add(attribute)
+
+            # Looking for described items and add them to the attribute
+            xml_described_item_list = xml_attribute.iter('describedItem')
+            for xml_described_item in xml_described_item_list:
+                attribute.add_described_item((xml_described_item.get("id"),
+                                              xml_described_item.get("value")))
+                Logger.set_debug(__name__, f"Element [{xml_described_item.get('id')}]"
+                                           f" is described by "
+                                           f"view [{attribute.id}, {attribute.name}]"
+                                           f" with the value : {xml_described_item.get('value')}")
+
+        return attribute_list
+
+    def parse_functional_interface_list(self):
+        """Parse XML functional interface list
+        @return functional interface list
+        """
+        functional_interface_list = set()
+        xml_fun_inter_list = self.root.iter('functionalInterface')
+        for xml_fun_inter in xml_fun_inter_list:
+            # Instantiate fun_inter and add them to a list
+            fun_inter = datamodel.FunctionalInterface(p_id=xml_fun_inter.get('id'),
+                                                      p_name=xml_fun_inter.get('name'),
+                                                      p_alias=xml_fun_inter.get('alias'),
+                                                      p_type=xml_fun_inter.get('type'),
+                                                      p_derived=xml_fun_inter.get('derived'))
+
+            functional_interface_list.add(fun_inter)
+
+            # Looking for allocated data and add them to the fun inter
+            xml_allocated_data_list = xml_fun_inter.iter('allocatedData')
+            for xml_data in xml_allocated_data_list:
+                fun_inter.add_allocated_data(xml_data.get("id"))
+                Logger.set_debug(__name__, f"Data [{xml_data.get('id')}]"
+                                           f" is allocated to "
+                                           f"functional interface [{fun_inter.id}, {fun_inter.name}]")
+
+        # Loop to update derived functional elements according to their ids
+        self.update_derived_object(functional_interface_list)
+
+        return functional_interface_list
+
+    def parse_physical_element_list(self):
+        """Parse XML physical element list
+        @return physical element list
+        """
+        physical_element_list = set()
+        parent_list = {}
+        xml_physical_element_list = self.root.iter('physicalElement')
+        for xml_phy_elem in xml_physical_element_list:
+            # Instantiate functional element and add them to a list
+            phy_elem = datamodel.PhysicalElement(p_id=xml_phy_elem.get('id'),
+                                                 p_name=xml_phy_elem.get('name'),
+                                                 p_alias=xml_phy_elem.get('alias'),
+                                                 p_type=xml_phy_elem.get('type'),
+                                                 p_derived=xml_phy_elem.get('derived'))
+            physical_element_list.add(phy_elem)
+
+            # Looking for "physicalPart" i.e child and create a list
+            xml_functional_part_list = xml_phy_elem.iter('physicalElementPart')
+            for xml_part in xml_functional_part_list:
+                parent_list[xml_part.get('id')] = phy_elem.id
+
+            # Looking for allocated functions and add them to the functional element
+            xml_allocated_fun_elem_list = xml_phy_elem.iter('allocatedFunctionalElement')
+            for xml_fun_elem in xml_allocated_fun_elem_list:
+                phy_elem.add_allocated_fun_elem(xml_fun_elem.get("id"))
+                Logger.set_debug(__name__, f"Functional element [{xml_fun_elem.get('id')}]"
+                                           f" is allocated to "
+                                           f"physical element [{phy_elem.id}, {phy_elem.name}]")
+
+            # Looking for exposed interface and add them to the functional element
+            xml_exposed_interface_list = xml_phy_elem.iter('exposedInterface')
+            for xml_exp_inter in xml_exposed_interface_list:
+                phy_elem.add_exposed_interface(xml_exp_inter.get("id"))
+                Logger.set_debug(__name__, f"Physical interface [{xml_exp_inter.get('id')}]"
+                                           f" is exposed by "
+                                           f"physical element [{phy_elem.id}, {phy_elem.name}]")
+
+        # Loop to set parent and child to functions
+        self.update_parental_relationship(parent_list, physical_element_list)
+
+        # Loop to update derived functions according to their ids
+        self.update_derived_object(physical_element_list)
+
+        return physical_element_list
+
+    def parse_physical_interface_list(self):
+        """Parse XML physical interface list
+        @return physical interface list
+        """
+        physical_interface_list = set()
+        xml_phy_inter_list = self.root.iter('physicalInterface')
+        for xml_phy_inter in xml_phy_inter_list:
+            # Instantiate phy_inter and add them to a list
+            phy_inter = datamodel.PhysicalInterface(p_id=xml_phy_inter.get('id'),
+                                                    p_name=xml_phy_inter.get('name'),
+                                                    p_alias=xml_phy_inter.get('alias'),
+                                                    p_type=xml_phy_inter.get('type'),
+                                                    p_derived=xml_phy_inter.get('derived'))
+            physical_interface_list.add(phy_inter)
+
+            # Looking for allocated fun_inter and add them to the phy inter
+            xml_allocated_inter_list = xml_phy_inter.iter('allocatedFunctionalInterface')
+            for xml_inter in xml_allocated_inter_list:
+                phy_inter.add_allocated_fun_inter(xml_inter.get("id"))
+                Logger.set_debug(__name__, f"Functional interface [{xml_inter.get('id')}]"
+                                           f" is allocated to "
+                                           f"physical interface [{phy_inter.id}, {phy_inter.name}]")
+
+        # Loop to update derived functions according to their ids
+        self.update_derived_object(physical_interface_list)
+
+        return physical_interface_list
+
+    def parse_type_list(self):
+        """Parse XML type list
+        @return type list
+        """
+        type_list = set()
+        xml_type_list = self.root.iter('type')
+        for xml_type in xml_type_list:
+            # Instantiate Type and add them to a list
+            type_obj = datamodel.Type(p_id=xml_type.get('id'),
+                                      p_name=xml_type.get('name'),
+                                      p_alias=xml_type.get('alias'),
+                                      p_base=xml_type.get('base'))
+            type_list.add(type_obj)
+
+        # Update base type depending if it is a 3SE base type or if it is a custom one
+        for obj_type in type_list:
+            if any(obj_type.base in a for a in [str(i) for i in datamodel.BaseType]):
+                obj_type.base = datamodel.BaseType[obj_type.base.upper().replace(" ", "_")]
+            else:
+                is_found = False
+                for base in type_list:
+                    if obj_type.base == base.id:
+                        obj_type.base = base
+                        is_found = True
                         break
-                break
-
-    for elem in physical_element_list:
-        for derived in physical_element_list:
-            if elem.derived == derived.id:
-                elem.derived = derived
-                break
-
-    return physical_element_list
-
-
-def get_physical_interface(root):
-    """Get Physical Interface objects"""
-    physical_interface_list = set()
-    xml_phy_inter_list = root.iter('physicalInterface')
-    for xml_phy_inter in xml_phy_inter_list:
-        # Instantiate phy_inter and add them to a list
-        phy_inter = datamodel.PhysicalInterface(p_id=xml_phy_inter.get('id'),
-                                                p_name=xml_phy_inter.get('name'),
-                                                p_alias=xml_phy_inter.get('alias'),
-                                                p_type=xml_phy_inter.get('type'),
-                                                p_derived=xml_phy_inter.get('derived'))
-        # Looking for allocated fun_inter and add them to the phy inter
-        xml_allocated_inter_list = xml_phy_inter.iter('allocatedFunctionalInterface')
-        for xml_allo_inter in xml_allocated_inter_list:
-            phy_inter.add_allocated_fun_inter(xml_allo_inter.get("id"))
-
-        physical_interface_list.add(phy_inter)
-
-    for inter in physical_interface_list:
-        for derived in physical_interface_list:
-            if inter.derived == derived.id:
-                inter.derived = derived
-                break
-
-    return physical_interface_list
-
-
-def get_type_list(root):
-    """Get Type objects"""
-    type_list = set()
-    xml_type_list = root.iter('type')
-    for xml_type in xml_type_list:
-        # Instantiate Type and add them to a list
-        type_obj = datamodel.Type(p_id=xml_type.get('id'),
-                                  p_name=xml_type.get('name'),
-                                  p_alias=xml_type.get('alias'),
-                                  p_base=xml_type.get('base'))
-        type_list.add(type_obj)
-
-    for obj_type in type_list:
-        if any(obj_type.base in a for a in [str(i) for i in datamodel.BaseType]):
-            obj_type.base = datamodel.BaseType[obj_type.base.upper().replace(" ", "_")]
-            continue
-        for base in type_list:
-            if obj_type.base == base.id:
-                obj_type.base = base
-                break
-                
-    return type_list
-
-
-def get_type_obj_from_str(xml_dict):
-    """Return xml lists with obj.type= ObjType/BaseType"""
-    unwanted_xml_list = ('xml_type_list', 'xml_consumer_function_list', 'xml_producer_function_list')
-    for key, xml_list in xml_dict.items():
-        if key not in unwanted_xml_list:
-            for obj in xml_list:
-                try:
-                    obj.type = datamodel.BaseType[obj.type.upper().replace(" ", "_")]
-                except KeyError:
-                    for type_obj in xml_dict['xml_type_list']:
-                        if obj.type == type_obj.id:
-                            obj.type = type_obj
-                            break
 
+                if not is_found:
+                    Logger.set_error(__name__,
+                                     f"Unknown type {obj_type} found when parsing xml")
+
+        return type_list
+
+    def update_object_type(self):
+        """Update objects in the dictionary with their types.
+        @return None
+        """
+        # Following lists does not contain any type definition
+        unwanted_xml_list = ('xml_type_list', 'xml_consumer_function_list', 'xml_producer_function_list')
+        for key, xml_list in self.xml_dict.items():
+            if key not in unwanted_xml_list:
+                for obj in xml_list:
+                    try:
+                        # Base type are defined with their names
+                        obj.type = datamodel.BaseType[obj.type.upper().replace(" ", "_")]
+                    except KeyError:
+                        # Extended types are defined in xml_type_list with their ids
+                        is_found = False
+                        for type_obj in self.xml_dict['xml_type_list']:
+                            if obj.type == type_obj.id:
+                                obj.type = type_obj
+                                is_found = True
+                                break
+
+                        if not is_found:
+                            Logger.set_error(__name__,
+                                             f"Unknown type {obj.type} found when parsing xml")
```

### Comparing `jarvis4se-1.3.4/src/xml_adapter/xml_writer.py` & `jarvis4se-1.3.5/src/xml_adapter/xml_writer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,579 +1,702 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""Module containing class methods to write within xml"""
+"""@defgroup xml_adapter
+Module for 3SE xml parsing and writing
+"""
 # Libraries
 from lxml import etree
+import os
 
+# Modules
 import datamodel
+from tools import Logger
 
 
-class GenerateXML:
-    """Class to generate XML"""
+class XmlWriter3SE:
+    """@ingroup xml_adapter
+    @anchor XmlWriter3SE
+    3SE XML writer
+    """
+
     def __init__(self, xml_file):
-        """Initialize XML structure/tags and file's object"""
+        """@var root
+        Reference to the XML root object
+
+        @var tree
+        Reference to the XML elements tree
+
+        @var file
+        Reference to the XML file to be written
+        """
+
         self.root = etree.Element("systemAnalysis")
+
         fun_arch = etree.SubElement(self.root, "funcArch")
         fun_arch_tags = ['functionList', 'dataList', 'stateList', 'transitionList',
                          'functionalElementList', 'functionalInterfaceList']
         for tag in fun_arch_tags:
             etree.SubElement(fun_arch, tag)
+
         phy_arch = etree.SubElement(self.root, "phyArch")
         phy_arch_tags = ['physicalElementList', 'physicalInterfaceList']
         for tag in phy_arch_tags:
             etree.SubElement(phy_arch, tag)
+
         viewpoint = etree.SubElement(self.root, "viewPoint")
         viewpoint_tags = ['viewList', 'attributeList', 'typeList']
         for tag in viewpoint_tags:
             etree.SubElement(viewpoint, tag)
+
         self.tree = etree.ElementTree(self.root)
 
         if len(xml_file) > 0:
             self.file = xml_file
         else:
             self.file = "Output.xml"
 
+    @staticmethod
+    def check_object_type(obj):
+        """Check object type against 3SE base types
+        @param[in] obj : object reference
+        @return object type to be written in XML file
+        """
+        if isinstance(obj, datamodel.BaseType):
+            # Object is a basic 3SE type
+            type_str = str(obj)
+        else:
+            type_str = obj.id
+
+        return type_str
+
     def write_function(self, function_list):
-        """Method to write functions from function's list"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            if root.find('.//functionList') is None:
-                etree.SubElement(root, 'functionList')
-            # Loop on each flow/data
-            for function_list_tag in root.findall(".//functionList"):
-                # Loop on function's list
-                for function in function_list:
-                    if isinstance(function.type, datamodel.BaseType):
-                        type_str = str(function.type)
-                    else:
-                        type_str = function.type.id
-                    function_tag = etree.SubElement(function_list_tag, "function",
-                                                    {'id': function.id,
-                                                     'name': function.name,
-                                                     'type': type_str,
-                                                     'alias': function.alias,
-                                                     'derived': function.derived})
+        """Write functions from list of functions
+        @param[in] function_list : list of functions
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        if root.find('.//functionList') is None:
+            etree.SubElement(root, 'functionList')
+
+        for function_list_tag in root.findall(".//functionList"):
+            for function in function_list:
+                function_tag = etree.SubElement(function_list_tag, "function",
+                                                {'id': function.id,
+                                                 'name': function.name,
+                                                 'type': self.check_object_type(function.type),
+                                                 'alias': function.alias,
+                                                 'derived': function.derived})
 
-                    _functional_part_list_tag = etree.SubElement(function_tag, "functionPartList")
+                _functional_part_list_tag = etree.SubElement(function_tag, "functionPartList")
 
-        self.write()
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write_data(self, data_list):
-        """Method to add data flows"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            if root.find('.//dataList') is None:
-                etree.SubElement(root, 'dataList')
-            for data_list_tag in root.findall('.//dataList'):
-                for data in data_list:
-                    if isinstance(data.type, datamodel.BaseType):
-                        type_str = str(data.type)
-                    else:
-                        type_str = data.type.id
-                    existing_data_tag = data_list_tag.find('.//dataList/data')
-                    if existing_data_tag is not None:
-                        tag = existing_data_tag
-                    else:
-                        tag = data_list_tag
-                    data_tag = etree.SubElement(tag, "data", {'name': data.name,
-                                                              'type': type_str,
-                                                              'id': data.id})
-
-                    _consumer_list_tag = etree.SubElement(data_tag, "consumerList")
-
-                    _producer_list_tag = etree.SubElement(data_tag, "producerList")
-
-                    _predecessor_list_tag = etree.SubElement(data_tag, "predecessorList")
-
-        self.write()
-
-    def write_consumer(self, consumer_list):
-        """Method to write consumers by list [data_name, function]"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            for i in consumer_list:
-                for consumer_list_tag in root.findall(".//dataList/data[@name='" + str(i[0])
-                                                      + "']/consumerList"):
-                    if not i[1].operand:
-                        _consumer_tag = etree.SubElement(consumer_list_tag, "consumer",
-                                                         {'id': i[1].id, 'role': "none"})
-                    else:
-                        _consumer_tag = etree.SubElement(consumer_list_tag, "consumer",
-                                                         {'id': i[1].id, 'role': i[1].operand})
-
-        self.write()
-
-    def write_producer(self, producer_list):
-        """Method to write producers by list [data_name, function]"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            for i in producer_list:
-                for producer_list_tag in root.findall(".//dataList/data[@name='" + str(i[0])
-                                                      + "']/producerList"):
-
-                    _producer_tag = etree.SubElement(producer_list_tag, "producer", {'id': i[1].id})
-
-        self.write()
-
-    def write_predecessor(self, predecessor_list):
-        """Method to write predecessors by list [data, predecessor]"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            for i in predecessor_list:
-                for predecessor_list_tag in root.findall(
-                        ".//dataList/data[@name='" + str(i[0].name) + "']/predecessorList"):
-
-                    _producer_tag = etree.SubElement(predecessor_list_tag, "predecessor",
-                                                     {'id': i[1].id})
-
-        self.write()
-
-    def delete_single_consumer_producer(self, data, function, value):
-        """Method to delete the parents (consumer or producer) when flow is within a component"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            # Find specific consumer/producer to delete
-            for tag in root.findall(
-                    ".//data[@name='" + data + "']/" + value + "List/" + value + "[@id='"
-                    + function.id + "']"):
-                tag.getparent().remove(tag)
-        self.write()
+        """Write data from list of data
+        @param[in] data_list : list of data
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        if root.find('.//dataList') is None:
+            etree.SubElement(root, 'dataList')
+
+        for data_list_tag in root.findall('.//dataList'):
+            for data in data_list:
+                data_tag = etree.SubElement(data_list_tag, "data",
+                                            {'name': data.name,
+                                             'type': self.check_object_type(data.type),
+                                             'id': data.id})
+
+            _consumer_list_tag = etree.SubElement(data_tag, "consumerList")
+
+            _producer_list_tag = etree.SubElement(data_tag, "producerList")
+
+            _predecessor_list_tag = etree.SubElement(data_tag, "predecessorList")
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
+
+    def write_data_consumer(self, consumer_list):
+        """Write consumers by list [data_name, function]
+        @param[in] consumer_list : list of consumers
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        for consumer in consumer_list:
+            for xml_element in root.findall(".//dataList/data[@name='" + str(consumer[0]) + "']"):
+                if xml_element.find('consumerList') is None:
+                    etree.SubElement(xml_element, 'consumerList')
+
+            for consumer_list_tag in root.findall(".//dataList/data[@name='" + str(consumer[0])
+                                                  + "']/consumerList"):
+                if not consumer[1].operand:
+                    _consumer_tag = etree.SubElement(consumer_list_tag, "consumer",
+                                                     {'id': consumer[1].id, 'role': "none"})
+                else:
+                    _consumer_tag = etree.SubElement(consumer_list_tag, "consumer",
+                                                     {'id': consumer[1].id, 'role': consumer[1].operand})
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
+
+    def write_data_producer(self, producer_list):
+        """Write producers by list [data_name, function]
+        @param[in] producer_list : list of producers
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        for producer in producer_list:
+            for xml_element in root.findall(".//dataList/data[@name='" + str(producer[0]) + "']"):
+                if xml_element.find('producerList') is None:
+                    etree.SubElement(xml_element, 'producerList')
+
+            for producer_list_tag in root.findall(".//dataList/data[@name='" + str(producer[0])
+                                                  + "']/producerList"):
+                _producer_tag = etree.SubElement(producer_list_tag, "producer", {'id': producer[1].id})
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
+
+    def write_data_predecessor(self, predecessor_list):
+        """Write predecessors by list [data, predecessor]
+        @param[in] predecessor_list : list of predecessors
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        for predecessor in predecessor_list:
+            for xml_element in root.findall(".//dataList/data[@name='" + str(predecessor[0].name) + "']"):
+                if xml_element.find('predecessorList') is None:
+                    etree.SubElement(xml_element, 'predecessorList')
+
+            for predecessor_list_tag in root.findall(
+                    ".//dataList/data[@name='" + str(predecessor[0].name) + "']/predecessorList"):
+                _predecessor_tag = etree.SubElement(predecessor_list_tag, "predecessor",
+                                                    {'id': predecessor[1].id})
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
+
+    def write_data_relationship(self, flow_function, relationship_type):
+        """Write data relationship (either consumer or producer or predecessor)
+
+        @param[in] object : [flow, function] to be deleted
+        @param[in] relationship_type : "consumer" or "producer" or "predecessor"
+        @return None
+        """
+        flow_function_list = [flow_function]
+
+        if relationship_type == "consumer":
+            self.write_data_consumer(flow_function_list)
+        elif relationship_type == "producer":
+            self.write_data_producer(flow_function_list)
+        elif relationship_type == "predecessor":
+            self.write_data_predecessor(flow_function_list)
+        else:
+            Logger.set_error(__name__, f"Unknown data relationship type: {relationship_type}")
+
+    def delete_data_relationship(self, flow_function, relationship_type):
+        """Delete data relationship (either consumer or producer or predecessor)
+
+        @param[in] object : [flow, function] to be deleted
+        @param[in] relationship_type : "consumer" or "producer" or "predecessor"
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        for tag in root.findall(
+                ".//data[@name='" + flow_function[0] + "']/" + relationship_type + "List/" + relationship_type +
+                "[@id='" + flow_function[1].id + "']"):
+            tag.getparent().remove(tag)
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write(self):
-        """Method to write within XML file"""
-        with open(self.file, "wb") as file:
-            self.tree.write(file, encoding='utf-8', xml_declaration=True, pretty_print=True)
+        """Write within the XML file
+        @return None
+        """
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write_state(self, state_list):
-        """Method to write states from state's list"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            if root.find('.//stateList') is None:
-                etree.SubElement(root, 'stateList')
-            for state_list_tag in root.findall(".//stateList"):
-                for state in state_list:
-                    if isinstance(state.type, datamodel.BaseType):
-                        type_str = str(state.type)
-                    else:
-                        type_str = state.type.id
-                    state_tag = etree.SubElement(state_list_tag, "state",
-                                                 {'id': state.id, 'name': state.name,
-                                                  'type': type_str, 'alias': state.alias})
-
-                    _state_part_list_tag = etree.SubElement(state_tag, "statePartList")
-                    _allocated_function_list_tag = etree.SubElement(state_tag,
-                                                                    "allocatedFunctionList")
-        self.write()
+        """Write state from list of states
+        @param[in] state_list : list of states
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        if root.find('.//stateList') is None:
+            etree.SubElement(root, 'stateList')
+
+        for state_list_tag in root.findall(".//stateList"):
+            for state in state_list:
+                state_tag = etree.SubElement(state_list_tag, "state",
+                                             {'id': state.id,
+                                              'name': state.name,
+                                              'type': self.check_object_type(state.type),
+                                              'alias': state.alias})
+
+                _state_part_list_tag = etree.SubElement(state_tag, "statePartList")
+                _allocated_function_list_tag = etree.SubElement(state_tag,
+                                                                "allocatedFunctionList")
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write_transition(self, transition_list):
-        """Method to write transition from transition's list"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            if root.find('.//transitionList') is None:
-                etree.SubElement(root, 'transitionList')
-            for transition_list_tag in root.findall(".//transitionList"):
-                for transition in transition_list:
-                    if isinstance(transition.type, datamodel.BaseType):
-                        type_str = str(transition.type)
-                    else:
-                        type_str = transition.type.id
-                    transition_tag = etree.SubElement(transition_list_tag, "transition",
-                                                      {'id': transition.id,
-                                                       'name': transition.name,
-                                                       'type': type_str,
-                                                       'alias': transition.alias,
-                                                       'source': str(transition.source),
-                                                       'destination': str(transition.destination)})
-                    _transition_part_list_tag = etree.SubElement(transition_tag, "conditionList")
-        self.write()
+        """Write transition from list of transitions
+        @param[in] transition_list : list of transitions
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        if root.find('.//transitionList') is None:
+            etree.SubElement(root, 'transitionList')
+
+        for transition_list_tag in root.findall(".//transitionList"):
+            for transition in transition_list:
+                transition_tag = etree.SubElement(transition_list_tag, "transition",
+                                                  {'id': transition.id,
+                                                   'name': transition.name,
+                                                   'type': self.check_object_type(transition.type),
+                                                   'alias': transition.alias,
+                                                   'source': str(transition.source),
+                                                   'destination': str(transition.destination)})
+                _transition_part_list_tag = etree.SubElement(transition_tag, "conditionList")
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write_transition_condition(self, transition_condition_list):
-        """Method to write transition's condition by list [transition, condition]"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            for transition in root.findall(".//transition"):
-                for tra, condition in transition_condition_list:
-                    if transition.get('id') == tra.id:
-                        tag = transition.find('conditionList')
-                        _state_part_tag = etree.SubElement(tag, "condition",
-                                                           {'text': str(condition)})
-        self.write()
-
-    def write_source(self, transition_source_list):
-        """Method to write transition's source by list [transition, source]"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            for transition_src in transition_source_list:
-                for state_tag in root.findall(".//transition[@id='" + transition_src[0].id + "']"):
-                    state_tag.set('source', transition_src[1].id)
-        self.write()
-
-    def write_destination(self, transition_destination_list):
-        """Method to write transition's destination by list [transition, destination]"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            for transition_dest in transition_destination_list:
-                for state_tag in root.findall(".//transition[@id='" + transition_dest[0].id + "']"):
-                    state_tag.set('destination', transition_dest[1].id)
-        self.write()
+        """Write transitions by list [transition, condition]
+        @param[in] transition_condition_list : list of transitions
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        for transition_tag in root.findall(".//transition"):
+            for transition, condition in transition_condition_list:
+                if transition_tag.get('id') == transition.id:
+                    tag = transition_tag.find('conditionList')
+                    _state_part_tag = etree.SubElement(tag, "condition",
+                                                       {'text': str(condition)})
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
+
+    def write_transition_source(self, transition_source_list):
+        """Write transition source by list [transition, source]
+        @param[in] transition_source_list : list of sources
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        for transition_src in transition_source_list:
+            for state_tag in root.findall(".//transition[@id='" + transition_src[0].id + "']"):
+                state_tag.set('source', transition_src[1].id)
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
+
+    def write_transition_destination(self, transition_destination_list):
+        """Write transition destination by list [transition, destination]
+        @param[in] transition_destination_list : list of destinations
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        for transition_dest in transition_destination_list:
+            for state_tag in root.findall(".//transition[@id='" + transition_dest[0].id + "']"):
+                state_tag.set('destination', transition_dest[1].id)
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write_functional_element(self, functional_element_list):
-        """Method to write functional element from functional elements list"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            if root.find('.//functionalElementList') is None:
-                etree.SubElement(root, 'functionalElementList')
-            for functional_element_list_tag in root.findall(".//functionalElementList"):
-                for functional_element in functional_element_list:
-                    if isinstance(functional_element.type, datamodel.BaseType):
-                        type_str = str(functional_element.type)
-                    else:
-                        type_str = functional_element.type.id
-                    functional_element_tag = etree.SubElement(
-                        functional_element_list_tag, "functionalElement",
-                        {
-                            'id': functional_element.id,
-                            'name': functional_element.name,
-                            'type': type_str,
-                            'alias': functional_element.alias,
-                            'derived': functional_element.derived}
-                    )
-
-                    _fun_elem_part_list_tag = etree.SubElement(functional_element_tag,
-                                                               "functionalElementPartList")
-                    _allocated_state_list_tag = etree.SubElement(functional_element_tag,
-                                                                 "allocatedStateList")
-                    _allocated_function_list_tag = etree.SubElement(functional_element_tag,
-                                                                    "allocatedFunctionList")
-                    _exposed_interface_list_tag = etree.SubElement(functional_element_tag,
-                                                                   "exposedInterfaceList")
-        self.write()
-
-    def write_exposed_interface(self, fun_elem_inter_list):
-        """Method to write exposed interfaces by list [fun_elem/phy_elem, exposed_interface]"""
-        if isinstance(fun_elem_inter_list[0][0], datamodel.FunctionalElement):
-            string_tag = ".//functionalElement"
-        else:
-            string_tag = ".//physicalElement"
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            for functional_element in root.findall(string_tag):
-                if functional_element.find('exposedInterfaceList') is None:
-                    etree.SubElement(functional_element, 'exposedInterfaceList')
-
-                for fun_elem, inter in fun_elem_inter_list:
-                    if functional_element.get('id') == fun_elem.id:
-                        tag = functional_element.find('exposedInterfaceList')
+        """Write functional element from list of functional elements
+        @param[in] functional_element_list : list of functional elements
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        if root.find('.//functionalElementList') is None:
+            etree.SubElement(root, 'functionalElementList')
+
+        for functional_element_list_tag in root.findall(".//functionalElementList"):
+            for functional_element in functional_element_list:
+                functional_element_tag = etree.SubElement(
+                    functional_element_list_tag, "functionalElement",
+                    {'id': functional_element.id,
+                     'name': functional_element.name,
+                     'type': self.check_object_type(functional_element.type),
+                     'alias': functional_element.alias,
+                     'derived': functional_element.derived})
+
+                _fun_elem_part_list_tag = etree.SubElement(functional_element_tag,
+                                                           "functionalElementPartList")
+                _allocated_state_list_tag = etree.SubElement(functional_element_tag,
+                                                             "allocatedStateList")
+                _allocated_function_list_tag = etree.SubElement(functional_element_tag,
+                                                                "allocatedFunctionList")
+                _exposed_interface_list_tag = etree.SubElement(functional_element_tag,
+                                                               "exposedInterfaceList")
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
+
+    def write_element_exposed_interface(self, element_interface_list):
+        """Write interface by list [element, interface]
+        @param[in] element_interface_list : list of interfaces
+        @return None
+        """
+        for element, inter in element_interface_list:
+            element_tag = self.get_object_tag(element)
+            if element_tag:
+                parser = etree.XMLParser(remove_blank_text=True)
+                root = self.tree.parse(self.file, parser)
+
+                for xml_element in root.findall(".//" + element_tag):
+                    if xml_element.find('exposedInterfaceList') is None:
+                        etree.SubElement(xml_element, 'exposedInterfaceList')
+
+                    if xml_element.get('id') == element.id:
+                        tag = xml_element.find('exposedInterfaceList')
                         _exposed_interface_tag = etree.SubElement(tag, "exposedInterface",
                                                                   {'id': inter.id})
-        self.write()
+
+                self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write_view(self, view_list):
-        """Method to write views from view's list"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            if root.find('.//viewList') is None:
-                etree.SubElement(root, 'viewList')
-            for view_list_tag in root.findall(".//viewList"):
-                for view in view_list:
-                    if isinstance(view.type, datamodel.BaseType):
-                        type_str = str(view.type)
-                    else:
-                        type_str = view.type.id
-                    view_tag = etree.SubElement(view_list_tag, "view",
-                                                 {'id': view.id, 'name': view.name,
-                                                  'type': type_str})
-                    _allocated_item_list_tag = etree.SubElement(view_tag, "allocatedItemList")
-        self.write()
+        """Write view from list of views
+        @param[in] view_list : list of views
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        if root.find('.//viewList') is None:
+            etree.SubElement(root, 'viewList')
+
+        for view_list_tag in root.findall(".//viewList"):
+            for view in view_list:
+                if isinstance(view.type, datamodel.BaseType):
+                    type_str = str(view.type)
+                else:
+                    type_str = view.type.id
+                view_tag = etree.SubElement(view_list_tag, "view",
+                                            {'id': view.id,
+                                             'name': view.name,
+                                             'type': type_str})
+                _allocated_item_list_tag = etree.SubElement(view_tag, "allocatedItemList")
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write_attribute(self, attribute_list):
-        """Method to write attributes from attribute's list"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            if root.find('.//attributeList') is None:
-                etree.SubElement(root, 'attributeList')
-            for attribute_list_tag in root.findall(".//attributeList"):
-                for attribute in attribute_list:
-                    if isinstance(attribute.type, datamodel.BaseType):
-                        type_str = str(attribute.type)
-                    else:
-                        type_str = attribute.type.id
-                    attribute_tag = etree.SubElement(attribute_list_tag, "attribute",
-                                                     {'id': attribute.id, 'name': attribute.name,
-                                                      'type': type_str,
-                                                      'alias': attribute.alias})
-
-                    _described_item_list_tag = etree.SubElement(attribute_tag, "describedItemList")
-
-        self.write()
-
-    def write_described_attribute_item(self, attribute_item_list):
-        """Method to write described item by list [attribute, (described_item, value)]"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            # Loop on each attribute
-            for attribute_element in root.findall(".//attribute"):
-                for attribute, item in attribute_item_list:
-                    if attribute_element.get('id') == attribute.id:
-                        tag = attribute_element.find('describedItemList')
-                        _allocated_item_tag = etree.SubElement(tag, "describedItem",
-                                                               {'id': item[0].id, 'value': item[1]})
-        self.write()
+        """Write attribute from list of attributes
+        @param[in] attribute_list : list of attributes
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        if root.find('.//attributeList') is None:
+            etree.SubElement(root, 'attributeList')
+
+        for attribute_list_tag in root.findall(".//attributeList"):
+            for attribute in attribute_list:
+                attribute_tag = etree.SubElement(attribute_list_tag, "attribute",
+                                                 {'id': attribute.id,
+                                                  'name': attribute.name,
+                                                  'type': self.check_object_type(attribute.type),
+                                                  'alias': attribute.alias})
+
+                _described_item_list_tag = etree.SubElement(attribute_tag, "describedItemList")
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
+
+    def write_attribute_described_item(self, attribute_item_list):
+        """Write attribute described item by list [attribute, (described_item, value)]
+        @param[in] attribute_item_list : list of attribute described items
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        for attribute_element in root.findall(".//attribute"):
+            for attribute, item in attribute_item_list:
+                if attribute_element.get('id') == attribute.id:
+                    tag = attribute_element.find('describedItemList')
+                    _allocated_item_tag = etree.SubElement(tag, "describedItem",
+                                                           {'id': item[0].id, 'value': item[1]})
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write_functional_interface(self, functional_interface_list):
-        """Method to write functional interfaces from interface's list"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            if root.find('.//functionalInterfaceList') is None:
-                etree.SubElement(root, 'functionalInterfaceList')
-            for fun_interface_list_tag in root.findall(".//functionalInterfaceList"):
-                for fun_interface in functional_interface_list:
-                    if isinstance(fun_interface.type, datamodel.BaseType):
-                        type_str = str(fun_interface.type)
-                    else:
-                        type_str = fun_interface.type.id
-                    fun_interface_tag = etree.SubElement(fun_interface_list_tag,
-                                                         "functionalInterface",
-                                                         {'id': fun_interface.id,
-                                                          'name': fun_interface.name,
-                                                          'type': type_str,
-                                                          'alias': fun_interface.alias,
-                                                          'derived': fun_interface.derived})
-                    _allocated_data_list_tag = etree.SubElement(fun_interface_tag,
-                                                                "allocatedDataList")
-        self.write()
+        """Write functional interface from list of functional interfaces
+        @param[in] functional_interface_list : list of functional interfaces
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        if root.find('.//functionalInterfaceList') is None:
+            etree.SubElement(root, 'functionalInterfaceList')
+
+        for fun_interface_list_tag in root.findall(".//functionalInterfaceList"):
+            for fun_interface in functional_interface_list:
+                fun_interface_tag = etree.SubElement(fun_interface_list_tag,
+                                                     "functionalInterface",
+                                                     {'id': fun_interface.id,
+                                                      'name': fun_interface.name,
+                                                      'type': self.check_object_type(fun_interface.type),
+                                                      'alias': fun_interface.alias,
+                                                      'derived': fun_interface.derived})
+
+                _allocated_data_list_tag = etree.SubElement(fun_interface_tag,
+                                                            "allocatedDataList")
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write_physical_element(self, physical_element_list):
-        """Method to write physical element from physical elements list"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            if root.find('.//physicalElementList') is None:
-                etree.SubElement(root, 'physicalElementList')
-            for physical_element_list_tag in root.findall(".//physicalElementList"):
-                for physical_element in physical_element_list:
-                    if isinstance(physical_element.type, datamodel.BaseType):
-                        type_str = str(physical_element.type)
-                    else:
-                        type_str = physical_element.type.id
-                    physical_element_tag = etree.SubElement(
-                        physical_element_list_tag, "physicalElement",
-                        {
-                            'id': physical_element.id,
-                            'name': physical_element.name,
-                            'type': type_str,
-                            'alias': physical_element.alias,
-                            'derived': physical_element.derived}
-                    )
-
-                    _phy_elem_part_list_tag = etree.SubElement(physical_element_tag,
-                                                               "physicalElementPartList")
-                    _allocated_fun_elem_list_tag = etree.SubElement(
-                        physical_element_tag, "allocatedFunctionalElementList")
-                    _exposed_interface_list_tag = etree.SubElement(physical_element_tag,
-                                                                   "exposedInterfaceList")
-        self.write()
+        """Write physical element from list of physical elements
+        @param[in] physical_element_list : list of physical elements
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        if root.find('.//physicalElementList') is None:
+            etree.SubElement(root, 'physicalElementList')
+
+        for physical_element_list_tag in root.findall(".//physicalElementList"):
+            for physical_element in physical_element_list:
+                physical_element_tag = etree.SubElement(
+                    physical_element_list_tag, "physicalElement",
+                    {'id': physical_element.id,
+                     'name': physical_element.name,
+                     'type': self.check_object_type(physical_element.type),
+                     'alias': physical_element.alias,
+                     'derived': physical_element.derived})
+
+                _phy_elem_part_list_tag = etree.SubElement(physical_element_tag,
+                                                           "physicalElementPartList")
+                _allocated_fun_elem_list_tag = etree.SubElement(
+                    physical_element_tag, "allocatedFunctionalElementList")
+                _exposed_interface_list_tag = etree.SubElement(physical_element_tag,
+                                                               "exposedInterfaceList")
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write_physical_interface(self, physical_interface_list):
-        """Method to write physical interfaces from interface's list"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            if root.find('.//physicalInterfaceList') is None:
-                etree.SubElement(root, 'physicalInterfaceList')
-            for phy_interface_list_tag in root.findall(".//physicalInterfaceList"):
-                for phy_interface in physical_interface_list:
-                    if isinstance(phy_interface.type, datamodel.BaseType):
-                        type_str = str(phy_interface.type)
-                    else:
-                        type_str = phy_interface.type.id
-                    phy_interface_tag = etree.SubElement(phy_interface_list_tag,
-                                                         "physicalInterface",
-                                                         {'id': phy_interface.id,
-                                                          'name': phy_interface.name,
-                                                          'type': str(phy_interface.type),
-                                                          'alias': phy_interface.alias,
-                                                          'derived': phy_interface.derived})
-                    _allocated_fun_inter_list_tag = etree.SubElement(
-                        phy_interface_tag, "allocatedFunctionalInterfaceList")
-        self.write()
+        """Write physical interface from list of physical interfaces
+        @param[in] physical_interface_list : list of physical interfaces
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        if root.find('.//physicalInterfaceList') is None:
+            etree.SubElement(root, 'physicalInterfaceList')
+
+        for phy_interface_list_tag in root.findall(".//physicalInterfaceList"):
+            for phy_interface in physical_interface_list:
+                phy_interface_tag = etree.SubElement(phy_interface_list_tag,
+                                                     "physicalInterface",
+                                                     {'id': phy_interface.id,
+                                                      'name': phy_interface.name,
+                                                      'type': self.check_object_type(phy_interface.type),
+                                                      'alias': phy_interface.alias,
+                                                      'derived': phy_interface.derived})
+
+                _allocated_fun_inter_list_tag = etree.SubElement(
+                    phy_interface_tag, "allocatedFunctionalInterfaceList")
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
+
+    @staticmethod
+    def get_object_tag(obj):
+        """Get the XML element tag corresponding to an object
+        @param[in] obj : object reference
+        @return XML tag (when retrieved) or None
+        """
+        elem_tag = None
+        if isinstance(obj, datamodel.Data):
+            elem_tag = "data"
+        elif isinstance(obj, datamodel.Function):
+            elem_tag = "function"
+        elif isinstance(obj, datamodel.FunctionalElement):
+            elem_tag = "functionalElement"
+        elif isinstance(obj, datamodel.FunctionalInterface):
+            elem_tag = "functionalInterface"
+        elif isinstance(obj, datamodel.PhysicalElement):
+            elem_tag = "physicalElement"
+        elif isinstance(obj, datamodel.PhysicalInterface):
+            elem_tag = "physicalInterface"
+        elif isinstance(obj, datamodel.State):
+            elem_tag = "state"
+        elif isinstance(obj, datamodel.Transition):
+            elem_tag = "transition"
+        elif isinstance(obj, datamodel.Attribute):
+            elem_tag = "attribute"
+        elif isinstance(obj, datamodel.View):
+            elem_tag = "view"
+        elif isinstance(obj, datamodel.Type):
+            # Object is an extension of the previous 3SE basic types
+            elem_tag = "type"
+        else:
+            Logger.set_error(__name__, f"Unsupported type for object {obj.id}")
+        return elem_tag
 
     def write_object_alias(self, object_list):
-        """Method to write object's alias by list [object]"""
-        elem_tag = get_object_tag(object_list[0])
-        if elem_tag:
-            with open(self.file, 'rb') as file:
+        """Write object alias by list [object]
+        @param[in] object_list : list of objects
+        @return None
+        """
+        for obj in object_list:
+            elem_tag = self.get_object_tag(obj)
+            if elem_tag:
                 parser = etree.XMLParser(remove_blank_text=True)
-                root = self.tree.parse(file, parser)
-                for obj in object_list:
-                    for obj_tag in root.findall(".//" + elem_tag + "[@id='" + obj.id + "']"):
-                        obj_tag.set('alias', str(obj.alias))
-            self.write()
-
-    def write_derived(self, derived_list):
-        """Method to write derived by list [Object]"""
-        for obj in derived_list:
-            elem_tag = get_object_tag(obj)
-            if elem_tag in derived_obj_tag:
-                with open(self.file, 'rb') as file:
-                    parser = etree.XMLParser(remove_blank_text=True)
-                    root = self.tree.parse(file, parser)
-                    for elem in derived_list:
-                        for fun_inter_tag in root.findall(".//" + elem_tag + "[@id='" +
-                                                          elem.id + "']"):
-                            fun_inter_tag.set('derived', str(elem.derived.id))
-            self.write()
+                root = self.tree.parse(self.file, parser)
+
+                for obj_tag in root.findall(".//" + elem_tag + "[@id='" + obj.id + "']"):
+                    obj_tag.set('alias', str(obj.alias))
+
+                self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
+
+    def write_object_derived(self, object_list):
+        """Write object derived reference by list [object]
+        @param[in] object_list : list of objects
+        @return None
+        """
+        for obj in object_list:
+            elem_tag = self.get_object_tag(obj)
+            if elem_tag:
+                parser = etree.XMLParser(remove_blank_text=True)
+                root = self.tree.parse(self.file, parser)
+
+                for obj_tag in root.findall(".//" + elem_tag + "[@id='" + obj.id + "']"):
+                    obj_tag.set('derived', str(obj.derived.id))
+
+                self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write_object_type(self, object_list):
-        """Method to write object's type by list [object]"""
-        elem_tag = get_object_tag(object_list[0])
-        if elem_tag:
-            with open(self.file, 'rb') as file:
+        """Write object type by list [object]
+        @param[in] object_list : list of objects
+        @return None
+        """
+        for obj in object_list:
+            elem_tag = self.get_object_tag(obj)
+            if elem_tag:
                 parser = etree.XMLParser(remove_blank_text=True)
-                root = self.tree.parse(file, parser)
-                for obj in object_list:
-                    for object_tag in root.findall(".//" + elem_tag + "[@id='" + obj.id + "']"):
-                        if isinstance(obj.type, datamodel.BaseType):
-                            type_name = str(obj.type)
-                        else:
-                            type_name = obj.type.id
-                        object_tag.set('type', type_name)
-            self.write()
+                root = self.tree.parse(self.file, parser)
+
+                for obj_tag in root.findall(".//" + elem_tag + "[@id='" + obj.id + "']"):
+                    obj_tag.set('type', self.check_object_type(obj.type))
+
+                self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write_object_child(self, object_child_list):
-        """Method to write child by list [parent, child]"""
-        elem_tag = get_object_tag(object_child_list[0][0])
-        if elem_tag:
-            with open(self.file, 'rb') as file:
+        """Write object child by list [parent, child]
+        @param[in] object_child_list : list of children
+        @return None
+        """
+        for parent, child in object_child_list:
+            elem_tag = self.get_object_tag(parent)
+            if elem_tag:
                 parser = etree.XMLParser(remove_blank_text=True)
-                root = self.tree.parse(file, parser)
+                root = self.tree.parse(self.file, parser)
                 for obj in root.findall(".//" + elem_tag):
-                    for parent, child in object_child_list:
-                        if obj.get('id') == parent.id:
-                            tag = obj.find(elem_tag + 'PartList')
-                            _obj_element_part_tag = etree.SubElement(tag,
-                                                                     elem_tag + 'Part',
-                                                                     {'id': child.id})
-            self.write()
+                    if obj.get('id') == parent.id:
+                        tag = obj.find(elem_tag + 'PartList')
+                        _obj_element_part_tag = etree.SubElement(tag,
+                                                                 elem_tag + 'Part',
+                                                                 {'id': child.id})
+
+                self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def delete_object(self, object_list):
-        """Method to delete objects by list [object]"""
-        elem_tag = get_object_tag(object_list[0])
-        if elem_tag:
-            with open(self.file, 'rb') as file:
+        """Delete object type by list [object]
+        @param[in] object_list : list of objects
+        @return None
+        """
+        for obj in object_list:
+            elem_tag = self.get_object_tag(obj)
+            if elem_tag:
                 parser = etree.XMLParser(remove_blank_text=True)
-                root = self.tree.parse(file, parser)
-                for obj in object_list:
-                    for obj_tag in root.findall(".//" + elem_tag + "[@id='" + obj.id + "']"):
-                        obj_tag.getparent().remove(obj_tag)
-            self.write()
-
-    def write_objects_allocation(self, objects_list):
-        """Method to write allocated objects from list [Object, Object]"""
-        elem_tag = get_object_tag(objects_list[0][0])
-        if elem_tag:
-            with open(self.file, 'rb') as file:
+                root = self.tree.parse(self.file, parser)
+
+                for obj_tag in root.findall(".//" + elem_tag + "[@id='" + obj.id + "']"):
+                    obj_tag.getparent().remove(obj_tag)
+
+                self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
+
+    @staticmethod
+    def get_allocation_tag(obj):
+        """Get the XML allocation tag corresponding to an object
+        @param[in] obj : object reference
+        @return XML tag (when retrieved) or None
+        """
+        elem_tag = None
+        if isinstance(obj, datamodel.Function):
+            elem_tag = "allocatedFunction"
+        elif isinstance(obj, datamodel.FunctionalElement):
+            elem_tag = "allocatedFunctionalElement"
+        elif isinstance(obj, datamodel.FunctionalInterface):
+            elem_tag = "allocatedFunctionalInterface"
+        elif isinstance(obj, datamodel.State):
+            elem_tag = "allocatedState"
+        elif isinstance(obj, datamodel.Data):
+            elem_tag = "allocatedData"
+        elif isinstance(obj, datamodel.View):
+            elem_tag = "allocatedItem"
+        else:
+            Logger.set_error(__name__, f"Unsupported type for object {obj.id} allocation")
+
+        return elem_tag
+
+    def write_object_allocation(self, object_allocated_object_list):
+        """Write allocated objects from list [Object, Allocated object]
+        @param[in] object_allocated_object_list : list of allocated objects
+        @return None
+        """
+        for obj, allocated_obj in object_allocated_object_list:
+            elem_tag = self.get_object_tag(obj)
+            if elem_tag:
                 parser = etree.XMLParser(remove_blank_text=True)
-                root = self.tree.parse(file, parser)
+                root = self.tree.parse(self.file, parser)
+
                 for obj_tag in root.findall(".//" + elem_tag):
-                    for obj, obj_to_alloc in objects_list:
-                        if obj_tag.get('id') == obj.id:
-                            if elem_tag == "view":
-                                alloc_tag = get_allocation_tag(obj)
-                            else:
-                                alloc_tag = get_allocation_tag(obj_to_alloc)
-                            tag = obj_tag.find(alloc_tag + 'List')
-                            _allocated_obj_tag = etree.SubElement(
-                                tag, alloc_tag, {'id': str(obj_to_alloc.id)})
-            self.write()
+                    if obj_tag.get('id') == obj.id:
+                        if elem_tag == "view":
+                            allocated_tag = self.get_allocation_tag(obj)
+                        else:
+                            allocated_tag = self.get_allocation_tag(allocated_obj)
+
+                        tag = obj_tag.find(allocated_tag + 'List')
+                        _allocated_obj_tag = etree.SubElement(
+                            tag, allocated_tag, {'id': str(allocated_obj.id)})
+
+            self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
 
     def write_type_element(self, type_list):
-        """Method to write type element from type's list"""
-        with open(self.file, 'rb') as file:
-            parser = etree.XMLParser(remove_blank_text=True)
-            root = self.tree.parse(file, parser)
-            if root.find('.//typeList') is None:
-                etree.SubElement(root.find('./viewPoint'), 'typeList')
-            for type_list_tag in root.findall(".//typeList"):
-                for type_elem in type_list:
-                    if isinstance(type_elem.base, datamodel.Type):
-                        base_type = type_elem.base.id
-                    else:
-                        base_type = str(type_elem.base)
-                    elem_tag = etree.SubElement(type_list_tag, "type",
-                                                {'id': type_elem.id, 'name': type_elem.name,
-                                                 'alias': type_elem.alias,
-                                                 'base': base_type})
-
-                    # _described_item_list_tag = etree.SubElement(elem_tag, "describedItemList")
-
-        self.write()
-
-
-derived_obj_tag = ("physicalInterface",
-                   "physicalElement",
-                   "function",
-                   "functionalElement",
-                   "functionalInterface")
-
-
-def get_object_tag(wanted_object):
-    """Get xml element tag corresponding to wanted_object"""
-    elem_tag = None
-    if isinstance(wanted_object, datamodel.PhysicalInterface):
-        elem_tag = "physicalInterface"
-    elif isinstance(wanted_object, datamodel.PhysicalElement):
-        elem_tag = "physicalElement"
-    elif isinstance(wanted_object, datamodel.Function):
-        elem_tag = "function"
-    elif isinstance(wanted_object, datamodel.FunctionalElement):
-        elem_tag = "functionalElement"
-    elif isinstance(wanted_object, datamodel.FunctionalInterface):
-        elem_tag = "functionalInterface"
-    elif isinstance(wanted_object, datamodel.Attribute):
-        elem_tag = "attribute"
-    elif isinstance(wanted_object, datamodel.Transition):
-        elem_tag = "transition"
-    elif isinstance(wanted_object, datamodel.State):
-        elem_tag = "state"
-    elif isinstance(wanted_object, datamodel.Data):
-        elem_tag = "data"
-    elif isinstance(wanted_object, datamodel.View):
-        elem_tag = "view"
-    elif isinstance(wanted_object, datamodel.Type):
-        elem_tag = "type"
-    return elem_tag
-
-
-def get_allocation_tag(wanted_object):
-    """Get xml allocation tag corresponding to wanted_object"""
-    elem_tag = None
-    if isinstance(wanted_object, datamodel.Function):
-        elem_tag = "allocatedFunction"
-    elif isinstance(wanted_object, datamodel.FunctionalElement):
-        elem_tag = "allocatedFunctionalElement"
-    elif isinstance(wanted_object, datamodel.FunctionalInterface):
-        elem_tag = "allocatedFunctionalInterface"
-    elif isinstance(wanted_object, datamodel.State):
-        elem_tag = "allocatedState"
-    elif isinstance(wanted_object, datamodel.Data):
-        elem_tag = "allocatedData"
-    elif isinstance(wanted_object, datamodel.View):
-        elem_tag = "allocatedItem"
-    return elem_tag
+        """Write type element from list of types
+        @param[in] type_list : list of types
+        @return None
+        """
+        parser = etree.XMLParser(remove_blank_text=True)
+        root = self.tree.parse(self.file, parser)
+
+        if root.find('.//typeList') is None:
+            etree.SubElement(root.find('./viewPoint'), 'typeList')
+
+        for type_list_tag in root.findall(".//typeList"):
+            for type_elem in type_list:
+                _elem_tag = etree.SubElement(type_list_tag, "type",
+                                             {'id': type_elem.id,
+                                              'name': type_elem.name,
+                                              'alias': type_elem.alias,
+                                              'base': self.check_object_type(type_elem.base)})
+
+        self.tree.write(self.file, encoding='utf-8', xml_declaration=True, pretty_print=True)
```

### Comparing `jarvis4se-1.3.4/tests/test_magic_tools.py` & `jarvis4se-1.3.5/tests/test_magic_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,45 @@
-"""Test module for tools pkg i.e. MagicTools"""
-from IPython import get_ipython
+"""@defgroup test_magic_tools
+Tests about Jarvis IPython magic tools
+"""
+# Libraries
 
-import jarvis
 
-ip = get_ipython()
-generator = jarvis.PlantUmlGen()
-my_magic = jarvis.MagicTools(ip, generator)
+# Modules
+import test_lib
 
+# Initialisation of Jarvis
+jarvis4se_all = test_lib.get_jarvis4se()
+generator = jarvis4se_all[1]
+jarvis4se_tool = jarvis4se_all[2]
 
-def test_retrieve_pkg_version(capsys):
-    """Notebook equivalent:
-    %retrieve_pkg_version
+
+def test_retrieve_pkg_version_tool(capsys):
+    """@ingroup test_magic_tools
+    Test the magic line "%retrieve_pkg_version"
+
+    @param[in] capsys : capture fixture reference
+    @return None
     """
-    my_magic.retrieve_pkg_version('')
+    jarvis4se_tool.retrieve_pkg_version('')
     captured = capsys.readouterr()
     expected = ["lxml==", "notebook==", "plantuml==", "jarvis4se==", "pandas==", "python=="]
     assert all(i in captured.out for i in expected)
 
 
-def test_diagram_cell(capsys, mocker):
-    """Notebook equivalent:
-    %%diagram
-    @startuml
-    !define Junction_Or circle #black
-    !define Junction_And circle #whitesmoke
-
-    Junction_And JunctionAnd
-    Junction_Or JunctionOr
-
-    archimate #Technology "VPN Server" as vpnServerA <<technology-device>>
-
-    rectangle GO #lightgreen
-    rectangle STOP #red
-    rectangle WAIT #orange
-    GO -up-> JunctionOr
-    STOP -up-> JunctionOr
-    STOP -down-> JunctionAnd
-    WAIT -down-> JunctionAnd
-    @enduml
+def test_diagram_cell_tool(capsys, mocker):
+    """@ingroup test_magic_tools
+    Test the magic cell "%%diagram"
+
+    @param[in] capsys : capture fixture reference
+    @param[in] mocker : mocker fixture reference
+    @return None
     """
     spy = mocker.spy(generator, "get_diagram_url")
-    my_magic.diagram('', "@startuml\n"
+    jarvis4se_tool.diagram('', "@startuml\n"
                          "!define Junction_Or circle #black\n"
                          "!define Junction_And circle #whitesmoke\n"
                          "\n"
                          "\n"
                          "Junction_And JunctionAnd\n"
                          "Junction_Or JunctionOr\n"
                          "\n"
```

