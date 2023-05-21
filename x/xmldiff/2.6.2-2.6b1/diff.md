# Comparing `tmp/xmldiff-2.6.2.tar.gz` & `tmp/xmldiff-2.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmldiff-2.6.2.tar", last modified: Sun May 21 11:02:02 2023, max compression
+gzip compressed data, was "xmldiff-2.6b1.tar", last modified: Thu Jan 12 08:50:49 2023, max compression
```

## Comparing `xmldiff-2.6.2.tar` & `xmldiff-2.6b1.tar`

### file list

```diff
@@ -1,77 +1,74 @@
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-21 11:02:02.283315 xmldiff-2.6.2/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       74 2023-05-21 11:02:01.000000 xmldiff-2.6.2/.coveragerc
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       46 2023-05-21 11:02:01.000000 xmldiff-2.6.2/.coveralls.yml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      566 2023-05-21 11:02:01.000000 xmldiff-2.6.2/.travis.yml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3345 2023-05-21 11:02:01.000000 xmldiff-2.6.2/CHANGES.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1064 2023-05-21 11:02:01.000000 xmldiff-2.6.2/LICENSE.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      409 2023-05-21 11:02:01.000000 xmldiff-2.6.2/MANIFEST.in
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1058 2023-05-21 11:02:01.000000 xmldiff-2.6.2/Makefile
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7817 2023-05-21 11:02:02.283315 xmldiff-2.6.2/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3333 2023-05-21 11:02:01.000000 xmldiff-2.6.2/README.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      143 2023-05-21 11:02:01.000000 xmldiff-2.6.2/README.txt
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-21 11:02:02.279315 xmldiff-2.6.2/docs/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7669 2023-05-21 11:02:01.000000 xmldiff-2.6.2/docs/Makefile
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7260 2023-05-21 11:02:01.000000 xmldiff-2.6.2/docs/make.bat
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-05-21 11:02:01.000000 xmldiff-2.6.2/docs/requirements.txt
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-21 11:02:02.279315 xmldiff-2.6.2/docs/source/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     8783 2023-05-21 11:02:01.000000 xmldiff-2.6.2/docs/source/advanced.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    18116 2023-05-21 11:02:01.000000 xmldiff-2.6.2/docs/source/api.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3239 2023-05-21 11:02:01.000000 xmldiff-2.6.2/docs/source/commandline.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9337 2023-05-21 11:02:01.000000 xmldiff-2.6.2/docs/source/conf.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4207 2023-05-21 11:02:01.000000 xmldiff-2.6.2/docs/source/contributing.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      842 2023-05-21 11:02:01.000000 xmldiff-2.6.2/docs/source/index.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      796 2023-05-21 11:02:01.000000 xmldiff-2.6.2/docs/source/installation.rst
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-21 11:02:02.279315 xmldiff-2.6.2/docs/source/static/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4647 2023-05-21 11:02:01.000000 xmldiff-2.6.2/docs/source/static/htmlformatter.xslt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1610 2023-05-21 11:02:02.283315 xmldiff-2.6.2/setup.cfg
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-05-21 11:02:01.000000 xmldiff-2.6.2/setup.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-21 11:02:02.279315 xmldiff-2.6.2/tests/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       55 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/__init__.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-21 11:02:02.283315 xmldiff-2.6.2/tests/test_data/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      881 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/all_actions.expected.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      430 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/all_actions.left.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      413 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/all_actions.right.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      134 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/bom_1.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      134 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/bom_2.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      695 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/complex-text-update.expected.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      333 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/complex-text-update.left.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      407 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/complex-text-update.right.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      367 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/example.expected.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      145 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/example.left.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      158 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/example.right.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      156 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/insert-node.diff
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      125 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/insert-node.expected.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       40 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/insert-node.left.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       63 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/insert-node.right.html
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      273 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/namespace.expected.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      119 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/namespace.left.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      102 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/namespace.right.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    18828 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/rmldoc.expected.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    17427 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/rmldoc.left.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    17910 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/rmldoc.right.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1482 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/sbt_template.expected.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      939 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/sbt_template.left.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1229 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_data/sbt_template.right.xml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    57557 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_diff.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    21871 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_formatting.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6712 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_main.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7664 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_patch.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4972 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/test_utils.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1730 2023-05-21 11:02:01.000000 xmldiff-2.6.2/tests/testing.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-21 11:02:02.279315 xmldiff-2.6.2/xmldiff/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        0 2023-05-21 11:02:01.000000 xmldiff-2.6.2/xmldiff/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      844 2023-05-21 11:02:01.000000 xmldiff-2.6.2/xmldiff/actions.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    20155 2023-05-21 11:02:02.000000 xmldiff-2.6.2/xmldiff/diff.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    80394 2023-05-21 11:02:02.000000 xmldiff-2.6.2/xmldiff/diff_match_patch.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    31093 2023-05-21 11:02:02.000000 xmldiff-2.6.2/xmldiff/formatting.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7636 2023-05-21 11:02:02.000000 xmldiff-2.6.2/xmldiff/main.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5751 2023-05-21 11:02:02.000000 xmldiff-2.6.2/xmldiff/patch.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4281 2023-05-21 11:02:02.000000 xmldiff-2.6.2/xmldiff/utils.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-21 11:02:02.283315 xmldiff-2.6.2/xmldiff.egg-info/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7817 2023-05-21 11:02:02.000000 xmldiff-2.6.2/xmldiff.egg-info/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1808 2023-05-21 11:02:02.000000 xmldiff-2.6.2/xmldiff.egg-info/SOURCES.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-05-21 11:02:02.000000 xmldiff-2.6.2/xmldiff.egg-info/dependency_links.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       93 2023-05-21 11:02:02.000000 xmldiff-2.6.2/xmldiff.egg-info/entry_points.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       82 2023-05-21 11:02:02.000000 xmldiff-2.6.2/xmldiff.egg-info/requires.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        8 2023-05-21 11:02:02.000000 xmldiff-2.6.2/xmldiff.egg-info/top_level.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-05-21 11:02:02.000000 xmldiff-2.6.2/xmldiff.egg-info/zip-safe
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.532935 xmldiff-2.6b1/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       74 2023-01-12 08:50:49.000000 xmldiff-2.6b1/.coveragerc
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       46 2023-01-12 08:50:49.000000 xmldiff-2.6b1/.coveralls.yml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      566 2023-01-12 08:50:49.000000 xmldiff-2.6b1/.travis.yml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2751 2023-01-12 08:50:49.000000 xmldiff-2.6b1/CHANGES.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1064 2023-01-12 08:50:49.000000 xmldiff-2.6b1/LICENSE.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      409 2023-01-12 08:50:49.000000 xmldiff-2.6b1/MANIFEST.in
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1058 2023-01-12 08:50:49.000000 xmldiff-2.6b1/Makefile
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7203 2023-01-12 08:50:49.532935 xmldiff-2.6b1/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3333 2023-01-12 08:50:49.000000 xmldiff-2.6b1/README.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      143 2023-01-12 08:50:49.000000 xmldiff-2.6b1/README.txt
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.528935 xmldiff-2.6b1/docs/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7669 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/Makefile
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7260 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/make.bat
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/requirements.txt
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.528935 xmldiff-2.6b1/docs/source/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     8636 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/advanced.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    17152 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/api.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3239 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/commandline.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9332 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/conf.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4207 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/contributing.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      842 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/index.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      796 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/installation.rst
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.528935 xmldiff-2.6b1/docs/source/static/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4647 2023-01-12 08:50:49.000000 xmldiff-2.6b1/docs/source/static/htmlformatter.xslt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1610 2023-01-12 08:50:49.532935 xmldiff-2.6b1/setup.cfg
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-01-12 08:50:49.000000 xmldiff-2.6b1/setup.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.532935 xmldiff-2.6b1/tests/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       55 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.532935 xmldiff-2.6b1/tests/test_data/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      736 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/all_actions.expected.xml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      323 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/all_actions.left.xml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      305 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/all_actions.right.xml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      134 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/bom_1.xml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      134 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/bom_2.xml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      695 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/complex-text-update.expected.html
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      333 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/complex-text-update.left.html
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      407 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/complex-text-update.right.html
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      367 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/example.expected.html
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      145 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/example.left.html
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      158 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/example.right.html
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      156 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/insert-node.diff
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      125 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/insert-node.expected.html
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       40 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/insert-node.left.html
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       63 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/insert-node.right.html
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    18828 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/rmldoc.expected.xml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    17427 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/rmldoc.left.xml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    17910 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/rmldoc.right.xml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1482 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/sbt_template.expected.xml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      939 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/sbt_template.left.xml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1229 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_data/sbt_template.right.xml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    57557 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_diff.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    21656 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_formatting.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     6712 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_main.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7664 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_patch.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4972 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/test_utils.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1730 2023-01-12 08:50:49.000000 xmldiff-2.6b1/tests/testing.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.528935 xmldiff-2.6b1/xmldiff/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      723 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/actions.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    19328 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/diff.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    80394 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/diff_match_patch.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    30028 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/formatting.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7230 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/main.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5172 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/patch.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4116 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff/utils.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-01-12 08:50:49.532935 xmldiff-2.6b1/xmldiff.egg-info/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7203 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1698 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       92 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/entry_points.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       82 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/requires.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        8 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/top_level.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-01-12 08:50:49.000000 xmldiff-2.6b1/xmldiff.egg-info/zip-safe
```

### Comparing `xmldiff-2.6.2/.travis.yml` & `xmldiff-2.6b1/.travis.yml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/CHANGES.rst` & `xmldiff-2.6b1/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,13 @@
 Changes
 =======
 
