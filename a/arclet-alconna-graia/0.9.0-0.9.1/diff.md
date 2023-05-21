# Comparing `tmp/arclet-alconna-graia-0.9.0.tar.gz` & `tmp/arclet-alconna-graia-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-graia-0.9.0.tar", last modified: Sun Nov 20 13:55:12 2022, max compression
+gzip compressed data, was "arclet-alconna-graia-0.9.1.tar", last modified: Tue Nov 22 04:22:57 2022, max compression
```

## Comparing `arclet-alconna-graia-0.9.0.tar` & `arclet-alconna-graia-0.9.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-rw-rw-   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-graia-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     1482 2022-11-20 13:51:28.873093 arclet-alconna-graia-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0     5212 2022-11-20 13:53:36.642607 arclet-alconna-graia-0.9.0/README.md
--rw-rw-rw-   0        0        0      654 2022-10-18 04:51:54.211778 arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/__init__.py
--rw-rw-rw-   0        0        0     2826 2022-11-20 13:15:49.196578 arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/alc.py
--rw-rw-rw-   0        0        0     2260 2022-11-20 13:15:49.189613 arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/analyser.py
--rw-rw-rw-   0        0        0     1507 2022-09-17 01:57:59.015905 arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/create.py
--rw-rw-rw-   0        0        0    10276 2022-11-20 13:15:49.182612 arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/dispatcher.py
--rw-rw-rw-   0        0        0      950 2022-09-11 01:57:46.621827 arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/model.py
--rw-rw-rw-   0        0        0     2825 2022-11-20 13:22:20.522482 arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/saya.py
--rw-rw-rw-   0        0        0    12635 2022-11-20 13:44:10.988867 arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/utils.py
--rw-rw-rw-   0        0        0     5888 2022-11-20 13:55:12.613533 arclet-alconna-graia-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-graia-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     1484 2022-11-22 04:22:02.034955 arclet-alconna-graia-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0     5209 2022-11-22 04:22:02.055898 arclet-alconna-graia-0.9.1/README.md
+-rw-rw-rw-   0        0        0      654 2022-10-18 04:51:54.211778 arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/__init__.py
+-rw-rw-rw-   0        0        0     2826 2022-11-20 13:15:49.196578 arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/alc.py
+-rw-rw-rw-   0        0        0     2260 2022-11-20 13:15:49.189613 arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/analyser.py
+-rw-rw-rw-   0        0        0     1507 2022-09-17 01:57:59.015905 arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/create.py
+-rw-rw-rw-   0        0        0    10276 2022-11-20 13:15:49.182612 arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/dispatcher.py
+-rw-rw-rw-   0        0        0      950 2022-09-11 01:57:46.621827 arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/model.py
+-rw-rw-rw-   0        0        0     2465 2022-11-22 04:22:02.048917 arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/saya.py
+-rw-rw-rw-   0        0        0    12745 2022-11-22 04:22:02.026975 arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/utils.py
+-rw-rw-rw-   0        0        0     5885 2022-11-22 04:22:57.151169 arclet-alconna-graia-0.9.1/PKG-INFO
```

### Comparing `arclet-alconna-graia-0.9.0/LICENSE` & `arclet-alconna-graia-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-graia-0.9.0/pyproject.toml` & `arclet-alconna-graia-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "arclet-alconna-graia"
-version = "0.9.0"
+version = "0.9.1"
 description = "Support Alconna to GraiaProject"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
-    "arclet-alconna<1.4.0, >=1.3.2",
+    "arclet-alconna<1.4.0, >=1.3.2.2",
     "arclet-alconna-tools>=0.2.0",
     "nepattern>=0.3.0",
     "creart-graia>=0.1.5",
     "creart>=0.2.1",
     "graia-amnesia>=0.5.0",
     "graia-ariadne<0.10.0, >=0.7.14",
     "graia-broadcast>=0.18.2",
