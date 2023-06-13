# Comparing `tmp/galaxy-test-base-22.1.1.tar.gz` & `tmp/galaxy-test-base-23.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-test-base-22.1.1.tar", last modified: Mon Aug 22 19:46:00 2022, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/test_base/dist/.tmp-r1rvjy6z/galaxy-test-base-23.0.2.tar", last modified: Tue Jun 13 17:14:14 2023, max compression
```

## Comparing `galaxy-test-base-22.1.1.tar` & `galaxy-test-base-23.0.2.tar`

### file list

```diff
@@ -1,63 +1,52 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:00.409917 galaxy-test-base-22.1.1/
--rw-r--r--   0 mvandenb   (501) staff       (20)      335 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2021-09-10 08:52:38.000000 galaxy-test-base-22.1.1/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)       65 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     2954 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/Makefile
--rw-r--r--   0 mvandenb   (501) staff       (20)     1604 2022-08-22 19:46:00.410035 galaxy-test-base-22.1.1/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      308 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:00.399266 galaxy-test-base-22.1.1/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       65 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      422 2022-08-22 19:45:30.000000 galaxy-test-base-22.1.1/galaxy/project_galaxy_test_base.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:00.399499 galaxy-test-base-22.1.1/galaxy_test/
--rw-r--r--   0 mvandenb   (501) staff       (20)       65 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy_test/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:00.403125 galaxy-test-base-22.1.1/galaxy_test/base/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5376 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy_test/base/api.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3606 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy_test/base/api_asserts.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1275 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/api_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      350 2022-08-18 15:49:02.000000 galaxy-test-base-22.1.1/galaxy_test/base/constants.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:00.407214 galaxy-test-base-22.1.1/galaxy_test/base/data/
--rw-r--r--   0 mvandenb   (501) staff       (20)      233 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/minimal_tool_no_id.json
--rw-r--r--   0 mvandenb   (501) staff       (20)    16151 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_subworkflow_with_integer_input.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     2699 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_1.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     3246 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_2.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     5126 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_batch.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     6714 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_map_reduce_pause.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     3740 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_matching_lists.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     2808 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_missing_tool.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     3658 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_pause.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     1801 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     1816 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)    13049 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_topoambigouity.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)    13050 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     3328 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_two_random_lines.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     1120 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_validation_1.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     2162 2022-08-18 15:49:02.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_with_input_tags.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     2162 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_with_runtime_input.ga
--rw-r--r--   0 mvandenb   (501) staff       (20)     1083 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy_test/base/env.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2309 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy_test/base/instrument.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      620 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy_test/base/interactor.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      878 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy_test/base/nose_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    94709 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy_test/base/populators.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     9555 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy_test/base/rules_test_data.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2017 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy_test/base/testcase.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      221 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy_test/base/tool_sheds_conf.xml
--rw-r--r--   0 mvandenb   (501) staff       (20)     5560 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy_test/base/uses_shed.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    17995 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/galaxy_test/base/workflow_fixtures.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:00.408938 galaxy-test-base-22.1.1/galaxy_test_base.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1604 2022-08-22 19:45:59.000000 galaxy-test-base-22.1.1/galaxy_test_base.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)     1961 2022-08-22 19:46:00.000000 galaxy-test-base-22.1.1/galaxy_test_base.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:59.000000 galaxy-test-base-22.1.1/galaxy_test_base.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       27 2022-08-22 19:45:59.000000 galaxy-test-base-22.1.1/galaxy_test_base.egg-info/entry_points.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:59.000000 galaxy-test-base-22.1.1/galaxy_test_base.egg-info/not-zip-safe
--rw-r--r--   0 mvandenb   (501) staff       (20)       24 2022-08-22 19:45:59.000000 galaxy-test-base-22.1.1/galaxy_test_base.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       12 2022-08-22 19:45:59.000000 galaxy-test-base-22.1.1/galaxy_test_base.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       25 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:00.409733 galaxy-test-base-22.1.1/scripts/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1442 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/scripts/commit_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2166 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/scripts/new_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      804 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/scripts/print_version_for_release.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    33060 2022-08-22 19:46:00.416000 galaxy-test-base-22.1.1/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)     2814 2022-08-22 19:45:28.000000 galaxy-test-base-22.1.1/setup.py
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-03-24 19:47:11.000000 galaxy-test-base-22.1.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:14.000000 galaxy-test-base-23.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-13 17:04:36.000000 galaxy-test-base-23.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-13 17:14:14.000000 galaxy-test-base-23.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:14.000000 galaxy-test-base-23.0.2/galaxy_test/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:14.000000 galaxy-test-base-23.0.2/galaxy_test/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/api_asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/api_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:14.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/minimal_tool_no_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16151 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_subworkflow_with_integer_input.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_1.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_2.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_batch.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_map_reduce_pause.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_matching_lists.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_missing_tool.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_pause.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_topoambigouity.ga
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_two_random_lines.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_validation_1.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_with_input_tags.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_with_runtime_input.ga
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/json_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125943 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/populators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/rules_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/uses_shed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/base/workflow_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/galaxy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:14.000000 galaxy-test-base-23.0.2/galaxy_test_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-13 17:14:14.000000 galaxy-test-base-23.0.2/galaxy_test_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-13 17:14:14.000000 galaxy-test-base-23.0.2/galaxy_test_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:14:14.000000 galaxy-test-base-23.0.2/galaxy_test_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 17:14:14.000000 galaxy-test-base-23.0.2/galaxy_test_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 17:14:14.000000 galaxy-test-base-23.0.2/galaxy_test_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-13 17:14:14.000000 galaxy-test-base-23.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:04:37.000000 galaxy-test-base-23.0.2/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-test-base-22.1.1/LICENSE` & `galaxy-test-base-23.0.2/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,61 @@
-Copyright (c) 2005-2016 Galaxy Contributors (see CONTRIBUTORS.md)
+Copyright (c) 2005-2022 Galaxy Contributors (see CONTRIBUTORS.md)
+
+Work contributed from 2021-04-07 onwards is licensed under the MIT License.
+Work contributed before this date is licensed under the Academic Free License
+version 3.0.
+See https://github.com/galaxyproject/galaxy/ for the contribution history.
+See below for the full text of both licenses.
+
+
+Some icons found in Galaxy are from the Silk Icons set, available under
+the Creative Commons Attribution 2.5 License, from:
+
+http://www.famfamfam.com/lab/icons/silk/
+
+
+Other images and documentation are licensed under the Creative Commons
+Attribution 3.0 (CC BY 3.0) License. See:
+
+http://creativecommons.org/licenses/by/3.0/
+
+
+--------------------------------------------------------------------------------
+
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+--------------------------------------------------------------------------------
+
+
+Academic Free License ("AFL") v. 3.0
+
+This Academic Free License (the "License") applies to any original work of
+authorship (the "Original Work") whose owner (the "Licensor") has placed the
+following licensing notice adjacent to the copyright notice for the Original
+Work:
 
 Licensed under the Academic Free License version 3.0
 
  1) Grant of Copyright License. Licensor grants You a worldwide, royalty-free, 
     non-exclusive, sublicensable license, for the duration of the copyright, to 
     do the following:
 
@@ -169,18 +222,7 @@
     replace the notice specified in the first paragraph above with the 
     notice "Licensed under <insert your license name here>" or with a notice 
     of your own that is not confusingly similar to the notice in this 
     License; and (iii) You may not claim that your original works are open 
     source software unless your Modified License has been approved by Open 
     Source Initiative (OSI) and You comply with its license review and 
     certification process.
-
-
-Some icons found in Galaxy are from the Silk Icons set, available under
-the Creative Commons Attribution 2.5 License, from:
-
-http://www.famfamfam.com/lab/icons/silk/
-
-
-Other images and documentation are licensed under the Creative Commons Attribution 3.0 (CC BY 3.0) License.   See 
-
-http://creativecommons.org/licenses/by/3.0/
```

### Comparing `galaxy-test-base-22.1.1/PKG-INFO` & `galaxy-test-base-23.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,77 @@
 Metadata-Version: 2.1
 Name: galaxy-test-base
-Version: 22.1.1
-Summary: Galaxy Testing Utilities
+Version: 23.0.2
+Summary: Galaxy testing utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-test-base.svg
    :target: https://pypi.org/project/galaxy-test-base/
 
 
 
 Overview
 --------
 
 The Galaxy_ testing base package.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.1.dev0
----------------------
+-------------------
+23.0.2 (2023-06-13)
+-------------------
+
+No recorded changes since last release
 
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
 
----------------------
+=========
+Bug fixes
+=========
+
+* Ensure history export contains all expected datasets by `@davelopez <https://github.com/davelopez>`_ in `#16013 <https://github.com/galaxyproject/galaxy/pull/16013>`_
+* Fix extended metadata file size handling by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16109 <https://github.com/galaxyproject/galaxy/pull/16109>`_
+
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * Initial release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * Initial import from the 20.05 branch of Galaxy.
-
-
```

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/api_asserts.py` & `galaxy-test-base-23.0.2/galaxy_test/base/api_asserts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 """Utility methods for making assertions about Galaxy API responses, etc...
 """
-from typing import Any, cast, Dict, Union
+from typing import (
+    Any,
+    cast,
+    Dict,
+    Union,
+)
 
 from requests import Response
 
 from galaxy.exceptions.error_codes import ErrorCode
 
 ASSERT_FAIL_ERROR_CODE = "Expected Galaxy error code %d, obtained %d"
 ASSERT_FAIL_STATUS_CODE = "Request status code (%d) was not expected value %s. Body was %s"
@@ -53,25 +58,19 @@
 
 
 def assert_error_code_is(response: Union[Response, dict], error_code: Union[int, ErrorCode]):
     """Assert that the supplied response has the supplied Galaxy error code.
 
     Galaxy error codes can be imported from :py:mod:`galaxy.exceptions.error_codes`
     to test against.
-
-    ::
-
-        from galaxy.exceptions import error_codes
-        assert_error_code_is(response, error_codes.USER_REQUEST_MISSING_PARAMETER)
-
     """
     as_dict = _as_dict(response)
     assert_has_keys(as_dict, "err_code")
     err_code = as_dict["err_code"]
-    assert err_code == int(error_code), ASSERT_FAIL_ERROR_CODE % (err_code, int(error_code))
+    assert err_code == int(error_code), ASSERT_FAIL_ERROR_CODE % (error_code, err_code)
 
 
 def assert_object_id_error(response: Response):
     # for tests that use fake object IDs - API might throw MalformedId (400) or
     # or ObjectNotFound (404) - depending if the ID happens to be parseable with
     # servers API key.
     error_code = response.status_code
```

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_subworkflow_with_integer_input.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_subworkflow_with_integer_input.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_1.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_1.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_2.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_2.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_batch.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_batch.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_map_reduce_pause.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_map_reduce_pause.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_matching_lists.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_matching_lists.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_missing_tool.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_missing_tool.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_pause.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_pause.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_randomlines_legacy_params.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_randomlines_legacy_params_mixed_types.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_topoambigouity.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_topoambigouity.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_topoambigouity_auto_laidout.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_two_random_lines.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_two_random_lines.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_validation_1.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_validation_1.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_with_input_tags.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_with_input_tags.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/data/test_workflow_with_runtime_input.ga` & `galaxy-test-base-23.0.2/galaxy_test/base/data/test_workflow_with_runtime_input.ga`

 * *Files identical despite different names*

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/env.py` & `galaxy-test-base-23.0.2/galaxy_test/base/env.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """Base utilities for working Galaxy test environments.
 """
 import fcntl
 import os
 import socket
 import struct
-from typing import Optional, Tuple
+from typing import (
+    Optional,
+    Tuple,
+)
 
-DEFAULT_WEB_HOST = socket.gethostbyname('localhost')
+DEFAULT_WEB_HOST = socket.gethostbyname("localhost")
 
 
 def setup_keep_outdir() -> str:
-    keep_outdir = os.environ.get('GALAXY_TEST_SAVE', '')
-    if keep_outdir > '':
+    keep_outdir = os.environ.get("GALAXY_TEST_SAVE", "")
+    if keep_outdir > "":
         try:
             os.makedirs(keep_outdir)
         except Exception:
             pass
     return keep_outdir
 
 
 def target_url_parts() -> Tuple[str, Optional[str], str]:
-    host = socket.gethostbyname(os.environ.get('GALAXY_TEST_HOST', DEFAULT_WEB_HOST))
-    port = os.environ.get('GALAXY_TEST_PORT')
+    host = socket.gethostbyname(os.environ.get("GALAXY_TEST_HOST", DEFAULT_WEB_HOST))
+    port = os.environ.get("GALAXY_TEST_PORT")
     if port:
         default_url = f"http://{host}:{port}"
     else:
         default_url = f"http://{host}"
-    url = os.environ.get('GALAXY_TEST_EXTERNAL', default_url)
+    url = os.environ.get("GALAXY_TEST_EXTERNAL", default_url)
     return host, port, url
 
 
 def get_ip_address(ifname: str) -> str:
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-    return socket.inet_ntoa(fcntl.ioctl(
-        s.fileno(),
-        0x8915,  # SIOCGIFADDR
-        struct.pack('256s', ifname[:15].encode('utf-8'))
-    )[20:24])
+    return socket.inet_ntoa(
+        fcntl.ioctl(s.fileno(), 0x8915, struct.pack("256s", ifname[:15].encode("utf-8")))[20:24]  # SIOCGIFADDR
+    )
```

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/interactor.py` & `galaxy-test-base-23.0.2/galaxy_test/base/interactor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from galaxy.tool_util.verify.interactor import GalaxyInteractorApi
 
 
 class TestCaseGalaxyInteractor(GalaxyInteractorApi):
