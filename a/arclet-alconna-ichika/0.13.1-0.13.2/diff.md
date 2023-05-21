# Comparing `tmp/arclet-alconna-ichika-0.13.1.tar.gz` & `tmp/arclet-alconna-ichika-0.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-ichika-0.13.1.tar", last modified: Thu May 11 16:06:02 2023, max compression
+gzip compressed data, was "arclet-alconna-ichika-0.13.2.tar", last modified: Sun May 21 05:34:50 2023, max compression
```

## Comparing `arclet-alconna-ichika-0.13.1.tar` & `arclet-alconna-ichika-0.13.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ichika-0.13.1/LICENSE
--rw-r--r--   0        0        0     6164 2023-05-11 15:54:03.114473 arclet-alconna-ichika-0.13.1/pyproject.toml
--rw-r--r--   0        0        0     7402 2023-05-10 15:25:33.392236 arclet-alconna-ichika-0.13.1/README.md
--rw-r--r--   0        0        0       80 2023-05-09 04:08:01.631055 arclet-alconna-ichika-0.13.1/src/arclet/alconna/ichika/__init__.py
--rw-r--r--   0        0        0     6020 2023-05-11 05:46:08.929144 arclet-alconna-ichika-0.13.1/src/arclet/alconna/ichika/adapter.py
--rw-r--r--   0        0        0     1256 2023-05-09 04:21:37.796354 arclet-alconna-ichika-0.13.1/src/arclet/alconna/ichika/typings.py
--rw-r--r--   0        0        0     7842 1970-01-01 00:00:00.000000 arclet-alconna-ichika-0.13.1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet-alconna-ichika-0.13.2/LICENSE
+-rw-r--r--   0        0        0     6164 2023-05-21 03:55:55.277777 arclet-alconna-ichika-0.13.2/pyproject.toml
+-rw-r--r--   0        0        0     7402 2023-05-10 15:25:33.392236 arclet-alconna-ichika-0.13.2/README.md
+-rw-r--r--   0        0        0       80 2023-05-09 04:08:01.631055 arclet-alconna-ichika-0.13.2/src/arclet/alconna/ichika/__init__.py
+-rw-r--r--   0        0        0     6078 2023-05-21 05:29:50.803685 arclet-alconna-ichika-0.13.2/src/arclet/alconna/ichika/adapter.py
+-rw-r--r--   0        0        0     1256 2023-05-09 04:21:37.796354 arclet-alconna-ichika-0.13.2/src/arclet/alconna/ichika/typings.py
+-rw-r--r--   0        0        0     7842 1970-01-01 00:00:00.000000 arclet-alconna-ichika-0.13.2/PKG-INFO
```

### Comparing `arclet-alconna-ichika-0.13.1/LICENSE` & `arclet-alconna-ichika-0.13.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ichika-0.13.1/pyproject.toml` & `arclet-alconna-ichika-0.13.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
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
@@ -56,29 +56,29 @@
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
@@ -108,20 +108,20 @@
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
@@ -149,20 +149,20 @@
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
@@ -191,20 +191,20 @@
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

### Comparing `arclet-alconna-ichika-0.13.1/README.md` & `arclet-alconna-ichika-0.13.2/README.md`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ichika-0.13.1/src/arclet/alconna/ichika/adapter.py` & `arclet-alconna-ichika-0.13.2/src/arclet/alconna/ichika/adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,67 +42,74 @@
     result = []
     for dispatcher in dispatchers:
         result.extend(dispatcher_mixin_handler(dispatcher))
     return result
 
 
 class AlconnaIchikaAdapter(AlconnaGraiaAdapter[MessageEvent]):
