# Comparing `tmp/AIPrompts-0.4.0.tar.gz` & `tmp/AIPrompts-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIPrompts-0.4.0.tar", last modified: Fri May  5 01:56:56 2023, max compression
+gzip compressed data, was "AIPrompts-0.5.0.tar", last modified: Sun May 21 00:58:49 2023, max compression
```

## Comparing `AIPrompts-0.4.0.tar` & `AIPrompts-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:56:56.391970 AIPrompts-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:56:56.387970 AIPrompts-0.4.0/AIPrompts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-05 01:56:56.000000 AIPrompts-0.4.0/AIPrompts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-05 01:56:56.000000 AIPrompts-0.4.0/AIPrompts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:56:56.000000 AIPrompts-0.4.0/AIPrompts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 01:56:56.000000 AIPrompts-0.4.0/AIPrompts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 01:56:56.000000 AIPrompts-0.4.0/AIPrompts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-05 01:56:56.391970 AIPrompts-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:56:56.391970 AIPrompts-0.4.0/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/turbo.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 01:56:56.391970 AIPrompts-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:56:56.391970 AIPrompts-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/tests/test_turbo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:58:49.847573 AIPrompts-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:58:49.843572 AIPrompts-0.5.0/AIPrompts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-21 00:58:49.000000 AIPrompts-0.5.0/AIPrompts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-21 00:58:49.000000 AIPrompts-0.5.0/AIPrompts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:58:49.000000 AIPrompts-0.5.0/AIPrompts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-21 00:58:49.000000 AIPrompts-0.5.0/AIPrompts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 00:58:49.000000 AIPrompts-0.5.0/AIPrompts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-21 00:58:49.847573 AIPrompts-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:58:49.847573 AIPrompts-0.5.0/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/prompts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:58:49.847573 AIPrompts-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:58:49.847573 AIPrompts-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-21 00:58:26.000000 AIPrompts-0.5.0/tests/test_turbo.py
```

### Comparing `AIPrompts-0.4.0/AIPrompts.egg-info/PKG-INFO` & `AIPrompts-0.5.0/AIPrompts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPrompts
-Version: 0.4.0
+Version: 0.5.0
 Summary: Create and parse prompts for large language models.
 Home-page: https://github.com/TeiaLabs/prompts
 Author: Teialabs
 Author-email: jonatas@teialabs.com
 Keywords: prompt openai teialabs gpt3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `AIPrompts-0.4.0/PKG-INFO` & `AIPrompts-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPrompts
-Version: 0.4.0
+Version: 0.5.0
 Summary: Create and parse prompts for large language models.
 Home-page: https://github.com/TeiaLabs/prompts
 Author: Teialabs
 Author-email: jonatas@teialabs.com
 Keywords: prompt openai teialabs gpt3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `AIPrompts-0.4.0/README.md` & `AIPrompts-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.4.0/prompts/dynamic.py` & `AIPrompts-0.5.0/prompts/dynamic.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.4.0/prompts/ensemble.py` & `AIPrompts-0.5.0/prompts/ensemble.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.4.0/prompts/exceptions.py` & `AIPrompts-0.5.0/prompts/exceptions.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.4.0/prompts/schemas.py` & `AIPrompts-0.5.0/prompts/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 from typing import Optional
 
 from pydantic import BaseModel, Field
 
 
 # ==== Generic classes ====
 class OpenAIModelSettings(BaseModel):
-    engine: str
+    model: str
     max_tokens: int = 256
     temperature: float = 0.0
     top_p: float = 1
     frequency_penalty: float = 0
     presence_penalty: float = 0
+    logit_bias: dict[int, int] | None = None
     stop: list[str] = Field(default_factory=list)
+    n: int = 1
+    user: str | None = None
 
 
-class PromptSchema(BaseModel):
+# ==== Dynamic classes ====
+class DynamicSchema(BaseModel):
     # Prompt identification
     name: str
     description: str = ""
 
     # Engine settings
     settings: OpenAIModelSettings
