# Comparing `tmp/giskard-2.0.0b6.tar.gz` & `tmp/giskard-2.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giskard-2.0.0b6.tar", last modified: Mon Jun 12 17:18:25 2023, max compression
+gzip compressed data, was "giskard-2.0.0b7.tar", last modified: Tue Jun 13 12:29:40 2023, max compression
```

## Comparing `giskard-2.0.0b6.tar` & `giskard-2.0.0b7.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.227971 giskard-2.0.0b6/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-12 17:18:25.228067 giskard-2.0.0b6/PKG-INFO
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     8643 2023-06-12 14:14:57.000000 giskard-2.0.0b6/README.md
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.197521 giskard-2.0.0b6/giskard/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1836 2023-06-12 16:43:55.000000 giskard-2.0.0b6/giskard/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/cli.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/cli_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.199303 giskard-2.0.0b6/giskard/client/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/client/dtos.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11444 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/client/giskard_client.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/client/io_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3620 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/client/project.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-06 13:35:03.000000 giskard-2.0.0b6/giskard/client/python_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.199886 giskard-2.0.0b6/giskard/commands/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15997 2023-06-12 16:24:17.000000 giskard-2.0.0b6/giskard/commands/cli_server.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7206 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/commands/cli_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.201028 giskard-2.0.0b6/giskard/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/core/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11799 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/core/core.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/core/dataset_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      890 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/core/errors.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13215 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/core/model_validation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15807 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/core/suite.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      574 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/core/validation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.201186 giskard-2.0.0b6/giskard/datasets/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2711 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/datasets/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.201341 giskard-2.0.0b6/giskard/datasets/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26225 2023-06-12 16:43:48.000000 giskard-2.0.0b6/giskard/datasets/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.202617 giskard-2.0.0b6/giskard/datasets/metadata/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/datasets/metadata/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/datasets/metadata/indexing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/datasets/metadata/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/datasets/metadata/text_metadata_provider.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.202990 giskard-2.0.0b6/giskard/demo/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3059 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/demo/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/demo/titanic.csv
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.203603 giskard-2.0.0b6/giskard/ml_worker/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.204477 giskard-2.0.0b6/giskard/ml_worker/bridge/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/ml_worker/bridge/data_encryptor.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/bridge/error.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/bridge/ml_worker_bridge.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/ml_worker/bridge/service_messages.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.204837 giskard-2.0.0b6/giskard/ml_worker/core/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/core/log_listener.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5858 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/core/savable.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.205360 giskard-2.0.0b6/giskard/ml_worker/exceptions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/exceptions/IllegalArgumentError.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/exceptions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/exceptions/giskard_exception.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.205717 giskard-2.0.0b6/giskard/ml_worker/generated/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard/ml_worker/generated/ml_worker_pb2.py
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3226 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/ml_worker.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.205982 giskard-2.0.0b6/giskard/ml_worker/server/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/server/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26425 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/server/ml_worker_service.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.206906 giskard-2.0.0b6/giskard/ml_worker/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b6/giskard/ml_worker/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.207517 giskard-2.0.0b6/giskard/ml_worker/testing/functions/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      170 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/functions/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3927 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/functions/slicing.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6602 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/functions/transformation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.208655 giskard-2.0.0b6/giskard/ml_worker/testing/registry/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1799 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2317 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/decorators_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/giskard_test.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6374 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/slicing_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5439 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/transformation_function.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1783 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/registry/udf_repository.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/ml_worker/testing/stat_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2649 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/test_result.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2036 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/testing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.209397 giskard-2.0.0b6/giskard/ml_worker/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b6/giskard/ml_worker/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/ml_worker/utils/file_utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/ml_worker/utils/logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1952 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/utils/network.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2514 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/ml_worker/utils/request_interceptor.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.209915 giskard-2.0.0b6/giskard/models/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2207 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/_precooked.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.210047 giskard-2.0.0b6/giskard/models/automodel/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9234 2023-06-12 16:43:52.000000 giskard-2.0.0b6/giskard/models/automodel/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.210260 giskard-2.0.0b6/giskard/models/base/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34331 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/base/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.210585 giskard-2.0.0b6/giskard/models/cache/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/cache/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/cache/cache.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.210714 giskard-2.0.0b6/giskard/models/catboost/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/catboost/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.210953 giskard-2.0.0b6/giskard/models/function/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/function/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.211080 giskard-2.0.0b6/giskard/models/huggingface/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5872 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/huggingface/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.211211 giskard-2.0.0b6/giskard/models/langchain/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2619 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/langchain/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6342 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/model_explanation.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.211339 giskard-2.0.0b6/giskard/models/pytorch/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7205 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/pytorch/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.211472 giskard-2.0.0b6/giskard/models/sklearn/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4321 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/models/sklearn/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.211599 giskard-2.0.0b6/giskard/models/tensorflow/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1656 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/tensorflow/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      844 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/models/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/path_utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.212712 giskard-2.0.0b6/giskard/scanner/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.213295 giskard-2.0.0b6/giskard/scanner/calibration/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/calibration/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/calibration/overconfidence_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/calibration/underconfidence_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.213547 giskard-2.0.0b6/giskard/scanner/common/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/common/examples.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/common/loss_based_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.213683 giskard-2.0.0b6/giskard/scanner/data_leakage/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/data_leakage/data_leakage_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/decorators.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/issues.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.213978 giskard-2.0.0b6/giskard/scanner/llm/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/llm/toxicity_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/llm/utils.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/logger.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.214587 giskard-2.0.0b6/giskard/scanner/performance/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/performance/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/performance/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/performance/metrics.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/performance/performance_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/registry.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3882 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/scanner/result.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.216854 giskard-2.0.0b6/giskard/scanner/robustness/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/robustness/base_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/scanner/robustness/entity_swap.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      953 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/scanner/robustness/ethical_bias_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/robustness/issues.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/robustness/nationalities.json
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1006 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/scanner/robustness/text_perturbation_detector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11955 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/scanner/robustness/text_transformations.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/scanner.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.217063 giskard-2.0.0b6/giskard/scanner/stochasticity/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/stochasticity/stochasticity_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.218262 giskard-2.0.0b6/giskard/scanner/templates/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      767 2023-06-12 14:14:57.000000 giskard-2.0.0b6/giskard/scanner/templates/_code_snippet.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.219360 giskard-2.0.0b6/giskard/scanner/templates/_issues/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/data_leakage.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/default.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/llm_toxicity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/overconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/performance.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/robustness.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/stochasticity.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues/underconfidence.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_issues_table.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_main_content.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/_tab_header.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      214 2023-06-12 11:29:06.000000 giskard-2.0.0b6/giskard/scanner/templates/base.html
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/scan_results.html
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.219990 giskard-2.0.0b6/giskard/scanner/templates/static/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/templates/static/external.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/templates/static/internal.js
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/templates/static/style.css
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.220442 giskard-2.0.0b6/giskard/scanner/visualization/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/scanner/visualization/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/scanner/visualization/custom_jinja.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/settings.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.222370 giskard-2.0.0b6/giskard/slicing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/base.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/bruteforce_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/category_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/multiscale_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/opt_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10534 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/slicing/slice.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15389 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/slicing/stop_words.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/slicing/text_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/slicing/tree_slicer.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/slicing/utils.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.222600 giskard-2.0.0b6/giskard/testing/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/testing/__init__.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.223472 giskard-2.0.0b6/giskard/testing/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b6/giskard/testing/tests/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33167 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/testing/tests/drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30208 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/testing/tests/metamorphic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25823 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/testing/tests/performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10370 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/testing/tests/statistic.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.224172 giskard-2.0.0b6/giskard/utils/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-12 07:28:20.000000 giskard-2.0.0b6/giskard/utils/__init__.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7152 2023-06-12 16:45:35.000000 giskard-2.0.0b6/giskard/utils/analytics_collector.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/utils/display.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-09 09:22:23.000000 giskard-2.0.0b6/giskard/utils/environment_detector.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.198359 giskard-2.0.0b6/giskard.egg-info/
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard.egg-info/PKG-INFO
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard.egg-info/SOURCES.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard.egg-info/dependency_links.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard.egg-info/entry_points.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      602 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard.egg-info/requires.txt
--rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       27 2023-06-12 17:18:25.000000 giskard-2.0.0b6/giskard.egg-info/top_level.txt
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7425 2023-06-12 16:48:36.000000 giskard-2.0.0b6/pyproject.toml
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-12 17:18:25.228306 giskard-2.0.0b6/setup.cfg
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-07 15:34:18.000000 giskard-2.0.0b6/setup.py
-drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-12 17:18:25.227763 giskard-2.0.0b6/tests/
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1513 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_custom_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15828 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_data_drift.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6395 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_data_processing_pipeline.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_dataset.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b6/tests/test_logging.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11293 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_metamorphic_direction.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10279 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_metamorphic_invariance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2409 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_model.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2148 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_model_auto_inference.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-07 15:34:18.000000 giskard-2.0.0b6/tests/test_model_explanation.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-07 15:34:18.000000 giskard-2.0.0b6/tests/test_model_postprocess.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_performance.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4572 2023-06-12 16:46:51.000000 giskard-2.0.0b6/tests/test_programmatic.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4283 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_project_uploads.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4554 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_statistical.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4570 2023-06-12 07:28:20.000000 giskard-2.0.0b6/tests/test_upload.py
--rw-r--r--   0 andreyavtomonov   (501) staff       (20)      450 2023-06-12 11:29:06.000000 giskard-2.0.0b6/tests/test_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.360038 giskard-2.0.0b7/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-13 12:29:40.360178 giskard-2.0.0b7/PKG-INFO
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     8643 2023-06-12 14:14:57.000000 giskard-2.0.0b7/README.md
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.300116 giskard-2.0.0b7/giskard/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1836 2023-06-12 16:43:55.000000 giskard-2.0.0b7/giskard/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      704 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/cli.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3388 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/cli_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.303788 giskard-2.0.0b7/giskard/client/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      420 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/client/dtos.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11444 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/client/giskard_client.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2136 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/client/io_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3620 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/client/project.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      673 2023-06-06 13:35:03.000000 giskard-2.0.0b7/giskard/client/python_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.304799 giskard-2.0.0b7/giskard/commands/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    16407 2023-06-13 10:37:18.000000 giskard-2.0.0b7/giskard/commands/cli_server.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7604 2023-06-13 10:46:54.000000 giskard-2.0.0b7/giskard/commands/cli_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.306163 giskard-2.0.0b7/giskard/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/core/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11799 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/core/core.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6466 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/core/dataset_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      890 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/core/errors.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    13215 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/core/model_validation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15807 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/core/suite.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      574 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/core/validation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.306341 giskard-2.0.0b7/giskard/datasets/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2711 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/datasets/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.306515 giskard-2.0.0b7/giskard/datasets/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26225 2023-06-12 16:43:48.000000 giskard-2.0.0b7/giskard/datasets/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.308000 giskard-2.0.0b7/giskard/datasets/metadata/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      206 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/datasets/metadata/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3431 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/datasets/metadata/indexing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      788 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/datasets/metadata/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1851 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/datasets/metadata/text_metadata_provider.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.308469 giskard-2.0.0b7/giskard/demo/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3059 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/demo/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    60302 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/demo/titanic.csv
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.309093 giskard-2.0.0b7/giskard/ml_worker/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.310097 giskard-2.0.0b7/giskard/ml_worker/bridge/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1406 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/ml_worker/bridge/data_encryptor.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       42 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/bridge/error.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9252 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/bridge/ml_worker_bridge.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       62 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/ml_worker/bridge/service_messages.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.310688 giskard-2.0.0b7/giskard/ml_worker/core/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1012 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/core/log_listener.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5858 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/core/savable.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.312751 giskard-2.0.0b7/giskard/ml_worker/exceptions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      375 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/exceptions/IllegalArgumentError.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/exceptions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      114 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/exceptions/giskard_exception.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.314684 giskard-2.0.0b7/giskard/ml_worker/generated/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    51492 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard/ml_worker/generated/ml_worker_pb2.py
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)    21397 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard/ml_worker/generated/ml_worker_pb2_grpc.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3226 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/ml_worker.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.314933 giskard-2.0.0b7/giskard/ml_worker/server/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/server/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    26425 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/server/ml_worker_service.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.316847 giskard-2.0.0b7/giskard/ml_worker/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-05-25 10:01:00.000000 giskard-2.0.0b7/giskard/ml_worker/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.317676 giskard-2.0.0b7/giskard/ml_worker/testing/functions/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      170 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/functions/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3927 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/functions/slicing.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6602 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/functions/transformation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.319193 giskard-2.0.0b7/giskard/ml_worker/testing/registry/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1799 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2317 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/decorators_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4703 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/giskard_test.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3943 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6374 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/slicing_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5439 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/transformation_function.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1783 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/registry/udf_repository.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4675 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/ml_worker/testing/stat_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2649 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/test_result.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2036 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/testing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.320178 giskard-2.0.0b7/giskard/ml_worker/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-04-12 00:50:05.000000 giskard-2.0.0b7/giskard/ml_worker/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      137 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/ml_worker/utils/file_utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2297 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/ml_worker/utils/logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1952 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/utils/network.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2514 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/ml_worker/utils/request_interceptor.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.321052 giskard-2.0.0b7/giskard/models/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15755 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2207 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/_precooked.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.321262 giskard-2.0.0b7/giskard/models/automodel/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     9234 2023-06-12 16:43:52.000000 giskard-2.0.0b7/giskard/models/automodel/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.321613 giskard-2.0.0b7/giskard/models/base/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    34331 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/base/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.322415 giskard-2.0.0b7/giskard/models/cache/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      803 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/cache/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2706 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/cache/cache.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.322608 giskard-2.0.0b7/giskard/models/catboost/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      698 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/catboost/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.322955 giskard-2.0.0b7/giskard/models/function/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1202 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/function/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.323120 giskard-2.0.0b7/giskard/models/huggingface/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5872 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/huggingface/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.323338 giskard-2.0.0b7/giskard/models/langchain/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2619 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/langchain/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6342 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/model_explanation.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.323533 giskard-2.0.0b7/giskard/models/pytorch/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7205 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/pytorch/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.323760 giskard-2.0.0b7/giskard/models/sklearn/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4321 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/models/sklearn/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.323995 giskard-2.0.0b7/giskard/models/tensorflow/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1656 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/tensorflow/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      844 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/models/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      528 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/path_utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.325545 giskard-2.0.0b7/giskard/scanner/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1595 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.326352 giskard-2.0.0b7/giskard/scanner/calibration/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3475 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/calibration/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3894 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/calibration/overconfidence_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3708 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/calibration/underconfidence_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.326781 giskard-2.0.0b7/giskard/scanner/common/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2568 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/common/examples.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4788 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/common/loss_based_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.326971 giskard-2.0.0b7/giskard/scanner/data_leakage/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2702 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/data_leakage/data_leakage_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      617 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/decorators.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1396 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/issues.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.327331 giskard-2.0.0b7/giskard/scanner/llm/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     5929 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/llm/toxicity_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      627 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/llm/utils.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       84 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/logger.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.328429 giskard-2.0.0b7/giskard/scanner/performance/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      159 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/performance/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4218 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/performance/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4638 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/performance/metrics.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6651 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/performance/performance_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      941 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/registry.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3882 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/scanner/result.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.331893 giskard-2.0.0b7/giskard/scanner/robustness/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6379 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/robustness/base_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)   455659 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/scanner/robustness/entity_swap.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      953 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/scanner/robustness/ethical_bias_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3322 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/robustness/issues.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19432 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/robustness/nationalities.json
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1006 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/scanner/robustness/text_perturbation_detector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11955 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/scanner/robustness/text_transformations.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7997 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/scanner.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.334034 giskard-2.0.0b7/giskard/scanner/stochasticity/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2237 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/stochasticity/stochasticity_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.335814 giskard-2.0.0b7/giskard/scanner/templates/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      767 2023-06-12 14:14:57.000000 giskard-2.0.0b7/giskard/scanner/templates/_code_snippet.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.337559 giskard-2.0.0b7/giskard/scanner/templates/_issues/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1475 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/data_leakage.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1653 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/default.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1501 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/llm_toxicity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2155 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/overconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2128 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/performance.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2020 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/robustness.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1468 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/stochasticity.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2144 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues/underconfidence.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1261 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_issues_table.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6806 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_main_content.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2862 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/_tab_header.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      214 2023-06-12 11:29:06.000000 giskard-2.0.0b7/giskard/scanner/templates/base.html
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      555 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/scan_results.html
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.338397 giskard-2.0.0b7/giskard/scanner/templates/static/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    19904 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/templates/static/external.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    65083 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/templates/static/internal.js
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    12690 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/templates/static/style.css
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.338826 giskard-2.0.0b7/giskard/scanner/visualization/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/scanner/visualization/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      820 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/scanner/visualization/custom_jinja.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      902 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/settings.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.341185 giskard-2.0.0b7/giskard/slicing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       82 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      707 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/base.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1300 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/bruteforce_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      615 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/category_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3174 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/multiscale_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1868 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/opt_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10534 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/slicing/slice.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15389 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/slicing/stop_words.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7652 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/slicing/text_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3460 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/slicing/tree_slicer.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1311 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/slicing/utils.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.341441 giskard-2.0.0b7/giskard/testing/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2085 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/testing/__init__.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.342521 giskard-2.0.0b7/giskard/testing/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)        0 2023-06-07 15:34:18.000000 giskard-2.0.0b7/giskard/testing/tests/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    33167 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/testing/tests/drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    30208 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/testing/tests/metamorphic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    25823 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/testing/tests/performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10370 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/testing/tests/statistic.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.344126 giskard-2.0.0b7/giskard/utils/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      385 2023-06-12 07:28:20.000000 giskard-2.0.0b7/giskard/utils/__init__.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7144 2023-06-13 11:00:17.000000 giskard-2.0.0b7/giskard/utils/analytics_collector.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      293 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/utils/display.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4919 2023-06-09 09:22:23.000000 giskard-2.0.0b7/giskard/utils/environment_detector.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.301257 giskard-2.0.0b7/giskard.egg-info/
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     9958 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard.egg-info/PKG-INFO
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)     6171 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard.egg-info/SOURCES.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)        1 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard.egg-info/dependency_links.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       44 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard.egg-info/entry_points.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)      602 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard.egg-info/requires.txt
+-rw-rw-rw-   0 andreyavtomonov   (501) staff       (20)       27 2023-06-13 12:29:40.000000 giskard-2.0.0b7/giskard.egg-info/top_level.txt
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     7425 2023-06-13 11:07:01.000000 giskard-2.0.0b7/pyproject.toml
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)       93 2023-06-13 12:29:40.360501 giskard-2.0.0b7/setup.cfg
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2281 2023-06-07 15:34:18.000000 giskard-2.0.0b7/setup.py
+drwxr-xr-x   0 andreyavtomonov   (501) staff       (20)        0 2023-06-13 12:29:40.359800 giskard-2.0.0b7/tests/
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     1513 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_custom_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    15828 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_data_drift.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     6395 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_data_processing_pipeline.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4533 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_dataset.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      199 2023-04-12 00:50:05.000000 giskard-2.0.0b7/tests/test_logging.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    11293 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_metamorphic_direction.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    10279 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_metamorphic_invariance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2409 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_model.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2148 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_model_auto_inference.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     2526 2023-06-07 15:34:18.000000 giskard-2.0.0b7/tests/test_model_explanation.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     3791 2023-06-07 15:34:18.000000 giskard-2.0.0b7/tests/test_model_postprocess.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)    14080 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_performance.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4572 2023-06-12 16:46:51.000000 giskard-2.0.0b7/tests/test_programmatic.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4283 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_project_uploads.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4554 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_statistical.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)     4570 2023-06-12 07:28:20.000000 giskard-2.0.0b7/tests/test_upload.py
+-rw-r--r--   0 andreyavtomonov   (501) staff       (20)      450 2023-06-12 11:29:06.000000 giskard-2.0.0b7/tests/test_utils.py
```

### Comparing `giskard-2.0.0b6/PKG-INFO` & `giskard-2.0.0b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.0.0b6
+Version: 2.0.0b7
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: giskard Version: 2.0.0b6 Summary: The testing
+Metadata-Version: 2.1 Name: giskard Version: 2.0.0b7 Summary: The testing
 framework dedicated to ML models, from tabular to LLMs Author-email: Giskard AI
 giskard.ai> License: Apache Software License 2.0 Project-URL: Homepage, https:/
 /giskard.ai Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues Project-
 URL: Documentation, https://docs.giskard.ai/ Project-URL: Discord, https://
 discord.gg/ABvfpbu69R Project-URL: Linkedin, https://www.linkedin.com/company/
 giskard-ai Project-URL: Mastodon, https://fosstodon.org/@Giskard Project-URL:
```

### Comparing `giskard-2.0.0b6/README.md` & `giskard-2.0.0b7/README.md`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/__init__.py` & `giskard-2.0.0b7/giskard/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/cli.py` & `giskard-2.0.0b7/giskard/cli.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/cli_utils.py` & `giskard-2.0.0b7/giskard/cli_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/client/giskard_client.py` & `giskard-2.0.0b7/giskard/client/giskard_client.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/client/io_utils.py` & `giskard-2.0.0b7/giskard/client/io_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/client/project.py` & `giskard-2.0.0b7/giskard/client/project.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/client/python_utils.py` & `giskard-2.0.0b7/giskard/client/python_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/commands/cli_server.py` & `giskard-2.0.0b7/giskard/commands/cli_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,15 +116,14 @@
             get_image_name(version),
             detach=not attached,
             name=get_container_name(version),
             ports={7860: port, 40051: ml_worker_port},
             volumes={home_volume.name: {"bind": "/home/giskard/datadir", "mode": "rw"}},
         )
     container.start()
-    analytics.track("Giskard Server started", {"client version": giskard.__version__, "server version": version})
     logger.info(f"Giskard Server {version} started. You can access it at http://localhost:{port}")
 
 
 def _check_downloaded(version: str):
     image = get_image_name(version)
     try:
         create_docker_client().images.get(image)
@@ -208,15 +207,14 @@
 
     http_tunnel = ngrok.connect(19000, "http", pyngrok_config=None if token else PyngrokConfig(region="us"))
     tcp_tunnel = ngrok.connect(40051, "tcp", pyngrok_config=None if token else PyngrokConfig(region="eu"))
 
     # Only split the last ':' in case the URL contains a port
     tcp_addr = urlparse(tcp_tunnel.public_url)
 
-    analytics.track("Giskard Server exposed via ngrok", {"client version": giskard.__version__})
     print("Giskard Server is now exposed to the internet.")
     print("You can now upload objects to the Giskard Server using the following client: \n")
 
     print(
         f"""token=...
 client = giskard.GiskardClient(\"{http_tunnel.public_url}\", token)
 
@@ -251,25 +249,33 @@
 def start(attached, version):
     """\b
     Start Giskard Server.
 
     By default, the server starts detached and will run in the background.
     You can attach to it by using -a
     """
+    analytics.track(
+        "giskard-server:start",
+        {
+            "attached": attached,
+            "version": version,
+        },
+    )
     _start(attached, version)
 
 
 @server.command("stop")
 @common_options
 def stop():
     """\b
     Stop Giskard Server.
 
     Stops a running Giskard server. Does nothing if Giskard server is not running.
     """
+    analytics.track("giskard-server:stop")
     container = get_container()
     if container.status != "exited":
         logger.info("Stopping Giskard Server")
         container.stop()
         logger.info("Giskard Server stopped")
     else:
         logger.info(f"Giskard container {container.name} is not running")
@@ -281,14 +287,21 @@
 @common_options
 def restart(service, hard):
     """\b
     Restart Giskard Server.
 
     Stops any running Giskard server and starts it again.
     """
+    analytics.track(
+        "giskard-server:restart",
+        {
+            "service": service,
+            "hard": hard,
+        },
+    )
     container = get_container()
     if container.status != "running":
         logger.info("Giskard server isn't running")
         _start()
     else:
         if hard:
             logger.info(f"Restarting {container.name} container")
@@ -312,14 +325,22 @@
 @click.option("--lines", "-l", "nb_lines", default=300, type=click.IntRange(0), help="Number of log lines to show")
 @click.option("--follow", "-f", "follow", is_flag=True, default=False, help="Follow the logs stream")
 @common_options
 def logs(service, nb_lines, follow):
     """\b
     Prints logs of server services
     """
+    analytics.track(
+        "giskard-server:logs",
+        {
+            "service": service,
+            "nb_lines": nb_lines,
+            "follow": follow,
+        },
+    )
     container = get_container()
     if not follow:
         if service:
             command = f"tail -{nb_lines} /home/giskard/datadir/run/{service}.log"
         else:
             command = "bash -c 'tail /home/giskard/datadir/run/*.log'"
         print(container.exec_run(command).output.decode())
@@ -343,48 +364,53 @@
     help="Destination directory to save diagnose archive to",
 )
 @common_options
 def diagnose(local_dir):
     """\b
     Save server logs to a local archive (Useful for support).
     """
+    analytics.track("giskard-server:diagnose")
     out_dir = Path(local_dir)
     assert out_dir.is_dir(), "'output' should be an existing directory"
     bits, stat = get_container().get_archive("/home/giskard/datadir/run", encode_stream=True)
     from datetime import datetime
 
     now = datetime.now().strftime("%Y%m%d_%H%M%S_%f")
     out_file = out_dir / f"giskard-diagnose-{get_version().replace('.', '_')}-{now}.tar.gz"
     with open(out_file, "wb") as f:
         for chunk in bits:
             f.write(chunk)
-    analytics.track("Giskard Server diagnosis ran", {"client version": giskard.__version__})
     logger.info(f"Wrote diagnose info to {out_file}")
 
 
 @server.command("update")
 @common_options
 @click.argument("version", required=False, default=None)
 def update(version):
     """\b
     Update Giskard Server. Uses the latest available version if not specified.
     """
+    analytics.track(
+        "giskard-server:update",
+        {
+            "version": version,
+        },
+    )
     latest_version = _fetch_latest_tag()
     if not version:
         version = latest_version
 
     installed_version = _get_settings().get("version")
     if installed_version == version:
         logger.info(f"Giskard server is already running version {version}")
         return
 
     logger.info(f"Updating Giskard Server {installed_version} -> {version}")
     _pull_image(version)
     _write_settings({**_get_settings(), **{"version": version}})
-    analytics.track("Giskard Server updated", {"client version": giskard.__version__, "server version": version})
     logger.info(f"Giskard Server updated to {version}")
 
 
 def read_version(version_str: str) -> Version:
     try:
         return version.parse(version_str)
     except InvalidVersion:
@@ -393,14 +419,15 @@
 
 @server.command("status")
 @common_options
 def status():
     """\b
     Check if server container is running and status of each internal service
     """
+    analytics.track("giskard-server:status")
     app_settings = _get_settings()
     if not app_settings:
         logger.info("Giskard Server is not installed. Install using `giskard server start`")
         return
     else:
         version = app_settings["version"]
 
@@ -423,14 +450,15 @@
 @server.command("clean")
 @click.option("--data", "delete_data", is_flag=True, help="Delete user data (giskard-home volume)")
 @common_options
 def clean(delete_data):
     """\b
     Delete Docker container, container (and possibly a volume) associated with the current version of Giskard Server
     """
+    analytics.track("giskard-server:clean", {"delete_data": delete_data})
     data_deletion_confirmed = delete_data and click.confirm(
         "Are you sure you want to delete user data (giskard-home volume)? "
         "This will permanently erase all of the Giskard activity results"
     )
 
     client = create_docker_client()
     container_name = get_container_name()
@@ -468,8 +496,9 @@
     "generated from https://dashboard.ngrok.com/get-started/your-authtoken",
 )
 @common_options
 def expose(token):
     """\b
     Expose your local Giskard Server to the outside world using ngrok to use in notebooks like Google Colab
     """
+    analytics.track("giskard-server:expose")
     _expose(token)
```

