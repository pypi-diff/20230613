# Comparing `tmp/backend.ai-kernel-23.3.4.tar.gz` & `tmp/backend.ai-kernel-23.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-kernel-23.3.4.tar", last modified: Mon May 29 10:42:36 2023, max compression
+gzip compressed data, was "backend.ai-kernel-23.3.5.tar", last modified: Tue Jun 13 03:42:13 2023, max compression
```

## Comparing `backend.ai-kernel-23.3.4.tar` & `backend.ai-kernel-23.3.5.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.022984 backend.ai-kernel-23.3.4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.022984 backend.ai-kernel-23.3.4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.026984 backend.ai-kernel-23.3.4/ai/backend/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.026984 backend.ai-kernel-23.3.4/ai/backend/kernel/app/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36687 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.026984 backend.ai-kernel-23.3.4/ai/backend/kernel/c/
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.026984 backend.ai-kernel-23.3.4/ai/backend/kernel/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.026984 backend.ai-kernel-23.3.4/ai/backend/kernel/git/
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.026984 backend.ai-kernel-23.3.4/ai/backend/kernel/golang/
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/golang/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.026984 backend.ai-kernel-23.3.4/ai/backend/kernel/haskell/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/haskell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/intrinsic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.026984 backend.ai-kernel-23.3.4/ai/backend/kernel/java/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.026984 backend.ai-kernel-23.3.4/ai/backend/kernel/julia/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/julia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/jupyter_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.026984 backend.ai-kernel-23.3.4/ai/backend/kernel/lua/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/lua/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.026984 backend.ai-kernel-23.3.4/ai/backend/kernel/nodejs/
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/nodejs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/ai/backend/kernel/octave/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/octave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/ai/backend/kernel/php/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/php/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/ai/backend/kernel/python/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/ai/backend/kernel/python/drawing/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/python/drawing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/python/drawing/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/python/drawing/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/python/drawing/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/python/drawing/turtle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/python/sitecustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/python/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/ai/backend/kernel/r/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/r/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/ai/backend/kernel/r_server_ms/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/r_server_ms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/ai/backend/kernel/rust/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/rust/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/ai/backend/kernel/scheme/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/scheme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/service_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/ai/backend/kernel/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/ai/backend/kernel/vendor/aws_polly/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/vendor/aws_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/vendor/aws_polly/inproc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/ai/backend/kernel/vendor/h2o/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/ai/backend/kernel/vendor/h2o/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/backend.ai_kernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-29 10:42:36.000000 backend.ai-kernel-23.3.4/backend.ai_kernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-29 10:42:36.000000 backend.ai-kernel-23.3.4/backend.ai_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:36.000000 backend.ai-kernel-23.3.4/backend.ai_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:36.000000 backend.ai-kernel-23.3.4/backend.ai_kernel.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/backend.ai_kernel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-29 10:42:36.000000 backend.ai-kernel-23.3.4/backend.ai_kernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-29 10:42:36.000000 backend.ai-kernel-23.3.4/backend.ai_kernel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:42:36.030984 backend.ai-kernel-23.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-29 10:42:35.000000 backend.ai-kernel-23.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.576274 backend.ai-kernel-23.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-13 03:42:13.576274 backend.ai-kernel-23.3.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.564274 backend.ai-kernel-23.3.5/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.564274 backend.ai-kernel-23.3.5/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.568274 backend.ai-kernel-23.3.5/ai/backend/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.568274 backend.ai-kernel-23.3.5/ai/backend/kernel/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39380 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.568274 backend.ai-kernel-23.3.5/ai/backend/kernel/c/
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.568274 backend.ai-kernel-23.3.5/ai/backend/kernel/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.568274 backend.ai-kernel-23.3.5/ai/backend/kernel/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/golang/
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/golang/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/haskell/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/haskell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/intrinsic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/java/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/julia/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/julia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/jupyter_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/lua/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/lua/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/nodejs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/nodejs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/octave/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/octave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/php/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/php/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/python/drawing/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/python/drawing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/python/drawing/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/python/drawing/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/python/drawing/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/python/drawing/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/python/sitecustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/python/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/r/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/r/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/r_server_ms/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/r_server_ms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/rust/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/scheme/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/service_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.572274 backend.ai-kernel-23.3.5/ai/backend/kernel/vendor/aws_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/vendor/aws_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/vendor/aws_polly/inproc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.576274 backend.ai-kernel-23.3.5/ai/backend/kernel/vendor/h2o/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/ai/backend/kernel/vendor/h2o/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.576274 backend.ai-kernel-23.3.5/backend.ai_kernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/backend.ai_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/backend.ai_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/backend.ai_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/backend.ai_kernel.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/backend.ai_kernel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/backend.ai_kernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/backend.ai_kernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:42:13.576274 backend.ai-kernel-23.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-13 03:42:13.000000 backend.ai-kernel-23.3.5/setup.py
```

### Comparing `backend.ai-kernel-23.3.4/PKG-INFO` & `backend.ai-kernel-23.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel
-Version: 23.3.4
+Version: 23.3.5
 Summary: Backend.AI Kernel Runner
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/__main__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/app/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/app/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/base.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import concurrent.futures
 import json
 import logging
 import os
 import signal
 import sys
 import time
