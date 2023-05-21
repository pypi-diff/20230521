# Comparing `tmp/pretext-1.5.4.dev20230519.tar.gz` & `tmp/pretext-1.5.4.dev20230521.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.5.4.dev20230519.tar", max compression
+gzip compressed data, was "pretext-1.5.4.dev20230521.tar", max compression
```

## Comparing `pretext-1.5.4.dev20230519.tar` & `pretext-1.5.4.dev20230521.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/LICENSE
--rw-r--r--   0        0        0     9664 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/README.md
--rw-r--r--   0        0        0     1440 2023-05-19 06:18:46.027659 pretext-1.5.4.dev20230519/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/__main__.py
--rw-r--r--   0        0        0     7344 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/build.py
--rw-r--r--   0        0        0    22954 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/core/__init__.py
--rw-r--r--   0        0        0   172432 2023-05-19 06:18:51.256048 pretext-1.5.4.dev20230519/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/core/resources.py
--rw-r--r--   0        0        0  1029942 2023-05-19 06:18:51.256048 pretext-1.5.4.dev20230519/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/generate.py
--rw-r--r--   0        0        0    24172 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/project.py
--rw-r--r--   0        0        0      516 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-05-19 06:18:51.336053 pretext-1.5.4.dev20230519/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-05-19 06:18:51.336053 pretext-1.5.4.dev20230519/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160548 2023-05-19 06:18:51.312051 pretext-1.5.4.dev20230519/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     8054 2023-05-19 06:18:51.300051 pretext-1.5.4.dev20230519/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173747 2023-05-19 06:18:51.332053 pretext-1.5.4.dev20230519/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2059 2023-05-19 06:18:51.336053 pretext-1.5.4.dev20230519/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     5095 2023-05-19 06:18:51.316052 pretext-1.5.4.dev20230519/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0      630 2023-05-19 06:18:51.336053 pretext-1.5.4.dev20230519/pretext/templates/resources/postCreateCommand.sh
--rw-r--r--   0        0        0     1710 2023-05-19 06:18:51.336053 pretext-1.5.4.dev20230519/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-05-19 06:18:51.336053 pretext-1.5.4.dev20230519/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8830 2023-05-19 06:18:51.316052 pretext-1.5.4.dev20230519/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18300 2023-05-19 06:17:54.203635 pretext-1.5.4.dev20230519/pretext/utils.py
--rw-r--r--   0        0        0     1119 2023-05-19 06:18:46.027659 pretext-1.5.4.dev20230519/pyproject.toml
--rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.4.dev20230519/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-05-21 06:16:30.929555 pretext-1.5.4.dev20230521/LICENSE
+-rw-r--r--   0        0        0     9664 2023-05-21 06:16:30.929555 pretext-1.5.4.dev20230521/README.md
+-rw-r--r--   0        0        0     1440 2023-05-21 06:17:08.959138 pretext-1.5.4.dev20230521/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-21 06:16:30.929555 pretext-1.5.4.dev20230521/pretext/__main__.py
+-rw-r--r--   0        0        0     7344 2023-05-21 06:16:30.929555 pretext-1.5.4.dev20230521/pretext/build.py
+-rw-r--r--   0        0        0    22954 2023-05-21 06:16:30.929555 pretext-1.5.4.dev20230521/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-05-21 06:16:30.929555 pretext-1.5.4.dev20230521/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-05-21 06:16:30.929555 pretext-1.5.4.dev20230521/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-05-21 06:16:30.929555 pretext-1.5.4.dev20230521/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172432 2023-05-21 06:17:14.503325 pretext-1.5.4.dev20230521/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-05-21 06:16:30.929555 pretext-1.5.4.dev20230521/pretext/core/resources.py
+-rw-r--r--   0        0        0  1030816 2023-05-21 06:17:14.503325 pretext-1.5.4.dev20230521/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-05-21 06:16:30.929555 pretext-1.5.4.dev20230521/pretext/generate.py
+-rw-r--r--   0        0        0    24172 2023-05-21 06:16:30.933555 pretext-1.5.4.dev20230521/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-05-21 06:16:30.933555 pretext-1.5.4.dev20230521/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-05-21 06:17:14.603329 pretext-1.5.4.dev20230521/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-21 06:17:14.603329 pretext-1.5.4.dev20230521/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160064 2023-05-21 06:17:14.567328 pretext-1.5.4.dev20230521/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7570 2023-05-21 06:17:14.555327 pretext-1.5.4.dev20230521/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173263 2023-05-21 06:17:14.599329 pretext-1.5.4.dev20230521/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2059 2023-05-21 06:17:14.603329 pretext-1.5.4.dev20230521/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4611 2023-05-21 06:17:14.571328 pretext-1.5.4.dev20230521/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-05-21 06:17:14.603329 pretext-1.5.4.dev20230521/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-05-21 06:17:14.603329 pretext-1.5.4.dev20230521/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8346 2023-05-21 06:17:14.575328 pretext-1.5.4.dev20230521/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18300 2023-05-21 06:16:30.933555 pretext-1.5.4.dev20230521/pretext/utils.py
+-rw-r--r--   0        0        0     1119 2023-05-21 06:17:08.959138 pretext-1.5.4.dev20230521/pyproject.toml
+-rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.4.dev20230521/PKG-INFO
```

### Comparing `pretext-1.5.4.dev20230519/LICENSE` & `pretext-1.5.4.dev20230521/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/README.md` & `pretext-1.5.4.dev20230521/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pretext/__init__.py` & `pretext-1.5.4.dev20230521/pretext/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
 
