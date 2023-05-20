# Comparing `tmp/xspf-lib-0.3.0.tar.gz` & `tmp/xspf_lib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xspf-lib-0.3.0.tar", last modified: Sat May 13 23:06:31 2023, max compression
+gzip compressed data, was "xspf_lib-0.3.1.tar", last modified: Sat May 20 22:04:05 2023, max compression
```

## Comparing `xspf-lib-0.3.0.tar` & `xspf_lib-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:06:31.407983 xspf-lib-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-13 23:06:31.407983 xspf-lib-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 23:06:31.407983 xspf-lib-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:06:31.407983 xspf-lib-0.3.0/xspf_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-13 23:06:21.000000 xspf-lib-0.3.0/xspf_lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 23:06:31.407983 xspf-lib-0.3.0/xspf_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-13 23:06:31.000000 xspf-lib-0.3.0/xspf_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-13 23:06:31.000000 xspf-lib-0.3.0/xspf_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 23:06:31.000000 xspf-lib-0.3.0/xspf_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-13 23:06:31.000000 xspf-lib-0.3.0/xspf_lib.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1072 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3321 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/README.rst
+-rw-r--r--   0        0        0     1016 2023-05-20 22:04:05.828345 xspf_lib-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     6975 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/test_module.py
+-rw-r--r--   0        0        0     3523 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/test_testcases_fail_validation.py
+-rw-r--r--   0        0        0     8113 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/test_testcases_pass_validation.py
+-rw-r--r--   0        0        0      260 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/test_uri.py
+-rw-r--r--   0        0        0      126 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/README.txt
+-rw-r--r--   0        0        0      198 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-attribute-forbidden-annotation.xspf
+-rw-r--r--   0        0        0      149 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-attribute-forbidden-playlist.xspf
+-rw-r--r--   0        0        0      382 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-baddate.xspf
+-rw-r--r--   0        0        0      237 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-badversion.xspf
+-rw-r--r--   0        0        0      190 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-element-forbidden-attribution.xspf
+-rw-r--r--   0        0        0      159 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-extension-application-missing.xspf
+-rw-r--r--   0        0        0      153 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-link-rel-missing.xspf
+-rw-r--r--   0        0        0      323 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-markup-annotation.xspf
+-rw-r--r--   0        0        0      314 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-markup-creator.xspf
+-rw-r--r--   0        0        0      331 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-markup-meta.xspf
+-rw-r--r--   0        0        0      308 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-markup-title.xspf
+-rw-r--r--   0        0        0      153 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-meta-rel-missing.xspf
+-rw-r--r--   0        0        0      232 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-missingtracklist.xspf
+-rw-r--r--   0        0        0      182 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-missingversion.xspf
+-rw-r--r--   0        0        0      199 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-namespace-missing.xspf
+-rw-r--r--   0        0        0      289 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-namespace-nested-broken.xspf
+-rw-r--r--   0        0        0      381 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-namespace-wrong-string.xspf
+-rw-r--r--   0        0        0      120 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-nonleaf-content-attribution.xspf
+-rw-r--r--   0        0        0       93 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-nonleaf-content-playlist.xspf
+-rw-r--r--   0        0        0      100 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-nonleaf-content-trackList.xspf
+-rw-r--r--   0        0        0      127 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-root-name.xspf
+-rw-r--r--   0        0        0      313 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-toomany-annotation.xspf
+-rw-r--r--   0        0        0      279 2023-05-20 22:03:57.812240 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-toomany-attribution.xspf
+-rw-r--r--   0        0        0      299 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-toomany-creator.xspf
+-rw-r--r--   0        0        0      320 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-toomany-date.xspf
+-rw-r--r--   0        0        0      336 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-toomany-identifier.xspf
+-rw-r--r--   0        0        0      311 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-toomany-image.xspf
+-rw-r--r--   0        0        0      330 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-toomany-info.xspf
+-rw-r--r--   0        0        0      321 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-toomany-license.xspf
+-rw-r--r--   0        0        0      350 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-toomany-location.xspf
+-rw-r--r--   0        0        0      289 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-toomany-title.xspf
+-rw-r--r--   0        0        0      257 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/playlist-toomany-tracklist.xspf
+-rw-r--r--   0        0        0      370 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-badint-duration.xspf
+-rw-r--r--   0        0        0      370 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-badint-tracknum.xspf
+-rw-r--r--   0        0        0      194 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-extension-application-missing.xspf
+-rw-r--r--   0        0        0      188 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-link-rel-missing.xspf
+-rw-r--r--   0        0        0      316 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-markup-album.xspf
+-rw-r--r--   0        0        0      336 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-markup-annotation.xspf
+-rw-r--r--   0        0        0      324 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-markup-creator.xspf
+-rw-r--r--   0        0        0      338 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-markup-meta.xspf
+-rw-r--r--   0        0        0      316 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-markup-title.xspf
+-rw-r--r--   0        0        0      188 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-meta-rel-missing.xspf
+-rw-r--r--   0        0        0      123 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-nonleaf-content.xspf
+-rw-r--r--   0        0        0      342 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-toomany-album.xspf
+-rw-r--r--   0        0        0      372 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-toomany-annotation.xspf
+-rw-r--r--   0        0        0      354 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-toomany-creator.xspf
+-rw-r--r--   0        0        0      352 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-toomany-duration.xspf
+-rw-r--r--   0        0        0      364 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-toomany-image.xspf
+-rw-r--r--   0        0        0      358 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-toomany-info.xspf
+-rw-r--r--   0        0        0      342 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-toomany-title.xspf
+-rw-r--r--   0        0        0      352 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/fail/track-toomany-tracknum.xspf
+-rw-r--r--   0        0        0      605 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-broken-relative-paths.xspf
+-rw-r--r--   0        0        0      137 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-empty-annotation.xspf
+-rw-r--r--   0        0        0      134 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-empty-creator.xspf
+-rw-r--r--   0        0        0      157 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-empty-meta.xspf
+-rw-r--r--   0        0        0      132 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-empty-title.xspf
+-rw-r--r--   0        0        0      379 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-extension.xspf
+-rw-r--r--   0        0        0     3342 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-extensive.xspf
+-rw-r--r--   0        0        0      869 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-inverted-order.xspf
+-rw-r--r--   0        0        0      250 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-namespace-nested-proper.xspf
+-rw-r--r--   0        0        0      139 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-namespace-nondefault.xspf
+-rw-r--r--   0        0        0      205 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-namespace-two-additions.xspf
+-rw-r--r--   0        0        0      336 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-noturi-attribution-identifier.xspf
+-rw-r--r--   0        0        0      330 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-noturi-attribution-location.xspf
+-rw-r--r--   0        0        0      317 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-noturi-extension.xspf
+-rw-r--r--   0        0        0      298 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-noturi-identifier.xspf
+-rw-r--r--   0        0        0      283 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-noturi-image.xspf
+-rw-r--r--   0        0        0      280 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-noturi-info.xspf
+-rw-r--r--   0        0        0      289 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-noturi-license.xspf
+-rw-r--r--   0        0        0      305 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-noturi-link-content.xspf
+-rw-r--r--   0        0        0      314 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-noturi-link-rel.xspf
+-rw-r--r--   0        0        0      292 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-noturi-location.xspf
+-rw-r--r--   0        0        0      303 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-noturi-meta.xspf
+-rw-r--r--   0        0        0      572 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-relative-paths.xspf
+-rw-r--r--   0        0        0      162 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-whitespace-dateTime.xspf
+-rw-r--r--   0        0        0     1543 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/playlist-xml-base.xspf
+-rw-r--r--   0        0        0      174 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-empty-album.xspf
+-rw-r--r--   0        0        0      179 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-empty-annotation.xspf
+-rw-r--r--   0        0        0      176 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-empty-creator.xspf
+-rw-r--r--   0        0        0      199 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-empty-meta.xspf
+-rw-r--r--   0        0        0      174 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-empty-title.xspf
+-rw-r--r--   0        0        0      320 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-extension.xspf
+-rw-r--r--   0        0        0     4160 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-extensive.xspf
+-rw-r--r--   0        0        0      917 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-inverted-order.xspf
+-rw-r--r--   0        0        0      342 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-noturi-extension.xspf
+-rw-r--r--   0        0        0      329 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-noturi-identifier.xspf
+-rw-r--r--   0        0        0      309 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-noturi-image.xspf
+-rw-r--r--   0        0        0      305 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-noturi-info.xspf
+-rw-r--r--   0        0        0      353 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-noturi-link-rel.xspf
+-rw-r--r--   0        0        0      330 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-noturi-link.xspf
+-rw-r--r--   0        0        0      321 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-noturi-location.xspf
+-rw-r--r--   0        0        0      342 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-noturi-meta-rel.xspf
+-rw-r--r--   0        0        0      412 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-whitespace-anyURI.xspf
+-rw-r--r--   0        0        0      414 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-whitespace-in-between.xspf
+-rw-r--r--   0        0        0      326 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/tests/testcase/version_1/pass/track-whitespace-nonNegativeInteger.xspf
+-rw-r--r--   0        0        0      353 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/xspf_lib/__init__.py
+-rw-r--r--   0        0        0      268 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/xspf_lib/base.py
+-rw-r--r--   0        0        0     4437 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/xspf_lib/builders.py
+-rw-r--r--   0        0        0      386 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/xspf_lib/constants.py
+-rw-r--r--   0        0        0    14039 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/xspf_lib/elements.py
+-rw-r--r--   0        0        0    13174 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/xspf_lib/parsers.py
+-rw-r--r--   0        0        0      358 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/xspf_lib/types.py
+-rw-r--r--   0        0        0      604 2023-05-20 22:03:57.816241 xspf_lib-0.3.1/xspf_lib/utils.py
+-rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 xspf_lib-0.3.1/PKG-INFO
```

### Comparing `xspf-lib-0.3.0/LICENSE` & `xspf_lib-0.3.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Dzmitry Izaitka
+Copyright (c) 2023 Dzmitry Izaitka
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `xspf-lib-0.3.0/PKG-INFO` & `xspf_lib-0.3.1/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,74 @@
-Metadata-Version: 2.1
-Name: xspf-lib
-Version: 0.3.0
-Summary: Library for work with xspf format
-Home-page: https://github.com/dem214/xspf-lib
-Author: Dzmitry Izaitka
-Author-email: dem214overlord@gmail.com
-License: UNKNOWN
-Description: ========
-        xspf-lib
-        ========
-        
-        .. image:: https://github.com/dem214/xspf-lib/workflows/Python%20package/badge.svg?branch=master
-            :alt: Python package
-        .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
-            :target: https://pycqa.github.io/isort/
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-        .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
-           :target: https://github.com/pre-commit/pre-commit
-           :alt: pre-commit
-        
-        
-        Library to work with xspf.
-        
-        Requirements
-        ------------
-        
-        * `Python 3.8 or higher <https://www.python.org/downloads/>`_
-        
-        Installing
-        ----------
-        
-        Install and update via `pip`_:
-        
-        .. code-block:: text
-        
-            pip install -U xspf-lib
-        
-        Example
-        -------
-        1. Generating new playlist.
-        
-        >>> import xspf_lib as xspf
-        >>> killer_queen = xspf.Track(location="file:///home/music/killer_queen.mp3",
-                                      title="Killer Queen",
-                                      creator="Queen",
-                                      album="Sheer Heart Attack",
-                                      trackNum=2,
-                                      duration=177000,
-                                      annotation="#2 in GB 1975",
-                                      info="https://ru.wikipedia.org/wiki/Killer_Queen",
-                                      image="file:///home/images/killer_queen_cover.png")
-        >>> anbtd = xspf.Track()
-        >>> anbtd.location = ["https://freemusic.example.com/loc.ogg",
-                              "file:///home/music/anbtd.mp3"]
-        >>> anbtd.title = "Another One Bites the Dust"
-        >>> anbtd.creator = "Queen"
-        >>> anbtd.identifier = ["id1.group"]
-        >>> anbtd.link = [xspf.Link("link.namespace", "link.uri.info")]
-        >>> anbtd.meta = [xspf.Meta("meta.namespace", "METADATA_INFO")]
-        >>> playlist = xspf.Playlist(title="Some Tracks",
-                                     creator="myself",
-                                     annotation="I did this only for examples!.",
-                                     trackList=[killer_queen, anbtd])
-        >>> print(playlist.xml_string())
-        <playlist version="1" xmlns="http://xspf.org/ns/0/"><title>Some Tracks</title><creator>myself</creator><annotation>I did this only for examples!.</annotation><date>2020-02-03T14:29:59.199202+03:00</date><trackList><track><location>file:///home/music/killer_queen.mp3</location><title>Killer Queen</title><creator>Queen</creator><annotation>#2 in GB 1975</annotation><info>https://ru.wikipedia.org/wiki/Killer_Queen</info><image>file:///home/images/killer_queen_cover.png</image><album>Sheer Heart Attack</album><trackNum>2</trackNum><duration>177000</duration></track><track><location>https://freemusic.example.com/loc.ogg</location><location>file:///home/music/anbtd.mp3</location><identifier>id1.group</identifier><title>Another One Bites the Dust</title><creator>Queen</creator><link rel="link.namespace">link.uri.info</link><meta rel="meta.namespace">METADATA_INFO</meta></track></trackList></playlist>
-        >>> playlist.write("some_tracks.xspf")
-        
-        2. Parsing from file.
-        
-        >>> from xspf_lib import Playlist
-        >>> playlist = Playlist.parse("some_tracks.xspf")
-        
-        License
-        -------
-        
-        The license of the project is MIT License - see LICENSE_ file for details.
-        
-        .. _LICENSE: https://github.com/dem214/xspf-lib/blob/master/LICENSE
-        
-        .. _pip: https://pip.pypa.io/en/stable/quickstart
-        
-Keywords: xspf playlist
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Multimedia :: Video
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
+========
+xspf-lib
+========
+
+.. image:: https://github.com/dem214/xspf-lib/workflows/Python%20package/badge.svg?branch=master
+    :alt: Python package
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+    :target: https://pycqa.github.io/isort/
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
+
+
+Library to work with xspf.
+
+Requirements
+------------
+
+* `Python 3.8 or higher <https://www.python.org/downloads/>`_
+
+Installing
+----------
+
+Install and update via `pip`_:
+
+.. code-block:: text
+
+    pip install -U xspf-lib
+
+Example
+-------
+1. Generating new playlist.
+
+>>> import xspf_lib as xspf
+>>> killer_queen = xspf.Track(location="file:///home/music/killer_queen.mp3",
+                              title="Killer Queen",
+                              creator="Queen",
+                              album="Sheer Heart Attack",
+                              trackNum=2,
+                              duration=177000,
+                              annotation="#2 in GB 1975",
+                              info="https://ru.wikipedia.org/wiki/Killer_Queen",
+                              image="file:///home/images/killer_queen_cover.png")
+>>> anbtd = xspf.Track()
+>>> anbtd.location = ["https://freemusic.example.com/loc.ogg",
+                      "file:///home/music/anbtd.mp3"]
+>>> anbtd.title = "Another One Bites the Dust"
+>>> anbtd.creator = "Queen"
+>>> anbtd.identifier = ["id1.group"]
+>>> anbtd.link = [xspf.Link("link.namespace", "link.uri.info")]
+>>> anbtd.meta = [xspf.Meta("meta.namespace", "METADATA_INFO")]
+>>> playlist = xspf.Playlist(title="Some Tracks",
+                             creator="myself",
+                             annotation="I did this only for examples!.",
+                             trackList=[killer_queen, anbtd])
+>>> print(playlist.xml_string())
+<playlist version="1" xmlns="http://xspf.org/ns/0/"><title>Some Tracks</title><creator>myself</creator><annotation>I did this only for examples!.</annotation><date>2020-02-03T14:29:59.199202+03:00</date><trackList><track><location>file:///home/music/killer_queen.mp3</location><title>Killer Queen</title><creator>Queen</creator><annotation>#2 in GB 1975</annotation><info>https://ru.wikipedia.org/wiki/Killer_Queen</info><image>file:///home/images/killer_queen_cover.png</image><album>Sheer Heart Attack</album><trackNum>2</trackNum><duration>177000</duration></track><track><location>https://freemusic.example.com/loc.ogg</location><location>file:///home/music/anbtd.mp3</location><identifier>id1.group</identifier><title>Another One Bites the Dust</title><creator>Queen</creator><link rel="link.namespace">link.uri.info</link><meta rel="meta.namespace">METADATA_INFO</meta></track></trackList></playlist>
+>>> playlist.write("some_tracks.xspf")
+
+2. Parsing from file.
+
+>>> from xspf_lib import Playlist
+>>> playlist = Playlist.parse("some_tracks.xspf")
+
+License
+-------
+
+The license of the project is MIT License - see LICENSE_ file for details.
+
+.. _LICENSE: https://github.com/dem214/xspf-lib/blob/master/LICENSE
+
+.. _pip: https://pip.pypa.io/en/stable/quickstart
```

#### html2text {}

```diff
@@ -1,10 +1,7 @@
-Metadata-Version: 2.1 Name: xspf-lib Version: 0.3.0 Summary: Library for work
-with xspf format Home-page: https://github.com/dem214/xspf-lib Author: Dzmitry
-Izaitka Author-email: dem214overlord@gmail.com License: UNKNOWN Description:
 ======== xspf-lib ======== .. image:: https://github.com/dem214/xspf-lib/
 workflows/Python%20package/badge.svg?branch=master :alt: Python package ..
 image:: https://img.shields.io/badge/%20imports-isort-
 %231674b1?style=flat&labelColor=ef8336 :target: https://pycqa.github.io/isort/
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg :target:
 https://github.com/psf/black .. image:: https://img.shields.io/badge/pre--
 commit-enabled-brightgreen?logo=pre-commit :target: https://github.com/pre-
