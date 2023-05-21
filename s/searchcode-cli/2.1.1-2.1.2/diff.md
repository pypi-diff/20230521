# Comparing `tmp/searchcode-cli-2.1.1.tar.gz` & `tmp/searchcode-cli-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchcode-cli-2.1.1.tar", last modified: Fri May 12 21:21:24 2023, max compression
+gzip compressed data, was "searchcode-cli-2.1.2.tar", last modified: Sun May 21 04:40:49 2023, max compression
```

## Comparing `searchcode-cli-2.1.1.tar` & `searchcode-cli-2.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42815 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/searchcode/
--rw-r--r--   0 runner    (1001) docker     (123)    19286 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/searchcode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/searchcode/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-05-12 21:21:11.000000 searchcode-cli-2.1.1/searchcode/miscellaneous.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/searchcode_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42815 2023-05-12 21:21:23.000000 searchcode-cli-2.1.1/searchcode_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-12 21:21:23.000000 searchcode-cli-2.1.1/searchcode_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:21:23.000000 searchcode-cli-2.1.1/searchcode_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-12 21:21:23.000000 searchcode-cli-2.1.1/searchcode_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 21:21:23.998345 searchcode-cli-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43192 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/searchcode/
+-rw-r--r--   0 runner    (1001) docker     (123)    26906 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/searchcode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/searchcode/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-05-21 04:40:38.000000 searchcode-cli-2.1.2/searchcode/miscellaneous.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/searchcode_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43192 2023-05-21 04:40:49.000000 searchcode-cli-2.1.2/searchcode_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-21 04:40:49.000000 searchcode-cli-2.1.2/searchcode_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 04:40:49.000000 searchcode-cli-2.1.2/searchcode_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 04:40:49.000000 searchcode-cli-2.1.2/searchcode_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 04:40:49.567396 searchcode-cli-2.1.2/setup.cfg
```

### Comparing `searchcode-cli-2.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `searchcode-cli-2.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `searchcode-cli-2.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.1/.github/workflows/codeql.yml` & `searchcode-cli-2.1.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.1/.github/workflows/python-publish.yml` & `searchcode-cli-2.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.1/.gitignore` & `searchcode-cli-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.1/LICENSE` & `searchcode-cli-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.1/PKG-INFO` & `searchcode-cli-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchcode-cli
-Version: 2.1.1
+Version: 2.1.2
 Summary: A Python wrapper around the searchcode API
 Author-email: Richard Mwewa <rly0nheart@duck.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,14 +695,18 @@
 
 ![searchcode-cli_banner](https://user-images.githubusercontent.com/74001397/203441377-ad53a2ab-16d6-42b3-bbec-542c9ed43534.png)
 
 
 A Python wrapper around the [SearchCode API](https://searchcode.com/api/)
 
 [![Upload Python Package](https://github.com/rly0nheart/searchcode-cli/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rly0nheart/searchcode-cli/actions/workflows/python-publish.yml) [![CodeQL](https://github.com/rly0nheart/searchcode-cli/actions/workflows/codeql.yml/badge.svg)](https://github.com/rly0nheart/searchcode-cli/actions/workflows/codeql.yml)
+![GitHub top language](https://img.shields.io/github/languages/top/rly0nheart/searchcode-cli?logo=github)
+![PyPI](https://img.shields.io/pypi/v/searchcode-cli?label=Latest%20Release&logo=pypi)
+![PyPI - Status](https://img.shields.io/pypi/status/searchcode-cli?label=Status&logo=pypi)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/searchcode-cli?label=Downloads&logo=pypi)
 
 # Documentation
 [Refer to the Wiki](https://github.com/rly0nheart/searchcode-cli/wiki) for installation instructions, code examples, in addition to all other documentation.
 
 # Notice
 > This project is developed with permission from [Benjamin Boyter](https://boyter.org/about/), the developer of [searchcode.com](https://searchcode.com).
 Therefore, I only take credit for this project. Not the API.
```

### Comparing `searchcode-cli-2.1.1/README.md` & `searchcode-cli-2.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 ![searchcode-cli_banner](https://user-images.githubusercontent.com/74001397/203441377-ad53a2ab-16d6-42b3-bbec-542c9ed43534.png)
 
 
 A Python wrapper around the [SearchCode API](https://searchcode.com/api/)
 
 [![Upload Python Package](https://github.com/rly0nheart/searchcode-cli/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rly0nheart/searchcode-cli/actions/workflows/python-publish.yml) [![CodeQL](https://github.com/rly0nheart/searchcode-cli/actions/workflows/codeql.yml/badge.svg)](https://github.com/rly0nheart/searchcode-cli/actions/workflows/codeql.yml)
+![GitHub top language](https://img.shields.io/github/languages/top/rly0nheart/searchcode-cli?logo=github)
+![PyPI](https://img.shields.io/pypi/v/searchcode-cli?label=Latest%20Release&logo=pypi)
+![PyPI - Status](https://img.shields.io/pypi/status/searchcode-cli?label=Status&logo=pypi)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/searchcode-cli?label=Downloads&logo=pypi)
 
 # Documentation
 [Refer to the Wiki](https://github.com/rly0nheart/searchcode-cli/wiki) for installation instructions, code examples, in addition to all other documentation.
 
 # Notice
 > This project is developed with permission from [Benjamin Boyter](https://boyter.org/about/), the developer of [searchcode.com](https://searchcode.com).
 Therefore, I only take credit for this project. Not the API.
```

#### html2text {}

```diff
@@ -1,17 +1,22 @@
 ![searchcode-cli_banner](https://user-images.githubusercontent.com/74001397/
 203441377-ad53a2ab-16d6-42b3-bbec-542c9ed43534.png) A Python wrapper around the
 [SearchCode API](https://searchcode.com/api/) [![Upload Python Package](https:/
 /github.com/rly0nheart/searchcode-cli/actions/workflows/python-publish.yml/
 badge.svg)](https://github.com/rly0nheart/searchcode-cli/actions/workflows/
 python-publish.yml) [![CodeQL](https://github.com/rly0nheart/searchcode-cli/
 actions/workflows/codeql.yml/badge.svg)](https://github.com/rly0nheart/
-searchcode-cli/actions/workflows/codeql.yml) # Documentation [Refer to the
-Wiki](https://github.com/rly0nheart/searchcode-cli/wiki) for installation
-instructions, code examples, in addition to all other documentation. # Notice >
-This project is developed with permission from [Benjamin Boyter](https://
-boyter.org/about/), the developer of [searchcode.com](https://searchcode.com).
-Therefore, I only take credit for this project. Not the API. # About SearchCode
-Read more about searchcode [here](https://searchcode.com/about/) # Support If
-you like this project and would like to show support, you can Buy Me A Coffee
-using the button below [Buy_Me_A_Coffee] Your support will be much
-appreciated!ð
+searchcode-cli/actions/workflows/codeql.yml) ![GitHub top language](https://
+img.shields.io/github/languages/top/rly0nheart/searchcode-cli?logo=github) !
+[PyPI](https://img.shields.io/pypi/v/searchcode-
+cli?label=Latest%20Release&logo=pypi) ![PyPI - Status](https://img.shields.io/
+pypi/status/searchcode-cli?label=Status&logo=pypi) ![PyPI - Downloads](https://
+img.shields.io/pypi/dm/searchcode-cli?label=Downloads&logo=pypi) #
+Documentation [Refer to the Wiki](https://github.com/rly0nheart/searchcode-cli/
+wiki) for installation instructions, code examples, in addition to all other
+documentation. # Notice > This project is developed with permission from
+[Benjamin Boyter](https://boyter.org/about/), the developer of [searchcode.com]
+(https://searchcode.com). Therefore, I only take credit for this project. Not
+the API. # About SearchCode Read more about searchcode [here](https://
+searchcode.com/about/) # Support If you like this project and would like to
+show support, you can Buy Me A Coffee using the button below [Buy_Me_A_Coffee]
+Your support will be much appreciated!ð
```

### Comparing `searchcode-cli-2.1.1/pyproject.toml` & `searchcode-cli-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "searchcode-cli"
-version = "2.1.1"
+version = "2.1.2"
 description = "A Python wrapper around the searchcode API"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["searchcode", "search-engine", "codesearch", "api-wrapper"]
 authors = [{name = "Richard Mwewa", email = "rly0nheart@duck.com"}]
 classifiers = [
```

### Comparing `searchcode-cli-2.1.1/searchcode/__init__.py` & `searchcode-cli-2.1.2/searchcode/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-
+# Search code api endpoints
 from typing import Union, Literal
 from searchcode.connection import __api_handler
-from searchcode.miscellaneous import __code_sources, __code_languages, __api_endpoints  # Search code api endpoints
+from searchcode.miscellaneous import __code_sources, __code_languages, __api_endpoints  # searchcode API endpoints
 
 
 def __join_parameters(names, sources) -> str:
     """
     Returns a single string of joined parameters for the given list of filter names and sources.
 
     Parameters:
@@ -52,358 +52,361 @@
                                     Literal['Tizen'],
                                     Literal['Gitorious'],
                                     Literal['Google Android'],
                                     Literal['GitLab'],
                                     Literal['Codeberg'],
                                     Literal['Repo.or.cz'],
                                     Literal['Sr.ht']] = None,
-                
+
                 code_languages: Union[Literal['XAML'],
-                Literal['ASP.NET'],
-                Literal['HTML'],
-                Literal['Unknown'],
-                Literal['MSBuild scripts'],
-                Literal['C#'],
-                Literal['XSD'],
-                Literal['XML'],
-                Literal['CMake'],
-                Literal['C++ Header'],
-                Literal['C++'],
-                Literal['Makefile'],
-                Literal['CSS'],
-                Literal['Python'],
-                Literal['MATLAB'],
-                Literal['Objective C'],
-                Literal['JavaScript'],
-                Literal['Java'],
-                Literal['PHP'],
-                Literal['Erlang'],
-                Literal['FORTRAN Legacy'],
-                Literal['FORTRAN Modern'],
-                Literal['C'],
-                Literal['Lisp'],
-                Literal['Visual Basic'],
-                Literal['Shell'],
-                Literal['Ruby'],
-                Literal['Vim Script'],
-                Literal['Assembly'],
-                Literal['Objective C++'],
-                Literal['Document Type Definition'],
-                Literal['SQL'],
-                Literal['YAML'],
-                Literal['Ruby HTML'],
-                Literal['Haskell'],
-                Literal['Bash'],
-                Literal['ActionScript'],
-                Literal['MXML'],
-                Literal['ASP'],
-                Literal['D'],
-                Literal['Pascal'],
-                Literal['Scala'],
-                Literal['Batch'],
-                Literal['Groovy'],
-                Literal['Extensible Stylesheet Language Transformations'],
-                Literal['Perl'],
-                Literal['Teamcenter def'],
-                Literal['IDL'],
-                Literal['Lua'],
-                Literal['Go'],
-                Literal['yacc'],
-                Literal['Cython'],
-                Literal['LEX'],
-                Literal['Ada'],
-                Literal['sed'],
-                Literal['m4'],
-                Literal['OCaml'],
-                Literal['Smarty Template'],
-                Literal['ColdFusion'],
-                Literal['NAnt scripts'],
-                Literal['Expect'],
-                Literal['C Shell'],
-                Literal['VHDL'],
-                Literal['TCL'],
-                Literal['JavaServer Pages'],
-                Literal['SKILL'],
-                Literal['AWK'],
-                Literal['MUMPS'],
-                Literal['SQL Data'],
-                Literal['Korn Shell'],
-                Literal['Patran Command Language'],
-                Literal['DAL'],
-                Literal['Fortran 95'],
-                Literal['Octave'],
-                Literal['Oracle Forms'],
-                Literal['Dart'],
-                Literal['COBOL'],
-                Literal['Modula3'],
-                Literal['Rexx'],
-                Literal['Oracle Reports'],
-                Literal['Softbridge Basic'],
-                Literal['bc'],
-                Literal['Teamcenter met'],
-                Literal['Kermit'],
-                Literal['Teamcenter mth'],
-                Literal['AMPLE'],
-                Literal['CCS'],
-                Literal['JCL'],
-                Literal['ABAP'],
-                Literal['Clojure'],
-                Literal['OpenCL'],
-                Literal['CoffeeScript'],
-                Literal['QML'],
-                Literal['AutoHotkey'],
-                Literal['ClojureScript'],
-                Literal['ColdFusion CFScript'],
-                Literal['gitignore'],
-                Literal['Config'],
-                Literal['Patch'],
-                Literal['Markdown'],
-                Literal['JSON'],
-                Literal['Portable Object'],
-                Literal['Certificate'],
-                Literal['Hg Ignore'],
-                Literal['MSBuild'],
-                Literal['Windows Module Definition'],
-                Literal['HLSL'],
-                Literal['Sass'],
-                Literal['LESS'],
-                Literal['CUDA'],
-                Literal['Swift'],
-                Literal['Maven'],
-                Literal['Visualforce Component'],
-                Literal['Verilog-SystemVerilog'],
-                Literal['JavaServer Faces'],
-                Literal['Racket'], Literal['R'],
-                Literal['Kotlin'],
-                Literal['Powershell'],
-                Literal['Rust'],
-                Literal['Velocity Template Language'],
-                Literal['Razor'],
-                Literal['F#'],
-                Literal['TypeScript'],
-                Literal['NAnt script'],
-                Literal['Ant'],
-                Literal['Arduino Sketch'],
-                Literal['Haml'],
-                Literal['Grails'],
-                Literal['Puppet'],
-                Literal['Vala'],
-                Literal['Windows Resource File'],
-                Literal['Unity-Prefab'],
-                Literal['Handlebars'],
-                Literal['Robot Framework'],
-                Literal['Pig Latin'],
-                Literal['WiX source'],
-                Literal['WiX include'],
-                Literal['Mustache'],
-                Literal['Windows Message File'],
-                Literal['XQuery'],
-                Literal['ECPP'],
-                Literal['Visualforce Page'],
-                Literal['WiX string localization'],
-                Literal['Apex Trigger'],
-                Literal['Vala Header'],
-                Literal['xBase Header'],
-                Literal['xBase'],
-                Literal['InstallShield'],
-                Literal['Harbour'],
-                Literal['Forth'],
-                Literal['PL/I'],
-                Literal['CSON'],
-                Literal['TeX'],
-                Literal['Brainfuck'],
-                Literal['Elixir'],
-                Literal['zsh'],
-                Literal['Julia'],
-                Literal['dtrace'],
-                Literal['Mathematica'],
-                Literal['Standard ML'],
-                Literal['SAS'],
-                Literal['Haxe'],
-                Literal['Nim'],
-                Literal['TTCN'],
-                Literal['Mercury'],
-                Literal['Clean'],
-                Literal['Prolog'],
-                Literal['PureScript'],
-                Literal['ERB'],
-                Literal['Stylus'],
-                Literal['XHTML'],
-                Literal['Qt Project'],
-                Literal['diff'],
-                Literal['INI'],
-                Literal['JSX'],
-                Literal['Qt Linguist'],
-                Literal['Qt'],
-                Literal['Jam'],
-                Literal['Protocol Buffers'],
-                Literal['liquid'],
-                Literal['Pug'],
-                Literal['Freemarker Template'],
-                Literal['XMI'], Literal['ClojureC'],
-                Literal['Titanium Style Sheet'],
-                Literal['Coq'],
-                Literal['Crystal'],
-                Literal['AspectJ'],
-                Literal['EEx'],
-                Literal['Elm'],
-                Literal['Twig'],
-                Literal['Slim'],
-                Literal['Logtalk'],
-                Literal['GDScript'],
-                Literal['PowerBuilder'],
-                Literal['Blade'],
-                Literal['builder'],
-                Literal['Visual Fox Pro'],
-                Literal['SQL Stored Procedure'],
-                Literal['License'],
-                Literal['Agda'],
-                Literal['Alchemist'],
-                Literal['Alex'],
-                Literal['Alloy'],
-                Literal['Android Interface Definition Language'],
-                Literal['Arvo'],
-                Literal['AsciiDoc'],
-                Literal['ATS'],
-                Literal['Autoconf'],
-                Literal['Basic'],
-                Literal['Bazel'],
-                Literal['Bitbake'],
-                Literal['Bitbucket Pipeline'],
-                Literal['Boo'],
-                Literal['Bosque'],
-                Literal['BuildStream'],
-                Literal['C Header'],
-                Literal['Cabal'],
-                Literal['Cargo Lock'],
-                Literal['Cassius'],
-                Literal['Ceylon'],
-                Literal['Closure Template'],
-                Literal['Cogent'],
-                Literal['Creole'],
-                Literal['CSV'],
-                Literal['Device Tree'],
-                Literal['Dhall'],
-                Literal['Docker ignore'],
-                Literal['Dockerfile'],
-                Literal['Emacs Dev Env'],
-                Literal['Emacs Lisp'],
-                Literal['F*'],
-                Literal['FIDL'],
-                Literal['Fish'],
-                Literal['Flow9'],
-                Literal['Fragment Shader File'],
-                Literal['Futhark'],
-                Literal['Game Maker Language'],
-                Literal['Game Maker Project'],
-                Literal['Gemfile'],
-                Literal['Gherkin Specification'],
-                Literal['GLSL'],
-                Literal['GN'],
-                Literal['Go Template'],
-                Literal['Gradle'],
-                Literal['Hamlet'],
-                Literal['Happy'],
-                Literal['HEX'],
-                Literal['Idris'],
-                Literal['ignore'],
-                Literal['Intel HEX'],
-                Literal['Isabelle'],
-                Literal['Jade'],
-                Literal['JAI'],
-                Literal['Janet'],
-                Literal['Jenkins Buildfile'],
-                Literal['Jinja'],
-                Literal['JSONL'],
-                Literal['Julius'],
-                Literal['Jupyter'],
-                Literal['Just'],
-                Literal['LaTeX'],
-                Literal['LD Script'],
-                Literal['Lean'],
-                Literal['LOLCODE'],
-                Literal['Lucius'],
-                Literal['Luna'],
-                Literal['Macromedia eXtensible Markup Language'],
-                Literal['Madlang'],
-                Literal['Mako'],
-                Literal['Meson'],
-                Literal['Module-Definition'],
-                Literal['Monkey C'],
-                Literal['MQL Header'],
-                Literal['MQL4'],
-                Literal['MQL5'],
-                Literal['Nix'],
-                Literal['nuspec'],
-                Literal['Opalang'],
-                Literal['Org'],
-                Literal['Oz'],
-                Literal['PKGBUILD'],
-                Literal['PL/SQL'],
-                Literal['Plain Text'],
-                Literal['Polly'],
-                Literal['Pony'],
-                Literal['Processing'],
-                Literal['Properties File'],
-                Literal['PSL Assertion'],
-                Literal['Q#'],
-                Literal['QCL'],
-                Literal['Rakefile'],
-                Literal['Report Definition Language'],
-                Literal['ReStructuredText'],
-                Literal['Scheme'],
-                Literal['Scons'],
-                Literal['SPDX'],
-                Literal['Specman e'],
-                Literal['Spice Netlist'],
-                Literal['SRecode Template'],
-                Literal['Stata'],
-                Literal['SVG'],
-                Literal['Swig'],
-                Literal['Systemd'],
-                Literal['SystemVerilog'],
-                Literal['TaskPaper'],
-                Literal['Terraform'],
-                Literal['Thrift'],
-                Literal['TOML'],
-                Literal['Twig Template'],
-                Literal['TypeScript Typings'],
-                Literal['Unreal Script'],
-                Literal['Ur/Web'],
-                Literal['Ur/Web Project'],
-                Literal['V'],
-                Literal['Varnish Configuration'],
-                Literal['Verilog'],
-                Literal['Verilog Args File'],
-                Literal['Vertex Shader File'],
-                Literal['Visual Basic for Applications'],
-                Literal['Vue'],
-                Literal['Web Services Description Language'],
-                Literal['Wolfram'],
-                Literal['Wren'],
-                Literal['Xcode Config'],
-                Literal['XML Schema'],
-                Literal['Xtend'],
-                Literal['Yarn'],
-                Literal['Zig'],
-                Literal['bait'],
-                Literal['CloudFormation (JSON)'],
-                Literal['CloudFormation (YAML)'],
-                Literal['CodeQL'],
-                Literal['DM'],
-                Literal['Fennel'],
-                Literal['FSL'],
-                Literal['FXML'],
-                Literal['hoon'],
-                Literal['Nial'],
-                Literal['ReasonML'],
-                Literal['Sieve'],
-                Literal['Solidity'],
-                Literal['Teal'],
-                Literal['TL'], None] = None) -> list:
+                                      Literal['ASP.NET'],
+                                      Literal['HTML'],
+                                      Literal['Unknown'],
+                                      Literal['MSBuild scripts'],
+                                      Literal['C#'],
+                                      Literal['XSD'],
+                                      Literal['XML'],
+                                      Literal['CMake'],
+                                      Literal['C++ Header'],
+                                      Literal['C++'],
+                                      Literal['Makefile'],
+                                      Literal['CSS'],
+                                      Literal['Python'],
+                                      Literal['MATLAB'],
+                                      Literal['Objective C'],
+                                      Literal['JavaScript'],
+                                      Literal['Java'],
+                                      Literal['PHP'],
+                                      Literal['Erlang'],
+                                      Literal['FORTRAN Legacy'],
+                                      Literal['FORTRAN Modern'],
+                                      Literal['C'],
+                                      Literal['Lisp'],
+                                      Literal['Visual Basic'],
+                                      Literal['Shell'],
+                                      Literal['Ruby'],
+                                      Literal['Vim Script'],
+                                      Literal['Assembly'],
+                                      Literal['Objective C++'],
+                                      Literal['Document Type Definition'],
+                                      Literal['SQL'],
+                                      Literal['YAML'],
+                                      Literal['Ruby HTML'],
+                                      Literal['Haskell'],
+                                      Literal['Bash'],
+                                      Literal['ActionScript'],
+                                      Literal['MXML'],
+                                      Literal['ASP'],
+                                      Literal['D'],
+                                      Literal['Pascal'],
+                                      Literal['Scala'],
+                                      Literal['Batch'],
+                                      Literal['Groovy'],
+                                      Literal['Extensible Stylesheet Language Transformations'],
+                                      Literal['Perl'],
+                                      Literal['Teamcenter def'],
+                                      Literal['IDL'],
+                                      Literal['Lua'],
+                                      Literal['Go'],
+                                      Literal['yacc'],
+                                      Literal['Cython'],
+                                      Literal['LEX'],
+                                      Literal['Ada'],
+                                      Literal['sed'],
+                                      Literal['m4'],
+                                      Literal['OCaml'],
+                                      Literal['Smarty Template'],
+                                      Literal['ColdFusion'],
+                                      Literal['NAnt scripts'],
+                                      Literal['Expect'],
+                                      Literal['C Shell'],
+                                      Literal['VHDL'],
+                                      Literal['TCL'],
+                                      Literal['JavaServer Pages'],
+                                      Literal['SKILL'],
+                                      Literal['AWK'],
+                                      Literal['MUMPS'],
+                                      Literal['SQL Data'],
+                                      Literal['Korn Shell'],
+                                      Literal['Patran Command Language'],
+                                      Literal['DAL'],
+                                      Literal['Fortran 95'],
+                                      Literal['Octave'],
+                                      Literal['Oracle Forms'],
+                                      Literal['Dart'],
+                                      Literal['COBOL'],
+                                      Literal['Modula3'],
+                                      Literal['Rexx'],
+                                      Literal['Oracle Reports'],
+                                      Literal['Softbridge Basic'],
+                                      Literal['bc'],
+                                      Literal['Teamcenter met'],
+                                      Literal['Kermit'],
+                                      Literal['Teamcenter mth'],
+                                      Literal['AMPLE'],
+                                      Literal['CCS'],
+                                      Literal['JCL'],
+                                      Literal['ABAP'],
+                                      Literal['Clojure'],
+                                      Literal['OpenCL'],
+                                      Literal['CoffeeScript'],
+                                      Literal['QML'],
+                                      Literal['AutoHotkey'],
+                                      Literal['ClojureScript'],
+                                      Literal['ColdFusion CFScript'],
+                                      Literal['gitignore'],
+                                      Literal['Config'],
+                                      Literal['Patch'],
+                                      Literal['Markdown'],
+                                      Literal['JSON'],
+                                      Literal['Portable Object'],
+                                      Literal['Certificate'],
+                                      Literal['Hg Ignore'],
+                                      Literal['MSBuild'],
+                                      Literal['Windows Module Definition'],
+                                      Literal['HLSL'],
+                                      Literal['Sass'],
+                                      Literal['LESS'],
+                                      Literal['CUDA'],
+                                      Literal['Swift'],
+                                      Literal['Maven'],
+                                      Literal['Visualforce Component'],
+                                      Literal['Verilog-SystemVerilog'],
+                                      Literal['JavaServer Faces'],
+                                      Literal['Racket'], 
+                                      Literal['R'],
+                                      Literal['Kotlin'],
+                                      Literal['Powershell'],
+                                      Literal['Rust'],
+                                      Literal['Velocity Template Language'],
+                                      Literal['Razor'],
+                                      Literal['F#'],
+                                      Literal['TypeScript'],
+                                      Literal['NAnt script'],
+                                      Literal['Ant'],
+                                      Literal['Arduino Sketch'],
+                                      Literal['Haml'],
+                                      Literal['Grails'],
+                                      Literal['Puppet'],
+                                      Literal['Vala'],
+                                      Literal['Windows Resource File'],
+                                      Literal['Unity-Prefab'],
+                                      Literal['Handlebars'],
+                                      Literal['Robot Framework'],
+                                      Literal['Pig Latin'],
+                                      Literal['WiX source'],
+                                      Literal['WiX include'],
+                                      Literal['Mustache'],
+                                      Literal['Windows Message File'],
+                                      Literal['XQuery'],
+                                      Literal['ECPP'],
+                                      Literal['Visualforce Page'],
+                                      Literal['WiX string localization'],
+                                      Literal['Apex Trigger'],
+                                      Literal['Vala Header'],
+                                      Literal['xBase Header'],
+                                      Literal['xBase'],
+                                      Literal['InstallShield'],
+                                      Literal['Harbour'],
+                                      Literal['Forth'],
+                                      Literal['PL/I'],
+                                      Literal['CSON'],
+                                      Literal['TeX'],
+                                      Literal['Brainfuck'],
+                                      Literal['Elixir'],
+                                      Literal['zsh'],
+                                      Literal['Julia'],
+                                      Literal['dtrace'],
+                                      Literal['Mathematica'],
+                                      Literal['Standard ML'],
+                                      Literal['SAS'],
+                                      Literal['Haxe'],
+                                      Literal['Nim'],
+                                      Literal['TTCN'],
+                                      Literal['Mercury'],
+                                      Literal['Clean'],
+                                      Literal['Prolog'],
+                                      Literal['PureScript'],
+                                      Literal['ERB'],
+                                      Literal['Stylus'],
+                                      Literal['XHTML'],
+                                      Literal['Qt Project'],
+                                      Literal['diff'],
+                                      Literal['INI'],
+                                      Literal['JSX'],
+                                      Literal['Qt Linguist'],
+                                      Literal['Qt'],
+                                      Literal['Jam'],
+                                      Literal['Protocol Buffers'],
+                                      Literal['liquid'],
+                                      Literal['Pug'],
+                                      Literal['Freemarker Template'],
+                                      Literal['XMI'], 
+                                      Literal['ClojureC'],
+                                      Literal['Titanium Style Sheet'],
+                                      Literal['Coq'],
+                                      Literal['Crystal'],
+                                      Literal['AspectJ'],
+                                      Literal['EEx'],
+                                      Literal['Elm'],
+                                      Literal['Twig'],
+                                      Literal['Slim'],
+                                      Literal['Logtalk'],
+                                      Literal['GDScript'],
+                                      Literal['PowerBuilder'],
+                                      Literal['Blade'],
+                                      Literal['builder'],
+                                      Literal['Visual Fox Pro'],
+                                      Literal['SQL Stored Procedure'],
+                                      Literal['License'],
+                                      Literal['Agda'],
+                                      Literal['Alchemist'],
+                                      Literal['Alex'],
+                                      Literal['Alloy'],
+                                      Literal['Android Interface Definition Language'],
+                                      Literal['Arvo'],
+                                      Literal['AsciiDoc'],
+                                      Literal['ATS'],
+                                      Literal['Autoconf'],
+                                      Literal['Basic'],
+                                      Literal['Bazel'],
+                                      Literal['Bitbake'],
+                                      Literal['Bitbucket Pipeline'],
+                                      Literal['Boo'],
+                                      Literal['Bosque'],
+                                      Literal['BuildStream'],
+                                      Literal['C Header'],
+                                      Literal['Cabal'],
+                                      Literal['Cargo Lock'],
+                                      Literal['Cassius'],
+                                      Literal['Ceylon'],
+                                      Literal['Closure Template'],
+                                      Literal['Cogent'],
+                                      Literal['Creole'],
+                                      Literal['CSV'],
+                                      Literal['Device Tree'],
+                                      Literal['Dhall'],
+                                      Literal['Docker ignore'],
+                                      Literal['Dockerfile'],
+                                      Literal['Emacs Dev Env'],
+                                      Literal['Emacs Lisp'],
+                                      Literal['F*'],
+                                      Literal['FIDL'],
+                                      Literal['Fish'],
+                                      Literal['Flow9'],
+                                      Literal['Fragment Shader File'],
+                                      Literal['Futhark'],
+                                      Literal['Game Maker Language'],
+                                      Literal['Game Maker Project'],
+                                      Literal['Gemfile'],
+                                      Literal['Gherkin Specification'],
+                                      Literal['GLSL'],
+                                      Literal['GN'],
+                                      Literal['Go Template'],
+                                      Literal['Gradle'],
+                                      Literal['Hamlet'],
+                                      Literal['Happy'],
+                                      Literal['HEX'],
+                                      Literal['Idris'],
+                                      Literal['ignore'],
+                                      Literal['Intel HEX'],
+                                      Literal['Isabelle'],
+                                      Literal['Jade'],
+                                      Literal['JAI'],
+                                      Literal['Janet'],
+                                      Literal['Jenkins Buildfile'],
+                                      Literal['Jinja'],
+                                      Literal['JSONL'],
+                                      Literal['Julius'],
+                                      Literal['Jupyter'],
+                                      Literal['Just'],
+                                      Literal['LaTeX'],
+                                      Literal['LD Script'],
+                                      Literal['Lean'],
+                                      Literal['LOLCODE'],
+                                      Literal['Lucius'],
+                                      Literal['Luna'],
+                                      Literal['Macromedia eXtensible Markup Language'],
+                                      Literal['Madlang'],
+                                      Literal['Mako'],
+                                      Literal['Meson'],
+                                      Literal['Module-Definition'],
+                                      Literal['Monkey C'],
+                                      Literal['MQL Header'],
+                                      Literal['MQL4'],
+                                      Literal['MQL5'],
+                                      Literal['Nix'],
+                                      Literal['nuspec'],
+                                      Literal['Opalang'],
+                                      Literal['Org'],
+                                      Literal['Oz'],
+                                      Literal['PKGBUILD'],
+                                      Literal['PL/SQL'],
+                                      Literal['Plain Text'],
+                                      Literal['Polly'],
+                                      Literal['Pony'],
+                                      Literal['Processing'],
+                                      Literal['Properties File'],
+                                      Literal['PSL Assertion'],
+                                      Literal['Q#'],
+                                      Literal['QCL'],
+                                      Literal['Rakefile'],
+                                      Literal['Report Definition Language'],
+                                      Literal['ReStructuredText'],
+                                      Literal['Scheme'],
+                                      Literal['Scons'],
+                                      Literal['SPDX'],
+                                      Literal['Specman e'],
+                                      Literal['Spice Netlist'],
+                                      Literal['SRecode Template'],
+                                      Literal['Stata'],
+                                      Literal['SVG'],
+                                      Literal['Swig'],
+                                      Literal['Systemd'],
+                                      Literal['SystemVerilog'],
+                                      Literal['TaskPaper'],
+                                      Literal['Terraform'],
+                                      Literal['Thrift'],
+                                      Literal['TOML'],
+                                      Literal['Twig Template'],
+                                      Literal['TypeScript Typings'],
+                                      Literal['Unreal Script'],
+                                      Literal['Ur/Web'],
+                                      Literal['Ur/Web Project'],
+                                      Literal['V'],
+                                      Literal['Varnish Configuration'],
+                                      Literal['Verilog'],
+                                      Literal['Verilog Args File'],
+                                      Literal['Vertex Shader File'],
+                                      Literal['Visual Basic for Applications'],
+                                      Literal['Vue'],
+                                      Literal['Web Services Description Language'],
+                                      Literal['Wolfram'],
+                                      Literal['Wren'],
+                                      Literal['Xcode Config'],
+                                      Literal['XML Schema'],
+                                      Literal['Xtend'],
+                                      Literal['Yarn'],
+                                      Literal['Zig'],
+                                      Literal['bait'],
+                                      Literal['CloudFormation (JSON)'],
+                                      Literal['CloudFormation (YAML)'],
+                                      Literal['CodeQL'],
+                                      Literal['DM'],
+                                      Literal['Fennel'],
+                                      Literal['FSL'],
+                                      Literal['FXML'],
+                                      Literal['hoon'],
+                                      Literal['Nial'],
+                                      Literal['ReasonML'],
+                                      Literal['Sieve'],
+                                      Literal['Solidity'],
+                                      Literal['Teal'],
+                                      Literal['TL']] = None) -> list:
+    
     """
     Queries the code index and returns at most 10 results.
     If the results list is empty, then this indicates that you have reached the end of the available results.
     To fetch all results for a given query, keep incrementing 'page_number'
     until you get a response with an empty results list.
 
     Parameters:
@@ -429,15 +432,16 @@
     It accepts several optional parameters, including query, page_number, per_page, max_retries, backoff_time,
     code_sources, and code_languages.
     The sources and languages lists are filtered by calling the __join_parameters function,
     which returns a single string of joined parameters based on the filter names and sources.
     The function then calls the __api_handler function to handle the API request, which returns a dictionary of results.
     The results list is then extracted and returned.
     If the results list is empty, this indicates that you have reached the end of the available results.
-    To fetch all results for a given query, keep incrementing 'page_number' until you get a page with an empty results list.
+    To fetch all results for a given query, 
+    keep incrementing 'page_number' until you get a page with an empty results list.
     """
     if code_languages is None:
         code_languages = []
     if code_sources is None:
         code_sources = []
 
     code_search_endpoint = __api_endpoints()[0]
```

### Comparing `searchcode-cli-2.1.1/searchcode/connection.py` & `searchcode-cli-2.1.2/searchcode/connection.py`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.1/searchcode/miscellaneous.py` & `searchcode-cli-2.1.2/searchcode/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `searchcode-cli-2.1.1/searchcode_cli.egg-info/PKG-INFO` & `searchcode-cli-2.1.2/searchcode_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchcode-cli
-Version: 2.1.1
+Version: 2.1.2
 Summary: A Python wrapper around the searchcode API
 Author-email: Richard Mwewa <rly0nheart@duck.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,14 +695,18 @@
 
 ![searchcode-cli_banner](https://user-images.githubusercontent.com/74001397/203441377-ad53a2ab-16d6-42b3-bbec-542c9ed43534.png)
 
 
 A Python wrapper around the [SearchCode API](https://searchcode.com/api/)
 
 [![Upload Python Package](https://github.com/rly0nheart/searchcode-cli/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rly0nheart/searchcode-cli/actions/workflows/python-publish.yml) [![CodeQL](https://github.com/rly0nheart/searchcode-cli/actions/workflows/codeql.yml/badge.svg)](https://github.com/rly0nheart/searchcode-cli/actions/workflows/codeql.yml)
+![GitHub top language](https://img.shields.io/github/languages/top/rly0nheart/searchcode-cli?logo=github)
+![PyPI](https://img.shields.io/pypi/v/searchcode-cli?label=Latest%20Release&logo=pypi)
+![PyPI - Status](https://img.shields.io/pypi/status/searchcode-cli?label=Status&logo=pypi)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/searchcode-cli?label=Downloads&logo=pypi)
 
 # Documentation
 [Refer to the Wiki](https://github.com/rly0nheart/searchcode-cli/wiki) for installation instructions, code examples, in addition to all other documentation.
 
 # Notice
 > This project is developed with permission from [Benjamin Boyter](https://boyter.org/about/), the developer of [searchcode.com](https://searchcode.com).
 Therefore, I only take credit for this project. Not the API.
```