-
     def __init__(self, functional_test_case, test_user=None, api_key=None):
         self.functional_test_case = functional_test_case
         super().__init__(
             galaxy_url=functional_test_case.url,
             master_api_key=getattr(functional_test_case, "master_api_key", None),
             api_key=api_key or getattr(functional_test_case, "user_api_key", None),
             test_user=test_user,
```

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/populators.py` & `galaxy-test-base-23.0.2/galaxy_test/base/populators.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,85 +33,108 @@
 is a bit ugly and this ugliness again stems from these organically growing from a
 framework that originally didn't use requests at all.
 
 API tests and Selenium tests routinely use requests directly and that is totally fine,
 requests should just be filtered through the verb abstractions if that functionality
 is then added to populators to be shared across tests or across testing frameworks.
 """
+import base64
 import contextlib
 import json
 import os
-import random
-import string
+import tarfile
+import tempfile
 import time
 import unittest
 import urllib.parse
-from abc import ABCMeta, abstractmethod
+from abc import (
+    ABCMeta,
+    abstractmethod,
+)
 from functools import wraps
 from io import StringIO
 from operator import itemgetter
 from typing import (
     Any,
     Callable,
     Dict,
+    Generator,
     List,
     NamedTuple,
     Optional,
     Set,
     Tuple,
+    Union,
 )
+from uuid import UUID
 
-import cwltest
+import cwltest.compare
 import requests
 import yaml
-from bioblend.galaxy import GalaxyClient
+from bioblend.galaxyclient import GalaxyClient
 from gxformat2 import (
     convert_and_import_workflow,
     ImporterGalaxyInterface,
 )
 from gxformat2._yaml import ordered_load
-from requests.models import Response
+from requests import Response
+from rocrate.rocrate import ROCrate
+from typing_extensions import Literal
 
 from galaxy.tool_util.client.staging import InteractorStaging
-from galaxy.tool_util.cwl.util import guess_artifact_type
+from galaxy.tool_util.cwl.util import (
+    download_output,
+    GalaxyOutput,
+    guess_artifact_type,
+    invocation_to_output,
+    output_to_cwl_json,
+    tool_response_to_output,
+)
 from galaxy.tool_util.verify.test_data import TestDataResolver
 from galaxy.tool_util.verify.wait import (
     timeout_type,
     TimeoutAssertionError,
     wait_on as tool_util_wait_on,
 )
 from galaxy.util import (
     DEFAULT_SOCKET_TIMEOUT,
     galaxy_root_path,
 )
 from galaxy.util.resources import resource_string
+from galaxy.util.unittest_utils import skip_if_site_down
+from galaxy_test.base.decorators import (
+    has_requirement,
+    using_requirement,
+)
+from galaxy_test.base.json_schema_utils import JsonSchemaValidator
 from . import api_asserts
 from .api import ApiTestInteractor
+from .api_util import random_name
 
+FILE_URL = "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/4.bed"
+FILE_MD5 = "37b59762b59fff860460522d271bc111"
 
 CWL_TOOL_DIRECTORY = os.path.join(galaxy_root_path, "test", "functional", "tools", "cwl_tools")
 
 # Simple workflow that takes an input and call cat wrapper on it.
 workflow_str = resource_string(__package__, "data/test_workflow_1.ga")
 # Simple workflow that takes an input and filters with random lines twice in a
 # row - first grabbing 8 lines at random and then 6.
 workflow_random_x2_str = resource_string(__package__, "data/test_workflow_2.ga")
 
-
 DEFAULT_TIMEOUT = 60  # Secs to wait for state to turn ok
 
 SKIP_FLAKEY_TESTS_ON_ERROR = os.environ.get("GALAXY_TEST_SKIP_FLAKEY_TESTS_ON_ERROR", None)
 
 
 def flakey(method):
-
     @wraps(method)
-    def wrapped_method(test_case, *args, **kwargs):
+    def wrapped_method(*args, **kwargs):
         try:
-            method(test_case, *args, **kwargs)
+            method(*args, **kwargs)
         except unittest.SkipTest:
             raise
         except Exception:
             if SKIP_FLAKEY_TESTS_ON_ERROR:
                 raise unittest.SkipTest("Error encountered during test marked as @flakey.")
             else:
                 raise
@@ -122,15 +145,14 @@
 def skip_without_tool(tool_id):
     """Decorate an API test method as requiring a specific tool.
 
     Have test framework skip the test case if the tool is unavailable.
     """
 
     def method_wrapper(method):
-
         def get_tool_ids(api_test_case):
             index = api_test_case.galaxy_interactor.get("tools", data=dict(in_panel=False))
             tools = index.json()
             # In panels by default, so flatten out sections...
             tool_ids = [itemgetter("id")(_) for _ in tools]
             return tool_ids
 
@@ -140,14 +162,26 @@
             return method(api_test_case, *args, **kwargs)
 
         return wrapped_method
 
     return method_wrapper
 
 
+def skip_without_asgi(method):
+    @wraps(method)
+    def wrapped_method(api_test_case, *args, **kwd):
+        config = api_test_case.galaxy_interactor.get("configuration").json()
+        asgi_enabled = config.get("asgi_enabled", False)
+        if not asgi_enabled:
+            raise unittest.SkipTest("ASGI not enabled, skipping test")
+        return method(api_test_case, *args, **kwd)
+
+    return wrapped_method
+
+
 def skip_without_datatype(extension):
     """Decorate an API test method as requiring a specific datatype.
 
     Have test framework skip the test case if the datatype is unavailable.
     """
 
     def has_datatype(api_test_case):
@@ -164,70 +198,32 @@
             method(api_test_case, *args, **kwargs)
 
         return wrapped_method
 
     return method_wrapper
 
 
-def is_site_up(url):
-    try:
-        response = requests.get(url, timeout=10)
-        return response.status_code == 200
-    except Exception:
-        return False
-
-
-def skip_if_site_down(url):
-
-    def method_wrapper(method):
-        @wraps(method)
-        def wrapped_method(api_test_case, *args, **kwargs):
-            _raise_skip_if(not is_site_up(url), f"Test depends on [{url}] being up and it appears to be down.")
-            method(api_test_case, *args, **kwargs)
-
-        return wrapped_method
-
-    return method_wrapper
-
-
 skip_if_toolshed_down = skip_if_site_down("https://toolshed.g2.bx.psu.edu")
-skip_if_github_down = skip_if_site_down("https://github.com/")
 
 
 def summarize_instance_history_on_error(method):
     @wraps(method)
     def wrapped_method(api_test_case, *args, **kwds):
         try:
             method(api_test_case, *args, **kwds)
         except Exception:
             api_test_case.dataset_populator._summarize_history(api_test_case.history_id)
             raise
 
     return wrapped_method
 
 
-def uses_test_history(**test_history_kwd):
-    """Can override require_new and cancel_executions using kwds to decorator.
-    """
-
-    def method_wrapper(method):
-        @wraps(method)
-        def wrapped_method(api_test_case, *args, **kwds):
-            with api_test_case.dataset_populator.test_history(**test_history_kwd) as history_id:
-                method(api_test_case, history_id, *args, **kwds)
-
-        return wrapped_method
-
-    return method_wrapper
-
-
 def _raise_skip_if(check, *args):
     if check:
-        from nose.plugins.skip import SkipTest
-        raise SkipTest(*args)
+        raise unittest.SkipTest(*args)
 
 
 def conformance_tests_gen(directory, filename="conformance_tests.yaml"):
     conformance_tests_path = os.path.join(directory, filename)
     with open(conformance_tests_path) as f:
         conformance_tests = yaml.safe_load(f)
 
@@ -237,204 +233,112 @@
             yield from conformance_tests_gen(os.path.join(directory, import_dir), import_filename)
         else:
             conformance_test["directory"] = directory
             yield conformance_test
 
 
 class CwlRun:
-
     def __init__(self, dataset_populator, history_id):
         self.dataset_populator = dataset_populator
         self.history_id = history_id
 
+    @abstractmethod
+    def _output_name_to_object(self, output_name) -> GalaxyOutput:
+        """
+        Convert the name of a run output to a GalaxyOutput object.
+        """
 
-class CwlToolRun(CwlRun):
+    def get_output_as_object(self, output_name, download_folder=None):
+        galaxy_output = self._output_name_to_object(output_name)
+
+        def get_metadata(history_content_type, content_id):
+            if history_content_type == "raw_value":
+                return {}
+            elif history_content_type == "dataset":
+                return self.dataset_populator.get_history_dataset_details(self.history_id, dataset_id=content_id)
+            else:
+                assert history_content_type == "dataset_collection"
+                # Don't wait - we've already done that, history might be "new"
+                return self.dataset_populator.get_history_collection_details(
+                    self.history_id, content_id=content_id, wait=False
+                )
+
+        def get_dataset(dataset_details, filename=None):
+            content = self.dataset_populator.get_history_dataset_content(
+                self.history_id, dataset_id=dataset_details["id"], type="content", filename=filename
+            )
+            if filename is None:
+                basename = dataset_details.get("created_from_basename")
+                if not basename:
+                    basename = dataset_details.get("name")
+            else:
+                basename = os.path.basename(filename)
+            return {"content": content, "basename": basename}
 
+        def get_extra_files(dataset_details):
+            return self.dataset_populator.get_history_dataset_extra_files(
+                self.history_id, dataset_id=dataset_details["id"]
+            )
+
+        output = output_to_cwl_json(
+            galaxy_output,
+            get_metadata,
+            get_dataset,
+            get_extra_files,
+            pseudo_location=True,
+        )
+        if download_folder:
+            if isinstance(output, dict) and "basename" in output:
+                download_path = os.path.join(download_folder, output["basename"])
+                download_output(galaxy_output, get_metadata, get_dataset, get_extra_files, download_path)
+                output["path"] = download_path
+                output["location"] = f"file://{download_path}"
+        return output
+
+    @abstractmethod
+    def wait(self):
+        """
+        Wait for the completion of the job(s) generated by this run.
+        """
+
+
+class CwlToolRun(CwlRun):
     def __init__(self, dataset_populator, history_id, run_response):
         super().__init__(dataset_populator, history_id)
         self.run_response = run_response
 
     @property
     def job_id(self):
         return self.run_response.json()["jobs"][0]["id"]
 
+    def _output_name_to_object(self, output_name):
+        return tool_response_to_output(self.run_response.json(), self.history_id, output_name)
+
     def wait(self):
         self.dataset_populator.wait_for_job(self.job_id, assert_ok=True)
 
 
 class CwlWorkflowRun(CwlRun):
-
     def __init__(self, dataset_populator, workflow_populator, history_id, workflow_id, invocation_id):
         super().__init__(dataset_populator, history_id)
         self.workflow_populator = workflow_populator
         self.workflow_id = workflow_id
         self.invocation_id = invocation_id
 
-    def wait(self):
-        self.workflow_populator.wait_for_invocation_and_jobs(
-            self.history_id, self.workflow_id, self.invocation_id
-        )
-
-
-class CwlPopulator:
-
-    def __init__(self, dataset_populator, workflow_populator):
-        self.dataset_populator = dataset_populator
-        self.workflow_populator = workflow_populator
-
-    def get_conformance_test(self, version, doc):
-        for test in conformance_tests_gen(os.path.join(CWL_TOOL_DIRECTORY, str(version))):
-            if test.get("doc") == doc:
-                return test
-        raise Exception(f"doc [{doc}] not found")
-
-    def _run_cwl_tool_job(
-        self,
-        tool_id: str,
-        job: dict,
-        history_id: str,
-        assert_ok: bool = True,
-    ):
-        galaxy_tool_id: Optional[str] = tool_id
-        tool_uuid = None
-
-        if os.path.exists(tool_id):
-            raw_tool_id = os.path.basename(tool_id)
-            index = self.dataset_populator._get("tools", data=dict(in_panel=False))
-            tools = index.json()
-            # In panels by default, so flatten out sections...
-            tool_ids = [itemgetter("id")(_) for _ in tools]
-            if raw_tool_id in tool_ids:
-                galaxy_tool_id = raw_tool_id
-            else:
-                dynamic_tool = self.dataset_populator.create_tool_from_path(tool_id)
-                galaxy_tool_id = None
-                tool_uuid = dynamic_tool["uuid"]
-
-        run_response = self.dataset_populator.run_tool_raw(galaxy_tool_id, job, history_id, tool_uuid=tool_uuid)
-        if assert_ok:
-            run_response.raise_for_status()
-        return CwlToolRun(self.dataset_populator, history_id, run_response)
-
-    def _run_cwl_workflow_job(
-        self,
-        workflow_path: str,
-        job: dict,
-        history_id: str,
-        assert_ok: bool = True,
-    ):
-        workflow_path, object_id = urllib.parse.urldefrag(workflow_path)
-        workflow_id = self.workflow_populator.import_workflow_from_path(workflow_path, object_id)
-
-        request = {
-            # TODO: rework tool state corrections so more of these are valid in Galaxy
-            # workflows as well, and then make it the default. Or decide they are safe.
-            "allow_tool_state_corrections": True,
-        }
-        invocation_id = self.workflow_populator.invoke_workflow(workflow_id, history_id=history_id, inputs=job, request=request, inputs_by="name")
-        return CwlWorkflowRun(self.dataset_populator, self.workflow_populator, history_id, workflow_id, invocation_id)
-
-    def run_cwl_job(
-        self,
-        artifact: str,
-        job_path: Optional[str] = None,
-        job: Optional[Dict] = None,
-        test_data_directory: Optional[str] = None,
-        history_id: Optional[str] = None,
-        assert_ok=True,
-    ):
-        """
-        :param artifact: CWL tool id, or (absolute or relative) path to a CWL
-          tool or workflow file
-        """
-        if history_id is None:
-            history_id = self.dataset_populator.new_history()
-        artifact_without_id = artifact.split("#", 1)[0]
-        if not os.path.exists(artifact_without_id):
-            # Assume it's a tool id
-            tool_or_workflow = "tool"
-        else:
-            tool_or_workflow = guess_artifact_type(artifact)
-        if job_path and not os.path.exists(job_path):
-            raise ValueError(f"job_path [{job_path}] does not exist")
-        if test_data_directory is None and job_path is not None:
-            test_data_directory = os.path.dirname(job_path)
-        if job_path is not None:
-            assert job is None
-            with open(job_path) as f:
-                if job_path.endswith(".yml") or job_path.endswith(".yaml"):
-                    job = yaml.safe_load(f)
-                else:
-                    job = json.load(f)
-        elif job is None:
-            job = {}
-        _, datasets_uploaded = stage_inputs(
-            self.dataset_populator.galaxy_interactor,
-            history_id,
-            job,
-            use_fetch_api=False,
-            tool_or_workflow=tool_or_workflow,
-            job_dir=test_data_directory,
-        )
-        if datasets_uploaded:
-            self.dataset_populator.wait_for_history(history_id=history_id, assert_ok=True)
-        if tool_or_workflow == "tool":
-            run_object = self._run_cwl_tool_job(
-                artifact,
-                job,
-                history_id,
-                assert_ok=assert_ok,
-            )
-        else:
-            run_object = self._run_cwl_workflow_job(
-                artifact,
-                job,
-                history_id,
-                assert_ok=assert_ok,
-            )
-        if assert_ok:
-            try:
-                run_object.wait()
-            except Exception:
-                self.dataset_populator._summarize_history(history_id)
-                raise
-        return run_object
-
-    def run_conformance_test(self, version, doc):
-        test = self.get_conformance_test(version, doc)
-        directory = test["directory"]
-        artifact = os.path.join(directory, test["tool"])
-        job_path = test.get("job")
-        if job_path is not None:
-            job_path = os.path.join(directory, job_path)
-        should_fail = test.get("should_fail", False)
-        try:
-            run = self.run_cwl_job(artifact, job_path=job_path)
-        except Exception:
-            # Should fail so this is good!
-            if should_fail:
-                return True
-            raise
-
-        if should_fail:
-            self.dataset_populator._summarize_history(run.history_id)
-            raise Exception("Expected run to fail but it didn't.")
+    def _output_name_to_object(self, output_name):
+        invocation_response = self.dataset_populator._get(f"invocations/{self.invocation_id}")
+        api_asserts.assert_status_code_is(invocation_response, 200)
+        invocation = invocation_response.json()
+        return invocation_to_output(invocation, self.history_id, output_name)
 
-        expected_outputs = test["output"]
-        try:
-            for key, value in expected_outputs.items():
-                actual_output = run.get_output_as_object(key)
-                cwltest.compare(value, actual_output)
-        except Exception:
-            self.dataset_populator._summarize_history(run.history_id)
-            raise
+    def wait(self):
+        self.workflow_populator.wait_for_invocation_and_jobs(self.history_id, self.workflow_id, self.invocation_id)
 
 
 class BasePopulator(metaclass=ABCMeta):
-
     galaxy_interactor: ApiTestInteractor
 
     @abstractmethod
     def _post(self, route, data=None, files=None, headers=None, admin=False, json: bool = False) -> Response:
         """POST data to target Galaxy instance on specified route."""
 
     @abstractmethod
@@ -445,101 +349,236 @@
     def _get(self, route, data=None, headers=None, admin=False) -> Response:
         """GET data from target Galaxy instance on specified route."""
 
     @abstractmethod
     def _delete(self, route, data=None, headers=None, admin=False, json: bool = False) -> Response:
         """DELETE against target Galaxy instance on specified route."""
 
+    def _get_to_tempfile(self, route, suffix=None, **kwd) -> str:
+        """Perform a _get and store the result in a tempfile."""
+        get_response = self._get(route, **kwd)
+        get_response.raise_for_status()
+        temp_file = tempfile.NamedTemporaryFile("wb", delete=False, suffix=suffix)
+        temp_file.write(get_response.content)
+        temp_file.flush()
+        return temp_file.name
+
 
 class BaseDatasetPopulator(BasePopulator):
-    """ Abstract description of API operations optimized for testing
+    """Abstract description of API operations optimized for testing
     Galaxy - implementations must implement _get, _post and _delete.
     """
 
-    def new_dataset(self, history_id: str, content=None, wait: bool = False, **kwds) -> dict:
-        """Create a new history dataset instance (HDA) and return its ID.
+    def new_dataset(
+        self,
+        history_id: str,
+        content=None,
+        wait: bool = False,
+        fetch_data=True,
+        to_posix_lines=True,
+        auto_decompress=True,
+        **kwds,
+    ) -> Dict[str, Any]:
+        """Create a new history dataset instance (HDA).
 
-        :returns: the HDA id of the new object
+        :returns: a dictionary describing the new HDA
         """
-        run_response = self.new_dataset_request(history_id, content=content, wait=wait, **kwds)
+        run_response = self.new_dataset_request(
+            history_id,
+            content=content,
+            wait=wait,
+            fetch_data=fetch_data,
+            to_posix_lines=to_posix_lines,
+            auto_decompress=auto_decompress,
+            **kwds,
+        )
         assert run_response.status_code == 200, f"Failed to create new dataset with response: {run_response.text}"
+        if fetch_data and wait:
+            return self.get_history_dataset_details_raw(
+                history_id=history_id, dataset_id=run_response.json()["outputs"][0]["id"]
+            ).json()
         return run_response.json()["outputs"][0]
 
-    def new_dataset_request(self, history_id: str, content=None, wait: bool = False, **kwds) -> requests.Response:
-        """Lower-level dataset creation that returns the upload tool response object.
-        """
+    def new_dataset_request(
+        self, history_id: str, content=None, wait: bool = False, fetch_data=True, **kwds
+    ) -> Response:
+        """Lower-level dataset creation that returns the upload tool response object."""
         if content is None and "ftp_files" not in kwds:
             content = "TestData123"
-        payload = self.upload_payload(history_id, content=content, **kwds)
-        run_response = self.tools_post(payload)
+        if not fetch_data:
+            payload = self.upload_payload(history_id, content=content, **kwds)
+            run_response = self.tools_post(payload)
+        else:
+            payload = self.fetch_payload(history_id, content=content, **kwds)
+            run_response = self.fetch(payload, wait=wait)
         if wait:
-            self.wait_for_tool_run(history_id, run_response, assert_ok=kwds.get('assert_ok', True))
+            self.wait_for_tool_run(history_id, run_response, assert_ok=kwds.get("assert_ok", True))
         return run_response
 
-    def fetch(self, payload: dict, assert_ok: bool = True, timeout: timeout_type = DEFAULT_TIMEOUT, wait: Optional[bool] = None):
-        tool_response = self._post("tools/fetch", data=payload)
+    def fetch(
+        self,
+        payload: dict,
+        assert_ok: bool = True,
+        timeout: timeout_type = DEFAULT_TIMEOUT,
+        wait: Optional[bool] = None,
+    ):
+        tool_response = self._post("tools/fetch", data=payload, json=True)
         if wait is None:
             wait = assert_ok
         if wait:
             job = self.check_run(tool_response)
             self.wait_for_job(job["id"], timeout=timeout)
             if assert_ok:
                 job = tool_response.json()["jobs"][0]
                 details = self.get_job_details(job["id"]).json()
                 assert details["state"] == "ok", details
 
         return tool_response
 
     def fetch_hdas(self, history_id: str, items: List[Dict[str, Any]], wait: bool = True) -> List[Dict[str, Any]]:
         destination = {"type": "hdas"}
-        targets = [{
-            "destination": destination,
-            "items": items,
-        }]
+        targets = [
+            {
+                "destination": destination,
+                "items": items,
+            }
+        ]
         payload = {
             "history_id": history_id,
-            "targets": json.dumps(targets),
+            "targets": targets,
         }
         fetch_response = self.fetch(payload, wait=wait)
         api_asserts.assert_status_code_is(fetch_response, 200)
         outputs = fetch_response.json()["outputs"]
         return outputs
 
-    def fetch_hda(self, history_id, item: Dict[str, Any], wait: bool = True) -> Dict[str, Any]:
+    def fetch_hda(self, history_id: str, item: Dict[str, Any], wait: bool = True) -> Dict[str, Any]:
         hdas = self.fetch_hdas(history_id, [item], wait=wait)
         assert len(hdas) == 1
         return hdas[0]
 
+    def create_deferred_hda(self, history_id, uri: str, ext: Optional[str] = None) -> Dict[str, Any]:
+        item = {
+            "src": "url",
+            "url": uri,
+            "deferred": True,
+        }
+        if ext:
+            item["ext"] = ext
+        output = self.fetch_hda(history_id, item)
+        details = self.get_history_dataset_details(history_id, dataset=output)
+        return details
+
     def tag_dataset(self, history_id, hda_id, tags):
         url = f"histories/{history_id}/contents/{hda_id}"
-        response = self._put(url, {'tags': tags}, json=True)
+        response = self._put(url, {"tags": tags}, json=True)
         response.raise_for_status()
         return response.json()
 
-    def wait_for_tool_run(self, history_id: str, run_response: requests.Response, timeout: timeout_type = DEFAULT_TIMEOUT, assert_ok: bool = True):
+    def create_from_store_raw(self, payload: Dict[str, Any]) -> Response:
+        create_response = self._post("histories/from_store", payload, json=True)
+        return create_response
+
+    def create_from_store_raw_async(self, payload: Dict[str, Any]) -> Response:
+        create_response = self._post("histories/from_store_async", payload, json=True)
+        return create_response
+
+    def create_from_store(
+        self,
+        store_dict: Optional[Dict[str, Any]] = None,
+        store_path: Optional[str] = None,
+        model_store_format: Optional[str] = None,
+    ) -> Dict[str, Any]:
+        payload = _store_payload(store_dict=store_dict, store_path=store_path, model_store_format=model_store_format)
+        create_response = self.create_from_store_raw(payload)
+        api_asserts.assert_status_code_is_ok(create_response)
+        return create_response.json()
+
+    def create_from_store_async(
+        self,
+        store_dict: Optional[Dict[str, Any]] = None,
+        store_path: Optional[str] = None,
+        model_store_format: Optional[str] = None,
+    ) -> Dict[str, Any]:
+        payload = _store_payload(store_dict=store_dict, store_path=store_path, model_store_format=model_store_format)
+        create_response = self.create_from_store_raw_async(payload)
+        create_response.raise_for_status()
+        return create_response.json()
+
+    def create_contents_from_store_raw(self, history_id: str, payload: Dict[str, Any]) -> Response:
+        create_response = self._post(f"histories/{history_id}/contents_from_store", payload, json=True)
+        return create_response
+
+    def create_contents_from_store(
+        self, history_id: str, store_dict: Optional[Dict[str, Any]] = None, store_path: Optional[str] = None
+    ) -> List[Dict[str, Any]]:
+        if store_dict is not None:
+            assert isinstance(store_dict, dict)
+        if store_path is not None:
+            assert isinstance(store_path, str)
+        payload = _store_payload(store_dict=store_dict, store_path=store_path)
+        create_response = self.create_contents_from_store_raw(history_id, payload)
+        create_response.raise_for_status()
+        return create_response.json()
+
+    def download_contents_to_store(self, history_id: str, history_content: Dict[str, Any], extension=".tgz") -> str:
+        url = f"histories/{history_id}/contents/{history_content['history_content_type']}s/{history_content['id']}/prepare_store_download"
+        download_response = self._post(url, dict(include_files=False, model_store_format=extension), json=True)
+        storage_request_id = self.assert_download_request_ok(download_response)
+        self.wait_for_download_ready(storage_request_id)
+        return self._get_to_tempfile(f"short_term_storage/{storage_request_id}")
+
+    def reupload_contents(self, history_content: Dict[str, Any]):
+        history_id = history_content["history_id"]
+        temp_tar = self.download_contents_to_store(history_id, history_content, "tgz")
+        with tarfile.open(name=temp_tar) as tf:
+            assert "datasets_attrs.txt" in tf.getnames()
+        new_history_id = self.new_history()
+        as_list = self.create_contents_from_store(
+            new_history_id,
+            store_path=temp_tar,
+        )
+        return new_history_id, as_list
+
+    def wait_for_tool_run(
+        self,
+        history_id: str,
+        run_response: Response,
+        timeout: timeout_type = DEFAULT_TIMEOUT,
+        assert_ok: bool = True,
+    ):
         job = self.check_run(run_response)
         self.wait_for_job(job["id"], timeout=timeout)
         self.wait_for_history(history_id, assert_ok=assert_ok, timeout=timeout)
         return run_response
 
-    def check_run(self, run_response: requests.Response) -> dict:
-        run = run_response.json()
-        assert run_response.status_code == 200, run
+    def check_run(self, run_response: Response) -> dict:
+        run = None
+        try:
+            run = run_response.json()
+            run_response.raise_for_status()
+        except Exception:
+            if run and run["err_msg"]:
+                raise Exception(run["err_msg"])
+            raise
         job = run["jobs"][0]
         return job
 
-    def wait_for_history(self, history_id: str, assert_ok: bool = False, timeout: timeout_type = DEFAULT_TIMEOUT) -> str:
+    def wait_for_history(
+        self, history_id: str, assert_ok: bool = False, timeout: timeout_type = DEFAULT_TIMEOUT
+    ) -> str:
         try:
-            return wait_on_state(lambda: self._get(f"histories/{history_id}"), desc="history state", assert_ok=assert_ok, timeout=timeout)
+            return wait_on_state(
+                lambda: self._get(f"histories/{history_id}"), desc="history state", assert_ok=assert_ok, timeout=timeout
+            )
         except AssertionError:
             self._summarize_history(history_id)
             raise
 
     def wait_for_history_jobs(self, history_id: str, assert_ok: bool = False, timeout: timeout_type = DEFAULT_TIMEOUT):
-
         def has_active_jobs():
             active_jobs = self.active_history_jobs(history_id)
             if len(active_jobs) == 0:
                 return True
             else:
                 return None
 
@@ -549,47 +588,120 @@
             jobs = self.history_jobs(history_id)
             message = f"Failed waiting on active jobs to complete, current jobs are [{jobs}]. {e}"
             raise TimeoutAssertionError(message)
 
         if assert_ok:
             self.wait_for_history(history_id, assert_ok=True, timeout=timeout)
 
-    def wait_for_job(self, job_id: str, assert_ok: bool = False, timeout: timeout_type = DEFAULT_TIMEOUT):
-        return wait_on_state(lambda: self.get_job_details(job_id, full=True), desc="job state", assert_ok=assert_ok, timeout=timeout)
+    def wait_for_jobs(
+        self,
+        jobs: Union[List[dict], List[str]],
+        assert_ok: bool = False,
+        timeout: timeout_type = DEFAULT_TIMEOUT,
+        ok_states=None,
+    ):
+        for job in jobs:
+            if isinstance(job, dict):
+                job_id = job["id"]
+            else:
+                job_id = job
+            self.wait_for_job(job_id, assert_ok=assert_ok, timeout=timeout, ok_states=ok_states)
+
+    def wait_for_job(
+        self, job_id: str, assert_ok: bool = False, timeout: timeout_type = DEFAULT_TIMEOUT, ok_states=None
+    ):
+        return wait_on_state(
+            lambda: self.get_job_details(job_id, full=True),
+            desc="job state",
+            assert_ok=assert_ok,
+            timeout=timeout,
+            ok_states=ok_states,
+        )
 
     def get_job_details(self, job_id: str, full: bool = False) -> Response:
         return self._get(f"jobs/{job_id}", {"full": full})
 
+    def compute_hash(
+        self,
+        dataset_id: str,
+        hash_function: Optional[str] = "MD5",
+        extra_files_path: Optional[str] = None,
+        wait: bool = True,
+    ) -> Response:
+        data: Dict[str, Any] = dict()
+        if hash_function:
+            data["hash_function"] = hash_function
+        if extra_files_path:
+            data["extra_files_path"] = extra_files_path
+        put_response = self._put(f"datasets/{dataset_id}/hash", data, json=True)
+        api_asserts.assert_status_code_is_ok(put_response)
+        if wait:
+            self.wait_on_task(put_response)
+        return put_response
+
     def cancel_history_jobs(self, history_id: str, wait=True) -> None:
         active_jobs = self.active_history_jobs(history_id)
         for active_job in active_jobs:
             self.cancel_job(active_job["id"])
 
     def history_jobs(self, history_id: str) -> List[Dict[str, Any]]:
         query_params = {"history_id": history_id, "order_by": "create_time"}
         jobs_response = self._get("jobs", query_params)
         assert jobs_response.status_code == 200
         return jobs_response.json()
 
+    def invocation_jobs(self, invocation_id: str) -> List[Dict[str, Any]]:
+        query_params = {"invocation_id": invocation_id, "order_by": "create_time"}
+        jobs_response = self._get("jobs", query_params)
+        assert jobs_response.status_code == 200
+        return jobs_response.json()
+
     def active_history_jobs(self, history_id: str) -> list:
         all_history_jobs = self.history_jobs(history_id)
         active_jobs = [j for j in all_history_jobs if j["state"] in ["new", "upload", "waiting", "queued", "running"]]
         return active_jobs
 
     def cancel_job(self, job_id: str) -> Response:
         return self._delete(f"jobs/{job_id}")
 
     def delete_history(self, history_id: str) -> None:
         delete_response = self._delete(f"histories/{history_id}")
         delete_response.raise_for_status()
 
-    def delete_dataset(self, history_id: str, content_id: str, purge: bool = False) -> Response:
-        delete_response = self._delete(f"histories/{history_id}/contents/{content_id}", {'purge': purge}, json=True)
+    def delete_dataset(
+        self,
+        history_id: str,
+        content_id: str,
+        purge: bool = False,
+        stop_job: bool = False,
+        wait_for_purge: bool = False,
+        use_query_params: bool = False,
+    ) -> Response:
+        dataset_url = f"histories/{history_id}/contents/{content_id}"
+        if use_query_params:
+            delete_response = self._delete(f"{dataset_url}?purge={purge}&stop_job={stop_job}")
+        else:
+            delete_response = self._delete(dataset_url, {"purge": purge, "stop_job": stop_job}, json=True)
+        delete_response.raise_for_status()
+        if wait_for_purge and delete_response.status_code == 202:
+            return self.wait_for_purge(history_id, content_id)
         return delete_response
 
+    def wait_for_purge(self, history_id, content_id):
+        dataset_url = f"histories/{history_id}/contents/{content_id}"
+
+        def _wait_for_purge():
+            dataset_response = self._get(dataset_url)
+            dataset_response.raise_for_status()
+            dataset = dataset_response.json()
+            return dataset.get("purged") or None
+
+        wait_on(_wait_for_purge, "dataset to become purged", timeout=2)
+        return self._get(dataset_url)
+
     def create_tool_from_path(self, tool_path: str) -> Dict[str, Any]:
         tool_directory = os.path.dirname(os.path.abspath(tool_path))
         payload = dict(
             src="from_path",
             path=tool_path,
             tool_directory=tool_directory,
         )
@@ -601,151 +713,212 @@
         payload = dict(
             representation=representation,
             tool_directory=tool_directory,
         )
         return self._create_tool_raw(payload)
 
     def _create_tool_raw(self, payload) -> Dict[str, Any]:
+        using_requirement("admin")
         try:
             create_response = self._post("dynamic_tools", data=payload, admin=True)
         except TypeError:
             create_response = self._post("dynamic_tools", data=payload)
         assert create_response.status_code == 200, create_response.text
         return create_response.json()
 
     def list_dynamic_tools(self) -> list:
+        using_requirement("admin")
         list_response = self._get("dynamic_tools", admin=True)
         assert list_response.status_code == 200, list_response
         return list_response.json()
 
     def show_dynamic_tool(self, uuid) -> dict:
+        using_requirement("admin")
         show_response = self._get(f"dynamic_tools/{uuid}", admin=True)
         assert show_response.status_code == 200, show_response
         return show_response.json()
 
     def deactivate_dynamic_tool(self, uuid) -> dict:
+        using_requirement("admin")
         delete_response = self._delete(f"dynamic_tools/{uuid}", admin=True)
         return delete_response.json()
 
+    @abstractmethod
     def _summarize_history(self, history_id: str) -> None:
         """Abstract method for summarizing a target history - override to provide details."""
 
+    def _cleanup_history(self, history_id: str) -> None:
+        self.cancel_history_jobs(history_id)
+
     @contextlib.contextmanager
-    def test_history(self, cancel_executions: bool = True, require_new: bool = True, **kwds):
-        cleanup = "GALAXY_TEST_NO_CLEANUP" not in os.environ
-        history_id = None
-
-        def wrap_up():
-            if cleanup and cancel_executions and history_id:
-                self.cancel_history_jobs(history_id)
+    def test_history_for(self, method) -> Generator[str, None, None]:
+        require_new_history = has_requirement(method, "new_history")
+        with self.test_history(require_new=require_new_history) as history_id:
+            yield history_id
 
-        try:
-            if not require_new:
-                history_id = kwds.get("GALAXY_TEST_HISTORY_ID", None)
+    @contextlib.contextmanager
+    def test_history(self, require_new: bool = True) -> Generator[str, None, None]:
+        with self._test_history(require_new=require_new, cleanup_callback=self._cleanup_history) as history_id:
+            yield history_id
 
-            history_id = history_id or self.new_history()
+    @contextlib.contextmanager
+    def _test_history(
+        self, require_new: bool = True, cleanup_callback: Optional[Callable[[str], None]] = None
+    ) -> Generator[str, None, None]:
+        history_id = self.new_history()
+        try:
             yield history_id
-            wrap_up()
         except Exception:
-            if history_id:
-                self._summarize_history(history_id)
-            wrap_up()
-            raise
+            cleanup_callback and cleanup_callback(history_id)
 
     def new_history(self, name="API Test History", **kwds) -> str:
         create_history_response = self._post("histories", data=dict(name=name))
         assert "id" in create_history_response.json(), create_history_response.text
         history_id = create_history_response.json()["id"]
         return history_id
 
     def copy_history(self, history_id, name="API Test Copied History", **kwds) -> Response:
         return self._post("histories", data={"name": name, "history_id": history_id, **kwds})
 
+    def fetch_payload(
+        self,
+        history_id: str,
+        content: str,
+        auto_decompress: bool = False,
+        file_type: str = "txt",
+        dbkey: str = "?",
+        name: str = "Test_Dataset",
+        **kwds,
+    ) -> dict:
+        __files = {}
+        element = {
+            "ext": file_type,
+            "dbkey": dbkey,
+            "name": name,
+            "auto_decompress": auto_decompress,
+        }
+        for arg in ["to_posix_lines", "space_to_tab"]:
+            val = kwds.get(arg)
+            if val:
+                element[arg] = val
+        target = {
+            "destination": {"type": "hdas"},
+            "elements": [element],
+        }
+        if "ftp_files" in kwds:
+            element["src"] = "ftp_import"
+            element["ftp_path"] = kwds["ftp_files"]
+        elif hasattr(content, "read"):
+            element["src"] = "files"
+            __files["files_0|file_data"] = content
+        elif content and "://" in content:
+            element["src"] = "url"
+            element["url"] = content
+        else:
+            element["src"] = "pasted"
+            element["paste_content"] = content
+        targets = [target]
+        payload = {"history_id": history_id, "targets": targets, "__files": __files}
+        return payload
+
     def upload_payload(self, history_id: str, content: Optional[str] = None, **kwds) -> dict:
         name = kwds.get("name", "Test_Dataset")
         dbkey = kwds.get("dbkey", "?")
-        file_type = kwds.get("file_type", 'txt')
+        file_type = kwds.get("file_type", "txt")
         upload_params = {
-            'files_0|NAME': name,
-            'dbkey': dbkey,
-            'file_type': file_type,
+            "files_0|NAME": name,
+            "dbkey": dbkey,
+            "file_type": file_type,
         }
         if dbkey is None:
             del upload_params["dbkey"]
         if content is None:
             upload_params["files_0|ftp_files"] = kwds.get("ftp_files")
-        elif hasattr(content, 'read'):
+        elif hasattr(content, "read"):
             upload_params["files_0|file_data"] = content
         else:
-            upload_params['files_0|url_paste'] = content
+            upload_params["files_0|url_paste"] = content
 
         if "to_posix_lines" in kwds:
             upload_params["files_0|to_posix_lines"] = kwds["to_posix_lines"]
         if "space_to_tab" in kwds:
             upload_params["files_0|space_to_tab"] = kwds["space_to_tab"]
         if "auto_decompress" in kwds:
             upload_params["files_0|auto_decompress"] = kwds["auto_decompress"]
         upload_params.update(kwds.get("extra_inputs", {}))
         return self.run_tool_payload(
-            tool_id='upload1',
-            inputs=upload_params,
-            history_id=history_id,
-            upload_type='upload_dataset'
+            tool_id="upload1", inputs=upload_params, history_id=history_id, upload_type="upload_dataset"
         )
 
     def get_remote_files(self, target: str = "ftp") -> dict:
         response = self._get("remote_files", data={"target": target})
         response.raise_for_status()
         return response.json()
 
-    def run_tool_payload(self, tool_id: str, inputs: dict, history_id: str, **kwds) -> dict:
+    def run_tool_payload(self, tool_id: Optional[str], inputs: dict, history_id: str, **kwds) -> dict:
         # Remove files_%d|file_data parameters from inputs dict and attach
         # as __files dictionary.
         for key, value in list(inputs.items()):
             if key.startswith("files_") and key.endswith("|file_data"):
                 if "__files" not in kwds:
                     kwds["__files"] = {}
                 kwds["__files"][key] = value
                 del inputs[key]
 
-        return dict(
-            tool_id=tool_id,
-            inputs=json.dumps(inputs),
-            history_id=history_id,
-            **kwds
-        )
+        return dict(tool_id=tool_id, inputs=json.dumps(inputs), history_id=history_id, **kwds)
 
     def build_tool_state(self, tool_id: str, history_id: str):
         response = self._post(f"tools/{tool_id}/build?history_id={history_id}")
         response.raise_for_status()
         return response.json()
 
-    def run_tool_raw(self, tool_id: str, inputs: dict, history_id: str, **kwds) -> Response:
+    def run_tool_raw(self, tool_id: Optional[str], inputs: dict, history_id: str, **kwds) -> Response:
         payload = self.run_tool_payload(tool_id, inputs, history_id, **kwds)
         return self.tools_post(payload)
 
     def run_tool(self, tool_id: str, inputs: dict, history_id: str, **kwds):
         tool_response = self.run_tool_raw(tool_id, inputs, history_id, **kwds)
         api_asserts.assert_status_code_is(tool_response, 200)
         return tool_response.json()
 
     def tools_post(self, payload: dict, url="tools") -> Response:
         tool_response = self._post(url, data=payload)
         return tool_response
 
-    def get_history_dataset_content(self, history_id: str, wait=True, filename=None, type='text', raw=False, **kwds):
+    def materialize_dataset_instance(self, history_id: str, id: str, source: str = "hda"):
+        payload: Dict[str, Any]
+        if source == "ldda":
+            url = f"histories/{history_id}/materialize"
+            payload = {
+                "source": "ldda",
+                "content": id,
+            }
+        else:
+            url = f"histories/{history_id}/contents/datasets/{id}/materialize"
+            payload = {}
+        create_response = self._post(url, payload, json=True)
+        api_asserts.assert_status_code_is_ok(create_response)
+        create_response_json = create_response.json()
+        assert "id" in create_response_json
+        return create_response_json
+
+    def get_history_dataset_content(
+        self, history_id: str, wait=True, filename=None, type="text", to_ext=None, raw=False, **kwds
+    ):
         dataset_id = self.__history_content_id(history_id, wait=wait, **kwds)
         data = {}
         if filename:
             data["filename"] = filename
         if raw:
-            data['raw'] = True
+            data["raw"] = True
+        if to_ext is not None:
+            data["to_ext"] = to_ext
         display_response = self._get_contents_request(history_id, f"/{dataset_id}/display", data=data)
         assert display_response.status_code == 200, display_response.text
-        if type == 'text':
+        if type == "text":
             return display_response.text
         else:
             return display_response.content
 
     def get_history_dataset_source_transform_actions(self, history_id: str, **kwd) -> Set[str]:
         details = self.get_history_dataset_details(history_id, **kwd)
         if "sources" not in details:
@@ -759,15 +932,15 @@
         assert "transform" in source_0
         transform = source_0["transform"]
         if transform is None:
             return set()
         assert isinstance(transform, list)
         return {t["action"] for t in transform}
 
-    def get_history_dataset_details(self, history_id: str, **kwds) -> dict:
+    def get_history_dataset_details(self, history_id: str, **kwds) -> Dict[str, Any]:
         dataset_id = self.__history_content_id(history_id, **kwds)
         details_response = self.get_history_dataset_details_raw(history_id, dataset_id)
         details_response.raise_for_status()
         return details_response.json()
 
     def get_history_dataset_details_raw(self, history_id: str, dataset_id: str) -> Response:
         details_response = self._get_contents_request(history_id, f"/datasets/{dataset_id}")
@@ -776,29 +949,30 @@
     def get_history_dataset_extra_files(self, history_id: str, **kwds) -> list:
         dataset_id = self.__history_content_id(history_id, **kwds)
         details_response = self._get_contents_request(history_id, f"/{dataset_id}/extra_files")
         assert details_response.status_code == 200, details_response.content
         return details_response.json()
 
     def get_history_collection_details(self, history_id: str, **kwds) -> dict:
+        kwds["history_content_type"] = "dataset_collection"
         hdca_id = self.__history_content_id(history_id, **kwds)
         details_response = self._get_contents_request(history_id, f"/dataset_collections/{hdca_id}")
         assert details_response.status_code == 200, details_response.content
         return details_response.json()
 
     def run_collection_creates_list(self, history_id: str, hdca_id: str) -> Response:
         inputs = {
             "input1": {"src": "hdca", "id": hdca_id},
         }
         self.wait_for_history(history_id, assert_ok=True)
         return self.run_tool("collection_creates_list", inputs, history_id)
 
     def run_exit_code_from_file(self, history_id: str, hdca_id: str) -> dict:
         exit_code_inputs = {
-            "input": {'batch': True, 'values': [{"src": "hdca", "id": hdca_id}]},
+            "input": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
         }
         response = self.run_tool("exit_code_from_file", exit_code_inputs, history_id)
         self.wait_for_history(history_id, assert_ok=False)
         return response
 
     def __history_content_id(self, history_id: str, wait=True, **kwds) -> str:
         if wait:
@@ -810,54 +984,74 @@
             history_content_id = kwds["dataset_id"]
         elif "content_id" in kwds:
             history_content_id = kwds["content_id"]
         elif "dataset" in kwds:
             history_content_id = kwds["dataset"]["id"]
         else:
             hid = kwds.get("hid", None)  # If not hid, just grab last dataset
-            history_contents = self._get_contents_request(history_id).json()
+            contents_request = self._get_contents_request(history_id)
+            contents_request.raise_for_status()
+            history_contents = contents_request.json()
             if hid:
                 history_content_id = None
                 for history_item in history_contents:
                     if history_item["hid"] == hid:
                         history_content_id = history_item["id"]
                 if history_content_id is None:
                     raise Exception(f"Could not find content with HID [{hid}] in [{history_contents}]")
             else:
                 # No hid specified - just grab most recent element of correct content type
-                if kwds.get('history_content_type'):
-                    history_contents = [c for c in history_contents if c['history_content_type'] == kwds['history_content_type']]
+                if kwds.get("history_content_type"):
+                    history_contents = [
+                        c for c in history_contents if c["history_content_type"] == kwds["history_content_type"]
+                    ]
                 history_content_id = history_contents[-1]["id"]
         return history_content_id
 
+    def get_history_contents(self, history_id: str) -> List[Dict[str, Any]]:
+        contents_response = self._get_contents_request(history_id)
+        contents_response.raise_for_status()
+        return contents_response.json()
+
     def _get_contents_request(self, history_id: str, suffix: str = "", data=None) -> Response:
         if data is None:
             data = {}
         url = f"histories/{history_id}/contents"
         if suffix:
             url = f"{url}{suffix}"
         return self._get(url, data=data)
 
     def ds_entry(self, history_content: dict) -> dict:
-        src = 'hda'
-        if 'history_content_type' in history_content and history_content['history_content_type'] == "dataset_collection":
-            src = 'hdca'
+        src = "hda"
+        if (
+            "history_content_type" in history_content
+            and history_content["history_content_type"] == "dataset_collection"
+        ):
+            src = "hdca"
         return dict(src=src, id=history_content["id"])
 
-    def dataset_storage_info(self, dataset_id: str) -> dict:
-        storage_response = self._get(f"datasets/{dataset_id}/storage")
-        storage_response.raise_for_status()
-        return storage_response.json()
+    def dataset_storage_info(self, dataset_id: str) -> Dict[str, Any]:
+        response = self.dataset_storage_info_raw(dataset_id)
+        response.raise_for_status()
+        return response.json()
+
+    def dataset_storage_info_raw(self, dataset_id: str) -> Response:
+        storage_url = f"datasets/{dataset_id}/storage"
+        get_storage_response = self._get(storage_url)
+        return get_storage_response
 
     def get_roles(self) -> list:
+        using_requirement("admin")
         roles_response = self._get("roles", admin=True)
         assert roles_response.status_code == 200
         return roles_response.json()
 
     def get_configuration(self, admin=False) -> Dict[str, Any]:
+        if admin:
+            using_requirement("admin")
         response = self._get("configuration", admin=admin)
         api_asserts.assert_status_code_is_ok(response)
         configuration = response.json()
         return configuration
 
     def user_email(self) -> str:
         users_response = self._get("users")
@@ -876,47 +1070,59 @@
         roles = self.get_roles()
         users_roles = [r for r in roles if r["name"] == user_email]
         assert len(users_roles) == 1, f"Did not find exactly one role for email {user_email} - {users_roles}"
         role = users_roles[0]
         assert "id" in role, role
         return role["id"]
 
+    def total_disk_usage(self) -> float:
+        response = self._get("users/current")
+        response.raise_for_status()
+        user_object = response.json()
+        assert "total_disk_usage" in user_object
+        return user_object["total_disk_usage"]
+
     def create_role(self, user_ids: list, description: Optional[str] = None) -> dict:
+        using_requirement("admin")
         payload = {
             "name": self.get_random_name(prefix="testpop"),
             "description": description or "Test Role",
             "user_ids": user_ids,
         }
         role_response = self._post("roles", data=payload, admin=True, json=True)
         assert role_response.status_code == 200
         return role_response.json()
 
     def create_quota(self, quota_payload: dict) -> dict:
+        using_requirement("admin")
         quota_response = self._post("quotas", data=quota_payload, admin=True)
         quota_response.raise_for_status()
         return quota_response.json()
 
     def get_quotas(self) -> list:
+        using_requirement("admin")
         quota_response = self._get("quotas", admin=True)
         quota_response.raise_for_status()
         return quota_response.json()
 
     def make_private(self, history_id: str, dataset_id: str) -> dict:
+        using_requirement("admin")
         role_id = self.user_private_role_id()
         # Give manage permission to the user.
         payload = {
             "access": [role_id],
             "manage": [role_id],
         }
         url = f"histories/{history_id}/contents/{dataset_id}/permissions"
         update_response = self._put(url, payload, admin=True, json=True)
         assert update_response.status_code == 200, update_response.content
         return update_response.json()
 
     def make_public(self, history_id: str) -> dict:
+        using_requirement("new_published_objects")
         sharing_response = self._put(f"histories/{history_id}/publish")
         assert sharing_response.status_code == 200
         return sharing_response.json()
 
     def validate_dataset(self, history_id: str, dataset_id: str) -> Dict[str, Any]:
         url = f"histories/{history_id}/contents/{dataset_id}/validate"
         update_response = self._put(url)
@@ -924,43 +1130,42 @@
         return update_response.json()
 
     def validate_dataset_and_wait(self, history_id, dataset_id) -> Optional[str]:
         self.validate_dataset(history_id, dataset_id)
 
         def validated():
             metadata = self.get_history_dataset_details(history_id, dataset_id=dataset_id)
-            validated_state = metadata['validated_state']
-            if validated_state == 'unknown':
+            validated_state = metadata["validated_state"]
+            if validated_state == "unknown":
                 return
             else:
                 return validated_state
 
-        return wait_on(
-            validated,
-            "dataset validation"
-        )
+        return wait_on(validated, "dataset validation")
 
     def setup_history_for_export_testing(self, history_name):
+        using_requirement("new_history")
         history_id = self.new_history(name=history_name)
-        hda = self.new_dataset(history_id, content="1 2 3")
-        tags = ['name:name']
-        response = self.tag_dataset(history_id, hda['id'], tags=tags)
-        assert response['tags'] == tags
+        hda = self.new_dataset(history_id, content="1 2 3", wait=True)
+        tags = ["name:name"]
+        response = self.tag_dataset(history_id, hda["id"], tags=tags)
+        assert response["tags"] == tags
         deleted_hda = self.new_dataset(history_id, content="1 2 3", wait=True)
         self.delete_dataset(history_id, deleted_hda["id"])
         deleted_details = self.get_history_dataset_details(history_id, id=deleted_hda["id"])
         assert deleted_details["deleted"]
         return history_id
 
     def prepare_export(self, history_id, data):
         url = f"histories/{history_id}/exports"
         put_response = self._put(url, data, json=True)
         put_response.raise_for_status()
 
         if put_response.status_code == 202:
+
             def export_ready_response():
                 put_response = self._put(url)
                 if put_response.status_code == 202:
                     return None
                 return put_response
 
             put_response = wait_on(export_ready_response, desc="export ready")
@@ -971,15 +1176,15 @@
             assert "job_id" in job_desc
             return self.wait_for_job(job_desc["job_id"])
 
     def export_url(self, history_id: str, data, check_download: bool = True) -> str:
         put_response = self.prepare_export(history_id, data)
         response = put_response.json()
         api_asserts.assert_has_keys(response, "download_url")
-        download_url = urllib.parse.urljoin(self.galaxy_interactor.api_url, response["download_url"].strip('/'))
+        download_url = urllib.parse.urljoin(self.galaxy_interactor.api_url, response["download_url"].strip("/"))
 
         if check_download:
             self.get_export_url(download_url)
 
         return download_url
 
     def get_export_url(self, export_url) -> Response:
@@ -990,84 +1195,219 @@
     def import_history(self, import_data):
         files = {}
         archive_file = import_data.pop("archive_file", None)
         if archive_file:
             files["archive_file"] = archive_file
         import_response = self._post("histories", data=import_data, files=files)
         api_asserts.assert_status_code_is(import_response, 200)
-        return import_response.json()['id']
+        return import_response.json()["id"]
 
-    def import_history_and_wait_for_name(self, import_data, history_name):
-        def history_names():
-            return {h["name"]: h for h in self.get_histories()}
+    def wait_for_history_with_name(self, history_name: str, desc: str) -> Dict[str, Any]:
+        def has_history_with_name():
+            histories = self.history_names()
+            return histories.get(history_name, None)
+
+        target_history = wait_on(has_history_with_name, desc=desc)
+        return target_history
 
+    def import_history_and_wait_for_name(self, import_data, history_name):
         import_name = f"imported from archive: {history_name}"
-        assert import_name not in history_names()
+        assert import_name not in self.history_names()
 
         job_id = self.import_history(import_data)
         self.wait_for_job(job_id, assert_ok=True)
 
-        def has_history_with_name():
-            histories = history_names()
-            return histories.get(import_name, None)
-
-        imported_history = wait_on(has_history_with_name, desc="import history")
+        imported_history = self.wait_for_history_with_name(import_name, "import history")
         imported_history_id = imported_history["id"]
         self.wait_for_history(imported_history_id)
         return imported_history_id
 
+    def history_names(self) -> Dict[str, Dict]:
+        return {h["name"]: h for h in self.get_histories()}
+
     def rename_history(self, history_id, new_name):
         update_url = f"histories/{history_id}"
         put_response = self._put(update_url, {"name": new_name}, json=True)
         return put_response
 
     def get_histories(self):
         history_index_response = self._get("histories")
         api_asserts.assert_status_code_is(history_index_response, 200)
         return history_index_response.json()
 
-    def wait_on_history_length(self, history_id, wait_on_history_length):
-
+    def wait_on_history_length(self, history_id: str, wait_on_history_length: int):
         def history_has_length():
             history_length = self.history_length(history_id)
             return None if history_length != wait_on_history_length else True
 
         wait_on(history_has_length, desc="import history population")
 
+    def wait_on_download(self, download_request_response: Response) -> Response:
+        storage_request_id = self.assert_download_request_ok(download_request_response)
+        return self.wait_on_download_request(storage_request_id)
+
+    def assert_download_request_ok(self, download_request_response: Response) -> UUID:
+        """Assert response is valid and okay and extract storage request ID."""
+        api_asserts.assert_status_code_is(download_request_response, 200)
+        download_async = download_request_response.json()
+        assert "storage_request_id" in download_async
+        storage_request_id = download_async["storage_request_id"]
+        return storage_request_id
+
+    def wait_for_download_ready(self, storage_request_id: UUID):
+        def is_ready():
+            is_ready_response = self._get(f"short_term_storage/{storage_request_id}/ready")
+            is_ready_response.raise_for_status()
+            is_ready_bool = is_ready_response.json()
+            return True if is_ready_bool else None
+
+        wait_on(is_ready, "waiting for download to become ready")
+        assert is_ready()
+
+    def wait_on_task(self, async_task_response: Response):
+        task_id = async_task_response.json()["id"]
+        return self.wait_on_task_id(task_id)
+
+    def wait_on_task_id(self, task_id: str):
+        def state():
+            state_response = self._get(f"tasks/{task_id}/state")
+            state_response.raise_for_status()
+            return state_response.json()
+
+        def is_ready():
+            is_complete = state() in ["SUCCESS", "FAILURE"]
+            return True if is_complete else None
+
+        wait_on(is_ready, "waiting for task to complete")
+        return state() == "SUCCESS"
+
+    def wait_on_download_request(self, storage_request_id: UUID) -> Response:
+        self.wait_for_download_ready(storage_request_id)
+        download_contents_response = self._get(f"short_term_storage/{storage_request_id}")
+        download_contents_response.raise_for_status()
+        return download_contents_response
+
     def history_length(self, history_id):
         contents_response = self._get(f"histories/{history_id}/contents")
         api_asserts.assert_status_code_is(contents_response, 200)
         contents = contents_response.json()
         return len(contents)
 
-    def reimport_history(self, history_id, history_name, wait_on_history_length, export_kwds):
+    def reimport_history(self, history_id, history_name, wait_on_history_length, export_kwds, task_based=False):
         # Make history public so we can import by url
         self.make_public(history_id)
-        # Export the history.
-        download_url = self.export_url(history_id, export_kwds, check_download=True)
+        if not task_based:
+            # Export the history.
+            full_download_url = self.export_url(history_id, export_kwds, check_download=True)
+        else:
+            # Give modern endpoint the legacy endpoint defaults for kwds...
+            if "include_files" in export_kwds:
+                export_kwds["include_files"] = True
+            if "include_hidden" not in export_kwds:
+                export_kwds["include_hidden"] = True
+            if "include_deleted" not in export_kwds:
+                export_kwds["include_hidden"] = False
+            prepare_download_response = self._post(
+                f"histories/{history_id}/prepare_store_download", export_kwds, json=True
+            )
+            storage_request_id = self.assert_download_request_ok(prepare_download_response)
+            self.wait_for_download_ready(storage_request_id)
+            api_key = self.galaxy_interactor.api_key
+            full_download_url = urllib.parse.urljoin(
+                self.galaxy_interactor.api_url, f"api/short_term_storage/{storage_request_id}?key={api_key}"
+            )
 
-        import_data = dict(archive_source=download_url, archive_type="url")
+        import_data = dict(archive_source=full_download_url, archive_type="url")
 
         imported_history_id = self.import_history_and_wait_for_name(import_data, history_name)
 
         if wait_on_history_length:
             self.wait_on_history_length(imported_history_id, wait_on_history_length)
 
         return imported_history_id
 
-    def get_random_name(self, prefix=None, suffix=None, len=10):
-        # stolen from navigates_galaxy.py
-        return '{}{}{}'.format(
-            prefix or '',
-            ''.join(random.choice(string.ascii_lowercase + string.digits) for _ in range(len)),
-            suffix or '',
+    def get_random_name(self, prefix: Optional[str] = None, suffix: Optional[str] = None, len: int = 10) -> str:
+        return random_name(prefix=prefix, suffix=suffix, len=len)
+
+    def wait_for_dataset(
+        self, history_id: str, dataset_id: str, assert_ok: bool = False, timeout: timeout_type = DEFAULT_TIMEOUT
+    ) -> str:
+        return wait_on_state(
+            lambda: self._get(f"histories/{history_id}/contents/{dataset_id}"),
+            desc="dataset state",
+            assert_ok=assert_ok,
+            timeout=timeout,
+        )
+
+    def new_page(
+        self, slug: str = "mypage", title: str = "MY PAGE", content_format: str = "html", content: Optional[str] = None
+    ) -> Dict[str, Any]:
+        page_response = self.new_page_raw(slug=slug, title=title, content_format=content_format, content=content)
+        page_response.raise_for_status()
+        return page_response.json()
+
+    def new_page_raw(
+        self, slug: str = "mypage", title: str = "MY PAGE", content_format: str = "html", content: Optional[str] = None
+    ) -> Response:
+        page_request = self.new_page_payload(slug=slug, title=title, content_format=content_format, content=content)
+        page_response = self._post("pages", page_request, json=True)
+        return page_response
+
+    def new_page_payload(
+        self, slug: str = "mypage", title: str = "MY PAGE", content_format: str = "html", content: Optional[str] = None
+    ) -> Dict[str, str]:
+        if content is None:
+            if content_format == "html":
+                content = "<p>Page!</p>"
+            else:
+                content = "*Page*\n\n"
+        request = dict(
+            slug=slug,
+            title=title,
+            content=content,
+            content_format=content_format,
         )
+        return request
 
-    def wait_for_dataset(self, history_id, dataset_id, assert_ok=False, timeout=DEFAULT_TIMEOUT):
-        return wait_on_state(lambda: self._get(f"histories/{history_id}/contents/{dataset_id}"), desc="dataset state", assert_ok=assert_ok, timeout=timeout)
+    def export_history_to_uri_async(
+        self, history_id: str, target_uri: str, model_store_format: str = "tgz", include_files: bool = True
+    ):
+        url = f"histories/{history_id}/write_store"
+        download_response = self._post(
+            url,
+            dict(target_uri=target_uri, include_files=include_files, model_store_format=model_store_format),
+            json=True,
+        )
+        api_asserts.assert_status_code_is_ok(download_response)
+        task_ok = self.wait_on_task(download_response)
+        assert task_ok, f"Task: Writing history to {target_uri} task failed"
+
+    def import_history_from_uri_async(self, target_uri: str, model_store_format: str):
+        import_async_response = self.create_from_store_async(
+            store_path=target_uri, model_store_format=model_store_format
+        )
+        task_id = import_async_response["id"]
+        task_ok = self.wait_on_task_id(task_id)
+        assert task_ok, f"Task: Import history from {target_uri} failed"
+
+    def download_history_to_store(self, history_id: str, extension: str = "tgz", serve_file: bool = False):
+        url = f"histories/{history_id}/prepare_store_download"
+        download_response = self._post(url, dict(include_files=False, model_store_format=extension), json=True)
+        storage_request_id = self.assert_download_request_ok(download_response)
+        self.wait_for_download_ready(storage_request_id)
+        if serve_file:
+            return self._get_to_tempfile(f"short_term_storage/{storage_request_id}")
+        else:
+            return storage_request_id
+
+    def get_history_export_tasks(self, history_id: str):
+        headers = {"accept": "application/vnd.galaxy.task.export+json"}
+        response = self._get(f"histories/{history_id}/exports", headers=headers)
+        api_asserts.assert_status_code_is_ok(response)
+        return response.json()
 
 
 class GalaxyInteractorHttpMixin:
     galaxy_interactor: ApiTestInteractor
 
     @property
     def _api_key(self):
@@ -1089,25 +1429,37 @@
         if data is None:
             data = {}
 
         return self.galaxy_interactor.delete(route, data=data, headers=headers, admin=admin, json=json)
 
 
 class DatasetPopulator(GalaxyInteractorHttpMixin, BaseDatasetPopulator):
-
-    def __init__(self, galaxy_interactor):
+    def __init__(self, galaxy_interactor: ApiTestInteractor) -> None:
         self.galaxy_interactor = galaxy_interactor
 
     def _summarize_history(self, history_id):
         self.galaxy_interactor._summarize_history(history_id)
 
+    @contextlib.contextmanager
+    def _test_history(
+        self, require_new: bool = True, cleanup_callback: Optional[Callable[[str], None]] = None
+    ) -> Generator[str, None, None]:
+        with self.galaxy_interactor.test_history(
+            require_new=require_new, cleanup_callback=cleanup_callback
+        ) as history_id:
+            yield history_id
+
+
+# Things gxformat2 knows how to upload as workflows
+YamlContentT = Union[str, os.PathLike, dict]
+
 
 class BaseWorkflowPopulator(BasePopulator):
     dataset_populator: BaseDatasetPopulator
-    dataset_collection_populator: 'BaseDatasetCollectionPopulator'
+    dataset_collection_populator: "BaseDatasetCollectionPopulator"
 
     def load_workflow(self, name: str, content: str = workflow_str, add_pja=False) -> dict:
         workflow = json.loads(content)
         workflow["name"] = name
         if add_pja:
             tool_step = workflow["steps"]["2"]
             tool_step["post_job_actions"]["RenameDatasetActionout_file1"] = dict(
@@ -1145,356 +1497,537 @@
 
     def create_workflow(self, workflow: Dict[str, Any], **create_kwds) -> str:
         upload_response = self.create_workflow_response(workflow, **create_kwds)
         uploaded_workflow_id = upload_response.json()["id"]
         return uploaded_workflow_id
 
     def create_workflow_response(self, workflow: Dict[str, Any], **create_kwds) -> Response:
-        data = dict(
-            workflow=json.dumps(workflow),
-            **create_kwds
-        )
+        data = dict(workflow=json.dumps(workflow), **create_kwds)
         upload_response = self._post("workflows/upload", data=data)
         return upload_response
 
-    def upload_yaml_workflow(self, has_yaml, **kwds) -> str:
+    def upload_yaml_workflow(self, yaml_content: YamlContentT, **kwds) -> str:
         round_trip_conversion = kwds.get("round_trip_format_conversion", False)
         client_convert = kwds.pop("client_convert", not round_trip_conversion)
         kwds["convert"] = client_convert
-        workflow = convert_and_import_workflow(has_yaml, galaxy_interface=self, **kwds)
+        workflow = convert_and_import_workflow(yaml_content, galaxy_interface=self, **kwds)
         workflow_id = workflow["id"]
         if round_trip_conversion:
             workflow_yaml_wrapped = self.download_workflow(workflow_id, style="format2_wrapped_yaml")
             assert "yaml_content" in workflow_yaml_wrapped, workflow_yaml_wrapped
             round_trip_converted_content = workflow_yaml_wrapped["yaml_content"]
-            workflow_id = self.upload_yaml_workflow(round_trip_converted_content, client_convert=False, round_trip_conversion=False)
+            workflow_id = self.upload_yaml_workflow(
+                round_trip_converted_content, client_convert=False, round_trip_conversion=False
+            )
 
         return workflow_id
 
-    def wait_for_invocation(self, workflow_id: str, invocation_id: str, timeout: timeout_type = DEFAULT_TIMEOUT, assert_ok: bool = True):
-        url = f"workflows/{workflow_id}/usage/{invocation_id}"
+    def wait_for_invocation(
+        self, workflow_id: str, invocation_id: str, timeout: timeout_type = DEFAULT_TIMEOUT, assert_ok: bool = True
+    ) -> str:
+        url = f"invocations/{invocation_id}"
 
         def workflow_state():
             return self._get(url)
 
         return wait_on_state(workflow_state, desc="workflow invocation state", timeout=timeout, assert_ok=assert_ok)
 
-    def history_invocations(self, history_id: str) -> list:
+    def workflow_invocations(self, workflow_id: str) -> List[Dict[str, Any]]:
+        response = self._get(f"workflows/{workflow_id}/invocations")
+        api_asserts.assert_status_code_is(response, 200)
+        return response.json()
+
+    def history_invocations(self, history_id: str) -> List[Dict[str, Any]]:
         history_invocations_response = self._get("invocations", {"history_id": history_id})
         api_asserts.assert_status_code_is(history_invocations_response, 200)
         return history_invocations_response.json()
 
-    def wait_for_history_workflows(self, history_id, assert_ok=True, timeout=DEFAULT_TIMEOUT, expected_invocation_count=None):
+    def wait_for_history_workflows(
+        self,
+        history_id: str,
+        assert_ok: bool = True,
+        timeout: timeout_type = DEFAULT_TIMEOUT,
+        expected_invocation_count: Optional[int] = None,
+    ) -> None:
         if expected_invocation_count is not None:
+
             def invocation_count():
                 invocations = self.history_invocations(history_id)
                 if len(invocations) == expected_invocation_count:
                     return True
 
             wait_on(invocation_count, f"{expected_invocation_count} history invocations")
         for invocation in self.history_invocations(history_id):
             workflow_id = invocation["workflow_id"]
             invocation_id = invocation["id"]
             self.wait_for_workflow(workflow_id, invocation_id, history_id, timeout=timeout, assert_ok=assert_ok)
 
-    def wait_for_workflow(self, workflow_id, invocation_id, history_id, assert_ok=True, timeout=DEFAULT_TIMEOUT):
-        """ Wait for a workflow invocation to completely schedule and then history
-        to be complete. """
+    def wait_for_workflow(
+        self,
+        workflow_id: str,
+        invocation_id: str,
+        history_id: str,
+        assert_ok: bool = True,
+        timeout: timeout_type = DEFAULT_TIMEOUT,
+    ) -> None:
+        """Wait for a workflow invocation to completely schedule and then history
+        to be complete."""
         self.wait_for_invocation(workflow_id, invocation_id, timeout=timeout, assert_ok=assert_ok)
         self.dataset_populator.wait_for_history_jobs(history_id, assert_ok=assert_ok, timeout=timeout)
 
     def get_invocation(self, invocation_id, step_details=False):
-        r = self._get(f"invocations/{invocation_id}", data={'step_details': step_details})
+        r = self._get(f"invocations/{invocation_id}", data={"step_details": step_details})
         r.raise_for_status()
         return r.json()
 
+    def download_invocation_to_store(self, invocation_id, include_files=False, extension="tgz"):
+        url = f"invocations/{invocation_id}/prepare_store_download"
+        download_response = self._post(url, dict(include_files=include_files, model_store_format=extension), json=True)
+        storage_request_id = self.dataset_populator.assert_download_request_ok(download_response)
+        self.dataset_populator.wait_for_download_ready(storage_request_id)
+        return self._get_to_tempfile(f"short_term_storage/{storage_request_id}")
+
+    def download_invocation_to_uri(self, invocation_id, target_uri, extension="tgz"):
+        url = f"invocations/{invocation_id}/write_store"
+        download_response = self._post(
+            url, dict(target_uri=target_uri, include_files=False, model_store_format=extension), json=True
+        )
+        api_asserts.assert_status_code_is_ok(download_response)
+        task_ok = self.dataset_populator.wait_on_task(download_response)
+        assert task_ok, f"waiting on task to write invocation to {target_uri} that failed"
+
+    def create_invocation_from_store_raw(
+        self,
+        history_id: str,
+        store_dict: Optional[Dict[str, Any]] = None,
+        store_path: Optional[str] = None,
+        model_store_format: Optional[str] = None,
+    ) -> Response:
+        url = "invocations/from_store"
+        payload = _store_payload(store_dict=store_dict, store_path=store_path, model_store_format=model_store_format)
+        payload["history_id"] = history_id
+        create_response = self._post(url, payload, json=True)
+        return create_response
+
+    def create_invocation_from_store(
+        self,
+        history_id: str,
+        store_dict: Optional[Dict[str, Any]] = None,
+        store_path: Optional[str] = None,
+        model_store_format: Optional[str] = None,
+    ) -> Response:
+        create_response = self.create_invocation_from_store_raw(
+            history_id, store_dict=store_dict, store_path=store_path, model_store_format=model_store_format
+        )
+        api_asserts.assert_status_code_is_ok(create_response)
+        return create_response.json()
+
     def get_biocompute_object(self, invocation_id):
         bco_response = self._get(f"invocations/{invocation_id}/biocompute")
         bco_response.raise_for_status()
         return bco_response.json()
 
-    def validate_biocompute_object(self, bco, expected_schema_version='https://w3id.org/ieee/ieee-2791-schema/2791object.json'):
-        # TODO: actually use jsonref and jsonschema to validate this someday
-        api_asserts.assert_has_keys(bco, "object_id", "spec_version", "etag", "provenance_domain", "usability_domain", "description_domain", "execution_domain", "parametric_domain", "io_domain", "error_domain")
-        assert bco['spec_version'] == expected_schema_version
-        api_asserts.assert_has_keys(bco['description_domain'], "keywords", "xref", "platform", "pipeline_steps")
-        api_asserts.assert_has_keys(bco['execution_domain'], "script_access_type", "script", "script_driver", "software_prerequisites", "external_data_endpoints", "environment_variables")
-        for p in bco['parametric_domain']:
-            api_asserts.assert_has_keys(p, "param", "value", "step")
-        api_asserts.assert_has_keys(bco['io_domain'], "input_subdomain", "output_subdomain")
+    def validate_biocompute_object(
+        self, bco, expected_schema_version="https://w3id.org/ieee/ieee-2791-schema/2791object.json"
+    ):
+        JsonSchemaValidator.validate_using_schema_url(bco, expected_schema_version)
+
+    def get_ro_crate(self, invocation_id, include_files=False):
+        crate_response = self.download_invocation_to_store(
+            invocation_id=invocation_id, include_files=include_files, extension="rocrate.zip"
+        )
+        return ROCrate(crate_response)
+
+    def validate_invocation_crate_directory(self, crate_directory):
+        # TODO: where can a ro_crate be extracted
+        metadata_json_path = crate_directory / "ro-crate-metadata.json"
+        with metadata_json_path.open() as f:
+            metadata_json = json.load(f)
+            assert metadata_json["@context"] == "https://w3id.org/ro/crate/1.1/context"
 
     def invoke_workflow_raw(self, workflow_id: str, request: dict, assert_ok: bool = False) -> Response:
         url = f"workflows/{workflow_id}/invocations"
         invocation_response = self._post(url, data=request)
         if assert_ok:
             invocation_response.raise_for_status()
         return invocation_response
 
-    def invoke_workflow(self, workflow_id: str, history_id: Optional[str] = None, inputs: Optional[dict] = None, request: Optional[dict] = None, assert_ok: bool = True, inputs_by: str = 'step_index'):
+    def invoke_workflow(
+        self,
+        workflow_id: str,
+        history_id: Optional[str] = None,
+        inputs: Optional[dict] = None,
+        request: Optional[dict] = None,
+        inputs_by: str = "step_index",
+    ) -> Response:
         if inputs is None:
             inputs = {}
 
         if request is None:
             request = {}
 
         if history_id:
             request["history"] = f"hist_id={history_id}"
         # else history may be in request...
 
         if inputs:
             request["inputs"] = json.dumps(inputs)
             request["inputs_by"] = inputs_by
         invocation_response = self.invoke_workflow_raw(workflow_id, request)
-        if assert_ok:
-            api_asserts.assert_status_code_is(invocation_response, 200)
-            invocation_id = invocation_response.json()["id"]
-            return invocation_id
-        else:
-            return invocation_response
+        return invocation_response
 
-    def invoke_workflow_and_wait(self, workflow_id: str, history_id: Optional[str] = None, inputs: Optional[dict] = None, request: Optional[dict] = None, assert_ok: bool = True):
-        invoke_return = self.invoke_workflow(workflow_id, history_id=history_id, inputs=inputs, request=request, assert_ok=assert_ok)
-        if assert_ok:
-            invocation_id = invoke_return
-        else:
-            invocation_id = invoke_return.json()["id"]
+    def invoke_workflow_and_assert_ok(
+        self,
+        workflow_id: str,
+        history_id: Optional[str] = None,
+        inputs: Optional[dict] = None,
+        request: Optional[dict] = None,
+        inputs_by: str = "step_index",
+    ) -> str:
+        invocation_response = self.invoke_workflow(
+            workflow_id, history_id=history_id, inputs=inputs, request=request, inputs_by=inputs_by
+        )
+        api_asserts.assert_status_code_is(invocation_response, 200)
+        invocation_id = invocation_response.json()["id"]
+        return invocation_id
+
+    def invoke_workflow_and_wait(
+        self,
+        workflow_id: str,
+        history_id: Optional[str] = None,
+        inputs: Optional[dict] = None,
+        request: Optional[dict] = None,
+    ) -> Response:
+        invoke_return = self.invoke_workflow(workflow_id, history_id=history_id, inputs=inputs, request=request)
+        invoke_return.raise_for_status()
+        invocation_id = invoke_return.json()["id"]
 
         if history_id is None and request:
             history_id = request.get("history_id")
         if history_id is None and request:
             history_id = request["history"]
             if history_id.startswith("hist_id="):
-                history_id = history_id[len("hist_id="):]
-        self.wait_for_workflow(workflow_id, invocation_id, history_id, assert_ok=assert_ok)
+                history_id = history_id[len("hist_id=") :]
+        assert history_id
+        self.wait_for_workflow(workflow_id, invocation_id, history_id, assert_ok=True)
         return invoke_return
 
     def workflow_report_json(self, workflow_id: str, invocation_id: str) -> dict:
         response = self._get(f"workflows/{workflow_id}/invocations/{invocation_id}/report")
         api_asserts.assert_status_code_is(response, 200)
         return response.json()
 
-    def download_workflow(self, workflow_id: str, style: Optional[str] = None, history_id: Optional[str] = None) -> dict:
+    def download_workflow(
+        self, workflow_id: str, style: Optional[str] = None, history_id: Optional[str] = None
+    ) -> dict:
         params = {}
         if style is not None:
             params["style"] = style
         if history_id is not None:
-            params['history_id'] = history_id
+            params["history_id"] = history_id
         response = self._get(f"workflows/{workflow_id}/download", data=params)
         api_asserts.assert_status_code_is(response, 200)
         if style != "format2":
             return response.json()
         else:
             return ordered_load(response.text)
 
+    def set_tags(self, workflow_id: str, tags: List[str]) -> None:
+        update_payload = {"tags": tags}
+        response = self.update_workflow(workflow_id, update_payload)
+        response.raise_for_status()
+
     def update_workflow(self, workflow_id: str, workflow_object: dict) -> Response:
-        data = dict(
-            workflow=workflow_object
-        )
-        raw_url = f'workflows/{workflow_id}'
+        data = dict(workflow=workflow_object)
+        raw_url = f"workflows/{workflow_id}"
         put_response = self._put(raw_url, data, json=True)
         return put_response
 
-    def refactor_workflow(self, workflow_id: str, actions: list, dry_run: Optional[bool] = None, style: Optional[str] = None) -> Response:
+    def refactor_workflow(
+        self, workflow_id: str, actions: list, dry_run: Optional[bool] = None, style: Optional[str] = None
+    ) -> Response:
         data: Dict[str, Any] = dict(
             actions=actions,
         )
         if style is not None:
             data["style"] = style
         if dry_run is not None:
             data["dry_run"] = dry_run
-        raw_url = f'workflows/{workflow_id}/refactor'
+        raw_url = f"workflows/{workflow_id}/refactor"
         put_response = self._put(raw_url, data, json=True)
         return put_response
 
     @contextlib.contextmanager
     def export_for_update(self, workflow_id):
         workflow_object = self.download_workflow(workflow_id)
         yield workflow_object
         put_respose = self.update_workflow(workflow_id, workflow_object)
         put_respose.raise_for_status()
 
-    def run_workflow(self, has_workflow, test_data=None, history_id=None, wait=True, source_type=None, jobs_descriptions=None, expected_response=200, assert_ok=True, client_convert=None, round_trip_format_conversion=False, raw_yaml=False):
+    def run_workflow(
+        self,
+        has_workflow: YamlContentT,
+        test_data: Optional[Union[str, dict]] = None,
+        history_id: Optional[str] = None,
+        wait: bool = True,
+        source_type: Optional[str] = None,
+        jobs_descriptions=None,
+        expected_response: int = 200,
+        assert_ok: bool = True,
+        client_convert: Optional[bool] = None,
+        round_trip_format_conversion: bool = False,
+        invocations: int = 1,
+        raw_yaml: bool = False,
+    ):
         """High-level wrapper around workflow API, etc. to invoke format 2 workflows."""
         workflow_populator = self
         if client_convert is None:
             client_convert = not round_trip_format_conversion
 
         workflow_id = workflow_populator.upload_yaml_workflow(
             has_workflow,
             source_type=source_type,
             client_convert=client_convert,
             round_trip_format_conversion=round_trip_format_conversion,
-            raw_yaml=raw_yaml
+            raw_yaml=raw_yaml,
         )
 
         if test_data is None:
             if jobs_descriptions is None:
                 assert source_type != "path"
-                jobs_descriptions = yaml.safe_load(has_workflow)
-
-            test_data = jobs_descriptions.get("test_data", {})
+                if isinstance(has_workflow, dict):
+                    jobs_descriptions = has_workflow
+                else:
+                    assert isinstance(has_workflow, str)
+                    jobs_descriptions = yaml.safe_load(has_workflow)
 
-        if not isinstance(test_data, dict):
-            test_data = yaml.safe_load(test_data)
+            test_data_dict = jobs_descriptions.get("test_data", {})
+        elif not isinstance(test_data, dict):
+            test_data_dict = yaml.safe_load(test_data)
+        else:
+            test_data_dict = test_data
 
-        parameters = test_data.pop('step_parameters', {})
-        replacement_parameters = test_data.pop("replacement_parameters", {})
+        parameters = test_data_dict.pop("step_parameters", {})
+        replacement_parameters = test_data_dict.pop("replacement_parameters", {})
         if history_id is None:
             history_id = self.dataset_populator.new_history()
-        inputs, label_map, has_uploads = load_data_dict(history_id, test_data, self.dataset_populator, self.dataset_collection_populator)
+        inputs, label_map, has_uploads = load_data_dict(
+            history_id, test_data_dict, self.dataset_populator, self.dataset_collection_populator
+        )
         workflow_request: Dict[str, Any] = dict(
             history=f"hist_id={history_id}",
             workflow_id=workflow_id,
         )
         workflow_request["inputs"] = json.dumps(label_map)
-        workflow_request["inputs_by"] = 'name'
+        workflow_request["inputs_by"] = "name"
         if parameters:
             workflow_request["parameters"] = json.dumps(parameters)
             workflow_request["parameters_normalized"] = True
         if replacement_parameters:
             workflow_request["replacement_params"] = json.dumps(replacement_parameters)
         if has_uploads:
             self.dataset_populator.wait_for_history(history_id, assert_ok=True)
-        invocation_response = workflow_populator.invoke_workflow_raw(workflow_id, workflow_request)
-        api_asserts.assert_status_code_is(invocation_response, expected_response)
-        invocation = invocation_response.json()
-        if expected_response != 200:
-            assert not assert_ok
-            return invocation
-        invocation_id = invocation.get('id')
-        if invocation_id:
-            # Wait for workflow to become fully scheduled and then for all jobs
-            # complete.
-            if wait:
-                workflow_populator.wait_for_workflow(workflow_id, invocation_id, history_id, assert_ok=assert_ok)
-            jobs = self.dataset_populator.history_jobs(history_id)
-            return RunJobsSummary(
-                history_id=history_id,
-                workflow_id=workflow_id,
-                invocation_id=invocation_id,
-                inputs=inputs,
-                jobs=jobs,
-                invocation=invocation,
-                workflow_request=workflow_request
-            )
+        assert invocations > 0
+        jobs = []
+        for _ in range(invocations):
+            invocation_response = workflow_populator.invoke_workflow_raw(workflow_id, workflow_request)
+            api_asserts.assert_status_code_is(invocation_response, expected_response)
+            invocation = invocation_response.json()
+            if expected_response != 200:
+                assert not assert_ok
+                return invocation
+            invocation_id = invocation.get("id")
+            if invocation_id:
+                # Wait for workflow to become fully scheduled and then for all jobs
+                # complete.
+                if wait:
+                    workflow_populator.wait_for_workflow(workflow_id, invocation_id, history_id, assert_ok=assert_ok)
+                jobs.extend(self.dataset_populator.invocation_jobs(invocation_id))
+        return RunJobsSummary(
+            history_id=history_id,
+            workflow_id=workflow_id,
+            invocation_id=invocation_id,
+            inputs=inputs,
+            jobs=jobs,
+            invocation=invocation,
+            workflow_request=workflow_request,
+        )
 
     def dump_workflow(self, workflow_id, style=None):
         raw_workflow = self.download_workflow(workflow_id, style=style)
         if style == "format2_wrapped_yaml":
             print(raw_workflow["yaml_content"])
         else:
             print(json.dumps(raw_workflow, sort_keys=True, indent=2))
 
     def workflow_inputs(self, workflow_id: str) -> Dict[str, Dict[str, Any]]:
-        workflow_show_resposne = self._get(f"workflows/{workflow_id}")
-        api_asserts.assert_status_code_is_ok(workflow_show_resposne)
-        workflow_inputs = workflow_show_resposne.json()["inputs"]
+        workflow_show_response = self._get(f"workflows/{workflow_id}")
+        api_asserts.assert_status_code_is_ok(workflow_show_response)
+        workflow_inputs = workflow_show_response.json()["inputs"]
         return workflow_inputs
 
     def build_ds_map(self, workflow_id: str, label_map: Dict[str, Any]) -> str:
         workflow_inputs = self.workflow_inputs(workflow_id)
         ds_map = {}
         for key, value in workflow_inputs.items():
             label = value["label"]
             if label in label_map:
                 ds_map[key] = label_map[label]
         return json.dumps(ds_map)
 
-    def setup_workflow_run(self, workflow: Optional[Dict[str, Any]] = None, inputs_by: str = 'step_id', history_id: Optional[str] = None, workflow_id: Optional[str] = None) -> Tuple[Dict[str, Any], str, str]:
+    def setup_workflow_run(
+        self,
+        workflow: Optional[Dict[str, Any]] = None,
+        inputs_by: str = "step_id",
+        history_id: Optional[str] = None,
+        workflow_id: Optional[str] = None,
+    ) -> Tuple[Dict[str, Any], str, str]:
         ds_entry = self.dataset_populator.ds_entry
         if not workflow_id:
             assert workflow, "If workflow_id not specified, must specify a workflow dictionary to load"
             workflow_id = self.create_workflow(workflow)
         if not history_id:
             history_id = self.dataset_populator.new_history()
-        hda1 = self.dataset_populator.new_dataset(history_id, content="1 2 3")
-        hda2 = self.dataset_populator.new_dataset(history_id, content="4 5 6")
+        hda1 = self.dataset_populator.new_dataset(history_id, content="1 2 3", wait=True)
+        hda2 = self.dataset_populator.new_dataset(history_id, content="4 5 6", wait=True)
         workflow_request = dict(
             history=f"hist_id={history_id}",
         )
-        label_map = {
-            'WorkflowInput1': ds_entry(hda1),
-            'WorkflowInput2': ds_entry(hda2)
-        }
-        if inputs_by == 'step_id':
+        label_map = {"WorkflowInput1": ds_entry(hda1), "WorkflowInput2": ds_entry(hda2)}
+        if inputs_by == "step_id":
             ds_map = self.build_ds_map(workflow_id, label_map)
             workflow_request["ds_map"] = ds_map
         elif inputs_by == "step_index":
-            index_map = {
-                '0': ds_entry(hda1),
-                '1': ds_entry(hda2)
-            }
+            index_map = {"0": ds_entry(hda1), "1": ds_entry(hda2)}
             workflow_request["inputs"] = json.dumps(index_map)
-            workflow_request["inputs_by"] = 'step_index'
+            workflow_request["inputs_by"] = "step_index"
         elif inputs_by == "name":
             workflow_request["inputs"] = json.dumps(label_map)
-            workflow_request["inputs_by"] = 'name'
+            workflow_request["inputs_by"] = "name"
         elif inputs_by in ["step_uuid", "uuid_implicitly"]:
             assert workflow, f"Must specify workflow for this inputs_by {inputs_by} parameter value"
             uuid_map = {
                 workflow["steps"]["0"]["uuid"]: ds_entry(hda1),
                 workflow["steps"]["1"]["uuid"]: ds_entry(hda2),
             }
             workflow_request["inputs"] = json.dumps(uuid_map)
             if inputs_by == "step_uuid":
                 workflow_request["inputs_by"] = "step_uuid"
 
         return workflow_request, history_id, workflow_id
 
-    def wait_for_invocation_and_jobs(self, history_id, workflow_id, invocation_id, assert_ok=True):
+    def wait_for_invocation_and_jobs(
+        self, history_id: str, workflow_id: str, invocation_id: str, assert_ok: bool = True
+    ) -> None:
         state = self.wait_for_invocation(workflow_id, invocation_id)
         if assert_ok:
             assert state == "scheduled", state
-        time.sleep(.5)
+        time.sleep(0.5)
         self.dataset_populator.wait_for_history_jobs(history_id, assert_ok=assert_ok)
-        time.sleep(.5)
+        time.sleep(0.5)
+
+    def index(
+        self,
+        show_shared: Optional[bool] = None,
+        show_published: Optional[bool] = None,
+        sort_by: Optional[str] = None,
+        sort_desc: Optional[bool] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        search: Optional[str] = None,
+        skip_step_counts: Optional[bool] = None,
+    ):
+        endpoint = "workflows?"
+        if show_shared is not None:
+            endpoint += f"show_shared={show_shared}&"
+        if show_published is not None:
+            endpoint += f"show_published={show_published}&"
+        if sort_by is not None:
+            endpoint += f"sort_by={sort_by}&"
+        if sort_desc is not None:
+            endpoint += f"sort_desc={sort_desc}&"
+        if limit is not None:
+            endpoint += f"limit={limit}&"
+        if offset is not None:
+            endpoint += f"offset={offset}&"
+        if search is not None:
+            endpoint += f"search={search}&"
+        if skip_step_counts is not None:
+            endpoint += f"skip_step_counts={skip_step_counts}&"
+        response = self._get(endpoint)
+        api_asserts.assert_status_code_is_ok(response)
+        return response.json()
+
+    def index_ids(
+        self,
+        show_shared: Optional[bool] = None,
+        show_published: Optional[bool] = None,
+        sort_by: Optional[str] = None,
+        sort_desc: Optional[bool] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        search: Optional[str] = None,
+    ):
+        workflows = self.index(
+            show_shared=show_shared,
+            show_published=show_published,
+            sort_by=sort_by,
+            sort_desc=sort_desc,
+            limit=limit,
+            offset=offset,
+            search=search,
+        )
+        return [w["id"] for w in workflows]
+
+    def share_with_user(self, workflow_id: str, user_id_or_email: str):
+        data = {"user_ids": [user_id_or_email]}
+        response = self._put(f"workflows/{workflow_id}/share_with_users", data, json=True)
+        api_asserts.assert_status_code_is_ok(response)
 
 
 class RunJobsSummary(NamedTuple):
     history_id: str
     workflow_id: str
     invocation_id: str
     inputs: dict
     jobs: list
     invocation: dict
     workflow_request: dict
 
 
 class WorkflowPopulator(GalaxyInteractorHttpMixin, BaseWorkflowPopulator, ImporterGalaxyInterface):
-
     def __init__(self, galaxy_interactor):
         self.galaxy_interactor = galaxy_interactor
         self.dataset_populator = DatasetPopulator(galaxy_interactor)
         self.dataset_collection_populator = DatasetCollectionPopulator(galaxy_interactor)
 
     # Required for ImporterGalaxyInterface interface - so we can recursively import
     # nested workflows.
     def import_workflow(self, workflow, **kwds) -> Dict[str, Any]:
         workflow_str = json.dumps(workflow, indent=4)
         data = {
-            'workflow': workflow_str,
+            "workflow": workflow_str,
         }
         data.update(**kwds)
         upload_response = self._post("workflows", data=data)
         assert upload_response.status_code == 200, upload_response.content
         return upload_response.json()
 
     def import_tool(self, tool) -> Dict[str, Any]:
-        """ Import a workflow via POST /api/workflows or
+        """Import a workflow via POST /api/workflows or
         comparable interface into Galaxy.
         """
         upload_response = self._import_tool_response(tool)
         assert upload_response.status_code == 200, upload_response
         return upload_response.json()
 
     def _import_tool_response(self, tool) -> Response:
+        using_requirement("admin")
         tool_str = json.dumps(tool, indent=4)
-        data = {
-            'representation': tool_str
-        }
+        data = {"representation": tool_str}
         upload_response = self._post("dynamic_tools", data=data, admin=True)
         return upload_response
 
     def scaling_workflow_yaml(self, **kwd):
         workflow_dict = self._scale_workflow_dict(**kwd)
         has_workflow = yaml.dump(workflow_dict)
         return has_workflow
@@ -1509,15 +2042,15 @@
 
     def _scale_workflow_dict_simple(self, **kwd) -> Dict[str, Any]:
         collection_size = kwd.get("collection_size", 2)
         workflow_depth = kwd.get("workflow_depth", 3)
 
         scale_workflow_steps = [
             {"tool_id": "create_input_collection", "state": {"collection_size": collection_size}, "label": "wf_input"},
-            {"tool_id": "cat", "state": {"input1": self._link("wf_input", "output")}, "label": "cat_0"}
+            {"tool_id": "cat", "state": {"input1": self._link("wf_input", "output")}, "label": "cat_0"},
         ]
 
         for i in range(workflow_depth):
             link = f"cat_{str(i)}/out_file1"
             scale_workflow_steps.append(
                 {"tool_id": "cat", "state": {"input1": self._link(link)}, "label": f"cat_{str(i + 1)}"}
             )
@@ -1531,15 +2064,19 @@
 
     def _scale_workflow_dict_two_outputs(self, **kwd) -> Dict[str, Any]:
         collection_size = kwd.get("collection_size", 10)
         workflow_depth = kwd.get("workflow_depth", 10)
 
         scale_workflow_steps = [
             {"tool_id": "create_input_collection", "state": {"collection_size": collection_size}, "label": "wf_input"},
-            {"tool_id": "cat", "state": {"input1": self._link("wf_input"), "input2": self._link("wf_input")}, "label": "cat_0"}
+            {
+                "tool_id": "cat",
+                "state": {"input1": self._link("wf_input"), "input2": self._link("wf_input")},
+                "label": "cat_0",
+            },
         ]
 
         for i in range(workflow_depth):
             link1 = f"cat_{str(i)}#out_file1"
             link2 = f"cat_{str(i)}#out_file2"
             scale_workflow_steps.append(
                 {"tool_id": "cat", "state": {"input1": self._link(link1), "input2": self._link(link2)}}
@@ -1579,16 +2116,168 @@
     @staticmethod
     def _link(link: str, output_name: Optional[str] = None) -> Dict[str, Any]:
         if output_name is not None:
             link = f"{str(link)}/{output_name}"
         return {"$link": link}
 
 
-class LibraryPopulator:
+class CwlPopulator:
+    def __init__(self, dataset_populator: DatasetPopulator, workflow_populator: WorkflowPopulator):
+        self.dataset_populator = dataset_populator
+        self.workflow_populator = workflow_populator
+
+    def get_conformance_test(self, version: str, doc: str):
+        for test in conformance_tests_gen(os.path.join(CWL_TOOL_DIRECTORY, version)):
+            if test.get("doc") == doc:
+                return test
+        raise Exception(f"doc [{doc}] not found")
+
+    def _run_cwl_tool_job(
+        self,
+        tool_id: str,
+        job: dict,
+        history_id: str,
+        assert_ok: bool = True,
+    ) -> CwlToolRun:
+        galaxy_tool_id: Optional[str] = tool_id
+        tool_uuid = None
+
+        if os.path.exists(tool_id):
+            raw_tool_id = os.path.basename(tool_id)
+            index = self.dataset_populator._get("tools", data=dict(in_panel=False))
+            index.raise_for_status()
+            tools = index.json()
+            # In panels by default, so flatten out sections...
+            tool_ids = [itemgetter("id")(_) for _ in tools]
+            if raw_tool_id in tool_ids:
+                galaxy_tool_id = raw_tool_id
+            else:
+                dynamic_tool = self.dataset_populator.create_tool_from_path(tool_id)
+                galaxy_tool_id = None
+                tool_uuid = dynamic_tool["uuid"]
+
+        run_response = self.dataset_populator.run_tool_raw(galaxy_tool_id, job, history_id, tool_uuid=tool_uuid)
+        if assert_ok:
+            run_response.raise_for_status()
+        return CwlToolRun(self.dataset_populator, history_id, run_response)
+
+    def _run_cwl_workflow_job(
+        self,
+        workflow_path: str,
+        job: dict,
+        history_id: str,
+        assert_ok: bool = True,
+    ):
+        workflow_path, object_id = urllib.parse.urldefrag(workflow_path)
+        workflow_id = self.workflow_populator.import_workflow_from_path(workflow_path, object_id)
+
+        request = {
+            # TODO: rework tool state corrections so more of these are valid in Galaxy
+            # workflows as well, and then make it the default. Or decide they are safe.
+            "allow_tool_state_corrections": True,
+        }
+        invocation_id = self.workflow_populator.invoke_workflow_and_assert_ok(
+            workflow_id, history_id=history_id, inputs=job, request=request, inputs_by="name"
+        )
+        return CwlWorkflowRun(self.dataset_populator, self.workflow_populator, history_id, workflow_id, invocation_id)
+
+    def run_cwl_job(
+        self,
+        artifact: str,
+        job_path: Optional[str] = None,
+        job: Optional[Dict] = None,
+        test_data_directory: Optional[str] = None,
+        history_id: Optional[str] = None,
+        assert_ok: bool = True,
+    ) -> CwlRun:
+        """
+        :param artifact: CWL tool id, or (absolute or relative) path to a CWL
+          tool or workflow file
+        """
+        if history_id is None:
+            history_id = self.dataset_populator.new_history()
+        artifact_without_id = artifact.split("#", 1)[0]
+        if os.path.exists(artifact_without_id):
+            tool_or_workflow: Literal["tool", "workflow"] = guess_artifact_type(artifact)
+        else:
+            # Assume it's a tool id
+            tool_or_workflow = "tool"
+        if job_path and not os.path.exists(job_path):
+            raise ValueError(f"job_path [{job_path}] does not exist")
+        if test_data_directory is None and job_path is not None:
+            test_data_directory = os.path.dirname(job_path)
+        if job_path is not None:
+            assert job is None
+            with open(job_path) as f:
+                job = yaml.safe_load(f)
+        elif job is None:
+            job = {}
+        _, datasets = stage_inputs(
+            self.dataset_populator.galaxy_interactor,
+            history_id,
+            job,
+            use_fetch_api=False,
+            tool_or_workflow=tool_or_workflow,
+            job_dir=test_data_directory,
+        )
+        if datasets:
+            self.dataset_populator.wait_for_history(history_id=history_id, assert_ok=True)
+        if tool_or_workflow == "tool":
+            run_object = self._run_cwl_tool_job(
+                artifact,
+                job,
+                history_id,
+                assert_ok=assert_ok,
+            )
+        else:
+            run_object = self._run_cwl_workflow_job(
+                artifact,
+                job,
+                history_id,
+                assert_ok=assert_ok,
+            )
+        if assert_ok:
+            try:
+                run_object.wait()
+            except Exception:
+                self.dataset_populator._summarize_history(history_id)
+                raise
+        return run_object
+
+    def run_conformance_test(self, version: str, doc: str):
+        test = self.get_conformance_test(version, doc)
+        directory = test["directory"]
+        artifact = os.path.join(directory, test["tool"])
+        job_path = test.get("job")
+        if job_path is not None:
+            job_path = os.path.join(directory, job_path)
+        should_fail = test.get("should_fail", False)
+        try:
+            run = self.run_cwl_job(artifact, job_path=job_path)
+        except Exception:
+            # Should fail so this is good!
+            if should_fail:
+                return True
+            raise
 
+        if should_fail:
+            self.dataset_populator._summarize_history(run.history_id)
+            raise Exception("Expected run to fail but it didn't.")
+
+        expected_outputs = test["output"]
+        try:
+            for key, value in expected_outputs.items():
+                actual_output = run.get_output_as_object(key)
+                cwltest.compare.compare(value, actual_output)
+        except Exception:
+            self.dataset_populator._summarize_history(run.history_id)
+            raise
+
+
+class LibraryPopulator:
     def __init__(self, galaxy_interactor):
         self.galaxy_interactor = galaxy_interactor
         self.dataset_populator = DatasetPopulator(galaxy_interactor)
 
     def get_libraries(self):
         get_response = self.galaxy_interactor.get("libraries")
         return get_response.json()
@@ -1597,28 +2286,67 @@
         library = self.new_library(name)
         library_id = library["id"]
 
         role_id = self.user_private_role_id()
         self.set_permissions(library_id, role_id)
         return library
 
+    def create_from_store_raw(self, payload: Dict[str, Any]) -> Response:
+        using_requirement("admin")
+        using_requirement("new_library")
+        create_response = self.galaxy_interactor.post("libraries/from_store", payload, json=True, admin=True)
+        return create_response
+
+    def create_from_store(
+        self, store_dict: Optional[Dict[str, Any]] = None, store_path: Optional[str] = None
+    ) -> List[Dict[str, Any]]:
+        payload = _store_payload(store_dict=store_dict, store_path=store_path)
+        create_response = self.create_from_store_raw(payload)
+        api_asserts.assert_status_code_is_ok(create_response)
+        return create_response.json()
+
     def new_library(self, name):
+        using_requirement("new_library")
+        using_requirement("admin")
         data = dict(name=name)
         create_response = self.galaxy_interactor.post("libraries", data=data, admin=True, json=True)
         return create_response.json()
 
+    def fetch_single_url_to_folder(self, file_type="auto", assert_ok=True):
+        history_id, library, destination = self.setup_fetch_to_folder("single_url")
+        items = [
+            {
+                "src": "url",
+                "url": FILE_URL,
+                "MD5": FILE_MD5,
+                "ext": file_type,
+            }
+        ]
+        targets = [
+            {
+                "destination": destination,
+                "items": items,
+            }
+        ]
+        payload = {
+            "history_id": history_id,  # TODO: Shouldn't be needed :(
+            "targets": targets,
+            "validate_hashes": True,
+        }
+        return library, self.dataset_populator.fetch(payload, assert_ok=assert_ok)
+
     def get_permissions(
         self,
         library_id,
         scope: Optional[str] = "current",
         is_library_access: Optional[bool] = False,
         page: Optional[int] = 1,
         page_limit: Optional[int] = 1000,
         q: Optional[str] = None,
-        admin: Optional[bool] = True
+        admin: Optional[bool] = True,
     ):
         query = f"&q={q}" if q else ""
         response = self.galaxy_interactor.get(
             f"libraries/{library_id}/permissions?scope={scope}&is_library_access={is_library_access}&page={page}&page_limit={page_limit}{query}",
             admin=admin,
         )
         api_asserts.assert_status_code_is(response, 200)
@@ -1664,15 +2392,18 @@
         permissions = {
             "action": action,
             permission: role_id or [],
         }
         self._set_permissions(library_id, permissions)
 
     def _set_permissions(self, library_id, permissions):
-        response = self.galaxy_interactor.post(f"libraries/{library_id}/permissions", data=permissions, admin=True, json=True)
+        using_requirement("admin")
+        response = self.galaxy_interactor.post(
+            f"libraries/{library_id}/permissions", data=permissions, admin=True, json=True
+        )
         api_asserts.assert_status_code_is(response, 200)
 
     def user_email(self):
         # deprecated - use DatasetPopulator
         return self.dataset_populator.user_email()
 
     def user_private_role_id(self):
@@ -1711,26 +2442,30 @@
         dataset = self.raw_library_contents_create(library["id"], payload, files=files).json()[0]
         return self.wait_on_library_dataset(library["id"], dataset["id"])
 
     def wait_on_library_dataset(self, library_id, dataset_id):
         def show():
             return self.galaxy_interactor.get(f"libraries/{library_id}/contents/{dataset_id}")
 
-        wait_on_state(show, assert_ok=True, timeout=DEFAULT_TIMEOUT)
+        wait_on_state(show, assert_ok=True)
         return show().json()
 
     def raw_library_contents_create(self, library_id, payload, files=None):
         if files is None:
             files = {}
 
         url_rel = f"libraries/{library_id}/contents"
         return self.galaxy_interactor.post(url_rel, payload, files=files)
 
-    def show_ld(self, library_id, library_dataset_id):
+    def show_ld_raw(self, library_id: str, library_dataset_id: str) -> Response:
         response = self.galaxy_interactor.get(f"libraries/{library_id}/contents/{library_dataset_id}")
+        return response
+
+    def show_ld(self, library_id: str, library_dataset_id: str) -> Dict[str, Any]:
+        response = self.show_ld_raw(library_id, library_dataset_id)
         response.raise_for_status()
         return response.json()
 
     def show_ldda(self, ldda_id):
         response = self.galaxy_interactor.get(f"datasets/{ldda_id}?hda_ldda=ldda")
         response.raise_for_status()
         return response.json()
@@ -1771,126 +2506,125 @@
         return history_id, library, destination
 
 
 class BaseDatasetCollectionPopulator:
     dataset_populator: BaseDatasetPopulator
 
     def create_list_from_pairs(self, history_id, pairs, name="Dataset Collection from pairs"):
-        return self.create_nested_collection(history_id=history_id,
-                                             collection=pairs,
-                                             collection_type='list:paired',
-                                             name=name)
+        return self.create_nested_collection(
+            history_id=history_id, collection=pairs, collection_type="list:paired", name=name
+        )
 
-    def nested_collection_identifiers(self, history_id, collection_type):
+    def nested_collection_identifiers(self, history_id: str, collection_type):
         rank_types = list(reversed(collection_type.split(":")))
         assert len(rank_types) > 0
         rank_type_0 = rank_types[0]
         if rank_type_0 == "list":
             identifiers = self.list_identifiers(history_id)
         else:
             identifiers = self.pair_identifiers(history_id)
         nested_collection_type = rank_type_0
 
         for i, rank_type in enumerate(reversed(rank_types[1:])):
             name = f"test_level_{i + 1}" if rank_type == "list" else "paired"
-            identifiers = [dict(
-                src="new_collection",
-                name=name,
-                collection_type=nested_collection_type,
-                element_identifiers=identifiers,
-            )]
+            identifiers = [
+                dict(
+                    src="new_collection",
+                    name=name,
+                    collection_type=nested_collection_type,
+                    element_identifiers=identifiers,
+                )
+            ]
             nested_collection_type = f"{rank_type}:{nested_collection_type}"
         return identifiers
 
-    def create_nested_collection(self, history_id, collection_type, name=None, collection=None, element_identifiers=None):
+    def create_nested_collection(
+        self, history_id, collection_type, name=None, collection=None, element_identifiers=None
+    ):
         """Create a nested collection either from collection or using collection_type)."""
         assert collection_type is not None
         name = name or f"Test {collection_type}"
         if collection is not None:
             assert element_identifiers is None
             element_identifiers = []
             for i, pair in enumerate(collection):
-                element_identifiers.append(dict(
-                    name=f"test{i}",
-                    src="hdca",
-                    id=pair
-                ))
+                element_identifiers.append(dict(name=f"test{i}", src="hdca", id=pair))
         if element_identifiers is None:
             element_identifiers = self.nested_collection_identifiers(history_id, collection_type)
 
         payload = dict(
             instance_type="history",
             history_id=history_id,
             element_identifiers=element_identifiers,
             collection_type=collection_type,
             name=name,
         )
         return self.__create(payload)
 
     def create_list_of_pairs_in_history(self, history_id, **kwds):
-        return self.upload_collection(history_id, "list:paired", elements=[
-            {
-                "name": "test0",
-                "elements": [
-                    {"src": "pasted", "paste_content": "TestData123", "name": "forward"},
-                    {"src": "pasted", "paste_content": "TestData123", "name": "reverse"},
-                ]
-            }
-        ])
+        return self.upload_collection(
+            history_id,
+            "list:paired",
+            elements=[
+                {
+                    "name": "test0",
+                    "elements": [
+                        {"src": "pasted", "paste_content": "TestData123", "name": "forward"},
+                        {"src": "pasted", "paste_content": "TestData123", "name": "reverse"},
+                    ],
+                }
+            ],
+        )
 
-    def create_list_of_list_in_history(self, history_id, **kwds):
+    def create_list_of_list_in_history(self, history_id: str, **kwds):
         # create_nested_collection will generate nested collection from just datasets,
         # this function uses recursive generation of history hdcas.
-        collection_type = kwds.pop('collection_type', 'list:list')
-        collection_types = collection_type.split(':')
-        list = self.create_list_in_history(history_id, **kwds).json()['id']
-        current_collection_type = 'list'
+        collection_type = kwds.pop("collection_type", "list:list")
+        collection_types = collection_type.split(":")
+        list = self.create_list_in_history(history_id, **kwds).json()["output_collections"][0]
+        current_collection_type = "list"
         for collection_type in collection_types[1:]:
             current_collection_type = f"{current_collection_type}:{collection_type}"
-            response = self.create_nested_collection(history_id=history_id,
-                                                     collection_type=current_collection_type,
-                                                     name=current_collection_type,
-                                                     collection=[list])
-            list = response.json()['id']
+            response = self.create_nested_collection(
+                history_id=history_id,
+                collection_type=current_collection_type,
+                name=current_collection_type,
+                collection=[list["id"]],
+            )
+            list = response.json()
         return response
 
-    def create_pair_in_history(self, history_id, **kwds):
-        payload = self.create_pair_payload(
-            history_id,
-            instance_type="history",
-            **kwds
-        )
-        return self.__create(payload)
+    def create_pair_in_history(self, history_id: str, wait: bool = False, **kwds):
+        payload = self.create_pair_payload(history_id, instance_type="history", **kwds)
+        return self.__create(payload, wait=wait)
+
+    def create_list_in_history(self, history_id: str, wait: bool = False, **kwds):
+        payload = self.create_list_payload(history_id, instance_type="history", **kwds)
+        return self.__create(payload, wait=wait)
 
-    def create_list_in_history(self, history_id, **kwds):
-        payload = self.create_list_payload(
-            history_id,
-            instance_type="history",
-            **kwds
-        )
-        return self.__create(payload)
-
-    def upload_collection(self, history_id, collection_type, elements, **kwds):
+    def upload_collection(self, history_id: str, collection_type, elements, wait: bool = False, **kwds):
         payload = self.__create_payload_fetch(history_id, collection_type, contents=elements, **kwds)
-        return self.__create(payload)
+        return self.__create(payload, wait=wait)
 
-    def create_list_payload(self, history_id, **kwds):
+    def create_list_payload(self, history_id: str, **kwds):
         return self.__create_payload(history_id, identifiers_func=self.list_identifiers, collection_type="list", **kwds)
 
-    def create_pair_payload(self, history_id, **kwds):
-        return self.__create_payload(history_id, identifiers_func=self.pair_identifiers, collection_type="paired", **kwds)
+    def create_pair_payload(self, history_id: str, **kwds):
+        return self.__create_payload(
+            history_id, identifiers_func=self.pair_identifiers, collection_type="paired", **kwds
+        )
 
-    def __create_payload(self, *args, **kwds):
-        direct_upload = kwds.pop("direct_upload", False)
+    def __create_payload(self, history_id: str, *args, **kwds):
+        direct_upload = kwds.pop("direct_upload", True)
         if direct_upload:
-            return self.__create_payload_fetch(*args, **kwds)
+            return self.__create_payload_fetch(history_id, *args, **kwds)
         else:
-            return self.__create_payload_collection(*args, **kwds)
+            return self.__create_payload_collection(history_id, *args, **kwds)
 
-    def __create_payload_fetch(self, history_id, collection_type, **kwds):
+    def __create_payload_fetch(self, history_id: str, collection_type, **kwds):
         contents = None
         if "contents" in kwds:
             contents = kwds["contents"]
             del kwds["contents"]
 
         elements = []
         if contents is None:
@@ -1921,190 +2655,219 @@
                         element_identifier = f"data{i}"
                     elif collection_type == "paired" and i == 0:
                         element_identifier = "forward"
                     else:
                         element_identifier = "reverse"
                 element["name"] = element_identifier
                 element["paste_content"] = dataset_contents
+                element["to_posix_lines"] = kwds.get("to_posix_lines", True)
                 elements.append(element)
 
         name = kwds.get("name", "Test Dataset Collection")
 
-        targets = [{
-            "destination": {"type": "hdca"},
-            "elements": elements,
-            "collection_type": collection_type,
-            "name": name,
-        }]
+        targets = [
+            {
+                "destination": {"type": "hdca"},
+                "elements": elements,
+                "collection_type": collection_type,
+                "name": name,
+            }
+        ]
         payload = dict(
             history_id=history_id,
-            targets=json.dumps(targets),
+            targets=targets,
         )
         return payload
 
-    def wait_for_fetched_collection(self, fetch_response):
-        self.dataset_populator.wait_for_job(fetch_response["jobs"][0]["id"], assert_ok=True)
-        initial_dataset_collection = fetch_response["outputs"][0]
-        dataset_collection = self.dataset_populator.get_history_collection_details(initial_dataset_collection["history_id"], hid=initial_dataset_collection["hid"])
+    def wait_for_fetched_collection(self, fetch_response: Union[Dict[str, Any], Response]):
+        fetch_response_dict: Dict[str, Any]
+        if isinstance(fetch_response, Response):
+            fetch_response_dict = fetch_response.json()
+        else:
+            fetch_response_dict = fetch_response
+        self.dataset_populator.wait_for_job(fetch_response_dict["jobs"][0]["id"], assert_ok=True)
+        initial_dataset_collection = fetch_response_dict["output_collections"][0]
+        dataset_collection = self.dataset_populator.get_history_collection_details(
+            initial_dataset_collection["history_id"], hid=initial_dataset_collection["hid"]
+        )
         return dataset_collection
 
-    def __create_payload_collection(self, history_id, identifiers_func, collection_type, **kwds):
+    def __create_payload_collection(self, history_id: str, identifiers_func, collection_type, **kwds):
         contents = None
         if "contents" in kwds:
             contents = kwds["contents"]
             del kwds["contents"]
 
         if "element_identifiers" not in kwds:
             kwds["element_identifiers"] = identifiers_func(history_id, contents=contents)
 
         if "name" not in kwds:
             kwds["name"] = "Test Dataset Collection"
 
-        payload = dict(
-            history_id=history_id,
-            collection_type=collection_type,
-            **kwds
-        )
+        payload = dict(history_id=history_id, collection_type=collection_type, **kwds)
         return payload
 
-    def pair_identifiers(self, history_id, contents=None):
+    def pair_identifiers(self, history_id: str, contents=None):
         hda1, hda2 = self.__datasets(history_id, count=2, contents=contents)
 
         element_identifiers = [
             dict(name="forward", src="hda", id=hda1["id"]),
             dict(name="reverse", src="hda", id=hda2["id"]),
         ]
         return element_identifiers
 
-    def list_identifiers(self, history_id, contents=None):
+    def list_identifiers(self, history_id: str, contents=None):
         count = 3 if contents is None else len(contents)
         # Contents can be a list of strings (with name auto-assigned here) or a list of
         # 2-tuples of form (name, dataset_content).
         if contents and isinstance(contents[0], tuple):
             hdas = self.__datasets(history_id, count=count, contents=[c[1] for c in contents])
 
             def hda_to_identifier(i, hda):
                 return dict(name=contents[i][0], src="hda", id=hda["id"])
+
         else:
             hdas = self.__datasets(history_id, count=count, contents=contents)
 
             def hda_to_identifier(i, hda):
                 return dict(name=f"data{i + 1}", src="hda", id=hda["id"])
+
         element_identifiers = [hda_to_identifier(i, hda) for (i, hda) in enumerate(hdas)]
         return element_identifiers
 
-    def __create(self, payload):
-        # Create a colleciton - either from existing datasets using collection creation API
+    def __create(self, payload, wait=False):
+        # Create a collection - either from existing datasets using collection creation API
         # or from direct uploads with the fetch API. Dispatch on "targets" keyword in payload
         # to decide which to use.
         if "targets" not in payload:
             return self._create_collection(payload)
         else:
-            return self.dataset_populator.fetch(payload)
+            return self.dataset_populator.fetch(payload, wait=wait)
 
-    def __datasets(self, history_id, count, contents=None):
+    def __datasets(self, history_id: str, count: int, contents=None):
         datasets = []
         for i in range(count):
             new_kwds = {}
             if contents:
                 new_kwds["content"] = contents[i]
             datasets.append(self.dataset_populator.new_dataset(history_id, **new_kwds))
         return datasets
 
-    def wait_for_dataset_collection(self, create_payload, assert_ok=False, timeout=DEFAULT_TIMEOUT):
+    def wait_for_dataset_collection(
+        self, create_payload: dict, assert_ok: bool = False, timeout: timeout_type = DEFAULT_TIMEOUT
+    ) -> None:
         for element in create_payload["elements"]:
-            if element['element_type'] == 'hda':
-                self.dataset_populator.wait_for_dataset(history_id=element['object']['history_id'],
-                                                        dataset_id=element['object']['id'],
-                                                        assert_ok=assert_ok,
-                                                        timeout=timeout)
-            elif element['element_type'] == 'dataset_collection':
-                self.wait_for_dataset_collection(element['object'], assert_ok=assert_ok, timeout=timeout)
+            if element["element_type"] == "hda":
+                self.dataset_populator.wait_for_dataset(
+                    history_id=element["object"]["history_id"],
+                    dataset_id=element["object"]["id"],
+                    assert_ok=assert_ok,
+                    timeout=timeout,
+                )
+            elif element["element_type"] == "dataset_collection":
+                self.wait_for_dataset_collection(element["object"], assert_ok=assert_ok, timeout=timeout)
 
     @abstractmethod
     def _create_collection(self, payload: dict) -> Response:
         """Create collection from specified payload."""
 
 
 class DatasetCollectionPopulator(BaseDatasetCollectionPopulator):
-
     def __init__(self, galaxy_interactor: ApiTestInteractor):
         self.galaxy_interactor = galaxy_interactor
         self.dataset_populator = DatasetPopulator(galaxy_interactor)
 
     def _create_collection(self, payload: dict) -> Response:
         create_response = self.galaxy_interactor.post("dataset_collections", data=payload, json=True)
         return create_response
 
 
-def load_data_dict(history_id, test_data, dataset_populator, dataset_collection_populator):
+LoadDataDictResponseT = Tuple[Dict[str, Any], Dict[str, Any], bool]
+
+
+def load_data_dict(
+    history_id: str,
+    test_data: Dict[str, Any],
+    dataset_populator: BaseDatasetPopulator,
+    dataset_collection_populator: BaseDatasetCollectionPopulator,
+) -> LoadDataDictResponseT:
     """Load a dictionary as inputs to a workflow (test data focused)."""
 
     def open_test_data(test_dict, mode="rb"):
         test_data_resolver = TestDataResolver()
-        filename = test_data_resolver.get_filename(test_dict["value"])
+        filename = test_data_resolver.get_filename(test_dict.pop("value"))
         return open(filename, mode)
 
     def read_test_data(test_dict):
         return open_test_data(test_dict, mode="r").read()
 
     inputs = {}
     label_map = {}
     has_uploads = False
 
     for key, value in test_data.items():
         is_dict = isinstance(value, dict)
-        if is_dict and ("elements" in value or value.get('collection_type')):
+        if is_dict and ("elements" in value or value.get("collection_type")):
             elements_data = value.get("elements", [])
             elements = []
             for element_data in elements_data:
                 # Adapt differences between test_data dict and fetch API description.
                 if "name" not in element_data:
-                    identifier = element_data["identifier"]
+                    identifier = element_data.pop("identifier")
                     element_data["name"] = identifier
-                input_type = element_data.get("type", "raw")
+                input_type = element_data.pop("type", "raw")
                 content = None
                 if input_type == "File":
                     content = read_test_data(element_data)
                 else:
-                    content = element_data["content"]
+                    content = element_data.pop("content")
                 if content is not None:
                     element_data["src"] = "pasted"
                     element_data["paste_content"] = content
                 elements.append(element_data)
             new_collection_kwds = {}
             if "name" in value:
                 new_collection_kwds["name"] = value["name"]
-            collection_type = value.get('collection_type', '')
+            collection_type = value.get("collection_type", "")
             if collection_type == "list:paired":
-                fetch_response = dataset_collection_populator.create_list_of_pairs_in_history(history_id, contents=elements, **new_collection_kwds).json()
-            elif collection_type and ':' in collection_type:
-                fetch_response = {'outputs': [dataset_collection_populator.create_nested_collection(history_id, collection_type=collection_type, **new_collection_kwds).json()]}
+                fetch_response = dataset_collection_populator.create_list_of_pairs_in_history(
+                    history_id, contents=elements, wait=True, **new_collection_kwds
+                ).json()
+            elif collection_type and ":" in collection_type:
+                fetch_response = {
+                    "outputs": [
+                        dataset_collection_populator.create_nested_collection(
+                            history_id, collection_type=collection_type, **new_collection_kwds
+                        ).json()
+                    ]
+                }
             elif collection_type == "list":
-                fetch_response = dataset_collection_populator.create_list_in_history(history_id, contents=elements, direct_upload=True, **new_collection_kwds).json()
+                fetch_response = dataset_collection_populator.create_list_in_history(
+                    history_id, contents=elements, direct_upload=True, wait=True, **new_collection_kwds
+                ).json()
             else:
-                fetch_response = dataset_collection_populator.create_pair_in_history(history_id, contents=elements or None, direct_upload=True, **new_collection_kwds).json()
+                fetch_response = dataset_collection_populator.create_pair_in_history(
+                    history_id, contents=elements or None, direct_upload=True, wait=True, **new_collection_kwds
+                ).json()
             hdca_output = fetch_response["outputs"][0]
             hdca = dataset_populator.ds_entry(hdca_output)
             hdca["hid"] = hdca_output["hid"]
             label_map[key] = hdca
             inputs[key] = hdca
             has_uploads = True
         elif is_dict and "type" in value:
-            input_type = value["type"]
+            input_type = value.pop("type")
             if input_type == "File":
                 content = open_test_data(value)
-                new_dataset_kwds = {
-                    "content": content
-                }
+                new_dataset_kwds = {"content": content}
                 if "name" in value:
                     new_dataset_kwds["name"] = value["name"]
                 if "file_type" in value:
                     new_dataset_kwds["file_type"] = value["file_type"]
-                hda = dataset_populator.new_dataset(history_id, **new_dataset_kwds)
+                hda = dataset_populator.new_dataset(history_id, wait=True, **new_dataset_kwds)
                 label_map[key] = dataset_populator.ds_entry(hda)
                 has_uploads = True
             elif input_type == "raw":
                 label_map[key] = value["value"]
                 inputs[key] = value["value"]
         elif not is_dict:
             has_uploads = True
@@ -2114,123 +2877,155 @@
         else:
             raise ValueError(f"Invalid test_data def {test_data}")
 
     return inputs, label_map, has_uploads
 
 
 def stage_inputs(
-    galaxy_interactor,
-    history_id,
-    job,
-    use_path_paste=True,
-    use_fetch_api=True,
-    to_posix_lines=True,
-    tool_or_workflow="workflow",
-    job_dir=None
-):
+    galaxy_interactor: ApiTestInteractor,
+    history_id: str,
+    job: Dict[str, Any],
+    use_path_paste: bool = True,
+    use_fetch_api: bool = True,
+    to_posix_lines: bool = True,
+    tool_or_workflow: Literal["tool", "workflow"] = "workflow",
+    job_dir: Optional[str] = None,
+) -> Tuple[Dict[str, Any], List[Dict[str, Any]]]:
     """Alternative to load_data_dict that uses production-style workflow inputs."""
-    kwds = dict(
+    kwds = {}
+    if job_dir is not None:
+        kwds["job_dir"] = job_dir
+    return InteractorStaging(galaxy_interactor, use_fetch_api=use_fetch_api).stage(
+        tool_or_workflow,
         history_id=history_id,
         job=job,
         use_path_paste=use_path_paste,
         to_posix_lines=to_posix_lines,
+        **kwds,
     )
-    if job_dir is not None:
-        kwds["job_dir"] = job_dir
-    inputs, datasets = InteractorStaging(galaxy_interactor, use_fetch_api=use_fetch_api).stage(
-        tool_or_workflow, **kwds
-    )
-    return inputs, datasets
 
 
-def stage_rules_example(galaxy_interactor, history_id, example):
+def stage_rules_example(
+    galaxy_interactor: ApiTestInteractor, history_id: str, example: Dict[str, Any]
+) -> Dict[str, Any]:
     """Wrapper around stage_inputs for staging collections defined by rules spec DSL."""
     input_dict = example["test_data"].copy()
     input_dict["collection_type"] = input_dict.pop("type")
     input_dict["class"] = "Collection"
     inputs, _ = stage_inputs(galaxy_interactor, history_id=history_id, job={"input": input_dict})
     return inputs
 
 
-def wait_on_state(state_func: Callable, desc="state", skip_states=None, ok_states=None, assert_ok=False, timeout=DEFAULT_TIMEOUT) -> str:
+def wait_on_state(
+    state_func: Callable,
+    desc: str = "state",
+    skip_states=None,
+    ok_states=None,
+    assert_ok: bool = False,
+    timeout: timeout_type = DEFAULT_TIMEOUT,
+) -> str:
     def get_state():
         response = state_func()
         assert response.status_code == 200, f"Failed to fetch state update while waiting. [{response.content}]"
         state_response = response.json()
         state = state_response["state"]
         if state in skip_states:
             return None
         else:
             if assert_ok:
                 assert state in ok_states, f"Final state - {state} - not okay. Full response: {state_response}"
             return state
 
     if skip_states is None:
-        skip_states = ["running", "queued", "new", "ready", "stop", "stopped", "setting_metadata"]
+        skip_states = ["running", "queued", "new", "ready", "stop", "stopped", "setting_metadata", "waiting"]
     if ok_states is None:
-        ok_states = ["ok", "scheduled"]
+        ok_states = ["ok", "scheduled", "deferred"]
+    # Remove ok_states from skip_states, so we can wait for a state to becoming running
+    skip_states = [s for s in skip_states if s not in ok_states]
     try:
         return wait_on(get_state, desc=desc, timeout=timeout)
     except TimeoutAssertionError as e:
         response = state_func()
         raise TimeoutAssertionError(f"{e} Current response containing state [{response.json()}].")
 
 
+def _store_payload(
+    store_dict: Optional[Dict[str, Any]] = None,
+    store_path: Optional[str] = None,
+    model_store_format: Optional[str] = None,
+) -> Dict[str, Any]:
+    payload: Dict[str, Any] = {}
+    # Ensure only one store method set.
+    assert store_dict is not None or store_path is not None
+    assert store_dict is None or store_path is None
+    if store_dict is not None:
+        payload["store_dict"] = store_dict
+    if store_path is not None and "://" not in store_path:
+        payload["store_content_uri"] = "base64://" + base64.b64encode(open(store_path, "rb").read()).decode("utf-8")
+    else:
+        payload["store_content_uri"] = store_path
+    if model_store_format is not None:
+        payload["model_store_format"] = model_store_format
+    return payload
+
+
 class GiHttpMixin:
     """Mixin for adapting Galaxy testing populators helpers to bioblend."""
+
     _gi: GalaxyClient
 
     @property
     def _api_key(self):
         return self._gi.key
 
     def _api_url(self):
         return self._gi.url
 
     def _get(self, route, data=None, headers=None, admin=False) -> Response:
-        if data is None:
-            data = {}
-        return self._gi.make_get_request(self._url(route), data=data)
+        return self._gi.make_get_request(self._url(route), params=data)
 
     def _post(self, route, data=None, files=None, headers=None, admin=False, json: bool = False) -> Response:
-        if data is None:
-            data = {}
-        data = data.copy()
-        data['key'] = self._gi.key
+        if headers is None:
+            headers = {}
+        headers = headers.copy()
+        headers["x-api-key"] = self._gi.key
         return requests.post(self._url(route), data=data, headers=headers, timeout=DEFAULT_SOCKET_TIMEOUT)
 
     def _put(self, route, data=None, headers=None, admin=False, json: bool = False):
-        if data is None:
-            data = {}
-        data = data.copy()
-        data['key'] = self._gi.key
+        if headers is None:
+            headers = {}
+        headers = headers.copy()
+        headers["x-api-key"] = self._gi.key
         return requests.put(self._url(route), data=data, headers=headers, timeout=DEFAULT_SOCKET_TIMEOUT)
 
     def _delete(self, route, data=None, headers=None, admin=False, json: bool = False):
-        if data is None:
-            data = {}
-        data = data.copy()
-        data['key'] = self._gi.key
+        if headers is None:
+            headers = {}
+        headers = headers.copy()
+        headers["x-api-key"] = self._gi.key
         return requests.delete(self._url(route), data=data, headers=headers, timeout=DEFAULT_SOCKET_TIMEOUT)
 
     def _url(self, route):
         if route.startswith("/api/"):
-            route = route[len("/api/"):]
+            route = route[len("/api/") :]
 
         return f"{self._api_url()}/{route}"
 
 
 class GiDatasetPopulator(GiHttpMixin, BaseDatasetPopulator):
 
     """Implementation of BaseDatasetPopulator backed by bioblend."""
 
     def __init__(self, gi):
         """Construct a dataset populator from a bioblend GalaxyInstance."""
         self._gi = gi
 
+    def _summarize_history(self, history_id: str) -> None:
+        pass
+
 
 class GiDatasetCollectionPopulator(GiHttpMixin, BaseDatasetCollectionPopulator):
 
     """Implementation of BaseDatasetCollectionPopulator backed by bioblend."""
 
     def __init__(self, gi):
         """Construct a dataset collection populator from a bioblend GalaxyInstance."""
@@ -2249,9 +3044,20 @@
 
     def __init__(self, gi):
         """Construct a workflow populator from a bioblend GalaxyInstance."""
         self._gi = gi
         self.dataset_populator = GiDatasetPopulator(gi)
 
 
-def wait_on(function, desc, timeout=DEFAULT_TIMEOUT):
+def wait_on(function: Callable, desc: str, timeout: timeout_type = DEFAULT_TIMEOUT):
     return tool_util_wait_on(function, desc, timeout)
+
+
+def wait_on_assertion(function: Callable, desc: str, timeout: timeout_type = DEFAULT_TIMEOUT):
+    def inner_func():
+        try:
+            function()
+            return True
+        except AssertionError:
+            return False
+
+    wait_on(inner_func, desc, timeout)
```

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/rules_test_data.py` & `galaxy-test-base-23.0.2/galaxy_test/base/rules_test_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 "class": "File",
             },
             {
                 "identifier": "i2",
                 "contents": "1",
                 "class": "File",
             },
