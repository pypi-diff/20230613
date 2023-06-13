# Comparing `tmp/brayns-3.1.2.tar.gz` & `tmp/brayns-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brayns-3.1.2.tar", last modified: Mon May  1 07:05:29 2023, max compression
+gzip compressed data, was "brayns-3.2.0.tar", last modified: Tue Jun 13 13:05:16 2023, max compression
```

## Comparing `brayns-3.1.2.tar` & `brayns-3.2.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:05:29.927529 brayns-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-01 07:05:26.000000 brayns-3.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-01 07:05:29.927529 brayns-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-01 07:05:26.000000 brayns-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:05:29.919529 brayns-3.1.2/brayns/
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:05:29.923529 brayns-3.1.2/brayns/core/
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/camera_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/color_ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/coloring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/framebuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/gbuffer_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/opacity_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/pick.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/core/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:05:29.923529 brayns-3.1.2/brayns/movie/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/movie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/movie/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/movie/movie_frames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:05:29.923529 brayns-3.1.2/brayns/network/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/future.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:05:29.927529 brayns-3.1.2/brayns/network/jsonrpc/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/jsonrpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/jsonrpc/json_rpc_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/jsonrpc/json_rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/jsonrpc/json_rpc_future.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/jsonrpc/json_rpc_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/jsonrpc/json_rpc_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/jsonrpc/json_rpc_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/jsonrpc/json_rpc_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/jsonrpc/json_rpc_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/jsonrpc/json_rpc_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/jsonrpc/json_rpc_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/jsonrpc/json_rpc_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:05:29.927529 brayns-3.1.2/brayns/network/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/websocket/async_web_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/websocket/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/websocket/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/websocket/web_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/websocket/web_socket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/websocket/web_socket_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/network/websocket/web_socket_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:05:29.927529 brayns-3.1.2/brayns/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/plugins/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/plugins/bbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/plugins/cell_placement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/plugins/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/plugins/cylindric_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/plugins/dti.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/plugins/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/plugins/nrrd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/plugins/protein.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/plugins/sonata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/plugins/xyz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:05:29.927529 brayns-3.1.2/brayns/service/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/service/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/service/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:05:29.927529 brayns-3.1.2/brayns/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/utils/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/utils/plane_equation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/utils/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/utils/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/utils/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-01 07:05:26.000000 brayns-3.1.2/brayns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:05:29.919529 brayns-3.1.2/brayns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-01 07:05:29.000000 brayns-3.1.2/brayns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-01 07:05:29.000000 brayns-3.1.2/brayns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:05:29.000000 brayns-3.1.2/brayns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 07:05:29.000000 brayns-3.1.2/brayns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 07:05:29.000000 brayns-3.1.2/brayns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-01 07:05:26.000000 brayns-3.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-01 07:05:29.931529 brayns-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-01 07:05:26.000000 brayns-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:16.561423 brayns-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 13:05:13.000000 brayns-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-13 13:05:16.561423 brayns-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-13 13:05:13.000000 brayns-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:16.549423 brayns-3.2.0/brayns/
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:16.553424 brayns-3.2.0/brayns/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/camera_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/color_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/coloring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/framebuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/gbuffer_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/opacity_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/pick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/core/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:16.553424 brayns-3.2.0/brayns/movie/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/movie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/movie/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/movie/movie_frames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:16.553424 brayns-3.2.0/brayns/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:16.557423 brayns-3.2.0/brayns/network/jsonrpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/jsonrpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/jsonrpc/json_rpc_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/jsonrpc/json_rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/jsonrpc/json_rpc_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/jsonrpc/json_rpc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/jsonrpc/json_rpc_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/jsonrpc/json_rpc_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/jsonrpc/json_rpc_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/jsonrpc/json_rpc_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/jsonrpc/json_rpc_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/jsonrpc/json_rpc_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/jsonrpc/json_rpc_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:16.557423 brayns-3.2.0/brayns/network/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/websocket/async_web_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/websocket/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/websocket/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/websocket/web_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/websocket/web_socket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/websocket/web_socket_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/network/websocket/web_socket_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:16.557423 brayns-3.2.0/brayns/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/plugins/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/plugins/bbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/plugins/cell_placement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/plugins/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/plugins/cylindric_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/plugins/dti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/plugins/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/plugins/nrrd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/plugins/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/plugins/sonata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/plugins/xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:16.557423 brayns-3.2.0/brayns/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/service/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/service/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:16.561423 brayns-3.2.0/brayns/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/utils/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/utils/plane_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/utils/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/utils/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/utils/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-13 13:05:13.000000 brayns-3.2.0/brayns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:16.549423 brayns-3.2.0/brayns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-13 13:05:16.000000 brayns-3.2.0/brayns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-13 13:05:16.000000 brayns-3.2.0/brayns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:05:16.000000 brayns-3.2.0/brayns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 13:05:16.000000 brayns-3.2.0/brayns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 13:05:16.000000 brayns-3.2.0/brayns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-13 13:05:13.000000 brayns-3.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-13 13:05:16.561423 brayns-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-13 13:05:13.000000 brayns-3.2.0/setup.py
```

### Comparing `brayns-3.1.2/PKG-INFO` & `brayns-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brayns
-Version: 3.1.2
+Version: 3.2.0
 Summary: Brayns Python API
 Home-page: https://github.com/BlueBrain/Brayns
 Author: Blue Brain Project
 Author-email: bbp-open-source@googlegroups.com
 License: LGPLv3
 Download-URL: https://github.com/BlueBrain/Brayns
 Project-URL: Tracker, https://bbpteam.epfl.ch/project/issues/projects/BRAYNS/issues
