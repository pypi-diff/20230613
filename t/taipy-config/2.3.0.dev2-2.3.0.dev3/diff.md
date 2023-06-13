# Comparing `tmp/taipy-config-2.3.0.dev2.tar.gz` & `tmp/taipy-config-2.3.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-config-2.3.0.dev2.tar", last modified: Thu Jun  8 19:22:56 2023, max compression
+gzip compressed data, was "taipy-config-2.3.0.dev3.tar", last modified: Tue Jun 13 17:24:10 2023, max compression
```

## Comparing `taipy-config-2.3.0.dev2.tar` & `taipy-config-2.3.0.dev3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.262503 taipy-config-2.3.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-08 19:22:56.262503 taipy-config-2.3.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:22:56.262503 taipy-config-2.3.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.254503 taipy-config-2.3.0.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.254503 taipy-config-2.3.0.dev2/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.254503 taipy-config-2.3.0.dev2/src/taipy/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.254503 taipy-config-2.3.0.dev2/src/taipy/_cli/_base_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/_cli/_base_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/_cli/_base_cli/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/_comparator_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/_config_comparator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/_serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_serializer/_base_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_serializer/_json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_serializer/_toml_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/checker/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/_auth_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/_global_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/issue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/issue_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/common/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/_classproperty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/_config_blocker.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/_template_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/_validate_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    35445 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/config.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/global_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/global_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/global_app/global_app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/section.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/unique_section.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.262503 taipy-config-2.3.0.dev2/src/taipy/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/logger/_taipy_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.262503 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-08 19:22:56.000000 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-08 19:22:56.000000 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:22:56.000000 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:22:49.000000 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 19:22:56.000000 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 19:22:56.000000 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.138005 taipy-config-2.3.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-13 17:24:10.138005 taipy-config-2.3.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:24:10.138005 taipy-config-2.3.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.130005 taipy-config-2.3.0.dev3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.130005 taipy-config-2.3.0.dev3/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.130005 taipy-config-2.3.0.dev3/src/taipy/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.130005 taipy-config-2.3.0.dev3/src/taipy/_cli/_base_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/_cli/_base_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/_cli/_base_cli/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.130005 taipy-config-2.3.0.dev3/src/taipy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.130005 taipy-config-2.3.0.dev3/src/taipy/config/_config_comparator/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/_config_comparator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/_config_comparator/_comparator_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/_config_comparator/_config_comparator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.134005 taipy-config-2.3.0.dev3/src/taipy/config/_serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/_serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/_serializer/_base_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/_serializer/_json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/_serializer/_toml_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.134005 taipy-config-2.3.0.dev3/src/taipy/config/checker/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/checker/_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.134005 taipy-config-2.3.0.dev3/src/taipy/config/checker/_checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/checker/_checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/checker/_checkers/_auth_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/checker/_checkers/_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/checker/_checkers/_global_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/checker/issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/checker/issue_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.134005 taipy-config-2.3.0.dev3/src/taipy/config/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/common/_classproperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/common/_config_blocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/common/_template_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/common/_validate_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/common/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/common/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42027 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/config.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.134005 taipy-config-2.3.0.dev3/src/taipy/config/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.134005 taipy-config-2.3.0.dev3/src/taipy/config/global_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/global_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/global_app/global_app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/unique_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.138005 taipy-config-2.3.0.dev3/src/taipy/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-13 17:23:56.000000 taipy-config-2.3.0.dev3/src/taipy/logger/_taipy_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:24:10.138005 taipy-config-2.3.0.dev3/src/taipy_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-13 17:24:10.000000 taipy-config-2.3.0.dev3/src/taipy_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-13 17:24:10.000000 taipy-config-2.3.0.dev3/src/taipy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:24:10.000000 taipy-config-2.3.0.dev3/src/taipy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:24:03.000000 taipy-config-2.3.0.dev3/src/taipy_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-13 17:24:10.000000 taipy-config-2.3.0.dev3/src/taipy_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 17:24:10.000000 taipy-config-2.3.0.dev3/src/taipy_config.egg-info/top_level.txt
```

### Comparing `taipy-config-2.3.0.dev2/LICENSE` & `taipy-config-2.3.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/PKG-INFO` & `taipy-config-2.3.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 2.3.0.dev2
+Version: 2.3.0.dev3
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-config-2.3.0.dev2/README.md` & `taipy-config-2.3.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/setup.py` & `taipy-config-2.3.0.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/__init__.py` & `taipy-config-2.3.0.dev3/src/taipy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,17 +65,17 @@
         from taipy.core.task.task import Task
         from taipy.core.task.task_id import TaskId
 
     if find_spec("taipy.gui"):
         from taipy.gui import Gui
 
         if find_spec("taipy.gui_core"):