-
-
-# ==== Dynamic classes ====
-class DynamicSchema(PromptSchema):
     template: str
 
 
 # ==== Turbo classes ====
 class Template(BaseModel):
     template_name: str
     template: str
@@ -57,17 +57,21 @@
     name: str | None = None
     role: PromptRole
 
     # Prompts template management
     template_name: str = "default"
 
 
-class TurboSchema(PromptSchema):
+class TurboSchema(BaseModel):
+    # Prompt identification
+    name: str
+    description: str = ""
+    # Engine settings
+    settings: OpenAIModelSettings
     # Prompt templates
     system_templates: list[Template] | str
     user_templates: list[Template] | str
     assistant_templates: list[Template] | str
-
     # Prompt initial config
     initial_template_data: list[TemplateData | TemplateContent] = Field(
         default_factory=list
     )
```

### Comparing `AIPrompts-0.4.0/prompts/turbo.py` & `AIPrompts-0.5.0/prompts/turbo.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.4.0/setup.py` & `AIPrompts-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.4.0/tests/test_ensemble.py` & `AIPrompts-0.5.0/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.4.0/tests/test_prompt.py` & `AIPrompts-0.5.0/tests/test_prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from prompts import DynamicPrompt, exceptions
+from prompts import DynamicPrompt, exceptions, OpenAIModelSettings
 
 
 class TestPrompt:
     
     template = 'a photo of a <img_label>'
     template_vars = ['img_label']
 
@@ -19,18 +19,18 @@
             'lets go\n'
             '\n'
             'Fixed sentence:\n'
         ))
         assert expected_prompt == prompt_str
 
         settings = prompt.settings
-        assert isinstance(settings, dict)
-        assert isinstance(settings['temperature'], float)
-        assert settings['temperature'] == 0.15
-        assert settings['engine'] == 'text-davinci-003'
+        assert isinstance(settings, OpenAIModelSettings)
+        assert isinstance(settings.temperature, float)
+        assert settings.temperature == 0.15
+        assert settings.model == 'text-davinci-003'
 
     @staticmethod
     def test_str_prompt():
 
         prompt = DynamicPrompt(TestPrompt.template, TestPrompt.template_vars)
         filled_prompt = prompt.build(img_label='dog')
         assert filled_prompt == 'a photo of a dog'
```

### Comparing `AIPrompts-0.4.0/tests/test_turbo.py` & `AIPrompts-0.5.0/tests/test_turbo.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     assert tp.name == "basic_turbo_prompt"
     assert tp.description == "Basic turbo prompt example"
     from prompts.schemas import OpenAIModelSettings
 
     assert tp.settings == OpenAIModelSettings(
         **{
             "temperature": 0.15,
-            "engine": "gpt-3.5-turbo",
+            "model": "gpt-3.5-turbo",
             "max_tokens": 32,
         }
     )
 
 
 def test_from_file_with_initial_template_data():
     tp = TurboPrompt.from_file("samples/sample.past.yaml")
@@ -127,15 +127,15 @@
     assert tp.name == "turbo_prompt_with_examples"
     assert (
         tp.description
         == "Example of turbo prompt with initial_template_data (few-shot)"
     )
     sets = tp.settings
     assert sets is not None
-    assert sets.engine == "gpt-3.5-turbo"
+    assert sets.model == "gpt-3.5-turbo"
 
 
 def test_a_from_settings():
     tp = TurboPrompt.from_file("samples/complex.yaml")
     built = tp.build()
     assert isinstance(built, list)
     assert isinstance(built[0], dict)
@@ -144,15 +144,15 @@
 
     tp = TurboPrompt.from_settings(
         name="turbo_prompt_inline",
         description="",
         system_template="You are an AI",
         user_template="Q:<message>",
         assistant_template="A:",
-        settings=OpenAIModelSettings(engine="gpt-4"),
+        settings=OpenAIModelSettings(model="gpt-4"),
         initial_template_data=[
             TemplateContent(
                 content="hey", template_name="default", role=PromptRole.SYSTEM
             )
         ],
     )
```