-CORE_COMMIT = '393d7a374feeb73971d9eda9cc2232dab7b68f31'
+CORE_COMMIT = 'ac42cd57a6136165d0dd3773a9207287a5e124a7'
 
 
 def activate():
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.5.4.dev20230519/pretext/build.py` & `pretext-1.5.4.dev20230521/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pretext/cli.py` & `pretext-1.5.4.dev20230521/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pretext/codechat.py` & `pretext-1.5.4.dev20230521/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pretext/config/xml_overlay.py` & `pretext-1.5.4.dev20230521/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pretext/core/pretext.py` & `pretext-1.5.4.dev20230521/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pretext/core/resources.py` & `pretext-1.5.4.dev20230521/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pretext/core/resources.zip` & `pretext-1.5.4.dev20230521/pretext/core/resources.zip`

 * *Files 20% similar despite different names*

#### zipinfo {}

```diff
@@ -1,142 +1,142 @@
-Zip file size: 1029942 bytes, number of entries: 140
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-May-19 06:18 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-May-19 06:18 script/mbx
--rw-r--r--  2.0 unx       92 b- defN 23-May-19 06:18 script/mjsre/update-sre
--rw-r--r--  2.0 unx      481 b- defN 23-May-19 06:18 script/mjsre/README.md
--rw-r--r--  2.0 unx      116 b- defN 23-May-19 06:18 script/mjsre/package.json
--rw-r--r--  2.0 unx     9251 b- defN 23-May-19 06:18 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx    18421 b- defN 23-May-19 06:18 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    58086 b- defN 23-May-19 06:18 schema/pretext.rnc
--rw-r--r--  2.0 unx    25290 b- defN 23-May-19 06:18 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx   134043 b- defN 23-May-19 06:18 schema/pretext.xml
--rw-r--r--  2.0 unx     1180 b- defN 23-May-19 06:18 schema/README.md
--rw-r--r--  2.0 unx   125135 b- defN 23-May-19 06:18 schema/pretext.xsd
--rw-r--r--  2.0 unx      326 b- defN 23-May-19 06:18 schema/xml.xsd
--rw-r--r--  2.0 unx    34210 b- defN 23-May-19 06:18 schema/pretext-dev.rng
--rw-r--r--  2.0 unx   101829 b- defN 23-May-19 06:18 schema/pretext.rng
--rw-r--r--  2.0 unx    17587 b- defN 23-May-19 06:18 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx     3135 b- defN 23-May-19 06:18 schema/build.sh
--rw-r--r--  2.0 unx     1367 b- defN 23-May-19 06:18 pretext/README.md
--rw-r--r--  2.0 unx   172432 b- defN 23-May-19 06:18 pretext/pretext.py
--rw-r--r--  2.0 unx     1955 b- defN 23-May-19 06:18 pretext/module-test.py
--rw-r--r--  2.0 unx    30908 b- defN 23-May-19 06:18 pretext/pretext
--rw-r--r--  2.0 unx        0 b- defN 23-May-19 06:18 pretext/__init__.py
--rw-r--r--  2.0 unx    35449 b- defN 23-May-19 06:18 pretext/braille_format.py
--rw-r--r--  2.0 unx     2566 b- defN 23-May-19 06:18 pretext/pretext.cfg
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 xsl/utilities/
--rw-r--r--  2.0 unx     9787 b- defN 23-May-19 06:18 xsl/entities.ent
--rw-r--r--  2.0 unx     3239 b- defN 23-May-19 06:18 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-May-19 06:18 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-May-19 06:18 xsl/README.md
--rw-r--r--  2.0 unx   139486 b- defN 23-May-19 06:18 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-May-19 06:18 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-May-19 06:18 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-May-19 06:18 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-May-19 06:18 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-May-19 06:18 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   261852 b- defN 23-May-19 06:18 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   103788 b- defN 23-May-19 06:18 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-May-19 06:18 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-May-19 06:18 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-May-19 06:18 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   540859 b- defN 23-May-19 06:18 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-May-19 06:18 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-May-19 06:18 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-May-19 06:18 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-May-19 06:18 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-May-19 06:18 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-May-19 06:18 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx   111553 b- defN 23-May-19 06:18 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-May-19 06:18 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-May-19 06:18 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx   544780 b- defN 23-May-19 06:18 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-May-19 06:18 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-May-19 06:18 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-May-19 06:18 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    88250 b- defN 23-May-19 06:18 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-May-19 06:18 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-May-19 06:18 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-May-19 06:18 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx   606187 b- defN 23-May-19 06:18 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-May-19 06:18 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-May-19 06:18 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-May-19 06:18 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-May-19 06:18 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-May-19 06:18 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-May-19 06:18 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-May-19 06:18 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-May-19 06:18 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-May-19 06:18 xsl/latex/pretext-latex-guide.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 23-May-19 06:18 xsl/support/README.md
--rw-r--r--  2.0 unx    10306 b- defN 23-May-19 06:18 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-May-19 06:18 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-May-19 06:18 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-May-19 06:18 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5800 b- defN 23-May-19 06:18 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     5065 b- defN 23-May-19 06:18 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     2657 b- defN 23-May-19 06:18 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx      722 b- defN 23-May-19 06:18 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     6621 b- defN 23-May-19 06:18 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    16518 b- defN 23-May-19 06:18 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-May-19 06:18 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-May-19 06:18 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-May-19 06:18 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-May-19 06:18 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-May-19 06:18 xsl/localizations/README.md
--rw-r--r--  2.0 unx    15938 b- defN 23-May-19 06:18 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-May-19 06:18 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-May-19 06:18 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-May-19 06:18 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-May-19 06:18 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx     2227 b- defN 23-May-19 06:18 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    15736 b- defN 23-May-19 06:18 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-May-19 06:18 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-May-19 06:18 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-May-19 06:18 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-May-19 06:18 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx     1810 b- defN 23-May-19 06:18 xsl/utilities/README.md
--rw-r--r--  2.0 unx    30257 b- defN 23-May-19 06:18 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-May-19 06:18 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-May-19 06:18 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-May-19 06:18 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-May-19 06:18 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     1276 b- defN 23-May-19 06:18 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     7761 b- defN 23-May-19 06:18 css/style_default.css
--rw-r--r--  2.0 unx     3473 b- defN 23-May-19 06:18 css/style_soundwriting.css
--rw-r--r--  2.0 unx    63664 b- defN 23-May-19 06:18 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     1865 b- defN 23-May-19 06:18 css/README.md
--rw-r--r--  2.0 unx     1280 b- defN 23-May-19 06:18 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_blue_red.css
--rw-r--r--  2.0 unx   435680 b- defN 23-May-19 06:18 css/mathbook-3.css
--rw-r--r--  2.0 unx   146685 b- defN 23-May-19 06:18 css/mathbook-content.css
--rw-r--r--  2.0 unx    22438 b- defN 23-May-19 06:18 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     4308 b- defN 23-May-19 06:18 css/colors_blue_green.css
--rw-r--r--  2.0 unx    71198 b- defN 23-May-19 06:18 css/pretext_add_on.css
--rw-r--r--  2.0 unx     2608 b- defN 23-May-19 06:18 css/colors_default.css
--rw-r--r--  2.0 unx     2438 b- defN 23-May-19 06:18 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2446 b- defN 23-May-19 06:18 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_orange_navy.css
--rw-r--r--  2.0 unx    12567 b- defN 23-May-19 06:18 css/style_oscarlevin.css
--rw-r--r--  2.0 unx      691 b- defN 23-May-19 06:18 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     1338 b- defN 23-May-19 06:18 css/colors_red_blue.css
--rw-r--r--  2.0 unx    14069 b- defN 23-May-19 06:18 css/setcolors.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     2446 b- defN 23-May-19 06:18 css/colors_martiansands.css
--rw-r--r--  2.0 unx     1362 b- defN 23-May-19 06:18 css/epub.css
--rw-r--r--  2.0 unx     2441 b- defN 23-May-19 06:18 css/kindle.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-19 06:18 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     4021 b- defN 23-May-19 06:18 css/update_css
-140 files, 4813832 bytes uncompressed, 1012614 bytes compressed:  79.0%
+Zip file size: 1030816 bytes, number of entries: 140
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-May-21 06:17 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-May-21 06:17 script/mbx
+-rw-r--r--  2.0 unx       92 b- defN 23-May-21 06:17 script/mjsre/update-sre
+-rw-r--r--  2.0 unx      481 b- defN 23-May-21 06:17 script/mjsre/README.md
+-rw-r--r--  2.0 unx      116 b- defN 23-May-21 06:17 script/mjsre/package.json
+-rw-r--r--  2.0 unx     9251 b- defN 23-May-21 06:17 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx    18421 b- defN 23-May-21 06:17 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    58086 b- defN 23-May-21 06:17 schema/pretext.rnc
+-rw-r--r--  2.0 unx    25290 b- defN 23-May-21 06:17 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx   134043 b- defN 23-May-21 06:17 schema/pretext.xml
+-rw-r--r--  2.0 unx     1180 b- defN 23-May-21 06:17 schema/README.md
+-rw-r--r--  2.0 unx   125135 b- defN 23-May-21 06:17 schema/pretext.xsd
+-rw-r--r--  2.0 unx      326 b- defN 23-May-21 06:17 schema/xml.xsd
+-rw-r--r--  2.0 unx    34210 b- defN 23-May-21 06:17 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx   101829 b- defN 23-May-21 06:17 schema/pretext.rng
+-rw-r--r--  2.0 unx    17587 b- defN 23-May-21 06:17 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx     3135 b- defN 23-May-21 06:17 schema/build.sh
+-rw-r--r--  2.0 unx     1367 b- defN 23-May-21 06:17 pretext/README.md
+-rw-r--r--  2.0 unx   172432 b- defN 23-May-21 06:17 pretext/pretext.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-May-21 06:17 pretext/module-test.py
+-rw-r--r--  2.0 unx    30908 b- defN 23-May-21 06:17 pretext/pretext
+-rw-r--r--  2.0 unx        0 b- defN 23-May-21 06:17 pretext/__init__.py
+-rw-r--r--  2.0 unx    35449 b- defN 23-May-21 06:17 pretext/braille_format.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-May-21 06:17 pretext/pretext.cfg
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 xsl/utilities/
+-rw-r--r--  2.0 unx     9787 b- defN 23-May-21 06:17 xsl/entities.ent
+-rw-r--r--  2.0 unx     3239 b- defN 23-May-21 06:17 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-May-21 06:17 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-May-21 06:17 xsl/README.md
+-rw-r--r--  2.0 unx   139486 b- defN 23-May-21 06:17 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-May-21 06:17 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-May-21 06:17 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-May-21 06:17 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-May-21 06:17 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-May-21 06:17 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx   262798 b- defN 23-May-21 06:17 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   104457 b- defN 23-May-21 06:17 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-May-21 06:17 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-May-21 06:17 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-May-21 06:17 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   541384 b- defN 23-May-21 06:17 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-May-21 06:17 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-May-21 06:17 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-May-21 06:17 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-May-21 06:17 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-May-21 06:17 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-May-21 06:17 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx   111553 b- defN 23-May-21 06:17 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-May-21 06:17 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-May-21 06:17 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx   544780 b- defN 23-May-21 06:17 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-21 06:17 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-May-21 06:17 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-May-21 06:17 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    89128 b- defN 23-May-21 06:17 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-May-21 06:17 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-May-21 06:17 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-May-21 06:17 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx   606258 b- defN 23-May-21 06:17 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-May-21 06:17 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-May-21 06:17 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-May-21 06:17 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-May-21 06:17 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-May-21 06:17 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-May-21 06:17 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-May-21 06:17 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-May-21 06:17 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-May-21 06:17 xsl/latex/pretext-latex-guide.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 23-May-21 06:17 xsl/support/README.md
+-rw-r--r--  2.0 unx    10306 b- defN 23-May-21 06:17 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-May-21 06:17 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-May-21 06:17 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-May-21 06:17 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5800 b- defN 23-May-21 06:17 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     5065 b- defN 23-May-21 06:17 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     2657 b- defN 23-May-21 06:17 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx      722 b- defN 23-May-21 06:17 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     6621 b- defN 23-May-21 06:17 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    16518 b- defN 23-May-21 06:17 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-May-21 06:17 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-May-21 06:17 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-May-21 06:17 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-May-21 06:17 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-May-21 06:17 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    15938 b- defN 23-May-21 06:17 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-May-21 06:17 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-May-21 06:17 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-May-21 06:17 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-May-21 06:17 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx     2227 b- defN 23-May-21 06:17 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    15736 b- defN 23-May-21 06:17 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-May-21 06:17 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-May-21 06:17 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-May-21 06:17 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-May-21 06:17 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx     1810 b- defN 23-May-21 06:17 xsl/utilities/README.md
+-rw-r--r--  2.0 unx    30257 b- defN 23-May-21 06:17 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-May-21 06:17 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-May-21 06:17 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4299 b- defN 23-May-21 06:17 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-May-21 06:17 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     1276 b- defN 23-May-21 06:17 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-May-21 06:17 css/style_default.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-May-21 06:17 css/style_soundwriting.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-May-21 06:17 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-May-21 06:17 css/README.md
+-rw-r--r--  2.0 unx     1280 b- defN 23-May-21 06:17 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-21 06:17 css/colors_blue_red.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-May-21 06:17 css/mathbook-3.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-May-21 06:17 css/mathbook-content.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-May-21 06:17 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-21 06:17 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-21 06:17 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-May-21 06:17 css/colors_blue_green.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-May-21 06:17 css/pretext_add_on.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-May-21 06:17 css/colors_default.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-May-21 06:17 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-21 06:17 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-21 06:17 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-21 06:17 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-May-21 06:17 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx      691 b- defN 23-May-21 06:17 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-May-21 06:17 css/colors_red_blue.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-May-21 06:17 css/setcolors.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-21 06:17 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-21 06:17 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-May-21 06:17 css/epub.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-May-21 06:17 css/kindle.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-21 06:17 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-May-21 06:17 css/update_css
+140 files, 4816921 bytes uncompressed, 1013488 bytes compressed:  79.0%
```

#### xsl/publisher-variables.xsl

##### xsl/publisher-variables.xsl

```diff
@@ -3725,14 +3725,32 @@
       <xsl:when test="($latex.geometry != '')">
         <xsl:value-of select="$latex.geometry"/>
       </xsl:when>
       <!-- empty is the signal to not use -->
       <xsl:otherwise/>
     </xsl:choose>
   </xsl:variable>
