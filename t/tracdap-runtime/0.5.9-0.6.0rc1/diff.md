# Comparing `tmp/tracdap-runtime-0.5.9.tar.gz` & `tmp/tracdap-runtime-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracdap-runtime-0.5.9.tar", last modified: Thu Jan 12 13:00:55 2023, max compression
+gzip compressed data, was "tracdap-runtime-0.6.0rc1.tar", last modified: Tue Jun 13 13:17:07 2023, max compression
```

## Comparing `tracdap-runtime-0.5.9.tar` & `tracdap-runtime-0.6.0rc1.tar`

### file list

```diff
@@ -1,103 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:55.544162 tracdap-runtime-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-01-12 13:00:55.544162 tracdap-runtime-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-01-12 13:00:55.548162 tracdap-runtime-0.5.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:55.536162 tracdap-runtime-0.5.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:55.536162 tracdap-runtime-0.5.9/src/tracdap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:55.536162 tracdap-runtime-0.5.9/src/tracdap/rt/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:55.536162 tracdap-runtime-0.5.9/src/tracdap/rt/_exec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_exec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22203 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_exec/actors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_exec/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    29174 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_exec/dev_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    24913 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_exec/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23935 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_exec/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_exec/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    27465 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_exec/graph_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_exec/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:55.540162 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15263 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/csv_codec.py
--rw-r--r--   0 runner    (1001) docker     (123)    30226 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    21672 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    18737 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/shim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/static_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22948 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/type_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_impl/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:55.540162 tracdap-runtime-0.5.9/src/tracdap/rt/_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_plugins/aws_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:55.540162 tracdap-runtime-0.5.9/src/tracdap/rt/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/api/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/api/model_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19831 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/api/static_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:55.540162 tracdap-runtime-0.5.9/src/tracdap/rt/config/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/config/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/config/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/config/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/config/gateway_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/config/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/config/job_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/config/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/config/platform_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/config/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/config/result_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/config/runtime_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:55.540162 tracdap-runtime-0.5.9/src/tracdap/rt/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/ext/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/ext/repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/ext/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:55.540162 tracdap-runtime-0.5.9/src/tracdap/rt/launch/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/launch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/launch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/launch/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-01-12 13:00:17.000000 tracdap-runtime-0.5.9/src/tracdap/rt/launch/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:55.544162 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/custom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/flow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/job_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/object_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/object_id_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/object_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/search_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/stoarge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/stoarge_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/tag_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/tag_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/tag_update_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-01-12 13:00:48.000000 tracdap-runtime-0.5.9/src/tracdap/rt/metadata/type_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:00:55.544162 tracdap-runtime-0.5.9/tracdap_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-01-12 13:00:55.000000 tracdap-runtime-0.5.9/tracdap_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-01-12 13:00:55.000000 tracdap-runtime-0.5.9/tracdap_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 13:00:55.000000 tracdap-runtime-0.5.9/tracdap_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-12 13:00:55.000000 tracdap-runtime-0.5.9/tracdap_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-12 13:00:55.000000 tracdap-runtime-0.5.9/tracdap_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:17:07.027536 tracdap-runtime-0.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-13 13:17:07.027536 tracdap-runtime-0.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-13 13:17:07.027536 tracdap-runtime-0.6.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:17:07.003536 tracdap-runtime-0.6.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:17:07.003536 tracdap-runtime-0.6.0rc1/src/tracdap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:17:07.007536 tracdap-runtime-0.6.0rc1/src/tracdap/rt/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:17:07.007536 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32242 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/actors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29337 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/dev_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29952 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23310 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10991 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29055 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/graph_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:17:07.011536 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15263 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30498 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/guard_rails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23148 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/static_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31457 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/type_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:17:07.015536 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/format_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/format_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/format_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/repo_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/repo_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/repo_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/storage_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/storage_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/storage_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:17:07.015536 tracdap-runtime-0.6.0rc1/src/tracdap/rt/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/api/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/api/model_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/api/static_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:17:07.019536 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/gateway_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/job_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/platform_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/result_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/runtime_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:17:07.019536 tracdap-runtime-0.6.0rc1/src/tracdap/rt/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/ext/_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/ext/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/ext/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/ext/repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/ext/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:17:07.019536 tracdap-runtime-0.6.0rc1/src/tracdap/rt/launch/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/launch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/launch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/launch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-06-13 13:15:55.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/launch/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:17:07.027536 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/custom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/flow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/job_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/object_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/object_id_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/object_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/search_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/stoarge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/stoarge_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/tag_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/tag_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/tag_update_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-13 13:16:58.000000 tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/type_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:17:07.027536 tracdap-runtime-0.6.0rc1/tracdap_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-13 13:17:06.000000 tracdap-runtime-0.6.0rc1/tracdap_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-13 13:17:07.000000 tracdap-runtime-0.6.0rc1/tracdap_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:17:06.000000 tracdap-runtime-0.6.0rc1/tracdap_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-13 13:17:06.000000 tracdap-runtime-0.6.0rc1/tracdap_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 13:17:06.000000 tracdap-runtime-0.6.0rc1/tracdap_runtime.egg-info/top_level.txt
```

### Comparing `tracdap-runtime-0.5.9/LICENSE` & `tracdap-runtime-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/PKG-INFO` & `tracdap-runtime-0.6.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracdap-runtime
-Version: 0.5.9
+Version: 0.6.0rc1
 Summary: Runtime package for building models on the TRAC Data & Analytics Platform
 Home-page: https://tracdap.finos.org/
 Author: Martin Traverse
 Author-email: martin.traverse@accenture.com
 License: Apache-2.0
 Project-URL: Documentation, https://tracdap.readthedocs.io/
 Project-URL: Source Code, https://github.com/finos/tracdap
@@ -35,17 +35,17 @@
 
 ## Requirements
 
 The TRAC runtime for Python has these requirements:
 
 * Python: 3.7 up to 3.11.x
 * Pandas: 1.2 up to 1.5.x
-* PySpark 2.4.x, or 3.0 up to 3.3.x
+* PySpark 3.0 up to 3.4.x (optional)
 
-Not every combination of versions will work, e.g. PySpark 3 requires Python 3.8.
+Not every combination of versions will work, e.g. using PySpark 3 requires Python 3.8.
 
 
 ## Installing the runtime
 
 The TRAC runtime package can be installed directly from PyPI:
 
     pip install tracdap-runtime
```

### Comparing `tracdap-runtime-0.5.9/README.md` & `tracdap-runtime-0.6.0rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 ## Requirements
 
 The TRAC runtime for Python has these requirements:
 
 * Python: 3.7 up to 3.11.x
 * Pandas: 1.2 up to 1.5.x
-* PySpark 2.4.x, or 3.0 up to 3.3.x
+* PySpark 3.0 up to 3.4.x (optional)
 
-Not every combination of versions will work, e.g. PySpark 3 requires Python 3.8.
+Not every combination of versions will work, e.g. using PySpark 3 requires Python 3.8.
 
 
 ## Installing the runtime
 
 The TRAC runtime package can be installed directly from PyPI:
 
     pip install tracdap-runtime
```

### Comparing `tracdap-runtime-0.5.9/setup.cfg` & `tracdap-runtime-0.6.0rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tracdap-runtime
-version = 0.5.9
+version = 0.6.0rc1
 description = Runtime package for building models on the TRAC Data & Analytics Platform
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache-2.0
 platform = any
 url = https://tracdap.finos.org/
 project_urls = 
@@ -31,23 +31,24 @@
 	tracdap.rt._plugins
 package_dir = 
 	tracdap = src/tracdap
 	tracdap.rt = src/tracdap/rt
 python_requires = >= 3.7, < 3.12
 install_requires = 
 	protobuf == 4.21.10
-	pyarrow == 10.0.1
+	pyarrow == 12.0.0
 	pyyaml == 6.0.0
+	dulwich == 0.21.2
 	requests == 2.28.1
 	
 	pandas >= 1.2.0, < 1.6.0
 
 [options.extras_require]
 spark = 
-	pyspark >= 2.4.0, < 3.4.0
+	pyspark >= 3.0.0, < 3.5.0
 aws = 
 	boto3 == 1.26.22
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/__init__.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/__init__.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_exec/context.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
+import pathlib
 import typing as tp
 import re
 import traceback
 
 import pandas as pd
 
 import tracdap.rt.api as _api
@@ -55,30 +56,33 @@
 
     __DEFAULT_TEMPORAL_OBJECTS = False
 
     def __init__(self,
                  model_def: _meta.ModelDefinition,
                  model_class: _api.TracModel.__class__,
                  local_ctx: tp.Dict[str, _data.DataView],
-                 schemas: tp.Dict[str, _meta.SchemaDefinition]):
+                 schemas: tp.Dict[str, _meta.SchemaDefinition],
+                 checkout_directory: pathlib.Path = None):
 
         self.__ctx_log = _util.logger_for_object(self)
         self.__model_log = _util.logger_for_class(model_class)
 
         self.__model_def = model_def
         self.__model_class = model_class
 
         self.__parameters = local_ctx or {}
         self.__data = local_ctx or {}
         self.__schemas = schemas
 
         self.__val = TracContextValidator(
             self.__ctx_log,
             self.__parameters,
-            self.__data)
+            self.__data,
+            checkout_directory)
+
 
     def get_parameter(self, parameter_name: str) -> tp.Any:
 
         _val.validate_signature(self.get_parameter, parameter_name)
 
         self.__val.check_param_not_null(parameter_name)
         self.__val.check_param_valid_identifier(parameter_name)
@@ -171,52 +175,38 @@
 
 
 class TracContextValidator:
 
     __VALID_IDENTIFIER = re.compile("^[a-zA-Z_]\\w*$",)
     __RESERVED_IDENTIFIER = re.compile("^(trac_|_)\\w*")
 
-    __LAST_MODEL_FRAME = -4
-    __FIRST_MODEL_FRAME_NAME = "run_model"
-    __FIRST_MODEL_FRAME_TEST_NAME = "_callTestMethod"
-
     def __init__(
             self, log: logging.Logger,
             parameters: tp.Dict[str, tp.Any],
-            data_ctx: tp.Dict[str, _data.DataView]):
+            data_ctx: tp.Dict[str, _data.DataView],
+            checkout_directory: pathlib.Path):
 
         self.__log = log
         self.__parameters = parameters
         self.__data_ctx = data_ctx
+        self.__checkout_directory = checkout_directory
 
     def _report_error(self, message):
 
-        model_stack = self._build_model_stack_trace()
+        full_stack = traceback.extract_stack()
+        model_stack = _util.filter_model_stack_trace(full_stack, self.__checkout_directory)
         model_stack_str = ''.join(traceback.format_list(list(reversed(model_stack))))
+        details = _util.error_details_from_trace(model_stack)
+        message = f"{message} {details}"
 
         self.__log.error(message)
         self.__log.error(f"Model stack trace:\n{model_stack_str}")
 
         raise _ex.ERuntimeValidation(message)
 
-    def _build_model_stack_trace(self):
-
-        full_stack = traceback.extract_stack()
-
-        frame_names = list(map(lambda frame: frame.name, full_stack))
-
-        if self.__FIRST_MODEL_FRAME_NAME in frame_names:
-            first_model_frame = frame_names.index(self.__FIRST_MODEL_FRAME_NAME)
-        elif self.__FIRST_MODEL_FRAME_TEST_NAME in frame_names:
-            first_model_frame = frame_names.index(self.__FIRST_MODEL_FRAME_TEST_NAME)
-        else:
-            first_model_frame = 0
-
-        return full_stack[first_model_frame:self.__LAST_MODEL_FRAME]
-
     def check_param_not_null(self, param_name):
 
         if param_name is None:
             self._report_error(f"Parameter name is null")
 
     def check_param_valid_identifier(self, param_name: str):
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_exec/dev_mode.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/dev_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -644,15 +644,16 @@
 
             x_storage_mgr = _storage.StorageManager(sys_config)
             x_storage = x_storage_mgr.get_file_storage(storage_key)
             x_orig_path = pathlib.PurePath(storage_path)
             x_name = x_orig_path.name
 
             if x_storage.exists(str(x_orig_path.parent)):
-                existing_files = x_storage.ls(str(x_orig_path.parent))
+                listing = x_storage.ls(str(x_orig_path.parent))
+                existing_files = list(map(lambda stat: stat.file_name, listing))
             else:
                 existing_files = []
 
             while x_name in existing_files:
 
                 snap_version += 1
                 x_name = f"{x_orig_path.stem}-{snap_version}"
@@ -667,15 +668,18 @@
 
         return data_obj, storage_obj
 
     @staticmethod
     def infer_format(storage_path: str, storage_config: _cfg.StorageConfig):
 
         if re.match(r'.*\.\w+$', storage_path):
