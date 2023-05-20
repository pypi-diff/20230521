# Comparing `tmp/llfuse-1.4.3.tar.gz` & `tmp/llfuse-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llfuse-1.4.3.tar", last modified: Tue May  9 13:15:14 2023, max compression
+gzip compressed data, was "llfuse-1.4.4.tar", last modified: Sat May 20 22:58:04 2023, max compression
```

## Comparing `llfuse-1.4.3.tar` & `llfuse-1.4.4.tar`

### file list

```diff
@@ -1,86 +1,85 @@
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.733315 llfuse-1.4.3/
--rw-r--r--   0 tw         (501) staff       (20)    13140 2023-05-09 13:10:13.000000 llfuse-1.4.3/Changes.rst
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.716790 llfuse-1.4.3/Include/
--rw-r--r--   0 tw         (501) staff       (20)     1839 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/fuse_common.pxd
--rw-r--r--   0 tw         (501) staff       (20)     7987 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/fuse_lowlevel.pxd
--rw-r--r--   0 tw         (501) staff       (20)      393 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/fuse_opt.pxd
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.717403 llfuse-1.4.3/Include/libc/
--rw-r--r--   0 tw         (501) staff       (20)       13 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/libc/__init__.py
--rw-r--r--   0 tw         (501) staff       (20)      546 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/libc/dirent.pxd
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.717848 llfuse-1.4.3/Include/libc/sys/
--rw-r--r--   0 tw         (501) staff       (20)       13 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/libc/sys/__init__.py
--rw-r--r--   0 tw         (501) staff       (20)      627 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/libc/sys/statvfs.pxd
--rw-r--r--   0 tw         (501) staff       (20)     1783 2022-05-16 19:57:28.000000 llfuse-1.4.3/Include/pthread.pxd
--rw-r--r--   0 tw         (501) staff       (20)    25960 2022-05-16 19:57:28.000000 llfuse-1.4.3/LICENSE
--rw-r--r--   0 tw         (501) staff       (20)     2881 2023-05-09 13:15:14.733403 llfuse-1.4.3/PKG-INFO
--rw-r--r--   0 tw         (501) staff       (20)     1626 2023-05-09 10:54:10.000000 llfuse-1.4.3/README.rst
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.718644 llfuse-1.4.3/examples/
--rwxr-xr-x   0 tw         (501) staff       (20)     5071 2022-05-16 19:57:28.000000 llfuse-1.4.3/examples/lltest.py
--rwxr-xr-x   0 tw         (501) staff       (20)    16688 2022-05-16 19:57:28.000000 llfuse-1.4.3/examples/passthroughfs.py
--rwxr-xr-x   0 tw         (501) staff       (20)    15838 2022-05-16 19:57:28.000000 llfuse-1.4.3/examples/tmpfs.py
--rw-r--r--   0 tw         (501) staff       (20)       81 2023-05-09 12:56:19.000000 llfuse-1.4.3/pyproject.toml
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.721472 llfuse-1.4.3/rst/
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.721658 llfuse-1.4.3/rst/_static/
--rw-r--r--   0 tw         (501) staff       (20)        0 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/_static/.placeholder
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.721799 llfuse-1.4.3/rst/_templates/
--rw-r--r--   0 tw         (501) staff       (20)       93 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/_templates/localtoc.html
--rw-r--r--   0 tw         (501) staff       (20)       80 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/about.rst
--rw-r--r--   0 tw         (501) staff       (20)       28 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/changes.rst
--rw-r--r--   0 tw         (501) staff       (20)     6947 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/conf.py
--rw-r--r--   0 tw         (501) staff       (20)     2927 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/data.rst
--rw-r--r--   0 tw         (501) staff       (20)      816 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/example.rst
--rw-r--r--   0 tw         (501) staff       (20)      327 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/fuse_api.rst
--rw-r--r--   0 tw         (501) staff       (20)     3226 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/general.rst
--rw-r--r--   0 tw         (501) staff       (20)      868 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/gotchas.rst
--rw-r--r--   0 tw         (501) staff       (20)      409 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/index.rst
--rw-r--r--   0 tw         (501) staff       (20)     2821 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/install.rst
--rw-r--r--   0 tw         (501) staff       (20)     2048 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/lock.rst
--rw-r--r--   0 tw         (501) staff       (20)      198 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/operations.rst
--rw-r--r--   0 tw         (501) staff       (20)      381 2022-05-16 19:57:28.000000 llfuse-1.4.3/rst/util.rst
--rw-r--r--   0 tw         (501) staff       (20)       87 2023-05-09 13:15:14.733704 llfuse-1.4.3/setup.cfg
--rwxr-xr-x   0 tw         (501) staff       (20)     9886 2023-05-09 13:06:13.000000 llfuse-1.4.3/setup.py
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.728508 llfuse-1.4.3/src/
--rw-r--r--   0 tw         (501) staff       (20)     6145 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/darwin_compat.c
--rw-r--r--   0 tw         (501) staff       (20)     1376 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/darwin_compat.h
--rw-r--r--   0 tw         (501) staff       (20)    19430 2023-05-09 10:54:10.000000 llfuse-1.4.3/src/fuse_api.pxi
--rw-r--r--   0 tw         (501) staff       (20)      963 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/gettime.h
--rw-r--r--   0 tw         (501) staff       (20)    23731 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/handlers.pxi
--rw-r--r--   0 tw         (501) staff       (20)  2481650 2023-05-09 13:11:22.000000 llfuse-1.4.3/src/llfuse.c
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.729337 llfuse-1.4.3/src/llfuse.egg-info/
--rw-r--r--   0 tw         (501) staff       (20)     2881 2023-05-09 13:15:14.000000 llfuse-1.4.3/src/llfuse.egg-info/PKG-INFO
--rw-r--r--   0 tw         (501) staff       (20)     1385 2023-05-09 13:15:14.000000 llfuse-1.4.3/src/llfuse.egg-info/SOURCES.txt
--rw-r--r--   0 tw         (501) staff       (20)        1 2023-05-09 13:15:14.000000 llfuse-1.4.3/src/llfuse.egg-info/dependency_links.txt
--rw-r--r--   0 tw         (501) staff       (20)        7 2023-05-09 13:15:14.000000 llfuse-1.4.3/src/llfuse.egg-info/top_level.txt
--rw-r--r--   0 tw         (501) staff       (20)        1 2022-05-16 19:58:20.000000 llfuse-1.4.3/src/llfuse.egg-info/zip-safe
--rw-r--r--   0 tw         (501) staff       (20)      924 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/llfuse.h
--rw-r--r--   0 tw         (501) staff       (20)     4171 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/llfuse.pyx
--rw-r--r--   0 tw         (501) staff       (20)     3893 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/lock.c
--rw-r--r--   0 tw         (501) staff       (20)      383 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/lock.h
--rw-r--r--   0 tw         (501) staff       (20)     1940 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/macros.c
--rw-r--r--   0 tw         (501) staff       (20)    21374 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/misc.pxi
--rw-r--r--   0 tw         (501) staff       (20)    19987 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/operations.pxi
--rw-r--r--   0 tw         (501) staff       (20)     3500 2022-05-16 19:57:28.000000 llfuse-1.4.3/src/xattr.h
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.731336 llfuse-1.4.3/test/
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.731899 llfuse-1.4.3/test/.pytest_cache/
--rw-r--r--   0 tw         (501) staff       (20)       37 2022-05-16 20:44:06.000000 llfuse-1.4.3/test/.pytest_cache/.gitignore
--rw-r--r--   0 tw         (501) staff       (20)      191 2022-05-16 20:44:06.000000 llfuse-1.4.3/test/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 tw         (501) staff       (20)      302 2022-05-16 20:44:06.000000 llfuse-1.4.3/test/.pytest_cache/README.md
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.714216 llfuse-1.4.3/test/.pytest_cache/v/
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.732586 llfuse-1.4.3/test/.pytest_cache/v/cache/
--rw-r--r--   0 tw         (501) staff       (20)       88 2022-05-16 20:50:14.000000 llfuse-1.4.3/test/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 tw         (501) staff       (20)      525 2023-05-09 13:14:27.000000 llfuse-1.4.3/test/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 tw         (501) staff       (20)        2 2023-05-09 13:14:27.000000 llfuse-1.4.3/test/.pytest_cache/v/cache/stepwise
--rwxr-xr-x   0 tw         (501) staff       (20)       75 2023-05-09 12:56:19.000000 llfuse-1.4.3/test/ci-install.sh
--rwxr-xr-x   0 tw         (501) staff       (20)      139 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/ci-test.sh
--rw-r--r--   0 tw         (501) staff       (20)     3650 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/conftest.py
--rw-r--r--   0 tw         (501) staff       (20)       81 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/pytest.ini
--rw-r--r--   0 tw         (501) staff       (20)     3885 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/pytest_checklogs.py
--rwxr-xr-x   0 tw         (501) staff       (20)     2962 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/test_api.py
--rwxr-xr-x   0 tw         (501) staff       (20)    11770 2023-05-09 10:54:10.000000 llfuse-1.4.3/test/test_examples.py
--rwxr-xr-x   0 tw         (501) staff       (20)     8337 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/test_fs.py
--rwxr-xr-x   0 tw         (501) staff       (20)     1228 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/test_rounding.py
--rw-r--r--   0 tw         (501) staff       (20)     3691 2022-05-16 19:57:28.000000 llfuse-1.4.3/test/util.py
-drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-09 13:15:14.733141 llfuse-1.4.3/util/
--rwxr-xr-x   0 tw         (501) staff       (20)      307 2022-05-16 19:57:28.000000 llfuse-1.4.3/util/sdist-sign
--rw-r--r--   0 tw         (501) staff       (20)     1021 2022-05-16 19:57:28.000000 llfuse-1.4.3/util/sphinx_cython.py
--rwxr-xr-x   0 tw         (501) staff       (20)      277 2022-05-16 19:57:28.000000 llfuse-1.4.3/util/upload-pypi
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.657605 llfuse-1.4.4/
+-rw-r--r--   0 tw         (501) staff       (20)    13556 2023-05-20 11:35:58.000000 llfuse-1.4.4/Changes.rst
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.646671 llfuse-1.4.4/Include/
+-rw-r--r--   0 tw         (501) staff       (20)     1839 2022-05-16 19:57:28.000000 llfuse-1.4.4/Include/fuse_common.pxd
+-rw-r--r--   0 tw         (501) staff       (20)     7987 2022-05-16 19:57:28.000000 llfuse-1.4.4/Include/fuse_lowlevel.pxd
+-rw-r--r--   0 tw         (501) staff       (20)      393 2022-05-16 19:57:28.000000 llfuse-1.4.4/Include/fuse_opt.pxd
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.646915 llfuse-1.4.4/Include/libc/
+-rw-r--r--   0 tw         (501) staff       (20)       13 2022-05-16 19:57:28.000000 llfuse-1.4.4/Include/libc/__init__.py
+-rw-r--r--   0 tw         (501) staff       (20)      546 2022-05-16 19:57:28.000000 llfuse-1.4.4/Include/libc/dirent.pxd
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.647191 llfuse-1.4.4/Include/libc/sys/
+-rw-r--r--   0 tw         (501) staff       (20)       13 2022-05-16 19:57:28.000000 llfuse-1.4.4/Include/libc/sys/__init__.py
+-rw-r--r--   0 tw         (501) staff       (20)      627 2022-05-16 19:57:28.000000 llfuse-1.4.4/Include/libc/sys/statvfs.pxd
+-rw-r--r--   0 tw         (501) staff       (20)     1783 2022-05-16 19:57:28.000000 llfuse-1.4.4/Include/pthread.pxd
+-rw-r--r--   0 tw         (501) staff       (20)    25960 2022-05-16 19:57:28.000000 llfuse-1.4.4/LICENSE
+-rw-r--r--   0 tw         (501) staff       (20)     2881 2023-05-20 22:58:04.657669 llfuse-1.4.4/PKG-INFO
+-rw-r--r--   0 tw         (501) staff       (20)     1626 2023-05-09 10:54:10.000000 llfuse-1.4.4/README.rst
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.648025 llfuse-1.4.4/examples/
+-rwxr-xr-x   0 tw         (501) staff       (20)     5547 2023-05-20 11:25:46.000000 llfuse-1.4.4/examples/lltest.py
+-rwxr-xr-x   0 tw         (501) staff       (20)    16688 2022-05-16 19:57:28.000000 llfuse-1.4.4/examples/passthroughfs.py
+-rwxr-xr-x   0 tw         (501) staff       (20)    15948 2023-05-20 11:25:46.000000 llfuse-1.4.4/examples/tmpfs.py
+-rw-r--r--   0 tw         (501) staff       (20)       81 2023-05-09 12:56:19.000000 llfuse-1.4.4/pyproject.toml
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.649890 llfuse-1.4.4/rst/
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.650031 llfuse-1.4.4/rst/_static/
+-rw-r--r--   0 tw         (501) staff       (20)        0 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/_static/.placeholder
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.650133 llfuse-1.4.4/rst/_templates/
+-rw-r--r--   0 tw         (501) staff       (20)       93 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/_templates/localtoc.html
+-rw-r--r--   0 tw         (501) staff       (20)       80 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/about.rst
+-rw-r--r--   0 tw         (501) staff       (20)       28 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/changes.rst
+-rw-r--r--   0 tw         (501) staff       (20)     6947 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/conf.py
+-rw-r--r--   0 tw         (501) staff       (20)     2927 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/data.rst
+-rw-r--r--   0 tw         (501) staff       (20)      816 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/example.rst
+-rw-r--r--   0 tw         (501) staff       (20)      327 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/fuse_api.rst
+-rw-r--r--   0 tw         (501) staff       (20)     3226 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/general.rst
+-rw-r--r--   0 tw         (501) staff       (20)      868 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/gotchas.rst
+-rw-r--r--   0 tw         (501) staff       (20)      409 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/index.rst
+-rw-r--r--   0 tw         (501) staff       (20)     2821 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/install.rst
+-rw-r--r--   0 tw         (501) staff       (20)     2048 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/lock.rst
+-rw-r--r--   0 tw         (501) staff       (20)      198 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/operations.rst
+-rw-r--r--   0 tw         (501) staff       (20)      381 2022-05-16 19:57:28.000000 llfuse-1.4.4/rst/util.rst
+-rw-r--r--   0 tw         (501) staff       (20)       87 2023-05-20 22:58:04.657873 llfuse-1.4.4/setup.cfg
+-rwxr-xr-x   0 tw         (501) staff       (20)     9886 2023-05-20 11:27:40.000000 llfuse-1.4.4/setup.py
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.653764 llfuse-1.4.4/src/
+-rw-r--r--   0 tw         (501) staff       (20)     6145 2022-05-16 19:57:28.000000 llfuse-1.4.4/src/darwin_compat.c
+-rw-r--r--   0 tw         (501) staff       (20)     1376 2022-05-16 19:57:28.000000 llfuse-1.4.4/src/darwin_compat.h
+-rw-r--r--   0 tw         (501) staff       (20)    19451 2023-05-20 11:25:46.000000 llfuse-1.4.4/src/fuse_api.pxi
+-rw-r--r--   0 tw         (501) staff       (20)      963 2022-05-16 19:57:28.000000 llfuse-1.4.4/src/gettime.h
+-rw-r--r--   0 tw         (501) staff       (20)    23731 2022-05-16 19:57:28.000000 llfuse-1.4.4/src/handlers.pxi
+-rw-r--r--   0 tw         (501) staff       (20)  2481700 2023-05-20 22:54:42.000000 llfuse-1.4.4/src/llfuse.c
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.654363 llfuse-1.4.4/src/llfuse.egg-info/
+-rw-r--r--   0 tw         (501) staff       (20)     2881 2023-05-20 22:58:04.000000 llfuse-1.4.4/src/llfuse.egg-info/PKG-INFO
+-rw-r--r--   0 tw         (501) staff       (20)     1366 2023-05-20 22:58:04.000000 llfuse-1.4.4/src/llfuse.egg-info/SOURCES.txt
+-rw-r--r--   0 tw         (501) staff       (20)        1 2023-05-20 22:58:04.000000 llfuse-1.4.4/src/llfuse.egg-info/dependency_links.txt
+-rw-r--r--   0 tw         (501) staff       (20)        7 2023-05-20 22:58:04.000000 llfuse-1.4.4/src/llfuse.egg-info/top_level.txt
+-rw-r--r--   0 tw         (501) staff       (20)        1 2022-05-16 19:58:20.000000 llfuse-1.4.4/src/llfuse.egg-info/zip-safe
+-rw-r--r--   0 tw         (501) staff       (20)      924 2022-05-16 19:57:28.000000 llfuse-1.4.4/src/llfuse.h
+-rw-r--r--   0 tw         (501) staff       (20)     4171 2022-05-16 19:57:28.000000 llfuse-1.4.4/src/llfuse.pyx
+-rw-r--r--   0 tw         (501) staff       (20)     3893 2022-05-16 19:57:28.000000 llfuse-1.4.4/src/lock.c
+-rw-r--r--   0 tw         (501) staff       (20)      383 2022-05-16 19:57:28.000000 llfuse-1.4.4/src/lock.h
+-rw-r--r--   0 tw         (501) staff       (20)     1940 2022-05-16 19:57:28.000000 llfuse-1.4.4/src/macros.c
+-rw-r--r--   0 tw         (501) staff       (20)    21392 2023-05-20 11:25:46.000000 llfuse-1.4.4/src/misc.pxi
+-rw-r--r--   0 tw         (501) staff       (20)    19987 2022-05-16 19:57:28.000000 llfuse-1.4.4/src/operations.pxi
+-rw-r--r--   0 tw         (501) staff       (20)     3500 2022-05-16 19:57:28.000000 llfuse-1.4.4/src/xattr.h
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.655831 llfuse-1.4.4/test/
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.656337 llfuse-1.4.4/test/.pytest_cache/
+-rw-r--r--   0 tw         (501) staff       (20)       37 2022-05-16 20:44:06.000000 llfuse-1.4.4/test/.pytest_cache/.gitignore
+-rw-r--r--   0 tw         (501) staff       (20)      191 2022-05-16 20:44:06.000000 llfuse-1.4.4/test/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 tw         (501) staff       (20)      302 2022-05-16 20:44:06.000000 llfuse-1.4.4/test/.pytest_cache/README.md
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.645103 llfuse-1.4.4/test/.pytest_cache/v/
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.657024 llfuse-1.4.4/test/.pytest_cache/v/cache/
+-rw-r--r--   0 tw         (501) staff       (20)       87 2023-05-14 13:03:17.000000 llfuse-1.4.4/test/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 tw         (501) staff       (20)      525 2023-05-14 13:52:54.000000 llfuse-1.4.4/test/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 tw         (501) staff       (20)        2 2023-05-14 13:52:54.000000 llfuse-1.4.4/test/.pytest_cache/v/cache/stepwise
+-rwxr-xr-x   0 tw         (501) staff       (20)      139 2022-05-16 19:57:28.000000 llfuse-1.4.4/test/ci-test.sh
+-rw-r--r--   0 tw         (501) staff       (20)     3650 2022-05-16 19:57:28.000000 llfuse-1.4.4/test/conftest.py
+-rw-r--r--   0 tw         (501) staff       (20)       81 2022-05-16 19:57:28.000000 llfuse-1.4.4/test/pytest.ini
+-rw-r--r--   0 tw         (501) staff       (20)     3885 2022-05-16 19:57:28.000000 llfuse-1.4.4/test/pytest_checklogs.py
+-rwxr-xr-x   0 tw         (501) staff       (20)     2962 2022-05-16 19:57:28.000000 llfuse-1.4.4/test/test_api.py
+-rwxr-xr-x   0 tw         (501) staff       (20)    11770 2023-05-14 13:29:15.000000 llfuse-1.4.4/test/test_examples.py
+-rwxr-xr-x   0 tw         (501) staff       (20)     8337 2022-05-16 19:57:28.000000 llfuse-1.4.4/test/test_fs.py
+-rwxr-xr-x   0 tw         (501) staff       (20)     1228 2022-05-16 19:57:28.000000 llfuse-1.4.4/test/test_rounding.py
+-rw-r--r--   0 tw         (501) staff       (20)     3443 2023-05-20 11:25:46.000000 llfuse-1.4.4/test/util.py
+drwxr-xr-x   0 tw         (501) staff       (20)        0 2023-05-20 22:58:04.657468 llfuse-1.4.4/util/
+-rwxr-xr-x   0 tw         (501) staff       (20)      307 2022-05-16 19:57:28.000000 llfuse-1.4.4/util/sdist-sign
+-rw-r--r--   0 tw         (501) staff       (20)     1021 2022-05-16 19:57:28.000000 llfuse-1.4.4/util/sphinx_cython.py
+-rwxr-xr-x   0 tw         (501) staff       (20)      277 2022-05-16 19:57:28.000000 llfuse-1.4.4/util/upload-pypi
```

### Comparing `llfuse-1.4.3/Changes.rst` & `llfuse-1.4.4/Changes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,24 @@
  Changelog
 ===========
 
 .. currentmodule:: llfuse
 
 **WARNING**: Python-LLFUSE is no longer actively developed.
 
