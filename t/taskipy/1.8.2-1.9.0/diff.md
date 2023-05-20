# Comparing `tmp/taskipy-1.8.2.tar.gz` & `tmp/taskipy-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskipy-1.8.2.tar", max compression
+gzip compressed data, was "taskipy-1.9.0.tar", max compression
```

## Comparing `taskipy-1.8.2.tar` & `taskipy-1.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1066 2021-05-14 14:43:29.817913 taskipy-1.8.2/LICENSE
--rw-r--r--   0        0        0     7746 2021-05-16 19:12:26.209480 taskipy-1.8.2/README.md
--rw-r--r--   0        0        0     2004 2021-09-08 12:15:41.355750 taskipy-1.8.2/pyproject.toml
--rw-r--r--   0        0        0        0 2021-05-14 14:43:29.819457 taskipy-1.8.2/taskipy/__init__.py
--rwxr-xr-x   0        0        0     1110 2021-05-14 17:15:51.514213 taskipy-1.8.2/taskipy/cli.py
--rw-r--r--   0        0        0     1850 2021-05-16 16:58:54.540172 taskipy-1.8.2/taskipy/exceptions.py
--rw-r--r--   0        0        0     1174 2021-05-16 16:58:54.540531 taskipy-1.8.2/taskipy/help.py
--rw-r--r--   0        0        0     2221 2021-05-16 16:58:54.541104 taskipy-1.8.2/taskipy/pyproject.py
--rw-r--r--   0        0        0     1516 2021-05-16 16:58:54.541660 taskipy-1.8.2/taskipy/task.py
--rw-r--r--   0        0        0     3463 2021-09-08 12:14:31.552996 taskipy-1.8.2/taskipy/task_runner.py
--rw-r--r--   0        0        0     8867 2021-09-08 12:15:41.731013 taskipy-1.8.2/setup.py
--rw-r--r--   0        0        0     8702 2021-09-08 12:15:41.731361 taskipy-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2021-05-14 14:43:29.817913 taskipy-1.9.0/LICENSE
+-rw-r--r--   0        0        0     9940 2021-09-27 16:36:10.998458 taskipy-1.9.0/README.md
+-rw-r--r--   0        0        0     2004 2021-09-27 16:37:50.198356 taskipy-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-05-14 14:43:29.819457 taskipy-1.9.0/taskipy/__init__.py
+-rwxr-xr-x   0        0        0     1110 2021-05-14 17:15:51.514213 taskipy-1.9.0/taskipy/cli.py
+-rw-r--r--   0        0        0     1850 2021-05-16 16:58:54.540172 taskipy-1.9.0/taskipy/exceptions.py
+-rw-r--r--   0        0        0     1174 2021-05-16 16:58:54.540531 taskipy-1.9.0/taskipy/help.py
+-rw-r--r--   0        0        0     2301 2021-09-27 16:15:44.979668 taskipy-1.9.0/taskipy/pyproject.py
+-rw-r--r--   0        0        0     2266 2021-09-27 16:15:44.980521 taskipy-1.9.0/taskipy/task.py
+-rw-r--r--   0        0        0     3793 2021-09-27 16:15:44.981379 taskipy-1.9.0/taskipy/task_runner.py
+-rw-r--r--   0        0        0    11125 2021-09-27 16:37:50.583247 taskipy-1.9.0/setup.py
+-rw-r--r--   0        0        0    10896 2021-09-27 16:37:50.583648 taskipy-1.9.0/PKG-INFO
```

### Comparing `taskipy-1.8.2/LICENSE` & `taskipy-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskipy-1.8.2/README.md` & `taskipy-1.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,52 @@
+Metadata-Version: 2.1
+Name: taskipy
+Version: 1.9.0
+Summary: tasks runner for python projects
+Home-page: https://github.com/illBeRoy/taskipy
+License: MIT
+Keywords: tasks,task runner,development
+Author: Roy Sommer
+Author-email: roy@sommer.co.il
+Requires-Python: >=3.6,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Build Tools
+Requires-Dist: colorama (>=0.4.4,<0.5.0)
+Requires-Dist: mslex (>=0.3.0,<0.4.0); sys_platform == "win32"
+Requires-Dist: psutil (>=5.7.2,<6.0.0)
+Requires-Dist: toml (>=0.10.0,<0.11.0)
+Project-URL: Repository, https://github.com/illBeRoy/taskipy
+Description-Content-Type: text/markdown
+
 <p align="center">
 
 <img src="https://github.com/illBeRoy/taskipy/raw/master/logo.svg" width="150" />
 
 </p>
 
