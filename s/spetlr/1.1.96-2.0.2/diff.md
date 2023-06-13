# Comparing `tmp/spetlr-1.1.96.tar.gz` & `tmp/spetlr-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spetlr-1.1.96.tar", last modified: Tue Jun  6 12:50:51 2023, max compression
+gzip compressed data, was "spetlr-2.0.2.tar", last modified: Tue Jun 13 07:37:29 2023, max compression
```

## Comparing `spetlr-1.1.96.tar` & `spetlr-2.0.2.tar`

### file list

```diff
@@ -1,257 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.475601 spetlr-1.1.96/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-06 12:50:39.000000 spetlr-1.1.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-06 12:50:39.000000 spetlr-1.1.96/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-06 12:50:51.475601 spetlr-1.1.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-06 12:50:39.000000 spetlr-1.1.96/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-06 12:50:39.000000 spetlr-1.1.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-06 12:50:51.475601 spetlr-1.1.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:50:39.000000 spetlr-1.1.96/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.451600 spetlr-1.1.96/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.455601 spetlr-1.1.96/src/spetlr/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/alias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.455601 spetlr-1.1.96/src/spetlr/cache/
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/cache/CachedLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/cache/CachedLoaderParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.455601 spetlr-1.1.96/src/spetlr/config_master/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/config_master/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.455601 spetlr-1.1.96/src/spetlr/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.455601 spetlr-1.1.96/src/spetlr/configurator/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/_cli/generate_keys_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    15383 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.455601 spetlr-1.1.96/src/spetlr/configurator/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/sql/StatementBlocks.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/sql/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/sql/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/sql/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/sql/init_sqlparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/sql/parse_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/sql/substructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/sql/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/configurator/sql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.455601 spetlr-1.1.96/src/spetlr/cosmos/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/cosmos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/cosmos/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/cosmos/cosmos_base_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/cosmos/cosmos_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/db_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.455601 spetlr-1.1.96/src/spetlr/delta/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/delta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/delta/db_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/delta/delta_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.459601 spetlr-1.1.96/src/spetlr/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/eh/EventHubCapture.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/eh/EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/eh/EventHubJsonPublisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/eh/EventHubStream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/eh/PartitionSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/eh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/eh/eh_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.459601 spetlr-1.1.96/src/spetlr/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/entry_points/generalized_task_entry_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/entry_points/task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.459601 spetlr-1.1.96/src/spetlr/etl/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.459601 spetlr-1.1.96/src/spetlr/etl/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/extractors/incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/extractors/schema_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/extractors/simple_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.459601 spetlr-1.1.96/src/spetlr/etl/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/loaders/DeleteDataLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/loaders/UpsertLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/loaders/simple_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/loaders/simple_sql_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/etl/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.459601 spetlr-1.1.96/src/spetlr/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/exceptions/cli_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/exceptions/configurator_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.459601 spetlr-1.1.96/src/spetlr/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/extractors/eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.459601 spetlr-1.1.96/src/spetlr/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/formatting/git_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.459601 spetlr-1.1.96/src/spetlr/mount/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/mount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/mount/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.459601 spetlr-1.1.96/src/spetlr/orchestrators/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/orchestrators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.459601 spetlr-1.1.96/src/spetlr/orchestrators/eh2bronze/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/orchestrators/eh2bronze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.459601 spetlr-1.1.96/src/spetlr/orchestrators/eh2silver/
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/orchestrators/eh2silver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.463601 spetlr-1.1.96/src/spetlr/orchestrators/ehjson2delta/
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/orchestrators/ehjson2delta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.463601 spetlr-1.1.96/src/spetlr/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/reporting/JobReflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/reporting/SlackNotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.463601 spetlr-1.1.96/src/spetlr/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/schema_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/schema_manager/schema_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/schema_manager/spark_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.463601 spetlr-1.1.96/src/spetlr/singleton/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/singleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/singleton/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/spark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.467601 spetlr-1.1.96/src/spetlr/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/sql/BaseExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/sql/CommonBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/sql/SqlBaseServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/sql/SqlExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/sql/SqlServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/sql/SqlServerBaseOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/sql/sql_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.467601 spetlr-1.1.96/src/spetlr/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/tables/TableHandle.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/tables/ThMaker.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.467601 spetlr-1.1.96/src/spetlr/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/country_to_alphacode_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/dropColumnsTransformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/drop_oldest_duplicate_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/generate_md5_column_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/selectColumnsTransformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/simple_sql_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/timezone_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/union_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/transformers/validfromto_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.467601 spetlr-1.1.96/src/spetlr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/utils/CheckDfMerge.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/utils/CleanupTestDatabases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/utils/DataframeCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/utils/DropOldestDuplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/utils/GetMergeStatement.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/utils/MockExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/utils/MockLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/utils/SelectAndCastColumns.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-06 12:50:39.000000 spetlr-1.1.96/src/spetlr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.455601 spetlr-1.1.96/src/spetlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-06 12:50:51.000000 spetlr-1.1.96/src/spetlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-06-06 12:50:51.000000 spetlr-1.1.96/src/spetlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:50:51.000000 spetlr-1.1.96/src/spetlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 12:50:51.000000 spetlr-1.1.96/src/spetlr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:50:51.000000 spetlr-1.1.96/src/spetlr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-06 12:50:51.000000 spetlr-1.1.96/src/spetlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 12:50:51.000000 spetlr-1.1.96/src/spetlr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.451600 spetlr-1.1.96/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.451600 spetlr-1.1.96/tests/cluster/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.467601 spetlr-1.1.96/tests/cluster/cache/
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/cache/test_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.467601 spetlr-1.1.96/tests/cluster/cosmos/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/cosmos/test_cosmos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.467601 spetlr-1.1.96/tests/cluster/db/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/db/test_db_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.471601 spetlr-1.1.96/tests/cluster/delta/
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/delta/test_cleanup_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/delta/test_delta_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/delta/test_sparkexecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.471601 spetlr-1.1.96/tests/cluster/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/eh/test_eh_json_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/eh/test_eh_json_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/eh/test_eh_saving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.471601 spetlr-1.1.96/tests/cluster/etl/
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/etl/test_delete_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/etl/test_deltaupsert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/etl/test_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/etl/test_incremental_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/etl/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/etl/test_orchestrator_etl_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/etl/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/etl/test_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/etl/test_upsertloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.471601 spetlr-1.1.96/tests/cluster/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.471601 spetlr-1.1.96/tests/cluster/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.471601 spetlr-1.1.96/tests/cluster/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/sql/test_deliveryexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/sql/test_deliverysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/sql/test_deliverysqlspn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/sql/test_simple_sql_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/sql/test_sqlhandle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.471601 spetlr-1.1.96/tests/cluster/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/transformations/test_merge_df_into_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/cluster/transformations/test_union_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.471601 spetlr-1.1.96/tests/local/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.471601 spetlr-1.1.96/tests/local/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/configurator/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/configurator/test_configurator_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.471601 spetlr-1.1.96/tests/local/eh/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/eh/test_EventHubCaptureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/eh/test_ehto_bronze_and_silver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/eh/test_ehtodeltabronze_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/eh/test_ehtodeltabronze_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/eh/test_ehtodeltasilver_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.471601 spetlr-1.1.96/tests/local/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/entry_points/test_task_entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.471601 spetlr-1.1.96/tests/local/etl/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/etl/test_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.475601 spetlr-1.1.96/tests/local/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/extractors/test_eventhub_stream_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.475601 spetlr-1.1.96/tests/local/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/reporting/test_slack_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.475601 spetlr-1.1.96/tests/local/schema_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/schema_manager/test_schema_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.475601 spetlr-1.1.96/tests/local/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/sql/test_SqlExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/test_get_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/test_spark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/test_sqlServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/test_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.475601 spetlr-1.1.96/tests/local/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_concat_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_country_to_alphacode_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_fuzzy_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_generate_md5_column_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_join_dataframes_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_select_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_simple_dataframe_filter_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_timezone_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_union_transformer_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/transformers/test_validfromto_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:50:51.475601 spetlr-1.1.96/tests/local/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/utils/test_cleandatabases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/utils/test_dataframe_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/utils/test_dropoldestduplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/utils/test_getmergestatement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/utils/test_mock_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-06 12:50:39.000000 spetlr-1.1.96/tests/local/utils/test_selectandcastcolumns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.394148 spetlr-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-13 07:37:15.000000 spetlr-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-13 07:37:15.000000 spetlr-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-13 07:37:29.394148 spetlr-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-13 07:37:15.000000 spetlr-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 07:37:15.000000 spetlr-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-13 07:37:29.394148 spetlr-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:37:15.000000 spetlr-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.374148 spetlr-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/alias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cache/CachedLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cache/CachedLoaderParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/config_master/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/config_master/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/configurator/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/_cli/ConfiguratorCli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/_cli/generate_keys_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/configurator/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/StatementBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/init_sqlparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/parse_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/substructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/configurator/sql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cosmos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cosmos/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cosmos/cosmos_base_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/cosmos/cosmos_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/db_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/delta/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/delta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/delta/db_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/delta/delta_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/EventHubCapture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/EventHubJsonPublisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/EventHubStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/PartitionSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/eh/eh_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/entry_points/generalized_task_entry_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/entry_points/task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/etl/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/extractors/incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/extractors/schema_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/extractors/simple_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/etl/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/loaders/DeleteDataLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/loaders/UpsertLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/loaders/simple_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/loaders/simple_sql_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/etl/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/exceptions/cli_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/exceptions/configurator_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/extractors/eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/formatting/git_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/mount/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/mount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/mount/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/orchestrators/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/orchestrators/eh2bronze/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/eh2bronze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/orchestrators/eh2silver/
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/eh2silver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/reporting/JobReflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/reporting/SlackNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.382148 spetlr-2.0.2/src/spetlr/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/schema_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/schema_manager/schema_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/schema_manager/spark_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/src/spetlr/singleton/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/singleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/singleton/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/spark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/src/spetlr/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/BaseExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/CommonBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/SqlBaseServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/SqlExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/SqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/SqlServerBaseOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/sql/sql_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/src/spetlr/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/tables/TableHandle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/tables/ThMaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/src/spetlr/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/country_to_alphacode_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/dropColumnsTransformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/drop_oldest_duplicate_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/generate_md5_column_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/selectColumnsTransformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/simple_sql_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/timezone_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/union_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/transformers/validfromto_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/src/spetlr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/CheckDfMerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/CleanupTestDatabases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/DataframeCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/DropOldestDuplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/GetMergeStatement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/MockExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/MockLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/SelectAndCastColumns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-13 07:37:15.000000 spetlr-2.0.2/src/spetlr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.378147 spetlr-2.0.2/src/spetlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 07:37:29.000000 spetlr-2.0.2/src/spetlr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.374148 spetlr-2.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.374148 spetlr-2.0.2/tests/cluster/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/tests/cluster/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/cache/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/tests/cluster/cosmos/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/cosmos/test_cosmos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/tests/cluster/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/db/test_db_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.386148 spetlr-2.0.2/tests/cluster/delta/
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/delta/test_cleanup_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/delta/test_delta_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/delta/test_sparkexecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/cluster/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/eh/test_eh_json_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/eh/test_eh_json_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/eh/test_eh_saving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/cluster/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_delete_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_deltaupsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_incremental_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_orchestrator_etl_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/etl/test_upsertloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/cluster/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/cluster/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/cluster/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/sql/test_deliveryexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/sql/test_deliverysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/sql/test_deliverysqlspn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/sql/test_simple_sql_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/sql/test_sqlhandle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/cluster/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/transformations/test_merge_df_into_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/cluster/transformations/test_union_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/configurator/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/configurator/test_configurator_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/eh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/eh/test_EventHubCaptureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/eh/test_ehto_bronze_and_silver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/eh/test_ehtodeltabronze_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/eh/test_ehtodeltabronze_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/eh/test_ehtodeltasilver_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/entry_points/test_task_entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/etl/test_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/extractors/test_eventhub_stream_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/reporting/test_slack_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/schema_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/schema_manager/test_schema_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.390148 spetlr-2.0.2/tests/local/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/sql/test_SqlExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/test_get_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/test_spark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/test_sqlServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/test_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.394148 spetlr-2.0.2/tests/local/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_concat_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_country_to_alphacode_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_fuzzy_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_generate_md5_column_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_join_dataframes_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_select_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_simple_dataframe_filter_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_timezone_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_union_transformer_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/transformers/test_validfromto_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:37:29.394148 spetlr-2.0.2/tests/local/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/utils/test_cleandatabases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/utils/test_dataframe_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/utils/test_dropoldestduplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/utils/test_getmergestatement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/utils/test_mock_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-13 07:37:15.000000 spetlr-2.0.2/tests/local/utils/test_selectandcastcolumns.py
```

### Comparing `spetlr-1.1.96/LICENSE` & `spetlr-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/setup.cfg` & `spetlr-2.0.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -31,20 +31,21 @@
 	=src
 packages = find:
 install_requires = 
 	pyyaml
 	sqlparse
 	Deprecated
 	pyodbc
