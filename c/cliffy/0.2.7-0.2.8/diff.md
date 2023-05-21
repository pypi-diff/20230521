# Comparing `tmp/cliffy-0.2.7.tar.gz` & `tmp/cliffy-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliffy-0.2.7.tar", max compression
+gzip compressed data, was "cliffy-0.2.8.tar", max compression
```

## Comparing `cliffy-0.2.7.tar` & `cliffy-0.2.8.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1060 2023-05-03 03:44:33.681462 cliffy-0.2.7/LICENSE
--rw-r--r--   0        0        0     5131 2023-05-03 03:44:33.685463 cliffy-0.2.7/README.md
--rw-r--r--   0        0        0        0 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/__init__.py
--rw-r--r--   0        0        0     4281 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/cli.py
--rw-r--r--   0        0        0        0 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/clis/__init__.py
--rw-r--r--   0        0        0     3923 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/commander.py
--rw-r--r--   0        0        0        0 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/commanders/__init__.py
--rw-r--r--   0        0        0      981 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/commanders/click.py
--rw-r--r--   0        0        0     1835 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/commanders/typer.py
--rw-r--r--   0        0        0     2758 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/helper.py
--rw-r--r--   0        0        0     3434 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/homer.py
--rw-r--r--   0        0        0     1361 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/loader.py
--rw-r--r--   0        0        0      297 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/manifests/__init__.py
--rw-r--r--   0        0        0     7441 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/manifests/v1.py
--rw-r--r--   0        0        0      137 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/merger.py
--rw-r--r--   0        0        0     4924 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/parser.py
--rw-r--r--   0        0        0      933 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/rich.py
--rw-r--r--   0        0        0       47 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/run.py
--rw-r--r--   0        0        0     3533 2023-05-03 03:44:33.685463 cliffy-0.2.7/cliffy/transformer.py
--rw-r--r--   0        0        0     1060 2023-05-03 03:44:33.685463 cliffy-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     6054 1970-01-01 00:00:00.000000 cliffy-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-05-21 17:30:19.035557 cliffy-0.2.8/LICENSE
+-rw-r--r--   0        0        0     6575 2023-05-21 17:30:19.035557 cliffy-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/__main__.py
+-rw-r--r--   0        0        0     1657 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/builder.py
+-rw-r--r--   0        0        0     6741 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/cli.py
+-rw-r--r--   0        0        0        0 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/clis/__init__.py
+-rw-r--r--   0        0        0     4072 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/commander.py
+-rw-r--r--   0        0        0        0 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/commanders/__init__.py
+-rw-r--r--   0        0        0      981 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/commanders/click.py
+-rw-r--r--   0        0        0     1939 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/commanders/typer.py
+-rw-r--r--   0        0        0     2775 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/helper.py
+-rw-r--r--   0        0        0     3030 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/homer.py
+-rw-r--r--   0        0        0     1366 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/loader.py
+-rw-r--r--   0        0        0      297 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/manifests/__init__.py
+-rw-r--r--   0        0        0     7504 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/manifests/v1.py
+-rw-r--r--   0        0        0      137 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/merger.py
+-rw-r--r--   0        0        0     4959 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/parser.py
+-rw-r--r--   0        0        0      860 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/rich.py
+-rw-r--r--   0        0        0       47 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/run.py
+-rw-r--r--   0        0        0     3515 2023-05-21 17:30:19.035557 cliffy-0.2.8/cliffy/transformer.py
+-rw-r--r--   0        0        0     1092 2023-05-21 17:30:19.039557 cliffy-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     7536 1970-01-01 00:00:00.000000 cliffy-0.2.8/PKG-INFO
```

### Comparing `cliffy-0.2.7/LICENSE` & `cliffy-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.7/README.md` & `cliffy-0.2.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,48 @@
 [![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jaykv/cliffy/python-app.yaml?branch=main)](https://github.com/jaykv/cliffy/actions)
 [![PyPI](https://img.shields.io/pypi/v/cliffy)](https://pypi.org/project/cliffy/)
 ![GitHub](https://img.shields.io/github/license/jaykv/cliffy)
 
 # cliffy :mountain:
-YAML-defined CLI generator and manager for python
+cliffy is a YAML-defined CLI generator, manager, and bundler for python. It offers dynamic abstractions to rapidly build, test, and deploy CLIs.
 
 ## Features
-* Build and generate YAML-defined CLIs
-* Dynamic abstractions to rapidly build and test CLIs
+* Generate CLIs from YAML files
 * Manage CLIs- load, list, update, and remove
-* Built-in shell and Python script support
-* Supports Jinja2-templating to create a flexible command flow
+* Built-in shell and Python scripting support
+* Supports Jinja2-templating
+* Build and bundle CLIs into self-contained, portable zipapps
 
 ## Install
-`pip install cliffy`
+* `pip install cliffy`
+
+or
+
+* `pip install "cliffy[rich]"` to include [Rich](https://github.com/Textualize/rich) for beautiful text and formatting
+
+## How it works
+1. Define CLI manifests in YAML files
+2. Run `cli` commands to load, list, update, and remove CLIs
+3. When loaded, cliffy parses the manifest and generates a [Typer](https://github.com/tiangolo/typer) CLI that is deployed directly as a script
+4. Run loaded CLIs straight from the terminal
+5. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
 
 ## Usage
 `cli <command>`
-* `init <cli name>`: Generate a template CLI manifest
+* `init <cli name>`: Generate a template CLI manifest for a new CLI
 * `load <manifest>`: Add a new CLI based on the manifest
-* `render <manifest>`: Render the YAML manifest into executable code
-* `list` or `ls`: Ouput a list of loaded CLIs 
-* `update <cli name>`: Reloads a CLI
+* `render <manifest>`: Render the CLI manifest into python code
+* `list` or `ls`: Output a list of loaded CLIs 
+* `update <cli name>`: Reload a loaded CLI
 * `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
+* `run <manifest> -- <args>`: Runs a CLI manifest as a one-time operation
+* `build <manifest>`: Build a CLI manifest into a self-contained zipapp
+* `bundle <cli name>`: Bundle a loaded CLI into a self-contained zipapp
 
-### Basic Example
+### Load
 
 1. Define a manifest
 ```yaml
 # hello.yaml
 name: hello
 version: 0.1.0
 
@@ -37,23 +51,61 @@
   python: print("hello from python")
 ```
 
 2. Load CLI
 ```
 $ cli load hello.yaml
 ```
+Parses `hello.yaml` to generate a Typer CLI and load it into the running Python environment.
 
 3. Run CLI directly
 
 `hello -h`
 
 ![hello-demo](docs/images/hello.png)
 
 For more examples, check [examples](examples/) directory.
 
+### Build
+
+1. Define a manifest
+```yaml
+# requires.yaml
+name: requires
+version: 0.1.0
+
+requires:
+  - requests >= 2.30.0
+  - six
+
+imports:
+  - import six
+
+commands:
+  bash: $echo "hello from bash"
+  python: print("hello from python")
+  py: |
+    if six.PY2:
+        print("python 2")
+    if six.PY3:
+        print("python 3")
+```
+
+2. Build CLI
+```
+$ cli build requires.yaml -o dist
+```
+
+Builds a portable zipapp containing the CLI and its package requirements.
+
+3. Run CLI
+```
+./dist/requires -h
+```
+
 ## Manifest template
 Generated by `cli init`:
 ```yaml
 # cliffy v1 template
 manifestVersion: v1
 
 # The name of the CLI
```

### Comparing `cliffy-0.2.7/cliffy/cli.py` & `cliffy-0.2.8/cliffy/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 ## CLI to generate CLIs
 import contextlib
+from tempfile import NamedTemporaryFile
 from typing import TextIO
 
 try:
-    import rich_click as click
+    import rich_click as click  # type: ignore
     from rich.console import Console
-    from rich.syntax import Syntax
-    from rich_click.rich_group import RichGroup as AliasGroup
+    from rich_click.rich_group import RichGroup as AliasGroup  # type: ignore
 except ImportError:
     import click
-    from .rich import Console, Syntax
+    from .rich import Console
     from click import Group as AliasGroup
 
-from .helper import print_rich_table, write_to_file
-from .homer import Homer
+from .builder import build_cli, run_cli
+from .helper import CLIFFY_CLI_DIR, print_rich_table, write_to_file
+from .homer import get_clis, get_metadata, get_metadata_path, remove_metadata, save_metadata
 from .loader import Loader
 from .manifests import Manifest, set_manifest_version
 from .transformer import Transformer
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 
-class AliasedGroup(AliasGroup):
+class AliasedGroup(AliasGroup):  # type: ignore
     def get_command(self, ctx, cmd_name):
         with contextlib.suppress(KeyError):
             cmd_name = ALIASES[cmd_name].name
         return super().get_command(ctx, cmd_name or "")
 
 
 @click.group(context_settings=CONTEXT_SETTINGS, cls=AliasedGroup)
@@ -36,30 +37,30 @@
 
 @cli.command()
 @click.argument('manifests', type=click.File('rb'), nargs=-1)
 def load(manifests: list[TextIO]) -> None:
     """Load CLI for given manifest(s)"""
     for manifest in manifests:
         T = Transformer(manifest)
-        Loader.load_cli(T.cli)
-        Homer.save_cli_metadata(manifest.name, T.cli)
+        Loader.load_from_cli(T.cli)
+        save_metadata(manifest.name, T.cli)
         click.secho(f"~ Generated {T.cli.name} CLI v{T.cli.version} ~", fg="green")
         click.secho(click.style("$", fg="magenta"), nl=False)
         click.echo(f" {T.cli.name} -h")
 
 
 @cli.command()
 @click.argument('cli_names', type=str, nargs=-1)
 def update(cli_names: list[str]) -> None:
     """Reloads CLI by name"""
     for cli_name in cli_names:
-        if cli_metadata := Homer.get_cli_metadata(cli_name):
+        if cli_metadata := get_metadata(cli_name):
             T = Transformer(open(cli_metadata.runner_path, "r"))
-            Loader.load_cli(T.cli)
-            Homer.save_cli_metadata(cli_metadata.runner_path, T.cli)
+            Loader.load_from_cli(T.cli)
+            save_metadata(cli_metadata.runner_path, T.cli)
             click.secho(f"~ Reloaded {T.cli.name} CLI v{T.cli.version} ~", fg="green")
             click.secho(click.style("$", fg="magenta"), nl=False)
             click.echo(f" {T.cli.name} -h")
         else:
             click.secho(f"~ {cli_name} not found", fg="red")
 
 
@@ -69,60 +70,114 @@
     """Render the CLI manifest generation as code"""
     T = Transformer(manifest)
     console = Console()
     console.print(T.cli.code, overflow="fold", emoji=False, markup=False)
     click.secho(f"# Rendered {T.cli.name} CLI v{T.cli.version} ~", fg="green")
 
 
+@cli.command("run")
+@click.argument('manifest', type=click.File('rb'))
+@click.argument('cli_args', type=str, nargs=-1)
+def cliffy_run(manifest: TextIO, cli_args: tuple[str]) -> None:
+    """Run CLI for a manifest"""
+    T = Transformer(manifest)
+    run_cli(T.cli.name, T.cli.code, cli_args)
+
+
 @cli.command()
 @click.argument('cli_name', type=str, default="cliffy")
 @click.option('--version', '-v', type=str, show_default=True, default="v1", help="Manifest version")
-@click.option(
-    '--render', type=bool, is_flag=True, show_default=True, default=False, help="Render template to terminal directly"
-)
+@click.option('--render', is_flag=True, show_default=True, default=False, help="Render template to terminal directly")
 @click.option(
     '--raw',
     type=bool,
     is_flag=True,
     show_default=True,
     default=False,
     help="Raw template without boilerplate helpers and examples.",
 )
 def init(cli_name: str, version: str, render: bool, raw: bool) -> None:
     """Generate a CLI manifest template"""
     set_manifest_version(version)
     template = Manifest.get_raw_template(cli_name) if raw else Manifest.get_template(cli_name)
 
     if render:
-        syntax = Syntax(template, "yaml", theme="monokai", line_numbers=False)
         console = Console()
-        console.print(syntax)
+        console.print(template, overflow="fold", emoji=False, markup=False)
     else:
         write_to_file(f'{cli_name}.yaml', text=template)
         click.secho(f"+ {cli_name}.yaml", fg="green")
 
 
 @cli.command("list")
-def list_clis() -> None:
+def cliffy_list() -> None:
     "List all CLIs loaded"
     cols = ["Name", "Version", "Manifest"]
-    rows = [[metadata.cli_name, metadata.version, metadata.runner_path] for metadata in Homer.get_clis()]
+    rows = [[metadata.cli_name, metadata.version, metadata.runner_path] for metadata in get_clis()]
     print_rich_table(cols, rows, styles=["cyan", "magenta", "green"])
 
 
 @cli.command()
 @click.argument('cli_names', type=str, nargs=-1)
 def remove(cli_names: list[str]) -> None:
     "Remove a loaded CLI by name"
     for cli_name in cli_names:
-        if Homer.get_cliffy_cli(cli_name):
-            Homer.remove_cli_metadata(cli_name)
+        if get_metadata_path(cli_name):
+            remove_metadata(cli_name)
             Loader.unload_cli(cli_name)
             click.secho(f"~ {cli_name} unloaded", fg="green")
         else:
-            click.secho(f"~ {cli_name} not found", fg="red")
+            click.secho(f"~ {cli_name} not loaded", fg="red")
+
+
+@cli.command()
+@click.argument('cli_names', type=str, nargs=-1)
+@click.option('--debug', is_flag=True, show_default=True, default=False, help="Display build output")
+@click.option('--output-dir', '-o', type=click.Path(file_okay=False, dir_okay=True, writable=True), help="Output dir")
+def bundle(cli_names: list[str], debug: bool, output_dir: str) -> None:
+    "Bundle a loaded CLI into a zipapp"
+    for cli_name in cli_names:
+        if not (metadata := get_metadata(cli_name)):
+            click.secho(f"~ {cli_name} not loaded", fg="red")
+            continue
+
+        result = build_cli(
+            cli_name, script_path=f'{CLIFFY_CLI_DIR}/{cli_name}.py', deps=metadata.requires, output_dir=output_dir
+        )
+
+        if result.exit_code != 0:
+            click.secho(result.stdout)
+            click.secho(f"~ {cli_name} bundle failed", fg="red", error=True)
+            continue
+
+        if debug:
+            click.secho(result.stdout)
+        click.secho(f"+ {cli_name} bundled", fg="green")
+
+
+@cli.command()
+@click.argument('manifests', type=click.File('rb'), nargs=-1)
+@click.option('--debug', is_flag=True, show_default=True, default=False, help="Display build output")
+@click.option('--output-dir', '-o', type=click.Path(file_okay=False, dir_okay=True, writable=True), help="Output dir")
+def build(manifests: list[TextIO], debug: bool, output_dir: str) -> None:
+    "Build a CLI manifest into a zipapp"
+    for manifest in manifests:
+        T = Transformer(manifest, validate_requires=False)
+        with NamedTemporaryFile(mode='w', prefix=f'{T.cli.name}_', suffix='.py', delete=True) as script:
+            script.write(T.cli.code)
+            script.flush()
+            result = build_cli(T.cli.name, script_path=script.name, deps=T.cli.requires, output_dir=output_dir)
+
+        if result.exit_code != 0:
+            click.secho(result.stdout)
+            click.secho(f"~ {T.cli.name} build failed", fg="red", error=True)
+            continue
+
+        if debug:
+            click.secho(result.stdout)
+        click.secho(f"+ {T.cli.name} built", fg="green")
 
 
 ALIASES = {
     "rm": remove,
-    "ls": list_clis,
+    "ls": cliffy_list,
 }
```

### Comparing `cliffy-0.2.7/cliffy/commander.py` & `cliffy-0.2.8/cliffy/commander.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from collections import defaultdict, namedtuple
 from typing import DefaultDict
 
 from .manifests import Manifest
 from .parser import Parser
 
 Command = namedtuple('Command', ['name', 'script'])
-CLI = namedtuple('CLI', ['name', 'version', 'code'])
+CLI = namedtuple('CLI', ['name', 'version', 'code', 'requires'])
 
 
 class Commander:
     """Generates commands based on the command config"""
 
     __slots__ = ('manifest', 'parser', 'cli', 'groups', 'greedy')
 
     def __init__(self, manifest: Manifest) -> None:
         self.manifest = manifest
         self.parser = Parser(self.manifest)
         self.cli: str = ""
         self.groups: DefaultDict[str, dict] = defaultdict(lambda: defaultdict())
-        self.greedy = []
+        self.greedy: list[Command] = []
 
     def build_cli(self) -> None:
         self.add_base_imports()
         self.add_imports()
         self.add_base_cli()
         self.add_functions()
         for name, script in self.manifest.commands.items():
             current_command = Command(name, script)
             self.add_command(current_command)
 
         self.add_greedy_commands()
+        self.add_main_block()
 
     def add_command(self, command: Command) -> None:
         # Check for greedy commands- evaluate them at the end
         if self.is_greedy(command.name):
             self.greedy.append(command)
             return
 
@@ -99,12 +100,15 @@
 
     def add_group_command(self, command: Command) -> None:
         raise NotImplementedError
 
     def add_sub_command(self, command: Command, group: str) -> None:
         raise NotImplementedError
 
+    def add_main_block(self) -> None:
+        raise NotImplementedError
+
 
 def build_cli(manifest: Manifest, commander_cls=Commander) -> CLI:
     commander = commander_cls(manifest)
     commander.build_cli()
-    return CLI(manifest.name, manifest.version, commander.cli)
+    return CLI(manifest.name, manifest.version, commander.cli, manifest.requires)
```

### Comparing `cliffy-0.2.7/cliffy/commanders/click.py` & `cliffy-0.2.8/cliffy/commanders/click.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.2.7/cliffy/commanders/typer.py` & `cliffy-0.2.8/cliffy/commanders/typer.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,7 +51,13 @@
     def add_sub_command(self, command: Command, group: str) -> None:
         self.cli += f"""
 @{group}_app.command("{self.parser.get_parsed_command_name(command)}")
 def {self.parser.get_command_func_name(command)}({self.parser.parse_args(command)}):
 {self.parser.parse_command(command.script)}
 
 """
+
+    def add_main_block(self) -> None:
+        self.cli += """
+if __name__ == "__main__":
+    cli()
+"""
```

### Comparing `cliffy-0.2.7/cliffy/helper.py` & `cliffy-0.2.8/cliffy/helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import operator
 import os
 import platform
 import subprocess
 import sys
+from importlib.resources import files
 from pathlib import Path
 from typing import Optional
 
 from packaging import version
 from pydantic import BaseModel
 
 try:
@@ -14,15 +15,15 @@
     from rich.table import Table
 except ImportError:
     from .rich import Console, Table
 
 HOME_PATH = str(Path.home())
 PYTHON_BIN = f"{sys.exec_prefix}/Scripts" if platform.system() == "Windows" else f"{sys.exec_prefix}/bin"
 PYTHON_EXECUTABLE = sys.executable
-CLIFFY_CLI_DIR = f"{Path(__file__).parent.resolve()}/clis"
+CLIFFY_CLI_DIR = files('cliffy.clis')
 CLIFFY_HOME_PATH = f"{HOME_PATH}/.cliffy"
 OPERATOR_MAP = {
     '==': operator.eq,
     '!=': operator.ne,
     '>=': operator.ge,
     '<=': operator.le,
     '<': operator.lt,
```

### Comparing `cliffy-0.2.7/cliffy/homer.py` & `cliffy-0.2.8/cliffy/homer.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,109 +7,109 @@
 from typing import Iterator, Optional
 
 from .commander import CLI
 from .helper import CLIFFY_HOME_PATH, write_to_file
 from .manifests.v1 import CLIMetadata
 
 
-class Homer:
-    @staticmethod
-    def save_cli_metadata(manifest_path: str, cli: CLI) -> None:
-        """Stores CLI metadata
-
-        Args:
-            manifest_path (str): CLI manifest path
-            cli (CLI): CLI
-        """
-        abs_manifest_path = os.path.realpath(manifest_path)
-        encoded_runnerpath = b32encode(cli.name.encode('ascii')).decode('utf-8')
-        save_metadata_path = f"{CLIFFY_HOME_PATH}/{encoded_runnerpath}/{cli.name}.json"
-        with open(manifest_path, "r") as manifest:
-            write_to_file(
-                save_metadata_path,
-                json.dumps(
-                    CLIMetadata(
-                        cli_name=cli.name,
-                        runner_path=abs_manifest_path,
-                        version=cli.version,
-                        loaded=datetime.now(),
-                        manifest=manifest.read(),
-                    ).dict(),
-                    default=str,
-                ),
-            )
-
-    @staticmethod
-    def remove_cli_metadata(cli_name: str) -> None:
-        """Clears CLI metadata by name
-
-        Args:
-            cli_name (str): CLI name
-        """
-        metadata_paths = glob.glob(f"{CLIFFY_HOME_PATH}/*/{cli_name}.*")
-        for path in metadata_paths:
-            parent_path = Path(path).parent.resolve()
-            os.remove(path)
-            os.rmdir(parent_path)
-
-    @staticmethod
-    def get_cli_metadata_bypath(path: Path) -> CLIMetadata:
-        """Fetches CLI metadata by metadata path
-
-        Args:
-            path (Path): Metadata path
-
-        Returns:
-            CLIMetadata: CLI metadata
-        """
-        try:
-            return CLIMetadata(**json.load(path.open("r")))
-        except Exception as e:
-            return CLIMetadata(
-                cli_name=path.name,
-                runner_path=path.absolute().name,
-                version="error",
-                loaded=datetime.now(),
-                manifest=f"could not load: {e}",
-            )
-
-    @classmethod
-    def get_cli_metadata(cls, cli_name: str) -> Optional[CLIMetadata]:
-        """Fetches CLI metadata by name
-
-        Args:
-            cli_name (str): CLI name
-
-        Returns:
-            Optional[CLIMetadata]: CLI metadata
-        """
-        cli_path = cls.get_cliffy_cli(cli_name)
-        if not cli_path:
-            return None
-
-        path = Path(cli_path)
-        return cls.get_cli_metadata_bypath(path)
-
-    @staticmethod
-    def get_cliffy_cli(cli_name: str) -> Optional[str]:
-        """Fetches CLI metadata path
-
-        Args:
-            cli_name (str): CLI name
-
-        Returns:
-            Optional[str]: CLI metadata path
-        """
-        if cli_metadata_path := glob.glob(f"{CLIFFY_HOME_PATH}/*/{cli_name}.json"):
-            return cli_metadata_path[0]
+def save_metadata(manifest_path: str, cli: CLI) -> None:
+    """Stores CLI metadata
+
+    Args:
+        manifest_path (str): CLI manifest path
+        cli (CLI): CLI
+    """
+    abs_manifest_path = os.path.realpath(manifest_path)
+    encoded_runnerpath = b32encode(cli.name.encode('ascii')).decode('utf-8')
+    save_metadata_path = f"{CLIFFY_HOME_PATH}/{encoded_runnerpath}/{cli.name}.json"
+    with open(manifest_path, "r") as manifest:
+        write_to_file(
+            save_metadata_path,
+            json.dumps(
+                CLIMetadata(
+                    cli_name=cli.name,
+                    runner_path=abs_manifest_path,
+                    version=cli.version,
+                    loaded=datetime.now(),
+                    manifest=manifest.read(),
+                    requires=cli.requires,
+                ).dict(),
+                default=str,
+            ),
+        )
+
+
+def remove_metadata(cli_name: str) -> None:
+    """Clears CLI metadata by name
+
+    Args:
+        cli_name (str): CLI name
+    """
+    metadata_paths = glob.glob(f"{CLIFFY_HOME_PATH}/*/{cli_name}.*")
+    for path in metadata_paths:
+        parent_path = Path(path).parent.resolve()
+        os.remove(path)
+        os.rmdir(parent_path)
+
+
+def get_metadata_bypath(path: Path) -> CLIMetadata:
+    """Fetches CLI metadata by metadata path
+
+    Args:
+        path (Path): Metadata path
+
+    Returns:
+        CLIMetadata: CLI metadata
+    """
+    try:
+        return CLIMetadata(**json.load(path.open("r")))
+    except Exception as e:
+        return CLIMetadata(
+            cli_name=path.name,
+            runner_path=path.absolute().name,
+            version="error",
+            loaded=datetime.now(),
+            manifest=f"could not load: {e}",
+            requires=[],
+        )
+
+
+def get_metadata(cli_name: str) -> Optional[CLIMetadata]:
+    """Fetches CLI metadata by name
+
+    Args:
+        cli_name (str): CLI name
+
+    Returns:
+        Optional[CLIMetadata]: CLI metadata
+    """
+    cli_path = get_metadata_path(cli_name)
+    if not cli_path:
         return None
 
-    @classmethod
-    def get_clis(cls) -> Iterator[CLIMetadata]:
-        """Fetches loaded CLIs metadata iteratively
-
-        Yields:
-            Iterator[CLIMetadata]: CLI metadata
-        """
-        metadata_paths = Path(CLIFFY_HOME_PATH).glob('*/*')
-        for metadata_path in metadata_paths:
-            yield cls.get_cli_metadata_bypath(metadata_path)
+    path = Path(cli_path)
+    return get_metadata_bypath(path)
+
+
+def get_metadata_path(cli_name: str) -> Optional[str]:
+    """Fetches CLI metadata path
+
+    Args:
+        cli_name (str): CLI name
+
+    Returns:
+        Optional[str]: CLI metadata path
+    """
+    if cli_metadata_path := glob.glob(f"{CLIFFY_HOME_PATH}/*/{cli_name}.json"):
+        return cli_metadata_path[0]
+    return None
+
+
+def get_clis() -> Iterator[CLIMetadata]:
+    """Fetches loaded CLIs metadata iteratively
+
+    Yields:
+        Iterator[CLIMetadata]: CLI metadata
+    """
+    metadata_paths = Path(CLIFFY_HOME_PATH).glob('*/*')
+    for metadata_path in metadata_paths:
+        yield get_metadata_bypath(metadata_path)
```

### Comparing `cliffy-0.2.7/cliffy/loader.py` & `cliffy-0.2.8/cliffy/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     def deploy_script(self) -> str:
         script_path = Loader.get_cli_script_path(self.cli.name)
         write_to_file(script_path, Loader.get_cli_script(self.cli.name), executable=True)
         return script_path
 
     @classmethod
-    def load_cli(cls, cli: CLI) -> None:
+    def load_from_cli(cls, cli: CLI) -> None:
         L = cls(cli)
         L.deploy_script()
         L.deploy_cli()
 
     @classmethod
     def unload_cli(cls, cli_name) -> None:
         with contextlib.suppress(FileNotFoundError):
```

### Comparing `cliffy-0.2.7/cliffy/manifests/v1.py` & `cliffy-0.2.8/cliffy/manifests/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     )
     help: str = Field(
         "",
         description="A brief description of the CLI that is displayed when the user invokes the --help or -h option.",
     )
     requires: list[str] = Field(
         [],
-        description="List of Python dependencies required for the CLI. Validated on CLI load and update. "
+        description="List of Python dependencies required for the CLI. Validated on CLI load, update and build. "
         "Supports basic requirements specifier syntax.",
     )
     includes: list[str] = Field(
         [],
         description="List of external CLI manifest paths to include into the main manifest. "
         "Performs a deep merge of manifests sequentially in the order given to assemble a merged manifest. "
         "and finally, deep merges the merged manifest with the main manifest.",
@@ -53,15 +53,15 @@
     )
     functions: list[str] = Field(
         [],
         description="A list containing any helper functions. "
         "Each element of the list can be a separate function. "
         "These functions should be defined as strings that can be executed by the Python interpreter.",
     )
-    args: dict[str, list] = Field(
+    args: dict[str, list[dict[str, str]]] = Field(
         {},
         description="A mapping containing the arguments and options for each command. "
         "Each key in the mapping should correspond to a command in the commands section. "
         "The value should be a list of mappings representing the params and options for that command.",
     )
     types: dict[str, str] = Field(
         {},
@@ -187,21 +187,22 @@
 
 class IncludeManifest(BaseModel):
     """Special manifest specifically to define the allowed named objects that can be included"""
 
     commands: dict[str, Union[str, list[Union[str, dict[Literal['help'], str]]]]] = {}
     imports: Union[str, list[str]] = []
     functions: list[str] = []
-    args: dict[str, list] = {}
+    args: dict[str, list[dict[str, str]]] = {}
     types: dict[str, str] = {}
     cli_options: dict[str, str] = {}
     requires: list[str]
 
 
 class CLIMetadata(BaseModel):
     """Metadata model"""
 
     cli_name: str
     runner_path: str
     version: str
     loaded: datetime
     manifest: str
+    requires: list[str]
```

### Comparing `cliffy-0.2.7/cliffy/parser.py` & `cliffy-0.2.8/cliffy/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## Command parser
 from typing import Any, Literal, Optional, Tuple, Union
 
-import pybash
+from pybash.transformer import transform as transform_bash
 
 from .manifests import Manifest
 
 
 class Parser:
     def __init__(self, manifest: Manifest) -> None:
         self.manifest = manifest
@@ -33,15 +33,15 @@
         return base_param_name, aliases
 
     def parse_command_block(self, script: str):
         ## Bash commands start with $
         if script.startswith('$'):
             script = script.replace('$ ', '$', 1)
             script = f'>{script[1:]}'
-            return " " * 4 + pybash.Transformer.transform_source(script)
+            return " " * 4 + transform_bash(script)
 
         return "".join(" " * 4 + line + "\n" for line in script.split('\n'))
 
     def parse_command(self, block: Union[str, list[Union[str, dict[Literal['help'], str]]]]) -> str:
         if isinstance(block, list):
             script_block = []
             help_text = ""
@@ -83,15 +83,15 @@
         parsed_arg_type += '),'
         return parsed_arg_type
 
     def parse_arg(self, arg_name: str, arg_type: str) -> str:
         is_required = self.is_param_required(arg_type)
         default_val = self.get_default_param_val(arg_type)
         param_type = 'Option' if self.is_param_option(arg_name) else 'Argument'
-        arg_aliases = []
+        arg_aliases: list[str] = []
 
         # extract default val before parsing it
         if '=' in arg_type:
             arg_type = arg_type.split('=')[0].strip()
 
         # strip - before parsing it
         if self.is_param_option(arg_name):
```

### Comparing `cliffy-0.2.7/cliffy/rich.py` & `cliffy-0.2.8/cliffy/rich.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 ## Mimic rich API methods for rich-less support
+from typing import Union
+
 import click
 
 
 class Console:
     def __init__(self) -> None:
         pass
 
     def print(self, text, **kwargs) -> None:
         if isinstance(text, Table):
             click.echo(text)
         else:
             print(text)
 
 
-class Syntax:
-    def __init__(self, text, *args, **kwargs) -> None:
-        self.text = text
-
-    def __str__(self) -> str:
-        return self.text
-
-
 class Table:
     def __init__(self) -> None:
-        self.cols = []
-        self.rows = []
+        self.cols: list[str] = []
+        self.rows: list[list[str]] = []
 
-    def add_column(self, col, style=None) -> None:
+    def add_column(self, col: str, style: Union[str, None] = None) -> None:
         self.cols.append(col)
 
     def add_row(self, *row) -> None:
         self.rows.append([*row])
 
     def __str__(self) -> str:
         text = "".join([click.style(f"{col:10}", fg="magenta") for col in self.cols]) + "\n"
```

### Comparing `cliffy-0.2.7/cliffy/transformer.py` & `cliffy-0.2.8/cliffy/transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import os
-from typing import Literal, TextIO
+from typing import Any, TextIO
 
 import yaml
-from jinja2 import BaseLoader, Environment, FileSystemLoader, Undefined
+from jinja2 import BaseLoader, Environment, FileSystemLoader
 from typing_extensions import Self
 
 from .commander import build_cli
 from .commanders.typer import TyperCommander
 from .helper import compare_versions, get_installed_pip_packages, parse_requirement
 from .manifests import IncludeManifest, Manifest, set_manifest_version
 from .merger import cliffy_merger
 
 
 class Transformer:
     """Loads command manifest and transforms it into a CLI"""
 
-    def __init__(self, manifest_io: TextIO, as_include: bool = False) -> None:
+    def __init__(self, manifest_io: TextIO, as_include: bool = False, validate_requires: bool = True) -> None:
         self.manifest_io = manifest_io
         self.command_config = self.load_manifest(manifest_io)
         self.manifest_version = self.command_config.pop('manifestVersion', 'v1')
 
         if self.command_config.get("includes"):
             self.includes_config = self.resolve_includes()
             cliffy_merger.merge(self.command_config, self.includes_config)
 
         set_manifest_version(self.manifest_version)
         if as_include:
             self.manifest = IncludeManifest(**self.command_config)
         else:
             self.manifest = Manifest(**self.command_config)
-            self.validate_cli_requires()
+            if validate_requires:
+                self.validate_cli_requires()
             self.cli = build_cli(self.manifest, commander_cls=TyperCommander)
 
     def validate_cli_requires(self) -> None:
         if not self.manifest.requires:
             return
 
         installed_pip_packages = get_installed_pip_packages()
@@ -54,38 +55,33 @@
                 raise SystemExit(
                     f"MissingRequirement: CLI requires `{dep}`, "
                     f"found version {installed_pip_packages[dep_spec.name]}"
                 )
 
     def resolve_includes(self) -> dict:
         include_transforms = map(self.resolve_include_by_path, set(self.command_config['includes']))
-        merged_config = {}
+        merged_config: dict[str, Any] = {}
         for transformed_include in include_transforms:
             cliffy_merger.merge(merged_config, transformed_include.command_config)
 
         return merged_config
 
     @classmethod
     def resolve_include_by_path(cls, path) -> Self:
         with open(path, "r") as m:
             return cls(m, as_include=True)
 
     @staticmethod
-    def load_manifest(manifest_io: TextIO) -> dict:
+    def load_manifest(manifest_io: TextIO) -> dict[str, Any]:
         try:
             manifest_path = os.path.realpath(manifest_io.name)
             all_vars = yaml.safe_load(open(manifest_path, "r")).get('vars', {})
             var_env = Environment(loader=BaseLoader())
             interpolated_vars = {
                 var_env.from_string(str(k)).render(all_vars): var_env.from_string(str(v)).render(all_vars)
                 for k, v in all_vars.items()
             }
             manifest_env = Environment(loader=FileSystemLoader(manifest_path)).get_template("")
             return yaml.safe_load(manifest_env.render(interpolated_vars))
         except yaml.YAMLError as e:
             print("load_manifest", e)
             raise
-
-
-class NullUndefined(Undefined):
-    def __getattr__(self, key) -> Literal['']:
-        return ''
```

### Comparing `cliffy-0.2.7/pyproject.toml` & `cliffy-0.2.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 [tool.poetry]
 name = "cliffy"
-version = "0.2.7"
+version = "0.2.8"
 description = "$ cli load from.yaml"
 authors = ["Jay <jay.github0@gmail.com>"]
 repository = "https://github.com/jaykv/cliffy"
 readme = "README.md"
 packages = [{include = "cliffy"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pybash = "^0.2.5"
+pybash = "^0.3.0"
 pyyaml = "^6.0"
-typer = "^0.8.0"
+typer = "^0.9.0"
 pydantic = "^1.10.7"
 deepmerge = "^1.1.0"
 jinja2 = "^3.1.2"
 packaging = "^23.1"
 rich-click = { version = "^1.6.1", optional = true }
 shellingham = { version = "^1.5.0.post1", optional = true }
+shiv = "^1.0.3"
 
 [tool.poetry.extras]
 rich = ["rich-click", "shellingham"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 pytest = "^7.2.1"
 isort = "^5.11.4"
 flake8 = "^6.0.0"
 autoflake = "^2.0.0"
 ruff = "^0.0.254"
+mypy = "^1.3.0"
 
 [tool.poetry.scripts]
 cli = "cliffy.run:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cliffy-0.2.7/PKG-INFO` & `cliffy-0.2.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,74 @@
 Metadata-Version: 2.1
 Name: cliffy
-Version: 0.2.7
+Version: 0.2.8
 Summary: $ cli load from.yaml
 Home-page: https://github.com/jaykv/cliffy
 Author: Jay
 Author-email: jay.github0@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: rich
 Requires-Dist: deepmerge (>=1.1.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: packaging (>=23.1,<24.0)
-Requires-Dist: pybash (>=0.2.5,<0.3.0)
+Requires-Dist: pybash (>=0.3.0,<0.4.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0) ; extra == "rich"
 Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0) ; extra == "rich"
-Requires-Dist: typer (>=0.8.0,<0.9.0)
+Requires-Dist: shiv (>=1.0.3,<2.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/jaykv/cliffy
 Description-Content-Type: text/markdown
 
 [![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jaykv/cliffy/python-app.yaml?branch=main)](https://github.com/jaykv/cliffy/actions)
 [![PyPI](https://img.shields.io/pypi/v/cliffy)](https://pypi.org/project/cliffy/)
 ![GitHub](https://img.shields.io/github/license/jaykv/cliffy)
 
 # cliffy :mountain:
-YAML-defined CLI generator and manager for python
+cliffy is a YAML-defined CLI generator, manager, and bundler for python. It offers dynamic abstractions to rapidly build, test, and deploy CLIs.
 
 ## Features
-* Build and generate YAML-defined CLIs
-* Dynamic abstractions to rapidly build and test CLIs
+* Generate CLIs from YAML files
 * Manage CLIs- load, list, update, and remove
-* Built-in shell and Python script support
-* Supports Jinja2-templating to create a flexible command flow
+* Built-in shell and Python scripting support
+* Supports Jinja2-templating
+* Build and bundle CLIs into self-contained, portable zipapps
 
 ## Install
-`pip install cliffy`
+* `pip install cliffy`
+
+or
+
+* `pip install "cliffy[rich]"` to include [Rich](https://github.com/Textualize/rich) for beautiful text and formatting
+
+## How it works
+1. Define CLI manifests in YAML files
+2. Run `cli` commands to load, list, update, and remove CLIs
+3. When loaded, cliffy parses the manifest and generates a [Typer](https://github.com/tiangolo/typer) CLI that is deployed directly as a script
+4. Run loaded CLIs straight from the terminal
+5. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
 
 ## Usage
 `cli <command>`
-* `init <cli name>`: Generate a template CLI manifest
+* `init <cli name>`: Generate a template CLI manifest for a new CLI
 * `load <manifest>`: Add a new CLI based on the manifest
-* `render <manifest>`: Render the YAML manifest into executable code
-* `list` or `ls`: Ouput a list of loaded CLIs 
-* `update <cli name>`: Reloads a CLI
+* `render <manifest>`: Render the CLI manifest into python code
+* `list` or `ls`: Output a list of loaded CLIs 
+* `update <cli name>`: Reload a loaded CLI
 * `remove <cli name>` or `rm <cli name>`: Remove a loaded CLI
+* `run <manifest> -- <args>`: Runs a CLI manifest as a one-time operation
+* `build <manifest>`: Build a CLI manifest into a self-contained zipapp
+* `bundle <cli name>`: Bundle a loaded CLI into a self-contained zipapp
 
-### Basic Example
+### Load
 
 1. Define a manifest
 ```yaml
 # hello.yaml
 name: hello
 version: 0.1.0
 
@@ -62,23 +77,61 @@
   python: print("hello from python")
 ```
 
 2. Load CLI
 ```
 $ cli load hello.yaml
 ```
+Parses `hello.yaml` to generate a Typer CLI and load it into the running Python environment.
 
 3. Run CLI directly
 
 `hello -h`
 
 ![hello-demo](docs/images/hello.png)
 
 For more examples, check [examples](examples/) directory.
 
+### Build
+
+1. Define a manifest
+```yaml
+# requires.yaml
+name: requires
+version: 0.1.0
+
+requires:
+  - requests >= 2.30.0
+  - six
+
+imports:
+  - import six
+
+commands:
+  bash: $echo "hello from bash"
+  python: print("hello from python")
+  py: |
+    if six.PY2:
+        print("python 2")
+    if six.PY3:
+        print("python 3")
+```
+
+2. Build CLI
+```
+$ cli build requires.yaml -o dist
+```
+
+Builds a portable zipapp containing the CLI and its package requirements.
+
+3. Run CLI
+```
+./dist/requires -h
+```
+
 ## Manifest template
 Generated by `cli init`:
 ```yaml
 # cliffy v1 template
 manifestVersion: v1
 
 # The name of the CLI
```

