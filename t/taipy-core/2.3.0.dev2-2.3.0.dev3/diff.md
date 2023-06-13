# Comparing `tmp/taipy-core-2.3.0.dev2.tar.gz` & `tmp/taipy-core-2.3.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-core-2.3.0.dev2.tar", last modified: Thu Jun  8 19:30:39 2023, max compression
+gzip compressed data, was "taipy-core-2.3.0.dev3.tar", last modified: Tue Jun 13 17:44:43 2023, max compression
```

## Comparing `taipy-core-2.3.0.dev2.tar` & `taipy-core-2.3.0.dev3.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.011577 taipy-core-2.3.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-08 19:30:39.011577 taipy-core-2.3.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:30:39.011577 taipy-core-2.3.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.987577 taipy-core-2.3.0.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.987577 taipy-core-2.3.0.dev2/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.987577 taipy-core-2.3.0.dev2/src/taipy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.987577 taipy-core-2.3.0.dev2/src/taipy/core/_backup/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_backup/_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_core_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.987577 taipy-core-2.3.0.dev2/src/taipy/core/_entity/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_labeled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_reload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_submittable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.991577 taipy-core-2.3.0.dev2/src/taipy/core/_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_manager/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_manager/_manager_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.991577 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_abstract_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.991577 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_orchestrator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.991577 taipy-core-2.3.0.dev2/src/taipy/core/_repository/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/_filesystem_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/_repository_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/_sql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.991577 taipy-core-2.3.0.dev2/src/taipy/core/_version/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.995577 taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/_bcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/_version_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.995577 taipy-core-2.3.0.dev2/src/taipy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/_listattributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/default_custom_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/warn_if_inputs_not_ready.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.995577 taipy-core-2.3.0.dev2/src/taipy/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/_core_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.995577 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_config_id_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_data_node_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_global_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_job_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_pipeline_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_scenario_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_task_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/config.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    49075 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/data_node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/job_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/scenario_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/task_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.999577 taipy-core-2.3.0.dev2/src/taipy/core/cycle/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/cycle_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.003577 taipy-core-2.3.0.dev2/src/taipy/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/abstract_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/abstract_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    21520 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/data_node_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.003577 taipy-core-2.3.0.dev2/src/taipy/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.003577 taipy-core-2.3.0.dev2/src/taipy/core/job/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/job_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.003577 taipy-core-2.3.0.dev2/src/taipy/core/notification/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/core_event_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/registration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.007577 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/pipeline_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.007577 taipy-core-2.3.0.dev2/src/taipy/core/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13465 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/scenario_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    26101 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/taipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.007577 taipy-core-2.3.0.dev2/src/taipy/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/task_id.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.007577 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-08 19:30:38.000000 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-08 19:30:38.000000 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:30:38.000000 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:30:31.000000 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-08 19:30:38.000000 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 19:30:38.000000 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.011577 taipy-core-2.3.0.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/tests/test_complex_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    30198 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/tests/test_taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.193087 taipy-core-2.3.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-13 17:44:43.193087 taipy-core-2.3.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:44:43.193087 taipy-core-2.3.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-13 17:44:35.000000 taipy-core-2.3.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.165086 taipy-core-2.3.0.dev3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.165086 taipy-core-2.3.0.dev3/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.169086 taipy-core-2.3.0.dev3/src/taipy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.169086 taipy-core-2.3.0.dev3/src/taipy/core/_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_backup/_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_core_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.169086 taipy-core-2.3.0.dev3/src/taipy/core/_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_entity/_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_entity/_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_entity/_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_entity/_labeled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_entity/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_entity/_reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_entity/_submittable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.169086 taipy-core-2.3.0.dev3/src/taipy/core/_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_manager/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_manager/_manager_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.169086 taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_abstract_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.169086 taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_orchestrator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.173086 taipy-core-2.3.0.dev3/src/taipy/core/_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_repository/_filesystem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_repository/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_repository/_repository_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_repository/_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_repository/_sql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_repository/_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.173086 taipy-core-2.3.0.dev3/src/taipy/core/_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.173086 taipy-core-2.3.0.dev3/src/taipy/core/_version/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_version/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_version/_cli/_bcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_version/_cli/_version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_version/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_version/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.173086 taipy-core-2.3.0.dev3/src/taipy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/common/_listattributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/common/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/common/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/common/default_custom_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/common/warn_if_inputs_not_ready.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.177086 taipy-core-2.3.0.dev3/src/taipy/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.177086 taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_config_id_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_data_node_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_global_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_job_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_pipeline_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_scenario_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_task_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/core_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49075 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/data_node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/job_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/scenario_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/config/task_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.177086 taipy-core-2.3.0.dev3/src/taipy/core/cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/cycle/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/cycle/cycle_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.181086 taipy-core-2.3.0.dev3/src/taipy/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/_data_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/_data_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/_data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/_data_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/_data_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/abstract_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/abstract_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21520 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/data_node_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/data/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.181086 taipy-core-2.3.0.dev3/src/taipy/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.185087 taipy-core-2.3.0.dev3/src/taipy/core/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/job/_job_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/job/_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/job/_job_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/job/_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/job/_job_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/job/_job_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/job/_job_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/job/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/job/job_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/job/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.185087 taipy-core-2.3.0.dev3/src/taipy/core/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/notification/core_event_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/notification/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/notification/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/notification/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/notification/registration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/notification/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.189087 taipy-core-2.3.0.dev3/src/taipy/core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/pipeline/pipeline_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.189087 taipy-core-2.3.0.dev3/src/taipy/core/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/scenario/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/scenario/scenario_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26101 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.189087 taipy-core-2.3.0.dev3/src/taipy/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/task/_task_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/task/_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/task/_task_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/task/_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/task/_task_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/task/_task_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/task/_task_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/task/task_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/src/taipy/core/version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.193087 taipy-core-2.3.0.dev3/src/taipy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-13 17:44:43.000000 taipy-core-2.3.0.dev3/src/taipy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-13 17:44:43.000000 taipy-core-2.3.0.dev3/src/taipy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:44:43.000000 taipy-core-2.3.0.dev3/src/taipy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:44:36.000000 taipy-core-2.3.0.dev3/src/taipy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-13 17:44:43.000000 taipy-core-2.3.0.dev3/src/taipy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 17:44:43.000000 taipy-core-2.3.0.dev3/src/taipy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:43.193087 taipy-core-2.3.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/tests/test_complex_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30198 2023-06-13 17:44:30.000000 taipy-core-2.3.0.dev3/tests/test_taipy.py
```

### Comparing `taipy-core-2.3.0.dev2/LICENSE` & `taipy-core-2.3.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/PKG-INFO` & `taipy-core-2.3.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.3.0.dev2
+Version: 2.3.0.dev3
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.3.0.dev2/README.md` & `taipy-core-2.3.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/setup.py` & `taipy-core-2.3.0.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "pyarrow>=10.0.1,<11.0",
     "networkx>=2.6,<3.0",
     "openpyxl>=3.0.7,<3.1",
     "modin[dask]>=0.16.2,<1.0",
     "pymongo>=4.2.0,<5.0",
     "sqlalchemy>=1.4,<2.0",
     "toml>=0.10,<0.11",
