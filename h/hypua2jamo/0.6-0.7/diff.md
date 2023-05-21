# Comparing `tmp/hypua2jamo-0.6.tar.gz` & `tmp/hypua2jamo-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypua2jamo-0.6.tar", last modified: Sat Apr  1 17:24:43 2023, max compression
+gzip compressed data, was "hypua2jamo-0.7.tar", last modified: Sun May 21 20:12:17 2023, max compression
```

## Comparing `hypua2jamo-0.6.tar` & `hypua2jamo-0.7.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 yoosung   (1000) yoosung   (1000)        0 2023-04-01 17:24:43.397281 hypua2jamo-0.6/
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      309 2023-04-01 17:24:43.000000 hypua2jamo-0.6/.coveragerc
--rwxr-xr-x   0 yoosung   (1000) yoosung   (1000)     2218 2023-04-01 17:24:43.000000 hypua2jamo-0.6/.manylinux-install.sh
--rwxr-xr-x   0 yoosung   (1000) yoosung   (1000)      608 2023-04-01 17:24:43.000000 hypua2jamo-0.6/.manylinux.sh
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      846 2023-04-01 17:24:43.000000 hypua2jamo-0.6/CHANGES.rst
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)    35147 2023-04-01 17:24:43.000000 hypua2jamo-0.6/COPYING
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     7651 2023-04-01 17:24:43.000000 hypua2jamo-0.6/COPYING.LESSER
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     1450 2023-04-01 17:24:43.000000 hypua2jamo-0.6/MANIFEST.in
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     4213 2023-04-01 17:24:43.000000 hypua2jamo-0.6/Makefile
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     4597 2023-04-01 17:24:43.397281 hypua2jamo-0.6/PKG-INFO
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     2452 2023-04-01 17:24:43.000000 hypua2jamo-0.6/README.rst
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     2569 2023-04-01 17:24:43.000000 hypua2jamo-0.6/appveyor.yml
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     6219 2023-04-01 17:24:43.000000 hypua2jamo-0.6/benchmark.py
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)       86 2023-04-01 17:24:43.000000 hypua2jamo-0.6/buildout.cfg
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      263 2023-04-01 17:24:43.000000 hypua2jamo-0.6/ccompiler-vc90.cmd
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      256 2023-04-01 17:24:43.000000 hypua2jamo-0.6/ccompiler-vs2019.cmd
-drwxr-xr-x   0 yoosung   (1000) yoosung   (1000)        0 2023-04-01 17:24:43.389281 hypua2jamo-0.6/docs/
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      588 2023-04-01 17:24:43.000000 hypua2jamo-0.6/docs/Makefile
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     6015 2023-04-01 17:24:43.000000 hypua2jamo-0.6/docs/conf.py
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      125 2023-04-01 17:24:43.000000 hypua2jamo-0.6/docs/hypua2jamo-cli.rst
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      587 2023-04-01 17:24:43.000000 hypua2jamo-0.6/docs/hypua2jamo.rst
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      476 2023-04-01 17:24:43.000000 hypua2jamo-0.6/docs/index.rst
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)       27 2023-04-01 17:24:43.000000 hypua2jamo-0.6/docs/intro.rst
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      756 2023-04-01 17:24:43.000000 hypua2jamo-0.6/docs/make.bat
-drwxr-xr-x   0 yoosung   (1000) yoosung   (1000)        0 2023-04-01 17:24:43.389281 hypua2jamo-0.6/examples/
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      109 2023-04-01 17:24:43.000000 hypua2jamo-0.6/examples/HunMinPreface.hypua.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      142 2023-04-01 17:24:43.000000 hypua2jamo-0.6/examples/HunMinPreface.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     4109 2023-04-01 17:24:43.000000 hypua2jamo-0.6/hypua2jamo_build.py
-drwxr-xr-x   0 yoosung   (1000) yoosung   (1000)        0 2023-04-01 17:24:43.389281 hypua2jamo-0.6/requirements/
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      269 2023-04-01 17:24:43.000000 hypua2jamo-0.6/requirements/dev.in
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     9817 2023-04-01 17:24:43.000000 hypua2jamo-0.6/requirements/dev.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      130 2023-04-01 17:24:43.000000 hypua2jamo-0.6/requirements/docs.in
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     1721 2023-04-01 17:24:43.000000 hypua2jamo-0.6/requirements/docs.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)       53 2023-04-01 17:24:43.000000 hypua2jamo-0.6/requirements/lint.in
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     1119 2023-04-01 17:24:43.000000 hypua2jamo-0.6/requirements/lint.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)       14 2023-04-01 17:24:43.000000 hypua2jamo-0.6/requirements/setup.in
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)        0 2023-04-01 17:24:43.000000 hypua2jamo-0.6/requirements/site.in
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      257 2023-04-01 17:24:43.000000 hypua2jamo-0.6/requirements/site.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)       56 2023-04-01 17:24:43.000000 hypua2jamo-0.6/requirements/test.in
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      493 2023-04-01 17:24:43.000000 hypua2jamo-0.6/requirements/test.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)       14 2023-04-01 17:24:43.000000 hypua2jamo-0.6/requirements.in
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      231 2023-04-01 17:24:43.000000 hypua2jamo-0.6/requirements.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      229 2023-04-01 17:24:43.397281 hypua2jamo-0.6/setup.cfg
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     7526 2023-04-01 17:24:43.000000 hypua2jamo-0.6/setup.py
-drwxr-xr-x   0 yoosung   (1000) yoosung   (1000)        0 2023-04-01 17:24:43.385281 hypua2jamo-0.6/src/
-drwxr-xr-x   0 yoosung   (1000) yoosung   (1000)        0 2023-04-01 17:24:43.389281 hypua2jamo-0.6/src/hypua2jamo/
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     2050 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo/__init__.py
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)    12905 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo/_cython.pyx
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)   357646 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo/_cython2.c
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)   357645 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo/_cython3.c
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     3340 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo/c2d.bin
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     5039 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo/cli.py
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     3066 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo/d2c.bin
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)    12810 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo/decoder.py
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     8687 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo/encoder.py
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)    35610 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo/jc2p.bin
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)    39114 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo/jd2p.bin
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)    41038 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo/p2jc.bin
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)    53472 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo/p2jd.bin
-drwxr-xr-x   0 yoosung   (1000) yoosung   (1000)        0 2023-04-01 17:24:43.397281 hypua2jamo-0.6/src/hypua2jamo-c/
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      553 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/CMakeLists.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)    28689 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/c2d-table.h
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     1570 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/c2d.cpp
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      216 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/config.h.in
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)   130552 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/d2c-tree.inc
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     1582 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/d2c.c
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     3066 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/hypua2jamo.h
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)  1645658 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/jc2p-tree.inc
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     1592 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/jc2p.c
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)  2180002 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/jd2p-tree.inc
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     1609 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/jd2p.c
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     5713 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/jx2p.cpp
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     1327 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/jx2p.h
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)   493061 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/p2jc-table.h
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     1581 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/p2jc.cpp
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)   542797 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/p2jd-table.h
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     1601 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo-c/p2jd.cpp
-drwxr-xr-x   0 yoosung   (1000) yoosung   (1000)        0 2023-04-01 17:24:43.397281 hypua2jamo-0.6/src/hypua2jamo.egg-info/
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     4597 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo.egg-info/PKG-INFO
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)     1742 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo.egg-info/SOURCES.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)        1 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo.egg-info/dependency_links.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)       51 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo.egg-info/entry_points.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)        1 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo.egg-info/not-zip-safe
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)       12 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo.egg-info/requires.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)       11 2023-04-01 17:24:43.000000 hypua2jamo-0.6/src/hypua2jamo.egg-info/top_level.txt
--rw-r--r--   0 yoosung   (1000) yoosung   (1000)      610 2023-04-01 17:24:43.000000 hypua2jamo-0.6/tox.ini
+drwxr-xr-x   0 mete0r    (1000) mete0r    (1000)        0 2023-05-21 20:12:17.831461 hypua2jamo-0.7/
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      309 2023-05-21 20:12:16.000000 hypua2jamo-0.7/.coveragerc
+-rwxr-xr-x   0 mete0r    (1000) mete0r    (1000)     2218 2023-05-21 20:12:16.000000 hypua2jamo-0.7/.manylinux-install.sh
+-rwxr-xr-x   0 mete0r    (1000) mete0r    (1000)      608 2023-05-21 20:12:16.000000 hypua2jamo-0.7/.manylinux.sh
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      918 2023-05-21 20:12:16.000000 hypua2jamo-0.7/CHANGES.rst
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)    35147 2023-05-21 20:12:16.000000 hypua2jamo-0.7/COPYING
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     7651 2023-05-21 20:12:16.000000 hypua2jamo-0.7/COPYING.LESSER
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     1450 2023-05-21 20:12:16.000000 hypua2jamo-0.7/MANIFEST.in
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     4213 2023-05-21 20:12:16.000000 hypua2jamo-0.7/Makefile
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     4669 2023-05-21 20:12:17.831461 hypua2jamo-0.7/PKG-INFO
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     2452 2023-05-21 20:12:16.000000 hypua2jamo-0.7/README.rst
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     2588 2023-05-21 20:12:16.000000 hypua2jamo-0.7/appveyor.yml
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     6219 2023-05-21 20:12:16.000000 hypua2jamo-0.7/benchmark.py
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)       86 2023-05-21 20:12:16.000000 hypua2jamo-0.7/buildout.cfg
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      263 2023-05-21 20:12:16.000000 hypua2jamo-0.7/ccompiler-vc90.cmd
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      256 2023-05-21 20:12:16.000000 hypua2jamo-0.7/ccompiler-vs2019.cmd
+drwxr-xr-x   0 mete0r    (1000) mete0r    (1000)        0 2023-05-21 20:12:17.807460 hypua2jamo-0.7/docs/
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      588 2023-05-21 20:12:16.000000 hypua2jamo-0.7/docs/Makefile
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     6015 2023-05-21 20:12:16.000000 hypua2jamo-0.7/docs/conf.py
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      125 2023-05-21 20:12:16.000000 hypua2jamo-0.7/docs/hypua2jamo-cli.rst
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      587 2023-05-21 20:12:16.000000 hypua2jamo-0.7/docs/hypua2jamo.rst
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      476 2023-05-21 20:12:16.000000 hypua2jamo-0.7/docs/index.rst
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)       27 2023-05-21 20:12:16.000000 hypua2jamo-0.7/docs/intro.rst
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      756 2023-05-21 20:12:16.000000 hypua2jamo-0.7/docs/make.bat
+drwxr-xr-x   0 mete0r    (1000) mete0r    (1000)        0 2023-05-21 20:12:17.807460 hypua2jamo-0.7/examples/
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      109 2023-05-21 20:12:16.000000 hypua2jamo-0.7/examples/HunMinPreface.hypua.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      142 2023-05-21 20:12:16.000000 hypua2jamo-0.7/examples/HunMinPreface.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     4109 2023-05-21 20:12:16.000000 hypua2jamo-0.7/hypua2jamo_build.py
+drwxr-xr-x   0 mete0r    (1000) mete0r    (1000)        0 2023-05-21 20:12:17.811460 hypua2jamo-0.7/requirements/
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      269 2023-05-21 20:12:16.000000 hypua2jamo-0.7/requirements/dev.in
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     9777 2023-05-21 20:12:16.000000 hypua2jamo-0.7/requirements/dev.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      130 2023-05-21 20:12:16.000000 hypua2jamo-0.7/requirements/docs.in
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     1721 2023-05-21 20:12:16.000000 hypua2jamo-0.7/requirements/docs.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)       53 2023-05-21 20:12:16.000000 hypua2jamo-0.7/requirements/lint.in
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     1119 2023-05-21 20:12:16.000000 hypua2jamo-0.7/requirements/lint.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)       14 2023-05-21 20:12:16.000000 hypua2jamo-0.7/requirements/setup.in
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)        0 2023-05-21 20:12:16.000000 hypua2jamo-0.7/requirements/site.in
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      257 2023-05-21 20:12:16.000000 hypua2jamo-0.7/requirements/site.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)       37 2023-05-21 20:12:16.000000 hypua2jamo-0.7/requirements/test.in
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      400 2023-05-21 20:12:16.000000 hypua2jamo-0.7/requirements/test.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)       14 2023-05-21 20:12:16.000000 hypua2jamo-0.7/requirements.in
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      231 2023-05-21 20:12:16.000000 hypua2jamo-0.7/requirements.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      229 2023-05-21 20:12:17.835461 hypua2jamo-0.7/setup.cfg
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     7526 2023-05-21 20:12:16.000000 hypua2jamo-0.7/setup.py
+drwxr-xr-x   0 mete0r    (1000) mete0r    (1000)        0 2023-05-21 20:12:17.795460 hypua2jamo-0.7/src/
+drwxr-xr-x   0 mete0r    (1000) mete0r    (1000)        0 2023-05-21 20:12:17.815461 hypua2jamo-0.7/src/hypua2jamo/
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     2050 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo/__init__.py
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)    12905 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo/_cython.pyx
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)   357685 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo/_cython2.c
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)   357684 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo/_cython3.c
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     3340 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo/c2d.bin
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     5026 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo/cli.py
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     3066 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo/d2c.bin
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)    12810 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo/decoder.py
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     8687 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo/encoder.py
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)    35610 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo/jc2p.bin
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)    39114 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo/jd2p.bin
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)    41038 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo/p2jc.bin
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)    53472 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo/p2jd.bin
+drwxr-xr-x   0 mete0r    (1000) mete0r    (1000)        0 2023-05-21 20:12:17.831461 hypua2jamo-0.7/src/hypua2jamo-c/
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      553 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/CMakeLists.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)    28689 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/c2d-table.h
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     1570 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/c2d.cpp
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      216 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/config.h.in
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)   130552 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/d2c-tree.inc
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     1582 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/d2c.c
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     3066 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/hypua2jamo.h
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)  1645658 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/jc2p-tree.inc
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     1592 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/jc2p.c
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)  2180002 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/jd2p-tree.inc
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     1609 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/jd2p.c
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     5713 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/jx2p.cpp
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     1327 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/jx2p.h
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)   493061 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/p2jc-table.h
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     1581 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/p2jc.cpp
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)   542797 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/p2jd-table.h
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     1601 2023-05-21 20:12:16.000000 hypua2jamo-0.7/src/hypua2jamo-c/p2jd.cpp
+drwxr-xr-x   0 mete0r    (1000) mete0r    (1000)        0 2023-05-21 20:12:17.831461 hypua2jamo-0.7/src/hypua2jamo.egg-info/
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     4669 2023-05-21 20:12:17.000000 hypua2jamo-0.7/src/hypua2jamo.egg-info/PKG-INFO
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)     1742 2023-05-21 20:12:17.000000 hypua2jamo-0.7/src/hypua2jamo.egg-info/SOURCES.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)        1 2023-05-21 20:12:17.000000 hypua2jamo-0.7/src/hypua2jamo.egg-info/dependency_links.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)       51 2023-05-21 20:12:17.000000 hypua2jamo-0.7/src/hypua2jamo.egg-info/entry_points.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)        1 2023-05-21 20:12:17.000000 hypua2jamo-0.7/src/hypua2jamo.egg-info/not-zip-safe
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)       12 2023-05-21 20:12:17.000000 hypua2jamo-0.7/src/hypua2jamo.egg-info/requires.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)       11 2023-05-21 20:12:17.000000 hypua2jamo-0.7/src/hypua2jamo.egg-info/top_level.txt
+-rw-r--r--   0 mete0r    (1000) mete0r    (1000)      638 2023-05-21 20:12:16.000000 hypua2jamo-0.7/tox.ini
```

### Comparing `hypua2jamo-0.6/.manylinux-install.sh` & `hypua2jamo-0.7/.manylinux-install.sh`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/.manylinux.sh` & `hypua2jamo-0.7/.manylinux.sh`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/CHANGES.rst` & `hypua2jamo-0.7/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changes
 =======
 
