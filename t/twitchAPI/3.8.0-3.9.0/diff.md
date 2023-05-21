# Comparing `tmp/twitchAPI-3.8.0.tar.gz` & `tmp/twitchAPI-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitchAPI-3.8.0.tar", last modified: Sun Feb 12 16:57:38 2023, max compression
+gzip compressed data, was "twitchAPI-3.9.0.tar", last modified: Sun Feb 26 16:09:48 2023, max compression
```

## Comparing `twitchAPI-3.8.0.tar` & `twitchAPI-3.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 16:57:38.865867 twitchAPI-3.8.0/
--rw-rw-rw-   0        0        0     1097 2020-03-23 19:50:28.000000 twitchAPI-3.8.0/LICENSE.txt
--rw-rw-rw-   0        0        0      110 2022-12-20 09:55:59.000000 twitchAPI-3.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0    12510 2023-02-12 16:57:38.865867 twitchAPI-3.8.0/PKG-INFO
--rw-rw-rw-   0        0        0    11333 2022-11-27 13:26:22.000000 twitchAPI-3.8.0/README.md
--rw-rw-rw-   0        0        0       93 2023-01-09 23:43:30.000000 twitchAPI-3.8.0/pyproject.toml
--rw-rw-rw-   0        0        0     1094 2023-02-12 16:57:38.866877 twitchAPI-3.8.0/setup.cfg
--rw-rw-rw-   0        0        0      641 2023-01-25 20:06:39.000000 twitchAPI-3.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-12 16:57:38.847872 twitchAPI-3.8.0/twitchAPI/
--rw-rw-rw-   0        0        0      198 2023-02-12 16:52:44.000000 twitchAPI-3.8.0/twitchAPI/__init__.py
--rw-rw-rw-   0        0        0    51218 2023-02-12 16:20:06.000000 twitchAPI-3.8.0/twitchAPI/chat.py
--rw-rw-rw-   0        0        0    75429 2023-02-12 01:53:32.000000 twitchAPI-3.8.0/twitchAPI/eventsub.py
--rw-rw-rw-   0        0        0     9245 2023-02-11 10:53:02.000000 twitchAPI-3.8.0/twitchAPI/helper.py
--rw-rw-rw-   0        0        0    15098 2023-02-04 03:51:25.000000 twitchAPI-3.8.0/twitchAPI/oauth.py
--rw-rw-rw-   0        0        0    22831 2023-01-31 06:17:28.000000 twitchAPI-3.8.0/twitchAPI/object.py
--rw-rw-rw-   0        0        0    30695 2023-02-07 01:42:31.000000 twitchAPI-3.8.0/twitchAPI/pubsub.py
--rw-rw-rw-   0        0        0        0 2023-01-25 20:05:14.000000 twitchAPI-3.8.0/twitchAPI/py.typed
--rw-rw-rw-   0        0        0   247416 2023-02-12 01:43:28.000000 twitchAPI-3.8.0/twitchAPI/twitch.py
--rw-rw-rw-   0        0        0    11155 2023-02-12 01:32:01.000000 twitchAPI-3.8.0/twitchAPI/types.py
-drwxrwxrwx   0        0        0        0 2023-02-12 16:57:38.864876 twitchAPI-3.8.0/twitchAPI.egg-info/
--rw-rw-rw-   0        0        0    12510 2023-02-12 16:57:38.000000 twitchAPI-3.8.0/twitchAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2023-02-12 16:57:38.000000 twitchAPI-3.8.0/twitchAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 16:57:38.000000 twitchAPI-3.8.0/twitchAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-02-12 16:57:38.000000 twitchAPI-3.8.0/twitchAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-12 16:57:38.000000 twitchAPI-3.8.0/twitchAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-12-20 09:46:34.000000 twitchAPI-3.8.0/twitchAPI.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-02-26 16:09:48.938179 twitchAPI-3.9.0/
+-rw-rw-rw-   0        0        0     1097 2020-03-23 19:50:28.000000 twitchAPI-3.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      110 2022-12-20 09:55:59.000000 twitchAPI-3.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12510 2023-02-26 16:09:48.938179 twitchAPI-3.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11333 2022-11-27 13:26:22.000000 twitchAPI-3.9.0/README.md
+-rw-rw-rw-   0        0        0       93 2023-01-09 23:43:30.000000 twitchAPI-3.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1094 2023-02-26 16:09:48.939180 twitchAPI-3.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-01-25 20:06:39.000000 twitchAPI-3.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-26 16:09:48.919175 twitchAPI-3.9.0/twitchAPI/
+-rw-rw-rw-   0        0        0      198 2023-02-26 16:05:27.000000 twitchAPI-3.9.0/twitchAPI/__init__.py
+-rw-rw-rw-   0        0        0    54260 2023-02-23 14:26:56.000000 twitchAPI-3.9.0/twitchAPI/chat.py
+-rw-rw-rw-   0        0        0    77343 2023-02-23 14:53:45.000000 twitchAPI-3.9.0/twitchAPI/eventsub.py
+-rw-rw-rw-   0        0        0     9259 2023-02-14 04:40:25.000000 twitchAPI-3.9.0/twitchAPI/helper.py
+-rw-rw-rw-   0        0        0    15092 2023-02-14 04:09:29.000000 twitchAPI-3.9.0/twitchAPI/oauth.py
+-rw-rw-rw-   0        0        0    25111 2023-02-23 14:01:11.000000 twitchAPI-3.9.0/twitchAPI/object.py
+-rw-rw-rw-   0        0        0    30783 2023-02-14 04:42:54.000000 twitchAPI-3.9.0/twitchAPI/pubsub.py
+-rw-rw-rw-   0        0        0        0 2023-01-25 20:05:14.000000 twitchAPI-3.9.0/twitchAPI/py.typed
+-rw-rw-rw-   0        0        0   251309 2023-02-23 14:04:59.000000 twitchAPI-3.9.0/twitchAPI/twitch.py
+-rw-rw-rw-   0        0        0    11220 2023-02-14 17:27:43.000000 twitchAPI-3.9.0/twitchAPI/types.py
+drwxrwxrwx   0        0        0        0 2023-02-26 16:09:48.937179 twitchAPI-3.9.0/twitchAPI.egg-info/
+-rw-rw-rw-   0        0        0    12510 2023-02-26 16:09:48.000000 twitchAPI-3.9.0/twitchAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2023-02-26 16:09:48.000000 twitchAPI-3.9.0/twitchAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-26 16:09:48.000000 twitchAPI-3.9.0/twitchAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-02-26 16:09:48.000000 twitchAPI-3.9.0/twitchAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-02-26 16:09:48.000000 twitchAPI-3.9.0/twitchAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-12-20 09:46:34.000000 twitchAPI-3.9.0/twitchAPI.egg-info/zip-safe
```

### Comparing `twitchAPI-3.8.0/LICENSE.txt` & `twitchAPI-3.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `twitchAPI-3.8.0/PKG-INFO` & `twitchAPI-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchAPI
-Version: 3.8.0
+Version: 3.9.0
 Summary: A Python 3.7+ implementation of the Twitch Helix API, PubSub, EventSub and Chat
 Home-page: https://github.com/Teekeks/pyTwitchAPI
 Author: Lena "Teekeks" During
 Author-email: info@teawork.de
 License: MIT
 Keywords: twitch,twitch.tv,chat,bot,event sub,EventSub,pub sub,PubSub,helix,api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `twitchAPI-3.8.0/README.md` & `twitchAPI-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `twitchAPI-3.8.0/setup.cfg` & `twitchAPI-3.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `twitchAPI-3.8.0/setup.py` & `twitchAPI-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `twitchAPI-3.8.0/twitchAPI/chat.py` & `twitchAPI-3.9.0/twitchAPI/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 Bot Ready
 =========
 
 - ChatEvent: :const:`~twitchAPI.types.ChatEvent.READY`
 - Payload: :const:`~twitchAPI.chat.EventData`
 
-This Event is triggered when the bot is stared up and ready to join channels.
+This Event is triggered when the bot is started up and ready to join channels.
 
 Message send
 ============
 
 - ChatEvent: :const:`~twitchAPI.types.ChatEvent.MESSAGE`
 - Payload: :const:`~twitchAPI.chat.ChatMessage`
 
@@ -157,14 +157,22 @@
 - ChatEvent: :const:`~twitchAPI.types.ChatEvent.WHISPER`
 - Payload: :const:`~twitchAPI.chat.WhisperEvent`
 
 Triggered when someone whispers to your bot.
 
 .. note:: You need the :const:`~twitchAPI.types.AuthScope.WHISPERS_READ` Auth Scope to receive this Event.
 
+Server notice
+============================
+
+- ChatEvent: :const:`~twitchAPI.types.ChatEvent.NOTICE`
+- Payload: :const:`~twitchAPI.chat.NoticeEvent`
+
+Triggered when server sends a notice message.
+
 
 ************
 Code example
 ************
 
 .. code-block:: python
 
@@ -262,20 +270,20 @@
 from asyncio import CancelledError
 from logging import getLogger, Logger
 from time import sleep
 import aiohttp
 from twitchAPI.twitch import Twitch
 from twitchAPI.object import TwitchUser
 from twitchAPI.helper import TWITCH_CHAT_URL, first, RateLimitBucket, RATE_LIMIT_SIZES
-from twitchAPI.types import ChatRoom, TwitchBackendException, AuthType, AuthScope, ChatEvent, MissingScopeException, UnauthorizedException
+from twitchAPI.types import ChatRoom, TwitchBackendException, AuthType, AuthScope, ChatEvent, UnauthorizedException
 
 from typing import List, Optional, Union, Callable, Dict, Awaitable, Any
 
 __all__ = ['Chat', 'ChatUser', 'EventData', 'ChatMessage', 'ChatCommand', 'ChatSub', 'ChatRoom', 'ChatEvent', 'RoomStateChangeEvent',
-           'JoinEvent', 'JoinedEvent', 'LeftEvent', 'ClearChatEvent', 'WhisperEvent', 'MessageDeletedEvent']
+           'JoinEvent', 'JoinedEvent', 'LeftEvent', 'ClearChatEvent', 'WhisperEvent', 'MessageDeletedEvent', 'NoticeEvent']
 
 
 class ChatUser:
     """Represents a user in a chat channel
     """
 
     def __init__(self, chat, parsed, name_override=None):
@@ -508,14 +516,31 @@
         """The message that was send"""
 
     @property
     def user(self) -> ChatUser:
         """The user that DMed your bot"""
         return ChatUser(self.chat, self._parsed)
 
+class NoticeEvent(EventData):
+    """Represents a server notice"""
+    
+    def __init__(self, chat, parsed):
+        super(NoticeEvent, self).__init__(chat)
+        self._room_name = parsed['command']['channel'][1:]
+        """The name of the chat room the notice is from"""
+        self.msg_id: str = parsed['tags'].get('msg-id')
+        """Message ID of the notice, `Msg-id reference <https://dev.twitch.tv/docs/irc/msg-id/>`__"""
+        self.message: str = parsed['parameters']
+        """Description for the msg_id"""
+
+    @property
+    def room(self) -> Optional[ChatRoom]:
+        """The room this notice is from"""
+        return self.chat.room_cache.get(self._room_name)
+        
 
 COMMAND_CALLBACK_TYPE = Callable[[ChatCommand], Awaitable[None]]
 EVENT_CALLBACK_TYPE = Callable[[Any], Awaitable[None]]
 
 
 class Chat:
     """The chat bot instance"""