-	databricks-api
 	importlib-metadata
 	azure-cosmos
 	timezonefinder==6.0.2
 	more_itertools
 	pycountry
+	databricks-sdk
+	urllib3==1.26.16
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	python3 = spetlr.alias:python3
```

### Comparing `spetlr-1.1.96/src/spetlr/cache/CachedLoader.py` & `spetlr-2.0.2/src/spetlr/cache/CachedLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/cache/CachedLoaderParameters.py` & `spetlr-2.0.2/src/spetlr/cache/CachedLoaderParameters.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/configurator/_cli/__init__.py` & `spetlr-2.0.2/src/spetlr/configurator/_cli/ConfiguratorCli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 import argparse
 
 from spetlr.exceptions.cli_exceptions import SpetlrCliException
 
 from . import generate_keys_file
 
 
-def cli(self):
-    """
-    This function exposes functionality to be used in code analysis and deployment.
-    Initialize the configurator in your project like
-
-    ```
-    def init_my_configurator():
-        c= Configurator()
-        c.add_resource_path(my_yaml_module)
-        c.register('ENV', config.my_env_name)
-        return c
-
-    def my_configurator_cli():
-        init_my_configurator().cli()
-    ```
-    Then expose the `my_configurator_cli` as a command line tool.
-    The cli has the following usage
-
-    <my_cli> [action [action_options]]
-
-    Available actions:
-
-    - generate-keys-file [-o output_file]
-        Generates a python file that contains every available key string as a python
-        object of the same name. Including this file in your python project allows
-        you to get auto-completion of key names.
-        The output is dumped to stdout unless -o output_file is specified.
-        The option -o has the side-effect of return an exit code 1 if the file was
-        updated. This allows you to check for a correctly updated keys file in your
-        CICD pipleine.
-    """
-    parser = argparse.ArgumentParser()
-    subp = parser.add_subparsers(help="actions")
-
-    generate_keys_file.setup_parser(subp.add_parser("generate-keys-file"))
-    # add further parsers here
-
-    options = parser.parse_args()
-
-    try:
-        func = options.func
-    except AttributeError:
-        parser.print_help()
-        raise SpetlrCliException("No actions given")
+class ConfiguratorCli:
+    """This base class encapsulates the cli functions of the configurator.
+    It is not intended to be instantiated directly."""
+
+    def cli(self):
+        """
+        This function exposes functionality to be used in code analysis and deployment.
+        Initialize the configurator in your project like
+
+        ```
+        def init_my_configurator():
+            c= Configurator()
+            c.add_resource_path(my_yaml_module)
+            c.register('ENV', config.my_env_name)
+            return c
+
+        def my_configurator_cli():
+            init_my_configurator().cli()
+        ```
+        Then expose the `my_configurator_cli` as a command line tool.
+        The cli has the following usage
+
+        <my_cli> [action [action_options]]
+
+        Available actions:
+
+        - generate-keys-file [-o output_file]
+            Generates a python file that contains every available key string as a python
+            object of the same name. Including this file in your python project allows
+            you to get auto-completion of key names.
+            The output is dumped to stdout unless -o output_file is specified.
+            The option -o has the side-effect of return an exit code 1 if the file was
+            updated. This allows you to check for a correctly updated keys file in your
+            CICD pipleine.
+        """
+        parser = argparse.ArgumentParser()
+        subp = parser.add_subparsers(help="actions")
+
+        generate_keys_file.setup_parser(subp.add_parser("generate-keys-file"))
+        # add further parsers here
+
+        options = parser.parse_args()
+
+        try:
+            func = options.func
+        except AttributeError:
+            parser.print_help()
+            raise SpetlrCliException("No actions given")
 