+0.7 (2023-05-22)
+----------------
+
+- Fix `hypua2jamo` script to work.
+
+
 0.6 (2023-04-02)
 ----------------
 
 - Build Win64 wheels.
 - Add support for Python 3.9 / 3.10 / 3.11
 - Drop support for Python 3.5 / Python 3.6
```

### Comparing `hypua2jamo-0.6/COPYING` & `hypua2jamo-0.7/COPYING`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/COPYING.LESSER` & `hypua2jamo-0.7/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/MANIFEST.in` & `hypua2jamo-0.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/Makefile` & `hypua2jamo-0.7/Makefile`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/PKG-INFO` & `hypua2jamo-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypua2jamo
-Version: 0.6
+Version: 0.7
 Summary: Convert Hanyang-PUA code to unicode Hangul Jamo, i.e., Syllable-Initial-Peak-Final Encoding (첫가끝 코드).
 Home-page: https://github.com/mete0r/hypua2jamo
 Author: mete0r
 Author-email: 137794+mete0r@users.noreply.github.com
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: Hanyang,PUA,Unicode,Syllable-Initial-Peak-Final Encoding
 Classifier: Development Status :: 5 - Production/Stable
@@ -102,14 +102,20 @@
 
 This work is based on `KTUG <http://www.ktug.or.kr>`_
 `Hanyang PUA Table Project <http://faq.ktug.or.kr/faq/HanyangPuaTableProject>`_.
 
 Changes
 =======
 
