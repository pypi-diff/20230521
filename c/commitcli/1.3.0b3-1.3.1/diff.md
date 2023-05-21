# Comparing `tmp/commitcli-1.3.0b3.tar.gz` & `tmp/commitcli-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitcli-1.3.0b3.tar", last modified: Tue Dec  6 16:13:48 2022, max compression
+gzip compressed data, was "commitcli-1.3.1.tar", last modified: Sun May 21 08:14:31 2023, max compression
```

## Comparing `commitcli-1.3.0b3.tar` & `commitcli-1.3.1.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2022-12-06 16:13:48.078939 commitcli-1.3.0b3/
--rw-r--r--   0 gallem    (1000) gallem    (1000)     3698 2022-12-06 16:13:48.078939 commitcli-1.3.0b3/PKG-INFO
-drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2022-12-06 16:13:48.070938 commitcli-1.3.0b3/commitcli/
--rw-r--r--   0 gallem    (1000) gallem    (1000)       48 2022-12-06 16:01:39.000000 commitcli-1.3.0b3/commitcli/__init__.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)      173 2022-10-01 21:48:20.000000 commitcli-1.3.0b3/commitcli/__main__.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)     8317 2022-11-26 04:42:51.000000 commitcli-1.3.0b3/commitcli/commit_message.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)     2822 2022-12-06 16:05:57.000000 commitcli-1.3.0b3/commitcli/commitcli.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)     6690 2022-12-06 08:22:45.000000 commitcli-1.3.0b3/commitcli/common.py
-drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2022-12-06 16:13:48.074939 commitcli-1.3.0b3/commitcli.egg-info/
--rw-r--r--   0 gallem    (1000) gallem    (1000)     3698 2022-12-06 16:13:47.000000 commitcli-1.3.0b3/commitcli.egg-info/PKG-INFO
--rw-r--r--   0 gallem    (1000) gallem    (1000)      619 2022-12-06 16:13:47.000000 commitcli-1.3.0b3/commitcli.egg-info/SOURCES.txt
--rw-r--r--   0 gallem    (1000) gallem    (1000)        1 2022-12-06 16:13:47.000000 commitcli-1.3.0b3/commitcli.egg-info/dependency_links.txt
--rw-r--r--   0 gallem    (1000) gallem    (1000)       55 2022-12-06 16:13:47.000000 commitcli-1.3.0b3/commitcli.egg-info/entry_points.txt
--rw-r--r--   0 gallem    (1000) gallem    (1000)       45 2022-12-06 16:13:47.000000 commitcli-1.3.0b3/commitcli.egg-info/requires.txt
--rw-r--r--   0 gallem    (1000) gallem    (1000)       37 2022-12-06 16:13:47.000000 commitcli-1.3.0b3/commitcli.egg-info/top_level.txt
-drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2022-12-06 16:13:48.074939 commitcli-1.3.0b3/common/
--rw-r--r--   0 gallem    (1000) gallem    (1000)       48 2022-12-06 15:56:15.000000 commitcli-1.3.0b3/common/__init__.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)      840 2022-11-19 08:13:39.000000 commitcli-1.3.0b3/common/environment.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)      245 2022-11-19 08:13:17.000000 commitcli-1.3.0b3/common/logger.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)       68 2022-12-06 15:57:20.000000 commitcli-1.3.0b3/common/versions.py
-drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2022-12-06 16:13:48.078939 commitcli-1.3.0b3/configmanager/
--rwxr-xr-x   0 gallem    (1000) gallem    (1000)       20 2022-11-06 06:44:56.000000 commitcli-1.3.0b3/configmanager/__init__.py
--rwxr-xr-x   0 gallem    (1000) gallem    (1000)     3651 2022-11-06 06:44:56.000000 commitcli-1.3.0b3/configmanager/config.py
--rwxr-xr-x   0 gallem    (1000) gallem    (1000)     5097 2022-12-06 08:22:45.000000 commitcli-1.3.0b3/configmanager/config_manager.py
--rwxr-xr-x   0 gallem    (1000) gallem    (1000)     2933 2022-11-26 04:42:51.000000 commitcli-1.3.0b3/configmanager/format_module_manager.py
--rwxr-xr-x   0 gallem    (1000) gallem    (1000)       36 2022-11-06 06:44:56.000000 commitcli-1.3.0b3/configmanager/test_configmanager.py
--rwxr-xr-x   0 gallem    (1000) gallem    (1000)      336 2022-11-06 06:44:56.000000 commitcli-1.3.0b3/configmanager/test_format_module_manager.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)       38 2022-12-06 16:13:48.078939 commitcli-1.3.0b3/setup.cfg
--rw-r--r--   0 gallem    (1000) gallem    (1000)     1362 2022-12-06 16:04:50.000000 commitcli-1.3.0b3/setup.py
-drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2022-12-06 16:13:48.078939 commitcli-1.3.0b3/tests/
--rw-r--r--   0 gallem    (1000) gallem    (1000)        0 2022-10-01 21:48:20.000000 commitcli-1.3.0b3/tests/__init__.py
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-21 08:14:31.321080 commitcli-1.3.1/
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     3696 2023-05-21 08:14:31.321080 commitcli-1.3.1/PKG-INFO
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-21 08:14:31.313080 commitcli-1.3.1/commitcli/
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       48 2022-12-06 16:01:39.000000 commitcli-1.3.1/commitcli/__init__.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)      173 2022-10-01 21:48:20.000000 commitcli-1.3.1/commitcli/__main__.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     8491 2023-05-21 04:51:51.000000 commitcli-1.3.1/commitcli/commit_message.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     3487 2023-05-21 08:14:27.000000 commitcli-1.3.1/commitcli/commitcli.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     6720 2022-12-14 06:25:36.000000 commitcli-1.3.1/commitcli/common.py
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-21 08:14:31.313080 commitcli-1.3.1/commitcli.egg-info/
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     3696 2023-05-21 08:14:31.000000 commitcli-1.3.1/commitcli.egg-info/PKG-INFO
+-rw-r--r--   0 gallem    (1000) gallem    (1000)      694 2023-05-21 08:14:31.000000 commitcli-1.3.1/commitcli.egg-info/SOURCES.txt
+-rw-r--r--   0 gallem    (1000) gallem    (1000)        1 2023-05-21 08:14:31.000000 commitcli-1.3.1/commitcli.egg-info/dependency_links.txt
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       55 2023-05-21 08:14:31.000000 commitcli-1.3.1/commitcli.egg-info/entry_points.txt
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       45 2023-05-21 08:14:31.000000 commitcli-1.3.1/commitcli.egg-info/requires.txt
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       42 2023-05-21 08:14:31.000000 commitcli-1.3.1/commitcli.egg-info/top_level.txt
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-21 08:14:31.317080 commitcli-1.3.1/common/
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       61 2023-04-12 05:50:39.000000 commitcli-1.3.1/common/__init__.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)      169 2023-05-18 06:58:05.000000 commitcli-1.3.1/common/constants.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)      840 2022-11-19 08:13:39.000000 commitcli-1.3.1/common/environment.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)      245 2022-11-19 08:13:17.000000 commitcli-1.3.1/common/logger.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       98 2023-05-17 06:05:23.000000 commitcli-1.3.1/common/versions.py
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-21 08:14:31.321080 commitcli-1.3.1/configmanager/
+-rwxr-xr-x   0 gallem    (1000) gallem    (1000)       20 2022-11-06 06:44:56.000000 commitcli-1.3.1/configmanager/__init__.py
+-rwxr-xr-x   0 gallem    (1000) gallem    (1000)     4585 2023-05-18 07:04:01.000000 commitcli-1.3.1/configmanager/config.py
+-rwxr-xr-x   0 gallem    (1000) gallem    (1000)     4786 2023-05-21 04:25:40.000000 commitcli-1.3.1/configmanager/config_manager.py
+-rwxr-xr-x   0 gallem    (1000) gallem    (1000)     3236 2023-05-15 08:51:24.000000 commitcli-1.3.1/configmanager/format_module_manager.py
+-rwxr-xr-x   0 gallem    (1000) gallem    (1000)       36 2022-11-06 06:44:56.000000 commitcli-1.3.1/configmanager/test_configmanager.py
+-rwxr-xr-x   0 gallem    (1000) gallem    (1000)      336 2022-11-06 06:44:56.000000 commitcli-1.3.1/configmanager/test_format_module_manager.py
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-21 08:14:31.321080 commitcli-1.3.1/data/
+-rw-r--r--   0 gallem    (1000) gallem    (1000)        0 2023-05-17 06:11:33.000000 commitcli-1.3.1/data/__init__.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     1153 2023-05-18 07:22:02.000000 commitcli-1.3.1/data/db.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     2894 2023-05-18 07:53:23.000000 commitcli-1.3.1/data/modules_repository.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       38 2023-05-21 08:14:31.321080 commitcli-1.3.1/setup.cfg
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     1362 2022-12-06 16:04:50.000000 commitcli-1.3.1/setup.py
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-21 08:14:31.321080 commitcli-1.3.1/tests/
+-rw-r--r--   0 gallem    (1000) gallem    (1000)        0 2022-10-01 21:48:20.000000 commitcli-1.3.1/tests/__init__.py
```

### Comparing `commitcli-1.3.0b3/PKG-INFO` & `commitcli-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitcli
-Version: 1.3.0b3
+Version: 1.3.1
 Summary: commit cli for git with some formats, by default short version of odoo format
 Home-page: https://github.com/marco-gallegos/commit-cli
 Author: Marco A. Gallegos
 Author-email: ma_galeza@hotmail.com
 License: MIT
 Keywords: cli,cc,commit,git,odoo,github,gitlab,bitbucket,conventional commits,semantic commits
 Classifier: Programming Language :: Python :: 3