-    func(self, options)
+        func(options)
```

### Comparing `spetlr-1.1.96/src/spetlr/configurator/_cli/generate_keys_file.py` & `spetlr-2.0.2/src/spetlr/configurator/_cli/generate_keys_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,26 +13,28 @@
         dest="check",
         action="store_true",
         help="Only check, don't update the output file",
     )
     parser.set_defaults(check=False)
 
 
-def generate_keys_file(self, options):
+def generate_keys_file(options):
     """Generate a keys file from configured keys.
     The arguments are as follows:
-        - self refers to the configurator object
         - options is a SimpleNamespace, expected to contain these attributes
             - output_file - str - the name of the output file, if none given,
               the generate file contents are printed to the console
             - check True/False, don't generate the file, verify an existing one.
     """
+    from spetlr import Configurator  # prevent circular import
+
+    c = Configurator()
     new_conts = "\n".join(
         ["# AUTO GENERATED FILE", "# contains all spetlr.Configurator keys", ""]
-        + [f"{key} = {repr(key)}" for key in sorted(self.all_keys())]
+        + [f"{key} = {repr(key)}" for key in sorted(c.all_keys())]
     )
 
     # if black is installed, use it to format the contents
     try:
         import black
 
         new_conts = black.format_file_contents(
```

### Comparing `spetlr-1.1.96/src/spetlr/configurator/configurator.py` & `spetlr-2.0.2/src/spetlr/configurator/configurator.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 from string import Formatter
 from types import ModuleType
 from typing import Dict, Set, Union
 
 import yaml
 from deprecated import deprecated
 
+from spetlr.configurator._cli.ConfiguratorCli import ConfiguratorCli
 from spetlr.configurator.sql import _parse_sql_to_config
 from spetlr.exceptions import NoSuchValueException
+from spetlr.functions import json_hash
 
 # recursive type definition of the details object
 TcDetails = Dict[str, Union[str, "TcDetails"]]
 TcValue = Union[str, TcDetails]
 
 
 class ConfiguratorSingleton(type):
@@ -28,15 +30,15 @@
         if ConfiguratorSingleton._instance is None:
             ConfiguratorSingleton._instance = super(
                 ConfiguratorSingleton, cls
             ).__call__(*args, **kwargs)
         return ConfiguratorSingleton._instance
 
 
-class Configurator(metaclass=ConfiguratorSingleton):
+class Configurator(ConfiguratorCli, metaclass=ConfiguratorSingleton):
     _unique_id: str
     _raw_resource_details: TcDetails
     _is_debug: bool
 
     # this dict contains all details for all resources
     table_details: Dict[str, str]
 
@@ -250,14 +252,31 @@
             # if any exception raised by the above code is caught.
             self._raw_resource_details = backup_details
             raise
 
     def add_sql_resource_path(self, resource_path: Union[str, ModuleType]) -> None:
         self._raw_resource_details.update(_parse_sql_to_config(resource_path))
 
+    def key_of(self, attribute: str, value: str) -> str:
+        """Obtain the key of the first registered item that has a given attribute
+        set to a given value. Uniqueness of the match is the responsibility of
+        the library user.
+
+        This function is slow as it performs a linear search. It is intended for use in
+        setup code.
+        """
+        for key, object in self._raw_resource_details.items():
+            try:
+                if object[attribute] == value:
+                    return key
+            except (KeyError, TypeError):
+                continue
+        else:
+            raise KeyError(f"No key with attribute {attribute}={repr(value)}")
+
     ############################################
     # all methods below are interface and convenience methods
     ############################################
 
     @deprecated(
         reason="register literal string values instead.",
     )
@@ -298,20 +317,32 @@
     def get_unique_id_length(self):
         """
         Return the character length of the UUID identifier inserted into
         names with the {ID} tag
         """
         return len(self._unique_id)
 
-    def register(self, key: str, value: TcValue):
+    def register(self, key: str, value: TcValue) -> str:
         """
-        Register a new item.
+        Register a new item and return its key.
         """
         self._raw_resource_details[key] = value
         self.table_details = dict()
+        return key
+
+    def define(self, **kwargs) -> str:
+        """
+        Register a new item based on its properties only and return its key.
+        The returned key is a hash-like string depending only on the values.
+        """
+        if not kwargs:
+            raise ValueError("No value passed.")
+
+        key = json_hash(kwargs)
+        return self.register(key, kwargs)
 
     def table_property(
         self, table_id: str, property_name: str, default_value: str = None
     ):
         """
         Return the table property (e.g. name, path, format, etc.)
             for the specified table id.
@@ -395,9 +426,7 @@
                         self.table_details[f"{table_id}_{property_name}"] = str(item)
 
         return self.table_details
 
     def regenerate_unique_id_and_clear_conf(self):
         self._unique_id = uuid.uuid4().hex
         self.clear_all_configurations()
-
-    from ._cli import cli
```

### Comparing `spetlr-1.1.96/src/spetlr/configurator/sql/StatementBlocks.py` & `spetlr-2.0.2/src/spetlr/configurator/sql/StatementBlocks.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/configurator/sql/comments.py` & `spetlr-2.0.2/src/spetlr/configurator/sql/comments.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/configurator/sql/create.py` & `spetlr-2.0.2/src/spetlr/configurator/sql/create.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/configurator/sql/db.py` & `spetlr-2.0.2/src/spetlr/configurator/sql/db.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/configurator/sql/init_sqlparse.py` & `spetlr-2.0.2/src/spetlr/configurator/sql/init_sqlparse.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/configurator/sql/parse_sql.py` & `spetlr-2.0.2/src/spetlr/configurator/sql/parse_sql.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/configurator/sql/substructures.py` & `spetlr-2.0.2/src/spetlr/configurator/sql/substructures.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/configurator/sql/table.py` & `spetlr-2.0.2/src/spetlr/configurator/sql/table.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/cosmos/cosmos.py` & `spetlr-2.0.2/src/spetlr/cosmos/cosmos.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/cosmos/cosmos_base_server.py` & `spetlr-2.0.2/src/spetlr/cosmos/cosmos_base_server.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/cosmos/cosmos_handle.py` & `spetlr-2.0.2/src/spetlr/cosmos/cosmos_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/delta/db_handle.py` & `spetlr-2.0.2/src/spetlr/delta/db_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/delta/delta_handle.py` & `spetlr-2.0.2/src/spetlr/delta/delta_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/eh/EventHubCapture.py` & `spetlr-2.0.2/src/spetlr/eh/EventHubCapture.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/eh/EventHubCaptureExtractor.py` & `spetlr-2.0.2/src/spetlr/eh/EventHubCaptureExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/eh/EventHubJsonPublisher.py` & `spetlr-2.0.2/src/spetlr/eh/EventHubJsonPublisher.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/eh/EventHubStream.py` & `spetlr-2.0.2/src/spetlr/eh/EventHubStream.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/eh/PartitionSpec.py` & `spetlr-2.0.2/src/spetlr/eh/PartitionSpec.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/entry_points/generalized_task_entry_point.py` & `spetlr-2.0.2/src/spetlr/entry_points/generalized_task_entry_point.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/entry_points/task_entry_point.py` & `spetlr-2.0.2/src/spetlr/entry_points/task_entry_point.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/etl/extractor.py` & `spetlr-2.0.2/src/spetlr/etl/extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/etl/extractors/incremental_extractor.py` & `spetlr-2.0.2/src/spetlr/etl/extractors/incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/etl/extractors/schema_extractor.py` & `spetlr-2.0.2/src/spetlr/etl/extractors/schema_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/etl/loader.py` & `spetlr-2.0.2/src/spetlr/etl/loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/etl/loaders/DeleteDataLoader.py` & `spetlr-2.0.2/src/spetlr/etl/loaders/DeleteDataLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/etl/loaders/UpsertLoader.py` & `spetlr-2.0.2/src/spetlr/etl/loaders/UpsertLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/etl/loaders/simple_loader.py` & `spetlr-2.0.2/src/spetlr/etl/loaders/simple_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/etl/orchestrator.py` & `spetlr-2.0.2/src/spetlr/etl/orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/etl/transformer.py` & `spetlr-2.0.2/src/spetlr/etl/transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/etl/transformer_nc.py` & `spetlr-2.0.2/src/spetlr/etl/transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/exceptions/__init__.py` & `spetlr-2.0.2/src/spetlr/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/extractors/eventhub_stream_extractor.py` & `spetlr-2.0.2/src/spetlr/extractors/eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/formatting/git_hooks.py` & `spetlr-2.0.2/src/spetlr/formatting/git_hooks.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/functions.py` & `spetlr-2.0.2/src/spetlr/functions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 A collection of useful pyspark snippets.
 """
-
+import hashlib
+import json
 import uuid as _uuid
+from typing import Any
 
 from deprecated import deprecated
 from pyspark.sql.functions import udf
 from pyspark.sql.types import StringType
 
 from spetlr.exceptions import NoDbUtils, NoTableException
 from spetlr.spark import Spark
@@ -63,7 +65,36 @@
     Spark.get().sql(f"DROP TABLE IF EXISTS {DBDotTableName}")
 
 
 def get_unique_tempview_name() -> str:
     unique_id = _uuid.uuid4().hex
     temp_view_name = f"source_{unique_id}"
     return temp_view_name
+
+
+def json_hash(value: Any):
+    """
+    Generate a hash from the json representation of a simple type.
+
+    This function converts the input to a JSON string,
+    generates a SHA256 hash of that string, and returns the hex digest.
+    Note that the function sorts any dictionary keys before converting
+    to a string to ensure consistent output for the same dictionary
+    regardless of the original key order.
+
+    Args:
+        value: A simple type or dictionary of simple types (e.g. int, str).
+
+    Returns:
+        str: A string representation of the input object.
+
+    Raises:
+        TypeError: If the value cannot be serialized to JSON.
+    """
+    # Convert the dictionary to a JSON string and encode it to bytes
+    input_bytes = json.dumps(value, sort_keys=True).encode("utf-8")
+
+    # Generate a SHA256 hash of the input
+    hash_object = hashlib.sha256(input_bytes)
+
+    # Get the hexadecimal representation of the hash
+    return hash_object.hexdigest()
```

### Comparing `spetlr-1.1.96/src/spetlr/mount/main.py` & `spetlr-2.0.2/src/spetlr/mount/main.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py` & `spetlr-2.0.2/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py` & `spetlr-2.0.2/src/spetlr/orchestrators/eh2bronze/EhToDeltaBronzeTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py` & `spetlr-2.0.2/src/spetlr/orchestrators/eh2silver/EhToDeltaSilverOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py` & `spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py` & `spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaOrchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py` & `spetlr-2.0.2/src/spetlr/orchestrators/ehjson2delta/EhJsonToDeltaTransformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/reporting/JobReflection.py` & `spetlr-2.0.2/src/spetlr/reporting/JobReflection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from functools import lru_cache
 from typing import Dict
 
+from databricks.sdk.service.jobs import Run
 from requests import HTTPError
 
 from spetlr.db_auto import getDbApi
 from spetlr.exceptions import NoDbUtils, NoRunId
 from spetlr.functions import init_dbutils
 
 
@@ -26,30 +27,30 @@
                 .toJson()
             )
         except (AttributeError, NoDbUtils):
             raise NoRunId()
 
     @classmethod
     @lru_cache
