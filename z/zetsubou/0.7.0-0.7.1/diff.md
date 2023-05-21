# Comparing `tmp/zetsubou-0.7.0.tar.gz` & `tmp/zetsubou-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zetsubou-0.7.0.tar", last modified: Sat May  6 10:40:26 2023, max compression
+gzip compressed data, was "zetsubou-0.7.1.tar", last modified: Sun May 21 10:56:19 2023, max compression
```

## Comparing `zetsubou-0.7.0.tar` & `zetsubou-0.7.1.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.097418 zetsubou-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-06 10:40:26.097418 zetsubou-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-06 10:40:10.000000 zetsubou-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-06 10:40:10.000000 zetsubou-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 10:40:26.097418 zetsubou-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-06 10:40:10.000000 zetsubou-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.085418 zetsubou-0.7.0/zetsubou/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.089418 zetsubou-0.7.0/zetsubou/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/base_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/clean_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/command_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/command_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/execute_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/commands/regen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.089418 zetsubou-0.7.0/zetsubou/conan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/conan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/conan/conan.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/conan/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/conan/deployer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/conan/from_conan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/conan/to_conan.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.089418 zetsubou-0.7.0/zetsubou/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.089418 zetsubou-0.7.0/zetsubou/data/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/data/rules/ClangRules.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/data/rules/MsvcRules.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.093418 zetsubou-0.7.0/zetsubou/fastbuild/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    54351 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/fastbuild_emit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/target_kinds.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/to_fastbuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/vcxproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/fastbuild/vssolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/logo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.093418 zetsubou-0.7.0/zetsubou/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/base_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/config_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.093418 zetsubou-0.7.0/zetsubou/project/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/cli_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/config_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/configuration_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/platform_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/project_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/runtime_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/toolchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/toolchain_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/toolchain_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/model/virtual_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.097418 zetsubou-0.7.0/zetsubou/project/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/runtime/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/runtime/project_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13274 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/runtime/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/project/runtime/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.097418 zetsubou-0.7.0/zetsubou/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/discover_toolchains.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.097418 zetsubou-0.7.0/zetsubou/system/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/windows/msvc.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/windows/vswhere.py
--rw-r--r--   0 runner    (1001) docker     (123)    18517 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/system/windows/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.097418 zetsubou-0.7.0/zetsubou/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/busy_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/cmd_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/dataclass_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/json_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/yaml_simple_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/utils/yaml_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/zetsubou.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-06 10:40:10.000000 zetsubou-0.7.0/zetsubou/zetsubou_conan_toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:40:26.085418 zetsubou-0.7.0/zetsubou.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-06 10:40:26.000000 zetsubou-0.7.0/zetsubou.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-06 10:40:26.000000 zetsubou-0.7.0/zetsubou.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 10:40:26.000000 zetsubou-0.7.0/zetsubou.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 10:40:26.000000 zetsubou-0.7.0/zetsubou.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-06 10:40:26.000000 zetsubou-0.7.0/zetsubou.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 10:40:26.000000 zetsubou-0.7.0/zetsubou.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.568208 zetsubou-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-21 10:56:19.568208 zetsubou-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-21 10:55:59.000000 zetsubou-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-21 10:55:59.000000 zetsubou-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 10:56:19.568208 zetsubou-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-21 10:55:59.000000 zetsubou-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.552207 zetsubou-0.7.1/zetsubou/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.556208 zetsubou-0.7.1/zetsubou/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/commands/base_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/commands/clean_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/commands/command_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/commands/command_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/commands/execute_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/commands/regen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.556208 zetsubou-0.7.1/zetsubou/conan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/conan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/conan/conan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/conan/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/conan/deployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/conan/from_conan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/conan/to_conan.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.560208 zetsubou-0.7.1/zetsubou/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.560208 zetsubou-0.7.1/zetsubou/data/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/data/rules/ClangRules.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/data/rules/MsvcRules.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.560208 zetsubou-0.7.1/zetsubou/fastbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/fastbuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/fastbuild/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56198 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/fastbuild/fastbuild_emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/fastbuild/target_kinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/fastbuild/to_fastbuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/fastbuild/vcxproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/fastbuild/vssolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/logo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.560208 zetsubou-0.7.1/zetsubou/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/base_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/config_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.564208 zetsubou-0.7.1/zetsubou/project/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/cli_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/config_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/configuration_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/platform_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/project_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/runtime_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/toolchain_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/toolchain_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/model/virtual_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.564208 zetsubou-0.7.1/zetsubou/project/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/runtime/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/runtime/project_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13991 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/runtime/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/project/runtime/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.564208 zetsubou-0.7.1/zetsubou/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/system/discover_toolchains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/system/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.564208 zetsubou-0.7.1/zetsubou/system/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/system/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/system/windows/msvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/system/windows/vswhere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18517 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/system/windows/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.568208 zetsubou-0.7.1/zetsubou/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/busy_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/cmd_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/dataclass_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/json_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/yaml_simple_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/utils/yaml_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/zetsubou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-05-21 10:55:59.000000 zetsubou-0.7.1/zetsubou/zetsubou_conan_toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:56:19.556208 zetsubou-0.7.1/zetsubou.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-21 10:56:19.000000 zetsubou-0.7.1/zetsubou.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-21 10:56:19.000000 zetsubou-0.7.1/zetsubou.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 10:56:19.000000 zetsubou-0.7.1/zetsubou.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-21 10:56:19.000000 zetsubou-0.7.1/zetsubou.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-21 10:56:19.000000 zetsubou-0.7.1/zetsubou.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 10:56:19.000000 zetsubou-0.7.1/zetsubou.egg-info/top_level.txt
```

### Comparing `zetsubou-0.7.0/PKG-INFO` & `zetsubou-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zetsubou
-Version: 0.7.0
+Version: 0.7.1
 Summary: FASTbuild generator for the helpless
 Author: BentouDev
 Project-URL: Homepage, https://github.com/BentouDev/Zetsubou
 Keywords: fastbuild,C++,cpp,C/C++,developer,tool
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zetsubou-0.7.0/README.md` & `zetsubou-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/pyproject.toml` & `zetsubou-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = [ 'zetsubou*' ]
 
 [tool.setuptools.package-data]
 'zetsubou.data.rules' = ["*.yml"]
 
 [project]
 name = "zetsubou"