+import urllib.error
+import urllib.request
 import uuid
 from abc import ABCMeta, abstractmethod
 from functools import partial
 from pathlib import Path
 from typing import (
     Awaitable,
     ClassVar,
@@ -590,27 +592,85 @@
         )
 
     @abstractmethod
     async def start_service(self, service_info):
         """Start an application service daemon."""
         return None, {}
 
-    async def _start_service(self, service_info, user_requested: bool = True):
+    async def start_model_service(self, model_info):
+        assert self.service_parser is not None
+        model_service_info = model_info.get("service")
+        result = {}
+        is_healthy = False
+        try:
+            if model_service_info is None:
+                result = {"status": "failed", "error": "service info not provided"}
+                return
+            service_name = f"{model_info['name']}-{model_service_info['port']}"
+            self.service_parser.add_model_service(service_name, model_service_info)
+            service_info = {
+                "name": service_name,
+                "port": model_service_info["port"],
+                "ports": [model_service_info["port"]],
+                "protocol": "http",
+                "options": {},
+            }
+            result = await self._start_service(service_info, do_not_wait=True)
+            if (result["status"] == "running" or result["status"] == "started") and (
+                (health_check_info := model_service_info.get("health_check")) is not None
+            ):
+                health_check_endpoint = (
+                    f"http://localhost:{model_service_info['port']}{health_check_info['path']}"
+                )
+                for _ in range(health_check_info["max_retries"]):
+                    try:
+                        async with timeout(health_check_info["max_wait_time"]):
+                            try:
+                                resp = await asyncio.get_running_loop().run_in_executor(
+                                    None, urllib.request.urlopen, health_check_endpoint
+                                )
+                                if resp.status == health_check_info["expected_status_code"]:
+                                    is_healthy = True
+                                    break
+                            except urllib.error.URLError:
+                                pass
+                            # falling to here means that health check has failed, so just wait until
+                            # timeout is fired to fill out the gap between max_wait_time and actual time elapsed
+                            await asyncio.sleep(health_check_info["max_wait_time"])
+                    except asyncio.TimeoutError:
+                        pass
+        finally:
+            if not is_healthy:
+                result = {"status": "failed", "error": "service unhealthy"}
+            await self.outsock.send_multipart(
+                [
+                    b"model-service-result",
+                    json.dumps(result).encode("utf8"),
+                ]
+            )
+
+    async def _start_service_and_feed_result(self, service_info):
+        result = await self._start_service(service_info)
+        await self.outsock.send_multipart(
+            [
+                b"service-result",
+                json.dumps(result).encode("utf8"),
+            ]
+        )
+
+    async def _start_service(self, service_info, do_not_wait=False):
         async with self._service_lock:
             try:
                 if service_info["protocol"] == "preopen":
                     # skip subprocess spawning as we assume the user runs it manually.
-                    result = {"status": "started"}
-                    return
+                    return {"status": "started"}
                 if service_info["name"] in self.services_running:
-                    result = {"status": "running"}
-                    return
+                    return {"status": "running"}
                 if service_info["protocol"] == "pty":
