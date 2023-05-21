# Comparing `tmp/qg-botsdk-2.7.0.tar.gz` & `tmp/qg-botsdk-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qg-botsdk-2.7.0.tar", last modified: Sat May 13 10:11:34 2023, max compression
+gzip compressed data, was "qg-botsdk-3.0.0.tar", last modified: Sun May 21 15:25:55 2023, max compression
```

## Comparing `qg-botsdk-2.7.0.tar` & `qg-botsdk-3.0.0.tar`

### file list

```diff
@@ -1,29 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 10:11:34.566653 qg-botsdk-2.7.0/
--rw-rw-rw-   0        0        0     1083 2022-05-05 08:39:00.000000 qg-botsdk-2.7.0/LICENSE
--rw-rw-rw-   0        0        0     7103 2023-05-13 10:11:34.566653 qg-botsdk-2.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     6740 2023-05-13 08:46:52.000000 qg-botsdk-2.7.0/README.md
--rw-rw-rw-   0        0        0     6556 2023-05-13 08:47:07.000000 qg-botsdk-2.7.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-13 10:11:34.559653 qg-botsdk-2.7.0/qg_botsdk/
--rw-rw-rw-   0        0        0      980 2023-03-30 14:45:13.000000 qg-botsdk-2.7.0/qg_botsdk/__init__.py
--rw-rw-rw-   0        0        0    23008 2023-05-13 09:58:12.000000 qg-botsdk-2.7.0/qg_botsdk/_api_model.py
--rw-rw-rw-   0        0        0      616 2023-02-05 14:08:39.000000 qg-botsdk-2.7.0/qg_botsdk/_queue.py
--rw-rw-rw-   0        0        0     1394 2023-01-05 02:29:18.000000 qg-botsdk-2.7.0/qg_botsdk/_statics.py
--rw-rw-rw-   0        0        0    13382 2023-02-26 07:33:31.000000 qg-botsdk-2.7.0/qg_botsdk/_utils.py
--rw-rw-rw-   0        0        0    47093 2023-05-13 10:04:40.000000 qg-botsdk-2.7.0/qg_botsdk/api.py
--rw-rw-rw-   0        0        0    73647 2023-05-13 10:04:03.000000 qg-botsdk-2.7.0/qg_botsdk/async_api.py
--rw-rw-rw-   0        0        0     5179 2023-02-26 11:45:25.000000 qg-botsdk-2.7.0/qg_botsdk/http.py
--rw-rw-rw-   0        0        0     6471 2023-01-14 05:41:49.000000 qg-botsdk-2.7.0/qg_botsdk/logger.py
--rw-rw-rw-   0        0        0    19717 2023-01-14 05:41:49.000000 qg-botsdk-2.7.0/qg_botsdk/model.py
--rw-rw-rw-   0        0        0     5522 2023-05-13 09:58:12.000000 qg-botsdk-2.7.0/qg_botsdk/plugins.py
--rw-rw-rw-   0        0        0    27014 2023-05-13 10:04:26.000000 qg-botsdk-2.7.0/qg_botsdk/qg_bot.py
--rw-rw-rw-   0        0        0    17604 2023-05-13 09:58:09.000000 qg-botsdk-2.7.0/qg_botsdk/qg_bot_ws.py
--rw-rw-rw-   0        0        0     1974 2023-01-14 05:41:49.000000 qg-botsdk-2.7.0/qg_botsdk/utils.py
--rw-rw-rw-   0        0        0       23 2023-05-13 10:09:25.000000 qg-botsdk-2.7.0/qg_botsdk/version.py
-drwxrwxrwx   0        0        0        0 2023-05-13 10:11:34.565665 qg-botsdk-2.7.0/qg_botsdk.egg-info/
--rw-rw-rw-   0        0        0     7103 2023-05-13 10:11:34.000000 qg-botsdk-2.7.0/qg_botsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-13 10:11:34.000000 qg-botsdk-2.7.0/qg_botsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 10:11:34.000000 qg-botsdk-2.7.0/qg_botsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-13 10:11:34.000000 qg-botsdk-2.7.0/qg_botsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-13 10:11:34.000000 qg-botsdk-2.7.0/qg_botsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      381 2023-05-13 10:11:34.567654 qg-botsdk-2.7.0/setup.cfg
--rw-rw-rw-   0        0        0      607 2023-05-13 10:11:18.000000 qg-botsdk-2.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:25:55.302856 qg-botsdk-3.0.0/
+-rw-rw-rw-   0        0        0     1083 2022-05-05 08:39:02.000000 qg-botsdk-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     7310 2023-05-21 15:25:55.302856 qg-botsdk-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6959 2023-05-14 14:33:12.000000 qg-botsdk-3.0.0/README.md
+-rw-rw-rw-   0        0        0     6763 2023-05-14 14:33:12.000000 qg-botsdk-3.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-21 15:25:55.283856 qg-botsdk-3.0.0/qg_botsdk/
+-rw-rw-rw-   0        0        0     1369 2023-05-21 14:48:31.000000 qg-botsdk-3.0.0/qg_botsdk/__init__.py
+-rw-rw-rw-   0        0        0    22958 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/_api_model.py
+-rw-rw-rw-   0        0        0      379 2023-05-21 14:48:29.000000 qg-botsdk-3.0.0/qg_botsdk/_exception.py
+-rw-rw-rw-   0        0        0      616 2023-02-05 14:08:40.000000 qg-botsdk-3.0.0/qg_botsdk/_queue.py
+-rw-rw-rw-   0        0        0    24671 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/_session.py
+-rw-rw-rw-   0        0        0     1465 2023-05-19 10:22:38.000000 qg-botsdk-3.0.0/qg_botsdk/_statics.py
+-rw-rw-rw-   0        0        0    15501 2023-05-21 15:23:06.000000 qg-botsdk-3.0.0/qg_botsdk/_utils.py
+-rw-rw-rw-   0        0        0    50456 2023-05-21 15:18:34.000000 qg-botsdk-3.0.0/qg_botsdk/api.py
+-rw-rw-rw-   0        0        0    77100 2023-05-21 15:18:34.000000 qg-botsdk-3.0.0/qg_botsdk/async_api.py
+-rw-rw-rw-   0        0        0     6023 2023-05-19 10:22:38.000000 qg-botsdk-3.0.0/qg_botsdk/http.py
+-rw-rw-rw-   0        0        0     6926 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/logger.py
+-rw-rw-rw-   0        0        0    25317 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/model.py
+-rw-rw-rw-   0        0        0     5282 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/plugins.py
+-rw-rw-rw-   0        0        0    29389 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/qg_bot.py
+-rw-rw-rw-   0        0        0    20262 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/qg_bot_ws.py
+-rw-rw-rw-   0        0        0     8524 2023-05-21 15:19:52.000000 qg-botsdk-3.0.0/qg_botsdk/session.py
+-rw-rw-rw-   0        0        0     2210 2023-05-19 10:22:41.000000 qg-botsdk-3.0.0/qg_botsdk/utils.py
+-rw-rw-rw-   0        0        0       23 2023-05-14 14:06:10.000000 qg-botsdk-3.0.0/qg_botsdk/version.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:25:55.289856 qg-botsdk-3.0.0/qg_botsdk.egg-info/
+-rw-rw-rw-   0        0        0     7310 2023-05-21 15:25:55.000000 qg-botsdk-3.0.0/qg_botsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2023-05-21 15:25:55.000000 qg-botsdk-3.0.0/qg_botsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 15:25:55.000000 qg-botsdk-3.0.0/qg_botsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-21 15:25:55.000000 qg-botsdk-3.0.0/qg_botsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-21 15:25:55.000000 qg-botsdk-3.0.0/qg_botsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      489 2023-05-21 15:25:55.303857 qg-botsdk-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      538 2023-05-13 10:50:24.000000 qg-botsdk-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:25:55.301859 qg-botsdk-3.0.0/test/
+-rw-rw-rw-   0        0        0        0 2023-05-14 02:41:18.000000 qg-botsdk-3.0.0/test/__init__.py
+-rw-rw-rw-   0        0        0     1705 2023-05-21 15:18:34.000000 qg-botsdk-3.0.0/test/_base_context.py
+-rw-rw-rw-   0        0        0      368 2023-05-19 10:22:38.000000 qg-botsdk-3.0.0/test/_testing_plugin.py
+-rw-rw-rw-   0        0        0      122 2023-05-19 10:22:38.000000 qg-botsdk-3.0.0/test/conftest.py
+-rw-rw-rw-   0        0        0     8133 2023-05-21 14:48:32.000000 qg-botsdk-3.0.0/test/test_api.py
+-rw-rw-rw-   0        0        0    16702 2023-05-21 15:22:40.000000 qg-botsdk-3.0.0/test/test_base.py
+-rw-rw-rw-   0        0        0    16503 2023-05-21 15:22:32.000000 qg-botsdk-3.0.0/test/test_run.py
+-rw-rw-rw-   0        0        0     8256 2023-05-21 15:01:02.000000 qg-botsdk-3.0.0/test/test_session.py
```

### Comparing `qg-botsdk-2.7.0/LICENSE` & `qg-botsdk-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qg-botsdk-2.7.0/PKG-INFO` & `qg-botsdk-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qg-botsdk
-Version: 2.7.0
+Version: 3.0.0
 Summary: easy-to-use SDK for Tencent QQ guild robot
 Home-page: https://github.com/GLGDLY/qg_botsdk
 Author: GDLY
 Author-email: tzlgdly@gmail.com
 Keywords: sample,example,setuptools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,14 +39,18 @@
 为此，qg_botsdk相应提供了另一个选择，这一款sdk虽然同样使用asyncio编写sdk底层，但其同时提供了threading和asyncio封装下的应用层调用，以抽象化封装的库编写方式，极大地降低应用层的开发难度。
 
 
 
 亮点
 =====
 
+-   两种应用层开发方式（threading、asyncio），可根据自己的喜好选择，而底层均为asyncio实现，保持高并发能力
+
+-   高覆盖率的单元测试，保证SDK的稳定性
+
 -   灵活的构建方式，即使官方删除或新增字段，SDK也不会规范于原来的数据格式，而会把真实数据反馈给你
 
 -   轻量，简洁，统一的代码结构，通过录入回调函数处理不同事件，10行即可构建一个简单的程序
 
 -   容易入门，无需学会asyncio、类继承等编程技巧也可使用，同时保留较高并发能力
 
 -   保留官方http API中Json数据的结构字段，带你学习官方结构，日后可自行开发适合自己的SDK
```

### Comparing `qg-botsdk-2.7.0/README.md` & `qg-botsdk-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 对于使用python进行频道官方机器人开发而言，市面上确实有不同的sdk可以选用，但其很多只提供异步asyncio+类继承的开发方式，对于不会相关技巧的朋友们，尤其新手，会有开发难度。
 
 为此，qg_botsdk相应提供了另一个选择，这一款sdk虽然同样使用asyncio编写sdk底层，但其同时提供了threading和asyncio封装下的应用层调用，以抽象化封装的库编写方式，极大地降低应用层的开发难度。 
 
 
 #### 亮点
 
+##### -   两种应用层开发方式（threading、asyncio），可根据自己的喜好选择，而底层均为asyncio实现，保持高并发能力
+
+##### -   高覆盖率的单元测试，保证SDK的稳定性
+
 ##### -   灵活的构建方式，即使官方删除或新增字段，SDK也不会规范于原来的数据格式，而会把真实数据反馈给你
 
 ##### -   轻量，简洁，统一的代码结构，通过录入回调函数处理不同事件，10行即可构建一个简单的程序
 
 ##### -   容易入门，无需学会asyncio、类继承等编程技巧也可使用，同时保留较高并发能力
 
 ##### -   保留官方http API中Json数据的结构字段，带你学习官方结构，日后可自行开发适合自己的SDK
```

### Comparing `qg-botsdk-2.7.0/README.rst` & `qg-botsdk-3.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 为此，qg_botsdk相应提供了另一个选择，这一款sdk虽然同样使用asyncio编写sdk底层，但其同时提供了threading和asyncio封装下的应用层调用，以抽象化封装的库编写方式，极大地降低应用层的开发难度。
 
 
 
 亮点
 =====
 
+-   两种应用层开发方式（threading、asyncio），可根据自己的喜好选择，而底层均为asyncio实现，保持高并发能力
+
+-   高覆盖率的单元测试，保证SDK的稳定性
+
 -   灵活的构建方式，即使官方删除或新增字段，SDK也不会规范于原来的数据格式，而会把真实数据反馈给你
 
 -   轻量，简洁，统一的代码结构，通过录入回调函数处理不同事件，10行即可构建一个简单的程序
 
 -   容易入门，无需学会asyncio、类继承等编程技巧也可使用，同时保留较高并发能力
 
 -   保留官方http API中Json数据的结构字段，带你学习官方结构，日后可自行开发适合自己的SDK
```

### Comparing `qg-botsdk-2.7.0/qg_botsdk/_api_model.py` & `qg-botsdk-3.0.0/qg_botsdk/_api_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from re import Pattern
-from typing import List, Optional, TypedDict
+from typing import Any, Callable, Dict, List, Optional
 
 from ._utils import object_class
-from .model import Model
+from .model import BotCommandObject, Model
 
 
-class Bot_Command_Obj(TypedDict, total=False):
-    command: list[str]
-    regex: Pattern
-    func: Model.MESSAGE
-    treat: bool
-    at: bool
-    short_circuit: bool
-    is_custom_short_circuit: bool
-    admin: bool
-    admin_error_msg: Optional[str]
+class WaifForCommandCallback:
+    def __init__(
+        self, command: BotCommandObject, callback: Callable[[Model.MESSAGE], Any]
+    ):
+        self.command = command
+        self.callback = callback
 
 
 apis = {
     ("获取用户ID", "get_bot_id"): [False, "此API不需要请求权限"],
     ("获取用户信息", "get_bot_info"): ["GET", "/users/@me"],
     ("获取用户频道列表", "get_bot_guilds"): ["GET", "/users/@me/guilds"],
     ("获取频道详情", "get_guild_info"): ["GET", "/guilds/{guild_id}"],
@@ -576,15 +571,15 @@
             id: str
             channel_id: str
             guild_id: str
             content: str
             timestamp: str
             tts: bool
             mention_everyone: bool
-            author: dict
+            author: Dict
             pinned: bool
             type: int
             flags: int
             seq_in_channel: str
             code: int
             message: str
```

### Comparing `qg-botsdk-2.7.0/qg_botsdk/_queue.py` & `qg-botsdk-3.0.0/qg_botsdk/_queue.py`

 * *Files identical despite different names*

### Comparing `qg-botsdk-2.7.0/qg_botsdk/_statics.py` & `qg-botsdk-3.0.0/qg_botsdk/_statics.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,7 +32,10 @@
         "OPEN_FORUM_REPLY_DELETE",
     )
     AUDIO = ("AUDIO_START", "AUDIO_FINISH", "AUDIO_ON_MIC", "AUDIO_OFF_MIC")
     ALC_MEMBER = (
         "AUDIO_OR_LIVE_CHANNEL_MEMBER_ENTER",
         "AUDIO_OR_LIVE_CHANNEL_MEMBER_EXIT",
     )
+
+
+TraceNames = ("start_callback_task", "async_start_callback_task")
```

### Comparing `qg-botsdk-2.7.0/qg_botsdk/_utils.py` & `qg-botsdk-3.0.0/qg_botsdk/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from asyncio import iscoroutinefunction
 from copy import deepcopy
 from functools import wraps
-from inspect import Signature, signature
+from inspect import Signature, signature, stack
 from json import dumps, loads
 from json.decoder import JSONDecodeError
 from sys import exc_info
 from time import localtime, strftime
 from traceback import extract_tb
-from typing import BinaryIO, Callable, Optional, Union
+from typing import BinaryIO, Callable, Dict, Iterable, Optional, Union
 
 from aiohttp import ContentTypeError
 
 from .version import __version__
 
 general_header = {"User-Agent": f"qg-botsdk v{__version__}"}
 security_header = {
@@ -95,14 +95,24 @@
                 if logger:
                     logger.error(f"调用内容安全检测接口失败，详情：{exception_handler(e)}")
                 return False
 
     return wrap
 
 
+def stack_exception_handler(error, stack_no: int = 1):
+    target_frame = stack()[stack_no]
+    return '[error:{}] File "{}", line {}, in {}'.format(
+        error.__repr__(),
+        target_frame.filename,
+        target_frame.lineno,
+        target_frame.function,
+    )
+
+
 def exception_handler(error):
     error_info = extract_tb(exc_info()[-1])[-1]
     return '[error:{}] File "{}", line {}, in {}'.format(
         error.__repr__(), *error_info[:3]
     )
 
 
@@ -111,19 +121,19 @@
     def wrap(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except Exception as e:
             logger = getattr(args[0], "logger", None)
             if logger:
                 logger.error(e.__repr__())
-                logger.debug(exception_handler(e))
+                logger.error(exception_handler(e))
             else:
                 t = strftime("%m-%d %H:%M:%S", localtime())
                 print(f"\033[1;31m[{t}] [ERROR]\033[0m {e.__repr__()}")
-                print(f"[{t}] [DEBUG] {exception_handler(e)}")
+                print(f"[{t}] [ERROR] {exception_handler(e)}")
 
     return wrap
 
 
 class object_class:
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
@@ -151,29 +161,38 @@
             id: str
             channel_id: str
             guild_id: str
             content: str
             timestamp: str
             tts: bool
             mention_everyone: bool
-            author: dict
+            author: Dict
             pinned: bool
             type: int
             flags: int
             seq_in_channel: str
             code: int
             message: str
 
         http_code: int
         trace_id: str
         result: bool
 
     return SendMsg
 
 
+_reply_args = (
+    "content",
+    "image",
+    "file_image",
+    "message_reference_id",
+    "ignore_message_reference_error",
+)
+
+
 class event_class(object_class):
     def reply(
         self,
         content: Optional[str] = None,
         image: Optional[str] = None,
         file_image: Optional[Union[bytes, BinaryIO, str]] = None,
         message_reference_id: Optional[str] = None,
@@ -191,16 +210,16 @@
         :param content: 消息文本（选填，此项与image至少需要有一个字段，否则无法下发消息）
         :param image: 图片url，不可发送本地图片（选填，此项与msg至少需要有一个字段，否则无法下发消息）
         :param file_image: 本地图片，可选三种方式传参，具体可参阅github中的example_10或帮助文档
         :param message_reference_id: 引用消息的id（选填）
         :param ignore_message_reference_error: 是否忽略获取引用消息详情错误，默认否（选填）
         :return: 返回的.data中为解析后的json数据
         """
-        kwargs = locals()
-        kwargs.pop("self", None)
+        raw_args = locals()
+        kwargs = {arg: raw_args[arg] for arg in _reply_args}
         t = getattr(self, "t", None)
         if t in msg_t:
             kwargs["message_id"] = getattr(self, "id", None)
         elif t in event_t:
             kwargs["message_id"] = getattr(self, "event_id", None)
         if "DIRECT_MESSAGE" in t:
             kwargs["guild_id"] = getattr(self, "guild_id", None)
@@ -235,16 +254,16 @@
         :param content: 消息文本（选填，此项与image至少需要有一个字段，否则无法下发消息）
         :param image: 图片url，不可发送本地图片（选填，此项与msg至少需要有一个字段，否则无法下发消息）
         :param file_image: 本地图片，可选三种方式传参，具体可参阅github中的example_10或帮助文档
         :param message_reference_id: 引用消息的id（选填）
         :param ignore_message_reference_error: 是否忽略获取引用消息详情错误，默认否（选填）
         :return: 返回的.data中为解析后的json数据
         """
-        kwargs = locals()
-        kwargs.pop("self", None)
+        raw_args = locals()
+        kwargs = {arg: raw_args[arg] for arg in _reply_args}
         t = getattr(self, "t", None)
         if t in msg_t:
             kwargs["message_id"] = getattr(self, "id", None)
         elif t in event_t:
             kwargs["message_id"] = getattr(self, "event_id", None)
         if "DIRECT_MESSAGE" in t:
             kwargs["guild_id"] = getattr(self, "guild_id", None)
@@ -298,15 +317,15 @@
         .replace("&lt;", "<")
         .replace("&gt;", ">")
         .replace("\xa0", " ")
         .strip()
     )
 
 
-def treat_thread(data: dict):
+def treat_thread(data: Dict):
     for items in ("content", "title"):
         try:
             data["d"]["thread_info"][items] = loads(
                 data.get("d", {}).get("thread_info", {}).get(items, "{}")
             )
         except JSONDecodeError:
             pass
@@ -376,23 +395,66 @@
             "trace_id": None,
             "http_code": None,
             "result": False,
         }
     )
 
 