@@ -536,39 +561,40 @@
         self._prefix: str = "!"
         self.twitch: Twitch = twitch
         if not self.twitch.has_required_auth(AuthType.USER, [AuthScope.CHAT_READ]):
             raise ValueError('passed twitch instance is missing User Auth.')
         self.connection_url: str = connection_url if connection_url is not None else TWITCH_CHAT_URL
         self.ping_frequency: int = 120
         self.ping_jitter: int = 4
-        self._initial_channel: Optional[List[str]] = initial_channel
         self.listen_confirm_timeout: int = 30
         self.reconnect_delay_steps: List[int] = [0, 1, 2, 4, 8, 16, 32, 64, 128]
         self.log_no_registered_command_handler: bool = True
         """Controls if instances of commands being issued in chat where no handler exists should be logged. |default|:code:`True`"""
         self.__connection = None
         self._session = None
-        self.__socket_thread: threading.Thread = None
+        self.__socket_thread: Optional[threading.Thread] = None
         self.__running: bool = False
         self.__socket_loop = None
         self.__startup_complete: bool = False
         self.__tasks = None
         self._ready = False
         self._send_buckets = {}
+        self._join_target = initial_channel if initial_channel is not None else []
         self._join_bucket = RateLimitBucket(10, 2000 if is_verified_bot else 20, 'channel_join', self.logger)
         self.__waiting_for_pong: bool = False
         self._event_handler = {}
         self._command_handler = {}
         self.room_cache: Dict[str, ChatRoom] = {}
         self._room_join_locks = []
         self._room_leave_locks = []
         self._closing: bool = False
         self.join_timeout: int = 10
-        self._mod_status_cache = {}
         """Time in seconds till a channel join attempt times out"""
+        self._mod_status_cache = {}
+        self._subscriber_status_cache = {}
 
     def __await__(self):
         t = asyncio.create_task(self._get_username())
         yield from t
         return self
 
     async def _get_username(self):
@@ -636,35 +662,36 @@
         parsed_message['parameters'] = raw_parameters_component
         if raw_parameters_component is not None and raw_parameters_component.startswith(self._prefix):
             parsed_message['command'] = self._parse_irc_parameters(raw_parameters_component, parsed_message['command'])
 
         return parsed_message
 
     def _parse_irc_parameters(self, raw_parameters_component: str, command):
-        idx = 0
         command_parts = raw_parameters_component[len(self._prefix)::].strip()
         try:
             params_idx = command_parts.index(' ')
         except ValueError:
             command['bot_command'] = command_parts
             return command
         command['bot_command'] = command_parts[:params_idx]
         command['bot_command_params'] = command_parts[params_idx:].strip()
         return command
 
-    def _parse_irc_source(self, raw_source_component: str):
+    @staticmethod
+    def _parse_irc_source(raw_source_component: str):
         if raw_source_component is None:
             return None
         source_parts = raw_source_component.split('!')
         return {
             'nick': source_parts[0] if len(source_parts) == 2 else None,
             'host': source_parts[1] if len(source_parts) == 2 else source_parts[0]
         }
 
-    def _parse_irc_tags(self, raw_tags_component: str):
+    @staticmethod
+    def _parse_irc_tags(raw_tags_component: str):
         tags_to_ignore = ('client-nonce', 'flags')
         parsed_tags = {}
 
         tags = raw_tags_component.split(';')
 
         for tag in tags:
             parsed_tag = tag.split('=')
@@ -791,15 +818,18 @@
         self._session = None
         self.room_cache = {}
         self._room_join_locks = []
         self._room_leave_locks = []
         self._closing = True
 
     async def __connect(self, is_startup=False):
-        self.logger.debug('connecting...')
+        if is_startup:
+            self.logger.debug('connecting...')
+        else:
+            self.logger.debug('reconnecting...')
         if self.__connection is not None and not self.__connection.closed:
             await self.__connection.close()
         retry = 0
         need_retry = True
         if self._session is None:
             self._session = aiohttp.ClientSession(timeout=self.twitch.session_timeout)
         while need_retry and retry < len(self.reconnect_delay_steps):
@@ -828,15 +858,16 @@
         self.__tasks = [
             asyncio.ensure_future(self.__task_receive(), loop=self.__socket_loop),
             asyncio.ensure_future(self.__task_startup(), loop=self.__socket_loop)
         ]
         # keep loop alive
         self.__socket_loop.run_until_complete(self._keep_loop_alive())
 
-    def _task_callback(self, task: asyncio.Task):
+    @staticmethod
+    def _task_callback(task: asyncio.Task):
         e = task.exception()
         if e is not None:
             traceback.print_exception(type(e), e, e.__traceback__, file=sys.stderr)
 
     async def _send_message(self, message: str):
         self.logger.debug(f'> "{message}"')
         await self.__connection.send_str(message)
@@ -872,26 +903,38 @@
                         if parsed is None:
                             continue
                         handler = handlers.get(parsed['command']['command'])
                         if handler is not None:
                             asyncio.ensure_future(handler(parsed))
                 elif message.type == aiohttp.WSMsgType.CLOSED:
                     self.logger.debug('websocket is closing')
-                    break
+                    if self.__running:
+                        try:
+                            await self._handle_base_reconnect()
+                        except TwitchBackendException:
+                            self.logger.exception('Connection to chat websocket lost and unable to reestablish connection!')
+                            break
+                    else:
+                        break
                 elif message.type == aiohttp.WSMsgType.ERROR:
-                    self.logger.warning('error in websocket')
+                    self.logger.warning('error in websocket: ' + str(self.__connection.exception()))
                     break
         except CancelledError:
             # we are closing down!
             # print('we are closing down!')
             return
 
+    async def _handle_base_reconnect(self):
+        await self.__connect(is_startup=False)
+        await self.__task_startup()
+
+    # noinspection PyUnusedLocal
     async def _handle_reconnect(self, parsed: dict):
         self.logger.info('got reconnect request...')
