# Comparing `tmp/tbump-6.8.0.tar.gz` & `tmp/tbump-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tbump-6.8.0.tar", max compression
+gzip compressed data, was "tbump-6.9.0.tar", max compression
```

## Comparing `tbump-6.8.0.tar` & `tbump-6.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1507 2021-12-17 08:47:38.679625 tbump-6.8.0/LICENSE
--rw-r--r--   0        0        0     8138 2021-12-22 19:36:23.282586 tbump-6.8.0/README.rst
--rw-r--r--   0        0        0     1105 2022-03-27 12:37:33.915185 tbump-6.8.0/pyproject.toml
--rw-r--r--   0        0        0       55 2021-12-22 19:14:16.877259 tbump-6.8.0/tbump/__init__.py
--rw-r--r--   0        0        0       35 2022-03-27 12:36:25.643493 tbump-6.8.0/tbump/__main__.py
--rw-r--r--   0        0        0      231 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/action.py
--rw-r--r--   0        0        0     6021 2022-03-27 12:37:33.919185 tbump-6.8.0/tbump/cli.py
--rw-r--r--   0        0        0     9757 2022-03-27 12:19:29.131678 tbump-6.8.0/tbump/config.py
--rw-r--r--   0        0        0      201 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/error.py
--rw-r--r--   0        0        0     3584 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/executor.py
--rw-r--r--   0        0        0     9569 2021-12-22 19:36:23.286586 tbump-6.8.0/tbump/file_bumper.py
--rw-r--r--   0        0        0     2165 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/git.py
--rw-r--r--   0        0        0     5300 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/git_bumper.py
--rw-r--r--   0        0        0     2518 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/hooks.py
--rw-r--r--   0        0        0     3062 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/init.py
--rw-r--r--   0        0        0        0 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/py.typed
--rw-r--r--   0        0        0        0 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/__init__.py
--rw-r--r--   0        0        0     1947 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/conftest.py
--rw-r--r--   0        0        0       15 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/project/VERSION
--rw-r--r--   0        0        0      266 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/project/after.py
--rw-r--r--   0        0        0      331 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/project/before.py
--rw-r--r--   0        0        0       99 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/project/glob-one.c
--rw-r--r--   0        0        0       75 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/project/glob-two.v
--rw-r--r--   0        0        0      146 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/project/package.json
--rw-r--r--   0        0        0       42 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/project/pub.js
--rw-r--r--   0        0        0      786 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/project/tbump.toml
--rw-r--r--   0        0        0       38 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/project/version_info.py
--rw-r--r--   0        0        0       95 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/project/yarn.lock
--rw-r--r--   0        0        0        0 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/pyproject/README.rst
--rw-r--r--   0        0        0       22 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/pyproject/foo/__init__.py
--rw-r--r--   0        0        0      690 2021-12-17 08:47:38.683625 tbump-6.8.0/tbump/test/pyproject/pyproject.toml
--rw-r--r--   0        0        0      525 2021-12-17 08:47:38.687625 tbump-6.8.0/tbump/test/test_api.py
--rw-r--r--   0        0        0    12212 2021-12-17 08:47:38.687625 tbump-6.8.0/tbump/test/test_cli.py
--rw-r--r--   0        0        0     7669 2021-12-22 19:32:39.135079 tbump-6.8.0/tbump/test/test_config.py
--rw-r--r--   0        0        0     5919 2021-12-17 08:47:38.687625 tbump-6.8.0/tbump/test/test_file_bumper.py
--rw-r--r--   0        0        0     1680 2021-12-17 08:47:38.687625 tbump-6.8.0/tbump/test/test_git_bumper.py
--rw-r--r--   0        0        0     2739 2021-12-17 08:47:38.687625 tbump-6.8.0/tbump/test/test_hooks.py
--rw-r--r--   0        0        0     1663 2021-12-17 08:47:38.687625 tbump-6.8.0/tbump/test/test_init.py
--rw-r--r--   0        0        0     9360 2022-03-27 12:37:53.379662 tbump-6.8.0/setup.py
--rw-r--r--   0        0        0     9078 2022-03-27 12:37:53.380373 tbump-6.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1507 2021-12-17 08:47:38.679625 tbump-6.9.0/LICENSE
+-rw-r--r--   0        0        0     8260 2022-05-14 13:25:09.676409 tbump-6.9.0/README.rst
+-rw-r--r--   0        0        0     1105 2022-05-14 14:57:59.198834 tbump-6.9.0/pyproject.toml
+-rw-r--r--   0        0        0       55 2021-12-22 19:14:16.877259 tbump-6.9.0/tbump/__init__.py
+-rw-r--r--   0        0        0       35 2022-03-27 12:36:25.643493 tbump-6.9.0/tbump/__main__.py
+-rw-r--r--   0        0        0      231 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/action.py
+-rw-r--r--   0        0        0     7409 2022-05-14 14:57:59.198834 tbump-6.9.0/tbump/cli.py
+-rw-r--r--   0        0        0     9757 2022-03-27 12:19:29.131678 tbump-6.9.0/tbump/config.py
+-rw-r--r--   0        0        0      201 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/error.py
+-rw-r--r--   0        0        0     3584 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/executor.py
+-rw-r--r--   0        0        0     9569 2021-12-22 19:36:23.286586 tbump-6.9.0/tbump/file_bumper.py
+-rw-r--r--   0        0        0     2165 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/git.py
+-rw-r--r--   0        0        0     5300 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/git_bumper.py
+-rw-r--r--   0        0        0     2518 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/hooks.py
+-rw-r--r--   0        0        0     3062 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/init.py
+-rw-r--r--   0        0        0        0 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/py.typed
+-rw-r--r--   0        0        0        0 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/__init__.py
+-rw-r--r--   0        0        0     1947 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/conftest.py
+-rw-r--r--   0        0        0       15 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/project/VERSION
+-rw-r--r--   0        0        0      266 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/project/after.py
+-rw-r--r--   0        0        0      331 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/project/before.py
+-rw-r--r--   0        0        0       99 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/project/glob-one.c
+-rw-r--r--   0        0        0       75 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/project/glob-two.v
+-rw-r--r--   0        0        0      146 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/project/package.json
+-rw-r--r--   0        0        0       42 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/project/pub.js
+-rw-r--r--   0        0        0      786 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/project/tbump.toml
+-rw-r--r--   0        0        0       38 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/project/version_info.py
+-rw-r--r--   0        0        0       95 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/project/yarn.lock
+-rw-r--r--   0        0        0        0 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/pyproject/README.rst
+-rw-r--r--   0        0        0       22 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/pyproject/foo/__init__.py
+-rw-r--r--   0        0        0      690 2021-12-17 08:47:38.683625 tbump-6.9.0/tbump/test/pyproject/pyproject.toml
+-rw-r--r--   0        0        0      525 2021-12-17 08:47:38.687625 tbump-6.9.0/tbump/test/test_api.py
+-rw-r--r--   0        0        0    12468 2022-05-14 14:41:27.329075 tbump-6.9.0/tbump/test/test_cli.py
+-rw-r--r--   0        0        0     7669 2021-12-22 19:32:39.135079 tbump-6.9.0/tbump/test/test_config.py
+-rw-r--r--   0        0        0     5919 2021-12-17 08:47:38.687625 tbump-6.9.0/tbump/test/test_file_bumper.py
+-rw-r--r--   0        0        0     1680 2021-12-17 08:47:38.687625 tbump-6.9.0/tbump/test/test_git_bumper.py
+-rw-r--r--   0        0        0     2739 2021-12-17 08:47:38.687625 tbump-6.9.0/tbump/test/test_hooks.py
+-rw-r--r--   0        0        0     1663 2021-12-17 08:47:38.687625 tbump-6.9.0/tbump/test/test_init.py
+-rw-r--r--   0        0        0     9488 2022-05-14 14:58:16.557157 tbump-6.9.0/setup.py
+-rw-r--r--   0        0        0     9200 2022-05-14 14:58:16.557892 tbump-6.9.0/PKG-INFO
```

### Comparing `tbump-6.8.0/LICENSE` & `tbump-6.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/README.rst` & `tbump-6.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,20 @@
 * Push the current branch and the tag.
 
 Note that by default, ``tbump`` will display all the changes and stop to ask if they are correct before performing any action, allowing you to abort and re-try the bump if something is not right.
 You can use ``--non-interactive`` to disable this behavior.
 
 If you only want to bump the files without performing any git actions or running the hook commands, use the ``--only-patch`` option.
 
