# Comparing `tmp/fflogsapi-1.0.1.tar.gz` & `tmp/fflogsapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fflogsapi-1.0.1.tar", last modified: Mon Mar 20 19:54:15 2023, max compression
+gzip compressed data, was "fflogsapi-1.1.0.tar", last modified: Sun May 21 13:18:52 2023, max compression
```

## Comparing `fflogsapi-1.0.1.tar` & `fflogsapi-1.1.0.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:15.265256 fflogsapi-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-03-20 19:54:15.265256 fflogsapi-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:15.253256 fflogsapi-1.0.1/fflogsapi/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:15.253256 fflogsapi-1.0.1/fflogsapi/characters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/characters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/characters/character.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/characters/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/characters/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:15.257256 fflogsapi-1.0.1/fflogsapi/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/data/page.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/data/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:15.257256 fflogsapi-1.0.1/fflogsapi/game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/game/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/game/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/game/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/game/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:15.257256 fflogsapi-1.0.1/fflogsapi/guilds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/guilds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/guilds/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/guilds/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/guilds/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/guilds/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/guilds/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:15.257256 fflogsapi-1.0.1/fflogsapi/prograce/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/prograce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/prograce/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/prograce/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:15.261256 fflogsapi-1.0.1/fflogsapi/reports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/reports/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/reports/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    17663 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/reports/fight.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/reports/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/reports/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/reports/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:15.261256 fflogsapi-1.0.1/fflogsapi/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/user/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/user/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/user_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:15.261256 fflogsapi-1.0.1/fflogsapi/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/util/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/util/gql_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/util/indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:15.265256 fflogsapi-1.0.1/fflogsapi/world/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/world/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/world/encounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/world/expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/world/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/world/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/world/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/world/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/fflogsapi/world/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:54:15.253256 fflogsapi-1.0.1/fflogsapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-03-20 19:54:15.000000 fflogsapi-1.0.1/fflogsapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-20 19:54:15.000000 fflogsapi-1.0.1/fflogsapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:54:15.000000 fflogsapi-1.0.1/fflogsapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-20 19:54:15.000000 fflogsapi-1.0.1/fflogsapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-20 19:54:15.000000 fflogsapi-1.0.1/fflogsapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-20 19:54:04.000000 fflogsapi-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 19:54:15.265256 fflogsapi-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:52.293582 fflogsapi-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-21 13:18:52.293582 fflogsapi-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:52.285582 fflogsapi-1.1.0/fflogsapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:52.285582 fflogsapi-1.1.0/fflogsapi/characters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/characters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/characters/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/characters/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/characters/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/characters/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:52.285582 fflogsapi-1.1.0/fflogsapi/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/data/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/data/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:52.289582 fflogsapi-1.1.0/fflogsapi/game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/game/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/game/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/game/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/game/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:52.289582 fflogsapi-1.1.0/fflogsapi/guilds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/guilds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/guilds/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/guilds/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/guilds/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/guilds/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/guilds/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:52.289582 fflogsapi-1.1.0/fflogsapi/prograce/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/prograce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/prograce/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/prograce/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:52.289582 fflogsapi-1.1.0/fflogsapi/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/reports/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/reports/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18420 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/reports/fight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/reports/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/reports/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/reports/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:52.289582 fflogsapi-1.1.0/fflogsapi/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/user/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/user/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/user_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:52.289582 fflogsapi-1.1.0/fflogsapi/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/util/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/util/gql_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/util/indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:52.293582 fflogsapi-1.1.0/fflogsapi/world/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/world/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/world/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/world/encounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/world/expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/world/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/world/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/world/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/world/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/fflogsapi/world/zone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 13:18:52.285582 fflogsapi-1.1.0/fflogsapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-21 13:18:52.000000 fflogsapi-1.1.0/fflogsapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-21 13:18:52.000000 fflogsapi-1.1.0/fflogsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 13:18:52.000000 fflogsapi-1.1.0/fflogsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-21 13:18:52.000000 fflogsapi-1.1.0/fflogsapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 13:18:52.000000 fflogsapi-1.1.0/fflogsapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-21 13:18:26.000000 fflogsapi-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 13:18:52.293582 fflogsapi-1.1.0/setup.cfg
```

### Comparing `fflogsapi-1.0.1/LICENSE` & `fflogsapi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/__init__.py` & `fflogsapi-1.1.0/fflogsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/characters/character.py` & `fflogsapi-1.1.0/fflogsapi/data/page.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,172 +1,176 @@
-from typing import TYPE_CHECKING, Any, Dict
+from typing import TYPE_CHECKING, Any, Optional
 