-            return _storage.FormatManager.format_for_extension(pathlib.Path(storage_path).suffix)
+            extension = pathlib.Path(storage_path).suffix
+            codec = _storage.FormatManager.get_data_format(extension, format_options={})
+            return codec.format_code()
+
         else:
             return storage_config.defaultFormat
 
     @classmethod
     def _generate_input_definition(
             cls, data_id: _meta.TagHeader, storage_id: _meta.TagHeader,
             storage_key: str, storage_path: str, storage_format: str,
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_exec/engine.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -110,25 +110,28 @@
             failed_job_key = None
 
             # Look for the job key corresponding to the failed actor
             for job_key, job_actor in self._job_actors.items():
                 if job_actor == signal.sender:
                     failed_job_key = job_key
 
-            # If the job key is not found, the job has already been stopped and no action is needed
             # If the job is still live, call job_failed explicitly
             if failed_job_key is not None:
-                if isinstance(signal, _actors.ErrorSignal) and signal.error:
-                    error = signal.error
-                else:
-                    error = _ex.ETracInternal("An unknown error occurred")
-                self.actors().send("job_failed", failed_job_key, error)
 
-            # Failed signal has been handled, do not propagate
-            return True
+                cause = signal.error if isinstance(signal, _actors.ErrorSignal) else None
+                cause_message = str(cause) if cause is not None else "(unknown)"
+                message = f"There was an error in the TRAC execution engine: " + \
+                          f"failed node = [{signal.sender}], cause = {cause_message}"
+                error = _ex .ETracInternal(message)
+                error.__cause__ = cause
+
+                self.actors().send(self.actors().id, "job_failed", failed_job_key, error)
+
+                # Failed signal has been handled, do not propagate
+                return True
 
         return super().on_signal(signal)
 
     @_actors.Message
     def submit_job(
             self, job_config: _cfg.JobConfig,
             job_result_dir: str,
@@ -137,52 +140,50 @@
         job_key = _util.object_key(job_config.jobId)
 
         result_needed = bool(job_result_dir)
         result_spec = _graph.JobResultSpec(result_needed, job_result_dir, job_result_format)
 
         self._log.info(f"Job submitted: [{job_key}]")
 
-        job_actor_id = self.actors().spawn(
-            JobProcessor, job_key,
-            job_config, result_spec,
-            self._models, self._storage)
+        job_processor = JobProcessor(job_key, job_config, result_spec,self._models, self._storage)
+        job_actor_id = self.actors().spawn(job_processor)
 
         job_actors = {**self._job_actors, job_key: job_actor_id}
         self._job_actors = job_actors
 
     @_actors.Message
     def job_succeeded(self, job_key: str, job_result: _cfg.JobResult):
 
         # Ignore duplicate messages from the job processor (can happen in unusual error cases)
         if job_key not in self._job_actors:
             self._log.warning(f"Ignoring [job_succeeded] message, job [{job_key}] has already completed")
             return
 
         self._log.info(f"Recording job as successful: {job_key}")
 
+        self._finalize_job(job_key)
+
         if self._notify_callback is not None:
             self._notify_callback(job_key, job_result, None)
 
-        self._finalize_job(job_key)
-
     @_actors.Message
     def job_failed(self, job_key: str, error: Exception):
 
         # Ignore duplicate messages from the job processor (can happen in unusual error cases)
         if job_key not in self._job_actors:
             self._log.warning(f"Ignoring [job_failed] message, job [{job_key}] has already completed")
             return
 
         self._log.error(f"Recording job as failed: {job_key}")
 
+        self._finalize_job(job_key)
+
         if self._notify_callback is not None:
             self._notify_callback(job_key, None, error)
 
-        self._finalize_job(job_key)
-
     def _finalize_job(self, job_key: str):
 
         job_actors = self._job_actors
         job_actor_id = job_actors.pop(job_key)
         self.actors().stop(job_actor_id)
         self._job_actors = job_actors
 
@@ -207,33 +208,55 @@
         self._models = models
         self._storage = storage
         self._log = _util.logger_for_object(self)
 
     def on_start(self):
         self._log.info(f"Starting job [{self.job_key}]")
         self._models.create_scope(self.job_key)
-        self.actors().spawn(GraphBuilder, self.job_config, self.result_spec, self._models, self._storage)
+        self.actors().spawn(GraphBuilder(self.job_config, self.result_spec, self._models, self._storage))
 
     def on_stop(self):
         self._log.info(f"Cleaning up job [{self.job_key}]")
         self._models.destroy_scope(self.job_key)
 
+    def on_signal(self, signal: Signal) -> tp.Optional[bool]:
+
+        if signal.message == _actors.SignalNames.FAILED and isinstance(signal, _actors.ErrorSignal):
+
+            if isinstance(signal.error, _ex.ETrac):
+                error = signal.error
+
+            else:
+                cause = str(signal.error) if signal.error is not None else "(unknown)"
+                message = f"There was an error in the TRAC execution engine: " + \
+                          f"failed node = [{signal.sender}], cause = {cause}"
+                error = _ex .ETracInternal(message)
+                error.__cause__ = signal.error
+
+            self.actors().send(self.actors().id, "job_failed",  error)
+
+            return True
+
+        return super().on_signal(signal)
+
     @_actors.Message
     def job_graph(self, graph: _EngineContext, root_id: NodeId):
-        self.actors().spawn(GraphProcessor, graph, root_id)
+        self.actors().spawn(GraphProcessor(graph, root_id))
         self.actors().stop(self.actors().sender)
 
     @_actors.Message
     def job_succeeded(self, job_result: _cfg.JobResult):
         self._log.info(f"Job succeeded {self.job_key}")
+        self.actors().stop(self.actors().sender)
         self.actors().send_parent("job_succeeded", self.job_key, job_result)
 
     @_actors.Message
     def job_failed(self, error: Exception):
         self._log.error(f"Job failed {self.job_key}")
+        self.actors().stop(self.actors().sender)
         self.actors().send_parent("job_failed", self.job_key, error)
 
 
 class GraphBuilder(_actors.Actor):
 
     """
     GraphBuilder is a worker (actors.Worker) responsible for building the execution graph for a job
@@ -305,14 +328,24 @@
     @_actors.Message
     def submit_viable_nodes(self):
 
         node_processors = dict()
 
         def process_graph(graph: _EngineContext) -> _EngineContext:
 
+            processed_graph = cp.copy(graph)
+            processed_graph.nodes = cp.copy(graph.nodes)
+
+            # Start by removing any nodes that are no longer needed
+            for node_id, node in graph.nodes.items():
+                if node_id in graph.succeeded_nodes and not self._is_required_node(node, graph):
+                    node = processed_graph.nodes.pop(node_id)
+                    NodeLogger.log_node_evict(node)
+                    del node
+
             pending_nodes = cp.copy(graph.pending_nodes)
             active_nodes = cp.copy(graph.active_nodes)
             failed_nodes = cp.copy(graph.failed_nodes)
 
             for node_id in graph.pending_nodes:
 
                 node = self.graph.nodes[node_id]
@@ -322,21 +355,33 @@
                     self._log.warning(f"SKIP {str(node_id)} (upstream failure)")
 
                     pending_nodes.discard(node_id)
                     failed_nodes.add(node_id)
 
                 elif self._is_viable_node(node, graph):
 
-                    node_ref = self.actors().spawn(NodeProcessor, self.graph, node_id, node)
+                    # This is very basic separation of different node types
+                    # Model and data nodes map to different thread pools in the actors engine
+                    # There is scope for a much more sophisticated approach, with prioritized scheduling
+
+                    if isinstance(node.node, _graph.RunModelNode) or isinstance(node.node, _graph.ImportModelNode):
+                        processor = ModelNodeProcessor(processed_graph, node_id, node)
+                    elif isinstance(node.node, _graph.LoadDataNode) or isinstance(node.node, _graph.SaveDataNode):
+                        processor = DataNodeProcessor(processed_graph, node_id, node)
+                    else:
+                        processor = NodeProcessor(processed_graph, node_id, node)
+
+                    # New nodes can be launched with the updated graph
+                    # Anything that was pruned is not needed by the new node
+                    node_ref = self.actors().spawn(processor)
                     node_processors[node_id] = node_ref
 
                     pending_nodes.discard(node_id)
                     active_nodes.add(node_id)
 
-            processed_graph = cp.copy(self.graph)
             processed_graph.pending_nodes = pending_nodes
             processed_graph.active_nodes = active_nodes
             processed_graph.failed_nodes = failed_nodes
 
             return processed_graph
 
         current_graph = self.graph
@@ -350,27 +395,47 @@
         self.graph = new_graph
         self.processors = {**self.processors, **node_processors}
 
         # Job may have completed due to error propagation
         self.check_job_status(do_submit=False)
 
     @classmethod
+    def _is_required_node(cls, node: _EngineNode, graph: _EngineContext):
+
+        if node.node.id not in graph.succeeded_nodes:
+            return False
+
+        def live_node(nid_n):
+            nid_, _ = nid_n
+            return nid_ in graph.active_nodes or nid_ in graph.pending_nodes
+
+        def use_target(nid_n):
+            _, n_ = nid_n
+            return node.node.id in n_.dependencies
+
+        return any(map(use_target, filter(live_node, graph.nodes.items())))
+
+    @classmethod
     def _is_viable_node(cls, node: _EngineNode, graph: _EngineContext):
 
         return all(dep in graph.succeeded_nodes for dep in node.dependencies)
 
     @classmethod
     def _upstream_failure(cls, node: _EngineNode, graph: _EngineContext):
 
         return any(not dep_type.tolerant and dep in graph.failed_nodes
                    for dep, dep_type in node.dependencies.items())
 
     @_actors.Message
     def node_succeeded(self, node_id: NodeId, result):
 
+        # Child node is no longer needed, it can be stopped to release resources
+        processor = self.processors.pop(node_id)
+        self.actors().stop(processor)
+
         old_node = self.graph.nodes[node_id]
         node = cp.copy(old_node)
         node.complete = True
         node.result = result
         results = {node_id: node}
 
         # For bundle nodes, add the individual bundle items to the result update
@@ -384,27 +449,34 @@
                 item_node = cp.copy(item_old_node)
                 item_node.complete = True
                 item_node.result = item_result
 
                 # Use the original node ID, to avoid overwriting the result type
                 results[item_node.node.id] = item_node
 
-        self._update_results(results)
+        if isinstance(node.node, _graph.ContextPopNode):
+            self._update_results(results, context_pop=node.node.id.namespace)
+        else:
+            self._update_results(results)
 
     @_actors.Message
     def node_failed(self, node_id: NodeId, error):
 
+        # Child node is no longer needed, it can be stopped to release resources
+        processor = self.processors.pop(node_id)
+        self.actors().stop(processor)
+
         old_node = self.graph.nodes[node_id]
         node = cp.copy(old_node)
         node.complete = True
         node.error = error
 
         self._update_results({node_id: node})
 
-    def _update_results(self, updates: tp.Dict[NodeId, _EngineNode]):
+    def _update_results(self, updates: tp.Dict[NodeId, _EngineNode], context_pop: _graph.NodeNamespace = None):
 
         nodes = {**self.graph.nodes, **updates}
 
         pending_nodes = cp.copy(self.graph.pending_nodes)
         active_nodes = cp.copy(self.graph.active_nodes)
         succeeded_nodes = cp.copy(self.graph.succeeded_nodes)
         failed_nodes = cp.copy(self.graph.failed_nodes)
@@ -423,14 +495,20 @@
             else:
                 succeeded_nodes.add(node_id)
 
             if node_id in self.processors:
                 node_ref = self.processors.pop(node_id)
                 self.actors().stop(node_ref)
 
+        # For context pop, remove all the nodes inside the pop context
+        # The graph builder is responsible for consistency, i.e. no dependencies across contexts
+        if context_pop:
+            for node_id in list(filter(lambda n: n.namespace == context_pop, nodes)):
+                nodes.pop(node_id)
+
         graph = _EngineContext(nodes, pending_nodes, active_nodes, succeeded_nodes, failed_nodes)
 
         self.graph = graph
         self.check_job_status()
 
     def check_job_status(self, do_submit=True):
 
@@ -465,28 +543,41 @@
 
 class NodeProcessor(_actors.Actor):
 
     """
     Processor responsible for running individual nodes in an execution graph
     """
 
-    # TODO: How to decide when to allocate an actors.Worker (long running, separate thread)
-
     __NONE_TYPE = type(None)
 
-    def __init__(self, graph: _EngineContext, node_id: str, node: _EngineNode):
+    def __init__(self, graph: _EngineContext, node_id: NodeId, node: _EngineNode):
         super().__init__()
         self.graph = graph
         self.node_id = node_id
         self.node = node
 
     def on_start(self):
 
         self.actors().send(self.actors().id, "evaluate_node")
 
+    def on_stop(self):
+
+        # Something in the engine occasionally holds onto node processors
+        # These hold a copy of the graph with the pre-execution version of their own engine node
+        # I.e. the engine node that gets retained does not hold any data
+
+        # This is not a serious issue in most cases, but it is still better to release the resources
+        # We can do this by unsetting the references to self.node and self.graph
+
+        # It would be good to find out where the reference to the processor is being held and fix at source
+        # We could also add some accounting to the _EngineNode class
+
+        self.node = None
+        self.graph = None
+
     @_actors.Message
     def graph_event(self):
         pass
 
     @_actors.Message
     def stream_event(self):
         pass
@@ -496,26 +587,26 @@
 
         try:
 
             NodeLogger.log_node_start(self.node)
 
             ctx = NodeContextImpl(self.graph.nodes)
             result = self.node.function(ctx)
-
             self._check_result_type(result)
-            self.actors().send_parent("node_succeeded", self.node_id, result)
 
             NodeLogger.log_node_succeeded(self.node)
 
-        except Exception as e:
+            self.actors().send_parent("node_succeeded", self.node_id, result)
 
-            self.actors().send_parent("node_failed", self.node_id, e)
+        except Exception as e:
 
             NodeLogger.log_node_failed(self.node, e)
 
+            self.actors().send_parent("node_failed", self.node_id, e)
+
     @classmethod
     def result_matches_type(cls, result, expected_type) -> bool:
 
         if expected_type is None or expected_type == cls.__NONE_TYPE:
             return result is None
 
         if expected_type == tp.Any:
@@ -558,14 +649,26 @@
         result_type = type(result)
 
         if not self.result_matches_type(result, expected_type):
             err = f"Node result is the wrong type, expected [{expected_type.__name__}], got [{result_type.__name__}]"
             raise _ex.ETracInternal(err)
 
 
+class ModelNodeProcessor(NodeProcessor):
+
+    def __init__(self, graph: _EngineContext, node_id: NodeId, node: _EngineNode):
+        super().__init__(graph, node_id, node)
+
+
+class DataNodeProcessor(NodeProcessor):
+
+    def __init__(self, graph: _EngineContext, node_id: NodeId, node: _EngineNode):
+        super().__init__(graph, node_id, node)
+
+
 class NodeLogger:
 
     """
     Log the activity of the NodeProcessor
     """
 
     # Separate out the logic for logging nodes, so the NodeProcessor itself stays a bit cleaner
@@ -619,14 +722,26 @@
         node_name = node.node.id.name
         namespace = node.node.id.namespace
 
         cls._log.error(f"FAILED {cls._func_type(node)} [{node_name}] / {namespace}")
         cls._log.exception(e)
 
     @classmethod
+    def log_node_evict(cls, node: _EngineNode):
+
+        logging_type = cls._logging_type(node)
+        node_name = node.node.id.name
+        namespace = node.node.id.namespace
+
+        if logging_type in [cls.LoggingType.STATIC_VALUE, cls.LoggingType.SIMPLE_MAPPING]:
+            return
+
+        cls._log.info(f"EVICT {cls._func_type(node)} [{node_name}] / {namespace}")
+
+    @classmethod
     def _log_push_pop_node_details(cls, node: tp.Union[_graph.ContextPushNode, _graph.ContextPopNode]):
 
         push_or_pop = "PUSH" if isinstance(node, _graph.ContextPushNode) else "POP"
         direction = "->" if isinstance(node, _graph.ContextPushNode) else "<-"
 
         for inner_id, outer_id in node.mapping.items():
             item_type = cls._type_str(inner_id.result_type)
@@ -648,15 +763,15 @@
 
         if isinstance(node.node, _graph.StaticValueNode):
             return cls.LoggingType.STATIC_VALUE
 
         if isinstance(node.node, _graph.ContextPushNode) or isinstance(node.node, _graph.ContextPopNode):
             return cls.LoggingType.PUSH_POP
 
-        if isinstance(node.node, _graph.IdentityNode):
+        if isinstance(node.node, _graph.IdentityNode) or isinstance(node.node, _graph.BundleItemNode):
             return cls.LoggingType.SIMPLE_MAPPING
 
         if isinstance(node.node, _graph.RunModelNode):
             return cls.LoggingType.MODEL
 
         return cls.LoggingType.DEFAULT
 
@@ -672,17 +787,17 @@
             return result_type.__name__
         else:
             return str(None)
 
     @classmethod
     def _func_type(cls, node: _EngineNode) -> str:
 
-        # Remove "Func" from "xxxFunc"
+        # Remove "Node" from "xxxNode"
 
-        func_type = type(node.function)
+        func_type = type(node.node)
         return func_type.__name__[:-4]
 
     @classmethod
     def _mapping_source(cls, node: _EngineNode) -> str:
 
         graph_node = node.node
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_exec/functions.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,18 +197,14 @@
 
         # TODO: Handle individual failed results
 
         for obj_id, node_id in self.node.objects.items():
             obj_def = _ctx_lookup(node_id, ctx)
             job_result.results[obj_id] = obj_def
 
-        for obj_id, node_id in self.node.attrs.items():
-            attrs = _ctx_lookup(node_id, ctx)
-            job_result.attrs[obj_id] = attrs
-
         for bundle_id in self.node.bundles:
             bundle = _ctx_lookup(bundle_id, ctx)
             job_result.results.update(bundle.items())
 
         return job_result
 
 
@@ -309,14 +305,16 @@
 
     def __init__(self, node: DynamicDataSpecNode, storage: _storage.StorageManager):
         self.node = node
         self.storage = storage
 
     def _execute(self, ctx: NodeContext) -> _data.DataSpec:
 
+        # When data def for an output was not supplied in the job, this function creates a dynamic data spec
+
         if self.node.prior_data_spec is not None:
             raise _ex.ETracInternal("Data updates not supported yet")
 
         data_view = _ctx_lookup(self.node.data_view_id, ctx)
 
         data_id = self.node.data_obj_id
         storage_id = self.node.storage_obj_id
@@ -370,14 +368,16 @@
             incarnationStatus=meta.IncarnationStatus.INCARNATION_AVAILABLE)
 
         storage_item = meta.StorageItem([storage_incarnation])
 
         storage_def = meta.StorageDefinition()
         storage_def.dataItems[data_item] = storage_item
 
+        # Dynamic data def will always use an embedded schema (this is no ID for an external schema)
+
         return _data.DataSpec(
             data_item,
             data_def,
             storage_def,
             schema_def=None)
 
 
@@ -505,45 +505,21 @@
 
         model_class = self._models.load_model_class(self.node.model_scope, model_stub)
         model_def = self._models.scan_model(model_stub, model_class)
 
         return meta.ObjectDefinition(meta.ObjectType.MODEL, model=model_def)
 
 
-class ImportAttrsFunc(NodeFunction[_config.TagUpdateList]):
-
-    # TODO: Remove this function, now staticAttributes are kept on model def
-
-    def __init__(self, node: ImportAttrsNode, models: _models.ModelLoader):
-        self.node = node
-        self._models = models
-
-    def _execute(self, ctx: NodeContext) -> _config.TagUpdateList:
-
-        model_stub = _model_def_for_import(self.node.import_details)
-        model_class = self._models.load_model_class(self.node.model_scope, model_stub)
-        model_def = self._models.scan_model(model_stub, model_class)
-
-        updates = []
-
-        for attr_name, attr_value in model_def.staticAttributes.items():
-
-            updates.append(meta.TagUpdate(
-                attrName=attr_name, value=attr_value,
-                operation=meta.TagOperation.CREATE_OR_REPLACE_ATTR))
-
-        return cfg.TagUpdateList(updates)
-
-
 class RunModelFunc(NodeFunction[Bundle[_data.DataView]]):
 
-    def __init__(self, node: RunModelNode, model_class: _api.TracModel.__class__):
+    def __init__(self, node: RunModelNode, model_class: _api.TracModel.__class__, checkout_directory: pathlib.Path):
         super().__init__()
         self.node = node
         self.model_class = model_class
+        self.checkout_directory = checkout_directory
 
     def _execute(self, ctx: NodeContext) -> Bundle[_data.DataView]:
 
         model_def = self.node.model_def
 
         # Create a context containing only declared items in the current namespace, addressed by name
         # The engine guarantees all required nodes are present and have type matching their node ID
@@ -583,15 +559,16 @@
 
         try:
             model = self.model_class()
             model.run_model(trac_ctx)
         except _ex.ETrac:
             raise
         except Exception as e:
-            msg = f"There was an unhandled error in the model: {str(e)}"
+            details = _util.error_details_from_model_exception(e, self.checkout_directory)
+            msg = f"There was an unhandled error in the model: {str(e)}{details}"
             raise _ex.EModelExec(msg) from e
 
         # The node result is just the model outputs taken from the local context
         model_outputs: Bundle[_data.DataView] = {
             name: obj for name, obj in local_ctx.items()
             if name in self.node.model_def.outputs}
 
@@ -646,43 +623,41 @@
 
     def resolve_dynamic_data_spec(self, node: DynamicDataSpecNode):
         return DynamicDataSpecFunc(node, self._storage)
 
     def resolve_import_model_node(self, node: ImportModelNode):
         return ImportModelFunc(node, self._models)
 
-    def resolve_import_attrs_node(self, node: ImportAttrsNode):
-        return ImportAttrsFunc(node, self._models)
-
     def resolve_run_model_node(self, node: RunModelNode) -> NodeFunction:
 
         model_class = self._models.load_model_class(node.model_scope, node.model_def)
+        checkout_directory = self._models.model_load_checkout_directory(node.model_scope, node.model_def)
 
         # TODO: Verify model_class against model_def
 
-        return RunModelFunc(node, model_class)
+        return RunModelFunc(node, model_class, checkout_directory)
 
     __basic_node_mapping: tp.Dict[Node.__class__, NodeFunction.__class__] = {
 
         ContextPushNode: ContextPushFunc,
         ContextPopNode: ContextPopFunc,
         IdentityNode: IdentityFunc,
         KeyedItemNode: KeyedItemFunc,
         DataViewNode: DataViewFunc,
         DataItemNode: DataItemFunc,
         BuildJobResultNode: BuildJobResultFunc,
         SaveJobResultNode: SaveJobResultFunc,
         DataResultNode: DataResultFunc,
         StaticValueNode: StaticValueFunc,
         BundleItemNode: NoopFunc,
-        NoopNode: NoopFunc
+        NoopNode: NoopFunc,
+        RunModelResultNode: NoopFunc
     }
 
     __node_mapping: tp.Dict[Node.__class__, __ResolveFunc] = {
 
         LoadDataNode: resolve_load_data,
         SaveDataNode: resolve_save_data,
         DynamicDataSpecNode: resolve_dynamic_data_spec,
         RunModelNode: resolve_run_model_node,
-        ImportModelNode: resolve_import_model_node,
-        ImportAttrsNode: resolve_import_attrs_node
+        ImportModelNode: resolve_import_model_node
     }
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_exec/graph.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -342,46 +342,44 @@
 class ImportModelNode(Node[meta.ObjectDefinition]):
 
     model_scope: str
     import_details: meta.ImportModelJob
 
 
 @_node_type
-class ImportAttrsNode(Node[cfg.TagUpdateList]):
-
-    # TODO: Remove this node, now staticAttributes are kept on model def
-
-    model_scope: str
-    import_details: meta.ImportModelJob
-
-
-@_node_type
 class RunModelNode(Node[Bundle[_data.DataView]]):
 
     model_scope: str
     model_def: meta.ModelDefinition
     parameter_ids: tp.FrozenSet[NodeId]
     input_ids: tp.FrozenSet[NodeId]
 
     def _node_dependencies(self) -> tp.Dict[NodeId, DependencyType]:
         return {dep_id: DependencyType.HARD for dep_id in [*self.parameter_ids, *self.input_ids]}
 
 
 @_node_type
+class RunModelResultNode(Node[None]):
+
+    model_id: NodeId
+
+    def _node_dependencies(self) -> tp.Dict[NodeId, DependencyType]:
+        return {self.model_id: DependencyType.HARD}
+
+
+@_node_type
 class BuildJobResultNode(Node[cfg.JobResult]):
 
     job_id: meta.TagHeader
 
     objects: tp.Dict[str, NodeId[meta.ObjectDefinition]] = dc.field(default_factory=dict)
-    attrs: tp.Dict[str, NodeId[cfg.TagUpdateList]] = dc.field(default_factory=dict)
-
     bundles: tp.List[NodeId[ObjectBundle]] = dc.field(default_factory=list)
 
     def _node_dependencies(self) -> tp.Dict[NodeId, DependencyType]:
-        dep_ids = [*self.bundles, *self.objects.values(), *self.attrs.values()]
+        dep_ids = [*self.bundles, *self.objects.values()]
         return {node_id: DependencyType.HARD for node_id in dep_ids}
 
 
 @_node_type
 class SaveJobResultNode(Node[None]):
 
     job_result_id: NodeId[cfg.JobResult]
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_exec/graph_builder.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/graph_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,25 +102,21 @@
 
         model_scope = _util.object_key(job_config.jobId)
         import_details = job_config.job.importModel
 
         import_id = NodeId.of("trac_import_model", job_namespace, meta.ObjectDefinition)
         import_node = ImportModelNode(import_id, model_scope, import_details, explicit_deps=[job_push_id])
 
-        import_attrs_id = NodeId.of("trac_import_attrs", job_namespace, config.TagUpdateList)
-        import_attrs_node = ImportAttrsNode(import_attrs_id, model_scope, import_details, explicit_deps=[import_id])
-
-        main_section = GraphSection(nodes={import_id: import_node, import_attrs_id: import_attrs_node})
+        main_section = GraphSection(nodes={import_id: import_node})
 
         # Build job-level metadata outputs
 
         result_section = cls.build_job_results(
             job_config, job_namespace, result_spec,
             objects={new_model_key: import_id},
-            attrs={new_model_key: import_attrs_id},
             explicit_deps=[job_push_id, *main_section.must_run])
 
         return cls._join_sections(main_section, result_section)
 
     @classmethod
     def build_run_model_job(
             cls, job_config: config.JobConfig, result_spec: JobResultSpec,
@@ -160,25 +156,25 @@
 
         params_section = cls.build_job_parameters(
             job_namespace, parameters,
             explicit_deps=[job_push_id])
 
         input_section = cls.build_job_inputs(
             job_config, job_namespace, inputs,
-            explicit_deps=[job_push_id, *params_section.must_run])
+            explicit_deps=[job_push_id])
 
         exec_obj = _util.get_job_resource(target, job_config)
 
         exec_section = cls.build_model_or_flow(
             job_config, job_namespace, exec_obj,
-            explicit_deps=[job_push_id, *params_section.must_run, *input_section.must_run])
+            explicit_deps=[job_push_id])
 
         output_section = cls.build_job_outputs(
             job_config, job_namespace, outputs,
-            explicit_deps=[job_push_id, *exec_section.must_run])
+            explicit_deps=[job_push_id])
 
         main_section = cls._join_sections(params_section, input_section, exec_section, output_section)
 
         # Build job-level metadata outputs
 
         data_result_ids = list(
             nid for nid, n in main_section.nodes.items()
@@ -223,30 +219,35 @@
         for input_name, data_selector in inputs.items():
 
             # Build a data spec using metadata from the job config
             # For now we are always loading the root part, snap 0, delta 0
             data_def = _util.get_job_resource(data_selector, job_config).data
             storage_def = _util.get_job_resource(data_def.storageId, job_config).storage
 
+            if data_def.schemaId:
+                schema_def = _util.get_job_resource(data_def.schemaId, job_config).schema
+            else:
+                schema_def = data_def.schema
+
             root_part_opaque_key = 'part-root'  # TODO: Central part names / constants
             data_item = data_def.parts[root_part_opaque_key].snap.deltas[0].dataItem
-            data_spec = _data.DataSpec(data_item, data_def, storage_def, schema_def=None)
+            data_spec = _data.DataSpec(data_item, data_def, storage_def, schema_def)
 
             # Data spec node is static, using the assembled data spec
             data_spec_id = NodeId.of(f"{input_name}:SPEC", job_namespace, _data.DataSpec)
             data_spec_node = StaticValueNode(data_spec_id, data_spec, explicit_deps=explicit_deps)
 
             # Physical load of data items from disk
             # Currently one item per input, since inputs are single part/delta
             data_load_id = NodeId.of(f"{input_name}:LOAD", job_namespace, _data.DataItem)
             data_load_node = LoadDataNode(data_load_id, data_spec_id, explicit_deps=explicit_deps)
 
             # Input views assembled by mapping one root part to each view
             data_view_id = NodeId.of(input_name, job_namespace, _data.DataView)
-            data_view_node = DataViewNode(data_view_id, data_def.schema, data_load_id)
+            data_view_node = DataViewNode(data_view_id, schema_def, data_load_id)
 
             nodes[data_spec_id] = data_spec_node
             nodes[data_load_id] = data_load_node
             nodes[data_view_id] = data_view_node
 
             # Job-level data view is an output of the load operation
             outputs.add(data_view_id)
@@ -270,29 +271,38 @@
             data_view_id = NodeId.of(output_name, job_namespace, _data.DataView)
             data_spec_id = NodeId.of(f"{output_name}:SPEC", job_namespace, _data.DataSpec)
 
             data_obj = _util.get_job_resource(data_selector, job_config, optional=True)
 
             if data_obj is not None:
 
+                # If data def for the output has been built in advance, use a static data spec
+
                 data_def = data_obj.data
-                storage_obj = _util.get_job_resource(data_def.storageId, job_config)
-                storage_def = storage_obj.storage
+                storage_def = _util.get_job_resource(data_def.storageId, job_config).storage
+
+                if data_def.schemaId:
+                    schema_def = _util.get_job_resource(data_def.schemaId, job_config).schema
+                else:
+                    schema_def = data_def.schema
 
                 root_part_opaque_key = 'part-root'  # TODO: Central part names / constants
                 data_item = data_def.parts[root_part_opaque_key].snap.deltas[0].dataItem
-                data_spec = _data.DataSpec(data_item, data_def, storage_def, schema_def=None)
+                data_spec = _data.DataSpec(data_item, data_def, storage_def, schema_def)
 
                 data_spec_node = StaticValueNode(data_spec_id, data_spec, explicit_deps=explicit_deps)
 
                 output_data_key = output_name + ":DATA"
                 output_storage_key = output_name + ":STORAGE"
 
             else:
 
+                # If output data def for an output was not supplied in the job, create a dynamic data spec
+                # Dynamic data def will always use an embedded schema (this is no ID for an external schema)
+
                 data_key = output_name + ":DATA"
                 data_id = job_config.resultMapping[data_key]
                 storage_key = output_name + ":STORAGE"
                 storage_id = job_config.resultMapping[storage_key]
 
                 data_spec_node = DynamicDataSpecNode(
                         data_spec_id, data_view_id,
@@ -326,31 +336,27 @@
 
         return GraphSection(nodes, inputs=inputs)
 
     @classmethod
     def build_job_results(
             cls, job_config: cfg.JobConfig, job_namespace: NodeNamespace, result_spec: JobResultSpec,
             objects: tp.Dict[str, NodeId[meta.ObjectDefinition]] = None,
-            attrs: tp.Dict[str, NodeId[config.TagUpdateList]] = None,
             bundles: tp.List[NodeId[ObjectBundle]] = None,
             explicit_deps: tp.Optional[tp.List[NodeId]] = None) \
             -> GraphSection:
 
         build_result_id = NodeId.of("trac_build_result", job_namespace, cfg.JobResult)
 
         if objects is not None:
 
             results_inputs = set(objects.values())
 
-            if attrs is not None:
-                results_inputs.update(attrs.values())
-
             build_result_node = BuildJobResultNode(
                 build_result_id, job_config.jobId,
-                objects=objects, attrs=attrs, explicit_deps=explicit_deps)
+                objects=objects, explicit_deps=explicit_deps)
 
         elif bundles is not None:
 
             results_inputs = set(bundles)
 
             build_result_node = BuildJobResultNode(
                 build_result_id, job_config.jobId,
@@ -381,14 +387,15 @@
 
         # Generate a name for a new unique sub-context
 
         sub_namespace_name = f"{model_or_flow.objectType.name} = {model_or_flow_name}"
         sub_namespace = NodeNamespace(sub_namespace_name, namespace)
 
         # Execute in the sub-context by doing PUSH, EXEC, POP
+        # Note that POP node must be in the sub namespace too
 
         push_section = cls.build_context_push(
             sub_namespace, input_mapping,
             explicit_deps)
 
         exec_section = cls.build_model_or_flow(
             job_config, sub_namespace, model_or_flow,
@@ -447,28 +454,31 @@
         model_id = NodeId(model_name, namespace, Bundle[_data.DataView])
 
         model_node = RunModelNode(
             model_id, model_scope, model_def,
             frozenset(parameter_ids), frozenset(input_ids),
             explicit_deps=explicit_deps, bundle=model_id.namespace)
 
-        nodes = {model_id: model_node}
+        module_result_id = NodeId(f"{model_name}:RESULT", namespace)
+        model_result_node = RunModelResultNode(module_result_id, model_id)
+
+        nodes = {model_id: model_node, module_result_id: model_result_node}
 
         # Create nodes for each model output
         # The model node itself outputs a bundle (dictionary of named outputs)
         # These need to be mapped to individual nodes in the graph
 
         # These output mapping nodes are closely tied to the representation of the model itself
         # In the future, we may want models to emit individual outputs before the whole model is complete
 
         for output_id in output_ids:
             nodes[output_id] = BundleItemNode(output_id, model_id, output_id.name)
 
         # Assemble a graph to include the model and its outputs
-        return GraphSection(nodes, inputs={*parameter_ids, *input_ids}, outputs=output_ids, must_run=[model_id])
+        return GraphSection(nodes, inputs={*parameter_ids, *input_ids}, outputs=output_ids, must_run=[module_result_id])
 
     @classmethod
     def build_flow(
             cls, job_config: config.JobConfig, namespace: NodeNamespace,
             flow_def: meta.FlowDefinition,
             explicit_deps: tp.Optional[tp.List[NodeId]] = None) \
             -> GraphSection:
@@ -520,15 +530,18 @@
                     target_edges_.remove(edge)
 
                     if len(target_edges_) == 0:
                         target_node = remaining_nodes.pop(target_node_name)
                         reachable_nodes[target_node_name] = target_node
 
         if any(remaining_nodes):
-            raise _ex.ETracInternal()  # todo: cyclic / unmet dependencies
+            missing_targets = [edge.target for node in remaining_edges_by_target.values() for edge in node]
+            missing_target_names = [f"{t.node}.{t.socket}" if t.socket else t.node for t in missing_targets]
+            missing_nodes = list(map(lambda n: NodeId(n, namespace), missing_target_names))
+            cls._invalid_graph_error(missing_nodes)
 
         return graph_section
 
     @classmethod
     def build_flow_node(
             cls, job_config: config.JobConfig, namespace: NodeNamespace,
             target_edges: tp.Dict[meta.FlowSocket, meta.FlowEdge],
@@ -652,28 +665,51 @@
 
         n_sections = len(sections)
         first_section = sections[0]
         last_section = sections[-1]
 
         nodes = {**first_section.nodes}
         inputs = set(first_section.inputs)
-        must_run = first_section.must_run or []
+        must_run = list(first_section.must_run) if first_section.must_run else []
 
         for i in range(1, n_sections):
 
             current_section = sections[i]
 
             requirements_not_met = set(filter(
                 lambda n: n not in nodes,
                 current_section.inputs))
 
             if any(requirements_not_met):
                 if allow_partial_inputs:
                     inputs.update(requirements_not_met)
                 else:
-                    err = ', '.join(map(str, requirements_not_met))
-                    raise _ex.ETracInternal(err)  # todo inconsistent graph
+                    cls._invalid_graph_error(requirements_not_met)
 
             nodes.update(current_section.nodes)
+
+            must_run = list(filter(lambda n: n not in current_section.inputs, must_run))
             must_run.extend(current_section.must_run)
 
         return GraphSection(nodes, inputs, last_section.outputs, must_run)
+
+    @classmethod
+    def _invalid_graph_error(cls, missing_dependencies: tp.Iterable[NodeId]):
+
+        missing_ids = ", ".join(map(cls._missing_item_display_name, missing_dependencies))
+        message = f"Invalid job config: The execution graph has unsatisfied dependencies: [{missing_ids}]"
+
+        raise _ex.EJobValidation(message)
+
+    @classmethod
+    def _missing_item_display_name(cls, node_id: NodeId):
+
+        components = node_id.namespace.components()
+
+        # The execution graph is built for an individual job, so the top-level namespace is always the job key
+        # Do not list the job key component with every missing node, that would be overly verbose
+        # If we ever start using global resources (to share between jobs), this logic may need to change
+
+        if len(components) <= 1:
+            return node_id.name
+        else:
+            return f"{node_id.name} / {', '.join(components[:-1])}"
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_exec/runtime.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_exec/runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,35 +21,43 @@
 import sys
 import pathlib
 import tempfile
 import typing as tp
 
 import tracdap.rt.api as _api
 import tracdap.rt.config as _cfg
-import tracdap.rt._version as _version
 import tracdap.rt.exceptions as _ex
+import tracdap.rt.ext.plugins as _plugins
 import tracdap.rt._exec.actors as _actors
 import tracdap.rt._exec.engine as _engine
 import tracdap.rt._exec.dev_mode as _dev_mode
 import tracdap.rt._impl.config_parser as _cparse  # noqa
-import tracdap.rt._impl.util as util  # noqa
+import tracdap.rt._impl.util as _util  # noqa
 import tracdap.rt._impl.models as _models  # noqa
 import tracdap.rt._impl.storage as _storage  # noqa
 import tracdap.rt._impl.static_api as _static_api  # noqa
+import tracdap.rt._impl.guard_rails as _guard  # noqa
+import tracdap.rt._version as _version
 
 
 @dc.dataclass
 class _RuntimeJobInfo:
     done: bool = dc.field(default=False)
     result: _cfg.JobResult = dc.field(default=None)
     error: Exception = dc.field(default=None)
 
 
 class TracRuntime:
 
+    # Basic configuration of engine threads
+    __THREAD_POOL_CONFIG = {"model": 1, "data": 3}
+    __THREAD_POOL_MAPPING = {
+        _engine.ModelNodeProcessor: "model",
+        _engine.DataNodeProcessor: "data"}
+
     def __init__(
             self,
             sys_config: tp.Union[str, pathlib.Path, _cfg.RuntimeConfig],
             job_result_dir: tp.Union[str, pathlib.Path, None] = None,
             job_result_format: tp.Optional[str] = None,
             scratch_dir: tp.Union[str, pathlib.Path, None] = None,
             scratch_dir_persist: bool = False,
@@ -66,16 +74,16 @@
 
         if dev_mode:
             print(f">>> Development mode enabled (DO NOT USE THIS IN PRODUCTION)")
 
         if isinstance(scratch_dir, str):
             scratch_dir = pathlib.Path(scratch_dir)
 
-        util.configure_logging()
-        self._log = util.logger_for_object(self)
+        _util.configure_logging()
+        self._log = _util.logger_for_object(self)
         self._log.info(f"TRAC D.A.P. Python Runtime {trac_version}")
 
         self._sys_config = sys_config if isinstance(sys_config, _cfg.RuntimeConfig) else None
         self._sys_config_path = pathlib.Path(sys_config) if not self._sys_config else None
         self._job_result_dir = job_result_dir
         self._job_result_format = job_result_format
         self._scratch_dir = scratch_dir
@@ -115,19 +123,23 @@
 
             self._log.info(f"Beginning pre-start sequence...")
 
             # Scratch dir is needed during pre-start (at least dev mode translation uses the model loader)
 
             self._prepare_scratch_dir()
 
-            # Plugins will be loaded here, before config
+            # Plugin manager and static API impl are singletons
+            # If these methods are called multiple times, the second and subsequent calls are ignored
 
+            _plugins.PluginManager.register_core_plugins()
             _static_api.StaticApiImpl.register_impl()
+            _guard.PythonGuardRails.protect_dangerous_functions()
 
-            # Load sys and job config (or use embedded)
+            # Load sys config (or use embedded), config errors are detected before start()
+            # Job config can also be checked before start() by using load_job_config()
 
             if self._sys_config is None:
                 sys_config_dev_mode = _dev_mode.DEV_MODE_SYS_CONFIG if self._dev_mode else None
                 sys_config_parser = _cparse.ConfigParser(_cfg.RuntimeConfig, sys_config_dev_mode)
                 sys_config_raw = sys_config_parser.load_raw_config(self._sys_config_path, config_file_name="system")
                 self._sys_config = sys_config_parser.parse(sys_config_raw, self._sys_config_path)
             else:
@@ -152,15 +164,19 @@
             self._models = _models.ModelLoader(self._sys_config, self._scratch_dir)
             self._storage = _storage.StorageManager(self._sys_config)
 
             self._engine = _engine.TracEngine(
                 self._sys_config, self._models, self._storage,
                 notify_callback=self._engine_callback)
 
-            self._system = _actors.ActorSystem(self._engine, system_thread="engine")
+            self._system = _actors.ActorSystem(
+                self._engine, system_thread="engine",
+                thread_pools=self.__THREAD_POOL_CONFIG,
+                thread_pool_mapping=self.__THREAD_POOL_MAPPING)
+
             self._system.start(wait=wait)
 
         except Exception as e:
             self._handle_startup_error(e)
 
     def stop(self, due_to_error=False):
 
@@ -214,15 +230,15 @@
             write_test_path.unlink()
         except Exception:
             raise _ex.EStartup(f"Scratch directory [{self._scratch_dir}] is not writable")
 
     def _clean_scratch_dir(self):
 
         if not self._scratch_dir_persist:
-            util.try_clean_dir(self._scratch_dir, remove=(not self._scratch_dir_provided))
+            _util.try_clean_dir(self._scratch_dir, remove=(not self._scratch_dir_provided))
 
     # ------------------------------------------------------------------------------------------------------------------
     # Job submission
     # ------------------------------------------------------------------------------------------------------------------
 
     def load_job_config(
             self, job_config: tp.Union[str, pathlib.Path, _cfg.JobConfig],
@@ -246,25 +262,25 @@
                 self._scratch_dir, config_dir,
                 model_class)
 
         return job_config
 
     def submit_job(self, job_config: _cfg.JobConfig):
 
-        job_key = util.object_key(job_config.jobId)
+        job_key = _util.object_key(job_config.jobId)
         self._jobs[job_key] = _RuntimeJobInfo()
 
         self._system.send(
             "submit_job", job_config,
             str(self._job_result_dir) if self._job_result_dir else "",
             self._job_result_format if self._job_result_format else "")
 
     def wait_for_job(self, job_id: _api.TagHeader):
 
-        job_key = util.object_key(job_id)
+        job_key = _util.object_key(job_id)
 
         if job_key not in self._jobs:
             raise _ex.ETracInternal(f"Attempt to wait for a job that was never started")
 
         with self._engine_event:
             while True:
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_impl/__init__.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_impl/config_parser.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/config_parser.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_impl/csv_codec.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/format_csv.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022 Accenture Global Solutions Limited
+#  Copyright 2023 Accenture Global Solutions Limited
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,34 +19,43 @@
 import csv
 import typing as tp
 
 import pyarrow as pa
 import pyarrow.compute as pac
 import pyarrow.csv as pa_csv
 
-import tracdap.rt.exceptions as _ex
-import tracdap.rt._impl.data as _data
-import tracdap.rt._impl.util as _util
+import tracdap.rt.ext.plugins as plugins
+import tracdap.rt.exceptions as ex
 
 # Import storage interfaces
 from tracdap.rt.ext.storage import IDataFormat
 
+# Set of common helpers across the core plugins (do not reference rt._impl)
+from . import _helpers
+
+# TODO: Remove dependency on internal code
+import tracdap.rt._impl.data as _data
+
 
 class CsvStorageFormat(IDataFormat):
 
+    FORMAT_CODE = "CSV"
+    FILE_EXTENSION = "csv"
+
     __LENIENT_CSV_PARSER = "lenient_csv_parser"
+    __LENIENT_MISSING_COLUMNS = "lenient_missing_columns"
     __DATE_FORMAT = "date_format"
     __DATETIME_FORMAT = "datetime_format"
 
     __TRUE_VALUES = ['true', 't', 'yes' 'y', '1']
     __FALSE_VALUES = ['false', 'f', 'no' 'n', '0']
 
     def __init__(self, format_options: tp.Dict[str, tp.Any] = None):
 
-        self._log = _util.logger_for_object(self)
+        self._log = _helpers.logger_for_object(self)
 
         self._format_options = format_options
         self._use_lenient_parser = False
         self._date_format = None
         self._datetime_format = None
 
         if format_options:
@@ -71,42 +80,48 @@
 
         if isinstance(lenient_flag, str):
             if lenient_flag.lower() == "false":
                 return False
             if lenient_flag.lower() == "true":
                 return True
 
-        raise _ex.EConfigParse(f"Invalid lenient flag for CSV storage: [{lenient_flag}]")
+        raise ex.EConfigParse(f"Invalid lenient flag for CSV storage: [{lenient_flag}]")
 
     @classmethod
     def _validate_date_format(cls, date_format: str):
 
         try:
             current_date = dt.datetime.now().date()
             current_date.strftime(date_format)
             return date_format
         except EncodingWarning:
-            raise _ex.EConfigParse(f"Invalid date format for CSV storage: [{date_format}]")
+            raise ex.EConfigParse(f"Invalid date format for CSV storage: [{date_format}]")
 
     @classmethod
     def _validate_datetime_format(cls, datetime_format: str):
 
         try:
             current_datetime = dt.datetime.now()
             current_datetime.strftime(datetime_format)
             return datetime_format
         except EncodingWarning:
-            raise _ex.EConfigParse(f"Invalid datetime format for CSV storage: [{datetime_format}]")
+            raise ex.EConfigParse(f"Invalid datetime format for CSV storage: [{datetime_format}]")
+
+    def format_code(self) -> str:
+        return self.FORMAT_CODE
+
+    def file_extension(self) -> str:
+        return self.FILE_EXTENSION
 
     def read_table(self, source: tp.BinaryIO, schema: tp.Optional[pa.Schema]) -> pa.Table:
 
         # For CSV data, if there is no schema then type inference will do unpredictable things!
 
         if schema is None or len(schema.names) == 0 or len(schema.types) == 0:
-            raise _ex.EDataConformance("An explicit schema is required to load CSV data")
+            raise ex.EDataConformance("An explicit schema is required to load CSV data")
 
         if self._use_lenient_parser:
             return self._read_table_lenient(source, schema)
         else:
             return self._read_table_arrow(source, schema)
 
     def write_table(self, target: tp.Union[str, pathlib.Path, tp.BinaryIO], table: pa.Table):
@@ -139,21 +154,21 @@
             convert_options.quoted_strings_can_be_null = False
 
             return pa_csv.read_csv(source, read_options, parse_options, convert_options)
 
         except pa.ArrowInvalid as e:
             err = f"CSV file decoding failed, content is garbled"
             self._log.exception(err)
-            raise _ex.EDataCorruption(err) from e
+            raise ex.EDataCorruption(err) from e
 
         except pa.ArrowKeyError as e:
             err = f"CSV file decoding failed, one or more columns is missing"
             self._log.error(err)
             self._log.exception(str(e))
-            raise _ex.EDataCorruption(err) from e
+            raise ex.EDataCorruption(err) from e
 
     @classmethod
     def _format_outputs(cls, table: pa.Table) -> pa.Table:
 
         for column_index in range(table.num_columns):
 
             column: pa.Array = table.column(column_index)
@@ -222,15 +237,15 @@
             return decimal_str.rstrip('0').rstrip('.')
 
         return pa.array(map(format_decimal, column), pa.utf8())
 
     @classmethod
     def _format_timestamp(cls, column: pa.Array) -> pa.Array:
 
-        # PyArrow outputs timestamps with a space (' ') separator between date and time
+        # PyArrow outputs timestamps with a space ' ' separator between date and time
         # ISO format requires a 'T' between date and time
 
         column_type: pa.TimestampType = column.type
 
         if column_type.unit == "s":
             timespec = 'seconds'
         elif column_type.unit == "ms":
@@ -251,94 +266,122 @@
 
         try:
 
             stream_reader = codecs.getreader('utf-8')
             text_source = stream_reader(source)
 
             csv_params = {
-                "skipinitialspace": True,
-                "doublequote": True
+                "skipinitialspace": True,  # noqa
+                "doublequote": True  # noqa
             }
 
             csv_reader = csv.reader(text_source, **csv_params)
-            header = next(csv_reader)
 
+            header = next(csv_reader)
             header_lower = list(map(str.lower, header))
+
+            schema_columns = dict((col.lower(), index) for index, col in enumerate(schema.names))
+
+            lenient_columns = _helpers.get_plugin_property(self._format_options, self.__LENIENT_MISSING_COLUMNS)
             missing_columns = list(filter(lambda col_: col_.lower() not in header_lower, schema.names))
 
+            # The lenient_missing_columns flag allows missing columns so long as they are nullable
+            # Primarily intended for reading schema files if not all the columns are needed
             if any(missing_columns):
-                msg = f"CSV data is missing one or more columns: [{', '.join(missing_columns)}]"
-                self._log.error(msg)
-                raise _ex.EDataConformance(msg)
 
-            schema_columns = {col.lower(): index for index, col in enumerate(schema.names)}
+                if not lenient_columns:
+                    msg = f"CSV data is missing one or more columns: [{', '.join(missing_columns)}]"
+                    self._log.error(msg)
+                    raise ex.EDataConformance(msg)
+
+                missing_not_null = list(filter(lambda col: not schema.field(col).nullable, missing_columns))
+
+                if any(missing_not_null):
+                    msg = f"CSV data is missing one or more not-null columns: [{', '.join(missing_not_null)}]"
+                    self._log.error(msg)
+                    raise ex.EDataConformance(msg)
+
+            # Set up column mappings using field indices (avoid string lookups in the loop)
+
             col_mapping = [schema_columns.get(col) for col in header_lower]
             python_types = list(map(_data.DataMapping.arrow_to_python_type, schema.types))
             nullable_flags = list(map(lambda c: schema.field(c).nullable, range(len(schema.names))))
 
             data = [[] for _ in range(len(schema.names))]
             csv_row = 1  # Allowing for header
             csv_col = 0
 
             for row in csv_reader:
 
+                # Extra values in the row is an error, they don't belong to any column
+                if len(row) > len(header):
+                    err = f"CSV decoding failed, unexpected extra columns on row [{csv_row}]"
+                    self._log.exception(err)
+                    raise ex.EDataCorruption(err)
+
+                # Missing values at the end of the row are filled with blanks/nulls
+                # This is only valid if the missing fields are nullable or of string type
+                if len(row) < len(header):
+                    null_values = ["" for _ in range(len(header) - len(row))]
+                    row = row + null_values
+
                 for raw_value in row:
 
                     col_name = header[csv_col]
                     output_col = col_mapping[csv_col]
 
                     if output_col is not None:
                         python_type = python_types[output_col]
                         nullable = nullable_flags[output_col]
                         python_value = self._convert_python_value(raw_value, python_type, nullable, csv_row, col_name)
                         data[output_col].append(python_value)
 
                     csv_col += 1
 
-                # Allow for trailing null columns
-                # TODO: What is the right behavior here? Use a flag to control?
-                for blank_col in range(csv_col, len(header)):
-                    output_col = col_mapping[blank_col]
-                    data[output_col].append(None)  # noqa
-
                 csv_col = 0
                 csv_row += 1
 
             data_dict = dict(zip(schema.names, data))
+
+            # In lenient column mode, fill in any missing nullable columns with nulls
+            if lenient_columns:
+                for output_col in missing_columns:
+                    data_dict[output_col] = list(None for _ in range(csv_row - 1))
+
             table = pa.Table.from_pydict(data_dict, schema)  # noqa
 
             return table
 
         except StopIteration as e:
             err = f"CSV decoding failed, no readable content"
             self._log.exception(err)
-            raise _ex.EDataCorruption(err) from e
+            raise ex.EDataCorruption(err) from e
 
         except UnicodeDecodeError as e:
             err = f"CSV decoding failed, content is garbled"
             self._log.exception(err)
-            raise _ex.EDataCorruption(err) from e
+            raise ex.EDataCorruption(err) from e
 
     def _convert_python_value(
             self, raw_value: tp.Any, python_type: type, nullable: bool,
             row: int, col: str) -> tp.Any:
 
         try:
 
             # Python's csv.reader does not know the difference between empty string and null
 
             if raw_value is None or (isinstance(raw_value, str) and raw_value == ""):
                 if python_type == str:
-                    return raw_value
+                    return raw_value if nullable else ""
                 if nullable:
                     return None
                 else:
                     msg = f"CSV data contains null value for a not-null field (col = {col}, row = {row})"
                     self._log.error(msg)
-                    raise _ex.EDataConformance(msg)
+                    raise ex.EDataConformance(msg)
 
             if isinstance(raw_value, python_type):
                 return raw_value
 
             if python_type == bool:
                 if isinstance(raw_value, str):
                     if raw_value.lower() in self.__TRUE_VALUES:
@@ -348,15 +391,15 @@
                 if isinstance(raw_value, int) or isinstance(raw_value, float):
                     if raw_value == 1:
                         return True
                     if raw_value == 0:
                         return False
 
             if python_type == int:
-                if isinstance(raw_value, float):
+                if isinstance(raw_value, float) and raw_value.is_integer():
                     return int(raw_value)
                 if isinstance(raw_value, str):
                     return int(raw_value)
 
             if python_type == float:
                 if isinstance(raw_value, int):
                     return float(raw_value)
@@ -391,16 +434,21 @@
         except Exception as e:
 
             msg = f"CSV data does not match the schema and cannot be converted" \
                 + f" (col = {col}, row = {row}, expected type = [{python_type.__name__}], value = [{str(raw_value)}])" \
                 + f": {str(e)}"
 
             self._log.exception(msg)
-            raise _ex.EDataConformance(msg) from e
+            raise ex.EDataConformance(msg) from e
 
         # Default case: unrecognized python_type
 
         msg = f"CSV data does not match the schema and cannot be converted" \
               + f" (col = {col}, row = {row}, expected type = [{python_type.__name__}], value = [{str(raw_value)}])"
 
         self._log.error(msg)
-        raise _ex.EDataConformance(msg)
+        raise ex.EDataConformance(msg)
+
+
+plugins.PluginManager.register_plugin(
+    IDataFormat, CsvStorageFormat,
+    ["CSV", ".csv", "text/csv"])
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_impl/data.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,21 +200,27 @@
 
     @classmethod
     def trac_to_arrow_schema(cls, trac_schema: _meta.SchemaDefinition) -> pa.Schema:
 
         if trac_schema.schemaType != _meta.SchemaType.TABLE:
             raise _ex.ETracInternal(f"Schema type [{trac_schema.schemaType}] cannot be converted for Apache Arrow")
 
-        arrow_fields = [
-            (f.fieldName, cls.trac_to_arrow_basic_type(f.fieldType))
-            for f in trac_schema.table.fields]
+        arrow_fields = list(map(cls.trac_to_arrow_field, trac_schema.table.fields))
 
         return pa.schema(arrow_fields, metadata={})
 
     @classmethod
+    def trac_to_arrow_field(cls, trac_field: _meta.FieldSchema):
+
+        arrow_type = cls.trac_to_arrow_basic_type(trac_field.fieldType)
+        nullable = not trac_field.notNull if trac_field.notNull is not None else not trac_field.businessKey
+
+        return pa.field(trac_field.fieldName, arrow_type, nullable)
+
+    @classmethod
     def trac_arrow_decimal_type(cls) -> pa.Decimal128Type:
 
         return pa.decimal128(
             cls.__TRAC_DECIMAL_PRECISION,
             cls.__TRAC_DECIMAL_SCALE)
 
     @classmethod
@@ -528,15 +534,15 @@
 
     @classmethod
     def _coerce_vector(cls, vector: pa.Array, field: pa.Field, pandas_type=None) -> pa.Array:
 
         if pa.types.is_null(vector.type):
 
             if field.nullable:
-                return pa.array([], type=field.type, size=len(vector))
+                return pa.nulls(size=len(vector), type=field.type)
             else:
                 raise _ex.EDataConformance(f"All null values in non-null field [{field.name}]")
 
         if pa.types.is_boolean(field.type):
             return cls._coerce_boolean(vector, field)
 
         if pa.types.is_integer(field.type):
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_impl/models.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -75,54 +75,87 @@
         del self.__scopes[scope]
 
         # Do not delete scope scratch dir here
         # The top level scratch dir is cleaned up on exit, depending on the --scratch-dir-persist flag
         # If the flag is set, all scratch content should be left behind
         # This can be for debugging, or because the scratch data is written to an ephemeral volume
 
-    def load_model_class(self, scope: str, model_def: _meta.ModelDefinition) -> _api.TracModel.__class__:
+    @staticmethod
+    def model_checkout_key(model_def: _meta.ModelDefinition):
 
-        scope_state = self.__scopes[scope]
+        # The "packageGroup" field is optional and may not be present for some repo types
+        # The "package" field remains optional until the 0.6 metadata upgrade
 
-        model_key = f"{model_def.repository}#{model_def.path}#{model_def.version}#{model_def.entryPoint}"
-        model_class = scope_state.model_cache.get(model_key)
+        group = model_def.packageGroup or "-"
+        package = model_def.package or "-"
+        version = model_def.version
 
-        if model_class is not None:
-            return model_class
-
-        self.__log.info(f"Loading model [{model_def.entryPoint}] (version=[{model_def.version}], scope=[{scope}])...")
+        return f"{group}/{package}/{version}"
 
+    def _get_checkout_dir(self, scope: str, model_def: _meta.ModelDefinition):
+        scope_state = self.__scopes[scope]
         repo = self.__repos.get_repository(model_def.repository)
-        checkout_key = repo.checkout_key(model_def)
+        checkout_key = self.model_checkout_key(model_def)
         checkout_subdir = pathlib.Path(checkout_key)
 
-        # Make sure the checkout key is safe to use as a directory name
-
         if checkout_subdir.is_absolute() or checkout_subdir.is_reserved():
 
             msg = f"Checkout failed: Invalid checkout key [{checkout_key}] in repo [{model_def.repository}]" + \
                   f" (type: {type(repo).__name__})"
 
             self.__log.error(msg)
             raise _ex.EUnexpected(msg)
 
-        # If the repo/checkout already exists in the code cache, we can use the existing checkout and package dir
-
         code_cache_key = f"{model_def.repository}#{checkout_key}"
 
         if code_cache_key in scope_state.code_cache:
             checkout_dir = scope_state.code_cache[code_cache_key]
-            package_dir = repo.package_path(model_def, checkout_dir)
 
         # Otherwise, we need to run the checkout, and store the checkout dir into the code cache
         # What gets cached is the checkout, which may contain multiple packages depending on the repo type
 
         else:
             scope_dir = scope_state.scratch_dir
             checkout_dir = scope_dir.joinpath(model_def.repository, checkout_subdir)
+
+        return checkout_dir
+
+    def model_load_checkout_directory(self, scope: str, model_def: _meta.ModelDefinition) -> pathlib.Path:
+
+        repo = self.__repos.get_repository(model_def.repository)
+        checkout_dir = self._get_checkout_dir(scope, model_def)
+
+        return repo.package_path(model_def, checkout_dir)
+
+    def load_model_class(self, scope: str, model_def: _meta.ModelDefinition) -> _api.TracModel.__class__:
+
+        checkout_dir = self._get_checkout_dir(scope, model_def)
+        scope_state = self.__scopes[scope]
+        model_key = f"{model_def.repository}#{model_def.path}#{model_def.version}#{model_def.entryPoint}"
+        model_class = scope_state.model_cache.get(model_key)
+
+        if model_class is not None:
+            return model_class
+
+        self.__log.info(f"Loading model [{model_def.entryPoint}] (version=[{model_def.version}], scope=[{scope}])...")
+
+        repo = self.__repos.get_repository(model_def.repository)
+        checkout_key = self.model_checkout_key(model_def)
+
+        # If the repo/checkout already exists in the code cache, we can use the existing checkout and package dir
+
+        code_cache_key = f"{model_def.repository}#{checkout_key}"
+
+        if code_cache_key in scope_state.code_cache:
+            package_dir = repo.package_path(model_def, checkout_dir)
+
+        # Otherwise, we need to run the checkout, and store the checkout dir into the code cache
+        # What gets cached is the checkout, which may contain multiple packages depending on the repo type
+
+        else:
             checkout_dir.mkdir(mode=0o750, parents=True, exist_ok=False)
             package_dir = repo.do_checkout(model_def, checkout_dir)
 
             scope_state.code_cache[code_cache_key] = checkout_dir
 
         # For the integrated repo (i.e. model code in PYTHONPATH), do not use a shim
         if package_dir is None:
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_impl/repos.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/repo_pypi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,235 +1,41 @@
-#  Copyright 2022 Accenture Global Solutions Limited
+#  Copyright 2023 Accenture Global Solutions Limited
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from __future__ import annotations
-
 import html.parser
 import json.decoder
+import pathlib
 import re
-import subprocess
-import subprocess as sp
+import typing as tp
 import urllib.parse
-import time
 import zipfile
 import io
 
 import requests
 
-import tracdap.rt.metadata as _meta
-import tracdap.rt.config as _cfg
-import tracdap.rt.exceptions as _ex
-import tracdap.rt._impl.util as _util
+import tracdap.rt.metadata as meta
+import tracdap.rt.exceptions as ex
 
 # Import repo interfaces
+import tracdap.rt.ext.plugins as plugins
 from tracdap.rt.ext.repos import *
 
-
-# Helper functions for handling credentials supplied via HTTP(S) URLs
-
-__REPO_TOKEN_KEY = "token"
-__REPO_USER_KEY = "username"
-__REPO_PASS_KEY = "password"
-
-
-def _get_credentials(url: urllib.parse.ParseResult, plugin_config: _cfg.PluginConfig):
-
-    token = _util.get_plugin_property(plugin_config, __REPO_TOKEN_KEY)
-    username = _util.get_plugin_property(plugin_config, __REPO_USER_KEY)
-    password = _util.get_plugin_property(plugin_config, __REPO_PASS_KEY)
-
-    if token is not None:
-        return token
-
-    if username is not None and password is not None:
-        return f"{username}:{password}"
-
-    if url.username:
-        credentials_sep = url.netloc.index("@")
-        return url.netloc[:credentials_sep]
-
-    return None
-
-
-def _apply_credentials(url: urllib.parse.ParseResult, credentials: str):
-
-    if credentials is None:
-        return url
-
-    if url.username is None:
-        location = f"{credentials}@{url.netloc}"
-
-    else:
-        location_sep = url.netloc.index("@")
-        location = f"{credentials}@{url.netloc[location_sep + 1:]}"
-
-    return url._replace(netloc=location)
-
-
-class IntegratedSource(IModelRepository):
-
-    def __init__(self, repo_config: _cfg.PluginConfig):
-        self._repo_config = repo_config
-
-    def checkout_key(self, model_def: _meta.ModelDefinition):
-        return "trac_integrated"
-
-    def package_path(
-            self, model_def: _meta.ModelDefinition,
-            checkout_dir: pathlib.Path) -> tp.Optional[pathlib.Path]:
-
-        return None
-
-    def do_checkout(
-            self, model_def: _meta.ModelDefinition,
-            checkout_dir: tp.Union[str, pathlib.Path]) \
-            -> None:
-
-        # For the integrated repo there is nothing to check out
-
-        return self.package_path(model_def, checkout_dir)
-
-
-class LocalRepository(IModelRepository):
-
-    REPO_URL_KEY = "repoUrl"
-
-    def __init__(self, repo_config: _cfg.PluginConfig):
-        self._repo_config = repo_config
-        self._repo_url = _util.get_plugin_property(self._repo_config, self.REPO_URL_KEY)
-
-        if not self._repo_url:
-            raise _ex.EConfigParse(f"Missing required property [{self.REPO_URL_KEY}] in local repository config")
-
-    def checkout_key(self, model_def: _meta.ModelDefinition):
-        return "trac_local"
-
-    def package_path(
-            self, model_def: _meta.ModelDefinition,
-            checkout_dir: pathlib.Path) -> tp.Optional[pathlib.Path]:
-
-        checkout_path = pathlib.Path(self._repo_url).joinpath(model_def.path)
-
-        return checkout_path
-
-    def do_checkout(self, model_def: _meta.ModelDefinition, checkout_dir: pathlib.Path) -> pathlib.Path:
-
-        # For local repos, checkout is a no-op since the model is already local
-        # Just return the existing package path
-
-        return self.package_path(model_def, checkout_dir)
-
-
-class GitRepository(IModelRepository):
-
-    REPO_URL_KEY = "repoUrl"
-    GIT_TIMEOUT_SECONDS = 30
-
-    def __init__(self, repo_config: _cfg.PluginConfig):
-
-        self._repo_config = repo_config
-        self._log = _util.logger_for_object(self)
-
-        repo_url_prop = _util.get_plugin_property(self._repo_config, self.REPO_URL_KEY)
-
-        if not repo_url_prop:
-            raise _ex.EConfigParse(f"Missing required property [{self.REPO_URL_KEY}] in Git repository config")
-
-        repo_url = urllib.parse.urlparse(repo_url_prop)
-        credentials = _get_credentials(repo_url, repo_config)
-
-        self._repo_url = _apply_credentials(repo_url, credentials)
-
-    def checkout_key(self, model_def: _meta.ModelDefinition):
-        return model_def.version
-
-    def package_path(
-            self, model_def: _meta.ModelDefinition,
-            checkout_dir: pathlib.Path) -> tp.Optional[pathlib.Path]:
-
-        return checkout_dir.joinpath(model_def.path)
-
-    def do_checkout(self, model_def: _meta.ModelDefinition, checkout_dir: pathlib.Path) -> pathlib.Path:
-
-        self._log.info(
-            f"Git checkout: repo = [{model_def.repository}], " +
-            f"group = [{model_def.packageGroup}], package = [{model_def.package}], version = [{model_def.version}]")
-
-        self._log.info(f"Checkout location: [{checkout_dir}]")
-
-        git_cli = ["git", "-C", str(checkout_dir)]
-
-        git_cmds = [
-            ["init"],
-            ["remote", "add", "origin", self._repo_url.geturl()],
-            ["fetch", "--depth=1", "origin", model_def.version],
-            ["reset", "--hard", "FETCH_HEAD"]]
-
-        # Work around Windows issues
-        if _util.is_windows():
-
-            # Some machines may still be setup without long path support in Windows and/or the Git client
-            # Workaround: Enable the core.longpaths flag for each individual Git command (do not rely on system config)
-            git_cli += ["-c", "core.longpaths=true"]
-
-            # On some systems, directories created by the TRAC runtime process may not be owned by the process owner
-            # This will cause Git to report an unsafe repo directory
-            # Finding the current owner requires either batch scripting or using the win32_api package
-            # Workaround: Explicitly take ownership of the repo directory, always, before starting the checkout
-            try:
-                self._log.info(f"Fixing filesystem permissions for [{checkout_dir}]")
-                subprocess.run(f"takeown /f \"{checkout_dir}\"")
-            except Exception:  # noqa
-                self._log.info(f"Failed to fix filesystem permissions, this might prevent checkout from succeeding")
-
-        for git_cmd in git_cmds:
-
-            safe_cmd = map(_util.log_safe, git_cmd)
-            self._log.info(f"git {' '.join(safe_cmd)}")
-
-            cmd = [*git_cli, *git_cmd]
-            cmd_result = sp.run(cmd, cwd=checkout_dir, stdout=sp.PIPE, stderr=sp.PIPE, timeout=self.GIT_TIMEOUT_SECONDS)
-
-            if cmd_result.returncode != 0:
-                time.sleep(1)
-                self._log.warning(f"git {' '.join(git_cmd)} (retrying)")
-                cmd_result = sp.run(cmd, cwd=checkout_dir, stdout=sp.PIPE, stderr=sp.PIPE, timeout=self.GIT_TIMEOUT_SECONDS)  # noqa
-
-            cmd_out = str(cmd_result.stdout, 'utf-8').splitlines()
-            cmd_err = str(cmd_result.stderr, 'utf-8').splitlines()
-
-            for line in cmd_out:
-                self._log.info(line)
-
-            if cmd_result.returncode == 0:
-                for line in cmd_err:
-                    self._log.info(line)
-
-            else:
-                for line in cmd_err:
-                    self._log.error(line)
-
-                error_msg = f"Git checkout failed for {model_def.package} {model_def.version}"
-                self._log.error(error_msg)
-                raise _ex.EModelRepo(error_msg)
-
-        self._log.info(f"Git checkout succeeded for {model_def.package} {model_def.version}")
-
-        return self.package_path(model_def, checkout_dir)
+# Set of common helpers across the core plugins (do not reference rt._impl)
+from . import _helpers
 
 
 class PyPiRepository(IModelRepository):
 
     SIMPLE_PACKAGE_PATH = "{}/{}/"
     JSON_PACKAGE_PATH = "{}/{}/{}/json"
 
@@ -245,53 +51,50 @@
         PIP_SIMPLE_FORMAT_JSON: "application/vnd.pypi.simple.v1+json",
         PIP_SIMPLE_FORMAT_HTML: "text/html"
     }
 
     PIP_SIMPLE_TYPE_JSON = "application/vnd.pypi.simple.v1+json"
     PIP_SIMPLE_TYPE_HTML = "text/html"
 
-    def __init__(self, repo_config: _cfg.PluginConfig):
+    def __init__(self, properties: tp.Dict[str, str]):
 
-        self._log = _util.logger_for_object(self)
+        self._log = _helpers.logger_for_object(self)
 
-        self._repo_config = repo_config
+        self._properties = properties
 
-        self._pip_index = _util.get_plugin_property(self._repo_config, self.PIP_INDEX_KEY)
-        self._pip_index_url = _util.get_plugin_property(self._repo_config, self.PIP_INDEX_URL_KEY)
-        self._pip_simple_format = _util.get_plugin_property(self._repo_config, self.PIP_SIMPLE_FORMAT_KEY)
+        self._pip_index = _helpers.get_plugin_property(self._properties, self.PIP_INDEX_KEY)
+        self._pip_index_url = _helpers.get_plugin_property(self._properties, self.PIP_INDEX_URL_KEY)
+        self._pip_simple_format = _helpers.get_plugin_property(self._properties, self.PIP_SIMPLE_FORMAT_KEY)
 
         if self._pip_index is None and self._pip_index_url is None:
             message = f"Neither [{self.PIP_INDEX_KEY}] nor [{self.PIP_INDEX_URL_KEY} is set in PyPi repository config"
-            raise _ex.EConfigParse(message)
-
-    def checkout_key(self, model_def: _meta.ModelDefinition):
-        return model_def.version
+            raise ex.EConfigParse(message)
 
     def package_path(
-            self, model_def: _meta.ModelDefinition,
-            checkout_dir: pathlib.Path) -> tp.Optional[pathlib.Path]:
+            self, model_def: meta.ModelDefinition,
+            checkout_dir: pathlib.Path) -> pathlib.Path:
 
         return checkout_dir
 
-    def do_checkout(self, model_def: _meta.ModelDefinition, checkout_dir: pathlib.Path) -> tp.Optional[pathlib.Path]:
+    def do_checkout(self, model_def: meta.ModelDefinition, checkout_dir: pathlib.Path) -> pathlib.Path:
 
         self._log.info(
             f"PyPI checkout: repo = [{model_def.repository}], " +
             f"package = [{model_def.package}], version = [{model_def.version}]")
 
         self._log.info(f"Checkout location: [{checkout_dir}]")
 
         if self._pip_index_url is not None:
             package_filename, package_url = self._pypi_simple_query(model_def)
 
         else:
             package_filename, package_url = self._pypi_json_query(model_def)
 
         self._log.info(f"Downloading [{package_filename}]")
-        self._log.info(f"GET: {_util.log_safe_url(package_url)}")
+        self._log.info(f"GET: {_helpers.log_safe_url(package_url)}")
 
         download_req = requests.get(package_url.geturl())
         content = download_req.content
         elapsed = download_req.elapsed
 
         self._log.info(f"Downloaded [{len(content) / 1024:.1f}] KB in [{elapsed.total_seconds():.1f}] seconds")
 
@@ -299,26 +102,26 @@
         download_whl.extractall(checkout_dir)
 
         self._log.info(f"Unpacked [{len(download_whl.filelist)}] files")
         self._log.info(f"PyPI checkout succeeded for {model_def.package} {model_def.version}")
 
         return self.package_path(model_def, checkout_dir)
 
-    def _pypi_simple_query(self, model_def: _meta.ModelDefinition):
+    def _pypi_simple_query(self, model_def: meta.ModelDefinition):
 
         # PEP describing PyPI simple protocol
         # https://peps.python.org/pep-0691/
 
         try:
 
             simple_root_url = urllib.parse.urlparse(self._pip_index_url)
             simple_content_type = self._pypi_simple_content_type()
             simple_headers = {"accept": simple_content_type}
 
-            credentials = _get_credentials(simple_root_url, self._repo_config)
+            credentials = _helpers.get_http_credentials(simple_root_url, self._properties)
 
             self._log.info(f"Query package: [{model_def.package}]")
 
             package_req = self._pypi_package_query(
                 self.SIMPLE_PACKAGE_PATH, simple_root_url, simple_headers,
                 credentials, model_def)
 
@@ -335,25 +138,25 @@
                 package_parser = _PypiSimpleHtmlParser(model_def.package, package_req.url)
                 package_parser.feed(package_req.text)
                 filename, url = self._pypi_simple_parse_response(model_def, package_parser.response)
 
             else:
                 err = f"Invalid response from package repository: Content type = [{received_content_type}]"
                 self._log.error(err)
-                raise _ex.EModelRepo(err)
+                raise ex.EModelRepo(err)
 
             package_url = urllib.parse.urlparse(url)
-            package_url = _apply_credentials(package_url, credentials)
+            package_url = _helpers.apply_http_credentials(package_url, credentials)
 
             return filename, package_url
 
         except json.JSONDecodeError as e:
             msg = f"Invalid response from model repository: {str(e)}"
             self._log.error(msg)
-            raise _ex.EModelRepo("Invalid response from model repository") from e
+            raise ex.EModelRepo("Invalid response from model repository") from e
 
     def _pypi_simple_content_type(self):
 
         if self._pip_simple_format in self.PIP_SIMPLE_CONTENT_TYPES:
             return self.PIP_SIMPLE_CONTENT_TYPES[self._pip_simple_format]
 
         if self._pip_simple_format is None:
@@ -387,34 +190,34 @@
 
                 match_info = filename, url, target
                 matches.append(match_info)
 
         if len(matches) == 0:
             message = f"No package found for [{package_name}] version [{model_def.version}]"
             self._log.error(message)
-            raise _ex.EModelRepo(message)
+            raise ex.EModelRepo(message)
 
         if len(matches) > 1:
             message = f"Multiple packages found for [{package_name}] version [{model_def.version}]" + \
                       f" (targets: " + ", ".join(map(lambda m: m[2], matches)) + ")"
             self._log.error(message)
-            raise _ex.EModelRepo(message)
+            raise ex.EModelRepo(message)
 
         filename, url, target = matches[0]
 
         self._log.info(f"Found package [{package_name}] version [{model_def.version}], target = [{target}]")
 
         return filename, url
 
-    def _pypi_json_query(self, model_def: _meta.ModelDefinition):
+    def _pypi_json_query(self, model_def: meta.ModelDefinition):
 
         json_root_url = urllib.parse.urlparse(self._pip_index)
         json_headers = {"accept": "application/json"}
 
-        credentials = _get_credentials(json_root_url, self._repo_config)
+        credentials = _helpers.get_http_credentials(json_root_url, self._properties)
 
         self._log.info(f"Query package: [{model_def.package}], version = [{model_def.version}]")
 
         package_req = self._pypi_package_query(
             self.JSON_PACKAGE_PATH, json_root_url, json_headers,
             credentials, model_def)
 
@@ -426,42 +229,42 @@
 
         urls = package_obj.get("urls") or []
         bdist_urls = list(filter(lambda d: d.get("packagetype") == "bdist_wheel", urls))
 
         if not bdist_urls:
             message = "No compatible packages found"
             self._log.error(message)
-            raise _ex.EModelRepo(message)
+            raise ex.EModelRepo(message)
 
         if len(bdist_urls) > 1:
             message = "Multiple compatible packages found (specialized distributions are not supported yet)"
             self._log.error(message)
-            raise _ex.EModelRepo(message)
+            raise ex.EModelRepo(message)
 
         package_url_info = bdist_urls[0]
         package_filename = package_url_info.get("filename")
         package_url = urllib.parse.urlparse(package_url_info.get("url"))
-        package_url = _apply_credentials(package_url, credentials)
+        package_url = _helpers.apply_http_credentials(package_url, credentials)
 
         return package_filename, package_url
 
     def _pypi_package_query(self, package_path_template, root_url, headers, credentials, model_def):
 
-        root_url = _apply_credentials(root_url, credentials)
+        root_url = _helpers.apply_http_credentials(root_url, credentials)
         package_path = package_path_template.format(root_url.path, model_def.package, model_def.version)
         package_url = root_url._replace(path=package_path)
 
-        self._log.info(f"GET: {_util.log_safe_url(package_url)}")
+        self._log.info(f"GET: {_helpers.log_safe_url(package_url)}")
 
         package_req = requests.get(package_url.geturl(), headers=headers)
 
         if package_req.status_code != requests.codes.OK:
             message = f"Package lookup failed: [{package_req.status_code}] {package_req.reason}"
             self._log.error(message)
-            raise _ex.EModelRepo(message)  # todo status code for access, not found etc
+            raise ex.EModelRepo(message)  # todo status code for access, not found etc
 
         return package_req
 
 
 class _PypiSimpleHtmlParser(html.parser.HTMLParser):
 
     def __init__(self, package_name: str, package_url: str):
@@ -477,15 +280,15 @@
 
         self.response = {
             "meta": {"api-version": None},
             "name": package_name,
             "files": []
         }
 
-    def handle_starttag(self, tag: str, attrs: list[tuple[str, str | None]]):
+    def handle_starttag(self, tag: str, attrs: tp.List[tp.Tuple[str, tp.Union[str, None]]]):
 
         element = (tag, attrs)
         self._stack.append(element)
         self._data = None
 
         if tag == "meta" and any(map(lambda a: a[0] == "name" and a[1] == "pypi:repository-version", attrs)):
             self._record_meta(attrs)
@@ -501,23 +304,23 @@
             stack_tag, _ = self._stack.pop()
 
     def handle_data(self, data: str):
 
         stripped_data = data.strip()
         self._data = stripped_data if len(stripped_data) > 0 else None
 
-    def _record_meta(self, attrs: list[tuple[str, str | None]]):
+    def _record_meta(self, attrs: tp.List[tp.Tuple[str, tp.Union[str, None]]]):
 
         content_attr = list(filter(lambda a: a[0] == "content", attrs))
 
         if len(content_attr) == 1:
             content, version = content_attr[0]
             self.response["meta"]["api-version"] = version
 
-    def _record_link(self, filename, attrs: list[tuple[str, str | None]]):
+    def _record_link(self, filename, attrs: tp.List[tp.Tuple[str, tp.Union[str, None]]]):
 
         href_attr = list(filter(lambda a: a[0] == "href", attrs))
         yanked_attr = list(filter(lambda a: a[0] == "data-yanked", attrs))
         python_version_attr = list(filter(lambda a: a[0] == "data-requires-python", attrs))
 
         if len(href_attr) != 1:
             return
@@ -547,55 +350,9 @@
             "hashes": hashes,
             "yanked": is_yanked
         }
 
         self.response["files"].append(file_info)
 
 
-# TODO: Move Git and PyPI repos into _plugins
-
-
-class RepositoryManager:
-
-    __repo_types: tp.Dict[str, tp.Callable[[_cfg.PluginConfig], IModelRepository]] = {
-        "integrated": IntegratedSource,
-        "local": LocalRepository,
-        "git": GitRepository,
-        "pypi": PyPiRepository
-    }
-
-    @classmethod
-    def register_repo_type(cls, repo_type: str, loader_class: tp.Callable[[_cfg.PluginConfig], IModelRepository]):
-        cls.__repo_types[repo_type] = loader_class
-
-    def __init__(self, sys_config: _cfg.RuntimeConfig):
-
-        self._log = _util.logger_for_object(self)
-        self._loaders: tp.Dict[str, IModelRepository] = dict()
-
-        for repo_name, repo_config in sys_config.repositories.items():
-
-            if repo_config.protocol not in self.__repo_types:
-
-                msg = f"Model repository type [{repo_config.protocol}] is not recognised" \
-                    + " (this could indicate a missing model repository plugin)"
-
-                self._log.error(msg)
-                raise _ex.EModelRepoConfig(msg)
-
-            loader_class = self.__repo_types[repo_config.protocol]
-            loader = loader_class(repo_config)
-            self._loaders[repo_name] = loader
-
-    def get_repository(self, repo_name: str) -> IModelRepository:
-
-        loader = self._loaders.get(repo_name)
-
-        if loader is None:
-
-            msg = f"Model repository [{repo_name}] is unknown or not configured" \
-                + " (this could indicate a missing repository entry in the system config)"
-
-            self._log.error(msg)
-            raise _ex.EModelRepoConfig(msg)
-
-        return loader
+# Register plugin
+plugins.PluginManager.register_plugin(IModelRepository, PyPiRepository, ["pypi"])
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_impl/schemas.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,36 +29,39 @@
 class SchemaLoader:
 
     _log: logging.Logger
 
     __SCHEMA_OF_SCHEMA = _meta.SchemaDefinition(
         schemaType=_meta.SchemaType.TABLE,
         table=_meta.TableSchema([
-            _meta.FieldSchema("field_name", 0, _meta.BasicType.STRING, "Field name", businessKey=True),
-            _meta.FieldSchema("field_type", 1, _meta.BasicType.STRING, "Field type", categorical=True),
-            _meta.FieldSchema("label", 2, _meta.BasicType.STRING, "Label"),
+            _meta.FieldSchema("field_name", 0, _meta.BasicType.STRING, "Field name", businessKey=True, notNull=True),
+            _meta.FieldSchema("field_type", 1, _meta.BasicType.STRING, "Field type", categorical=True, notNull=True),
+            _meta.FieldSchema("label", 2, _meta.BasicType.STRING, "Label", notNull=True),
             _meta.FieldSchema("business_key", 3, _meta.BasicType.BOOLEAN, "Business key flag"),
             _meta.FieldSchema("categorical", 4, _meta.BasicType.BOOLEAN, "Categorical flag"),
-            _meta.FieldSchema("format_code", 5, _meta.BasicType.STRING, "Format code"),
+            _meta.FieldSchema("not_null", 5, _meta.BasicType.BOOLEAN, "Not null flag"),
+            _meta.FieldSchema("format_code", 6, _meta.BasicType.STRING, "Format code"),
         ])
     )
 
     @classmethod
     def load_schema(cls, package: tp.Union[ts.ModuleType, str], schema_file: str) \
             -> _meta.SchemaDefinition:
 
         try:
 
-            csv_format = _storage.FormatManager.get_data_format("text/csv", {"lenient_csv_parser": True})
+            csv_options = {"lenient_csv_parser": True, "lenient_missing_columns": True}
+            csv_format = _storage.FormatManager.get_data_format("text/csv", csv_options)
 
             # Any resource loading failure will raise EModelRepoResource
             with _shim.ShimLoader.open_resource(package, schema_file) as schema_io:
 
                 schema_of_schema = _data.DataMapping.trac_to_arrow_schema(cls.__SCHEMA_OF_SCHEMA)
                 schema_data = csv_format.read_table(schema_io, schema_of_schema)
+                schema_data = _data.DataConformance.conform_to_schema(schema_data, schema_of_schema)
 
             return cls._decode_schema_data(schema_data)
 
         except _ex.EData as e:
 
             err = f"Invalid schema file [{schema_file}]: {str(e)}"
             cls._log.exception(err)
@@ -68,32 +71,35 @@
     def _decode_schema_data(cls, schema_data: pa.Table) -> _meta.SchemaDefinition:
 
         name_vec: pa.StringArray = schema_data.column(0)
         type_vec: pa.StringArray = schema_data.column(1)
         label_vec: pa.StringArray = schema_data.column(2)
         business_key_vec: pa.BooleanArray = schema_data.column(3)
         categorical_vec: pa.BooleanArray = schema_data.column(4)
-        format_code_vec: pa.StringArray = schema_data.column(5)
+        not_null_vec: pa.BooleanArray = schema_data.column(5)
+        format_code_vec: pa.StringArray = schema_data.column(6)
 
         field_list = []
 
         for field_index in range(schema_data.num_rows):
 
             field_name_val = name_vec[field_index]
             type_name_val: pa.StringScalar = type_vec[field_index]
             label_val = label_vec[field_index]
             business_key_val = business_key_vec[field_index]
             categorical_val = categorical_vec[field_index]
+            not_null_val = not_null_vec[field_index]
             format_code_val = format_code_vec[field_index]
 
             field_name = cls._arrow_to_py_string("field_name", None, field_index, field_name_val, required=True)
             type_name = cls._arrow_to_py_string("field_type", field_name, field_index, type_name_val, required=True)
             label = cls._arrow_to_py_string("label", field_name, field_index, label_val, required=True)
             business_key = cls._arrow_to_py_boolean("business_key", field_name, field_index, business_key_val, default=False)  # noqa
             categorical = cls._arrow_to_py_boolean("categorical", field_name, field_index, categorical_val, default=False)  # noqa
+            not_null = cls._arrow_to_py_boolean("not_null", field_name, field_index, not_null_val, default=business_key)  # noqa
             format_code = cls._arrow_to_py_string("format_code", field_name, field_index, format_code_val)
 
             if field_name is None or len(field_name.strip()) == 0:
                 err = f"Field name cannot be blank for field at index [{field_index}]"
                 cls._log.error(err)
                 raise _ex.EDataConformance(err)
 
@@ -114,28 +120,28 @@
                 display_type_name = type_name or str(None)
                 err = f"Unknown field type [{display_type_name}] for field [{field_name}] at index [{field_index}]"
                 cls._log.error(err)
                 raise _ex.EDataConformance(err)
 
             field_schema = _meta.FieldSchema(
                 field_name, field_index, field_type, label,
-                business_key, categorical, format_code)
+                business_key, categorical, not_null, format_code)
 
             field_list.append(field_schema)
 
         return _meta.SchemaDefinition(
             schemaType=_meta.SchemaType.TABLE,
             table=_meta.TableSchema(field_list))
 
     @classmethod
     def _arrow_to_py_string(
             cls, schema_field_name: str, field_name: tp.Optional[str], field_index: int,
             arrow_value: pa.StringScalar, required: bool = False):
 
-        if arrow_value is not None:
+        if arrow_value is not None and arrow_value.is_valid:
             return arrow_value.as_py()
 
         if not required:
             return None
 
         if field_name:
             err_suffix = f" for field [{field_name}] at index [{field_index}]"
@@ -147,15 +153,15 @@
         raise _ex.EDataConformance(err)
 
     @classmethod
     def _arrow_to_py_boolean(
             cls, schema_field_name: str, field_name: str, field_index: int,
             arrow_value: pa.BooleanScalar, required: bool = False, default: tp.Optional[bool] = None):
 
-        if arrow_value is not None:
+        if arrow_value is not None and arrow_value.is_valid:
             return arrow_value.as_py()
 
         if not required:
             return default
 
         err = f"Missing required value {schema_field_name} for field [{field_name}] at index [{field_index}]"
         cls._log.error(err)
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_impl/shim.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/shim.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,113 +16,129 @@
 import types
 import itertools
 import logging
 import pathlib
 import sys
 import contextlib
 import functools as fn
-import traceback as tb
 
 import inspect
 import importlib as _il
 import importlib.util as _ilu
 import importlib.abc as _ila
 import importlib.machinery as _ilm
 import importlib.resources as _ilr
 
 import tracdap.rt.exceptions as _ex
+import tracdap.rt._impl.guard_rails as _guard
 import tracdap.rt._impl.util as _util
 
 
+class _Shim:
+
+    def __init__(self, shim_id: int, namespace: str, search_locations: tp.List[str]):
+        self.shim_id = shim_id
+        self.namespace = namespace
+        self.search_locations = search_locations
+
+
 class _ActiveShim:
 
     # Wrapper class to hold a reference to the active shim
     # This reference needs to be shared across the various pieces of machinery for shim loading
 
     def __init__(self):
         self.shim: tp.Optional[str] = None
+        self.main_module: tp.Optional[str] = None
 
 
 class _ActiveShimFinder(_ila.MetaPathFinder):
 
     # The active shim finder trys to resolve global module imports in the active shim
     # For imports of the form: import acme_global.module
     # The module name is mapped: acme_global.module -> tracdap.shim._XXX.acme_global.module
     # The shimmed module name is passed back to importlib for resolution
 
-    # Absolute imports in model code will always come to this finder
-    # Consequently, absolute imports only work when the shim is active, i.e. when the model module is imported
-    # Absolute imports in model code will not work (imports in model code is very bad practice anyway)!
+    # This finder will handle loading the root model packages, after which
+    # absolute and qualified imports are handled by the normal mechanism
 
-    def __init__(self, shim_map: tp.Dict[str, pathlib.Path], active_shim: _ActiveShim):
-        self.__shim_map = shim_map
-        self.__active_shim = active_shim
+    # Unqualified (i.e. relative) imports will always come to this loader
+    # This is because the names are qualified before adding to the module cache
+    # So, unqualified relative imports only work when the shim is active, i.e. during initial load
+    # Relative imports used dynamically will not work (this is very bad practice anyway)!
 
-    def set_shim_map(self, shim_map: tp.Dict[str, pathlib.Path]):
+    def __init__(self, shim_map: tp.Dict[str, _Shim], active_shim: _ActiveShim):
         self.__shim_map = shim_map
-
-    def set_active_shim(self, active_shim: tp.Optional[str]):
         self.__active_shim = active_shim
 
     def find_spec(
             self, fullname: str,
             path: tp.Optional[tp.Sequence[tp.Union[bytes, str]]] = None,
             target: tp.Optional[types.ModuleType] = None) \
             -> tp.Optional[_ilm.ModuleSpec]:
 
+        # The active shim finder works by translating the supplied module name
+        # E.g. acme.rockets -> import tracdap.shim._0.acme.rockets
+        # The loader issue a new call to find_module for the translated name
+        # Theis new call will hit the namespace shim finder
+
         # If the module name is already qualified with a shim, don't try to re-qualify it
         if fullname.startswith(ShimLoader.SHIM_NAMESPACE):
             return None
 
         # If there is no active shim set, don't return a module
         if self.__active_shim.shim is None:
             return None
 
-        shim_module = f"{self.__active_shim.shim}.{fullname}"
-        shim_path = self.__shim_map.get(self.__active_shim.shim)
-
-        # Looking for the shimmed module will hit the namespace shim finder
-        return _ilu.find_spec(shim_module, str(shim_path))
+        # Python adds the directory containing __main__ to PYTHONPATH ahead of other source dirs
+        # This has the effect that relative imports are given priority in the loading order
+        # To replicate this behavior, we can attempt a relative import before looking for absolute names
+
+        # Different models have different main modules, so relative names will resolve differently
+        # Several models can be loaded in the same shim, so we can't put relative imports in the root namespace
+        # Instead we qualify relative imports, using the model main module as the relative root
+
+        if self.__active_shim.main_module is not None:
+
+            # Only try relative import if the relative root is already loaded
+            shim_relative_root = f"{self.__active_shim.shim}.{self.__active_shim.main_module}"
+            if shim_relative_root in sys.modules:
+
+                # Relative root for packages is the root name
+                # Relative root for modules is the parent of the root name
+                shim_relative_module = sys.modules[shim_relative_root]
+                if not shim_relative_module.__spec__.origin.endswith("__init__.py"):
+                    shim_relative_root = shim_relative_root[:shim_relative_root.rfind(".")]
+
+                # We need to check down the tree for the relative import
+                # find_spec() will raise an error f we look for a module before the parent is loaded
+                # We want to return None in this case, and fall back to the absolute import
+                shim_relative_name = shim_relative_root
+                shim_relative_spec = None
+                for level in fullname.split("."):
+                    shim_relative_name += f".{level}"
+                    shim_relative_spec = _ilu.find_spec(shim_relative_name)
+                    if shim_relative_spec is None:
+                        break
+
+                # If the relative module is found then we can return that spec
+                if shim_relative_spec is not None:
+                    return shim_relative_spec
+
+        # No relative module available, so now try to load using the absolute module name
+        shim_absolute_name = f"{self.__active_shim.shim}.{fullname}"
+        return _ilu.find_spec(shim_absolute_name)
 
     def invalidate_caches(self) -> None:
         pass
 
 
-class _ActiveShimLoader(_ilm.SourceFileLoader):
-
-    # When loading in an active shim, put a global entry in sys.modules for the relative module name
-    # Submodule loads will expect the parent module to be present with the relative module name
-    # This behavior is built into the base implementation of Pythons module loading mechanism
-    # It is important to add the global entry before the module is executed, which is when submodule imports happen
-
-    # Global module names are removed from sys.modules when the shim is deactivated
-    # At that point all module members are available in the shim namespace and global names are no longer needed
-
-    # Logic code around import statements will work, so long as all that logic executes during the initial import
-    # Very strange behaviors, like attempting dynamic imports at runtime, are likely to fail or behave erratically
-
-    def __init__(self, relative_name, fullname, path):
-        super().__init__(fullname, path)
-        self._relative_name = relative_name
-
-    def create_module(self, spec: _ilm.ModuleSpec) -> tp.Optional[types.ModuleType]:
-
-        return super().create_module(spec)
-
-    def exec_module(self, module: types.ModuleType) -> None:
-
-        if self._relative_name not in sys.modules:
-            sys.modules[self._relative_name] = module
-
-        super().exec_module(module)
-
-
 class _NamespaceShimFinder(_ila.MetaPathFinder):
 
-    def __init__(self, shim_map: tp.Dict[str, pathlib.Path], active_shim: _ActiveShim):
+    def __init__(self, shim_map: tp.Dict[str, _Shim], active_shim: _ActiveShim):
         self.__shim_map = shim_map
         self.__active_shim = active_shim
         self._log = _util.logger_for_class(ShimLoader)
 
     def find_spec(
             self, fullname: str,
             path: tp.Optional[tp.Sequence[tp.Union[bytes, str]]] = None,
@@ -140,50 +156,80 @@
         if len(module_parts) == 2:
             spec = _ilm.ModuleSpec(fullname, origin=None, is_package=True, loader=None)
             return spec
 
         # The shim namespace is the first three parts of the module name, tracdap.shim._XXX
         # This should have been registered in the shim map by ShimLoader.create_shim
         shim_namespace = ".".join(module_parts[:3])
-        shim_path = self.__shim_map.get(shim_namespace)
+        shim = self.__shim_map.get(shim_namespace)
 
         # The relative module name is everything after the shim namespace
         # This is what would be written in the original model code, and will look familiar to modellers
         relative_parts = module_parts[3:]
         relative_name = ".".join(relative_parts)
 
         # If the shim is not registered, this is probably a bug
         # The loader mechanism should not generate requests to load from unregistered shims
         # The alternative is an explicit reference to a shim in model code, which should definitely not be allowed!
-        if shim_path is None:
+        if shim is None:
 
             self._log.error("There was an error in the model loading mechanism (this is a bug)")
             self._log.error(f"Attempt to load module [{relative_name}] from unregistered shim [{shim_namespace}]")
             raise _ex.ETracInternal("There was an error in the model loading mechanism (this is a bug)")
 
         # If this request is for a shim namespace package, create a namespace module spec
         # This should only happen after the shim has been created in ShimLoader
         # Attach the shim path to the spec, this will be the location to search for modules in the shim
         if len(module_parts) == 3:
 
             self._log.debug(f"Creating namespace package for shim [{shim_namespace}]")
-
             spec = _ilm.ModuleSpec(fullname, origin=None, is_package=True, loader=None)
-            spec.submodule_search_locations = str(shim_path)
+
+            # Do not set search locations on the shim package
+            # We want to force root packages back through the shim loader mechanism
+            # Setting search locations will let them use the regular file-based finder / loader
+
+            spec.submodule_search_locations = []
 
             return spec
 
-        # Once the code falls through to here, the request is for a module inside a recognized shim
+        for source_path in shim.search_locations:
+
+            shim_path = pathlib.Path(source_path)
+
+            module_spec = self._try_load_module(
+                fullname, relative_name, relative_parts,
+                shim_namespace, shim_path)
+
+            if module_spec is not None:
+                return module_spec
+
+        # Module not found, return None
+
+        self._log.debug(f"Module [{relative_name}] not found in shim [{shim_namespace}]")
+
+        return None
+
+    def _try_load_module(
+            self, fullname: str,
+            relative_name: str, relative_parts: tp.List[str],
+            shim_namespace, shim_path: pathlib.Path):
 
         # The requested module can be either a normal module or a package
         # The expected path is different for modules and packages, we need to check for both
         parent_path = fn.reduce(lambda p, q: p.joinpath(q), relative_parts[:-1], shim_path)
         package_path = parent_path.joinpath(relative_parts[-1], "__init__.py")
         module_path = parent_path.joinpath(relative_parts[-1] + ".py")
 
+        # Windows still has a path length limit of 260 characters! Above that you have to use UNC-style paths
+        # Model checkout paths can easily exceed the limit, to be safe always use UNC paths on Windows
+        if _util.is_windows():
+            package_path = pathlib.Path(f"\\\\?\\{str(package_path)}")
+            module_path = pathlib.Path(f"\\\\?\\{str(module_path)}")
+
         # A module can exist as both a module and a package in the same source path
         # This is a very bad thing to do and should always be avoided
         # However, it is allowed when using the regular Python loader mechanisms
         # We want to replicate the same behaviour, to avoid unexpected breaks when loading to the platform
         # The Python behaviour is to give precedence to packages, so the shim loader should do the same
 
         if package_path.exists() and module_path.exists():
@@ -195,71 +241,110 @@
         # When the active shim is deactivated, shim modules will be removed from the global namespace
         # If the shim is not active the only option is a regular source loader in the shim namespace
         # This does not normally happen unless model code uses dynamic imports (highly unrecommended)!
         if package_path.exists() and package_path.is_file():
 
             self._log.debug(f"Loading package [{relative_name}] in shim [{shim_namespace}]")
 
-            if shim_namespace == self.__active_shim.shim:
-                shim_loader = _ActiveShimLoader(relative_name, fullname, str(package_path))
-            else:
-                shim_loader = _ilm.SourceFileLoader(fullname, str(package_path))
+            loader = _NamespaceShimLoader(
+                self.__active_shim, shim_namespace, relative_name,
+                fullname, str(package_path))
+
+            spec = _ilm.ModuleSpec(fullname, origin=str(package_path), is_package=True, loader=loader)
+
+            # Do not set search locations on the shim package
+            # We want to force shim imports back through the shim loader mechanism
+            # Setting search locations will let them use the regular file-based finder / loader
+
+            spec.submodule_search_locations = []
 
-            spec = _ilm.ModuleSpec(fullname, origin=str(package_path), is_package=True, loader=shim_loader)
-            spec.submodule_search_locations = str(package_path.parent)
             return spec
 
         # If the module path is found, return a spec for a regular module
         # The module exists in the shim namespace only
         # Since modules have no children, there will be no issues resolving submodules with absolute imports
         elif module_path.exists() and module_path.is_file():
 
             self._log.debug(f"Loading module [{relative_name}] in shim [{shim_namespace}]")
 
-            shim_loader = _ilm.SourceFileLoader(fullname, str(module_path))
-            spec = _ilm.ModuleSpec(fullname, origin=str(module_path), loader=shim_loader)
-            return spec
+            loader = _ilm.SourceFileLoader(fullname, str(module_path))
+            spec = _ilm.ModuleSpec(fullname, origin=str(module_path), loader=loader)
 
-        # Module not found, return None
-        else:
-            self._log.debug(f"Module [{relative_name}] not found in shim [{shim_namespace}]")
-            return None
+            return spec
 
     def invalidate_caches(self) -> None:
         pass
 
 
+class _NamespaceShimLoader(_ilm.SourceFileLoader):
+
+    # When loading in an active shim, put a global entry in sys.modules for the relative module name
+    # Submodule loads will expect the parent module to be present with the relative module name
+    # This behavior is built into the base implementation of Pythons module loading mechanism
+    # It is important to add the global entry before the module is executed, which is when submodule imports happen
+
+    # Global module names are removed from sys.modules when the shim is deactivated
+    # At that point all module members are available in the shim namespace and global names are no longer needed
+
+    # Logic code around import statements will work, so long as all that logic executes during the initial import
+    # Very strange behaviors, like attempting dynamic imports at runtime, are likely to fail or behave erratically
+
+    def __init__(self, active_shim, shim_namespace, relative_name, fullname, path):
+        super().__init__(fullname, path)
+        self.__active_shim = active_shim
+        self._shim_namespace = shim_namespace
+        self._relative_name = relative_name
+
+    def create_module(self, spec: _ilm.ModuleSpec) -> tp.Optional[types.ModuleType]:
+
+        return super().create_module(spec)
+
+    def exec_module(self, module: types.ModuleType) -> None:
+
+        if self.__active_shim.shim == self._shim_namespace:
+            if self._relative_name not in sys.modules:
+                sys.modules[self._relative_name] = module
+
+        super().exec_module(module)
+
+
 class ShimLoader:
 
     SHIM_NAMESPACE = "tracdap.shim"
 
     _T = tp.TypeVar("_T")
 
     _log: tp.Optional[logging.Logger] = None
 
     __shim_id_seq = itertools.count()
-    __shim_map: tp.Dict[str, pathlib.Path] = dict()
+    __shim_map: tp.Dict[str, _Shim] = dict()
     __active_shim = _ActiveShim()
 
     @classmethod
     def _init(cls):
 
         sys.meta_path.append(_NamespaceShimFinder(cls.__shim_map, cls.__active_shim))
         sys.meta_path.append(_ActiveShimFinder(cls.__shim_map, cls.__active_shim))
 
     @classmethod
-    def create_shim(cls, package_root: tp.Union[str, pathlib.Path]) -> str:
+    def create_shim(cls, shim_root_path: tp.Union[str, pathlib.Path], source_paths: tp.List[str] = None) -> str:
+
+        # If source paths not specified, preserve the old behavior and look in the shim root
+        if not source_paths:
+            source_paths = ["."]
 
         shim_id = next(cls.__shim_id_seq)
         shim_namespace = f"{cls.SHIM_NAMESPACE}._{shim_id}"
-        package_root = pathlib.Path(package_root).resolve()
+        shim_root = pathlib.Path(shim_root_path).resolve()
+
+        search_locations = list(map(lambda p: str(shim_root.joinpath(p).resolve()), source_paths))
 
-        cls.__shim_map[shim_namespace] = package_root
+        cls.__shim_map[shim_namespace] = _Shim(shim_id, shim_namespace, search_locations)
 
-        cls._log.debug(f"Creating shim [{shim_namespace}] for path [{package_root}]")
+        cls._log.debug(f"Creating shim [{shim_namespace}] for root path [{shim_root}]")
 
         _il.import_module(shim_namespace)
 
         return shim_namespace
 
     @classmethod
     def activate_shim(cls, shim_namespace: str):
@@ -315,21 +400,25 @@
         for module_name in shim_modules:
             del sys.modules[module_name]
 
     @classmethod
     @contextlib.contextmanager
     def use_shim(cls, shim_namespace: str):
 
-        if shim_namespace:
-            cls.activate_shim(shim_namespace)
+        try:
+
+            if shim_namespace:
+                cls.activate_shim(shim_namespace)
+
+            yield
 
-        yield
+        finally:
 
-        if shim_namespace:
-            cls.deactivate_shim()
+            if shim_namespace:
+                cls.deactivate_shim()
 
     @classmethod
     def load_class(
             cls, module: tp.Union[types.ModuleType, str],
             class_name: str, class_type: tp.Type[_T]) -> tp.Type[_T]:
 
         cls._run_model_guard()
@@ -340,15 +429,21 @@
             module_name = module
 
         try:
 
             cls._log.debug(f"Loading class [{class_name}] from [{module_name}]")
 
             if isinstance(module, str):
-                module = _il.import_module(module_name)
+                try:
+                    # Set the root module for class loading
+                    # Relative imports will be resolved relative to this root
+                    cls.__active_shim.main_module = module_name
+                    module = cls.trac_model_code_import(module_name)
+                finally:
+                    cls.__active_shim.main_module = None
 
             class_ = module.__dict__.get(class_name)
 
             if class_ is None:
                 err = f"Loading classes failed in module [{module_name}]: Class [{class_name}] not found"
                 cls._log.error(err)
                 raise _ex.EModelLoad(err)
@@ -365,30 +460,36 @@
                 raise _ex.EModelLoad(err)
 
             return class_
 
         except _ex.EModelLoad:
             raise
 
-        except ModuleNotFoundError as e:
-            err = f"Loading classes failed in module [{module_name}]: {str(e)}"
-            cls._log.error(err)
-            raise _ex.EModelLoad(err) from e
-
-        except NameError as e:
-            err = f"Loading classes failed in module [{module_name}]: {str(e)} ({cls._last_frame(e)}"
+        except (ModuleNotFoundError, NameError) as e:
+            details = _util.error_details_from_exception(e)
+            err = f"Loading classes failed in module [{module_name}]: {str(e)}{details}"
             cls._log.error(err)
             raise _ex.EModelLoad(err) from e
 
         except Exception as e:
-            err = f"Loading classes failed in module [{module_name}]: Unexpected error"
+            err = f"Loading classes failed in module [{module_name}]: {str(e)}"
             cls._log.error(err)
             raise _ex.EModelLoad(err) from e
 
     @classmethod
+    def trac_model_code_import(cls, module_name):
+
+        # Guard rails can interfere with import
+        # This method turns off some of the rails that interfere with importing
+        # This method name is used as a hook in PythonGuardRails, to detect model code imports
+
+        with _guard.PythonGuardRails.enable_import_functions():
+            return _il.import_module(module_name)
+
+    @classmethod
     def load_resource(
             cls, module: tp.Union[types.ModuleType, str],
             resource_name: str) -> bytes:
 
         return cls._load_or_open_resource(module, resource_name, _ilr.read_binary)
 
     @classmethod
@@ -419,31 +520,27 @@
                 module = _il.import_module(module_name)
 
             return load_func(module, resource_name)
 
         except _ex.EModelLoad:
             raise
 
-        except ModuleNotFoundError as e:
-            err = f"Loading resources failed in module [{module_name}]: {str(e)}"
+        except (ModuleNotFoundError, NameError) as e:
+            details = _util.error_details_from_exception(e)
+            err = f"Loading resources failed in module [{module_name}]: {str(e)}{details}"
             cls._log.error(err)
             raise _ex.EModelLoad(err) from e
 
         except FileNotFoundError as e:
-            err = f"Loading resources failed in module [{module_name}]: Resource not found for [{resource_name}]"
-            cls._log.error(err)
-            raise _ex.EModelLoad(err) from e
-
-        except NameError as e:
-            err = f"Loading classes failed in module [{module_name}]: {str(e)} ({cls._last_frame(e)}"
+            err = f"Loading resources failed in module [{module_name}]: File not found for [{resource_name}]"
             cls._log.error(err)
             raise _ex.EModelLoad(err) from e
 
         except Exception as e:
-            err = f"Loading classes failed in module [{module_name}]: Unexpected error"
+            err = f"Loading resources failed in module [{module_name}]: Unexpected error"
             cls._log.error(err)
             raise _ex.EModelLoad(err) from e
 
     @classmethod
     def _run_model_guard(cls):
 
         # Loading resources from inside run_model is an invalid use of the runtime API
@@ -458,17 +555,10 @@
             frame = stack[frame_index]
 
             if frame.function == "run_model" and parent_frame.function == "_execute":
                 err = f"Loading resources is not allowed inside run_model()"
                 cls._log.error(err)
                 raise _ex.ERuntimeValidation(err)
 
-    @classmethod
-    def _last_frame(cls, error: Exception):
-        trace = tb.extract_tb(error.__traceback__)
-        last_frame = trace[len(trace) - 1]
-        filename = pathlib.PurePath(last_frame.filename).name
-        return f"{filename} line {last_frame.lineno}, {last_frame.line}"
-
 
 ShimLoader._log = _util.logger_for_class(ShimLoader)
 ShimLoader._init()  # noqa
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_impl/static_api.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/static_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,43 +78,53 @@
 
         if isinstance(param_type, _meta.TypeDescriptor):
             param_type_descriptor = param_type
         else:
             param_type_descriptor = _meta.TypeDescriptor(param_type, None, None)
 
         if default_value is not None and not isinstance(default_value, _meta.Value):
-            default_value = _type_system.MetadataCodec.encode_value(default_value)
+            try:
+                default_value = _type_system.MetadataCodec.convert_value(default_value, param_type_descriptor)
+            except _ex.ETrac as e:
+                msg = f"Default value for parameter [{param_name}] does not match the declared type"
+                raise _ex.EModelValidation(msg) from e
 
         return _Named(param_name, _meta.ModelParameter(param_type_descriptor, label, default_value))
 
     def define_parameters(
             self, *params: _tp.Union[_Named[_meta.ModelParameter], _tp.List[_Named[_meta.ModelParameter]]]) \
             -> _tp.Dict[str, _meta.ModelParameter]:
 
         _val.validate_signature(self.define_parameters, *params)
 
         return self._build_named_dict(*params)
 
     def define_field(
             self, field_name: str, field_type: _meta.BasicType, label: str,
-            business_key: bool = False, categorical: bool = False,
+            business_key: bool = False, categorical: bool = False, not_null: _tp.Optional[bool] = None,
             format_code: _tp.Optional[str] = None, field_order: _tp.Optional[int] = None) \
             -> _meta.FieldSchema:
 
         _val.validate_signature(
             self.define_field, field_name, field_type, label,
-            business_key, categorical, format_code, field_order)
+            business_key, categorical, not_null,
+            format_code, field_order)
+
+        # Set the not_null flag for business keys if it is not specified
+        if not_null is None:
+            not_null = business_key
 
         return _meta.FieldSchema(
             field_name,
             field_order,
             field_type,
             label,
             businessKey=business_key,
             categorical=categorical,
+            notNull=not_null,
             formatCode=format_code)
 
     def define_schema(
             self, *fields: _tp.Union[_meta.FieldSchema, _tp.List[_meta.FieldSchema]],
             schema_type: _meta.SchemaType = _meta.SchemaType.TABLE) \
             -> _meta.SchemaDefinition:
 
@@ -133,30 +143,30 @@
             -> _meta.SchemaDefinition:
 
         _val.validate_signature(self.load_schema, package, schema_file, schema_type)
 
         return _schemas.SchemaLoader.load_schema(package, schema_file)
 
     def define_input_table(
-            self, *fields: _tp.Union[_meta.FieldSchema, _tp.List[_meta.FieldSchema]]) \
+            self, *fields: _tp.Union[_meta.FieldSchema, _tp.List[_meta.FieldSchema]], label: _tp.Optional[str] = None) \
             -> _meta.ModelInputSchema:
 
-        _val.validate_signature(self.define_input_table, *fields)
+        _val.validate_signature(self.define_input_table, *fields, label=label)
 
         schema_def = self.define_schema(*fields, schema_type=_meta.SchemaType.TABLE)
-        return _meta.ModelInputSchema(schema=schema_def)
+        return _meta.ModelInputSchema(schema=schema_def, label=label)
 
     def define_output_table(
-            self, *fields: _tp.Union[_meta.FieldSchema, _tp.List[_meta.FieldSchema]]) \
+            self, *fields: _tp.Union[_meta.FieldSchema, _tp.List[_meta.FieldSchema]], label: _tp.Optional[str] = None) \
             -> _meta.ModelOutputSchema:
 
-        _val.validate_signature(self.define_output_table, *fields)
+        _val.validate_signature(self.define_output_table, *fields, label=label)
 
         schema_def = self.define_schema(*fields, schema_type=_meta.SchemaType.TABLE)
-        return _meta.ModelOutputSchema(schema=schema_def)
+        return _meta.ModelOutputSchema(schema=schema_def, label=label)
 
     @staticmethod
     def _build_named_dict(
             *attrs: _tp.Union[_Named[_T], _tp.List[_Named[_T]]]) \
             -> _tp.Dict[str, _T]:
 
         if len(attrs) == 1 and isinstance(attrs[0], list):
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_impl/type_system.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/type_system.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_impl/util.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from __future__ import annotations
-
 import datetime as dt
 import logging
 import pathlib
 import platform
-import urllib.parse
 
 import sys
 import typing as tp
 import uuid
 
 import tracdap.rt.exceptions as ex
 import tracdap.rt.metadata as meta
 import tracdap.rt.config as cfg
 
+import traceback as tb
+
 
 __IS_WINDOWS = platform.system() == "Windows"
+__FIRST_MODEL_FRAME_NAME = "run_model"
+__FIRST_MODEL_FRAME_TEST_NAME = "_callTestMethod"
 
 
 def is_windows():
     return __IS_WINDOWS
 
 
 class ColorFormatter(logging.Formatter):
@@ -140,14 +141,36 @@
     return logging.getLogger(qualified_class_name)
 
 
 def logger_for_namespace(namespace: str) -> logging.Logger:
     return logging.getLogger(namespace)
 
 
+def format_file_size(size: int) -> str:
+
+    if size < 1024:
+        if size == 0:
+            return "0 bytes"
+        elif size == 1:
+            return "1 byte"
+        else:
+            return f"{size} bytes"
+
+    if size < 1024 ** 2:
+        kb = size / 1024
+        return f"{kb:.1f} KB"
+
+    if size < 1024 ** 3:
+        mb = size / (1024 ** 2)
+        return f"{mb:.1f} MB"
+
+    gb = size / (1024 ** 3)
+    return f"{gb:.1f} GB"
+
+
 def new_object_id(object_type: meta.ObjectType) -> meta.TagHeader:
 
     timestamp = dt.datetime.utcnow()
 
     return meta.TagHeader(
         objectType=object_type,
         objectId=str(uuid.uuid4()),
@@ -199,44 +222,24 @@
 
     resource_key = object_key(selector)
     resource_id = job_config.resourceMapping.get(resource_key)
 
     if resource_id is not None:
         resource_key = object_key(resource_id)
 
-    if optional:
-        return job_config.resources.get(resource_key)
-    else:
-        return job_config.resources[resource_key]
-
-
-__T = tp.TypeVar("__T")
-
-
-class __LogClose(tp.Generic[__T]):
-
-    def __init__(self, ctx_mgr: __T, log, msg):
-        self.__ctx_mgr = ctx_mgr
-        self.__log = log
-        self.__msg = msg
-
-    def __getitem__(self, item):
-        return self.__ctx_mgr.__getitem__(item)
+    resource = job_config.resources.get(resource_key)
 
-    def __enter__(self):
-        return self.__ctx_mgr.__enter__()
+    if resource is not None:
+        return resource
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.__ctx_mgr.__exit__(exc_type, exc_val, exc_tb)
-        self.__log.info(self.__msg)
-
-
-def log_close(ctx_mgg: __T, log: logging.Logger, msg: str) -> __T:
+    if optional:
+        return None
 
-    return __LogClose(ctx_mgg, log, msg)
+    err = f"Missing required {selector.objectType} resource [{object_key(selector)}]"
+    raise ex.ERuntimeValidation(err)
 
 
 def get_origin(metaclass: type):
 
     # Minimum supported Python is 3.7, which does not provide get_origin and get_args
 
     if "get_origin" in tp.__dict__:
@@ -287,63 +290,57 @@
         try:
             normalized_path.rmdir()
             return clean_ok
         except Exception:  # noqa
             return False
 
 
-def log_safe(param: tp.Any):
-
-    if isinstance(param, urllib.parse.ParseResult) or isinstance(param, urllib.parse.ParseResultBytes):
-        return log_safe_url(param)
-
-    if isinstance(param, str):
-        try:
-            url = urllib.parse.urlparse(param)
-            return log_safe_url(url)
-        except ValueError:
-            return param
-
-    return param
-
-
-def log_safe_url(url: tp.Union[str, urllib.parse.ParseResult, urllib.parse.ParseResultBytes]):
-
-    if isinstance(url, str):
-        url = urllib.parse.urlparse(url)
+def error_details_from_trace(trace: tb.StackSummary):
+    last_frame = trace[len(trace) - 1]
+    filename = pathlib.PurePath(last_frame.filename).name
+    # Do not report errors from inside C modules,
+    # they will not be meaningful to users
+    if filename.startswith("<"):
+        return ""
+    else:
+        return f" ({filename} line {last_frame.lineno}, {last_frame.line})"
 
-    if url.password:
 
-        user_sep = url.netloc.index(":")
-        pass_sep = url.netloc.index("@")
+def error_details_from_model_exception(error: Exception, checkout_directory: pathlib.Path):
+    trace = tb.extract_tb(error.__traceback__)
+    filtered_trace = filter_model_stack_trace(trace, checkout_directory)
+    return error_details_from_trace(filtered_trace)
 
-        user = url.netloc[:user_sep]
-        safe_location = f"{user}:*****@{url.netloc[pass_sep + 1:]}"
 
-        return url._replace(netloc=safe_location).geturl()
+def error_details_from_exception(error: Exception):
+    trace = tb.extract_tb(error.__traceback__)
+    return error_details_from_trace(trace)
 
-    elif url.username:
 
-        separator = url.netloc.index("@")
-        safe_location = f"*****@{url.netloc[separator + 1:]}"
+def filter_model_stack_trace(full_stack: tb.StackSummary, checkout_directory: pathlib.Path):
 
-        return url._replace(netloc=safe_location).geturl()
+    frame_names = list(map(lambda frame_: frame_.name, full_stack))
 
+    if __FIRST_MODEL_FRAME_NAME in frame_names:
+        first_model_frame = frame_names.index(__FIRST_MODEL_FRAME_NAME)
+    elif __FIRST_MODEL_FRAME_TEST_NAME in frame_names:
+        first_model_frame = frame_names.index(__FIRST_MODEL_FRAME_TEST_NAME)
     else:
-        return url.geturl()
-
-
-def get_plugin_property(config: cfg.PluginConfig, property_name: str):
-
-    if property_name in config.properties:
-        return config.properties[property_name]
+        first_model_frame = 0
 
-    # Allow for properties set up via env variables on Windows
-    # Python for Windows makes env var names uppercase when querying the environment
-    # This will allow properties to be found, even if the case has been changed
-    if is_windows():
+    last_model_frame = first_model_frame
 
-        for key, value in config.properties.items():
-            if key.lower() == property_name.lower():
-                return value
+    for frame_index, frame in enumerate(full_stack[first_model_frame:]):
+        module_path = pathlib.Path(frame.filename)
+        if "tracdap" in module_path.parts:
+            tracdap_index = len(module_path.parts) - 1 - list(reversed(module_path.parts)).index("tracdap")
+            if tracdap_index < len(module_path.parts)-1:
+                if module_path.parts[tracdap_index+1] == "rt":
+                    break
+        if ("site-packages" in module_path.parts) or ("venv" in module_path.parts):
+            break
+        # is_relative_to only supported in Python 3.9+, we need to support 3.7
+        if (checkout_directory is not None) and (checkout_directory not in module_path.parents):
+            break
+        last_model_frame = first_model_frame + frame_index
 
-    return None
+    return full_stack[first_model_frame:last_model_frame+1]
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_impl/validation.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_impl/validation.py`

 * *Files 15% similar despite different names*

```diff
@@ -231,16 +231,17 @@
             raise ex.ETracInternal(f"Validation of [{origin.__name__}] generic parameters is not supported yet")
 
         return type_var.__name__
 
 
 class _StaticValidator:
 
-    __identifier_pattern = re.compile("\\A[a-zA-Z_]\\w+\\Z", re.ASCII)
+    __identifier_pattern = re.compile("\\A[a-zA-Z_]\\w*\\Z", re.ASCII)
     __reserved_identifier_pattern = re.compile("\\A(_|trac_)", re.ASCII)
+    __label_length_limit = 4096
 
     __PRIMITIVE_TYPES = [
         meta.BasicType.BOOLEAN,
         meta.BasicType.INTEGER,
         meta.BasicType.FLOAT,
         meta.BasicType.DECIMAL,
         meta.BasicType.STRING,
@@ -292,19 +293,39 @@
         # Note unique context does not include static attributes
         # They are not part of the runtime context, so there is no need to constrain them
         unique_ctx = {}
         cls._unique_context_check(unique_ctx, model_def.parameters.keys(), "model parameter")
         cls._unique_context_check(unique_ctx, model_def.inputs.keys(), "model input")
         cls._unique_context_check(unique_ctx, model_def.outputs.keys(), "model output")
 
-        cls._check_table_fields(model_def.inputs)
-        cls._check_table_fields(model_def.outputs)
+        cls._check_parameters(model_def.parameters)
+        cls._check_inputs_or_outputs(model_def.inputs)
+        cls._check_inputs_or_outputs(model_def.outputs)
 
     @classmethod
-    def _check_table_fields(cls, inputs_or_outputs):
+    def _check_label(cls, label, param_name):
+        if label is not None:
+            if len(label) > cls.__label_length_limit:
+                cls._fail(f"Invalid model parameter: [{param_name}] label exceeds maximum length limit "
+                          f"({cls.__label_length_limit} characters)")
+            if len(label.strip()) == 0:
+                cls._fail(f"Invalid model parameter: [{param_name}] label is blank")
+
+    @classmethod
+    def _check_parameters(cls, parameters):
+
+        for param_name, param in parameters.items():
+
+            if param.label is None:
+                cls._fail(f"Invalid model parameter: [{param_name}] label is missing")
+            else:
+                cls._check_label(param.label, param_name)
+
+    @classmethod
+    def _check_inputs_or_outputs(cls, inputs_or_outputs):
 
         for input_name, input_schema in inputs_or_outputs.items():
 
             cls._log.info(f"Checking {input_name}")
 
             fields = input_schema.schema.table.fields
             field_names = list(map(lambda f: f.fieldName, fields))
@@ -312,33 +333,45 @@
 
             cls._valid_identifiers(field_names, property_type)
             cls._case_insensitive_duplicates(field_names, property_type)
 
             for field in fields:
                 cls._check_single_field(field, property_type)
 
+            label = input_schema.label
+            cls._check_label(label, input_name)
+
     @classmethod
     def _check_single_field(cls, field: meta.FieldSchema, property_type):
 
         # Valid identifier and not trac reserved checked separately
 
         cls._log.info(field.fieldName)
 
         if field.fieldOrder < 0:
             cls._fail(f"Invalid {property_type}: [{field.fieldName}] fieldOrder < 0")
 
         if field.fieldType not in cls.__PRIMITIVE_TYPES:
             cls._fail(f"Invalid {property_type}: [{field.fieldName}] fieldType is not a primitive type")
 
+        if field.label is None or len(field.label.strip()) == 0:
+            cls._fail(f"Invalid {property_type}: [{field.fieldName}] label is missing or blank")
+
+        if len(field.label) > cls.__label_length_limit:
+            cls._fail(f"Invalid {property_type}: [{field.fieldName}] label exceeds maximum length limit ({cls.__label_length_limit} characters)")  # noqa
+
         if field.businessKey and field.fieldType not in cls.__BUSINESS_KEY_TYPES:
             cls._fail(f"Invalid {property_type}: [{field.fieldName}] fieldType {field.fieldType} used as business key")
 
         if field.categorical and field.fieldType != meta.BasicType.STRING:
             cls._fail(f"Invalid {property_type}: [{field.fieldName}] fieldType {field.fieldType} used as categorical")
 
+        if field.businessKey and not field.notNull:
+            cls._fail(f"Invalid {property_type}: [{field.fieldName}] is a business key but not_null = False")
+
     @classmethod
     def _valid_identifiers(cls, keys, property_type):
 
         for key in keys:
             if not cls.__identifier_pattern.match(key):
                 cls._fail(f"Invalid {property_type}: [{key}] is not a valid identifier")
             if cls.__reserved_identifier_pattern.match(key):
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_plugins/aws_storage.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_plugins/storage_aws.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,283 +7,361 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+
+import typing as tp
 import http
 import io
 
-import botocore.response
+import tracdap.rt.config as cfg
+import tracdap.rt.exceptions as ex
 
+# Import storage interfaces
+import tracdap.rt.ext.plugins as plugins
 from tracdap.rt.ext.storage import *
 
-import tracdap.rt.config as _cfg
-import tracdap.rt.exceptions as _ex
-import tracdap.rt._impl.util as _util
-
-# AWS SDK
-import boto3
-import botocore.exceptions as _aws_ex  # noqa
+from pyarrow import fs as afs
 
+# Set of common helpers across the core plugins (do not reference rt._impl)
+from . import _helpers
 
-class S3ObjectStorage(IFileStorage):
 
-    # This is a quick implementation of IFileStorage on S3 using the boto3 AWS SDK
+try:
+    # AWS SDK
+    import boto3  # noqa
+    import botocore.response  # noqa
+    import botocore.exceptions as aws_ex  # noqa
+    boto_available = True
+except ImportError:
+    boto_available = False
 
-    # TODO: Migrate IFileStorage interface to use object storage as the primary concept
-    # It is much easier to express objects on a file system than vice versa
-    # This change must also be made in the Java code
 
-    # TODO: Switch to using Apache Arrow file system interface
-    # Arrow already has implementations for AWS, GCP, HDFS and local files
-    # The arrow interface also allows extension with fsspec, to support Azure blob storage or custom implementations
+class AwsStorageProvider(IStorageProvider):
 
-    # https://arrow.apache.org/docs/python/filesystems.html
+    ARROW_NATIVE_FS_PROPERTY = "arrowNativeFs"
+    ARROW_NATIVE_FS_DEFAULT = False
 
     BUCKET_PROPERTY = "bucket"
     PREFIX_PROPERTY = "prefix"
     REGION_PROPERTY = "region"
     ENDPOINT_PROPERTY = "endpoint"
 
     CREDENTIALS_PROPERTY = "credentials"
     CREDENTIALS_DEFAULT = "default"
     CREDENTIALS_STATIC = "static"
 
     ACCESS_KEY_ID_PROPERTY = "accessKeyId"
     SECRET_ACCESS_KEY_PROPERTY = "secretAccessKey"
 
-    def __init__(self, config: _cfg.PluginConfig, options: dict = None):
+    ARROW_CLIENT_ARGS = {
+        REGION_PROPERTY: "region",
+        ENDPOINT_PROPERTY: "endpoint_override",
+        ACCESS_KEY_ID_PROPERTY: "access_key",
+        SECRET_ACCESS_KEY_PROPERTY: "secret_key"
+    }
+
+    BOTO_CLIENT_ARGS = {
+        REGION_PROPERTY: "region_name",
+        ENDPOINT_PROPERTY: "endpoint_url",
+        ACCESS_KEY_ID_PROPERTY: "aws_access_key_id",
+        SECRET_ACCESS_KEY_PROPERTY: "aws_secret_access_key"
+    }
+
+    def __init__(self, properties: tp.Dict[str, str]):
+
+        self._log = _helpers.logger_for_object(self)
+        self._properties = properties
+
+        self._arrow_native = _helpers.get_plugin_property_boolean(
+            properties, self.ARROW_NATIVE_FS_PROPERTY, self.ARROW_NATIVE_FS_DEFAULT)
+
+    def has_arrow_native(self) -> bool:
+        return True if self._arrow_native else False
+
+    def has_file_storage(self) -> bool:
+        return True if not self._arrow_native and boto_available else False
+
+    def get_arrow_native(self) -> afs.SubTreeFileSystem:
+
+        s3fs_args = self.setup_client_args(self.ARROW_CLIENT_ARGS)
+        s3fs = afs.S3FileSystem(**s3fs_args)
+
+        bucket = _helpers.get_plugin_property(self._properties, self.BUCKET_PROPERTY)
+        prefix = _helpers.get_plugin_property(self._properties, self.PREFIX_PROPERTY)
+
+        if bucket is None or len(bucket.strip()) == 0:
+            message = f"Missing required config property [{self.BUCKET_PROPERTY}] for S3 storage"
+            self._log.error(message)
+            raise ex.EConfigParse(message)
+
+        root_path = f"{bucket}/{prefix}" if prefix else bucket
+
+        return afs.SubTreeFileSystem(root_path, s3fs)
+
+    def get_file_storage(self) -> IFileStorage:
+
+        client_args = self.setup_client_args(self.BOTO_CLIENT_ARGS)
+        client_args["service_name"] = "s3"
 
-        self._log = _util.logger_for_object(self)
+        config = cfg.PluginConfig()
+        config.protocol = "S3"
+        config.properties = self._properties
 
-        self._config = config
-        self._options = options
+        return S3ObjectStorage(config, client_args)
 
-        self._bucket = _util.get_plugin_property(self._config, self.BUCKET_PROPERTY)
-        self._prefix = _util.get_plugin_property(self._config, self.PREFIX_PROPERTY) or ""
-        self._region = _util.get_plugin_property(self._config, self.REGION_PROPERTY)
-        self._endpoint = _util.get_plugin_property(self._config, self.ENDPOINT_PROPERTY)
+    def setup_client_args(self, key_mapping: tp.Dict[str, str]) -> tp.Dict[str, tp.Any]:
 
-        credentials_params = self.setup_credentials()
+        client_args = dict()
 
-        client_args = {
-            "service_name": "s3",
-            **credentials_params}
+        region = _helpers.get_plugin_property(self._properties, self.REGION_PROPERTY)
+        endpoint = _helpers.get_plugin_property(self._properties, self.ENDPOINT_PROPERTY)
 
-        if self._region is not None:
-            client_args["region_name"] = self._region
+        if region is not None:
+            region_key = key_mapping[self.REGION_PROPERTY]
+            client_args[region_key] = region
 
-        if self._endpoint is not None:
-            client_args["endpoint_url"] = self._endpoint
+        if endpoint is not None:
+            endpoint_key = key_mapping[self.ENDPOINT_PROPERTY]
+            client_args[endpoint_key] = endpoint
 
-        self.__client = boto3.client(**client_args)
+        credentials = self.setup_credentials(key_mapping)
+        client_args.update(credentials)
 
-    def setup_credentials(self):
+        return client_args
 
-        mechanism = _util.get_plugin_property(self._config, self.CREDENTIALS_PROPERTY) or self.CREDENTIALS_DEFAULT
+    def setup_credentials(self, key_mapping: tp.Dict[str, str]):
 
-        if mechanism.lower() == self.CREDENTIALS_DEFAULT:
+        mechanism = _helpers.get_plugin_property(self._properties, self.CREDENTIALS_PROPERTY)
+
+        if mechanism is None or len(mechanism) == 0 or mechanism.lower() == self.CREDENTIALS_DEFAULT:
             self._log.info(f"Using [{self.CREDENTIALS_DEFAULT}] credentials mechanism")
-            return {}
+            return dict()
 
         if mechanism.lower() == self.CREDENTIALS_STATIC:
 
-            access_key_id = _util.get_plugin_property(self._config, self.ACCESS_KEY_ID_PROPERTY)
-            secret_access_key = _util.get_plugin_property(self._config, self.SECRET_ACCESS_KEY_PROPERTY)
+            access_key_id = _helpers.get_plugin_property(self._properties, self.ACCESS_KEY_ID_PROPERTY)
+            secret_access_key = _helpers.get_plugin_property(self._properties, self.SECRET_ACCESS_KEY_PROPERTY)
 
             self._log.info(
                 f"Using [{self.CREDENTIALS_STATIC}] credentials mechanism, " +
                 f"access key id = [{access_key_id}]")
 
-            return {"aws_access_key_id": access_key_id, "aws_secret_access_key": secret_access_key}
+            access_key_id_arg = key_mapping[self.ACCESS_KEY_ID_PROPERTY]
+            secret_access_key_arg = key_mapping[self.SECRET_ACCESS_KEY_PROPERTY]
+
+            return {
+                access_key_id_arg: access_key_id,
+                secret_access_key_arg: secret_access_key}
 
         message = f"Unrecognised credentials mechanism: [{mechanism}]"
         self._log.error(message)
-        raise _ex.EStartup(message)
+        raise ex.EStartup(message)
 
-    def exists(self, storage_path: str) -> bool:
 
-        try:
-            self._log.info(f"EXISTS [{storage_path}]")
+plugins.PluginManager.register_plugin(IStorageProvider, AwsStorageProvider, ["S3"])
 
-            object_key = self._resolve_path(storage_path)
-            self.__client.head_object(Bucket=self._bucket, Key=object_key)
-            return True
 
-        except _aws_ex.ClientError as error:
-            _aws_code = error.response['Error']['Code']
-            if _aws_code == str(http.HTTPStatus.NOT_FOUND.value):  # noqa
-                return False
-            raise _ex.EStorageRequest(f"Storage error: {str(error)}") from error
+# ----------------------------------------------------------------------------------------------------------------------
+# CUSTOM IMPLEMENTATION FOR S3 STORAGE
+# ----------------------------------------------------------------------------------------------------------------------
 
-    def size(self, storage_path: str) -> int:
+# This is the old implementation that was used before Arrow native was made available
+# It is likely to be removed in a future release
 
-        try:
-            self._log.info(f"SIZE [{storage_path}]")
 
-            object_key = self._resolve_path(storage_path)
-            response = self.__client.head_object(Bucket=self._bucket, Key=object_key)
-            return response['ContentLength']
+if boto_available:
 
-        except _aws_ex.ClientError as error:
-            _aws_code = error.response['Error']['Code']
-            raise _ex.EStorageRequest(f"Storage error: {str(error)}") from error
+    class S3ObjectStorage(IFileStorage):
 
-    def stat(self, storage_path: str) -> FileStat:
+        # This is a quick implementation of IFileStorage on S3 using the boto3 AWS SDK
 
-        self._log.info(f"STAT [{storage_path}]")
+        def __init__(self, config: cfg.PluginConfig, client_args: dict):
 
-        if self.exists(storage_path):
+            self._log = _helpers.logger_for_object(self)
 
-            # Only OBJECTS can support stat atm
-            # Handling for directories needs to be changed, as part of refactor onto object storage
-            size = self.size(storage_path)
-            return FileStat(FileType.FILE, size)
+            self._properties = config.properties
+            self._bucket = _helpers.get_plugin_property(self._properties, AwsStorageProvider.BUCKET_PROPERTY)
+            self._prefix = _helpers.get_plugin_property(self._properties, AwsStorageProvider.PREFIX_PROPERTY) or ""
 
-        else:
+            if self._bucket is None or len(self._bucket.strip()) == 0:
+                message = f"Missing required config property [{AwsStorageProvider.BUCKET_PROPERTY}] for S3 storage"
+                self._log.error(message)
+                raise ex.EConfigParse(message)
 
-            self.ls(storage_path)
-            return FileStat(FileType.DIRECTORY, 0)
+            self._client = boto3.client(**client_args)
 
-    def ls(self, storage_path: str) -> tp.List[str]:
+        def exists(self, storage_path: str) -> bool:
 
-        self._log.info(f"LS [{storage_path}]")
+            try:
+                self._log.info(f"EXISTS [{storage_path}]")
 
-        prefix = self._resolve_path(storage_path) + "/"
+                object_key = self._resolve_path(storage_path)
+                self._client.head_object(Bucket=self._bucket, Key=object_key)
+                return True
 
-        response = self.__client.list_objects_v2(
-            Bucket=self._bucket,
-            Prefix=prefix,
-            Delimiter="/")
+            except aws_ex.ClientError as error:
+                aws_code = error.response['Error']['Code']
+                if aws_code == str(http.HTTPStatus.NOT_FOUND.value):  # noqa
+                    return False
+                raise ex.EStorageRequest(f"Storage error: {str(error)}") from error
 
-        keys = []
+        def size(self, storage_path: str) -> int:
 
-        if "Contents" not in response and "CommonPrefixes" not in response:
-            raise _ex.EStorageRequest(f"Storage prefix not found: [{storage_path}]")
+            try:
+                self._log.info(f"SIZE [{storage_path}]")
 
-        if "Contents" in response:
-            for entry in response["Contents"]:
-                raw_key = entry["Key"]
-                if raw_key == prefix:
-                    continue
-                key = raw_key.replace(prefix, "")
-                keys.append(key)
+                object_key = self._resolve_path(storage_path)
+                response = self._client.head_object(Bucket=self._bucket, Key=object_key)
+                return response['ContentLength']
 
-        if "CommonPrefixes" in response:
-            for raw_prefix in response["CommonPrefixes"]:
-                common_prefix = raw_prefix.replace(prefix, "")
-                keys.append(common_prefix)
+            except aws_ex.ClientError as error:
+                raise ex.EStorageRequest(f"Storage error: {str(error)}") from error
 
-        return keys
+        def stat(self, storage_path: str) -> FileStat:
 
-    def mkdir(self, storage_path: str, recursive: bool = False, exists_ok: bool = False):
+            self._log.info(f"STAT [{storage_path}]")
 
-        self._log.info(f"MKDIR [{storage_path}]")
+            name = storage_path.split("/")[-1]
 
-        # No-op in object storage
-        pass
+            if self.exists(storage_path):
 
-    def rm(self, storage_path: str, recursive: bool = False):
+                # Only OBJECTS can support stat atm
+                # Handling for directories needs to be changed, as part of refactor onto object storage
+                size = self.size(storage_path)
+                return FileStat(name, FileType.FILE, storage_path, size)
 
-        try:
-            self._log.info(f"RM [{storage_path}]")
+            else:
 
-            if recursive:
-                raise RuntimeError("RM (recursive) not available for S3 storage")
+                self.ls(storage_path)
+                return FileStat(name, FileType.DIRECTORY, storage_path, 0)
 
-            object_key = self._resolve_path(storage_path)
-            self.__client.delete_object(Bucket=self._bucket, Key=object_key)
+        def ls(self, storage_path: str, recursive: bool = False) -> tp.List[FileStat]:
 
-        except _aws_ex.ClientError as error:
-            _aws_code = error.response['Error']['Code']
-            raise _ex.EStorageRequest(f"Storage error: {str(error)}") from error
+            self._log.info(f"LS [{storage_path}]")
 
-    def read_bytes(self, storage_path: str) -> bytes:
+            prefix = self._resolve_path(storage_path) + "/"
 
-        self._log.info(f"READ BYTES [{storage_path}]")
+            response = self._client.list_objects_v2(
+                Bucket=self._bucket,
+                Prefix=prefix,
+                Delimiter="/")
 
-        body = self._read_impl(storage_path)
-        return body.read()
+            keys = []
 
-    def read_byte_stream(self, storage_path: str) -> tp.BinaryIO:
+            if "Contents" not in response and "CommonPrefixes" not in response:
+                raise ex.EStorageRequest(f"Storage prefix not found: [{storage_path}]")
 
-        self._log.info(f"READ BYTE STREAM [{storage_path}]")
+            if "Contents" in response:
+                for entry in response["Contents"]:
+                    raw_key = entry["Key"]
+                    if raw_key == prefix:
+                        continue
+                    key = raw_key.replace(prefix, "")
+                    size = entry["Size"]
+                    mtime = entry["LastModified "]
+                    stat = FileStat(key, FileType.FILE, raw_key, size, mtime=mtime)
+                    keys.append(stat)
 
-        data = self.read_bytes(storage_path)
-        return io.BytesIO(data)
+            if "CommonPrefixes" in response:
+                for raw_prefix in response["CommonPrefixes"]:
+                    common_prefix = raw_prefix.replace(prefix, "")
+                    stat = FileStat(common_prefix, FileType.DIRECTORY, raw_prefix, 0)
+                    keys.append(stat)
 
-    def _read_impl(self, storage_path: str) -> botocore.response.StreamingBody:
+            return keys
 
-        try:
+        def mkdir(self, storage_path: str, recursive: bool = False):
 
-            object_key = self._resolve_path(storage_path)
-            response = self.__client.get_object(Bucket=self._bucket, Key=object_key)
-            return response['Body']
+            self._log.info(f"MKDIR [{storage_path}]")
 
-        except _aws_ex.ClientError as error:
-            _aws_code = error.response['Error']['Code']
-            raise _ex.EStorageRequest(f"Storage error: {str(error)}") from error
+            # No-op in object storage
+            pass
 
-    def write_bytes(self, storage_path: str, data: bytes, overwrite: bool = False):
+        def rm(self, storage_path: str):
 
-        try:
-            self._log.info(f"WRITE BYTES [{storage_path}]")
+            try:
+                self._log.info(f"RM [{storage_path}]")
 
-            object_key = self._resolve_path(storage_path)
+                object_key = self._resolve_path(storage_path)
+                self._client.delete_object(Bucket=self._bucket, Key=object_key)
 
-            self.__client.put_object(
-                Bucket=self._bucket,
-                Key=object_key,
-                Body=data)
+            except aws_ex.ClientError as error:
+                raise ex.EStorageRequest(f"Storage error: {str(error)}") from error
+
+        def rmdir(self, storage_path: str):
+
+            raise RuntimeError("RMDIR (recursive) not available for S3 storage")
+
+        def read_bytes(self, storage_path: str) -> bytes:
+
+            self._log.info(f"READ BYTES [{storage_path}]")
+
+            body = self._read_impl(storage_path)
+            return body.read()
+
+        def read_byte_stream(self, storage_path: str) -> tp.BinaryIO:
+
+            self._log.info(f"READ BYTE STREAM [{storage_path}]")
+
+            data = self.read_bytes(storage_path)
+            return io.BytesIO(data)
+
+        def _read_impl(self, storage_path: str) -> botocore.response.StreamingBody:
+
+            try:
+
+                object_key = self._resolve_path(storage_path)
+                response = self._client.get_object(Bucket=self._bucket, Key=object_key)
+                return response['Body']
 
-        except _aws_ex.ClientError as error:
-            _aws_code = error.response['Error']['Code']
-            raise _ex.EStorageRequest(f"Storage error: {str(error)}") from error
+            except aws_ex.ClientError as error:
+                raise ex.EStorageRequest(f"Storage error: {str(error)}") from error
 
-    def write_byte_stream(self, storage_path: str, overwrite: bool = False) -> tp.BinaryIO:
+        def write_bytes(self, storage_path: str, data: bytes):
 
-        self._log.info(f"WRITE BYTE STREAM [{storage_path}]")
+            try:
+                self._log.info(f"WRITE BYTES [{storage_path}]")
 
-        return self._AwsWriteBuf(self, storage_path, overwrite)
+                object_key = self._resolve_path(storage_path)
 
-    class _AwsWriteBuf(io.BytesIO):
+                self._client.put_object(
+                    Bucket=self._bucket,
+                    Key=object_key,
+                    Body=data)
 
-        def __init__(self, storage, storage_path, overwrite: bool):
-            super().__init__()
-            self._storage = storage
-            self._storage_path = storage_path
-            self._overwrite = overwrite
-            self._written = False
+            except aws_ex.ClientError as error:
+                raise ex.EStorageRequest(f"Storage error: {str(error)}") from error
 
-        def close(self):
-            if not self._written:
-                self.seek(0)
-                data = self.read()
-                self._storage.write_bytes(self._storage_path, data, self._overwrite)
-                self._written = True
+        def write_byte_stream(self, storage_path: str) -> tp.BinaryIO:
 
-    # TODO: These methods can be removed from the interface, they are not needed
-    # (storage layer only needs to work in binary mode)
+            self._log.info(f"WRITE BYTE STREAM [{storage_path}]")
 
-    def read_text(self, storage_path: str, encoding: str = 'utf-8') -> str:
-        raise RuntimeError("READ (text mode) not available for S3 storage")
+            return self._AwsWriteBuf(self, storage_path)
 
-    def read_text_stream(self, storage_path: str, encoding: str = 'utf-8') -> tp.TextIO:
-        raise RuntimeError("READ (text mode) not available for S3 storage")
+        class _AwsWriteBuf(io.BytesIO):
 
-    def write_text(self, storage_path: str, data: str, encoding: str = 'utf-8', overwrite: bool = False):
-        raise RuntimeError("WRITE (text mode) not available for S3 storage")
+            def __init__(self, storage, storage_path):
+                super().__init__()
+                self._storage = storage
+                self._storage_path = storage_path
+                self._written = False
 
-    def write_text_stream(self, storage_path: str, encoding: str = 'utf-8', overwrite: bool = False) -> tp.TextIO:
-        raise RuntimeError("WRITE (text mode) not available for S3 storage")
+            def close(self):
+                if not self._written:
+                    self.seek(0)
+                    data = self.read()
+                    self._storage.write_bytes(self._storage_path, data)
+                    self._written = True
 
-    def _resolve_path(self, storage_path: str) -> str:
+        def _resolve_path(self, storage_path: str) -> str:
 
-        if self._prefix is None or self._prefix.strip() == "":
-            return storage_path
+            if self._prefix is None or self._prefix.strip() == "":
+                return storage_path
 
-        separator = "" if self._prefix.endswith("/") else "/"
-        full_path = self._prefix + separator + storage_path
+            separator = "" if self._prefix.endswith("/") else "/"
+            full_path = self._prefix + separator + storage_path
 
-        return full_path[1:] if full_path.startswith("/") else full_path
+            return full_path[1:] if full_path.startswith("/") else full_path
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/_version.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.5.9"
+__version__ = "0.6.0rc1"
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/api/__init__.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/api/hook.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/api/hook.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             -> _tp.Dict[str, _meta.ModelParameter]:
 
         pass
 
     @_abc.abstractmethod
     def define_field(
             self, field_name: str, field_type: _meta.BasicType, label: str,
-            business_key: bool = False, categorical: bool = False,
+            business_key: bool = False, categorical: bool = False, not_null: _tp.Optional[bool] = None,
             format_code: _tp.Optional[str] = None, field_order: _tp.Optional[int] = None) \
             -> _meta.FieldSchema:
 
         pass
 
     @_abc.abstractmethod
     def define_schema(
@@ -115,18 +115,18 @@
             schema_type: _meta.SchemaType = _meta.SchemaType.TABLE) \
             -> _meta.SchemaDefinition:
 
         pass
 
     @_abc.abstractmethod
     def define_input_table(
-            self, *fields: _tp.Union[_meta.FieldSchema, _tp.List[_meta.FieldSchema]]) \
+            self, *fields: _tp.Union[_meta.FieldSchema, _tp.List[_meta.FieldSchema]], label: _tp.Optional[str] = None) \
             -> _meta.ModelInputSchema:
 
         pass
 
     @_abc.abstractmethod
     def define_output_table(
-            self, *fields: _tp.Union[_meta.FieldSchema, _tp.List[_meta.FieldSchema]]) \
+            self, *fields: _tp.Union[_meta.FieldSchema, _tp.List[_meta.FieldSchema]], label: _tp.Optional[str] = None) \
             -> _meta.ModelOutputSchema:
 
         pass
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/api/model_api.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/api/model_api.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/api/static_api.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/api/static_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,15 +121,16 @@
     The name, type and label are required fields to define a parameter. Name is used as the identifier
     to work with the parameter in code, e.g. when calling :py:meth:`get_parameter` or defining parameters
     in a job config.
 
     If a default value is specified, the model parameter becomes optional. It is ok to omit optional parameters
     when running models or setting up jobs, in which case the default value will be used. If no default is
     specified then the model parameter becomes mandatory, a value must always be supplied in order to execute
-    the model.
+    the model. TRAC will apply type coercion where possible to ensure the default value matches the parameter type,
+    if the default value cannot be coerced to match the parameter type then model validation will fail.
 
     Once defined model parameters can be passed to :py:func:`define_parameters`,
     either as a list or as individual arguments, to create the set of parameters for a model.
 
     :param param_name: The parameter name, used to identify the parameter in code (must be a valid identifier)
     :param param_type: The parameter type, expressed in the TRAC type system
     :param label: A descriptive label for the parameter (required)
@@ -235,117 +236,126 @@
 
 def define_field(
         field_name: str,
         field_type: BasicType,
         label: str,
         business_key: bool = False,
         categorical: bool = False,
+        not_null: _tp.Optional[bool] = None,
         format_code: _tp.Optional[str] = None,
         field_order: _tp.Optional[int] = None) \
         -> FieldSchema:
 
     """
     Define the schema for an individual field, which can be used in a model input or output schema.
 
     Individual fields in a dataset can be defined using this method or the shorthand alias :py:func:`F`.
     The name, type and label of a field are always required.
     The business_key and categorical flags are false by default.
+    The not_null flag is false by default unless the field is a business key, in which case it is true by default.
+    Explicitly specifying not_null=False for a business key will cause a validation error.
     Format code is optional.
 
     If no field ordering is supplied, fields will automatically be assigned a contiguous ordering starting at 0.
     In this case care must be taken when creating an updated version of a model, that the order of existing
     fields is not disturbed. Adding fields to the end of a list is always safe.
-    If field orders are specified explicitly, the must for a contiguous ordering starting at 0.
+    If field orders are specified explicitly, they must form a contiguous ordering starting at 0.
 
     Once defined field schemas can be passed to :py:func:`define_input_table` or :py:func:`define_output_table`,
     either as a list or as individual arguments, to create the full schema for an input or output.
 
     :param field_name: The field's name, used as the field identifier in code and queries (must be a valid identifier)
     :param field_type: The data type of the field, only primitive types are allowed
     :param label: A descriptive label for the field (required)
     :param business_key: Flag indicating whether this field is a business key for its dataset (default: False)
     :param categorical: Flag indicating whether this is a categorical field (default: False)
+    :param not_null: Whether this field has a not null constraint (default: True for business keys, false otherwise)
     :param format_code: A code that can be interpreted by client applications to format the field (optional)
     :param field_order: Explicit field ordering (optional)
     :return: A field schema, suitable for use in a schema definition
 
     :type field_name: str
     :type field_type: :py:class:`BasicType <tracdap.rt.metadata.BasicType>`
     :type label: str
     :type business_key: bool
     :type categorical: bool
+    :type not_null: _tp.Optional[bool]
     :type format_code: _tp.Optional[str]
     :type field_order: _tp.Optional[int]
     :rtype: :py:class:`FieldSchema <tracdap.rt.metadata.FieldSchema>`
     """
 
     sa = _StaticApiHook.get_instance()
 
     return sa.define_field(
         field_name, field_type, label,
-        business_key, categorical,
+        business_key, categorical, not_null,
         format_code, field_order)
 
 
 def declare_field(
         field_name: str,
         field_type: BasicType,
         label: str,
         business_key: bool = False,
         categorical: bool = False,
+        not_null: _tp.Optional[bool] = None,
         format_code: _tp.Optional[str] = None,
         field_order: _tp.Optional[int] = None) \
         -> FieldSchema:
 
     """
     .. deprecated:: 0.4.4
        Use :py:func:`define_field` or :py:func:`F` instead.
 
     :type field_name: str
     :type field_type: :py:class:`BasicType <tracdap.rt.metadata.BasicType>`
     :type label: str
     :type business_key: bool
     :type categorical: bool
+    :type not_null: _tp.Optional[bool]
     :type format_code: _tp.Optional[str]
     :type field_order: _tp.Optional[int]
     :rtype: :py:class:`FieldSchema <tracdap.rt.metadata.FieldSchema>`
     """
 
     return define_field(
         field_name, field_type, label,
-        business_key, categorical,
+        business_key, categorical, not_null,
         format_code, field_order)
 
 
 def F(  # noqa
         field_name: str,
         field_type: BasicType,
         label: str,
         business_key: bool = False,
         categorical: bool = False,
+        not_null: _tp.Optional[bool] = None,
         format_code: _tp.Optional[str] = None,
         field_order: _tp.Optional[int] = None) \
         -> FieldSchema:
 
     """
     Shorthand alias for :py:func:`define_field`
 
     :type field_name: str
     :type field_type: :py:class:`BasicType <tracdap.rt.metadata.BasicType>`
     :type label: str
     :type business_key: bool
     :type categorical: bool
+    :type not_null: _tp.Optional[bool]
     :type format_code: _tp.Optional[str]
     :type field_order: _tp.Optional[int]
     :rtype: :py:class:`FieldSchema <tracdap.rt.metadata.FieldSchema>`
     """
 
     return define_field(
         field_name, field_type, label,
-        business_key, categorical,
+        business_key, categorical, not_null,
         format_code, field_order)
 
 
 def define_schema(
         *fields: _tp.Union[FieldSchema, _tp.List[FieldSchema]],
         schema_type: SchemaType = SchemaType.TABLE) \
         -> SchemaDefinition:
@@ -413,33 +423,34 @@
     """
 
     sa = _StaticApiHook.get_instance()
     return sa.load_schema(package, schema_file, schema_type=schema_type)
 
 
 def define_input_table(
-        *fields: _tp.Union[FieldSchema, _tp.List[FieldSchema]]) \
+        *fields: _tp.Union[FieldSchema, _tp.List[FieldSchema]], label: _tp.Optional[str] = None) \
         -> ModelInputSchema:
 
     """
     Define a model input with a table schema.
 
     Fields can be supplied either as individual arguments to this function or as a list.
     Individual fields should be defined using :py:func:`define_field` or the shorthand alias :py:func:`F`.
 
     :param fields: A set of fields to make up a :py:class:`TableSchema <tracdap.rt.metadata.TableSchema>`
+    :param label: An optional label (of type str) for a model input schema. Default value: None.
     :return: A model input schema, suitable for returning from :py:meth:`TracModel.define_inputs`
 
     :type fields: :py:class:`FieldSchema <tracdap.rt.metadata.FieldSchema>` |
                   List[:py:class:`FieldSchema <tracdap.rt.metadata.FieldSchema>`]
     :rtype: :py:class:`ModelInputSchema <tracdap.rt.metadata.ModelInputSchema>`
     """
 
     sa = _StaticApiHook.get_instance()
-    return sa.define_input_table(*fields)
+    return sa.define_input_table(*fields, label=label)
 
 
 def declare_input_table(
         *fields: _tp.Union[FieldSchema, _tp.List[FieldSchema]]) \
         -> ModelInputSchema:
 
     """
@@ -451,33 +462,34 @@
     :rtype: :py:class:`ModelInputSchema <tracdap.rt.metadata.ModelInputSchema>`
     """
 
     return define_input_table(*fields)
 
 
 def define_output_table(
-        *fields: _tp.Union[FieldSchema, _tp.List[FieldSchema]]) \
+        *fields: _tp.Union[FieldSchema, _tp.List[FieldSchema]], label: _tp.Optional[str] = None) \
         -> ModelOutputSchema:
 
     """
     Define a model output with a table schema.
 
     Fields can be supplied either as individual arguments to this function or as a list.
     Individual fields should be defined using :py:func:`define_field` or the shorthand alias :py:func:`F`.
 
     :param fields: A set of fields to make up a :py:class:`TableSchema <tracdap.rt.metadata.TableSchema>`
+    :param label: An optional label (of type str) for a model output schema. Default value: None.
     :return: A model output schema, suitable for returning from :py:meth:`TracModel.define_outputs`
 
     :type fields: :py:class:`FieldSchema <tracdap.rt.metadata.FieldSchema>` |
                   List[:py:class:`FieldSchema <tracdap.rt.metadata.FieldSchema>`]
     :rtype: :py:class:`ModelOutputSchema <tracdap.rt.metadata.ModelOutputSchema>`
     """
 
     sa = _StaticApiHook.get_instance()