```

### Comparing `commitcli-1.3.0b3/commitcli/commit_message.py` & `commitcli-1.3.1/commitcli/commit_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 @Author Marco A. Gallegos
 @Date   2020/12/31
 @Update 2020/12/31
 @Description
     This file contains a class to abstract a commit message
 """
 import inquirer
+from configmanager.format_module_manager import ModuleManager
 from commitcli.common import changes_choices_by_format, get_questions, get_preselected_questions, PreselectedQuestion
 
 from configmanager.config_manager import ConfigManager
 from configmanager.format_module_manager import ModuleConfig
 import pendulum
 
 class CommitMessage(object):
@@ -18,21 +19,22 @@
 
     Args:
         object (object): base object from python
     """
     
     def __init__(
         self,
-        format: str = "cc",
+        # format: str = "cc",
+        module_manager: ModuleManager,
         configuration_manager: ConfigManager = ConfigManager(),
-        tag: str = None,
-        module: str = None,
-        header: str = None,
-        body: str = None,
-        footer: str = None,
+        tag: str|None = None,
+        module: str|None = None,
+        header: str|None= None,
+        body: str|None = None,
+        footer: str|None = None,
     ):
         """Constructor of the class
 
         Args:
             format (str, optional): format to use. Defaults to "odoo".
             tag (str, optional): tag for the commit string. Defaults to None.
             module (str, optional): module affected for the commit string. Defaults to None.
@@ -42,14 +44,15 @@
         super()
         self.tag = tag
         self.module = module
         self.header = header
         self.body = body
         self.footer = footer
         self.config:ConfigManager = configuration_manager
+        self.module_manager:ModuleManager = module_manager
         
         self.format = self.config.config.config['format']
 
         self.choices:dict[str,list[tuple]] = changes_choices_by_format
 
 
     def get_commit_string(self)->str:
@@ -110,15 +113,15 @@
     def get_preselected_answers(self) -> list[dict]:
         """check for possible preselected answers according the current format, make quuestions if is needed"""
         preselected_answers:list[dict] = []
         
         preselected_questions:list[PreselectedQuestion] = get_preselected_questions(format=self.format)
         
         for preselected_question in preselected_questions:
-            question = preselected_question.get_value(self.config.moduleManager) 
+            question = preselected_question.get_value(self.module_manager) 
             if question :
                 preselected_answers.append(question)
         
         return preselected_answers
 
 
     def get_answers(self):
@@ -188,15 +191,15 @@
         2 - get modules in file (in this point this module should exist in module manager)
         3 - search for our module inside the result
             3.1 -  if exist update counter and last used
             3.2 - if not exists addit to the list
                 a - limit number of modules to write to 10
         4 - save the modules infomation
         """
