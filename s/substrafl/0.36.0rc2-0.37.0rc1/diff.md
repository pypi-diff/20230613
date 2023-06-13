# Comparing `tmp/substrafl-0.36.0rc2.tar.gz` & `tmp/substrafl-0.37.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrafl-0.36.0rc2.tar", last modified: Thu May 11 15:07:46 2023, max compression
+gzip compressed data, was "substrafl-0.37.0rc1.tar", last modified: Tue Jun 13 15:16:46 2023, max compression
```

## Comparing `substrafl-0.36.0rc2.tar` & `substrafl-0.37.0rc1.tar`

### file list

```diff
@@ -1,71 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.109447 substrafl-0.36.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 15:07:46.109447 substrafl-0.36.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:07:46.109447 substrafl-0.36.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.097447 substrafl-0.36.0rc2/substrafl/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.101447 substrafl-0.36.0rc2/substrafl/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.101447 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_base_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_fed_pca_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    23421 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_scaffold_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_single_organization_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/algorithms/pytorch/weight_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/evaluation_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.101447 substrafl-0.36.0rc2/substrafl/index_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/index_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/index_generator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/index_generator/np_index_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/model_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.105447 substrafl-0.36.0rc2/substrafl/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/aggregation_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.105447 substrafl-0.36.0rc2/substrafl/nodes/references/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/references/local_state.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/references/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/test_data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/nodes/train_data_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.105447 substrafl-0.36.0rc2/substrafl/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.105447 substrafl-0.36.0rc2/substrafl/remote/register/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/register/generate_wheel.py
--rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/register/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/remote_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.105447 substrafl-0.36.0rc2/substrafl/remote/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/serializers/pickle_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/serializers/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/remote/substratools_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.109447 substrafl-0.36.0rc2/substrafl/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/fed_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/fed_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/newton_raphson.py
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/single_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-05-11 15:07:40.000000 substrafl-0.36.0rc2/substrafl/strategies/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:07:46.101447 substrafl-0.36.0rc2/substrafl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-11 15:07:45.000000 substrafl-0.36.0rc2/substrafl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-11 15:07:46.000000 substrafl-0.36.0rc2/substrafl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:07:45.000000 substrafl-0.36.0rc2/substrafl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-11 15:07:45.000000 substrafl-0.36.0rc2/substrafl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-11 15:07:45.000000 substrafl-0.36.0rc2/substrafl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23454 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/algorithms/pytorch/weight_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/compute_plan_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/dependency/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/dependency/path_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/dependency/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/evaluation_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl/index_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/index_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/index_generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/index_generator/np_index_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/model_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/aggregation_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/substrafl/nodes/references/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/references/local_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/references/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/test_data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/nodes/train_data_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/substrafl/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/substrafl/remote/register/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/register/manage_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/register/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/remote_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/substrafl/remote/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/serializers/pickle_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/serializers/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/remote/substratools_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.180891 substrafl-0.37.0rc1/substrafl/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/fed_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/fed_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/newton_raphson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/single_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-13 15:16:43.000000 substrafl-0.37.0rc1/substrafl/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:16:46.176890 substrafl-0.37.0rc1/substrafl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-13 15:16:45.000000 substrafl-0.37.0rc1/substrafl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-13 15:16:46.000000 substrafl-0.37.0rc1/substrafl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:16:45.000000 substrafl-0.37.0rc1/substrafl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-13 15:16:45.000000 substrafl-0.37.0rc1/substrafl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 15:16:45.000000 substrafl-0.37.0rc1/substrafl.egg-info/top_level.txt
```

### Comparing `substrafl-0.36.0rc2/LICENSE` & `substrafl-0.37.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/PKG-INFO` & `substrafl-0.37.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.36.0rc2
+Version: 0.37.0rc1
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.36.0rc2/README.md` & `substrafl-0.37.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/pyproject.toml` & `substrafl-0.37.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/setup.py` & `substrafl-0.37.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,21 +38,22 @@
     packages=find_packages(exclude=["tests*", "benchmark*"]),
     # Not compatible with substratools 0.8.0 because
     # that release is private and in the Docker container
     # it has access only to the public PyPi
     install_requires=[
         "numpy>=1.20.3,!=1.24.*",
         "cloudpickle>=1.6.0",
-        "substra~=0.44.0rc1",
+        "substra~=0.45.0rc1",
         "substratools~=0.20.0",
         "pydantic>=1.9.0",
         "pip>=21.2",
         "wheel",
         "six",
         "packaging",
+        "pip-tools",
     ],
     extras_require={
         "dev": [
             "pytest>=6.2.4",
             "pytest-cov>=2.12.0",
             "pytest-mock",
             "pre-commit>=2.13.0",
```

### Comparing `substrafl-0.36.0rc2/substrafl/__init__.py` & `substrafl-0.37.0rc1/substrafl/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import logging
 
 from substrafl.__version__ import __version__  # noqa
+from substrafl.compute_plan_builder import ComputePlanBuilder
 from substrafl.evaluation_strategy import EvaluationStrategy
 from substrafl.experiment import execute_experiment
 from substrafl.index_generator.np_index_generator import NpIndexGenerator
 from substrafl.logger import set_logging_level
-from substrafl.model_loading import download_algo_files
-from substrafl.model_loading import load_algo
-from substrafl.schemas import StrategyName
 
 set_logging_level(loglevel=logging.INFO)
 
 __all__ = [
     "execute_experiment",
     "set_logging_level",
     "NpIndexGenerator",
     "EvaluationStrategy",
-    "StrategyName",
-    "load_algo",
-    "download_algo_files",
+    "ComputePlanBuilder",
 ]
```

### Comparing `substrafl-0.36.0rc2/substrafl/algorithms/algo.py` & `substrafl-0.37.0rc1/substrafl/algorithms/algo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+from __future__ import annotations
+
 import abc
 from pathlib import Path
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import List
 
 from substrafl.remote.decorators import remote
-from substrafl.schemas import StrategyName
+
+if TYPE_CHECKING:
+    from substrafl.strategies.schemas import StrategyName
 
 
 class Algo(abc.ABC):
     """The base class to be inherited for substrafl algorithms."""
 
     def __init__(self, *args, **kwargs):
         self.args = args
@@ -41,15 +46,16 @@
     @abc.abstractmethod
     def train(self, datasamples, shared_state: Any) -> Any:
         """Is executed for each TrainDataOrganizations.
         This functions takes the output of the ``get_data`` method from the opener, plus the shared state from the
         aggregator if there is one, and returns a shared state (state to send to the aggregator). Any variable that
         needs to be saved and updated from one round to another should be an attribute of ``self``
         (e.g. ``self._my_local_state_variable``), and be saved and loaded in the
-        :py:func:`~substrafl.algorithms.algo.Algo.save` and :py:func:`~substrafl.algorithms.algo.Algo.load` functions.
+        :py:func:`~substrafl.algorithms.algo.Algo.save_local_state` and
+        :py:func:`~substrafl.algorithms.algo.Algo.load_local_state` functions.
 
         Args:
             datasamples (typing.Any): The output of the ``get_data`` method of the opener.
             shared_state (typing.Any): None for the first round of the computation graph
                 then the returned object from the previous organization of the computation graph.
 
         Raises:
@@ -77,15 +83,15 @@
 
         Raises:
             NotImplementedError
         """
         raise NotImplementedError
 
     @abc.abstractmethod
-    def load(self, path: Path) -> Any:
+    def load_local_state(self, path: Path) -> Any:
         """Executed at the beginning of each step of the computation graph so for each organization, at each step of
         the computation graph the previous local state can be retrieved.
 
         Args:
             path (pathlib.Path): The path where the previous local state has been saved.
 
         Raises:
@@ -94,23 +100,26 @@
         Returns:
             typing.Any: The loaded element.
         """
 
         raise NotImplementedError
 
     @abc.abstractmethod
-    def save(self, path: Path):
+    def save_local_state(self, path: Path) -> None:
         """Executed at the end of each step of the computation graph so for each organization,
         the local state can be saved.
 
         Args:
             path (pathlib.Path): The path where the previous local state has been saved.
 
         Raises:
             NotImplementedError
+
+        Returns:
+            None
         """
 
         raise NotImplementedError
 
     @remote
     def initialize(self, shared_states):
         """Empty function, useful to load the algo in the different organizations
```

### Comparing `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/__init__.py` & `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_base_algo.py` & `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_base_algo.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
         if self._device == torch.device("cpu"):
             torch.set_rng_state(checkpoint.pop("rng_state").to(self._device))
         else:
             torch.cuda.set_rng_state(checkpoint.pop("rng_state").to("cpu"))
 
         return checkpoint
 
-    def load(self, path: Path) -> "TorchAlgo":
+    def load_local_state(self, path: Path) -> "TorchAlgo":
         """Load the stateful arguments of this class.
         Child classes do not need to override that function.
 
         Args:
             path (pathlib.Path): The path where the class has been saved.
 
         Returns:
@@ -352,20 +352,23 @@
                 "The __init__() function of the torch Dataset must contain datasamples as parameter."
             )
         elif "is_inference" not in init_parameters:
             raise DatasetSignatureError(
                 "The __init__() function of the torch Dataset must contain is_inference as parameter."
             )
 
-    def save(self, path: Path):
+    def save_local_state(self, path: Path) -> None:
         """Saves all the stateful elements of the class to the specified path.
         Child classes do not need to override that function.
 
         Args:
             path (pathlib.Path): A path where to save the class.
+
+        Returns:
+            None
         """
         torch.save(
             self._get_state_to_save(),
             path,
         )
         assert path.is_file(), f'Did not save the model properly {list(path.parent.glob("*"))}'
```

### Comparing `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_fed_avg_algo.py` & `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 import torch
 
 from substrafl.algorithms.pytorch import weight_manager
 from substrafl.algorithms.pytorch.torch_base_algo import TorchAlgo
 from substrafl.index_generator import BaseIndexGenerator
 from substrafl.remote import remote_data
-from substrafl.schemas import FedAvgAveragedState
-from substrafl.schemas import FedAvgSharedState
-from substrafl.schemas import StrategyName
+from substrafl.strategies.schemas import FedAvgAveragedState
+from substrafl.strategies.schemas import FedAvgSharedState
+from substrafl.strategies.schemas import StrategyName
 
 logger = logging.getLogger(__name__)
 
 
 class TorchFedAvgAlgo(TorchAlgo):
     """To be inherited. Wraps the necessary operation so a torch model can be trained in the Federated Averaging
     strategy.
```

### Comparing `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_fed_pca_algo.py` & `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 import torch
 
 from substrafl.algorithms.pytorch import weight_manager
 from substrafl.algorithms.pytorch.torch_base_algo import TorchAlgo
 from substrafl.index_generator import NpIndexGenerator
 from substrafl.remote import remote_data
-from substrafl.schemas import FedPCAAveragedState
-from substrafl.schemas import FedPCASharedState
-from substrafl.schemas import StrategyName
+from substrafl.strategies.schemas import FedPCAAveragedState
+from substrafl.strategies.schemas import FedPCASharedState
+from substrafl.strategies.schemas import StrategyName
 
 
 class TorchLinearModel(torch.nn.Module):
     """Define linear model to encapsulate eigenvectors.
 
     Args:
         in_features (int): dimension of input vectors
```

### Comparing `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py` & `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 from substrafl.algorithms.pytorch import weight_manager
 from substrafl.algorithms.pytorch.torch_base_algo import TorchAlgo
 from substrafl.exceptions import CriterionReductionError
 from substrafl.exceptions import NegativeHessianMatrixError
 from substrafl.index_generator import NpIndexGenerator
 from substrafl.remote import remote_data
-from substrafl.schemas import NewtonRaphsonAveragedStates
-from substrafl.schemas import NewtonRaphsonSharedState
-from substrafl.schemas import StrategyName
+from substrafl.strategies.schemas import NewtonRaphsonAveragedStates
+from substrafl.strategies.schemas import NewtonRaphsonSharedState
+from substrafl.strategies.schemas import StrategyName
 
 
 class TorchNewtonRaphsonAlgo(TorchAlgo):
     """To be inherited. Wraps the necessary operation so a torch model can be trained in the Newton-Raphson strategy.
 
     The ``train`` method:
 
@@ -51,18 +51,18 @@
         use_gpu: bool = True,
         *args,
         **kwargs,
     ):
         """The ``__init__`` function is called at each call of the ``train`` or ``predict`` function.
 
         For ``round>=2``, some attributes will then be overwritten by their previous states in the
-        :py:func:`~substrafl.algorithms.pytorch.torch_base_algo.TorchAlgo.load` function, before the
+        :py:func:`~substrafl.algorithms.pytorch.torch_base_algo.TorchAlgo.load_local_state` function, before the
         ``train`` or ``predict`` function is ran.
 
-        ``TorchNewtonRaphsonAlgo`` computes its :py:class:`~substrafl.schemas.NewtonRaphsonSharedState`
+        ``TorchNewtonRaphsonAlgo`` computes its :py:class:`~substrafl.strategies.schemas.NewtonRaphsonSharedState`
         (gradients and Hessian matrix) on all the samples of the dataset. Data might be split into mini-batches to
         prevent loading too much data at once.
 
         Args:
             model (torch.nn.modules.module.Module): A torch model.
             criterion (torch.nn.modules.loss._Loss): A torch criterion (loss).
             batch_size (int): The size of the batch. If set to None it will be set to the number of samples in the
```

### Comparing `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_scaffold_algo.py` & `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from substrafl.algorithms.pytorch import weight_manager
 from substrafl.algorithms.pytorch.torch_base_algo import TorchAlgo
 from substrafl.exceptions import NumUpdatesValueError
 from substrafl.exceptions import ScaffoldLearningRateError
 from substrafl.exceptions import TorchScaffoldAlgoParametersUpdateError
 from substrafl.index_generator import BaseIndexGenerator
 from substrafl.remote import remote_data
-from substrafl.schemas import ScaffoldAveragedStates
-from substrafl.schemas import ScaffoldSharedState
-from substrafl.schemas import StrategyName
+from substrafl.strategies.schemas import ScaffoldAveragedStates
+from substrafl.strategies.schemas import ScaffoldSharedState
+from substrafl.strategies.schemas import StrategyName
 
 logger = logging.getLogger(__name__)
 
 
 class CUpdateRule(IntEnum):
     """The rule used to update the client control variate
```

### Comparing `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/torch_single_organization_algo.py` & `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 import torch
 
 from substrafl.algorithms.pytorch.torch_base_algo import TorchAlgo
 from substrafl.index_generator import BaseIndexGenerator
 from substrafl.remote import remote_data
-from substrafl.schemas import StrategyName
+from substrafl.strategies.schemas import StrategyName
 
 logger = logging.getLogger(__name__)
 
 
 class TorchSingleOrganizationAlgo(TorchAlgo):
     """To be inherited. Wraps the necessary operation so a torch model can be trained in the Single organization
     strategy.
```

### Comparing `substrafl-0.36.0rc2/substrafl/algorithms/pytorch/weight_manager.py` & `substrafl-0.37.0rc1/substrafl/algorithms/pytorch/weight_manager.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/substrafl/evaluation_strategy.py` & `substrafl-0.37.0rc1/substrafl/evaluation_strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/substrafl/exceptions.py` & `substrafl-0.37.0rc1/substrafl/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,31 @@
+class ArgumentConflictError(ValueError):
+    """Incompatible value in the given arguments."""
+
+
 class BatchSizeNotFoundError(Exception):
     """No batch size found."""
 
 
 class SubstraToolsDeprecationWarning(DeprecationWarning):
     """The substratools version used is deprecated."""
 
 
+class UnsupportedPythonVersionError(Exception):
+    """The Python version used is not supported by Substra."""
+
+
+class InvalidUserModuleError(Exception):
+    """The local folder passed by the user as a dependency is not a valid Python module."""
+
+
+class InvalidDependenciesError(Exception):
+    """The set of constraints given on dependencies cannot be solved or is otherwise invalid (wrong package name)."""
+
+
 class CriterionReductionError(Exception):
     """The criterion reduction must be set to 'mean' to use the Newton-Raphson strategy."""
 
 
 class DampingFactorValueError(Exception):
     """The damping factor must be greater than 0 and less than or equal to 1"""
 
@@ -85,46 +101,42 @@
     """When using  :class:`~substrafl.algorithms.pytorch.torch_scaffold_algo.TorchScaffoldAlgo`,
     :func:`~substrafl.algorithms.pytorch.torch_scaffold_algo.TorchScaffoldAlgo._scaffold_parameters_update` method
     must be called once for each update within the
     :func:`~substrafl.algorithms.pytorch.torch_scaffold_algo.TorchScaffoldAlgo._local_train` method.
     """
 
 
-class TrainTaskNotFoundError(Exception):
-    """When using the :func:`~substrafl.model_loading.download_algo_files` function. The provided compute plan must
-    contain a task:
+class TaskNotFoundError(Exception):
+    """The provided compute plan must contain a task:
 
-        - hosted by the worker associated to the given client
-        - tagged with the given round_idx
+    - hosted by the worker associated to the given client
+    - tagged with the given round_idx or rank_idx
     """
 
 
-class MultipleTrainTaskError(Exception):
-    """When using the :func:`~substrafl.model_loading.download_algo_files` function in remote mode. The experiment to
-    get the algo files from can't have multiple TrainDataNodes hosted on the same organization."""
+class MultipleTaskError(Exception):
+    """The experiment from which to get the algo files can't have multiple task tagged with the given round_idx or
+    rank_idx hosted on the same organization."""
 
 
-class UnfinishedTrainTaskError(Exception):
-    """When using the :func:`~substrafl.model_loading.download_algo_files` function. The task to get the algo files
-    from shall be in status ``STATUS_DONE``."""
+class UnfinishedTaskError(Exception):
+    """The task from which to get the algo files shall be in status ``STATUS_DONE``."""
 
 
-class LoadAlgoMetadataError(Exception):
-    """When using the :func:`~substrafl.model_loading.load_algo`, the metadata.json file within the folder given as
-    input must contain a ``local_state_file``"""
+class LoadMetadataError(Exception):
+    """The metadata.json file within the folder given as input must contain a ``model_file``"""
 
 
-class LoadAlgoFileNotFoundError(Exception):
-    """When using the :func:`~substrafl.model_loading.load_algo`, the given folder must contains the following files:
-    function.tar.gz, metadata.json, the file entered in the ``local_state_file`` key of the dictionary."""
+class LoadFileNotFoundError(Exception):
+    """The given folder must contains the following files: function.tar.gz, metadata.json, the file entered in the
+    ``model_file`` key of the dictionary."""
 
 
-class LoadAlgoLocalDependencyError(Exception):
-    """When using the :func:`~substrafl.model_loading.load_algo`, all dependencies from the local input folder should be
-    install by the user."""
+class LoadLocalDependencyError(Exception):
+    """All dependencies from the local input folder should be install by the user."""
 
 
 class UnsupportedPytorchVersionError(Exception):
     """Unsupported Pytorch version"""
 
 
 class MetricFunctionSignatureError(Exception):
```

### Comparing `substrafl-0.36.0rc2/substrafl/experiment.py` & `substrafl-0.37.0rc1/substrafl/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 from typing import Tuple
 from typing import Union
 
 import substra
 import substratools
 
 import substrafl
+from substrafl.compute_plan_builder import ComputePlanBuilder
 from substrafl.dependency import Dependency
 from substrafl.evaluation_strategy import EvaluationStrategy
 from substrafl.exceptions import KeyMetadataError
 from substrafl.exceptions import LenMetadataError
 from substrafl.nodes.aggregation_node import AggregationNode
 from substrafl.nodes.node import OperationKey
 from substrafl.nodes.train_data_node import TrainDataNode
 from substrafl.remote.remote_struct import RemoteStruct
-from substrafl.strategies.strategy import Strategy
 
 logger = logging.getLogger(__name__)
 
 
 def _register_operations(
     client: substra.Client,
     train_data_nodes: List[TrainDataNode],
@@ -111,15 +111,15 @@
 
     return tasks, operation_cache
 
 
 def _save_experiment_summary(
     experiment_folder: Path,
     compute_plan_key: str,
-    strategy: Strategy,
+    strategy: ComputePlanBuilder,
     num_rounds: int,
     operation_cache: Dict[RemoteStruct, OperationKey],
     train_data_nodes: TrainDataNode,
     aggregation_node: Optional[AggregationNode],
     evaluation_strategy: EvaluationStrategy,
     timestamp: str,
     additional_metadata: Optional[Dict],
@@ -142,15 +142,16 @@
     experiment_folder = Path(experiment_folder)
     experiment_folder.mkdir(exist_ok=True)
     experiment_summary = dict()
 
     # add attributes of interest and summaries of the classes to the experiment summary
     experiment_summary["compute_plan_key"] = compute_plan_key
     experiment_summary["strategy"] = type(strategy).__name__
-    experiment_summary["num_rounds"] = num_rounds
+    if num_rounds is not None:
+        experiment_summary["num_rounds"] = num_rounds
     experiment_summary["function_keys"] = {
         operation_cache[remote_struct]: remote_struct.summary() for remote_struct in operation_cache
     }
     experiment_summary["train_data_nodes"] = [train_data_node.summary() for train_data_node in train_data_nodes]
     experiment_summary["test_data_nodes"] = []
     if evaluation_strategy is not None:
         experiment_summary["test_data_nodes"] = [
@@ -177,17 +178,15 @@
         raise ValueError(
             "num_rounds set in evaluation_strategy does not match num_rounds set in the experiment: "
             f"{evaluation_strategy.num_rounds} is not {num_rounds}"
         )
 
 
 def _check_additional_metadata(additional_metadata: Dict):
-    unauthorized_keys = set(
-        ("substrafl_version", "substra_version", "substratools_version", "python_version", "num_rounds")
-    )
+    unauthorized_keys = {"substrafl_version", "substra_version", "substratools_version", "python_version"}
     invalid_keys = set(additional_metadata.keys()).intersection(unauthorized_keys)
 
     if len(invalid_keys) > 0:
         raise KeyMetadataError(
             f"None of: `{'`, `'.join(unauthorized_keys)}` can be used as"
             f" metadata key but `{' '.join(invalid_keys)}` were/was found"
         )
@@ -213,18 +212,18 @@
         "python_version": python_version(),
     }
 
 
 def execute_experiment(
     *,
     client: substra.Client,
-    strategy: Strategy,
+    strategy: ComputePlanBuilder,
     train_data_nodes: List[TrainDataNode],
-    num_rounds: int,
     experiment_folder: Union[str, Path],
+    num_rounds: Optional[int] = None,
     aggregation_node: Optional[AggregationNode] = None,
     evaluation_strategy: Optional[EvaluationStrategy] = None,
     dependencies: Optional[Dependency] = None,
     clean_models: bool = True,
     name: Optional[str] = None,
     additional_metadata: Optional[Dict] = None,
     task_submission_batch_size: int = 500,
@@ -253,14 +252,15 @@
         client (substra.Client): A substra client to interact with the Substra platform
         strategy (Strategy): The strategy that will be executed
         train_data_nodes (typing.List[TrainDataNode]): List of the nodes where training on data
             occurs evaluation_strategy (EvaluationStrategy, Optional): If None performance will not be measured at all.
             Otherwise measuring of performance will follow the EvaluationStrategy. Defaults to None.
         aggregation_node (typing.Optional[AggregationNode]): For centralized strategy, the aggregation
             node, where all the shared tasks occurs else None.
+        evaluation_strategy: Optional[EvaluationStrategy]
         num_rounds (int): The number of time your strategy will be executed
         dependencies (Dependency, Optional): Dependencies of the experiment. It must be defined from
             the SubstraFL Dependency class. Defaults None.
         experiment_folder (typing.Union[str, pathlib.Path]): path to the folder where the experiment summary is saved.
         clean_models (bool): Clean the intermediary models on the Substra platform. Set it to False
             if you want to download or re-use intermediary models. This causes the disk space to fill
             quickly so should be set to True unless needed. Defaults to True.
@@ -296,20 +296,17 @@
     if additional_metadata is not None:
         _check_additional_metadata(additional_metadata)
         cp_metadata.update(additional_metadata)
 
     # Adding substrafl, substratools and substra versions to the cp metadata
     cp_metadata.update(_get_packages_versions())
 
-    # Adding rounds metadata to cp_meta_data
-    cp_metadata["num_rounds"] = num_rounds
-
     logger.info("Building the compute plan.")
 
-    strategy.build_graph(
+    strategy.build_compute_plan(
         train_data_nodes=train_data_nodes,
         aggregation_node=aggregation_node,
         evaluation_strategy=evaluation_strategy,
         num_rounds=num_rounds,
         clean_models=clean_models,
     )
```

### Comparing `substrafl-0.36.0rc2/substrafl/index_generator/base.py` & `substrafl-0.37.0rc1/substrafl/index_generator/base.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/substrafl/index_generator/np_index_generator.py` & `substrafl-0.37.0rc1/substrafl/index_generator/np_index_generator.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/substrafl/logger.py` & `substrafl-0.37.0rc1/substrafl/logger.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/substrafl/nodes/__init__.py` & `substrafl-0.37.0rc1/substrafl/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/substrafl/nodes/aggregation_node.py` & `substrafl-0.37.0rc1/substrafl/nodes/aggregation_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 import uuid
 from typing import Dict
+from typing import Optional
 from typing import Set
 from typing import TypeVar
 
 import substra
 
 from substrafl.dependency import Dependency
 from substrafl.nodes.node import InputIdentifiers
 from substrafl.nodes.node import Node
 from substrafl.nodes.node import OperationKey
 from substrafl.nodes.node import OutputIdentifiers
 from substrafl.nodes.references.shared_state import SharedStateRef
 from substrafl.remote.operations import RemoteOperation
 from substrafl.remote.register import register_function
 from substrafl.remote.remote_struct import RemoteStruct
+from substrafl.schemas import TaskType
 
 SharedState = TypeVar("SharedState")
 
 
 class AggregationNode(Node):
     """The node which applies operations to the shared states which are received from ``TrainDataNode``
     data operations.
     The result is sent to the ``TrainDataNode`` and/or ``TestDataNode`` data operations.
     """
 
     def update_states(
         self,
         operation: RemoteOperation,
         *,
-        round_idx: int,
         authorized_ids: Set[str],
+        round_idx: Optional[int] = None,
         clean_models: bool = False,
     ) -> SharedStateRef:
         """Adding an aggregated task to the list of operations to be executed by the node during the compute plan.
         This is done in a static way, nothing is submitted to substra.
         This is why the function key is a RemoteStruct (substrafl local reference of the algorithm)
         and not a substra function_key as nothing has been submitted yet.
 
         Args:
             operation (RemoteOperation): Automatically generated structure returned by
                 the :py:func:`~substrafl.remote.decorators.remote` decorator. This allows to register an
                 operation and execute it later on.
-            round_idx (int): Round number, it starts at 1.
+            round_idx (int): Used in case of learning compute plans. Round number, it starts at 1. Default to None.
             authorized_ids (Set[str]): Authorized org to access the output model.
             clean_models (bool): Whether outputs of this operation are transient (deleted when they are not used
                 anymore) or not. Defaults to False.
 
         Raises:
             TypeError: operation must be an RemoteOperation, make sure to decorate your (user defined) aggregate
                 function of the strategy with @remote.
@@ -71,28 +73,27 @@
                 )
                 for ref in operation.shared_states
             ]
             if operation.shared_states is not None
             else None
         )
 
+        task_metadata = {"round_idx": round_idx} if round_idx is not None else {}
         aggregate_task = substra.schemas.ComputePlanTaskSpec(
             function_key=str(uuid.uuid4()),  # bogus function key
             task_id=op_id,
             inputs=inputs,
             outputs={
                 OutputIdentifiers.model: substra.schemas.ComputeTaskOutputSpec(
                     permissions=substra.schemas.Permissions(public=False, authorized_ids=list(authorized_ids)),
                     transient=clean_models,
                 )
             },
-            metadata={
-                "round_idx": round_idx,
-            },
-            tag="aggregate",
+            metadata=task_metadata,
+            tag=TaskType.AGGREGATE,
             worker=self.organization_id,
         ).dict()
 
         aggregate_task.pop("function_key")
         aggregate_task["remote_operation"] = operation.remote_struct
 
         self.tasks.append(aggregate_task)
```

### Comparing `substrafl-0.36.0rc2/substrafl/nodes/node.py` & `substrafl-0.37.0rc1/substrafl/nodes/node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/substrafl/nodes/test_data_node.py` & `substrafl-0.37.0rc1/substrafl/nodes/test_data_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import inspect
 import uuid
 from collections.abc import Iterable
+from string import printable
 from typing import Callable
 from typing import Dict
 from typing import List
+from typing import Optional
 from typing import Union
 
 import substra
 
 from substrafl import exceptions
 from substrafl.dependency import Dependency
 from substrafl.nodes.node import InputIdentifiers
@@ -72,24 +74,24 @@
 
         super().__init__(organization_id)
 
     def update_states(
         self,
         traintask_id: str,
         operation: RemoteDataOperation,
-        round_idx: int,
+        round_idx: Optional[int] = None,
     ):
         """Creating a test task based on the node characteristic.
 
         Args:
             traintask_id (str): The substra parent id
             operation (RemoteDataOperation): Automatically generated structure returned by
                 the :py:func:`~substrafl.remote.decorators.remote_data` decorator. This allows to register an
                 operation and execute it later on.
-            round_idx: (int): Round number of the strategy starting at 1.
+            round_idx (int): Used in case of learning compute plans. Round number, it starts at 1. Default to None.
 
         """
 
         predicttask_id = str(uuid.uuid4())
 
         data_inputs = [
             substra.schemas.InputRef(identifier=InputIdentifiers.opener, asset_key=self.data_manager_key)
@@ -108,28 +110,27 @@
         test_input = [
             substra.schemas.InputRef(
                 identifier=InputIdentifiers.predictions,
                 parent_task_key=predicttask_id,
                 parent_task_output_identifier=OutputIdentifiers.predictions,
             )
         ]
+        task_metadata = {"round_idx": round_idx} if round_idx is not None else {}
 
         predicttask = substra.schemas.ComputePlanTaskSpec(
             function_key=str(uuid.uuid4()),  # bogus function key
             task_id=predicttask_id,
             inputs=data_inputs + predict_input,
             outputs={
                 OutputIdentifiers.predictions: substra.schemas.ComputeTaskOutputSpec(
                     permissions=substra.schemas.Permissions(public=False, authorized_ids=[self.organization_id]),
                     transient=True,
                 )
             },
-            metadata={
-                "round_idx": round_idx,
-            },
+            metadata=task_metadata,
             worker=self.organization_id,
         ).dict()
 
         predicttask.pop("function_key")
         predicttask["remote_operation"] = operation.remote_struct
         self.predicttasks.append(predicttask)
 
@@ -140,17 +141,15 @@
             outputs={
                 metric_function_id: substra.schemas.ComputeTaskOutputSpec(
                     permissions=substra.schemas.Permissions(public=True, authorized_ids=[]),
                     transient=False,
                 )
                 for metric_function_id in self.metric_functions
             },
-            metadata={
-                "round_idx": round_idx,
-            },
+            metadata=task_metadata,
             worker=self.organization_id,
         ).dict()
         testtask.pop("function_key")
         testtask["remote_operation"] = operation.remote_struct
         self.testtasks.append(testtask)
 
     def register_test_operations(
@@ -309,12 +308,26 @@
     Args:
         identifier (str): identifier used for the registration of the metric function given by the user.
 
     Raises:
         exceptions.InvalidMetricIdentifierError: the identifier must not be in the OutputIdentifiers list used
         internally by SubstraFL.
     """
+
     if identifier in list(OutputIdentifiers):
         raise exceptions.InvalidMetricIdentifierError(
-            f" A metric name or identifier cannot be in {[id.value for id in list(OutputIdentifiers)]}. \
+            f"A metric name or identifier cannot be in {[id.value for id in list(OutputIdentifiers)]}. \
             These values are used internally by SusbtraFL."
         )
+
+    unauthorized_characters = set(identifier).difference(
+        set(printable) - {"|"}
+    )  # | is used in the backend as a separator for identifiers.
+    if unauthorized_characters:
+        raise exceptions.InvalidMetricIdentifierError(
+            f"{unauthorized_characters} cannot be used to define a metric name."
+        )
+
+    if identifier == "":
+        raise exceptions.InvalidMetricIdentifierError("A metric name cannot be an empty string.")
+    elif len(identifier) > 36:  # Max length is the uuid4 length.
+        raise exceptions.InvalidMetricIdentifierError("A metric name must be of length inferior to 36.")
```

### Comparing `substrafl-0.36.0rc2/substrafl/nodes/train_data_node.py` & `substrafl-0.37.0rc1/substrafl/nodes/train_data_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from substrafl.nodes.node import OutputIdentifiers
 from substrafl.nodes.references.local_state import LocalStateRef
 from substrafl.nodes.references.shared_state import SharedStateRef
 from substrafl.remote.operations import RemoteDataOperation
 from substrafl.remote.operations import RemoteOperation
 from substrafl.remote.register import register_function
 from substrafl.remote.remote_struct import RemoteStruct
+from substrafl.schemas import TaskType
 
 
 class TrainDataNode(Node):
     """
     A predefined structure that allows you to register operations
     on your train node in a static way before submitting them to substra.
 
@@ -63,48 +64,48 @@
                     permissions=substra.schemas.Permissions(public=False, authorized_ids=list(authorized_ids)),
                     transient=clean_models,
                 ),
             },
             metadata={
                 "round_idx": round_idx,
             },
-            tag="init",
+            tag=TaskType.INITIALIZATION,
             worker=self.organization_id,
         ).dict()
 
         init_task.pop("function_key")
         init_task["remote_operation"] = operation.remote_struct
 
         self.init_task = init_task
 
         return LocalStateRef(key=op_id, init=True)
 
     def update_states(
         self,
         operation: RemoteDataOperation,
         *,
-        round_idx: int,
         authorized_ids: Set[str],
+        round_idx: Optional[int] = None,
         aggregation_id: Optional[str] = None,
         clean_models: bool = False,
         local_state: Optional[LocalStateRef] = None,
     ) -> Tuple[LocalStateRef, SharedStateRef]:
         """Adding a train task to the list of operations to
         be executed by the node during the compute plan. This is done in a static
         way, nothing is submitted to substra.
         This is why the function key is a RemoteStruct (substrafl local reference of the algorithm)
         and not a substra function_key as nothing has been submitted yet.
 
         Args:
             operation (RemoteDataOperation): Automatically generated structure returned by
                 the :py:func:`~substrafl.remote.decorators.remote_data` decorator. This allows to register an
                 operation and execute it later on.
-            round_idx (int): Round number, it starts at 1. In case of a centralized strategy,
-                it is preceded by an initialization round tagged: 0.
             authorized_ids (typing.Set[str]): Authorized org to access the output model.
+            round_idx (int): Used in case of learning compute plans. Round number, it starts at 1.
+                In case of a centralized strategy, it is preceded by an initialization round tagged: 0. Default to None
             aggregation_id (str): Aggregation node id to authorize access to the shared model. Defaults to None.
             clean_models (bool): Whether outputs of this operation are transient (deleted when they are not used
                 anymore) or not. Defaults to False.
             local_state (typing.Optional[LocalStateRef]): The parent task LocalStateRef. Defaults to None.
 
         Raises:
             TypeError: operation must be a RemoteDataOperation, make sure to decorate the train and predict methods of
@@ -155,14 +156,15 @@
                     parent_task_output_identifier=OutputIdentifiers.shared,
                 )
             ]
 
         else:
             shared_inputs = []
 
+        task_metadata = {"round_idx": round_idx} if round_idx is not None else {}
         train_task = substra.schemas.ComputePlanTaskSpec(
             function_key=str(uuid.uuid4()),  # bogus function key
             task_id=op_id,
             inputs=data_inputs + local_inputs + shared_inputs,
             outputs={
                 OutputIdentifiers.shared: substra.schemas.ComputeTaskOutputSpec(
                     permissions=substra.schemas.Permissions(
@@ -172,18 +174,16 @@
                     transient=clean_models,
                 ),
                 OutputIdentifiers.local: substra.schemas.ComputeTaskOutputSpec(
                     permissions=substra.schemas.Permissions(public=False, authorized_ids=list(authorized_ids)),
                     transient=clean_models,
                 ),
             },
-            metadata={
-                "round_idx": round_idx,
-            },
-            tag="train",
+            metadata=task_metadata,
+            tag=TaskType.TRAIN,
             worker=self.organization_id,
         ).dict()
 
         train_task.pop("function_key")
         train_task["remote_operation"] = operation.remote_struct
 
         self.tasks.append(train_task)
```

### Comparing `substrafl-0.36.0rc2/substrafl/remote/decorators.py` & `substrafl-0.37.0rc1/substrafl/remote/decorators.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/substrafl/remote/operations.py` & `substrafl-0.37.0rc1/substrafl/remote/operations.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/substrafl/remote/register/register.py` & `substrafl-0.37.0rc1/substrafl/remote/register/register.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,76 @@
 """
 Create the Substra function assets and register them to the platform.
 """
+
 import logging
 import os
-import shutil
 import tarfile
 import tempfile
 import typing
 import warnings
 from distutils import util
 from pathlib import Path
+from pathlib import PurePosixPath
 from platform import python_version
 
 import substra
 import substratools
 from packaging import version
 
 import substrafl
 from substrafl import exceptions
+from substrafl.constants import TMP_SUBSTRAFL_PREFIX
 from substrafl.dependency import Dependency
+from substrafl.exceptions import UnsupportedPythonVersionError
 from substrafl.nodes.node import InputIdentifiers
-from substrafl.remote.register.generate_wheel import local_lib_wheels
-from substrafl.remote.register.generate_wheel import pypi_lib_wheels
+from substrafl.remote.register.manage_dependencies import compile_requirements
+from substrafl.remote.register.manage_dependencies import copy_local_wheels
+from substrafl.remote.register.manage_dependencies import get_pypi_dependencies_versions
+from substrafl.remote.register.manage_dependencies import local_lib_wheels
 from substrafl.remote.remote_struct import RemoteStruct
 from substrafl.remote.substratools_methods import RemoteMethod
 
 logger = logging.getLogger(__name__)
 
 # Substra tools version for which the image naming scheme changed
 MINIMAL_DOCKER_SUBSTRATOOLS_VERSION = "0.16.0"
 
-TMP_SUBSTRAFL_PREFIX = "tmp_substrafl"
+# minimal and maximal values of Python 3 minor versions supported
+# we need to store this as integer, else "3.10" < "3.9" (string comparison)
+MINIMAL_PYTHON_VERSION = 8  # 3.8
+MAXIMAL_PYTHON_VERSION = 10  # 3.10
 
 _DEFAULT_SUBSTRATOOLS_IMAGE = "ghcr.io/substra/substra-tools:\
 {substratools_version}-nvidiacuda11.8.0-base-ubuntu22.04-python{python_version}"
 
 SUBSTRAFL_FOLDER = "substrafl_internal"
 
 DOCKERFILE_TEMPLATE = """
 FROM {docker_image}
 
 # install dependencies
 RUN python{python_version} -m pip install -U pip
 
-# Install substrafl, substra (and substratools if editable mode)
-{cl_deps}
-
-# PyPi dependencies
-{pypi_dependencies}
+# Copy local wheels
+{copy_wheels}
 
-# Install local dependencies
-{local_dependencies}
+# Copy requirements.txt
+COPY {internal_dir}/requirements.txt requirements.txt
 
-ENTRYPOINT ["python{python_version}", "function.py", "--function-name", "{method_name}"]
+# Install requirements
+RUN python{python_version} -m pip install --no-cache-dir -r requirements.txt
 
-COPY . .
+# Copy all other files
+COPY function.py .
+COPY {internal_dir}/cls_cloudpickle {internal_dir}/
+COPY {internal_dir}/description.md {internal_dir}/
+{copy_local_code}
 
+ENTRYPOINT ["python{python_version}", "function.py", "--function-name", "{method_name}"]
 """
 
 FUNCTION = """
 import json
 import cloudpickle
 
 import substratools as tools
@@ -79,90 +90,136 @@
     remote_instance.register_substratools_function()
 
     # Execute the function using substra-tools
     tools.execute()
 """
 
 
-def _copy_local_packages(
-    path: Path, local_dependencies: typing.List[Path], python_major_minor: str, operation_dir: Path
-):
-    """Copy the local libraries given by the user and generate the installation command."""
-    dependencies_buffer = []
-    path.mkdir(exist_ok=True)
-    for dependency_path in local_dependencies:
-        dest_path = path / dependency_path.name
-        if dependency_path.is_dir():
-            shutil.copytree(
-                dependency_path,
-                dest_path,
-                ignore=shutil.ignore_patterns(
-                    "local-worker",
-                    TMP_SUBSTRAFL_PREFIX + "*",
-                ),
-            )
-        elif dependency_path.is_file():
-            shutil.copy(dependency_path, dest_path)
-        else:
-            raise ValueError(f"Does not exist {dependency_path}")
-
-        dependencies_buffer.append(f"{dest_path.relative_to(operation_dir)}")
-
-    local_dependencies_cmd = "\n".join(
-        [
-            f"COPY {dependency}  {dependency} \n"
-            + f"RUN python{python_major_minor} -m pip install --no-cache-dir {dependency} \n"
-            for dependency in dependencies_buffer
-        ]
-    )
-
-    return local_dependencies_cmd
-
-
-def _copy_local_code(path: Path, operation_dir: Path):
-    """Copy the local code given by the user to the operation directory."""
-    if path.is_dir():
-        shutil.copytree(path, operation_dir / path.name)
-    elif path.is_file():
-        shutil.copy(path, operation_dir / path.name)
-    else:
-        raise ValueError(f"Does not exist {path}")
-
-
 def _create_archive(archive_path: Path, src_path: Path):
     """Create a tar archive from a folder"""
     with tarfile.open(archive_path, "w:gz") as tar:
         for filepath in src_path.glob("*"):
             if not filepath.name.endswith(".tar.gz"):
                 tar.add(filepath, arcname=filepath.name, recursive=True)
 
 
-def _get_base_docker_image(python_major_minor: str, editable_mode: bool):
+def _check_python_version(python_major_minor: str) -> None:
+    """Raise UnsupportedPythonVersionError exception if the Python version is not supported"""
+    major, minor = python_major_minor.split(".")
+    if major != "3":
+        raise UnsupportedPythonVersionError("Only Python 3 is supported")
+    if int(minor) < MINIMAL_PYTHON_VERSION or int(minor) > MAXIMAL_PYTHON_VERSION:
+        raise UnsupportedPythonVersionError(
+            f"The current Python version is {python_major_minor}, which is unsupported;"
+            f"supported versions are 3.{MINIMAL_PYTHON_VERSION} to 3.{MAXIMAL_PYTHON_VERSION}"
+        )
+
+
+def _get_base_docker_image(python_major_minor: str, editable_mode: bool) -> str:
     """Get the base Docker image for the Dockerfile"""
 
     substratools_image_version = substratools.__version__
     if util.strtobool(os.environ.get("USE_LATEST_SUBSTRATOOLS", "False")):
         substratools_image_version = "latest"
     elif version.parse(substratools_image_version) < version.parse(MINIMAL_DOCKER_SUBSTRATOOLS_VERSION):
         if not editable_mode:
             warnings.warn(
                 f"Your environment uses substra-tools={substratools_image_version}. Version \
                 {MINIMAL_DOCKER_SUBSTRATOOLS_VERSION} will be used on Docker.",
                 exceptions.SubstraToolsDeprecationWarning,
                 stacklevel=2,
             )
         substratools_image_version = MINIMAL_DOCKER_SUBSTRATOOLS_VERSION
+
+    _check_python_version(python_major_minor)
+
     substratools_image = _DEFAULT_SUBSTRATOOLS_IMAGE.format(
         substratools_version=substratools_image_version,
         python_version=python_major_minor,
     )
 
     return substratools_image
 
 
+def _generate_copy_local_files(local_files: typing.List[Path]) -> str:
+    # In Dockerfiles, we need to always have '/'. PurePosixPath resolves that.
+    return "\n".join([f"COPY {PurePosixPath(file)} {PurePosixPath(file)}" for file in local_files])
+
+
+def _create_dockerfile(install_libraries: bool, dependencies: Dependency, operation_dir: Path, method_name: str) -> str:
+    substrafl_internal = operation_dir / SUBSTRAFL_FOLDER
+    substrafl_internal.mkdir(exist_ok=True)
+
+    # get Python version
+    # Required to select the correct version of python inside the docker Image
+    # Cloudpickle will crash if we don't deserialize with the same major.minor
+    python_major_minor = ".".join(python_version().split(".")[:2])
+
+    # Get the base Docker image
+    substratools_image = _get_base_docker_image(
+        python_major_minor=python_major_minor, editable_mode=dependencies.editable_mode
+    )
+
+    pypi_dependencies = dependencies.pypi_dependencies
+    wheels = []
+    # Build Substrafl, Substra and Substratools, and local dependencies wheels if necessary
+    if install_libraries:
+        # Substrafl, Substra and Substratools
+        # Install either from pypi wheel or repo in editable mode
+        if dependencies.editable_mode or util.strtobool(os.environ.get("SUBSTRA_FORCE_EDITABLE_MODE", "False")):
+            substra_wheel_dir = substrafl_internal / "dist"
+            substra_wheels = local_lib_wheels(
+                lib_modules=[
+                    substrafl,
+                    substra,
+                    substratools,
+                ],  # We reinstall substratools in editable mode to overwrite the installed version
+                dest_dir=substra_wheel_dir,
+            )
+            wheels += [substra_wheel_dir.relative_to(operation_dir) / wheel_name for wheel_name in substra_wheels]
+        else:
+            pypi_dependencies += get_pypi_dependencies_versions(
+                lib_modules=[substrafl],
+            )
+
+        local_dep_dir = substrafl_internal / "local_dependencies"
+        wheels += [
+            local_dep_dir.relative_to(operation_dir) / wheel_name
+            for wheel_name in copy_local_wheels(
+                path=local_dep_dir,
+                dependencies=dependencies,
+            )
+        ]
+        # generate the copy wheel command
+        copy_wheels_cmd = _generate_copy_local_files(wheels)
+
+        # create a requirements.in with all requirements (substra libs and user-defined)
+        dependency_list = pypi_dependencies + wheels
+
+    else:
+        dependency_list = []
+        copy_wheels_cmd = ""
+
+    # user-defined local dependencies
+    local_paths = dependencies.copy_dependencies_local_code(dest_dir=operation_dir)
+    copy_local_code_cmd = _generate_copy_local_files(local_paths)
+
+    # pip-compile the requirements.in into a requirements.txt
+    compile_requirements(dependency_list, operation_dir=operation_dir, sub_dir=SUBSTRAFL_FOLDER)
+
+    return DOCKERFILE_TEMPLATE.format(
+        docker_image=substratools_image,
+        python_version=python_major_minor,
+        copy_wheels=copy_wheels_cmd,
+        copy_local_code=copy_local_code_cmd,
+        method_name=method_name,
+        internal_dir=SUBSTRAFL_FOLDER,
+    )
+
+
 def _create_substra_function_files(
     remote_struct: RemoteStruct,
     install_libraries: bool,
     dependencies: Dependency,
     operation_dir: Path,
 ) -> typing.Tuple[Path, Path]:
     """Creates the necessary files from the remote struct to register the associated function to substra, zip them into
@@ -172,109 +229,68 @@
 
             - the RemoteStruct (wrapped code) dump file
             - the wheel of the current version of Substrafl and Substra
             - the Dockerfile
             - the description.md
             - the function.py entrypoint
 
+        Target tree structure:
+            ├── Dockerfile
+            ├── function.py
+            ├── function.tar.gz
+            ├── local_code.py
+            └── substrafl_internal
+                ├── cls_cloudpickle
+                ├── description.md
+                ├── dist
+                │   ├── substra-0.44.0-py3-none-any.whl
+                │   ├── substrafl-0.36.0-py3-none-any.whl
+                │   └── substratools-0.20.0-py3-none-any.whl
+                ├── local_dependencies
+                │   └── local-module-1.6.1-py3-none-any.whl
+                ├── requirements.in
+                └── requirements.txt
+
     Args:
         remote_struct (RemoteStruct): A representation of a substra algorithm.
         install_libraries (bool): whether we need to build the wheels and copy the files to install the libraries
         dependencies (Dependency): Function dependencies.
         operation_dir (pathlib.Path): path to the operation directory
 
         Returns:
             Tuple[Path, Path]: The archive path and the description file path.
     """
     substrafl_internal = operation_dir / SUBSTRAFL_FOLDER
     substrafl_internal.mkdir()
 
     remote_struct.save(dest=substrafl_internal)
 
-    # get Python version
-    # Required to select the correct version of python inside the docker Image
-    # Cloudpickle will crash if we don't deserialize with the same major.minor
-    python_major_minor = ".".join(python_version().split(".")[:2])
-
-    # Build Substrafl, Substra and Substratools wheel if needed
-    install_cmd = ""
-
-    if install_libraries:
-        # Install either from pypi wheel or repo in editable mode
-        if dependencies.editable_mode:
-            install_cmd = local_lib_wheels(
-                lib_modules=[
-                    substrafl,
-                    substra,
-                    substratools,
-                ],  # We reinstall substratools in editable mode to overwrite the installed version
-                operation_dir=operation_dir,
-                python_major_minor=python_major_minor,
-                dest_dir=f"{SUBSTRAFL_FOLDER}/dist",
-            )
-        else:
-            install_cmd = pypi_lib_wheels(
-                lib_modules=[substrafl, substra],
-                operation_dir=operation_dir,
-                python_major_minor=python_major_minor,
-                dest_dir=f"{SUBSTRAFL_FOLDER}/dist",
-            )
-
-    # Pypi dependencies docker command if specified by the user
-    pypi_dependencies_cmd = (
-        f"RUN python{python_major_minor} -m pip install --no-cache-dir {' '.join(dependencies.pypi_dependencies)}"
-        if dependencies is not None and len(dependencies.pypi_dependencies) > 0
-        else ""
+    # Write dockerfile based on template
+    dockerfile_path = operation_dir / "Dockerfile"
+    dockerfile_path.write_text(
+        _create_dockerfile(
+            install_libraries=install_libraries,
+            dependencies=dependencies,
+            operation_dir=operation_dir,
+            method_name=remote_struct._method_name,
+        )
     )
 
-    # The files to copy to the container must be in the same folder as the Dockerfile
-    local_dependencies_cmd = ""
-    if dependencies is not None:
-        for path in dependencies.local_code:
-            _copy_local_code(path=path, operation_dir=operation_dir)
-
-        if install_libraries:
-            local_dep_dir = substrafl_internal / "local_dependencies"
-            local_dependencies_cmd = _copy_local_packages(
-                path=local_dep_dir,
-                local_dependencies=dependencies.local_dependencies,
-                python_major_minor=python_major_minor,
-                operation_dir=operation_dir,
-            )
-
     # Write template to function.py
     function_path = operation_dir / "function.py"
     function_path.write_text(
         FUNCTION.format(
             substrafl_folder=SUBSTRAFL_FOLDER,
         )
     )
 
     # Write description
     description_path = substrafl_internal / "description.md"
     description_path.write_text("# Substrafl Operation")
 
-    # Get the base Docker image
-    substratools_image = _get_base_docker_image(
-        python_major_minor=python_major_minor, editable_mode=dependencies.editable_mode
-    )
-
-    # Write dockerfile based on template
-    dockerfile_path = operation_dir / "Dockerfile"
-    dockerfile_path.write_text(
-        DOCKERFILE_TEMPLATE.format(
-            docker_image=substratools_image,
-            python_version=python_major_minor,
-            cl_deps=install_cmd,
-            pypi_dependencies=pypi_dependencies_cmd,
-            local_dependencies=local_dependencies_cmd,
-            method_name=remote_struct._method_name,
-        )
-    )
-
     # Create necessary archive to register the operation on substra
     archive_path = operation_dir / "function.tar.gz"
     _create_archive(archive_path=archive_path, src_path=operation_dir)
 
     return archive_path, description_path
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `substrafl-0.36.0rc2/substrafl/remote/remote_struct.py` & `substrafl-0.37.0rc1/substrafl/remote/remote_struct.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/substrafl/remote/serializers/pickle_serializer.py` & `substrafl-0.37.0rc1/substrafl/remote/serializers/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.36.0rc2/substrafl/remote/substratools_methods.py` & `substrafl-0.37.0rc1/substrafl/remote/substratools_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,24 +145,24 @@
 
         Args:
             path (str): path to the saved instance
 
         Returns:
             Any: loaded instance
         """
-        return self.instance.load(Path(path))
+        return self.instance.load_local_state(Path(path))
 
     def save_instance(self, path: str) -> None:
         """Save the instance
 
         Args:
             model (Any): Instance to save
             path (str): Path where to save the instance
         """
-        self.instance.save(Path(path))
+        self.instance.save_local_state(Path(path))
 
     def register_substratools_function(self):
         """Register the function that can be accessed and executed by substratools."""
 
         tools.register(
             function=self.generic_function,
             function_name=self.method_name,
```

### Comparing `substrafl-0.36.0rc2/substrafl/schemas.py` & `substrafl-0.37.0rc1/substrafl/strategies/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Schemas used in the application.
+"""Schemas used in the strategies.
 """
 from enum import Enum
 from typing import List
 
 import numpy as np
 import pydantic
```

### Comparing `substrafl-0.36.0rc2/substrafl/strategies/fed_avg.py` & `substrafl-0.37.0rc1/substrafl/strategies/fed_avg.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from substrafl.exceptions import EmptySharedStatesError
 from substrafl.nodes.aggregation_node import AggregationNode
 from substrafl.nodes.references.local_state import LocalStateRef
 from substrafl.nodes.references.shared_state import SharedStateRef
 from substrafl.nodes.test_data_node import TestDataNode
 from substrafl.nodes.train_data_node import TrainDataNode
 from substrafl.remote import remote
-from substrafl.schemas import FedAvgAveragedState
-from substrafl.schemas import FedAvgSharedState
-from substrafl.schemas import StrategyName
+from substrafl.strategies.schemas import FedAvgAveragedState
+from substrafl.strategies.schemas import FedAvgSharedState
+from substrafl.strategies.schemas import StrategyName
 from substrafl.strategies.strategy import Strategy
 
 
 class FedAvg(Strategy):
     """Federated averaging strategy.
 
     Federated averaging is the simplest federating strategy.
```

### Comparing `substrafl-0.36.0rc2/substrafl/strategies/fed_pca.py` & `substrafl-0.37.0rc1/substrafl/strategies/fed_pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from substrafl.exceptions import EmptySharedStatesError
 from substrafl.nodes.aggregation_node import AggregationNode
 from substrafl.nodes.references.local_state import LocalStateRef
 from substrafl.nodes.references.shared_state import SharedStateRef
 from substrafl.nodes.test_data_node import TestDataNode
 from substrafl.nodes.train_data_node import TrainDataNode
 from substrafl.remote import remote
-from substrafl.schemas import FedPCAAveragedState
-from substrafl.schemas import FedPCASharedState
-from substrafl.schemas import StrategyName
+from substrafl.strategies.schemas import FedPCAAveragedState
+from substrafl.strategies.schemas import FedPCASharedState
+from substrafl.strategies.schemas import StrategyName
 from substrafl.strategies.strategy import Strategy
 
 logger = logging.getLogger(__name__)
 
 
 class FedPCA(Strategy):
     """Federated Principal Component Analysis strategy.
```

### Comparing `substrafl-0.36.0rc2/substrafl/strategies/newton_raphson.py` & `substrafl-0.37.0rc1/substrafl/strategies/newton_raphson.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from substrafl.exceptions import SharedStatesError
 from substrafl.nodes.aggregation_node import AggregationNode
 from substrafl.nodes.references.local_state import LocalStateRef
 from substrafl.nodes.references.shared_state import SharedStateRef
 from substrafl.nodes.test_data_node import TestDataNode
 from substrafl.nodes.train_data_node import TrainDataNode
 from substrafl.remote import remote
-from substrafl.schemas import NewtonRaphsonAveragedStates
-from substrafl.schemas import NewtonRaphsonSharedState
-from substrafl.schemas import StrategyName
+from substrafl.strategies.schemas import NewtonRaphsonAveragedStates
+from substrafl.strategies.schemas import NewtonRaphsonSharedState
+from substrafl.strategies.schemas import StrategyName
 from substrafl.strategies.strategy import Strategy
 
 
 class NewtonRaphson(Strategy):
     """Newton-Raphson strategy.
 
     Newton-Raphson strategy is based on Newton-Raphson distributed method. It leads to a faster divergence than
```

### Comparing `substrafl-0.36.0rc2/substrafl/strategies/scaffold.py` & `substrafl-0.37.0rc1/substrafl/strategies/scaffold.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from substrafl.algorithms.algo import Algo
 from substrafl.nodes.aggregation_node import AggregationNode
 from substrafl.nodes.references.local_state import LocalStateRef
 from substrafl.nodes.references.shared_state import SharedStateRef
 from substrafl.nodes.test_data_node import TestDataNode
 from substrafl.nodes.train_data_node import TrainDataNode
 from substrafl.remote import remote
-from substrafl.schemas import ScaffoldAveragedStates
-from substrafl.schemas import ScaffoldSharedState
-from substrafl.schemas import StrategyName
+from substrafl.strategies.schemas import ScaffoldAveragedStates
+from substrafl.strategies.schemas import ScaffoldSharedState
+from substrafl.strategies.schemas import StrategyName
 from substrafl.strategies.strategy import Strategy
 
 
 class Scaffold(Strategy):
     """Scaffold strategy.
     Paper: https://arxiv.org/pdf/1910.06378.pdf
     Scaffold is Federated Averaging with control variates.
```

### Comparing `substrafl-0.36.0rc2/substrafl/strategies/single_organization.py` & `substrafl-0.37.0rc1/substrafl/strategies/single_organization.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional
 
 from substrafl.algorithms import Algo
 from substrafl.nodes import AggregationNode
 from substrafl.nodes import TestDataNode
 from substrafl.nodes import TrainDataNode
 from substrafl.nodes.references.local_state import LocalStateRef
-from substrafl.schemas import StrategyName
+from substrafl.strategies.schemas import StrategyName
 from substrafl.strategies.strategy import Strategy
 
 logger = logging.getLogger(__name__)
 
 
 class SingleOrganization(Strategy):
     """Single organization strategy.
```

### Comparing `substrafl-0.36.0rc2/substrafl/strategies/strategy.py` & `substrafl-0.37.0rc1/substrafl/strategies/strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from abc import ABC
 from abc import abstractmethod
+from pathlib import Path
+from typing import Any
 from typing import List
 from typing import Optional
 from typing import TypeVar
 
 from substrafl import exceptions
 from substrafl.algorithms.algo import Algo
+from substrafl.compute_plan_builder import ComputePlanBuilder
 from substrafl.evaluation_strategy import EvaluationStrategy
 from substrafl.nodes.aggregation_node import AggregationNode
 from substrafl.nodes.test_data_node import TestDataNode
 from substrafl.nodes.train_data_node import TrainDataNode
-from substrafl.schemas import StrategyName
+from substrafl.strategies.schemas import StrategyName
 
 SharedState = TypeVar("SharedState")
 
 
-class Strategy(ABC):
+class Strategy(ComputePlanBuilder):
     """Base strategy to be inherited from SubstraFL strategies."""
 
     def __init__(self, algo: Algo, *args, **kwargs):
         """
         All child class arguments need to be passed to it through its ``args`` and ``kwargs``
         in order to use them when instantiating it as a RemoteStruct in each process.
 
         Example:
 
             .. code-block:: python
 
                 class MyStrat(Strategy):
                     def __init__(self, algo, my_custom_arg):
-                        super.__init__(algo=algo, my_custom_arg=my_custom_arg)
+                        super().__init__(algo=algo, my_custom_arg=my_custom_arg)
 
         Args:
             algo (Algo): The algorithm your strategy will execute (i.e. train and test on all the specified nodes)
 
         Raises:
             exceptions.IncompatibleAlgoStrategyError: Raise an error if the strategy name is not in ``algo.strategies``.
         """
-        self.args = args
-        self.kwargs = kwargs
 
-        self.kwargs.update({"algo": algo})
+        super().__init__(algo=algo, *args, **kwargs)
 
         self.algo = algo
 
         if self.name not in algo.strategies:
             raise exceptions.IncompatibleAlgoStrategyError(
                 f"The algo {self.algo.__class__.__name__} is not compatible with the strategy "
                 f"{self.__class__.__name__}, "
@@ -137,39 +137,42 @@
             test_data_nodes (typing.List[TestDataNode]): list of nodes on which to evaluate
             train_data_nodes (typing.List[TrainDataNode]): list of nodes on which the model has
                 been trained
             round_idx (int): index of the round
         """
         raise NotImplementedError
 
-    def build_graph(
+    def build_compute_plan(
         self,
         train_data_nodes: List[TrainDataNode],
         aggregation_node: Optional[List[AggregationNode]],
         evaluation_strategy: Optional[EvaluationStrategy],
         num_rounds: int,
-        clean_models: Optional[bool],
-    ):
-        """Build the computation graph of the strategy.
+        clean_models: Optional[bool] = True,
+    ) -> None:
+        """Build the compute plan of the strategy.
         The built graph will be stored by side effect in the given train_data_nodes,
         aggregation_nodes and evaluation_strategy.
         This function create a graph be first calling the initialization_round method of the strategy
         at round 0, and then call the perform_round method for each new round.
         If the current round is part of the evaluation strategy, the perform_predict method is
         called to complete the graph.
 
         Args:
             train_data_nodes (typing.List[TrainDataNode]): list of the train organizations
             aggregation_node (typing.Optional[AggregationNode]): aggregation node, necessary for
                 centralized strategy, unused otherwise
-            evaluation_strategy (Optional[EvaluationStrategy]): _description_
-            num_rounds (int): _description_
+            evaluation_strategy (Optional[EvaluationStrategy]): evaluation strategy to follow for testing models.
+            num_rounds (int): Number of times to repeat the compute plan sub-graph (define in perform round).
             clean_models (bool): Clean the intermediary models on the Substra platform. Set it to False
                 if you want to download or re-use intermediary models. This causes the disk space to fill
                 quickly so should be set to True unless needed. Defaults to True.
+
+        Returns:
+            None
         """
         additional_orgs_permissions = (
             evaluation_strategy.test_data_nodes_org_ids if evaluation_strategy is not None else set()
         )
 
         # create computation graph.
         for round_idx in range(0, num_rounds + 1):
@@ -190,7 +193,13 @@
 
             if evaluation_strategy is not None and next(evaluation_strategy):
                 self.perform_predict(
                     train_data_nodes=train_data_nodes,
                     test_data_nodes=evaluation_strategy.test_data_nodes,
                     round_idx=round_idx,
                 )
+
+    def save_local_state(self, path: Path) -> None:
+        self.algo.save_local_state(path)
+
+    def load_local_state(self, path: Path) -> Any:
+        return self.algo.load_local_state(path)
```

### Comparing `substrafl-0.36.0rc2/substrafl.egg-info/PKG-INFO` & `substrafl-0.37.0rc1/substrafl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrafl
-Version: 0.36.0rc2
+Version: 0.37.0rc1
 Summary: A high-level federated learning Python library to run      federated learning experiments at scale on a Substra network
 Home-page: https://docs.substra.org/
 Author: Owkin, Inc.
 License: Apache 2.0
 Description: readme
 Keywords: substrafl
 Platform: UNKNOWN
```

### Comparing `substrafl-0.36.0rc2/substrafl.egg-info/SOURCES.txt` & `substrafl-0.37.0rc1/substrafl.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 substrafl/__init__.py
 substrafl/__version__.py
-substrafl/dependency.py
+substrafl/compute_plan_builder.py
+substrafl/constants.py
 substrafl/evaluation_strategy.py
 substrafl/exceptions.py
 substrafl/experiment.py
 substrafl/logger.py
 substrafl/model_loading.py
 substrafl/schemas.py
 substrafl.egg-info/PKG-INFO
@@ -22,14 +23,18 @@
 substrafl/algorithms/pytorch/torch_base_algo.py
 substrafl/algorithms/pytorch/torch_fed_avg_algo.py
 substrafl/algorithms/pytorch/torch_fed_pca_algo.py
 substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
 substrafl/algorithms/pytorch/torch_scaffold_algo.py
 substrafl/algorithms/pytorch/torch_single_organization_algo.py
 substrafl/algorithms/pytorch/weight_manager.py
+substrafl/dependency/__init__.py
+substrafl/dependency/constants.py
+substrafl/dependency/path_management.py
+substrafl/dependency/schemas.py
 substrafl/index_generator/__init__.py
 substrafl/index_generator/base.py
 substrafl/index_generator/np_index_generator.py
 substrafl/nodes/__init__.py
 substrafl/nodes/aggregation_node.py
 substrafl/nodes/node.py
 substrafl/nodes/test_data_node.py
@@ -39,19 +44,20 @@
 substrafl/nodes/references/shared_state.py
 substrafl/remote/__init__.py
 substrafl/remote/decorators.py
 substrafl/remote/operations.py
 substrafl/remote/remote_struct.py
 substrafl/remote/substratools_methods.py
 substrafl/remote/register/__init__.py
-substrafl/remote/register/generate_wheel.py
+substrafl/remote/register/manage_dependencies.py
 substrafl/remote/register/register.py
 substrafl/remote/serializers/__init__.py
 substrafl/remote/serializers/pickle_serializer.py
 substrafl/remote/serializers/serializer.py
 substrafl/strategies/__init__.py
 substrafl/strategies/fed_avg.py
 substrafl/strategies/fed_pca.py
 substrafl/strategies/newton_raphson.py
 substrafl/strategies/scaffold.py
+substrafl/strategies/schemas.py
 substrafl/strategies/single_organization.py
 substrafl/strategies/strategy.py
```

