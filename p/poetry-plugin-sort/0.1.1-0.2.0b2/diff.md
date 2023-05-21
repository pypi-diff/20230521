# Comparing `tmp/poetry_plugin_sort-0.1.1.tar.gz` & `tmp/poetry_plugin_sort-0.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_sort-0.1.1.tar", max compression
+gzip compressed data, was "poetry_plugin_sort-0.2.0b2.tar", max compression
```

## Comparing `poetry_plugin_sort-0.1.1.tar` & `poetry_plugin_sort-0.2.0b2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1073 2022-09-01 22:04:20.415030 poetry_plugin_sort-0.1.1/LICENSE
--rw-r--r--   0        0        0     1994 2022-10-25 20:24:19.415470 poetry_plugin_sort-0.1.1/README.md
--rw-r--r--   0        0        0        0 2022-08-31 19:09:20.899554 poetry_plugin_sort-0.1.1/poetry_plugin_sort/__init__.py
--rw-r--r--   0        0        0     2288 2022-09-03 14:00:55.322154 poetry_plugin_sort-0.1.1/poetry_plugin_sort/plugins.py
--rw-r--r--   0        0        0     2612 2022-10-25 20:17:54.835096 poetry_plugin_sort-0.1.1/poetry_plugin_sort/sort.py
--rw-r--r--   0        0        0     1054 2022-10-25 20:19:37.929210 poetry_plugin_sort-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 poetry_plugin_sort-0.1.1/setup.py
--rw-r--r--   0        0        0     2849 1970-01-01 00:00:00.000000 poetry_plugin_sort-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-21 10:59:03.218084 poetry_plugin_sort-0.2.0b2/LICENSE
+-rw-r--r--   0        0        0     2009 2023-05-21 10:59:03.218084 poetry_plugin_sort-0.2.0b2/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 10:59:03.218084 poetry_plugin_sort-0.2.0b2/poetry_plugin_sort/__init__.py
+-rw-r--r--   0        0        0     1126 2023-05-21 10:59:03.218084 poetry_plugin_sort-0.2.0b2/poetry_plugin_sort/config.py
+-rw-r--r--   0        0        0     2671 2023-05-21 10:59:03.218084 poetry_plugin_sort-0.2.0b2/poetry_plugin_sort/plugins.py
+-rw-r--r--   0        0        0     4610 2023-05-21 10:59:03.218084 poetry_plugin_sort-0.2.0b2/poetry_plugin_sort/sort.py
+-rw-r--r--   0        0        0      262 2023-05-21 10:59:03.218084 poetry_plugin_sort-0.2.0b2/poetry_plugin_sort/utils.py
+-rw-r--r--   0        0        0     1132 2023-05-21 10:59:03.218084 poetry_plugin_sort-0.2.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 poetry_plugin_sort-0.2.0b2/PKG-INFO
```

### Comparing `poetry_plugin_sort-0.1.1/LICENSE` & `poetry_plugin_sort-0.2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_sort-0.1.1/README.md` & `poetry_plugin_sort-0.2.0b2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,40 @@
+Metadata-Version: 2.1
+Name: poetry-plugin-sort
+Version: 0.2.0b2
+Summary: Poetry plugin to sort the dependencies alphabetically
+Home-page: https://github.com/andrei-shabanski/poetry-plugin-sort
+License: MIT
+Keywords: poetry,plugin,dependencies sorting
+Author: Andrei Shabanski
+Author-email: shabanski.andrei@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: poetry (>=1.2.0,<2.0.0)
+Project-URL: Repository, https://github.com/andrei-shabanski/poetry-plugin-sort
+Description-Content-Type: text/markdown
+
 # Poetry Plugin: Dependencies sorting
 
 [![PyPI Version](https://img.shields.io/pypi/v/poetry-plugin-sort?label=PyPI)](https://pypi.org/project/poetry-plugin-sort/)
+[![Python Versions](https://img.shields.io/pypi/pyversions/poetry-plugin-sort)](https://pypi.org/project/poetry-plugin-sort/)
+[![check](https://github.com/andrei-shabanski/poetry-plugin-sort/actions/workflows/test.yml/badge.svg)](https://github.com/andrei-shabanski/poetry-plugin-sort/actions/workflows/test.yml)
 
 This package is a plugin that sort dependencies alphabetically in pyproject.toml
-after running `poetry init`, `poetry add`, or `poetry remove`.
+after running `poetry init` and `poetry add`.
 Since [Introduce dependency sorting #3996](https://github.com/python-poetry/poetry/pull/3996) pull request still open
 this plugin is a workaround for [!312](https://github.com/python-poetry/poetry/issues/312) issue.
 
-**Note**: the plugin is in the beta version!
-
-Before: 
-
-```toml
-[tool.poetry]
-name = "test"
-version = "0.1.0"
-description = ""
-authors = ["<author@example.com>"]
-
-[tool.poetry.dependencies]
-# a comment about a python version
-python = "^3.11"
-pydantic = "==1.6.2"  # upgrade pydantic to ...
-# Some notes about uvicorn
-uvicorn = "^0.19.0"
-#starlette = "==0.20.4"
-fastapi = "^0.85.1"
-
-#[tool.black]
-#target-version = ['py11']
-```
-
-After:
-
-```toml
-[tool.poetry]
-name = "test"
-version = "0.1.0"
-description = ""
-authors = ["<author@example.com>"]
-
-[tool.poetry.dependencies]
-# a comment about a python version
-python = "^3.11"
-#starlette = "==0.20.4"
-fastapi = "^0.85.1"
-pydantic = "==1.6.2"  # upgrade pydantic to ...
-# Some notes about uvicorn
-uvicorn = "^0.19.0"
-
-#[tool.black]
-#target-version = ['py11']
-```
-
-# Installation
+## Installation
 
 Just use `poetry self add` command to add this plugin.
 
 ```bash
 poetry self add poetry-plugin-sort
 ```
 
@@ -69,17 +46,28 @@
 
 And if you installed Poetry using pip, you can install the plugin the same way.
 
 ```bash
 pip install poetry poetry-plugin-sort
 ```
 
-# Usage
+## Usage
 
-The plugin sorts dependencies each time when you change dependencies via the `poetry init`, `poetry add`, or
-`poetry remove` commands.
+The plugin sorts dependencies each time when you change dependencies via the `poetry init` and `poetry add` commands.
 
-To sort dependencies without making changes to the depenencies list, the plugin provides a  `sort` command.
+To sort dependencies without making changes to the dependencies list, the plugin provides a  `sort` command.
 
 ```bash
 poetry sort
 ```
+
+### Available options
+
+* `--check`: Checks if dependencies are sorted and exits with a non-zero status code when it doesn't.
+
+### Configurations
+
+The following configuration can be set in `[tool.poetry-sort]` section of the pyproject.toml file or as system-wide environment variables:
+
+* `enable` \ `POETRY_SORT_ENABLED`: Enable or disable sorting after invoking `poetry init` and `poetry add` commands. Default: `True`.
+* `optionals-separately` \ `POETRY_SORT_OPTIONALS_SEPARATELY`: Move optional packages to the bottom. Default: `False`.
+
```

### Comparing `poetry_plugin_sort-0.1.1/poetry_plugin_sort/plugins.py` & `poetry_plugin_sort-0.2.0b2/poetry_plugin_sort/plugins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,77 @@
 from __future__ import annotations
 
 from typing import Type
 
 from cleo.events import console_events
 from cleo.events.console_terminate_event import ConsoleTerminateEvent
+from cleo.events.event import Event
 from cleo.events.event_dispatcher import EventDispatcher
+from cleo.helpers import option
 from cleo.io.io import IO
 from poetry.console.application import Application
 from poetry.console.commands.add import AddCommand
 from poetry.console.commands.command import Command
 from poetry.console.commands.init import InitCommand
-from poetry.console.commands.remove import RemoveCommand
 from poetry.plugins.application_plugin import ApplicationPlugin
 
+from poetry_plugin_sort import config
 from poetry_plugin_sort.sort import Sorter
 
 
 class SortCommand(Command):
     name = "sort"
     description = "Sorts the dependencies in pyproject.toml"
+    options = [
+        option(
+            "check", flag=True, description="Don't sort, just check if already sorted."
+        )
+    ]
 
     def handle(self) -> int:
-        sorter = Sorter(self.poetry, self.io)
-        sorter.sort()
-        return 0
+        sorter = Sorter(self.poetry, self.io, check=self.option("check"))
+        return 0 if sorter.sort() else 1
 
 
 class SortDependenciesPlugin(ApplicationPlugin):
     """Sorts dependencies in pyproject.toml file"""
 
     @property
     def commands(self) -> list[Type[Command]]:
         return [SortCommand]
 
     def activate(self, application: Application) -> None:
-        application.event_dispatcher.add_listener(
-            console_events.TERMINATE, self.sort_dependencies
-        )
+        if config.is_sorting_enabled(application.poetry):
+            application.event_dispatcher.add_listener(  # type: ignore[union-attr]
+                console_events.TERMINATE, self.sort_dependencies
+            )
 
         super().activate(application)
 
     def sort_dependencies(
-        self, event: ConsoleTerminateEvent, event_name: str, dispatcher: EventDispatcher
+        self, event: Event, event_name: str, dispatcher: EventDispatcher
     ) -> None:
+        assert isinstance(event, ConsoleTerminateEvent)
+
         io = event.io
         command = event.command
 
         if event.exit_code != 0:
             self._write_debug_lines(
                 io, "Skip sorting dependencies due to non-zero exit code."
             )
             return
 
-        if not isinstance(command, (InitCommand, AddCommand, RemoveCommand)):
+        if not isinstance(command, (InitCommand, AddCommand)):
             self._write_debug_lines(
                 io,
-                f"Skip sorting dependencies due to {command} does not change the"
-                " state.",
+                (
+                    f"Skip sorting dependencies due to {command} does not change the"
+                    " state."
+                ),
             )
             return
 
         if command.option("dry-run", False):
             self._write_debug_lines(
                 io, "Skip sorting dependencies due to --dry-run option."
             )
```

### Comparing `poetry_plugin_sort-0.1.1/pyproject.toml` & `poetry_plugin_sort-0.2.0b2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-sort"
-version = "0.1.1"
+version = "0.2.0b2"
 description = "Poetry plugin to sort the dependencies alphabetically"
 authors = ["Andrei Shabanski <shabanski.andrei@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/andrei-shabanski/poetry-plugin-sort"
 repository = "https://github.com/andrei-shabanski/poetry-plugin-sort"
 keywords = ["poetry", "plugin", "dependencies sorting"]
@@ -12,30 +12,35 @@
 packages = [{include = "poetry_plugin_sort"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 poetry = "^1.2.0"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^2.20.0"
-pytest = "^7.1.3"
-pytest-mock = "^3.8.2"
+mypy = "^1.2"
+pre-commit = "^2.20"
+pytest = "^7.1"
+pytest-mock = "^3.9"
 
 [tool.poetry.plugins."poetry.application.plugin"]
 sort = "poetry_plugin_sort.plugins:SortDependenciesPlugin"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 target-version = ['py37']
 preview = true
 
 [tool.isort]
 profile = "black"
-force_single_line = true
 atomic = true
 include_trailing_comma = true
 lines_after_imports = 2
 lines_between_types = 1
 use_parentheses = true
+
+[tool.mypy]
+python_version  = "3.7"
+ignore_missing_imports = true
+check_untyped_defs = true
```

