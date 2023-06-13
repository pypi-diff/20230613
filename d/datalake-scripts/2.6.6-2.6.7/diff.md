# Comparing `tmp/datalake-scripts-2.6.6.tar.gz` & `tmp/datalake-scripts-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalake-scripts-2.6.6.tar", last modified: Tue Jan 17 15:10:10 2023, max compression
+gzip compressed data, was "datalake-scripts-2.6.7.tar", last modified: Tue Jun 13 14:11:41 2023, max compression
```

## Comparing `datalake-scripts-2.6.6.tar` & `datalake-scripts-2.6.7.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.413178 datalake-scripts-2.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-01-17 15:10:10.413178 datalake-scripts-2.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.405178 datalake-scripts-2.6.6/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.405178 datalake-scripts-2.6.6/datalake/api_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/api_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/api_objects/bulk_search_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.409178 datalake-scripts-2.6.6/datalake/common/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/common/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/common/atom_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/common/ouput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/common/throttler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/common/token_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/common/warn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/datalake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.409178 datalake-scripts-2.6.6/datalake/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/endpoints/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/endpoints/bulk_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/endpoints/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/endpoints/sightings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/endpoints/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake/endpoints/threats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.409178 datalake-scripts-2.6.6/datalake_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.409178 datalake-scripts-2.6.6/datalake_scripts/common/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/common/base_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/common/base_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/common/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.409178 datalake-scripts-2.6.6/datalake_scripts/engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/engines/get_engine.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5400 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/engines/post_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.409178 datalake-scripts-2.6.6/datalake_scripts/helper_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/helper_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/helper_scripts/output_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/helper_scripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.409178 datalake-scripts-2.6.6/datalake_scripts/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/scripts/add_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/scripts/add_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/scripts/add_threats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/scripts/advanced_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8317 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/scripts/bulk_lookup_threats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/scripts/edit_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/scripts/get_query_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/scripts/get_threats_by_hashkey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/scripts/get_threats_from_query_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/datalake_scripts/scripts/lookup_threats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.413178 datalake-scripts-2.6.6/datalake_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-01-17 15:10:10.000000 datalake-scripts-2.6.6/datalake_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-01-17 15:10:10.000000 datalake-scripts-2.6.6/datalake_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 15:10:10.000000 datalake-scripts-2.6.6/datalake_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-01-17 15:10:10.000000 datalake-scripts-2.6.6/datalake_scripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-17 15:10:10.000000 datalake-scripts-2.6.6/datalake_scripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-17 15:10:10.000000 datalake-scripts-2.6.6/datalake_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-01-17 15:10:10.413178 datalake-scripts-2.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.409178 datalake-scripts-2.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.413178 datalake-scripts-2.6.6/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/common/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.413178 datalake-scripts-2.6.6/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/lib/test_advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/lib/test_atom_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/lib/test_auth_via_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/lib/test_bulk_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/lib/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/lib/test_sightings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/lib/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    21118 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/lib/test_threats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 15:10:10.413178 datalake-scripts-2.6.6/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/scripts/test_add_new_threats.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/scripts/test_base_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/scripts/test_csv_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/scripts/test_endpoint_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-01-17 15:09:59.000000 datalake-scripts-2.6.6/tests/scripts/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.882451 datalake-scripts-2.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-13 14:11:41.882451 datalake-scripts-2.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.862451 datalake-scripts-2.6.7/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.862451 datalake-scripts-2.6.7/datalake/api_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/api_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/api_objects/bulk_search_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.866451 datalake-scripts-2.6.7/datalake/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/atom_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/ouput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/throttler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/warn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/datalake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.870451 datalake-scripts-2.6.7/datalake/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/bulk_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/sightings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/threats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.870451 datalake-scripts-2.6.7/datalake_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.870451 datalake-scripts-2.6.7/datalake_scripts/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/common/base_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/common/base_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/common/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.870451 datalake-scripts-2.6.7/datalake_scripts/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/engines/get_engine.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5400 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/engines/post_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.870451 datalake-scripts-2.6.7/datalake_scripts/helper_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/helper_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/helper_scripts/output_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/helper_scripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.874451 datalake-scripts-2.6.7/datalake_scripts/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/add_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/add_threats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/advanced_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8317 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/bulk_lookup_threats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/edit_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/get_query_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/get_threats_by_hashkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/get_threats_from_query_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/lookup_threats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.882451 datalake-scripts-2.6.7/datalake_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-13 14:11:41.000000 datalake-scripts-2.6.7/datalake_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-13 14:11:41.000000 datalake-scripts-2.6.7/datalake_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:11:41.000000 datalake-scripts-2.6.7/datalake_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-13 14:11:41.000000 datalake-scripts-2.6.7/datalake_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 14:11:41.000000 datalake-scripts-2.6.7/datalake_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 14:11:41.000000 datalake-scripts-2.6.7/datalake_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-13 14:11:41.882451 datalake-scripts-2.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.874451 datalake-scripts-2.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.874451 datalake-scripts-2.6.7/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/common/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.878451 datalake-scripts-2.6.7/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_atom_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_auth_via_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_bulk_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14739 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_sightings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21118 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_threats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.882451 datalake-scripts-2.6.7/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/scripts/test_add_new_threats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/scripts/test_base_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/scripts/test_csv_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/scripts/test_endpoint_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/scripts/test_utils.py
```

### Comparing `datalake-scripts-2.6.6/PKG-INFO` & `datalake-scripts-2.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalake-scripts
-Version: 2.6.6
+Version: 2.6.7
 Summary: A collection of scripts to easily use the API of OCD Datalake
 Home-page: https://github.com/cert-orangecyberdefense/datalake/
 Author: OCD
 Author-email: cert-contact.ocd@orange.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `datalake-scripts-2.6.6/README.md` & `datalake-scripts-2.6.7/README.md`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/__init__.py` & `datalake-scripts-2.6.7/datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/api_objects/bulk_search_task.py` & `datalake-scripts-2.6.7/datalake/api_objects/bulk_search_task.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/common/atom.py` & `datalake-scripts-2.6.7/datalake/common/atom.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/common/atom_type.py` & `datalake-scripts-2.6.7/datalake/common/atom_type.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/common/ouput.py` & `datalake-scripts-2.6.7/datalake/common/ouput.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/common/throttler.py` & `datalake-scripts-2.6.7/datalake/common/throttler.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/common/token_manager.py` & `datalake-scripts-2.6.7/datalake/common/token_manager.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/common/utils.py` & `datalake-scripts-2.6.7/datalake/common/utils.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/datalake.py` & `datalake-scripts-2.6.7/datalake/datalake.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/endpoints/advanced_search.py` & `datalake-scripts-2.6.7/datalake/endpoints/advanced_search.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/endpoints/bulk_search.py` & `datalake-scripts-2.6.7/datalake/endpoints/bulk_search.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/endpoints/endpoint.py` & `datalake-scripts-2.6.7/datalake/endpoints/endpoint.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/endpoints/sightings.py` & `datalake-scripts-2.6.7/datalake/endpoints/sightings.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         threat_types: List[ThreatType] = None,
         tags: List[str] = None,
         description: str = None,
         atoms: List[Atom] = None,
         hashkeys: List[str] = None,
         relation: SightingRelation = None,
         editable: bool = None,
