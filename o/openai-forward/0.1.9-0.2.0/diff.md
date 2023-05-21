# Comparing `tmp/openai_forward-0.1.9.tar.gz` & `tmp/openai_forward-0.2.0.tar.gz`

## Comparing `openai_forward-0.1.9.tar` & `openai_forward-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.9/openai_forward/__init__.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 openai_forward-0.1.9/openai_forward/__main__.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 openai_forward-0.1.9/openai_forward/app.py
--rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 openai_forward-0.1.9/openai_forward/base.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 openai_forward-0.1.9/openai_forward/config.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 openai_forward-0.1.9/openai_forward/openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.9/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 openai_forward-0.1.9/openai_forward/content/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.9/openai_forward/content/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.9/openai_forward/routers/__init__.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 openai_forward-0.1.9/openai_forward/routers/openai_v1.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openai_forward-0.1.9/openai_forward/routers/schemas.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 openai_forward-0.1.9/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.9/LICENSE
--rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 openai_forward-0.1.9/README.md
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 openai_forward-0.1.9/pyproject.toml
--rw-r--r--   0        0        0    10064 2020-02-02 00:00:00.000000 openai_forward-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/__init__.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/__main__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/app.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/base.py
+-rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/config.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/content/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/content/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 openai_forward-0.2.0/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 openai_forward-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 openai_forward-0.2.0/README.md
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 openai_forward-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 openai_forward-0.2.0/PKG-INFO
```

### Comparing `openai_forward-0.1.9/openai_forward/__main__.py` & `openai_forward-0.2.0/openai_forward/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+import os
+
 import fire
 import uvicorn
-import os
 
 
 class Cli:
     @staticmethod
-    def run(port=8000,
-            workers=1,
-            api_key=None,
-            forward_key=None,
-            base_url=None,
-            log_chat=None,
-            route_prefix=None,
-            ip_whitelist=None,
-            ip_blacklist=None,
-            ):
-        """ Run forwarding serve.
+    def run(
+        port=8000,
+        workers=1,
+        api_key=None,
+        forward_key=None,
+        base_url=None,
+        log_chat=None,
+        route_prefix=None,
+        ip_whitelist=None,
+        ip_blacklist=None,
+    ):
+        """Run forwarding serve.
 
         Parameters
         ----------
 
         port: int, default 8000
         workers: int, 1
         api_key: str, None
@@ -41,22 +43,24 @@
         if route_prefix:
             os.environ['ROUTE_PREFIX'] = route_prefix
         if ip_whitelist:
             os.environ['IP_WHITELIST'] = ip_whitelist
         if ip_blacklist:
             os.environ['IP_BLACKLIST'] = ip_blacklist
 
+        ssl_keyfile = os.environ.get("ssl_keyfile", None) or None
+        ssl_certfile = os.environ.get("ssl_certfile", None) or None
         uvicorn.run(
             app="openai_forward.app:app",
             host="0.0.0.0",
             port=port,
             workers=workers,
             app_dir='..',
-            ssl_keyfile=os.environ.get("ssl_keyfile", None),
-            ssl_certfile=os.environ.get("ssl_certfile", None),
+            ssl_keyfile=ssl_keyfile,
+            ssl_certfile=ssl_certfile,
         )
 
 
 def main():
     fire.Fire(Cli)
```

### Comparing `openai_forward-0.1.9/openai_forward/base.py` & `openai_forward-0.2.0/openai_forward/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from fastapi import Request, HTTPException, status
+import os
+from itertools import cycle
+
+import httpx
+from fastapi import HTTPException, Request, status
 from fastapi.responses import StreamingResponse
 from loguru import logger
-import httpx
 from starlette.background import BackgroundTask
-import os
-from itertools import cycle
+
+from .config import env2list, print_startup_info, setting_log
 from .content.chat import ChatSaver
-from .config import env2list, print_startup_info
 
 
 class OpenaiBase:
     BASE_URL = os.environ.get("OPENAI_BASE_URL", "https://api.openai.com").strip()
     ROUTE_PREFIX = os.environ.get("ROUTE_PREFIX", "").strip()
     _LOG_CHAT = os.environ.get("LOG_CHAT", "False").strip().lower() == "true"
     _openai_api_key_list = env2list("OPENAI_API_KEY", sep=" ")
@@ -22,24 +24,33 @@
 
     if ROUTE_PREFIX:
         if ROUTE_PREFIX.endswith('/'):
             ROUTE_PREFIX = ROUTE_PREFIX[:-1]
         if not ROUTE_PREFIX.startswith('/'):
             ROUTE_PREFIX = '/' + ROUTE_PREFIX
     timeout = 30
-    chatsaver = ChatSaver(save_interval=10)
-    print_startup_info(BASE_URL, ROUTE_PREFIX, _openai_api_key_list, _FWD_KEYS, _LOG_CHAT)
+
+    print_startup_info(
+        BASE_URL, ROUTE_PREFIX, _openai_api_key_list, _FWD_KEYS, _LOG_CHAT
+    )
+    if _LOG_CHAT:
+        setting_log(save_file=False)
+        chatsaver = ChatSaver(save_interval=10)
 
     def validate_request_host(self, ip):
         if self.IP_WHITELIST and ip not in self.IP_WHITELIST:
-            raise HTTPException(status_code=status.HTTP_403_FORBIDDEN,
-                                detail=f"Forbidden, ip={ip} not in whitelist!")
+            raise HTTPException(
+                status_code=status.HTTP_403_FORBIDDEN,
+                detail=f"Forbidden, ip={ip} not in whitelist!",
+            )
         if self.IP_BLACKLIST and ip in self.IP_BLACKLIST:
-            raise HTTPException(status_code=status.HTTP_403_FORBIDDEN,
-                                detail=f"Forbidden, ip={ip} in blacklist!")
+            raise HTTPException(
+                status_code=status.HTTP_403_FORBIDDEN,
+                detail=f"Forbidden, ip={ip} in blacklist!",
+            )
 
     @classmethod
     async def aiter_bytes(cls, r: httpx.Response, route_path: str):
         bytes_ = b''
         async for chunk in r.aiter_bytes():
             bytes_ += chunk
             yield chunk
@@ -47,67 +58,84 @@
             target_info = cls.chatsaver.parse_bytes_to_content(bytes_, route_path)
             cls.chatsaver.add_chat({target_info['role']: target_info['content']})
         except Exception as e:
             logger.debug(f"log chat (not) error:\n{e=}")
 
     @classmethod
     async def _reverse_proxy(cls, request: Request):
-        client: httpx.AsyncClient = request.app.state.client
+        client = httpx.AsyncClient(base_url=cls.BASE_URL, http1=True, http2=False)
         url_path = request.url.path
