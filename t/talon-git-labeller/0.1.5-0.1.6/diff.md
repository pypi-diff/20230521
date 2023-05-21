# Comparing `tmp/talon_git_labeller-0.1.5.tar.gz` & `tmp/talon_git_labeller-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talon_git_labeller-0.1.5.tar", last modified: Mon Mar 20 21:18:38 2023, max compression
+gzip compressed data, was "talon_git_labeller-0.1.6.tar", last modified: Sun May 21 17:19:10 2023, max compression
```

## Comparing `talon_git_labeller-0.1.5.tar` & `talon_git_labeller-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-03-20 21:18:38.874418 talon_git_labeller-0.1.5/
--rw-r--r--   0 mike      (1000) mike      (1000)     1076 2023-01-04 16:55:43.000000 talon_git_labeller-0.1.5/LICENSE.txt
--rw-r--r--   0 mike      (1000) mike      (1000)     2164 2023-03-20 21:18:38.874418 talon_git_labeller-0.1.5/PKG-INFO
--rw-r--r--   0 mike      (1000) mike      (1000)     1726 2023-01-05 16:03:34.000000 talon_git_labeller-0.1.5/README.md
--rw-r--r--   0 mike      (1000) mike      (1000)       38 2023-03-20 21:18:38.874418 talon_git_labeller-0.1.5/setup.cfg
--rw-r--r--   0 mike      (1000) mike      (1000)     1044 2023-01-04 16:56:42.000000 talon_git_labeller-0.1.5/setup.py
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-03-20 21:18:38.874418 talon_git_labeller-0.1.5/talon_git_labeller/
--rw-r--r--   0 mike      (1000) mike      (1000)       22 2023-03-20 21:17:51.000000 talon_git_labeller-0.1.5/talon_git_labeller/__init__.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1233 2023-01-05 16:15:04.000000 talon_git_labeller-0.1.5/talon_git_labeller/cli.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2243 2023-01-05 16:15:04.000000 talon_git_labeller-0.1.5/talon_git_labeller/commands.py
--rw-r--r--   0 mike      (1000) mike      (1000)      173 2023-01-04 16:53:05.000000 talon_git_labeller-0.1.5/talon_git_labeller/const.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2138 2023-03-20 19:40:57.000000 talon_git_labeller-0.1.5/talon_git_labeller/helpers.py
--rw-r--r--   0 mike      (1000) mike      (1000)      390 2023-01-07 13:46:44.000000 talon_git_labeller-0.1.5/talon_git_labeller/write.py
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-03-20 21:18:38.874418 talon_git_labeller-0.1.5/talon_git_labeller.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)     2164 2023-03-20 21:18:38.000000 talon_git_labeller-0.1.5/talon_git_labeller.egg-info/PKG-INFO
--rw-r--r--   0 mike      (1000) mike      (1000)      417 2023-03-20 21:18:38.000000 talon_git_labeller-0.1.5/talon_git_labeller.egg-info/SOURCES.txt
--rw-r--r--   0 mike      (1000) mike      (1000)        1 2023-03-20 21:18:38.000000 talon_git_labeller-0.1.5/talon_git_labeller.egg-info/dependency_links.txt
--rw-r--r--   0 mike      (1000) mike      (1000)      153 2023-03-20 21:18:38.000000 talon_git_labeller-0.1.5/talon_git_labeller.egg-info/entry_points.txt
--rw-r--r--   0 mike      (1000) mike      (1000)       19 2023-03-20 21:18:38.000000 talon_git_labeller-0.1.5/talon_git_labeller.egg-info/top_level.txt
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-05-21 17:19:10.503609 talon_git_labeller-0.1.6/
+-rw-r--r--   0 mike      (1000) mike      (1000)     1076 2023-01-04 16:55:43.000000 talon_git_labeller-0.1.6/LICENSE.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)     2164 2023-05-21 17:19:10.493609 talon_git_labeller-0.1.6/PKG-INFO
+-rw-r--r--   0 mike      (1000) mike      (1000)     1726 2023-01-05 16:03:34.000000 talon_git_labeller-0.1.6/README.md
+-rw-r--r--   0 mike      (1000) mike      (1000)       38 2023-05-21 17:19:10.503609 talon_git_labeller-0.1.6/setup.cfg
+-rw-r--r--   0 mike      (1000) mike      (1000)     1044 2023-01-04 16:56:42.000000 talon_git_labeller-0.1.6/setup.py
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-05-21 17:19:10.493609 talon_git_labeller-0.1.6/talon_git_labeller/
+-rw-r--r--   0 mike      (1000) mike      (1000)       22 2023-05-21 17:16:28.000000 talon_git_labeller-0.1.6/talon_git_labeller/__init__.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1233 2023-01-05 16:15:04.000000 talon_git_labeller-0.1.6/talon_git_labeller/cli.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2370 2023-05-21 17:08:43.000000 talon_git_labeller-0.1.6/talon_git_labeller/commands.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      173 2023-01-04 16:53:05.000000 talon_git_labeller-0.1.6/talon_git_labeller/const.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2138 2023-03-20 19:40:57.000000 talon_git_labeller-0.1.6/talon_git_labeller/helpers.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      390 2023-01-07 13:46:44.000000 talon_git_labeller-0.1.6/talon_git_labeller/write.py
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2023-05-21 17:19:10.493609 talon_git_labeller-0.1.6/talon_git_labeller.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)     2164 2023-05-21 17:19:10.000000 talon_git_labeller-0.1.6/talon_git_labeller.egg-info/PKG-INFO
+-rw-r--r--   0 mike      (1000) mike      (1000)      417 2023-05-21 17:19:10.000000 talon_git_labeller-0.1.6/talon_git_labeller.egg-info/SOURCES.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)        1 2023-05-21 17:19:10.000000 talon_git_labeller-0.1.6/talon_git_labeller.egg-info/dependency_links.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)      153 2023-05-21 17:19:10.000000 talon_git_labeller-0.1.6/talon_git_labeller.egg-info/entry_points.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)       19 2023-05-21 17:19:10.000000 talon_git_labeller-0.1.6/talon_git_labeller.egg-info/top_level.txt
```

### Comparing `talon_git_labeller-0.1.5/LICENSE.txt` & `talon_git_labeller-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `talon_git_labeller-0.1.5/PKG-INFO` & `talon_git_labeller-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talon_git_labeller
-Version: 0.1.5
+Version: 0.1.6
 Summary: Adds items to a talon list when certain git commands are executed, allowing files to be easily selected by voice.
 Home-page: https://github.com/mrob95/talon-git-labeller
 Author: Mike Roberts
 License: MIT
 Project-URL: Issues, https://github.com/mrob95/talon_git_labeller/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `talon_git_labeller-0.1.5/README.md` & `talon_git_labeller-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `talon_git_labeller-0.1.5/setup.py` & `talon_git_labeller-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `talon_git_labeller-0.1.5/talon_git_labeller/cli.py` & `talon_git_labeller-0.1.6/talon_git_labeller/cli.py`

 * *Files identical despite different names*

### Comparing `talon_git_labeller-0.1.5/talon_git_labeller/commands.py` & `talon_git_labeller-0.1.6/talon_git_labeller/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,59 @@
-from typing import List, Dict
+from typing import List, Dict, Tuple
 import sys
 import re
 
 from talon_git_labeller.const import PLATFORM
 from talon_git_labeller.helpers import run_command, map_numbers_to_spoken, sort_out_windows_colours
 
 
 COLOUR_GREEN = "\x1b[32m"
 COLOUR_RED   = "\x1b[31m"
 COLOUR_RESET = "\x1b[0m"
 
