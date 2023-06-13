# Comparing `tmp/taipy-rest-2.3.0.dev1.tar.gz` & `tmp/taipy-rest-2.3.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-rest-2.3.0.dev1.tar", last modified: Mon Jun  5 16:16:58 2023, max compression
+gzip compressed data, was "taipy-rest-2.3.0.dev2.tar", last modified: Tue Jun 13 17:49:57 2023, max compression
```

## Comparing `taipy-rest-2.3.0.dev1.tar` & `taipy-rest-2.3.0.dev2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:16:58.180915 taipy-rest-2.3.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-05 16:16:58.180915 taipy-rest-2.3.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:16:58.180915 taipy-rest-2.3.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:16:58.176915 taipy-rest-2.3.0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:16:58.176915 taipy-rest-2.3.0.dev1/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:16:58.176915 taipy-rest-2.3.0.dev1/src/taipy/rest/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:16:58.176915 taipy-rest-2.3.0.dev1/src/taipy/rest/api/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/error_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:16:58.176915 taipy-rest-2.3.0.dev1/src/taipy/rest/api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:16:58.176915 taipy-rest-2.3.0.dev1/src/taipy/rest/api/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/middlewares/_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:16:58.176915 taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    24795 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:16:58.180915 taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:16:58.180915 taipy-rest-2.3.0.dev1/src/taipy/rest/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/commons/apispec.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/commons/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/commons/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/commons/to_from_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/src/taipy/rest/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:16:58.180915 taipy-rest-2.3.0.dev1/src/taipy_rest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-05 16:16:58.000000 taipy-rest-2.3.0.dev1/src/taipy_rest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-05 16:16:58.000000 taipy-rest-2.3.0.dev1/src/taipy_rest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:16:58.000000 taipy-rest-2.3.0.dev1/src/taipy_rest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-05 16:16:58.000000 taipy-rest-2.3.0.dev1/src/taipy_rest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 16:16:58.000000 taipy-rest-2.3.0.dev1/src/taipy_rest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:16:58.180915 taipy-rest-2.3.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/tests/test_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/tests/test_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/tests/test_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/tests/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-05 16:16:46.000000 taipy-rest-2.3.0.dev1/tests/test_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:49:57.287670 taipy-rest-2.3.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-13 17:49:57.287670 taipy-rest-2.3.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:49:57.287670 taipy-rest-2.3.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-13 17:49:47.000000 taipy-rest-2.3.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:49:57.271669 taipy-rest-2.3.0.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:49:57.275669 taipy-rest-2.3.0.dev2/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:49:57.275669 taipy-rest-2.3.0.dev2/src/taipy/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:49:57.279669 taipy-rest-2.3.0.dev2/src/taipy/rest/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/error_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:49:57.279669 taipy-rest-2.3.0.dev2/src/taipy/rest/api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:49:57.279669 taipy-rest-2.3.0.dev2/src/taipy/rest/api/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/middlewares/_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:49:57.283670 taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24795 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:49:57.283670 taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:49:57.287670 taipy-rest-2.3.0.dev2/src/taipy/rest/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/commons/apispec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/commons/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/commons/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/commons/to_from_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/src/taipy/rest/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:49:57.287670 taipy-rest-2.3.0.dev2/src/taipy_rest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-13 17:49:57.000000 taipy-rest-2.3.0.dev2/src/taipy_rest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-13 17:49:57.000000 taipy-rest-2.3.0.dev2/src/taipy_rest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:49:57.000000 taipy-rest-2.3.0.dev2/src/taipy_rest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-13 17:49:57.000000 taipy-rest-2.3.0.dev2/src/taipy_rest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 17:49:57.000000 taipy-rest-2.3.0.dev2/src/taipy_rest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:49:57.287670 taipy-rest-2.3.0.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/tests/test_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/tests/test_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/tests/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-13 17:49:37.000000 taipy-rest-2.3.0.dev2/tests/test_task.py
```

### Comparing `taipy-rest-2.3.0.dev1/LICENSE` & `taipy-rest-2.3.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/PKG-INFO` & `taipy-rest-2.3.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-rest
-Version: 2.3.0.dev1
+Version: 2.3.0.dev2
 Summary: Library to expose taipy-core REST APIs.
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-rest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `taipy-rest-2.3.0.dev1/README.md` & `taipy-rest-2.3.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/setup.py` & `taipy-rest-2.3.0.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,10 +52,10 @@
         "flask-migrate>=3.1,<4.0",
         "flask-jwt-extended>=4.3,<5.0",
         "flask-marshmallow>=0.14,<0.15",
         "marshmallow-sqlalchemy>=0.25,<0.29",
         "passlib>=1.7.4,<1.8",
         "apispec[yaml]>=5.1,<6.0",
         "apispec-webframeworks>=0.5.2,<0.6",
-        "taipy-core>=2.3.0.dev0",
+        "taipy-core==2.3.0.dev3",
     ],
 )
```

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/__init__.py` & `taipy-rest-2.3.0.dev2/src/taipy/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,14 +47,15 @@
             get_latest_job,
             get_parents,
             get_pipelines,
             get_primary,
             get_primary_scenarios,
             get_scenarios,
             get_tasks,