-        ]
+        ],
     },
     "check": check_example_1,
     "output_hid": 6,
 }
 
 
 EXAMPLE_2 = {
@@ -113,15 +113,15 @@
             {
                 "type": "add_column_metadata",
                 "value": "identifier0",
             },
             {
                 "type": "add_column_metadata",
                 "value": "identifier0",
-            }
+            },
         ],
         "mapping": [
             {
                 "type": "list_identifiers",
                 "columns": [0, 1],
             }
         ],
@@ -135,15 +135,15 @@
                 "class": "File",
             },
             {
                 "identifier": "i2",
                 "contents": "1",
                 "class": "File",
             },
-        ]
+        ],
     },
     "check": check_example_2,
     "output_hid": 6,
 }
 
 # Flatten
 EXAMPLE_3 = {
@@ -157,108 +157,77 @@
                 "type": "add_column_metadata",
                 "value": "identifier1",
             },
             {
                 "type": "add_column_concatenate",
                 "target_column_0": 0,
                 "target_column_1": 1,
-            }
+            },
         ],
         "mapping": [
             {
                 "type": "list_identifiers",
                 "columns": [2],
             }
         ],
     },
     "test_data": {
         "type": "list:paired",
         "elements": [
             {
                 "identifier": "test0",
                 "elements": [
-                    {
-                        "identifier": "forward",
-                        "class": "File",
-                        "contents": "TestData123"
-                    },
-                    {
-                        "identifier": "reverse",
-                        "class": "File",
-                        "contents": "TestData123"
-                    },
-                ]
+                    {"identifier": "forward", "class": "File", "contents": "TestData123"},
+                    {"identifier": "reverse", "class": "File", "contents": "TestData123"},
+                ],
             }
-        ]
+        ],
     },
     "check": check_example_3,
     "output_hid": 6,
 }
 
 # Nesting with group tags.
 EXAMPLE_4 = {
     "rules": {
         "rules": [
             {
                 "type": "add_column_metadata",
                 "value": "identifier0",
             },
-            {
-                "type": "add_column_group_tag_value",
-                "value": "type",
-                "default_value": "unused"
-            }
+            {"type": "add_column_group_tag_value", "value": "type", "default_value": "unused"},
         ],
         "mapping": [
             {
                 "type": "list_identifiers",
                 "columns": [1, 0],
             }
         ],
     },
     "test_data": {
         "type": "list",
         "elements": [
-            {
-                "identifier": "i1",
-                "contents": "0",
-                "class": "File",
-                "tags": ["random", "group:type:single"]
-            },
-            {
-                "identifier": "i2",
-                "contents": "1",
-                "class": "File",
-                "tags": ["random", "group:type:paired"]
-            },
-            {
-                "identifier": "i3",
-                "contents": "2",
-                "class": "File",
-                "tags": ["random", "group:type:paired"]
-            },
-        ]
+            {"identifier": "i1", "contents": "0", "class": "File", "tags": ["random", "group:type:single"]},
+            {"identifier": "i2", "contents": "1", "class": "File", "tags": ["random", "group:type:paired"]},
+            {"identifier": "i3", "contents": "2", "class": "File", "tags": ["random", "group:type:paired"]},
+        ],
     },
     "check": check_example_4,
     "output_hid": 8,
 }
 
 
 EXAMPLE_5 = {
     "rules": {
         "rules": [
             {
                 "type": "add_column_metadata",
                 "value": "identifier0",
             },
-            {
-                "type": "add_column_group_tag_value",
-                "value": "type",
-                "default_value": "unused"
-            }
+            {"type": "add_column_group_tag_value", "value": "type", "default_value": "unused"},
         ],
         "mapping": [
             {
                 "type": "list_identifiers",
                 "columns": [1, 0],
             },
             {
@@ -270,33 +239,18 @@
                 "columns": [0],
             },
         ],
     },
     "test_data": {
         "type": "list",
         "elements": [
-            {
-                "identifier": "i1",
-                "contents": "0",
-                "class": "File",
-                "tags": ["random", "group:type:single"]
-            },
-            {
-                "identifier": "i2",
-                "contents": "1",
-                "class": "File",
-                "tags": ["random", "group:type:paired"]
-            },
-            {
-                "identifier": "i3",
-                "contents": "2",
-                "class": "File",
-                "tags": ["random", "group:type:paired"]
-            },
-        ]
+            {"identifier": "i1", "contents": "0", "class": "File", "tags": ["random", "group:type:single"]},
+            {"identifier": "i2", "contents": "1", "class": "File", "tags": ["random", "group:type:paired"]},
+            {"identifier": "i3", "contents": "2", "class": "File", "tags": ["random", "group:type:paired"]},
+        ],
     },
     "check": check_example_5,
     "output_hid": 8,
 }
 
 
 EXAMPLE_6 = {
@@ -305,15 +259,15 @@
             {
                 "type": "add_column_metadata",
                 "value": "identifier0",
             },
             {
                 "type": "add_column_metadata",
                 "value": "tags",
-            }
+            },
         ],
         "mapping": [
             {
                 "type": "list_identifiers",
                 "columns": [0],
             },
             {
@@ -321,30 +275,15 @@
                 "columns": [1],
             },
         ],
     },
     "test_data": {
         "type": "list",
         "elements": [
-            {
-                "identifier": "i1",
-                "contents": "0",
-                "class": "File",
-                "tags": ["random", "group:type:single"]
-            },
-            {
-                "identifier": "i2",
-                "contents": "1",
-                "class": "File",
-                "tags": ["random", "group:type:paired"]
-            },
-            {
-                "identifier": "i3",
-                "contents": "2",
-                "class": "File",
-                "tags": ["random", "group:type:paired"]
-            },
-        ]
+            {"identifier": "i1", "contents": "0", "class": "File", "tags": ["random", "group:type:single"]},
+            {"identifier": "i2", "contents": "1", "class": "File", "tags": ["random", "group:type:paired"]},
+            {"identifier": "i3", "contents": "2", "class": "File", "tags": ["random", "group:type:paired"]},
+        ],
     },
     "check": check_example_6,
     "output_hid": 8,
 }
