# Comparing `tmp/shell_gpt-0.9.0.tar.gz` & `tmp/shell_gpt-0.9.1.tar.gz`

## Comparing `shell_gpt-0.9.0.tar` & `shell_gpt-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/LICENSE
--rw-r--r--   0        0        0    18734 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/README.md
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/__main__.py
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/app.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/cache.py
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/client.py
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/config.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/make_prompt.py
--rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/role.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/handlers/__init__.py
--rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/handlers/chat_handler.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/handlers/default_handler.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/handlers/handler.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/sgpt/handlers/repl_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0    15148 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/tests/test_integration.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/tests/test_unit.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/LICENSE
--rw-r--r--   0        0        0    18734 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/README.md
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    20762 2020-02-02 00:00:00.000000 shell_gpt-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/LICENSE
+-rw-r--r--   0        0        0    19376 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/README.md
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/__main__.py
+-rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/app.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/cache.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/client.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/config.py
+-rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/role.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/handlers/__init__.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/handlers/chat_handler.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/handlers/default_handler.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/handlers/handler.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/sgpt/handlers/repl_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0    17250 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/tests/test_integration.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/tests/test_unit.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/LICENSE
+-rw-r--r--   0        0        0    19376 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/README.md
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    21403 2020-02-02 00:00:00.000000 shell_gpt-0.9.1/PKG-INFO
```

### Comparing `shell_gpt-0.9.0/LICENSE` & `shell_gpt-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.0/README.md` & `shell_gpt-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ShellGPT
 A command-line productivity tool powered by OpenAI's GPT models. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort. ShellGPT is cross-platform compatible and supports all major operating systems, including Linux, macOS, and Windows with all major shells, such as PowerShell, CMD, Bash, Zsh, Fish, and many others.
 
 https://user-images.githubusercontent.com/16740832/231569156-a3a9f9d4-18b1-4fff-a6e1-6807651aa894.mp4
 
 ## Installation
 ```shell
-pip install shell-gpt==0.9.0
+pip install shell-gpt==0.9.1
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -41,47 +41,60 @@
 This powerful feature simplifies the process of managing and understanding data from different sources, making it easier for you to focus on what really matters: improving your projects and applications.
 
 ### Shell commands
 Have you ever found yourself forgetting common shell commands, such as `chmod`, and needing to look up the syntax online? With `--shell` or shortcut `-s` option, you can quickly find and execute the commands you need right in the terminal.
 ```shell
 sgpt --shell "make all files in current directory read only"
 # -> chmod 444 *
-# -> Execute shell command? [y/N]: y
-# ...
+# -> [E]xecute, [D]escribe, [A]bort: e
+...
 ```
 Shell GPT is aware of OS and `$SHELL` you are using, it will provide shell command for specific system you have. For instance, if you ask `sgpt` to update your system, it will return a command based on your OS. Here's an example using macOS:
 ```shell
 sgpt -s "update my system"
 # -> sudo softwareupdate -i -a
+# -> [E]xecute, [D]escribe, [A]bort: e
+...
 ```
 The same prompt, when used on Ubuntu, will generate a different suggestion:
 ```shell
 sgpt -s "update my system"
 # -> sudo apt update && sudo apt upgrade -y
+# -> [E]xecute, [D]escribe, [A]bort: e
+...
+```
+We can ask GPT to describe suggested shell command, it will provide a short description of what the command does:
+```shell
+sgpt -s "show all txt files in current folder"
+# -> ls *.txt
+# -> [E]xecute, [D]escribe, [A]bort: d
+# -> List all files with .txt extension in current directory
+# -> [E]xecute, [D]escribe, [A]bort: e
+...
 ```
 Let's try some docker containers:
 ```shell
 sgpt -s "start nginx using docker, forward 443 and 80 port, mount current folder with index.html"
 # -> docker run -d -p 443:443 -p 80:80 -v $(pwd):/usr/share/nginx/html nginx
-# -> Execute shell command? [y/N]: y
-# ...
+# -> [E]xecute, [D]escribe, [A]bort: e
+...
 ```
 We can still use pipes to pass input to `sgpt` and get shell commands as output:
 ```shell
 cat data.json | sgpt -s "curl localhost with provided json"
 # -> curl -X POST -H "Content-Type: application/json" -d '{"a": 1, "b": 2, "c": 3}' http://localhost
 ````
 We can apply additional shell magic in our prompt, in this example passing file names to ffmpeg:
 ```shell
 ls
 # -> 1.mp4 2.mp4 3.mp4
 sgpt -s "using ffmpeg combine multiple videos into one without audio. Video file names: $(ls -m)"
 # -> ffmpeg -i 1.mp4 -i 2.mp4 -i 3.mp4 -filter_complex "[0:v] [1:v] [2:v] concat=n=3:v=1 [v]" -map "[v]" out.mp4
-# -> Execute shell command? [y/N]: y
-# ...
+# -> [E]xecute, [D]escribe, [A]bort: e
+...
 ```
 ### Generating code
 With `--code` parameters we can query only code as output, for example:
 ```shell
 sgpt --code "Solve classic fizz buzz problem using Python"
 ```
 ```python
@@ -137,15 +150,15 @@
 sgpt --chat number "please remember my favorite number: 4"
 # -> I will remember that your favorite number is 4.
 sgpt --chat number "what would be my favorite number + 4?"
 # -> Your favorite number is 4, so if we add 4 to it, the result would be 8.
 ```
 You can also use chat sessions to iteratively improve GPT suggestions by providing additional clues.
 ```shell
-sgpt --chat python_requst --code "make an example request to localhost using Python"
+sgpt --chat python_request --code "make an example request to localhost using Python"
 ```
 ```python
 import requests
 
 response = requests.get('http://localhost')
 print(response.text)
 ```
