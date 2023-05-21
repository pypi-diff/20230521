# Comparing `tmp/alfred_cli-2.0.0b2.tar.gz` & `tmp/alfred_cli-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred_cli-2.0.0b2.tar", max compression
+gzip compressed data, was "alfred_cli-2.0.0b3.tar", max compression
```

## Comparing `alfred_cli-2.0.0b2.tar` & `alfred_cli-2.0.0b3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/LICENSE
--rw-r--r--   0        0        0     9788 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/README.md
--rw-r--r--   0        0        0     1584 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/pyproject.toml
--rw-r--r--   0        0        0      284 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/__init__.py
--rw-r--r--   0        0        0     1483 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/alfred_command.py
--rw-r--r--   0        0        0     5180 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/cli.py
--rw-r--r--   0        0        0     4636 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/commands.py
--rw-r--r--   0        0        0     3568 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/ctx.py
--rw-r--r--   0        0        0      682 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/decorator.py
--rw-r--r--   0        0        0        0 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/domain/__init__.py
--rw-r--r--   0        0        0     2404 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/domain/command.py
--rw-r--r--   0        0        0     1470 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/domain/manifest.py
--rw-r--r--   0        0        0      605 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/echo.py
--rw-r--r--   0        0        0      590 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/exceptions.py
--rw-r--r--   0        0        0     2571 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/interpreter.py
--rw-r--r--   0        0        0     2308 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/lib.py
--rw-r--r--   0        0        0      208 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/logger.py
--rw-r--r--   0        0        0     9465 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/main.py
--rw-r--r--   0        0        0     7872 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/manifest.py
--rw-r--r--   0        0        0      619 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/os.py
--rw-r--r--   0        0        0        9 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/resources/.alfred.toml
--rw-r--r--   0        0        0        0 2023-05-19 08:10:58.288941 alfred_cli-2.0.0b2/src/alfred/resources/__init__.py
--rw-r--r--   0        0        0      168 2023-05-19 08:10:58.292940 alfred_cli-2.0.0b2/src/alfred/resources/cmd.py
--rw-r--r--   0        0        0    11178 1970-01-01 00:00:00.000000 alfred_cli-2.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-21 09:38:29.925030 alfred_cli-2.0.0b3/LICENSE
+-rw-r--r--   0        0        0    10857 2023-05-21 09:38:29.925030 alfred_cli-2.0.0b3/README.md
+-rw-r--r--   0        0        0     1584 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0      284 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/__init__.py
+-rw-r--r--   0        0        0     1483 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/alfred_command.py
+-rw-r--r--   0        0        0     5527 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/cli.py
+-rw-r--r--   0        0        0     5614 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/commands.py
+-rw-r--r--   0        0        0     3486 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/ctx.py
+-rw-r--r--   0        0        0      682 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/decorator.py
+-rw-r--r--   0        0        0        0 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/domain/__init__.py
+-rw-r--r--   0        0        0     2404 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/domain/command.py
+-rw-r--r--   0        0        0     1470 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/domain/manifest.py
+-rw-r--r--   0        0        0      605 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/echo.py
+-rw-r--r--   0        0        0      645 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/exceptions.py
+-rw-r--r--   0        0        0     2978 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/interpreter.py
+-rw-r--r--   0        0        0     2605 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/lib.py
+-rw-r--r--   0        0        0      208 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/logger.py
+-rw-r--r--   0        0        0     9465 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/main.py
+-rw-r--r--   0        0        0     7872 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/manifest.py
+-rw-r--r--   0        0        0      619 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/os.py
+-rw-r--r--   0        0        0      432 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/resources/.alfred.toml
+-rw-r--r--   0        0        0        0 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/resources/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-21 09:38:29.929030 alfred_cli-2.0.0b3/src/alfred/resources/cmd.py
+-rw-r--r--   0        0        0    12199 1970-01-01 00:00:00.000000 alfred_cli-2.0.0b3/PKG-INFO
```

### Comparing `alfred_cli-2.0.0b2/LICENSE` & `alfred_cli-2.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b2/README.md` & `alfred_cli-2.0.0b3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 ## Alfred
 
 Alfred is an extensible building tool that can replace a Makefile or Fabric.
-Writing commands in python is done in a few minutes, even in the case of a mono-repository.
 
