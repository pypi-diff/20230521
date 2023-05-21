# Comparing `tmp/llm_code-0.2.tar.gz` & `tmp/llm_code-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_code-0.2.tar", max compression
+gzip compressed data, was "llm_code-0.3.tar", max compression
```

## Comparing `llm_code-0.2.tar` & `llm_code-0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-05-19 17:43:32.824715 llm_code-0.2/LICENSE
--rw-r--r--   0        0        0     1833 2023-05-20 05:46:21.650675 llm_code-0.2/README.md
--rw-r--r--   0        0        0        0 2023-05-19 17:43:32.824978 llm_code-0.2/llm_code/__init__.py
--rw-r--r--   0        0        0     2696 2023-05-20 05:32:25.595648 llm_code-0.2/llm_code/llm_code.py
--rw-r--r--   0        0        0     3293 2023-05-19 22:57:07.356159 llm_code-0.2/llm_code/templates.py
--rw-r--r--   0        0        0      161 2023-05-19 18:26:22.445515 llm_code-0.2/prompts/coding/system.toml
--rw-r--r--   0        0        0      613 2023-05-19 18:23:27.578834 llm_code-0.2/prompts/coding/user/input.toml
--rw-r--r--   0        0        0      396 2023-05-19 18:19:43.905655 llm_code-0.2/prompts/coding/user/simple.toml
--rw-r--r--   0        0        0     1116 2023-05-20 05:58:54.951619 llm_code-0.2/pyproject.toml
--rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 llm_code-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-19 17:20:49.716226 llm_code-0.3/LICENSE
+-rw-r--r--   0        0        0     2933 2023-05-21 02:48:12.815312 llm_code-0.3/README.md
+-rw-r--r--   0        0        0       75 2023-05-21 03:18:50.955110 llm_code-0.3/llm_code/__init__.py
+-rw-r--r--   0        0        0     2949 2023-05-21 03:25:05.157471 llm_code-0.3/llm_code/llm_code.py
+-rw-r--r--   0        0        0     3293 2023-05-21 02:14:00.115437 llm_code-0.3/llm_code/templates.py
+-rw-r--r--   0        0        0      161 2023-05-21 02:14:00.117237 llm_code-0.3/prompts/coding/system.toml
+-rw-r--r--   0        0        0      613 2023-05-21 02:14:00.117511 llm_code-0.3/prompts/coding/user/input.toml
+-rw-r--r--   0        0        0      396 2023-05-21 02:14:00.117693 llm_code-0.3/prompts/coding/user/simple.toml
+-rw-r--r--   0        0        0     1132 2023-05-21 03:31:31.039632 llm_code-0.3/pyproject.toml
+-rw-r--r--   0        0        0     3865 1970-01-01 00:00:00.000000 llm_code-0.3/PKG-INFO
```

### Comparing `llm_code-0.2/LICENSE` & `llm_code-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_code-0.2/README.md` & `llm_code-0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,62 @@
 # llm-code
 
