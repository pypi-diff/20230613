# Comparing `tmp/ai_transform-0.32.0.tar.gz` & `tmp/ai_transform-0.32.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.32.0.tar", last modified: Mon Jun  5 07:15:37 2023, max compression
+gzip compressed data, was "ai_transform-0.32.1.tar", last modified: Tue Jun 13 06:47:09 2023, max compression
```

## Comparing `ai_transform-0.32.0.tar` & `ai_transform-0.32.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.004160 ai_transform-0.32.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-06-05 07:15:05.000000 ai_transform-0.32.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-05 07:15:37.004160 ai_transform-0.32.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-05 07:15:05.000000 ai_transform-0.32.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:36.992159 ai_transform-0.32.0/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:36.996159 ai_transform-0.32.0/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29452 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:36.996159 ai_transform-0.32.0/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:36.996159 ai_transform-0.32.0/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:36.996159 ai_transform-0.32.0/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-05 07:15:05.000000 ai_transform-0.32.0/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:36.996159 ai_transform-0.32.0/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-05 07:15:36.000000 ai_transform-0.32.0/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-05 07:15:36.000000 ai_transform-0.32.0/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:15:36.000000 ai_transform-0.32.0/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-05 07:15:36.000000 ai_transform-0.32.0/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 07:15:36.000000 ai_transform-0.32.0/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-05 07:15:05.000000 ai_transform-0.32.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:15:37.004160 ai_transform-0.32.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-05 07:15:05.000000 ai_transform-0.32.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.000159 ai_transform-0.32.0/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.004160 ai_transform-0.32.0/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.004160 ai_transform-0.32.0/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:37.004160 ai_transform-0.32.0/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-05 07:15:05.000000 ai_transform-0.32.0/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.457221 ai_transform-0.32.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-06-13 06:46:50.000000 ai_transform-0.32.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 06:47:09.457221 ai_transform-0.32.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-13 06:46:50.000000 ai_transform-0.32.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.449221 ai_transform-0.32.1/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.449221 ai_transform-0.32.1/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29487 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.449221 ai_transform-0.32.1/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.449221 ai_transform-0.32.1/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15130 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15264 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-13 06:46:50.000000 ai_transform-0.32.1/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.449221 ai_transform-0.32.1/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 06:47:09.000000 ai_transform-0.32.1/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-13 06:47:09.000000 ai_transform-0.32.1/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:47:09.000000 ai_transform-0.32.1/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-13 06:47:09.000000 ai_transform-0.32.1/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 06:47:09.000000 ai_transform-0.32.1/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 06:46:50.000000 ai_transform-0.32.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:47:09.457221 ai_transform-0.32.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-13 06:46:50.000000 ai_transform-0.32.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.453221 ai_transform-0.32.1/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.457221 ai_transform-0.32.1/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.457221 ai_transform-0.32.1/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.457221 ai_transform-0.32.1/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:09.457221 ai_transform-0.32.1/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-13 06:46:50.000000 ai_transform-0.32.1/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.32.0/LICENSE` & `ai_transform-0.32.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/README.md` & `ai_transform-0.32.1/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/__init__.py` & `ai_transform-0.32.1/ai_transform/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.32.0"
+__version__ = "0.32.1"
 
 from ai_transform.timer import Timer
 
 _TIMER = Timer()
 _TIMER.start()
```

### Comparing `ai_transform-0.32.0/ai_transform/api/api.py` & `ai_transform-0.32.1/ai_transform/api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,17 +158,18 @@
     def _list_datasets(self):
         response = self.get(suffix="/datasets/list")
         return get_response(response)
 
     def _create_dataset(
         self, dataset_id: str, schema: Optional[Schema] = None, upsert: bool = True, expire: bool = False
     ) -> Any:
-        response = self.post(
-            suffix=f"/datasets/create", json=dict(id=dataset_id, schema=schema, upsert=upsert, expire=expire)
-        )
+        obj = dict(id=dataset_id, upsert=upsert, expire=expire)
+        if schema:
+            obj["schema"] = schema
+        response = self.post(suffix=f"/datasets/create", json=obj)
         return get_response(response)
 
     def _delete_dataset(self, dataset_id: str) -> Any:
         response = self.post(suffix=f"/datasets/{dataset_id}/delete")
         return get_response(response)
 
     def _get_schema(self, dataset_id: str) -> Schema:
```

### Comparing `ai_transform-0.32.0/ai_transform/api/client.py` & `ai_transform-0.32.1/ai_transform/api/client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/api/helpers.py` & `ai_transform-0.32.1/ai_transform/api/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/api/wrappers.py` & `ai_transform-0.32.1/ai_transform/api/wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/components/components.py` & `ai_transform-0.32.1/ai_transform/components/components.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/config.py` & `ai_transform-0.32.1/ai_transform/config.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/dataset/dataset.py` & `ai_transform-0.32.1/ai_transform/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/dataset/field.py` & `ai_transform-0.32.1/ai_transform/dataset/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,19 +103,18 @@
         return [{"field": self._field, "filter_type": filter_type, "condition": ">=", "condition_value": other}]
 
     def contains(self, other: str) -> Filter:
         return [{"field": self._field, "filter_type": "contains", "condition": "==", "condition_value": other}]
 
     def exists(self) -> Filter:
         if "_chunk_" in self._field:
-            count = self._field.count(".")
-            if count:
-                parent_field = self._field.split(".")[0]
-            else:
+            if self._field.endswith("_chunk_"):
                 parent_field = self._field
+            else:
+                parent_field = self._field.split(".")[0]
 
             return [{"chunk": {"path": parent_field, "filters": [{"fieldExists": {"field": self._field}}]}}]
         return [{"field": self._field, "filter_type": "exists", "condition": "==", "condition_value": " "}]
 
     def not_exists(self) -> Filter:
         return [{"field": self._field, "filter_type": "exists", "condition": "!=", "condition_value": " "}]
```

### Comparing `ai_transform-0.32.0/ai_transform/engine/abstract_engine.py` & `ai_transform-0.32.1/ai_transform/engine/abstract_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         if select_fields is not None:
             fields_to_add = []
             for field in select_fields:
                 if "_chunk_" in field:
                     chunk_index = field.index("_chunk_") + len("_chunk_")
                     chunk_field = field[:chunk_index]
                     fields_to_add += [chunk_field]
-            select_fields += fields_to_add
+            select_fields = select_fields + fields_to_add
             select_fields = list(set(select_fields))
         else:
             select_fields = []
 
         self._select_fields = select_fields
 
         self.worker_number = worker_number
@@ -105,16 +105,16 @@
         if filters is None:
             filters = []
         assert isinstance(filters, list), "Filters must be applied as a list of Dictionaries"
 
         self._refresh = refresh
         self._after_id = after_id
 
-        filters += self._get_refresh_filter()
-        filters += self._get_workflow_filter()
+        filters = filters + self._get_refresh_filter()
+        filters = filters + self._get_workflow_filter()
 
         self._filters = filters
 
         if self.documents:
             self._size = len(documents)
         else:
             self._size = dataset.len(filters=filters) if self._limit_documents is None else self._limit_documents
```

### Comparing `ai_transform-0.32.0/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.32.1/ai_transform/engine/dense_output_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from ai_transform.operator.dense_operator import DenseOperator
 from ai_transform.engine.abstract_engine import AbstractEngine
 from ai_transform.types import Filter
 from ai_transform.logger import ic
 
 
 class DenseOutputEngine(AbstractEngine):