-                    result = {"status": "failed", "error": "not implemented yet"}
-                    return
+                    return {"status": "failed", "error": "not implemented yet"}
                 cwd = Path.cwd()
                 cmdargs: Optional[Sequence[Union[str, os.PathLike]]]
                 env: Mapping[str, str]
                 cmdargs, env = None, {}
                 if service_info["name"] == "ttyd":
                     cmdargs, env = await prepare_ttyd_service(service_info)
                 elif service_info["name"] == "sshd":
@@ -630,19 +690,18 @@
                     elif len(start_info) == 3:
                         cmdargs, env, cwd = start_info
                     elif len(start_info) == 2:
                         cmdargs, env = start_info
                 if cmdargs is None:
                     # still not found?
                     log.warning("The service {0} is not supported.", service_info["name"])
-                    result = {
+                    return {
                         "status": "failed",
                         "error": "unsupported service",
                     }
-                    return
                 log.debug("cmdargs: {0}", cmdargs)
                 log.debug("env: {0}", env)
                 service_env = {**self.child_env, **env}
                 # avoid conflicts with Python binary used by service apps.
                 if "LD_LIBRARY_PATH" in service_env:
                     service_env["LD_LIBRARY_PATH"] = service_env["LD_LIBRARY_PATH"].replace(
                         "/opt/backend.ai/lib:", ""
@@ -651,63 +710,56 @@
                     proc = await asyncio.create_subprocess_exec(
                         *map(str, cmdargs),
                         env=service_env,
                         cwd=cwd,
                     )
                     self.services_running[service_info["name"]] = proc
                     asyncio.create_task(self._wait_service_proc(service_info["name"], proc))
-                    with timeout(5.0):
-                        await wait_local_port_open(service_info["port"])
+                    if not do_not_wait:
+                        with timeout(5.0):
+                            await wait_local_port_open(service_info["port"])
                     log.info(
                         "Service {} has started (pid: {}, port: {})",
                         service_info["name"],
                         proc.pid,
                         service_info["port"],
                     )
-                    result = {"status": "started"}
+                    return {"status": "started"}
                 except asyncio.CancelledError:
                     # This may happen if the service process gets started but it fails to
                     # open the port and then terminates (with an error).
-                    result = {
+                    return {
                         "status": "failed",
                         "error": f"the process did not start properly: {cmdargs[0]}",
                     }
                 except asyncio.TimeoutError:
                     # Takes too much time to open a local port.
                     if service_info["name"] in self.services_running:
                         await terminate_and_wait(proc, timeout=10.0)
                         self.services_running.pop(service_info["name"], None)
-                    result = {
+                    return {
                         "status": "failed",
                         "error": f"opening the service port timed out: {service_info['name']}",
                     }
                 except PermissionError:
-                    result = {
+                    return {
                         "status": "failed",
                         "error": f"the target file is not executable: {cmdargs[0]}",
                     }
                 except FileNotFoundError:
-                    result = {
+                    return {
                         "status": "failed",
                         "error": f"the executable file is not found: {cmdargs[0]}",
                     }
             except Exception as e:
                 log.exception("start_service: unexpected error")
-                result = {
+                return {
                     "status": "failed",
                     "error": repr(e),
                 }
-            finally:
-                if user_requested:
-                    await self.outsock.send_multipart(
-                        [
-                            b"service-result",
-                            json.dumps(result).encode("utf8"),
-                        ]
-                    )
 
     async def _wait_service_proc(
         self,
         service_name: str,
         proc: asyncio.subprocess.Process,
     ) -> None:
         exitcode = await proc.wait()
@@ -865,25 +917,23 @@
         intrinsic_spawn_coros.append(
             self._start_service(
                 {
                     "name": "sshd",
                     "port": self.intrinsic_host_ports_mapping.get("sshd", 2200),
                     "protocol": "tcp",
                 },
-                user_requested=False,
             )
         )
         intrinsic_spawn_coros.append(
             self._start_service(
                 {
                     "name": "ttyd",
                     "port": self.intrinsic_host_ports_mapping.get("ttyd", 7681),
                     "protocol": "http",
                 },
-                user_requested=False,
             )
         )
         results = await asyncio.gather(*intrinsic_spawn_coros, return_exceptions=True)
         for result in results:
             if isinstance(result, Exception):
                 log.exception(
                     "error during starting intrinsic services",
@@ -913,17 +963,20 @@
                 elif op_type == "complete":  # auto-completion
                     data = json.loads(text)
                     await self._complete(data)
                 elif op_type == "interrupt":
                     await self._interrupt()
                 elif op_type == "status":
                     await self._send_status()
+                elif op_type == "start-model-service":  # activate a service port
+                    data = json.loads(text)
+                    asyncio.create_task(self.start_model_service(data))
                 elif op_type == "start-service":  # activate a service port
                     data = json.loads(text)
-                    asyncio.create_task(self._start_service(data))
+                    asyncio.create_task(self._start_service_and_feed_result(data))
                 elif op_type == "shutdown-service":  # shutdown the service by its name
                     data = json.loads(text)
                     await self._shutdown_service(data)
                 elif op_type == "get-apps":
                     await self._get_apps(text)
             except asyncio.CancelledError:
                 break
```

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/c/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/c/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/compat.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/compat.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/cpp/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/cpp/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/git/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/git/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/golang/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/golang/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/haskell/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/haskell/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/intrinsic.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/intrinsic.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,16 +144,18 @@
         cmdargs.extend(["-p", f"0.0.0.0:{port_config}"])
     env = {}
     return cmdargs, env
 
 
 async def prepare_ttyd_service(service_info):
     shell = "sh"
-    if Path("/bin/bash").exists():
+    if Path("/bin/zsh").exists():
+        shell = "zsh"
+    elif Path("/bin/bash").exists():
         shell = "bash"
     elif Path("/bin/ash").exists():
         shell = "ash"
 
     cmdargs = ["/opt/backend.ai/bin/ttyd", "-p", service_info["port"], f"/bin/{shell}"]
     if shell != "ash":  # Currently Alpine-based containers are not supported.
-        cmdargs += ["-c", "/opt/kernel/tmux -2 attach"]
+        cmdargs += ["-c", f"export SHELL=/bin/{shell}; /opt/kernel/tmux -2 attach"]
     return cmdargs, {}
```

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/java/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/java/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/julia/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/julia/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/jupyter_client.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/jupyter_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/logging.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/logging.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/lua/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/lua/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/nodejs/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/nodejs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/octave/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/octave/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/php/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/php/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/python/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/python/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/python/drawing/canvas.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/python/drawing/canvas.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/python/drawing/color.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/python/drawing/color.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/python/drawing/turtle.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/python/drawing/turtle.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/python/sitecustomize.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/python/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/python/types.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/python/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/r/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/r/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/r_server_ms/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/r_server_ms/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/rust/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/rust/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/scheme/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/scheme/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/service.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,21 @@
                 )
             name = service_def_file.stem
             try:
                 self.services[name] = ServiceDefinition(**raw_service_def)
             except TypeError as e:
                 raise InvalidServiceDefinition(e.args[0][11:])  # lstrip "__init__() "
 
+    def add_model_service(self, name, model_service_info) -> None:
+        service_def = ServiceDefinition(
+            model_service_info["start_command"],
+            prestart_actions=model_service_info["pre_start_actions"],
+        )
+        self.services[name] = service_def
+
     async def start_service(
         self,
         service_name: str,
         frozen_envs: Collection[str],
         opts: Mapping[str, Any],
     ) -> Tuple[Optional[Sequence[str]], Mapping[str, str]]:
         if service_name not in self.services.keys():
```

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/service_actions.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/service_actions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/terminal.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/terminal.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/utils.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/vendor/aws_polly/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/vendor/aws_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/vendor/aws_polly/inproc.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/vendor/aws_polly/inproc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/ai/backend/kernel/vendor/h2o/__init__.py` & `backend.ai-kernel-23.3.5/ai/backend/kernel/vendor/h2o/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/backend.ai_kernel.egg-info/PKG-INFO` & `backend.ai-kernel-23.3.5/backend.ai_kernel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel
-Version: 23.3.4
+Version: 23.3.5
 Summary: Backend.AI Kernel Runner
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-23.3.4/backend.ai_kernel.egg-info/SOURCES.txt` & `backend.ai-kernel-23.3.5/backend.ai_kernel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/backend_shim.py` & `backend.ai-kernel-23.3.5/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.4/setup.py` & `backend.ai-kernel-23.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,11 +72,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.4
+    'version': """23.03.5
 """,
     'zip_safe': False,
 })
```