```

### Comparing `arclet-alconna-graia-0.9.0/README.md` & `arclet-alconna-graia-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 ```
 ### 使用 Saya Util
 
 in module.py:
 
 ```python
-from graia.ariadne.util.saya import listen
+from graiax.shortcut.saya import listen
 from arclet.alconna.graia import Match, alcommand, from_command, startswith, endswith
 from arclet.alconna import Alconna, Args, Arpamar
 
 ...
 
 
 @alcommand(Alconna("!jrrp", Args["sth", str, 1123]), private=False)
```

### Comparing `arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/__init__.py` & `arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/__init__.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/alc.py` & `arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/alc.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/analyser.py` & `arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/analyser.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/create.py` & `arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/create.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/dispatcher.py` & `arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/dispatcher.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/model.py` & `arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/model.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/saya.py` & `arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/saya.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-import inspect
 from dataclasses import dataclass
-from pathlib import Path
 from typing import Any, Union
 
-from arclet.alconna import config
 from arclet.alconna.core import Alconna
 from arclet.alconna.manager import CommandManager
 from arclet.alconna.tools import AlconnaString
 from graia.broadcast import Broadcast
 from graia.saya.behaviour import Behaviour
 from graia.saya.cube import Cube
 from graia.saya.schema import BaseSchema
@@ -27,21 +24,14 @@
 
     def record(self, func: Any):
         command: Alconna
         if isinstance(self.command, AlconnaDispatcher):
             command = self.command.command
         else:
             command = self.command
-        try:
-            file = inspect.getsourcefile(func)
-        except TypeError:
-            return
-        if command.namespace == config.default_namespace.name and file:
-            path = Path(file)
-            command.reset_namespace(f"{path.parts[-2]}.{path.stem}")
         if shortcuts := getattr(func, "__alc_shortcuts__", {}):
             for k, v in shortcuts.items():
                 command.shortcut(k, v)
 
 
 class AlconnaBehaviour(Behaviour):
     """命令行为"""
```

### Comparing `arclet-alconna-graia-0.9.0/src/arclet/alconna/graia/utils.py` & `arclet-alconna-graia-0.9.1/src/arclet/alconna/graia/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,16 @@
     private: bool = True,
     send_error: bool = False,
     post: bool = False,
 ) -> SchemaWrapper:
     """
     saya-util 形式的注册一个消息事件监听器并携带 AlconnaDispatcher
 
+    请将其放置在装饰器的顶层
+
     Args:
         alconna: 使用的 Alconna 命令
         guild: 命令是否群聊可用
         private: 命令是否私聊可用
         send_error: 是否发送错误信息
         post: 是否以事件发送输出信息
     """
@@ -225,14 +227,17 @@
 
 
 _seminal = type("_seminal", (object,), {})
 
 
 @buffer_modifier
 def assign(path: str, value: Any = _seminal, or_not: bool = False) -> BufferModifier:
+    """
+    match_path 与 match_value 的合并形式
+    """
     def wrapper(buffer: Dict[str, Any]):
         if value == _seminal:
             if or_not:
                 buffer.setdefault("decorators", []).append(match_path("$main"))
             buffer.setdefault("decorators", []).append(match_path(path))
         else:
             buffer.setdefault("decorators", []).append(match_value(path, value, or_not))
```

### Comparing `arclet-alconna-graia-0.9.0/PKG-INFO` & `arclet-alconna-graia-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-graia
-Version: 0.9.0
+Version: 0.9.1
 Summary: Support Alconna to GraiaProject
 License: AGPL-3.0
 Keywords: alconna,graia,dispatcher,arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -86,15 +86,15 @@
 
 ```
 ### 使用 Saya Util
 
 in module.py:
 
 ```python
-from graia.ariadne.util.saya import listen
+from graiax.shortcut.saya import listen
 from arclet.alconna.graia import Match, alcommand, from_command, startswith, endswith
 from arclet.alconna import Alconna, Args, Arpamar
 
 ...
 
 
 @alcommand(Alconna("!jrrp", Args["sth", str, 1123]), private=False)
```

