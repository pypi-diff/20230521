# Comparing `tmp/conjuring-0.3.0.tar.gz` & `tmp/conjuring-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conjuring-0.3.0.tar", max compression
+gzip compressed data, was "conjuring-0.4.0.tar", max compression
```

## Comparing `conjuring-0.3.0.tar` & `conjuring-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1410 2023-05-20 13:21:30.743577 conjuring-0.3.0/docs/README.md
--rw-r--r--   0        0        0     1576 2023-05-20 13:21:30.743577 conjuring-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1867 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/__init__.py
--rw-r--r--   0        0        0      541 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/colors.py
--rw-r--r--   0        0        0      313 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/constants.py
--rw-r--r--   0        0        0    10777 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/grimoire.py
--rw-r--r--   0        0        0        0 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/aws.py
--rw-r--r--   0        0        0     3001 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/blanket.py
--rw-r--r--   0        0        0     1437 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/conjuring.py
--rw-r--r--   0        0        0     1239 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/docker.py
--rw-r--r--   0        0        0     1725 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/duplicity.py
--rw-r--r--   0        0        0     1000 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/fork.py
--rw-r--r--   0        0        0    14739 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/git.py
--rw-r--r--   0        0        0     1008 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/jrnl.py
--rw-r--r--   0        0        0     2851 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/k8s.py
--rw-r--r--   0        0        0     7044 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/media.py
--rw-r--r--   0        0        0      777 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/mkdocs.py
--rw-r--r--   0        0        0     2695 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/mr.py
--rw-r--r--   0        0        0      824 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/onedrive.py
--rw-r--r--   0        0        0    11455 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/paperless.py
--rw-r--r--   0        0        0     2721 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/pre_commit.py
--rw-r--r--   0        0        0     6741 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/py.py
--rw-r--r--   0        0        0     1092 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/spells/shell.py
--rw-r--r--   0        0        0     1931 2023-05-20 13:21:30.743577 conjuring-0.3.0/src/conjuring/visibility.py
--rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 conjuring-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1410 2023-05-21 11:47:31.040329 conjuring-0.4.0/docs/README.md
+-rw-r--r--   0        0        0     9163 2023-05-21 11:47:31.040329 conjuring-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1900 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/__init__.py
+-rw-r--r--   0        0        0      541 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/colors.py
+-rw-r--r--   0        0        0      313 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/constants.py
+-rw-r--r--   0        0        0    10397 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/grimoire.py
+-rw-r--r--   0        0        0        0 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/__init__.py
+-rw-r--r--   0        0        0     2191 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/aws.py
+-rw-r--r--   0        0        0     3018 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/blanket.py
+-rw-r--r--   0        0        0     1438 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/conjuring.py
+-rw-r--r--   0        0        0     1240 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/docker.py
+-rw-r--r--   0        0        0     1725 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/duplicity.py
+-rw-r--r--   0        0        0     1018 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/fork.py
+-rw-r--r--   0        0        0    14779 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/git.py
+-rw-r--r--   0        0        0     1008 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/jrnl.py
+-rw-r--r--   0        0        0     2967 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/k8s.py
+-rw-r--r--   0        0        0     7050 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/media.py
+-rw-r--r--   0        0        0      777 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/mkdocs.py
+-rw-r--r--   0        0        0     2647 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/mr.py
+-rw-r--r--   0        0        0      824 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/onedrive.py
+-rw-r--r--   0        0        0    11612 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/paperless.py
+-rw-r--r--   0        0        0     2724 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/pre_commit.py
+-rw-r--r--   0        0        0     9159 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/py.py
+-rw-r--r--   0        0        0     1081 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/spells/shell.py
+-rw-r--r--   0        0        0     1928 2023-05-21 11:47:31.044329 conjuring-0.4.0/src/conjuring/visibility.py
+-rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 conjuring-0.4.0/PKG-INFO
```

### Comparing `conjuring-0.3.0/docs/README.md` & `conjuring-0.4.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `conjuring-0.3.0/src/conjuring/__init__.py` & `conjuring-0.4.0/src/conjuring/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,19 @@
     """Load all spell modules except the chosen ones by partial task name."""
     return _cast_chosen_spells(include=None, exclude=exclude)
 
 
 def _cast_chosen_spells(*, include: Optional[Sequence[str]], exclude: Optional[Sequence[str]]) -> Collection:
     """Load the chosen spell modules dynamically and add their tasks to the namespace."""
     namespace = collection_from_python_files(
-        sys.modules[__name__], "tasks.py", "conjuring*.py", include=include, exclude=exclude
+        sys.modules[__name__],
+        "tasks.py",
+        "conjuring*.py",
+        include=include,
+        exclude=exclude,
     )
 
     spell_dir = (Path(__file__).parent / "spells").absolute()
     parent_modules = ".".join(spell_dir.parts[-2:])
     for module_file in spell_dir.glob("*.py"):
         module_name = module_file.stem
         if module_name == "__init__":
```