+    operator: DenseOperator
+
     def __init__(
         self,
         dataset: Dataset = None,
         operator: DenseOperator = None,
         filters: Optional[List[Filter]] = None,
         select_fields: Optional[List[str]] = None,
         pull_chunksize: Optional[int] = 3000,
@@ -68,20 +70,28 @@
         output_dataset_ids = []
 
         self.operator.pre_hooks(self._dataset)
 
         for mega_batch in self.api_progress(iterator):
             for mini_batch in AbstractEngine.chunk_documents(self._transform_chunksize, mega_batch):
                 document_mapping = self._operate(mini_batch)
+
                 for dataset_id, documents in document_mapping.items():
                     output_dataset_ids.append(dataset_id)
                     dataset = Dataset.from_details(dataset_id, self.token)
                     result = dataset.bulk_insert(documents)
                     ic({"dataset_id": dataset_id, "result": result})
 
         self.operator.post_hooks(self._dataset)
 
         output_datasets = self.datasets_from_ids(output_dataset_ids)
-        self.operator.store_dataset_relationship(self.dataset, output_datasets)
+        self.store_dataset_relationship(output_datasets)
 
     def datasets_from_ids(self, dataset_ids: Sequence[str]) -> Sequence[Dataset]:
         return [Dataset.from_details(dataset_id, self.token) for dataset_id in dataset_ids]
+
+    def store_dataset_relationship(self, output_datasets: Sequence[Dataset]):
+        self.dataset.update_metadata(
+            {"_child_datasets_": [output_dataset.dataset_id for output_dataset in output_datasets]}
+        )
+        for output_dataset in output_datasets:
+            output_dataset.update_metadata({"_parent_dataset_": self.dataset.dataset_id})
```

### Comparing `ai_transform-0.32.0/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.32.1/ai_transform/engine/in_memory_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/engine/multipass_engine.py` & `ai_transform-0.32.1/ai_transform/engine/multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.32.1/ai_transform/engine/small_batch_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/engine/stable_engine.py` & `ai_transform-0.32.1/ai_transform/engine/stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/errors.py` & `ai_transform-0.32.1/ai_transform/errors.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/logger.py` & `ai_transform-0.32.1/ai_transform/logger.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/operator/abstract_operator.py` & `ai_transform-0.32.1/ai_transform/operator/abstract_operator.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 class AbstractOperator(ABC):
     def __init__(
         self,
         input_fields: Optional[List[str]] = None,
         output_fields: Optional[Union[Dict[str, str], List[str]]] = None,
         enable_postprocess: Optional[bool] = True,
     ):
-
         if input_fields is not None and output_fields is not None:
             if any(input_field in output_fields for input_field in input_fields):
                 detected_fields = [input_field for input_field in input_fields if input_field in output_fields]
                 warnings.warn(f"Some input fields are present in the output fields, namely {str(detected_fields)}")
                 for field in detected_fields:
                     output_fields.remove(field)
 
@@ -167,24 +166,30 @@
     ):
         """
         Transform and upload an object
         """
         from ai_transform.api.client import Client
 
         output = self.transform(documents=documents)
+        if hasattr(documents, "to_json"):
+            output = output.to_json()
+        else:
+            for index in range(len(output)):
+                if hasattr(output[index], "to_json"):
+                    output[index] = output[index].to_json()
         client = Client(authorization_token)
         return client.api._set_workflow_status(
             job_id=job_id,
             workflow_name=workflow_name,
             additional_information=additional_information,
             metadata=metadata,
             status=status,
             send_email=send_email,
             worker_number=worker_number,
-            output=output,
+            output={"output": output},
         )
 
     def pre_hooks(self, dataset: Dataset):
         pass
 
     def post_hooks(self, dataset: Dataset):
         pass
```

### Comparing `ai_transform-0.32.0/ai_transform/operator/dense_operator.py` & `ai_transform-0.32.1/ai_transform/operator/dense_operator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 
 from abc import abstractmethod
 
 from typing import Dict, Sequence
 
 from ai_transform.operator.abstract_operator import AbstractOperator
-from ai_transform.dataset.dataset import Dataset
 from ai_transform.utils.document import Document
 from ai_transform.utils.document_list import DocumentList
 
 logger = logging.getLogger(__file__)
 
 
 DatasetID = str
@@ -20,22 +19,17 @@
     "please ensure the output of the operator is a dict that is a mapping of dataset_ids to documents"
 )
 
 
 class DenseOperator(AbstractOperator):
     def __call__(self, old_documents: DocumentList) -> DenseOperatorOutput:
         datum = self.transform(old_documents)
-        assert isinstance(datum, dict), BAD_OPERATOR_MESSAGE
+        if not isinstance(datum, dict):
+            raise ValueError(BAD_OPERATOR_MESSAGE)
         for _, documents in datum.items():
-            assert isinstance(documents, Sequence)
+            if not isinstance(documents, Sequence):
+                raise ValueError(BAD_OPERATOR_MESSAGE)
         return datum
 
     @abstractmethod
     def transform(self, documents: DocumentList) -> DenseOperatorOutput:
         raise NotImplementedError