-from ..util.decorators import fetch_data
 from ..util.filters import construct_filter_string
 from ..util.indexing import itindex
-from .queries import Q_CHARACTER_DATA
+from .queries import Q_PAGE_META
 
 if TYPE_CHECKING:
-    from ..client import FFLogsClient
-    from ..guilds.guild import FFLogsGuild
-    from ..world.server import FFLogsServer
+    from client import FFLogsClient
 
 
-class FFLogsCharacter:
+class FFLogsPage:
     '''
-    Representation of a character on FFLogs.
+    Representation of a page of data on FFLogs.
+    Base class for specific page types, do not use.
     '''
 
-    DATA_INDICES = ['characterData', 'character']
-
-    def __init__(self, filters: dict = {}, id: int = -1, client: 'FFLogsClient' = None) -> None:
+    # Base query from which to find pages
+    PAGINATION_QUERY: str = ''
+    # How to index the queried data to reach page metadata
+    PAGE_INDICES: list = []
+    # The data fields of the objects in the page to retrieve
+    DATA_FIELDS = []
+
+    def __init__(self,
+                 page_num: int,
+                 filters: dict[str, str] = {},
+                 client: 'FFLogsClient' = None,
+                 additional_formatting: dict[str, str] = {},
+                 ) -> None:
+        self.page_num = page_num
+        self.n_from = -1
+        self.n_to = -1
         self.filters = filters.copy()
-        if id != -1 and 'id' not in self.filters:
-            self.filters['id'] = id
+        self.additional_formatting = additional_formatting
+        self.data = None
+        self.objects = None
 
-        self._id = self.filters['id'] if 'id' in self.filters else -1
-        self._data = {}
         self._client = client
+        self._initialized = False
 
-    def _query_data(self, query: str, ignore_cache: bool = False) -> Dict[Any, Any]:
-        '''
-        Query for a specific piece of information about a character
-        '''
-        filters = construct_filter_string(self.filters)
-        result = self._client.q(Q_CHARACTER_DATA.format(
-            filters=filters,
-            innerQuery=query,
-        ), ignore_cache=ignore_cache)
+    def __iter__(self) -> 'FFLogsPageIterator':
+        return FFLogsPageIterator(page=self)
 
-        return itindex(result, self.DATA_INDICES)
+    def __len__(self) -> int:
+        return self.count()
 
-    @fetch_data('id')
-    def id(self) -> int:
+    def _query_page(self) -> None:
         '''
-        Get the character's ID.
-
-        Returns:
-            The character's ID.
-        '''
-        # A tiny bit of bookkeeping. Store the ID if we don't have it already,
-        # then use it to filter in the future
-        if self._id == -1:
-            self._id = self._data['id']
-            self.filters = {'id': self._id}
-        return self._data['id']
-
-    @fetch_data('lodestoneID')
-    def lodestone_id(self) -> int:
+        Retrieves metadata about data contained in this page.
+        Specifically, IDs/codes are gathered and stored.
         '''
-        Get the character's Lodestone ID.
-
-        Returns:
-            The character's Lodestone ID.
-        '''
-        return self._data['lodestoneID']
+        self.filters['page'] = self.page_num
+        filters = construct_filter_string(self.filters)
+        data_fields = ','.join(self.DATA_FIELDS)
+        page_data = self._client.q(self.PAGINATION_QUERY.format(
+            filters=filters,
+            innerQuery=Q_PAGE_META.format(dataFields=data_fields),
+            **self.additional_formatting,
+        ))
+        page_data = itindex(page_data, self.PAGE_INDICES)
 
-    @fetch_data('name')
-    def name(self) -> str:
-        '''
-        Get the character's name.
+        self.n_from = page_data['from']
+        self.n_to = page_data['to']
+        self.data = page_data['data']
+        self.objects = [None] * len(self.data)
 
-        Returns:
-            The character's name.
-        '''
-        return self._data['name']
+        self._initialized = True
 
-    def server(self) -> 'FFLogsServer':
+    def count(self) -> int:
         '''
-        Get the server the character belongs to.
-
         Returns:
-            The character's server.
+            The amount of objects in this page.
         '''
-        from ..world.server import FFLogsServer
-        server_id = self._query_data('server{ id }')['server']['id']
-        return FFLogsServer(filters={'id': server_id}, client=self._client)
+        if not self._initialized:
+            self._query_page()
 