### Comparing `conjuring-0.3.0/src/conjuring/colors.py` & `conjuring-0.4.0/src/conjuring/colors.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.3.0/src/conjuring/grimoire.py` & `conjuring-0.4.0/src/conjuring/grimoire.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import types
 from collections import defaultdict
 from collections.abc import Sequence
 from dataclasses import dataclass
 from importlib import import_module
 from pathlib import Path
 from shlex import quote
-from typing import Callable, overload
+from typing import Callable
 
 from invoke import Collection, Context, Result, Task
 
 from conjuring.colors import COLOR_BOLD_WHITE, COLOR_LIGHT_GREEN, COLOR_LIGHT_RED, COLOR_NONE, COLOR_YELLOW
 from conjuring.visibility import display_task
 
 CONJURING_IGNORE_MODULES = os.environ.get("CONJURING_IGNORE_MODULES", "").split(",")
@@ -73,15 +73,15 @@
 def print_warning(*message: str, nl=False):
     """Print a warning message."""
     print_color(*message, color=COLOR_YELLOW, nl=nl)
 
 
 def ask_user_prompt(*message: str, color: str = COLOR_BOLD_WHITE, allowed_keys: str = "") -> str:
     """Display a prompt with a message. Wait a little before, so stdout is flushed before the input message."""
-    lowercase_key_list = [char.lower() for char in allowed_keys] if allowed_keys else None
+    lowercase_key_list = [char.lower() for char in allowed_keys] if allowed_keys else []
     options = "/".join(allowed_keys) if allowed_keys else None
     prefix = f"Type {options} +" if allowed_keys else "Press"
 
     while True:
         print()
         print_color(*message, color=color)
         time.sleep(0.2)
@@ -91,28 +91,15 @@
             return typed_input
 
         lowercase_key = typed_input.lower()
         if lowercase_key in lowercase_key_list:
             return lowercase_key
 
 
-# TODO: refactor: Overloaded function signatures 1 and 2 overlap with incompatible return types
-@overload
-def run_with_fzf(c: Context, *pieces: str, query=...) -> str:  # type:ignore[misc]
-    ...
-
-
-@overload
-def run_with_fzf(c: Context, *pieces: str, query=..., multi: bool = ...) -> list[str]:
-    ...
-
-
-def run_with_fzf(
-    c: Context, *pieces: str, query="", header="", multi=False, options="", preview="", **kwargs
-) -> str | list[str]:
+def run_with_fzf(c: Context, *pieces: str, query="", header="", multi=False, options="", preview="", **kwargs) -> str:
     """Run a command with fzf and return the chosen entry."""
     fzf_pieces = ["| fzf --reverse --select-1 --height 40% --cycle"]
     if query:
         fzf_pieces.append(f"-q '{query}'")
     if header:
         fzf_pieces.append(f"--header='{header}'")
     if multi:
@@ -127,18 +114,15 @@
     kwargs.setdefault("hide", False)
     kwargs.setdefault("pty", False)
     return which_function(c, *pieces, *fzf_pieces, **kwargs)
 
 
 def ignore_module(module_name: str) -> bool:
     """Ignore a module by its name."""
-    for ignore_str in CONJURING_IGNORE_MODULES:
-        if ignore_str and ignore_str in module_name:
-            return True
-    return False
+    return any(ignore_str and ignore_str in module_name for ignore_str in CONJURING_IGNORE_MODULES)
 
 
 def resolve_module_str(module_or_str: types.ModuleType | str) -> types.ModuleType | None:
     if isinstance(module_or_str, str):
         module = import_module(module_or_str)
         if ignore_module(module_or_str):
             return None
@@ -165,28 +149,25 @@
 @dataclass
 class SpellBook:
     prefix: str
     module: types.ModuleType
     display_all_tasks: bool
 
 
-def _is_task_present(name: str, list_: list[str] | None) -> bool:
+def _is_task_present(name: str, list_: Sequence[str] | None) -> bool:
     if not list_:
         return True