@@ -196,15 +209,15 @@
 Entering shell REPL mode, type [e] to execute commands or press Ctrl+C to exit.
 >>> What is in current folder?
 ls
 >>> Show file sizes
 ls -lh
 >>> Sort them by file sizes
 ls -lhS
->>> e (enter just e to execute commands)
+>>> e (enter just e to execute commands, or d to describe them)
 ...
 ```
 Example of using REPL mode to generate code:
 ```text
 sgpt --repl temp --code
 Entering REPL mode, press Ctrl+C to exit.
 >>> Using Python request localhost:80
@@ -282,34 +295,37 @@
 REQUEST_TIMEOUT=60
 # Default OpenAI model to use.
 DEFAULT_MODEL=gpt-3.5-turbo
 # Default color for OpenAI completions.
 DEFAULT_COLOR=magenta
 # Force use system role messages (not recommended).
 SYSTEM_ROLES=false
+# When in --shell mode, default to "Y" for no input.
+DEFAULT_EXECUTE_SHELL_CMD=false
 ```
 Possible options for `DEFAULT_COLOR`: black, red, green, yellow, blue, magenta, cyan, white, bright_black, bright_red, bright_green, bright_yellow, bright_blue, bright_magenta, bright_cyan, bright_white.
 
 Switch `SYSTEM_ROLES` to force use [system roles](https://help.openai.com/en/articles/7042661-chatgpt-api-transition-guide) messages, this is not recommended, since it doesn't perform well with current GPT models.
 
 ### Full list of arguments
 ```text
 ╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────╮
 │   prompt      [PROMPT]  The prompt to generate completions for.                                             │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --model            [gpt-3.5-turbo|gpt-4|gpt-4-32k]  OpenAI GPT model to use. [default: gpt-3.5-turbo]       │
-│ --temperature      FLOAT RANGE [0.0<=x<=1.0]        Randomness of generated output. [default: 0.1]          │
+│ --temperature      FLOAT RANGE [0.0<=x<=2.0]        Randomness of generated output. [default: 0.1]          │
 │ --top-probability  FLOAT RANGE [0.1<=x<=1.0]        Limits highest probable tokens (words). [default: 1.0]  │
 │ --editor                                            Open $EDITOR to provide a prompt. [default: no-editor]  │
 │ --cache                                             Cache completion results. [default: cache]              │
 │ --help                                              Show this message and exit.                             │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Assistance Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --shell  -s                 Generate and execute shell commands.                                            │
+│ --describe-shell  -d        Describe a shell command.                                                       │
 │ --code       --no-code      Generate only code. [default: no-code]                                          │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Chat Options ──────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --chat        TEXT  Follow conversation with id, use "temp" for quick session. [default: None]              │
 │ --repl        TEXT  Start a REPL (Read–eval–print loop) session. [default: None]                            │
 │ --show-chat   TEXT  Show all messages from provided chat id. [default: None]                                │
 │ --list-chats        List all existing chat ids. [default: no-list-chats]                                    │
```

### Comparing `shell_gpt-0.9.0/pyproject.toml` & `shell_gpt-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "requests >= 2.28.2, < 3.0.0",
     "typer >= 0.7.0, < 1.0.0",
     "click >= 7.1.1, < 9.0.0",
-    "rich >= 10.11.0, < 13.0.0",
+    "rich >= 13.1.0, < 14.0.0",
     "distro >= 1.8.0, < 2.0.0",
     'pyreadline3 >= 3.4.1, < 4.0.0; sys_platform == "win32"',
 ]
 
 [project.scripts]
 sgpt = "sgpt:cli"
