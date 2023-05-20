# Comparing `tmp/gpyt-0.2.8.tar.gz` & `tmp/gpyt-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpyt-0.2.8.tar", max compression
+gzip compressed data, was "gpyt-0.2.9.tar", max compression
```

## Comparing `gpyt-0.2.8.tar` & `gpyt-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      859 2023-05-05 06:36:00.377304 gpyt-0.2.8/README.md
--rw-r--r--   0        0        0     1964 2023-05-05 05:05:45.027304 gpyt-0.2.8/gpyt/__init__.py
--rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.8/gpyt/__main__.py
--rw-r--r--   0        0        0    15622 2023-05-05 06:26:52.067304 gpyt-0.2.8/gpyt/app.py
--rw-r--r--   0        0        0     3421 2023-05-05 04:58:02.177304 gpyt-0.2.8/gpyt/assistant.py
--rw-r--r--   0        0        0      187 2023-05-04 05:27:38.937304 gpyt-0.2.8/gpyt/conversation.py
--rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.8/gpyt/exception.py
--rw-r--r--   0        0        0      558 2023-05-05 05:00:41.717304 gpyt-0.2.8/gpyt/id.py
--rw-r--r--   0        0        0     1281 2023-05-05 06:09:18.137304 gpyt-0.2.8/gpyt/styles.cssx
--rw-r--r--   0        0        0      494 2023-05-05 06:36:30.377304 gpyt-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 gpyt-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      889 2023-05-05 17:50:29.707304 gpyt-0.2.9/README.md
+-rw-r--r--   0        0        0     2242 2023-05-05 07:34:22.177304 gpyt-0.2.9/gpyt/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.2.9/gpyt/__main__.py
+-rw-r--r--   0        0        0    16169 2023-05-05 18:37:37.767304 gpyt-0.2.9/gpyt/app.py
+-rw-r--r--   0        0        0     3421 2023-05-05 04:58:02.177304 gpyt-0.2.9/gpyt/assistant.py
+-rw-r--r--   0        0        0      187 2023-05-04 05:27:38.937304 gpyt-0.2.9/gpyt/conversation.py
+-rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.2.9/gpyt/exception.py
+-rw-r--r--   0        0        0      558 2023-05-05 05:00:41.717304 gpyt-0.2.9/gpyt/id.py
+-rw-r--r--   0        0        0     1326 2023-05-05 17:52:11.477304 gpyt-0.2.9/gpyt/styles.cssx
+-rw-r--r--   0        0        0      494 2023-05-05 18:39:47.397304 gpyt-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1459 1970-01-01 00:00:00.000000 gpyt-0.2.9/PKG-INFO
```

### Comparing `gpyt-0.2.8/README.md` & `gpyt-0.2.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -32,7 +32,8 @@
 - [ ] add gpt jailbreaks (DAN-esque)
 - [ ] add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
 - [ ] (informal) or -f (for file input) or --dan (for jailbreak)
 - [ ] model select CLI
 - [ ] add API_KEY from CLI
 - [ ] gpt4free integration (for 3.5 and 4)
 - [ ] refactor the f**k out of `app.py`