+        impersonate_id: int = None,
     ):
         """
         Submit a list of sightings.
         Either threat hashkeys or list of atom objects is required.
         Possible sightings type: POSITIVE, NEGATIVE, NEUTRAL. For POSITIVE and NEGATIVE sightings "threat_types"
         field is required. End date timestamp should always be in the past.
         relation field requires specific permission for the user.
@@ -37,14 +38,15 @@
             visibility,
             count,
             threat_types,
             tags,
             description,
             relation,
             editable,
+            impersonate_id,
         )
         url = self._build_url_for_endpoint("submit-sightings")
         res = self.datalake_requests(url, "post", self._post_headers(), payload).json()
         return res
 
     @staticmethod
     def _check_sightings_payload_parameters(
@@ -89,14 +91,15 @@
         visibility,
         count,
         threat_types=None,
         tags=None,
         description=None,
         relation=None,
         editable=None,
+        impersonate_id=None,
     ):
         """
         Internal function to prepare a list of Atoms for sighting submission to the format the API expects.
         """
         self._check_sightings_payload_parameters(
             atoms, hashkeys, sighting_type, visibility, count, threat_types, relation
         )
@@ -132,14 +135,16 @@
             ]
         if tags:
             payload["tags"] = tags
         if description:
             payload["description"] = description
         if editable is not None:
             payload["editable"] = editable
+        if impersonate_id:
+            payload["impersonate_id"] = impersonate_id
         return payload
 
     def sightings_filtered(
         self,
         threat_hashkey: str = None,
         limit: int = None,
         offset: int = None,
```

### Comparing `datalake-scripts-2.6.6/datalake/endpoints/tags.py` & `datalake-scripts-2.6.7/datalake/endpoints/tags.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake/endpoints/threats.py` & `datalake-scripts-2.6.7/datalake/endpoints/threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/cli.py` & `datalake-scripts-2.6.7/datalake_scripts/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from datalake_scripts.scripts import add_threats, get_threats_by_hashkey, edit_score, get_threats_from_query_hash, \
     add_comments, lookup_threats, add_tags, get_query_hash, bulk_lookup_threats, advanced_search
 
 
 class Cli:
     CLI_NAME = "ocd-dtl"
-    VERSION = "2.6.6"
+    VERSION = "2.6.7"
 
     def __init__(self):
         parser = argparse.ArgumentParser(
             description='Cli to interact with OCD\'s Datalake',
             usage=f'''
             {self.CLI_NAME} <command> [<args>]
```

### Comparing `datalake-scripts-2.6.6/datalake_scripts/common/__init__.py` & `datalake-scripts-2.6.7/datalake_scripts/common/__init__.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/common/base_engine.py` & `datalake-scripts-2.6.7/datalake_scripts/common/base_engine.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/common/base_script.py` & `datalake-scripts-2.6.7/datalake_scripts/common/base_script.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/common/mixins.py` & `datalake-scripts-2.6.7/datalake_scripts/common/mixins.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/engines/get_engine.py` & `datalake-scripts-2.6.7/datalake_scripts/engines/get_engine.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/engines/post_engine.py` & `datalake-scripts-2.6.7/datalake_scripts/engines/post_engine.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/helper_scripts/output_builder.py` & `datalake-scripts-2.6.7/datalake_scripts/helper_scripts/output_builder.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/helper_scripts/utils.py` & `datalake-scripts-2.6.7/datalake_scripts/helper_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/scripts/add_comments.py` & `datalake-scripts-2.6.7/datalake_scripts/scripts/add_comments.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/scripts/add_tags.py` & `datalake-scripts-2.6.7/datalake_scripts/scripts/add_tags.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/scripts/add_threats.py` & `datalake-scripts-2.6.7/datalake_scripts/scripts/add_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/scripts/advanced_search.py` & `datalake-scripts-2.6.7/datalake_scripts/scripts/advanced_search.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/scripts/bulk_lookup_threats.py` & `datalake-scripts-2.6.7/datalake_scripts/scripts/bulk_lookup_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/scripts/edit_score.py` & `datalake-scripts-2.6.7/datalake_scripts/scripts/edit_score.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/scripts/get_query_hash.py` & `datalake-scripts-2.6.7/datalake_scripts/scripts/get_query_hash.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/scripts/get_threats_by_hashkey.py` & `datalake-scripts-2.6.7/datalake_scripts/scripts/get_threats_by_hashkey.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/scripts/get_threats_from_query_hash.py` & `datalake-scripts-2.6.7/datalake_scripts/scripts/get_threats_from_query_hash.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts/scripts/lookup_threats.py` & `datalake-scripts-2.6.7/datalake_scripts/scripts/lookup_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/datalake_scripts.egg-info/PKG-INFO` & `datalake-scripts-2.6.7/datalake_scripts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalake-scripts
-Version: 2.6.6
+Version: 2.6.7
 Summary: A collection of scripts to easily use the API of OCD Datalake
 Home-page: https://github.com/cert-orangecyberdefense/datalake/
 Author: OCD
 Author-email: cert-contact.ocd@orange.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `datalake-scripts-2.6.6/datalake_scripts.egg-info/SOURCES.txt` & `datalake-scripts-2.6.7/datalake_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/setup.py` & `datalake-scripts-2.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/tests/common/fixture.py` & `datalake-scripts-2.6.7/tests/common/fixture.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/tests/lib/test_advanced_search.py` & `datalake-scripts-2.6.7/tests/lib/test_advanced_search.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/tests/lib/test_atom_type.py` & `datalake-scripts-2.6.7/tests/lib/test_atom_type.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/tests/lib/test_auth_via_tokens.py` & `datalake-scripts-2.6.7/tests/lib/test_auth_via_tokens.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/tests/lib/test_bulk_search.py` & `datalake-scripts-2.6.7/tests/lib/test_bulk_search.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/tests/lib/test_output.py` & `datalake-scripts-2.6.7/tests/lib/test_output.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/tests/lib/test_sightings.py` & `datalake-scripts-2.6.7/tests/lib/test_sightings.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,47 @@
     payload = datalake.Sightings._prepare_sightings_payload(
         atoms, None, start, end, sighting_type, visibility, count, tags=[]
     )
 
     assert expected_payload == payload
 
 
+def test_prepare_sightings_payload_with_impersonate_id(datalake):
+    atoms = [file_atom]
+    sighting_type = SightingType.NEUTRAL
+    visibility = Visibility.ORGANIZATION
+    count = 1
+    impersonate_id = "1234567890"
+
+    expected_payload = {
+        "file_list": [
+            {
+                "hashes": {
+                    "md5": "d26351ba789fba3385d2382aa9d24908",
+                    "sha1": "a61e243f25b8b08661011869a53315363697a0f4",
+                    "sha256": "c056f9206143bc43a7f524f946149ad77c0c491ce816a2865feb6e5f2eaf521e",
+                    "sha512": "01525491943d324e928e4d30702fa731db20a2c82dc6b1d8bf7cf157227517de"
+                    "48f10be15053a63be598f75618ea0179c33f8726bde620e976c7ff5a4fbaa944",
+                }
+            }
+        ],
+        "start_timestamp": "2021-05-10T16:20:23Z",
+        "end_timestamp": "2021-05-11T16:20:23Z",
+        "visibility": "ORGANIZATION",
+        "type": "neutral",
+        "count": 1,
+        "impersonate_id": "1234567890",
+    }
+
+    payload = datalake.Sightings._prepare_sightings_payload(
+        atoms, None, start, end, sighting_type, visibility, count, impersonate_id=impersonate_id
+    )
+
+    assert expected_payload == payload
+
 @responses.activate
 def test_submit_sightings(datalake):
     url = "https://datalake.cert.orangecyberdefense.com/api/v2/mrti/threats/sighting/"
 
     expected_request = {
         "file_list": [
             {
```

### Comparing `datalake-scripts-2.6.6/tests/lib/test_tags.py` & `datalake-scripts-2.6.7/tests/lib/test_tags.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/tests/lib/test_threats.py` & `datalake-scripts-2.6.7/tests/lib/test_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/tests/scripts/test_add_new_threats.py` & `datalake-scripts-2.6.7/tests/scripts/test_add_new_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/tests/scripts/test_base_engine.py` & `datalake-scripts-2.6.7/tests/scripts/test_base_engine.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/tests/scripts/test_csv_builder.py` & `datalake-scripts-2.6.7/tests/scripts/test_csv_builder.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/tests/scripts/test_endpoint_config.py` & `datalake-scripts-2.6.7/tests/scripts/test_endpoint_config.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.6/tests/scripts/test_utils.py` & `datalake-scripts-2.6.7/tests/scripts/test_utils.py`

 * *Files identical despite different names*