+Release 1.4.4 (2023-05-21)
+==========================
+
+- CI: use the matrix for cy/py combinations, support and test on Cython 3 beta
+- cy3: cdef void* f(void* d) noexcept with gil, #78
+- cy3: cdef nogil -> noexcept nogil
+- tests: use shutil.which() instead of which(1) executable
+- tests/examples: fix tmpfs: backport fix from pyfuse3
+- tests/examples: fix lltest: add statfs implementation, remove -l from umount
+
 Release 1.4.3 (2023-05-09)
 ==========================
 
 * cythonize with Cython 0.29.34 (brings python 3.12 support)
 * also test on python 3.12-dev
 * add a minimal pyproject.toml, #70
 * fix basedir in setup.py (malfunctioned with pip install -e .)
```

### Comparing `llfuse-1.4.3/Include/fuse_common.pxd` & `llfuse-1.4.4/Include/fuse_common.pxd`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/Include/fuse_lowlevel.pxd` & `llfuse-1.4.4/Include/fuse_lowlevel.pxd`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/Include/libc/dirent.pxd` & `llfuse-1.4.4/Include/libc/dirent.pxd`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/Include/libc/sys/statvfs.pxd` & `llfuse-1.4.4/Include/libc/sys/statvfs.pxd`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/Include/pthread.pxd` & `llfuse-1.4.4/Include/pthread.pxd`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/LICENSE` & `llfuse-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/PKG-INFO` & `llfuse-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llfuse
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python bindings for the low-level FUSE API
 Home-page: https://github.com/python-llfuse/python-llfuse/
 Author: Nikolaus Rath
 Author-email: Nikolaus@rath.org
 License: LGPL
 Keywords: FUSE,python
 Platform: Linux
```