+- [ ] copy/pasting with mouse
```

### Comparing `gpyt-0.2.8/gpyt/__init__.py` & `gpyt-0.2.9/gpyt/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,20 +48,27 @@
 
 <the rest of your response>
 
 --end intermediate to complex topics instructions--
 """
 
 SUMMARY_PROMPT = "Summarize the user's input in 6 words or less. Try to capture the big idea. DO NOT USE more than 6 words and DO NOT answer their question. Simply echo back to them your summary."
-API_ERROR_FALLBACK = [
-    {
-        "choices": [
-            {"delta": {"content": "There was an error with OpenAI, try again later."}}
-        ]
-    }
-]
+
+API_ERROR_MESSAGE = """
+❗ There was an error with OpenAI.
+
+# Diagnostics
+
+Make sure that:
+    1) You have a proper OPENAI_API_KEY configured at `$HOME/.env` starting with "sk-"
+    2) You have configured Billing over at https://platform.openai.com/account/billing
+    3) You aren't getting rate limited (9000 tokens per minute)
+
+Try Again Later.
+"""
+API_ERROR_FALLBACK = [{"choices": [{"delta": {"content": API_ERROR_MESSAGE}}]}]
 
 
 INTRO = "Ask me anything. I'll try to assist you!"
 
 AVAILABLE_MODELS = ("gpt-3.5-turbo", "gpt4")
 MODEL = "gpt-3.5-turbo"
```

### Comparing `gpyt-0.2.8/gpyt/app.py` & `gpyt-0.2.9/gpyt/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+import pyperclip
 from pathlib import Path
 from typing import Callable, Generator
 from rich.style import Style
 
 from textual import work
 from textual.app import App, ComposeResult
 from textual.containers import Container, ScrollableContainer
@@ -63,15 +64,15 @@
             keyword_callback()
             return  # don't give anything to the assistant if we use a special callback
 
         app.fetch_assistant_response(user_input)
 
 
 class ConversationOption(ListItem):
-    ELLIPSIFY_CUTOFF = 36
+    ELLIPSIFY_CUTOFF = 35
 
     def __init__(self, conversation: Conversation):
         super().__init__()
         self.conversation = conversation
 
     def compose(self) -> ComposeResult:
         yield Label(self._ellipsify_long_summary(self.conversation.summary))
@@ -136,26 +137,31 @@
     """Each User/Assistant interaction"""
 
     def __init__(self, question: str = "", id: str = ""):
         super().__init__()
         self.question = question
         self._id = id
         self.response_view = Markdown()
+        self._last_content = ""
 
     def compose(self) -> ComposeResult:
         self.user_question = Label(f"😀: {self.question}", classes="convo")
         yield self.user_question
         yield Label("🤖:", classes="convo")
         container = Container(self.response_view, id="response-container")
         container.border_subtitle = f"message-id: 0x{self._id}"
         yield container
 
+    def on_click(self) -> None:
+        pyperclip.copy(self._last_content)
+
     @work()
     def update_response(self, content: str) -> None:
         app.call_from_thread(self.response_view.update, content)
+        self._last_content = content
 
 
 class AssistantResponses(Static):
     """Container for individual AssistantResponse widgets"""
 
     def __init__(self):
         super().__init__()
@@ -191,15 +197,16 @@
             new_response.update_response(assistant_response.content)
             new_history.append({"role": "user", "content": user_message.content})
             new_history.append(
                 {"role": "assistant", "content": assistant_response.content}
             )
 
         app.assistant.set_history(new_history)
-        app.action_toggle_sidebar()
+        app.past_conversations.add_class("hidden")
+        app.focus_user_input()
 
     @work()
     def add_response(self, stream: Generator, message: Message) -> None:
         new_response = AssistantResponse(question=message.content, id=message.id)
         app.call_from_thread(self.container.mount, new_response)
         app.call_from_thread(new_response.scroll_visible)
         markdown = ""
@@ -231,14 +238,16 @@
 class AssistantApp(App):
     """Base app for all user->assistant interactions"""
 
     BINDINGS = [
         ("ctrl+b", "toggle_dark", "Toggle Dark Mode"),
         ("ctrl+n", "toggle_sidebar", "Past Conversations"),
         ("ctrl+c", "handle_exit", "Quit"),
+        ("up", "scroll_convo_up", "Scroll Up Convo"),
+        ("down", "scroll_convo_down", "Scroll Down Convo"),
     ]
 
     CSS_PATH = "styles.cssx"
 
     def __init__(self, assistant: Assistant):
         super().__init__()
         self.assistant = assistant
@@ -416,14 +425,20 @@
     def focus_user_input(self) -> None:
         inp = self.query_one("#user-input")
         inp.focus()
 
     def action_handle_exit(self) -> None:
         exit()
 
+    def action_scroll_convo_up(self) -> None:
+        self.assistant_responses.container.scroll_relative(y=-4)
+
+    def action_scroll_convo_down(self) -> None:
+        self.assistant_responses.container.scroll_relative(y=4)
+
 
 class gpyt(AssistantApp):
     """Used strictly for the purposes of renaming the Header widget."""
 
     def __init__(self, assistant: Assistant):
         super().__init__(assistant=assistant)
```

### Comparing `gpyt-0.2.8/gpyt/assistant.py` & `gpyt-0.2.9/gpyt/assistant.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.8/gpyt/id.py` & `gpyt-0.2.9/gpyt/id.py`

 * *Files identical despite different names*

### Comparing `gpyt-0.2.8/gpyt/styles.cssx` & `gpyt-0.2.9/gpyt/styles.cssx`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,17 @@
 }
 
 PastConversations {
   layer: overlay;
   margin-top: 1;
   width: 40;
   height: 60%;
-  border: panel $panel-lighten-2;
-  border-title-color: rgb(225,225,225);
+  border: panel $primary-background-lighten-1;
+  border-title-color: rgb(225, 225, 225);
+  border-title-align: center;
   background: $panel;
   transition: offset 400ms in_back;
 }
 
 PastConversations:focus-within {
   offset-x: 0 !important;
 }
```

### Comparing `gpyt-0.2.8/PKG-INFO` & `gpyt-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpyt
-Version: 0.2.8
+Version: 0.2.9
 Summary: GPT on the command line.
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.5,<0.28.0)
@@ -49,8 +49,9 @@
 - [ ] add gpt jailbreaks (DAN-esque)
 - [ ] add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
 - [ ] (informal) or -f (for file input) or --dan (for jailbreak)
 - [ ] model select CLI
 - [ ] add API_KEY from CLI
 - [ ] gpt4free integration (for 3.5 and 4)
 - [ ] refactor the f**k out of `app.py`
+- [ ] copy/pasting with mouse
```

