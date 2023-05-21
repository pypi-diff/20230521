# Comparing `tmp/mkdpdf-0.2.1.tar.gz` & `tmp/mkdpdf-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdpdf-0.2.1.tar", last modified: Wed Apr 13 00:42:42 2022, max compression
+gzip compressed data, was "mkdpdf-0.2.2.tar", last modified: Sun May 21 19:41:12 2023, max compression
```

## Comparing `mkdpdf-0.2.1.tar` & `mkdpdf-0.2.2.tar`

### file list

```diff
@@ -1,64 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.408083 mkdpdf-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      433 2022-04-13 00:42:42.407083 mkdpdf-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      193 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.396082 mkdpdf-0.2.1/mkdpdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.399082 mkdpdf-0.2.1/mkdpdf/document/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11465 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/document/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.390082 mkdpdf-0.2.1/mkdpdf/document/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.391082 mkdpdf-0.2.1/mkdpdf/document/templates/pdf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.401082 mkdpdf-0.2.1/mkdpdf/document/templates/pdf/style/
--rw-rw-rw-   0 root         (0) root         (0)      180 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/document/templates/pdf/style/document.css
--rw-rw-rw-   0 root         (0) root         (0)      268 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/document/templates/pdf/style/footer.css
--rw-rw-rw-   0 root         (0) root         (0)      249 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/document/templates/pdf/style/header.css
--rw-rw-rw-   0 root         (0) root         (0)     6683 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/document/templates/pdf/style/mermaid.css
--rw-rw-rw-   0 root         (0) root         (0)     2097 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/document/templates/pdf/style/pdf.css
--rw-rw-rw-   0 root         (0) root         (0)     3199 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/document/templates/pdf/style/reset.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.401082 mkdpdf-0.2.1/mkdpdf/documentation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/documentation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9590 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/documentation/documentation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.392082 mkdpdf-0.2.1/mkdpdf/documentation/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.402083 mkdpdf-0.2.1/mkdpdf/documentation/templates/md/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.403082 mkdpdf-0.2.1/mkdpdf/documentation/templates/md/class/
--rw-rw-rw-   0 root         (0) root         (0)      564 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/documentation/templates/md/class/header.md
--rw-rw-rw-   0 root         (0) root         (0)      137 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/documentation/templates/md/class/main.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.403082 mkdpdf-0.2.1/mkdpdf/documentation/templates/md/functions/
--rw-rw-rw-   0 root         (0) root         (0)      517 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/documentation/templates/md/functions/header.md
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/documentation/templates/md/functions/main.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/documentation/templates/md/header.md
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/documentation/templates/md/main.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.392082 mkdpdf-0.2.1/mkdpdf/documentation/templates/pdf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.404083 mkdpdf-0.2.1/mkdpdf/documentation/templates/pdf/style/
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/documentation/templates/pdf/style/document.css
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/documentation/templates/pdf/style/footer.css
--rw-rw-rw-   0 root         (0) root         (0)       49 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/documentation/templates/pdf/style/header.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.405083 mkdpdf-0.2.1/mkdpdf/md/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/md/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1246 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/md/md.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.406083 mkdpdf-0.2.1/mkdpdf/pdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/pdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4660 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/pdf/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     3234 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/pdf/publisher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.406083 mkdpdf-0.2.1/mkdpdf/report/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/report/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/report/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.394082 mkdpdf-0.2.1/mkdpdf/report/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.407083 mkdpdf-0.2.1/mkdpdf/report/templates/md/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/report/templates/md/footer.md
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/report/templates/md/header.md
--rw-rw-rw-   0 root         (0) root         (0)       72 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/mkdpdf/report/templates/md/main.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-13 00:42:42.398082 mkdpdf-0.2.1/mkdpdf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      433 2022-04-13 00:42:42.000000 mkdpdf-0.2.1/mkdpdf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1420 2022-04-13 00:42:42.000000 mkdpdf-0.2.1/mkdpdf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-13 00:42:42.000000 mkdpdf-0.2.1/mkdpdf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2022-04-13 00:42:42.000000 mkdpdf-0.2.1/mkdpdf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2022-04-13 00:42:42.000000 mkdpdf-0.2.1/mkdpdf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-04-13 00:42:42.000000 mkdpdf-0.2.1/mkdpdf.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-04-13 00:42:42.408083 mkdpdf-0.2.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      976 2022-04-13 00:42:34.000000 mkdpdf-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.561535 mkdpdf-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-21 19:41:12.561535 mkdpdf-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      193 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.554535 mkdpdf-0.2.2/mkdpdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.555535 mkdpdf-0.2.2/mkdpdf/document/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/document/document.md
+-rw-rw-rw-   0 root         (0) root         (0)    11386 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/document/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.550536 mkdpdf-0.2.2/mkdpdf/document/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.550536 mkdpdf-0.2.2/mkdpdf/document/templates/pdf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.556535 mkdpdf-0.2.2/mkdpdf/document/templates/pdf/style/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/document/templates/pdf/style/document.css
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/document/templates/pdf/style/footer.css
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/document/templates/pdf/style/header.css
+-rw-rw-rw-   0 root         (0) root         (0)     6683 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/document/templates/pdf/style/mermaid.css
+-rw-rw-rw-   0 root         (0) root         (0)     2193 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/document/templates/pdf/style/pdf.css
+-rw-rw-rw-   0 root         (0) root         (0)     3199 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/document/templates/pdf/style/reset.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.557536 mkdpdf-0.2.2/mkdpdf/documentation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/documentation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8053 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/documentation/documentation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.551535 mkdpdf-0.2.2/mkdpdf/documentation/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.557536 mkdpdf-0.2.2/mkdpdf/documentation/templates/md/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.557536 mkdpdf-0.2.2/mkdpdf/documentation/templates/md/class/
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/documentation/templates/md/class/header.md
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/documentation/templates/md/class/main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.558535 mkdpdf-0.2.2/mkdpdf/documentation/templates/md/functions/
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/documentation/templates/md/functions/header.md
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/documentation/templates/md/functions/main.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/documentation/templates/md/header.md
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/documentation/templates/md/main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.551535 mkdpdf-0.2.2/mkdpdf/documentation/templates/pdf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.558535 mkdpdf-0.2.2/mkdpdf/documentation/templates/pdf/style/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/documentation/templates/pdf/style/document.css
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/documentation/templates/pdf/style/footer.css
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/documentation/templates/pdf/style/header.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.558535 mkdpdf-0.2.2/mkdpdf/md/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/md/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/md/md.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.559535 mkdpdf-0.2.2/mkdpdf/pdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/pdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4763 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/pdf/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/pdf/publisher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.559535 mkdpdf-0.2.2/mkdpdf/report/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/report/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/report/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.552535 mkdpdf-0.2.2/mkdpdf/report/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.560536 mkdpdf-0.2.2/mkdpdf/report/templates/md/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/report/templates/md/footer.md
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/report/templates/md/header.md
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/report/templates/md/main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.560536 mkdpdf-0.2.2/mkdpdf/report/templates/pdf/
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/report/templates/pdf/footer.html
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/report/templates/pdf/header.html
+-rw-rw-rw-   0 root         (0) root         (0)     1338 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/report/templates/pdf/main.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.561535 mkdpdf-0.2.2/mkdpdf/report/templates/pdf/style/
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/report/templates/pdf/style/document.css
+-rw-rw-rw-   0 root         (0) root         (0)      755 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/report/templates/pdf/style/footer.css
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/report/templates/pdf/style/header.css
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/mkdpdf/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 19:41:12.555535 mkdpdf-0.2.2/mkdpdf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-21 19:41:12.000000 mkdpdf-0.2.2/mkdpdf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1723 2023-05-21 19:41:12.000000 mkdpdf-0.2.2/mkdpdf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 19:41:12.000000 mkdpdf-0.2.2/mkdpdf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-21 19:41:12.000000 mkdpdf-0.2.2/mkdpdf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-21 19:41:12.000000 mkdpdf-0.2.2/mkdpdf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-21 19:41:12.000000 mkdpdf-0.2.2/mkdpdf.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 19:41:12.561535 mkdpdf-0.2.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      976 2023-05-21 19:41:05.000000 mkdpdf-0.2.2/setup.py
```

### Comparing `mkdpdf-0.2.1/mkdpdf/configuration.py` & `mkdpdf-0.2.2/mkdpdf/configuration.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import datetime
 import os
 
 import mkdpdf
 
 # FILE SYSTEM