-        url_path = url_path[len(cls.ROUTE_PREFIX):]
+        url_path = url_path[len(cls.ROUTE_PREFIX) :]
         url = httpx.URL(path=url_path, query=request.url.query.encode('utf-8'))
         headers = dict(request.headers)
         auth = headers.pop("authorization", None)
         if auth and str(auth).startswith("Bearer sk-"):
             tmp_headers = {'Authorization': auth}
         elif cls._openai_api_key_list:
             logger.info(f"Use forward key: {cls._use_forward_key}")
             if cls._use_forward_key:
                 fk_prefix = "Bearer fk-"
                 logger.info(f"current forward key: {auth}")
-                if auth and str(auth).startswith(fk_prefix) and auth[len("Bearer "):] in cls._FWD_KEYS:
+                if (
+                    auth
+                    and str(auth).startswith(fk_prefix)
+                    and auth[len("Bearer ") :] in cls._FWD_KEYS
+                ):
                     auth = "Bearer " + next(cls._cycle_api_key)
                     tmp_headers = {'Authorization': auth}
                 else:
                     tmp_headers = {}
             else:
                 auth = "Bearer " + next(cls._cycle_api_key)
                 tmp_headers = {'Authorization': auth}
         else:
             tmp_headers = {}
 
         log_chat_completions = False
         if cls._LOG_CHAT and request.method == 'POST':
             try:
-                chat_info = await cls.chatsaver.parse_payload_to_content(request, route_path=url_path)
+                chat_info = await cls.chatsaver.parse_payload_to_content(
+                    request, route_path=url_path
+                )
                 if chat_info:
                     cls.chatsaver.add_chat(chat_info)
                     log_chat_completions = True
             except Exception as e:
-                logger.debug(f"log chat error:\n{request.client.host=} {request.method=}: {e}")
+                logger.debug(
+                    f"log chat error:\n{request.client.host=} {request.method=}: {e}"
+                )
 
         tmp_headers.update({"Content-Type": "application/json"})
         req = client.build_request(
-            request.method, url, headers=tmp_headers,
+            request.method,
+            url,
+            headers=tmp_headers,
             content=request.stream(),
             timeout=cls.timeout,
         )
         try:
             r = await client.send(req, stream=True)
         except (httpx.ConnectError, httpx.ConnectTimeout) as e:
-            error_info = f"{type(e)}: {e} | " \
-                         f"Please check if host={request.client.host} can access [{cls.BASE_URL}] successfully?"
+            error_info = (
+                f"{type(e)}: {e} | "
+                f"Please check if host={request.client.host} can access [{cls.BASE_URL}] successfully?"
+            )
             logger.error(error_info)
-            raise HTTPException(status_code=status.HTTP_504_GATEWAY_TIMEOUT, detail=error_info)
+            raise HTTPException(
+                status_code=status.HTTP_504_GATEWAY_TIMEOUT, detail=error_info
+            )
         except Exception as e:
             error_info = f"{type(e)}: {e}"
             logger.error(error_info)
-            raise HTTPException(status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=error_info)
+            raise HTTPException(
+                status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=error_info
+            )
 
-        aiter_bytes = cls.aiter_bytes(r, url_path) if log_chat_completions else r.aiter_bytes()
+        aiter_bytes = (
+            cls.aiter_bytes(r, url_path) if log_chat_completions else r.aiter_bytes()
+        )
         return StreamingResponse(
             aiter_bytes,
             status_code=r.status_code,
-            # headers=r.headers, # do not use r.headers, it will cause error
             media_type=r.headers.get("content-type"),
-            background=BackgroundTask(r.aclose)
+            background=BackgroundTask(r.aclose),
         )
```

### Comparing `openai_forward-0.1.9/openai_forward/config.py` & `openai_forward-0.2.0/openai_forward/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-from loguru import logger
-import orjson
-from sparrow import relp
-from typing import Union, List, Dict
-import sys
 import logging
 import os
+import sys
 import time
+from typing import Dict, List, Union
+
+import orjson
+from loguru import logger
 from rich import print
 from rich.panel import Panel
 from rich.table import Table
+from sparrow import relp
 
 
 def print_startup_info(base_url, route_prefix, api_key, forward_key, log_chat):
     try:
         from dotenv import load_dotenv
+
         load_dotenv('.env')
     except Exception:
         ...
     route_prefix = route_prefix or "/"
     api_key_info = True if len(api_key) else False
     forward_key_info = True if len(forward_key) else False
     table = Table(title="", box=None, width=100)
     table.add_column("base-url", justify="left", style="#df412f")
     table.add_column("route-prefix", justify="center", style="#df412f")
     table.add_column("openai-api-key", justify="center", style="green")
     table.add_column("forward-key", justify="center", style="green")
     table.add_column("Log-chat", justify="center", style="green")
     table.add_column("Log-dir", justify="center", style="#f5bb00")
-    table.add_row(base_url, route_prefix, str(api_key_info), str(forward_key_info), str(log_chat), "./Log/*.log")
+    table.add_row(
+        base_url,
+        route_prefix,
+        str(api_key_info),
+        str(forward_key_info),
+        str(log_chat),
+        "./Log/*.log",
+    )
     print(Panel(table, title="🤗openai-forward is ready to serve!", expand=False))
 
 
 class InterceptHandler(logging.Handler):
     def emit(self, record):
         # Get corresponding Loguru level if it exists
         try:
@@ -40,34 +49,43 @@
             level = record.levelno
 
         # Find caller from where originated the logged message
         frame, depth = logging.currentframe(), 6
         while frame.f_code.co_filename == logging.__file__:
             frame = frame.f_back
             depth += 1
-        logger.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
+        logger.opt(depth=depth, exception=record.exc_info).log(
+            level, record.getMessage()
+        )
 
 
-def setting_log(log_name, multi_process=True):
+def setting_log(save_file=False, log_name=None, multi_process=True):
     # TODO 修复时区配置
     if os.environ.get("TZ") == "Asia/Shanghai":
         os.environ['TZ'] = "UTC-8"
         if hasattr(time, 'tzset'):
             time.tzset()
 
     logging.root.handlers = [InterceptHandler()]
     for name in logging.root.manager.loggerDict.keys():
         logging.getLogger(name).handlers = []
         logging.getLogger(name).propagate = True