+0.7 (2023-05-22)
+----------------
+
+- Fix `hypua2jamo` script to work.
+
+
 0.6 (2023-04-02)
 ----------------
 
 - Build Win64 wheels.
 - Add support for Python 3.9 / 3.10 / 3.11
 - Drop support for Python 3.5 / Python 3.6
```

### Comparing `hypua2jamo-0.6/README.rst` & `hypua2jamo-0.7/README.rst`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/appveyor.yml` & `hypua2jamo-0.7/appveyor.yml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   - Visual Studio 2015
   - Visual Studio 2019
 
 branches:
   only:
     - master
     - develop
-    - /\d+\.\d+\.\d+/
+    - /\d+\.\d+(\.\d+)?/
 
 clone_folder: c:\projects\hypua2jamo
 
 max_jobs: 2
 
 environment:
 
@@ -110,10 +110,10 @@
       "C:\\Python%python%\\python" -m coverage run --parallel -m unittest discover tests
 
 artifacts:
   - path: 'dist\*.whl'
     name: wheel
 
 deploy_script:
-  - ps: if ($env:APPVEYOR_REPO_TAG -eq $TRUE) { pip install twine; twine upload dist/*.whl }
+  - ps: if ($env:APPVEYOR_REPO_TAG -eq $TRUE) { pip install twine; twine upload --skip-existing dist/*.whl }
 
 deploy: on
```