```

### Comparing `brayns-3.1.2/README.md` & `brayns-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/__init__.py` & `brayns-3.2.0/brayns/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     EmissiveMaterial,
     Entrypoint,
     Fovy,
     Framebuffer,
     GBufferChannel,
     GBufferExporter,
     Geometry,
+    GhostMaterial,
     GlassMaterial,
     Image,
     ImageInfo,
     InteractiveRenderer,
     Light,
     Loader,
     LoaderInfo,
@@ -310,14 +311,15 @@
     "get_model",
     "get_models",
     "get_renderer_name",
     "get_renderer",
     "get_scene",
     "get_simulation",
     "get_version",
+    "GhostMaterial",
     "GlassMaterial",
     "Image",
     "ImageFormat",
     "ImageInfo",
     "Instance",
     "instantiate_model",
     "InteractiveRenderer",
```

### Comparing `brayns-3.1.2/brayns/core/__init__.py` & `brayns-3.2.0/brayns/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     RawVolumeLoader,
     VolumeDataType,
     get_loaders,
 )
 from .material import (
     CarPaintMaterial,
     EmissiveMaterial,
+    GhostMaterial,
     GlassMaterial,
     Material,
     MatteMaterial,
     MetalMaterial,
     PhongMaterial,
     PlasticMaterial,
     get_material,
@@ -188,14 +189,15 @@
     "get_model",
     "get_models",
     "get_renderer_name",
     "get_renderer",
     "get_scene",
     "get_simulation",
     "get_version",
+    "GhostMaterial",
     "GlassMaterial",
     "Image",
     "ImageInfo",
     "instantiate_model",
     "InteractiveRenderer",
     "Light",
     "Loader",
```

### Comparing `brayns-3.1.2/brayns/core/application.py` & `brayns-3.2.0/brayns/core/application.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/camera.py` & `brayns-3.2.0/brayns/core/camera.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/camera_controller.py` & `brayns-3.2.0/brayns/core/camera_controller.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/color_ramp.py` & `brayns-3.2.0/brayns/core/color_ramp.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/coloring.py` & `brayns-3.2.0/brayns/core/coloring.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/entrypoint.py` & `brayns-3.2.0/brayns/core/entrypoint.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/framebuffer.py` & `brayns-3.2.0/brayns/core/framebuffer.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/gbuffer_exporter.py` & `brayns-3.2.0/brayns/core/gbuffer_exporter.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/geometry.py` & `brayns-3.2.0/brayns/core/geometry.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/image.py` & `brayns-3.2.0/brayns/core/image.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/light.py` & `brayns-3.2.0/brayns/core/light.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/loader.py` & `brayns-3.2.0/brayns/core/loader.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/material.py` & `brayns-3.2.0/brayns/core/material.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,37 @@
 
     def update_properties(self, message: dict[str, Any]) -> None:
         """Low level API to deserialize from JSON."""
         self.refraction_index = message["index_of_refraction"]
 
 
 @dataclass
+class GhostMaterial(Material):
+    """Ghost material."""
+
+    @classmethod
+    @property
+    def name(cls) -> str:
+        """Get the material name.
+
+        :return: Material name
+        :rtype: str
+        """
+        return "ghost"
+
+    def get_properties(self) -> dict[str, Any]:
+        """Low level API to serialize to JSON."""
+        return {}
+
+    def update_properties(self, message: dict[str, Any]) -> None:
+        """Low level API to deserialize from JSON."""
+        pass
+
+
+@dataclass
 class MatteMaterial(Material):
     """Matte material.
 
     :param opacity: Opacity (0-1), defaults to fully opaque.
     :type opacity: float, optional
     """
```

### Comparing `brayns-3.1.2/brayns/core/model.py` & `brayns-3.2.0/brayns/core/model.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/opacity_curve.py` & `brayns-3.2.0/brayns/core/opacity_curve.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/pick.py` & `brayns-3.2.0/brayns/core/pick.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/projection.py` & `brayns-3.2.0/brayns/core/projection.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/renderer.py` & `brayns-3.2.0/brayns/core/renderer.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/simulation.py` & `brayns-3.2.0/brayns/core/simulation.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/snapshot.py` & `brayns-3.2.0/brayns/core/snapshot.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/version.py` & `brayns-3.2.0/brayns/core/version.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/core/view.py` & `brayns-3.2.0/brayns/core/view.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/movie/__init__.py` & `brayns-3.2.0/brayns/movie/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/movie/movie.py` & `brayns-3.2.0/brayns/movie/movie.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/movie/movie_frames.py` & `brayns-3.2.0/brayns/movie/movie_frames.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/__init__.py` & `brayns-3.2.0/brayns/network/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/client.py` & `brayns-3.2.0/brayns/network/client.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/connector.py` & `brayns-3.2.0/brayns/network/connector.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/future.py` & `brayns-3.2.0/brayns/network/future.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/instance.py` & `brayns-3.2.0/brayns/network/instance.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/jsonrpc/__init__.py` & `brayns-3.2.0/brayns/network/jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/jsonrpc/json_rpc_dispatcher.py` & `brayns-3.2.0/brayns/network/jsonrpc/json_rpc_dispatcher.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/jsonrpc/json_rpc_error.py` & `brayns-3.2.0/brayns/network/jsonrpc/json_rpc_error.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/jsonrpc/json_rpc_future.py` & `brayns-3.2.0/brayns/network/jsonrpc/json_rpc_future.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/jsonrpc/json_rpc_handler.py` & `brayns-3.2.0/brayns/network/jsonrpc/json_rpc_handler.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/jsonrpc/json_rpc_listener.py` & `brayns-3.2.0/brayns/network/jsonrpc/json_rpc_listener.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/jsonrpc/json_rpc_manager.py` & `brayns-3.2.0/brayns/network/jsonrpc/json_rpc_manager.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/jsonrpc/json_rpc_progress.py` & `brayns-3.2.0/brayns/network/jsonrpc/json_rpc_progress.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/jsonrpc/json_rpc_reply.py` & `brayns-3.2.0/brayns/network/jsonrpc/json_rpc_reply.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/jsonrpc/json_rpc_request.py` & `brayns-3.2.0/brayns/network/jsonrpc/json_rpc_request.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/jsonrpc/json_rpc_task.py` & `brayns-3.2.0/brayns/network/jsonrpc/json_rpc_task.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/jsonrpc/json_rpc_tasks.py` & `brayns-3.2.0/brayns/network/jsonrpc/json_rpc_tasks.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/listener.py` & `brayns-3.2.0/brayns/network/listener.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/logger.py` & `brayns-3.2.0/brayns/network/logger.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/websocket/__init__.py` & `brayns-3.2.0/brayns/network/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/websocket/async_web_socket.py` & `brayns-3.2.0/brayns/network/websocket/async_web_socket.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/websocket/errors.py` & `brayns-3.2.0/brayns/network/websocket/errors.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/websocket/event_loop.py` & `brayns-3.2.0/brayns/network/websocket/event_loop.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/websocket/web_socket.py` & `brayns-3.2.0/brayns/network/websocket/web_socket.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/websocket/web_socket_client.py` & `brayns-3.2.0/brayns/network/websocket/web_socket_client.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/websocket/web_socket_connector.py` & `brayns-3.2.0/brayns/network/websocket/web_socket_connector.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/network/websocket/web_socket_listener.py` & `brayns-3.2.0/brayns/network/websocket/web_socket_listener.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/plugins/__init__.py` & `brayns-3.2.0/brayns/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/plugins/atlas.py` & `brayns-3.2.0/brayns/plugins/atlas.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/plugins/bbp.py` & `brayns-3.2.0/brayns/plugins/bbp.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/plugins/cell_placement.py` & `brayns-3.2.0/brayns/plugins/cell_placement.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/plugins/circuit.py` & `brayns-3.2.0/brayns/plugins/circuit.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/plugins/cylindric_camera.py` & `brayns-3.2.0/brayns/plugins/cylindric_camera.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/plugins/dti.py` & `brayns-3.2.0/brayns/plugins/dti.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/plugins/morphology.py` & `brayns-3.2.0/brayns/plugins/morphology.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/plugins/nrrd.py` & `brayns-3.2.0/brayns/plugins/nrrd.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/plugins/protein.py` & `brayns-3.2.0/brayns/plugins/protein.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/plugins/sonata.py` & `brayns-3.2.0/brayns/plugins/sonata.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/plugins/xyz.py` & `brayns-3.2.0/brayns/plugins/xyz.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/service/__init__.py` & `brayns-3.2.0/brayns/service/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/service/manager.py` & `brayns-3.2.0/brayns/service/manager.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/service/process.py` & `brayns-3.2.0/brayns/service/process.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/service/service.py` & `brayns-3.2.0/brayns/service/service.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/utils/__init__.py` & `brayns-3.2.0/brayns/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/utils/bounds.py` & `brayns-3.2.0/brayns/utils/bounds.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/utils/color.py` & `brayns-3.2.0/brayns/utils/color.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/utils/error.py` & `brayns-3.2.0/brayns/utils/error.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/utils/image.py` & `brayns-3.2.0/brayns/utils/image.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/utils/json_schema.py` & `brayns-3.2.0/brayns/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/utils/plane_equation.py` & `brayns-3.2.0/brayns/utils/plane_equation.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/utils/quaternion.py` & `brayns-3.2.0/brayns/utils/quaternion.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/utils/rotation.py` & `brayns-3.2.0/brayns/utils/rotation.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/utils/transform.py` & `brayns-3.2.0/brayns/utils/transform.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/utils/vector.py` & `brayns-3.2.0/brayns/utils/vector.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/brayns/version.py` & `brayns-3.2.0/requirements.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) 2015-2023 EPFL/Blue Brain Project
-# All rights reserved. Do not distribute without permission.
-#
-# Responsible Author: adrien.fleury@epfl.ch
+# Copyright (c) 2015-2023, Blue Brain Project
+#                          Raphael Dumusc <raphael.dumusc@epfl.ch>
+#                          Daniel Nachbaur <daniel.nachbaur@epfl.ch>
+#                          Cyrille Favreau <cyrille.favreau@epfl.ch>
+#                          Nadir Roman <nadir.romanguerrero@epfl.ch>
 #
 # This file is part of Brayns <https://github.com/BlueBrain/Brayns>
 #
 # This library is free software; you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License version 3.0 as published
 # by the Free Software Foundation.
 #