-DIRECTORY_PATH_OUTPUT = os.environ["DIRECTORY_PATH_OUTPUT"] if "DIRECTORY_PATH_OUTPUT" in os.environ else os.getcwd()
+DIRECTORY_PATH_OUTPUT = os.environ.get("DIRECTORY_PATH_OUTPUT", os.getcwd())
 DIRECTORY_PATH_PACKAGE = os.path.dirname(mkdpdf.__file__)
-FILENAME = (os.environ["FILENAME"].split(".")[0] if "." in os.environ["FILENAME"] else os.environ["FILENAME"]) if "FILENAME" in os.environ else None
+FILENAME_FULL = os.environ.get("FILENAME", None)
+FILENAME = FILENAME.split(".")[0] if FILENAME_FULL and "." in FILENAME_FULL else None
 
 # LAYOUT
 DOCUMENT_EXTRA_VERTICAL_MARGIN = 30
 DOCUMENT_SIDE_MARGIN = 2
 GITFLAVOR_BREAK_RETURN = "\r\n"
 GITFLAVOR_RETURN = "\r\n\r\n"
-FORMAT = os.environ["FORMAT"] if "FORMAT" in os.environ else "md"
+FORMAT = os.environ.get("FORMAT", "md")
 # output render format : input template format
 TEMPLATES = {
     "md": "md",
     "pdf": "html"
 }
 
 # TIME
