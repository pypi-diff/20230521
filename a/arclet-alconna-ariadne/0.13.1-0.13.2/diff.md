# Comparing `tmp/arclet-alconna-ariadne-0.13.1.tar.gz` & `tmp/arclet-alconna-ariadne-0.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-ariadne-0.13.1.tar", last modified: Thu May 11 16:05:58 2023, max compression
+gzip compressed data, was "arclet-alconna-ariadne-0.13.2.tar", last modified: Sun May 21 05:34:46 2023, max compression
```

## Comparing `arclet-alconna-ariadne-0.13.1.tar` & `arclet-alconna-ariadne-0.13.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ariadne-0.13.1/LICENSE
--rw-r--r--   0        0        0     6165 2023-05-11 15:54:03.114473 arclet-alconna-ariadne-0.13.1/pyproject.toml
--rw-r--r--   0        0        0     7402 2023-05-10 15:25:33.392236 arclet-alconna-ariadne-0.13.1/README.md
--rw-r--r--   0        0        0       81 2023-02-20 07:51:15.898481 arclet-alconna-ariadne-0.13.1/src/arclet/alconna/ariadne/__init__.py
--rw-r--r--   0        0        0     6016 2023-05-11 05:46:08.898508 arclet-alconna-ariadne-0.13.1/src/arclet/alconna/ariadne/adapter.py
--rw-r--r--   0        0        0     1262 2023-05-08 17:03:36.101915 arclet-alconna-ariadne-0.13.1/src/arclet/alconna/ariadne/typings.py
--rw-r--r--   0        0        0     7835 1970-01-01 00:00:00.000000 arclet-alconna-ariadne-0.13.1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ariadne-0.13.2/LICENSE
+-rw-r--r--   0        0        0     6165 2023-05-21 03:55:55.277777 arclet-alconna-ariadne-0.13.2/pyproject.toml
+-rw-r--r--   0        0        0     7402 2023-05-10 15:25:33.392236 arclet-alconna-ariadne-0.13.2/README.md
+-rw-r--r--   0        0        0       81 2023-02-20 07:51:15.898481 arclet-alconna-ariadne-0.13.2/src/arclet/alconna/ariadne/__init__.py
+-rw-r--r--   0        0        0     6031 2023-05-21 05:29:50.785370 arclet-alconna-ariadne-0.13.2/src/arclet/alconna/ariadne/adapter.py
+-rw-r--r--   0        0        0     1262 2023-05-08 17:03:36.101915 arclet-alconna-ariadne-0.13.2/src/arclet/alconna/ariadne/typings.py
+-rw-r--r--   0        0        0     7835 1970-01-01 00:00:00.000000 arclet-alconna-ariadne-0.13.2/PKG-INFO
```

### Comparing `arclet-alconna-ariadne-0.13.1/LICENSE` & `arclet-alconna-ariadne-0.13.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ariadne-0.13.1/pyproject.toml` & `arclet-alconna-ariadne-0.13.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-alconna-ariadne"
-version = "0.13.1"
+version = "0.13.2"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "graia-ariadne<1.0.0,>=0.7.14",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
@@ -55,29 +55,29 @@
 [tool.mina.packages.core]
 includes = [
     "src/arclet/alconna/graia",
 ]
 
 [tool.mina.packages.core.project]
 name = "arclet-alconna-graia"
-version = "0.13.1"
+version = "0.13.2"
 description = "Support Alconna to GraiaProject"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "alconna",
     "graia",
     "arclet",
     "ariadne",
 ]
 dependencies = [
-    "arclet-alconna<2.0.0, >=1.7.0",
+    "arclet-alconna<2.0.0, >=1.7.6",
     "arclet-alconna-tools<0.7.0, >=0.6.0",
     "tarina>=0.3.3",
     "nepattern<0.6.0, >=0.5.6",
     "creart-graia>=0.1.5",
     "creart>=0.2.1",
     "graia-amnesia>=0.5.0",
     "graia-broadcast>=0.18.2",
@@ -107,20 +107,20 @@
 alconna_behavior = "arclet.alconna.graia.create:AlconnaBehaviorCreator"
 
 [tool.mina.packages.ariadne]
 includes = [
     "src/arclet/alconna/ariadne",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.13.1, >= 0.13.1",
+    "arclet-alconna-graia<0.13.2, >= 0.13.2",
 ]
 
 [tool.mina.packages.ariadne.project]
 name = "arclet-alconna-ariadne"
-version = "0.13.1"
+version = "0.13.2"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "graia-ariadne<1.0.0, >=0.7.14",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
@@ -148,20 +148,20 @@
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.mina.packages.avilla]
 includes = [
     "src/arclet/alconna/avilla",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.13.1, >= 0.13.1",
+    "arclet-alconna-graia<0.13.2, >= 0.13.2",
 ]
 
 [tool.mina.packages.avilla.project]
 name = "arclet-alconna-avilla"
-version = "0.13.1"
+version = "0.13.2"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "avilla-core>=1.0.0a5",
 ]
 description = "Support Alconna to GraiaProject/Avilla"
@@ -190,20 +190,20 @@
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.mina.packages.ichika]
 includes = [
     "src/arclet/alconna/ichika",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.13.1, >= 0.13.1",
+    "arclet-alconna-graia<0.13.2, >= 0.13.2",
 ]
 
 [tool.mina.packages.ichika.project]
 name = "arclet-alconna-ichika"
-version = "0.13.1"
+version = "0.13.2"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "ichika>=0.0.5",
 ]
 description = "Support Alconna to BlueGlassBlock/Ichika"