@@ -13,10 +14,18 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
+# All rights reserved. Do not distribute without further notice.
 
-VERSION = "3.1.2"
-"""Version tag of brayns Python package (major.minor.patch)."""
+websockets~=10.3
+Pillow~=9.3.0
+PySimpleGUI~=4.60.1
+pyright~=1.1.284
+black~=22.12.0
+flake8~=6.0.0
+sphinx-bluebrain-theme~=0.4.0
+sphinx-jsonschema~=1.19.1
+sphinx~=6.1.3
```

### Comparing `brayns-3.1.2/brayns.egg-info/PKG-INFO` & `brayns-3.2.0/brayns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brayns
-Version: 3.1.2
+Version: 3.2.0
 Summary: Brayns Python API
 Home-page: https://github.com/BlueBrain/Brayns
 Author: Blue Brain Project
 Author-email: bbp-open-source@googlegroups.com
 License: LGPLv3
 Download-URL: https://github.com/BlueBrain/Brayns
 Project-URL: Tracker, https://bbpteam.epfl.ch/project/issues/projects/BRAYNS/issues
```

### Comparing `brayns-3.1.2/brayns.egg-info/SOURCES.txt` & `brayns-3.2.0/brayns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brayns-3.1.2/requirements.txt` & `brayns-3.2.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
 # Copyright (c) 2015-2023, Blue Brain Project
 #                          Raphael Dumusc <raphael.dumusc@epfl.ch>
 #                          Daniel Nachbaur <daniel.nachbaur@epfl.ch>
 #                          Cyrille Favreau <cyrille.favreau@epfl.ch>
 #                          Nadir Roman <nadir.romanguerrero@epfl.ch>
 #
 # This file is part of Brayns <https://github.com/BlueBrain/Brayns>
