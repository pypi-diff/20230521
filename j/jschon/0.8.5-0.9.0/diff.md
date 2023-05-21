# Comparing `tmp/jschon-0.8.5.tar.gz` & `tmp/jschon-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jschon-0.8.5.tar", last modified: Tue May 10 19:23:26 2022, max compression
+gzip compressed data, was "jschon-0.9.0.tar", last modified: Sun Aug 14 09:47:16 2022, max compression
```

## Comparing `jschon-0.8.5.tar` & `jschon-0.9.0.tar`

### file list

```diff
@@ -1,84 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.397019 jschon-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (121)     6687 2022-05-10 19:23:06.000000 jschon-0.8.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-05-10 19:23:06.000000 jschon-0.8.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-05-10 19:23:06.000000 jschon-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-05-10 19:23:06.000000 jschon-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4884 2022-05-10 19:23:26.397019 jschon-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3878 2022-05-10 19:23:06.000000 jschon-0.8.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-05-10 19:23:06.000000 jschon-0.8.5/TESTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.389019 jschon-0.8.5/jschon/
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.393020 jschon-0.8.5/jschon/catalog/
--rw-r--r--   0 runner    (1001) docker     (121)     3253 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/catalog/_2019_09.py
--rw-r--r--   0 runner    (1001) docker     (121)     3370 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/catalog/_2020_12.py
--rw-r--r--   0 runner    (1001) docker     (121)    11979 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/catalog/_translation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.393020 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-05-10 19:23:08.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/hyper-schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     3110 2022-05-10 19:23:08.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/links.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.393020 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-05-10 19:23:08.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/applicator.json
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-05-10 19:23:08.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/content.json
--rw-r--r--   0 runner    (1001) docker     (121)     1531 2022-05-10 19:23:08.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/core.json
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-05-10 19:23:08.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/format.json
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-05-10 19:23:08.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/hyper-schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-05-10 19:23:08.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/meta-data.json
--rw-r--r--   0 runner    (1001) docker     (121)     2834 2022-05-10 19:23:08.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/validation.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.393020 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/output/
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-05-10 19:23:08.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/output/hyper-schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     2172 2022-05-10 19:23:08.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/output/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     4413 2022-05-10 19:23:08.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/output/verbose-example.json
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-05-10 19:23:08.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.393020 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.393020 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/archive/
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/archive/hyper-schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     3298 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/archive/links.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.393020 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/archive/meta/
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/archive/meta/hyper-schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/hyper-schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/links.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.393020 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/applicator.json
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/content.json
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/core.json
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/format-annotation.json
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/format-assertion.json
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/hyper-schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/meta-data.json
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/unevaluated.json
--rw-r--r--   0 runner    (1001) docker     (121)     2834 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/validation.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.393020 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/output/
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/output/hyper-schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     2371 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/output/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     4377 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/output/verbose-example.json
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.393020 jschon-0.8.5/jschon/catalog/json-translation-vocabulary/
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-translation-vocabulary/schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     2346 2022-05-10 19:23:09.000000 jschon-0.8.5/jschon/catalog/json-translation-vocabulary/vocab.json
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8421 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/json.py
--rw-r--r--   0 runner    (1001) docker     (121)    10548 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/jsonpatch.py
--rw-r--r--   0 runner    (1001) docker     (121)    12114 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/jsonpointer.py
--rw-r--r--   0 runner    (1001) docker     (121)    17434 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (121)     3749 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/output.py
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     6151 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/translation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3731 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/uri.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.397019 jschon-0.8.5/jschon/vocabulary/
--rw-r--r--   0 runner    (1001) docker     (121)     5031 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/vocabulary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/vocabulary/annotation.py
--rw-r--r--   0 runner    (1001) docker     (121)    11969 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/vocabulary/applicator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6839 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/vocabulary/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/vocabulary/format.py
--rw-r--r--   0 runner    (1001) docker     (121)     4805 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/vocabulary/legacy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6512 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/vocabulary/translation.py
--rw-r--r--   0 runner    (1001) docker     (121)     7630 2022-05-10 19:23:06.000000 jschon-0.8.5/jschon/vocabulary/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-10 19:23:26.389019 jschon-0.8.5/jschon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4884 2022-05-10 19:23:25.000000 jschon-0.8.5/jschon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-05-10 19:23:26.000000 jschon-0.8.5/jschon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-10 19:23:25.000000 jschon-0.8.5/jschon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-05-10 19:23:26.000000 jschon-0.8.5/jschon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-10 19:23:26.000000 jschon-0.8.5/jschon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-10 19:23:26.397019 jschon-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-05-10 19:23:06.000000 jschon-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 09:47:16.176885 jschon-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     7689 2022-08-14 09:46:51.000000 jschon-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-08-14 09:46:51.000000 jschon-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-08-14 09:46:51.000000 jschon-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-14 09:46:51.000000 jschon-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4777 2022-08-14 09:47:16.176885 jschon-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3771 2022-08-14 09:46:51.000000 jschon-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-08-14 09:46:51.000000 jschon-0.9.0/TESTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 09:47:16.168884 jschon-0.9.0/jschon/
+-rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 09:47:16.172885 jschon-0.9.0/jschon/catalog/
+-rw-r--r--   0 runner    (1001) docker     (121)     3253 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/catalog/_2019_09.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3370 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/catalog/_2020_12.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11802 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 09:47:16.172885 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-08-14 09:46:56.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/hyper-schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3110 2022-08-14 09:46:56.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/links.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 09:47:16.172885 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-08-14 09:46:56.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/applicator.json
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-08-14 09:46:56.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/content.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1531 2022-08-14 09:46:56.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/core.json
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-08-14 09:46:56.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/format.json
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-08-14 09:46:56.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/hyper-schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-08-14 09:46:56.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/meta-data.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2834 2022-08-14 09:46:56.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/validation.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 09:47:16.172885 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/output/
+-rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-08-14 09:46:56.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/output/hyper-schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2172 2022-08-14 09:46:56.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/output/schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4413 2022-08-14 09:46:56.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/output/verbose-example.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-08-14 09:46:56.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 09:47:16.172885 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 09:47:16.172885 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/archive/
+-rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/archive/hyper-schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3298 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/archive/links.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 09:47:16.172885 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/archive/meta/
+-rw-r--r--   0 runner    (1001) docker     (121)      882 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/archive/meta/hyper-schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/hyper-schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/links.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 09:47:16.176885 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/
+-rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/applicator.json
+-rw-r--r--   0 runner    (1001) docker     (121)      519 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/content.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/core.json
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/format-annotation.json
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/format-assertion.json
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/hyper-schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/meta-data.json
+-rw-r--r--   0 runner    (1001) docker     (121)      506 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/unevaluated.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2834 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/validation.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 09:47:16.176885 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/output/
+-rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/output/hyper-schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2371 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/output/schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4377 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/output/verbose-example.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-08-14 09:46:58.000000 jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10236 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/json.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10548 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/jsonpatch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12114 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/jsonpointer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18355 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3735 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/output.py
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     3731 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/uri.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 09:47:16.176885 jschon-0.9.0/jschon/vocabulary/
+-rw-r--r--   0 runner    (1001) docker     (121)     5258 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/vocabulary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/vocabulary/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12955 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/vocabulary/applicator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6819 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/vocabulary/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/vocabulary/format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5237 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/vocabulary/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7908 2022-08-14 09:46:51.000000 jschon-0.9.0/jschon/vocabulary/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 09:47:16.172885 jschon-0.9.0/jschon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4777 2022-08-14 09:47:16.000000 jschon-0.9.0/jschon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2573 2022-08-14 09:47:16.000000 jschon-0.9.0/jschon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-14 09:47:16.000000 jschon-0.9.0/jschon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-08-14 09:47:16.000000 jschon-0.9.0/jschon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-14 09:47:16.000000 jschon-0.9.0/jschon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-14 09:47:16.176885 jschon-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-08-14 09:46:51.000000 jschon-0.9.0/setup.py
```

### Comparing `jschon-0.8.5/CHANGELOG.rst` & `jschon-0.9.0/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,39 @@
 Changelog
 =========
 
