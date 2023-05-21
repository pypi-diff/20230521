# Comparing `tmp/kivy-ios-2023.1.29.tar.gz` & `tmp/kivy-ios-2023.5.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivy-ios-2023.1.29.tar", last modified: Sun Jan 29 16:10:06 2023, max compression
+gzip compressed data, was "kivy-ios-2023.5.21.tar", last modified: Sun May 21 13:23:21 2023, max compression
```

## Comparing `kivy-ios-2023.1.29.tar` & `kivy-ios-2023.5.21.tar`

### file list

```diff
@@ -1,176 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.898492 kivy-ios-2023.1.29/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-01-29 16:10:06.898492 kivy-ios-2023.1.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.882492 kivy-ios-2023.1.29/kivy_ios/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/context_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/audiostream/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/audiostream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/click/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/click/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/curly/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/curly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/cymunk/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/cymunk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/ffmpeg/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/ffmpeg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/ffpyplayer/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/ffpyplayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/ffpyplayer/misc-visibility.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/flask/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/flask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/freetype/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/freetype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/host_setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/host_setuptools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/host_setuptools/setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/host_setuptools/setuptools/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/host_setuptools3/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/host_setuptools3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/host_setuptools3/setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/host_setuptools3/setuptools/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/hostopenssl/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/hostopenssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/hostpython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/hostpython3/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/hostpython3/ModulesSetup
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/hostpython3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/hostpython3/disable_sysconfig_cflags.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios/recipes/ios/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/ios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/ios.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/ios_browser.m
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/ios_filechooser.m
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/ios_mail.m
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/ios_utils.m
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/ios_wrapper.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/itsdangerous/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/itsdangerous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/jinja2/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/jinja2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/kivent_core/
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/kivent_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/kivy/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/kivy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/libcurl/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/libcurl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/libffi/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/libffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/libffi/enable-tramp-build.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/libjpeg/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/libjpeg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/libpng/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/libpng/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/libzbar/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/libzbar/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/libzbar/werror.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/markupsafe/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/markupsafe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/netifaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/netifaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/numpy/duplicated_symbols.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/openssl/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/openssl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/photolibrary/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/photolibrary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/pillow/
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/pillow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/pillow/bypass-find-library.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/plyer/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/plyer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/py3dns/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/py3dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/py3dns/ios.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/pycrypto/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/pycrypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/pycrypto/hash_SHA2_template.c.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/pykka/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/pykka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.890492 kivy-ios-2023.1.29/kivy_ios/recipes/pyobjus/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/pyobjus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/recipes/python3/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/python3/ModulesSetup
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/python3/ModulesSetup.mobile
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/python3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/python3/config.sub.patch
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/python3/configure.patch
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/python3/ctypes_duplicate.patch
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/python3/dynload_shlib.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.882492 kivy-ios-2023.1.29/kivy_ios/recipes/python3/mock_modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/recipes/python3/mock_modules/_sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/python3/mock_modules/_sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/python3/mock_modules/_sqlite3/_sqlite3.cpython-39-darwin.so
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/python3/posixmodule.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/recipes/pyyaml/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/pyyaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/recipes/sdl2/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/sdl2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/sdl2/uikit-transparent.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/recipes/sdl2_image/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/sdl2_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/sdl2_image/fix-ios-xcodebuild.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/recipes/sdl2_mixer/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/sdl2_mixer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/recipes/sdl2_ttf/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/sdl2_ttf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/recipes/werkzeug/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/werkzeug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/recipes/zbarlight/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3004 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/zbarlight/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/recipes/zbarlight/zbarlight_1_2.patch
--rwxr-xr-x   0 runner    (1001) docker     (123)    55979 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/toolchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/biglink
--rwxr-xr-x   0 runner    (1001) docker     (123)     1545 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/cythonize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/tools/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/external/xcassets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1747 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/liblink
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/tools/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/Storyboards/
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/Storyboards/Launch Screen.storyboard
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.894492 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/android.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.898492 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/.empty
--rw-r--r--   0 runner    (1001) docker     (123)   328449 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/5509213687_ffd18df0b9_b.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   437958 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/5552597274_de8b3fb5d2_b.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   224866 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/faust_github.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/pictures.kv
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/shadow32.png
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/bridge.h
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/bridge.m
--rw-r--r--   0 runner    (1001) docker     (123)    16577 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/main.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.882492 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.882492 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}/Images.xcassets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.898492 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}/Images.xcassets/AppIcon.appiconset/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}/Images.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}-Info.plist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.898492 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}.xcodeproj/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13947 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}.xcodeproj/project.pbxproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.898492 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}.xcodeproj/project.xcworkspace/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}.xcodeproj/project.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:10:06.886492 kivy-ios-2023.1.29/kivy_ios.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-01-29 16:10:06.000000 kivy-ios-2023.1.29/kivy_ios.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-01-29 16:10:06.000000 kivy-ios-2023.1.29/kivy_ios.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 16:10:06.000000 kivy-ios-2023.1.29/kivy_ios.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-29 16:10:06.000000 kivy-ios-2023.1.29/kivy_ios.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-29 16:10:06.000000 kivy-ios-2023.1.29/kivy_ios.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-29 16:10:06.000000 kivy-ios-2023.1.29/kivy_ios.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-01-29 16:10:06.898492 kivy-ios-2023.1.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-29 16:09:57.000000 kivy-ios-2023.1.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.561884 kivy-ios-2023.5.21/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-21 13:23:21.561884 kivy-ios-2023.5.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12029 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.549884 kivy-ios-2023.5.21/kivy_ios/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/context_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.549884 kivy-ios-2023.5.21/kivy_ios/recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.549884 kivy-ios-2023.5.21/kivy_ios/recipes/audiostream/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/audiostream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.549884 kivy-ios-2023.5.21/kivy_ios/recipes/click/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/click/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.549884 kivy-ios-2023.5.21/kivy_ios/recipes/curly/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/curly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.549884 kivy-ios-2023.5.21/kivy_ios/recipes/cymunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/cymunk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.549884 kivy-ios-2023.5.21/kivy_ios/recipes/ffmpeg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/ffmpeg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.549884 kivy-ios-2023.5.21/kivy_ios/recipes/ffpyplayer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/ffpyplayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/ffpyplayer/misc-visibility.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/flask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/freetype/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/freetype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/hostopenssl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/hostopenssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/hostpython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/hostpython3/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/hostpython3/ModulesSetup
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/hostpython3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/hostpython3/allow-cflags-override.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/hostpython3/disable_sysconfig_cflags.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/ios/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/ios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/ios.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/ios_browser.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/ios_filechooser.m
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/ios_mail.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/ios_utils.m
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/ios_wrapper.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/itsdangerous/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/itsdangerous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/jinja2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/kivent_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/kivent_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/kivy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/kivy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/libcurl/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/libcurl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/libffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/libffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/libffi/enable-tramp-build.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/libjpeg/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/libjpeg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/libpng/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/libpng/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/libzbar/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/libzbar/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/libzbar/werror.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/markupsafe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/markupsafe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/netifaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/netifaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/numpy/duplicated_symbols.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/numpy/skip-math-test.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.553884 kivy-ios-2023.5.21/kivy_ios/recipes/openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/openssl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/photolibrary/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/photolibrary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/pillow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/pillow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/pillow/bypass-find-library.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/plyer/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/plyer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/py3dns/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/py3dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/py3dns/ios.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/pycrypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/pycrypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/pycrypto/hash_SHA2_template.c.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/pykka/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/pykka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/pyobjus/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/pyobjus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/python3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/python3/ModulesSetup
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/python3/ModulesSetup.mobile
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/python3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/python3/configure.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/python3/ctypes_duplicate.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/python3/dynload_shlib.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/python3/posixmodule.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/pyyaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/pyyaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/sdl2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/sdl2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/sdl2/disable-hidapi.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/sdl2/uikit-transparent.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/sdl2_image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/sdl2_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/sdl2_image/fix-ios-xcodebuild.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/sdl2_mixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/sdl2_mixer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/sdl2_ttf/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/sdl2_ttf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/werkzeug/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/werkzeug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/recipes/zbarlight/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3004 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/zbarlight/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/recipes/zbarlight/zbarlight_1_2.patch
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56349 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/toolchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/biglink
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1545 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/cythonize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.557884 kivy-ios-2023.5.21/kivy_ios/tools/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/external/xcassets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1747 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/liblink
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.561884 kivy-ios-2023.5.21/kivy_ios/tools/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.561884 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.561884 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/Storyboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/Storyboards/Launch Screen.storyboard
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.561884 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/android.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.561884 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/.empty
+-rw-r--r--   0 runner    (1001) docker     (123)   328449 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/5509213687_ffd18df0b9_b.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   437958 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/5552597274_de8b3fb5d2_b.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   224866 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/faust_github.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/pictures.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/shadow32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/bridge.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/bridge.m
+-rw-r--r--   0 runner    (1001) docker     (123)    16577 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/main.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.549884 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.549884 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}/Images.xcassets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.561884 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}/Images.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}/Images.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}-Info.plist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.561884 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}.xcodeproj/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13949 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}.xcodeproj/project.pbxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.561884 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:23:21.549884 kivy-ios-2023.5.21/kivy_ios.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-21 13:23:21.000000 kivy-ios-2023.5.21/kivy_ios.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-21 13:23:21.000000 kivy-ios-2023.5.21/kivy_ios.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 13:23:21.000000 kivy-ios-2023.5.21/kivy_ios.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-21 13:23:21.000000 kivy-ios-2023.5.21/kivy_ios.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 13:23:21.000000 kivy-ios-2023.5.21/kivy_ios.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 13:23:21.000000 kivy-ios-2023.5.21/kivy_ios.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-21 13:23:21.561884 kivy-ios-2023.5.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 13:23:13.000000 kivy-ios-2023.5.21/setup.py
```

### Comparing `kivy-ios-2023.1.29/LICENSE` & `kivy-ios-2023.5.21/LICENSE`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/PKG-INFO` & `kivy-ios-2023.5.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivy-ios
-Version: 2023.1.29
+Version: 2023.5.21
 Summary: Kivy for iOS
 Home-page: https://github.com/kivy/kivy-ios
 Author: The Kivy team
 Author-email: kivy-dev@googlegroups.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,15 +41,15 @@
 
 Install [Kivy for iOS from PyPI](https://pypi.org/project/kivy-ios) with pip like any Python package.
 
       pip3 install kivy-ios
 
 Additionally, you would need a few system dependencies and configuration.
 
-- Xcode 10 or above, with an iOS SDK and command line tools installed:
+- Xcode 13 or above, with an iOS SDK and command line tools installed:
 
       xcode-select --install
 
 - Using brew, you can install the following dependencies:
 
       brew install autoconf automake libtool pkg-config
       brew link libtool
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kivy-ios Version: 2023.1.29 Summary: Kivy for iOS
+Metadata-Version: 2.1 Name: kivy-ios Version: 2023.5.21 Summary: Kivy for iOS
 Home-page: https://github.com/kivy/kivy-ios Author: The Kivy team Author-email:
 kivy-dev@googlegroups.com License: MIT License Description-Content-Type: text/
 markdown License-File: LICENSE # Kivy for iOS [![kivy-ios](https://github.com/
 kivy/kivy-ios/workflows/kivy-ios/badge.svg)](https://github.com/kivy/kivy-ios/
 actions?query=workflow%3Akivy-ios) [![PyPI version](https://badge.fury.io/py/
 kivy-ios.svg)](https://badge.fury.io/py/kivy-ios) [![Backers on Open
 Collective](https://opencollective.com/kivy/backers/badge.svg)](#backers) [!
@@ -13,15 +13,15 @@
 need to compile it at least once before creating your Xcode project. The
 toolchain supports: - iPhone Simulator (x86_64) - iPhone / iOS (arm64) These
 recipes are not ported to the new toolchain yet: - lxml ## Installation &
 requirements Before we start, we strongly advise using a Python virtual
 environment to install Python packages. python3 -m venv venv . venv/bin/
 activate Install [Kivy for iOS from PyPI](https://pypi.org/project/kivy-ios)
 with pip like any Python package. pip3 install kivy-ios Additionally, you would
-need a few system dependencies and configuration. - Xcode 10 or above, with an
+need a few system dependencies and configuration. - Xcode 13 or above, with an
 iOS SDK and command line tools installed: xcode-select --install - Using brew,
 you can install the following dependencies: brew install autoconf automake
 libtool pkg-config brew link libtool ## Using the toolchain Any Python
 extensions or C/C++ library must be compiled: you need to have what we call a
 `recipe` to compile it. For example, Python, libffi, SDL2, SDL_image,
 freetype... all the dependencies, compilation, and packaging instructions are
 contained in a `recipe`. You can list the available recipes and their versions
```

