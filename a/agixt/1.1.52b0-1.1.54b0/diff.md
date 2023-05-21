# Comparing `tmp/agixt-1.1.52b0.tar.gz` & `tmp/agixt-1.1.54b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agixt-1.1.52b0.tar", last modified: Sun May 21 00:41:02 2023, max compression
+gzip compressed data, was "agixt-1.1.54b0.tar", last modified: Sun May 21 04:01:23 2023, max compression
```

## Comparing `agixt-1.1.52b0.tar` & `agixt-1.1.54b0.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.542321 agixt-1.1.52b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-21 00:40:48.000000 agixt-1.1.52b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-21 00:40:48.000000 agixt-1.1.52b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-05-21 00:41:02.542321 agixt-1.1.52b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.534321 agixt-1.1.52b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-05-21 00:40:48.000000 agixt-1.1.52b0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 00:40:48.000000 agixt-1.1.52b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 00:41:02.542321 agixt-1.1.52b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-21 00:40:48.000000 agixt-1.1.52b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.534321 agixt-1.1.52b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.538321 agixt-1.1.52b0/src/agixt/
--rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/AGiXT.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.538321 agixt-1.1.52b0/src/agixt/Config/
--rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Config/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/CustomPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Memories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/Tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.542321 agixt-1.1.52b0/src/agixt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/bing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/claude.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/fastchat.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/gpugpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/kobold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/llamacpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/oobabooga.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/provider/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 00:40:48.000000 agixt-1.1.52b0/src/agixt/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:41:02.538321 agixt-1.1.52b0/src/agixt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-05-21 00:41:02.000000 agixt-1.1.52b0/src/agixt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-21 00:41:02.000000 agixt-1.1.52b0/src/agixt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:41:02.000000 agixt-1.1.52b0/src/agixt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-21 00:41:02.000000 agixt-1.1.52b0/src/agixt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 00:41:02.000000 agixt-1.1.52b0/src/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:01:23.788818 agixt-1.1.54b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-21 04:01:12.000000 agixt-1.1.54b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-21 04:01:12.000000 agixt-1.1.54b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-21 04:01:23.788818 agixt-1.1.54b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:01:23.784818 agixt-1.1.54b0/agixt/
+-rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/AGiXT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:01:23.784818 agixt-1.1.54b0/agixt/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)    14046 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Config/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/CustomPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Memories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/Tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:01:23.788818 agixt-1.1.54b0/agixt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/bing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/claude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/fastchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/gpugpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/kobold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/llamacpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/oobabooga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/provider/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 04:01:12.000000 agixt-1.1.54b0/agixt/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:01:23.784818 agixt-1.1.54b0/agixt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-21 04:01:23.000000 agixt-1.1.54b0/agixt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-21 04:01:23.000000 agixt-1.1.54b0/agixt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 04:01:23.000000 agixt-1.1.54b0/agixt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-21 04:01:23.000000 agixt-1.1.54b0/agixt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 04:01:23.000000 agixt-1.1.54b0/agixt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:01:23.788818 agixt-1.1.54b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-21 04:01:12.000000 agixt-1.1.54b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 04:01:12.000000 agixt-1.1.54b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 04:01:23.788818 agixt-1.1.54b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 04:01:12.000000 agixt-1.1.54b0/setup.py
```

### Comparing `agixt-1.1.52b0/LICENSE` & `agixt-1.1.54b0/LICENSE`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/PKG-INFO` & `agixt-1.1.54b0/docs/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,55 @@
-Metadata-Version: 2.1
-Name: agixt
-Version: 1.1.52b0
-Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
-Author: Josh XT
-Author-email: josh@devxt.com
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AGiXT
 ![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic) 
 [![STATUS](https://img.shields.io/badge/status-beta-blue?label=Release%20Status&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
 
 [![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 [![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/Agent-LLM-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/labels/help%20wanted) 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT) 
 [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) 
 
-![Logo](AGiXT.svg)
+![Logo](images/AGiXT.svg)
 
 AGiXT is a dynamic Artificial Intelligence Automation Platform engineered to orchestrate efficient AI instruction management and task execution across a multitude of providers. Our solution infuses adaptive memory handling with a broad spectrum of commands to enhance AI's understanding and responsiveness, leading to improved task completion. The platform's smart features, like Smart Instruct and Smart Chat, seamlessly integrate web search, planning strategies, and conversation continuity, transforming the interaction between users and AI. By leveraging a powerful plugin system that includes web browsing and command execution, AGiXT stands as a versatile bridge between AI models and users. With an expanding roster of AI providers, code evaluation capabilities, comprehensive chain management, and platform interoperability, AGiXT is consistently evolving to drive a multitude of applications, affirming its place at the forefront of AI technology.
 
 Embracing the spirit of extremity in every facet of life, we introduce AGiXT. This advanced AI Automation Platform is our bold step towards the realization of Artificial General Intelligence (AGI). Seamlessly orchestrating instruction management and executing complex tasks across diverse AI providers, AGiXT combines adaptive memory, smart features, and a versatile plugin system to maximize AI potential. With our unwavering commitment to innovation, we're dedicated to pushing the boundaries of AI and bringing AGI closer to reality.
 
-## ⚠️ Monitor Your Usage!
-Please note that using some AI providers (such as OpenAI's GPT-4 API) can be expensive! Monitor your usage carefully to avoid incurring unexpected costs.  We're **NOT** responsible for your usage under any circumstance.
-
-## ⚠️ Under Development!
-This project is under active development and may still have issues. We appreciate your understanding and patience. If you encounter any problems, please first check the open issues. If your issue is not listed, kindly create a new issue detailing the error or problem you experienced. Thank you for your support!
-
 ## Table of Contents 📖
 
 - [AGiXT](#agixt)
-  - [⚠️ Monitor Your Usage!](#️-monitor-your-usage)
-  - [⚠️ Under Development!](#️-under-development)
   - [Table of Contents 📖](#table-of-contents-)
-  - [Media Coverage ⏯️](#media-coverage-️)
-    - [Video](#video)
+  - [⚠️ Disclaimers!](#️-disclaimers)
+    - [Monitor Your Usage!](#monitor-your-usage)
+    - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
-  - [Run with Docker](#run-with-docker)
-    - [Linux or Windows](#linux-or-windows)
+  - [Quickstart with Docker](#quickstart-with-docker)
     - [Windows Docker Desktop (streamlit only example)](#windows-docker-desktop-streamlit-only-example)
+    - [Alternative Docker Compose Profiles](#alternative-docker-compose-profiles)
     - [Development using docker](#development-using-docker)
   - [Local Development](#local-development)
+    - [API Endpoints](#api-endpoints)
   - [Configuration](#configuration)
-  - [API Endpoints](#api-endpoints)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
   - [Acknowledgments](#acknowledgments)
   - [History](#history)
 
-## Media Coverage ⏯️
-
-### Video
-- From [World of AI](https://www.youtube.com/@intheworldofai) on YouTube: [AGiXT: AI Automation Bot for Managing and Implementing AI Through Applications](https://www.youtube.com/watch?v=g0_36Mf2-To)
+## ⚠️ Disclaimers!
+### Monitor Your Usage!
+Please note that using some AI providers (such as OpenAI's GPT-4 API) can be expensive! Monitor your usage carefully to avoid incurring unexpected costs.  We're **NOT** responsible for your usage under any circumstance.
 
+### Under Development!
+This project is under active development and may still have issues. We appreciate your understanding and patience. If you encounter any problems, please first check the open issues. If your issue is not listed, kindly create a new issue detailing the error or problem you experienced. Thank you for your support!
 
 ## Key Features 🗝️
 
 - **Context and Token Management**: Adaptive handling of long-term and short-term memory for an optimized AI performance, allowing the software to process information more efficiently and accurately.
 - **Smart Instruct**: An advanced feature enabling AI to comprehend, plan, and execute tasks effectively. The system leverages web search, planning strategies, and executes instructions while ensuring output accuracy.
 - **Interactive Chat & Smart Chat**: User-friendly chat interface for dynamic conversational tasks. The Smart Chat feature integrates AI with web research to deliver accurate and contextually relevant responses.
 - **Task Execution & Smart Task Management**: Efficient management and execution of complex tasks broken down into sub-tasks. The Smart Task feature employs AI-driven agents to dynamically handle tasks, optimizing efficiency and avoiding redundancy.
@@ -76,72 +60,70 @@
 - **Docker Deployment**: Simplified setup and maintenance through Docker deployment.
 - **Audio-to-Text & Text-to-Speech Options**: Integration with Hugging Face for seamless audio-to-text transcription, and multiple TTS choices, featuring Brian TTS, Mac OS TTS, and ElevenLabs.
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
-## Run with Docker
-Clone the repositories for the AGiXT front/back ends then start the services with Docker.
-
-### Linux or Windows
+## Quickstart with Docker
+Download the `docker-compose` file and run the AGiXT Streamlit Web App.
 ```