-    for element in list_:
-        if fnmatch.fnmatch(name, element):
-            return True
-    return False
+    return any(fnmatch.fnmatch(name, element) for element in list_)
 
 
 def add_single_task_to(
     collection: Collection,
     task: Task,
-    include: list[str] | None,
-    exclude: list[str] | None,
+    include: Sequence[str] | None,
+    exclude: Sequence[str] | None,
     *,
     prefix: str | None,
     task_name: str | None,
 ) -> bool:
     guessed_name = guess_full_task_name(prefix, task.name)
     should_include = not include or _is_task_present(guessed_name, include)
     should_exclude = exclude and _is_task_present(guessed_name, exclude)
@@ -199,16 +180,16 @@
     return False
 
 
 def magically_add_tasks(  # noqa: C901 # TODO: refactor: magically_add_tasks is too complex (12)
     to_collection: Collection,
     from_module_or_str: types.ModuleType | str,
     *,
-    include: Sequence[str] = None,
-    exclude: Sequence[str] = None,
+    include: Sequence[str] | None = None,
+    exclude: Sequence[str] | None = None,
 ) -> None:
     """Magically add tasks to the collection according to the module/task configuration.
 
     Task-specific configuration has precedence over the module.
 
     1. If the task is a :py:class:`MagicTask`, then its ``should_display()`` method is used to check visibility.
     2. If the module has a ``should_display_tasks()`` function,
@@ -258,16 +239,16 @@
                     continue
                 raise
 
 
 def collection_from_python_files(
     current_module,
     *py_glob_patterns: str,
-    include: Sequence[str] = None,
-    exclude: Sequence[str] = None,
+    include: Sequence[str] | None = None,
+    exclude: Sequence[str] | None = None,
 ):
     """Create a custom collection by adding tasks from multiple files.
 
     Search directories for glob patterns:
     1. Root dir.
     2. Current dir.
```

### Comparing `conjuring-0.3.0/src/conjuring/spells/aws.py` & `conjuring-0.4.0/src/conjuring/spells/aws.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 def list_aws_profiles(c: Context) -> list[str]:
     """List AWS profiles from the config file."""
     return run_lines(c, LIST_AWS_PROFILES_COMMAND)
 
 
 def fzf_aws_profile(c, partial_name: Optional[str] = None) -> str:
     """Select an AWS profile from a partial profile name using fzf."""
-    if not partial_name and (aws_profile := os.environ.get("AWS_PROFILE")):
-        if aws_profile:
-            print(f"Using env variable AWS_PROFILE (set to '{aws_profile}')")
-            return aws_profile
+    if not partial_name and (aws_profile := os.environ.get("AWS_PROFILE")) and aws_profile:
+        print(f"Using env variable AWS_PROFILE (set to '{aws_profile}')")
+        return aws_profile
 
     return run_with_fzf(c, LIST_AWS_PROFILES_COMMAND, query=partial_name)
 
 
 def fzf_aws_account(c) -> str:
     """Select an AWS account from the config file."""
     return run_with_fzf(c, f"rg -o 'aws:iam::[^:]+' {AWS_CONFIG} | cut -d ':' -f 4 | sort -u")
```

### Comparing `conjuring-0.3.0/src/conjuring/spells/blanket.py` & `conjuring-0.4.0/src/conjuring/spells/blanket.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 @task(
     help={
         "cz": "Run commitizen (cz check) to validate the description of the to-do item as a commit message",
         "valid": "When using cz check, print valid to-do items",
         "invalid": "When using cz check, print invalid to-do items",
         "short": "Short format: only the description, without the lines of code where to-do items were found",
         "priority": f"Show only higher priority tasks ({FIX_ME})",
-    }
+    },
 )
 def todo(c, cz=False, valid=True, invalid=True, short=False, priority=False):
     """List to-dos and fix-mes in code. Optionally check if the description follows Conventional Commits (cz check)."""
     all_todos: dict[Task, list[Location]] = defaultdict(list)
     all_keys: list[Task] = []
 
     for which in (FIX_ME,) if priority else (FIX_ME, TO_DO):
         # This command freezes if pty=False
         for line in run_lines(c, f"rg --color=never --no-heading {which}", warn=True, pty=True):
             before, after = line.split(which, maxsplit=1)  # type: str,str
             key = Task(which, after.strip(": "))
             all_keys.append(key)
-            location = Location(*before.strip("/# ").split(":", maxsplit=2))
+            location = Location(*before.strip("/# ").split(":", maxsplit=2))  # type: ignore
             all_todos[key].append(location)
 
     for item, locations in sorted(all_todos.items()):  # type: Task, list[Location]
         func = print_success
         if cz:
             result = run_command(c, "cz check -m", quote(item.description), hide=True, warn=True)
             if result.ok:
```

### Comparing `conjuring-0.3.0/src/conjuring/spells/conjuring.py` & `conjuring-0.4.0/src/conjuring/spells/conjuring.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 should_display_tasks: ShouldDisplayTasks = is_home_dir
 
 
 @task(
     help={
         "edit": "Open the config file with $EDITOR",
         "revert": "Revert the changes and go back to using tasks.py as the default tasks file",
-    }
+    },
 )
 def setup(c, edit=False, revert=False):
     """Setup Conjuring on your home dir."""
     config_file = Path("~/.invoke.yaml").expanduser()
     json_config = """'{"tasks":{"collection_name":"conjuring_summon"}}'"""
     if config_file.exists():
         message = "Remove this from" if revert else "Add this to"
```

### Comparing `conjuring-0.3.0/src/conjuring/spells/docker.py` & `conjuring-0.4.0/src/conjuring/spells/docker.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 @task(
     help={
         "container": "Container name to remove (regexp)",
         "all_": "All containers",
         "exited": "Exited containers",
-    }
+    },
 )
 def rm_containers(c, container="", all_=False, exited=False):
     """Remove Docker containers."""
     cmd = []
     if all_:
         cmd = ["docker ps -a"]
     elif exited:
@@ -29,15 +29,15 @@
     run_command(c, *cmd, "| tail +2 | awk '{print $1}' | xargs docker rm -f")
     run_command(c, *cmd)
 
 
 @task(help=({"dangling": "Dangling volumes"}))
 def rm_volumes(c, dangling=False):
     """Remove Docker volumes."""
-    cmd = []
+    cmd = ""
     if dangling:
         cmd = 'docker volume ls -f "dangling=true"'
     if not cmd:
         print_error("Choose one argument. Run with --help to see available argument")
         return
 
     run_command(c, cmd, dry=False)
```

### Comparing `conjuring-0.3.0/src/conjuring/spells/duplicity.py` & `conjuring-0.4.0/src/conjuring/spells/duplicity.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.3.0/src/conjuring/spells/fork.py` & `conjuring-0.4.0/src/conjuring/spells/fork.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 @task
 def remote(c, username, remote=""):
     """Configure a remote for a fork.
 
     https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/configuring-a-remote-for-a-fork
     """
     if username.startswith("-"):
-        raise Exit("Arguments should be: username [--remote]")
+        msg = "Arguments should be: username [--remote]"
+        raise Exit(msg)
     if not remote:
         remote = username
 
     project = c.run(r"git remote -v | rg origin | head -1 | rg -o '/(.+)\.git' -r '$1'", pty=False).stdout.strip()
     c.run(f"git remote add {remote} https://github.com/{username}/{project}.git", warn=True)
     c.run("git remote -v")
```

### Comparing `conjuring-0.3.0/src/conjuring/spells/git.py` & `conjuring-0.4.0/src/conjuring/spells/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     def current_branch(self) -> str:
         """Return the current branch name."""
         return run_stdout(self.context, "git branch --show-current")
 
     def default_branch(self) -> str:
         """Return the default branch name (master/main/develop/development)."""
         return run_stdout(
-            self.context, "git branch -a | rg -o -e /master -e /develop.+ -e /main | sort -u | cut -b 2- | head -1"
+            self.context,
+            "git branch -a | rg -o -e /master -e /develop.+ -e /main | sort -u | cut -b 2- | head -1",
         )
 
     def checkout(self, *branches: str) -> str:
         """Try checking out the specified branches in order."""
         for branch in branches:
             try:
                 self.context.run(f"git checkout {branch}")
