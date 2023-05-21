# Comparing `tmp/spetlr-1.1.84.tar.gz` & `tmp/spetlr-1.1.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spetlr-1.1.84.tar", last modified: Tue May 16 11:24:21 2023, max compression
+gzip compressed data, was "spetlr-1.1.86.tar", last modified: Sun May 21 21:12:43 2023, max compression
```

## Comparing `spetlr-1.1.84.tar` & `spetlr-1.1.86.tar`

### file list

```diff
@@ -1,271 +1,271 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.949528 spetlr-1.1.84/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-16 11:24:10.000000 spetlr-1.1.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 11:24:10.000000 spetlr-1.1.84/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-16 11:24:21.949528 spetlr-1.1.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-16 11:24:10.000000 spetlr-1.1.84/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-16 11:24:10.000000 spetlr-1.1.84/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-16 11:24:21.949528 spetlr-1.1.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 11:24:10.000000 spetlr-1.1.84/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.925528 spetlr-1.1.84/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.929528 spetlr-1.1.84/src/spetlr/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/alias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.929528 spetlr-1.1.84/src/spetlr/cache/
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/cache/CachedLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/cache/CachedLoaderParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.929528 spetlr-1.1.84/src/spetlr/config_master/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/config_master/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.929528 spetlr-1.1.84/src/spetlr/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.929528 spetlr-1.1.84/src/spetlr/configurator/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/_cli/generate_keys_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.933528 spetlr-1.1.84/src/spetlr/configurator/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/StatementBlocks.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/init_sqlparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/parse_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.933528 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.933528 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/engine/filter_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/engine/grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/engine/statement_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.933528 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/aligned_indent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/others.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/reindent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/right_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20547 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/substructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/configurator/sql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.933528 spetlr-1.1.84/src/spetlr/cosmos/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/cosmos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/cosmos/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/cosmos/cosmos_base_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/cosmos/cosmos_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/db_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.933528 spetlr-1.1.84/src/spetlr/delta/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/delta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/delta/db_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/delta/delta_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.933528 spetlr-1.1.84/src/spetlr/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/eh/EventHubCapture.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/eh/EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/eh/EventHubJsonPublisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/eh/EventHubStream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/eh/PartitionSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/eh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/eh/eh_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/entry_points/generalized_task_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/entry_points/task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/etl/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/etl/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/extractors/incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/extractors/schema_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/extractors/simple_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/etl/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/loaders/DeleteDataLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/loaders/UpsertLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/loaders/simple_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/loaders/simple_sql_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/etl/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/exceptions/cli_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/exceptions/configurator_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/extractors/eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/formatting/git_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/mount/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/mount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/mount/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/orchestrators/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/orchestrators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/orchestrators/eh2bronze/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/orchestrators/eh2bronze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/orchestrators/eh2silver/
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/orchestrators/eh2silver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/orchestrators/ehjson2delta/
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/orchestrators/ehjson2delta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/reporting/JobReflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/reporting/SlackNotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.937528 spetlr-1.1.84/src/spetlr/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/schema_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/schema_manager/schema_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/schema_manager/spark_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.941528 spetlr-1.1.84/src/spetlr/singleton/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/singleton/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/spark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.941528 spetlr-1.1.84/src/spetlr/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/sql/BaseExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/sql/CommonBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/sql/SqlBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/sql/SqlExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13169 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/sql/SqlServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/sql/SqlServerBaseOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/sql/sql_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.941528 spetlr-1.1.84/src/spetlr/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/tables/TableHandle.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/tables/ThMaker.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.941528 spetlr-1.1.84/src/spetlr/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformers/dropColumnsTransformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformers/drop_oldest_duplicate_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformers/fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformers/join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformers/selectColumnsTransformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformers/simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformers/simple_sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformers/timezone_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformers/union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformers/union_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/transformers/validfromto_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.941528 spetlr-1.1.84/src/spetlr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/utils/CheckDfMerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/utils/DataframeCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/utils/DropOldestDuplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/utils/GetMergeStatement.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/utils/MockExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/utils/MockLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/utils/SelectAndCastColumns.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-16 11:24:10.000000 spetlr-1.1.84/src/spetlr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.929528 spetlr-1.1.84/src/spetlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-16 11:24:21.000000 spetlr-1.1.84/src/spetlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-16 11:24:21.000000 spetlr-1.1.84/src/spetlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:24:21.000000 spetlr-1.1.84/src/spetlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-16 11:24:21.000000 spetlr-1.1.84/src/spetlr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:24:21.000000 spetlr-1.1.84/src/spetlr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-16 11:24:21.000000 spetlr-1.1.84/src/spetlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 11:24:21.000000 spetlr-1.1.84/src/spetlr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.925528 spetlr-1.1.84/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.925528 spetlr-1.1.84/tests/cluster/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.941528 spetlr-1.1.84/tests/cluster/cache/
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/cache/test_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.941528 spetlr-1.1.84/tests/cluster/cosmos/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/cosmos/test_cosmos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.941528 spetlr-1.1.84/tests/cluster/db/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/db/test_db_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.941528 spetlr-1.1.84/tests/cluster/delta/
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/delta/test_delta_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.941528 spetlr-1.1.84/tests/cluster/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/eh/test_eh_json_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/eh/test_eh_json_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/eh/test_eh_saving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.945528 spetlr-1.1.84/tests/cluster/etl/
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/etl/test_delete_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/etl/test_deltaupsert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/etl/test_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/etl/test_incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/etl/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/etl/test_orchestrator_etl_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/etl/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/etl/test_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/etl/test_upsertloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.945528 spetlr-1.1.84/tests/cluster/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.945528 spetlr-1.1.84/tests/cluster/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.945528 spetlr-1.1.84/tests/cluster/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/sql/test_deliveryexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/sql/test_deliverysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/sql/test_deliverysqlspn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/sql/test_simple_sql_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/sql/test_sqlhandle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.945528 spetlr-1.1.84/tests/cluster/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/transformations/test_merge_df_into_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/cluster/transformations/test_union_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.945528 spetlr-1.1.84/tests/local/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.945528 spetlr-1.1.84/tests/local/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/configurator/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/configurator/test_configurator_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.945528 spetlr-1.1.84/tests/local/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/eh/test_EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/eh/test_ehto_bronze_and_silver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/eh/test_ehtodeltabronze_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/eh/test_ehtodeltabronze_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/eh/test_ehtodeltasilver_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.945528 spetlr-1.1.84/tests/local/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/entry_points/test_task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.945528 spetlr-1.1.84/tests/local/etl/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/etl/test_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.945528 spetlr-1.1.84/tests/local/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/extractors/test_eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.945528 spetlr-1.1.84/tests/local/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.945528 spetlr-1.1.84/tests/local/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.949528 spetlr-1.1.84/tests/local/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/sql/test_SqlExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/test_get_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/test_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/test_sqlServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/test_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.949528 spetlr-1.1.84/tests/local/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/transformers/test_concat_df.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/transformers/test_drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/transformers/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/transformers/test_fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/transformers/test_join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/transformers/test_select_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/transformers/test_simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/transformers/test_timezone_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/transformers/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/transformers/test_union_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/transformers/test_validfromto_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:24:21.949528 spetlr-1.1.84/tests/local/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/utils/test_dataframe_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/utils/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/utils/test_getmergestatement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/utils/test_mock_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-05-16 11:24:10.000000 spetlr-1.1.84/tests/local/utils/test_selectandcastcolumns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.409796 spetlr-1.1.86/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-21 21:12:28.000000 spetlr-1.1.86/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-21 21:12:28.000000 spetlr-1.1.86/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-21 21:12:43.413796 spetlr-1.1.86/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-21 21:12:28.000000 spetlr-1.1.86/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-21 21:12:28.000000 spetlr-1.1.86/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-21 21:12:43.413796 spetlr-1.1.86/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 21:12:28.000000 spetlr-1.1.86/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.353796 spetlr-1.1.86/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.369796 spetlr-1.1.86/src/spetlr/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/alias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.369796 spetlr-1.1.86/src/spetlr/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/cache/CachedLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/cache/CachedLoaderParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.369796 spetlr-1.1.86/src/spetlr/config_master/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/config_master/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.369796 spetlr-1.1.86/src/spetlr/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.369796 spetlr-1.1.86/src/spetlr/configurator/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/_cli/generate_keys_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.373796 spetlr-1.1.86/src/spetlr/configurator/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/StatementBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/init_sqlparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/parse_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.373796 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.373796 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/engine/filter_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14096 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/engine/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/engine/statement_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.377796 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/aligned_indent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/others.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/reindent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/right_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20547 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/substructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/configurator/sql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.377796 spetlr-1.1.86/src/spetlr/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/cosmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/cosmos/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/cosmos/cosmos_base_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/cosmos/cosmos_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/db_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.377796 spetlr-1.1.86/src/spetlr/delta/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/delta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/delta/db_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/delta/delta_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.385796 spetlr-1.1.86/src/spetlr/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/eh/EventHubCapture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/eh/EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/eh/EventHubJsonPublisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/eh/EventHubStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/eh/PartitionSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/eh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/eh/eh_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.385796 spetlr-1.1.86/src/spetlr/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/entry_points/generalized_task_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/entry_points/task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.385796 spetlr-1.1.86/src/spetlr/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.389796 spetlr-1.1.86/src/spetlr/etl/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/extractors/incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/extractors/schema_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/extractors/simple_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.389796 spetlr-1.1.86/src/spetlr/etl/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/loaders/DeleteDataLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/loaders/UpsertLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/loaders/simple_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/loaders/simple_sql_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/etl/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.389796 spetlr-1.1.86/src/spetlr/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/exceptions/cli_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/exceptions/configurator_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.389796 spetlr-1.1.86/src/spetlr/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/extractors/eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.389796 spetlr-1.1.86/src/spetlr/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/formatting/git_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.389796 spetlr-1.1.86/src/spetlr/mount/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/mount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/mount/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.389796 spetlr-1.1.86/src/spetlr/orchestrators/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/orchestrators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.389796 spetlr-1.1.86/src/spetlr/orchestrators/eh2bronze/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/orchestrators/eh2bronze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.389796 spetlr-1.1.86/src/spetlr/orchestrators/eh2silver/
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/orchestrators/eh2silver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.393796 spetlr-1.1.86/src/spetlr/orchestrators/ehjson2delta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/orchestrators/ehjson2delta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.393796 spetlr-1.1.86/src/spetlr/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/reporting/JobReflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/reporting/SlackNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.393796 spetlr-1.1.86/src/spetlr/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/schema_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/schema_manager/schema_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/schema_manager/spark_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.393796 spetlr-1.1.86/src/spetlr/singleton/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/singleton/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/spark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.393796 spetlr-1.1.86/src/spetlr/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/sql/BaseExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/sql/CommonBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/sql/SqlBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/sql/SqlExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/sql/SqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/sql/SqlServerBaseOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/sql/sql_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.397796 spetlr-1.1.86/src/spetlr/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/tables/TableHandle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/tables/ThMaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.397796 spetlr-1.1.86/src/spetlr/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformers/dropColumnsTransformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformers/drop_oldest_duplicate_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformers/fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformers/join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformers/selectColumnsTransformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformers/simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformers/simple_sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformers/timezone_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformers/union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformers/union_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/transformers/validfromto_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.401796 spetlr-1.1.86/src/spetlr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/utils/CheckDfMerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/utils/DataframeCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/utils/DropOldestDuplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/utils/GetMergeStatement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/utils/MockExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/utils/MockLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/utils/SelectAndCastColumns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-21 21:12:28.000000 spetlr-1.1.86/src/spetlr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.369796 spetlr-1.1.86/src/spetlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-21 21:12:42.000000 spetlr-1.1.86/src/spetlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-21 21:12:43.000000 spetlr-1.1.86/src/spetlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:12:42.000000 spetlr-1.1.86/src/spetlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-21 21:12:42.000000 spetlr-1.1.86/src/spetlr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:12:42.000000 spetlr-1.1.86/src/spetlr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-21 21:12:42.000000 spetlr-1.1.86/src/spetlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 21:12:42.000000 spetlr-1.1.86/src/spetlr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.365796 spetlr-1.1.86/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.361796 spetlr-1.1.86/tests/cluster/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.401796 spetlr-1.1.86/tests/cluster/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/cache/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.401796 spetlr-1.1.86/tests/cluster/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/cosmos/test_cosmos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.401796 spetlr-1.1.86/tests/cluster/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/db/test_db_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.401796 spetlr-1.1.86/tests/cluster/delta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/delta/test_delta_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.401796 spetlr-1.1.86/tests/cluster/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/eh/test_eh_json_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/eh/test_eh_json_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/eh/test_eh_saving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.401796 spetlr-1.1.86/tests/cluster/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/etl/test_delete_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/etl/test_deltaupsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/etl/test_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/etl/test_incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/etl/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/etl/test_orchestrator_etl_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/etl/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/etl/test_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/etl/test_upsertloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.401796 spetlr-1.1.86/tests/cluster/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.405796 spetlr-1.1.86/tests/cluster/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.405796 spetlr-1.1.86/tests/cluster/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/sql/test_deliveryexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/sql/test_deliverysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/sql/test_deliverysqlspn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/sql/test_simple_sql_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/sql/test_sqlhandle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.405796 spetlr-1.1.86/tests/cluster/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/transformations/test_merge_df_into_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/cluster/transformations/test_union_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.405796 spetlr-1.1.86/tests/local/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.405796 spetlr-1.1.86/tests/local/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/configurator/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/configurator/test_configurator_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.405796 spetlr-1.1.86/tests/local/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/eh/test_EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/eh/test_ehto_bronze_and_silver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/eh/test_ehtodeltabronze_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/eh/test_ehtodeltabronze_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/eh/test_ehtodeltasilver_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.405796 spetlr-1.1.86/tests/local/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/entry_points/test_task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.405796 spetlr-1.1.86/tests/local/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/etl/test_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.409796 spetlr-1.1.86/tests/local/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/extractors/test_eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.409796 spetlr-1.1.86/tests/local/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.409796 spetlr-1.1.86/tests/local/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.409796 spetlr-1.1.86/tests/local/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/sql/test_SqlExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/test_get_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/test_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/test_sqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/test_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.409796 spetlr-1.1.86/tests/local/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/transformers/test_concat_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/transformers/test_drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/transformers/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/transformers/test_fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/transformers/test_join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/transformers/test_select_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/transformers/test_simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/transformers/test_timezone_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/transformers/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/transformers/test_union_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/transformers/test_validfromto_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:12:43.409796 spetlr-1.1.86/tests/local/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/utils/test_dataframe_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/utils/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/utils/test_getmergestatement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/utils/test_mock_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-05-21 21:12:28.000000 spetlr-1.1.86/tests/local/utils/test_selectandcastcolumns.py
```

### Comparing `spetlr-1.1.84/LICENSE` & `spetlr-1.1.86/LICENSE`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/PKG-INFO` & `spetlr-1.1.86/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr
-Version: 1.1.84
+Version: 1.1.86
 Summary: A python SPark ETL libRary (SPETLR) for Databricks.
 Home-page: https://github.com/atc-net/atc-dataplatform
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr/issues
```