-2.6.2 (2023-05-21)
-------------------
-
-- Solved an error in the xmlformatter when using default namespaces. #89, #113
-
-
-2.6.1 (2023-04-05)
-------------------
-
-- #108: Fixed an error that happens if using namespaces like ns0 or ns1.
-
-
-2.6 (2023-04-03)
-----------------
-
-- Added `InsertNamespace` and `DeleteNamespace` actions for better handling
-  of changing namespaces. Should improve any "Unknown namespace prefix"
-  errors. Changing the URI of a a namespace prefix is not supported, and will
-  raise an error.
-
 2.6b1 (2023-01-12)
 ------------------
 
-- Used geometric mean for the node_ratio, for better handling of simple nodes.
-
 - Added an experimental --best-match method that is slower, but generate
   smaller diffs when you have many nodes that are similar.
 
 - The -F argument now also affects the --fast-match stage.
 
 
 2.5 (2023-01-11)
```

### Comparing `xmldiff-2.6.2/LICENSE.txt` & `xmldiff-2.6b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/Makefile` & `xmldiff-2.6b1/Makefile`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/PKG-INFO` & `xmldiff-2.6b1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: xmldiff
-Version: 2.6.2
+Version: 2.6b1
 Summary: Creates diffs of XML files
 Home-page: https://github.com/Shoobx/xmldiff
 Author: Lennart Regebro
 Author-email: lregebro@shoobx.com
 License: MIT
 Project-URL: Source Code, https://github.com/Shoobx/xmldiff
 Keywords: xml,html,diff
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -120,39 +119,17 @@
 
 The diff algorithm is based on "`Change Detection in Hierarchically Structured Information <http://ilpubs.stanford.edu/115/1/1995-46.pdf>`_",
 and the text diff is using Google's ``diff_match_patch`` algorithm.
 
 Changes
 =======
 
