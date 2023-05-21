# Comparing `tmp/devchat-0.1.6.tar.gz` & `tmp/devchat-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devchat-0.1.6.tar", last modified: Fri May 19 17:53:58 2023, max compression
+gzip compressed data, was "devchat-0.1.7.tar", last modified: Sun May 21 11:37:41 2023, max compression
```

## Comparing `devchat-0.1.6.tar` & `devchat-0.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-19 17:53:58.898735 devchat-0.1.6/
--rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-05-05 13:17:54.000000 devchat-0.1.6/LICENSE
--rw-r--r--   0 basicthinker   (501) staff       (20)      415 2023-05-19 17:53:58.898580 devchat-0.1.6/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)     3584 2023-05-19 17:28:29.000000 devchat-0.1.6/README.md
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-19 17:53:58.894792 devchat-0.1.6/devchat/
--rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.6/devchat/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5660 2023-05-18 09:46:55.000000 devchat-0.1.6/devchat/_cli.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     4552 2023-05-12 00:41:47.000000 devchat-0.1.6/devchat/assistant.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1464 2023-05-05 13:17:54.000000 devchat-0.1.6/devchat/chat.py
--rw-r--r--   0 basicthinker   (501) staff       (20)      614 2023-05-07 23:44:52.000000 devchat-0.1.6/devchat/message.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-19 17:53:58.896829 devchat-0.1.6/devchat/openai/
--rw-r--r--   0 basicthinker   (501) staff       (20)      248 2023-05-05 13:17:54.000000 devchat-0.1.6/devchat/openai/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3399 2023-05-18 09:47:11.000000 devchat-0.1.6/devchat/openai/openai_chat.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1561 2023-05-07 23:44:52.000000 devchat-0.1.6/devchat/openai/openai_message.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     6017 2023-05-18 05:09:41.000000 devchat-0.1.6/devchat/openai/openai_prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     6447 2023-05-12 00:56:54.000000 devchat-0.1.6/devchat/prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     3704 2023-05-19 17:29:57.000000 devchat-0.1.6/devchat/store.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     4981 2023-05-12 00:21:13.000000 devchat-0.1.6/devchat/utils.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-19 17:53:58.895860 devchat-0.1.6/devchat.egg-info/
--rw-r--r--   0 basicthinker   (501) staff       (20)      415 2023-05-19 17:53:58.000000 devchat-0.1.6/devchat.egg-info/PKG-INFO
--rw-r--r--   0 basicthinker   (501) staff       (20)      628 2023-05-19 17:53:58.000000 devchat-0.1.6/devchat.egg-info/SOURCES.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-05-19 17:53:58.000000 devchat-0.1.6/devchat.egg-info/dependency_links.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-05-19 17:53:58.000000 devchat-0.1.6/devchat.egg-info/entry_points.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)      116 2023-05-19 17:53:58.000000 devchat-0.1.6/devchat.egg-info/requires.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)       14 2023-05-19 17:53:58.000000 devchat-0.1.6/devchat.egg-info/top_level.txt
--rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-05-05 13:17:54.000000 devchat-0.1.6/pyproject.toml
--rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-05-19 17:53:58.898773 devchat-0.1.6/setup.cfg
--rw-r--r--   0 basicthinker   (501) staff       (20)      770 2023-05-19 17:52:56.000000 devchat-0.1.6/setup.py
-drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-19 17:53:58.898284 devchat-0.1.6/tests/
--rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.6/tests/__init__.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5996 2023-05-12 00:42:14.000000 devchat-0.1.6/tests/test_cli.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1809 2023-05-07 23:44:52.000000 devchat-0.1.6/tests/test_openai_message.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     5908 2023-05-12 00:53:18.000000 devchat-0.1.6/tests/test_openai_prompt.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     2303 2023-05-05 15:34:17.000000 devchat-0.1.6/tests/test_store.py
--rw-r--r--   0 basicthinker   (501) staff       (20)     1225 2023-05-07 23:44:52.000000 devchat-0.1.6/tests/test_utils.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-21 11:37:41.706506 devchat-0.1.7/
+-rw-r--r--   0 basicthinker   (501) staff       (20)    11357 2023-05-05 13:17:54.000000 devchat-0.1.7/LICENSE
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5174 2023-05-21 11:37:41.706358 devchat-0.1.7/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4718 2023-05-21 11:37:13.000000 devchat-0.1.7/README.md
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-21 11:37:41.702882 devchat-0.1.7/devchat/
+-rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.7/devchat/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5660 2023-05-18 09:46:55.000000 devchat-0.1.7/devchat/_cli.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4552 2023-05-12 00:41:47.000000 devchat-0.1.7/devchat/assistant.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1464 2023-05-05 13:17:54.000000 devchat-0.1.7/devchat/chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)      614 2023-05-07 23:44:52.000000 devchat-0.1.7/devchat/message.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-21 11:37:41.704681 devchat-0.1.7/devchat/openai/
+-rw-r--r--   0 basicthinker   (501) staff       (20)      248 2023-05-05 13:17:54.000000 devchat-0.1.7/devchat/openai/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3399 2023-05-18 09:47:11.000000 devchat-0.1.7/devchat/openai/openai_chat.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1561 2023-05-07 23:44:52.000000 devchat-0.1.7/devchat/openai/openai_message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     6017 2023-05-18 05:09:41.000000 devchat-0.1.7/devchat/openai/openai_prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     6447 2023-05-12 00:56:54.000000 devchat-0.1.7/devchat/prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     3704 2023-05-19 17:29:57.000000 devchat-0.1.7/devchat/store.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     4981 2023-05-12 00:21:13.000000 devchat-0.1.7/devchat/utils.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-21 11:37:41.703837 devchat-0.1.7/devchat.egg-info/
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5174 2023-05-21 11:37:41.000000 devchat-0.1.7/devchat.egg-info/PKG-INFO
+-rw-r--r--   0 basicthinker   (501) staff       (20)      628 2023-05-21 11:37:41.000000 devchat-0.1.7/devchat.egg-info/SOURCES.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)        1 2023-05-21 11:37:41.000000 devchat-0.1.7/devchat.egg-info/dependency_links.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)       46 2023-05-21 11:37:41.000000 devchat-0.1.7/devchat.egg-info/entry_points.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)      116 2023-05-21 11:37:41.000000 devchat-0.1.7/devchat.egg-info/requires.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)       14 2023-05-21 11:37:41.000000 devchat-0.1.7/devchat.egg-info/top_level.txt
+-rw-r--r--   0 basicthinker   (501) staff       (20)      102 2023-05-05 13:17:54.000000 devchat-0.1.7/pyproject.toml
+-rw-r--r--   0 basicthinker   (501) staff       (20)       38 2023-05-21 11:37:41.706543 devchat-0.1.7/setup.cfg
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1112 2023-05-21 11:37:27.000000 devchat-0.1.7/setup.py
+drwxr-xr-x   0 basicthinker   (501) staff       (20)        0 2023-05-21 11:37:41.706060 devchat-0.1.7/tests/
+-rw-r--r--   0 basicthinker   (501) staff       (20)        0 2023-05-05 13:17:54.000000 devchat-0.1.7/tests/__init__.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5996 2023-05-12 00:42:14.000000 devchat-0.1.7/tests/test_cli.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1809 2023-05-07 23:44:52.000000 devchat-0.1.7/tests/test_openai_message.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     5908 2023-05-12 00:53:18.000000 devchat-0.1.7/tests/test_openai_prompt.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     2303 2023-05-05 15:34:17.000000 devchat-0.1.7/tests/test_store.py
+-rw-r--r--   0 basicthinker   (501) staff       (20)     1225 2023-05-07 23:44:52.000000 devchat-0.1.7/tests/test_utils.py
```

### Comparing `devchat-0.1.6/LICENSE` & `devchat-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/README.md` & `devchat-0.1.7/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -15,81 +15,97 @@
 
 </div>
 <br>
 <div align="left">
 
 The DevChat core library and CLI.
 