```

### Comparing `arclet-alconna-ariadne-0.13.1/README.md` & `arclet-alconna-ariadne-0.13.2/README.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ariadne-0.13.1/src/arclet/alconna/ariadne/adapter.py` & `arclet-alconna-ariadne-0.13.2/src/arclet/alconna/ariadne/adapter.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Callable
 
 from arclet.alconna.exceptions import SpecialOptionTriggered
 from graia.ariadne.app import Ariadne
 from graia.ariadne.dispatcher import ContextDispatcher
 from graia.ariadne.event.message import FriendMessage, GroupMessage, MessageEvent
 from graia.ariadne.message.chain import MessageChain
-from graia.ariadne.message.element import At, Plain
+from graia.ariadne.message.element import At, Plain, Source, File, Quote
 from graia.ariadne.model import Friend
 from graia.ariadne.util import resolve_dispatchers_mixin
 from graia.ariadne.util.interrupt import AnnotationWaiter
 from graia.broadcast.builtin.decorators import Depend
 from graia.broadcast.exceptions import ExecutionStop
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
 from graia.broadcast.interrupt import Waiter
@@ -26,50 +26,54 @@
 from ..graia.dispatcher import AlconnaDispatcher, AlconnaOutputMessage
 from ..graia.utils import listen
 
 AlconnaDispatcher.default_send_handler = lambda _, x: MessageChain([Plain(x)])
 
 
 class AlconnaAriadneAdapter(AlconnaGraiaAdapter[MessageEvent]):
-    def completion_waiter(self, interface: DispatcherInterface[MessageEvent], priority: int = 15) -> Waiter:
-        return AnnotationWaiter(MessageChain, [interface.event.__class__], block_propagation=True, priority=priority)
+    def completion_waiter(self, source: MessageEvent, priority: int = 15) -> Waiter:
+        return AnnotationWaiter(MessageChain, [source.__class__], block_propagation=True, priority=priority)
 
     async def lookup_source(self, interface: DispatcherInterface[MessageEvent]) -> MessageChain:
         return await interface.lookup_param("__message_chain__", MessageChain, MessageChain("Unknown"))
 
+    def source_id(self, source: MessageEvent | None = None) -> str:
+        return str(source.source.id) if source else "_"
+
     async def send(
         self,
         dispatcher: AlconnaDispatcher,
         result: Arparma[MessageChain],
         output_text: str | None = None,
         source: MessageEvent | None = None,
-        exclude: bool = True,
+    ) -> None:
+        app: Ariadne = Ariadne.current()
+        help_message: MessageChain = await run_always_await(
+            dispatcher.converter,
+            str(result.error_info) if isinstance(result.error_info, SpecialOptionTriggered) else "help",
+            output_text,
+        )
+        if isinstance(source, GroupMessage):
+            await app.send_group_message(source.sender.group, help_message)
+        else:
+            await app.send_message(source.sender, help_message)  # type: ignore
+
+    async def property(
+        self,
+        dispatcher: AlconnaDispatcher,
+        result: Arparma[MessageChain],
+        output_text: str | None = None,
+        source: MessageEvent | None = None,
     ) -> AlconnaProperty[MessageEvent]:
         if not isinstance(source, MessageEvent) or (result.matched or not output_text):
             return AlconnaProperty(result, None, source)
-        if exclude:
-            id_ = str(source.source.id) if source else '_'
-            cache = self.output_cache.setdefault(id_, set())
-            if dispatcher.command in cache:
-                return AlconnaProperty(result, None, source)
-            cache.clear()
-            cache.add(dispatcher.command)
         if dispatcher.send_flag == "stay":
             return AlconnaProperty(result, output_text, source)
         if dispatcher.send_flag == "reply":
-            app: Ariadne = Ariadne.current()
-            help_message: MessageChain = await run_always_await(
-                dispatcher.converter,
-                str(result.error_info) if isinstance(result.error_info, SpecialOptionTriggered) else "help",
-                output_text
-            )
-            if isinstance(source, GroupMessage):
-                await app.send_group_message(source.sender.group, help_message)
-            else:
-                await app.send_message(source.sender, help_message)  # type: ignore
+            await self.send(dispatcher, result, output_text, source)
         elif dispatcher.send_flag == "post":
             with suppress(LookupError):
                 interface = DispatcherInterface.ctx.get()
                 dispatchers = resolve_dispatchers_mixin([source.Dispatcher, ContextDispatcher]) + [
                     self.Dispatcher(dispatcher.command, output_text, source)
                 ]
                 for listener in interface.broadcast.default_listener_generator(AlconnaOutputMessage):
@@ -124,12 +128,12 @@
 class AriadneMessageChainArgv(BaseMessageChainArgv):
     ...
 
 
 set_default_argv_type(AriadneMessageChainArgv)
 argv_config(
     target=AriadneMessageChainArgv,
-    filter_out=["Source", "File", "Quote"],
+    filter_out=[Source, File, Quote],
     checker=lambda x: isinstance(x, MessageChain),
     to_text=lambda x: x.text if x.__class__ is Plain else None,
-    converter=lambda x: MessageChain(x)
+    converter=lambda x: MessageChain(x),
 )
```

### Comparing `arclet-alconna-ariadne-0.13.1/src/arclet/alconna/ariadne/typings.py` & `arclet-alconna-ariadne-0.13.2/src/arclet/alconna/ariadne/typings.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ariadne-0.13.1/PKG-INFO` & `arclet-alconna-ariadne-0.13.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-ariadne
-Version: 0.13.1
+Version: 0.13.2
 Summary: Support Alconna to GraiaProject/Ariadne
 License: AGPL-3.0
 Keywords: alconna,graia,arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