-git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.yml
+docker compose --profile streamlit up
 ```
 
-Choose a service you want to run using profiles, e.g.
-`docker compose --profile streamlit up`
-
-Run all available services
-`docker compose --profile all up`
-
 - Web Interface http://localhost:8501
-
 ### Windows Docker Desktop (streamlit only example)
 - Container Name: AGiXT
 - Host Port: 8501:8501/tcp
 
+### Alternative Docker Compose Profiles
+
+Run all available services, this includes the FastAPI back end (Port 7437) and NextJS front end (Port 3000).
+```
+docker compose --profile all up
+```
+
 ### Development using docker
 ```
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.yml
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.dev.yml
 docker compose --profile all -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
 ## Local Development
 
 Clone the repository for the AGiXT back end and start it.
 
 ```
 git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT/src/agixt
+cd AGiXT/agixt
 pip install -r requirements.txt
 streamlit run streamlit.py
 ```
 
 Access the web interface at http://localhost:8501
 
-## Configuration
-
-Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
-
-## API Endpoints
+### API Endpoints
 
 AGiXT provides several API endpoints for managing agents, prompts and chains.
 
 If you're not running with Docker, the back end can be run with:
 ```
-python src/agixt/app.py
+python agixt/app.py
 ```
 
 To learn more about the API endpoints and their usage, visit the API documentation at 
 - [Swagger](http://localhost:7437)
 - [Redoc](http://localhost:7437/redoc)
 
 This documentation is hosted locally and the frontend must be running for these links to work.
+## Configuration
 
+Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
 ## Documentation
 
 Not enough information? Check out the [documentation](https://josh-xt.github.io/AGiXT) for more details.
 
 ## Contributing
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted)
```

### Comparing `agixt-1.1.52b0/docs/README.md` & `agixt-1.1.54b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,65 @@
+Metadata-Version: 2.1
+Name: agixt
+Version: 1.1.54b0
+Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
+Author: Josh XT
+Author-email: josh@devxt.com
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # AGiXT
 ![RELEASE](https://img.shields.io/github/v/release/Josh-XT/AGiXT?label=Release%20Version&style=plastic) 
 [![STATUS](https://img.shields.io/badge/status-beta-blue?label=Release%20Status&style=plastic)](https://github.com/josh-xt/AGiXT) 
 [![LICENSE: MIT](https://img.shields.io/github/license/Josh-XT/AGiXT?label=License&style=plastic)](https://github.com/Josh-XT/AGiXT/blob/main/LICENSE) 
 ![DOCKER](https://img.shields.io/github/actions/workflow/status/Josh-XT/AGiXT/publish-docker.yml?branch=main&label=Docker&style=plastic) [![CODESTYLE](https://img.shields.io/badge/code%20style-Black-black?branch=main&label=Code%20Style&style=plastic)](https://black.readthedocs.io/en/stable/the_black_code_style/index.html)
 
 [![GitHub](https://img.shields.io/badge/GitHub-Frontend_Repository-grey?logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend)
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 [![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/Agent-LLM-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/labels/help%20wanted) 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT) 
 [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) 
 
-![Logo](AGiXT.svg)
+![Logo](images/AGiXT.svg)
 
 AGiXT is a dynamic Artificial Intelligence Automation Platform engineered to orchestrate efficient AI instruction management and task execution across a multitude of providers. Our solution infuses adaptive memory handling with a broad spectrum of commands to enhance AI's understanding and responsiveness, leading to improved task completion. The platform's smart features, like Smart Instruct and Smart Chat, seamlessly integrate web search, planning strategies, and conversation continuity, transforming the interaction between users and AI. By leveraging a powerful plugin system that includes web browsing and command execution, AGiXT stands as a versatile bridge between AI models and users. With an expanding roster of AI providers, code evaluation capabilities, comprehensive chain management, and platform interoperability, AGiXT is consistently evolving to drive a multitude of applications, affirming its place at the forefront of AI technology.
 
 Embracing the spirit of extremity in every facet of life, we introduce AGiXT. This advanced AI Automation Platform is our bold step towards the realization of Artificial General Intelligence (AGI). Seamlessly orchestrating instruction management and executing complex tasks across diverse AI providers, AGiXT combines adaptive memory, smart features, and a versatile plugin system to maximize AI potential. With our unwavering commitment to innovation, we're dedicated to pushing the boundaries of AI and bringing AGI closer to reality.
 
-## ⚠️ Monitor Your Usage!
-Please note that using some AI providers (such as OpenAI's GPT-4 API) can be expensive! Monitor your usage carefully to avoid incurring unexpected costs.  We're **NOT** responsible for your usage under any circumstance.
-
-## ⚠️ Under Development!
-This project is under active development and may still have issues. We appreciate your understanding and patience. If you encounter any problems, please first check the open issues. If your issue is not listed, kindly create a new issue detailing the error or problem you experienced. Thank you for your support!
-
 ## Table of Contents 📖
 
 - [AGiXT](#agixt)
-  - [⚠️ Monitor Your Usage!](#️-monitor-your-usage)
-  - [⚠️ Under Development!](#️-under-development)
   - [Table of Contents 📖](#table-of-contents-)
-  - [Media Coverage ⏯️](#media-coverage-️)
-    - [Video](#video)
+  - [⚠️ Disclaimers!](#️-disclaimers)
+    - [Monitor Your Usage!](#monitor-your-usage)
+    - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
-  - [Run with Docker](#run-with-docker)
-    - [Linux or Windows](#linux-or-windows)
+  - [Quickstart with Docker](#quickstart-with-docker)
     - [Windows Docker Desktop (streamlit only example)](#windows-docker-desktop-streamlit-only-example)
+    - [Alternative Docker Compose Profiles](#alternative-docker-compose-profiles)
     - [Development using docker](#development-using-docker)
   - [Local Development](#local-development)
+    - [API Endpoints](#api-endpoints)
   - [Configuration](#configuration)
-  - [API Endpoints](#api-endpoints)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
   - [Acknowledgments](#acknowledgments)
   - [History](#history)
 
-## Media Coverage ⏯️
-
-### Video
-- From [World of AI](https://www.youtube.com/@intheworldofai) on YouTube: [AGiXT: AI Automation Bot for Managing and Implementing AI Through Applications](https://www.youtube.com/watch?v=g0_36Mf2-To)
+## ⚠️ Disclaimers!
+### Monitor Your Usage!
+Please note that using some AI providers (such as OpenAI's GPT-4 API) can be expensive! Monitor your usage carefully to avoid incurring unexpected costs.  We're **NOT** responsible for your usage under any circumstance.
 
+### Under Development!
+This project is under active development and may still have issues. We appreciate your understanding and patience. If you encounter any problems, please first check the open issues. If your issue is not listed, kindly create a new issue detailing the error or problem you experienced. Thank you for your support!
 
 ## Key Features 🗝️
 
 - **Context and Token Management**: Adaptive handling of long-term and short-term memory for an optimized AI performance, allowing the software to process information more efficiently and accurately.
 - **Smart Instruct**: An advanced feature enabling AI to comprehend, plan, and execute tasks effectively. The system leverages web search, planning strategies, and executes instructions while ensuring output accuracy.
 - **Interactive Chat & Smart Chat**: User-friendly chat interface for dynamic conversational tasks. The Smart Chat feature integrates AI with web research to deliver accurate and contextually relevant responses.
 - **Task Execution & Smart Task Management**: Efficient management and execution of complex tasks broken down into sub-tasks. The Smart Task feature employs AI-driven agents to dynamically handle tasks, optimizing efficiency and avoiding redundancy.
@@ -66,72 +70,70 @@
 - **Docker Deployment**: Simplified setup and maintenance through Docker deployment.
 - **Audio-to-Text & Text-to-Speech Options**: Integration with Hugging Face for seamless audio-to-text transcription, and multiple TTS choices, featuring Brian TTS, Mac OS TTS, and ElevenLabs.
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
-## Run with Docker
-Clone the repositories for the AGiXT front/back ends then start the services with Docker.
-
-### Linux or Windows
+## Quickstart with Docker
+Download the `docker-compose` file and run the AGiXT Streamlit Web App.
 ```
-git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.yml
+docker compose --profile streamlit up
 ```
 
-Choose a service you want to run using profiles, e.g.
-`docker compose --profile streamlit up`
-
-Run all available services
-`docker compose --profile all up`
-
 - Web Interface http://localhost:8501
-
 ### Windows Docker Desktop (streamlit only example)
 - Container Name: AGiXT
 - Host Port: 8501:8501/tcp
 
+### Alternative Docker Compose Profiles
+
+Run all available services, this includes the FastAPI back end (Port 7437) and NextJS front end (Port 3000).
+```
+docker compose --profile all up
+```
+
 ### Development using docker
 ```
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.yml
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.dev.yml
 docker compose --profile all -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
 ## Local Development
 
 Clone the repository for the AGiXT back end and start it.
 
 ```
 git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT/src/agixt
+cd AGiXT/agixt
 pip install -r requirements.txt
 streamlit run streamlit.py
 ```
 
 Access the web interface at http://localhost:8501
 
-## Configuration
-
-Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
-
-## API Endpoints
+### API Endpoints
 
 AGiXT provides several API endpoints for managing agents, prompts and chains.
 
 If you're not running with Docker, the back end can be run with:
 ```
-python src/agixt/app.py
+python agixt/app.py
 ```
 
 To learn more about the API endpoints and their usage, visit the API documentation at 
 - [Swagger](http://localhost:7437)
 - [Redoc](http://localhost:7437/redoc)
 
 This documentation is hosted locally and the frontend must be running for these links to work.
+## Configuration
 
+Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
 ## Documentation
 
 Not enough information? Check out the [documentation](https://josh-xt.github.io/AGiXT) for more details.
 
 ## Contributing
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted)
```

### Comparing `agixt-1.1.52b0/setup.py` & `agixt-1.1.54b0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,31 +7,30 @@
 
 # Read the contents of the README file
 with open(readme_path, encoding="utf-8") as f:
     long_description = f.read()
 
 # Get requirements from requirements.txt to a list
 with open(
-    os.path.join(this_directory, "src/agixt/requirements.txt"), encoding="utf-8"
+    os.path.join(this_directory, "agixt/requirements.txt"), encoding="utf-8"
 ) as f:
     install_requires = f.read().splitlines()
 requirements = []
 for reqs in install_requires:
     if "--" not in reqs and ":" not in reqs and "#" not in reqs:
         requirements.append(reqs)
-# Get version from version file in src/agixt/version
-with open(os.path.join(this_directory, "src/agixt/version"), encoding="utf-8") as f:
+# Get version from version file in agixt/version
+with open(os.path.join(this_directory, "agixt/version"), encoding="utf-8") as f:
     version = f.read().strip()
 
 setup(
     name="agixt",
     version=version,
     description="An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.",
     long_description=long_description,
     long_description_content_type="text/markdown",  # This should match the format of your README
     author="Josh XT",
     author_email="josh@devxt.com",
-    package_dir={"": "src"},
-    packages=find_packages(where="src"),
+    packages=find_packages(),
     python_requires=">=3.10",
     install_requires=requirements,
 )
```

### Comparing `agixt-1.1.52b0/src/agixt/AGiXT.py` & `agixt-1.1.54b0/agixt/AGiXT.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/Chain.py` & `agixt-1.1.54b0/agixt/Chain.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/Commands.py` & `agixt-1.1.54b0/agixt/Commands.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/Config/Agent.py` & `agixt-1.1.54b0/agixt/Config/Agent.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/Config/__init__.py` & `agixt-1.1.54b0/agixt/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/CustomPrompt.py` & `agixt-1.1.54b0/agixt/CustomPrompt.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/Embedding.py` & `agixt-1.1.54b0/agixt/Embedding.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/Memories.py` & `agixt-1.1.54b0/agixt/Memories.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/Tasks.py` & `agixt-1.1.54b0/agixt/Tasks.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/app.py` & `agixt-1.1.54b0/agixt/app.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/__init__.py` & `agixt-1.1.54b0/agixt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/azure.py` & `agixt-1.1.54b0/agixt/provider/azure.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/bing.py` & `agixt-1.1.54b0/agixt/provider/bing.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/claude.py` & `agixt-1.1.54b0/agixt/provider/claude.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/fastchat.py` & `agixt-1.1.54b0/agixt/provider/fastchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/gpt4all.py` & `agixt-1.1.54b0/agixt/provider/gpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/gpt4free.py` & `agixt-1.1.54b0/agixt/provider/gpt4free.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/gpugpt4all.py` & `agixt-1.1.54b0/agixt/provider/gpugpt4all.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/huggingchat.py` & `agixt-1.1.54b0/agixt/provider/huggingchat.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/kobold.py` & `agixt-1.1.54b0/agixt/provider/kobold.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/llamacpp.py` & `agixt-1.1.54b0/agixt/provider/llamacpp.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/oobabooga.py` & `agixt-1.1.54b0/agixt/provider/oobabooga.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/openai.py` & `agixt-1.1.54b0/agixt/provider/openai.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/palm.py` & `agixt-1.1.54b0/agixt/provider/palm.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/provider/transformer.py` & `agixt-1.1.54b0/agixt/provider/transformer.py`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt/requirements.txt` & `agixt-1.1.54b0/agixt/requirements.txt`

 * *Files identical despite different names*

### Comparing `agixt-1.1.52b0/src/agixt.egg-info/PKG-INFO` & `agixt-1.1.54b0/agixt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agixt
-Version: 1.1.52b0
+Version: 1.1.54b0
 Summary: An Artificial Intelligence Automation Platform. AI Instruction management from various providers, has an adaptive memory, and a versatile plugin system with many commands including web browsing. Supports many AI providers and models and growing support every day.
 Author: Josh XT
 Author-email: josh@devxt.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,54 +18,48 @@
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute%20Backend&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted) 
 [![Contribute](https://img.shields.io/github/issues/JamesonRGrieve/Agent-LLM-Frontend/help%20wanted?color=purple&label=Quick%20Contribute%20Frontend&logo=github&style=plastic)](https://github.com/JamesonRGrieve/Agent-LLM-Frontend/labels/help%20wanted) 
 [![Discord](https://img.shields.io/discord/1097720481970397356?label=Discord&logo=discord&logoColor=white&style=plastic&color=5865f2)](https://discord.gg/d3TkHRZcjD) 
 [![Twitter](https://img.shields.io/badge/Twitter-Follow_@AGi_XT-blue?logo=twitter&style=plastic)](https://twitter.com/AGi_XT) 
 [![EMail](https://img.shields.io/badge/E--Mail-Outreach_&_Media-5865f2?logo=gmail&style=plastic)](https://twitter.com/AGi_XT) 
 
-![Logo](AGiXT.svg)
+![Logo](images/AGiXT.svg)
 
 AGiXT is a dynamic Artificial Intelligence Automation Platform engineered to orchestrate efficient AI instruction management and task execution across a multitude of providers. Our solution infuses adaptive memory handling with a broad spectrum of commands to enhance AI's understanding and responsiveness, leading to improved task completion. The platform's smart features, like Smart Instruct and Smart Chat, seamlessly integrate web search, planning strategies, and conversation continuity, transforming the interaction between users and AI. By leveraging a powerful plugin system that includes web browsing and command execution, AGiXT stands as a versatile bridge between AI models and users. With an expanding roster of AI providers, code evaluation capabilities, comprehensive chain management, and platform interoperability, AGiXT is consistently evolving to drive a multitude of applications, affirming its place at the forefront of AI technology.
 
 Embracing the spirit of extremity in every facet of life, we introduce AGiXT. This advanced AI Automation Platform is our bold step towards the realization of Artificial General Intelligence (AGI). Seamlessly orchestrating instruction management and executing complex tasks across diverse AI providers, AGiXT combines adaptive memory, smart features, and a versatile plugin system to maximize AI potential. With our unwavering commitment to innovation, we're dedicated to pushing the boundaries of AI and bringing AGI closer to reality.
 
-## ⚠️ Monitor Your Usage!
-Please note that using some AI providers (such as OpenAI's GPT-4 API) can be expensive! Monitor your usage carefully to avoid incurring unexpected costs.  We're **NOT** responsible for your usage under any circumstance.
-
-## ⚠️ Under Development!
-This project is under active development and may still have issues. We appreciate your understanding and patience. If you encounter any problems, please first check the open issues. If your issue is not listed, kindly create a new issue detailing the error or problem you experienced. Thank you for your support!
-
 ## Table of Contents 📖
 
 - [AGiXT](#agixt)
-  - [⚠️ Monitor Your Usage!](#️-monitor-your-usage)
-  - [⚠️ Under Development!](#️-under-development)
   - [Table of Contents 📖](#table-of-contents-)
-  - [Media Coverage ⏯️](#media-coverage-️)
-    - [Video](#video)
+  - [⚠️ Disclaimers!](#️-disclaimers)
+    - [Monitor Your Usage!](#monitor-your-usage)
+    - [Under Development!](#under-development)
   - [Key Features 🗝️](#key-features-️)
-  - [Run with Docker](#run-with-docker)
-    - [Linux or Windows](#linux-or-windows)
+  - [Quickstart with Docker](#quickstart-with-docker)
     - [Windows Docker Desktop (streamlit only example)](#windows-docker-desktop-streamlit-only-example)
+    - [Alternative Docker Compose Profiles](#alternative-docker-compose-profiles)
     - [Development using docker](#development-using-docker)
   - [Local Development](#local-development)
+    - [API Endpoints](#api-endpoints)
   - [Configuration](#configuration)
-  - [API Endpoints](#api-endpoints)
   - [Documentation](#documentation)
   - [Contributing](#contributing)
   - [Donations and Sponsorships](#donations-and-sponsorships)
   - [Our Team 🧑‍💻](#our-team-)
   - [Acknowledgments](#acknowledgments)
   - [History](#history)
 
-## Media Coverage ⏯️
-
-### Video
-- From [World of AI](https://www.youtube.com/@intheworldofai) on YouTube: [AGiXT: AI Automation Bot for Managing and Implementing AI Through Applications](https://www.youtube.com/watch?v=g0_36Mf2-To)
+## ⚠️ Disclaimers!
+### Monitor Your Usage!
+Please note that using some AI providers (such as OpenAI's GPT-4 API) can be expensive! Monitor your usage carefully to avoid incurring unexpected costs.  We're **NOT** responsible for your usage under any circumstance.
 
+### Under Development!
+This project is under active development and may still have issues. We appreciate your understanding and patience. If you encounter any problems, please first check the open issues. If your issue is not listed, kindly create a new issue detailing the error or problem you experienced. Thank you for your support!
 
 ## Key Features 🗝️
 
 - **Context and Token Management**: Adaptive handling of long-term and short-term memory for an optimized AI performance, allowing the software to process information more efficiently and accurately.
 - **Smart Instruct**: An advanced feature enabling AI to comprehend, plan, and execute tasks effectively. The system leverages web search, planning strategies, and executes instructions while ensuring output accuracy.
 - **Interactive Chat & Smart Chat**: User-friendly chat interface for dynamic conversational tasks. The Smart Chat feature integrates AI with web research to deliver accurate and contextually relevant responses.
 - **Task Execution & Smart Task Management**: Efficient management and execution of complex tasks broken down into sub-tasks. The Smart Task feature employs AI-driven agents to dynamically handle tasks, optimizing efficiency and avoiding redundancy.
@@ -76,72 +70,70 @@
 - **Docker Deployment**: Simplified setup and maintenance through Docker deployment.
 - **Audio-to-Text & Text-to-Speech Options**: Integration with Hugging Face for seamless audio-to-text transcription, and multiple TTS choices, featuring Brian TTS, Mac OS TTS, and ElevenLabs.
 - **Platform Interoperability & AI Agent Management**: Streamlined creation, renaming, deletion, and updating of AI agent settings along with easy interaction with popular platforms like Twitter, GitHub, Google, DALL-E, and more.
 - **Custom Prompts & Command Control**: Granular control over agent abilities through enabling or disabling specific commands, and easy creation, editing, and deletion of custom prompts to standardize user inputs.
 - **RESTful API**: FastAPI-powered RESTful API for seamless integration with external applications and services.
 - **Expanding AI Support**: Continually updated to include new AI providers and services, ensuring the software stays at the forefront of AI technology.
 
-## Run with Docker
-Clone the repositories for the AGiXT front/back ends then start the services with Docker.
-
-### Linux or Windows
+## Quickstart with Docker
+Download the `docker-compose` file and run the AGiXT Streamlit Web App.
 ```
-git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.yml
+docker compose --profile streamlit up
 ```
 
-Choose a service you want to run using profiles, e.g.
-`docker compose --profile streamlit up`
-
-Run all available services
-`docker compose --profile all up`
-
 - Web Interface http://localhost:8501
-
 ### Windows Docker Desktop (streamlit only example)
 - Container Name: AGiXT
 - Host Port: 8501:8501/tcp
 
+### Alternative Docker Compose Profiles
+
+Run all available services, this includes the FastAPI back end (Port 7437) and NextJS front end (Port 3000).
+```
+docker compose --profile all up
+```
+
 ### Development using docker
 ```
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.yml
+wget https://raw.githubusercontent.com/Josh-XT/AGiXT/main/docker/docker-compose.dev.yml
 docker compose --profile all -f docker-compose.yml -f docker-compose.dev.yaml up
 ```
 
 ## Local Development
 
 Clone the repository for the AGiXT back end and start it.
 
 ```
 git clone https://github.com/Josh-XT/AGiXT
-cd AGiXT/src/agixt
+cd AGiXT/agixt
 pip install -r requirements.txt
 streamlit run streamlit.py
 ```
 
 Access the web interface at http://localhost:8501
 
-## Configuration
-
-Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
-
-## API Endpoints
+### API Endpoints
 
 AGiXT provides several API endpoints for managing agents, prompts and chains.
 
 If you're not running with Docker, the back end can be run with:
 ```
-python src/agixt/app.py
+python agixt/app.py
 ```
 
 To learn more about the API endpoints and their usage, visit the API documentation at 
 - [Swagger](http://localhost:7437)
 - [Redoc](http://localhost:7437/redoc)
 
 This documentation is hosted locally and the frontend must be running for these links to work.
+## Configuration
 
+Each AGiXT Agent has its own settings for interfacing with AI providers, and other configuration options. These settings can be set and modified through the web interface.
 ## Documentation
 
 Not enough information? Check out the [documentation](https://josh-xt.github.io/AGiXT) for more details.
 
 ## Contributing
 
 [![Contribute](https://img.shields.io/github/issues/Josh-XT/AGiXT/help%20wanted?color=purple&label=Quick%20Contribute&logo=github&style=plastic)](https://github.com/Josh-XT/AGiXT/labels/help%20wanted)
```

### Comparing `agixt-1.1.52b0/src/agixt.egg-info/requires.txt` & `agixt-1.1.54b0/agixt.egg-info/requires.txt`

 * *Files identical despite different names*