-:point_right: For a better experience, check out our [Visual Studio Code extension](https://github.com/covespace/devchat-vscode) on [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=merico.devchat)! Install and enjoy the enhanced UI :clap:
-
-
-
-https://github.com/covespace/devchat/assets/592493/76e997fe-33a3-4fee-8f67-5523df90316e
-
-
+👉 For a better experience, check out our [Visual Studio Code extension](https://github.com/covespace/devchat-vscode) on [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=merico.devchat)! Install and enjoy the enhanced UI 👏
 
 ***
 
 ## What is DevChat?
 
 DevChat is an open-source tool that helps you write prompts to generate code and documentation.
 It is _not_ limited to performing predefined operations on short code snippets.
   
 DevChat is the way developers interact and collaborate with AI.
 
-:speech_balloon: Build the future with prompts, _not_ code.
+💬 Build the future with prompts, _not_ code.
 
 ## Why DevChat?
 
 - To enable AI to write code, DevChat assists you in providing **the right context** for AI.
   
+  ![20230519-231038-00 00 00 000-00 00 20 989](https://github.com/covespace/devchat-vscode/assets/592493/cfb96c7f-bd45-4573-810e-17148aac79d1)
+  
   Chat history, code, files, directory trees, `git diff --cached`, or the output of any command.
 
-  <img width="500" alt="image" src="https://github.com/covespace/devchat-vscode/assets/592493/415df4aa-66d6-46e4-a30d-8bba6277028c">
- 
 - To apply AI-generated code, DevChat streamlines your **actions to take**.
 
-  View diffs, copy or insert, commit & sync, or export to documentation, wikis, and more.
+  ![20230519-231038-00 00 24 989-00 00 44 688](https://github.com/covespace/devchat-vscode/assets/592493/2a0c4acf-6801-409c-bb18-ac75bae96938)
   
-  <img width="500" alt="image" src="https://github.com/covespace/devchat-vscode/assets/592493/bcccbf20-0d30-46f4-b19f-5f532c1caf85">
+  View diffs, copy or insert, commit & sync, or export to documentation, wikis, and more.
   
 - To guide AI in your work, define **your own workflows** with DevChat.
   
-  Prompt templates, iterative calls to AI, and program operations.
+  ![20230519-231038-00 00 45 034-00 01 00 000](https://github.com/covespace/devchat-vscode/assets/592493/5a72e43f-0ed9-446a-81be-3e5f00009961)
+  
+  More prompt templates, iterative calls to AI, and program operations.
 
 - To suit your preferences, customize **your own experiences** with DevChat.
   
   Open-source, no waiting for opaque feature schedules. Access GPT-4 today and more models in the future.
   
 ## What is Prompt-Centric Software Development (PSSD)?
 
 - The traditional code-centric paradigm is evolving.
 
 - Write prompts to create code. Transform prompts into everything.
 
+  <img width="600" alt="image" src="https://github.com/covespace/devchat/assets/592493/dd32e900-92fd-4fa4-8489-96ed17ab5e0e">
+
+  <sub>(This image is licensed by devchat.ai under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.)</sub>
+  
 - It is DevPromptOps
   
   <img width="500" alt="image" src="https://github.com/covespace/devchat/assets/592493/e8e1215b-53b0-4473-ab00-0665d33f204a">
-
+  
+  <sub>(This image is licensed by devchat.ai under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.)</sub>
 
 ***
 
 ## Quick Start
 
-- Install DevChat by running: `pip install devchat`
-- Make sure you are in a Git repository, as DevChat only works within one.
-- To access help, use the commands: `devchat --help` and `devchat prompt --help`
+For UI, install the [Visual Studio Code extension](https://github.com/covespace/devchat-vscode) from [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=merico.devchat).
+
+For CLI:
+- Install DevChat by running: `pip install devchat`.
+- Make sure you are working in a Git repository, as DevChat only works within one.
+- Set your [OpenAI API Key](https://platform.openai.com/account/api-keys) by running `export OPENAI_API_KEY="[sk-...]"`.
+- To access help, use the commands: `devchat --help` and `devchat prompt --help`.
 
 ## Community
 
 - Join our [Discord](https://discord.gg/9t3yrbBUXD)!
 
 - Participate in [discussions](https://github.com/covespace/devchat/discussions)!
 
+## Contributing
+
+Issues and pull request are welcome: https://github.com/covespace/devchat/issues
+  
 ## Roadmap
 
 - [x] Implement code diff application.
 - [ ] Improve code diff application using code change instructions.
 - [ ] Develop a framework for defining workflows.
 - [ ] Implement topic management.
 - [ ] Enable interaction with external development tools.
 - [ ] Introduce more selective workflows.
+  
+## Contact
+  
+hello@merico.dev
+
+We are creators of [Apache DevLake](https://devlake.apache.org/).
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `devchat-0.1.6/devchat/_cli.py` & `devchat-0.1.7/devchat/_cli.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/devchat/assistant.py` & `devchat-0.1.7/devchat/assistant.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/devchat/chat.py` & `devchat-0.1.7/devchat/chat.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/devchat/message.py` & `devchat-0.1.7/devchat/message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/devchat/openai/openai_chat.py` & `devchat-0.1.7/devchat/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/devchat/openai/openai_message.py` & `devchat-0.1.7/devchat/openai/openai_message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/devchat/openai/openai_prompt.py` & `devchat-0.1.7/devchat/openai/openai_prompt.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/devchat/prompt.py` & `devchat-0.1.7/devchat/prompt.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/devchat/store.py` & `devchat-0.1.7/devchat/store.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/devchat/utils.py` & `devchat-0.1.7/devchat/utils.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/devchat.egg-info/SOURCES.txt` & `devchat-0.1.7/devchat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/tests/test_cli.py` & `devchat-0.1.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/tests/test_openai_message.py` & `devchat-0.1.7/tests/test_openai_message.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/tests/test_openai_prompt.py` & `devchat-0.1.7/tests/test_openai_prompt.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/tests/test_store.py` & `devchat-0.1.7/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `devchat-0.1.6/tests/test_utils.py` & `devchat-0.1.7/tests/test_utils.py`

 * *Files identical despite different names*

