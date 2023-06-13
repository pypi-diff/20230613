# Comparing `tmp/ml-management-0.0.35.tar.gz` & `tmp/ml-management-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ml-management-0.0.35.tar", last modified: Wed Jun  7 14:31:26 2023, max compression
+gzip compressed data, was "ml-management-0.0.36.tar", last modified: Tue Jun 13 14:34:11 2023, max compression
```

## Comparing `ml-management-0.0.35.tar` & `ml-management-0.0.36.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.313684 ml-management-0.0.35/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)       18 2022-11-15 15:35:02.000000 ml-management-0.0.35/MANIFEST.in
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.305684 ml-management-0.0.35/ML_management/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.35/ML_management/__init__.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/collectors/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      120 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     1092 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      456 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     1318 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/collectors.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/collectors/dummy/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      463 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/collectors/s3/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)    10557 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/collectors/topic_markers/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)   331440 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     3167 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/dataset_loader_template/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     2407 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      457 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/executor_template/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/executor_template/default_executors/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      895 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      843 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      869 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     4566 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      402 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      334 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/mlmanagement/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      581 2022-09-29 11:08:30.000000 ml-management-0.0.35/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     3392 2023-03-13 16:12:20.000000 ml-management-0.0.35/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     5054 2023-03-13 16:12:20.000000 ml-management-0.0.35/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)    13486 2023-06-07 12:57:40.000000 ml-management-0.0.35/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)    10262 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      201 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     5001 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      316 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/models/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.35/ML_management/models/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      949 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/models/patterns/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     4202 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      561 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      445 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      457 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/registry/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.35/ML_management/registry/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     2566 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/registry/exceptions.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     7556 2023-05-15 09:28:39.000000 ml-management-0.0.35/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.309684 ml-management-0.0.35/ML_management/tests/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-12-07 10:58:45.000000 ml-management-0.0.35/ML_management/tests/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     3361 2022-12-07 10:58:45.000000 ml-management-0.0.35/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     9298 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.313684 ml-management-0.0.35/ML_management/uploader_data/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     1582 2023-05-31 08:55:31.000000 ml-management-0.0.35/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      312 2023-06-07 14:31:26.313684 ml-management-0.0.35/PKG-INFO
--rw-rw-r--   0 boeing    (1000) boeing    (1000)       56 2022-08-01 13:04:47.000000 ml-management-0.0.35/README.md
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        7 2023-06-07 14:31:07.000000 ml-management-0.0.35/VERSION
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-07 14:31:26.313684 ml-management-0.0.35/ml_management.egg-info/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      312 2023-06-07 14:31:26.000000 ml-management-0.0.35/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     2449 2023-06-07 14:31:26.000000 ml-management-0.0.35/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        1 2023-06-07 14:31:26.000000 ml-management-0.0.35/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      154 2023-06-07 14:31:26.000000 ml-management-0.0.35/ml_management.egg-info/requires.txt
--rw-rw-r--   0 boeing    (1000) boeing    (1000)       14 2023-06-07 14:31:26.000000 ml-management-0.0.35/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 boeing    (1000) boeing    (1000)       38 2023-06-07 14:31:26.313684 ml-management-0.0.35/setup.cfg
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     1053 2023-05-31 08:55:31.000000 ml-management-0.0.35/setup.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.051743 ml-management-0.0.36/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       18 2023-05-04 09:01:13.000000 ml-management-0.0.36/MANIFEST.in
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.039743 ml-management-0.0.36/ML_management/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-04 09:01:13.000000 ml-management-0.0.36/ML_management/__init__.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.039743 ml-management-0.0.36/ML_management/collectors/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      120 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/collectors/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1092 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      456 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1318 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/collectors/collectors.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.039743 ml-management-0.0.36/ML_management/collectors/dummy/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      463 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.039743 ml-management-0.0.36/ML_management/collectors/s3/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)    10609 2023-06-13 11:06:20.000000 ml-management-0.0.36/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.043743 ml-management-0.0.36/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)   331440 2023-06-07 09:26:42.000000 ml-management-0.0.36/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     3167 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.043743 ml-management-0.0.36/ML_management/dataset_loader_template/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     2407 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      457 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.043743 ml-management-0.0.36/ML_management/executor_template/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.043743 ml-management-0.0.36/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      895 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      843 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      869 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     4566 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      402 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      334 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.047743 ml-management-0.0.36/ML_management/mlmanagement/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      581 2023-05-04 09:01:13.000000 ml-management-0.0.36/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     3392 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     5054 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)    13486 2023-06-08 10:13:29.000000 ml-management-0.0.36/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)    10262 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      201 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     5001 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      316 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.047743 ml-management-0.0.36/ML_management/models/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-04 09:01:13.000000 ml-management-0.0.36/ML_management/models/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      949 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.047743 ml-management-0.0.36/ML_management/models/patterns/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     4202 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      561 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      445 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      457 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.047743 ml-management-0.0.36/ML_management/registry/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-04 09:01:13.000000 ml-management-0.0.36/ML_management/registry/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     2566 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/registry/exceptions.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     7556 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.047743 ml-management-0.0.36/ML_management/tests/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-04 09:01:13.000000 ml-management-0.0.36/ML_management/tests/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     3361 2023-05-04 09:01:13.000000 ml-management-0.0.36/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     9275 2023-06-13 11:06:20.000000 ml-management-0.0.36/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.051743 ml-management-0.0.36/ML_management/uploader_data/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1694 2023-06-13 11:06:20.000000 ml-management-0.0.36/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      367 2023-06-13 14:34:11.051743 ml-management-0.0.36/PKG-INFO
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       56 2023-05-04 09:01:13.000000 ml-management-0.0.36/README.md
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        7 2023-06-13 14:30:58.000000 ml-management-0.0.36/VERSION
+drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.051743 ml-management-0.0.36/ml_management.egg-info/
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      367 2023-06-13 14:34:11.000000 ml-management-0.0.36/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     2449 2023-06-13 14:34:11.000000 ml-management-0.0.36/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        1 2023-06-13 14:34:11.000000 ml-management-0.0.36/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      154 2023-06-13 14:34:11.000000 ml-management-0.0.36/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       14 2023-06-13 14:34:11.000000 ml-management-0.0.36/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       38 2023-06-13 14:34:11.051743 ml-management-0.0.36/setup.cfg
+-rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1053 2023-06-07 09:12:12.000000 ml-management-0.0.36/setup.py
```

### Comparing `ml-management-0.0.35/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.36/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/collectors/collectors.py` & `ml-management-0.0.36/ML_management/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.36/ML_management/collectors/s3/s3collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,16 @@
     def _download_file(self, bucket: str, service_client, remote_file_path: str, local_path: str):
         dirpath = posixpath.dirname(remote_file_path)
         local_dir_path = os.path.join(local_path, dirpath)
         local_file_path = os.path.join(local_path, remote_file_path)
         if not os.path.exists(local_dir_path):
             os.makedirs(local_dir_path, exist_ok=True)
         try:
-            service_client.download_file(bucket, remote_file_path, local_file_path)
+            with open(local_file_path, "wb") as _file:
+                service_client.download_fileobj(bucket, remote_file_path, _file)
         except ClientError as err:
             if err.response["Error"]["Code"] == "404":
                 # maybe user forgot to add trailing slash? Try to download as folder
                 try:
                     remote_folder_path = remote_file_path + "/"
                     self._download_folder(bucket, service_client, remote_folder_path, local_path)
                 except S3FolderNotFound:
```

### Comparing `ml-management-0.0.35/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.36/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.36/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/dataset_loader_template/dataset_loader_pattern.py` & `ml-management-0.0.36/ML_management/dataset_loader_template/dataset_loader_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.36/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.36/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.36/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.36/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.36/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.36/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.36/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.36/ML_management/mlmanagement/mlmanagement.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.36/ML_management/mlmanagement/mlmanager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.36/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.36/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.36/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.36/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/registry/exceptions.py` & `ml-management-0.0.36/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/registry/registry_manager.py` & `ml-management-0.0.36/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.36/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.36/ML_management/tests/test_s3_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 from ML_management.collectors import COLLECTORS
 from ML_management.collectors.s3.s3collector import S3BucketNotFound, S3FolderNotFound, S3ObjectNotFound
 
 
 def mock_client_download_successful(*args, **kwargs):
     client = Mock(spec=boto3.client)
 
-    def mock_download_file(Bucket, Key, Filename, ExtraArgs=None, Callback=None, Config=None):
+    def mock_download_file(Bucket, Key, Fileobj, ExtraArgs=None, Callback=None, Config=None):
         files_content_map = {
             "sample_data/1.txt": "one\n",
             "sample_data/2.txt": "two\n",
             "sample_data/sample_folder/3.txt": "three\n",
         }