### Comparing `hypua2jamo-0.6/benchmark.py` & `hypua2jamo-0.7/benchmark.py`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/docs/Makefile` & `hypua2jamo-0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/docs/conf.py` & `hypua2jamo-0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/docs/hypua2jamo.rst` & `hypua2jamo-0.7/docs/hypua2jamo.rst`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/docs/make.bat` & `hypua2jamo-0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/hypua2jamo_build.py` & `hypua2jamo-0.7/hypua2jamo_build.py`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/requirements/dev.txt` & `hypua2jamo-0.7/requirements/dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 alabaster==0.7.13
     # via
     #   -r requirements/docs.in
     #   sphinx
 anyio==3.6.2
     # via jupyter-server
-argcomplete==3.0.5
+argcomplete==3.0.8
     # via -r requirements/dev.in
 argon2-cffi==21.3.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 argon2-cffi-bindings==21.2.0
@@ -73,15 +73,15 @@
     # via -r requirements/dev.in
 comm==0.1.3
     # via ipykernel
 coverage==5.5
     # via -r requirements/test.in
 cryptography==40.0.1
     # via secretstorage
-cython==0.29.33
+cython==0.29.34
     # via -r requirements/dev.in
 debugpy==1.6.6
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
@@ -93,15 +93,15 @@
     #   readme-renderer
     #   restview
     #   sphinx
 executing==1.2.0
     # via stack-data
 fastjsonschema==2.16.3
     # via nbformat
