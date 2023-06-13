# Comparing `tmp/lamini-0.0.17a2.tar.gz` & `tmp/lamini-0.0.17a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamini-0.0.17a2.tar", last modified: Wed Jun  7 06:54:45 2023, max compression
+gzip compressed data, was "lamini-0.0.17a3.tar", last modified: Wed Jun  7 08:59:57 2023, max compression
```

## Comparing `lamini-0.0.17a2.tar` & `lamini-0.0.17a3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 06:54:45.293827 lamini-0.0.17a2/
--rw-r--r--   0 jonathanli   (501) staff       (20)    11340 2023-03-02 20:01:20.000000 lamini-0.0.17a2/LICENSE
--rw-r--r--   0 jonathanli   (501) staff       (20)    13356 2023-06-07 06:54:45.293418 lamini-0.0.17a2/PKG-INFO
--rw-r--r--   0 jonathanli   (501) staff       (20)    12972 2023-05-23 00:37:01.000000 lamini-0.0.17a2/README.md
-drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 06:54:45.277663 lamini-0.0.17a2/lamini.egg-info/
--rw-r--r--   0 jonathanli   (501) staff       (20)    13356 2023-06-07 06:54:45.000000 lamini-0.0.17a2/lamini.egg-info/PKG-INFO
--rw-r--r--   0 jonathanli   (501) staff       (20)     1833 2023-06-07 06:54:45.000000 lamini-0.0.17a2/lamini.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanli   (501) staff       (20)        1 2023-06-07 06:54:45.000000 lamini-0.0.17a2/lamini.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanli   (501) staff       (20)       80 2023-06-07 06:54:45.000000 lamini-0.0.17a2/lamini.egg-info/requires.txt
--rw-r--r--   0 jonathanli   (501) staff       (20)        6 2023-06-07 06:54:45.000000 lamini-0.0.17a2/lamini.egg-info/top_level.txt
-drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 06:54:45.277780 lamini-0.0.17a2/llama/
--rw-r--r--   0 jonathanli   (501) staff       (20)      465 2023-05-31 16:59:44.000000 lamini-0.0.17a2/llama/__init__.py
-drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 06:54:45.278021 lamini-0.0.17a2/llama/error/
--rw-r--r--   0 jonathanli   (501) staff       (20)      274 2023-03-29 05:59:59.000000 lamini-0.0.17a2/llama/error/error.py
-drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 06:54:45.278504 lamini-0.0.17a2/llama/metrics/
--rw-r--r--   0 jonathanli   (501) staff       (20)      616 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/metrics/compare_equal_metric.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      104 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/metrics/metric.py
-drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 06:54:45.279287 lamini-0.0.17a2/llama/program/
--rw-r--r--   0 jonathanli   (501) staff       (20)    11110 2023-06-07 06:35:26.000000 lamini-0.0.17a2/llama/program/builder.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      765 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/program/function.py
-drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 06:54:45.281022 lamini-0.0.17a2/llama/program/operations/
--rw-r--r--   0 jonathanli   (501) staff       (20)      737 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/program/operations/batch_llama_operation.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     1028 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/program/operations/call_operation.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     1218 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/program/operations/feedback_operation.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      505 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/program/operations/get_argument_operation.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      618 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/program/operations/get_element_operation.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      632 2023-03-24 08:23:54.000000 lamini-0.0.17a2/llama/program/operations/get_field_operation.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      615 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/program/operations/llama_operation.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      514 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/program/operations/metric_operation.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      755 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/program/operations/return_operation.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      286 2023-05-29 17:46:08.000000 lamini-0.0.17a2/llama/program/operations/train_operation.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     1516 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/program/program.py
-drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 06:54:45.281898 lamini-0.0.17a2/llama/program/util/
--rw-r--r--   0 jonathanli   (501) staff       (20)     3336 2023-06-07 06:35:26.000000 lamini-0.0.17a2/llama/program/util/api_actions.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     1105 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/program/util/config.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     3893 2023-05-31 16:59:44.000000 lamini-0.0.17a2/llama/program/util/run_ai.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     1121 2023-03-04 02:28:32.000000 lamini-0.0.17a2/llama/program/util/type_to_dict.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     2656 2023-05-31 16:59:44.000000 lamini-0.0.17a2/llama/program/value.py
-drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 06:54:45.282622 lamini-0.0.17a2/llama/tools/
--rw-r--r--   0 jonathanli   (501) staff       (20)     2669 2023-05-22 21:09:27.000000 lamini-0.0.17a2/llama/tools/balancer.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      205 2023-05-18 21:29:25.000000 lamini-0.0.17a2/llama/tools/embedding.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      215 2023-05-22 21:09:27.000000 lamini-0.0.17a2/llama/tools/json_to_object.py
-drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 06:54:45.283249 lamini-0.0.17a2/llama/types/
--rw-r--r--   0 jonathanli   (501) staff       (20)     2293 2023-06-06 04:49:09.000000 lamini-0.0.17a2/llama/types/base_specification.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      178 2023-03-02 20:01:20.000000 lamini-0.0.17a2/llama/types/context.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     1707 2023-05-15 20:27:06.000000 lamini-0.0.17a2/llama/types/type.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      861 2023-06-07 06:54:36.000000 lamini-0.0.17a2/pyproject.toml
--rw-r--r--   0 jonathanli   (501) staff       (20)       38 2023-06-07 06:54:45.293877 lamini-0.0.17a2/setup.cfg
-drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 06:54:45.293151 lamini-0.0.17a2/tests/
--rw-r--r--   0 jonathanli   (501) staff       (20)     2201 2023-06-02 05:14:33.000000 lamini-0.0.17a2/tests/test_add_data.py
--rw-r--r--   0 jonathanli   (501) staff       (20)    20676 2023-06-02 05:14:33.000000 lamini-0.0.17a2/tests/test_batch_operation.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      505 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_chat_gpt.py
--rw-r--r--   0 jonathanli   (501) staff       (20)    82798 2023-06-02 05:14:33.000000 lamini-0.0.17a2/tests/test_chunking.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     2419 2023-06-02 04:27:45.000000 lamini-0.0.17a2/tests/test_complex_types.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     3256 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_config.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      550 2023-05-15 20:27:06.000000 lamini-0.0.17a2/tests/test_embedding.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      972 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_error.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     3236 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_feedback.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      483 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_gpt4.py
--rw-r--r--   0 jonathanli   (501) staff       (20)    13613 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_improve_remove_numbers.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      801 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_infer_context.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     1492 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_multiple_models.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     2756 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_multiple_models_add_data.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      637 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_output_list.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      947 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_output_str.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     4464 2023-05-31 16:59:44.000000 lamini-0.0.17a2/tests/test_parallel_values.py
--rw-r--r--   0 jonathanli   (501) staff       (20)    12478 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_parse_field_output.py
--rw-r--r--   0 jonathanli   (501) staff       (20)    22637 2023-06-06 22:18:02.000000 lamini-0.0.17a2/tests/test_queue_program.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     1158 2023-06-02 04:17:41.000000 lamini-0.0.17a2/tests/test_random.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     4472 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_rlhf.py
--rw-r--r--   0 jonathanli   (501) staff       (20)    12552 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_sample.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      542 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_spec_context.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     1134 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_stop_token.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     2560 2023-06-07 06:35:26.000000 lamini-0.0.17a2/tests/test_train.py
--rw-r--r--   0 jonathanli   (501) staff       (20)     1141 2023-05-31 16:59:44.000000 lamini-0.0.17a2/tests/test_unblocked_prompt.py
--rw-r--r--   0 jonathanli   (501) staff       (20)      844 2023-05-23 00:37:01.000000 lamini-0.0.17a2/tests/test_unpaired_data.py
+drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 08:59:57.549884 lamini-0.0.17a3/
+-rw-r--r--   0 jonathanli   (501) staff       (20)    11340 2023-03-02 20:01:20.000000 lamini-0.0.17a3/LICENSE
+-rw-r--r--   0 jonathanli   (501) staff       (20)    13356 2023-06-07 08:59:57.549661 lamini-0.0.17a3/PKG-INFO
+-rw-r--r--   0 jonathanli   (501) staff       (20)    12972 2023-05-23 00:37:01.000000 lamini-0.0.17a3/README.md
+drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 08:59:57.530625 lamini-0.0.17a3/lamini.egg-info/
+-rw-r--r--   0 jonathanli   (501) staff       (20)    13356 2023-06-07 08:59:57.000000 lamini-0.0.17a3/lamini.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanli   (501) staff       (20)     1833 2023-06-07 08:59:57.000000 lamini-0.0.17a3/lamini.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanli   (501) staff       (20)        1 2023-06-07 08:59:57.000000 lamini-0.0.17a3/lamini.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanli   (501) staff       (20)       80 2023-06-07 08:59:57.000000 lamini-0.0.17a3/lamini.egg-info/requires.txt
+-rw-r--r--   0 jonathanli   (501) staff       (20)        6 2023-06-07 08:59:57.000000 lamini-0.0.17a3/lamini.egg-info/top_level.txt
+drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 08:59:57.530765 lamini-0.0.17a3/llama/
+-rw-r--r--   0 jonathanli   (501) staff       (20)      465 2023-05-31 16:59:44.000000 lamini-0.0.17a3/llama/__init__.py
+drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 08:59:57.531009 lamini-0.0.17a3/llama/error/
+-rw-r--r--   0 jonathanli   (501) staff       (20)      274 2023-03-29 05:59:59.000000 lamini-0.0.17a3/llama/error/error.py
+drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 08:59:57.531701 lamini-0.0.17a3/llama/metrics/
+-rw-r--r--   0 jonathanli   (501) staff       (20)      616 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/metrics/compare_equal_metric.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      104 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/metrics/metric.py
+drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 08:59:57.532633 lamini-0.0.17a3/llama/program/
+-rw-r--r--   0 jonathanli   (501) staff       (20)    11260 2023-06-07 08:57:23.000000 lamini-0.0.17a3/llama/program/builder.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      765 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/program/function.py
+drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 08:59:57.534456 lamini-0.0.17a3/llama/program/operations/
+-rw-r--r--   0 jonathanli   (501) staff       (20)      737 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/program/operations/batch_llama_operation.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     1028 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/program/operations/call_operation.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     1218 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/program/operations/feedback_operation.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      505 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/program/operations/get_argument_operation.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      618 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/program/operations/get_element_operation.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      632 2023-03-24 08:23:54.000000 lamini-0.0.17a3/llama/program/operations/get_field_operation.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      615 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/program/operations/llama_operation.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      514 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/program/operations/metric_operation.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      755 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/program/operations/return_operation.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      286 2023-05-29 17:46:08.000000 lamini-0.0.17a3/llama/program/operations/train_operation.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     1516 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/program/program.py
+drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 08:59:57.535341 lamini-0.0.17a3/llama/program/util/
+-rw-r--r--   0 jonathanli   (501) staff       (20)     3336 2023-06-07 06:35:26.000000 lamini-0.0.17a3/llama/program/util/api_actions.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     1105 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/program/util/config.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     3893 2023-05-31 16:59:44.000000 lamini-0.0.17a3/llama/program/util/run_ai.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     1121 2023-03-04 02:28:32.000000 lamini-0.0.17a3/llama/program/util/type_to_dict.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     2656 2023-05-31 16:59:44.000000 lamini-0.0.17a3/llama/program/value.py
+drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 08:59:57.542141 lamini-0.0.17a3/llama/tools/
+-rw-r--r--   0 jonathanli   (501) staff       (20)     2669 2023-05-22 21:09:27.000000 lamini-0.0.17a3/llama/tools/balancer.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      205 2023-05-18 21:29:25.000000 lamini-0.0.17a3/llama/tools/embedding.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      215 2023-05-22 21:09:27.000000 lamini-0.0.17a3/llama/tools/json_to_object.py
+drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 08:59:57.543191 lamini-0.0.17a3/llama/types/
+-rw-r--r--   0 jonathanli   (501) staff       (20)     2293 2023-06-06 04:49:09.000000 lamini-0.0.17a3/llama/types/base_specification.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      178 2023-03-02 20:01:20.000000 lamini-0.0.17a3/llama/types/context.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     1707 2023-05-15 20:27:06.000000 lamini-0.0.17a3/llama/types/type.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      861 2023-06-07 08:59:53.000000 lamini-0.0.17a3/pyproject.toml
+-rw-r--r--   0 jonathanli   (501) staff       (20)       38 2023-06-07 08:59:57.549930 lamini-0.0.17a3/setup.cfg
+drwxr-xr-x   0 jonathanli   (501) staff       (20)        0 2023-06-07 08:59:57.549434 lamini-0.0.17a3/tests/
+-rw-r--r--   0 jonathanli   (501) staff       (20)     2201 2023-06-02 05:14:33.000000 lamini-0.0.17a3/tests/test_add_data.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)    20676 2023-06-02 05:14:33.000000 lamini-0.0.17a3/tests/test_batch_operation.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      505 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_chat_gpt.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)    82798 2023-06-02 05:14:33.000000 lamini-0.0.17a3/tests/test_chunking.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     2419 2023-06-02 04:27:45.000000 lamini-0.0.17a3/tests/test_complex_types.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     3256 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_config.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      550 2023-05-15 20:27:06.000000 lamini-0.0.17a3/tests/test_embedding.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      972 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_error.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     3236 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_feedback.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      483 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_gpt4.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)    13613 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_improve_remove_numbers.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      801 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_infer_context.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     1492 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_multiple_models.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     2756 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_multiple_models_add_data.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      637 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_output_list.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      947 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_output_str.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     4464 2023-05-31 16:59:44.000000 lamini-0.0.17a3/tests/test_parallel_values.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)    12478 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_parse_field_output.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)    22637 2023-06-06 22:18:02.000000 lamini-0.0.17a3/tests/test_queue_program.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     1158 2023-06-02 04:17:41.000000 lamini-0.0.17a3/tests/test_random.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     4472 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_rlhf.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)    12552 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_sample.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      542 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_spec_context.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     1134 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_stop_token.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     2560 2023-06-07 06:35:26.000000 lamini-0.0.17a3/tests/test_train.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)     1141 2023-05-31 16:59:44.000000 lamini-0.0.17a3/tests/test_unblocked_prompt.py
+-rw-r--r--   0 jonathanli   (501) staff       (20)      844 2023-05-23 00:37:01.000000 lamini-0.0.17a3/tests/test_unpaired_data.py
```

### Comparing `lamini-0.0.17a2/LICENSE` & `lamini-0.0.17a3/LICENSE`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/PKG-INFO` & `lamini-0.0.17a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamini
-Version: 0.0.17a2
+Version: 0.0.17a3
 Summary: Build on large language models faster
 Author-email: PowerML <info@powerml.co>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `lamini-0.0.17a2/README.md` & `lamini-0.0.17a3/README.md`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/lamini.egg-info/PKG-INFO` & `lamini-0.0.17a3/lamini.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamini
-Version: 0.0.17a2
+Version: 0.0.17a3
 Summary: Build on large language models faster
 Author-email: PowerML <info@powerml.co>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `lamini-0.0.17a2/lamini.egg-info/SOURCES.txt` & `lamini-0.0.17a3/lamini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/metrics/compare_equal_metric.py` & `lamini-0.0.17a3/llama/metrics/compare_equal_metric.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/builder.py` & `lamini-0.0.17a3/llama/program/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         else:
             new_input = [input]
             values = self.add_model(new_input, output_type, *args, **kwargs)
             results = gen_queue_batch(values)
             return results
 
     def submit_training_job(self, data=[]):