### Comparing `spetlr-1.1.84/README.md` & `spetlr-1.1.86/README.md`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/setup.cfg` & `spetlr-1.1.86/setup.cfg`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/cache/CachedLoader.py` & `spetlr-1.1.86/src/spetlr/cache/CachedLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/cache/CachedLoaderParameters.py` & `spetlr-1.1.86/src/spetlr/cache/CachedLoaderParameters.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/_cli/__init__.py` & `spetlr-1.1.86/src/spetlr/configurator/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/_cli/generate_keys_file.py` & `spetlr-1.1.86/src/spetlr/configurator/_cli/generate_keys_file.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/configurator.py` & `spetlr-1.1.86/src/spetlr/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/StatementBlocks.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/StatementBlocks.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/comments.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/comments.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/create.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/create.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/db.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/db.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/init_sqlparse.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/init_sqlparse.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/parse_sql.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/parse_sql.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/__init__.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/__main__.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/__main__.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/cli.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/cli.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/engine/__init__.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/engine/filter_stack.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/engine/filter_stack.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/engine/grouping.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/engine/grouping.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/engine/statement_splitter.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/engine/statement_splitter.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/__init__.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/aligned_indent.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/aligned_indent.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/others.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/others.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/output.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/output.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/reindent.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/reindent.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/right_margin.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/right_margin.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/filters/tokens.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/filters/tokens.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/formatter.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/formatter.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/keywords.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/keywords.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/lexer.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/lexer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/sql.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/sql.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/tokens.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/tokens.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/sqlparse/utils.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/sqlparse/utils.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/substructures.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/substructures.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/configurator/sql/table.py` & `spetlr-1.1.86/src/spetlr/configurator/sql/table.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/cosmos/cosmos.py` & `spetlr-1.1.86/src/spetlr/cosmos/cosmos.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/cosmos/cosmos_base_server.py` & `spetlr-1.1.86/src/spetlr/cosmos/cosmos_base_server.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/cosmos/cosmos_handle.py` & `spetlr-1.1.86/src/spetlr/cosmos/cosmos_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/db_auto.py` & `spetlr-1.1.86/src/spetlr/db_auto.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/delta/db_handle.py` & `spetlr-1.1.86/src/spetlr/delta/db_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/delta/delta_handle.py` & `spetlr-1.1.86/src/spetlr/delta/delta_handle.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,52 +110,30 @@
         Spark.get().sql(sql)
 
     def recreate_hive_table(self):
         self.drop()
         self.create_hive_table()
 
     def get_partitioning(self):