-filelock==3.10.6
+filelock==3.11.0
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via -r requirements/lint.in
 fqdn==1.5.1
     # via jsonschema
@@ -217,17 +217,15 @@
 mccabe==0.7.0
     # via flake8
 mdurl==0.1.2
     # via markdown-it-py
 mistune==2.0.5
     # via nbconvert
 more-itertools==5.0.0
-    # via
-    #   -r requirements/test.in
-    #   jaraco-classes
+    # via jaraco-classes
 nbclassic==0.5.3
     # via notebook
 nbclient==0.7.2
     # via nbconvert
 nbconvert==7.2.10
     # via
     #   jupyter
@@ -242,21 +240,21 @@
     #   nbconvert
     #   notebook
 nest-asyncio==1.5.6
     # via
     #   ipykernel
     #   nbclassic
     #   notebook
-notebook==6.5.3
+notebook==6.5.4
     # via
     #   -r requirements/dev.in
     #   jupyter
 notebook-shim==0.2.2
     # via nbclassic
-packaging==23.0
+packaging==23.1
     # via
     #   build
     #   ipykernel
     #   jupyter-server
     #   nbconvert
     #   pyproject-api
     #   pyroma
@@ -272,15 +270,15 @@
     #   ktug-hanyang-pua
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pip-tools==6.12.3
+pip-tools==6.13.0
     # via -r requirements/dev.in
 pkginfo==1.9.6
     # via twine
 platformdirs==3.2.0
     # via
     #   jupyter-core
     #   tox