-        with open(Filename, "w") as f:
-            f.write(files_content_map[Key])
+        Fileobj.write(files_content_map[Key].encode("utf-8"))
 
-    client.download_file = Mock(side_effect=mock_download_file)
+    client.download_fileobj = Mock(side_effect=mock_download_file)
     return client
 
 
 def mock_client_download_folder_successful(*args, **kwargs):
     client = Mock(spec=boto3.client)
 
     class mock_paginator:
@@ -38,24 +37,23 @@
                         {"Key": "sample_data/1.txt"},
                         {"Key": "sample_data/2.txt"},
                         {"Key": "sample_data/sample_folder/3.txt"},
                     ],
                 }
             ]
 
-    def mock_download_file(Bucket, Key, Filename, ExtraArgs=None, Callback=None, Config=None):
+    def mock_download_file(Bucket, Key, Fileobj, ExtraArgs=None, Callback=None, Config=None):
         files_content_map = {
             "sample_data/1.txt": "one\n",
             "sample_data/2.txt": "two\n",
             "sample_data/sample_folder/3.txt": "three\n",
         }
-        with open(Filename, "w") as f:
-            f.write(files_content_map[Key])
+        Fileobj.write(files_content_map[Key].encode("utf-8"))
 
-    client.download_file = Mock(side_effect=mock_download_file)
+    client.download_fileobj = Mock(side_effect=mock_download_file)
     client.get_paginator = Mock(return_value=mock_paginator())
     return client
 
 
 def mock_client_bad_folder(*args, **kwargs):
     client = Mock(spec=boto3.client)
 
@@ -70,15 +68,15 @@
 def mock_client_bad_object(*args, **kwargs):
     client = Mock(spec=boto3.client)
 
     class mock_paginator:
         def paginate(self, *args, **kwargs):
             return [{"KeyCount": 0}]
 
-    client.download_file = Mock(side_effect=ClientError({"Error": {"Code": "404"}}, "download_file"))
+    client.download_fileobj = Mock(side_effect=ClientError({"Error": {"Code": "404"}}, "download_fileobj"))
     client.get_paginator = Mock(return_value=mock_paginator())
     client.head_bucket = Mock()
     return client
 
 
 def mock_client_bad_bucket_folder(*args, **kwargs):
     client = Mock(spec=boto3.client)
@@ -95,17 +93,17 @@
 def mock_client_bad_bucket_object(*args, **kwargs):
     client = Mock(spec=boto3.client)
 
     class mock_paginator:
         def paginate(self, *args, **kwargs):
             return [{"KeyCount": 0}]
 
-    client.download_file = Mock(side_effect=ClientError({"Error": {"Code": "404"}}, "download_file"))
+    client.download_fileobj = Mock(side_effect=ClientError({"Error": {"Code": "404"}}, "download_fileobj"))
     client.get_paginator = Mock(return_value=mock_paginator())
-    client.head_bucket = Mock(side_effect=ClientError({"Error": {"Code": "404"}}, "download_file"))
+    client.head_bucket = Mock(side_effect=ClientError({"Error": {"Code": "404"}}, "download_fileobj"))
     return client
 
 
 class TestS3Dataset(unittest.TestCase):
     """
     Mock S3 structure:
```

### Comparing `ml-management-0.0.35/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.36/ML_management/uploader_data/s3_uploader.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,13 +28,15 @@
             aws_secret_access_key=self.default_secret_access_key,
         )
         buckets = [item["Name"] for item in service_client.list_buckets()["Buckets"]]
         if bucket not in buckets:
             service_client.create_bucket(Bucket=bucket)
 
         if os.path.isfile(local_path):
-            service_client.upload_file(local_path, bucket)
+            with open(local_path, "rb") as _file:
+                service_client.upload_fileobj(_file, bucket)
         else:
             for root, _, files in os.walk(local_path):
                 for file in files:
                     filename = file if root == local_path else os.path.join(os.path.relpath(root, start=local_path), file)
-                    service_client.upload_file(os.path.join(root, file), bucket, filename)
+                    with open(os.path.join(root, file), "rb") as _file:
+                        service_client.upload_fileobj(_file, bucket, filename)
```

### Comparing `ml-management-0.0.35/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.36/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.35/setup.py` & `ml-management-0.0.36/setup.py`

 * *Files identical despite different names*