-```bash
-# use alfred to run continuous integration process
-alfred ci
+It allows you to build your **continuous integration scripts** in python, and much more. You can replace any scripts using the best of both worlds, shell and python.
+
+Want to try and look for inspiration, here are examples of commands that I implement in my projects :
 
-# use alfred to publish a package on pypi
-alfred publish
+```bash
+alfred ci # run your own continuous integration process
+alfred publish # publish a package on pypi
+alfred run # run your app
+alfred db:init # initialize a database
+alfred db:migrate # plays your migrations on your database
+...
 ```
 
 [![version](https://img.shields.io/pypi/v/alfred-cli.svg?label=version)](https://pypi.org/project/alfred-cli/) [![MIT](https://img.shields.io/badge/license-MIT-007EC7.svg)](LICENSE.md)
 
 [![ci](https://github.com/FabienArcellier/alfred-cli/actions/workflows/ci.yml/badge.svg)](https://github.com/FabienArcellier/alfred-cli/actions/workflows/ci.yml) [![ci-windows](https://github.com/FabienArcellier/alfred-cli/actions/workflows/ci-windows.yml/badge.svg)](https://github.com/FabienArcellier/pyalfred/actions/workflows/ci-windows.yml)
 
 <!-- TOC start (generated with https://github.com/derlin/bitdowntoc) -->
 
 - [Getting started](#getting-started)
 - [Links](#links)
 - [Cookbook](#cookbook)
-  * [Add a new build command](#add-a-new-build-command)
+  * [Write your first command](#write-your-first-command)
+  * [Write your first workflow](#write-your-first-workflow)
+- [Benefits](#benefits)
+  * [Alfred scales with your team](#alfred-scales-with-your-team)
+  * [Alfred likes mono-repository](#alfred-likes-mono-repository)
 - [Behind the scene](#behind-the-scene)
-- [Why using alfred instead of Makefile or Bash scripts](#why-using-alfred-instead-of-makefile-or-bash-scripts)
+  * [Why using alfred instead of Makefile or Bash scripts](#why-using-alfred-instead-of-makefile-or-bash-scripts)
 - [Why not using alfred](#why-not-using-alfred)
 - [The latest version](#the-latest-version)
 - [Cookbook](#cookbook-1)
-  * [Display the commands really executed behind the scene](#display-the-commands-really-executed-behind-the-scene)
+  * [Display the commands really executed](#display-the-commands-really-executed)
   * [Customize a command for a specific OS](#customize-a-command-for-a-specific-os)
   * [Override environment variables](#override-environment-variables)
     + [Add directories into pythonpath](#add-directories-into-pythonpath)
 - [Developper guideline](#developper-guideline)
   * [Run the linter and the unit tests](#run-the-linter-and-the-unit-tests)
 - [Contributors](#contributors)
 - [License](#license)
@@ -42,100 +50,102 @@
 To configure a python project to use alfred, here is the procedure:
 
 ```bash
 pip3 install alfred-cli
 alfred init
 ```
 
-A hello_world command was created for the example:
+Une première commande a été crée pour vous. Elle vous permet de tester alfred.
 
 ```bash
 alfred hello_world --name "Fabien"
 ```
 
-A file `.alfred.yml` will be initialized at the root of the repository.
+A file `.alfred.toml` will be initialized at the root of the repository.
 
 ## Links
 
 * Documentation : https://alfred-cli.readthedocs.io/en/latest
 * PyPI Release : https://pypi.org/project/alfred-cli
 * Source code: https://github.com/FabienArcellier/alfred-cli
 * Chat: https://discord.gg/nMn9YPRGSY
 
 ## Cookbook
 
-### Add a new command
+### Write your first command
 
 You can add your command in a new module in `./alfred`.
 In this example we will add the command `alfred lint` :
 
+*alfred/lint.py*
 ```python
-import os
-
 import alfred
 
-ROOT_DIR = os.path.realpath(os.path.join(__file__, "..", ".."))
-
-@alfred.command('lint', help="validate alfred using pylint on the package alfred")
+@alfred.command('lint', help="validate your product using mypy")
 def lint():