```

### Comparing `shell_gpt-0.9.0/sgpt/app.py` & `shell_gpt-0.9.1/sgpt/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 """
 # To allow users to use arrow keys in the REPL.
 import readline  # noqa: F401
 import sys
 
 import typer
 from click import BadArgumentUsage, MissingParameter
+from click.types import Choice
 
-from sgpt.client import OpenAIClient
 from sgpt.config import cfg
 from sgpt.handlers.chat_handler import ChatHandler
 from sgpt.handlers.default_handler import DefaultHandler
 from sgpt.handlers.repl_handler import ReplHandler
 from sgpt.role import DefaultRoles, SystemRole
 from sgpt.utils import ModelOptions, get_edited_prompt, run_command
 
@@ -30,15 +30,15 @@
     model: ModelOptions = typer.Option(
         ModelOptions(cfg.get("DEFAULT_MODEL")).value,
         help="OpenAI GPT model to use.",
     ),
     temperature: float = typer.Option(
         0.1,
         min=0.0,
-        max=1.0,
+        max=2.0,
         help="Randomness of generated output.",
     ),
     top_probability: float = typer.Option(
         1.0,
         min=0.1,
         max=1.0,
         help="Limits highest probable tokens (words).",
@@ -46,14 +46,21 @@
     shell: bool = typer.Option(
         False,
         "--shell",
         "-s",
         help="Generate and execute shell commands.",
         rich_help_panel="Assistance Options",
     ),
+    describe_shell: bool = typer.Option(
+        False,
+        "--describe-shell",
+        "-d",
+        help="Describe a shell command.",
+        rich_help_panel="Assistance Options",
+    ),
     code: bool = typer.Option(
         False,
         help="Generate only code.",
         rich_help_panel="Assistance Options",
     ),
     editor: bool = typer.Option(
         False,
@@ -113,63 +120,84 @@
 
     if stdin_passed and not repl:
         prompt = f"{sys.stdin.read()}\n\n{prompt or ''}"
 
     if not prompt and not editor and not repl:
         raise MissingParameter(param_hint="PROMPT", param_type="string")
 
-    if shell and code:
-        raise BadArgumentUsage("--shell and --code options cannot be used together.")
+    if sum((shell, describe_shell, code)) > 1:
+        raise BadArgumentUsage(
+            "Only one of --shell, --describe-shell, and --code options can be used at a time."
+        )
 
     if chat and repl:
         raise BadArgumentUsage("--chat and --repl options cannot be used together.")
 
     if editor and stdin_passed:
         raise BadArgumentUsage("--editor option cannot be used with stdin input.")
 
     if editor:
         prompt = get_edited_prompt()
 
-    api_host = cfg.get("OPENAI_API_HOST")
-    api_key = cfg.get("OPENAI_API_KEY")
-    client = OpenAIClient(api_host, api_key)
-
-    role_class = DefaultRoles.get(shell, code) if not role else SystemRole.get(role)
+    role_class = (
+        DefaultRoles.check_get(shell, describe_shell, code)
+        if not role
+        else SystemRole.get(role)
+    )
 
     if repl:
         # Will be in infinite loop here until user exits with Ctrl+C.
-        ReplHandler(client, repl, role_class).handle(
+        ReplHandler(repl, role_class).handle(
             prompt,
             model=model.value,
             temperature=temperature,
             top_probability=top_probability,
             chat_id=repl,
             caching=cache,
         )
 
     if chat:
-        full_completion = ChatHandler(client, chat, role_class).handle(
+        full_completion = ChatHandler(chat, role_class).handle(
             prompt,
             model=model.value,
             temperature=temperature,
             top_probability=top_probability,
             chat_id=chat,
             caching=cache,
         )
     else:
-        full_completion = DefaultHandler(client, role_class).handle(
+        full_completion = DefaultHandler(role_class).handle(
             prompt,
             model=model.value,
             temperature=temperature,
             top_probability=top_probability,
             caching=cache,
         )
 
-    if shell and not stdin_passed and typer.confirm("Execute shell command?"):
-        run_command(full_completion)
+    while shell and not stdin_passed:
+        option = typer.prompt(
+            text="[E]xecute, [D]escribe, [A]bort",
+            type=Choice(("e", "d", "a", "y"), case_sensitive=False),
+            default="e" if cfg.get("DEFAULT_EXECUTE_SHELL_CMD") == "true" else "a",
+            show_choices=False,
+            show_default=False,
+        )
+        if option in ("e", "y"):
+            # "y" option is for keeping compatibility with old version.
+            run_command(full_completion)
+        elif option == "d":
+            DefaultHandler(DefaultRoles.DESCRIBE_SHELL.get_role()).handle(
+                full_completion,
+                model=model.value,
+                temperature=temperature,
+                top_probability=top_probability,
+                caching=cache,
+            )
+            continue
+        break
 
 
 def entry_point() -> None:
     # Python package entry point defined in setup.py
     typer.run(main)
```

### Comparing `shell_gpt-0.9.0/sgpt/cache.py` & `shell_gpt-0.9.1/sgpt/cache.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.0/sgpt/client.py` & `shell_gpt-0.9.1/sgpt/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 REQUEST_TIMEOUT = int(cfg.get("REQUEST_TIMEOUT"))
 
 
 class OpenAIClient:
     cache = Cache(CACHE_LENGTH, CACHE_PATH)
 
     def __init__(self, api_host: str, api_key: str) -> None:
-        self.api_key = api_key
+        self.__api_key = api_key
         self.api_host = api_host
 
     @cache
     def _request(
         self,
         messages: List[Dict[str, str]],
         model: str = "gpt-3.5-turbo",
@@ -29,32 +29,36 @@
     ) -> Generator[str, None, None]:
         """
         Make request to OpenAI API, read more:
         https://platform.openai.com/docs/api-reference/chat
 
         :param messages: List of messages {"role": user or assistant, "content": message_string}
         :param model: String gpt-3.5-turbo or gpt-3.5-turbo-0301