-        await self.__connect(is_startup=False)
+        await self._handle_base_reconnect()
         self.logger.info('reconnect completed')
 
     async def _handle_whisper(self, parsed: dict):
         e = WhisperEvent(self, parsed)
         for handler in self._event_handler.get(ChatEvent.WHISPER, []):
             t = asyncio.ensure_future(handler(e))
             t.add_done_callback(self._task_callback)
@@ -899,16 +942,19 @@
     async def _handle_clear_chat(self, parsed: dict):
         e = ClearChatEvent(self, parsed)
         for handler in self._event_handler.get(ChatEvent.CHAT_CLEARED, []):
             t = asyncio.ensure_future(handler(e))
             t.add_done_callback(self._task_callback)
 
     async def _handle_notice(self, parsed: dict):
+        e = NoticeEvent(self, parsed)
+        for handler in self._event_handler.get(ChatEvent.NOTICE, []):
+            t = asyncio.ensure_future(handler(e))
+            t.add_done_callback(self._task_callback)
         self.logger.debug(f'got NOTICE for channel {parsed["command"]["channel"]}: {parsed["tags"]["msg-id"]}')
-        pass
 
     async def _handle_clear_msg(self, parsed: dict):
         ev = MessageDeletedEvent(self, parsed)
         for handler in self._event_handler.get(ChatEvent.MESSAGE_DELETE, []):
             t = asyncio.ensure_future(handler(ev))
             t.add_done_callback(self._task_callback)
 
@@ -986,30 +1032,34 @@
             
     async def _handle_user_state(self, parsed: dict):
         self.logger.debug('got user state event')
         is_broadcaster = False
         if parsed['tags'].get('badges') is not None:
             is_broadcaster = parsed['tags']['badges'].get('broadcaster') is not None
         self._mod_status_cache[parsed['command']['channel'][1:]] = 'mod' if parsed['tags']['mod'] == '1' or is_broadcaster else 'user'
+        self._subscriber_status_cache[parsed['command']['channel'][1:]] = 'sub' if parsed['tags']['subscriber'] == '1' else 'non-sub'
 
     async def _handle_ping(self, parsed: dict):
         self.logger.debug('got PING')
         await self._send_message('PONG ' + parsed['parameters'])
 
+    # noinspection PyUnusedLocal
     async def _handle_ready(self, parsed: dict):
         self.logger.debug('got ready event')
         dat = EventData(self)
+        was_ready = self._ready
         self._ready = True
-        if self._initial_channel is not None and len(self._initial_channel) > 0:
-            _failed = await self.join_room(self._initial_channel)
+        if self._join_target is not None and len(self._join_target) > 0:
+            _failed = await self.join_room(self._join_target)
             if len(_failed) > 0:
                 self.logger.warning(f'failed to join the following channel of the initial following list: {", ".join(_failed)}')
-        for h in self._event_handler.get(ChatEvent.READY, []):
-            t = asyncio.ensure_future(h(dat))
-            t.add_done_callback(self._task_callback)
+        if not was_ready:
+            for h in self._event_handler.get(ChatEvent.READY, []):
+                t = asyncio.ensure_future(h(dat))
+                t.add_done_callback(self._task_callback)
 
     async def _handle_msg(self, parsed: dict):
         self.logger.debug('got new message, call handler')
         if parsed['command'].get('bot_command') is not None:
             command_name = parsed['command'].get('bot_command').lower()
             handler = self._command_handler.get(command_name)
             if handler is not None:
@@ -1022,15 +1072,15 @@
         message = ChatMessage(self, parsed)
         for h in handler:
             t = asyncio.ensure_future(h(message))
             t.add_done_callback(self._task_callback)
 
     async def __task_startup(self):
         await self._send_message('CAP REQ :twitch.tv/membership twitch.tv/tags twitch.tv/commands')
-        await self._send_message(f'PASS oauth:{self.twitch.get_user_auth_token()}')
+        await self._send_message(f'PASS oauth:{await self.twitch.get_refreshed_user_auth_token()}')
         await self._send_message(f'NICK {self.username}')
         self.__startup_complete = True
 
     def _get_message_bucket(self, channel) -> RateLimitBucket:
         bucket = self._send_buckets.get(channel)
         if bucket is None:
             bucket = RateLimitBucket(30, 20, channel, self.logger)
@@ -1114,14 +1164,28 @@
         if isinstance(room, ChatRoom):
             room = room.name
         if room is None or len(room) == 0:
             raise ValueError('please specify a room')
         if room[0] == '#':
             room = room[1:]
         return self._mod_status_cache.get(room.lower(), 'user') == 'mod'
+    
+    def is_subscriber(self, room: Union[str, ChatRoom]) -> bool:
+        """Check if chat bot is a subscriber in a channel
+
+        :param room: The chat room you want to check if bot is a subscriber in.
+            This can either be a instance of :const:`~twitchAPI.types.ChatRoom` or a string with the room name (either with leading # or without)
+        :return: Returns True if chat bot is a subscriber """
+        if isinstance(room, ChatRoom):
+            room = room.name
+        if room is None or len(room) == 0:
+            raise ValueError('please specify a room')
+        if room[0] == '#':
+            room = room[1:]
+        return self._subscriber_status_cache.get(room.lower(), 'user') == 'sub'
 
     def is_in_room(self, room: Union[str, ChatRoom]) -> bool:
         """Check if the bot is currently in the given chat room
 
         :param room: The chat room you want to check
             This can either be a instance of :const:`~twitchAPI.types.ChatRoom` or a string with the room name (either with leading # or without)
         """
@@ -1156,14 +1220,15 @@
             await self._join_bucket.put(len(target))
             await self._send_message(f'JOIN {",".join([f"#{x}" for x in target])}')
         # wait for us to join all rooms
         timeout = datetime.datetime.now() + datetime.timedelta(seconds=self.join_timeout)
         while any([r in self._room_join_locks for r in target]) and timeout > datetime.datetime.now():
             await asyncio.sleep(0.01)
         failed_to_join = [r for r in self._room_join_locks if r in target]
+        self._join_target.extend([x for x in target if x not in failed_to_join])
         for r in failed_to_join:
             self._room_join_locks.remove(r)
         return failed_to_join
 
     async def send_raw_irc_message(self, message: str):
         """Send a raw IRC message
 
@@ -1213,10 +1278,13 @@
         if isinstance(chat_rooms, str):
             chat_rooms = [chat_rooms]
         room_str = ','.join([f'#{c}'.lower() if c[0] != '#' else c.lower() for c in chat_rooms])
         target = [c[1:].lower() if c[0] == '#' else c.lower() for c in chat_rooms]
         for r in target:
             self._room_leave_locks.append(r)
         await self._send_message(f'PART {room_str}')
+        for x in target:
+            if x in self._join_target:
+                self._join_target.remove(x)
         # wait to leave all rooms
         while any([r in self._room_leave_locks for r in target]):
             await asyncio.sleep(0.01)
```

### Comparing `twitchAPI-3.8.0/twitchAPI/eventsub.py` & `twitchAPI-3.9.0/twitchAPI/eventsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         """The full URL of the webhook."""
         self.__client_id: str = api_client_id
         self._port: int = port
         self.__ssl_context: Optional[SSLContext] = ssl_context
         self.__twitch: Twitch = twitch
         self.logger: Logger = getLogger('twitchAPI.eventsub')
         """The logger used for EventSub related log messages"""
-        self.secret: str = ''.join(random.choice(string.ascii_lowercase) for i in range(20))
+        self.secret: str = ''.join(random.choice(string.ascii_lowercase) for _ in range(20))
         """A random secret string. Set this for added security. |default| :code:`A random 20 character long string`"""
         self.wait_for_subscription_confirm: bool = True
         """Set this to false if you don't want to wait for a subscription confirm. |default| :code:`True`"""
         self.wait_for_subscription_confirm_timeout: int = 30
         """Max time in seconds to wait for a subscription confirmation. Only used if ``wait_for_subscription_confirm`` is set to True. 
             |default| :code:`30`"""
         self.unsubscribe_on_stop: bool = True
@@ -296,15 +296,17 @@
                                    digestmod=hashlib.sha256).hexdigest().lower()
         return sig == expected
 
     # ==================================================================================================================
     # HANDLERS
     # ==================================================================================================================
 
-    async def __handle_default(self, request: 'web.Request'):
+    # noinspection PyUnusedLocal
+    @staticmethod
+    async def __handle_default(request: 'web.Request'):
         return web.Response(text="pyTwitchAPI EventSub")
 
     async def __handle_challenge(self, request: 'web.Request', data: dict):
         self.logger.debug(f'received challenge for subscription {data.get("subscription").get("id")}')
         if not await self._verify_signature(request):
             self.logger.warning(f'message signature is not matching! Discarding message')
             return web.Response(status=403)
