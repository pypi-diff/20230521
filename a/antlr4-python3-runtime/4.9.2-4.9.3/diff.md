# Comparing `tmp/antlr4-python3-runtime-4.9.2.tar.gz` & `tmp/antlr4-python3-runtime-4.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antlr4-python3-runtime-4.9.2.tar", last modified: Thu Mar 11 22:36:56 2021, max compression
+gzip compressed data, was "dist/antlr4-python3-runtime-4.9.3.tar", last modified: Sat Nov  6 17:52:22 2021, max compression
```

## Comparing `antlr4-python3-runtime-4.9.2.tar` & `antlr4-python3-runtime-4.9.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:56.554024 antlr4-python3-runtime-4.9.2/
--rw-r--r--   0 parrt      (502) wheel        (0)       46 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/MANIFEST.in
--rw-r--r--   0 parrt      (502) wheel        (0)      282 2021-03-11 22:36:56.553612 antlr4-python3-runtime-4.9.2/PKG-INFO
--rw-r--r--   0 parrt      (502) wheel        (0)      186 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/README.txt
--rw-r--r--   0 parrt      (502) wheel        (0)      387 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/RELEASE-4.5.txt
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:56.532377 antlr4-python3-runtime-4.9.2/bin/
--rwxr-xr-x   0 parrt      (502) wheel        (0)     6111 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/bin/pygrun
--rw-r--r--   0 parrt      (502) wheel        (0)       38 2021-03-11 22:36:56.554140 antlr4-python3-runtime-4.9.2/setup.cfg
--rw-r--r--   0 parrt      (502) wheel        (0)      527 2021-03-11 22:02:06.000000 antlr4-python3-runtime-4.9.2/setup.py
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:56.530931 antlr4-python3-runtime-4.9.2/src/
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:56.538621 antlr4-python3-runtime-4.9.2/src/antlr4/
--rw-r--r--   0 parrt      (502) wheel        (0)    10740 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/BufferedTokenStream.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2110 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/CommonTokenFactory.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2770 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/CommonTokenStream.py
--rw-r--r--   0 parrt      (502) wheel        (0)      868 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/FileStream.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2334 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/InputStream.py
--rw-r--r--   0 parrt      (502) wheel        (0)     5965 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/IntervalSet.py
--rw-r--r--   0 parrt      (502) wheel        (0)     7752 2021-02-16 17:10:10.000000 antlr4-python3-runtime-4.9.2/src/antlr4/LL1Analyzer.py
--rw-r--r--   0 parrt      (502) wheel        (0)    11542 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/Lexer.py
--rw-r--r--   0 parrt      (502) wheel        (0)     5356 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/ListTokenSource.py
--rw-r--r--   0 parrt      (502) wheel        (0)    22883 2021-02-16 17:10:10.000000 antlr4-python3-runtime-4.9.2/src/antlr4/Parser.py
--rw-r--r--   0 parrt      (502) wheel        (0)     7206 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/ParserInterpreter.py
--rw-r--r--   0 parrt      (502) wheel        (0)     6762 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/ParserRuleContext.py
--rw-r--r--   0 parrt      (502) wheel        (0)    22977 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/PredictionContext.py
--rw-r--r--   0 parrt      (502) wheel        (0)     5383 2021-03-11 22:02:09.000000 antlr4-python3-runtime-4.9.2/src/antlr4/Recognizer.py
--rw-r--r--   0 parrt      (502) wheel        (0)     8099 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/RuleContext.py
--rw-r--r--   0 parrt      (502) wheel        (0)      303 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/StdinStream.py
--rw-r--r--   0 parrt      (502) wheel        (0)     5206 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/Token.py
--rw-r--r--   0 parrt      (502) wheel        (0)    10324 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/TokenStreamRewriter.py
--rw-r--r--   0 parrt      (502) wheel        (0)      931 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/Utils.py
--rw-r--r--   0 parrt      (502) wheel        (0)     1125 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/__init__.py
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:56.543129 antlr4-python3-runtime-4.9.2/src/antlr4/atn/
--rw-r--r--   0 parrt      (502) wheel        (0)     5789 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATN.py
--rw-r--r--   0 parrt      (502) wheel        (0)     6565 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATNConfig.py
--rw-r--r--   0 parrt      (502) wheel        (0)     8312 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATNConfigSet.py
--rw-r--r--   0 parrt      (502) wheel        (0)     1010 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATNDeserializationOptions.py
--rw-r--r--   0 parrt      (502) wheel        (0)    22252 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATNDeserializer.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2298 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATNSimulator.py
--rw-r--r--   0 parrt      (502) wheel        (0)     7663 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATNState.py
--rw-r--r--   0 parrt      (502) wheel        (0)      422 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATNType.py
--rw-r--r--   0 parrt      (502) wheel        (0)    25465 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/LexerATNSimulator.py
--rw-r--r--   0 parrt      (502) wheel        (0)    10014 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/LexerAction.py
--rw-r--r--   0 parrt      (502) wheel        (0)     6420 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/LexerActionExecutor.py
--rw-r--r--   0 parrt      (502) wheel        (0)    80365 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/ParserATNSimulator.py
--rw-r--r--   0 parrt      (502) wheel        (0)    22486 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/PredictionMode.py
--rw-r--r--   0 parrt      (502) wheel        (0)    10495 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/SemanticContext.py
--rw-r--r--   0 parrt      (502) wheel        (0)     8762 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/Transition.py
--rw-r--r--   0 parrt      (502) wheel        (0)       28 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/atn/__init__.py
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:56.544181 antlr4-python3-runtime-4.9.2/src/antlr4/dfa/
--rw-r--r--   0 parrt      (502) wheel        (0)     5388 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/dfa/DFA.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2518 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/dfa/DFASerializer.py
--rw-r--r--   0 parrt      (502) wheel        (0)     5583 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/dfa/DFAState.py
--rw-r--r--   0 parrt      (502) wheel        (0)       28 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/dfa/__init__.py
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:56.545963 antlr4-python3-runtime-4.9.2/src/antlr4/error/
--rw-r--r--   0 parrt      (502) wheel        (0)     4430 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/error/DiagnosticErrorListener.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2722 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/error/ErrorListener.py
--rw-r--r--   0 parrt      (502) wheel        (0)    30391 2021-02-16 17:10:10.000000 antlr4-python3-runtime-4.9.2/src/antlr4/error/ErrorStrategy.py
--rw-r--r--   0 parrt      (502) wheel        (0)     6759 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/error/Errors.py
--rw-r--r--   0 parrt      (502) wheel        (0)       28 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/error/__init__.py
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:56.550028 antlr4-python3-runtime-4.9.2/src/antlr4/tree/
--rw-r--r--   0 parrt      (502) wheel        (0)      695 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/tree/Chunk.py
--rw-r--r--   0 parrt      (502) wheel        (0)     4485 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/tree/ParseTreeMatch.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2825 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/tree/ParseTreePattern.py
--rw-r--r--   0 parrt      (502) wheel        (0)    16388 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/tree/ParseTreePatternMatcher.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2022 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/tree/RuleTagToken.py
--rw-r--r--   0 parrt      (502) wheel        (0)     1576 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/tree/TokenTagToken.py
--rw-r--r--   0 parrt      (502) wheel        (0)     5572 2021-01-03 17:32:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4/tree/Tree.py
--rw-r--r--   0 parrt      (502) wheel        (0)     3968 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/tree/Trees.py
--rw-r--r--   0 parrt      (502) wheel        (0)        0 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/tree/__init__.py
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:56.550836 antlr4-python3-runtime-4.9.2/src/antlr4/xpath/
--rw-r--r--   0 parrt      (502) wheel        (0)    13015 2021-01-03 18:05:48.000000 antlr4-python3-runtime-4.9.2/src/antlr4/xpath/XPath.py
--rw-r--r--   0 parrt      (502) wheel        (0)       28 2020-11-26 18:51:12.000000 antlr4-python3-runtime-4.9.2/src/antlr4/xpath/__init__.py
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:56.553026 antlr4-python3-runtime-4.9.2/src/antlr4_python3_runtime.egg-info/
--rw-r--r--   0 parrt      (502) wheel        (0)      282 2021-03-11 22:36:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4_python3_runtime.egg-info/PKG-INFO
--rw-r--r--   0 parrt      (502) wheel        (0)     1968 2021-03-11 22:36:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4_python3_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 parrt      (502) wheel        (0)        1 2021-03-11 22:36:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4_python3_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 parrt      (502) wheel        (0)       34 2021-03-11 22:36:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4_python3_runtime.egg-info/requires.txt
--rw-r--r--   0 parrt      (502) wheel        (0)        7 2021-03-11 22:36:56.000000 antlr4-python3-runtime-4.9.2/src/antlr4_python3_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:52:21.999339 antlr4-python3-runtime-4.9.3/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)       46 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/MANIFEST.in
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      282 2021-11-06 17:52:21.998926 antlr4-python3-runtime-4.9.3/PKG-INFO
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      186 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/README.txt
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      387 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/RELEASE-4.5.txt
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:52:21.969584 antlr4-python3-runtime-4.9.3/bin/
+-rwxr-xr-x   0 ericvergnaud   (501) staff       (20)     6111 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/bin/pygrun
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)       38 2021-11-06 17:52:21.999487 antlr4-python3-runtime-4.9.3/setup.cfg
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      527 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/setup.py
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:52:21.968132 antlr4-python3-runtime-4.9.3/src/
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:52:21.977090 antlr4-python3-runtime-4.9.3/src/antlr4/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    10780 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/BufferedTokenStream.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2110 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/CommonTokenFactory.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2770 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/CommonTokenStream.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      868 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/FileStream.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2334 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/InputStream.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5965 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/IntervalSet.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     7752 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/LL1Analyzer.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    11542 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/Lexer.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5356 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/ListTokenSource.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    22883 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/Parser.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     7206 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/ParserInterpreter.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     6762 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/ParserRuleContext.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    22977 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/PredictionContext.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5383 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/Recognizer.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     8099 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/RuleContext.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      303 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/StdinStream.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5206 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/Token.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    10324 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/TokenStreamRewriter.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      931 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/Utils.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     1125 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/__init__.py
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:52:21.985275 antlr4-python3-runtime-4.9.3/src/antlr4/atn/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5789 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATN.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     6565 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATNConfig.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     8312 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATNConfigSet.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     1010 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATNDeserializationOptions.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    22252 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATNDeserializer.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2298 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATNSimulator.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     7663 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATNState.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      422 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATNType.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    25465 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/LexerATNSimulator.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    10014 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/LexerAction.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     6420 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/LexerActionExecutor.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    80365 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/ParserATNSimulator.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    22486 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/PredictionMode.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    10495 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/SemanticContext.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     8762 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/Transition.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)       28 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/atn/__init__.py
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:52:21.987449 antlr4-python3-runtime-4.9.3/src/antlr4/dfa/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5388 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/dfa/DFA.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2518 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/dfa/DFASerializer.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5583 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/dfa/DFAState.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)       28 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/dfa/__init__.py
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:52:21.990318 antlr4-python3-runtime-4.9.3/src/antlr4/error/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     4430 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/error/DiagnosticErrorListener.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2722 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/error/ErrorListener.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    30391 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/error/ErrorStrategy.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     6759 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/error/Errors.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)       28 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/error/__init__.py
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:52:21.994996 antlr4-python3-runtime-4.9.3/src/antlr4/tree/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      695 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/tree/Chunk.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     4485 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/tree/ParseTreeMatch.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2825 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/tree/ParseTreePattern.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    16388 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/tree/ParseTreePatternMatcher.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2022 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/tree/RuleTagToken.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     1576 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/tree/TokenTagToken.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5572 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/tree/Tree.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     3968 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/tree/Trees.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/tree/__init__.py
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:52:21.995798 antlr4-python3-runtime-4.9.3/src/antlr4/xpath/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    13015 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/xpath/XPath.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)       28 2021-11-06 15:35:29.000000 antlr4-python3-runtime-4.9.3/src/antlr4/xpath/__init__.py
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:52:21.998299 antlr4-python3-runtime-4.9.3/src/antlr4_python3_runtime.egg-info/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      282 2021-11-06 17:52:21.000000 antlr4-python3-runtime-4.9.3/src/antlr4_python3_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     1968 2021-11-06 17:52:21.000000 antlr4-python3-runtime-4.9.3/src/antlr4_python3_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)        1 2021-11-06 17:52:21.000000 antlr4-python3-runtime-4.9.3/src/antlr4_python3_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)       34 2021-11-06 17:52:21.000000 antlr4-python3-runtime-4.9.3/src/antlr4_python3_runtime.egg-info/requires.txt
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)        7 2021-11-06 17:52:21.000000 antlr4-python3-runtime-4.9.3/src/antlr4_python3_runtime.egg-info/top_level.txt
```

### Comparing `antlr4-python3-runtime-4.9.2/bin/pygrun` & `antlr4-python3-runtime-4.9.3/bin/pygrun`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/setup.py` & `antlr4-python3-runtime-4.9.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 setup(
     name='antlr4-python3-runtime',
-    version='4.9.2',
+    version='4.9.3',
     packages=['antlr4', 'antlr4.atn', 'antlr4.dfa', 'antlr4.tree', 'antlr4.error', 'antlr4.xpath'],
     package_dir={'': 'src'},
     install_requires=[
         "typing ; python_version<'3.5'",
     ],
     url='http://www.antlr.org',
     license='BSD',
     author='Eric Vergnaud, Terence Parr, Sam Harwell',
     author_email='eric.vergnaud@wanadoo.fr',
     scripts=["bin/pygrun"],
-    description='ANTLR 4.9.2 runtime for Python 3.7'
+    description='ANTLR 4.9.3 runtime for Python 3.7'
 )
```

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/BufferedTokenStream.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/BufferedTokenStream.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,25 +195,25 @@
         self.tokenSource = tokenSource
         self.tokens = []
         self.index = -1
         self.fetchedEOF = False
 
 
     # Given a starting index, return the index of the next token on channel.