-        :param temperature: Float in 0.0 - 1.0 range.
+        :param temperature: Float in 0.0 - 2.0 range.
         :param top_probability: Float in 0.0 - 1.0 range.
         :return: Response body JSON.
         """
-        headers = {
-            "Content-Type": "application/json",
-            "Authorization": f"Bearer {self.api_key}",
-        }
         data = {
             "messages": messages,
             "model": model,
             "temperature": temperature,
             "top_p": top_probability,
             "stream": True,
         }
         endpoint = f"{self.api_host}/v1/chat/completions"
         response = requests.post(
-            endpoint, headers=headers, json=data, timeout=REQUEST_TIMEOUT, stream=True
+            endpoint,
+            # Hide API key from Rich traceback.
+            headers={
+                "Content-Type": "application/json",
+                "Authorization": f"Bearer {self.__api_key}",
+            },
+            json=data,
+            timeout=REQUEST_TIMEOUT,
+            stream=True,
         )
         response.raise_for_status()
         # TODO: Optimise.
         # https://github.com/openai/openai-python/blob/237448dc072a2c062698da3f9f512fae38300c1c/openai/api_requestor.py#L98
         for line in response.iter_lines():
             data = line.lstrip(b"data: ").decode("utf-8")
             if data == "[DONE]":  # type: ignore
```

### Comparing `shell_gpt-0.9.0/sgpt/config.py` & `shell_gpt-0.9.1/sgpt/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "CACHE_LENGTH": int(os.getenv("CHAT_CACHE_LENGTH", "100")),
     "REQUEST_TIMEOUT": int(os.getenv("REQUEST_TIMEOUT", "60")),
     "DEFAULT_MODEL": os.getenv("DEFAULT_MODEL", ModelOptions.GPT3.value),
     "OPENAI_API_HOST": os.getenv("OPENAI_API_HOST", "https://api.openai.com"),
     "DEFAULT_COLOR": os.getenv("DEFAULT_COLOR", "magenta"),
     "ROLE_STORAGE_PATH": os.getenv("ROLE_STORAGE_PATH", str(ROLE_STORAGE_PATH)),
     "SYSTEM_ROLES": os.getenv("SYSTEM_ROLES", "false"),
+    "DEFAULT_EXECUTE_SHELL_CMD": os.getenv("DEFAULT_EXECUTE_SHELL_CMD", "false"),
     # New features might add their own config variables here.
 }
 
 
 class Config(dict):  # type: ignore
     def __init__(self, config_path: Path, **defaults: Any):
         self.config_path = config_path
@@ -45,16 +46,16 @@
                     self[key] = value
             if has_new_config:
                 self._write()
         else:
             config_path.parent.mkdir(parents=True, exist_ok=True)
             # Don't write API key to config file if it is in the environment.
             if not defaults.get("OPENAI_API_KEY") and not os.getenv("OPENAI_API_KEY"):
-                api_key = getpass(prompt="Please enter your OpenAI API key: ")
-                defaults["OPENAI_API_KEY"] = api_key
+                __api_key = getpass(prompt="Please enter your OpenAI API key: ")
+                defaults["OPENAI_API_KEY"] = __api_key
             super().__init__(**defaults)
             self._write()
 
     @property
     def _exists(self) -> bool:
         return self.config_path.exists()
 
@@ -64,16 +65,17 @@
             for key, value in self.items():
                 string_config += f"{key}={value}\n"
             file.write(string_config)
 
     def _read(self) -> None:
         with open(self.config_path, "r", encoding="utf-8") as file:
             for line in file:
-                key, value = line.strip().split("=")
-                self[key] = value
+                if not line.startswith("#"):
+                    key, value = line.strip().split("=")
+                    self[key] = value
 
     def get(self, key: str) -> str:  # type: ignore
         # Prioritize environment variables over config file.
         value = os.getenv(key) or super().get(key)
         if not value:
             raise UsageError(f"Missing config key: {key}")
         return value
```

### Comparing `shell_gpt-0.9.0/sgpt/role.py` & `shell_gpt-0.9.1/sgpt/role.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 from .utils import option_callback
 
 SHELL_ROLE = """Provide only {shell} commands for {os} without any description.
 If there is a lack of details, provide most logical solution.
 Ensure the output is a valid shell command.
 If multiple steps required try to combine them together."""
 
+DESCRIBE_SHELL_ROLE = """Provide a terse, single sentence description
+of the given shell command. Provide only plain text without Markdown formatting.
+Do not show any warnings or information regarding your capabilities.
+If you need to store any data, assume it will be stored in the chat."""
+
 CODE_ROLE = """Provide only code as output without any description.
 IMPORTANT: Provide only plain text without Markdown formatting.
 IMPORTANT: Do not include markdown formatting such as ```.
 If there is a lack of details, provide most logical solution.
 You are not allowed to ask for more details.
 Ignore any potential risk of errors or confusion."""
 
@@ -63,14 +68,15 @@
     @classmethod
     def create_defaults(cls) -> None:
         cls.storage.parent.mkdir(parents=True, exist_ok=True)
         variables = {"shell": cls.shell_name(), "os": cls.os_name()}
         for default_role in (
             SystemRole("default", DEFAULT_ROLE, "Answer", variables),
             SystemRole("shell", SHELL_ROLE, "Command", variables),
+            SystemRole("describe_shell", DESCRIBE_SHELL_ROLE, "Description", variables),
             SystemRole("code", CODE_ROLE, "Code"),
         ):
             if not default_role.exists:
                 default_role.save()
 
     @classmethod
     def os_name(cls) -> str:
@@ -108,15 +114,16 @@
         return cls(**json.loads(file_path.read_text()))
 
     @classmethod
     @option_callback
     def create(cls, name: str) -> None:
         role = typer.prompt("Enter role description")
         expecting = typer.prompt(
-            "Enter expecting result, e.g. answer, code, shell command, etc."
+            "Enter expecting result, e.g. answer, code, \
+            shell command, command description, etc."
         )
         role = cls(name, role, expecting)
         role.save()
 
     @classmethod
     @option_callback
     def list(cls, _value: str) -> None:
@@ -179,19 +186,25 @@
             return False
         return True if f"Role name: {self.name}" in initial_message else False
 
 
 class DefaultRoles(Enum):
     DEFAULT = "default"
     SHELL = "shell"
+    DESCRIBE_SHELL = "describe_shell"
     CODE = "code"
 
     @classmethod
-    def get(cls, shell: bool, code: bool) -> SystemRole:
+    def check_get(cls, shell: bool, describe_shell: bool, code: bool) -> SystemRole:
         if shell:
             return SystemRole.get(DefaultRoles.SHELL.value)
+        if describe_shell:
+            return SystemRole.get(DefaultRoles.DESCRIBE_SHELL.value)
         if code:
             return SystemRole.get(DefaultRoles.CODE.value)
         return SystemRole.get(DefaultRoles.DEFAULT.value)
 
+    def get_role(self) -> SystemRole:
+        return SystemRole.get(self.value)
+
 
 SystemRole.create_defaults()
```