-    "taipy-config>=2.3.0.dev0",
+    "taipy-config==2.3.0.dev3",
 ]
 
 test_requirements = ["pytest>=3.8"]
 
 extras_require = {
     "fastparquet": ["fastparquet==2022.11.0"],
     "mssql": ["pyodbc>=4,<4.1"],
```

### Comparing `taipy-core-2.3.0.dev2/src/taipy/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,28 +24,62 @@
         from taipy.core.job.job import Job
         from taipy.core.job.job_id import JobId
         from taipy.core.job.status import Status
         from taipy.core.pipeline.pipeline import Pipeline
         from taipy.core.pipeline.pipeline_id import PipelineId
         from taipy.core.scenario.scenario import Scenario
         from taipy.core.scenario.scenario_id import ScenarioId
+        from taipy.core.taipy import (
+            cancel_job,
+            clean_all_entities,
+            clean_all_entities_by_version,
+            compare_scenarios,
+            create_pipeline,
+            create_scenario,
+            delete,
+            delete_job,
+            delete_jobs,
+            export_scenario,
+            get,
+            get_cycles,
+            get_cycles_scenarios,
+            get_data_nodes,
+            get_jobs,
+            get_latest_job,
+            get_parents,
+            get_pipelines,
+            get_primary,
+            get_primary_scenarios,
+            get_scenarios,
+            get_tasks,
+            is_deletable,
+            set,
+            set_primary,
+            submit,
+            subscribe_pipeline,
+            subscribe_scenario,
+            tag,
+            unsubscribe_pipeline,
+            unsubscribe_scenario,
+            untag,
+        )
         from taipy.core.task.task import Task
         from taipy.core.task.task_id import TaskId
 
     if find_spec("taipy.gui"):
         from taipy.gui import Gui
 
         if find_spec("taipy.gui_core"):
-            from taipy.gui_core.GuiCoreLib import GuiCore
+            from taipy.gui_core.GuiCoreLib import _GuiCore
 
-            Gui.add_library(GuiCore())
+            Gui.add_library(_GuiCore())
 
         if find_spec("taipy.enterprise") and find_spec("taipy.enterprise.gui"):
             from taipy.enterprise.gui import _init_gui_enterprise
 
             _init_gui_enterprise(Gui)
 
     if find_spec("taipy.rest"):
         from taipy.rest import Rest
 
     if find_spec("taipy._run"):
-        pass
+        from taipy._run import _run as run
```

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_backup/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_backup/_backup.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_backup/_backup.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_core.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_core.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_core_cli.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_core_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_entity/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_dag.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_entity/_dag.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_entity.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_entity/_entity.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_entity_ids.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_entity/_entity_ids.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_labeled.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_entity/_labeled.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_properties.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_entity/_properties.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_reload.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_entity/_reload.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_submittable.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_entity/_submittable.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_manager/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_manager/_manager.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_manager/_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_manager/_manager_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_manager/_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_abstract_orchestrator.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_abstract_orchestrator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_orchestrator.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_orchestrator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_orchestrator_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/_orchestrator_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/utils.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_orchestrator/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_repository/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_repository/_filesystem_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_repository/_filesystem_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_repository/_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_repository/_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_repository/_repository_adapter.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_repository/_repository_adapter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_repository/_repository_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_repository/_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_repository/_sql_model.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_repository/_sql_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_repository/_sql_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_repository/_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_version/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_version/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_version/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/_bcolor.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_version/_cli/_bcolor.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/_version_cli.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_version/_cli/_version_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_version/_utils.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_version/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_version/_version.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_fs_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_manager.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_manager_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_model.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_repository_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_sql_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/_version/_version_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/common/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/common/_listattributes.py` & `taipy-core-2.3.0.dev3/src/taipy/core/common/_listattributes.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/common/_repr_enum.py` & `taipy-core-2.3.0.dev3/src/taipy/core/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/common/_utils.py` & `taipy-core-2.3.0.dev3/src/taipy/core/common/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/common/_warnings.py` & `taipy-core-2.3.0.dev3/src/taipy/core/common/_warnings.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/common/default_custom_document.py` & `taipy-core-2.3.0.dev3/src/taipy/core/common/default_custom_document.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/common/warn_if_inputs_not_ready.py` & `taipy-core-2.3.0.dev3/src/taipy/core/common/warn_if_inputs_not_ready.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 from taipy.config import _inject_section
 from taipy.config.checker._checker import _Checker
 from taipy.config.common.frequency import Frequency  # type: ignore
 from taipy.config.common.scope import Scope  # type: ignore
 from taipy.config.config import Config  # type: ignore
 from taipy.config.global_app.global_app_config import GlobalAppConfig  # type: ignore
 
-from ._core_section import CoreSection
 from .checkers import _global_config_checker
 from .checkers._config_id_checker import _ConfigIdChecker
 from .checkers._data_node_config_checker import _DataNodeConfigChecker
 from .checkers._job_config_checker import _JobConfigChecker
 from .checkers._pipeline_config_checker import _PipelineConfigChecker
 from .checkers._scenario_config_checker import _ScenarioConfigChecker
 from .checkers._task_config_checker import _TaskConfigChecker
+from .core_section import CoreSection
 from .data_node_config import DataNodeConfig
 from .job_config import JobConfig
 from .pipeline_config import PipelineConfig
 from .scenario_config import ScenarioConfig
 from .task_config import TaskConfig
 
 _inject_section(
```

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/_core_section.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/core_section.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     @staticmethod
     def _configure(
         mode: Optional[str] = None,
         version_number: Optional[str] = None,
         force: Optional[bool] = None,
         clean_entities: Optional[bool] = None,
         **properties,
-    ):
+    ) -> "CoreSection":
         """Configure the Core service.
 
         Parameters:
             mode (Optional[str], optional): Indicates the mode of the version management system.
                 Possible values are *"development"*, *"experiment"*, or *"production"*.
             version_number (Optional[str], optional): The string identifier of the version.
                  In development mode, the version number is ignored.
```

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_config_id_checker.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_config_id_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_data_node_config_checker.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_data_node_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_global_config_checker.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_global_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_job_config_checker.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_job_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_pipeline_config_checker.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_pipeline_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_scenario_config_checker.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_scenario_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_task_config_checker.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/checkers/_task_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/config.schema.json` & `taipy-core-2.3.0.dev3/src/taipy/core/config/config.schema.json`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/data_node_config.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/data_node_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/job_config.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/job_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/pipeline_config.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/scenario_config.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/scenario_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/config/task_config.py` & `taipy-core-2.3.0.dev3/src/taipy/core/config/task_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/cycle/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_fs_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_manager.py` & `taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_manager_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_model.py` & `taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_repository_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_sql_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/cycle/_cycle_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/cycle/cycle.py` & `taipy-core-2.3.0.dev3/src/taipy/core/cycle/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/cycle/cycle_id.py` & `taipy-core-2.3.0.dev3/src/taipy/core/cycle/cycle_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_fs_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/_data_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_manager.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/_data_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import os
-from typing import Dict, Iterable, Optional, Set, Union
+from typing import Dict, Iterable, List, Optional, Set, Union
 
 from taipy.config._config import _Config
 from taipy.config.common.scope import Scope
 from taipy.config.config import Config
 
 from .._backup._backup import _append_to_backup_file, _remove_from_backup_file
 from .._manager._manager import _Manager
@@ -37,19 +37,20 @@
     _repository = _DataRepositoryFactory._build_repository()  # type: ignore
     _ENTITY_NAME = DataNode.__name__
     _EVENT_ENTITY_TYPE = EventEntityType.DATA_NODE
 
     @classmethod
     def _bulk_get_or_create(
         cls,
-        data_node_configs: Set[DataNodeConfig],
+        data_node_configs: List[DataNodeConfig],
         cycle_id: Optional[CycleId] = None,
         scenario_id: Optional[ScenarioId] = None,
         pipeline_id: Optional[PipelineId] = None,
     ) -> Dict[DataNodeConfig, DataNode]:
+        data_node_configs = [Config.data_nodes[dnc.id] for dnc in data_node_configs]
         dn_configs_and_owner_id = []
         for dn_config in data_node_configs:
             scope = dn_config.scope
             owner_id: Union[Optional[PipelineId], Optional[ScenarioId], Optional[CycleId]]
             if scope == Scope.PIPELINE:
                 owner_id = pipeline_id
             elif scope == Scope.SCENARIO:
```

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_manager_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/_data_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_model.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/_data_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/_data_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_repository_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/_data_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_sql_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/_data_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/_filter.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/_filter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/abstract_file.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/abstract_file.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/abstract_sql.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/abstract_sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/csv.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/csv.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/data_node.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/data_node.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/data_node_id.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/data_node_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/excel.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/excel.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/generic.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/generic.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/in_memory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/in_memory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/json.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/json.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/mongo.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/mongo.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/operator.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/operator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/parquet.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/parquet.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/pickle.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/pickle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/sql.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/data/sql_table.py` & `taipy-core-2.3.0.dev3/src/taipy/core/data/sql_table.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/exceptions/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/exceptions/exceptions.py` & `taipy-core-2.3.0.dev3/src/taipy/core/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/job/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_fs_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/job/_job_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_manager.py` & `taipy-core-2.3.0.dev3/src/taipy/core/job/_job_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_manager_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/job/_job_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_model.py` & `taipy-core-2.3.0.dev3/src/taipy/core/job/_job_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/job/_job_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_repository_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/job/_job_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_sql_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/job/_job_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/job/job.py` & `taipy-core-2.3.0.dev3/src/taipy/core/job/job.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/job/job_id.py` & `taipy-core-2.3.0.dev3/src/taipy/core/job/job_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/job/status.py` & `taipy-core-2.3.0.dev3/src/taipy/core/job/status.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/notification/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/notification/core_event_consumer.py` & `taipy-core-2.3.0.dev3/src/taipy/core/notification/core_event_consumer.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/notification/event.py` & `taipy-core-2.3.0.dev3/src/taipy/core/notification/event.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/notification/notifier.py` & `taipy-core-2.3.0.dev3/src/taipy/core/notification/notifier.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/notification/registration.py` & `taipy-core-2.3.0.dev3/src/taipy/core/notification/registration.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/notification/registration_id.py` & `taipy-core-2.3.0.dev3/src/taipy/core/notification/registration_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/notification/topic.py` & `taipy-core-2.3.0.dev3/src/taipy/core/notification/topic.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_fs_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_manager.py` & `taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from functools import partial
 from typing import Any, Callable, List, Optional, Union
 
+from taipy import Config
 from taipy.config.common.scope import Scope
 
 from .._entity._entity_ids import _EntityIds
 from .._manager._manager import _Manager
 from .._version._version_manager_factory import _VersionManagerFactory
 from ..common.warn_if_inputs_not_ready import _warn_if_inputs_not_ready
 from ..config.pipeline_config import PipelineConfig
@@ -82,16 +83,17 @@
         cls,
         pipeline_config: PipelineConfig,
         cycle_id: Optional[CycleId] = None,
         scenario_id: Optional[ScenarioId] = None,
     ) -> Pipeline:
         pipeline_id = Pipeline._new_id(str(pipeline_config.id))
 
+        task_configs = [Config.tasks[t.id] for t in pipeline_config.task_configs]
         task_manager = _TaskManagerFactory._build_manager()
-        tasks = task_manager._bulk_get_or_create(pipeline_config.task_configs, cycle_id, scenario_id, pipeline_id)
+        tasks = task_manager._bulk_get_or_create(task_configs, cycle_id, scenario_id, pipeline_id)
 
         scope = min(task.scope for task in tasks) if len(tasks) != 0 else Scope.GLOBAL
         owner_id: Union[Optional[PipelineId], Optional[ScenarioId], Optional[CycleId]]
         if scope == Scope.PIPELINE:
             owner_id = pipeline_id
         elif scope == Scope.SCENARIO:
             owner_id = scenario_id
```

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_manager_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_model.py` & `taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_repository_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_sql_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/pipeline/_pipeline_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/pipeline.py` & `taipy-core-2.3.0.dev3/src/taipy/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/pipeline_id.py` & `taipy-core-2.3.0.dev3/src/taipy/core/pipeline/pipeline_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/scenario/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_fs_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_manager.py` & `taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,23 +92,26 @@
     @classmethod
     def _create(
         cls,
         config: ScenarioConfig,
         creation_date: Optional[datetime.datetime] = None,
         name: Optional[str] = None,
     ) -> Scenario:
+        config = Config.scenarios[config.id]
         scenario_id = Scenario._new_id(str(config.id))
         cycle = (
             _CycleManagerFactory._build_manager()._get_or_create(config.frequency, creation_date)
             if config.frequency
             else None
         )
 
         pipelines = [
-            _PipelineManagerFactory._build_manager()._get_or_create(p_config, cycle.id if cycle else None, scenario_id)
+            _PipelineManagerFactory._build_manager()._get_or_create(
+                Config.pipelines[p_config.id], cycle.id if cycle else None, scenario_id
+            )
             for p_config in config.pipeline_configs
         ]
 
         is_primary_scenario = len(cls._get_all_by_cycle(cycle)) == 0 if cycle else False
         props = config._properties.copy()
         if name:
             props["name"] = name
```

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_manager_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_model.py` & `taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_repository_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_sql_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/scenario/_scenario_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/scenario/scenario.py` & `taipy-core-2.3.0.dev3/src/taipy/core/scenario/scenario.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/scenario/scenario_id.py` & `taipy-core-2.3.0.dev3/src/taipy/core/scenario/scenario_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/taipy.py` & `taipy-core-2.3.0.dev3/src/taipy/core/taipy.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/task/__init__.py` & `taipy-core-2.3.0.dev3/src/taipy/core/task/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_fs_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/task/_task_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_manager.py` & `taipy-core-2.3.0.dev3/src/taipy/core/task/_task_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from typing import Callable, List, Optional, Type, Union
 
+from taipy.config import Config
 from taipy.config.common.scope import Scope
 
 from .._entity._entity_ids import _EntityIds
 from .._manager._manager import _Manager
 from .._orchestrator._abstract_orchestrator import _AbstractOrchestrator
 from .._orchestrator._orchestrator_factory import _OrchestratorFactory
 from .._version._version_manager_factory import _VersionManagerFactory
@@ -53,24 +54,25 @@
         task_configs: List[TaskConfig],
         cycle_id: Optional[CycleId] = None,
         scenario_id: Optional[ScenarioId] = None,
         pipeline_id: Optional[PipelineId] = None,
     ) -> List[Task]:
         data_node_configs = set()
         for task_config in task_configs:
-            data_node_configs.update(task_config.input_configs)
-            data_node_configs.update(task_config.output_configs)
+            data_node_configs.update([Config.data_nodes[dnc.id] for dnc in task_config.input_configs])
+            data_node_configs.update([Config.data_nodes[dnc.id] for dnc in task_config.output_configs])
 
         data_nodes = _DataManagerFactory._build_manager()._bulk_get_or_create(
-            data_node_configs, cycle_id, scenario_id, pipeline_id
+            list(data_node_configs), cycle_id, scenario_id, pipeline_id
         )
-
         tasks_configs_and_owner_id = []
         for task_config in task_configs:
-            task_dn_configs = task_config.output_configs + task_config.input_configs
+            task_dn_configs = [Config.data_nodes[dnc.id] for dnc in task_config.output_configs] + [
+                Config.data_nodes[dnc.id] for dnc in task_config.input_configs
+            ]
             task_config_data_nodes = [data_nodes[dn_config] for dn_config in task_dn_configs]
             scope = min(dn.scope for dn in task_config_data_nodes) if len(task_config_data_nodes) != 0 else Scope.GLOBAL
             owner_id: Union[Optional[PipelineId], Optional[ScenarioId], Optional[CycleId]]
             if scope == Scope.PIPELINE:
                 owner_id = pipeline_id
             elif scope == Scope.SCENARIO:
                 owner_id = scenario_id
@@ -85,16 +87,22 @@
 
         tasks = []
         for task_config, owner_id in tasks_configs_and_owner_id:
             if task := tasks_by_config.get((task_config, owner_id)):
                 tasks.append(task)
             else:
                 version = _VersionManagerFactory._build_manager()._get_latest_version()
-                inputs = [data_nodes[input_config] for input_config in task_config.input_configs]
-                outputs = [data_nodes[output_config] for output_config in task_config.output_configs]
+                inputs = [
+                    data_nodes[input_config]
+                    for input_config in [Config.data_nodes[dnc.id] for dnc in task_config.input_configs]
+                ]
+                outputs = [
+                    data_nodes[output_config]
+                    for output_config in [Config.data_nodes[dnc.id] for dnc in task_config.output_configs]
+                ]
                 skippable = task_config.skippable
                 task = Task(
                     str(task_config.id),
                     dict(**task_config._properties),
                     task_config.function,
                     inputs,
                     outputs,
```

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_manager_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/task/_task_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_model.py` & `taipy-core-2.3.0.dev3/src/taipy/core/task/_task_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/task/_task_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_repository_factory.py` & `taipy-core-2.3.0.dev3/src/taipy/core/task/_task_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_sql_repository.py` & `taipy-core-2.3.0.dev3/src/taipy/core/task/_task_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/task/task.py` & `taipy-core-2.3.0.dev3/src/taipy/core/task/task.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy/core/task/task_id.py` & `taipy-core-2.3.0.dev3/src/taipy/core/task/task_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/src/taipy_core.egg-info/PKG-INFO` & `taipy-core-2.3.0.dev3/src/taipy_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.3.0.dev2
+Version: 2.3.0.dev3
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.3.0.dev2/src/taipy_core.egg-info/SOURCES.txt` & `taipy-core-2.3.0.dev3/src/taipy_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 src/taipy/core/common/_listattributes.py
 src/taipy/core/common/_repr_enum.py
 src/taipy/core/common/_utils.py
 src/taipy/core/common/_warnings.py
 src/taipy/core/common/default_custom_document.py
 src/taipy/core/common/warn_if_inputs_not_ready.py
 src/taipy/core/config/__init__.py
-src/taipy/core/config/_core_section.py
 src/taipy/core/config/config.schema.json
+src/taipy/core/config/core_section.py
 src/taipy/core/config/data_node_config.py
 src/taipy/core/config/job_config.py
 src/taipy/core/config/pipeline_config.py
 src/taipy/core/config/scenario_config.py
 src/taipy/core/config/task_config.py
 src/taipy/core/config/checkers/__init__.py
 src/taipy/core/config/checkers/_config_id_checker.py
```

### Comparing `taipy-core-2.3.0.dev2/tests/test_complex_application.py` & `taipy-core-2.3.0.dev3/tests/test_complex_application.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev2/tests/test_taipy.py` & `taipy-core-2.3.0.dev3/tests/test_taipy.py`

 * *Files identical despite different names*

