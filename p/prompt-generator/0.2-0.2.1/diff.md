# Comparing `tmp/prompt-generator-0.2.tar.gz` & `tmp/prompt-generator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt-generator-0.2.tar", last modified: Sat May 20 00:05:29 2023, max compression
+gzip compressed data, was "prompt-generator-0.2.1.tar", last modified: Sun May 21 18:32:12 2023, max compression
```

## Comparing `prompt-generator-0.2.tar` & `prompt-generator-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:05:29.975597 prompt-generator-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-20 00:05:09.000000 prompt-generator-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-20 00:05:29.975597 prompt-generator-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-20 00:05:09.000000 prompt-generator-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-20 00:05:09.000000 prompt-generator-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 00:05:29.975597 prompt-generator-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:05:29.971597 prompt-generator-0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:05:29.971597 prompt-generator-0.2/src/markdown_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-20 00:05:09.000000 prompt-generator-0.2/src/markdown_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-20 00:05:09.000000 prompt-generator-0.2/src/markdown_parser/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:05:29.975597 prompt-generator-0.2/src/prompt_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-20 00:05:29.000000 prompt-generator-0.2/src/prompt_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-20 00:05:29.000000 prompt-generator-0.2/src/prompt_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:05:29.000000 prompt-generator-0.2/src/prompt_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-20 00:05:29.000000 prompt-generator-0.2/src/prompt_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-20 00:05:29.000000 prompt-generator-0.2/src/prompt_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-20 00:05:29.000000 prompt-generator-0.2/src/prompt_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:32:12.002254 prompt-generator-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-21 18:32:11.998254 prompt-generator-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 18:32:12.002254 prompt-generator-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:32:11.998254 prompt-generator-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:32:11.998254 prompt-generator-0.2.1/src/directory_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/directory_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/directory_structure/get_directory_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:32:11.998254 prompt-generator-0.2.1/src/markdown_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/markdown_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/markdown_parser/parse_md.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:32:11.998254 prompt-generator-0.2.1/src/print_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/print_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/print_utils/print_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-21 18:32:00.000000 prompt-generator-0.2.1/src/print_utils/print_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 18:32:11.998254 prompt-generator-0.2.1/src/prompt_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-21 18:32:11.000000 prompt-generator-0.2.1/src/prompt_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-21 18:32:11.000000 prompt-generator-0.2.1/src/prompt_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 18:32:11.000000 prompt-generator-0.2.1/src/prompt_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-21 18:32:11.000000 prompt-generator-0.2.1/src/prompt_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 18:32:11.000000 prompt-generator-0.2.1/src/prompt_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-21 18:32:11.000000 prompt-generator-0.2.1/src/prompt_generator.egg-info/top_level.txt
```

### Comparing `prompt-generator-0.2/LICENSE` & `prompt-generator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prompt-generator-0.2/pyproject.toml` & `prompt-generator-0.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "prompt-generator"
-version = "0.2"
-description = "Prompt Generator is a flexible and user-friendly package that offers customizable scripts for generating meaningful and context-aware prompts. These prompts can be used to guide the writing, enhancement, and debugging of code."
+version = "0.2.1"
+description = "Prompt Generator is a flexible and user-friendly package that offers customizable scripts for generating effective and context-aware prompts. These prompts can be used to guide the writing, improvement, and debugging of code."
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
-    {name = "Vincenzo Cascone"},
+    { name = "Vincenzo Cascone" },
 ]
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "pyperclip",
+    "pathspec",
 ]
 
 [project.scripts]
 parse_md = "markdown_parser:main"
+get_directory_structure = "directory_structure:main"
 
 [project.urls]
 repository = "https://github.com/vincenzocascone/prompt-generator"
```

