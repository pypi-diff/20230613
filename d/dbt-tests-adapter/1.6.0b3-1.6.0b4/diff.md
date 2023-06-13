# Comparing `tmp/dbt-tests-adapter-1.6.0b3.tar.gz` & `tmp/dbt-tests-adapter-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-tests-adapter-1.6.0b3.tar", last modified: Thu Jun  8 20:55:15 2023, max compression
+gzip compressed data, was "dbt-tests-adapter-1.6.0b4.tar", last modified: Tue Jun 13 21:43:42 2023, max compression
```

## Comparing `dbt-tests-adapter-1.6.0b3.tar` & `dbt-tests-adapter-1.6.0b4.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.305822 dbt-tests-adapter-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-08 20:55:15.305822 dbt-tests-adapter-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.285822 dbt-tests-adapter-1.6.0b3/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.285822 dbt-tests-adapter-1.6.0b3/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.289821 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.289821 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/aliases/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/aliases/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/aliases/test_aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.289821 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/expected_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_adapter_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_docs_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_incremental.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_singular_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_snapshot_check_cols.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_snapshot_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_table_materialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_validate_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.289821 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/caching/
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/caching/test_caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.289821 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/column_types/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/column_types/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/column_types/test_column_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.289821 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/concurrency/
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/concurrency/test_concurrency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/constraints/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/constraints/test_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/dbt_debug/
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/dbt_debug/test_dbt_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/ephemeral/
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/ephemeral/test_ephemeral.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/base_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_incremental_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_invalid_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_model_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_seed_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_snapshot_grants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/test_model_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/test_run_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)    17492 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_unique_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/materialized_view/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/materialized_view/on_configuration_change.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/persist_docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/persist_docs/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/persist_docs/test_persist_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/python_model/test_python_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/python_model/test_spark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/query_comment/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/query_comment/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/query_comment/test_query_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/relations/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/relations/test_changing_relation_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.297822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/
--rw-r--r--   0 runner    (1001) docker     (123)    19865 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/test_copy_uppercase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/test_simple_copy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.297822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    78093 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/test_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/test_seed_type_override.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.297822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/test_snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.297822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/store_test_failures_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/store_test_failures_tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.305822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/base_array_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/base_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.305822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/base_data_type_macro.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_bigint.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_float.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_int.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_any_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_array_append.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_array_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_array_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_bool_or.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_cast_bool_to_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_date_trunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_dateadd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_datediff.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_equals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_escape_single_quotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_except.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_last_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_listagg.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_null_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_right.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_safe_cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_split_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_any_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_array_append.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_array_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_array_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_bool_or.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_cast_bool_to_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_current_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_date_trunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_dateadd.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_datediff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_equals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_escape_single_quotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_except.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_last_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_listagg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_null_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_right.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_safe_cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_split_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_timestamps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.305822 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-08 20:55:15.000000 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-06-08 20:55:15.000000 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:55:15.000000 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:55:15.000000 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 20:55:15.000000 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 20:55:15.000000 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:55:15.305822 dbt-tests-adapter-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.266134 dbt-tests-adapter-1.6.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-13 21:43:42.266134 dbt-tests-adapter-1.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.234134 dbt-tests-adapter-1.6.0b4/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.234134 dbt-tests-adapter-1.6.0b4/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.238134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.238134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/aliases/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/aliases/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/aliases/test_aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.242134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/expected_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_adapter_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_docs_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_singular_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_snapshot_check_cols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_snapshot_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_table_materialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_validate_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.242134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/caching/test_caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.242134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/column_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/column_types/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/column_types/test_column_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.242134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/concurrency/test_concurrency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.242134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/constraints/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17933 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/constraints/test_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.242134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/dbt_debug/
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/dbt_debug/test_dbt_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.242134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/ephemeral/
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/ephemeral/test_ephemeral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.242134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/grants/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/grants/base_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/grants/test_incremental_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/grants/test_invalid_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/grants/test_model_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/grants/test_seed_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/grants/test_snapshot_grants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.242134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/hooks/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/hooks/test_model_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/hooks/test_run_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.246134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/incremental/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/incremental/test_incremental_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17492 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/incremental/test_incremental_unique_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.246134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/materialized_view/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/materialized_view/on_configuration_change.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.246134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/persist_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/persist_docs/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/persist_docs/test_persist_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.246134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/python_model/test_python_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/python_model/test_spark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.246134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/query_comment/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/query_comment/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/query_comment/test_query_comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.246134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/relations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/relations/test_changing_relation_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.246134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_copy/
+-rw-r--r--   0 runner    (1001) docker     (123)    19865 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_copy/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_copy/test_copy_uppercase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_copy/test_simple_copy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.250134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_seed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_seed/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78093 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_seed/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_seed/test_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_seed/test_seed_type_override.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.250134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_snapshot/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_snapshot/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_snapshot/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_snapshot/test_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.250134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/store_test_failures_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/store_test_failures_tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.262134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/base_array_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/base_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.262134 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/base_data_type_macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_bigint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_any_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_array_append.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_array_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_array_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_bool_or.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_cast_bool_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_date_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_dateadd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_datediff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_equals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_escape_single_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_except.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_last_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_listagg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_null_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_safe_cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_split_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_string_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_any_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_array_append.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_array_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_array_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_bool_or.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_cast_bool_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_current_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_date_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_dateadd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_datediff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_equals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_escape_single_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_except.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_last_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_listagg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_null_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_safe_cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_split_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_string_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_timestamps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:43:42.266134 dbt-tests-adapter-1.6.0b4/dbt_tests_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-13 21:43:42.000000 dbt-tests-adapter-1.6.0b4/dbt_tests_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-06-13 21:43:42.000000 dbt-tests-adapter-1.6.0b4/dbt_tests_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:43:42.000000 dbt-tests-adapter-1.6.0b4/dbt_tests_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:43:42.000000 dbt-tests-adapter-1.6.0b4/dbt_tests_adapter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 21:43:42.000000 dbt-tests-adapter-1.6.0b4/dbt_tests_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 21:43:42.000000 dbt-tests-adapter-1.6.0b4/dbt_tests_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:43:42.266134 dbt-tests-adapter-1.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-13 21:43:22.000000 dbt-tests-adapter-1.6.0b4/setup.py
```

### Comparing `dbt-tests-adapter-1.6.0b3/PKG-INFO` & `dbt-tests-adapter-1.6.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-tests-adapter
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: The dbt adapter tests for adapter plugins
 Home-page: https://github.com/dbt-labs/dbt-core/tree/main/tests/adapter
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-tests-adapter-1.6.0b3/README.md` & `dbt-tests-adapter-1.6.0b4/README.md`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/aliases/fixtures.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/aliases/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/aliases/test_aliases.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/aliases/test_aliases.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/expected_catalog.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/expected_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/files.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/files.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_adapter_methods.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_adapter_methods.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_base.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_base.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_docs_generate.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_empty.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_empty.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_ephemeral.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_generic_tests.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_incremental.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_incremental.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_singular_tests.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_singular_tests.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_snapshot_check_cols.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_snapshot_check_cols.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_snapshot_timestamp.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_snapshot_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_table_materialization.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/basic/test_table_materialization.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/caching/test_caching.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/caching/test_caching.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/column_types/fixtures.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/column_types/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/column_types/test_column_types.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/column_types/test_column_types.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/concurrency/test_concurrency.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/concurrency/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/constraints/fixtures.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/constraints/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,24 +247,33 @@
   -- null value for 'id'
   cast(null as {{ dbt.type_int() }}) as id,
   -- change the color as well (to test rollback)
   'red' as color,
   '2019-01-01' as date_day
 """
 
+
+# 'from' is a reserved word, so it must be quoted
+my_model_with_quoted_column_name_sql = """
+select
+  'blue' as {{ adapter.quote('from') }},
+  1 as id,
+  '2019-01-01' as date_day
+"""
+
+
 model_schema_yml = """
 version: 2
 models:
   - name: my_model
     config:
       contract:
         enforced: true
     columns:
       - name: id
-        quote: true
         data_type: integer
         description: hello
         constraints:
           - type: not_null
           - type: primary_key
           - type: check
             expression: (id > 0)
@@ -340,15 +349,14 @@
 models:
   - name: my_model
     config:
       contract:
         enforced: true
     columns:
       - name: id
-        quote: true
         data_type: integer
         description: hello
         constraints:
           - type: not_null
           - type: primary_key
           - type: check
             expression: (id > 0)
@@ -450,15 +458,14 @@
         columns: [ color, date_day ]
         name: strange_uniqueness_requirement
       - type: foreign_key
         columns: [ id ]
         expression: {schema}.foreign_key_model (id)
     columns:
       - name: id
-        quote: true
         data_type: integer
         description: hello
         constraints:
           - type: not_null
         tests:
           - unique
       - name: color
@@ -486,14 +493,45 @@
       contract:
         enforced: true
     columns:
       - name: wrong_data_type_column_name
         data_type: {data_type}
 """
 
+
+model_quoted_column_schema_yml = """
+version: 2
+models:
+  - name: my_model
+    config:
+      contract:
+        enforced: true
+      materialized: table
+    constraints:
+      - type: check
+        # this one is the on the user
+        expression: ("from" = 'blue')
+        columns: [ '"from"' ]
+    columns:
+      - name: id
+        data_type: integer
+        description: hello
+        constraints:
+          - type: not_null
+        tests:
+          - unique
+      - name: from  # reserved word
+        quote: true
+        data_type: text
+        constraints:
+          - type: not_null
+      - name: date_day
+        data_type: text
+"""
+
 model_contract_header_schema_yml = """
 version: 2
 models:
   - name: my_model_contract_sql_header
     config:
       contract:
         enforced: true
```

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/constraints/test_constraints.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/constraints/test_constraints.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,19 @@
     model_data_type_schema_yml,
     my_model_view_wrong_order_sql,
     my_model_view_wrong_name_sql,
     my_model_incremental_wrong_order_sql,
     my_model_incremental_wrong_name_sql,
     my_model_with_nulls_sql,
     my_model_incremental_with_nulls_sql,