### Comparing `shell_gpt-0.9.0/sgpt/utils.py` & `shell_gpt-0.9.1/sgpt/utils.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.0/sgpt/handlers/chat_handler.py` & `shell_gpt-0.9.1/sgpt/handlers/chat_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 from pathlib import Path
 from typing import Any, Callable, Dict, Generator, List, Optional
 
 import typer
 from click import BadArgumentUsage
 
-from ..client import OpenAIClient
 from ..config import cfg
 from ..role import SystemRole
 from .handler import Handler
 
 CHAT_CACHE_LENGTH = int(cfg.get("CHAT_CACHE_LENGTH"))
 CHAT_CACHE_PATH = Path(cfg.get("CHAT_CACHE_PATH"))
 
@@ -87,23 +86,17 @@
         # Sort files by last modification time in ascending order.
         return sorted(files, key=lambda f: f.stat().st_mtime)
 
 
 class ChatHandler(Handler):
     chat_session = ChatSession(CHAT_CACHE_LENGTH, CHAT_CACHE_PATH)
 
-    def __init__(
-        self,
-        client: OpenAIClient,
-        chat_id: str,
-        role: SystemRole,
-    ) -> None:
-        super().__init__(client, role)
+    def __init__(self, chat_id: str, role: SystemRole) -> None:
+        super().__init__(role)
         self.chat_id = chat_id
-        self.client = client
         self.role = role
 
         if chat_id == "temp":
             # If the chat id is "temp", we don't want to save the chat session.
             self.chat_session.invalidate(chat_id)
 
         self.validate()
```

### Comparing `shell_gpt-0.9.0/sgpt/handlers/default_handler.py` & `shell_gpt-0.9.1/sgpt/handlers/default_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 from pathlib import Path
 from typing import Dict, List
 
-from ..client import OpenAIClient
 from ..config import cfg
 from ..role import SystemRole
 from .handler import Handler
 
 CHAT_CACHE_LENGTH = int(cfg.get("CHAT_CACHE_LENGTH"))
 CHAT_CACHE_PATH = Path(cfg.get("CHAT_CACHE_PATH"))
 
 
 class DefaultHandler(Handler):
-    def __init__(
-        self,
-        client: OpenAIClient,
-        role: SystemRole,
-    ) -> None:
-        super().__init__(client, role)
-        self.client = client
+    def __init__(self, role: SystemRole) -> None:
+        super().__init__(role)
         self.role = role
 
     def make_prompt(self, prompt: str) -> str:
         prompt = prompt.strip()
         return self.role.make_prompt(prompt, initial=True)
 
     def make_messages(self, prompt: str) -> List[Dict[str, str]]:
```

### Comparing `shell_gpt-0.9.0/sgpt/handlers/handler.py` & `shell_gpt-0.9.1/sgpt/handlers/handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 from ..client import OpenAIClient
 from ..config import cfg
 from ..role import SystemRole
 
 
 class Handler:
-    def __init__(self, client: OpenAIClient, role: SystemRole) -> None:
-        self.client = client
+    def __init__(self, role: SystemRole) -> None:
+        self.client = OpenAIClient(
+            cfg.get("OPENAI_API_HOST"), cfg.get("OPENAI_API_KEY")
+        )
         self.role = role
         self.color = cfg.get("DEFAULT_COLOR")
 
     def make_prompt(self, prompt: str) -> str:
         raise NotImplementedError
 
     def make_messages(self, prompt: str) -> List[Dict[str, str]]:
```

### Comparing `shell_gpt-0.9.0/sgpt/handlers/repl_handler.py` & `shell_gpt-0.9.1/sgpt/handlers/repl_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 from typing import Any
 
 import typer
 from rich import print as rich_print
 from rich.rule import Rule
 
-from ..client import OpenAIClient
 from ..role import DefaultRoles, SystemRole
 from ..utils import run_command
 from .chat_handler import ChatHandler
+from .default_handler import DefaultHandler
 
 
 class ReplHandler(ChatHandler):
-    def __init__(self, client: OpenAIClient, chat_id: str, role: SystemRole) -> None:
-        super().__init__(client, chat_id, role)
+    def __init__(self, chat_id: str, role: SystemRole) -> None:
+        super().__init__(chat_id, role)
 
     def handle(self, prompt: str, **kwargs: Any) -> None:  # type: ignore
         if self.initiated:
             rich_print(Rule(title="Chat History", style="bold magenta"))
             self.show_messages(self.chat_id)
             rich_print(Rule(style="bold magenta"))
 
         info_message = (
             "Entering REPL mode, press Ctrl+C to exit."
             if not self.role.name == DefaultRoles.SHELL.value
-            else "Entering shell REPL mode, type [e] to execute commands or press Ctrl+C to exit."
+            else (
+                "Entering shell REPL mode, type [e] to execute commands "
+                "or [d] to describe the commands, press Ctrl+C to exit."
+            )
         )
         typer.secho(info_message, fg="yellow")
 