@@ -16,16 +19,10 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 # All rights reserved. Do not distribute without further notice.
 
-websockets~=10.3
-Pillow~=9.3.0
-PySimpleGUI~=4.60.1
-pyright~=1.1.284
-black~=22.12.0
-flake8~=6.0.0
-sphinx-bluebrain-theme~=0.4.0
-sphinx-jsonschema~=1.19.1
-sphinx~=6.1.3
+import setuptools
+
+setuptools.setup()
```

### Comparing `brayns-3.1.2/setup.cfg` & `brayns-3.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = brayns
-version = 3.1.2
+version = 3.2.0
 url = https://github.com/BlueBrain/Brayns
 download_url = https://github.com/BlueBrain/Brayns
 project_urls = 
 	Tracker = https://bbpteam.epfl.ch/project/issues/projects/BRAYNS/issues
 	Source = https://github.com/BlueBrain/Brayns
 author = Blue Brain Project
 author_email = bbp-open-source@googlegroups.com
```

### Comparing `brayns-3.1.2/setup.py` & `brayns-3.2.0/brayns/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Copyright (c) 2015-2023, Blue Brain Project
-#                          Raphael Dumusc <raphael.dumusc@epfl.ch>
-#                          Daniel Nachbaur <daniel.nachbaur@epfl.ch>
-#                          Cyrille Favreau <cyrille.favreau@epfl.ch>
-#                          Nadir Roman <nadir.romanguerrero@epfl.ch>
+# Copyright (c) 2015-2023 EPFL/Blue Brain Project
+# All rights reserved. Do not distribute without permission.
+#
+# Responsible Author: adrien.fleury@epfl.ch
 #
 # This file is part of Brayns <https://github.com/BlueBrain/Brayns>
 #
 # This library is free software; you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License version 3.0 as published
 # by the Free Software Foundation.
 #
@@ -17,12 +13,10 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
-# All rights reserved. Do not distribute without further notice.
-
-import setuptools
 
-setuptools.setup()
+VERSION = "3.2.0"
+"""Version tag of brayns Python package (major.minor.patch)."""
```