-        current_modules:list = self.config.moduleManager.get_modules()
+        current_modules:list = self.module_manager.get_modules()
         new_modules:list[ModuleConfig] = []
         current_date = pendulum.now()
         exist_in_module_list:bool = False
 
         modules_as_csv = ""
         
         if current_modules and len(current_modules) > 0:
```

### Comparing `commitcli-1.3.0b3/commitcli/commitcli.py` & `commitcli-1.3.1/commitcli/commitcli.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,78 +8,105 @@
 """
 import os
 from commitcli.commit_message import CommitMessage
 from configmanager.config_manager import ConfigManager
 import click
 from common.logger import logger
 from common.versions import get_version
+from configmanager.format_module_manager import ModuleManager
+
 
 @click.command()
 @click.option('-nop', '--nooptionals', required=False, is_flag=True, help='Do not ask for optional questions')
 @click.option('-log', '--onlylog', required=False, is_flag=True, help="Avoid confirmimg the message only make a lopg from the final message" )
 @click.option('-v', '--version', required=False, is_flag=True, help="Show the current version" )
 def main(nooptionals: bool, onlylog: bool, version: bool) -> bool:
     """Main funtion on this module is implemented to handle a cli call """
     if version is True:
-        print(f"version: {get_version()}")
+        get_current_version()
     else:
         do_a_commit(nooptionals, onlylog)
     return True
 
+
 def get_current_version():
     print(f"current version : {get_version()}")
     return True
 
 
+def validate_current_repository() -> bool:
+    """Validate that we can make a commit"""
+    are_there_changes:int = os.system("git status --short -uno >> /dev/null")
+    if are_there_changes == 32768:
+        print("there's not a git repository.")
+        return False
+
+    are_there_changes_output:str = os.popen("git diff --name-only --cached").read()  # str with the output
+    if len(are_there_changes_output) == 0:
+        print("looks like theres no changes to commit.")
+        return False
+    return True
+
 
 def do_a_commit(nooptionals: bool, onlylog: bool) -> bool:
     """Function to make commits, its a wrapper for the 'git commit' command
     this uses the '~/.commitclirc' file to store and manage the config.
 
 
     :return: execution status
     :rtype: bool
     """
-    forced_config:dict[str, bool] = {
+    can_commit = validate_current_repository()
+    if (can_commit is not True):
+        return False
+    
+    forced_config:dict[str, bool]|None = {
         "avoid_optionals": not nooptionals,
     }
     logger.log("INFO","forced config runing")
     logger.log("INFO", forced_config)
-    configuration_manager:ConfigManager = ConfigManager(override_config=forced_config, loadModuleManager=True)
-    message_created:bool = create_commit_message(configuration_manager, onlylog)
+
+    configuration_manager:ConfigManager = ConfigManager(override_config=forced_config)
+
+    logger.log("INFO", configuration_manager.config)
+
+    module_manager = ModuleManager(configuration_manager.config)   
+
+    message_created:bool = False 
+    message_created = create_commit_message(configuration_manager, module_manager, onlylog)
+
     return message_created
 
 
+def create_commit_message(configuration_manager: ConfigManager, module_manager:ModuleManager, onlylog: bool) -> bool:
+    commit_msg:CommitMessage = CommitMessage(configuration_manager=configuration_manager, module_manager=module_manager)
 
-def create_commit_message(configuration_manager: ConfigManager, onlylog: bool) -> bool:
-    commit_msg:CommitMessage = CommitMessage(configuration_manager=configuration_manager)
-    are_there_changes:int = os.system("git status --short -uno >> /dev/null")
-    if are_there_changes == 32768:
-        print("there's not a git repository.")
-        return False
+    commit_string:str|None = None
+    
+    try:
+        commit_msg.get_answers()
+    except KeyboardInterrupt:
+        #BUG: this doesn works
+        print("cancelling commit.")
+    except Exception:
+        print("Cancelling commit.")
 
-    are_there_changes_output:str = os.popen("git diff --name-only --cached").read()  # str with the output
-    if len(are_there_changes_output) == 0:
-        print("looks like theres no changes to commit.")
-        return False
+    commit_string = commit_msg.get_commit_string()
 
-    commit_msg.get_answers()
-    commit_string:str|None = commit_msg.get_commit_string()
 
     if commit_string is None:
         return False
 
     print("commiting...")
     # print("=="*30)
-    
 
     commit_command:str = f"git commit -m '{commit_string}'"
 
     if onlylog and onlylog is True:
         print(commit_command)
     else:
         os.system(commit_command)
-    
+
     # update preselected files
     commit_msg.update_preselected_data()
 
     return True
```

### Comparing `commitcli-1.3.0b3/commitcli/common.py` & `commitcli-1.3.1/commitcli/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 
 def get_preselected_module(moduleManager:ModuleManager) -> dict[str, str]:
     """function to get the preselected Module"""
     # get module lis
     module_list:list[ModuleConfig] = moduleManager.get_modules()
     answer:dict = {}
 
-    module_options_list = [
-        ("No, let me write it", "no")
-    ]
+    module_options_list:list = []
     
     if module_list and len(module_list) > 0:
         module_options_temporal_list = [ (x.name, x.name) for x in  module_list ]
 
         module_options_list += module_options_temporal_list
+        module_options_list.insert(1,("No, let me write it", "no"))
         
         # here we expect a array so we want make a questio
         questions = [
             inquirer.List(name="module", message="your module is here?", choices=module_options_list)
         ]
 
         answer = inquirer.prompt(questions)
```

### Comparing `commitcli-1.3.0b3/commitcli.egg-info/PKG-INFO` & `commitcli-1.3.1/commitcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitcli
-Version: 1.3.0b3
+Version: 1.3.1
 Summary: commit cli for git with some formats, by default short version of odoo format
 Home-page: https://github.com/marco-gallegos/commit-cli
 Author: Marco A. Gallegos
 Author-email: ma_galeza@hotmail.com
 License: MIT
 Keywords: cli,cc,commit,git,odoo,github,gitlab,bitbucket,conventional commits,semantic commits
 Classifier: Programming Language :: Python :: 3
```

### Comparing `commitcli-1.3.0b3/commitcli.egg-info/SOURCES.txt` & `commitcli-1.3.1/commitcli.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -7,17 +7,21 @@
 commitcli.egg-info/PKG-INFO
 commitcli.egg-info/SOURCES.txt
 commitcli.egg-info/dependency_links.txt
 commitcli.egg-info/entry_points.txt
 commitcli.egg-info/requires.txt
 commitcli.egg-info/top_level.txt
 common/__init__.py
+common/constants.py
 common/environment.py
 common/logger.py
 common/versions.py
 configmanager/__init__.py
 configmanager/config.py
 configmanager/config_manager.py
 configmanager/format_module_manager.py
 configmanager/test_configmanager.py
 configmanager/test_format_module_manager.py
+data/__init__.py
+data/db.py
+data/modules_repository.py
 tests/__init__.py
```

### Comparing `commitcli-1.3.0b3/common/environment.py` & `commitcli-1.3.1/common/environment.py`

 * *Files identical despite different names*

### Comparing `commitcli-1.3.0b3/configmanager/config.py` & `commitcli-1.3.1/configmanager/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,74 +9,95 @@
 
 
 class Configuration(object):
     config: dict = {
         "format": None,
         "signgpg": None,
         "avoid_optionals": False,
+        "db": "localfile",
+        "db_url": None,
+        "db_port": None,
+        "db_user": None,
+        "db_password": None
     }
     supported_formats: list = [
         "odoo",
         "sgc",
         "cc",
         "free",
     ]
 
-    def __init__(self, config:dict = None, signgpg: bool = False, override_config: dict = None) -> None:
+    def __init__(self, config:dict|None = None, signgpg: bool = False, override_config: dict|None = None) -> None:
         self.config = {
-            'format': "odoo",
+            'format': "cc",
             'signgpg': signgpg,
-            'avoid_optionals': override_config['avoid_optionals'] if override_config else False
+            'avoid_optionals': override_config['avoid_optionals'] if override_config else False,
+            "db": "localfile",
+            "db_url": None,
+            "db_port": None,
+            "db_user": None,
+            "db_password": None
         }
 
         self.supported_formats = [
             "odoo",
             "sgc",
             "cc",
             "free",
         ]
 
         if config:
-            self.config['format'] = config['format'].lower() if 'format' in config else self.config['format'].lower()
+            self.config['format'] = config['format'].lower() if 'format' in config else self.config['format']
             self.config['signgpg'] = config['signgpg'] if 'signgpg' in config else self.config['signgpg']
+            
+            self.config['db'] = config['db'].lower() if 'db' in config else self.config['db']
+            self.config['db_url'] = config['db_url'].lower() if 'db_url' in config else self.config['db_url']
+            self.config['db_port'] = config['db_port'].lower() if 'db_port' in config else self.config['db_port']
+            self.config['db_user'] = config['db_user'].lower() if 'db_user' in config else self.config['db_user']
+            self.config['db_password'] = config['db_password'].lower() if 'db_password' in config else self.config['db_password']
 
             if self.config['signgpg'] and not self.can_sign_gpg():
                 print("Tu configuracion solicita firmar commits pero git no esta configurado")
                 self.config['signgpg']=False
             if not (self.config['format'] in self.supported_formats):
                 print(
                     f"{self.config['format']} is not a supported format, instead we will use "
                     f"{self.supported_formats[0]} as default"
                 )
                 self.config['format'] = self.supported_formats[0]
 
+
         self.can_sign_gpg()
-    
+
+
     def __str__(self)->str:
         """Return a string representation of the object, this function
         is called by the built in print function
 
         :return: string representation
         :rtype: str
         """
         return f"configuracion->  format: {self.config['format']} || sign: {self.config['signgpg']}" \
-               f" || avoid_optionals: {self.config['avoid_optionals']}"
-    
+                f" || avoid_optionals: {self.config['avoid_optionals']} \n db : {self.config['db']}" \
+                f"\ndb url: {self.config['db_url']}"
+
+
     def can_sign_gpg(self)->bool:
         """Return true if the users git repository is configured to sign the commits
 
         :return: indicates that the user can sign the commits
         :rtype: bool
         """
         signkey = os.popen("git config --global user.signingkey").read() 
         if not signkey :
             return False
         else:
             return True
 
+
     def is_a_valid_format(self, format: str) -> bool:
         """Return true if the format parameter string is a supported commit format.
 
         :param format: format to evaluate
         :type format: str
         :return: boolean if the format is supported
         :rtype: bool