@@ -396,15 +394,15 @@
     #   rfc3339-validator
 sniffio==1.3.0
     # via anyio
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.4
     # via beautifulsoup4
-sphinx==6.1.3
+sphinx==7.0.1
     # via
     #   -r requirements/docs.in
     #   repoze-sphinx-autointerface
     #   sphinx-argparse
     #   sphinx-intl
 sphinx-argparse==0.4.0
     # via -r requirements/docs.in
@@ -443,15 +441,15 @@
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
-tox==4.4.8
+tox==4.5.1
     # via -r requirements/dev.in
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
```

### Comparing `hypua2jamo-0.6/requirements/docs.txt` & `hypua2jamo-0.7/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/requirements/lint.txt` & `hypua2jamo-0.7/requirements/lint.txt`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/setup.py` & `hypua2jamo-0.7/setup.py`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo/__init__.py` & `hypua2jamo-0.7/src/hypua2jamo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with hypua2jamo.  If not, see <http://www.gnu.org/licenses/>.
 import sys
 import logging
 
 
-__version__ = '0.6'
+__version__ = '0.7'
 
 
 logger = logging.getLogger(__name__)
 jython = sys.platform.startswith('java')
 if sys.version >= '3':
     unichr = chr
```

### Comparing `hypua2jamo-0.6/src/hypua2jamo/_cython.pyx` & `hypua2jamo-0.7/src/hypua2jamo/_cython.pyx`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo/_cython2.c` & `hypua2jamo-0.7/src/hypua2jamo/_cython2.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -83,15 +83,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -199,15 +199,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +238,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -548,35 +548,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1375,26 +1375,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -5762,15 +5762,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -6093,15 +6093,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_hypua2jamo___cython) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -6736,28 +6736,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -7343,15 +7343,15 @@
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `hypua2jamo-0.6/src/hypua2jamo/_cython3.c` & `hypua2jamo-0.7/src/hypua2jamo/_cython3.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -83,15 +83,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -199,15 +199,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +238,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -548,35 +548,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1375,26 +1375,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -5762,15 +5762,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -6093,15 +6093,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_hypua2jamo___cython) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -6736,28 +6736,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -7343,15 +7343,15 @@
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `hypua2jamo-0.6/src/hypua2jamo/c2d.bin` & `hypua2jamo-0.7/src/hypua2jamo/c2d.bin`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo/cli.py` & `hypua2jamo-0.7/src/hypua2jamo/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,30 +111,31 @@
     try:
         translate = translator.encode
     except AttributeError:
         translate = translator.decode
 
     with io.open(args.FILE, 'r', encoding='utf-8') as fp:
         for encoded in (translate(line) for line in fp):
-            sys.stdout.write(encoded.encode('utf-8'))
+            sys.stdout.write(encoded)
         encoded = translate('', final=True)
-        sys.stdout.write(encoded.encode('utf-8'))
+        sys.stdout.write(encoded)
 
 
 def main_argparse():
     parser = ArgumentParser()
     parser.add_argument(
         '--version',
         action='version',
         version='%(prog)s {}'.format(__version__),
         help=_('output version information and exit')
     )
     parser.add_argument(
         '-v', '--verbose',
         action='count',
+        default=0,
         help=_('increase verbosity')
     )
     parser.add_argument(
         '-s', '--source',
         action='store',
         help=_('source encoding (composed, decomposed, PUA)'),
     )