-    #  Return i if tokens[i] is on channel.  Return -1 if there are no tokens
-    #  on channel between i and EOF.
+    #  Return i if tokens[i] is on channel.  Return the index of the EOF token
+    # if there are no tokens on channel between i and EOF.
     #/
     def nextTokenOnChannel(self, i:int, channel:int):
         self.sync(i)
         if i>=len(self.tokens):
-            return -1
+            return len(self.tokens) - 1
         token = self.tokens[i]
         while token.channel!=channel:
             if token.type==Token.EOF:
-                return -1
+                return i
             i += 1
             self.sync(i)
             token = self.tokens[i]
         return i
 
     # Given a starting index, return the index of the previous token on channel.
     #  Return i if tokens[i] is on channel. Return -1 if there are no tokens
```

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/CommonTokenFactory.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/CommonTokenFactory.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/CommonTokenStream.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/CommonTokenStream.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/FileStream.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/FileStream.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/InputStream.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/InputStream.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/IntervalSet.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/IntervalSet.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from io import StringIO
 from antlr4.Token import Token
 
 # need forward declarations
 IntervalSet = None
 
 class IntervalSet(object):
-    __slots__ = ('intervals', 'readOnly')
+    __slots__ = ('intervals', 'readonly')
 
     def __init__(self):
         self.intervals = None
-        self.readOnly = False
+        self.readonly = False
 
     def __iter__(self):
         if self.intervals is not None:
             for i in self.intervals:
                 for c in i:
                     yield c
```

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/LL1Analyzer.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/LL1Analyzer.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/Lexer.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/Lexer.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/ListTokenSource.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/ListTokenSource.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/Parser.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/Parser.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/ParserInterpreter.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/ParserInterpreter.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/ParserRuleContext.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/ParserRuleContext.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/PredictionContext.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/PredictionContext.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/Recognizer.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/Recognizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             pos = version.find("-")
         if pos==-1:
             pos = len(version)
         minor = version[0:pos]
         return major, minor
 
     def checkVersion(self, toolVersion):