-    @fetch_data('guildRank')
-    def fc_rank(self) -> str:
-        '''
-        Get the FC rank of the character. This is game data, not FFLogs data.
-
-        Returns:
-            The character's FC rank.
-        '''
-        return self._data['guildRank']
+        return (self.n_to - self.n_from) + 1
 
-    def guilds(self) -> list['FFLogsGuild']:
+    def init_object(self, data: dict) -> Any:
         '''
-        Get a list of all guilds that this character belongs to.
-
-        Returns:
-            A list of guilds the character is in.
+        Initializes an instance of the object being paginated. Up to implementation.
         '''
-        from ..guilds.guild import FFLogsGuild
-        guilds = self._query_data('guilds{ id }')['guilds']
-        return [FFLogsGuild(id=guild['id'], client=self._client) for guild in guilds]
+        pass
 
-    def game_data(self, filters: dict = {}) -> dict:
+    def object(self, idx: int) -> Optional[Any]:
         '''
-        Get cached game data tied to the character, such as gear.
+        Get a specific object from this page.
 
         Args:
-            filters: Filter game data to a specific `specID` or force an update by the API with
-                     `forceUpdate`.
+            idx: The page index of the object to retrieve from the page
         Returns:
-            The character's game data.
+            An object or None if the object is not contained in the page
         '''
-        filters = construct_filter_string(filters)
-        if filters:
-            filters = f'({filters})'
+        if not self._initialized:
+            self._query_page()
 
-        result = self._query_data(f'gameData{filters}')
-        return result['gameData']
+        if idx < 0 or idx > len(self.data):
+            return None
 
-    @fetch_data('hidden')
-    def hidden(self) -> bool:
-        '''
-        Whether or not the character's rankings are hidden.
+        if self.objects[idx] is None:
+            self.objects[idx] = self.init_object(self.data[idx])
 
-        Returns:
-            True if the rankings are hidden, False otherwise.
-        '''
-        return self._data['hidden']
+        return self.objects[idx]
 
-    def encounter_rankings(self, filters: Dict[str, Any] = {}) -> Dict:
-        '''
-        Get this character's rankings for different encounters. `encounterID` is mandatory.
 
-        For valid filter fields, see the API documentation:
-        https://www.fflogs.com/v2-api-docs/ff/character.doc.html
+class FFLogsPageIterator:
+    '''
+    Iterates over a page, returning the object being paginated
+    '''
 
-        Args:
-            filters: Key-value filters to filter the rankings by. E.g. job name, encounter ID, etc.
-        Returns:
-            The character's filtered ranking data.
-        '''
-        filters = construct_filter_string(filters)
-        if filters:
-            filters = f'({filters})'
+    def __init__(self, page: 'FFLogsPage') -> None:
+        self._page = page
+        self._cur_idx = -1
+        self._max_amount = page.count()
+
+    def __iter__(self) -> 'FFLogsPageIterator':
+        return self
+
+    def __next__(self) -> Any:
+        self._cur_idx += 1
+        if self._cur_idx < self._max_amount:
+            return self._page.object(self._cur_idx)
+        else:
+            self._cur_idx = -1
+            raise StopIteration
 
-        result = self._query_data(f'encounterRankings{filters}')
-        return result['encounterRankings']
 
-    def zone_rankings(self, filters: Dict[str, Any] = {}) -> Dict:
-        '''
-        Get this character's rankings for different zones (bosses).
+class FFLogsPaginationIterator:
+    '''
+    Iterates over multiple pages (a pagination), returning pages
+    '''
 
-        For valid filter fields, see the API documentation:
-        https://www.fflogs.com/v2-api-docs/ff/character.doc.html
+    # The page class of the pages in the pagination
+    PAGE_CLASS = None
 
-        Args:
-            filters: Key-value filters to filter the rankings by. E.g. job name, zone ID, etc.
-        Returns:
-            The character's filtered ranking data.
+    def __init__(
+        self,
+        client: 'FFLogsClient',
+        filters: dict[str, Any] = {},
+        additional_formatting: dict[str, str] = {},
+    ) -> None:
         '''