```

### Comparing `commitcli-1.3.0b3/configmanager/config_manager.py` & `commitcli-1.3.1/configmanager/config_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,96 +6,92 @@
     The config manager is a class to manage the configuration file by default in ~/.commitclirc
 """
 import distutils.util
 import os
 import pathlib
 import re
 
+from loguru import logger
+
 from configmanager.config import Configuration
-from configmanager.format_module_manager import ModuleManager
 
 
 class ConfigManager(object):
     # data
     # moduleManager:ModuleManager|None
 
     def __init__(
             self, file: str = '.commitclirc',
-            config: Configuration = None,
-            override_config:dict = None,
-            moduleManager:ModuleManager = None,
-            loadModuleManager:bool = False
+            config: Configuration|None = None,
+            override_config:dict|None = None,
         ) -> None:
+
         self._file:str = file
-        self.config:Configuration = config
-        self.regex_clave_valor = r'[\D]+[=]{1}[\w]+'
+        self.config:Configuration|None = config
+        self.regex_clave_valor = r'[\D]+[=]{1}[\w.]+'
         self.pattern_regex_clave_valor = re.compile(self.regex_clave_valor)
 
         # some initial starts
         self.init_config(override_config=override_config)
 
-        # module manager
-        self.moduleManager:ModuleManager = None 
-        if loadModuleManager is True and moduleManager is None:
-            self.moduleManager = ModuleManager()
-        elif loadModuleManager is False and moduleManager is not None:
-            self.moduleManager = moduleManager
-
-
 
     def current_file(self) -> str:
         """this function return the fullpath of the file to store
         the configuration
 
         :return: string with the full path of the file to
         :rtype: str
         """
         global_file = f"{pathlib.Path.home()}/{self._file}"
         project_file = f"{pathlib.Path.cwd()}/{self._file}"
         return project_file if self.exist_file(project_file) else global_file
 
+
     def exist_file(self, file: str) -> bool:
         """this function returns a boolean value on true if the file
         to store the configuration
 
         :return: if the file exists on the filesystem
         :rtype: bool
         """
         exist = os.path.exists(file)
         return True if exist else False
 
-    def stringline_to_key_value(self, string_line: str = "#comentario") -> str:
+
+    def stringline_to_key_value(self, string_line: str = "#comentario") -> tuple[str|None, str|None]:
         """This functions returns the separated values by '=' of a string in 
         format 'some=other'
 
         :param string_line: a string in fomat 'some=other', defaults to "#comentario"
         :type string_line: str, optional
         :return: the values on left and right side of the '=' character
         :rtype: str, str
         """
         key, value = None, None
         match = re.fullmatch(self.pattern_regex_clave_valor, string_line)
         if match and type(string_line) == str and string_line:
             elements = string_line.split("=")
             key= elements[0]
             value= elements[1]
+            logger.info(key, value)
         return key, value
 
-    def load_file(self, file: str) -> dict:
+
+    def load_file(self, file: str) -> dict|None:
         """Method to convert the configuration file into a dictionary
 
         :return: dictionary with al the key value files in thee file
         :rtype: dict
         """
         current_file = file
         if self.exist_file(current_file):
             data_dict = {}
-            file = open(current_file, 'r')
-            file_text = file.readlines()
-            file.close()
+            file_read = open(current_file, 'r')
+            file_text = file_read.readlines()
+            file_read.close()
             for file_line in file_text:
                 file_line = file_line.replace('\n', '')
                 key, value = self.stringline_to_key_value(string_line=file_line)
                 if value == "False" or value == "True" or value == "false" or value == "true":
                     value = bool(distutils.util.strtobool(value.lower()))
                 if key is not None and value is not None:
                     data_dict[key] = value
@@ -110,15 +106,16 @@
         :rtype: bool
         """
         file = open(self.current_file(), 'w')
         file.write(self.config.get_configuration_file_string())
         file.close()
         return True
 