-    return sa.define_output_table(*fields)
+    return sa.define_output_table(*fields, label=label)
 
 
 def declare_output_table(
         *fields: _tp.Union[FieldSchema, _tp.List[FieldSchema]]) \
         -> ModelOutputSchema:
 
     """
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/config/__init__.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # Code generated by TRAC
 
+from .job import JobConfig
+
+from .result import TagUpdateList
+from .result import JobResult
+
 from .common import _ConfigFile
 from .common import PluginConfig
 from .common import PlatformInfo
 from .common import AuthenticationConfig
 
-from .gateway import GwProtocol
-from .gateway import GwRestMapping
-from .gateway import GatewayConfig
-from .gateway import GwRoute
-from .gateway import GwMatch
-from .gateway import GwTarget
-from .gateway import GwServiceMap
-from .gateway import GwService
-
 from .platform import PlatformConfig
 from .platform import MetadataConfig
 from .platform import StorageConfig
 from .platform import TenantConfig
+from .platform import WebServerConfig
+from .platform import WebServerRewriteRule
+from .platform import WebServerRedirect
 from .platform import InstantMap
 from .platform import InstanceConfig
 from .platform import ServiceMap
 from .platform import ServiceConfig
 
 from .runtime import RuntimeConfig
 from .runtime import SparkSettings
 
-from .job import JobConfig
-
-from .result import TagUpdateList
-from .result import JobResult
+from .gateway import GwProtocol
+from .gateway import GwRestMapping
+from .gateway import GatewayConfig
+from .gateway import GwRoute
+from .gateway import GwMatch
+from .gateway import GwTarget
+from .gateway import GwServiceMap
+from .gateway import GwService
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/config/common.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -44,7 +44,15 @@
     jwtRefresh: int = None
 
     provider: _tp.Optional[PluginConfig] = None
 
     disableAuth: bool = None
 
     disableSigning: bool = None
+
+    systemUserId: str = None
+
+    systemUserName: str = None
+
+    systemTicketDuration: int = None
+
+    systemTicketRefresh: int = None
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/config/common_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/common_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1btracdap/config/common.proto\x12\x0etracdap.config\"u\n\x0b_ConfigFile\x12\x37\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\'.tracdap.config._ConfigFile.ConfigEntry\x1a-\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x81\x02\n\x0cPluginConfig\x12\x10\n\x08protocol\x18\x01 \x01(\t\x12@\n\nproperties\x18\x02 \x03(\x0b\x32,.tracdap.config.PluginConfig.PropertiesEntry\x12:\n\x07secrets\x18\x03 \x03(\x0b\x32).tracdap.config.PluginConfig.SecretsEntry\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cSecretsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb8\x01\n\x0cPlatformInfo\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x12\n\nproduction\x18\x02 \x01(\x08\x12H\n\x0e\x64\x65ploymentInfo\x18\x03 \x03(\x0b\x32\x30.tracdap.config.PlatformInfo.DeploymentInfoEntry\x1a\x35\n\x13\x44\x65ploymentInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xd1\x01\n\x14\x41uthenticationConfig\x12\x11\n\tjwtIssuer\x18\x01 \x01(\t\x12\x11\n\tjwtExpiry\x18\x02 \x01(\x11\x12\x10\n\x08jwtLimit\x18\x06 \x01(\x11\x12\x12\n\njwtRefresh\x18\x07 \x01(\x11\x12\x33\n\x08provider\x18\x03 \x01(\x0b\x32\x1c.tracdap.config.PluginConfigH\x00\x88\x01\x01\x12\x13\n\x0b\x64isableAuth\x18\x04 \x01(\x08\x12\x16\n\x0e\x64isableSigning\x18\x05 \x01(\x08\x42\x0b\n\t_providerB\x1c\n\x18org.finos.tracdap.configP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1btracdap/config/common.proto\x12\x0etracdap.config\"u\n\x0b_ConfigFile\x12\x37\n\x06\x63onfig\x18\x01 \x03(\x0b\x32\'.tracdap.config._ConfigFile.ConfigEntry\x1a-\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x81\x02\n\x0cPluginConfig\x12\x10\n\x08protocol\x18\x01 \x01(\t\x12@\n\nproperties\x18\x02 \x03(\x0b\x32,.tracdap.config.PluginConfig.PropertiesEntry\x12:\n\x07secrets\x18\x03 \x03(\x0b\x32).tracdap.config.PluginConfig.SecretsEntry\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a.\n\x0cSecretsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb8\x01\n\x0cPlatformInfo\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t\x12\x12\n\nproduction\x18\x02 \x01(\x08\x12H\n\x0e\x64\x65ploymentInfo\x18\x03 \x03(\x0b\x32\x30.tracdap.config.PlatformInfo.DeploymentInfoEntry\x1a\x35\n\x13\x44\x65ploymentInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xba\x02\n\x14\x41uthenticationConfig\x12\x11\n\tjwtIssuer\x18\x01 \x01(\t\x12\x11\n\tjwtExpiry\x18\x02 \x01(\x11\x12\x10\n\x08jwtLimit\x18\x06 \x01(\x11\x12\x12\n\njwtRefresh\x18\x07 \x01(\x11\x12\x33\n\x08provider\x18\x03 \x01(\x0b\x32\x1c.tracdap.config.PluginConfigH\x00\x88\x01\x01\x12\x13\n\x0b\x64isableAuth\x18\x04 \x01(\x08\x12\x16\n\x0e\x64isableSigning\x18\x05 \x01(\x08\x12\x14\n\x0csystemUserId\x18\x08 \x01(\t\x12\x16\n\x0esystemUserName\x18\t \x01(\t\x12\x1c\n\x14systemTicketDuration\x18\n \x01(\x11\x12\x1b\n\x13systemTicketRefresh\x18\x0b \x01(\x11\x42\x0b\n\t_providerB\x1c\n\x18org.finos.tracdap.configP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tracdap.config.common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\030org.finos.tracdap.configP\001'
@@ -40,9 +40,9 @@
   _PLUGINCONFIG_SECRETSENTRY._serialized_start=378
   _PLUGINCONFIG_SECRETSENTRY._serialized_end=424
   _PLATFORMINFO._serialized_start=427
   _PLATFORMINFO._serialized_end=611
   _PLATFORMINFO_DEPLOYMENTINFOENTRY._serialized_start=558
   _PLATFORMINFO_DEPLOYMENTINFOENTRY._serialized_end=611
   _AUTHENTICATIONCONFIG._serialized_start=614
-  _AUTHENTICATIONCONFIG._serialized_end=823
+  _AUTHENTICATIONCONFIG._serialized_end=928
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/config/gateway.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/gateway.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/config/gateway_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/gateway_pb2.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/config/job.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/job.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/config/job_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/job_pb2.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/config/platform.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/platform.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,16 +23,20 @@
 
     storage: StorageConfig = None
 
     repositories: _tp.Dict[str, PluginConfig] = _dc.field(default_factory=dict)
 
     executor: PluginConfig = None
 
+    jobCache: PluginConfig = None
+
     tenants: _tp.Dict[str, TenantConfig] = _dc.field(default_factory=dict)
 
+    webServer: _tp.Optional[WebServerConfig] = None
+
     instances: InstantMap = None
 
     services: ServiceMap = None
 
 
 @_dc.dataclass
 class MetadataConfig:
@@ -57,14 +61,46 @@
 
     defaultBucket: _tp.Optional[str] = None
 
     defaultFormat: _tp.Optional[str] = None
 
 
 @_dc.dataclass
+class WebServerConfig:
+
+    enabled: bool = None
+
+    port: int = None
+
+    contentRoot: PluginConfig = None
+
+    rewriteRules: _tp.List[WebServerRewriteRule] = _dc.field(default_factory=list)
+
+    redirects: _tp.List[WebServerRedirect] = _dc.field(default_factory=list)
+
+
+@_dc.dataclass
+class WebServerRewriteRule:
+
+    source: str = None
+
+    target: str = None
+
+
+@_dc.dataclass
+class WebServerRedirect:
+
+    source: str = None
+
+    target: str = None
+
+    status: int = None
+
+
+@_dc.dataclass
 class InstantMap:
 
     meta: _tp.List[InstanceConfig] = _dc.field(default_factory=list)
 
     data: _tp.List[InstanceConfig] = _dc.field(default_factory=list)
 
     orch: _tp.List[InstanceConfig] = _dc.field(default_factory=list)
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/config/platform_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/platform_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from tracdap.metadata import common_pb2 as tracdap_dot_metadata_dot_common__pb2
 from tracdap.config import common_pb2 as tracdap_dot_config_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dtracdap/config/platform.proto\x12\x0etracdap.config\x1a\x1dtracdap/metadata/common.proto\x1a\x1btracdap/config/common.proto\"\x83\x06\n\x0ePlatformConfig\x12:\n\x06\x63onfig\x18\x01 \x03(\x0b\x32*.tracdap.config.PlatformConfig.ConfigEntry\x12\x32\n\x0cplatformInfo\x18\x02 \x01(\x0b\x32\x1c.tracdap.config.PlatformInfo\x12<\n\x0e\x61uthentication\x18\x05 \x01(\x0b\x32$.tracdap.config.AuthenticationConfig\x12\x30\n\x08metadata\x18\x06 \x01(\x0b\x32\x1e.tracdap.config.MetadataConfig\x12.\n\x07storage\x18\x07 \x01(\x0b\x32\x1d.tracdap.config.StorageConfig\x12\x46\n\x0crepositories\x18\x08 \x03(\x0b\x32\x30.tracdap.config.PlatformConfig.RepositoriesEntry\x12.\n\x08\x65xecutor\x18\t \x01(\x0b\x32\x1c.tracdap.config.PluginConfig\x12<\n\x07tenants\x18\n \x03(\x0b\x32+.tracdap.config.PlatformConfig.TenantsEntry\x12-\n\tinstances\x18\x03 \x01(\x0b\x32\x1a.tracdap.config.InstantMap\x12,\n\x08services\x18\x04 \x01(\x0b\x32\x1a.tracdap.config.ServiceMap\x1a-\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1aQ\n\x11RepositoriesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.tracdap.config.PluginConfig:\x02\x38\x01\x1aL\n\x0cTenantsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.tracdap.config.TenantConfig:\x02\x38\x01\"r\n\x0eMetadataConfig\x12.\n\x08\x64\x61tabase\x18\x01 \x01(\x0b\x32\x1c.tracdap.config.PluginConfig\x12\x30\n\x06\x66ormat\x18\x02 \x01(\x0e\x32 .tracdap.metadata.MetadataFormat\"\xc8\x01\n\rStorageConfig\x12;\n\x07\x62uckets\x18\x01 \x03(\x0b\x32*.tracdap.config.StorageConfig.BucketsEntry\x12\x15\n\rdefaultBucket\x18\x02 \x01(\t\x12\x15\n\rdefaultFormat\x18\x03 \x01(\t\x1aL\n\x0c\x42ucketsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.tracdap.config.PluginConfig:\x02\x38\x01\"j\n\x0cTenantConfig\x12\x1a\n\rdefaultBucket\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x1a\n\rdefaultFormat\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x10\n\x0e_defaultBucketB\x10\n\x0e_defaultFormat\"\x96\x01\n\nInstantMap\x12,\n\x04meta\x18\x01 \x03(\x0b\x32\x1e.tracdap.config.InstanceConfig\x12,\n\x04\x64\x61ta\x18\x02 \x03(\x0b\x32\x1e.tracdap.config.InstanceConfig\x12,\n\x04orch\x18\x03 \x03(\x0b\x32\x1e.tracdap.config.InstanceConfig\"<\n\x0eInstanceConfig\x12\x0e\n\x06scheme\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x0c\n\x04port\x18\x03 \x01(\r\"\x93\x01\n\nServiceMap\x12+\n\x04meta\x18\x01 \x01(\x0b\x32\x1d.tracdap.config.ServiceConfig\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.tracdap.config.ServiceConfig\x12+\n\x04orch\x18\x03 \x01(\x0b\x32\x1d.tracdap.config.ServiceConfig\"\x1d\n\rServiceConfig\x12\x0c\n\x04port\x18\x01 \x01(\rB\x1c\n\x18org.finos.tracdap.configP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dtracdap/config/platform.proto\x12\x0etracdap.config\x1a\x1dtracdap/metadata/common.proto\x1a\x1btracdap/config/common.proto\"\xfa\x06\n\x0ePlatformConfig\x12:\n\x06\x63onfig\x18\x01 \x03(\x0b\x32*.tracdap.config.PlatformConfig.ConfigEntry\x12\x32\n\x0cplatformInfo\x18\x02 \x01(\x0b\x32\x1c.tracdap.config.PlatformInfo\x12<\n\x0e\x61uthentication\x18\x05 \x01(\x0b\x32$.tracdap.config.AuthenticationConfig\x12\x30\n\x08metadata\x18\x06 \x01(\x0b\x32\x1e.tracdap.config.MetadataConfig\x12.\n\x07storage\x18\x07 \x01(\x0b\x32\x1d.tracdap.config.StorageConfig\x12\x46\n\x0crepositories\x18\x08 \x03(\x0b\x32\x30.tracdap.config.PlatformConfig.RepositoriesEntry\x12.\n\x08\x65xecutor\x18\t \x01(\x0b\x32\x1c.tracdap.config.PluginConfig\x12.\n\x08jobCache\x18\x0c \x01(\x0b\x32\x1c.tracdap.config.PluginConfig\x12<\n\x07tenants\x18\n \x03(\x0b\x32+.tracdap.config.PlatformConfig.TenantsEntry\x12\x37\n\twebServer\x18\x0b \x01(\x0b\x32\x1f.tracdap.config.WebServerConfigH\x00\x88\x01\x01\x12-\n\tinstances\x18\x03 \x01(\x0b\x32\x1a.tracdap.config.InstantMap\x12,\n\x08services\x18\x04 \x01(\x0b\x32\x1a.tracdap.config.ServiceMap\x1a-\n\x0b\x43onfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1aQ\n\x11RepositoriesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.tracdap.config.PluginConfig:\x02\x38\x01\x1aL\n\x0cTenantsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.tracdap.config.TenantConfig:\x02\x38\x01\x42\x0c\n\n_webServer\"r\n\x0eMetadataConfig\x12.\n\x08\x64\x61tabase\x18\x01 \x01(\x0b\x32\x1c.tracdap.config.PluginConfig\x12\x30\n\x06\x66ormat\x18\x02 \x01(\x0e\x32 .tracdap.metadata.MetadataFormat\"\xc8\x01\n\rStorageConfig\x12;\n\x07\x62uckets\x18\x01 \x03(\x0b\x32*.tracdap.config.StorageConfig.BucketsEntry\x12\x15\n\rdefaultBucket\x18\x02 \x01(\t\x12\x15\n\rdefaultFormat\x18\x03 \x01(\t\x1aL\n\x0c\x42ucketsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.tracdap.config.PluginConfig:\x02\x38\x01\"j\n\x0cTenantConfig\x12\x1a\n\rdefaultBucket\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x1a\n\rdefaultFormat\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x10\n\x0e_defaultBucketB\x10\n\x0e_defaultFormat\"\xd5\x01\n\x0fWebServerConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x31\n\x0b\x63ontentRoot\x18\x03 \x01(\x0b\x32\x1c.tracdap.config.PluginConfig\x12:\n\x0crewriteRules\x18\x04 \x03(\x0b\x32$.tracdap.config.WebServerRewriteRule\x12\x34\n\tredirects\x18\x05 \x03(\x0b\x32!.tracdap.config.WebServerRedirect\"6\n\x14WebServerRewriteRule\x12\x0e\n\x06source\x18\x01 \x01(\t\x12\x0e\n\x06target\x18\x02 \x01(\t\"C\n\x11WebServerRedirect\x12\x0e\n\x06source\x18\x01 \x01(\t\x12\x0e\n\x06target\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\x05\"\x96\x01\n\nInstantMap\x12,\n\x04meta\x18\x01 \x03(\x0b\x32\x1e.tracdap.config.InstanceConfig\x12,\n\x04\x64\x61ta\x18\x02 \x03(\x0b\x32\x1e.tracdap.config.InstanceConfig\x12,\n\x04orch\x18\x03 \x03(\x0b\x32\x1e.tracdap.config.InstanceConfig\"<\n\x0eInstanceConfig\x12\x0e\n\x06scheme\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x0c\n\x04port\x18\x03 \x01(\r\"\x93\x01\n\nServiceMap\x12+\n\x04meta\x18\x01 \x01(\x0b\x32\x1d.tracdap.config.ServiceConfig\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.tracdap.config.ServiceConfig\x12+\n\x04orch\x18\x03 \x01(\x0b\x32\x1d.tracdap.config.ServiceConfig\"\x1d\n\rServiceConfig\x12\x0c\n\x04port\x18\x01 \x01(\rB\x1c\n\x18org.finos.tracdap.configP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tracdap.config.platform_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\030org.finos.tracdap.configP\001'
@@ -28,31 +28,37 @@
   _PLATFORMCONFIG_REPOSITORIESENTRY._options = None
   _PLATFORMCONFIG_REPOSITORIESENTRY._serialized_options = b'8\001'
   _PLATFORMCONFIG_TENANTSENTRY._options = None
   _PLATFORMCONFIG_TENANTSENTRY._serialized_options = b'8\001'
   _STORAGECONFIG_BUCKETSENTRY._options = None
   _STORAGECONFIG_BUCKETSENTRY._serialized_options = b'8\001'
   _PLATFORMCONFIG._serialized_start=110
-  _PLATFORMCONFIG._serialized_end=881
-  _PLATFORMCONFIG_CONFIGENTRY._serialized_start=675
-  _PLATFORMCONFIG_CONFIGENTRY._serialized_end=720
-  _PLATFORMCONFIG_REPOSITORIESENTRY._serialized_start=722
-  _PLATFORMCONFIG_REPOSITORIESENTRY._serialized_end=803
-  _PLATFORMCONFIG_TENANTSENTRY._serialized_start=805
-  _PLATFORMCONFIG_TENANTSENTRY._serialized_end=881
-  _METADATACONFIG._serialized_start=883
-  _METADATACONFIG._serialized_end=997
-  _STORAGECONFIG._serialized_start=1000
-  _STORAGECONFIG._serialized_end=1200
-  _STORAGECONFIG_BUCKETSENTRY._serialized_start=1124
-  _STORAGECONFIG_BUCKETSENTRY._serialized_end=1200
-  _TENANTCONFIG._serialized_start=1202
-  _TENANTCONFIG._serialized_end=1308
-  _INSTANTMAP._serialized_start=1311
-  _INSTANTMAP._serialized_end=1461
-  _INSTANCECONFIG._serialized_start=1463
-  _INSTANCECONFIG._serialized_end=1523
-  _SERVICEMAP._serialized_start=1526
-  _SERVICEMAP._serialized_end=1673
-  _SERVICECONFIG._serialized_start=1675
-  _SERVICECONFIG._serialized_end=1704
+  _PLATFORMCONFIG._serialized_end=1000
+  _PLATFORMCONFIG_CONFIGENTRY._serialized_start=780
+  _PLATFORMCONFIG_CONFIGENTRY._serialized_end=825
+  _PLATFORMCONFIG_REPOSITORIESENTRY._serialized_start=827
+  _PLATFORMCONFIG_REPOSITORIESENTRY._serialized_end=908
+  _PLATFORMCONFIG_TENANTSENTRY._serialized_start=910
+  _PLATFORMCONFIG_TENANTSENTRY._serialized_end=986
+  _METADATACONFIG._serialized_start=1002
+  _METADATACONFIG._serialized_end=1116
+  _STORAGECONFIG._serialized_start=1119
+  _STORAGECONFIG._serialized_end=1319
+  _STORAGECONFIG_BUCKETSENTRY._serialized_start=1243
+  _STORAGECONFIG_BUCKETSENTRY._serialized_end=1319
+  _TENANTCONFIG._serialized_start=1321
+  _TENANTCONFIG._serialized_end=1427
+  _WEBSERVERCONFIG._serialized_start=1430
+  _WEBSERVERCONFIG._serialized_end=1643
+  _WEBSERVERREWRITERULE._serialized_start=1645
+  _WEBSERVERREWRITERULE._serialized_end=1699
+  _WEBSERVERREDIRECT._serialized_start=1701
+  _WEBSERVERREDIRECT._serialized_end=1768
+  _INSTANTMAP._serialized_start=1771
+  _INSTANTMAP._serialized_end=1921
+  _INSTANCECONFIG._serialized_start=1923
+  _INSTANCECONFIG._serialized_end=1983
+  _SERVICEMAP._serialized_start=1986
+  _SERVICEMAP._serialized_end=2133
+  _SERVICECONFIG._serialized_start=2135
+  _SERVICECONFIG._serialized_end=2164
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/config/result.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/result.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,9 +21,7 @@
     jobId: metadata.TagHeader = None
 
     statusCode: metadata.JobStatusCode = metadata.JobStatusCode.JOB_STATUS_CODE_NOT_SET
 
     statusMessage: str = None
 
     results: _tp.Dict[str, metadata.ObjectDefinition] = _dc.field(default_factory=dict)
-
-    attrs: _tp.Dict[str, TagUpdateList] = _dc.field(default_factory=dict)
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/config/result_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/result_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,28 +13,24 @@
 
 from tracdap.metadata import object_id_pb2 as tracdap_dot_metadata_dot_object__id__pb2
 from tracdap.metadata import object_pb2 as tracdap_dot_metadata_dot_object__pb2
 from tracdap.metadata import job_pb2 as tracdap_dot_metadata_dot_job__pb2
 from tracdap.metadata import tag_update_pb2 as tracdap_dot_metadata_dot_tag__update__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1btracdap/config/result.proto\x12\x0etracdap.config\x1a tracdap/metadata/object_id.proto\x1a\x1dtracdap/metadata/object.proto\x1a\x1atracdap/metadata/job.proto\x1a!tracdap/metadata/tag_update.proto\";\n\rTagUpdateList\x12*\n\x05\x61ttrs\x18\x01 \x03(\x0b\x32\x1b.tracdap.metadata.TagUpdate\"\x92\x03\n\tJobResult\x12*\n\x05jobId\x18\x01 \x01(\x0b\x32\x1b.tracdap.metadata.TagHeader\x12\x33\n\nstatusCode\x18\x02 \x01(\x0e\x32\x1f.tracdap.metadata.JobStatusCode\x12\x15\n\rstatusMessage\x18\x03 \x01(\t\x12\x37\n\x07results\x18\x04 \x03(\x0b\x32&.tracdap.config.JobResult.ResultsEntry\x12\x33\n\x05\x61ttrs\x18\x05 \x03(\x0b\x32$.tracdap.config.JobResult.AttrsEntry\x1aR\n\x0cResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".tracdap.metadata.ObjectDefinition:\x02\x38\x01\x1aK\n\nAttrsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x1d.tracdap.config.TagUpdateList:\x02\x38\x01\x42\x1c\n\x18org.finos.tracdap.configP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1btracdap/config/result.proto\x12\x0etracdap.config\x1a tracdap/metadata/object_id.proto\x1a\x1dtracdap/metadata/object.proto\x1a\x1atracdap/metadata/job.proto\x1a!tracdap/metadata/tag_update.proto\";\n\rTagUpdateList\x12*\n\x05\x61ttrs\x18\x01 \x03(\x0b\x32\x1b.tracdap.metadata.TagUpdate\"\x9d\x02\n\tJobResult\x12*\n\x05jobId\x18\x01 \x01(\x0b\x32\x1b.tracdap.metadata.TagHeader\x12\x33\n\nstatusCode\x18\x02 \x01(\x0e\x32\x1f.tracdap.metadata.JobStatusCode\x12\x15\n\rstatusMessage\x18\x03 \x01(\t\x12\x37\n\x07results\x18\x04 \x03(\x0b\x32&.tracdap.config.JobResult.ResultsEntry\x1aR\n\x0cResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".tracdap.metadata.ObjectDefinition:\x02\x38\x01J\x04\x08\x05\x10\x06R\x05\x61ttrsB\x1c\n\x18org.finos.tracdap.configP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tracdap.config.result_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\030org.finos.tracdap.configP\001'
   _JOBRESULT_RESULTSENTRY._options = None
   _JOBRESULT_RESULTSENTRY._serialized_options = b'8\001'
-  _JOBRESULT_ATTRSENTRY._options = None
-  _JOBRESULT_ATTRSENTRY._serialized_options = b'8\001'
   _TAGUPDATELIST._serialized_start=175
   _TAGUPDATELIST._serialized_end=234
   _JOBRESULT._serialized_start=237
-  _JOBRESULT._serialized_end=639
-  _JOBRESULT_RESULTSENTRY._serialized_start=480
-  _JOBRESULT_RESULTSENTRY._serialized_end=562
-  _JOBRESULT_ATTRSENTRY._serialized_start=564
-  _JOBRESULT_ATTRSENTRY._serialized_end=639
+  _JOBRESULT._serialized_end=522
+  _JOBRESULT_RESULTSENTRY._serialized_start=427
+  _JOBRESULT_RESULTSENTRY._serialized_end=509
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/config/runtime.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/runtime.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/config/runtime_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/config/runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/exceptions.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,23 @@
     """
     Storage referenced in metadata is either not supported or not configured
     """
 
     pass
 
 
+class EStorageValidation(EStorage):
+
+    """
+    Storage request is invalid or not allowed (e.g. illegal chars in storage path or path escapes storage root)
+    """
+
+    pass
+
+
 class EStorageCommunication(EStorage):
 
     """
     Communication with the storage layer fails for a technical reason
 
     These errors will manifest as time-outs, partial or garbled responses.
     """
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/ext/__init__.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/ext/embed.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/ext/embed.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,54 +9,60 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import tracdap.rt.config as _cfg
+import tracdap.rt.ext._guard as _guard
+
+# Dependency back into the main runtime implementation
 import tracdap.rt._exec.runtime as _rt  # noqa
-import tracdap.rt._impl.validation as _val  # noqa
 
 
 class __EmbeddedRuntime:
 
     def __init__(self, runtime: _rt.TracRuntime):
+        _guard.run_model_guard("Using __EmbeddedRuntime")
         self.__runtime = runtime
         self.__destroyed = False
 
     def __enter__(self):
+        _guard.run_model_guard("Using __EmbeddedRuntime")
         self.__runtime.__enter__()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+        _guard.run_model_guard("Using __EmbeddedRuntime")
         self.__runtime.__exit__(exc_type, exc_val, exc_tb)
         self.__destroyed = True
 
     def __del__(self):
+        _guard.run_model_guard("Using __EmbeddedRuntime")
         if not self.__destroyed:
             self.__runtime.stop()
             self.__destroyed = True
 
     def run_job_(self, job_config: _cfg.JobConfig):
 
-        _val.validate_signature(self.run_job_, job_config)
+        _guard.run_model_guard("Using __EmbeddedRuntime")
 
         self.__runtime.submit_job(job_config)
 
         return self.__runtime.wait_for_job(job_config.jobId)
 
 
-def create_runtime(sys_config: _cfg.RuntimeConfig, dev_mode: bool = False):
+def create_runtime(sys_config: _cfg.RuntimeConfig, dev_mode: bool = False) -> __EmbeddedRuntime:
 
-    _val.validate_signature(create_runtime, sys_config, dev_mode)
+    _guard.run_model_guard()
 
     runtime = _rt.TracRuntime(sys_config, dev_mode=dev_mode)
     runtime.pre_start()
 
     return __EmbeddedRuntime(runtime)
 
 
 def run_job(runtime: __EmbeddedRuntime, job_config: _cfg.JobConfig) -> _cfg.JobResult:
 
-    _val.validate_signature(run_job, runtime, job_config)
+    _guard.run_model_guard()
 
     return runtime.run_job_(job_config)
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/ext/repos.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/ext/repos.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,73 +8,67 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-import abc
-import pathlib
-import typing as tp
+import abc as _abc
+import pathlib as _pathlib
 
 import tracdap.rt.metadata as _meta
 
 
 class IModelRepository:
 
-    @abc.abstractmethod
-    def checkout_key(self, model_def: _meta.ModelDefinition) -> str:
+    @_abc.abstractmethod
+    def do_checkout(
+            self, model_def: _meta.ModelDefinition,
+            checkout_dir: _pathlib.Path) \
+            -> _pathlib.Path:
 
         """
