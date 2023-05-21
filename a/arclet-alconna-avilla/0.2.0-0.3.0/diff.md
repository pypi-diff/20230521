# Comparing `tmp/arclet-alconna-avilla-0.2.0.tar.gz` & `tmp/arclet-alconna-avilla-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-avilla-0.2.0.tar", last modified: Mon Sep 19 10:13:39 2022, max compression
+gzip compressed data, was "arclet-alconna-avilla-0.3.0.tar", last modified: Sat Dec 31 15:48:15 2022, max compression
```

## Comparing `arclet-alconna-avilla-0.2.0.tar` & `arclet-alconna-avilla-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-rw-rw-   0        0        0      727 2022-09-12 12:24:39.857371 arclet-alconna-avilla-0.2.0/arclet/alconna/avilla/__init__.py
--rw-rw-rw-   0        0        0     3992 2022-09-19 10:08:59.391806 arclet-alconna-avilla-0.2.0/arclet/alconna/avilla/dispatcher.py
--rw-rw-rw-   0        0        0     3856 2022-09-19 10:13:19.059564 arclet-alconna-avilla-0.2.0/arclet/alconna/avilla/utils.py
--rw-rw-rw-   0        0        0      589 2022-09-19 10:13:19.068539 arclet-alconna-avilla-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      456 2022-09-03 00:30:04.702498 arclet-alconna-avilla-0.2.0/README.md
--rw-rw-rw-   0        0        0      669 2022-09-19 10:13:39.886416 arclet-alconna-avilla-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2022-12-31 15:47:48.075376 arclet-alconna-avilla-0.3.0/arclet/alconna/avilla/__init__.py
+-rw-rw-rw-   0        0        0     3362 2022-12-31 15:20:33.657103 arclet-alconna-avilla-0.3.0/arclet/alconna/avilla/dispatcher.py
+-rw-rw-rw-   0        0        0     5514 2022-12-31 15:45:51.299013 arclet-alconna-avilla-0.3.0/arclet/alconna/avilla/utils.py
+-rw-rw-rw-   0        0        0      559 2022-12-31 15:05:33.257781 arclet-alconna-avilla-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      456 2022-09-03 00:30:04.702498 arclet-alconna-avilla-0.3.0/README.md
+-rw-rw-rw-   0        0        0      669 2022-12-31 15:48:15.929794 arclet-alconna-avilla-0.3.0/PKG-INFO
```

### Comparing `arclet-alconna-avilla-0.2.0/arclet/alconna/avilla/__init__.py` & `arclet-alconna-avilla-0.3.0/arclet/alconna/avilla/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from arclet.alconna.graia import (
+    alc as alc,
     Alc as Alc,
     GraiaCommandAnalyser as GraiaCommandAnalyser,
     Match as Match,
     Query as Query,
+    Header as Header,
     success_record as success_record,
     AlconnaProperty as AlconnaProperty,
     AlconnaSchema as AlconnaSchema,
     AlconnaBehaviour as AlconnaBehaviour,
     shortcuts as shortcuts,
     match_path as match_path,
     match_value as match_value,
```

### Comparing `arclet-alconna-avilla-0.2.0/arclet/alconna/avilla/dispatcher.py` & `arclet-alconna-avilla-0.3.0/arclet/alconna/avilla/dispatcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 from contextlib import suppress
 from typing import Optional, Union
-from arclet.alconna import Arpamar
-from arclet.alconna.core import Alconna, AlconnaGroup
 
+from arclet.alconna import Arparma
+from arclet.alconna.core import Alconna, AlconnaGroup
+from arclet.alconna.graia.dispatcher import AlconnaDispatcher, output_cache
+from arclet.alconna.graia.model import AlconnaProperty
+from avilla.core.context import Context
+from avilla.core.event import AvillaEvent
+from avilla.spec.core.message import MessageReceived
+from graia.amnesia.message import MessageChain
 from graia.broadcast.entities.dispatcher import BaseDispatcher
 from graia.broadcast.interfaces.dispatcher import DispatcherInterface
 from graia.broadcast.utilles import run_always_await
 
-from graia.amnesia.message import MessageChain
-
-from arclet.alconna.graia.dispatcher import output_cache, AlconnaProperty, AlconnaDispatcher
-
-from avilla.core.event import AvillaEvent
-from avilla.core.event.message import MessageReceived
-from avilla.core.relationship import Relationship
-from avilla.core.message import Message
-from avilla.core.utilles.selector import Selector
-
 
 class AvillaOutputDispatcher(BaseDispatcher):
-
     def __init__(
         self, command: Union[Alconna, AlconnaGroup], text: str, source: MessageReceived
     ):
         self.command = command
         self.output = text
         self.source_event = source
 
@@ -50,63 +45,44 @@
 
     output: str
     """输出信息"""
 
     source_event: MessageReceived
     """来源事件"""
 
-    @property
-    def ctx(self) -> Selector:
-        return self.source_event.ctx
-
-
-async def _fetch_quote(self: AlconnaDispatcher, message: MessageChain) -> bool:  # noqa
-    try:
-        interface = DispatcherInterface.ctx.get()
-    except LookupError:
-        return False
-    message: Message = await interface.lookup_param(
-        "message", Message, None
-    )
-    return not self.allow_quote and message.reply
-
-AlconnaDispatcher.fetch_quote = _fetch_quote
-
 
 async def _send_output(
     self: AlconnaDispatcher,
-    result: Arpamar,
+    result: Arparma,
     output_text: Optional[str] = None,
     source: Optional[MessageReceived] = None,
 ) -> AlconnaProperty[MessageReceived]:
     if not isinstance(source, MessageReceived) or (result.matched or not output_text):
         return AlconnaProperty(result, None, source)
     id_ = id(source) if source else 0
     cache = output_cache.setdefault(id_, set())
     if self.command in cache:
         return AlconnaProperty(result, None, source)
     cache.clear()
     cache.add(self.command)
     if self.send_flag == "stay":
         return AlconnaProperty(result, output_text, source)
     if self.send_flag == "reply":
-        rs: Relationship = await source.account.get_relationship(source.ctx)
+        ctx: Context = source.context
         help_message: MessageChain = await run_always_await(
             self.send_handler, output_text
         )
-        await rs.send_message(help_message)
+        await ctx.scene.send_message(help_message)
     elif self.send_flag == "post":
         with suppress(LookupError):
             interface = DispatcherInterface.ctx.get()
             dispatchers = [AvillaOutputDispatcher(self.command, output_text, source)]
             for listener in interface.broadcast.default_listener_generator(
-                    AvillaAlconnaOutputMessage
+                AvillaAlconnaOutputMessage
             ):
-                await interface.broadcast.Executor(
-                    listener, dispatchers=dispatchers
-                )
+                await interface.broadcast.Executor(listener, dispatchers=dispatchers)
                 listener.oplog.clear()
             return AlconnaProperty(result, None, source)
     return AlconnaProperty(result, None, source)
 
 
 AlconnaDispatcher.send_output = _send_output
```

### Comparing `arclet-alconna-avilla-0.2.0/PKG-INFO` & `arclet-alconna-avilla-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-avilla
-Version: 0.2.0
+Version: 0.3.0
 Summary: Support Alconna for Avilla
 License: AGPL-3.0
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Alconna-Avilla
```