### Comparing `kivy-ios-2023.1.29/README.md` & `kivy-ios-2023.5.21/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 Install [Kivy for iOS from PyPI](https://pypi.org/project/kivy-ios) with pip like any Python package.
 
       pip3 install kivy-ios
 
 Additionally, you would need a few system dependencies and configuration.
 
-- Xcode 10 or above, with an iOS SDK and command line tools installed:
+- Xcode 13 or above, with an iOS SDK and command line tools installed:
 
       xcode-select --install
 
 - Using brew, you can install the following dependencies:
 
       brew install autoconf automake libtool pkg-config
       brew link libtool
```

#### html2text {}

```diff
@@ -10,15 +10,15 @@
 at least once before creating your Xcode project. The toolchain supports: -
 iPhone Simulator (x86_64) - iPhone / iOS (arm64) These recipes are not ported
 to the new toolchain yet: - lxml ## Installation & requirements Before we
 start, we strongly advise using a Python virtual environment to install Python
 packages. python3 -m venv venv . venv/bin/activate Install [Kivy for iOS from
 PyPI](https://pypi.org/project/kivy-ios) with pip like any Python package. pip3
 install kivy-ios Additionally, you would need a few system dependencies and
-configuration. - Xcode 10 or above, with an iOS SDK and command line tools
+configuration. - Xcode 13 or above, with an iOS SDK and command line tools
 installed: xcode-select --install - Using brew, you can install the following
 dependencies: brew install autoconf automake libtool pkg-config brew link
 libtool ## Using the toolchain Any Python extensions or C/C++ library must be
 compiled: you need to have what we call a `recipe` to compile it. For example,
 Python, libffi, SDL2, SDL_image, freetype... all the dependencies, compilation,
 and packaging instructions are contained in a `recipe`. You can list the
 available recipes and their versions with: $ toolchain recipes audiostream
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/context_managers.py` & `kivy-ios-2023.5.21/kivy_ios/context_managers.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/click/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/click/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/cymunk/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/cymunk/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/ffmpeg/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/ffmpeg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from kivy_ios.toolchain import Recipe, shprint
 from os.path import join
 import sh
 
 
 class FFMpegRecipe(Recipe):
-    version = "n4.3.1"
+    version = "n4.4.2"
     url = "https://github.com/FFmpeg/FFmpeg/archive/{version}.zip"
     include_per_arch = True
     include_dir = "dist/include"
     optional_depends = ["openssl"]
     libraries = [
         "libavcodec/libavcodec.a",
         "libavdevice/libavdevice.a",
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/ffpyplayer/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/ffpyplayer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from kivy_ios.toolchain import CythonRecipe
 from os.path import join
 
 
 class FFPyplayerRecipe(CythonRecipe):
-    version = "4.2.0"
+    version = "v4.3.5"
     url = "https://github.com/matham/ffpyplayer/archive/{version}.zip"
     library = "libffpyplayer.a"
-    depends = ["python", "ffmpeg"]
+    depends = ["python", "sdl2", "ffmpeg"]
     pbx_frameworks = [
         "CoreVideo", "CoreMedia", "CoreImage", "AVFoundation", "UIKit",
         "CoreMotion"]
     pbx_libraries = ["libiconv"]
     pre_build_ext = True
 
     def get_recipe_env(self, arch):
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/ffpyplayer/misc-visibility.patch` & `kivy-ios-2023.5.21/kivy_ios/recipes/ffpyplayer/misc-visibility.patch`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/flask/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/freetype/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/freetype/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/host_setuptools3/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/itsdangerous/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from kivy_ios.toolchain import HostRecipe, shprint, cache_execution
-from kivy_ios.context_managers import cd, python_path
+# pure-python package, this can be removed when we'll support any python package
+from kivy_ios.toolchain import PythonRecipe, shprint
+from kivy_ios.context_managers import cd
+from os.path import join
 import sh
 
 
-class HostSetuptools3(HostRecipe):
-    depends = ["openssl", "hostpython3", "python3"]
-    version = '59.2.0'
-    url = 'https://pypi.python.org/packages/source/s/setuptools/setuptools-{version}.tar.gz'
+class ItsDangerousRecipe(PythonRecipe):
+    version = "1.1.0"
+    url = "https://github.com/mitsuhiko/itsdangerous/archive/{version}.zip"
+    depends = ["python"]
 
-    @cache_execution
     def install(self):
-        arch = self.filtered_archs[0]
+        arch = list(self.filtered_archs)[0]
         build_dir = self.get_build_dir(arch.arch)
         hostpython = sh.Command(self.ctx.hostpython)
+        build_env = arch.get_env()
+        dest_dir = join(self.ctx.dist_dir, "root", "python3")
+        build_env['PYTHONPATH'] = self.ctx.site_packages_dir
+        with cd(build_dir):
+            shprint(hostpython, "setup.py", "install", "--prefix", dest_dir, _env=build_env)
 
-        with python_path(self.ctx.site_packages_dir):
-            with cd(build_dir):
-                shprint(hostpython, "setup.py", "install",
-                        f"--prefix={self.ctx.python_prefix}")
 
-
-recipe = HostSetuptools3()
+recipe = ItsDangerousRecipe()
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/hostopenssl/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/hostopenssl/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/hostpython.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/hostpython.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/hostpython3/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/hostpython3/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from kivy_ios.context_managers import cd
 
 
 logger = logging.getLogger(__name__)
 
 
 class Hostpython3Recipe(HostRecipe):
-    version = "3.9.9"
+    version = "3.10.10"
     url = "https://www.python.org/ftp/python/{version}/Python-{version}.tgz"
     depends = ["hostopenssl"]
     optional_depends = []
     build_subdir = 'native-build'
 
     def init_with_ctx(self, ctx):
         super().init_with_ctx(ctx)
-        self.set_hostpython(self, "3.9")
-        self.ctx.so_suffix = ".cpython-39m-darwin.so"
+        self.set_hostpython(self, "3.10")
+        self.ctx.so_suffix = ".cpython-310m-darwin.so"
         self.ctx.hostpython = join(self.ctx.dist_dir, "hostpython3", "bin", "python")
         self.ctx.hostpgen = join(self.ctx.dist_dir, "hostpython3", "bin", "pgen")
         logger.info("Global: hostpython located at {}".format(self.ctx.hostpython))
         logger.info("Global: hostpgen located at {}".format(self.ctx.hostpgen))
 
     def get_build_subdir(self, arch):
         return join(self.get_build_dir(arch), self.build_subdir)
@@ -83,9 +83,28 @@
                 "-C", build_subdir,
                 "install",
                 _env=build_env)
         shutil.copy(
             join(self.ctx.dist_dir, "hostpython3", "bin", "python3"),
             join(self.ctx.dist_dir, "hostpython3", "bin", "python"))
 
+        # hostpython3 installs bundled versions of `pip`
+        # and `setuptools` in `lib/python3.10/site-packages`.
+        # This is fine, but `setuptools` have a bug that prevents
+        # it from working properly when cross-compiling, so we
+        # patch it here.
+        # We can't do that before cause the packaged setuptools
+        # is installed from a wheel.
+        self.apply_patch(
+            "allow-cflags-override.patch",
+            join(
+                self.ctx.dist_dir,
+                "hostpython3",
+                "lib",
+                "python3.10",
+                "site-packages",
+                "setuptools",
+            ),
+        )
+
 
 recipe = Hostpython3Recipe()
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/hostpython3/disable_sysconfig_cflags.patch` & `kivy-ios-2023.5.21/kivy_ios/recipes/hostpython3/disable_sysconfig_cflags.patch`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/ios.pyx` & `kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/ios.pyx`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/ios_browser.m` & `kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/ios_browser.m`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/ios_filechooser.m` & `kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/ios_filechooser.m`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/ios_mail.m` & `kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/ios_mail.m`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/ios_utils.m` & `kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/ios_utils.m`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 	    return dpi;
     }
 }
 
 padding ios_get_safe_area() {
 	padding safearea;
 	if (@available(iOS 11.0, *)){
-		UIWindow *window = UIApplication.sharedApplication.windows[0];
+		UIWindow *window = [[[UIApplication sharedApplication] delegate] window];
 		safearea.top = window.safeAreaInsets.top;
 		safearea.bottom = window.safeAreaInsets.bottom;
 		safearea.left = window.safeAreaInsets.left;
 		safearea.right = window.safeAreaInsets.right;
 	} else {
 		safearea.top = 0;
 		safearea.bottom = 0;
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/ios/src/ios_wrapper.h` & `kivy-ios-2023.5.21/kivy_ios/recipes/ios/src/ios_wrapper.h`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/itsdangerous/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/netifaces/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,41 @@
-# pure-python package, this can be removed when we'll support any python package
-from kivy_ios.toolchain import PythonRecipe, shprint
-from kivy_ios.context_managers import cd
-from os.path import join
 import sh
 
+from os.path import join
+
+from kivy_ios.toolchain import CythonRecipe, shprint
+from kivy_ios.context_managers import cd
+
+
+class NetifacesRecipe(CythonRecipe):
+    version = "0.10.9"
+    url = "https://pypi.io/packages/source/n/netifaces/netifaces-{version}.tar.gz"
+    depends = ["python3"]
+    python_depends = ["setuptools"]
+    library = "libnetifaces.a"
+    cythonize = False
 
-class ItsDangerousRecipe(PythonRecipe):
-    version = "1.1.0"
-    url = "https://github.com/mitsuhiko/itsdangerous/archive/{version}.zip"
-    depends = ["python"]
+    def dest_dir(self):
+        return join(self.ctx.dist_dir, "root", "python3")
+
+    def get_netifaces_env(self, arch):
+        build_env = arch.get_env()
+        build_env["PYTHONPATH"] = self.ctx.site_packages_dir
+        return build_env
 
     def install(self):
         arch = list(self.filtered_archs)[0]
         build_dir = self.get_build_dir(arch.arch)
+        build_env = self.get_netifaces_env(arch)
         hostpython = sh.Command(self.ctx.hostpython)
-        build_env = arch.get_env()
-        dest_dir = join(self.ctx.dist_dir, "root", "python3")
-        build_env['PYTHONPATH'] = self.ctx.site_packages_dir
         with cd(build_dir):
-            shprint(hostpython, "setup.py", "install", "--prefix", dest_dir, _env=build_env)
+            shprint(
+                hostpython,
+                "setup.py",
+                "install",
+                "--prefix",
+                self.dest_dir(),
+                _env=build_env,
+            )
 
 
-recipe = ItsDangerousRecipe()
+recipe = NetifacesRecipe()
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/jinja2/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/kivent_core/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/kivent_core/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/kivy/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/kivy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import logging
 import shutil
 
 logger = logging.getLogger(__name__)
 
 
 class KivyRecipe(CythonRecipe):
-    version = "0e77e2ab94e54ebaf1f232f5dd66d4d103e08fbb"  # 2.1.0 + camera enhancements
+    version = "2.2.0"
     url = "https://github.com/kivy/kivy/archive/{version}.zip"
     library = "libkivy.a"
     depends = ["sdl2", "sdl2_image", "sdl2_mixer", "sdl2_ttf", "ios",
-               "pyobjus", "python", "host_setuptools3"]
-    python_depends = ["certifi"]
+               "pyobjus", "python"]
+    python_depends = ["certifi", "charset-normalizer", "idna", "requests", "urllib3"]
     pbx_frameworks = ["OpenGLES", "Accelerate", "CoreMedia", "CoreVideo"]
     pre_build_ext = True
 
     def get_recipe_env(self, arch):
         env = super().get_recipe_env(arch)
         env["KIVY_SDL2_PATH"] = ":".join([
             join(self.ctx.dist_dir, "include", "common", "sdl2"),
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/libcurl/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/libcurl/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/libffi/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/libffi/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/libffi/enable-tramp-build.patch` & `kivy-ios-2023.5.21/kivy_ios/recipes/libffi/enable-tramp-build.patch`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/libjpeg/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/libjpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/libpng/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/libpng/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/libzbar/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/libzbar/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/markupsafe/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/numpy/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/numpy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from kivy_ios.toolchain import CythonRecipe
 from os.path import join
 import sh
 import shutil
 
 
 class NumpyRecipe(CythonRecipe):
-    version = "1.20.2"
-    url = "https://pypi.python.org/packages/source/n/numpy/numpy-{version}.zip"
+    version = "1.24.2"
+    url = "https://pypi.python.org/packages/source/n/numpy/numpy-{version}.tar.gz"
     library = "libnumpy.a"
     libraries = ["libnpymath.a", "libnpyrandom.a"]
     include_dir = "numpy/core/include"
     depends = ["python"]
     hostpython_prerequisites = ["Cython"]
     cythonize = False
 
     def prebuild_arch(self, arch):
         if self.has_marker("patched"):
             return
+        self.apply_patch("skip-math-test.patch")
         self.apply_patch("duplicated_symbols.patch")
         self.set_marker("patched")
 
     def get_recipe_env(self, arch):
         env = super().get_recipe_env(arch)
         # CC must have the CFLAGS with arm arch, because numpy tries first to
         # compile and execute an empty C to see if the compiler works. This is
@@ -47,10 +48,12 @@
         shutil.rmtree(join(dest_dir, "lib", "tests"))
         shutil.rmtree(join(dest_dir, "linalg", "tests"))
         shutil.rmtree(join(dest_dir, "ma", "tests"))
         shutil.rmtree(join(dest_dir, "matrixlib", "tests"))
         shutil.rmtree(join(dest_dir, "polynomial", "tests"))
         shutil.rmtree(join(dest_dir, "random", "tests"))
         shutil.rmtree(join(dest_dir, "tests"))
+        sh.rm(join(dest_dir, "core", "lib", "libnpymath.a"))
+        sh.rm(join(dest_dir, "random", "lib", "libnpyrandom.a"))
 
 
 recipe = NumpyRecipe()
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/openssl/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/openssl/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/pillow/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/pillow/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 class PillowRecipe(CythonRecipe):
     version = "8.2.0"
     url = "https://pypi.python.org/packages/source/P/Pillow/Pillow-{version}.tar.gz"
     library = "libpillow.a"
     depends = [
         "hostpython3",
-        "host_setuptools3",
         "freetype",
         "libjpeg",
         "python3",
         "ios",
     ]
     python_depends = ["setuptools"]
     pbx_libraries = ["libz", "libbz2"]
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/pillow/bypass-find-library.patch` & `kivy-ios-2023.5.21/kivy_ios/recipes/pillow/bypass-find-library.patch`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/py3dns/ios.patch` & `kivy-ios-2023.5.21/kivy_ios/recipes/py3dns/ios.patch`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/pycrypto/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/pycrypto/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/python.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/python.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/python3/ModulesSetup` & `kivy-ios-2023.5.21/kivy_ios/recipes/python3/ModulesSetup`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 # Static compilation instructions for all binary modules.
 #####################################################################
 
 *static*
 _asyncio _asynciomodule.c
 _bisect _bisectmodule.c
 _blake2 _blake2/blake2module.c _blake2/blake2b_impl.c _blake2/blake2s_impl.c
-_sqlite3 -I$(srcdir)/Modules/_sqlite -DMODULE_NAME='\"sqlite3\"' _sqlite/cache.c _sqlite/connection.c _sqlite/cursor.c _sqlite/microprotocols.c _sqlite/module.c _sqlite/prepare_protocol.c _sqlite/row.c _sqlite/statement.c _sqlite/util.c
+_sqlite3 _sqlite/cache.c \
+        _sqlite/connection.c \
+        _sqlite/cursor.c \
+        _sqlite/microprotocols.c \
+        _sqlite/module.c \
+        _sqlite/prepare_protocol.c \
+        _sqlite/row.c \
+        _sqlite/statement.c \
+        _sqlite/util.c -DSQLITE_OMIT_LOAD_EXTENSION
 _bz2 _bz2module.c -I$(srcdir)/../bzip2/include -L$(srcdir)/../Support/BZip2 -lbz2
 _codecs_cn cjkcodecs/_codecs_cn.c
 _codecs_hk cjkcodecs/_codecs_hk.c
 _codecs_iso2022 cjkcodecs/_codecs_iso2022.c
 _codecs_jp cjkcodecs/_codecs_jp.c
 _codecs_kr cjkcodecs/_codecs_kr.c
 _codecs_tw cjkcodecs/_codecs_tw.c
@@ -44,16 +52,15 @@
 array arraymodule.c
 audioop audioop.c
 binascii binascii.c
 cmath cmathmodule.c _math.c
 fcntl fcntlmodule.c
 grp grpmodule.c
 math mathmodule.c
-# mmap mmapmodule.c
-parser parsermodule.c
+mmap mmapmodule.c
 pyexpat expat/xmlparse.c \
     expat/xmlrole.c \
     expat/xmltok.c \
     pyexpat.c \
     -I$(srcdir)/Modules/expat \
     -DHAVE_EXPAT_CONFIG_H -DUSE_PYEXPAT_CAPI -DXML_DEV_URANDOM
 resource resource.c
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/python3/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/python3/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,48 @@
 from kivy_ios.toolchain import Recipe, shprint
 from kivy_ios.context_managers import cd
 from os.path import join
 import sh
-import shutil
 import os
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 class Python3Recipe(Recipe):
-    version = "3.9.9"
+    version = "3.10.10"
     url = "https://www.python.org/ftp/python/{version}/Python-{version}.tgz"
     depends = ["hostpython3", "libffi", "openssl"]
-    library = "libpython3.9.a"
+    library = "libpython3.10.a"
     pbx_libraries = ["libz", "libbz2", "libsqlite3"]
 
     def init_with_ctx(self, ctx):
         super().init_with_ctx(ctx)
-        self.set_python(self, "3.9")
-        ctx.python_ver_dir = "python3.9"
+        self.set_python(self, "3.10")
+        ctx.python_ver_dir = "python3.10"
         ctx.python_prefix = join(ctx.dist_dir, "root", "python3")
         ctx.site_packages_dir = join(
             ctx.python_prefix, "lib", ctx.python_ver_dir, "site-packages")
 
     def prebuild_arch(self, arch):
         # common to all archs
         if self.has_marker("patched"):
             return
-        self.apply_patch("config.sub.patch")
         self.apply_patch("configure.patch")
         self.apply_patch("posixmodule.patch")
         self.apply_patch("dynload_shlib.patch")
         self.apply_patch("ctypes_duplicate.patch")
         self.copy_file("ModulesSetup", "Modules/Setup.local")
         self.append_file("ModulesSetup.mobile", "Modules/Setup.local")
         self.set_marker("patched")
 
     def postbuild_arch(self, arch):
-        # include _sqlite module to .a
-        py_arch = arch.arch
-        if py_arch == "arm64":
-            py_arch = "aarch64"
-        tmp_folder = "temp.ios-{}-3.9{}".format(py_arch, self.build_dir)
-        build_env = self.get_build_env(arch)
-        for o_file in [
-            "cache.o",
-            "connection.o",
-            "cursor.o",
-            "microprotocols.o",
-            "module.o",
-            "prepare_protocol.o",
-            "row.o",
-            "statement.o",
-            "util.o",
-        ]:
-            shprint(sh.Command(build_env['AR']),
-                    "-r",
-                    "{}/{}".format(self.build_dir, self.library),
-                    "{}/build/{}/Modules/_sqlite/{}".format(self.build_dir, tmp_folder, o_file))
-        print("Added _sqlite to archive")
+        # We need to skip remove_junk, because we need to keep few files.
+        # A cleanup will be done in the final step.
+        return
 
     def get_build_env(self, arch):
         build_env = arch.get_env()
         build_env["PATH"] = "{}:{}".format(
             join(self.ctx.dist_dir, "hostpython3", "bin"),
             os.environ["PATH"])
         build_env["CFLAGS"] += " --sysroot={}".format(arch.sysroot)
@@ -113,14 +92,17 @@
                 "ac_cv_func_futimesat=no",
                 "ac_cv_func_copy_file_range=no",
                 "ac_cv_func_fexecve=no",
                 "ac_cv_func_execve=no",
                 "ac_cv_func_sched_rr_get_interval=no",
                 "ac_cv_func_explicit_bzero=no",
                 "ac_cv_func_explicit_memset=no",
+                "ac_cv_func_close_range=no",
+                "ac_cv_func_splice=no",
+                "ac_cv_func_mremap=no",
                 "--host={}-apple-ios".format(py_arch),
                 "--build=x86_64-apple-darwin",
                 "--prefix={}".format(prefix),
                 "--without-ensurepip",
                 "--with-system-ffi",
                 "--enable-ipv6",
                 "PYTHON_FOR_BUILD=_PYTHON_PROJECT_BASE=$(abs_builddir) \
@@ -136,49 +118,40 @@
         build_env = self.get_build_env(arch)
         build_dir = self.get_build_dir(arch.arch)
         shprint(sh.make, self.ctx.concurrent_make,
                 "-C", build_dir,
                 "install",
                 "prefix={}".format(join(self.ctx.dist_dir, "root", "python3")),
                 _env=build_env)
-        self.install_mock_modules()
         self.reduce_python()
 
-    def install_mock_modules(self):
-        logger.info("Install mock modules")
-        sqlite3_src = join(self.recipe_dir, 'mock_modules', '_sqlite3')
-        site_packages_folder = join(
-                self.ctx.dist_dir, "root", "python3", "lib", "python3.9", "site-packages", "_sqlite3")
-        shutil.rmtree(site_packages_folder, ignore_errors=True)  # Needed in case of rebuild
-        shutil.copytree(sqlite3_src, site_packages_folder)
-
     def reduce_python(self):
         logger.info("Reduce python")
         logger.info("Remove files unlikely to be used")
         with cd(join(self.ctx.dist_dir, "root", "python3")):
             sh.rm("-rf", "bin", "share")
         # platform binaries and configuration
         with cd(join(
                 self.ctx.dist_dir, "root", "python3", "lib",
-                "python3.9", "config-3.9-darwin")):
+                "python3.10", "config-3.10-darwin")):
             sh.rm(
-                "libpython3.9.a",
+                "libpython3.10.a",
                 "python.o",
                 "config.c.in",
                 "makesetup",
                 "install-sh",
             )
 
         # cleanup pkgconfig and compiled lib
         with cd(join(self.ctx.dist_dir, "root", "python3", "lib")):
-            sh.rm("-rf", "pkgconfig", "libpython3.9.a")
+            sh.rm("-rf", "pkgconfig", "libpython3.10.a")
 
         # cleanup python libraries
         with cd(join(
-                self.ctx.dist_dir, "root", "python3", "lib", "python3.9")):
+                self.ctx.dist_dir, "root", "python3", "lib", "python3.10")):
             sh.rm("-rf", "wsgiref", "curses", "idlelib", "lib2to3",
                   "ensurepip", "turtledemo", "lib-dynload", "venv",
                   "pydoc_data")
             sh.find(".", "-path", "*/test*/*", "-delete")
             sh.find(".", "-name", "*.exe", "-type", "f", "-delete")
             sh.find(".", "-name", "test*", "-type", "d", "-delete")
             sh.find(".", "-iname", "*.pyc", "-delete")
