# Comparing `tmp/antlr4-python2-runtime-4.9.2.tar.gz` & `tmp/antlr4-python2-runtime-4.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antlr4-python2-runtime-4.9.2.tar", last modified: Thu Mar 11 22:36:45 2021, max compression
+gzip compressed data, was "dist/antlr4-python2-runtime-4.9.3.tar", last modified: Sat Nov  6 17:51:03 2021, max compression
```

## Comparing `antlr4-python2-runtime-4.9.2.tar` & `antlr4-python2-runtime-4.9.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/
--rw-r--r--   0 parrt      (502) wheel        (0)      444 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/RELEASE-4.5.txt
--rw-r--r--   0 parrt      (502) wheel        (0)      285 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/PKG-INFO
--rw-r--r--   0 parrt      (502) wheel        (0)       13 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/MANIFEST.in
--rw-r--r--   0 parrt      (502) wheel        (0)      431 2021-03-11 22:01:58.000000 antlr4-python2-runtime-4.9.2/setup.py
--rw-r--r--   0 parrt      (502) wheel        (0)      186 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/README.txt
--rw-r--r--   0 parrt      (502) wheel        (0)       38 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/setup.cfg
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/src/
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/src/antlr4/
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/src/antlr4/tree/
--rw-r--r--   0 parrt      (502) wheel        (0)     5298 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/tree/Tree.py
--rw-r--r--   0 parrt      (502) wheel        (0)     1993 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/tree/RuleTagToken.py
--rw-r--r--   0 parrt      (502) wheel        (0)    16014 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/tree/ParseTreePatternMatcher.py
--rw-r--r--   0 parrt      (502) wheel        (0)        0 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/tree/__init__.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2564 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/tree/ParseTreePattern.py
--rw-r--r--   0 parrt      (502) wheel        (0)      681 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/tree/Chunk.py
--rw-r--r--   0 parrt      (502) wheel        (0)     1577 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/tree/TokenTagToken.py
--rw-r--r--   0 parrt      (502) wheel        (0)     3806 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/tree/Trees.py
--rw-r--r--   0 parrt      (502) wheel        (0)     4341 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/tree/ParseTreeMatch.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2040 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/CommonTokenFactory.py
--rw-r--r--   0 parrt      (502) wheel        (0)     5193 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/Token.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2965 2020-11-26 19:01:56.000000 antlr4-python2-runtime-4.9.2/src/antlr4/InputStream.py
--rw-r--r--   0 parrt      (502) wheel        (0)      900 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/FileStream.py
--rw-r--r--   0 parrt      (502) wheel        (0)     5275 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/ListTokenSource.py
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/src/antlr4/xpath/
--rw-r--r--   0 parrt      (502) wheel        (0)       28 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/xpath/__init__.py
--rw-r--r--   0 parrt      (502) wheel        (0)    11668 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/xpath/XPath.py
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/src/antlr4/dfa/
--rw-r--r--   0 parrt      (502) wheel        (0)     2485 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/dfa/DFASerializer.py
--rw-r--r--   0 parrt      (502) wheel        (0)       28 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/dfa/__init__.py
--rw-r--r--   0 parrt      (502) wheel        (0)     5280 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/dfa/DFA.py
--rw-r--r--   0 parrt      (502) wheel        (0)     5435 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/dfa/DFAState.py
--rw-r--r--   0 parrt      (502) wheel        (0)     5203 2021-03-11 22:02:03.000000 antlr4-python2-runtime-4.9.2/src/antlr4/Recognizer.py
--rw-r--r--   0 parrt      (502) wheel        (0)     1111 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/__init__.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2304 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/CodePoints.py
--rw-r--r--   0 parrt      (502) wheel        (0)    10619 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/BufferedTokenStream.py
--rw-r--r--   0 parrt      (502) wheel        (0)    22057 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/Parser.py
--rw-r--r--   0 parrt      (502) wheel        (0)     6476 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/ParserRuleContext.py
--rw-r--r--   0 parrt      (502) wheel        (0)     6859 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/ParserInterpreter.py
--rw-r--r--   0 parrt      (502) wheel        (0)     7564 2021-02-16 17:10:10.000000 antlr4-python2-runtime-4.9.2/src/antlr4/LL1Analyzer.py
--rw-r--r--   0 parrt      (502) wheel        (0)    22598 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/PredictionContext.py
--rw-r--r--   0 parrt      (502) wheel        (0)     1085 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/Utils.py
--rw-r--r--   0 parrt      (502) wheel        (0)     7979 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/RuleContext.py
--rw-r--r--   0 parrt      (502) wheel        (0)    11022 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/Lexer.py
--rw-r--r--   0 parrt      (502) wheel        (0)     9085 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/IntervalSet.py
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/
--rw-r--r--   0 parrt      (502) wheel        (0)      847 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATNDeserializationOptions.py
--rw-r--r--   0 parrt      (502) wheel        (0)    10015 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/SemanticContext.py
--rwxr-xr-x   0 parrt      (502) wheel        (0)     8080 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATNConfigSet.py
--rw-r--r--   0 parrt      (502) wheel        (0)     5308 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATN.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2091 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATNSimulator.py
--rw-r--r--   0 parrt      (502) wheel        (0)     8170 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/Transition.py
--rw-r--r--   0 parrt      (502) wheel        (0)       28 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/__init__.py
--rw-r--r--   0 parrt      (502) wheel        (0)      304 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATNType.py
--rw-r--r--   0 parrt      (502) wheel        (0)     9997 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/LexerAction.py
--rw-r--r--   0 parrt      (502) wheel        (0)    22068 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATNDeserializer.py
--rw-r--r--   0 parrt      (502) wheel        (0)    24433 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/LexerATNSimulator.py
--rwxr-xr-x   0 parrt      (502) wheel        (0)    78880 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/ParserATNSimulator.py
--rw-r--r--   0 parrt      (502) wheel        (0)     6173 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/LexerActionExecutor.py
--rw-r--r--   0 parrt      (502) wheel        (0)    22272 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/PredictionMode.py
--rw-r--r--   0 parrt      (502) wheel        (0)     7542 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATNState.py
--rw-r--r--   0 parrt      (502) wheel        (0)     6075 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATNConfig.py
--rw-r--r--   0 parrt      (502) wheel        (0)      572 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/StdinStream.py
--rw-r--r--   0 parrt      (502) wheel        (0)    10258 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/TokenStreamRewriter.py
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/src/antlr4/error/
--rw-r--r--   0 parrt      (502) wheel        (0)     2783 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/error/ErrorListener.py
--rw-r--r--   0 parrt      (502) wheel        (0)       28 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/error/__init__.py
--rw-r--r--   0 parrt      (502) wheel        (0)    30008 2021-02-16 17:10:10.000000 antlr4-python2-runtime-4.9.2/src/antlr4/error/ErrorStrategy.py
--rw-r--r--   0 parrt      (502) wheel        (0)     6478 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/error/Errors.py
--rw-r--r--   0 parrt      (502) wheel        (0)     4265 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/error/DiagnosticErrorListener.py
--rw-r--r--   0 parrt      (502) wheel        (0)     2714 2020-11-26 18:51:12.000000 antlr4-python2-runtime-4.9.2/src/antlr4/CommonTokenStream.py
-drwxr-xr-x   0 parrt      (502) wheel        (0)        0 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/src/antlr4_python2_runtime.egg-info/
--rw-r--r--   0 parrt      (502) wheel        (0)      285 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/src/antlr4_python2_runtime.egg-info/PKG-INFO
--rw-r--r--   0 parrt      (502) wheel        (0)     1933 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/src/antlr4_python2_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 parrt      (502) wheel        (0)        7 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/src/antlr4_python2_runtime.egg-info/top_level.txt
--rw-r--r--   0 parrt      (502) wheel        (0)        1 2021-03-11 22:36:45.000000 antlr4-python2-runtime-4.9.2/src/antlr4_python2_runtime.egg-info/dependency_links.txt
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      444 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/RELEASE-4.5.txt
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      285 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/PKG-INFO
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)       13 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/MANIFEST.in
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      431 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/setup.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      186 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/README.txt
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)       38 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/setup.cfg
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/src/
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/src/antlr4/
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/src/antlr4/tree/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5298 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/tree/Tree.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     1993 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/tree/RuleTagToken.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    16014 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/tree/ParseTreePatternMatcher.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/tree/__init__.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2564 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/tree/ParseTreePattern.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      681 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/tree/Chunk.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     1577 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/tree/TokenTagToken.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     3806 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/tree/Trees.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     4341 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/tree/ParseTreeMatch.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2040 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/CommonTokenFactory.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5193 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/Token.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2965 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/InputStream.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      900 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/FileStream.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5275 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/ListTokenSource.py
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/src/antlr4/xpath/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)       28 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/xpath/__init__.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    11668 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/xpath/XPath.py
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/src/antlr4/dfa/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2485 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/dfa/DFASerializer.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)       28 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/dfa/__init__.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5280 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/dfa/DFA.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5435 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/dfa/DFAState.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5203 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/Recognizer.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     1111 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/__init__.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2304 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/CodePoints.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    10660 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/BufferedTokenStream.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    22057 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/Parser.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     6476 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/ParserRuleContext.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     6859 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/ParserInterpreter.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     7564 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/LL1Analyzer.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    22598 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/PredictionContext.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     1085 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/Utils.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     7979 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/RuleContext.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    11022 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/Lexer.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     9105 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/IntervalSet.py
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      847 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATNDeserializationOptions.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    10015 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/SemanticContext.py
+-rwxr-xr-x   0 ericvergnaud   (501) staff       (20)     8080 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATNConfigSet.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     5308 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATN.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2091 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATNSimulator.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     8170 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/Transition.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)       28 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/__init__.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      304 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATNType.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     9997 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/LexerAction.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    22068 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATNDeserializer.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    24433 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/LexerATNSimulator.py
+-rwxr-xr-x   0 ericvergnaud   (501) staff       (20)    78880 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/ParserATNSimulator.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     6173 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/LexerActionExecutor.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    22272 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/PredictionMode.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     7542 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATNState.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     6075 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATNConfig.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      572 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/StdinStream.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    10258 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/TokenStreamRewriter.py
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/src/antlr4/error/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2783 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/error/ErrorListener.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)       28 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/error/__init__.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)    30008 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/error/ErrorStrategy.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     6478 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/error/Errors.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     4265 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/error/DiagnosticErrorListener.py
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     2714 2021-11-06 15:35:29.000000 antlr4-python2-runtime-4.9.3/src/antlr4/CommonTokenStream.py
+drwxr-xr-x   0 ericvergnaud   (501) staff       (20)        0 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/src/antlr4_python2_runtime.egg-info/
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)      285 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/src/antlr4_python2_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)     1933 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/src/antlr4_python2_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)        7 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/src/antlr4_python2_runtime.egg-info/top_level.txt
+-rw-r--r--   0 ericvergnaud   (501) staff       (20)        1 2021-11-06 17:51:03.000000 antlr4-python2-runtime-4.9.3/src/antlr4_python2_runtime.egg-info/dependency_links.txt
```

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/tree/Tree.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/tree/Tree.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/tree/RuleTagToken.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/tree/RuleTagToken.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/tree/ParseTreePatternMatcher.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/tree/ParseTreePatternMatcher.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/tree/ParseTreePattern.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/tree/ParseTreePattern.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/tree/Chunk.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/tree/Chunk.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/tree/TokenTagToken.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/tree/TokenTagToken.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/tree/Trees.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/tree/Trees.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/tree/ParseTreeMatch.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/tree/ParseTreeMatch.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/CommonTokenFactory.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/CommonTokenFactory.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/Token.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/Token.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/InputStream.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/InputStream.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/FileStream.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/FileStream.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/ListTokenSource.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/ListTokenSource.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/xpath/XPath.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/xpath/XPath.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/dfa/DFASerializer.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/dfa/DFASerializer.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/dfa/DFA.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/dfa/DFA.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/dfa/DFAState.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/dfa/DFAState.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/Recognizer.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/Recognizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
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

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/__init__.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/__init__.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/CodePoints.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/CodePoints.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/BufferedTokenStream.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/BufferedTokenStream.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,25 +192,25 @@
         self.tokenSource = tokenSource
         self.tokens = []
         self.index = -1
         self.fetchedEOF = False
 
 
     # Given a starting index, return the index of the next token on channel.
-    #  Return i if tokens[i] is on channel.  Return -1 if there are no tokens
-    #  on channel between i and EOF.
+    #  Return i if tokens[i] is on channel.  Return the index of the EOF toekn
+    #  if there are no tokens on channel between i and EOF.
     #/
     def nextTokenOnChannel(self, i, channel):
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

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/Parser.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/Parser.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/ParserRuleContext.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/ParserRuleContext.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/ParserInterpreter.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/ParserInterpreter.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/LL1Analyzer.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/LL1Analyzer.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/PredictionContext.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/PredictionContext.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/Utils.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/Utils.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/RuleContext.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/RuleContext.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/Lexer.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/Lexer.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/IntervalSet.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/IntervalSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     def __iter__(self):
         return iter(self.range)
 
 
 class IntervalSet(object):
 
     def __init__(self):
-        self.intervals = None
-        self.readOnly = False
+        self.intervals = None # type: list | None
+        self.readonly = False
 
     def __iter__(self):
         if self.intervals is not None:
             for i in self.intervals:
                 for c in i:
                     yield c
```

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATNDeserializationOptions.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATNDeserializationOptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # can be found in the LICENSE.txt file in the project root.
 
 class ATNDeserializationOptions(object):
 
     defaultOptions = None
 
     def __init__(self, copyFrom = None):
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

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/SemanticContext.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/SemanticContext.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATNConfigSet.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATNConfigSet.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATN.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATN.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATNSimulator.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATNSimulator.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/Transition.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/Transition.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/LexerAction.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/LexerAction.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATNDeserializer.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATNDeserializer.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/LexerATNSimulator.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/LexerATNSimulator.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/ParserATNSimulator.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/ParserATNSimulator.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/LexerActionExecutor.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/LexerActionExecutor.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/PredictionMode.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/PredictionMode.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATNState.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATNState.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/atn/ATNConfig.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/atn/ATNConfig.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/StdinStream.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/StdinStream.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/TokenStreamRewriter.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/TokenStreamRewriter.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/error/ErrorListener.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/error/ErrorListener.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/error/ErrorStrategy.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/error/ErrorStrategy.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/error/Errors.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/error/Errors.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/error/DiagnosticErrorListener.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/error/DiagnosticErrorListener.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4/CommonTokenStream.py` & `antlr4-python2-runtime-4.9.3/src/antlr4/CommonTokenStream.py`

 * *Files identical despite different names*

### Comparing `antlr4-python2-runtime-4.9.2/src/antlr4_python2_runtime.egg-info/SOURCES.txt` & `antlr4-python2-runtime-4.9.3/src/antlr4_python2_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