@@ -371,27 +373,55 @@
         :raises ~twitchAPI.types.TwitchBackendException: if the subscription failed due to a twitch backend error
         """
         return await self._subscribe('channel.update', '1', {'broadcaster_user_id': broadcaster_user_id}, callback)
 
     async def listen_channel_follow(self, broadcaster_user_id: str, callback: CALLBACK_TYPE) -> str:
         """A specified channel receives a follow.
 
+        .. warning:: This subscription is deprecated and will be removed on or soon after the 3rd of August 2023\n
+            Please use :const:`~twitchAPI.eventsub.EventSub.listen_channel_follow_v2()`
+
         For more information see here: https://dev.twitch.tv/docs/eventsub/eventsub-subscription-types#channelfollow
 
         :param broadcaster_user_id: the id of the user you want to listen to
         :param callback: function for callback
         :raises ~twitchAPI.types.EventSubSubscriptionConflict: if a conflict was found with this subscription
             (e.g. already subscribed to this exact topic)
         :raises ~twitchAPI.types.EventSubSubscriptionTimeout: if :code:`wait_for_subscription_confirm`
             is true and the subscription was not fully confirmed in time
         :raises ~twitchAPI.types.EventSubSubscriptionError: if the subscription failed (see error message for details)
         :raises ~twitchAPI.types.TwitchBackendException: if the subscription failed due to a twitch backend error
         """
         return await self._subscribe('channel.follow', '1', {'broadcaster_user_id': broadcaster_user_id}, callback)
 
+    async def listen_channel_follow_v2(self,
+                                       broadcaster_user_id: str,
+                                       moderator_user_id: str,
+                                       callback: CALLBACK_TYPE) -> str:
+        """A specified channel receives a follow.
+
+        User Authentication with :code:`~twitchAPI.types.AuthScope.MODERATOR_READ_FOLLOWERS` is required.
+
+        For more information see here: https://dev.twitch.tv/docs/eventsub/eventsub-subscription-types#channelfollow
+
+        :param broadcaster_user_id: the id of the user you want to listen to
+        :param moderator_user_id: The ID of the moderator of the channel you want to get follow notifications for.
+        :param callback: function for callback
+        :raises ~twitchAPI.types.EventSubSubscriptionConflict: if a conflict was found with this subscription
+            (e.g. already subscribed to this exact topic)
+        :raises ~twitchAPI.types.EventSubSubscriptionTimeout: if :code:`wait_for_subscription_confirm`
+            is true and the subscription was not fully confirmed in time
+        :raises ~twitchAPI.types.EventSubSubscriptionError: if the subscription failed (see error message for details)
+        :raises ~twitchAPI.types.TwitchBackendException: if the subscription failed due to a twitch backend error
+        """
+        return await self._subscribe('channel.follow',
+                                     '2',
+                                     {'broadcaster_user_id': broadcaster_user_id, 'moderator_user_id': moderator_user_id},
+                                     callback)
+
     async def listen_channel_subscribe(self, broadcaster_user_id: str, callback: CALLBACK_TYPE) -> str:
         """A notification when a specified channel receives a subscriber. This does not include resubscribes.
 
         For more information see here: https://dev.twitch.tv/docs/eventsub/eventsub-subscription-types#channelsubscribe
 
         :param broadcaster_user_id: the id of the user you want to listen to
         :param callback: function for callback
@@ -647,15 +677,16 @@
 
     async def listen_channel_points_custom_reward_redemption_add(self,
                                                                  broadcaster_user_id: str,
                                                                  callback: CALLBACK_TYPE,
                                                                  reward_id: Optional[str] = None) -> str:
         """A viewer has redeemed a custom channel points reward on the specified channel.
 
-        For more information see here: https://dev.twitch.tv/docs/eventsub/eventsub-subscription-types#channelchannel_points_custom_reward_redemptionadd
+        For more information see here:
+        https://dev.twitch.tv/docs/eventsub/eventsub-subscription-types#channelchannel_points_custom_reward_redemptionadd
 
         :param broadcaster_user_id: the id of the user you want to listen to
         :param reward_id: the id of the reward you want to get updates from. |default| :code:`None`
         :param callback: function for callback
         :raises ~twitchAPI.types.EventSubSubscriptionConflict: if a conflict was found with this subscription
             (e.g. already subscribed to this exact topic)
         :raises ~twitchAPI.types.EventSubSubscriptionTimeout: if :code:`wait_for_subscription_confirm`
@@ -672,15 +703,16 @@
 
     async def listen_channel_points_custom_reward_redemption_update(self,
                                                                     broadcaster_user_id: str,
                                                                     callback: CALLBACK_TYPE,
                                                                     reward_id: Optional[str] = None) -> str:
         """A redemption of a channel points custom reward has been updated for the specified channel.
 
-        For more information see here: https://dev.twitch.tv/docs/eventsub/eventsub-subscription-types#channelchannel_points_custom_reward_redemptionupdate
+        For more information see here:
+        https://dev.twitch.tv/docs/eventsub/eventsub-subscription-types#channelchannel_points_custom_reward_redemptionupdate
 
         :param broadcaster_user_id: the id of the user you want to listen to
         :param reward_id: the id of the reward you want to get updates from. |default| :code:`None`
         :param callback: function for callback
         :raises ~twitchAPI.types.EventSubSubscriptionConflict: if a conflict was found with this subscription
             (e.g. already subscribed to this exact topic)
         :raises ~twitchAPI.types.EventSubSubscriptionTimeout: if :code:`wait_for_subscription_confirm`
@@ -1032,16 +1064,16 @@
 
     async def listen_channel_shield_mode_begin(self,
                                                broadcaster_user_id: str,
                                                moderator_user_id: str,
                                                callback: CALLBACK_TYPE) -> str:
         """Sends a notification when the broadcaster activates Shield Mode.
 
-        Requires the :const:`~twitchAPI.types.AuthScope.MODERATOR_READ_SHIELD_MODE` or :const:`~twitchAPI.types.AuthScope.MODERATOR_MANAGE_SHIELD_MODE`
-        auth scope.
+        Requires the :const:`~twitchAPI.types.AuthScope.MODERATOR_READ_SHIELD_MODE` or
+        :const:`~twitchAPI.types.AuthScope.MODERATOR_MANAGE_SHIELD_MODE` auth scope.
 
         For more information see here: https://dev.twitch.tv/docs/eventsub/eventsub-subscription-types/#channelshield_modebegin
 
         :param broadcaster_user_id: The ID of the broadcaster that you want to receive notifications about when they activate Shield Mode.
         :param moderator_user_id: The ID of the broadcaster or one of the broadcaster’s moderators.
         :param callback: function for callback
         :raises ~twitchAPI.types.EventSubSubscriptionConflict: if a conflict was found with this subscription
@@ -1059,16 +1091,16 @@
 
     async def listen_channel_shield_mode_end(self,
                                              broadcaster_user_id: str,
                                              moderator_user_id: str,
                                              callback: CALLBACK_TYPE) -> str:
         """Sends a notification when the broadcaster deactivates Shield Mode.
 
-        Requires the :const:`~twitchAPI.types.AuthScope.MODERATOR_READ_SHIELD_MODE` or :const:`~twitchAPI.types.AuthScope.MODERATOR_MANAGE_SHIELD_MODE`
-        auth scope.
+        Requires the :const:`~twitchAPI.types.AuthScope.MODERATOR_READ_SHIELD_MODE` or
+        :const:`~twitchAPI.types.AuthScope.MODERATOR_MANAGE_SHIELD_MODE` auth scope.
 
         For more information see here: https://dev.twitch.tv/docs/eventsub/eventsub-subscription-types/#channelshield_modeend
 
         :param broadcaster_user_id: The ID of the broadcaster that you want to receive notifications about when they deactivate Shield Mode.
         :param moderator_user_id: The ID of the broadcaster or one of the broadcaster’s moderators.
         :param callback: function for callback
         :raises ~twitchAPI.types.EventSubSubscriptionConflict: if a conflict was found with this subscription