@@ -105,15 +106,15 @@
 
 
 @task(
     help={
         "new_project_dir": "Dir of the project to be created. The dir might exist or not",
         "reset": "Remove the new dir and start over",
         "keep": "Keep branches and remote after the extracting is done",
-    }
+    },
 )
 def extract_subtree(c, new_project_dir, reset=False, keep=False):
     """Extract files from subdirectories of the current Git repo to another repo, using git subtree.
 
     The files will be moved to the root of the new repo.
 
     Solutions adapted from:
@@ -132,15 +133,15 @@
         run_with_fzf(
             c,
             Git.SHOW_ALL_FILE_HISTORY,
             dry=False,
             header="Use TAB to choose the files you want to KEEP",
             multi=True,
             preview="test -f {} && head -20 {} || echo FILE NOT FOUND, IT EXISTS ONLY IN GIT HISTORY",
-        )
+        ),
     )
     sub_dirs = {part.rsplit("/", 1)[0] for part in chosen_files}
     obliterate = set(all_files.difference(chosen_files))
 
     first_date = run_stdout(c, 'git log --format="%cI" --root | sort -u | head -1')
 
     prefixes: list[str] = []
@@ -209,15 +210,15 @@
 
 @task(
     help={
         "full": "Display all info: files, authors, dates",
         "files": "Display all files in Git history, even the ones that were deleted and don't exist anymore",
         "author": "Display authors",
         "dates": "Display committer and author dates in different colors",
-    }
+    },
 )
 def history(c, full=False, files=False, author=False, dates=False):
     """Grep the whole Git log and display information."""
     option_chosen = False
     if full:
         option_chosen = True
         files = author = dates = True
@@ -232,33 +233,34 @@
         header = True
         for line in run_lines(c, 'git log --format="%H|%cI|%aI|%GK|%s"', hide=False):
             if header:
                 print_success("Green = dates are equal")
                 print_error("Red = dates are different")
                 print(
                     "Commit                                   Committer Date            "
-                    "Author Date               GPG key          Subject"
+                    "Author Date               GPG key          Subject",
                 )
                 header = False
 
             fields = line.split("|")
             committer_date = fields[1]
             author_date = fields[2]
             func = print_success if committer_date == author_date else print_error
             func(*fields)
     if not option_chosen:
-        raise Exit("Choose at least one option: --full, --files, --author, --dates", 1)
+        msg = "Choose at least one option: --full, --files, --author, --dates"
+        raise Exit(msg, 1)
 
 
 @task(
     help={
         "commit": "Base commit to be used for the range (default: --root)",
         "gpg": "Sign the commit (default: True)",
         "author": "Set the current author (from 'git config') on the commit range",
-    }
+    },
 )
 def rewrite(c, commit="--root", gpg=True, author=True):
     """Rewrite a range of commits, signing with GPG and setting the author.
 
     https://git-scm.com/docs/git-commit
     https://git-scm.com/docs/git-rebase
     """
@@ -270,15 +272,15 @@
         email = run_stdout(c, "git config user.email", dry=False)
         author_flag = f' --author "{name} <{email}>"'
 
     c.run(f'git log --format="%H %cI %aI %s" {commit} > $TMPDIR/rebase_sign_hashlist')
     c.run(
         "git rebase --committer-date-is-author-date --exec 'GIT_COMMITTER_DATE="
         '$(fgrep -m 1 "$(git log -1 --format="%aI %s" $GIT_COMMIT)" $TMPDIR/rebase_sign_hashlist'
-        f' | cut -d" " -f3) git commit --amend --no-edit -n{author_flag}{gpg_flag}\' -i {commit}'
+        f' | cut -d" " -f3) git commit --amend --no-edit -n{author_flag}{gpg_flag}\' -i {commit}',
     )
     history(c, dates=True)
     print()
     print("NOTE: If commits were modified during the rebase above, their committer date will be the current date")
     print("Rebase again with this command, without changing any commit, and all dates should be green")
 
 
@@ -297,15 +299,15 @@
 
 @task(
     help={
         "remote": "List remote branches (default: False)",
         "update": "Update the repo before merging (default: True)",
         "push": "Push the merge to the remote (default: True)",
         "rebase": "Rebase the default branch before merging (default: False)",
-    }
+    },
 )
 def merge_default(c, remote=False, update=True, push=True, rebase=False):
     """Merge the default branch of the repo. Also set it with "git config", if not already set."""
     default_branch = set_default_branch(c, remote)
 
     if update:
         tidy_up(c)
@@ -334,15 +336,15 @@
 
 
 @task(
     help={
         "tag": "Name of the tag to compare to (default: last created tag)",
         "files": "Display files instead of commits (default: false)",
         "verbose": "Files: display changes/insertions/deletion. Commits: display the full commit message, author... (default: False)",
-    }
+    },
 )
 def changes_since_tag(c, tag="", files=False, verbose=False):
     """Display changes (commits or files) since the last tag (or a chosen tag)."""
     which_tag = tag or run_stdout(c, "git tag --list --sort -creatordate | head -1", hide=False, dry=False)
     default_branch = set_default_branch(c)
     if files:
         option = "" if verbose else " --name-only"
@@ -364,15 +366,15 @@
         c.run("gh repo view --web")
 
 
 @task(
     help={
         "prefix": "Keep the Conventional Commits prefix",
         "sort": "Sort bullets",
-    }
+    },
 )
 def body(c, prefix=True, sort=True):
     """Prepare a commit body to be used on pull requests and squashed commits."""
     default_branch = set_default_branch(c)
     bullets = []
     for line in run_lines(c, f"git log {default_branch}..", "--format=%s%n%b"):
         clean = line.strip(" -")
```

### Comparing `conjuring-0.3.0/src/conjuring/spells/jrnl.py` & `conjuring-0.4.0/src/conjuring/spells/jrnl.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.3.0/src/conjuring/spells/k8s.py` & `conjuring-0.4.0/src/conjuring/spells/k8s.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """Kubernetes."""
 from dataclasses import dataclass
+from typing import Optional, cast
 
 from invoke import Context, Result, task
 
 from conjuring.grimoire import run_command, run_lines, run_with_fzf
 
 SHOULD_PREFIX = True
 
 
 @dataclass
 class Kubectl:
     """Kubectl commands."""
 
     context: Context
 
-    def choose_apps(self, partial_app_name: str = None, *, multi=False) -> list[str]:
+    def choose_apps(self, partial_app_name: Optional[str] = None, *, multi=False) -> list[str]:
         """Select apps from Kubernetes deployments, using a partial app name and fzf."""
-        return run_with_fzf(
-            self.context,
-            """kubectl get deployments.apps -o jsonpath='{range .items[*]}{.metadata.name}{"\\n"}{end}'""",
-            query=partial_app_name,
-            multi=multi,
+        return cast(
+            list[str],
+            run_with_fzf(
+                self.context,
+                """kubectl get deployments.apps -o jsonpath='{range .items[*]}{.metadata.name}{"\\n"}{end}'""",
+                query=partial_app_name,
+                multi=multi,
+            ),
         )
 
     @staticmethod
     def _app_selector(apps: list[str]) -> str:
         """Return the app selector for one or more apps."""
         sorted_unique_apps = sorted(set(apps))
         if len(sorted_unique_apps) == 1:
```

### Comparing `conjuring-0.3.0/src/conjuring/spells/media.py` & `conjuring-0.4.0/src/conjuring/spells/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,24 +85,24 @@
 
 
 @task(
     help={
         "organize": "Call 'organize run' before categorizing",
         "browse": "Open dir on Finder",
         "empty": "Check dirs that are not empty but should be",
-    }
+    },
 )
 def categorize(c, organize=True, browse=True, empty=True):
     """Open directories with files/photos that have to be categorized/moved/renamed."""
     if organize:
         c.run("invoke organize")
 
     empty_dirs = (
         [
-            Path(d).expanduser()
+            Path(str(d)).expanduser()
             for d in [
                 DOWNLOADS_DIR,
                 DESKTOP_DIR,
                 "~/Documents/Shared_Downloads",
                 PICTURES_DIR / "Telegram",
                 PICTURES_DIR / "Samsung_Gallery/Pictures/Telegram",
                 ONE_DRIVE_DIR / "Documents/Mayan_Staging/Portugues",
```

### Comparing `conjuring-0.3.0/src/conjuring/spells/mkdocs.py` & `conjuring-0.4.0/src/conjuring/spells/mkdocs.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.3.0/src/conjuring/spells/mr.py` & `conjuring-0.4.0/src/conjuring/spells/mr.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,15 @@
 @dataclass
 class MyRepos:
     context: Context
 
     def find_configs(self, partial_name: str, echo=False) -> list[Path]:
         """Find config files in the current dir or dirs above."""
         lower_partial_name = partial_name.lower()
-        if not lower_partial_name:
-            glob_pattern = MRCONFIG_FILE
-        else:
-            glob_pattern = f"{MRCONFIG_FILE}*{lower_partial_name}*"
+        glob_pattern = MRCONFIG_FILE if not lower_partial_name else f"{MRCONFIG_FILE}*{lower_partial_name}*"
         config_dir = self._find_dir_with_mrconfigs(glob_pattern)
         if not config_dir:
             msg = f"No {MRCONFIG_FILE}* file was found in {Path.cwd()} or its parents"
             raise FileNotFoundError(msg)
 
         if not lower_partial_name:
             return [config_dir / MRCONFIG_FILE]
@@ -53,15 +50,15 @@
         return None
 
 
 @task(
     help={
         "config": f"Specific config file to use. Use fzf if multiple are found. Default: {MRCONFIG_FILE}",
         "echo": "Echo the commands being executed, for debugging purposes. Default: False",
-    }
+    },
 )
 def grep(c, search_text, config="", echo=False):
     """Grep mr repositories with a search text and print the directories in which the text was found.
 
     Needs mr to be preconfigured with files starting with the ".mrconfig" prefix.
     """
     for chosen in MyRepos(c).find_configs(config, echo=echo):
```

### Comparing `conjuring-0.3.0/src/conjuring/spells/onedrive.py` & `conjuring-0.4.0/src/conjuring/spells/onedrive.py`

 * *Files identical despite different names*

### Comparing `conjuring-0.3.0/src/conjuring/spells/paperless.py` & `conjuring-0.4.0/src/conjuring/spells/paperless.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Wrapper tasks for papaerless commands https://github.com/paperless-ngx/paperless-ngx."""
 from __future__ import annotations
 
 import re
 import shutil
 from collections import defaultdict