-    def init_config(self, force_reload: bool = False, override_config: dict = None) -> bool:
+
+    def init_config(self, force_reload: bool = False, override_config: dict|None = None) -> bool:
         """Method to initialize the class, triggering the load of the file or load
         creating a defaul config and save it on the file.
 
         :return: boolean representing the previous existence of the config file
         :rtype: bool
         """
         if self.config is None:
@@ -127,15 +124,16 @@
                 data = self.load_file(current_file)
                 self.config = Configuration(config=data, override_config=override_config)
                 return True
             else:
                 self.config = Configuration(override_config=override_config)
                 self.save_file()
                 return False
+        print("config", self.config)
         return False 
 
     def get_config(self, name: str) -> str or bool or None:
         if self.config is not None and self.config.config is not None and self.config.config[name] is not None:
             return self.config.config[name]
         else:
             return None
-        return None
+
```

### Comparing `commitcli-1.3.0b3/configmanager/format_module_manager.py` & `commitcli-1.3.1/configmanager/format_module_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from io import TextIOWrapper
 import pathlib
 import os
+from data.modules_repository import ModulesRepository
 
 
 class ModuleConfig(object):
     name:str
     date:int
     last_used:int
     use_count:int
@@ -24,19 +25,24 @@
 
 
 class ModuleManager(object):
     """
     File format
     """
     _file:str