```

### Comparing `twitchAPI-3.8.0/twitchAPI/helper.py` & `twitchAPI-3.9.0/twitchAPI/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,36 +98,36 @@
     :param data: dict or list
     :param fields: list of keys to be replaced
     :param _enum: Type of Enum to be replaced
     :param default: The default value if _enum does not contain the field value
     """
     _enum_vals = [e.value for e in _enum.__members__.values()]
 
-    def make_dict_field_enum(data: dict,
-                             fields: List[str],
+    def make_dict_field_enum(_data: dict,
+                             _fields: List[str],
                              _enum: Type[Enum],
-                             default: Optional[Enum]) -> Union[dict, Enum, None]:
-        fd = data
-        if isinstance(data, str):
-            if data not in _enum_vals:
-                return default
+                             _default: Optional[Enum]) -> Union[dict, Enum, None]:
+        fd = _data
+        if isinstance(_data, str):
+            if _data not in _enum_vals:
+                return _default
             else:
-                return _enum(data)
-        for key, value in data.items():
+                return _enum(_data)
+        for key, value in _data.items():
             # TODO fix for non string values
             if isinstance(value, str):
                 if key in fields:
                     if value not in _enum_vals:
-                        fd[key] = default
+                        fd[key] = _default
                     else:
                         fd[key] = _enum(value)
             elif isinstance(value, dict):
-                fd[key] = make_dict_field_enum(value, fields, _enum, default)
+                fd[key] = make_dict_field_enum(value, _fields, _enum, _default)
             elif isinstance(value, list):
-                fd[key] = fields_to_enum(value, fields, _enum, default)
+                fd[key] = fields_to_enum(value, _fields, _enum, _default)
         return fd
 
     if isinstance(data, list):
         return [make_dict_field_enum(d, fields, _enum, default) for d in data]
     else:
         return make_dict_field_enum(data, fields, _enum, default)
```

### Comparing `twitchAPI-3.8.0/twitchAPI/oauth.py` & `twitchAPI-3.9.0/twitchAPI/oauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 from .helper import build_url, build_scope, get_uuid, TWITCH_AUTH_BASE_URL, fields_to_enum
 from .types import AuthScope, InvalidRefreshTokenException, UnauthorizedException, TwitchAPIException
 from typing import Optional, Callable
 import webbrowser
 from aiohttp import web
 import asyncio
 from threading import Thread
-from concurrent.futures._base import CancelledError
+from concurrent.futures import CancelledError
 from logging import getLogger, Logger
 
 from typing import List, Union
 
 __all__ = ['refresh_access_token', 'validate_token', 'get_user_info', 'revoke_token', 'UserAuthenticator']
```

### Comparing `twitchAPI-3.8.0/twitchAPI/object.py` & `twitchAPI-3.9.0/twitchAPI/object.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,29 @@
 
 from twitchAPI.helper import build_url
 from twitchAPI.types import StatusCode, VideoType, HypeTrainContributionMethod, DropsEntitlementFulfillmentStatus, CustomRewardRedemptionStatus, \
     PollStatus, PredictionStatus, SoundtrackSourceType
 
 T = TypeVar('T')
 
+__all__ = ['TwitchObject', 'IterTwitchObject', 'AsyncIterTwitchObject', 'TwitchUser', 'TwitchUserFollow', 'TwitchUserFollowResult', 'DateRange',
+           'ExtensionAnalytic', 'GameAnalytics', 'CreatorGoal', 'BitsLeaderboardEntry', 'BitsLeaderboard', 'ProductCost', 'ProductData',
+           'ExtensionTransaction', 'ChatSettings', 'CreatedClip', 'Clip', 'CodeStatus', 'Game', 'AutoModStatus', 'BannedUser', 'BanUserResponse',
+           'BlockedTerm', 'Moderator', 'CreateStreamMarkerResponse', 'Stream', 'StreamMarker', 'StreamMarkers', 'GetStreamMarkerResponse',
+           'BroadcasterSubscription', 'BroadcasterSubscriptions', 'UserSubscription', 'StreamTag', 'TeamUser', 'ChannelTeam', 'UserExtension',
+           'ActiveUserExtension', 'UserActiveExtensions', 'VideoMutedSegments', 'Video', 'ChannelInformation', 'SearchChannelResult',
+           'SearchCategoryResult', 'StartCommercialResult', 'Cheermote', 'GetCheermotesResponse', 'HypeTrainContribution', 'HypeTrainEventData',
+           'HypeTrainEvent', 'DropsEntitlement', 'MaxPerStreamSetting', 'MaxPerUserPerStreamSetting', 'GlobalCooldownSetting', 'CustomReward',
+           'PartialCustomReward', 'CustomRewardRedemption', 'ChannelEditor', 'BlockListEntry', 'PollChoice', 'Poll', 'Predictor', 'PredictionOutcome',
+           'Prediction', 'RaidStartResult', 'ChatBadgeVersion', 'ChatBadge', 'Emote', 'GetEmotesResponse', 'EventSubSubscription',
+           'GetEventSubSubscriptionResult', 'StreamCategory', 'ChannelStreamScheduleSegment', 'StreamVacation', 'ChannelStreamSchedule',
+           'ChannelVIP', 'UserChatColor', 'Artist', 'Album', 'Soundtrack', 'TrackSource', 'CurrentSoundtrack', 'Playlist', 'Chatter',
+           'GetChattersResponse', 'ShieldModeStatus', 'CharityAmount', 'CharityCampaign', 'CharityCampaignDonation', 'AutoModSettings',
+           'ChannelFollower', 'ChannelFollowersResult', 'FollowedChannel', 'FollowedChannelsResult']
+
 
 class TwitchObject:
     """
     A lot of API calls return a child of this in some way (either directly or via generator).
     You can always use the :const:`~twitchAPI.object.TwitchObject.to_dict()` method to turn that object to a dictionary.
 
     Example:
@@ -167,18 +182,15 @@
             self.__idx += 1
             return data[self.__idx - 1]
         # make request
         if self._data['param']['after'] is None:
             raise StopAsyncIteration()
         _url = build_url(self._data['url'], self._data['param'], remove_none=True, split_lists=self._data['split'])
         async with ClientSession() as session:
-            if self._data['body'] is None:
-                response = await self._data['req'](session, _url, self._data['auth_t'], self._data['auth_s'])
-            else:
-                response = await self._data['req'](session, _url, self._data['auth_t'], self._data['auth_s'], body=self._data['body'])
+            response = await self._data['req'](session, _url, self._data['auth_t'], self._data['auth_s'], self._data['body'])
             _data = await response.json()
         _after = _data.get('pagination', {}).get('cursor')
         self._data['param']['after'] = _after
         if self._data['in_data']:
             _data = _data['data']
         # refill data
         merged_annotations = self._get_annotations()
@@ -218,14 +230,38 @@
 
 
 class TwitchUserFollowResult(AsyncIterTwitchObject[TwitchUserFollow]):
     total: int
     data: List[TwitchUserFollow]
 
 
+class ChannelFollower(TwitchObject):
+    followed_at: datetime
+    user_id: str
+    user_name: str
+    user_login: str
+
+
+class ChannelFollowersResult(AsyncIterTwitchObject[ChannelFollower]):
+    total: int
+    data: List[ChannelFollower]
+
+
+class FollowedChannel(TwitchObject):
+    broadcaster_id: str
+    broadcaster_login: str
+    broadcaster_name: str
+    followed_at: datetime
+
+
+class FollowedChannelsResult(AsyncIterTwitchObject[FollowedChannel]):
+    total: int
+    data: List[FollowedChannel]
+
+
 class DateRange(TwitchObject):
     ended_at: datetime
     started_at: datetime
 
 
 class ExtensionAnalytic(TwitchObject):
     extension_id: str
```

### Comparing `twitchAPI-3.8.0/twitchAPI/pubsub.py` & `twitchAPI-3.9.0/twitchAPI/pubsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 import json
 from random import randrange
 import datetime
 from logging import getLogger, Logger
 from uuid import UUID
 from time import sleep
 
-from typing import Callable, List, Dict, Awaitable
+from typing import Callable, List, Dict, Awaitable, Optional
 
 __all__ = ['PubSub']
 
 
 CALLBACK_FUNC = Callable[[UUID, dict], Awaitable[None]]
 
 
@@ -104,15 +104,15 @@
            This should never be shorter than 12 + `ping_jitter` seconds to avoid problems with the pong timeout. |default| :code:`120`"""
         self.ping_jitter: int = 4
         """time in seconds added or subtracted from `ping_frequency`. You probably don't want to change this. |default| :code:`4`"""
         self.listen_confirm_timeout: int = 30
         """maximum time in seconds waited for a listen confirm. |default| :code:`30`"""
         self.reconnect_delay_steps: List[int] = [1, 2, 4, 8, 16, 32, 64, 128]
         self.__connection = None
-        self.__socket_thread: threading.Thread = None
+        self.__socket_thread: Optional[threading.Thread] = None
         self.__running: bool = False
         self.__socket_loop = None
         self.__topics: dict = {}
         self._session = None
         self.__startup_complete: bool = False
         self.__tasks = None
         self.__waiting_for_pong: bool = False
@@ -322,18 +322,20 @@
         except CancelledError:
             return
 
 ###########################################################################################
 # Handler
 ###########################################################################################
 