-version = "0.7.0"
+version = "0.7.1"
 description = "FASTbuild generator for the helpless"
 readme = "README.md"
 authors = [{ name = "BentouDev" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -40,15 +40,15 @@
 [project.urls]
 Homepage = "https://github.com/BentouDev/Zetsubou"
 
 [project.scripts]
 zetsubou = "zetsubou.zetsubou:main"
 
 [tool.bumpver]
-current_version = "0.7.0"
+current_version = "0.7.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[bot] Bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `zetsubou-0.7.0/zetsubou/__main__.py` & `zetsubou-0.7.1/zetsubou/__main__.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/commands/base_command.py` & `zetsubou-0.7.1/zetsubou/commands/base_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,29 +81,33 @@
         raise NotImplementedError()
 
     def _load_project(self, context : CommandContext):
         if context.project_template is None:
 
             logger.Command('load_project')
 
+            if not context.file_cache.load(context.project_fs):
+                logger.Info('Stale cache, will regenerate')
+
             external_config = ExternalConfig()
 
             # handle platform from external file
             if hasattr(context.command_args, 'profile') and context.command_args.profile is not None:
                 profile_file = os.path.relpath(context.command_args.profile, context.fs_root) if os.path.isabs(context.command_args.profile) else context.command_args.profile
                 external_config.profile_file = fix_path(profile_file)
 
                 logger.Info(f"Using profile from external file '{external_config.profile_file}'")
 
             # load and process project
             context.project_template = execute_stage(lambda: load_project_from_file(
                                         context.project_fs,
                                         context.fs_root,
                                         context.project_file,
-                                        external_config=external_config),
+                                        external_config=external_config,
+                                        file_cache=context.file_cache),
                                         'Project loaded',
                                         EErrorCode.UNABLE_TO_LOAD_PROJECT)
 
             context.project_template.platforms = tools.filter_platforms_by_host(
                 context.host_system,
                 context.host_arch,
                 context.project_template.platforms)
```

### Comparing `zetsubou-0.7.0/zetsubou/commands/build.py` & `zetsubou-0.7.1/zetsubou/commands/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from argparse import ArgumentParser
 from zetsubou.commands.base_command import Command
 from zetsubou.commands.command_context import CommandContext
+from zetsubou.commands.generate import Generate
+from zetsubou.commands.install import Install
 from zetsubou.fastbuild.fastbuild_emit import FastbuildEmitter
 from zetsubou.project.model.config_string import EDefaultConfigSlots
 from zetsubou.project.model.kind import ETargetKind
 from zetsubou.project.runtime.emit import EDefaultTargets, EmitContext
 from zetsubou.project.runtime.project_loader import ProjectTemplate
 from zetsubou.utils import logger
 from zetsubou.utils.common import null_or_empty
@@ -15,15 +17,15 @@
 class Build(Command):
     @property
     def name(self):
         return 'build'
 
     @property
     def desc(self):
-        return 'Builds specified target for specified or all configs.'
+        return 'Builds specified target for specified or all configs. Triggers Install and Generate if user changes were detected since last run.'
 
     @property
     def help(self):
         return self.desc
 
     def ParseArgs(self, arg_parser: ArgumentParser):
         config_or_variant = arg_parser.add_mutually_exclusive_group()
@@ -58,15 +60,20 @@
         build_target = context.project_template.find_target(arg_target)
         if build_target is None:
             raise ProjectError(f"Unknown target '{arg_target}'")
 
         return context.project_template.compile_target_variant_name(build_target.config.kind, build_target.target)
 
     def OnExecute(self, context: CommandContext):
-        context.resolve_venv()
+        if context.file_cache.is_stale():
+            Command.get_command_instance(Install).Execute(context)
+            Command.get_command_instance(Generate).Execute(context)
+        else:
+            # Already done by the above, if cache is fresh, we just find the venv
+            context.resolve_venv()
 
         try:
             arg_target = context.command_args.target
             arg_config = context.command_args.config
             arg_variant = context.command_args.target_variant
 
             target_variants = []
```

### Comparing `zetsubou-0.7.0/zetsubou/commands/clean.py` & `zetsubou-0.7.1/zetsubou/commands/clean.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/commands/clean_build.py` & `zetsubou-0.7.1/zetsubou/commands/clean_build.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/commands/command_context.py` & `zetsubou-0.7.1/zetsubou/commands/command_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from zetsubou.project.config_matrix import ConfigMatrix
 from zetsubou.project.base_context import BaseContext
 from zetsubou.project.model.target import Target
 from zetsubou.project.model.virtual_environment import VirtualEnvironment, resolve_venv
 from zetsubou.project.runtime.resolve import ResolvedTarget
 from zetsubou.project.runtime.project_loader import ProjectTemplate
 from zetsubou.utils.error_codes import EErrorCode
+from zetsubou.utils.file_cache import FileCache
 
 @dataclass
 class Fastbuild:
     emit_fs : FS
     bff_dir : str
     bff_file : str
 
@@ -34,14 +35,19 @@
 
     project_template: Optional[ProjectTemplate] = None
     # toolchains: List[ToolchainDefinition] = field(default_factory=list)
     config_matrix: Optional[ConfigMatrix] = None
     resolved_targets: List[ResolvedTarget] = field(default_factory=list)
     fastbuild: Optional[Fastbuild] = None
     conan: Conan = field(default_factory=Conan)
+    file_cache: FileCache = field(default_factory=FileCache)
+
+    def cache_file(self, filename:str):
+        if self.file_cache:
+            self.file_cache.add_file(filename)
 
     def to_out_path(self, path : str):
         return fix_path(os.path.join(self.fs_root, path))
 
     def resolve_cli_tools(self):
         for cli_tool in self.project_template.cli_tools:
             if not cli_tool.resolve(self.fs_venv):
```

### Comparing `zetsubou-0.7.0/zetsubou/commands/command_registry.py` & `zetsubou-0.7.1/zetsubou/commands/command_registry.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/commands/config.py` & `zetsubou-0.7.1/zetsubou/commands/config.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/commands/create.py` & `zetsubou-0.7.1/zetsubou/commands/create.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/commands/execute_stage.py` & `zetsubou-0.7.1/zetsubou/commands/execute_stage.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/commands/generate.py` & `zetsubou-0.7.1/zetsubou/commands/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from argparse import ArgumentParser
 import os
 from fs.base import FS
 from fs.copy import copy_fs
 from zetsubou.commands.base_command import Command
 from zetsubou.commands.command_context import CommandContext, Fastbuild
 from zetsubou.commands.execute_stage import execute_stage
-from zetsubou.commands.install import Install
+from zetsubou.commands.install import CONAN_DEPS_FILE, Install
 from zetsubou.conan.dependencies import ConanDependencies
 from zetsubou.fastbuild.fastbuild_emit import FastbuildEmitter
 from zetsubou.project.model.target import Target
 from zetsubou.project.model.virtual_environment import VirtualEnvironment
 from zetsubou.project.runtime.emit import EmitContext, emit_project
 from zetsubou.project.runtime.project_loader import load_dataclass_list
 from zetsubou.project.runtime.resolve import ResolveContext, resolve_target_variants
@@ -90,28 +90,30 @@
 def load_dependencies(context: CommandContext):
     loader = YAMLLoader()
     local_types = base.get_types_from_modules([__name__, 'zetsubou.project.model.target'])
     dep_targets = []
 
     conan_deps = context.project_template.project.conan.dependencies
     if conan_deps is None:
-        return
+        return True
 
     conan_deps = context.to_out_path(conan_deps)
 
     def load_deps():
-        path = 'build/conan_deps.yml'
+        path = CONAN_DEPS_FILE
 
         # Merge files, only parts from deployer exist
         if not context.project_fs.exists(path):
             Command.get_command_instance(Install).merge_generated_part_files(context, conan_deps)
             return True
 
         # Load merged yaml
         with context.project_fs.open(path, 'r', encoding='utf-8') as obj_file:
+            context.cache_file(path)
+
             obj_templ : ConanDependencies = loader.load_dataclass(ConanDependencies, path, obj_file.read(), local_types)
 
             if obj_templ is None:
                 return False
 
             context.conan.yml_files = obj_templ.targets
 
@@ -120,15 +122,15 @@
     if len(context.conan.yml_files) == 0:
         if not load_deps():
             return False
 
     dep_targets = context.conan.yml_files
 
     if len(dep_targets) != 0:
-        context.conan.dependencies = load_dataclass_list(Target, dep_targets, '', context.project_fs, loader, local_types)
+        context.conan.dependencies = load_dataclass_list(Target, dep_targets, '', context.project_fs, loader, local_types, context.file_cache)
 
     return True
 
 
 def validate_project(context: CommandContext):
     vctx = ValidationContext()
     vctx.error_format = base.EErrorFormat.MSVC if context.command_args.ide else base.EErrorFormat.Pretty
```

### Comparing `zetsubou-0.7.0/zetsubou/commands/install.py` & `zetsubou-0.7.1/zetsubou/commands/install.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from zetsubou.utils.yaml_tools import to_yaml
 from zetsubou.conan.conan import check_conan_present, call_conan
 from zetsubou.conan.to_conan import runtime_to_conan, toolchain_to_conan, platform_to_conan, config_base_to_conan
 from zetsubou.conan.deployer import get_conan_deployer_path
 
 
 CONAN_OUT_PATH = 'build/conan'
+CONAN_DEPS_FILE = 'build/conan_deps.yml'
 
 
 class Install(Command):
     @property
     def name(self):
         return 'install'
 
@@ -30,14 +31,19 @@
     def help(self):
         return self.desc
 
     def ParseArgs(self, arg_parser: ArgumentParser):
         pass
 
     def OnExecute(self, context: CommandContext):
+        if (is_conanfile_fresh(context, context.project_template.project.conan.build_tools) and
+            is_conanfile_fresh(context, context.project_template.project.conan.dependencies) and
+            is_conanfile_fresh(context, CONAN_DEPS_FILE)):
+            return
+
         context.project_fs.makedirs('build/venv', recreate=True)
 
         if context.project_template.project.conan is not None and check_conan_present():
             self.generate_conan_environment(context)
         else:
             generate_empty_environment(context.project_fs)
 
@@ -75,35 +81,38 @@
 
             with context.project_fs.open(out_yml_path, mode='w') as out_file:
                 out_file.write(''.join(dep_content))
 
         # Merge targets into one file
         if len(out_ymls) > 0:
 
-            with context.project_fs.open('build/conan_deps.yml', mode='w') as out_file:
+            with context.project_fs.open(CONAN_DEPS_FILE, mode='w') as out_file:
                 conan_deps = ConanDependencies(conanfile=conan_deps, targets=out_ymls)
                 out_file.write(to_yaml(conan_deps))
 
+            context.cache_file(CONAN_DEPS_FILE)
             context.conan.yml_files = out_ymls
 
     def generate_conan_environment(self, context: CommandContext):
         conan_build_tools = context.project_template.project.conan.build_tools
         if conan_build_tools is not None:
+            context.cache_file(conan_build_tools)
             conan_build_tools = context.to_out_path(conan_build_tools)
             conan_out_directory = context.to_out_path("build/venv")
             execute_stage(lambda: call_conan(['install', conan_build_tools, '-g=VirtualBuildEnv', f'-of={conan_out_directory}'], conan_out_directory),
                         'Conan build tools installed',
                         EErrorCode.UNABLE_TO_INSTALL_CONAN_BUILD_TOOLS)
 
             context.resolve_venv()
 
         conan_deps = context.project_template.project.conan.dependencies
         if conan_deps is None:
             return
 
+        context.cache_file(conan_deps)
         conan_deps = context.to_out_path(conan_deps)
 
         for config_variant in context.config_matrix.variants:
             logger.Verbose(f"Installing configuration '{config_variant.config_string}'")
 
             plat_name = config_variant.get_slot('platform')
             platform = context.project_template.find_platform(plat_name)
@@ -131,7 +140,13 @@
             execute_stage(lambda: call_conan(conan_call_args + conan_settings,
                         context.to_out_path(conan_config_out_path),
                         context.fs_venv),
                         f"Conan configuration '{config_variant.config_string}' installed",
                         EErrorCode.UNABLE_TO_INSTALL_CONAN_DEPENDENCIES)
 
         self.merge_generated_part_files(context, conan_deps)
+
+
+def is_conanfile_fresh(context:CommandContext, filename:str):
+    if filename == '' or filename is None:
+        return True
+    return context.file_cache.is_fresh(filename)
```

### Comparing `zetsubou-0.7.0/zetsubou/commands/regen.py` & `zetsubou-0.7.1/zetsubou/commands/regen.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/conan/conan.py` & `zetsubou-0.7.1/zetsubou/conan/conan.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/conan/deployer.py` & `zetsubou-0.7.1/zetsubou/conan/deployer.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/conan/from_conan.py` & `zetsubou-0.7.1/zetsubou/conan/from_conan.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/conan/to_conan.py` & `zetsubou-0.7.1/zetsubou/conan/to_conan.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/data/rules/ClangRules.yml` & `zetsubou-0.7.1/zetsubou/data/rules/ClangRules.yml`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/data/rules/MsvcRules.yml` & `zetsubou-0.7.1/zetsubou/data/rules/MsvcRules.yml`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/fastbuild/compiler.py` & `zetsubou-0.7.1/zetsubou/fastbuild/compiler.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/fastbuild/fastbuild_emit.py` & `zetsubou-0.7.1/zetsubou/fastbuild/fastbuild_emit.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 import fs
 from pathlib import Path
 
 from dataclasses import dataclass, is_dataclass, fields
 from enum import Enum
 from inspect import isclass
 from typing import Optional, List, Any, Set, Callable, Tuple, Generic, TypeVar
-from typing_inspect import get_origin, is_optional_type
+from typing_inspect import is_optional_type
+from bentoudev.dataclass.base import is_clazz_list, is_clazz_dict
 from zetsubou.fastbuild.to_fastbuild import compiler_family_to_fastbuild
 
 from zetsubou.project.config_matrix import ConfigVariant, get_config_matrix_os_name
 from zetsubou.project.model.config_string import EDefaultConfigSlots
 from zetsubou.project.model.configuration import Configuration
 from zetsubou.project.runtime.emit import EDefaultTargets, Emitter, EmitContext
 from zetsubou.project.runtime.project_loader import ProjectTemplate
 from zetsubou.project.runtime.resolve import ResolvedTarget, TargetVariant
 from zetsubou.project.model.target import Target, TargetReference, Source
 from zetsubou.project.model.kind import ETargetKind, is_target_kind_linkable, is_target_library, is_target_prebuild_step
 from zetsubou.project.model.toolchain import Toolchain, ToolchainDefinition
-from zetsubou.utils.common import join_unique, list_to_string, split, filter_none
+from zetsubou.utils.common import join_unique, list_to_string, split
 
 import zetsubou.fastbuild.target_kinds as target_kinds
 import zetsubou.fastbuild.vcxproject as vcxproject
 import zetsubou.fastbuild.vssolution as vssolution
 from zetsubou.fastbuild.compiler import Compiler
 from zetsubou.system.windows.msvc import arch_to_msvc_platform
-from zetsubou.utils.subprocess import call_process_venv
 
 
 FASTBUILD_BFF_HEADER = '// Generated by Zetsubou, do not manually edit!'
 FASTBUILD_ALL_TARGET = 'AllTargets'
 PROJ_OUTPUT_DIR = '^$(SolutionDir)/build'
 FBUILD_OUTPUT_DIR = 'build/fbuild'
 DEFAULT_INDENT = 4
@@ -98,16 +98,15 @@
             return False
         if bff_writer.is_list(obj):
             return len(obj) == 0
         return obj is None
 
     @staticmethod
     def is_list(obj) -> bool:
-        t = type(obj)
-        return t == list or get_origin(t) == list
+        return is_clazz_list(type(obj))
 
     @staticmethod
     def is_single_value(obj) -> bool:
         t = type(obj)
         if bff_writer.is_list(obj):
             return False
         if t == TargetReference:
@@ -471,15 +470,16 @@
         proj_path = fs.path.join(context.ROOT_DIR, project_subdir)
         abs_out_path = fs.path.join(context.fs_root, proj_path)
         result = fs.path.relativefrom(abs_out_path, abs_dir_path)
         return result
 
 
     def get_target_output_path(self, context : EmitContext, target: ResolvedTarget):
-        return self.project_to_output_path(context, fs.path.dirname(target.target.get_loaded_from_file()))
+        path = self.project_to_output_path(context, fs.path.dirname(target.target.get_loaded_from_file()))
+        return path if path != '' else '.'
 
 
     def get_bin_output_path(self, config_name : str):
         return f'{PROJ_OUTPUT_DIR}/obj/{config_name}'
 
 
     def get_compiler_output_path(self, config_str : str, subdir : str):
@@ -545,14 +545,27 @@
 
 
     @staticmethod
     def get_zetsubout_update_rebuild_command(context: EmitContext):
         return f'zetsubou regen {context.project_file} --ide --nologo'
 
 
+    # Reference only to matching variant of other targets
+    @staticmethod
+    def map_target_ref_to_str(ref, target_variant: TargetVariant):
+        if isinstance(ref, TargetReference):
+            return ProjectTemplate.compile_target_variant_name(ref.target.config.kind, ref.name, target_variant.config_variant.config_string)
+        return ref
+
+
+    @staticmethod
+    def map_target_references_to_variant(refs, target_variant:TargetVariant):
+        return list(map(lambda r: FastbuildEmitter.map_target_ref_to_str(r, target_variant), refs))
+
+
     # Formats path containing {root} and {config_variant} like so:
     # {root}/mydir -> C:\Projects\MyProject\mydir
     # build/generated/{config_variant} -> build/generated/Windows_Debug_MSVC_x64_v193_v143
     @staticmethod
     def format_path(format_path:str, context:EmitContext, config_variant:ConfigVariant):
         return format_path.format(root=context.fs_root, config_variant=get_config_matrix_os_name(config_variant.config_string))
 
@@ -601,26 +614,22 @@
         ])
 
         def filter_target_ref(ref):
             return isinstance(ref, TargetReference)
 
         refs, libs = split(filter_target_ref, link_libs_with_refs)
 