-        A unique key identifying the checkout required for the given model definition.
+        Perform a checkout for the given model definition, into the supplied checkout dir.
 
-        For example, in Git repositories the checkout key might be a commit hash or tag.
-        For binary packages in Nexus, the checkout key might involve both package and version.
-        Other repositories might need to use the path as well.
+        The checkout dir will be empty before this method is called.
 
-        This key is used to avoid duplicate checkouts. So for example, if several models exist in
-        the same version of a package, returning the same key will mean the checkout is only performed once.
+        The return value is the path given to the module loader, to load the model.
+        I.e. it should contain the root packages / modules that the model will load.
 
-        :param model_def: Model to request a checkout key for
-        :return: Checkout key for the given model
+        Repo implementations are free to put packages directly into checkout_dir,
+        in which case the return value should be checkout_dir. It may be helpful to
+        create a folder structure inside checkout_dir, e.g. to separate temporary files,
+        in which case the return value will be a subfolder of checkout_dir containing
+        just the model packages to be loaded. Source repositories are likely to have a
+        folder structure in the model repo itself, for example in a source repository where
+        the root source folder is "src", the return value might be <checkout_dir>/src.
+
+        :param model_def: The model to check out
+        :param checkout_dir: Empty directory into which the checkout will be performed
+        :return: Path for the root packages / modules that the model will load
         """
 
         pass
 
-    @abc.abstractmethod
+    @_abc.abstractmethod
     def package_path(
             self, model_def: _meta.ModelDefinition,
-            checkout_dir: pathlib.Path) \
-            -> tp.Optional[pathlib.Path]:
-
-        """
-        Get the root directory for package loading, assuming the model is checked out in the supplied directory.
-        The package directory will contain the Python package for the model described by the model definition,
-        it can be used as a package root (Python source root) by the TRAC model loading mechanism.
+            checkout_dir: _pathlib.Path) \
+            -> _pathlib.Path:
 