-    def get_job_api_details(cls) -> Dict:
+    def get_job_api_details(cls) -> Run:
         run_id = cls.get_current_run_id()
         db_api = getDbApi()
 
         try:
             return db_api.jobs.get_run(run_id=run_id)
         except HTTPError:
             raise NoRunId("DbApi returned http error.")
 
     @classmethod
     def get_job_results_url(cls) -> str:
-        return cls.get_job_api_details()["run_page_url"]
+        return cls.get_job_api_details().run_page_url
 
     @classmethod
     def get_job_name(cls) -> str:
-        return cls.get_job_api_details()["run_name"]
+        return cls.get_job_api_details().run_name
 
     @classmethod
     @lru_cache
     def get_current_run_id(cls) -> int:
         details = cls.get_job_details()
         try:
             # the first part is set in a task orchestration job
```

### Comparing `spetlr-1.1.96/src/spetlr/reporting/SlackNotifier.py` & `spetlr-2.0.2/src/spetlr/reporting/SlackNotifier.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/schema_manager/schema_manager.py` & `spetlr-2.0.2/src/spetlr/schema_manager/schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/schema_manager/spark_schema.py` & `spetlr-2.0.2/src/spetlr/schema_manager/spark_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/spark.py` & `spetlr-2.0.2/src/spetlr/spark.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/sql/CommonBaseServer.py` & `spetlr-2.0.2/src/spetlr/sql/CommonBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/sql/SqlBaseServer.py` & `spetlr-2.0.2/src/spetlr/sql/SqlBaseServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/sql/SqlExecutor.py` & `spetlr-2.0.2/src/spetlr/sql/SqlExecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/sql/SqlServer.py` & `spetlr-2.0.2/src/spetlr/sql/SqlServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/sql/sql_handle.py` & `spetlr-2.0.2/src/spetlr/sql/sql_handle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/tables/TableHandle.py` & `spetlr-2.0.2/src/spetlr/tables/TableHandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformations.py` & `spetlr-2.0.2/src/spetlr/transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/__init__.py` & `spetlr-2.0.2/src/spetlr/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/country_to_alphacode_transformer_nc.py` & `spetlr-2.0.2/src/spetlr/transformers/country_to_alphacode_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/dropColumnsTransformer_nc.py` & `spetlr-2.0.2/src/spetlr/transformers/dropColumnsTransformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/drop_oldest_duplicate_transformer.py` & `spetlr-2.0.2/src/spetlr/transformers/drop_oldest_duplicate_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/fuzzy_select.py` & `spetlr-2.0.2/src/spetlr/transformers/fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/generate_md5_column_transformer_nc.py` & `spetlr-2.0.2/src/spetlr/transformers/generate_md5_column_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/join_dataframes_transformer.py` & `spetlr-2.0.2/src/spetlr/transformers/join_dataframes_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/selectColumnsTransformer_nc.py` & `spetlr-2.0.2/src/spetlr/transformers/selectColumnsTransformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py` & `spetlr-2.0.2/src/spetlr/transformers/select_and_cast_columns_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/simple_dataframe_filter_transformer.py` & `spetlr-2.0.2/src/spetlr/transformers/simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py` & `spetlr-2.0.2/src/spetlr/transformers/simple_dataframe_filter_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/simple_sql_transformer.py` & `spetlr-2.0.2/src/spetlr/transformers/simple_sql_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/timezone_transformer_nc.py` & `spetlr-2.0.2/src/spetlr/transformers/timezone_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/union_transformer.py` & `spetlr-2.0.2/src/spetlr/transformers/union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/union_transformer_nc.py` & `spetlr-2.0.2/src/spetlr/transformers/union_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/transformers/validfromto_transformer.py` & `spetlr-2.0.2/src/spetlr/transformers/validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/utils/CheckDfMerge.py` & `spetlr-2.0.2/src/spetlr/utils/CheckDfMerge.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/utils/CleanupTestDatabases.py` & `spetlr-2.0.2/src/spetlr/utils/CleanupTestDatabases.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/utils/DataframeCreator.py` & `spetlr-2.0.2/src/spetlr/utils/DataframeCreator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/utils/DropOldestDuplicates.py` & `spetlr-2.0.2/src/spetlr/utils/DropOldestDuplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/utils/GetMergeStatement.py` & `spetlr-2.0.2/src/spetlr/utils/GetMergeStatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/utils/MockLoader.py` & `spetlr-2.0.2/src/spetlr/utils/MockLoader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr/utils/SelectAndCastColumns.py` & `spetlr-2.0.2/src/spetlr/utils/SelectAndCastColumns.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/src/spetlr.egg-info/SOURCES.txt` & `spetlr-2.0.2/src/spetlr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 src/spetlr.egg-info/top_level.txt
 src/spetlr/cache/CachedLoader.py
 src/spetlr/cache/CachedLoaderParameters.py
 src/spetlr/cache/__init__.py
 src/spetlr/config_master/__init__.py
 src/spetlr/configurator/__init__.py
 src/spetlr/configurator/configurator.py