-        if not prompt:
-            prompt = typer.prompt(">>>", prompt_suffix=" ")
-        else:
-            typer.echo(f">>> {prompt}")
-
+        full_completion = ""
         while True:
-            full_completion = super().handle(prompt, **kwargs)
+            # Infinite loop until user exits with Ctrl+C.
             prompt = typer.prompt(">>>", prompt_suffix=" ")
             if prompt == "exit()":
                 # This is also useful during tests.
                 raise typer.Exit()
-            if self.role.name == DefaultRoles.SHELL.value:
-                if prompt == "e":
-                    typer.echo()
-                    run_command(full_completion)
-                    typer.echo()
-                    rich_print(Rule(style="bold magenta"))
-                    prompt = typer.prompt(">>> ", prompt_suffix=" ")
+            if self.role.name == DefaultRoles.SHELL.value and prompt == "e":
+                typer.echo()
+                run_command(full_completion)
+                typer.echo()
+                rich_print(Rule(style="bold magenta"))
+            elif self.role.name == DefaultRoles.SHELL.value and prompt == "d":
+                DefaultHandler(DefaultRoles.DESCRIBE_SHELL.get_role()).handle(
+                    full_completion,
+                    model=kwargs.get("model"),
+                    temperature=kwargs.get("temperature"),
+                    top_probability=kwargs.get("top_probability"),
+                    caching=kwargs.get("caching"),
+                )
+            else:
+                full_completion = super().handle(prompt, **kwargs)
```

### Comparing `shell_gpt-0.9.0/tests/test_integration.py` & `shell_gpt-0.9.1/tests/test_integration.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from unittest.mock import ANY, patch
 from uuid import uuid4
 
 import typer
 from typer.testing import CliRunner
 
 from sgpt.app import main
-from sgpt.client import OpenAIClient
 from sgpt.config import cfg
 from sgpt.handlers.handler import Handler
 from sgpt.role import SystemRole
 
 runner = CliRunner()
 app = typer.Typer()
 app.command()(main)
@@ -59,14 +58,23 @@
             "prompt": "make a commit using git",
             "--shell": True,
         }
         result = runner.invoke(app, self.get_arguments(**dict_arguments))
         assert result.exit_code == 0
         assert "git commit" in result.stdout
 
+    def test_describe_shell(self):
+        dict_arguments = {
+            "prompt": "ls",
+            "--describe-shell": True,
+        }
+        result = runner.invoke(app, self.get_arguments(**dict_arguments))
+        assert result.exit_code == 0
+        assert "List " in result.stdout
+
     def test_code(self):
         """
         This test will request from OpenAI API a python code to make CLI app,
         which will be written to a temp file, and then it will be executed
         in shell with two positional int arguments. As the output we are
         expecting the result of multiplying them.
         """
@@ -141,14 +149,31 @@
         dict_arguments["--code"] = True
         del dict_arguments["--shell"]
         assert "--shell" not in dict_arguments
         result = runner.invoke(app, self.get_arguments(**dict_arguments))
         # If we are using --code, we cannot use --shell.
         assert result.exit_code == 2
 
+    def test_chat_describe_shell(self):
+        chat_name = uuid4()
+        dict_arguments = {
+            "prompt": "git add",
+            "--chat": f"test_{chat_name}",
+            "--describe-shell": True,
+        }
+        result = runner.invoke(app, self.get_arguments(**dict_arguments))
+        assert result.exit_code == 0
+        assert "Add file contents to the index." in result.stdout
+        dict_arguments["prompt"] = "'-A'"
+        # Prevent Too Many Requests.
+        sleep(1)
+        result = runner.invoke(app, self.get_arguments(**dict_arguments))
+        assert result.exit_code == 0
+        assert "all" in result.stdout
+
     def test_chat_code(self):
         chat_name = uuid4()
         dict_arguments = {
             "prompt": "Using python request localhost:80.",
             "--chat": f"test_{chat_name}",
             "--code": True,
         }
@@ -190,15 +215,15 @@
         dict_arguments = {
             "prompt": "What is the capital of the Czech Republic?",
             "--code": True,
             "--shell": True,
         }
         result = runner.invoke(app, self.get_arguments(**dict_arguments))
         assert result.exit_code == 2