-        For example, in Git repositories this will be the path from the model definition, relative to the checkout dir.
-
-        :param model_def: Model for which the package path is requested
-        :param checkout_dir: Directory where the model is checked out (checkout must have happened previously)
-        :return: A package root directory, containing the Python package of the requested model
         """
+        Get the package path that would be returned by :py:meth:`do_checkout()`,
+        for the given checkout_dir and model_dir, without doing a checkout.
 
-        pass
-
-    @abc.abstractmethod
-    def do_checkout(
-            self, model_def: _meta.ModelDefinition,
-            checkout_dir: pathlib.Path) \
-            -> tp.Optional[pathlib.Path]:
-
-        """
-        Perform a checkout for the given model definition, into the supplied checkout dir.
+        This is used by the loader mechanism to avoid repeating the same checkout multiple times.
+        E.g. if there are multiple models or resources being loaded from the same package,
+        or if a model is referenced multiple times.
 
-        The checkout dir must be empty before this method is called.
-        The return value is the package path for the model, as per :py:meth:`package_path()`.
+        This method is always required and may be called before :py:meth:`do_checkout()`.
+        The return value should be deterministic for a given model_def and checkout_dir.
 
-        :param model_def: The model to check out
-        :param checkout_dir: Empty directory into which the checkout will be performed
-        :return: The package path for the model, as per :py:meth:`package_path()`.
+        :param model_def: Model for which the package path is requested
+        :param checkout_dir: Directory where the model is (or will be) checked out
+        :return: Path for the root packages / modules that the model will load
         """
 
         pass
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/launch/__init__.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/launch/__init__.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/launch/__main__.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/launch/__main__.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/launch/cli.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/launch/cli.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/launch/launch.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/launch/launch.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/__init__.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Code generated by TRAC
 
+from .custom import CustomDefinition
+
 from .common import MetadataFormat
 from .common import MetadataVersion
 from .common import TenantInfo
 
 from .type import BasicType
 from .type import TypeDescriptor
 from .type import DecimalValue
@@ -33,37 +35,35 @@
 from .search import SearchOperator
 from .search import LogicalOperator
 from .search import SearchTerm
 from .search import LogicalExpression
 from .search import SearchExpression
 from .search import SearchParameters
 
+from .tag_update import TagOperation
+from .tag_update import TagUpdate
+
 from .flow import FlowNodeType
 from .flow import FlowNode
 from .flow import FlowSocket
 from .flow import FlowEdge
 from .flow import FlowDefinition
 
-from .tag_update import TagOperation
-from .tag_update import TagUpdate
-
-from .custom import CustomDefinition
-
 from .job import JobType
 from .job import JobStatusCode
 from .job import JobDefinition
 from .job import RunModelJob
 from .job import RunFlowJob
 from .job import ImportModelJob
 
+from .file import FileDefinition
+
 from .stoarge import CopyStatus
 from .stoarge import IncarnationStatus
 from .stoarge import StorageCopy
 from .stoarge import StorageIncarnation
 from .stoarge import StorageItem
 from .stoarge import StorageDefinition
 
-from .file import FileDefinition
-
 from .object import ObjectDefinition
 
 from .tag import Tag
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/common.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/common.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/common_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/common_pb2.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/custom_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/custom_pb2.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/data.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,18 @@
 
     label: str = None
 
     businessKey: bool = None
 
     categorical: bool = None
 
+    notNull: _tp.Optional[bool] = None
+
+    """This could become mandatory with the next metadata update"""
+
     formatCode: _tp.Optional[str] = None
 
 
 @_dc.dataclass
 class TableSchema:
 
     fields: _tp.List[FieldSchema] = _dc.field(default_factory=list)
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/data_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/data_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 _sym_db = _symbol_database.Default()
 
 
 from tracdap.metadata import type_pb2 as tracdap_dot_metadata_dot_type__pb2
 from tracdap.metadata import object_id_pb2 as tracdap_dot_metadata_dot_object__id__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1btracdap/metadata/data.proto\x12\x10tracdap.metadata\x1a\x1btracdap/metadata/type.proto\x1a tracdap/metadata/object_id.proto\"\xc5\x01\n\x0b\x46ieldSchema\x12\x11\n\tfieldName\x18\x01 \x01(\t\x12\x12\n\nfieldOrder\x18\x02 \x01(\x11\x12.\n\tfieldType\x18\x03 \x01(\x0e\x32\x1b.tracdap.metadata.BasicType\x12\r\n\x05label\x18\x04 \x01(\t\x12\x13\n\x0b\x62usinessKey\x18\x05 \x01(\x08\x12\x13\n\x0b\x63\x61tegorical\x18\x06 \x01(\x08\x12\x17\n\nformatCode\x18\x07 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_formatCode\"<\n\x0bTableSchema\x12-\n\x06\x66ields\x18\x01 \x03(\x0b\x32\x1d.tracdap.metadata.FieldSchema\"\xba\x01\n\x10SchemaDefinition\x12\x30\n\nschemaType\x18\x01 \x01(\x0e\x32\x1c.tracdap.metadata.SchemaType\x12,\n\x08partType\x18\x02 \x01(\x0e\x32\x1a.tracdap.metadata.PartType\x12.\n\x05table\x18\x03 \x01(\x0b\x32\x1d.tracdap.metadata.TableSchemaH\x00\x42\x16\n\x14schemaTypeDefinition\"\x81\x02\n\x07PartKey\x12\x11\n\topaqueKey\x18\x01 \x01(\t\x12,\n\x08partType\x18\x02 \x01(\x0e\x32\x1a.tracdap.metadata.PartType\x12+\n\npartValues\x18\x03 \x03(\x0b\x32\x17.tracdap.metadata.Value\x12\x32\n\x0cpartRangeMin\x18\x04 \x01(\x0b\x32\x17.tracdap.metadata.ValueH\x00\x88\x01\x01\x12\x32\n\x0cpartRangeMax\x18\x05 \x01(\x0b\x32\x17.tracdap.metadata.ValueH\x01\x88\x01\x01\x42\x0f\n\r_partRangeMinB\x0f\n\r_partRangeMax\"\xba\x04\n\x0e\x44\x61taDefinition\x12\x31\n\x08schemaId\x18\x01 \x01(\x0b\x32\x1d.tracdap.metadata.TagSelectorH\x00\x12\x34\n\x06schema\x18\x02 \x01(\x0b\x32\".tracdap.metadata.SchemaDefinitionH\x00\x12:\n\x05parts\x18\x03 \x03(\x0b\x32+.tracdap.metadata.DataDefinition.PartsEntry\x12\x30\n\tstorageId\x18\x04 \x01(\x0b\x32\x1d.tracdap.metadata.TagSelector\x1a-\n\x05\x44\x65lta\x12\x12\n\ndeltaIndex\x18\x01 \x01(\r\x12\x10\n\x08\x64\x61taItem\x18\x02 \x01(\t\x1aQ\n\x04Snap\x12\x11\n\tsnapIndex\x18\x01 \x01(\r\x12\x36\n\x06\x64\x65ltas\x18\x02 \x03(\x0b\x32&.tracdap.metadata.DataDefinition.Delta\x1ag\n\x04Part\x12*\n\x07partKey\x18\x01 \x01(\x0b\x32\x19.tracdap.metadata.PartKey\x12\x33\n\x04snap\x18\x02 \x01(\x0b\x32%.tracdap.metadata.DataDefinition.Snap\x1aS\n\nPartsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.tracdap.metadata.DataDefinition.Part:\x02\x38\x01\x42\x11\n\x0fschemaSpecifier*0\n\nSchemaType\x12\x17\n\x13SCHEMA_TYPE_NOT_SET\x10\x00\x12\t\n\x05TABLE\x10\x01*?\n\x08PartType\x12\r\n\tPART_ROOT\x10\x00\x12\x11\n\rPART_BY_RANGE\x10\x01\x12\x11\n\rPART_BY_VALUE\x10\x02\x42\x1e\n\x1aorg.finos.tracdap.metadataP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1btracdap/metadata/data.proto\x12\x10tracdap.metadata\x1a\x1btracdap/metadata/type.proto\x1a tracdap/metadata/object_id.proto\"\xe7\x01\n\x0b\x46ieldSchema\x12\x11\n\tfieldName\x18\x01 \x01(\t\x12\x12\n\nfieldOrder\x18\x02 \x01(\x11\x12.\n\tfieldType\x18\x03 \x01(\x0e\x32\x1b.tracdap.metadata.BasicType\x12\r\n\x05label\x18\x04 \x01(\t\x12\x13\n\x0b\x62usinessKey\x18\x05 \x01(\x08\x12\x13\n\x0b\x63\x61tegorical\x18\x06 \x01(\x08\x12\x14\n\x07notNull\x18\x08 \x01(\x08H\x00\x88\x01\x01\x12\x17\n\nformatCode\x18\x07 \x01(\tH\x01\x88\x01\x01\x42\n\n\x08_notNullB\r\n\x0b_formatCode\"<\n\x0bTableSchema\x12-\n\x06\x66ields\x18\x01 \x03(\x0b\x32\x1d.tracdap.metadata.FieldSchema\"\xba\x01\n\x10SchemaDefinition\x12\x30\n\nschemaType\x18\x01 \x01(\x0e\x32\x1c.tracdap.metadata.SchemaType\x12,\n\x08partType\x18\x02 \x01(\x0e\x32\x1a.tracdap.metadata.PartType\x12.\n\x05table\x18\x03 \x01(\x0b\x32\x1d.tracdap.metadata.TableSchemaH\x00\x42\x16\n\x14schemaTypeDefinition\"\x81\x02\n\x07PartKey\x12\x11\n\topaqueKey\x18\x01 \x01(\t\x12,\n\x08partType\x18\x02 \x01(\x0e\x32\x1a.tracdap.metadata.PartType\x12+\n\npartValues\x18\x03 \x03(\x0b\x32\x17.tracdap.metadata.Value\x12\x32\n\x0cpartRangeMin\x18\x04 \x01(\x0b\x32\x17.tracdap.metadata.ValueH\x00\x88\x01\x01\x12\x32\n\x0cpartRangeMax\x18\x05 \x01(\x0b\x32\x17.tracdap.metadata.ValueH\x01\x88\x01\x01\x42\x0f\n\r_partRangeMinB\x0f\n\r_partRangeMax\"\xba\x04\n\x0e\x44\x61taDefinition\x12\x31\n\x08schemaId\x18\x01 \x01(\x0b\x32\x1d.tracdap.metadata.TagSelectorH\x00\x12\x34\n\x06schema\x18\x02 \x01(\x0b\x32\".tracdap.metadata.SchemaDefinitionH\x00\x12:\n\x05parts\x18\x03 \x03(\x0b\x32+.tracdap.metadata.DataDefinition.PartsEntry\x12\x30\n\tstorageId\x18\x04 \x01(\x0b\x32\x1d.tracdap.metadata.TagSelector\x1a-\n\x05\x44\x65lta\x12\x12\n\ndeltaIndex\x18\x01 \x01(\r\x12\x10\n\x08\x64\x61taItem\x18\x02 \x01(\t\x1aQ\n\x04Snap\x12\x11\n\tsnapIndex\x18\x01 \x01(\r\x12\x36\n\x06\x64\x65ltas\x18\x02 \x03(\x0b\x32&.tracdap.metadata.DataDefinition.Delta\x1ag\n\x04Part\x12*\n\x07partKey\x18\x01 \x01(\x0b\x32\x19.tracdap.metadata.PartKey\x12\x33\n\x04snap\x18\x02 \x01(\x0b\x32%.tracdap.metadata.DataDefinition.Snap\x1aS\n\nPartsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.tracdap.metadata.DataDefinition.Part:\x02\x38\x01\x42\x11\n\x0fschemaSpecifier*0\n\nSchemaType\x12\x17\n\x13SCHEMA_TYPE_NOT_SET\x10\x00\x12\t\n\x05TABLE\x10\x01*?\n\x08PartType\x12\r\n\tPART_ROOT\x10\x00\x12\x11\n\rPART_BY_RANGE\x10\x01\x12\x11\n\rPART_BY_VALUE\x10\x02\x42\x1e\n\x1aorg.finos.tracdap.metadataP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tracdap.metadata.data_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\032org.finos.tracdap.metadataP\001'
   _DATADEFINITION_PARTSENTRY._options = None
   _DATADEFINITION_PARTSENTRY._serialized_options = b'8\001'
-  _SCHEMATYPE._serialized_start=1396
-  _SCHEMATYPE._serialized_end=1444
-  _PARTTYPE._serialized_start=1446
-  _PARTTYPE._serialized_end=1509
+  _SCHEMATYPE._serialized_start=1430
+  _SCHEMATYPE._serialized_end=1478
+  _PARTTYPE._serialized_start=1480
+  _PARTTYPE._serialized_end=1543
   _FIELDSCHEMA._serialized_start=113
-  _FIELDSCHEMA._serialized_end=310
-  _TABLESCHEMA._serialized_start=312
-  _TABLESCHEMA._serialized_end=372
-  _SCHEMADEFINITION._serialized_start=375
-  _SCHEMADEFINITION._serialized_end=561
-  _PARTKEY._serialized_start=564
-  _PARTKEY._serialized_end=821
-  _DATADEFINITION._serialized_start=824
-  _DATADEFINITION._serialized_end=1394
-  _DATADEFINITION_DELTA._serialized_start=1057
-  _DATADEFINITION_DELTA._serialized_end=1102
-  _DATADEFINITION_SNAP._serialized_start=1104
-  _DATADEFINITION_SNAP._serialized_end=1185
-  _DATADEFINITION_PART._serialized_start=1187
-  _DATADEFINITION_PART._serialized_end=1290
-  _DATADEFINITION_PARTSENTRY._serialized_start=1292
-  _DATADEFINITION_PARTSENTRY._serialized_end=1375
+  _FIELDSCHEMA._serialized_end=344
+  _TABLESCHEMA._serialized_start=346
+  _TABLESCHEMA._serialized_end=406
+  _SCHEMADEFINITION._serialized_start=409
+  _SCHEMADEFINITION._serialized_end=595
+  _PARTKEY._serialized_start=598
+  _PARTKEY._serialized_end=855
+  _DATADEFINITION._serialized_start=858
+  _DATADEFINITION._serialized_end=1428
+  _DATADEFINITION_DELTA._serialized_start=1091
+  _DATADEFINITION_DELTA._serialized_end=1136
+  _DATADEFINITION_SNAP._serialized_start=1138
+  _DATADEFINITION_SNAP._serialized_end=1219
+  _DATADEFINITION_PART._serialized_start=1221
+  _DATADEFINITION_PART._serialized_end=1324
+  _DATADEFINITION_PARTSENTRY._serialized_start=1326
+  _DATADEFINITION_PARTSENTRY._serialized_end=1409
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/file_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/file_pb2.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/flow.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/flow.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import typing as _tp  # noqa
 import dataclasses as _dc  # noqa
 import enum as _enum  # noqa
 
 from .type import *  # noqa
 from .model import *  # noqa
 from .search import *  # noqa
+from .tag_update import *  # noqa
 
 
 class FlowNodeType(_enum.Enum):
 
     NODE_TYPE_NOT_SET = 0, 
 
     INPUT_NODE = 1, 
@@ -28,14 +29,18 @@
 
     inputs: _tp.List[str] = _dc.field(default_factory=list)
 
     outputs: _tp.List[str] = _dc.field(default_factory=list)
 
     nodeSearch: SearchExpression = None
 
+    nodeAttrs: _tp.List[TagUpdate] = _dc.field(default_factory=list)
+
+    label: str = None
+
 
 @_dc.dataclass
 class FlowSocket:
 
     node: str = None
 
     socket: str = None
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/flow_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/flow_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from tracdap.metadata import type_pb2 as tracdap_dot_metadata_dot_type__pb2
 from tracdap.metadata import model_pb2 as tracdap_dot_metadata_dot_model__pb2
 from tracdap.metadata import search_pb2 as tracdap_dot_metadata_dot_search__pb2
+from tracdap.metadata import tag_update_pb2 as tracdap_dot_metadata_dot_tag__update__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1btracdap/metadata/flow.proto\x12\x10tracdap.metadata\x1a\x1btracdap/metadata/type.proto\x1a\x1ctracdap/metadata/model.proto\x1a\x1dtracdap/metadata/search.proto\"\xa2\x01\n\x08\x46lowNode\x12\x30\n\x08nodeType\x18\x01 \x01(\x0e\x32\x1e.tracdap.metadata.FlowNodeType\x12\x0e\n\x06inputs\x18\x02 \x03(\t\x12\x0f\n\x07outputs\x18\x03 \x03(\t\x12\x36\n\nnodeSearch\x18\x04 \x01(\x0b\x32\".tracdap.metadata.SearchExpressionR\x0bparameters;\"*\n\nFlowSocket\x12\x0c\n\x04node\x18\x01 \x01(\t\x12\x0e\n\x06socket\x18\x02 \x01(\t\"f\n\x08\x46lowEdge\x12,\n\x06source\x18\x01 \x01(\x0b\x32\x1c.tracdap.metadata.FlowSocket\x12,\n\x06target\x18\x02 \x01(\x0b\x32\x1c.tracdap.metadata.FlowSocket\"\x82\x05\n\x0e\x46lowDefinition\x12:\n\x05nodes\x18\x01 \x03(\x0b\x32+.tracdap.metadata.FlowDefinition.NodesEntry\x12)\n\x05\x65\x64ges\x18\x02 \x03(\x0b\x32\x1a.tracdap.metadata.FlowEdge\x12\x44\n\nparameters\x18\x03 \x03(\x0b\x32\x30.tracdap.metadata.FlowDefinition.ParametersEntry\x12<\n\x06inputs\x18\x04 \x03(\x0b\x32,.tracdap.metadata.FlowDefinition.InputsEntry\x12>\n\x07outputs\x18\x05 \x03(\x0b\x32-.tracdap.metadata.FlowDefinition.OutputsEntry\x1aH\n\nNodesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.tracdap.metadata.FlowNode:\x02\x38\x01\x1aS\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .tracdap.metadata.ModelParameter:\x02\x38\x01\x1aQ\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".tracdap.metadata.ModelInputSchema:\x02\x38\x01\x1aS\n\x0cOutputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.tracdap.metadata.ModelOutputSchema:\x02\x38\x01*V\n\x0c\x46lowNodeType\x12\x15\n\x11NODE_TYPE_NOT_SET\x10\x00\x12\x0e\n\nINPUT_NODE\x10\x01\x12\x0f\n\x0bOUTPUT_NODE\x10\x02\x12\x0e\n\nMODEL_NODE\x10\x03\x42\x1e\n\x1aorg.finos.tracdap.metadataP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1btracdap/metadata/flow.proto\x12\x10tracdap.metadata\x1a\x1btracdap/metadata/type.proto\x1a\x1ctracdap/metadata/model.proto\x1a\x1dtracdap/metadata/search.proto\x1a!tracdap/metadata/tag_update.proto\"\xe1\x01\n\x08\x46lowNode\x12\x30\n\x08nodeType\x18\x01 \x01(\x0e\x32\x1e.tracdap.metadata.FlowNodeType\x12\x0e\n\x06inputs\x18\x02 \x03(\t\x12\x0f\n\x07outputs\x18\x03 \x03(\t\x12\x36\n\nnodeSearch\x18\x04 \x01(\x0b\x32\".tracdap.metadata.SearchExpression\x12.\n\tnodeAttrs\x18\x05 \x03(\x0b\x32\x1b.tracdap.metadata.TagUpdate\x12\r\n\x05label\x18\x06 \x01(\tR\x0bparameters;\"*\n\nFlowSocket\x12\x0c\n\x04node\x18\x01 \x01(\t\x12\x0e\n\x06socket\x18\x02 \x01(\t\"f\n\x08\x46lowEdge\x12,\n\x06source\x18\x01 \x01(\x0b\x32\x1c.tracdap.metadata.FlowSocket\x12,\n\x06target\x18\x02 \x01(\x0b\x32\x1c.tracdap.metadata.FlowSocket\"\x82\x05\n\x0e\x46lowDefinition\x12:\n\x05nodes\x18\x01 \x03(\x0b\x32+.tracdap.metadata.FlowDefinition.NodesEntry\x12)\n\x05\x65\x64ges\x18\x02 \x03(\x0b\x32\x1a.tracdap.metadata.FlowEdge\x12\x44\n\nparameters\x18\x03 \x03(\x0b\x32\x30.tracdap.metadata.FlowDefinition.ParametersEntry\x12<\n\x06inputs\x18\x04 \x03(\x0b\x32,.tracdap.metadata.FlowDefinition.InputsEntry\x12>\n\x07outputs\x18\x05 \x03(\x0b\x32-.tracdap.metadata.FlowDefinition.OutputsEntry\x1aH\n\nNodesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.tracdap.metadata.FlowNode:\x02\x38\x01\x1aS\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .tracdap.metadata.ModelParameter:\x02\x38\x01\x1aQ\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".tracdap.metadata.ModelInputSchema:\x02\x38\x01\x1aS\n\x0cOutputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.tracdap.metadata.ModelOutputSchema:\x02\x38\x01*V\n\x0c\x46lowNodeType\x12\x15\n\x11NODE_TYPE_NOT_SET\x10\x00\x12\x0e\n\nINPUT_NODE\x10\x01\x12\x0f\n\x0bOUTPUT_NODE\x10\x02\x12\x0e\n\nMODEL_NODE\x10\x03\x42\x1e\n\x1aorg.finos.tracdap.metadataP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tracdap.metadata.flow_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\032org.finos.tracdap.metadataP\001'
@@ -28,26 +29,26 @@
   _FLOWDEFINITION_NODESENTRY._serialized_options = b'8\001'
   _FLOWDEFINITION_PARAMETERSENTRY._options = None
   _FLOWDEFINITION_PARAMETERSENTRY._serialized_options = b'8\001'
   _FLOWDEFINITION_INPUTSENTRY._options = None
   _FLOWDEFINITION_INPUTSENTRY._serialized_options = b'8\001'
   _FLOWDEFINITION_OUTPUTSENTRY._options = None
   _FLOWDEFINITION_OUTPUTSENTRY._serialized_options = b'8\001'
-  _FLOWNODETYPE._serialized_start=1097
-  _FLOWNODETYPE._serialized_end=1183
-  _FLOWNODE._serialized_start=140
-  _FLOWNODE._serialized_end=302
-  _FLOWSOCKET._serialized_start=304
-  _FLOWSOCKET._serialized_end=346
-  _FLOWEDGE._serialized_start=348
-  _FLOWEDGE._serialized_end=450
-  _FLOWDEFINITION._serialized_start=453
-  _FLOWDEFINITION._serialized_end=1095
-  _FLOWDEFINITION_NODESENTRY._serialized_start=770
-  _FLOWDEFINITION_NODESENTRY._serialized_end=842
-  _FLOWDEFINITION_PARAMETERSENTRY._serialized_start=844
-  _FLOWDEFINITION_PARAMETERSENTRY._serialized_end=927
-  _FLOWDEFINITION_INPUTSENTRY._serialized_start=929
-  _FLOWDEFINITION_INPUTSENTRY._serialized_end=1010
-  _FLOWDEFINITION_OUTPUTSENTRY._serialized_start=1012
-  _FLOWDEFINITION_OUTPUTSENTRY._serialized_end=1095
+  _FLOWNODETYPE._serialized_start=1195
+  _FLOWNODETYPE._serialized_end=1281
+  _FLOWNODE._serialized_start=175
+  _FLOWNODE._serialized_end=400
+  _FLOWSOCKET._serialized_start=402
+  _FLOWSOCKET._serialized_end=444
+  _FLOWEDGE._serialized_start=446
+  _FLOWEDGE._serialized_end=548
+  _FLOWDEFINITION._serialized_start=551
+  _FLOWDEFINITION._serialized_end=1193
+  _FLOWDEFINITION_NODESENTRY._serialized_start=868
+  _FLOWDEFINITION_NODESENTRY._serialized_end=940
+  _FLOWDEFINITION_PARAMETERSENTRY._serialized_start=942
+  _FLOWDEFINITION_PARAMETERSENTRY._serialized_end=1025
+  _FLOWDEFINITION_INPUTSENTRY._serialized_start=1027
+  _FLOWDEFINITION_INPUTSENTRY._serialized_end=1108
+  _FLOWDEFINITION_OUTPUTSENTRY._serialized_start=1110
+  _FLOWDEFINITION_OUTPUTSENTRY._serialized_end=1193
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/job.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/job.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/job_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/job_pb2.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/model.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     schema is provided at runtime and can be interrogated by the model code. Models may also
     define inputs with some required fields and a dynamic portion. For non-tabular inputs,
     other options may be required. These capabilities may be added in future releases.
     """
 
     schema: SchemaDefinition = None
 