-2.6.2 (2023-05-21)
-------------------
-
-- Solved an error in the xmlformatter when using default namespaces. #89, #113
-
-
-2.6.1 (2023-04-05)
-------------------
-
-- #108: Fixed an error that happens if using namespaces like ns0 or ns1.
-
-
-2.6 (2023-04-03)
-----------------
-
-- Added `InsertNamespace` and `DeleteNamespace` actions for better handling
-  of changing namespaces. Should improve any "Unknown namespace prefix"
-  errors. Changing the URI of a a namespace prefix is not supported, and will
-  raise an error.
-
 2.6b1 (2023-01-12)
 ------------------
 
-- Used geometric mean for the node_ratio, for better handling of simple nodes.
-
 - Added an experimental --best-match method that is slower, but generate
   smaller diffs when you have many nodes that are similar.
 
 - The -F argument now also affects the --fast-match stage.
 
 
 2.5 (2023-01-11)
@@ -244,9 +221,7 @@
 
   - A format intended to be parseable by anyone parsing the old format.
 
   - XML with changes marked though tags and attributes
 
 - xmldiff 2.0 is significantly slower than xmldiff 0.6 or 1.0,
   the emphasis so far is on correctness, not speed.
-
-
```

### Comparing `xmldiff-2.6.2/README.rst` & `xmldiff-2.6b1/README.rst`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/docs/Makefile` & `xmldiff-2.6b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/docs/make.bat` & `xmldiff-2.6b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/docs/source/advanced.rst` & `xmldiff-2.6b1/docs/source/advanced.rst`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,19 @@
 the output can in some cases be less than useful,
 especially in the case where formatting is added:
 
 .. doctest::
   :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
 
   >>> left = '<body><p>My Fine Content</p></body>'
-  >>> right = '<body><p><b>My <i>Fine</i> Content</b></p></body>'
+  >>> right = '<body><p>My <i>Fine</i> Content</p></body>'
   >>> result = main.diff_texts(left, right, formatter=formatter)
   >>> print(result)
   <body xmlns:diff="http://namespaces.shoobx.com/diff">
-    <p diff:insert="">
-      <b diff:insert="" diff:rename="p">My <i diff:insert="">Fine</i><diff:insert> Content</diff:insert></b>
-    </p>
+    <p diff:insert="">My <i diff:insert="">Fine</i><diff:insert> Content</diff:insert></p>
     <p diff:delete="">My Fine Content</p>
   </body>
   <BLANKLINE>
 
 Notice how the the whole text was inserted with formatting,
 and the whole unformatted text was deleted.
 The XMLFormatter supports a better handling of text with the ``text_tags`` and ``formatting_tags`` parameters. Here is a simple and incomplete example with some common HTML tags:
@@ -64,17 +62,15 @@
   >>> formatter=formatting.XMLFormatter(
   ...     text_tags=('p', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'li'),
   ...     formatting_tags=('b', 'u', 'i', 'strike', 'em', 'super',
   ...                      'sup', 'sub', 'link', 'a', 'span'))
   >>> result = main.diff_texts(left, right, formatter=formatter)
   >>> print(result)
   <body xmlns:diff="http://namespaces.shoobx.com/diff">
