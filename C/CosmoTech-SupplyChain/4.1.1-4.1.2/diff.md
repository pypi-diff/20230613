# Comparing `tmp/CosmoTech-SupplyChain-4.1.1.tar.gz` & `tmp/CosmoTech-SupplyChain-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CosmoTech-SupplyChain-4.1.1.tar", last modified: Thu Apr 20 13:46:40 2023, max compression
+gzip compressed data, was "CosmoTech-SupplyChain-4.1.2.tar", last modified: Tue Jun 13 08:32:09 2023, max compression
```

## Comparing `CosmoTech-SupplyChain-4.1.1.tar` & `CosmoTech-SupplyChain-4.1.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:40.843059 CosmoTech-SupplyChain-4.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:40.831059 CosmoTech-SupplyChain-4.1.1/CosmoTech_SupplyChain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-20 13:46:40.000000 CosmoTech-SupplyChain-4.1.1/CosmoTech_SupplyChain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2203 2023-04-20 13:46:40.000000 CosmoTech-SupplyChain-4.1.1/CosmoTech_SupplyChain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 13:46:40.000000 CosmoTech-SupplyChain-4.1.1/CosmoTech_SupplyChain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-20 13:46:40.000000 CosmoTech-SupplyChain-4.1.1/CosmoTech_SupplyChain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-20 13:46:40.000000 CosmoTech-SupplyChain-4.1.1/CosmoTech_SupplyChain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1195 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-20 13:46:40.843059 CosmoTech-SupplyChain-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:40.831059 CosmoTech-SupplyChain-4.1.1/Supplychain/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:40.835059 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3344 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/adt_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/adx_and_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/adx_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/cosmo_api_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3385 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/csv_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/csv_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/duration.py
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/excel_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/excel_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/folder_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/json_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/json_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/memory_folder_io.py
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/simulator_io.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/storage_queue_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:40.835059 CosmoTech-SupplyChain-4.1.1/Supplychain/Protocol/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Protocol/cmaes_optimization_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7621 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Protocol/default_transformation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4276 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Protocol/multiprocessing_optimization.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Protocol/objective_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Protocol/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:40.839059 CosmoTech-SupplyChain-4.1.1/Supplychain/Run/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5391 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Run/cmaes_optimization.py
--rw-r--r--   0 runner    (1001) docker     (122)    31357 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Run/local_sensitivity_analysis_comets.py
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Run/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Run/simulation_comets.py
--rw-r--r--   0 runner    (1001) docker     (122)     7760 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Run/uncertainty_analysis.py
--rw-r--r--   0 runner    (1001) docker     (122)    33487 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Run/uncertainty_analysis_comets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:40.839059 CosmoTech-SupplyChain-4.1.1/Supplychain/Schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Schema/adt_column_description.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Schema/default_values.py
--rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Schema/simulator_files_description.py
--rw-r--r--   0 runner    (1001) docker     (122)    20522 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Schema/validation_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:40.839059 CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6539 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/complete_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)    39924 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/from_dict_to_simulator.py
--rw-r--r--   0 runner    (1001) docker     (122)    11669 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/from_dict_to_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     6822 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/from_table_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)    52415 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/from_table_to_dict_old.py
--rw-r--r--   0 runner    (1001) docker     (122)    11402 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/patch_dict_with_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3058 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/production_route.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:40.839059 CosmoTech-SupplyChain-4.1.1/Supplychain/Validate/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21965 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Validate/validate_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:40.839059 CosmoTech-SupplyChain-4.1.1/Supplychain/Wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Wrappers/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)    18535 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/Wrappers/simulator.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 13:46:29.000000 CosmoTech-SupplyChain-4.1.1/Supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 13:46:40.843059 CosmoTech-SupplyChain-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-04-20 13:46:30.000000 CosmoTech-SupplyChain-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.719530 CosmoTech-SupplyChain-4.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.711530 CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-06-13 08:32:09.000000 CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2203 2023-06-13 08:32:09.000000 CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 08:32:09.000000 CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-13 08:32:09.000000 CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-13 08:32:09.000000 CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1195 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.711530 CosmoTech-SupplyChain-4.1.2/Supplychain/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.711530 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3344 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/adt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/adx_and_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/adx_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/cosmo_api_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3385 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/csv_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/csv_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/duration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/excel_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/excel_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/folder_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/json_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/json_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/memory_folder_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/simulator_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/storage_queue_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/cmaes_optimization_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7621 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/default_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4276 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/multiprocessing_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/objective_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5391 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/cmaes_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31357 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/local_sensitivity_analysis_comets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/simulation_comets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7760 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/uncertainty_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33487 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/uncertainty_analysis_comets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/adt_column_description.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/default_values.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/simulator_files_description.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20522 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/validation_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6539 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/complete_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39924 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_dict_to_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11669 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_dict_to_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6822 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_table_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52415 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_table_to_dict_old.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11402 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/patch_dict_with_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3058 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/production_route.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/Supplychain/Validate/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21965 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Validate/validate_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/Supplychain/Wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Wrappers/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18535 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Wrappers/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 08:32:09.719530 CosmoTech-SupplyChain-4.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-13 08:32:01.000000 CosmoTech-SupplyChain-4.1.2/setup.py
```

### Comparing `CosmoTech-SupplyChain-4.1.1/CosmoTech_SupplyChain.egg-info/SOURCES.txt` & `CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/LICENSE` & `CosmoTech-SupplyChain-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/README.md` & `CosmoTech-SupplyChain-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/adt_writer.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/adt_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/adx_and_file_writer.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/adx_and_file_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/adx_wrapper.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/adx_wrapper.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/cosmo_api_parameters.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/cosmo_api_parameters.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/csv_folder_reader.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/csv_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/csv_folder_writer.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/csv_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/duration.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/duration.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/excel_folder_reader.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/excel_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/excel_folder_writer.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/excel_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/folder_io.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/folder_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/json_folder_reader.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/json_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/json_folder_writer.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/json_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/memory_folder_io.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/memory_folder_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/simulator_io.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/simulator_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/storage_queue_writer.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/storage_queue_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Generic/timer.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/timer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Protocol/cmaes_optimization_algorithm.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/cmaes_optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Protocol/default_transformation.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/default_transformation.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Protocol/multiprocessing_optimization.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/multiprocessing_optimization.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Protocol/objective_functions.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/objective_functions.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Protocol/protocol.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Run/cmaes_optimization.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Run/cmaes_optimization.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Run/local_sensitivity_analysis_comets.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Run/local_sensitivity_analysis_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Run/simulation.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Run/simulation.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Run/simulation_comets.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Run/simulation_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Run/uncertainty_analysis.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Run/uncertainty_analysis.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Run/uncertainty_analysis_comets.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Run/uncertainty_analysis_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Schema/adt_column_description.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/adt_column_description.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Schema/default_values.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/default_values.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Schema/simulator_files_description.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/simulator_files_description.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Schema/validation_schemas.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/validation_schemas.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/complete_dict.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/complete_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/from_dict_to_simulator.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_dict_to_simulator.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/from_dict_to_table.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_dict_to_table.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/from_table_to_dict.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_table_to_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/from_table_to_dict_old.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_table_to_dict_old.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/patch_dict_with_parameters.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/patch_dict_with_parameters.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Transform/production_route.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/production_route.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Validate/validate_dict.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Validate/validate_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Wrappers/environment_variables.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Wrappers/environment_variables.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/Supplychain/Wrappers/simulator.py` & `CosmoTech-SupplyChain-4.1.2/Supplychain/Wrappers/simulator.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.1/setup.py` & `CosmoTech-SupplyChain-4.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = "4.1.1"
+VERSION = "v4.1.2"
 
 setuptools.setup(
     name='CosmoTech-SupplyChain',
     version=VERSION,
     author='Alexis Fossart',
     author_email='alexis.fossart@cosmotech.com',
     url='https://github.com/Cosmo-Tech/supplychain-python-library<',
```