-
-    def store_dataset_relationship(self, input_dataset: Dataset, output_datasets: Sequence[Dataset]):
-        input_dataset.update_metadata(
-            {"_child_datasets_": [output_dataset.dataset_id for output_dataset in output_datasets]}
-        )
-        for output_dataset in output_datasets:
-            output_dataset.update_metadata({"_parent_dataset_": input_dataset.dataset_id})
```

### Comparing `ai_transform-0.32.0/ai_transform/timer.py` & `ai_transform-0.32.1/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/types.py` & `ai_transform-0.32.1/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/utils/document.py` & `ai_transform-0.32.1/ai_transform/utils/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,25 +137,15 @@
         """
         List the available chunks inside of the document.
         """
         # based on conversation with API team
         return [k for k in self.keys() if k.endswith("_chunk_")]
 
     def get_chunk(self, chunk_field: str, field: str = None, default: str = None):
-        """
-        Returns a list of values.
-        """
-        # provide a recursive implementation for getting chunks
-        from ai_transform.utils.document_list import DocumentList
-
-        document_list = DocumentList(self.get(chunk_field, default=default))
-        # Get the field across chunks
-        if field is None:
-            return document_list
-        return [d.get(field, default=default) for d in document_list.data]
+        return [document.get(field, default) for document in self.get(chunk_field, default=default)]
 
     def _create_chunk_documents(self, field: str, values: list, generate_id: bool = False):
         """
         create chunk documents based on a given field and value.
         """
         from ai_transform.utils.document_list import DocumentList
```

### Comparing `ai_transform-0.32.0/ai_transform/utils/document_list.py` & `ai_transform-0.32.1/ai_transform/utils/document_list.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/utils/example_documents.py` & `ai_transform-0.32.1/ai_transform/utils/example_documents.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
 
 def create_id():
     return str(uuid.uuid4())
 
 
 def generate_random_string(string_length: int = 5) -> str:
-
     """Generate a random string of letters and numbers"""
     return "".join(random.choice(string.ascii_uppercase + string.digits) for _ in range(string_length))
 
 
 def generate_random_vector(vector_length: int = 5) -> Vector:
     """Generate a random list of floats"""
     return [random.random() for _ in range(vector_length)]
@@ -88,15 +87,24 @@
         "_chunk_": [{"label": generate_random_label(), "label_chunkvector_": generate_random_vector()}],
     }
 
     return Document(document)
 
 
 def mock_documents(n: int = 100, vector_length: int = 5) -> DocumentList:
-    return DocumentList([vector_document(vector_length) for _ in range(n)])
+    documents = [vector_document(vector_length) for _ in range(n)]
+    return DocumentList(documents)
+
+
+def incomplete_documents(n: int = 100, vector_length: int = 5) -> DocumentList:
+    documents = [vector_document(vector_length).data for _ in range(n)]
+    for document in documents:
+        for key in random.sample(document.keys(), 3):
+            document.pop(key)
+    return DocumentList(documents)
 
 
 def static_documents(n: int = 100) -> DocumentList:
     return DocumentList([{"text_field": str(i), "numeric_field": i} for i in range(n)])
 
 
 def tag_document(n_tags: int = 5):
```

### Comparing `ai_transform-0.32.0/ai_transform/utils/json_encoder.py` & `ai_transform-0.32.1/ai_transform/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/utils/keyphrase.py` & `ai_transform-0.32.1/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.32.1/ai_transform/workflow/abstract_workflow.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/workflow/context_manager.py` & `ai_transform-0.32.1/ai_transform/workflow/context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform/workflow/helpers.py` & `ai_transform-0.32.1/ai_transform/workflow/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.32.1/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/setup.py` & `ai_transform-0.32.1/setup.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/conftest.py` & `ai_transform-0.32.1/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,22 @@
 from ai_transform.engine.stable_engine import StableEngine
 
 from ai_transform.operator.abstract_operator import AbstractOperator
 from ai_transform.operator.dense_operator import DenseOperator
 
 from ai_transform.utils.document import Document
 from ai_transform.utils.document_list import DocumentList