@@ -31,13 +28,8 @@
 freemusic.example.com/loc.oggfile:///home/music/anbtd.mp3id1.group
 Queen
 link.uri.info
 METADATA_INFO >>> playlist.write("some_tracks.xspf") 2. Parsing from file. >>>
 from xspf_lib import Playlist >>> playlist = Playlist.parse("some_tracks.xspf")
 License ------- The license of the project is MIT License - see LICENSE_ file
 for details. .. _LICENSE: https://github.com/dem214/xspf-lib/blob/master/
-LICENSE .. _pip: https://pip.pypa.io/en/stable/quickstart Keywords: xspf
-playlist Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
-OS Independent Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Multimedia :: Sound/Audio Classifier: Topic ::
-Multimedia :: Video Requires-Python: >=3.7 Description-Content-Type: text/x-rst
+LICENSE .. _pip: https://pip.pypa.io/en/stable/quickstart
```

### Comparing `xspf-lib-0.3.0/xspf_lib/builders.py` & `xspf_lib-0.3.1/xspf_lib/builders.py`

 * *Files identical despite different names*

### Comparing `xspf-lib-0.3.0/xspf_lib/elements.py` & `xspf_lib-0.3.1/xspf_lib/elements.py`

 * *Files identical despite different names*

### Comparing `xspf-lib-0.3.0/xspf_lib/parsers.py` & `xspf_lib-0.3.1/xspf_lib/parsers.py`

 * *Files identical despite different names*

### Comparing `xspf-lib-0.3.0/xspf_lib/utils.py` & `xspf_lib-0.3.1/xspf_lib/utils.py`

 * *Files identical despite different names*

### Comparing `xspf-lib-0.3.0/xspf_lib.egg-info/PKG-INFO` & `xspf_lib-0.3.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,92 @@
 Metadata-Version: 2.1
 Name: xspf-lib
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library for work with xspf format
-Home-page: https://github.com/dem214/xspf-lib
-Author: Dzmitry Izaitka
-Author-email: dem214overlord@gmail.com
-License: UNKNOWN
-Description: ========
-        xspf-lib
-        ========
-        
-        .. image:: https://github.com/dem214/xspf-lib/workflows/Python%20package/badge.svg?branch=master
-            :alt: Python package
-        .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
-            :target: https://pycqa.github.io/isort/
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/psf/black
-        .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
-           :target: https://github.com/pre-commit/pre-commit
-           :alt: pre-commit
-        
-        
-        Library to work with xspf.
-        
-        Requirements
-        ------------
-        
-        * `Python 3.8 or higher <https://www.python.org/downloads/>`_
-        
-        Installing
-        ----------
-        
-        Install and update via `pip`_:
-        
-        .. code-block:: text
-        
-            pip install -U xspf-lib
-        
-        Example
-        -------
-        1. Generating new playlist.
-        
-        >>> import xspf_lib as xspf
-        >>> killer_queen = xspf.Track(location="file:///home/music/killer_queen.mp3",
-                                      title="Killer Queen",
-                                      creator="Queen",
-                                      album="Sheer Heart Attack",
-                                      trackNum=2,
-                                      duration=177000,
-                                      annotation="#2 in GB 1975",
-                                      info="https://ru.wikipedia.org/wiki/Killer_Queen",
-                                      image="file:///home/images/killer_queen_cover.png")
-        >>> anbtd = xspf.Track()
-        >>> anbtd.location = ["https://freemusic.example.com/loc.ogg",
-                              "file:///home/music/anbtd.mp3"]
-        >>> anbtd.title = "Another One Bites the Dust"
-        >>> anbtd.creator = "Queen"
-        >>> anbtd.identifier = ["id1.group"]
-        >>> anbtd.link = [xspf.Link("link.namespace", "link.uri.info")]
-        >>> anbtd.meta = [xspf.Meta("meta.namespace", "METADATA_INFO")]
-        >>> playlist = xspf.Playlist(title="Some Tracks",
-                                     creator="myself",
-                                     annotation="I did this only for examples!.",
-                                     trackList=[killer_queen, anbtd])
-        >>> print(playlist.xml_string())
-        <playlist version="1" xmlns="http://xspf.org/ns/0/"><title>Some Tracks</title><creator>myself</creator><annotation>I did this only for examples!.</annotation><date>2020-02-03T14:29:59.199202+03:00</date><trackList><track><location>file:///home/music/killer_queen.mp3</location><title>Killer Queen</title><creator>Queen</creator><annotation>#2 in GB 1975</annotation><info>https://ru.wikipedia.org/wiki/Killer_Queen</info><image>file:///home/images/killer_queen_cover.png</image><album>Sheer Heart Attack</album><trackNum>2</trackNum><duration>177000</duration></track><track><location>https://freemusic.example.com/loc.ogg</location><location>file:///home/music/anbtd.mp3</location><identifier>id1.group</identifier><title>Another One Bites the Dust</title><creator>Queen</creator><link rel="link.namespace">link.uri.info</link><meta rel="meta.namespace">METADATA_INFO</meta></track></trackList></playlist>
-        >>> playlist.write("some_tracks.xspf")
-        
-        2. Parsing from file.
-        
-        >>> from xspf_lib import Playlist
-        >>> playlist = Playlist.parse("some_tracks.xspf")
-        
-        License
-        -------
-        
-        The license of the project is MIT License - see LICENSE_ file for details.
-        
-        .. _LICENSE: https://github.com/dem214/xspf-lib/blob/master/LICENSE
-        
-        .. _pip: https://pip.pypa.io/en/stable/quickstart
-        
 Keywords: xspf playlist