+![PyPi](https://img.shields.io/pypi/v/llm-code?color=green)
+[![Coverage Status](https://coveralls.io/repos/github/radoshi/llm-code/badge.svg?branch=main)](https://coveralls.io/github/radoshi/llm-code?branch=main)
+
+---
+
 An OpenAI LLM based CLI coding assistant.
 
 `llm-code` is inspired by
 [Simon Wilson](https://simonwillison.net/2023/May/18/cli-tools-for-llms/)'s
 [llm](https://github.com/simonw/llm) package. It takes a similar approach of developing
 a simple tool to create an LLM based assistant that helps write code.
 
 ## Installation
 
 ```bash
 pipx install llm-code
 ```
 
+## Configuration
+
+`llm-code` requires an OpenAI API key. You can get one from [OpenAI](https://openai.com/).
+
+You can set the key in a few different ways, depending on your preference:
+
+1. Set the `OPENAI_API_KEY` environment variable.
+
+```bash
+export OPENAI_API_KEY = sk-...
+```
+
+2. Use an env file in ~/.llm_code/env
+
+```bash
+mkdir -p ~/.llm_code
+echo "OPENAI_API_KEY=sk-..." > ~/.llm_code/env
+```
+
 ## Usage
 
+`llm-code` is meant to be simple to use. The default prompts should be good enough. There are two broad modes:
+
+1. Generage some code from scratch.
+
+```bash
+llm-code write a function that takes a list of numbers and returns the sum of the numbers in python. Add type hints.
+```
+
+2. Give in some input files and ask for changes.
+
+```bash
+llm-code -i my_file.py add docstrings to all python functions.
+```
+
 ```bash
 llm-code --help
 ```
 
 ```
 Usage: llm-code [OPTIONS] [INSTRUCTIONS]...
 
@@ -39,41 +77,47 @@
 
 ```rust
 fn main() {
     println!("Hello, world!");
 }
 ```
 
+---
+
 Sum of two numbers with type hints.
 
 ```bash
 llm-code write a function that takes a list of numbers and returns the sum of the numbers in python. Add type hints.
 ```
 
 ```python
 from typing import List
 
 def sum_numbers(numbers: List[int]) -> int:
     return sum(numbers)
 ```
 
+---
+
 Lets assume that we stuck the output of the previous call in `out.py`. We can now say:
 
 ```bash
 llm-code -i out.py add appropriate docstrings
 ```
 
 ```python
 from typing import List
 
 def sum_numbers(numbers: List[int]) -> int:
     """Return the sum of the given list of numbers."""
     return sum(numbers)
 ```
 
+---
+
 Or we could write some unit tests.
 
 ```bash
 llm-code -i out.py write a complete unit test file using pytest.
 ```
 
 ```python
@@ -87,10 +131,11 @@
     assert sum_numbers([1, 2, 3]) == 6
     assert sum_numbers([-1, 0, 1]) == 0
     assert sum_numbers([]) == 0
 ```
 
 ## TODO
 
-- [ ] Add a `--stats` option to output token counts.
 - [ ] Add a simple cache to replay the same query.
+- [ ] Add an `--exec` option to execute the generated code.
+- [ ] Add a `--stats` option to output token counts.
 - [ ] Add logging to a local sqllite db.
```

### Comparing `llm_code-0.2/llm_code/llm_code.py` & `llm_code-0.3/llm_code/llm_code.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import click
 import openai
 from pydantic import BaseSettings
 from rich.console import Console
 from rich.syntax import Syntax
 
+from llm_code import __version__
+
 from .templates import Message, TemplateLibrary
 
 
 class Settings(BaseSettings):
     openai_api_key: str = ""
     model: str = "gpt-3.5-turbo"
     temperature: float = 0.8
@@ -30,27 +32,32 @@
     else:
         return None
 
 
 @click.command()
 @click.option("-i", "--inputs", default=None, help="Glob of input files.")
 @click.option("-ln", "--line-numbers", is_flag=True, help="Show line numbers.")
+@click.option("--version", is_flag=True, help="Show version.")
 @click.argument("instructions", nargs=-1)
-def main(inputs, line_numbers, instructions):
+def main(inputs, line_numbers, instructions, version):
     """Coding assistant using OpenAI's chat models.
 
     Requires OPENAI_API_KEY as an environment variable. Alternately, you can set it in
     ~/.llm_code/env.
     """
+    console = Console()
+
+    if version:
+        console.print(f"[bold green]llm_code[/] version {__version__}")
+        sys.exit(0)
+
     settings = Settings()
     if not settings.openai_api_key:
         raise click.UsageError("OPENAI_API_KEY must be set.")
 
-    console = Console()
-
     instructions = " ".join(instructions)
     if not instructions:
         raise click.UsageError("Please provide some instructions.")
 
     library = load_templates(settings.config_dir) or load_templates(
         Path(__file__).parent.parent
     )
@@ -83,7 +90,9 @@
     else:
         console.print(f"No code found in message: \n\n{message.content}")
         sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
+if __name__ == "__main__":
+    main()
```

### Comparing `llm_code-0.2/llm_code/templates.py` & `llm_code-0.3/llm_code/templates.py`

 * *Files identical despite different names*

### Comparing `llm_code-0.2/prompts/coding/user/input.toml` & `llm_code-0.3/prompts/coding/user/input.toml`

 * *Files identical despite different names*

### Comparing `llm_code-0.2/pyproject.toml` & `llm_code-0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-code"
-version = "0.2"
+version = "0.3"
 description = "An OpenAI LLM based CLI coding assistant."
 authors = ["Rushabh Doshi <radoshi+pypi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "llm_code" }]
 homepage = "https://github.com/radoshi/llm-code"
 repository = "https://github.com/radoshi/llm-code"
@@ -29,14 +29,15 @@
 tomli = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 ruff = "^0.0.269"
 pytest-cov = "^4.0.0"
+mypy = "^1.3.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-watch = "^4.2.0"
 
 [build-system]
```