```

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/testcase.py` & `galaxy-test-base-23.0.2/galaxy_test/base/testcase.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import logging
 import os
-import unittest
-from typing import Any, Optional
+from typing import (
+    Any,
+    Optional,
+)
 
 from galaxy.tool_util.verify.test_data import TestDataResolver
-from galaxy_test.base.env import setup_keep_outdir, target_url_parts
+from galaxy.util.unittest import TestCase
+from galaxy_test.base.env import (
+    setup_keep_outdir,
+    target_url_parts,
+)
 
 log = logging.getLogger(__name__)
 
 
-class FunctionalTestCase(unittest.TestCase):
+class FunctionalTestCase(TestCase):
     """Base class for tests targetting actual Galaxy servers.
 
     Subclass should override galaxy_driver_class if a Galaxy server
     needs to be launched to run the test, this base class assumes a
     server is already running.
     """
+
     galaxy_driver_class: Optional[type] = None
-    history_id: Optional[str]
     host: str
     port: Optional[str]
     url: str
     keepOutdir: str
     test_data_resolver: TestDataResolver
     _test_driver: Optional[Any]
 
     def setUp(self) -> None:
-        self.history_id = os.environ.get('GALAXY_TEST_HISTORY_ID', None)
         self.host, self.port, self.url = target_url_parts()
-        server_wrapper = self._test_driver and self._test_driver.server_wrappers[0]
+        server_wrapper = (
+            self._test_driver and self._test_driver.server_wrappers and self._test_driver.server_wrappers[0]
+        )
         if server_wrapper:
             self.host = server_wrapper.host
             self.port = server_wrapper.port
             self.url = f"http://{self.host}:{self.port}{server_wrapper.prefix.rstrip('/')}/"
         self.test_data_resolver = TestDataResolver()
         self.keepOutdir = setup_keep_outdir()
```