-Platform: UNKNOWN
+Author-Email: Dzmitry Izaitka <dem214overlord@gmail.com>
+License: MIT
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Source, https://github.com/dem214/xspf-lib
+Project-URL: Bug tracker, https://github.com/dem214/xspf-lib/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+
+========
+xspf-lib
+========
+
+.. image:: https://github.com/dem214/xspf-lib/workflows/Python%20package/badge.svg?branch=master
+    :alt: Python package
+.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+    :target: https://pycqa.github.io/isort/
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
+
+
+Library to work with xspf.
+
+Requirements
+------------
+
+* `Python 3.8 or higher <https://www.python.org/downloads/>`_
+
+Installing
+----------
+
+Install and update via `pip`_:
+
+.. code-block:: text
+
+    pip install -U xspf-lib
+
+Example
+-------
+1. Generating new playlist.
+
+>>> import xspf_lib as xspf
+>>> killer_queen = xspf.Track(location="file:///home/music/killer_queen.mp3",
+                              title="Killer Queen",
+                              creator="Queen",
+                              album="Sheer Heart Attack",
+                              trackNum=2,
+                              duration=177000,
+                              annotation="#2 in GB 1975",
+                              info="https://ru.wikipedia.org/wiki/Killer_Queen",
+                              image="file:///home/images/killer_queen_cover.png")
+>>> anbtd = xspf.Track()
+>>> anbtd.location = ["https://freemusic.example.com/loc.ogg",
+                      "file:///home/music/anbtd.mp3"]
+>>> anbtd.title = "Another One Bites the Dust"
+>>> anbtd.creator = "Queen"
+>>> anbtd.identifier = ["id1.group"]
+>>> anbtd.link = [xspf.Link("link.namespace", "link.uri.info")]
+>>> anbtd.meta = [xspf.Meta("meta.namespace", "METADATA_INFO")]
+>>> playlist = xspf.Playlist(title="Some Tracks",
+                             creator="myself",
+                             annotation="I did this only for examples!.",
+                             trackList=[killer_queen, anbtd])
+>>> print(playlist.xml_string())
+<playlist version="1" xmlns="http://xspf.org/ns/0/"><title>Some Tracks</title><creator>myself</creator><annotation>I did this only for examples!.</annotation><date>2020-02-03T14:29:59.199202+03:00</date><trackList><track><location>file:///home/music/killer_queen.mp3</location><title>Killer Queen</title><creator>Queen</creator><annotation>#2 in GB 1975</annotation><info>https://ru.wikipedia.org/wiki/Killer_Queen</info><image>file:///home/images/killer_queen_cover.png</image><album>Sheer Heart Attack</album><trackNum>2</trackNum><duration>177000</duration></track><track><location>https://freemusic.example.com/loc.ogg</location><location>file:///home/music/anbtd.mp3</location><identifier>id1.group</identifier><title>Another One Bites the Dust</title><creator>Queen</creator><link rel="link.namespace">link.uri.info</link><meta rel="meta.namespace">METADATA_INFO</meta></track></trackList></playlist>
+>>> playlist.write("some_tracks.xspf")
+
+2. Parsing from file.
+
+>>> from xspf_lib import Playlist
+>>> playlist = Playlist.parse("some_tracks.xspf")
+
+License
+-------
+
+The license of the project is MIT License - see LICENSE_ file for details.
+
+.. _LICENSE: https://github.com/dem214/xspf-lib/blob/master/LICENSE
+
+.. _pip: https://pip.pypa.io/en/stable/quickstart
```

#### html2text {}

```diff
@@ -1,19 +1,24 @@
-Metadata-Version: 2.1 Name: xspf-lib Version: 0.3.0 Summary: Library for work
-with xspf format Home-page: https://github.com/dem214/xspf-lib Author: Dzmitry
-Izaitka Author-email: dem214overlord@gmail.com License: UNKNOWN Description:
-======== xspf-lib ======== .. image:: https://github.com/dem214/xspf-lib/
-workflows/Python%20package/badge.svg?branch=master :alt: Python package ..
-image:: https://img.shields.io/badge/%20imports-isort-
-%231674b1?style=flat&labelColor=ef8336 :target: https://pycqa.github.io/isort/
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg :target:
-https://github.com/psf/black .. image:: https://img.shields.io/badge/pre--
-commit-enabled-brightgreen?logo=pre-commit :target: https://github.com/pre-
-commit/pre-commit :alt: pre-commit Library to work with xspf. Requirements ----
--------- * `Python 3.8 or higher
+Metadata-Version: 2.1 Name: xspf-lib Version: 0.3.1 Summary: Library for work
+with xspf format Keywords: xspf playlist Author-Email: Dzmitry Izaitka
+gmail.com> License: MIT Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Topic :: Multimedia :: Sound/Audio Classifier: Topic
+:: Multimedia :: Video Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Project-URL: Source, https://github.com/dem214/xspf-lib
+Project-URL: Bug tracker, https://github.com/dem214/xspf-lib/issues Requires-
+Python: >=3.7 Description-Content-Type: text/x-rst ======== xspf-lib ========
+.. image:: https://github.com/dem214/xspf-lib/workflows/Python%20package/
+badge.svg?branch=master :alt: Python package .. image:: https://img.shields.io/
+badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336 :target: https://
+pycqa.github.io/isort/ .. image:: https://img.shields.io/badge/code%20style-
+black-000000.svg :target: https://github.com/psf/black .. image:: https://
+img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit :target:
+https://github.com/pre-commit/pre-commit :alt: pre-commit Library to work with
+xspf. Requirements ------------ * `Python 3.8 or higher
 www.python.org/downloads/>`_ Installing ---------- Install and update via
 `pip`_: .. code-block:: text pip install -U xspf-lib Example ------- 1.
 Generating new playlist. >>> import xspf_lib as xspf >>> killer_queen =
 xspf.Track(location="file:///home/music/killer_queen.mp3", title="Killer
 Queen", creator="Queen", album="Sheer Heart Attack", trackNum=2,
 duration=177000, annotation="#2 in GB 1975", info="https://ru.wikipedia.org/
 wiki/Killer_Queen", image="file:///home/images/killer_queen_cover.png") >>>
@@ -31,13 +36,8 @@
 freemusic.example.com/loc.oggfile:///home/music/anbtd.mp3id1.group
 Queen
 link.uri.info
 METADATA_INFO >>> playlist.write("some_tracks.xspf") 2. Parsing from file. >>>
 from xspf_lib import Playlist >>> playlist = Playlist.parse("some_tracks.xspf")
 License ------- The license of the project is MIT License - see LICENSE_ file
 for details. .. _LICENSE: https://github.com/dem214/xspf-lib/blob/master/
-LICENSE .. _pip: https://pip.pypa.io/en/stable/quickstart Keywords: xspf
-playlist Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
-OS Independent Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Multimedia :: Sound/Audio Classifier: Topic ::
-Multimedia :: Video Requires-Python: >=3.7 Description-Content-Type: text/x-rst
+LICENSE .. _pip: https://pip.pypa.io/en/stable/quickstart
```