-    def completion_waiter(self, interface: DispatcherInterface[MessageEvent], priority: int = 15) -> Waiter:
+    def completion_waiter(self, source: MessageEvent, priority: int = 15) -> Waiter:
         @Waiter.create_using_function(
-            [interface.event.__class__], block_propagation=True, priority=priority,
+            [source.__class__],
+            block_propagation=True,
+            priority=priority,
         )
         async def waiter(m: MessageChain):
             return m
 
         return waiter  # type: ignore
 
     async def lookup_source(self, interface: DispatcherInterface[MessageEvent]) -> MessageChain:
         return await interface.lookup_param("__message_chain__", MessageChain, MessageChain([Text("Unknown")]))
 
-    async def send(
+    def source_id(self, source: MessageEvent | None = None) -> str:
+        return str(source.source.id) if source else "_"
+
+    async def property(
         self,
         dispatcher: AlconnaDispatcher,
         result: Arparma[MessageChain],
         output_text: str | None = None,
         source: MessageEvent | None = None,
-        exclude: bool = True,
     ) -> AlconnaProperty[MessageEvent]:
         if not isinstance(source, MessageEvent) or (result.matched or not output_text):
             return AlconnaProperty(result, None, source)
-        if exclude:
-            id_ = str(source.source.seq) if source else '_'
-            cache = self.output_cache.setdefault(id_, set())
-            if dispatcher.command in cache:
-                return AlconnaProperty(result, None, source)
-            cache.clear()
-            cache.add(dispatcher.command)
         if dispatcher.send_flag == "stay":
             return AlconnaProperty(result, output_text, source)
         if dispatcher.send_flag == "reply":
-            client: Client = CLIENT_INSTANCE.get()
-            help_message: MessageChain = await run_always_await(
-                dispatcher.converter,
-                str(result.error_info) if isinstance(result.error_info, SpecialOptionTriggered) else "help",
-                output_text
-            )
-            if isinstance(source, GroupMessage):
-                await client.send_group_message(source.group.uin, help_message)
-            else:
-                await client.send_friend_message(source.sender.uin, help_message)  # type: ignore
+            await self.send(dispatcher, result, output_text, source)
         elif dispatcher.send_flag == "post":
             with suppress(LookupError):
                 interface = DispatcherInterface.ctx.get()
                 dispatchers = resolve_dispatchers_mixin([source.Dispatcher, IchikaClientDispatcher]) + [
                     self.Dispatcher(dispatcher.command, output_text, source)
                 ]
                 for listener in interface.broadcast.default_listener_generator(AlconnaOutputMessage):
                     await interface.broadcast.Executor(listener, dispatchers)
                     listener.oplog.clear()
         return AlconnaProperty(result, None, source)
 
+    async def send(
+        self,
+        dispatcher: AlconnaDispatcher,
+        result: Arparma[MessageChain],
+        output_text: str | None = None,
+        source: MessageEvent | None = None,
+    ) -> None:
+        client: Client = CLIENT_INSTANCE.get()
+        help_message: MessageChain = await run_always_await(
+            dispatcher.converter,
+            str(result.error_info) if isinstance(result.error_info, SpecialOptionTriggered) else "help",
+            output_text,
+        )
+        if isinstance(source, GroupMessage):
+            source: GroupMessage
+            await client.send_group_message(source.group.uin, help_message)
+        else:
+            await client.send_friend_message(source.sender.uin, help_message)  # type: ignore
+
     def fetch_name(self, path: str) -> Depend:
         async def __wrapper__(result: AlconnaProperty):
             event = result.source
             arp = result.result
             if t := arp.all_matched_args.get(path, None):
                 return t.display or "Unknown" if isinstance(t, At) else t
             elif isinstance(event.sender, Friend):
```

### Comparing `arclet-alconna-ichika-0.13.1/src/arclet/alconna/ichika/typings.py` & `arclet-alconna-ichika-0.13.2/src/arclet/alconna/ichika/typings.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-ichika-0.13.1/PKG-INFO` & `arclet-alconna-ichika-0.13.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-ichika
-Version: 0.13.1
+Version: 0.13.2
 Summary: Support Alconna to BlueGlassBlock/Ichika
 License: AGPL-3.0
 Keywords: alconna,graia,arclet,ichika
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