+  <!-- For crop marks to make sense, a paper size must be known -->
+  <!-- There is no error-checking here, any non-empty value     -->
+  <!-- initiates the crop marks and becomes the paper size.     -->
+  <!-- Values from the  crop  package, 2023-05-19 are:          -->
+  <!--     a0, a1, a2, a3, a4, a5, a6,                          -->
+  <!--     b0, b1, b2, b3, b4, b5, b6,                          -->
+  <!--     letter, legal, executive                             -->
+  <xsl:variable name="latex-crop-papersize">
+    <xsl:choose>
+      <xsl:when test="$publication/latex/page/@crop-marks = 'none'"/>
+      <xsl:when test="not($publication/latex/page/@crop-marks)"/>
+      <xsl:otherwise>
+        <xsl:value-of select="$publication/latex/page/@crop-marks"/>
+      </xsl:otherwise>
+    </xsl:choose>
+  </xsl:variable>
+  <!-- empty implies feature not selected -->
+  <xsl:variable name="b-latex-crop-marks" select="not($latex-crop-papersize = '')"/>
   <!-- The default for the use of page references varies, so that  -->
   <!-- particular logic is in the -latex conversion.  Here we just -->
   <!-- sanitize to "yes", "no" or empty (i.e. ignored)             -->
   <xsl:variable name="latex-pageref">
     <xsl:choose>
       <!-- given in publication file -->
       <xsl:when test="$publication/latex/@pageref">