+from collections.abc import Sequence
 from dataclasses import dataclass, field
 from pathlib import Path
 
 import requests
 from invoke import task
 
 from conjuring.constants import DOT_DS_STORE, DOWNLOADS_DIR
@@ -88,27 +89,36 @@
         "orphans": "Show orphan files",
         "thumbnails": "Show thumbnail files",
         "documents": "Show documents with issues",
         "unknown": "Show unknown lines from the log",
         "together": f"Keep {ORPHAN_ORIGINALS} and {ORPHAN_ARCHIVE} in the same output directory",
         "fix": "Fix broken files by copying them to the downloads dir",
         "move": "Move files instead of copying",
-    }
+    },
 )
 def sanity(
-    c, hide=True, orphans=False, thumbnails=False, documents=False, unknown=True, together=False, fix=False, move=False
+    c,
+    hide=True,
+    orphans=False,
+    thumbnails=False,
+    documents=False,
+    unknown=True,
+    together=False,
+    fix=False,
+    move=False,
 ):
     """Sanity checker. Optionally fix orphan files (copies or movies them to the download dir).
 
     https://docs.paperless-ngx.com/administration/#sanity-checker
     """
     # Fail fast if the env var is not set
     documents_dir = paperless_documents_dir() if fix else None
     if documents_dir and not documents_dir.exists():