+    my_model_with_quoted_column_name_sql,
     model_schema_yml,
     model_fk_constraint_schema_yml,
     constrained_model_schema_yml,
+    model_quoted_column_schema_yml,
     foreign_key_model_sql,
     my_model_wrong_order_depends_on_fk_sql,
     my_model_incremental_wrong_order_depends_on_fk_sql,
     my_model_contract_sql_header_sql,
     my_model_incremental_contract_sql_header_sql,
     model_contract_header_schema_yml,
 )
@@ -161,19 +163,20 @@
             my_model_config = manifest.nodes[model_id].config
             contract_actual_config = my_model_config.contract
 
             assert contract_actual_config.enforced is True
 
 
 def _normalize_whitespace(input: str) -> str:
-    return re.sub(r"\s+", " ", input).lower().strip()
+    subbed = re.sub(r"\s+", " ", input)
+    return re.sub(r"\s?([\(\),])\s?", r"\1", subbed).lower().strip()
 
 
 def _find_and_replace(sql, find, replace):
-    sql_tokens = sql.split(" ")
+    sql_tokens = sql.split()
     for idx in [n for n, x in enumerate(sql_tokens) if find in x]:
         sql_tokens[idx] = replace
     return " ".join(sql_tokens)
 
 
 class BaseConstraintsRuntimeDdlEnforcement:
     """
@@ -231,25 +234,20 @@
         # assert at least my_model was run - additional upstreams may or may not be provided to the test setup via models fixture
         assert len(results) >= 1
 
         # grab the sql and replace the model identifier to make it generic for all adapters
         # the name is not what we're testing here anyways and varies based on materialization
         # TODO: consider refactoring this to introspect logs instead
         generated_sql = read_file("target", "run", "test", "models", "my_model.sql")
-        generated_sql_modified = _normalize_whitespace(generated_sql)
-        generated_sql_generic = _find_and_replace(
-            generated_sql_modified, "my_model", "<model_identifier>"
-        )
+        generated_sql_generic = _find_and_replace(generated_sql, "my_model", "<model_identifier>")
         generated_sql_generic = _find_and_replace(
             generated_sql_generic, "foreign_key_model", "<foreign_key_model_identifier>"
         )
 
-        expected_sql_check = _normalize_whitespace(expected_sql)
-
-        assert expected_sql_check == generated_sql_generic
+        assert _normalize_whitespace(expected_sql) == _normalize_whitespace(generated_sql_generic)
 
 
 class BaseConstraintsRollback:
     @pytest.fixture(scope="class")
     def models(self):
         return {
             "my_model.sql": my_model_sql,
@@ -481,19 +479,54 @@
             "constraints_schema.yml",
         )
 
         results = run_dbt(["run", "-s", "+my_model"])
         # assert at least my_model was run - additional upstreams may or may not be provided to the test setup via models fixture
         assert len(results) >= 1
         generated_sql = read_file("target", "run", "test", "models", "my_model.sql")
-        generated_sql_modified = _normalize_whitespace(generated_sql)
-        generated_sql_generic = _find_and_replace(
-            generated_sql_modified, "my_model", "<model_identifier>"
-        )
+
+        generated_sql_generic = _find_and_replace(generated_sql, "my_model", "<model_identifier>")
         generated_sql_generic = _find_and_replace(
             generated_sql_generic, "foreign_key_model", "<foreign_key_model_identifier>"
         )
-        assert _normalize_whitespace(expected_sql) == generated_sql_generic
+
+        assert _normalize_whitespace(expected_sql) == _normalize_whitespace(generated_sql_generic)
 
 
 class TestModelConstraintsRuntimeEnforcement(BaseModelConstraintsRuntimeEnforcement):
     pass
+
+
+class BaseConstraintQuotedColumn(BaseConstraintsRuntimeDdlEnforcement):
+    @pytest.fixture(scope="class")
+    def models(self):
+        return {
+            "my_model.sql": my_model_with_quoted_column_name_sql,
+            "constraints_schema.yml": model_quoted_column_schema_yml,
+        }
+
+    @pytest.fixture(scope="class")
+    def expected_sql(self):
+        return """
+create table <model_identifier> (
+    id integer not null,
+    "from" text not null,
+    date_day text,
+    check (("from" = 'blue'))
+) ;
+insert into <model_identifier> (
+    id, "from", date_day
+)
+(
+    select id, "from", date_day
+    from (
+        select
+          'blue' as "from",
+          1 as id,
+          '2019-01-01' as date_day
+    ) as model_subq
+);
+"""
+
+
+class TestConstraintQuotedColumn(BaseConstraintQuotedColumn):
+    pass
```

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/dbt_debug/test_dbt_debug.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/dbt_debug/test_dbt_debug.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/ephemeral/test_ephemeral.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/ephemeral/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/base_grants.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/grants/base_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_incremental_grants.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/grants/test_incremental_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_invalid_grants.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/grants/test_invalid_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_model_grants.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/grants/test_model_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_seed_grants.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/grants/test_seed_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_snapshot_grants.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/grants/test_snapshot_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/fixtures.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/hooks/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/test_model_hooks.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/hooks/test_model_hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/test_run_hooks.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/hooks/test_run_hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/fixtures.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/incremental/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_predicates.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/incremental/test_incremental_predicates.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_unique_id.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/incremental/test_incremental_unique_id.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/materialized_view/base.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/materialized_view/base.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/materialized_view/on_configuration_change.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/materialized_view/on_configuration_change.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/persist_docs/fixtures.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/persist_docs/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/persist_docs/test_persist_docs.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/persist_docs/test_persist_docs.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/python_model/test_python_model.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/python_model/test_python_model.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/python_model/test_spark.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/python_model/test_spark.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/query_comment/fixtures.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/query_comment/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/query_comment/test_query_comment.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/query_comment/test_query_comment.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/relations/test_changing_relation_type.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/relations/test_changing_relation_type.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/fixtures.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_copy/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/test_copy_uppercase.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_copy/test_copy_uppercase.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/test_simple_copy.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_copy/test_simple_copy.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/fixtures.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_seed/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/seeds.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_seed/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/test_seed.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_seed/test_seed.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/test_seed_type_override.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_seed/test_seed_type_override.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/common.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_snapshot/common.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/seeds.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_snapshot/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/snapshots.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_snapshot/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/test_snapshot.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/simple_snapshot/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/store_test_failures_tests/fixtures.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/store_test_failures_tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/base_array_utils.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/base_array_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/base_utils.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/base_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/base_data_type_macro.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/base_data_type_macro.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_bigint.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_bigint.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_boolean.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_boolean.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_float.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_float.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_int.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_int.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_numeric.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_numeric.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_string.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_string.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_timestamp.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/data_types/test_type_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_any_value.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_any_value.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_array_concat.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_array_concat.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_bool_or.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_bool_or.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_concat.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_concat.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_date_trunc.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_date_trunc.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_dateadd.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_dateadd.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_datediff.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_datediff.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_equals.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_equals.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_escape_single_quotes.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_escape_single_quotes.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_except.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_except.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_hash.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_hash.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_intersect.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_intersect.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_last_day.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_last_day.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_listagg.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_listagg.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_null_compare.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_null_compare.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_position.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_position.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_replace.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_replace.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_right.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_right.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_split_part.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_split_part.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_string_literal.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/fixture_string_literal.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_any_value.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_any_value.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_array_append.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_array_append.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_array_concat.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_array_concat.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_array_construct.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_array_construct.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_bool_or.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_bool_or.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_cast_bool_to_text.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_cast_bool_to_text.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_concat.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_concat.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_current_timestamp.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_current_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_date_trunc.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_date_trunc.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_dateadd.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_dateadd.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_datediff.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_datediff.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_equals.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_equals.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_escape_single_quotes.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_escape_single_quotes.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_except.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_except.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_hash.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_hash.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_intersect.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_intersect.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_last_day.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_last_day.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_length.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_length.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_listagg.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_listagg.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_null_compare.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_null_compare.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_position.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_position.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_replace.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_replace.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_right.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_right.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_safe_cast.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_safe_cast.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_split_part.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_split_part.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_string_literal.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_string_literal.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_timestamps.py` & `dbt-tests-adapter-1.6.0b4/dbt/tests/adapter/utils/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/PKG-INFO` & `dbt-tests-adapter-1.6.0b4/dbt_tests_adapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-tests-adapter
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: The dbt adapter tests for adapter plugins
 Home-page: https://github.com/dbt-labs/dbt-core/tree/main/tests/adapter
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/SOURCES.txt` & `dbt-tests-adapter-1.6.0b4/dbt_tests_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b3/setup.py` & `dbt-tests-adapter-1.6.0b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     # the user has a downlevel version of setuptools.
     print("Error: dbt requires setuptools v40.1.0 or higher.")
     print('Please upgrade setuptools with "pip install --upgrade setuptools" ' "and try again")
     sys.exit(1)
 
 
 package_name = "dbt-tests-adapter"
-package_version = "1.6.0b3"
+package_version = "1.6.0b4"
 description = """The dbt adapter tests for adapter plugins"""
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 setup(
```