-    logger_config = {
-        "handlers": [
-            {"sink": sys.stdout, "level": "DEBUG"},
-            {"sink": f"./Log/{log_name}.log", "enqueue": multi_process, "rotation": "100 MB", "level": "INFO"},
-        ],
-    }
+
+    config_handlers = [
+        {"sink": sys.stdout, "level": "DEBUG"},
+    ]
+    if save_file:
+        config_handlers += {
+            "sink": f"./Log/{log_name}.log",
+            "enqueue": multi_process,
+            "rotation": "100 MB",
+            "level": "INFO",
+        }
+
+    logger_config = {"handlers": config_handlers}
     logger.configure(**logger_config)
 
 
 def yaml_dump(data, filepath, rel_path=False, mode='w'):
     abs_path = relp(filepath, parents=1) if rel_path else filepath
     from yaml import dump
 
@@ -95,15 +113,17 @@
 
 def json_load(filepath: str, rel=False, mode='rb'):
     abs_path = relp(filepath, parents=1) if rel else filepath
     with open(abs_path, mode=mode) as f:
         return orjson.loads(f.read())
 
 
-def json_dump(data: Union[List, Dict], filepath: str, rel=False, indent_2=False, mode='wb'):
+def json_dump(
+    data: Union[List, Dict], filepath: str, rel=False, indent_2=False, mode='wb'
+):
     orjson_option = 0
     if indent_2:
         orjson_option = orjson.OPT_INDENT_2
     abs_path = relp(filepath, parents=1) if rel else filepath
     with open(abs_path, mode=mode) as f:
         f.write(orjson.dumps(data, option=orjson_option))
```

### Comparing `openai_forward-0.1.9/openai_forward/content/chat.py` & `openai_forward-0.2.0/openai_forward/content/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import os
+from pathlib import Path
+from typing import Dict, List
+
 import orjson
-from orjson import JSONDecodeError
-from loguru import logger
-from httpx._decoders import LineDecoder
 from fastapi import Request
-from pathlib import Path
+from httpx._decoders import LineDecoder
+from loguru import logger
+from orjson import JSONDecodeError
 from sparrow import relp
-from typing import List, Dict
-import os
 
 decoder = LineDecoder()
 
 
 def _parse_iter_line_content(line: str):
     line = line[6:]
     try:
@@ -60,14 +61,17 @@
         self._init_chat_file()
 
     @property
     def chat_file(self):
         return os.path.join(self._log_dir, f"chat_{self._file_idx}.txt")
 
     def _init_chat_file(self):
+        _log_dir = Path(self._log_dir)
+        if not _log_dir.exists():
+            _log_dir.mkdir(parents=True)
         while Path(self.chat_file).exists():
             self._file_idx += 1
 
     @staticmethod
     async def parse_payload_to_content(request: Request, route_path: str):
         payload = await request.json()
         if route_path == "/v1/chat/completions":
@@ -101,15 +105,17 @@
                 logger.info(f"{self._cur_chat_file_size} is too large, create new file")
                 self._file_idx += 1
                 self._cur_chat_file_size = 1
             self.dump_chat_list(self._chat_list, self.chat_file, mode='a+', _end='\n')
             self._chat_list = []
 
     @staticmethod
-    def dump_chat_list(data: List[Dict], filepath: str, rel=False, mode='w', _sep='\n', _end="\n"):
+    def dump_chat_list(
+        data: List[Dict], filepath: str, rel=False, mode='w', _sep='\n', _end="\n"
+    ):
         str_data = _sep.join([str(i) for i in data]) + _end
         abs_path = relp(filepath, parents=1) if rel else filepath
         with open(abs_path, mode=mode) as f:
             f.write(str_data)
 
     @staticmethod
     def load_chat_list(filepath: str, rel=False, mode='r', _sep='\n'):
```

### Comparing `openai_forward-0.1.9/openai_forward/routers/schemas.py` & `openai_forward-0.2.0/openai_forward/routers/schemas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,54 @@
 from __future__ import annotations
 
+from typing import Dict, List, Optional, Union
+
 from pydantic import BaseModel, Field
-from typing import List, Dict, Optional, Union
 
 
 class OpenAIV1ChatCompletion(BaseModel):
     """Creates a completion for the chat message"""
-    model: str = Field(..., description="The model to use for the completion", example="gpt-3.5-turbo")
-    messages: List[Dict[str, str]] = Field(..., description="The message to complete",
-                                           example=[{"role": "user", "content": "hi"}])
+
+    model: str = Field(
+        ..., description="The model to use for the completion", example="gpt-3.5-turbo"
+    )
+    messages: List[Dict[str, str]] = Field(
+        ...,
+        description="The message to complete",
+        example=[{"role": "user", "content": "hi"}],
+    )
     temperature: float = Field(default=1, description="0会导致更确定的结果，1会导致更随机的结果")
     top_p: float = Field(default=1, description="0会导致更确定的结果，1会导致更随机的结果")
-    n: int = Field(default=1, description="How many chat completion choices to generate for each input message.")
+    n: int = Field(
+        default=1,
+        description="How many chat completion choices to generate for each input message.",
+    )
     stream: bool = Field(default=False)