-
-def git_status(cmd: List[str]) -> Dict[str, str]:
+def parse_status(out: str) -> Tuple[List[str], Dict[str, str]]:
     COLOUR_MAP = {
         "Changes to be committed:": COLOUR_GREEN,
         "Changes not staged for commit:": COLOUR_RED,
         "Untracked files:": COLOUR_RED,
         "Unmerged paths:": COLOUR_RED,
     }
 
-    out = run_command(["git", *cmd])
-    if PLATFORM == "windows":
-        sort_out_windows_colours()
-
-    file_num = 1
+    lines = []
     file_map = {}
+    file_num = 1
     colour = ""
 
     for line in out.strip().split("\n"):
         if line in COLOUR_MAP:
             colour = COLOUR_MAP[line]
 
-        contains_file = re.match(r"^\s+[^(\s]", line)
-        if contains_file:
-            # first group is e.g. 'modified:' or 'deleted:'
-            file_name_match = re.match(r"^\s+([a-z\s]+:\s+)?(.+?)( \(.+?\))?$", line)
-            if file_name_match:
-                file_name = file_name_match.group(2)
-                spoken = map_numbers_to_spoken(file_num)
-                file_map[spoken] = file_name
-                print(f"  {file_num: >2}.   {colour}{line.strip()}{COLOUR_RESET}")
-                file_num += 1
-            else:
-                # Shouldn't ever hit this, means the regexes are missing something
-                print(line)
+        # first group is e.g. 'modified:' or 'deleted:'
+        file_name_match = re.match(r"^\t([a-z\s]+:\s+)?(.+?)( \(.+?\))?$", line)
+        if file_name_match:
+            file_name = file_name_match.group(2)
+            if file_name_match.group(1) and file_name_match.group(1).strip() == "renamed:":
+                _, _, file_name = file_name.rpartition(" -> ")
+            spoken = map_numbers_to_spoken(file_num)
+            file_map[spoken] = file_name
+            lines.append(f"  {file_num: >2}.   {colour}{line.strip()}{COLOUR_RESET}")
+            file_num += 1
         else:
-            print(line)
+            lines.append(line)
+
+    return lines, file_map
+
+
+def git_status(cmd: List[str]) -> Dict[str, str]:
+    out = run_command(["git", *cmd])
+    if PLATFORM == "windows":
+        sort_out_windows_colours()
 
+    lines, file_map = parse_status(out)
+    sys.stdout.write("\n".join(lines) + "\n")
     sys.stdout.flush()
     return file_map
 
 
 def git_branch() -> Dict[str, str]:
     out = run_command(["git", "branch"])
     if PLATFORM == "windows":
```

### Comparing `talon_git_labeller-0.1.5/talon_git_labeller/helpers.py` & `talon_git_labeller-0.1.6/talon_git_labeller/helpers.py`

 * *Files identical despite different names*

### Comparing `talon_git_labeller-0.1.5/talon_git_labeller.egg-info/PKG-INFO` & `talon_git_labeller-0.1.6/talon_git_labeller.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talon-git-labeller
-Version: 0.1.5
+Version: 0.1.6
 Summary: Adds items to a talon list when certain git commands are executed, allowing files to be easily selected by voice.
 Home-page: https://github.com/mrob95/talon-git-labeller
 Author: Mike Roberts
 License: MIT
 Project-URL: Issues, https://github.com/mrob95/talon_git_labeller/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