-        raise RuntimeError(f"Documents directory doesn't exist: {documents_dir}")
+        msg = f"Documents directory doesn't exist: {documents_dir}"
+        raise RuntimeError(msg)
 
     # TODO: fix(paperless): implement dry-run mode with dry=False and actually avoid files being copied/moved
     lines = run_lines(c, paperless_cmd(), "document_sanity_checker", hide=hide, warn=True, pty=True)
 
     progress_bar: list[str] = []
     original_or_archive_files: dict[str, list[OrphanFile]] = defaultdict(list)
     matched_files: list[OrphanFile] = []
@@ -168,15 +178,17 @@
         _split_original_archive(original_or_archive_files, partial_path, documents_dir)
         return
 
     orphan_files.append(str(partial_path))
 
 
 def _split_original_archive(
-    original_or_archive_files: dict[str, list[OrphanFile]], partial_path: Path, documents_dir: Path = None
+    original_or_archive_files: dict[str, list[OrphanFile]],
+    partial_path: Path,
+    documents_dir: Path | None = None,
 ):
     file_key = str(Path("/".join(partial_path.parts[1:])).with_suffix(""))
     expanded_parts = []
     for part in partial_path.parts[:-1]:
         if "," in part:
             expanded_parts.extend(sorted(part.split(",")))
         else:
@@ -209,34 +221,39 @@
             if together:
                 for orphan_file in originals_first:
                     match_path = orphan_file.destination
                     file_without_first_part = Path("/".join(match_path.parts[1:]))
                     if str(match_path).startswith(ORPHAN_ARCHIVE):
                         # Append ORPHAN_ARCHIVE to the file stem
                         orphan_file.destination = file_without_first_part.with_stem(
-                            f"{match_path.stem}-{ORPHAN_ARCHIVE}"
+                            f"{match_path.stem}-{ORPHAN_ARCHIVE}",
                         )
                     else:
                         orphan_file.destination = file_without_first_part
                     matched_files.append(orphan_file)
             else:
                 matched_files.extend(originals_first)
         else:
             unmatched_files.extend(single_or_pair)
 
 
-def _handle_items(fix: bool, move: bool, show_details: bool, title: str, collection: list[str | OrphanFile | Document]):
+def _handle_items(
+    fix: bool,
+    move: bool,
+    show_details: bool,
+    title: str,
+    collection: Sequence[str | OrphanFile | Document],
+):
     length = len(collection)
     which_function = print_error if length else print_success
     which_function(f"{title} (count: {length})")
     if not show_details:
         return
 
     # https://docs.python.org/3/library/shutil.html#shutil.copy2
