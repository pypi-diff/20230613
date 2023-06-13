# Comparing `tmp/resotolib-3.5.0.tar.gz` & `tmp/resotolib-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotolib-3.5.0.tar", last modified: Fri May 26 18:24:17 2023, max compression
+gzip compressed data, was "resotolib-3.5.1.tar", last modified: Fri Jun  2 14:53:31 2023, max compression
```

## Comparing `resotolib-3.5.0.tar` & `resotolib-3.5.1.tar`

### file list

```diff
@@ -1,108 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.649375 resotolib-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 18:21:38.000000 resotolib-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-26 18:24:17.649375 resotolib-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-26 18:21:38.000000 resotolib-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-26 18:21:38.000000 resotolib-3.5.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-26 18:21:38.000000 resotolib-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.641375 resotolib-3.5.0/resotolib/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.641375 resotolib-3.5.0/resotolib/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.641375 resotolib-3.5.0/resotolib/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/web/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/web/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/baseplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    41019 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)    17649 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.645375 resotolib-3.5.0/resotolib/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/custom_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/model_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/durations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.645375 resotolib-3.5.0/resotolib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)    26773 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/graph/graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/json_bender.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.645375 resotolib-3.5.0/resotolib/log/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    23264 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.645375 resotolib-3.5.0/resotolib/web/
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.645375 resotolib-3.5.0/resotolib/web/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/picnic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.641375 resotolib-3.5.0/resotolib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-26 18:24:17.000000 resotolib-3.5.0/resotolib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-26 18:24:17.000000 resotolib-3.5.0/resotolib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:17.000000 resotolib-3.5.0/resotolib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:17.000000 resotolib-3.5.0/resotolib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-26 18:24:17.000000 resotolib-3.5.0/resotolib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 18:24:17.000000 resotolib-3.5.0/resotolib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-26 18:24:17.649375 resotolib-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-26 18:21:38.000000 resotolib-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.649375 resotolib-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.649375 resotolib-3.5.0/test/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/asynchronous/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.649375 resotolib-3.5.0/test/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/asynchronous/web/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.649375 resotolib-3.5.0/test/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/core/custom_command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/core/model_check_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/core/model_export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/core/progress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/core/tasks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/durations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/json_bender_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/parse_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:31.578656 resotolib-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 14:49:29.000000 resotolib-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-02 14:53:31.578656 resotolib-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-02 14:49:29.000000 resotolib-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-02 14:49:29.000000 resotolib-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:31.570656 resotolib-3.5.1/resotolib/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:31.570656 resotolib-3.5.1/resotolib/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/asynchronous/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/asynchronous/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:31.570656 resotolib-3.5.1/resotolib/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/asynchronous/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/asynchronous/web/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/asynchronous/web/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/baseplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41003 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17649 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:31.574656 resotolib-3.5.1/resotolib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/core/ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/core/custom_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/core/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/core/model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/core/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/durations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:31.574656 resotolib-3.5.1/resotolib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    26637 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/graph/graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/json_bender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:31.574656 resotolib-3.5.1/resotolib/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23264 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:31.574656 resotolib-3.5.1/resotolib/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/web/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:31.574656 resotolib-3.5.1/resotolib/web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/web/static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/web/static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/web/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/web/static/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/web/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/web/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/web/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/web/static/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/web/static/picnic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/web/static/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-06-02 14:49:29.000000 resotolib-3.5.1/resotolib/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:31.570656 resotolib-3.5.1/resotolib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-02 14:53:31.000000 resotolib-3.5.1/resotolib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-02 14:53:31.000000 resotolib-3.5.1/resotolib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:53:31.000000 resotolib-3.5.1/resotolib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:50:18.000000 resotolib-3.5.1/resotolib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-02 14:53:31.000000 resotolib-3.5.1/resotolib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 14:53:31.000000 resotolib-3.5.1/resotolib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 14:53:31.578656 resotolib-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:31.578656 resotolib-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-02 14:49:29.000000 resotolib-3.5.1/test/test_x509.py
```

### Comparing `resotolib-3.5.0/PKG-INFO` & `resotolib-3.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto common library.
-Home-page: https://github.com/someengineering/resoto/tree/main/resotolib
-License: Apache 2.0
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotolib
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: test
 
 # `resotolib`
 Resoto common library
 
 
 ## Table of contents