-        assert "--shell and --code options cannot be used together" in result.stdout
+        assert "Only one of --shell, --describe-shell, and --code" in result.stdout
 
     def test_repl_default(
         self,
     ):
         dict_arguments = {
             "prompt": "",
             "--repl": "temp",
@@ -239,14 +264,35 @@
         # TODO: Implement same check in chat mode tests.
         assert chat_messages[0]["content"].startswith("###")
         assert chat_messages[0]["content"].endswith("\n###\nCommand:")
         assert chat_messages[1]["content"] == "ls"
         assert chat_messages[2]["content"].endswith("\nCommand:")
         assert chat_messages[3]["content"] == "ls | sort"
 
+    def test_repl_describe_command(self):
+        # Temp chat session from previous test should be overwritten.
+        dict_arguments = {
+            "prompt": "",
+            "--repl": "temp",
+            "--describe-shell": True,
+        }
+        inputs = ["pacman -S", "-yu", "exit()"]
+        result = runner.invoke(
+            app, self.get_arguments(**dict_arguments), input="\n".join(inputs)
+        )
+        assert result.exit_code == 0
+        assert "Install" in result.stdout
+        assert "Update" in result.stdout
+
+        chat_storage = cfg.get("CHAT_CACHE_PATH")
+        tmp_chat = Path(chat_storage) / "temp"
+        chat_messages = json.loads(tmp_chat.read_text())
+        assert chat_messages[0]["content"].startswith("###")
+        assert chat_messages[0]["content"].endswith("\n###\nDescription:")
+
     def test_repl_code(self):
         dict_arguments = {
             "prompt": "",
             "--repl": f"test_{uuid4()}",
             "--code": True,
         }
         inputs = (
@@ -317,18 +363,18 @@
             caching=False,
         )
         assert result.exit_code == 0
 
     def test_color_output(self):
         color = cfg.get("DEFAULT_COLOR")
         role = SystemRole.get("default")
-        handler = Handler(OpenAIClient("test", "test"), role=role)
+        handler = Handler(role=role)
         assert handler.color == color
         os.environ["DEFAULT_COLOR"] = "red"
-        handler = Handler(OpenAIClient("test", "test"), role=role)
+        handler = Handler(role=role)
         assert handler.color == "red"
 
     def test_simple_stdin(self):
         result = runner.invoke(app, input="What is the capital of Germany?\n")
         assert "Berlin" in result.stdout
 
     def test_shell_stdin_with_prompt(self):
@@ -388,7 +434,18 @@
         result = runner.invoke(app, self.get_arguments(**dict_arguments), input=stdin)
         assert result.exit_code == 0
         generated_json = json.loads(result.stdout)
         assert "username" in generated_json
         assert "password" in generated_json
         assert "email" in generated_json
         test_role.unlink(missing_ok=True)
+
+    def test_shell_command_run_description(self):
+        dict_arguments = {
+            "prompt": "say hello",
+            "--shell": True,
+        }
+        result = runner.invoke(app, self.get_arguments(**dict_arguments), input="d\n")
+        assert result.exit_code == 0
+        # Cant really test it since stdin in disable for --shell flag.
+        # for word in ("prints", "hello", "console"):
+        #     assert word in result.stdout
```

### Comparing `shell_gpt-0.9.0/tests/test_unit.py` & `shell_gpt-0.9.1/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.0/PKG-INFO` & `shell_gpt-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell_gpt
-Version: 0.9.0
+Version: 0.9.1
 Summary: A command-line productivity tool powered by OpenAI GPT models, will help you accomplish your tasks faster and more efficiently.
 Project-URL: homepage, https://github.com/ther1d/shell_gpt
 Project-URL: repository, https://github.com/ther1d/shell_gpt
 Project-URL: documentation, https://github.com/TheR1D/shell_gpt/blob/main/README.md
 Author-email: Farkhod Sadykov <farkhod@sadykov.dev>
 License-Expression: MIT
 License-File: LICENSE
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Python: >=3.6
 Requires-Dist: click<9.0.0,>=7.1.1
 Requires-Dist: distro<2.0.0,>=1.8.0
 Requires-Dist: pyreadline3<4.0.0,>=3.4.1; sys_platform == 'win32'
 Requires-Dist: requests<3.0.0,>=2.28.2
-Requires-Dist: rich<13.0.0,>=10.11.0
+Requires-Dist: rich<14.0.0,>=13.1.0
 Requires-Dist: typer<1.0.0,>=0.7.0
 Provides-Extra: dev
 Requires-Dist: pre-commit<4.0.0,>=3.1.1; extra == 'dev'
 Requires-Dist: ruff==0.0.256; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: black==23.1.0; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.12.0; extra == 'test'
@@ -45,15 +45,15 @@
 # ShellGPT
 A command-line productivity tool powered by OpenAI's GPT models. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort. ShellGPT is cross-platform compatible and supports all major operating systems, including Linux, macOS, and Windows with all major shells, such as PowerShell, CMD, Bash, Zsh, Fish, and many others.
 
 https://user-images.githubusercontent.com/16740832/231569156-a3a9f9d4-18b1-4fff-a6e1-6807651aa894.mp4
 
 ## Installation
 ```shell
-pip install shell-gpt==0.9.0
+pip install shell-gpt==0.9.1
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
@@ -85,47 +85,60 @@
 This powerful feature simplifies the process of managing and understanding data from different sources, making it easier for you to focus on what really matters: improving your projects and applications.
 
 ### Shell commands
 Have you ever found yourself forgetting common shell commands, such as `chmod`, and needing to look up the syntax online? With `--shell` or shortcut `-s` option, you can quickly find and execute the commands you need right in the terminal.
 ```shell
 sgpt --shell "make all files in current directory read only"
 # -> chmod 444 *
-# -> Execute shell command? [y/N]: y
-# ...
+# -> [E]xecute, [D]escribe, [A]bort: e
+...
 ```
 Shell GPT is aware of OS and `$SHELL` you are using, it will provide shell command for specific system you have. For instance, if you ask `sgpt` to update your system, it will return a command based on your OS. Here's an example using macOS:
 ```shell
 sgpt -s "update my system"
 # -> sudo softwareupdate -i -a
+# -> [E]xecute, [D]escribe, [A]bort: e
+...
 ```
 The same prompt, when used on Ubuntu, will generate a different suggestion:
 ```shell
 sgpt -s "update my system"
 # -> sudo apt update && sudo apt upgrade -y
+# -> [E]xecute, [D]escribe, [A]bort: e
+...
+```
+We can ask GPT to describe suggested shell command, it will provide a short description of what the command does:
+```shell
+sgpt -s "show all txt files in current folder"
+# -> ls *.txt
+# -> [E]xecute, [D]escribe, [A]bort: d
+# -> List all files with .txt extension in current directory
+# -> [E]xecute, [D]escribe, [A]bort: e
+...
 ```
 Let's try some docker containers:
 ```shell
 sgpt -s "start nginx using docker, forward 443 and 80 port, mount current folder with index.html"
 # -> docker run -d -p 443:443 -p 80:80 -v $(pwd):/usr/share/nginx/html nginx
-# -> Execute shell command? [y/N]: y
-# ...
+# -> [E]xecute, [D]escribe, [A]bort: e
+...
 ```
 We can still use pipes to pass input to `sgpt` and get shell commands as output:
 ```shell
 cat data.json | sgpt -s "curl localhost with provided json"
 # -> curl -X POST -H "Content-Type: application/json" -d '{"a": 1, "b": 2, "c": 3}' http://localhost
 ````
 We can apply additional shell magic in our prompt, in this example passing file names to ffmpeg:
 ```shell
 ls
 # -> 1.mp4 2.mp4 3.mp4
 sgpt -s "using ffmpeg combine multiple videos into one without audio. Video file names: $(ls -m)"
 # -> ffmpeg -i 1.mp4 -i 2.mp4 -i 3.mp4 -filter_complex "[0:v] [1:v] [2:v] concat=n=3:v=1 [v]" -map "[v]" out.mp4
-# -> Execute shell command? [y/N]: y
-# ...
+# -> [E]xecute, [D]escribe, [A]bort: e
+...
 ```
 ### Generating code
 With `--code` parameters we can query only code as output, for example:
 ```shell
 sgpt --code "Solve classic fizz buzz problem using Python"
 ```
 ```python
@@ -181,15 +194,15 @@
 sgpt --chat number "please remember my favorite number: 4"
 # -> I will remember that your favorite number is 4.
 sgpt --chat number "what would be my favorite number + 4?"
 # -> Your favorite number is 4, so if we add 4 to it, the result would be 8.
 ```
 You can also use chat sessions to iteratively improve GPT suggestions by providing additional clues.
 ```shell
-sgpt --chat python_requst --code "make an example request to localhost using Python"
+sgpt --chat python_request --code "make an example request to localhost using Python"
 ```
 ```python
 import requests
 
 response = requests.get('http://localhost')
 print(response.text)
 ```
@@ -240,15 +253,15 @@
 Entering shell REPL mode, type [e] to execute commands or press Ctrl+C to exit.
 >>> What is in current folder?
 ls
 >>> Show file sizes
 ls -lh
 >>> Sort them by file sizes
 ls -lhS
->>> e (enter just e to execute commands)
+>>> e (enter just e to execute commands, or d to describe them)
 ...
 ```
 Example of using REPL mode to generate code:
 ```text
 sgpt --repl temp --code
 Entering REPL mode, press Ctrl+C to exit.
 >>> Using Python request localhost:80
@@ -326,34 +339,37 @@
 REQUEST_TIMEOUT=60
 # Default OpenAI model to use.
 DEFAULT_MODEL=gpt-3.5-turbo
 # Default color for OpenAI completions.
 DEFAULT_COLOR=magenta
 # Force use system role messages (not recommended).
 SYSTEM_ROLES=false
+# When in --shell mode, default to "Y" for no input.
+DEFAULT_EXECUTE_SHELL_CMD=false
 ```
 Possible options for `DEFAULT_COLOR`: black, red, green, yellow, blue, magenta, cyan, white, bright_black, bright_red, bright_green, bright_yellow, bright_blue, bright_magenta, bright_cyan, bright_white.
 
 Switch `SYSTEM_ROLES` to force use [system roles](https://help.openai.com/en/articles/7042661-chatgpt-api-transition-guide) messages, this is not recommended, since it doesn't perform well with current GPT models.
 
 ### Full list of arguments
 ```text
 ╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────╮
 │   prompt      [PROMPT]  The prompt to generate completions for.                                             │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --model            [gpt-3.5-turbo|gpt-4|gpt-4-32k]  OpenAI GPT model to use. [default: gpt-3.5-turbo]       │
-│ --temperature      FLOAT RANGE [0.0<=x<=1.0]        Randomness of generated output. [default: 0.1]          │
+│ --temperature      FLOAT RANGE [0.0<=x<=2.0]        Randomness of generated output. [default: 0.1]          │
 │ --top-probability  FLOAT RANGE [0.1<=x<=1.0]        Limits highest probable tokens (words). [default: 1.0]  │
 │ --editor                                            Open $EDITOR to provide a prompt. [default: no-editor]  │
 │ --cache                                             Cache completion results. [default: cache]              │
 │ --help                                              Show this message and exit.                             │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Assistance Options ────────────────────────────────────────────────────────────────────────────────────────╮
 │ --shell  -s                 Generate and execute shell commands.                                            │
+│ --describe-shell  -d        Describe a shell command.                                                       │
 │ --code       --no-code      Generate only code. [default: no-code]                                          │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Chat Options ──────────────────────────────────────────────────────────────────────────────────────────────╮
 │ --chat        TEXT  Follow conversation with id, use "temp" for quick session. [default: None]              │
 │ --repl        TEXT  Start a REPL (Read–eval–print loop) session. [default: None]                            │
 │ --show-chat   TEXT  Show all messages from provided chat id. [default: None]                                │
 │ --list-chats        List all existing chat ids. [default: no-list-chats]                                    │
```