-    # get the command pylint in the user system or show error message if it's missing
-    pylint = alfred.sh('pylint', "pylint is not installed")
-
-    # behind the scene, it invokes the command `pylint alfred`
+    pylint = alfred.sh('mypy', "mypy is not installed")
     alfred.run(pylint, ["src/alfred"])
 ```
 
+### Write your first workflow
+
+*alfred/ci.py*
+```python
+import alfred
+
+@alfred.command('ci', help="execute continuous integration process")
+def ci(verbose: bool):
+    alfred.invoke_command('lint')
+    alfred.invoke_command('tests')
+```
+
+## Benefits
+
+### Alfred scales with your team
+
+Alfred grows with your team. You can start with one command and then add more. When you feel that your command file is too crowded, you can restructure it into several files, or even separate it into several subfolders. Alfred is able to search all your orders by scanning a folder and its subfolders. It's all configurable.
+
+### Alfred likes mono-repository
+
+Alfred is built with the idea of being usable in a mono-repository which brings together several python, react, node projects in the same code repository. You can create several alfred sub-projects. At the root of the project, you will have access to all the commands of all the subprojects using the subproject name ``alfred project1 ci``.
+
 ## Behind the scene
 
 Alfred rely heavily on click and plumblum :
 
 * [click](https://click.palletsprojects.com/en/8.0.x/)
 * [plumblum](https://plumbum.readthedocs.io/en/latest/)
 
-## Why using alfred instead of Makefile or Bash scripts
+### Why using alfred instead of Makefile or Bash scripts
+
+One of the advantages of `bash` and `Makefile` is their native presence in many environments. By default, a `Makefile` allows you to segment these commands efficiently. Autocompletion is first-citizen  feature. Alfred doesn't have it yet.
+
+Alfred allows you to create more complex commands than with Make. From the start, you benefit from a formatted documentation for each of your orders. It is easy to create one command per file  thanks to auto discovery. You can see an implementation in this repository in [`alfred_cmd/`](alfred/).
+
+Alfred allows you to mix shell code with python instructions. In some cases, it allows you to perform efficient processing on API calls. You can use either the cli (for git, ...) or pythons libraries depending on the nature of the treatment you want to perform.
 
-One of the advantages of `bash` and `Makefile` is their native presence in many environments.
-By default, a `Makefile` allows you to segment these commands efficiently. Autocompletion is first-citizen
-feature. Alfred doesn't have it yet.
-
-Alfred allows you to create more complex commands than with Make. From the start, you benefit from a
-formatted documentation for each of your orders. It is easy to create one command per file  thanks
-to auto discovery. You can see an implementation in this repository in [`alfred_cmd/`](alfred/).
-
-Thanks to the power of Click, it's easy to add options to your commands.
-They allow for example to implement flags for your CI process which
-offer you an execution for the frontend.
-
-Alfred allows you to mix shell code with python instructions. In some cases, it allows you
-to perform efficient processing on API calls. You can use either the cli (for git, ...) or
-pythons libraries depending on the nature of the treatment you want to perform.
-
-In our development process, we frequently need to operate on application with several process (frontend in react,
-server in flask, two external service in flask). To mount those process, we use `honcho` with alfred
-to load `Procfile` that will manage those process.
+In our development process, we frequently need to operate on application with several process (frontend in react, server in flask, two external service in flask). To mount those process, we use `honcho` with alfred to load `Procfile` that will manage those process.
 
 ## Why not using alfred
 
-If you want to create a cli you will distribute, alfred is not designed for that. I won't recommand
-as well to use it to build a data application even if you can use python and many library.
+If you want to create a cli you will distribute, alfred is not designed for that. I won't recommand as well to use it to build a data application even if you can use python and many library.
 
-Alfred command can import only installed library. You can't use relative import. That makes difficult to
-share code between your commands.
+Alfred command can import only installed library. You can't use relative import. That makes difficult to share code between your commands.
 
 ## The latest version
 
 You can find the latest version to ...
 
 ```bash
 git clone https://github.com/FabienArcellier/alfred-cli.git
 ```
 
 ## Cookbook
 
-### Display the commands really executed behind the scene
+### Display the commands really executed
 
 You can display the commands really executed, either to debug the arguments,
 either to run in your terminal again with other attributes.
 
 The option `d` / `--debug` display all the shell commands that are executed by
 `alfred.run()` in your alfred command.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alfred_cli-2.0.0b2/pyproject.toml` & `alfred_cli-2.0.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alfred-cli"
-version = "2.0.0b2"
+version = "2.0.0b3"
 description = "alfred is an extensible building tool that can replace a Makefile or Fabric. Writing commands in python is done in minutes."
 authors = ["Fabien Arcellier <fabien.arcellier@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "alfred", from = "src"}]
 include = [
     { path = "alfred/resources/*" }
```

### Comparing `alfred_cli-2.0.0b2/src/alfred/alfred_command.py` & `alfred_cli-2.0.0b3/src/alfred/alfred_command.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b2/src/alfred/cli.py` & `alfred_cli-2.0.0b3/src/alfred/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import logging
 import os
 import shutil
 import sys
 from typing import List, Any, Generator
 
 import click
+from click.exceptions import Exit
 
