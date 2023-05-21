# Comparing `tmp/Shimarin-0.0.6.tar.gz` & `tmp/Shimarin-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shimarin-0.0.6.tar", last modified: Sat May 20 00:02:44 2023, max compression
+gzip compressed data, was "Shimarin-0.0.7.tar", last modified: Sun May 21 03:10:39 2023, max compression
```

## Comparing `Shimarin-0.0.6.tar` & `Shimarin-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:02:44.248553 Shimarin-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-20 00:02:44.248553 Shimarin-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-20 00:02:35.000000 Shimarin-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:02:44.248553 Shimarin-0.0.6/Shimarin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:02:35.000000 Shimarin-0.0.6/Shimarin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:02:44.248553 Shimarin-0.0.6/Shimarin/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:02:35.000000 Shimarin-0.0.6/Shimarin/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-20 00:02:35.000000 Shimarin-0.0.6/Shimarin/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-20 00:02:35.000000 Shimarin-0.0.6/Shimarin/client/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-20 00:02:35.000000 Shimarin-0.0.6/Shimarin/client/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:02:44.248553 Shimarin-0.0.6/Shimarin/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 00:02:35.000000 Shimarin-0.0.6/Shimarin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-20 00:02:35.000000 Shimarin-0.0.6/Shimarin/server/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 00:02:44.248553 Shimarin-0.0.6/Shimarin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-20 00:02:44.000000 Shimarin-0.0.6/Shimarin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-20 00:02:44.000000 Shimarin-0.0.6/Shimarin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:02:44.000000 Shimarin-0.0.6/Shimarin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 00:02:44.000000 Shimarin-0.0.6/Shimarin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 00:02:44.000000 Shimarin-0.0.6/Shimarin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-20 00:02:35.000000 Shimarin-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-20 00:02:44.248553 Shimarin-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:10:39.561192 Shimarin-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-21 03:10:39.561192 Shimarin-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-21 03:10:29.000000 Shimarin-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:10:39.561192 Shimarin-0.0.7/Shimarin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 03:10:29.000000 Shimarin-0.0.7/Shimarin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:10:39.561192 Shimarin-0.0.7/Shimarin/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 03:10:29.000000 Shimarin-0.0.7/Shimarin/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-21 03:10:29.000000 Shimarin-0.0.7/Shimarin/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-21 03:10:29.000000 Shimarin-0.0.7/Shimarin/client/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-21 03:10:29.000000 Shimarin-0.0.7/Shimarin/client/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:10:39.561192 Shimarin-0.0.7/Shimarin/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 03:10:29.000000 Shimarin-0.0.7/Shimarin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-21 03:10:29.000000 Shimarin-0.0.7/Shimarin/server/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 03:10:39.561192 Shimarin-0.0.7/Shimarin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-21 03:10:39.000000 Shimarin-0.0.7/Shimarin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-21 03:10:39.000000 Shimarin-0.0.7/Shimarin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:10:39.000000 Shimarin-0.0.7/Shimarin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 03:10:39.000000 Shimarin-0.0.7/Shimarin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-21 03:10:39.000000 Shimarin-0.0.7/Shimarin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 03:10:39.000000 Shimarin-0.0.7/Shimarin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-21 03:10:29.000000 Shimarin-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-21 03:10:39.565192 Shimarin-0.0.7/setup.cfg
```

### Comparing `Shimarin-0.0.6/PKG-INFO` & `Shimarin-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimarin
-Version: 0.0.6
+Version: 0.0.7
 Summary: asynchronous event-based communication between client and server
 Home-page: 
 Author: Kamuri Amorim
 Author-email: myk.gata14@gmail.com
 License: MIT
 Keywords: python events client server asynchronous
 Description-Content-Type: text/markdown
```

### Comparing `Shimarin-0.0.6/Shimarin/client/events.py` & `Shimarin-0.0.7/Shimarin/server/events.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,115 +1,88 @@
-import aiohttp
 import asyncio
-import json
-
+import inspect
+import uuid
+from datetime import datetime
 from typing import Callable, Any
 
-from .config import config
-from .networking import send_get_request, Response
-
 
 class Event:
-    def __init__(self, event_type: str, identifier: str, payload: str | None, session: aiohttp.ClientSession) -> None:
+    def __init__(self, event_type: str, payload: str = None, callback: Callable |  None = None):
         self.event_type = event_type
         self.payload = payload
-        self.identifier = identifier
-        self.__session = session
+        self.callback = callback
+        self.identifier = str(uuid.uuid1())
+        self.answered = True if callback is None else False
+        self.__answer = ""
+        self.__creation_date = datetime.now()
+        self.done = False
+        self.delete = False  # this config will be used later when callbacks are merged into emitter
 
     @staticmethod
-    def new(event_data: dict[str, str], session: aiohttp.ClientSession | None) -> 'Event':
-        return Event(event_data['event_type'], event_data['identifier'], event_data['payload'], session)
+    def new(event_type: str, payload: str = None, callback: Callable |  None = None) -> 'Event':
+        return Event(event_type, payload, callback)
     