@@ -191,17 +164,17 @@
             # sh.find(".", "-iname", "*.py", "-delete")
 
             # some pycache are recreated after compileall
             sh.find(".", "-path", "*/__pycache__/*", "-delete")
             sh.find(".", "-name", "__pycache__", "-type", "d", "-delete")
 
             # create the lib zip
-            logger.info("Create a python3.9.zip")
-            sh.mv("config-3.9-darwin", "..")
+            logger.info("Create a python3.10.zip")
+            sh.mv("config-3.10-darwin", "..")
             sh.mv("site-packages", "..")
-            sh.zip("-r", "../python39.zip", sh.glob("*"))
+            sh.zip("-r", "../python310.zip", sh.glob("*"))
             sh.rm("-rf", sh.glob("*"))
-            sh.mv("../config-3.9-darwin", ".")
+            sh.mv("../config-3.10-darwin", ".")
             sh.mv("../site-packages", ".")
 
 
 recipe = Python3Recipe()
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/python3/configure.patch` & `kivy-ios-2023.5.21/kivy_ios/recipes/python3/configure.patch`

 * *Files 11% similar despite different names*

```diff
@@ -1,90 +1,104 @@
-diff -Naur Python-3.8.2.orig/configure Python-3.8.2/configure
---- Python-3.8.2.orig/configure	2020-04-12 00:00:42.000000000 +0200
-+++ Python-3.8.2/configure	2020-04-12 00:08:45.000000000 +0200
-@@ -3271,6 +3271,15 @@
+diff -Naur Python-3.10.10.orig/configure Python-3.10.10/configure
+--- Python-3.10.10.orig/configure	2023-02-12 15:08:28
++++ Python-3.10.10/configure	2023-02-12 15:10:45
+@@ -3344,6 +3344,15 @@
  	*-*-cygwin*)
  		ac_sys_system=Cygwin
  		;;
 +  *-apple-ios)