-    copy_function = shutil.move if move else shutil.copy2
     msg = "Moving" if move else "Copying"
 
     dest_dir = DOWNLOAD_DESTINATION_DIR / title
     for item in collection:
         if not isinstance(item, OrphanFile):
             print(str(item))
             continue
@@ -249,15 +266,18 @@
             print_error(f"Not found: {item.source}")
             continue
 
         dest_file = dest_dir / item.destination
         dest_file.parent.mkdir(parents=True, exist_ok=True)
         print_success(f"{msg} {item.source} to {dest_file}")
 
-        copy_function(item.source, dest_file)
+        if move:
+            shutil.move(item.source, dest_file)
+        else:
+            shutil.copy2(item.source, dest_file)
 
 
 @task
 def delete_failed_duplicates(c, max_delete=100):
     """Delete records marked as duplicate but that cannot be downloaded. So the PDF files can be reimported."""
     session = requests.Session()
     session.headers.update({"authorization": f"token {paperless_token()}"})
```

### Comparing `conjuring-0.3.0/src/conjuring/spells/pre_commit.py` & `conjuring-0.4.0/src/conjuring/spells/pre_commit.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,29 +41,29 @@
     installed_hooks = [hook for hook in run_stdout(c, "ls .git/hooks", dry=False).splitlines() if ".sample" not in hook]
     c.run(f"pre-commit uninstall {get_hook_types(commit_msg, installed_hooks)}")
 
 
 @task(
     help={
         "hooks": "Comma-separated list of partial hook IDs (fzf will be used to match them)."
-        " Use 'all', '.' or '-' to run all hooks."
-    }
+        " Use 'all', '.' or '-' to run all hooks.",
+    },
 )
 def run(c, hooks):
     """Pre-commit run all hooks or a specific one. Don't stop on failures. Needs fzf and yq."""
     split_hooks = hooks.split(",")
     chosen_hooks = []
     for special in ("all", ".", "-"):
         if special in split_hooks:
             chosen_hooks.append("")
             break
     if not chosen_hooks:
         for partial_hook in split_hooks:
             chosen_hooks.append(
-                run_with_fzf(c, "yq e '.repos[].hooks[].id' .pre-commit-config.yaml", query=partial_hook, dry=False)
+                run_with_fzf(c, "yq e '.repos[].hooks[].id' .pre-commit-config.yaml", query=partial_hook, dry=False),
             )
 
     for chosen_hook in chosen_hooks:
         run_command(c, "pre-commit run --all-files", chosen_hook, warn=True)
 
 
 @task()
```

### Comparing `conjuring-0.3.0/src/conjuring/spells/shell.py` & `conjuring-0.4.0/src/conjuring/spells/shell.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,8 +32,7 @@
 @task
 def completion_uninstall(c, app):
     """Uninstall shell completion from both completion dirs."""
     for completion_dir in COMPLETION_DIRS:
         with c.cd(completion_dir):
             c.run(f"rm -v {app}*", warn=True)
     completion_list(c)
-    return
```

### Comparing `conjuring-0.3.0/src/conjuring/visibility.py` & `conjuring-0.4.0/src/conjuring/visibility.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from typing import Callable
 
 from invoke import Task
 
 POETRY_LINE = re.compile(r"\[tool\..*poetry\]")
 ShouldDisplayTasks = Callable[[], bool]
 
-always_visible: ShouldDisplayTasks = lambda: True
+
+def always_visible():
+    return True
 
 
 def has_pre_commit_config_yaml() -> bool:
     return Path(".pre-commit-config.yaml").exists()
 
 
 def is_home_dir() -> bool:
@@ -54,15 +56,15 @@
         help=None,
         pre=None,
         post=None,
         autoprint=False,
         iterable=None,
         incrementable=None,
         should_display: ShouldDisplayTasks = always_visible,
-    ):
+    ) -> None:
         self.should_display: ShouldDisplayTasks = should_display
         super().__init__(
             body,
             name,
             aliases,
             positional,
             optional,
```

### Comparing `conjuring-0.3.0/PKG-INFO` & `conjuring-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conjuring
-Version: 0.3.0
+Version: 0.4.0
 Summary: 🐍🤖 Reusable global Invoke tasks that can be merged with local project tasks
 Home-page: https://github.com/andreoliwa/conjuring
 License: MIT
 Keywords: invoke,tasks,automation,cli,python
 Author: W. Augusto Andreoli
 Author-email: andreoliwa@gmail.com
 Requires-Python: >=3.9,<4.0
```

