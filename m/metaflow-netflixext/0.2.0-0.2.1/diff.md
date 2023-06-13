# Comparing `tmp/metaflow-netflixext-0.2.0.tar.gz` & `tmp/metaflow-netflixext-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-netflixext-0.2.0.tar", last modified: Tue Jun  6 20:47:03 2023, max compression
+gzip compressed data, was "metaflow-netflixext-0.2.1.tar", last modified: Tue Jun 13 17:44:56 2023, max compression
```

## Comparing `metaflow-netflixext-0.2.0.tar` & `metaflow-netflixext-0.2.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.308158 metaflow-netflixext-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-06 20:47:03.308158 metaflow-netflixext-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.300157 metaflow-netflixext-0.2.0/metaflow_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.300157 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/environment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35351 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/environment/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/generate_vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   176395 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    30240 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    49517 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
--rw-r--r--   0 runner    (1001) docker     (123)    37196 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
--rw-r--r--   0 runner    (1001) docker     (123)   113678 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    19164 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/environment_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.304158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/toplevel/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.300157 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.308158 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)    39124 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:47:03.308158 metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-06 20:47:03.000000 metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-06 20:47:03.000000 metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:47:03.000000 metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 20:47:03.000000 metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-06 20:47:03.000000 metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:47:03.308158 metaflow-netflixext-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-06 20:46:45.000000 metaflow-netflixext-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.829685 metaflow-netflixext-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-13 17:44:56.829685 metaflow-netflixext-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.821685 metaflow-netflixext-0.2.1/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35523 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/environment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/generate_vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181679 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9779 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40641 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50296 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37869 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   113678 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20971 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/environment_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/mfextinit_netflixext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/toplevel/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/toplevel/mfextinit_netflixext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/toplevel/netflixext_toplevel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.821685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.825685 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39124 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:44:56.829685 metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-06-13 17:44:56.000000 metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-13 17:44:56.000000 metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:44:56.000000 metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 17:44:56.000000 metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 17:44:56.000000 metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:44:56.829685 metaflow-netflixext-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-13 17:44:40.000000 metaflow-netflixext-0.2.1/setup.py
```

### Comparing `metaflow-netflixext-0.2.0/LICENSE` & `metaflow-netflixext-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/PKG-INFO` & `metaflow-netflixext-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 0.2.0
+Version: 0.2.1
 Summary: EXPERIMENTAL Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `metaflow-netflixext-0.2.0/README.md` & `metaflow-netflixext-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/environment/environment_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,14 +351,18 @@
         for env_id, resolved_env, _ in resolver.all_environments(
             include_builder_envs=True
         ):
             obj.conda.set_default_environment(resolved_env.env_id)
 
         cast(Conda, obj.conda).write_out_environments()
 
+        # We are going to be creating this new environment going forward (not the
+        # initial env we got)
+        _, env, _ = next(resolver.resolved_environments())
+
         delta_time = int(time.time() - start)
         obj.echo(" done in %d second%s." % (delta_time, plural_marker(delta_time)))
 
     name = name or "metaflowtmp_%s_%s" % (env.env_id.req_id, env.env_id.full_id)
 
     existing_env = obj.conda.created_environment(name)
     if existing_env:
```

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/cmd/environment/utils.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/cmd/environment/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/config/mfextinit_netflixext.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,23 @@
     "CONDA_PREFERRED_FORMAT",
     None,
     get_validate_choice_fn([".tar.bz2", ".conda"]),
 )
 
 CONDA_DEFAULT_PIP_SOURCE = from_conf("CONDA_DEFAULT_PIP_SOURCE", None)
 
