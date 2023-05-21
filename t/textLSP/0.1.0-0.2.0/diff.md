# Comparing `tmp/textLSP-0.1.0.tar.gz` & `tmp/textLSP-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/textLSP-0.1.0.tar", last modified: Sat Feb 18 17:08:42 2023, max compression
+gzip compressed data, was "textLSP-0.2.0.tar", last modified: Sun May 21 11:19:27 2023, max compression
```

## Comparing `textLSP-0.1.0.tar` & `textLSP-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,57 @@
-drwxr-xr-x   0 hangyav  (31247) student  (30500)        0 2023-02-18 17:08:42.893148 textLSP-0.1.0/
--rw-r--r--   0 hangyav  (31247) student  (30500)    35149 2022-11-18 08:38:39.000000 textLSP-0.1.0/LICENSE
--rw-r--r--   0 hangyav  (31247) student  (30500)     6663 2023-02-18 17:08:42.889148 textLSP-0.1.0/PKG-INFO
--rw-r--r--   0 hangyav  (31247) student  (30500)     4955 2023-02-18 17:00:56.000000 textLSP-0.1.0/README.md
--rw-r--r--   0 hangyav  (31247) student  (30500)       38 2023-02-18 17:08:42.893148 textLSP-0.1.0/setup.cfg
--rw-r--r--   0 hangyav  (31247) student  (30500)     1223 2023-02-18 16:58:13.000000 textLSP-0.1.0/setup.py
-drwxr-xr-x   0 hangyav  (31247) student  (30500)        0 2023-02-18 17:08:42.737147 textLSP-0.1.0/textLSP/
--rw-r--r--   0 hangyav  (31247) student  (30500)        0 2022-11-18 09:43:28.000000 textLSP-0.1.0/textLSP/__init__.py
-drwxr-xr-x   0 hangyav  (31247) student  (30500)        0 2023-02-18 17:08:42.793147 textLSP-0.1.0/textLSP/analysers/
--rw-r--r--   0 hangyav  (31247) student  (30500)        0 2022-12-23 11:17:05.000000 textLSP-0.1.0/textLSP/analysers/__init__.py
--rw-r--r--   0 hangyav  (31247) student  (30500)    14526 2023-02-12 06:59:30.000000 textLSP-0.1.0/textLSP/analysers/analyser.py
-drwxr-xr-x   0 hangyav  (31247) student  (30500)        0 2023-02-18 17:08:42.805148 textLSP-0.1.0/textLSP/analysers/gramformer/
--rw-r--r--   0 hangyav  (31247) student  (30500)       43 2023-01-22 17:02:17.000000 textLSP-0.1.0/textLSP/analysers/gramformer/__init__.py
--rw-r--r--   0 hangyav  (31247) student  (30500)     5601 2023-01-25 14:53:04.000000 textLSP-0.1.0/textLSP/analysers/gramformer/gramformer.py
-drwxr-xr-x   0 hangyav  (31247) student  (30500)        0 2023-02-18 17:08:42.821148 textLSP-0.1.0/textLSP/analysers/grammarbot/
--rw-r--r--   0 hangyav  (31247) student  (30500)       43 2023-01-03 16:51:19.000000 textLSP-0.1.0/textLSP/analysers/grammarbot/__init__.py
--rw-r--r--   0 hangyav  (31247) student  (30500)     6560 2023-02-12 10:51:47.000000 textLSP-0.1.0/textLSP/analysers/grammarbot/grammarbot.py
--rw-r--r--   0 hangyav  (31247) student  (30500)     7233 2023-02-12 08:58:52.000000 textLSP-0.1.0/textLSP/analysers/handler.py
-drwxr-xr-x   0 hangyav  (31247) student  (30500)        0 2023-02-18 17:08:42.833148 textLSP-0.1.0/textLSP/analysers/languagetool/
--rw-r--r--   0 hangyav  (31247) student  (30500)       47 2022-12-25 16:06:47.000000 textLSP-0.1.0/textLSP/analysers/languagetool/__init__.py
--rw-r--r--   0 hangyav  (31247) student  (30500)     6043 2023-01-25 14:25:02.000000 textLSP-0.1.0/textLSP/analysers/languagetool/languagetool.py
-drwxr-xr-x   0 hangyav  (31247) student  (30500)        0 2023-02-18 17:08:42.845148 textLSP-0.1.0/textLSP/analysers/openai/
--rw-r--r--   0 hangyav  (31247) student  (30500)       35 2023-01-28 08:41:24.000000 textLSP-0.1.0/textLSP/analysers/openai/__init__.py
--rw-r--r--   0 hangyav  (31247) student  (30500)     9899 2023-02-18 08:17:22.000000 textLSP-0.1.0/textLSP/analysers/openai/openai.py
--rw-r--r--   0 hangyav  (31247) student  (30500)      884 2022-12-24 10:42:20.000000 textLSP-0.1.0/textLSP/cli.py
-drwxr-xr-x   0 hangyav  (31247) student  (30500)        0 2023-02-18 17:08:42.853148 textLSP-0.1.0/textLSP/documents/
--rw-r--r--   0 hangyav  (31247) student  (30500)        0 2022-12-25 16:08:39.000000 textLSP-0.1.0/textLSP/documents/__init__.py
--rw-r--r--   0 hangyav  (31247) student  (30500)    19244 2023-02-18 08:18:09.000000 textLSP-0.1.0/textLSP/documents/document.py
-drwxr-xr-x   0 hangyav  (31247) student  (30500)        0 2023-02-18 17:08:42.865148 textLSP-0.1.0/textLSP/documents/latex/
--rw-r--r--   0 hangyav  (31247) student  (30500)       33 2022-12-26 08:08:08.000000 textLSP-0.1.0/textLSP/documents/latex/__init__.py
--rw-r--r--   0 hangyav  (31247) student  (30500)     5616 2023-02-16 13:41:11.000000 textLSP-0.1.0/textLSP/documents/latex/latex.py
-drwxr-xr-x   0 hangyav  (31247) student  (30500)        0 2023-02-18 17:08:42.873148 textLSP-0.1.0/textLSP/documents/org/
--rw-r--r--   0 hangyav  (31247) student  (30500)       29 2023-01-27 13:04:03.000000 textLSP-0.1.0/textLSP/documents/org/__init__.py
--rw-r--r--   0 hangyav  (31247) student  (30500)     5178 2023-01-28 07:23:36.000000 textLSP-0.1.0/textLSP/documents/org/org.py
-drwxr-xr-x   0 hangyav  (31247) student  (30500)        0 2023-02-18 17:08:42.885148 textLSP-0.1.0/textLSP/documents/txt/
--rw-r--r--   0 hangyav  (31247) student  (30500)       29 2022-12-26 08:08:39.000000 textLSP-0.1.0/textLSP/documents/txt/__init__.py
--rw-r--r--   0 hangyav  (31247) student  (30500)       80 2022-12-26 08:11:40.000000 textLSP-0.1.0/textLSP/documents/txt/txt.py
--rw-r--r--   0 hangyav  (31247) student  (30500)     6063 2023-02-12 06:52:05.000000 textLSP-0.1.0/textLSP/server.py
--rw-r--r--   0 hangyav  (31247) student  (30500)     7213 2023-01-28 11:19:01.000000 textLSP-0.1.0/textLSP/types.py
--rw-r--r--   0 hangyav  (31247) student  (30500)     2473 2023-02-12 08:51:53.000000 textLSP-0.1.0/textLSP/utils.py
--rw-r--r--   0 hangyav  (31247) student  (30500)     2081 2023-01-27 14:27:34.000000 textLSP-0.1.0/textLSP/workspace.py
-drwxr-xr-x   0 hangyav  (31247) student  (30500)        0 2023-02-18 17:08:42.777147 textLSP-0.1.0/textLSP.egg-info/
--rw-r--r--   0 hangyav  (31247) student  (30500)     6663 2023-02-18 17:08:42.000000 textLSP-0.1.0/textLSP.egg-info/PKG-INFO
--rw-r--r--   0 hangyav  (31247) student  (30500)      996 2023-02-18 17:08:42.000000 textLSP-0.1.0/textLSP.egg-info/SOURCES.txt
--rw-r--r--   0 hangyav  (31247) student  (30500)        1 2023-02-18 17:08:42.000000 textLSP-0.1.0/textLSP.egg-info/dependency_links.txt
--rw-r--r--   0 hangyav  (31247) student  (30500)       46 2023-02-18 17:08:42.000000 textLSP-0.1.0/textLSP.egg-info/entry_points.txt
--rw-r--r--   0 hangyav  (31247) student  (30500)      160 2023-02-18 17:08:42.000000 textLSP-0.1.0/textLSP.egg-info/requires.txt
--rw-r--r--   0 hangyav  (31247) student  (30500)        8 2023-02-18 17:08:42.000000 textLSP-0.1.0/textLSP.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.020941 textLSP-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 11:19:23.000000 textLSP-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-21 11:19:27.020941 textLSP-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-21 11:19:23.000000 textLSP-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 11:19:27.020941 textLSP-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-21 11:19:23.000000 textLSP-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.012941 textLSP-0.2.0/textLSP/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.012941 textLSP-0.2.0/textLSP/analysers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/analyser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.012941 textLSP-0.2.0/textLSP/analysers/gramformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/gramformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/gramformer/gramformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.016941 textLSP-0.2.0/textLSP/analysers/grammarbot/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/grammarbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/grammarbot/grammarbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.016941 textLSP-0.2.0/textLSP/analysers/hf_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/hf_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/hf_checker/hf_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.016941 textLSP-0.2.0/textLSP/analysers/hf_completion/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/hf_completion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/hf_completion/hf_completion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.016941 textLSP-0.2.0/textLSP/analysers/languagetool/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/languagetool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/languagetool/languagetool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.016941 textLSP-0.2.0/textLSP/analysers/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/analysers/openai/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.016941 textLSP-0.2.0/textLSP/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20065 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/documents/document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.016941 textLSP-0.2.0/textLSP/documents/latex/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/documents/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/documents/latex/latex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.016941 textLSP-0.2.0/textLSP/documents/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/documents/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/documents/markdown/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.020941 textLSP-0.2.0/textLSP/documents/org/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/documents/org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/documents/org/org.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.020941 textLSP-0.2.0/textLSP/documents/txt/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/documents/txt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/documents/txt/txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-21 11:19:23.000000 textLSP-0.2.0/textLSP/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:19:27.012941 textLSP-0.2.0/textLSP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-21 11:19:26.000000 textLSP-0.2.0/textLSP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-21 11:19:27.000000 textLSP-0.2.0/textLSP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 11:19:26.000000 textLSP-0.2.0/textLSP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-21 11:19:26.000000 textLSP-0.2.0/textLSP.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-21 11:19:26.000000 textLSP-0.2.0/textLSP.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 11:19:26.000000 textLSP-0.2.0/textLSP.egg-info/top_level.txt
```

### Comparing `textLSP-0.1.0/LICENSE` & `textLSP-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textLSP-0.1.0/PKG-INFO` & `textLSP-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,165 +1,196 @@
 Metadata-Version: 2.1
 Name: textLSP