-        filters = construct_filter_string(filters)
-        if filters:
-            filters = f'({filters})'
-
-        result = self._query_data(f'zoneRankings{filters}')
-        return result['zoneRankings']
+        If the pagination query requires any additional formatting,
+        it can be specified using `additional_formatting`.
+        '''
+        self._client = client
+        self._cur_page = 0
+        self._filters = filters.copy()
+        self.additional_formatting = additional_formatting
+
+        pagination_filters = self._filters.copy()
+        pagination_filters['page'] = 1
+        filters = construct_filter_string(pagination_filters)
+        result = self._client.q(self.PAGE_CLASS.PAGINATION_QUERY.format(
+            filters=filters,
+            innerQuery='last_page',
+            **additional_formatting,
+        ))
+
+        self._last_page = itindex(result, self.PAGE_CLASS.PAGE_INDICES)['last_page']
+
+    def __iter__(self) -> 'FFLogsPaginationIterator':
+        return self
+
+    def __next__(self) -> FFLogsPage:
+        self._cur_page += 1
+        if self._cur_page <= self._last_page:
+            return self.PAGE_CLASS(
+                page_num=self._cur_page,
+                filters=self._filters,
+                client=self._client,
+                additional_formatting=self.additional_formatting,
+            )
+        else:
+            self._cur_page = 0
+            raise StopIteration
```

### Comparing `fflogsapi-1.0.1/fflogsapi/characters/client_extensions.py` & `fflogsapi-1.1.0/fflogsapi/characters/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/client.py` & `fflogsapi-1.1.0/fflogsapi/client.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/constants.py` & `fflogsapi-1.1.0/fflogsapi/constants.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/game/client_extensions.py` & `fflogsapi-1.1.0/fflogsapi/game/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/game/dataclasses.py` & `fflogsapi-1.1.0/fflogsapi/game/dataclasses.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/game/pages.py` & `fflogsapi-1.1.0/fflogsapi/game/pages.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/game/queries.py` & `fflogsapi-1.1.0/fflogsapi/game/queries.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/guilds/client_extensions.py` & `fflogsapi-1.1.0/fflogsapi/guilds/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/guilds/dataclasses.py` & `fflogsapi-1.1.0/fflogsapi/guilds/dataclasses.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/guilds/guild.py` & `fflogsapi-1.1.0/fflogsapi/guilds/guild.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/guilds/pages.py` & `fflogsapi-1.1.0/fflogsapi/guilds/pages.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/guilds/queries.py` & `fflogsapi-1.1.0/fflogsapi/guilds/queries.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/prograce/client_extensions.py` & `fflogsapi-1.1.0/fflogsapi/prograce/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/reports/client_extensions.py` & `fflogsapi-1.1.0/fflogsapi/reports/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/reports/dataclasses.py` & `fflogsapi-1.1.0/fflogsapi/reports/dataclasses.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/reports/fight.py` & `fflogsapi-1.1.0/fflogsapi/reports/fight.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,14 +105,39 @@
     def fight_percentage(self) -> float:
         '''
         Returns:
             The minimum percentage of the entire fight that was reached
         '''
         return self._data['fightPercentage']
 
+    @fetch_data('lastPhase')
+    def last_phase(self) -> int:
+        '''
+        Returns:
+            The last phase the fight was in when it ended
+        '''
+        return self._data['lastPhase']
+
+    @fetch_data('lastPhaseAsAbsoluteIndex')
+    def last_phase_absolute(self) -> int:
+        '''
+        Returns:
+            The last phase the fight was in when it ended,
+            counting from 0 and including intermissions
+        '''
+        return self._data['lastPhaseAsAbsoluteIndex']
+
+    @fetch_data('lastPhaseIsIntermission')
+    def last_phase_intermission(self) -> bool:
+        '''
+        Returns:
+            Whether or not the last phase of the fight is an intermission
+        '''
+        return self._data['lastPhaseIsIntermission']
+
     @fetch_data('difficulty')
     def difficulty(self) -> Optional[int]:
         '''
         Usually not very descriptive, as difficulty level 100 covers a wide variety of content.
 
         Returns:
             The difficulty of the fight.