+# Allows you to specify URLs that need to be authenticated (basically Conda or PIP
+# package sources). Metaflow will glean all the information it can from traditional
+# configuration sources (like pip.conf) but this allows you to specify additional URLs
+# for which authentication is required. A dictionary should be passed in (or a JSON
+# version of it in string form).
+# key: hostname that needs authentication
+# value: a tuple/list of username and password
+CONDA_SRCS_AUTH_INFO = from_conf("CONDA_SRCS_AUTH_INFO", {})
+
 CONDA_REMOTE_COMMANDS = ("batch", "kubernetes")
 
 def _validate_remote_latest(name, value):
     if not value:
         raise MetaflowException("%s must not be empty." % name)
     if value[0] == ":" and value not in (":none:", ":username:", ":any:"):
         raise MetaflowException(
```

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/generate_vendor.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/generate_vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     Tuple,
     Union,
     cast,
 )
 from shutil import which
 from urllib.parse import urlparse, unquote
 
+from requests.auth import AuthBase
+
 from metaflow.plugins.datastores.local_storage import LocalStorage
 from metaflow.datastore.datastore_storage import DataStoreStorage
 
 from metaflow.debug import debug
 from metaflow.exception import MetaflowException, MetaflowNotFound
 from metaflow.metaflow_config import (
     CONDA_DEPENDENCY_RESOLVER,
@@ -69,14 +71,15 @@
 
 from .utils import (
     CONDA_FORMATS,
     AliasType,
     CondaException,
     CondaStepException,
     arch_id,
+    auth_from_urls,
     change_pip_package_version,
     correct_splitext,
     get_conda_root,
     is_alias_mutable,
     merge_dep_dicts,
     parse_explicit_url_conda,
     parse_explicit_url_pip,
@@ -219,14 +222,44 @@
         if len(conda_packages) == 1:
             # This is a pip only mode
             env_type = EnvType.PIP_ONLY
         elif len(pip_packages) > 0:
             env_type = EnvType.MIXED
         return env_type
 
+    @property
+    def default_conda_channels(self) -> List[str]:
+        if not self._found_binaries:
+            self._find_conda_binary()
+        return list(self._info["channels"] or [])
+
+    @property
+    def default_pip_sources(self) -> List[str]:
+        # TODO: Maybe we also need to get this from poetry but that gets a bit tricky
+        # since we don't actually check for a poetry install and use the one within
+        # conda lock. This is, for now, used to get authentication values so we should
+        # be ok relying on the pip repo. We also provide a side mechanism to specify
+        # other authentication values so we don't need to worry too much here.
+        sources = []  # type: List[str]
+        if not self._found_binaries:
+            self._find_conda_binary()
+
+        if "pip" not in self._bins:
+            return sources
+
+        config_values = self._call_binary(["config", "list"], binary="pip").decode(
+            encoding="utf-8"
+        )
+        for line in config_values.splitlines():
+            key, value = line.split("=", 1)
+            _, key = key.split(".")
+            if key in ("index-url", "extra-index-url"):
+                sources.extend(value.splitlines())
+        return sources
+
     def resolve(
         self,
         using_steps: Sequence[str],
         deps: Sequence[TStr],
         sources: Sequence[TStr],
         extras: Sequence[TStr],
         architecture: str,
@@ -753,22 +786,23 @@
         )
 
         debug.conda_exec(
             "%s (type %s)%sfound locally (resolved %s)"
             % (env_alias, alias_type.value, " " if env_id else " not ", resolved_alias)
         )
 
-        if env_id:
-            return env_id
-
-        if not local_only and self._storage is not None:
-            env_id = self._remote_fetch_alias([(alias_type, resolved_alias)], arch)
-            if env_id:
-                return env_id[0]
-        return None
+        if (
+            not local_only
+            and self._storage is not None
+            and (env_id is None or is_alias_mutable(alias_type, resolved_alias))
+        ):
+            env_id_list = self._remote_fetch_alias([(alias_type, resolved_alias)], arch)
+            if env_id_list:
+                env_id = env_id_list[0]
+        return env_id
 
     def environment_from_alias(
         self, env_alias: str, arch: Optional[str] = None, local_only: bool = False
     ) -> Optional[ResolvedEnvironment]:
         """
         Convenience function allowing you to go from an alias to a ResolvedEnvironment
         directly
@@ -1003,16 +1037,22 @@
         # Here we take the resolved env (which has more information but maybe not
         # all if we request a different package format for example) if it exists or
         # the one we just resolved
         resolved_env = [
             cached_env if cached_env else env
             for cached_env, env in zip(cached_resolved_envs, resolved_envs)
         ]
-
+        all_sources = list(
+            chain(self.default_conda_channels, self.default_pip_sources)
+        )  # type: List[str]
         for resolved_env in resolved_envs:
+            # First check the sources so we can figure out any authentication that
+            # may be needed
+            all_sources.extend([s.value for s in resolved_env.sources])
+
             # We are now going to try to figure out all the locations we need to check
             # in the cache for the presence of the files we need
             env_id = resolved_env.env_id
             for req_pkg in resolved_env.packages:
                 if req_pkg.url in url_to_pkgs:
                     old_arch, all_pkgs = url_to_pkgs[req_pkg.url]
                     all_pkgs.append(req_pkg)
@@ -1137,14 +1177,15 @@
                     self._echo, search_dirs, self._package_dir_lockfile_name
                 ):
                     require_conda_format = cache_formats.get("conda", [])
                     if len(require_conda_format) > 0 and "_any" in require_conda_format:
                         require_conda_format = []
                     self._lazy_fetch_packages(
                         pkgs,
+                        auth_from_urls(all_sources),
                         dest_dir,
                         require_conda_format=require_conda_format,
                         require_url_format=True,
                         requested_arch=arch,
                         search_dirs=search_dirs,
                     )
             # Upload everything for all packages. We iterate over all packages in case
@@ -1263,14 +1304,15 @@
         return os.path.join(
             cast(str, CONDA_ENVS_DIRNAME), "aliases", alias_type.value, env_alias
         )
 
     def _lazy_fetch_packages(
         self,
         packages: Iterable[PackageSpecification],
+        auth_info: Optional[AuthBase],
         dest_dir: str,
         require_conda_format: Optional[Sequence[str]] = None,
         require_url_format: bool = False,
         requested_arch: str = arch_id(),
         search_dirs: Optional[List[str]] = None,
     ):
         # Lazily fetch all packages specified by the PackageSpecification
@@ -1337,15 +1379,16 @@
             base_hash = pkg_spec.base_hash()
             debug.conda_exec(
                 "%s -> download %s to %s"
                 % (pkg_spec.filename, pkg_spec.url, local_path)
             )
             try:
                 with open(local_path, "wb") as f:
-                    with session.get(pkg_spec.url, stream=True) as r:
+                    with session.get(pkg_spec.url, stream=True, auth=auth_info) as r:
+                        r.raise_for_status()
                         for chunk in r.iter_content(chunk_size=None):
                             base_hash.update(chunk)
                             f.write(chunk)
                 pkg_spec.add_local_file(
                     pkg_spec.url_format,
                     local_path,
                     pkg_hash=base_hash.hexdigest(),
@@ -1636,15 +1679,15 @@
                         )
                     else:
                         pending_errors.append(
                             "Internal error: trying to download a non-existent cache item for %s"
                             % pkg_spec.filename
                         )
                 with storage.load_bytes(keys_to_info.keys()) as load_results:  # type: ignore
-                    for (key, tmpfile, _) in load_results:  # type: ignore
+                    for key, tmpfile, _ in load_results:  # type: ignore
                         pkg_spec, pkg_format, pkg_hash, local_path = keys_to_info[key]  # type: ignore
                         if not tmpfile:
                             pending_errors.append(
                                 "Error downloading package from cache for '%s': not found at %s"
                                 % (pkg_spec.filename, key)
                             )
                         else:
@@ -1719,15 +1762,14 @@
             raise CondaException(
                 "Could not fetch packages -- see pretty-printed errors above."
             )
 
     def _resolve_env_with_micromamba_server(
         self, deps: Sequence[TStr], channels: Sequence[TStr], architecture: str
     ) -> List[PackageSpecification]:
-
         deps = [d for d in deps if d.category in ("conda", "npconda")]
 
         if not self._have_micromamba_server:
             raise CondaException(
                 "Micromamba server not supported by installed version of micromamba"
             )
 
@@ -1779,15 +1821,14 @@
         self,
         deps: Sequence[TStr],
         sources: Sequence[TStr],
         architecture: str,
         builder_env: Optional[ResolvedEnvironment],
         base_env: Optional[ResolvedEnvironment],
     ) -> Tuple[List[PackageSpecification], Optional[ResolvedEnvironment]]:
-
         if base_env:
             local_packages = [
                 p for p in base_env.packages if not p.is_downloadable_url()
             ]
             if local_packages:
                 raise CondaException(
                     "Local packages are not allowed in Conda: %s"
@@ -1902,15 +1943,14 @@
         deps: Sequence[TStr],
         sources: Sequence[TStr],
         extras: Sequence[TStr],
         architecture: str,
         builder_env: Optional[ResolvedEnvironment],
         base_env: Optional[ResolvedEnvironment],
     ) -> Tuple[List[PackageSpecification], Optional[ResolvedEnvironment]]:
-
         if base_env:
             local_packages = [
                 p
                 for p in base_env.packages
                 if p.TYPE == "pip" and (not p.is_downloadable_url() or p.is_derived())
             ]
         else:
@@ -1966,36 +2006,38 @@
                 "--dry-run",
                 "--target",
                 pip_dir,
                 "--report",
                 os.path.join(pip_dir, "out.json"),
             ]
             args.extend(extra_args)
+            all_sources = []  # type: List[str]
             if CONDA_DEFAULT_PIP_SOURCE:
                 args.extend(["-i", CONDA_DEFAULT_PIP_SOURCE])
+                all_sources.append(CONDA_DEFAULT_PIP_SOURCE)
             for c in chain(
                 (s.value for s in sources if s.category == "pip"),
             ):
                 args.extend(["--extra-index-url", c])
+                all_sources.append(c)
 
             supported_tags = pip_tags_from_arch(python_version, architecture)
 
             if architecture != arch_id():
-
                 implementations = []  # type: List[str]
                 abis = []  # type: List[str]
                 platforms = []  # type: List[str]
                 for tag in supported_tags:
                     implementations.append(tag.interpreter)
                     abis.append(tag.abi)
                     platforms.append(tag.platform)
                 implementations = [x.interpreter for x in supported_tags]
                 extra_args = (
                     "--only-binary=:all:",
-                    # This seems to overly constrain things so skipping for now
+                    # Seems to overly constrain stuff
                     # *(
                     #    chain.from_iterable(
                     #        product(["--implementation"], set(implementations))
                     #    )
                     # ),
                     *(chain.from_iterable(product(["--abi"], set(abis)))),
                     *(chain.from_iterable(product(["--platform"], set(platforms)))),
@@ -2003,17 +2045,49 @@
 
                 args.extend(extra_args)
 
             # If we have local packages, we download them to a directory and point
             # pip to it using the `--find-links` argument.
             local_packages_dict = {}  # type: Dict[str, PackageSpecification]
             if local_packages:
-                os.makedirs(os.path.join(pip_dir, "local_packages"))
+                # This is a bit convoluted but we try to avoid downloading packages
+                # that we already have but we also don't want to point pip to a directory
+                # full of packages that we may not want to use so we will create symlinks
+                # to packages we already have and download the others
+                base_local_pip_packages = os.path.join(self._package_dirs[0], "pip")
+                tmp_local_pip_packages = os.path.realpath(
+                    os.path.join(pip_dir, "local_packages", "pip")
+                )
+                os.makedirs(tmp_local_pip_packages)
+                new_local_packages = []  # type: List[PackageSpecification]
+                for p in local_packages:
+                    for fmt in PipPackageSpecification.allowed_formats():
+                        filename = "%s%s" % (p.filename, fmt)
+                        if os.path.isfile(
+                            os.path.join(base_local_pip_packages, filename)
+                        ):
+                            os.symlink(
+                                os.path.join(base_local_pip_packages, filename),
+                                os.path.join(tmp_local_pip_packages, filename),
+                            )
+                            local_packages_dict[
+                                os.path.join(tmp_local_pip_packages, filename)
+                            ] = p
+                            p.add_local_file(
+                                fmt,
+                                os.path.join(base_local_pip_packages, filename),
+                                replace=True,
+                            )
+                            break
+                    else:
+                        new_local_packages.append(p)
+                local_packages = new_local_packages
+                # This will not fetch on the web so no need for auth object
                 self._lazy_fetch_packages(
-                    local_packages, os.path.join(pip_dir, "local_packages")
+                    local_packages, None, os.path.join(pip_dir, "local_packages")
                 )
                 args.extend(
                     ["--find-links", os.path.join(pip_dir, "local_packages", "pip")]
                 )
 
                 for p in local_packages:
                     for _, f in p.local_files:
@@ -2073,26 +2147,36 @@
                         raise CondaException(
                             "Cannot include an editable PIP package: '%s'" % url
                         )
                     if os.path.isdir(local_path):
                         packages_to_build.append(dl_info)
                     else:
                         # A local wheel or tarball
-                        if url in local_packages_dict:
-                            debug.conda_exec("This is a known local package")
+                        if local_path in local_packages_dict:
                             # We are going to move this file to a less "temporary"
                             # location so that it can be installed if needed
+
                             pkg_spec = local_packages_dict[local_path]
-                            filename = os.path.split(local_path)[1]
-                            file_format = correct_splitext(filename)[1]
-                            shutil.move(local_path, self._package_dirs[0])
-                            pkg_spec.add_local_file(
-                                file_format,
-                                os.path.join(self._package_dirs[0], filename),
-                            )
+                            if not os.path.islink(local_path):
+                                debug.conda_exec("Known package -- moving in place")
+                                filename = os.path.split(local_path)[1]
+                                file_format = correct_splitext(filename)[1]
+                                shutil.move(
+                                    local_path,
+                                    os.path.join(self._package_dirs[0], "pip"),
+                                )
+                                pkg_spec.add_local_file(
+                                    file_format,
+                                    os.path.join(
+                                        self._package_dirs[0], "pip", filename
+                                    ),
+                                    replace=True,
+                                )
+                            else:
+                                debug.conda_exec("Known package already in place")
                             result.append(pkg_spec)
                         else:
                             parse_result = parse_explicit_path_pip(url)
                             if parse_result.url_format != ".whl":
                                 # This is a source package so we need to build it
                                 packages_to_build.append(dl_info)
                             else:
@@ -2274,14 +2358,15 @@
                     built_pip_packages, builder_env = self._build_pip_packages(
                         python_version,
                         to_build_pkg_info,
                         builder_env,
                         pip_dir,
                         architecture,
                         supported_tags,
+                        all_sources,
                     )
                     result.extend(built_pip_packages)
                 else:
                     non_relocatable_packages = [
                         k for k, v in to_build_pkg_info.items() if not v["url"]
                     ]
                     if non_relocatable_packages:
@@ -2633,14 +2718,15 @@
                         built_pip_packages, builder_env = self._build_pip_packages(
                             python_version,
                             packages_to_build,
                             builder_env,
                             build_dir,
                             architecture,
                             supported_tags,
+                            pip_channels,
                         )
                         result.extend(built_pip_packages)
                     else:
                         # Here it was just URLs so we are good
                         result.extend(
                             [
                                 cast(PackageSpecification, v["spec"])
@@ -2663,15 +2749,14 @@
                     "if p.startswith('metaflow_inserted%s_')]; " % salt
                 )
                 _poetry_exec(python_cmd)
 
     def _build_builder_env(
         self, deps: Sequence[TStr], sources: Sequence[TStr], architecture: str
     ) -> ResolvedEnvironment:
-
         python_dep = [
             d for d in deps if d.category == "conda" and d.value.startswith("python==")
         ]
         conda_only_sources = [s for s in sources if s.category == "conda"]
 
         if arch_id() == architecture:
             conda_only_deps = [d for d in deps if d.category == "npconda"] + python_dep
@@ -2707,16 +2792,16 @@
         self,
         python_version: str,
         to_build_pkg_info: Dict[str, Any],
         builder_env: Optional[ResolvedEnvironment],
         build_dir: str,
         architecture: str,
         supported_tags: List[Tag],
+        pip_sources: List[str],
     ) -> Tuple[List[PackageSpecification], Optional[ResolvedEnvironment]]:
-
         # We check in the cache -- we don't actually have the filename or
         # hash so we check things starting with the partial URL.
         # The URL in cache will be:
         #  - <base url>/<filename>/<hash>/<filename>
 
         debug.conda_exec(
             "Checking for pre-built packages: %s"
@@ -2886,15 +2971,18 @@
             )
         )
         debug.conda_exec(
             "Going to fetch sources for %s"
             % ", ".join([p.filename for p in pkgs_to_fetch])
         )
         if pkgs_to_fetch:
-            self._lazy_fetch_packages(pkgs_to_fetch, target_directory)
+            pip_sources.extend(self.default_pip_sources)
+            self._lazy_fetch_packages(
+                pkgs_to_fetch, auth_from_urls(pip_sources), target_directory
+            )
 
         def _build_with_pip(
             identifier: int, key: str, spec: PipPackageSpecification, build_url: str
         ):
             dest_path = os.path.join(build_dir, "build_%d" % identifier)
             src = spec.local_file(spec.url_format) or build_url
             debug.conda_exec("%s: building from '%s' in '%s'" % (key, src, dest_path))
@@ -3118,15 +3206,23 @@
             self._bins["micromamba"] = self._bins["conda"]
             self._conda_executable_type = "micromamba"
 
     def _install_remote_conda(self):
         from metaflow.plugins import DATASTORES
 
         # We download the installer and return a path to it
-        final_path = os.path.join(os.getcwd(), "__conda_installer")
+        # To be clean, we try to be in the parent of our current directory to avoid
+        # polluting the user code. If that is not possible though, we create something
+        # inside the current directory
+        parent_dir = os.path.dirname(os.getcwd())
+        if os.access(parent_dir, os.W_OK):
+            final_path = os.path.join(parent_dir, "conda_env", "__conda_installer")
+        else:
+            final_path = os.path.join(os.getcwd(), "conda_env", "__conda_installer")
+        os.makedirs(os.path.dirname(final_path))
 
         path_to_fetch = os.path.join(
             CONDA_REMOTE_INSTALLER_DIRNAME,
             CONDA_REMOTE_INSTALLER.format(arch=arch_id()),
         )
         storage_opts = [d for d in DATASTORES if d.TYPE == self._datastore_type]
         if len(storage_opts) == 0:
@@ -3156,15 +3252,14 @@
             | stat.S_IROTH
             | stat.S_IXOTH,
         )
         self._bins = {"conda": final_path, "micromamba": final_path}
         self._conda_executable_type = "micromamba"
 
     def _validate_conda_installation(self) -> Optional[Exception]:
-
         # If this is installed in CONDA_LOCAL_PATH look for special marker
         if self._mode == "local" and CONDA_LOCAL_PATH is not None:
             if not os.path.isfile(
                 os.path.join(CONDA_LOCAL_PATH, ".metaflow-local-env")
             ):
                 return InvalidEnvironmentException(
                     "Missing special marker .metaflow-local-env in locally installed environment"
@@ -3227,15 +3322,15 @@
                     "is required) --ignoring"
                 )
                 del self._bins["conda-lock"]
         if "pip" in self._bins:
             pip_version = self._call_binary(["--version"], binary="pip").split(b" ", 2)[
                 1
             ]
-            # 22.3 has PEP 658 support which is a bit performance boost
+            # 22.3 has PEP 658 support which can be a big performance boost
             if LooseVersion(pip_version.decode("utf-8")) < LooseVersion("22.3"):
                 self._echo(
                     "pip is installed but not recent enough (22.3 or later is required) "
                     "-- ignoring"
                 )
                 del self._bins["pip"]
 
@@ -3474,15 +3569,14 @@
                     if cur_dir == "/":
                         break
                     cur_dir = os.path.dirname(cur_dir)
 
         return self._cached_info
 
     def _create(self, env: ResolvedEnvironment, env_name: str) -> None:
-
         # We first check to see if the environment exists -- if it does, we skip it
         env_dir = os.path.join(self._root_env_dir, env_name)
 
         self._cached_info = None
 
         if os.path.isdir(env_dir):
             possible_env_id = self._is_valid_env(env_dir)
@@ -3507,15 +3601,26 @@
                             possible_env_id.full_id,
                         )
                     )
                 self._remove(env_name)
 
         # We first get all the packages needed
         self._lazy_fetch_packages(
-            env.packages, self._package_dirs[0], search_dirs=self._package_dirs
+            env.packages,
+            auth_from_urls(
+                list(
+                    chain(
+                        [s.value for s in env.sources],
+                        self.default_conda_channels,
+                        self.default_pip_sources,
+                    )
+                )
+            ),
+            self._package_dirs[0],
+            search_dirs=self._package_dirs,
         )
 
         # We build the list of explicit URLs to pass to conda to create the environment
         # We know here that we have all the packages present one way or another, we just
         # need to format the URLs appropriately.
         explicit_urls = []  # type: List[str]
         pip_paths = []  # type: List[str]
```

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,28 @@
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Set,
     Tuple,
+    Union,
     cast,
 )
 
 from metaflow.plugins.datastores.local_storage import LocalStorage
 from metaflow.flowspec import FlowSpec
 
