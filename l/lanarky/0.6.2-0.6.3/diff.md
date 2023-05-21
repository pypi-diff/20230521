# Comparing `tmp/lanarky-0.6.2.tar.gz` & `tmp/lanarky-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanarky-0.6.2.tar", max compression
+gzip compressed data, was "lanarky-0.6.3.tar", max compression
```

## Comparing `lanarky-0.6.2.tar` & `lanarky-0.6.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1073 2023-05-18 01:02:27.388100 lanarky-0.6.2/LICENSE
--rw-r--r--   0        0        0     3621 2023-05-18 01:02:27.388100 lanarky-0.6.2/README.md
--rw-r--r--   0        0        0        0 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/__init__.py
--rw-r--r--   0        0        0     2867 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/callbacks/__init__.py
--rw-r--r--   0        0        0      940 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/callbacks/base.py
--rw-r--r--   0        0        0     1360 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/callbacks/llm.py
--rw-r--r--   0        0        0     2675 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/callbacks/qa_with_sources.py
--rw-r--r--   0        0        0     2853 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0     1332 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/register.py
--rw-r--r--   0        0        0       74 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/responses/__init__.py
--rw-r--r--   0        0        0     2810 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/responses/streaming.py
--rw-r--r--   0        0        0      536 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/schemas.py
--rw-r--r--   0        0        0       69 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/testing/__init__.py
--rw-r--r--   0        0        0     3212 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/testing/settings.py
--rw-r--r--   0        0        0       73 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/websockets/__init__.py
--rw-r--r--   0        0        0     3608 2023-05-18 01:02:27.592099 lanarky-0.6.2/lanarky/websockets/base.py
--rw-r--r--   0        0        0      788 2023-05-18 01:02:27.592099 lanarky-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 lanarky-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-21 20:37:29.283520 lanarky-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3864 2023-05-21 20:37:29.283520 lanarky-0.6.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/__init__.py
+-rw-r--r--   0        0        0     3018 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/callbacks/__init__.py
+-rw-r--r--   0        0        0     2334 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/callbacks/agents.py
+-rw-r--r--   0        0        0     1507 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/callbacks/base.py
+-rw-r--r--   0        0        0     1421 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/callbacks/llm.py
+-rw-r--r--   0        0        0     2675 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/callbacks/qa_with_sources.py
+-rw-r--r--   0        0        0     2801 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0     1352 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/register.py
+-rw-r--r--   0        0        0       74 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/responses/__init__.py
+-rw-r--r--   0        0        0     2676 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/responses/streaming.py
+-rw-r--r--   0        0        0      536 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/testing/__init__.py
+-rw-r--r--   0        0        0     3212 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/websockets/__init__.py
+-rw-r--r--   0        0        0     3844 2023-05-21 20:37:29.487520 lanarky-0.6.3/lanarky/websockets/base.py
+-rw-r--r--   0        0        0      918 2023-05-21 20:37:29.487520 lanarky-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     4642 1970-01-01 00:00:00.000000 lanarky-0.6.3/PKG-INFO
```

### Comparing `lanarky-0.6.2/LICENSE` & `lanarky-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.2/README.md` & `lanarky-0.6.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 <div align="center">
 