+    modules:list[ModuleConfig] | None
 
 
-    def __init__(self) -> None:
+    def __init__(self, config) -> None:
         self._file:str|None = ".ignore.commitcli_modules"
-        self.load_modules()
+        
+        modulesRepository = ModulesRepository(config)
+        modulesLoaded = modulesRepository.getAll()
+        self.modules:list[ModuleConfig]|None = modulesLoaded
+
 
 
     def current_file(self) -> str :
         """this function return the fullpath of the file to store
         the configuration
 
         :return: string with the full path of the file to
@@ -52,15 +58,16 @@
 
         :return: if the file exists on the filesystem
         :rtype: bool
         """
         exist = os.path.exists(file)
         return True if exist else False
 
-
+    
+    #NOTE: deprecated use module repository tech instead
     def load_modules(self) -> list[ModuleConfig]:
         current_file:str|None = self.current_file()
 
         if current_file is not None:
             modules_file:TextIOWrapper = open(current_file, "r")
             file_content:list[str] = modules_file.readlines()
             modules_file.close()
@@ -84,15 +91,16 @@
 
 
     def update_modules(self):
         pass
 
 
     def get_modules(self) -> list[ModuleConfig]:
-        return self.load_modules()
+
+        return self.modules
 
 
 
 if __name__ == "__main__":
     moduleManager:ModuleManager = ModuleManager()
     # row:ModuleConfig = ModuleConfig("tmti", 10, 9, 1)
     row:ModuleConfig = ModuleConfig()
```

### Comparing `commitcli-1.3.0b3/setup.py` & `commitcli-1.3.1/setup.py`

 * *Files identical despite different names*

