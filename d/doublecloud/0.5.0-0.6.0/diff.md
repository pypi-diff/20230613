# Comparing `tmp/doublecloud-0.5.0.tar.gz` & `tmp/doublecloud-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doublecloud-0.5.0.tar", last modified: Tue May  2 11:23:04 2023, max compression
+gzip compressed data, was "doublecloud-0.6.0.tar", last modified: Tue Jun 13 09:30:46 2023, max compression
```

## Comparing `doublecloud-0.5.0.tar` & `doublecloud-0.6.0.tar`

### file list

```diff
@@ -1,210 +1,222 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.456065 doublecloud-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 11:22:36.000000 doublecloud-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-02 11:23:04.456065 doublecloud-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-02 11:22:36.000000 doublecloud-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.416064 doublecloud-0.5.0/doublecloud/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/_auth_fabric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/_auth_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/_backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/_operation_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/_retry_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.420064 doublecloud-0.5.0/doublecloud/_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.420064 doublecloud-0.5.0/doublecloud/_wrappers/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/_wrappers/clickhouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.420064 doublecloud-0.5.0/doublecloud/_wrappers/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/_wrappers/kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.420064 doublecloud-0.5.0/doublecloud/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.428064 doublecloud-0.5.0/doublecloud/clickhouse/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/backup_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/backup_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/backup_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/backup_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/backup_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/cluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/cluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/cluster_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/cluster_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17637 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/operation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/version_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/version_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/version_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/version_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/version_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.428064 doublecloud-0.5.0/doublecloud/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.436065 doublecloud-0.5.0/doublecloud/kafka/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/cluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/cluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/cluster_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/cluster_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20537 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/operation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/topic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/topic_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/topic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/topic_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/topic_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/user_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/user_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/version_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/version_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/version_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/version_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/version_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/kafka/v1/version_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.436065 doublecloud-0.5.0/doublecloud/network/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.436065 doublecloud-0.5.0/doublecloud/network/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/network_connection_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/network_connection_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/network_connection_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/network_connection_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/network_connection_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/network_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/network_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/network_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/network_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/network_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/network_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/operation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/network/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.436065 doublecloud-0.5.0/doublecloud/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.440065 doublecloud-0.5.0/doublecloud/transfer/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.444065 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.452065 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24164 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/kafka_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/kafka_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/mongo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/mongo_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/mysql_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/mysql_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/parsers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/parsers_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/postgres_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/postgres_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/operation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/operation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/transfer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/transfer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/transfer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/transfer_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/transfer_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13479 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.452065 doublecloud-0.5.0/doublecloud/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/v1/cluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/v1/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/v1/cluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/v1/maintenance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/v1/maintenance_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/v1/maintenance_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/v1/operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/v1/operation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/v1/operation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/v1/paging_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/v1/paging_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/v1/paging_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.452065 doublecloud-0.5.0/doublecloud/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.456065 doublecloud-0.5.0/doublecloud/visualization/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/visualization/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/visualization/v1/workbook_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/visualization/v1/workbook_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/visualization/v1/workbook_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/visualization/v1/workbook_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/visualization/v1/workbook_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-05-02 11:22:36.000000 doublecloud-0.5.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:23:04.420064 doublecloud-0.5.0/doublecloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-02 11:23:04.000000 doublecloud-0.5.0/doublecloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-05-02 11:23:04.000000 doublecloud-0.5.0/doublecloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:23:04.000000 doublecloud-0.5.0/doublecloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:23:04.000000 doublecloud-0.5.0/doublecloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 11:23:04.000000 doublecloud-0.5.0/doublecloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 11:23:04.000000 doublecloud-0.5.0/doublecloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-02 11:22:36.000000 doublecloud-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:23:04.456065 doublecloud-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-02 11:23:01.000000 doublecloud-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.797770 doublecloud-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 09:30:13.000000 doublecloud-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-13 09:30:46.797770 doublecloud-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-13 09:30:13.000000 doublecloud-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_auth_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_auth_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_operation_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_retry_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/_wrappers/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_wrappers/clickhouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/_wrappers/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/_wrappers/kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/clickhouse/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24545 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/version_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/version_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/version_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/version_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/version_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.785770 doublecloud-0.6.0/doublecloud/kafka/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/cluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/cluster_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/cluster_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20537 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/connector_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14894 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/connector_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/connector_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/connector_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/connector_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/connector_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/topic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/topic_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/topic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/topic_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/topic_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/user_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/user_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/version_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/version_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/version_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/version_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/version_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/kafka/v1/version_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.785770 doublecloud-0.6.0/doublecloud/network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.789770 doublecloud-0.6.0/doublecloud/network/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_connection_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_connection_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_connection_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_connection_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_connection_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/network_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/network/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.789770 doublecloud-0.6.0/doublecloud/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.789770 doublecloud-0.6.0/doublecloud/transfer/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.793770 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.793770 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24164 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/delta_lake_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/kafka_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/kafka_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mongo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mongo_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mysql_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mysql_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/parsers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/parsers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/postgres_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/postgres_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/operation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/operation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/transfer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/transfer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/transfer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/transfer_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/transfer_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19365 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.797770 doublecloud-0.6.0/doublecloud/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/cluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/cluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/maintenance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/maintenance_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/maintenance_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/operation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/operation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/paging_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/paging_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/v1/paging_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.797770 doublecloud-0.6.0/doublecloud/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.797770 doublecloud-0.6.0/doublecloud/visualization/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/workbook_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/workbook_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/workbook_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/workbook_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/workbook_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-06-13 09:30:13.000000 doublecloud-0.6.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:30:46.781770 doublecloud-0.6.0/doublecloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-13 09:30:46.000000 doublecloud-0.6.0/doublecloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-06-13 09:30:46.000000 doublecloud-0.6.0/doublecloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:30:46.000000 doublecloud-0.6.0/doublecloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:30:46.000000 doublecloud-0.6.0/doublecloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 09:30:46.000000 doublecloud-0.6.0/doublecloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 09:30:46.000000 doublecloud-0.6.0/doublecloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 09:30:13.000000 doublecloud-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:30:46.797770 doublecloud-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-13 09:30:42.000000 doublecloud-0.6.0/setup.py
```

### Comparing `doublecloud-0.5.0/LICENSE` & `doublecloud-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/PKG-INFO` & `doublecloud-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doublecloud
-Version: 0.5.0
+Version: 0.6.0
 Summary: The Double.Cloud official SDK
 Home-page: https://github.com/doublecloud/python-sdk
 Author: DoubleCloud GmbH
 Author-email: support@double.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doublecloud-0.5.0/README.md` & `doublecloud-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/_auth_fabric.py` & `doublecloud-0.6.0/doublecloud/_auth_fabric.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/_auth_plugin.py` & `doublecloud-0.6.0/doublecloud/_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/_backoff.py` & `doublecloud-0.6.0/doublecloud/_backoff.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/_channels.py` & `doublecloud-0.6.0/doublecloud/_channels.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/_operation_waiter.py` & `doublecloud-0.6.0/doublecloud/_operation_waiter.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/_retry_interceptor.py` & `doublecloud-0.6.0/doublecloud/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/_sdk.py` & `doublecloud-0.6.0/doublecloud/_sdk.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/backup_pb2.py` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/clickhouse/v1/backup.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&doublecloud/clickhouse/v1/backup.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\xfe\x02\n\x06\x42\x61\x63kup\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12;\n\x0b\x63reate_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x39\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12*\n\x11source_cluster_id\x18\x06 \x01(\tR\x0fsourceClusterId\x12\x12\n\x04size\x18\x07 \x01(\x03R\x04size\x12:\n\x04type\x18\x08 \x01(\x0e\x32&.doublecloud.clickhouse.v1.Backup.TypeR\x04type\"=\n\x04Type\x12\x10\n\x0cTYPE_INVALID\x10\x00\x12\x12\n\x0eTYPE_AUTOMATED\x10\x01\x12\x0f\n\x0bTYPE_MANUAL\x10\x02\x42\x41Z?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&doublecloud/clickhouse/v1/backup.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\xfe\x02\n\x06\x42\x61\x63kup\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12;\n\x0b\x63reate_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x39\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12*\n\x11source_cluster_id\x18\x06 \x01(\tR\x0fsourceClusterId\x12\x12\n\x04size\x18\x07 \x01(\x03R\x04size\x12:\n\x04type\x18\x08 \x01(\x0e\x32&.doublecloud.clickhouse.v1.Backup.TypeR\x04type\"=\n\x04Type\x12\x10\n\x0cTYPE_INVALID\x10\x00\x12\x12\n\x0eTYPE_AUTOMATED\x10\x01\x12\x0f\n\x0bTYPE_MANUAL\x10\x02\x42IZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.clickhouse.v1.backup_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouse'
+  DESCRIPTOR._serialized_options = b'ZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouse'
   _globals['_BACKUP']._serialized_start=103
   _globals['_BACKUP']._serialized_end=485
   _globals['_BACKUP_TYPE']._serialized_start=424
   _globals['_BACKUP_TYPE']._serialized_end=485
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/backup_pb2.pyi` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/backup_service_pb2.py` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/clickhouse/v1/backup_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 from doublecloud.clickhouse.v1 import backup_pb2 as doublecloud_dot_clickhouse_dot_v1_dot_backup__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.doublecloud/clickhouse/v1/backup_service.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\x1a&doublecloud/clickhouse/v1/backup.proto\"/\n\x10GetBackupRequest\x12\x1b\n\tbackup_id\x18\x01 \x01(\tR\x08\x62\x61\x63kupId\"c\n\x12ListBackupsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x89\x01\n\x13ListBackupsResponse\x12;\n\x07\x62\x61\x63kups\x18\x01 \x03(\x0b\x32!.doublecloud.clickhouse.v1.BackupR\x07\x62\x61\x63kups\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"H\n\x13\x43reateBackupRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\"2\n\x13\x44\x65leteBackupRequest\x12\x1b\n\tbackup_id\x18\x01 \x01(\tR\x08\x62\x61\x63kupId2\xf7\x02\n\rBackupService\x12U\n\x03Get\x12+.doublecloud.clickhouse.v1.GetBackupRequest\x1a!.doublecloud.clickhouse.v1.Backup\x12\x65\n\x04List\x12-.doublecloud.clickhouse.v1.ListBackupsRequest\x1a..doublecloud.clickhouse.v1.ListBackupsResponse\x12S\n\x06\x43reate\x12..doublecloud.clickhouse.v1.CreateBackupRequest\x1a\x19.doublecloud.v1.Operation\x12S\n\x06\x44\x65lete\x12..doublecloud.clickhouse.v1.DeleteBackupRequest\x1a\x19.doublecloud.v1.OperationBAZ?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.doublecloud/clickhouse/v1/backup_service.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\x1a&doublecloud/clickhouse/v1/backup.proto\"/\n\x10GetBackupRequest\x12\x1b\n\tbackup_id\x18\x01 \x01(\tR\x08\x62\x61\x63kupId\"c\n\x12ListBackupsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x89\x01\n\x13ListBackupsResponse\x12;\n\x07\x62\x61\x63kups\x18\x01 \x03(\x0b\x32!.doublecloud.clickhouse.v1.BackupR\x07\x62\x61\x63kups\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"H\n\x13\x43reateBackupRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\"2\n\x13\x44\x65leteBackupRequest\x12\x1b\n\tbackup_id\x18\x01 \x01(\tR\x08\x62\x61\x63kupId2\xf7\x02\n\rBackupService\x12U\n\x03Get\x12+.doublecloud.clickhouse.v1.GetBackupRequest\x1a!.doublecloud.clickhouse.v1.Backup\x12\x65\n\x04List\x12-.doublecloud.clickhouse.v1.ListBackupsRequest\x1a..doublecloud.clickhouse.v1.ListBackupsResponse\x12S\n\x06\x43reate\x12..doublecloud.clickhouse.v1.CreateBackupRequest\x1a\x19.doublecloud.v1.Operation\x12S\n\x06\x44\x65lete\x12..doublecloud.clickhouse.v1.DeleteBackupRequest\x1a\x19.doublecloud.v1.OperationBIZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.clickhouse.v1.backup_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouse'
+  DESCRIPTOR._serialized_options = b'ZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouse'
   _globals['_GETBACKUPREQUEST']._serialized_start=178
   _globals['_GETBACKUPREQUEST']._serialized_end=225
   _globals['_LISTBACKUPSREQUEST']._serialized_start=227
   _globals['_LISTBACKUPSREQUEST']._serialized_end=326
   _globals['_LISTBACKUPSRESPONSE']._serialized_start=329
   _globals['_LISTBACKUPSRESPONSE']._serialized_end=466
   _globals['_CREATEBACKUPREQUEST']._serialized_start=468
```

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/backup_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/backup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/cluster_pb2.py` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/clickhouse/v1/cluster.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from doublecloud.clickhouse.v1 import config_pb2 as doublecloud_dot_clickhouse_dot_v1_dot_config__pb2
 from doublecloud.v1 import cluster_pb2 as doublecloud_dot_v1_dot_cluster__pb2
 from doublecloud.v1 import maintenance_pb2 as doublecloud_dot_v1_dot_maintenance__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'doublecloud/clickhouse/v1/cluster.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a&doublecloud/clickhouse/v1/config.proto\x1a\x1c\x64oublecloud/v1/cluster.proto\x1a doublecloud/v1/maintenance.proto\"\xd7\x07\n\x07\x43luster\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x03 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x04 \x01(\tR\x08regionId\x12;\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x07 \x01(\tR\x0b\x64\x65scription\x12\x35\n\x06status\x18\x08 \x01(\x0e\x32\x1d.doublecloud.v1.ClusterStatusR\x06status\x12\x18\n\x07version\x18\t \x01(\tR\x07version\x12I\n\tresources\x18\n \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClusterResourcesR\tresources\x12R\n\x0f\x63onnection_info\x18\x0b \x01(\x0b\x32).doublecloud.clickhouse.v1.ConnectionInfoR\x0e\x63onnectionInfo\x12.\n\x06\x61\x63\x63\x65ss\x18\x0c \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12h\n\x17private_connection_info\x18\r \x01(\x0b\x32\x30.doublecloud.clickhouse.v1.PrivateConnectionInfoR\x15privateConnectionInfo\x12>\n\nencryption\x18\x0e \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\x0f \x01(\tR\tnetworkId\x12X\n\x11\x63lickhouse_config\x18\x10 \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClickhouseConfigR\x10\x63lickhouseConfig\x12P\n\x12maintenance_window\x18\x11 \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12Y\n\x15maintenance_operation\x18\x12 \x01(\x0b\x32$.doublecloud.v1.MaintenanceOperationR\x14maintenanceOperation\"\xe1\x02\n\x10\x43lusterResources\x12V\n\nclickhouse\x18\x01 \x01(\x0b\x32\x36.doublecloud.clickhouse.v1.ClusterResources.ClickhouseR\nclickhouse\x1a\xf4\x01\n\nClickhouse\x12,\n\x12resource_preset_id\x18\x01 \x01(\tR\x10resourcePresetId\x12\x38\n\tdisk_size\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x08\x64iskSize\x12@\n\rreplica_count\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0creplicaCount\x12<\n\x0bshard_count\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\nshardCount\"\xd1\x02\n\x0e\x43onnectionInfo\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\x12:\n\nhttps_port\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\thttpsPort\x12\x43\n\x0ftcp_port_secure\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\rtcpPortSecure\x12\'\n\x0fnative_protocol\x18\x06 \x01(\tR\x0enativeProtocol\x12\x1b\n\thttps_uri\x18\x07 \x01(\tR\x08httpsUri\x12\x19\n\x08jdbc_uri\x18\x08 \x01(\tR\x07jdbcUri\x12\x19\n\x08odbc_uri\x18\t \x01(\tR\x07odbcUri\"\xd8\x02\n\x15PrivateConnectionInfo\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\x12:\n\nhttps_port\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\thttpsPort\x12\x43\n\x0ftcp_port_secure\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\rtcpPortSecure\x12\'\n\x0fnative_protocol\x18\x06 \x01(\tR\x0enativeProtocol\x12\x1b\n\thttps_uri\x18\x07 \x01(\tR\x08httpsUri\x12\x19\n\x08jdbc_uri\x18\x08 \x01(\tR\x07jdbcUri\x12\x19\n\x08odbc_uri\x18\t \x01(\tR\x07odbcUri\"{\n\x04Host\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ncluster_id\x18\x02 \x01(\tR\tclusterId\x12\x1d\n\nshard_name\x18\x03 \x01(\tR\tshardName\x12!\n\x0cprivate_name\x18\x04 \x01(\tR\x0bprivateNameBAZ?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'doublecloud/clickhouse/v1/cluster.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a&doublecloud/clickhouse/v1/config.proto\x1a\x1c\x64oublecloud/v1/cluster.proto\x1a doublecloud/v1/maintenance.proto\"\xdb\x08\n\x07\x43luster\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x03 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x04 \x01(\tR\x08regionId\x12;\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x07 \x01(\tR\x0b\x64\x65scription\x12\x35\n\x06status\x18\x08 \x01(\x0e\x32\x1d.doublecloud.v1.ClusterStatusR\x06status\x12\x18\n\x07version\x18\t \x01(\tR\x07version\x12I\n\tresources\x18\n \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClusterResourcesR\tresources\x12R\n\x0f\x63onnection_info\x18\x0b \x01(\x0b\x32).doublecloud.clickhouse.v1.ConnectionInfoR\x0e\x63onnectionInfo\x12.\n\x06\x61\x63\x63\x65ss\x18\x0c \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12h\n\x17private_connection_info\x18\r \x01(\x0b\x32\x30.doublecloud.clickhouse.v1.PrivateConnectionInfoR\x15privateConnectionInfo\x12>\n\nencryption\x18\x0e \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\x0f \x01(\tR\tnetworkId\x12X\n\x11\x63lickhouse_config\x18\x10 \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClickhouseConfigR\x10\x63lickhouseConfig\x12P\n\x12maintenance_window\x18\x11 \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12Y\n\x15maintenance_operation\x18\x12 \x01(\x0b\x32$.doublecloud.v1.MaintenanceOperationR\x14maintenanceOperation\x12\x81\x01\n metrics_exporter_connection_info\x18\x13 \x01(\x0b\x32\x38.doublecloud.clickhouse.v1.MetricsExporterConnectionInfoR\x1dmetricsExporterConnectionInfo\"\xe1\x02\n\x10\x43lusterResources\x12V\n\nclickhouse\x18\x01 \x01(\x0b\x32\x36.doublecloud.clickhouse.v1.ClusterResources.ClickhouseR\nclickhouse\x1a\xf4\x01\n\nClickhouse\x12,\n\x12resource_preset_id\x18\x01 \x01(\tR\x10resourcePresetId\x12\x38\n\tdisk_size\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x08\x64iskSize\x12@\n\rreplica_count\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0creplicaCount\x12<\n\x0bshard_count\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\nshardCount\"\xd1\x02\n\x0e\x43onnectionInfo\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\x12:\n\nhttps_port\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\thttpsPort\x12\x43\n\x0ftcp_port_secure\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\rtcpPortSecure\x12\'\n\x0fnative_protocol\x18\x06 \x01(\tR\x0enativeProtocol\x12\x1b\n\thttps_uri\x18\x07 \x01(\tR\x08httpsUri\x12\x19\n\x08jdbc_uri\x18\x08 \x01(\tR\x07jdbcUri\x12\x19\n\x08odbc_uri\x18\t \x01(\tR\x07odbcUri\"\xd8\x02\n\x15PrivateConnectionInfo\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\x12:\n\nhttps_port\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\thttpsPort\x12\x43\n\x0ftcp_port_secure\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\rtcpPortSecure\x12\'\n\x0fnative_protocol\x18\x06 \x01(\tR\x0enativeProtocol\x12\x1b\n\thttps_uri\x18\x07 \x01(\tR\x08httpsUri\x12\x19\n\x08jdbc_uri\x18\x08 \x01(\tR\x07jdbcUri\x12\x19\n\x08odbc_uri\x18\t \x01(\tR\x07odbcUri\"O\n\x1dMetricsExporterConnectionInfo\x12\x12\n\x04user\x18\x01 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x02 \x01(\tR\x08password\"\xaf\x01\n\x04Host\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ncluster_id\x18\x02 \x01(\tR\tclusterId\x12\x1d\n\nshard_name\x18\x03 \x01(\tR\tshardName\x12!\n\x0cprivate_name\x18\x04 \x01(\tR\x0bprivateName\x12\x32\n\x06status\x18\x05 \x01(\x0e\x32\x1a.doublecloud.v1.HostStatusR\x06statusBIZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.clickhouse.v1.cluster_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouse'
+  DESCRIPTOR._serialized_options = b'ZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouse'
   _globals['_CLUSTER']._serialized_start=240
-  _globals['_CLUSTER']._serialized_end=1223
-  _globals['_CLUSTERRESOURCES']._serialized_start=1226
-  _globals['_CLUSTERRESOURCES']._serialized_end=1579
-  _globals['_CLUSTERRESOURCES_CLICKHOUSE']._serialized_start=1335
-  _globals['_CLUSTERRESOURCES_CLICKHOUSE']._serialized_end=1579
-  _globals['_CONNECTIONINFO']._serialized_start=1582
-  _globals['_CONNECTIONINFO']._serialized_end=1919
-  _globals['_PRIVATECONNECTIONINFO']._serialized_start=1922
-  _globals['_PRIVATECONNECTIONINFO']._serialized_end=2266
-  _globals['_HOST']._serialized_start=2268
-  _globals['_HOST']._serialized_end=2391
+  _globals['_CLUSTER']._serialized_end=1355
+  _globals['_CLUSTERRESOURCES']._serialized_start=1358
+  _globals['_CLUSTERRESOURCES']._serialized_end=1711
+  _globals['_CLUSTERRESOURCES_CLICKHOUSE']._serialized_start=1467
+  _globals['_CLUSTERRESOURCES_CLICKHOUSE']._serialized_end=1711
+  _globals['_CONNECTIONINFO']._serialized_start=1714
+  _globals['_CONNECTIONINFO']._serialized_end=2051
+  _globals['_PRIVATECONNECTIONINFO']._serialized_start=2054
+  _globals['_PRIVATECONNECTIONINFO']._serialized_end=2398
+  _globals['_METRICSEXPORTERCONNECTIONINFO']._serialized_start=2400
+  _globals['_METRICSEXPORTERCONNECTIONINFO']._serialized_end=2479
+  _globals['_HOST']._serialized_start=2482
+  _globals['_HOST']._serialized_end=2657
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/cluster_pb2.pyi` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Cluster(_message.Message):
-    __slots__ = ["id", "project_id", "cloud_type", "region_id", "create_time", "name", "description", "status", "version", "resources", "connection_info", "access", "private_connection_info", "encryption", "network_id", "clickhouse_config", "maintenance_window", "maintenance_operation"]
+    __slots__ = ["id", "project_id", "cloud_type", "region_id", "create_time", "name", "description", "status", "version", "resources", "connection_info", "access", "private_connection_info", "encryption", "network_id", "clickhouse_config", "maintenance_window", "maintenance_operation", "metrics_exporter_connection_info"]
     ID_FIELD_NUMBER: _ClassVar[int]
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     CLOUD_TYPE_FIELD_NUMBER: _ClassVar[int]
     REGION_ID_FIELD_NUMBER: _ClassVar[int]
     CREATE_TIME_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
@@ -25,14 +25,15 @@
     ACCESS_FIELD_NUMBER: _ClassVar[int]
     PRIVATE_CONNECTION_INFO_FIELD_NUMBER: _ClassVar[int]
     ENCRYPTION_FIELD_NUMBER: _ClassVar[int]
     NETWORK_ID_FIELD_NUMBER: _ClassVar[int]
     CLICKHOUSE_CONFIG_FIELD_NUMBER: _ClassVar[int]
     MAINTENANCE_WINDOW_FIELD_NUMBER: _ClassVar[int]
     MAINTENANCE_OPERATION_FIELD_NUMBER: _ClassVar[int]
+    METRICS_EXPORTER_CONNECTION_INFO_FIELD_NUMBER: _ClassVar[int]
     id: str
     project_id: str
     cloud_type: str
     region_id: str
     create_time: _timestamp_pb2.Timestamp
     name: str
     description: str
@@ -43,15 +44,16 @@
     access: _cluster_pb2.Access
     private_connection_info: PrivateConnectionInfo
     encryption: _cluster_pb2.DataEncryption
     network_id: str
     clickhouse_config: _config_pb2.ClickhouseConfig
     maintenance_window: _maintenance_pb2.MaintenanceWindow
     maintenance_operation: _maintenance_pb2.MaintenanceOperation
-    def __init__(self, id: _Optional[str] = ..., project_id: _Optional[str] = ..., cloud_type: _Optional[str] = ..., region_id: _Optional[str] = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., status: _Optional[_Union[_cluster_pb2.ClusterStatus, str]] = ..., version: _Optional[str] = ..., resources: _Optional[_Union[ClusterResources, _Mapping]] = ..., connection_info: _Optional[_Union[ConnectionInfo, _Mapping]] = ..., access: _Optional[_Union[_cluster_pb2.Access, _Mapping]] = ..., private_connection_info: _Optional[_Union[PrivateConnectionInfo, _Mapping]] = ..., encryption: _Optional[_Union[_cluster_pb2.DataEncryption, _Mapping]] = ..., network_id: _Optional[str] = ..., clickhouse_config: _Optional[_Union[_config_pb2.ClickhouseConfig, _Mapping]] = ..., maintenance_window: _Optional[_Union[_maintenance_pb2.MaintenanceWindow, _Mapping]] = ..., maintenance_operation: _Optional[_Union[_maintenance_pb2.MaintenanceOperation, _Mapping]] = ...) -> None: ...
+    metrics_exporter_connection_info: MetricsExporterConnectionInfo
+    def __init__(self, id: _Optional[str] = ..., project_id: _Optional[str] = ..., cloud_type: _Optional[str] = ..., region_id: _Optional[str] = ..., create_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., status: _Optional[_Union[_cluster_pb2.ClusterStatus, str]] = ..., version: _Optional[str] = ..., resources: _Optional[_Union[ClusterResources, _Mapping]] = ..., connection_info: _Optional[_Union[ConnectionInfo, _Mapping]] = ..., access: _Optional[_Union[_cluster_pb2.Access, _Mapping]] = ..., private_connection_info: _Optional[_Union[PrivateConnectionInfo, _Mapping]] = ..., encryption: _Optional[_Union[_cluster_pb2.DataEncryption, _Mapping]] = ..., network_id: _Optional[str] = ..., clickhouse_config: _Optional[_Union[_config_pb2.ClickhouseConfig, _Mapping]] = ..., maintenance_window: _Optional[_Union[_maintenance_pb2.MaintenanceWindow, _Mapping]] = ..., maintenance_operation: _Optional[_Union[_maintenance_pb2.MaintenanceOperation, _Mapping]] = ..., metrics_exporter_connection_info: _Optional[_Union[MetricsExporterConnectionInfo, _Mapping]] = ...) -> None: ...
 
 class ClusterResources(_message.Message):
     __slots__ = ["clickhouse"]
     class Clickhouse(_message.Message):
         __slots__ = ["resource_preset_id", "disk_size", "replica_count", "shard_count"]
         RESOURCE_PRESET_ID_FIELD_NUMBER: _ClassVar[int]
         DISK_SIZE_FIELD_NUMBER: _ClassVar[int]
@@ -106,18 +108,28 @@
     tcp_port_secure: _wrappers_pb2.Int64Value
     native_protocol: str
     https_uri: str
     jdbc_uri: str
     odbc_uri: str
     def __init__(self, host: _Optional[str] = ..., user: _Optional[str] = ..., password: _Optional[str] = ..., https_port: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., tcp_port_secure: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., native_protocol: _Optional[str] = ..., https_uri: _Optional[str] = ..., jdbc_uri: _Optional[str] = ..., odbc_uri: _Optional[str] = ...) -> None: ...
 
+class MetricsExporterConnectionInfo(_message.Message):
+    __slots__ = ["user", "password"]
+    USER_FIELD_NUMBER: _ClassVar[int]
+    PASSWORD_FIELD_NUMBER: _ClassVar[int]
+    user: str
+    password: str
+    def __init__(self, user: _Optional[str] = ..., password: _Optional[str] = ...) -> None: ...
+
 class Host(_message.Message):
-    __slots__ = ["name", "cluster_id", "shard_name", "private_name"]
+    __slots__ = ["name", "cluster_id", "shard_name", "private_name", "status"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     CLUSTER_ID_FIELD_NUMBER: _ClassVar[int]
     SHARD_NAME_FIELD_NUMBER: _ClassVar[int]
     PRIVATE_NAME_FIELD_NUMBER: _ClassVar[int]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
     name: str
     cluster_id: str
     shard_name: str
     private_name: str
-    def __init__(self, name: _Optional[str] = ..., cluster_id: _Optional[str] = ..., shard_name: _Optional[str] = ..., private_name: _Optional[str] = ...) -> None: ...
+    status: _cluster_pb2.HostStatus
+    def __init__(self, name: _Optional[str] = ..., cluster_id: _Optional[str] = ..., shard_name: _Optional[str] = ..., private_name: _Optional[str] = ..., status: _Optional[_Union[_cluster_pb2.HostStatus, str]] = ...) -> None: ...
```

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/cluster_service_pb2.py` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/clickhouse/v1/cluster_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
@@ -17,23 +17,23 @@
 from doublecloud.clickhouse.v1 import backup_pb2 as doublecloud_dot_clickhouse_dot_v1_dot_backup__pb2
 from doublecloud.clickhouse.v1 import cluster_pb2 as doublecloud_dot_clickhouse_dot_v1_dot_cluster__pb2
 from doublecloud.clickhouse.v1 import config_pb2 as doublecloud_dot_clickhouse_dot_v1_dot_config__pb2
 from doublecloud.v1 import cluster_pb2 as doublecloud_dot_v1_dot_cluster__pb2
 from doublecloud.v1 import maintenance_pb2 as doublecloud_dot_v1_dot_maintenance__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/doublecloud/clickhouse/v1/cluster_service.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\x1a&doublecloud/clickhouse/v1/backup.proto\x1a\'doublecloud/clickhouse/v1/cluster.proto\x1a&doublecloud/clickhouse/v1/config.proto\x1a\x1c\x64oublecloud/v1/cluster.proto\x1a doublecloud/v1/maintenance.proto\"P\n\x11GetClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1c\n\tsensitive\x18\x02 \x01(\x08R\tsensitive\"\xa0\x01\n\x13ListClustersRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\x12:\n\x04view\x18\x03 \x01(\x0e\x32&.doublecloud.clickhouse.v1.ClusterViewR\x04view\"\x8d\x01\n\x14ListClustersResponse\x12>\n\x08\x63lusters\x18\x01 \x03(\x0b\x32\".doublecloud.clickhouse.v1.ClusterR\x08\x63lusters\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\xc7\x04\n\x14\x43reateClusterRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x02 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x06 \x01(\tR\x07version\x12I\n\tresources\x18\x07 \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x08 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12>\n\nencryption\x18\t \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\n \x01(\tR\tnetworkId\x12X\n\x11\x63lickhouse_config\x18\x0b \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClickhouseConfigR\x10\x63lickhouseConfig\x12P\n\x12maintenance_window\x18\x0c \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\"\xac\x03\n\x14UpdateClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x04 \x01(\tR\x07version\x12I\n\tresources\x18\x05 \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12X\n\x11\x63lickhouse_config\x18\x07 \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClickhouseConfigR\x10\x63lickhouseConfig\x12P\n\x12maintenance_window\x18\x08 \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\"5\n\x14\x44\x65leteClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"?\n\x1eResetClusterCredentialsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"h\n\x17ListClusterHostsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x88\x01\n\x18ListClusterHostsResponse\x12\x35\n\x05hosts\x18\x01 \x03(\x0b\x32\x1f.doublecloud.clickhouse.v1.HostR\x05hosts\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\xc6\x04\n\x15RestoreClusterRequest\x12\x1b\n\tbackup_id\x18\x01 \x01(\tR\x08\x62\x61\x63kupId\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x06 \x01(\tR\x07version\x12I\n\tresources\x18\x07 \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x08 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12>\n\nencryption\x18\t \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\n \x01(\tR\tnetworkId\x12X\n\x11\x63lickhouse_config\x18\x0b \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClickhouseConfigR\x10\x63lickhouseConfig\x12P\n\x12maintenance_window\x18\x0c \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\"j\n\x19ListClusterBackupsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x90\x01\n\x1aListClusterBackupsResponse\x12;\n\x07\x62\x61\x63kups\x18\x01 \x03(\x0b\x32!.doublecloud.clickhouse.v1.BackupR\x07\x62\x61\x63kups\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"4\n\x13StartClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"3\n\x12StopClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"\xd0\x01\n\x1cRescheduleMaintenanceRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12G\n\x0freschedule_type\x18\x02 \x01(\x0e\x32\x1e.doublecloud.v1.RescheduleTypeR\x0erescheduleType\x12H\n\x12\x64\x65layed_until_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x64\x65layedUntilTime\"m\n\x1cListClusterOperationsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x91\x01\n\x1dListClusterOperationsResponse\x12\x39\n\noperations\x18\x01 \x03(\x0b\x32\x19.doublecloud.v1.OperationR\noperations\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage*V\n\x0b\x43lusterView\x12\x18\n\x14\x43LUSTER_VIEW_INVALID\x10\x00\x12\x16\n\x12\x43LUSTER_VIEW_BASIC\x10\x01\x12\x15\n\x11\x43LUSTER_VIEW_FULL\x10\x02\x32\xa1\n\n\x0e\x43lusterService\x12W\n\x03Get\x12,.doublecloud.clickhouse.v1.GetClusterRequest\x1a\".doublecloud.clickhouse.v1.Cluster\x12g\n\x04List\x12..doublecloud.clickhouse.v1.ListClustersRequest\x1a/.doublecloud.clickhouse.v1.ListClustersResponse\x12T\n\x06\x43reate\x12/.doublecloud.clickhouse.v1.CreateClusterRequest\x1a\x19.doublecloud.v1.Operation\x12T\n\x06Update\x12/.doublecloud.clickhouse.v1.UpdateClusterRequest\x1a\x19.doublecloud.v1.Operation\x12T\n\x06\x44\x65lete\x12/.doublecloud.clickhouse.v1.DeleteClusterRequest\x1a\x19.doublecloud.v1.Operation\x12h\n\x10ResetCredentials\x12\x39.doublecloud.clickhouse.v1.ResetClusterCredentialsRequest\x1a\x19.doublecloud.v1.Operation\x12t\n\tListHosts\x12\x32.doublecloud.clickhouse.v1.ListClusterHostsRequest\x1a\x33.doublecloud.clickhouse.v1.ListClusterHostsResponse\x12V\n\x07Restore\x12\x30.doublecloud.clickhouse.v1.RestoreClusterRequest\x1a\x19.doublecloud.v1.Operation\x12z\n\x0bListBackups\x12\x34.doublecloud.clickhouse.v1.ListClusterBackupsRequest\x1a\x35.doublecloud.clickhouse.v1.ListClusterBackupsResponse\x12R\n\x05Start\x12..doublecloud.clickhouse.v1.StartClusterRequest\x1a\x19.doublecloud.v1.Operation\x12P\n\x04Stop\x12-.doublecloud.clickhouse.v1.StopClusterRequest\x1a\x19.doublecloud.v1.Operation\x12k\n\x15RescheduleMaintenance\x12\x37.doublecloud.clickhouse.v1.RescheduleMaintenanceRequest\x1a\x19.doublecloud.v1.Operation\x12\x83\x01\n\x0eListOperations\x12\x37.doublecloud.clickhouse.v1.ListClusterOperationsRequest\x1a\x38.doublecloud.clickhouse.v1.ListClusterOperationsResponseBAZ?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/doublecloud/clickhouse/v1/cluster_service.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\x1a&doublecloud/clickhouse/v1/backup.proto\x1a\'doublecloud/clickhouse/v1/cluster.proto\x1a&doublecloud/clickhouse/v1/config.proto\x1a\x1c\x64oublecloud/v1/cluster.proto\x1a doublecloud/v1/maintenance.proto\"P\n\x11GetClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1c\n\tsensitive\x18\x02 \x01(\x08R\tsensitive\"\xa0\x01\n\x13ListClustersRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\x12:\n\x04view\x18\x03 \x01(\x0e\x32&.doublecloud.clickhouse.v1.ClusterViewR\x04view\"\x8d\x01\n\x14ListClustersResponse\x12>\n\x08\x63lusters\x18\x01 \x03(\x0b\x32\".doublecloud.clickhouse.v1.ClusterR\x08\x63lusters\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\xc7\x04\n\x14\x43reateClusterRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x02 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x06 \x01(\tR\x07version\x12I\n\tresources\x18\x07 \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x08 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12>\n\nencryption\x18\t \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\n \x01(\tR\tnetworkId\x12X\n\x11\x63lickhouse_config\x18\x0b \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClickhouseConfigR\x10\x63lickhouseConfig\x12P\n\x12maintenance_window\x18\x0c \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\"\xac\x03\n\x14UpdateClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x04 \x01(\tR\x07version\x12I\n\tresources\x18\x05 \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12X\n\x11\x63lickhouse_config\x18\x07 \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClickhouseConfigR\x10\x63lickhouseConfig\x12P\n\x12maintenance_window\x18\x08 \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\"5\n\x14\x44\x65leteClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"?\n\x1eResetClusterCredentialsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"h\n\x17ListClusterHostsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x88\x01\n\x18ListClusterHostsResponse\x12\x35\n\x05hosts\x18\x01 \x03(\x0b\x32\x1f.doublecloud.clickhouse.v1.HostR\x05hosts\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\xc6\x04\n\x15RestoreClusterRequest\x12\x1b\n\tbackup_id\x18\x01 \x01(\tR\x08\x62\x61\x63kupId\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x06 \x01(\tR\x07version\x12I\n\tresources\x18\x07 \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x08 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12>\n\nencryption\x18\t \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\n \x01(\tR\tnetworkId\x12X\n\x11\x63lickhouse_config\x18\x0b \x01(\x0b\x32+.doublecloud.clickhouse.v1.ClickhouseConfigR\x10\x63lickhouseConfig\x12P\n\x12maintenance_window\x18\x0c \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\"j\n\x19ListClusterBackupsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x90\x01\n\x1aListClusterBackupsResponse\x12;\n\x07\x62\x61\x63kups\x18\x01 \x03(\x0b\x32!.doublecloud.clickhouse.v1.BackupR\x07\x62\x61\x63kups\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"4\n\x13StartClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"3\n\x12StopClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"\xd0\x01\n\x1cRescheduleMaintenanceRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12G\n\x0freschedule_type\x18\x02 \x01(\x0e\x32\x1e.doublecloud.v1.RescheduleTypeR\x0erescheduleType\x12H\n\x12\x64\x65layed_until_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x64\x65layedUntilTime\"m\n\x1cListClusterOperationsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x91\x01\n\x1dListClusterOperationsResponse\x12\x39\n\noperations\x18\x01 \x03(\x0b\x32\x19.doublecloud.v1.OperationR\noperations\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage*V\n\x0b\x43lusterView\x12\x18\n\x14\x43LUSTER_VIEW_INVALID\x10\x00\x12\x16\n\x12\x43LUSTER_VIEW_BASIC\x10\x01\x12\x15\n\x11\x43LUSTER_VIEW_FULL\x10\x02\x32\xa1\n\n\x0e\x43lusterService\x12W\n\x03Get\x12,.doublecloud.clickhouse.v1.GetClusterRequest\x1a\".doublecloud.clickhouse.v1.Cluster\x12g\n\x04List\x12..doublecloud.clickhouse.v1.ListClustersRequest\x1a/.doublecloud.clickhouse.v1.ListClustersResponse\x12T\n\x06\x43reate\x12/.doublecloud.clickhouse.v1.CreateClusterRequest\x1a\x19.doublecloud.v1.Operation\x12T\n\x06Update\x12/.doublecloud.clickhouse.v1.UpdateClusterRequest\x1a\x19.doublecloud.v1.Operation\x12T\n\x06\x44\x65lete\x12/.doublecloud.clickhouse.v1.DeleteClusterRequest\x1a\x19.doublecloud.v1.Operation\x12h\n\x10ResetCredentials\x12\x39.doublecloud.clickhouse.v1.ResetClusterCredentialsRequest\x1a\x19.doublecloud.v1.Operation\x12t\n\tListHosts\x12\x32.doublecloud.clickhouse.v1.ListClusterHostsRequest\x1a\x33.doublecloud.clickhouse.v1.ListClusterHostsResponse\x12V\n\x07Restore\x12\x30.doublecloud.clickhouse.v1.RestoreClusterRequest\x1a\x19.doublecloud.v1.Operation\x12z\n\x0bListBackups\x12\x34.doublecloud.clickhouse.v1.ListClusterBackupsRequest\x1a\x35.doublecloud.clickhouse.v1.ListClusterBackupsResponse\x12R\n\x05Start\x12..doublecloud.clickhouse.v1.StartClusterRequest\x1a\x19.doublecloud.v1.Operation\x12P\n\x04Stop\x12-.doublecloud.clickhouse.v1.StopClusterRequest\x1a\x19.doublecloud.v1.Operation\x12k\n\x15RescheduleMaintenance\x12\x37.doublecloud.clickhouse.v1.RescheduleMaintenanceRequest\x1a\x19.doublecloud.v1.Operation\x12\x83\x01\n\x0eListOperations\x12\x37.doublecloud.clickhouse.v1.ListClusterOperationsRequest\x1a\x38.doublecloud.clickhouse.v1.ListClusterOperationsResponseBIZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.clickhouse.v1.cluster_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouse'
+  DESCRIPTOR._serialized_options = b'ZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouse'
   _globals['_CLUSTERVIEW']._serialized_start=3545
   _globals['_CLUSTERVIEW']._serialized_end=3631
   _globals['_GETCLUSTERREQUEST']._serialized_start=357
   _globals['_GETCLUSTERREQUEST']._serialized_end=437
   _globals['_LISTCLUSTERSREQUEST']._serialized_start=440
   _globals['_LISTCLUSTERSREQUEST']._serialized_end=600
   _globals['_LISTCLUSTERSRESPONSE']._serialized_start=603
```

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/cluster_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/config_pb2.py` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/config_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/clickhouse/v1/config.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&doublecloud/clickhouse/v1/config.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xf1+\n\x10\x43lickhouseConfig\x12Q\n\tlog_level\x18\x01 \x01(\x0e\x32\x34.doublecloud.clickhouse.v1.ClickhouseConfig.LogLevelR\x08logLevel\x12\x44\n\x0fmax_connections\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0emaxConnections\x12Q\n\x16max_concurrent_queries\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x14maxConcurrentQueries\x12G\n\x12keep_alive_timeout\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10keepAliveTimeout\x12S\n\x17uncompressed_cache_size\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x15uncompressedCacheSize\x12\x43\n\x0fmark_cache_size\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\rmarkCacheSize\x12O\n\x16max_table_size_to_drop\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12maxTableSizeToDrop\x12W\n\x1amax_partition_size_to_drop\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x16maxPartitionSizeToDrop\x12\x38\n\x08timezone\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08timezone\x12M\n\x14\x62\x61\x63kground_pool_size\x18\n \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12\x62\x61\x63kgroundPoolSize\x12^\n\x1d\x62\x61\x63kground_schedule_pool_size\x18\x0b \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1a\x62\x61\x63kgroundSchedulePoolSize\x12\\\n\x1c\x62\x61\x63kground_fetches_pool_size\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x19\x62\x61\x63kgroundFetchesPoolSize\x12V\n\x19\x62\x61\x63kground_move_pool_size\x18\r \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x16\x62\x61\x63kgroundMovePoolSize\x12Z\n\x1b\x62\x61\x63kground_common_pool_size\x18\x0e \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x18\x62\x61\x63kgroundCommonPoolSize\x12}\n-background_merges_mutations_concurrency_ratio\x18\x0f \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR)backgroundMergesMutationsConcurrencyRatio\x12X\n\x1atotal_memory_profiler_step\x18\x10 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x17totalMemoryProfilerStep\x12r\n\'total_memory_tracker_sample_probability\x18\x17 \x01(\x0b\x32\x1c.google.protobuf.DoubleValueR#totalMemoryTrackerSampleProbability\x12T\n\nmerge_tree\x18\x11 \x01(\x0b\x32\x35.doublecloud.clickhouse.v1.ClickhouseConfig.MergeTreeR\tmergeTree\x12Y\n\x0b\x63ompression\x18\x12 \x03(\x0b\x32\x37.doublecloud.clickhouse.v1.ClickhouseConfig.CompressionR\x0b\x63ompression\x12h\n\x0fgraphite_rollup\x18\x13 \x03(\x0b\x32?.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollupEntryR\x0egraphiteRollup\x12G\n\x05kafka\x18\x14 \x01(\x0b\x32\x31.doublecloud.clickhouse.v1.ClickhouseConfig.KafkaR\x05kafka\x12_\n\x0ckafka_topics\x18\x15 \x03(\x0b\x32<.doublecloud.clickhouse.v1.ClickhouseConfig.KafkaTopicsEntryR\x0bkafkaTopics\x12P\n\x08rabbitmq\x18\x16 \x01(\x0b\x32\x34.doublecloud.clickhouse.v1.ClickhouseConfig.RabbitmqR\x08rabbitmq\x1a\xab\x0c\n\tMergeTree\x12\x63\n\x1freplicated_deduplication_window\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1dreplicatedDeduplicationWindow\x12p\n\'replicated_deduplication_window_seconds\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR$replicatedDeduplicationWindowSeconds\x12N\n\x15parts_to_delay_insert\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12partsToDelayInsert\x12N\n\x15parts_to_throw_insert\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12partsToThrowInsert\x12_\n\x1einactive_parts_to_delay_insert\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1ainactivePartsToDelayInsert\x12_\n\x1einactive_parts_to_throw_insert\x18\r \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1ainactivePartsToThrowInsert\x12_\n\x1emax_replicated_merges_in_queue\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1amaxReplicatedMergesInQueue\x12\x8e\x01\n9number_of_free_entries_in_pool_to_lower_max_size_of_merge\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR.numberOfFreeEntriesInPoolToLowerMaxSizeOfMerge\x12m\n\'max_bytes_to_merge_at_min_space_in_pool\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1fmaxBytesToMergeAtMinSpaceInPool\x12m\n\'max_bytes_to_merge_at_max_space_in_pool\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1fmaxBytesToMergeAtMaxSpaceInPool\x12Q\n\x17min_bytes_for_wide_part\x18\t \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x13minBytesForWidePart\x12O\n\x16min_rows_for_wide_part\x18\n \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12minRowsForWidePart\x12I\n\x13ttl_only_drop_parts\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x10ttlOnlyDropParts\x12N\n\x16merge_with_ttl_timeout\x18\x0f \x01(\x0b\x32\x19.google.protobuf.DurationR\x13mergeWithTtlTimeout\x12i\n$merge_with_recompression_ttl_timeout\x18\x10 \x01(\x0b\x32\x19.google.protobuf.DurationR mergeWithRecompressionTtlTimeout\x12k\n%allow_remote_fs_zero_copy_replication\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.BoolValueR allowRemoteFsZeroCopyReplication\x1a\xc3\x05\n\x05Kafka\x12o\n\x11security_protocol\x18\x01 \x01(\x0e\x32\x42.doublecloud.clickhouse.v1.ClickhouseConfig.Kafka.SecurityProtocolR\x10securityProtocol\x12\x66\n\x0esasl_mechanism\x18\x02 \x01(\x0e\x32?.doublecloud.clickhouse.v1.ClickhouseConfig.Kafka.SaslMechanismR\rsaslMechanism\x12\x41\n\rsasl_username\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0csaslUsername\x12\x41\n\rsasl_password\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0csaslPassword\"\xb3\x01\n\x10SecurityProtocol\x12\x1d\n\x19SECURITY_PROTOCOL_INVALID\x10\x00\x12\x1f\n\x1bSECURITY_PROTOCOL_PLAINTEXT\x10\x01\x12\x19\n\x15SECURITY_PROTOCOL_SSL\x10\x02\x12$\n SECURITY_PROTOCOL_SASL_PLAINTEXT\x10\x03\x12\x1e\n\x1aSECURITY_PROTOCOL_SASL_SSL\x10\x04\"\xa4\x01\n\rSaslMechanism\x12\x1a\n\x16SASL_MECHANISM_INVALID\x10\x00\x12\x19\n\x15SASL_MECHANISM_GSSAPI\x10\x01\x12\x18\n\x14SASL_MECHANISM_PLAIN\x10\x02\x12 \n\x1cSASL_MECHANISM_SCRAM_SHA_256\x10\x03\x12 \n\x1cSASL_MECHANISM_SCRAM_SHA_512\x10\x04\x1a\xb2\x01\n\x08Rabbitmq\x12\x38\n\x08username\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08username\x12\x38\n\x08password\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08password\x12\x32\n\x05vhost\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x05vhost\x1a\xbc\x02\n\x0b\x43ompression\x12V\n\x06method\x18\x01 \x01(\x0e\x32>.doublecloud.clickhouse.v1.ClickhouseConfig.Compression.MethodR\x06method\x12\"\n\rmin_part_size\x18\x02 \x01(\x03R\x0bminPartSize\x12-\n\x13min_part_size_ratio\x18\x03 \x01(\x01R\x10minPartSizeRatio\x12\x31\n\x05level\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x05level\"O\n\x06Method\x12\x12\n\x0eMETHOD_INVALID\x10\x00\x12\x0e\n\nMETHOD_LZ4\x10\x01\x12\x0f\n\x0bMETHOD_ZSTD\x10\x02\x12\x10\n\x0cMETHOD_LZ4HC\x10\x03\x1a\x95\x03\n\x0eGraphiteRollup\x12^\n\x08patterns\x18\x01 \x03(\x0b\x32\x42.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollup.PatternR\x08patterns\x1a\xa2\x02\n\x07Pattern\x12\x34\n\x06regexp\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x06regexp\x12\x38\n\x08\x66unction\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08\x66unction\x12j\n\tretention\x18\x03 \x03(\x0b\x32L.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollup.Pattern.RetentionR\tretention\x1a;\n\tRetention\x12\x10\n\x03\x61ge\x18\x01 \x01(\x03R\x03\x61ge\x12\x1c\n\tprecision\x18\x02 \x01(\x03R\tprecision\x1a}\n\x13GraphiteRollupEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12P\n\x05value\x18\x02 \x01(\x0b\x32:.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollupR\x05value:\x02\x38\x01\x1aq\n\x10KafkaTopicsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12G\n\x05value\x18\x02 \x01(\x0b\x32\x31.doublecloud.clickhouse.v1.ClickhouseConfig.KafkaR\x05value:\x02\x38\x01\"\x92\x01\n\x08LogLevel\x12\x15\n\x11LOG_LEVEL_INVALID\x10\x00\x12\x13\n\x0fLOG_LEVEL_TRACE\x10\x01\x12\x13\n\x0fLOG_LEVEL_DEBUG\x10\x02\x12\x19\n\x15LOG_LEVEL_INFORMATION\x10\x03\x12\x15\n\x11LOG_LEVEL_WARNING\x10\x04\x12\x13\n\x0fLOG_LEVEL_ERROR\x10\x05\x42\x41Z?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&doublecloud/clickhouse/v1/config.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xdc,\n\x10\x43lickhouseConfig\x12Q\n\tlog_level\x18\x01 \x01(\x0e\x32\x34.doublecloud.clickhouse.v1.ClickhouseConfig.LogLevelR\x08logLevel\x12\x44\n\x0fmax_connections\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0emaxConnections\x12Q\n\x16max_concurrent_queries\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x14maxConcurrentQueries\x12G\n\x12keep_alive_timeout\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x10keepAliveTimeout\x12S\n\x17uncompressed_cache_size\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x15uncompressedCacheSize\x12\x43\n\x0fmark_cache_size\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\rmarkCacheSize\x12O\n\x16max_table_size_to_drop\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12maxTableSizeToDrop\x12W\n\x1amax_partition_size_to_drop\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x16maxPartitionSizeToDrop\x12\x38\n\x08timezone\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08timezone\x12M\n\x14\x62\x61\x63kground_pool_size\x18\n \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12\x62\x61\x63kgroundPoolSize\x12^\n\x1d\x62\x61\x63kground_schedule_pool_size\x18\x0b \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1a\x62\x61\x63kgroundSchedulePoolSize\x12\\\n\x1c\x62\x61\x63kground_fetches_pool_size\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x19\x62\x61\x63kgroundFetchesPoolSize\x12V\n\x19\x62\x61\x63kground_move_pool_size\x18\r \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x16\x62\x61\x63kgroundMovePoolSize\x12Z\n\x1b\x62\x61\x63kground_common_pool_size\x18\x0e \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x18\x62\x61\x63kgroundCommonPoolSize\x12}\n-background_merges_mutations_concurrency_ratio\x18\x0f \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR)backgroundMergesMutationsConcurrencyRatio\x12X\n\x1atotal_memory_profiler_step\x18\x10 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x17totalMemoryProfilerStep\x12r\n\'total_memory_tracker_sample_probability\x18\x17 \x01(\x0b\x32\x1c.google.protobuf.DoubleValueR#totalMemoryTrackerSampleProbability\x12T\n\nmerge_tree\x18\x11 \x01(\x0b\x32\x35.doublecloud.clickhouse.v1.ClickhouseConfig.MergeTreeR\tmergeTree\x12Y\n\x0b\x63ompression\x18\x12 \x03(\x0b\x32\x37.doublecloud.clickhouse.v1.ClickhouseConfig.CompressionR\x0b\x63ompression\x12h\n\x0fgraphite_rollup\x18\x13 \x03(\x0b\x32?.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollupEntryR\x0egraphiteRollup\x12G\n\x05kafka\x18\x14 \x01(\x0b\x32\x31.doublecloud.clickhouse.v1.ClickhouseConfig.KafkaR\x05kafka\x12_\n\x0ckafka_topics\x18\x15 \x03(\x0b\x32<.doublecloud.clickhouse.v1.ClickhouseConfig.KafkaTopicsEntryR\x0bkafkaTopics\x12P\n\x08rabbitmq\x18\x16 \x01(\x0b\x32\x34.doublecloud.clickhouse.v1.ClickhouseConfig.RabbitmqR\x08rabbitmq\x1a\xab\x0c\n\tMergeTree\x12\x63\n\x1freplicated_deduplication_window\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1dreplicatedDeduplicationWindow\x12p\n\'replicated_deduplication_window_seconds\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR$replicatedDeduplicationWindowSeconds\x12N\n\x15parts_to_delay_insert\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12partsToDelayInsert\x12N\n\x15parts_to_throw_insert\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12partsToThrowInsert\x12_\n\x1einactive_parts_to_delay_insert\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1ainactivePartsToDelayInsert\x12_\n\x1einactive_parts_to_throw_insert\x18\r \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1ainactivePartsToThrowInsert\x12_\n\x1emax_replicated_merges_in_queue\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1amaxReplicatedMergesInQueue\x12\x8e\x01\n9number_of_free_entries_in_pool_to_lower_max_size_of_merge\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR.numberOfFreeEntriesInPoolToLowerMaxSizeOfMerge\x12m\n\'max_bytes_to_merge_at_min_space_in_pool\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1fmaxBytesToMergeAtMinSpaceInPool\x12m\n\'max_bytes_to_merge_at_max_space_in_pool\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x1fmaxBytesToMergeAtMaxSpaceInPool\x12Q\n\x17min_bytes_for_wide_part\x18\t \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x13minBytesForWidePart\x12O\n\x16min_rows_for_wide_part\x18\n \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x12minRowsForWidePart\x12I\n\x13ttl_only_drop_parts\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x10ttlOnlyDropParts\x12N\n\x16merge_with_ttl_timeout\x18\x0f \x01(\x0b\x32\x19.google.protobuf.DurationR\x13mergeWithTtlTimeout\x12i\n$merge_with_recompression_ttl_timeout\x18\x10 \x01(\x0b\x32\x19.google.protobuf.DurationR mergeWithRecompressionTtlTimeout\x12k\n%allow_remote_fs_zero_copy_replication\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.BoolValueR allowRemoteFsZeroCopyReplication\x1a\xae\x06\n\x05Kafka\x12o\n\x11security_protocol\x18\x01 \x01(\x0e\x32\x42.doublecloud.clickhouse.v1.ClickhouseConfig.Kafka.SecurityProtocolR\x10securityProtocol\x12\x66\n\x0esasl_mechanism\x18\x02 \x01(\x0e\x32?.doublecloud.clickhouse.v1.ClickhouseConfig.Kafka.SaslMechanismR\rsaslMechanism\x12\x41\n\rsasl_username\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0csaslUsername\x12\x41\n\rsasl_password\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0csaslPassword\x12i\n#enable_ssl_certificate_verification\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR enableSslCertificateVerification\"\xb3\x01\n\x10SecurityProtocol\x12\x1d\n\x19SECURITY_PROTOCOL_INVALID\x10\x00\x12\x1f\n\x1bSECURITY_PROTOCOL_PLAINTEXT\x10\x01\x12\x19\n\x15SECURITY_PROTOCOL_SSL\x10\x02\x12$\n SECURITY_PROTOCOL_SASL_PLAINTEXT\x10\x03\x12\x1e\n\x1aSECURITY_PROTOCOL_SASL_SSL\x10\x04\"\xa4\x01\n\rSaslMechanism\x12\x1a\n\x16SASL_MECHANISM_INVALID\x10\x00\x12\x19\n\x15SASL_MECHANISM_GSSAPI\x10\x01\x12\x18\n\x14SASL_MECHANISM_PLAIN\x10\x02\x12 \n\x1cSASL_MECHANISM_SCRAM_SHA_256\x10\x03\x12 \n\x1cSASL_MECHANISM_SCRAM_SHA_512\x10\x04\x1a\xb2\x01\n\x08Rabbitmq\x12\x38\n\x08username\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08username\x12\x38\n\x08password\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08password\x12\x32\n\x05vhost\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x05vhost\x1a\xbc\x02\n\x0b\x43ompression\x12V\n\x06method\x18\x01 \x01(\x0e\x32>.doublecloud.clickhouse.v1.ClickhouseConfig.Compression.MethodR\x06method\x12\"\n\rmin_part_size\x18\x02 \x01(\x03R\x0bminPartSize\x12-\n\x13min_part_size_ratio\x18\x03 \x01(\x01R\x10minPartSizeRatio\x12\x31\n\x05level\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x05level\"O\n\x06Method\x12\x12\n\x0eMETHOD_INVALID\x10\x00\x12\x0e\n\nMETHOD_LZ4\x10\x01\x12\x0f\n\x0bMETHOD_ZSTD\x10\x02\x12\x10\n\x0cMETHOD_LZ4HC\x10\x03\x1a\x95\x03\n\x0eGraphiteRollup\x12^\n\x08patterns\x18\x01 \x03(\x0b\x32\x42.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollup.PatternR\x08patterns\x1a\xa2\x02\n\x07Pattern\x12\x34\n\x06regexp\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x06regexp\x12\x38\n\x08\x66unction\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08\x66unction\x12j\n\tretention\x18\x03 \x03(\x0b\x32L.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollup.Pattern.RetentionR\tretention\x1a;\n\tRetention\x12\x10\n\x03\x61ge\x18\x01 \x01(\x03R\x03\x61ge\x12\x1c\n\tprecision\x18\x02 \x01(\x03R\tprecision\x1a}\n\x13GraphiteRollupEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12P\n\x05value\x18\x02 \x01(\x0b\x32:.doublecloud.clickhouse.v1.ClickhouseConfig.GraphiteRollupR\x05value:\x02\x38\x01\x1aq\n\x10KafkaTopicsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12G\n\x05value\x18\x02 \x01(\x0b\x32\x31.doublecloud.clickhouse.v1.ClickhouseConfig.KafkaR\x05value:\x02\x38\x01\"\x92\x01\n\x08LogLevel\x12\x15\n\x11LOG_LEVEL_INVALID\x10\x00\x12\x13\n\x0fLOG_LEVEL_TRACE\x10\x01\x12\x13\n\x0fLOG_LEVEL_DEBUG\x10\x02\x12\x19\n\x15LOG_LEVEL_INFORMATION\x10\x03\x12\x15\n\x11LOG_LEVEL_WARNING\x10\x04\x12\x13\n\x0fLOG_LEVEL_ERROR\x10\x05\x42IZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.clickhouse.v1.config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouse'
+  DESCRIPTOR._serialized_options = b'ZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouse'
   _CLICKHOUSECONFIG_GRAPHITEROLLUPENTRY._options = None
   _CLICKHOUSECONFIG_GRAPHITEROLLUPENTRY._serialized_options = b'8\001'
   _CLICKHOUSECONFIG_KAFKATOPICSENTRY._options = None
   _CLICKHOUSECONFIG_KAFKATOPICSENTRY._serialized_options = b'8\001'
   _globals['_CLICKHOUSECONFIG']._serialized_start=134
-  _globals['_CLICKHOUSECONFIG']._serialized_end=5751
+  _globals['_CLICKHOUSECONFIG']._serialized_end=5858
   _globals['_CLICKHOUSECONFIG_MERGETREE']._serialized_start=2163
   _globals['_CLICKHOUSECONFIG_MERGETREE']._serialized_end=3742
   _globals['_CLICKHOUSECONFIG_KAFKA']._serialized_start=3745
-  _globals['_CLICKHOUSECONFIG_KAFKA']._serialized_end=4452
-  _globals['_CLICKHOUSECONFIG_KAFKA_SECURITYPROTOCOL']._serialized_start=4106
-  _globals['_CLICKHOUSECONFIG_KAFKA_SECURITYPROTOCOL']._serialized_end=4285
-  _globals['_CLICKHOUSECONFIG_KAFKA_SASLMECHANISM']._serialized_start=4288
-  _globals['_CLICKHOUSECONFIG_KAFKA_SASLMECHANISM']._serialized_end=4452
-  _globals['_CLICKHOUSECONFIG_RABBITMQ']._serialized_start=4455
-  _globals['_CLICKHOUSECONFIG_RABBITMQ']._serialized_end=4633
-  _globals['_CLICKHOUSECONFIG_COMPRESSION']._serialized_start=4636
-  _globals['_CLICKHOUSECONFIG_COMPRESSION']._serialized_end=4952
-  _globals['_CLICKHOUSECONFIG_COMPRESSION_METHOD']._serialized_start=4873
-  _globals['_CLICKHOUSECONFIG_COMPRESSION_METHOD']._serialized_end=4952
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP']._serialized_start=4955
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP']._serialized_end=5360
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN']._serialized_start=5070
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN']._serialized_end=5360
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN_RETENTION']._serialized_start=5301
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN_RETENTION']._serialized_end=5360
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUPENTRY']._serialized_start=5362
-  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUPENTRY']._serialized_end=5487
-  _globals['_CLICKHOUSECONFIG_KAFKATOPICSENTRY']._serialized_start=5489
-  _globals['_CLICKHOUSECONFIG_KAFKATOPICSENTRY']._serialized_end=5602
-  _globals['_CLICKHOUSECONFIG_LOGLEVEL']._serialized_start=5605
-  _globals['_CLICKHOUSECONFIG_LOGLEVEL']._serialized_end=5751
+  _globals['_CLICKHOUSECONFIG_KAFKA']._serialized_end=4559
+  _globals['_CLICKHOUSECONFIG_KAFKA_SECURITYPROTOCOL']._serialized_start=4213
+  _globals['_CLICKHOUSECONFIG_KAFKA_SECURITYPROTOCOL']._serialized_end=4392
+  _globals['_CLICKHOUSECONFIG_KAFKA_SASLMECHANISM']._serialized_start=4395
+  _globals['_CLICKHOUSECONFIG_KAFKA_SASLMECHANISM']._serialized_end=4559
+  _globals['_CLICKHOUSECONFIG_RABBITMQ']._serialized_start=4562
+  _globals['_CLICKHOUSECONFIG_RABBITMQ']._serialized_end=4740
+  _globals['_CLICKHOUSECONFIG_COMPRESSION']._serialized_start=4743
+  _globals['_CLICKHOUSECONFIG_COMPRESSION']._serialized_end=5059
+  _globals['_CLICKHOUSECONFIG_COMPRESSION_METHOD']._serialized_start=4980
+  _globals['_CLICKHOUSECONFIG_COMPRESSION_METHOD']._serialized_end=5059
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP']._serialized_start=5062
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP']._serialized_end=5467
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN']._serialized_start=5177
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN']._serialized_end=5467
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN_RETENTION']._serialized_start=5408
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUP_PATTERN_RETENTION']._serialized_end=5467
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUPENTRY']._serialized_start=5469
+  _globals['_CLICKHOUSECONFIG_GRAPHITEROLLUPENTRY']._serialized_end=5594
+  _globals['_CLICKHOUSECONFIG_KAFKATOPICSENTRY']._serialized_start=5596
+  _globals['_CLICKHOUSECONFIG_KAFKATOPICSENTRY']._serialized_end=5709
+  _globals['_CLICKHOUSECONFIG_LOGLEVEL']._serialized_start=5712
+  _globals['_CLICKHOUSECONFIG_LOGLEVEL']._serialized_end=5858
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/config_pb2.pyi` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/config_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         min_rows_for_wide_part: _wrappers_pb2.Int64Value
         ttl_only_drop_parts: _wrappers_pb2.BoolValue
         merge_with_ttl_timeout: _duration_pb2.Duration
         merge_with_recompression_ttl_timeout: _duration_pb2.Duration
         allow_remote_fs_zero_copy_replication: _wrappers_pb2.BoolValue
         def __init__(self, replicated_deduplication_window: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., replicated_deduplication_window_seconds: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., parts_to_delay_insert: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., parts_to_throw_insert: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., inactive_parts_to_delay_insert: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., inactive_parts_to_throw_insert: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_replicated_merges_in_queue: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., number_of_free_entries_in_pool_to_lower_max_size_of_merge: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_bytes_to_merge_at_min_space_in_pool: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., max_bytes_to_merge_at_max_space_in_pool: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., min_bytes_for_wide_part: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., min_rows_for_wide_part: _Optional[_Union[_wrappers_pb2.Int64Value, _Mapping]] = ..., ttl_only_drop_parts: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ..., merge_with_ttl_timeout: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., merge_with_recompression_ttl_timeout: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., allow_remote_fs_zero_copy_replication: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
     class Kafka(_message.Message):
-        __slots__ = ["security_protocol", "sasl_mechanism", "sasl_username", "sasl_password"]
+        __slots__ = ["security_protocol", "sasl_mechanism", "sasl_username", "sasl_password", "enable_ssl_certificate_verification"]
         class SecurityProtocol(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
             __slots__ = []
             SECURITY_PROTOCOL_INVALID: _ClassVar[ClickhouseConfig.Kafka.SecurityProtocol]
             SECURITY_PROTOCOL_PLAINTEXT: _ClassVar[ClickhouseConfig.Kafka.SecurityProtocol]
             SECURITY_PROTOCOL_SSL: _ClassVar[ClickhouseConfig.Kafka.SecurityProtocol]
             SECURITY_PROTOCOL_SASL_PLAINTEXT: _ClassVar[ClickhouseConfig.Kafka.SecurityProtocol]
             SECURITY_PROTOCOL_SASL_SSL: _ClassVar[ClickhouseConfig.Kafka.SecurityProtocol]
@@ -85,19 +85,21 @@
         SASL_MECHANISM_PLAIN: ClickhouseConfig.Kafka.SaslMechanism
         SASL_MECHANISM_SCRAM_SHA_256: ClickhouseConfig.Kafka.SaslMechanism
         SASL_MECHANISM_SCRAM_SHA_512: ClickhouseConfig.Kafka.SaslMechanism
         SECURITY_PROTOCOL_FIELD_NUMBER: _ClassVar[int]
         SASL_MECHANISM_FIELD_NUMBER: _ClassVar[int]
         SASL_USERNAME_FIELD_NUMBER: _ClassVar[int]
         SASL_PASSWORD_FIELD_NUMBER: _ClassVar[int]
+        ENABLE_SSL_CERTIFICATE_VERIFICATION_FIELD_NUMBER: _ClassVar[int]
         security_protocol: ClickhouseConfig.Kafka.SecurityProtocol
         sasl_mechanism: ClickhouseConfig.Kafka.SaslMechanism
         sasl_username: _wrappers_pb2.StringValue
         sasl_password: _wrappers_pb2.StringValue
-        def __init__(self, security_protocol: _Optional[_Union[ClickhouseConfig.Kafka.SecurityProtocol, str]] = ..., sasl_mechanism: _Optional[_Union[ClickhouseConfig.Kafka.SaslMechanism, str]] = ..., sasl_username: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., sasl_password: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ...) -> None: ...
+        enable_ssl_certificate_verification: _wrappers_pb2.BoolValue
+        def __init__(self, security_protocol: _Optional[_Union[ClickhouseConfig.Kafka.SecurityProtocol, str]] = ..., sasl_mechanism: _Optional[_Union[ClickhouseConfig.Kafka.SaslMechanism, str]] = ..., sasl_username: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., sasl_password: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., enable_ssl_certificate_verification: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
     class Rabbitmq(_message.Message):
         __slots__ = ["username", "password", "vhost"]
         USERNAME_FIELD_NUMBER: _ClassVar[int]
         PASSWORD_FIELD_NUMBER: _ClassVar[int]
         VHOST_FIELD_NUMBER: _ClassVar[int]
         username: _wrappers_pb2.StringValue
         password: _wrappers_pb2.StringValue
```

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/operation_service_pb2.py` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/operation_service_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/clickhouse/v1/operation_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n1doublecloud/clickhouse/v1/operation_service.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"8\n\x13GetOperationRequest\x12!\n\x0coperation_id\x18\x01 \x01(\tR\x0boperationId\"f\n\x15ListOperationsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x8a\x01\n\x16ListOperationsResponse\x12\x39\n\noperations\x18\x01 \x03(\x0b\x32\x19.doublecloud.v1.OperationR\noperations\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage2\xd1\x01\n\x10OperationService\x12P\n\x03Get\x12..doublecloud.clickhouse.v1.GetOperationRequest\x1a\x19.doublecloud.v1.Operation\x12k\n\x04List\x12\x30.doublecloud.clickhouse.v1.ListOperationsRequest\x1a\x31.doublecloud.clickhouse.v1.ListOperationsResponseBAZ?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n1doublecloud/clickhouse/v1/operation_service.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"8\n\x13GetOperationRequest\x12!\n\x0coperation_id\x18\x01 \x01(\tR\x0boperationId\"f\n\x15ListOperationsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x8a\x01\n\x16ListOperationsResponse\x12\x39\n\noperations\x18\x01 \x03(\x0b\x32\x19.doublecloud.v1.OperationR\noperations\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage2\xd1\x01\n\x10OperationService\x12P\n\x03Get\x12..doublecloud.clickhouse.v1.GetOperationRequest\x1a\x19.doublecloud.v1.Operation\x12k\n\x04List\x12\x30.doublecloud.clickhouse.v1.ListOperationsRequest\x1a\x31.doublecloud.clickhouse.v1.ListOperationsResponseBIZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.clickhouse.v1.operation_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouse'
+  DESCRIPTOR._serialized_options = b'ZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouse'
   _globals['_GETOPERATIONREQUEST']._serialized_start=141
   _globals['_GETOPERATIONREQUEST']._serialized_end=197
   _globals['_LISTOPERATIONSREQUEST']._serialized_start=199
   _globals['_LISTOPERATIONSREQUEST']._serialized_end=301
   _globals['_LISTOPERATIONSRESPONSE']._serialized_start=304
   _globals['_LISTOPERATIONSRESPONSE']._serialized_end=442
   _globals['_OPERATIONSERVICE']._serialized_start=445
```

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/operation_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/version_pb2.py` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/version_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/clickhouse/v1/version.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'doublecloud/clickhouse/v1/version.proto\x12\x19\x64oublecloud.clickhouse.v1\"p\n\x07Version\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1e\n\ndeprecated\x18\x03 \x01(\x08R\ndeprecated\x12!\n\x0cupdatable_to\x18\x04 \x03(\tR\x0bupdatableToBAZ?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'doublecloud/clickhouse/v1/version.proto\x12\x19\x64oublecloud.clickhouse.v1\"p\n\x07Version\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1e\n\ndeprecated\x18\x03 \x01(\x08R\ndeprecated\x12!\n\x0cupdatable_to\x18\x04 \x03(\tR\x0bupdatableToBIZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.clickhouse.v1.version_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouse'
+  DESCRIPTOR._serialized_options = b'ZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouse'
   _globals['_VERSION']._serialized_start=70
   _globals['_VERSION']._serialized_end=182
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/version_pb2.pyi` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/version_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/version_service_pb2.py` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/version_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/clickhouse/v1/version_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 from doublecloud.clickhouse.v1 import version_pb2 as doublecloud_dot_clickhouse_dot_v1_dot_version__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/doublecloud/clickhouse/v1/version_service.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1b\x64oublecloud/v1/paging.proto\x1a\'doublecloud/clickhouse/v1/version.proto\"E\n\x13ListVersionsRequest\x12.\n\x06paging\x18\x01 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x8d\x01\n\x14ListVersionsResponse\x12>\n\x08versions\x18\x01 \x03(\x0b\x32\".doublecloud.clickhouse.v1.VersionR\x08versions\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage2y\n\x0eVersionService\x12g\n\x04List\x12..doublecloud.clickhouse.v1.ListVersionsRequest\x1a/.doublecloud.clickhouse.v1.ListVersionsResponseBAZ?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/doublecloud/clickhouse/v1/version_service.proto\x12\x19\x64oublecloud.clickhouse.v1\x1a\x1b\x64oublecloud/v1/paging.proto\x1a\'doublecloud/clickhouse/v1/version.proto\"E\n\x13ListVersionsRequest\x12.\n\x06paging\x18\x01 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x8d\x01\n\x14ListVersionsResponse\x12>\n\x08versions\x18\x01 \x03(\x0b\x32\".doublecloud.clickhouse.v1.VersionR\x08versions\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage2y\n\x0eVersionService\x12g\n\x04List\x12..doublecloud.clickhouse.v1.ListVersionsRequest\x1a/.doublecloud.clickhouse.v1.ListVersionsResponseBIZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.clickhouse.v1.version_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z?github.com/doublecloud/api/doublecloud/clickhouse/v1;clickhouse'
+  DESCRIPTOR._serialized_options = b'ZGgithub.com/doublecloud/go-genproto/doublecloud/clickhouse/v1;clickhouse'
   _globals['_LISTVERSIONSREQUEST']._serialized_start=148
   _globals['_LISTVERSIONSREQUEST']._serialized_end=217
   _globals['_LISTVERSIONSRESPONSE']._serialized_start=220
   _globals['_LISTVERSIONSRESPONSE']._serialized_end=361
   _globals['_VERSIONSERVICE']._serialized_start=363
   _globals['_VERSIONSERVICE']._serialized_end=484
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/version_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/version_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/clickhouse/v1/version_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/cluster_pb2.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/cluster_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/kafka/v1/cluster.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from doublecloud.v1 import cluster_pb2 as doublecloud_dot_v1_dot_cluster__pb2
 from doublecloud.v1 import maintenance_pb2 as doublecloud_dot_v1_dot_maintenance__pb2
 from doublecloud.kafka.v1 import config_pb2 as doublecloud_dot_kafka_dot_v1_dot_config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"doublecloud/kafka/v1/cluster.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1c\x64oublecloud/v1/cluster.proto\x1a doublecloud/v1/maintenance.proto\x1a!doublecloud/kafka/v1/config.proto\"\x8c\t\n\x07\x43luster\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x03 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x04 \x01(\tR\x08regionId\x12;\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x07 \x01(\tR\x0b\x64\x65scription\x12\x35\n\x06status\x18\x08 \x01(\x0e\x32\x1d.doublecloud.v1.ClusterStatusR\x06status\x12\x18\n\x07version\x18\t \x01(\tR\x07version\x12\x44\n\tresources\x18\n \x01(\x0b\x32&.doublecloud.kafka.v1.ClusterResourcesR\tresources\x12M\n\x0f\x63onnection_info\x18\x0b \x01(\x0b\x32$.doublecloud.kafka.v1.ConnectionInfoR\x0e\x63onnectionInfo\x12.\n\x06\x61\x63\x63\x65ss\x18\x0c \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12>\n\nencryption\x18\r \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\x0e \x01(\tR\tnetworkId\x12\x63\n\x17private_connection_info\x18\x0f \x01(\x0b\x32+.doublecloud.kafka.v1.PrivateConnectionInfoR\x15privateConnectionInfo\x12P\n\x12maintenance_window\x18\x10 \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12Q\n\x11planned_operation\x18\x11 \x01(\x0b\x32$.doublecloud.v1.MaintenanceOperationR\x10plannedOperation\x12\x44\n\x0ckafka_config\x18\x12 \x01(\x0b\x32!.doublecloud.kafka.v1.KafkaConfigR\x0bkafkaConfig\x12|\n metrics_exporter_connection_info\x18\x13 \x01(\x0b\x32\x33.doublecloud.kafka.v1.MetricsExporterConnectionInfoR\x1dmetricsExporterConnectionInfo\x12`\n\x16schema_registry_config\x18\x14 \x01(\x0b\x32*.doublecloud.kafka.v1.SchemaRegistryConfigR\x14schemaRegistryConfig\"\xc4\x02\n\x10\x43lusterResources\x12\x42\n\x05kafka\x18\x01 \x01(\x0b\x32,.doublecloud.kafka.v1.ClusterResources.KafkaR\x05kafka\x1a\xeb\x01\n\x05Kafka\x12,\n\x12resource_preset_id\x18\x01 \x01(\tR\x10resourcePresetId\x12\x38\n\tdisk_size\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x08\x64iskSize\x12>\n\x0c\x62roker_count\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0b\x62rokerCount\x12:\n\nzone_count\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\tzoneCount\"m\n\x0e\x43onnectionInfo\x12+\n\x11\x63onnection_string\x18\x01 \x01(\tR\x10\x63onnectionString\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\"t\n\x15PrivateConnectionInfo\x12+\n\x11\x63onnection_string\x18\x01 \x01(\tR\x10\x63onnectionString\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\"O\n\x1dMetricsExporterConnectionInfo\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\"m\n\x04Host\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ncluster_id\x18\x02 \x01(\tR\tclusterId\x12\x32\n\x06status\x18\x03 \x01(\x0e\x32\x1a.doublecloud.v1.HostStatusR\x06statusB7Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafkab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"doublecloud/kafka/v1/cluster.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1c\x64oublecloud/v1/cluster.proto\x1a doublecloud/v1/maintenance.proto\x1a!doublecloud/kafka/v1/config.proto\"\x8c\t\n\x07\x43luster\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x03 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x04 \x01(\tR\x08regionId\x12;\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x07 \x01(\tR\x0b\x64\x65scription\x12\x35\n\x06status\x18\x08 \x01(\x0e\x32\x1d.doublecloud.v1.ClusterStatusR\x06status\x12\x18\n\x07version\x18\t \x01(\tR\x07version\x12\x44\n\tresources\x18\n \x01(\x0b\x32&.doublecloud.kafka.v1.ClusterResourcesR\tresources\x12M\n\x0f\x63onnection_info\x18\x0b \x01(\x0b\x32$.doublecloud.kafka.v1.ConnectionInfoR\x0e\x63onnectionInfo\x12.\n\x06\x61\x63\x63\x65ss\x18\x0c \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12>\n\nencryption\x18\r \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\x0e \x01(\tR\tnetworkId\x12\x63\n\x17private_connection_info\x18\x0f \x01(\x0b\x32+.doublecloud.kafka.v1.PrivateConnectionInfoR\x15privateConnectionInfo\x12P\n\x12maintenance_window\x18\x10 \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12Q\n\x11planned_operation\x18\x11 \x01(\x0b\x32$.doublecloud.v1.MaintenanceOperationR\x10plannedOperation\x12\x44\n\x0ckafka_config\x18\x12 \x01(\x0b\x32!.doublecloud.kafka.v1.KafkaConfigR\x0bkafkaConfig\x12|\n metrics_exporter_connection_info\x18\x13 \x01(\x0b\x32\x33.doublecloud.kafka.v1.MetricsExporterConnectionInfoR\x1dmetricsExporterConnectionInfo\x12`\n\x16schema_registry_config\x18\x14 \x01(\x0b\x32*.doublecloud.kafka.v1.SchemaRegistryConfigR\x14schemaRegistryConfig\"\xc4\x02\n\x10\x43lusterResources\x12\x42\n\x05kafka\x18\x01 \x01(\x0b\x32,.doublecloud.kafka.v1.ClusterResources.KafkaR\x05kafka\x1a\xeb\x01\n\x05Kafka\x12,\n\x12resource_preset_id\x18\x01 \x01(\tR\x10resourcePresetId\x12\x38\n\tdisk_size\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x08\x64iskSize\x12>\n\x0c\x62roker_count\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0b\x62rokerCount\x12:\n\nzone_count\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\tzoneCount\"m\n\x0e\x43onnectionInfo\x12+\n\x11\x63onnection_string\x18\x01 \x01(\tR\x10\x63onnectionString\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\"t\n\x15PrivateConnectionInfo\x12+\n\x11\x63onnection_string\x18\x01 \x01(\tR\x10\x63onnectionString\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\"O\n\x1dMetricsExporterConnectionInfo\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\"m\n\x04Host\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ncluster_id\x18\x02 \x01(\tR\tclusterId\x12\x32\n\x06status\x18\x03 \x01(\x0e\x32\x1a.doublecloud.v1.HostStatusR\x06statusB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.kafka.v1.cluster_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafka'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafka'
   _globals['_CLUSTER']._serialized_start=225
   _globals['_CLUSTER']._serialized_end=1389
   _globals['_CLUSTERRESOURCES']._serialized_start=1392
   _globals['_CLUSTERRESOURCES']._serialized_end=1716
   _globals['_CLUSTERRESOURCES_KAFKA']._serialized_start=1481
   _globals['_CLUSTERRESOURCES_KAFKA']._serialized_end=1716
   _globals['_CONNECTIONINFO']._serialized_start=1718
```

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/cluster_pb2.pyi` & `doublecloud-0.6.0/doublecloud/kafka/v1/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/cluster_service_pb2.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/cluster_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/kafka/v1/cluster_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from doublecloud.v1 import cluster_pb2 as doublecloud_dot_v1_dot_cluster__pb2
 from doublecloud.v1 import maintenance_pb2 as doublecloud_dot_v1_dot_maintenance__pb2
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 from doublecloud.kafka.v1 import cluster_pb2 as doublecloud_dot_kafka_dot_v1_dot_cluster__pb2
 from doublecloud.kafka.v1 import config_pb2 as doublecloud_dot_kafka_dot_v1_dot_config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*doublecloud/kafka/v1/cluster_service.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1c\x64oublecloud/v1/cluster.proto\x1a doublecloud/v1/maintenance.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\x1a\"doublecloud/kafka/v1/cluster.proto\x1a!doublecloud/kafka/v1/config.proto\"P\n\x11GetClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1c\n\tsensitive\x18\x02 \x01(\x08R\tsensitive\"\x9b\x01\n\x13ListClustersRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\x12\x35\n\x04view\x18\x03 \x01(\x0e\x32!.doublecloud.kafka.v1.ClusterViewR\x04view\"\x88\x01\n\x14ListClustersResponse\x12\x39\n\x08\x63lusters\x18\x01 \x03(\x0b\x32\x1d.doublecloud.kafka.v1.ClusterR\x08\x63lusters\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\x90\x05\n\x14\x43reateClusterRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x02 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x06 \x01(\tR\x07version\x12\x44\n\tresources\x18\x07 \x01(\x0b\x32&.doublecloud.kafka.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x08 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12>\n\nencryption\x18\t \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\n \x01(\tR\tnetworkId\x12P\n\x12maintenance_window\x18\x0b \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12\x44\n\x0ckafka_config\x18\x0c \x01(\x0b\x32!.doublecloud.kafka.v1.KafkaConfigR\x0bkafkaConfig\x12`\n\x16schema_registry_config\x18\r \x01(\x0b\x32*.doublecloud.kafka.v1.SchemaRegistryConfigR\x14schemaRegistryConfig\"\xf5\x03\n\x14UpdateClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x04 \x01(\tR\x07version\x12\x44\n\tresources\x18\x05 \x01(\x0b\x32&.doublecloud.kafka.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12P\n\x12maintenance_window\x18\x07 \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12\x44\n\x0ckafka_config\x18\x08 \x01(\x0b\x32!.doublecloud.kafka.v1.KafkaConfigR\x0bkafkaConfig\x12`\n\x16schema_registry_config\x18\t \x01(\x0b\x32*.doublecloud.kafka.v1.SchemaRegistryConfigR\x14schemaRegistryConfig\"5\n\x14\x44\x65leteClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"?\n\x1eResetClusterCredentialsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"h\n\x17ListClusterHostsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x83\x01\n\x18ListClusterHostsResponse\x12\x30\n\x05hosts\x18\x01 \x03(\x0b\x32\x1a.doublecloud.kafka.v1.HostR\x05hosts\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"4\n\x13StartClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"3\n\x12StopClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"\xd0\x01\n\x1cRescheduleMaintenanceRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12G\n\x0freschedule_type\x18\x02 \x01(\x0e\x32\x1e.doublecloud.v1.RescheduleTypeR\x0erescheduleType\x12H\n\x12\x64\x65layed_until_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x64\x65layedUntilTime\"m\n\x1cListClusterOperationsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x91\x01\n\x1dListClusterOperationsResponse\x12\x39\n\noperations\x18\x01 \x03(\x0b\x32\x19.doublecloud.v1.OperationR\noperations\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage*V\n\x0b\x43lusterView\x12\x18\n\x14\x43LUSTER_VIEW_INVALID\x10\x00\x12\x16\n\x12\x43LUSTER_VIEW_BASIC\x10\x01\x12\x15\n\x11\x43LUSTER_VIEW_FULL\x10\x02\x32\x81\x08\n\x0e\x43lusterService\x12M\n\x03Get\x12\'.doublecloud.kafka.v1.GetClusterRequest\x1a\x1d.doublecloud.kafka.v1.Cluster\x12]\n\x04List\x12).doublecloud.kafka.v1.ListClustersRequest\x1a*.doublecloud.kafka.v1.ListClustersResponse\x12O\n\x06\x43reate\x12*.doublecloud.kafka.v1.CreateClusterRequest\x1a\x19.doublecloud.v1.Operation\x12O\n\x06Update\x12*.doublecloud.kafka.v1.UpdateClusterRequest\x1a\x19.doublecloud.v1.Operation\x12O\n\x06\x44\x65lete\x12*.doublecloud.kafka.v1.DeleteClusterRequest\x1a\x19.doublecloud.v1.Operation\x12\x63\n\x10ResetCredentials\x12\x34.doublecloud.kafka.v1.ResetClusterCredentialsRequest\x1a\x19.doublecloud.v1.Operation\x12j\n\tListHosts\x12-.doublecloud.kafka.v1.ListClusterHostsRequest\x1a..doublecloud.kafka.v1.ListClusterHostsResponse\x12M\n\x05Start\x12).doublecloud.kafka.v1.StartClusterRequest\x1a\x19.doublecloud.v1.Operation\x12K\n\x04Stop\x12(.doublecloud.kafka.v1.StopClusterRequest\x1a\x19.doublecloud.v1.Operation\x12\x66\n\x15RescheduleMaintenance\x12\x32.doublecloud.kafka.v1.RescheduleMaintenanceRequest\x1a\x19.doublecloud.v1.Operation\x12y\n\x0eListOperations\x12\x32.doublecloud.kafka.v1.ListClusterOperationsRequest\x1a\x33.doublecloud.kafka.v1.ListClusterOperationsResponseB7Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafkab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*doublecloud/kafka/v1/cluster_service.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1c\x64oublecloud/v1/cluster.proto\x1a doublecloud/v1/maintenance.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\x1a\"doublecloud/kafka/v1/cluster.proto\x1a!doublecloud/kafka/v1/config.proto\"P\n\x11GetClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1c\n\tsensitive\x18\x02 \x01(\x08R\tsensitive\"\x9b\x01\n\x13ListClustersRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\x12\x35\n\x04view\x18\x03 \x01(\x0e\x32!.doublecloud.kafka.v1.ClusterViewR\x04view\"\x88\x01\n\x14ListClustersResponse\x12\x39\n\x08\x63lusters\x18\x01 \x03(\x0b\x32\x1d.doublecloud.kafka.v1.ClusterR\x08\x63lusters\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\x90\x05\n\x14\x43reateClusterRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x02 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x06 \x01(\tR\x07version\x12\x44\n\tresources\x18\x07 \x01(\x0b\x32&.doublecloud.kafka.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x08 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12>\n\nencryption\x18\t \x01(\x0b\x32\x1e.doublecloud.v1.DataEncryptionR\nencryption\x12\x1d\n\nnetwork_id\x18\n \x01(\tR\tnetworkId\x12P\n\x12maintenance_window\x18\x0b \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12\x44\n\x0ckafka_config\x18\x0c \x01(\x0b\x32!.doublecloud.kafka.v1.KafkaConfigR\x0bkafkaConfig\x12`\n\x16schema_registry_config\x18\r \x01(\x0b\x32*.doublecloud.kafka.v1.SchemaRegistryConfigR\x14schemaRegistryConfig\"\xf5\x03\n\x14UpdateClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07version\x18\x04 \x01(\tR\x07version\x12\x44\n\tresources\x18\x05 \x01(\x0b\x32&.doublecloud.kafka.v1.ClusterResourcesR\tresources\x12.\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x16.doublecloud.v1.AccessR\x06\x61\x63\x63\x65ss\x12P\n\x12maintenance_window\x18\x07 \x01(\x0b\x32!.doublecloud.v1.MaintenanceWindowR\x11maintenanceWindow\x12\x44\n\x0ckafka_config\x18\x08 \x01(\x0b\x32!.doublecloud.kafka.v1.KafkaConfigR\x0bkafkaConfig\x12`\n\x16schema_registry_config\x18\t \x01(\x0b\x32*.doublecloud.kafka.v1.SchemaRegistryConfigR\x14schemaRegistryConfig\"5\n\x14\x44\x65leteClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"?\n\x1eResetClusterCredentialsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"h\n\x17ListClusterHostsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x83\x01\n\x18ListClusterHostsResponse\x12\x30\n\x05hosts\x18\x01 \x03(\x0b\x32\x1a.doublecloud.kafka.v1.HostR\x05hosts\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"4\n\x13StartClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"3\n\x12StopClusterRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\"\xd0\x01\n\x1cRescheduleMaintenanceRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12G\n\x0freschedule_type\x18\x02 \x01(\x0e\x32\x1e.doublecloud.v1.RescheduleTypeR\x0erescheduleType\x12H\n\x12\x64\x65layed_until_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x64\x65layedUntilTime\"m\n\x1cListClusterOperationsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x91\x01\n\x1dListClusterOperationsResponse\x12\x39\n\noperations\x18\x01 \x03(\x0b\x32\x19.doublecloud.v1.OperationR\noperations\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage*V\n\x0b\x43lusterView\x12\x18\n\x14\x43LUSTER_VIEW_INVALID\x10\x00\x12\x16\n\x12\x43LUSTER_VIEW_BASIC\x10\x01\x12\x15\n\x11\x43LUSTER_VIEW_FULL\x10\x02\x32\x81\x08\n\x0e\x43lusterService\x12M\n\x03Get\x12\'.doublecloud.kafka.v1.GetClusterRequest\x1a\x1d.doublecloud.kafka.v1.Cluster\x12]\n\x04List\x12).doublecloud.kafka.v1.ListClustersRequest\x1a*.doublecloud.kafka.v1.ListClustersResponse\x12O\n\x06\x43reate\x12*.doublecloud.kafka.v1.CreateClusterRequest\x1a\x19.doublecloud.v1.Operation\x12O\n\x06Update\x12*.doublecloud.kafka.v1.UpdateClusterRequest\x1a\x19.doublecloud.v1.Operation\x12O\n\x06\x44\x65lete\x12*.doublecloud.kafka.v1.DeleteClusterRequest\x1a\x19.doublecloud.v1.Operation\x12\x63\n\x10ResetCredentials\x12\x34.doublecloud.kafka.v1.ResetClusterCredentialsRequest\x1a\x19.doublecloud.v1.Operation\x12j\n\tListHosts\x12-.doublecloud.kafka.v1.ListClusterHostsRequest\x1a..doublecloud.kafka.v1.ListClusterHostsResponse\x12M\n\x05Start\x12).doublecloud.kafka.v1.StartClusterRequest\x1a\x19.doublecloud.v1.Operation\x12K\n\x04Stop\x12(.doublecloud.kafka.v1.StopClusterRequest\x1a\x19.doublecloud.v1.Operation\x12\x66\n\x15RescheduleMaintenance\x12\x32.doublecloud.kafka.v1.RescheduleMaintenanceRequest\x1a\x19.doublecloud.v1.Operation\x12y\n\x0eListOperations\x12\x32.doublecloud.kafka.v1.ListClusterOperationsRequest\x1a\x33.doublecloud.kafka.v1.ListClusterOperationsResponseB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.kafka.v1.cluster_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafka'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafka'
   _globals['_CLUSTERVIEW']._serialized_start=2776
   _globals['_CLUSTERVIEW']._serialized_end=2862
   _globals['_GETCLUSTERREQUEST']._serialized_start=297
   _globals['_GETCLUSTERREQUEST']._serialized_end=377
   _globals['_LISTCLUSTERSREQUEST']._serialized_start=380
   _globals['_LISTCLUSTERSREQUEST']._serialized_end=535
   _globals['_LISTCLUSTERSRESPONSE']._serialized_start=538
```

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/cluster_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/kafka/v1/cluster_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/cluster_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/config_pb2.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/config_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/kafka/v1/config.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!doublecloud/kafka/v1/config.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xaa\x01\n\x0bKafkaConfig\x12G\n\x11message_max_bytes\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0fmessageMaxBytes\x12R\n\x17replica_fetch_max_bytes\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x14replicaFetchMaxBytes\"0\n\x14SchemaRegistryConfig\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabledB7Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafkab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!doublecloud/kafka/v1/config.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xaa\x01\n\x0bKafkaConfig\x12G\n\x11message_max_bytes\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0fmessageMaxBytes\x12R\n\x17replica_fetch_max_bytes\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x14replicaFetchMaxBytes\"0\n\x14SchemaRegistryConfig\x12\x18\n\x07\x65nabled\x18\x01 \x01(\x08R\x07\x65nabledB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.kafka.v1.config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafka'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafka'
   _globals['_KAFKACONFIG']._serialized_start=92
   _globals['_KAFKACONFIG']._serialized_end=262
   _globals['_SCHEMAREGISTRYCONFIG']._serialized_start=264
   _globals['_SCHEMAREGISTRYCONFIG']._serialized_end=312
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/config_pb2.pyi` & `doublecloud-0.6.0/doublecloud/kafka/v1/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/operation_service_pb2.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/operation_service_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/kafka/v1/operation_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,doublecloud/kafka/v1/operation_service.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"8\n\x13GetOperationRequest\x12!\n\x0coperation_id\x18\x01 \x01(\tR\x0boperationId\"f\n\x15ListOperationsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x8a\x01\n\x16ListOperationsResponse\x12\x39\n\noperations\x18\x01 \x03(\x0b\x32\x19.doublecloud.v1.OperationR\noperations\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage2\xc2\x01\n\x10OperationService\x12K\n\x03Get\x12).doublecloud.kafka.v1.GetOperationRequest\x1a\x19.doublecloud.v1.Operation\x12\x61\n\x04List\x12+.doublecloud.kafka.v1.ListOperationsRequest\x1a,.doublecloud.kafka.v1.ListOperationsResponseB7Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafkab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,doublecloud/kafka/v1/operation_service.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"8\n\x13GetOperationRequest\x12!\n\x0coperation_id\x18\x01 \x01(\tR\x0boperationId\"f\n\x15ListOperationsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x8a\x01\n\x16ListOperationsResponse\x12\x39\n\noperations\x18\x01 \x03(\x0b\x32\x19.doublecloud.v1.OperationR\noperations\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage2\xc2\x01\n\x10OperationService\x12K\n\x03Get\x12).doublecloud.kafka.v1.GetOperationRequest\x1a\x19.doublecloud.v1.Operation\x12\x61\n\x04List\x12+.doublecloud.kafka.v1.ListOperationsRequest\x1a,.doublecloud.kafka.v1.ListOperationsResponseB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.kafka.v1.operation_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafka'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafka'
   _globals['_GETOPERATIONREQUEST']._serialized_start=131
   _globals['_GETOPERATIONREQUEST']._serialized_end=187
   _globals['_LISTOPERATIONSREQUEST']._serialized_start=189
   _globals['_LISTOPERATIONSREQUEST']._serialized_end=291
   _globals['_LISTOPERATIONSRESPONSE']._serialized_start=294
   _globals['_LISTOPERATIONSRESPONSE']._serialized_end=432
   _globals['_OPERATIONSERVICE']._serialized_start=435
```

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/operation_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/kafka/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/topic_pb2.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/topic_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/kafka/v1/topic.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n doublecloud/kafka/v1/topic.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1egoogle/protobuf/wrappers.proto\"\x84\x03\n\x05Topic\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ncluster_id\x18\x02 \x01(\tR\tclusterId\x12;\n\npartitions\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\npartitions\x12J\n\x12replication_factor\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x11replicationFactor\x12N\n\x10topic_config_2_8\x18\x05 \x01(\x0b\x32#.doublecloud.kafka.v1.TopicConfig28H\x00R\rtopicConfig28\x12J\n\x0etopic_config_3\x18\x07 \x01(\x0b\x32\".doublecloud.kafka.v1.TopicConfig3H\x00R\x0ctopicConfig3\x12\x13\n\x05is_ha\x18\x08 \x01(\x08R\x04isHaB\x0e\n\x0ctopic_config\"\xd4\x02\n\tTopicSpec\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\npartitions\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\npartitions\x12J\n\x12replication_factor\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x11replicationFactor\x12N\n\x10topic_config_2_8\x18\x04 \x01(\x0b\x32#.doublecloud.kafka.v1.TopicConfig28H\x00R\rtopicConfig28\x12J\n\x0etopic_config_3\x18\x06 \x01(\x0b\x32\".doublecloud.kafka.v1.TopicConfig3H\x00R\x0ctopicConfig3B\x0e\n\x0ctopic_config\"\x85\x06\n\rTopicConfig28\x12X\n\x0e\x63leanup_policy\x18\x01 \x01(\x0e\x32\x31.doublecloud.kafka.v1.TopicConfig28.CleanupPolicyR\rcleanupPolicy\x12^\n\x10\x63ompression_type\x18\x02 \x01(\x0e\x32\x33.doublecloud.kafka.v1.TopicConfig28.CompressionTypeR\x0f\x63ompressionType\x12\x44\n\x0fretention_bytes\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0eretentionBytes\x12>\n\x0cretention_ms\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0bretentionMs\x12G\n\x11max_message_bytes\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0fmaxMessageBytes\"\x89\x01\n\rCleanupPolicy\x12\x1a\n\x16\x43LEANUP_POLICY_INVALID\x10\x00\x12\x19\n\x15\x43LEANUP_POLICY_DELETE\x10\x01\x12\x1a\n\x16\x43LEANUP_POLICY_COMPACT\x10\x02\x12%\n!CLEANUP_POLICY_COMPACT_AND_DELETE\x10\x03\"\xde\x01\n\x0f\x43ompressionType\x12\x1c\n\x18\x43OMPRESSION_TYPE_INVALID\x10\x00\x12!\n\x1d\x43OMPRESSION_TYPE_UNCOMPRESSED\x10\x01\x12\x19\n\x15\x43OMPRESSION_TYPE_ZSTD\x10\x02\x12\x18\n\x14\x43OMPRESSION_TYPE_LZ4\x10\x03\x12\x1b\n\x17\x43OMPRESSION_TYPE_SNAPPY\x10\x04\x12\x19\n\x15\x43OMPRESSION_TYPE_GZIP\x10\x05\x12\x1d\n\x19\x43OMPRESSION_TYPE_PRODUCER\x10\x06\"\x82\x06\n\x0cTopicConfig3\x12W\n\x0e\x63leanup_policy\x18\x01 \x01(\x0e\x32\x30.doublecloud.kafka.v1.TopicConfig3.CleanupPolicyR\rcleanupPolicy\x12]\n\x10\x63ompression_type\x18\x02 \x01(\x0e\x32\x32.doublecloud.kafka.v1.TopicConfig3.CompressionTypeR\x0f\x63ompressionType\x12\x44\n\x0fretention_bytes\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0eretentionBytes\x12>\n\x0cretention_ms\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0bretentionMs\x12G\n\x11max_message_bytes\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0fmaxMessageBytes\"\x89\x01\n\rCleanupPolicy\x12\x1a\n\x16\x43LEANUP_POLICY_INVALID\x10\x00\x12\x19\n\x15\x43LEANUP_POLICY_DELETE\x10\x01\x12\x1a\n\x16\x43LEANUP_POLICY_COMPACT\x10\x02\x12%\n!CLEANUP_POLICY_COMPACT_AND_DELETE\x10\x03\"\xde\x01\n\x0f\x43ompressionType\x12\x1c\n\x18\x43OMPRESSION_TYPE_INVALID\x10\x00\x12!\n\x1d\x43OMPRESSION_TYPE_UNCOMPRESSED\x10\x01\x12\x19\n\x15\x43OMPRESSION_TYPE_ZSTD\x10\x02\x12\x18\n\x14\x43OMPRESSION_TYPE_LZ4\x10\x03\x12\x1b\n\x17\x43OMPRESSION_TYPE_SNAPPY\x10\x04\x12\x19\n\x15\x43OMPRESSION_TYPE_GZIP\x10\x05\x12\x1d\n\x19\x43OMPRESSION_TYPE_PRODUCER\x10\x06\x42\x37Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafkab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n doublecloud/kafka/v1/topic.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1egoogle/protobuf/wrappers.proto\"\x84\x03\n\x05Topic\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ncluster_id\x18\x02 \x01(\tR\tclusterId\x12;\n\npartitions\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\npartitions\x12J\n\x12replication_factor\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x11replicationFactor\x12N\n\x10topic_config_2_8\x18\x05 \x01(\x0b\x32#.doublecloud.kafka.v1.TopicConfig28H\x00R\rtopicConfig28\x12J\n\x0etopic_config_3\x18\x07 \x01(\x0b\x32\".doublecloud.kafka.v1.TopicConfig3H\x00R\x0ctopicConfig3\x12\x13\n\x05is_ha\x18\x08 \x01(\x08R\x04isHaB\x0e\n\x0ctopic_config\"\xd4\x02\n\tTopicSpec\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12;\n\npartitions\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\npartitions\x12J\n\x12replication_factor\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x11replicationFactor\x12N\n\x10topic_config_2_8\x18\x04 \x01(\x0b\x32#.doublecloud.kafka.v1.TopicConfig28H\x00R\rtopicConfig28\x12J\n\x0etopic_config_3\x18\x06 \x01(\x0b\x32\".doublecloud.kafka.v1.TopicConfig3H\x00R\x0ctopicConfig3B\x0e\n\x0ctopic_config\"\x85\x06\n\rTopicConfig28\x12X\n\x0e\x63leanup_policy\x18\x01 \x01(\x0e\x32\x31.doublecloud.kafka.v1.TopicConfig28.CleanupPolicyR\rcleanupPolicy\x12^\n\x10\x63ompression_type\x18\x02 \x01(\x0e\x32\x33.doublecloud.kafka.v1.TopicConfig28.CompressionTypeR\x0f\x63ompressionType\x12\x44\n\x0fretention_bytes\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0eretentionBytes\x12>\n\x0cretention_ms\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0bretentionMs\x12G\n\x11max_message_bytes\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0fmaxMessageBytes\"\x89\x01\n\rCleanupPolicy\x12\x1a\n\x16\x43LEANUP_POLICY_INVALID\x10\x00\x12\x19\n\x15\x43LEANUP_POLICY_DELETE\x10\x01\x12\x1a\n\x16\x43LEANUP_POLICY_COMPACT\x10\x02\x12%\n!CLEANUP_POLICY_COMPACT_AND_DELETE\x10\x03\"\xde\x01\n\x0f\x43ompressionType\x12\x1c\n\x18\x43OMPRESSION_TYPE_INVALID\x10\x00\x12!\n\x1d\x43OMPRESSION_TYPE_UNCOMPRESSED\x10\x01\x12\x19\n\x15\x43OMPRESSION_TYPE_ZSTD\x10\x02\x12\x18\n\x14\x43OMPRESSION_TYPE_LZ4\x10\x03\x12\x1b\n\x17\x43OMPRESSION_TYPE_SNAPPY\x10\x04\x12\x19\n\x15\x43OMPRESSION_TYPE_GZIP\x10\x05\x12\x1d\n\x19\x43OMPRESSION_TYPE_PRODUCER\x10\x06\"\x82\x06\n\x0cTopicConfig3\x12W\n\x0e\x63leanup_policy\x18\x01 \x01(\x0e\x32\x30.doublecloud.kafka.v1.TopicConfig3.CleanupPolicyR\rcleanupPolicy\x12]\n\x10\x63ompression_type\x18\x02 \x01(\x0e\x32\x32.doublecloud.kafka.v1.TopicConfig3.CompressionTypeR\x0f\x63ompressionType\x12\x44\n\x0fretention_bytes\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0eretentionBytes\x12>\n\x0cretention_ms\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0bretentionMs\x12G\n\x11max_message_bytes\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64ValueR\x0fmaxMessageBytes\"\x89\x01\n\rCleanupPolicy\x12\x1a\n\x16\x43LEANUP_POLICY_INVALID\x10\x00\x12\x19\n\x15\x43LEANUP_POLICY_DELETE\x10\x01\x12\x1a\n\x16\x43LEANUP_POLICY_COMPACT\x10\x02\x12%\n!CLEANUP_POLICY_COMPACT_AND_DELETE\x10\x03\"\xde\x01\n\x0f\x43ompressionType\x12\x1c\n\x18\x43OMPRESSION_TYPE_INVALID\x10\x00\x12!\n\x1d\x43OMPRESSION_TYPE_UNCOMPRESSED\x10\x01\x12\x19\n\x15\x43OMPRESSION_TYPE_ZSTD\x10\x02\x12\x18\n\x14\x43OMPRESSION_TYPE_LZ4\x10\x03\x12\x1b\n\x17\x43OMPRESSION_TYPE_SNAPPY\x10\x04\x12\x19\n\x15\x43OMPRESSION_TYPE_GZIP\x10\x05\x12\x1d\n\x19\x43OMPRESSION_TYPE_PRODUCER\x10\x06\x42?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.kafka.v1.topic_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafka'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafka'
   _globals['_TOPIC']._serialized_start=91
   _globals['_TOPIC']._serialized_end=479
   _globals['_TOPICSPEC']._serialized_start=482
   _globals['_TOPICSPEC']._serialized_end=822
   _globals['_TOPICCONFIG28']._serialized_start=825
   _globals['_TOPICCONFIG28']._serialized_end=1598
   _globals['_TOPICCONFIG28_CLEANUPPOLICY']._serialized_start=1236
```

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/topic_pb2.pyi` & `doublecloud-0.6.0/doublecloud/kafka/v1/topic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/topic_service_pb2.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/topic_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/kafka/v1/topic_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 from doublecloud.kafka.v1 import topic_pb2 as doublecloud_dot_kafka_dot_v1_dot_topic__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(doublecloud/kafka/v1/topic_service.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\x1a doublecloud/kafka/v1/topic.proto\"O\n\x0fGetTopicRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1d\n\ntopic_name\x18\x02 \x01(\tR\ttopicName\"b\n\x11ListTopicsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x80\x01\n\x12ListTopicsResponse\x12\x33\n\x06topics\x18\x01 \x03(\x0b\x32\x1b.doublecloud.kafka.v1.TopicR\x06topics\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"s\n\x12\x43reateTopicRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12>\n\ntopic_spec\x18\x02 \x01(\x0b\x32\x1f.doublecloud.kafka.v1.TopicSpecR\ttopicSpec\"\x92\x01\n\x12UpdateTopicRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1d\n\ntopic_name\x18\x02 \x01(\tR\ttopicName\x12>\n\ntopic_spec\x18\x03 \x01(\x0b\x32\x1f.doublecloud.kafka.v1.TopicSpecR\ttopicSpec\"R\n\x12\x44\x65leteTopicRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1d\n\ntopic_name\x18\x02 \x01(\tR\ttopicName2\xa1\x03\n\x0cTopicService\x12I\n\x03Get\x12%.doublecloud.kafka.v1.GetTopicRequest\x1a\x1b.doublecloud.kafka.v1.Topic\x12Y\n\x04List\x12\'.doublecloud.kafka.v1.ListTopicsRequest\x1a(.doublecloud.kafka.v1.ListTopicsResponse\x12M\n\x06\x43reate\x12(.doublecloud.kafka.v1.CreateTopicRequest\x1a\x19.doublecloud.v1.Operation\x12M\n\x06Update\x12(.doublecloud.kafka.v1.UpdateTopicRequest\x1a\x19.doublecloud.v1.Operation\x12M\n\x06\x44\x65lete\x12(.doublecloud.kafka.v1.DeleteTopicRequest\x1a\x19.doublecloud.v1.OperationB7Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafkab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(doublecloud/kafka/v1/topic_service.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\x1a doublecloud/kafka/v1/topic.proto\"O\n\x0fGetTopicRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1d\n\ntopic_name\x18\x02 \x01(\tR\ttopicName\"b\n\x11ListTopicsRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x80\x01\n\x12ListTopicsResponse\x12\x33\n\x06topics\x18\x01 \x03(\x0b\x32\x1b.doublecloud.kafka.v1.TopicR\x06topics\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"s\n\x12\x43reateTopicRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12>\n\ntopic_spec\x18\x02 \x01(\x0b\x32\x1f.doublecloud.kafka.v1.TopicSpecR\ttopicSpec\"\x92\x01\n\x12UpdateTopicRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1d\n\ntopic_name\x18\x02 \x01(\tR\ttopicName\x12>\n\ntopic_spec\x18\x03 \x01(\x0b\x32\x1f.doublecloud.kafka.v1.TopicSpecR\ttopicSpec\"R\n\x12\x44\x65leteTopicRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1d\n\ntopic_name\x18\x02 \x01(\tR\ttopicName2\xa1\x03\n\x0cTopicService\x12I\n\x03Get\x12%.doublecloud.kafka.v1.GetTopicRequest\x1a\x1b.doublecloud.kafka.v1.Topic\x12Y\n\x04List\x12\'.doublecloud.kafka.v1.ListTopicsRequest\x1a(.doublecloud.kafka.v1.ListTopicsResponse\x12M\n\x06\x43reate\x12(.doublecloud.kafka.v1.CreateTopicRequest\x1a\x19.doublecloud.v1.Operation\x12M\n\x06Update\x12(.doublecloud.kafka.v1.UpdateTopicRequest\x1a\x19.doublecloud.v1.Operation\x12M\n\x06\x44\x65lete\x12(.doublecloud.kafka.v1.DeleteTopicRequest\x1a\x19.doublecloud.v1.OperationB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.kafka.v1.topic_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafka'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafka'
   _globals['_GETTOPICREQUEST']._serialized_start=161
   _globals['_GETTOPICREQUEST']._serialized_end=240
   _globals['_LISTTOPICSREQUEST']._serialized_start=242
   _globals['_LISTTOPICSREQUEST']._serialized_end=340
   _globals['_LISTTOPICSRESPONSE']._serialized_start=343
   _globals['_LISTTOPICSRESPONSE']._serialized_end=471
   _globals['_CREATETOPICREQUEST']._serialized_start=473
```

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/topic_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/kafka/v1/topic_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/topic_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/user_pb2.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/user_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/kafka/v1/user.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x64oublecloud/kafka/v1/user.proto\x12\x14\x64oublecloud.kafka.v1\"}\n\x04User\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ncluster_id\x18\x02 \x01(\tR\tclusterId\x12\x42\n\x0bpermissions\x18\x03 \x03(\x0b\x32 .doublecloud.kafka.v1.PermissionR\x0bpermissions\"~\n\x08UserSpec\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1a\n\x08password\x18\x02 \x01(\tR\x08password\x12\x42\n\x0bpermissions\x18\x03 \x03(\x0b\x32 .doublecloud.kafka.v1.PermissionR\x0bpermissions\"\xde\x01\n\nPermission\x12\x1d\n\ntopic_name\x18\x01 \x01(\tR\ttopicName\x12?\n\x04role\x18\x02 \x01(\x0e\x32+.doublecloud.kafka.v1.Permission.AccessRoleR\x04role\"p\n\nAccessRole\x12\x17\n\x13\x41\x43\x43\x45SS_ROLE_INVALID\x10\x00\x12\x18\n\x14\x41\x43\x43\x45SS_ROLE_PRODUCER\x10\x01\x12\x18\n\x14\x41\x43\x43\x45SS_ROLE_CONSUMER\x10\x02\x12\x15\n\x11\x41\x43\x43\x45SS_ROLE_ADMIN\x10\x03\x42\x37Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafkab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x64oublecloud/kafka/v1/user.proto\x12\x14\x64oublecloud.kafka.v1\"}\n\x04User\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1d\n\ncluster_id\x18\x02 \x01(\tR\tclusterId\x12\x42\n\x0bpermissions\x18\x03 \x03(\x0b\x32 .doublecloud.kafka.v1.PermissionR\x0bpermissions\"~\n\x08UserSpec\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1a\n\x08password\x18\x02 \x01(\tR\x08password\x12\x42\n\x0bpermissions\x18\x03 \x03(\x0b\x32 .doublecloud.kafka.v1.PermissionR\x0bpermissions\"\xde\x01\n\nPermission\x12\x1d\n\ntopic_name\x18\x01 \x01(\tR\ttopicName\x12?\n\x04role\x18\x02 \x01(\x0e\x32+.doublecloud.kafka.v1.Permission.AccessRoleR\x04role\"p\n\nAccessRole\x12\x17\n\x13\x41\x43\x43\x45SS_ROLE_INVALID\x10\x00\x12\x18\n\x14\x41\x43\x43\x45SS_ROLE_PRODUCER\x10\x01\x12\x18\n\x14\x41\x43\x43\x45SS_ROLE_CONSUMER\x10\x02\x12\x15\n\x11\x41\x43\x43\x45SS_ROLE_ADMIN\x10\x03\x42?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.kafka.v1.user_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafka'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafka'
   _globals['_USER']._serialized_start=57
   _globals['_USER']._serialized_end=182
   _globals['_USERSPEC']._serialized_start=184
   _globals['_USERSPEC']._serialized_end=310
   _globals['_PERMISSION']._serialized_start=313
   _globals['_PERMISSION']._serialized_end=535
   _globals['_PERMISSION_ACCESSROLE']._serialized_start=423
```

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/user_pb2.pyi` & `doublecloud-0.6.0/doublecloud/kafka/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/user_service_pb2.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/user_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/kafka/v1/user_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 from doublecloud.kafka.v1 import user_pb2 as doublecloud_dot_kafka_dot_v1_dot_user__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'doublecloud/kafka/v1/user_service.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\x1a\x1f\x64oublecloud/kafka/v1/user.proto\x1a\x1egoogle/protobuf/wrappers.proto\"L\n\x0eGetUserRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1b\n\tuser_name\x18\x02 \x01(\tR\x08userName\"a\n\x10ListUsersRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"|\n\x11ListUsersResponse\x12\x30\n\x05users\x18\x01 \x03(\x0b\x32\x1a.doublecloud.kafka.v1.UserR\x05users\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"o\n\x11\x43reateUserRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12;\n\tuser_spec\x18\x02 \x01(\x0b\x32\x1e.doublecloud.kafka.v1.UserSpecR\x08userSpec\"\xae\x03\n\x11UpdateUserRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1b\n\tuser_name\x18\x02 \x01(\tR\x08userName\x12S\n\x0bupdate_spec\x18\x03 \x01(\x0b\x32\x32.doublecloud.kafka.v1.UpdateUserRequest.UpdateSpecR\nupdateSpec\x1a\x87\x02\n\nUpdateSpec\x12\x38\n\x08password\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08password\x12\x66\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x44.doublecloud.kafka.v1.UpdateUserRequest.UpdateSpec.UpdatePermissionsR\x0bpermissions\x1aW\n\x11UpdatePermissions\x12\x42\n\x0bpermissions\x18\x01 \x03(\x0b\x32 .doublecloud.kafka.v1.PermissionR\x0bpermissions\"O\n\x11\x44\x65leteUserRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1b\n\tuser_name\x18\x02 \x01(\tR\x08userName\"\x9a\x01\n\x1aGrantUserPermissionRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1b\n\tuser_name\x18\x02 \x01(\tR\x08userName\x12@\n\npermission\x18\x03 \x01(\x0b\x32 .doublecloud.kafka.v1.PermissionR\npermission\"\x9b\x01\n\x1bRevokeUserPermissionRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1b\n\tuser_name\x18\x02 \x01(\tR\x08userName\x12@\n\npermission\x18\x03 \x01(\x0b\x32 .doublecloud.kafka.v1.PermissionR\npermission2\xdb\x04\n\x0bUserService\x12G\n\x03Get\x12$.doublecloud.kafka.v1.GetUserRequest\x1a\x1a.doublecloud.kafka.v1.User\x12W\n\x04List\x12&.doublecloud.kafka.v1.ListUsersRequest\x1a\'.doublecloud.kafka.v1.ListUsersResponse\x12L\n\x06\x43reate\x12\'.doublecloud.kafka.v1.CreateUserRequest\x1a\x19.doublecloud.v1.Operation\x12L\n\x06Update\x12\'.doublecloud.kafka.v1.UpdateUserRequest\x1a\x19.doublecloud.v1.Operation\x12L\n\x06\x44\x65lete\x12\'.doublecloud.kafka.v1.DeleteUserRequest\x1a\x19.doublecloud.v1.Operation\x12^\n\x0fGrantPermission\x12\x30.doublecloud.kafka.v1.GrantUserPermissionRequest\x1a\x19.doublecloud.v1.Operation\x12`\n\x10RevokePermission\x12\x31.doublecloud.kafka.v1.RevokeUserPermissionRequest\x1a\x19.doublecloud.v1.OperationB7Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafkab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'doublecloud/kafka/v1/user_service.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\x1a\x1f\x64oublecloud/kafka/v1/user.proto\x1a\x1egoogle/protobuf/wrappers.proto\"L\n\x0eGetUserRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1b\n\tuser_name\x18\x02 \x01(\tR\x08userName\"a\n\x10ListUsersRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"|\n\x11ListUsersResponse\x12\x30\n\x05users\x18\x01 \x03(\x0b\x32\x1a.doublecloud.kafka.v1.UserR\x05users\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"o\n\x11\x43reateUserRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12;\n\tuser_spec\x18\x02 \x01(\x0b\x32\x1e.doublecloud.kafka.v1.UserSpecR\x08userSpec\"\xae\x03\n\x11UpdateUserRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1b\n\tuser_name\x18\x02 \x01(\tR\x08userName\x12S\n\x0bupdate_spec\x18\x03 \x01(\x0b\x32\x32.doublecloud.kafka.v1.UpdateUserRequest.UpdateSpecR\nupdateSpec\x1a\x87\x02\n\nUpdateSpec\x12\x38\n\x08password\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08password\x12\x66\n\x0bpermissions\x18\x02 \x01(\x0b\x32\x44.doublecloud.kafka.v1.UpdateUserRequest.UpdateSpec.UpdatePermissionsR\x0bpermissions\x1aW\n\x11UpdatePermissions\x12\x42\n\x0bpermissions\x18\x01 \x03(\x0b\x32 .doublecloud.kafka.v1.PermissionR\x0bpermissions\"O\n\x11\x44\x65leteUserRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1b\n\tuser_name\x18\x02 \x01(\tR\x08userName\"\x9a\x01\n\x1aGrantUserPermissionRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1b\n\tuser_name\x18\x02 \x01(\tR\x08userName\x12@\n\npermission\x18\x03 \x01(\x0b\x32 .doublecloud.kafka.v1.PermissionR\npermission\"\x9b\x01\n\x1bRevokeUserPermissionRequest\x12\x1d\n\ncluster_id\x18\x01 \x01(\tR\tclusterId\x12\x1b\n\tuser_name\x18\x02 \x01(\tR\x08userName\x12@\n\npermission\x18\x03 \x01(\x0b\x32 .doublecloud.kafka.v1.PermissionR\npermission2\xdb\x04\n\x0bUserService\x12G\n\x03Get\x12$.doublecloud.kafka.v1.GetUserRequest\x1a\x1a.doublecloud.kafka.v1.User\x12W\n\x04List\x12&.doublecloud.kafka.v1.ListUsersRequest\x1a\'.doublecloud.kafka.v1.ListUsersResponse\x12L\n\x06\x43reate\x12\'.doublecloud.kafka.v1.CreateUserRequest\x1a\x19.doublecloud.v1.Operation\x12L\n\x06Update\x12\'.doublecloud.kafka.v1.UpdateUserRequest\x1a\x19.doublecloud.v1.Operation\x12L\n\x06\x44\x65lete\x12\'.doublecloud.kafka.v1.DeleteUserRequest\x1a\x19.doublecloud.v1.Operation\x12^\n\x0fGrantPermission\x12\x30.doublecloud.kafka.v1.GrantUserPermissionRequest\x1a\x19.doublecloud.v1.Operation\x12`\n\x10RevokePermission\x12\x31.doublecloud.kafka.v1.RevokeUserPermissionRequest\x1a\x19.doublecloud.v1.OperationB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.kafka.v1.user_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafka'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafka'
   _globals['_GETUSERREQUEST']._serialized_start=191
   _globals['_GETUSERREQUEST']._serialized_end=267
   _globals['_LISTUSERSREQUEST']._serialized_start=269
   _globals['_LISTUSERSREQUEST']._serialized_end=366
   _globals['_LISTUSERSRESPONSE']._serialized_start=368
   _globals['_LISTUSERSRESPONSE']._serialized_end=492
   _globals['_CREATEUSERREQUEST']._serialized_start=494
```

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/user_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/kafka/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/user_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/version_pb2.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/version_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/kafka/v1/version.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"doublecloud/kafka/v1/version.proto\x12\x14\x64oublecloud.kafka.v1\"p\n\x07Version\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1e\n\ndeprecated\x18\x03 \x01(\x08R\ndeprecated\x12!\n\x0cupdatable_to\x18\x04 \x03(\tR\x0bupdatableToB7Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafkab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"doublecloud/kafka/v1/version.proto\x12\x14\x64oublecloud.kafka.v1\"p\n\x07Version\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1e\n\ndeprecated\x18\x03 \x01(\x08R\ndeprecated\x12!\n\x0cupdatable_to\x18\x04 \x03(\tR\x0bupdatableToB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.kafka.v1.version_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafka'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafka'
   _globals['_VERSION']._serialized_start=60
   _globals['_VERSION']._serialized_end=172
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/version_pb2.pyi` & `doublecloud-0.6.0/doublecloud/kafka/v1/version_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/version_service_pb2.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/version_service_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/kafka/v1/version_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 from doublecloud.kafka.v1 import version_pb2 as doublecloud_dot_kafka_dot_v1_dot_version__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*doublecloud/kafka/v1/version_service.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1b\x64oublecloud/v1/paging.proto\x1a\"doublecloud/kafka/v1/version.proto\"E\n\x13ListVersionsRequest\x12.\n\x06paging\x18\x01 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x88\x01\n\x14ListVersionsResponse\x12\x39\n\x08versions\x18\x01 \x03(\x0b\x32\x1d.doublecloud.kafka.v1.VersionR\x08versions\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage2o\n\x0eVersionService\x12]\n\x04List\x12).doublecloud.kafka.v1.ListVersionsRequest\x1a*.doublecloud.kafka.v1.ListVersionsResponseB7Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafkab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*doublecloud/kafka/v1/version_service.proto\x12\x14\x64oublecloud.kafka.v1\x1a\x1b\x64oublecloud/v1/paging.proto\x1a\"doublecloud/kafka/v1/version.proto\"E\n\x13ListVersionsRequest\x12.\n\x06paging\x18\x01 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x88\x01\n\x14ListVersionsResponse\x12\x39\n\x08versions\x18\x01 \x03(\x0b\x32\x1d.doublecloud.kafka.v1.VersionR\x08versions\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage2o\n\x0eVersionService\x12]\n\x04List\x12).doublecloud.kafka.v1.ListVersionsRequest\x1a*.doublecloud.kafka.v1.ListVersionsResponseB?Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafkab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.kafka.v1.version_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/kafka/v1;kafka'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/kafka/v1;kafka'
   _globals['_LISTVERSIONSREQUEST']._serialized_start=133
   _globals['_LISTVERSIONSREQUEST']._serialized_end=202
   _globals['_LISTVERSIONSRESPONSE']._serialized_start=205
   _globals['_LISTVERSIONSRESPONSE']._serialized_end=341
   _globals['_VERSIONSERVICE']._serialized_start=343
   _globals['_VERSIONSERVICE']._serialized_end=454
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/version_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/kafka/v1/version_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/kafka/v1/version_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/kafka/v1/version_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/network/v1/network_connection_pb2.py` & `doublecloud-0.6.0/doublecloud/network/v1/network_connection_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/network/v1/network_connection.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/doublecloud/network/v1/network_connection.proto\x12\x16\x64oublecloud.network.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\xff\x04\n\x11NetworkConnection\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nnetwork_id\x18\x02 \x01(\tR\tnetworkId\x12\x44\n\x03\x61ws\x18\x04 \x01(\x0b\x32\x30.doublecloud.network.v1.AWSNetworkConnectionInfoH\x00R\x03\x61ws\x12;\n\x0b\x63reate_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12 \n\x0b\x64\x65scription\x18\x08 \x01(\tR\x0b\x64\x65scription\x12Y\n\x06status\x18\t \x01(\x0e\x32\x41.doublecloud.network.v1.NetworkConnection.NetworkConnectionStatusR\x06status\x12#\n\rstatus_reason\x18\n \x01(\tR\x0cstatusReason\"\x82\x02\n\x17NetworkConnectionStatus\x12%\n!NETWORK_CONNECTION_STATUS_INVALID\x10\x00\x12&\n\"NETWORK_CONNECTION_STATUS_CREATING\x10\x01\x12%\n!NETWORK_CONNECTION_STATUS_PENDING\x10\x02\x12$\n NETWORK_CONNECTION_STATUS_ACTIVE\x10\x03\x12&\n\"NETWORK_CONNECTION_STATUS_DELETING\x10\x04\x12#\n\x1fNETWORK_CONNECTION_STATUS_ERROR\x10\x05\x42\x11\n\x0f\x63onnection_info\"w\n\x18\x41WSNetworkConnectionInfo\x12S\n\x07peering\x18\x01 \x01(\x0b\x32\x37.doublecloud.network.v1.AWSNetworkConnectionPeeringInfoH\x00R\x07peeringB\x06\n\x04type\"\xe6\x02\n\x1f\x41WSNetworkConnectionPeeringInfo\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12\x1d\n\naccount_id\x18\x02 \x01(\tR\taccountId\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12&\n\x0fipv4_cidr_block\x18\x04 \x01(\tR\ripv4CidrBlock\x12&\n\x0fipv6_cidr_block\x18\x05 \x01(\tR\ripv6CidrBlock\x12\x32\n\x15peering_connection_id\x18\x06 \x01(\tR\x13peeringConnectionId\x12\x35\n\x17managed_ipv4_cidr_block\x18\x07 \x01(\tR\x14managedIpv4CidrBlock\x12\x35\n\x17managed_ipv6_cidr_block\x18\x08 \x01(\tR\x14managedIpv6CidrBlockB;Z9github.com/doublecloud/api/doublecloud/network/v1;networkb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/doublecloud/network/v1/network_connection.proto\x12\x16\x64oublecloud.network.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\xff\x04\n\x11NetworkConnection\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nnetwork_id\x18\x02 \x01(\tR\tnetworkId\x12\x44\n\x03\x61ws\x18\x04 \x01(\x0b\x32\x30.doublecloud.network.v1.AWSNetworkConnectionInfoH\x00R\x03\x61ws\x12;\n\x0b\x63reate_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12 \n\x0b\x64\x65scription\x18\x08 \x01(\tR\x0b\x64\x65scription\x12Y\n\x06status\x18\t \x01(\x0e\x32\x41.doublecloud.network.v1.NetworkConnection.NetworkConnectionStatusR\x06status\x12#\n\rstatus_reason\x18\n \x01(\tR\x0cstatusReason\"\x82\x02\n\x17NetworkConnectionStatus\x12%\n!NETWORK_CONNECTION_STATUS_INVALID\x10\x00\x12&\n\"NETWORK_CONNECTION_STATUS_CREATING\x10\x01\x12%\n!NETWORK_CONNECTION_STATUS_PENDING\x10\x02\x12$\n NETWORK_CONNECTION_STATUS_ACTIVE\x10\x03\x12&\n\"NETWORK_CONNECTION_STATUS_DELETING\x10\x04\x12#\n\x1fNETWORK_CONNECTION_STATUS_ERROR\x10\x05\x42\x11\n\x0f\x63onnection_info\"w\n\x18\x41WSNetworkConnectionInfo\x12S\n\x07peering\x18\x01 \x01(\x0b\x32\x37.doublecloud.network.v1.AWSNetworkConnectionPeeringInfoH\x00R\x07peeringB\x06\n\x04type\"\xe6\x02\n\x1f\x41WSNetworkConnectionPeeringInfo\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12\x1d\n\naccount_id\x18\x02 \x01(\tR\taccountId\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12&\n\x0fipv4_cidr_block\x18\x04 \x01(\tR\ripv4CidrBlock\x12&\n\x0fipv6_cidr_block\x18\x05 \x01(\tR\ripv6CidrBlock\x12\x32\n\x15peering_connection_id\x18\x06 \x01(\tR\x13peeringConnectionId\x12\x35\n\x17managed_ipv4_cidr_block\x18\x07 \x01(\tR\x14managedIpv4CidrBlock\x12\x35\n\x17managed_ipv6_cidr_block\x18\x08 \x01(\tR\x14managedIpv6CidrBlockBCZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;networkb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.network.v1.network_connection_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z9github.com/doublecloud/api/doublecloud/network/v1;network'
+  DESCRIPTOR._serialized_options = b'ZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;network'
   _globals['_NETWORKCONNECTION']._serialized_start=109
   _globals['_NETWORKCONNECTION']._serialized_end=748
   _globals['_NETWORKCONNECTION_NETWORKCONNECTIONSTATUS']._serialized_start=471
   _globals['_NETWORKCONNECTION_NETWORKCONNECTIONSTATUS']._serialized_end=729
   _globals['_AWSNETWORKCONNECTIONINFO']._serialized_start=750
   _globals['_AWSNETWORKCONNECTIONINFO']._serialized_end=869
   _globals['_AWSNETWORKCONNECTIONPEERINGINFO']._serialized_start=872
```

### Comparing `doublecloud-0.5.0/doublecloud/network/v1/network_connection_pb2.pyi` & `doublecloud-0.6.0/doublecloud/network/v1/network_connection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/network/v1/network_connection_service_pb2.py` & `doublecloud-0.6.0/doublecloud/network/v1/network_connection_service_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/network/v1/network_connection_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.network.v1 import network_connection_pb2 as doublecloud_dot_network_dot_v1_dot_network__connection__pb2
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7doublecloud/network/v1/network_connection_service.proto\x12\x16\x64oublecloud.network.v1\x1a/doublecloud/network/v1/network_connection.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"Q\n\x1bGetNetworkConnectionRequest\x12\x32\n\x15network_connection_id\x18\x01 \x01(\tR\x13networkConnectionId\"n\n\x1dListNetworkConnectionsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\xb3\x01\n\x1eListNetworkConnectionsResponse\x12Z\n\x13network_connections\x18\x01 \x03(\x0b\x32).doublecloud.network.v1.NetworkConnectionR\x12networkConnections\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\xba\x01\n\x1e\x43reateNetworkConnectionRequest\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\x12M\n\x03\x61ws\x18\x03 \x01(\x0b\x32\x39.doublecloud.network.v1.CreateAWSNetworkConnectionRequestH\x00R\x03\x61ws\x12 \n\x0b\x64\x65scription\x18\x06 \x01(\tR\x0b\x64\x65scriptionB\x08\n\x06params\"\x89\x01\n!CreateAWSNetworkConnectionRequest\x12\\\n\x07peering\x18\x01 \x01(\x0b\x32@.doublecloud.network.v1.CreateAWSNetworkConnectionPeeringRequestH\x00R\x07peeringB\x06\n\x04type\"\xcd\x01\n(CreateAWSNetworkConnectionPeeringRequest\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12\x1d\n\naccount_id\x18\x02 \x01(\tR\taccountId\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12&\n\x0fipv4_cidr_block\x18\x04 \x01(\tR\ripv4CidrBlock\x12&\n\x0fipv6_cidr_block\x18\x05 \x01(\tR\ripv6CidrBlock\"T\n\x1e\x44\x65leteNetworkConnectionRequest\x12\x32\n\x15network_connection_id\x18\x01 \x01(\tR\x13networkConnectionId\"v\n\x1eUpdateNetworkConnectionRequest\x12\x32\n\x15network_connection_id\x18\x01 \x01(\tR\x13networkConnectionId\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription2\xb2\x03\n\x18NetworkConnectionService\x12\x65\n\x03Get\x12\x33.doublecloud.network.v1.GetNetworkConnectionRequest\x1a).doublecloud.network.v1.NetworkConnection\x12u\n\x04List\x12\x35.doublecloud.network.v1.ListNetworkConnectionsRequest\x1a\x36.doublecloud.network.v1.ListNetworkConnectionsResponse\x12[\n\x06\x43reate\x12\x36.doublecloud.network.v1.CreateNetworkConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12[\n\x06\x44\x65lete\x12\x36.doublecloud.network.v1.DeleteNetworkConnectionRequest\x1a\x19.doublecloud.v1.OperationB;Z9github.com/doublecloud/api/doublecloud/network/v1;networkb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7doublecloud/network/v1/network_connection_service.proto\x12\x16\x64oublecloud.network.v1\x1a/doublecloud/network/v1/network_connection.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"Q\n\x1bGetNetworkConnectionRequest\x12\x32\n\x15network_connection_id\x18\x01 \x01(\tR\x13networkConnectionId\"n\n\x1dListNetworkConnectionsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\xb3\x01\n\x1eListNetworkConnectionsResponse\x12Z\n\x13network_connections\x18\x01 \x03(\x0b\x32).doublecloud.network.v1.NetworkConnectionR\x12networkConnections\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\xba\x01\n\x1e\x43reateNetworkConnectionRequest\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\x12M\n\x03\x61ws\x18\x03 \x01(\x0b\x32\x39.doublecloud.network.v1.CreateAWSNetworkConnectionRequestH\x00R\x03\x61ws\x12 \n\x0b\x64\x65scription\x18\x06 \x01(\tR\x0b\x64\x65scriptionB\x08\n\x06params\"\x89\x01\n!CreateAWSNetworkConnectionRequest\x12\\\n\x07peering\x18\x01 \x01(\x0b\x32@.doublecloud.network.v1.CreateAWSNetworkConnectionPeeringRequestH\x00R\x07peeringB\x06\n\x04type\"\xcd\x01\n(CreateAWSNetworkConnectionPeeringRequest\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12\x1d\n\naccount_id\x18\x02 \x01(\tR\taccountId\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12&\n\x0fipv4_cidr_block\x18\x04 \x01(\tR\ripv4CidrBlock\x12&\n\x0fipv6_cidr_block\x18\x05 \x01(\tR\ripv6CidrBlock\"T\n\x1e\x44\x65leteNetworkConnectionRequest\x12\x32\n\x15network_connection_id\x18\x01 \x01(\tR\x13networkConnectionId\"v\n\x1eUpdateNetworkConnectionRequest\x12\x32\n\x15network_connection_id\x18\x01 \x01(\tR\x13networkConnectionId\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription2\xb2\x03\n\x18NetworkConnectionService\x12\x65\n\x03Get\x12\x33.doublecloud.network.v1.GetNetworkConnectionRequest\x1a).doublecloud.network.v1.NetworkConnection\x12u\n\x04List\x12\x35.doublecloud.network.v1.ListNetworkConnectionsRequest\x1a\x36.doublecloud.network.v1.ListNetworkConnectionsResponse\x12[\n\x06\x43reate\x12\x36.doublecloud.network.v1.CreateNetworkConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12[\n\x06\x44\x65lete\x12\x36.doublecloud.network.v1.DeleteNetworkConnectionRequest\x1a\x19.doublecloud.v1.OperationBCZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;networkb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.network.v1.network_connection_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z9github.com/doublecloud/api/doublecloud/network/v1;network'
+  DESCRIPTOR._serialized_options = b'ZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;network'
   _globals['_GETNETWORKCONNECTIONREQUEST']._serialized_start=193
   _globals['_GETNETWORKCONNECTIONREQUEST']._serialized_end=274
   _globals['_LISTNETWORKCONNECTIONSREQUEST']._serialized_start=276
   _globals['_LISTNETWORKCONNECTIONSREQUEST']._serialized_end=386
   _globals['_LISTNETWORKCONNECTIONSRESPONSE']._serialized_start=389
   _globals['_LISTNETWORKCONNECTIONSRESPONSE']._serialized_end=568
   _globals['_CREATENETWORKCONNECTIONREQUEST']._serialized_start=571
```

### Comparing `doublecloud-0.5.0/doublecloud/network/v1/network_connection_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/network/v1/network_connection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/network/v1/network_connection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/network/v1/network_pb2.py` & `doublecloud-0.6.0/doublecloud/network/v1/network_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/network/v1/network.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$doublecloud/network/v1/network.proto\x12\x16\x64oublecloud.network.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xb9\x05\n\x07Network\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x03 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x04 \x01(\tR\x08regionId\x12;\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x07 \x01(\tR\x0b\x64\x65scription\x12&\n\x0fipv4_cidr_block\x18\x08 \x01(\tR\ripv4CidrBlock\x12&\n\x0fipv6_cidr_block\x18\t \x01(\tR\ripv6CidrBlock\x12\x45\n\x06status\x18\n \x01(\x0e\x32-.doublecloud.network.v1.Network.NetworkStatusR\x06status\x12#\n\rstatus_reason\x18\x0b \x01(\tR\x0cstatusReason\x12@\n\x03\x61ws\x18\x0c \x01(\x0b\x32,.doublecloud.network.v1.AwsExternalResourcesH\x00R\x03\x61ws\x12\x1f\n\x0bis_external\x18\r \x01(\x08R\nisExternal\"\x9a\x01\n\rNetworkStatus\x12\x1a\n\x16NETWORK_STATUS_INVALID\x10\x00\x12\x1b\n\x17NETWORK_STATUS_CREATING\x10\x01\x12\x19\n\x15NETWORK_STATUS_ACTIVE\x10\x02\x12\x1b\n\x17NETWORK_STATUS_DELETING\x10\x03\x12\x18\n\x14NETWORK_STATUS_ERROR\x10\x04\x42\x14\n\x12\x65xternal_resources\"\xdf\x03\n\x14\x41wsExternalResources\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12M\n\x07subnets\x18\x02 \x03(\x0b\x32\x33.doublecloud.network.v1.AwsExternalResources.SubnetR\x07subnets\x12*\n\x11security_group_id\x18\x03 \x01(\tR\x0fsecurityGroupId\x12;\n\naccount_id\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\taccountId\x12>\n\x0ciam_role_arn\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\niamRoleArn\x12\x37\n\x08stack_id\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x07stackId\x12L\n\x13\x63\x66_template_version\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x11\x63\x66TemplateVersion\x1a\x31\n\x06Subnet\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07zone_id\x18\x02 \x01(\tR\x06zoneIdB;Z9github.com/doublecloud/api/doublecloud/network/v1;networkb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$doublecloud/network/v1/network.proto\x12\x16\x64oublecloud.network.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xb9\x05\n\x07Network\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x03 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x04 \x01(\tR\x08regionId\x12;\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x07 \x01(\tR\x0b\x64\x65scription\x12&\n\x0fipv4_cidr_block\x18\x08 \x01(\tR\ripv4CidrBlock\x12&\n\x0fipv6_cidr_block\x18\t \x01(\tR\ripv6CidrBlock\x12\x45\n\x06status\x18\n \x01(\x0e\x32-.doublecloud.network.v1.Network.NetworkStatusR\x06status\x12#\n\rstatus_reason\x18\x0b \x01(\tR\x0cstatusReason\x12@\n\x03\x61ws\x18\x0c \x01(\x0b\x32,.doublecloud.network.v1.AwsExternalResourcesH\x00R\x03\x61ws\x12\x1f\n\x0bis_external\x18\r \x01(\x08R\nisExternal\"\x9a\x01\n\rNetworkStatus\x12\x1a\n\x16NETWORK_STATUS_INVALID\x10\x00\x12\x1b\n\x17NETWORK_STATUS_CREATING\x10\x01\x12\x19\n\x15NETWORK_STATUS_ACTIVE\x10\x02\x12\x1b\n\x17NETWORK_STATUS_DELETING\x10\x03\x12\x18\n\x14NETWORK_STATUS_ERROR\x10\x04\x42\x14\n\x12\x65xternal_resources\"\xdf\x03\n\x14\x41wsExternalResources\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12M\n\x07subnets\x18\x02 \x03(\x0b\x32\x33.doublecloud.network.v1.AwsExternalResources.SubnetR\x07subnets\x12*\n\x11security_group_id\x18\x03 \x01(\tR\x0fsecurityGroupId\x12;\n\naccount_id\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\taccountId\x12>\n\x0ciam_role_arn\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\niamRoleArn\x12\x37\n\x08stack_id\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x07stackId\x12L\n\x13\x63\x66_template_version\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x11\x63\x66TemplateVersion\x1a\x31\n\x06Subnet\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x17\n\x07zone_id\x18\x02 \x01(\tR\x06zoneIdBCZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;networkb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.network.v1.network_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z9github.com/doublecloud/api/doublecloud/network/v1;network'
+  DESCRIPTOR._serialized_options = b'ZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;network'
   _globals['_NETWORK']._serialized_start=130
   _globals['_NETWORK']._serialized_end=827
   _globals['_NETWORK_NETWORKSTATUS']._serialized_start=651
   _globals['_NETWORK_NETWORKSTATUS']._serialized_end=805
   _globals['_AWSEXTERNALRESOURCES']._serialized_start=830
   _globals['_AWSEXTERNALRESOURCES']._serialized_end=1309
   _globals['_AWSEXTERNALRESOURCES_SUBNET']._serialized_start=1260
```

### Comparing `doublecloud-0.5.0/doublecloud/network/v1/network_pb2.pyi` & `doublecloud-0.6.0/doublecloud/network/v1/network_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/network/v1/network_service_pb2.py` & `doublecloud-0.6.0/doublecloud/network/v1/network_service_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/network/v1/network_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.network.v1 import network_pb2 as doublecloud_dot_network_dot_v1_dot_network__pb2
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,doublecloud/network/v1/network_service.proto\x12\x16\x64oublecloud.network.v1\x1a$doublecloud/network/v1/network.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"2\n\x11GetNetworkRequest\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\"d\n\x13ListNetworksRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x8a\x01\n\x14ListNetworksResponse\x12;\n\x08networks\x18\x01 \x03(\x0b\x32\x1f.doublecloud.network.v1.NetworkR\x08networks\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\xcf\x01\n\x14\x43reateNetworkRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x02 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12&\n\x0fipv4_cidr_block\x18\x06 \x01(\tR\ripv4CidrBlock\"5\n\x14\x44\x65leteNetworkRequest\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\"\xb6\x01\n\x14ImportNetworkRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12?\n\x03\x61ws\x18\x04 \x01(\x0b\x32+.doublecloud.network.v1.ImportAWSVPCRequestH\x00R\x03\x61wsB\x08\n\x06params\"\xbf\x01\n\x13ImportAWSVPCRequest\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12\x1b\n\tregion_id\x18\x02 \x01(\tR\x08regionId\x12\x1d\n\naccount_id\x18\x03 \x01(\tR\taccountId\x12 \n\x0ciam_role_arn\x18\x04 \x01(\tR\niamRoleArn\x12\x19\n\x08stack_id\x18\x05 \x01(\tR\x07stackId\x12\x18\n\x07version\x18\x06 \x01(\tR\x07version2\xbf\x03\n\x0eNetworkService\x12Q\n\x03Get\x12).doublecloud.network.v1.GetNetworkRequest\x1a\x1f.doublecloud.network.v1.Network\x12\x61\n\x04List\x12+.doublecloud.network.v1.ListNetworksRequest\x1a,.doublecloud.network.v1.ListNetworksResponse\x12Q\n\x06\x43reate\x12,.doublecloud.network.v1.CreateNetworkRequest\x1a\x19.doublecloud.v1.Operation\x12Q\n\x06\x44\x65lete\x12,.doublecloud.network.v1.DeleteNetworkRequest\x1a\x19.doublecloud.v1.Operation\x12Q\n\x06Import\x12,.doublecloud.network.v1.ImportNetworkRequest\x1a\x19.doublecloud.v1.OperationB;Z9github.com/doublecloud/api/doublecloud/network/v1;networkb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,doublecloud/network/v1/network_service.proto\x12\x16\x64oublecloud.network.v1\x1a$doublecloud/network/v1/network.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\x1a\x1egoogle/protobuf/wrappers.proto\"2\n\x11GetNetworkRequest\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\"\xb7\x03\n\x13ListNetworksRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\x12J\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x32.doublecloud.network.v1.ListNetworksRequest.FilterR\x06\x66ilter\x1a\x84\x02\n\x06\x46ilter\x12;\n\ncloud_type\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\tcloudType\x12\x39\n\tregion_id\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x08regionId\x12\x45\n\x06status\x18\x03 \x01(\x0e\x32-.doublecloud.network.v1.Network.NetworkStatusR\x06status\x12;\n\x0bis_external\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\nisExternal\"\x8a\x01\n\x14ListNetworksResponse\x12;\n\x08networks\x18\x01 \x03(\x0b\x32\x1f.doublecloud.network.v1.NetworkR\x08networks\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\xcf\x01\n\x14\x43reateNetworkRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x1d\n\ncloud_type\x18\x02 \x01(\tR\tcloudType\x12\x1b\n\tregion_id\x18\x03 \x01(\tR\x08regionId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12&\n\x0fipv4_cidr_block\x18\x06 \x01(\tR\ripv4CidrBlock\"5\n\x14\x44\x65leteNetworkRequest\x12\x1d\n\nnetwork_id\x18\x01 \x01(\tR\tnetworkId\"\xb6\x01\n\x14ImportNetworkRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12?\n\x03\x61ws\x18\x04 \x01(\x0b\x32+.doublecloud.network.v1.ImportAWSVPCRequestH\x00R\x03\x61wsB\x08\n\x06params\"\xbf\x01\n\x13ImportAWSVPCRequest\x12\x15\n\x06vpc_id\x18\x01 \x01(\tR\x05vpcId\x12\x1b\n\tregion_id\x18\x02 \x01(\tR\x08regionId\x12\x1d\n\naccount_id\x18\x03 \x01(\tR\taccountId\x12 \n\x0ciam_role_arn\x18\x04 \x01(\tR\niamRoleArn\x12\x19\n\x08stack_id\x18\x05 \x01(\tR\x07stackId\x12\x18\n\x07version\x18\x06 \x01(\tR\x07version2\xbf\x03\n\x0eNetworkService\x12Q\n\x03Get\x12).doublecloud.network.v1.GetNetworkRequest\x1a\x1f.doublecloud.network.v1.Network\x12\x61\n\x04List\x12+.doublecloud.network.v1.ListNetworksRequest\x1a,.doublecloud.network.v1.ListNetworksResponse\x12Q\n\x06\x43reate\x12,.doublecloud.network.v1.CreateNetworkRequest\x1a\x19.doublecloud.v1.Operation\x12Q\n\x06\x44\x65lete\x12,.doublecloud.network.v1.DeleteNetworkRequest\x1a\x19.doublecloud.v1.Operation\x12Q\n\x06Import\x12,.doublecloud.network.v1.ImportNetworkRequest\x1a\x19.doublecloud.v1.OperationBCZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;networkb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.network.v1.network_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z9github.com/doublecloud/api/doublecloud/network/v1;network'
-  _globals['_GETNETWORKREQUEST']._serialized_start=171
-  _globals['_GETNETWORKREQUEST']._serialized_end=221
-  _globals['_LISTNETWORKSREQUEST']._serialized_start=223
-  _globals['_LISTNETWORKSREQUEST']._serialized_end=323
-  _globals['_LISTNETWORKSRESPONSE']._serialized_start=326
-  _globals['_LISTNETWORKSRESPONSE']._serialized_end=464
-  _globals['_CREATENETWORKREQUEST']._serialized_start=467
-  _globals['_CREATENETWORKREQUEST']._serialized_end=674
-  _globals['_DELETENETWORKREQUEST']._serialized_start=676
-  _globals['_DELETENETWORKREQUEST']._serialized_end=729
-  _globals['_IMPORTNETWORKREQUEST']._serialized_start=732
-  _globals['_IMPORTNETWORKREQUEST']._serialized_end=914
-  _globals['_IMPORTAWSVPCREQUEST']._serialized_start=917
-  _globals['_IMPORTAWSVPCREQUEST']._serialized_end=1108
-  _globals['_NETWORKSERVICE']._serialized_start=1111
-  _globals['_NETWORKSERVICE']._serialized_end=1558
+  DESCRIPTOR._serialized_options = b'ZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;network'
+  _globals['_GETNETWORKREQUEST']._serialized_start=203
+  _globals['_GETNETWORKREQUEST']._serialized_end=253
+  _globals['_LISTNETWORKSREQUEST']._serialized_start=256
+  _globals['_LISTNETWORKSREQUEST']._serialized_end=695
+  _globals['_LISTNETWORKSREQUEST_FILTER']._serialized_start=435
+  _globals['_LISTNETWORKSREQUEST_FILTER']._serialized_end=695
+  _globals['_LISTNETWORKSRESPONSE']._serialized_start=698
+  _globals['_LISTNETWORKSRESPONSE']._serialized_end=836
+  _globals['_CREATENETWORKREQUEST']._serialized_start=839
+  _globals['_CREATENETWORKREQUEST']._serialized_end=1046
+  _globals['_DELETENETWORKREQUEST']._serialized_start=1048
+  _globals['_DELETENETWORKREQUEST']._serialized_end=1101
+  _globals['_IMPORTNETWORKREQUEST']._serialized_start=1104
+  _globals['_IMPORTNETWORKREQUEST']._serialized_end=1286
+  _globals['_IMPORTAWSVPCREQUEST']._serialized_start=1289
+  _globals['_IMPORTAWSVPCREQUEST']._serialized_end=1480
+  _globals['_NETWORKSERVICE']._serialized_start=1483
+  _globals['_NETWORKSERVICE']._serialized_end=1930
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/network/v1/network_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/network/v1/network_service_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 from doublecloud.network.v1 import network_pb2 as _network_pb2
 from doublecloud.v1 import operation_pb2 as _operation_pb2
 from doublecloud.v1 import paging_pb2 as _paging_pb2
+from google.protobuf import wrappers_pb2 as _wrappers_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class GetNetworkRequest(_message.Message):
     __slots__ = ["network_id"]
     NETWORK_ID_FIELD_NUMBER: _ClassVar[int]
     network_id: str
     def __init__(self, network_id: _Optional[str] = ...) -> None: ...
 
 class ListNetworksRequest(_message.Message):
-    __slots__ = ["project_id", "paging"]
+    __slots__ = ["project_id", "paging", "filter"]
+    class Filter(_message.Message):
+        __slots__ = ["cloud_type", "region_id", "status", "is_external"]
+        CLOUD_TYPE_FIELD_NUMBER: _ClassVar[int]
+        REGION_ID_FIELD_NUMBER: _ClassVar[int]
+        STATUS_FIELD_NUMBER: _ClassVar[int]
+        IS_EXTERNAL_FIELD_NUMBER: _ClassVar[int]
+        cloud_type: _wrappers_pb2.StringValue
+        region_id: _wrappers_pb2.StringValue
+        status: _network_pb2.Network.NetworkStatus
+        is_external: _wrappers_pb2.BoolValue
+        def __init__(self, cloud_type: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., region_id: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., status: _Optional[_Union[_network_pb2.Network.NetworkStatus, str]] = ..., is_external: _Optional[_Union[_wrappers_pb2.BoolValue, _Mapping]] = ...) -> None: ...
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     PAGING_FIELD_NUMBER: _ClassVar[int]
+    FILTER_FIELD_NUMBER: _ClassVar[int]
     project_id: str
     paging: _paging_pb2.Paging
-    def __init__(self, project_id: _Optional[str] = ..., paging: _Optional[_Union[_paging_pb2.Paging, _Mapping]] = ...) -> None: ...
+    filter: ListNetworksRequest.Filter
+    def __init__(self, project_id: _Optional[str] = ..., paging: _Optional[_Union[_paging_pb2.Paging, _Mapping]] = ..., filter: _Optional[_Union[ListNetworksRequest.Filter, _Mapping]] = ...) -> None: ...
 
 class ListNetworksResponse(_message.Message):
     __slots__ = ["networks", "next_page"]
     NETWORKS_FIELD_NUMBER: _ClassVar[int]
     NEXT_PAGE_FIELD_NUMBER: _ClassVar[int]
     networks: _containers.RepeatedCompositeFieldContainer[_network_pb2.Network]
     next_page: _paging_pb2.NextPage
```

### Comparing `doublecloud-0.5.0/doublecloud/network/v1/network_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/network/v1/network_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/network/v1/operation_service_pb2.py` & `doublecloud-0.6.0/doublecloud/network/v1/operation_service_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/network/v1/operation_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.doublecloud/network/v1/operation_service.proto\x12\x16\x64oublecloud.network.v1\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"8\n\x13GetOperationRequest\x12!\n\x0coperation_id\x18\x01 \x01(\tR\x0boperationId\"f\n\x15ListOperationsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x8a\x01\n\x16ListOperationsResponse\x12\x39\n\noperations\x18\x01 \x03(\x0b\x32\x19.doublecloud.v1.OperationR\noperations\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage2\xc8\x01\n\x10OperationService\x12M\n\x03Get\x12+.doublecloud.network.v1.GetOperationRequest\x1a\x19.doublecloud.v1.Operation\x12\x65\n\x04List\x12-.doublecloud.network.v1.ListOperationsRequest\x1a..doublecloud.network.v1.ListOperationsResponseB;Z9github.com/doublecloud/api/doublecloud/network/v1;networkb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.doublecloud/network/v1/operation_service.proto\x12\x16\x64oublecloud.network.v1\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"8\n\x13GetOperationRequest\x12!\n\x0coperation_id\x18\x01 \x01(\tR\x0boperationId\"f\n\x15ListOperationsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12.\n\x06paging\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x06paging\"\x8a\x01\n\x16ListOperationsResponse\x12\x39\n\noperations\x18\x01 \x03(\x0b\x32\x19.doublecloud.v1.OperationR\noperations\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage2\xc8\x01\n\x10OperationService\x12M\n\x03Get\x12+.doublecloud.network.v1.GetOperationRequest\x1a\x19.doublecloud.v1.Operation\x12\x65\n\x04List\x12-.doublecloud.network.v1.ListOperationsRequest\x1a..doublecloud.network.v1.ListOperationsResponseBCZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;networkb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.network.v1.operation_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z9github.com/doublecloud/api/doublecloud/network/v1;network'
+  DESCRIPTOR._serialized_options = b'ZAgithub.com/doublecloud/go-genproto/doublecloud/network/v1;network'
   _globals['_GETOPERATIONREQUEST']._serialized_start=135
   _globals['_GETOPERATIONREQUEST']._serialized_end=191
   _globals['_LISTOPERATIONSREQUEST']._serialized_start=193
   _globals['_LISTOPERATIONSREQUEST']._serialized_end=295
   _globals['_LISTOPERATIONSRESPONSE']._serialized_start=298
   _globals['_LISTOPERATIONSRESPONSE']._serialized_end=436
   _globals['_OPERATIONSERVICE']._serialized_start=439
```

### Comparing `doublecloud-0.5.0/doublecloud/network/v1/operation_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/network/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/network/v1/operation_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/network/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n@doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xe1\x01\n\x0f\x41mazonAdsSource\x12\x1b\n\tclient_id\x18\x01 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x02 \x01(\tR\x0c\x63lientSecret\x12\x14\n\x05scope\x18\x03 \x01(\tR\x05scope\x12#\n\rrefresh_token\x18\x04 \x01(\tR\x0crefreshToken\x12\x1d\n\nstart_date\x18\x05 \x01(\tR\tstartDate\x12\x16\n\x06region\x18\x06 \x01(\tR\x06region\x12\x1a\n\x08profiles\x18\x07 \x03(\x01R\x08profilesBVZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n@doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xe1\x01\n\x0f\x41mazonAdsSource\x12\x1b\n\tclient_id\x18\x01 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x02 \x01(\tR\x0c\x63lientSecret\x12\x14\n\x05scope\x18\x03 \x01(\tR\x05scope\x12#\n\rrefresh_token\x18\x04 \x01(\tR\x0crefreshToken\x12\x1d\n\nstart_date\x18\x05 \x01(\tR\tstartDate\x12\x16\n\x06region\x18\x06 \x01(\tR\x06region\x12\x1a\n\x08profiles\x18\x07 \x03(\x01R\x08profilesB^Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.airbyte.amazon_ads_source_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
+  DESCRIPTOR._serialized_options = b'Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
   _globals['_AMAZONADSSOURCE']._serialized_start=111
   _globals['_AMAZONADSSOURCE']._serialized_end=336
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nEdoublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xa0\x01\n\x13\x41WSCloudTrailSource\x12\x1c\n\naws_key_id\x18\x01 \x01(\tR\x08\x61wsKeyId\x12$\n\x0e\x61ws_secret_key\x18\x02 \x01(\tR\x0c\x61wsSecretKey\x12&\n\x0f\x61ws_region_name\x18\x03 \x01(\tR\rawsRegionName\x12\x1d\n\nstart_date\x18\x04 \x01(\tR\tstartDateBVZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nEdoublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xa0\x01\n\x13\x41WSCloudTrailSource\x12\x1c\n\naws_key_id\x18\x01 \x01(\tR\x08\x61wsKeyId\x12$\n\x0e\x61ws_secret_key\x18\x02 \x01(\tR\x0c\x61wsSecretKey\x12&\n\x0f\x61ws_region_name\x18\x03 \x01(\tR\rawsRegionName\x12\x1d\n\nstart_date\x18\x04 \x01(\tR\tstartDateB^Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.airbyte.aws_cloud_trail_source_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
+  DESCRIPTOR._serialized_options = b'Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
   _globals['_AWSCLOUDTRAILSOURCE']._serialized_start=116
   _globals['_AWSCLOUDTRAILSOURCE']._serialized_end=276
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: doublecloud/transfer/v1/endpoint/airbyte/bigquery_source.proto
+# source: doublecloud/transfer/v1/endpoint/airbyte/instagram_source.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n>doublecloud/transfer/v1/endpoint/airbyte/bigquery_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"y\n\x0e\x42igQuerySource\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x1d\n\ndataset_id\x18\x02 \x01(\tR\tdatasetId\x12)\n\x10\x63redentials_json\x18\x03 \x01(\tR\x0f\x63redentialsJsonBVZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n?doublecloud/transfer/v1/endpoint/airbyte/instagram_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"S\n\x0fInstagramSource\x12\x1d\n\nstart_date\x18\x01 \x01(\tR\tstartDate\x12!\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\tR\x0b\x61\x63\x63\x65ssTokenB^Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.airbyte.bigquery_source_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.airbyte.instagram_source_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
-  _globals['_BIGQUERYSOURCE']._serialized_start=108
-  _globals['_BIGQUERYSOURCE']._serialized_end=229
+  DESCRIPTOR._serialized_options = b'Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
+  _globals['_INSTAGRAMSOURCE']._serialized_start=109
+  _globals['_INSTAGRAMSOURCE']._serialized_end=192
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/bigquery_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHdoublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\x9d\'\n\x17\x46\x61\x63\x65\x62ookMarketingSource\x12\x1d\n\nstart_date\x18\x01 \x01(\tR\tstartDate\x12\x1d\n\naccount_id\x18\x03 \x01(\tR\taccountId\x12\x19\n\x08\x65nd_date\x18\x02 \x01(\tR\x07\x65ndDate\x12!\n\x0c\x61\x63\x63\x65ss_token\x18\x04 \x01(\tR\x0b\x61\x63\x63\x65ssToken\x12\'\n\x0finclude_deleted\x18\x05 \x01(\x08R\x0eincludeDeleted\x12\x34\n\x16\x66\x65tch_thumbnail_images\x18\x06 \x01(\x08R\x14\x66\x65tchThumbnailImages\x12x\n\x0f\x63ustom_insights\x18\x07 \x03(\x0b\x32O.doublecloud.transfer.v1.endpoint.airbyte.FacebookMarketingSource.InsightConfigR\x0e\x63ustomInsights\x1a\xf1\x02\n\rInsightConfig\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12_\n\x06\x66ields\x18\x02 \x03(\x0e\x32G.doublecloud.transfer.v1.endpoint.airbyte.FacebookMarketingSource.FieldR\x06\x66ields\x12k\n\nbreakdowns\x18\x03 \x03(\x0e\x32K.doublecloud.transfer.v1.endpoint.airbyte.FacebookMarketingSource.BreakdownR\nbreakdowns\x12~\n\x11\x61\x63tion_breakdowns\x18\x04 \x03(\x0e\x32Q.doublecloud.transfer.v1.endpoint.airbyte.FacebookMarketingSource.ActionBreakdownR\x10\x61\x63tionBreakdowns\"\xf3\x1a\n\x05\x46ield\x12\x15\n\x11\x46IELD_UNSPECIFIED\x10\x00\x12\x14\n\x10\x41\x43\x43OUNT_CURRENCY\x10\x01\x12\x0e\n\nACCOUNT_ID\x10\x02\x12\x10\n\x0c\x41\x43\x43OUNT_NAME\x10\x03\x12\x11\n\rACTION_VALUES\x10\x04\x12\x0b\n\x07\x41\x43TIONS\x10\x05\x12\x10\n\x0c\x41\x44_BID_VALUE\x10\x06\x12\x14\n\x10\x41\x44_CLICK_ACTIONS\x10\x07\x12\t\n\x05\x41\x44_ID\x10\x08\x12\x19\n\x15\x41\x44_IMPRESSION_ACTIONS\x10\t\x12\x0b\n\x07\x41\x44_NAME\x10\n\x12\x13\n\x0f\x41\x44SET_BID_VALUE\x10\x0b\x12\r\n\tADSET_END\x10\x0c\x12\x0c\n\x08\x41\x44SET_ID\x10\r\x12\x0e\n\nADSET_NAME\x10\x0e\x12\x0f\n\x0b\x41\x44SET_START\x10\x0f\x12\x11\n\rAGE_TARGETING\x10\x10\x12\x17\n\x13\x41TTRIBUTION_SETTING\x10\x11\x12\x0f\n\x0b\x41UCTION_BID\x10\x12\x12\x1b\n\x17\x41UCTION_COMPETITIVENESS\x10\x13\x12\x1e\n\x1a\x41UCTION_MAX_COMPETITOR_BID\x10\x14\x12\x0f\n\x0b\x42UYING_TYPE\x10\x15\x12\x0f\n\x0b\x43\x41MPAIGN_ID\x10\x16\x12\x11\n\rCAMPAIGN_NAME\x10\x17\x12\x1b\n\x17\x43\x41NVAS_AVG_VIEW_PERCENT\x10\x18\x12\x18\n\x14\x43\x41NVAS_AVG_VIEW_TIME\x10\x19\x12\x1b\n\x17\x43\x41TALOG_SEGMENT_ACTIONS\x10\x1a\x12\x19\n\x15\x43\x41TALOG_SEGMENT_VALUE\x10\x1b\x12.\n*CATALOG_SEGMENT_VALUE_MOBILE_PURCHASE_ROAS\x10\x1c\x12,\n(CATALOG_SEGMENT_VALUE_OMNI_PURCHASE_ROAS\x10\x1d\x12/\n+CATALOG_SEGMENT_VALUE_WEBSITE_PURCHASE_ROAS\x10\x1e\x12\n\n\x06\x43LICKS\x10\x1f\x12\x1b\n\x17\x43ONVERSION_RATE_RANKING\x10 \x12\x15\n\x11\x43ONVERSION_VALUES\x10!\x12\x0f\n\x0b\x43ONVERSIONS\x10\"\x12\x1e\n\x1a\x43ONVERTED_PRODUCT_QUANTITY\x10#\x12\x1b\n\x17\x43ONVERTED_PRODUCT_VALUE\x10$\x12\x1e\n\x1a\x43OST_PER_15_SEC_VIDEO_VIEW\x10%\x12(\n$COST_PER_2_SEC_CONTINUOUS_VIDEO_VIEW\x10&\x12\x18\n\x14\x43OST_PER_ACTION_TYPE\x10\'\x12\x15\n\x11\x43OST_PER_AD_CLICK\x10(\x12\x17\n\x13\x43OST_PER_CONVERSION\x10)\x12\x1e\n\x1a\x43OST_PER_DDA_COUNTBY_CONVS\x10*\x12#\n\x1f\x43OST_PER_ESTIMATED_AD_RECALLERS\x10+\x12\x1e\n\x1a\x43OST_PER_INLINE_LINK_CLICK\x10,\x12#\n\x1f\x43OST_PER_INLINE_POST_ENGAGEMENT\x10-\x12\'\n#COST_PER_ONE_THOUSAND_AD_IMPRESSION\x10.\x12\x1b\n\x17\x43OST_PER_OUTBOUND_CLICK\x10/\x12\x15\n\x11\x43OST_PER_THRUPLAY\x10\x30\x12\x1f\n\x1b\x43OST_PER_UNIQUE_ACTION_TYPE\x10\x31\x12\x19\n\x15\x43OST_PER_UNIQUE_CLICK\x10\x32\x12\x1e\n\x1a\x43OST_PER_UNIQUE_CONVERSION\x10\x33\x12%\n!COST_PER_UNIQUE_INLINE_LINK_CLICK\x10\x34\x12\"\n\x1e\x43OST_PER_UNIQUE_OUTBOUND_CLICK\x10\x35\x12\x07\n\x03\x43PC\x10\x36\x12\x07\n\x03\x43PM\x10\x37\x12\x07\n\x03\x43PP\x10\x38\x12\x10\n\x0c\x43REATED_TIME\x10\x39\x12\x07\n\x03\x43TR\x10:\x12\x0e\n\nDATE_START\x10;\x12\r\n\tDATE_STOP\x10<\x12\x15\n\x11\x44\x44\x41_COUNTBY_CONVS\x10=\x12\x0f\n\x0b\x44\x44\x41_RESULTS\x10>\x12\x1b\n\x17\x45NGAGEMENT_RATE_RANKING\x10?\x12\x1c\n\x18\x45STIMATED_AD_RECALL_RATE\x10@\x12(\n$ESTIMATED_AD_RECALL_RATE_LOWER_BOUND\x10\x41\x12(\n$ESTIMATED_AD_RECALL_RATE_UPPER_BOUND\x10\x42\x12\x1a\n\x16\x45STIMATED_AD_RECALLERS\x10\x43\x12&\n\"ESTIMATED_AD_RECALLERS_LOWER_BOUND\x10\x44\x12&\n\"ESTIMATED_AD_RECALLERS_UPPER_BOUND\x10\x45\x12\r\n\tFREQUENCY\x10\x46\x12\x19\n\x15\x46ULL_VIEW_IMPRESSIONS\x10G\x12\x13\n\x0f\x46ULL_VIEW_REACH\x10H\x12\x14\n\x10GENDER_TARGETING\x10I\x12\x0f\n\x0bIMPRESSIONS\x10J\x12\x19\n\x15INLINE_LINK_CLICK_CTR\x10K\x12\x16\n\x12INLINE_LINK_CLICKS\x10L\x12\x1a\n\x16INLINE_POST_ENGAGEMENT\x10M\x12%\n!INSTANT_EXPERIENCE_CLICKS_TO_OPEN\x10N\x12&\n\"INSTANT_EXPERIENCE_CLICKS_TO_START\x10O\x12&\n\"INSTANT_EXPERIENCE_OUTBOUND_CLICKS\x10P\x12\x1d\n\x19INTERACTIVE_COMPONENT_TAP\x10Q\x12\n\n\x06LABELS\x10R\x12\x0c\n\x08LOCATION\x10S\x12\x1c\n\x18MOBILE_APP_PURCHASE_ROAS\x10T\x12\r\n\tOBJECTIVE\x10U\x12\x15\n\x11OPTIMIZATION_GOAL\x10V\x12\x13\n\x0fOUTBOUND_CLICKS\x10W\x12\x17\n\x13OUTBOUND_CLICKS_CTR\x10X\x12\x13\n\x0fPLACE_PAGE_NAME\x10Y\x12\x11\n\rPURCHASE_ROAS\x10Z\x12+\n\'QUALIFYING_QUESTION_QUALIFY_ANSWER_RATE\x10[\x12\x13\n\x0fQUALITY_RANKING\x10\\\x12\x16\n\x12QUALITY_SCORE_ECTR\x10]\x12\x16\n\x12QUALITY_SCORE_ECVR\x10^\x12\x19\n\x15QUALITY_SCORE_ORGANIC\x10_\x12\t\n\x05REACH\x10`\x12\x10\n\x0cSOCIAL_SPEND\x10\x61\x12\t\n\x05SPEND\x10\x62\x12\x13\n\x0fTOTAL_POSTBACKS\x10\x63\x12\x12\n\x0eUNIQUE_ACTIONS\x10\x64\x12\x11\n\rUNIQUE_CLICKS\x10\x65\x12\x16\n\x12UNIQUE_CONVERSIONS\x10\x66\x12\x0e\n\nUNIQUE_CTR\x10g\x12 \n\x1cUNIQUE_INLINE_LINK_CLICK_CTR\x10h\x12\x1d\n\x19UNIQUE_INLINE_LINK_CLICKS\x10i\x12\x1a\n\x16UNIQUE_LINK_CLICKS_CTR\x10j\x12\x1a\n\x16UNIQUE_OUTBOUND_CLICKS\x10k\x12\x1e\n\x1aUNIQUE_OUTBOUND_CLICKS_CTR\x10l\x12\x31\n-UNIQUE_VIDEO_CONTINUOUS_2_SEC_WATCHED_ACTIONS\x10m\x12\x1c\n\x18UNIQUE_VIDEO_VIEW_15_SEC\x10n\x12\x10\n\x0cUPDATED_TIME\x10o\x12 \n\x1cVIDEO_15_SEC_WATCHED_ACTIONS\x10p\x12 \n\x1cVIDEO_30_SEC_WATCHED_ACTIONS\x10q\x12\"\n\x1eVIDEO_AVG_TIME_WATCHED_ACTIONS\x10r\x12*\n&VIDEO_CONTINUOUS_2_SEC_WATCHED_ACTIONS\x10s\x12\x1e\n\x1aVIDEO_P100_WATCHED_ACTIONS\x10t\x12\x1d\n\x19VIDEO_P25_WATCHED_ACTIONS\x10u\x12\x1d\n\x19VIDEO_P50_WATCHED_ACTIONS\x10v\x12\x1d\n\x19VIDEO_P75_WATCHED_ACTIONS\x10w\x12\x1d\n\x19VIDEO_P95_WATCHED_ACTIONS\x10x\x12\x16\n\x12VIDEO_PLAY_ACTIONS\x10y\x12\x1c\n\x18VIDEO_PLAY_CURVE_ACTIONS\x10z\x12)\n%VIDEO_PLAY_RETENTION_0_TO_15S_ACTIONS\x10{\x12*\n&VIDEO_PLAY_RETENTION_20_TO_60S_ACTIONS\x10|\x12&\n\"VIDEO_PLAY_RETENTION_GRAPH_ACTIONS\x10}\x12\"\n\x1eVIDEO_THRUPLAY_WATCHED_ACTIONS\x10~\x12\x1e\n\x1aVIDEO_TIME_WATCHED_ACTIONS\x10\x7f\x12\x10\n\x0bWEBSITE_CTR\x10\x80\x01\x12\x1a\n\x15WEBSITE_PURCHASE_ROAS\x10\x82\x01\x12\r\n\x08WISH_BID\x10\x83\x01\"\x98\x04\n\tBreakdown\x12\x19\n\x15\x42REAKDOWN_UNSPECIFIED\x10\x00\x12\x13\n\x0f\x41\x44_FORMAT_ASSET\x10\x01\x12\x07\n\x03\x41GE\x10\x02\x12\n\n\x06\x41PP_ID\x10\x03\x12\x0e\n\nBODY_ASSET\x10\x04\x12\x18\n\x14\x43\x41LL_TO_ACTION_ASSET\x10\x05\x12\x0b\n\x07\x43OUNTRY\x10\x06\x12\x15\n\x11\x44\x45SCRIPTION_ASSET\x10\x07\x12\x13\n\x0f\x44\x45VICE_PLATFORM\x10\x08\x12\x07\n\x03\x44MA\x10\t\x12\x13\n\x0f\x46REQUENCY_VALUE\x10\n\x12\n\n\x06GENDER\x10\x0b\x12\x33\n/HOURLY_STATS_AGGREGATED_BY_ADVERTISER_TIME_ZONE\x10\x0c\x12\x31\n-HOURLY_STATS_AGGREGATED_BY_AUDIENCE_TIME_ZONE\x10\r\x12\x0f\n\x0bIMAGE_ASSET\x10\x0e\x12\x15\n\x11IMPRESSION_DEVICE\x10\x0f\x12\x12\n\x0eLINK_URL_ASSET\x10\x10\x12\x11\n\rPLACE_PAGE_ID\x10\x11\x12\x15\n\x11PLATFORM_POSITION\x10\x12\x12\x0e\n\nPRODUCT_ID\x10\x13\x12\x16\n\x12PUBLISHER_PLATFORM\x10\x14\x12\n\n\x06REGION\x10\x15\x12\x16\n\x12SKAN_CONVERSION_ID\x10\x16\x12\x0f\n\x0bTITLE_ASSET\x10\x17\x12\x0e\n\nVIDEO_ASSE\x10\x18\"\xa7\x02\n\x0f\x41\x63tionBreakdown\x12 \n\x1c\x41\x43TION_BREAKDOWN_UNSPECIFIED\x10\x00\x12 \n\x1c\x41\x43TION_CANVAS_COMPONENT_NAME\x10\x01\x12\x1b\n\x17\x41\x43TION_CAROUSEL_CARD_ID\x10\x02\x12\x1d\n\x19\x41\x43TION_CAROUSEL_CARD_NAME\x10\x03\x12\x16\n\x12\x41\x43TION_DESTINATION\x10\x04\x12\x11\n\rACTION_DEVICE\x10\x05\x12\x13\n\x0f\x41\x43TION_REACTION\x10\x06\x12\x14\n\x10\x41\x43TION_TARGET_ID\x10\x07\x12\x0f\n\x0b\x41\x43TION_TYPE\x10\x08\x12\x16\n\x12\x41\x43TION_VIDEO_SOUND\x10\t\x12\x15\n\x11\x41\x43TION_VIDEO_TYPE\x10\nBVZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHdoublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\x9d\'\n\x17\x46\x61\x63\x65\x62ookMarketingSource\x12\x1d\n\nstart_date\x18\x01 \x01(\tR\tstartDate\x12\x1d\n\naccount_id\x18\x03 \x01(\tR\taccountId\x12\x19\n\x08\x65nd_date\x18\x02 \x01(\tR\x07\x65ndDate\x12!\n\x0c\x61\x63\x63\x65ss_token\x18\x04 \x01(\tR\x0b\x61\x63\x63\x65ssToken\x12\'\n\x0finclude_deleted\x18\x05 \x01(\x08R\x0eincludeDeleted\x12\x34\n\x16\x66\x65tch_thumbnail_images\x18\x06 \x01(\x08R\x14\x66\x65tchThumbnailImages\x12x\n\x0f\x63ustom_insights\x18\x07 \x03(\x0b\x32O.doublecloud.transfer.v1.endpoint.airbyte.FacebookMarketingSource.InsightConfigR\x0e\x63ustomInsights\x1a\xf1\x02\n\rInsightConfig\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12_\n\x06\x66ields\x18\x02 \x03(\x0e\x32G.doublecloud.transfer.v1.endpoint.airbyte.FacebookMarketingSource.FieldR\x06\x66ields\x12k\n\nbreakdowns\x18\x03 \x03(\x0e\x32K.doublecloud.transfer.v1.endpoint.airbyte.FacebookMarketingSource.BreakdownR\nbreakdowns\x12~\n\x11\x61\x63tion_breakdowns\x18\x04 \x03(\x0e\x32Q.doublecloud.transfer.v1.endpoint.airbyte.FacebookMarketingSource.ActionBreakdownR\x10\x61\x63tionBreakdowns\"\xf3\x1a\n\x05\x46ield\x12\x15\n\x11\x46IELD_UNSPECIFIED\x10\x00\x12\x14\n\x10\x41\x43\x43OUNT_CURRENCY\x10\x01\x12\x0e\n\nACCOUNT_ID\x10\x02\x12\x10\n\x0c\x41\x43\x43OUNT_NAME\x10\x03\x12\x11\n\rACTION_VALUES\x10\x04\x12\x0b\n\x07\x41\x43TIONS\x10\x05\x12\x10\n\x0c\x41\x44_BID_VALUE\x10\x06\x12\x14\n\x10\x41\x44_CLICK_ACTIONS\x10\x07\x12\t\n\x05\x41\x44_ID\x10\x08\x12\x19\n\x15\x41\x44_IMPRESSION_ACTIONS\x10\t\x12\x0b\n\x07\x41\x44_NAME\x10\n\x12\x13\n\x0f\x41\x44SET_BID_VALUE\x10\x0b\x12\r\n\tADSET_END\x10\x0c\x12\x0c\n\x08\x41\x44SET_ID\x10\r\x12\x0e\n\nADSET_NAME\x10\x0e\x12\x0f\n\x0b\x41\x44SET_START\x10\x0f\x12\x11\n\rAGE_TARGETING\x10\x10\x12\x17\n\x13\x41TTRIBUTION_SETTING\x10\x11\x12\x0f\n\x0b\x41UCTION_BID\x10\x12\x12\x1b\n\x17\x41UCTION_COMPETITIVENESS\x10\x13\x12\x1e\n\x1a\x41UCTION_MAX_COMPETITOR_BID\x10\x14\x12\x0f\n\x0b\x42UYING_TYPE\x10\x15\x12\x0f\n\x0b\x43\x41MPAIGN_ID\x10\x16\x12\x11\n\rCAMPAIGN_NAME\x10\x17\x12\x1b\n\x17\x43\x41NVAS_AVG_VIEW_PERCENT\x10\x18\x12\x18\n\x14\x43\x41NVAS_AVG_VIEW_TIME\x10\x19\x12\x1b\n\x17\x43\x41TALOG_SEGMENT_ACTIONS\x10\x1a\x12\x19\n\x15\x43\x41TALOG_SEGMENT_VALUE\x10\x1b\x12.\n*CATALOG_SEGMENT_VALUE_MOBILE_PURCHASE_ROAS\x10\x1c\x12,\n(CATALOG_SEGMENT_VALUE_OMNI_PURCHASE_ROAS\x10\x1d\x12/\n+CATALOG_SEGMENT_VALUE_WEBSITE_PURCHASE_ROAS\x10\x1e\x12\n\n\x06\x43LICKS\x10\x1f\x12\x1b\n\x17\x43ONVERSION_RATE_RANKING\x10 \x12\x15\n\x11\x43ONVERSION_VALUES\x10!\x12\x0f\n\x0b\x43ONVERSIONS\x10\"\x12\x1e\n\x1a\x43ONVERTED_PRODUCT_QUANTITY\x10#\x12\x1b\n\x17\x43ONVERTED_PRODUCT_VALUE\x10$\x12\x1e\n\x1a\x43OST_PER_15_SEC_VIDEO_VIEW\x10%\x12(\n$COST_PER_2_SEC_CONTINUOUS_VIDEO_VIEW\x10&\x12\x18\n\x14\x43OST_PER_ACTION_TYPE\x10\'\x12\x15\n\x11\x43OST_PER_AD_CLICK\x10(\x12\x17\n\x13\x43OST_PER_CONVERSION\x10)\x12\x1e\n\x1a\x43OST_PER_DDA_COUNTBY_CONVS\x10*\x12#\n\x1f\x43OST_PER_ESTIMATED_AD_RECALLERS\x10+\x12\x1e\n\x1a\x43OST_PER_INLINE_LINK_CLICK\x10,\x12#\n\x1f\x43OST_PER_INLINE_POST_ENGAGEMENT\x10-\x12\'\n#COST_PER_ONE_THOUSAND_AD_IMPRESSION\x10.\x12\x1b\n\x17\x43OST_PER_OUTBOUND_CLICK\x10/\x12\x15\n\x11\x43OST_PER_THRUPLAY\x10\x30\x12\x1f\n\x1b\x43OST_PER_UNIQUE_ACTION_TYPE\x10\x31\x12\x19\n\x15\x43OST_PER_UNIQUE_CLICK\x10\x32\x12\x1e\n\x1a\x43OST_PER_UNIQUE_CONVERSION\x10\x33\x12%\n!COST_PER_UNIQUE_INLINE_LINK_CLICK\x10\x34\x12\"\n\x1e\x43OST_PER_UNIQUE_OUTBOUND_CLICK\x10\x35\x12\x07\n\x03\x43PC\x10\x36\x12\x07\n\x03\x43PM\x10\x37\x12\x07\n\x03\x43PP\x10\x38\x12\x10\n\x0c\x43REATED_TIME\x10\x39\x12\x07\n\x03\x43TR\x10:\x12\x0e\n\nDATE_START\x10;\x12\r\n\tDATE_STOP\x10<\x12\x15\n\x11\x44\x44\x41_COUNTBY_CONVS\x10=\x12\x0f\n\x0b\x44\x44\x41_RESULTS\x10>\x12\x1b\n\x17\x45NGAGEMENT_RATE_RANKING\x10?\x12\x1c\n\x18\x45STIMATED_AD_RECALL_RATE\x10@\x12(\n$ESTIMATED_AD_RECALL_RATE_LOWER_BOUND\x10\x41\x12(\n$ESTIMATED_AD_RECALL_RATE_UPPER_BOUND\x10\x42\x12\x1a\n\x16\x45STIMATED_AD_RECALLERS\x10\x43\x12&\n\"ESTIMATED_AD_RECALLERS_LOWER_BOUND\x10\x44\x12&\n\"ESTIMATED_AD_RECALLERS_UPPER_BOUND\x10\x45\x12\r\n\tFREQUENCY\x10\x46\x12\x19\n\x15\x46ULL_VIEW_IMPRESSIONS\x10G\x12\x13\n\x0f\x46ULL_VIEW_REACH\x10H\x12\x14\n\x10GENDER_TARGETING\x10I\x12\x0f\n\x0bIMPRESSIONS\x10J\x12\x19\n\x15INLINE_LINK_CLICK_CTR\x10K\x12\x16\n\x12INLINE_LINK_CLICKS\x10L\x12\x1a\n\x16INLINE_POST_ENGAGEMENT\x10M\x12%\n!INSTANT_EXPERIENCE_CLICKS_TO_OPEN\x10N\x12&\n\"INSTANT_EXPERIENCE_CLICKS_TO_START\x10O\x12&\n\"INSTANT_EXPERIENCE_OUTBOUND_CLICKS\x10P\x12\x1d\n\x19INTERACTIVE_COMPONENT_TAP\x10Q\x12\n\n\x06LABELS\x10R\x12\x0c\n\x08LOCATION\x10S\x12\x1c\n\x18MOBILE_APP_PURCHASE_ROAS\x10T\x12\r\n\tOBJECTIVE\x10U\x12\x15\n\x11OPTIMIZATION_GOAL\x10V\x12\x13\n\x0fOUTBOUND_CLICKS\x10W\x12\x17\n\x13OUTBOUND_CLICKS_CTR\x10X\x12\x13\n\x0fPLACE_PAGE_NAME\x10Y\x12\x11\n\rPURCHASE_ROAS\x10Z\x12+\n\'QUALIFYING_QUESTION_QUALIFY_ANSWER_RATE\x10[\x12\x13\n\x0fQUALITY_RANKING\x10\\\x12\x16\n\x12QUALITY_SCORE_ECTR\x10]\x12\x16\n\x12QUALITY_SCORE_ECVR\x10^\x12\x19\n\x15QUALITY_SCORE_ORGANIC\x10_\x12\t\n\x05REACH\x10`\x12\x10\n\x0cSOCIAL_SPEND\x10\x61\x12\t\n\x05SPEND\x10\x62\x12\x13\n\x0fTOTAL_POSTBACKS\x10\x63\x12\x12\n\x0eUNIQUE_ACTIONS\x10\x64\x12\x11\n\rUNIQUE_CLICKS\x10\x65\x12\x16\n\x12UNIQUE_CONVERSIONS\x10\x66\x12\x0e\n\nUNIQUE_CTR\x10g\x12 \n\x1cUNIQUE_INLINE_LINK_CLICK_CTR\x10h\x12\x1d\n\x19UNIQUE_INLINE_LINK_CLICKS\x10i\x12\x1a\n\x16UNIQUE_LINK_CLICKS_CTR\x10j\x12\x1a\n\x16UNIQUE_OUTBOUND_CLICKS\x10k\x12\x1e\n\x1aUNIQUE_OUTBOUND_CLICKS_CTR\x10l\x12\x31\n-UNIQUE_VIDEO_CONTINUOUS_2_SEC_WATCHED_ACTIONS\x10m\x12\x1c\n\x18UNIQUE_VIDEO_VIEW_15_SEC\x10n\x12\x10\n\x0cUPDATED_TIME\x10o\x12 \n\x1cVIDEO_15_SEC_WATCHED_ACTIONS\x10p\x12 \n\x1cVIDEO_30_SEC_WATCHED_ACTIONS\x10q\x12\"\n\x1eVIDEO_AVG_TIME_WATCHED_ACTIONS\x10r\x12*\n&VIDEO_CONTINUOUS_2_SEC_WATCHED_ACTIONS\x10s\x12\x1e\n\x1aVIDEO_P100_WATCHED_ACTIONS\x10t\x12\x1d\n\x19VIDEO_P25_WATCHED_ACTIONS\x10u\x12\x1d\n\x19VIDEO_P50_WATCHED_ACTIONS\x10v\x12\x1d\n\x19VIDEO_P75_WATCHED_ACTIONS\x10w\x12\x1d\n\x19VIDEO_P95_WATCHED_ACTIONS\x10x\x12\x16\n\x12VIDEO_PLAY_ACTIONS\x10y\x12\x1c\n\x18VIDEO_PLAY_CURVE_ACTIONS\x10z\x12)\n%VIDEO_PLAY_RETENTION_0_TO_15S_ACTIONS\x10{\x12*\n&VIDEO_PLAY_RETENTION_20_TO_60S_ACTIONS\x10|\x12&\n\"VIDEO_PLAY_RETENTION_GRAPH_ACTIONS\x10}\x12\"\n\x1eVIDEO_THRUPLAY_WATCHED_ACTIONS\x10~\x12\x1e\n\x1aVIDEO_TIME_WATCHED_ACTIONS\x10\x7f\x12\x10\n\x0bWEBSITE_CTR\x10\x80\x01\x12\x1a\n\x15WEBSITE_PURCHASE_ROAS\x10\x82\x01\x12\r\n\x08WISH_BID\x10\x83\x01\"\x98\x04\n\tBreakdown\x12\x19\n\x15\x42REAKDOWN_UNSPECIFIED\x10\x00\x12\x13\n\x0f\x41\x44_FORMAT_ASSET\x10\x01\x12\x07\n\x03\x41GE\x10\x02\x12\n\n\x06\x41PP_ID\x10\x03\x12\x0e\n\nBODY_ASSET\x10\x04\x12\x18\n\x14\x43\x41LL_TO_ACTION_ASSET\x10\x05\x12\x0b\n\x07\x43OUNTRY\x10\x06\x12\x15\n\x11\x44\x45SCRIPTION_ASSET\x10\x07\x12\x13\n\x0f\x44\x45VICE_PLATFORM\x10\x08\x12\x07\n\x03\x44MA\x10\t\x12\x13\n\x0f\x46REQUENCY_VALUE\x10\n\x12\n\n\x06GENDER\x10\x0b\x12\x33\n/HOURLY_STATS_AGGREGATED_BY_ADVERTISER_TIME_ZONE\x10\x0c\x12\x31\n-HOURLY_STATS_AGGREGATED_BY_AUDIENCE_TIME_ZONE\x10\r\x12\x0f\n\x0bIMAGE_ASSET\x10\x0e\x12\x15\n\x11IMPRESSION_DEVICE\x10\x0f\x12\x12\n\x0eLINK_URL_ASSET\x10\x10\x12\x11\n\rPLACE_PAGE_ID\x10\x11\x12\x15\n\x11PLATFORM_POSITION\x10\x12\x12\x0e\n\nPRODUCT_ID\x10\x13\x12\x16\n\x12PUBLISHER_PLATFORM\x10\x14\x12\n\n\x06REGION\x10\x15\x12\x16\n\x12SKAN_CONVERSION_ID\x10\x16\x12\x0f\n\x0bTITLE_ASSET\x10\x17\x12\x0e\n\nVIDEO_ASSE\x10\x18\"\xa7\x02\n\x0f\x41\x63tionBreakdown\x12 \n\x1c\x41\x43TION_BREAKDOWN_UNSPECIFIED\x10\x00\x12 \n\x1c\x41\x43TION_CANVAS_COMPONENT_NAME\x10\x01\x12\x1b\n\x17\x41\x43TION_CAROUSEL_CARD_ID\x10\x02\x12\x1d\n\x19\x41\x43TION_CAROUSEL_CARD_NAME\x10\x03\x12\x16\n\x12\x41\x43TION_DESTINATION\x10\x04\x12\x11\n\rACTION_DEVICE\x10\x05\x12\x13\n\x0f\x41\x43TION_REACTION\x10\x06\x12\x14\n\x10\x41\x43TION_TARGET_ID\x10\x07\x12\x0f\n\x0b\x41\x43TION_TYPE\x10\x08\x12\x16\n\x12\x41\x43TION_VIDEO_SOUND\x10\t\x12\x15\n\x11\x41\x43TION_VIDEO_TYPE\x10\nB^Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.airbyte.facebook_marketing_source_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
+  DESCRIPTOR._serialized_options = b'Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
   _globals['_FACEBOOKMARKETINGSOURCE']._serialized_start=119
   _globals['_FACEBOOKMARKETINGSOURCE']._serialized_end=5140
   _globals['_FACEBOOKMARKETINGSOURCE_INSIGHTCONFIG']._serialized_start=488
   _globals['_FACEBOOKMARKETINGSOURCE_INSIGHTCONFIG']._serialized_end=857
   _globals['_FACEBOOKMARKETINGSOURCE_FIELD']._serialized_start=860
   _globals['_FACEBOOKMARKETINGSOURCE_FIELD']._serialized_end=4303
   _globals['_FACEBOOKMARKETINGSOURCE_BREAKDOWN']._serialized_start=4306
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/airbyte/google_ads_source.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n@doublecloud/transfer/v1/endpoint/airbyte/google_ads_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xc3\x04\n\x0fGoogleAdsSource\x12\x1f\n\x0b\x63ustomer_id\x18\x01 \x01(\tR\ncustomerId\x12\x1d\n\nstart_date\x18\x02 \x01(\tR\tstartDate\x12\x19\n\x08\x65nd_date\x18\x03 \x01(\tR\x07\x65ndDate\x12l\n\x0e\x63ustom_queries\x18\x04 \x03(\x0b\x32\x45.doublecloud.transfer.v1.endpoint.airbyte.GoogleAdsSource.CustomQueryR\rcustomQueries\x12*\n\x11login_customer_id\x18\x05 \x01(\tR\x0floginCustomerId\x12\x34\n\x16\x63onversion_window_days\x18\x06 \x01(\x01R\x14\x63onversionWindowDays\x1a\x42\n\x0b\x43ustomQuery\x12\x14\n\x05query\x18\x01 \x01(\tR\x05query\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x1a\xc0\x01\n\x0b\x43redentials\x12\'\n\x0f\x64\x65veloper_token\x18\x01 \x01(\tR\x0e\x64\x65veloperToken\x12\x1b\n\tclient_id\x18\x02 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x03 \x01(\tR\x0c\x63lientSecret\x12!\n\x0c\x61\x63\x63\x65ss_token\x18\x04 \x01(\tR\x0b\x61\x63\x63\x65ssToken\x12#\n\rrefresh_token\x18\x05 \x01(\tR\x0crefreshTokenBVZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n@doublecloud/transfer/v1/endpoint/airbyte/google_ads_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xc3\x04\n\x0fGoogleAdsSource\x12\x1f\n\x0b\x63ustomer_id\x18\x01 \x01(\tR\ncustomerId\x12\x1d\n\nstart_date\x18\x02 \x01(\tR\tstartDate\x12\x19\n\x08\x65nd_date\x18\x03 \x01(\tR\x07\x65ndDate\x12l\n\x0e\x63ustom_queries\x18\x04 \x03(\x0b\x32\x45.doublecloud.transfer.v1.endpoint.airbyte.GoogleAdsSource.CustomQueryR\rcustomQueries\x12*\n\x11login_customer_id\x18\x05 \x01(\tR\x0floginCustomerId\x12\x34\n\x16\x63onversion_window_days\x18\x06 \x01(\x01R\x14\x63onversionWindowDays\x1a\x42\n\x0b\x43ustomQuery\x12\x14\n\x05query\x18\x01 \x01(\tR\x05query\x12\x1d\n\ntable_name\x18\x02 \x01(\tR\ttableName\x1a\xc0\x01\n\x0b\x43redentials\x12\'\n\x0f\x64\x65veloper_token\x18\x01 \x01(\tR\x0e\x64\x65veloperToken\x12\x1b\n\tclient_id\x18\x02 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x03 \x01(\tR\x0c\x63lientSecret\x12!\n\x0c\x61\x63\x63\x65ss_token\x18\x04 \x01(\tR\x0b\x61\x63\x63\x65ssToken\x12#\n\rrefresh_token\x18\x05 \x01(\tR\x0crefreshTokenB^Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.airbyte.google_ads_source_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
+  DESCRIPTOR._serialized_options = b'Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
   _globals['_GOOGLEADSSOURCE']._serialized_start=111
   _globals['_GOOGLEADSSOURCE']._serialized_end=690
   _globals['_GOOGLEADSSOURCE_CUSTOMQUERY']._serialized_start=429
   _globals['_GOOGLEADSSOURCE_CUSTOMQUERY']._serialized_end=495
   _globals['_GOOGLEADSSOURCE_CREDENTIALS']._serialized_start=498
   _globals['_GOOGLEADSSOURCE_CREDENTIALS']._serialized_end=690
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/google_ads_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/instagram_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nBdoublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xd9\x03\n\x11LinkedinAdsSource\x12\x1d\n\nstart_date\x18\x01 \x01(\tR\tstartDate\x12\x1f\n\x0b\x61\x63\x63ount_ids\x18\x02 \x03(\x03R\naccountIds\x12i\n\x0b\x63redentials\x18\x03 \x01(\x0b\x32G.doublecloud.transfer.v1.endpoint.airbyte.LinkedinAdsSource.CredentialsR\x0b\x63redentials\x1a\x98\x02\n\x0b\x43redentials\x12\x65\n\x05oauth\x18\x01 \x01(\x0b\x32M.doublecloud.transfer.v1.endpoint.airbyte.LinkedinAdsSource.Credentials.OAuthH\x00R\x05oauth\x12#\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\tH\x00R\x0b\x61\x63\x63\x65ssToken\x1an\n\x05OAuth\x12\x1b\n\tclient_id\x18\x01 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x02 \x01(\tR\x0c\x63lientSecret\x12#\n\rrefresh_token\x18\x03 \x01(\tR\x0crefreshTokenB\r\n\x0b\x63redentialsBVZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nBdoublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xd9\x03\n\x11LinkedinAdsSource\x12\x1d\n\nstart_date\x18\x01 \x01(\tR\tstartDate\x12\x1f\n\x0b\x61\x63\x63ount_ids\x18\x02 \x03(\x03R\naccountIds\x12i\n\x0b\x63redentials\x18\x03 \x01(\x0b\x32G.doublecloud.transfer.v1.endpoint.airbyte.LinkedinAdsSource.CredentialsR\x0b\x63redentials\x1a\x98\x02\n\x0b\x43redentials\x12\x65\n\x05oauth\x18\x01 \x01(\x0b\x32M.doublecloud.transfer.v1.endpoint.airbyte.LinkedinAdsSource.Credentials.OAuthH\x00R\x05oauth\x12#\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\tH\x00R\x0b\x61\x63\x63\x65ssToken\x1an\n\x05OAuth\x12\x1b\n\tclient_id\x18\x01 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x02 \x01(\tR\x0c\x63lientSecret\x12#\n\rrefresh_token\x18\x03 \x01(\tR\x0crefreshTokenB\r\n\x0b\x63redentialsB^Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.airbyte.linkedin_ads_source_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
+  DESCRIPTOR._serialized_options = b'Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
   _globals['_LINKEDINADSSOURCE']._serialized_start=113
   _globals['_LINKEDINADSSOURCE']._serialized_end=586
   _globals['_LINKEDINADSSOURCE_CREDENTIALS']._serialized_start=306
   _globals['_LINKEDINADSSOURCE_CREDENTIALS']._serialized_end=586
   _globals['_LINKEDINADSSOURCE_CREDENTIALS_OAUTH']._serialized_start=461
   _globals['_LINKEDINADSSOURCE_CREDENTIALS_OAUTH']._serialized_end=571
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/airbyte/mssql_source.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;doublecloud/transfer/v1/endpoint/airbyte/mssql_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xf1\x07\n\x0bMSSQLSource\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04port\x18\x02 \x01(\x03R\x04port\x12\x1a\n\x08\x64\x61tabase\x18\x03 \x01(\tR\x08\x64\x61tabase\x12\x1a\n\x08username\x18\x04 \x01(\tR\x08username\x12\x1a\n\x08password\x18\x05 \x01(\tR\x08password\x12{\n\x12replication_method\x18\x06 \x01(\x0e\x32L.doublecloud.transfer.v1.endpoint.airbyte.MSSQLSource.MSSQLReplicationMethodR\x11replicationMethod\x12^\n\nssl_method\x18\x07 \x01(\x0b\x32?.doublecloud.transfer.v1.endpoint.airbyte.MSSQLSource.SSLConfigR\tsslMethod\x1a\x10\n\x0eSSLUnencrypted\x1a\x15\n\x13SSLEncryptedTrusted\x1aQ\n\x16SSLEncryptedVerifyCert\x12\x37\n\x18host_name_in_certificate\x18\x01 \x01(\tR\x15hostNameInCertificate\x1a\xb1\x03\n\tSSLConfig\x12h\n\x0bunencrypted\x18\x01 \x01(\x0b\x32\x44.doublecloud.transfer.v1.endpoint.airbyte.MSSQLSource.SSLUnencryptedH\x00R\x0bunencrypted\x12\x98\x01\n\"encrypted_trust_server_certificate\x18\x02 \x01(\x0b\x32I.doublecloud.transfer.v1.endpoint.airbyte.MSSQLSource.SSLEncryptedTrustedH\x00R\x1f\x65ncryptedTrustServerCertificate\x12\x90\x01\n\x1c\x65ncrypted_verify_certificate\x18\x03 \x01(\x0b\x32L.doublecloud.transfer.v1.endpoint.airbyte.MSSQLSource.SSLEncryptedVerifyCertH\x00R\x1a\x65ncryptedVerifyCertificateB\x0c\n\nssl_method\"Y\n\x16MSSQLReplicationMethod\x12(\n$MSSQL_REPLICATION_METHOD_UNSPECIFIED\x10\x00\x12\x0c\n\x08STANDARD\x10\x01\x12\x07\n\x03\x43\x44\x43\x10\x02\x42VZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;doublecloud/transfer/v1/endpoint/airbyte/mssql_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xf1\x07\n\x0bMSSQLSource\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04port\x18\x02 \x01(\x03R\x04port\x12\x1a\n\x08\x64\x61tabase\x18\x03 \x01(\tR\x08\x64\x61tabase\x12\x1a\n\x08username\x18\x04 \x01(\tR\x08username\x12\x1a\n\x08password\x18\x05 \x01(\tR\x08password\x12{\n\x12replication_method\x18\x06 \x01(\x0e\x32L.doublecloud.transfer.v1.endpoint.airbyte.MSSQLSource.MSSQLReplicationMethodR\x11replicationMethod\x12^\n\nssl_method\x18\x07 \x01(\x0b\x32?.doublecloud.transfer.v1.endpoint.airbyte.MSSQLSource.SSLConfigR\tsslMethod\x1a\x10\n\x0eSSLUnencrypted\x1a\x15\n\x13SSLEncryptedTrusted\x1aQ\n\x16SSLEncryptedVerifyCert\x12\x37\n\x18host_name_in_certificate\x18\x01 \x01(\tR\x15hostNameInCertificate\x1a\xb1\x03\n\tSSLConfig\x12h\n\x0bunencrypted\x18\x01 \x01(\x0b\x32\x44.doublecloud.transfer.v1.endpoint.airbyte.MSSQLSource.SSLUnencryptedH\x00R\x0bunencrypted\x12\x98\x01\n\"encrypted_trust_server_certificate\x18\x02 \x01(\x0b\x32I.doublecloud.transfer.v1.endpoint.airbyte.MSSQLSource.SSLEncryptedTrustedH\x00R\x1f\x65ncryptedTrustServerCertificate\x12\x90\x01\n\x1c\x65ncrypted_verify_certificate\x18\x03 \x01(\x0b\x32L.doublecloud.transfer.v1.endpoint.airbyte.MSSQLSource.SSLEncryptedVerifyCertH\x00R\x1a\x65ncryptedVerifyCertificateB\x0c\n\nssl_method\"Y\n\x16MSSQLReplicationMethod\x12(\n$MSSQL_REPLICATION_METHOD_UNSPECIFIED\x10\x00\x12\x0c\n\x08STANDARD\x10\x01\x12\x07\n\x03\x43\x44\x43\x10\x02\x42^Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.airbyte.mssql_source_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
+  DESCRIPTOR._serialized_options = b'Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
   _globals['_MSSQLSOURCE']._serialized_start=106
   _globals['_MSSQLSOURCE']._serialized_end=1115
   _globals['_MSSQLSOURCE_SSLUNENCRYPTED']._serialized_start=466
   _globals['_MSSQLSOURCE_SSLUNENCRYPTED']._serialized_end=482
   _globals['_MSSQLSOURCE_SSLENCRYPTEDTRUSTED']._serialized_start=484
   _globals['_MSSQLSOURCE_SSLENCRYPTEDTRUSTED']._serialized_end=505
   _globals['_MSSQLSOURCE_SSLENCRYPTEDVERIFYCERT']._serialized_start=507
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/airbyte/redshift_source.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n>doublecloud/transfer/v1/endpoint/airbyte/redshift_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xa6\x01\n\x0eRedshiftSource\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04port\x18\x02 \x01(\x03R\x04port\x12\x1a\n\x08\x64\x61tabase\x18\x03 \x01(\tR\x08\x64\x61tabase\x12\x18\n\x07schemas\x18\x04 \x03(\tR\x07schemas\x12\x1a\n\x08username\x18\x05 \x01(\tR\x08username\x12\x1a\n\x08password\x18\x06 \x01(\tR\x08passwordBVZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n>doublecloud/transfer/v1/endpoint/airbyte/redshift_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xa6\x01\n\x0eRedshiftSource\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04port\x18\x02 \x01(\x03R\x04port\x12\x1a\n\x08\x64\x61tabase\x18\x03 \x01(\tR\x08\x64\x61tabase\x12\x18\n\x07schemas\x18\x04 \x03(\tR\x07schemas\x12\x1a\n\x08username\x18\x05 \x01(\tR\x08username\x12\x1a\n\x08password\x18\x06 \x01(\tR\x08passwordB^Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.airbyte.redshift_source_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
+  DESCRIPTOR._serialized_options = b'Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
   _globals['_REDSHIFTSOURCE']._serialized_start=109
   _globals['_REDSHIFTSOURCE']._serialized_end=275
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/airbyte/s3_source.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8doublecloud/transfer/v1/endpoint/airbyte/s3_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xc9\r\n\x08S3Source\x12\x18\n\x07\x64\x61taset\x18\x01 \x01(\tR\x07\x64\x61taset\x12!\n\x0cpath_pattern\x18\x02 \x01(\tR\x0bpathPattern\x12\x16\n\x06schema\x18\x03 \x01(\tR\x06schema\x12Q\n\x06\x66ormat\x18\x05 \x01(\x0b\x32\x39.doublecloud.transfer.v1.endpoint.airbyte.S3Source.FormatR\x06\x66ormat\x12W\n\x08provider\x18\x06 \x01(\x0b\x32;.doublecloud.transfer.v1.endpoint.airbyte.S3Source.ProviderR\x08provider\x1a\xd7\x02\n\x06\x46ormat\x12J\n\x03\x63sv\x18\x04 \x01(\x0b\x32\x36.doublecloud.transfer.v1.endpoint.airbyte.S3Source.CsvH\x00R\x03\x63sv\x12V\n\x07parquet\x18\x05 \x01(\x0b\x32:.doublecloud.transfer.v1.endpoint.airbyte.S3Source.ParquetH\x00R\x07parquet\x12M\n\x04\x61vro\x18\x06 \x01(\x0b\x32\x37.doublecloud.transfer.v1.endpoint.airbyte.S3Source.AvroH\x00R\x04\x61vro\x12P\n\x05jsonl\x18\x07 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.airbyte.S3Source.JsonlH\x00R\x05jsonlB\x08\n\x06\x66ormat\x1a\xfe\x01\n\x08Provider\x12\x16\n\x06\x62ucket\x18\x01 \x01(\tR\x06\x62ucket\x12)\n\x11\x61ws_access_key_id\x18\x02 \x01(\tR\x0e\x61wsAccessKeyId\x12\x31\n\x15\x61ws_secret_access_key\x18\x03 \x01(\tR\x12\x61wsSecretAccessKey\x12\x1f\n\x0bpath_prefix\x18\x04 \x01(\tR\npathPrefix\x12\x1a\n\x08\x65ndpoint\x18\x05 \x01(\tR\x08\x65ndpoint\x12\x17\n\x07use_ssl\x18\x06 \x01(\x08R\x06useSsl\x12&\n\x0fverify_ssl_cert\x18\x07 \x01(\x08R\rverifySslCert\x1a\xd6\x02\n\x03\x43sv\x12\x1c\n\tdelimiter\x18\x02 \x01(\tR\tdelimiter\x12\x1d\n\nquote_char\x18\x03 \x01(\tR\tquoteChar\x12\x1f\n\x0b\x65scape_char\x18\x04 \x01(\tR\nescapeChar\x12\x1a\n\x08\x65ncoding\x18\x05 \x01(\tR\x08\x65ncoding\x12!\n\x0c\x64ouble_quote\x18\x06 \x01(\x08R\x0b\x64oubleQuote\x12,\n\x12newlines_in_values\x18\x07 \x01(\x08R\x10newlinesInValues\x12\x1d\n\nblock_size\x18\x08 \x01(\x03R\tblockSize\x12:\n\x19\x61\x64\x64itional_reader_options\x18\t \x01(\tR\x17\x61\x64\x64itionalReaderOptions\x12)\n\x10\x61\x64vanced_options\x18\n \x01(\tR\x0f\x61\x64vancedOptions\x1a\x06\n\x04\x41vro\x1a\x9a\x03\n\x05Jsonl\x12,\n\x12newlines_in_values\x18\x02 \x01(\x08R\x10newlinesInValues\x12\x8c\x01\n\x19unexpected_field_behavior\x18\x03 \x01(\x0e\x32P.doublecloud.transfer.v1.endpoint.airbyte.S3Source.Jsonl.UnexpectedFieldBehaviorR\x17unexpectedFieldBehavior\x12\x1d\n\nblock_size\x18\x04 \x01(\x03R\tblockSize\"\xb4\x01\n\x17UnexpectedFieldBehavior\x12)\n%UNEXPECTED_FIELD_BEHAVIOR_UNSPECIFIED\x10\x00\x12$\n UNEXPECTED_FIELD_BEHAVIOR_IGNORE\x10\x01\x12#\n\x1fUNEXPECTED_FIELD_BEHAVIOR_INFER\x10\x02\x12#\n\x1fUNEXPECTED_FIELD_BEHAVIOR_ERROR\x10\x03\x1a\x63\n\x07Parquet\x12\x1f\n\x0b\x62uffer_size\x18\x02 \x01(\x03R\nbufferSize\x12\x18\n\x07\x63olumns\x18\x03 \x03(\tR\x07\x63olumns\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSizeBVZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8doublecloud/transfer/v1/endpoint/airbyte/s3_source.proto\x12(doublecloud.transfer.v1.endpoint.airbyte\"\xc9\r\n\x08S3Source\x12\x18\n\x07\x64\x61taset\x18\x01 \x01(\tR\x07\x64\x61taset\x12!\n\x0cpath_pattern\x18\x02 \x01(\tR\x0bpathPattern\x12\x16\n\x06schema\x18\x03 \x01(\tR\x06schema\x12Q\n\x06\x66ormat\x18\x05 \x01(\x0b\x32\x39.doublecloud.transfer.v1.endpoint.airbyte.S3Source.FormatR\x06\x66ormat\x12W\n\x08provider\x18\x06 \x01(\x0b\x32;.doublecloud.transfer.v1.endpoint.airbyte.S3Source.ProviderR\x08provider\x1a\xd7\x02\n\x06\x46ormat\x12J\n\x03\x63sv\x18\x04 \x01(\x0b\x32\x36.doublecloud.transfer.v1.endpoint.airbyte.S3Source.CsvH\x00R\x03\x63sv\x12V\n\x07parquet\x18\x05 \x01(\x0b\x32:.doublecloud.transfer.v1.endpoint.airbyte.S3Source.ParquetH\x00R\x07parquet\x12M\n\x04\x61vro\x18\x06 \x01(\x0b\x32\x37.doublecloud.transfer.v1.endpoint.airbyte.S3Source.AvroH\x00R\x04\x61vro\x12P\n\x05jsonl\x18\x07 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.airbyte.S3Source.JsonlH\x00R\x05jsonlB\x08\n\x06\x66ormat\x1a\xfe\x01\n\x08Provider\x12\x16\n\x06\x62ucket\x18\x01 \x01(\tR\x06\x62ucket\x12)\n\x11\x61ws_access_key_id\x18\x02 \x01(\tR\x0e\x61wsAccessKeyId\x12\x31\n\x15\x61ws_secret_access_key\x18\x03 \x01(\tR\x12\x61wsSecretAccessKey\x12\x1f\n\x0bpath_prefix\x18\x04 \x01(\tR\npathPrefix\x12\x1a\n\x08\x65ndpoint\x18\x05 \x01(\tR\x08\x65ndpoint\x12\x17\n\x07use_ssl\x18\x06 \x01(\x08R\x06useSsl\x12&\n\x0fverify_ssl_cert\x18\x07 \x01(\x08R\rverifySslCert\x1a\xd6\x02\n\x03\x43sv\x12\x1c\n\tdelimiter\x18\x02 \x01(\tR\tdelimiter\x12\x1d\n\nquote_char\x18\x03 \x01(\tR\tquoteChar\x12\x1f\n\x0b\x65scape_char\x18\x04 \x01(\tR\nescapeChar\x12\x1a\n\x08\x65ncoding\x18\x05 \x01(\tR\x08\x65ncoding\x12!\n\x0c\x64ouble_quote\x18\x06 \x01(\x08R\x0b\x64oubleQuote\x12,\n\x12newlines_in_values\x18\x07 \x01(\x08R\x10newlinesInValues\x12\x1d\n\nblock_size\x18\x08 \x01(\x03R\tblockSize\x12:\n\x19\x61\x64\x64itional_reader_options\x18\t \x01(\tR\x17\x61\x64\x64itionalReaderOptions\x12)\n\x10\x61\x64vanced_options\x18\n \x01(\tR\x0f\x61\x64vancedOptions\x1a\x06\n\x04\x41vro\x1a\x9a\x03\n\x05Jsonl\x12,\n\x12newlines_in_values\x18\x02 \x01(\x08R\x10newlinesInValues\x12\x8c\x01\n\x19unexpected_field_behavior\x18\x03 \x01(\x0e\x32P.doublecloud.transfer.v1.endpoint.airbyte.S3Source.Jsonl.UnexpectedFieldBehaviorR\x17unexpectedFieldBehavior\x12\x1d\n\nblock_size\x18\x04 \x01(\x03R\tblockSize\"\xb4\x01\n\x17UnexpectedFieldBehavior\x12)\n%UNEXPECTED_FIELD_BEHAVIOR_UNSPECIFIED\x10\x00\x12$\n UNEXPECTED_FIELD_BEHAVIOR_IGNORE\x10\x01\x12#\n\x1fUNEXPECTED_FIELD_BEHAVIOR_INFER\x10\x02\x12#\n\x1fUNEXPECTED_FIELD_BEHAVIOR_ERROR\x10\x03\x1a\x63\n\x07Parquet\x12\x1f\n\x0b\x62uffer_size\x18\x02 \x01(\x03R\nbufferSize\x12\x18\n\x07\x63olumns\x18\x03 \x03(\tR\x07\x63olumns\x12\x1d\n\nbatch_size\x18\x04 \x01(\x03R\tbatchSizeB^Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyteb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.airbyte.s3_source_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZTgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
+  DESCRIPTOR._serialized_options = b'Z\\github.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint/airbyte;endpoint_airbyte'
   _globals['_S3SOURCE']._serialized_start=103
   _globals['_S3SOURCE']._serialized_end=1840
   _globals['_S3SOURCE_FORMAT']._serialized_start=373
   _globals['_S3SOURCE_FORMAT']._serialized_end=716
   _globals['_S3SOURCE_PROVIDER']._serialized_start=719
   _globals['_S3SOURCE_PROVIDER']._serialized_end=973
   _globals['_S3SOURCE_CSV']._serialized_start=976
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/clickhouse.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from doublecloud.transfer.v1.endpoint import common_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n1doublecloud/transfer/v1/endpoint/clickhouse.proto\x12 doublecloud.transfer.v1.endpoint\x1a\x1bgoogle/protobuf/empty.proto\x1a-doublecloud/transfer/v1/endpoint/common.proto\";\n\x0f\x43lickhouseShard\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x14\n\x05hosts\x18\x02 \x03(\tR\x05hosts\"\xe4\x01\n\x13OnPremiseClickhouse\x12I\n\x06shards\x18\x01 \x03(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.ClickhouseShardR\x06shards\x12\x1b\n\thttp_port\x18\x03 \x01(\x03R\x08httpPort\x12\x1f\n\x0bnative_port\x18\x04 \x01(\x03R\nnativePort\x12\x44\n\x08tls_mode\x18\x08 \x01(\x0b\x32).doublecloud.transfer.v1.endpoint.TLSModeR\x07tlsMode\"\x9e\x02\n\x1b\x43lickhouseConnectionOptions\x12&\n\x0emdb_cluster_id\x18\x05 \x01(\tH\x00R\x0cmdbClusterId\x12V\n\non_premise\x18\x02 \x01(\x0b\x32\x35.doublecloud.transfer.v1.endpoint.OnPremiseClickhouseH\x00R\tonPremise\x12\x1a\n\x08\x64\x61tabase\x18\x08 \x01(\tR\x08\x64\x61tabase\x12\x12\n\x04user\x18\x06 \x01(\tR\x04user\x12\x44\n\x08password\x18\x07 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08passwordB\t\n\x07\x61\x64\x64ress\"\x94\x01\n\x14\x43lickhouseConnection\x12n\n\x12\x63onnection_options\x18\x01 \x01(\x0b\x32=.doublecloud.transfer.v1.endpoint.ClickhouseConnectionOptionsH\x00R\x11\x63onnectionOptionsB\x0c\n\nconnection\"\x9e\x05\n\x12\x43lickhouseSharding\x12r\n\x11\x63olumn_value_hash\x18\x01 \x01(\x0b\x32\x44.doublecloud.transfer.v1.endpoint.ClickhouseSharding.ColumnValueHashH\x00R\x0f\x63olumnValueHash\x12p\n\x0e\x63ustom_mapping\x18\x02 \x01(\x0b\x32G.doublecloud.transfer.v1.endpoint.ClickhouseSharding.ColumnValueMappingH\x00R\rcustomMapping\x12\x39\n\x0btransfer_id\x18\x03 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00R\ntransferId\x1a\x32\n\x0f\x43olumnValueHash\x12\x1f\n\x0b\x63olumn_name\x18\x01 \x01(\tR\ncolumnName\x1a\xa6\x02\n\x12\x43olumnValueMapping\x12\x1f\n\x0b\x63olumn_name\x18\x01 \x01(\tR\ncolumnName\x12n\n\x07mapping\x18\x02 \x03(\x0b\x32T.doublecloud.transfer.v1.endpoint.ClickhouseSharding.ColumnValueMapping.ValueToShardR\x07mapping\x1a\x7f\n\x0cValueToShard\x12P\n\x0c\x63olumn_value\x18\x01 \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.ColumnValueR\x0b\x63olumnValue\x12\x1d\n\nshard_name\x18\x02 \x01(\tR\tshardNameB\n\n\x08sharding\"\xb8\x01\n\x10\x43lickhouseSource\x12V\n\nconnection\x18\x01 \x01(\x0b\x32\x36.doublecloud.transfer.v1.endpoint.ClickhouseConnectionR\nconnection\x12%\n\x0einclude_tables\x18\x07 \x03(\tR\rincludeTables\x12%\n\x0e\x65xclude_tables\x18\x08 \x03(\tR\rexcludeTables\"\x9e\x03\n\x10\x43lickhouseTarget\x12V\n\nconnection\x18\x02 \x01(\x0b\x32\x36.doublecloud.transfer.v1.endpoint.ClickhouseConnectionR\nconnection\x12\x36\n\x17\x63lickhouse_cluster_name\x18\x32 \x01(\tR\x15\x63lickhouseClusterName\x12\x46\n\talt_names\x18\x11 \x03(\x0b\x32).doublecloud.transfer.v1.endpoint.AltNameR\x08\x61ltNames\x12P\n\x08sharding\x18\x16 \x01(\x0b\x32\x34.doublecloud.transfer.v1.endpoint.ClickhouseShardingR\x08sharding\x12`\n\x0e\x63leanup_policy\x18\x15 \x01(\x0e\x32\x39.doublecloud.transfer.v1.endpoint.ClickhouseCleanupPolicyR\rcleanupPolicy*\xb8\x01\n\x17\x43lickhouseCleanupPolicy\x12)\n%CLICKHOUSE_CLEANUP_POLICY_UNSPECIFIED\x10\x00\x12&\n\"CLICKHOUSE_CLEANUP_POLICY_DISABLED\x10\x01\x12\"\n\x1e\x43LICKHOUSE_CLEANUP_POLICY_DROP\x10\x02\x12&\n\"CLICKHOUSE_CLEANUP_POLICY_TRUNCATE\x10\x03\x42\x46ZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n1doublecloud/transfer/v1/endpoint/clickhouse.proto\x12 doublecloud.transfer.v1.endpoint\x1a\x1bgoogle/protobuf/empty.proto\x1a-doublecloud/transfer/v1/endpoint/common.proto\";\n\x0f\x43lickhouseShard\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x14\n\x05hosts\x18\x02 \x03(\tR\x05hosts\"\xe4\x01\n\x13OnPremiseClickhouse\x12I\n\x06shards\x18\x01 \x03(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.ClickhouseShardR\x06shards\x12\x1b\n\thttp_port\x18\x03 \x01(\x03R\x08httpPort\x12\x1f\n\x0bnative_port\x18\x04 \x01(\x03R\nnativePort\x12\x44\n\x08tls_mode\x18\x08 \x01(\x0b\x32).doublecloud.transfer.v1.endpoint.TLSModeR\x07tlsMode\"\x9e\x02\n\x1b\x43lickhouseConnectionOptions\x12&\n\x0emdb_cluster_id\x18\x05 \x01(\tH\x00R\x0cmdbClusterId\x12V\n\non_premise\x18\x02 \x01(\x0b\x32\x35.doublecloud.transfer.v1.endpoint.OnPremiseClickhouseH\x00R\tonPremise\x12\x1a\n\x08\x64\x61tabase\x18\x08 \x01(\tR\x08\x64\x61tabase\x12\x12\n\x04user\x18\x06 \x01(\tR\x04user\x12\x44\n\x08password\x18\x07 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08passwordB\t\n\x07\x61\x64\x64ress\"\x94\x01\n\x14\x43lickhouseConnection\x12n\n\x12\x63onnection_options\x18\x01 \x01(\x0b\x32=.doublecloud.transfer.v1.endpoint.ClickhouseConnectionOptionsH\x00R\x11\x63onnectionOptionsB\x0c\n\nconnection\"\x9e\x05\n\x12\x43lickhouseSharding\x12r\n\x11\x63olumn_value_hash\x18\x01 \x01(\x0b\x32\x44.doublecloud.transfer.v1.endpoint.ClickhouseSharding.ColumnValueHashH\x00R\x0f\x63olumnValueHash\x12p\n\x0e\x63ustom_mapping\x18\x02 \x01(\x0b\x32G.doublecloud.transfer.v1.endpoint.ClickhouseSharding.ColumnValueMappingH\x00R\rcustomMapping\x12\x39\n\x0btransfer_id\x18\x03 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00R\ntransferId\x1a\x32\n\x0f\x43olumnValueHash\x12\x1f\n\x0b\x63olumn_name\x18\x01 \x01(\tR\ncolumnName\x1a\xa6\x02\n\x12\x43olumnValueMapping\x12\x1f\n\x0b\x63olumn_name\x18\x01 \x01(\tR\ncolumnName\x12n\n\x07mapping\x18\x02 \x03(\x0b\x32T.doublecloud.transfer.v1.endpoint.ClickhouseSharding.ColumnValueMapping.ValueToShardR\x07mapping\x1a\x7f\n\x0cValueToShard\x12P\n\x0c\x63olumn_value\x18\x01 \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.ColumnValueR\x0b\x63olumnValue\x12\x1d\n\nshard_name\x18\x02 \x01(\tR\tshardNameB\n\n\x08sharding\"\xb8\x01\n\x10\x43lickhouseSource\x12V\n\nconnection\x18\x01 \x01(\x0b\x32\x36.doublecloud.transfer.v1.endpoint.ClickhouseConnectionR\nconnection\x12%\n\x0einclude_tables\x18\x07 \x03(\tR\rincludeTables\x12%\n\x0e\x65xclude_tables\x18\x08 \x03(\tR\rexcludeTables\"\x9e\x03\n\x10\x43lickhouseTarget\x12V\n\nconnection\x18\x02 \x01(\x0b\x32\x36.doublecloud.transfer.v1.endpoint.ClickhouseConnectionR\nconnection\x12\x36\n\x17\x63lickhouse_cluster_name\x18\x32 \x01(\tR\x15\x63lickhouseClusterName\x12\x46\n\talt_names\x18\x11 \x03(\x0b\x32).doublecloud.transfer.v1.endpoint.AltNameR\x08\x61ltNames\x12P\n\x08sharding\x18\x16 \x01(\x0b\x32\x34.doublecloud.transfer.v1.endpoint.ClickhouseShardingR\x08sharding\x12`\n\x0e\x63leanup_policy\x18\x15 \x01(\x0e\x32\x39.doublecloud.transfer.v1.endpoint.ClickhouseCleanupPolicyR\rcleanupPolicy*\xb8\x01\n\x17\x43lickhouseCleanupPolicy\x12)\n%CLICKHOUSE_CLEANUP_POLICY_UNSPECIFIED\x10\x00\x12&\n\"CLICKHOUSE_CLEANUP_POLICY_DISABLED\x10\x01\x12\"\n\x1e\x43LICKHOUSE_CLEANUP_POLICY_DROP\x10\x02\x12&\n\"CLICKHOUSE_CLEANUP_POLICY_TRUNCATE\x10\x03\x42NZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.clickhouse_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpoint'
+  DESCRIPTOR._serialized_options = b'ZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpoint'
   _globals['_CLICKHOUSECLEANUPPOLICY']._serialized_start=2173
   _globals['_CLICKHOUSECLEANUPPOLICY']._serialized_end=2357
   _globals['_CLICKHOUSESHARD']._serialized_start=163
   _globals['_CLICKHOUSESHARD']._serialized_end=222
   _globals['_ONPREMISECLICKHOUSE']._serialized_start=225
   _globals['_ONPREMISECLICKHOUSE']._serialized_end=453
   _globals['_CLICKHOUSECONNECTIONOPTIONS']._serialized_start=456
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/common_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/common_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/common.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-doublecloud/transfer/v1/endpoint/common.proto\x12 doublecloud.transfer.v1.endpoint\x1a\x1bgoogle/protobuf/empty.proto\"?\n\x07\x41ltName\x12\x1b\n\tfrom_name\x18\x01 \x01(\tR\x08\x66romName\x12\x17\n\x07to_name\x18\x02 \x01(\tR\x06toName\"%\n\x06Secret\x12\x12\n\x03raw\x18\x01 \x01(\tH\x00R\x03rawB\x07\n\x05value\"\xa3\x01\n\tColSchema\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12@\n\x04type\x18\x02 \x01(\x0e\x32,.doublecloud.transfer.v1.endpoint.ColumnTypeR\x04type\x12\x10\n\x03key\x18\x03 \x01(\x08R\x03key\x12\x1a\n\x08required\x18\x04 \x01(\x08R\x08required\x12\x12\n\x04path\x18\x05 \x01(\tR\x04path\"\x94\x01\n\x07TLSMode\x12\x34\n\x08\x64isabled\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00R\x08\x64isabled\x12G\n\x07\x65nabled\x18\x02 \x01(\x0b\x32+.doublecloud.transfer.v1.endpoint.TLSConfigH\x00R\x07\x65nabledB\n\n\x08tls_mode\"2\n\tTLSConfig\x12%\n\x0e\x63\x61_certificate\x18\x01 \x01(\tR\rcaCertificate\";\n\x0b\x43olumnValue\x12#\n\x0cstring_value\x18\x01 \x01(\tH\x00R\x0bstringValueB\x07\n\x05value\"P\n\tFieldList\x12\x43\n\x06\x66ields\x18\x02 \x03(\x0b\x32+.doublecloud.transfer.v1.endpoint.ColSchemaR\x06\x66ields\"\x80\x01\n\nDataSchema\x12\x45\n\x06\x66ields\x18\x02 \x01(\x0b\x32+.doublecloud.transfer.v1.endpoint.FieldListH\x00R\x06\x66ields\x12!\n\x0bjson_fields\x18\x01 \x01(\tH\x00R\njsonFieldsB\x08\n\x06schema\"\x08\n\x06NoAuth*h\n\x13ObjectTransferStage\x12%\n!OBJECT_TRANSFER_STAGE_UNSPECIFIED\x10\x00\x12\x0f\n\x0b\x42\x45\x46ORE_DATA\x10\x01\x12\x0e\n\nAFTER_DATA\x10\x02\x12\t\n\x05NEVER\x10\x03*U\n\rCleanupPolicy\x12\x1e\n\x1a\x43LEANUP_POLICY_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x44ISABLED\x10\x01\x12\x08\n\x04\x44ROP\x10\x02\x12\x0c\n\x08TRUNCATE\x10\x03*\xc9\x01\n\nColumnType\x12\x1b\n\x17\x43OLUMN_TYPE_UNSPECIFIED\x10\x00\x12\t\n\x05INT64\x10\x0e\x12\t\n\x05INT32\x10\x01\x12\t\n\x05INT16\x10\x02\x12\x08\n\x04INT8\x10\x03\x12\n\n\x06UINT64\x10\x04\x12\n\n\x06UINT32\x10\x05\x12\n\n\x06UINT16\x10\x06\x12\t\n\x05UINT8\x10\x07\x12\n\n\x06\x44OUBLE\x10\x08\x12\x0b\n\x07\x42OOLEAN\x10\t\x12\n\n\x06STRING\x10\n\x12\x08\n\x04UTF8\x10\x0b\x12\x07\n\x03\x41NY\x10\x0c\x12\x0c\n\x08\x44\x41TETIME\x10\rBFZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-doublecloud/transfer/v1/endpoint/common.proto\x12 doublecloud.transfer.v1.endpoint\x1a\x1bgoogle/protobuf/empty.proto\"?\n\x07\x41ltName\x12\x1b\n\tfrom_name\x18\x01 \x01(\tR\x08\x66romName\x12\x17\n\x07to_name\x18\x02 \x01(\tR\x06toName\"%\n\x06Secret\x12\x12\n\x03raw\x18\x01 \x01(\tH\x00R\x03rawB\x07\n\x05value\"\xa3\x01\n\tColSchema\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12@\n\x04type\x18\x02 \x01(\x0e\x32,.doublecloud.transfer.v1.endpoint.ColumnTypeR\x04type\x12\x10\n\x03key\x18\x03 \x01(\x08R\x03key\x12\x1a\n\x08required\x18\x04 \x01(\x08R\x08required\x12\x12\n\x04path\x18\x05 \x01(\tR\x04path\"\x94\x01\n\x07TLSMode\x12\x34\n\x08\x64isabled\x18\x01 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00R\x08\x64isabled\x12G\n\x07\x65nabled\x18\x02 \x01(\x0b\x32+.doublecloud.transfer.v1.endpoint.TLSConfigH\x00R\x07\x65nabledB\n\n\x08tls_mode\"2\n\tTLSConfig\x12%\n\x0e\x63\x61_certificate\x18\x01 \x01(\tR\rcaCertificate\";\n\x0b\x43olumnValue\x12#\n\x0cstring_value\x18\x01 \x01(\tH\x00R\x0bstringValueB\x07\n\x05value\"P\n\tFieldList\x12\x43\n\x06\x66ields\x18\x02 \x03(\x0b\x32+.doublecloud.transfer.v1.endpoint.ColSchemaR\x06\x66ields\"\x80\x01\n\nDataSchema\x12\x45\n\x06\x66ields\x18\x02 \x01(\x0b\x32+.doublecloud.transfer.v1.endpoint.FieldListH\x00R\x06\x66ields\x12!\n\x0bjson_fields\x18\x01 \x01(\tH\x00R\njsonFieldsB\x08\n\x06schema\"\x08\n\x06NoAuth*h\n\x13ObjectTransferStage\x12%\n!OBJECT_TRANSFER_STAGE_UNSPECIFIED\x10\x00\x12\x0f\n\x0b\x42\x45\x46ORE_DATA\x10\x01\x12\x0e\n\nAFTER_DATA\x10\x02\x12\t\n\x05NEVER\x10\x03*U\n\rCleanupPolicy\x12\x1e\n\x1a\x43LEANUP_POLICY_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x44ISABLED\x10\x01\x12\x08\n\x04\x44ROP\x10\x02\x12\x0c\n\x08TRUNCATE\x10\x03*\xc9\x01\n\nColumnType\x12\x1b\n\x17\x43OLUMN_TYPE_UNSPECIFIED\x10\x00\x12\t\n\x05INT64\x10\x0e\x12\t\n\x05INT32\x10\x01\x12\t\n\x05INT16\x10\x02\x12\x08\n\x04INT8\x10\x03\x12\n\n\x06UINT64\x10\x04\x12\n\n\x06UINT32\x10\x05\x12\n\n\x06UINT16\x10\x06\x12\t\n\x05UINT8\x10\x07\x12\n\n\x06\x44OUBLE\x10\x08\x12\x0b\n\x07\x42OOLEAN\x10\t\x12\n\n\x06STRING\x10\n\x12\x08\n\x04UTF8\x10\x0b\x12\x07\n\x03\x41NY\x10\x0c\x12\x0c\n\x08\x44\x41TETIME\x10\rBNZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpoint'
+  DESCRIPTOR._serialized_options = b'ZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpoint'
   _globals['_OBJECTTRANSFERSTAGE']._serialized_start=869
   _globals['_OBJECTTRANSFERSTAGE']._serialized_end=973
   _globals['_CLEANUPPOLICY']._serialized_start=975
   _globals['_CLEANUPPOLICY']._serialized_end=1060
   _globals['_COLUMNTYPE']._serialized_start=1063
   _globals['_COLUMNTYPE']._serialized_end=1264
   _globals['_ALTNAME']._serialized_start=112
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/common_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/kafka_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/kafka.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.transfer.v1.endpoint import common_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_common__pb2
 from doublecloud.transfer.v1.endpoint import parsers_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_parsers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,doublecloud/transfer/v1/endpoint/kafka.proto\x12 doublecloud.transfer.v1.endpoint\x1a-doublecloud/transfer/v1/endpoint/common.proto\x1a.doublecloud/transfer/v1/endpoint/parsers.proto\"\x9a\x01\n\x16KafkaConnectionOptions\x12\x1f\n\ncluster_id\x18\x01 \x01(\tH\x00R\tclusterId\x12Q\n\non_premise\x18\x02 \x01(\x0b\x32\x30.doublecloud.transfer.v1.endpoint.OnPremiseKafkaH\x00R\tonPremiseB\x0c\n\nconnection\"w\n\x0eOnPremiseKafka\x12\x1f\n\x0b\x62roker_urls\x18\x01 \x03(\tR\nbrokerUrls\x12\x44\n\x08tls_mode\x18\x05 \x01(\x0b\x32).doublecloud.transfer.v1.endpoint.TLSModeR\x07tlsMode\"\xa7\x01\n\tKafkaAuth\x12I\n\x04sasl\x18\x01 \x01(\x0b\x32\x33.doublecloud.transfer.v1.endpoint.KafkaSaslSecurityH\x00R\x04sasl\x12\x43\n\x07no_auth\x18\x02 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.NoAuthH\x00R\x06noAuthB\n\n\x08security\"\xbd\x01\n\x11KafkaSaslSecurity\x12\x12\n\x04user\x18\x01 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12N\n\tmechanism\x18\x03 \x01(\x0e\x32\x30.doublecloud.transfer.v1.endpoint.KafkaMechanismR\tmechanism\"\x89\x02\n\x0bKafkaSource\x12X\n\nconnection\x18\x01 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.KafkaConnectionOptionsR\nconnection\x12?\n\x04\x61uth\x18\x02 \x01(\x0b\x32+.doublecloud.transfer.v1.endpoint.KafkaAuthR\x04\x61uth\x12\x1d\n\ntopic_name\x18\x04 \x01(\tR\ttopicName\x12@\n\x06parser\x18\x07 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.ParserR\x06parser\"\x8b\x02\n\x0bKafkaTarget\x12X\n\nconnection\x18\x01 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.KafkaConnectionOptionsR\nconnection\x12?\n\x04\x61uth\x18\x02 \x01(\x0b\x32+.doublecloud.transfer.v1.endpoint.KafkaAuthR\x04\x61uth\x12\x61\n\x0etopic_settings\x18\x07 \x01(\x0b\x32:.doublecloud.transfer.v1.endpoint.KafkaTargetTopicSettingsR\rtopicSettings\"\x9d\x01\n\x18KafkaTargetTopicSettings\x12J\n\x05topic\x18\x01 \x01(\x0b\x32\x32.doublecloud.transfer.v1.endpoint.KafkaTargetTopicH\x00R\x05topic\x12#\n\x0ctopic_prefix\x18\x02 \x01(\tH\x00R\x0btopicPrefixB\x10\n\x0etopic_settings\"U\n\x10KafkaTargetTopic\x12\x1d\n\ntopic_name\x18\x01 \x01(\tR\ttopicName\x12\"\n\rsave_tx_order\x18\x02 \x01(\x08R\x0bsaveTxOrder*i\n\x0eKafkaMechanism\x12\x1f\n\x1bKAFKA_MECHANISM_UNSPECIFIED\x10\x00\x12\x1a\n\x16KAFKA_MECHANISM_SHA256\x10\x01\x12\x1a\n\x16KAFKA_MECHANISM_SHA512\x10\x02\x42\x46ZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,doublecloud/transfer/v1/endpoint/kafka.proto\x12 doublecloud.transfer.v1.endpoint\x1a-doublecloud/transfer/v1/endpoint/common.proto\x1a.doublecloud/transfer/v1/endpoint/parsers.proto\"\x9a\x01\n\x16KafkaConnectionOptions\x12\x1f\n\ncluster_id\x18\x01 \x01(\tH\x00R\tclusterId\x12Q\n\non_premise\x18\x02 \x01(\x0b\x32\x30.doublecloud.transfer.v1.endpoint.OnPremiseKafkaH\x00R\tonPremiseB\x0c\n\nconnection\"w\n\x0eOnPremiseKafka\x12\x1f\n\x0b\x62roker_urls\x18\x01 \x03(\tR\nbrokerUrls\x12\x44\n\x08tls_mode\x18\x05 \x01(\x0b\x32).doublecloud.transfer.v1.endpoint.TLSModeR\x07tlsMode\"\xa7\x01\n\tKafkaAuth\x12I\n\x04sasl\x18\x01 \x01(\x0b\x32\x33.doublecloud.transfer.v1.endpoint.KafkaSaslSecurityH\x00R\x04sasl\x12\x43\n\x07no_auth\x18\x02 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.NoAuthH\x00R\x06noAuthB\n\n\x08security\"\xbd\x01\n\x11KafkaSaslSecurity\x12\x12\n\x04user\x18\x01 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12N\n\tmechanism\x18\x03 \x01(\x0e\x32\x30.doublecloud.transfer.v1.endpoint.KafkaMechanismR\tmechanism\"\x89\x02\n\x0bKafkaSource\x12X\n\nconnection\x18\x01 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.KafkaConnectionOptionsR\nconnection\x12?\n\x04\x61uth\x18\x02 \x01(\x0b\x32+.doublecloud.transfer.v1.endpoint.KafkaAuthR\x04\x61uth\x12\x1d\n\ntopic_name\x18\x04 \x01(\tR\ttopicName\x12@\n\x06parser\x18\x07 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.ParserR\x06parser\"\x8b\x02\n\x0bKafkaTarget\x12X\n\nconnection\x18\x01 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.KafkaConnectionOptionsR\nconnection\x12?\n\x04\x61uth\x18\x02 \x01(\x0b\x32+.doublecloud.transfer.v1.endpoint.KafkaAuthR\x04\x61uth\x12\x61\n\x0etopic_settings\x18\x07 \x01(\x0b\x32:.doublecloud.transfer.v1.endpoint.KafkaTargetTopicSettingsR\rtopicSettings\"\x9d\x01\n\x18KafkaTargetTopicSettings\x12J\n\x05topic\x18\x01 \x01(\x0b\x32\x32.doublecloud.transfer.v1.endpoint.KafkaTargetTopicH\x00R\x05topic\x12#\n\x0ctopic_prefix\x18\x02 \x01(\tH\x00R\x0btopicPrefixB\x10\n\x0etopic_settings\"U\n\x10KafkaTargetTopic\x12\x1d\n\ntopic_name\x18\x01 \x01(\tR\ttopicName\x12\"\n\rsave_tx_order\x18\x02 \x01(\x08R\x0bsaveTxOrder*i\n\x0eKafkaMechanism\x12\x1f\n\x1bKAFKA_MECHANISM_UNSPECIFIED\x10\x00\x12\x1a\n\x16KAFKA_MECHANISM_SHA256\x10\x01\x12\x1a\n\x16KAFKA_MECHANISM_SHA512\x10\x02\x42NZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.kafka_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpoint'
+  DESCRIPTOR._serialized_options = b'ZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpoint'
   _globals['_KAFKAMECHANISM']._serialized_start=1602
   _globals['_KAFKAMECHANISM']._serialized_end=1707
   _globals['_KAFKACONNECTIONOPTIONS']._serialized_start=178
   _globals['_KAFKACONNECTIONOPTIONS']._serialized_end=332
   _globals['_ONPREMISEKAFKA']._serialized_start=334
   _globals['_ONPREMISEKAFKA']._serialized_end=453
   _globals['_KAFKAAUTH']._serialized_start=456
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/kafka_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/kafka_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mongo_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/mongo.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.transfer.v1.endpoint import common_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,doublecloud/transfer/v1/endpoint/mongo.proto\x12 doublecloud.transfer.v1.endpoint\x1a-doublecloud/transfer/v1/endpoint/common.proto\"\xa1\x01\n\x0eOnPremiseMongo\x12\x14\n\x05hosts\x18\x01 \x03(\tR\x05hosts\x12\x12\n\x04port\x18\x02 \x01(\x03R\x04port\x12\x44\n\x08tls_mode\x18\x06 \x01(\x0b\x32).doublecloud.transfer.v1.endpoint.TLSModeR\x07tlsMode\x12\x1f\n\x0breplica_set\x18\x05 \x01(\tR\nreplicaSet\"\xf1\x01\n\x16MongoConnectionOptions\x12Q\n\non_premise\x18\x02 \x01(\x0b\x32\x30.doublecloud.transfer.v1.endpoint.OnPremiseMongoH\x00R\tonPremise\x12\x12\n\x04user\x18\x03 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12\x1f\n\x0b\x61uth_source\x18\x05 \x01(\tR\nauthSourceB\t\n\x07\x61\x64\x64ress\"\x8a\x01\n\x0fMongoConnection\x12i\n\x12\x63onnection_options\x18\x03 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.MongoConnectionOptionsH\x00R\x11\x63onnectionOptionsB\x0c\n\nconnection\"_\n\x0fMongoCollection\x12#\n\rdatabase_name\x18\x01 \x01(\tR\x0c\x64\x61tabaseName\x12\'\n\x0f\x63ollection_name\x18\x02 \x01(\tR\x0e\x63ollectionName\"\xd5\x02\n\x0bMongoSource\x12Q\n\nconnection\x18\x01 \x01(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.MongoConnectionR\nconnection\x12S\n\x0b\x63ollections\x18\x06 \x03(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.MongoCollectionR\x0b\x63ollections\x12\x64\n\x14\x65xcluded_collections\x18\x07 \x03(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.MongoCollectionR\x13\x65xcludedCollections\x12\x38\n\x18secondary_preferred_mode\x18\x08 \x01(\x08R\x16secondaryPreferredMode\"\xd4\x01\n\x0bMongoTarget\x12Q\n\nconnection\x18\x01 \x01(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.MongoConnectionR\nconnection\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12V\n\x0e\x63leanup_policy\x18\x06 \x01(\x0e\x32/.doublecloud.transfer.v1.endpoint.CleanupPolicyR\rcleanupPolicyBFZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,doublecloud/transfer/v1/endpoint/mongo.proto\x12 doublecloud.transfer.v1.endpoint\x1a-doublecloud/transfer/v1/endpoint/common.proto\"\xa1\x01\n\x0eOnPremiseMongo\x12\x14\n\x05hosts\x18\x01 \x03(\tR\x05hosts\x12\x12\n\x04port\x18\x02 \x01(\x03R\x04port\x12\x44\n\x08tls_mode\x18\x06 \x01(\x0b\x32).doublecloud.transfer.v1.endpoint.TLSModeR\x07tlsMode\x12\x1f\n\x0breplica_set\x18\x05 \x01(\tR\nreplicaSet\"\xf1\x01\n\x16MongoConnectionOptions\x12Q\n\non_premise\x18\x02 \x01(\x0b\x32\x30.doublecloud.transfer.v1.endpoint.OnPremiseMongoH\x00R\tonPremise\x12\x12\n\x04user\x18\x03 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12\x1f\n\x0b\x61uth_source\x18\x05 \x01(\tR\nauthSourceB\t\n\x07\x61\x64\x64ress\"\x8a\x01\n\x0fMongoConnection\x12i\n\x12\x63onnection_options\x18\x03 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.MongoConnectionOptionsH\x00R\x11\x63onnectionOptionsB\x0c\n\nconnection\"_\n\x0fMongoCollection\x12#\n\rdatabase_name\x18\x01 \x01(\tR\x0c\x64\x61tabaseName\x12\'\n\x0f\x63ollection_name\x18\x02 \x01(\tR\x0e\x63ollectionName\"\xd5\x02\n\x0bMongoSource\x12Q\n\nconnection\x18\x01 \x01(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.MongoConnectionR\nconnection\x12S\n\x0b\x63ollections\x18\x06 \x03(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.MongoCollectionR\x0b\x63ollections\x12\x64\n\x14\x65xcluded_collections\x18\x07 \x03(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.MongoCollectionR\x13\x65xcludedCollections\x12\x38\n\x18secondary_preferred_mode\x18\x08 \x01(\x08R\x16secondaryPreferredMode\"\xd4\x01\n\x0bMongoTarget\x12Q\n\nconnection\x18\x01 \x01(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.MongoConnectionR\nconnection\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12V\n\x0e\x63leanup_policy\x18\x06 \x01(\x0e\x32/.doublecloud.transfer.v1.endpoint.CleanupPolicyR\rcleanupPolicyBNZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.mongo_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpoint'
+  DESCRIPTOR._serialized_options = b'ZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpoint'
   _globals['_ONPREMISEMONGO']._serialized_start=130
   _globals['_ONPREMISEMONGO']._serialized_end=291
   _globals['_MONGOCONNECTIONOPTIONS']._serialized_start=294
   _globals['_MONGOCONNECTIONOPTIONS']._serialized_end=535
   _globals['_MONGOCONNECTION']._serialized_start=538
   _globals['_MONGOCONNECTION']._serialized_end=676
   _globals['_MONGOCOLLECTION']._serialized_start=678
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/mongo_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mongo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mysql_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/mysql.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.transfer.v1.endpoint import common_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,doublecloud/transfer/v1/endpoint/mysql.proto\x12 doublecloud.transfer.v1.endpoint\x1a-doublecloud/transfer/v1/endpoint/common.proto\"\x80\x01\n\x0eOnPremiseMysql\x12\x14\n\x05hosts\x18\x05 \x03(\tR\x05hosts\x12\x12\n\x04port\x18\x02 \x01(\x03R\x04port\x12\x44\n\x08tls_mode\x18\x06 \x01(\x0b\x32).doublecloud.transfer.v1.endpoint.TLSModeR\x07tlsMode\"r\n\x0fMysqlConnection\x12Q\n\non_premise\x18\x02 \x01(\x0b\x32\x30.doublecloud.transfer.v1.endpoint.OnPremiseMysqlH\x00R\tonPremiseB\x0c\n\nconnection\"\xd9\x02\n\x1bMysqlObjectTransferSettings\x12I\n\x04view\x18\x01 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x04view\x12O\n\x07routine\x18\x02 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x07routine\x12O\n\x07trigger\x18\x03 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x07trigger\x12M\n\x06tables\x18\x04 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x06tables\"\xfa\x03\n\x0bMysqlSource\x12Q\n\nconnection\x18\x01 \x01(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.MysqlConnectionR\nconnection\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12)\n\x10service_database\x18\x0f \x01(\tR\x0fserviceDatabase\x12\x12\n\x04user\x18\x03 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12\x30\n\x14include_tables_regex\x18\x0c \x03(\tR\x12includeTablesRegex\x12\x30\n\x14\x65xclude_tables_regex\x18\r \x03(\tR\x12\x65xcludeTablesRegex\x12\x1a\n\x08timezone\x18\x08 \x01(\tR\x08timezone\x12w\n\x18object_transfer_settings\x18\x0b \x01(\x0b\x32=.doublecloud.transfer.v1.endpoint.MysqlObjectTransferSettingsR\x16objectTransferSettings\"\xef\x03\n\x0bMysqlTarget\x12Q\n\nconnection\x18\x01 \x01(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.MysqlConnectionR\nconnection\x12\'\n\x0fsecurity_groups\x18\x10 \x03(\tR\x0esecurityGroups\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12\x12\n\x04user\x18\x03 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12\x19\n\x08sql_mode\x18\x05 \x01(\tR\x07sqlMode\x12\x34\n\x16skip_constraint_checks\x18\x06 \x01(\x08R\x14skipConstraintChecks\x12\x1a\n\x08timezone\x18\x07 \x01(\tR\x08timezone\x12V\n\x0e\x63leanup_policy\x18\x08 \x01(\x0e\x32/.doublecloud.transfer.v1.endpoint.CleanupPolicyR\rcleanupPolicy\x12)\n\x10service_database\x18\x0f \x01(\tR\x0fserviceDatabaseBFZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,doublecloud/transfer/v1/endpoint/mysql.proto\x12 doublecloud.transfer.v1.endpoint\x1a-doublecloud/transfer/v1/endpoint/common.proto\"\x80\x01\n\x0eOnPremiseMysql\x12\x14\n\x05hosts\x18\x05 \x03(\tR\x05hosts\x12\x12\n\x04port\x18\x02 \x01(\x03R\x04port\x12\x44\n\x08tls_mode\x18\x06 \x01(\x0b\x32).doublecloud.transfer.v1.endpoint.TLSModeR\x07tlsMode\"r\n\x0fMysqlConnection\x12Q\n\non_premise\x18\x02 \x01(\x0b\x32\x30.doublecloud.transfer.v1.endpoint.OnPremiseMysqlH\x00R\tonPremiseB\x0c\n\nconnection\"\xd9\x02\n\x1bMysqlObjectTransferSettings\x12I\n\x04view\x18\x01 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x04view\x12O\n\x07routine\x18\x02 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x07routine\x12O\n\x07trigger\x18\x03 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x07trigger\x12M\n\x06tables\x18\x04 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x06tables\"\xfa\x03\n\x0bMysqlSource\x12Q\n\nconnection\x18\x01 \x01(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.MysqlConnectionR\nconnection\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12)\n\x10service_database\x18\x0f \x01(\tR\x0fserviceDatabase\x12\x12\n\x04user\x18\x03 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12\x30\n\x14include_tables_regex\x18\x0c \x03(\tR\x12includeTablesRegex\x12\x30\n\x14\x65xclude_tables_regex\x18\r \x03(\tR\x12\x65xcludeTablesRegex\x12\x1a\n\x08timezone\x18\x08 \x01(\tR\x08timezone\x12w\n\x18object_transfer_settings\x18\x0b \x01(\x0b\x32=.doublecloud.transfer.v1.endpoint.MysqlObjectTransferSettingsR\x16objectTransferSettings\"\xef\x03\n\x0bMysqlTarget\x12Q\n\nconnection\x18\x01 \x01(\x0b\x32\x31.doublecloud.transfer.v1.endpoint.MysqlConnectionR\nconnection\x12\'\n\x0fsecurity_groups\x18\x10 \x03(\tR\x0esecurityGroups\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12\x12\n\x04user\x18\x03 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12\x19\n\x08sql_mode\x18\x05 \x01(\tR\x07sqlMode\x12\x34\n\x16skip_constraint_checks\x18\x06 \x01(\x08R\x14skipConstraintChecks\x12\x1a\n\x08timezone\x18\x07 \x01(\tR\x08timezone\x12V\n\x0e\x63leanup_policy\x18\x08 \x01(\x0e\x32/.doublecloud.transfer.v1.endpoint.CleanupPolicyR\rcleanupPolicy\x12)\n\x10service_database\x18\x0f \x01(\tR\x0fserviceDatabaseBNZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.mysql_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpoint'
+  DESCRIPTOR._serialized_options = b'ZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpoint'
   _globals['_ONPREMISEMYSQL']._serialized_start=130
   _globals['_ONPREMISEMYSQL']._serialized_end=258
   _globals['_MYSQLCONNECTION']._serialized_start=260
   _globals['_MYSQLCONNECTION']._serialized_end=374
   _globals['_MYSQLOBJECTTRANSFERSETTINGS']._serialized_start=377
   _globals['_MYSQLOBJECTTRANSFERSETTINGS']._serialized_end=722
   _globals['_MYSQLSOURCE']._serialized_start=725
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/mysql_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/mysql_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/parsers_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/parsers.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.transfer.v1.endpoint import common_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.doublecloud/transfer/v1/endpoint/parsers.proto\x12 doublecloud.transfer.v1.endpoint\x1a-doublecloud/transfer/v1/endpoint/common.proto\"\xc6\x01\n\x06Parser\x12X\n\x0bjson_parser\x18\x01 \x01(\x0b\x32\x35.doublecloud.transfer.v1.endpoint.GenericParserCommonH\x00R\njsonParser\x12X\n\x0btskv_parser\x18\x06 \x01(\x0b\x32\x35.doublecloud.transfer.v1.endpoint.GenericParserCommonH\x00R\ntskvParserB\x08\n\x06parser\"\xb8\x01\n\x13GenericParserCommon\x12M\n\x0b\x64\x61ta_schema\x18\x01 \x01(\x0b\x32,.doublecloud.transfer.v1.endpoint.DataSchemaR\ndataSchema\x12*\n\x11null_keys_allowed\x18\x02 \x01(\x08R\x0fnullKeysAllowed\x12&\n\x0f\x61\x64\x64_rest_column\x18\x03 \x01(\x08R\raddRestColumnBFZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.doublecloud/transfer/v1/endpoint/parsers.proto\x12 doublecloud.transfer.v1.endpoint\x1a-doublecloud/transfer/v1/endpoint/common.proto\"\xc6\x01\n\x06Parser\x12X\n\x0bjson_parser\x18\x01 \x01(\x0b\x32\x35.doublecloud.transfer.v1.endpoint.GenericParserCommonH\x00R\njsonParser\x12X\n\x0btskv_parser\x18\x06 \x01(\x0b\x32\x35.doublecloud.transfer.v1.endpoint.GenericParserCommonH\x00R\ntskvParserB\x08\n\x06parser\"\xb8\x01\n\x13GenericParserCommon\x12M\n\x0b\x64\x61ta_schema\x18\x01 \x01(\x0b\x32,.doublecloud.transfer.v1.endpoint.DataSchemaR\ndataSchema\x12*\n\x11null_keys_allowed\x18\x02 \x01(\x08R\x0fnullKeysAllowed\x12&\n\x0f\x61\x64\x64_rest_column\x18\x03 \x01(\x08R\raddRestColumnBNZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.parsers_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpoint'
+  DESCRIPTOR._serialized_options = b'ZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpoint'
   _globals['_PARSER']._serialized_start=132
   _globals['_PARSER']._serialized_end=330
   _globals['_GENERICPARSERCOMMON']._serialized_start=333
   _globals['_GENERICPARSERCOMMON']._serialized_end=517
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/parsers_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/parsers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/postgres_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint/postgres.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.transfer.v1.endpoint import common_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/doublecloud/transfer/v1/endpoint/postgres.proto\x12 doublecloud.transfer.v1.endpoint\x1a-doublecloud/transfer/v1/endpoint/common.proto\"\x8b\x0c\n\x1ePostgresObjectTransferSettings\x12Q\n\x08sequence\x18\x01 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x08sequence\x12\x61\n\x11sequence_owned_by\x18\x02 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x0fsequenceOwnedBy\x12X\n\x0csequence_set\x18\x12 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x0bsequenceSet\x12K\n\x05table\x18\x03 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x05table\x12V\n\x0bprimary_key\x18\x04 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\nprimaryKey\x12Z\n\rfk_constraint\x18\x05 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x0c\x66kConstraint\x12\\\n\x0e\x64\x65\x66\x61ult_values\x18\x06 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\rdefaultValues\x12U\n\nconstraint\x18\x07 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\nconstraint\x12K\n\x05index\x18\x08 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x05index\x12I\n\x04view\x18\t \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x04view\x12\x62\n\x11materialized_view\x18\x11 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x10materializedView\x12Q\n\x08\x66unction\x18\n \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x08\x66unction\x12O\n\x07trigger\x18\x0b \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x07trigger\x12I\n\x04type\x18\x0c \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x04type\x12I\n\x04rule\x18\r \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x04rule\x12S\n\tcollation\x18\x0e \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\tcollation\x12M\n\x06policy\x18\x0f \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x06policy\x12I\n\x04\x63\x61st\x18\x10 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x04\x63\x61st\"\x83\x01\n\x11OnPremisePostgres\x12\x14\n\x05hosts\x18\x05 \x03(\tR\x05hosts\x12\x12\n\x04port\x18\x02 \x01(\x03R\x04port\x12\x44\n\x08tls_mode\x18\x06 \x01(\x0b\x32).doublecloud.transfer.v1.endpoint.TLSModeR\x07tlsMode\"x\n\x12PostgresConnection\x12T\n\non_premise\x18\x02 \x01(\x0b\x32\x33.doublecloud.transfer.v1.endpoint.OnPremisePostgresH\x00R\tonPremiseB\x0c\n\nconnection\"\xfc\x03\n\x0ePostgresSource\x12T\n\nconnection\x18\x01 \x01(\x0b\x32\x34.doublecloud.transfer.v1.endpoint.PostgresConnectionR\nconnection\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12\x12\n\x04user\x18\x03 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12%\n\x0einclude_tables\x18\x05 \x03(\tR\rincludeTables\x12%\n\x0e\x65xclude_tables\x18\x06 \x03(\tR\rexcludeTables\x12-\n\x13slot_byte_lag_limit\x18\x08 \x01(\x03R\x10slotByteLagLimit\x12%\n\x0eservice_schema\x18\t \x01(\tR\rserviceSchema\x12z\n\x18object_transfer_settings\x18\r \x01(\x0b\x32@.doublecloud.transfer.v1.endpoint.PostgresObjectTransferSettingsR\x16objectTransferSettings\"\xdd\x02\n\x0ePostgresTarget\x12T\n\nconnection\x18\x01 \x01(\x0b\x32\x34.doublecloud.transfer.v1.endpoint.PostgresConnectionR\nconnection\x12\'\n\x0fsecurity_groups\x18\x07 \x03(\tR\x0esecurityGroups\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12\x12\n\x04user\x18\x03 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12V\n\x0e\x63leanup_policy\x18\x05 \x01(\x0e\x32/.doublecloud.transfer.v1.endpoint.CleanupPolicyR\rcleanupPolicyBFZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/doublecloud/transfer/v1/endpoint/postgres.proto\x12 doublecloud.transfer.v1.endpoint\x1a-doublecloud/transfer/v1/endpoint/common.proto\"\x8b\x0c\n\x1ePostgresObjectTransferSettings\x12Q\n\x08sequence\x18\x01 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x08sequence\x12\x61\n\x11sequence_owned_by\x18\x02 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x0fsequenceOwnedBy\x12X\n\x0csequence_set\x18\x12 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x0bsequenceSet\x12K\n\x05table\x18\x03 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x05table\x12V\n\x0bprimary_key\x18\x04 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\nprimaryKey\x12Z\n\rfk_constraint\x18\x05 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x0c\x66kConstraint\x12\\\n\x0e\x64\x65\x66\x61ult_values\x18\x06 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\rdefaultValues\x12U\n\nconstraint\x18\x07 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\nconstraint\x12K\n\x05index\x18\x08 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x05index\x12I\n\x04view\x18\t \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x04view\x12\x62\n\x11materialized_view\x18\x11 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x10materializedView\x12Q\n\x08\x66unction\x18\n \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x08\x66unction\x12O\n\x07trigger\x18\x0b \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x07trigger\x12I\n\x04type\x18\x0c \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x04type\x12I\n\x04rule\x18\r \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x04rule\x12S\n\tcollation\x18\x0e \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\tcollation\x12M\n\x06policy\x18\x0f \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x06policy\x12I\n\x04\x63\x61st\x18\x10 \x01(\x0e\x32\x35.doublecloud.transfer.v1.endpoint.ObjectTransferStageR\x04\x63\x61st\"\x83\x01\n\x11OnPremisePostgres\x12\x14\n\x05hosts\x18\x05 \x03(\tR\x05hosts\x12\x12\n\x04port\x18\x02 \x01(\x03R\x04port\x12\x44\n\x08tls_mode\x18\x06 \x01(\x0b\x32).doublecloud.transfer.v1.endpoint.TLSModeR\x07tlsMode\"x\n\x12PostgresConnection\x12T\n\non_premise\x18\x02 \x01(\x0b\x32\x33.doublecloud.transfer.v1.endpoint.OnPremisePostgresH\x00R\tonPremiseB\x0c\n\nconnection\"\xfc\x03\n\x0ePostgresSource\x12T\n\nconnection\x18\x01 \x01(\x0b\x32\x34.doublecloud.transfer.v1.endpoint.PostgresConnectionR\nconnection\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12\x12\n\x04user\x18\x03 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12%\n\x0einclude_tables\x18\x05 \x03(\tR\rincludeTables\x12%\n\x0e\x65xclude_tables\x18\x06 \x03(\tR\rexcludeTables\x12-\n\x13slot_byte_lag_limit\x18\x08 \x01(\x03R\x10slotByteLagLimit\x12%\n\x0eservice_schema\x18\t \x01(\tR\rserviceSchema\x12z\n\x18object_transfer_settings\x18\r \x01(\x0b\x32@.doublecloud.transfer.v1.endpoint.PostgresObjectTransferSettingsR\x16objectTransferSettings\"\xdd\x02\n\x0ePostgresTarget\x12T\n\nconnection\x18\x01 \x01(\x0b\x32\x34.doublecloud.transfer.v1.endpoint.PostgresConnectionR\nconnection\x12\'\n\x0fsecurity_groups\x18\x07 \x03(\tR\x0esecurityGroups\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12\x12\n\x04user\x18\x03 \x01(\tR\x04user\x12\x44\n\x08password\x18\x04 \x01(\x0b\x32(.doublecloud.transfer.v1.endpoint.SecretR\x08password\x12V\n\x0e\x63leanup_policy\x18\x05 \x01(\x0e\x32/.doublecloud.transfer.v1.endpoint.CleanupPolicyR\rcleanupPolicyBNZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpointb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint.postgres_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZDgithub.com/doublecloud/api/doublecloud/transfer/v1/endpoint;endpoint'
+  DESCRIPTOR._serialized_options = b'ZLgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1/endpoint;endpoint'
   _globals['_POSTGRESOBJECTTRANSFERSETTINGS']._serialized_start=133
   _globals['_POSTGRESOBJECTTRANSFERSETTINGS']._serialized_end=1680
   _globals['_ONPREMISEPOSTGRES']._serialized_start=1683
   _globals['_ONPREMISEPOSTGRES']._serialized_end=1814
   _globals['_POSTGRESCONNECTION']._serialized_start=1816
   _globals['_POSTGRESCONNECTION']._serialized_end=1936
   _globals['_POSTGRESSOURCE']._serialized_start=1939
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint/postgres_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint/postgres_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.transfer.v1.endpoint import clickhouse_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_clickhouse__pb2
 from doublecloud.transfer.v1.endpoint import common_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_common__pb2
@@ -23,27 +23,28 @@
 from doublecloud.transfer.v1.endpoint.airbyte import bigquery_source_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_airbyte_dot_bigquery__source__pb2
 from doublecloud.transfer.v1.endpoint.airbyte import mssql_source_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_airbyte_dot_mssql__source__pb2
 from doublecloud.transfer.v1.endpoint.airbyte import amazon_ads_source_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_airbyte_dot_amazon__ads__source__pb2
 from doublecloud.transfer.v1.endpoint.airbyte import facebook_marketing_source_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_airbyte_dot_facebook__marketing__source__pb2
 from doublecloud.transfer.v1.endpoint.airbyte import linkedin_ads_source_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_airbyte_dot_linkedin__ads__source__pb2
 from doublecloud.transfer.v1.endpoint.airbyte import instagram_source_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_airbyte_dot_instagram__source__pb2
 from doublecloud.transfer.v1.endpoint.airbyte import google_ads_source_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_airbyte_dot_google__ads__source__pb2
+from doublecloud.transfer.v1.endpoint.airbyte import snowflake_source_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint_dot_airbyte_dot_snowflake__source__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&doublecloud/transfer/v1/endpoint.proto\x12\x17\x64oublecloud.transfer.v1\x1a\x31\x64oublecloud/transfer/v1/endpoint/clickhouse.proto\x1a-doublecloud/transfer/v1/endpoint/common.proto\x1a,doublecloud/transfer/v1/endpoint/kafka.proto\x1a,doublecloud/transfer/v1/endpoint/mongo.proto\x1a,doublecloud/transfer/v1/endpoint/mysql.proto\x1a/doublecloud/transfer/v1/endpoint/postgres.proto\x1a\x38\x64oublecloud/transfer/v1/endpoint/airbyte/s3_source.proto\x1a>doublecloud/transfer/v1/endpoint/airbyte/redshift_source.proto\x1a\x45\x64oublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source.proto\x1a>doublecloud/transfer/v1/endpoint/airbyte/bigquery_source.proto\x1a;doublecloud/transfer/v1/endpoint/airbyte/mssql_source.proto\x1a@doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source.proto\x1aHdoublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source.proto\x1a\x42\x64oublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source.proto\x1a?doublecloud/transfer/v1/endpoint/airbyte/instagram_source.proto\x1a@doublecloud/transfer/v1/endpoint/airbyte/google_ads_source.proto\"\xb8\x02\n\x08\x45ndpoint\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x45\n\x06labels\x18\x06 \x03(\x0b\x32-.doublecloud.transfer.v1.Endpoint.LabelsEntryR\x06labels\x12\x45\n\x08settings\x18\x34 \x01(\x0b\x32).doublecloud.transfer.v1.EndpointSettingsR\x08settings\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xb8\x0f\n\x10\x45ndpointSettings\x12R\n\x0cmysql_source\x18\x01 \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.MysqlSourceH\x00R\x0bmysqlSource\x12[\n\x0fpostgres_source\x18\x02 \x01(\x0b\x32\x30.doublecloud.transfer.v1.endpoint.PostgresSourceH\x00R\x0epostgresSource\x12R\n\x0ckafka_source\x18\x08 \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.KafkaSourceH\x00R\x0bkafkaSource\x12R\n\x0cmongo_source\x18\t \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.MongoSourceH\x00R\x0bmongoSource\x12\x61\n\x11\x63lickhouse_source\x18\x10 \x01(\x0b\x32\x32.doublecloud.transfer.v1.endpoint.ClickhouseSourceH\x00R\x10\x63lickhouseSource\x12Q\n\ts3_source\x18| \x01(\x0b\x32\x32.doublecloud.transfer.v1.endpoint.airbyte.S3SourceH\x00R\x08s3Source\x12s\n\x15\x61ws_cloudtrail_source\x18\x7f \x01(\x0b\x32=.doublecloud.transfer.v1.endpoint.airbyte.AWSCloudTrailSourceH\x00R\x13\x61wsCloudtrailSource\x12\x65\n\x10\x62ig_query_source\x18\x80\x01 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.airbyte.BigQuerySourceH\x00R\x0e\x62igQuerySource\x12\x80\x01\n\x19\x66\x61\x63\x65\x62ook_marketing_source\x18\x82\x01 \x01(\x0b\x32\x41.doublecloud.transfer.v1.endpoint.airbyte.FacebookMarketingSourceH\x00R\x17\x66\x61\x63\x65\x62ookMarketingSource\x12h\n\x11google_ads_source\x18\x84\x01 \x01(\x0b\x32\x39.doublecloud.transfer.v1.endpoint.airbyte.GoogleAdsSourceH\x00R\x0fgoogleAdsSource\x12h\n\x11\x61mazon_ads_source\x18\x86\x01 \x01(\x0b\x32\x39.doublecloud.transfer.v1.endpoint.airbyte.AmazonAdsSourceH\x00R\x0f\x61mazonAdsSource\x12g\n\x10instagram_source\x18\x88\x01 \x01(\x0b\x32\x39.doublecloud.transfer.v1.endpoint.airbyte.InstagramSourceH\x00R\x0finstagramSource\x12n\n\x13linkedin_ads_source\x18\x89\x01 \x01(\x0b\x32;.doublecloud.transfer.v1.endpoint.airbyte.LinkedinAdsSourceH\x00R\x11linkedinAdsSource\x12[\n\x0cmssql_source\x18\x8a\x01 \x01(\x0b\x32\x35.doublecloud.transfer.v1.endpoint.airbyte.MSSQLSourceH\x00R\x0bmssqlSource\x12\x64\n\x0fredshift_source\x18\x8b\x01 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.airbyte.RedshiftSourceH\x00R\x0eredshiftSource\x12R\n\x0cmysql_target\x18\x65 \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.MysqlTargetH\x00R\x0bmysqlTarget\x12[\n\x0fpostgres_target\x18\x66 \x01(\x0b\x32\x30.doublecloud.transfer.v1.endpoint.PostgresTargetH\x00R\x0epostgresTarget\x12\x61\n\x11\x63lickhouse_target\x18h \x01(\x0b\x32\x32.doublecloud.transfer.v1.endpoint.ClickhouseTargetH\x00R\x10\x63lickhouseTarget\x12R\n\x0ckafka_target\x18n \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.KafkaTargetH\x00R\x0bkafkaTarget\x12R\n\x0cmongo_target\x18o \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.MongoTargetH\x00R\x0bmongoTargetB\n\n\x08settingsB=Z;github.com/doublecloud/api/doublecloud/transfer/v1;transferb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&doublecloud/transfer/v1/endpoint.proto\x12\x17\x64oublecloud.transfer.v1\x1a\x31\x64oublecloud/transfer/v1/endpoint/clickhouse.proto\x1a-doublecloud/transfer/v1/endpoint/common.proto\x1a,doublecloud/transfer/v1/endpoint/kafka.proto\x1a,doublecloud/transfer/v1/endpoint/mongo.proto\x1a,doublecloud/transfer/v1/endpoint/mysql.proto\x1a/doublecloud/transfer/v1/endpoint/postgres.proto\x1a\x38\x64oublecloud/transfer/v1/endpoint/airbyte/s3_source.proto\x1a>doublecloud/transfer/v1/endpoint/airbyte/redshift_source.proto\x1a\x45\x64oublecloud/transfer/v1/endpoint/airbyte/aws_cloud_trail_source.proto\x1a>doublecloud/transfer/v1/endpoint/airbyte/bigquery_source.proto\x1a;doublecloud/transfer/v1/endpoint/airbyte/mssql_source.proto\x1a@doublecloud/transfer/v1/endpoint/airbyte/amazon_ads_source.proto\x1aHdoublecloud/transfer/v1/endpoint/airbyte/facebook_marketing_source.proto\x1a\x42\x64oublecloud/transfer/v1/endpoint/airbyte/linkedin_ads_source.proto\x1a?doublecloud/transfer/v1/endpoint/airbyte/instagram_source.proto\x1a@doublecloud/transfer/v1/endpoint/airbyte/google_ads_source.proto\x1a?doublecloud/transfer/v1/endpoint/airbyte/snowflake_source.proto\"\xb8\x02\n\x08\x45ndpoint\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x45\n\x06labels\x18\x06 \x03(\x0b\x32-.doublecloud.transfer.v1.Endpoint.LabelsEntryR\x06labels\x12\x45\n\x08settings\x18\x34 \x01(\x0b\x32).doublecloud.transfer.v1.EndpointSettingsR\x08settings\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xa1\x10\n\x10\x45ndpointSettings\x12R\n\x0cmysql_source\x18\x01 \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.MysqlSourceH\x00R\x0bmysqlSource\x12[\n\x0fpostgres_source\x18\x02 \x01(\x0b\x32\x30.doublecloud.transfer.v1.endpoint.PostgresSourceH\x00R\x0epostgresSource\x12R\n\x0ckafka_source\x18\x08 \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.KafkaSourceH\x00R\x0bkafkaSource\x12R\n\x0cmongo_source\x18\t \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.MongoSourceH\x00R\x0bmongoSource\x12\x61\n\x11\x63lickhouse_source\x18\x10 \x01(\x0b\x32\x32.doublecloud.transfer.v1.endpoint.ClickhouseSourceH\x00R\x10\x63lickhouseSource\x12Q\n\ts3_source\x18| \x01(\x0b\x32\x32.doublecloud.transfer.v1.endpoint.airbyte.S3SourceH\x00R\x08s3Source\x12s\n\x15\x61ws_cloudtrail_source\x18\x7f \x01(\x0b\x32=.doublecloud.transfer.v1.endpoint.airbyte.AWSCloudTrailSourceH\x00R\x13\x61wsCloudtrailSource\x12\x65\n\x10\x62ig_query_source\x18\x80\x01 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.airbyte.BigQuerySourceH\x00R\x0e\x62igQuerySource\x12\x80\x01\n\x19\x66\x61\x63\x65\x62ook_marketing_source\x18\x82\x01 \x01(\x0b\x32\x41.doublecloud.transfer.v1.endpoint.airbyte.FacebookMarketingSourceH\x00R\x17\x66\x61\x63\x65\x62ookMarketingSource\x12h\n\x11google_ads_source\x18\x84\x01 \x01(\x0b\x32\x39.doublecloud.transfer.v1.endpoint.airbyte.GoogleAdsSourceH\x00R\x0fgoogleAdsSource\x12h\n\x11\x61mazon_ads_source\x18\x86\x01 \x01(\x0b\x32\x39.doublecloud.transfer.v1.endpoint.airbyte.AmazonAdsSourceH\x00R\x0f\x61mazonAdsSource\x12g\n\x10instagram_source\x18\x88\x01 \x01(\x0b\x32\x39.doublecloud.transfer.v1.endpoint.airbyte.InstagramSourceH\x00R\x0finstagramSource\x12n\n\x13linkedin_ads_source\x18\x89\x01 \x01(\x0b\x32;.doublecloud.transfer.v1.endpoint.airbyte.LinkedinAdsSourceH\x00R\x11linkedinAdsSource\x12[\n\x0cmssql_source\x18\x8a\x01 \x01(\x0b\x32\x35.doublecloud.transfer.v1.endpoint.airbyte.MSSQLSourceH\x00R\x0bmssqlSource\x12\x64\n\x0fredshift_source\x18\x8b\x01 \x01(\x0b\x32\x38.doublecloud.transfer.v1.endpoint.airbyte.RedshiftSourceH\x00R\x0eredshiftSource\x12g\n\x10snowflake_source\x18\x94\x01 \x01(\x0b\x32\x39.doublecloud.transfer.v1.endpoint.airbyte.SnowflakeSourceH\x00R\x0fsnowflakeSource\x12R\n\x0cmysql_target\x18\x65 \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.MysqlTargetH\x00R\x0bmysqlTarget\x12[\n\x0fpostgres_target\x18\x66 \x01(\x0b\x32\x30.doublecloud.transfer.v1.endpoint.PostgresTargetH\x00R\x0epostgresTarget\x12\x61\n\x11\x63lickhouse_target\x18h \x01(\x0b\x32\x32.doublecloud.transfer.v1.endpoint.ClickhouseTargetH\x00R\x10\x63lickhouseTarget\x12R\n\x0ckafka_target\x18n \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.KafkaTargetH\x00R\x0bkafkaTarget\x12R\n\x0cmongo_target\x18o \x01(\x0b\x32-.doublecloud.transfer.v1.endpoint.MongoTargetH\x00R\x0bmongoTargetB\n\n\x08settingsBEZCgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1;transferb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z;github.com/doublecloud/api/doublecloud/transfer/v1;transfer'
+  DESCRIPTOR._serialized_options = b'ZCgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1;transfer'
   _ENDPOINT_LABELSENTRY._options = None
   _ENDPOINT_LABELSENTRY._serialized_options = b'8\001'
-  _globals['_ENDPOINT']._serialized_start=1010
-  _globals['_ENDPOINT']._serialized_end=1322
-  _globals['_ENDPOINT_LABELSENTRY']._serialized_start=1265
-  _globals['_ENDPOINT_LABELSENTRY']._serialized_end=1322
-  _globals['_ENDPOINTSETTINGS']._serialized_start=1325
-  _globals['_ENDPOINTSETTINGS']._serialized_end=3301
+  _globals['_ENDPOINT']._serialized_start=1075
+  _globals['_ENDPOINT']._serialized_end=1387
+  _globals['_ENDPOINT_LABELSENTRY']._serialized_start=1330
+  _globals['_ENDPOINT_LABELSENTRY']._serialized_end=1387
+  _globals['_ENDPOINTSETTINGS']._serialized_start=1390
+  _globals['_ENDPOINTSETTINGS']._serialized_end=3471
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from doublecloud.transfer.v1.endpoint.airbyte import bigquery_source_pb2 as _bigquery_source_pb2
 from doublecloud.transfer.v1.endpoint.airbyte import mssql_source_pb2 as _mssql_source_pb2
 from doublecloud.transfer.v1.endpoint.airbyte import amazon_ads_source_pb2 as _amazon_ads_source_pb2
 from doublecloud.transfer.v1.endpoint.airbyte import facebook_marketing_source_pb2 as _facebook_marketing_source_pb2
 from doublecloud.transfer.v1.endpoint.airbyte import linkedin_ads_source_pb2 as _linkedin_ads_source_pb2
 from doublecloud.transfer.v1.endpoint.airbyte import instagram_source_pb2 as _instagram_source_pb2
 from doublecloud.transfer.v1.endpoint.airbyte import google_ads_source_pb2 as _google_ads_source_pb2
+from doublecloud.transfer.v1.endpoint.airbyte import snowflake_source_pb2 as _snowflake_source_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
@@ -41,15 +42,15 @@
     name: str
     description: str
     labels: _containers.ScalarMap[str, str]
     settings: EndpointSettings
     def __init__(self, id: _Optional[str] = ..., project_id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ..., labels: _Optional[_Mapping[str, str]] = ..., settings: _Optional[_Union[EndpointSettings, _Mapping]] = ...) -> None: ...
 
 class EndpointSettings(_message.Message):
-    __slots__ = ["mysql_source", "postgres_source", "kafka_source", "mongo_source", "clickhouse_source", "s3_source", "aws_cloudtrail_source", "big_query_source", "facebook_marketing_source", "google_ads_source", "amazon_ads_source", "instagram_source", "linkedin_ads_source", "mssql_source", "redshift_source", "mysql_target", "postgres_target", "clickhouse_target", "kafka_target", "mongo_target"]
+    __slots__ = ["mysql_source", "postgres_source", "kafka_source", "mongo_source", "clickhouse_source", "s3_source", "aws_cloudtrail_source", "big_query_source", "facebook_marketing_source", "google_ads_source", "amazon_ads_source", "instagram_source", "linkedin_ads_source", "mssql_source", "redshift_source", "snowflake_source", "mysql_target", "postgres_target", "clickhouse_target", "kafka_target", "mongo_target"]
     MYSQL_SOURCE_FIELD_NUMBER: _ClassVar[int]
     POSTGRES_SOURCE_FIELD_NUMBER: _ClassVar[int]
     KAFKA_SOURCE_FIELD_NUMBER: _ClassVar[int]
     MONGO_SOURCE_FIELD_NUMBER: _ClassVar[int]
     CLICKHOUSE_SOURCE_FIELD_NUMBER: _ClassVar[int]
     S3_SOURCE_FIELD_NUMBER: _ClassVar[int]
     AWS_CLOUDTRAIL_SOURCE_FIELD_NUMBER: _ClassVar[int]
@@ -57,14 +58,15 @@
     FACEBOOK_MARKETING_SOURCE_FIELD_NUMBER: _ClassVar[int]
     GOOGLE_ADS_SOURCE_FIELD_NUMBER: _ClassVar[int]
     AMAZON_ADS_SOURCE_FIELD_NUMBER: _ClassVar[int]
     INSTAGRAM_SOURCE_FIELD_NUMBER: _ClassVar[int]
     LINKEDIN_ADS_SOURCE_FIELD_NUMBER: _ClassVar[int]
     MSSQL_SOURCE_FIELD_NUMBER: _ClassVar[int]
     REDSHIFT_SOURCE_FIELD_NUMBER: _ClassVar[int]
+    SNOWFLAKE_SOURCE_FIELD_NUMBER: _ClassVar[int]
     MYSQL_TARGET_FIELD_NUMBER: _ClassVar[int]
     POSTGRES_TARGET_FIELD_NUMBER: _ClassVar[int]
     CLICKHOUSE_TARGET_FIELD_NUMBER: _ClassVar[int]
     KAFKA_TARGET_FIELD_NUMBER: _ClassVar[int]
     MONGO_TARGET_FIELD_NUMBER: _ClassVar[int]
     mysql_source: _mysql_pb2.MysqlSource
     postgres_source: _postgres_pb2.PostgresSource
@@ -77,13 +79,14 @@
     facebook_marketing_source: _facebook_marketing_source_pb2.FacebookMarketingSource
     google_ads_source: _google_ads_source_pb2.GoogleAdsSource
     amazon_ads_source: _amazon_ads_source_pb2.AmazonAdsSource
     instagram_source: _instagram_source_pb2.InstagramSource
     linkedin_ads_source: _linkedin_ads_source_pb2.LinkedinAdsSource
     mssql_source: _mssql_source_pb2.MSSQLSource
     redshift_source: _redshift_source_pb2.RedshiftSource
+    snowflake_source: _snowflake_source_pb2.SnowflakeSource
     mysql_target: _mysql_pb2.MysqlTarget
     postgres_target: _postgres_pb2.PostgresTarget
     clickhouse_target: _clickhouse_pb2.ClickhouseTarget
     kafka_target: _kafka_pb2.KafkaTarget
     mongo_target: _mongo_pb2.MongoTarget
-    def __init__(self, mysql_source: _Optional[_Union[_mysql_pb2.MysqlSource, _Mapping]] = ..., postgres_source: _Optional[_Union[_postgres_pb2.PostgresSource, _Mapping]] = ..., kafka_source: _Optional[_Union[_kafka_pb2.KafkaSource, _Mapping]] = ..., mongo_source: _Optional[_Union[_mongo_pb2.MongoSource, _Mapping]] = ..., clickhouse_source: _Optional[_Union[_clickhouse_pb2.ClickhouseSource, _Mapping]] = ..., s3_source: _Optional[_Union[_s3_source_pb2.S3Source, _Mapping]] = ..., aws_cloudtrail_source: _Optional[_Union[_aws_cloud_trail_source_pb2.AWSCloudTrailSource, _Mapping]] = ..., big_query_source: _Optional[_Union[_bigquery_source_pb2.BigQuerySource, _Mapping]] = ..., facebook_marketing_source: _Optional[_Union[_facebook_marketing_source_pb2.FacebookMarketingSource, _Mapping]] = ..., google_ads_source: _Optional[_Union[_google_ads_source_pb2.GoogleAdsSource, _Mapping]] = ..., amazon_ads_source: _Optional[_Union[_amazon_ads_source_pb2.AmazonAdsSource, _Mapping]] = ..., instagram_source: _Optional[_Union[_instagram_source_pb2.InstagramSource, _Mapping]] = ..., linkedin_ads_source: _Optional[_Union[_linkedin_ads_source_pb2.LinkedinAdsSource, _Mapping]] = ..., mssql_source: _Optional[_Union[_mssql_source_pb2.MSSQLSource, _Mapping]] = ..., redshift_source: _Optional[_Union[_redshift_source_pb2.RedshiftSource, _Mapping]] = ..., mysql_target: _Optional[_Union[_mysql_pb2.MysqlTarget, _Mapping]] = ..., postgres_target: _Optional[_Union[_postgres_pb2.PostgresTarget, _Mapping]] = ..., clickhouse_target: _Optional[_Union[_clickhouse_pb2.ClickhouseTarget, _Mapping]] = ..., kafka_target: _Optional[_Union[_kafka_pb2.KafkaTarget, _Mapping]] = ..., mongo_target: _Optional[_Union[_mongo_pb2.MongoTarget, _Mapping]] = ...) -> None: ...
+    def __init__(self, mysql_source: _Optional[_Union[_mysql_pb2.MysqlSource, _Mapping]] = ..., postgres_source: _Optional[_Union[_postgres_pb2.PostgresSource, _Mapping]] = ..., kafka_source: _Optional[_Union[_kafka_pb2.KafkaSource, _Mapping]] = ..., mongo_source: _Optional[_Union[_mongo_pb2.MongoSource, _Mapping]] = ..., clickhouse_source: _Optional[_Union[_clickhouse_pb2.ClickhouseSource, _Mapping]] = ..., s3_source: _Optional[_Union[_s3_source_pb2.S3Source, _Mapping]] = ..., aws_cloudtrail_source: _Optional[_Union[_aws_cloud_trail_source_pb2.AWSCloudTrailSource, _Mapping]] = ..., big_query_source: _Optional[_Union[_bigquery_source_pb2.BigQuerySource, _Mapping]] = ..., facebook_marketing_source: _Optional[_Union[_facebook_marketing_source_pb2.FacebookMarketingSource, _Mapping]] = ..., google_ads_source: _Optional[_Union[_google_ads_source_pb2.GoogleAdsSource, _Mapping]] = ..., amazon_ads_source: _Optional[_Union[_amazon_ads_source_pb2.AmazonAdsSource, _Mapping]] = ..., instagram_source: _Optional[_Union[_instagram_source_pb2.InstagramSource, _Mapping]] = ..., linkedin_ads_source: _Optional[_Union[_linkedin_ads_source_pb2.LinkedinAdsSource, _Mapping]] = ..., mssql_source: _Optional[_Union[_mssql_source_pb2.MSSQLSource, _Mapping]] = ..., redshift_source: _Optional[_Union[_redshift_source_pb2.RedshiftSource, _Mapping]] = ..., snowflake_source: _Optional[_Union[_snowflake_source_pb2.SnowflakeSource, _Mapping]] = ..., mysql_target: _Optional[_Union[_mysql_pb2.MysqlTarget, _Mapping]] = ..., postgres_target: _Optional[_Union[_postgres_pb2.PostgresTarget, _Mapping]] = ..., clickhouse_target: _Optional[_Union[_clickhouse_pb2.ClickhouseTarget, _Mapping]] = ..., kafka_target: _Optional[_Union[_kafka_pb2.KafkaTarget, _Mapping]] = ..., mongo_target: _Optional[_Union[_mongo_pb2.MongoTarget, _Mapping]] = ...) -> None: ...
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint_service_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/endpoint_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from doublecloud.transfer.v1 import endpoint_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint__pb2
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.doublecloud/transfer/v1/endpoint_service.proto\x12\x17\x64oublecloud.transfer.v1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a&doublecloud/transfer/v1/endpoint.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"5\n\x12GetEndpointRequest\x12\x1f\n\x0b\x65ndpoint_id\x18\x01 \x01(\tR\nendpointId\"a\n\x14ListEndpointsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12*\n\x04page\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x04page\"\x8f\x01\n\x15ListEndpointsResponse\x12?\n\tendpoints\x18\x01 \x03(\x0b\x32!.doublecloud.transfer.v1.EndpointR\tendpoints\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\xc2\x02\n\x15\x43reateEndpointRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12R\n\x06labels\x18\x04 \x03(\x0b\x32:.doublecloud.transfer.v1.CreateEndpointRequest.LabelsEntryR\x06labels\x12\x45\n\x08settings\x18\x34 \x01(\x0b\x32).doublecloud.transfer.v1.EndpointSettingsR\x08settings\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xc4\x02\n\x15UpdateEndpointRequest\x12\x1f\n\x0b\x65ndpoint_id\x18\n \x01(\tR\nendpointId\x12\x12\n\x04name\x18\x0b \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x0c \x01(\tR\x0b\x64\x65scription\x12R\n\x06labels\x18\r \x03(\x0b\x32:.doublecloud.transfer.v1.UpdateEndpointRequest.LabelsEntryR\x06labels\x12\x45\n\x08settings\x18\x34 \x01(\x0b\x32).doublecloud.transfer.v1.EndpointSettingsR\x08settings\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"8\n\x15\x44\x65leteEndpointRequest\x12\x1f\n\x0b\x65ndpoint_id\x18\x01 \x01(\tR\nendpointId2\x80\x05\n\x0f\x45ndpointService\x12y\n\x03Get\x12+.doublecloud.transfer.v1.GetEndpointRequest\x1a!.doublecloud.transfer.v1.Endpoint\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/v1/endpoint/{endpoint_id}\x12\x8e\x01\n\x04List\x12-.doublecloud.transfer.v1.ListEndpointsRequest\x1a..doublecloud.transfer.v1.ListEndpointsResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/v1/endpoints/list/{project_id}\x12l\n\x06\x43reate\x12..doublecloud.transfer.v1.CreateEndpointRequest\x1a\x19.doublecloud.v1.Operation\"\x17\x82\xd3\xe4\x93\x02\x11:\x01*\"\x0c/v1/endpoint\x12z\n\x06Update\x12..doublecloud.transfer.v1.UpdateEndpointRequest\x1a\x19.doublecloud.v1.Operation\"%\x82\xd3\xe4\x93\x02\x1f:\x01*2\x1a/v1/endpoint/{endpoint_id}\x12w\n\x06\x44\x65lete\x12..doublecloud.transfer.v1.DeleteEndpointRequest\x1a\x19.doublecloud.v1.Operation\"\"\x82\xd3\xe4\x93\x02\x1c*\x1a/v1/endpoint/{endpoint_id}B=Z;github.com/doublecloud/api/doublecloud/transfer/v1;transferb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.doublecloud/transfer/v1/endpoint_service.proto\x12\x17\x64oublecloud.transfer.v1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a&doublecloud/transfer/v1/endpoint.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"5\n\x12GetEndpointRequest\x12\x1f\n\x0b\x65ndpoint_id\x18\x01 \x01(\tR\nendpointId\"a\n\x14ListEndpointsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12*\n\x04page\x18\x02 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x04page\"\x8f\x01\n\x15ListEndpointsResponse\x12?\n\tendpoints\x18\x01 \x03(\x0b\x32!.doublecloud.transfer.v1.EndpointR\tendpoints\x12\x35\n\tnext_page\x18\x02 \x01(\x0b\x32\x18.doublecloud.v1.NextPageR\x08nextPage\"\xc2\x02\n\x15\x43reateEndpointRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12R\n\x06labels\x18\x04 \x03(\x0b\x32:.doublecloud.transfer.v1.CreateEndpointRequest.LabelsEntryR\x06labels\x12\x45\n\x08settings\x18\x34 \x01(\x0b\x32).doublecloud.transfer.v1.EndpointSettingsR\x08settings\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xc4\x02\n\x15UpdateEndpointRequest\x12\x1f\n\x0b\x65ndpoint_id\x18\n \x01(\tR\nendpointId\x12\x12\n\x04name\x18\x0b \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x0c \x01(\tR\x0b\x64\x65scription\x12R\n\x06labels\x18\r \x03(\x0b\x32:.doublecloud.transfer.v1.UpdateEndpointRequest.LabelsEntryR\x06labels\x12\x45\n\x08settings\x18\x34 \x01(\x0b\x32).doublecloud.transfer.v1.EndpointSettingsR\x08settings\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"8\n\x15\x44\x65leteEndpointRequest\x12\x1f\n\x0b\x65ndpoint_id\x18\x01 \x01(\tR\nendpointId2\x80\x05\n\x0f\x45ndpointService\x12y\n\x03Get\x12+.doublecloud.transfer.v1.GetEndpointRequest\x1a!.doublecloud.transfer.v1.Endpoint\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/v1/endpoint/{endpoint_id}\x12\x8e\x01\n\x04List\x12-.doublecloud.transfer.v1.ListEndpointsRequest\x1a..doublecloud.transfer.v1.ListEndpointsResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/v1/endpoints/list/{project_id}\x12l\n\x06\x43reate\x12..doublecloud.transfer.v1.CreateEndpointRequest\x1a\x19.doublecloud.v1.Operation\"\x17\x82\xd3\xe4\x93\x02\x11\"\x0c/v1/endpoint:\x01*\x12z\n\x06Update\x12..doublecloud.transfer.v1.UpdateEndpointRequest\x1a\x19.doublecloud.v1.Operation\"%\x82\xd3\xe4\x93\x02\x1f\x32\x1a/v1/endpoint/{endpoint_id}:\x01*\x12w\n\x06\x44\x65lete\x12..doublecloud.transfer.v1.DeleteEndpointRequest\x1a\x19.doublecloud.v1.Operation\"\"\x82\xd3\xe4\x93\x02\x1c*\x1a/v1/endpoint/{endpoint_id}BEZCgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1;transferb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.endpoint_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z;github.com/doublecloud/api/doublecloud/transfer/v1;transfer'
+  DESCRIPTOR._serialized_options = b'ZCgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1;transfer'
   _CREATEENDPOINTREQUEST_LABELSENTRY._options = None
   _CREATEENDPOINTREQUEST_LABELSENTRY._serialized_options = b'8\001'
   _UPDATEENDPOINTREQUEST_LABELSENTRY._options = None
   _UPDATEENDPOINTREQUEST_LABELSENTRY._serialized_options = b'8\001'
   _ENDPOINTSERVICE.methods_by_name['Get']._options = None
   _ENDPOINTSERVICE.methods_by_name['Get']._serialized_options = b'\202\323\344\223\002\034\022\032/v1/endpoint/{endpoint_id}'
   _ENDPOINTSERVICE.methods_by_name['List']._options = None
   _ENDPOINTSERVICE.methods_by_name['List']._serialized_options = b'\202\323\344\223\002!\022\037/v1/endpoints/list/{project_id}'
   _ENDPOINTSERVICE.methods_by_name['Create']._options = None
-  _ENDPOINTSERVICE.methods_by_name['Create']._serialized_options = b'\202\323\344\223\002\021:\001*\"\014/v1/endpoint'
+  _ENDPOINTSERVICE.methods_by_name['Create']._serialized_options = b'\202\323\344\223\002\021\"\014/v1/endpoint:\001*'
   _ENDPOINTSERVICE.methods_by_name['Update']._options = None
-  _ENDPOINTSERVICE.methods_by_name['Update']._serialized_options = b'\202\323\344\223\002\037:\001*2\032/v1/endpoint/{endpoint_id}'
+  _ENDPOINTSERVICE.methods_by_name['Update']._serialized_options = b'\202\323\344\223\002\0372\032/v1/endpoint/{endpoint_id}:\001*'
   _ENDPOINTSERVICE.methods_by_name['Delete']._options = None
   _ENDPOINTSERVICE.methods_by_name['Delete']._serialized_options = b'\202\323\344\223\002\034*\032/v1/endpoint/{endpoint_id}'
   _globals['_GETENDPOINTREQUEST']._serialized_start=240
   _globals['_GETENDPOINTREQUEST']._serialized_end=293
   _globals['_LISTENDPOINTSREQUEST']._serialized_start=295
   _globals['_LISTENDPOINTSREQUEST']._serialized_end=392
   _globals['_LISTENDPOINTSRESPONSE']._serialized_start=395
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/endpoint_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/operation_service_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/operation_service_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/operation_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/doublecloud/transfer/v1/operation_service.proto\x12\x17\x64oublecloud.transfer.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x64oublecloud/v1/operation.proto\"8\n\x13GetOperationRequest\x12!\n\x0coperation_id\x18\x01 \x01(\tR\x0boperationId2\x88\x01\n\x10OperationService\x12t\n\x03Get\x12,.doublecloud.transfer.v1.GetOperationRequest\x1a\x19.doublecloud.v1.Operation\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/operation/{operation_id}B=Z;github.com/doublecloud/api/doublecloud/transfer/v1;transferb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/doublecloud/transfer/v1/operation_service.proto\x12\x17\x64oublecloud.transfer.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x1e\x64oublecloud/v1/operation.proto\"8\n\x13GetOperationRequest\x12!\n\x0coperation_id\x18\x01 \x01(\tR\x0boperationId2\x88\x01\n\x10OperationService\x12t\n\x03Get\x12,.doublecloud.transfer.v1.GetOperationRequest\x1a\x19.doublecloud.v1.Operation\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/operation/{operation_id}BEZCgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1;transferb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.operation_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z;github.com/doublecloud/api/doublecloud/transfer/v1;transfer'
+  DESCRIPTOR._serialized_options = b'ZCgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1;transfer'
   _OPERATIONSERVICE.methods_by_name['Get']._options = None
   _OPERATIONSERVICE.methods_by_name['Get']._serialized_options = b'\202\323\344\223\002\036\022\034/v1/operation/{operation_id}'
   _globals['_GETOPERATIONREQUEST']._serialized_start=138
   _globals['_GETOPERATIONREQUEST']._serialized_end=194
   _globals['_OPERATIONSERVICE']._serialized_start=197
   _globals['_OPERATIONSERVICE']._serialized_end=333
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/operation_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/operation_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/operation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/transfer_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/transfer_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/transfer.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from doublecloud.transfer.v1 import endpoint_pb2 as doublecloud_dot_transfer_dot_v1_dot_endpoint__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&doublecloud/transfer/v1/transfer.proto\x12\x17\x64oublecloud.transfer.v1\x1a&doublecloud/transfer/v1/endpoint.proto\"\xfd\x03\n\x08Transfer\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x45\n\x06labels\x18\x06 \x03(\x0b\x32-.doublecloud.transfer.v1.Transfer.LabelsEntryR\x06labels\x12\x39\n\x06source\x18\x07 \x01(\x0b\x32!.doublecloud.transfer.v1.EndpointR\x06source\x12\x39\n\x06target\x18\x08 \x01(\x0b\x32!.doublecloud.transfer.v1.EndpointR\x06target\x12?\n\x06status\x18\n \x01(\x0e\x32\'.doublecloud.transfer.v1.TransferStatusR\x06status\x12\x39\n\x04type\x18\x0c \x01(\x0e\x32%.doublecloud.transfer.v1.TransferTypeR\x04type\x12\x18\n\x07warning\x18\x0f \x01(\tR\x07warning\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01*p\n\x0cTransferType\x12\x1d\n\x19TRANSFER_TYPE_UNSPECIFIED\x10\x00\x12\x1a\n\x16SNAPSHOT_AND_INCREMENT\x10\x01\x12\x11\n\rSNAPSHOT_ONLY\x10\x02\x12\x12\n\x0eINCREMENT_ONLY\x10\x03*\x9b\x01\n\x0eTransferStatus\x12\x1f\n\x1bTRANSFER_STATUS_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x43REATING\x10\x01\x12\x0b\n\x07\x43REATED\x10\x02\x12\x0b\n\x07RUNNING\x10\x03\x12\x0c\n\x08STOPPING\x10\x04\x12\x0b\n\x07STOPPED\x10\x05\x12\t\n\x05\x45RROR\x10\x06\x12\x10\n\x0cSNAPSHOTTING\x10\x07\x12\x08\n\x04\x44ONE\x10\x08\x42=Z;github.com/doublecloud/api/doublecloud/transfer/v1;transferb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&doublecloud/transfer/v1/transfer.proto\x12\x17\x64oublecloud.transfer.v1\x1a&doublecloud/transfer/v1/endpoint.proto\"\xfd\x03\n\x08Transfer\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x45\n\x06labels\x18\x06 \x03(\x0b\x32-.doublecloud.transfer.v1.Transfer.LabelsEntryR\x06labels\x12\x39\n\x06source\x18\x07 \x01(\x0b\x32!.doublecloud.transfer.v1.EndpointR\x06source\x12\x39\n\x06target\x18\x08 \x01(\x0b\x32!.doublecloud.transfer.v1.EndpointR\x06target\x12?\n\x06status\x18\n \x01(\x0e\x32\'.doublecloud.transfer.v1.TransferStatusR\x06status\x12\x39\n\x04type\x18\x0c \x01(\x0e\x32%.doublecloud.transfer.v1.TransferTypeR\x04type\x12\x18\n\x07warning\x18\x0f \x01(\tR\x07warning\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01*p\n\x0cTransferType\x12\x1d\n\x19TRANSFER_TYPE_UNSPECIFIED\x10\x00\x12\x1a\n\x16SNAPSHOT_AND_INCREMENT\x10\x01\x12\x11\n\rSNAPSHOT_ONLY\x10\x02\x12\x12\n\x0eINCREMENT_ONLY\x10\x03*\x9b\x01\n\x0eTransferStatus\x12\x1f\n\x1bTRANSFER_STATUS_UNSPECIFIED\x10\x00\x12\x0c\n\x08\x43REATING\x10\x01\x12\x0b\n\x07\x43REATED\x10\x02\x12\x0b\n\x07RUNNING\x10\x03\x12\x0c\n\x08STOPPING\x10\x04\x12\x0b\n\x07STOPPED\x10\x05\x12\t\n\x05\x45RROR\x10\x06\x12\x10\n\x0cSNAPSHOTTING\x10\x07\x12\x08\n\x04\x44ONE\x10\x08\x42\x45ZCgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1;transferb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.transfer_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z;github.com/doublecloud/api/doublecloud/transfer/v1;transfer'
+  DESCRIPTOR._serialized_options = b'ZCgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1;transfer'
   _TRANSFER_LABELSENTRY._options = None
   _TRANSFER_LABELSENTRY._serialized_options = b'8\001'
   _globals['_TRANSFERTYPE']._serialized_start=619
   _globals['_TRANSFERTYPE']._serialized_end=731
   _globals['_TRANSFERSTATUS']._serialized_start=734
   _globals['_TRANSFERSTATUS']._serialized_end=889
   _globals['_TRANSFER']._serialized_start=108
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/transfer_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/transfer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/transfer_service_pb2.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/transfer_service_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,60 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/transfer/v1/transfer_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from doublecloud.transfer.v1 import transfer_pb2 as doublecloud_dot_transfer_dot_v1_dot_transfer__pb2
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.v1 import paging_pb2 as doublecloud_dot_v1_dot_paging__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.doublecloud/transfer/v1/transfer_service.proto\x12\x17\x64oublecloud.transfer.v1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a&doublecloud/transfer/v1/transfer.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"\xf0\x02\n\x15\x43reateTransferRequest\x12\x1b\n\tsource_id\x18\x01 \x01(\tR\x08sourceId\x12\x1b\n\ttarget_id\x18\x02 \x01(\tR\x08targetId\x12\x12\n\x04name\x18\x07 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12R\n\x06labels\x18\x08 \x03(\x0b\x32:.doublecloud.transfer.v1.CreateTransferRequest.LabelsEntryR\x06labels\x12\x1d\n\nproject_id\x18\x04 \x01(\tR\tprojectId\x12\x39\n\x04type\x18\x06 \x01(\x0e\x32%.doublecloud.transfer.v1.TransferTypeR\x04type\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xfd\x01\n\x15UpdateTransferRequest\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12R\n\x06labels\x18\x06 \x03(\x0b\x32:.doublecloud.transfer.v1.UpdateTransferRequest.LabelsEntryR\x06labels\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"8\n\x15\x44\x65leteTransferRequest\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId\"a\n\x14ListTransfersRequest\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12*\n\x04page\x18\x03 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x04page\"\x80\x01\n\x15ListTransfersResponse\x12?\n\ttransfers\x18\x01 \x03(\x0b\x32!.doublecloud.transfer.v1.TransferR\ttransfers\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken\"5\n\x12GetTransferRequest\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId\"<\n\x19\x44\x65\x61\x63tivateTransferRequest\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId\":\n\x17\x41\x63tivateTransferRequest\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId2\x9a\x07\n\x0fTransferService\x12l\n\x06\x43reate\x12..doublecloud.transfer.v1.CreateTransferRequest\x1a\x19.doublecloud.v1.Operation\"\x17\x82\xd3\xe4\x93\x02\x11:\x01*\"\x0c/v1/transfer\x12z\n\x06Update\x12..doublecloud.transfer.v1.UpdateTransferRequest\x1a\x19.doublecloud.v1.Operation\"%\x82\xd3\xe4\x93\x02\x1f:\x01*2\x1a/v1/transfer/{transfer_id}\x12w\n\x06\x44\x65lete\x12..doublecloud.transfer.v1.DeleteTransferRequest\x1a\x19.doublecloud.v1.Operation\"\"\x82\xd3\xe4\x93\x02\x1c*\x1a/v1/transfer/{transfer_id}\x12\x8e\x01\n\x04List\x12-.doublecloud.transfer.v1.ListTransfersRequest\x1a..doublecloud.transfer.v1.ListTransfersResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/v1/transfers/list/{project_id}\x12y\n\x03Get\x12+.doublecloud.transfer.v1.GetTransferRequest\x1a!.doublecloud.transfer.v1.Transfer\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/v1/transfer/{transfer_id}\x12\x8d\x01\n\nDeactivate\x12\x32.doublecloud.transfer.v1.DeactivateTransferRequest\x1a\x19.doublecloud.v1.Operation\"0\x82\xd3\xe4\x93\x02*:\x01*\"%/v1/transfer/{transfer_id}:deactivate\x12\x87\x01\n\x08\x41\x63tivate\x12\x30.doublecloud.transfer.v1.ActivateTransferRequest\x1a\x19.doublecloud.v1.Operation\".\x82\xd3\xe4\x93\x02(:\x01*\"#/v1/transfer/{transfer_id}:activateB=Z;github.com/doublecloud/api/doublecloud/transfer/v1;transferb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.doublecloud/transfer/v1/transfer_service.proto\x12\x17\x64oublecloud.transfer.v1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a&doublecloud/transfer/v1/transfer.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a\x1b\x64oublecloud/v1/paging.proto\"\xf0\x02\n\x15\x43reateTransferRequest\x12\x1b\n\tsource_id\x18\x01 \x01(\tR\x08sourceId\x12\x1b\n\ttarget_id\x18\x02 \x01(\tR\x08targetId\x12\x12\n\x04name\x18\x07 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12R\n\x06labels\x18\x08 \x03(\x0b\x32:.doublecloud.transfer.v1.CreateTransferRequest.LabelsEntryR\x06labels\x12\x1d\n\nproject_id\x18\x04 \x01(\tR\tprojectId\x12\x39\n\x04type\x18\x06 \x01(\x0e\x32%.doublecloud.transfer.v1.TransferTypeR\x04type\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xfd\x01\n\x15UpdateTransferRequest\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12R\n\x06labels\x18\x06 \x03(\x0b\x32:.doublecloud.transfer.v1.UpdateTransferRequest.LabelsEntryR\x06labels\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x1a\x39\n\x0bLabelsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"8\n\x15\x44\x65leteTransferRequest\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId\"a\n\x14ListTransfersRequest\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12*\n\x04page\x18\x03 \x01(\x0b\x32\x16.doublecloud.v1.PagingR\x04page\"\x80\x01\n\x15ListTransfersResponse\x12?\n\ttransfers\x18\x01 \x03(\x0b\x32!.doublecloud.transfer.v1.TransferR\ttransfers\x12&\n\x0fnext_page_token\x18\x02 \x01(\tR\rnextPageToken\"5\n\x12GetTransferRequest\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId\"<\n\x19\x44\x65\x61\x63tivateTransferRequest\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId\":\n\x17\x41\x63tivateTransferRequest\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId\"4\n\x11GetMetricsRequest\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId\"\xa4\x01\n\x0fTransferMetrics\x12I\n\x07metrics\x18\x01 \x03(\x0b\x32/.doublecloud.transfer.v1.TransferMetrics.MetricR\x07metrics\x1a\x46\n\x06Metric\x12\x12\n\x04help\x18\x01 \x01(\tR\x04help\x12\x12\n\x04type\x18\x02 \x01(\tR\x04type\x12\x14\n\x05value\x18\x03 \x01(\tR\x05value\"F\n#MetricExporterConnectionInfoRequest\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId\"\x83\x01\n$MetricExporterConnectionInfoMetadata\x12+\n\x11\x63onnection_string\x18\x01 \x01(\tR\x10\x63onnectionString\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\"F\n#DeleteExporterConnectionInfoRequest\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId\"G\n$DeleteExporterConnectionInfoMetadata\x12\x1f\n\x0btransfer_id\x18\x01 \x01(\tR\ntransferId2\xa6\x0b\n\x0fTransferService\x12l\n\x06\x43reate\x12..doublecloud.transfer.v1.CreateTransferRequest\x1a\x19.doublecloud.v1.Operation\"\x17\x82\xd3\xe4\x93\x02\x11\"\x0c/v1/transfer:\x01*\x12z\n\x06Update\x12..doublecloud.transfer.v1.UpdateTransferRequest\x1a\x19.doublecloud.v1.Operation\"%\x82\xd3\xe4\x93\x02\x1f\x32\x1a/v1/transfer/{transfer_id}:\x01*\x12w\n\x06\x44\x65lete\x12..doublecloud.transfer.v1.DeleteTransferRequest\x1a\x19.doublecloud.v1.Operation\"\"\x82\xd3\xe4\x93\x02\x1c*\x1a/v1/transfer/{transfer_id}\x12\x8e\x01\n\x04List\x12-.doublecloud.transfer.v1.ListTransfersRequest\x1a..doublecloud.transfer.v1.ListTransfersResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/v1/transfers/list/{project_id}\x12y\n\x03Get\x12+.doublecloud.transfer.v1.GetTransferRequest\x1a!.doublecloud.transfer.v1.Transfer\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/v1/transfer/{transfer_id}\x12\x8d\x01\n\nDeactivate\x12\x32.doublecloud.transfer.v1.DeactivateTransferRequest\x1a\x19.doublecloud.v1.Operation\"0\x82\xd3\xe4\x93\x02*\"%/v1/transfer/{transfer_id}:deactivate:\x01*\x12\x87\x01\n\x08\x41\x63tivate\x12\x30.doublecloud.transfer.v1.ActivateTransferRequest\x1a\x19.doublecloud.v1.Operation\".\x82\xd3\xe4\x93\x02(\"#/v1/transfer/{transfer_id}:activate:\x01*\x12\x8e\x01\n\nGetMetrics\x12*.doublecloud.transfer.v1.GetMetricsRequest\x1a(.doublecloud.transfer.v1.TransferMetrics\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/transfer/{transfer_id}/metrics\x12\xcb\x01\n\x1fGetMetricExporterConnectionInfo\x12<.doublecloud.transfer.v1.MetricExporterConnectionInfoRequest\x1a=.doublecloud.transfer.v1.MetricExporterConnectionInfoMetadata\"+\x82\xd3\xe4\x93\x02%\x12#/v1/transfer/{transfer_id}/exporter\x12\xaa\x01\n\"DeleteMetricExporterConnectionInfo\x12<.doublecloud.transfer.v1.DeleteExporterConnectionInfoRequest\x1a\x19.doublecloud.v1.Operation\"+\x82\xd3\xe4\x93\x02%*#/v1/transfer/{transfer_id}/exporterBEZCgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1;transferb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.transfer.v1.transfer_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z;github.com/doublecloud/api/doublecloud/transfer/v1;transfer'
+  DESCRIPTOR._serialized_options = b'ZCgithub.com/doublecloud/go-genproto/doublecloud/transfer/v1;transfer'
   _CREATETRANSFERREQUEST_LABELSENTRY._options = None
   _CREATETRANSFERREQUEST_LABELSENTRY._serialized_options = b'8\001'
   _UPDATETRANSFERREQUEST_LABELSENTRY._options = None
   _UPDATETRANSFERREQUEST_LABELSENTRY._serialized_options = b'8\001'
   _TRANSFERSERVICE.methods_by_name['Create']._options = None
-  _TRANSFERSERVICE.methods_by_name['Create']._serialized_options = b'\202\323\344\223\002\021:\001*\"\014/v1/transfer'
+  _TRANSFERSERVICE.methods_by_name['Create']._serialized_options = b'\202\323\344\223\002\021\"\014/v1/transfer:\001*'
   _TRANSFERSERVICE.methods_by_name['Update']._options = None
-  _TRANSFERSERVICE.methods_by_name['Update']._serialized_options = b'\202\323\344\223\002\037:\001*2\032/v1/transfer/{transfer_id}'
+  _TRANSFERSERVICE.methods_by_name['Update']._serialized_options = b'\202\323\344\223\002\0372\032/v1/transfer/{transfer_id}:\001*'
   _TRANSFERSERVICE.methods_by_name['Delete']._options = None
   _TRANSFERSERVICE.methods_by_name['Delete']._serialized_options = b'\202\323\344\223\002\034*\032/v1/transfer/{transfer_id}'
   _TRANSFERSERVICE.methods_by_name['List']._options = None
   _TRANSFERSERVICE.methods_by_name['List']._serialized_options = b'\202\323\344\223\002!\022\037/v1/transfers/list/{project_id}'
   _TRANSFERSERVICE.methods_by_name['Get']._options = None
   _TRANSFERSERVICE.methods_by_name['Get']._serialized_options = b'\202\323\344\223\002\034\022\032/v1/transfer/{transfer_id}'
   _TRANSFERSERVICE.methods_by_name['Deactivate']._options = None
-  _TRANSFERSERVICE.methods_by_name['Deactivate']._serialized_options = b'\202\323\344\223\002*:\001*\"%/v1/transfer/{transfer_id}:deactivate'
+  _TRANSFERSERVICE.methods_by_name['Deactivate']._serialized_options = b'\202\323\344\223\002*\"%/v1/transfer/{transfer_id}:deactivate:\001*'
   _TRANSFERSERVICE.methods_by_name['Activate']._options = None
-  _TRANSFERSERVICE.methods_by_name['Activate']._serialized_options = b'\202\323\344\223\002(:\001*\"#/v1/transfer/{transfer_id}:activate'
+  _TRANSFERSERVICE.methods_by_name['Activate']._serialized_options = b'\202\323\344\223\002(\"#/v1/transfer/{transfer_id}:activate:\001*'
+  _TRANSFERSERVICE.methods_by_name['GetMetrics']._options = None
+  _TRANSFERSERVICE.methods_by_name['GetMetrics']._serialized_options = b'\202\323\344\223\002$\022\"/v1/transfer/{transfer_id}/metrics'
+  _TRANSFERSERVICE.methods_by_name['GetMetricExporterConnectionInfo']._options = None
+  _TRANSFERSERVICE.methods_by_name['GetMetricExporterConnectionInfo']._serialized_options = b'\202\323\344\223\002%\022#/v1/transfer/{transfer_id}/exporter'
+  _TRANSFERSERVICE.methods_by_name['DeleteMetricExporterConnectionInfo']._options = None
+  _TRANSFERSERVICE.methods_by_name['DeleteMetricExporterConnectionInfo']._serialized_options = b'\202\323\344\223\002%*#/v1/transfer/{transfer_id}/exporter'
   _globals['_CREATETRANSFERREQUEST']._serialized_start=241
   _globals['_CREATETRANSFERREQUEST']._serialized_end=609
   _globals['_CREATETRANSFERREQUEST_LABELSENTRY']._serialized_start=552
   _globals['_CREATETRANSFERREQUEST_LABELSENTRY']._serialized_end=609
   _globals['_UPDATETRANSFERREQUEST']._serialized_start=612
   _globals['_UPDATETRANSFERREQUEST']._serialized_end=865
   _globals['_UPDATETRANSFERREQUEST_LABELSENTRY']._serialized_start=552
@@ -61,10 +67,24 @@
   _globals['_LISTTRANSFERSRESPONSE']._serialized_end=1153
   _globals['_GETTRANSFERREQUEST']._serialized_start=1155
   _globals['_GETTRANSFERREQUEST']._serialized_end=1208
   _globals['_DEACTIVATETRANSFERREQUEST']._serialized_start=1210
   _globals['_DEACTIVATETRANSFERREQUEST']._serialized_end=1270
   _globals['_ACTIVATETRANSFERREQUEST']._serialized_start=1272
   _globals['_ACTIVATETRANSFERREQUEST']._serialized_end=1330
-  _globals['_TRANSFERSERVICE']._serialized_start=1333
-  _globals['_TRANSFERSERVICE']._serialized_end=2255
+  _globals['_GETMETRICSREQUEST']._serialized_start=1332
+  _globals['_GETMETRICSREQUEST']._serialized_end=1384
+  _globals['_TRANSFERMETRICS']._serialized_start=1387
+  _globals['_TRANSFERMETRICS']._serialized_end=1551
+  _globals['_TRANSFERMETRICS_METRIC']._serialized_start=1481
+  _globals['_TRANSFERMETRICS_METRIC']._serialized_end=1551
+  _globals['_METRICEXPORTERCONNECTIONINFOREQUEST']._serialized_start=1553
+  _globals['_METRICEXPORTERCONNECTIONINFOREQUEST']._serialized_end=1623
+  _globals['_METRICEXPORTERCONNECTIONINFOMETADATA']._serialized_start=1626
+  _globals['_METRICEXPORTERCONNECTIONINFOMETADATA']._serialized_end=1757
+  _globals['_DELETEEXPORTERCONNECTIONINFOREQUEST']._serialized_start=1759
+  _globals['_DELETEEXPORTERCONNECTIONINFOREQUEST']._serialized_end=1829
+  _globals['_DELETEEXPORTERCONNECTIONINFOMETADATA']._serialized_start=1831
+  _globals['_DELETEEXPORTERCONNECTIONINFOMETADATA']._serialized_end=1902
+  _globals['_TRANSFERSERVICE']._serialized_start=1905
+  _globals['_TRANSFERSERVICE']._serialized_end=3351
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/transfer_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/transfer/v1/transfer_service_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -89,7 +89,56 @@
     def __init__(self, transfer_id: _Optional[str] = ...) -> None: ...
 
 class ActivateTransferRequest(_message.Message):
     __slots__ = ["transfer_id"]
     TRANSFER_ID_FIELD_NUMBER: _ClassVar[int]
     transfer_id: str
     def __init__(self, transfer_id: _Optional[str] = ...) -> None: ...
+
+class GetMetricsRequest(_message.Message):
+    __slots__ = ["transfer_id"]
+    TRANSFER_ID_FIELD_NUMBER: _ClassVar[int]
+    transfer_id: str
+    def __init__(self, transfer_id: _Optional[str] = ...) -> None: ...
+
+class TransferMetrics(_message.Message):
+    __slots__ = ["metrics"]
+    class Metric(_message.Message):
+        __slots__ = ["help", "type", "value"]
+        HELP_FIELD_NUMBER: _ClassVar[int]
+        TYPE_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        help: str
+        type: str
+        value: str
+        def __init__(self, help: _Optional[str] = ..., type: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    METRICS_FIELD_NUMBER: _ClassVar[int]
+    metrics: _containers.RepeatedCompositeFieldContainer[TransferMetrics.Metric]
+    def __init__(self, metrics: _Optional[_Iterable[_Union[TransferMetrics.Metric, _Mapping]]] = ...) -> None: ...
+
+class MetricExporterConnectionInfoRequest(_message.Message):
+    __slots__ = ["transfer_id"]
+    TRANSFER_ID_FIELD_NUMBER: _ClassVar[int]
+    transfer_id: str
+    def __init__(self, transfer_id: _Optional[str] = ...) -> None: ...
+
+class MetricExporterConnectionInfoMetadata(_message.Message):
+    __slots__ = ["connection_string", "user", "password"]
+    CONNECTION_STRING_FIELD_NUMBER: _ClassVar[int]
+    USER_FIELD_NUMBER: _ClassVar[int]
+    PASSWORD_FIELD_NUMBER: _ClassVar[int]
+    connection_string: str
+    user: str
+    password: str
+    def __init__(self, connection_string: _Optional[str] = ..., user: _Optional[str] = ..., password: _Optional[str] = ...) -> None: ...
+
+class DeleteExporterConnectionInfoRequest(_message.Message):
+    __slots__ = ["transfer_id"]
+    TRANSFER_ID_FIELD_NUMBER: _ClassVar[int]
+    transfer_id: str
+    def __init__(self, transfer_id: _Optional[str] = ...) -> None: ...
+
+class DeleteExporterConnectionInfoMetadata(_message.Message):
+    __slots__ = ["transfer_id"]
+    TRANSFER_ID_FIELD_NUMBER: _ClassVar[int]
+    transfer_id: str
+    def __init__(self, transfer_id: _Optional[str] = ...) -> None: ...
```

### Comparing `doublecloud-0.5.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/transfer/v1/transfer_service_pb2_grpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,14 +47,29 @@
                 response_deserializer=doublecloud_dot_v1_dot_operation__pb2.Operation.FromString,
                 )
         self.Activate = channel.unary_unary(
                 '/doublecloud.transfer.v1.TransferService/Activate',
                 request_serializer=doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.ActivateTransferRequest.SerializeToString,
                 response_deserializer=doublecloud_dot_v1_dot_operation__pb2.Operation.FromString,
                 )
+        self.GetMetrics = channel.unary_unary(
+                '/doublecloud.transfer.v1.TransferService/GetMetrics',
+                request_serializer=doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.GetMetricsRequest.SerializeToString,
+                response_deserializer=doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.TransferMetrics.FromString,
+                )
+        self.GetMetricExporterConnectionInfo = channel.unary_unary(
+                '/doublecloud.transfer.v1.TransferService/GetMetricExporterConnectionInfo',
+                request_serializer=doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.MetricExporterConnectionInfoRequest.SerializeToString,
+                response_deserializer=doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.MetricExporterConnectionInfoMetadata.FromString,
+                )
+        self.DeleteMetricExporterConnectionInfo = channel.unary_unary(
+                '/doublecloud.transfer.v1.TransferService/DeleteMetricExporterConnectionInfo',
+                request_serializer=doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.DeleteExporterConnectionInfoRequest.SerializeToString,
+                response_deserializer=doublecloud_dot_v1_dot_operation__pb2.Operation.FromString,
+                )
 
 
 class TransferServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Create(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -94,14 +109,33 @@
 
     def Activate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetMetrics(self, request, context):
+        """Allows scraping of metrics by a prometheus scraper
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetMetricExporterConnectionInfo(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DeleteMetricExporterConnectionInfo(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_TransferServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Create': grpc.unary_unary_rpc_method_handler(
                     servicer.Create,
                     request_deserializer=doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.CreateTransferRequest.FromString,
                     response_serializer=doublecloud_dot_v1_dot_operation__pb2.Operation.SerializeToString,
@@ -132,14 +166,29 @@
                     response_serializer=doublecloud_dot_v1_dot_operation__pb2.Operation.SerializeToString,
             ),
             'Activate': grpc.unary_unary_rpc_method_handler(
                     servicer.Activate,
                     request_deserializer=doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.ActivateTransferRequest.FromString,
                     response_serializer=doublecloud_dot_v1_dot_operation__pb2.Operation.SerializeToString,
             ),
+            'GetMetrics': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetMetrics,
+                    request_deserializer=doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.GetMetricsRequest.FromString,
+                    response_serializer=doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.TransferMetrics.SerializeToString,
+            ),
+            'GetMetricExporterConnectionInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetMetricExporterConnectionInfo,
+                    request_deserializer=doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.MetricExporterConnectionInfoRequest.FromString,
+                    response_serializer=doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.MetricExporterConnectionInfoMetadata.SerializeToString,
+            ),
+            'DeleteMetricExporterConnectionInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteMetricExporterConnectionInfo,
+                    request_deserializer=doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.DeleteExporterConnectionInfoRequest.FromString,
+                    response_serializer=doublecloud_dot_v1_dot_operation__pb2.Operation.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'doublecloud.transfer.v1.TransferService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -260,7 +309,58 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/doublecloud.transfer.v1.TransferService/Activate',
             doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.ActivateTransferRequest.SerializeToString,
             doublecloud_dot_v1_dot_operation__pb2.Operation.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetMetrics(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/doublecloud.transfer.v1.TransferService/GetMetrics',
+            doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.GetMetricsRequest.SerializeToString,
+            doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.TransferMetrics.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetMetricExporterConnectionInfo(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/doublecloud.transfer.v1.TransferService/GetMetricExporterConnectionInfo',
+            doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.MetricExporterConnectionInfoRequest.SerializeToString,
+            doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.MetricExporterConnectionInfoMetadata.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteMetricExporterConnectionInfo(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/doublecloud.transfer.v1.TransferService/DeleteMetricExporterConnectionInfo',
+            doublecloud_dot_transfer_dot_v1_dot_transfer__service__pb2.DeleteExporterConnectionInfoRequest.SerializeToString,
+            doublecloud_dot_v1_dot_operation__pb2.Operation.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `doublecloud-0.5.0/doublecloud/v1/cluster_pb2.py` & `doublecloud-0.6.0/doublecloud/v1/cluster_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/v1/cluster.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x64oublecloud/v1/cluster.proto\x12\x0e\x64oublecloud.v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xb8\x04\n\x06\x41\x63\x63\x65ss\x12N\n\x10ipv4_cidr_blocks\x18\x01 \x01(\x0b\x32$.doublecloud.v1.Access.CidrBlockListR\x0eipv4CidrBlocks\x12N\n\x10ipv6_cidr_blocks\x18\x02 \x01(\x0b\x32$.doublecloud.v1.Access.CidrBlockListR\x0eipv6CidrBlocks\x12K\n\rdata_services\x18\x03 \x01(\x0b\x32&.doublecloud.v1.Access.DataServiceListR\x0c\x64\x61taServices\x1a\x43\n\tCidrBlock\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x1aI\n\rCidrBlockList\x12\x38\n\x06values\x18\x01 \x03(\x0b\x32 .doublecloud.v1.Access.CidrBlockR\x06values\x1aM\n\x0f\x44\x61taServiceList\x12:\n\x06values\x18\x01 \x03(\x0e\x32\".doublecloud.v1.Access.DataServiceR\x06values\"b\n\x0b\x44\x61taService\x12\x18\n\x14\x44\x41TA_SERVICE_INVALID\x10\x00\x12\x1e\n\x1a\x44\x41TA_SERVICE_VISUALIZATION\x10\x01\x12\x19\n\x15\x44\x41TA_SERVICE_TRANSFER\x10\x02\"F\n\x0e\x44\x61taEncryption\x12\x34\n\x07\x65nabled\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x07\x65nabled*\xc1\x02\n\rClusterStatus\x12\x1a\n\x16\x43LUSTER_STATUS_INVALID\x10\x00\x12\x18\n\x14\x43LUSTER_STATUS_ALIVE\x10\x01\x12\x1b\n\x17\x43LUSTER_STATUS_DEGRADED\x10\x02\x12\x17\n\x13\x43LUSTER_STATUS_DEAD\x10\x03\x12\x1a\n\x16\x43LUSTER_STATUS_UNKNOWN\x10\x04\x12\x1b\n\x17\x43LUSTER_STATUS_CREATING\x10\x05\x12\x1b\n\x17\x43LUSTER_STATUS_UPDATING\x10\x06\x12\x1b\n\x17\x43LUSTER_STATUS_STOPPING\x10\x07\x12\x1a\n\x16\x43LUSTER_STATUS_STOPPED\x10\x08\x12\x1b\n\x17\x43LUSTER_STATUS_STARTING\x10\t\x12\x18\n\x14\x43LUSTER_STATUS_ERROR\x10\n*l\n\nHostStatus\x12\x17\n\x13HOST_STATUS_INVALID\x10\x00\x12\x15\n\x11HOST_STATUS_ALIVE\x10\x01\x12\x14\n\x10HOST_STATUS_DEAD\x10\x02\x12\x18\n\x14HOST_STATUS_DEGRADED\x10\x03\x42\x37Z5github.com/doublecloud/api/doublecloud/v1;doublecloudb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x64oublecloud/v1/cluster.proto\x12\x0e\x64oublecloud.v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xb8\x04\n\x06\x41\x63\x63\x65ss\x12N\n\x10ipv4_cidr_blocks\x18\x01 \x01(\x0b\x32$.doublecloud.v1.Access.CidrBlockListR\x0eipv4CidrBlocks\x12N\n\x10ipv6_cidr_blocks\x18\x02 \x01(\x0b\x32$.doublecloud.v1.Access.CidrBlockListR\x0eipv6CidrBlocks\x12K\n\rdata_services\x18\x03 \x01(\x0b\x32&.doublecloud.v1.Access.DataServiceListR\x0c\x64\x61taServices\x1a\x43\n\tCidrBlock\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x1aI\n\rCidrBlockList\x12\x38\n\x06values\x18\x01 \x03(\x0b\x32 .doublecloud.v1.Access.CidrBlockR\x06values\x1aM\n\x0f\x44\x61taServiceList\x12:\n\x06values\x18\x01 \x03(\x0e\x32\".doublecloud.v1.Access.DataServiceR\x06values\"b\n\x0b\x44\x61taService\x12\x18\n\x14\x44\x41TA_SERVICE_INVALID\x10\x00\x12\x1e\n\x1a\x44\x41TA_SERVICE_VISUALIZATION\x10\x01\x12\x19\n\x15\x44\x41TA_SERVICE_TRANSFER\x10\x02\"F\n\x0e\x44\x61taEncryption\x12\x34\n\x07\x65nabled\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x07\x65nabled*\xc1\x02\n\rClusterStatus\x12\x1a\n\x16\x43LUSTER_STATUS_INVALID\x10\x00\x12\x18\n\x14\x43LUSTER_STATUS_ALIVE\x10\x01\x12\x1b\n\x17\x43LUSTER_STATUS_DEGRADED\x10\x02\x12\x17\n\x13\x43LUSTER_STATUS_DEAD\x10\x03\x12\x1a\n\x16\x43LUSTER_STATUS_UNKNOWN\x10\x04\x12\x1b\n\x17\x43LUSTER_STATUS_CREATING\x10\x05\x12\x1b\n\x17\x43LUSTER_STATUS_UPDATING\x10\x06\x12\x1b\n\x17\x43LUSTER_STATUS_STOPPING\x10\x07\x12\x1a\n\x16\x43LUSTER_STATUS_STOPPED\x10\x08\x12\x1b\n\x17\x43LUSTER_STATUS_STARTING\x10\t\x12\x18\n\x14\x43LUSTER_STATUS_ERROR\x10\n*l\n\nHostStatus\x12\x17\n\x13HOST_STATUS_INVALID\x10\x00\x12\x15\n\x11HOST_STATUS_ALIVE\x10\x01\x12\x14\n\x10HOST_STATUS_DEAD\x10\x02\x12\x18\n\x14HOST_STATUS_DEGRADED\x10\x03\x42?Z=github.com/doublecloud/go-genproto/doublecloud/v1;doublecloudb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.v1.cluster_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/v1;doublecloud'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/v1;doublecloud'
   _globals['_CLUSTERSTATUS']._serialized_start=724
   _globals['_CLUSTERSTATUS']._serialized_end=1045
   _globals['_HOSTSTATUS']._serialized_start=1047
   _globals['_HOSTSTATUS']._serialized_end=1155
   _globals['_ACCESS']._serialized_start=81
   _globals['_ACCESS']._serialized_end=649
   _globals['_ACCESS_CIDRBLOCK']._serialized_start=328
```

### Comparing `doublecloud-0.5.0/doublecloud/v1/cluster_pb2.pyi` & `doublecloud-0.6.0/doublecloud/v1/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/v1/maintenance_pb2.py` & `doublecloud-0.6.0/doublecloud/v1/maintenance_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/v1/maintenance.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.type import dayofweek_pb2 as google_dot_type_dot_dayofweek__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n doublecloud/v1/maintenance.proto\x12\x0e\x64oublecloud.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/type/dayofweek.proto\"\xca\x01\n\x11MaintenanceWindow\x12\x44\n\x07\x61nytime\x18\x01 \x01(\x0b\x32(.doublecloud.v1.AnytimeMaintenanceWindowH\x00R\x07\x61nytime\x12\x65\n\x19weekly_maintenance_window\x18\x02 \x01(\x0b\x32\'.doublecloud.v1.WeeklyMaintenanceWindowH\x00R\x17weeklyMaintenanceWindowB\x08\n\x06policy\"\x1a\n\x18\x41nytimeMaintenanceWindow\"W\n\x17WeeklyMaintenanceWindow\x12(\n\x03\x64\x61y\x18\x01 \x01(\x0e\x32\x16.google.type.DayOfWeekR\x03\x64\x61y\x12\x12\n\x04hour\x18\x02 \x01(\x03R\x04hour\"\xb9\x02\n\x14MaintenanceOperation\x12\x12\n\x04info\x18\x01 \x01(\tR\x04info\x12X\n\x1ascheduled_maintenance_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x18scheduledMaintenanceTime\x12V\n\x19\x64\x65\x61\x64line_maintenance_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x17\x64\x65\x61\x64lineMaintenanceTime\x12[\n\x1cnext_maintenance_window_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x19nextMaintenanceWindowTime*\x9a\x01\n\x0eRescheduleType\x12\x1b\n\x17RESCHEDULE_TYPE_INVALID\x10\x00\x12\x1d\n\x19RESCHEDULE_TYPE_IMMEDIATE\x10\x01\x12)\n%RESCHEDULE_TYPE_NEXT_AVAILABLE_WINDOW\x10\x02\x12!\n\x1dRESCHEDULE_TYPE_SPECIFIC_TIME\x10\x03\x42\x37Z5github.com/doublecloud/api/doublecloud/v1;doublecloudb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n doublecloud/v1/maintenance.proto\x12\x0e\x64oublecloud.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/type/dayofweek.proto\"\xca\x01\n\x11MaintenanceWindow\x12\x44\n\x07\x61nytime\x18\x01 \x01(\x0b\x32(.doublecloud.v1.AnytimeMaintenanceWindowH\x00R\x07\x61nytime\x12\x65\n\x19weekly_maintenance_window\x18\x02 \x01(\x0b\x32\'.doublecloud.v1.WeeklyMaintenanceWindowH\x00R\x17weeklyMaintenanceWindowB\x08\n\x06policy\"\x1a\n\x18\x41nytimeMaintenanceWindow\"W\n\x17WeeklyMaintenanceWindow\x12(\n\x03\x64\x61y\x18\x01 \x01(\x0e\x32\x16.google.type.DayOfWeekR\x03\x64\x61y\x12\x12\n\x04hour\x18\x02 \x01(\x03R\x04hour\"\xb9\x02\n\x14MaintenanceOperation\x12\x12\n\x04info\x18\x01 \x01(\tR\x04info\x12X\n\x1ascheduled_maintenance_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x18scheduledMaintenanceTime\x12V\n\x19\x64\x65\x61\x64line_maintenance_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x17\x64\x65\x61\x64lineMaintenanceTime\x12[\n\x1cnext_maintenance_window_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x19nextMaintenanceWindowTime*\x9a\x01\n\x0eRescheduleType\x12\x1b\n\x17RESCHEDULE_TYPE_INVALID\x10\x00\x12\x1d\n\x19RESCHEDULE_TYPE_IMMEDIATE\x10\x01\x12)\n%RESCHEDULE_TYPE_NEXT_AVAILABLE_WINDOW\x10\x02\x12!\n\x1dRESCHEDULE_TYPE_SPECIFIC_TIME\x10\x03\x42?Z=github.com/doublecloud/go-genproto/doublecloud/v1;doublecloudb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.v1.maintenance_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/v1;doublecloud'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/v1;doublecloud'
   _globals['_RESCHEDULETYPE']._serialized_start=753
   _globals['_RESCHEDULETYPE']._serialized_end=907
   _globals['_MAINTENANCEWINDOW']._serialized_start=115
   _globals['_MAINTENANCEWINDOW']._serialized_end=317
   _globals['_ANYTIMEMAINTENANCEWINDOW']._serialized_start=319
   _globals['_ANYTIMEMAINTENANCEWINDOW']._serialized_end=345
   _globals['_WEEKLYMAINTENANCEWINDOW']._serialized_start=347
```

### Comparing `doublecloud-0.5.0/doublecloud/v1/maintenance_pb2.pyi` & `doublecloud-0.6.0/doublecloud/v1/maintenance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/v1/operation_pb2.py` & `doublecloud-0.6.0/doublecloud/v1/operation_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/v1/operation.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.rpc import status_pb2 as google_dot_rpc_dot_status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x64oublecloud/v1/operation.proto\x12\x0e\x64oublecloud.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17google/rpc/status.proto\"\x8e\x05\n\tOperation\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1d\n\ncreated_by\x18\x04 \x01(\tR\tcreatedBy\x12\x43\n\x08metadata\x18\x05 \x03(\x0b\x32\'.doublecloud.v1.Operation.MetadataEntryR\x08metadata\x12;\n\x0b\x63reate_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x39\n\nstart_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12;\n\x0b\x66inish_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\nfinishTime\x12\x38\n\x06status\x18\t \x01(\x0e\x32 .doublecloud.v1.Operation.StatusR\x06status\x12(\n\x05\x65rror\x18\n \x01(\x0b\x32\x12.google.rpc.StatusR\x05\x65rror\x12\x1f\n\x0bresource_id\x18\x0b \x01(\tR\nresourceId\x1a;\n\rMetadataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"U\n\x06Status\x12\x12\n\x0eSTATUS_INVALID\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x12\n\x0eSTATUS_RUNNING\x10\x02\x12\x0f\n\x0bSTATUS_DONE\x10\x03\x42\x37Z5github.com/doublecloud/api/doublecloud/v1;doublecloudb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x64oublecloud/v1/operation.proto\x12\x0e\x64oublecloud.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17google/rpc/status.proto\"\x8e\x05\n\tOperation\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1d\n\ncreated_by\x18\x04 \x01(\tR\tcreatedBy\x12\x43\n\x08metadata\x18\x05 \x03(\x0b\x32\'.doublecloud.v1.Operation.MetadataEntryR\x08metadata\x12;\n\x0b\x63reate_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ncreateTime\x12\x39\n\nstart_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12;\n\x0b\x66inish_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\nfinishTime\x12\x38\n\x06status\x18\t \x01(\x0e\x32 .doublecloud.v1.Operation.StatusR\x06status\x12(\n\x05\x65rror\x18\n \x01(\x0b\x32\x12.google.rpc.StatusR\x05\x65rror\x12\x1f\n\x0bresource_id\x18\x0b \x01(\tR\nresourceId\x1a;\n\rMetadataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"U\n\x06Status\x12\x12\n\x0eSTATUS_INVALID\x10\x00\x12\x12\n\x0eSTATUS_PENDING\x10\x01\x12\x12\n\x0eSTATUS_RUNNING\x10\x02\x12\x0f\n\x0bSTATUS_DONE\x10\x03\x42?Z=github.com/doublecloud/go-genproto/doublecloud/v1;doublecloudb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.v1.operation_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/v1;doublecloud'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/v1;doublecloud'
   _OPERATION_METADATAENTRY._options = None
   _OPERATION_METADATAENTRY._serialized_options = b'8\001'
   _globals['_OPERATION']._serialized_start=109
   _globals['_OPERATION']._serialized_end=763
   _globals['_OPERATION_METADATAENTRY']._serialized_start=617
   _globals['_OPERATION_METADATAENTRY']._serialized_end=676
   _globals['_OPERATION_STATUS']._serialized_start=678
```

### Comparing `doublecloud-0.5.0/doublecloud/v1/operation_pb2.pyi` & `doublecloud-0.6.0/doublecloud/v1/operation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/v1/paging_pb2.py` & `doublecloud-0.6.0/doublecloud/v1/paging_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/v1/paging.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x64oublecloud/v1/paging.proto\x12\x0e\x64oublecloud.v1\"D\n\x06Paging\x12\x1b\n\tpage_size\x18\x01 \x01(\x03R\x08pageSize\x12\x1d\n\npage_token\x18\x02 \x01(\tR\tpageToken\" \n\x08NextPage\x12\x14\n\x05token\x18\x01 \x01(\tR\x05tokenB7Z5github.com/doublecloud/api/doublecloud/v1;doublecloudb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x64oublecloud/v1/paging.proto\x12\x0e\x64oublecloud.v1\"D\n\x06Paging\x12\x1b\n\tpage_size\x18\x01 \x01(\x03R\x08pageSize\x12\x1d\n\npage_token\x18\x02 \x01(\tR\tpageToken\" \n\x08NextPage\x12\x14\n\x05token\x18\x01 \x01(\tR\x05tokenB?Z=github.com/doublecloud/go-genproto/doublecloud/v1;doublecloudb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.v1.paging_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/doublecloud/api/doublecloud/v1;doublecloud'
+  DESCRIPTOR._serialized_options = b'Z=github.com/doublecloud/go-genproto/doublecloud/v1;doublecloud'
   _globals['_PAGING']._serialized_start=47
   _globals['_PAGING']._serialized_end=115
   _globals['_NEXTPAGE']._serialized_start=117
   _globals['_NEXTPAGE']._serialized_end=149
 # @@protoc_insertion_point(module_scope)
```

### Comparing `doublecloud-0.5.0/doublecloud/v1/paging_pb2.pyi` & `doublecloud-0.6.0/doublecloud/v1/paging_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/visualization/v1/workbook_pb2.py` & `doublecloud-0.6.0/doublecloud/visualization/v1/workbook_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/visualization/v1/workbook.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+doublecloud/visualization/v1/workbook.proto\x12\x1c\x64oublecloud.visualization.v1\x1a\x1cgoogle/protobuf/struct.proto\"%\n\x0bPlainSecret\x12\x16\n\x06secret\x18\x01 \x01(\tR\x06secret\"b\n\x06Secret\x12N\n\x0cplain_secret\x18\x01 \x01(\x0b\x32).doublecloud.visualization.v1.PlainSecretH\x00R\x0bplainSecretB\x08\n\x06secret\":\n\x08Workbook\x12.\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x06\x63onfig\"9\n\x07\x44\x61taset\x12.\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x06\x63onfig\"<\n\nConnection\x12.\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x06\x63onfigBGZEgithub.com/doublecloud/api/doublecloud/visualization/v1;visualizationb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+doublecloud/visualization/v1/workbook.proto\x12\x1c\x64oublecloud.visualization.v1\x1a\x1cgoogle/protobuf/struct.proto\"%\n\x0bPlainSecret\x12\x16\n\x06secret\x18\x01 \x01(\tR\x06secret\"b\n\x06Secret\x12N\n\x0cplain_secret\x18\x01 \x01(\x0b\x32).doublecloud.visualization.v1.PlainSecretH\x00R\x0bplainSecretB\x08\n\x06secret\":\n\x08Workbook\x12.\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x06\x63onfig\"9\n\x07\x44\x61taset\x12.\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x06\x63onfig\"<\n\nConnection\x12.\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x06\x63onfigBOZMgithub.com/doublecloud/go-genproto/doublecloud/visualization/v1;visualizationb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.visualization.v1.workbook_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZEgithub.com/doublecloud/api/doublecloud/visualization/v1;visualization'
+  DESCRIPTOR._serialized_options = b'ZMgithub.com/doublecloud/go-genproto/doublecloud/visualization/v1;visualization'
   _globals['_PLAINSECRET']._serialized_start=107
   _globals['_PLAINSECRET']._serialized_end=144
   _globals['_SECRET']._serialized_start=146
   _globals['_SECRET']._serialized_end=244
   _globals['_WORKBOOK']._serialized_start=246
   _globals['_WORKBOOK']._serialized_end=304
   _globals['_DATASET']._serialized_start=306
```

### Comparing `doublecloud-0.5.0/doublecloud/visualization/v1/workbook_pb2.pyi` & `doublecloud-0.6.0/doublecloud/visualization/v1/workbook_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/visualization/v1/workbook_service_pb2.py` & `doublecloud-0.6.0/doublecloud/visualization/v1/workbook_service_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: doublecloud/visualization/v1/workbook_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from doublecloud.v1 import operation_pb2 as doublecloud_dot_v1_dot_operation__pb2
 from doublecloud.visualization.v1 import workbook_pb2 as doublecloud_dot_visualization_dot_v1_dot_workbook__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3doublecloud/visualization/v1/workbook_service.proto\x12\x1c\x64oublecloud.visualization.v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a+doublecloud/visualization/v1/workbook.proto\"5\n\x12GetWorkbookRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\"Y\n\x13GetWorkbookResponse\x12\x42\n\x08workbook\x18\x01 \x01(\x0b\x32&.doublecloud.visualization.v1.WorkbookR\x08workbook\"]\n\x15\x43reateWorkbookRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12%\n\x0eworkbook_title\x18\x02 \x01(\tR\rworkbookTitle\"\xbd\x01\n\x15UpdateWorkbookRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\x42\n\x08workbook\x18\x02 \x01(\x0b\x32&.doublecloud.visualization.v1.WorkbookR\x08workbook\x12?\n\rforce_rewrite\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x0c\x66orceRewrite\"8\n\x15\x44\x65leteWorkbookRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\"h\n\x1cGetWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\"i\n\x1dGetWorkbookConnectionResponse\x12H\n\nconnection\x18\x01 \x01(\x0b\x32(.doublecloud.visualization.v1.ConnectionR\nconnection\"\xf3\x01\n\x1f\x43reateWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\x12H\n\nconnection\x18\x03 \x01(\x0b\x32(.doublecloud.visualization.v1.ConnectionR\nconnection\x12<\n\x06secret\x18\x04 \x01(\x0b\x32$.doublecloud.visualization.v1.SecretR\x06secret\"\xf3\x01\n\x1fUpdateWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\x12H\n\nconnection\x18\x03 \x01(\x0b\x32(.doublecloud.visualization.v1.ConnectionR\nconnection\x12<\n\x06secret\x18\x04 \x01(\x0b\x32$.doublecloud.visualization.v1.SecretR\x06secret\"k\n\x1f\x44\x65leteWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\"\xb6\x01\n\x1a\x41\x64viseDatasetFieldsRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\x12N\n\x0fpartial_dataset\x18\x03 \x01(\x0b\x32%.doublecloud.visualization.v1.DatasetR\x0epartialDataset\"^\n\x1b\x41\x64viseDatasetFieldsResponse\x12?\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32%.doublecloud.visualization.v1.DatasetR\x07\x64\x61taset2\xed\x07\n\x0fWorkbookService\x12j\n\x03Get\x12\x30.doublecloud.visualization.v1.GetWorkbookRequest\x1a\x31.doublecloud.visualization.v1.GetWorkbookResponse\x12X\n\x06\x43reate\x12\x33.doublecloud.visualization.v1.CreateWorkbookRequest\x1a\x19.doublecloud.v1.Operation\x12X\n\x06Update\x12\x33.doublecloud.visualization.v1.UpdateWorkbookRequest\x1a\x19.doublecloud.v1.Operation\x12X\n\x06\x44\x65lete\x12\x33.doublecloud.visualization.v1.DeleteWorkbookRequest\x1a\x19.doublecloud.v1.Operation\x12\x88\x01\n\rGetConnection\x12:.doublecloud.visualization.v1.GetWorkbookConnectionRequest\x1a;.doublecloud.visualization.v1.GetWorkbookConnectionResponse\x12l\n\x10\x43reateConnection\x12=.doublecloud.visualization.v1.CreateWorkbookConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12l\n\x10UpdateConnection\x12=.doublecloud.visualization.v1.UpdateWorkbookConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12l\n\x10\x44\x65leteConnection\x12=.doublecloud.visualization.v1.DeleteWorkbookConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12\x8a\x01\n\x13\x41\x64viseDatasetFields\x12\x38.doublecloud.visualization.v1.AdviseDatasetFieldsRequest\x1a\x39.doublecloud.visualization.v1.AdviseDatasetFieldsResponseBGZEgithub.com/doublecloud/api/doublecloud/visualization/v1;visualizationb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3doublecloud/visualization/v1/workbook_service.proto\x12\x1c\x64oublecloud.visualization.v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1e\x64oublecloud/v1/operation.proto\x1a+doublecloud/visualization/v1/workbook.proto\"5\n\x12GetWorkbookRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\"Y\n\x13GetWorkbookResponse\x12\x42\n\x08workbook\x18\x01 \x01(\x0b\x32&.doublecloud.visualization.v1.WorkbookR\x08workbook\"]\n\x15\x43reateWorkbookRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12%\n\x0eworkbook_title\x18\x02 \x01(\tR\rworkbookTitle\"\xbd\x01\n\x15UpdateWorkbookRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\x42\n\x08workbook\x18\x02 \x01(\x0b\x32&.doublecloud.visualization.v1.WorkbookR\x08workbook\x12?\n\rforce_rewrite\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x0c\x66orceRewrite\"8\n\x15\x44\x65leteWorkbookRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\"h\n\x1cGetWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\"i\n\x1dGetWorkbookConnectionResponse\x12H\n\nconnection\x18\x01 \x01(\x0b\x32(.doublecloud.visualization.v1.ConnectionR\nconnection\"\xf3\x01\n\x1f\x43reateWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\x12H\n\nconnection\x18\x03 \x01(\x0b\x32(.doublecloud.visualization.v1.ConnectionR\nconnection\x12<\n\x06secret\x18\x04 \x01(\x0b\x32$.doublecloud.visualization.v1.SecretR\x06secret\"\xf3\x01\n\x1fUpdateWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\x12H\n\nconnection\x18\x03 \x01(\x0b\x32(.doublecloud.visualization.v1.ConnectionR\nconnection\x12<\n\x06secret\x18\x04 \x01(\x0b\x32$.doublecloud.visualization.v1.SecretR\x06secret\"k\n\x1f\x44\x65leteWorkbookConnectionRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\"\xb6\x01\n\x1a\x41\x64viseDatasetFieldsRequest\x12\x1f\n\x0bworkbook_id\x18\x01 \x01(\tR\nworkbookId\x12\'\n\x0f\x63onnection_name\x18\x02 \x01(\tR\x0e\x63onnectionName\x12N\n\x0fpartial_dataset\x18\x03 \x01(\x0b\x32%.doublecloud.visualization.v1.DatasetR\x0epartialDataset\"^\n\x1b\x41\x64viseDatasetFieldsResponse\x12?\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32%.doublecloud.visualization.v1.DatasetR\x07\x64\x61taset2\xed\x07\n\x0fWorkbookService\x12j\n\x03Get\x12\x30.doublecloud.visualization.v1.GetWorkbookRequest\x1a\x31.doublecloud.visualization.v1.GetWorkbookResponse\x12X\n\x06\x43reate\x12\x33.doublecloud.visualization.v1.CreateWorkbookRequest\x1a\x19.doublecloud.v1.Operation\x12X\n\x06Update\x12\x33.doublecloud.visualization.v1.UpdateWorkbookRequest\x1a\x19.doublecloud.v1.Operation\x12X\n\x06\x44\x65lete\x12\x33.doublecloud.visualization.v1.DeleteWorkbookRequest\x1a\x19.doublecloud.v1.Operation\x12\x88\x01\n\rGetConnection\x12:.doublecloud.visualization.v1.GetWorkbookConnectionRequest\x1a;.doublecloud.visualization.v1.GetWorkbookConnectionResponse\x12l\n\x10\x43reateConnection\x12=.doublecloud.visualization.v1.CreateWorkbookConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12l\n\x10UpdateConnection\x12=.doublecloud.visualization.v1.UpdateWorkbookConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12l\n\x10\x44\x65leteConnection\x12=.doublecloud.visualization.v1.DeleteWorkbookConnectionRequest\x1a\x19.doublecloud.v1.Operation\x12\x8a\x01\n\x13\x41\x64viseDatasetFields\x12\x38.doublecloud.visualization.v1.AdviseDatasetFieldsRequest\x1a\x39.doublecloud.visualization.v1.AdviseDatasetFieldsResponseBOZMgithub.com/doublecloud/go-genproto/doublecloud/visualization/v1;visualizationb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'doublecloud.visualization.v1.workbook_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZEgithub.com/doublecloud/api/doublecloud/visualization/v1;visualization'
+  DESCRIPTOR._serialized_options = b'ZMgithub.com/doublecloud/go-genproto/doublecloud/visualization/v1;visualization'
   _globals['_GETWORKBOOKREQUEST']._serialized_start=194
   _globals['_GETWORKBOOKREQUEST']._serialized_end=247
   _globals['_GETWORKBOOKRESPONSE']._serialized_start=249
   _globals['_GETWORKBOOKRESPONSE']._serialized_end=338
   _globals['_CREATEWORKBOOKREQUEST']._serialized_start=340
   _globals['_CREATEWORKBOOKREQUEST']._serialized_end=433
   _globals['_UPDATEWORKBOOKREQUEST']._serialized_start=436
```

### Comparing `doublecloud-0.5.0/doublecloud/visualization/v1/workbook_service_pb2.pyi` & `doublecloud-0.6.0/doublecloud/visualization/v1/workbook_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py` & `doublecloud-0.6.0/doublecloud/visualization/v1/workbook_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/doublecloud.egg-info/PKG-INFO` & `doublecloud-0.6.0/doublecloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doublecloud
-Version: 0.5.0
+Version: 0.6.0
 Summary: The Double.Cloud official SDK
 Home-page: https://github.com/doublecloud/python-sdk
 Author: DoubleCloud GmbH
 Author-email: support@double.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `doublecloud-0.5.0/doublecloud.egg-info/SOURCES.txt` & `doublecloud-0.6.0/doublecloud.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,20 @@
 doublecloud/kafka/v1/cluster_pb2_grpc.py
 doublecloud/kafka/v1/cluster_service_pb2.py
 doublecloud/kafka/v1/cluster_service_pb2.pyi
 doublecloud/kafka/v1/cluster_service_pb2_grpc.py
 doublecloud/kafka/v1/config_pb2.py
 doublecloud/kafka/v1/config_pb2.pyi
 doublecloud/kafka/v1/config_pb2_grpc.py
+doublecloud/kafka/v1/connector_pb2.py
+doublecloud/kafka/v1/connector_pb2.pyi
+doublecloud/kafka/v1/connector_pb2_grpc.py
+doublecloud/kafka/v1/connector_service_pb2.py
+doublecloud/kafka/v1/connector_service_pb2.pyi
+doublecloud/kafka/v1/connector_service_pb2_grpc.py
 doublecloud/kafka/v1/operation_service_pb2.py
 doublecloud/kafka/v1/operation_service_pb2.pyi
 doublecloud/kafka/v1/operation_service_pb2_grpc.py
 doublecloud/kafka/v1/topic_pb2.py
 doublecloud/kafka/v1/topic_pb2.pyi
 doublecloud/kafka/v1/topic_pb2_grpc.py
 doublecloud/kafka/v1/topic_service_pb2.py
@@ -116,14 +122,17 @@
 doublecloud/transfer/v1/endpoint/__init__.py
 doublecloud/transfer/v1/endpoint/clickhouse_pb2.py
 doublecloud/transfer/v1/endpoint/clickhouse_pb2.pyi
 doublecloud/transfer/v1/endpoint/clickhouse_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/common_pb2.py
 doublecloud/transfer/v1/endpoint/common_pb2.pyi
 doublecloud/transfer/v1/endpoint/common_pb2_grpc.py
+doublecloud/transfer/v1/endpoint/delta_lake_pb2.py
+doublecloud/transfer/v1/endpoint/delta_lake_pb2.pyi
+doublecloud/transfer/v1/endpoint/delta_lake_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/kafka_pb2.py
 doublecloud/transfer/v1/endpoint/kafka_pb2.pyi
 doublecloud/transfer/v1/endpoint/kafka_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/mongo_pb2.py
 doublecloud/transfer/v1/endpoint/mongo_pb2.pyi
 doublecloud/transfer/v1/endpoint/mongo_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/mysql_pb2.py
@@ -162,14 +171,17 @@
 doublecloud/transfer/v1/endpoint/airbyte/mssql_source_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.py
 doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/redshift_source_pb2_grpc.py
 doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.py
 doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2.pyi
 doublecloud/transfer/v1/endpoint/airbyte/s3_source_pb2_grpc.py
+doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.py
+doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2.pyi
+doublecloud/transfer/v1/endpoint/airbyte/snowflake_source_pb2_grpc.py
 doublecloud/v1/__init__.py
 doublecloud/v1/cluster_pb2.py
 doublecloud/v1/cluster_pb2.pyi
 doublecloud/v1/cluster_pb2_grpc.py
 doublecloud/v1/maintenance_pb2.py
 doublecloud/v1/maintenance_pb2.pyi
 doublecloud/v1/maintenance_pb2_grpc.py
```

### Comparing `doublecloud-0.5.0/pyproject.toml` & `doublecloud-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doublecloud-0.5.0/setup.py` & `doublecloud-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 packages = find_packages(".", include=["doublecloud*"])
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 setup(
     name="doublecloud",
     version=__version__,
     description="The Double.Cloud official SDK",
     url="https://github.com/doublecloud/python-sdk",
     author="DoubleCloud GmbH",
```