```

### Comparing `mkdpdf-0.2.1/mkdpdf/document/document.py` & `mkdpdf-0.2.2/mkdpdf/document/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from email.mime.text import MIMEText
 
 import mkdpdf
 
 from mkdpdf import configuration
 from mkdpdf.md.md import MD
 from mkdpdf.pdf.pdf import PDF
+from mkdpdf.utilities import clean
 
 class Document:
     """
     Document is a Markdown or Portable Document Format document.
     """
 
     def __init__(self, title: str = None, format: str = configuration.FORMAT, filename: str = configuration.FILENAME, directory_path_output: str = configuration.DIRECTORY_PATH_OUTPUT, directory_name_templates: str = None, directory_path_templates: str = None, email_host: str = None):
@@ -190,25 +191,15 @@
         Render document to filesystem.
 
         Args:
             content (string): partial of Markdown or HTML
             file_path (string): output file path
         """
 
-        # clean up content
-        content = re.sub(r"^__", "", content, flags=re.MULTILINE)
-        content = re.sub(r"^None", "\n", content, flags=re.MULTILINE)
-        content = re.sub(r"(\r\n\r\n)+", "REPLACE_RETURNS", content)
-        content = re.sub(r"\r\n", "KEEP_RETURNS", content)
-        content = re.sub(r"\n+", "REPLACE_RETURNS", content)
-        content = re.sub(r"KEEP_RETURNS", configuration.GITFLAVOR_BREAK_RETURN, content)
-        content = re.sub(r"REPLACE_RETURNS", "\n\n", content)
-        content = re.sub(r"\n+\Z", "", content)
-        content = re.sub(r"```python\n+", "```python%s" % configuration.GITFLAVOR_BREAK_RETURN, content)
-        content = re.sub(r"\n+```\n+", "%s```%s" % (configuration.GITFLAVOR_BREAK_RETURN, configuration.GITFLAVOR_RETURN), content)
+        content = content if self.format != "md" else clean(content)
 
         self.document.render(content, file_path)
 
     def template(self, type: str, section) -> str:
         """
         Determine template from provided or core class template.
 