-    <p>
-      <b diff:insert-formatting="">My <i diff:insert-formatting="">Fine</i> Content</b>
-    </p>
+    <p>My <i diff:insert-formatting="">Fine</i> Content</p>
   </body>
 
 This gives a result that flags the ``<i>`` tag as new formatting.
 This more compact output is much more useful and easier to transform into a visual output.
 
 
 Making a Visual Diff
@@ -134,17 +130,15 @@
   >>> formatter = HTMLFormatter(
   ...     text_tags=('p', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'li'),
   ...     formatting_tags=('b', 'u', 'i', 'strike', 'em', 'super',
   ...                      'sup', 'sub', 'link', 'a', 'span'))
   >>> result = main.diff_texts(left, right, formatter=formatter)
   >>> print(result)
   <body xmlns:diff="http://namespaces.shoobx.com/diff">
-    <p>
-      <b class="insert-formatting">My <i class="insert-formatting">Fine</i> Content</b>
-    </p>
+    <p>My <i class="insert-formatting">Fine</i> Content</p>
   </body>
 
 You can then add into your CSS files classes that make inserted text green,
 deleted text red with an overstrike,
 and formatting changes could for example be blue.
 This makes it easy to see what has been changed in a HTML document.
```

### Comparing `xmldiff-2.6.2/docs/source/api.rst` & `xmldiff-2.6b1/docs/source/api.rst`

 * *Files 3% similar despite different names*

```diff
@@ -444,50 +444,14 @@
 
   >>> left = '<document><node>Content</node></document>'
   >>> right = '<document><!-- A comment --><node>Content</node></document>'
   >>> main.diff_texts(left, right)
   [InsertComment(target='/document[1]', position=0, text=' A comment ')]
 
 
-``InsertNamespace(prefix, uri)``
-................................
-
-Adds a new namespace to the XML document. You need to have this before
-adding a node that uses a namespace that is not in the original XML tree.
-
-Example:
-
-.. doctest::
-  :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-  >>> left = '<document></document>'
-  >>> right = '<document xmlns:new="http://theuri"></document>'
-  >>> main.diff_texts(left, right)
-  [InsertNamespace(prefix='new', uri='http://theuri')]
-
-
-``DeleteNamespace(prefix)``
-................................
-
-Removes a namespace from the XML document. You don't need to handle this,
-strictly speaking, nothing will break if there is an unused namespace,
-but `xmldiff` will return this action.
-
-Example:
-
-.. doctest::
-  :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
-
-  >>> left = '<document xmlns:new="http://theuri"></document>'
-  >>> right = '<document></document>'
-  >>> main.diff_texts(left, right)
-  [DeleteNamespace(prefix='new')]
-
-
-
 The patching API
 ----------------
 
 There is also an API to patch files using the diff output:
 
 .. doctest::
   :options: -ELLIPSIS, +NORMALIZE_WHITESPACE
```

### Comparing `xmldiff-2.6.2/docs/source/commandline.rst` & `xmldiff-2.6b1/docs/source/commandline.rst`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/docs/source/conf.py` & `xmldiff-2.6b1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.doctest",
     "sphinx.ext.coverage",
-    #    "sphinxarg.ext",
+    "sphinxarg.ext",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
@@ -62,15 +62,15 @@
 # release = u'2.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command-line for these cases.
-language = "en"
+language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
```

### Comparing `xmldiff-2.6.2/docs/source/contributing.rst` & `xmldiff-2.6b1/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/docs/source/index.rst` & `xmldiff-2.6b1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/docs/source/installation.rst` & `xmldiff-2.6b1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/docs/source/static/htmlformatter.xslt` & `xmldiff-2.6b1/docs/source/static/htmlformatter.xslt`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/setup.cfg` & `xmldiff-2.6b1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xmldiff
-version = 2.6.2
+version = 2.6b1
 description = Creates diffs of XML files
 long_description = file: README.rst, CHANGES.rst
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Intended Audience :: End Users/Desktop
 	Topic :: Text Processing :: Markup :: XML