+    label: _tp.Optional[str] = None
+
 
 @_dc.dataclass
 class ModelOutputSchema:
 
     """
     Describes the data schema of a model output
     
@@ -54,14 +56,16 @@
     same schema as dynamic input Y) and pass-through-extend schemas (output X has the schema of
     dynamic input Y, plus one or more new columns) can also be useful. These capabilities may be
     added in future releases.
     """
 
     schema: SchemaDefinition = None
 
+    label: _tp.Optional[str] = None
+
 
 @_dc.dataclass
 class ModelDefinition:
 
     """Define a model for execution on the TRAC platform"""
 
     language: str = None
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/model_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/model_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from tracdap.metadata import type_pb2 as tracdap_dot_metadata_dot_type__pb2
 from tracdap.metadata import data_pb2 as tracdap_dot_metadata_dot_data__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ctracdap/metadata/model.proto\x12\x10tracdap.metadata\x1a\x1btracdap/metadata/type.proto\x1a\x1btracdap/metadata/data.proto\"\x99\x01\n\x0eModelParameter\x12\x33\n\tparamType\x18\x01 \x01(\x0b\x32 .tracdap.metadata.TypeDescriptor\x12\r\n\x05label\x18\x02 \x01(\t\x12\x32\n\x0c\x64\x65\x66\x61ultValue\x18\x03 \x01(\x0b\x32\x17.tracdap.metadata.ValueH\x00\x88\x01\x01\x42\x0f\n\r_defaultValue\"F\n\x10ModelInputSchema\x12\x32\n\x06schema\x18\x01 \x01(\x0b\x32\".tracdap.metadata.SchemaDefinition\"G\n\x11ModelOutputSchema\x12\x32\n\x06schema\x18\x01 \x01(\x0b\x32\".tracdap.metadata.SchemaDefinition\"\x9e\x06\n\x0fModelDefinition\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x12\n\nrepository\x18\x02 \x01(\t\x12\x19\n\x0cpackageGroup\x18\n \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x07package\x18\x0b \x01(\t\x12\x0f\n\x07version\x18\x06 \x01(\t\x12\x12\n\nentryPoint\x18\x05 \x01(\t\x12\x11\n\x04path\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x45\n\nparameters\x18\x07 \x03(\x0b\x32\x31.tracdap.metadata.ModelDefinition.ParametersEntry\x12=\n\x06inputs\x18\x08 \x03(\x0b\x32-.tracdap.metadata.ModelDefinition.InputsEntry\x12?\n\x07outputs\x18\t \x03(\x0b\x32..tracdap.metadata.ModelDefinition.OutputsEntry\x12Q\n\x10staticAttributes\x18\x0c \x03(\x0b\x32\x37.tracdap.metadata.ModelDefinition.StaticAttributesEntry\x1aS\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .tracdap.metadata.ModelParameter:\x02\x38\x01\x1aQ\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".tracdap.metadata.ModelInputSchema:\x02\x38\x01\x1aS\n\x0cOutputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.tracdap.metadata.ModelOutputSchema:\x02\x38\x01\x1aP\n\x15StaticAttributesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.tracdap.metadata.Value:\x02\x38\x01\x42\x0f\n\r_packageGroupB\x07\n\x05_pathB\x1e\n\x1aorg.finos.tracdap.metadataP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ctracdap/metadata/model.proto\x12\x10tracdap.metadata\x1a\x1btracdap/metadata/type.proto\x1a\x1btracdap/metadata/data.proto\"\x99\x01\n\x0eModelParameter\x12\x33\n\tparamType\x18\x01 \x01(\x0b\x32 .tracdap.metadata.TypeDescriptor\x12\r\n\x05label\x18\x02 \x01(\t\x12\x32\n\x0c\x64\x65\x66\x61ultValue\x18\x03 \x01(\x0b\x32\x17.tracdap.metadata.ValueH\x00\x88\x01\x01\x42\x0f\n\r_defaultValue\"d\n\x10ModelInputSchema\x12\x32\n\x06schema\x18\x01 \x01(\x0b\x32\".tracdap.metadata.SchemaDefinition\x12\x12\n\x05label\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_label\"e\n\x11ModelOutputSchema\x12\x32\n\x06schema\x18\x01 \x01(\x0b\x32\".tracdap.metadata.SchemaDefinition\x12\x12\n\x05label\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_label\"\x9e\x06\n\x0fModelDefinition\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x12\n\nrepository\x18\x02 \x01(\t\x12\x19\n\x0cpackageGroup\x18\n \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x07package\x18\x0b \x01(\t\x12\x0f\n\x07version\x18\x06 \x01(\t\x12\x12\n\nentryPoint\x18\x05 \x01(\t\x12\x11\n\x04path\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x45\n\nparameters\x18\x07 \x03(\x0b\x32\x31.tracdap.metadata.ModelDefinition.ParametersEntry\x12=\n\x06inputs\x18\x08 \x03(\x0b\x32-.tracdap.metadata.ModelDefinition.InputsEntry\x12?\n\x07outputs\x18\t \x03(\x0b\x32..tracdap.metadata.ModelDefinition.OutputsEntry\x12Q\n\x10staticAttributes\x18\x0c \x03(\x0b\x32\x37.tracdap.metadata.ModelDefinition.StaticAttributesEntry\x1aS\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .tracdap.metadata.ModelParameter:\x02\x38\x01\x1aQ\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\".tracdap.metadata.ModelInputSchema:\x02\x38\x01\x1aS\n\x0cOutputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.tracdap.metadata.ModelOutputSchema:\x02\x38\x01\x1aP\n\x15StaticAttributesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.tracdap.metadata.Value:\x02\x38\x01\x42\x0f\n\r_packageGroupB\x07\n\x05_pathB\x1e\n\x1aorg.finos.tracdap.metadataP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tracdap.metadata.model_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\032org.finos.tracdap.metadataP\001'