+src/spetlr/configurator/_cli/ConfiguratorCli.py
 src/spetlr/configurator/_cli/__init__.py
 src/spetlr/configurator/_cli/generate_keys_file.py
 src/spetlr/configurator/sql/StatementBlocks.py
 src/spetlr/configurator/sql/__init__.py
 src/spetlr/configurator/sql/comments.py
 src/spetlr/configurator/sql/create.py
 src/spetlr/configurator/sql/db.py
```

### Comparing `spetlr-1.1.96/tests/cluster/cache/test_cache.py` & `spetlr-2.0.2/tests/cluster/cache/test_cache.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/cosmos/test_cosmos.py` & `spetlr-2.0.2/tests/cluster/cosmos/test_cosmos.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/delta/test_cleanup_databases.py` & `spetlr-2.0.2/tests/cluster/delta/test_cleanup_databases.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/delta/test_delta_class.py` & `spetlr-2.0.2/tests/cluster/delta/test_delta_class.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/delta/test_sparkexecutor.py` & `spetlr-2.0.2/tests/cluster/delta/test_sparkexecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/eh/test_eh_json_orchestrator.py` & `spetlr-2.0.2/tests/cluster/eh/test_eh_json_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/eh/test_eh_json_transformer.py` & `spetlr-2.0.2/tests/cluster/eh/test_eh_json_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/eh/test_eh_saving.py` & `spetlr-2.0.2/tests/cluster/eh/test_eh_saving.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/etl/test_delete_data_loader.py` & `spetlr-2.0.2/tests/cluster/etl/test_delete_data_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/etl/test_deltaupsert.py` & `spetlr-2.0.2/tests/cluster/etl/test_deltaupsert.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/etl/test_extractor.py` & `spetlr-2.0.2/tests/cluster/etl/test_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/etl/test_incremental_extractor.py` & `spetlr-2.0.2/tests/cluster/etl/test_incremental_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/etl/test_loader.py` & `spetlr-2.0.2/tests/cluster/etl/test_loader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/etl/test_orchestrator_etl_warning.py` & `spetlr-2.0.2/tests/cluster/etl/test_orchestrator_etl_warning.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/etl/test_transformer.py` & `spetlr-2.0.2/tests/cluster/etl/test_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/etl/test_transformer_nc.py` & `spetlr-2.0.2/tests/cluster/etl/test_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/etl/test_upsertloader.py` & `spetlr-2.0.2/tests/cluster/etl/test_upsertloader.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/reporting/test_slack_reporting.py` & `spetlr-2.0.2/tests/cluster/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/schema_manager/test_schema_manager.py` & `spetlr-2.0.2/tests/cluster/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/sql/test_deliveryexecutor.py` & `spetlr-2.0.2/tests/cluster/sql/test_deliveryexecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/sql/test_deliverysql.py` & `spetlr-2.0.2/tests/cluster/sql/test_deliverysql.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/sql/test_simple_sql_etl.py` & `spetlr-2.0.2/tests/cluster/sql/test_simple_sql_etl.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/sql/test_sqlhandle.py` & `spetlr-2.0.2/tests/cluster/sql/test_sqlhandle.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/transformations/test_merge_df_into_target.py` & `spetlr-2.0.2/tests/cluster/transformations/test_merge_df_into_target.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/cluster/transformations/test_union_transformer.py` & `spetlr-2.0.2/tests/cluster/transformations/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/configurator/test_configurator.py` & `spetlr-2.0.2/tests/local/configurator/test_configurator.py`

 * *Files 8% similar despite different names*

```diff
@@ -200,7 +200,38 @@
 
         first_extension = c.get_all_details()["ID"]
         c.regenerate_unique_id_and_clear_conf()
         second_extension = c.get_all_details()["ID"]
 
         self.assertEqual(first_extension, "")
         self.assertEqual(second_extension, "")