-        # Linking only to matching variant of other targets
-        def map_target_ref_to_str(ref):
-            if isinstance(ref, TargetReference):
-                return ProjectTemplate.compile_target_variant_name(ref.target.config.kind, ref.name, target_variant.config_variant.config_string)
-            return ref
-
-        fbuild.Libraries = list(map(map_target_ref_to_str, filter(filter_target_linkable, refs)))
+        fbuild.Libraries = FastbuildEmitter.map_target_references_to_variant(filter(filter_target_linkable, refs), target_variant)
         fbuild.LinkerOptions += list_to_string( [ toolchain.definition.i_linker.link(l) for l in libs ])
         fbuild.LinkerOptions += list_to_string( [ toolchain.definition.i_linker.dir(l)  for l in lib_paths ])
 
         # Depend on copying distributed files to bin
-        fbuild.PreBuildDependencies = [ FastbuildEmitter.get_copy_distributed_files_target_name(target_variant.config_variant.config_string) ]
+        fbuild.PreBuildDependencies = [
+            FastbuildEmitter.get_copy_distributed_files_target_name(target_variant.config_variant.config_string)
+        ] + FastbuildEmitter.map_target_references_to_variant(target_variant.build_require, target_variant)
 
 
     def compiler_relative_path(self, context : EmitContext, path : str, target : ResolvedTarget, target_variant : TargetVariant):
         formatted_path = self.format_path(path, context, target_variant.config_variant)
         if not os.path.isabs(formatted_path):
             return fs.path.join( fs.path.dirname(target.target.get_loaded_from_file()), formatted_path)
         else:
@@ -651,26 +660,28 @@
 
         excluded_paths = list(map(lambda p: self.compiler_relative_path(context, p, target, target_variant), target_variant.source_exclude.paths))
 
         fbuild.CompilerInputPath = out_path
         fbuild.CompilerInputPattern = target_variant.source.patterns
         fbuild.CompilerInputExcludePath = excluded_paths
         fbuild.CompilerInputExcludePattern = target_variant.source_exclude.patterns
+        fbuild.PreBuildDependencies = FastbuildEmitter.map_target_references_to_variant(target_variant.build_require, target_variant)
 
 
     def fill_library(self, context : EmitContext, fbuild : target_kinds.StaticLibTarget, target: ResolvedTarget, target_variant: TargetVariant, root_dir : str, toolchain : Toolchain):
         # self.fill_object(context, fbuild, target, target_variant, root_dir, toolchain)
         fbuild.CompilerOutputPath = self.get_compiler_output_path(target_variant.config_variant.config_string, 'obj')
 
         fbuild.LibrarianOptions = list_to_string(join_unique([
             target_variant.librarian_flags.public,
             target_variant.librarian_flags.private
         ]))
 
         fbuild.LibrarianOutput = f'{self.get_compiler_output_path(target_variant.config_variant.config_string, "lib")}/{target.target.target}.lib'
+        fbuild.PreBuildDependencies = FastbuildEmitter.map_target_references_to_variant(target_variant.build_require, target_variant)
 
 
     def emit_vcxproj(self, writer : bff_writer, vcxproj : vcxproject.VCXProject, project_configs_list : str, includes : List[str]):
         # Conflig list predefine
         writer.newline()
         write_field(writer, project_configs_list, [])
 
@@ -1238,32 +1249,58 @@
                     substruct.write_field('Projects', all_projects)
                     substruct.write_field('Dependencies', [all_target_proj])
 
                 min_ver, max_ver = get_min_max_msvc_version(context, context.project_template)
                 struct.write_field('SolutionVisualStudioVersion', max_ver)
                 struct.write_field('SolutionMinimumVisualStudioVersion', min_ver)
 
-                # Folders
                 folders = []
+                current_path = []
+
+                # Fastbuild wants subfolders to be specified by just the path with / delimeters
+                def build_folder_list(data):
+                    this_type = type(data)
+                    if is_clazz_dict(this_type):
+                        for key, value in data.items():
+                            current_path.append(key)
+                            build_folder_list(value)
+                            current_path.pop()
+                    if is_clazz_list(this_type):
+                        if len(current_path) != 0:
+                            # Swap path to file into a fastbuild project reference
+                            folders.append((
+                                '/'.join(current_path),
+                                current_path[-1],
+                                [ f'{target.target}-proj' for target in map(context.project_template.find_target_by_file, data) ]
+                            ))
+
+                build_folder_list(context.project_template.project.targets)
+
+                # Folders
+                solution_folders = []
                 def add_folder(name : str, title : str, targets : List[str]):
-                    folders.append(f'.{name}')
+                    solution_folders.append(f'.{name}')
                     writer.newline()
                     write_assign(writer, name)
                     with bff_struct(writer) as commands:
                         commands.write_field('Path', title)
                         commands.write_field('Projects', targets)
 
                 writer.newline()