+The current version of the project can be found using the command:
+
+.. code-block:: console
+
+    $ tbump current-version
+
 Advanced configuration
 ----------------------
 
 Restricting the lines that are replaced
 +++++++++++++++++++++++++++++++++++++++
```

### Comparing `tbump-6.8.0/pyproject.toml` & `tbump-6.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "tbump"
-version = "6.8.0"
+version = "6.9.0"
 description = "Bump software releases"
 readme = "README.rst"
 authors = ["Dimitri Merejkowsky <dimitri@dmerej.info>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/dmerejkowsky/tbump"
 
 [tool.poetry.urls]
```

### Comparing `tbump-6.8.0/tbump/cli.py` & `tbump-6.9.0/tbump/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import sys
 import textwrap
 import urllib.parse
 from dataclasses import dataclass
 from pathlib import Path
-from typing import List, Optional
+from typing import Dict, List, Optional
 
 import cli_ui as ui
 import docopt
 
 from tbump.config import get_config_file
 from tbump.error import Error
 from tbump.executor import Executor
 from tbump.file_bumper import FileBumper
 from tbump.git import GitError
 from tbump.git_bumper import GitBumper
 from tbump.hooks import HooksRunner
 from tbump.init import init
 
-TBUMP_VERSION = "6.8.0"
+TBUMP_VERSION = "6.9.0"
 
 USAGE = textwrap.dedent(
     """
 Usage:
   tbump [options] <new_version>
+  tbump [options] current-version
   tbump [options] init [--pyproject] <current_version>
   tbump --help
   tbump --version
 
 Options:
    -h --help          Show this screen.
    -v --version       Show version.
@@ -52,74 +53,117 @@
     working_path: Path
     new_version: str
     interactive: bool = True
     dry_run: bool = False
     config_path: Optional[Path] = None
 
 
+@dataclass
+class Arguments:
+    dry_run: bool
+    interactive: bool
+    current_version: str
+    new_version: str
+    run_init: bool
+    show_version: bool
+    specified_config_path: Optional[Path]
+    working_path: Path
+    use_pyproject: bool
+    operations: List[str]
+
+    @classmethod
+    def from_opts(cls, opt_dict: Dict[str, str]) -> "Arguments":
+        config_opt = opt_dict["--config"]
+        if config_opt:
+            specified_config_path: Optional[Path] = Path(config_opt)
+        else:
+            specified_config_path = None
+        if opt_dict["--cwd"]:
+            working_path = Path(opt_dict["--cwd"])
+        else:
+            working_path = Path.cwd()
+
+        operations = ["patch", "hooks", "commit", "tag", "push_commit", "push_tag"]
+        if opt_dict["--only-patch"]:
+            operations = ["patch"]
+        if opt_dict["--no-push"]:
+            operations.remove("push_commit")
+            operations.remove("push_tag")
+        if opt_dict["--no-tag-push"]:
+            operations.remove("push_tag")
+        if opt_dict["--no-tag"]:
+            operations.remove("tag")
+            # Also remove push_tag if it's still in the list:
+            if "push_tag" in operations:
+                operations.remove("push_tag")
+
+        return cls(
+            current_version=opt_dict["<current_version>"],
+            show_version=bool(opt_dict["--version"]),
+            new_version=opt_dict["<new_version>"],
+            specified_config_path=specified_config_path,
+            use_pyproject=bool(opt_dict["--pyproject"]),
+            working_path=working_path,
+            run_init=bool(opt_dict["init"]),
+            dry_run=bool(opt_dict["--dry-run"]),
+            interactive=not opt_dict["--non-interactive"],
+            operations=operations,
+        )
+
+
 def run(cmd: List[str]) -> None:
     opt_dict = docopt.docopt(USAGE, argv=cmd)
-    if opt_dict["--version"]:
+    arguments = Arguments.from_opts(opt_dict)
+
+    if arguments.show_version:
         print("tbump", TBUMP_VERSION)
         return
 
     # when running `tbump init` (with current_version missing),
     # docopt thinks we are running `tbump` with new_version = "init"
     # bail out early in this case
-    if opt_dict["<new_version>"] == "init":
+    if arguments.new_version == "init":
         sys.exit(USAGE)
 
-    config_opt = opt_dict["--config"]
-    if config_opt:
-        specified_config_path: Optional[Path] = Path(config_opt)
-    else:
-        specified_config_path = None
-
-    if opt_dict["--cwd"]:
-        working_path = Path(opt_dict["--cwd"])
-    else:
-        working_path = Path.cwd()
-
-    if opt_dict["init"]:
-        current_version = opt_dict["<current_version>"]
-        use_pyproject = opt_dict["--pyproject"]
-
-        init(
-            working_path,
-            current_version=current_version,
-            use_pyproject=use_pyproject,
-            specified_config_path=specified_config_path,
+    # Ditto for `tbump current-version`
+    if arguments.new_version == "current-version":
+        config_file = get_config_file(
+            arguments.working_path,
+            specified_config_path=arguments.specified_config_path,
         )
+        config = config_file.get_config()
+        print(config.current_version)
+        return
+
+    if arguments.run_init:
+        run_init(arguments)
         return
 
-    new_version = opt_dict["<new_version>"]
+    run_bump(arguments)
+
+
+def run_init(arguments: Arguments) -> None:
+    init(
+        arguments.working_path,
+        current_version=arguments.current_version,
+        use_pyproject=arguments.use_pyproject,
+        specified_config_path=arguments.specified_config_path,
+    )
+
+
+def run_bump(arguments: Arguments) -> None:
     bump_options = BumpOptions(
-        working_path=working_path,
-        new_version=new_version,
-        config_path=specified_config_path,
+        working_path=arguments.working_path,
+        new_version=arguments.new_version,
+        config_path=arguments.specified_config_path,
+        dry_run=arguments.dry_run,
+        interactive=arguments.interactive,
     )
-    if opt_dict["--dry-run"]:
-        bump_options.dry_run = True
-    if opt_dict["--non-interactive"]:
-        bump_options.interactive = False
-
-    operations = ["patch", "hooks", "commit", "tag", "push_commit", "push_tag"]
-    if opt_dict["--only-patch"]:
-        operations = ["patch"]
-    if opt_dict["--no-push"]:
-        operations.remove("push_commit")
-        operations.remove("push_tag")
-    if opt_dict["--no-tag-push"]:
-        operations.remove("push_tag")
-    if opt_dict["--no-tag"]:
-        operations.remove("tag")
-        # Also remove push_tag if it's still in the list:
-        if "push_tag" in operations:
-            operations.remove("push_tag")
-    bump(bump_options, operations)
+
+    bump(bump_options, arguments.operations)
 
 
 def bump(options: BumpOptions, operations: List[str]) -> None:
     working_path = options.working_path
     new_version = options.new_version
     interactive = options.interactive
     dry_run = options.dry_run
```

### Comparing `tbump-6.8.0/tbump/config.py` & `tbump-6.9.0/tbump/config.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/executor.py` & `tbump-6.9.0/tbump/executor.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/file_bumper.py` & `tbump-6.9.0/tbump/file_bumper.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/git.py` & `tbump-6.9.0/tbump/git.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/git_bumper.py` & `tbump-6.9.0/tbump/git_bumper.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/hooks.py` & `tbump-6.9.0/tbump/hooks.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/init.py` & `tbump-6.9.0/tbump/init.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/test/conftest.py` & `tbump-6.9.0/tbump/test/conftest.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/test/project/tbump.toml` & `tbump-6.9.0/tbump/test/project/tbump.toml`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/test/pyproject/pyproject.toml` & `tbump-6.9.0/tbump/test/pyproject/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/test/test_api.py` & `tbump-6.9.0/tbump/test/test_api.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/test/test_cli.py` & `tbump-6.9.0/tbump/test/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,21 @@
             not tag_created(test_repo),
             not branch_pushed(test_repo, previous_commit),
             not tag_pushed(test_repo),
         )
     )
 
 
+def test_get_current_version(test_repo: Path, capsys: pytest.CaptureFixture) -> None:
+    run_tbump(["-C", str(test_repo), "current-version"])
+    captured = capsys.readouterr()
+    assert captured.out == "1.2.41-alpha-1\n"
+    assert captured.err == ""
+
+
 def test_end_to_end_using_tbump_toml(test_repo: Path) -> None:
     _, previous_commit = run_git_captured(test_repo, "rev-parse", "HEAD")
     run_tbump(["-C", str(test_repo), "1.2.41-alpha-2", "--non-interactive"])
 
     assert bump_done(test_repo, previous_commit)
```

### Comparing `tbump-6.8.0/tbump/test/test_config.py` & `tbump-6.9.0/tbump/test/test_config.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/test/test_file_bumper.py` & `tbump-6.9.0/tbump/test/test_file_bumper.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/test/test_git_bumper.py` & `tbump-6.9.0/tbump/test/test_git_bumper.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/test/test_hooks.py` & `tbump-6.9.0/tbump/test/test_hooks.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/tbump/test/test_init.py` & `tbump-6.9.0/tbump/test/test_init.py`

 * *Files identical despite different names*

### Comparing `tbump-6.8.0/setup.py` & `tbump-6.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'tomlkit>=0.5.8']
 
 entry_points = \
 {'console_scripts': ['tbump = tbump.cli:main']}
 
 setup_kwargs = {
     'name': 'tbump',
-    'version': '6.8.0',
+    'version': '6.9.0',
     'description': 'Bump software releases',
-    'long_description': '.. image:: https://img.shields.io/pypi/v/tbump.svg\n  :target: https://pypi.org/project/tbump/\n\n.. image:: https://img.shields.io/github/license/dmerejkowsky/tbump.svg\n  :target: https://github.com/dmerejkowsky/tbump/blob/main/LICENSE\n\n.. image:: https://github.com/dmerejkowsky/tbump/workflows/tests/badge.svg\n   :target: https://github.com/dmerejkowsky/tbump/actions\n\n.. image:: https://github.com/dmerejkowsky/tbump/workflows/linters/badge.svg\n   :target: https://github.com/dmerejkowsky/tbump/actions\n\n.. image:: https://img.shields.io/badge/deps%20scanning-pyup.io-green\n   :target: https://github.com/dmerejkowsky/tbump/workflows/safety/\n\n.. image:: https://img.shields.io/badge/code%20style-black-black.svg\n   :target: https://github.com/psf/black\n\n.. image:: https://img.shields.io/badge/mypy-checked-blue.svg\n   :target: https://mypy-lang.org\n\n\ntbump: bump software releases\n=============================\n\ntbump helps you bump the version of your project in a easy way.\n\nNote\n----\n\nThis project was originally hosted on the `TankerHQ\n<https://github.com/TankerHQ>`_ organization, which was my employer from 2016\nto 2021. They kindly agreed to give back ownership of this project to\nme. Thanks!\n\nInstallation\n------------\n\nThe recommended way to install ``tbump`` is to use `pipx <https://pipxproject.github.io/pipx/>`_\n\n* Make sure to have Python **3.7** or later installed.\n* Install ``pipx``\n* Run ``pipx install tbump``.\n\n``tbump`` is also available on ``pypi`` and can be installed with ``pip`` if you know what you are doing.\n\nScreenshot\n-----------\n\nHere\'s what a typical usage of ``tbump`` looks like:\n\n.. code-block:: console\n\n    $ tbump 5.0.5\n    :: Bumping from 5.0.4 to 5.0.5\n    => Would patch these files\n    - setup.py:14 version="5.0.4",\n    + setup.py:14 version="5.0.5",\n    - tbump.toml:2 current = "5.0.4"\n    + tbump.toml:2 current = "5.0.5"\n    => Would run these hooks before commit\n    * (1/2) $ ./test.sh\n    * (2/2) $ grep -q -F 5.0.5 Changelog.rst\n    => Would run these git commands\n     * git add --update\n     * git commit --message Bump to 5.0.5\n     * git tag --annotate --message v5.0.5 v5.0.5\n     * git push origin master\n     * git push origin v5.0.5\n    => Would run these hooks after push\n    * (1/1) $ ./publish.sh\n    :: Looking good? (y/N)\n    y\n    => Patching files\n    ...\n    => Running hooks before commit\n    ...\n    => Making bump commit and push matching tags\n    ...\n    => Running hooks after push\n    ...\n    Done ✓\n\n\n\nUsage\n------\n\nFirst, run ``tbump init <current_version>``, where ``current_version``\nis the current version of your program. This will create a\n``tbump.toml`` file looking like this:\n\n.. code-block:: ini\n\n    [version]\n    current = "1.2.41"\n    regex = \'\'\'\n      (?P<major>\\d+)\n      \\.\n      (?P<minor>\\d+)\n      \\.\n      (?P<patch>\\d+)\n    \'\'\'\n\n    [git]\n    message_template = "Bump to {new_version}"\n    tag_template = "v{new_version}"\n\n    [[file]]\n    src = "setup.py"\n\n\n.. note::\n\n * The file uses `toml syntax <https://github.com/toml-lang/toml>`_.\n * Strings should be templated using curly brackets, to be used with\n   Python\'s built-in ``.format()`` method.\n * Paths may contain unix-style `globs\n   <https://docs.python.org/3/library/glob.html>`_, e.g. ``src =\n   "a/**/script.?s"`` matches both ``a/b/script.js`` and\n   ``a/b/c/script.ts``.\n * The version regular expression will be used in `verbose mode\n   <https://docs.python.org/3/library/re.html#re.VERBOSE>`_ and can\n   contain named groups (see below).\n * tbump will also look for a ``[tool.tbump]`` section in the\n   `pyproject.toml` file if its exists. You can use ``tbump init`` with\n   the ``--pyproject`` option to append the configuration in this file\n   instead of creating a new file.\n\n\nThen run:\n\n.. code-block:: console\n\n    $ tbump 1.2.42\n\n``tbump`` will:\n\n* Replace the string ``1.2.41`` by ``1.2.42`` in every file listed in the\n  configuration\n\n* Make a commit based on the ``message_template``.\n\n* Make an **annotated** tag based on the ``tag_template``\n\n* Push the current branch and the tag.\n\nNote that by default, ``tbump`` will display all the changes and stop to ask if they are correct before performing any action, allowing you to abort and re-try the bump if something is not right.\nYou can use ``--non-interactive`` to disable this behavior.\n\nIf you only want to bump the files without performing any git actions or running the hook commands, use the ``--only-patch`` option.\n\nAdvanced configuration\n----------------------\n\nRestricting the lines that are replaced\n+++++++++++++++++++++++++++++++++++++++\n\n\nSometimes you want to make sure only the line matching a given pattern is replaced. For instance, with the following ``package.json``:\n\n.. code-block:: js\n\n    /* in package.json */\n    {\n       "name": "foo",\n       "version": "0.42",\n       "dependencies": {\n         "some-dep": "0.42",\n         "other-dep": "1.3",\n       }\n    }\n\nyou\'ll want to make sure that when you bump from ``0.42`` to ``0.43`` that the line containing ``some-dep`` does not change.\n\nIn this case, you can set a ``search`` option in the ``file`` section:\n\n.. code-block:: ini\n\n    # In tbump.toml\n\n    [[file]]\n    src = "package.json"\n    search = \'"version": "{current_version}"\'\n\nNote that the search string is actually a full regular expression, except for the ``{current_version}`` marker which is substituted as plain text.\n\n\nUsing a custom version template\n+++++++++++++++++++++++++++++++\n\nIf you are using a version schema like ``1.2.3-alpha-4``, you may want to expose a variable that only contains the "public" part of the version string. (``1.2.3`` in this case).\n\nTo do so, add a ``version_template`` option in the ``file`` section. The names used in the format string should match the group names in the regular expression.\n\n\n.. code-block:: js\n\n      /* in version.js */\n\n      export FULL_VERSION = \'1.2.3-alpha-4\';\n      export PUBLIC_VERSION = \'1.2.3\';\n\n.. code-block:: ini\n\n\n      [[file]]\n      src = "version.js"\n      version_template = "{major}.{minor}.{patch}"\n      search = "export PUBLIC_VERSION = \'{current_version}\'"\n\n      [[file]]\n      src = "version.js"\n      search = "export FULL_VERSION = \'{current_version}\'"\n\n\nRunning commands before commit\n++++++++++++++++++++++++++++++\n\nYou can specify a list of hooks to be run after the file have changed, but before the commit is made and pushed.\n\nThis is useful if some of the files under version control are generated through an external program.\n\nHere\'s an example:\n\n\n.. code-block:: ini\n\n    [[before_commit]]\n    name = "Check Changelog"\n    cmd = "grep -q -F {new_version} Changelog.rst"\n\n\nThe name is mandatory. The command will be executed via the shell, after the  ``{new_version}``  placeholder is replaced with the new version.\n\nAny hook that fails will interrupt the bump. You may want to run ``git reset --hard`` before trying again to undo the changes made in the files.\n\nRunning commands after push\n+++++++++++++++++++++++++++\n\nYou can specify a list of hooks to be run right after the tag has been pushed, using an `[[after_push]]` section.\n\nThis is useful if you need the command to run on a clean repository, without un-committed changes, for instance to publish ``rust`` packages:\n\n.. code-block:: ini\n\n    [[after_push]]\n    name = "Publish to crates.io"\n    cmd = "cargo publish"\n\n\nSetting default values for version fields\n+++++++++++++++++++++++++++++++++++++++++\n\n\n(Added in 6.6.0)\n\nIf you have a ``version_template`` that includes fields that don\'t always have a match\n(e.g. prerelease info),\nyou can set a default value to use instead of ``None``,\nwhich would raise an error.\n\nFor example:\n\n.. code-block:: ini\n\n    [version]\n    current = "1.2.3"\n    regex = """\n      (?P<major>\\d+)\n      \\.\n      (?P<minor>\\d+)\n      \\.\n      (?P<patch>\\d+)\n      (\\-\n        (?P<extra>.+)\n      )?\n      """\n\n    [[file]]\n    src = "version.py"\n    version_template = \'({major}, {minor}, {patch}, "{extra}")\'\n    search = "version_info = {current_version}"\n\n    [[field]]\n    # the name of the field\n    name = "extra"\n    # the default value to use, if there is no match\n    default = ""\n',
+    'long_description': '.. image:: https://img.shields.io/pypi/v/tbump.svg\n  :target: https://pypi.org/project/tbump/\n\n.. image:: https://img.shields.io/github/license/dmerejkowsky/tbump.svg\n  :target: https://github.com/dmerejkowsky/tbump/blob/main/LICENSE\n\n.. image:: https://github.com/dmerejkowsky/tbump/workflows/tests/badge.svg\n   :target: https://github.com/dmerejkowsky/tbump/actions\n\n.. image:: https://github.com/dmerejkowsky/tbump/workflows/linters/badge.svg\n   :target: https://github.com/dmerejkowsky/tbump/actions\n\n.. image:: https://img.shields.io/badge/deps%20scanning-pyup.io-green\n   :target: https://github.com/dmerejkowsky/tbump/workflows/safety/\n\n.. image:: https://img.shields.io/badge/code%20style-black-black.svg\n   :target: https://github.com/psf/black\n\n.. image:: https://img.shields.io/badge/mypy-checked-blue.svg\n   :target: https://mypy-lang.org\n\n\ntbump: bump software releases\n=============================\n\ntbump helps you bump the version of your project in a easy way.\n\nNote\n----\n\nThis project was originally hosted on the `TankerHQ\n<https://github.com/TankerHQ>`_ organization, which was my employer from 2016\nto 2021. They kindly agreed to give back ownership of this project to\nme. Thanks!\n\nInstallation\n------------\n\nThe recommended way to install ``tbump`` is to use `pipx <https://pipxproject.github.io/pipx/>`_\n\n* Make sure to have Python **3.7** or later installed.\n* Install ``pipx``\n* Run ``pipx install tbump``.\n\n``tbump`` is also available on ``pypi`` and can be installed with ``pip`` if you know what you are doing.\n\nScreenshot\n-----------\n\nHere\'s what a typical usage of ``tbump`` looks like:\n\n.. code-block:: console\n\n    $ tbump 5.0.5\n    :: Bumping from 5.0.4 to 5.0.5\n    => Would patch these files\n    - setup.py:14 version="5.0.4",\n    + setup.py:14 version="5.0.5",\n    - tbump.toml:2 current = "5.0.4"\n    + tbump.toml:2 current = "5.0.5"\n    => Would run these hooks before commit\n    * (1/2) $ ./test.sh\n    * (2/2) $ grep -q -F 5.0.5 Changelog.rst\n    => Would run these git commands\n     * git add --update\n     * git commit --message Bump to 5.0.5\n     * git tag --annotate --message v5.0.5 v5.0.5\n     * git push origin master\n     * git push origin v5.0.5\n    => Would run these hooks after push\n    * (1/1) $ ./publish.sh\n    :: Looking good? (y/N)\n    y\n    => Patching files\n    ...\n    => Running hooks before commit\n    ...\n    => Making bump commit and push matching tags\n    ...\n    => Running hooks after push\n    ...\n    Done ✓\n\n\n\nUsage\n------\n\nFirst, run ``tbump init <current_version>``, where ``current_version``\nis the current version of your program. This will create a\n``tbump.toml`` file looking like this:\n\n.. code-block:: ini\n\n    [version]\n    current = "1.2.41"\n    regex = \'\'\'\n      (?P<major>\\d+)\n      \\.\n      (?P<minor>\\d+)\n      \\.\n      (?P<patch>\\d+)\n    \'\'\'\n\n    [git]\n    message_template = "Bump to {new_version}"\n    tag_template = "v{new_version}"\n\n    [[file]]\n    src = "setup.py"\n\n\n.. note::\n\n * The file uses `toml syntax <https://github.com/toml-lang/toml>`_.\n * Strings should be templated using curly brackets, to be used with\n   Python\'s built-in ``.format()`` method.\n * Paths may contain unix-style `globs\n   <https://docs.python.org/3/library/glob.html>`_, e.g. ``src =\n   "a/**/script.?s"`` matches both ``a/b/script.js`` and\n   ``a/b/c/script.ts``.\n * The version regular expression will be used in `verbose mode\n   <https://docs.python.org/3/library/re.html#re.VERBOSE>`_ and can\n   contain named groups (see below).\n * tbump will also look for a ``[tool.tbump]`` section in the\n   `pyproject.toml` file if its exists. You can use ``tbump init`` with\n   the ``--pyproject`` option to append the configuration in this file\n   instead of creating a new file.\n\n\nThen run:\n\n.. code-block:: console\n\n    $ tbump 1.2.42\n\n``tbump`` will:\n\n* Replace the string ``1.2.41`` by ``1.2.42`` in every file listed in the\n  configuration\n\n* Make a commit based on the ``message_template``.\n\n* Make an **annotated** tag based on the ``tag_template``\n\n* Push the current branch and the tag.\n\nNote that by default, ``tbump`` will display all the changes and stop to ask if they are correct before performing any action, allowing you to abort and re-try the bump if something is not right.\nYou can use ``--non-interactive`` to disable this behavior.\n\nIf you only want to bump the files without performing any git actions or running the hook commands, use the ``--only-patch`` option.\n\nThe current version of the project can be found using the command:\n\n.. code-block:: console\n\n    $ tbump current-version\n\nAdvanced configuration\n----------------------\n\nRestricting the lines that are replaced\n+++++++++++++++++++++++++++++++++++++++\n\n\nSometimes you want to make sure only the line matching a given pattern is replaced. For instance, with the following ``package.json``:\n\n.. code-block:: js\n\n    /* in package.json */\n    {\n       "name": "foo",\n       "version": "0.42",\n       "dependencies": {\n         "some-dep": "0.42",\n         "other-dep": "1.3",\n       }\n    }\n\nyou\'ll want to make sure that when you bump from ``0.42`` to ``0.43`` that the line containing ``some-dep`` does not change.\n\nIn this case, you can set a ``search`` option in the ``file`` section:\n\n.. code-block:: ini\n\n    # In tbump.toml\n\n    [[file]]\n    src = "package.json"\n    search = \'"version": "{current_version}"\'\n\nNote that the search string is actually a full regular expression, except for the ``{current_version}`` marker which is substituted as plain text.\n\n\nUsing a custom version template\n+++++++++++++++++++++++++++++++\n\nIf you are using a version schema like ``1.2.3-alpha-4``, you may want to expose a variable that only contains the "public" part of the version string. (``1.2.3`` in this case).\n\nTo do so, add a ``version_template`` option in the ``file`` section. The names used in the format string should match the group names in the regular expression.\n\n\n.. code-block:: js\n\n      /* in version.js */\n\n      export FULL_VERSION = \'1.2.3-alpha-4\';\n      export PUBLIC_VERSION = \'1.2.3\';\n\n.. code-block:: ini\n\n\n      [[file]]\n      src = "version.js"\n      version_template = "{major}.{minor}.{patch}"\n      search = "export PUBLIC_VERSION = \'{current_version}\'"\n\n      [[file]]\n      src = "version.js"\n      search = "export FULL_VERSION = \'{current_version}\'"\n\n\nRunning commands before commit\n++++++++++++++++++++++++++++++\n\nYou can specify a list of hooks to be run after the file have changed, but before the commit is made and pushed.\n\nThis is useful if some of the files under version control are generated through an external program.\n\nHere\'s an example:\n\n\n.. code-block:: ini\n\n    [[before_commit]]\n    name = "Check Changelog"\n    cmd = "grep -q -F {new_version} Changelog.rst"\n\n\nThe name is mandatory. The command will be executed via the shell, after the  ``{new_version}``  placeholder is replaced with the new version.\n\nAny hook that fails will interrupt the bump. You may want to run ``git reset --hard`` before trying again to undo the changes made in the files.\n\nRunning commands after push\n+++++++++++++++++++++++++++\n\nYou can specify a list of hooks to be run right after the tag has been pushed, using an `[[after_push]]` section.\n\nThis is useful if you need the command to run on a clean repository, without un-committed changes, for instance to publish ``rust`` packages:\n\n.. code-block:: ini\n\n    [[after_push]]\n    name = "Publish to crates.io"\n    cmd = "cargo publish"\n\n\nSetting default values for version fields\n+++++++++++++++++++++++++++++++++++++++++\n\n\n(Added in 6.6.0)\n\nIf you have a ``version_template`` that includes fields that don\'t always have a match\n(e.g. prerelease info),\nyou can set a default value to use instead of ``None``,\nwhich would raise an error.\n\nFor example:\n\n.. code-block:: ini\n\n    [version]\n    current = "1.2.3"\n    regex = """\n      (?P<major>\\d+)\n      \\.\n      (?P<minor>\\d+)\n      \\.\n      (?P<patch>\\d+)\n      (\\-\n        (?P<extra>.+)\n      )?\n      """\n\n    [[file]]\n    src = "version.py"\n    version_template = \'({major}, {minor}, {patch}, "{extra}")\'\n    search = "version_info = {current_version}"\n\n    [[field]]\n    # the name of the field\n    name = "extra"\n    # the default value to use, if there is no match\n    default = ""\n',
     'author': 'Dimitri Merejkowsky',
     'author_email': 'dimitri@dmerej.info',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/dmerejkowsky/tbump',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `tbump-6.8.0/PKG-INFO` & `tbump-6.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tbump
-Version: 6.8.0
+Version: 6.9.0
 Summary: Bump software releases
 Home-page: https://github.com/dmerejkowsky/tbump
 License: BSD-3-Clause
 Author: Dimitri Merejkowsky
 Author-email: dimitri@dmerej.info
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -170,14 +170,20 @@
 * Push the current branch and the tag.
 
 Note that by default, ``tbump`` will display all the changes and stop to ask if they are correct before performing any action, allowing you to abort and re-try the bump if something is not right.
 You can use ``--non-interactive`` to disable this behavior.
 
 If you only want to bump the files without performing any git actions or running the hook commands, use the ``--only-patch`` option.
 
+The current version of the project can be found using the command:
+
+.. code-block:: console
+
+    $ tbump current-version
+
 Advanced configuration
 ----------------------
 
 Restricting the lines that are replaced
 +++++++++++++++++++++++++++++++++++++++
```