+import alfred
 from alfred import ctx as alfred_ctx, manifest, echo, project_directory
 from alfred import commands
 from alfred.ctx import Context
 from alfred.decorator import AlfredCommand
 from alfred.exceptions import NotInitialized
 from alfred.lib import ROOT_DIR, override_pythonpath
 from alfred.logger import logger
@@ -88,32 +90,36 @@
         """
         Invoking an alfred command may run with a different interpreter than
         the one a developer first invoked alfred with.
 
         From the command, if it is played with the wrong interpreter, alfred restarts itself with the target interpreter.
         """
         args = [*ctx.protected_args, *ctx.args]
-        cmd_output = self.resolve_command(ctx, args)
-
-        if cmd_output is not None and alfred_ctx.should_use_external_venv():
-            alfred_ctx.invoke_through_external_venv(args)
-
-
-            return
+        if ctx.params['version'] is True:
+            echo.message(f"{alfred.__version__}")
+            raise Exit(code=0)
+
+        if len(args) > 0:
+            cmd_output = self.resolve_command(ctx, args)
+
+            if cmd_output is not None and alfred_ctx.should_use_external_venv():
+                alfred_ctx.invoke_through_external_venv(args)
+                return
 
         """
         The command is executed by click normally.
         """
         super().invoke(ctx)
 
 
 @click.command(cls=AlfredCli,
                help='alfred is a building tool to make engineering tasks easier to develop and to maintain')
 @click.option("-d", "--debug", is_flag=True, help="display debug information like command runned and working directory")
-def cli(debug: bool):
+@click.option("-v", "--version", is_flag=True, help="display the version of alfred")
+def cli(debug: bool, version: bool):  # pylint: disable=unused-argument
     if debug:
         logger.setLevel(logging.DEBUG)
 
     display_obsolete_manifests()
 
 
 def display_obsolete_manifests():
```

### Comparing `alfred_cli-2.0.0b2/src/alfred/commands.py` & `alfred_cli-2.0.0b3/src/alfred/commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 Ce module fournit des fonctions pour charger les commandes d'un projet
 alfred et de ses sous projets.
 """
 import glob
 import os
 import typing as t
+from functools import lru_cache
 from typing import List
 
 import click
 from click import Context, Command
 
 from alfred import manifest, echo
 from alfred.domain.command import AlfredCommand
-from alfred.lib import list_python_modules, import_python
-
+from alfred.lib import list_python_modules, import_python, InvalidCommandModule
 
 class AlfredSubprojectCommand(click.MultiCommand):
 
     def __init__(self, *args, **attrs: t.Any):
         if "path" in attrs:
             self.path = attrs["path"]
             del attrs["path"]
@@ -25,58 +25,60 @@
         super().__init__(*args, **attrs)
 
     def list_commands(self, ctx: Context) -> t.List[str]:
         all_commands = list_all(self.path)
         return [command.name for command in all_commands]
 
     def get_command(self, ctx: Context, cmd_name: str) -> t.Optional[Command]:
-        all_commands = list_all(self.path)
+        all_commands = list_all(self.path, show_error=False)
         for _command in all_commands:
             if _command.name == cmd_name:
                 return _command.command
 
         return None
 
 
-def list_all(project_dir: t.Optional[str] = None) -> List[AlfredCommand]:
+def cache_clear():
+    """
+    Reset the cache of commands and cause them to be loaded again when the module is called again.
+
+    Resets the cache of the list_all function.
+    """
+    list_all.cache_clear()
+
+
+@lru_cache(maxsize=None)
+def list_all(project_dir: t.Optional[str] = None, show_error: bool = True) -> List[AlfredCommand]:
     """
     Loads all commands available in the project. This function retrieves the .alfred.yml manifest,
     analyzes the plugins present and loads the commands.
 
     The search for the manifest is done from the current directory. If the manifest is not found, the search continues
     and goes back to the parent folder.
 