@@ -30,21 +30,21 @@
   _MODELDEFINITION_OUTPUTSENTRY._options = None
   _MODELDEFINITION_OUTPUTSENTRY._serialized_options = b'8\001'
   _MODELDEFINITION_STATICATTRIBUTESENTRY._options = None
   _MODELDEFINITION_STATICATTRIBUTESENTRY._serialized_options = b'8\001'
   _MODELPARAMETER._serialized_start=109
   _MODELPARAMETER._serialized_end=262
   _MODELINPUTSCHEMA._serialized_start=264
-  _MODELINPUTSCHEMA._serialized_end=334
-  _MODELOUTPUTSCHEMA._serialized_start=336
-  _MODELOUTPUTSCHEMA._serialized_end=407
-  _MODELDEFINITION._serialized_start=410
-  _MODELDEFINITION._serialized_end=1208
-  _MODELDEFINITION_PARAMETERSENTRY._serialized_start=849
-  _MODELDEFINITION_PARAMETERSENTRY._serialized_end=932
-  _MODELDEFINITION_INPUTSENTRY._serialized_start=934
-  _MODELDEFINITION_INPUTSENTRY._serialized_end=1015
-  _MODELDEFINITION_OUTPUTSENTRY._serialized_start=1017
-  _MODELDEFINITION_OUTPUTSENTRY._serialized_end=1100
-  _MODELDEFINITION_STATICATTRIBUTESENTRY._serialized_start=1102
-  _MODELDEFINITION_STATICATTRIBUTESENTRY._serialized_end=1182
+  _MODELINPUTSCHEMA._serialized_end=364
+  _MODELOUTPUTSCHEMA._serialized_start=366
+  _MODELOUTPUTSCHEMA._serialized_end=467
+  _MODELDEFINITION._serialized_start=470
+  _MODELDEFINITION._serialized_end=1268
+  _MODELDEFINITION_PARAMETERSENTRY._serialized_start=909
+  _MODELDEFINITION_PARAMETERSENTRY._serialized_end=992
+  _MODELDEFINITION_INPUTSENTRY._serialized_start=994
+  _MODELDEFINITION_INPUTSENTRY._serialized_end=1075
+  _MODELDEFINITION_OUTPUTSENTRY._serialized_start=1077
+  _MODELDEFINITION_OUTPUTSENTRY._serialized_end=1160
+  _MODELDEFINITION_STATICATTRIBUTESENTRY._serialized_start=1162
+  _MODELDEFINITION_STATICATTRIBUTESENTRY._serialized_end=1242
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/object.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/object.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/object_id.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/object_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,14 +76,22 @@
 
     """Version of this tag."""
 
     tagTimestamp: DatetimeValue = None
 
     """Timestamp for when this version of the tag was created."""
 