-from ai_transform.utils.example_documents import mock_documents, static_documents, tag_documents
+from ai_transform.utils.example_documents import (
+    mock_documents,
+    static_documents,
+    tag_documents,
+    generate_random_vector,
+    incomplete_documents,
+)
+
 
 TEST_TOKEN = os.getenv("TEST_TOKEN")
 test_creds = process_token(TEST_TOKEN)
 
 
 @pytest.fixture(scope="session")
 def test_token() -> str:
@@ -40,19 +47,19 @@
 @pytest.fixture(scope="function")
 def test_dataset_id() -> str:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
     return dataset_id
 
 
-@pytest.fixture(scope="class")
+@pytest.fixture(scope="function")
 def empty_dataset(test_client: Client) -> Dataset:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
-    dataset = test_client.Dataset(dataset_id, expire=True)
+    dataset = test_client.Dataset(dataset_id, expire=False)
     yield dataset
     test_client.delete_dataset(dataset_id)
 
 
 @pytest.fixture(scope="class")
 def full_dataset(test_client: Client) -> Dataset:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
@@ -133,34 +140,44 @@
     dataset_id = f"_sample_dataset_{salt}"
     dataset = test_client.Dataset(dataset_id, expire=True)
     dataset.insert_documents(static_documents(20))
     yield dataset
     test_client.delete_dataset(dataset_id)
 
 
-@pytest.fixture(scope="class")
-def dense_input_dataset(test_client: Client) -> Dataset:
+@pytest.fixture(scope="function")
+def dense_input_dataset1(test_client: Client) -> Dataset:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
     dataset = test_client.Dataset(dataset_id, expire=True)
     dataset.insert_documents(static_documents(2))
     yield dataset
     test_client.delete_dataset(dataset_id)
 
 
-@pytest.fixture(scope="class")
+@pytest.fixture(scope="function")
+def dense_input_dataset2(test_client: Client) -> Dataset:
+    salt = "".join(random.choices(string.ascii_lowercase, k=10))
+    dataset_id = f"_sample_dataset_{salt}"
+    dataset = test_client.Dataset(dataset_id, expire=True)
+    dataset.insert_documents(mock_documents(100))
+    yield dataset
+    test_client.delete_dataset(dataset_id)
+
+
+@pytest.fixture(scope="function")
 def dense_output_dataset1(test_client: Client) -> Dataset:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
     dataset = test_client.Dataset(dataset_id, expire=True)
     yield dataset
     test_client.delete_dataset(dataset_id)
 
 
-@pytest.fixture(scope="class")
+@pytest.fixture(scope="function")
 def dense_output_dataset2(test_client: Client) -> Dataset:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
     dataset = test_client.Dataset(dataset_id, expire=True)
     yield dataset
     test_client.delete_dataset(dataset_id)
 
@@ -261,14 +278,45 @@
             return {dataset_id: documents for dataset_id in self.output_dataset_ids}
 
     output_dataset_ids = (dense_output_dataset1.dataset_id, dense_output_dataset2.dataset_id)
     return TestDenseOperator(output_dataset_ids)
 
 
 @pytest.fixture(scope="function")
+def test_chunk_dense_operator(dense_output_dataset1: Dataset, dense_output_dataset2: Dataset) -> DenseOperator:
+    class TestDenseOperator(DenseOperator):
+        def __init__(self, output_dataset_ids: Sequence[str]):
+            self.output_dataset_ids = output_dataset_ids
+            self._chunk_field = "_chunk_"
+            self._text_field = "label"
+            self._alias = "default"
+            super().__init__()
+
+        def transform(self, documents: List[Document]) -> List[Document]:
+            outputs = []
+            for document in documents:
+                texts = document.get_chunk(chunk_field=self._chunk_field, field=self._text_field)
+                text_vectors = [generate_random_vector() for _ in range(len(texts))]
+
+                for sent_index, text_vector in enumerate(text_vectors):
+                    outputs.append(
+                        {
+                            "_id": document["_id"] + f":{sent_index}",
+                            f"{self._text_field}_{self._alias}_vector_": text_vector,
+                            "_order": sent_index,
+                        }
+                    )
+
+            return {dataset_id: documents for dataset_id in self.output_dataset_ids}
+
+    output_dataset_ids = (dense_output_dataset1.dataset_id, dense_output_dataset2.dataset_id)
+    return TestDenseOperator(output_dataset_ids)
+
+
+@pytest.fixture(scope="function")
 def test_engine(full_dataset: Dataset, test_operator: AbstractOperator) -> StableEngine:
     return StableEngine(dataset=full_dataset, operator=test_operator)
 
 
 @pytest.fixture(scope="function")
 def test_paid_engine(full_dataset: Dataset, test_paid_operator: AbstractOperator) -> StableEngine:
     return StableEngine(dataset=full_dataset, operator=test_paid_operator)