-Version: 0.1.0
+Version: 0.2.0
 Summary: Language server for text spell and grammar check with various tools.
 Home-page: https://github.com/hangyav/textLSP
 Author: Viktor Hangya
 Author-email: hangyav@gmail.com
 License: GPLv3
-Description: # textLSP
-        Language server for text spell and grammar check with various AI tools.
-        
-        _This tool is in early development._
-        
-        ![textLSP](https://user-images.githubusercontent.com/414596/219856412-8095caa5-9ce6-49fe-9713-78d234837ac4.png)
-        
-        # Features
-        
-        ## LSP features
-        
-        * Diagnostics: spelling or grammatical errors
-        * Code actions:
-            * Fix suggestions
-            * Analyze paragraph with a selected passive analyzer (if the analyzer does not check on save or change)
-                <details><summary>Showcase</summary>
-                   <img src="https://user-images.githubusercontent.com/414596/219856438-0810eb43-929c-4bc3-811e-2ab53a5b2ae3.gif" height=80% width=80%/>
-                </details>
-            * Only on the first character of the first line: analyze the whole document if it was not fully checked yet
-                <details><summary>Showcase</summary>
-                   <img src="https://user-images.githubusercontent.com/414596/219856461-406c1e8f-ef71-4b6d-9270-6955320bd6aa.gif" height=80% width=80%/>
-                </details>
-        
-            * Custom actions defined by a given analyzer (e.g. prompt OpenAI)
-        
-        ## Analyzers
-        
-        ### Local tools
-        
-        The following tools run on the local system:
-        
-        * [LanguageTool](https://languagetool.org): Mainly for development purposes, see [ltex-ls](https://github.com/valentjn/ltex-ls) for a more mature implementation.
-        * [Gramformer](https://github.com/PrithivirajDamodaran/Gramformer): Neural network based system.
-            * Gramformer needs to be installed manually:
-              
-              ```pip install git+https://github.com/PrithivirajDamodaran/Gramformer.git```
-        
-        ### Tools using remote services
-        
-        **DISCLAIMER: THE RELATED APIS REQUIRE REGISTRATION AND ARE NOT FREE TO USE! USE THESE ANALYZERS ON YOUR OWN RESPONSIBILITY! THE AUTHORS OF TEXTLSP DO NOT ASSUME ANY RESPONSIBILITY FOR THE COSTS INCURRED!**
-        
-        The following tools use remote text APIs.
-        Due to potential costs turning off automatic analysis if suggested.
-        
-        * [OpenAI](https://openai.com/api): Supports text correction as well as text generation through a magic command in the text file.
-            <details><summary>Generation showcase</summary>
-                <img src="https://user-images.githubusercontent.com/414596/219856479-b85b5c2d-6158-44be-9063-12254b76e39c.gif" height=80% width=80%/>
-            </details>
-        * [GrammarBot](https://rapidapi.com/grammarbot/api/grammarbot): The GrammarBot API provides spelling and grammar checking.
-        
-        ## Supported File Types
-        
-        * latex
-        * org
-        * any other file types as plain text
-        
-        # Setup
-        
-        ## Install
-        ```
-        pip install textLSP
-        ```
-        
-        For the latest version:
-        ```
-        pip install git+https://github.com/hangyav/textLSP
-        ```
-        
-        ## Running
-        Simply run:
-        ```
-        textlsp
-        ```
-        
-        Since some analyzers are computation intensive, consider running it on a server using the TCP interface:
-        ```
-        textlsp --address 0.0.0.0 --port 1234
-        ```
-        or simply over ssh (with ssh key) if the client doesn't support it:
-        ```
-        ssh <server> textlsp
-        ```
-        
-        ## Configuration
-        
-        Using textLSP within an editor depends on the editor of choice.
-        For a few examples how to setup language servers in general in some of the popular editors see [here](https://github.com/openlawlibrary/pygls/tree/master/examples/hello-world#editor-configurations) or take a look at the related documentation of your editor.
-        
-        By default all analyzers are disabled in textLSP, they have to be turned on in the settings.
-        Example configuration in lua for nvim (other editors should be set up accordingly):
-        
-        ```lua
-        textLSP = {
-            analysers = {
-                languagetool = {
-                    enabled = true,
-                    check_text = {
-                        on_open = true,
-                        on_save = true,
-                        on_change = false,
-                    }
-                },
-                gramformer = {
-                    -- gramformer dependency needs to be installed manually
-                    enabled = true,
-                    gpu = false,
-                    check_text = {
-                        on_open = false,
-                        on_save = true,
-                        on_change = false,
-                    }
-                },
-                openai = {
-                    enabled = true,
-                    api_key = '<MY_API_KEY>',
-                    check_text = {
-                        on_open = false,
-                        on_save = false,
-                        on_change = false,
-                    },
-                    -- model = 'text-ada-001',
-                    model = 'text-babbage-001',
-                    -- model = 'text-curie-001',
-                    -- model = 'text-davinci-003',
-                    edit_model = 'text-davinci-edit-001',
-                    max_token = 16,
-                },
-                grammarbot = {
-                    enabled = false,
-                    api_key = '<MY_API_KEY>',
-                    -- longer texts are split, this parameter sets the maximum number of splits per analysis
-                    input_max_requests = 1,
-                    check_text = {
-                        on_open = false,
-                        on_save = false,
-                        on_change = false,
-                    }
-                },
-            },
-            documents = {
-                org = {
-                    org_todo_keywords = {
-                        'TODO',
-                        'IN_PROGRESS',
-                        'DONE'
-                    },
-                },
-            },
-        }
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# textLSP
+Language server for text spell and grammar check with various AI tools.
+
+_This tool is in early development._
+
+![textLSP](https://user-images.githubusercontent.com/414596/219856412-8095caa5-9ce6-49fe-9713-78d234837ac4.png)
+
+# Features
+
+## LSP features
+
+* Diagnostics:
+    * spelling or grammatical errors
+* Code actions:
+    * Fix suggestions
+    * Analyze paragraph with a selected passive analyzer (if the analyzer does not check on save or change)
+        <details><summary>Showcase</summary>
+           <img src="https://user-images.githubusercontent.com/414596/219856438-0810eb43-929c-4bc3-811e-2ab53a5b2ae3.gif" height=80% width=80%/>
+        </details>
+    * Only on the first character of the first line: analyze the whole document if it was not fully checked yet
+        <details><summary>Showcase</summary>
+           <img src="https://user-images.githubusercontent.com/414596/219856461-406c1e8f-ef71-4b6d-9270-6955320bd6aa.gif" height=80% width=80%/>
+        </details>
+    * Custom actions defined by a given analyzer
+      <details><summary>E.g. OpenAI text generation</summary>
+        <img src="https://user-images.githubusercontent.com/414596/219856479-b85b5c2d-6158-44be-9063-12254b76e39c.gif" height=80% width=80%/>
+      </details>
+* Context based word suggestion
+   <details><summary>Showcase</summary>
+      <img src="https://user-images.githubusercontent.com/414596/225412142-0cd83321-4a8e-47cf-8b5a-2cec4193800d.gif" height=80% width=80%/>
+   </details>
+
+## Analyzers
+
+### Local tools
+
+The following tools run on the local system:
+
+* [LanguageTool](https://languagetool.org): Mainly for development purposes, see [ltex-ls](https://github.com/valentjn/ltex-ls) for a more mature implementation.
+* [Gramformer](https://github.com/PrithivirajDamodaran/Gramformer): Neural network based system.
+    * Gramformer needs to be installed manually:
+
+      ```pip install git+https://github.com/PrithivirajDamodaran/Gramformer.git```
+* hf_checker: Huggingface `text2text-generation` pipline based analyser. See the [flan-t5-large-grammar-synthesis](https://huggingface.co/pszemraj/flan-t5-large-grammar-synthesis) model for an example.
+* [hf_completion](https://huggingface.co/docs/transformers/task_summary#language-modeling): Huggingface `fill-mask` pipline based text completion.
+
+### Tools using remote services
+
+**DISCLAIMER: THE RELATED APIS REQUIRE REGISTRATION AND ARE NOT FREE TO USE! USE THESE ANALYZERS ON YOUR OWN RESPONSIBILITY! THE AUTHORS OF TEXTLSP DO NOT ASSUME ANY RESPONSIBILITY FOR THE COSTS INCURRED!**
+
+The following tools use remote text APIs.
+Due to potential costs turning off automatic analysis if suggested.
+
+* [OpenAI](https://openai.com/api): Supports text correction as well as text generation through a magic command in the text file.
+    <details><summary>Generation showcase</summary>
+        <img src="https://user-images.githubusercontent.com/414596/219856479-b85b5c2d-6158-44be-9063-12254b76e39c.gif" height=80% width=80%/>
+    </details>
+* [GrammarBot](https://rapidapi.com/grammarbot/api/grammarbot): The GrammarBot API provides spelling and grammar checking.
+
+## Supported File Types
+
+* latex
+* org
+* markdown
+* any other file types as plain text
+
+# Setup
+
+## Install
+```
+pip install textLSP
+```
+
+For the latest version:
+```
+pip install git+https://github.com/hangyav/textLSP
+```
+
+## Running
+Simply run:
+```
+textlsp
+```
+
+Since some analyzers are computation intensive, consider running it on a server using the TCP interface:
+```
+textlsp --address 0.0.0.0 --port 1234
+```
+or simply over ssh (with ssh key) if the client doesn't support it:
+```
+ssh <server> textlsp
+```
+
+## Configuration
+
+Using textLSP within an editor depends on the editor of choice.
+For a few examples how to setup language servers in general in some of the popular editors see [here](https://github.com/openlawlibrary/pygls/tree/master/examples/hello-world#editor-configurations) or take a look at the related documentation of your editor.
+
+By default all analyzers are disabled in textLSP, they have to be turned on in the settings.
+Example configuration in lua for nvim (other editors should be set up accordingly):
+
+```lua
+textLSP = {
+    analysers = {
+        languagetool = {
+            enabled = true,
+            check_text = {
+                on_open = true,
+                on_save = true,
+                on_change = false,
+            }
+        },
+        gramformer = {
+            -- gramformer dependency needs to be installed manually
+            enabled = false,
+            gpu = false,
+            check_text = {
+                on_open = false,
+                on_save = true,
+                on_change = false,
+            }
+        },
+        hf_checker = {
+            enabled = true,
+            gpu = false,
+            model='pszemraj/flan-t5-large-grammar-synthesis',
+            -- model='pszemraj/grammar-synthesis-large',
+            min_length=40,
+            check_text = {
+                on_open = false,
+                on_save = true,
+                on_change = false,
+            }
+        },
+        hf_completion = {
+            enabled = true,
+            gpu = false,
+            model='bert-base-multilingual-cased',
+            topk=5,
+        },
+        openai = {
+            enabled = false,
+            api_key = '<MY_API_KEY>',
+            check_text = {
+                on_open = false,
+                on_save = false,
+                on_change = false,
+            },
+            -- model = 'text-ada-001',
+            model = 'text-babbage-001',
+            -- model = 'text-curie-001',
+            -- model = 'text-davinci-003',
+            edit_model = 'text-davinci-edit-001',
+            max_token = 16,
+        },
+        grammarbot = {
+            enabled = false,
+            api_key = '<MY_API_KEY>',
+            -- longer texts are split, this parameter sets the maximum number of splits per analysis
+            input_max_requests = 1,
+            check_text = {
+                on_open = false,
+                on_save = false,
+                on_change = false,
+            }
+        },
+    },
+    documents = {
+        org = {
+            org_todo_keywords = {
+                'TODO',
+                'IN_PROGRESS',
+                'DONE'
+            },
+        },
+        txt = {
+            parse = true,
+        },
+    },
+}
+```
```

### Comparing `textLSP-0.1.0/README.md` & `textLSP-0.2.0/textLSP.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,67 @@
+Metadata-Version: 2.1
+Name: textLSP
+Version: 0.2.0
+Summary: Language server for text spell and grammar check with various tools.
+Home-page: https://github.com/hangyav/textLSP
+Author: Viktor Hangya
+Author-email: hangyav@gmail.com
+License: GPLv3
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # textLSP
 Language server for text spell and grammar check with various AI tools.
 
 _This tool is in early development._
 
 ![textLSP](https://user-images.githubusercontent.com/414596/219856412-8095caa5-9ce6-49fe-9713-78d234837ac4.png)
 
 # Features
 
 ## LSP features
 
-* Diagnostics: spelling or grammatical errors
+* Diagnostics:
+    * spelling or grammatical errors
 * Code actions:
     * Fix suggestions
     * Analyze paragraph with a selected passive analyzer (if the analyzer does not check on save or change)
         <details><summary>Showcase</summary>
            <img src="https://user-images.githubusercontent.com/414596/219856438-0810eb43-929c-4bc3-811e-2ab53a5b2ae3.gif" height=80% width=80%/>
         </details>
     * Only on the first character of the first line: analyze the whole document if it was not fully checked yet
         <details><summary>Showcase</summary>
            <img src="https://user-images.githubusercontent.com/414596/219856461-406c1e8f-ef71-4b6d-9270-6955320bd6aa.gif" height=80% width=80%/>
         </details>
-
-    * Custom actions defined by a given analyzer (e.g. prompt OpenAI)
+    * Custom actions defined by a given analyzer
+      <details><summary>E.g. OpenAI text generation</summary>
+        <img src="https://user-images.githubusercontent.com/414596/219856479-b85b5c2d-6158-44be-9063-12254b76e39c.gif" height=80% width=80%/>
+      </details>
+* Context based word suggestion
+   <details><summary>Showcase</summary>
+      <img src="https://user-images.githubusercontent.com/414596/225412142-0cd83321-4a8e-47cf-8b5a-2cec4193800d.gif" height=80% width=80%/>
+   </details>
 
 ## Analyzers
 
 ### Local tools
 
 The following tools run on the local system:
 
 * [LanguageTool](https://languagetool.org): Mainly for development purposes, see [ltex-ls](https://github.com/valentjn/ltex-ls) for a more mature implementation.
 * [Gramformer](https://github.com/PrithivirajDamodaran/Gramformer): Neural network based system.
     * Gramformer needs to be installed manually:
-      
+
       ```pip install git+https://github.com/PrithivirajDamodaran/Gramformer.git```
+* hf_checker: Huggingface `text2text-generation` pipline based analyser. See the [flan-t5-large-grammar-synthesis](https://huggingface.co/pszemraj/flan-t5-large-grammar-synthesis) model for an example.
+* [hf_completion](https://huggingface.co/docs/transformers/task_summary#language-modeling): Huggingface `fill-mask` pipline based text completion.
 
 ### Tools using remote services
 
 **DISCLAIMER: THE RELATED APIS REQUIRE REGISTRATION AND ARE NOT FREE TO USE! USE THESE ANALYZERS ON YOUR OWN RESPONSIBILITY! THE AUTHORS OF TEXTLSP DO NOT ASSUME ANY RESPONSIBILITY FOR THE COSTS INCURRED!**
 
 The following tools use remote text APIs.
 Due to potential costs turning off automatic analysis if suggested.
@@ -48,14 +72,15 @@
     </details>
 * [GrammarBot](https://rapidapi.com/grammarbot/api/grammarbot): The GrammarBot API provides spelling and grammar checking.
 
 ## Supported File Types
 
 * latex
 * org
+* markdown
 * any other file types as plain text
 
 # Setup
 
 ## Install
 ```
 pip install textLSP
@@ -98,24 +123,42 @@
                 on_open = true,
                 on_save = true,
                 on_change = false,
             }
         },
         gramformer = {
             -- gramformer dependency needs to be installed manually
+            enabled = false,
+            gpu = false,
+            check_text = {
+                on_open = false,
+                on_save = true,
+                on_change = false,
+            }
+        },
+        hf_checker = {
             enabled = true,
             gpu = false,
+            model='pszemraj/flan-t5-large-grammar-synthesis',
+            -- model='pszemraj/grammar-synthesis-large',
+            min_length=40,
             check_text = {
                 on_open = false,
                 on_save = true,
                 on_change = false,
             }
         },
-        openai = {
+        hf_completion = {
             enabled = true,
+            gpu = false,
+            model='bert-base-multilingual-cased',
+            topk=5,
+        },
+        openai = {
+            enabled = false,
             api_key = '<MY_API_KEY>',
             check_text = {
                 on_open = false,
                 on_save = false,
                 on_change = false,
             },
             -- model = 'text-ada-001',
@@ -141,10 +184,13 @@
         org = {
             org_todo_keywords = {
                 'TODO',
                 'IN_PROGRESS',
                 'DONE'
             },
         },
+        txt = {
+            parse = true,
+        },
     },
 }
 ```
```

### Comparing `textLSP-0.1.0/setup.py` & `textLSP-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Utility function to read the README file.
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="textLSP",
-    version="0.1.0",
+    version="0.2.0",
     author="Viktor Hangya",
     author_email="hangyav@gmail.com",
     description=("Language server for text spell and grammar check with various tools."),
     license="GPLv3",
     url="https://github.com/hangyav/textLSP",
     packages=find_packages(include=['textLSP*']),
     long_description=read('README.md'),
@@ -30,15 +30,16 @@
         'pygls>=1.0.0',
         'lsprotocol>=2022.0.0a9',
         'language-tool-python>=2.7.1',
         'tree_sitter>=0.20.1',
         'gitpython>=3.1.29',
         'appdirs>=1.4.4',
         'torch>=1.13.1',
-        'openai>=0.26.4'
+        'openai>=0.26.4',
+        'transformers>=4.25.1',
     ],
     extras_require={
         'dev': [
             'pytest',
         ]
     },
 )
```

### Comparing `textLSP-0.1.0/textLSP/analysers/analyser.py` & `textLSP-0.2.0/textLSP/analysers/analyser.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         MessageType,
         CompletionParams,
         CompletionList,
 )
 
 from ..documents.document import BaseDocument, ChangeTracker
 from ..utils import merge_dicts
-from ..types import Interval, TextLSPCodeActionKind
+from ..types import Interval, TextLSPCodeActionKind, ProgressBar
 
 
 class Analyser():
     CONFIGURATION_SEVERITY = 'severity'
     CONFIGURATION_CHECK = 'check_text'
     CONFIGURATION_CHECK_ON_OPEN = 'on_open'
     CONFIGURATION_CHECK_ON_CHANGE = 'on_change'
@@ -50,25 +50,31 @@
         self.language_server = language_server
         self.config = dict()
         self.update_settings(config)
         self._diagnostics_dict = dict()
         self._code_actions_dict = dict()
         self._content_change_dict = dict()
         self._checked_documents = set()
+        self._progressbar_token = ProgressBar.create_token()
 
     def _did_open(self, doc: Document):
         raise NotImplementedError()
 
     def did_open(self, params: DidOpenTextDocumentParams):
         doc = self.get_document(params)
         self.init_document_items(doc)
         self._content_change_dict[doc.uri] = ChangeTracker(doc, True)
         if self.should_run_on(Analyser.CONFIGURATION_CHECK_ON_OPEN):
-            self._did_open(doc)
-            self._checked_documents.add(doc.uri)
+            with ProgressBar(
+                    self.language_server,
+                    f'{self.name} checking',
+                    token=self._progressbar_token
+            ):
+                self._did_open(doc)
+                self._checked_documents.add(doc.uri)
 
     def _did_change(self, doc: Document, changes: List[Interval]):
         raise NotImplementedError()
 
     def _get_line_shifts(self, params: DidChangeTextDocumentParams) -> List:
         res = list()
         for change in params.content_changes:
@@ -172,15 +178,20 @@
         if self.should_run_on(Analyser.CONFIGURATION_CHECK_ON_CHANGE):
             if self._content_change_dict[doc.uri].full_document_change:
                 self.did_open(
                     DidOpenTextDocumentParams(params.text_document)
                 )
             else:
                 changes = self._content_change_dict[doc.uri].get_changes()
-                self._did_change(doc, changes)
+                with ProgressBar(
+                        self.language_server,
+                        f'{self.name} checking',
+                        token=self._progressbar_token
+                ):
+                    self._did_change(doc, changes)
                 self._content_change_dict[doc.uri] = ChangeTracker(doc, True)
         elif len(line_shifts) > 0:
             self.language_server.publish_stored_diagnostics(doc)
 
     def update_document(self, doc: Document, change: TextDocumentContentChangeEvent):
         self._content_change_dict[doc.uri].update_document(change)
 
@@ -191,15 +202,20 @@
             if len(self._content_change_dict[doc.uri]) > 0:
                 if self._content_change_dict[doc.uri].full_document_change:
                     self.did_open(
                         DidOpenTextDocumentParams(params.text_document)
                     )
                 else:
                     changes = self._content_change_dict[doc.uri].get_changes()
-                    self._did_change(doc, changes)
+                    with ProgressBar(
+                            self.language_server,
+                            f'{self.name} checking',
+                            token=self._progressbar_token
+                    ):
+                        self._did_change(doc, changes)
                     self._content_change_dict[doc.uri] = ChangeTracker(doc, True)
 
     def _did_close(self, doc: Document):
         pass
 
     def did_close(self, params: DidCloseTextDocumentParams):
         self._did_close(self.get_document(params))
@@ -281,15 +297,15 @@
                     action.edit.document_changes[0].edits[0].range.start <= range.start
                     and action.edit.document_changes[0].edits[0].range.end >= range.end
                 )
                 # if it's not reachable by the cursor
                 or (
                     action.edit.document_changes[0].edits[0].range.start.line == range.start.line
                     and len(
-                        doc.lines[range.start.line]
+                        doc.lines[range.start.line].strip()
                     ) <= action.edit.document_changes[0].edits[0].range.start.character
                 )
             )
         ]
 
         if not (
             self.should_run_on(self.CONFIGURATION_CHECK_ON_CHANGE)
@@ -387,17 +403,27 @@
 
     def command_analyse(self, *args):
         args = args[0]
         doc = self.get_document(args['uri'])
         if 'interval' in args:
             interval = args['interval']
             interval = Interval(interval['start'], interval['length'])
-            self._command_analyse(doc, interval)
+            with ProgressBar(
+                    self.language_server,
+                    f'{self.name} checking',
+                    token=self._progressbar_token
+            ):
+                self._command_analyse(doc, interval)
         else:
-            self._command_analyse(doc)
+            with ProgressBar(
+                    self.language_server,
+                    f'{self.name} checking',
+                    token=self._progressbar_token
+            ):
+                self._command_analyse(doc)
             self._checked_documents.add(args['uri'])
 
     def get_completions(self, params: Optional[CompletionParams] = None) -> Optional[CompletionList]:
         return None
 
 
 class AnalysisError(Exception):
```

### Comparing `textLSP-0.1.0/textLSP/analysers/gramformer/gramformer.py` & `textLSP-0.2.0/textLSP/analysers/gramformer/gramformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,17 +94,24 @@
                 range = Range(
                     start=range.start,
                     end=Position(
                         line=range.end.line,
                         character=range.end.character+1,
                     )
                 )
+                if len(token) > 0 and len(edit[4]) > 0:
+                    message = f'"{token}": use "{edit[4]}" instead'
+                elif len(token) > 0:
+                    message = f'"{token}": remove'
+                else:
+                    message = f'insert "{edit[4]}"'
+
                 diagnostic = Diagnostic(
                     range=range,
-                    message=f'"{token}": Gramformer suggestion',
+                    message=message,
                     source='gramformer',
                     severity=self.get_severity(),
                     code=f'gramformer:{edit[0]}',
                 )
                 action = self.build_single_suggestion_action(
                     doc=doc,
                     title=f'"{token}" -> "{edit[4]}"',
```

### Comparing `textLSP-0.1.0/textLSP/analysers/grammarbot/grammarbot.py` & `textLSP-0.2.0/textLSP/analysers/grammarbot/grammarbot.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.1.0/textLSP/analysers/handler.py` & `textLSP-0.2.0/textLSP/analysers/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         CompletionList,
 )
 from pygls.workspace import Document
 
 from .. import analysers
 from .analyser import Analyser, AnalysisError
 from ..utils import get_class
-from ..types import ConfigurationError
+from ..types import ConfigurationError, ProgressBar
 
 
 logger = logging.getLogger(__name__)
 
 
 class AnalyserHandler():
 
@@ -43,23 +43,24 @@
                 continue
             if name in old_analysers:
                 analyser = old_analysers[name]
                 analyser.update_settings(config)
                 self.analysers[name] = analyser
             else:
                 try:
-                    cls = get_class(
-                        '{}.{}'.format(analysers.__name__, name),
-                        Analyser,
-                    )
-                    self.analysers[name] = cls(
-                        self.language_server,
-                        config,
-                        name
-                    )
+                    with ProgressBar(self.language_server, f'{name} init'):
+                        cls = get_class(
+                            '{}.{}'.format(analysers.__name__, name),
+                            Analyser,
+                        )
+                        self.analysers[name] = cls(
+                            self.language_server,
+                            config,
+                            name
+                        )
                 except ImportError as e:
                     self.language_server.show_message(
                         str(e),
                         MessageType.Error,
                     )
                 except ConfigurationError as e:
                     self.language_server.show_message(
```

### Comparing `textLSP-0.1.0/textLSP/analysers/languagetool/languagetool.py` & `textLSP-0.2.0/textLSP/analysers/languagetool/languagetool.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.1.0/textLSP/analysers/openai/openai.py` & `textLSP-0.2.0/textLSP/analysers/openai/openai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import openai
+from openai.error import OpenAIError
 
 from typing import List, Tuple, Optional
 from lsprotocol.types import (
         Diagnostic,
         Range,
         Position,
         TextEdit,
@@ -12,19 +13,20 @@
         Command,
         CodeActionParams,
         TextDocumentEdit,
         VersionedTextDocumentIdentifier,
         CompletionParams,
         CompletionList,
         CompletionItem,
+        MessageType,
 )
 from pygls.server import LanguageServer
 
 from ..analyser import Analyser
-from ...types import Interval, ConfigurationError, TokenDiff
+from ...types import Interval, ConfigurationError, TokenDiff, ProgressBar
 from ...documents.document import BaseDocument
 
 
 logger = logging.getLogger(__name__)
 
 
 class OpenAIAnalyser(Analyser):
@@ -51,34 +53,47 @@
     def __init__(self, language_server: LanguageServer, config: dict, name: str):
         super().__init__(language_server, config, name)
         if self.CONFIGURATION_API_KEY not in self.config:
             raise ConfigurationError(f'Reqired parameter: {name}.{self.CONFIGURATION_API_KEY}')
         openai.api_key = self.config[self.CONFIGURATION_API_KEY]
 
     def _edit(self, text) -> List[TokenDiff]:
-        res = openai.Edit.create(
-            model=self.config.get(self.CONFIGURATION_EDIT_MODEL, self.SETTINGS_DEFAULT_EDIT_MODEL),
-            instruction=self.config.get(self.CONFIGURATION_EDIT_INSTRUCTION, self.SETTINGS_DEFAULT_EDIT_INSTRUCTION),
-            input=text,
-            temperature=self.config.get(self.CONFIGURATION_TEMPERATURE, self.SETTINGS_DEFAULT_TEMPERATURE),
-        )
-        if len(res.choices) > 0:
-            return TokenDiff.token_level_diff(text, res.choices[0]['text'].strip())
+        try:
+            res = openai.Edit.create(
+                model=self.config.get(self.CONFIGURATION_EDIT_MODEL, self.SETTINGS_DEFAULT_EDIT_MODEL),
+                instruction=self.config.get(self.CONFIGURATION_EDIT_INSTRUCTION, self.SETTINGS_DEFAULT_EDIT_INSTRUCTION),
+                input=text,
+                temperature=self.config.get(self.CONFIGURATION_TEMPERATURE, self.SETTINGS_DEFAULT_TEMPERATURE),
+            )
+            if len(res.choices) > 0:
+                return TokenDiff.token_level_diff(text, res.choices[0]['text'].strip())
+        except OpenAIError as e:
+            self.language_server.show_message(
+                str(e),
+                MessageType.Error,
+            )
+
         return []
 
     def _generate(self, text) -> Optional[str]:
-        res = openai.Completion.create(
-            model=self.config.get(self.CONFIGURATION_MODEL, self.SETTINGS_DEFAULT_MODEL),
-            prompt=text,
-            temperature=self.config.get(self.CONFIGURATION_TEMPERATURE, self.SETTINGS_DEFAULT_TEMPERATURE),
-            max_tokens=self.config.get(self.CONFIGURATION_MAX_TOKEN, self.SETTINGS_DEFAULT_MAX_TOKEN),
-        )
+        try:
+            res = openai.Completion.create(
+                model=self.config.get(self.CONFIGURATION_MODEL, self.SETTINGS_DEFAULT_MODEL),
+                prompt=text,
+                temperature=self.config.get(self.CONFIGURATION_TEMPERATURE, self.SETTINGS_DEFAULT_TEMPERATURE),
+                max_tokens=self.config.get(self.CONFIGURATION_MAX_TOKEN, self.SETTINGS_DEFAULT_MAX_TOKEN),
+            )
 
-        if len(res.choices) > 0:
-            return res.choices[0]['text'].strip()
+            if len(res.choices) > 0:
+                return res.choices[0]['text'].strip()
+        except OpenAIError as e:
+            self.language_server.show_message(
+                str(e),
+                MessageType.Error,
+            )
 
         return None
 
     def _analyse(self, text, doc, offset=0) -> Tuple[List[Diagnostic], List[CodeAction]]:
         diagnostics = list()
         code_actions = list()
 
@@ -99,19 +114,27 @@
                 start=range.start,
                 end=Position(
                     line=range.end.line,
                     character=range.end.character+1,
                 )
             )
 
+            if edit.type == TokenDiff.INSERT:
+                message = f'insert "{edit.new_token}"'
+            elif edit.type == TokenDiff.REPLACE:
+                message = f'"{token}": use "{edit.new_token}" instead'
+            else:
+                message = f'"{token}": remove'
+
             diagnostic = Diagnostic(
                 range=range,
-                message=f'"{token}": openai {edit.type}',
+                message=message,
                 source='openai',
                 severity=self.get_severity(),
+                code=f'openai:{edit.type}',
             )
             action = self.build_single_suggestion_action(
                 doc=doc,
                 title=f'"{token}" -> "{edit.new_token}"',
                 edit=TextEdit(
                     range=diagnostic.range,
                     new_text=edit.new_token,
@@ -194,42 +217,50 @@
     def command_generate(
             self,
             uri: str,
             prompt: str,
             position: str,
             new_line=True
     ):
-        doc = self.get_document(uri)
+        with ProgressBar(
+                self.language_server,
+                f'{self.name} generating',
+                token=self._progressbar_token
+        ):
+            doc = self.get_document(uri)
+
+            new_text = self._generate(prompt)
+            if new_text is None:
+                return
 
-        new_text = self._generate(prompt)
-        new_text += '\n'
-        position = Position(**eval(position))
-        range = Range(
-            start=position,
-            end=position,
-        )
+            new_text += '\n'
+            position = Position(**eval(position))
+            range = Range(
+                start=position,
+                end=position,
+            )
 
-        edit = WorkspaceEdit(
-            document_changes=[
-                TextDocumentEdit(
-                    text_document=VersionedTextDocumentIdentifier(
-                        uri=doc.uri,
-                        version=doc.version,
-                    ),
-                    edits=[
-                        TextEdit(
-                            range=range,
-                            new_text=new_text,
+            edit = WorkspaceEdit(
+                document_changes=[
+                    TextDocumentEdit(
+                        text_document=VersionedTextDocumentIdentifier(
+                            uri=doc.uri,
+                            version=doc.version,
                         ),
-
-                    ]
-                )
-            ]
-        )
-        self.language_server.apply_edit(edit, 'textlsp.openai.generate')
+                        edits=[
+                            TextEdit(
+                                range=range,
+                                new_text=new_text,
+                            ),
+
+                        ]
+                    )
+                ]
+            )
+            self.language_server.apply_edit(edit, 'textlsp.openai.generate')
 
     def get_code_actions(self, params: CodeActionParams) -> Optional[List[CodeAction]]:
         doc = self.get_document(params)
         res = super().get_code_actions(params)
 
         if params.range.start != params.range.end:
             return res
@@ -271,15 +302,16 @@
         if params.position == Position(line=0, character=0):
             return None
 
         doc = self.get_document(params)
         line = doc.lines[params.position.line]
         magic = self.config.get(self.CONFIGURATION_PROMPT_MAGIC, self.SETTINGS_DEFAULT_PROMPT_MAGIC)
 
-        if len(line[:params.position.character].strip()) == 0:
+        line_prefix = line[:params.position.character].strip()
+        if len(line_prefix) == 0 or line_prefix in magic:
             return [
                 CompletionItem(
                     label=magic,
                     detail='OpenAI magic command for text generation based on'
                     ' the prompt that follows.'
                 )
             ]
```

### Comparing `textLSP-0.1.0/textLSP/cli.py` & `textLSP-0.2.0/textLSP/cli.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.1.0/textLSP/documents/document.py` & `textLSP-0.2.0/textLSP/documents/document.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 
 logger = logging.getLogger(__name__)
 
 
 class BaseDocument(Document):
     def __init__(self, *args, config: Dict = None, **kwargs):
         super().__init__(*args, **kwargs)
-        self.config = config
+        if config is None:
+            self.config = dict()
+        else:
+            self.config = config
 
     @property
     def cleaned_source(self) -> str:
         return self.source
 
     @property
     def cleaned_lines(self):
@@ -55,18 +58,24 @@
         assert offset == pos, 'Offset it over the document\'s end!'
         return Position(
             line=lidx,
             character=offset-pos
         )
 
     def range_at_offset(self, offset: int, length: int, cleaned=False) -> Range:
-        start = self.position_at_offset(offset)
+        start = self.position_at_offset(offset, cleaned)
         if start is None:
             return None
 
+        if length == 0:
+            return Range(
+                start=start,
+                end=start,
+            )
+
         length = start.character + length
         lines = self.cleaned_lines if cleaned else self.lines
         for lidx, line in enumerate(lines[start.line:], start.line):
             line_len = len(line)
             if line_len >= length:
                 return Range(
                     start=start,
@@ -232,14 +241,26 @@
     def _clean_source(self):
         raise NotImplementedError()
 
     def apply_change(self, change: TextDocumentContentChangeEvent) -> None:
         super().apply_change(change)
         self._cleaned_source = None
 
+    def position_at_offset(self, offset: int, cleaned=False) -> Position:
+        if not cleaned:
+            return super().position_at_offset(offset, cleaned)
+
+        raise NotImplementedError()
+
+    def range_at_offset(self, offset: int, length: int, cleaned=False) -> Range:
+        if not cleaned:
+            return super().range_at_offset(offset, length, cleaned)
+
+        raise NotImplementedError()
+
     def offset_at_position(self, position: Position, cleaned=False) -> int:
         if not cleaned:
             return super().offset_at_position(position, cleaned)
 
         raise NotImplementedError()
 
     def paragraphs_at_range(self, position_range: Range, cleaned=False) -> Interval:
@@ -304,55 +325,60 @@
 
 
 class TreeSitterDocument(CleanableDocument):
     LIB_PATH_TEMPLATE = '{}/treesitter/{}.so'.format(get_user_cache(), '{}')
 
     def __init__(self, language_name, grammar_url, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._language = TreeSitterDocument.get_language(language_name, grammar_url)
-        self._parser = TreeSitterDocument.get_parser(
+        self._language = self.get_language(language_name, grammar_url)
+        self._parser = self.get_parser(
             language_name,
             grammar_url,
             self._language
         )
         self._text_intervals = None
 
-    @staticmethod
-    def build_library(name, url) -> None:
+    @classmethod
+    def build_library(cls, name, url) -> None:
         with tempfile.TemporaryDirectory() as tmpdir:
             git_clone(url, tmpdir)
             Language.build_library(
-                TreeSitterDocument.LIB_PATH_TEMPLATE.format(name),
+                cls.LIB_PATH_TEMPLATE.format(name),
                 [tmpdir]
             )
 
-    @staticmethod
-    def get_language(name, url) -> Language:
+    @classmethod
+    def get_language(cls, name, url) -> Language:
         try:
             return Language(
-                TreeSitterDocument.LIB_PATH_TEMPLATE.format(name),
+                cls.LIB_PATH_TEMPLATE.format(name),
                 name,
             )
         except Exception:
-            TreeSitterDocument.build_library(name, url)
+            cls.build_library(name, url)
             return Language(
-                TreeSitterDocument.LIB_PATH_TEMPLATE.format(name),
+                cls.LIB_PATH_TEMPLATE.format(name),
                 name,
             )
 
-    @staticmethod
-    def get_parser(name, url, language=None) -> Parser:
+    @classmethod
+    def get_parser(cls, name=None, url=None, language=None) -> Parser:
         parser = Parser()
         if language is None:
-            language = TreeSitterDocument.get_language(name, url)
+            assert name is not None
+            assert url is not None
+            language = cls.get_language(name, url)
         parser.set_language(language)
         return parser
 
+    def _parse_source(self):
+        return self._parser.parse(bytes(self.source, 'utf-8'))
+
     def _clean_source(self):
-        tree = self._parser.parse(bytes(self.source, 'utf-8'))
+        tree = self._parse_source()
         self._text_intervals = OffsetPositionIntervalList()
 
         offset = 0
         for node in self._iterate_text_nodes(tree):
             node_len = len(node)
             self._text_intervals.add_interval_values(
                     offset,
@@ -387,14 +413,20 @@
         )
 
     def range_at_offset(self, offset: int, length: int, cleaned=False) -> Range:
         if not cleaned:
             return super().range_at_offset(offset, length, cleaned)
 
         start = self.position_at_offset(offset, cleaned)
+        if length == 0:
+            return Range(
+                start=start,
+                end=start,
+            )
+
         offset += length
         item = self._text_intervals.get_interval_at_offset(offset-1)
         item_end = item.offset_interval.start + item.offset_interval.length
         assert offset <= item_end, f'{offset}, {item_end}, {item}'
         diff = item_end - offset
 
         end = Position(
@@ -465,14 +497,15 @@
         return last.position_range.end
 
 
 class DocumentTypeFactory():
     TYPE_MAP = {
         'text': 'txt',
         'tex': 'latex',
+        'md': 'markdown',
     }
 
     @staticmethod
     def get_file_type(language_id):
         return DocumentTypeFactory.TYPE_MAP.get(language_id) or language_id
 
     @staticmethod
```

### Comparing `textLSP-0.1.0/textLSP/documents/latex/latex.py` & `textLSP-0.2.0/textLSP/documents/latex/latex.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.1.0/textLSP/documents/org/org.py` & `textLSP-0.2.0/textLSP/documents/org/org.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,17 +25,20 @@
     }
 
     TEXT_ROOTS_WITH_ITEM = {
         HEADLINE,
     }
 
     NEWLINE_AFTER_ONE = {
-        PARAGRAPH,
+        # SECTION,
+    }
+
+    NEWLINE_AFTER_TWO = {
         HEADLINE,
-        SECTION,
+        PARAGRAPH,
     }
 
     def __init__(self, *args, **kwargs):
         super().__init__(
             'org',
             'https://github.com/milisims/tree-sitter-org',
             *args,
@@ -57,14 +60,17 @@
 
         for root in self.TEXT_ROOTS_WITH_ITEM:
             query_str += f'({root} (item ({self.EXPR}) @{self.NODE_CONTENT}))\n'
 
         for root in self.NEWLINE_AFTER_ONE:
             query_str += f'({root}) @{self.NODE_NEWLINE_AFTER_ONE}\n'
 
+        for root in self.NEWLINE_AFTER_TWO:
+            query_str += f'({root}) @{self.NODE_NEWLINE_AFTER_TWO}\n'
+
         return self._language.query(query_str)
 
     def _iterate_text_nodes(self, tree: Tree) -> Generator[TextNode, None, None]:
         lines = tree.text.decode('utf-8').split('\n')
 
         last_sent = None
         new_lines_after = list()
@@ -79,22 +85,22 @@
                             yield nl
                     new_lines_after.pop(0)
                 else:
                     break
 
             if node[1] == self.NODE_CONTENT:
                 # check if we need newlines due to linebreaks in source
-                if (
-                    last_sent is not None
-                    and node[0].start_point[0] - last_sent.end_point[0] > 1
-                    and '' in lines[last_sent.end_point[0]+1:node[0].start_point[0]]
-                ):
-                    for nl_node in TextNode.get_new_lines(1, last_sent.end_point):
-                        yield nl_node
-                        last_sent = nl_node
+                # if (
+                #     last_sent is not None
+                #     and node[0].start_point[0] - last_sent.end_point[0] > 1
+                #     and '' in lines[last_sent.end_point[0]+1:node[0].start_point[0]]
+                # ):
+                #     for nl_node in TextNode.get_new_lines(1, last_sent.end_point):
+                #         yield nl_node
+                #         last_sent = nl_node
 
                 # handle spaces
                 if self._needs_space_before(node[0], lines, last_sent):
                     sp = node[0].start_point
                     if sp[1] > 0:
                         yield TextNode.space(
                             start_point=(sp[0], sp[1]-1),
@@ -113,14 +119,16 @@
                         )
 
                 if self._valid_content_node(node[0]):
                     last_sent = TextNode.from_ts_node(node[0])
                     yield last_sent
             elif node[1] == self.NODE_NEWLINE_AFTER_ONE:
                 self._insert_point_in_order(node[0].end_point, new_lines_after)
+            elif node[1] == self.NODE_NEWLINE_AFTER_TWO:
+                self._insert_point_in_order(node[0].end_point, new_lines_after, 2)
 
         yield from TextNode.get_new_lines(
             1,
             last_sent.end_point if last_sent else (0, 0)
         )
 
     def _valid_content_node(self, node: Node):
```

### Comparing `textLSP-0.1.0/textLSP/server.py` & `textLSP-0.2.0/textLSP/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     COMMAND_CUSTOM = 'custom_command'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.settings = dict()
         self.init_settings()
         self.analyser_handler = AnalyserHandler(self)
+        logger.warning('TextLSP initialized!')
 
     def init_settings(self):
         self.settings.setdefault(self.CONFIGURATION_SECTION, dict())
         self.settings[self.CONFIGURATION_SECTION].setdefault(self.CONFIGURATION_ANALYSERS, None)
         self.settings[self.CONFIGURATION_SECTION].setdefault(self.CONFIGURATION_DOCUMENTS, None)
 
     def get_analyser_settings(self, settings=None):
@@ -96,14 +97,15 @@
         ):
             return self.settings[self.CONFIGURATION_SECTION][self.CONFIGURATION_DOCUMENTS]
         return None
 
     def update_settings(self, settings):
         if settings is None or len(settings) == 0:
             return
+
         self.settings = merge_dicts(self.settings, settings)
         if self.get_analyser_settings(settings):
             # update only if there was any update related to it
             self.analyser_handler.update_settings(
                 self.get_analyser_settings()
             )
         if self.get_document_settings(settings):
```

### Comparing `textLSP-0.1.0/textLSP/types.py` & `textLSP-0.2.0/textLSP/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 import re
 import bisect
 import enum
 import difflib
+import uuid
 
 from typing import Optional, Any, List
 from dataclasses import dataclass
 
-from lsprotocol.types import Position, Range, CodeActionKind
+from lsprotocol.types import (
+    Position,
+    Range,
+    CodeActionKind,
+    WorkDoneProgressBegin,
+    WorkDoneProgressReport,
+    WorkDoneProgressEnd,
+)
 
 
 TEXT_PASSAGE_PATTERN = re.compile('[.?!] |\\n')
+LINE_PATTERN = re.compile('\\n')
 
 
 class ConfigurationError(Exception):
     pass
 
 
 @dataclass
@@ -185,15 +194,15 @@
         if idx == length:
             return None if strict else length-1
 
         if self._position_start_character[idx] <= position.character <= self._position_end_character[idx]:
             return idx
         if position.character < self._position_start_character[idx]:
             return None if strict else idx
-        # if position.character > self._position_end_character[idx]
+
         return None if strict else min(idx+1, length-1)
 
     def get_interval_at_position(self, position: Position, strict=True) -> OffsetPositionInterval:
         """
         :param strict: If Flase, return the object of the next (or last) interval if does not exist
         """
         idx = self.get_idx_at_position(position, strict)
@@ -233,7 +242,65 @@
                 new_token=' '.join(tokens2[item[3]:item[4]]),
                 offset=0 if item[1] == 0 else len(' '.join(tokens1[:item[1]]))+1,
                 length=len(' '.join(tokens1[item[1]:item[2]])),
             )
             for item in diff.get_opcodes()
             if item[0] != 'equal'
         ]
+
+    def __str__(self):
+        return (
+            f'{self.type}: {self.old_token} -> {self.new_token} '
+            f'({self.offset}, {self.length})'
+        )
+
+
+class ProgressBar():
+    def __init__(self, ls, title='', percentage=0, token=None):
+        self.ls = ls
+        self.title = title
+        self.percentage = percentage
+        self.token = token
+        if self.token is None:
+            self.token = self.create_token()
+
+    def begin(self, title=None, percentage=None):
+        if title is not None:
+            self.title = title
+        if percentage is not None:
+            self.percentage = percentage
+
+        if self.token not in self.ls.progress.tokens:
+            self.ls.progress.create(self.token)
+        self.ls.progress.begin(
+            self.token,
+            WorkDoneProgressBegin(
+                title=self.title,
+                percentage=self.percentage,
+            )
+        )
+
+    def update(self, message, percentage=0):
+        self.ls.progress.report(
+            self.token,
+            WorkDoneProgressReport(
+                message=message,
+                percentage=percentage
+            ),
+        )
+
+    def end(self, message):
+        self.ls.progress.end(
+            self.token,
+            WorkDoneProgressEnd(message=message)
+        )
+
+    def __enter__(self):
+        self.begin()
+        return self
+
+    def __exit__(self, type, value, traceback):
+        self.end('Done')
+
+    @staticmethod
+    def create_token():
+        return str(uuid.uuid4())
```

### Comparing `textLSP-0.1.0/textLSP/utils.py` & `textLSP-0.2.0/textLSP/utils.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.1.0/textLSP/workspace.py` & `textLSP-0.2.0/textLSP/workspace.py`

 * *Files identical despite different names*

### Comparing `textLSP-0.1.0/textLSP.egg-info/PKG-INFO` & `textLSP-0.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,165 +1,181 @@
-Metadata-Version: 2.1
-Name: textLSP
-Version: 0.1.0
-Summary: Language server for text spell and grammar check with various tools.
-Home-page: https://github.com/hangyav/textLSP
-Author: Viktor Hangya
-Author-email: hangyav@gmail.com
-License: GPLv3
-Description: # textLSP
-        Language server for text spell and grammar check with various AI tools.
-        
-        _This tool is in early development._
-        
-        ![textLSP](https://user-images.githubusercontent.com/414596/219856412-8095caa5-9ce6-49fe-9713-78d234837ac4.png)
-        
-        # Features
-        
-        ## LSP features
-        
-        * Diagnostics: spelling or grammatical errors
-        * Code actions:
-            * Fix suggestions
-            * Analyze paragraph with a selected passive analyzer (if the analyzer does not check on save or change)
-                <details><summary>Showcase</summary>
-                   <img src="https://user-images.githubusercontent.com/414596/219856438-0810eb43-929c-4bc3-811e-2ab53a5b2ae3.gif" height=80% width=80%/>
-                </details>
-            * Only on the first character of the first line: analyze the whole document if it was not fully checked yet
-                <details><summary>Showcase</summary>
-                   <img src="https://user-images.githubusercontent.com/414596/219856461-406c1e8f-ef71-4b6d-9270-6955320bd6aa.gif" height=80% width=80%/>
-                </details>
-        
-            * Custom actions defined by a given analyzer (e.g. prompt OpenAI)
-        
-        ## Analyzers
-        
-        ### Local tools
-        
-        The following tools run on the local system:
-        
-        * [LanguageTool](https://languagetool.org): Mainly for development purposes, see [ltex-ls](https://github.com/valentjn/ltex-ls) for a more mature implementation.
-        * [Gramformer](https://github.com/PrithivirajDamodaran/Gramformer): Neural network based system.
-            * Gramformer needs to be installed manually:
-              
-              ```pip install git+https://github.com/PrithivirajDamodaran/Gramformer.git```
-        
-        ### Tools using remote services
-        
-        **DISCLAIMER: THE RELATED APIS REQUIRE REGISTRATION AND ARE NOT FREE TO USE! USE THESE ANALYZERS ON YOUR OWN RESPONSIBILITY! THE AUTHORS OF TEXTLSP DO NOT ASSUME ANY RESPONSIBILITY FOR THE COSTS INCURRED!**
-        
-        The following tools use remote text APIs.
-        Due to potential costs turning off automatic analysis if suggested.
-        
-        * [OpenAI](https://openai.com/api): Supports text correction as well as text generation through a magic command in the text file.
-            <details><summary>Generation showcase</summary>
-                <img src="https://user-images.githubusercontent.com/414596/219856479-b85b5c2d-6158-44be-9063-12254b76e39c.gif" height=80% width=80%/>
-            </details>
-        * [GrammarBot](https://rapidapi.com/grammarbot/api/grammarbot): The GrammarBot API provides spelling and grammar checking.
-        
-        ## Supported File Types
-        
-        * latex
-        * org
-        * any other file types as plain text
-        
-        # Setup
-        
-        ## Install
-        ```
-        pip install textLSP
-        ```
-        
-        For the latest version:
-        ```
-        pip install git+https://github.com/hangyav/textLSP
-        ```
-        
-        ## Running
-        Simply run:
-        ```
-        textlsp
-        ```
-        
-        Since some analyzers are computation intensive, consider running it on a server using the TCP interface:
-        ```
-        textlsp --address 0.0.0.0 --port 1234
-        ```
-        or simply over ssh (with ssh key) if the client doesn't support it:
-        ```
-        ssh <server> textlsp
-        ```
-        
-        ## Configuration
-        
-        Using textLSP within an editor depends on the editor of choice.
-        For a few examples how to setup language servers in general in some of the popular editors see [here](https://github.com/openlawlibrary/pygls/tree/master/examples/hello-world#editor-configurations) or take a look at the related documentation of your editor.
-        
-        By default all analyzers are disabled in textLSP, they have to be turned on in the settings.
-        Example configuration in lua for nvim (other editors should be set up accordingly):
-        
-        ```lua
-        textLSP = {
-            analysers = {
-                languagetool = {
-                    enabled = true,
-                    check_text = {
-                        on_open = true,
-                        on_save = true,
-                        on_change = false,
-                    }
-                },
-                gramformer = {
-                    -- gramformer dependency needs to be installed manually
-                    enabled = true,
-                    gpu = false,
-                    check_text = {
-                        on_open = false,
-                        on_save = true,
-                        on_change = false,
-                    }
-                },
-                openai = {
-                    enabled = true,
-                    api_key = '<MY_API_KEY>',
-                    check_text = {
-                        on_open = false,
-                        on_save = false,
-                        on_change = false,
-                    },
-                    -- model = 'text-ada-001',
-                    model = 'text-babbage-001',
-                    -- model = 'text-curie-001',
-                    -- model = 'text-davinci-003',
-                    edit_model = 'text-davinci-edit-001',
-                    max_token = 16,
-                },
-                grammarbot = {
-                    enabled = false,
-                    api_key = '<MY_API_KEY>',
-                    -- longer texts are split, this parameter sets the maximum number of splits per analysis
-                    input_max_requests = 1,
-                    check_text = {
-                        on_open = false,
-                        on_save = false,
-                        on_change = false,
-                    }
-                },
+# textLSP
+Language server for text spell and grammar check with various AI tools.
+
+_This tool is in early development._
+
+![textLSP](https://user-images.githubusercontent.com/414596/219856412-8095caa5-9ce6-49fe-9713-78d234837ac4.png)
+
+# Features
+
+## LSP features
+
+* Diagnostics:
+    * spelling or grammatical errors
+* Code actions:
+    * Fix suggestions
+    * Analyze paragraph with a selected passive analyzer (if the analyzer does not check on save or change)
+        <details><summary>Showcase</summary>
+           <img src="https://user-images.githubusercontent.com/414596/219856438-0810eb43-929c-4bc3-811e-2ab53a5b2ae3.gif" height=80% width=80%/>
+        </details>
+    * Only on the first character of the first line: analyze the whole document if it was not fully checked yet
+        <details><summary>Showcase</summary>
+           <img src="https://user-images.githubusercontent.com/414596/219856461-406c1e8f-ef71-4b6d-9270-6955320bd6aa.gif" height=80% width=80%/>
+        </details>
+    * Custom actions defined by a given analyzer
+      <details><summary>E.g. OpenAI text generation</summary>
+        <img src="https://user-images.githubusercontent.com/414596/219856479-b85b5c2d-6158-44be-9063-12254b76e39c.gif" height=80% width=80%/>
+      </details>
+* Context based word suggestion
+   <details><summary>Showcase</summary>
+      <img src="https://user-images.githubusercontent.com/414596/225412142-0cd83321-4a8e-47cf-8b5a-2cec4193800d.gif" height=80% width=80%/>
+   </details>
+
+## Analyzers
+
+### Local tools
+
+The following tools run on the local system:
+
+* [LanguageTool](https://languagetool.org): Mainly for development purposes, see [ltex-ls](https://github.com/valentjn/ltex-ls) for a more mature implementation.
+* [Gramformer](https://github.com/PrithivirajDamodaran/Gramformer): Neural network based system.
+    * Gramformer needs to be installed manually:
+
+      ```pip install git+https://github.com/PrithivirajDamodaran/Gramformer.git```
+* hf_checker: Huggingface `text2text-generation` pipline based analyser. See the [flan-t5-large-grammar-synthesis](https://huggingface.co/pszemraj/flan-t5-large-grammar-synthesis) model for an example.
+* [hf_completion](https://huggingface.co/docs/transformers/task_summary#language-modeling): Huggingface `fill-mask` pipline based text completion.
+
+### Tools using remote services
+
+**DISCLAIMER: THE RELATED APIS REQUIRE REGISTRATION AND ARE NOT FREE TO USE! USE THESE ANALYZERS ON YOUR OWN RESPONSIBILITY! THE AUTHORS OF TEXTLSP DO NOT ASSUME ANY RESPONSIBILITY FOR THE COSTS INCURRED!**
+
+The following tools use remote text APIs.
+Due to potential costs turning off automatic analysis if suggested.
+
+* [OpenAI](https://openai.com/api): Supports text correction as well as text generation through a magic command in the text file.
+    <details><summary>Generation showcase</summary>
+        <img src="https://user-images.githubusercontent.com/414596/219856479-b85b5c2d-6158-44be-9063-12254b76e39c.gif" height=80% width=80%/>
+    </details>
+* [GrammarBot](https://rapidapi.com/grammarbot/api/grammarbot): The GrammarBot API provides spelling and grammar checking.
+
+## Supported File Types
+
+* latex
+* org
+* markdown
+* any other file types as plain text
+
+# Setup
+
+## Install
+```
+pip install textLSP
+```
+
+For the latest version:
+```
+pip install git+https://github.com/hangyav/textLSP
+```
+
+## Running
+Simply run:
+```
+textlsp
+```
+
+Since some analyzers are computation intensive, consider running it on a server using the TCP interface:
+```
+textlsp --address 0.0.0.0 --port 1234
+```
+or simply over ssh (with ssh key) if the client doesn't support it:
+```
+ssh <server> textlsp
+```
+
+## Configuration
+
+Using textLSP within an editor depends on the editor of choice.
+For a few examples how to setup language servers in general in some of the popular editors see [here](https://github.com/openlawlibrary/pygls/tree/master/examples/hello-world#editor-configurations) or take a look at the related documentation of your editor.
+
+By default all analyzers are disabled in textLSP, they have to be turned on in the settings.
+Example configuration in lua for nvim (other editors should be set up accordingly):
+
+```lua
+textLSP = {
+    analysers = {
+        languagetool = {
+            enabled = true,
+            check_text = {
+                on_open = true,
+                on_save = true,
+                on_change = false,
+            }
+        },
+        gramformer = {
+            -- gramformer dependency needs to be installed manually
+            enabled = false,
+            gpu = false,
+            check_text = {
+                on_open = false,
+                on_save = true,
+                on_change = false,
+            }
+        },
+        hf_checker = {
+            enabled = true,
+            gpu = false,
+            model='pszemraj/flan-t5-large-grammar-synthesis',
+            -- model='pszemraj/grammar-synthesis-large',
+            min_length=40,
+            check_text = {
+                on_open = false,
+                on_save = true,
+                on_change = false,
+            }
+        },
+        hf_completion = {
+            enabled = true,
+            gpu = false,
+            model='bert-base-multilingual-cased',
+            topk=5,
+        },
+        openai = {
+            enabled = false,
+            api_key = '<MY_API_KEY>',
+            check_text = {
+                on_open = false,
+                on_save = false,
+                on_change = false,
             },
-            documents = {
-                org = {
-                    org_todo_keywords = {
-                        'TODO',
-                        'IN_PROGRESS',
-                        'DONE'
-                    },
-                },
+            -- model = 'text-ada-001',
+            model = 'text-babbage-001',
+            -- model = 'text-curie-001',
+            -- model = 'text-davinci-003',
+            edit_model = 'text-davinci-edit-001',
+            max_token = 16,
+        },
+        grammarbot = {
+            enabled = false,
+            api_key = '<MY_API_KEY>',
+            -- longer texts are split, this parameter sets the maximum number of splits per analysis
+            input_max_requests = 1,
+            check_text = {
+                on_open = false,
+                on_save = false,
+                on_change = false,
+            }
+        },
+    },
+    documents = {
+        org = {
+            org_todo_keywords = {
+                'TODO',
+                'IN_PROGRESS',
+                'DONE'
             },
-        }
-        ```
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+        },
+        txt = {
+            parse = true,
+        },
+    },
+}
+```
```

### Comparing `textLSP-0.1.0/textLSP.egg-info/SOURCES.txt` & `textLSP-0.2.0/textLSP.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,19 +16,25 @@
 textLSP/analysers/__init__.py
 textLSP/analysers/analyser.py
 textLSP/analysers/handler.py
 textLSP/analysers/gramformer/__init__.py
 textLSP/analysers/gramformer/gramformer.py
 textLSP/analysers/grammarbot/__init__.py
 textLSP/analysers/grammarbot/grammarbot.py
+textLSP/analysers/hf_checker/__init__.py
+textLSP/analysers/hf_checker/hf_checker.py
+textLSP/analysers/hf_completion/__init__.py
+textLSP/analysers/hf_completion/hf_completion.py
 textLSP/analysers/languagetool/__init__.py
 textLSP/analysers/languagetool/languagetool.py
 textLSP/analysers/openai/__init__.py
 textLSP/analysers/openai/openai.py
 textLSP/documents/__init__.py
 textLSP/documents/document.py
 textLSP/documents/latex/__init__.py
 textLSP/documents/latex/latex.py
+textLSP/documents/markdown/__init__.py
+textLSP/documents/markdown/markdown.py
 textLSP/documents/org/__init__.py
 textLSP/documents/org/org.py
 textLSP/documents/txt/__init__.py
 textLSP/documents/txt/txt.py
```