```

### Comparing `xmldiff-2.6.2/tests/test_data/complex-text-update.expected.html` & `xmldiff-2.6b1/tests/test_data/complex-text-update.expected.html`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/tests/test_data/rmldoc.expected.xml` & `xmldiff-2.6b1/tests/test_data/rmldoc.expected.xml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/tests/test_data/rmldoc.left.xml` & `xmldiff-2.6b1/tests/test_data/rmldoc.left.xml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/tests/test_data/rmldoc.right.xml` & `xmldiff-2.6b1/tests/test_data/rmldoc.right.xml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/tests/test_data/sbt_template.expected.xml` & `xmldiff-2.6b1/tests/test_data/sbt_template.expected.xml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/tests/test_data/sbt_template.left.xml` & `xmldiff-2.6b1/tests/test_data/sbt_template.left.xml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/tests/test_data/sbt_template.right.xml` & `xmldiff-2.6b1/tests/test_data/sbt_template.right.xml`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/tests/test_diff.py` & `xmldiff-2.6b1/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/tests/test_formatting.py` & `xmldiff-2.6b1/tests/test_formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,16 +484,14 @@
         here = os.path.split(__file__)[0]
         lfile = os.path.join(here, "test_data", "all_actions.left.xml")
         rfile = os.path.join(here, "test_data", "all_actions.right.xml")
 
         formatter = formatting.XmlDiffFormatter()
         result = main.diff_files(lfile, rfile, formatter=formatter)
         expected = (
-            "[insert-namespace, space, http://namespaces.shoobx.com/outerspace]\n"
-            "[delete-namespace, name]\n"
             "[move-after, /document/node[2], /document/tag[1]]\n"
             "[insert-comment, /document[1], 0,  Insert a new comment ]\n"
             '[update, /document/node[1]/@name, "was updated"]\n'
             "[remove, /document/node[1]/@attribute]\n"
             "[insert, /document/node[1], \n"
             "<@newtribute>\n"
             "renamed\n"
@@ -503,16 +501,16 @@
             "is new\n"
             "</@this>]\n"
             "[remove, /document/node[1]/@attr]\n"
             '[update, /document/node[1]/text()[1], "\\n    Modified\\n  "]\n'
             '[update, /document/node[1]/text()[2], "\\n    '
             'New tail content\\n  "]\n'
             "[rename, /document/node[2], nod]\n"
-            "[rename, /document/name:space[1], {http://namespaces.shoobx.com/outerspace}name]\n"
-            '[update, /document/space:name[1]/text()[2], "\\n  "]\n'
+            "[insert-after, /document/tail[1], \n"
+            "<new/>]\n"
             "[remove, /document/tail[1]]"
         )
         self.assertEqual(result, expected)
 
 
 class FormatterFileTests(unittest.TestCase):
```

### Comparing `xmldiff-2.6.2/tests/test_main.py` & `xmldiff-2.6b1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/tests/test_patch.py` & `xmldiff-2.6b1/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/tests/test_utils.py` & `xmldiff-2.6b1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/tests/testing.py` & `xmldiff-2.6b1/tests/testing.py`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/xmldiff/actions.py` & `xmldiff-2.6b1/xmldiff/actions.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,10 +11,7 @@
 
 UpdateAttrib = namedtuple("UpdateAttrib", "node name value")
 DeleteAttrib = namedtuple("DeleteAttrib", "node name")
 InsertAttrib = namedtuple("InsertAttrib", "node name value")
 RenameAttrib = namedtuple("RenameAttrib", "node oldname newname")
 
 InsertComment = namedtuple("InsertComment", "target position text")
-
-InsertNamespace = namedtuple("InsertNamespace", "prefix uri")
-DeleteNamespace = namedtuple("DeleteNamespace", "prefix")
```

### Comparing `xmldiff-2.6.2/xmldiff/diff.py` & `xmldiff-2.6b1/xmldiff/diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -422,35 +422,14 @@
             self._inorder.add(rchild)
 
     def diff(self, left=None, right=None):
         # Make sure the matching is done first, diff() needs the l2r/r2l maps.
         if not self._matches:
             self.match(left, right)
 
-        # First, deal with namespaces:
-        rnsmap = self.right.nsmap
-        lnsmap = self.left.nsmap
-        for k, v in rnsmap.items():
-            # Make sure it's registered:
-            if k is not None and not utils.RESERVED_NS.match(k):
-                etree.register_namespace(k, v)
-            if k not in lnsmap:
-                yield actions.InsertNamespace(k, v)
-            elif lnsmap[k] != v:
-                raise RuntimeError(
-                    "Sorry, we do not support changing the URI of namespaces in xmldiff"
-                )
-
-        for k, v in lnsmap.items():
-            # Make sure it's registered:
-            if k is not None and not utils.RESERVED_NS.match(k):
-                etree.register_namespace(k, v)
-            if k not in rnsmap:
-                yield actions.DeleteNamespace(k)
-
         # The paper talks about the five phases, and then does four of them
         # in one phase, in a different order that described. This
         # implementation in turn differs in order yet again.
         ltree = self.left.getroottree()
 
         for rnode in utils.breadth_first_traverse(self.right):
             # (a)
```

### Comparing `xmldiff-2.6.2/xmldiff/diff_match_patch.py` & `xmldiff-2.6b1/xmldiff/diff_match_patch.py`

 * *Files identical despite different names*

### Comparing `xmldiff-2.6.2/xmldiff/formatting.py` & `xmldiff-2.6b1/xmldiff/formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,23 +331,22 @@
         # and also because we don't want to modify the original tree.
         result = deepcopy(orig_tree)
         if isinstance(result, etree._ElementTree):
             root = result.getroot()
         else:
             root = result
 