```

#### xsl/pretext-runestone.xsl

##### xsl/pretext-runestone.xsl

```diff
@@ -1684,39 +1684,19 @@
                         <xsl:text>,</xsl:text>
                       </xsl:if>
                     </xsl:for-each>
                   </xsl:attribute>
                 </xsl:if>
                 <!-- allow @include attribute on <program> -->
                 <xsl:if test="@include">
-                  <xsl:variable name="tokens" select="str:tokenize(@include, ', ')"/>
+                  <!-- space-separated this time -->
                   <xsl:attribute name="data-include">
-                    <xsl:for-each select="$tokens">
-                      <!-- attribute value is an xml:id, get target "program" -->
-                      <xsl:variable name="the-id">
-                        <xsl:value-of select="."/>
-                      </xsl:variable>
-                      <xsl:for-each select="$original">
-                        <xsl:variable name="target" select="id($the-id)"/>
-                        <xsl:if test="not($target)">
-                          <xsl:message>
-                            PTX:ERROR:   an included &quot;program&quot; with @xml:id value
-                            <xsl:value-of select="$the-id"/>
-                            was not found
-                          </xsl:message>
-                        </xsl:if>
-                        <!-- build database id of the target -->
-                        <xsl:apply-templates select="$target" mode="runestone-id"/>
-                        <!-- n - 1 separators, required by receiving Javascript -->
-                      </xsl:for-each>
-                      <!-- space-separated this time -->
-                      <xsl:if test="following-sibling::token">
-                        <xsl:text/>
-                      </xsl:if>
-                    </xsl:for-each>
+                    <xsl:apply-templates select="@include" mode="runestone-targets">
+                      <xsl:with-param name="separator" select="' '"/>
+                    </xsl:apply-templates>
                   </xsl:attribute>
                 </xsl:if>
                 <!-- SQL (only) needs an attribute so it can find some code -->
                 <xsl:if test="$active-language = 'sql'">
                   <xsl:attribute name="data-wasm">
                     <xsl:text>/_static</xsl:text>
                   </xsl:attribute>