+            is_deletable,
             set,
             set_primary,
             submit,
             subscribe_pipeline,
             subscribe_scenario,
             tag,
             unsubscribe_pipeline,
@@ -63,14 +64,19 @@
         )
         from taipy.core.task.task import Task
         from taipy.core.task.task_id import TaskId
 
     if find_spec("taipy.gui"):
         from taipy.gui import Gui
 
+        if find_spec("taipy.gui_core"):
+            from taipy.gui_core.GuiCoreLib import _GuiCore
+
+            Gui.add_library(_GuiCore())
+
         if find_spec("taipy.enterprise") and find_spec("taipy.enterprise.gui"):
             from taipy.enterprise.gui import _init_gui_enterprise
 
             _init_gui_enterprise(Gui)
 
     if find_spec("taipy.rest"):
         from taipy.rest import Rest
```

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/__init__.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/__init__.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/error_handler.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/error_handler.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/exceptions/__init__.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/exceptions/exceptions.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/middlewares/__init__.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/middlewares/_middleware.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/middlewares/_middleware.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/__init__.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/cycle.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/datanode.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/datanode.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/job.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/job.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/pipeline.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/pipeline.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/scenario.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/scenario.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/resources/task.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/resources/task.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/__init__.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/cycle.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/datanode.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/datanode.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/job.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/job.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/pipeline.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/pipeline.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/scenario.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/scenario.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/schemas/task.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/schemas/task.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/api/views.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/api/views.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/app.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/app.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/commons/__init__.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/commons/apispec.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/commons/apispec.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/commons/pagination.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/commons/pagination.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/commons/to_from_model.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/commons/to_from_model.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/extensions.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/extensions.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/rest.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/rest.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy/rest/version.py` & `taipy-rest-2.3.0.dev2/src/taipy/rest/version.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/src/taipy_rest.egg-info/PKG-INFO` & `taipy-rest-2.3.0.dev2/src/taipy_rest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-rest
-Version: 2.3.0.dev1
+Version: 2.3.0.dev2
 Summary: Library to expose taipy-core REST APIs.
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-rest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `taipy-rest-2.3.0.dev1/src/taipy_rest.egg-info/SOURCES.txt` & `taipy-rest-2.3.0.dev2/src/taipy_rest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/tests/test_cycle.py` & `taipy-rest-2.3.0.dev2/tests/test_cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/tests/test_datanode.py` & `taipy-rest-2.3.0.dev2/tests/test_datanode.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/tests/test_end_to_end.py` & `taipy-rest-2.3.0.dev2/tests/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/tests/test_job.py` & `taipy-rest-2.3.0.dev2/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/tests/test_middleware.py` & `taipy-rest-2.3.0.dev2/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/tests/test_pipeline.py` & `taipy-rest-2.3.0.dev2/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/tests/test_scenario.py` & `taipy-rest-2.3.0.dev2/tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `taipy-rest-2.3.0.dev1/tests/test_task.py` & `taipy-rest-2.3.0.dev2/tests/test_task.py`

 * *Files identical despite different names*