### Comparing `llfuse-1.4.3/README.rst` & `llfuse-1.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/examples/lltest.py` & `llfuse-1.4.4/examples/lltest.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,15 +87,33 @@
         return inode
 
     def readdir(self, fh, off):
         assert fh == llfuse.ROOT_INODE
 
         # only one entry
         if off == 0:
-            yield (self.hello_name, self.getattr(self.hello_inode), 1)
+            yield (self.hello_name, self.getattr(self.hello_inode), self.hello_inode)
+
+    def statfs(self, ctx):
+        stat_ = llfuse.StatvfsData()
+
+        stat_.f_bsize = 512
+        stat_.f_frsize = 512
+
+        size = 1024 * stat_.f_frsize
+        stat_.f_blocks = size // stat_.f_frsize
+        stat_.f_bfree = max(size // stat_.f_frsize, 1024)
+        stat_.f_bavail = stat_.f_bfree
+
+        inodes = 100
+        stat_.f_files = inodes
+        stat_.f_ffree = max(inodes, 100)
+        stat_.f_favail = stat_.f_ffree
+
+        return stat_
 
     def open(self, inode, flags, ctx):
         if inode != self.hello_inode:
             raise llfuse.FUSEError(errno.ENOENT)
         if flags & os.O_RDWR or flags & os.O_WRONLY:
             raise llfuse.FUSEError(errno.EACCES)
         return inode
```

### Comparing `llfuse-1.4.3/examples/passthroughfs.py` & `llfuse-1.4.4/examples/passthroughfs.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/examples/tmpfs.py` & `llfuse-1.4.4/examples/tmpfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,18 @@
             except NoSuchRowError:
                 raise(llfuse.FUSEError(errno.ENOENT))
 
         return self.getattr(inode, ctx)
 
 
     def getattr(self, inode, ctx=None):
-        row = self.get_row('SELECT * FROM inodes WHERE id=?', (inode,))
+        try:
+            row = self.get_row('SELECT * FROM inodes WHERE id=?', (inode,))
+        except NoSuchRowError:
+            raise(llfuse.FUSEError(errno.ENOENT))
 
         entry = llfuse.EntryAttributes()
         entry.st_ino = inode
         entry.generation = 0
         entry.entry_timeout = 300
         entry.attr_timeout = 300
         entry.st_mode = row['mode']
@@ -254,16 +257,16 @@
         if entry_new.st_nlink == 1 and entry_new.st_ino not in self.inode_open_count:
             self.cursor.execute("DELETE FROM inodes WHERE id=?", (entry_new.st_ino,))
 
 
     def link(self, inode, new_inode_p, new_name, ctx):
         entry_p = self.getattr(new_inode_p)
         if entry_p.st_nlink == 0:
-            log.warn('Attempted to create entry %s with unlinked parent %d',
-                     new_name, new_inode_p)
+            log.warning('Attempted to create entry %s with unlinked parent %d',
+                        new_name, new_inode_p)
             raise FUSEError(errno.EINVAL)
 
         self.cursor.execute("INSERT INTO contents (name, inode, parent_inode) VALUES(?,?,?)",
                             (new_name, inode, new_inode_p))
 
         return self.getattr(inode)
 
@@ -342,16 +345,16 @@
         #pylint: disable=W0612
         entry = self._create(inode_parent, name, mode, ctx)
         self.inode_open_count[entry.st_ino] += 1
         return (entry.st_ino, entry)
 
     def _create(self, inode_p, name, mode, ctx, rdev=0, target=None):
         if self.getattr(inode_p).st_nlink == 0:
-            log.warn('Attempted to create entry %s with unlinked parent %d',
-                     name, inode_p)
+            log.warning('Attempted to create entry %s with unlinked parent %d',
+                        name, inode_p)
             raise FUSEError(errno.EINVAL)
 
         now_ns = int(time() * 1e9)
         self.cursor.execute('INSERT INTO inodes (uid, gid, mode, mtime_ns, atime_ns, '
                             'ctime_ns, target, rdev) VALUES(?, ?, ?, ?, ?, ?, ?, ?)',
                             (ctx.uid, ctx.gid, mode, now_ns, now_ns, now_ns, target, rdev))
```

### Comparing `llfuse-1.4.3/rst/conf.py` & `llfuse-1.4.4/rst/conf.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/rst/data.rst` & `llfuse-1.4.4/rst/data.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/rst/example.rst` & `llfuse-1.4.4/rst/example.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/rst/general.rst` & `llfuse-1.4.4/rst/general.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/rst/gotchas.rst` & `llfuse-1.4.4/rst/gotchas.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/rst/install.rst` & `llfuse-1.4.4/rst/install.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/rst/lock.rst` & `llfuse-1.4.4/rst/lock.rst`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/setup.py` & `llfuse-1.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     # DeprecationWarning.
     warnings.simplefilter('default')
 
 # Add src to load path, important for Sphinx autodoc
 # to work properly
 sys.path.insert(0, os.path.join(basedir, 'src'))
 
-LLFUSE_VERSION = '1.4.3'
+LLFUSE_VERSION = '1.4.4'
 
 def main():
 
     try:
         from sphinx.application import Sphinx #pylint: disable-msg=W0612
     except ImportError:
         pass
```

### Comparing `llfuse-1.4.3/src/darwin_compat.c` & `llfuse-1.4.4/src/darwin_compat.c`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/src/darwin_compat.h` & `llfuse-1.4.4/src/darwin_compat.h`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/src/fuse_api.pxi` & `llfuse-1.4.4/src/fuse_api.pxi`

 * *Files 0% similar despite different names*

```diff
@@ -368,30 +368,30 @@
     sem_t* sem
     int thread_no
     int started
     pthread_t thread_id
     void* buf
     size_t bufsize
 
-cdef void* worker_start(void* data) with gil:
+cdef void* worker_start(void* data) noexcept with gil:
     cdef worker_data_t *wd
     cdef int res
     cdef uintptr_t tid
     global exc_info
 
     wd = <worker_data_t*> data
 
     t = threading.current_thread()
     t.name = 'fuse-worker-%d' % (wd.thread_no+1,)
 
     try:
         session_loop(wd.buf, wd.bufsize)
     except:
         fuse_session_exit(session)
-        tid = wd.thread_id
+        tid = <uintptr_t> wd.thread_id
         log.error('FUSE worker thread %d terminated with exception, '
                   'aborting processing', tid)
         res = pthread_mutex_lock(&exc_info_mutex)
         if res != 0:
             log.error('pthread_mutex_lock failed with %s',
                       strerror(res))
         if not exc_info:
```

### Comparing `llfuse-1.4.3/src/gettime.h` & `llfuse-1.4.4/src/gettime.h`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/src/handlers.pxi` & `llfuse-1.4.4/src/handlers.pxi`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/src/llfuse.c` & `llfuse-1.4.4/src/llfuse.c`

 * *Files 0% similar despite different names*

```diff
@@ -37645,15 +37645,15 @@
   __pyx_v_cap->ptr = __pyx_v_ptr;
 
   /* "src/misc.pxi":686
  *     cap = VoidPtrCapsule.__new__(VoidPtrCapsule)
  *     cap.ptr = ptr
  *     return cap             # <<<<<<<<<<<<<<
  * 
- * cdef void signal_handler(int sig, siginfo_t *si, void* ctx) nogil:
+ * cdef void signal_handler(int sig, siginfo_t *si, void* ctx) noexcept nogil:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_cap));
   __pyx_r = ((PyObject *)__pyx_v_cap);
   goto __pyx_L0;
 
   /* "src/misc.pxi":682
@@ -37675,24 +37675,24 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "src/misc.pxi":688
  *     return cap
  * 
- * cdef void signal_handler(int sig, siginfo_t *si, void* ctx) nogil:             # <<<<<<<<<<<<<<
+ * cdef void signal_handler(int sig, siginfo_t *si, void* ctx) noexcept nogil:             # <<<<<<<<<<<<<<
  *     global exit_reason
  *     if session != NULL:
  */
 
 static void __pyx_f_6llfuse_signal_handler(int __pyx_v_sig, CYTHON_UNUSED siginfo_t *__pyx_v_si, CYTHON_UNUSED void *__pyx_v_ctx) {
   int __pyx_t_1;
 
   /* "src/misc.pxi":690
- * cdef void signal_handler(int sig, siginfo_t *si, void* ctx) nogil:
+ * cdef void signal_handler(int sig, siginfo_t *si, void* ctx) noexcept nogil:
  *     global exit_reason
  *     if session != NULL:             # <<<<<<<<<<<<<<
  *         fuse_session_exit(session)
  *     exit_reason = sig
  */
   __pyx_t_1 = ((__pyx_v_6llfuse_session != NULL) != 0);
   if (__pyx_t_1) {
@@ -37703,46 +37703,46 @@
  *         fuse_session_exit(session)             # <<<<<<<<<<<<<<
  *     exit_reason = sig
  * 
  */
     fuse_session_exit(__pyx_v_6llfuse_session);
 
     /* "src/misc.pxi":690
- * cdef void signal_handler(int sig, siginfo_t *si, void* ctx) nogil:
+ * cdef void signal_handler(int sig, siginfo_t *si, void* ctx) noexcept nogil:
  *     global exit_reason
  *     if session != NULL:             # <<<<<<<<<<<<<<
  *         fuse_session_exit(session)
  *     exit_reason = sig
  */
   }
 
   /* "src/misc.pxi":692
  *     if session != NULL:
  *         fuse_session_exit(session)
  *     exit_reason = sig             # <<<<<<<<<<<<<<
  * 
- * cdef void do_nothing(int sig, siginfo_t *si, void* ctx) nogil:
+ * cdef void do_nothing(int sig, siginfo_t *si, void* ctx) noexcept nogil:
  */
   __pyx_v_6llfuse_exit_reason = __pyx_v_sig;
 
   /* "src/misc.pxi":688
  *     return cap
  * 
- * cdef void signal_handler(int sig, siginfo_t *si, void* ctx) nogil:             # <<<<<<<<<<<<<<
+ * cdef void signal_handler(int sig, siginfo_t *si, void* ctx) noexcept nogil:             # <<<<<<<<<<<<<<
  *     global exit_reason
  *     if session != NULL:
  */
 
   /* function exit code */
 }
 
 /* "src/misc.pxi":694
  *     exit_reason = sig
  * 
- * cdef void do_nothing(int sig, siginfo_t *si, void* ctx) nogil:             # <<<<<<<<<<<<<<
+ * cdef void do_nothing(int sig, siginfo_t *si, void* ctx) noexcept nogil:             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 static void __pyx_f_6llfuse_do_nothing(CYTHON_UNUSED int __pyx_v_sig, CYTHON_UNUSED siginfo_t *__pyx_v_si, CYTHON_UNUSED void *__pyx_v_ctx) {
 
   /* function exit code */
@@ -41718,15 +41718,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "src/fuse_api.pxi":375
  *     size_t bufsize
  * 
- * cdef void* worker_start(void* data) with gil:             # <<<<<<<<<<<<<<
+ * cdef void* worker_start(void* data) noexcept with gil:             # <<<<<<<<<<<<<<
  *     cdef worker_data_t *wd
  *     cdef int res
  */
 
 static void *__pyx_f_6llfuse_worker_start(void *__pyx_v_data) {
   __pyx_t_6llfuse_worker_data_t *__pyx_v_wd;
   int __pyx_v_res;
@@ -41736,28 +41736,27 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
-  pthread_t __pyx_t_7;
+  PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
-  PyObject *__pyx_t_11 = NULL;
-  int __pyx_t_12;
-  PyObject *__pyx_t_13 = NULL;
+  int __pyx_t_11;
+  PyObject *__pyx_t_12 = NULL;
+  int __pyx_t_13;
   int __pyx_t_14;
   int __pyx_t_15;
-  int __pyx_t_16;
-  char const *__pyx_t_17;
+  char const *__pyx_t_16;
+  PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
   PyObject *__pyx_t_19 = NULL;
-  PyObject *__pyx_t_20 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("worker_start", 0);
@@ -41862,112 +41861,111 @@
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
 
       /* "src/fuse_api.pxi":388
  *     try:
  *         session_loop(wd.buf, wd.bufsize)
  *     except:             # <<<<<<<<<<<<<<
  *         fuse_session_exit(session)
- *         tid = wd.thread_id
+ *         tid = <uintptr_t> wd.thread_id
  */
       /*except:*/ {
         __Pyx_AddTraceback("llfuse.worker_start", __pyx_clineno, __pyx_lineno, __pyx_filename);
         if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_1, &__pyx_t_2) < 0) __PYX_ERR(3, 388, __pyx_L8_except_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_GOTREF(__pyx_t_2);
 
         /* "src/fuse_api.pxi":389
  *         session_loop(wd.buf, wd.bufsize)
  *     except:
  *         fuse_session_exit(session)             # <<<<<<<<<<<<<<
- *         tid = wd.thread_id
+ *         tid = <uintptr_t> wd.thread_id
  *         log.error('FUSE worker thread %d terminated with exception, '
  */
         fuse_session_exit(__pyx_v_6llfuse_session);
 
         /* "src/fuse_api.pxi":390
  *     except:
  *         fuse_session_exit(session)
- *         tid = wd.thread_id             # <<<<<<<<<<<<<<
+ *         tid = <uintptr_t> wd.thread_id             # <<<<<<<<<<<<<<
  *         log.error('FUSE worker thread %d terminated with exception, '
  *                   'aborting processing', tid)
  */
-        __pyx_t_7 = __pyx_v_wd->thread_id;
-        __pyx_v_tid = __pyx_t_7;
+        __pyx_v_tid = ((uintptr_t)__pyx_v_wd->thread_id);
 
         /* "src/fuse_api.pxi":391
  *         fuse_session_exit(session)
- *         tid = wd.thread_id
+ *         tid = <uintptr_t> wd.thread_id
  *         log.error('FUSE worker thread %d terminated with exception, '             # <<<<<<<<<<<<<<
  *                   'aborting processing', tid)
  *         res = pthread_mutex_lock(&exc_info_mutex)
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_log); if (unlikely(!__pyx_t_9)) __PYX_ERR(3, 391, __pyx_L8_except_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_log); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 391, __pyx_L8_except_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_error); if (unlikely(!__pyx_t_9)) __PYX_ERR(3, 391, __pyx_L8_except_error)
         __Pyx_GOTREF(__pyx_t_9);
-        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_error); if (unlikely(!__pyx_t_10)) __PYX_ERR(3, 391, __pyx_L8_except_error)
-        __Pyx_GOTREF(__pyx_t_10);
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
         /* "src/fuse_api.pxi":392
- *         tid = wd.thread_id
+ *         tid = <uintptr_t> wd.thread_id
  *         log.error('FUSE worker thread %d terminated with exception, '
  *                   'aborting processing', tid)             # <<<<<<<<<<<<<<
  *         res = pthread_mutex_lock(&exc_info_mutex)
  *         if res != 0:
  */
-        __pyx_t_9 = __Pyx_PyInt_FromSize_t(__pyx_v_tid); if (unlikely(!__pyx_t_9)) __PYX_ERR(3, 392, __pyx_L8_except_error)
-        __Pyx_GOTREF(__pyx_t_9);
-        __pyx_t_11 = NULL;
-        __pyx_t_12 = 0;
-        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
-          __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_10);
-          if (likely(__pyx_t_11)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
-            __Pyx_INCREF(__pyx_t_11);
+        __pyx_t_8 = __Pyx_PyInt_FromSize_t(__pyx_v_tid); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 392, __pyx_L8_except_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __pyx_t_10 = NULL;
+        __pyx_t_11 = 0;
+        if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_9))) {
+          __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
+          if (likely(__pyx_t_10)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+            __Pyx_INCREF(__pyx_t_10);
             __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_10, function);
-            __pyx_t_12 = 1;
+            __Pyx_DECREF_SET(__pyx_t_9, function);
+            __pyx_t_11 = 1;
           }
         }
         #if CYTHON_FAST_PYCALL
-        if (PyFunction_Check(__pyx_t_10)) {
-          PyObject *__pyx_temp[3] = {__pyx_t_11, __pyx_kp_u_FUSE_worker_thread_d_terminated, __pyx_t_9};
-          __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 391, __pyx_L8_except_error)
-          __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __Pyx_GOTREF(__pyx_t_8);
-          __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        if (PyFunction_Check(__pyx_t_9)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_kp_u_FUSE_worker_thread_d_terminated, __pyx_t_8};
+          __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 391, __pyx_L8_except_error)
+          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __Pyx_GOTREF(__pyx_t_7);
+          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         #if CYTHON_FAST_PYCCALL
-        if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
-          PyObject *__pyx_temp[3] = {__pyx_t_11, __pyx_kp_u_FUSE_worker_thread_d_terminated, __pyx_t_9};
-          __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 391, __pyx_L8_except_error)
-          __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __Pyx_GOTREF(__pyx_t_8);
-          __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
+          PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_kp_u_FUSE_worker_thread_d_terminated, __pyx_t_8};
+          __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 391, __pyx_L8_except_error)
+          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __Pyx_GOTREF(__pyx_t_7);
+          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else
         #endif
         {
-          __pyx_t_13 = PyTuple_New(2+__pyx_t_12); if (unlikely(!__pyx_t_13)) __PYX_ERR(3, 391, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_13);
-          if (__pyx_t_11) {
-            __Pyx_GIVEREF(__pyx_t_11); PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_11); __pyx_t_11 = NULL;
+          __pyx_t_12 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(3, 391, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          if (__pyx_t_10) {
+            __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
           }
           __Pyx_INCREF(__pyx_kp_u_FUSE_worker_thread_d_terminated);
           __Pyx_GIVEREF(__pyx_kp_u_FUSE_worker_thread_d_terminated);
-          PyTuple_SET_ITEM(__pyx_t_13, 0+__pyx_t_12, __pyx_kp_u_FUSE_worker_thread_d_terminated);
-          __Pyx_GIVEREF(__pyx_t_9);
-          PyTuple_SET_ITEM(__pyx_t_13, 1+__pyx_t_12, __pyx_t_9);
-          __pyx_t_9 = 0;
-          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_13, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 391, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_8);
-          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+          PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_kp_u_FUSE_worker_thread_d_terminated);
+          __Pyx_GIVEREF(__pyx_t_8);
+          PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, __pyx_t_8);
+          __pyx_t_8 = 0;
+          __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_12, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 391, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_7);
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         }
-        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
         /* "src/fuse_api.pxi":393
  *         log.error('FUSE worker thread %d terminated with exception, '
  *                   'aborting processing', tid)
  *         res = pthread_mutex_lock(&exc_info_mutex)             # <<<<<<<<<<<<<<
  *         if res != 0:
  *             log.error('pthread_mutex_lock failed with %s',
@@ -41977,87 +41975,87 @@
         /* "src/fuse_api.pxi":394
  *                   'aborting processing', tid)
  *         res = pthread_mutex_lock(&exc_info_mutex)
  *         if res != 0:             # <<<<<<<<<<<<<<
  *             log.error('pthread_mutex_lock failed with %s',
  *                       strerror(res))
  */
-        __pyx_t_14 = ((__pyx_v_res != 0) != 0);
-        if (__pyx_t_14) {
+        __pyx_t_13 = ((__pyx_v_res != 0) != 0);
+        if (__pyx_t_13) {
 
           /* "src/fuse_api.pxi":395
  *         res = pthread_mutex_lock(&exc_info_mutex)
  *         if res != 0:
  *             log.error('pthread_mutex_lock failed with %s',             # <<<<<<<<<<<<<<
  *                       strerror(res))
  *         if not exc_info:
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_log); if (unlikely(!__pyx_t_10)) __PYX_ERR(3, 395, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_error); if (unlikely(!__pyx_t_13)) __PYX_ERR(3, 395, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_13);
-          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_log); if (unlikely(!__pyx_t_9)) __PYX_ERR(3, 395, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_9);
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_error); if (unlikely(!__pyx_t_12)) __PYX_ERR(3, 395, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
           /* "src/fuse_api.pxi":396
  *         if res != 0:
  *             log.error('pthread_mutex_lock failed with %s',
  *                       strerror(res))             # <<<<<<<<<<<<<<
  *         if not exc_info:
  *             exc_info = sys.exc_info()
  */
-          __pyx_t_10 = __pyx_f_6llfuse_strerror(__pyx_v_res); if (unlikely(!__pyx_t_10)) __PYX_ERR(3, 396, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_10);
-          __pyx_t_9 = NULL;
-          __pyx_t_12 = 0;
-          if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_13))) {
-            __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_13);
-            if (likely(__pyx_t_9)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
-              __Pyx_INCREF(__pyx_t_9);
+          __pyx_t_9 = __pyx_f_6llfuse_strerror(__pyx_v_res); if (unlikely(!__pyx_t_9)) __PYX_ERR(3, 396, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_9);
+          __pyx_t_8 = NULL;
+          __pyx_t_11 = 0;
+          if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
+            __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_12);
+            if (likely(__pyx_t_8)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+              __Pyx_INCREF(__pyx_t_8);
               __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_13, function);
-              __pyx_t_12 = 1;
+              __Pyx_DECREF_SET(__pyx_t_12, function);
+              __pyx_t_11 = 1;
             }
           }
           #if CYTHON_FAST_PYCALL
-          if (PyFunction_Check(__pyx_t_13)) {
-            PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_kp_u_pthread_mutex_lock_failed_with_s, __pyx_t_10};
-            __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_13, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 395, __pyx_L8_except_error)
-            __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-            __Pyx_GOTREF(__pyx_t_8);
-            __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+          if (PyFunction_Check(__pyx_t_12)) {
+            PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_kp_u_pthread_mutex_lock_failed_with_s, __pyx_t_9};
+            __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 395, __pyx_L8_except_error)
+            __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+            __Pyx_GOTREF(__pyx_t_7);
+            __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
           } else
           #endif
           #if CYTHON_FAST_PYCCALL
-          if (__Pyx_PyFastCFunction_Check(__pyx_t_13)) {
-            PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_kp_u_pthread_mutex_lock_failed_with_s, __pyx_t_10};
-            __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_13, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 395, __pyx_L8_except_error)
-            __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-            __Pyx_GOTREF(__pyx_t_8);
-            __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+          if (__Pyx_PyFastCFunction_Check(__pyx_t_12)) {
+            PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_kp_u_pthread_mutex_lock_failed_with_s, __pyx_t_9};
+            __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_12, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 395, __pyx_L8_except_error)
+            __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+            __Pyx_GOTREF(__pyx_t_7);
+            __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
           } else
           #endif
           {
-            __pyx_t_11 = PyTuple_New(2+__pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(3, 395, __pyx_L8_except_error)
-            __Pyx_GOTREF(__pyx_t_11);
-            if (__pyx_t_9) {
-              __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_9); __pyx_t_9 = NULL;
+            __pyx_t_10 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_10)) __PYX_ERR(3, 395, __pyx_L8_except_error)
+            __Pyx_GOTREF(__pyx_t_10);
+            if (__pyx_t_8) {
+              __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
             }
             __Pyx_INCREF(__pyx_kp_u_pthread_mutex_lock_failed_with_s);
             __Pyx_GIVEREF(__pyx_kp_u_pthread_mutex_lock_failed_with_s);
-            PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_12, __pyx_kp_u_pthread_mutex_lock_failed_with_s);
-            __Pyx_GIVEREF(__pyx_t_10);
-            PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_12, __pyx_t_10);
-            __pyx_t_10 = 0;
-            __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_13, __pyx_t_11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 395, __pyx_L8_except_error)
-            __Pyx_GOTREF(__pyx_t_8);
-            __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+            PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_11, __pyx_kp_u_pthread_mutex_lock_failed_with_s);
+            __Pyx_GIVEREF(__pyx_t_9);
+            PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_11, __pyx_t_9);
+            __pyx_t_9 = 0;
+            __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_10, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 395, __pyx_L8_except_error)
+            __Pyx_GOTREF(__pyx_t_7);
+            __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
           }
-          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
           /* "src/fuse_api.pxi":394
  *                   'aborting processing', tid)
  *         res = pthread_mutex_lock(&exc_info_mutex)
  *         if res != 0:             # <<<<<<<<<<<<<<
  *             log.error('pthread_mutex_lock failed with %s',
  *                       strerror(res))
@@ -42067,49 +42065,49 @@
         /* "src/fuse_api.pxi":397
  *             log.error('pthread_mutex_lock failed with %s',
  *                       strerror(res))
  *         if not exc_info:             # <<<<<<<<<<<<<<
  *             exc_info = sys.exc_info()
  *         else:
  */
-        __pyx_t_14 = __Pyx_PyObject_IsTrue(__pyx_v_6llfuse_exc_info); if (unlikely(__pyx_t_14 < 0)) __PYX_ERR(3, 397, __pyx_L8_except_error)
-        __pyx_t_15 = ((!__pyx_t_14) != 0);
-        if (__pyx_t_15) {
+        __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_v_6llfuse_exc_info); if (unlikely(__pyx_t_13 < 0)) __PYX_ERR(3, 397, __pyx_L8_except_error)
+        __pyx_t_14 = ((!__pyx_t_13) != 0);
+        if (__pyx_t_14) {
 
           /* "src/fuse_api.pxi":398
  *                       strerror(res))
  *         if not exc_info:
  *             exc_info = sys.exc_info()             # <<<<<<<<<<<<<<
  *         else:
  *             log.exception('Only one exception can be re-raised, the following '
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_sys); if (unlikely(!__pyx_t_13)) __PYX_ERR(3, 398, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_13);
-          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_exc_info); if (unlikely(!__pyx_t_11)) __PYX_ERR(3, 398, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-          __pyx_t_13 = NULL;
-          if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
-            __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_11);
-            if (likely(__pyx_t_13)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
-              __Pyx_INCREF(__pyx_t_13);
+          __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_sys); if (unlikely(!__pyx_t_12)) __PYX_ERR(3, 398, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_exc_info); if (unlikely(!__pyx_t_10)) __PYX_ERR(3, 398, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_10);
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __pyx_t_12 = NULL;
+          if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
+            __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_10);
+            if (likely(__pyx_t_12)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+              __Pyx_INCREF(__pyx_t_12);
               __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_11, function);
+              __Pyx_DECREF_SET(__pyx_t_10, function);
             }
           }
-          __pyx_t_8 = (__pyx_t_13) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_13) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
-          __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 398, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_8);
-          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+          __pyx_t_7 = (__pyx_t_12) ? __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_12) : __Pyx_PyObject_CallNoArg(__pyx_t_10);
+          __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+          if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 398, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_7);
+          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
           __Pyx_XGOTREF(__pyx_v_6llfuse_exc_info);
-          __Pyx_DECREF_SET(__pyx_v_6llfuse_exc_info, __pyx_t_8);
-          __Pyx_GIVEREF(__pyx_t_8);
-          __pyx_t_8 = 0;
+          __Pyx_DECREF_SET(__pyx_v_6llfuse_exc_info, __pyx_t_7);
+          __Pyx_GIVEREF(__pyx_t_7);
+          __pyx_t_7 = 0;
 
           /* "src/fuse_api.pxi":397
  *             log.error('pthread_mutex_lock failed with %s',
  *                       strerror(res))
  *         if not exc_info:             # <<<<<<<<<<<<<<
  *             exc_info = sys.exc_info()
  *         else:
@@ -42121,35 +42119,35 @@
  *             exc_info = sys.exc_info()
  *         else:
  *             log.exception('Only one exception can be re-raised, the following '             # <<<<<<<<<<<<<<
  *                           'exception will be lost:')
  *         pthread_mutex_unlock(&exc_info_mutex)
  */
         /*else*/ {
-          __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_log); if (unlikely(!__pyx_t_11)) __PYX_ERR(3, 400, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_11);
-          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_exception); if (unlikely(!__pyx_t_13)) __PYX_ERR(3, 400, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_13);
-          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_11 = NULL;
-          if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_13))) {
-            __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_13);
-            if (likely(__pyx_t_11)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
-              __Pyx_INCREF(__pyx_t_11);
+          __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_log); if (unlikely(!__pyx_t_10)) __PYX_ERR(3, 400, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_10);
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_exception); if (unlikely(!__pyx_t_12)) __PYX_ERR(3, 400, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __pyx_t_10 = NULL;
+          if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_12))) {
+            __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_12);
+            if (likely(__pyx_t_10)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+              __Pyx_INCREF(__pyx_t_10);
               __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_13, function);
+              __Pyx_DECREF_SET(__pyx_t_12, function);
             }
           }
-          __pyx_t_8 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_13, __pyx_t_11, __pyx_kp_u_Only_one_exception_can_be_re_rai_2) : __Pyx_PyObject_CallOneArg(__pyx_t_13, __pyx_kp_u_Only_one_exception_can_be_re_rai_2);
-          __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 400, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_8);
-          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __pyx_t_7 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_12, __pyx_t_10, __pyx_kp_u_Only_one_exception_can_be_re_rai_2) : __Pyx_PyObject_CallOneArg(__pyx_t_12, __pyx_kp_u_Only_one_exception_can_be_re_rai_2);
+          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+          if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 400, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_7);
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+          __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         }
         __pyx_L15:;
 
         /* "src/fuse_api.pxi":402
  *             log.exception('Only one exception can be re-raised, the following '
  *                           'exception will be lost:')
  *         pthread_mutex_unlock(&exc_info_mutex)             # <<<<<<<<<<<<<<
@@ -42161,87 +42159,87 @@
         /* "src/fuse_api.pxi":403
  *                           'exception will be lost:')
  *         pthread_mutex_unlock(&exc_info_mutex)
  *         if res != 0:             # <<<<<<<<<<<<<<
  *             log.error('pthread_mutex_ulock failed with %s',
  *                       strerror(res))
  */
-        __pyx_t_15 = ((__pyx_v_res != 0) != 0);
-        if (__pyx_t_15) {
+        __pyx_t_14 = ((__pyx_v_res != 0) != 0);
+        if (__pyx_t_14) {
 
           /* "src/fuse_api.pxi":404
  *         pthread_mutex_unlock(&exc_info_mutex)
  *         if res != 0:
  *             log.error('pthread_mutex_ulock failed with %s',             # <<<<<<<<<<<<<<
  *                       strerror(res))
  * 
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_log); if (unlikely(!__pyx_t_13)) __PYX_ERR(3, 404, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_13);
-          __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_error); if (unlikely(!__pyx_t_11)) __PYX_ERR(3, 404, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_11);
-          __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+          __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_log); if (unlikely(!__pyx_t_12)) __PYX_ERR(3, 404, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_error); if (unlikely(!__pyx_t_10)) __PYX_ERR(3, 404, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_10);
+          __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
 
           /* "src/fuse_api.pxi":405
  *         if res != 0:
  *             log.error('pthread_mutex_ulock failed with %s',
  *                       strerror(res))             # <<<<<<<<<<<<<<
  * 
  *     finally:
  */
-          __pyx_t_13 = __pyx_f_6llfuse_strerror(__pyx_v_res); if (unlikely(!__pyx_t_13)) __PYX_ERR(3, 405, __pyx_L8_except_error)
-          __Pyx_GOTREF(__pyx_t_13);
-          __pyx_t_10 = NULL;
-          __pyx_t_12 = 0;
-          if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_11))) {
-            __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_11);
-            if (likely(__pyx_t_10)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
-              __Pyx_INCREF(__pyx_t_10);
+          __pyx_t_12 = __pyx_f_6llfuse_strerror(__pyx_v_res); if (unlikely(!__pyx_t_12)) __PYX_ERR(3, 405, __pyx_L8_except_error)
+          __Pyx_GOTREF(__pyx_t_12);
+          __pyx_t_9 = NULL;
+          __pyx_t_11 = 0;
+          if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
+            __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
+            if (likely(__pyx_t_9)) {
+              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
+              __Pyx_INCREF(__pyx_t_9);
               __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_11, function);
-              __pyx_t_12 = 1;
+              __Pyx_DECREF_SET(__pyx_t_10, function);
+              __pyx_t_11 = 1;
             }
           }
           #if CYTHON_FAST_PYCALL
-          if (PyFunction_Check(__pyx_t_11)) {
-            PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_kp_u_pthread_mutex_ulock_failed_with, __pyx_t_13};
-            __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 404, __pyx_L8_except_error)
-            __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-            __Pyx_GOTREF(__pyx_t_8);
-            __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+          if (PyFunction_Check(__pyx_t_10)) {
+            PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_kp_u_pthread_mutex_ulock_failed_with, __pyx_t_12};
+            __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 404, __pyx_L8_except_error)
+            __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+            __Pyx_GOTREF(__pyx_t_7);
+            __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           } else
           #endif
           #if CYTHON_FAST_PYCCALL
-          if (__Pyx_PyFastCFunction_Check(__pyx_t_11)) {
-            PyObject *__pyx_temp[3] = {__pyx_t_10, __pyx_kp_u_pthread_mutex_ulock_failed_with, __pyx_t_13};
-            __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_11, __pyx_temp+1-__pyx_t_12, 2+__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 404, __pyx_L8_except_error)
-            __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-            __Pyx_GOTREF(__pyx_t_8);
-            __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+          if (__Pyx_PyFastCFunction_Check(__pyx_t_10)) {
+            PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_kp_u_pthread_mutex_ulock_failed_with, __pyx_t_12};
+            __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_10, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 404, __pyx_L8_except_error)
+            __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+            __Pyx_GOTREF(__pyx_t_7);
+            __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           } else
           #endif
           {
-            __pyx_t_9 = PyTuple_New(2+__pyx_t_12); if (unlikely(!__pyx_t_9)) __PYX_ERR(3, 404, __pyx_L8_except_error)
-            __Pyx_GOTREF(__pyx_t_9);
-            if (__pyx_t_10) {
-              __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_10); __pyx_t_10 = NULL;
+            __pyx_t_8 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 404, __pyx_L8_except_error)
+            __Pyx_GOTREF(__pyx_t_8);
+            if (__pyx_t_9) {
+              __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_9); __pyx_t_9 = NULL;
             }
             __Pyx_INCREF(__pyx_kp_u_pthread_mutex_ulock_failed_with);
             __Pyx_GIVEREF(__pyx_kp_u_pthread_mutex_ulock_failed_with);
-            PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_12, __pyx_kp_u_pthread_mutex_ulock_failed_with);
-            __Pyx_GIVEREF(__pyx_t_13);
-            PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_12, __pyx_t_13);
-            __pyx_t_13 = 0;
-            __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(3, 404, __pyx_L8_except_error)
-            __Pyx_GOTREF(__pyx_t_8);
-            __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+            PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_11, __pyx_kp_u_pthread_mutex_ulock_failed_with);
+            __Pyx_GIVEREF(__pyx_t_12);
+            PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_11, __pyx_t_12);
+            __pyx_t_12 = 0;
+            __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_10, __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(3, 404, __pyx_L8_except_error)
+            __Pyx_GOTREF(__pyx_t_7);
+            __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
           }
-          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
           /* "src/fuse_api.pxi":403
  *                           'exception will be lost:')
  *         pthread_mutex_unlock(&exc_info_mutex)
  *         if res != 0:             # <<<<<<<<<<<<<<
  *             log.error('pthread_mutex_ulock failed with %s',
  *                       strerror(res))
@@ -42287,72 +42285,72 @@
       (void)(sem_post(__pyx_v_wd->sem));
       goto __pyx_L5;
     }
     __pyx_L4_error:;
     /*exception exit:*/{
       __Pyx_PyThreadState_declare
       __Pyx_PyThreadState_assign
-      __pyx_t_6 = 0; __pyx_t_5 = 0; __pyx_t_4 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0;
+      __pyx_t_6 = 0; __pyx_t_5 = 0; __pyx_t_4 = 0; __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+      __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_18, &__pyx_t_19, &__pyx_t_20);
+      if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_17, &__pyx_t_18, &__pyx_t_19);
       if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_6, &__pyx_t_5, &__pyx_t_4) < 0)) __Pyx_ErrFetch(&__pyx_t_6, &__pyx_t_5, &__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_4);
+      __Pyx_XGOTREF(__pyx_t_17);
       __Pyx_XGOTREF(__pyx_t_18);
       __Pyx_XGOTREF(__pyx_t_19);
-      __Pyx_XGOTREF(__pyx_t_20);
-      __pyx_t_12 = __pyx_lineno; __pyx_t_16 = __pyx_clineno; __pyx_t_17 = __pyx_filename;
+      __pyx_t_11 = __pyx_lineno; __pyx_t_15 = __pyx_clineno; __pyx_t_16 = __pyx_filename;
       {
         (void)(sem_post(__pyx_v_wd->sem));
       }
       if (PY_MAJOR_VERSION >= 3) {
+        __Pyx_XGIVEREF(__pyx_t_17);
         __Pyx_XGIVEREF(__pyx_t_18);
         __Pyx_XGIVEREF(__pyx_t_19);
-        __Pyx_XGIVEREF(__pyx_t_20);
-        __Pyx_ExceptionReset(__pyx_t_18, __pyx_t_19, __pyx_t_20);
+        __Pyx_ExceptionReset(__pyx_t_17, __pyx_t_18, __pyx_t_19);
       }
       __Pyx_XGIVEREF(__pyx_t_6);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_ErrRestore(__pyx_t_6, __pyx_t_5, __pyx_t_4);
-      __pyx_t_6 = 0; __pyx_t_5 = 0; __pyx_t_4 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0; __pyx_t_20 = 0;
-      __pyx_lineno = __pyx_t_12; __pyx_clineno = __pyx_t_16; __pyx_filename = __pyx_t_17;
+      __pyx_t_6 = 0; __pyx_t_5 = 0; __pyx_t_4 = 0; __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0;
+      __pyx_lineno = __pyx_t_11; __pyx_clineno = __pyx_t_15; __pyx_filename = __pyx_t_16;
       goto __pyx_L1_error;
     }
     __pyx_L5:;
   }
 
   /* "src/fuse_api.pxi":375
  *     size_t bufsize
  * 
- * cdef void* worker_start(void* data) with gil:             # <<<<<<<<<<<<<<
+ * cdef void* worker_start(void* data) noexcept with gil:             # <<<<<<<<<<<<<<
  *     cdef worker_data_t *wd
  *     cdef int res
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_XDECREF(__pyx_t_13);
+  __Pyx_XDECREF(__pyx_t_12);
   __Pyx_WriteUnraisable("llfuse.worker_start", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_t);
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
```

### Comparing `llfuse-1.4.3/src/llfuse.egg-info/PKG-INFO` & `llfuse-1.4.4/src/llfuse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llfuse
-Version: 1.4.3
+Version: 1.4.4
 Summary: Python bindings for the low-level FUSE API
 Home-page: https://github.com/python-llfuse/python-llfuse/
 Author: Nikolaus Rath
 Author-email: Nikolaus@rath.org
 License: LGPL
 Keywords: FUSE,python
 Platform: Linux
```

### Comparing `llfuse-1.4.3/src/llfuse.egg-info/SOURCES.txt` & `llfuse-1.4.4/src/llfuse.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 src/operations.pxi
 src/xattr.h
 src/llfuse.egg-info/PKG-INFO
 src/llfuse.egg-info/SOURCES.txt
 src/llfuse.egg-info/dependency_links.txt
 src/llfuse.egg-info/top_level.txt
 src/llfuse.egg-info/zip-safe
-test/ci-install.sh
 test/ci-test.sh
 test/conftest.py
 test/pytest.ini
 test/pytest_checklogs.py
 test/test_api.py
 test/test_examples.py
 test/test_fs.py
```

### Comparing `llfuse-1.4.3/src/llfuse.h` & `llfuse-1.4.4/src/llfuse.h`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/src/llfuse.pyx` & `llfuse-1.4.4/src/llfuse.pyx`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/src/lock.c` & `llfuse-1.4.4/src/lock.c`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/src/macros.c` & `llfuse-1.4.4/src/macros.c`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/src/misc.pxi` & `llfuse-1.4.4/src/misc.pxi`

 * *Files 1% similar despite different names*

```diff
@@ -681,21 +681,21 @@
 
 cdef inline encap_ptr(void *ptr):
     cdef VoidPtrCapsule cap
     cap = VoidPtrCapsule.__new__(VoidPtrCapsule)
     cap.ptr = ptr
     return cap
 
-cdef void signal_handler(int sig, siginfo_t *si, void* ctx) nogil:
+cdef void signal_handler(int sig, siginfo_t *si, void* ctx) noexcept nogil:
     global exit_reason
     if session != NULL:
         fuse_session_exit(session)
     exit_reason = sig
 
-cdef void do_nothing(int sig, siginfo_t *si, void* ctx) nogil:
+cdef void do_nothing(int sig, siginfo_t *si, void* ctx) noexcept nogil:
     pass
 
 cdef int sigaction_p(int sig, sigaction_t *sa,
                      sigaction_t *old_sa) except -1:
     cdef int res
     res = sigaction(sig, sa, old_sa)
     if res != 0:
```

### Comparing `llfuse-1.4.3/src/operations.pxi` & `llfuse-1.4.4/src/operations.pxi`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/src/xattr.h` & `llfuse-1.4.4/src/xattr.h`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/test/.pytest_cache/v/cache/nodeids` & `llfuse-1.4.4/test/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/test/conftest.py` & `llfuse-1.4.4/test/conftest.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/test/pytest_checklogs.py` & `llfuse-1.4.4/test/pytest_checklogs.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/test/test_api.py` & `llfuse-1.4.4/test/test_api.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/test/test_examples.py` & `llfuse-1.4.4/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/test/test_fs.py` & `llfuse-1.4.4/test/test_fs.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/test/test_rounding.py` & `llfuse-1.4.4/test/test_rounding.py`

 * *Files identical despite different names*

### Comparing `llfuse-1.4.3/test/util.py` & `llfuse-1.4.4/test/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 This file is part of Python-LLFUSE. This work may be distributed under
 the terms of the GNU LGPL.
 '''
 
 
 import platform
+import shutil
 import subprocess
 import pytest
 import os
 import stat
 import time
 
 
@@ -26,23 +27,17 @@
     '''
 
     if platform.system() == 'Darwin':
         # No working autodetection, just assume it will work.
         return pytest.mark.uses_fuse()
     skip = lambda x: pytest.mark.skip(reason=x)
 
-    # Python 2.x: Popen is not a context manager...
-    which = subprocess.Popen(['which', 'fusermount'], stdout=subprocess.PIPE,
-                             universal_newlines=True)
-    try:
-        fusermount_path = which.communicate()[0].strip()
-    finally:
-        which.wait()
+    fusermount_path = shutil.which("fusermount")
 
-    if not fusermount_path or which.returncode != 0:
+    if fusermount_path is None:
         return skip("Can't find fusermount executable")
 
     if not os.path.exists('/dev/fuse'):
         return skip("FUSE kernel module does not seem to be loaded")
 
     if os.getuid() == 0:
         return pytest.mark.uses_fuse()
@@ -102,15 +97,15 @@
                         stderr=subprocess.STDOUT)
     else:
         subprocess.call(['fusermount', '-z', '-u', mnt_dir], stdout=subprocess.DEVNULL,
                         stderr=subprocess.STDOUT)
 
 def umount(mount_process, mnt_dir):
     if platform.system() == 'Darwin':
-        subprocess.check_call(['umount', '-l', mnt_dir])
+        subprocess.check_call(['umount', mnt_dir])
     else:
         subprocess.check_call(['fusermount', '-z', '-u', mnt_dir])
     assert not os.path.ismount(mnt_dir)
 
     # Give mount process a little while to terminate. Popen.wait(timeout)
     # was only added in 3.3...
     elapsed = 0
```

### Comparing `llfuse-1.4.3/util/sphinx_cython.py` & `llfuse-1.4.4/util/sphinx_cython.py`

 * *Files identical despite different names*