@@ -1922,8 +1902,50 @@
           </xsl:element>
         </xsl:when>
         <!-- no other source/PTX element is supported , bail out-->
         <xsl:otherwise/>
       </xsl:choose>
     </div>
   </xsl:template>
+  <!-- ######### -->
+  <!-- Utilities -->
+  <!-- ######### -->
+  <!-- Runestone components, such as data files and select questions,  -->
+  <!-- frequently point to other Runestone components in the database. -->
+  <!--   * Authors point in their source with @xml:id                  -->
+  <!--     values in a space- or comma- separated list                 -->
+  <!--   * We locate the targets in the orginal source                 -->
+  <!--   * Compute the Runestone database id                           -->
+  <!--   * Return a list (varying separator) to use in Runestone HTML. -->
+  <xsl:template match="@*" mode="runestone-targets">
+    <xsl:param name="separator" select="'MISSING SEPARATOR'"/>
+    <!-- save off original context attribute for error-reporting -->
+    <xsl:variable name="original-attribute" select="."/>
+    <!-- comma or space separated in PreTeXt source -->
+    <xsl:variable name="tokens" select="str:tokenize(., ', ')"/>
+    <xsl:for-each select="$tokens">
+      <!-- attribute value is an xml:id, get target interactive -->
+      <xsl:variable name="the-id">
+        <xsl:value-of select="."/>
+      </xsl:variable>
+      <!-- context shift so  id()  functions properly -->
+      <xsl:for-each select="$original">
+        <xsl:variable name="target" select="id($the-id)"/>
+        <xsl:if test="not($target)">
+          <xsl:message>
+            PTX:ERROR:   an interactive with @xml:id value &quot;
+            <xsl:value-of select="$the-id"/>
+            &quot; in a &quot;@
+            <xsl:value-of select="local-name($original-attribute)"/>
+            &quot; attribute was not found
+          </xsl:message>
+        </xsl:if>
+        <!-- build Runestone database id of the target -->
+        <xsl:apply-templates select="$target" mode="runestone-id"/>
+        <!-- n - 1 separators, required by receiving Javascript -->
+      </xsl:for-each>
+      <xsl:if test="following-sibling::token">
+        <xsl:value-of select="$separator"/>
+      </xsl:if>
+    </xsl:for-each>
+  </xsl:template>
 </xsl:stylesheet>