+v0.9.0 (2022-08-14)
+-------------------
+Features:
+
+* JSON array/object mutation
+* JSON serialization to string/file
+* JSON deserialization from remote location
+
+Breaking changes:
+
+* Rename Scope to Result
+* Remove JSON support for decimal.Decimal (#31)
+* Rename Keyword.types to Keyword.instance_types
+* Rename Keyword.depends to Keyword.depends_on
+* Move translation vocabulary implementation to its own repo (jschon-translation)
+
+Miscellaneous:
+
+* Allow any JSON-compatible value to be set as an error on a Result node
+* Array/object applicator keywords -- additionalProperties, unevaluatedProperties,
+  propertyNames, additionalItems, items, prefixItems, unevaluatedItems -- now
+  produce an error array of failing child indices
+* Register output formatters with a decorator
+* Remove JSON type checks for unsupported usage
+* Append (rather than replace) the suffix when resolving a LocalSource filepath
+* Flatten dict of subresults on Result node
+* Provide a useful __str__ method for Result node
+
+
 v0.8.5 (2022-05-10)
 -------------------
 Features:
 
 * Added JSONPointer prefix test operators (#29)
```

### Comparing `jschon-0.8.5/CONTRIBUTING.rst` & `jschon-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/LICENSE` & `jschon-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/PKG-INFO` & `jschon-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jschon
-Version: 0.8.5
+Version: 0.9.0
 Summary: A pythonic, extensible JSON Schema implementation.
 Home-page: https://github.com/marksparkza/jschon
 Author: Mark Jacobson
 Author-email: mark@saeon.ac.za
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -43,15 +43,14 @@
   * Support for custom keywords, vocabularies and meta-schemas
   * Support for format validation
 
 * JSON class implementing the JSON data model
 * JSON Pointer (`RFC 6901 <https://tools.ietf.org/html/rfc6901.html>`_)
 * JSON Patch (`RFC 6902 <https://tools.ietf.org/html/rfc6902.html>`_)
 * Relative JSON Pointer (`draft <https://json-schema.org/draft/2020-12/relative-json-pointer.html>`_)
-* JSON document translation (`experimental <https://github.com/marksparkza/json-translation-vocabulary>`_)
 
 Installation
 ------------
 ::
 
     pip install jschon
```

### Comparing `jschon-0.8.5/README.rst` & `jschon-0.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
   * Support for custom keywords, vocabularies and meta-schemas
   * Support for format validation
 
 * JSON class implementing the JSON data model
 * JSON Pointer (`RFC 6901 <https://tools.ietf.org/html/rfc6901.html>`_)
 * JSON Patch (`RFC 6902 <https://tools.ietf.org/html/rfc6902.html>`_)
 * Relative JSON Pointer (`draft <https://json-schema.org/draft/2020-12/relative-json-pointer.html>`_)
-* JSON document translation (`experimental <https://github.com/marksparkza/json-translation-vocabulary>`_)
 
 Installation
 ------------
 ::
 
     pip install jschon
```

### Comparing `jschon-0.8.5/TESTING.rst` & `jschon-0.9.0/TESTING.rst`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/__init__.py` & `jschon-0.9.0/jschon/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,33 +22,32 @@
     'LocalSource',
     'RemoteSource',
     'URI',
     'URIError',
     'create_catalog',
 ]
 
-__version__ = '0.8.5'
+__version__ = '0.9.0'
 
 
 def create_catalog(*vocabularies: str, name: str = 'catalog') -> Catalog:
     """Create and return a :class:`Catalog` instance, configured with
     support for the specified JSON Schema vocabularies.
 
-    :param vocabularies: any of ``2019-09``, ``2020-12``, ``translation``
+    :param vocabularies: any of ``2019-09``, ``2020-12``
     :param name: a unique name for the :class:`Catalog` instance
     :raise ValueError: if a supplied vocabulary parameter is not recognized
     """
-    from .catalog import _2019_09, _2020_12, _translation
+    from .catalog import _2019_09, _2020_12
 
     catalog = Catalog(name=name)
 
     vocabulary_initializers = {
         '2019-09': _2019_09.initialize,
         '2020-12': _2020_12.initialize,
-        'translation': _translation.initialize,
     }
     try:
         for vocabulary in vocabularies:
             vocabulary_init = vocabulary_initializers[vocabulary]
             vocabulary_init(catalog)
 
     except KeyError as e:
```

### Comparing `jschon-0.8.5/jschon/catalog/_2019_09.py` & `jschon-0.9.0/jschon/catalog/_2019_09.py`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/_2020_12.py` & `jschon-0.9.0/jschon/catalog/_2020_12.py`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/__init__.py` & `jschon-0.9.0/jschon/catalog/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from os import PathLike
 from typing import Any, ContextManager, Dict, Hashable, Mapping, Union
 
 from jschon.exceptions import CatalogError, JSONPointerError, URIError
 from jschon.json import JSONCompatible
 from jschon.jsonpointer import JSONPointer
 from jschon.jsonschema import JSONSchema
-from jschon.output import JSONSchemaOutputFormatter, OutputFormatter
 from jschon.uri import URI
 from jschon.utils import json_loadf, json_loadr
 from jschon.vocabulary import KeywordClass, Metaschema, Vocabulary
 from jschon.vocabulary.format import FormatValidator
 
 __all__ = [
     'Catalog',
@@ -36,15 +35,16 @@
     def __init__(self, base_dir: Union[str, PathLike], **kwargs: Any) -> None:
         super().__init__(**kwargs)
         self.base_dir = base_dir
 
     def __call__(self, relative_path: str) -> JSONCompatible:
         filepath = pathlib.Path(self.base_dir) / relative_path
         if self.suffix:
-            filepath = filepath.with_suffix(self.suffix)
+            filepath = str(filepath)
+            filepath += self.suffix
 
         return json_loadf(filepath)
 
 
 class RemoteSource(Source):
     def __init__(self, base_url: URI, **kwargs: Any) -> None:
         super().__init__(**kwargs)
@@ -79,17 +79,14 @@
         :param name: a unique name for this :class:`Catalog` instance
         """
         self.__class__._catalog_registry[name] = self
 
         self.name: str = name
         """The unique name of this :class:`Catalog` instance."""
 
-        self.output_formatter: OutputFormatter = JSONSchemaOutputFormatter()
-        """A JSON Schema output formatter."""
-
         self._uri_sources: Dict[URI, Source] = {}
         self._vocabularies: Dict[URI, Vocabulary] = {}
         self._format_validators: Dict[str, FormatValidator] = {}
         self._schema_cache: Dict[Hashable, Dict[URI, JSONSchema]] = {}
 
     def add_uri_source(self, base_uri: URI, source: Source):
         """Register a source for URI-identified JSON resources.
```

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/hyper-schema.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/links.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/links.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/applicator.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/applicator.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/content.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/content.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/core.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/core.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/hyper-schema.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/meta-data.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/meta-data.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/meta/validation.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/meta/validation.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/output/hyper-schema.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/output/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/output/schema.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/output/schema.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/output/verbose-example.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/output/verbose-example.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2019-09/schema.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2019-09/schema.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/archive/hyper-schema.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/archive/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/archive/links.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/archive/links.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/archive/meta/hyper-schema.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/archive/meta/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/hyper-schema.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/links.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/links.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/applicator.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/applicator.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/content.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/content.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/core.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/core.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/hyper-schema.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/meta-data.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/meta-data.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/meta/validation.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/meta/validation.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/output/hyper-schema.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/output/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/output/schema.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/output/schema.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/output/verbose-example.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/output/verbose-example.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/catalog/json-schema-spec-2020-12/schema.json` & `jschon-0.9.0/jschon/catalog/json-schema-spec-2020-12/schema.json`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/json.py` & `jschon-0.9.0/jschon/json.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 from __future__ import annotations
 
 import json
 from collections import deque
-from decimal import Decimal
 from functools import cached_property
 from os import PathLike
-from typing import Sequence, Mapping, Type, Optional, Iterator, Union, Any, List, Dict
+from typing import Any, Dict, Iterator, List, Mapping, MutableMapping, MutableSequence, Optional, Sequence, Type, Union
 
 from jschon.jsonpointer import JSONPointer
-from jschon.utils import json_loadf, json_loads
+from jschon.utils import json_dumpf, json_dumps, json_loadf, json_loadr, json_loads
 
 __all__ = [
     'JSON',
     'JSONCompatible',
 ]
 
-JSONCompatible = Union[None, bool, int, float, Decimal, str, Sequence[Any], Mapping[str, Any]]
+JSONCompatible = Union[None, bool, int, float, str, Sequence[Any], Mapping[str, Any]]
 """Type hint for a JSON-compatible Python object."""
 
 
-class JSON(Sequence['JSON'], Mapping[str, 'JSON']):
+class JSON(MutableSequence['JSON'], MutableMapping[str, 'JSON']):
     """An implementation of the JSON data model."""
 
     @classmethod
     def loadf(cls, path: Union[str, PathLike], **kwargs: Any) -> JSON:
         """Deserialize a JSON file to a :class:`JSON` instance.
 
         :param path: the path to the file
         :param kwargs: keyword arguments to pass to the :class:`JSON` (subclass) constructor
         """
         return cls(json_loadf(path), **kwargs)
 
     @classmethod
+    def loadr(cls, url: str, **kwargs: Any) -> JSON:
+        """Deserialize a remote JSON resource to a :class:`JSON` instance.
+
+        :param url: the URL of the resource
+        :param kwargs: keyword arguments to pass to the :class:`JSON` (subclass) constructor
+        """
+        return cls(json_loadr(url), **kwargs)
+
+    @classmethod
     def loads(cls, value: str, **kwargs: Any) -> JSON:
         """Deserialize a JSON string to a :class:`JSON` instance.
 
         :param value: the JSON string
         :param kwargs: keyword arguments to pass to the :class:`JSON` (subclass) constructor
         """
         return cls(json_loads(value), **kwargs)
@@ -63,70 +71,70 @@
             child nodes of arrays and objects (default: :class:`JSON`)
         :param itemkwargs: keyword arguments to pass to the `itemclass`
             constructor
         """
 
         self.type: str
         """The JSON type of the instance. One of
-        ``"null"``, ``"boolean"``, ``"number"``, ``"string"``, ``"array"``, ``"object"``."""
+        ``null``, ``boolean``, ``number``, ``string``, ``array``, ``object``."""
 
-        self.data: Union[None, bool, int, Decimal, str, List[JSON], Dict[str, JSON]]
+        self.data: Union[None, bool, int, float, str, List[JSON], Dict[str, JSON]]
         """The instance data.
         
         =========   ===============
         JSON type   data type
         =========   ===============
         null        None
         boolean     bool
-        number      int | Decimal
+        number      int | float
         string      str
         array       list[JSON]
         object      dict[str, JSON]
         =========   ===============
         """
 
         self.parent: Optional[JSON] = parent
         """The containing JSON instance."""
 
         self.key: Optional[str] = key
         """The index of the instance within its parent."""
 
+        self.itemclass: Type[JSON] = itemclass or JSON
+        """The :class:`JSON` class type of child instances."""
+
+        self.itemkwargs: Dict[str, Any] = itemkwargs
+        """Keyword arguments to the :attr:`itemclass` constructor."""
+
         if value is None:
             self.type = "null"
             self.data = None
 
         elif isinstance(value, bool):
             self.type = "boolean"
             self.data = value
 
-        elif isinstance(value, (int, Decimal)):
+        elif isinstance(value, (int, float)):
             self.type = "number"
             self.data = value
 
-        elif isinstance(value, float):
-            self.type = "number"
-            self.data = Decimal(f'{value}')
-
         elif isinstance(value, str):
             self.type = "string"
             self.data = value
 
         elif isinstance(value, Sequence):
-            itemclass = itemclass or JSON
             self.type = "array"
             self.data = [
-                itemclass(v, parent=self, key=str(i), **itemkwargs)
+                self.itemclass(v, parent=self, key=str(i), **self.itemkwargs)
                 for i, v in enumerate(value)
             ]
 
         elif isinstance(value, Mapping):
-            itemclass = itemclass or JSON
             self.type = "object"
             self.data = {
-                k: itemclass(v, parent=self, key=k, **itemkwargs)
+                k: self.itemclass(v, parent=self, key=k, **self.itemkwargs)
                 for k, v in value.items()
             }
 
         else:
             raise TypeError(f"{value=} is not JSON-compatible")
 
     @cached_property
@@ -144,51 +152,118 @@
         """Return the instance data as a JSON-compatible Python object."""
         if isinstance(self.data, list):
             return [item.value for item in self.data]
         if isinstance(self.data, dict):
             return {key: item.value for key, item in self.data.items()}
         return self.data
 
+    def _invalidate_path(self) -> None:
+        try:
+            del self.path
+        except AttributeError:
+            pass
+        if self.type == 'array':
+            for item in self.data:
+                item._invalidate_path()
+        elif self.type == 'object':
+            for item in self.data.values():
+                item._invalidate_path()
+
+    def _invalidate_value(self) -> None:
+        try:
+            del self.value
+        except AttributeError:
+            pass
+        if self.parent is not None:
+            self.parent._invalidate_value()
+
+    def dumpf(self, path: Union[str, PathLike]) -> None:
+        """Serialize the instance data to a JSON file.
+
+        :param path: the path to the file
+        """
+        json_dumpf(self.data, path)
+
+    def dumps(self) -> str:
+        """Serialize the instance data to a JSON string."""
+        return json_dumps(self.data)
+
     def __repr__(self) -> str:
         """Return `repr(self)`."""
-        return f'{self.__class__.__name__}({json.loads(str(self))!r})'
+        return f'{self.__class__.__name__}({json.loads(self.dumps())!r})'
 
     def __str__(self) -> str:
         """Return `str(self)`."""
-        def default(o):
-            if isinstance(o, JSON):
-                return o.data
-            if isinstance(o, Decimal):
-                return float(o)
-            raise TypeError
-
-        return json.dumps(self.data, default=default,
-                          ensure_ascii=False, allow_nan=False)
+        return self.dumps()
 
     def __bool__(self) -> bool:
         """Return `bool(self)`."""
         return bool(self.data)
 
     def __len__(self) -> int:
-        """Return `len(self)` for an instance of type ``"string"``, ``"array"``
-        or ``"object"``."""
+        """Return `len(self)`.
+
+        Supported for JSON types ``string``, ``array`` and ``object``.
+        """
         return len(self.data)
 
     def __iter__(self) -> Iterator:
-        """Return `iter(self)` for an instance of type ``"array"`` or ``"object"``."""
-        if self.type in ("array", "object"):
-            return iter(self.data)
-        raise TypeError(f"{self!r} is not iterable")
+        """Return `iter(self)`.
+
+        Supported for JSON types ``array`` and ``object``.
+        """
+        return iter(self.data)
 
     def __getitem__(self, index: Union[int, slice, str]) -> JSON:
-        """Return `self[index]` for an instance of type ``"array"`` or ``"object"``."""
-        if isinstance(index, (int, slice)) and self.type == "array" or \
-                isinstance(index, str) and self.type == "object":
-            return self.data[index]
-        raise TypeError(f"{self!r} is not subscriptable by {index!r}")
+        """Return `self[index]`.
+
+        Supported for JSON types ``array`` and ``object``.
+        """
+        return self.data[index]
+
+    def __setitem__(self, index: Union[int, str], obj: Union[JSON, JSONCompatible]) -> None:
+        """Set `self[index]` to `obj`.
+
+        Supported for JSON types ``array`` and ``object``.
+        """
+        self.data[index] = self.itemclass(
+            obj.value if isinstance(obj, JSON) else obj,
+            parent=self,
+            key=str(index),
+            **self.itemkwargs,
+        )
+        self._invalidate_value()
+
+    def __delitem__(self, index: Union[int, str]) -> None:
+        """Delete `self[index]`.
+
+        Supported for JSON types ``array`` and ``object``.
+        """
+        del self.data[index]
+        self._invalidate_value()
+        if self.type == 'array':
+            for item in self.data[index:]:
+                item.key = str(int(item.key) - 1)
+                item._invalidate_path()
+
+    def insert(self, index: int, obj: Union[JSON, JSONCompatible]) -> None:
+        """Insert `obj` before `index`.
+
+        Supported for JSON type ``array``.
+        """
+        self.data.insert(index, self.itemclass(
+            obj.value if isinstance(obj, JSON) else obj,
+            parent=self,
+            key=str(index),
+            **self.itemkwargs,
+        ))
+        self._invalidate_value()
+        for item in self.data[index + 1:]:
+            item.key = str(int(item.key) + 1)
+            item._invalidate_path()
 
     def __eq__(self, other: Union[JSON, JSONCompatible]) -> bool:
         """Return `self == other`."""
         if not isinstance(other, JSON):
             other = JSON(other)
         if self.type == other.type:
             if self.type == "array":
@@ -196,38 +271,42 @@
                        all(item == other[i] for i, item in enumerate(self))
             if self.type == "object":
                 return self.keys() == other.keys() and \
                        all(item == other[k] for k, item in self.items())
             return self.data == other.data
         return NotImplemented
 
-    def __ge__(self, other: Union[JSON, int, float, Decimal, str]) -> bool:
-        """Return `self >= other`, for instances of type ``"number"`` or ``"string"``."""
+    def __ge__(self, other: Union[JSON, int, float, str]) -> bool:
+        """Return `self >= other`.
+
+        Supported for JSON types ``number`` and ``string``.
+        """
         if isinstance(other, JSON):
             return self.data >= other.data
-        if isinstance(other, float):
-            return self.data >= Decimal(f'{other}')
         return self.data >= other
 
-    def __gt__(self, other: Union[JSON, int, float, Decimal, str]) -> bool:
-        """Return `self > other`, for instances of type ``"number"`` or ``"string"``."""
+    def __gt__(self, other: Union[JSON, int, float, str]) -> bool:
+        """Return `self > other`.
+
+        Supported for JSON types ``number`` and ``string``.
+        """
         if isinstance(other, JSON):
             return self.data > other.data
-        if isinstance(other, float):
-            return self.data > Decimal(f'{other}')
         return self.data > other
 
-    def __le__(self, other: Union[JSON, int, float, Decimal, str]) -> bool:
-        """Return `self <= other`, for instances of type ``"number"`` or ``"string"``."""
+    def __le__(self, other: Union[JSON, int, float, str]) -> bool:
+        """Return `self <= other`.
+
+        Supported for JSON types ``number`` and ``string``.
+        """
         if isinstance(other, JSON):
             return self.data <= other.data
-        if isinstance(other, float):
-            return self.data <= Decimal(f'{other}')
         return self.data <= other
 
-    def __lt__(self, other: Union[JSON, int, float, Decimal, str]) -> bool:
-        """Return `self < other`, for instances of type ``"number"`` or ``"string"``."""
+    def __lt__(self, other: Union[JSON, int, float, str]) -> bool:
+        """Return `self < other`.
+
+        Supported for JSON types ``number`` and ``string``.
+        """
         if isinstance(other, JSON):
             return self.data < other.data
-        if isinstance(other, float):
-            return self.data < Decimal(f'{other}')
         return self.data < other
```

### Comparing `jschon-0.8.5/jschon/jsonpatch.py` & `jschon-0.9.0/jschon/jsonpatch.py`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/jsonpointer.py` & `jschon-0.9.0/jschon/jsonpointer.py`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/jsonschema.py` & `jschon-0.9.0/jschon/jsonschema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from collections import deque
 from contextlib import contextmanager
 from functools import cached_property
-from typing import Any, ContextManager, Dict, Hashable, Iterator, Mapping, Optional, TYPE_CHECKING, Type, Union
+from typing import Any, ContextManager, Dict, Hashable, Iterator, Mapping, Optional, TYPE_CHECKING, Tuple, Type, Union
 from uuid import uuid4
 
 from jschon.exceptions import JSONSchemaError
 from jschon.json import JSON, JSONCompatible
 from jschon.jsonpointer import JSONPointer
 from jschon.uri import URI
 
 if TYPE_CHECKING:
     from jschon.catalog import Catalog
     from jschon.vocabulary import Keyword, KeywordClass, Metaschema
 
 __all__ = [
     'JSONSchema',
-    'Scope',
+    'Result',
 ]
 
 
 class JSONSchema(JSON):
     """JSON schema document model."""
 
     def __init__(
@@ -153,15 +153,15 @@
                 for item in kw.json.values():
                     if isinstance(item, JSONSchema):
                         item._resolve_references()
 
     @staticmethod
     def _resolve_dependencies(kwclasses: Dict[str, KeywordClass]) -> Iterator[KeywordClass]:
         dependencies = {
-            kwclass: [depclass for dep in kwclass.depends
+            kwclass: [depclass for dep in kwclass.depends_on
                       if (depclass := kwclasses.get(dep))]
             for kwclass in kwclasses.values()
         }
         while dependencies:
             for kwclass, depclasses in dependencies.items():
                 if not depclasses:
                     del dependencies[kwclass]
@@ -169,50 +169,48 @@
                         try:
                             deps.remove(kwclass)
                         except ValueError:
                             pass
                     yield kwclass
                     break
 
-    def validate(self) -> Scope:
+    def validate(self) -> Result:
         """Validate the schema against its metaschema."""
         return self.metaschema.evaluate(self)
 
-    def evaluate(self, instance: JSON, scope: Scope = None) -> Scope:
-        """Evaluate a JSON document.
-        
-        The returned :class:`Scope` represents the complete evaluation
-        result tree for this (sub)schema node.
+    def evaluate(self, instance: JSON, result: Result = None) -> Result:
+        """Evaluate a JSON document and return the evaluation result.
 
         :param instance: the JSON document to evaluate
-        :param scope: the dynamic evaluation scope; used by keywords
+        :param result: the current result node; given by keywords
             when invoking this method recursively
         """
-        if scope is None:
-            scope = Scope(self, instance)
+        if result is None:
+            result = Result(self, instance)
 
         if self.data is True:
             pass
 
         elif self.data is False:
-            scope.fail("The instance is disallowed by a boolean false schema")
+            result.fail("The instance is disallowed by a boolean false schema")
 
         else:
             for key, keyword in self.keywords.items():
                 if not keyword.static and keyword.can_evaluate(instance):
-                    with scope(instance, key, self) as subscope:
-                        keyword.evaluate(instance, subscope)
+                    with result(instance, key, self) as subresult:
+                        keyword.evaluate(instance, subresult)
 
             if any(
                     not child.passed
-                    for child in scope.iter_children(instance)
+                    for child in result.children.values()
+                    if child.instance.path == instance.path
             ):
-                scope.fail()
+                result.fail()
 
-        return scope
+        return result
 
     @cached_property
     def parentschema(self) -> Optional[JSONSchema]:
         """The containing :class:`JSONSchema` instance.
         
         Note that this is not necessarily the same as `self.parent`.
         """
@@ -306,30 +304,57 @@
                     relpath = JSONPointer.parse_uri_fragment(fragment) / keys
                 else:
                     relpath = JSONPointer(keys)
 
                 return node._uri.copy(fragment=relpath.uri_fragment())
 
 
-class Scope:
+class Result:
+    """The result of evaluating a JSON document
+    node against a JSON schema node.
+
+    The root of a :class:`Result` tree represents
+    a complete document evaluation result.
+    """
+
     def __init__(
             self,
             schema: JSONSchema,
             instance: JSON,
             *,
-            parent: Scope = None,
+            parent: Result = None,
             key: str = None,
-    ):
+    ) -> None:
+        self.path: JSONPointer
+        """The dynamic evaluation path to the current schema node."""
+
+        self.relpath: JSONPointer
+        """The path to the current schema node relative to the evaluating (sub)schema."""
+
         self.schema: JSONSchema = schema
+        """The evaluating (sub)schema."""
+
         self.instance: JSON = instance
-        self.parent: Optional[Scope] = parent
+        """The instance under evaluation."""
+
+        self.parent: Optional[Result] = parent
+        """The parent result node."""
+
         self.key: Optional[str] = key
-        self.children: Dict[JSONPointer, Dict[str, Scope]] = {}
+        """The index of the current schema node within its dynamic parent."""
+
+        self.children: Dict[Tuple[str, JSONPointer], Result] = {}
+        """Subresults of the current result node, indexed by schema key and instance path."""
+
         self.annotation: JSONCompatible = None
-        self.error: Optional[str] = None
+        """The annotation value of the result."""
+
+        self.error: JSONCompatible = None
+        """The error value of the result."""
+
         self._valid = True
         self._assert = True
         self._discard = False
         self._refschema: Optional[JSONSchema] = None
 
         if parent is None:
             self.path = JSONPointer()
@@ -343,152 +368,154 @@
     @contextmanager
     def __call__(
             self,
             instance: JSON,
             key: str,
             schema: JSONSchema = None,
             *,
-            cls: Type[Scope] = None,
-    ) -> ContextManager[Scope]:
-        """Yield a subscope of the current scope, for evaluating `instance`.
+            cls: Type[Result] = None,
+    ) -> ContextManager[Result]:
+        """Yield a subresult for the evaluation of `instance`.
         Descend down the evaluation path by `key`, into `schema` if given, or
-        within the schema of the current scope otherwise.
+        within `self.schema` otherwise.
 
-        Extension keywords may provide a custom Scope class via `cls`, which
-        is applied to all nodes within the yielded subtree.
+        Extension keywords may provide a custom :class:`Result` class via `cls`,
+        which is applied to all nodes within the yielded subtree.
         """
         if schema is None:
             schema = self.schema
 
-        self.children.setdefault(instance_path := instance.path, {})
-        self.children[instance_path][key] = (child := (cls or self.__class__)(
+        self.children[key, instance.path] = (child := (cls or self.__class__)(
             schema,
             instance,
             parent=self,
             key=key,
         ))
 
         try:
             yield child
         finally:
             if child._discard:
-                del self.children[instance_path][key]
+                del self.children[key, instance.path]
 
     @cached_property
     def globals(self) -> Dict:
         root = self
         while root.parent is not None:
             root = root.parent
         return root._globals
 
     @cached_property
     def schema_node(self) -> JSON:
-        """Return the schema node associated with this scope."""
+        """Return the current schema node."""
         return self.relpath.evaluate(self.schema)
 
-    def sibling(self, instance: JSON, key: str) -> Optional[Scope]:
+    def sibling(self, instance: JSON, key: str) -> Optional[Result]:
+        """Return a sibling schema node's evaluation result for `instance`."""
         try:
-            return self.parent.children[instance.path][key] if self.parent else None
+            return self.parent.children[key, instance.path] if self.parent else None
         except KeyError:
             return None
 
     def annotate(self, value: JSONCompatible) -> None:
-        """Set an annotation on the scope."""
+        """Annotate the result."""
         self.annotation = value
 
-    def fail(self, error: str = None) -> None:
-        """Flag the scope as invalid, optionally with an error message."""
+    def fail(self, error: JSONCompatible = None) -> None:
+        """Mark the result as invalid, optionally with an error."""
         self._valid = False
         self.error = error
 
     def pass_(self) -> None:
-        """Flag the scope as valid.
+        """Mark the result as valid.
         
-        A scope is initially valid, so this should ordinarily only need
-        to be called by a keyword when it must reverse a scope failure.
+        A result is initially valid, so this should only need
+        to be called by a keyword when it must reverse a failure.
         """
         self._valid = True
         self.error = None
 
     def noassert(self) -> None:
-        """Indicate that the scope's validity should not affect its
-        assertion result."""
+        """Indicate that evaluation passes regardless of validity."""
         self._assert = False
 
     def discard(self) -> None:
-        """Indicate that the scope should be ignored and discarded."""
+        """Indicate that the result should be ignored and discarded."""
         self._discard = True
 
     def refschema(self, schema: JSONSchema) -> None:
-        """Set the referenced schema for the scope of a by-reference keyword.
+        """Set the referenced schema for a by-reference keyword.
         
-        The referenced schema's URI is then returned by :attr:`absolute_uri`,
-        instead of calculating the absolute URI using the containing schema.
+        This ensures that :attr:`absolute_uri` returns the URI of the
+        referenced schema rather than the referencing keyword.
         """
         self._refschema = schema
 
     @property
     def valid(self) -> bool:
-        """Return the validation result of the scope.
-
-        :rtype: bool
-        """
+        """Return the validity of the instance against the schema."""
         return self._valid
 
     @property
     def passed(self) -> bool:
-        """Return the assertion result of the scope.
-        
-        In the current implementation, this can only ever differ from
-        :attr:`valid` for an "if" keyword subscope: its validation result
-        may be false (triggering "else") while its assertion result is always
-        true. For the root scope (representing the overall document evaluation
-        result), :attr:`valid` will always equal :attr:`passed`.
+        """Return the assertion result for the schema node.
+
+        In the standard JSON Schema vocabulary, this can only differ
+        from :attr:`valid` for the ``if`` keyword: validity may be false
+        (triggering ``else``) while its assertion result is always true.
 
-        :rtype: bool
+        For the root result node, :attr:`passed` will always equal :attr:`valid`.
         """
         return self._valid or not self._assert
 
     @property
     def absolute_uri(self) -> Optional[URI]:
+        """Return the absolute URI of the current schema node."""
         if self._refschema is not None:
             return self._refschema.canonical_uri
 
         if (schema_uri := self.schema.canonical_uri) is not None:
             if fragment := schema_uri.fragment:
                 relpath = JSONPointer.parse_uri_fragment(fragment) / self.relpath
             else:
                 relpath = self.relpath
             return schema_uri.copy(fragment=relpath.uri_fragment())
 
-    def iter_children(self, instance: JSON = None) -> Iterator[Scope]:
-        """Return an iterator over child scopes of this scope, optionally
-        filtered by an instance to which they apply."""
-        for instance_path, keyword_scopes in self.children.items():
-            if instance is None or instance.path == instance_path:
-                yield from keyword_scopes.values()
-
     def collect_annotations(self, instance: JSON = None, key: str = None) -> Iterator[JSONCompatible]:
         """Return an iterator over annotations produced in this subtree,
         optionally filtered by instance and/or keyword."""
         if self._valid and not self._discard:
             if self.annotation is not None and \
                     (key is None or key == self.key) and \
                     (instance is None or instance.path == self.instance.path):
                 yield self.annotation
-            for child in self.iter_children():
+            for child in self.children.values():
                 yield from child.collect_annotations(instance, key)
 
+    def collect_errors(self, instance: JSON = None, key: str = None) -> Iterator[JSONCompatible]:
+        """Return an iterator over errors produced in this subtree,
+        optionally filtered by instance and/or keyword."""
+        if not self._valid and not self._discard:
+            if self.error is not None and \
+                    (key is None or key == self.key) and \
+                    (instance is None or instance.path == self.instance.path):
+                yield self.error
+            for child in self.children.values():
+                yield from child.collect_errors(instance, key)
+
     def output(self, format: str, **kwargs: Any) -> JSONCompatible:
         """Return the evaluation result in the specified `format`.
 
-        :param format: The format of the returned document. The default
-            :class:`~jschon.output.JSONSchemaOutputFormatter` supports
-            the ``flag``, ``basic``, ``detailed`` and ``verbose`` output
-            formats, as defined by the JSON Schema specification.
-        :param kwargs: Additional keyword arguments to pass to the output
-            formatter.
+        :param format: One of the standard JSON Schema output formats --
+            ``flag``, ``basic``, ``detailed`` or ``verbose`` -- or any
+            format registered with the :func:`~jschon.output.output_formatter`
+            decorator.
+        :param kwargs: Keyword arguments to pass to the output formatter.
         """
-        return self.schema.catalog.output_formatter.create_output(self, format, **kwargs)
+        from jschon.output import create_output
+        return create_output(self, format, **kwargs)
 
     def __str__(self) -> str:
-        return str(self.path)
+        s = 'valid' if self.valid else 'invalid'
+        if self.parent:
+            s = f'{self.path}: {s}'
+        return s
```

### Comparing `jschon-0.8.5/jschon/output.py` & `jschon-0.9.0/jschon/output.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,125 @@
-from typing import Any, Dict
+from typing import Any, Callable, Dict
 
 from jschon.json import JSONCompatible
-from jschon.jsonschema import Scope
+from jschon.jsonschema import Result
 
 __all__ = [
     'OutputFormatter',
-    'JSONSchemaOutputFormatter',
+    'output_formatter',
+    'create_output',
 ]
 
+OutputFormatter = Callable[..., JSONCompatible]
+"""Call signature for a function decorated with :func:`output_formatter`.
 
-class OutputFormatter:
+The function must take a :class:`~jschon.jsonschema.Result` object
+as its first argument.
+"""
 
-    def create_output(self, scope: Scope, format: str, **kwargs: Any) -> JSONCompatible:
-        raise NotImplementedError
+_formatters: Dict[str, OutputFormatter] = {}
 
 
-class JSONSchemaOutputFormatter(OutputFormatter):
+def output_formatter(name: str = None):
+    """A decorator for a JSON Schema output formatting function.
 
-    def create_output(self, scope: Scope, format: str, **kwargs: Any) -> JSONCompatible:
-        if format == 'flag':
-            return self._flag(scope)
-        if format == 'basic':
-            return self._basic(scope)
-        if format == 'detailed':
-            return self._detailed(scope)
-        if format == 'verbose':
-            return self._verbose(scope)
-
-    @staticmethod
-    def _flag(scope: Scope) -> Dict[str, JSONCompatible]:
-        return {
-            "valid": scope.valid
-        }
+    :param name: The format name; defaults to the name of the decorated
+        function.
+    """
 
-    @staticmethod
-    def _basic(scope: Scope) -> Dict[str, JSONCompatible]:
-        def visit(node: Scope):
-            if node.valid is valid:
-                if (msgval := getattr(node, msgkey)) is not None:
-                    yield {
-                        "instanceLocation": str(node.instance.path),
-                        "keywordLocation": str(node.path),
-                        "absoluteKeywordLocation": str(node.absolute_uri),
-                        msgkey: msgval,
-                    }
-                for child in node.iter_children():
-                    yield from visit(child)
+    def decorator(f):
+        formatter_name = name if isinstance(name, str) else f.__name__
+        _formatters[formatter_name] = f
+        return f
 
-        valid = scope.valid
-        msgkey = "annotation" if valid else "error"
-        childkey = "annotations" if valid else "errors"
+    return decorator(name) if callable(name) else decorator
 
-        return {
-            "valid": valid,
-            childkey: [result for result in visit(scope)],
-        }
 
-    @staticmethod
-    def _detailed(scope: Scope) -> Dict[str, JSONCompatible]:
-        def visit(node: Scope):
-            result = {
-                "instanceLocation": str(node.instance.path),
-                "keywordLocation": str(node.path),
-                "absoluteKeywordLocation": str(node.absolute_uri),
-                childkey: [visit(child) for child in node.iter_children()
-                           if child.valid is valid],
-            }
-            if not result[childkey]:
-                del result[childkey]
-                if (msgval := getattr(node, msgkey)) is not None:
-                    result[msgkey] = msgval
-            elif len(result[childkey]) == 1:
-                result = result[childkey][0]
+def create_output(result: Result, format: str, **kwargs: Any) -> JSONCompatible:
+    return _formatters[format](result, **kwargs)
 
-            return result
 
-        valid = scope.valid
-        msgkey = "annotation" if valid else "error"
-        childkey = "annotations" if valid else "errors"
+@output_formatter
+def flag(result: Result) -> JSONCompatible:
+    return {
+        "valid": result.valid
+    }
+
 
-        return {
-            "valid": valid,
-            "instanceLocation": str(scope.instance.path),
-            "keywordLocation": str(scope.path),
-            "absoluteKeywordLocation": str(scope.absolute_uri),
-            childkey: [visit(child) for child in scope.iter_children()
+@output_formatter
+def basic(result: Result) -> JSONCompatible:
+    def visit(node: Result):
+        if node.valid is valid:
+            if (msgval := getattr(node, msgkey)) is not None:
+                yield {
+                    "instanceLocation": str(node.instance.path),
+                    "keywordLocation": str(node.path),
+                    "absoluteKeywordLocation": str(node.absolute_uri),
+                    msgkey: msgval,
+                }
+            for child in node.children.values():
+                yield from visit(child)
+
+    valid = result.valid
+    msgkey = "annotation" if valid else "error"
+    childkey = "annotations" if valid else "errors"
+
+    return {
+        "valid": valid,
+        childkey: [output for output in visit(result)],
+    }
+
+
+@output_formatter
+def detailed(result: Result) -> JSONCompatible:
+    def visit(node: Result):
+        output = {
+            "instanceLocation": str(node.instance.path),
+            "keywordLocation": str(node.path),
+            "absoluteKeywordLocation": str(node.absolute_uri),
+            childkey: [visit(child) for child in node.children.values()
                        if child.valid is valid],
         }
-
-    @staticmethod
-    def _verbose(scope: Scope) -> Dict[str, JSONCompatible]:
-        def visit(node: Scope):
-            result = {
-                "valid": (valid := node.valid),
-                "instanceLocation": str(node.instance.path),
-                "keywordLocation": str(node.path),
-                "absoluteKeywordLocation": str(node.absolute_uri),
-            }
-
-            msgkey = "annotation" if valid else "error"
+        if not output[childkey]:
+            del output[childkey]
             if (msgval := getattr(node, msgkey)) is not None:
-                result[msgkey] = msgval
+                output[msgkey] = msgval
+        elif len(output[childkey]) == 1:
+            output = output[childkey][0]
+
+        return output
+
+    valid = result.valid
+    msgkey = "annotation" if valid else "error"
+    childkey = "annotations" if valid else "errors"
+
+    return {
+        "valid": valid,
+        "instanceLocation": str(result.instance.path),
+        "keywordLocation": str(result.path),
+        "absoluteKeywordLocation": str(result.absolute_uri),
+        childkey: [visit(child) for child in result.children.values()
+                   if child.valid is valid],
+    }
+
+
+@output_formatter
+def verbose(result: Result) -> JSONCompatible:
+    def visit(node: Result):
+        output = {
+            "valid": (valid := node.valid),
+            "instanceLocation": str(node.instance.path),
+            "keywordLocation": str(node.path),
+            "absoluteKeywordLocation": str(node.absolute_uri),
+        }
 
-            childkey = "annotations" if valid else "errors"
-            if childarr := [visit(child) for child in node.iter_children()]:
-                result[childkey] = childarr
+        msgkey = "annotation" if valid else "error"
+        if (msgval := getattr(node, msgkey)) is not None:
+            output[msgkey] = msgval
+
+        childkey = "annotations" if valid else "errors"
+        if childarr := [visit(child) for child in node.children.values()]:
+            output[childkey] = childarr
 
-            return result
+        return output
 
-        return visit(scope)
+    return visit(result)
```

### Comparing `jschon-0.8.5/jschon/uri.py` & `jschon-0.9.0/jschon/uri.py`

 * *Files identical despite different names*

### Comparing `jschon-0.8.5/jschon/utils.py` & `jschon-0.9.0/jschon/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
-from decimal import Decimal
 from os import PathLike
 from typing import Any, Tuple, Iterable, Union
 
 __all__ = [
     'tuplify',
+    'json_dumpf',
+    'json_dumps',
     'json_loadf',
     'json_loadr',
     'json_loads',
 ]
 
 requests = None
 
@@ -27,32 +28,50 @@
     if isinstance(value, Tuple):
         return value
     if isinstance(value, Iterable) and not isinstance(value, str):
         return tuple(value)
     return value,
 
 
+def json_dumpf(obj: Any, path: Union[str, PathLike]) -> None:
+    """Serialize a JSON-compatible Python object to a JSON file."""
+    with open(path, 'w') as f:
+        json.dump(obj, f, ensure_ascii=False, allow_nan=False, default=_serialize_custom_obj)
+
+
+def json_dumps(obj: Any) -> str:
+    """Serialize a JSON-compatible Python object to a JSON string."""
+    return json.dumps(obj, ensure_ascii=False, allow_nan=False, default=_serialize_custom_obj)
+
+
 def json_loadf(path: Union[str, PathLike]) -> Any:
-    """Open and deserialize a JSON file, returning a JSON-compatible Python object."""
+    """Deserialize a JSON file, returning a JSON-compatible Python object."""
     with open(path) as f:
-        return json.load(f, parse_float=Decimal, parse_constant=_parse_invalid_const)
+        return json.load(f, parse_constant=_parse_invalid_const)
 
 
 def json_loadr(url: str) -> Any:
     """Fetch and deserialize a remote JSON resource, returning a JSON-compatible Python object."""
     if requests is None:
         _import_requests()
     r = requests.get(url)
     r.raise_for_status()
-    return r.json(parse_float=Decimal, parse_constant=_parse_invalid_const)
+    return r.json(parse_constant=_parse_invalid_const)
 
 
 def json_loads(value: str) -> Any:
     """Deserialize a JSON string, returning a JSON-compatible Python object."""
-    return json.loads(value, parse_float=Decimal, parse_constant=_parse_invalid_const)
+    return json.loads(value, parse_constant=_parse_invalid_const)
 
 
 def _parse_invalid_const(c):
     """Called when '-Infinity', 'Infinity' or 'NaN' is encountered in the
     JSON-encoded input. These JavaScript constants are not strictly allowed
     by the JSON data model."""
     raise ValueError(f"{c} is not a valid JSON value")
+
+
+def _serialize_custom_obj(o):
+    from jschon.json import JSON
+    if isinstance(o, JSON):
+        return o.data
+    raise TypeError
```

### Comparing `jschon-0.8.5/jschon/vocabulary/__init__.py` & `jschon-0.9.0/jschon/vocabulary/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import inspect
 from typing import Any, Dict, Mapping, Optional, Sequence, TYPE_CHECKING, Tuple, Type
 
 from jschon.json import JSON, JSONCompatible
-from jschon.jsonschema import JSONSchema, Scope
+from jschon.jsonschema import JSONSchema, Result
 from jschon.uri import URI
 
 if TYPE_CHECKING:
     from jschon.catalog import Catalog
 
 __all__ = [
     'Metaschema',
@@ -62,39 +62,44 @@
         self.kwclasses: Dict[str, KeywordClass] = {
             kwclass.key: kwclass for kwclass in kwclasses
         }
 
 
 class Keyword:
     key: str = ...
-    types: Tuple[str, ...] = ()
-    depends: Tuple[str, ...] = ()
+
+    instance_types: Tuple[str, ...] = "null", "boolean", "integer", "number", "string", "array", "object",
+    """The types of instance that the keyword can evaluate."""
+
+    depends_on: Tuple[str, ...] = ()
+    """Keywords that must be evaluated before this keyword can be evaluated."""
+
     static: bool = False
 
     def __init__(self, parentschema: JSONSchema, value: JSONCompatible):
         for base_cls in inspect.getmro(self.__class__):
             if issubclass(base_cls, ApplicatorMixin):
                 if (kwjson := base_cls.jsonify(parentschema, self.key, value)) is not None:
                     break
         else:
             kwjson = JSON(value, parent=parentschema, key=self.key)
 
         self.json: JSON = kwjson
         self.parentschema: JSONSchema = parentschema
 
     def can_evaluate(self, instance: JSON) -> bool:
-        if not self.types or instance.type in self.types:
+        if instance.type in self.instance_types:
             return True
 
-        if instance.type == "number" and "integer" in self.types:
+        if instance.type == "number" and "integer" in self.instance_types:
             return instance.data == int(instance.data)
 
         return False
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         pass
 
     def __str__(self) -> str:
         return f'{self.json.path}: {self.json}'
 
 
 KeywordClass = Type[Keyword]
```

### Comparing `jschon-0.8.5/jschon/vocabulary/annotation.py` & `jschon-0.9.0/jschon/vocabulary/annotation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from jschon.json import JSON
-from jschon.jsonschema import Scope
+from jschon.jsonschema import Result
 from jschon.vocabulary import Keyword
 
 __all__ = [
     'TitleKeyword',
     'DescriptionKeyword',
     'DefaultKeyword',
     'DeprecatedKeyword',
@@ -14,17 +14,17 @@
     'ContentEncodingKeyword',
     'ContentSchemaKeyword',
 ]
 
 
 class AnnotationKeyword(Keyword):
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        scope.annotate(self.json.data)
-        scope.noassert()
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        result.annotate(self.json.data)
+        result.noassert()
 
 
 class TitleKeyword(AnnotationKeyword):
     key = "title"
 
 
 class DescriptionKeyword(AnnotationKeyword):
@@ -49,25 +49,25 @@
 
 class ExamplesKeyword(AnnotationKeyword):
     key = "examples"
 
 
 class ContentMediaTypeKeyword(AnnotationKeyword):
     key = "contentMediaType"
-    types = "string",
+    instance_types = "string",
 
 
 class ContentEncodingKeyword(AnnotationKeyword):
     key = "contentEncoding"
-    types = "string",
+    instance_types = "string",
 
 
 class ContentSchemaKeyword(AnnotationKeyword):
     key = "contentSchema"
-    types = "string",
-    depends = "contentMediaType",
+    instance_types = "string",
+    depends_on = "contentMediaType",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        if scope.sibling(instance, "contentMediaType"):
-            super().evaluate(instance, scope)
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        if result.sibling(instance, "contentMediaType"):
+            super().evaluate(instance, result)
         else:
-            scope.discard()
+            result.discard()
```

### Comparing `jschon-0.8.5/jschon/vocabulary/applicator.py` & `jschon-0.9.0/jschon/vocabulary/applicator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 
 from jschon.json import JSON
-from jschon.jsonschema import Scope
-from jschon.vocabulary import Keyword, Applicator, ArrayApplicator, PropertyApplicator
+from jschon.jsonschema import Result
+from jschon.vocabulary import Applicator, ArrayApplicator, Keyword, PropertyApplicator
 
 __all__ = [
     'AllOfKeyword',
     'AnyOfKeyword',
     'OneOfKeyword',
     'NotKeyword',
     'IfKeyword',
@@ -24,329 +24,357 @@
     'PropertyNamesKeyword',
 ]
 
 
 class AllOfKeyword(Keyword, ArrayApplicator):
     key = "allOf"
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         err_indices = []
         for index, subschema in enumerate(self.json):
-            with scope(instance, str(index)) as subscope:
-                subschema.evaluate(instance, subscope)
-                if not subscope.passed:
+            with result(instance, str(index)) as subresult:
+                subschema.evaluate(instance, subresult)
+                if not subresult.passed:
                     err_indices += [index]
 
         if err_indices:
-            scope.fail(f'The instance is invalid against subschemas {err_indices}')
+            result.fail(f'The instance is invalid against subschemas {err_indices}')
 
 
 class AnyOfKeyword(Keyword, ArrayApplicator):
     key = "anyOf"
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         valid = False
         for index, subschema in enumerate(self.json):
-            with scope(instance, str(index)) as subscope:
-                subschema.evaluate(instance, subscope)
-                if subscope.passed:
+            with result(instance, str(index)) as subresult:
+                subschema.evaluate(instance, subresult)
+                if subresult.passed:
                     valid = True
 
         if not valid:
-            scope.fail(f'The instance must be valid against at least one subschema')
+            result.fail(f'The instance must be valid against at least one subschema')
 
 
 class OneOfKeyword(Keyword, ArrayApplicator):
     key = "oneOf"
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         valid_indices = []
         err_indices = []
         for index, subschema in enumerate(self.json):
-            with scope(instance, str(index)) as subscope:
-                subschema.evaluate(instance, subscope)
-                if subscope.passed:
+            with result(instance, str(index)) as subresult:
+                subschema.evaluate(instance, subresult)
+                if subresult.passed:
                     valid_indices += [index]
                 else:
                     err_indices += [index]
 
         if len(valid_indices) != 1:
-            scope.fail('The instance must be valid against exactly one subschema; '
-                       f'it is valid against {valid_indices} and invalid against {err_indices}')
+            result.fail('The instance must be valid against exactly one subschema; '
+                        f'it is valid against {valid_indices} and invalid against {err_indices}')
 
 
 class NotKeyword(Keyword, Applicator):
     key = "not"
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        self.json.evaluate(instance, scope)
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        self.json.evaluate(instance, result)
 
-        if scope.passed:
-            scope.fail('The instance must not be valid against the subschema')
+        if result.passed:
+            result.fail('The instance must not be valid against the subschema')
         else:
-            scope.pass_()
+            result.pass_()
 
 
 class IfKeyword(Keyword, Applicator):
     key = "if"
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        self.json.evaluate(instance, scope)
-        scope.noassert()
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        self.json.evaluate(instance, result)
+        result.noassert()
 
 
 class ThenKeyword(Keyword, Applicator):
     key = "then"
-    depends = "if",
+    depends_on = "if",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        if (if_ := scope.sibling(instance, "if")) and if_.valid:
-            self.json.evaluate(instance, scope)
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        if (if_ := result.sibling(instance, "if")) and if_.valid:
+            self.json.evaluate(instance, result)
         else:
-            scope.discard()
+            result.discard()
 
 
 class ElseKeyword(Keyword, Applicator):
     key = "else"
-    depends = "if",
+    depends_on = "if",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        if (if_ := scope.sibling(instance, "if")) and not if_.valid:
-            self.json.evaluate(instance, scope)
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        if (if_ := result.sibling(instance, "if")) and not if_.valid:
+            self.json.evaluate(instance, result)
         else:
-            scope.discard()
+            result.discard()
 
 
 class DependentSchemasKeyword(Keyword, PropertyApplicator):
     key = "dependentSchemas"
-    types = "object",
+    instance_types = "object",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         annotation = []
         err_names = []
         for name, subschema in self.json.items():
             if name in instance:
-                with scope(instance, name) as subscope:
-                    subschema.evaluate(instance, subscope)
-                    if subscope.passed:
+                with result(instance, name) as subresult:
+                    subschema.evaluate(instance, subresult)
+                    if subresult.passed:
                         annotation += [name]
                     else:
                         err_names += [name]
 
         if err_names:
-            scope.fail(f'Properties {err_names} are invalid against '
-                       f'the corresponding "dependentSchemas" subschemas')
+            result.fail(f'Properties {err_names} are invalid against '
+                        f'the corresponding "dependentSchemas" subschemas')
         else:
-            scope.annotate(annotation)
+            result.annotate(annotation)
 
 
 class PrefixItemsKeyword(Keyword, ArrayApplicator):
     key = "prefixItems"
-    types = "array",
+    instance_types = "array",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        eval_index = None
-        err_indices = []
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        annotation = None
+        error = []
         for index, item in enumerate(instance[:len(self.json)]):
-            eval_index = index
-            with scope(item, str(index)) as subscope:
-                self.json[index].evaluate(item, subscope)
-                if not subscope.passed:
-                    err_indices += [index]
-
-        if err_indices:
-            scope.fail(f"Array elements {err_indices} are invalid")
-        elif eval_index is not None:
-            if eval_index == len(instance) - 1:
-                eval_index = True
-            scope.annotate(eval_index)
+            annotation = index
+            with result(item, str(index)) as subresult:
+                if not self.json[index].evaluate(item, subresult).passed:
+                    error += [index]
+
+        if error:
+            result.fail(error)
+        elif annotation is not None:
+            if annotation == len(instance) - 1:
+                annotation = True
+            result.annotate(annotation)
 
 
 class ItemsKeyword(Keyword, Applicator):
     key = "items"
-    types = "array",
-    depends = "prefixItems",
+    instance_types = "array",
+    depends_on = "prefixItems",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        if prefix_items := scope.sibling(instance, "prefixItems"):
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        if prefix_items := result.sibling(instance, "prefixItems"):
             start_index = len(prefix_items.schema_node)
         else:
             start_index = 0
 
         annotation = None
-        for index, item in enumerate(instance[start_index:]):
-            annotation = True
-            self.json.evaluate(item, scope)
+        error = []
+        for index, item in enumerate(instance[start_index:], start_index):
+            if self.json.evaluate(item, result).passed:
+                annotation = True
+            else:
+                error += [index]
+                # reset to passed for the next iteration
+                result.pass_()
 
-        if annotation is True and scope.passed:
-            scope.annotate(annotation)
+        if error:
+            result.fail(error)
+        else:
+            result.annotate(annotation)
 
 
 class UnevaluatedItemsKeyword(Keyword, Applicator):
     key = "unevaluatedItems"
-    types = "array",
-    depends = "prefixItems", "items", "contains", "if", "then", "else", "allOf", "anyOf", "oneOf", "not",
+    instance_types = "array",
+    depends_on = "prefixItems", "items", "contains", "if", "then", "else", "allOf", "anyOf", "oneOf", "not",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         last_evaluated_item = -1
-        for prefix_items_annotation in scope.parent.collect_annotations(instance, "prefixItems"):
+        for prefix_items_annotation in result.parent.collect_annotations(instance, "prefixItems"):
             if prefix_items_annotation is True:
-                scope.discard()
+                result.discard()
                 return
             if prefix_items_annotation > last_evaluated_item:
                 last_evaluated_item = prefix_items_annotation
 
-        for items_annotation in scope.parent.collect_annotations(instance, "items"):
+        for items_annotation in result.parent.collect_annotations(instance, "items"):
             if items_annotation is True:
-                scope.discard()
+                result.discard()
                 return
 
-        for unevaluated_items_annotation in scope.parent.collect_annotations(instance, "unevaluatedItems"):
+        for unevaluated_items_annotation in result.parent.collect_annotations(instance, "unevaluatedItems"):
             if unevaluated_items_annotation is True:
-                scope.discard()
+                result.discard()
                 return
 
         contains_indices = set()
-        for contains_annotation in scope.parent.collect_annotations(instance, "contains"):
+        for contains_annotation in result.parent.collect_annotations(instance, "contains"):
             contains_indices |= set(contains_annotation)
 
         annotation = None
+        error = []
         for index, item in enumerate(instance[(start := last_evaluated_item + 1):], start):
             if index not in contains_indices:
-                annotation = True
-                self.json.evaluate(item, scope)
+                if self.json.evaluate(item, result).passed:
+                    annotation = True
+                else:
+                    error += [index]
+                    # reset to passed for the next iteration
+                    result.pass_()
 
-        if scope.passed:
-            scope.annotate(annotation)
+        if error:
+            result.fail(error)
+        else:
+            result.annotate(annotation)
 
 
 class ContainsKeyword(Keyword, Applicator):
     key = "contains"
-    types = "array",
+    instance_types = "array",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         annotation = []
         for index, item in enumerate(instance):
-            if self.json.evaluate(item, scope).passed:
+            if self.json.evaluate(item, result).passed:
                 annotation += [index]
             else:
-                scope.pass_()
+                result.pass_()
 
-        scope.annotate(annotation)
+        result.annotate(annotation)
         if not annotation:
-            scope.fail('The array does not contain any element that is valid '
-                       f'against the "{self.key}" subschema')
+            result.fail('The array does not contain any element that is valid '
+                        f'against the "{self.key}" subschema')
 
 
 class PropertiesKeyword(Keyword, PropertyApplicator):
     key = "properties"
-    types = "object",
+    instance_types = "object",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         annotation = []
         err_names = []
         for name, item in instance.items():
             if name in self.json:
-                with scope(item, name) as subscope:
-                    self.json[name].evaluate(item, subscope)
-                    if subscope.passed:
+                with result(item, name) as subresult:
+                    self.json[name].evaluate(item, subresult)
+                    if subresult.passed:
                         annotation += [name]
                     else:
                         err_names += [name]
 
         if err_names:
-            scope.fail(f"Properties {err_names} are invalid")
+            result.fail(f"Properties {err_names} are invalid")
         else:
-            scope.annotate(annotation)
+            result.annotate(annotation)
 
 
 class PatternPropertiesKeyword(Keyword, PropertyApplicator):
     key = "patternProperties"
-    types = "object",
+    instance_types = "object",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         matched_names = set()
         err_names = []
         for name, item in instance.items():
             for regex, subschema in self.json.items():
                 if re.search(regex, name) is not None:
-                    with scope(item, regex) as subscope:
-                        subschema.evaluate(item, subscope)
-                        if subscope.passed:
+                    with result(item, regex) as subresult:
+                        subschema.evaluate(item, subresult)
+                        if subresult.passed:
                             matched_names |= {name}
                         else:
                             err_names += [name]
 
         if err_names:
-            scope.fail(f"Properties {err_names} are invalid")
+            result.fail(f"Properties {err_names} are invalid")
         else:
-            scope.annotate(list(matched_names))
+            result.annotate(list(matched_names))
 
 
 class AdditionalPropertiesKeyword(Keyword, Applicator):
     key = "additionalProperties"
-    types = "object",
-    depends = "properties", "patternProperties",
+    instance_types = "object",
+    depends_on = "properties", "patternProperties",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        if properties := scope.sibling(instance, "properties"):
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        if properties := result.sibling(instance, "properties"):
             known_property_names = properties.schema_node.keys()
         else:
             known_property_names = ()
 
-        if pattern_properties := scope.sibling(instance, "patternProperties"):
+        if pattern_properties := result.sibling(instance, "patternProperties"):
             known_property_patterns = pattern_properties.schema_node.keys()
         else:
             known_property_patterns = ()
 
         annotation = []
+        error = []
         for name, item in instance.items():
             if name not in known_property_names and not any(
-                re.search(regex, name) for regex in known_property_patterns
+                    re.search(regex, name) for regex in known_property_patterns
             ):
-                if self.json.evaluate(item, scope).passed:
+                if self.json.evaluate(item, result).passed:
                     annotation += [name]
+                else:
+                    error += [name]
+                    # reset to passed for the next iteration
+                    result.pass_()
 
-        if scope.passed:
-            scope.annotate(annotation)
+        if error:
+            result.fail(error)
+        else:
+            result.annotate(annotation)
 
 
 class UnevaluatedPropertiesKeyword(Keyword, Applicator):
     key = "unevaluatedProperties"
-    types = "object",
-    depends = "properties", "patternProperties", "additionalProperties", \
-              "if", "then", "else", "dependentSchemas", \
-              "allOf", "anyOf", "oneOf", "not",
+    instance_types = "object",
+    depends_on = "properties", "patternProperties", "additionalProperties", \
+                 "if", "then", "else", "dependentSchemas", \
+                 "allOf", "anyOf", "oneOf", "not",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         evaluated_names = set()
-        for properties_annotation in scope.parent.collect_annotations(instance, "properties"):
+        for properties_annotation in result.parent.collect_annotations(instance, "properties"):
             evaluated_names |= set(properties_annotation)
-        for pattern_properties_annotation in scope.parent.collect_annotations(instance, "patternProperties"):
+        for pattern_properties_annotation in result.parent.collect_annotations(instance, "patternProperties"):
             evaluated_names |= set(pattern_properties_annotation)
-        for additional_properties_annotation in scope.parent.collect_annotations(instance, "additionalProperties"):
+        for additional_properties_annotation in result.parent.collect_annotations(instance, "additionalProperties"):
             evaluated_names |= set(additional_properties_annotation)
-        for unevaluated_properties_annotation in scope.parent.collect_annotations(instance, "unevaluatedProperties"):
+        for unevaluated_properties_annotation in result.parent.collect_annotations(instance, "unevaluatedProperties"):
             evaluated_names |= set(unevaluated_properties_annotation)
 
         annotation = []
+        error = []
         for name, item in instance.items():
             if name not in evaluated_names:
-                if self.json.evaluate(item, scope).passed:
+                if self.json.evaluate(item, result).passed:
                     annotation += [name]
+                else:
+                    error += [name]
+                    # reset to passed for the next iteration
+                    result.pass_()
 
-        if scope.passed:
-            scope.annotate(annotation)
+        if error:
+            result.fail(error)
+        else:
+            result.annotate(annotation)
 
 
 class PropertyNamesKeyword(Keyword, Applicator):
     key = "propertyNames"
-    types = "object",
+    instance_types = "object",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        err_names = []
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        error = []
         for name in instance:
-            if not self.json.evaluate(JSON(name, parent=instance, key=name), scope).passed:
-                err_names += [name]
+            if not self.json.evaluate(JSON(name, parent=instance, key=name), result).passed:
+                error += [name]
+                result.pass_()
 
-        if err_names:
-            scope.fail(f"Property names {err_names} are invalid")
+        if error:
+            result.fail(error)
```

### Comparing `jschon-0.8.5/jschon/vocabulary/core.py` & `jschon-0.9.0/jschon/vocabulary/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Mapping
 
-from jschon.exceptions import JSONSchemaError, URIError, CatalogError
+from jschon.exceptions import CatalogError, JSONSchemaError, URIError
 from jschon.json import JSON
-from jschon.jsonschema import JSONSchema, Scope
+from jschon.jsonschema import JSONSchema, Result
 from jschon.uri import URI
-from jschon.vocabulary import Keyword, PropertyApplicator, Metaschema
+from jschon.vocabulary import Keyword, Metaschema, PropertyApplicator
 
 __all__ = [
     'SchemaKeyword',
     'VocabularyKeyword',
     'IdKeyword',
     'RefKeyword',
     'AnchorKeyword',
@@ -94,17 +94,17 @@
             else:
                 raise JSONSchemaError(f'No base URI against which to resolve the "$ref" value "{uri}"')
 
         self.refschema = self.parentschema.catalog.get_schema(
             uri, metaschema_uri=self.parentschema.metaschema_uri, session=self.parentschema.session
         )
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        self.refschema.evaluate(instance, scope)
-        scope.refschema(self.refschema)
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        self.refschema.evaluate(instance, result)
+        result.refschema(self.refschema)
 
 
 class AnchorKeyword(Keyword):
     key = "$anchor"
     static = True
 
     def __init__(self, parentschema: JSONSchema, value: str):
@@ -143,39 +143,39 @@
 
         self.refschema = self.parentschema.catalog.get_schema(
             uri, metaschema_uri=self.parentschema.metaschema_uri, session=self.parentschema.session
         )
         if (dynamic_anchor := self.refschema.get("$dynamicAnchor")) and dynamic_anchor.data == self.fragment:
             self.dynamic = True
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         refschema = self.refschema
 
         if self.dynamic:
-            target_scope = scope
+            target = result
             checked_uris = set()
 
-            while target_scope is not None:
-                if (base_uri := target_scope.schema.base_uri) is not None and base_uri not in checked_uris:
+            while target is not None:
+                if (base_uri := target.schema.base_uri) is not None and base_uri not in checked_uris:
                     checked_uris |= {base_uri}
                     target_uri = URI(f"#{self.fragment}").resolve(base_uri)
                     try:
                         found_schema = self.parentschema.catalog.get_schema(
                             target_uri, session=self.parentschema.session
                         )
                         if (dynamic_anchor := found_schema.get("$dynamicAnchor")) and \
                                 dynamic_anchor.data == self.fragment:
                             refschema = found_schema
                     except CatalogError:
                         pass
 
-                target_scope = target_scope.parent
+                target = target.parent
 
-        refschema.evaluate(instance, scope)
-        scope.refschema(refschema)
+        refschema.evaluate(instance, result)
+        result.refschema(refschema)
 
 
 class DynamicAnchorKeyword(Keyword):
     key = "$dynamicAnchor"
     static = True
 
     def __init__(self, parentschema: JSONSchema, value: str):
```

### Comparing `jschon-0.8.5/jschon/vocabulary/format.py` & `jschon-0.9.0/jschon/vocabulary/format.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable
 
 from jschon.exceptions import CatalogError
-from jschon.json import JSONCompatible, JSON
-from jschon.jsonschema import JSONSchema, Scope
+from jschon.json import JSON, JSONCompatible
+from jschon.jsonschema import JSONSchema, Result
 from jschon.vocabulary import Keyword
 
 __all__ = [
     'FormatKeyword',
     'FormatValidator',
 ]
 
@@ -27,16 +27,16 @@
         super().__init__(parentschema, value)
 
         try:
             self.validator: FormatValidator = parentschema.catalog.get_format_validator(value)
         except CatalogError:
             self.validator = None
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        scope.annotate(self.json.data)
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        result.annotate(self.json.data)
         if self.validator is not None:
             try:
                 self.validator(instance.data)
             except ValueError as e:
-                scope.fail(f'The instance is invalid against the "{self.json.data}" format: {e}')
+                result.fail(f'The instance is invalid against the "{self.json.data}" format: {e}')
         else:
-            scope.noassert()
+            result.noassert()
```

### Comparing `jschon-0.8.5/jschon/vocabulary/legacy.py` & `jschon-0.9.0/jschon/vocabulary/legacy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from jschon.exceptions import JSONSchemaError
 from jschon.json import JSON
-from jschon.jsonschema import JSONSchema, Scope
-from jschon.vocabulary import Keyword, Applicator, ArrayApplicator
+from jschon.jsonschema import JSONSchema, Result
+from jschon.vocabulary import Applicator, ArrayApplicator, Keyword
 
 __all__ = [
     'RecursiveRefKeyword_2019_09',
     'RecursiveAnchorKeyword_2019_09',
     'ItemsKeyword_2019_09',
     'AdditionalItemsKeyword_2019_09',
     'UnevaluatedItemsKeyword_2019_09',
@@ -26,112 +26,126 @@
         if (base_uri := self.parentschema.base_uri) is not None:
             self.refschema = self.parentschema.catalog.get_schema(
                 base_uri, metaschema_uri=self.parentschema.metaschema_uri, session=self.parentschema.session
             )
         else:
             raise JSONSchemaError(f'No base URI against which to resolve "$recursiveRef"')
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         refschema = self.refschema
         if (recursive_anchor := refschema.get("$recursiveAnchor")) and \
                 recursive_anchor.data is True:
 
-            target_scope = scope
-            while target_scope is not None:
-                if (base_anchor := target_scope.schema.get("$recursiveAnchor")) and \
+            target = result
+            while target is not None:
+                if (base_anchor := target.schema.get("$recursiveAnchor")) and \
                         base_anchor.data is True:
-                    refschema = target_scope.schema
+                    refschema = target.schema
 
-                target_scope = target_scope.parent
+                target = target.parent
 
-        refschema.evaluate(instance, scope)
-        scope.refschema(refschema)
+        refschema.evaluate(instance, result)
+        result.refschema(refschema)
 
 
 class RecursiveAnchorKeyword_2019_09(Keyword):
     key = "$recursiveAnchor"
     static = True
 
 
 class ItemsKeyword_2019_09(Keyword, Applicator, ArrayApplicator):
     key = "items"
-    types = "array",
+    instance_types = "array",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if len(instance) == 0:
             return
 
         elif isinstance(self.json.data, bool):
-            self.json.evaluate(instance, scope)
+            self.json.evaluate(instance, result)
 
         elif isinstance(self.json, JSONSchema):
             for index, item in enumerate(instance):
-                self.json.evaluate(item, scope)
+                self.json.evaluate(item, result)
 
-            if scope.passed:
-                scope.annotate(True)
+            if result.passed:
+                result.annotate(True)
 
         elif self.json.type == "array":
-            eval_index = None
-            err_indices = []
+            annotation = None
+            error = []
             for index, item in enumerate(instance[:len(self.json)]):
-                eval_index = index
-                with scope(item, str(index)) as subscope:
-                    self.json[index].evaluate(item, subscope)
-                    if not subscope.passed:
-                        err_indices += [index]
+                annotation = index
+                with result(item, str(index)) as subresult:
+                    if not self.json[index].evaluate(item, subresult).passed:
+                        error += [index]
 
-            if err_indices:
-                scope.fail(f"Array elements {err_indices} are invalid")
+            if error:
+                result.fail(error)
             else:
-                scope.annotate(eval_index)
+                result.annotate(annotation)
 
 
 class AdditionalItemsKeyword_2019_09(Keyword, Applicator):
     key = "additionalItems"
-    types = "array",
-    depends = "items",
+    instance_types = "array",
+    depends_on = "items",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        if (items := scope.sibling(instance, "items")) and type(items.annotation) is int:
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        if (items := result.sibling(instance, "items")) and type(items.annotation) is int:
             annotation = None
-            for index, item in enumerate(instance[items.annotation + 1:]):
-                annotation = True
-                self.json.evaluate(item, scope)
+            error = []
+            for index, item in enumerate(instance[(start := items.annotation + 1):], start):
+                if self.json.evaluate(item, result).passed:
+                    annotation = True
+                else:
+                    error += [index]
+                    # reset to passed for the next iteration
+                    result.pass_()
+
+            if error:
+                result.fail(error)
+            else:
+                result.annotate(annotation)
 
-            if scope.passed:
-                scope.annotate(annotation)
         else:
-            scope.discard()
+            result.discard()
 
 
 class UnevaluatedItemsKeyword_2019_09(Keyword, Applicator):
     key = "unevaluatedItems"
-    types = "array",
-    depends = "items", "additionalItems", "if", "then", "else", "allOf", "anyOf", "oneOf", "not",
+    instance_types = "array",
+    depends_on = "items", "additionalItems", "if", "then", "else", "allOf", "anyOf", "oneOf", "not",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         last_evaluated_item = -1
-        for items_annotation in scope.parent.collect_annotations(instance, "items"):
+        for items_annotation in result.parent.collect_annotations(instance, "items"):
             if items_annotation is True:
-                scope.discard()
+                result.discard()
                 return
             if type(items_annotation) is int and items_annotation > last_evaluated_item:
                 last_evaluated_item = items_annotation
 
-        for additional_items_annotation in scope.parent.collect_annotations(instance, "additionalItems"):
+        for additional_items_annotation in result.parent.collect_annotations(instance, "additionalItems"):
             if additional_items_annotation is True:
-                scope.discard()
+                result.discard()
                 return
 
-        for unevaluated_items_annotation in scope.parent.collect_annotations(instance, "unevaluatedItems"):
+        for unevaluated_items_annotation in result.parent.collect_annotations(instance, "unevaluatedItems"):
             if unevaluated_items_annotation is True:
-                scope.discard()
+                result.discard()
                 return
 
         annotation = None
-        for index, item in enumerate(instance[last_evaluated_item + 1:]):
-            annotation = True
-            self.json.evaluate(item, scope)
+        error = []
+        for index, item in enumerate(instance[(start := last_evaluated_item + 1):], start):
+            if self.json.evaluate(item, result).passed:
+                annotation = True
+            else:
+                error += [index]
+                # reset to passed for the next iteration
+                result.pass_()
 
-        if scope.passed:
-            scope.annotate(annotation)
+        if error:
+            result.fail(error)
+        else:
+            result.annotate(annotation)
```

### Comparing `jschon-0.8.5/jschon/vocabulary/validation.py` & `jschon-0.9.0/jschon/vocabulary/validation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import decimal
 import re
+from decimal import Decimal, InvalidOperation
 
 from jschon.json import JSON
-from jschon.jsonschema import Scope, JSONSchema
+from jschon.jsonschema import JSONSchema, Result
 from jschon.utils import tuplify
 from jschon.vocabulary import Keyword
 
 __all__ = [
     'TypeKeyword',
     'EnumKeyword',
     'ConstKeyword',
@@ -29,228 +29,228 @@
     'DependentRequiredKeyword',
 ]
 
 
 class TypeKeyword(Keyword):
     key = "type"
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         types = tuplify(self.json.data)
         if instance.type in types:
             valid = True
         elif instance.type == "number" and "integer" in types:
             valid = instance.data == int(instance.data)
         else:
             valid = False
 
         if not valid:
-            scope.fail(f"The instance must be of type {self.json}")
+            result.fail(f"The instance must be of type {self.json}")
 
 
 class EnumKeyword(Keyword):
     key = "enum"
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if instance not in self.json:
-            scope.fail("The instance value must be equal to one of the elements "
-                       "in the defined enumeration")
+            result.fail("The instance value must be equal to one of the elements "
+                        "in the defined enumeration")
 
 
 class ConstKeyword(Keyword):
     key = "const"
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if instance != self.json:
-            scope.fail(f"The instance value must be equal to the defined constant")
+            result.fail(f"The instance value must be equal to the defined constant")
 
 
 class MultipleOfKeyword(Keyword):
     key = "multipleOf"
-    types = "number",
+    instance_types = "number",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         try:
-            if instance.data % self.json.data != 0:
-                scope.fail(f"The value must be a multiple of {self.json}")
-        except decimal.InvalidOperation:
-            scope.fail(f"Invalid operation: {instance} % {self.json}")
+            if Decimal(f'{instance.data}') % Decimal(f'{self.json.data}') != 0:
+                result.fail(f"The value must be a multiple of {self.json}")
+        except InvalidOperation:
+            result.fail(f"Invalid operation: {instance} % {self.json}")
 
 
 class MaximumKeyword(Keyword):
     key = "maximum"
-    types = "number",
+    instance_types = "number",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if instance > self.json:
-            scope.fail(f"The value may not be greater than {self.json}")
+            result.fail(f"The value may not be greater than {self.json}")
 
 
 class ExclusiveMaximumKeyword(Keyword):
     key = "exclusiveMaximum"
-    types = "number",
+    instance_types = "number",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if instance >= self.json:
-            scope.fail(f"The value must be less than {self.json}")
+            result.fail(f"The value must be less than {self.json}")
 
 
 class MinimumKeyword(Keyword):
     key = "minimum"
-    types = "number",
+    instance_types = "number",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if instance < self.json:
-            scope.fail(f"The value may not be less than {self.json}")
+            result.fail(f"The value may not be less than {self.json}")
 
 
 class ExclusiveMinimumKeyword(Keyword):
     key = "exclusiveMinimum"
-    types = "number",
+    instance_types = "number",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if instance <= self.json:
-            scope.fail(f"The value must be greater than {self.json}")
+            result.fail(f"The value must be greater than {self.json}")
 
 
 class MaxLengthKeyword(Keyword):
     key = "maxLength"
-    types = "string",
+    instance_types = "string",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if len(instance) > self.json:
-            scope.fail(f"The text is too long (maximum {self.json} characters)")
+            result.fail(f"The text is too long (maximum {self.json} characters)")
 
 
 class MinLengthKeyword(Keyword):
     key = "minLength"
-    types = "string",
+    instance_types = "string",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if len(instance) < self.json:
-            scope.fail(f"The text is too short (minimum {self.json} characters)")
+            result.fail(f"The text is too short (minimum {self.json} characters)")
 
 
 class PatternKeyword(Keyword):
     key = "pattern"
-    types = "string",
+    instance_types = "string",
 
     def __init__(self, parentschema: JSONSchema, value: str):
         super().__init__(parentschema, value)
         self.regex = re.compile(value)
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if self.regex.search(instance.data) is None:
-            scope.fail(f"The text must match the regular expression {self.json}")
+            result.fail(f"The text must match the regular expression {self.json}")
 
 
 class MaxItemsKeyword(Keyword):
     key = "maxItems"
-    types = "array",
+    instance_types = "array",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if len(instance) > self.json:
-            scope.fail(f"The array has too many elements (maximum {self.json})")
+            result.fail(f"The array has too many elements (maximum {self.json})")
 
 
 class MinItemsKeyword(Keyword):
     key = "minItems"
-    types = "array",
+    instance_types = "array",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if len(instance) < self.json:
-            scope.fail(f"The array has too few elements (minimum {self.json})")
+            result.fail(f"The array has too few elements (minimum {self.json})")
 
 
 class UniqueItemsKeyword(Keyword):
     key = "uniqueItems"
-    types = "array",
+    instance_types = "array",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if not self.json.data:
             return
 
         uniquified = []
         for item in instance:
             if item not in uniquified:
                 uniquified += [item]
 
         if len(instance) > len(uniquified):
-            scope.fail("The array's elements must all be unique")
+            result.fail("The array's elements must all be unique")
 
 
 class MaxContainsKeyword(Keyword):
     key = "maxContains"
-    types = "array",
-    depends = "contains",
+    instance_types = "array",
+    depends_on = "contains",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        if contains := scope.sibling(instance, "contains"):
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        if contains := result.sibling(instance, "contains"):
             if contains.annotation is not None and len(contains.annotation) > self.json:
-                scope.fail('The array has too many elements matching the '
-                           f'"contains" subschema (maximum {self.json})')
+                result.fail('The array has too many elements matching the '
+                            f'"contains" subschema (maximum {self.json})')
 
 
 class MinContainsKeyword(Keyword):
     key = "minContains"
-    types = "array",
-    depends = "contains", "maxContains",
+    instance_types = "array",
+    depends_on = "contains", "maxContains",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
-        if contains := scope.sibling(instance, "contains"):
+    def evaluate(self, instance: JSON, result: Result) -> None:
+        if contains := result.sibling(instance, "contains"):
             contains_count = len(contains.annotation) \
                 if contains.annotation is not None \
                 else 0
 
             valid = contains_count >= self.json
 
             if valid and not contains.valid:
-                max_contains = scope.sibling(instance, "maxContains")
+                max_contains = result.sibling(instance, "maxContains")
                 if not max_contains or max_contains.valid:
                     contains.pass_()
 
             if not valid:
-                scope.fail('The array has too few elements matching the '
-                           f'"contains" subschema (minimum {self.json})')
+                result.fail('The array has too few elements matching the '
+                            f'"contains" subschema (minimum {self.json})')
 
 
 class MaxPropertiesKeyword(Keyword):
     key = "maxProperties"
-    types = "object",
+    instance_types = "object",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if len(instance) > self.json:
-            scope.fail(f"The object has too many properties (maximum {self.json})")
+            result.fail(f"The object has too many properties (maximum {self.json})")
 
 
 class MinPropertiesKeyword(Keyword):
     key = "minProperties"
-    types = "object",
+    instance_types = "object",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         if len(instance) < self.json:
-            scope.fail(f"The object has too few properties (minimum {self.json})")
+            result.fail(f"The object has too few properties (minimum {self.json})")
 
 
 class RequiredKeyword(Keyword):
     key = "required"
-    types = "object",
+    instance_types = "object",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         missing = [name.value for name in self.json if name.data not in instance]
         if missing:
-            scope.fail(f"The object is missing required properties {missing}")
+            result.fail(f"The object is missing required properties {missing}")
 
 
 class DependentRequiredKeyword(Keyword):
     key = "dependentRequired"
-    types = "object",
+    instance_types = "object",
 
-    def evaluate(self, instance: JSON, scope: Scope) -> None:
+    def evaluate(self, instance: JSON, result: Result) -> None:
         missing = {}
         for name, dependents in self.json.items():
             if name in instance:
                 missing_deps = [dep for dep in dependents if dep.data not in instance]
                 if missing_deps:
                     missing[name] = missing_deps
 
         if missing:
-            scope.fail(f"The object is missing dependent properties {missing}")
+            result.fail(f"The object is missing dependent properties {missing}")
```

### Comparing `jschon-0.8.5/jschon.egg-info/PKG-INFO` & `jschon-0.9.0/jschon.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jschon
-Version: 0.8.5
+Version: 0.9.0
 Summary: A pythonic, extensible JSON Schema implementation.
 Home-page: https://github.com/marksparkza/jschon
 Author: Mark Jacobson
 Author-email: mark@saeon.ac.za
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -43,15 +43,14 @@
   * Support for custom keywords, vocabularies and meta-schemas
   * Support for format validation
 
 * JSON class implementing the JSON data model
 * JSON Pointer (`RFC 6901 <https://tools.ietf.org/html/rfc6901.html>`_)
 * JSON Patch (`RFC 6902 <https://tools.ietf.org/html/rfc6902.html>`_)
 * Relative JSON Pointer (`draft <https://json-schema.org/draft/2020-12/relative-json-pointer.html>`_)
-* JSON document translation (`experimental <https://github.com/marksparkza/json-translation-vocabulary>`_)
 
 Installation
 ------------
 ::
 
     pip install jschon
```

### Comparing `jschon-0.8.5/jschon.egg-info/SOURCES.txt` & `jschon-0.9.0/jschon.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,24 @@
 jschon/exceptions.py
 jschon/json.py
 jschon/jsonpatch.py
 jschon/jsonpointer.py
 jschon/jsonschema.py
 jschon/output.py
 jschon/py.typed
-jschon/translation.py
 jschon/uri.py
 jschon/utils.py
 jschon.egg-info/PKG-INFO
 jschon.egg-info/SOURCES.txt
 jschon.egg-info/dependency_links.txt
 jschon.egg-info/requires.txt
 jschon.egg-info/top_level.txt
 jschon/catalog/_2019_09.py
 jschon/catalog/_2020_12.py
 jschon/catalog/__init__.py
-jschon/catalog/_translation.py
 jschon/catalog/json-schema-spec-2019-09/hyper-schema.json
 jschon/catalog/json-schema-spec-2019-09/links.json
 jschon/catalog/json-schema-spec-2019-09/schema.json
 jschon/catalog/json-schema-spec-2019-09/meta/applicator.json
 jschon/catalog/json-schema-spec-2019-09/meta/content.json
 jschon/catalog/json-schema-spec-2019-09/meta/core.json
 jschon/catalog/json-schema-spec-2019-09/meta/format.json
@@ -52,17 +50,14 @@
 jschon/catalog/json-schema-spec-2020-12/meta/hyper-schema.json
 jschon/catalog/json-schema-spec-2020-12/meta/meta-data.json
 jschon/catalog/json-schema-spec-2020-12/meta/unevaluated.json
 jschon/catalog/json-schema-spec-2020-12/meta/validation.json
 jschon/catalog/json-schema-spec-2020-12/output/hyper-schema.json
 jschon/catalog/json-schema-spec-2020-12/output/schema.json
 jschon/catalog/json-schema-spec-2020-12/output/verbose-example.json
-jschon/catalog/json-translation-vocabulary/schema.json
-jschon/catalog/json-translation-vocabulary/vocab.json
 jschon/vocabulary/__init__.py
 jschon/vocabulary/annotation.py
 jschon/vocabulary/applicator.py
 jschon/vocabulary/core.py
 jschon/vocabulary/format.py
 jschon/vocabulary/legacy.py
-jschon/vocabulary/translation.py
 jschon/vocabulary/validation.py
```

### Comparing `jschon-0.8.5/setup.py` & `jschon-0.9.0/setup.py`

 * *Files identical despite different names*