```

### Comparing `resotolib-3.5.0/README.md` & `resotolib-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/args.py` & `resotolib-3.5.1/resotolib/args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/asynchronous/periodic.py` & `resotolib-3.5.1/resotolib/asynchronous/periodic.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/asynchronous/utils.py` & `resotolib-3.5.1/resotolib/asynchronous/utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/asynchronous/web/auth.py` & `resotolib-3.5.1/resotolib/asynchronous/web/auth.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/asynchronous/web/runner.py` & `resotolib-3.5.1/resotolib/asynchronous/web/runner.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/asynchronous/web/ws_handler.py` & `resotolib-3.5.1/resotolib/asynchronous/web/ws_handler.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/baseplugin.py` & `resotolib-3.5.1/resotolib/baseplugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 
     @staticmethod
     def pre_cleanup(config: Config, resource: BaseResource, graph: Graph) -> bool:
         return resource.pre_cleanup(graph)
 
     @staticmethod
     def cleanup(config: Config, resource: BaseResource, graph: Graph) -> bool:
-        return resource.cleanup(graph)  # type: ignore
+        return resource.cleanup(graph)
 
     def go(self) -> None:
         self.collect()
 
 
 class BasePostCollectPlugin(ABC):
     """A resoto Post Collect plugin is a thread that runs after collection is done.
```

### Comparing `resotolib-3.5.0/resotolib/baseresources.py` & `resotolib-3.5.1/resotolib/baseresources.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
             log.debug(f"Protecting resource {self.rtdname}")
             self.log("Protecting resource")
             self._changes.add("protected")
             self._protected = value
 
     # deprecated. future collectors plugins should be responsible for running pre_cleanup
     # and calling delete_resource on resources
-    @metrics_resource_cleanup.time()  # type: ignore
+    @metrics_resource_cleanup.time()
     @unless_protected
     def cleanup(self, graph: Optional[Any] = None) -> bool:
         if self.phantom:
             raise RuntimeError(f"Can't cleanup phantom resource {self.rtdname}")
 
         if self.cleaned:
             log.info(f"Resource {self.rtdname} has already been cleaned up")
```

### Comparing `resotolib-3.5.0/resotolib/config.py` & `resotolib-3.5.1/resotolib/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/core/__init__.py` & `resotolib-3.5.1/resotolib/core/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,31 @@
 import warnings
 from resotolib.logger import log
 from resotolib.args import ArgumentParser
 from urllib.parse import urlparse, ParseResult
 from typing import Optional
 
 
+class CLIEnvelope:
+    """
+    Envelope fields that are used by the CLI.
+    Those fields are encoded as HTTP Headers into the HTTP response.
+    """
+
+    # Defines the action that should be performed.
+    # Use cases:
+    # - "edit": A file that is returned from the core should be opened in an editor.
+    #           The result of the edit should be sent back to the core, identified by the "command" envelope field.
+    action = "Resoto-Shell-Action"
+    # Defines the command that should be executed after the edit was performed.
+    command = "Resoto-Shell-Command"
+    # Do not add this command to the shell history.
+    no_history = "Resoto-Shell-No-History"
+
+
 def add_args(arg_parser: ArgumentParser) -> None:
     arg_parser.add_argument(
         "--resotocore-uri",
         help="resotocore URI (default: https://localhost:8900)",
         default="https://localhost:8900",
         dest="resotocore_uri",
     )
```

### Comparing `resotolib-3.5.0/resotolib/core/actions.py` & `resotolib-3.5.1/resotolib/core/actions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/core/ca.py` & `resotolib-3.5.1/resotolib/core/ca.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/core/config.py` & `resotolib-3.5.1/resotolib/core/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/core/custom_command.py` & `resotolib-3.5.1/resotolib/core/custom_command.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/core/events.py` & `resotolib-3.5.1/resotolib/core/events.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/core/model_check.py` & `resotolib-3.5.1/resotolib/core/model_check.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/core/model_export.py` & `resotolib-3.5.1/resotolib/core/model_export.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/core/progress.py` & `resotolib-3.5.1/resotolib/core/progress.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/core/search.py` & `resotolib-3.5.1/resotolib/core/search.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/core/tasks.py` & `resotolib-3.5.1/resotolib/core/tasks.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/durations.py` & `resotolib-3.5.1/resotolib/durations.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/event.py` & `resotolib-3.5.1/resotolib/event.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/graph/__init__.py` & `resotolib-3.5.1/resotolib/graph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,15 +273,15 @@
                 edges_per_type[key.edge_type].append(edge)
         for edges in edges_per_type.values():
             typed_graph = self.edge_subgraph(edges)
             if not is_directed_acyclic_graph(typed_graph):
                 return [edge[2] for edge in networkx.algorithms.cycles.find_cycle(typed_graph)]
         return None
 
-    @metrics_graph_search.time()  # type: ignore
+    @metrics_graph_search.time()
     def search(self, attr: str, value: Any, regex_search: bool = False) -> Iterator[BaseResource]:
         """Search for graph nodes by their attribute value"""
         if value is None:
             log.debug(f"Not searching graph for nodes with attribute values {attr}: {value}")
             return ()
         log.debug((f"Searching graph for nodes with attribute values {attr}: {value}" f" (regex: {regex_search})"))
         for node in self.nodes():
@@ -292,48 +292,48 @@
                 and (
                     (regex_search is False and node_attr == value)
                     or (regex_search is True and re.search(value, str(node_attr)))
                 )
             ):
                 yield node
 
-    @metrics_graph_searchre.time()  # type: ignore
+    @metrics_graph_searchre.time()
     def searchre(self, attr: str, regex: str) -> Iterator[BaseResource]:
         """Regex search for graph nodes by their attribute value"""
         log.debug(f"Regex searching graph for nodes with attribute values {attr}: {regex}")
         yield from self.search(attr, regex, regex_search=True)
 
-    @metrics_graph_searchall.time()  # type: ignore
+    @metrics_graph_searchall.time()
     def searchall(self, match: Dict[str, Any]) -> Iterator[BaseResource]:
         """Search for graph nodes by multiple attributes and values"""
         for node in self.nodes():
             if all(getattr(node, attr, None) == value for attr, value in match.items()):
                 yield node
 
-    @metrics_graph_search_first.time()  # type: ignore
+    @metrics_graph_search_first.time()
     def search_first(self, attr: str, value: Any) -> Optional[BaseResource]:
         """Return the first graph node that matches a certain attribute value"""
         node = next(iter(self.search(attr, value)), None)
         if node:
             log.debug(f"Found node {node} with {attr}: {value}")
         else:
             log.debug(f"Found no node with {attr}: {value}")
-        return node  # type: ignore
+        return node  # type
 
-    @metrics_graph_search_first_all.time()  # type: ignore
+    @metrics_graph_search_first_all.time()
     def search_first_all(self, match: Dict[str, Any]) -> Optional[BaseResource]:
         """Return the first graph node that matches multiple attributes and values"""
         node = next(iter(self.searchall(match)), None)
         if node:
             log.debug(f"Found node {node} with {match}")
         else:
             log.debug(f"Found no node with {match}")
-        return node  # type: ignore
+        return node
 
-    @metrics_graph_search_first_parent_class.time()  # type: ignore
+    @metrics_graph_search_first_parent_class.time()
     def search_first_parent_class(self, node: BaseResource, cls: Type[T]) -> Optional[T]:
         """Return the first parent node matching a certain class
 
         This is being used to search up the graph and e.g. find the account that the
         graph node is a member of.
         """
         queue = deque(self.predecessors(node))
@@ -344,15 +344,15 @@
                 return current
             for n in self.predecessors(current):
                 if n not in already_checked:
                     already_checked.add(n)
                     queue.append(n)
         return None
 
-    @metrics_graph_resolve_deferred_connections.time()  # type: ignore
+    @metrics_graph_resolve_deferred_connections.time()
     def resolve_deferred_connections(self) -> None:
         log.debug("Resolving deferred graph connections")
         for node in self.nodes:
             if isinstance(node, BaseResource):
                 node.resolve_deferred_connections(self)
 
     def export_model(self, **kwargs: Any) -> List[Json]:
```

### Comparing `resotolib-3.5.0/resotolib/graph/graph_extensions.py` & `resotolib-3.5.1/resotolib/graph/graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/json.py` & `resotolib-3.5.1/resotolib/json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/json_bender.py` & `resotolib-3.5.1/resotolib/json_bender.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/jwt.py` & `resotolib-3.5.1/resotolib/jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/lock.py` & `resotolib-3.5.1/resotolib/lock.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/logger.py` & `resotolib-3.5.1/resotolib/logger.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/parse_util.py` & `resotolib-3.5.1/resotolib/parse_util.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/proc.py` & `resotolib-3.5.1/resotolib/proc.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/tree.py` & `resotolib-3.5.1/resotolib/tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/utils.py` & `resotolib-3.5.1/resotolib/utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/web/__init__.py` & `resotolib-3.5.1/resotolib/web/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/web/metrics.py` & `resotolib-3.5.1/resotolib/web/metrics.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/web/static/android-chrome-192x192.png` & `resotolib-3.5.1/resotolib/web/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/web/static/android-chrome-512x512.png` & `resotolib-3.5.1/resotolib/web/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/web/static/apple-touch-icon.png` & `resotolib-3.5.1/resotolib/web/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/web/static/favicon-16x16.png` & `resotolib-3.5.1/resotolib/web/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/web/static/favicon-32x32.png` & `resotolib-3.5.1/resotolib/web/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/web/static/index.html` & `resotolib-3.5.1/resotolib/web/static/index.html`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/web/static/mstile-150x150.png` & `resotolib-3.5.1/resotolib/web/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/web/static/picnic.min.css` & `resotolib-3.5.1/resotolib/web/static/picnic.min.css`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib/x509.py` & `resotolib-3.5.1/resotolib/x509.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/resotolib.egg-info/PKG-INFO` & `resotolib-3.5.1/resotolib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto common library.
-Home-page: https://github.com/someengineering/resoto/tree/main/resotolib
-License: Apache 2.0
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotolib
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: test
 
 # `resotolib`
 Resoto common library
 
 
 ## Table of contents
```

### Comparing `resotolib-3.5.0/resotolib.egg-info/SOURCES.txt` & `resotolib-3.5.1/resotolib.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 MANIFEST.in
 README.md
-requirements-test.txt
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 resotolib/__init__.py
 resotolib/args.py
 resotolib/baseplugin.py
 resotolib/baseresources.py
 resotolib/config.py
 resotolib/durations.py
 resotolib/event.py
@@ -59,35 +57,21 @@
 resotolib/web/static/browserconfig.xml
 resotolib/web/static/favicon-16x16.png
 resotolib/web/static/favicon-32x32.png
 resotolib/web/static/index.html
 resotolib/web/static/mstile-150x150.png
 resotolib/web/static/picnic.min.css
 resotolib/web/static/site.webmanifest
-test/__init__.py
-test/durations_test.py
-test/json_bender_test.py
-test/parse_util_test.py
 test/test_args.py
 test/test_baseresources.py
 test/test_ca.py
 test/test_config.py
 test/test_graph.py
 test/test_graph_extensions.py
 test/test_json.py
 test/test_jwt.py
 test/test_logging.py
 test/test_plugin.py
 test/test_tree.py
 test/test_utils.py
 test/test_web.py
-test/test_x509.py
-test/asynchronous/__init__.py
-test/asynchronous/test_utils.py
-test/asynchronous/web/__init__.py
-test/asynchronous/web/test_auth.py
-test/core/__init__.py
-test/core/custom_command_test.py
-test/core/model_check_test.py
-test/core/model_export_test.py
-test/core/progress_test.py
-test/core/tasks_test.py
+test/test_x509.py
```

### Comparing `resotolib-3.5.0/setup.py` & `resotolib-3.5.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,78 @@
-import os
-import resotolib
-import pkg_resources
-from setuptools import setup, find_packages
-
-
-def read(file_name: str) -> str:
-    with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
-        return of.read()
-
-
-setup(
-    name=resotolib.__title__,
-    version=resotolib.__version__,
-    description=resotolib.__description__,
-    license=resotolib.__license__,
-    packages=find_packages(),
-    package_data={"resotolib": ["py.typed"]},
-    long_description=read("README.md"),
-    long_description_content_type="text/markdown",
-    include_package_data=True,
-    zip_safe=False,
-    install_requires=[str(requirement) for requirement in pkg_resources.parse_requirements(read("requirements.txt"))],
-    setup_requires=["pytest-runner"],
-    tests_require=["pytest"],
-    classifiers=[
-        # Current project status
-        "Development Status :: 4 - Beta",
-        # Audience
-        "Intended Audience :: System Administrators",
-        "Intended Audience :: Information Technology",
-        # License information
-        "License :: OSI Approved :: Apache Software License",
-        # Supported python versions
-        "Programming Language :: Python :: 3.9",
-        # Supported OS's
-        "Operating System :: POSIX :: Linux",
-        "Operating System :: Unix",
-        # Extra metadata
-        "Environment :: Console",
-        "Natural Language :: English",
-        "Topic :: Security",
-        "Topic :: Utilities",
-    ],
-    keywords="cloud security",
-    url="https://github.com/someengineering/resoto/tree/main/resotolib",
-)
+[project]
+name = "resotolib"
+version = "3.5.1"
+authors = [{name="Some Engineering Inc."}]
+description = "Resoto common library."
+license = {file="LICENSE"}
+requires-python = ">=3.9"
+classifiers = [
+    # Current project status
+    "Development Status :: 4 - Beta",
+    # Audience
+    "Intended Audience :: System Administrators",
+    "Intended Audience :: Information Technology",
+    # License information
+    "License :: OSI Approved :: Apache Software License",
+    # Supported python versions
+    "Programming Language :: Python :: 3.9",
+    # Supported OS's
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: Unix",
+    # Extra metadata
+    "Environment :: Console",
+    "Natural Language :: English",
+    "Topic :: Security",
+    "Topic :: Utilities",
+]
+readme = {file="README.md", content-type="text/markdown"}
+keywords = ["cloud security"]
+
+dependencies = [
+    "CherryPy",
+    "Pint",
+    "PyJWT",
+    "PyYAML",
+    "aiohttp[speedups]",
+    "attrs",
+    "cattrs",
+    "cryptography",
+    "jsons",
+    "networkx",
+    "parsy",
+    "prometheus-client",
+    "psutil",
+    "requests",
+    "typeguard",
+    "tzdata",
+    "tzlocal",
+    "websocket-client",
+]
+
+[project.optional-dependencies]
+test = [
+    "black",
+    "coverage",
+    "flake8",
+    "hypothesis",
+    "mypy",
+    "pep8-naming",
+    "pylint",
+    "pytest",
+    "pytest-asyncio",
+    "pytest-cov",
+    "pytest-runner",
+    "tox",
+    "wheel",
+]
+
+[project.urls]
+Documentation = "https://resoto.com"
+Source = "https://github.com/someengineering/resoto/tree/main/resotolib"
+
+[tool.setuptools.package-data]
+resotolib = ["py.typed"]
+
+[build-system]
+requires = ["setuptools>=67.8.0", "wheel>=0.40.0", "build>=0.10.0"]
+build-backend = "setuptools.build_meta"
+
```

### Comparing `resotolib-3.5.0/test/test_args.py` & `resotolib-3.5.1/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/test/test_baseresources.py` & `resotolib-3.5.1/test/test_baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/test/test_config.py` & `resotolib-3.5.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/test/test_graph.py` & `resotolib-3.5.1/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/test/test_graph_extensions.py` & `resotolib-3.5.1/test/test_graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/test/test_json.py` & `resotolib-3.5.1/test/test_json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/test/test_jwt.py` & `resotolib-3.5.1/test/test_jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/test/test_plugin.py` & `resotolib-3.5.1/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/test/test_tree.py` & `resotolib-3.5.1/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/test/test_utils.py` & `resotolib-3.5.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/test/test_web.py` & `resotolib-3.5.1/test/test_web.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.5.0/test/test_x509.py` & `resotolib-3.5.1/test/test_x509.py`

 * *Files identical despite different names*