-    Once the commands are loaded, they are available in _commands global variable.
+    If a command module is invalid, for example, the python code has a syntax error, an error message is displayed in the terminal.
+    The commands of the other modules remain executable.
+
+    The result of this function is cached to avoid displaying the same error messages several times and
+    to avoid loading the content of the commands several times during an execution.
 
     >>> from alfred import commands
     >>> commands.list_all()
     """
     subproject = None
     main_project_dir = manifest.lookup_project_dir()
     if project_dir is None:
         project_dir = main_project_dir
 
     if main_project_dir != project_dir:
         subproject = manifest.name(project_dir)
 
     commands = []
     for pattern in manifest.project_commands(project_dir):
-        pattern_path = os.path.join(project_dir, pattern)
-        prefix = manifest.prefix(project_dir)
-        for python_module in list_python_modules(pattern_path):
-            module_path = os.path.join(project_dir, python_module)
-            module = import_python(module_path)
-            for command in module.values():
-                if isinstance(command, AlfredCommand):
-                    command.module = python_module
-                    command.path = os.path.realpath(python_module)
-                    command.project_dir = os.path.realpath(project_dir)
-                    command.command.name = f"{prefix}{command.name}"
-                    command.subproject = subproject
-                    commands.append(command)
+        commands = _load_commands(commands, pattern, project_dir, subproject, show_error)
 
     subprojects_glob = manifest.subprojects(project_dir)
     for subproject in subprojects_glob:
         directories = glob.glob(subproject)
         for directory in directories:
             if os.path.isdir(directory) and manifest.contains_manifest(directory):
                 commands = _load_subproject(commands, directory)
@@ -94,15 +96,15 @@
     Searches for an order based on its project and its name.
 
     >>> _command = commands.lookup(["product1", 'build'])
     """
     if isinstance(command, str):
         command = [command]
 
-    all_commands = list_all(project_dir)
+    all_commands = list_all(project_dir, show_error=False)
     for _command in all_commands:
         if _command.name == command[0]:
             if isinstance(_command.command, AlfredSubprojectCommand):
                 if len(command) == 1:
                     return _command
 
                 subcommands = list_all(_command.project_dir)
@@ -111,14 +113,36 @@
                         return subcommand
 
             return _command
 
     return None
 
 
+def _load_commands(commands: list, pattern: str, project_dir: str, subproject: str, show_error: bool):
+    pattern_path = os.path.join(project_dir, pattern)
+    prefix = manifest.prefix(project_dir)
+    for python_module in list_python_modules(pattern_path):
+        module_path = os.path.join(project_dir, python_module)
+        try:
+            module = import_python(module_path)
+            for command in module.values():
+                if isinstance(command, AlfredCommand):
+                    command.module = python_module
+                    command.path = os.path.realpath(python_module)
+                    command.project_dir = os.path.realpath(project_dir)
+                    command.command.name = f"{prefix}{command.name}"
+                    command.subproject = subproject
+                    commands.append(command)
+        except InvalidCommandModule as exception:
+            if show_error:
+                echo.error(str(exception))
+
+    return commands
+
+
 def _load_subproject(commands: list, directory: str) -> list:
     _subproject_manifest = manifest.lookup(directory)
     name = manifest.name(directory)
     if ' ' in name:
         echo.error(f"Subproject ignored: project name from {directory} cannot contain spaces, {name=}")
     else:
         command = AlfredCommand()
```

### Comparing `alfred_cli-2.0.0b2/src/alfred/ctx.py` & `alfred_cli-2.0.0b3/src/alfred/ctx.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 import contextlib
 import dataclasses
 from typing import List, Optional
 
 from click.exceptions import Exit
 
-from alfred import manifest, interpreter, echo
+from alfred import manifest, interpreter
 from alfred.decorator import AlfredCommand
 from alfred.exceptions import NotInCommand
 from alfred.logger import get_logger
 
 
 @dataclasses.dataclass
 class Context:
@@ -48,18 +48,15 @@
 def invoke_through_external_venv(args: List[str]) -> None:
     """
     Invokes the current alfred command in its own virtual environment.
 
     """
     alfred_cmd = current_command()
     venv = manifest.lookup_venv(alfred_cmd.project_dir)