```

### Comparing `fflogsapi-1.0.1/fflogsapi/reports/pages.py` & `fflogsapi-1.1.0/fflogsapi/reports/pages.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/reports/queries.py` & `fflogsapi-1.1.0/fflogsapi/reports/queries.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/reports/report.py` & `fflogsapi-1.1.0/fflogsapi/reports/report.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/user/client_extensions.py` & `fflogsapi-1.1.0/fflogsapi/user/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/user/user.py` & `fflogsapi-1.1.0/fflogsapi/user/user.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/user_auth.py` & `fflogsapi-1.1.0/fflogsapi/user_auth.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/util/decorators.py` & `fflogsapi-1.1.0/fflogsapi/util/decorators.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/util/filters.py` & `fflogsapi-1.1.0/fflogsapi/util/filters.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/world/client_extensions.py` & `fflogsapi-1.1.0/fflogsapi/world/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/world/encounter.py` & `fflogsapi-1.1.0/fflogsapi/world/encounter.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/world/expansion.py` & `fflogsapi-1.1.0/fflogsapi/world/expansion.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/world/pages.py` & `fflogsapi-1.1.0/fflogsapi/world/pages.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/world/queries.py` & `fflogsapi-1.1.0/fflogsapi/world/queries.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/world/region.py` & `fflogsapi-1.1.0/fflogsapi/world/region.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/world/server.py` & `fflogsapi-1.1.0/fflogsapi/world/server.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-1.0.1/fflogsapi/world/zone.py` & `fflogsapi-1.1.0/fflogsapi/world/zone.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Union
+from warnings import warn
 
 from ..util.decorators import fetch_data
 from ..util.indexing import itindex
+from .dataclasses import FFLogsPartition
 from .queries import Q_ZONE
 
 if TYPE_CHECKING:
     from ..client import FFLogsClient
     from .encounter import FFLogsEncounter
     from .expansion import FFLogsExpansion
 
@@ -83,23 +85,39 @@
 
         Returns:
             The zone's bracket information.
         '''
         bracket_info = self._query_data('brackets{ type, min, max, bucket }')
         return bracket_info['brackets']
 
-    def partitions(self) -> dict:
+    def partitions(self, use_dataclass=False) -> Union[dict, list[FFLogsPartition]]:
         '''
         Get partition information about the zone.
 
         Returns:
             The zone's partition information.
         '''
         partition_info = self._query_data('partitions{ id, name, compactName, default }')
-        return partition_info['partitions']
+        partition_info = partition_info['partitions']
+
+        if not use_dataclass:
+            warn(
+                'dict returns from FFLogsZone.partitions is being deprecated. '
+                'pass use_dataclass=True to get the new dataclass return instead.',
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+            return partition_info
+
+        return [FFLogsPartition(
+            id=partition['id'],
+            name=partition['name'],
+            compact_name=partition['compactName'],
+            default=partition['default'],
+        ) for partition in partition_info]
 
     def difficulties(self) -> dict:
         '''
         Get difficulty information about the zone.
 
         Returns:
             The zone's difficulty information.
```

### Comparing `fflogsapi-1.0.1/fflogsapi.egg-info/SOURCES.txt` & `fflogsapi-1.1.0/fflogsapi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 fflogsapi.egg-info/SOURCES.txt
 fflogsapi.egg-info/dependency_links.txt
 fflogsapi.egg-info/requires.txt
 fflogsapi.egg-info/top_level.txt
 fflogsapi/characters/__init__.py
 fflogsapi/characters/character.py
 fflogsapi/characters/client_extensions.py
+fflogsapi/characters/dataclasses.py
 fflogsapi/characters/queries.py
 fflogsapi/data/__init__.py
 fflogsapi/data/page.py
 fflogsapi/data/queries.py
 fflogsapi/game/__init__.py
 fflogsapi/game/client_extensions.py
 fflogsapi/game/dataclasses.py
@@ -45,14 +46,15 @@
 fflogsapi/util/__init__.py
 fflogsapi/util/decorators.py
 fflogsapi/util/filters.py
 fflogsapi/util/gql_enums.py
 fflogsapi/util/indexing.py
 fflogsapi/world/__init__.py
 fflogsapi/world/client_extensions.py
+fflogsapi/world/dataclasses.py
 fflogsapi/world/encounter.py
 fflogsapi/world/expansion.py
 fflogsapi/world/pages.py
 fflogsapi/world/queries.py
 fflogsapi/world/region.py
 fflogsapi/world/server.py
 fflogsapi/world/zone.py
```

### Comparing `fflogsapi-1.0.1/pyproject.toml` & `fflogsapi-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'fflogsapi'
-version = '1.0.1'
+version = '1.1.0'
 description = 'Python client for the FF Logs v2 API'
 readme = 'README.md'
 authors = [
     { name = 'Markus Wang Halvorsen', email = 'mwh@halvorsenfamilien.com' },
 ]
 keywords = ['api', 'client', 'ffxiv', 'fflogs', 'lazy']
 classifiers = [
```