+    # noinspection PyUnusedLocal
     async def __handle_pong(self, data):
         self.__waiting_for_pong = False
         self.logger.debug('received pong')
 
+    # noinspection PyUnusedLocal
     async def __handle_reconnect(self, data):
         self.logger.info('received reconnect command, reconnecting now...')
         await self.__connect()
 
     async def __handle_response(self, data):
         error = make_enum(data.get('error'),
                           PubSubResponseError,
```

### Comparing `twitchAPI-3.8.0/twitchAPI/twitch.py` & `twitchAPI-3.9.0/twitchAPI/twitch.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,17 +89,18 @@
         print(segment.title)
 
 
 AsyncGenerator
 ==============
 
 AsyncGenerators are used to automatically itterate over all possible resuts of your API call, this will also automatically handle pagination for you.
-In some cases (for example stream schedules with repeating entries), this may result in a endless stream of entries returned so make sure to add your own
-exit conditions in such cases.
-The generated objects will always be children of :py:const:`~twitchAPI.object.TwitchObject`, see the docs of the API call to see the exact object type.
+In some cases (for example stream schedules with repeating entries), this may result in a endless stream of entries returned so make sure to add your
+own exit conditions in such cases.
+The generated objects will always be children of :py:const:`~twitchAPI.object.TwitchObject`, see the docs of the API call to see the exact
+object type.
 
 Example:
 
 .. code-block:: python
 
     async for tag in twitch.get_all_stream_tags():
         print(tag.tag_id)
@@ -195,19 +196,20 @@
     twitch.user_auth_refresh_callback = user_refresh
 
 *******************
 Class Documentation
 *******************
 """
 import asyncio
-
 import aiohttp.helpers
+from datetime import datetime
 from aiohttp import ClientSession, ClientResponse
 from aiohttp.client import ClientTimeout
-from .helper import TWITCH_API_BASE_URL, TWITCH_AUTH_BASE_URL, build_scope, enum_value_or_none, datetime_to_str, remove_none_values, ResultType
+from .helper import TWITCH_API_BASE_URL, TWITCH_AUTH_BASE_URL, build_scope, enum_value_or_none, datetime_to_str, remove_none_values, ResultType, \
+    build_url
 from logging import getLogger, Logger
 from .object import *
 from .types import *
 from typing import Union, List, Optional, Callable, AsyncGenerator, TypeVar, Dict, Awaitable
 
 __all__ = ['Twitch']
 T = TypeVar('T')
@@ -254,22 +256,30 @@
         """If set to true, auto refresh the auth token once it expires. |default| :code:`True`"""
         self._authenticate_app = authenticate_app
         self._target_app_scope = target_app_auth_scope
         self.base_url: str = base_url
         """The URL to the Twitch API used"""
         self._user_token_refresh_lock: bool = False
         self._app_token_refresh_lock: bool = False
+        self._r_lookup: Dict[str, Callable] = {
+            'get': self.__api_get_request,
+            'post': self.__api_post_request,
+            'delete': self.__api_delete_request,
+            'patch': self.__api_patch_request,
+            'put': self.__api_put_request
+        }
 
     def __await__(self):
         if self._authenticate_app:
             t = asyncio.create_task(self.authenticate_app(self._target_app_scope if self._target_app_scope is not None else []))
             yield from t
         return self
 
-    async def close(self):
+    @staticmethod
+    async def close():
         """Gracefully close the connection to the Twitch API"""
         # ensure that asyncio actually gracefully shut down
         await asyncio.sleep(0.25)
 
     def __generate_header(self, auth_type: 'AuthType', required_scope: List[Union[AuthScope, List[AuthScope]]]) -> dict:
         header = {"Client-ID": self.app_id}
         if auth_type == AuthType.EITHER:
@@ -370,37 +380,30 @@
                 if self.app_auth_refresh_callback is not None:
                     await self.app_auth_refresh_callback(self.__app_auth_token)
 
     async def __check_request_return(self,
                                      session: ClientSession,
                                      response: ClientResponse,
                                      retry_func: Callable,
-                                     reply_func_has_data: bool,
                                      url: str,
                                      auth_type: 'AuthType',
                                      required_scope: List[AuthScope],
                                      data: Optional[dict] = None,
                                      retries: int = 1
                                      ) -> ClientResponse:
         if self.auto_refresh_auth and retries > 0:
             if response.status == 401:
                 # unauthorized, lets try to refresh the token once
                 self.logger.debug('got 401 response -> try to refresh token')
                 await self.refresh_used_token()
-                if reply_func_has_data:
-                    return await retry_func(session, url, auth_type, required_scope, data=data, retries=retries - 1)
-                else:
-                    return await retry_func(session, url, auth_type, required_scope, retries=retries - 1)
+                return await retry_func(session, url, auth_type, required_scope, data=data, retries=retries - 1)
             elif response.status == 503:
                 # service unavailable, retry exactly once as recommended by twitch documentation
                 self.logger.debug('got 503 response -> retry once')
-                if reply_func_has_data:
-                    return await retry_func(session, url, auth_type, required_scope, data=data, retries=retries - 1)
-                else:
-                    return await retry_func(session, url, auth_type, required_scope, retries=retries - 1)
+                return await retry_func(session, url, auth_type, required_scope, data=data, retries=retries - 1)
         elif self.auto_refresh_auth and retries <= 0:
             if response.status == 503:
                 raise TwitchBackendException('The Twitch API returns a server error')
             if response.status == 401:
                 msg = (await response.json()).get('message', '')
                 self.logger.debug(f'got 401 response and can\'t refresh. Message: "{msg}"')
                 raise UnauthorizedException(msg)
@@ -429,108 +432,87 @@
                                  auth_type: 'AuthType',
                                  required_scope: List[Union[AuthScope, List[AuthScope]]],
                                  data: Optional[dict] = None,
                                  retries: int = 1) -> ClientResponse:
         """Make POST request with authorization"""
         headers = self.__generate_header(auth_type, required_scope)
         self.logger.debug(f'making POST request to {url}')
-        if data is None:
-            req = await session.post(url, headers=headers)
-        else:
-            req = await session.post(url, headers=headers, json=data)
-        return await self.__check_request_return(session, req, self.__api_post_request, True, url, auth_type, required_scope, data, retries)
+        req = await session.post(url, headers=headers, json=data)
+        return await self.__check_request_return(session, req, self.__api_post_request, url, auth_type, required_scope, data, retries)
 
     async def __api_put_request(self,
                                 session: ClientSession,
                                 url: str,
                                 auth_type: 'AuthType',
                                 required_scope: List[Union[AuthScope, List[AuthScope]]],
                                 data: Optional[dict] = None,
                                 retries: int = 1) -> ClientResponse:
         """Make PUT request with authorization"""
         headers = self.__generate_header(auth_type, required_scope)
         self.logger.debug(f'making PUT request to {url}')
-        if data is None:
-            req = await session.put(url, headers=headers)
-        else:
-            req = await session.put(url, headers=headers, json=data)
-        return await self.__check_request_return(session, req, self.__api_put_request, True, url, auth_type, required_scope, data, retries)
+        req = await session.put(url, headers=headers, json=data)
+        return await self.__check_request_return(session, req, self.__api_put_request, url, auth_type, required_scope, data, retries)
 
     async def __api_patch_request(self,
                                   session: ClientSession,
                                   url: str,
                                   auth_type: 'AuthType',
                                   required_scope: List[Union[AuthScope, List[AuthScope]]],
                                   data: Optional[dict] = None,
                                   retries: int = 1) -> ClientResponse:
         """Make PATCH request with authorization"""
         headers = self.__generate_header(auth_type, required_scope)
         self.logger.debug(f'making PATCH request to {url}')
-        if data is None:
-            req = await session.patch(url, headers=headers)
-        else:
-            req = await session.patch(url, headers=headers, json=data)
-        return await self.__check_request_return(session, req, self.__api_patch_request, True, url, auth_type, required_scope, data, retries)
+        req = await session.patch(url, headers=headers, json=data)
+        return await self.__check_request_return(session, req, self.__api_patch_request, url, auth_type, required_scope, data, retries)
 
     async def __api_delete_request(self,
                                    session: ClientSession,
                                    url: str,
                                    auth_type: 'AuthType',
                                    required_scope: List[Union[AuthScope, List[AuthScope]]],
                                    data: Optional[dict] = None,
                                    retries: int = 1) -> ClientResponse:
         """Make DELETE request with authorization"""
         headers = self.__generate_header(auth_type, required_scope)
         self.logger.debug(f'making DELETE request to {url}')
-        if data is None:
-            req = await session.delete(url, headers=headers)
-        else:
-            req = await session.delete(url, headers=headers, json=data)
-        return await self.__check_request_return(session, req, self.__api_delete_request, True, url, auth_type, required_scope, data, retries)
+        req = await session.delete(url, headers=headers, json=data)
+        return await self.__check_request_return(session, req, self.__api_delete_request, url, auth_type, required_scope, data, retries)
 
     async def __api_get_request(self,
                                 session: ClientSession,
                                 url: str,
                                 auth_type: 'AuthType',
                                 required_scope: List[Union[AuthScope, List[AuthScope]]],
-                                retries: int = 1) -> [ClientResponse, ClientSession]:
+                                data: Optional[dict] = None,
+                                retries: int = 1) -> ClientResponse:
         """Make GET request with authorization"""
         headers = self.__generate_header(auth_type, required_scope)
         self.logger.debug(f'making GET request to {url}')
-        req = await session.get(url, headers=headers)
-        return await self.__check_request_return(session, req, self.__api_get_request, False, url, auth_type, required_scope, None, retries)
+        req = await session.get(url, headers=headers, json=data)
+        return await self.__check_request_return(session, req, self.__api_get_request, url, auth_type, required_scope, data, retries)
 
     async def _build_generator(self,
                                req,
                                url: str,
                                url_params: dict,
                                auth_type: AuthType,
                                auth_scope: List[Union[AuthScope, List[AuthScope]]],
                                return_type: T,
                                body_data: Optional[dict] = None,
                                split_lists: bool = False,
                                error_handler: Optional[Dict[int, BaseException]] = None) -> AsyncGenerator[T, None]:
-        r_lookup: Dict[str, Callable] = {
-            'get': self.__api_get_request,
-            'post': self.__api_post_request,
-            'delete': self.__api_delete_request,
-            'patch': self.__api_patch_request,
-            'put': self.__api_put_request
-        }
-        req = r_lookup.get(req.lower())
+        req = self._r_lookup.get(req.lower())
         _after = url_params.get('after')
         _first = True
         async with ClientSession(timeout=self.session_timeout) as session:
             while _first or _after is not None:
                 url_params['after'] = _after
                 _url = build_url(self.base_url + url, url_params, remove_none=True, split_lists=split_lists)
-                if body_data is None:
-                    response = await req(session, _url, auth_type, auth_scope)
-                else:
-                    response = await req(session, _url, auth_type, auth_scope, data=body_data)
+                response = await req(session, _url, auth_type, auth_scope, data=body_data)
                 if error_handler is not None:
                     if response.status in error_handler.keys():
                         raise error_handler[response.status]
                 data = await response.json()
                 for entry in data.get('data', []):
                     yield return_type(**entry)
                 _after = data.get('pagination', {}).get('cursor')
@@ -543,28 +525,18 @@
                                  auth_type: AuthType,
                                  auth_scope: List[Union[AuthScope, List[AuthScope]]],
                                  return_type: T,
                                  body_data: Optional[dict] = None,
                                  split_lists: bool = False,
                                  iter_field: str = 'data',
                                  in_data: bool = False):
-        r_lookup: Dict[str, Callable] = {
-            'get': self.__api_get_request,
-            'post': self.__api_post_request,
-            'delete': self.__api_delete_request,
-            'patch': self.__api_patch_request,
-            'put': self.__api_put_request
-        }
-        req = r_lookup.get(req.lower())
+        req = self._r_lookup.get(req.lower())
         _url = build_url(self.base_url + url, url_params, remove_none=True, split_lists=split_lists)
         async with ClientSession(timeout=self.session_timeout) as session:
-            if body_data is None:
-                response = await req(session, _url, auth_type, auth_scope)
-            else:
-                response = await req(session, _url, auth_type, auth_scope, data=body_data)
+            response = await req(session, _url, auth_type, auth_scope, data=body_data)
             data = await response.json()
         url_params['after'] = data.get('pagination', {}).get('cursor')
         if in_data:
             data = data['data']
         cont_data = {
             'req': req,
             'url': self.base_url + url,
@@ -586,28 +558,18 @@
                             auth_scope: List[Union[AuthScope, List[AuthScope]]],
                             return_type: T,
                             body_data: Optional[dict] = None,
                             split_lists: bool = False,
                             get_from_data: bool = True,
                             result_type: ResultType = ResultType.RETURN_TYPE,
                             error_handler: Optional[Dict[int, BaseException]] = None):
-        r_lookup: Dict[str, Callable] = {
-            'get': self.__api_get_request,
-            'post': self.__api_post_request,
-            'delete': self.__api_delete_request,
-            'patch': self.__api_patch_request,
-            'put': self.__api_put_request
-        }
         async with ClientSession(timeout=self.session_timeout) as session:
-            req = r_lookup.get(req.lower())
+            req = self._r_lookup.get(req.lower())
             _url = build_url(self.base_url + url, url_params, remove_none=True, split_lists=split_lists)
-            if body_data is None:
-                response = await req(session, _url, auth_type, auth_scope)
-            else:
-                response = await req(session, _url, auth_type, auth_scope, data=body_data)
+            response = await req(session, _url, auth_type, auth_scope, data=body_data)
             if error_handler is not None:
                 if response.status in error_handler.keys():
                     raise error_handler[response.status]
             if result_type == ResultType.STATUS_CODE:
                 return response.status
             if result_type == ResultType.TEXT:
                 return await response.text()
@@ -724,14 +686,27 @@
     def get_user_auth_token(self) -> Union[str, None]:
         """Returns the current user auth token, None if no user Authentication is set
 
         :return: current user auth token
         """
         return self.__user_auth_token
 
+    async def get_refreshed_user_auth_token(self) -> Union[str, None]:
+        """Validates the current set user auth token and returns it
+
+        Will reauth if token is invalid"""
+        if self.__user_auth_token is None:
+            return None
+        from .oauth import validate_token
+        val_result = await validate_token(self.__user_auth_token)
+        if val_result.get('status', 200) != 200:
+            # refresh token
+            await self.refresh_used_token()
+        return self.__user_auth_token
+
     def get_used_token(self) -> Union[str, None]:
         """Returns the currently used token, can be either the app or user auth Token or None if no auth is set
 
         :return: the currently used auth token or None if no Authentication is set
         """
         # if no auth is set, self.__app_auth_token will be None
         return self.__user_auth_token if self.__has_user_auth else self.__app_auth_token
@@ -1574,15 +1549,16 @@
         :param before: Cursor for backward pagination |default| :code:`None`
         :param first: Maximum number of objects to return. Maximum: 100. |default| :code:`20`
         :param game_id: Returns streams broadcasting a specified game ID. You can specify up to 100 IDs. |default| :code:`None`
         :param language: Stream language. You can specify up to 100 languages. |default| :code:`None`
         :param user_id: Returns streams broadcast by one or more specified user IDs. You can specify up to 100 IDs. |default| :code:`None`
         :param user_login: Returns streams broadcast by one or more specified user login names.
                         You can specify up to 100 names. |default| :code:`None`
-        :param stream_type: The type of stream to filter the list of streams by. Possible values are :code:`all` and :code:`live` |default| :code:`None`
+        :param stream_type: The type of stream to filter the list of streams by. Possible values are :code:`all` and :code:`live`
+                        |default| :code:`None`
         :raises ~twitchAPI.types.TwitchAPIException: if the request was malformed
         :raises ~twitchAPI.types.UnauthorizedException: if app authentication is not set or invalid
         :raises ~twitchAPI.types.TwitchAuthorizationException: if the used authentication token became invalid and a re authentication failed
         :raises ~twitchAPI.types.TwitchBackendException: if the Twitch API itself runs into problems
         :raises ValueError: if first is not in range 1 to 100 or one of the following fields have more than 100 entries:
                         `user_id, game_id, language, user_login`
         """
@@ -1890,14 +1866,84 @@
             'after': after,
             'first': first,
             'from_id': from_id,
             'to_id': to_id
         }
         return await self._build_iter_result('GET', 'users/follows', param, AuthType.EITHER, [], TwitchUserFollowResult)
 