-        """The result of DESCRIBE TABLE tablename is like this:
-        +-----------------+---------------+-------+
-        |         col_name|      data_type|comment|
-        +-----------------+---------------+-------+
-        |           mycolA|         string|       |
-        |           myColB|            int|       |
-        |                 |               |       |
-        |   # Partitioning|               |       |
-        |           Part 0|         mycolA|       |
-        +-----------------+---------------+-------+
+        """The result of DESCRIBE DETAIL tablename is like this:
+        +------+--------------------+--------------------+----------------+-------+
+        |format|                  id|                name|partitionColumns|  ...  |
+        +------+--------------------+--------------------+----------------+-------+
+        | delta|c96a1e94-314b-427...|spark_catalog.tes...|    [colB, colA]|  ...  |
+        +------+--------------------+--------------------+----------------+-------+
         but this method return the partitioning in the form ['mycolA'],
         if there is no partitioning, an empty list is returned.
         """
         if self._partitioning is None:
-            # create an iterator object and use it in two steps
-            rows_iter = iter(
-                Spark.get().sql(f"DESCRIBE TABLE {self.get_tablename()}").collect()
+            self._partitioning = (
+                Spark.get()
+                .sql(f"DESCRIBE DETAIL {self.get_tablename()}")
+                .select("partitionColumns")
+                .collect()[0][0]
             )
-
-            # roll over the iterator until you see the title line
-            for row in rows_iter:
-                # discard rows until the important section header
-                if row.col_name.strip() == "# Partitioning":
-                    break
-            # at this point, the iterator has moved past the section heading
-            # leaving only the rows with "Part 1" etc.
-
-            # create a list from the rest of the iterator like [(0,colA), (1,colB)]
-            parts = [
-                (int(row.col_name[5:]), row.data_type)
-                for row in rows_iter
-                if row.col_name.startswith("Part ")
-            ]
-            # sort, just in case the parts were out of order.
-            parts.sort()
-
-            # discard the index and put into an ordered list.
-            self._partitioning = [p[1] for p in parts]
         return self._partitioning
 
     def get_tablename(self) -> str:
         return self._name
 
     def upsert(
         self,
```

### Comparing `spetlr-1.1.84/src/spetlr/eh/EventHubCapture.py` & `spetlr-1.1.86/src/spetlr/eh/EventHubCapture.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/eh/EventHubCaptureExtractor.py` & `spetlr-1.1.86/src/spetlr/eh/EventHubCaptureExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/eh/EventHubJsonPublisher.py` & `spetlr-1.1.86/src/spetlr/eh/EventHubJsonPublisher.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/eh/EventHubStream.py` & `spetlr-1.1.86/src/spetlr/eh/EventHubStream.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/eh/PartitionSpec.py` & `spetlr-1.1.86/src/spetlr/eh/PartitionSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/entry_points/generalized_task_entry_point.py` & `spetlr-1.1.86/src/spetlr/entry_points/generalized_task_entry_point.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/entry_points/task_entry_point.py` & `spetlr-1.1.86/src/spetlr/entry_points/task_entry_point.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/etl/extractor.py` & `spetlr-1.1.86/src/spetlr/etl/extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/etl/extractors/incremental_extractor.py` & `spetlr-1.1.86/src/spetlr/etl/extractors/incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/etl/extractors/schema_extractor.py` & `spetlr-1.1.86/src/spetlr/etl/extractors/schema_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/etl/loader.py` & `spetlr-1.1.86/src/spetlr/etl/loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/etl/loaders/DeleteDataLoader.py` & `spetlr-1.1.86/src/spetlr/etl/loaders/DeleteDataLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/etl/loaders/UpsertLoader.py` & `spetlr-1.1.86/src/spetlr/etl/loaders/UpsertLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/etl/loaders/simple_loader.py` & `spetlr-1.1.86/src/spetlr/etl/loaders/simple_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/etl/orchestrator.py` & `spetlr-1.1.86/src/spetlr/etl/orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/etl/transformer.py` & `spetlr-1.1.86/src/spetlr/etl/transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/etl/transformer_nc.py` & `spetlr-1.1.86/src/spetlr/etl/transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/exceptions/__init__.py` & `spetlr-1.1.86/src/spetlr/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/extractors/eventhub_stream_extractor.py` & `spetlr-1.1.86/src/spetlr/extractors/eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/formatting/git_hooks.py` & `spetlr-1.1.86/src/spetlr/formatting/git_hooks.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/functions.py` & `spetlr-1.1.86/src/spetlr/functions.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/mount/main.py` & `spetlr-1.1.86/src/spetlr/mount/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py` & `spetlr-1.1.86/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py` & `spetlr-1.1.86/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py` & `spetlr-1.1.86/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py` & `spetlr-1.1.86/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py` & `spetlr-1.1.86/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py` & `spetlr-1.1.86/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/reporting/JobReflection.py` & `spetlr-1.1.86/src/spetlr/reporting/JobReflection.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/reporting/SlackNotifier.py` & `spetlr-1.1.86/src/spetlr/reporting/SlackNotifier.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/schema_manager/schema_manager.py` & `spetlr-1.1.86/src/spetlr/schema_manager/schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/schema_manager/spark_schema.py` & `spetlr-1.1.86/src/spetlr/schema_manager/spark_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/spark.py` & `spetlr-1.1.86/src/spetlr/spark.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,7 +67,8 @@
         return cls._spark
 
     @classmethod
     def version(cls) -> Tuple:
         return tuple(int(p) for p in cls.get().version.split("."))
 
     DATABRICKS_RUNTIME_9_1 = (3, 1, 2)
+    DATABRICKS_RUNTIME_11_3 = (3, 3, 0)
```

### Comparing `spetlr-1.1.84/src/spetlr/sql/CommonBaseServer.py` & `spetlr-1.1.86/src/spetlr/sql/CommonBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/sql/SqlBaseServer.py` & `spetlr-1.1.86/src/spetlr/sql/SqlBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/sql/SqlExecutor.py` & `spetlr-1.1.86/src/spetlr/sql/SqlExecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/sql/SqlServer.py` & `spetlr-1.1.86/src/spetlr/sql/SqlServer.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,64 +30,108 @@
         spnpassword: str = None,
         options: SqlServerBaseOptions = None,
     ):
         """Create object to interact with sql servers. Pass all but
         connection_string to connect via values or pass only the
         connection_string as a keyword param to connect via connection string"""
         self.options = options or SqlServerBaseOptions()
+        self._use_builtin_driver = Spark.version() >= Spark.DATABRICKS_RUNTIME_11_3
 
         if connection_string is not None:
             hostname, port, username, password, database = self.from_connection_string(
                 connection_string
             )
-        if not (hostname and database and port):
+        self.hostname = hostname
+        self.username = username
+        self.password = password
+        self.database = database
+        self.port = port
+        self.spnid = spnid
+        self.spnpassword = spnpassword
+
+        if not (self.hostname and self.database and self.port):
             raise ValueError("Hostname or database parameters missing.")
 
+        self._vaidate_auth_usage()
+
         self.timeout = 180  # 180 sec due to serverless
         self.sleep_time = 5  # Every 5 seconds the connection tries to be established
 
         self.url = (
-            f"jdbc:sqlserver://{hostname}:{port};"
-            f"database={database};"
+            f"jdbc:sqlserver://{self.hostname}:{self.port};"
+            f"database={self.database};"
             f"queryTimeout=0;"
             f"loginTimeout={self.timeout};"
             f"driver={self.options.jdbc_driver};"
         )
 
-        if spnpassword and spnid and not password and not username:
+        if self._use_spn():
             # Use spn
             self.url += (
-                f"AADSecurePrincipalId={spnid};"
-                f"AADSecurePrincipalSecret={spnpassword};"
+                f"AADSecurePrincipalId={self.spnid};"
+                f"AADSecurePrincipalSecret={self.spnpassword};"
                 f"encrypt=true;"
                 f"trustServerCertificate=false;"
                 f"hostNameInCertificate=*.database.windows.net;"
                 f"authentication=ActiveDirectoryServicePrincipal"
             )
-
-        elif password and username and not spnpassword and not spnid:
+        else:
             # Use SQL admin
             self.url += f"user={username};password={password}"
-        else:
-            raise ValueError("Use either SPN or SQL user - never both")
 
         self.odbc = (
             f"DRIVER={{{self.options.pyodbc_driver}}};"
             f"SERVER={hostname};"
             f"DATABASE={database};"
             f"PORT={port};"
             f"UID={username or spnid};"
             f"PWD={password or spnpassword};"
             f"Connection Timeout={self.timeout}"
         )
 
         # If it is a SPN user, then it should use AD SPN authentication
-        if spnid:
+        if self._use_spn():
             self.odbc += ";Authentication=ActiveDirectoryServicePrincipal"
 
+    def _vaidate_auth_usage(self):
+        usage = (
+            bool(self.spnpassword),
+            bool(self.spnid),
+            bool(self.password),
+            bool(self.username),
+        )
+        if not any(usage):
+            raise ValueError("No auth information supplied")
+        if usage not in [(True, True, False, False), (False, False, True, True)]:
+            raise ValueError("Use either SPN or SQL user - never both")
+
+    def _use_spn(self):
+        return bool(self.spnid)
+
+    def _add_sqlserver_auth(self, writer_or_reader):
+        """should only be used in connectiuon with .format("sqlserver")"""
+        writer_or_reader = (
+            writer_or_reader.option("host", self.hostname)
+            .option("port", self.port)
+            .option("database", self.database)
+        )
+        if self._use_spn():
+            return (
+                writer_or_reader.option("AADSecurePrincipalId", self.spnid)
+                .option("AADSecurePrincipalSecret", self.spnpassword)
+                .option("encrypt", "true")
+                .option("trustServerCertificate", "false")
+                .option("hostNameInCertificate", "*.database.windows.net")
+                .option("authentication", "ActiveDirectoryServicePrincipal")
+            )
+        else:
+            return writer_or_reader.option("user", self.username).option(
+                "password", self.password
+            )
+
     @staticmethod
     def from_connection_string(connection_string):
         """Extracts values for connection to sql server, as described in:
         https://docs.microsoft.com/en-us/dotnet/api/system.data.sqlclient.sqlconnection.connectionstring?view=dotnet-plat-ext-6.0#remarks
         """
         try:
             server_pattern = (
@@ -140,46 +184,55 @@
         self.execute_sql(sql)
 
     def load_sql(self, sql: str):
         self.test_odbc_connection()
         return Spark.get().read.jdbc(url=self.url, table=sql)
 
     def read_table_by_name(self, table_name: str):
-        return self.load_sql(f"(SELECT * FROM {table_name}) target")
+        if self._use_builtin_driver:
+            return self._add_sqlserver_auth(
+                Spark.get().read.format("sqlserver").option("dbtable", table_name)
+            ).load()
+        else:
+            return self.load_sql(f"(SELECT * FROM {table_name}) target")
 
     def write_table_by_name(
         self,
         df_source: DataFrame,
         table_name: str,
         append: bool = False,
         big_data_set: bool = True,
         batch_size: int = 10 * 1024,
         partition_count: int = 60,
     ):
         self.test_odbc_connection()
 
-        df_source.repartition(partition_count).write.format(
-            "com.microsoft.sqlserver.jdbc.spark" if big_data_set else "jdbc"
-        ).mode("append" if append else "overwrite").option(
-            "schemaCheckEnabled", False
-        ).option(
-            # https://learn.microsoft.com/en-us/sql/connect/spark/connector?view=sql-server-ver16#supported-options
-            # https://github.com/microsoft/sql-spark-connector/blob/master/README.md
-            # Implements an insert with TABLOCK option to improve write performance
-            "tableLock",
-            True,
-        ).option(
-            "batchSize", batch_size
-        ).option(
-            "truncate", not append
-        ).option(
-            "url", self.url
-        ).option(
-            "dbtable", table_name
-        ).save()
+        writer = df_source.repartition(partition_count).write
+        if self._use_builtin_driver:
+            writer = self._add_sqlserver_auth(writer.format("sqlserver"))
+        else:
+            writer = writer.format(
+                "com.microsoft.sqlserver.jdbc.spark" if big_data_set else "jdbc"
+            ).option("url", self.url)
+
+        (
+            writer.mode("append" if append else "overwrite")
+            .option("schemaCheckEnabled", False)
+            .option(
+                # https://learn.microsoft.com/en-us/sql/connect/spark/connector?view=sql-server-ver16#supported-options
+                # https://github.com/microsoft/sql-spark-connector/blob/master/README.md
+                # Implements an insert with TABLOCK option to improve write performance
+                "tableLock",
+                True,
+            )
+            .option("batchSize", batch_size)
+            .option("truncate", not append)
+            .option("dbtable", table_name)
+            .save()
+        )
 
     def upsert_to_table_by_name(
         self,
         df_source: DataFrame,
         table_name: str,
         join_cols: List[str],
         filter_join_cols: bool = True,
```

### Comparing `spetlr-1.1.84/src/spetlr/sql/sql_handle.py` & `spetlr-1.1.86/src/spetlr/sql/sql_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/tables/TableHandle.py` & `spetlr-1.1.86/src/spetlr/tables/TableHandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformations.py` & `spetlr-1.1.86/src/spetlr/transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformers/__init__.py` & `spetlr-1.1.86/src/spetlr/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformers/dropColumnsTransformer_nc.py` & `spetlr-1.1.86/src/spetlr/transformers/dropColumnsTransformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformers/drop_oldest_duplicate_transformer.py` & `spetlr-1.1.86/src/spetlr/transformers/drop_oldest_duplicate_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformers/fuzzy_select.py` & `spetlr-1.1.86/src/spetlr/transformers/fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformers/join_dataframes_transformer.py` & `spetlr-1.1.86/src/spetlr/transformers/join_dataframes_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformers/selectColumnsTransformer_nc.py` & `spetlr-1.1.86/src/spetlr/transformers/selectColumnsTransformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py` & `spetlr-1.1.86/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformers/simple_dataframe_filter_transformer.py` & `spetlr-1.1.86/src/spetlr/transformers/simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformers/simple_sql_transformer.py` & `spetlr-1.1.86/src/spetlr/transformers/simple_sql_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformers/timezone_transformer_nc.py` & `spetlr-1.1.86/src/spetlr/transformers/timezone_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformers/union_transformer.py` & `spetlr-1.1.86/src/spetlr/transformers/union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformers/union_transformer_nc.py` & `spetlr-1.1.86/src/spetlr/transformers/union_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/transformers/validfromto_transformer.py` & `spetlr-1.1.86/src/spetlr/transformers/validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/utils/CheckDfMerge.py` & `spetlr-1.1.86/src/spetlr/utils/CheckDfMerge.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/utils/DataframeCreator.py` & `spetlr-1.1.86/src/spetlr/utils/DataframeCreator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/utils/DropOldestDuplicates.py` & `spetlr-1.1.86/src/spetlr/utils/DropOldestDuplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/utils/GetMergeStatement.py` & `spetlr-1.1.86/src/spetlr/utils/GetMergeStatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/utils/MockLoader.py` & `spetlr-1.1.86/src/spetlr/utils/MockLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr/utils/SelectAndCastColumns.py` & `spetlr-1.1.86/src/spetlr/utils/SelectAndCastColumns.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/src/spetlr.egg-info/PKG-INFO` & `spetlr-1.1.86/src/spetlr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spetlr
-Version: 1.1.84
+Version: 1.1.86
 Summary: A python SPark ETL libRary (SPETLR) for Databricks.
 Home-page: https://github.com/atc-net/atc-dataplatform
 Author: Spetlr.Org
 Author-email: spetlr.org@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/spetlr-org/spetlr
 Project-URL: Bug Reports, https://github.com/spetlr-org/spetlr/issues
```

### Comparing `spetlr-1.1.84/src/spetlr.egg-info/SOURCES.txt` & `spetlr-1.1.86/src/spetlr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/cache/test_cache.py` & `spetlr-1.1.86/tests/cluster/cache/test_cache.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/cosmos/test_cosmos.py` & `spetlr-1.1.86/tests/cluster/cosmos/test_cosmos.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/delta/test_delta_class.py` & `spetlr-1.1.86/tests/cluster/delta/test_delta_class.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/eh/test_eh_json_orchestrator.py` & `spetlr-1.1.86/tests/cluster/eh/test_eh_json_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/eh/test_eh_json_transformer.py` & `spetlr-1.1.86/tests/cluster/eh/test_eh_json_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/eh/test_eh_saving.py` & `spetlr-1.1.86/tests/cluster/eh/test_eh_saving.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/etl/test_delete_data_loader.py` & `spetlr-1.1.86/tests/cluster/etl/test_delete_data_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/etl/test_deltaupsert.py` & `spetlr-1.1.86/tests/cluster/etl/test_deltaupsert.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/etl/test_extractor.py` & `spetlr-1.1.86/tests/cluster/etl/test_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/etl/test_incremental_extractor.py` & `spetlr-1.1.86/tests/cluster/etl/test_incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/etl/test_loader.py` & `spetlr-1.1.86/tests/cluster/etl/test_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/etl/test_orchestrator_etl_warning.py` & `spetlr-1.1.86/tests/cluster/etl/test_orchestrator_etl_warning.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/etl/test_transformer.py` & `spetlr-1.1.86/tests/cluster/etl/test_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/etl/test_transformer_nc.py` & `spetlr-1.1.86/tests/cluster/etl/test_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/etl/test_upsertloader.py` & `spetlr-1.1.86/tests/cluster/etl/test_upsertloader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/reporting/test_slack_reporting.py` & `spetlr-1.1.86/tests/cluster/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/schema_manager/test_schema_manager.py` & `spetlr-1.1.86/tests/cluster/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/sql/test_deliveryexecutor.py` & `spetlr-1.1.86/tests/cluster/sql/test_deliveryexecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/sql/test_deliverysql.py` & `spetlr-1.1.86/tests/cluster/sql/test_deliverysql.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/sql/test_simple_sql_etl.py` & `spetlr-1.1.86/tests/cluster/sql/test_simple_sql_etl.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/sql/test_sqlhandle.py` & `spetlr-1.1.86/tests/cluster/sql/test_sqlhandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/transformations/test_merge_df_into_target.py` & `spetlr-1.1.86/tests/cluster/transformations/test_merge_df_into_target.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/cluster/transformations/test_union_transformer.py` & `spetlr-1.1.86/tests/cluster/transformations/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/configurator/test_configurator.py` & `spetlr-1.1.86/tests/local/configurator/test_configurator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/configurator/test_configurator_cli.py` & `spetlr-1.1.86/tests/local/configurator/test_configurator_cli.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/eh/test_EventHubCaptureExtractor.py` & `spetlr-1.1.86/tests/local/eh/test_EventHubCaptureExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/eh/test_ehto_bronze_and_silver.py` & `spetlr-1.1.86/tests/local/eh/test_ehto_bronze_and_silver.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/eh/test_ehtodeltabronze_orchestrator.py` & `spetlr-1.1.86/tests/local/eh/test_ehtodeltabronze_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/eh/test_ehtodeltabronze_transformer.py` & `spetlr-1.1.86/tests/local/eh/test_ehtodeltabronze_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/eh/test_ehtodeltasilver_orchestrator.py` & `spetlr-1.1.86/tests/local/eh/test_ehtodeltasilver_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/extractors/test_eventhub_stream_extractor.py` & `spetlr-1.1.86/tests/local/extractors/test_eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/reporting/test_slack_reporting.py` & `spetlr-1.1.86/tests/local/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/schema_manager/test_schema_manager.py` & `spetlr-1.1.86/tests/local/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/sql/test_SqlExecutor.py` & `spetlr-1.1.86/tests/local/sql/test_SqlExecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/test_functions.py` & `spetlr-1.1.86/tests/local/test_functions.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/test_get_schema.py` & `spetlr-1.1.86/tests/local/test_get_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/test_sqlServer.py` & `spetlr-1.1.86/tests/local/test_sqlServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/test_transformations.py` & `spetlr-1.1.86/tests/local/test_transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/transformers/test_concat_df.py` & `spetlr-1.1.86/tests/local/transformers/test_concat_df.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/transformers/test_drop_columns.py` & `spetlr-1.1.86/tests/local/transformers/test_drop_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/transformers/test_dropoldestduplicates.py` & `spetlr-1.1.86/tests/local/transformers/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/transformers/test_fuzzy_select.py` & `spetlr-1.1.86/tests/local/transformers/test_fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/transformers/test_join_dataframes_transformer.py` & `spetlr-1.1.86/tests/local/transformers/test_join_dataframes_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py` & `spetlr-1.1.86/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/transformers/test_select_columns.py` & `spetlr-1.1.86/tests/local/transformers/test_select_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/transformers/test_simple_dataframe_filter_transformer.py` & `spetlr-1.1.86/tests/local/transformers/test_simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/transformers/test_timezone_transformer_nc.py` & `spetlr-1.1.86/tests/local/transformers/test_timezone_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/transformers/test_union_transformer.py` & `spetlr-1.1.86/tests/local/transformers/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/transformers/test_union_transformer_nc.py` & `spetlr-1.1.86/tests/local/transformers/test_union_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/transformers/test_validfromto_transformer.py` & `spetlr-1.1.86/tests/local/transformers/test_validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/utils/test_dataframe_creation.py` & `spetlr-1.1.86/tests/local/utils/test_dataframe_creation.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/utils/test_dropoldestduplicates.py` & `spetlr-1.1.86/tests/local/utils/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/utils/test_getmergestatement.py` & `spetlr-1.1.86/tests/local/utils/test_getmergestatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/utils/test_mock_etl.py` & `spetlr-1.1.86/tests/local/utils/test_mock_etl.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.84/tests/local/utils/test_selectandcastcolumns.py` & `spetlr-1.1.86/tests/local/utils/test_selectandcastcolumns.py`

 * *Files identical despite different names*