-def check_func(func, *args, is_async: bool = False):
+def func_type_checker(func, *args, is_async: bool = False):
     sig = signature(func).parameters
     sig_keys = list(sig.keys())
     sig_keys_len = len(sig_keys)
     if sig_keys_len != len(args):
-        raise TypeError(f'函数{func.__name__}应包含以下类型的参数：{" ".join(args)}')
+        raise TypeError(
+            f'函数{func.__name__}应包含以下类型的{len(args)}个参数：{" ".join(args)}\n'
+            f"当前为{sig_keys_len}个参数：{sig_keys}"
+        )
     for i in range(sig_keys_len):
         annotation = sig[sig_keys[i]].annotation
         if annotation is not Signature.empty and annotation != args[i]:
             raise TypeError(f"函数{func.__name__}中{sig_keys[i]}参数应为类型：{args[i]}")
     if is_async:
         if not iscoroutinefunction(func):
             raise TypeError(f"函数{func.__name__}应为一个async coroutine函数")
     else:
         if not isinstance(func, Callable) or iscoroutinefunction(func):
             raise TypeError(f"函数{func.__name__}应为一个普通函数")
+
+
+class TraceCallerData:
+    def __init__(self, caller_names: Iterable[str], datas: Iterable[str]):
+        self.caller_names = caller_names
+        self.datas = datas
+
+    def get_target_data(self):
+        for frame in stack():
+            caller_name = frame.function
+            if caller_name in self.caller_names:
+                if not self.datas:
+                    return frame.frame.f_locals
+                try:
+                    target_data = frame.frame.f_locals
+                    for data in self.datas:
+                        target_data = (
+                            target_data.get(data, None)
+                            if isinstance(target_data, dict)
+                            else getattr(target_data, data, None)
+                        )
+                    return target_data
+                except Exception:
+                    pass
+
+    def __getattr__(self, item):
+        target_data = self.get_target_data()
+        if target_data:
+            return getattr(target_data, item)
+        raise AttributeError(
+            f"没有追溯到 {'::'.join(self.datas)} 变量（probably because of haven't start bot instance）"
+        )
+
+    def __getitem__(self, item):
+        target_data = self.get_target_data()
+        if target_data:
+            return target_data[item]
+        raise KeyError(
+            f"没有追溯到 {'::'.join(self.datas)} 变量（probably because of haven't start bot instance）"
+        )
```

### Comparing `qg-botsdk-2.7.0/qg_botsdk/api.py` & `qg-botsdk-3.0.0/qg_botsdk/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,66 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from asyncio import AbstractEventLoop, run_coroutine_threadsafe
-from time import sleep
-from typing import BinaryIO, Dict, List, Optional, Tuple, Union
+from time import sleep, time
+from typing import BinaryIO, Dict, Iterable, List, Optional, Tuple, Union
 
-from . import _api_model
+from . import _api_model, model
+from ._exception import WaitError, WaitTimeoutError
+from ._statics import TraceNames
+from ._utils import TraceCallerData
 from .async_api import AsyncAPI
 
 
 class API:
-    def __init__(self, api: AsyncAPI, loop: AbstractEventLoop):
+    def __init__(
+        self, api: AsyncAPI, loop: AbstractEventLoop, timeout: int, session_manager
+    ):
         self._api = api
         self._loop = loop
+        self._timeout = timeout
+        self.__session_manager = session_manager
+        self.__session_manager.api = self
+
+    # sdk internal api
+    def wait_for(
+        self,
+        scope: Union[model.Scope, Iterable[model.Scope]],
+        command_obj: model.BotCommandObject,
+        timeout: int = None,
+    ) -> model.Model.MESSAGE:
+        """
+        等待指定的command被触发
+
+        :param scope: 指定的校验作用域或作用域列表(USER, GUILD, CHANNEL, GLOBAL)，用作谁和在哪可以触发此wait_for
+        :param command_obj: 指定的Command，仅生效以下BotCommandObject的参数（command, regex, treat, at, short_circuit）
+        :param timeout: 超时时间，单位秒，None为永远等待
+        :return: Model.MESSAGE
+        """
+        self.__check_ready()
+        data = TraceCallerData(TraceNames, ("args",))[0]
+        command_obj.func = None
+        scope_key = self.__session_manager.register_wait_for(data, scope, command_obj)
+        _timeout_stamp = time() + timeout if timeout else None
+        while True:
+            check, result = self.__session_manager.check_wait_for(
+                scope_key, command_obj
+            )
+            if not check:
+                self.__session_manager.del_wait_for(data, command_obj)
+                raise WaitError("找不到对应的wait_for()等待任务")
+            if result is not None:
+                break
+            if _timeout_stamp and time() > _timeout_stamp:
+                self.__session_manager.del_wait_for(data, command_obj)
+                raise WaitTimeoutError(f"wait_for()等待超时： {command_obj}")
+            sleep(0.5)
+        return result
 
+    # bot api
     def __check_ready(self):
         if not self._loop.is_running():
             raise RuntimeError(
                 "Event loop is not running，请先通过BOT()实例的start()或block()方法启动bot并运行事件循环"
             )
 
     def security_setup(self, mini_id: str, mini_secret: str):