-                add_folder('Folder_Commands', '0. Commands', default_targets)
-                add_folder('Folder_Conan', '1. Dependencies', [ f'{target.target}-proj' for target in context.conan.dependencies ])
-                add_folder('Folder_Libraries', '2. Libraries', [ f'{target.target}-proj' for target in filter(filter_target_libraries, context.project_template.targets) ])
-                add_folder('Folder_Apps', '3. Apps', [ f'{target.target}-proj' for target in filter(filter_target_executable, context.project_template.targets) ])
+                add_folder('Folder_Commands', 'commands', default_targets)
+                add_folder('Folder_Conan', 'dependencies', [ f'{target.target}-proj' for target in context.conan.dependencies ])
+
+                for path, name, data in folders:
+                    add_folder(name, path, data)
+
+                #add_folder('Folder_Libraries', '2. Libraries', [ f'{target.target}-proj' for target in filter(filter_target_libraries, context.project_template.targets) ])
+                #add_folder('Folder_Apps', '3. Apps', [ f'{target.target}-proj' for target in filter(filter_target_executable, context.project_template.targets) ])
 
                 writer.newline()
-                write_field(writer, 'SolutionFolders', folders, no_quotations=True)
+                write_field(writer, 'SolutionFolders', solution_folders, no_quotations=True)
 
             context.write_file(self.main_file_name, writer.to_string())
 
         self.emit_runner_script(context)
 
         return self.main_file_name
```

### Comparing `zetsubou-0.7.0/zetsubou/fastbuild/target_kinds.py` & `zetsubou-0.7.1/zetsubou/fastbuild/target_kinds.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/fastbuild/vcxproject.py` & `zetsubou-0.7.1/zetsubou/fastbuild/vcxproject.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/fastbuild/vssolution.py` & `zetsubou-0.7.1/zetsubou/fastbuild/vssolution.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/logo.py` & `zetsubou-0.7.1/zetsubou/logo.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/project/config_matrix.py` & `zetsubou-0.7.1/zetsubou/project/config_matrix.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/project/model/cli_tool.py` & `zetsubou-0.7.1/zetsubou/project/model/cli_tool.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/project/model/configuration.py` & `zetsubou-0.7.1/zetsubou/project/model/configuration.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/project/model/kind.py` & `zetsubou-0.7.1/zetsubou/project/model/kind.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/project/model/platform.py` & `zetsubou-0.7.1/zetsubou/project/model/platform.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/project/model/project_template.py` & `zetsubou-0.7.1/zetsubou/project/model/project_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Any
 from dataclasses import dataclass, field
 
 from bentoudev.dataclass.base import loaded_from_file, track_source
 
 
 @dataclass
 @track_source
@@ -32,10 +32,10 @@
 
 
 @loaded_from_file
 @dataclass
 class Project:
     project: str
     config: ProjectConfig
-    targets: List[str]
+    targets: Any
     conan: Optional[Conan] = None
     options: Optional[List[Option]] = field(default_factory=list)
```

### Comparing `zetsubou-0.7.0/zetsubou/project/model/target.py` & `zetsubou-0.7.1/zetsubou/project/model/target.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     defines: Optional[PropertyList] = field(default=None)
     compiler_flags: Optional[PropertyList] = field(default=None)
     linker_flags: Optional[PropertyList] = field(default=None)
     librarian_flags: Optional[PropertyList] = field(default=None)
     linker_paths: Optional[PathList] = field(default=None)
     link_libraries: Optional[PropertyList] = field(default=None)
     distribute_files: Optional[Source] = field(default=None)
+    build_require: Optional[List['zetsubou.project.model.target.TargetReference']] = field(default_factory=list) # noqa: F821
 
 
 @dataclass
 class TargetFilterData(TargetData):
     filter: TargetFilter = field(default_factory=TargetFilter)
```

### Comparing `zetsubou-0.7.0/zetsubou/project/model/toolchain.py` & `zetsubou-0.7.1/zetsubou/project/model/toolchain.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/project/model/toolchain_enums.py` & `zetsubou-0.7.1/zetsubou/project/model/toolchain_enums.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/project/model/toolchain_profile.py` & `zetsubou-0.7.1/zetsubou/project/model/toolchain_profile.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/project/model/virtual_environment.py` & `zetsubou-0.7.1/zetsubou/project/model/virtual_environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,14 +80,16 @@
 
             if activate == '' or deactivate == '':
                 proj_yml_path = proj.get_loaded_from_file()
                 logger.CriticalError('Virtual environment not found! \n'
                     f" Path '{proj.config.venv}' doesn't contain 'activate' and 'deactivate' scripts! Run 'zetsubou install' command or create them manually.")
                 return None
 
-            return VirtualEnvironment(activate=activate, deactivate=deactivate)
+            return VirtualEnvironment(
+                activate=os.path.join(proj.config.venv, activate),
+                deactivate=os.path.join(proj.config.venv, deactivate))
 
         else:
             raise ProjectError(proj.config.format_field_message("venv", "error",
                 f"Virtual environment not found! Path '{proj.config.venv}' doesnt exist or is not a directory!",
                 logger.GetErrorFormat())
             )
```

### Comparing `zetsubou-0.7.0/zetsubou/project/runtime/emit.py` & `zetsubou-0.7.1/zetsubou/project/runtime/emit.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/project/runtime/project_loader.py` & `zetsubou-0.7.1/zetsubou/project/runtime/project_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from zetsubou.project.model.toolchain_profile import Profile
 from zetsubou.project.model.rule import Rule
 from zetsubou.project.model.target import Target, find_target
 from zetsubou.project.model.toolchain import ToolchainDefinition, Toolchain
 from zetsubou.utils import logger, yaml_loader
 from zetsubou.utils.common import null_or_empty
 from zetsubou.utils.error import ProjectError
+from zetsubou.utils.file_cache import FileCache
 
 
 class NoTraceError(Exception):
     pass
 
 
 @dataclass
@@ -40,14 +41,21 @@
     system_toolchains: List[ToolchainDefinition]
     platform_toolchains: Dict[str, List[Toolchain]]
     cli_tools: List[CommandlineTool]
     configurations: List[Configuration]
     rules: List[Rule]
     targets: List[Target]
 
+    def find_target_by_file(self, filepath:str):
+        filename = os.path.basename(filepath)
+        for target in self.targets:
+            if filename == os.path.basename(target.get_loaded_from_file()):
+                return target
+        return None
+
     def find_target(self, name:str):
         return find_target(self.targets, name)
 
     def find_platform(self, name : str):
         for plat in self.platforms:
             if plat.platform == name:
                 return plat
@@ -169,27 +177,33 @@
 
 #             obj_templ.set_loaded_from_file(obj_path)
 #             return obj_templ
 #         else:
 #             raise NoTraceError()
 
 
-def load_dataclass_list(clazz: type, obj_ref_list: Optional[List[str]], proj_dir : str, project_fs : FS, loader, local_types):
+def load_dataclass_list(clazz: type, obj_ref_list: Optional[List[str]], proj_dir : str, project_fs : FS, loader, local_types, file_cache:Optional[FileCache] = None):
     result = []
 
     error_format = base.EErrorFormat.MSVC if logger.IsIde() else base.EErrorFormat.Pretty
 
     if not base.is_loaded_from_file(clazz):
         clazz = base.loaded_from_file(clazz)
 
     if obj_ref_list is not None and len(obj_ref_list) > 0:
 
         for obj_ref in obj_ref_list:
+            if os.path.dirname(obj_ref) == '':
+                logger.Warning(f"File '{obj_ref}' included from the same directory as main project file. Placement into subfolder is advised.")
+
             obj_path = fs.path.join(proj_dir, obj_ref)
 
+            if file_cache is not None:
+                file_cache.add_file(obj_path)
+
             if not project_fs.exists(obj_path) or not project_fs.isfile(obj_path):
                 raise ProjectError(f"Unknown to locate file '{obj_path}'")
 
             with project_fs.open(obj_path, 'r', encoding='utf-8') as obj_file:
                 obj_templ = loader.load_dataclass(clazz, obj_path, obj_file.read(), local_types, error_format=error_format)
 
                 if obj_templ is not None:
@@ -198,15 +212,15 @@
 
                     if logger.IsVisible(logger.ELogLevel.Verbose):
                         logger.Success(f"Loaded [{clazz.__name__}] '{obj_path}'")
 
                     obj_templ.set_loaded_from_file(obj_path)
                     result.append(obj_templ)
                 else:
-                    raise NoTraceError()
+                    raise ProjectError(f"Unable to load {clazz} from file '{obj_path}'")
 
     return result
 
 
 def load_bundled_rules(loader, local_types) -> List[Rule]:
     result = []
     for res_path in [ 'MsvcRules.yml', 'ClangRules.yml' ]:
@@ -221,29 +235,56 @@
                 logger.Success(f"Loaded [Rule] '{res_path}'")
 
             obj_templ.set_loaded_from_file(res_path)
             result.append(obj_templ)
     return result
 
 
-def load_project_template(project_fs: FS, fs_root : str, filename: str, proj_file_content: str, *, loader=yaml_loader.YamlDataclassLoader(), external_config:Optional[ExternalConfig]=None) -> Optional[ProjectTemplate]:
+def unpack_targets_from_any(any_targets) -> List[str]:
+    result : List[str] = []
+
+    def process_any(data):
+        tp = type(data)
+
+        if base.is_clazz_dict(tp):
+            for _, value in data.items():
+                process_any(value)
+
+        if base.is_clazz_list(tp):
+            for value in data:
+                process_any(value)
+
+        if tp is str:
+            result.append(data)
+
+    process_any(any_targets)
+
+    return result
+
+
+def load_project_template(project_fs: FS, fs_root : str, filename: str, proj_file_content: str, *,
+                          loader=yaml_loader.YamlDataclassLoader(), external_config:Optional[ExternalConfig]=None, file_cache:Optional[FileCache]=None) -> Optional[ProjectTemplate]:
     try:
         local_types = base.get_types_from_modules([__name__, 'zetsubou.project.model.target'])
 
+        if file_cache is not None:
+            file_cache.add_file(filename)
+
         proj_dir = os.path.dirname(filename)
         proj_templ: Project = loader.load_dataclass(Project, filename, proj_file_content, local_types)
         if proj_templ is None:
             return
 
         proj_templ.set_loaded_from_file(filename)
 
         def load_dataclasses(clazz: type, obj_ref_list: Optional[List[str]]):
-            return load_dataclass_list(clazz, obj_ref_list, proj_dir, project_fs, loader, local_types)
+            return load_dataclass_list(clazz, obj_ref_list, proj_dir, project_fs, loader, local_types, file_cache)
 
