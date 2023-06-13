# Comparing `tmp/vald-client-python-1.7.5.tar.gz` & `tmp/vald-client-python-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vald-client-python-1.7.5.tar", last modified: Tue Apr 25 02:48:47 2023, max compression
+gzip compressed data, was "vald-client-python-1.7.6.tar", last modified: Tue Jun 13 05:54:33 2023, max compression
```

## Comparing `vald-client-python-1.7.5.tar` & `vald-client-python-1.7.6.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.901369 vald-client-python-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-25 02:48:47.901369 vald-client-python-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-25 02:48:47.901369 vald-client-python-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/google/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/google/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/google/api/annotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/google/api/annotations_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/google/rpc/status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/google/rpc/status_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/vald/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/vald/v1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/vald/v1/agent/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/vald/v1/agent/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/agent/core/agent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/agent/core/agent_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/vald/v1/filter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/vald/v1/filter/egress/
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/filter/egress/egress_filter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/filter/egress/egress_filter_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/vald/v1/filter/ingress/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/filter/ingress/ingress_filter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/filter/ingress/ingress_filter_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/vald/v1/payload/
--rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/payload/payload_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/payload/payload_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/vald/v1/vald/
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/filter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/filter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/insert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/insert_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/object_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/object_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/remove_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/remove_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/search_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21741 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/search_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/update_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/update_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/upsert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/vald/v1/vald/upsert_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.897369 vald-client-python-1.7.5/src/vald_client_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-25 02:48:47.000000 vald-client-python-1.7.5/src/vald_client_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-25 02:48:47.000000 vald-client-python-1.7.5/src/vald_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 02:48:47.000000 vald-client-python-1.7.5/src/vald_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 02:48:47.000000 vald-client-python-1.7.5/src/vald_client_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-25 02:48:47.000000 vald-client-python-1.7.5/src/vald_client_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 02:48:47.000000 vald-client-python-1.7.5/src/vald_client_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 02:48:47.901369 vald-client-python-1.7.5/src/validate/
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/validate/validate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-25 02:48:37.000000 vald-client-python-1.7.5/src/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.385976 vald-client-python-1.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-13 05:54:33.385976 vald-client-python-1.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-13 05:54:33.389977 vald-client-python-1.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.373976 vald-client-python-1.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.369976 vald-client-python-1.7.6/src/google/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.373976 vald-client-python-1.7.6/src/google/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/google/api/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/google/api/annotations_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.377976 vald-client-python-1.7.6/src/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/google/rpc/status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/google/rpc/status_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.369976 vald-client-python-1.7.6/src/vald/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.369976 vald-client-python-1.7.6/src/vald/v1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.369976 vald-client-python-1.7.6/src/vald/v1/agent/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.377976 vald-client-python-1.7.6/src/vald/v1/agent/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/agent/core/agent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/agent/core/agent_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.369976 vald-client-python-1.7.6/src/vald/v1/filter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.377976 vald-client-python-1.7.6/src/vald/v1/filter/egress/
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/filter/egress/egress_filter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/filter/egress/egress_filter_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.377976 vald-client-python-1.7.6/src/vald/v1/filter/ingress/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/filter/ingress/ingress_filter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/filter/ingress/ingress_filter_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.381976 vald-client-python-1.7.6/src/vald/v1/payload/
+-rw-r--r--   0 runner    (1001) docker     (123)    25480 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/payload/payload_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/payload/payload_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.385976 vald-client-python-1.7.6/src/vald/v1/vald/
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/filter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/filter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/insert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/insert_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/object_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/object_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/remove_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/remove_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/search_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21741 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/search_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/update_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/update_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/upsert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vald/v1/vald/upsert_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.385976 vald-client-python-1.7.6/src/vald_client_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-13 05:54:33.000000 vald-client-python-1.7.6/src/vald_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-13 05:54:33.000000 vald-client-python-1.7.6/src/vald_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:54:33.000000 vald-client-python-1.7.6/src/vald_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:54:33.000000 vald-client-python-1.7.6/src/vald_client_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 05:54:33.000000 vald-client-python-1.7.6/src/vald_client_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-13 05:54:33.000000 vald-client-python-1.7.6/src/vald_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.385976 vald-client-python-1.7.6/src/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/validate/validate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:54:33.385976 vald-client-python-1.7.6/src/vtproto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vtproto/ext_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 05:54:18.000000 vald-client-python-1.7.6/src/vtproto/ext_pb2_grpc.py
```

### Comparing `vald-client-python-1.7.5/LICENSE` & `vald-client-python-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/PKG-INFO` & `vald-client-python-1.7.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vald-client-python
-Version: 1.7.5
+Version: 1.7.6
 Summary: a client library for Vald (https://github.com/vdaas/vald).
 Home-page: https://github.com/vdaas/vald-client-python
 Author: vald team
 Author-email: vald@vdaas.org
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `vald-client-python-1.7.5/README.md` & `vald-client-python-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/setup.cfg` & `vald-client-python-1.7.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vald-client-python
-version = 1.7.5
+version = 1.7.6
 url = https://github.com/vdaas/vald-client-python
 description = a client library for Vald (https://github.com/vdaas/vald).
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = vald team
 author_email = vald@vdaas.org
 license_file = LICENSE
```

### Comparing `vald-client-python-1.7.5/src/google/api/annotations_pb2.py` & `vald-client-python-1.7.6/src/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/google/rpc/status_pb2.py` & `vald-client-python-1.7.6/src/google/rpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/agent/core/agent_pb2.py` & `vald-client-python-1.7.6/src/vald/v1/agent/core/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/agent/core/agent_pb2_grpc.py` & `vald-client-python-1.7.6/src/vald/v1/agent/core/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/filter/egress/egress_filter_pb2.py` & `vald-client-python-1.7.6/src/vald/v1/filter/egress/egress_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/filter/egress/egress_filter_pb2_grpc.py` & `vald-client-python-1.7.6/src/vald/v1/filter/egress/egress_filter_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/filter/ingress/ingress_filter_pb2.py` & `vald-client-python-1.7.6/src/vald/v1/filter/ingress/ingress_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/filter/ingress/ingress_filter_pb2_grpc.py` & `vald-client-python-1.7.6/src/vald/v1/filter/ingress/ingress_filter_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/filter_pb2.py` & `vald-client-python-1.7.6/src/vald/v1/vald/filter_pb2.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/filter_pb2_grpc.py` & `vald-client-python-1.7.6/src/vald/v1/vald/filter_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/insert_pb2.py` & `vald-client-python-1.7.6/src/vald/v1/vald/insert_pb2.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/insert_pb2_grpc.py` & `vald-client-python-1.7.6/src/vald/v1/vald/insert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/object_pb2.py` & `vald-client-python-1.7.6/src/vald/v1/vald/object_pb2.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/object_pb2_grpc.py` & `vald-client-python-1.7.6/src/vald/v1/vald/object_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/remove_pb2.py` & `vald-client-python-1.7.6/src/vald/v1/vald/remove_pb2.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/remove_pb2_grpc.py` & `vald-client-python-1.7.6/src/vald/v1/vald/remove_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/search_pb2.py` & `vald-client-python-1.7.6/src/vald/v1/vald/search_pb2.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/search_pb2_grpc.py` & `vald-client-python-1.7.6/src/vald/v1/vald/search_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/update_pb2.py` & `vald-client-python-1.7.6/src/vald/v1/vald/update_pb2.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/update_pb2_grpc.py` & `vald-client-python-1.7.6/src/vald/v1/vald/update_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/upsert_pb2.py` & `vald-client-python-1.7.6/src/vald/v1/vald/upsert_pb2.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald/v1/vald/upsert_pb2_grpc.py` & `vald-client-python-1.7.6/src/vald/v1/vald/upsert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `vald-client-python-1.7.5/src/vald_client_python.egg-info/PKG-INFO` & `vald-client-python-1.7.6/src/vald_client_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vald-client-python
-Version: 1.7.5
+Version: 1.7.6
 Summary: a client library for Vald (https://github.com/vdaas/vald).
 Home-page: https://github.com/vdaas/vald-client-python
 Author: vald team
 Author-email: vald@vdaas.org
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `vald-client-python-1.7.5/src/vald_client_python.egg-info/SOURCES.txt` & `vald-client-python-1.7.6/src/vald_client_python.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -31,8 +31,10 @@
 src/vald_client_python.egg-info/PKG-INFO
 src/vald_client_python.egg-info/SOURCES.txt
 src/vald_client_python.egg-info/dependency_links.txt
 src/vald_client_python.egg-info/not-zip-safe
 src/vald_client_python.egg-info/requires.txt
 src/vald_client_python.egg-info/top_level.txt
 src/validate/validate_pb2.py
-src/validate/validate_pb2_grpc.py
+src/validate/validate_pb2_grpc.py
+src/vtproto/ext_pb2.py
+src/vtproto/ext_pb2_grpc.py
```

### Comparing `vald-client-python-1.7.5/src/validate/validate_pb2.py` & `vald-client-python-1.7.6/src/validate/validate_pb2.py`

 * *Files identical despite different names*