@@ -32,97 +76,96 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.security_check(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     @staticmethod
     def get_bot_id():
         raise DeprecationWarning("SDK版本>=2.3.2后已遗弃get_bot_id()的api，改为BOT.robot.id")
 
     def get_bot_info(self) -> _api_model.get_bot_info():
         """
         获取机器人详情
 
         :return:返回的.data中为解析后的json数据
         """
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.get_bot_info(), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_bot_guilds(self) -> _api_model.get_bot_guilds():
         """
         获取机器人所在的所有频道列表
 
         :return: 返回的.data中为包含所有数据的一个list，列表每个项均为object数据
         """
         self.__check_ready()
-        print(self._loop.is_running())
         future_ = run_coroutine_threadsafe(self._api.get_bot_guilds(), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_guild_info(self, guild_id: str) -> _api_model.get_guild_info():
         """
         获取频道详情信息
 
         :param guild_id: 频道id
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_guild_info(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_guild_channels(self, guild_id: str) -> _api_model.get_guild_channels():
         """
         获取频道的所有子频道列表数据
 
         :param guild_id: 频道id
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_guild_channels(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_channels_info(self, channel_id: str) -> _api_model.get_channels_info():
         """
         获取子频道数据
 
         :param channel_id: 子频道id
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_channels_info(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def create_channels(
         self,
         guild_id: str,
         name: str,
         type_: int,
         position: int,
-        parent_id: str,
-        sub_type: int,
-        private_type: int,
-        private_user_ids: List[str],
-        speak_permission: int,
+        parent_id: str = None,
+        sub_type: int = None,
+        private_type: int = None,
+        private_user_ids: List[str] = None,
+        speak_permission: int = None,
         application_id: Optional[str] = None,
     ) -> _api_model.create_channels():
         """
         用于在 guild_id 指定的频道下创建一个子频道，一般仅私域机器人可用
 
         :param guild_id: 频道id
         :param name: 需要创建的子频道名
@@ -138,15 +181,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.create_channels(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def patch_channels(
         self,
         channel_id: str,
         name: Optional[str] = None,
         position: Optional[int] = None,
         parent_id: Optional[str] = None,
@@ -166,45 +209,45 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.patch_channels(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def delete_channels(self, channel_id) -> _api_model.delete_channels():
         """
         用于删除 channel_id 指定的子频道
 
         :param channel_id: 子频道id
         :return: 返回的.result显示是否成功
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.delete_channels(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_guild_members(self, guild_id: str) -> _api_model.get_guild_members():
         """
         用于获取 guild_id 指定的频道中所有成员的详情列表
 
         :param guild_id: 频道id
         :return: 返回的.data中为包含所有数据的一个list，列表每个项均为object数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_guild_members(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_role_members(
         self, guild_id: str, role_id: str
     ) -> _api_model.get_role_members():
         """
         用于获取 guild_id 频道中指定 role_id 身份组下所有成员的详情列表
 
@@ -214,15 +257,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_role_members(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_member_info(
         self, guild_id: str, user_id: str
     ) -> _api_model.get_member_info():
         """
         用于获取 guild_id 指定的频道中 user_id 对应成员的详细信息
 
@@ -232,15 +275,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_member_info(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def delete_member(
         self,
         guild_id: str,
         user_id: str,
         add_blacklist: bool = False,
         delete_history_msg_days: int = 0,
@@ -254,30 +297,30 @@
         :param delete_history_msg_days: 用于撤回该成员的消息，可以指定撤回消息的时间范围
         :return: 返回的.result显示是否成功
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.delete_member(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_guild_roles(self, guild_id: str) -> _api_model.get_guild_roles():
         """
         用于获取 guild_id指定的频道下的身份组列表
 
         :param guild_id: 频道id
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_guild_roles(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def create_role(
         self,
         guild_id: str,
         name: Optional[str] = None,
         hoist: Optional[bool] = None,
         color: Optional[Union[str, Tuple[int, int, int]]] = None,
@@ -291,15 +334,15 @@
         :param color: 身份组颜色，支持输入RGB的三位tuple或HEX的sting颜色（选填)
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.create_role(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def patch_role(
         self,
         guild_id: str,
         role_id: str,
         name: Optional[str] = None,
         hoist: Optional[bool] = None,
@@ -315,29 +358,29 @@
         :param color: 身份组颜色，支持输入RGB的三位tuple或HEX的sting颜色（选填)
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.patch_role(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def delete_role(self, guild_id: str, role_id: str) -> _api_model.delete_role():
         """
         用于删除频道 guild_id下 role_id 对应的身份组
 
         :param guild_id: 频道ID
         :param role_id: 需要删除的身份组ID
         :return: 返回的.result显示是否成功
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.delete_role(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def create_role_member(
         self,
         user_id: str,
         guild_id: str,
         role_id: str,
         channel_id: Optional[str] = None,
@@ -353,15 +396,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.create_role_member(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def delete_role_member(
         self,
         user_id: str,
         guild_id: str,
         role_id: str,
         channel_id: Optional[str] = None,
@@ -377,15 +420,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.delete_role_member(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_channel_member_permission(
         self, channel_id: str, user_id: str
     ) -> _api_model.get_channel_member_permission():
         """
         用于获取 子频道 channel_id 下用户 user_id 的权限
 
@@ -395,39 +438,39 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_channel_member_permission(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def put_channel_member_permission(
         self,
         channel_id: str,
         user_id: str,
         add: Optional[str] = None,
         remove: Optional[str] = None,
     ) -> _api_model.put_channel_mr_permission():
         """
         用于修改子频道 channel_id 下用户 user_id 的权限
 
         :param channel_id: 子频道id
         :param user_id: 用户id
-        :param add: 需要添加的权限，string格式，可选：1，2，4，8
-        :param remove:需要删除的权限，string格式，可选：1，2，4，8
+        :param add: 需要添加的权限，string格式，1，2，4，8按需进行位运算后的结果
+        :param remove:需要删除的权限，string格式，1，2，4，8按需进行位运算后的结果
         :return: 返回的.result显示是否成功
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.put_channel_member_permission(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_channel_role_permission(
         self, channel_id: str, role_id: str
     ) -> _api_model.get_channel_role_permission():
         """
         用于获取 子频道 channel_id 下身份组 role_id 的权限
 
@@ -437,39 +480,39 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_channel_role_permission(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def put_channel_role_permission(
         self,
         channel_id: str,
         role_id: str,
         add: Optional[str] = None,
         remove: Optional[str] = None,
     ) -> _api_model.put_channel_mr_permission():
         """
         用于修改子频道 channel_id 下身份组 role_id 的权限
 
         :param channel_id: 子频道id
         :param role_id: 身份组id
-        :param add: 需要添加的权限，string格式，可选：1，2，4，8
-        :param remove:需要删除的权限，string格式，可选：1，2，4，8
+        :param add: 需要添加的权限，string格式，1，2，4，8按需进行位运算后的结果
+        :param remove:需要删除的权限，string格式，1，2，4，8按需进行位运算后的结果
         :return: 返回的.result显示是否成功
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.put_channel_role_permission(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_message_info(
         self, channel_id: str, message_id: str
     ) -> _api_model.get_message_info():
         """
         用于获取子频道 channel_id 下的消息 message_id 的详情
 
@@ -479,15 +522,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_message_info(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def send_msg(
         self,
         channel_id: str,
         content: Optional[str] = None,
         image: Optional[str] = None,
         file_image: Optional[Union[bytes, BinaryIO, str]] = None,
@@ -509,15 +552,15 @@
         :param ignore_message_reference_error: 是否忽略获取引用消息详情错误，默认否（选填）
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.send_msg(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def send_embed(
         self,
         channel_id: str,
         title: Optional[str] = None,
         content: Optional[List[str]] = None,
         image: Optional[str] = None,
@@ -537,15 +580,15 @@
         :param event_id: 事件id（选填）
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.send_embed(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def send_ark_23(
         self,
         channel_id: str,
         content: List[str],
         link: List[str],
         desc: Optional[str] = None,
@@ -565,15 +608,15 @@
         :param event_id: 事件id（选填）
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.send_ark_23(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def send_ark_24(
         self,
         channel_id: str,
         title: Optional[str] = None,
         content: Optional[str] = None,
         subtitile: Optional[str] = None,
@@ -599,15 +642,15 @@
         :param event_id: 事件id（选填）
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.send_ark_24(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def send_ark_37(
         self,
         channel_id: str,
         title: Optional[str] = None,
         content: Optional[str] = None,
         link: Optional[str] = None,
@@ -629,28 +672,28 @@
         :param event_id: 事件id（选填）
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.send_ark_37(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def send_markdown(
         self,
         channel_id: str,
         template_id: Optional[str] = None,
         key_values: Optional[
             Union[
                 List[Dict[str, Union[str, List[str]]]], Dict[str, Union[str, List[str]]]
             ]
         ] = None,
         content: Optional[str] = None,
         keyboard_id: Optional[str] = None,
-        keyboard_content: Optional[dict] = None,
+        keyboard_content: Optional[Dict] = None,
         message_id: Optional[str] = None,
         event_id: Optional[str] = None,
     ) -> _api_model.send_msg():
         """
         发送markdown消息的API，请注意机器人是否有权限使用此API
 
         :param channel_id: 子频道id
@@ -663,15 +706,15 @@
         :param event_id: 事件id（选填）
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.send_markdown(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def delete_msg(
         self, channel_id: str, message_id: str, hidetip: bool = False
     ) -> _api_model.delete_msg():
         """
         撤回消息的API，注意一般情况下仅私域可以使用
 
@@ -680,30 +723,30 @@
         :param hidetip: 是否隐藏提示小灰条，True为隐藏，False为显示（选填）
         :return: 返回的.result显示是否成功
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.delete_msg(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_guild_setting(self, guild_id: str) -> _api_model.get_guild_setting():
         """
         用于获取机器人在频道 guild_id 内的消息频率设置
 
         :param guild_id: 频道id
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_guild_setting(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def create_dm_guild(
         self, target_id: str, guild_id: str
     ) -> _api_model.create_dm_guild():
         """
         当机器人主动跟用户私信时，创建并获取一个虚拟频道id的API
 
@@ -713,15 +756,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.create_dm_guild(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def send_dm(
         self,
         guild_id: str,
         content: Optional[str] = None,
         image: Optional[str] = None,
         file_image: Optional[Union[bytes, BinaryIO, str]] = None,
@@ -743,15 +786,15 @@
         :param ignore_message_reference_error: 是否忽略获取引用消息详情错误，默认否（选填）
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.send_dm(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def delete_dm_msg(
         self, guild_id: str, message_id: str, hidetip: bool = False
     ) -> _api_model.delete_msg():
         """
         用于撤回私信频道 guild_id 中 message_id 指定的私信消息。只能用于撤回机器人自己发送的私信
 
@@ -760,15 +803,15 @@
         :param hidetip: 是否隐藏提示小灰条，True为隐藏，False为显示（选填）
         :return: 返回的.result显示是否成功
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.delete_dm_msg(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def mute_all_member(
         self,
         guild_id: str,
         mute_end_timestamp: Optional[str],
         mute_seconds: Optional[str],
     ) -> _api_model.mute_member():
@@ -782,15 +825,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.mute_all_member(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def mute_member(
         self,
         guild_id: str,
         user_id: str,
         mute_end_timestamp: Optional[str],
         mute_seconds: Optional[str],
@@ -804,15 +847,15 @@
         :param mute_seconds: 禁言多少秒（两个字段二选一，默认以 mute_end_timestamp 为准）
         :return: 返回的.result显示是否成功
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.mute_member(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def mute_members(
         self,
         guild_id: str,
         user_id: List[str],
         mute_end_timestamp: Optional[str],
         mute_seconds: Optional[str],
@@ -826,43 +869,45 @@
         :param mute_seconds: 禁言多少秒（两个字段二选一，默认以 mute_end_timestamp 为准）
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.mute_members(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def create_announce(
         self,
-        guild_id,
+        guild_id: str,
         channel_id: Optional[str] = None,
         message_id: Optional[str] = None,
         announces_type: Optional[int] = None,
+        recommend_channels: Optional[List[model.AnnounceRecommendChannels]] = None,
         recommend_channels_id: Optional[List[str]] = None,
         recommend_channels_introduce: Optional[List[str]] = None,
     ) -> _api_model.create_announce():
         """
         用于创建频道全局公告，公告类型分为 消息类型的频道公告 和 推荐子频道类型的频道公告
 
         :param guild_id: 频道id
         :param channel_id: 子频道id，message_id 有值则为必填
         :param message_id: 消息id，此项有值则优选将某条消息设置为成员公告
         :param announces_type: 公告类别 0：成员公告，1：欢迎公告，默认为成员公告
-        :param recommend_channels_id: 推荐子频道id列表，会一次全部替换推荐子频道列表
-        :param recommend_channels_introduce: 推荐子频道推荐语列表，列表长度应与recommend_channels_id一致
+        :param recommend_channels: 推荐子频道id与推荐语的dict列表，会一次全部替换推荐子频道列表
+        :param recommend_channels_id: deprecated
+        :param recommend_channels_introduce: deprecated
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.create_announce(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def delete_announce(
         self, guild_id: str, message_id: str = "all"
     ) -> _api_model.delete_announce():
         """
         用于删除频道 guild_id 下指定 message_id 的全局公告
 
@@ -872,29 +917,29 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.delete_announce(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def create_pinmsg(self, channel_id: str, message_id: str) -> _api_model.pinmsg():
         """
         用于添加子频道 channel_id 内的精华消息
 
         :param channel_id: 子频道id
         :param message_id: 目标消息id
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.create_pinmsg(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def delete_pinmsg(
         self, channel_id: str, message_id: str
     ) -> _api_model.delete_pinmsg():
         """
         用于删除子频道 channel_id 下指定 message_id 的精华消息
 
@@ -902,28 +947,28 @@
         :param message_id: 目标消息id
         :return: 返回的.result显示是否成功
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.delete_pinmsg(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_pinmsg(self, channel_id: str) -> _api_model.pinmsg():
         """
         用于获取子频道 channel_id 内的精华消息
 
         :param channel_id: 子频道id
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.get_pinmsg(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_schedules(
         self, channel_id: str, since: Optional[int] = None
     ) -> _api_model.get_schedules():
         """
         用于获取channel_id指定的子频道中当天的日程列表
 
@@ -931,15 +976,15 @@
         :param since: 起始时间戳(ms)
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.get_schedules(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_schedule_info(
         self, channel_id: str, schedule_id: str
     ) -> _api_model.schedule_info():
         """
         获取日程子频道 channel_id 下 schedule_id 指定的的日程的详情
 
@@ -949,15 +994,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_schedule_info(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def create_schedule(
         self,
         channel_id: str,
         schedule_name: str,
         start_timestamp: str,
         end_timestamp: str,
@@ -977,15 +1022,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.create_schedule(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def patch_schedule(
         self,
         channel_id: str,
         schedule_id: str,
         schedule_name: str,
         start_timestamp: str,
@@ -1007,15 +1052,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.patch_schedule(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def delete_schedule(
         self, channel_id: str, schedule_id: str
     ) -> _api_model.delete_schedule():
         """
         用于删除日程子频道 channel_id 下 schedule_id 指定的日程
 
@@ -1025,15 +1070,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.delete_schedule(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def create_reaction(
         self, channel_id: str, message_id: str, type_: str, id_: str
     ) -> _api_model.reactions():
         """
         对message_id指定的消息进行表情表态
 
@@ -1045,15 +1090,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.create_reaction(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def delete_reaction(
         self, channel_id: str, message_id: str, type_: str, id_: str
     ) -> _api_model.reactions():
         """
         删除自己对message_id指定消息的表情表态
 
@@ -1065,15 +1110,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.delete_reaction(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_reaction_users(
         self, channel_id: str, message_id: str, type_: str, id_: str
     ) -> _api_model.get_reaction_users():
         """
         拉取对消息 message_id 指定表情表态的用户列表
 
@@ -1085,15 +1130,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_reaction_users(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def control_audio(
         self,
         channel_id: str,
         status: int,
         audio_url: Optional[str] = None,
         text: Optional[str] = None,
@@ -1107,54 +1152,54 @@
         :param text: 状态文本（比如：简单爱-周杰伦），可选，status为0时传，其他操作不传
         :return: 返回的.result显示是否成功
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.control_audio(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def bot_on_mic(self, channel_id: str) -> _api_model.audio():
         """
         机器人在 channel_id 对应的语音子频道上麦
 
         :param channel_id: 子频道id
         :return: 返回的.result显示是否成功
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.bot_on_mic(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def bot_off_mic(self, channel_id: str) -> _api_model.audio():
         """
         机器人在 channel_id 对应的语音子频道下麦
 
         :param channel_id: 子频道id
         :return: 返回的.result显示是否成功
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.bot_off_mic(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_threads(self, channel_id: str) -> _api_model.get_threads():
         """
         获取子频道下的帖子列表
 
         :param channel_id: 目标论坛子频道id
         :return: 返回的.data中为解析后的json数据列表
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.get_threads(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_thread_info(
         self, channel_id: str, thread_id: str
     ) -> _api_model.get_thread_info():
         """
         获取子频道下的帖子详情
 
@@ -1164,33 +1209,33 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_thread_info(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def create_thread(
-        self, channel_id: str, title: str, content: Union[str, dict], format_: int
+        self, channel_id: str, title: str, content: Union[str, Dict], format_: int
     ) -> _api_model.create_thread():
         """
         创建帖子，创建成功后，返回创建成功的任务ID
 
         :param channel_id: 目标论坛子频道id
         :param title: 帖子标题
         :param content: 帖子内容（具体格式根据format_判断）
         :param format_: 帖子文本格式（1：普通文本、2：HTML、3：Markdown、4：Json）
         :return: 返回的.data中为解析后的json数据
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.create_thread(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def delete_thread(
         self, channel_id: str, thread_id: str
     ) -> _api_model.delete_thread():
         """
         删除指定子频道下的某个帖子
 
@@ -1198,15 +1243,15 @@
         :param thread_id: 帖子id
         :return: 返回的.result显示是否成功
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(self._api.delete_thread(**_args), self._loop)
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def get_guild_permissions(
         self, guild_id: str
     ) -> _api_model.get_guild_permissions():
         """
         获取机器人在频道 guild_id 内可以使用的权限列表
 
@@ -1215,15 +1260,15 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.get_guild_permissions(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
 
     def create_permission_demand(
         self, guild_id: str, channel_id: str, api: str, desc: Optional[str]
     ) -> _api_model.create_permission_demand():
         """
         发送频道API接口权限授权链接到频道
 
@@ -1235,8 +1280,8 @@
         """
         _args = locals()
         _args.pop("self")
         self.__check_ready()
         future_ = run_coroutine_threadsafe(
             self._api.create_permission_demand(**_args), self._loop
         )
-        return future_.result()
+        return future_.result(timeout=self._timeout)
```

### Comparing `qg-botsdk-2.7.0/qg_botsdk/async_api.py` & `qg-botsdk-3.0.0/qg_botsdk/async_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,106 +1,147 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+from asyncio import sleep
 from io import BufferedReader
 from json import dumps, loads
 from json.decoder import JSONDecodeError
 from os.path import exists
 from time import time
-from typing import BinaryIO, Dict, List, Optional, Tuple, Union
+from typing import BinaryIO, Dict, Iterable, List, Optional, Tuple, Union
 
-from . import _api_model
+from . import _api_model, model
+from ._exception import WaitError, WaitTimeoutError
+from ._statics import TraceNames
 from ._utils import (
+    TraceCallerData,
     empty_temp,
     http_temp,
     objectize,
     regular_temp,
     sdk_error_temp,
     security_header,
     security_wrapper,
 )
 from .http import FormData_
 from .utils import convert_color
 
 
 class AsyncAPI:
-    def __init__(self, bot_url, session, logger, check_warning):
-        self.bot_url = bot_url
+    def __init__(self, bot_url, session, logger, check_warning, session_manager):
+        self._bot_url = bot_url
         self._mini_id = None
         self._mini_secret = None
         self._session = session
-        self.logger = logger
-        self.check_warning = check_warning
-        self.security_code = ""
-        self.code_expire = 0
+        self._logger = logger
+        self._check_warning = check_warning
+        self._security_code = ""
+        self._code_expire = 0
+        self.__session_manager = session_manager
+        self.__session_manager.api = self
+
+    # sdk api
+    async def wait_for(
+        self,
+        scope: Union[model.Scope, Iterable[model.Scope]],
+        command_obj: model.BotCommandObject,
+        timeout: int = None,
+    ) -> model.Model.MESSAGE:
+        """
+        等待指定的command被触发
+
+        :param scope: 指定的校验作用域或作用域列表(USER, GUILD, CHANNEL, GLOBAL)，用作谁和在哪可以触发此wait_for
+        :param command_obj: 指定的Command，仅生效以下BotCommandObject的参数（command, regex, treat, at, short_circuit）
+        :param timeout: 超时时间，单位秒，None为永远等待
+        :return: Model.MESSAGE
+        """
+        data = TraceCallerData(TraceNames, ("args",))[0]
+        command_obj.func = None
+        scope_key = self.__session_manager.register_wait_for(data, scope, command_obj)
+        _timeout_stamp = time() + timeout if timeout else None
+        while True:
+            check, result = self.__session_manager.check_wait_for(
+                scope_key, command_obj
+            )
+            if not check:
+                self.__session_manager.del_wait_for(data, command_obj)
+                raise WaitError("找不到对应的wait_for()等待任务")
+            if result is not None:
+                break
+            if _timeout_stamp and time() > _timeout_stamp:
+                self.__session_manager.del_wait_for(data, command_obj)
+                raise WaitTimeoutError(f"wait_for()等待超时： {command_obj}")
+            await sleep(0.5)
+        return result
 
+    # bot open api
     def security_setup(self, mini_id: str, mini_secret: str):
         self._mini_id = mini_id
         self._mini_secret = mini_secret
 
     @security_wrapper
     async def __security_check_code(self):
         if self._mini_secret is None:
-            self.logger.error("无法调用内容安全检测接口（备注：没有填入小程序密钥）")
+            self._logger.error("无法调用内容安全检测接口（备注：没有填入小程序密钥）")
             return None
         return_ = await self._session.get(
             f"https://api.q.qq.com/api/getToken?grant_type=client_credential&"
             f"appid={self._mini_id}&secret={self._mini_secret}"
         )
         resp = await return_.json()
         code = resp.get("access_token")
         if not code:
-            self.logger.error(
+            self._logger.error(
                 f"无法调用内容安全检测接口（code: {return_.status}, content: {await return_.text()}）"
             )
             return None
-        self.security_code = code
-        self.code_expire = time() + 7000
-        return self.security_code
+        self._security_code = code
+        self._code_expire = time() + 7000
+        return self._security_code
 
     @security_wrapper
     async def security_check(self, content: str) -> bool:
         """
         腾讯小程序侧内容安全检测接口，使用此接口必须填入bot_secret密钥
 
         :param content: 需要检测的内容
         :return: True或False（bool），代表是否通过安全检测
         """
-        if not self.security_code or time() >= self.code_expire:
+        if not self._security_code or time() >= self._code_expire:
             await self.__security_check_code()
         return_ = await self._session.post(
-            f"https://api.q.qq.com/api/json/security/MsgSecCheck?access_token={self.security_code}",
+            f"https://api.q.qq.com/api/json/security/MsgSecCheck?access_token={self._security_code}",
             json={"content": content},
             headers=security_header,
         )
         check = await return_.json()
-        self.logger.debug(f"[安全接口] {check}")
+        self._logger.debug(f"[安全接口] {check}")
         if check.get("errCode") in (-1800110107, -1800110108, -1800110109):
             await self.__security_check_code()
             return_ = await self._session.post(
-                f"https://api.q.qq.com/api/json/security/MsgSecCheck?access_token={self.security_code}",
+                f"https://api.q.qq.com/api/json/security/MsgSecCheck?access_token={self._security_code}",
                 json={"content": content},
                 headers=security_header,
             )
             check = await return_.json()
-            self.logger.debug(f"[安全接口] {check}")
+            self._logger.debug(f"[安全接口] {check}")
         if check["errCode"] == 0:
             return True
         return False
 
     @staticmethod
     async def get_bot_id():
         raise DeprecationWarning("SDK版本>=2.3.2后已遗弃get_bot_id()的api，改为BOT.robot.id")
 
     async def get_bot_info(self) -> _api_model.get_bot_info():
         """
         获取机器人详情
 
         :return:返回的.data中为解析后的json数据
         """
-        return_ = await self._session.get(f"{self.bot_url}/users/@me")
+        return_ = await self._session.get(f"{self._bot_url}/users/@me")
         return await regular_temp(return_)
 
     async def get_bot_guilds(self) -> _api_model.get_bot_guilds():
         """
         获取机器人所在的所有频道列表
 
         :return: 返回的.data中为包含所有数据的一个list，列表每个项均为object数据
@@ -110,19 +151,19 @@
         results = []
         data = []
         return_dict = None
         try:
             while True:
                 if return_dict is None:
                     return_ = await self._session.get(
-                        f"{self.bot_url}/users/@me/guilds"
+                        f"{self._bot_url}/users/@me/guilds"
                     )
                 elif len(return_dict) == 100:
                     return_ = await self._session.get(
-                        f'{self.bot_url}/users/@me/guilds?after={return_dict[-1]["id"]}'
+                        f'{self._bot_url}/users/@me/guilds?after={return_dict[-1]["id"]}'
                     )
                 else:
                     break
                 trace_ids.append(return_.headers["X-Tps-Trace-Id"])
                 codes.append(return_.status)
                 return_dict = await return_.json()
                 if isinstance(return_dict, dict) and "code" in return_dict.keys():
@@ -144,52 +185,52 @@
     async def get_guild_info(self, guild_id: str) -> _api_model.get_guild_info():
         """
         获取频道详情信息
 
         :param guild_id: 频道id
         :return: 返回的.data中为解析后的json数据
         """
-        return_ = await self._session.get(f"{self.bot_url}/guilds/{guild_id}")
+        return_ = await self._session.get(f"{self._bot_url}/guilds/{guild_id}")
         return await regular_temp(return_)
 
     async def get_guild_channels(
         self, guild_id: str
     ) -> _api_model.get_guild_channels():
         """
         获取频道的所有子频道列表数据
 
         :param guild_id: 频道id
         :return: 返回的.data中为解析后的json数据
         """
-        return_ = await self._session.get(f"{self.bot_url}/guilds/{guild_id}/channels")
+        return_ = await self._session.get(f"{self._bot_url}/guilds/{guild_id}/channels")
         return await regular_temp(return_)
 
     async def get_channels_info(
         self, channel_id: str
     ) -> _api_model.get_channels_info():
         """
         获取子频道数据
 
         :param channel_id: 子频道id
         :return: 返回的.data中为解析后的json数据
         """
-        return_ = await self._session.get(f"{self.bot_url}/channels/{channel_id}")
+        return_ = await self._session.get(f"{self._bot_url}/channels/{channel_id}")
         return await regular_temp(return_)
 
     async def create_channels(
         self,
         guild_id: str,
         name: str,
         type_: int,
         position: int,
-        parent_id: str,
-        sub_type: int,
-        private_type: int,
-        private_user_ids: List[str],
-        speak_permission: int,
+        parent_id: str = None,
+        sub_type: int = None,
+        private_type: int = None,
+        private_user_ids: List[str] = None,
+        speak_permission: int = None,
         application_id: Optional[str] = None,
     ) -> _api_model.create_channels():
         """
         用于在 guild_id 指定的频道下创建一个子频道，一般仅私域机器人可用
 
         :param guild_id: 频道id
         :param name: 需要创建的子频道名
@@ -199,28 +240,28 @@
         :param sub_type: 需要创建的子频道子类型
         :param private_type: 需要创建的子频道私密类型
         :param private_user_ids: 需要创建的子频道私密类型成员ID列表
         :param speak_permission: 需要创建的子频道发言权限
         :param application_id: 需要创建的应用类型子频道应用 AppID，仅应用子频道需要该字段
         :return: 返回的.data中为解析后的json数据
         """
-        self.check_warning("创建子频道")
+        self._check_warning("创建子频道")
         json_ = {
             "name": name,
             "type": type_,
             "position": position,
             "parent_id": parent_id,
             "sub_type": sub_type,
             "private_type": private_type,
             "private_user_ids": private_user_ids,
             "speak_permission": speak_permission,
             "application_id": application_id,
         }
         return_ = await self._session.post(
-            f"{self.bot_url}/guilds/{guild_id}/channels", json=json_
+            f"{self._bot_url}/guilds/{guild_id}/channels", json=json_
         )
         return await regular_temp(return_)
 
     async def patch_channels(
         self,
         channel_id: str,
         name: Optional[str] = None,
@@ -236,36 +277,40 @@
         :param name: 子频道名
         :param position: 子频道排序
         :param parent_id: 子频道所属分组id
         :param private_type: 子频道私密类型
         :param speak_permission: 子频道发言权限
         :return: 返回的.data中为解析后的json数据
         """
-        self.check_warning("修改子频道")
-        json_ = {
-            "name": name,
-            "position": position,
-            "parent_id": parent_id,
-            "private_type": private_type,
-            "speak_permission": speak_permission,
-        }
+        self._check_warning("修改子频道")
+        json_ = {}
+        if name is not None:
+            json_["name"] = name
+        if position is not None:
+            json_["position"] = position
+        if parent_id is not None:
+            json_["parent_id"] = parent_id
+        if private_type is not None:
+            json_["private_type"] = private_type
+        if speak_permission is not None:
+            json_["speak_permission"] = speak_permission
         return_ = await self._session.patch(
-            f"{self.bot_url}/channels/{channel_id}", json=json_
+            f"{self._bot_url}/channels/{channel_id}", json=json_
         )
         return await regular_temp(return_)
 
     async def delete_channels(self, channel_id) -> _api_model.delete_channels():
         """
         用于删除 channel_id 指定的子频道
 
         :param channel_id: 子频道id
         :return: 返回的.result显示是否成功
         """
-        self.check_warning("删除子频道")
-        return_ = await self._session.delete(f"{self.bot_url}/channels/{channel_id}")
+        self._check_warning("删除子频道")
+        return_ = await self._session.delete(f"{self._bot_url}/channels/{channel_id}")
         return await http_temp(return_, 200)
 
     async def get_guild_members(self, guild_id: str) -> _api_model.get_guild_members():
         """
         用于获取 guild_id 指定的频道中所有成员的详情列表
 
         :param guild_id: 频道id
@@ -276,21 +321,21 @@
         results = []
         data = []
         return_dict = None
         try:
             while True:
                 if return_dict is None:
                     return_ = await self._session.get(
-                        f"{self.bot_url}/guilds/{guild_id}/members?limit=400"
+                        f"{self._bot_url}/guilds/{guild_id}/members?limit=400"
                     )
                 elif not return_dict:
                     break
                 else:
                     return_ = await self._session.get(
-                        f"{self.bot_url}/guilds/{guild_id}/members?limit=400&after="
+                        f"{self._bot_url}/guilds/{guild_id}/members?limit=400&after="
                         + return_dict[-1]["user"]["id"]
                     )
                 trace_ids.append(return_.headers["X-Tps-Trace-Id"])
                 codes.append(return_.status)
                 return_dict = await return_.json()
                 if isinstance(return_dict, dict) and "code" in return_dict.keys():
                     results.append(False)
@@ -346,15 +391,15 @@
         return_dict = None
         start_index = 0
         try:
             while True:
                 if return_dict is not None and not return_dict.get("data"):
                     break
                 return_ = await self._session.get(
-                    f"{self.bot_url}/guilds/{guild_id}/roles/{role_id}/members?"
+                    f"{self._bot_url}/guilds/{guild_id}/roles/{role_id}/members?"
                     f"limit=400&start_index={start_index}"
                 )
                 trace_ids.append(return_.headers["X-Tps-Trace-Id"])
                 codes.append(return_.status)
                 return_dict = await return_.json()
                 if isinstance(return_dict, dict) and "code" in return_dict.keys():
                     results.append(False)
@@ -403,15 +448,15 @@
         用于获取 guild_id 指定的频道中 user_id 对应成员的详细信息
 
         :param guild_id: 频道id
         :param user_id: 成员id
         :return: 返回的.data中为解析后的json数据
         """
         return_ = await self._session.get(
-            f"{self.bot_url}/guilds/{guild_id}/members/{user_id}"
+            f"{self._bot_url}/guilds/{guild_id}/members/{user_id}"
         )
         return await regular_temp(return_)
 
     async def delete_member(
         self,
         guild_id: str,
         user_id: str,
@@ -423,34 +468,34 @@
 
         :param guild_id: 频道ID
         :param user_id: 目标用户ID
         :param add_blacklist: 是否同时添加黑名单
         :param delete_history_msg_days: 用于撤回该成员的消息，可以指定撤回消息的时间范围
         :return: 返回的.result显示是否成功
         """
-        self.check_warning("删除频道成员")
+        self._check_warning("删除频道成员")
         if delete_history_msg_days not in (3, 7, 15, 30, 0, -1):
             return sdk_error_temp("注意delete_history_msg_days的数值只能是3，7，15，30，0，-1")
         json_ = {
             "add_blacklist": add_blacklist,
             "delete_history_msg_days": delete_history_msg_days,
         }
         return_ = await self._session.delete(
-            f"{self.bot_url}/guilds/{guild_id}/members/{user_id}", json=json_
+            f"{self._bot_url}/guilds/{guild_id}/members/{user_id}", json=json_
         )
         return await http_temp(return_, 204)
 
     async def get_guild_roles(self, guild_id: str) -> _api_model.get_guild_roles():
         """
         用于获取 guild_id指定的频道下的身份组列表
 
         :param guild_id: 频道id
         :return: 返回的.data中为解析后的json数据
         """
-        return_ = await self._session.get(f"{self.bot_url}/guilds/{guild_id}/roles")
+        return_ = await self._session.get(f"{self._bot_url}/guilds/{guild_id}/roles")
         return await regular_temp(return_)
 
     async def create_role(
         self,
         guild_id: str,
         name: Optional[str] = None,
         hoist: Optional[bool] = None,
@@ -474,15 +519,15 @@
             hoist_ = None
         if color is not None:
             color_ = convert_color(color)
         else:
             color_ = None
         json_ = {"name": name, "color": color_, "hoist": hoist_}
         return_ = await self._session.post(
-            f"{self.bot_url}/guilds/{guild_id}/roles", json=json_
+            f"{self._bot_url}/guilds/{guild_id}/roles", json=json_
         )
         return await regular_temp(return_)
 
     async def patch_role(
         self,
         guild_id: str,
         role_id: str,
@@ -509,30 +554,30 @@
             hoist_ = None
         if color is not None:
             color_ = convert_color(color)
         else:
             color_ = None
         json_ = {"name": name, "color": color_, "hoist": hoist_}
         return_ = await self._session.patch(
-            f"{self.bot_url}/guilds/{guild_id}/roles/{role_id}", json=json_
+            f"{self._bot_url}/guilds/{guild_id}/roles/{role_id}", json=json_
         )
         return await regular_temp(return_)
 
     async def delete_role(
         self, guild_id: str, role_id: str
     ) -> _api_model.delete_role():
         """
         用于删除频道 guild_id下 role_id 对应的身份组
 
         :param guild_id: 频道ID
         :param role_id: 需要删除的身份组ID
         :return: 返回的.result显示是否成功
         """
         return_ = await self._session.delete(
-            f"{self.bot_url}/guilds/{guild_id}/roles/{role_id}"
+            f"{self._bot_url}/guilds/{guild_id}/roles/{role_id}"
         )
         return await http_temp(return_, 204)
 
     async def create_role_member(
         self,
         user_id: str,
         guild_id: str,
@@ -547,25 +592,25 @@
         :param role_id: 身份组编号，可从例如get_roles函数获取
         :param channel_id: 如果要增加的身份组ID是5-子频道管理员，需要输入此项来指定具体是哪个子频道
         :return: 返回的.result显示是否成功
         """
         if role_id == "5":
             if channel_id is not None:
                 return_ = await self._session.put(
-                    f"{self.bot_url}/guilds/{guild_id}/members/{user_id}/roles/"
+                    f"{self._bot_url}/guilds/{guild_id}/members/{user_id}/roles/"
                     f"{role_id}",
                     json={"channel": {"id": channel_id}},
                 )
             else:
                 return sdk_error_temp(
                     "注意如果要增加的身份组ID是5-子频道管理员，需要输入channel_id项来指定具体是哪个子频道"
                 )
         else:
             return_ = await self._session.put(
-                f"{self.bot_url}/guilds/{guild_id}/members/{user_id}/roles/{role_id}"
+                f"{self._bot_url}/guilds/{guild_id}/members/{user_id}/roles/{role_id}"
             )
         return await http_temp(return_, 204)
 
     async def delete_role_member(
         self,
         user_id: str,
         guild_id: str,
@@ -580,40 +625,40 @@
         :param role_id: 身份组编号，可从例如get_roles函数获取
         :param channel_id: 如果要增加的身份组ID是5-子频道管理员，需要输入此项来指定具体是哪个子频道
         :return: 返回的.result显示是否成功
         """
         if role_id == "5":
             if channel_id is not None:
                 return_ = await self._session.delete(
-                    f"{self.bot_url}/guilds/{guild_id}/members/{user_id}/roles/"
+                    f"{self._bot_url}/guilds/{guild_id}/members/{user_id}/roles/"
                     f"{role_id}",
                     json={"channel": {"id": channel_id}},
                 )
             else:
                 return sdk_error_temp(
                     "注意如果要增加的身份组ID是5-子频道管理员，需要输入channel_id项来指定具体是哪个子频道"
                 )
         else:
             return_ = await self._session.delete(
-                f"{self.bot_url}/guilds/{guild_id}/members/{user_id}/roles/{role_id}"
+                f"{self._bot_url}/guilds/{guild_id}/members/{user_id}/roles/{role_id}"
             )
         return await http_temp(return_, 204)
 
     async def get_channel_member_permission(
         self, channel_id: str, user_id: str
     ) -> _api_model.get_channel_member_permission():
         """
         用于获取 子频道 channel_id 下用户 user_id 的权限
 
         :param channel_id: 子频道id
         :param user_id: 用户id
         :return: 返回的.data中为解析后的json数据
         """
         return_ = await self._session.get(
-            f"{self.bot_url}/channels/{channel_id}/members/{user_id}/permissions"
+            f"{self._bot_url}/channels/{channel_id}/members/{user_id}/permissions"
         )
         return await regular_temp(return_)
 
     async def put_channel_member_permission(
         self,
         channel_id: str,
         user_id: str,
@@ -621,23 +666,26 @@
         remove: Optional[str] = None,
     ) -> _api_model.put_channel_mr_permission():
         """
         用于修改子频道 channel_id 下用户 user_id 的权限
 
         :param channel_id: 子频道id
         :param user_id: 用户id
-        :param add: 需要添加的权限，string格式，可选：1，2，4，8
-        :param remove:需要删除的权限，string格式，可选：1，2，4，8
+        :param add: 需要添加的权限，string格式，1，2，4，8按需进行位运算后的结果
+        :param remove:需要删除的权限，string格式，1，2，4，8按需进行位运算后的结果
         :return: 返回的.result显示是否成功
         """
-        if not all([items in ("1", "2", "4", "8", None) for items in (add, remove)]):
-            return sdk_error_temp("注意add或remove的值只能为为1、2、4或8的文本格式内容")
-        json_ = {"add": add, "remove": remove}
+        try:
+            if not all([int(items) < 16 for items in (add, remove)]):  # 16 == 1 << 4
+                return sdk_error_temp("注意add或remove的值只能为为1、2、4或8的位或运算内容")
+        except ValueError:
+            return sdk_error_temp("注意add或remove的值只能为为1、2、4或8的位或运算内容")
+        json_ = {"add": str(add), "remove": str(remove)}
         return_ = await self._session.put(
-            f"{self.bot_url}/channels/{channel_id}/members/{user_id}/permissions",
+            f"{self._bot_url}/channels/{channel_id}/members/{user_id}/permissions",
             json=json_,
         )
         return await http_temp(return_, 204)
 
     async def get_channel_role_permission(
         self, channel_id: str, role_id: str
     ) -> _api_model.get_channel_role_permission():
@@ -645,15 +693,15 @@
         用于获取 子频道 channel_id 下身份组 role_id 的权限
 
         :param channel_id: 子频道id
         :param role_id: 身份组id
         :return: 返回的.data中为解析后的json数据
         """
         return_ = await self._session.get(
-            f"{self.bot_url}/channels/{channel_id}/roles/{role_id}/permissions"
+            f"{self._bot_url}/channels/{channel_id}/roles/{role_id}/permissions"
         )
         return await regular_temp(return_)
 
     async def put_channel_role_permission(
         self,
         channel_id: str,
         role_id: str,
@@ -661,23 +709,26 @@
         remove: Optional[str] = None,
     ) -> _api_model.put_channel_mr_permission():
         """
         用于修改子频道 channel_id 下身份组 role_id 的权限
 
         :param channel_id: 子频道id
         :param role_id: 身份组id
-        :param add: 需要添加的权限，string格式，可选：1，2，4，8
-        :param remove:需要删除的权限，string格式，可选：1，2，4，8
+        :param add: 需要添加的权限，string格式，1，2，4，8按需进行位运算后的结果
+        :param remove:需要删除的权限，string格式，1，2，4，8按需进行位运算后的结果
         :return: 返回的.result显示是否成功
         """
-        if not all([items in ("1", "2", "4", "8", None) for items in (add, remove)]):
-            return sdk_error_temp("注意add或remove的值只能为为1、2、4或8的文本格式内容")
-        json_ = {"add": add, "remove": remove}
+        try:
+            if not all([int(items) < 16 for items in (add, remove)]):  # 16 == 1 << 4
+                return sdk_error_temp("注意add或remove的值只能为为1、2、4或8的位或运算内容")
+        except ValueError:
+            return sdk_error_temp("注意add或remove的值只能为为1、2、4或8的位或运算内容")
+        json_ = {"add": str(add), "remove": str(remove)}
         return_ = await self._session.put(
-            f"{self.bot_url}/channels/{channel_id}/roles/{role_id}/permissions",
+            f"{self._bot_url}/channels/{channel_id}/roles/{role_id}/permissions",
             json=json_,
         )
         return await http_temp(return_, 204)
 
     async def get_message_info(
         self, channel_id: str, message_id: str
     ) -> _api_model.get_message_info():
@@ -685,15 +736,15 @@
         用于获取子频道 channel_id 下的消息 message_id 的详情
 
         :param channel_id: 频道ID
         :param message_id: 目标消息ID
         :return: 返回的.data中为解析后的json数据
         """
         return_ = await self._session.get(
-            f"{self.bot_url}/channels/{channel_id}/messages/{message_id}"
+            f"{self._bot_url}/channels/{channel_id}/messages/{message_id}"
         )
         return await regular_temp(return_)
 
     async def send_msg(
         self,
         channel_id: str,
         content: Optional[str] = None,
@@ -754,19 +805,19 @@
                 return sdk_error_temp(f"file_image不支持{type(file_image)}的内容")
             json_["file_image"] = file_image
             data_ = FormData_()
             for keys, values in json_.items():
                 if values is not None and keys != "image":
                     data_.add_field(keys, values)
             return_ = await self._session.post(
-                f"{self.bot_url}/channels/{channel_id}/messages", data=data_
+                f"{self._bot_url}/channels/{channel_id}/messages", data=data_
             )
         else:
             return_ = await self._session.post(
-                f"{self.bot_url}/channels/{channel_id}/messages", json=json_
+                f"{self._bot_url}/channels/{channel_id}/messages", json=json_
             )
         return await regular_temp(return_)
 
     async def send_embed(
         self,
         channel_id: str,
         title: Optional[str] = None,
@@ -798,15 +849,15 @@
             "msg_id": message_id,
             "event_id": event_id,
         }
         if content is not None:
             for items in content:
                 json_["embed"]["fields"].append({"name": str(items)})
         return_ = await self._session.post(
-            f"{self.bot_url}/channels/{channel_id}/messages", json=json_
+            f"{self._bot_url}/channels/{channel_id}/messages", json=json_
         )
         return await regular_temp(return_)
 
     async def send_ark_23(
         self,
         channel_id: str,
         content: List[str],
@@ -852,15 +903,15 @@
                     "obj_kv": [
                         {"key": "desc", "value": _content},
                         {"key": "link", "value": _link},
                     ]
                 }
             )
         return_ = await self._session.post(
-            f"{self.bot_url}/channels/{channel_id}/messages", json=json_
+            f"{self._bot_url}/channels/{channel_id}/messages", json=json_
         )
         return await regular_temp(return_)
 
     async def send_ark_24(
         self,
         channel_id: str,
         title: Optional[str] = None,
@@ -901,15 +952,15 @@
                     {"key": "#SUBTITLE#", "value": subtitile},
                 ],
             },
             "msg_id": message_id,
             "event_id": event_id,
         }
         return_ = await self._session.post(
-            f"{self.bot_url}/channels/{channel_id}/messages", json=json_
+            f"{self._bot_url}/channels/{channel_id}/messages", json=json_
         )
         return await regular_temp(return_)
 
     async def send_ark_37(
         self,
         channel_id: str,
         title: Optional[str] = None,
@@ -944,30 +995,30 @@
                     {"key": "#METAURL#", "value": link},
                 ],
             },
             "msg_id": message_id,
             "event_id": event_id,
         }
         return_ = await self._session.post(
-            f"{self.bot_url}/channels/{channel_id}/messages", json=json_
+            f"{self._bot_url}/channels/{channel_id}/messages", json=json_
         )
         return await regular_temp(return_)
 
     async def send_markdown(
         self,
         channel_id: str,
         template_id: Optional[str] = None,
         key_values: Optional[
             Union[
                 List[Dict[str, Union[str, List[str]]]], Dict[str, Union[str, List[str]]]
             ]
         ] = None,
         content: Optional[str] = None,
         keyboard_id: Optional[str] = None,
-        keyboard_content: Optional[dict] = None,
+        keyboard_content: Optional[Dict] = None,
         message_id: Optional[str] = None,
         event_id: Optional[str] = None,
     ) -> _api_model.send_msg():
         """
         发送markdown消息的API，请注意机器人是否有权限使用此API
 
         :param channel_id: 子频道id
@@ -978,25 +1029,25 @@
         :param keyboard_content: 原生 keyboard 内容（选填，与keyboard_id不可同时存在）
         :param message_id: 消息id（选填）
         :param event_id: 事件id（选填）
         :return: 返回的.data中为解析后的json数据
         """
         if keyboard_content:
             if keyboard_id:
-                self.logger.warning(
+                self._logger.warning(
                     "注意keyboard_id与keyboard_content不可同时存在，注意系统已根据优先级仅保留keyboard_content"
                 )
             keyboard = {"content": keyboard_content}
         elif keyboard_id:
             keyboard = {"id": keyboard_id}
         else:
             keyboard = None
         if content:
             if template_id:
-                self.logger.warning("注意content与template_id不可同时存在，注意系统已根据优先级仅保留content")
+                self._logger.warning("注意content与template_id不可同时存在，注意系统已根据优先级仅保留content")
             json_ = {
                 "markdown": {"content": content},
                 "msg_id": message_id,
                 "event_id": event_id,
                 "keyboard": keyboard,
             }
         else:
@@ -1026,60 +1077,60 @@
             json_ = {
                 "markdown": {"custom_template_id": template_id, "params": params},
                 "msg_id": message_id,
                 "event_id": event_id,
                 "keyboard": keyboard,
             }
         return_ = await self._session.post(
-            f"{self.bot_url}/channels/{channel_id}/messages", json=json_
+            f"{self._bot_url}/channels/{channel_id}/messages", json=json_
         )
         return await regular_temp(return_)
 
     async def delete_msg(
         self, channel_id: str, message_id: str, hidetip: bool = False
     ) -> _api_model.delete_msg():
         """
         撤回消息的API，注意一般情况下仅私域可以使用
 
         :param channel_id: 子频道id
         :param message_id: 需撤回消息的消息id
         :param hidetip: 是否隐藏提示小灰条，True为隐藏，False为显示（选填）
         :return: 返回的.result显示是否成功
         """
-        self.check_warning("撤回消息")
+        self._check_warning("撤回消息")
         return_ = await self._session.delete(
-            f"{self.bot_url}/channels/{channel_id}/messages/{message_id}"
+            f"{self._bot_url}/channels/{channel_id}/messages/{message_id}"
             f"?hidetip={str(hidetip).lower()}"
         )
         return await http_temp(return_, 200)
 
     async def get_guild_setting(self, guild_id: str) -> _api_model.get_guild_setting():
         """
         用于获取机器人在频道 guild_id 内的消息频率设置
 
         :param guild_id: 频道id
         :return: 返回的.data中为解析后的json数据
         """
         return_ = await self._session.get(
-            f"{self.bot_url}/guilds/{guild_id}/message/setting"
+            f"{self._bot_url}/guilds/{guild_id}/message/setting"
         )
         return await regular_temp(return_)
 
     async def create_dm_guild(
         self, target_id: str, guild_id: str
     ) -> _api_model.create_dm_guild():
         """
         当机器人主动跟用户私信时，创建并获取一个虚拟频道id的API
 
         :param target_id: 目标用户id
         :param guild_id: 机器人跟目标用户所在的频道id
         :return: 返回的.data中为解析后的json数据，注意发送私信仅需要使用guild_id这一项虚拟频道id的数据
         """
-        json_ = {"recipient_id": target_id, "source_guild_id": guild_id}
-        return_ = await self._session.post(f"{self.bot_url}/users/@me/dms", json=json_)
+        json_ = {"recipient_id": str(target_id), "source_guild_id": str(guild_id)}
+        return_ = await self._session.post(f"{self._bot_url}/users/@me/dms", json=json_)
         return await regular_temp(return_)
 
     async def send_dm(
         self,
         guild_id: str,
         content: Optional[str] = None,
         image: Optional[str] = None,
@@ -1137,105 +1188,117 @@
                 return sdk_error_temp(f"file_image不支持{type(file_image)}的内容")
             json_["file_image"] = file_image
             data_ = FormData_()
             for keys, values in json_.items():
                 if values is not None and keys != "image":
                     data_.add_field(keys, values)
             return_ = await self._session.post(
-                f"{self.bot_url}/dms/{guild_id}/messages", data=data_
+                f"{self._bot_url}/dms/{guild_id}/messages", data=data_
             )
         else:
             return_ = await self._session.post(
-                f"{self.bot_url}/dms/{guild_id}/messages", json=json_
+                f"{self._bot_url}/dms/{guild_id}/messages", json=json_
             )
         return await regular_temp(return_)
 
     async def delete_dm_msg(
         self, guild_id: str, message_id: str, hidetip: bool = False
     ) -> _api_model.delete_msg():
         """
         用于撤回私信频道 guild_id 中 message_id 指定的私信消息。只能用于撤回机器人自己发送的私信
 
         :param guild_id: 虚拟频道id（非子频道id），从用户主动私信机器人的事件、或机器人主动创建私信的API中获取
         :param message_id: 需撤回消息的消息id
         :param hidetip: 是否隐藏提示小灰条，True为隐藏，False为显示（选填）
         :return: 返回的.result显示是否成功
         """
-        self.check_warning("撤回私信消息")
+        self._check_warning("撤回私信消息")
         return_ = await self._session.delete(
-            f"{self.bot_url}/dms/{guild_id}/messages/{message_id}?"
+            f"{self._bot_url}/dms/{guild_id}/messages/{message_id}?"
             f"hidetip={str(hidetip).lower()}"
         )
         return await http_temp(return_, 200)
 
     async def mute_all_member(
         self,
         guild_id: str,
-        mute_end_timestamp: Optional[str],
-        mute_seconds: Optional[str],
+        mute_end_timestamp: Optional[str] = None,
+        mute_seconds: Optional[str] = None,
     ) -> _api_model.mute_member():
         """
         用于将频道的全体成员（非管理员）禁言
 
         :param guild_id: 频道id
         :param mute_end_timestamp: 禁言到期时间戳，绝对时间戳，单位：秒（与 mute_seconds 字段同时赋值的话，以该字段为准）
         :param mute_seconds: 禁言多少秒（两个字段二选一，默认以 mute_end_timestamp 为准）
         :return: 返回的.result显示是否成功
         """
-        json_ = {"mute_end_timestamp": mute_end_timestamp, "mute_seconds": mute_seconds}
+        json_ = {
+            "mute_end_timestamp": str(mute_end_timestamp)
+            if mute_end_timestamp is not None
+            else None,
+            "mute_seconds": str(mute_seconds) if mute_seconds is not None else None,
+        }
         return_ = await self._session.patch(
-            f"{self.bot_url}/guilds/{guild_id}/mute", json=json_
+            f"{self._bot_url}/guilds/{guild_id}/mute", json=json_
         )
         return await http_temp(return_, 204)
 
     async def mute_member(
         self,
         guild_id: str,
         user_id: str,
-        mute_end_timestamp: Optional[str],
-        mute_seconds: Optional[str],
+        mute_end_timestamp: Optional[str] = None,
+        mute_seconds: Optional[str] = None,
     ) -> _api_model.mute_member():
         """
         用于禁言频道 guild_id 下的成员 user_id
 
         :param guild_id: 频道id
         :param user_id: 目标成员的用户ID
         :param mute_end_timestamp: 禁言到期时间戳，绝对时间戳，单位：秒（与 mute_seconds 字段同时赋值的话，以该字段为准）
         :param mute_seconds: 禁言多少秒（两个字段二选一，默认以 mute_end_timestamp 为准）
         :return: 返回的.result显示是否成功
         """
-        json_ = {"mute_end_timestamp": mute_end_timestamp, "mute_seconds": mute_seconds}
+        json_ = {
+            "mute_end_timestamp": str(mute_end_timestamp)
+            if mute_end_timestamp is not None
+            else None,
+            "mute_seconds": str(mute_seconds) if mute_seconds is not None else None,
+        }
         return_ = await self._session.patch(
-            f"{self.bot_url}/guilds/{guild_id}/members/{user_id}/mute", json=json_
+            f"{self._bot_url}/guilds/{guild_id}/members/{user_id}/mute", json=json_
         )
         return await http_temp(return_, 204)
 
     async def mute_members(
         self,
         guild_id: str,
         user_id: List[str],
-        mute_end_timestamp: Optional[str],
-        mute_seconds: Optional[str],
+        mute_end_timestamp: Optional[str] = None,
+        mute_seconds: Optional[str] = None,
     ) -> _api_model.mute_members():
         """
         用于将频道的指定批量成员（非管理员）禁言
 
         :param guild_id: 频道id
         :param user_id: 目标成员的用户ID列表
         :param mute_end_timestamp: 禁言到期时间戳，绝对时间戳，单位：秒（与 mute_seconds 字段同时赋值的话，以该字段为准）
         :param mute_seconds: 禁言多少秒（两个字段二选一，默认以 mute_end_timestamp 为准）
         :return: 返回的.data中为解析后的json数据
         """
         json_ = {
-            "mute_end_timestamp": mute_end_timestamp,
-            "mute_seconds": mute_seconds,
+            "mute_end_timestamp": str(mute_end_timestamp)
+            if mute_end_timestamp is not None
+            else None,
+            "mute_seconds": str(mute_seconds) if mute_seconds is not None else None,
             "user_ids": user_id,
         }
         return_ = await self._session.patch(
-            f"{self.bot_url}/guilds/{guild_id}/mute", json=json_
+            f"{self._bot_url}/guilds/{guild_id}/mute", json=json_
         )
         trace_id = (
             return_.headers.get("X-Tps-Trace-Id", None)
             if hasattr(return_, "headers")
             else None
         )
         status_code = getattr(return_, "status", None)
@@ -1261,137 +1324,144 @@
                     "http_code": status_code,
                     "result": False,
                 }
             )
 
     async def create_announce(
         self,
-        guild_id,
+        guild_id: str,
         channel_id: Optional[str] = None,
         message_id: Optional[str] = None,
         announces_type: Optional[int] = None,
+        recommend_channels: Optional[List[model.AnnounceRecommendChannels]] = None,
         recommend_channels_id: Optional[List[str]] = None,
         recommend_channels_introduce: Optional[List[str]] = None,
     ) -> _api_model.create_announce():
         """
         用于创建频道全局公告，公告类型分为 消息类型的频道公告 和 推荐子频道类型的频道公告
 
         :param guild_id: 频道id
         :param channel_id: 子频道id，message_id 有值则为必填
         :param message_id: 消息id，此项有值则优选将某条消息设置为成员公告
         :param announces_type: 公告类别 0：成员公告，1：欢迎公告，默认为成员公告
-        :param recommend_channels_id: 推荐子频道id列表，会一次全部替换推荐子频道列表
-        :param recommend_channels_introduce: 推荐子频道推荐语列表，列表长度应与recommend_channels_id一致
+        :param recommend_channels: 推荐子频道id与推荐语的dict列表，会一次全部替换推荐子频道列表
+        :param recommend_channels_id: deprecated
+        :param recommend_channels_introduce: deprecated
         :return: 返回的.data中为解析后的json数据
         """
         json_ = {
-            "channel_id": channel_id,
+            "channel_id": str(channel_id) if channel_id is not None else None,
             "message_id": message_id,
             "announces_type": announces_type,
-            "recommend_channels": [],
+            "recommend_channels": recommend_channels,
         }
-        if recommend_channels_id is not None and recommend_channels_id:
-            if len(recommend_channels_id) == len(recommend_channels_introduce):
-                for i, items in enumerate(recommend_channels_id):
-                    json_["recommend_channels"].append(
-                        {
-                            "channel_id": items,
-                            "introduce": recommend_channels_introduce[i],
-                        }
-                    )
-            else:
-                return sdk_error_temp("注意推荐子频道ID列表长度，应与推荐子频道推荐语列表长度一致")
+        if (
+            recommend_channels_id
+            and recommend_channels_introduce
+            and not recommend_channels
+        ):
+            if recommend_channels_id is not None and recommend_channels_id:
+                if len(recommend_channels_id) == len(recommend_channels_introduce):
+                    for i, items in enumerate(recommend_channels_id):
+                        json_["recommend_channels"].append(
+                            model.AnnounceRecommendChannels(
+                                channel_id=items,
+                                introduce=recommend_channels_introduce[i],
+                            )
+                        )
+                else:
+                    return sdk_error_temp("注意推荐子频道ID列表长度，应与推荐子频道推荐语列表长度一致")
         return_ = await self._session.post(
-            f"{self.bot_url}/guilds/{guild_id}/announces", json=json_
+            f"{self._bot_url}/guilds/{guild_id}/announces", json=json_
         )
         return await regular_temp(return_)
 
     async def delete_announce(
         self, guild_id: str, message_id: str = "all"
     ) -> _api_model.delete_announce():
         """
         用于删除频道 guild_id 下指定 message_id 的全局公告
 
         :param guild_id: 频道id
         :param message_id: message_id有值时会校验message_id合法性；若不校验，请将message_id设置为all（默认为all）
         :return: 返回的.result显示是否成功
         """
         return_ = await self._session.delete(
-            f"{self.bot_url}/guilds/{guild_id}/announces/{message_id}"
+            f"{self._bot_url}/guilds/{guild_id}/announces/{message_id}"
         )
         return await http_temp(return_, 204)
 
     async def create_pinmsg(
         self, channel_id: str, message_id: str
     ) -> _api_model.pinmsg():
         """
         用于添加子频道 channel_id 内的精华消息
 
         :param channel_id: 子频道id
         :param message_id: 目标消息id
         :return: 返回的.data中为解析后的json数据
         """
         return_ = await self._session.put(
-            f"{self.bot_url}/channels/{channel_id}/pins/{message_id}"
+            f"{self._bot_url}/channels/{channel_id}/pins/{message_id}"
         )
         return await regular_temp(return_)
 
     async def delete_pinmsg(
         self, channel_id: str, message_id: str
     ) -> _api_model.delete_pinmsg():
         """
         用于删除子频道 channel_id 下指定 message_id 的精华消息
 
         :param channel_id: 子频道id
         :param message_id: 目标消息id
         :return: 返回的.result显示是否成功
         """
         return_ = await self._session.delete(
-            f"{self.bot_url}/channels/{channel_id}/pins/{message_id}"
+            f"{self._bot_url}/channels/{channel_id}/pins/{message_id}"
         )
         return await http_temp(return_, 204)
 
     async def get_pinmsg(self, channel_id: str) -> _api_model.pinmsg():
         """
         用于获取子频道 channel_id 内的精华消息
 
         :param channel_id: 子频道id
         :return: 返回的.data中为解析后的json数据
         """
-        return_ = await self._session.get(f"{self.bot_url}/channels/{channel_id}/pins")
+        return_ = await self._session.get(f"{self._bot_url}/channels/{channel_id}/pins")
         return await regular_temp(return_)
 
     async def get_schedules(
         self, channel_id: str, since: Optional[int] = None
     ) -> _api_model.get_schedules():
         """
         用于获取channel_id指定的子频道中当天的日程列表
 
         :param channel_id: 日程子频道id
         :param since: 起始时间戳(ms)
         :return: 返回的.data中为解析后的json数据
         """
         json_ = {"since": since}
         return_ = await self._session.get(
-            f"{self.bot_url}/channels/{channel_id}/schedules", json=json_
+            f"{self._bot_url}/channels/{channel_id}/schedules", json=json_
         )
         return await regular_temp(return_)
 
     async def get_schedule_info(
         self, channel_id: str, schedule_id: str
     ) -> _api_model.schedule_info():
         """
         获取日程子频道 channel_id 下 schedule_id 指定的的日程的详情
 
         :param channel_id: 日程子频道id
         :param schedule_id: 日程id
         :return: 返回的.data中为解析后的json数据
         """
         return_ = await self._session.get(
-            f"{self.bot_url}/channels/{channel_id}/schedules/{schedule_id}"
+            f"{self._bot_url}/channels/{channel_id}/schedules/{schedule_id}"
         )
         return await regular_temp(return_)
 
     async def create_schedule(
         self,
         channel_id: str,
         schedule_name: str,
@@ -1417,15 +1487,15 @@
                 "start_timestamp": start_timestamp,
                 "end_timestamp": end_timestamp,
                 "jump_channel_id": jump_channel_id,
                 "remind_type": remind_type,
             }
         }
         return_ = await self._session.post(
-            f"{self.bot_url}/channels/{channel_id}/schedules", json=json_
+            f"{self._bot_url}/channels/{channel_id}/schedules", json=json_
         )
         return await regular_temp(return_)
 
     async def patch_schedule(
         self,
         channel_id: str,
         schedule_id: str,
@@ -1453,30 +1523,30 @@
                 "start_timestamp": start_timestamp,
                 "end_timestamp": end_timestamp,
                 "jump_channel_id": jump_channel_id,
                 "remind_type": remind_type,
             }
         }
         return_ = await self._session.patch(
-            f"{self.bot_url}/channels/{channel_id}/schedules/{schedule_id}", json=json_
+            f"{self._bot_url}/channels/{channel_id}/schedules/{schedule_id}", json=json_
         )
         return await regular_temp(return_)
 
     async def delete_schedule(
         self, channel_id: str, schedule_id: str
     ) -> _api_model.delete_schedule():
         """
         用于删除日程子频道 channel_id 下 schedule_id 指定的日程
 
         :param channel_id: 日程子频道id
         :param schedule_id: 日程id
         :return: 返回的.result显示是否成功
         """
         return_ = await self._session.delete(
-            f"{self.bot_url}/channels/{channel_id}/schedules/{schedule_id}"
+            f"{self._bot_url}/channels/{channel_id}/schedules/{schedule_id}"
         )
         return await http_temp(return_, 204)
 
     async def create_reaction(
         self, channel_id: str, message_id: str, type_: str, id_: str
     ) -> _api_model.reactions():
         """
@@ -1485,15 +1555,15 @@
         :param channel_id: 子频道id
         :param message_id: 目标消息id
         :param type_: 表情类型
         :param id_: 表情id
         :return: 返回的.result显示是否成功
         """
         return_ = await self._session.put(
-            f"{self.bot_url}/channels/{channel_id}/messages/{message_id}/reactions/"
+            f"{self._bot_url}/channels/{channel_id}/messages/{message_id}/reactions/"
             f"{type_}/{id_}"
         )
         return await http_temp(return_, 204)
 
     async def delete_reaction(
         self, channel_id: str, message_id: str, type_: str, id_: str
     ) -> _api_model.reactions():
@@ -1503,15 +1573,15 @@
         :param channel_id: 子频道id
         :param message_id: 目标消息id
         :param type_: 表情类型
         :param id_: 表情id
         :return: 返回的.result显示是否成功
         """
         return_ = await self._session.delete(
-            f"{self.bot_url}/channels/{channel_id}/messages/{message_id}/reactions/"
+            f"{self._bot_url}/channels/{channel_id}/messages/{message_id}/reactions/"
             f"{type_}/{id_}"
         )
         return await http_temp(return_, 204)
 
     async def get_reaction_users(
         self, channel_id: str, message_id: str, type_: str, id_: str
     ) -> _api_model.get_reaction_users():
@@ -1521,15 +1591,15 @@
         :param channel_id: 子频道id
         :param message_id: 目标消息id
         :param type_: 表情类型
         :param id_: 表情id
         :return: 返回的.data中为解析后的json数据列表
         """
         return_ = await self._session.get(
-            f"{self.bot_url}/channels/{channel_id}/messages/{message_id}/reactions/"
+            f"{self._bot_url}/channels/{channel_id}/messages/{message_id}/reactions/"
             f"{type_}/{id_}?cookie=&limit=50"
         )
         trace_ids = [
             return_.headers.get("X-Tps-Trace-Id", None)
             if hasattr(return_, "headers")
             else None
         ]
@@ -1544,15 +1614,15 @@
                 for items in return_dict["users"]:
                     all_users.append(items)
                 results = [True]
                 while True:
                     if return_dict["is_end"]:
                         break
                     return_ = await self._session.get(
-                        f"{self.bot_url}/channels/{channel_id}/messages/{message_id}/"
+                        f"{self._bot_url}/channels/{channel_id}/messages/{message_id}/"
                         f'reactions/{type_}/{id_}?cookies={return_dict["cookie"]}'
                     )
                     trace_ids.append(return_.headers["X-Tps-Trace-Id"])
                     codes.append(return_.status)
                     return_dict = await return_.json()
                     if isinstance(return_dict, dict) and "code" in return_dict.keys():
                         results.append(False)
@@ -1594,50 +1664,50 @@
         :param status: 播放状态
         :param audio_url: 音频数据的url，可选，status为0时传
         :param text: 状态文本（比如：简单爱-周杰伦），可选，status为0时传，其他操作不传
         :return: 返回的.result显示是否成功
         """
         json_ = {"audio_url": audio_url, "text": text, "status": status}
         return_ = await self._session.post(
-            f"{self.bot_url}/channels/{channel_id}/audio", json=json_
+            f"{self._bot_url}/channels/{channel_id}/audio", json=json_
         )
         return await empty_temp(return_)
 
     async def bot_on_mic(self, channel_id: str) -> _api_model.audio():
         """
         机器人在 channel_id 对应的语音子频道上麦
 
         :param channel_id: 子频道id
         :return: 返回的.result显示是否成功
         """
-        return_ = await self._session.put(f"{self.bot_url}/channels/{channel_id}/mic")
+        return_ = await self._session.put(f"{self._bot_url}/channels/{channel_id}/mic")
         return await empty_temp(return_)
 
     async def bot_off_mic(self, channel_id: str) -> _api_model.audio():
         """
         机器人在 channel_id 对应的语音子频道下麦
 
         :param channel_id: 子频道id
         :return: 返回的.result显示是否成功
         """
         return_ = await self._session.delete(
-            f"{self.bot_url}/channels/{channel_id}/mic"
+            f"{self._bot_url}/channels/{channel_id}/mic"
         )
         return await empty_temp(return_)
 
     async def get_threads(self, channel_id: str) -> _api_model.get_threads():
         """
         获取子频道下的帖子列表
 
         :param channel_id: 目标论坛子频道id
         :return: 返回的.data中为解析后的json数据列表
         """
-        self.check_warning("获取帖子列表")
+        self._check_warning("获取帖子列表")
         return_ = await self._session.get(
-            f"{self.bot_url}/channels/{channel_id}/threads"
+            f"{self._bot_url}/channels/{channel_id}/threads"
         )
         trace_ids = [
             return_.headers.get("X-Tps-Trace-Id", None)
             if hasattr(return_, "headers")
             else None
         ]
         codes = [getattr(return_, "status", None)]
@@ -1658,15 +1728,15 @@
                         )
                     all_threads.append(items)
                 results = [True]
                 while True:
                     if return_dict["is_finish"]:
                         break
                     return_ = await self._session.get(
-                        f"{self.bot_url}/channels/{channel_id}/threads"
+                        f"{self._bot_url}/channels/{channel_id}/threads"
                     )
                     trace_ids.append(return_.headers["X-Tps-Trace-Id"])
                     codes.append(return_.status)
                     return_dict = await return_.json()
                     if isinstance(return_dict, dict) and "code" in return_dict.keys():
                         results.append(False)
                         all_threads.append(return_dict)
@@ -1706,71 +1776,71 @@
         """
         获取子频道下的帖子详情
 
         :param channel_id: 目标论坛子频道id
         :param thread_id: 帖子id
         :return: 返回的.data中为解析后的json数据
         """
-        self.check_warning("获取帖子详情")
+        self._check_warning("获取帖子详情")
         return_ = await self._session.get(
-            f"{self.bot_url}/channels/{channel_id}/threads/{thread_id}"
+            f"{self._bot_url}/channels/{channel_id}/threads/{thread_id}"
         )
         return await regular_temp(return_)
 
     async def create_thread(
-        self, channel_id: str, title: str, content: Union[str, dict], format_: int
+        self, channel_id: str, title: str, content: Union[str, Dict], format_: int
     ) -> _api_model.create_thread():
         """
         创建帖子，创建成功后，返回创建成功的任务ID
 
         :param channel_id: 目标论坛子频道id
         :param title: 帖子标题
         :param content: 帖子内容（具体格式根据format_判断）
         :param format_: 帖子文本格式（1：普通文本、2：HTML、3：Markdown、4：Json）
         :return: 返回的.data中为解析后的json数据
         """
-        self.check_warning("发表帖子")
+        self._check_warning("发表帖子")
         if isinstance(content, dict):
             json_ = {"title": title, "content": dumps(content), "format": format_}
         elif isinstance(content, str):
             json_ = {"title": title, "content": content, "format": format_}
         else:
             return sdk_error_temp("content参数类型错误，应为str或dict")
         return_ = await self._session.put(
-            f"{self.bot_url}/channels/{channel_id}/threads", json=json_
+            f"{self._bot_url}/channels/{channel_id}/threads", json=json_
         )
         return await regular_temp(return_)
 
     async def delete_thread(
         self, channel_id: str, thread_id: str
     ) -> _api_model.delete_thread():
         """
         删除指定子频道下的某个帖子
 
         :param channel_id: 目标论坛子频道id
         :param thread_id: 帖子id
         :return: 返回的.result显示是否成功
         """
-        self.check_warning("删除帖子")
+        self._check_warning("删除帖子")
         return_ = await self._session.delete(
-            f"{self.bot_url}/channels/{channel_id}/threads/{thread_id}"
+            f"{self._bot_url}/channels/{channel_id}/threads/{thread_id}"
         )
         return await http_temp(return_, 204)
 
     async def get_guild_permissions(
         self, guild_id: str
     ) -> _api_model.get_guild_permissions():
         """
         获取机器人在频道 guild_id 内可以使用的权限列表
 
         :param guild_id: 频道id
         :return: 返回的.data中为解析后的json数据
         """
         return_ = await self._session.get(
-            f"{self.bot_url}/guilds/{guild_id}/api_permission"
+            f"{self._bot_url}/guilds/{guild_id}/api_permission"
         )
         trace_id = (
             return_.headers.get("X-Tps-Trace-Id", None)
             if hasattr(return_, "headers")
             else None
         )
         status_code = getattr(return_, "status", None)
@@ -1815,15 +1885,15 @@
         :param desc: 机器人申请对应的API接口权限后可以使用功能的描述
         :return: 返回成功或不成功
         """
         path, method = _api_model.api_converter(api)
         if not path:
             return sdk_error_temp("目标API不存在，请检查API名称是否正确")
         json_ = {
-            "channel_id": channel_id,
+            "channel_id": str(channel_id),
             "api_identify": {"path": path, "method": method.upper()},
             "desc": desc,
         }
         return_ = await self._session.post(
-            f"{self.bot_url}/guilds/{guild_id}/api_permission/demand", json=json_
+            f"{self._bot_url}/guilds/{guild_id}/api_permission/demand", json=json_
         )
         return await empty_temp(return_)
```

### Comparing `qg-botsdk-2.7.0/qg_botsdk/http.py` & `qg-botsdk-3.0.0/qg_botsdk/http.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from asyncio import get_event_loop
 from ssl import create_default_context
 from typing import Optional
 
 from aiohttp import (
     ClientSession,
     ClientTimeout,
     FormData,
@@ -70,35 +71,64 @@
 
             self._writer.append_payload(part)
 
         self._is_processed = True
         return self._writer
 
 
+from asyncio import AbstractEventLoop
+
+
 class Session:
     def __init__(
-        self, loop, is_retry, is_log_error, logger, max_concurrency, timeout, **kwargs
+        self,
+        loop: AbstractEventLoop,
+        is_retry,
+        is_log_error,
+        logger,
+        max_concurrency,
+        timeout,
+        **kwargs,
     ):
         self._is_retry = is_retry
         self._is_log_error = is_log_error
         self._logger = logger
         self._queue = Queue(max_concurrency)
-        kwargs["connector"] = kwargs.get(
-            "connector",
-            TCPConnector(limit=0, ssl=create_default_context(), force_close=True),
-        )
+        if not kwargs.get("connector", None):
+            if not loop.is_running():
+                kwargs["connector"] = loop.run_until_complete(self._create_connector())
+            else:
+
+                def __callback(f):
+                    self._kwargs["connector"] = f.result()
+
+                loop.create_task(self._create_connector()).add_done_callback(__callback)
         self._kwargs = kwargs
         self._session: Optional[ClientSession] = None
         self._timeout = ClientTimeout(total=timeout)
         self._loop = loop
-        loop.run_until_complete(self._check_session())
+        if not loop.is_running():
+            loop.run_until_complete(self._check_session())
+        else:
+            loop.create_task(self._check_session())
 
     def __del__(self):
         if self._session and not self._session.closed:
-            self._loop.run_until_complete(self._session.close())
+            try:
+                loop = get_event_loop()
+                if loop.is_running():
+                    loop.create_task(self._session.close())
+                else:
+                    loop.run_until_complete(self._session.close())
+            except Exception:
+                pass
+
+    @staticmethod
+    async def _create_connector(*args, **kwargs):
+        return TCPConnector(*args, **kwargs)
 
     async def _check_session(self):
         if not self._session or self._session.closed:
             self._session = ClientSession(timeout=self._timeout, **self._kwargs)
 
     async def _warning(self, url, resp):
         self._logger.warning(
```

### Comparing `qg-botsdk-2.7.0/qg_botsdk/logger.py` & `qg-botsdk-3.0.0/qg_botsdk/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 from functools import wraps
 from logging import FileHandler, Formatter, StreamHandler, getLogger
 from os import PathLike, getcwd, makedirs, sep
 from os.path import exists, isdir, join
 from re import split as re_split
 from time import localtime, strftime
-from typing import List, Union
+from typing import Dict, List, Union
 
 try:
     from colorama import init as color_init
 
     color_init(strip=False)
 except (ImportError, ModuleNotFoundError):
     from os import system
@@ -30,14 +30,26 @@
         except UnicodeDecodeError:
             pass
 
     return wrap
 
 
 class Logger:
+    __instances = {}
+
+    def __new__(cls, *args, **kwargs):
+        bot_app_id = kwargs.get("bot_app_id", None) or args[0]
+        instance = cls.__instances.get(bot_app_id, None)
+        if instance:
+            return instance
+        else:
+            instance = super().__new__(cls)
+            cls.__instances[bot_app_id] = instance
+            return instance
+
     def __init__(
         self,
         bot_app_id: str,
         file_path: Union[str, PathLike] = None,
         disable_logger: List[str] = None,
     ):
         """
@@ -47,16 +59,17 @@
         :param file_path: 可选填，自定义log文件输出路径，不填默认为：当前目录/log/[bot_app_id]/
         :param disable_logger: 可选填，需要disable的logger名称列表，不填默认无
         """
         getLogger("asyncio").disabled = True
         if disable_logger:
             for items in disable_logger:
                 getLogger(items).disabled = True
-        self._bot_app_id = bot_app_id
-        self._logger = getLogger(__name__)
+        self.bot_app_id = str(bot_app_id)
+        self._logger = getLogger(self.bot_app_id)
+        self._logger.handlers.clear()
         self._logger.setLevel("DEBUG")
         self._format = "[%(asctime)s] [%(levelname)s] %(message)s"
         self._date_format = "%m-%d %H:%M:%S"
         self._cmdh = StreamHandler()
         self._cmdh.setFormatter(self._Stream_Formatter())
         self._cmdh.setLevel("INFO")
         self.file_path = file_path
@@ -64,15 +77,15 @@
             file_path = re_split(r"[\\|/]", file_path)
             if file_path[0] == ".":
                 self.file_path = join(*file_path)
             else:
                 file_path[0] += sep
                 self.file_path = join(sep, *file_path)
         else:
-            self.file_path = join(getcwd(), "log", self._bot_app_id)
+            self.file_path = join(getcwd(), "log", self.bot_app_id)
         if not exists(self.file_path):
             makedirs(self.file_path)
         assert isdir(self.file_path), "自定义Log输出路径必须为一个directory资料夹"
         self._logh = None
         self._new_logh(strftime("%m-%d", localtime()))
         self._logger.addHandler(self._cmdh)
         self._previous_time = strftime("%m-%d", localtime())
@@ -80,15 +93,15 @@
     class _Stream_Formatter(Formatter):
         FORMATS = {
             20: "\033[1;32m[%(asctime)s] [%(levelname)s]\033[0m %(message)s",
             30: "\033[1;33m[%(asctime)s] [%(levelname)s]\033[0m %(message)s",
             40: "\033[1;31m[%(asctime)s] [%(levelname)s]\033[0m %(message)s",
         }
 
-        def __init__(self, formats: dict = None, date_format: str = None):
+        def __init__(self, formats: Dict = None, date_format: str = None):
             super().__init__()
             if formats is not None:
                 self.FORMATS[20] = formats.get(20, None) or self.FORMATS[20]
                 self.FORMATS[30] = formats.get(30, None) or self.FORMATS[30]
                 self.FORMATS[40] = formats.get(40, None) or self.FORMATS[40]
             self._date_format = date_format or "%m-%d %H:%M:%S"
 
@@ -153,20 +166,20 @@
             join(self.file_path, f"{str_time}.log"), encoding="utf-8"
         )
         self._logh.setFormatter(Formatter(self._format, self._date_format))
         self._logger.addHandler(self._logh)
 
     @_log_wrapper
     def debug(self, msg):
-        self._logger.debug(msg)
+        self._logger.debug(str(msg))
 
     @_log_wrapper
     def info(self, msg):
-        self._logger.info(msg)
+        self._logger.info(str(msg))
 
     @_log_wrapper
     def warning(self, msg):
-        self._logger.warning(msg)
+        self._logger.warning(str(msg))
 
     @_log_wrapper
     def error(self, msg):
-        self._logger.error(msg)
+        self._logger.error(str(msg))
```

### Comparing `qg-botsdk-2.7.0/qg_botsdk/qg_bot.py` & `qg-botsdk-3.0.0/qg_botsdk/qg_bot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+import json
 from asyncio import Lock as ALock
-from asyncio import get_event_loop, new_event_loop, sleep
+from asyncio import get_event_loop, new_event_loop
 from importlib.machinery import SourceFileLoader
 from os import getpid
 from os.path import exists
 from os.path import split as path_split
 from re import Pattern
 from threading import Lock as TLock
 from time import sleep as t_sleep
-from typing import Any, Callable, List, Optional, Union
+from typing import Any, Callable, Iterable, List, Optional, Union
 
+from . import _exception
 from ._api_model import robot_model
-from ._utils import check_func
+from ._session import SessionManager
+from ._utils import func_type_checker
 from .api import API
 from .async_api import AsyncAPI
 from .http import Session
 from .logger import Logger
-from .model import Model
+from .model import BotCommandObject, Model
 from .plugins import Plugins
 from .qg_bot_ws import BotWs as _BotWs
+from .session import AbstractSessionManager, SessionPatcher
 from .version import __version__
 
 pid = getpid()
 print(f"本次程序进程ID：{pid} | SDK版本：{__version__} | 即将开始运行机器人……")
 t_sleep(0.5)
+json.JSONEncoder.default = lambda self, obj: (
+    obj.__json__() if hasattr(obj, "__json__") else str(obj)
+)
 
 
 class BOT:
     def __init__(
         self,
         bot_id: str,
         bot_token: str,
@@ -40,14 +47,15 @@
         is_retry: bool = True,
         is_log_error: bool = True,
         shard_no: int = 0,
         total_shard: int = 1,
         max_workers: int = 32,
         api_max_concurrency: int = 0,
         api_timeout: int = 20,
+        disable_reconnect_on_not_recv_msg: float = 1000,
     ):
         """
         机器人主体，输入BotAppID和密钥，并绑定函数后即可快速使用
 
         :param bot_id: 机器人平台后台BotAppID（开发者ID）项，必填
         :param bot_token: 机器人平台后台机器人令牌项，必填
         :param bot_secret: 机器人平台后台机器人密钥项（已废弃）
@@ -58,14 +66,15 @@
         :param is_retry: 使用api时，如遇可重试的错误码是否自动进行重试，默认开启
         :param is_log_error: 使用api时，如返回的结果为不成功，可自动log输出报错信息，默认开启
         :param shard_no: 当前分片数，如不熟悉相关配置请不要轻易改动此项，默认0
         :param total_shard: 最大分片数，如不熟悉相关配置请不要轻易改动此项，默认1
         :param max_workers: 在同步模式下，允许同时运行的最大线程数，默认32
         :param api_max_concurrency: API允许的最大并发数，超过此并发数将进入队列，如此数值<=0代表不开启任何队列，默认0
         :param api_timeout: API请求的超时设置。默认20
+        :param disable_reconnect_on_not_recv_msg: 当机器人长时间未收到消息后进行连接而非重连。默认1000秒
         """
         self.logger = Logger(bot_id)
         self.bot_id = bot_id
         self.bot_token = bot_token
         if bot_secret:
             raise DeprecationWarning(
                 "bot_secret已被废弃，如需使用安全接口，请通过security_setup()绑定小程序ID和secret"
@@ -75,15 +84,15 @@
             self.logger.info(
                 "已开启沙箱环境，发送消息时将频道方将自动添加[sandbox]字样，如需关闭请传参is_sandbox=False"
             )
             self.bot_url = r"https://sandbox.api.sgroup.qq.com"
         else:
             self.bot_url = r"https://api.sgroup.qq.com"
         if not bot_id or not bot_token:
-            raise type("IdTokenMissing", (Exception,), {})(
+            raise _exception.IdTokenMissing(
                 "你还没有输入 bot_id 和 bot_token，无法连接使用机器人\n如尚未有相关票据，"
                 "请参阅 https://qg-botsdk.readthedocs.io/zh_CN/latest/quick_start 了解相关详情"
             )
         try:
             self._loop = get_event_loop()
         except RuntimeError:
             self._loop = new_event_loop()
@@ -96,39 +105,51 @@
         self._on_start_function = None
         self.del_is_filter_self = True
         self.check_interval = 10
         self.__running = False
         self.__await_closure = False
         self.auth = f"Bot {bot_id}.{bot_token}"
         self.bot_headers = {"Authorization": self.auth}
-        self._session = Session(
+        self._http_session = Session(
             self._loop,
             is_retry,
             is_log_error,
             self.logger,
             api_max_concurrency,
             api_timeout,
             headers=self.bot_headers,
         )
         self.msg_treat = True
         self.dm_treat = False
         self.no_permission_warning = no_permission_warning
         self.max_workers = max_workers
         self.is_async = is_async
+        self.__session_manager = SessionManager(self.logger)
         self.api: Union[AsyncAPI, API] = AsyncAPI(
             self.bot_url,
-            self._session,
+            self._http_session,
             self.logger,
             self._check_warning,
+            self.__session_manager,
         )
         if not is_async:
             self.lock = TLock()
-            self.api = API(self.api, self._loop)
+            self.api = API(
+                self.api,
+                self._loop,
+                api_timeout,
+                self.__session_manager,
+            )
         else:
             self.lock = ALock()
+        self.__task = None
+        self._commands: List[BotCommandObject] = []
+        self._preprocessors: List[Callable[[Model.MESSAGE], Any]] = []
+        self.session: AbstractSessionManager = SessionPatcher()
+        self.disable_reconnect_on_not_recv_msg = disable_reconnect_on_not_recv_msg
 
     def __repr__(self):
         return f"<qg_botsdk.BOT object [id: {self.bot_id}, token: {self.bot_token}]>"
 
     @property
     def robot(self) -> robot_model():
         return self._bot_class.robot
@@ -164,60 +185,89 @@
                 if is_log:
                     self.logger.info("消息（所有消息）接收函数订阅成功")
             else:
                 self._intents = self._intents | 1 << 30
                 if is_log:
                     self.logger.info("消息（艾特消息）接收函数订阅成功")
 
-    def _get_plugins(self):
+    def _retrieve_new_plugins(self):
         commands, preprocessors = Plugins()
         if commands:
             for items in commands:
-                check_func(items["func"], Model.MESSAGE, is_async=self.is_async)
+                func_type_checker(items.func, Model.MESSAGE, is_async=self.is_async)
             self.__register_msg_intents()
         for func in preprocessors:
-            check_func(func, Model.MESSAGE, is_async=self.is_async)
+            func_type_checker(func, Model.MESSAGE, is_async=self.is_async)
         return commands, preprocessors
 
-    @staticmethod
-    def load_plugins(path_to_plugins: str):
+    def refresh_plugins(self):
+        commands, preprocessors = self._retrieve_new_plugins()
+        self._commands.extend(commands)
+        self._preprocessors.extend(preprocessors)
+
+    def clear_current_plugins(self):
+        self._commands.clear()
+        self._preprocessors.clear()
+
+    def remove_command(self, command_obj: BotCommandObject):
+        if command_obj in self._commands:
+            self._commands.remove(command_obj)
+        else:
+            raise ValueError(f"未找到指定的command {command_obj}")
+
+    def remove_preprocessors(self, preprocessor: Callable[[Model.MESSAGE], Any]):
+        if preprocessor in self._preprocessors:
+            self._preprocessors.remove(preprocessor)
+        else:
+            raise ValueError(f"未找到指定的preprocessor {preprocessor}")
+
+    @property
+    def get_current_commands(self) -> List[BotCommandObject]:
+        return self._commands[:]
+
+    @property
+    def get_current_preprocessors(self) -> List[Callable[[Model.MESSAGE], Any]]:
+        return self._preprocessors[:]
+
+    def load_plugins(self, path_to_plugins: str):
         """
         用于加载插件的.py程序
 
         :param path_to_plugins: 指向相应.py插件文件的相对或绝对路径
         :return:
         """
         if not exists(path_to_plugins):
             raise ModuleNotFoundError(f"指向plugin的路径 [{path_to_plugins}] 并不存在")
         if not path_to_plugins.endswith(".py"):
             path_to_plugins += ".py"
         _name = path_split(path_to_plugins)[1][:-3]
         try:
             SourceFileLoader(_name, path_to_plugins).load_module()
-            with open(path_to_plugins, "r", encoding="utf-8") as f:
-                exec(f.read())
         except Exception:
             raise ImportError(f"plugin [{path_to_plugins}] 导入失败")
+        if self._bot_class and self._bot_class.running:
+            self.refresh_plugins()
 
-    @staticmethod
-    def before_command():
+    def before_command(self):
         """
         注册预处理器，将在检查所有commands前执行
         """
 
-        def wrap(func: Model.MESSAGE):
+        def wrap(func: Callable[[Model.MESSAGE], Any]):
             Plugins.before_command()(func)
+            if self._bot_class and self._bot_class.running:
+                self.refresh_plugins()
             return func
 
         return wrap
 
-    @staticmethod
     def on_command(
-        command: Optional[Union[List[str], str]] = None,
-        regex: Optional[Union[Pattern, str]] = None,
+        self,
+        command: Optional[Union[Iterable[str], str]] = None,
+        regex: Optional[Union[Pattern, str, Iterable[Union[Pattern, str]]]] = None,
         is_treat: bool = True,
         is_require_at: bool = False,
         is_short_circuit: bool = True,
         is_custom_short_circuit: bool = False,
         is_require_admin: bool = False,
         admin_error_msg: Optional[str] = None,
     ):
@@ -225,30 +275,32 @@
         指令装饰器。用于快速注册消息事件，当连同bind_msg使用时，如没有触发短路，bind_msg注册的函数将在最后被调用
 
         :param command: 可触发事件的指令列表，与正则regex互斥，优先使用此项
         :param regex: 可触发指令的正则compile实例或正则表达式，与指令表互斥
         :param is_treat: 是否在treated_msg中同时处理指令，如正则将返回.groups()，默认是
         :param is_require_at: 是否要求必须艾特机器人才能触发指令，默认否
         :param is_short_circuit: 如果触发指令成功是否短路不运行后续指令（将根据注册顺序排序指令的短路机制），默认是
-        :param is_custom_short_circuit: 如果触发指令成功而返回True则不运行后续指令，与is_short_circuit不能同时存在，默认否
+        :param is_custom_short_circuit: 如果触发指令成功而回调函数返回True则不运行后续指令，存在时优先于is_short_circuit，默认否
         :param is_require_admin: 是否要求频道主或或管理才可触发指令，默认否
         :param admin_error_msg: 当is_require_admin为True，而触发用户的权限不足时，如此项不为None，返回此消息并短路；否则不进行短路
         """
 
-        def wrap(callback: Model.MESSAGE):
+        def wrap(callback: Callable[[Model.MESSAGE], Any]):
             Plugins.on_command(
                 command,
                 regex,
                 is_treat,
                 is_require_at,
                 is_short_circuit,
                 is_custom_short_circuit,
                 is_require_admin,
                 admin_error_msg,
             )(callback)
+            if self._bot_class and self._bot_class.running:
+                self.refresh_plugins()
             return callback
 
         return wrap
 
     def bind_msg(
         self,
         callback: Callable[[Model.MESSAGE], Any] = None,
@@ -260,15 +312,15 @@
 
         :param callback: 类型为function，该回调函数应包含一个参数以接收Object消息数据进行处理
         :param treated_data: 是否返回经转义处理的文本，如是则会在返回的Object中添加一个treated_msg的子类，默认True
         :param all_msg: 是否无视公私域限制，强制开启全部消息接收，默认None（不判断此项参数）
         """
 
         def wraps(func):
-            check_func(func, Model.MESSAGE, is_async=self.is_async)
+            func_type_checker(func, Model.MESSAGE, is_async=self.is_async)
             self._func_registers["on_msg"] = func
             if not treated_data:
                 self.msg_treat = False
             if all_msg is None:
                 self.__register_msg_intents()
             elif all_msg:
                 self._intents = self._intents | 1 << 9
@@ -290,19 +342,18 @@
         用作绑定接收私信消息的函数
 
         :param callback: 类型为function，该回调函数应包含一个参数以接收Object消息数据进行处理
         :param treated_data: 是否返回经转义处理的文本，如是则会在返回的Object中添加一个treated_msg的子类，默认True
         """
 
         def wraps(func):
-            check_func(func, Model.DIRECT_MESSAGE, is_async=self.is_async)
+            func_type_checker(func, Model.DIRECT_MESSAGE, is_async=self.is_async)
             self._func_registers["on_dm"] = func
             self._intents = self._intents | 1 << 12
-            if treated_data:
-                self.dm_treat = True
+            self.dm_treat = treated_data
             self.logger.info("私信接收函数订阅成功")
 
         if not callback:
             return wraps
         wraps(callback)
 
     def bind_msg_delete(
@@ -314,15 +365,15 @@
         用作绑定接收消息撤回事件的回调函数，注册时将自动根据公域私域注册艾特或全部消息，但不会主动注册私信事件
 
         :param callback:类型为function，该回调函数应包含一个参数以接收Object消息数据进行处理
         :param is_filter_self: 是否过滤用户自行撤回的消息，只接受管理撤回事件
         """
 
         def wraps(func):
-            check_func(func, Model.MESSAGE_DELETE, is_async=self.is_async)
+            func_type_checker(func, Model.MESSAGE_DELETE, is_async=self.is_async)
             self._func_registers["on_delete"] = func
             self._func_registers["del_is_filter_self"] = is_filter_self
             self.__register_msg_intents(False)
             self.logger.info("撤回事件订阅成功")
 
         if not callback:
             return wraps
@@ -332,15 +383,15 @@
         """
         用作绑定接收频道信息的函数
 
         :param callback: 类型为function，该回调函数应包含一个参数以接收Object消息数据进行处理
         """
 
         def wraps(func):
-            check_func(func, Model.GUILDS, is_async=self.is_async)
+            func_type_checker(func, Model.GUILDS, is_async=self.is_async)
             self._func_registers["on_guild_event"] = func
             self._intents = self._intents | 1
             self.logger.info("频道事件订阅成功")
 
         if not callback:
             return wraps
         wraps(callback)
@@ -349,15 +400,15 @@
         """
         用作绑定接收子频道信息的函数
 
         :param callback: 类型为function，该回调函数应包含一个参数以接收Object消息数据进行处理
         """
 
         def wraps(func):
-            check_func(func, Model.CHANNELS, is_async=self.is_async)
+            func_type_checker(func, Model.CHANNELS, is_async=self.is_async)
             self._func_registers["on_channel_event"] = func
             self._intents = self._intents | 1
             self.logger.info("子频道事件订阅成功")
 
         if not callback:
             return wraps
         wraps(callback)
@@ -366,15 +417,15 @@
         """
         用作绑定接收频道成员信息的函数
 
         :param callback: 类型为function，该回调函数应包含一个参数以接收Object消息数据进行处理
         """
 
         def wraps(func):
-            check_func(func, Model.GUILD_MEMBERS, is_async=self.is_async)
+            func_type_checker(func, Model.GUILD_MEMBERS, is_async=self.is_async)
             self._func_registers["on_guild_member"] = func
             self._intents = self._intents | 1 << 1
             self.logger.info("频道成员事件订阅成功")
 
         if not callback:
             return wraps
         wraps(callback)
@@ -383,15 +434,15 @@
         """
         用作绑定接收表情表态信息的函数
 
         :param callback: 类型为function，该回调函数应包含一个参数以接收Object消息数据进行处理
         """
 
         def wraps(func):
-            check_func(func, Model.REACTION, is_async=self.is_async)
+            func_type_checker(func, Model.REACTION, is_async=self.is_async)
             self._func_registers["on_reaction"] = func
             self._intents = self._intents | 1 << 10
             self.logger.info("表情表态事件订阅成功")
 
         if not callback:
             return wraps
         wraps(callback)
@@ -400,15 +451,15 @@
         """
         用作绑定接收互动事件的回调函数
 
         :param callback: 类型为function，该回调函数应包含一个参数以接收Object消息数据进行处理
         """
 
         def wraps(func):
-            check_func(func, Model.INTERACTION, is_async=self.is_async)
+            func_type_checker(func, Model.INTERACTION, is_async=self.is_async)
             self._func_registers["on_interaction"] = func
             self._intents = self._intents | 1 << 26
             self.logger.info("互动事件订阅成功")
 
         if not callback:
             return wraps
         wraps(callback)
@@ -417,15 +468,15 @@
         """
         用作绑定接收审核事件的回调函数
 
         :param callback: 类型为function，该回调函数应包含一个参数以接收Object消息数据进行处理
         """
 
         def wraps(func):
-            check_func(func, Model.MESSAGE_AUDIT, is_async=self.is_async)
+            func_type_checker(func, Model.MESSAGE_AUDIT, is_async=self.is_async)
             self._func_registers["on_audit"] = func
             self._intents = self._intents | 1 << 27
             self.logger.info("审核事件订阅成功")
 
         if not callback:
             return wraps
         wraps(callback)
@@ -437,15 +488,15 @@
         .. note::
             当前仅可以接收FORUM_THREAD_CREATE、FORUM_THREAD_UPDATE、FORUM_THREAD_DELETE三个事件
 
         :param callback: 类型为function，该回调函数应包含一个参数以接收Object消息数据进行处理
         """
 
         def wraps(func):
-            check_func(func, Model.FORUMS_EVENT, is_async=self.is_async)
+            func_type_checker(func, Model.FORUMS_EVENT, is_async=self.is_async)
             self._func_registers["on_forum"] = func
             self._intents = self._intents | 1 << 28
             self.logger.info("论坛事件订阅成功")
             if not self.is_private and self.no_permission_warning:
                 self.logger.warning("请注意，一般公域机器人并不能注册论坛事件，请检查自身是否拥有相关权限")
 
         if not callback:
@@ -459,15 +510,15 @@
         .. note::
             当前仅可以接收OPEN_FORUM_THREAD_CREATE、OPEN_FORUM_THREAD_UPDATE、OPEN_FORUM_THREAD_DELETE三个事件
 
         :param callback: 类型为function，该回调函数应包含一个参数以接收Object消息数据进行处理
         """
 
         def wraps(func):
-            check_func(func, Model.OPEN_FORUMS, is_async=self.is_async)
+            func_type_checker(func, Model.OPEN_FORUMS, is_async=self.is_async)
             self._func_registers["on_open_forum"] = func
             self._intents = self._intents | 1 << 18
             self.logger.info("论坛事件订阅成功")
 
         if not callback:
             return wraps
         wraps(callback)
@@ -476,15 +527,15 @@
         """
         用作绑定接收论坛事件的回调函数
 
         :param callback: 类型为function，该回调函数应包含一个参数以接收Object消息数据进行处理
         """
 
         def wraps(func):
-            check_func(func, Model.AUDIO_ACTION, is_async=self.is_async)
+            func_type_checker(func, Model.AUDIO_ACTION, is_async=self.is_async)
             self._func_registers["on_audio"] = func
             self._intents = self._intents | 1 << 29
             self.logger.info("音频事件订阅成功")
             if self.no_permission_warning:
                 self.logger.warning("请注意，一般机器人并不能注册音频事件（需先进行申请），请检查自身是否拥有相关权限")
 
         if not callback:
@@ -498,15 +549,15 @@
         """
         用作绑定接收音视频/直播子频道成员进出事件的回调函数
 
         :param callback: 类型为function，该回调函数应包含一个参数以接收Object消息数据进行处理
         """
 
         def wraps(func):
-            check_func(func, Model.LIVE_CHANNEL_MEMBER, is_async=self.is_async)
+            func_type_checker(func, Model.LIVE_CHANNEL_MEMBER, is_async=self.is_async)
             self._func_registers["on_live_channel_member"] = func
             self._intents = self._intents | 1 << 19
             self.logger.info("音视频/直播子频道成员进出事件订阅成功")
 
         if not callback:
             return wraps
         wraps(callback)
@@ -520,15 +571,15 @@
         用作注册重复事件的回调函数，注册并开始机器人后，会根据间隔时间不断调用该回调函数
 
         :param time_function: 类型为function，该函数不应包含任何参数
         :param check_interval: 每多少秒检查调用一次时间事件函数，默认10
         """
 
         def wraps(func):
-            check_func(func, is_async=self.is_async)
+            func_type_checker(func, is_async=self.is_async)
             self._repeat_function = func
             self.check_interval = check_interval
             self.logger.info("重复运行事件注册成功")
 
         if not time_function:
             return wraps
         wraps(time_function)
@@ -537,15 +588,15 @@
         """
         用作注册机器人开始时运行的函数，此函数不应有无限重复的内容，会在机器人完成登录后调用该回调函数
 
         :param on_start_function: 类型为function，该函数不应包含任何参数
         """
 
         def wraps(func):
-            check_func(func, is_async=self.is_async)
+            func_type_checker(func, is_async=self.is_async)
             self._on_start_function = func
             self.logger.info("初始事件注册成功")
 
         if not on_start_function:
             return wraps
         wraps(on_start_function)
 
@@ -576,28 +627,28 @@
 
         :param is_blocking: 机器人是否阻塞运行，如选择False，机器人将以异步任务的方式非阻塞性运行，如不熟悉异步编程请不要使用此项
         """
         try:
             if not self.__running and not self._bot_class:
                 self.__running = True
                 gateway = self._loop.run_until_complete(
-                    self._session.get(f"{self.bot_url}/gateway/bot")
+                    self._http_session.get(f"{self.bot_url}/gateway/bot")
                 )
                 gateway = self._loop.run_until_complete(gateway.json())
                 url = gateway.get("url")
                 if not url:
-                    raise type("IdTokenError", (Exception,), {})(
+                    raise _exception.IdTokenError(
                         "你输入的 bot_id 和/或 bot_token 错误，无法连接使用机器人\n如尚未有相关票据，"
                         "请参阅 https://qg-botsdk.readthedocs.io/zh_CN/latest/quick_start 了解相关详情"
                     )
                 self.logger.debug("[机器人ws地址] " + url)
-                commands, preprocessors = self._get_plugins()
+                self.refresh_plugins()
                 self._bot_class = _BotWs(
                     self._loop,
-                    self._session,
+                    self._http_session,
                     self.logger,
                     self._total_shard,
                     self._shard_no,
                     url,
                     self.auth,
                     self._func_registers,
                     self._intents,
@@ -605,34 +656,38 @@
                     self.dm_treat,
                     self._on_start_function,
                     self.check_interval,
                     self._repeat_function,
                     self.is_async,
                     self.max_workers,
                     self.api,
-                    commands,
-                    preprocessors,
+                    self._commands,
+                    self._preprocessors,
+                    self.disable_reconnect_on_not_recv_msg,
+                    self.__session_manager,
                 )
-                self._loop.create_task(self._bot_class.starter())
-                if is_blocking:
-
-                    self._loop.run_forever()
+                self.__task = self._loop.create_task(self._bot_class.starter())
+                if is_blocking and not self._loop.is_running():
+                    self._loop.run_until_complete(self.__task)
             else:
                 self.logger.error("当前机器人已在运行中！")
         except KeyboardInterrupt:
             self.logger.info("结束运行机器人（KeyboardInterrupt）")
             exit()
 
     def block(self):
         """
         当BOT.start()选择is_blocking=False的非阻塞性运行时，此函数能在后续阻塞主进程而继续运行机器人
         """
         try:
             if self.__running or self.__await_closure:
-                self._loop.run_forever()
+                if self.__task and not self._loop.is_running():
+                    self._loop.run_until_complete(self.__task)
+                    return
+            self.logger.error("当前机器人没有运行！")
         except KeyboardInterrupt:
             self.logger.info("结束运行机器人（KeyboardInterrupt）")
             exit()
 
     def close(self):
         """
         结束运行机器人的函数
@@ -642,18 +697,10 @@
             https://qg-botsdk.readthedocs.io/zh_CN/latest/index.html
         """
         if self.__running:
             self.__await_closure = True
             self.__running = False
             self.logger.info("WS链接已开始结束进程，请等待另一端完成握手并等待 TCP 连接终止")
             self._bot_class.running = False
-            timeout = self._loop.time() + 60
-            while self._loop.time() < timeout:
-                t_sleep(1)
-                if not self._bot_class or self._bot_class.ws.closed:
-                    self.__await_closure = False
-                    return
-            self._bot_class = None
-            self.logger.info("判断超时，WS链接已强制结束")
-            self.__await_closure = False
+            self._loop.create_task(self._bot_class.close())
         else:
             self.logger.error("当前机器人没有运行！")
```

### Comparing `qg-botsdk-2.7.0/qg_botsdk/qg_bot_ws.py` & `qg-botsdk-3.0.0/qg_botsdk/qg_bot_ws.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,72 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from asyncio import AbstractEventLoop, all_tasks, sleep
+from asyncio import AbstractEventLoop
+from asyncio import TimeoutError as AsyncTimeoutError
+from asyncio import all_tasks, sleep
 from concurrent.futures import ThreadPoolExecutor
 from copy import copy, deepcopy
 from json import dumps, loads
 from ssl import create_default_context
-from typing import Any, Callable, Union
-from unittest.mock import PropertyMock, patch
+from typing import Any, Callable, Dict, List, Union
 
 from aiohttp import ClientSession, WSMsgType, WSServerHandshakeError
 
-from ._api_model import Bot_Command_Obj
+from ._session import SessionManager
 from ._statics import EVENTS
 from ._utils import (
     exception_handler,
     exception_processor,
     object_class,
     objectize,
     treat_msg,
     treat_thread,
 )
 from .api import API
 from .async_api import AsyncAPI
 from .http import Session
 from .logger import Logger
-from .model import Model
-from .plugins import Plugins
+from .model import BotCommandObject, Model
+
+Op9RetryTime = 2
 
 
 class BotWs:
     def __init__(
         self,
         loop: AbstractEventLoop,
-        session: Session,
+        http_session: Session,
         logger: Logger,
         total_shard: int,
         shard_no: int,
         ws_url: str,
         auth: str,
-        func_registers: dict,
+        func_registers: Dict,
         intents: int,
         msg_treat: bool,
         dm_treat: bool,
         on_start_function: Callable[[], Any],
         check_interval: int,
         repeat_function: Callable[[], Any],
         is_async: bool,
         max_workers: int,
         api: Union[AsyncAPI, API],
-        commands: list[Bot_Command_Obj],
-        preprocessors: list[Model.MESSAGE],
+        commands: List[BotCommandObject],
+        preprocessors: List[Callable[[Model.MESSAGE], Any]],
+        disable_reconnect_on_not_recv_msg: float,
+        session_manager: SessionManager,
     ):
         """
         此为SDK内部使用类，注册机器人请使用from qg_botsdk.qg_bot import BOT
 
         .. seealso::
             更多教程和相关资讯可参阅：
             https://qg-botsdk.readthedocs.io/zh_CN/latest/快速入门.html
         """
-        self.session = session
+        self.http_session = http_session
         self._ssl = create_default_context()
         self.logger = logger
         self.total_shard = total_shard
         self.shard_no = shard_no
         self.ws_url = ws_url
         self.auth = auth
         self.on_start_function = on_start_function
@@ -112,15 +116,19 @@
                 )
             ),
         }
         self.threads = ThreadPoolExecutor(max_workers) if not self.is_async else None
         self.api = api
         self.commands = commands
         self.preprocessors = preprocessors
+        self.session_manager = session_manager
         self.at = "<@!%s>"
+        self.disable_reconnect = False
+        self.disable_reconnect_on_not_recv_msg = disable_reconnect_on_not_recv_msg
+        self.skip_connect_waiting = False
 
     @exception_processor
     async def _time_event_run(self):
         if self.is_async:
             self.loop.create_task(self.repeat_function())
         else:
             self.threads.submit(self.repeat_function)
@@ -133,17 +141,19 @@
     async def _start_event(self):
         self.is_first_run = True
         self.robot = await self.get_robot_info()
         self.at = self.at % self.robot.id
         self.logger.info(f"机器人频道用户ID：{self.robot.id}")
         if self.on_start_function is not None:
             if self.is_async:
-                self.loop.create_task(self.on_start_function())
+                self.loop.create_task(
+                    self.async_start_callback_task(self.on_start_function)
+                )
             else:
-                self.threads.submit(self.start_task, self.on_start_function)
+                self.threads.submit(self.start_callback_task, self.on_start_function)
         if self.repeat_function is not None:
             self.loop.create_task(self._time_event_check())
 
     async def send_connect(self):
         connect_paras = {
             "op": 2,
             "d": {
@@ -174,48 +184,46 @@
                 await self.ws.send_str(dumps(heart_json))
 
     def start_heartbeat(self):
         if self.heartbeat is None or self.heartbeat not in all_tasks():
             self.heartbeat = self.loop.create_task(self.heart())
 
     async def get_robot_info(self, retry=False):
-        robot_info = await self.session.get(r"https://api.sgroup.qq.com/users/@me")
+        robot_info = await self.http_session.get(r"https://api.sgroup.qq.com/users/@me")
         robot_info = await robot_info.json()
         if "id" not in robot_info:
             if not retry:
                 return self.get_robot_info(retry)
             else:
                 self.logger.error("当前获取机器人信息失败，机器人启动失败，程序将退出运行（可重试）")
                 exit()
         return objectize(robot_info)
 
     @exception_processor
-    async def async_start_task(self, func, *args):
-        with patch.object(Plugins, "api", new_callable=PropertyMock) as mock_api:
-            mock_api.return_value = self.api
-            await func(*args)
+    async def async_start_callback_task(self, func, *args):
+        return await func(*args)
 
     @exception_processor
-    def start_task(self, func, *args):
-        with patch.object(Plugins, "api", new_callable=PropertyMock) as mock_api:
-            mock_api.return_value = self.api
-            func(*args)
+    def start_callback_task(self, func, *args):
+        return func(*args)
 
     @exception_processor
     async def distribute(
-        self, function, data: dict = None, objectized_data: object_class = None
+        self, function, data: Dict = None, objectized_data: object_class = None
     ):
         if function:
             if not objectized_data:
                 objectized_data = objectize(data.get("d", {}), self.api, self.is_async)
             if not self.is_async:
-                return self.threads.submit(self.start_task, function, objectized_data)
+                return self.threads.submit(
+                    self.start_callback_task, function, objectized_data
+                )
             else:
                 return self.loop.create_task(
-                    self.async_start_task(function, objectized_data)
+                    self.async_start_callback_task(function, objectized_data)
                 )
 
     @exception_processor
     def treat_command(
         self, objectized_data: Model.MESSAGE, treated_msg, command=None, regex=None
     ):
         if self.msg_treat:
@@ -237,84 +245,117 @@
         return objectized_data
 
     @exception_processor
     async def check_command(
         self,
         objectized_data: Model.MESSAGE,
         treated_msg: str,
-        command_obj: Bot_Command_Obj,
+        command_obj: BotCommandObject,
         **kwargs,
     ):
-        # command: {command or regex, func, treat, at, short_circuit, admin, admin_error_msg}
-        if command_obj["admin"]:
+        if command_obj.admin:
             try:
                 roles = objectized_data.member.roles
             except Exception:
                 command_str = kwargs.get("command") or getattr(
                     kwargs.get("regex"), "pattern", None
                 )
                 self.logger.error(
                     f"cannot check roles of member for admin command: {command_str}"
                 )
                 return False
             if "2" not in roles and "4" not in roles:  # if not admin
-                if command_obj["admin_error_msg"]:
+                if command_obj.admin_error_msg:
                     if self.is_async:
                         self.loop.create_task(
                             objectized_data.reply(
-                                command_obj["admin_error_msg"],
+                                command_obj.admin_error_msg,
                             )
                         )
                     else:
                         self.threads.submit(
                             objectized_data.reply,
-                            command_obj["admin_error_msg"],
+                            command_obj.admin_error_msg,
                         )
                     return True
                 return False
-        if command_obj["treat"] and self.msg_treat:
+        if command_obj.treat:
             objectized_data = self.treat_command(objectized_data, treated_msg, **kwargs)
-            task = await self.distribute(
-                command_obj["func"], objectized_data=objectized_data
-            )
-            if not command_obj["is_custom_short_circuit"]:
-                return command_obj["short_circuit"]  # True or False
+        task = await self.distribute(command_obj.func, objectized_data=objectized_data)
+        if not command_obj.is_custom_short_circuit:
+            return command_obj.short_circuit  # True or False
+        else:
+            while not task.done():
+                await sleep(0.1)
+            r = task.result()
+            return r  # True or False
+
+    def process_wait_for_commands(self, objectized_data, msg, treated_msg):
+        wait_for_commands = self.session_manager.wait_for_message_checker(
+            objectized_data
+        )
+        for x in wait_for_commands:
+            commands = x.command.command
+            regexs = x.command.regex
+            if commands:
+                for command in commands:
+                    if command in msg and (not x.command.at or self.at in msg):
+                        if x.command.treat:
+                            objectized_data = self.treat_command(
+                                objectized_data, treated_msg, command=command
+                            )
+                        x.callback(objectized_data)
+                        if x.command.short_circuit:
+                            return True
+                        break
             else:
-                while not task.done():
-                    await sleep(0.5)
-                return task.result()  # True or False
+                for regex in regexs:
+                    regex = regex.search(msg)
+                    if regex and (not x.command.at or self.at in msg):
+                        if x.command.treat:
+                            objectized_data = self.treat_command(
+                                objectized_data, treated_msg, regex=regex
+                            )
+                        x.callback(objectized_data)
+                        if x.command.short_circuit:
+                            return True
+                        break
+        return False
 
     @exception_processor
-    async def distribute_commands(self, data: dict, treated_msg: str):
+    async def distribute_commands(self, data: Dict, treated_msg: str):
         objectized_data = objectize(data.get("d", {}), self.api, self.is_async)
         # run preprocessors
         for func in self.preprocessors:
             await self.distribute(func, objectized_data=objectized_data)
         # check commands
         msg = data.get("d", {}).get("content", "")
-        # commands = [{command or regex, func, treat, at, short_circuit, admin, admin_error_msg}]
+        if self.process_wait_for_commands(objectized_data, msg, treated_msg):
+            return True
         for items in self.commands:
-            commands = items.get("command", [])
+            commands = items.command
+            regexs = items.regex
             if commands:
                 for command in commands:
-                    if command in msg and (not items["at"] or self.at in msg):
+                    if command in msg and (not items.at or self.at in msg):
                         if await self.check_command(
                             objectized_data, treated_msg, items, command=command
                         ):
                             return True
             else:
-                regex = items.get("regex").search(msg)
-                if regex and (not items["at"] or self.at in msg):
-                    if await self.check_command(
-                        objectized_data, treated_msg, items, regex=regex
-                    ):
-                        return True
+                for regex in regexs:
+                    regex = regex.search(msg)
+                    if regex and (not items.at or self.at in msg):
+                        if await self.check_command(
+                            objectized_data, treated_msg, items, regex=regex
+                        ):
+                            return True
 
     @exception_processor
-    async def data_process(self, data: dict):
+    async def data_process(self, data: Dict):
         # initialize values
         t = data.get("t")
         d = data.get("d", {})
         if not d:
             data["d"] = d
         data["d"]["t"] = t
         data["d"]["event_id"] = data.get("id")
@@ -355,19 +396,15 @@
         op = data.get("op")
         if "s" in data:
             self.s = data["s"]
         if op == 11:
             self.logger.debug("心跳发送成功")
         elif op == 9:
             self.logger.error("[错误] op9参数出错（一般此报错为传递了无权限的事件订阅，请检查是否有权限订阅相关事件）")
-            await sleep(3)
-            if not self.is_reconnect:
-                await self.send_connect()
-            else:
-                await self.send_reconnect()
+            self.disable_reconnect = True
         elif op == 10:
             self.heartbeat_time = (
                 int(data.get("d", {}).get("heartbeat_interval", 40)) * 0.001
             )
             if not self.is_reconnect:
                 await self.send_connect()
             else:
@@ -384,32 +421,49 @@
             elif t == "RESUMED":
                 self.reconnect_times = 0
                 self.start_heartbeat()
                 self.logger.info("重连成功，机器人继续运行")
             else:
                 await self.data_process(data)
 
+    async def close(self):
+        if self.heartbeat is not None and not self.heartbeat.cancelled():
+            self.heartbeat.cancel()
+        await self.ws.close()
+        self.logger.info("WS链接已结束")
+
     async def connect(self):
         self.reconnect_times += 1
         try:
             async with ClientSession() as ws_session:
                 async with ws_session.ws_connect(self.ws_url, ssl=self._ssl) as self.ws:
                     while not self.ws.closed:
-                        message = await self.ws.receive()
-                        if not self.running:
+                        try:
+                            message = await self.ws.receive(
+                                timeout=self.disable_reconnect_on_not_recv_msg
+                            )
+                        except AsyncTimeoutError:
+                            self.logger.warning("BOT_WS链接已断开，正在尝试重连……")
                             if (
                                 self.heartbeat is not None
                                 and not self.heartbeat.cancelled()
                             ):
                                 self.heartbeat.cancel()
-                            await self.ws.close()
-                            self.logger.info("WS链接已结束")
+                            self.disable_reconnect = True
+                            self.skip_connect_waiting = True
+                            return
+                        if not self.running:
+                            if not not self.ws.closed:
+                                await self.close()
                             return
                         if message.type == WSMsgType.TEXT:
                             self.loop.create_task(self.dispatch_events(message.data))
+                            if self.disable_reconnect:
+                                await self.ws.close()
+                                return
                         elif message.type in (
                             WSMsgType.CLOSE,
                             WSMsgType.CLOSED,
                             WSMsgType.ERROR,
                         ):
                             if self.running:
                                 self.is_reconnect = True
@@ -420,20 +474,27 @@
                                     self.heartbeat.cancel()
                                 self.logger.warning("BOT_WS链接已断开，正在尝试重连……")
                                 return
         except Exception as e:
             self.logger.warning("BOT_WS链接已断开，正在尝试重连……")
             if self.heartbeat is not None and not self.heartbeat.cancelled():
                 self.heartbeat.cancel()
-            self.logger.error(e)
-            self.logger.debug(exception_handler(e))
+            self.logger.error(repr(e))
+            self.logger.error(exception_handler(e))
             return
 
     async def starter(self):
+        self.session_manager.start(self.loop)
         await self.connect()
         while self.running:
-            self.is_reconnect = self.reconnect_times < 20
+            if self.disable_reconnect:
+                if not self.skip_connect_waiting:
+                    await sleep(Op9RetryTime)
+                self.skip_connect_waiting = False
+                self.disable_reconnect = False
+                self.is_reconnect = False
             try:
                 await self.connect()
             except WSServerHandshakeError:
                 self.logger.warning("网络连线不稳定或已断开，请检查网络链接")
-            await sleep(5)
+            await sleep(3)
+            self.is_reconnect = self.reconnect_times < 20
```

### Comparing `qg-botsdk-2.7.0/qg_botsdk/utils.py` & `qg-botsdk-3.0.0/qg_botsdk/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+from io import IOBase
 from typing import Any, Dict, Tuple, Union
 
 try:
     from yaml import safe_load
 except (ImportError, ModuleNotFoundError):
     safe_load = None
 
 
-def read_yaml(yaml_path) -> Dict[str, Any]:
+def read_yaml(target: Union[str, IOBase], encoding: str = "utf-8") -> Dict[str, Any]:
     if not safe_load:
         raise AssertionError("如需使用read_yaml函数，必须先pip install pyyaml")
-    with open(yaml_path, "r", encoding="utf-8") as f:
-        return safe_load(f)
+    if isinstance(target, str):
+        with open(target, "r", encoding=encoding) as f:
+            return safe_load(f)
+    elif isinstance(target, IOBase):
+        return safe_load(target)
+    else:
+        raise TypeError("target应为str或IO")
 
 
 def convert_color(color: Union[Tuple[int, int, int], str]):
     colors = []
     if isinstance(color, tuple):
         if len(color) == 3:
             for items in color:
```

### Comparing `qg-botsdk-2.7.0/qg_botsdk.egg-info/PKG-INFO` & `qg-botsdk-3.0.0/qg_botsdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qg-botsdk
-Version: 2.7.0
+Version: 3.0.0
 Summary: easy-to-use SDK for Tencent QQ guild robot
 Home-page: https://github.com/GLGDLY/qg_botsdk
 Author: GDLY
 Author-email: tzlgdly@gmail.com
 Keywords: sample,example,setuptools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,14 +39,18 @@
 为此，qg_botsdk相应提供了另一个选择，这一款sdk虽然同样使用asyncio编写sdk底层，但其同时提供了threading和asyncio封装下的应用层调用，以抽象化封装的库编写方式，极大地降低应用层的开发难度。
 
 
 
 亮点
 =====
 
+-   两种应用层开发方式（threading、asyncio），可根据自己的喜好选择，而底层均为asyncio实现，保持高并发能力
+
+-   高覆盖率的单元测试，保证SDK的稳定性
+
 -   灵活的构建方式，即使官方删除或新增字段，SDK也不会规范于原来的数据格式，而会把真实数据反馈给你
 
 -   轻量，简洁，统一的代码结构，通过录入回调函数处理不同事件，10行即可构建一个简单的程序
 
 -   容易入门，无需学会asyncio、类继承等编程技巧也可使用，同时保留较高并发能力
 
 -   保留官方http API中Json数据的结构字段，带你学习官方结构，日后可自行开发适合自己的SDK
```