-from metaflow.metaflow_config import (
-    CONDA_MAGIC_FILE_V2,
-)
+from metaflow.exception import MetaflowException
+
+from metaflow.metaflow_config import CONDA_MAGIC_FILE_V2
 
 from metaflow.metaflow_environment import MetaflowEnvironment
 
+
 from .envsresolver import EnvsResolver
 from .utils import get_conda_manifest_path
 
 from .env_descr import CachedEnvironmentInfo, EnvID, ResolvedEnvironment
 from .conda import Conda
 from .conda_step_decorator import get_conda_decorator
 
@@ -67,15 +69,15 @@
         self._conda = cast(Conda, self._conda)
         resolver = EnvsResolver(self._conda)
 
         for step in self._flow:
             # Figure out the environments that we need to resolve for all steps
             # We will resolve all unique environments in parallel
             step_conda_dec = get_conda_decorator(self._flow, step.name)
-            if step_conda_dec.is_enabled():
+            if step_conda_dec.is_enabled() and not step_conda_dec.is_fetch_at_exec():
                 resolver.add_environment_for_step(step.name, step_conda_dec)
 
         resolver.resolve_environments(echo)
 
         update_envs = []  # type: List[ResolvedEnvironment]
         if self._datastore_type != "local":
             # We may need to update caches
@@ -116,53 +118,70 @@
         return self.base_env.validate_environment(echo, datastore_type)
 
     def decospecs(self) -> Tuple[str, ...]:
         # Apply conda and pip decorator and base environment's decorators to all steps.
         # We will later resolve which to keep.
         return ("conda", "pip") + self.base_env.decospecs()
 
-    def _get_env_id(self, step_name: str) -> Optional[EnvID]:
+    def _get_env_id(self, step_name: str) -> Optional[Union[str, EnvID]]:
         conda_decorator = get_conda_decorator(self._flow, step_name)
         if conda_decorator.is_enabled():
-            resolved_env = cast(Conda, self._conda).environment(conda_decorator.env_id)
-            if resolved_env:
-                return resolved_env.env_id
+            if not conda_decorator.is_fetch_at_exec():
+                resolved_env = cast(Conda, self._conda).environment(
+                    conda_decorator.env_id
+                )
+                if resolved_env:
+                    return resolved_env.env_id
+                else:
+                    raise MetaflowException(
+                        "Cannot find environment for step '%s'" % step_name
+                    )
+            else:
+                resolved_env_id = os.environ.get("_METAFLOW_CONDA_ENV")
+                if resolved_env_id:
+                    return EnvID(*json.loads(resolved_env_id))
+                # Here we will return the name of the environment
+                return conda_decorator.from_env_name_unresolved
         return None
 
     def _get_executable(self, step_name: str) -> Optional[str]:
         env_id = self._get_env_id(step_name)
         if env_id is not None:
             # The create method in Conda() sets up this symlink when creating the
             # environment.
             return os.path.join(".", "__conda_python")
         return None
 
     def bootstrap_commands(self, step_name: str, datastore_type: str) -> List[str]:
         # Bootstrap conda and execution environment for step
         env_id = self._get_env_id(step_name)
         if env_id is not None:
+            if isinstance(env_id, EnvID):
+                arg1 = env_id.req_id
+                arg2 = env_id.full_id
+            else:
+                arg1 = env_id
+                arg2 = "_fetch_exec"
             return [
                 "export CONDA_START=$(date +%s)",
                 "echo 'Bootstrapping environment ...'",
                 'python -m %s.remote_bootstrap "%s" "%s" %s %s %s'
                 % (
                     "metaflow_extensions.netflix_ext.plugins.conda",
                     self._flow.name,
                     step_name,
-                    env_id.req_id,
-                    env_id.full_id,
+                    arg1,
+                    arg2,
                     datastore_type,
                 ),
-                "export _METAFLOW_CONDA_ENV='%s'"
-                % json.dumps(env_id).replace('"', '\\"'),
+                "export _METAFLOW_CONDA_ENV=$(cat _env_id)",
                 "export PYTHONPATH=$(pwd)/_escape_trampolines:$(printenv PYTHONPATH)",
                 "echo 'Environment bootstrapped.'",
                 "export CONDA_END=$(date +%s)",
             ]
-            # TODO: Add the PATH part (need conda directory)
         return []
 
     def add_to_package(self) -> List[Tuple[str, str]]:
         # TODO: Improve this to only extract the environments that we care about
         # The issue is that we need to pass a path which is a bit annoying since
         # we then can't clean it up easily.
         files = self.base_env.add_to_package()
```

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_flow_decorator.py`

 * *Files 21% similar despite different names*

```diff
@@ -29,27 +29,35 @@
     pip_packages : Optional[Dict[str, str]]
         Same as libraries but for pip packages.
     pip_sources : Optional[List[str]]
         Same as channels but for pip sources.
     python : Optional[str]
         Version of Python to use, e.g. '3.7.4'. If not specified, the current Python
         version will be used.
+    fetch_at_exec : bool, default False
+        If set to True, the environment will be fetched when the task is
+        executing as opposed to at the beginning of the flow (or at deploy time if
+        deploying to a scheduler). This option requires name or pathspec to be
+        specified. This is useful, for example, if you want this step to always use
+        the latest named environment when it runs as opposed to the latest when it
+        is deployed.
     disabled : bool, default False
         If set to True, disables Conda
     """
 
     name = "conda_base"
     defaults = {
         "name": None,
         "pathspec": None,
         "libraries": {},
         "channels": [],
         "pip_packages": {},
         "pip_sources": [],
         "python": None,
+        "fetch_at_exec": None,
         "disabled": None,
     }
 
     def flow_init(
         self, flow, graph, environment, flow_datastore, metadata, logger, echo, options
     ):
         if "pip_base" in flow._flow_decorators:
@@ -98,26 +106,34 @@
         be specified either as a specific version or as a comma separated string
         of constraints like "<2.0,>=1.5".
     sources : Optional[List[str]]
         Additional channels to search for
     python : Optional[str]
         Version of Python to use, e.g. '3.7.4'. If not specified, the current version
         will be used.
+    fetch_at_exec : bool, default False
+        If set to True, the environment will be fetched when the task is
+        executing as opposed to at the beginning of the flow (or at deploy time if
+        deploying to a scheduler). This option requires name or pathspec to be
+        specified. This is useful, for example, if you want this step to always use
+        the latest named environment when it runs as opposed to the latest when it
+        is deployed.
     disabled : bool, default False
         If set to True, disables Pip
     """
 
     name = "pip_base"
 
     defaults = {
         "name": None,
         "pathspec": None,
         "packages": {},
         "sources": [],
         "python": None,
+        "fetch_at_exec": None,
         "disabled": None,
     }
 
     def flow_init(
         self, flow, graph, environment, flow_datastore, metadata, logger, echo, options
     ):
         if "conda_base" in flow._flow_decorators:
```

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_lock_micromamba_server.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/conda_step_decorator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pyright: strict, reportTypeCommentUsage=false, reportMissingTypeStubs=false
 
 import importlib
 import json
 import os
 import platform
+import re
 import shutil
 import sys
 import tempfile
 
 from itertools import chain
 
 from typing import (
@@ -15,14 +16,15 @@
     Callable,
     Dict,
     List,
     Optional,
     Sequence,
     Set,
     Tuple,
+    Union,
     cast,
 )
 
 from metaflow.plugins.datastores.local_storage import LocalStorage
 from metaflow.datastore.flow_datastore import FlowDataStore
 from metaflow.datastore.task_datastore import TaskDataStore
 from metaflow.debug import debug
@@ -70,65 +72,90 @@
     will prevail.
 
     Parameters
     ----------
     name : Optional[str]
         If specified, can refer to a named environment. The environment referred to
         here will be the one used for this step. If specified, nothing else can be
-        specified in this decorator
+        specified in this decorator. In the name, you can use `@{}` values and
+        environment variables will be used to substitute.
     pathspec : Optional[str]
         If specified, can refer to the pathspec of an existing step. The environment
         of this referred step will be used here. If specified, nothing else can be
-        specified in this decorator.
+        specified in this decorator. In the pathspec, you can use `@{}` values and
+        environment variables will be used to substitute.
     libraries : Optional[Dict[str, str]]
         Libraries to use for this step. The key is the name of the package
         and the value is the version to use (default: `{}`). Note that versions can
         be specified either as a specific version or as a comma separated string
         of constraints like "<2.0,>=1.5".
     channels : Optional[List[str]]
         Additional channels to search
     pip_packages : Optional[Dict[str, str]]
         Same as libraries but for pip packages
     pip_sources : Optional[List[str]]
         Same as channels but for pip sources
     python : Optional[str]
         Version of Python to use, e.g. '3.7.4'. If not specified, the current version
         will be used.