### Comparing `galaxy-test-base-22.1.1/galaxy_test/base/workflow_fixtures.py` & `galaxy-test-base-23.0.2/galaxy_test/base/workflow_fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,14 +174,29 @@
   text_input: |
     a
     b
     c
     d
 """
 
+WORKFLOW_WITH_MAPPED_OUTPUT_COLLECTION = """
+class: GalaxyWorkflow
+inputs:
+  input1:
+    type: data_collection_input
+    collection_type: list
+outputs:
+  wf_output_1:
+    outputSource: first_cat/out_file1
+steps:
+  first_cat:
+    tool_id: cat
+    in:
+      input1: input1
+"""
 
 WORKFLOW_WITH_DYNAMIC_OUTPUT_COLLECTION = """
 class: GalaxyWorkflow
 inputs:
   text_input1: data
   text_input2: data
 steps:
@@ -444,14 +459,26 @@
       input1: input1
   second_cat:
     tool_id: cat1
     in:
       input1: first_cat/out_file1
 """
 
+WORKFLOW_INPUTS_AS_OUTPUTS = """
+class: GalaxyWorkflow
+inputs:
+  input1: data
+  text_input: text
+outputs:
+  wf_output_1:
+    outputSource: input1
+  wf_output_param:
+    outputSource: text_input
+steps: []
+"""
 
 WORKFLOW_PARAMETER_INPUT_INTEGER_REQUIRED = """
 class: GalaxyWorkflow
 inputs:
   data_input: data
   int_input: integer
 steps:
@@ -583,14 +610,52 @@
     in:
       f1: input1
     out:
       out1: out1
 """
 
 
+WORKFLOW_OPTIONAL_INPUT_DELAYED_SCHEDULING = """
+class: GalaxyWorkflow
+inputs:
+  required:
+    type: data
+  optional:
+    type: data
+    optional: true
+outputs:
+  out1:
+    outputSource: count_multi_file/out_file1
+steps:
+  expression:
+    tool_id: expression_parse_int
+    state:
+      input1: 1
+  head:
+    tool_id: head
+    in:
+      input: required
+    state:
+      lineNum:
+        $link:  expression/out1
+  count_multi_file:
+    tool_id: count_multi_file
+    in:
+      input1:
+      - optional
+      - head/out_file1
+    out:
+      out_file1: out_file1
+test_data:
+  required:
+    value: 1.bed
+    type: File
+"""
+
+
 WORKFLOW_RUNTIME_PARAMETER_SIMPLE = """
 class: GalaxyWorkflow
 inputs:
   input1: data
 steps:
   random:
     tool_id: random_lines1
@@ -894,7 +959,95 @@
 input_list:
   collection_type: list
   elements:
     - identifier: i1
       content: "0"
   name: example list
 """
+
+
+WORKFLOW_WITH_BAD_COLUMN_PARAMETER = """
+class: GalaxyWorkflow
+inputs:
+    bed_input: data
+steps:
+  cat1:
+    tool_id: cat1
+    in:
+      input1: bed_input
+  column_param_list:
+    tool_id: column_param
+    in:
+      input1: cat1/out_file1
+    state:
+      col: 9
+      col_names: notacolumn
+"""
+
+
+WORKFLOW_WITH_BAD_COLUMN_PARAMETER_GOOD_TEST_DATA = """
+step_parameters:
+  '2':
+    'col': 1
+    'col_names': 'c1: chr1'
+bed_input:
+  value: 1.bed
+  file_type: bed
+  type: File
+"""
+
+
+NESTED_WORKFLOW_WITH_CONDITIONAL_SUBWORKFLOW_AND_DISCONNECTED_MAP_OVER_SOURCE = """
+class: GalaxyWorkflow
+inputs:
+  boolean_input_files: collection
+steps:
+  create_list_of_boolean:
+    tool_id: param_value_from_file
+    in:
+       input1: boolean_input_files
+    state:
+      param_type: boolean
+  subworkflow:
+    run:
+      class: GalaxyWorkflow
+      inputs:
+        boolean_input_file: data
+        should_run: boolean
+      steps:
+        create_more_inputs:
+          tool_id: collection_creates_dynamic_nested
+        consume_expression_parameter:
+          tool_id: cat1
+          state:
+            input1:
+              $link: create_more_inputs/list_output
+            queries:
+              - input2:
+                $link: boolean_input_file
+          out:
+            out_file1:
+              change_datatype: txt
+        consume_expression_parameter_2:
+          tool_id: cat1
+          state:
+            input1:
+              $link: consume_expression_parameter/out_file1
+      outputs:
+        inner_create_nested:
+          outputSource: create_more_inputs/list_output
+        inner_output_1:
+          outputSource: consume_expression_parameter/out_file1
+        inner_output_2:
+          outputSource: consume_expression_parameter_2/out_file1
+    in:
+      boolean_input_file: boolean_input_files
+      should_run: create_list_of_boolean/boolean_param
+    when: $(inputs.should_run)
+outputs:
+  outer_create_nested:
+    outputSource: subworkflow/inner_create_nested
+  outer_output_1:
+    outputSource: subworkflow/inner_output_1
+  outer_output_2:
+    outputSource: subworkflow/inner_output_2
+"""
```

### Comparing `galaxy-test-base-22.1.1/galaxy_test_base.egg-info/PKG-INFO` & `galaxy-test-base-23.0.2/galaxy_test_base.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,77 @@
 Metadata-Version: 2.1
 Name: galaxy-test-base
-Version: 22.1.1
-Summary: Galaxy Testing Utilities
+Version: 23.0.2
+Summary: Galaxy testing utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-test-base.svg
    :target: https://pypi.org/project/galaxy-test-base/
 
 
 
 Overview
 --------
 
 The Galaxy_ testing base package.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.1.dev0
----------------------
+-------------------
+23.0.2 (2023-06-13)
+-------------------
+
+No recorded changes since last release
 
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
 
----------------------
+=========
+Bug fixes
+=========
+
+* Ensure history export contains all expected datasets by `@davelopez <https://github.com/davelopez>`_ in `#16013 <https://github.com/galaxyproject/galaxy/pull/16013>`_
+* Fix extended metadata file size handling by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16109 <https://github.com/galaxyproject/galaxy/pull/16109>`_
+
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * Initial release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * Initial import from the 20.05 branch of Galaxy.
-
-
```

### Comparing `galaxy-test-base-22.1.1/galaxy_test_base.egg-info/SOURCES.txt` & `galaxy-test-base-23.0.2/galaxy_test_base.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 HISTORY.rst
 LICENSE
 MANIFEST.in
-Makefile
 README.rst
 dev-requirements.txt
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 test-requirements.txt
-galaxy/__init__.py
-galaxy/project_galaxy_test_base.py
 galaxy_test/__init__.py
+galaxy_test/py.typed
 galaxy_test/base/__init__.py
 galaxy_test/base/api.py
 galaxy_test/base/api_asserts.py
 galaxy_test/base/api_util.py
 galaxy_test/base/constants.py
+galaxy_test/base/decorators.py
 galaxy_test/base/env.py
-galaxy_test/base/instrument.py
 galaxy_test/base/interactor.py
-galaxy_test/base/nose_util.py
+galaxy_test/base/json_schema_utils.py
 galaxy_test/base/populators.py
 galaxy_test/base/rules_test_data.py
 galaxy_test/base/testcase.py
-galaxy_test/base/tool_sheds_conf.xml
-galaxy_test/base/uses_shed.py
+galaxy_test/base/uses_shed_api.py
 galaxy_test/base/workflow_fixtures.py
 galaxy_test/base/data/minimal_tool_no_id.json
 galaxy_test/base/data/test_subworkflow_with_integer_input.ga
 galaxy_test/base/data/test_workflow_1.ga
 galaxy_test/base/data/test_workflow_2.ga
 galaxy_test/base/data/test_workflow_batch.ga
 galaxy_test/base/data/test_workflow_map_reduce_pause.ga
@@ -42,14 +38,9 @@
 galaxy_test/base/data/test_workflow_two_random_lines.ga
 galaxy_test/base/data/test_workflow_validation_1.ga
 galaxy_test/base/data/test_workflow_with_input_tags.ga
 galaxy_test/base/data/test_workflow_with_runtime_input.ga
 galaxy_test_base.egg-info/PKG-INFO
 galaxy_test_base.egg-info/SOURCES.txt
 galaxy_test_base.egg-info/dependency_links.txt
-galaxy_test_base.egg-info/entry_points.txt
-galaxy_test_base.egg-info/not-zip-safe
 galaxy_test_base.egg-info/requires.txt
-galaxy_test_base.egg-info/top_level.txt
-scripts/commit_version.py
-scripts/new_version.py
-scripts/print_version_for_release.py
+galaxy_test_base.egg-info/top_level.txt
```

