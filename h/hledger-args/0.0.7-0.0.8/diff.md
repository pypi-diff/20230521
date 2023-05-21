# Comparing `tmp/hledger_args-0.0.7.tar.gz` & `tmp/hledger_args-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hledger_args-0.0.7.tar", last modified: Sun May 14 02:16:08 2023, max compression
+gzip compressed data, was "hledger_args-0.0.8.tar", last modified: Sun May 21 15:20:36 2023, max compression
```

## Comparing `hledger_args-0.0.7.tar` & `hledger_args-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.089698 hledger_args-0.0.7/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9493 2023-05-14 02:16:08.089698 hledger_args-0.0.7/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9153 2023-05-14 02:13:20.000000 hledger_args-0.0.7/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.081698 hledger_args-0.0.7/docs/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9153 2023-05-14 02:13:20.000000 hledger_args-0.0.7/docs/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.083698 hledger_args-0.0.7/hledger_args/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:28.000000 hledger_args-0.0.7/hledger_args/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       84 2023-05-09 19:53:32.000000 hledger_args-0.0.7/hledger_args/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1288 2023-05-11 14:44:16.000000 hledger_args-0.0.7/hledger_args/base_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1968 2023-05-14 02:09:23.000000 hledger_args-0.0.7/hledger_args/batch_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3766 2023-05-14 02:09:23.000000 hledger_args-0.0.7/hledger_args/cli.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4819 2023-05-13 15:05:41.000000 hledger_args-0.0.7/hledger_args/inter_args.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-09 16:55:37.000000 hledger_args-0.0.7/hledger_args/options.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1173 2023-05-14 02:09:10.000000 hledger_args-0.0.7/hledger_args/output_result.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.084698 hledger_args-0.0.7/hledger_args.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9493 2023-05-14 02:16:08.000000 hledger_args-0.0.7/hledger_args.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      748 2023-05-14 02:16:08.000000 hledger_args-0.0.7/hledger_args.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-14 02:16:08.000000 hledger_args-0.0.7/hledger_args.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-14 02:16:08.000000 hledger_args-0.0.7/hledger_args.egg-info/entry_points.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       29 2023-05-14 02:16:08.000000 hledger_args-0.0.7/hledger_args.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-05-14 02:16:08.000000 hledger_args-0.0.7/hledger_args.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1152 2023-05-14 02:14:48.000000 hledger_args-0.0.7/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-14 02:16:08.089698 hledger_args-0.0.7/setup.cfg
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.084698 hledger_args-0.0.7/tests/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:22.000000 hledger_args-0.0.7/tests/__init__.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.081698 hledger_args-0.0.7/venv/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-14 02:16:08.089698 hledger_args-0.0.7/venv/bin/
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2html.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2html4.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2html5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2latex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2man.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2odt.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2s5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2xetex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rst2xml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-05-09 16:48:40.000000 hledger_args-0.0.7/venv/bin/rstpep2html.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.419602 hledger_args-0.0.8/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9956 2023-05-21 15:20:36.418603 hledger_args-0.0.8/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9616 2023-05-21 15:18:13.000000 hledger_args-0.0.8/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.409602 hledger_args-0.0.8/docs/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9616 2023-05-21 15:18:13.000000 hledger_args-0.0.8/docs/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.411602 hledger_args-0.0.8/hledger_args/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:28.000000 hledger_args-0.0.8/hledger_args/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       84 2023-05-09 19:53:32.000000 hledger_args-0.0.8/hledger_args/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1822 2023-05-21 15:20:30.000000 hledger_args-0.0.8/hledger_args/base_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2106 2023-05-16 20:53:33.000000 hledger_args-0.0.8/hledger_args/batch_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3766 2023-05-16 20:59:33.000000 hledger_args-0.0.8/hledger_args/cli.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4924 2023-05-21 15:08:55.000000 hledger_args-0.0.8/hledger_args/inter_args.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3115 2023-05-16 19:54:39.000000 hledger_args-0.0.8/hledger_args/options.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1203 2023-05-16 21:00:47.000000 hledger_args-0.0.8/hledger_args/output_result.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.412602 hledger_args-0.0.8/hledger_args.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9956 2023-05-21 15:20:36.000000 hledger_args-0.0.8/hledger_args.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      748 2023-05-21 15:20:36.000000 hledger_args-0.0.8/hledger_args.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-05-21 15:20:36.000000 hledger_args-0.0.8/hledger_args.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-05-21 15:20:36.000000 hledger_args-0.0.8/hledger_args.egg-info/entry_points.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       35 2023-05-21 15:20:36.000000 hledger_args-0.0.8/hledger_args.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-05-21 15:20:36.000000 hledger_args-0.0.8/hledger_args.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1167 2023-05-21 15:19:01.000000 hledger_args-0.0.8/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-05-21 15:20:36.419602 hledger_args-0.0.8/setup.cfg
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.412602 hledger_args-0.0.8/tests/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-05-09 16:42:22.000000 hledger_args-0.0.8/tests/__init__.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.408602 hledger_args-0.0.8/venv/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-05-21 15:20:36.418603 hledger_args-0.0.8/venv/bin/
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2html.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2html4.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2html5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2latex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2man.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2odt.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2s5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rst2xml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-05-09 16:48:40.000000 hledger_args-0.0.8/venv/bin/rstpep2html.py
```

### Comparing `hledger_args-0.0.7/PKG-INFO` & `hledger_args-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger_args
-Version: 0.0.7
+Version: 0.0.8
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-args
 Project-URL: documentation, https://edkedk99.github.io/hledger-args/
 Project-URL: repository, https://github.com/edkedk99/hledger-args
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -28,20 +28,30 @@
 | {payee}      | fuzzy search existing payee                                                    |
 | {tag}        | fuzzy search existing tags and values                                          |
 | {tag_name}   | search tag name after "_" and fuzzy search existing values for this tag        |
 | {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger** |
 | {type}       | select between accounts type                                                   |
 | {cur}        | fuzzy search existing commodities                                              |
 
+### Non hledger commands
+
+It is possible to run other commands beside the default *hledger*. For that, name the arg as /shell_name/ and /hledger-args/ will execute it according to the conditions:
+
+- It can accept inputs from the terminal stdin.
+- The string /[file]/ will be replaces by the name of the "--file" option.
+- It will not be saved in PDF report
+
+It is useful if you want to add a command that doesn't use hledger but needs the file name being used.
+
 ### PDF output.
 
 There are two ways to output the reports to pdf:
 
 - Option **--pdf-file**: Save the report to the specified file.
-- Option **--pdf-dir**: Save the report to a directory named after the current date under the specified directory. Creates it if doesn't exist. Should be used to keep a history of generated reports
+- Option **--pdf-dir**: Save the report to a directory named after the current date under the specified directory. Creates it if doesn't exist. Should be used to keep a history of generated reports.
 
 
 ## Installation
 
 ### Dependencies
 
 - python 3.8
```

### Comparing `hledger_args-0.0.7/README.md` & `hledger_args-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,20 +18,30 @@
 | {payee}      | fuzzy search existing payee                                                    |
 | {tag}        | fuzzy search existing tags and values                                          |
 | {tag_name}   | search tag name after "_" and fuzzy search existing values for this tag        |
 | {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger** |
 | {type}       | select between accounts type                                                   |
 | {cur}        | fuzzy search existing commodities                                              |
 
+### Non hledger commands
+
+It is possible to run other commands beside the default *hledger*. For that, name the arg as /shell_name/ and /hledger-args/ will execute it according to the conditions:
+
+- It can accept inputs from the terminal stdin.
+- The string /[file]/ will be replaces by the name of the "--file" option.
+- It will not be saved in PDF report
+
+It is useful if you want to add a command that doesn't use hledger but needs the file name being used.
+
 ### PDF output.
 
 There are two ways to output the reports to pdf:
 
 - Option **--pdf-file**: Save the report to the specified file.
-- Option **--pdf-dir**: Save the report to a directory named after the current date under the specified directory. Creates it if doesn't exist. Should be used to keep a history of generated reports
+- Option **--pdf-dir**: Save the report to a directory named after the current date under the specified directory. Creates it if doesn't exist. Should be used to keep a history of generated reports.
 
 
 ## Installation
 
 ### Dependencies
 
 - python 3.8
```

### Comparing `hledger_args-0.0.7/docs/README.md` & `hledger_args-0.0.8/docs/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,20 +18,30 @@
 | {payee}      | fuzzy search existing payee                                                    |
 | {tag}        | fuzzy search existing tags and values                                          |
 | {tag_name}   | search tag name after "_" and fuzzy search existing values for this tag        |
 | {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger** |
 | {type}       | select between accounts type                                                   |
 | {cur}        | fuzzy search existing commodities                                              |
 
+### Non hledger commands
+
+It is possible to run other commands beside the default *hledger*. For that, name the arg as /shell_name/ and /hledger-args/ will execute it according to the conditions:
+
+- It can accept inputs from the terminal stdin.
+- The string /[file]/ will be replaces by the name of the "--file" option.
+- It will not be saved in PDF report
+
+It is useful if you want to add a command that doesn't use hledger but needs the file name being used.
+
 ### PDF output.
 
 There are two ways to output the reports to pdf:
 
 - Option **--pdf-file**: Save the report to the specified file.
-- Option **--pdf-dir**: Save the report to a directory named after the current date under the specified directory. Creates it if doesn't exist. Should be used to keep a history of generated reports
+- Option **--pdf-dir**: Save the report to a directory named after the current date under the specified directory. Creates it if doesn't exist. Should be used to keep a history of generated reports.
 
 
 ## Installation
 
 ### Dependencies
 
 - python 3.8
```

### Comparing `hledger_args-0.0.7/hledger_args/base_args.py` & `hledger_args-0.0.8/hledger_args/base_args.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,22 +15,25 @@
 
 
 class BaseArgs:
     NAMESPACE = "args"
 
     def __init__(self, files: Tuple[str, ...]) -> None:
         self.files = files
-
         vars = HledgerVars(files)
-        self.args = vars.get_namespace_vars(self.NAMESPACE)
-        self.names = set(list(self.args.keys()))
+        namespace_args = vars.get_namespace_vars(self.NAMESPACE)
+        self.args = {
+            key: value.replace("[file]", self.files[0])
+            for key, value in namespace_args.items()
+        }
+        self.names = list(self.args.keys())
         self.has_ask = {
             name for name, var in self.args.items() if re.search(r"\{(.*?)\}", var)
         }
-        self.no_ask = self.names.difference(self.has_ask)
+        self.no_ask = set(self.names).difference(self.has_ask)
 
         self.files_comm = get_files_comm(files)
 
     def run_args(self, options: str, extra: Optional[Tuple[str, ...]] = None):
         options_list = shlex.split(options)
         if extra:
             options_list = [*options_list, *extra]
@@ -38,7 +41,17 @@
         base_comm = ["hledger", *self.files_comm, *options_list]
         proc = subprocess.run(base_comm, capture_output=True, check=True)
         report = proc.stdout.decode("utf8")
 
         base_comm_str = shlex.join(base_comm)
         print(f"stderr: {base_comm_str}\n", file=sys.stderr)
         return report
+
+    def run_shell(self, options: str, extra: Optional[Tuple[str, ...]] = None):
+        options_list = shlex.split(options)
+        if extra:
+            options_list = [*options_list, *extra]
+
+        base_comm_str = shlex.join(options_list)
+        print(f"stderr: {base_comm_str}\n", file=sys.stderr)
+
+        subprocess.run(options_list, capture_output=False, check=True, input=None)
```

### Comparing `hledger_args-0.0.7/hledger_args/batch_args.py` & `hledger_args-0.0.8/hledger_args/batch_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,8 +57,11 @@
             return self.run_all()
         elif self.name not in self.names:
             raise KeyError(f"{self.name} not found.\n\n{self.available_txt}")
         elif self.name in self.has_ask:
             raise KeyError(f"{self.name} is interactive only.\n\n{self.available_txt}")
         else:
             options = self.args[self.name]
-            return self.run_args(options, self.hledger_options)
+            if self.name.startswith("shell_"):
+                return self.run_shell(options, self.hledger_options)
+            else:
+                return self.run_args(options, self.hledger_options)
```

### Comparing `hledger_args-0.0.7/hledger_args/cli.py` & `hledger_args-0.0.8/hledger_args/cli.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/hledger_args/inter_args.py` & `hledger_args-0.0.8/hledger_args/inter_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,14 @@
                 Cash="C",
                 Conversion="V",
             )
             choices = list(types.keys())
             _type = questionary.select("Account Type", choices=choices).ask()
             type_code = types[_type]
             answer = f'"type:{type_code}"'
-
         else:
             answer = questionary.text(placeholder).ask()
 
         return answer
 
     def substitute(self, match: re.Match):
         placeholder: Optional[str] = match.group(1)
@@ -130,8 +129,12 @@
             show_selected=False,
         ).ask()
         return name
 
     def get_report(self):
         options_str = self.args[self.name]
         replaced = self.replace_options(options_str)
-        return self.run_args(replaced)
+
+        if self.name.startswith("shell_"):
+            return self.run_shell(replaced)
+        else:
+            return self.run_args(replaced)
```

### Comparing `hledger_args-0.0.7/hledger_args/options.py` & `hledger_args-0.0.8/hledger_args/options.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/hledger_args/output_result.py` & `hledger_args-0.0.8/hledger_args/output_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,16 +34,17 @@
     elif pdf_dir:
         today = datetime.today().strftime("%Y%m%d")
         file_dir = Path(pdf_dir).joinpath(today)
         file_dir.mkdir(parents=True, exist_ok=True)
         name = args.name or "empty"
         file_dest = file_dir.joinpath(f"{name}.pdf")
     else:
-        print(args.report)
+        print(args.report or "")
         return
 
     header = f"""Report: {args.name}
 _________________
 
 """
 
-    create_pdf(header, args.report, file_dest)
+    if args.report:
+        create_pdf(header, args.report, file_dest)
```

### Comparing `hledger_args-0.0.7/hledger_args.egg-info/PKG-INFO` & `hledger_args-0.0.8/hledger_args.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hledger-args
-Version: 0.0.7
+Version: 0.0.8
 License: MIT License
 Project-URL: homepage, https://github.com/edkedk99/hledger-args
 Project-URL: documentation, https://edkedk99.github.io/hledger-args/
 Project-URL: repository, https://github.com/edkedk99/hledger-args
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
@@ -28,20 +28,30 @@
 | {payee}      | fuzzy search existing payee                                                    |
 | {tag}        | fuzzy search existing tags and values                                          |
 | {tag_name}   | search tag name after "_" and fuzzy search existing values for this tag        |
 | {months}     | prompt initial and end dates both inclusive. **Diferent from default hledger** |
 | {type}       | select between accounts type                                                   |
 | {cur}        | fuzzy search existing commodities                                              |
 
+### Non hledger commands
+
+It is possible to run other commands beside the default *hledger*. For that, name the arg as /shell_name/ and /hledger-args/ will execute it according to the conditions:
+
+- It can accept inputs from the terminal stdin.
+- The string /[file]/ will be replaces by the name of the "--file" option.
+- It will not be saved in PDF report
+
+It is useful if you want to add a command that doesn't use hledger but needs the file name being used.
+
 ### PDF output.
 
 There are two ways to output the reports to pdf:
 
 - Option **--pdf-file**: Save the report to the specified file.
-- Option **--pdf-dir**: Save the report to a directory named after the current date under the specified directory. Creates it if doesn't exist. Should be used to keep a history of generated reports
+- Option **--pdf-dir**: Save the report to a directory named after the current date under the specified directory. Creates it if doesn't exist. Should be used to keep a history of generated reports.
 
 
 ## Installation
 
 ### Dependencies
 
 - python 3.8
```

### Comparing `hledger_args-0.0.7/hledger_args.egg-info/SOURCES.txt` & `hledger_args-0.0.8/hledger_args.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/pyproject.toml` & `hledger_args-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,23 @@
 keyword = ["hledger","PTA", "investments", "accounting"]
 classifiers = [""]
 author = "Eduardo"
 author_email = "edkedk99@hotmail.com"
 
 [project]
 name = "hledger_args"
-version = "0.0.7"
+version = "0.0.8"
 readme= "docs/README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 dependencies = [
 	     "click",
 	     "rich_click",
-	     "questionary"
+	     "questionary",
+	     "fpdf2"
 ]
 
 [project.urls]
 homepage = "https://github.com/edkedk99/hledger-args"
 documentation = "https://edkedk99.github.io/hledger-args/"
 repository = "https://github.com/edkedk99/hledger-args"
 # changelog = ""
```

### Comparing `hledger_args-0.0.7/venv/bin/rst2html.py` & `hledger_args-0.0.8/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/venv/bin/rst2html4.py` & `hledger_args-0.0.8/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/venv/bin/rst2html5.py` & `hledger_args-0.0.8/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/venv/bin/rst2latex.py` & `hledger_args-0.0.8/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/venv/bin/rst2man.py` & `hledger_args-0.0.8/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/venv/bin/rst2odt.py` & `hledger_args-0.0.8/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/venv/bin/rst2odt_prepstyles.py` & `hledger_args-0.0.8/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/venv/bin/rst2pseudoxml.py` & `hledger_args-0.0.8/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/venv/bin/rst2s5.py` & `hledger_args-0.0.8/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/venv/bin/rst2xetex.py` & `hledger_args-0.0.8/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/venv/bin/rst2xml.py` & `hledger_args-0.0.8/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hledger_args-0.0.7/venv/bin/rstpep2html.py` & `hledger_args-0.0.8/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