```

#### xsl/pretext-latex.xsl

##### xsl/pretext-latex.xsl

```diff
@@ -463,14 +463,24 @@
     <xsl:text>}}</xsl:text>
     <xsl:text>%% Custom Page Layout Adjustments (use publisher page-geometry entry)</xsl:text>
     <xsl:if test="$latex-page-geometry != ''">
       <xsl:text>\geometry{</xsl:text>
       <xsl:value-of select="$latex-page-geometry"/>
       <xsl:text>}</xsl:text>
     </xsl:if>
+    <!-- Crop marks, as independent of author tools           -->
+    <!-- Always *after* geometry package, no driver selected, -->
+    <!-- since it should auto-detect.  Tested with xelatex.   -->
+    <!-- crop  package suggests explicitly turning off driver -->
+    <!-- options for the geometery package.  We don't.        -->
+    <xsl:if test="$b-latex-crop-marks">
+      <xsl:text>\usepackage[</xsl:text>
+      <xsl:value-of select="$latex-crop-papersize"/>
+      <xsl:text>,cam,center]{crop}</xsl:text>
+    </xsl:if>
     <xsl:if test="$latex-right-alignment = 'ragged'">
       <xsl:text>%% better handing of text alignment</xsl:text>
       <xsl:text>\usepackage{ragged2e}</xsl:text>
     </xsl:if>
     <!--                                  -->
     <!-- Conditional LaTeX engine support -->
     <!-- (exclusive of fonts)             -->
@@ -1692,15 +1702,14 @@
       <xsl:value-of select="$watermark-scale"/>
       <xsl:text>}</xsl:text>
     </xsl:if>
     <xsl:if test="$author-tools-new = 'yes'">
       <xsl:text>%% Collected author tools options (author-tools='yes')</xsl:text>
       <xsl:text>%% others need to be elsewhere, these are simply package additions</xsl:text>
       <xsl:text>\usepackage{showkeys}</xsl:text>
-      <xsl:text>\usepackage[letter,cam,center,pdflatex]{crop}</xsl:text>
     </xsl:if>
     <xsl:if test="$latex-image-preamble">
       <xsl:text>%% Graphics Preamble Entries</xsl:text>
       <xsl:value-of select="$latex-image-preamble"/>
     </xsl:if>
     <xsl:text>%% If tikz has been loaded, replace ampersand with \amp macro</xsl:text>
     <xsl:if test="$document-root//latex-image">
@@ -7589,14 +7598,15 @@
       <xsl:value-of select="key('kbdkey-key', $kbdkey-name)/@latex"/>
     </xsl:for-each>
     <xsl:text>}</xsl:text>
   </xsl:template>
   <!-- ################ -->
   <!-- Biological Names -->
   <!-- ################ -->
+  <!-- See a potentially cleaner template in the braille conversion -->
   <xsl:template match="taxon[not(genus) and not(species)]">
     <xsl:text>\textit{</xsl:text>
     <xsl:apply-templates/>
     <xsl:text>}</xsl:text>
   </xsl:template>
   <xsl:template match="taxon[genus or species]">
     <xsl:if test="genus">
```

#### xsl/pretext-braille-preprint.xsl

##### xsl/pretext-braille-preprint.xsl

```diff
@@ -1306,14 +1306,40 @@
   <!-- Bold -->
   <xsl:template match="term|alert">
     <!-- Python will assume "bold" as element name -->
     <bold>
       <xsl:apply-templates select="node()"/>
     </bold>
   </xsl:template>
+  <!-- Biological Names -->
+  <xsl:template match="taxon">
+    <!-- In italic font -->
+    <italic>
+      <xsl:choose>
+        <!-- both substructures -->
+        <xsl:when test="genus and species">
+          <xsl:apply-templates select="genus"/>
+          <xsl:text/>
+          <xsl:apply-templates select="species"/>
+        </xsl:when>
+        <!-- just one -->
+        <xsl:when test="genus">
+          <xsl:apply-templates select="genus"/>
+        </xsl:when>
+        <!-- just the other one -->
+        <xsl:when test="species">
+          <xsl:apply-templates select="species"/>
+        </xsl:when>
+        <!-- not structured, use content -->
+        <xsl:otherwise>
+          <xsl:apply-templates/>
+        </xsl:otherwise>
+      </xsl:choose>
+    </italic>
+  </xsl:template>
   <!-- Code -->
   <!-- Accomplished in UEB Grade 2, but with transcriber emphasis scheme 1 -->
   <!-- from liblouis (where is this defined?).  See liblouis table         -->
   <!-- "en-ueb-g1.ctb" for exact definition of emphasis code "trans1".     -->
   <!--                                                                     -->
   <!--     emphletter trans1 4-3456-23                                     -->
   <!--     begemphword trans1 4-3456-2                                     -->
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -8494,14 +8494,15 @@
         <xsl:value-of select="key('kbdkey-key', $kbdkey-name)/@unicode"/>
       </xsl:for-each>
     </kbd>
   </xsl:template>
   <!-- ################ -->
   <!-- Biological Names -->
   <!-- ################ -->