-    exit_code, stdout, stderr = interpreter.run_module(module='alfred.cli', venv=venv, args=args)
-    print(stdout)
-    if stderr != "":
-        echo.error(stderr)
+    exit_code, _, _ = interpreter.run_module(module='alfred.cli', venv=venv, args=args)
 
     if exit_code != 0:
         raise Exit(exit_code)
 
 
 def root_command() -> Optional[AlfredCommand]:
     """
```

### Comparing `alfred_cli-2.0.0b2/src/alfred/decorator.py` & `alfred_cli-2.0.0b3/src/alfred/decorator.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b2/src/alfred/domain/command.py` & `alfred_cli-2.0.0b3/src/alfred/domain/command.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b2/src/alfred/domain/manifest.py` & `alfred_cli-2.0.0b3/src/alfred/domain/manifest.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b2/src/alfred/echo.py` & `alfred_cli-2.0.0b3/src/alfred/echo.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b2/src/alfred/exceptions.py` & `alfred_cli-2.0.0b3/src/alfred/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,17 @@
     def __init__(self, message: str, *args, **kwargs):
         super().__init__(args, kwargs)
         self.message = message
 
     def __str__(self):
         return self.message
 
+class InvalidCommandModule(AlfredException):
+    pass
+
 
 class NotInitialized(AlfredException):
     pass
 
 
 class NotInCommand(AlfredException):
     def __init__(self, instruction: str):
```

### Comparing `alfred_cli-2.0.0b2/src/alfred/interpreter.py` & `alfred_cli-2.0.0b3/src/alfred/interpreter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import sys
 from typing import Optional, List, Tuple, Union
 
 import plumbum
 from plumbum import local
+from plumbum.commands.modifiers import _TEE
 
 from alfred.os import is_windows
 from alfred.exceptions import AlfredException
 from alfred.logger import logger
 
 
 def current() -> str:
@@ -43,15 +44,24 @@
         raise AlfredException(f"bin folder not found in venv: {venv}, {bin_path=}")
 
     python = plumbum.local[python_path]
     logger.debug(f"alfred interpreter - switch to python: {python_path} : {args=}")
 
     with local.env(VIRTUAL_ENV=venv, PATH=global_path):
         python_args = ['-m', module] + args
-        exit_code, stdout, stderr = python[python_args].run(retcode=None)
+        if is_windows():
+            # windows does not support streaming through plumbum.
+            # the publication is done at the end of the call.
+            #
+            # I don't know how to do better.
+            exit_code, stdout, stderr = python[python_args].run(retcode=None)
+            print(stdout)
+            print(stderr)
+        else:
+            exit_code, stdout, stderr = python[python_args] & _TEE(retcode=None)
         return exit_code, stdout, stderr
 
 
 def venv_bin_path(venv: str) -> str:
     """
     Determines the path to the binary folder based on the OS and virtual environment path.
     """
```

### Comparing `alfred_cli-2.0.0b2/src/alfred/lib.py` & `alfred_cli-2.0.0b3/src/alfred/lib.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,40 +3,41 @@
 import io
 import os
 import sys
 from typing import List, Iterator
 
 from plumbum import local
 
+from alfred.exceptions import InvalidCommandModule
 from alfred.logger import get_logger
 
 ROOT_DIR = os.path.realpath(os.path.join(__file__, '..'))
 
 
-class InvalidPythonModule(Exception):
-    pass
-
-
 def import_python(python_path: str) -> dict:
 
     module = {"__file__": python_path}
     with io.open(python_path, encoding="utf8") as file:
         content = file.read()
         try:
             code = compile(content, python_path, 'exec')
             eval(code, module, module)  # pylint: disable=eval-used
-        except Exception as exception:
+        except Exception as exception: # pylint: disable=broad-except
             rows = content.split("\n")
             exc_type, _, exc_tb = sys.exc_info()
-            line = "N/D"
-            if hasattr(exc_tb, "tb_next"):
+            line = None
+            if hasattr(exc_tb, "tb_next") and hasattr(exc_tb.tb_next, "tb_lineno"):
                 line = exc_tb.tb_next.tb_lineno
-            raise InvalidPythonModule(f"""Invalid command module : "{python_path}", Line {line}
-  {rows[line - 1]}\n
-  {exc_type.__name__} : {exception}\n""") from exception
+
+            if line is not None:
+                content = rows[line - 1]
+                raise InvalidCommandModule(f"""command module "{python_path}" is not valid at line {line} : {content}.\n {exc_type.__name__} : {exception}\n""") from exception
+
+            raise InvalidCommandModule(f"""command module "{python_path}" is not valid.\n {exc_type.__name__} : {exception}\n""") from exception
+
 
     return module
 
 
 def list_python_modules(glob_expression: str) -> Iterator[str]:
     for filename in glob.glob(glob_expression):
         if filename.endswith('.py') and filename != '__init__.py':
```

### Comparing `alfred_cli-2.0.0b2/src/alfred/main.py` & `alfred_cli-2.0.0b3/src/alfred/main.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b2/src/alfred/manifest.py` & `alfred_cli-2.0.0b3/src/alfred/manifest.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b2/src/alfred/os.py` & `alfred_cli-2.0.0b3/src/alfred/os.py`

 * *Files identical despite different names*

### Comparing `alfred_cli-2.0.0b2/PKG-INFO` & `alfred_cli-2.0.0b3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred-cli
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: alfred is an extensible building tool that can replace a Makefile or Fabric. Writing commands in python is done in minutes.
 Home-page: https://github.com/FabienArcellier/alfred-cli#alfred
 License: MIT
 Keywords: building tool,makefile,productivity,automation,continuous integration,developper friendly
 Author: Fabien Arcellier
 Author-email: fabien.arcellier@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -13,54 +13,61 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: plumbum (>=1.8.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Documentation, https://alfred-cli.readthedocs.io/en/latest
 Project-URL: Repository, https://github.com/FabienArcellier/alfred-cli
 Description-Content-Type: text/markdown
 
 ## Alfred
 
 Alfred is an extensible building tool that can replace a Makefile or Fabric.
-Writing commands in python is done in a few minutes, even in the case of a mono-repository.
 
-```bash
-# use alfred to run continuous integration process
-alfred ci
+It allows you to build your **continuous integration scripts** in python, and much more. You can replace any scripts using the best of both worlds, shell and python.
+
+Want to try and look for inspiration, here are examples of commands that I implement in my projects :
 
-# use alfred to publish a package on pypi
-alfred publish
+```bash
+alfred ci # run your own continuous integration process
+alfred publish # publish a package on pypi
+alfred run # run your app
+alfred db:init # initialize a database
+alfred db:migrate # plays your migrations on your database
+...
 ```
 
 [![version](https://img.shields.io/pypi/v/alfred-cli.svg?label=version)](https://pypi.org/project/alfred-cli/) [![MIT](https://img.shields.io/badge/license-MIT-007EC7.svg)](LICENSE.md)
 
 [![ci](https://github.com/FabienArcellier/alfred-cli/actions/workflows/ci.yml/badge.svg)](https://github.com/FabienArcellier/alfred-cli/actions/workflows/ci.yml) [![ci-windows](https://github.com/FabienArcellier/alfred-cli/actions/workflows/ci-windows.yml/badge.svg)](https://github.com/FabienArcellier/pyalfred/actions/workflows/ci-windows.yml)
 
 <!-- TOC start (generated with https://github.com/derlin/bitdowntoc) -->
 
 - [Getting started](#getting-started)
 - [Links](#links)
 - [Cookbook](#cookbook)
-  * [Add a new build command](#add-a-new-build-command)
+  * [Write your first command](#write-your-first-command)
+  * [Write your first workflow](#write-your-first-workflow)
+- [Benefits](#benefits)
+  * [Alfred scales with your team](#alfred-scales-with-your-team)
+  * [Alfred likes mono-repository](#alfred-likes-mono-repository)
 - [Behind the scene](#behind-the-scene)
-- [Why using alfred instead of Makefile or Bash scripts](#why-using-alfred-instead-of-makefile-or-bash-scripts)
+  * [Why using alfred instead of Makefile or Bash scripts](#why-using-alfred-instead-of-makefile-or-bash-scripts)
 - [Why not using alfred](#why-not-using-alfred)
 - [The latest version](#the-latest-version)
 - [Cookbook](#cookbook-1)
-  * [Display the commands really executed behind the scene](#display-the-commands-really-executed-behind-the-scene)
+  * [Display the commands really executed](#display-the-commands-really-executed)
   * [Customize a command for a specific OS](#customize-a-command-for-a-specific-os)
   * [Override environment variables](#override-environment-variables)
     + [Add directories into pythonpath](#add-directories-into-pythonpath)
 - [Developper guideline](#developper-guideline)
   * [Run the linter and the unit tests](#run-the-linter-and-the-unit-tests)
 - [Contributors](#contributors)
 - [License](#license)
@@ -72,100 +79,102 @@
 To configure a python project to use alfred, here is the procedure:
 
 ```bash
 pip3 install alfred-cli
 alfred init
 ```
 
-A hello_world command was created for the example:
+Une première commande a été crée pour vous. Elle vous permet de tester alfred.
 
 ```bash
 alfred hello_world --name "Fabien"
 ```
 
-A file `.alfred.yml` will be initialized at the root of the repository.
+A file `.alfred.toml` will be initialized at the root of the repository.
 
 ## Links
 
 * Documentation : https://alfred-cli.readthedocs.io/en/latest
 * PyPI Release : https://pypi.org/project/alfred-cli
 * Source code: https://github.com/FabienArcellier/alfred-cli
 * Chat: https://discord.gg/nMn9YPRGSY
 
 ## Cookbook
 
-### Add a new command
+### Write your first command
 
 You can add your command in a new module in `./alfred`.
 In this example we will add the command `alfred lint` :
 
+*alfred/lint.py*
 ```python
-import os
-
 import alfred
 
-ROOT_DIR = os.path.realpath(os.path.join(__file__, "..", ".."))
-
-@alfred.command('lint', help="validate alfred using pylint on the package alfred")
+@alfred.command('lint', help="validate your product using mypy")
 def lint():
-    # get the command pylint in the user system or show error message if it's missing
-    pylint = alfred.sh('pylint', "pylint is not installed")
-
-    # behind the scene, it invokes the command `pylint alfred`
+    pylint = alfred.sh('mypy', "mypy is not installed")
     alfred.run(pylint, ["src/alfred"])
 ```
 
+### Write your first workflow
+
+*alfred/ci.py*
+```python
+import alfred
+
+@alfred.command('ci', help="execute continuous integration process")
+def ci(verbose: bool):
+    alfred.invoke_command('lint')
+    alfred.invoke_command('tests')
+```
+
+## Benefits
+
+### Alfred scales with your team
+
+Alfred grows with your team. You can start with one command and then add more. When you feel that your command file is too crowded, you can restructure it into several files, or even separate it into several subfolders. Alfred is able to search all your orders by scanning a folder and its subfolders. It's all configurable.
+
+### Alfred likes mono-repository
+
+Alfred is built with the idea of being usable in a mono-repository which brings together several python, react, node projects in the same code repository. You can create several alfred sub-projects. At the root of the project, you will have access to all the commands of all the subprojects using the subproject name ``alfred project1 ci``.
+
 ## Behind the scene
 
 Alfred rely heavily on click and plumblum :
 
 * [click](https://click.palletsprojects.com/en/8.0.x/)
 * [plumblum](https://plumbum.readthedocs.io/en/latest/)
 
-## Why using alfred instead of Makefile or Bash scripts
+### Why using alfred instead of Makefile or Bash scripts
+
+One of the advantages of `bash` and `Makefile` is their native presence in many environments. By default, a `Makefile` allows you to segment these commands efficiently. Autocompletion is first-citizen  feature. Alfred doesn't have it yet.
+
+Alfred allows you to create more complex commands than with Make. From the start, you benefit from a formatted documentation for each of your orders. It is easy to create one command per file  thanks to auto discovery. You can see an implementation in this repository in [`alfred_cmd/`](alfred/).
+
+Alfred allows you to mix shell code with python instructions. In some cases, it allows you to perform efficient processing on API calls. You can use either the cli (for git, ...) or pythons libraries depending on the nature of the treatment you want to perform.
 
-One of the advantages of `bash` and `Makefile` is their native presence in many environments.
-By default, a `Makefile` allows you to segment these commands efficiently. Autocompletion is first-citizen
-feature. Alfred doesn't have it yet.
-
-Alfred allows you to create more complex commands than with Make. From the start, you benefit from a
-formatted documentation for each of your orders. It is easy to create one command per file  thanks
-to auto discovery. You can see an implementation in this repository in [`alfred_cmd/`](alfred/).
-
-Thanks to the power of Click, it's easy to add options to your commands.
-They allow for example to implement flags for your CI process which
-offer you an execution for the frontend.
-
-Alfred allows you to mix shell code with python instructions. In some cases, it allows you
-to perform efficient processing on API calls. You can use either the cli (for git, ...) or
-pythons libraries depending on the nature of the treatment you want to perform.
-
-In our development process, we frequently need to operate on application with several process (frontend in react,
-server in flask, two external service in flask). To mount those process, we use `honcho` with alfred
-to load `Procfile` that will manage those process.
+In our development process, we frequently need to operate on application with several process (frontend in react, server in flask, two external service in flask). To mount those process, we use `honcho` with alfred to load `Procfile` that will manage those process.
 
 ## Why not using alfred
 
-If you want to create a cli you will distribute, alfred is not designed for that. I won't recommand
-as well to use it to build a data application even if you can use python and many library.
+If you want to create a cli you will distribute, alfred is not designed for that. I won't recommand as well to use it to build a data application even if you can use python and many library.
 
-Alfred command can import only installed library. You can't use relative import. That makes difficult to
-share code between your commands.
+Alfred command can import only installed library. You can't use relative import. That makes difficult to share code between your commands.
 
 ## The latest version
 
 You can find the latest version to ...
 
 ```bash
 git clone https://github.com/FabienArcellier/alfred-cli.git
 ```
 
 ## Cookbook
 
-### Display the commands really executed behind the scene
+### Display the commands really executed
 
 You can display the commands really executed, either to debug the arguments,
 either to run in your terminal again with other attributes.
 
 The option `d` / `--debug` display all the shell commands that are executed by
 `alfred.run()` in your alfred command.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