-        self.add_data(data)
+        self.save_data(data)
         value = self.current_function.add_operation(TrainOperation())
         results = gen_submit_training_job(value, self.id, self.model_name)
         return results
 
     def check_job_status(self, job_id):
         status = gen_check_job_status(job_id)
         return status
@@ -193,15 +193,21 @@
                     )
                 )
                 new_operation = gen_value(new_operation)
             new_operations.append(new_operation)
 
         return new_operations
 
+    def set_data(self, data: List):
+        self.program.add_data(examples=data)
+
     def add_data(self, data: List):
+        self.save_data(data)
+
+    def save_data(self, data: List):
         self.program.add_data(examples=data)
         results = gen_submit_data(self.program, self.id)
         return results
 
     def improve(
         self,
         on: str,
```

### Comparing `lamini-0.0.17a2/llama/program/function.py` & `lamini-0.0.17a3/llama/program/function.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/operations/batch_llama_operation.py` & `lamini-0.0.17a3/llama/program/operations/batch_llama_operation.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/operations/call_operation.py` & `lamini-0.0.17a3/llama/program/operations/call_operation.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/operations/feedback_operation.py` & `lamini-0.0.17a3/llama/program/operations/feedback_operation.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/operations/get_element_operation.py` & `lamini-0.0.17a3/llama/program/operations/get_element_operation.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/operations/get_field_operation.py` & `lamini-0.0.17a3/llama/program/operations/get_field_operation.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/operations/llama_operation.py` & `lamini-0.0.17a3/llama/program/operations/llama_operation.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/operations/metric_operation.py` & `lamini-0.0.17a3/llama/program/operations/metric_operation.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/operations/return_operation.py` & `lamini-0.0.17a3/llama/program/operations/return_operation.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/program.py` & `lamini-0.0.17a3/llama/program/program.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/util/api_actions.py` & `lamini-0.0.17a3/llama/program/util/api_actions.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/util/config.py` & `lamini-0.0.17a3/llama/program/util/config.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/util/run_ai.py` & `lamini-0.0.17a3/llama/program/util/run_ai.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/util/type_to_dict.py` & `lamini-0.0.17a3/llama/program/util/type_to_dict.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/program/value.py` & `lamini-0.0.17a3/llama/program/value.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/tools/balancer.py` & `lamini-0.0.17a3/llama/tools/balancer.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/types/base_specification.py` & `lamini-0.0.17a3/llama/types/base_specification.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/llama/types/type.py` & `lamini-0.0.17a3/llama/types/type.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/pyproject.toml` & `lamini-0.0.17a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lamini"
-version = "0.0.17a2"
+version = "0.0.17a3"
 authors = [
   { name="PowerML", email="info@powerml.co" },
 ]
 description = "Build on large language models faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lamini-0.0.17a2/tests/test_add_data.py` & `lamini-0.0.17a3/tests/test_add_data.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_batch_operation.py` & `lamini-0.0.17a3/tests/test_batch_operation.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_chunking.py` & `lamini-0.0.17a3/tests/test_chunking.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_complex_types.py` & `lamini-0.0.17a3/tests/test_complex_types.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_config.py` & `lamini-0.0.17a3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_embedding.py` & `lamini-0.0.17a3/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_error.py` & `lamini-0.0.17a3/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_feedback.py` & `lamini-0.0.17a3/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_improve_remove_numbers.py` & `lamini-0.0.17a3/tests/test_improve_remove_numbers.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_infer_context.py` & `lamini-0.0.17a3/tests/test_infer_context.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_multiple_models.py` & `lamini-0.0.17a3/tests/test_multiple_models.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_multiple_models_add_data.py` & `lamini-0.0.17a3/tests/test_multiple_models_add_data.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_output_list.py` & `lamini-0.0.17a3/tests/test_output_list.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_output_str.py` & `lamini-0.0.17a3/tests/test_output_str.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_parallel_values.py` & `lamini-0.0.17a3/tests/test_parallel_values.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_parse_field_output.py` & `lamini-0.0.17a3/tests/test_parse_field_output.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_queue_program.py` & `lamini-0.0.17a3/tests/test_queue_program.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_random.py` & `lamini-0.0.17a3/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_rlhf.py` & `lamini-0.0.17a3/tests/test_rlhf.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_sample.py` & `lamini-0.0.17a3/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_spec_context.py` & `lamini-0.0.17a3/tests/test_spec_context.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_stop_token.py` & `lamini-0.0.17a3/tests/test_stop_token.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_train.py` & `lamini-0.0.17a3/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_unblocked_prompt.py` & `lamini-0.0.17a3/tests/test_unblocked_prompt.py`

 * *Files identical despite different names*

### Comparing `lamini-0.0.17a2/tests/test_unpaired_data.py` & `lamini-0.0.17a3/tests/test_unpaired_data.py`

 * *Files identical despite different names*