-        targets = load_dataclasses(Target, proj_templ.targets)
+        target_file_list = unpack_targets_from_any(proj_templ.targets)
+        targets = load_dataclasses(Target, target_file_list)
 
         proj = ProjectTemplate(
             project=proj_templ,
             profile=None,
             platforms=load_dataclasses(Platform, proj_templ.config.platforms),
             system_toolchains=[],
             platform_toolchains={},
@@ -290,13 +331,13 @@
 
     except Exception as error:
         logger.Exception(error)
         logger.CriticalError(f'Failed to load project  \'{filename}\'')
         return None
 
 
-def load_project_from_file(project_fs: FS, fs_root : str, filename: str, *, external_config:Optional[ExternalConfig]=None) -> Optional[ProjectTemplate]:
+def load_project_from_file(project_fs: FS, fs_root : str, filename: str, *, external_config:Optional[ExternalConfig]=None, file_cache:Optional[FileCache]=None) -> Optional[ProjectTemplate]:
     if not project_fs.exists(filename):
         logger.CriticalError(f"Unable to locate file '{filename}'")
         return None
     with project_fs.open(filename, 'r', encoding='utf-8') as proj_file:
-        return load_project_template(project_fs, fs_root, filename, proj_file.read(), external_config=external_config)
+        return load_project_template(project_fs, fs_root, filename, proj_file.read(), external_config=external_config, file_cache=file_cache)
```

### Comparing `zetsubou-0.7.0/zetsubou/project/runtime/resolve.py` & `zetsubou-0.7.1/zetsubou/project/runtime/resolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from typing import List, Optional, Any, Dict
 from dataclasses import dataclass, field, fields, is_dataclass
+from typing_inspect import get_origin
 import os
 import fnmatch, typing_inspect
 from zetsubou.project.model.config_string import EDefaultConfigSlots
 from zetsubou.project.model.configuration import Configuration
 from zetsubou.project.model.filter import TargetFilter
 
 from zetsubou.project.base_context import BaseContext
 from zetsubou.project.model.kind import ETargetKind
 from zetsubou.project.config_matrix import ConfigVariant, ConfigMatrix
 from zetsubou.project.runtime.project_loader import ProjectTemplate
 from zetsubou.project.model.target import PathList, Target, TargetData, Source, TargetReference, PropertyList
 from zetsubou.project.model.toolchain import Toolchain
+from zetsubou.utils import logger
+from bentoudev.dataclass.base import is_clazz_list
 
 
 def PrintDataclass(clazz, id = 0):
     prefix = ''
     for _ in range(id):
         prefix += ' '
 
@@ -93,24 +96,29 @@
             prop.interface = []
             prop.public = []
             prop.private = []
 
         for data_field in fields(TargetData):
             # Handle Optionals
             field_type = data_field.type
+
             if typing_inspect.is_optional_type(field_type):
                 field_type = field_type.__args__[0]
 
             self_value = getattr(self, data_field.name)
-            self_value = field_type()
 
-            if issubclass(field_type, Source):
-                init_sources(self_value)
+            if is_clazz_list(field_type):
+                self_value = list()
             else:
-                init_properties(self_value)
+                self_value = field_type()
+
+                if issubclass(field_type, Source):
+                    init_sources(self_value)
+                elif issubclass(field_type, PropertyList):
+                    init_properties(self_value)
 
             setattr(self, data_field.name, self_value)
 
 
     def apply(self, data: TargetData):
 
         for data_field in fields(TargetData):
@@ -118,21 +126,24 @@
             field_type = data_field.type
             if typing_inspect.is_optional_type(field_type):
                 field_type = field_type.__args__[0]
 
             self_value = getattr(self, data_field.name)
             other_value = getattr(data, data_field.name)
 
-            if issubclass(field_type, Source):
-                append_source(self_value, other_value)
-            elif issubclass(field_type, PathList):
-                # TODO: Needs fix, cannot blindly append relative paths
-                append_properties(self_value, other_value)
+            if is_clazz_list(field_type):
+                append_list(self_value, other_value)
             else:
-                append_properties(self_value, other_value)
+                if issubclass(field_type, Source):
+                    append_source(self_value, other_value)
+                elif issubclass(field_type, PathList):
+                    # TODO: Needs fix, cannot blindly append relative paths
+                    append_properties(self_value, other_value)
+                else:
+                    append_properties(self_value, other_value)
 
             setattr(self, data_field.name, self_value)
 
 
 @dataclass
 class ResolvedTarget:
     name: str
@@ -212,67 +223,77 @@
     target_cls_fields = fields(TargetData)
     target_source_path = target.get_loaded_from_file()
 
     accessors = [ 'private', 'public', 'interface' ]
     for access in accessors:
         deps : Optional[List[TargetReference]] = getattr(target_variant.dependencies, access)
 
-        if deps is not None:
-            for dep_ref in deps:
-                lnk_libs = getattr(target_variant.link_libraries, access)
-                lnk_libs.append(dep_ref)
-                setattr(target_variant.link_libraries, access, lnk_libs)
+        if deps is None:
+            continue
+
+        for dep_ref in deps:
+            lnk_libs = getattr(target_variant.link_libraries, access)
+            lnk_libs.append(dep_ref)
+            setattr(target_variant.link_libraries, access, lnk_libs)
+
+            dep_variant = create_target_variant(context, dep_ref.target, config_variant, config, toolchain)
+            dep_source_path = dep_ref.target.get_loaded_from_file()
+
+            imported_dep_target : bool = dep_ref.target.config.kind == ETargetKind.IMPORTED_TARGET
+            custom_dep_target   : bool = dep_ref.target.config.kind == ETargetKind.BUILD_STEP
 
-                dep_variant = create_target_variant(context, dep_ref.target, config_variant, config, toolchain)
-                dep_source_path = dep_ref.target.get_loaded_from_file()
+            # For custom build steps, manually make sure that they are executed before target is built
+            if custom_dep_target:
+                target_variant.build_require.append(dep_ref)
 
-                imported_dep_target : bool = dep_ref.target.config.kind == ETargetKind.IMPORTED_TARGET
+            if imported_dep_target:
+                # Manually pass imported includes as system ones
+                sys_inc_value_access = getattr(target_variant.system_includes, access)
 
-                if imported_dep_target:
-                    # Manually pass imported includes as system ones
-                    sys_inc_value_access = getattr(target_variant.system_includes, access)
+                append_paths(sys_inc_value_access, dep_variant.includes.public, target_source_path, dep_source_path, context.fs_root)
+                append_paths(sys_inc_value_access, dep_variant.includes.interface, target_source_path, dep_source_path, context.fs_root)
 
-                    append_paths(sys_inc_value_access, dep_variant.includes.public, target_source_path, dep_source_path, context.fs_root)
-                    append_paths(sys_inc_value_access, dep_variant.includes.interface, target_source_path, dep_source_path, context.fs_root)
+                append_paths(sys_inc_value_access, dep_variant.system_includes.public, target_source_path, dep_source_path, context.fs_root)
+                append_paths(sys_inc_value_access, dep_variant.system_includes.interface, target_source_path, dep_source_path, context.fs_root)
 
-                    append_paths(sys_inc_value_access, dep_variant.system_includes.public, target_source_path, dep_source_path, context.fs_root)
-                    append_paths(sys_inc_value_access, dep_variant.system_includes.interface, target_source_path, dep_source_path, context.fs_root)
+                setattr(target_variant.system_includes, access, sys_inc_value_access)
 
-                    setattr(target_variant.system_includes, access, sys_inc_value_access)
+            for data_field in target_cls_fields:
+                dep_field_holder = getattr(dep_variant, data_field.name)
 
-                for data_field in target_cls_fields:
-                    dep_field_holder = getattr(dep_variant, data_field.name)
+                if dep_field_holder is None:
+                    continue
 
-                    if dep_field_holder is None:
-                        continue
+                field_value = getattr(target_variant, data_field.name)
 
-                    field_value = getattr(target_variant, data_field.name)
+                # Handle Optionals
+                field_type = data_field.type
+                if typing_inspect.is_optional_type(field_type):
+                    field_type = field_type.__args__[0]
 
-                    # Handle Optionals
-                    field_type = data_field.type
-                    if typing_inspect.is_optional_type(field_type):
-                        field_type = field_type.__args__[0]
+                if field_type == list or get_origin(field_type) == list:
+                    append_list(field_value, dep_field_holder)
 
-                    if issubclass(field_type, PropertyList):
-                        dep_field_public = getattr(dep_field_holder, 'public')
-                        dep_field_iface = getattr(dep_field_holder, 'interface')
-                        field_value_access = getattr(field_value, access)
+                elif issubclass(field_type, PropertyList):
+                    dep_field_public = getattr(dep_field_holder, 'public')
+                    dep_field_iface = getattr(dep_field_holder, 'interface')
+                    field_value_access = getattr(field_value, access)
 
-                        if issubclass(field_type, PathList):
-                            # Includes for imported targets have to be handled manually
-                            if not (imported_dep_target and data_field.name.find('includes') != -1):
-                                append_paths(field_value_access, dep_field_public, target_source_path, dep_source_path, context.fs_root)
-                                append_paths(field_value_access, dep_field_iface, target_source_path, dep_source_path, context.fs_root)
-                        else:
-                            append_list(field_value_access, dep_field_public)
-                            append_list(field_value_access, dep_field_iface)
+                    if issubclass(field_type, PathList):
+                        # Includes for imported targets have to be handled manually
+                        if not (imported_dep_target and data_field.name.find('includes') != -1):
+                            append_paths(field_value_access, dep_field_public, target_source_path, dep_source_path, context.fs_root)
+                            append_paths(field_value_access, dep_field_iface, target_source_path, dep_source_path, context.fs_root)
+                    else:
+                        append_list(field_value_access, dep_field_public)
+                        append_list(field_value_access, dep_field_iface)
 
-                        setattr(field_value, access, field_value_access)
+                    setattr(field_value, access, field_value_access)
 
-                    setattr(target_variant, data_field.name, field_value)
+                setattr(target_variant, data_field.name, field_value)
 
 
 def create_target_variant(context: ResolveContext, target: Target, config_variant: ConfigVariant, config: Configuration, toolchain:Toolchain) -> TargetVariant:
     target_variant = context.find_target_variant(target, config_variant.config_string)
     if target_variant is None:
         target_variant = TargetVariant(config_variant)
         target_variant.apply(target)
```

### Comparing `zetsubou-0.7.0/zetsubou/project/runtime/validation.py` & `zetsubou-0.7.1/zetsubou/project/runtime/validation.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/system/discover_toolchains.py` & `zetsubou-0.7.1/zetsubou/system/discover_toolchains.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/system/tools.py` & `zetsubou-0.7.1/zetsubou/system/tools.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/system/windows/msvc.py` & `zetsubou-0.7.1/zetsubou/system/windows/msvc.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/system/windows/vswhere.py` & `zetsubou-0.7.1/zetsubou/system/windows/vswhere.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/system/windows/windows.py` & `zetsubou-0.7.1/zetsubou/system/windows/windows.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/utils/busy_indicator.py` & `zetsubou-0.7.1/zetsubou/utils/busy_indicator.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/utils/cmd_arguments.py` & `zetsubou-0.7.1/zetsubou/utils/cmd_arguments.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/utils/common.py` & `zetsubou-0.7.1/zetsubou/utils/common.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/utils/error_codes.py` & `zetsubou-0.7.1/zetsubou/utils/error_codes.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/utils/logger.py` & `zetsubou-0.7.1/zetsubou/utils/logger.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/utils/subprocess.py` & `zetsubou-0.7.1/zetsubou/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/utils/yaml_loader.py` & `zetsubou-0.7.1/zetsubou/utils/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/utils/yaml_simple_writer.py` & `zetsubou-0.7.1/zetsubou/utils/yaml_simple_writer.py`

 * *Files identical despite different names*

### Comparing `zetsubou-0.7.0/zetsubou/zetsubou.py` & `zetsubou-0.7.1/zetsubou/zetsubou.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 
         logger.Info(f"Current working directory - '{os.getcwd()}'")
         logger.Info(f"Project working directory - '{fs_root}'")
 
         cmd = Command.get_command_by_name(zet_args.command)
         cmd.Execute(command_context)
 
+        command_context.file_cache.save()
+
         end_time = time.time()
 
         if not zet_args.silent:
             print(f'\nFinished in {end_time - start_time:.2f} sec')
 
         return 0
```

### Comparing `zetsubou-0.7.0/zetsubou/zetsubou_conan_toolchain.py` & `zetsubou-0.7.1/zetsubou/zetsubou_conan_toolchain.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,29 +37,32 @@
     platform_file = None
 
     _project_template = None
     _conan_dependencies = None
 
     def _load_project_template(self, project_yml:str):
         if not os.path.exists(project_yml):
-            return None
+            raise ConanException(f"Project file '{project_yml}' not found! Ensure that it is added to both 'export' and 'export_sources' in conan recipe!")
         if self._project_template is None:
             with open(project_yml, mode='r') as in_proj:
                 self._project_template = yaml.load(in_proj, yaml.SafeLoader)
         return self._project_template
 
-    def _load_conan_ini(self, conan_ini:Optional[str]):
+    def _load_conan_ini(self, conan_ini:Optional[str], project_yml:str):
         if conan_ini is None:
             return None
 
+        conan_ini = os.path.join(os.path.dirname(project_yml), conan_ini)
+
         if not os.path.exists(conan_ini) or not os.path.isfile(conan_ini):
-            return None
+            raise ConanException(f"Dependency file '{conan_ini}' not found! Ensure that it is added to both 'export' and 'export_sources' in conan recipe!")
 
         with open(conan_ini, mode='r') as in_ini:
             conan_ini_content = in_ini.read()
+            print(f"Loaded: {os.path.abspath(conan_ini)}")
             return ConanFileTextLoader(conan_ini_content)
 
     def _load_conan_dependencies(self, project_yml:str):
         if self._conan_dependencies is None:
             proj = self._load_project_template(project_yml)
             if proj is None:
                 return None
@@ -69,32 +72,38 @@
                 return None
 
             tools_req_file = conan_data.get('build_tools', None)
             req_file = conan_data.get('dependencies', None)
 
             result = {}
 
-            tools_ini = self._load_conan_ini(tools_req_file)
+            tools_ini = self._load_conan_ini(tools_req_file, project_yml)
             if tools_ini is not None:
                 result['tool_requirements'] = tools_ini.tool_requirements
 
-            main_ini = self._load_conan_ini(req_file)
+            main_ini = self._load_conan_ini(req_file, project_yml)
             if main_ini is not None:
                 result['requirements'] = main_ini.requirements
 
             self._conan_dependencies = result
         return self._conan_dependencies
 
     def fill_requirements(self, conanfile:ConanFile, project_yml:str):
-        for entry in self._load_conan_dependencies(project_yml).get('requirements', []):
+        deps = self._load_conan_dependencies(project_yml)
+        if deps is None:
+            return
+        for entry in deps.get('requirements', []):
             if not any(filter(lambda r : r.ref.matches(entry, is_consumer=False), conanfile.requires.values())):
                 conanfile.requires(entry)
 
     def fill_tool_requirements(self, conanfile:ConanFile, project_yml:str):
-        for entry in self._load_conan_dependencies(project_yml).get('tool_requirements', []):
+        deps = self._load_conan_dependencies(project_yml)
+        if deps is None:
+            return
+        for entry in deps.get('tool_requirements', []):
             if not any(filter(lambda r : r.ref.matches(entry, is_consumer=False), conanfile.requires.values())):
                 conanfile.requires.tool_require(entry)
 
     def profile_filename(self, dir:str):
         return os.path.join(dir, 'conan_profile.yml')
 
     def init(self, conanfile:ConanFile, project_file:str="project.yml"):
@@ -149,39 +158,43 @@
             print("Zetsubou not initialized!")
         return self._zetsubou
 
     # This is unfortunately a hack
     # We store dependency data outside conanfile.py and need to read and setup them here
     # What makes life harder is a fact that folder paths are being setuped after dependency graph
     # So we need to guess where hardcoded project.yml is based on recipe path
-    # TODO Might not work for Conan 2.0!
+    # Additionaly, project.yml and dependency.ini files must be added to export and export_sources of the recipe
+    # Such files are not downloaded because source is called after requirements()
     @property
     def default_project(self):
         if self._project_yml == '':
             from_recipe_folder = os.path.join(self.recipe_folder, 'project.yml')
 
             if os.path.exists(from_recipe_folder) and os.path.isfile(from_recipe_folder):
                 self._project_yml = from_recipe_folder
+                print(f"From recipe folder: {from_recipe_folder}")
+
             elif self.recipe_folder.endswith('e'):
                 from_export = os.path.normpath(os.path.join(self.recipe_folder, '..', 'es', 'project.yml'))
                 if os.path.exists(from_export) and os.path.isfile(from_export):
                     self._project_yml = from_export
+                    print(f"From export folder: {from_export}")
 
         return self._project_yml
 
     def requirements(self):
         self.zetsubou.fill_requirements(self, self.default_project)
 
     def build_requirements(self):
         self.zetsubou.fill_tool_requirements(self, self.default_project)
 
 
 class ZetsubouGeneratorPackage(ConanFile):
     name = "zetsubougen"
-    version = "0.7.0"
+    version = "0.7.1"
     license = "MIT"
     description = 'Zetsubou yml files generator'
     url = "https://github.com/BentouDev/Zetsubou"
     package_type = "python-require"
 
     # Must be placed at the root of the source
     # Conan no longer allows referencing parent directory in relative paths
```

### Comparing `zetsubou-0.7.0/zetsubou.egg-info/PKG-INFO` & `zetsubou-0.7.1/zetsubou.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zetsubou
-Version: 0.7.0
+Version: 0.7.1
 Summary: FASTbuild generator for the helpless
 Author: BentouDev
 Project-URL: Homepage, https://github.com/BentouDev/Zetsubou
 Keywords: fastbuild,C++,cpp,C/C++,developer,tool
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zetsubou-0.7.0/zetsubou.egg-info/SOURCES.txt` & `zetsubou-0.7.1/zetsubou.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -78,13 +78,14 @@
 zetsubou/utils/__init__.py
 zetsubou/utils/busy_indicator.py
 zetsubou/utils/cmd_arguments.py
 zetsubou/utils/common.py
 zetsubou/utils/dataclass_loader.py
 zetsubou/utils/error.py
 zetsubou/utils/error_codes.py
+zetsubou/utils/file_cache.py
 zetsubou/utils/json_tools.py
 zetsubou/utils/logger.py
 zetsubou/utils/subprocess.py
 zetsubou/utils/yaml_loader.py
 zetsubou/utils/yaml_simple_writer.py
 zetsubou/utils/yaml_tools.py
```