@@ -280,14 +271,32 @@
 
         Returns:
             A string representing a partial in the file format of the template.
         """
 
         result = template
 
+        # check if subtemplates are in result
+        if result and "SUBTEMPLATE_" in result:
+
+            # get subtemplates
+            subtemplates = re.findall(r"SUBTEMPLATE_.+", result)
+
+            # loop through subtemplates
+            for placeholder in subtemplates:
+
+                # get subtemplate method
+                subtemplate_method = getattr(self, placeholder)
+
+                # generate content for subtemplate
+                subtemplate = subtemplate_method(section[placeholder])
+
+                # update reference dictionary
+                section[placeholder] = subtemplate
+
         # loop through keys
         for key in section:
 
             # set replacement content
             replacement = section[key]
 
             # look for markdown table format when processing pdf format
```

### Comparing `mkdpdf-0.2.1/mkdpdf/document/templates/pdf/style/mermaid.css` & `mkdpdf-0.2.2/mkdpdf/document/templates/pdf/style/mermaid.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.1/mkdpdf/document/templates/pdf/style/pdf.css` & `mkdpdf-0.2.2/mkdpdf/document/templates/pdf/style/pdf.css`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,17 @@
     text-wrap: balance;
 
 }
 
 p, li {
 
   font-family: var(--sans-serif);
+  -webkit-column-break-inside: avoid;
+  page-break-inside: avoid;
+  break-inside: avoid-column;
 
 }
 
 li {
 
     list-style: disc;
     padding-left: 1em;
```

### Comparing `mkdpdf-0.2.1/mkdpdf/document/templates/pdf/style/reset.css` & `mkdpdf-0.2.2/mkdpdf/document/templates/pdf/style/reset.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.1/mkdpdf/documentation/documentation.py` & `mkdpdf-0.2.2/mkdpdf/documentation/documentation.py`

 * *Files 14% similar despite different names*

```diff
@@ -146,56 +146,7 @@
                 "**%s**" % v["type"] if v["type"] else str(),
                 "<br>".join([
                             "`%s`" % d.strip() for d in v["value"].split("|")
                         ]) if "|" in v["value"] else v["value"],
                 v["default"]
             )
         """
-
-    def transpile(self, section: dict, template: str) -> str:
-        """
-        Replace placeholders in templates with provided content.
-
-        Args:
-            section (dictionary): key/value pairs to find/replace in package template
-            template (string): partial section of document
-
-        Returns:
-            A string representing a partial in the file format of the template.
-        """
-
-        result = template
-
-        # check if subtemplates are in result
-        if result and "SUBTEMPLATE_" in result:
-
-            # get subtemplates
-            subtemplates = re.findall(r"SUBTEMPLATE_.+", result)
-
-            # loop through subtemplates
-            for placeholder in subtemplates:
-
-                # get subtemplate method
-                subtemplate_method = getattr(self, placeholder)
-
-                # generate content for subtemplate
-                subtemplate = subtemplate_method(section[placeholder])
-
-                # update reference dictionary
-                section[placeholder] = subtemplate
-
-        # loop through keys
-        for key in section:
-
-            # set replacement content
-            replacement = section[key]
-
-            # look for markdown table format when processing pdf format
-            if self.format == "pdf" and "| :-- |" in section[key]:
-
-                # convert markdown to html
-                replacement = self.document.table(section[key])
-
-            # replace in template
-            result = result.replace(key, replacement)
-
-        return result
```

### Comparing `mkdpdf-0.2.1/mkdpdf/documentation/templates/md/class/header.md` & `mkdpdf-0.2.2/mkdpdf/documentation/templates/md/class/header.md`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.1/mkdpdf/documentation/templates/md/functions/header.md` & `mkdpdf-0.2.2/mkdpdf/documentation/templates/md/functions/header.md`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.1/mkdpdf/md/md.py` & `mkdpdf-0.2.2/mkdpdf/md/md.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.1/mkdpdf/pdf/pdf.py` & `mkdpdf-0.2.2/mkdpdf/pdf/pdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import markdown
 
 from weasyprint import HTML
 
 from mkdpdf import configuration
 from mkdpdf.pdf.publisher import PDFPublisher