-        self._nsmap = [(DIFF_PREFIX, DIFF_NS)]
         etree.register_namespace(DIFF_PREFIX, DIFF_NS)
 
         for action in diff:
             self.handle_action(action, root)
 
         self.finalize(root)
 
-        etree.cleanup_namespaces(result, top_nsmap=dict(self._nsmap))
+        etree.cleanup_namespaces(result, top_nsmap={DIFF_PREFIX: DIFF_NS})
         return self.render(result)
 
     def render(self, result):
         return etree.tounicode(result, pretty_print=self.pretty_print)
 
     def handle_action(self, action, result):
         action_type = type(action)
@@ -366,19 +365,14 @@
             parent.remove(element)
 
     def _xpath(self, node, xpath):
         # This method finds an element with xpath and makes sure that
         # one and exactly one element is found. This is to protect against
         # formatting a diff on the wrong tree, or against using ambiguous
         # edit script xpaths.
-
-        # First, make a namespace map that uses the left tree's URI's:
-        nsmap = dict(self._nsmap)
-        nsmap.update(node.nsmap)
-
         if xpath[0] == "/":
             root = True
             xpath = xpath[1:]
         else:
             root = False
 
         if "/" in xpath:
@@ -395,20 +389,19 @@
             index = 0
             multiple = True
 
         if root:
             path = "/" + path
 
         matches = []
-        if None in nsmap:
-            del nsmap[None]
-        for match in node.xpath(path, namespaces=nsmap):
+        for match in node.xpath(path, namespaces=node.nsmap):
             # Skip nodes that have been deleted
             if DELETE_NAME not in match.attrib:
                 matches.append(match)
+
         if index >= len(matches):
             raise ValueError(
                 "xpath {}[{}] not found at {}.".format(
                     path, index + 1, utils.getpath(node)
                 )
             )
         if len(matches) > 1 and multiple:
@@ -635,22 +628,14 @@
         right_value = action.text
         node.tail = None
 
         self._make_diff_tags(left_value, right_value, node, node.getparent())
 
         return node
 
-    def _handle_InsertNamespace(self, action, tree):
-        # There is no way to mark this so it's visible, so we'll just update the tree
-        self._nsmap.append((action.prefix, action.uri))
-
-    def _handle_DeleteNamespace(self, action, tree):
-        # This will be handled by the namespace cleanup
-        pass
-
     # There is no InsertComment handler, as this formatter removes all comments
 
 
 class DiffFormatter(BaseFormatter):
     def __init__(self, normalize=WS_TAGS, pretty_print=False):
         self.normalize = normalize
         # No pretty print support, nothing to be pretty about
@@ -713,27 +698,14 @@
         return (
             "insert-comment",
             action.target,
             str(action.position),
             json.dumps(action.text),
         )
 
-    def _handle_InsertNamespace(self, action):
-        return (
-            "insert-namespace",
-            action.prefix,
-            action.uri,
-        )
-
-    def _handle_DeleteNamespace(self, action):
-        return (
-            "delete-namespace",
-            action.prefix,
-        )
-
 
 class XmlDiffFormatter(BaseFormatter):
     """A formatter for an output trying to be xmldiff 0.6 compatible"""
 
     def __init__(self, normalize=WS_TAGS, pretty_print=False):
         self.normalize = normalize
         # No pretty print support, nothing to be pretty about
@@ -816,14 +788,8 @@
     def _handle_UpdateTextAfter(self, action, orig_tree):
         yield "update", action.node + "/text()[2]", json.dumps(action.text)
 
     def _handle_RenameNode(self, action, orig_tree):
         yield "rename", action.node, action.tag
 
     def _handle_InsertComment(self, action, orig_tree):
-        yield "insert-comment", action.target, str(action.position), action.text
-
-    def _handle_InsertNamespace(self, action, orig_tree):
-        yield "insert-namespace", action.prefix, action.uri
-
-    def _handle_DeleteNamespace(self, action, orig_tree):
-        yield "delete-namespace", action.prefix
+        yield ("insert-comment", action.target, str(action.position), action.text)
```

### Comparing `xmldiff-2.6.2/xmldiff/main.py` & `xmldiff-2.6b1/xmldiff/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """All major API points and command-line tools"""
 import pkg_resources
 