-    stop: Union[List[str], str, None] = Field(default=None,
-                                              description="Up to 4 sequences where the API will stop generating further tokens.")
-    max_tokens: Union[int, None] = Field(default=None, description="The maximum number of tokens to generate in the chat completion. The total length of input tokens and generated tokens is limited by the model's context length.")
-    presence_penalty: float = Field(default=0, description="Number between -2.0 and 2.0. ")
-    frequency_penalty: float = Field(default=0, description="Number between -2.0 and 2.0. ")
-    logit_bias: Optional[Dict[str, float]] = Field(default=None, description="取值[-100, 100]， 取值越大，生成的结果越偏向于该token。 取-100表示完全不考虑该token。")
-    user: Optional[str] = Field(default=None,
-                                description="A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. ",
-                                )
+    stop: Union[List[str], str, None] = Field(
+        default=None,
+        description="Up to 4 sequences where the API will stop generating further tokens.",
+    )
+    max_tokens: Union[int, None] = Field(
+        default=None,
+        description="The maximum number of tokens to generate in the chat completion. The total length of input tokens and generated tokens is limited by the model's context length.",
+    )
+    presence_penalty: float = Field(
+        default=0, description="Number between -2.0 and 2.0. "
+    )
+    frequency_penalty: float = Field(
+        default=0, description="Number between -2.0 and 2.0. "
+    )
+    logit_bias: Optional[Dict[str, float]] = Field(
+        default=None,
+        description="取值[-100, 100]， 取值越大，生成的结果越偏向于该token。 取-100表示完全不考虑该token。",
+    )
+    user: Optional[str] = Field(
+        default=None,
+        description="A unique identifier representing your end-user, which can help OpenAI to monitor and detect abuse. ",
+    )
 
     class Config:
         schema_extra = {
             "example": {
                 "model": "gpt-3.5-turbo",
                 "messages": [{"role": "user", "content": "hi"}],
                 "stream": False,
```

### Comparing `openai_forward-0.1.9/.gitignore` & `openai_forward-0.2.0/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+.github/release-template.ejs
+scripts/release.sh
+node_modules
+package-lock.json
+package.json
 .idea/
 .vscode/
 .DS_Store
 third-party/
 run.sh
 ssl/
 chat.yaml
 chat_*.yaml
 
-.env.example
 Log/
 Log-caloi-top/
 dist/
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
@@ -135,7 +139,8 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+.vercel
```

### Comparing `openai_forward-0.1.9/LICENSE` & `openai_forward-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.9/README.md` & `openai_forward-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+Metadata-Version: 2.1
+Name: openai_forward
+Version: 0.2.0
+Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · stream forwarding
+Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
+Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
+Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
+Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
+Author-email: kunyuan <beidongjiedeguang@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
+Keywords: OpenAI API Forwarding,chatgpt,fastapi,httpx,openai,openai-api,openai-proxy,python,streaming-api
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Requires-Dist: fastapi
+Requires-Dist: httpx
+Requires-Dist: loguru
+Requires-Dist: orjson
+Requires-Dist: python-dotenv
+Requires-Dist: pytz
+Requires-Dist: sparrow-python>=0.1.3
+Requires-Dist: uvicorn
+Provides-Extra: bard
+Requires-Dist: googlebard; extra == 'bard'
+Provides-Extra: chatgpt
+Requires-Dist: revchatgpt; extra == 'chatgpt'
+Provides-Extra: edge
+Requires-Dist: edgegpt; extra == 'edge'
+Provides-Extra: ssl
+Requires-Dist: certbot; extra == 'ssl'
+Description-Content-Type: text/markdown
+
 **中文** | [**English**](./README_EN.md)
 
 <h1 align="center">
     <br>
     OpenAI Forward
     <br>
 </h1>
@@ -20,267 +54,216 @@
     </a>
     <a href="https://github.com/beidongjiedeguang/openai-forward">
         <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/beidongjiedeguang/openai-forward">
     </a>
     <a href="https://hub.docker.com/r/beidongjiedeguang/openai-forward">
         <img alt="docer image size" src="https://img.shields.io/docker/image-size/beidongjiedeguang/openai-forward?style=flat&label=docker image">
     </a>
-    <a href="https://github.com/beidongjiedeguang/openai-forward/actions/workflows/run_tests.yaml">
-        <img alt="tests" src="https://img.shields.io/github/actions/workflow/status/beidongjiedeguang/openai-forward/run_tests.yml?label=tests">
+    <a href="https://github.com/beidongjiedeguang/openai-forward/actions/workflows/ci.yml">
+        <img alt="tests" src="https://img.shields.io/github/actions/workflow/status/beidongjiedeguang/openai-forward/ci.yml?label=tests">
     </a>
-    <a href="https://pypi.org/project/openai_forward/">
+    <a href="https://pypistats.org/packages/openai-forward">
         <img alt="pypi downloads" src="https://img.shields.io/pypi/dm/openai_forward">
     </a>
     <a href="https://codecov.io/gh/beidongjiedeguang/openai-forward">
         <img alt="codecov" src="https://codecov.io/gh/beidongjiedeguang/openai-forward/branch/dev/graph/badge.svg">
     </a>
 </p>
 
 
 
 本项目用于解决一些地区无法直接访问OpenAI的问题，将该服务部署在可以正常访问openai
 api的服务器上，通过该服务转发OpenAI的请求。即搭建反向代理服务  
 
 ---
 
-测试访问：https://caloi.top/openai/v1/chat/completions  
-或者说 https://caloi.top/openai 等价于 https://api.openai.com
+由本项目搭建的长期代理地址：
+> https://api.openai-forward.top  
+
 
----
 
-# 目录
+## 目录
 
 - [功能](#功能)
+- [部署指南](#部署指南)
 - [应用](#应用)
-- [安装部署](#安装部署)
-- [服务调用](#服务调用)
 - [配置选项](#配置选项)
 - [聊天日志](#聊天日志)
 - [高级配置](#高级配置)
 
-# 功能
+## 功能
 **基础功能**  
 - [x] 支持转发OpenAI所有接口
 - [x] 支持流式响应
 - [x] 支持指定转发路由前缀
 - [x] docker部署
 - [x] pip 安装部署
+- [x] vercel 一键个人免费部署
+  [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fbeidongjiedeguang%2Fopenai-forward&project-name=openai-forward&repository-name=openai-forward&framework=other)
 
 **高级功能**  
 - [x] 实时记录聊天记录(包括流式响应的聊天内容)
-- [x] 支持默认openai api key(多api key 循环调用)
-- [x] 自定义forward api key 代替 openai api key (见高级配置)
+- [x] 允许输入多个openai api key 组成轮询池
+- [x] 自定义 api key (见高级配置)
 - [x] 支持请求IP验证(IP白名单与黑名单)
 
-# 应用
+## 部署指南
 
-> 这里以个人使用该项目搭建好的代理服务 https://caloi.top/openai 为例
+提供三种部署方式
+1. [vps + pip 安装部署](deploy.md#pip-推荐) (推荐)
+2. [vps + Docker](deploy.md#docker-推荐) (推荐) 
+    > https://api.openai-forward.top 
+3. [一键Vercel部署](deploy.md#vercel-一键部署) 
+   > https://vercel.openai-forward.top 
 
-### [caloi.top](https://caloi.top)
+## 应用
+
+### [聊天应用](https://chat.beidongjiedeguang.top)
 
 基于开源项目[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)搭建自己的chatgpt服务  
 替换docker启动命令中的 `BASE_URL`为我们自己搭建的代理服务地址
 
 ```bash 
 docker run -d \
     -p 3000:3000 \
     -e OPENAI_API_KEY="sk-******" \
-    -e BASE_URL="caloi.top/openai" \
-    -e CODE="<your password>" \
+    -e BASE_URL="https://api.openai-forward.top" \
+    -e CODE="kunyuan" \
     yidadaa/chatgpt-next-web 
 ``` 
+这里部署了一个，供大家轻度使用:  
+ https://chat.beidongjiedeguang.top , 访问密码: `kunyuan` 
 
-访问 https://caloi.top 。访问密码为 `beidongjiedeguang`
-
-### 在模块中使用
+### 在代码中使用
 
 **JS/TS**
 
 ```diff
   import { Configuration } from "openai";
   
   const configuration = new Configuration({
-+ basePath: "https://caloi.top/openai/v1",
++ basePath: "https://api.openai-forward.top/v1",
   apiKey: "sk-******",
   });
 ```
 
 **Python**
 
 ```diff
   import openai
-+ openai.api_base = "https://caloi.top/openai/v1"
++ openai.api_base = "https://api.openai-forward.top/v1"
   openai.api_key = "sk-******"
 ```
 
-### Image Generation (DALL-E):
+**gpt-3.5-turbo**
+```bash
+curl https://api.openai-forward.top/v1/chat/completions \
+  -H "Content-Type: application/json" \
+  -H "Authorization: Bearer sk-******" \
+  -d '{
+    "model": "gpt-3.5-turbo",
+    "messages": [{"role": "user", "content": "Hello!"}]
+  }'
+```
 
+**Image Generation (DALL-E)**
 ```bash
-curl --location 'https://caloi.top/openai/v1/images/generations' \
+curl --location 'https://api.openai-forward.top/v1/images/generations' \
 --header 'Authorization: Bearer sk-******' \
 --header 'Content-Type: application/json' \
 --data '{
     "prompt": "A photo of a cat",
     "n": 1,
     "size": "512x512"
 }'
 ```
 
-# 安装部署
-
-选择一种即可
 
-## pip
-
-**安装**
-
-```bash
-pip install openai-forward
-```
-
-**运行转发服务**  
-可通过`--port`指定端口号，默认为`8000`
-
-```bash
-openai_forward run --port=9999 
-```
-
-服务就搭建完成了，使用方式只需将`https://api.openai.com` 替换为服务所在端口`http://{ip}:{port}` 即可。
-
-当然也可以将 OPENAI_API_KEY 作为环境变量或`--api_key`参数传入作为默认api key， 这样客户端在请求相关路由时可以无需在Header中传入Authorization。
-带默认api key的启动方式：
-
-```bash
-openai_forward run --port=9999 --api_key="sk-******"
-```
-
-注: 如果既存在默认api key又在请求头中传入了api key，则以请求头中的api key会覆盖默认api key.
-
-## Docker (推荐)
-
-```bash
-docker run -d -p 9999:8000 beidongjiedeguang/openai-forward:latest 
-```
-
-将映射宿主机的9999端口，通过`http://{ip}:9999`访问服务。  
-注：同样可以在启动命令中通过-e传入环境变量OPENAI_API_KEY=sk-xxx作为默认api key
-
-## 源码部署
-
-```bash
-git clone https://github.com/beidongjiedeguang/openai-forward.git --depth=1
-cd openai-forward
-```
-
-**Docker**
-
-```bash
-docker-compose up
-```
-
-**pip**
-
-```bash
-pip install -e .
-openai-forward run 
-```
-
-# 服务调用
-
-替换openai的api地址为该服务的地址即可，如：
-
-```bash
-https://api.openai.com/v1/chat/completions
-```
-
-替换为
-
-```bash
-http://{ip}:{port}/v1/chat/completions
-```
-
-# 配置选项
+## 配置选项
 
 **`openai-forward run`参数配置项**
 
 | 配置项       | 说明 | 默认值 |
 |-----------| --- | :---: |
 | --port    | 服务端口号 | 8000 |
 | --workers | 工作进程数 | 1 |
 
+更多参数 `openai-forward run --help` 查看
+
 **环境变量配置项**  
 支持从运行目录下的`.env`文件中读取: 
 
 | 环境变量            | 说明                                                              |           默认值            |
 |-----------------|-----------------------------------------------------------------|:------------------------:|
 | OPENAI_API_KEY  | 默认openai api key，支持多个默认api key, 以 `sk-` 开头， 以空格分割      |            无             |
 | FORWARD_KEY     | 允许调用方使用该key代替openai api key，支持多个forward key, 以`fk-` 开头, 以空格分割 |      无             |
 | OPENAI_BASE_URL | 转发base url                                                      | `https://api.openai.com` |
 | LOG_CHAT        | 是否记录聊天内容                                                        |          `true`          |
 | ROUTE_PREFIX    | 路由前缀                                                            |            无             |
 | IP_WHITELIST    | ip白名单, 空格分开                                                     |           无            |
 | IP_BLACKLIST    | ip黑名单, 空格分开                                                     |           无            | 
 
-# 聊天日志
-
-保存路径在当前目录下的`Log/`路径中。  
-聊天日志以 `chat_`开头, 默认每5轮对话写入一次文件    
-记录格式为
-
-```text
-{'host': xxx, 'model': xxx, 'message': [{'user': xxx}, {'assistant': xxx}]}
-{'assistant': xxx}
-
-{'host': ...}
-{'assistant': ...}
-
-...
-```
 
-# 高级配置
+## 高级配置
 
 **设置api_key为自己设置的forward key**  
 需要配置 OPENAI_API_KEY 和 FORWARD_KEY, 例如
 
 ```bash
 OPENAI_API_KEY=sk-*******
 FORWARD_KEY=fk-****** # 这里fk-token由我们自己定义
 ```
 这里我们配置了FORWARD_KEY为`fk-******`, 那么后面客户端在调用时只需设置OPENAI_API_KEY为我们自定义的`fk-******` 即可。  
 这样的好处是在使用一些需要输入OPENAI_API_KEY的第三方应用时，我们可以使用`fk-******`搭配proxy使用（如下面的例子） 而无需担心OPENAI_API_KEY被泄露。
 
 **用例:**
 ```bash
-curl https://caloi.top/openai/v1/chat/completions \
+curl https://api.openai-forward.top/v1/chat/completions \
   -H "Content-Type: application/json" \
-  -H "Authorization: Bearer fk-mytoken-abcd" \
+  -H "Authorization: Bearer fk-******" \
   -d '{
     "model": "gpt-3.5-turbo",
     "messages": [{"role": "user", "content": "Hello!"}]
   }'
 ```
 **Python**
 ```diff
   import openai
-+ openai.api_base = "https://caloi.top/openai/v1"
++ openai.api_base = "https://api.openai-forward.top/v1"
 - openai.api_key = "sk-******"
 + openai.api_key = "fk-******"
 ```
 **Web application**
 ```bash 
 docker run -d \
     -p 3000:3000 \
     -e OPENAI_API_KEY="fk-******" \
-    -e BASE_URL="caloi.top/openai" \
+    -e BASE_URL="https://api.openai-forward.top" \
     -e CODE="<your password>" \
     yidadaa/chatgpt-next-web 
 ``` 
 
-# Backer and Sponsor
+## 聊天日志
+
+保存路径在当前目录下的`Log/`路径中。  
+聊天日志以 `chat_`开头, 默认每5轮对话写入一次文件    
+记录格式为
+
+```text
+{'host': xxx, 'model': xxx, 'message': [{'user': xxx}, {'assistant': xxx}]}
+{'assistant': xxx}
+
+{'host': ...}
+{'assistant': ...}
+
+...
+```
+
+## Backer and Sponsor
 
 <a href="https://www.jetbrains.com/?from=beidongjiedeguang/openai-forward" target="_blank">
-<img src="./img/jetbrains.svg" width="100px" height="100px">
+<img src=".github/images/jetbrains.svg" width="100px" height="100px">
 </a>
 
-# License
+## License
 
 Openai-forward is licensed under the [MIT](https://opensource.org/license/mit/) license.
```

#### html2text {}

```diff
@@ -1,92 +1,101 @@
+Metadata-Version: 2.1 Name: openai_forward Version: 0.2.0 Summary: ð Openai
+api forward Â· OpenAI æ¥å£è½¬åæå¡ Â· stream forwarding Project-URL:
+Homepage, https://github.com/beidongjiedeguang/openai-forward Project-URL:
+Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-
+forward Project-URL: Issues, https://github.com/beidongjiedeguang/openai-
+forward/issues Project-URL: Source, https://github.com/beidongjiedeguang/
+openai-forward Author-email: kunyuan
+gmail.com> License-Expression: MIT License-File: LICENSE Keywords: OpenAI API
+Forwarding,chatgpt,fastapi,httpx,openai,openai-api,openai-
+proxy,python,streaming-api Classifier: Development Status :: 5 - Production/
+Stable Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist: fastapi Requires-
+Dist: httpx Requires-Dist: loguru Requires-Dist: orjson Requires-Dist: python-
+dotenv Requires-Dist: pytz Requires-Dist: sparrow-python>=0.1.3 Requires-Dist:
+uvicorn Provides-Extra: bard Requires-Dist: googlebard; extra == 'bard'
+Provides-Extra: chatgpt Requires-Dist: revchatgpt; extra == 'chatgpt' Provides-
+Extra: edge Requires-Dist: edgegpt; extra == 'edge' Provides-Extra: ssl
+Requires-Dist: certbot; extra == 'ssl' Description-Content-Type: text/markdown
 **ä¸­æ** | [**English**](./README_EN.md)
                                     ******
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                 image_size] [tests] [pypi_downloads] [codecov]
 æ¬é¡¹ç®ç¨äºè§£å³ä¸äºå°åºæ æ³ç´æ¥è®¿é®OpenAIçé®é¢ï¼å°è¯¥æå¡é¨ç½²å¨å¯ä»¥æ­£å¸¸è®¿é®openai
 apiçæå¡å¨ä¸ï¼éè¿è¯¥æå¡è½¬åOpenAIçè¯·æ±ãå³æ­å»ºååä»£çæå¡
---- æµè¯è®¿é®ï¼https://caloi.top/openai/v1/chat/completions æèè¯´
-https://caloi.top/openai ç­ä»·äº https://api.openai.com --- # ç®å½ -
-[åè½](#åè½) - [åºç¨](#åºç¨) - [å®è£é¨ç½²](#å®è£é¨ç½²) -
-[æå¡è°ç¨](#æå¡è°ç¨) - [éç½®éé¡¹](#éç½®éé¡¹) - [èå¤©æ¥å¿]
-(#èå¤©æ¥å¿) - [é«çº§éç½®](#é«çº§éç½®) # åè½ **åºç¡åè½** - [x]
+--- ç±æ¬é¡¹ç®æ­å»ºçé¿æä»£çå°åï¼ > https://api.openai-forward.top
+## ç®å½ - [åè½](#åè½) - [é¨ç½²æå](#é¨ç½²æå) - [åºç¨]
+(#åºç¨) - [éç½®éé¡¹](#éç½®éé¡¹) - [èå¤©æ¥å¿](#èå¤©æ¥å¿) -
+[é«çº§éç½®](#é«çº§éç½®) ## åè½ **åºç¡åè½** - [x]
 æ¯æè½¬åOpenAIæææ¥å£ - [x] æ¯ææµå¼ååº - [x]
-æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½² - [x] pip å®è£é¨ç½²
+æ¯ææå®è½¬åè·¯ç±åç¼ - [x] dockeré¨ç½² - [x] pip å®è£é¨ç½² - [x]
+vercel ä¸é®ä¸ªäººåè´¹é¨ç½² [![Deploy with Vercel](https://vercel.com/
+button)](https://vercel.com/new/clone?repository-
+url=https%3A%2F%2Fgithub.com%2Fbeidongjiedeguang%2Fopenai-forward&project-
+name=openai-forward&repository-name=openai-forward&framework=other)
 **é«çº§åè½** - [x] å®æ¶è®°å½èå¤©è®°å½
-(åæ¬æµå¼ååºçèå¤©åå®¹) - [x] æ¯æé»è®¤openai api key(å¤api key
-å¾ªç¯è°ç¨) - [x] èªå®ä¹forward api key ä»£æ¿ openai api key
-(è§é«çº§éç½®) - [x] æ¯æè¯·æ±IPéªè¯(IPç½ååä¸é»åå) # åºç¨
-> è¿éä»¥ä¸ªäººä½¿ç¨è¯¥é¡¹ç®æ­å»ºå¥½çä»£çæå¡ https://caloi.top/
-openai ä¸ºä¾ ### [caloi.top](https://caloi.top) åºäºå¼æºé¡¹ç®[ChatGPT-
-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-
-Web)æ­å»ºèªå·±çchatgptæå¡ æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
+(åæ¬æµå¼ååºçèå¤©åå®¹) - [x] åè®¸è¾å¥å¤ä¸ªopenai api key
+ç»æè½®è¯¢æ±  - [x] èªå®ä¹ api key (è§é«çº§éç½®) - [x]
+æ¯æè¯·æ±IPéªè¯(IPç½ååä¸é»åå) ## é¨ç½²æå
+æä¾ä¸ç§é¨ç½²æ¹å¼ 1. [vps + pip å®è£é¨ç½²](deploy.md#pip-æ¨è)
+(æ¨è) 2. [vps + Docker](deploy.md#docker-æ¨è) (æ¨è) > https://
+api.openai-forward.top 3. [ä¸é®Vercelé¨ç½²](deploy.md#vercel-ä¸é®é¨ç½²) >
+https://vercel.openai-forward.top ## åºç¨ ### [èå¤©åºç¨](https://
+chat.beidongjiedeguang.top) åºäºå¼æºé¡¹ç®[ChatGPT-Next-Web](https://
+github.com/Yidadaa/ChatGPT-Next-Web)æ­å»ºèªå·±çchatgptæå¡
+æ¿æ¢dockerå¯å¨å½ä»¤ä¸­ç
 `BASE_URL`ä¸ºæä»¬èªå·±æ­å»ºçä»£çæå¡å°å ```bash docker run -d \ -
-p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -e BASE_URL="caloi.top/openai" \
--e CODE="" \ yidadaa/chatgpt-next-web ``` è®¿é® https://caloi.top
-ãè®¿é®å¯ç ä¸º `beidongjiedeguang` ### å¨æ¨¡åä¸­ä½¿ç¨ **JS/TS** ```diff
-import { Configuration } from "openai"; const configuration = new Configuration
-({ + basePath: "https://caloi.top/openai/v1", apiKey: "sk-******", }); ```
-**Python** ```diff import openai + openai.api_base = "https://caloi.top/openai/
-v1" openai.api_key = "sk-******" ``` ### Image Generation (DALL-E): ```bash
-curl --location 'https://caloi.top/openai/v1/images/generations' \ --header
-'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
---data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` #
-å®è£é¨ç½² éæ©ä¸ç§å³å¯ ## pip **å®è£** ```bash pip install openai-
-forward ``` **è¿è¡è½¬åæå¡** å¯éè¿`--
-port`æå®ç«¯å£å·ï¼é»è®¤ä¸º`8000` ```bash openai_forward run --port=9999
-``` æå¡å°±æ­å»ºå®æäºï¼ä½¿ç¨æ¹å¼åªéå°`https://api.openai.com`
-æ¿æ¢ä¸ºæå¡æå¨ç«¯å£`http://{ip}:{port}` å³å¯ã å½ç¶ä¹å¯ä»¥å°
-OPENAI_API_KEY ä½ä¸ºç¯å¢åéæ`--api_key`åæ°ä¼ å¥ä½ä¸ºé»è®¤api
-keyï¼
-è¿æ ·å®¢æ·ç«¯å¨è¯·æ±ç¸å³è·¯ç±æ¶å¯ä»¥æ éå¨Headerä¸­ä¼ å¥Authorizationã
-å¸¦é»è®¤api keyçå¯å¨æ¹å¼ï¼ ```bash openai_forward run --port=9999 --
-api_key="sk-******" ``` æ³¨: å¦ææ¢å­å¨é»è®¤api
-keyåå¨è¯·æ±å¤´ä¸­ä¼ å¥äºapi keyï¼åä»¥è¯·æ±å¤´ä¸­çapi
-keyä¼è¦çé»è®¤api key. ## Docker (æ¨è) ```bash docker run -d -p 9999:
-8000 beidongjiedeguang/openai-forward:latest ```
-å°æ å°å®¿ä¸»æºç9999ç«¯å£ï¼éè¿`http://{ip}:9999`è®¿é®æå¡ã
-æ³¨ï¼åæ ·å¯ä»¥å¨å¯å¨å½ä»¤ä¸­éè¿-
-eä¼ å¥ç¯å¢åéOPENAI_API_KEY=sk-xxxä½ä¸ºé»è®¤api key ## æºç é¨ç½²
-```bash git clone https://github.com/beidongjiedeguang/openai-forward.git --
-depth=1 cd openai-forward ``` **Docker** ```bash docker-compose up ``` **pip**
-```bash pip install -e . openai-forward run ``` # æå¡è°ç¨
-æ¿æ¢openaiçapiå°åä¸ºè¯¥æå¡çå°åå³å¯ï¼å¦ï¼ ```bash https://
-api.openai.com/v1/chat/completions ``` æ¿æ¢ä¸º ```bash http://{ip}:{port}/v1/
-chat/completions ``` # éç½®éé¡¹ **`openai-forward run`åæ°éç½®é¡¹** |
-éç½®é¡¹ | è¯´æ | é»è®¤å¼ | |-----------| --- | :---: | | --port |
-æå¡ç«¯å£å· | 8000 | | --workers | å·¥ä½è¿ç¨æ° | 1 |
-**ç¯å¢åééç½®é¡¹** æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å: |
-ç¯å¢åé | è¯´æ | é»è®¤å¼ | |-----------------|------------------------
------------------------------------------|:------------------------:| |
-OPENAI_API_KEY | é»è®¤openai api keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-
-` å¼å¤´ï¼ ä»¥ç©ºæ ¼åå² | æ  | | FORWARD_KEY |
-åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai api keyï¼æ¯æå¤ä¸ªforward key,
-ä»¥`fk-` å¼å¤´, ä»¥ç©ºæ ¼åå² | æ  | | OPENAI_BASE_URL | è½¬åbase url |
-`https://api.openai.com` | | LOG_CHAT | æ¯å¦è®°å½èå¤©åå®¹ | `true` | |
-ROUTE_PREFIX | è·¯ç±åç¼ | æ  | | IP_WHITELIST | ipç½åå, ç©ºæ ¼åå¼
-| æ  | | IP_BLACKLIST | ipé»åå, ç©ºæ ¼åå¼ | æ  | # èå¤©æ¥å¿
-ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/`è·¯å¾ä¸­ã èå¤©æ¥å¿ä»¥
-`chat_`å¼å¤´, é»è®¤æ¯5è½®å¯¹è¯åå¥ä¸æ¬¡æä»¶ è®°å½æ ¼å¼ä¸º ```text
-{'host': xxx, 'model': xxx, 'message': [{'user': xxx}, {'assistant': xxx}]}
-{'assistant': xxx} {'host': ...} {'assistant': ...} ... ``` # é«çº§éç½®
-**è®¾ç½®api_keyä¸ºèªå·±è®¾ç½®çforward key** éè¦éç½® OPENAI_API_KEY å
-FORWARD_KEY, ä¾å¦ ```bash OPENAI_API_KEY=sk-******* FORWARD_KEY=fk-****** #
-è¿éfk-tokenç±æä»¬èªå·±å®ä¹ ``` è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-
-******`,
+p 3000:3000 \ -e OPENAI_API_KEY="sk-******" \ -e BASE_URL="https://api.openai-
+forward.top" \ -e CODE="kunyuan" \ yidadaa/chatgpt-next-web ```
+è¿éé¨ç½²äºä¸ä¸ªï¼ä¾å¤§å®¶è½»åº¦ä½¿ç¨: https://
+chat.beidongjiedeguang.top , è®¿é®å¯ç : `kunyuan` ### å¨ä»£ç ä¸­ä½¿ç¨
+**JS/TS** ```diff import { Configuration } from "openai"; const configuration =
+new Configuration({ + basePath: "https://api.openai-forward.top/v1", apiKey:
+"sk-******", }); ``` **Python** ```diff import openai + openai.api_base =
+"https://api.openai-forward.top/v1" openai.api_key = "sk-******" ``` **gpt-3.5-
+turbo** ```bash curl https://api.openai-forward.top/v1/chat/completions \ -
+H "Content-Type: application/json" \ -H "Authorization: Bearer sk-******" \ -
+d '{ "model": "gpt-3.5-turbo", "messages": [{"role": "user", "content":
+"Hello!"}] }' ``` **Image Generation (DALL-E)** ```bash curl --location 'https:
+//api.openai-forward.top/v1/images/generations' \ --header 'Authorization:
+Bearer sk-******' \ --header 'Content-Type: application/json' \ --data '
+{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ##
+éç½®éé¡¹ **`openai-forward run`åæ°éç½®é¡¹** | éç½®é¡¹ | è¯´æ |
+é»è®¤å¼ | |-----------| --- | :---: | | --port | æå¡ç«¯å£å· | 8000 | | -
+-workers | å·¥ä½è¿ç¨æ° | 1 | æ´å¤åæ° `openai-forward run --help`
+æ¥ç **ç¯å¢åééç½®é¡¹**
+æ¯æä»è¿è¡ç®å½ä¸ç`.env`æä»¶ä¸­è¯»å: | ç¯å¢åé | è¯´æ |
+é»è®¤å¼ | |-----------------|------------------------------------------------
+-----------------|:------------------------:| | OPENAI_API_KEY | é»è®¤openai
+api keyï¼æ¯æå¤ä¸ªé»è®¤api key, ä»¥ `sk-` å¼å¤´ï¼ ä»¥ç©ºæ ¼åå² | æ 
+| | FORWARD_KEY | åè®¸è°ç¨æ¹ä½¿ç¨è¯¥keyä»£æ¿openai api
+keyï¼æ¯æå¤ä¸ªforward key, ä»¥`fk-` å¼å¤´, ä»¥ç©ºæ ¼åå² | æ  | |
+OPENAI_BASE_URL | è½¬åbase url | `https://api.openai.com` | | LOG_CHAT |
+æ¯å¦è®°å½èå¤©åå®¹ | `true` | | ROUTE_PREFIX | è·¯ç±åç¼ | æ  | |
+IP_WHITELIST | ipç½åå, ç©ºæ ¼åå¼ | æ  | | IP_BLACKLIST | ipé»åå,
+ç©ºæ ¼åå¼ | æ  | ## é«çº§éç½® **è®¾ç½®api_keyä¸ºèªå·±è®¾ç½®çforward
+key** éè¦éç½® OPENAI_API_KEY å FORWARD_KEY, ä¾å¦ ```bash
+OPENAI_API_KEY=sk-******* FORWARD_KEY=fk-****** # è¿éfk-
+tokenç±æä»¬èªå·±å®ä¹ ``` è¿éæä»¬éç½®äºFORWARD_KEYä¸º`fk-******`,
 é£ä¹åé¢å®¢æ·ç«¯å¨è°ç¨æ¶åªéè®¾ç½®OPENAI_API_KEYä¸ºæä»¬èªå®ä¹ç`fk-
 ******` å³å¯ã
 è¿æ ·çå¥½å¤æ¯å¨ä½¿ç¨ä¸äºéè¦è¾å¥OPENAI_API_KEYçç¬¬ä¸æ¹åºç¨æ¶ï¼æä»¬å¯ä»¥ä½¿ç¨`fk-
 ******`æ­éproxyä½¿ç¨ï¼å¦ä¸é¢çä¾å­ï¼
 èæ éæå¿OPENAI_API_KEYè¢«æ³é²ã **ç¨ä¾:** ```bash curl https://
-caloi.top/openai/v1/chat/completions \ -H "Content-Type: application/json" \ -
-H "Authorization: Bearer fk-mytoken-abcd" \ -d '{ "model": "gpt-3.5-turbo",
+api.openai-forward.top/v1/chat/completions \ -H "Content-Type: application/
+json" \ -H "Authorization: Bearer fk-******" \ -d '{ "model": "gpt-3.5-turbo",
 "messages": [{"role": "user", "content": "Hello!"}] }' ``` **Python** ```diff
-import openai + openai.api_base = "https://caloi.top/openai/v1" -
+import openai + openai.api_base = "https://api.openai-forward.top/v1" -
 openai.api_key = "sk-******" + openai.api_key = "fk-******" ``` **Web
 application** ```bash docker run -d \ -p 3000:3000 \ -e OPENAI_API_KEY="fk-
-******" \ -e BASE_URL="caloi.top/openai" \ -e CODE="" \ yidadaa/chatgpt-next-
-web ``` # Backer and Sponsor [./img/jetbrains.svg] # License Openai-forward is
-licensed under the [MIT](https://opensource.org/license/mit/) license.
+******" \ -e BASE_URL="https://api.openai-forward.top" \ -e CODE="" \ yidadaa/
+chatgpt-next-web ``` ## èå¤©æ¥å¿ ä¿å­è·¯å¾å¨å½åç®å½ä¸ç`Log/
+`è·¯å¾ä¸­ã èå¤©æ¥å¿ä»¥ `chat_`å¼å¤´,
+é»è®¤æ¯5è½®å¯¹è¯åå¥ä¸æ¬¡æä»¶ è®°å½æ ¼å¼ä¸º ```text {'host': xxx,
+'model': xxx, 'message': [{'user': xxx}, {'assistant': xxx}]} {'assistant':
+xxx} {'host': ...} {'assistant': ...} ... ``` ## Backer and Sponsor [.github/
+images/jetbrains.svg] ## License Openai-forward is licensed under the [MIT]
+(https://opensource.org/license/mit/) license.
```

### Comparing `openai_forward-0.1.9/pyproject.toml` & `openai_forward-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 [project]
 name = "openai_forward"
 description = "🚀 Openai api forward · OpenAI 接口转发服务 · stream forwarding"
 authors = [
     { name = "kunyuan", email = "beidongjiedeguang@gmail.com" },
 ]
+license = "MIT"
 requires-python = ">=3.6"
 readme = "README.md"
-keywords = ["openai", "chatgpt", "openai-api", "openai-proxy", "forward", "streaming-api", "fastapi", "python"]
+keywords = ["openai", "chatgpt", "openai-api", "openai-proxy", "OpenAI API Forwarding", "streaming-api", "fastapi", "python", "httpx"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3"
 ]
 
 dependencies = [
@@ -22,15 +23,14 @@
     "sparrow-python>=0.1.3",
     "fastapi",
     "uvicorn",
     "orjson",
     "python-dotenv",
     "httpx",
     "pytz",
-    "chardet",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/beidongjiedeguang/openai-forward"
 Documentation = "https://github.com/beidongjiedeguang/openai-forward#openai-forward"
```