+    fetch_at_exec : bool, default False
+        If set to True, the environment will be fetched when the task is
+        executing as opposed to at the beginning of the flow (or at deploy time if
+        deploying to a scheduler). This option requires name or pathspec to be
+        specified. This is useful, for example, if you want this step to always use
+        the latest named environment when it runs as opposed to the latest when it
+        is deployed.
     disabled : bool, default False
         If set to True, disables Conda.
     """
 
     name = "conda"
+    TYPE = "conda"
+
     defaults = {
         "name": None,
         "pathspec": None,
         "libraries": {},
         "channels": [],
         "pip_packages": {},
         "pip_sources": [],
         "python": None,
+        "fetch_at_exec": None,
         "disabled": None,
     }  # type: Dict[str, Any]
 
     conda = None  # type: Optional[Conda]
     _local_root = None  # type: Optional[str]
 
     def is_enabled(self, ubf_context: Optional[str] = None) -> bool:
         if ubf_context == UBF_CONTROL:
             return False
         return not next(
             x
             for x in [
-                self.attributes["disabled"],
+                self._self_disabled(),
                 self._base_attributes["disabled"],
                 False,
             ]
             if x is not None
         )
 
+    def is_fetch_at_exec(self, ubf_context: Optional[str] = None) -> bool:
+        if ubf_context == UBF_CONTROL:
+            return False
+        return next(
+            x
+            for x in [
+                self.attributes["fetch_at_exec"],
+                self._base_attributes["fetch_at_exec"],
+                False,
+            ]
+            if x is not None
+        )
+
     @property
     def env_ids(self) -> List[EnvID]:
         # Note this returns a list because initially we had support to specify
         # architectures in the decorator -- keeping for now as this is still valid code
         debug.conda_exec(
             "Requested for step %s: deps: %s; sources: %s"
             % (self._step_name, str(self.step_deps), str(self.source_deps))
@@ -187,14 +214,18 @@
         return self._local_root
 
     @property
     def from_env_name(self) -> Optional[str]:
         return self._from()
 
     @property
+    def from_env_name_unresolved(self) -> Optional[str]:
+        return self._from(True)
+
+    @property
     def from_env(self) -> Optional[ResolvedEnvironment]:
         from_alias = self._from()
         if from_alias is not None:
             if self._from_env:
                 return self._from_env
             # Else, we need to resolve it
             self._get_conda(self._echo, self._flow_datastore_type)
@@ -212,14 +243,35 @@
                     % (from_alias, self._arch)
                 )
         return self._from_env
 
     def set_conda(self, conda: Conda):
         self.conda = conda
 
+    @staticmethod
+    def sub_envvars_in_envname(
+        name: str, addl_env: Optional[Dict[str, Union[str, Callable[[], str]]]] = None
+    ) -> str:
+        init_name = name
+        if addl_env is None:
+            addl_env = {}
+        envvars_to_sub = re.findall(r"\@{(\w+)}", name)
+        for envvar in set(envvars_to_sub):
+            replacement = os.environ.get(envvar, addl_env.get(envvar))
+            if callable(replacement):
+                replacement = replacement()
+            if replacement is not None:
+                name = name.replace("@{%s}" % envvar, replacement)
+            else:
+                raise InvalidEnvironmentException(
+                    "Could not find '%s' in the environment -- needed to resolve '%s'"
+                    % (envvar, name)
+                )
+        return name
+
     def step_init(
         self,
         flow: FlowSpec,
         graph: FlowGraph,
         step_name: str,
         decorators: List[StepDecorator],
         environment: MetaflowEnvironment,
@@ -234,14 +286,15 @@
         if not self._resolve_pip_or_conda_deco(flow, decorators):
             return
         self._echo = logger
         self._env = environment
         self._flow = flow
         self._step_name = step_name
         self._flow_datastore_type = flow_datastore.TYPE  # type: str
+        self._flow_datastore = flow_datastore
         self._base_attributes = self._get_base_attributes()
 
         self._is_remote = any(
             [deco.name in CONDA_REMOTE_COMMANDS for deco in decorators]
         )
         if self._is_remote:
             self._arch = "linux-64"
@@ -255,27 +308,55 @@
         # Information about the environment this environment is built from
         self._from_env = None  # type: Optional[ResolvedEnvironment]
         self._resolved_non_base_deps = None  # type: Optional[Sequence[TStr]]
         self._resolved_non_base_sources = None  # type: Optional[Sequence[TStr]]
         self._resolved_deps = None  # type: Optional[Sequence[TStr]]
         self._resolved_sources = None  # type: Optional[Sequence[TStr]]
         self._env_type = None  # type: Optional[EnvType]
+        self._env_for_fetch = {}  # type: Dict[str, Union[str, Callable[[], str]]]
+        self._flow = None  # type: Optional[FlowSpec]
 
-        if (self.attributes["name"] or self.attributes["pathspec"]) and len(
+        if (self.attributes["name"] or self.attributes["pathspec"]) and any(
             [
-                k
+                True
                 for k, v in self.attributes.items()
-                if v and k not in ("name", "pathspec")
+                if v and k not in ("name", "pathspec", "fetch_at_exec")
             ]
         ):
             raise InvalidEnvironmentException(
                 "You cannot specify `name` or `pathspec` along with other attributes in @%s"
                 % self.name
             )
 
+        if self.is_fetch_at_exec():
+            if not self._from(raw_name=True):
+                raise InvalidEnvironmentException(
+                    "You cannot specify a `fetch_at_exec` environment and no environment "
+                    "to fetch (either through `name` or `pathspec`) in @%s" % self.name
+                )
+            # We are also very strict that the environment should be *only* a name
+            # and nothing else as we won't re-resolve
+            if any(
+                [
+                    True
+                    for k, v in self.attributes.items()
+                    if v and k not in ("name", "pathspec", "fetch_at_exec")
+                ]
+            ) or any(
+                [
+                    True
+                    for k, v in self._base_attributes.items()
+                    if v and k not in ("name", "pathspec", "fetch_at_exec")
+                ]
+            ):
+                raise InvalidEnvironmentException(
+                    "You cannot specify a `fetch_at_exec` environment with anything "
+                    "other than a pure named environment in @%s" % self.name
+                )
+
         os.environ["PYTHONNOUSERSITE"] = "1"
 
     def runtime_init(self, flow: FlowSpec, graph: FlowGraph, package: Any, run_id: str):
         # Create a symlink to installed version of metaflow to execute user code against
         path_to_metaflow = os.path.join(get_metaflow_root(), "metaflow")
         path_to_info = os.path.join(get_metaflow_root(), "INFO")
         self._metaflow_home = tempfile.mkdtemp(dir="/tmp")
@@ -330,40 +411,86 @@
                     os.symlink(p, os.path.join(temp_dir, EXT_PKG))
                     self._addl_paths.append(temp_dir)
 
         # Also install any environment escape overrides directly here to enable
         # the escape to work even in non metaflow-created subprocesses
         generate_trampolines(self._metaflow_home)
 
+        # If we need to fetch the environment on exec, save the information we need
+        # so that we can resolve it using information such as run id, step name, task
+        # id and parameter values
+        if self.is_enabled() and self.is_fetch_at_exec():
+            self._flow = flow
+            self._env_for_fetch["METAFLOW_RUN_ID"] = run_id
+            self._env_for_fetch["METAFLOW_STEP_NAME"] = self.name
+
+    def runtime_task_created(
+        self,
+        task_datastore: TaskDataStore,
+        task_id: str,
+        split_index: int,
+        input_paths: List[str],
+        is_cloned: bool,
+        ubf_context: str,
+    ):
+        if self.is_enabled(ubf_context) and self.is_fetch_at_exec(ubf_context):
+            # We need to ensure we can properly find the environment we are
+            # going to run in
+            run_id, step_name, task_id = input_paths[0].split("/")
+            parent_ds = self._flow_datastore.get_task_datastore(
+                run_id, step_name, task_id
+            )
+            for var, _ in self._flow._get_parameters():
+                self._env_for_fetch[
+                    "METAFLOW_INIT_%s" % var.upper().replace("-", "_")
+                ] = lambda _param=getattr(
+                    self._flow, var
+                ), _var=var, _ds=parent_ds: str(
+                    _param.load_parameter(_ds[_var])
+                )
+            self._env_for_fetch["METAFLOW_TASK_ID"] = task_id
+
+            self._get_conda(self._echo, self._flow_datastore_type)
+            assert self.conda
+            # Calling from_env_name will resolve the environment name using all the
+            # additional variables injected above.
+            resolved_env_id = self.conda.env_id_from_alias(
+                cast(str, self.from_env_name), arch=self._arch
+            )
+            if resolved_env_id is None:
+                raise RuntimeError(
+                    "Cannot find environment '%s' (from '%s') for arch '%s'"
+                    % (self.from_env_name, self.from_env_name_unresolved, self._arch)
+                )
+
     def runtime_step_cli(
         self,
         cli_args: Any,  # Importing CLIArgs causes an issue so ignore for now
         retry_count: int,
         max_user_code_retries: int,
         ubf_context: str,
     ):
-        # If remote -- we don't do anything
-        if self._is_remote:
-            return
-
-        if self.is_enabled(UBF_TASK):
+        # We also set the env var in remote case for is_fetch_at_exec
+        # so that it can be used to fill out the bootstrap command with
+        # the proper environment
+        if self.is_enabled(UBF_TASK) or self.is_fetch_at_exec(ubf_context):
             self._get_conda(self._echo, self._flow_datastore_type)
             assert self.conda
             resolved_env = cast(
                 ResolvedEnvironment, self.conda.environment(self.env_id)
             )
             my_env_id = resolved_env.env_id
             # Export this for local runs, we will use it to read the "resolved"
             # environment ID in task_pre_step; this makes it compatible with the remote
             # bootstrap which also exports it. We do this even for UBF control tasks as
             # this environment variable is then passed to the actual tasks. We don't create
             # the environment for the control task -- just for the actual tasks.
             cli_args.env["_METAFLOW_CONDA_ENV"] = json.dumps(my_env_id)
 
-        if not self.is_enabled(ubf_context):
+        if not self.is_enabled(ubf_context) or self._is_remote:
             return
         # Create the environment we are going to use
 
         if self.conda.created_environment(my_env_id):
             self._echo(
                 "Using existing Conda environment %s (%s)"
                 % (my_env_id.req_id, my_env_id.full_id)
@@ -435,28 +562,42 @@
             raise InvalidEnvironmentException(
                 "@conda decorator is not compatible with @pip_base decorator."
             )
         if "conda_base" in self._flow._flow_decorators:
             return self._flow._flow_decorators["conda_base"][0].attributes
         return self.defaults
 
+    def _self_disabled(self) -> bool:
+        self_disabled = self.attributes["disabled"]
+        if self_disabled is None:
+            # If the user sets anything we consider that disabled = False
+            if (
+                self.attributes["name"]
+                or self.attributes["pathspec"]
+                or self.attributes["libraries"]
+                or self.attributes["pip_packages"]
+                or self.attributes["python"]
+            ):
+                self_disabled = False
+        return self_disabled
+
     def _python_version(self) -> str:
         return next(
             x
             for x in [
                 self.attributes["python"],
                 self._base_attributes["python"],
                 self._from_env_python(),
                 platform.python_version(),
             ]
             if x is not None
         )
 
-    def _from(self) -> Optional[str]:
-        return (
+    def _from(self, raw_name: bool = False) -> Optional[str]:
+        possible_name = (
             next(
                 x
                 for x in [
                     self.attributes["name"],
                     "step:%s" % self.attributes["pathspec"]
                     if self.attributes["pathspec"]
                     else None,
@@ -467,14 +608,24 @@
                     "",
                 ]
                 if x is not None
             )
             or None
         )
 
+        if possible_name is None:
+            return None
+
+        possible_name = cast(str, possible_name)
+        if raw_name:
+            return possible_name
+
+        # Substitute environment variables
+        return self.sub_envvars_in_envname(possible_name, self._env_for_fetch)
+
     def _from_env_python(self) -> Optional[str]:
         from_env = self.from_env
         if from_env:
             for p in from_env.packages:
                 if p.package_name == "python":
                     return p.package_version
             raise InvalidEnvironmentException(
@@ -623,14 +774,15 @@
             (
                 _,
                 self._resolved_sources,
                 self._resolved_deps,
                 _,
                 _,
             ) = EnvsResolver.extract_info_from_base(
+                self.conda,
                 self.from_env,
                 self._resolved_non_base_deps,
                 self._resolved_non_base_sources,
                 [],
                 self.from_env.env_id.arch,
             )
         else:
@@ -644,62 +796,113 @@
         )
 
     def _resolve_pip_or_conda_deco(
         self, flow: FlowSpec, decorators: List[StepDecorator]
     ) -> bool:
         has_pip_base = "pip_base" in flow._flow_decorators
         has_conda_base = "conda_base" in flow._flow_decorators
-        conda_decs = [(d, idx) for idx, d in enumerate(decorators) if d.name == "conda"]
-        pip_decs = [(d, idx) for idx, d in enumerate(decorators) if d.name == "pip"]
 
-        # It is possible we don't have both if we call step_init twice (which can
-        # happen when deploying to schedulers since we attach an additional deco
-        # and then call step_init again. In that case, we just continue for the
-        # decorator and ignore this function -- we already properly checked the
-        # first time around since both conda and pip decorators are added to all
-        # steps
+        # Note that other decorators *extend* either a conda decorator or a pip decorator
+        # so we look for those decorators as well.
+        # The pip decorator also extends the conda decorator but here we mean more
+        # in terms of functionality:
+        #  - extending a conda decorator means providing both pip and conda dependencies
+        #    (potentially)
+        #  - extending a pip decorator means providing only pip packages
+        all_decs = [d for d in decorators if isinstance(d, CondaStepDecorator)]
+        last_deco = all_decs[-1]
+        conda_decs = [d for d in all_decs if d.TYPE == "conda"]
+        pip_decs = [d for d in all_decs if d.TYPE == "pip"]
+
+        to_remove = []
+        if len(conda_decs) > 1:
+            # There is at least one user defined decorator so we remove all the others
+            to_remove = [x for x in conda_decs if not x.statically_defined]
+            conda_decs = [x for x in conda_decs if x.statically_defined]
+        if len(pip_decs) > 1:
+            # Ditto for pip
+            to_remove = [x for x in pip_decs if not x.statically_defined]
+            pip_decs = [x for x in pip_decs if x.statically_defined]
+
+        # In the environment with decospecs, we add both conda and pip
+        # decorators so that we can choose the best one based on the presence of the
+        # base decorators for example. In this function, we clean up the
+        # decorators and remove all the extraneous ones. In some cases, however,
+        # this function can be called multiple times (when deploying to a scheduler,
+        # the step_init (which calls this) is called twice). In that case, we just
+        # continue along as we already cleaned things out the first time.
         if len(conda_decs) == 0 or len(pip_decs) == 0:
             return True
 
-        conda_step_decorator, conda_idx = conda_decs[0]
-        pip_step_decorator, pip_idx = pip_decs[0]
+        if len(conda_decs) > 1:
+            # We can only have one Conda-type decorator
+            raise InvalidEnvironmentException(
+                "Multiple decorators (%s) provide @conda-like functionality for "
+                "step '%s'. Please add only one such decorator and include any "
+                "additional dependencies using the same arguments as for @conda."
+                % (", ".join(["@%s" % d.name for d in conda_decs]), self.name)
+            )
+        if len(pip_decs) > 1:
+            # Ditto with Pip-type decorators
+            raise InvalidEnvironmentException(
+                "Multiple decorators (%s) provide @pip-like functionality for "
+                "step '%s'. Please add only one such decorator and include any "
+                "additional dependencies using the same arguments as for @pip."
+                % (", ".join(["@%s" % d.name for d in pip_decs]), self.name)
+            )
 
-        my_idx = pip_idx if self.name == "pip" else conda_idx
+        conda_deco = conda_decs[0]
+        pip_deco = pip_decs[0]
 
         debug.conda_exec(
-            "In %s decorator: pip_base(%s), conda_base(%s), conda_idx(%d), pip_idx(%d)"
-            % (self.name, has_pip_base, has_conda_base, conda_idx, pip_idx)
+            "In %s decorator: pip_base(%s), conda_base(%s), conda_deco(%s), pip_deco(%s)"
+            % (self.name, has_pip_base, has_conda_base, conda_deco.name, pip_deco.name)
         )
-        if (
-            conda_step_decorator.statically_defined
-            and pip_step_decorator.statically_defined
-        ):
+        if conda_deco.statically_defined and pip_deco.statically_defined:
             raise InvalidEnvironmentException(
-                "Cannot specify both @conda and @pip on a step. "
-                "If you need both pip and conda dependencies, use @conda and "
-                "pass in the pip dependencies as `pip_packages` and the sources as "
-                "`pip_sources`"
-            )
-        if has_pip_base and conda_step_decorator.statically_defined:
-            raise InvalidEnvironmentException("@pip_base is not compatible with @conda")
-        if has_conda_base and pip_step_decorator.statically_defined:
-            raise InvalidEnvironmentException("@conda_base is not compatible with @pip")
+                "Cannot specify both @%s (Conda decorator) and @%s (Pip decorator) "
+                "in step '%s'. If you need both pip and conda dependencies, "
+                "use @%s and pass in the pip dependencies as `pip_packages` and "
+                "the sources as `pip_sources`"
+                % (
+                    conda_deco.name,
+                    pip_deco.name,
+                    self.name,
+                    conda_deco.name,
+                )
+            )
+        if has_pip_base and conda_deco.statically_defined:
+            raise InvalidEnvironmentException(
+                "@pip_base is not compatible with @%s. "
+                "Use @conda_base instead (using `pip_packages` instead of `packages` "
+                "and `pip_sources` instead of `sources`)" % conda_deco.name
+            )
+        if has_conda_base and pip_deco.statically_defined:
+            raise InvalidEnvironmentException(
+                "@conda_base is not compatible with @%s. Use @pip_base if only using "
+                "pip dependencies or replace @%s with a @conda decorator (using "
+                "`pip_packages` instead of `packages` and `pip_sources` instead of "
+                "`sources)" % (pip_deco.name, pip_deco.name)
+            )
 
         # At this point, we have at most one statically defined so we keep that one
         # or the one derived from the base decorator.
-        # If we have none, we keep the conda one (base one). We remove only when
-        # we are the second decorator
+        # If we have none, we keep the conda one (base one).
         # Return true if we should continue the function. False if we return (ie:
         # we are going to be deleted)
-        del_idx = pip_idx
-        if pip_step_decorator.statically_defined or has_pip_base:
-            del_idx = conda_idx
-        if my_idx == max(pip_idx, conda_idx):
-            del decorators[del_idx]
-        return my_idx != del_idx
+        del_deco = pip_deco
+        if pip_deco.statically_defined or has_pip_base:
+            del_deco = conda_deco
+        to_remove.append(del_deco)
+        # We remove only when we are the last decorator since this is called while
+        # we are iterating on the list
+        if self.name == last_deco.name:
+            for d in to_remove:
+                decorators.remove(d)
+        return self.name not in [d.name for d in to_remove]
 
     @classmethod
     def _get_conda(cls, echo: Callable[..., None], datastore_type: str) -> None:
         if cls.conda is None:
             cls.conda = Conda(echo, datastore_type)
 
 
@@ -717,42 +920,66 @@
     will prevail.
 
     Parameters
     ----------
     name : Optional[str]
         If specified, can refer to a named environment. The environment referred to
         here will be the one used for this step. If specified, nothing else can be
-        specified in this decorator
+        specified in this decorator. In the name, you can use `@{}` values and
+        environment variables will be used to substitute.
     pathspec : Optional[str]
         If specified, can refer to the pathspec of an existing step. The environment
         of this referred step will be used here. If specified, nothing else can be
-        specified in this decorator.
+        specified in this decorator. In the name, you can use `@{}` values and
+        environment variables will be used to substitute.
     packages : Optional[Dict[str, str]]
         Packages to use for this step. The key is the name of the package
         and the value is the version to use (default: `{}`).
     sources : Optional[List[str]]
         Additional channels to search for
     python : Optional[str]
         Version of Python to use, e.g. '3.7.4'. If not specified, the current python
         version will be used.
+    fetch_at_exec : bool, default False
+        If set to True, the environment will be fetched when the task is
+        executing as opposed to at the beginning of the flow (or at deploy time if
+        deploying to a scheduler). This option requires name or pathspec to be
+        specified. This is useful, for example, if you want this step to always use
+        the latest named environment when it runs as opposed to the latest when it
+        is deployed.
     disabled : bool, default False
         If set to True, disables Pip.
     """
 
     name = "pip"