-    async def reply(self, payload: Any):
-        data = {
-            "identifier": str(self.identifier),
-            "payload": json.dumps(payload)
+    @property
+    def age(self):
+        return datetime.now() - self.__creation_date
+    
+    @property
+    def answer(self):
+        self.done = True
+        return self.__answer
+    
+    async def get_answer(self):
+        while self.answered is False:
+            await asyncio.sleep(0)
+        return self.answer
+
+    def json(self) -> dict:
+        return {
+            "event_type": self.event_type,
+            "payload": self.payload,
+            "identifier": self.identifier
         }
-        await send_get_request(self.__session, f"{config.SERVER_ENDPOINT}/callback", json=data)
     
-    def __str__(self) -> str:
-        return f"Event: {self.event_type}, Identifier: {self.identifier}, Payload: {self.payload}"
+    def __repr__(self):
+        return self.json().__str__()
     
-    def __repr__(self) -> str:
-        return self.__str__()
+    async def trigger(self, payload: Any):
+        self.answered = True
+        if inspect.iscoroutinefunction(self.callback):
+            self.__answer = await self.callback(payload)
+        else:
+            self.__answer = self.callback(payload)
+        return self.__answer
 
 
-class EventHandler:
-    def __init__(self, event_type: str, callback: Callable[[Any, Any], Any]) -> None:
-        self.event_type = event_type
-        self.callback = callback
+class EventEmitter:
+    def __init__(self):
+        self.events: list[Event] = []
 
-    async def trigger(self, *args, **kwargs) -> None:
-        await self.callback(*args, **kwargs)
+    async def fetch_event(self, last: bool = True) -> Event:
+        try:
+            return self.events.pop(0 if not last else -1)
+        except IndexError:
+            return Event(None, None, None)
+        
+    async def send(self, event: Event) -> None:
+        self.events.append(event)
 
-    def __str__(self) -> str:
-        return f"Event: {self.event_type}, Callback: {self.callback}"
-    
-    def __repr__(self) -> str:
-        return self.__str__()
 
-
-class EventsHandlers:
+class CallbacksHandlers:
     def __init__(self):
-        self.handlers: list[EventHandler] = []
-    
-    def register(self, handler: EventHandler) -> None:
-        self.handlers.append(handler)
-
-    def new(self, event_name: str):
-        def wrapper(func: Callable):
-            event_handler = EventHandler(event_name, func)
-            self.register(event_handler)
-            return func
-        return wrapper
-
-    async def handle(self, event: Event) -> None:
-        for handle in self.handlers:
-            if handle.event_type == event.event_type:
-                asyncio.gather(handle.trigger(event))
-    
-    def __str__(self) -> str:
-        return f"Handlers: {self.handlers}"
-    
-    def __repr__(self) -> str:
-        return self.__str__()
-
+        self.events: list[Event] = []
 
-class EventPolling:
-    def __init__(self, events_handlers: EventsHandlers) -> None:
-        self.session = aiohttp.ClientSession()
-        self.events_handlers = events_handlers
-        self.is_polling = False
-        self.running_tasks: set[asyncio.Task] = set()
-
-    async def __aenter__(self):
-        await self.session.__aenter__()
-        return self
-
-    async def __aexit__(self, exc_type, exc_val, tb):
-        if self.session:
-            await self.session.__aexit__(exc_type, exc_val, tb)
-
-    async def start(self, polling_interval: int = 1, fetch: int = 10, custom_headers: dict = {}):
-        self.is_polling = True
-        while self.is_polling:
-            events: Response = await send_get_request(self.session, f"{config.SERVER_ENDPOINT}/events?fetch={fetch}", headers=custom_headers)
-            if events.status == 200:
-                event_json = await events.json()
-                for event in event_json:
-                    if event_json:
-                        event = Event.new(event, self.session)
-                        await self.__task_manager(event)
-            await asyncio.sleep(polling_interval)
-
-    async def __task_manager(self, event: Event):
-        task = asyncio.create_task(self.events_handlers.handle(event))
-        self.running_tasks.add(task) 
-        task.add_done_callback(lambda t: self.running_tasks.remove(t))
-
-    async def stop(self):
-        if self.is_polling:
-            self.is_polling = False
-            for task in self.running_tasks:
-                task.cancel()
-            for task in self.running_tasks.copy():
-                self.running_tasks.remove(task)
+    async def clear_done(self):
+        for event in self.events.copy():
+            if event.done:
+                self.events.remove(event)
+
+    async def register(self, event: Event):
+        await self.clear_done()
+        self.events.append(event)
+
+    async def handle(self, unique_identifier: str, payload: Any):
+        await self.clear_done()
+        for event in self.events:
+            if event.identifier == unique_identifier:
+                return await event.trigger(payload)
```

### Comparing `Shimarin-0.0.6/Shimarin/client/networking.py` & `Shimarin-0.0.7/Shimarin/client/networking.py`

 * *Files identical despite different names*

### Comparing `Shimarin-0.0.6/Shimarin.egg-info/PKG-INFO` & `Shimarin-0.0.7/Shimarin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimarin
-Version: 0.0.6
+Version: 0.0.7
 Summary: asynchronous event-based communication between client and server
 Home-page: 
 Author: Kamuri Amorim
 Author-email: myk.gata14@gmail.com
 License: MIT
 Keywords: python events client server asynchronous
 Description-Content-Type: text/markdown
```