+    async def get_channel_followers(self,
+                                    broadcaster_id: str,
+                                    user_id: Optional[str] = None,
+                                    first: Optional[int] = None,
+                                    after: Optional[str] = None) -> ChannelFollowersResult:
+        """ Gets a list of users that follow the specified broadcaster.
+        You can also use this endpoint to see whether a specific user follows the broadcaster.
+
+        Requires User Authentication with :const:`~twitchAPI.types.AuthScope.MODERATOR_READ_FOLLOWERS`\n
+        For detailed documentation, see here: https://dev.twitch.tv/docs/api/reference#get-channel-followers
+
+        :param broadcaster_id: The broadcaster’s ID. Returns the list of users that follow this broadcaster.
+        :param user_id: A user’s ID. Use this parameter to see whether the user follows this broadcaster.
+            If specified, the response contains this user if they follow the broadcaster.
+            If not specified, the response contains all users that follow the broadcaster. |default|:code:`None`
+        :param first: The maximum number of items to return per page in the response. Minimum 1, Maximum 100 |default| :code:`20`
+        :param after: The cursor used to get the next page of results.
+        :raises ~twitchAPI.types.TwitchAPIException: if the request was malformed
+        :raises ~twitchAPI.types.UnauthorizedException: if user authentication is not set or invalid
+        :raises ~twitchAPI.types.MissingScopeException: if the user authentication is missing the required scope
+        :raises ~twitchAPI.types.TwitchAuthorizationException: if the used authentication token became invalid and a re authentication failed
+        :raises ~twitchAPI.types.TwitchBackendException: if the Twitch API itself runs into problems
+        :raises ~twitchAPI.types.TwitchAPIException: if a Query Parameter is missing or invalid
+        :raises ValueError: if first is not in range 1 to 100
+        """
+        if first is not None and (first < 1 or first > 100):
+            raise ValueError('first must be in range 1 to 100')
+        param = {
+            'broadcaster_id': broadcaster_id,
+            'user_id': user_id,
+            'first': first,
+            'after': after
+        }
+        return await self._build_iter_result('GET', 'channels/followers', param, AuthType.USER, [AuthScope.MODERATOR_READ_FOLLOWERS],
+                                             ChannelFollowersResult)
+
+    async def get_followed_channels(self,
+                                    user_id: str,
+                                    broadcaster_id: Optional[str] = None,
+                                    first: Optional[int] = None,
+                                    after: Optional[str] = None) -> FollowedChannelsResult:
+        """Gets a list of broadcasters that the specified user follows.
+        You can also use this endpoint to see whether a user follows a specific broadcaster.
+
+        Requires User Authentication with :const:`~twitchAPI.types.AuthScope.USER_READ_FOLLOWS`\n
+        For detailed documentation, see here: https://dev.twitch.tv/docs/api/reference#get-followed-channels
+
+        :param user_id: A user’s ID. Returns the list of broadcasters that this user follows. This ID must match the user ID in the user OAuth token.
+        :param broadcaster_id: A broadcaster’s ID. Use this parameter to see whether the user follows this broadcaster.
+            If specified, the response contains this broadcaster if the user follows them.
+            If not specified, the response contains all broadcasters that the user follows. |default| :code:`None`
+        :param first: The maximum number of items to return per page in the response. Minimum 1, Maximum 100 |default| :code:`20`
+        :param after: The cursor used to get the next page of results.
+        :raises ~twitchAPI.types.TwitchAPIException: if the request was malformed
+        :raises ~twitchAPI.types.UnauthorizedException: if user authentication is not set or invalid
+        :raises ~twitchAPI.types.MissingScopeException: if the user authentication is missing the required scope
+        :raises ~twitchAPI.types.TwitchAuthorizationException: if the used authentication token became invalid and a re authentication failed
+        :raises ~twitchAPI.types.TwitchBackendException: if the Twitch API itself runs into problems
+        :raises ~twitchAPI.types.TwitchAPIException: if a Query Parameter is missing or invalid
+        :raises ValueError: if first is not in range 1 to 100
+        """
+        if first is not None and (first < 1 or first > 100):
+            raise ValueError('first must be in range 1 to 100')
+        param = {
+            'user_id': user_id,
+            'broadcaster_id': broadcaster_id,
+            'first': first,
+            'after': after
+        }
+        return await self._build_iter_result('GET', 'channels/followed', param, AuthType.USER, [AuthScope.USER_READ_FOLLOWS], FollowedChannelsResult)
 
     async def update_user(self,
                           description: str) -> TwitchUser:
         """Updates the description of the Authenticated user.\n\n
 
         Requires User authentication with scope :const:`~twitchAPI.types.AuthScope.USER_EDIT`\n
         For detailed documentation, see here: https://dev.twitch.tv/docs/api/reference#update-user
@@ -2872,17 +2918,16 @@
         :raises ~twitchAPI.types.TwitchBackendException: if the Twitch API itself runs into problems
         :raises ~twitchAPI.types.TwitchAPIException: if a Query Parameter is missing or invalid
         :raises ValueError: if first is not in range 1 to 20
         :raises ValueError: if prediction_ids contains more than 100 entries
         """
         if first is not None and (first < 1 or first > 20):
             raise ValueError('first must be in range 1 to 20')