-        runtimeVersion = "4.9.2"
+        runtimeVersion = "4.9.3"
         rvmajor, rvminor = self.extractVersion(runtimeVersion)
         tvmajor, tvminor = self.extractVersion(toolVersion)
         if rvmajor!=tvmajor or rvminor!=tvminor:
             print("ANTLR runtime and generated code versions disagree: "+runtimeVersion+"!="+toolVersion)
 
     def addErrorListener(self, listener):
         self._listeners.append(listener)
```

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/RuleContext.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/RuleContext.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/Token.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/Token.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/TokenStreamRewriter.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/TokenStreamRewriter.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/Utils.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/Utils.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/__init__.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/__init__.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATN.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATN.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     # Compute the set of valid tokens that can occur starting in {@code s} and
     # staying in same rule. {@link Token#EPSILON} is in set if we reach end of
     # rule.
     def nextTokensNoContext(self, s:ATNState):
         if s.nextTokenWithinRule is not None:
             return s.nextTokenWithinRule
         s.nextTokenWithinRule = self.nextTokensInContext(s, None)
-        s.nextTokenWithinRule.readOnly = True
+        s.nextTokenWithinRule.readonly = True
         return s.nextTokenWithinRule
 
     def nextTokens(self, s:ATNState, ctx:RuleContext = None):
         if ctx==None:
             return self.nextTokensNoContext(s)
         else:
             return self.nextTokensInContext(s, ctx)
```

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATNConfig.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATNConfig.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATNConfigSet.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATNConfigSet.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATNDeserializationOptions.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATNDeserializationOptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 # Use of this file is governed by the BSD 3-clause license that
 # can be found in the LICENSE.txt file in the project root.
 
 # need a forward declaration
 ATNDeserializationOptions = None
 
 class ATNDeserializationOptions(object):