+
+    def test_12_define_nameless(self):
+        """The value of the tableId may not be interesting.
+        When defined in this way, the `tbl` object can be
+        inspected with IntelliSense."""
+
+        c = Configurator()
+        c.clear_all_configurations()
+        c.set_prod()
+
+        tbl = c.define(name="MyDb.MyTable{ID}", path="/mnt/path/to{ID}/data")
+
+        self.assertEqual(c.get(tbl, "name"), "MyDb.MyTable")
+
+    def test_13_test_keyof(self):
+        """Test the ability to extract the key of an object for which only
+        the defined name is known."""
+        c = Configurator()
+        c.clear_all_configurations()
+
+        c.register("MySecretKey", {"name": "MyDb.MyTable{ID}", "path": "/mnt/to/data"})
+
+        key = c.key_of("name", "MyDb.MyTable{ID}")
+
+        self.assertEqual(key, "MySecretKey")
+
+        # key not captured
+        c.define(name="anotherName", path="/somewhere")
+        # recover  key
+        key = c.key_of("name", "anotherName")
+        self.assertEqual(c.get(key, "path"), "/somewhere")
```

### Comparing `spetlr-1.1.96/tests/local/configurator/test_configurator_cli.py` & `spetlr-2.0.2/tests/local/configurator/test_configurator_cli.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/eh/test_EventHubCaptureExtractor.py` & `spetlr-2.0.2/tests/local/eh/test_EventHubCaptureExtractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/eh/test_ehto_bronze_and_silver.py` & `spetlr-2.0.2/tests/local/eh/test_ehto_bronze_and_silver.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/eh/test_ehtodeltabronze_orchestrator.py` & `spetlr-2.0.2/tests/local/eh/test_ehtodeltabronze_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/eh/test_ehtodeltabronze_transformer.py` & `spetlr-2.0.2/tests/local/eh/test_ehtodeltabronze_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/eh/test_ehtodeltasilver_orchestrator.py` & `spetlr-2.0.2/tests/local/eh/test_ehtodeltasilver_orchestrator.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/extractors/test_eventhub_stream_extractor.py` & `spetlr-2.0.2/tests/local/extractors/test_eventhub_stream_extractor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/reporting/test_slack_reporting.py` & `spetlr-2.0.2/tests/local/reporting/test_slack_reporting.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/schema_manager/test_schema_manager.py` & `spetlr-2.0.2/tests/local/schema_manager/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/sql/test_SqlExecutor.py` & `spetlr-2.0.2/tests/local/sql/test_SqlExecutor.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/test_functions.py` & `spetlr-2.0.2/tests/local/test_functions.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/test_get_schema.py` & `spetlr-2.0.2/tests/local/test_get_schema.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/test_sqlServer.py` & `spetlr-2.0.2/tests/local/test_sqlServer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/test_transformations.py` & `spetlr-2.0.2/tests/local/test_transformations.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_concat_df.py` & `spetlr-2.0.2/tests/local/transformers/test_concat_df.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_country_to_alphacode_transformer.py` & `spetlr-2.0.2/tests/local/transformers/test_country_to_alphacode_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_drop_columns.py` & `spetlr-2.0.2/tests/local/transformers/test_drop_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_dropoldestduplicates.py` & `spetlr-2.0.2/tests/local/transformers/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_fuzzy_select.py` & `spetlr-2.0.2/tests/local/transformers/test_fuzzy_select.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_generate_md5_column_transformer_nc.py` & `spetlr-2.0.2/tests/local/transformers/test_generate_md5_column_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_join_dataframes_transformer.py` & `spetlr-2.0.2/tests/local/transformers/test_join_dataframes_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py` & `spetlr-2.0.2/tests/local/transformers/test_select_and_cast_columns_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_select_columns.py` & `spetlr-2.0.2/tests/local/transformers/test_select_columns.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_simple_dataframe_filter_transformer.py` & `spetlr-2.0.2/tests/local/transformers/test_simple_dataframe_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py` & `spetlr-2.0.2/tests/local/transformers/test_simple_dataframe_filter_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_timezone_transformer_nc.py` & `spetlr-2.0.2/tests/local/transformers/test_timezone_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_union_transformer.py` & `spetlr-2.0.2/tests/local/transformers/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_union_transformer_nc.py` & `spetlr-2.0.2/tests/local/transformers/test_union_transformer_nc.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/transformers/test_validfromto_transformer.py` & `spetlr-2.0.2/tests/local/transformers/test_validfromto_transformer.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/utils/test_dataframe_creation.py` & `spetlr-2.0.2/tests/local/utils/test_dataframe_creation.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/utils/test_dropoldestduplicates.py` & `spetlr-2.0.2/tests/local/utils/test_dropoldestduplicates.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/utils/test_getmergestatement.py` & `spetlr-2.0.2/tests/local/utils/test_getmergestatement.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/utils/test_mock_etl.py` & `spetlr-2.0.2/tests/local/utils/test_mock_etl.py`

 * *Files identical despite different names*

### Comparing `spetlr-1.1.96/tests/local/utils/test_selectandcastcolumns.py` & `spetlr-2.0.2/tests/local/utils/test_selectandcastcolumns.py`

 * *Files identical despite different names*