+    isLatestObject: bool = None
+
+    """isLatest flag for the object the tag is associated with."""
+
+    isLatestTag: bool = None
+
+    """isLatest flag for the tag."""
+
 
 @_dc.dataclass
 class TagSelector:
 
     """
     A tag selector describes the selection of a unique object at a point in time.
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/object_id_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/object_id_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from tracdap.metadata import type_pb2 as tracdap_dot_metadata_dot_type__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tracdap/metadata/object_id.proto\x12\x10tracdap.metadata\x1a\x1btracdap/metadata/type.proto\"\xeb\x01\n\tTagHeader\x12\x30\n\nobjectType\x18\x01 \x01(\x0e\x32\x1c.tracdap.metadata.ObjectType\x12\x10\n\x08objectId\x18\x02 \x01(\t\x12\x15\n\robjectVersion\x18\x03 \x01(\x05\x12\x38\n\x0fobjectTimestamp\x18\x04 \x01(\x0b\x32\x1f.tracdap.metadata.DatetimeValue\x12\x12\n\ntagVersion\x18\x05 \x01(\x05\x12\x35\n\x0ctagTimestamp\x18\x06 \x01(\x0b\x32\x1f.tracdap.metadata.DatetimeValue\"\xb9\x02\n\x0bTagSelector\x12\x30\n\nobjectType\x18\x01 \x01(\x0e\x32\x1c.tracdap.metadata.ObjectType\x12\x10\n\x08objectId\x18\x02 \x01(\t\x12\x16\n\x0clatestObject\x18\x03 \x01(\x08H\x00\x12\x17\n\robjectVersion\x18\x04 \x01(\x05H\x00\x12\x35\n\nobjectAsOf\x18\x05 \x01(\x0b\x32\x1f.tracdap.metadata.DatetimeValueH\x00\x12\x13\n\tlatestTag\x18\x06 \x01(\x08H\x01\x12\x14\n\ntagVersion\x18\x07 \x01(\x05H\x01\x12\x32\n\x07tagAsOf\x18\x08 \x01(\x0b\x32\x1f.tracdap.metadata.DatetimeValueH\x01\x42\x10\n\x0eobjectCriteriaB\r\n\x0btagCriteria*|\n\nObjectType\x12\x17\n\x13OBJECT_TYPE_NOT_SET\x10\x00\x12\x08\n\x04\x44\x41TA\x10\x01\x12\t\n\x05MODEL\x10\x02\x12\x08\n\x04\x46LOW\x10\x03\x12\x07\n\x03JOB\x10\x04\x12\x08\n\x04\x46ILE\x10\x05\x12\n\n\x06\x43USTOM\x10\x06\x12\x0b\n\x07STORAGE\x10\x07\x12\n\n\x06SCHEMA\x10\x08\x42\x1e\n\x1aorg.finos.tracdap.metadataP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n tracdap/metadata/object_id.proto\x12\x10tracdap.metadata\x1a\x1btracdap/metadata/type.proto\"\x98\x02\n\tTagHeader\x12\x30\n\nobjectType\x18\x01 \x01(\x0e\x32\x1c.tracdap.metadata.ObjectType\x12\x10\n\x08objectId\x18\x02 \x01(\t\x12\x15\n\robjectVersion\x18\x03 \x01(\x05\x12\x38\n\x0fobjectTimestamp\x18\x04 \x01(\x0b\x32\x1f.tracdap.metadata.DatetimeValue\x12\x12\n\ntagVersion\x18\x05 \x01(\x05\x12\x35\n\x0ctagTimestamp\x18\x06 \x01(\x0b\x32\x1f.tracdap.metadata.DatetimeValue\x12\x16\n\x0eisLatestObject\x18\x07 \x01(\x08\x12\x13\n\x0bisLatestTag\x18\x08 \x01(\x08\"\xb9\x02\n\x0bTagSelector\x12\x30\n\nobjectType\x18\x01 \x01(\x0e\x32\x1c.tracdap.metadata.ObjectType\x12\x10\n\x08objectId\x18\x02 \x01(\t\x12\x16\n\x0clatestObject\x18\x03 \x01(\x08H\x00\x12\x17\n\robjectVersion\x18\x04 \x01(\x05H\x00\x12\x35\n\nobjectAsOf\x18\x05 \x01(\x0b\x32\x1f.tracdap.metadata.DatetimeValueH\x00\x12\x13\n\tlatestTag\x18\x06 \x01(\x08H\x01\x12\x14\n\ntagVersion\x18\x07 \x01(\x05H\x01\x12\x32\n\x07tagAsOf\x18\x08 \x01(\x0b\x32\x1f.tracdap.metadata.DatetimeValueH\x01\x42\x10\n\x0eobjectCriteriaB\r\n\x0btagCriteria*|\n\nObjectType\x12\x17\n\x13OBJECT_TYPE_NOT_SET\x10\x00\x12\x08\n\x04\x44\x41TA\x10\x01\x12\t\n\x05MODEL\x10\x02\x12\x08\n\x04\x46LOW\x10\x03\x12\x07\n\x03JOB\x10\x04\x12\x08\n\x04\x46ILE\x10\x05\x12\n\n\x06\x43USTOM\x10\x06\x12\x0b\n\x07STORAGE\x10\x07\x12\n\n\x06SCHEMA\x10\x08\x42\x1e\n\x1aorg.finos.tracdap.metadataP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tracdap.metadata.object_id_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\032org.finos.tracdap.metadataP\001'
-  _OBJECTTYPE._serialized_start=637
-  _OBJECTTYPE._serialized_end=761
+  _OBJECTTYPE._serialized_start=682
+  _OBJECTTYPE._serialized_end=806
   _TAGHEADER._serialized_start=84
-  _TAGHEADER._serialized_end=319
-  _TAGSELECTOR._serialized_start=322
-  _TAGSELECTOR._serialized_end=635
+  _TAGHEADER._serialized_end=364
+  _TAGSELECTOR._serialized_start=367
+  _TAGSELECTOR._serialized_end=680
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/object_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/object_pb2.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/search.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,22 @@
     primitive type. Arrays of BOOLEAN values are not supported, use EQ to match boolean
     attributes.
     
     Exact matches may behave erratically for FLOAT values due to rounding errors,
     for this reason it is not recommended to use the IN operator with FLOAT values.
     """
 
+    EXISTS = 8, """EXISTS
+    
+    If an attribute type is provided the EXISTS operator matches a tag of specified
+    name when the tag has an attribute whose type is matched with type provided attribute
+    type. If no attribute type is provided, then it is enough for the tag to be of
+    specified name to be matched.
+    """
+
 
 class LogicalOperator(_enum.Enum):
 
     """
     Metadata search logical operator, used as part of a LogicalExpression.
     
     .. seealso::
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/search_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/search_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 _sym_db = _symbol_database.Default()
 
 
 from tracdap.metadata import type_pb2 as tracdap_dot_metadata_dot_type__pb2
 from tracdap.metadata import object_id_pb2 as tracdap_dot_metadata_dot_object__id__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dtracdap/metadata/search.proto\x12\x10tracdap.metadata\x1a\x1btracdap/metadata/type.proto\x1a tracdap/metadata/object_id.proto\"\xaf\x01\n\nSearchTerm\x12\x10\n\x08\x61ttrName\x18\x01 \x01(\t\x12-\n\x08\x61ttrType\x18\x02 \x01(\x0e\x32\x1b.tracdap.metadata.BasicType\x12\x32\n\x08operator\x18\x03 \x01(\x0e\x32 .tracdap.metadata.SearchOperator\x12,\n\x0bsearchValue\x18\x04 \x01(\x0b\x32\x17.tracdap.metadata.Value\"z\n\x11LogicalExpression\x12\x33\n\x08operator\x18\x01 \x01(\x0e\x32!.tracdap.metadata.LogicalOperator\x12\x30\n\x04\x65xpr\x18\x02 \x03(\x0b\x32\".tracdap.metadata.SearchExpression\"\x80\x01\n\x10SearchExpression\x12,\n\x04term\x18\x01 \x01(\x0b\x32\x1c.tracdap.metadata.SearchTermH\x00\x12\x36\n\x07logical\x18\x02 \x01(\x0b\x32#.tracdap.metadata.LogicalExpressionH\x00\x42\x06\n\x04\x65xpr\"\xeb\x01\n\x10SearchParameters\x12\x30\n\nobjectType\x18\x01 \x01(\x0e\x32\x1c.tracdap.metadata.ObjectType\x12\x32\n\x06search\x18\x02 \x01(\x0b\x32\".tracdap.metadata.SearchExpression\x12\x38\n\nsearchAsOf\x18\x03 \x01(\x0b\x32\x1f.tracdap.metadata.DatetimeValueH\x00\x88\x01\x01\x12\x15\n\rpriorVersions\x18\x04 \x01(\x08\x12\x11\n\tpriorTags\x18\x05 \x01(\x08\x42\r\n\x0b_searchAsOf*e\n\x0eSearchOperator\x12\x1b\n\x17SEARCH_OPERATOR_NOT_SET\x10\x00\x12\x06\n\x02\x45Q\x10\x01\x12\x06\n\x02NE\x10\x02\x12\x06\n\x02LT\x10\x03\x12\x06\n\x02LE\x10\x04\x12\x06\n\x02GT\x10\x05\x12\x06\n\x02GE\x10\x06\x12\x06\n\x02IN\x10\x07*I\n\x0fLogicalOperator\x12\x1c\n\x18LOGICAL_OPERATOR_NOT_SET\x10\x00\x12\x07\n\x03\x41ND\x10\x01\x12\x06\n\x02OR\x10\x02\x12\x07\n\x03NOT\x10\x03\x42\x1e\n\x1aorg.finos.tracdap.metadataP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dtracdap/metadata/search.proto\x12\x10tracdap.metadata\x1a\x1btracdap/metadata/type.proto\x1a tracdap/metadata/object_id.proto\"\xaf\x01\n\nSearchTerm\x12\x10\n\x08\x61ttrName\x18\x01 \x01(\t\x12-\n\x08\x61ttrType\x18\x02 \x01(\x0e\x32\x1b.tracdap.metadata.BasicType\x12\x32\n\x08operator\x18\x03 \x01(\x0e\x32 .tracdap.metadata.SearchOperator\x12,\n\x0bsearchValue\x18\x04 \x01(\x0b\x32\x17.tracdap.metadata.Value\"z\n\x11LogicalExpression\x12\x33\n\x08operator\x18\x01 \x01(\x0e\x32!.tracdap.metadata.LogicalOperator\x12\x30\n\x04\x65xpr\x18\x02 \x03(\x0b\x32\".tracdap.metadata.SearchExpression\"\x80\x01\n\x10SearchExpression\x12,\n\x04term\x18\x01 \x01(\x0b\x32\x1c.tracdap.metadata.SearchTermH\x00\x12\x36\n\x07logical\x18\x02 \x01(\x0b\x32#.tracdap.metadata.LogicalExpressionH\x00\x42\x06\n\x04\x65xpr\"\xeb\x01\n\x10SearchParameters\x12\x30\n\nobjectType\x18\x01 \x01(\x0e\x32\x1c.tracdap.metadata.ObjectType\x12\x32\n\x06search\x18\x02 \x01(\x0b\x32\".tracdap.metadata.SearchExpression\x12\x38\n\nsearchAsOf\x18\x03 \x01(\x0b\x32\x1f.tracdap.metadata.DatetimeValueH\x00\x88\x01\x01\x12\x15\n\rpriorVersions\x18\x04 \x01(\x08\x12\x11\n\tpriorTags\x18\x05 \x01(\x08\x42\r\n\x0b_searchAsOf*q\n\x0eSearchOperator\x12\x1b\n\x17SEARCH_OPERATOR_NOT_SET\x10\x00\x12\x06\n\x02\x45Q\x10\x01\x12\x06\n\x02NE\x10\x02\x12\x06\n\x02LT\x10\x03\x12\x06\n\x02LE\x10\x04\x12\x06\n\x02GT\x10\x05\x12\x06\n\x02GE\x10\x06\x12\x06\n\x02IN\x10\x07\x12\n\n\x06\x45XISTS\x10\x08*I\n\x0fLogicalOperator\x12\x1c\n\x18LOGICAL_OPERATOR_NOT_SET\x10\x00\x12\x07\n\x03\x41ND\x10\x01\x12\x06\n\x02OR\x10\x02\x12\x07\n\x03NOT\x10\x03\x42\x1e\n\x1aorg.finos.tracdap.metadataP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tracdap.metadata.search_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\032org.finos.tracdap.metadataP\001'
   _SEARCHOPERATOR._serialized_start=785
-  _SEARCHOPERATOR._serialized_end=886
-  _LOGICALOPERATOR._serialized_start=888
-  _LOGICALOPERATOR._serialized_end=961
+  _SEARCHOPERATOR._serialized_end=898
+  _LOGICALOPERATOR._serialized_start=900
+  _LOGICALOPERATOR._serialized_end=973
   _SEARCHTERM._serialized_start=115
   _SEARCHTERM._serialized_end=290
   _LOGICALEXPRESSION._serialized_start=292
   _LOGICALEXPRESSION._serialized_end=414
   _SEARCHEXPRESSION._serialized_start=417
   _SEARCHEXPRESSION._serialized_end=545
   _SEARCHPARAMETERS._serialized_start=548
```

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/stoarge.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/stoarge.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/stoarge_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/stoarge_pb2.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/tag.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/tag.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/tag_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/tag_pb2.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/tag_update.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/tag_update.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/tag_update_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/tag_update_pb2.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/type.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/type.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/src/tracdap/rt/metadata/type_pb2.py` & `tracdap-runtime-0.6.0rc1/src/tracdap/rt/metadata/type_pb2.py`

 * *Files identical despite different names*

### Comparing `tracdap-runtime-0.5.9/tracdap_runtime.egg-info/PKG-INFO` & `tracdap-runtime-0.6.0rc1/tracdap_runtime.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracdap-runtime
-Version: 0.5.9
+Version: 0.6.0rc1
 Summary: Runtime package for building models on the TRAC Data & Analytics Platform
 Home-page: https://tracdap.finos.org/
 Author: Martin Traverse
 Author-email: martin.traverse@accenture.com
 License: Apache-2.0
 Project-URL: Documentation, https://tracdap.readthedocs.io/
 Project-URL: Source Code, https://github.com/finos/tracdap
@@ -35,17 +35,17 @@
 
 ## Requirements
 
 The TRAC runtime for Python has these requirements:
 
 * Python: 3.7 up to 3.11.x
 * Pandas: 1.2 up to 1.5.x
-* PySpark 2.4.x, or 3.0 up to 3.3.x
+* PySpark 3.0 up to 3.4.x (optional)
 
-Not every combination of versions will work, e.g. PySpark 3 requires Python 3.8.
+Not every combination of versions will work, e.g. using PySpark 3 requires Python 3.8.
 
 
 ## Installing the runtime
 
 The TRAC runtime package can be installed directly from PyPI:
 
     pip install tracdap-runtime
```

### Comparing `tracdap-runtime-0.5.9/tracdap_runtime.egg-info/SOURCES.txt` & `tracdap-runtime-0.6.0rc1/tracdap_runtime.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,26 +12,36 @@
 src/tracdap/rt/_exec/engine.py
 src/tracdap/rt/_exec/functions.py
 src/tracdap/rt/_exec/graph.py
 src/tracdap/rt/_exec/graph_builder.py
 src/tracdap/rt/_exec/runtime.py
 src/tracdap/rt/_impl/__init__.py
 src/tracdap/rt/_impl/config_parser.py
-src/tracdap/rt/_impl/csv_codec.py
 src/tracdap/rt/_impl/data.py
+src/tracdap/rt/_impl/guard_rails.py
 src/tracdap/rt/_impl/models.py
 src/tracdap/rt/_impl/repos.py
 src/tracdap/rt/_impl/schemas.py
 src/tracdap/rt/_impl/shim.py
 src/tracdap/rt/_impl/static_api.py
 src/tracdap/rt/_impl/storage.py
 src/tracdap/rt/_impl/type_system.py
 src/tracdap/rt/_impl/util.py
 src/tracdap/rt/_impl/validation.py
-src/tracdap/rt/_plugins/aws_storage.py
+src/tracdap/rt/_plugins/__init__.py
+src/tracdap/rt/_plugins/_helpers.py
+src/tracdap/rt/_plugins/format_arrow.py
+src/tracdap/rt/_plugins/format_csv.py
+src/tracdap/rt/_plugins/format_parquet.py
+src/tracdap/rt/_plugins/repo_git.py
+src/tracdap/rt/_plugins/repo_local.py
+src/tracdap/rt/_plugins/repo_pypi.py
+src/tracdap/rt/_plugins/storage_aws.py
+src/tracdap/rt/_plugins/storage_gcp.py
+src/tracdap/rt/_plugins/storage_local.py
 src/tracdap/rt/api/__init__.py
 src/tracdap/rt/api/hook.py
 src/tracdap/rt/api/model_api.py
 src/tracdap/rt/api/static_api.py
 src/tracdap/rt/config/__init__.py
 src/tracdap/rt/config/common.py
 src/tracdap/rt/config/common_pb2.py
@@ -42,15 +52,17 @@
 src/tracdap/rt/config/platform.py
 src/tracdap/rt/config/platform_pb2.py
 src/tracdap/rt/config/result.py
 src/tracdap/rt/config/result_pb2.py
 src/tracdap/rt/config/runtime.py
 src/tracdap/rt/config/runtime_pb2.py
 src/tracdap/rt/ext/__init__.py
+src/tracdap/rt/ext/_guard.py
 src/tracdap/rt/ext/embed.py
+src/tracdap/rt/ext/plugins.py
 src/tracdap/rt/ext/repos.py
 src/tracdap/rt/ext/storage.py
 src/tracdap/rt/launch/__init__.py
 src/tracdap/rt/launch/__main__.py
 src/tracdap/rt/launch/cli.py
 src/tracdap/rt/launch/launch.py
 src/tracdap/rt/metadata/__init__.py
```