-<img src="assets/logo.png" alt="lanarky-logo" width="150">
+<img src="https://raw.githubusercontent.com/ajndkr/lanarky/main/assets/logo.png" alt="lanarky-logo" width="150">
 
 <h1> Lanarky </h1>
 
 [![stars](https://img.shields.io/github/stars/ajndkr/lanarky)](https://github.com/ajndkr/lanarky/stargazers)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/lanarky/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/lanarky.svg)](https://pypi.org/project/lanarky/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-3916/)
+[![Code Coverage](https://coveralls.io/repos/github/ajndkr/lanarky/badge.svg?branch=main)](https://coveralls.io/github/ajndkr/lanarky?branch=main)
 
 </div>
 
 Lanarky is an open-source framework to deploy LLM applications in production. It is built on top of [FastAPI](https://github.com/tiangolo/fastapi)
 and comes with batteries included.
 
 ## 🚀 Features
@@ -80,12 +81,12 @@
 
 [![Code check](https://github.com/ajndkr/lanarky/actions/workflows/code-check.yaml/badge.svg)](https://github.com/ajndkr/lanarky/actions/workflows/code-check.yaml)
 [![Publish](https://github.com/ajndkr/lanarky/actions/workflows/publish.yaml/badge.svg)](https://github.com/ajndkr/lanarky/actions/workflows/publish.yaml)
 
 Contributions are more than welcome! If you have an idea for a new feature or want to help improve lanarky,
 please create an issue or submit a pull request on [GitHub](https://github.com/ajndkr/lanarky).
 
-See [CONTRIBUTING.md](./CONTRIBUTING.md) for more information.
+See [CONTRIBUTING.md](https://github.com/ajndkr/lanarky/blob/main/CONTRIBUTING.md) for more information.
 
 ## ⚖️ License
 
 The library is released under the [MIT License](https://github.com/ajndkr/lanarky/blob/main/LICENSE).
```

### Comparing `lanarky-0.6.2/lanarky/callbacks/__init__.py` & `lanarky-0.6.3/lanarky/callbacks/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from langchain.chains.base import Chain
 
 from lanarky.register import STREAMING_CALLBACKS, WEBSOCKET_CALLBACKS
 
+from .agents import AsyncAgentsStreamingCallback, AsyncAgentsWebsocketCallback
 from .base import AsyncStreamingResponseCallback, AsyncWebsocketCallback
 from .llm import (
     AsyncConversationChainStreamingCallback,
     AsyncConversationChainWebsocketCallback,
     AsyncLLMChainStreamingCallback,
     AsyncLLMChainWebsocketCallback,
 )
@@ -39,14 +40,16 @@
     "AsyncQAWithSourcesChainWebsocketCallback",
     "AsyncRetrievalQAWithSourcesChainStreamingCallback",
     "AsyncRetrievalQAWithSourcesChainWebsocketCallback",
     "AsyncVectorDBQAWithSourcesChainStreamingCallback",
     "AsyncVectorDBQAWithSourcesChainWebsocketCallback",
     "AsyncConversationalRetrievalChainStreamingCallback",
     "AsyncConversationalRetrievalChainWebsocketCallback",
+    "AsyncAgentsStreamingCallback",
+    "AsyncAgentsWebsocketCallback",
 ]
 
 ERROR_MESSAGE = """Error! Chain type '{chain_type}' is not currently supported by '{callable_name}'."""
 
 
 def get_streaming_callback(
     chain: Chain, *args, **kwargs
```

### Comparing `lanarky-0.6.2/lanarky/callbacks/base.py` & `lanarky-0.6.3/lanarky/callbacks/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,47 @@
+from abc import abstractmethod
+from typing import Any
+
 from fastapi import WebSocket
 from langchain.callbacks.base import AsyncCallbackHandler
 from pydantic import BaseModel, Field
-from starlette.types import Send
+from starlette.types import Message, Send
 
 from lanarky.schemas import WebsocketResponse
 
 
-class AsyncStreamingResponseCallback(AsyncCallbackHandler, BaseModel):
+class AsyncLanarkyCallback(AsyncCallbackHandler, BaseModel):
     """Async Callback handler for FastAPI StreamingResponse."""
 
-    send: Send = Field(...)
-
     @property
     def always_verbose(self) -> bool:
         """Whether to call verbose callbacks even if verbose is False."""
         return True
 
+    class Config:
+        arbitrary_types_allowed = True
+
+    @abstractmethod
+    def _construct_message(self, message: str) -> Any:  # pragma: no cover
+        """Construct a Message from a string."""
+        pass
+
+
+class AsyncStreamingResponseCallback(AsyncLanarkyCallback):
+    """Async Callback handler for FastAPI StreamingResponse."""
+
+    send: Send = Field(...)
+
+    def _construct_message(self, message_str: str) -> Message:
+        """Construct a Message from a string."""
+        return {"type": "http.response.body", "body": message_str, "more_body": True}
+
 
-class AsyncWebsocketCallback(AsyncCallbackHandler, BaseModel):
+class AsyncWebsocketCallback(AsyncLanarkyCallback):
     """Async Callback handler for FastAPI websocket connection."""
 
     websocket: WebSocket = Field(...)
     response: WebsocketResponse = Field(...)
 
-    class Config:
-        arbitrary_types_allowed = True
-
-    @property
-    def always_verbose(self) -> bool:
-        """Whether to call verbose callbacks even if verbose is False."""
-        return True
+    def _construct_message(self, message_str: str) -> dict:
+        """Construct a WebsocketResponse from a string."""
+        return {**self.response.dict(), **{"message": message_str}}
```

### Comparing `lanarky-0.6.2/lanarky/callbacks/llm.py` & `lanarky-0.6.3/lanarky/callbacks/llm.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 
 @register_streaming_callback("LLMChain")
 class AsyncLLMChainStreamingCallback(AsyncStreamingResponseCallback):
     """AsyncStreamingResponseCallback handler for LLMChain."""
 
     async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         """Run on new LLM token. Only available when streaming is enabled."""
-        await self.send(token)
+        message = self._construct_message(token)
+        await self.send(message)
 
 
 @register_websocket_callback("LLMChain")
 class AsyncLLMChainWebsocketCallback(AsyncWebsocketCallback):
     """AsyncWebsocketCallback handler for LLMChain."""
 
     async def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         """Run on new LLM token. Only available when streaming is enabled."""
-        await self.websocket.send_json({**self.response.dict(), **{"message": token}})
+        message = self._construct_message(token)
+        await self.websocket.send_json(message)
 
 
 @register_streaming_callback("ConversationChain")
 class AsyncConversationChainStreamingCallback(AsyncLLMChainStreamingCallback):
     """AsyncStreamingResponseCallback handler for ConversationChain."""
 
     pass
```

### Comparing `lanarky-0.6.2/lanarky/callbacks/qa_with_sources.py` & `lanarky-0.6.3/lanarky/callbacks/qa_with_sources.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.2/lanarky/callbacks/retrieval_qa.py` & `lanarky-0.6.3/lanarky/callbacks/retrieval_qa.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,49 +14,44 @@
     """AsyncStreamingResponseCallback handler for BaseRetrievalQA."""
 
     source_document_template: str = SOURCE_DOCUMENT_TEMPLATE
 
     async def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> None:
         """Run when chain ends running."""
         if "source_documents" in outputs:
-            await self.send("\n\nSOURCE DOCUMENTS: \n")
+            message = self._construct_message("\n\nSOURCE DOCUMENTS: \n")
+            await self.send(message)
             for document in outputs["source_documents"]:
-                await self.send(
+                message = self._construct_message(
                     self.source_document_template.format(
                         page_content=document.page_content,
                         source=document.metadata["source"],
                     )
                 )
+                await self.send(message)
 
 
 class AsyncBaseRetrievalQAWebsocketCallback(AsyncLLMChainWebsocketCallback):
     """AsyncWebsocketCallback handler for BaseRetrievalQA."""
 
     source_document_template: str = SOURCE_DOCUMENT_TEMPLATE
 
     async def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> None:
         """Run when chain ends running."""
         if "source_documents" in outputs:
-            await self.websocket.send_json(
-                {
-                    **self.response.dict(),
-                    **{"message": "\n\nSOURCE DOCUMENTS: \n"},
-                }
-            )
+            message = self._construct_message("\n\nSOURCE DOCUMENTS: \n")
+            await self.websocket.send_json(message)
             for document in outputs["source_documents"]:
-                source_document = self.source_document_template.format(
-                    page_content=document.page_content,
-                    source=document.metadata["source"],
-                )
-                await self.websocket.send_json(
-                    {
-                        **self.response.dict(),
-                        **{"message": source_document},
-                    }
+                message = self._construct_message(
+                    self.source_document_template.format(
+                        page_content=document.page_content,
+                        source=document.metadata["source"],
+                    )
                 )
+                await self.websocket.send_json(message)
 
 
 @register_streaming_callback("RetrievalQA")
 class AsyncRetrievalQAStreamingCallback(AsyncBaseRetrievalQAStreamingCallback):
     """AsyncStreamingResponseCallback handler for RetrievalQA."""
 
     pass
```

### Comparing `lanarky-0.6.2/lanarky/register.py` & `lanarky-0.6.3/lanarky/register.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Callable, Dict, List, Tuple
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 
 def register(key: str, _registry: Dict[str, Tuple[Any, List[str]]]) -> Any:
     """Add a class/function to a registry with required keyword arguments.
 
     ``_registry`` is a dictionary mapping from a key to a tuple of the class/function
     and a list of required keyword arguments, if keyword arguments are passed. Otherwise
     it is a dictionary mapping from a key to the class/function.
     """
 
-    def _register_cls(cls: Any, required_kwargs: List = None) -> Any:
+    def _register_cls(cls: Any, required_kwargs: Optional[List] = None) -> Any:
         if key in _registry:
             raise KeyError(f"{cls} already registered as {key}")
         _registry[key] = cls if required_kwargs is None else (cls, required_kwargs)
         return cls
 
     return _register_cls
```

### Comparing `lanarky-0.6.2/lanarky/responses/streaming.py` & `lanarky-0.6.3/lanarky/responses/streaming.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Credits:
 
 * `gist@ninely <https://gist.github.com/ninely/88485b2e265d852d3feb8bd115065b1a>`_
 * `langchain@#1705 <https://github.com/hwchase17/langchain/discussions/1706>`_
 """
-from typing import Any, Awaitable, Callable, Dict, Optional, Union
+from typing import Any, Awaitable, Callable, Optional, Union
 
 from fastapi.responses import StreamingResponse as _StreamingResponse
 from langchain.chains.base import Chain
 from starlette.background import BackgroundTask
 from starlette.types import Send
 
 from lanarky.callbacks import get_streaming_callback
@@ -32,21 +32,16 @@
             {
                 "type": "http.response.start",
                 "status": self.status_code,
                 "headers": self.raw_headers,
             }
         )
 
-        async def send_token(token: Union[str, bytes]):
-            if not isinstance(token, bytes):
-                token = token.encode(self.charset)
-            await send({"type": "http.response.body", "body": token, "more_body": True})
-
         try:
-            outputs = await self.chain_executor(send_token)
+            outputs = await self.chain_executor(send)
             if self.background is not None:
                 self.background.kwargs["outputs"] = outputs
         except Exception as e:
             if self.background is not None:
                 self.background.kwargs["outputs"] = str(e)
             await send(
                 {
@@ -57,31 +52,33 @@
             )
             return
 
         await send({"type": "http.response.body", "body": b"", "more_body": False})
 
     @staticmethod
     def _create_chain_executor(
-        chain: Chain, inputs: Union[Dict[str, Any], Any]
+        chain: Chain, inputs: Union[dict[str, Any], Any], **callback_kwargs
     ) -> Callable[[Send], Awaitable[Any]]:
         async def wrapper(send: Send):
             return await chain.acall(
-                inputs=inputs, callbacks=[get_streaming_callback(chain, send=send)]
+                inputs=inputs,
+                callbacks=[get_streaming_callback(chain, send=send, **callback_kwargs)],
             )
 
         return wrapper
 
     @classmethod
     def from_chain(
         cls,
         chain: Chain,
-        inputs: Union[Dict[str, Any], Any],
+        inputs: Union[dict[str, Any], Any],
         background: Optional[BackgroundTask] = None,
+        callback_kwargs: dict[str, Any] = {},
         **kwargs: Any,
     ) -> "StreamingResponse":
-        chain_executor = cls._create_chain_executor(chain, inputs)
+        chain_executor = cls._create_chain_executor(chain, inputs, **callback_kwargs)
 
         return cls(
             chain_executor=chain_executor,
             background=background,
             **kwargs,
         )
```

### Comparing `lanarky-0.6.2/lanarky/schemas.py` & `lanarky-0.6.3/lanarky/schemas.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.2/lanarky/testing/gradio.py` & `lanarky-0.6.3/lanarky/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.6.2/lanarky/websockets/base.py` & `lanarky-0.6.3/lanarky/websockets/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 Credits:
-- https://github.com/hwchase17/chat-langchain
-- https://github.com/pors/langchain-chat-websockets
+
+* `chat-langchain <https://github.com/hwchase17/chat-langchain>`_
+* `langchain-chat-websockets <https://github.com/pors/langchain-chat-websockets>`_
 """
 import logging
-from abc import abstractstaticmethod
 from typing import Any, Awaitable, Callable
 
 from fastapi import WebSocket, WebSocketDisconnect
 from langchain.chains.base import Chain
 from pydantic import BaseModel, Field
 
 from lanarky.callbacks import get_websocket_callback
 from lanarky.schemas import Message, MessageType, Sender, WebsocketResponse
 
 logger = logging.getLogger(__name__)
 
 
 class BaseWebsocketConnection(BaseModel):
     websocket: WebSocket = Field(...)
-    chain_executor: Callable[[], Awaitable[Any]] = Field(...)
+    chain_executor: Callable[[str], Awaitable[Any]] = Field(...)
 
     class Config:
         arbitrary_types_allowed = True
 
     async def connect(self):
         await self.websocket.accept()
         while True:
@@ -60,34 +60,37 @@
                     WebsocketResponse(
                         sender=Sender.BOT,
                         message=Message.ERROR,
                         message_type=MessageType.ERROR,
                     ).dict()
                 )
 
-    @abstractstaticmethod
+    @staticmethod
     def _create_chain_executor(
         chain: Chain,
         websocket: WebSocket,
         response: WebsocketResponse,
+        **callback_kwargs,
     ) -> Callable[[str], Awaitable[Any]]:
         raise NotImplementedError
 
     @classmethod
     def from_chain(
         cls,
         chain: Chain,
         websocket: WebSocket,
+        callback_kwargs: dict[str, Any] = {},
     ) -> "BaseWebsocketConnection":
         chain_executor = cls._create_chain_executor(
             chain,
             websocket,
             WebsocketResponse(
                 sender=Sender.BOT, message=Message.NULL, message_type=MessageType.STREAM
             ),
+            **callback_kwargs,
         )
 
         return cls(
             chain_executor=chain_executor,
             websocket=websocket,
         )
 
@@ -96,19 +99,23 @@
     """BaseLangchainStreamingResponse class wrapper for LLMChain instances."""
 
     @staticmethod
     def _create_chain_executor(
         chain: Chain,
         websocket: WebSocket,
         response: WebsocketResponse,
-    ) -> Callable[[], Awaitable[Any]]:
+        **callback_kwargs,
+    ) -> Callable[[str], Awaitable[Any]]:
         async def wrapper(user_message: str):
             return await chain.acall(
                 inputs=user_message,
                 callbacks=[
                     get_websocket_callback(
-                        chain=chain, websocket=websocket, response=response
+                        chain=chain,
+                        websocket=websocket,
+                        response=response,
+                        **callback_kwargs,
                     )
                 ],
             )
 
         return wrapper
```

### Comparing `lanarky-0.6.2/pyproject.toml` & `lanarky-0.6.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 [tool.poetry]
 name = "lanarky"
-version = "0.6.2"
+version = "0.6.3"
 description = "Ship production-ready LLM projects with FastAPI"
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ajndkr/lanarky"
 repository = "https://github.com/ajndkr/lanarky"
 license = "MIT"
 packages = [{include = "lanarky"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-fastapi = "^0.95.1"
-langchain = ">=0.0.172"
+fastapi = ">=0.95.2"
+langchain = ">=0.0.175"
 urllib3 = "<=1.26.15"  # added due to poetry errors
 python-dotenv = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.1"
 
 
 [tool.poetry.group.docs.dependencies]
 furo = "^2023.3.27"
 sphinx-autobuild = "^2021.3.14"
 
+
+[tool.poetry.group.tests.dependencies]
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+pytest-asyncio = "^0.21.0"
+coveralls = "^3.3.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 ignore = ["E501"]
```

### Comparing `lanarky-0.6.2/PKG-INFO` & `lanarky-0.6.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: lanarky
-Version: 0.6.2
+Version: 0.6.3
 Summary: Ship production-ready LLM projects with FastAPI
 Home-page: https://github.com/ajndkr/lanarky
 License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.95.1,<0.96.0)
-Requires-Dist: langchain (>=0.0.172)
+Requires-Dist: fastapi (>=0.95.2)
+Requires-Dist: langchain (>=0.0.175)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: urllib3 (<=1.26.15)
 Project-URL: Repository, https://github.com/ajndkr/lanarky
 Description-Content-Type: text/markdown
 
 <div align="center">
 
-<img src="assets/logo.png" alt="lanarky-logo" width="150">
+<img src="https://raw.githubusercontent.com/ajndkr/lanarky/main/assets/logo.png" alt="lanarky-logo" width="150">
 
 <h1> Lanarky </h1>
 
 [![stars](https://img.shields.io/github/stars/ajndkr/lanarky)](https://github.com/ajndkr/lanarky/stargazers)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/lanarky/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/lanarky.svg)](https://pypi.org/project/lanarky/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-3916/)
+[![Code Coverage](https://coveralls.io/repos/github/ajndkr/lanarky/badge.svg?branch=main)](https://coveralls.io/github/ajndkr/lanarky?branch=main)
 
 </div>
 
 Lanarky is an open-source framework to deploy LLM applications in production. It is built on top of [FastAPI](https://github.com/tiangolo/fastapi)
 and comes with batteries included.
 
 ## 🚀 Features
@@ -101,13 +102,13 @@
 
 [![Code check](https://github.com/ajndkr/lanarky/actions/workflows/code-check.yaml/badge.svg)](https://github.com/ajndkr/lanarky/actions/workflows/code-check.yaml)
 [![Publish](https://github.com/ajndkr/lanarky/actions/workflows/publish.yaml/badge.svg)](https://github.com/ajndkr/lanarky/actions/workflows/publish.yaml)
 
 Contributions are more than welcome! If you have an idea for a new feature or want to help improve lanarky,
 please create an issue or submit a pull request on [GitHub](https://github.com/ajndkr/lanarky).
 
-See [CONTRIBUTING.md](./CONTRIBUTING.md) for more information.
+See [CONTRIBUTING.md](https://github.com/ajndkr/lanarky/blob/main/CONTRIBUTING.md) for more information.
 
 ## ⚖️ License
 
 The library is released under the [MIT License](https://github.com/ajndkr/lanarky/blob/main/LICENSE).
```