```

### Comparing `hypua2jamo-0.6/src/hypua2jamo/d2c.bin` & `hypua2jamo-0.7/src/hypua2jamo/d2c.bin`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo/decoder.py` & `hypua2jamo-0.7/src/hypua2jamo/decoder.py`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo/encoder.py` & `hypua2jamo-0.7/src/hypua2jamo/encoder.py`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo/jc2p.bin` & `hypua2jamo-0.7/src/hypua2jamo/jc2p.bin`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo/jd2p.bin` & `hypua2jamo-0.7/src/hypua2jamo/jd2p.bin`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo/p2jc.bin` & `hypua2jamo-0.7/src/hypua2jamo/p2jc.bin`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo/p2jd.bin` & `hypua2jamo-0.7/src/hypua2jamo/p2jd.bin`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/CMakeLists.txt` & `hypua2jamo-0.7/src/hypua2jamo-c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/c2d-table.h` & `hypua2jamo-0.7/src/hypua2jamo-c/c2d-table.h`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/c2d.cpp` & `hypua2jamo-0.7/src/hypua2jamo-c/c2d.cpp`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/d2c-tree.inc` & `hypua2jamo-0.7/src/hypua2jamo-c/d2c-tree.inc`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/d2c.c` & `hypua2jamo-0.7/src/hypua2jamo-c/d2c.c`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/hypua2jamo.h` & `hypua2jamo-0.7/src/hypua2jamo-c/hypua2jamo.h`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/jc2p-tree.inc` & `hypua2jamo-0.7/src/hypua2jamo-c/jc2p-tree.inc`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/jc2p.c` & `hypua2jamo-0.7/src/hypua2jamo-c/jc2p.c`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/jd2p-tree.inc` & `hypua2jamo-0.7/src/hypua2jamo-c/jd2p-tree.inc`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/jd2p.c` & `hypua2jamo-0.7/src/hypua2jamo-c/jd2p.c`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/jx2p.cpp` & `hypua2jamo-0.7/src/hypua2jamo-c/jx2p.cpp`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/jx2p.h` & `hypua2jamo-0.7/src/hypua2jamo-c/jx2p.h`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/p2jc-table.h` & `hypua2jamo-0.7/src/hypua2jamo-c/p2jc-table.h`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/p2jc.cpp` & `hypua2jamo-0.7/src/hypua2jamo-c/p2jc.cpp`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/p2jd-table.h` & `hypua2jamo-0.7/src/hypua2jamo-c/p2jd-table.h`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo-c/p2jd.cpp` & `hypua2jamo-0.7/src/hypua2jamo-c/p2jd.cpp`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/src/hypua2jamo.egg-info/PKG-INFO` & `hypua2jamo-0.7/src/hypua2jamo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypua2jamo
-Version: 0.6
+Version: 0.7
 Summary: Convert Hanyang-PUA code to unicode Hangul Jamo, i.e., Syllable-Initial-Peak-Final Encoding (첫가끝 코드).
 Home-page: https://github.com/mete0r/hypua2jamo
 Author: mete0r
 Author-email: 137794+mete0r@users.noreply.github.com
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: Hanyang,PUA,Unicode,Syllable-Initial-Peak-Final Encoding
 Classifier: Development Status :: 5 - Production/Stable
@@ -102,14 +102,20 @@
 
 This work is based on `KTUG <http://www.ktug.or.kr>`_
 `Hanyang PUA Table Project <http://faq.ktug.or.kr/faq/HanyangPuaTableProject>`_.
 
 Changes
 =======
 
+0.7 (2023-05-22)
+----------------
+
+- Fix `hypua2jamo` script to work.
+
+
 0.6 (2023-04-02)
 ----------------
 
 - Build Win64 wheels.
 - Add support for Python 3.9 / 3.10 / 3.11
 - Drop support for Python 3.5 / Python 3.6
```

### Comparing `hypua2jamo-0.6/src/hypua2jamo.egg-info/SOURCES.txt` & `hypua2jamo-0.7/src/hypua2jamo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypua2jamo-0.6/tox.ini` & `hypua2jamo-0.7/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 [testenv:docs]
 skip_install =
 	true
 deps =
 	-r{toxinidir}/requirements/docs.txt
 changedir = {toxinidir}
+allowlist_externals =
+	make
 whitelist_externals =
 	make
 commands =
 	make -C docs html latexpdf
 
 
 [testenv:lint]
```