-        if prediction_ids is not None:
-            if len(prediction_ids) > 100:
-                raise ValueError('maximum of 100 prediction ids allowed')
+        if prediction_ids is not None and len(prediction_ids) > 100:
+            raise ValueError('maximum of 100 prediction ids allowed')
 
         param = {
             'broadcaster_id': broadcaster_id,
             'id': prediction_ids,
             'after': after,
             'first': first
         }
@@ -2919,16 +2964,15 @@
             raise ValueError('outcomes must have between 2 entries and 10 entries')
         body = {
             'broadcaster_id': broadcaster_id,
             'title': title,
             'outcomes': [{'title': x} for x in outcomes],
             'prediction_window': prediction_window
         }
-        return await self._build_result('POST', 'predictions', {}, AuthType.USER, [AuthScope.CHANNEL_MANAGE_PREDICTIONS], Prediction,
-                                        body_data=body)
+        return await self._build_result('POST', 'predictions', {}, AuthType.USER, [AuthScope.CHANNEL_MANAGE_PREDICTIONS], Prediction, body_data=body)
 
     async def end_prediction(self,
                              broadcaster_id: str,
                              prediction_id: str,
                              status: PredictionStatus,
                              winning_outcome_id: Optional[str] = None) -> Prediction:
         """Lock, resolve, or cancel a Channel Points Prediction.
@@ -2947,17 +2991,16 @@
         :raises ~twitchAPI.types.TwitchBackendException: if the Twitch API itself runs into problems
         :raises ~twitchAPI.types.TwitchAPIException: if a Query Parameter is missing or invalid
         :raises ValueError: if winning_outcome_id is None and status is RESOLVED
         :raises ValueError: if status is not one of RESOLVED, CANCELED or LOCKED
         """
         if status not in (PredictionStatus.RESOLVED, PredictionStatus.CANCELED, PredictionStatus.LOCKED):
             raise ValueError('status has to be one of RESOLVED, CANCELED or LOCKED')
-        if status == PredictionStatus.RESOLVED:
-            if winning_outcome_id is None:
-                raise ValueError('need to specify winning_outcome_id for status RESOLVED')
+        if status == PredictionStatus.RESOLVED and winning_outcome_id is None:
+            raise ValueError('need to specify winning_outcome_id for status RESOLVED')
         body = {
             'broadcaster_id': broadcaster_id,
             'id': prediction_id,
             'status': status.value
         }
         if winning_outcome_id is not None:
             body['winning_outcome_id'] = winning_outcome_id
```

### Comparing `twitchAPI-3.8.0/twitchAPI/types.py` & `twitchAPI-3.9.0/twitchAPI/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,18 @@
     USER_LEFT = 'user_left'
     """Triggered when a user leaves a chat channel"""
     MESSAGE_DELETE = 'message_delete'
     """Triggered when a message gets deleted from a channel"""
     CHAT_CLEARED = 'chat_cleared'
     """Triggered when a user was banned, timed out or all messaged from a user where deleted"""
     WHISPER = 'whisper'
-    """Triggered when someone whispers to your bot. NOTE: You need the :const:`~twitchAPI.types.AuthScope.WHISPERS_READ` Auth Scope to get this Event."""
+    """Triggered when someone whispers to your bot. NOTE: You need the :const:`~twitchAPI.types.AuthScope.WHISPERS_READ` Auth Scope
+    to get this Event."""
+    NOTICE = 'notice'
+    """Triggerd on server notice"""
 
 
 @dataclass
 class ChatRoom:
     name: str
     is_emote_only: bool
     is_subs_only: bool
```

### Comparing `twitchAPI-3.8.0/twitchAPI.egg-info/PKG-INFO` & `twitchAPI-3.9.0/twitchAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchAPI
-Version: 3.8.0
+Version: 3.9.0
 Summary: A Python 3.7+ implementation of the Twitch Helix API, PubSub, EventSub and Chat
 Home-page: https://github.com/Teekeks/pyTwitchAPI
 Author: Lena "Teekeks" During
 Author-email: info@teawork.de
 License: MIT
 Keywords: twitch,twitch.tv,chat,bot,event sub,EventSub,pub sub,PubSub,helix,api
 Classifier: Development Status :: 5 - Production/Stable
```