-            from taipy.gui_core.GuiCoreLib import GuiCore
+            from taipy.gui_core.GuiCoreLib import _GuiCore
 
-            Gui.add_library(GuiCore())
+            Gui.add_library(_GuiCore())
 
         if find_spec("taipy.enterprise") and find_spec("taipy.enterprise.gui"):
             from taipy.enterprise.gui import _init_gui_enterprise
 
             _init_gui_enterprise(Gui)
 
     if find_spec("taipy.rest"):
```

### Comparing `taipy-config-2.3.0.dev2/src/taipy/_cli/__init__.py` & `taipy-config-2.3.0.dev3/src/taipy/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/_cli/_base_cli/__init__.py` & `taipy-config-2.3.0.dev3/src/taipy/_cli/_base_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/_cli/_base_cli/_cli.py` & `taipy-config-2.3.0.dev3/src/taipy/_cli/_base_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/__init__.py` & `taipy-config-2.3.0.dev3/src/taipy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/_config.py` & `taipy-config-2.3.0.dev3/src/taipy/config/_config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/__init__.py` & `taipy-config-2.3.0.dev3/src/taipy/config/_config_comparator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/_comparator_result.py` & `taipy-config-2.3.0.dev3/src/taipy/config/_config_comparator/_comparator_result.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/_config_comparator.py` & `taipy-config-2.3.0.dev3/src/taipy/config/_config_comparator/_config_comparator.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/_serializer/__init__.py` & `taipy-config-2.3.0.dev3/src/taipy/config/_serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/_serializer/_base_serializer.py` & `taipy-config-2.3.0.dev3/src/taipy/config/_serializer/_base_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/_serializer/_json_serializer.py` & `taipy-config-2.3.0.dev3/src/taipy/config/_serializer/_json_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/_serializer/_toml_serializer.py` & `taipy-config-2.3.0.dev3/src/taipy/config/_serializer/_toml_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/checker/__init__.py` & `taipy-config-2.3.0.dev3/src/taipy/config/checker/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/checker/_checker.py` & `taipy-config-2.3.0.dev3/src/taipy/config/checker/_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/__init__.py` & `taipy-config-2.3.0.dev3/src/taipy/config/checker/_checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/_auth_config_checker.py` & `taipy-config-2.3.0.dev3/src/taipy/config/checker/_checkers/_auth_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/_config_checker.py` & `taipy-config-2.3.0.dev3/src/taipy/config/checker/_checkers/_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/_global_config_checker.py` & `taipy-config-2.3.0.dev3/src/taipy/config/checker/_checkers/_global_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/checker/issue.py` & `taipy-config-2.3.0.dev3/src/taipy/config/checker/issue.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/checker/issue_collector.py` & `taipy-config-2.3.0.dev3/src/taipy/config/checker/issue_collector.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/common/__init__.py` & `taipy-config-2.3.0.dev3/src/taipy/config/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/common/_classproperty.py` & `taipy-config-2.3.0.dev3/src/taipy/config/common/_classproperty.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/common/_config_blocker.py` & `taipy-config-2.3.0.dev3/src/taipy/config/common/_config_blocker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/common/_repr_enum.py` & `taipy-config-2.3.0.dev3/src/taipy/config/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/common/_template_handler.py` & `taipy-config-2.3.0.dev3/src/taipy/config/common/_template_handler.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/common/_validate_id.py` & `taipy-config-2.3.0.dev3/src/taipy/config/common/_validate_id.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/common/frequency.py` & `taipy-config-2.3.0.dev3/src/taipy/config/common/frequency.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/common/scope.py` & `taipy-config-2.3.0.dev3/src/taipy/config/common/scope.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/config.py` & `taipy-config-2.3.0.dev3/src/taipy/config/config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/config.pyi` & `taipy-config-2.3.0.dev3/src/taipy/config/config.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -311,102 +311,131 @@
                 a single task configuration object is this pipeline holds a single task.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The default pipeline configuration.
         """
 
     @staticmethod
-    def configure_default_data_node(storage_type: str, scope: Optional[Scope] = None, **properties) -> "DataNodeConfig":
+    def configure_default_data_node(
+        storage_type: str, scope: Optional[Scope] = None, validity_period: Optional[timedelta] = None, **properties
+    ) -> "DataNodeConfig":
         """Configure the default values for data node configurations.
 
         This function creates the _default data node configuration_ object,
         where all data node configuration objects will find their default
         values when needed.
 
         Parameters:
             storage_type (str): The default storage type for all data node configurations.
                 The possible values are *"pickle"* (the default value), *"csv"*, *"excel"*,
                 *"sql"*, *"mongo_collection"*, *"in_memory"*, *"json"*, *"parquet"* or
                 *"generic"*.
             scope (Optional[Scope^]): The default scope for all data node configurations.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The default data node configuration.
         """
 
     @classmethod
     def configure_data_node(
-        cls, id: str, storage_type: Optional[str] = None, scope: Optional[Scope] = None, **properties
+        cls,
+        id: str,
+        storage_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
+        **properties,
     ) -> "DataNodeConfig":
         """Configure a new data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new data node configuration.
             storage_type (Optional[str]): The data node configuration storage type. The possible values
                 are None (which is the default value of *"pickle"*, unless it has been overloaded by the
                 *storage_type* value set in the default data node configuration
                 (see `(Config.)configure_default_data_node()^`)), *"pickle"*, *"csv"*, *"excel"*,
                 *"sql_table"*, *"sql"*, *"json"*, *"parquet"*, *"mongo_collection"*, *"in_memory"*, or
                 *"generic"*.
             scope (Optional[Scope^]): The scope of the data node configuration.<br/>
                 The default value is `Scope.SCENARIO` (or the one specified in
                 `(Config.)configure_default_data_node()^`).
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new data node configuration.
         """
 
     @classmethod
     def configure_csv_data_node(
         cls,
         id: str,
         default_path: Optional[str] = None,
         has_header: Optional[bool] = None,
         exposed_type: Optional[str] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new CSV data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new CSV data node configuration.
             default_path (Optional[str]): The default path of the CSV file.
             has_header (Optional[bool]): If True, indicates that the CSV file has a header.
             exposed_type (Optional[str]): The exposed type of the data read from CSV file.<br/>
                 The default value is `pandas`.
             scope (Optional[Scope^]): The scope of the CSV data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new CSV data node configuration.
         """
 
     @classmethod
     def configure_json_data_node(
         cls,
         id: str,
         default_path: Optional[str] = None,
         encoder: Optional[json.JSONEncoder] = None,
         decoder: Optional[json.JSONDecoder] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new JSON data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new JSON data node configuration.
             default_path (Optional[str]): The default path of the JSON file.
             encoder (Optional[json.JSONEncoder]): The JSON encoder used to write data into the JSON file.
             decoder (Optional[json.JSONDecoder]): The JSON decoder used to read data from the JSON file.
             scope (Optional[Scope^]): The scope of the JSON data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The new JSON data node configuration.
         """
 
     @classmethod
     def configure_parquet_data_node(
@@ -415,14 +444,15 @@
         default_path: Optional[str] = None,
         engine: Optional[str] = None,
         compression: Optional[str] = None,
         read_kwargs: Optional[Dict] = None,
         write_kwargs: Optional[Dict] = None,
         exposed_type: Optional[str] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new Parquet data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new Parquet data node configuration.
             default_path (Optional[str]): The default path of the Parquet file.
@@ -437,14 +467,19 @@
                 `pandas.DataFrame.write_parquet()` function.<br/>
                 The parameters in *read_kwargs* and *write_kwargs* have a **higher precedence** than the
                 top-level parameters which are also passed to Pandas.
             exposed_type (Optional[str]): The exposed type of the data read from Parquet file.<br/>
                 The default value is `pandas`.
             scope (Optional[Scope^]): The scope of the Parquet data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new Parquet data node configuration.
         """
 
     @classmethod
@@ -452,28 +487,34 @@
         cls,
         id: str,
         default_path: Optional[str] = None,
         has_header: Optional[bool] = None,
         sheet_name: Optional[Union[List[str], str]] = None,
         exposed_type: Optional[str] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new Excel data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new Excel data node configuration.
             default_path (Optional[str]): The path of the Excel file.
             has_header (Optional[bool]): If True, indicates that the Excel file has a header.
             sheet_name (Optional[Union[List[str], str]]): The list of sheet names to be used.
                 This can be a unique name.
             exposed_type (Optional[str]): The exposed type of the data read from Excel file.<br/>
                 The default value is `pandas`.
             scope (Optional[Scope^]): The scope of the Excel data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new Excel data node configuration.
         """
 
     @classmethod
@@ -481,14 +522,15 @@
         cls,
         id: str,
         read_fct: Optional[Callable] = None,
         write_fct: Optional[Callable] = None,
         read_fct_args: Optional[List] = None,
         write_fct_args: Optional[List] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new generic data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new generic data node configuration.
             read_fct (Optional[Callable]): The Python function called to read the data.
@@ -496,55 +538,76 @@
                 The provided function must have at least one parameter that receives the data to be written.
             read_fct_args (Optional[List]): The list of arguments that are passed to the function
                 *read_fct* to read data.
             write_fct_args (Optional[List]): The list of arguments that are passed to the function
                 *write_fct* to write the data.
             scope (Optional[Scope^]): The scope of the Generic data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The new Generic data node configuration.
         """
 
     @classmethod
     def configure_in_memory_data_node(
-        cls, id: str, default_data: Optional[Any] = None, scope: Optional[Scope] = None, **properties
+        cls,
+        id: str,
+        default_data: Optional[Any] = None,
+        scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
+        **properties,
     ) -> "DataNodeConfig":
         """Configure a new *in-memory* data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new in_memory data node configuration.
             default_data (Optional[any]): The default data of the data nodes instantiated from
                 this in_memory data node configuration.
             scope (Optional[Scope^]): The scope of the in_memory data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new *in-memory* data node configuration.
         """
 
     @classmethod
     def configure_pickle_data_node(
         cls,
         id: str,
         default_path: Optional[str] = None,
         default_data: Optional[Any] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new pickle data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new pickle data node configuration.
             default_path (Optional[str]): The path of the pickle file.
             default_data (Optional[any]): The default data of the data nodes instantiated from
                 this pickle data node configuration.
             scope (Optional[Scope^]): The scope of the pickle data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new pickle data node configuration.
         """
 
     @classmethod
@@ -560,14 +623,15 @@
         db_port: Optional[int] = None,
         db_driver: Optional[str] = None,
         sqlite_folder_path: Optional[str] = None,
         sqlite_file_extension: Optional[str] = None,
         db_extra_args: Optional[Dict[str, Any]] = None,
         exposed_type: Optional[str] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new SQL table data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new SQL data node configuration.
             db_name (str): The database name, or the name of the SQLite database file.
@@ -589,14 +653,19 @@
                 The default value is ".db".
             db_extra_args (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
                 into database connection string.
             exposed_type (Optional[str]): The exposed type of the data read from SQL table.<br/>
                 The default value is "pandas".
             scope (Optional[Scope^]): The scope of the SQL data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new SQL data node configuration.
         """
 
     @classmethod
@@ -613,14 +682,15 @@
         db_port: Optional[int] = None,
         db_driver: Optional[str] = None,
         sqlite_folder_path: Optional[str] = None,
         sqlite_file_extension: Optional[str] = None,
         db_extra_args: Optional[Dict[str, Any]] = None,
         exposed_type: Optional[str] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new SQL data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new SQL data node configuration.
             db_name (str): The database name, or the name of the SQLite database file.
@@ -644,14 +714,19 @@
                 The default value is ".db".
             db_extra_args (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
                 into database connection string.
             exposed_type (Optional[str]): The exposed type of the data read from SQL query.<br/>
                 The default value is "pandas".
             scope (Optional[Scope^]): The scope of the SQL data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The new SQL data node configuration.
         """
 
     @classmethod
     def configure_mongo_collection_data_node(
@@ -662,14 +737,15 @@
         custom_document: Optional[Any] = None,
         db_username: Optional[str] = None,
         db_password: Optional[str] = None,
         db_host: Optional[str] = None,
         db_port: Optional[int] = None,
         db_extra_args: Optional[Dict[str, Any]] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new Mongo collection data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new Mongo collection data node configuration.
             db_name (str): The database name.
@@ -685,14 +761,19 @@
                 The default value is "localhost".
             db_port (Optional[int]): The database port.<br/>
                 The default value is 27017.
             db_extra_args (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
                 into database connection string.
             scope (Optional[Scope^]): The scope of the Mongo collection data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new Mongo collection data node configuration.
         """
 
     @staticmethod
@@ -753,15 +834,18 @@
                 arguments.
         Returns:
             The default task configuration.
         """
 
     @staticmethod
     def configure_job_executions(
-        mode: str = None, nb_of_workers: Union[int, str] = None, max_nb_of_workers: Union[int, str] = None, **properties
+        mode: Optional[str] = None,
+        nb_of_workers: Optional[Union[int, str]] = None,
+        max_nb_of_workers: Optional[Union[int, str]] = None,
+        **properties
     ) -> "JobConfig":
         """Configure job execution.
 
         Parameters:
             mode (Optional[str]): The job execution mode.
                 Possible values are: *"standalone"* (the default value) or *"development"*.
             max_nb_of_workers (Optional[int, str]): Parameter used only in default *"standalone"* mode.
```

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/exceptions/__init__.py` & `taipy-config-2.3.0.dev3/src/taipy/config/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/exceptions/exceptions.py` & `taipy-config-2.3.0.dev3/src/taipy/config/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/global_app/global_app_config.py` & `taipy-config-2.3.0.dev3/src/taipy/config/global_app/global_app_config.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/section.py` & `taipy-config-2.3.0.dev3/src/taipy/config/section.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/config/unique_section.py` & `taipy-config-2.3.0.dev3/src/taipy/config/unique_section.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/logger/__init__.py` & `taipy-config-2.3.0.dev3/src/taipy/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy/logger/_taipy_logger.py` & `taipy-config-2.3.0.dev3/src/taipy/logger/_taipy_logger.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev2/src/taipy_config.egg-info/PKG-INFO` & `taipy-config-2.3.0.dev3/src/taipy_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 2.3.0.dev2
+Version: 2.3.0.dev3
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-config-2.3.0.dev2/src/taipy_config.egg-info/SOURCES.txt` & `taipy-config-2.3.0.dev3/src/taipy_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