+- [General](#general)
+- [Requirements](#requirements)
+- [Usage](#usage)
+  * [Installation](#installation)
+  * [Adding Tasks](#adding-tasks)
+  * [Running Tasks](#running-tasks)
+  * [Passing Command Line Args to Tasks](#passing-command-line-args-to-tasks)
+  * [Composing Tasks](#composing-tasks)
+  * [Using Variables](#using-variables)
+  * [Using Taskipy Without Poetry](#using-taskipy-without-poetry)
+  * [Advanced Use Cases](#advanced-use-cases)
+- [Maintainers 🚧](#maintainers---)
+- [Contributors ✨](#contributors--)
+
 ## General
 [![pypi](https://img.shields.io/pypi/v/taskipy?style=flat-square)](https://pypi.org/project/taskipy/)
 [![ci](https://img.shields.io/github/workflow/status/illberoy/taskipy/Taskipy%20Test%20CI?style=flat-square)](https://github.com/illBeRoy/taskipy/actions?query=workflow%3A%22Taskipy+Test+CI%22)
 [![All Contributors](https://img.shields.io/github/all-contributors/illberoy/taskipy?color=orange&style=flat-square)](#contributors-)
 
 **The complementary task runner for python.**
 
@@ -155,14 +194,61 @@
 test = "python -m unittest tests/test_*.py"
 post_test = "task lint"
 lint = "pylint tests taskipy"
 ```
 
 The posttask hook looks for `post_<task_name>` task for a given `task_name`. It will run it after running the task itself. If the task failed, then taskipy will not run the posttask hook.
 
+### Using Variables
+In some cases, you might find yourself passing the same arguments over and over again. Let us take a look at the following tasks:
+
+```toml
+[tool.taskipy.tasks]
+lint = "pylint path/to/my_module"
+black = "black path/to/my_module"
+```
+
+As you can see, we provide the same path argument to both `pylint` and `black`.
+
+In order to encourage DRY and improve your ability to change these values later on, taskipy actually lets you declare and reuse variables in your tasks:
+
+```toml
+[tool.taskipy.variables]
+path = "path/to/my_module"
+
+[tool.taskipy.tasks]
+lint = { cmd = "pylint {path}", use_vars = true }
+black = { cmd = "pylint {path}", use_vars = true }
+```
+
+We have made the following changes to our configuration:
+1. We declared variables under `tool.taskipy.variables`
+2. We flagged the relevant task using `use_vars` to note that they should use the variables
+3. We replaced the repeating path with a `{path}` variable
+
+#### String Formatting
+The formatting of the task commands uses python's own `string.format` method, and therefore supports everything that python's [formatted string literals](https://docs.python.org/3/tutorial/inputoutput.html#formatted-string-literals) let you do.
+
+#### Always Use Variables
+Using variables is opt-in, which means that by default commands do **not** use them, and you will have to turn them on a task to task basis.
+
+If you want to turn on `use_vars` globally, all you need to do is to declare that under taskipy's **settings** table:
+
+```toml
+[tool.taskipy.settings]
+use_vars = true
+
+[tool.taskipy.variables]
+path = "path/to/my_module"
+
+[tool.taskipy.tasks]
+lint = "pylint {path}"
+black = "black {path}"
+```
+
 ### Using Taskipy Without Poetry
 Taskipy was created with poetry projects in mind, but actually only requires a valid `pyproject.toml` file in your project's directory. As a result, you can use it even eithout poetry:
 
 #### Installing With PIP
 Install taskipy on your machine or in your virtualenv using:
 ```bash
 pip install taskipy
@@ -202,7 +288,8 @@
 </table>
 
 <!-- markdownlint-enable -->
 <!-- prettier-ignore-end -->
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
+
```

### Comparing `taskipy-1.8.2/pyproject.toml` & `taskipy-1.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "taskipy"
 description = "tasks runner for python projects"
-version = "1.8.2"
+version = "1.9.0"
 authors = ["Roy Sommer <roy@sommer.co.il>"]
 readme = "README.md"
 repository = "https://github.com/illBeRoy/taskipy"
 license = "MIT"
 keywords = ["tasks", "task runner", "development"]
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `taskipy-1.8.2/taskipy/cli.py` & `taskipy-1.9.0/taskipy/cli.py`

 * *Files identical despite different names*

### Comparing `taskipy-1.8.2/taskipy/exceptions.py` & `taskipy-1.9.0/taskipy/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskipy-1.8.2/taskipy/help.py` & `taskipy-1.9.0/taskipy/help.py`

 * *Files identical despite different names*

### Comparing `taskipy-1.8.2/taskipy/pyproject.py` & `taskipy-1.9.0/taskipy/pyproject.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from typing import Any, Dict, MutableMapping, Optional, Union
 
 from taskipy.task import Task
 from taskipy.exceptions import (
     InvalidRunnerTypeError,
     MalformedPyProjectError,
     MissingPyProjectFileError,
-    MissingTaskipyTasksSectionError,
-    MissingTaskipySettingsSectionError
+    MissingTaskipyTasksSectionError
 )
 
 
 class PyProject:
     def __init__(self, base_dir: Path):
         pyproject_path = self.__find_pyproject_path(base_dir)
         self.__items = PyProject.__load_toml_file(pyproject_path)
@@ -24,30 +23,37 @@
             return {
                 task_name: Task(task_name, task_toml_contents) for
                 task_name, task_toml_contents in self.__items['tool']['taskipy']['tasks'].items() }
         except KeyError:
             raise MissingTaskipyTasksSectionError()
 
     @property
+    def variables(self) -> Dict[str, Task]:
+        try:
+            return self.__items['tool']['taskipy'].get('variables', {})
+        except KeyError:
+            return {}
+
+    @property
     def settings(self) -> dict:
         try:
             return self.__items['tool']['taskipy']['settings']
         except KeyError:
-            raise MissingTaskipySettingsSectionError()
+            return {}
 
     @property
     def runner(self) -> Optional[str]:
         try:
             runner = self.settings['runner']
 
             if not isinstance(runner, str):
                 raise InvalidRunnerTypeError()
 
             return runner.strip()
-        except (KeyError, MissingTaskipySettingsSectionError):
+        except KeyError:
             return None
 
     @staticmethod
     def __load_toml_file(file_path: Union[str, Path]) -> MutableMapping[str, Any]:
         try:
             if isinstance(file_path, str):
                 file_path = Path(file_path).resolve()
```

### Comparing `taskipy-1.8.2/taskipy/task.py` & `taskipy-1.9.0/taskipy/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,43 +2,58 @@
 
 
 class Task:
     def __init__(self, task_name: str, task_toml_contents: object):
         self.__task_name = task_name
         self.__task_command = self.__extract_task_command(task_toml_contents)
         self.__task_description = self.__extract_task_description(task_toml_contents)
+        self.__task_use_vars = self.__extract_task_use_vars(task_toml_contents)
 
     @property
     def name(self):
         return self.__task_name
 
     @property
     def command(self):
         return self.__task_command
 
     @property
     def description(self):
         return self.__task_description
 
+    @property
+    def use_vars(self):
+        return self.__task_use_vars
+
+    def __extract_task_use_vars(self, task_toml_contents: object) -> bool:
+        if isinstance(task_toml_contents, str):
+            return False
+        if isinstance(task_toml_contents, dict):
+            value = task_toml_contents.get('use_vars', False)
+            if not isinstance(value, bool):
+                raise MalformedTaskError(self.__task_name, f'task\'s "use_vars" arg has to be bool type got {type(value)}')
+            return value
+        raise MalformedTaskError(self.__task_name, 'tasks must be strings, or dicts that contain { cmd, help, use_vars }')
+
     def __extract_task_command(self, task_toml_contents: object) -> str:
         if isinstance(task_toml_contents, str):
             return task_toml_contents
 
         if isinstance(task_toml_contents, dict):
             try:
                 return task_toml_contents['cmd']
             except KeyError:
                 raise MalformedTaskError(self.__task_name, 'the task item does not have the "cmd" property')
 
-        raise MalformedTaskError(self.__task_name, 'tasks must be strings, or dicts that contain { cmd, help }')
+        raise MalformedTaskError(self.__task_name, 'tasks must be strings, or dicts that contain { cmd, help, use_vars }')
 
     def __extract_task_description(self, task_toml_contents: object) -> str:
         if isinstance(task_toml_contents, str):
             return ''
 
         if isinstance(task_toml_contents, dict):
             try:
                 return task_toml_contents['help']
             except KeyError:
                 return ''
 
-        raise MalformedTaskError(self.__task_name, 'tasks must be strings, or dicts that contain { cmd, help }')
+        raise MalformedTaskError(self.__task_name, 'tasks must be strings, or dicts that contain { cmd, help, use_vars}')
```

### Comparing `taskipy-1.8.2/taskipy/task_runner.py` & `taskipy-1.9.0/taskipy/task_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import psutil  # type: ignore
 import signal
 import subprocess
 from pathlib import Path
 from typing import List, Union, Optional
 
 from taskipy.pyproject import PyProject
-from taskipy.exceptions import TaskNotFoundError
+from taskipy.exceptions import TaskNotFoundError, MalformedTaskError
 from taskipy.task import Task
 from taskipy.help import HelpFormatter
 
 if platform.system() == 'Windows':
     import mslex as shlex  # type: ignore # pylint: disable=E0401
 else:
     import shlex  # type: ignore[no-redef]
@@ -32,34 +32,41 @@
         try:
             task = self.__project.tasks[task_name]
         except KeyError:
             raise TaskNotFoundError(task_name)
 
         pre_task = self.__pre_task(task_name)
         if pre_task is not None:
-            exit_code = self.__run_command_and_return_exit_code(pre_task.command)
+            exit_code = self.__run_command_and_return_exit_code(pre_task)
             if exit_code != 0:
                 return exit_code
 
-        exit_code = self.__run_command_and_return_exit_code(task.command, args)
+        exit_code = self.__run_command_and_return_exit_code(task, args)
         if exit_code != 0:
             return exit_code
 
         post_task = self.__post_task(task_name)
         if post_task is not None:
-            exit_code = self.__run_command_and_return_exit_code(post_task.command)
+            exit_code = self.__run_command_and_return_exit_code(post_task)
             if exit_code != 0:
                 return exit_code
 
         return 0
 
-    def __run_command_and_return_exit_code(self, command: str, args: List[str] = None) -> int:
+    def __run_command_and_return_exit_code(self, task: Task, args: List[str] = None) -> int:
         if args is None:
             args = []
 
+        command = task.command
+        if task.use_vars or self.__project.settings.get('use_vars', {}):
+            try:
+                command = command.format(**self.__project.variables)
+            except KeyError as e:
+                raise MalformedTaskError(task.name, f"{e} variable expected in [pyproject.taskipy.variables]")
+
         if self.__project.runner is not None:
             command = f'{self.__project.runner} {command}'
 
         def send_signal_to_task_process(signum: int, _frame) -> None:
             # pylint: disable=W0640
             psutil_process_wrapper = psutil.Process(process.pid)
             is_direct_subprocess_a_shell_process = sys.platform != 'darwin'  # pylint: disable=C0103
```

### Comparing `taskipy-1.8.2/setup.py` & `taskipy-1.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 {':sys_platform == "win32"': ['mslex>=0.3.0,<0.4.0']}
 
 entry_points = \
 {'console_scripts': ['task = taskipy.cli:main']}
 
 setup_kwargs = {
     'name': 'taskipy',
-    'version': '1.8.2',
+    'version': '1.9.0',
     'description': 'tasks runner for python projects',
-    'long_description': '<p align="center">\n\n<img src="https://github.com/illBeRoy/taskipy/raw/master/logo.svg" width="150" />\n\n</p>\n\n## General\n[![pypi](https://img.shields.io/pypi/v/taskipy?style=flat-square)](https://pypi.org/project/taskipy/)\n[![ci](https://img.shields.io/github/workflow/status/illberoy/taskipy/Taskipy%20Test%20CI?style=flat-square)](https://github.com/illBeRoy/taskipy/actions?query=workflow%3A%22Taskipy+Test+CI%22)\n[![All Contributors](https://img.shields.io/github/all-contributors/illberoy/taskipy?color=orange&style=flat-square)](#contributors-)\n\n**The complementary task runner for python.**\n\nEvery development pipeline has tasks, such as `test`, `lint` or `publish`. With taskipy, you can define those tasks in one file and run them with a simple command.\n\nFor instance, instead of running the following command:\n```bash\npython -m unittest tests/test_*.py\n```\n\nYou can create a task called `test` and simply run:\n```bash\npoetry run task test\n```\n\nOr (if you\'re not using poetry):\n```bash\ntask test\n```\n\nIn addition, you can compose tasks and group them together, and also create dependencies between them.\n\nThis project is heavily inspired by npm\'s [run script command](https://docs.npmjs.com/cli/run-script).\n\n## Requirements\nPython 3.6 or newer.\n\nYour project directory should include a valid `pyproject.toml` file, as specified in [PEP-518](https://www.python.org/dev/peps/pep-0518/).\n\n## Usage\n### Installation\nTo install taskipy as a dev dependency, simply run:\n```bash\npoetry add --dev taskipy\n```\n\n### Adding Tasks \nIn your `pyproject.toml` file, add a new section called `[tool.taskipy.tasks]`.\n\nThe section is a key-value map, from the names of the task to the actual command that should be run in the shell.\n\nThere are two ways to define tasks. The easy way is to simply write the command down as a string:\n\n__pyproject.toml__\n```toml\n[tool.taskipy.tasks]\ntest = "python -m unittest tests/test_*.py"\nlint = "pylint tests taskipy"\n```\n\nAlternatively, you can define tasks more explicitly by declaring both the command and a helpful description using an inline table:\n\n__pyproject.toml__\n```toml\n[tool.taskipy.tasks]\ntest = { cmd = "python -m unittest tests/test_*.py", help = "runs all unit tests" }\nlint = { cmd = "pylint tests taskipy", help = "confirms code style using pylint" } \n```\n\nThe explicit notation is more verbose, but provides better context to anyone who uses the task.\n\n### Running Tasks\nIn order to run a task, run the following command in your terminal:\n```bash\n$ poetry run task test\n```\n\nYou can also list all existing tasks by running the following:\n```bash\n$ poetry run task --list\ntest                python -m unittest tests/test_*.py\nlint                pylint tests taskipy\n```\n\nIf you declared your task explicitly, you will see the description of the task by the side of the task\'s name:\n```bash\n$ poetry run task --list\ntest                runs all unit tests\nlint                confirms code style using pylint\n```\n\n### Passing Command Line Args to Tasks\nIf you want to pass command line arguments to tasks (positional or named), simply append them to the end of the task command.\n\nFor example, running the above task like this:\n```bash\npoetry run task test -h\n```\n\nIs equivalent to running:\n```bash\npython -m unittest tests/test_*.py -h\n```\n\nAnd will show unittest\'s help instead of actually running it.\n\n> ⚠️ Note: if you are using pre \\ post hooks, do notice that arguments are not passed to them, only to the task itself.\n\n### Composing Tasks\n#### Grouping Subtasks Together\nSome tasks are composed of multiple subtasks. Instead of writing plain shell commands and stringing them together, you can break them down into multiple subtasks:\n```toml\n[tool.taskipy.tasks]\nlint_pylint = "pylint tests taskipy"\nlint_mypy = "mypy tests taskipy"\n```\n\nAnd then create a composite task:\n```toml\n[tool.taskipy.tasks]\nlint = "task lint_pylint && task lint_mypy"\nlint_pylint = "pylint tests taskipy"\nlint_mypy = "mypy tests taskipy"\n```\n\n#### Pre Task Hook\nTasks might also depend on one another. For example, tests might require some binaries to be built. Take the two following commands, for instance:\n```toml\n[tool.taskipy.tasks]\ntest = "python -m unittest tests/test_*.py"\nbuild = "make ."\n```\n\nYou could make tests depend on building, by using the **pretask hook**:\n```toml\n[tool.taskipy.tasks]\npre_test = "task build"\ntest = "python -m unittest tests/test_*.py"\nbuild = "make ."\n```\n\nThe pretask hook looks for `pre_<task_name>` task for a given `task_name`. It will run it before running the task itself. If the pretask fails, then taskipy will exit without running the task itself.\n\n#### Post Task Hook\nFrom time to time, you might want to run a task in conjuction with another. For example, you might want to run linting after a successful test run. Take the two following commands, for instance:\n```toml\n[tool.taskipy.tasks]\ntest = "python -m unittest tests/test_*.py"\nlint = "pylint tests taskipy"\n```\n\nYou could make tests trigger linting, by using the **posttask hook**:\n```toml\n[tool.taskipy.tasks]\ntest = "python -m unittest tests/test_*.py"\npost_test = "task lint"\nlint = "pylint tests taskipy"\n```\n\nThe posttask hook looks for `post_<task_name>` task for a given `task_name`. It will run it after running the task itself. If the task failed, then taskipy will not run the posttask hook.\n\n### Using Taskipy Without Poetry\nTaskipy was created with poetry projects in mind, but actually only requires a valid `pyproject.toml` file in your project\'s directory. As a result, you can use it even eithout poetry:\n\n#### Installing With PIP\nInstall taskipy on your machine or in your virtualenv using:\n```bash\npip install taskipy\n```\n\n#### Running Tasks\nHead into your project\'s directory (don\'t forget to activate virtualenv if you\'re using one), and run the following command:\n```bash\ntask TASK\n```\nWhere `TASK` is the name of your task.\n\n### Advanced Use Cases\nIf you have a more specific use case, you might not be the first to run into it! Head over to the [ADVANCED_FEATURES](./docs/ADVANCED_FEATURES.md) doc, and look it up.\n\n## Maintainers 🚧\n\n<table>\n  <tr>\n    <td align="center"><a href="https://github.com/illBeRoy"><img src="https://avatars2.githubusercontent.com/u/6681893?v=4" width="100px;" alt=""/><br /><sub><b>Roy Sommer</b></sub></a></td>\n  </tr>\n</table>\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tr>\n    <td align="center"><a href="http://triguba.com"><img src="https://avatars3.githubusercontent.com/u/15860938?v=4" width="100px;" alt=""/><br /><sub><b>Eugene Triguba</b></sub></a><br /><a href="https://github.com/illBeRoy/taskipy/commits?author=eugenetriguba" title="Code">💻</a></td>\n    <td align="center"><a href="https://github.com/RobinFrcd"><img src="https://avatars0.githubusercontent.com/u/29704178?v=4" width="100px;" alt=""/><br /><sub><b>RobinFrcd</b></sub></a><br /><a href="https://github.com/illBeRoy/taskipy/commits?author=RobinFrcd" title="Code">💻</a></td>\n    <td align="center"><a href="http://granitosaurus.rocks"><img src="https://avatars0.githubusercontent.com/u/5476164?v=4" width="100px;" alt=""/><br /><sub><b>Bernardas Ališauskas</b></sub></a><br /><a href="https://github.com/illBeRoy/taskipy/commits?author=Granitosaurus" title="Code">💻</a></td>\n  </tr>\n</table>\n\n<!-- markdownlint-enable -->\n<!-- prettier-ignore-end -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n',
+    'long_description': '<p align="center">\n\n<img src="https://github.com/illBeRoy/taskipy/raw/master/logo.svg" width="150" />\n\n</p>\n\n- [General](#general)\n- [Requirements](#requirements)\n- [Usage](#usage)\n  * [Installation](#installation)\n  * [Adding Tasks](#adding-tasks)\n  * [Running Tasks](#running-tasks)\n  * [Passing Command Line Args to Tasks](#passing-command-line-args-to-tasks)\n  * [Composing Tasks](#composing-tasks)\n  * [Using Variables](#using-variables)\n  * [Using Taskipy Without Poetry](#using-taskipy-without-poetry)\n  * [Advanced Use Cases](#advanced-use-cases)\n- [Maintainers 🚧](#maintainers---)\n- [Contributors ✨](#contributors--)\n\n## General\n[![pypi](https://img.shields.io/pypi/v/taskipy?style=flat-square)](https://pypi.org/project/taskipy/)\n[![ci](https://img.shields.io/github/workflow/status/illberoy/taskipy/Taskipy%20Test%20CI?style=flat-square)](https://github.com/illBeRoy/taskipy/actions?query=workflow%3A%22Taskipy+Test+CI%22)\n[![All Contributors](https://img.shields.io/github/all-contributors/illberoy/taskipy?color=orange&style=flat-square)](#contributors-)\n\n**The complementary task runner for python.**\n\nEvery development pipeline has tasks, such as `test`, `lint` or `publish`. With taskipy, you can define those tasks in one file and run them with a simple command.\n\nFor instance, instead of running the following command:\n```bash\npython -m unittest tests/test_*.py\n```\n\nYou can create a task called `test` and simply run:\n```bash\npoetry run task test\n```\n\nOr (if you\'re not using poetry):\n```bash\ntask test\n```\n\nIn addition, you can compose tasks and group them together, and also create dependencies between them.\n\nThis project is heavily inspired by npm\'s [run script command](https://docs.npmjs.com/cli/run-script).\n\n## Requirements\nPython 3.6 or newer.\n\nYour project directory should include a valid `pyproject.toml` file, as specified in [PEP-518](https://www.python.org/dev/peps/pep-0518/).\n\n## Usage\n### Installation\nTo install taskipy as a dev dependency, simply run:\n```bash\npoetry add --dev taskipy\n```\n\n### Adding Tasks \nIn your `pyproject.toml` file, add a new section called `[tool.taskipy.tasks]`.\n\nThe section is a key-value map, from the names of the task to the actual command that should be run in the shell.\n\nThere are two ways to define tasks. The easy way is to simply write the command down as a string:\n\n__pyproject.toml__\n```toml\n[tool.taskipy.tasks]\ntest = "python -m unittest tests/test_*.py"\nlint = "pylint tests taskipy"\n```\n\nAlternatively, you can define tasks more explicitly by declaring both the command and a helpful description using an inline table:\n\n__pyproject.toml__\n```toml\n[tool.taskipy.tasks]\ntest = { cmd = "python -m unittest tests/test_*.py", help = "runs all unit tests" }\nlint = { cmd = "pylint tests taskipy", help = "confirms code style using pylint" } \n```\n\nThe explicit notation is more verbose, but provides better context to anyone who uses the task.\n\n### Running Tasks\nIn order to run a task, run the following command in your terminal:\n```bash\n$ poetry run task test\n```\n\nYou can also list all existing tasks by running the following:\n```bash\n$ poetry run task --list\ntest                python -m unittest tests/test_*.py\nlint                pylint tests taskipy\n```\n\nIf you declared your task explicitly, you will see the description of the task by the side of the task\'s name:\n```bash\n$ poetry run task --list\ntest                runs all unit tests\nlint                confirms code style using pylint\n```\n\n### Passing Command Line Args to Tasks\nIf you want to pass command line arguments to tasks (positional or named), simply append them to the end of the task command.\n\nFor example, running the above task like this:\n```bash\npoetry run task test -h\n```\n\nIs equivalent to running:\n```bash\npython -m unittest tests/test_*.py -h\n```\n\nAnd will show unittest\'s help instead of actually running it.\n\n> ⚠️ Note: if you are using pre \\ post hooks, do notice that arguments are not passed to them, only to the task itself.\n\n### Composing Tasks\n#### Grouping Subtasks Together\nSome tasks are composed of multiple subtasks. Instead of writing plain shell commands and stringing them together, you can break them down into multiple subtasks:\n```toml\n[tool.taskipy.tasks]\nlint_pylint = "pylint tests taskipy"\nlint_mypy = "mypy tests taskipy"\n```\n\nAnd then create a composite task:\n```toml\n[tool.taskipy.tasks]\nlint = "task lint_pylint && task lint_mypy"\nlint_pylint = "pylint tests taskipy"\nlint_mypy = "mypy tests taskipy"\n```\n\n#### Pre Task Hook\nTasks might also depend on one another. For example, tests might require some binaries to be built. Take the two following commands, for instance:\n```toml\n[tool.taskipy.tasks]\ntest = "python -m unittest tests/test_*.py"\nbuild = "make ."\n```\n\nYou could make tests depend on building, by using the **pretask hook**:\n```toml\n[tool.taskipy.tasks]\npre_test = "task build"\ntest = "python -m unittest tests/test_*.py"\nbuild = "make ."\n```\n\nThe pretask hook looks for `pre_<task_name>` task for a given `task_name`. It will run it before running the task itself. If the pretask fails, then taskipy will exit without running the task itself.\n\n#### Post Task Hook\nFrom time to time, you might want to run a task in conjuction with another. For example, you might want to run linting after a successful test run. Take the two following commands, for instance:\n```toml\n[tool.taskipy.tasks]\ntest = "python -m unittest tests/test_*.py"\nlint = "pylint tests taskipy"\n```\n\nYou could make tests trigger linting, by using the **posttask hook**:\n```toml\n[tool.taskipy.tasks]\ntest = "python -m unittest tests/test_*.py"\npost_test = "task lint"\nlint = "pylint tests taskipy"\n```\n\nThe posttask hook looks for `post_<task_name>` task for a given `task_name`. It will run it after running the task itself. If the task failed, then taskipy will not run the posttask hook.\n\n### Using Variables\nIn some cases, you might find yourself passing the same arguments over and over again. Let us take a look at the following tasks:\n\n```toml\n[tool.taskipy.tasks]\nlint = "pylint path/to/my_module"\nblack = "black path/to/my_module"\n```\n\nAs you can see, we provide the same path argument to both `pylint` and `black`.\n\nIn order to encourage DRY and improve your ability to change these values later on, taskipy actually lets you declare and reuse variables in your tasks:\n\n```toml\n[tool.taskipy.variables]\npath = "path/to/my_module"\n\n[tool.taskipy.tasks]\nlint = { cmd = "pylint {path}", use_vars = true }\nblack = { cmd = "pylint {path}", use_vars = true }\n```\n\nWe have made the following changes to our configuration:\n1. We declared variables under `tool.taskipy.variables`\n2. We flagged the relevant task using `use_vars` to note that they should use the variables\n3. We replaced the repeating path with a `{path}` variable\n\n#### String Formatting\nThe formatting of the task commands uses python\'s own `string.format` method, and therefore supports everything that python\'s [formatted string literals](https://docs.python.org/3/tutorial/inputoutput.html#formatted-string-literals) let you do.\n\n#### Always Use Variables\nUsing variables is opt-in, which means that by default commands do **not** use them, and you will have to turn them on a task to task basis.\n\nIf you want to turn on `use_vars` globally, all you need to do is to declare that under taskipy\'s **settings** table:\n\n```toml\n[tool.taskipy.settings]\nuse_vars = true\n\n[tool.taskipy.variables]\npath = "path/to/my_module"\n\n[tool.taskipy.tasks]\nlint = "pylint {path}"\nblack = "black {path}"\n```\n\n### Using Taskipy Without Poetry\nTaskipy was created with poetry projects in mind, but actually only requires a valid `pyproject.toml` file in your project\'s directory. As a result, you can use it even eithout poetry:\n\n#### Installing With PIP\nInstall taskipy on your machine or in your virtualenv using:\n```bash\npip install taskipy\n```\n\n#### Running Tasks\nHead into your project\'s directory (don\'t forget to activate virtualenv if you\'re using one), and run the following command:\n```bash\ntask TASK\n```\nWhere `TASK` is the name of your task.\n\n### Advanced Use Cases\nIf you have a more specific use case, you might not be the first to run into it! Head over to the [ADVANCED_FEATURES](./docs/ADVANCED_FEATURES.md) doc, and look it up.\n\n## Maintainers 🚧\n\n<table>\n  <tr>\n    <td align="center"><a href="https://github.com/illBeRoy"><img src="https://avatars2.githubusercontent.com/u/6681893?v=4" width="100px;" alt=""/><br /><sub><b>Roy Sommer</b></sub></a></td>\n  </tr>\n</table>\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tr>\n    <td align="center"><a href="http://triguba.com"><img src="https://avatars3.githubusercontent.com/u/15860938?v=4" width="100px;" alt=""/><br /><sub><b>Eugene Triguba</b></sub></a><br /><a href="https://github.com/illBeRoy/taskipy/commits?author=eugenetriguba" title="Code">💻</a></td>\n    <td align="center"><a href="https://github.com/RobinFrcd"><img src="https://avatars0.githubusercontent.com/u/29704178?v=4" width="100px;" alt=""/><br /><sub><b>RobinFrcd</b></sub></a><br /><a href="https://github.com/illBeRoy/taskipy/commits?author=RobinFrcd" title="Code">💻</a></td>\n    <td align="center"><a href="http://granitosaurus.rocks"><img src="https://avatars0.githubusercontent.com/u/5476164?v=4" width="100px;" alt=""/><br /><sub><b>Bernardas Ališauskas</b></sub></a><br /><a href="https://github.com/illBeRoy/taskipy/commits?author=Granitosaurus" title="Code">💻</a></td>\n  </tr>\n</table>\n\n<!-- markdownlint-enable -->\n<!-- prettier-ignore-end -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n',
     'author': 'Roy Sommer',
     'author_email': 'roy@sommer.co.il',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/illBeRoy/taskipy',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `taskipy-1.8.2/PKG-INFO` & `taskipy-1.9.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,27 @@
-Metadata-Version: 2.1
-Name: taskipy
-Version: 1.8.2
-Summary: tasks runner for python projects
-Home-page: https://github.com/illBeRoy/taskipy
-License: MIT
-Keywords: tasks,task runner,development
-Author: Roy Sommer
-Author-email: roy@sommer.co.il
-Requires-Python: >=3.6,<4.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Build Tools
-Requires-Dist: colorama (>=0.4.4,<0.5.0)
-Requires-Dist: mslex (>=0.3.0,<0.4.0); sys_platform == "win32"
-Requires-Dist: psutil (>=5.7.2,<6.0.0)
-Requires-Dist: toml (>=0.10.0,<0.11.0)
-Project-URL: Repository, https://github.com/illBeRoy/taskipy
-Description-Content-Type: text/markdown
-
 <p align="center">
 
 <img src="https://github.com/illBeRoy/taskipy/raw/master/logo.svg" width="150" />
 
 </p>
 
+- [General](#general)
+- [Requirements](#requirements)
+- [Usage](#usage)
+  * [Installation](#installation)
+  * [Adding Tasks](#adding-tasks)
+  * [Running Tasks](#running-tasks)
+  * [Passing Command Line Args to Tasks](#passing-command-line-args-to-tasks)
+  * [Composing Tasks](#composing-tasks)
+  * [Using Variables](#using-variables)
+  * [Using Taskipy Without Poetry](#using-taskipy-without-poetry)
+  * [Advanced Use Cases](#advanced-use-cases)
+- [Maintainers 🚧](#maintainers---)
+- [Contributors ✨](#contributors--)
+
 ## General
 [![pypi](https://img.shields.io/pypi/v/taskipy?style=flat-square)](https://pypi.org/project/taskipy/)
 [![ci](https://img.shields.io/github/workflow/status/illberoy/taskipy/Taskipy%20Test%20CI?style=flat-square)](https://github.com/illBeRoy/taskipy/actions?query=workflow%3A%22Taskipy+Test+CI%22)
 [![All Contributors](https://img.shields.io/github/all-contributors/illberoy/taskipy?color=orange&style=flat-square)](#contributors-)
 
 **The complementary task runner for python.**
 
@@ -180,14 +169,61 @@
 test = "python -m unittest tests/test_*.py"
 post_test = "task lint"
 lint = "pylint tests taskipy"
 ```
 
 The posttask hook looks for `post_<task_name>` task for a given `task_name`. It will run it after running the task itself. If the task failed, then taskipy will not run the posttask hook.
 
+### Using Variables
+In some cases, you might find yourself passing the same arguments over and over again. Let us take a look at the following tasks:
+
+```toml
+[tool.taskipy.tasks]
+lint = "pylint path/to/my_module"
+black = "black path/to/my_module"
+```
+
+As you can see, we provide the same path argument to both `pylint` and `black`.
+
+In order to encourage DRY and improve your ability to change these values later on, taskipy actually lets you declare and reuse variables in your tasks:
+
+```toml
+[tool.taskipy.variables]
+path = "path/to/my_module"
+
+[tool.taskipy.tasks]
+lint = { cmd = "pylint {path}", use_vars = true }
+black = { cmd = "pylint {path}", use_vars = true }
+```
+
+We have made the following changes to our configuration:
+1. We declared variables under `tool.taskipy.variables`
+2. We flagged the relevant task using `use_vars` to note that they should use the variables
+3. We replaced the repeating path with a `{path}` variable
+
+#### String Formatting
+The formatting of the task commands uses python's own `string.format` method, and therefore supports everything that python's [formatted string literals](https://docs.python.org/3/tutorial/inputoutput.html#formatted-string-literals) let you do.
+
+#### Always Use Variables
+Using variables is opt-in, which means that by default commands do **not** use them, and you will have to turn them on a task to task basis.
+
+If you want to turn on `use_vars` globally, all you need to do is to declare that under taskipy's **settings** table:
+
+```toml
+[tool.taskipy.settings]
+use_vars = true
+
+[tool.taskipy.variables]
+path = "path/to/my_module"
+
+[tool.taskipy.tasks]
+lint = "pylint {path}"
+black = "black {path}"
+```
+
 ### Using Taskipy Without Poetry
 Taskipy was created with poetry projects in mind, but actually only requires a valid `pyproject.toml` file in your project's directory. As a result, you can use it even eithout poetry:
 
 #### Installing With PIP
 Install taskipy on your machine or in your virtualenv using:
 ```bash
 pip install taskipy
@@ -227,8 +263,7 @@
 </table>
 
 <!-- markdownlint-enable -->
 <!-- prettier-ignore-end -->
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
-
```