-    __slots__ = ('readOnly', 'verifyATN', 'generateRuleBypassTransitions')
+    __slots__ = ('readonly', 'verifyATN', 'generateRuleBypassTransitions')
 
     defaultOptions = None
 
     def __init__(self, copyFrom:ATNDeserializationOptions = None):
-        self.readOnly = False
+        self.readonly = False
         self.verifyATN = True if copyFrom is None else copyFrom.verifyATN
         self.generateRuleBypassTransitions = False if copyFrom is None else copyFrom.generateRuleBypassTransitions
 
     def __setattr__(self, key, value):
-        if key!="readOnly" and self.readOnly:
+        if key!="readonly" and self.readonly:
             raise Exception("The object is read only.")
         super(type(self), self).__setattr__(key,value)
 
 ATNDeserializationOptions.defaultOptions = ATNDeserializationOptions()
-ATNDeserializationOptions.defaultOptions.readOnly = True
+ATNDeserializationOptions.defaultOptions.readonly = True
```

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATNDeserializer.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATNDeserializer.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATNSimulator.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATNSimulator.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/ATNState.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/ATNState.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/LexerATNSimulator.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/LexerATNSimulator.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/LexerAction.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/LexerAction.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/LexerActionExecutor.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/LexerActionExecutor.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/ParserATNSimulator.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/ParserATNSimulator.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/PredictionMode.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/PredictionMode.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/SemanticContext.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/SemanticContext.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/atn/Transition.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/atn/Transition.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/dfa/DFA.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/dfa/DFA.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/dfa/DFASerializer.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/dfa/DFASerializer.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/dfa/DFAState.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/dfa/DFAState.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/error/DiagnosticErrorListener.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/error/DiagnosticErrorListener.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/error/ErrorListener.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/error/ErrorListener.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/error/ErrorStrategy.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/error/ErrorStrategy.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/error/Errors.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/error/Errors.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/tree/Chunk.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/tree/Chunk.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/tree/ParseTreeMatch.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/tree/ParseTreeMatch.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/tree/ParseTreePattern.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/tree/ParseTreePattern.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/tree/ParseTreePatternMatcher.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/tree/ParseTreePatternMatcher.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/tree/RuleTagToken.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/tree/RuleTagToken.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/tree/TokenTagToken.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/tree/TokenTagToken.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/tree/Tree.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/tree/Tree.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/tree/Trees.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/tree/Trees.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4/xpath/XPath.py` & `antlr4-python3-runtime-4.9.3/src/antlr4/xpath/XPath.py`

 * *Files identical despite different names*

### Comparing `antlr4-python3-runtime-4.9.2/src/antlr4_python3_runtime.egg-info/SOURCES.txt` & `antlr4-python3-runtime-4.9.3/src/antlr4_python3_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