### Comparing `giskard-2.0.0b6/giskard/commands/cli_worker.py` & `giskard-2.0.0b7/giskard/commands/cli_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 from giskard.cli_utils import common_options
 from giskard.cli_utils import (
     create_pid_file_path,
     remove_stale_pid_file,
     run_daemon,
     get_log_path,
     tail,
-    follow_file, validate_url,
+    follow_file,
+    validate_url,
 )
 from giskard.path_utils import run_dir
 from giskard.settings import settings
 from giskard.utils.analytics_collector import anonymize, analytics
 
 logger = logging.getLogger(__name__)
 
@@ -85,14 +86,18 @@
     ML Worker can be started in 2 modes:
 
     - server: used by default by an ML Worker shipped by Giskard. ML Worker acts as a server that Giskard connects to.
 
     - client: ML Worker acts as a client and should connect to a running Giskard instance
         by specifying this instance's host and port.
     """
+    analytics.track(
+        "giskard-worker:start",
+        {"is_server": is_server, "url": anonymize(url), "is_daemon": is_daemon},
+    )
     api_key = initialize_api_key(api_key, is_server)
     _start_command(is_server, url, api_key, is_daemon)
 
 
 def initialize_api_key(api_key, is_server):
     if is_server:
         return None
@@ -103,18 +108,14 @@
         del os.environ["GSK_API_KEY"]
     return api_key
 
 
 def _start_command(is_server, url: AnyHttpUrl, api_key, is_daemon):
     from giskard.ml_worker.ml_worker import MLWorker
 
-    analytics.track(
-        "Start ML Worker", {"is_server": is_server, "url": anonymize(url), "is_daemon": is_daemon}, force=True
-    )
-
     start_msg = "Starting ML Worker"
     start_msg += " server" if is_server else " client"
     if is_daemon:
         start_msg += " daemon"
     logger.info(start_msg)
     logger.info(f"Python: {sys.executable} ({platform.python_version()})")
     logger.info(f"Giskard Home: {settings.home_dir}")
@@ -143,17 +144,16 @@
             asyncio.get_event_loop().run_until_complete(ml_worker.stop())
     except lockfile.AlreadyLocked:
         existing_pid = read_pid_from_pidfile(pid_file_path)
         logger.warning(
             f"Another ML Worker {_ml_worker_description(is_server, url)} "
             f"is already running with PID: {existing_pid}. "
             "Not starting a new one. "
-            "To stop a running worker for this instance execute: \"giskard worker stop\" or "
-            "\"giskard worker stop -a\" to stop all running workers"
-
+            'To stop a running worker for this instance execute: "giskard worker stop" or '
+            '"giskard worker stop -a" to stop all running workers'
         )
     finally:
         if pid_file.i_am_locking():
             pid_file.release()
 
 
 def _ml_worker_description(is_server, url):
@@ -163,28 +163,36 @@
 @worker.command("stop", help="Stop running ML Workers")
 @common_options
 @start_stop_options
 @click.option("--all", "-a", "stop_all", is_flag=True, default=False, help="Stop all running ML Workers")
 def stop_command(is_server, url, stop_all):
     import re
 
+    analytics.track(
+        "giskard-worker:stop",
+        {"is_server": is_server, "url": anonymize(url), "stop_all": stop_all},
+    )
     if stop_all:
         for pid_fname in os.listdir(run_dir):
             if not re.match(r"^ml-worker-.*\.pid$", pid_fname):
                 continue
             _stop_pid_fname(pid_fname)
     else:
         _find_and_stop(is_server, url)
 
 
 @worker.command("restart", help="Restart ML Worker")
 @common_options
 @start_stop_options
 @click.option("--api-key", "-k", "api_key", help="Giskard server API key")
 def restart_command(is_server, url, api_key):
+    analytics.track(
+        "giskard-worker:restart",
+        {"is_server": is_server, "url": anonymize(url)},
+    )
     api_key = initialize_api_key(api_key, is_server)
 
     _find_and_stop(is_server, url)
     _start_command(is_server, url, api_key, is_daemon=True)
 
 
 def _stop_pid_fname(pid_fname):
@@ -226,14 +234,21 @@
     "-f",
     "is_follow",
     is_flag=True,
     default=False,
     help="Output appended data as new logs are being generated",
 )
 def read_logs(lines, is_follow):
+    analytics.track(
+        "giskard-worker:logs",
+        {
+            "lines": lines,
+            "is_follow": is_follow,
+        },
+    )
     log_path = get_log_path()
 
     if not os.path.exists(log_path):
         print(f"Unable to find any logfile!\n{log_path} does not exists")
         exit(-1)
 
     for line in tail(log_path, lines):
```

### Comparing `giskard-2.0.0b6/giskard/core/core.py` & `giskard-2.0.0b7/giskard/core/core.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/core/dataset_validation.py` & `giskard-2.0.0b7/giskard/core/dataset_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/core/errors.py` & `giskard-2.0.0b7/giskard/core/errors.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/core/model_validation.py` & `giskard-2.0.0b7/giskard/core/model_validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/core/suite.py` & `giskard-2.0.0b7/giskard/core/suite.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/core/validation.py` & `giskard-2.0.0b7/giskard/core/validation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/datasets/__init__.py` & `giskard-2.0.0b7/giskard/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/datasets/base/__init__.py` & `giskard-2.0.0b7/giskard/datasets/base/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/datasets/metadata/indexing.py` & `giskard-2.0.0b7/giskard/datasets/metadata/indexing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/datasets/metadata/registry.py` & `giskard-2.0.0b7/giskard/datasets/metadata/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/datasets/metadata/text_metadata_provider.py` & `giskard-2.0.0b7/giskard/datasets/metadata/text_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/demo/__init__.py` & `giskard-2.0.0b7/giskard/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/demo/titanic.csv` & `giskard-2.0.0b7/giskard/demo/titanic.csv`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/bridge/data_encryptor.py` & `giskard-2.0.0b7/giskard/ml_worker/bridge/data_encryptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/bridge/ml_worker_bridge.py` & `giskard-2.0.0b7/giskard/ml_worker/bridge/ml_worker_bridge.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/core/log_listener.py` & `giskard-2.0.0b7/giskard/ml_worker/core/log_listener.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/core/savable.py` & `giskard-2.0.0b7/giskard/ml_worker/core/savable.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/generated/ml_worker_pb2.py` & `giskard-2.0.0b7/giskard/ml_worker/generated/ml_worker_pb2.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/generated/ml_worker_pb2_grpc.py` & `giskard-2.0.0b7/giskard/ml_worker/generated/ml_worker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/ml_worker.py` & `giskard-2.0.0b7/giskard/ml_worker/ml_worker.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/server/ml_worker_service.py` & `giskard-2.0.0b7/giskard/ml_worker/server/ml_worker_service.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/testing/functions/slicing.py` & `giskard-2.0.0b7/giskard/ml_worker/testing/functions/slicing.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/testing/functions/transformation.py` & `giskard-2.0.0b7/giskard/ml_worker/testing/functions/transformation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/testing/registry/decorators.py` & `giskard-2.0.0b7/giskard/ml_worker/testing/registry/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/testing/registry/decorators_utils.py` & `giskard-2.0.0b7/giskard/ml_worker/testing/registry/decorators_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/testing/registry/giskard_test.py` & `giskard-2.0.0b7/giskard/ml_worker/testing/registry/giskard_test.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/testing/registry/registry.py` & `giskard-2.0.0b7/giskard/ml_worker/testing/registry/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/testing/registry/slicing_function.py` & `giskard-2.0.0b7/giskard/ml_worker/testing/registry/slicing_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/testing/registry/transformation_function.py` & `giskard-2.0.0b7/giskard/ml_worker/testing/registry/transformation_function.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/testing/registry/udf_repository.py` & `giskard-2.0.0b7/giskard/ml_worker/testing/registry/udf_repository.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/testing/stat_utils.py` & `giskard-2.0.0b7/giskard/ml_worker/testing/stat_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/testing/test_result.py` & `giskard-2.0.0b7/giskard/ml_worker/testing/test_result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/testing/utils.py` & `giskard-2.0.0b7/giskard/ml_worker/testing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/utils/logging.py` & `giskard-2.0.0b7/giskard/ml_worker/utils/logging.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/utils/network.py` & `giskard-2.0.0b7/giskard/ml_worker/utils/network.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/ml_worker/utils/request_interceptor.py` & `giskard-2.0.0b7/giskard/ml_worker/utils/request_interceptor.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/__init__.py` & `giskard-2.0.0b7/giskard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/_precooked.py` & `giskard-2.0.0b7/giskard/models/_precooked.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/automodel/__init__.py` & `giskard-2.0.0b7/giskard/models/automodel/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/base/__init__.py` & `giskard-2.0.0b7/giskard/models/base/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/cache/__init__.py` & `giskard-2.0.0b7/giskard/models/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/cache/cache.py` & `giskard-2.0.0b7/giskard/models/cache/cache.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/catboost/__init__.py` & `giskard-2.0.0b7/giskard/models/catboost/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/function/__init__.py` & `giskard-2.0.0b7/giskard/models/function/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/huggingface/__init__.py` & `giskard-2.0.0b7/giskard/models/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/langchain/__init__.py` & `giskard-2.0.0b7/giskard/models/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/model_explanation.py` & `giskard-2.0.0b7/giskard/models/model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/pytorch/__init__.py` & `giskard-2.0.0b7/giskard/models/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/sklearn/__init__.py` & `giskard-2.0.0b7/giskard/models/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/tensorflow/__init__.py` & `giskard-2.0.0b7/giskard/models/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/models/utils.py` & `giskard-2.0.0b7/giskard/models/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/path_utils.py` & `giskard-2.0.0b7/giskard/path_utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/__init__.py` & `giskard-2.0.0b7/giskard/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/calibration/issues.py` & `giskard-2.0.0b7/giskard/scanner/calibration/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/calibration/overconfidence_detector.py` & `giskard-2.0.0b7/giskard/scanner/calibration/overconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/calibration/underconfidence_detector.py` & `giskard-2.0.0b7/giskard/scanner/calibration/underconfidence_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/common/examples.py` & `giskard-2.0.0b7/giskard/scanner/common/examples.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/common/loss_based_detector.py` & `giskard-2.0.0b7/giskard/scanner/common/loss_based_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/data_leakage/data_leakage_detector.py` & `giskard-2.0.0b7/giskard/scanner/data_leakage/data_leakage_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/decorators.py` & `giskard-2.0.0b7/giskard/scanner/decorators.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/issues.py` & `giskard-2.0.0b7/giskard/scanner/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/llm/toxicity_detector.py` & `giskard-2.0.0b7/giskard/scanner/llm/toxicity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/llm/utils.py` & `giskard-2.0.0b7/giskard/scanner/llm/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/performance/issues.py` & `giskard-2.0.0b7/giskard/scanner/performance/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/performance/metrics.py` & `giskard-2.0.0b7/giskard/scanner/performance/metrics.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/performance/performance_bias_detector.py` & `giskard-2.0.0b7/giskard/scanner/performance/performance_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/registry.py` & `giskard-2.0.0b7/giskard/scanner/registry.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/result.py` & `giskard-2.0.0b7/giskard/scanner/result.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/robustness/base_detector.py` & `giskard-2.0.0b7/giskard/scanner/robustness/base_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/robustness/entity_swap.py` & `giskard-2.0.0b7/giskard/scanner/robustness/entity_swap.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/robustness/ethical_bias_detector.py` & `giskard-2.0.0b7/giskard/scanner/robustness/ethical_bias_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/robustness/issues.py` & `giskard-2.0.0b7/giskard/scanner/robustness/issues.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/robustness/nationalities.json` & `giskard-2.0.0b7/giskard/scanner/robustness/nationalities.json`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/robustness/text_perturbation_detector.py` & `giskard-2.0.0b7/giskard/scanner/robustness/text_perturbation_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/robustness/text_transformations.py` & `giskard-2.0.0b7/giskard/scanner/robustness/text_transformations.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/scanner.py` & `giskard-2.0.0b7/giskard/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/stochasticity/stochasticity_detector.py` & `giskard-2.0.0b7/giskard/scanner/stochasticity/stochasticity_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/_code_snippet.html` & `giskard-2.0.0b7/giskard/scanner/templates/_code_snippet.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/_issues/data_leakage.html` & `giskard-2.0.0b7/giskard/scanner/templates/_issues/data_leakage.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/_issues/default.html` & `giskard-2.0.0b7/giskard/scanner/templates/_issues/default.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/_issues/llm_toxicity.html` & `giskard-2.0.0b7/giskard/scanner/templates/_issues/llm_toxicity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/_issues/overconfidence.html` & `giskard-2.0.0b7/giskard/scanner/templates/_issues/overconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/_issues/performance.html` & `giskard-2.0.0b7/giskard/scanner/templates/_issues/performance.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/_issues/robustness.html` & `giskard-2.0.0b7/giskard/scanner/templates/_issues/robustness.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/_issues/stochasticity.html` & `giskard-2.0.0b7/giskard/scanner/templates/_issues/stochasticity.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/_issues/underconfidence.html` & `giskard-2.0.0b7/giskard/scanner/templates/_issues/underconfidence.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/_issues_table.html` & `giskard-2.0.0b7/giskard/scanner/templates/_issues_table.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/_main_content.html` & `giskard-2.0.0b7/giskard/scanner/templates/_main_content.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/_tab_header.html` & `giskard-2.0.0b7/giskard/scanner/templates/_tab_header.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/scan_results.html` & `giskard-2.0.0b7/giskard/scanner/templates/scan_results.html`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/static/external.js` & `giskard-2.0.0b7/giskard/scanner/templates/static/external.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/static/internal.js` & `giskard-2.0.0b7/giskard/scanner/templates/static/internal.js`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/templates/static/style.css` & `giskard-2.0.0b7/giskard/scanner/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/scanner/visualization/custom_jinja.py` & `giskard-2.0.0b7/giskard/scanner/visualization/custom_jinja.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/settings.py` & `giskard-2.0.0b7/giskard/settings.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/slicing/base.py` & `giskard-2.0.0b7/giskard/slicing/base.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/slicing/bruteforce_slicer.py` & `giskard-2.0.0b7/giskard/slicing/bruteforce_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/slicing/category_slicer.py` & `giskard-2.0.0b7/giskard/slicing/category_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/slicing/multiscale_slicer.py` & `giskard-2.0.0b7/giskard/slicing/multiscale_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/slicing/opt_slicer.py` & `giskard-2.0.0b7/giskard/slicing/opt_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/slicing/slice.py` & `giskard-2.0.0b7/giskard/slicing/slice.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/slicing/stop_words.py` & `giskard-2.0.0b7/giskard/slicing/stop_words.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/slicing/text_slicer.py` & `giskard-2.0.0b7/giskard/slicing/text_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/slicing/tree_slicer.py` & `giskard-2.0.0b7/giskard/slicing/tree_slicer.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/slicing/utils.py` & `giskard-2.0.0b7/giskard/slicing/utils.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/testing/__init__.py` & `giskard-2.0.0b7/giskard/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/testing/tests/drift.py` & `giskard-2.0.0b7/giskard/testing/tests/drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/testing/tests/metamorphic.py` & `giskard-2.0.0b7/giskard/testing/tests/metamorphic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/testing/tests/performance.py` & `giskard-2.0.0b7/giskard/testing/tests/performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/testing/tests/statistic.py` & `giskard-2.0.0b7/giskard/testing/tests/statistic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard/utils/analytics_collector.py` & `giskard-2.0.0b7/giskard/utils/analytics_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,16 @@
         self.initialize_user_properties()
 
         if self.is_enabled or force:
             merged_props = {
                 "giskard_version": self.giskard_version,
                 "python_version": platform.python_version(),
                 "environment": self.environment,
+                # only for aggregated stats: city, country, region. IP itself isn't stored
+                "ip": self.ip,
             }
             if properties is not None:
                 merged_props = {**merged_props, **properties}
             if self.server_info is not None:
                 merged_props = {**merged_props, **self.server_info}
 
             self.mp.track(
@@ -172,16 +174,14 @@
                 self.distinct_user_id,
                 {
                     "$name": "",
                     "arch": platform.machine(),
                     "$os": platform.system(),
                     "os-full": platform.platform(aliased=True),
                 },
-                # only for aggregated stats: city, country, region. IP itself isn't stored
-                meta={"$ip": self.ip},
             )
 
     @staticmethod
     def machine_based_user_id():
         try:
             return anonymize(str(uuid.getnode()) + getpass.getuser())
         except BaseException:  # noqa NOSONAR
```

### Comparing `giskard-2.0.0b6/giskard/utils/environment_detector.py` & `giskard-2.0.0b7/giskard/utils/environment_detector.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard.egg-info/PKG-INFO` & `giskard-2.0.0b7/giskard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giskard
-Version: 2.0.0b6
+Version: 2.0.0b7
 Summary: The testing framework dedicated to ML models, from tabular to LLMs
 Author-email: Giskard AI <hello@giskard.ai>
 License: Apache Software License 2.0
 Project-URL: Homepage, https://giskard.ai
 Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues
 Project-URL: Documentation, https://docs.giskard.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: giskard Version: 2.0.0b6 Summary: The testing
+Metadata-Version: 2.1 Name: giskard Version: 2.0.0b7 Summary: The testing
 framework dedicated to ML models, from tabular to LLMs Author-email: Giskard AI
 giskard.ai> License: Apache Software License 2.0 Project-URL: Homepage, https:/
 /giskard.ai Project-URL: Source Code, https://github.com/Giskard-AI/giskard
 Project-URL: Bug Tracker, https://github.com/Giskard-AI/giskard/issues Project-
 URL: Documentation, https://docs.giskard.ai/ Project-URL: Discord, https://
 discord.gg/ABvfpbu69R Project-URL: Linkedin, https://www.linkedin.com/company/
 giskard-ai Project-URL: Mastodon, https://fosstodon.org/@Giskard Project-URL:
```

### Comparing `giskard-2.0.0b6/giskard.egg-info/SOURCES.txt` & `giskard-2.0.0b7/giskard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/giskard.egg-info/requires.txt` & `giskard-2.0.0b7/giskard.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/pyproject.toml` & `giskard-2.0.0b7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 "Twitter" = "https://twitter.com/giskard_ai"
 
 
 [project]
 name = "giskard"
 readme = "README.md"
 license = { text = "Apache Software License 2.0" }
-version = "2.0.0b6"
+version = "2.0.0b7"
 description = "The testing framework dedicated to ML models, from tabular to LLMs"
 authors = [
     { name = "Giskard AI", email = "hello@giskard.ai" },
 ]
 keywords = [
     "Artificial Intelligence",
     "Machine Learning",
```

### Comparing `giskard-2.0.0b6/setup.py` & `giskard-2.0.0b7/setup.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_custom_model.py` & `giskard-2.0.0b7/tests/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_data_drift.py` & `giskard-2.0.0b7/tests/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_data_processing_pipeline.py` & `giskard-2.0.0b7/tests/test_data_processing_pipeline.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_dataset.py` & `giskard-2.0.0b7/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_metamorphic_direction.py` & `giskard-2.0.0b7/tests/test_metamorphic_direction.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_metamorphic_invariance.py` & `giskard-2.0.0b7/tests/test_metamorphic_invariance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_model.py` & `giskard-2.0.0b7/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_model_auto_inference.py` & `giskard-2.0.0b7/tests/test_model_auto_inference.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_model_explanation.py` & `giskard-2.0.0b7/tests/test_model_explanation.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_model_postprocess.py` & `giskard-2.0.0b7/tests/test_model_postprocess.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_performance.py` & `giskard-2.0.0b7/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_programmatic.py` & `giskard-2.0.0b7/tests/test_programmatic.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_project_uploads.py` & `giskard-2.0.0b7/tests/test_project_uploads.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_statistical.py` & `giskard-2.0.0b7/tests/test_statistical.py`

 * *Files identical despite different names*

### Comparing `giskard-2.0.0b6/tests/test_upload.py` & `giskard-2.0.0b7/tests/test_upload.py`

 * *Files identical despite different names*