-from argparse import ArgumentParser, ArgumentTypeError
+from argparse import ArgumentParser
 from lxml import etree
 from xmldiff import diff, formatting, patch
 
 __version__ = pkg_resources.require("xmldiff")[0].version
 
 FORMATTERS = {
     "diff": formatting.DiffFormatter,
@@ -49,27 +49,14 @@
 def diff_files(left, right, diff_options=None, formatter=None):
     """Takes two filenames or streams, and diffs the XML in those files"""
     return _diff(
         etree.parse, left, right, diff_options=diff_options, formatter=formatter
     )
 
 
-def validate_F(arg):
-    """Type function for argparse - a float within some predefined bounds"""
-    try:
-        F = float(arg)
-    except ValueError:
-        raise ArgumentTypeError("Must be a floating point number")
-    if F <= 0:
-        raise ArgumentTypeError("F can not be zero or lower")
-    if F > 1:
-        raise ArgumentTypeError("F can not be above 1")
-    return F
-
-
 def make_diff_parser():
     parser = ArgumentParser(
         description="Create a diff for two XML files.", add_help=False
     )
     parser.add_argument("file1", type=str, help="The first input file.")
     parser.add_argument("file2", type=str, help="The second input file.")
     parser.add_argument(
@@ -104,15 +91,15 @@
         "-p",
         "--pretty-print",
         action="store_true",
         help="Try to make XML output more readable.",
     )
     parser.add_argument(
         "-F",
-        type=validate_F,
+        type=float,
         help="A value between 0 and 1 that determines how "
         "similar nodes must be to match.",
     )
     parser.add_argument(
         "--unique-attributes",
         type=str,
         nargs="?",
```

### Comparing `xmldiff-2.6.2/xmldiff/patch.py` & `xmldiff-2.6b1/xmldiff/patch.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,95 +2,81 @@
 from csv import reader
 from json import loads
 from lxml import etree
 from xmldiff import actions
 
 
 class Patcher:
-    @property
-    def nsmap(self):
-        return getattr(self, "_nsmap", {})
-
     def patch(self, actions, tree):
         if isinstance(tree, etree._ElementTree):
             tree = tree.getroot()
 
-        # Save the namespace:
-        self._nsmap = tree.nsmap
-
         # Copy the tree so we don't modify the original
         result = deepcopy(tree)
 
         for action in actions:
             self.handle_action(action, result)
 
         return result
 
     def handle_action(self, action, tree):
         action_type = type(action)
         method = getattr(self, "_handle_" + action_type.__name__)
         method(action, tree)
 
     def _handle_DeleteNode(self, action, tree):
-        node = tree.xpath(action.node, namespaces=self.nsmap)[0]
+        node = tree.xpath(action.node, namespaces=tree.nsmap)[0]
         node.getparent().remove(node)
 
     def _handle_InsertNode(self, action, tree):
-        target = tree.xpath(action.target, namespaces=self.nsmap)[0]
+        target = tree.xpath(action.target, namespaces=tree.nsmap)[0]
         node = target.makeelement(action.tag)
         target.insert(action.position, node)
 
     def _handle_RenameNode(self, action, tree):
-        tree.xpath(action.node, namespaces=self.nsmap)[0].tag = action.tag
+        tree.xpath(action.node, namespaces=tree.nsmap)[0].tag = action.tag
 
     def _handle_MoveNode(self, action, tree):
-        node = tree.xpath(action.node, namespaces=self.nsmap)[0]
+        node = tree.xpath(action.node, namespaces=tree.nsmap)[0]
         node.getparent().remove(node)
         target = tree.xpath(action.target)[0]
         target.insert(action.position, node)
 
     def _handle_UpdateTextIn(self, action, tree):
-        tree.xpath(action.node, namespaces=self.nsmap)[0].text = action.text
+        tree.xpath(action.node, namespaces=tree.nsmap)[0].text = action.text
 
     def _handle_UpdateTextAfter(self, action, tree):
-        tree.xpath(action.node, namespaces=self.nsmap)[0].tail = action.text
+        tree.xpath(action.node, namespaces=tree.nsmap)[0].tail = action.text
 
     def _handle_UpdateAttrib(self, action, tree):
-        node = tree.xpath(action.node, namespaces=self.nsmap)[0]
+        node = tree.xpath(action.node, namespaces=tree.nsmap)[0]
         # This should not be used to insert new attributes.
         assert action.name in node.attrib
         node.attrib[action.name] = action.value
 
     def _handle_DeleteAttrib(self, action, tree):
-        del tree.xpath(action.node, namespaces=self.nsmap)[0].attrib[action.name]
+        del tree.xpath(action.node, namespaces=tree.nsmap)[0].attrib[action.name]
 
     def _handle_InsertAttrib(self, action, tree):
-        node = tree.xpath(action.node, namespaces=self.nsmap)[0]
+        node = tree.xpath(action.node, namespaces=tree.nsmap)[0]
         # This should not be used to update existing attributes.
         assert action.name not in node.attrib
         node.attrib[action.name] = action.value
 
     def _handle_RenameAttrib(self, action, tree):
-        node = tree.xpath(action.node, namespaces=self.nsmap)[0]
+        node = tree.xpath(action.node, namespaces=tree.nsmap)[0]
         assert action.oldname in node.attrib
         assert action.newname not in node.attrib
         node.attrib[action.newname] = node.attrib[action.oldname]
         del node.attrib[action.oldname]
 
     def _handle_InsertComment(self, action, tree):
         target = tree.xpath(action.target)[0]
         target.insert(action.position, etree.Comment(action.text))
 
-    def _handle_InsertNamespace(self, action, tree):
-        self.nsmap[action.prefix] = action.uri
-
-    def _handle_DeleteNamespace(self, action, tree):
-        # Nothing needs to be done, it will be handled by cleanup
-        pass
-
 
 class DiffParser:
     """Makes a text diff into a list of actions"""
 
     def parse(self, diff):
         incomplete = ""
 
@@ -152,13 +138,7 @@
         return actions.InsertAttrib(node, name, loads(value))
 
     def _handle_rename_attribute(self, node, oldname, newname):
         return actions.RenameAttrib(node, oldname, newname)
 
     def _handle_insert_comment(self, target, position, text):
         return actions.InsertComment(target, int(position), loads(text))
-
-    def _handle_insert_namespace(self, prefix, uri):
-        return actions.InsertNamespace(prefix, uri)
-
-    def _handle_delete_namespace(self, prefix):
-        return actions.DeleteNamespace(prefix)
```

### Comparing `xmldiff-2.6.2/xmldiff/utils.py` & `xmldiff-2.6b1/xmldiff/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import re
 
 from operator import eq
 
-# This namespace is reserved for lxml internal use, which only
-# means we get an error if we try registering it:
-RESERVED_NS = re.compile(r"ns\d+", flags=re.ASCII)
-
 
 def post_order_traverse(node):
     for child in node.getchildren():
         # PY3: Man, I want yield from!
         yield from post_order_traverse(child)
     yield node
```

### Comparing `xmldiff-2.6.2/xmldiff.egg-info/PKG-INFO` & `xmldiff-2.6b1/xmldiff.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: xmldiff
-Version: 2.6.2
+Version: 2.6b1
 Summary: Creates diffs of XML files
 Home-page: https://github.com/Shoobx/xmldiff
 Author: Lennart Regebro
 Author-email: lregebro@shoobx.com
 License: MIT
 Project-URL: Source Code, https://github.com/Shoobx/xmldiff
 Keywords: xml,html,diff
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -120,39 +119,17 @@
 
 The diff algorithm is based on "`Change Detection in Hierarchically Structured Information <http://ilpubs.stanford.edu/115/1/1995-46.pdf>`_",
 and the text diff is using Google's ``diff_match_patch`` algorithm.
 
 Changes
 =======
 
-2.6.2 (2023-05-21)
-------------------
-
-- Solved an error in the xmlformatter when using default namespaces. #89, #113
-
-
-2.6.1 (2023-04-05)
-------------------
-
-- #108: Fixed an error that happens if using namespaces like ns0 or ns1.
-
-
-2.6 (2023-04-03)
-----------------
-
-- Added `InsertNamespace` and `DeleteNamespace` actions for better handling
-  of changing namespaces. Should improve any "Unknown namespace prefix"
-  errors. Changing the URI of a a namespace prefix is not supported, and will
-  raise an error.
-
 2.6b1 (2023-01-12)
 ------------------
 
-- Used geometric mean for the node_ratio, for better handling of simple nodes.
-
 - Added an experimental --best-match method that is slower, but generate
   smaller diffs when you have many nodes that are similar.
 
 - The -F argument now also affects the --fast-match stage.
 
 
 2.5 (2023-01-11)
@@ -244,9 +221,7 @@
 
   - A format intended to be parseable by anyone parsing the old format.
 
   - XML with changes marked though tags and attributes
 
 - xmldiff 2.0 is significantly slower than xmldiff 0.6 or 1.0,
   the emphasis so far is on correctness, not speed.
-
-
```

### Comparing `xmldiff-2.6.2/xmldiff.egg-info/SOURCES.txt` & `xmldiff-2.6b1/xmldiff.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -46,17 +46,14 @@
 tests/test_data/example.expected.html
 tests/test_data/example.left.html
 tests/test_data/example.right.html
 tests/test_data/insert-node.diff
 tests/test_data/insert-node.expected.html
 tests/test_data/insert-node.left.html
 tests/test_data/insert-node.right.html
-tests/test_data/namespace.expected.xml
-tests/test_data/namespace.left.xml
-tests/test_data/namespace.right.xml
 tests/test_data/rmldoc.expected.xml
 tests/test_data/rmldoc.left.xml
 tests/test_data/rmldoc.right.xml
 tests/test_data/sbt_template.expected.xml
 tests/test_data/sbt_template.left.xml
 tests/test_data/sbt_template.right.xml
 xmldiff.egg-info/PKG-INFO
```