+from mkdpdf.utilities import clean
 
 class PDF(PDFPublisher):
     """
     PDF is a Portable Document Format render object.
     """
 
     def __init__(self, directory_path_templates: str):
@@ -68,24 +69,24 @@
         header_height = 0
 
         # account for overlays
         if header:
 
             # wrap in required tag if not already
             if (isinstance(header, str) and not header.startswith("<header>")) or (isinstance(header, str) and not header.endswith("</header>")):
-                header = "<header>%s</header>" % header
+                header = "<header>%s</header>" % clean(header)
 
             # calculate space
             header_body, header_height = self.configure_overlay("header", header)
 
         if footer:
 
             # wrap in required tag if not already
             if (isinstance(footer, str) and not footer.startswith("<footer>")) or (isinstance(footer, str) and not footer.endswith("</footer>")):
-                footer = "<footer>%s</footer>" % footer
+                footer = "<footer>%s</footer>" % clean(footer)
 
             # calculate space
             footer_body, footer_height = self.configure_overlay("footer", footer)
 
         # if not core document class
         if self.template != "document":
 
@@ -102,17 +103,20 @@
                 main = "<main>%s</main>" % main
 
         else:
 
             # set empty content
             main = "<main></main>"
 
+        # clean up main content
+        m = clean(main)
+
         # generate main body
         main_body = HTML(
-            string=main,
+            string=m,
             base_url="/notebooks"
         ).render(
             stylesheets=self.stylesheets
         )
 
         # check for overlays
         if header or footer:
```

### Comparing `mkdpdf-0.2.1/mkdpdf/pdf/publisher.py` & `mkdpdf-0.2.2/mkdpdf/pdf/publisher.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.1/mkdpdf.egg-info/SOURCES.txt` & `mkdpdf-0.2.2/mkdpdf.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 README.md
 VERSION
 requirements-test.txt
 requirements.txt
 setup.py
 mkdpdf/__init__.py
 mkdpdf/configuration.py
+mkdpdf/utilities.py
 mkdpdf.egg-info/PKG-INFO
 mkdpdf.egg-info/SOURCES.txt
 mkdpdf.egg-info/dependency_links.txt
 mkdpdf.egg-info/entry_points.txt
 mkdpdf.egg-info/requires.txt
 mkdpdf.egg-info/top_level.txt
 mkdpdf/document/__init__.py
+mkdpdf/document/document.md
 mkdpdf/document/document.py
 mkdpdf/document/templates/pdf/style/document.css
 mkdpdf/document/templates/pdf/style/footer.css
 mkdpdf/document/templates/pdf/style/header.css
 mkdpdf/document/templates/pdf/style/mermaid.css
 mkdpdf/document/templates/pdf/style/pdf.css
 mkdpdf/document/templates/pdf/style/reset.css
@@ -36,8 +38,14 @@
 mkdpdf/pdf/__init__.py
 mkdpdf/pdf/pdf.py
 mkdpdf/pdf/publisher.py
 mkdpdf/report/__init__.py
 mkdpdf/report/report.py
 mkdpdf/report/templates/md/footer.md
 mkdpdf/report/templates/md/header.md
-mkdpdf/report/templates/md/main.md
+mkdpdf/report/templates/md/main.md
+mkdpdf/report/templates/pdf/footer.html
+mkdpdf/report/templates/pdf/header.html
+mkdpdf/report/templates/pdf/main.html
+mkdpdf/report/templates/pdf/style/document.css
+mkdpdf/report/templates/pdf/style/footer.css
+mkdpdf/report/templates/pdf/style/header.css
```

### Comparing `mkdpdf-0.2.1/setup.py` & `mkdpdf-0.2.2/setup.py`

 * *Files identical despite different names*