@@ -280,15 +328,15 @@
 
 
 @pytest.fixture(scope="function")
 def test_sentiment_workflow_token(test_client: Client) -> str:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
     dataset = test_client.Dataset(dataset_id, expire=True)
-    dataset.insert_documents(mock_documents(20))
+    dataset.insert_documents(incomplete_documents(20))
     time.sleep(1)
     job_id = str(uuid.uuid4())
     config = dict(
         job_id=job_id,
         authorizationToken=test_client.credentials.token,
         dataset_id=dataset_id,
         text_field="sample_1_label",
@@ -357,15 +405,15 @@
 
 
 @pytest.fixture(scope="function")
 def test_cluster_workflow_token(test_client: Client) -> str:
     salt = "".join(random.choices(string.ascii_lowercase, k=10))
     dataset_id = f"_sample_dataset_{salt}"
     dataset = test_client.Dataset(dataset_id, expire=True)
-    dataset.insert_documents(mock_documents(20))
+    dataset.insert_documents(incomplete_documents(20))
     job_id = str(uuid.uuid4())
     print(job_id)
     config = dict(
         job_id=job_id,
         authorizationToken=test_client.credentials.token,
         dataset_id=dataset_id,
         vector_fields=["sample_1_vector_"],
```

### Comparing `ai_transform-0.32.0/tests/core/test_api/test_client.py` & `ai_transform-0.32.1/tests/core/test_api/test_client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/core/test_api/test_endpoints.py` & `ai_transform-0.32.1/tests/core/test_api/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.32.1/tests/core/test_api/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/core/test_api/test_wrappers.py` & `ai_transform-0.32.1/tests/core/test_api/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.32.1/tests/core/test_dataset/test_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import pytest
 import random
 
 from ai_transform.dataset.dataset import Dataset
 from ai_transform.utils.example_documents import mock_documents
 
 
-@pytest.mark.usefixtures("empty_dataset")
 class TestDataset1:
-    def test_create_delete(self, empty_dataset: Dataset):
-        empty_dataset.delete()
-        empty_dataset.create()
-        assert True
-
     def test_insert(self, empty_dataset: Dataset):
         documents = mock_documents(100)
         result = empty_dataset.insert_documents(documents)
         assert result["inserted"] == 100
 
     def test_get_all(self, full_dataset: Dataset):
         res = full_dataset.get_all_documents()
         assert len(res["documents"]) == 20
 
+    def test_create_delete(self, empty_dataset: Dataset):
+        empty_dataset.delete()
+        empty_dataset.create()
+        assert True
+
 
 @pytest.mark.usefixtures("full_dataset")
 class TestDataset2:
     def test_schema(self, full_dataset: Dataset):
         documents = mock_documents(5)
         keys = documents[0].keys()
         keys = [".".join([sf for sf in nested_field.split(".") if not sf.isdigit()]) for nested_field in keys]
```

### Comparing `ai_transform-0.32.0/tests/core/test_dataset/test_field.py` & `ai_transform-0.32.1/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.32.1/tests/core/test_dataset/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/core/test_engine/test_engine.py` & `ai_transform-0.32.1/tests/core/test_engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.32.1/tests/core/test_engine/test_engine_playground.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.32.1/tests/core/test_engine/test_multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.32.1/tests/core/test_engine/test_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/core/test_operator/test_abstract_operator.py` & `ai_transform-0.32.1/tests/core/test_operator/test_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.32.1/tests/core/test_operator/test_document_diff.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.32.1/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.32.0/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.32.1/tests/core/test_workflow/test_workflow.py`

 * *Files identical despite different names*