-+  	ac_sys_system=iOS
-+  	;;
++    ac_sys_system=iOS
++    ;;
 +  *-apple-tvos)
-+  	ac_sys_system=tvOS
-+  	;;
++    ac_sys_system=tvOS
++    ;;
 +  *-apple-watchos)
-+  	ac_sys_system=watchOS
-+  	;;
++    ac_sys_system=watchOS
++    ;;
  	*-*-vxworks*)
  	    ac_sys_system=VxWorks
  	    ;;
-@@ -3318,6 +3327,15 @@
+@@ -3391,6 +3400,15 @@
  			_host_cpu=$host_cpu
  		esac
  		;;
 +  *-apple-*)
-+      case "$host_cpu" in
-+      arm*)
-+          _host_cpu=arm
-+          ;;
-+      *)
-+          _host_cpu=$host_cpu
++    case "$host_cpu" in
++    arm*)
++        _host_cpu=arm
++        ;;
++    *)
++        _host_cpu=$host_cpu
 +    esac
 +    ;;
  	*-*-cygwin*)
  		_host_cpu=
  		;;
-@@ -3396,6 +3414,13 @@
+@@ -3469,6 +3487,13 @@
      define_xopen_source=no;;
-   Darwin/1[0-9].*)
+   Darwin/[12][0-9].*)
      define_xopen_source=no;;
 +  # On iOS, defining _POSIX_C_SOURCE also disables platform specific features.
 +  iOS/*)
 +    define_xopen_source=no;;
 +  tvOS/*)
 +    define_xopen_source=no;;
 +  watchOS/*)
 +    define_xopen_source=no;;
-   # On AIX 4 and 5.1, mbstate_t is defined only when _XOPEN_SOURCE == 500 but
-   # used in wcsnrtombs() and mbsnrtowcs() even if _XOPEN_SOURCE is not defined
-   # or has another value. By not (re)defining it, the defaults come in place.
-@@ -6165,10 +6190,16 @@
+   # On QNX 6.3.2, defining _XOPEN_SOURCE prevents netdb.h from
+   # defining NI_NUMERICHOST.
+   QNX/6.3.2)
+@@ -5389,6 +5414,12 @@
+ case $ac_sys_system in #(
+   Darwin*) :
+     MULTIARCH="" ;; #(
++  iOS*) :
++    MULTIARCH="" ;; #(
++  tvOS*) :
++    MULTIARCH="" ;; #(
++  watchOS*) :
++    MULTIARCH="" ;; #(
+   FreeBSD*) :
+     MULTIARCH="" ;; #(
+   *) :
+@@ -6249,11 +6280,17 @@
  fi
  
  if test "$cross_compiling" = yes; then
 -    case "$READELF" in
 -	readelf|:)
 -	as_fn_error $? "readelf for the host is required for cross builds" "$LINENO" 5
 -	;;
+-    esac
 +    case "$host" in
 +    *-apple-*os)
 +        # readelf not required for iOS cross builds.
 +        ;;
 +    *)
 +        case "$READELF" in
 +            readelf|:)
 +            as_fn_error $? "readelf for the host is required for cross builds" "$LINENO" 5
 +            ;;
 +        esac
-     esac
++     esac
  fi
  
-@@ -6920,8 +6951,6 @@
+ 
+@@ -7051,7 +7088,6 @@
  # tweak BASECFLAGS based on compiler and platform
  case $GCC in
  yes)
 -    CFLAGS_NODIST="$CFLAGS_NODIST -std=c99"
--
+ 
      { $as_echo "$as_me:${as_lineno-$LINENO}: checking for -Wextra" >&5
  $as_echo_n "checking for -Wextra... " >&6; }
-      ac_save_cc="$CC"
-@@ -11438,6 +11467,10 @@
- 	;;
+@@ -11912,6 +11948,10 @@
+ then
+ 	case $ac_sys_system/$ac_sys_release in
  	hp*|HP*) DYNLOADFILE="dynload_hpux.o";;
 +  # Dynamic loading on iOS
 +  iOS/*) DYNLOADFILE="dynload_shlib.o";;
 +  tvOS/*) DYNLOADFILE="dynload_shlib.o";;
 +  watchOS/*) DYNLOADFILE="dynload_shlib.o";;
-	*)
+ 	*)
  	# use dynload_shlib.c and dlopen() if we have it; otherwise stub
  	# out any dynamic loading
- 	if test "$ac_cv_func_dlopen" = yes
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/python3/ctypes_duplicate.patch` & `kivy-ios-2023.5.21/kivy_ios/recipes/python3/ctypes_duplicate.patch`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/python3/dynload_shlib.patch` & `kivy-ios-2023.5.21/kivy_ios/recipes/python3/dynload_shlib.patch`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/pyyaml/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/pyyaml/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/sdl2/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/sdl2/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,21 @@
     version = "2.24.1"
     url = "https://github.com/libsdl-org/SDL/releases/download/release-{version}/SDL2-{version}.tar.gz"
     library = "Xcode/SDL/build/Release-{arch.sdk}/libSDL2.a"
     include_dir = "include"
     pbx_frameworks = [
         "OpenGLES", "AudioToolbox", "QuartzCore", "CoreGraphics",
         "CoreMotion", "GameController", "AVFoundation", "Metal",
-        "UIKit", "CoreHaptics", "CoreBluetooth"]
+        "UIKit", "CoreHaptics"]
 
     def prebuild_arch(self, arch):
         if self.has_marker("patched"):
             return
         self.apply_patch("uikit-transparent.patch")
+        self.apply_patch("disable-hidapi.patch")
         self.set_marker("patched")
 
     def build_arch(self, arch):
         env = arch.get_env()
         shprint(sh.xcodebuild, self.ctx.concurrent_xcodebuild,
                 "ONLY_ACTIVE_ARCH=NO",
                 "ARCHS={}".format(arch.arch),
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/sdl2/uikit-transparent.patch` & `kivy-ios-2023.5.21/kivy_ios/recipes/sdl2/uikit-transparent.patch`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/sdl2_image/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/sdl2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/sdl2_image/fix-ios-xcodebuild.patch` & `kivy-ios-2023.5.21/kivy_ios/recipes/sdl2_image/fix-ios-xcodebuild.patch`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/sdl2_mixer/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/sdl2_mixer/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/sdl2_ttf/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/sdl2_ttf/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/werkzeug/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/werkzeug/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/recipes/zbarlight/__init__.py` & `kivy-ios-2023.5.21/kivy_ios/recipes/zbarlight/__init__.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/toolchain.py` & `kivy-ios-2023.5.21/kivy_ios/toolchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -941,15 +941,15 @@
                     logger.info("Copy Include {} to {}".format(src_dir, dest))
                     ensure_dir(dirname(dest))
                     shutil.copy(src_dir, dest)
 
     @cache_execution
     def install_python_deps(self):
         for dep in self.python_depends:
-            _pip(["install", dep])
+            _pip(["install", "--no-deps", "--platform", "any", dep])
 
     @cache_execution
     def install(self):
         pass
 
     @classmethod
     def list_recipes(cls, **kwargs):
@@ -1174,15 +1174,24 @@
         "PYTHONOPTIMIZE": "2",
         # "PIP_INSTALL_TARGET": ctx.site_packages_dir
     }
 
     pip_path = join(ctx.dist_dir, 'hostpython3', 'bin', 'pip3')
 
     if len(args) > 1 and args[0] == "install":
-        pip_args = ["--isolated", "--prefix", ctx.python_prefix]
+        pip_args = ["--isolated"]
+
+        # --platform option requires --target, but --target can't be used
+        # with --prefix. We should prefer --prefix if it's possible,
+        # cause it notices already installed dependencies.
+        if "--platform" in args:
+            pip_args += ["--target", ctx.site_packages_dir]
+        else:
+            pip_args += ["--prefix", ctx.python_prefix]
+
         args = ["install"] + pip_args + args[1:]
 
     logger.info("Executing pip with: {}".format(args))
     pip_cmd = sh.Command(pip_path)
     shprint(pip_cmd, *args, _env=pip_env)
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/biglink` & `kivy-ios-2023.5.21/kivy_ios/tools/biglink`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/cythonize.py` & `kivy-ios-2023.5.21/kivy_ios/tools/cythonize.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/external/xcassets.py` & `kivy-ios-2023.5.21/kivy_ios/tools/external/xcassets.py`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/liblink` & `kivy-ios-2023.5.21/kivy_ios/tools/liblink`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/Storyboards/Launch Screen.storyboard` & `kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/Storyboards/Launch Screen.storyboard`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/README.txt` & `kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/README.txt`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/5509213687_ffd18df0b9_b.jpg` & `kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/5509213687_ffd18df0b9_b.jpg`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/5552597274_de8b3fb5d2_b.jpg` & `kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/5552597274_de8b3fb5d2_b.jpg`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/faust_github.jpg` & `kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/images/faust_github.jpg`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/pictures.kv` & `kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/pictures.kv`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/shadow32.png` & `kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/YourApp/shadow32.png`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/icon.png` & `kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/icon.png`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/main.m` & `kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/main.m`

 * *Files 9% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     // Export orientation preferences for Kivy
     export_orientation();
 
     NSString * resourcePath = [[NSBundle mainBundle] resourcePath];
     NSString *python_home = [NSString stringWithFormat:@"PYTHONHOME=%@", resourcePath, nil];
     putenv((char *)[python_home UTF8String]);
 
-    NSString *python_path = [NSString stringWithFormat:@"PYTHONPATH=%@:%@/lib/python3.9/:%@/lib/python3.9/site-packages:.", resourcePath, resourcePath, resourcePath, nil];
+    NSString *python_path = [NSString stringWithFormat:@"PYTHONPATH=%@:%@/lib/python3.10/:%@/lib/python3.10/site-packages:.", resourcePath, resourcePath, resourcePath, nil];
     putenv((char *)[python_path UTF8String]);
 
     NSString *tmp_path = [NSString stringWithFormat:@"TMP=%@/tmp", resourcePath, nil];
     putenv((char *)[tmp_path UTF8String]);
 
     NSLog(@"Initializing python");
     Py_Initialize();
@@ -142,14 +142,15 @@
         "    import _imp\n" \
         "    EXTS = _imp.extension_suffixes()\n" \
         "    sys.modules['subprocess'] = types.ModuleType(name='subprocess')\n" \
         "    sys.modules['subprocess'].PIPE = None\n" \
         "    sys.modules['subprocess'].STDOUT = None\n" \
         "    sys.modules['subprocess'].DEVNULL = None\n" \
         "    sys.modules['subprocess'].CalledProcessError = Exception\n" \
+        "    sys.modules['subprocess'].CompletedProcess = None\n" \
         "    sys.modules['subprocess'].check_output = None\n" \
         "except ImportError:\n" \
         "    EXTS = ['.so']\n"
         "# Fake redirection to supress console output\n" \
         "if environ.get('KIVY_NO_CONSOLE', '0') == '1':\n" \
         "    class fakestd(object):\n" \
         "        def write(self, *args, **kw): pass\n" \
```

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}-Info.plist` & `kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}-Info.plist`

 * *Files identical despite different names*

### Comparing `kivy-ios-2023.1.29/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}.xcodeproj/project.pbxproj` & `kivy-ios-2023.5.21/kivy_ios/tools/templates/{{ cookiecutter.project_name }}-ios/{{ cookiecutter.project_name }}.xcodeproj/project.pbxproj`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
 				GCC_DYNAMIC_NO_PIC = NO;
 				GCC_OPTIMIZATION_LEVEL = 0;
 				GCC_PRECOMPILE_PREFIX_HEADER = YES;
 				GCC_PREFIX_HEADER = "";
 				GCC_PREPROCESSOR_DEFINITIONS = "DEBUG=1";
 				GCC_VERSION = com.apple.compilers.llvm.clang.1_0;
 				HEADER_SEARCH_PATHS = (
-					"{{ cookiecutter.dist_dir }}/root/python3/include/python3.9/**",
+					"{{ cookiecutter.dist_dir }}/root/python3/include/python3.10/**",
 					"{{ cookiecutter.dist_dir }}/include/common/sdl2",
 				);
 				INFOPLIST_FILE = "{{ cookiecutter.project_name }}-Info.plist";
 				IPHONEOS_DEPLOYMENT_TARGET = 9.0;
 				LIBRARY_SEARCH_PATHS = (
 					"$(inherited)",
 					"{{ cookiecutter.dist_dir }}/lib",
@@ -286,15 +286,15 @@
 				EXCLUDED_ARCHS = "";
 				"EXCLUDED_ARCHS[sdk=iphonesimulator*]" = arm64;
 				FRAMEWORK_SEARCH_PATHS = "{{ cookiecutter.dist_dir }}/frameworks";
 				GCC_PRECOMPILE_PREFIX_HEADER = YES;
 				GCC_PREFIX_HEADER = "";
 				GCC_VERSION = com.apple.compilers.llvm.clang.1_0;
 				HEADER_SEARCH_PATHS = (
-					"{{ cookiecutter.dist_dir }}/root/python3/include/python3.9/**",
+					"{{ cookiecutter.dist_dir }}/root/python3/include/python3.10/**",
 					"{{ cookiecutter.dist_dir }}/include/common/sdl2",
 				);
 				INFOPLIST_FILE = "{{ cookiecutter.project_name }}-Info.plist";
 				IPHONEOS_DEPLOYMENT_TARGET = 9.0;
 				LIBRARY_SEARCH_PATHS = (
 					"$(inherited)",
 					"{{ cookiecutter.dist_dir }}/lib",
```

### Comparing `kivy-ios-2023.1.29/kivy_ios.egg-info/PKG-INFO` & `kivy-ios-2023.5.21/kivy_ios.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivy-ios
-Version: 2023.1.29
+Version: 2023.5.21
 Summary: Kivy for iOS
 Home-page: https://github.com/kivy/kivy-ios
 Author: The Kivy team
 Author-email: kivy-dev@googlegroups.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,15 +41,15 @@
 
 Install [Kivy for iOS from PyPI](https://pypi.org/project/kivy-ios) with pip like any Python package.
 
       pip3 install kivy-ios
 
 Additionally, you would need a few system dependencies and configuration.
 
-- Xcode 10 or above, with an iOS SDK and command line tools installed:
+- Xcode 13 or above, with an iOS SDK and command line tools installed:
 
       xcode-select --install
 
 - Using brew, you can install the following dependencies:
 
       brew install autoconf automake libtool pkg-config
       brew link libtool
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kivy-ios Version: 2023.1.29 Summary: Kivy for iOS
+Metadata-Version: 2.1 Name: kivy-ios Version: 2023.5.21 Summary: Kivy for iOS
 Home-page: https://github.com/kivy/kivy-ios Author: The Kivy team Author-email:
 kivy-dev@googlegroups.com License: MIT License Description-Content-Type: text/
 markdown License-File: LICENSE # Kivy for iOS [![kivy-ios](https://github.com/
 kivy/kivy-ios/workflows/kivy-ios/badge.svg)](https://github.com/kivy/kivy-ios/
 actions?query=workflow%3Akivy-ios) [![PyPI version](https://badge.fury.io/py/
 kivy-ios.svg)](https://badge.fury.io/py/kivy-ios) [![Backers on Open
 Collective](https://opencollective.com/kivy/backers/badge.svg)](#backers) [!
@@ -13,15 +13,15 @@
 need to compile it at least once before creating your Xcode project. The
 toolchain supports: - iPhone Simulator (x86_64) - iPhone / iOS (arm64) These
 recipes are not ported to the new toolchain yet: - lxml ## Installation &
 requirements Before we start, we strongly advise using a Python virtual
 environment to install Python packages. python3 -m venv venv . venv/bin/
 activate Install [Kivy for iOS from PyPI](https://pypi.org/project/kivy-ios)
 with pip like any Python package. pip3 install kivy-ios Additionally, you would
-need a few system dependencies and configuration. - Xcode 10 or above, with an
+need a few system dependencies and configuration. - Xcode 13 or above, with an
 iOS SDK and command line tools installed: xcode-select --install - Using brew,
 you can install the following dependencies: brew install autoconf automake
 libtool pkg-config brew link libtool ## Using the toolchain Any Python
 extensions or C/C++ library must be compiled: you need to have what we call a
 `recipe` to compile it. For example, Python, libffi, SDL2, SDL_image,
 freetype... all the dependencies, compilation, and packaging instructions are
 contained in a `recipe`. You can list the available recipes and their versions
```

### Comparing `kivy-ios-2023.1.29/kivy_ios.egg-info/SOURCES.txt` & `kivy-ios-2023.5.21/kivy_ios.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,21 +21,18 @@
 kivy_ios/recipes/curly/__init__.py
 kivy_ios/recipes/cymunk/__init__.py
 kivy_ios/recipes/ffmpeg/__init__.py
 kivy_ios/recipes/ffpyplayer/__init__.py
 kivy_ios/recipes/ffpyplayer/misc-visibility.patch
 kivy_ios/recipes/flask/__init__.py
 kivy_ios/recipes/freetype/__init__.py
-kivy_ios/recipes/host_setuptools/__init__.py
-kivy_ios/recipes/host_setuptools/setuptools/README.rst
-kivy_ios/recipes/host_setuptools3/__init__.py
-kivy_ios/recipes/host_setuptools3/setuptools/README.rst
 kivy_ios/recipes/hostopenssl/__init__.py
 kivy_ios/recipes/hostpython3/ModulesSetup
 kivy_ios/recipes/hostpython3/__init__.py
+kivy_ios/recipes/hostpython3/allow-cflags-override.patch
 kivy_ios/recipes/hostpython3/disable_sysconfig_cflags.patch
 kivy_ios/recipes/ios/__init__.py
 kivy_ios/recipes/ios/src/ios.pyx
 kivy_ios/recipes/ios/src/ios_browser.m
 kivy_ios/recipes/ios/src/ios_filechooser.m
 kivy_ios/recipes/ios/src/ios_mail.m
 kivy_ios/recipes/ios/src/ios_utils.m
@@ -52,37 +49,36 @@
 kivy_ios/recipes/libpng/__init__.py
 kivy_ios/recipes/libzbar/__init__.py
 kivy_ios/recipes/libzbar/werror.patch
 kivy_ios/recipes/markupsafe/__init__.py
 kivy_ios/recipes/netifaces/__init__.py
 kivy_ios/recipes/numpy/__init__.py
 kivy_ios/recipes/numpy/duplicated_symbols.patch
+kivy_ios/recipes/numpy/skip-math-test.patch
 kivy_ios/recipes/openssl/__init__.py
 kivy_ios/recipes/photolibrary/__init__.py
 kivy_ios/recipes/pillow/__init__.py
 kivy_ios/recipes/pillow/bypass-find-library.patch
 kivy_ios/recipes/plyer/__init__.py
 kivy_ios/recipes/py3dns/__init__.py
 kivy_ios/recipes/py3dns/ios.patch
 kivy_ios/recipes/pycrypto/__init__.py
 kivy_ios/recipes/pycrypto/hash_SHA2_template.c.patch
 kivy_ios/recipes/pykka/__init__.py
 kivy_ios/recipes/pyobjus/__init__.py
 kivy_ios/recipes/python3/ModulesSetup
 kivy_ios/recipes/python3/ModulesSetup.mobile
 kivy_ios/recipes/python3/__init__.py
-kivy_ios/recipes/python3/config.sub.patch
 kivy_ios/recipes/python3/configure.patch
 kivy_ios/recipes/python3/ctypes_duplicate.patch
 kivy_ios/recipes/python3/dynload_shlib.patch
 kivy_ios/recipes/python3/posixmodule.patch
-kivy_ios/recipes/python3/mock_modules/_sqlite3/__init__.py
-kivy_ios/recipes/python3/mock_modules/_sqlite3/_sqlite3.cpython-39-darwin.so
 kivy_ios/recipes/pyyaml/__init__.py
 kivy_ios/recipes/sdl2/__init__.py
+kivy_ios/recipes/sdl2/disable-hidapi.patch
 kivy_ios/recipes/sdl2/uikit-transparent.patch
 kivy_ios/recipes/sdl2_image/__init__.py
 kivy_ios/recipes/sdl2_image/fix-ios-xcodebuild.patch
 kivy_ios/recipes/sdl2_mixer/__init__.py
 kivy_ios/recipes/sdl2_ttf/__init__.py
 kivy_ios/recipes/werkzeug/__init__.py
 kivy_ios/recipes/zbarlight/__init__.py
```

### Comparing `kivy-ios-2023.1.29/setup.cfg` & `kivy-ios-2023.5.21/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kivy-ios
-version = 2023.01.29
+version = 2023.05.21
 description = Kivy for iOS
 license = MIT License
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = The Kivy team
 author_email = kivy-dev@googlegroups.com
 url = https://github.com/kivy/kivy-ios
```