+  <!-- See a potentially cleaner template in the braille conversion -->
   <xsl:template match="taxon[not(genus) and not(species)]">
     <span class="taxon">
       <xsl:apply-templates/>
     </span>
   </xsl:template>
   <xsl:template match="taxon[genus or species]">
     <span class="taxon">
```

### Comparing `pretext-1.5.4.dev20230519/pretext/generate.py` & `pretext-1.5.4.dev20230521/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pretext/project.py` & `pretext-1.5.4.dev20230521/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pretext/templates/__init__.py` & `pretext-1.5.4.dev20230521/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pretext/templates/resources/.gitignore` & `pretext-1.5.4.dev20230521/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pretext/templates/resources/article.zip` & `pretext-1.5.4.dev20230521/pretext/templates/resources/article.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,16 @@
-Zip file size: 160548 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 source/
--rw-r--r--  2.0 unx       86 b- defN 23-May-19 06:17 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-19 06:18 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-19 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-19 06:18 .gitignore
--rw-r--r--  2.0 unx   154806 b- defN 23-May-19 06:17 assets/frog.jpg
--rw-r--r--  2.0 unx     2059 b- defN 23-May-19 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-19 06:18 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx      242 b- defN 23-May-19 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-May-19 06:17 source/main.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-May-19 06:17 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-May-19 06:17 source/section-2.ptx
-15 files, 165338 bytes uncompressed, 158882 bytes compressed:  3.9%
+Zip file size: 160064 bytes, number of entries: 14
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 source/
+-rw-r--r--  2.0 unx       86 b- defN 23-May-21 06:16 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-21 06:17 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-21 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-21 06:17 .gitignore
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-21 06:16 assets/frog.jpg
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-21 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 23-May-21 06:16 publication/publication.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-May-21 06:16 source/main.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-May-21 06:16 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-May-21 06:16 source/section-2.ptx
+14 files, 164708 bytes uncompressed, 158542 bytes compressed:  3.7%
```

#### zipnote {}

```diff
@@ -24,17 +24,14 @@
 
 Filename: assets/frog.jpg
 Comment: 
 
 Filename: .devcontainer/devcontainer.json
 Comment: 
 
-Filename: .devcontainer/postCreateCommand.sh
-Comment: 
-
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
 Filename: source/section-1.ptx
```

### Comparing `pretext-1.5.4.dev20230519/pretext/templates/resources/book.zip` & `pretext-1.5.4.dev20230521/pretext/templates/resources/book.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,12 @@
-Zip file size: 8054 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 source/
--rw-r--r--  2.0 unx       82 b- defN 23-May-19 06:17 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-19 06:18 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-19 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-19 06:18 .gitignore
--rw-r--r--  2.0 unx     2059 b- defN 23-May-19 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-19 06:18 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     6114 b- defN 23-May-19 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-May-19 06:17 source/main.ptx
-11 files, 16306 bytes uncompressed, 6816 bytes compressed:  58.2%
+Zip file size: 7570 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-May-21 06:16 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-21 06:17 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-21 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-21 06:17 .gitignore
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-21 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     6114 b- defN 23-May-21 06:16 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-May-21 06:16 source/main.ptx
+10 files, 15676 bytes uncompressed, 6476 bytes compressed:  58.7%
```

#### zipnote {}

```diff
@@ -18,17 +18,14 @@
 
 Filename: .gitignore
 Comment: 
 
 Filename: .devcontainer/devcontainer.json
 Comment: 
 
-Filename: .devcontainer/postCreateCommand.sh
-Comment: 
-
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.5.4.dev20230519/pretext/templates/resources/demo.zip` & `pretext-1.5.4.dev20230521/pretext/templates/resources/demo.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,37 +1,36 @@
-Zip file size: 173747 bytes, number of entries: 35
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 source/
--rw-r--r--  2.0 unx       82 b- defN 23-May-19 06:17 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-19 06:18 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-19 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-19 06:18 .gitignore
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-May-19 06:17 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-May-19 06:17 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     2059 b- defN 23-May-19 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-19 06:18 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx     6092 b- defN 23-May-19 06:17 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 source/images/
--rw-r--r--  2.0 unx      847 b- defN 23-May-19 06:17 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-May-19 06:17 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-May-19 06:17 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-May-19 06:17 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-May-19 06:17 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-May-19 06:17 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-May-19 06:17 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-May-19 06:17 source/frontmatter.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-May-19 06:17 source/ch-features.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-May-19 06:17 source/ch-generate.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-May-19 06:17 source/sec-features.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-May-19 06:17 source/backmatter.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-May-19 06:17 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-May-19 06:17 source/ch-empty.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-May-19 06:17 source/ex-first.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-May-19 06:17 source/docinfo.ptx
--rw-r--r--  2.0 unx       10 b- defN 23-May-19 06:17 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-May-19 06:17 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 23-May-19 06:17 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-May-19 06:17 source/images/sageplot3d.sage
-35 files, 190601 bytes uncompressed, 169647 bytes compressed:  11.0%
+Zip file size: 173263 bytes, number of entries: 34
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-May-21 06:16 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-21 06:17 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-21 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-21 06:17 .gitignore
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-21 06:16 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-May-21 06:16 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-21 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     6092 b- defN 23-May-21 06:16 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 source/images/
+-rw-r--r--  2.0 unx      847 b- defN 23-May-21 06:16 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-May-21 06:16 source/main.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-May-21 06:16 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-May-21 06:16 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-May-21 06:16 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-May-21 06:16 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-May-21 06:16 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-May-21 06:16 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-May-21 06:16 source/ch-features.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-May-21 06:16 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-May-21 06:16 source/sec-features.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-May-21 06:16 source/backmatter.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-May-21 06:16 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-May-21 06:16 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-May-21 06:16 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-May-21 06:16 source/docinfo.ptx
+-rw-r--r--  2.0 unx       10 b- defN 23-May-21 06:16 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-May-21 06:16 source/images/cflag.asy
+-rw-r--r--  2.0 unx      357 b- defN 23-May-21 06:16 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 23-May-21 06:16 source/images/sageplot3d.sage
+34 files, 189971 bytes uncompressed, 169307 bytes compressed:  10.9%
```

#### zipnote {}

```diff
@@ -30,17 +30,14 @@
 
 Filename: assets/jsxgraph/infinity.js
 Comment: 
 
 Filename: .devcontainer/devcontainer.json
 Comment: 
 