+    TYPE = "pip"
 
     defaults = {
         "name": None,
         "pathspec": None,
         "packages": {},
         "sources": [],
         "python": None,
+        "fetch_at_exec": None,
         "disabled": None,
     }
 
+    def _self_disabled(self) -> bool:
+        self_disabled = self.attributes["disabled"]
+        if self_disabled is None:
+            # If the user sets anything we consider that disabled = False
+            if (
+                self.attributes["name"]
+                or self.attributes["pathspec"]
+                or self.attributes["packages"]
+                or self.attributes["python"]
+            ):
+                self_disabled = False
+        return self_disabled
+
     def _np_conda_deps(self) -> Dict[str, str]:
         return {}
 
     def _conda_deps(self) -> Dict[str, str]:
         if self.from_env and self.from_env.env_type != EnvType.PIP_ONLY:
             return dict(
                 get_pinned_conda_libs(self._python_version(), self._flow_datastore_type)
```

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/env_descr.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from metaflow.util import get_username
 
 from .utils import (
     _ALL_PIP_FORMATS,
     FAKEURL_PATHCOMPONENT,
     AliasType,
     arch_id,
+    channel_from_url,
     correct_splitext,
     get_conda_manifest_path,
     is_alias_mutable,
 )
 
 # Order should be maintained
 EnvID = NamedTuple("EnvID", [("req_id", str), ("full_id", str), ("arch", str)])
@@ -167,15 +168,14 @@
             )
         base_cache_url = cls.make_partial_cache_url(base_url, is_real_url)
         return os.path.join(
             base_cache_url, filename_with_ext, file_hash, filename_with_ext
         )
 
     def __init__(self, url: str):
-
         self._url = url
         basename, filename = os.path.split(url)
         _, self._pkg_fmt = correct_splitext(filename)
         if self._pkg_fmt not in self.allowed_formats():
             raise ValueError(
                 "URL '%s' does not end with a supported file format %s"
                 % (url, str(self.allowed_formats()))
@@ -314,14 +314,30 @@
     def filename(self) -> str:
         return self._filename
 
     @property
     def package_name(self) -> str:
         return self._package_name
 
+    def package_name_with_channel(
+        self, ignore_channels: Optional[List[str]] = None
+    ) -> str:
+        if ignore_channels is None:
+            ignore_channels = []
+        if self.TYPE != "conda":
+            return self.package_name
+        if self.is_downloadable_url():
+            # Extract the channel information from the URL. We only extract implicit
+            # channels (ie: things like comet_ml) that can be embedded in the name
+            # (for example: comet_ml::comet_ml)
+            channel = channel_from_url(self.url)
+            if channel and channel not in ignore_channels:
+                return "%s::%s" % (channel, self.package_name)
+        return self.package_name
+
     @property
     def package_version(self) -> str:
         return self._package_version
 
     @property
     def package_detailed_version(self) -> str:
         return self._package_detailed_version
@@ -370,16 +386,18 @@
 
     def local_file(self, pkg_format: str) -> Optional[str]:
         # Return the local tar-ball for this package (depending on the format)
         return self._local_path.get(pkg_format)
 
     @property
     def local_files(self) -> Iterable[Tuple[str, str]]:
-        for pkg_fmt, local_path in self._local_path.items():
-            yield (pkg_fmt, local_path)
+        for pkg_fmt in self.allowed_formats():
+            local_path = self._local_path.get(pkg_fmt)
+            if local_path:
+                yield (pkg_fmt, local_path)
 
     def is_fetched(self, pkg_format: str) -> bool:
         # Return whether the local tar-ball for this package had to be fetched from
         # either cache or web
         return pkg_format in self._is_fetched
 
     def is_downloadable_url(self, pkg_format: Optional[str] = None) -> bool:
@@ -420,39 +438,37 @@
 
     def add_local_file(
         self,
         pkg_format: str,
         local_path: str,
         pkg_hash: Optional[str] = None,
         downloaded: bool = False,
+        replace: bool = False,
     ):
         # Add a local file for this package indicating whether it was downloaded
         existing_path = self.local_file(pkg_format)
-        if existing_path:
-            if local_path != existing_path:
-                raise ValueError(
-                    "Attempting to add inconsistent local files of format %s for a package %s; "
-                    "adding %s when already have %s"
-                    % (pkg_format, self.filename, local_path, existing_path)
-                )
-        else:
-            self._dirty = True
-            self._local_path[pkg_format] = local_path
+        if not replace and existing_path and local_path != existing_path:
+            raise ValueError(
+                "Attempting to add inconsistent local files of format %s for a package %s; "
+                "adding %s when already have %s"
+                % (pkg_format, self.filename, local_path, existing_path)
+            )
+
         known_hash = self._hashes.get(pkg_format)
         added_hash = pkg_hash or self.hash_pkg(local_path)
-        if known_hash:
-            if known_hash != added_hash:
-                raise ValueError(
-                    "Attempting to add inconsistent local files of format %s for package %s; "
-                    "got a hash of %s but expected %s"
-                    % (pkg_format, self.filename, added_hash, known_hash)
-                )
-        else:
-            self._dirty = True
-            self._hashes[pkg_format] = added_hash
+        if not replace and known_hash and known_hash != added_hash:
+            raise ValueError(
+                "Attempting to add inconsistent local files of format %s for package %s; "
+                "got a hash of %s but expected %s"
+                % (pkg_format, self.filename, added_hash, known_hash)
+            )
+        self._dirty = replace or existing_path is None or known_hash is None
+        self._local_path[pkg_format] = local_path
+        self._hashes[pkg_format] = added_hash
+
         if downloaded and pkg_format not in self._is_fetched:
             self._dirty = True
             self._is_fetched.append(pkg_format)
 
     def cached_version(self, pkg_format: str) -> Optional[CachePackage]:
         return self._cache_info.get(
             self._url_format if pkg_format == "_any" else pkg_format
```

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/envsresolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 from .env_descr import EnvID, EnvType, PackageSpecification, ResolvedEnvironment, TStr
 from .conda import Conda
 from .conda_step_decorator import CondaStepDecorator
 from .utils import (
     AliasType,
     CondaException,
+    channel_from_url,
     arch_id,
     merge_dep_dicts,
     plural_marker,
     resolve_env_alias,
     split_into_dict,
 )
 
@@ -113,15 +114,15 @@
             (
                 env_id,
                 user_sources,
                 user_deps,
                 deps,
                 extras,
             ) = self.extract_info_from_base(
-                base_env, user_deps, user_sources, extras, architecture
+                self._conda, base_env, user_deps, user_sources, extras, architecture
             )
         else:
             env_id = EnvID(
                 ResolvedEnvironment.get_req_id(user_deps, user_sources, extras),
                 "_default",
                 architecture,
             )
@@ -208,14 +209,15 @@
             (
                 env_id,
                 user_sources,
                 user_deps,
                 deps,
                 extras,
             ) = self.extract_info_from_base(
+                self._conda,
                 from_env,
                 decorator.non_base_step_deps,
                 decorator.source_deps,
                 [],
                 arch_id(),
             )
             env_ids = [env_id]
@@ -714,15 +716,20 @@
                     if (
                         addl_builder_env
                         and addl_builder_env.env_id not in self._builder_envs
                     ):
                         # We "hack" the extract_from_base to get the proper user and
                         # full requirements from addl_builder_env
                         _, _, user_deps, full_deps, _ = self.extract_info_from_base(
-                            addl_builder_env, [], [], [], addl_builder_env.env_id.arch
+                            self._conda,
+                            addl_builder_env,
+                            [],
+                            [],
+                            [],
+                            addl_builder_env.env_id.arch,
                         )
                         self._builder_envs[addl_builder_env.env_id] = {
                             "id": addl_builder_env.env_id,
                             "steps": self._requested_envs[env_id]["steps"],
                             "user_deps": user_deps,
                             "deps": full_deps,
                             "sources": addl_builder_env.sources,
@@ -765,14 +772,15 @@
                     )
 
         duration = int(time.time() - start)
         echo(" done in %d second%s." % (duration, plural_marker(duration)))
 
     @staticmethod
     def extract_info_from_base(
+        conda: Conda,
         base_env: ResolvedEnvironment,
         deps: Sequence[TStr],
         sources: Sequence[TStr],
         extras: Sequence[TStr],
         architecture: str,
     ) -> Tuple[EnvID, Sequence[TStr], Sequence[TStr], Sequence[TStr], Sequence[TStr]]:
         """
@@ -828,32 +836,40 @@
             incoming_pip_deps,
         )
         user_npconda_deps = merge_dep_dicts(
             split_into_dict([d for d in base_env.deps if d.category == "npconda"]),
             incoming_npconda_deps,
         )
 
+        # Extract the implicit channels that are already listed somewhere
+        sources = list(set(chain(base_env.sources, sources)))
+        extras = list(set(chain(base_env.extras, extras)))
+
+        included_channels = set()  # type: Set[str]
+        for s in chain(sources, conda.default_conda_channels):
+            channel = channel_from_url(s.value if isinstance(s, TStr) else s)
+            if channel:
+                included_channels.add(channel)
+
+        included_channels_list = list(included_channels)
         conda_deps = {
-            p.package_name: p.package_version
+            p.package_name_with_channel(included_channels_list): p.package_version
             for p in base_env.packages
             if p.TYPE == "conda"
         }
         conda_deps = merge_dep_dicts(conda_deps, incoming_conda_deps)
         conda_deps = merge_dep_dicts(conda_deps, incoming_npconda_deps)
 
         pip_deps = {
             p.package_name: p.package_version
             for p in base_env.packages
             if p.TYPE == "pip"
         }
         pip_deps = merge_dep_dicts(pip_deps, incoming_pip_deps)
 
-        sources = list(set(chain(base_env.sources, sources)))
-        extras = list(set(chain(base_env.extras, extras)))
-
         deps = list(
             chain(
                 [
                     TStr("conda", "%s==%s" % (k, v) if v else k)
                     for k, v in conda_deps.items()
                 ],
                 [
```

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/remote_bootstrap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # pyright: strict, reportTypeCommentUsage=false, reportMissingTypeStubs=false
+import json
 import os
 import shutil
 import sys
 import time
 from typing import Any, Callable
 
 from metaflow.metaflow_config import DATASTORE_LOCAL_DIR, CONDA_MAGIC_FILE_V2
@@ -10,14 +11,15 @@
 from metaflow.cli import echo_always
 
 from metaflow.debug import debug
 
 from metaflow.plugins.env_escape import generate_trampolines, ENV_ESCAPE_PY
 
 from .conda import Conda
+from .conda_step_decorator import CondaStepDecorator
 from .env_descr import EnvID
 from .utils import arch_id
 
 
 def my_echo_always(*args: Any, **kwargs: Any) -> Callable[..., None]:
     kwargs["err"] = False
     return echo_always(*args, **kwargs)
@@ -28,14 +30,25 @@
 ):
     start = time.time()
     my_echo_always("    Setting up Conda ...", nl=False)
     setup_conda_manifest()
     my_conda = Conda(my_echo_always, datastore_type, mode="remote")
     my_echo_always(" done in %d seconds." % int(time.time() - start))
 
+    # Resolve a late environment if full_id is a special string _fetch_exec
+    if full_id == "_fetch_exec":
+        alias_to_fetch = CondaStepDecorator.sub_envvars_in_envname(req_id)
+        env_id = my_conda.env_id_from_alias(alias_to_fetch)
+        if env_id is None:
+            raise RuntimeError(
+                "Cannot find environment '%s' (from '%s') for arch '%s'"
+                % (alias_to_fetch, req_id, arch_id())
+            )
+        req_id = env_id.req_id
+        full_id = env_id.full_id
     resolved_env = my_conda.environment(
         EnvID(req_id=req_id, full_id=full_id, arch=arch_id())
     )
     if resolved_env is None:
         raise RuntimeError(
             "Cannot find cached environment for hash %s:%s" % (req_id, full_id)
         )
@@ -49,14 +62,18 @@
         os.makedirs(trampoline_dir)
         generate_trampolines(trampoline_dir)
         # print("Environment escape will use %s as the interpreter" % ENV_ESCAPE_PY)
     else:
         pass
         # print("Could not find a environment escape interpreter")
 
+    # We write out the env_id to _env_id so it can be read by the outer bash script
+    with open("_env_id", mode="w", encoding="utf-8") as f:
+        json.dump(EnvID(req_id, full_id, arch_id()), f)
+
 
 def setup_conda_manifest():
     manifest_folder = os.path.join(os.getcwd(), DATASTORE_LOCAL_DIR)
     if not os.path.exists(manifest_folder):
         os.makedirs(manifest_folder)
     shutil.move(
         os.path.join(os.getcwd(), CONDA_MAGIC_FILE_V2),
```

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/resources/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/terminal_menu.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/conda/utils.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/conda/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,32 @@
 
 from enum import Enum
 from itertools import chain
 from typing import (
     Dict,
     FrozenSet,
     List,
+    Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Tuple,
     Union,
+    cast,
 )
 from urllib.parse import urlparse, unquote
 
+from requests import PreparedRequest
+from requests.auth import AuthBase, HTTPBasicAuth
+
 from metaflow_extensions.netflix_ext.vendor.packaging.tags import (
     compatible_tags,
     _cpython_abis,
     cpython_tags,
+    mac_platforms,
     Tag,
 )
 
 from metaflow_extensions.netflix_ext.vendor.packaging.utils import (
     BuildTag,
     parse_wheel_filename,
 )
@@ -40,26 +46,27 @@
 
 from metaflow.debug import debug
 from metaflow.exception import MetaflowException
 import metaflow.metaflow_config as mf_config
 from metaflow.metaflow_config import (
     CONDA_MAGIC_FILE_V2,  # type: ignore
     CONDA_PREFERRED_FORMAT,  # type: ignore
+    CONDA_SRCS_AUTH_INFO,
 )
 
 from metaflow.metaflow_environment import InvalidEnvironmentException
 
 # NOTA: Most of the code does not assume that there are only two formats BUT the
 # transmute code does (since you can only specify the infile -- the outformat and file
 # are inferred)
 _ALL_CONDA_FORMATS = (".tar.bz2", ".conda")
 # NOTE: Order is important as it is a preference order
 _ALL_PIP_FORMATS = (".whl", ".tar.gz", ".zip")
-_VALID_IMAGE_NAME = "[^a-z0-9_/]"
-_VALID_TAG_NAME = "[^a-z0-9_]"
+_VALID_IMAGE_NAME = "[^-a-z0-9_/]"
+_VALID_TAG_NAME = "[^-a-z0-9_]"
 
 
 class AliasType(Enum):
     PATHSPEC = "pathspec"
     FULL_ID = "full-id"
     REQ_FULL_ID = "both-id"
     GENERIC = "generic"
@@ -144,33 +151,38 @@
 def pip_tags_from_arch(python_version: str, arch: str) -> List[Tag]:
     # Converts a Conda architecture to a tuple containing (implementation, platforms, abis)
     # This function will assume a CPython implementation
 
     # This is inspired by what pip does:
     # https://github.com/pypa/pip/blob/0442875a68f19b0118b0b88c747bdaf6b24853ba/src/pip/_internal/utils/compatibility_tags.py
     py_version = tuple(map(int, python_version.split(".")[:2]))
-    if arch.startswith("linux-"):
-        detail = arch.split("-")[-1]
-        if detail == "64":
-            detail = "x86_64"
+    if arch == "linux-64":
         platforms = [
-            "manylinux%s_%s" % (tag, arch) for tag in ["_2_17", "2014", "2010", "1"]
+            "manylinux%s_x86_64" % s
+            for s in (
+                "1",
+                "2010",
+                "2014",
+                "_2_17",
+                "_2_18",
+                "_2_19",
+                "_2_20",
+                "_2_21",
+                "_2_23",
+                "_2_24",
+                "_2_25",
+                "_2_26",
+                "_2_27",
+            )
         ]
-        platforms.append("linux_%s" % detail)
+        platforms.append("linux_x86_64")
     elif arch == "osx-64":
-        platforms = [
-            "macosx_10_9_x86_64",
-            *("macosx_10_%s_universal2" % v for v in range(16, 3, -1)),
-            *("macosx_10_%s_universal" % v for v in range(16, 3, -1)),
-        ]
+        platforms = mac_platforms((11, 0), "x86_64")
     elif arch == "osx-arm64":
-        platforms = [
-            "macosx_11_0_arm64",
-            *("macosx_10_%s_universal2" % v for v in range(16, 3, -1)),
-        ]
+        platforms = mac_platforms((11, 0), "arm64")
     else:
         raise InvalidEnvironmentException("Unsupported platform: %s" % arch)
 
     interpreter = "cp%s" % ("".join(map(str, py_version)))
 
     abis = _cpython_abis(py_version)
 
@@ -292,24 +304,24 @@
             image_tag = splits[1]
         else:
             image_name = env_alias
             image_tag = "latest"
         if re.search(_VALID_IMAGE_NAME, image_name):
             raise MetaflowException(
                 "An environment name must contain only "
-                "lowercase alphanumeric characters, underscores and forward slashes."
+                "lowercase alphanumeric characters, dashes, underscores and forward slashes."
             )
         if image_name[0] == "/" or image_name[-1] == "/":
             raise MetaflowException(
                 "An environment name must not start or end with '/'"
             )
         if re.search(_VALID_TAG_NAME, image_tag):
             raise MetaflowException(
                 "An environment tag name must contain only "
-                "lowercase alphanumeric characters and underscores."
+                "lowercase alphanumeric characters, dashes and underscores."
             )
         return AliasType.GENERIC, "/".join([image_name, image_tag])
     raise MetaflowException("Invalid format for environment alias: '%s'" % env_alias)
 
 
 def is_alias_mutable(alias_type: AliasType, resolved_alias: str) -> bool:
     if alias_type != AliasType.GENERIC:
@@ -404,14 +416,56 @@
 _UNDERSCORE_REGEX = re.compile(r"[-_.]+")
 
 
 def normalize_to_underscore(name: str) -> str:
     return _UNDERSCORE_REGEX.sub("_", name).lower()
 
 
+def channel_from_url(url: str) -> Optional[str]:
+    up = urlparse(url)
+    if up.hostname == "conda.anaconda.org":
+        return up.path.split("/", 2)[1]
+    return None
+
+
+def auth_from_urls(urls: List[str]) -> Optional[AuthBase]:
+    auths_per_hostname = {
+        cast(str, h): HTTPBasicAuth(username, pwd)
+        for h, (username, pwd) in CONDA_SRCS_AUTH_INFO.items()
+    }
+
+    for url in urls:
+        up = urlparse(url.strip("'\" \t\n"))
+        if up.hostname and up.username:
+            auths_per_hostname[up.hostname] = HTTPBasicAuth(
+                up.username, up.password or ""
+            )
+    if auths_per_hostname:
+        return PerHostAuth(auths_per_hostname)
+    return None
+
+
+class PerHostAuth(AuthBase):
+    def __init__(self, auths_per_hostname: Mapping[str, AuthBase]):
+        self._my_auths = auths_per_hostname
+
+    def __call__(self, r: PreparedRequest):
+        up = urlparse(r.url)
+        if up.hostname:
+            h = (
+                up.hostname
+                if isinstance(up.hostname, str)
+                else up.hostname.decode(encoding="utf-8")
+            )
+            auth_provider = self._my_auths.get(h or "<none>")
+            if auth_provider:
+                return auth_provider(r)
+        return r
+
+
 # Function heavily inspired from https://github.com/hauntsaninja/change_wheel_version
 # MIT license of that source file:
 # MIT License
 
 # Copyright (c) 2023 hauntsaninja
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -420,14 +474,15 @@
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 
 # The above copyright notice and this permission notice shall be included in all
 # copies or substantial portions of the Software.
 
+
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
```

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/plugins/environment_cli.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/plugins/environment_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/markers.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/tags.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/utils.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_extensions/netflix_ext/vendor/packaging/version.py` & `metaflow-netflixext-0.2.1/metaflow_extensions/netflix_ext/vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/PKG-INFO` & `metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-netflixext
-Version: 0.2.0
+Version: 0.2.1
 Summary: EXPERIMENTAL Metaflow extensions from Netflix
 Author: Netflix Metaflow Developers
 Author-email: metaflow-dev@netflix.com
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow-nflx-extensions
 Project-URL: Tracker, https://github.com/Netflix/metaflow-nflx-extensions/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `metaflow-netflixext-0.2.0/metaflow_netflixext.egg-info/SOURCES.txt` & `metaflow-netflixext-0.2.1/metaflow_netflixext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-netflixext-0.2.0/setup.py` & `metaflow-netflixext-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_namespace_packages
 
-version = "0.2.0"
+version = "0.2.1"
 
 setup(
     name="metaflow-netflixext",
     version=version,
     description="EXPERIMENTAL Metaflow extensions from Netflix",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