-Filename: .devcontainer/postCreateCommand.sh
-Comment: 
-
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/images/
 Comment: 
 
 Filename: source/sec-first-intro.ptx
```

### Comparing `pretext-1.5.4.dev20230519/pretext/templates/resources/devcontainer.json` & `pretext-1.5.4.dev20230521/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pretext/templates/resources/hello.zip` & `pretext-1.5.4.dev20230521/pretext/templates/resources/hello.zip`

 * *Files 23% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,12 @@
-Zip file size: 5095 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 source/
--rw-r--r--  2.0 unx       69 b- defN 23-May-19 06:17 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-May-19 06:17 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-19 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-19 06:18 .gitignore
--rw-r--r--  2.0 unx     2059 b- defN 23-May-19 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-19 06:18 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx      242 b- defN 23-May-19 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-May-19 06:17 source/main.ptx
-11 files, 8317 bytes uncompressed, 3857 bytes compressed:  53.6%
+Zip file size: 4611 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 source/
+-rw-r--r--  2.0 unx       69 b- defN 23-May-21 06:16 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-May-21 06:16 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-21 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-21 06:17 .gitignore
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-21 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 23-May-21 06:16 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-May-21 06:16 source/main.ptx
+10 files, 7687 bytes uncompressed, 3517 bytes compressed:  54.2%
```

#### zipnote {}

```diff
@@ -18,17 +18,14 @@
 
 Filename: .gitignore
 Comment: 
 
 Filename: .devcontainer/devcontainer.json
 Comment: 
 
-Filename: .devcontainer/postCreateCommand.sh
-Comment: 
-
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.5.4.dev20230519/pretext/templates/resources/project.ptx` & `pretext-1.5.4.dev20230521/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pretext/templates/resources/slideshow.zip` & `pretext-1.5.4.dev20230521/pretext/templates/resources/slideshow.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 8830 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-19 06:17 xsl/
--rw-r--r--  2.0 unx      784 b- defN 23-May-19 06:17 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-19 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-19 06:18 .gitignore
--rw-r--r--  2.0 unx     2059 b- defN 23-May-19 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      630 b- defN 23-May-19 06:18 .devcontainer/postCreateCommand.sh
--rw-r--r--  2.0 unx      190 b- defN 23-May-19 06:17 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-May-19 06:17 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-May-19 06:17 source/main.ptx
-12 files, 20904 bytes uncompressed, 7498 bytes compressed:  64.1%
+Zip file size: 8346 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:17 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-21 06:16 xsl/
+-rw-r--r--  2.0 unx      784 b- defN 23-May-21 06:16 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-21 06:17 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-21 06:17 .gitignore
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-21 06:17 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      190 b- defN 23-May-21 06:16 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 23-May-21 06:16 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-May-21 06:16 source/main.ptx
+11 files, 20274 bytes uncompressed, 7158 bytes compressed:  64.7%
```

#### zipnote {}

```diff
@@ -18,17 +18,14 @@
 
 Filename: .gitignore
 Comment: 
 
 Filename: .devcontainer/devcontainer.json
 Comment: 
 
-Filename: .devcontainer/postCreateCommand.sh
-Comment: 
-
 Filename: xsl/slides.xsl
 Comment: 
 
 Filename: publication/publication.ptx
 Comment: 
 
 Filename: source/main.ptx
```

### Comparing `pretext-1.5.4.dev20230519/pretext/utils.py` & `pretext-1.5.4.dev20230521/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230519/pyproject.toml` & `pretext-1.5.4.dev20230521/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.5.4.dev20230519"
+version = "1.5.4.dev20230521"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.5.4.dev20230519/PKG-INFO` & `pretext-1.5.4.dev20230521/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.5.4.dev20230519
+Version: 1.5.4.dev20230521
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

