# Comparing `tmp/galaxy-test-api-22.5.0.dev0.tar.gz` & `tmp/galaxy-test-api-23.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-test-api-22.5.0.dev0.tar", last modified: Thu Dec  8 12:00:31 2022, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/test_api/dist/.tmp-zrstd1o3/galaxy-test-api-23.0.2.tar", last modified: Tue Jun 13 17:15:20 2023, max compression
```

## Comparing `galaxy-test-api-22.5.0.dev0.tar` & `galaxy-test-api-23.0.2.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-12-08 12:00:31.052080 galaxy-test-api-22.5.0.dev0/
--rw-r--r--   0 mvandenb   (501) staff       (20)      227 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2022-12-08 11:38:32.000000 galaxy-test-api-22.5.0.dev0/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)       58 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     1579 2022-12-08 12:00:31.052228 galaxy-test-api-22.5.0.dev0/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      295 2022-12-08 11:38:33.000000 galaxy-test-api-22.5.0.dev0/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-12-08 12:00:31.030455 galaxy-test-api-22.5.0.dev0/galaxy_test/
--rw-r--r--   0 mvandenb   (501) staff       (20)       65 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-12-08 12:00:31.049529 galaxy-test-api-22.5.0.dev0/galaxy_test/api/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:11.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      994 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/_framework.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-12-08 12:00:31.049937 galaxy-test-api-22.5.0.dev0/galaxy_test/api/cwl/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-11-16 11:10:40.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/cwl/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      363 2022-11-16 11:10:40.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/embed_test_1.gxwf.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)       95 2022-03-24 19:47:11.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/embed_test_1_tool.gxtool.yml
--rw-r--r--   0 mvandenb   (501) staff       (20)     7532 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/sharable.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2658 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_authenticate.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1847 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_configuration.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      910 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_container_resolution.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    28032 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_dataset_collections.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    25061 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_datasets.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4345 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_datatypes.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2107 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_display_applications.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    10516 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_folder_contents.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     6396 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_folders.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1684 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_framework.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5730 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_group_roles.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5678 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_group_users.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4393 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_groups.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    31358 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_histories.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    78434 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_history_contents.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2300 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_history_contents_provenance.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    48359 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_jobs.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    28275 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_libraries.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      797 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_licenses.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1788 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_page_revisions.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    19254 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_pages.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5888 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_roles.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1355 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_search.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3744 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_tool_data.py
--rw-r--r--   0 mvandenb   (501) staff       (20)   147860 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_tools.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    45787 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_tools_upload.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      935 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_tours.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     8798 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_users.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4159 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_visualizations.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1244 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_webhooks.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    27405 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_workflow_extraction.py
--rw-r--r--   0 mvandenb   (501) staff       (20)   225219 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_workflows.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      414 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_workflows_cwl.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    11561 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_workflows_from_yaml.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-12-08 12:00:31.051771 galaxy-test-api-22.5.0.dev0/galaxy_test_api.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1579 2022-12-08 12:00:31.000000 galaxy-test-api-22.5.0.dev0/galaxy_test_api.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)     1760 2022-12-08 12:00:31.000000 galaxy-test-api-22.5.0.dev0/galaxy_test_api.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-12-08 12:00:31.000000 galaxy-test-api-22.5.0.dev0/galaxy_test_api.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       84 2022-12-08 12:00:31.000000 galaxy-test-api-22.5.0.dev0/galaxy_test_api.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       12 2022-12-08 12:00:31.000000 galaxy-test-api-22.5.0.dev0/galaxy_test_api.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       81 2022-12-08 11:44:37.000000 galaxy-test-api-22.5.0.dev0/pyproject.toml
--rw-r--r--   0 mvandenb   (501) staff       (20)     1225 2022-12-08 12:00:31.052898 galaxy-test-api-22.5.0.dev0/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-11-16 11:10:40.000000 galaxy-test-api-22.5.0.dev0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:15:20.000000 galaxy-test-api-23.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-13 17:04:36.000000 galaxy-test-api-23.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-13 17:15:20.000000 galaxy-test-api-23.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:15:20.000000 galaxy-test-api-23.0.2/galaxy_test/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:15:20.000000 galaxy-test-api-23.0.2/galaxy_test/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:15:20.000000 galaxy-test-api-23.0.2/galaxy_test/api/cwl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/cwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/embed_test_1.gxwf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/embed_test_1_tool.gxtool.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/sharable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_container_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32663 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_dataset_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_display_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_drs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19565 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_folder_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32996 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_histories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66820 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_history_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_history_contents_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48126 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29256 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_page_revisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19259 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_short_term_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_tool_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146748 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46294 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_tools_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_tours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27653 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_workflow_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)   258805 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_workflows_cwl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/api/test_workflows_from_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/galaxy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:15:20.000000 galaxy-test-api-23.0.2/galaxy_test_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-13 17:15:20.000000 galaxy-test-api-23.0.2/galaxy_test_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-13 17:15:20.000000 galaxy-test-api-23.0.2/galaxy_test_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:15:20.000000 galaxy-test-api-23.0.2/galaxy_test_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-13 17:15:20.000000 galaxy-test-api-23.0.2/galaxy_test_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 17:15:20.000000 galaxy-test-api-23.0.2/galaxy_test_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-13 17:15:20.000000 galaxy-test-api-23.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:04:37.000000 galaxy-test-api-23.0.2/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-test-api-22.5.0.dev0/LICENSE` & `galaxy-test-api-23.0.2/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,61 @@
-Copyright (c) 2005-2016 Galaxy Contributors (see CONTRIBUTORS.md)
+Copyright (c) 2005-2022 Galaxy Contributors (see CONTRIBUTORS.md)
+
+Work contributed from 2021-04-07 onwards is licensed under the MIT License.
+Work contributed before this date is licensed under the Academic Free License
+version 3.0.
+See https://github.com/galaxyproject/galaxy/ for the contribution history.
+See below for the full text of both licenses.
+
+
+Some icons found in Galaxy are from the Silk Icons set, available under
+the Creative Commons Attribution 2.5 License, from:
+
+http://www.famfamfam.com/lab/icons/silk/
+
+
+Other images and documentation are licensed under the Creative Commons
+Attribution 3.0 (CC BY 3.0) License. See:
+
+http://creativecommons.org/licenses/by/3.0/
+
+
+--------------------------------------------------------------------------------
+
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+--------------------------------------------------------------------------------
+
+
+Academic Free License ("AFL") v. 3.0
+
+This Academic Free License (the "License") applies to any original work of
+authorship (the "Original Work") whose owner (the "Licensor") has placed the
+following licensing notice adjacent to the copyright notice for the Original
+Work:
 
 Licensed under the Academic Free License version 3.0
 
  1) Grant of Copyright License. Licensor grants You a worldwide, royalty-free, 
     non-exclusive, sublicensable license, for the duration of the copyright, to 
     do the following:
 
@@ -169,18 +222,7 @@
     replace the notice specified in the first paragraph above with the 
     notice "Licensed under <insert your license name here>" or with a notice 
     of your own that is not confusingly similar to the notice in this 
     License; and (iii) You may not claim that your original works are open 
     source software unless your Modified License has been approved by Open 
     Source Initiative (OSI) and You comply with its license review and 
     certification process.
-
-
-Some icons found in Galaxy are from the Silk Icons set, available under
-the Creative Commons Attribution 2.5 License, from:
-
-http://www.famfamfam.com/lab/icons/silk/
-
-
-Other images and documentation are licensed under the Creative Commons Attribution 3.0 (CC BY 3.0) License.   See 
-
-http://creativecommons.org/licenses/by/3.0/
```

### Comparing `galaxy-test-api-22.5.0.dev0/PKG-INFO` & `galaxy-test-api-23.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-api
-Version: 22.5.0.dev0
+Version: 23.0.2
 Summary: Galaxy API tests
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: driver
 License-File: LICENSE
@@ -33,29 +34,49 @@
 
 
 Overview
 --------
 
 The Galaxy_ API tests.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.1.dev0
----------------------
+-------------------
+23.0.2 (2023-06-13)
+-------------------
 
+No recorded changes since last release
 
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
----------------------
+
+=========
+Bug fixes
+=========
+
+* Display DCE in job parameter component, allow rerunning with DCE input by `@mvdbeek <https://github.com/mvdbeek>`_ in `#15744 <https://github.com/galaxyproject/galaxy/pull/15744>`_
+* Fix folder listing via file browser by `@mvdbeek <https://github.com/mvdbeek>`_ in `#15950 <https://github.com/galaxyproject/galaxy/pull/15950>`_
+* Fix case sensitive filtering by name in histories by `@davelopez <https://github.com/davelopez>`_ in `#16036 <https://github.com/galaxyproject/galaxy/pull/16036>`_
+* Fix dataype_change not updating HDCA update_time by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16099 <https://github.com/galaxyproject/galaxy/pull/16099>`_
+* Extract HDA for code_file validate_input hook by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16120 <https://github.com/galaxyproject/galaxy/pull/16120>`_
+
+============
+Enhancements
+============
+
+* Add support for launching workflows via Tutorial Mode by `@hexylena <https://github.com/hexylena>`_ in `#15684 <https://github.com/galaxyproject/galaxy/pull/15684>`_
+* Allow setting auto_decompress property in staging interface by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16014 <https://github.com/galaxyproject/galaxy/pull/16014>`_
+
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * Initial import from dev branch of Galaxy during 20.09 branch of Galaxy.
-
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/_framework.py` & `galaxy-test-api-23.0.2/galaxy_test/api/_framework.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from typing import Optional
-from unittest import (
-    SkipTest,
-    TestCase,
+from typing import (
+    Iterator,
+    Optional,
 )
+from unittest import SkipTest
+
+import pytest
 
 from galaxy_test.base.api import (
     UsesApiTestCaseMixin,
     UsesCeleryTasks,
 )
 from galaxy_test.base.testcase import FunctionalTestCase
 
@@ -14,22 +16,27 @@
     from galaxy_test.driver.driver_util import GalaxyTestDriver
 except ImportError:
     # Galaxy libraries and galaxy test driver not available, just assume we're
     # targetting a remote Galaxy.
     GalaxyTestDriver = None  # type: ignore[misc,assignment]
 
 
-class ApiTestCase(FunctionalTestCase, UsesApiTestCaseMixin, UsesCeleryTasks, TestCase):
+class ApiTestCase(FunctionalTestCase, UsesApiTestCaseMixin, UsesCeleryTasks):
     galaxy_driver_class = GalaxyTestDriver
     _test_driver: Optional[GalaxyTestDriver]
 
     def setUp(self):
         super().setUp()
         self._setup_interactor()
 
     def driver_or_skip_test_if_remote(self) -> GalaxyTestDriver:
         if self._test_driver is None:
             raise SkipTest("This test does not work with remote Galaxy instances.")
         return self._test_driver
 
+    @pytest.fixture
+    def history_id(self) -> Iterator[str]:
+        with self.galaxy_interactor.test_history() as history_id:
+            yield history_id
+
 
 __all__ = ("ApiTestCase",)
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/sharable.py` & `galaxy-test-api-23.0.2/galaxy_test/api/sharable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import (
     Any,
     Dict,
     List,
 )
 from unittest import SkipTest
+from uuid import uuid4
 
 from galaxy_test.base.api import UsesApiTestCaseMixin
 
 
 class SharingApiTests(UsesApiTestCaseMixin):
     """Includes some tests for the sharing functionality of a particular resource type."""
 
@@ -136,19 +137,20 @@
         assert sharing_response["errors"]
         assert invalid_user_email in sharing_response["errors"][0]
 
     def test_set_slug(self):
         resource_id = self.create("resource-to-set-slug")
         other_resource_id = self.create("other-resource-to-set-slug")
 
-        response = self._set_slug(resource_id, "new-slug")
+        new_slug = f"new-slug-{uuid4()}"
+        response = self._set_slug(resource_id, new_slug)
         self._assert_status_code_is_ok(response)
 
         # Slugs must be unique for the same user/resource
-        response = self._set_slug(other_resource_id, "new-slug")
+        response = self._set_slug(other_resource_id, new_slug)
         self._assert_status_code_is(response, 409)
 
         # Other users cannot change the slug if they don't own the resource
         with self._different_user():
             response = self._set_slug(resource_id, "another-slug")
             self._assert_status_code_is(response, 403)
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_authenticate.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_authenticate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-import base64
 from urllib.parse import urljoin
 
 from requests import get
 
+from galaxy_test.base.api_util import baseauth_headers
+from galaxy_test.base.decorators import requires_new_user
 from ._framework import ApiTestCase
 
 TEST_USER_EMAIL = "auth_user_test@bx.psu.edu"
 TEST_USER_PASSWORD = "testpassword1"
 
 
-class AuthenticationApiTestCase(ApiTestCase):
+class TestAuthenticateApi(ApiTestCase):
+    @requires_new_user
     def test_auth(self):
         self._setup_user(TEST_USER_EMAIL, TEST_USER_PASSWORD)
         baseauth_url = self._api_url("authenticate/baseauth", use_key=False)
-        unencoded_credentials = f"{TEST_USER_EMAIL}:{TEST_USER_PASSWORD}"
-        authorization = base64.b64encode(unencoded_credentials.encode("utf-8"))
-        headers = {
-            "Authorization": authorization,
-        }
+        headers = baseauth_headers(TEST_USER_EMAIL, TEST_USER_PASSWORD)
         auth_response = get(baseauth_url, headers=headers)
         self._assert_status_code_is(auth_response, 200)
         auth_dict = auth_response.json()
         self._assert_has_keys(auth_dict, "api_key")
 
         # Verify key...
         random_api_url = self._api_url("users", use_key=False)
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_configuration.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from galaxy_test.base.api_asserts import (
     assert_has_keys,
     assert_not_has_keys,
 )
 from galaxy_test.base.api_util import TEST_USER
+from galaxy_test.base.decorators import requires_admin
 from ._framework import ApiTestCase
 
 TEST_KEYS_FOR_ALL_USERS = [
     "enable_unique_workflow_defaults",
     "ftp_upload_site",
     "wiki_url",
     "support_url",
@@ -18,25 +19,26 @@
     "library_import_dir",
     "user_library_import_dir",
     "allow_library_path_paste",
     "allow_user_deletion",
 ]
 
 
-class ConfigurationApiTestCase(ApiTestCase):
+class TestConfigurationApi(ApiTestCase):
     def test_whoami(self):
         response = self._get("whoami")
         self._assert_status_code_is(response, 200)
         assert response.json()["email"] == TEST_USER
 
     def test_normal_user_configuration(self):
         config = self._get_configuration()
         assert_has_keys(config, *TEST_KEYS_FOR_ALL_USERS)
         assert_not_has_keys(config, *TEST_KEYS_FOR_ADMIN_ONLY)
 
+    @requires_admin
     def test_admin_user_configuration(self):
         config = self._get_configuration(admin=True)
         assert_has_keys(config, *TEST_KEYS_FOR_ALL_USERS)
         assert_has_keys(config, *TEST_KEYS_FOR_ADMIN_ONLY)
 
     def test_normal_user_decode_id(self):
         decode_response = self._get("configuration/decode/badhombre", admin=False)
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_container_resolution.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_container_resolution.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+from galaxy_test.base.decorators import requires_admin
 from galaxy_test.base.populators import skip_without_tool
 from ._framework import ApiTestCase
 
 
-class ContainerResolutionApiTestCase(ApiTestCase):
+class TestContainerResolutionApi(ApiTestCase):
+    @requires_admin
     def test_index(self):
         response = self._get("container_resolvers", admin=True)
         assert response.status_code == 200
         assert isinstance(response.json(), list)
 
+    @requires_admin
     def test_show(self):
         response = self._get("container_resolvers/0", admin=True)
         assert response.status_code == 200
         assert isinstance(response.json(), dict)
 
     @skip_without_tool("cat1")
+    @requires_admin
     def test_resolve(self):
         tool_id = "cat1"
 
         # no index
         response = self._get(f"container_resolvers/resolve?tool_id={tool_id}", admin=True)
         assert response.status_code == 200
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_dataset_collections.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_dataset_collections.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,454 +1,493 @@
 import zipfile
 from io import BytesIO
 from typing import List
 
+from galaxy.util.unittest_utils import skip_if_github_down
 from galaxy_test.base.api_asserts import assert_object_id_error
 from galaxy_test.base.populators import (
     DatasetCollectionPopulator,
     DatasetPopulator,
-    skip_if_github_down,
 )
 from ._framework import ApiTestCase
 
 
-class DatasetCollectionApiTestCase(ApiTestCase):
-    history_id: str
+class TestDatasetCollectionsApi(ApiTestCase):
+    dataset_populator: DatasetPopulator
 
     def setUp(self):
         super().setUp()
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
         self.dataset_collection_populator = DatasetCollectionPopulator(self.galaxy_interactor)
-        self.history_id = self.dataset_populator.new_history()
 
     def test_create_pair_from_history(self):
-        payload = self.dataset_collection_populator.create_pair_payload(
-            self.history_id,
-            instance_type="history",
-        )
-        create_response = self.dataset_populator.fetch(payload, wait=True)
-        dataset_collection = self._check_create_response(create_response)
-        returned_datasets = dataset_collection["elements"]
-        assert len(returned_datasets) == 2, dataset_collection
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            payload = self.dataset_collection_populator.create_pair_payload(
+                history_id,
+                instance_type="history",
+            )
+            create_response = self.dataset_populator.fetch(payload, wait=True)
+            dataset_collection = self._check_create_response(create_response)
+            returned_datasets = dataset_collection["elements"]
+            assert len(returned_datasets) == 2, dataset_collection
 
     def test_create_list_from_history(self):
-        element_identifiers = self.dataset_collection_populator.list_identifiers(self.history_id)
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            element_identifiers = self.dataset_collection_populator.list_identifiers(history_id)
 
-        payload = dict(
-            instance_type="history",
-            history_id=self.history_id,
-            element_identifiers=element_identifiers,
-            collection_type="list",
-        )
+            payload = dict(
+                instance_type="history",
+                history_id=history_id,
+                element_identifiers=element_identifiers,
+                collection_type="list",
+            )
 
-        create_response = self._post("dataset_collections", payload, json=True)
-        dataset_collection = self._check_create_response(create_response)
-        returned_datasets = dataset_collection["elements"]
-        assert len(returned_datasets) == 3, dataset_collection
+            create_response = self._post("dataset_collections", payload, json=True)
+            dataset_collection = self._check_create_response(create_response)
+            returned_datasets = dataset_collection["elements"]
+            assert len(returned_datasets) == 3, dataset_collection
 
     def test_create_list_of_existing_pairs(self):
-        pair_payload = self.dataset_collection_populator.create_pair_payload(
-            self.history_id,
-            instance_type="history",
-        )
-        pair_create_response = self._post("tools/fetch", pair_payload, json=True)
-        dataset_collection = self._check_create_response(pair_create_response)
-        hdca_id = dataset_collection["id"]
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            pair_payload = self.dataset_collection_populator.create_pair_payload(
+                history_id,
+                instance_type="history",
+            )
+            pair_create_response = self._post("tools/fetch", pair_payload, json=True)
+            dataset_collection = self._check_create_response(pair_create_response)
+            hdca_id = dataset_collection["id"]
 
-        element_identifiers = [dict(name="test1", src="hdca", id=hdca_id)]
+            element_identifiers = [dict(name="test1", src="hdca", id=hdca_id)]
 
-        payload = dict(
-            instance_type="history",
-            history_id=self.history_id,
-            element_identifiers=element_identifiers,
-            collection_type="list",
-        )
-        create_response = self._post("dataset_collections", payload, json=True)
-        dataset_collection = self._check_create_response(create_response)
-        returned_collections = dataset_collection["elements"]
-        assert len(returned_collections) == 1, dataset_collection
+            payload = dict(
+                instance_type="history",
+                history_id=history_id,
+                element_identifiers=element_identifiers,
+                collection_type="list",
+            )
+            create_response = self._post("dataset_collections", payload, json=True)
+            dataset_collection = self._check_create_response(create_response)
+            returned_collections = dataset_collection["elements"]
+            assert len(returned_collections) == 1, dataset_collection
 
     def test_create_list_of_new_pairs(self):
-        identifiers = self.dataset_collection_populator.nested_collection_identifiers(self.history_id, "list:paired")
-        payload = dict(
-            collection_type="list:paired",
-            instance_type="history",
-            history_id=self.history_id,
-            name="a nested collection",
-            element_identifiers=identifiers,
-        )
-        create_response = self._post("dataset_collections", payload, json=True)
-        dataset_collection = self._check_create_response(create_response)
-        assert dataset_collection["collection_type"] == "list:paired"
-        assert dataset_collection["name"] == "a nested collection"
-        returned_collections = dataset_collection["elements"]
-        assert len(returned_collections) == 1, dataset_collection
-        pair_1_element = returned_collections[0]
-        self._assert_has_keys(pair_1_element, "element_identifier", "element_index", "object")
-        assert pair_1_element["element_identifier"] == "test_level_1", pair_1_element
-        assert pair_1_element["element_index"] == 0, pair_1_element
-        pair_1_object = pair_1_element["object"]
-        self._assert_has_keys(pair_1_object, "collection_type", "elements", "element_count")
-        self.assertEqual(pair_1_object["collection_type"], "paired")
-        self.assertEqual(pair_1_object["populated"], True)
-        pair_elements = pair_1_object["elements"]
-        assert len(pair_elements) == 2
-        pair_1_element_1 = pair_elements[0]
-        assert pair_1_element_1["element_index"] == 0
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            identifiers = self.dataset_collection_populator.nested_collection_identifiers(history_id, "list:paired")
+            payload = dict(
+                collection_type="list:paired",
+                instance_type="history",
+                history_id=history_id,
+                name="a nested collection",
+                element_identifiers=identifiers,
+            )
+            create_response = self._post("dataset_collections", payload, json=True)
+            dataset_collection = self._check_create_response(create_response)
+            assert dataset_collection["collection_type"] == "list:paired"
+            assert dataset_collection["name"] == "a nested collection"
+            returned_collections = dataset_collection["elements"]
+            assert len(returned_collections) == 1, dataset_collection
+            pair_1_element = returned_collections[0]
+            self._assert_has_keys(pair_1_element, "element_identifier", "element_index", "object")
+            assert pair_1_element["element_identifier"] == "test_level_1", pair_1_element
+            assert pair_1_element["element_index"] == 0, pair_1_element
+            pair_1_object = pair_1_element["object"]
+            self._assert_has_keys(pair_1_object, "collection_type", "elements", "element_count")
+            assert pair_1_object["collection_type"] == "paired"
+            assert pair_1_object["populated"] is True
+            pair_elements = pair_1_object["elements"]
+            assert len(pair_elements) == 2
+            pair_1_element_1 = pair_elements[0]
+            assert pair_1_element_1["element_index"] == 0
 
     def test_list_download(self):
-        fetch_response = self.dataset_collection_populator.create_list_in_history(
-            self.history_id, direct_upload=True
-        ).json()
-        dataset_collection = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)
-        returned_dce = dataset_collection["elements"]
-        assert len(returned_dce) == 3, dataset_collection
-        create_response = self._download_dataset_collection(
-            history_id=self.history_id, hdca_id=dataset_collection["id"]
-        )
-        self._assert_status_code_is(create_response, 200)
-        archive = zipfile.ZipFile(BytesIO(create_response.content))
-        namelist = archive.namelist()
-        assert len(namelist) == 3, f"Expected 3 elements in [{namelist}]"
-        collection_name = dataset_collection["name"]
-        for element, zip_path in zip(returned_dce, namelist):
-            assert f"{collection_name}/{element['element_identifier']}.{element['object']['file_ext']}" == zip_path
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            fetch_response = self.dataset_collection_populator.create_list_in_history(
+                history_id, direct_upload=True
+            ).json()
+            dataset_collection = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)
+            returned_dce = dataset_collection["elements"]
+            assert len(returned_dce) == 3, dataset_collection
+            create_response = self._download_dataset_collection(history_id=history_id, hdca_id=dataset_collection["id"])
+            self._assert_status_code_is(create_response, 200)
+            archive = zipfile.ZipFile(BytesIO(create_response.content))
+            namelist = archive.namelist()
+            assert len(namelist) == 3, f"Expected 3 elements in [{namelist}]"
+            collection_name = dataset_collection["name"]
+            for element, zip_path in zip(returned_dce, namelist):
+                assert f"{collection_name}/{element['element_identifier']}.{element['object']['file_ext']}" == zip_path
 
     def test_pair_download(self):
-        fetch_response = self.dataset_collection_populator.create_pair_in_history(
-            self.history_id, direct_upload=True
-        ).json()
-        dataset_collection = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)
-        returned_dce = dataset_collection["elements"]
-        assert len(returned_dce) == 2, dataset_collection
-        hdca_id = dataset_collection["id"]
-        create_response = self._download_dataset_collection(history_id=self.history_id, hdca_id=hdca_id)
-        self._assert_status_code_is(create_response, 200)
-        archive = zipfile.ZipFile(BytesIO(create_response.content))
-        namelist = archive.namelist()
-        assert len(namelist) == 2, f"Expected 2 elements in [{namelist}]"
-        collection_name = dataset_collection["name"]
-        for element, zip_path in zip(returned_dce, namelist):
-            assert f"{collection_name}/{element['element_identifier']}.{element['object']['file_ext']}" == zip_path
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            fetch_response = self.dataset_collection_populator.create_pair_in_history(
+                history_id, direct_upload=True
+            ).json()
+            dataset_collection = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)
+            returned_dce = dataset_collection["elements"]
+            assert len(returned_dce) == 2, dataset_collection
+            hdca_id = dataset_collection["id"]
+            create_response = self._download_dataset_collection(history_id=history_id, hdca_id=hdca_id)
+            self._assert_status_code_is(create_response, 200)
+            archive = zipfile.ZipFile(BytesIO(create_response.content))
+            namelist = archive.namelist()
+            assert len(namelist) == 2, f"Expected 2 elements in [{namelist}]"
+            collection_name = dataset_collection["name"]
+            for element, zip_path in zip(returned_dce, namelist):
+                assert f"{collection_name}/{element['element_identifier']}.{element['object']['file_ext']}" == zip_path
 
     def test_list_pair_download(self):
-        fetch_response = self.dataset_collection_populator.create_list_of_pairs_in_history(self.history_id).json()
-        dataset_collection = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)
-        returned_dce = dataset_collection["elements"]
-        assert len(returned_dce) == 1, dataset_collection
-        list_collection_name = dataset_collection["name"]
-        pair = returned_dce[0]
-        create_response = self._download_dataset_collection(
-            history_id=self.history_id, hdca_id=dataset_collection["id"]
-        )
-        self._assert_status_code_is(create_response, 200)
-        archive = zipfile.ZipFile(BytesIO(create_response.content))
-        namelist = archive.namelist()
-        assert len(namelist) == 2, f"Expected 2 elements in [{namelist}]"
-        pair_collection_name = pair["element_identifier"]
-        for element, zip_path in zip(pair["object"]["elements"], namelist):
-            assert (
-                f"{list_collection_name}/{pair_collection_name}/{element['element_identifier']}.{element['object']['file_ext']}"
-                == zip_path
-            )
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            fetch_response = self.dataset_collection_populator.create_list_of_pairs_in_history(history_id).json()
+            dataset_collection = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)
+            returned_dce = dataset_collection["elements"]
+            assert len(returned_dce) == 1, dataset_collection
+            list_collection_name = dataset_collection["name"]
+            pair = returned_dce[0]
+            create_response = self._download_dataset_collection(history_id=history_id, hdca_id=dataset_collection["id"])
+            self._assert_status_code_is(create_response, 200)
+            archive = zipfile.ZipFile(BytesIO(create_response.content))
+            namelist = archive.namelist()
+            assert len(namelist) == 2, f"Expected 2 elements in [{namelist}]"
+            pair_collection_name = pair["element_identifier"]
+            for element, zip_path in zip(pair["object"]["elements"], namelist):
+                assert (
+                    f"{list_collection_name}/{pair_collection_name}/{element['element_identifier']}.{element['object']['file_ext']}"
+                    == zip_path
+                )
 
     def test_list_list_download(self):
-        dataset_collection = self.dataset_collection_populator.create_list_of_list_in_history(
-            self.history_id, wait=True
-        ).json()
-        returned_dce = dataset_collection["elements"]
-        assert len(returned_dce) == 1, dataset_collection
-        create_response = self._download_dataset_collection(
-            history_id=self.history_id, hdca_id=dataset_collection["id"]
-        )
-        self._assert_status_code_is(create_response, 200)
-        archive = zipfile.ZipFile(BytesIO(create_response.content))
-        namelist = archive.namelist()
-        assert len(namelist) == 3, f"Expected 3 elements in [{namelist}]"
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            dataset_collection = self.dataset_collection_populator.create_list_of_list_in_history(
+                history_id, wait=True
+            ).json()
+            returned_dce = dataset_collection["elements"]
+            assert len(returned_dce) == 1, dataset_collection
+            create_response = self._download_dataset_collection(history_id=history_id, hdca_id=dataset_collection["id"])
+            self._assert_status_code_is(create_response, 200)
+            archive = zipfile.ZipFile(BytesIO(create_response.content))
+            namelist = archive.namelist()
+            assert len(namelist) == 3, f"Expected 3 elements in [{namelist}]"
 
     def test_list_list_list_download(self):
-        dataset_collection = self.dataset_collection_populator.create_list_of_list_in_history(
-            self.history_id,
-            collection_type="list:list:list",
-            wait=True,
-        ).json()
-        returned_dce = dataset_collection["elements"]
-        assert len(returned_dce) == 1, dataset_collection
-        create_response = self._download_dataset_collection(
-            history_id=self.history_id, hdca_id=dataset_collection["id"]
-        )
-        self._assert_status_code_is(create_response, 200)
-        archive = zipfile.ZipFile(BytesIO(create_response.content))
-        namelist = archive.namelist()
-        assert len(namelist) == 3, f"Expected 3 elements in [{namelist}]"
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            dataset_collection = self.dataset_collection_populator.create_list_of_list_in_history(
+                history_id,
+                collection_type="list:list:list",
+                wait=True,
+            ).json()
+            returned_dce = dataset_collection["elements"]
+            assert len(returned_dce) == 1, dataset_collection
+            create_response = self._download_dataset_collection(history_id=history_id, hdca_id=dataset_collection["id"])
+            self._assert_status_code_is(create_response, 200)
+            archive = zipfile.ZipFile(BytesIO(create_response.content))
+            namelist = archive.namelist()
+            assert len(namelist) == 3, f"Expected 3 elements in [{namelist}]"
 
     def test_hda_security(self):
-        element_identifiers = self.dataset_collection_populator.pair_identifiers(self.history_id)
-        self.dataset_populator.make_private(self.history_id, element_identifiers[0]["id"])
-        with self._different_user():
-            history_id = self.dataset_populator.new_history()
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            element_identifiers = self.dataset_collection_populator.pair_identifiers(history_id)
+            self.dataset_populator.make_private(history_id, element_identifiers[0]["id"])
+            with self._different_user():
+                history_id = self.dataset_populator.new_history()
+                payload = dict(
+                    instance_type="history",
+                    history_id=history_id,
+                    element_identifiers=element_identifiers,
+                    collection_type="paired",
+                )
+                create_response = self._post("dataset_collections", payload, json=True)
+                self._assert_status_code_is(create_response, 403)
+
+    def test_dataset_collection_element_security(self):
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            dataset_collection = self.dataset_collection_populator.create_list_of_list_in_history(
+                history_id,
+                collection_type="list:list:list",
+                wait=True,
+            ).json()
+            first_element = dataset_collection["elements"][0]
+            assert first_element["model_class"] == "DatasetCollectionElement"
+            assert first_element["element_type"] == "dataset_collection"
+            first_element_url = f"/api/dataset_collection_element/{first_element['id']}"
+            # Make one dataset private to check that access permissions are respected
+            first_dataset_element = first_element["object"]["elements"][0]["object"]["elements"][0]
+            self.dataset_populator.make_private(history_id, first_dataset_element["object"]["id"])
+            with self._different_user():
+                assert self._get(first_element_url).status_code == 403
+            collection_dce_response = self._get(first_element_url)
+            collection_dce_response.raise_for_status()
+            collection_dce = collection_dce_response.json()
+            assert collection_dce["model_class"] == "DatasetCollectionElement"
+            assert collection_dce["element_type"] == "dataset_collection"
+            first_dataset_element = first_element["object"]["elements"][0]["object"]["elements"][0]
+            assert first_dataset_element["model_class"] == "DatasetCollectionElement"
+            assert first_dataset_element["element_type"] == "hda"
+            first_dataset_element_url = f"/api/dataset_collection_element/{first_dataset_element['id']}"
+            with self._different_user():
+                assert self._get(first_dataset_element_url).status_code == 403
+            dataset_dce_response = self._get(first_dataset_element_url)
+            dataset_dce_response.raise_for_status()
+            dataset_dce = dataset_dce_response.json()
+            assert dataset_dce["model_class"] == "DatasetCollectionElement"
+            assert dataset_dce["element_type"] == "hda"
+            assert dataset_dce["object"]["model_class"] == "HistoryDatasetAssociation"
+
+    def test_enforces_unique_names(self):
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            element_identifiers = self.dataset_collection_populator.list_identifiers(history_id)
+            element_identifiers[2]["name"] = element_identifiers[0]["name"]
             payload = dict(
                 instance_type="history",
                 history_id=history_id,
                 element_identifiers=element_identifiers,
-                collection_type="paired",
+                collection_type="list",
             )
-            create_response = self._post("dataset_collections", payload, json=True)
-            self._assert_status_code_is(create_response, 403)
-
-    def test_enforces_unique_names(self):
-        element_identifiers = self.dataset_collection_populator.list_identifiers(self.history_id)
-        element_identifiers[2]["name"] = element_identifiers[0]["name"]
-        payload = dict(
-            instance_type="history",
-            history_id=self.history_id,
-            element_identifiers=element_identifiers,
-            collection_type="list",
-        )
 
-        create_response = self._post("dataset_collections", payload, json=True)
-        self._assert_status_code_is(create_response, 400)
+            create_response = self._post("dataset_collections", payload, json=True)
+            self._assert_status_code_is(create_response, 400)
 
     def test_upload_collection(self):
-        elements = [
-            {
-                "src": "files",
-                "dbkey": "hg19",
-                "info": "my cool bed",
-                "tags": ["name:data1", "group:condition:treated", "machine:illumina"],
-            }
-        ]
-        targets = [
-            {
-                "destination": {"type": "hdca"},
-                "elements": elements,
-                "collection_type": "list",
-                "name": "Test upload",
-                "tags": ["name:collection1"],
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            elements = [
+                {
+                    "src": "files",
+                    "dbkey": "hg19",
+                    "info": "my cool bed",
+                    "tags": ["name:data1", "group:condition:treated", "machine:illumina"],
+                }
+            ]
+            targets = [
+                {
+                    "destination": {"type": "hdca"},
+                    "elements": elements,
+                    "collection_type": "list",
+                    "name": "Test upload",
+                    "tags": ["name:collection1"],
+                }
+            ]
+            payload = {
+                "history_id": history_id,
+                "targets": targets,
+                "__files": {"files_0|file_data": open(self.test_data_resolver.get_filename("4.bed"))},
             }
-        ]
-        payload = {
-            "history_id": self.history_id,
-            "targets": targets,
-            "__files": {"files_0|file_data": open(self.test_data_resolver.get_filename("4.bed"))},
-        }
-        self.dataset_populator.fetch(payload)
-        hdca = self._assert_one_collection_created_in_history()
-        self.assertEqual(hdca["name"], "Test upload")
-        hdca_tags = hdca["tags"]
-        assert len(hdca_tags) == 1
-        assert "name:collection1" in hdca_tags
-        assert len(hdca["elements"]) == 1, hdca
-        element0 = hdca["elements"][0]
-        assert element0["element_identifier"] == "4.bed"
-        dataset0 = element0["object"]
-        assert dataset0["file_size"] == 61
-        dataset_tags = dataset0["tags"]
-        assert len(dataset_tags) == 3, dataset0
+            self.dataset_populator.fetch(payload)
+            hdca = self._assert_one_collection_created_in_history(history_id)
+            assert hdca["name"] == "Test upload"
+            hdca_tags = hdca["tags"]
+            assert len(hdca_tags) == 1
+            assert "name:collection1" in hdca_tags
+            assert len(hdca["elements"]) == 1, hdca
+            element0 = hdca["elements"][0]
+            assert element0["element_identifier"] == "4.bed"
+            dataset0 = element0["object"]
+            assert dataset0["file_size"] == 61
+            dataset_tags = dataset0["tags"]
+            assert len(dataset_tags) == 3, dataset0
 
     def test_upload_nested(self):
-        elements = [{"name": "samp1", "elements": [{"src": "files", "dbkey": "hg19", "info": "my cool bed"}]}]
-        targets = [
-            {
-                "destination": {"type": "hdca"},
-                "elements": elements,
-                "collection_type": "list:list",
-                "name": "Test upload",
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            elements = [{"name": "samp1", "elements": [{"src": "files", "dbkey": "hg19", "info": "my cool bed"}]}]
+            targets = [
+                {
+                    "destination": {"type": "hdca"},
+                    "elements": elements,
+                    "collection_type": "list:list",
+                    "name": "Test upload",
+                }
+            ]
+            payload = {
+                "history_id": history_id,
+                "targets": targets,
+                "__files": {"files_0|file_data": open(self.test_data_resolver.get_filename("4.bed"))},
             }
-        ]
-        payload = {
-            "history_id": self.history_id,
-            "targets": targets,
-            "__files": {"files_0|file_data": open(self.test_data_resolver.get_filename("4.bed"))},
-        }
-        self.dataset_populator.fetch(payload)
-        hdca = self._assert_one_collection_created_in_history()
-        self.assertEqual(hdca["name"], "Test upload")
-        assert len(hdca["elements"]) == 1, hdca
-        element0 = hdca["elements"][0]
-        assert element0["element_identifier"] == "samp1"
+            self.dataset_populator.fetch(payload)
+            hdca = self._assert_one_collection_created_in_history(history_id)
+            assert hdca["name"] == "Test upload"
+            assert len(hdca["elements"]) == 1, hdca
+            element0 = hdca["elements"][0]
+            assert element0["element_identifier"] == "samp1"
 
     @skip_if_github_down
     def test_upload_collection_from_url(self):
-        elements = [
-            {
-                "src": "url",
-                "url": "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/4.bed",
-                "info": "my cool bed",
-            }
-        ]
-        targets = [
-            {
-                "destination": {"type": "hdca"},
-                "elements": elements,
-                "collection_type": "list",
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            elements = [
+                {
+                    "src": "url",
+                    "url": "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/4.bed",
+                    "info": "my cool bed",
+                }
+            ]
+            targets = [
+                {
+                    "destination": {"type": "hdca"},
+                    "elements": elements,
+                    "collection_type": "list",
+                }
+            ]
+            payload = {
+                "history_id": history_id,
+                "targets": targets,
             }
-        ]
-        payload = {
-            "history_id": self.history_id,
-            "targets": targets,
-        }
-        self.dataset_populator.fetch(payload)
-        hdca = self._assert_one_collection_created_in_history()
-        assert len(hdca["elements"]) == 1, hdca
-        element0 = hdca["elements"][0]
-        assert element0["element_identifier"] == "4.bed"
-        assert element0["object"]["file_size"] == 61
+            self.dataset_populator.fetch(payload)
+            hdca = self._assert_one_collection_created_in_history(history_id)
+            assert len(hdca["elements"]) == 1, hdca
+            element0 = hdca["elements"][0]
+            assert element0["element_identifier"] == "4.bed"
+            assert element0["object"]["file_size"] == 61
 
     def test_upload_collection_deferred(self):
-        elements = [
-            {
-                "src": "url",
-                "url": "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/4.bed",
-                "info": "my cool bed",
-                "deferred": True,
-            }
-        ]
-        targets = [
-            {
-                "destination": {"type": "hdca"},
-                "elements": elements,
-                "collection_type": "list",
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            elements = [
+                {
+                    "src": "url",
+                    "url": "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/4.bed",
+                    "info": "my cool bed",
+                    "deferred": True,
+                }
+            ]
+            targets = [
+                {
+                    "destination": {"type": "hdca"},
+                    "elements": elements,
+                    "collection_type": "list",
+                }
+            ]
+            payload = {
+                "history_id": history_id,
+                "targets": targets,
             }
-        ]
-        payload = {
-            "history_id": self.history_id,
-            "targets": targets,
-        }
-        self.dataset_populator.fetch(payload)
-        hdca = self._assert_one_collection_created_in_history()
-        assert len(hdca["elements"]) == 1, hdca
-        element0 = hdca["elements"][0]
-        assert element0["element_identifier"] == "4.bed"
-        object0 = element0["object"]
-        assert object0["state"] == "deferred"
+            self.dataset_populator.fetch(payload)
+            hdca = self._assert_one_collection_created_in_history(history_id)
+            assert len(hdca["elements"]) == 1, hdca
+            element0 = hdca["elements"][0]
+            assert element0["element_identifier"] == "4.bed"
+            object0 = element0["object"]
+            assert object0["state"] == "deferred"
 
     @skip_if_github_down
     def test_upload_collection_failed_expansion_url(self):
-        targets = [
-            {
-                "destination": {"type": "hdca"},
-                "elements_from": "bagit",
-                "collection_type": "list",
-                "src": "url",
-                "url": "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/4.bed",
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            targets = [
+                {
+                    "destination": {"type": "hdca"},
+                    "elements_from": "bagit",
+                    "collection_type": "list",
+                    "src": "url",
+                    "url": "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/4.bed",
+                }
+            ]
+            payload = {
+                "history_id": history_id,
+                "targets": targets,
             }
-        ]
-        payload = {
-            "history_id": self.history_id,
-            "targets": targets,
-        }
-        self.dataset_populator.fetch(payload, assert_ok=False, wait=True)
-        hdca = self._assert_one_collection_created_in_history()
-        assert hdca["populated"] is False
-        assert "bagit.txt" in hdca["populated_state_message"], hdca
+            self.dataset_populator.fetch(payload, assert_ok=False, wait=True)
+            hdca = self._assert_one_collection_created_in_history(history_id)
+            assert hdca["populated"] is False
+            assert "bagit.txt" in hdca["populated_state_message"], hdca
 
-    def _assert_one_collection_created_in_history(self):
-        contents_response = self._get(f"histories/{self.history_id}/contents/dataset_collections")
+    def _assert_one_collection_created_in_history(self, history_id: str):
+        contents_response = self._get(f"histories/{history_id}/contents/dataset_collections")
         self._assert_status_code_is(contents_response, 200)
         contents = contents_response.json()
         assert len(contents) == 1
         hdca = contents[0]
         assert hdca["history_content_type"] == "dataset_collection"
         hdca_id = hdca["id"]
-        collection_response = self._get(f"histories/{self.history_id}/contents/dataset_collections/{hdca_id}")
+        collection_response = self._get(f"histories/{history_id}/contents/dataset_collections/{hdca_id}")
         self._assert_status_code_is(collection_response, 200)
         return collection_response.json()
 
     def _check_create_response(self, create_response):
         self._assert_status_code_is(create_response, 200)
         dataset_collection = create_response.json()
         if "output_collections" in dataset_collection:
             # fetch data response, we'll have to check the final response
             dataset_collection = dataset_collection["output_collections"][0]
             dataset_collection = self._get(f"dataset_collections/{dataset_collection['id']}").json()
         self._assert_has_keys(dataset_collection, "elements", "url", "name", "collection_type", "element_count")
         return dataset_collection
 
-    def _download_dataset_collection(self, history_id, hdca_id):
+    def _download_dataset_collection(self, history_id: str, hdca_id: str):
         return self._get(f"histories/{history_id}/contents/dataset_collections/{hdca_id}/download")
 
-    def test_collection_contents_security(self):
+    def test_collection_contents_security(self, history_id):
         # request contents on an hdca that doesn't belong to user
-        hdca, contents_url = self._create_collection_contents_pair()
+        hdca, contents_url = self._create_collection_contents_pair(history_id)
         with self._different_user():
             contents_response = self._get(contents_url)
             self._assert_status_code_is(contents_response, 403)
 
-    def test_collection_contents_invalid_collection(self):
+    def test_collection_contents_invalid_collection(self, history_id):
         # request an invalid collection from a valid hdca, should get 404
-        hdca, contents_url = self._create_collection_contents_pair()
+        hdca, contents_url = self._create_collection_contents_pair(history_id)
         response = self._get(contents_url)
         self._assert_status_code_is(response, 200)
         fake_collection_id = "5d7db0757a2eb7ef"
         fake_contents_url = f"/api/dataset_collections/{hdca['id']}/contents/{fake_collection_id}"
         error_response = self._get(fake_contents_url)
         assert_object_id_error(error_response)
 
-    def test_show_dataset_collection(self):
-        fetch_response = self.dataset_collection_populator.create_list_in_history(
-            self.history_id, direct_upload=True
-        ).json()
+    def test_show_dataset_collection(self, history_id):
+        fetch_response = self.dataset_collection_populator.create_list_in_history(history_id, direct_upload=True).json()
         dataset_collection = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)
         returned_dce = dataset_collection["elements"]
         assert len(returned_dce) == 3, dataset_collection
         hdca_id = dataset_collection["id"]
         dataset_collection_url = f"/api/dataset_collections/{hdca_id}"
         dataset_collection = self._get(dataset_collection_url).json()
         assert dataset_collection["id"] == hdca_id
         assert dataset_collection["collection_type"] == "list"
 
-    def test_show_dataset_collection_contents(self):
+    def test_show_dataset_collection_contents(self, history_id):
         # Get contents_url from history contents, use it to show the first level
         # of collection contents in the created HDCA, then use it again to drill
         # down into the nested collection contents
-        hdca = self.dataset_collection_populator.create_list_of_list_in_history(self.history_id).json()
-        root_contents_url = self._get_contents_url_for_hdca(hdca)
+        hdca = self.dataset_collection_populator.create_list_of_list_in_history(history_id).json()
+        root_contents_url = self._get_contents_url_for_hdca(history_id, hdca)
 
         # check root contents for this collection
         root_contents = self._get(root_contents_url).json()
         assert len(root_contents) == len(hdca["elements"])
         self._compare_collection_contents_elements(root_contents, hdca["elements"])
 
         # drill down, retrieve nested collection contents
         assert "object" in root_contents[0]
         assert "contents_url" in root_contents[0]["object"]
         drill_contents_url = root_contents[0]["object"]["contents_url"]
         drill_contents = self._get(drill_contents_url).json()
         assert len(drill_contents) == len(hdca["elements"][0]["object"]["elements"])
         self._compare_collection_contents_elements(drill_contents, hdca["elements"][0]["object"]["elements"])
 
-    def test_collection_contents_limit_offset(self):
+    def test_collection_contents_limit_offset(self, history_id):
         # check limit/offset params for collection contents endpoint
-        hdca, root_contents_url = self._create_collection_contents_pair()
+        hdca, root_contents_url = self._create_collection_contents_pair(history_id)
 
         # check limit
         limited_contents = self._get(f"{root_contents_url}?limit=1").json()
         assert len(limited_contents) == 1
         assert limited_contents[0]["element_index"] == 0
 
         # check offset
         offset_contents = self._get(f"{root_contents_url}?offset=1").json()
         assert len(offset_contents) == 1
         assert offset_contents[0]["element_index"] == 1
 
-    def test_collection_contents_empty_root(self):
+    def test_collection_contents_empty_root(self, history_id):
         create_response = self.dataset_collection_populator.create_list_in_history(
-            self.history_id, contents=[], wait=True
+            history_id, contents=[], wait=True
         ).json()
         hdca = create_response["output_collections"][0]
         assert hdca["elements"] == []
         root_contents_url = hdca["contents_url"]
         response = self._get(root_contents_url)
         response.raise_for_status()
         assert response.json() == []
 
-    def test_get_suitable_converters_single_datatype(self):
+    def test_get_suitable_converters_single_datatype(self, history_id):
         response = self.dataset_collection_populator.upload_collection(
-            self.history_id,
+            history_id,
             "list:paired",
             elements=[
                 {
                     "name": "test0",
                     "elements": [
                         {"src": "pasted", "paste_content": "123\n", "name": "forward", "ext": "bed"},
                         {"src": "pasted", "paste_content": "456\n", "name": "reverse", "ext": "bed"},
@@ -482,17 +521,17 @@
         for converter in converters.json():
             actual.append(converter["tool_id"])
         missing_expected_converters = set(expected) - set(actual)
         assert (
             not missing_expected_converters
         ), f"Expected converter(s) {', '.join(missing_expected_converters)} missing from response"
 
-    def test_get_suitable_converters_different_datatypes_matches(self):
+    def test_get_suitable_converters_different_datatypes_matches(self, history_id):
         response = self.dataset_collection_populator.upload_collection(
-            self.history_id,
+            history_id,
             "list:paired",
             elements=[
                 {
                     "name": "test0",
                     "elements": [
                         {"src": "pasted", "paste_content": "123\n", "name": "forward", "ext": "bed"},
                         {"src": "pasted", "paste_content": "456\n", "name": "reverse", "ext": "bed"},
@@ -513,17 +552,17 @@
         converters = self._get("dataset_collections/" + hdca_list_id + "/suitable_converters")
         expected = "tabular_to_csv"
         actual = []
         for converter in converters.json():
             actual.append(converter["tool_id"])
         assert expected in actual
 
-    def test_get_suitable_converters_different_datatypes_no_matches(self):
+    def test_get_suitable_converters_different_datatypes_no_matches(self, history_id):
         response = self.dataset_collection_populator.upload_collection(
-            self.history_id,
+            history_id,
             "list:paired",
             elements=[
                 {
                     "name": "test0",
                     "elements": [
                         {"src": "pasted", "paste_content": "123\n", "name": "forward", "ext": "bed"},
                         {"src": "pasted", "paste_content": "456\n", "name": "reverse", "ext": "bed"},
@@ -543,67 +582,67 @@
         hdca_list_id = response.json()["outputs"][0]["id"]
         converters = self._get("dataset_collections/" + hdca_list_id + "/suitable_converters")
         actual: List[str] = []
         for converter in converters.json():
             actual.append(converter["tool_id"])
         assert actual == []
 
-    def test_collection_tools_tag_propagation(self):
+    def test_collection_tools_tag_propagation(self, history_id):
         elements = [{"src": "files", "tags": ["name:element_tag"]}]
         targets = [
             {
                 "destination": {"type": "hdca"},
                 "elements": elements,
                 "collection_type": "list",
                 "name": "Test collection",
                 "tags": ["name:collection_tag"],
             }
         ]
         payload = {
-            "history_id": self.history_id,
+            "history_id": history_id,
             "targets": targets,
             "__files": {"files_0|file_data": open(self.test_data_resolver.get_filename("4.bed"))},
         }
         hdca_id = self.dataset_populator.fetch(payload).json()["output_collections"][0]["id"]
         inputs = {
             "input": {"batch": False, "src": "hdca", "id": hdca_id},
         }
         payload = self.dataset_populator.run_tool_payload(
             tool_id="__FILTER_FAILED_DATASETS__",
             inputs=inputs,
-            history_id=self.history_id,
+            history_id=history_id,
             input_format="legacy",
         )
         response = self._post("tools", payload).json()
-        self.dataset_populator.wait_for_history(self.history_id, assert_ok=False)
+        self.dataset_populator.wait_for_history(history_id, assert_ok=False)
         output_collection = response["output_collections"][0]
         # collection should not inherit tags from input collection elements, only parent collection
         assert output_collection["tags"] == ["name:collection_tag"]
         element = output_collection["elements"][0]
         # new element hda should have tags copied from old hda
         assert element["object"]["tags"] == ["name:element_tag"]
 
     def _compare_collection_contents_elements(self, contents_elements, hdca_elements):
         # compare collection api results to existing hdca element contents
         fields = ["element_identifier", "element_index", "element_type", "id", "model_class"]
-        for (content_element, hdca_element) in zip(contents_elements, hdca_elements):
+        for content_element, hdca_element in zip(contents_elements, hdca_elements):
             for f in fields:
                 assert content_element[f] == hdca_element[f]
 
-    def _create_collection_contents_pair(self):
+    def _create_collection_contents_pair(self, history_id: str):
         # Create a simple collection, return hdca and contents_url
-        payload = self.dataset_collection_populator.create_pair_payload(self.history_id, instance_type="history")
+        payload = self.dataset_collection_populator.create_pair_payload(history_id, instance_type="history")
         create_response = self.dataset_populator.fetch(payload=payload, wait=True)
         hdca = self._check_create_response(create_response)
-        root_contents_url = self._get_contents_url_for_hdca(hdca)
+        root_contents_url = self._get_contents_url_for_hdca(history_id, hdca)
         return hdca, root_contents_url
 
-    def _get_contents_url_for_hdca(self, hdca):
+    def _get_contents_url_for_hdca(self, history_id: str, hdca):
         # look up the history contents using optional serialization key
-        history_contents_url = f"histories/{self.history_id}/contents?v=dev&view=summary&keys=contents_url"
+        history_contents_url = f"histories/{history_id}/contents?v=dev&view=summary&keys=contents_url"
         json = self._get(history_contents_url).json()
 
         # filter out the collection we just made id = hdca.id
         # make sure the contents_url appears
         def find_hdca(c):
             return c["history_content_type"] == "dataset_collection" and c["id"] == hdca["id"]
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_datasets.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_datasets.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,64 @@
 )
 
 from galaxy.model.unittest_utils.store_fixtures import (
     deferred_hda_model_store_dict,
     one_hda_model_store_dict,
     TEST_SOURCE_URI,
 )
+from galaxy.util.unittest_utils import skip_if_github_down
 from galaxy_test.base.api_asserts import assert_has_keys
+from galaxy_test.base.decorators import (
+    requires_admin,
+    requires_new_history,
+)
 from galaxy_test.base.populators import (
     DatasetCollectionPopulator,
     DatasetPopulator,
-    skip_if_github_down,
     skip_without_datatype,
     skip_without_tool,
 )
 from ._framework import ApiTestCase
 
+COMPOSITE_DATA_FETCH_REQUEST_1 = {
+    "src": "composite",
+    "ext": "velvet",
+    "composite": {
+        "items": [
+            {"src": "pasted", "paste_content": "sequences content"},
+            {"src": "pasted", "paste_content": "roadmaps content"},
+            {"src": "pasted", "paste_content": "log content"},
+        ]
+    },
+}
+
 
-class DatasetsApiTestCase(ApiTestCase):
-    history_id: str
+class TestDatasetsApi(ApiTestCase):
+    dataset_populator: DatasetPopulator
 
     def setUp(self):
         super().setUp()
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
         self.dataset_collection_populator = DatasetCollectionPopulator(self.galaxy_interactor)
-        self.history_id = self.dataset_populator.new_history()
 
     def test_index(self):
         index_response = self._get("datasets")
         self._assert_status_code_is(index_response, 200)
 
-    def test_index_using_keys(self):
+    def test_index_using_keys(self, history_id):
         expected_keys = "id"
-        self.dataset_populator.new_dataset(self.history_id)
+        self.dataset_populator.new_dataset(history_id)
         index_response = self._get(f"datasets?keys={expected_keys}")
         self._assert_status_code_is(index_response, 200)
         datasets = index_response.json()
         for dataset in datasets:
             assert len(dataset) == 1
             self._assert_has_keys(dataset, "id")
 
+    @requires_new_history
     def test_index_order_by_size(self):
         num_datasets = 3
         history_id = self.dataset_populator.new_history()
         dataset_ids_ordered_by_size_asc = []
         for index in range(num_datasets):
             dataset_content = (index + 1) * "content"
             hda = self.dataset_populator.new_dataset(history_id, content=dataset_content)
@@ -67,229 +83,239 @@
         datasets_response = self._get(f"histories/{history_id}/contents?v=dev&keys=size&order={order_by}")
         self._assert_status_code_is(datasets_response, 200)
         datasets = datasets_response.json()
         assert len(datasets) == len(expected_ids_order)
         for index, dataset in enumerate(datasets):
             assert dataset["id"] == expected_ids_order[index]
 
+    @requires_new_history
     def test_search_datasets(self):
-        hda_id = self.dataset_populator.new_dataset(self.history_id)["id"]
-        payload = {"limit": 1, "offset": 0, "history_id": self.history_id}
-        index_response = self._get("datasets", payload).json()
-        assert len(index_response) == 1
-        assert index_response[0]["id"] == hda_id
-        fetch_response = self.dataset_collection_populator.create_list_in_history(
-            self.history_id, contents=["1\n2\n3"]
-        ).json()
-        hdca_id = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)["id"]
-        index_payload_1 = {"limit": 3, "offset": 0, "order": "hid", "history_id": self.history_id}
-        index_response = self._get("datasets", index_payload_1).json()
-        assert len(index_response) == 3
-        assert index_response[0]["hid"] == 3
-        assert index_response[1]["hid"] == 2
-        assert index_response[2]["hid"] == 1
-        assert index_response[2]["history_content_type"] == "dataset"
-        assert index_response[2]["id"] == hda_id
-        assert index_response[1]["history_content_type"] == "dataset_collection"
-        assert index_response[1]["id"] == hdca_id
-        index_payload_2 = {"limit": 2, "offset": 0, "q": ["history_content_type"], "qv": ["dataset"]}
-        index_response = self._get("datasets", index_payload_2).json()
-        assert index_response[1]["id"] == hda_id
+        with self.dataset_populator.test_history_for(self.test_search_datasets) as history_id:
+            hda_id = self.dataset_populator.new_dataset(history_id)["id"]
+            payload = {"limit": 1, "offset": 0, "history_id": history_id}
+            index_response = self._get("datasets", payload).json()
+            assert len(index_response) == 1
+            assert index_response[0]["id"] == hda_id
+            fetch_response = self.dataset_collection_populator.create_list_in_history(
+                history_id, contents=["1\n2\n3"]
+            ).json()
+            hdca_id = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)["id"]
+            index_payload_1 = {"limit": 3, "offset": 0, "order": "hid", "history_id": history_id}
+            index_response = self._get("datasets", index_payload_1).json()
+            assert len(index_response) == 3
+            assert index_response[0]["hid"] == 3
+            assert index_response[1]["hid"] == 2
+            assert index_response[2]["hid"] == 1
+            assert index_response[2]["history_content_type"] == "dataset"
+            assert index_response[2]["id"] == hda_id
+            assert index_response[1]["history_content_type"] == "dataset_collection"
+            assert index_response[1]["id"] == hdca_id
+            index_payload_2 = {"limit": 2, "offset": 0, "q": ["history_content_type"], "qv": ["dataset"]}
+            index_response = self._get("datasets", index_payload_2).json()
+            assert index_response[1]["id"] == hda_id
 
+    @requires_new_history
     def test_search_by_tag(self):
-        hda_id = self.dataset_populator.new_dataset(self.history_id)["id"]
-        update_payload = {
-            "tags": ["cool:new_tag", "cool:another_tag"],
-        }
-        updated_hda = self._put(f"histories/{self.history_id}/contents/{hda_id}", update_payload, json=True).json()
-        assert "cool:new_tag" in updated_hda["tags"]
-        assert "cool:another_tag" in updated_hda["tags"]
-        payload = {
-            "limit": 10,
-            "offset": 0,
-            "q": ["history_content_type", "tag"],
-            "qv": ["dataset", "cool:new_tag"],
-            "history_id": self.history_id,
-        }
-        index_response = self._get("datasets", payload).json()
-        assert len(index_response) == 1
-        payload = {
-            "limit": 10,
-            "offset": 0,
-            "q": ["history_content_type", "tag-contains"],
-            "qv": ["dataset", "new_tag"],
-            "history_id": self.history_id,
-        }
-        index_response = self._get("datasets", payload).json()
-        assert len(index_response) == 1
-        payload = {
-            "limit": 10,
-            "offset": 0,
-            "q": ["history_content_type", "tag-contains"],
-            "qv": ["dataset", "notag"],
-            "history_id": self.history_id,
-        }
-        index_response = self._get("datasets", payload).json()
-        assert len(index_response) == 0
+        with self.dataset_populator.test_history_for(self.test_search_by_tag) as history_id:
+            hda_id = self.dataset_populator.new_dataset(history_id)["id"]
+            update_payload = {
+                "tags": ["cool:new_tag", "cool:another_tag"],
+            }
+            updated_hda = self._put(f"histories/{history_id}/contents/{hda_id}", update_payload, json=True).json()
+            assert "cool:new_tag" in updated_hda["tags"]
+            assert "cool:another_tag" in updated_hda["tags"]
+            payload = {
+                "limit": 10,
+                "offset": 0,
+                "q": ["history_content_type", "tag"],
+                "qv": ["dataset", "cool:new_tag"],
+                "history_id": history_id,
+            }
+            index_response = self._get("datasets", payload).json()
+            assert len(index_response) == 1
+            payload = {
+                "limit": 10,
+                "offset": 0,
+                "q": ["history_content_type", "tag-contains"],
+                "qv": ["dataset", "new_tag"],
+                "history_id": history_id,
+            }
+            index_response = self._get("datasets", payload).json()
+            assert len(index_response) == 1
+            payload = {
+                "limit": 10,
+                "offset": 0,
+                "q": ["history_content_type", "tag-contains"],
+                "qv": ["dataset", "notag"],
+                "history_id": history_id,
+            }
+            index_response = self._get("datasets", payload).json()
+            assert len(index_response) == 0
 
+    @requires_new_history
     def test_search_by_tag_case_insensitive(self):
-        history_id = self.dataset_populator.new_history()
-        hda_id = self.dataset_populator.new_dataset(history_id)["id"]
-        update_payload = {
-            "tags": ["name:new_TAG", "cool:another_TAG"],
-        }
-        updated_hda = self._put(f"histories/{history_id}/contents/{hda_id}", update_payload, json=True).json()
-        assert "name:new_TAG" in updated_hda["tags"]
-        assert "cool:another_TAG" in updated_hda["tags"]
-        payload = {
-            "limit": 10,
-            "offset": 0,
-            "q": ["history_content_type", "tag"],
-            "qv": ["dataset", "name:new_tag"],
-            "history_id": history_id,
-        }
-        index_response = self._get("datasets", payload).json()
-        assert len(index_response) == 1
-        payload = {
-            "limit": 10,
-            "offset": 0,
-            "q": ["history_content_type", "tag-contains"],
-            "qv": ["dataset", "new_tag"],
-            "history_id": history_id,
-        }
-        index_response = self._get("datasets", payload).json()
-        assert len(index_response) == 1
-        payload = {
-            "limit": 10,
-            "offset": 0,
-            "q": ["history_content_type", "tag-contains"],
-            "qv": ["dataset", "notag"],
-            "history_id": history_id,
-        }
-        index_response = self._get("datasets", payload).json()
-        assert len(index_response) == 0
+        with self.dataset_populator.test_history_for(self.test_search_by_tag_case_insensitive) as history_id:
+            hda_id = self.dataset_populator.new_dataset(history_id)["id"]
+            update_payload = {
+                "tags": ["name:new_TAG", "cool:another_TAG"],
+            }
+            updated_hda = self._put(f"histories/{history_id}/contents/{hda_id}", update_payload, json=True).json()
+            assert "name:new_TAG" in updated_hda["tags"]
+            assert "cool:another_TAG" in updated_hda["tags"]
+            payload = {
+                "limit": 10,
+                "offset": 0,
+                "q": ["history_content_type", "tag"],
+                "qv": ["dataset", "name:new_tag"],
+                "history_id": history_id,
+            }
+            index_response = self._get("datasets", payload).json()
+            assert len(index_response) == 1
+            payload = {
+                "limit": 10,
+                "offset": 0,
+                "q": ["history_content_type", "tag-contains"],
+                "qv": ["dataset", "new_tag"],
+                "history_id": history_id,
+            }
+            index_response = self._get("datasets", payload).json()
+            assert len(index_response) == 1
+            payload = {
+                "limit": 10,
+                "offset": 0,
+                "q": ["history_content_type", "tag-contains"],
+                "qv": ["dataset", "notag"],
+                "history_id": history_id,
+            }
+            index_response = self._get("datasets", payload).json()
+            assert len(index_response) == 0
 
+    @requires_new_history
     def test_search_by_tool_id(self):
-        self.dataset_populator.new_dataset(self.history_id)
-        payload = {
-            "limit": 1,
-            "offset": 0,
-            "q": ["history_content_type", "tool_id"],
-            "qv": ["dataset", "__DATA_FETCH__"],
-            "history_id": self.history_id,
-        }
-        assert len(self._get("datasets", payload).json()) == 1
-        payload = {
-            "limit": 1,
-            "offset": 0,
-            "q": ["history_content_type", "tool_id"],
-            "qv": ["dataset", "__DATA_FETCH__X"],
-            "history_id": self.history_id,
-        }
-        assert len(self._get("datasets", payload).json()) == 0
-        payload = {
-            "limit": 1,
-            "offset": 0,
-            "q": ["history_content_type", "tool_id-contains"],
-            "qv": ["dataset", "ATA_FETCH"],
-            "history_id": self.history_id,
-        }
-        assert len(self._get("datasets", payload).json()) == 1
-        self.dataset_collection_populator.create_list_in_history(
-            self.history_id, name="search by tool id", contents=["1\n2\n3"], wait=True
-        )
-        payload = {
-            "limit": 10,
-            "offset": 0,
-            "q": ["name", "tool_id"],
-            "qv": ["search by tool id", "__DATA_FETCH__"],
-            "history_id": self.history_id,
-        }
-        result = self._get("datasets", payload).json()
-        assert result[0]["name"] == "search by tool id", result
-        payload = {
-            "limit": 1,
-            "offset": 0,
-            "q": ["history_content_type", "tool_id"],
-            "qv": ["dataset_collection", "uploadX"],
-            "history_id": self.history_id,
-        }
-        result = self._get("datasets", payload).json()
-        assert len(result) == 0
+        with self.dataset_populator.test_history_for(self.test_search_by_tool_id) as history_id:
+            self.dataset_populator.new_dataset(history_id)
+            payload = {
+                "limit": 1,
+                "offset": 0,
+                "q": ["history_content_type", "tool_id"],
+                "qv": ["dataset", "__DATA_FETCH__"],
+                "history_id": history_id,
+            }
+            assert len(self._get("datasets", payload).json()) == 1
+            payload = {
+                "limit": 1,
+                "offset": 0,
+                "q": ["history_content_type", "tool_id"],
+                "qv": ["dataset", "__DATA_FETCH__X"],
+                "history_id": history_id,
+            }
+            assert len(self._get("datasets", payload).json()) == 0
+            payload = {
+                "limit": 1,
+                "offset": 0,
+                "q": ["history_content_type", "tool_id-contains"],
+                "qv": ["dataset", "ATA_FETCH"],
+                "history_id": history_id,
+            }
+            assert len(self._get("datasets", payload).json()) == 1
+            self.dataset_collection_populator.create_list_in_history(
+                history_id, name="search by tool id", contents=["1\n2\n3"], wait=True
+            )
+            payload = {
+                "limit": 10,
+                "offset": 0,
+                "q": ["name", "tool_id"],
+                "qv": ["search by tool id", "__DATA_FETCH__"],
+                "history_id": history_id,
+            }
+            result = self._get("datasets", payload).json()
+            assert result[0]["name"] == "search by tool id", result
+            payload = {
+                "limit": 1,
+                "offset": 0,
+                "q": ["history_content_type", "tool_id"],
+                "qv": ["dataset_collection", "uploadX"],
+                "history_id": history_id,
+            }
+            result = self._get("datasets", payload).json()
+            assert len(result) == 0
 
+    @requires_new_history
     def test_search_by_extension(self):
-        self.dataset_populator.new_dataset(self.history_id, wait=True)
-        payload = {
-            "q": ["extension"],
-            "qv": ["txt"],
-            "history_id": self.history_id,
-        }
-        assert len(self._get("datasets", payload).json()) == 1
-        payload = {
-            "q": ["extension"],
-            "qv": ["bam"],
-            "history_id": self.history_id,
-        }
-        assert len(self._get("datasets", payload).json()) == 0
-        payload = {
-            "q": ["extension-in"],
-            "qv": ["bam,txt"],
-            "history_id": self.history_id,
-        }
-        assert len(self._get("datasets", payload).json()) == 1
-        payload = {
-            "q": ["extension-like"],
-            "qv": ["t%t"],
-            "history_id": self.history_id,
-        }
-        assert len(self._get("datasets", payload).json()) == 1
-        payload = {
-            "q": ["extension-like"],
-            "qv": ["b%m"],
-            "history_id": self.history_id,
-        }
-        assert len(self._get("datasets", payload).json()) == 0
+        with self.dataset_populator.test_history_for(self.test_search_by_extension) as history_id:
+            self.dataset_populator.new_dataset(history_id, wait=True)
+            payload = {
+                "q": ["extension"],
+                "qv": ["txt"],
+                "history_id": history_id,
+            }
+            assert len(self._get("datasets", payload).json()) == 1
+            payload = {
+                "q": ["extension"],
+                "qv": ["bam"],
+                "history_id": history_id,
+            }
+            assert len(self._get("datasets", payload).json()) == 0
+            payload = {
+                "q": ["extension-in"],
+                "qv": ["bam,txt"],
+                "history_id": history_id,
+            }
+            assert len(self._get("datasets", payload).json()) == 1
+            payload = {
+                "q": ["extension-like"],
+                "qv": ["t%t"],
+                "history_id": history_id,
+            }
+            assert len(self._get("datasets", payload).json()) == 1
+            payload = {
+                "q": ["extension-like"],
+                "qv": ["b%m"],
+                "history_id": history_id,
+            }
+            assert len(self._get("datasets", payload).json()) == 0
 
     def test_invalid_search(self):
         payload = {
             "limit": 10,
             "offset": 0,
             "q": ["history_content_type", "tag-invalid_op"],
             "qv": ["dataset", "notag"],
         }
         index_response = self._get("datasets", payload)
         self._assert_status_code_is(index_response, 400)
         assert index_response.json()["err_msg"] == "bad op in filter"
 
-    def test_search_returns_only_accessible(self):
-        hda_id = self.dataset_populator.new_dataset(self.history_id)["id"]
+    def test_search_returns_only_accessible(self, history_id):
+        hda_id = self.dataset_populator.new_dataset(history_id)["id"]
         with self._different_user():
             payload = {"limit": 10, "offset": 0, "q": ["history_content_type"], "qv": ["dataset"]}
             index_response = self._get("datasets", payload).json()
             for item in index_response:
                 assert hda_id != item["id"]
 
-    def test_show(self):
-        hda1 = self.dataset_populator.new_dataset(self.history_id)
+    def test_show(self, history_id):
+        hda1 = self.dataset_populator.new_dataset(history_id)
         show_response = self._get(f"datasets/{hda1['id']}")
         self._assert_status_code_is(show_response, 200)
         self.__assert_matches_hda(hda1, show_response.json())
 
-    def test_show_permission_denied(self):
-        hda = self.dataset_populator.new_dataset(self.history_id)
-        self.dataset_populator.make_private(history_id=self.history_id, dataset_id=hda["id"])
+    def test_show_permission_denied(self, history_id):
+        hda = self.dataset_populator.new_dataset(history_id)
+        self.dataset_populator.make_private(history_id=history_id, dataset_id=hda["id"])
         with self._different_user():
             show_response = self._get(f"datasets/{hda['id']}")
             self._assert_status_code_is(show_response, 403)
 
-    def test_admin_can_update_permissions(self):
+    @requires_admin
+    def test_admin_can_update_permissions(self, history_id):
         # Create private dataset
-        hda = self.dataset_populator.new_dataset(self.history_id)
+        hda = self.dataset_populator.new_dataset(history_id)
         dataset_id = hda["id"]
-        self.dataset_populator.make_private(history_id=self.history_id, dataset_id=dataset_id)
+        self.dataset_populator.make_private(history_id=history_id, dataset_id=dataset_id)
 
         # Admin removes restrictions
         payload = {"action": "remove_restrictions"}
         update_response = self._put(f"datasets/{dataset_id}/permissions", payload, admin=True, json=True)
         self._assert_status_code_is_ok(update_response)
 
         # Other users can access the dataset
@@ -298,40 +324,38 @@
             self._assert_status_code_is_ok(show_response)
 
     def __assert_matches_hda(self, input_hda, query_hda):
         self._assert_has_keys(query_hda, "id", "name")
         assert input_hda["name"] == query_hda["name"]
         assert input_hda["id"] == query_hda["id"]
 
-    def test_display(self):
+    def test_display(self, history_id):
         contents = textwrap.dedent(
             """\
         1   2   3   4
         A   B   C   D
         10  20  30  40
         """
         )
-        hda1 = self.dataset_populator.new_dataset(self.history_id, content=contents, wait=True)
-        display_response = self._get(f"histories/{self.history_id}/contents/{hda1['id']}/display", {"raw": "True"})
+        hda1 = self.dataset_populator.new_dataset(history_id, content=contents, wait=True)
+        display_response = self._get(f"histories/{history_id}/contents/{hda1['id']}/display", {"raw": "True"})
         self._assert_status_code_is(display_response, 200)
         assert display_response.text == contents
 
-    def test_head(self):
-        history_id = self.history_id
+    def test_head(self, history_id):
         hda1 = self.dataset_populator.new_dataset(history_id, wait=True)
         display_response = self._head(f"histories/{history_id}/contents/{hda1['id']}/display", {"raw": "True"})
         self._assert_status_code_is(display_response, 200)
         assert display_response.text == ""
         display_response = self._head(
             f"histories/{history_id}/contents/{hda1['id']}{hda1['id']}/display", {"raw": "True"}
         )
         self._assert_status_code_is(display_response, 400)
 
-    def test_byte_range_support(self):
-        history_id = self.history_id
+    def test_byte_range_support(self, history_id):
         hda1 = self.dataset_populator.new_dataset(history_id, wait=True)
         head_response = self._head(f"histories/{history_id}/contents/{hda1['id']}/display", {"raw": "True"})
         self._assert_status_code_is(head_response, 200)
         assert head_response.headers["content-length"] == "12"
         assert head_response.text == ""
         assert head_response.headers["accept-ranges"] == "bytes"
         valid_headers = {"range": "bytes=0-0"}
@@ -344,95 +368,95 @@
         assert display_response.headers["content-range"] == "bytes 0-0/12"
         invalid_headers = {"range": "bytes=-1-1"}
         display_response = self._get(
             f"histories/{history_id}/contents/{hda1['id']}/display", {"raw": "True"}, headers=invalid_headers
         )
         self._assert_status_code_is(display_response, 416)
 
-    def test_tag_change(self):
-        hda_id = self.dataset_populator.new_dataset(self.history_id)["id"]
+    def test_tag_change(self, history_id):
+        hda_id = self.dataset_populator.new_dataset(history_id)["id"]
         payload = {
             "item_id": hda_id,
             "item_class": "HistoryDatasetAssociation",
             "item_tags": ["cool:tag_a", "cool:tag_b", "tag_c", "name:tag_d", "#tag_e"],
         }
 
         put_response = self._put("tags", data=payload, json=True)
         self._assert_status_code_is_ok(put_response)
-        updated_hda = self._get(f"histories/{self.history_id}/contents/{hda_id}").json()
+        updated_hda = self._get(f"histories/{history_id}/contents/{hda_id}").json()
         assert "cool:tag_a" in updated_hda["tags"]
         assert "cool:tag_b" in updated_hda["tags"]
         assert "tag_c" in updated_hda["tags"]
         assert "name:tag_d" in updated_hda["tags"]
         assert "name:tag_e" in updated_hda["tags"]
 
     @skip_without_tool("cat_data_and_sleep")
-    def test_update_datatype(self):
-        hda_id = self.dataset_populator.new_dataset(self.history_id)["id"]
-        original_hda = self._get(f"histories/{self.history_id}/contents/{hda_id}").json()
+    def test_update_datatype(self, history_id):
+        hda_id = self.dataset_populator.new_dataset(history_id)["id"]
+        original_hda = self._get(f"histories/{history_id}/contents/{hda_id}").json()
         assert original_hda["extension"] == "txt"
         assert original_hda["data_type"] == "galaxy.datatypes.data.Text"
 
         inputs = {
             "input1": {"src": "hda", "id": hda_id},
             "sleep_time": 10,
         }
         run_response = self.dataset_populator.run_tool_raw(
             "cat_data_and_sleep",
             inputs,
-            self.history_id,
+            history_id,
         )
         queued_id = run_response.json()["outputs"][0]["id"]
 
         update_while_incomplete_response = self._put(  # try updating datatype while used as output of a running job
-            f"histories/{self.history_id}/contents/{queued_id}", data={"datatype": "tabular"}, json=True
+            f"histories/{history_id}/contents/{queued_id}", data={"datatype": "tabular"}, json=True
         )
         self._assert_status_code_is(update_while_incomplete_response, 400)
 
-        self.dataset_populator.wait_for_history_jobs(self.history_id)  # now wait for upload to complete
+        self.dataset_populator.wait_for_history_jobs(history_id)  # now wait for upload to complete
 
         successful_updated_hda_response = self._put(
-            f"histories/{self.history_id}/contents/{hda_id}", data={"datatype": "tabular"}, json=True
+            f"histories/{history_id}/contents/{hda_id}", data={"datatype": "tabular"}, json=True
         ).json()
         assert successful_updated_hda_response["extension"] == "tabular"
         assert successful_updated_hda_response["data_type"] == "galaxy.datatypes.tabular.Tabular"
 
         invalidly_updated_hda_response = self._put(  # try updating with invalid datatype
-            f"histories/{self.history_id}/contents/{hda_id}", data={"datatype": "invalid"}, json=True
+            f"histories/{history_id}/contents/{hda_id}", data={"datatype": "invalid"}, json=True
         )
         self._assert_status_code_is(invalidly_updated_hda_response, 400)
 
     @skip_without_tool("cat_data_and_sleep")
-    def test_delete_cancels_job(self):
-        self._run_cancel_job(use_query_params=False)
+    def test_delete_cancels_job(self, history_id):
+        self._run_cancel_job(history_id, use_query_params=False)
 
     @skip_without_tool("cat_data_and_sleep")
-    def test_delete_cancels_job_with_query_params(self):
-        self._run_cancel_job(use_query_params=True)
+    def test_delete_cancels_job_with_query_params(self, history_id):
+        self._run_cancel_job(history_id, use_query_params=True)
 
-    def _run_cancel_job(self, use_query_params=False):
-        hda_id = self.dataset_populator.new_dataset(self.history_id)["id"]
+    def _run_cancel_job(self, history_id: str, use_query_params: bool = False):
+        hda_id = self.dataset_populator.new_dataset(history_id)["id"]
         inputs = {
             "input1": {"src": "hda", "id": hda_id},
             "sleep_time": 10,
         }
         run_response = self.dataset_populator.run_tool_raw(
             "cat_data_and_sleep",
             inputs,
-            self.history_id,
+            history_id,
         ).json()
         output_hda_id = run_response["outputs"][0]["id"]
         job_id = run_response["jobs"][0]["id"]
 
         job_details = self.dataset_populator.get_job_details(job_id).json()
         assert job_details["state"] in ("new", "queued", "running"), job_details
 
         # Use stop_job to cancel the creating job
         delete_response = self.dataset_populator.delete_dataset(
-            self.history_id, output_hda_id, stop_job=True, use_query_params=use_query_params
+            history_id, output_hda_id, stop_job=True, use_query_params=use_query_params
         )
         self._assert_status_code_is_ok(delete_response)
         deleted_hda = delete_response.json()
         assert deleted_hda["deleted"], deleted_hda
 
         # The job should be cancelled
         deleted_job_details = self.dataset_populator.get_job_details(job_id).json()
@@ -442,14 +466,16 @@
         num_datasets = 4
         dataset_map: Dict[int, str] = {}
         history_id = self.dataset_populator.new_history()
         for index in range(num_datasets):
             hda = self.dataset_populator.new_dataset(history_id)
             dataset_map[index] = hda["id"]
 
+        self.dataset_populator.wait_for_history(history_id)
+
         expected_deleted_source_ids = [
             {"id": dataset_map[1], "src": "hda"},
             {"id": dataset_map[2], "src": "hda"},
         ]
         delete_payload = {"datasets": expected_deleted_source_ids}
         deleted_result = self._delete_batch_with_payload(delete_payload)
 
@@ -508,76 +534,145 @@
     def _delete_batch_with_payload(self, payload):
         delete_response = self._delete("datasets", data=payload, json=True)
         self._assert_status_code_is_ok(delete_response)
         deleted_result = delete_response.json()
         return deleted_result
 
     @skip_without_datatype("velvet")
-    def test_composite_datatype_download(self):
-        item = {
-            "src": "composite",
-            "ext": "velvet",
-            "composite": {
-                "items": [
-                    {"src": "pasted", "paste_content": "sequences content"},
-                    {"src": "pasted", "paste_content": "roadmaps content"},
-                    {"src": "pasted", "paste_content": "log content"},
-                ]
-            },
-        }
-        output = self.dataset_populator.fetch_hda(self.history_id, item, wait=True)
-        print(output)
-        response = self._get(f"histories/{self.history_id}/contents/{output['id']}/display?to_ext=zip")
+    def test_composite_datatype_download(self, history_id):
+        output = self.dataset_populator.fetch_hda(history_id, COMPOSITE_DATA_FETCH_REQUEST_1, wait=True)
+        response = self._get(f"histories/{history_id}/contents/{output['id']}/display?to_ext=zip")
         self._assert_status_code_is(response, 200)
         archive = zipfile.ZipFile(BytesIO(response.content))
         namelist = archive.namelist()
         assert len(namelist) == 4, f"Expected 3 elements in [{namelist}]"
 
-    def test_storage_show(self):
-        hda = self.dataset_populator.new_dataset(self.history_id, wait=True)
-        hda_details = self.dataset_populator.get_history_dataset_details(self.history_id, dataset=hda)
+    def test_compute_md5_on_primary_dataset(self, history_id):
+        hda = self.dataset_populator.new_dataset(history_id, wait=True)
+        hda_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=hda)
+        assert "hashes" in hda_details, str(hda_details.keys())
+        hashes = hda_details["hashes"]
+        assert len(hashes) == 0
+
+        self.dataset_populator.compute_hash(hda["id"])
+        hda_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=hda)
+        self.assert_hash_value(hda_details, "940cbe15c94d7e339dc15550f6bdcf4d", "MD5")
+
+    def test_compute_sha1_on_composite_dataset(self, history_id):
+        output = self.dataset_populator.fetch_hda(history_id, COMPOSITE_DATA_FETCH_REQUEST_1, wait=True)
+        hda_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=output)
+        assert "hashes" in hda_details, str(hda_details.keys())
+        hashes = hda_details["hashes"]
+        assert len(hashes) == 0
+
+        self.dataset_populator.compute_hash(hda_details["id"], hash_function="SHA-256", extra_files_path="Roadmaps")
+        hda_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=output)
+        self.assert_hash_value(
+            hda_details,
+            "3cbd311889963528954fe03b28b68a09685ea7a75660bd2268d5b44cafbe0d22",
+            "SHA-256",
+            extra_files_path="Roadmaps",
+        )
+
+    def test_duplicated_hash_requests_on_primary(self, history_id):
+        hda = self.dataset_populator.new_dataset(history_id, wait=True)
+        hda_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=hda)
+        assert "hashes" in hda_details, str(hda_details.keys())
+        hashes = hda_details["hashes"]
+        assert len(hashes) == 0
+
+        self.dataset_populator.compute_hash(hda["id"])
+        self.dataset_populator.compute_hash(hda["id"])
+        hda_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=hda)
+        self.assert_hash_value(hda_details, "940cbe15c94d7e339dc15550f6bdcf4d", "MD5")
+
+    def test_duplicated_hash_requests_on_extra_files(self, history_id):
+        output = self.dataset_populator.fetch_hda(history_id, COMPOSITE_DATA_FETCH_REQUEST_1, wait=True)
+        hda_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=output)
+        assert "hashes" in hda_details, str(hda_details.keys())
+        hashes = hda_details["hashes"]
+        assert len(hashes) == 0
+
+        # 4 unique requests, but make them twice...
+        for _ in range(2):
+            self.dataset_populator.compute_hash(hda_details["id"], hash_function="SHA-256", extra_files_path="Roadmaps")
+            self.dataset_populator.compute_hash(hda_details["id"], hash_function="SHA-1", extra_files_path="Roadmaps")
+            self.dataset_populator.compute_hash(hda_details["id"], hash_function="MD5", extra_files_path="Roadmaps")
+            self.dataset_populator.compute_hash(
+                hda_details["id"], hash_function="SHA-256", extra_files_path="Sequences"
+            )
+
+        hda_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=output)
+        self.assert_hash_value(hda_details, "ce0c0ef1073317ff96c896c249b002dc", "MD5", extra_files_path="Roadmaps")
+        self.assert_hash_value(
+            hda_details, "fe2e06cdd03922a1ddf3fe6c7e0d299c8044fc8e", "SHA-1", extra_files_path="Roadmaps"
+        )
+        self.assert_hash_value(
+            hda_details,
+            "3cbd311889963528954fe03b28b68a09685ea7a75660bd2268d5b44cafbe0d22",
+            "SHA-256",
+            extra_files_path="Roadmaps",
+        )
+        self.assert_hash_value(
+            hda_details,
+            "4688dca47fe3214516c35acd284a79d97bd6df2bc1c55981b556d995495b91b6",
+            "SHA-256",
+            extra_files_path="Sequences",
+        )
+
+    def assert_hash_value(self, dataset_details, expected_hash_value, hash_function, extra_files_path=None):
+        assert "hashes" in dataset_details, str(dataset_details.keys())
+        hashes = dataset_details["hashes"]
+        matching_hashes = [
+            h for h in hashes if h["extra_files_path"] == extra_files_path and h["hash_function"] == hash_function
+        ]
+        assert len(matching_hashes) == 1
+        hash_value = matching_hashes[0]["hash_value"]
+        assert expected_hash_value == hash_value
+
+    def test_storage_show(self, history_id):
+        hda = self.dataset_populator.new_dataset(history_id, wait=True)
+        hda_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=hda)
         dataset_id = hda_details["dataset_id"]
         storage_info_dict = self.dataset_populator.dataset_storage_info(dataset_id)
         assert_has_keys(storage_info_dict, "object_store_id", "name", "description")
 
-    def test_storage_show_on_discarded(self):
+    def test_storage_show_on_discarded(self, history_id):
         as_list = self.dataset_populator.create_contents_from_store(
-            self.history_id,
+            history_id,
             store_dict=one_hda_model_store_dict(),
         )
         assert len(as_list) == 1
         hda_id = as_list[0]["id"]
         storage_info_dict = self.dataset_populator.dataset_storage_info(hda_id)
         assert_has_keys(storage_info_dict, "object_store_id", "name", "description", "sources", "hashes")
 
         assert storage_info_dict["object_store_id"] is None
         sources = storage_info_dict["sources"]
         assert len(sources) == 1
         assert sources[0]["source_uri"] == TEST_SOURCE_URI
 
-    def test_storage_show_on_deferred(self):
+    def test_storage_show_on_deferred(self, history_id):
         as_list = self.dataset_populator.create_contents_from_store(
-            self.history_id,
+            history_id,
             store_dict=deferred_hda_model_store_dict(),
         )
         assert len(as_list) == 1
         hda_id = as_list[0]["id"]
         storage_info_dict = self.dataset_populator.dataset_storage_info(hda_id)
         assert_has_keys(storage_info_dict, "object_store_id", "name", "description", "sources", "hashes")
 
         assert storage_info_dict["object_store_id"] is None
         sources = storage_info_dict["sources"]
         assert len(sources) == 1
         assert sources[0]["source_uri"] == TEST_SOURCE_URI
 
     @skip_if_github_down
-    def test_display_application_link(self):
+    def test_display_application_link(self, history_id):
         item = {
             "src": "url",
             "url": "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/1.bam",
             "ext": "bam",
         }
-        output = self.dataset_populator.fetch_hda(self.history_id, item)
-        dataset_details = self.dataset_populator.get_history_dataset_details(
-            self.history_id, dataset=output, assert_ok=True
-        )
+        output = self.dataset_populator.fetch_hda(history_id, item)
+        dataset_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=output, assert_ok=True)
         assert "display_application/" in dataset_details["display_apps"][0]["links"][0]["href"]
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_datatypes.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_datatypes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import time
 
 from requests import put
 
+from galaxy_test.base.decorators import requires_admin
 from ._framework import ApiTestCase
 
 HIDDEN_DURING_UPLOAD_DATATYPE = "fli"
 
 
-class DatatypesApiTestCase(ApiTestCase):
+class TestDatatypesApi(ApiTestCase):
     def test_index(self):
         datatypes = self._index_datatypes()
         for common_type in ["tabular", "fasta"]:
             assert common_type in datatypes, f"{common_type} not in {datatypes}"
 
     def test_index_upload_only(self):
         # fli is not displayed in upload - so only show it if upload_only
@@ -66,14 +67,15 @@
         for converter in converters_list:
             self._assert_has_key(converter, "source", "target", "tool_id")
             if converter["source"] == "fasta" and converter["target"] == "tabular":
                 found_fasta_to_tabular = True
 
         assert found_fasta_to_tabular
 
+    @requires_admin
     def test_converter_present_after_toolbox_reload(self):
         response = self._get("tools", data={"tool_id": "CONVERTER_fasta_to_tabular"})
         self._assert_status_code_is(response, 200)
         converters = len(response.json())
         assert converters == 1
         url = self._api_url("configuration/toolbox")
         put_response = put(url, params=dict(key=self.master_api_key))
@@ -85,21 +87,34 @@
 
     def test_edam_formats(self):
         response = self._get("datatypes/edam_formats")
         self._assert_status_code_is(response, 200)
         edam_formats = response.json()
         assert isinstance(edam_formats, dict)
         assert edam_formats["ab1"] == "format_3000"
+        response = self._get("datatypes/edam_formats/detailed")
+        self._assert_status_code_is(response, 200)
+        edam_formats = response.json()
+        assert isinstance(edam_formats, dict)
+        assert isinstance(edam_formats["afg"], dict)
+        assert edam_formats["afg"]["prefix_IRI"] == "format_3582"
+        assert edam_formats["afg"]["label"] == "afg"
 
     def test_edam_data(self):
         response = self._get("datatypes/edam_data")
         self._assert_status_code_is(response, 200)
         edam_data = response.json()
         assert isinstance(edam_data, dict)
         assert edam_data["ab1"] == "data_0924"
+        response = self._get("datatypes/edam_data/detailed")
+        edam_data = response.json()
+        assert isinstance(edam_data, dict)
+        assert isinstance(edam_data["afg"], dict)
+        assert edam_data["afg"]["prefix_IRI"] == "data_0925"
+        assert edam_data["afg"]["label"] == "Sequence assembly"
 
     def _index_datatypes(self, data=None):
         data = data or {}
         response = self._get("datatypes", data=data)
         self._assert_status_code_is(response, 200)
         datatypes = response.json()
         assert isinstance(datatypes, list)
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_display_applications.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_display_applications.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 import random
 from typing import List
 
+from galaxy_test.base.decorators import requires_admin
 from ._framework import ApiTestCase
 
 
-class DisplayApplicationsApiTestCase(ApiTestCase):
+class TestDisplayApplicationsApi(ApiTestCase):
     def test_index(self):
         response = self._get("display_applications")
         self._assert_status_code_is(response, 200)
         as_list = response.json()
         assert isinstance(as_list, list)
         assert len(as_list) > 0
         for display_app in as_list:
             self._assert_has_keys(display_app, "id", "name", "version", "filename_", "links")
 
+    @requires_admin
     def test_reload_as_admin(self):
         response = self._post("display_applications/reload", admin=True)
         self._assert_status_code_is(response, 200)
 
+    @requires_admin
     def test_reload_with_some_ids(self):
         response = self._get("display_applications")
         self._assert_status_code_is(response, 200)
         display_apps = response.json()
         all_ids = [display_app["id"] for display_app in display_apps]
         input_ids = self._get_half_random_items(all_ids)
         payload = {"ids": input_ids}
         response = self._post("display_applications/reload", payload, admin=True)
         self._assert_status_code_is(response, 200)
         reloaded = response.json()["reloaded"]
         assert len(reloaded) == len(input_ids)
         assert all(elem in reloaded for elem in input_ids)
 
-    def test_reload_unknow_returns_as_failed(self):
+    @requires_admin
+    def test_reload_unknown_returns_as_failed(self):
         unknown_id = "unknown"
         payload = {"ids": [unknown_id]}
         response = self._post("display_applications/reload", payload, admin=True)
         self._assert_status_code_is(response, 200)
         reloaded = response.json()["reloaded"]
         failed = response.json()["failed"]
         assert len(reloaded) == 0
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_framework.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_framework.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file doesn't test any API in particular but is meant to functionally
 # test the API framework itself.
+from galaxy_test.base.decorators import requires_admin
 from ._framework import ApiTestCase
 
 
-class ApiFrameworkTestCase(ApiTestCase):
+class TestApiFramework(ApiTestCase):
     def test_default_xframe_options(self):
         get_response = self._get("licenses")
         assert get_response.headers["x-frame-options"] == "SAMEORIGIN"
 
     # Next several tests test the API's run_as functionality.
     def test_user_cannont_run_as(self):
         run_as_user = self._setup_user("for_run_as@bx.psu.edu")
@@ -16,25 +17,27 @@
         create_response = self._post(
             "histories",
             data=post_data,
             headers={"run-as": run_as_user["id"]},
         )
         self._assert_status_code_is(create_response, 403)
 
+    @requires_admin
     def test_run_as_invalid_user(self):
         post_data = dict(name="TestHistory1")
         # admin user can run_as, but this user doesn't exist, expect 400.
         create_response = self._post(
             "histories",
             data=post_data,
             headers={"run-as": "another_user"},
             admin=True,
         )
         self._assert_status_code_is(create_response, 400)
 
+    @requires_admin
     def test_run_as_valid_user(self):
         run_as_user = self._setup_user("for_run_as@bx.psu.edu")
         post_data = dict(name="TestHistory1")
         # Use run_as with admin user and for another user just created, this
         # should work.
         create_response = self._post(
             "histories",
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_group_roles.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_group_roles.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 from typing import (
     List,
     Optional,
 )
 
+from galaxy_test.api._framework import ApiTestCase
+from galaxy_test.base.decorators import (
+    requires_admin,
+    using_requirement,
+)
 from galaxy_test.base.populators import DatasetPopulator
-from ._framework import ApiTestCase
 
 
-class GroupRolesApiTestCase(ApiTestCase):
+class TestGroupRolesApi(ApiTestCase):
+    dataset_populator: DatasetPopulator
+
     def setUp(self):
         super().setUp()
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
 
+    @requires_admin
     def test_index(self, group_name: Optional[str] = None):
         group_name = group_name or "test-group_roles"
         group = self._create_group(group_name)
         encoded_group_id = group["id"]
 
         group_roles = self._get_group_roles(encoded_group_id)
 
@@ -25,41 +32,45 @@
             self._assert_valid_group_role(group_role)
 
     def test_index_only_admin(self):
         encoded_group_id = "any-group-id"
         response = self._get(f"groups/{encoded_group_id}/roles")
         self._assert_status_code_is(response, 403)
 
+    @requires_admin
     def test_index_unknown_group_raises_400(self):
         encoded_group_id = "unknown-group-id"
         response = self._get(f"groups/{encoded_group_id}/roles", admin=True)
         self._assert_status_code_is(response, 400)
 
+    @requires_admin
     def test_show(self):
         encoded_role_id = self.dataset_populator.user_private_role_id()
         group = self._create_group("test-group-show-role", encoded_role_ids=[encoded_role_id])
         encoded_group_id = group["id"]
         response = self._get(f"groups/{encoded_group_id}/roles/{encoded_role_id}", admin=True)
         self._assert_status_code_is(response, 200)
         group_role = response.json()
-        self._assert_valid_group_role(group_role)
+        self._assert_valid_group_role(group_role, assert_id=encoded_role_id)
 
     def test_show_only_admin(self):
         encoded_group_id = "any-group-id"
         encoded_role_id = "any-role-id"
         response = self._get(f"groups/{encoded_group_id}/roles/{encoded_role_id}")
         self._assert_status_code_is(response, 403)
 
+    @requires_admin
     def test_show_unknown_raises_400(self):
         group = self._create_group("test-group-with-unknown-role")
         encoded_group_id = group["id"]
         encoded_role_id = "unknown-role-id"
         response = self._get(f"groups/{encoded_group_id}/roles/{encoded_role_id}", admin=True)
         self._assert_status_code_is(response, 400)
 
+    @requires_admin
     def test_update(self):
         group_name = "group-without-roles"
         group = self._create_group(group_name, encoded_role_ids=[])
         encoded_group_id = group["id"]
 
         group_roles = self._get_group_roles(encoded_group_id)
         assert len(group_roles) == 0
@@ -67,20 +78,22 @@
         encoded_role_id = self.dataset_populator.user_private_role_id()
         update_response = self._put(f"groups/{encoded_group_id}/roles/{encoded_role_id}", admin=True)
         self._assert_status_code_is_ok(update_response)
         group_role = update_response.json()
         self._assert_valid_group_role(group_role, assert_id=encoded_role_id)
         assert group_role["url"] == f"/api/groups/{encoded_group_id}/roles/{encoded_role_id}"
 
+    @requires_admin
     def test_update_only_admin(self):
         encoded_group_id = "any-group-id"
         encoded_role_id = "any-role-id"
         response = self._put(f"groups/{encoded_group_id}/roles/{encoded_role_id}")
         self._assert_status_code_is(response, 403)
 
+    @requires_admin
     def test_delete(self):
         group_name = "group-with-role-to-delete"
         encoded_role_id = self.dataset_populator.user_private_role_id()
         group = self._create_group(group_name, encoded_role_ids=[encoded_role_id])
         encoded_group_id = group["id"]
 
         group_roles = self._get_group_roles(encoded_group_id)
@@ -96,14 +109,15 @@
 
     def test_delete_only_admin(self):
         encoded_group_id = "any-group-id"
         encoded_role_id = "any-role-id"
         response = self._delete(f"groups/{encoded_group_id}/roles/{encoded_role_id}")
         self._assert_status_code_is(response, 403)
 
+    @requires_admin
     def test_delete_unknown_raises_400(self):
         group_name = "group-without-role-to-delete"
         group = self._create_group(group_name, encoded_role_ids=[])
         encoded_group_id = group["id"]
 
         group_roles = self._get_group_roles(encoded_group_id)
         assert len(group_roles) == 0
@@ -116,20 +130,22 @@
         if encoded_role_ids is None:
             encoded_role_ids = [self.dataset_populator.user_private_role_id()]
         role_ids = encoded_role_ids
         payload = {
             "name": group_name,
             "role_ids": role_ids,
         }
+        using_requirement("admin")
         response = self._post("groups", payload, admin=True, json=True)
         self._assert_status_code_is(response, 200)
         group = response.json()[0]  # POST /api/groups returns a list
         return group
 
     def _get_group_roles(self, encoded_group_id: str):
+        using_requirement("admin")
         response = self._get(f"groups/{encoded_group_id}/roles", admin=True)
         self._assert_status_code_is(response, 200)
         group_roles = response.json()
         return group_roles
 
     def _assert_valid_group_role(self, role, assert_id=None):
         self._assert_has_keys(role, "id", "name", "url")
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_group_users.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_group_users.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 from typing import (
     List,
     Optional,
 )
 
+from galaxy_test.api._framework import ApiTestCase
+from galaxy_test.base.decorators import (
+    requires_admin,
+    using_requirement,
+)
 from galaxy_test.base.populators import DatasetPopulator
-from ._framework import ApiTestCase
 
 
-class GroupUsersApiTestCase(ApiTestCase):
+class TestGroupUsersApi(ApiTestCase):
+    dataset_populator: DatasetPopulator
+
     def setUp(self):
         super().setUp()
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
 
+    @requires_admin
     def test_index(self, group_name: Optional[str] = None):
         group_name = group_name or "test-group_users"
         group = self._create_group(group_name)
         encoded_group_id = group["id"]
 
         group_users = self._get_group_users(encoded_group_id)
 
@@ -25,41 +32,45 @@
             self._assert_valid_group_user(group_user)
 
     def test_index_only_admin(self):
         encoded_group_id = "any-group-id"
         response = self._get(f"groups/{encoded_group_id}/users")
         self._assert_status_code_is(response, 403)
 
+    @requires_admin
     def test_index_unknown_group_raises_400(self):
         encoded_group_id = "unknown-group-id"
         response = self._get(f"groups/{encoded_group_id}/users", admin=True)
         self._assert_status_code_is(response, 400)
 
+    @requires_admin
     def test_show(self):
         encoded_user_id = self.dataset_populator.user_id()
         group = self._create_group("test-group-show-user", encoded_user_ids=[encoded_user_id])
         encoded_group_id = group["id"]
         response = self._get(f"groups/{encoded_group_id}/users/{encoded_user_id}", admin=True)
         self._assert_status_code_is(response, 200)
         group_user = response.json()
-        self._assert_valid_group_user(group_user)
+        self._assert_valid_group_user(group_user, assert_id=encoded_user_id)
 
     def test_show_only_admin(self):
         encoded_group_id = "any-group-id"
         encoded_user_id = "any-user-id"
         response = self._get(f"groups/{encoded_group_id}/users/{encoded_user_id}")
         self._assert_status_code_is(response, 403)
 
+    @requires_admin
     def test_show_unknown_raises_400(self):
         group = self._create_group("test-group-with-unknown-user")
         encoded_group_id = group["id"]
         encoded_user_id = "unknown-user-id"
         response = self._get(f"groups/{encoded_group_id}/users/{encoded_user_id}", admin=True)
         self._assert_status_code_is(response, 400)
 
+    @requires_admin
     def test_update(self):
         group_name = "group-without-users"
         group = self._create_group(group_name, encoded_user_ids=[])
         encoded_group_id = group["id"]
 
         group_users = self._get_group_users(encoded_group_id)
         assert len(group_users) == 0
@@ -73,14 +84,15 @@
 
     def test_update_only_admin(self):
         encoded_group_id = "any-group-id"
         encoded_user_id = "any-user-id"
         response = self._put(f"groups/{encoded_group_id}/users/{encoded_user_id}")
         self._assert_status_code_is(response, 403)
 
+    @requires_admin
     def test_delete(self):
         group_name = "group-with-user-to-delete"
         encoded_user_id = self.dataset_populator.user_id()
         group = self._create_group(group_name, encoded_user_ids=[encoded_user_id])
         encoded_group_id = group["id"]
 
         group_users = self._get_group_users(encoded_group_id)
@@ -96,14 +108,15 @@
 
     def test_delete_only_admin(self):
         encoded_group_id = "any-group-id"
         encoded_user_id = "any-user-id"
         response = self._delete(f"groups/{encoded_group_id}/users/{encoded_user_id}")
         self._assert_status_code_is(response, 403)
 
+    @requires_admin
     def test_delete_unknown_raises_400(self):
         group_name = "group-without-user-to-delete"
         group = self._create_group(group_name, encoded_user_ids=[])
         encoded_group_id = group["id"]
 
         group_users = self._get_group_users(encoded_group_id)
         assert len(group_users) == 0
@@ -116,20 +129,22 @@
         if encoded_user_ids is None:
             encoded_user_ids = [self.dataset_populator.user_id()]
         user_ids = encoded_user_ids
         payload = {
             "name": group_name,
             "user_ids": user_ids,
         }
+        using_requirement("admin")
         response = self._post("groups", payload, admin=True, json=True)
         self._assert_status_code_is(response, 200)
         group = response.json()[0]  # POST /api/groups returns a list
         return group
 
     def _get_group_users(self, encoded_group_id: str):
+        using_requirement("admin")
         response = self._get(f"groups/{encoded_group_id}/users", admin=True)
         self._assert_status_code_is(response, 200)
         group_users = response.json()
         return group_users
 
     def _assert_valid_group_user(self, user, assert_id=None):
         self._assert_has_keys(user, "id", "email", "url")
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_groups.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Optional
 
 from galaxy_test.base.populators import DatasetPopulator
 from ._framework import ApiTestCase
 
 
-class GroupsApiTestCase(ApiTestCase):
+class TestGroupsApi(ApiTestCase):
+    dataset_populator: DatasetPopulator
+
     def setUp(self):
         super().setUp()
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
 
     def test_create_valid(self, group_name: Optional[str] = None):
         payload = self._build_valid_group_payload(group_name)
         response = self._post("groups", payload, admin=True, json=True)
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_histories.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_histories.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,46 +28,46 @@
         put_response = put(update_url, json=data)
         return put_response
 
     def _create_history(self, name):
         post_data = dict(name=name)
         create_response = self._post("histories", data=post_data).json()
         self._assert_has_keys(create_response, "name", "id")
-        self.assertEqual(create_response["name"], name)
+        assert create_response["name"] == name
         return create_response
 
     def _assert_history_length(self, history_id, n):
         contents_response = self._get(f"histories/{history_id}/contents")
         self._assert_status_code_is(contents_response, 200)
         contents = contents_response.json()
         assert len(contents) == n, contents
 
 
-class HistoriesApiTestCase(ApiTestCase, BaseHistories):
+class TestHistoriesApi(ApiTestCase, BaseHistories):
     def setUp(self):
         super().setUp()
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
         self.dataset_collection_populator = DatasetCollectionPopulator(self.galaxy_interactor)
 
     def test_create_history(self):
         # Create a history.
         create_response = self._create_history("TestHistory1")
         created_id = create_response["id"]
 
         # Make sure new history appears in index of user's histories.
         index_response = self._get("histories").json()
         indexed_history = [h for h in index_response if h["id"] == created_id][0]
-        self.assertEqual(indexed_history["name"], "TestHistory1")
+        assert indexed_history["name"] == "TestHistory1"
 
     def test_create_history_json(self):
         name = "TestHistoryJson"
         post_data = dict(name=name)
         create_response = self._post("histories", data=post_data, json=True).json()
         self._assert_has_keys(create_response, "name", "id")
-        self.assertEqual(create_response["name"], name)
+        assert create_response["name"] == name
         return create_response
 
     def test_show_history(self):
         history_id = self._create_history("TestHistoryForShow")["id"]
         show_response = self._show(history_id)
         self._assert_has_key(
             show_response, "id", "name", "annotation", "size", "contents_url", "state", "state_details", "state_ids"
@@ -132,14 +132,50 @@
         # Delete the history
         self._delete(f"histories/{expected_history_id}")
         # Now it should match the query
         index_response = self._get(f"histories{query}").json()
         assert len(index_response) == 1
         assert index_response[0]["name"] == expected_history_name
 
+    def test_index_case_insensitive_contains_query(self):
+        # Create the histories with a different user to ensure the test
+        # is not conflicted with the current user's histories.
+        with self._different_user(f"user_{uuid4()}@bx.psu.edu"):
+            unique_id = uuid4()
+            expected_history_name = f"Test History That Match Query_{unique_id}"
+            self._create_history(expected_history_name)
+            self._create_history(expected_history_name.upper())
+            self._create_history(expected_history_name.lower())
+            self._create_history(f"Another history_{uuid4()}")
+
+            name_contains = "history"
+            query = f"?q=name-contains&qv={name_contains}"
+            index_response = self._get(f"histories{query}").json()
+            assert len(index_response) == 4
+
+            name_contains = "history that match query"
+            query = f"?q=name-contains&qv={name_contains}"
+            index_response = self._get(f"histories{query}").json()
+            assert len(index_response) == 3
+
+            name_contains = "ANOTHER"
+            query = f"?q=name-contains&qv={name_contains}"
+            index_response = self._get(f"histories{query}").json()
+            assert len(index_response) == 1
+
+            name_contains = "test"
+            query = f"?q=name-contains&qv={name_contains}"
+            index_response = self._get(f"histories{query}").json()
+            assert len(index_response) == 3
+
+            name_contains = unique_id
+            query = f"?q=name-contains&qv={name_contains}"
+            index_response = self._get(f"histories{query}").json()
+            assert len(index_response) == 3
+
     def test_delete(self):
         # Setup a history and ensure it is in the index
         history_id = self._create_history("TestHistoryForDelete")["id"]
         index_response = self._get("histories").json()
         assert index_response[0]["id"] == history_id
 
         show_response = self._show(history_id)
@@ -500,15 +536,14 @@
             history_name,
             wait_on_history_length=wait_on_history_length,
             export_kwds=export_kwds,
             task_based=self.task_based,
         )
 
     def _import_history_and_wait(self, import_data, history_name, wait_on_history_length=None):
-
         imported_history_id = self.dataset_populator.import_history_and_wait_for_name(import_data, history_name)
 
         if wait_on_history_length:
             self.dataset_populator.wait_on_history_length(imported_history_id, wait_on_history_length)
 
         return imported_history_id
 
@@ -552,23 +587,23 @@
         if collection_type is not None:
             assert imported_collection_metadata["collection_type"] == collection_type, imported_collection_metadata
 
         if elements_checker is not None:
             elements_checker(imported_collection_metadata["elements"])
 
 
-class ImportExportHistoryTestCase(ApiTestCase, ImportExportTests):
+class TestImportExportHistory(ApiTestCase, ImportExportTests):
     task_based = False
 
     def setUp(self):
         super().setUp()
         self._set_up_populators()
 
 
-class SharingHistoryTestCase(ApiTestCase, BaseHistories, SharingApiTests):
+class TestSharingHistory(ApiTestCase, BaseHistories, SharingApiTests):
     """Tests specific for the particularities of sharing Histories."""
 
     api_name = "histories"
 
     def create(self, name: str) -> str:
         response_json = self._create_history(name)
         history_id = response_json["id"]
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_history_contents.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_history_contents.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,86 +1,84 @@
-import time
 import urllib.parse
-from datetime import datetime
 from typing import (
     Any,
     List,
     Optional,
     Tuple,
 )
 
-from galaxy.webapps.galaxy.services.history_contents import DirectionOptions
 from galaxy_test.api._framework import ApiTestCase
 from galaxy_test.base.populators import (
     DatasetCollectionPopulator,
     DatasetPopulator,
     LibraryPopulator,
     skip_without_tool,
 )
 
 TEST_SOURCE_URI = "http://google.com/dataset.txt"
 TEST_HASH_FUNCTION = "MD5"
 TEST_HASH_VALUE = "moocowpretendthisisahas"
 
 
 # TODO: Test anonymous access.
-class HistoryContentsApiTestCase(ApiTestCase):
+class TestHistoryContentsApi(ApiTestCase):
+    dataset_populator: DatasetPopulator
+
     def setUp(self):
         super().setUp()
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
         self.dataset_collection_populator = DatasetCollectionPopulator(self.galaxy_interactor)
         self.library_populator = LibraryPopulator(self.galaxy_interactor)
-        self.history_id = self.dataset_populator.new_history()
 
-    def test_index_hda_summary(self):
-        hda1 = self.dataset_populator.new_dataset(self.history_id)
-        contents_response = self._get(f"histories/{self.history_id}/contents")
+    def test_index_hda_summary(self, history_id):
+        hda1 = self.dataset_populator.new_dataset(history_id)
+        contents_response = self._get(f"histories/{history_id}/contents")
         hda_summary = self.__check_for_hda(contents_response, hda1)
         assert "display_types" not in hda_summary  # Quick summary, not full details
 
-    def test_make_private_and_public(self):
-        hda1 = self._wait_for_new_hda()
-        update_url = f"histories/{self.history_id}/contents/{hda1['id']}/permissions"
+    def test_make_private_and_public(self, history_id):
+        hda1 = self._wait_for_new_hda(history_id)
+        update_url = f"histories/{history_id}/contents/{hda1['id']}/permissions"
 
         role_id = self.dataset_populator.user_private_role_id()
         # Give manage permission to the user.
         payload = {
             "access": [],
             "manage": [role_id],
         }
         update_response = self._update_permissions(update_url, payload, admin=True)
         self._assert_status_code_is(update_response, 200)
-        self._assert_other_user_can_access(hda1["id"])
+        self._assert_other_user_can_access(history_id, hda1["id"])
         # Then we restrict access.
         payload = {
             "action": "make_private",
         }
         update_response = self._update_permissions(update_url, payload)
         self._assert_status_code_is(update_response, 200)
-        self._assert_other_user_cannot_access(hda1["id"])
+        self._assert_other_user_cannot_access(history_id, hda1["id"])
 
         # Then we restrict access.
         payload = {
             "action": "remove_restrictions",
         }
         update_response = self._update_permissions(update_url, payload)
         self._assert_status_code_is(update_response, 200)
-        self._assert_other_user_can_access(hda1["id"])
+        self._assert_other_user_can_access(history_id, hda1["id"])
 
-    def test_set_permissions_add_admin_history_contents(self):
-        self._verify_dataset_permissions("history_contents")
+    def test_set_permissions_add_admin_history_contents(self, history_id):
+        self._verify_dataset_permissions(history_id, "history_contents")
 
-    def test_set_permissions_add_admin_datasets(self):
-        self._verify_dataset_permissions("dataset")
+    def test_set_permissions_add_admin_datasets(self, history_id):
+        self._verify_dataset_permissions(history_id, "dataset")
 
-    def _verify_dataset_permissions(self, api_endpoint):
-        hda1 = self._wait_for_new_hda()
+    def _verify_dataset_permissions(self, history_id: str, api_endpoint):
+        hda1 = self._wait_for_new_hda(history_id)
         hda_id = hda1["id"]
         if api_endpoint == "history_contents":
-            update_url = f"histories/{self.history_id}/contents/{hda_id}/permissions"
+            update_url = f"histories/{history_id}/contents/{hda_id}/permissions"
         else:
             update_url = f"datasets/{hda_id}/permissions"
 
         role_id = self.dataset_populator.user_private_role_id()
 
         payload = {
             "access": [role_id],
@@ -89,37 +87,37 @@
 
         # Other users cannot modify permissions.
         with self._different_user():
             update_response = self._update_permissions(update_url, payload)
             self._assert_status_code_is(update_response, 403)
 
         # First the details render for another user.
-        self._assert_other_user_can_access(hda_id)
+        self._assert_other_user_can_access(history_id, hda_id)
 
         # Then we restrict access.
         update_response = self._update_permissions(update_url, payload, admin=True)
         self._assert_status_code_is(update_response, 200)
 
         # Finally the details don't render.
-        self._assert_other_user_cannot_access(hda_id)
+        self._assert_other_user_cannot_access(history_id, hda_id)
 
         # But they do for the original user.
-        contents_response = self._get(f"histories/{self.history_id}/contents/{hda_id}").json()
+        contents_response = self._get(f"histories/{history_id}/contents/{hda_id}").json()
         assert "name" in contents_response
 
         update_response = self._update_permissions(update_url, payload)
         self._assert_status_code_is(update_response, 200)
 
         payload = {
             "access": [role_id],
             "manage": [role_id],
         }
         update_response = self._update_permissions(update_url, payload)
         self._assert_status_code_is(update_response, 200)
-        self._assert_other_user_cannot_access(hda_id)
+        self._assert_other_user_cannot_access(history_id, hda_id)
 
         user_id = self.dataset_populator.user_id()
         with self._different_user():
             different_user_id = self.dataset_populator.user_id()
         combined_user_role = self.dataset_populator.create_role(
             [user_id, different_user_id], description="role for testing permissions"
         )
@@ -127,122 +125,122 @@
         payload = {
             "access": [combined_user_role["id"]],
             "manage": [role_id],
         }
         update_response = self._update_permissions(update_url, payload)
         self._assert_status_code_is(update_response, 200)
         # Now other user can see dataset again with access permission.
-        self._assert_other_user_can_access(hda_id)
+        self._assert_other_user_can_access(history_id, hda_id)
         # access doesn't imply management though...
         with self._different_user():
             update_response = self._update_permissions(update_url, payload)
             self._assert_status_code_is(update_response, 403)
 
-    def _assert_other_user_cannot_access(self, history_content_id):
+    def _assert_other_user_cannot_access(self, history_id: str, history_content_id: str):
         with self._different_user():
             contents_response = self.dataset_populator.get_history_dataset_details_raw(
-                history_id=self.history_id, dataset_id=history_content_id
+                history_id=history_id, dataset_id=history_content_id
             )
             assert contents_response.status_code == 403
 
-    def _assert_other_user_can_access(self, history_content_id):
+    def _assert_other_user_can_access(self, history_id: str, history_content_id: str):
         with self._different_user():
             contents_response = self.dataset_populator.get_history_dataset_details_raw(
-                history_id=self.history_id, dataset_id=history_content_id
+                history_id=history_id, dataset_id=history_content_id
             )
             contents_response.raise_for_status()
             assert "name" in contents_response.json()
 
-    def test_index_hda_all_details(self):
-        hda1 = self.dataset_populator.new_dataset(self.history_id)
-        contents_response = self._get(f"histories/{self.history_id}/contents?details=all")
+    def test_index_hda_all_details(self, history_id):
+        hda1 = self.dataset_populator.new_dataset(history_id)
+        contents_response = self._get(f"histories/{history_id}/contents?details=all")
         hda_details = self.__check_for_hda(contents_response, hda1)
         self.__assert_hda_has_full_details(hda_details)
 
-    def test_index_hda_detail_by_id(self):
-        hda1 = self.dataset_populator.new_dataset(self.history_id)
-        contents_response = self._get(f"histories/{self.history_id}/contents?details={hda1['id']}")
+    def test_index_hda_detail_by_id(self, history_id):
+        hda1 = self.dataset_populator.new_dataset(history_id)
+        contents_response = self._get(f"histories/{history_id}/contents?details={hda1['id']}")
         hda_details = self.__check_for_hda(contents_response, hda1)
         self.__assert_hda_has_full_details(hda_details)
 
-    def test_index_detail_parameter_error(self):
-        hda1 = self.dataset_populator.new_dataset(self.history_id)
+    def test_index_detail_parameter_error(self, history_id):
+        hda1 = self.dataset_populator.new_dataset(history_id)
         # Invalid details should return 400
-        contents_response = self._get(f"histories/{self.history_id}/contents?v=dev&details= ")
+        contents_response = self._get(f"histories/{history_id}/contents?v=dev&details= ")
         self._assert_status_code_is(contents_response, 400)
         # Empty IDs should return 400
-        contents_response = self._get(f"histories/{self.history_id}/contents?v=dev&details=,,{hda1['id']}")
+        contents_response = self._get(f"histories/{history_id}/contents?v=dev&details=,,{hda1['id']}")
         self._assert_status_code_is(contents_response, 400)
 
         # Invalid IDs should return 400
-        contents_response = self._get(f"histories/{self.history_id}/contents?v=dev&details={hda1['id']}, ,{hda1['id']}")
+        contents_response = self._get(f"histories/{history_id}/contents?v=dev&details={hda1['id']}, ,{hda1['id']}")
         self._assert_status_code_is(contents_response, 400)
 
-    def test_show_hda(self):
-        hda1 = self.dataset_populator.new_dataset(self.history_id)
-        show_response = self.__show(hda1)
+    def test_show_hda(self, history_id):
+        hda1 = self.dataset_populator.new_dataset(history_id)
+        show_response = self.__show(history_id, hda1)
         self._assert_status_code_is(show_response, 200)
         self.__assert_matches_hda(hda1, show_response.json())
 
-    def _create_copy(self):
-        hda1 = self.dataset_populator.new_dataset(self.history_id)
+    def _create_copy(self, history_id: str):
+        hda1 = self.dataset_populator.new_dataset(history_id)
         create_data = dict(
             source="hda",
             content=hda1["id"],
         )
         second_history_id = self.dataset_populator.new_history()
         assert self.__count_contents(second_history_id) == 0
         create_response = self._post(f"histories/{second_history_id}/contents", create_data, json=True)
         self._assert_status_code_is(create_response, 200)
         return create_response.json()
 
-    def test_hda_copy(self):
-        response = self._create_copy()
+    def test_hda_copy(self, history_id):
+        response = self._create_copy(history_id)
         assert self.__count_contents(response["history_id"]) == 1
 
-    def test_inheritance_chain(self):
-        response = self._create_copy()
+    def test_inheritance_chain(self, history_id):
+        response = self._create_copy(history_id)
         inheritance_chain_response = self._get(f"datasets/{response['id']}/inheritance_chain")
         self._assert_status_code_is_ok(inheritance_chain_response)
         inheritance_chain = inheritance_chain_response.json()
         assert len(inheritance_chain) == 1
 
-    def test_library_copy(self):
+    def test_library_copy(self, history_id):
         ld = self.library_populator.new_library_dataset("lda_test_library")
         create_data = dict(
             source="library",
             content=ld["id"],
         )
-        assert self.__count_contents(self.history_id) == 0
-        create_response = self._post(f"histories/{self.history_id}/contents", create_data, json=True)
+        assert self.__count_contents(history_id) == 0
+        create_response = self._post(f"histories/{history_id}/contents", create_data, json=True)
         self._assert_status_code_is(create_response, 200)
-        assert self.__count_contents(self.history_id) == 1
+        assert self.__count_contents(history_id) == 1
 
-    def test_update(self):
-        hda1 = self._wait_for_new_hda()
+    def test_update(self, history_id):
+        hda1 = self._wait_for_new_hda(history_id)
         assert str(hda1["deleted"]).lower() == "false"
-        update_response = self._update(hda1["id"], dict(deleted=True))
+        update_response = self._update(history_id, hda1["id"], dict(deleted=True))
         self._assert_status_code_is(update_response, 200)
-        show_response = self.__show(hda1)
+        show_response = self.__show(history_id, hda1)
         assert str(show_response.json()["deleted"]).lower() == "true"
 
-        update_response = self._update(hda1["id"], dict(name="Updated Name"))
-        assert self.__show(hda1).json()["name"] == "Updated Name"
+        update_response = self._update(history_id, hda1["id"], dict(name="Updated Name"))
+        assert self.__show(history_id, hda1).json()["name"] == "Updated Name"
 
-        update_response = self._update(hda1["id"], dict(name="Updated Name"))
-        assert self.__show(hda1).json()["name"] == "Updated Name"
+        update_response = self._update(history_id, hda1["id"], dict(name="Updated Name"))
+        assert self.__show(history_id, hda1).json()["name"] == "Updated Name"
 
         unicode_name = "ржевский сапоги"
-        update_response = self._update(hda1["id"], dict(name=unicode_name))
-        updated_hda = self.__show(hda1).json()
+        update_response = self._update(history_id, hda1["id"], dict(name=unicode_name))
+        updated_hda = self.__show(history_id, hda1).json()
         assert updated_hda["name"] == unicode_name, updated_hda
 
         quoted_name = '"Mooo"'
-        update_response = self._update(hda1["id"], dict(name=quoted_name))
-        updated_hda = self.__show(hda1).json()
+        update_response = self._update(history_id, hda1["id"], dict(name=quoted_name))
+        updated_hda = self.__show(history_id, hda1).json()
         assert updated_hda["name"] == quoted_name, quoted_name
 
         data = {
             "dataset_id": hda1["id"],
             "name": "moocow",
             "dbkey": "?",
             "annotation": None,
@@ -252,194 +250,193 @@
         update_response = self._set_edit_update(data)
         # No key or anything supplied, expect a permission problem.
         # A bit questionable but I think this is a 400 instead of a 403 so that
         # we don't distinguish between this is a valid ID you don't have access to
         # and this is an invalid ID.
         assert update_response.status_code == 400, update_response.content
 
-    def test_update_batch(self):
-        hda1 = self._wait_for_new_hda()
+    def test_update_batch(self, history_id):
+        hda1 = self._wait_for_new_hda(history_id)
         assert str(hda1["deleted"]).lower() == "false"
         assert str(hda1["visible"]).lower() == "true"
 
         # update deleted flag => true
         payload = dict(items=[{"history_content_type": "dataset", "id": hda1["id"]}], deleted=True)
-        update_response = self._update_batch(payload)
+        update_response = self._update_batch(history_id, payload)
         objects = update_response.json()
         assert objects[0]["deleted"] is True
         assert objects[0]["visible"] is True
 
         # update visibility flag => false
         payload = dict(items=[{"history_content_type": "dataset", "id": hda1["id"]}], visible=False)
-        update_response = self._update_batch(payload)
+        update_response = self._update_batch(history_id, payload)
         objects = update_response.json()
         assert objects[0]["deleted"] is True
         assert objects[0]["visible"] is False
 
         # update both flags
         payload = dict(items=[{"history_content_type": "dataset", "id": hda1["id"]}], deleted=False, visible=True)
-        update_response = self._update_batch(payload)
+        update_response = self._update_batch(history_id, payload)
         objects = update_response.json()
         assert objects[0]["deleted"] is False
         assert objects[0]["visible"] is True
 
-    def test_update_batch_collections(self):
-        hdca = self._create_pair_collection()
+    def test_update_batch_collections(self, history_id):
+        hdca = self._create_pair_collection(history_id)
         assert hdca["deleted"] is False
         assert hdca["visible"] is True
 
         # update deleted flag => true
         payload = dict(items=[{"history_content_type": "dataset_collection", "id": hdca["id"]}], deleted=True)
-        update_response = self._update_batch(payload)
+        update_response = self._update_batch(history_id, payload)
         objects = update_response.json()
         assert objects[0]["deleted"] is True
         assert objects[0]["visible"] is True
 
         # update visibility flag => false
         payload = dict(items=[{"history_content_type": "dataset_collection", "id": hdca["id"]}], visible=False)
-        update_response = self._update_batch(payload)
+        update_response = self._update_batch(history_id, payload)
         objects = update_response.json()
         assert objects[0]["deleted"] is True
         assert objects[0]["visible"] is False
 
         # update both flags
         payload = dict(
             items=[{"history_content_type": "dataset_collection", "id": hdca["id"]}], deleted=False, visible=True
         )
-        update_response = self._update_batch(payload)
+        update_response = self._update_batch(history_id, payload)
         objects = update_response.json()
         assert objects[0]["deleted"] is False
         assert objects[0]["visible"] is True
 
-    def test_update_type_failures(self):
-        hda1 = self._wait_for_new_hda()
-        update_response = self._update(hda1["id"], dict(deleted="not valid"))
+    def test_update_type_failures(self, history_id):
+        hda1 = self._wait_for_new_hda(history_id)
+        update_response = self._update(history_id, hda1["id"], dict(deleted="not valid"))
         self._assert_status_code_is(update_response, 400)
 
-    def _wait_for_new_hda(self):
-        hda1 = self.dataset_populator.new_dataset(self.history_id)
-        self.dataset_populator.wait_for_history(self.history_id)
+    def _wait_for_new_hda(self, history_id: str):
+        hda1 = self.dataset_populator.new_dataset(history_id)
+        self.dataset_populator.wait_for_history(history_id)
         return hda1
 
     def _set_edit_update(self, data):
         update_response = self._put(urllib.parse.urljoin(self.url, "dataset/set_edit"), data=data, json=True)
         return update_response
 
-    def _update(self, item_id, data, admin=False, history_id=None):
-        history_id = history_id or self.history_id
+    def _update(self, history_id: str, item_id, data, admin=False):
         update_response = self._put(f"histories/{history_id}/contents/{item_id}", data=data, json=True, admin=admin)
         return update_response
 
     def _update_permissions(self, url, data, admin=False):
         update_response = self._put(url, data=data, json=True, admin=admin)
         return update_response
 
-    def _update_batch(self, data):
-        update_response = self._put(f"histories/{self.history_id}/contents", data=data, json=True)
+    def _update_batch(self, history_id: str, data):
+        update_response = self._put(f"histories/{history_id}/contents", data=data, json=True)
         return update_response
 
-    def test_delete(self):
-        hda1 = self.dataset_populator.new_dataset(self.history_id)
-        self.dataset_populator.wait_for_history(self.history_id)
-        assert str(self.__show(hda1).json()["deleted"]).lower() == "false"
-        delete_response = self._delete(f"histories/{self.history_id}/contents/{hda1['id']}")
+    def test_delete(self, history_id):
+        hda1 = self.dataset_populator.new_dataset(history_id)
+        self.dataset_populator.wait_for_history(history_id)
+        assert str(self.__show(history_id, hda1).json()["deleted"]).lower() == "false"
+        delete_response = self._delete(f"histories/{history_id}/contents/{hda1['id']}")
         assert delete_response.status_code < 300  # Something in the 200s :).
-        assert str(self.__show(hda1).json()["deleted"]).lower() == "true"
+        assert str(self.__show(history_id, hda1).json()["deleted"]).lower() == "true"
 
     def test_delete_anon(self):
         with self._different_user(anon=True):
             history_id = self._get(urllib.parse.urljoin(self.url, "history/current_history_json")).json()["id"]
             hda1 = self.dataset_populator.new_dataset(history_id)
             self.dataset_populator.wait_for_history(history_id)
-            assert str(self.__show(hda1).json()["deleted"]).lower() == "false"
+            assert str(self.__show(history_id, hda1).json()["deleted"]).lower() == "false"
             delete_response = self._delete(f"histories/{history_id}/contents/{hda1['id']}")
             assert delete_response.status_code < 300  # Something in the 200s :).
-            assert str(self.__show(hda1).json()["deleted"]).lower() == "true"
+            assert str(self.__show(history_id, hda1).json()["deleted"]).lower() == "true"
 
-    def test_delete_permission_denied(self):
-        hda1 = self.dataset_populator.new_dataset(self.history_id)
+    def test_delete_permission_denied(self, history_id):
+        hda1 = self.dataset_populator.new_dataset(history_id)
         with self._different_user(anon=True):
-            delete_response = self._delete(f"histories/{self.history_id}/contents/{hda1['id']}")
+            delete_response = self._delete(f"histories/{history_id}/contents/{hda1['id']}")
             assert delete_response.status_code == 403
             assert delete_response.json()["err_msg"] == "HistoryDatasetAssociation is not owned by user"
 
-    def test_purge(self):
-        hda1 = self.dataset_populator.new_dataset(self.history_id)
-        self.dataset_populator.wait_for_history(self.history_id)
-        assert str(self.__show(hda1).json()["deleted"]).lower() == "false"
-        assert str(self.__show(hda1).json()["purged"]).lower() == "false"
+    def test_purge(self, history_id):
+        hda1 = self.dataset_populator.new_dataset(history_id)
+        self.dataset_populator.wait_for_history(history_id)
+        assert str(self.__show(history_id, hda1).json()["deleted"]).lower() == "false"
+        assert str(self.__show(history_id, hda1).json()["purged"]).lower() == "false"
         data = {"purge": True}
-        delete_response = self._delete(f"histories/{self.history_id}/contents/{hda1['id']}", data=data, json=True)
+        delete_response = self._delete(f"histories/{history_id}/contents/{hda1['id']}", data=data, json=True)
         assert delete_response.status_code < 300  # Something in the 200s :).
         # Purging and deleting the dataset may or may not happen asynchronously.
         # On 202 the request was accepted and purging will happen later.
         if delete_response.status_code == 202:
-            self.dataset_populator.wait_for_purge(self.history_id, hda1["id"])
+            self.dataset_populator.wait_for_purge(history_id, hda1["id"])
         else:
-            assert self.__show(hda1).json()["deleted"]
-            assert self.__show(hda1).json()["purged"]
+            assert self.__show(history_id, hda1).json()["deleted"]
+            assert self.__show(history_id, hda1).json()["purged"]
 
-    def test_dataset_collection_creation_on_contents(self):
+    def test_dataset_collection_creation_on_contents(self, history_id):
         payload = self.dataset_collection_populator.create_pair_payload(
-            self.history_id, type="dataset_collection", wait=True
+            history_id, type="dataset_collection", wait=True
         )
         endpoint = "tools/fetch"
-        self._check_pair_creation(endpoint, payload)
+        self._check_pair_creation(history_id, endpoint, payload)
 
-    def test_dataset_collection_creation_on_typed_contents(self):
-        payload = self.dataset_collection_populator.create_pair_payload(self.history_id, wait=True)
+    def test_dataset_collection_creation_on_typed_contents(self, history_id):
+        payload = self.dataset_collection_populator.create_pair_payload(history_id, wait=True)
         endpoint = "tools/fetch"
-        self._check_pair_creation(endpoint, payload)
+        self._check_pair_creation(history_id, endpoint, payload)
 
     def test_dataset_collection_create_from_exisiting_datasets_with_new_tags(self):
         with self.dataset_populator.test_history() as history_id:
             hda_id = self.dataset_populator.new_dataset(history_id, content="1 2 3")["id"]
             hda2_id = self.dataset_populator.new_dataset(history_id, content="1 2 3")["id"]
-            update_response = self._update(hda2_id, dict(tags=["existing:tag"]), history_id=history_id).json()
+            update_response = self._update(history_id, hda2_id, dict(tags=["existing:tag"])).json()
             assert update_response["tags"] == ["existing:tag"]
             creation_payload = {
                 "collection_type": "list",
                 "history_id": history_id,
                 "element_identifiers": [
                     {"id": hda_id, "src": "hda", "name": "element_id1", "tags": ["my_new_tag"]},
                     {"id": hda2_id, "src": "hda", "name": "element_id2", "tags": ["another_new_tag"]},
                 ],
                 "type": "dataset_collection",
                 "copy_elements": True,
             }
-            r = self._post(f"histories/{self.history_id}/contents", creation_payload, json=True).json()
+            r = self._post(f"histories/{history_id}/contents", creation_payload, json=True).json()
             assert r["elements"][0]["object"]["id"] != hda_id, "HDA has not been copied"
             assert len(r["elements"][0]["object"]["tags"]) == 1
             assert r["elements"][0]["object"]["tags"][0] == "my_new_tag"
             assert len(r["elements"][1]["object"]["tags"]) == 2, r["elements"][1]["object"]["tags"]
             original_hda = self.dataset_populator.get_history_dataset_details(history_id=history_id, dataset_id=hda_id)
             assert len(original_hda["tags"]) == 0, original_hda["tags"]
 
-    def _check_pair_creation(self, endpoint, payload):
-        pre_collection_count = self.__count_contents(type="dataset_collection")
-        pre_dataset_count = self.__count_contents(type="dataset")
-        pre_combined_count = self.__count_contents(type="dataset,dataset_collection")
+    def _check_pair_creation(self, history_id: str, endpoint, payload):
+        pre_collection_count = self.__count_contents(history_id, type="dataset_collection")
+        pre_dataset_count = self.__count_contents(history_id, type="dataset")
+        pre_combined_count = self.__count_contents(history_id, type="dataset,dataset_collection")
 
         dataset_collection_response = self._post(endpoint, payload, json=True)
 
         dataset_collection = self.__check_create_collection_response(dataset_collection_response)
 
-        post_collection_count = self.__count_contents(type="dataset_collection")
-        post_dataset_count = self.__count_contents(type="dataset")
-        post_combined_count = self.__count_contents(type="dataset,dataset_collection")
+        post_collection_count = self.__count_contents(history_id, type="dataset_collection")
+        post_dataset_count = self.__count_contents(history_id, type="dataset")
+        post_combined_count = self.__count_contents(history_id, type="dataset,dataset_collection")
 
         # Test filtering types with index.
         assert pre_collection_count == 0
         assert post_collection_count == 1
         assert post_combined_count == pre_dataset_count + 1
         assert post_combined_count == pre_combined_count + 1
         assert pre_dataset_count == post_dataset_count
 
-        # Test show dataset colleciton.
-        collection_url = f"histories/{self.history_id}/contents/dataset_collections/{dataset_collection['id']}"
+        # Test show dataset collection.
+        collection_url = f"histories/{history_id}/contents/dataset_collections/{dataset_collection['id']}"
         show_response = self._get(collection_url)
         self._assert_status_code_is(show_response, 200)
         dataset_collection = show_response.json()
         self._assert_has_keys(dataset_collection, "url", "name", "deleted")
 
         assert not dataset_collection["deleted"]
 
@@ -447,128 +444,126 @@
         self._assert_status_code_is(delete_response, 200)
 
         show_response = self._get(collection_url)
         dataset_collection = show_response.json()
         assert dataset_collection["deleted"]
 
     @skip_without_tool("collection_creates_list")
-    def test_jobs_summary_simple_hdca(self):
+    def test_jobs_summary_simple_hdca(self, history_id):
         fetch_response = self.dataset_collection_populator.create_list_in_history(
-            self.history_id, contents=["a\nb\nc\nd", "e\nf\ng\nh"]
+            history_id, contents=["a\nb\nc\nd", "e\nf\ng\nh"]
         ).json()
         hdca_id = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)["id"]
-        run = self.dataset_populator.run_collection_creates_list(self.history_id, hdca_id)
+        run = self.dataset_populator.run_collection_creates_list(history_id, hdca_id)
         collections = run["output_collections"]
         collection = collections[0]
-        jobs_summary_url = f"histories/{self.history_id}/contents/dataset_collections/{collection['id']}/jobs_summary"
+        jobs_summary_url = f"histories/{history_id}/contents/dataset_collections/{collection['id']}/jobs_summary"
         jobs_summary_response = self._get(jobs_summary_url)
         self._assert_status_code_is(jobs_summary_response, 200)
         jobs_summary = jobs_summary_response.json()
         self._assert_has_keys(jobs_summary, "populated_state", "states")
 
     @skip_without_tool("cat1")
-    def test_jobs_summary_implicit_hdca(self):
+    def test_jobs_summary_implicit_hdca(self, history_id):
         create_response = self.dataset_collection_populator.create_pair_in_history(
-            self.history_id, contents=["123", "456"], wait=True
+            history_id, contents=["123", "456"], wait=True
         )
         hdca_id = create_response.json()["outputs"][0]["id"]
         inputs = {
             "input1": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
         }
-        run = self.dataset_populator.run_tool("cat1", inputs=inputs, history_id=self.history_id)
-        self.dataset_populator.wait_for_history_jobs(self.history_id)
+        run = self.dataset_populator.run_tool("cat1", inputs=inputs, history_id=history_id)
+        self.dataset_populator.wait_for_history_jobs(history_id)
         collections = run["implicit_collections"]
         collection = collections[0]
-        jobs_summary_url = f"histories/{self.history_id}/contents/dataset_collections/{collection['id']}/jobs_summary"
+        jobs_summary_url = f"histories/{history_id}/contents/dataset_collections/{collection['id']}/jobs_summary"
         jobs_summary_response = self._get(jobs_summary_url)
         self._assert_status_code_is(jobs_summary_response, 200)
         jobs_summary = jobs_summary_response.json()
         self._assert_has_keys(jobs_summary, "populated_state", "states")
         states = jobs_summary["states"]
         assert states.get("ok") == 2, states
 
-    def test_dataset_collection_hide_originals(self):
+    def test_dataset_collection_hide_originals(self, history_id):
         payload = self.dataset_collection_populator.create_pair_payload(
-            self.history_id, type="dataset_collection", direct_upload=False
+            history_id, type="dataset_collection", direct_upload=False
         )
 
         payload["hide_source_items"] = True
-        dataset_collection_response = self._post(f"histories/{self.history_id}/contents", payload, json=True)
+        dataset_collection_response = self._post(f"histories/{history_id}/contents", payload, json=True)
         self.__check_create_collection_response(dataset_collection_response)
 
-        contents_response = self._get(f"histories/{self.history_id}/contents")
+        contents_response = self._get(f"histories/{history_id}/contents")
         datasets = [
             d for d in contents_response.json() if d["history_content_type"] == "dataset" and d["hid"] in [1, 2]
         ]
         # Assert two datasets in source were hidden.
         assert len(datasets) == 2
         assert not datasets[0]["visible"]
         assert not datasets[1]["visible"]
 
-    def test_update_dataset_collection(self):
-        hdca = self._create_pair_collection()
+    def test_update_dataset_collection(self, history_id):
+        hdca = self._create_pair_collection(history_id)
         body = dict(name="newnameforpair")
         update_response = self._put(
-            f"histories/{self.history_id}/contents/dataset_collections/{hdca['id']}", data=body, json=True
+            f"histories/{history_id}/contents/dataset_collections/{hdca['id']}", data=body, json=True
         )
         self._assert_status_code_is(update_response, 200)
-        show_response = self.__show(hdca)
+        show_response = self.__show(history_id, hdca)
         assert str(show_response.json()["name"]) == "newnameforpair"
 
-    def test_update_batch_dataset_collection(self):
-        hdca = self._create_pair_collection()
+    def test_update_batch_dataset_collection(self, history_id):
+        hdca = self._create_pair_collection(history_id)
         body = {"items": [{"history_content_type": "dataset_collection", "id": hdca["id"]}], "name": "newnameforpair"}
-        update_response = self._put(f"histories/{self.history_id}/contents", data=body, json=True)
+        update_response = self._put(f"histories/{history_id}/contents", data=body, json=True)
         self._assert_status_code_is(update_response, 200)
-        show_response = self.__show(hdca)
+        show_response = self.__show(history_id, hdca)
         assert str(show_response.json()["name"]) == "newnameforpair"
 
-    def _create_pair_collection(self):
-        payload = self.dataset_collection_populator.create_pair_payload(self.history_id, type="dataset_collection")
+    def _create_pair_collection(self, history_id: str):
+        payload = self.dataset_collection_populator.create_pair_payload(history_id, type="dataset_collection")
         dataset_collection_response = self._post("tools/fetch", payload, json=True)
         self._assert_status_code_is(dataset_collection_response, 200)
         hdca = dataset_collection_response.json()["output_collections"][0]
         return hdca
 
-    def test_hdca_copy(self):
-        hdca = self.dataset_collection_populator.create_pair_in_history(self.history_id, wait=True).json()
+    def test_hdca_copy(self, history_id):
+        hdca = self.dataset_collection_populator.create_pair_in_history(history_id, wait=True).json()
         hdca_id = hdca["outputs"][0]["id"]
         second_history_id = self.dataset_populator.new_history()
         create_data = dict(
             source="hdca",
             content=hdca_id,
         )
         assert len(self._get(f"histories/{second_history_id}/contents/dataset_collections").json()) == 0
         create_response = self._post(
             f"histories/{second_history_id}/contents/dataset_collections", create_data, json=True
         )
         self.__check_create_collection_response(create_response)
         contents = self._get(f"histories/{second_history_id}/contents/dataset_collections").json()
         assert len(contents) == 1
-        new_forward, _ = self.__get_paired_response_elements(contents[0])
+        new_forward, _ = self.__get_paired_response_elements(history_id, contents[0])
         self._assert_has_keys(new_forward, "history_id")
-        assert new_forward["history_id"] == self.history_id
+        assert new_forward["history_id"] == history_id
 
-    def test_hdca_copy_with_new_dbkey(self):
-        fetch_response = self.dataset_collection_populator.create_pair_in_history(self.history_id, wait=True).json()
+    def test_hdca_copy_with_new_dbkey(self, history_id):
+        fetch_response = self.dataset_collection_populator.create_pair_in_history(history_id, wait=True).json()
         hdca = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)
         hdca_id = hdca["id"]
         assert hdca["elements"][0]["object"]["metadata_dbkey"] == "?"
         assert hdca["elements"][0]["object"]["genome_build"] == "?"
         create_data = {"source": "hdca", "content": hdca_id, "dbkey": "hg19"}
-        create_response = self._post(
-            f"histories/{self.history_id}/contents/dataset_collections", create_data, json=True
-        )
+        create_response = self._post(f"histories/{history_id}/contents/dataset_collections", create_data, json=True)
         collection = self.__check_create_collection_response(create_response)
         new_forward = collection["elements"][0]["object"]
         assert new_forward["metadata_dbkey"] == "hg19"
         assert new_forward["genome_build"] == "hg19"
 
-    def test_hdca_copy_and_elements(self):
-        hdca = self.dataset_collection_populator.create_pair_in_history(self.history_id, wait=True).json()["outputs"][0]
+    def test_hdca_copy_and_elements(self, history_id):
+        hdca = self.dataset_collection_populator.create_pair_in_history(history_id, wait=True).json()["outputs"][0]
         hdca_id = hdca["id"]
         second_history_id = self.dataset_populator.new_history()
         create_data = dict(
             source="hdca",
             content=hdca_id,
             copy_elements=True,
         )
@@ -576,35 +571,34 @@
         create_response = self._post(
             f"histories/{second_history_id}/contents/dataset_collections", create_data, json=True
         )
         self.__check_create_collection_response(create_response)
 
         contents = self._get(f"histories/{second_history_id}/contents/dataset_collections").json()
         assert len(contents) == 1
-        new_forward, _ = self.__get_paired_response_elements(contents[0])
+        new_forward, _ = self.__get_paired_response_elements(history_id, contents[0])
         self._assert_has_keys(new_forward, "history_id")
         assert new_forward["history_id"] == second_history_id
 
-    def __get_paired_response_elements(self, contents):
-        hdca = self.__show(contents).json()
+    def __get_paired_response_elements(self, history_id: str, contents):
+        hdca = self.__show(history_id, contents).json()
         self._assert_has_keys(hdca, "name", "deleted", "visible", "elements")
         elements = hdca["elements"]
         assert len(elements) == 2
         element0 = elements[0]
         element1 = elements[1]
         self._assert_has_keys(element0, "object")
         self._assert_has_keys(element1, "object")
 
         return element0["object"], element1["object"]
 
-    def test_hdca_from_library_datasets(self):
+    def test_hdca_from_library_datasets(self, history_id):
         ld = self.library_populator.new_library_dataset("el1")
         ldda_id = ld["ldda_id"]
         element_identifiers = [{"name": "el1", "src": "ldda", "id": ldda_id}]
-        history_id = self.dataset_populator.new_history()
         create_data = dict(
             history_id=history_id,
             type="dataset_collection",
             name="Test From Library",
             element_identifiers=element_identifiers,
             collection_type="list",
         )
@@ -614,22 +608,22 @@
         assert len(elements) == 1
         hda = elements[0]["object"]
         assert hda["hda_ldda"] == "hda"
         assert hda["history_content_type"] == "dataset"
         assert hda["copied_from_ldda_id"] == ldda_id
         assert hda["history_id"] == history_id
 
-    def test_hdca_from_inaccessible_library_datasets(self):
+    def test_hdca_from_inaccessible_library_datasets(self, history_id):
         library, library_dataset = self.library_populator.new_library_dataset_in_private_library(
             "HDCACreateInaccesibleLibrary"
         )
         ldda_id = library_dataset["id"]
         element_identifiers = [{"name": "el1", "src": "ldda", "id": ldda_id}]
         create_data = dict(
-            history_id=self.history_id,
+            history_id=history_id,
             type="dataset_collection",
             name="Test From Library",
             element_identifiers=element_identifiers,
             collection_type="list",
         )
         with self._different_user():
             second_history_id = self.dataset_populator.new_history()
@@ -642,23 +636,21 @@
         self._assert_status_code_is(response, 200)
         dataset_collection = response.json()
         if "output_collections" in dataset_collection:
             dataset_collection = dataset_collection["output_collections"][0]
         self._assert_has_keys(dataset_collection, "url", "name", "deleted", "visible", "elements")
         return dataset_collection
 
-    def __show(self, contents):
+    def __show(self, history_id, contents):
         show_response = self._get(
-            f"histories/{self.history_id}/contents/{contents['history_content_type']}s/{contents['id']}"
+            f"histories/{history_id}/contents/{contents['history_content_type']}s/{contents['id']}"
         )
         return show_response
 
-    def __count_contents(self, history_id=None, **kwds):
-        if history_id is None:
-            history_id = self.history_id
+    def __count_contents(self, history_id: str, **kwds):
         contents_response = self._get(f"histories/{history_id}/contents", kwds)
         return len(contents_response.json())
 
     def __assert_hda_has_full_details(self, hda_details):
         self._assert_has_keys(hda_details, "display_types", "display_apps")
 
     def __check_for_hda(self, contents_response, hda):
@@ -670,161 +662,30 @@
         return hda_summary
 
     def __assert_matches_hda(self, input_hda, query_hda):
         self._assert_has_keys(query_hda, "id", "name")
         assert input_hda["name"] == query_hda["name"]
         assert input_hda["id"] == query_hda["id"]
 
-    def test_job_state_summary_field(self):
+    def test_job_state_summary_field(self, history_id):
         create_response = self.dataset_collection_populator.create_pair_in_history(
-            self.history_id,
+            history_id,
             contents=["123", "456"],
         )
         self._assert_status_code_is(create_response, 200)
-        contents_response = self._get(f"histories/{self.history_id}/contents?v=dev&keys=job_state_summary&view=summary")
+        contents_response = self._get(f"histories/{history_id}/contents?v=dev&keys=job_state_summary&view=summary")
         self._assert_status_code_is(contents_response, 200)
         contents = contents_response.json()
         for c in contents:
             if c["history_content_type"] == "dataset_collection":
                 assert isinstance(c, dict)
                 assert "job_state_summary" in c
                 assert isinstance(c["job_state_summary"], dict)
 
-    def _get_content(self, history_id, update_time):
-        return self._get(f"/api/histories/{history_id}/contents/near/100/100?update_time-gt={update_time}").json()
-
-    def test_history_contents_near_with_update_time(self):
-        with self.dataset_populator.test_history() as history_id:
-            first_time = datetime.utcnow().isoformat()
-            assert len(self._get_content(history_id, update_time=first_time)) == 0
-            self.dataset_collection_populator.create_list_in_history(history_id=history_id, wait=True)
-            assert len(self._get_content(history_id, update_time=first_time)) == 4  # 3 datasets
-            self.dataset_populator.wait_for_history(history_id)
-            all_datasets_finished = first_time = datetime.utcnow().isoformat()
-            assert len(self._get_content(history_id, update_time=all_datasets_finished)) == 0
-
-    def test_history_contents_near_with_since(self):
-        with self.dataset_populator.test_history() as history_id:
-            original_history = self._get(f"/api/histories/{history_id}").json()
-            original_history_stamp = original_history["update_time"]
-
-            # check empty contents, with no since flag, should return an empty 200 result
-            history_contents = self._get(f"/api/histories/{history_id}/contents/near/100/100")
-            assert history_contents.status_code == 200
-            assert len(history_contents.json()) == 0
-
-            # adding a since parameter, should return a 204 if history has not changed at all
-            history_contents = self._get(
-                f"/api/histories/{history_id}/contents/near/100/100?since={original_history_stamp}"
-            )
-            assert history_contents.status_code == 204
-
-            # add some stuff
-            self.dataset_collection_populator.create_list_in_history(history_id=history_id, wait=True)
-            self.dataset_populator.wait_for_history(history_id)
-
-            # check to make sure the added stuff is there
-            changed_history_contents = self._get(f"/api/histories/{history_id}/contents/near/100/100")
-            assert changed_history_contents.status_code == 200
-            assert len(changed_history_contents.json()) == 4
-
-            # check to make sure the history date has actually changed due to changing the contents
-            changed_history = self._get(f"/api/histories/{history_id}").json()
-            changed_history_stamp = changed_history["update_time"]
-            assert original_history_stamp != changed_history_stamp
-
-            # a repeated contents request with since=original_history_stamp should now return data
-            # because we have added datasets and the update_time should have been changed
-            changed_content = self._get(
-                f"/api/histories/{history_id}/contents/near/100/100?since={original_history_stamp}"
-            )
-            assert changed_content.status_code == 200
-            assert len(changed_content.json()) == 4
-
-    def test_history_contents_near_since_with_standard_iso8601_date(self):
-        with self.dataset_populator.test_history() as history_id:
-            original_history = self._get(f"/api/histories/{history_id}").json()
-            original_history_stamp = original_history["update_time"]
-
-            # this is the standard date format that javascript will emit using .toISOString(), it
-            # should be the expected date format for any modern api
-            # https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date/toISOString
-
-            # checking to make sure that the same exact history.update_time returns a "not changed"
-            # result after date parsing
-            valid_iso8601_date = original_history_stamp + "Z"
-            encoded_valid_date = urllib.parse.quote_plus(valid_iso8601_date)
-            history_contents = self._get(
-                f"/api/histories/{history_id}/contents/near/100/100?since={encoded_valid_date}"
-            )
-            assert history_contents.status_code == 204
-
-            # test parsing for other standard is08601 formats
-            sample_formats = ["2021-08-26T15:53:02+00:00", "2021-08-26T15:53:02Z", "2002-10-10T12:00:00-05:00"]
-            for date_str in sample_formats:
-                encoded_date = urllib.parse.quote_plus(date_str)  # handles pluses, minuses
-                history_contents = self._get(f"/api/histories/{history_id}/contents/near/100/100?since={encoded_date}")
-                self._assert_status_code_is_ok(history_contents)
-
-    @skip_without_tool("cat_data_and_sleep")
-    def test_history_contents_near_with_update_time_implicit_collection(self):
-        with self.dataset_populator.test_history() as history_id:
-            fetch_response = self.dataset_collection_populator.create_list_in_history(history_id=history_id).json()
-            hdca_id = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)["id"]
-            self.dataset_populator.wait_for_history(history_id)
-            inputs = {
-                "input1": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
-                "sleep_time": 2,
-            }
-            response = self.dataset_populator.run_tool(
-                "cat_data_and_sleep",
-                inputs,
-                history_id,
-            )
-            update_time = datetime.utcnow().isoformat()
-            collection_id = response["implicit_collections"][0]["id"]
-            for _ in range(20):
-                time.sleep(1)
-                update = self._get_content(history_id, update_time=update_time)
-                if any(
-                    c
-                    for c in update
-                    if c["history_content_type"] == "dataset_collection" and c["job_state_summary"]["ok"] == 3
-                ):
-                    return
-            raise Exception(
-                f"History content update time query did not include final update for implicit collection {collection_id}"
-            )
-
-    @skip_without_tool("collection_creates_dynamic_nested")
-    def test_history_contents_near_with_update_time_explicit_collection(self):
-        with self.dataset_populator.test_history() as history_id:
-            inputs = {"foo": "bar", "sleep_time": 2}
-            response = self.dataset_populator.run_tool(
-                "collection_creates_dynamic_nested",
-                inputs,
-                history_id,
-            )
-            update_time = datetime.utcnow().isoformat()
-            collection_id = response["output_collections"][0]["id"]
-            for _ in range(20):
-                time.sleep(1)
-                update = self._get_content(history_id, update_time=update_time)
-                if any(
-                    c
-                    for c in update
-                    if c["history_content_type"] == "dataset_collection" and c["populated_state"] == "ok"
-                ):
-                    return
-            raise Exception(
-                f"History content update time query did not include populated_state update for dynamic nested collection {collection_id}"
-            )
-
-    def test_index_filter_by_type(self):
-        history_id = self.dataset_populator.new_history()
+    def test_index_filter_by_type(self, history_id):
         self.dataset_populator.new_dataset(history_id)
         self.dataset_collection_populator.create_list_in_history(history_id=history_id, wait=True)
 
         contents_response = self._get(f"histories/{history_id}/contents").json()
         num_items = len(contents_response)
         expected_num_collections = 1
         expected_num_datasets = num_items - expected_num_collections
@@ -834,16 +695,15 @@
         contents_response = self._get(f"histories/{history_id}/contents?types=dataset_collection").json()
         assert len(contents_response) == expected_num_collections
         contents_response = self._get(f"histories/{history_id}/contents?types=dataset,dataset_collection").json()
         assert len(contents_response) == expected_num_datasets + expected_num_collections
         contents_response = self._get(f"histories/{history_id}/contents?types=dataset&types=dataset_collection").json()
         assert len(contents_response) == expected_num_datasets + expected_num_collections
 
-    def test_index_filter_by_name_ignores_case(self):
-        history_id = self.dataset_populator.new_history()
+    def test_index_filter_by_name_ignores_case(self, history_id):
         self.dataset_populator.new_dataset(history_id, name="AC")
         self.dataset_populator.new_dataset(history_id, name="ac")
         self.dataset_populator.new_dataset(history_id, name="Bc")
 
         contains_text = "a"
         contents_response = self._get(
             f"histories/{history_id}/contents?v=dev&q=name-contains&qv={contains_text}"
@@ -861,16 +721,15 @@
         assert len(contents_response) == 3
         contains_text = "%"
         contents_response = self._get(
             f"histories/{history_id}/contents?v=dev&q=name-contains&qv={contains_text}"
         ).json()
         assert len(contents_response) == 0
 
-    def test_elements_datatypes_field(self):
-        history_id = self.dataset_populator.new_history()
+    def test_elements_datatypes_field(self, history_id):
         collection_name = "homogeneous"
         expected_datatypes = ["txt"]
         elements = [  # List with all elements of txt datatype (homogeneous)
             {"name": "test1", "src": "pasted", "paste_content": "abc", "ext": "txt"},
             {"name": "test2", "src": "pasted", "paste_content": "abc", "ext": "txt"},
         ]
         self._upload_collection_list_with_elements(history_id, collection_name, elements)
@@ -893,131 +752,18 @@
 
     def _assert_collection_has_expected_elements_datatypes(self, history_id, collection_name, expected_datatypes):
         contents_response = self._get(
             f"histories/{history_id}/contents?v=dev&view=detailed&q=name-eq&qv={collection_name}"
         )
         self._assert_status_code_is(contents_response, 200)
         collection = contents_response.json()[0]
-        self.assertCountEqual(collection["elements_datatypes"], expected_datatypes)
-
-
-class HistoryContentsApiNearTestCase(ApiTestCase):
-    """
-    Test the /api/histories/{history_id}/contents/{direction}/{hid}/{limit} endpoint.
-    """
-
-    NEAR = DirectionOptions.near
-    BEFORE = DirectionOptions.before
-    AFTER = DirectionOptions.after
-
-    def setUp(self):
-        super().setUp()
-        self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
-        self.dataset_collection_populator = DatasetCollectionPopulator(self.galaxy_interactor)
-
-    def _create_list_in_history(self, history_id, n=2):
-        # Creates list of size n*4 (n collections with 3 items each)
-        for _ in range(n):
-            self.dataset_collection_populator.create_list_in_history(history_id=history_id, wait=True)
-
-    def _get_content(self, history_id, direction, *, hid, limit=1000):
-        return self._get(f"/api/histories/{history_id}/contents/{direction}/{hid}/{limit}").json()
-
-    def test_returned_hid_sequence_in_base_case(self):
-        with self.dataset_populator.test_history() as history_id:
-            self._create_list_in_history(history_id)
-            result = self._get_content(history_id, self.NEAR, hid=1)
-            assert len(result) == 8
-            assert result[0]["hid"] == 8
-            assert result[1]["hid"] == 7
-            assert result[2]["hid"] == 6
-            assert result[3]["hid"] == 5
-            assert result[4]["hid"] == 4
-            assert result[5]["hid"] == 3
-            assert result[6]["hid"] == 2
-            assert result[7]["hid"] == 1
-
-    def test_near_even_limit(self):
-        with self.dataset_populator.test_history() as history_id:
-            self._create_list_in_history(history_id)
-            result = self._get_content(history_id, self.NEAR, hid=5, limit=3)
-            assert len(result) == 3
-            assert result[0]["hid"] == 6  # hid + 1
-            assert result[1]["hid"] == 5  # hid
-            assert result[2]["hid"] == 4  # hid - 1
-
-    def test_near_odd_limit(self):
-        with self.dataset_populator.test_history() as history_id:
-            self._create_list_in_history(history_id)
-            result = self._get_content(history_id, self.NEAR, hid=5, limit=4)
-            assert len(result) == 4
-            assert result[0]["hid"] == 7  # hid + 2
-            assert result[1]["hid"] == 6  # hid + 1
-            assert result[2]["hid"] == 5  # hid
-            assert result[3]["hid"] == 4  # hid - 1
+        assert sorted(collection["elements_datatypes"]) == sorted(expected_datatypes)
 
-    def test_near_less_than_before_limit(self):  # n before < limit // 2
-        with self.dataset_populator.test_history() as history_id:
-            self._create_list_in_history(history_id)
-            result = self._get_content(history_id, self.NEAR, hid=1, limit=3)
-            assert len(result) == 2
-            assert result[0]["hid"] == 2  # hid + 1
-            assert result[1]["hid"] == 1  # hid (there's nothing before hid=1)
-
-    def test_near_less_than_after_limit(self):  # n after < limit // 2 + 1
-        with self.dataset_populator.test_history() as history_id:
-            self._create_list_in_history(history_id)
-            result = self._get_content(history_id, self.NEAR, hid=8, limit=3)
-            assert len(result) == 2
-            assert result[0]["hid"] == 8  # hid (there's nothing after hid=8)
-            assert result[1]["hid"] == 7  # hid - 1
-
-    def test_near_less_than_before_and_after_limit(self):
-        with self.dataset_populator.test_history() as history_id:
-            self._create_list_in_history(history_id, n=1)
-            result = self._get_content(history_id, self.NEAR, hid=2, limit=10)
-            assert len(result) == 4
-            assert result[0]["hid"] == 4  # hid + 2  (can't go after hid=4)
-            assert result[1]["hid"] == 3  # hid + 1
-            assert result[2]["hid"] == 2  # hid
-            assert result[3]["hid"] == 1  # hid - 1  (can't go before hid=1)
 
-    def test_before(self):
-        with self.dataset_populator.test_history() as history_id:
-            self._create_list_in_history(history_id)
-            result = self._get_content(history_id, self.BEFORE, hid=5, limit=3)
-            assert len(result) == 3
-            assert result[0]["hid"] == 4  # hid - 1
-            assert result[1]["hid"] == 3  # hid - 2
-            assert result[2]["hid"] == 2  # hid - 3
-
-    def test_before_less_than_limit(self):
-        with self.dataset_populator.test_history() as history_id:
-            self._create_list_in_history(history_id)
-            result = self._get_content(history_id, self.BEFORE, hid=2, limit=3)
-            assert len(result) == 1
-            assert result[0]["hid"] == 1  # hid - 1
-
-    def test_after(self):
-        with self.dataset_populator.test_history() as history_id:
-            self._create_list_in_history(history_id)
-            result = self._get_content(history_id, self.AFTER, hid=5, limit=2)
-            assert len(result) == 2
-            assert result[0]["hid"] == 7  # hid + 2 (hid + 3 not included: tests reversed order)
-            assert result[1]["hid"] == 6  # hid + 1
-
-    def test_after_less_than_limit(self):
-        with self.dataset_populator.test_history() as history_id:
-            self._create_list_in_history(history_id)
-            result = self._get_content(history_id, self.AFTER, hid=7, limit=3)
-            assert len(result) == 1
-            assert result[0]["hid"] == 8  # hid + 1
-
-
-class HistoryContentsApiBulkOperationTestCase(ApiTestCase):
+class TestHistoryContentsApiBulkOperation(ApiTestCase):
     """
     Test the `/api/histories/{history_id}/contents/bulk` endpoint and the new
     `count` special view for `/api/histories/{history_id}/contents?v=dev`
     """
 
     def setUp(self):
         super().setUp()
@@ -1331,21 +1077,22 @@
                 assert "metadata_column_names" in item
 
     def test_bulk_datatype_change_collection(self):
         with self.dataset_populator.test_history() as history_id:
             _, collection_ids, history_contents = self._create_test_history_contents(history_id)
 
             history_contents = self._get_history_contents(history_id, query="?v=dev&keys=extension,data_type,metadata")
+            original_collection_update_times = []
             for item in history_contents:
                 if item["history_content_type"] == "dataset":
                     assert item["extension"] == "txt"
                     assert item["data_type"] == "galaxy.datatypes.data.Text"
                     assert "metadata_column_names" not in item
-
-            self.dataset_populator.wait_for_history_jobs(history_id)
+                if item["history_content_type"] == "dataset_collection":
+                    original_collection_update_times.append(item["update_time"])
 
             expected_datatype = "tabular"
             # Change datatype of all datasets
             payload = {
                 "operation": "change_datatype",
                 "params": {
                     "type": "change_datatype",
@@ -1357,19 +1104,24 @@
             )
             self._assert_bulk_success(bulk_operation_result, expected_success_count=len(collection_ids))
 
             # Wait for celery tasks to finish
             self.dataset_populator.wait_for_history(history_id)
 
             history_contents = self._get_history_contents(history_id, query="?v=dev&keys=extension,data_type,metadata")
+            new_collection_update_times = []
             for item in history_contents:
                 if item["history_content_type"] == "dataset":
                     assert item["extension"] == "tabular"
                     assert item["data_type"] == "galaxy.datatypes.tabular.Tabular"
                     assert "metadata_column_names" in item
+                if item["history_content_type"] == "dataset_collection":
+                    new_collection_update_times.append(item["update_time"])
+
+            assert original_collection_update_times != new_collection_update_times
 
     def test_bulk_datatype_change_should_skip_set_metadata_on_deferred_data(self):
         with self.dataset_populator.test_history() as history_id:
             details = self.dataset_populator.create_deferred_hda(
                 history_id, "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/1.bed", ext="bed"
             )
             assert details["state"] == "deferred"
@@ -1498,15 +1250,15 @@
                 expected_total_matches=len(datasets_ids),
             )
 
     def test_index_with_stats_fails_with_non_orm_filters(self):
         with self.dataset_populator.test_history() as history_id:
             self._create_test_history_contents(history_id)
 
-            invalid_filter_keys_with_stats = ["genome_build", "data_type", "annotation"]
+            invalid_filter_keys_with_stats = ["data_type", "annotation"]
 
             for filter_key in invalid_filter_keys_with_stats:
                 response = self._get_contents_with_stats(
                     history_id,
                     search_query=f"&q={filter_key}-contains&qv=anything",
                 )
                 self._assert_status_code_is(response, 400)
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_history_contents_provenance.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_history_contents_provenance.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 MINIMAL_PROV_KEYS = ("id", "uuid")
 OTHER_PROV_KEYS = ("job_id", "stdout", "stderr", "parameters", "tool_id")
 ALL_PROV_KEYS = MINIMAL_PROV_KEYS + OTHER_PROV_KEYS
 
 
 class TestProvenance(ApiTestCase):
+    dataset_populator: DatasetPopulator
+
     def setUp(self):
         super().setUp()
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
 
     @skip_without_tool("cat1")
     def test_get_prov(self):
         history_id = self.dataset_populator.new_history()
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_jobs.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_jobs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 import datetime
 import json
 import os
 import time
 import urllib.parse
 from operator import itemgetter
+from unittest import SkipTest
 
+import pytest
 import requests
 from dateutil.parser import isoparse
 
 from galaxy_test.api.test_tools import TestsTools
 from galaxy_test.base.api_asserts import assert_status_code_is_ok
 from galaxy_test.base.populators import (
     DatasetCollectionPopulator,
     DatasetPopulator,
     skip_without_tool,
-    uses_test_history,
     wait_on,
     wait_on_state,
     WorkflowPopulator,
 )
 from ._framework import ApiTestCase
 
 
-class JobsApiTestCase(ApiTestCase, TestsTools):
+class TestJobsApi(ApiTestCase, TestsTools):
+    dataset_populator: DatasetPopulator
+
     def setUp(self):
         super().setUp()
         self.workflow_populator = WorkflowPopulator(self.galaxy_interactor)
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
         self.dataset_collection_populator = DatasetCollectionPopulator(self.galaxy_interactor)
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_index(self, history_id):
         # Create HDA to ensure at least one job exists...
         self.__history_with_new_dataset(history_id)
         jobs = self.__jobs_index()
         assert "__DATA_FETCH__" in map(itemgetter("tool_id"), jobs)
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_system_details_admin_only(self, history_id):
         self.__history_with_new_dataset(history_id)
         jobs = self.__jobs_index(admin=False)
         job = jobs[0]
         self._assert_not_has_keys(job, "external_id")
 
         jobs = self.__jobs_index(admin=True)
         job = jobs[0]
         self._assert_has_keys(job, "command_line", "external_id")
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_admin_job_list(self, history_id):
         self.__history_with_new_dataset(history_id)
         jobs_response = self._get("jobs?view=admin_job_list", admin=False)
         assert jobs_response.status_code == 403
         assert jobs_response.json()["err_msg"] == "Only admins can use the admin_job_list view"
 
         jobs = self._get("jobs?view=admin_job_list", admin=True).json()
         job = jobs[0]
         self._assert_has_keys(job, "command_line", "external_id", "handler")
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_index_state_filter(self, history_id):
         # Initial number of ok jobs
         original_count = len(self.__uploads_with_state("ok"))
         # Run through dataset upload to ensure num uplaods at least greater
         # by 1.
         self.__history_with_ok_dataset(history_id)
 
@@ -76,15 +79,15 @@
             time.sleep(0.1)
 
         if not count_increased:
             template = "Jobs in ok state did not increase (was %d, now %d)"
             message = template % (original_count, new_count)
             raise AssertionError(message)
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_index_date_filter(self, history_id):
         two_weeks_ago = (datetime.datetime.utcnow() - datetime.timedelta(14)).isoformat()
         last_week = (datetime.datetime.utcnow() - datetime.timedelta(7)).isoformat()
         before = datetime.datetime.utcnow().isoformat()
         today = before[:10]
         tomorrow = (datetime.datetime.utcnow() + datetime.timedelta(1)).isoformat()[:10]
         self.__history_with_new_dataset(history_id)
@@ -99,25 +102,25 @@
         # Test using datetimes
         jobs = self.__jobs_index(data={"date_range_min": before, "date_range_max": after})
         assert today_job_id in map(itemgetter("id"), jobs), f"before: {before}, after: {after}, job: {today_job}"
 
         jobs = self.__jobs_index(data={"date_range_min": two_weeks_ago, "date_range_max": last_week})
         assert today_job_id not in map(itemgetter("id"), jobs)
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_index_history(self, history_id):
         self.__history_with_new_dataset(history_id)
         jobs = self.__jobs_index(data={"history_id": history_id})
         assert len(jobs) > 0
 
         with self.dataset_populator.test_history() as other_history_id:
             jobs = self.__jobs_index(data={"history_id": other_history_id})
             assert len(jobs) == 0
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     @skip_without_tool("cat1")
     def test_index_workflow_and_invocation_filter(self, history_id):
         workflow_simple = """
 class: GalaxyWorkflow
 name: Simple Workflow
 inputs:
   input1: data
@@ -138,15 +141,15 @@
         self.workflow_populator.wait_for_invocation(workflow_id, invocation_id)
         jobs1 = self.__jobs_index(data={"workflow_id": workflow_id})
         assert len(jobs1) == 1
         jobs2 = self.__jobs_index(data={"invocation_id": invocation_id})
         assert len(jobs2) == 1
         assert jobs1 == jobs2
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     @skip_without_tool("multi_data_optional")
     def test_index_workflow_filter_implicit_jobs(self, history_id):
         workflow_id = self.workflow_populator.upload_yaml_workflow(
             """
 class: GalaxyWorkflow
 inputs:
   input_datasets: collection
@@ -172,39 +175,39 @@
             workflow_id, history_id=history_id, inputs=inputs
         ).json()["id"]
         workflow_jobs = self.__jobs_index(data={"workflow_id": workflow_id})
         second_invocation_jobs = self.__jobs_index(data={"invocation_id": second_invocation_id})
         assert len(workflow_jobs) == 2
         assert len(second_invocation_jobs) == 1
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_index_limit_and_offset_filter(self, history_id):
         self.__history_with_new_dataset(history_id)
         jobs = self.__jobs_index(data={"history_id": history_id})
         assert len(jobs) > 0
         length = len(jobs)
         jobs = self.__jobs_index(data={"history_id": history_id, "offset": 1})
         assert len(jobs) == length - 1
         jobs = self.__jobs_index(data={"history_id": history_id, "limit": 0})
         assert len(jobs) == 0
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_index_search_filter_tool_id(self, history_id):
         self.__history_with_new_dataset(history_id)
         jobs = self.__jobs_index(data={"history_id": history_id})
         assert len(jobs) > 0
         length = len(jobs)
         jobs = self.__jobs_index(data={"history_id": history_id, "search": "emptyresult"})
         assert len(jobs) == 0
         jobs = self.__jobs_index(data={"history_id": history_id, "search": "FETCH"})
         assert len(jobs) == length
         jobs = self.__jobs_index(data={"history_id": history_id, "search": "tool:'FETCH'"})
         assert len(jobs) == 0
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_index_search_filter_email(self, history_id):
         self.__history_with_new_dataset(history_id)
         jobs = self.__jobs_index(data={"history_id": history_id, "search": "FETCH"})
         user_email = self.dataset_populator.user_email()
         jobs = self.__jobs_index(data={"history_id": history_id, "search": user_email})
         assert len(jobs) == 0
         # we can search on email...
@@ -229,15 +232,15 @@
         jobs = self.__jobs_index(data={"user_id": user["id"]}, admin=True)
         assert jobs == []
         # Normal user should not be able to see jobs of another user.
         jobs_response = self._get("jobs", data={"user_id": user["id"]})
         self._assert_status_code_is(jobs_response, 403)
         assert jobs_response.json() == {"err_msg": "Only admins can index the jobs of others", "err_code": 403006}
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_index_handler_runner_filters(self, history_id):
         self.__history_with_new_dataset(history_id)
 
         jobs = self._get(f"jobs?view=admin_job_list&history_id={history_id}", admin=True).json()
         job = jobs[0]
         handler = job["handler"]
         assert handler
@@ -274,28 +277,28 @@
         ).json()
         assert jobs
         jobs = self._get(
             f"jobs?view=admin_job_list&history_id={history_id}&search=handler:%27{runner}%27", admin=True
         ).json()
         assert not jobs
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_index_multiple_states_filter(self, history_id):
         # Initial number of ok jobs
         original_count = len(self.__uploads_with_state("ok", "new"))
 
         # Run through dataset upload to ensure num uploads at least greater
         # by 1.
         self.__history_with_ok_dataset(history_id)
 
         # Verify number of ok jobs is actually greater.
         new_count = len(self.__uploads_with_state("new", "ok"))
         assert original_count < new_count, new_count
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_show(self, history_id):
         job_properties_tool_run = self.dataset_populator.run_tool(
             tool_id="job_properties",
             inputs={},
             history_id=history_id,
         )
         first_job = self.__jobs_index()[0]
@@ -334,15 +337,15 @@
         assert "The bool is not true\n" not in job_details["job_stdout"]
         assert "The bool is very not true\n" not in job_details["job_stderr"]
         assert job_details["tool_stdout"] == "The bool is not true\n"
         assert job_details["tool_stderr"] == "The bool is very not true\n"
         assert "The bool is not true\n" in job_details["stdout"]
         assert "The bool is very not true\n" in job_details["stderr"]
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_show_security(self, history_id):
         self.__history_with_new_dataset(history_id)
         jobs_response = self._get("jobs", data={"history_id": history_id})
         job = jobs_response.json()[0]
         job_id = job["id"]
 
         job_lock_response = self._get("job_lock", admin=True)
@@ -495,16 +498,16 @@
                 tool_id="detect_errors_aggressive",
                 inputs={"error_bool": "true"},
                 history_id=history_id,
             )
             run_response = self._post("tools", data=payload, key=self.master_api_key)
             self._assert_status_code_is(run_response, 400)
 
+    @pytest.mark.require_new_history
     @skip_without_tool("create_2")
-    @uses_test_history(require_new=True)
     def test_deleting_output_keep_running_until_all_deleted(self, history_id):
         job_state, outputs = self._setup_running_two_output_job(history_id, 120)
 
         self._hack_to_skip_test_if_state_ok(job_state)
 
         # Delete one of the two outputs and make sure the job is still running.
         self._raw_update_history_item(history_id, outputs[0]["id"], {"deleted": True})
@@ -519,16 +522,16 @@
         assert state == "running", state
 
         # Delete the second output and make sure the job is cancelled.
         self._raw_update_history_item(history_id, outputs[1]["id"], {"deleted": True})
         final_state = wait_on_state(job_state, assert_ok=False, timeout=15)
         assert final_state in ["deleting", "deleted"], final_state
 
+    @pytest.mark.require_new_history
     @skip_without_tool("create_2")
-    @uses_test_history(require_new=True)
     def test_purging_output_keep_running_until_all_purged(self, history_id):
         job_state, outputs = self._setup_running_two_output_job(history_id, 120)
 
         # Pretty much right away after the job is running, these paths should be populated -
         # if they are grab them and make sure they are deleted at the end of the job.
         dataset_1 = self._get_history_item_as_admin(history_id, outputs[0]["id"])
         dataset_2 = self._get_history_item_as_admin(history_id, outputs[1]["id"])
@@ -562,16 +565,16 @@
         def paths_deleted():
             if not os.path.exists(output_dataset_paths[0]) and not os.path.exists(output_dataset_paths[1]):
                 return True
 
         if output_dataset_paths_exist:
             wait_on(paths_deleted, "path deletion")
 
+    @pytest.mark.require_new_history
     @skip_without_tool("create_2")
-    @uses_test_history(require_new=True)
     def test_purging_output_cleaned_after_ok_run(self, history_id):
         job_state, outputs = self._setup_running_two_output_job(history_id, 10)
 
         # Pretty much right away after the job is running, these paths should be populated -
         # if they are grab them and make sure they are deleted at the end of the job.
         dataset_1 = self._get_history_item_as_admin(history_id, outputs[0]["id"])
         dataset_2 = self._get_history_item_as_admin(history_id, outputs[1]["id"])
@@ -595,16 +598,14 @@
         if output_dataset_paths_exist:
             time.sleep(0.5)
             # Make sure the non-purged dataset is on disk and the purged one is not.
             assert os.path.exists(output_dataset_paths[1])
             assert not os.path.exists(output_dataset_paths[0])
 
     def _hack_to_skip_test_if_state_ok(self, job_state):
-        from nose.plugins.skip import SkipTest
-
         if job_state().json()["state"] == "ok":
             message = "Job state switch from running to ok too quickly - the rest of the test requires the job to be in a running state. Skipping test."
             raise SkipTest(message)
 
     def _setup_running_two_output_job(self, history_id, sleep_time):
         payload = self.dataset_populator.run_tool_payload(
             tool_id="create_2",
@@ -635,16 +636,16 @@
 
     def _raw_update_history_item(self, history_id, item_id, data):
         update_url = self._api_url(f"histories/{history_id}/contents/{item_id}", use_key=True)
         update_response = requests.put(update_url, json=data)
         assert_status_code_is_ok(update_response)
         return update_response
 
+    @pytest.mark.require_new_history
     @skip_without_tool("cat_data_and_sleep")
-    @uses_test_history(require_new=True)
     def test_resume_job(self, history_id):
         hda1 = self.dataset_populator.new_dataset(history_id, content="samp1\t10.0\nsamp2\t20.0\n")
         hda2 = self.dataset_populator.new_dataset(history_id, content="samp1\t30.0\nsamp2\t40.0\n")
         # Submit first job
         payload = self.dataset_populator.run_tool_payload(
             tool_id="cat_data_and_sleep",
             inputs={
@@ -683,15 +684,15 @@
         assert dataset_details["state"] == "ok"
 
     def _get_history_item_as_admin(self, history_id, item_id):
         response = self._get(f"histories/{history_id}/contents/{item_id}?view=detailed", admin=True)
         assert_status_code_is_ok(response)
         return response.json()
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_search(self, history_id):
         dataset_id = self.__history_with_ok_dataset(history_id)
         # We first copy the datasets, so that the update time is lower than the job creation time
         new_history_id = self.dataset_populator.new_history()
         copy_payload = {"content": dataset_id, "source": "hda", "type": "dataset"}
         copy_response = self._post(f"histories/{new_history_id}/contents", data=copy_payload, json=True)
         self._assert_status_code_is(copy_response, 200)
@@ -707,15 +708,15 @@
         self._assert_status_code_is(delete_respone, 200)
         self._search(search_payload, expected_search_count=1)
         # Now we also delete the copy -- we shouldn't find a job
         delete_respone = self._delete(f"histories/{new_history_id}/contents/{new_dataset_id}")
         self._assert_status_code_is(delete_respone, 200)
         self._search(search_payload, expected_search_count=0)
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_search_handle_identifiers(self, history_id):
         # Test that input name and element identifier of a jobs' output must match for a job to be returned.
         dataset_id = self.__history_with_ok_dataset(history_id)
         inputs = json.dumps({"input1": {"src": "hda", "id": dataset_id}})
         self._job_search(tool_id="identifier_single", history_id=history_id, inputs=inputs)
         dataset_details = self._get(f"histories/{history_id}/contents/{dataset_id}").json()
         dataset_details["name"] = "Renamed Test Dataset"
@@ -723,26 +724,26 @@
             f"histories/{history_id}/contents/{dataset_id}", data=dict(name="Renamed Test Dataset"), json=True
         )
         self._assert_status_code_is(dataset_update_response, 200)
         assert dataset_update_response.json()["name"] == "Renamed Test Dataset"
         search_payload = self._search_payload(history_id=history_id, tool_id="identifier_single", inputs=inputs)
         self._search(search_payload, expected_search_count=0)
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_search_delete_outputs(self, history_id):
         dataset_id = self.__history_with_ok_dataset(history_id)
         inputs = json.dumps({"input1": {"src": "hda", "id": dataset_id}})
         tool_response = self._job_search(tool_id="cat1", history_id=history_id, inputs=inputs)
         output_id = tool_response.json()["outputs"][0]["id"]
         delete_respone = self._delete(f"histories/{history_id}/contents/{output_id}")
         self._assert_status_code_is(delete_respone, 200)
         search_payload = self._search_payload(history_id=history_id, tool_id="cat1", inputs=inputs)
         self._search(search_payload, expected_search_count=0)
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_search_with_hdca_list_input(self, history_id):
         list_id_a = self.__history_with_ok_collection(collection_type="list", history_id=history_id)
         list_id_b = self.__history_with_ok_collection(collection_type="list", history_id=history_id)
         inputs = json.dumps(
             {
                 "f1": {"src": "hdca", "id": list_id_a},
                 "f2": {"src": "hdca", "id": list_id_b},
@@ -762,15 +763,15 @@
         # and use the correct input job definition, the job should not be found
         output_id = tool_response.json()["outputs"][0]["id"]
         delete_respone = self._delete(f"histories/{history_id}/contents/{output_id}")
         self._assert_status_code_is(delete_respone, 200)
         search_payload = self._search_payload(history_id=history_id, tool_id="multi_data_param", inputs=inputs)
         self._search(search_payload, expected_search_count=0)
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_search_delete_hdca_output(self, history_id):
         list_id_a = self.__history_with_ok_collection(collection_type="list", history_id=history_id)
         inputs = json.dumps(
             {
                 "input1": {"src": "hdca", "id": list_id_a},
             }
         )
@@ -785,15 +786,15 @@
         output_collection_id = tool_response.json()["output_collections"][0]["id"]
         # We delete a collection output, no job should be returned
         delete_respone = self._delete(f"histories/{history_id}/contents/dataset_collections/{output_collection_id}")
         self._assert_status_code_is(delete_respone, 200)
         search_payload = self._search_payload(history_id=history_id, tool_id="collection_creates_list", inputs=inputs)
         self._search(search_payload, expected_search_count=0)
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_search_with_hdca_pair_input(self, history_id):
         list_id_a = self.__history_with_ok_collection(collection_type="pair", history_id=history_id)
         inputs = json.dumps(
             {
                 "f1": {"src": "hdca", "id": list_id_a},
                 "f2": {"src": "hdca", "id": list_id_a},
             }
@@ -820,26 +821,26 @@
         self._assert_status_code_is(delete_respone, 200)
         self._search(search_payload, expected_search_count=1)
         # Now we also delete the copy -- we shouldn't find a job
         delete_respone = self._delete(f"histories/{history_id}/contents/dataset_collections/{new_list_a}")
         self._assert_status_code_is(delete_respone, 200)
         self._search(search_payload, expected_search_count=0)
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_search_with_hdca_list_pair_input(self, history_id):
         list_id_a = self.__history_with_ok_collection(collection_type="list:pair", history_id=history_id)
         inputs = json.dumps(
             {
                 "f1": {"src": "hdca", "id": list_id_a},
                 "f2": {"src": "hdca", "id": list_id_a},
             }
         )
         self._job_search(tool_id="multi_data_param", history_id=history_id, inputs=inputs)
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_search_with_hdca_list_pair_collection_mapped_over_pair_input(self, history_id):
         list_id_a = self.__history_with_ok_collection(collection_type="list:pair", history_id=history_id)
         inputs = json.dumps(
             {
                 "f1": {"batch": True, "values": [{"src": "hdca", "id": list_id_a, "map_over_type": "paired"}]},
             }
         )
@@ -863,42 +864,39 @@
         if private:
             hdca = self.dataset_populator.get_history_collection_details(history_id=history_id, content_id=list_id_a)
             for element in hdca["elements"][0]["object"]["elements"]:
                 self.dataset_populator.make_private(history_id, element["object"]["id"])
         return rerun_params
 
     @skip_without_tool("collection_paired_test")
-    @uses_test_history(require_new=False)
     def test_job_build_for_rerun(self, history_id):
         rerun_params = self._get_simple_rerun_params(history_id)
         self._run(
             history_id=history_id,
             tool_id="collection_paired_test",
             inputs=rerun_params["state_inputs"],
             wait_for_job=True,
             assert_ok=True,
         )
 
     @skip_without_tool("collection_paired_test")
-    @uses_test_history(require_new=False)
     def test_dce_submission_security(self, history_id):
         rerun_params = self._get_simple_rerun_params(history_id, private=True)
         with self._different_user():
             other_history_id = self.dataset_populator.new_history()
             response = self._run(
                 history_id=other_history_id,
                 tool_id="collection_paired_test",
                 inputs=rerun_params["state_inputs"],
                 wait_for_job=False,
                 assert_ok=False,
             )
             assert response.status_code == 403
 
     @skip_without_tool("identifier_collection")
-    @uses_test_history(require_new=False)
     def test_job_build_for_rerun_list_list(self, history_id):
         list_id_a = self.__history_with_ok_collection(collection_type="list", history_id=history_id)
         list_id_b = self.__history_with_ok_collection(collection_type="list", history_id=history_id)
         list_list = self.dataset_collection_populator.create_nested_collection(
             history_id=history_id,
             collection_type="list:list",
             name="list list collection",
@@ -939,15 +937,15 @@
         )
         assert rerun_content == run_content
 
     def _job_search(self, tool_id, history_id, inputs):
         search_payload = self._search_payload(history_id=history_id, tool_id=tool_id, inputs=inputs)
         empty_search_response = self._post("jobs/search", data=search_payload)
         self._assert_status_code_is(empty_search_response, 200)
-        self.assertEqual(len(empty_search_response.json()), 0)
+        assert len(empty_search_response.json()) == 0
         tool_response = self._post("tools", data=search_payload)
         self.dataset_populator.wait_for_tool_run(history_id, run_response=tool_response)
         self._search(search_payload, expected_search_count=1)
         return tool_response
 
     def _search_payload(self, history_id, tool_id, inputs, state="ok"):
         search_payload = dict(tool_id=tool_id, inputs=inputs, history_id=history_id, state=state)
@@ -973,15 +971,15 @@
         search_json = search_response.json()
         return len(search_json)
 
     def __uploads_with_state(self, *states):
         jobs_response = self._get("jobs", data=dict(state=states))
         self._assert_status_code_is(jobs_response, 200)
         jobs = jobs_response.json()
-        assert not [j for j in jobs if not j["state"] in states]
+        assert not [j for j in jobs if j["state"] not in states]
         return [j for j in jobs if j["tool_id"] == "__DATA_FETCH__"]
 
     def __history_with_new_dataset(self, history_id):
         dataset_id = self.dataset_populator.new_dataset(history_id, wait=True)["id"]
         return dataset_id
 
     def __history_with_ok_dataset(self, history_id):
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_libraries.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_libraries.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 import unittest
 
-import pytest
-import requests
-
 from galaxy.model.unittest_utils.store_fixtures import (
     one_ld_library_model_store_dict,
     TEST_LIBRARY_NAME,
 )
+from galaxy.util.unittest_utils import skip_if_github_down
+from galaxy_test.base import api_asserts
+from galaxy_test.base.decorators import requires_new_library
 from galaxy_test.base.populators import (
     DatasetCollectionPopulator,
     DatasetPopulator,
     FILE_URL,
     LibraryPopulator,
-    skip_if_github_down,
     skip_without_asgi,
 )
 from ._framework import ApiTestCase
 
 
-class LibrariesApiTestCase(ApiTestCase):
+class TestLibrariesApi(ApiTestCase):
+    dataset_populator: DatasetPopulator
+
     def setUp(self):
         super().setUp()
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
         self.dataset_collection_populator = DatasetCollectionPopulator(self.galaxy_interactor)
         self.library_populator = LibraryPopulator(self.galaxy_interactor)
 
+    @requires_new_library
     def test_create(self):
         data = dict(name="CreateTestLibrary")
         create_response = self._post("libraries", data=data, admin=True, json=True)
         self._assert_status_code_is(create_response, 200)
         library = create_response.json()
         self._assert_has_keys(library, "name")
         assert library["name"] == "CreateTestLibrary"
 
     @skip_without_asgi
+    @requires_new_library
     def test_create_from_store(self):
         response = self.library_populator.create_from_store(store_dict=one_ld_library_model_store_dict())
         assert isinstance(response, list)
         assert len(response) == 1
         library_summary = response[0]
         assert library_summary["name"] == TEST_LIBRARY_NAME
         assert "id" in library_summary
         ld = self.library_populator.get_library_contents_with_path(library_summary["id"], "/my cool name")
         assert ld
 
+    @requires_new_library
     def test_delete(self):
         library = self.library_populator.new_library("DeleteTestLibrary")
         create_response = self._delete(f"libraries/{library['id']}", admin=True)
         self._assert_status_code_is(create_response, 200)
         library = create_response.json()
         self._assert_has_keys(library, "deleted")
         assert library["deleted"] is True
@@ -68,25 +72,27 @@
         create_response = self._delete(f"libraries/{library['id']}", admin=False, anon=True)
         self._assert_status_code_is(create_response, 403)
         # Anons can't update libs
         data = dict(name="ChangedName", description="ChangedDescription", synopsis="ChangedSynopsis")
         create_response = self._patch(f"libraries/{library['id']}", data=data, admin=False, anon=True, json=True)
         self._assert_status_code_is(create_response, 403)
 
+    @requires_new_library
     def test_update(self):
         library = self.library_populator.new_library("UpdateTestLibrary")
         data = dict(name="ChangedName", description="ChangedDescription", synopsis="ChangedSynopsis")
         create_response = self._patch(f"libraries/{library['id']}", data=data, admin=True, json=True)
         self._assert_status_code_is(create_response, 200)
         library = create_response.json()
         self._assert_has_keys(library, "name", "description", "synopsis")
         assert library["name"] == "ChangedName"
         assert library["description"] == "ChangedDescription"
         assert library["synopsis"] == "ChangedSynopsis"
 
+    @requires_new_library
     def test_update_non_admins_with_permission(self):
         library = self.library_populator.new_library("UpdateTestLibraryNonAdmin")
         library_id = library["id"]
         role_id = self.library_populator.user_private_role_id()
         data = dict(name="ChangedName", description="ChangedDescription", synopsis="ChangedSynopsis")
         # User has no permission by default
         create_response = self._patch(f"libraries/{library['id']}", data=data, json=True)
@@ -97,38 +103,41 @@
         self._assert_status_code_is(create_response, 200)
         library = create_response.json()
         self._assert_has_keys(library, "name", "description", "synopsis")
         assert library["name"] == "ChangedName"
         assert library["description"] == "ChangedDescription"
         assert library["synopsis"] == "ChangedSynopsis"
 
+    @requires_new_library
     def test_create_private_library_legacy_permissions(self):
         library = self.library_populator.new_library("LegacyPermissionTestLibrary")
         library_id = library["id"]
         role_id = self.library_populator.user_private_role_id()
         self.library_populator.set_permissions(library_id, role_id)
         create_response = self._create_folder(library)
         self._assert_status_code_is(create_response, 200)
 
         with self._different_user():
             create_response = self._create_folder(library)
             self._assert_status_code_is(create_response, 403)
 
+    @requires_new_library
     def test_create_private_library_permissions(self):
         library = self.library_populator.new_library("PermissionTestLibrary")
         library_id = library["id"]
         role_id = self.library_populator.user_private_role_id()
         self.library_populator.set_permissions_with_action(library_id, role_id, action="set_permissions")
         create_response = self._create_folder(library)
         self._assert_status_code_is(create_response, 200)
 
         with self._different_user():
             create_response = self._create_folder(library)
             self._assert_status_code_is(create_response, 403)
 
+    @requires_new_library
     def test_get_library_current_permissions(self):
         library = self.library_populator.new_library("GetCurrentPermissionTestLibrary")
         library_id = library["id"]
         current = self.library_populator.get_permissions(library_id, scope="current")
         self._assert_has_keys(
             current,
             "access_library_role_list",
@@ -141,23 +150,25 @@
         self.library_populator.set_permissions_with_action(library_id, role_id, action="set_permissions")
         current = self.library_populator.get_permissions(library_id, scope="current")
         assert role_id in current["access_library_role_list"][0]
         assert role_id in current["modify_library_role_list"][0]
         assert role_id in current["manage_library_role_list"][0]
         assert role_id in current["add_library_item_role_list"][0]
 
+    @requires_new_library
     def test_get_library_available_permissions(self):
         library = self.library_populator.new_library("GetAvailablePermissionTestLibrary")
         library_id = library["id"]
         role_id = self.library_populator.user_private_role_id()
         # As we can manage this library our role will be available
         available = self.library_populator.get_permissions(library_id, scope="available")
         available_role_ids = [role["id"] for role in available["roles"]]
         assert role_id in available_role_ids
 
+    @requires_new_library
     def test_get_library_available_permissions_with_query(self):
         library = self.library_populator.new_library("GetAvailablePermissionWithQueryTestLibrary")
         library_id = library["id"]
 
         with self._different_user():
             email = self.library_populator.user_email()
 
@@ -168,53 +179,57 @@
 
         # test query for specific role/email
         available = self.library_populator.get_permissions(library_id, scope="available", q=email)
         available_role_emails = [role["name"] for role in available["roles"]]
         assert available["total"] == 1
         assert available_role_emails[0] == email
 
+    @requires_new_library
     def test_create_library_dataset_bootstrap_user(self, library_name="private_dataset", wait=True):
         library = self.library_populator.new_private_library(library_name)
         payload, files = self.library_populator.create_dataset_request(library, file_type="txt", contents="create_test")
         create_response = self.galaxy_interactor.post(
             "libraries/%s/contents" % library["id"], payload, files=files, key=self.master_api_key
         )
         self._assert_status_code_is(create_response, 400)
 
+    @requires_new_library
     def test_create_dataset_denied(self):
         url, payload = self._create_dataset_kwargs()
         with self._different_user():
-            create_response = self._post(url, payload)
+            create_response = self._post(url, payload, json=True)
             self._assert_status_code_is(create_response, 403)
 
+    @requires_new_library
     def test_create_dataset_bootstrap_admin_user(self):
         url, payload = self._create_dataset_kwargs()
         with self._different_user():
-            create_response = self._post(url, payload, key=self.master_api_key)
+            create_response = self._post(url, payload, key=self.master_api_key, json=True)
             self._assert_status_code_is(create_response, 400)
 
     def _create_dataset_kwargs(self):
         library = self.library_populator.new_private_library("ForCreateDatasets")
         folder_response = self._create_folder(library)
         self._assert_status_code_is(folder_response, 200)
         folder_id = folder_response.json()[0]["id"]
         history_id = self.dataset_populator.new_history()
         hda_id = self.dataset_populator.new_dataset(history_id, content="1 2 3")["id"]
         return f"folders/{folder_id}/contents", {"from_hda_id": hda_id}
 
+    @requires_new_library
     def test_show_private_dataset_permissions(self):
         library, library_dataset = self.library_populator.new_library_dataset_in_private_library(
             "ForCreateDatasets", wait=True
         )
         with self._different_user():
-            with pytest.raises(requests.exceptions.HTTPError) as exc_info:
-                self.library_populator.show_ld(library["id"], library_dataset["id"])
-            # TODO: this should really be 403 and a proper JSON exception.
-            self._assert_status_code_is(exc_info.value.response, 400)
+            response = self.library_populator.show_ld_raw(library["id"], library_dataset["id"])
+            api_asserts.assert_status_code_is(response, 403)
+            api_asserts.assert_error_code_is(response, 403002)
 
+    @requires_new_library
     def test_create_dataset(self):
         library, library_dataset = self.library_populator.new_library_dataset_in_private_library(
             "ForCreateDatasets", wait=True
         )
         self._assert_has_keys(library_dataset, "peek", "data_type")
         assert library_dataset["peek"].find("create_test") >= 0
         assert library_dataset["file_ext"] == "txt", library_dataset["file_ext"]
@@ -225,14 +240,15 @@
         assert library_dataset_from_show["folder_id"] == library["root_folder_id"]
         # Get library dataset dataset association
         ldda = self.library_populator.show_ldda(library_dataset_from_show["ldda_id"])
         assert ldda["library_dataset_id"] == library_dataset["id"]
         assert ldda["parent_library_id"] == library["id"]
         assert ldda["file_ext"] == "txt"
 
+    @requires_new_library
     def test_fetch_upload_to_folder(self):
         history_id, library, destination = self._setup_fetch_to_folder("flat_zip")
         items = [{"src": "files", "dbkey": "hg19", "info": "my cool bed", "created_from_basename": "4.bed"}]
         targets = [{"destination": destination, "items": items}]
         payload = {
             "history_id": history_id,  # TODO: Shouldn't be needed :(
             "targets": targets,
@@ -242,14 +258,15 @@
         dataset = self.library_populator.get_library_contents_with_path(library["id"], "/4.bed")
         assert dataset["file_size"] == 61, dataset
         assert dataset["genome_build"] == "hg19", dataset
         assert dataset["misc_info"] == "my cool bed", dataset
         assert dataset["file_ext"] == "bed", dataset
         assert dataset["created_from_basename"] == "4.bed"
 
+    @requires_new_library
     def test_fetch_zip_to_folder(self):
         history_id, library, destination = self._setup_fetch_to_folder("flat_zip")
         bed_test_data_path = self.test_data_resolver.get_filename("4.bed.zip")
         targets = [
             {
                 "destination": destination,
                 "items_from": "archive",
@@ -261,24 +278,27 @@
             "targets": targets,
             "__files": {"files_0|file_data": open(bed_test_data_path, "rb")},
         }
         self.dataset_populator.fetch(payload)
         dataset = self.library_populator.get_library_contents_with_path(library["id"], "/4.bed")
         assert dataset["file_size"] == 61, dataset
 
+    @requires_new_library
     def test_fetch_single_url_to_folder(self):
         library, response = self.library_populator.fetch_single_url_to_folder()
         dataset = self.library_populator.get_library_contents_with_path(library["id"], "/4.bed")
         assert dataset["file_size"] == 61, dataset
 
+    @requires_new_library
     def test_fetch_single_url_with_invalid_datatype(self):
         _, response = self.library_populator.fetch_single_url_to_folder("xxx", assert_ok=False)
         self._assert_status_code_is(response, 400)
         assert response.json()["err_msg"] == "Requested extension 'xxx' unknown, cannot upload dataset."
 
+    @requires_new_library
     def test_legacy_upload_unknown_datatype(self):
         library = self.library_populator.new_private_library("ForLegacyUpload")
         folder_response = self._create_folder(library)
         self._assert_status_code_is(folder_response, 200)
         folder_id = folder_response.json()[0]["id"]
         payload = {
             "folder_id": folder_id,
@@ -288,14 +308,15 @@
             "files_0|url_paste": FILE_URL,
         }
         create_response = self._post(f"libraries/{library['id']}/contents", payload)
         self._assert_status_code_is(create_response, 400)
         assert create_response.json() == "Requested extension 'xxx' unknown, cannot upload dataset."
 
     @skip_if_github_down
+    @requires_new_library
     def test_fetch_failed_validation(self):
         # Exception handling is really rough here - we should be creating a dataset in error instead
         # of just failing the job like this.
         history_id, library, destination = self._setup_fetch_to_folder("single_url")
         items = [
             {
                 "src": "url",
@@ -323,14 +344,15 @@
         details = self.dataset_populator.get_job_details(job["id"]).json()
         assert details["state"] == "ok", details
 
         dataset = self.library_populator.get_library_contents_with_path(library["id"], "/4.bed")
         assert dataset["state"] == "error", dataset
 
     @skip_if_github_down
+    @requires_new_library
     def test_fetch_url_archive_to_folder(self):
         history_id, library, destination = self._setup_fetch_to_folder("single_url")
         targets = [
             {
                 "destination": destination,
                 "items_from": "archive",
                 "src": "url",
@@ -367,95 +389,104 @@
 
         dataset = self.library_populator.get_library_contents_with_path(library["id"], "/bdbag-profile.json")
         assert dataset["file_size"] == 723, dataset
 
     def _setup_fetch_to_folder(self, test_name):
         return self.library_populator.setup_fetch_to_folder(test_name)
 
+    @requires_new_library
     def test_create_dataset_in_folder(self):
         library = self.library_populator.new_private_library("ForCreateDatasets")
         folder_response = self._create_folder(library)
         self._assert_status_code_is(folder_response, 200)
         folder_id = folder_response.json()[0]["id"]
         history_id = self.dataset_populator.new_history()
         hda_id = self.dataset_populator.new_dataset(history_id, content="1 2 3")["id"]
         payload = {"from_hda_id": hda_id}
-        create_response = self._post(f"folders/{folder_id}/contents", payload)
+        create_response = self._post(f"folders/{folder_id}/contents", payload, json=True)
         self._assert_status_code_is(create_response, 200)
         self._assert_has_keys(create_response.json(), "name", "id")
 
+    @requires_new_library
     def test_create_dataset_in_subfolder(self):
         library = self.library_populator.new_private_library("ForCreateDatasets")
         folder_response = self._create_folder(library)
         self._assert_status_code_is(folder_response, 200)
         folder_id = folder_response.json()[0]["id"]
         subfolder_response = self._create_subfolder(folder_id)
         self._assert_status_code_is(folder_response, 200)
         print(subfolder_response.json())
         subfolder_id = subfolder_response.json()["id"]
         history_id = self.dataset_populator.new_history()
         hda_id = self.dataset_populator.new_dataset(history_id, content="1 2 3 sub")["id"]
         payload = {"from_hda_id": hda_id}
-        create_response = self._post(f"folders/{subfolder_id}/contents", payload)
+        create_response = self._post(f"folders/{subfolder_id}/contents", payload, json=True)
         self._assert_status_code_is(create_response, 200)
         self._assert_has_keys(create_response.json(), "name", "id")
         dataset_update_time = create_response.json()["update_time"]
         container_fetch_response = self.galaxy_interactor.get(f"folders/{folder_id}/contents")
         container_update_time = container_fetch_response.json()["folder_contents"][0]["update_time"]
         assert dataset_update_time == container_update_time, container_fetch_response
 
     def _patch_library_dataset(self, library_dataset_id, data):
         create_response = self._patch(f"libraries/datasets/{library_dataset_id}", data=data, json=True)
         self._assert_status_code_is(create_response, 200)
         ld = create_response.json()
         library_id = ld["parent_library_id"]
         return self.library_populator.wait_on_library_dataset(library_id, ld["id"])
 
+    @requires_new_library
     def test_update_dataset_in_folder(self):
         ld = self._create_dataset_in_folder_in_library("ForUpdateDataset", content=">seq\nATGC", wait=True).json()
         data = {
             "name": "updated_name",
             "file_ext": "fasta",
             "misc_info": "updated_info",
             "genome_build": "updated_genome_build",
         }
         ld_updated = self._patch_library_dataset(ld["id"], data)
         self._assert_has_keys(ld_updated, "name", "file_ext", "misc_info", "genome_build")
 
+    @requires_new_library
     def test_update_dataset_tags(self):
         ld = self._create_dataset_in_folder_in_library("ForTagtestDataset", wait=True).json()
         data = {"tags": ["#Lancelot", "name:Holy Grail", "blue"]}
         ld_updated = self._patch_library_dataset(ld["id"], data)
         self._assert_has_keys(ld_updated, "tags")
         assert ld_updated["tags"] == "name:Lancelot, name:HolyGrail, blue"
 
+    @requires_new_library
     def test_invalid_update_dataset_in_folder(self):
         ld = self._create_dataset_in_folder_in_library("ForInvalidUpdateDataset", wait=True).json()
         data = {"file_ext": "nonexisting_type"}
         create_response = self._patch(f"libraries/datasets/{ld['id']}", data=data, json=True)
         self._assert_status_code_is(create_response, 400)
         assert "This Galaxy does not recognize the datatype of:" in create_response.json()["err_msg"]
 
+    @requires_new_library
     def test_detect_datatype_of_dataset_in_folder(self):
         ld = self._create_dataset_in_folder_in_library("ForDetectDataset", wait=True).json()
         data = {"file_ext": "data"}
         ld_updated = self._patch_library_dataset(ld["id"], data)
         self._assert_has_keys(ld_updated, "file_ext")
         assert ld_updated["file_ext"] == "data"
         data = {"file_ext": "auto"}
         ld_updated = self._patch_library_dataset(ld["id"], data)
         self._assert_has_keys(ld_updated, "file_ext")
         assert ld_updated["file_ext"] == "txt"
 
+    @requires_new_library
     def test_ldda_collection_import_to_history(self):
         self._import_to_history(visible=True)
 
+    @requires_new_library
     def test_ldda_collection_import_to_history_hide_source(self):
         self._import_to_history(visible=False)
 
+    @requires_new_library
     def test_import_paired_collection(self):
         ld = self._create_dataset_in_folder_in_library("ForHistoryImport").json()
         history_id = self.dataset_populator.new_history()
         url = f"histories/{history_id}/contents"
         collection_name = "Paired-end data (from library)"
         payload = {
             "name": collection_name,
@@ -499,47 +530,49 @@
         new_collection = self._post(url, payload, json=True).json()
         assert new_collection["name"] == collection_name
         assert new_collection["element_count"] == 1
         element = new_collection["elements"][0]
         assert element["element_identifier"] == element_identifer
         assert element["object"]["visible"] == visible
 
+    @requires_new_library
     def test_create_datasets_in_library_from_collection(self):
         library = self.library_populator.new_private_library("ForCreateDatasetsFromCollection")
         folder_response = self._create_folder(library)
         self._assert_status_code_is(folder_response, 200)
         folder_id = folder_response.json()[0]["id"]
         history_id = self.dataset_populator.new_history()
         hdca_id = self.dataset_collection_populator.create_list_in_history(
             history_id, contents=["xxx", "yyy"], direct_upload=True, wait=True
         ).json()["outputs"][0]["id"]
         payload = {"from_hdca_id": hdca_id, "create_type": "file", "folder_id": folder_id}
         create_response = self._post(f"libraries/{library['id']}/contents", payload)
         self._assert_status_code_is(create_response, 200)
 
+    @requires_new_library
     def test_create_datasets_in_folder_from_collection(self):
         library = self.library_populator.new_private_library("ForCreateDatasetsFromCollection")
         history_id = self.dataset_populator.new_history()
         hdca_id = self.dataset_collection_populator.create_list_in_history(
             history_id, contents=["xxx", "yyy"], direct_upload=True, wait=True
         ).json()["outputs"][0]["id"]
         folder_response = self._create_folder(library)
         self._assert_status_code_is(folder_response, 200)
         folder_id = folder_response.json()[0]["id"]
         payload = {"from_hdca_id": hdca_id}
-        create_response = self._post(f"folders/{folder_id}/contents", payload)
+        create_response = self._post(f"folders/{folder_id}/contents", payload, json=True)
         self._assert_status_code_is(create_response, 200)
         assert len(create_response.json()) == 2
         # Also test that anything different from a flat dataset collection list
         # is refused
         hdca_pair_id = self.dataset_collection_populator.create_list_of_pairs_in_history(history_id, wait=True).json()[
             "outputs"
         ][0]["id"]
         payload = {"from_hdca_id": hdca_pair_id}
-        create_response = self._post(f"folders/{folder_id}/contents", payload)
+        create_response = self._post(f"folders/{folder_id}/contents", payload, json=True)
         self._assert_status_code_is(create_response, 501)
         assert (
             create_response.json()["err_msg"]
             == "Cannot add nested collections to library. Please flatten your collection first."
         )
 
     def _create_folder(self, library):
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_licenses.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_licenses.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ._framework import ApiTestCase
 
 
-class LicensesApiTestCase(ApiTestCase):
+class TestLicensesApi(ApiTestCase):
     def test_index(self):
         response = self._get("licenses")
         self._assert_status_code_is(response, 200)
 
     def test_get_license(self):
         licenseId = "Apache-2.0"
         response = self._get(f"licenses/{licenseId}")
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_page_revisions.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_page_revisions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from galaxy.exceptions import error_codes
-from .test_pages import BasePageApiTestCase
+from .test_pages import BasePagesApiTestCase
 
 
-class PageRevisionsApiTestCase(BasePageApiTestCase):
+class TestPageRevisionsApi(BasePagesApiTestCase):
     def test_create(self):
         page_json = self._create_valid_page_with_slug("pr1")
         revision_data = dict(content="<p>NewContent!</p>")
         page_revision_response = self._post(f"pages/{page_json['id']}/revisions", data=revision_data)
         self._assert_status_code_is(page_revision_response, 200)
         page_revision_json = page_revision_response.json()
         self._assert_has_keys(page_revision_json, "id", "content")
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_pages.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_pages.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 )
 from unittest import SkipTest
 
 from requests import delete
 from requests.models import Response
 
 from galaxy.exceptions import error_codes
+from galaxy_test.api._framework import ApiTestCase
 from galaxy_test.api.sharable import SharingApiTests
 from galaxy_test.base import api_asserts
 from galaxy_test.base.populators import (
     DatasetPopulator,
     skip_without_tool,
     WorkflowPopulator,
 )
-from ._framework import ApiTestCase
 
 
-class BasePageApiTestCase(ApiTestCase):
+class BasePagesApiTestCase(ApiTestCase):
+    dataset_populator: DatasetPopulator
+
     def setUp(self):
         super().setUp()
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
         self.workflow_populator = WorkflowPopulator(self.galaxy_interactor)
 
     def _create_valid_page_with_slug(self, slug):
         return self.dataset_populator.new_page(slug=slug)
@@ -37,16 +39,15 @@
         self._assert_status_code_is(page_response, 200)
         return page_response.json()
 
     def _test_page_payload(self, **kwds):
         return self.dataset_populator.new_page_payload(**kwds)
 
 
-class PageApiTestCase(BasePageApiTestCase, SharingApiTests):
-
+class TestPagesApi(BasePagesApiTestCase, SharingApiTests):
     api_name = "pages"
 
     def create(self, name: str) -> str:
         response_json = self._create_valid_page_with_slug(name)
         return response_json["id"]
 
     def test_create(self):
@@ -94,17 +95,17 @@
             page_response = self._post("pages", page_request, json=True)
             self._assert_status_code_is(page_response, 200)
             page_response = page_response.json()
             show_response = self._get(f"pages/{page_response['id']}")
             self._assert_status_code_is(show_response, 200)
             show_json = show_response.json()
             self._assert_has_keys(show_json, "slug", "title", "id")
-            self.assertEqual(show_json["slug"], "invocation-report")
-            self.assertEqual(show_json["title"], "Invocation Report")
-            self.assertEqual(show_json["content_format"], "markdown")
+            assert show_json["slug"] == "invocation-report"
+            assert show_json["title"] == "Invocation Report"
+            assert show_json["content_format"] == "markdown"
             markdown_content = show_json["content"]
             assert "## Workflow Outputs" in markdown_content
             assert "## Workflow Inputs" in markdown_content
             assert "## About This Report" not in markdown_content
 
     def test_index(self):
         create_response_json = self._create_valid_page_with_slug("indexpage")
@@ -165,17 +166,17 @@
         assert not self._users_index_has_page_with_id(response_shared, dict(show_shared=False))
         # make sure published workflows still enabled by default...
         assert self._users_index_has_page_with_id(response_published, dict(show_shared=False))
 
     def test_index_show_shared_with_me_deleted(self):
         user_id = self.dataset_populator.user_id()
         with self._different_user():
-            response_published = self._create_valid_page_with_slug("indexshowsharedpublished")
+            response_published = self._create_valid_page_with_slug("indexshowsharedpublisheddeleted")
             self._make_public(response_published["id"])
-            response_shared = self._create_valid_page_with_slug("indexshowsharedshared")
+            response_shared = self._create_valid_page_with_slug("indexshowsharedshareddeleted")
             self._share_with_user(response_shared["id"], user_id)
             self._delete(f"pages/{response_published['id']}").raise_for_status()
             self._delete(f"pages/{response_shared['id']}").raise_for_status()
 
         assert not self._users_index_has_page_with_id(response_shared, dict(show_shared=True, show_published=True))
         assert not self._users_index_has_page_with_id(response_published, dict(show_shared=True, show_published=True))
         assert not self._users_index_has_page_with_id(
@@ -303,18 +304,18 @@
 
     def test_show(self):
         response_json = self._create_valid_page_with_slug("pagetoshow")
         show_response = self._get(f"pages/{response_json['id']}")
         self._assert_status_code_is(show_response, 200)
         show_json = show_response.json()
         self._assert_has_keys(show_json, "slug", "title", "id")
-        self.assertEqual(show_json["slug"], "pagetoshow")
-        self.assertEqual(show_json["title"], "MY PAGE")
-        self.assertEqual(show_json["content"], "<p>Page!</p>")
-        self.assertEqual(show_json["content_format"], "html")
+        assert show_json["slug"] == "pagetoshow"
+        assert show_json["title"] == "MY PAGE"
+        assert show_json["content"] == "<p>Page!</p>"
+        assert show_json["content_format"] == "html"
 
     def test_403_on_unowner_show(self):
         response_json = self._create_valid_page_as("others_page_show@bx.psu.edu", "otherspageshow")
         show_response = self._get(f"pages/{response_json['id']}")
         self._assert_status_code_is(show_response, 403)
         self._assert_error_code_is(show_response, error_codes.error_codes_by_name["USER_CANNOT_ACCESS_ITEM"])
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_roles.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_roles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,40 @@
+from typing import (
+    Any,
+    Dict,
+    Optional,
+)
+
 from galaxy.exceptions import error_codes
 from galaxy_test.base.api_asserts import (
     assert_error_code_is,
     assert_has_keys,
     assert_status_code_is,
 )
+from galaxy_test.base.decorators import requires_admin
 from galaxy_test.base.populators import DatasetPopulator
 from ._framework import ApiTestCase
 
 
-class RolesApiTestCase(ApiTestCase):
+class TestRolesApi(ApiTestCase):
+    dataset_populator: DatasetPopulator
+
     def setUp(self):
         super().setUp()
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
 
+    @requires_admin
     def test_list_and_show(self):
         def check_roles_response(response):
             assert_status_code_is(response, 200)
             as_list = response.json()
             assert isinstance(as_list, list)
             assert len(as_list) > 0
             for role in as_list:
-                RolesApiTestCase.check_role_dict(role)
+                self.check_role_dict(role)
 
         user_role_id = self.dataset_populator.user_private_role_id()
         with self._different_user():
             different_user_role_id = self.dataset_populator.user_private_role_id()
 
         admin_roles_response = self._get("roles", admin=True)
         user_roles_response = self._get("roles")
@@ -42,16 +52,17 @@
         assert user_role_id in admin_roles_response_ids
         assert different_user_role_id in admin_roles_response_ids
 
         # Check showing a valid, role.
         role_response = self._get(f"roles/{user_role_id}")
         assert_status_code_is(role_response, 200)
         role = role_response.json()
-        RolesApiTestCase.check_role_dict(role, assert_id=user_role_id)
+        self.check_role_dict(role, assert_id=user_role_id)
 
+    @requires_admin
     def test_create_invalid_params(self):
         # In theory these low-level validation test cases could be handled in more
         # of a unit test style but it makes sense during the transition from wsgi to
         # asgi to have some tests that validate the whole pipeline is being integrated
         # properly in terms of exception handling.
 
         # Test missing description
@@ -63,48 +74,49 @@
         }
         response = self._post("roles", payload, admin=True, json=True)
         assert_status_code_is(response, 400)
         assert_error_code_is(response, error_codes.error_codes_by_name["USER_REQUEST_MISSING_PARAMETER"].code)
         assert "description" in response.json()["err_msg"]
 
         # Test missing name
-        payload = {
+        payload_missing_name = {
             "name": None,
             "description": description,
             "user_ids": [self.dataset_populator.user_id()],
         }
-        response = self._post("roles", payload, admin=True, json=True)
+        response = self._post("roles", payload_missing_name, admin=True, json=True)
         assert_status_code_is(response, 400)
         assert_error_code_is(response, error_codes.error_codes_by_name["USER_REQUEST_MISSING_PARAMETER"].code)
         assert "name" in response.json()["err_msg"]
 
         # Test invalid type for name
-        payload = {
+        payload_invalid_type = {
             "name": ["a test", "name"],
             "description": description,
             "user_ids": [self.dataset_populator.user_id()],
         }
-        response = self._post("roles", payload, admin=True, json=True)
+        response = self._post("roles", payload_invalid_type, admin=True, json=True)
         assert_status_code_is(response, 400)
         assert_error_code_is(response, error_codes.error_codes_by_name["USER_REQUEST_INVALID_PARAMETER"].code)
         assert "name" in response.json()["err_msg"]
         assert "validation_errors" in response.json()
 
+    @requires_admin
     def test_create_valid(self):
         name = self.dataset_populator.get_random_name()
         description = "A test role."
         payload = {
             "name": name,
             "description": description,
             "user_ids": [self.dataset_populator.user_id()],
         }
         response = self._post("roles", payload, admin=True, json=True)
         assert_status_code_is(response, 200)
         role = response.json()
-        RolesApiTestCase.check_role_dict(role)
+        self.check_role_dict(role)
 
         assert role["name"] == name
         assert role["description"] == description
 
         user_roles_response = self._get("roles")
         with self._different_user():
             different_user_roles_response = self._get("roles")
@@ -112,31 +124,33 @@
         user_roles_response_ids = [r["id"] for r in user_roles_response.json()]
         different_user_roles_response_ids = [r["id"] for r in different_user_roles_response.json()]
 
         # This new role is public, all users see it.
         assert role["id"] in user_roles_response_ids
         assert role["id"] in different_user_roles_response_ids
 
+    @requires_admin
     def test_show_error_codes(self):
         # Bad role ids are 400.
         response = self._get("roles/badroleid")
         assert_status_code_is(response, 400)
 
         # Trying to access roles are errors - should probably be 403 not 400 though?
         with self._different_user():
             different_user_role_id = self.dataset_populator.user_private_role_id()
         response = self._get(f"roles/{different_user_role_id}")
         assert_status_code_is(response, 400)
 
+    @requires_admin
     def test_create_only_admin(self):
         response = self._post("roles", json=True)
         assert_status_code_is(response, 403)
         response_err = response.json()
         assert response_err["err_code"] == 403006
         assert "administrator" in response_err["err_msg"]
 
     @staticmethod
-    def check_role_dict(role_dict, assert_id=None):
+    def check_role_dict(role_dict: Dict[str, Any], assert_id: Optional[str] = None) -> None:
         assert_has_keys(role_dict, "id", "name", "model_class", "url")
         assert role_dict["model_class"] == "Role"
         if assert_id is not None:
             assert role_dict["id"] == assert_id
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_search.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from requests import delete
 
 from galaxy_test.base.populators import WorkflowPopulator
 from ._framework import ApiTestCase
 
 
-class SearchApiTestCase(ApiTestCase):
+class TestSearchApi(ApiTestCase):
     def test_search_workflows(self):
         workflow_populator = WorkflowPopulator(self.galaxy_interactor)
         workflow_id = workflow_populator.simple_workflow("test_for_search")
         search_response = self.__search("select * from workflow")
         assert self.__has_result_with_name(search_response, "test_for_search"), search_response.text
 
         # Deleted
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_tool_data.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_tool_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 import operator
 
 from ._framework import ApiTestCase
 
 
-class ToolDataApiTestCase(ApiTestCase):
+class TestToolDataApi(ApiTestCase):
     def test_admin_only(self):
         index_response = self._get("tool_data", admin=False)
         self._assert_status_code_is(index_response, 403)
 
     def test_list(self):
         index_response = self._get("tool_data", admin=True)
         self._assert_status_code_is(index_response, 200)
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_tools.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 # Test tools API.
 import contextlib
 import json
 import os
 import zipfile
 from io import BytesIO
+from typing import (
+    Any,
+    Dict,
+    List,
+)
 
 import pytest
 from requests import (
     get,
     put,
 )
 
+from galaxy.tool_util.verify.interactor import ValidToolTestDict
 from galaxy.util import galaxy_root_path
+from galaxy.util.unittest_utils import skip_if_github_down
 from galaxy_test.base import rules_test_data
 from galaxy_test.base.api_asserts import (
     assert_has_keys,
     assert_status_code_is,
 )
+from galaxy_test.base.decorators import requires_new_history
 from galaxy_test.base.populators import (
     BaseDatasetCollectionPopulator,
-    BaseDatasetPopulator,
     DatasetCollectionPopulator,
     DatasetPopulator,
     LibraryPopulator,
-    skip_if_github_down,
     skip_without_tool,
     stage_rules_example,
-    uses_test_history,
 )
 from ._framework import ApiTestCase
 
 MINIMAL_TOOL = {
     "id": "minimal_tool",
     "name": "Minimal Tool",
     "class": "GalaxyTool",
@@ -50,15 +55,15 @@
     "outputs": dict(
         output1=dict(format="txt"),
     ),
 }
 
 
 class TestsTools:
-    dataset_populator: BaseDatasetPopulator
+    dataset_populator: DatasetPopulator
     dataset_collection_populator: BaseDatasetCollectionPopulator
 
     def _build_pair(self, history_id, contents):
         create_response = self.dataset_collection_populator.create_pair_in_history(
             history_id,
             contents=contents,
             direct_upload=True,
@@ -121,15 +126,17 @@
             create = create_response.json()
             assert_has_keys(create, "outputs")
             return create
         else:
             return create_response
 
 
-class ToolsTestCase(ApiTestCase, TestsTools):
+class TestToolsApi(ApiTestCase, TestsTools):
+    dataset_populator: DatasetPopulator
+
     def setUp(self):
         super().setUp()
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
         self.dataset_collection_populator = DatasetCollectionPopulator(self.galaxy_interactor)
 
     def test_index(self):
         tool_ids = self.__tool_ids()
@@ -162,15 +169,15 @@
         # No need to flatten out sections, with in_panel=False, only tools are
         # returned.
         tool_ids = [_["id"] for _ in tools_index]
         assert "upload1" in tool_ids
 
     @skip_without_tool("test_sam_to_bam_conversions")
     def test_requirements(self):
-        requirements_response = self._get(f"tools/{'test_sam_to_bam_conversions'}/requirements", admin=True)
+        requirements_response = self._get("tools/test_sam_to_bam_conversions/requirements", admin=True)
         self._assert_status_code_is_ok(requirements_response)
         requirements = requirements_response.json()
         assert len(requirements) == 1, requirements
         requirement = requirements[0]
         assert requirement["name"] == "samtools", requirement
 
     @skip_without_tool("cat1")
@@ -332,228 +339,230 @@
         tool_show_response = self._get(f"tools/{tool_id}", data=data)
         self._assert_status_code_is(tool_show_response, 200)
         tool_info = tool_show_response.json()
         self._assert_has_keys(tool_info, "inputs", "outputs", "panel_section_id")
         return tool_info
 
     @skip_without_tool("model_attributes")
-    @uses_test_history(require_new=False)
-    def test_model_attributes_sanitization(self, history_id):
-        cool_name_with_quote = 'cool name with a quo"te'
-        cool_name_without_quote = "cool name with a quo__dq__te"
-
-        current_user = self._get("users/current").json()
-        user_info_url = self._api_url(f"users/{current_user['id']}/information/inputs", use_key=True)
-        put_response = put(user_info_url, data=json.dumps({"address_0|desc": cool_name_with_quote}))
-        put_response.raise_for_status()
-
-        response = get(user_info_url).json()
-        self.assertEqual(len(response["addresses"]), 1)
-        self.assertEqual(response["addresses"][0]["desc"], cool_name_with_quote)
-
-        hda1 = self.dataset_populator.new_dataset(history_id, content="1\t2\t3", name=cool_name_with_quote)
-        assert hda1["name"] == cool_name_with_quote
-
-        rval = self._run(
-            tool_id="model_attributes",
-            inputs={"input1": dataset_to_param(hda1)},
-            history_id=history_id,
-            assert_ok=True,
-            wait_for_job=True,
-        )
-        sanitized_dataset_name = self.dataset_populator.get_history_dataset_content(
-            history_id, dataset=rval["outputs"][0]
-        )
-        assert sanitized_dataset_name.strip() == cool_name_without_quote
+    def test_model_attributes_sanitization(self):
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            cool_name_with_quote = 'cool name with a quo"te'
+            cool_name_without_quote = "cool name with a quo__dq__te"
+
+            current_user = self._get("users/current").json()
+            user_info_url = self._api_url(f"users/{current_user['id']}/information/inputs", use_key=True)
+            put_response = put(user_info_url, data=json.dumps({"address_0|desc": cool_name_with_quote}))
+            put_response.raise_for_status()
+
+            response = get(user_info_url).json()
+            assert len(response["addresses"]) == 1
+            assert response["addresses"][0]["desc"] == cool_name_with_quote
+
+            hda1 = self.dataset_populator.new_dataset(history_id, content="1\t2\t3", name=cool_name_with_quote)
+            assert hda1["name"] == cool_name_with_quote
+
+            rval = self._run(
+                tool_id="model_attributes",
+                inputs={"input1": dataset_to_param(hda1)},
+                history_id=history_id,
+                assert_ok=True,
+                wait_for_job=True,
+            )
+            sanitized_dataset_name = self.dataset_populator.get_history_dataset_content(
+                history_id, dataset=rval["outputs"][0]
+            )
+            assert sanitized_dataset_name.strip() == cool_name_without_quote
 
-        sanitized_email = self.dataset_populator.get_history_dataset_content(history_id, dataset=rval["outputs"][1])
-        assert '"' not in sanitized_email
+            sanitized_email = self.dataset_populator.get_history_dataset_content(history_id, dataset=rval["outputs"][1])
+            assert '"' not in sanitized_email
 
-        sanitized_address = self.dataset_populator.get_history_dataset_content(history_id, dataset=rval["outputs"][2])
-        assert sanitized_address.strip() == cool_name_without_quote
+            sanitized_address = self.dataset_populator.get_history_dataset_content(
+                history_id, dataset=rval["outputs"][2]
+            )
+            assert sanitized_address.strip() == cool_name_without_quote
 
     @skip_without_tool("composite_output")
     def test_test_data_filepath_security(self):
-        test_data_response = self._get(
-            f"tools/{'composite_output'}/test_data_path?filename=../CONTRIBUTORS.md", admin=True
-        )
+        test_data_response = self._get("tools/composite_output/test_data_path?filename=../CONTRIBUTORS.md", admin=True)
         assert test_data_response.status_code == 404, test_data_response.text
 
     @skip_without_tool("composite_output")
     def test_test_data_admin_security(self):
-        test_data_response = self._get(f"tools/{'composite_output'}/test_data_path?filename=../CONTRIBUTORS.md")
+        test_data_response = self._get("tools/composite_output/test_data_path?filename=../CONTRIBUTORS.md")
         assert test_data_response.status_code == 403, test_data_response.text
 
     @skip_without_tool("dbkey_filter_multi_input")
     def test_data_table_requirement_annotated(self):
-        test_data_response = self._get(f"tools/{'dbkey_filter_multi_input'}/test_data")
+        test_data_response = self._get("tools/dbkey_filter_multi_input/test_data")
         assert test_data_response.status_code == 200
         test_case = test_data_response.json()[0]
         assert test_case["required_data_tables"][0] == "test_fasta_indexes"
         assert len(test_case["required_loc_files"]) == 0
 
     @skip_without_tool("composite_output")
     def test_test_data_composite_output(self):
-        test_data_response = self._get(f"tools/{'composite_output'}/test_data")
+        test_data_response = self._get("tools/composite_output/test_data")
         assert test_data_response.status_code == 200
         test_data = test_data_response.json()
         assert len(test_data) == 1
         test_case = test_data[0]
         self._assert_has_keys(test_case, "inputs", "outputs", "output_collections", "required_files")
         assert len(test_case["inputs"]) == 1, test_case
         # input0 = next(iter(test_case["inputs"].values()))
 
     @skip_without_tool("collection_two_paired")
     def test_test_data_collection_two_paired(self):
-        test_data_response = self._get(f"tools/{'collection_two_paired'}/test_data")
+        test_data_response = self._get("tools/collection_two_paired/test_data")
         assert test_data_response.status_code == 200
         test_data = test_data_response.json()
         assert len(test_data) == 2
         test_case = test_data[0]
         assert len(test_case["required_data_tables"]) == 0
         assert len(test_case["required_loc_files"]) == 0
         self._assert_has_keys(test_case, "inputs", "outputs", "output_collections", "required_files")
         assert len(test_case["inputs"]) == 3, test_case
 
     @skip_without_tool("collection_nested_test")
     def test_test_data_collection_nested(self):
-        test_data_response = self._get(f"tools/{'collection_nested_test'}/test_data")
+        test_data_response = self._get("tools/collection_nested_test/test_data")
         assert test_data_response.status_code == 200
         test_data = test_data_response.json()
         assert len(test_data) == 2
         test_case = test_data[0]
         self._assert_has_keys(test_case, "inputs", "outputs", "output_collections", "required_files")
         assert len(test_case["inputs"]) == 1, test_case
 
-    @skip_without_tool("expression_null_handling_1")
+    @skip_without_tool("expression_null_handling_boolean")
     def test_test_data_null_boolean_inputs(self):
-        test_data_response = self._get(f"tools/{'expression_null_handling_1'}/test_data")
+        test_data_response = self._get("tools/expression_null_handling_boolean/test_data")
         assert test_data_response.status_code == 200
         test_data = test_data_response.json()
         assert len(test_data) == 3
         test_case = test_data[2]
         self._assert_has_keys(test_case, "inputs", "outputs", "output_collections", "required_files")
         inputs = test_case["inputs"]
         assert len(inputs) == 1, test_case
         assert "bool_input" in inputs, inputs
         assert inputs["bool_input"] is None, inputs
 
     @skip_without_tool("simple_constructs_y")
     def test_test_data_yaml_tools(self):
-        test_data_response = self._get(f"tools/{'simple_constructs_y'}/test_data")
+        test_data_response = self._get("tools/simple_constructs_y/test_data")
         assert test_data_response.status_code == 200
         test_data = test_data_response.json()
         assert len(test_data) == 3
 
     @skip_without_tool("cat1")
     def test_test_data_download(self):
-        test_data_response = self._get(f"tools/{'cat1'}/test_data_download?filename=1.bed")
+        test_data_response = self._get("tools/cat1/test_data_download?filename=1.bed")
         assert test_data_response.status_code == 200, test_data_response.text.startswith("chr")
 
     @skip_without_tool("composite_output")
     def test_test_data_downloads_security(self):
-        test_data_response = self._get(f"tools/{'composite_output'}/test_data_download?filename=../CONTRIBUTORS.md")
+        test_data_response = self._get("tools/composite_output/test_data_download?filename=../CONTRIBUTORS.md")
         assert test_data_response.status_code == 404, test_data_response.text
 
     @skip_without_tool("composite_output")
     def test_test_data_download_composite(self):
-        test_data_response = self._get(f"tools/{'composite_output'}/test_data_download?filename=velveth_test1")
+        test_data_response = self._get("tools/composite_output/test_data_download?filename=velveth_test1")
         assert test_data_response.status_code == 200
         with zipfile.ZipFile(BytesIO(test_data_response.content)) as contents:
             namelist = contents.namelist()
         assert len(namelist) == 6
         expected_names = {
             "velveth_test1/Roadmaps",
             "velveth_test1/output.html",
             "velveth_test1/Sequences",
             "velveth_test1/Log",
             "velveth_test1/output/",
             "velveth_test1/output/1",
         }
         assert set(namelist) == expected_names
 
-    @uses_test_history(require_new=False)
-    def test_convert_dataset_explicit_history(self, history_id):
-        fasta1_contents = open(self.get_filename("1.fasta")).read()
-        hda1 = self.dataset_populator.new_dataset(history_id, content=fasta1_contents)
-
-        payload = {
-            "src": "hda",
-            "id": hda1["id"],
-            "source_type": "fasta",
-            "target_type": "tabular",
-            "history_id": history_id,
-        }
-        create_response = self._post("tools/CONVERTER_fasta_to_tabular/convert", data=payload)
-        self.dataset_populator.wait_for_job(create_response.json()["jobs"][0]["id"], assert_ok=True)
-        create_response.raise_for_status()
-        assert len(create_response.json()["implicit_collections"]) == 0
-        for output in create_response.json()["outputs"]:
-            assert output["file_ext"] == "tabular"
-
-    @uses_test_history(require_new=False)
-    def test_convert_dataset_implicit_history(self, history_id):
-        fasta1_contents = open(self.get_filename("1.fasta")).read()
-        hda1 = self.dataset_populator.new_dataset(history_id, content=fasta1_contents)
-
-        payload = {"src": "hda", "id": hda1["id"], "source_type": "fasta", "target_type": "tabular"}
-        create_response = self._post("tools/CONVERTER_fasta_to_tabular/convert", data=payload)
-        self.dataset_populator.wait_for_job(create_response.json()["jobs"][0]["id"], assert_ok=True)
-        create_response.raise_for_status()
-        assert len(create_response.json()["implicit_collections"]) == 0
-        for output in create_response.json()["outputs"]:
-            assert output["file_ext"] == "tabular"
-
-    @uses_test_history(require_new=False)
-    def test_convert_hdca(self, history_id):
-        data = [
-            {
-                "name": "test0",
-                "elements": [
-                    {"src": "pasted", "paste_content": "123\n", "name": "forward", "ext": "fasta"},
-                    {"src": "pasted", "paste_content": "456\n", "name": "reverse", "ext": "fasta"},
-                ],
-            },
-            {
-                "name": "test1",
-                "elements": [
-                    {"src": "pasted", "paste_content": "789\n", "name": "forward", "ext": "fasta"},
-                    {"src": "pasted", "paste_content": "0ab\n", "name": "reverse", "ext": "fasta"},
-                ],
-            },
-        ]
-        hdca1 = self.dataset_collection_populator.upload_collection(history_id, "list:paired", elements=data, wait=True)
-        self._assert_status_code_is(hdca1, 200)
+    def test_convert_dataset_explicit_history(self):
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            fasta1_contents = open(self.get_filename("1.fasta")).read()
+            hda1 = self.dataset_populator.new_dataset(history_id, content=fasta1_contents)
+
+            payload = {
+                "src": "hda",
+                "id": hda1["id"],
+                "source_type": "fasta",
+                "target_type": "tabular",
+                "history_id": history_id,
+            }
+            create_response = self._post("tools/CONVERTER_fasta_to_tabular/convert", data=payload)
+            self.dataset_populator.wait_for_job(create_response.json()["jobs"][0]["id"], assert_ok=True)
+            create_response.raise_for_status()
+            assert len(create_response.json()["implicit_collections"]) == 0
+            for output in create_response.json()["outputs"]:
+                assert output["file_ext"] == "tabular"
+
+    def test_convert_dataset_implicit_history(self):
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            fasta1_contents = open(self.get_filename("1.fasta")).read()
+            hda1 = self.dataset_populator.new_dataset(history_id, content=fasta1_contents)
+
+            payload = {"src": "hda", "id": hda1["id"], "source_type": "fasta", "target_type": "tabular"}
+            create_response = self._post("tools/CONVERTER_fasta_to_tabular/convert", data=payload)
+            self.dataset_populator.wait_for_job(create_response.json()["jobs"][0]["id"], assert_ok=True)
+            create_response.raise_for_status()
+            assert len(create_response.json()["implicit_collections"]) == 0
+            for output in create_response.json()["outputs"]:
+                assert output["file_ext"] == "tabular"
+
+    def test_convert_hdca(self):
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            data = [
+                {
+                    "name": "test0",
+                    "elements": [
+                        {"src": "pasted", "paste_content": "123\n", "name": "forward", "ext": "fasta"},
+                        {"src": "pasted", "paste_content": "456\n", "name": "reverse", "ext": "fasta"},
+                    ],
+                },
+                {
+                    "name": "test1",
+                    "elements": [
+                        {"src": "pasted", "paste_content": "789\n", "name": "forward", "ext": "fasta"},
+                        {"src": "pasted", "paste_content": "0ab\n", "name": "reverse", "ext": "fasta"},
+                    ],
+                },
+            ]
+            hdca1 = self.dataset_collection_populator.upload_collection(
+                history_id, "list:paired", elements=data, wait=True
+            )
+            self._assert_status_code_is(hdca1, 200)
 
-        payload = {
-            "src": "hdca",
-            "id": hdca1.json()["outputs"][0]["id"],
-            "source_type": "fasta",
-            "target_type": "tabular",
-            "history_id": history_id,
-        }
-        create_response = self._post("tools/CONVERTER_fasta_to_tabular/convert", payload)
-        create_response.raise_for_status()
-        assert create_response.json()["implicit_collections"] != []
-        hid = create_response.json()["implicit_collections"][0]["hid"]
-        self.dataset_populator.wait_for_history(history_id, assert_ok=True)
-        collection_details = self.dataset_populator.get_history_collection_details(history_id, hid=hid)
-        for element in collection_details["elements"][0]["object"]["elements"]:
-            assert element["object"]["file_ext"] == "tabular"
+            payload = {
+                "src": "hdca",
+                "id": hdca1.json()["outputs"][0]["id"],
+                "source_type": "fasta",
+                "target_type": "tabular",
+                "history_id": history_id,
+            }
+            create_response = self._post("tools/CONVERTER_fasta_to_tabular/convert", payload)
+            create_response.raise_for_status()
+            assert create_response.json()["implicit_collections"] != []
+            hid = create_response.json()["implicit_collections"][0]["hid"]
+            self.dataset_populator.wait_for_history(history_id, assert_ok=True)
+            collection_details = self.dataset_populator.get_history_collection_details(history_id, hid=hid)
+            for element in collection_details["elements"][0]["object"]["elements"]:
+                assert element["object"]["file_ext"] == "tabular"
 
     def test_unzip_collection(self):
-        with self.dataset_populator.test_history() as history_id:
+        with self.dataset_populator.test_history(require_new=False) as history_id:
             hdca_id = self._build_pair(history_id, ["123", "456"])
             inputs = {
                 "input": {"src": "hdca", "id": hdca_id},
             }
             self.dataset_populator.wait_for_history(history_id, assert_ok=True)
             response = self._run("__UNZIP_COLLECTION__", history_id, inputs, assert_ok=True)
             outputs = response["outputs"]
-            self.assertEqual(len(outputs), 2)
+            assert len(outputs) == 2
             output_forward = outputs[0]
             output_reverse = outputs[1]
             output_forward_content = self.dataset_populator.get_history_dataset_content(
                 history_id, dataset=output_forward
             )
             output_reverse_content = self.dataset_populator.get_history_dataset_content(
                 history_id, dataset=output_reverse
@@ -564,15 +573,15 @@
             output_forward = self.dataset_populator.get_history_dataset_details(history_id, dataset=output_forward)
             output_reverse = self.dataset_populator.get_history_dataset_details(history_id, dataset=output_reverse)
 
             assert output_forward["history_id"] == history_id
             assert output_reverse["history_id"] == history_id
 
     def test_unzip_nested(self):
-        with self.dataset_populator.test_history() as history_id:
+        with self.dataset_populator.test_history(require_new=False) as history_id:
             response = self.dataset_collection_populator.upload_collection(
                 history_id,
                 "list:paired",
                 elements=[
                     {
                         "name": "test0",
                         "elements": [
@@ -601,104 +610,104 @@
                 "input": {
                     "batch": True,
                     "values": [{"src": "hdca", "map_over_type": "paired", "id": hdca_id}],
                 }
             }
             response = self._run("__UNZIP_COLLECTION__", history_id, inputs, assert_ok=True)
             implicit_collections = response["implicit_collections"]
-            self.assertEqual(len(implicit_collections), 2)
+            assert len(implicit_collections) == 2
             unzipped_hdca = self.dataset_populator.get_history_collection_details(
                 history_id, hid=implicit_collections[0]["hid"]
             )
             assert unzipped_hdca["elements"][0]["element_type"] == "hda", unzipped_hdca
 
     def test_zip_inputs(self):
-        with self.dataset_populator.test_history() as history_id:
+        with self.dataset_populator.test_history(require_new=False) as history_id:
             hda1 = dataset_to_param(self.dataset_populator.new_dataset(history_id, content="1\t2\t3"))
             hda2 = dataset_to_param(self.dataset_populator.new_dataset(history_id, content="4\t5\t6"))
             inputs = {
                 "input_forward": hda1,
                 "input_reverse": hda2,
             }
             self.dataset_populator.wait_for_history(history_id, assert_ok=True)
             response = self._run("__ZIP_COLLECTION__", history_id, inputs, assert_ok=True)
             output_collections = response["output_collections"]
-            self.assertEqual(len(output_collections), 1)
+            assert len(output_collections) == 1
             self.dataset_populator.wait_for_job(response["jobs"][0]["id"], assert_ok=True)
             zipped_hdca = self.dataset_populator.get_history_collection_details(
                 history_id, hid=output_collections[0]["hid"]
             )
             assert zipped_hdca["collection_type"] == "paired"
 
     @skip_without_tool("__ZIP_COLLECTION__")
-    @uses_test_history(require_new=False)
-    def test_collection_operation_dataset_input_permissions(self, history_id):
-        hda1 = dataset_to_param(self.dataset_populator.new_dataset(history_id, content="1\t2\t3"))
-        self.dataset_populator.wait_for_history(history_id, assert_ok=True)
-        self.dataset_populator.make_private(history_id, hda1["id"])
-        inputs = {
-            "input_forward": hda1,
-            "input_reverse": hda1,
-        }
-        with self._different_user_and_history() as other_history_id:
-            response = self._run("__ZIP_COLLECTION__", other_history_id, inputs, assert_ok=False)
-            self._assert_dataset_permission_denied_response(response)
+    def test_collection_operation_dataset_input_permissions(self):
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            hda1 = dataset_to_param(self.dataset_populator.new_dataset(history_id, content="1\t2\t3"))
+            self.dataset_populator.wait_for_history(history_id, assert_ok=True)
+            self.dataset_populator.make_private(history_id, hda1["id"])
+            inputs = {
+                "input_forward": hda1,
+                "input_reverse": hda1,
+            }
+            with self._different_user_and_history() as other_history_id:
+                response = self._run("__ZIP_COLLECTION__", other_history_id, inputs, assert_ok=False)
+                self._assert_dataset_permission_denied_response(response)
 
     @skip_without_tool("__UNZIP_COLLECTION__")
-    @uses_test_history(require_new=False)
-    def test_collection_operation_collection_input_permissions(self, history_id):
-        create_response = self.dataset_collection_populator.create_pair_in_history(
-            history_id, direct_upload=True, wait=True
-        )
-        self._assert_status_code_is(create_response, 200)
-        collection = create_response.json()["outputs"][0]
-        self.dataset_populator.wait_for_history(history_id, assert_ok=True)
-        collection = self.dataset_populator.get_history_collection_details(history_id, hid=collection["hid"])
-        element_id = collection["elements"][0]["object"]["id"]
-        self.dataset_populator.make_private(history_id, element_id)
-        inputs = {
-            "input": {"src": "hdca", "id": collection["id"]},
-        }
-        with self._different_user_and_history() as other_history_id:
-            response = self._run("__UNZIP_COLLECTION__", other_history_id, inputs, assert_ok=False)
-            self._assert_dataset_permission_denied_response(response)
+    def test_collection_operation_collection_input_permissions(self):
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            create_response = self.dataset_collection_populator.create_pair_in_history(
+                history_id, direct_upload=True, wait=True
+            )
+            self._assert_status_code_is(create_response, 200)
+            collection = create_response.json()["outputs"][0]
+            self.dataset_populator.wait_for_history(history_id, assert_ok=True)
+            collection = self.dataset_populator.get_history_collection_details(history_id, hid=collection["hid"])
+            element_id = collection["elements"][0]["object"]["id"]
+            self.dataset_populator.make_private(history_id, element_id)
+            inputs = {
+                "input": {"src": "hdca", "id": collection["id"]},
+            }
+            with self._different_user_and_history() as other_history_id:
+                response = self._run("__UNZIP_COLLECTION__", other_history_id, inputs, assert_ok=False)
+                self._assert_dataset_permission_denied_response(response)
 
     def test_zip_list_inputs(self):
-        with self.dataset_populator.test_history() as history_id:
+        with self.dataset_populator.test_history(require_new=False) as history_id:
             hdca1_id = self.dataset_collection_populator.create_list_in_history(
                 history_id, contents=["a\nb\nc\nd", "e\nf\ng\nh"], wait=True
             ).json()["outputs"][0]["id"]
 
             hdca2_id = self.dataset_collection_populator.create_list_in_history(
                 history_id, contents=["1\n2\n3\n4", "5\n6\n7\n8"], wait=True
             ).json()["outputs"][0]["id"]
             inputs = {
                 "input_forward": {"batch": True, "values": [{"src": "hdca", "id": hdca1_id}]},
                 "input_reverse": {"batch": True, "values": [{"src": "hdca", "id": hdca2_id}]},
             }
             self.dataset_populator.wait_for_history(history_id, assert_ok=True)
             response = self._run("__ZIP_COLLECTION__", history_id, inputs, assert_ok=True)
             implicit_collections = response["implicit_collections"]
-            self.assertEqual(len(implicit_collections), 1)
+            assert len(implicit_collections) == 1
             self.dataset_populator.wait_for_job(response["jobs"][0]["id"], assert_ok=True)
             zipped_hdca = self.dataset_populator.get_history_collection_details(
                 history_id, hid=implicit_collections[0]["hid"]
             )
             assert zipped_hdca["collection_type"] == "list:paired"
 
     @skip_without_tool("__FILTER_FAILED_DATASETS__")
     def test_filter_failed_list(self):
-        with self.dataset_populator.test_history() as history_id:
+        with self.dataset_populator.test_history(require_new=False) as history_id:
             ok_hdca_id = self.dataset_collection_populator.create_list_in_history(
                 history_id, contents=["0", "1", "0", "1"], wait=True
             ).json()["outputs"][0]["id"]
             response = self.dataset_populator.run_exit_code_from_file(history_id, ok_hdca_id)
 
             mixed_implicit_collections = response["implicit_collections"]
-            self.assertEqual(len(mixed_implicit_collections), 1)
+            assert len(mixed_implicit_collections) == 1
             mixed_hdca_hid = mixed_implicit_collections[0]["hid"]
             mixed_hdca = self.dataset_populator.get_history_collection_details(
                 history_id, hid=mixed_hdca_hid, wait=False
             )
 
             def get_state(dce):
                 return dce["object"]["state"]
@@ -708,28 +717,28 @@
 
             filtered_hdca = self._run_filter(history_id=history_id, failed_hdca_id=mixed_hdca["id"])
             filtered_states = [get_state(_) for _ in filtered_hdca["elements"]]
             assert filtered_states == ["ok", "ok"], filtered_states
 
     @skip_without_tool("__FILTER_FAILED_DATASETS__")
     def test_filter_failed_list_paired(self):
-        with self.dataset_populator.test_history() as history_id:
+        with self.dataset_populator.test_history(require_new=False) as history_id:
             pair1 = self.dataset_collection_populator.create_pair_in_history(
                 history_id, contents=["0", "0"], wait=True
             ).json()["outputs"][0]["id"]
             pair2 = self.dataset_collection_populator.create_pair_in_history(
                 history_id, contents=["0", "1"], wait=True
             ).json()["outputs"][0]["id"]
             ok_hdca_id = self.dataset_collection_populator.create_list_from_pairs(history_id, [pair1, pair2]).json()[
                 "id"
             ]
             response = self.dataset_populator.run_exit_code_from_file(history_id, ok_hdca_id)
 
             mixed_implicit_collections = response["implicit_collections"]
-            self.assertEqual(len(mixed_implicit_collections), 1)
+            assert len(mixed_implicit_collections) == 1
             mixed_hdca_hid = mixed_implicit_collections[0]["hid"]
             mixed_hdca = self.dataset_populator.get_history_collection_details(
                 history_id, hid=mixed_hdca_hid, wait=False
             )
 
             def get_state(dce):
                 return dce["object"]["state"]
@@ -770,28 +779,28 @@
                 "input": {"batch": batch, "src": "hdca", "id": failed_hdca_id},
             }
         response = self._run("__FILTER_FAILED_DATASETS__", history_id, inputs, assert_ok=False).json()
         self.dataset_populator.wait_for_history(history_id, assert_ok=False)
         filter_output_collections = response["output_collections"]
         if batch:
             return response["implicit_collections"][0]
-        self.assertEqual(len(filter_output_collections), 1)
+        assert len(filter_output_collections) == 1
         filtered_hid = filter_output_collections[0]["hid"]
         filtered_hdca = self.dataset_populator.get_history_collection_details(history_id, hid=filtered_hid, wait=False)
         return filtered_hdca
 
-    def _apply_rules_and_check(self, example):
-        with self.dataset_populator.test_history() as history_id:
+    def _apply_rules_and_check(self, example: Dict[str, Any]) -> None:
+        with self.dataset_populator.test_history(require_new=False) as history_id:
             inputs = stage_rules_example(self.galaxy_interactor, history_id, example)
             hdca = inputs["input"]
             inputs = {"input": {"src": "hdca", "id": hdca["id"]}, "rules": example["rules"]}
             self.dataset_populator.wait_for_history(history_id)
             response = self._run("__APPLY_RULES__", history_id, inputs, assert_ok=True)
             output_collections = response["output_collections"]
-            self.assertEqual(len(output_collections), 1)
+            assert len(output_collections) == 1
             output_hid = output_collections[0]["hid"]
             output_hdca = self.dataset_populator.get_history_collection_details(history_id, hid=output_hid, wait=False)
             example["check"](output_hdca, self.dataset_populator)
 
     def test_apply_rules_1(self):
         self._apply_rules_and_check(rules_test_data.EXAMPLE_1)
 
@@ -806,55 +815,72 @@
 
     def test_apply_rules_5(self):
         self._apply_rules_and_check(rules_test_data.EXAMPLE_5)
 
     def test_apply_rules_6(self):
         self._apply_rules_and_check(rules_test_data.EXAMPLE_6)
 
+    @skip_without_tool("galaxy_json_sleep")
+    def test_dataset_hidden_after_job_finish(self):
+        with self.dataset_populator.test_history() as history_id:
+            inputs = {
+                "sleep_time": 5,
+            }
+            response = self._run("galaxy_json_sleep", history_id, inputs, assert_ok=True)
+            output = response["outputs"][0]
+            response = self._put(
+                f"histories/{history_id}/contents/datasets/{output['id']}", data={"visible": False}, json=True
+            )
+            response.raise_for_status()
+            output_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=output, wait=False)
+            assert not output_details["visible"]
+            output_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=output, wait=True)
+            assert not output_details["visible"]
+
     @skip_without_tool("multi_select")
     def test_multi_select_as_list(self):
-        with self.dataset_populator.test_history() as history_id:
+        with self.dataset_populator.test_history(require_new=False) as history_id:
             inputs = {
                 "select_ex": ["--ex1", "ex2"],
             }
             response = self._run("multi_select", history_id, inputs, assert_ok=True)
             output = response["outputs"][0]
             output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output)
 
             assert output1_content == "--ex1,ex2"
 
     @skip_without_tool("multi_select")
     def test_multi_select_optional(self):
-        with self.dataset_populator.test_history() as history_id:
+        with self.dataset_populator.test_history(require_new=False) as history_id:
             inputs = {
                 "select_ex": ["--ex1"],
                 "select_optional": None,
             }
             response = self._run("multi_select", history_id, inputs, assert_ok=True)
             output = response["outputs"]
             output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output[0])
             output2_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output[1])
             assert output1_content.strip() == "--ex1"
             assert output2_content.strip() == "None", output2_content
 
     @skip_without_tool("library_data")
     def test_library_data_param(self):
-        with self.dataset_populator.test_history() as history_id:
+        with self.dataset_populator.test_history(require_new=False) as history_id:
             ld = LibraryPopulator(self.galaxy_interactor).new_library_dataset("lda_test_library")
             inputs = {"library_dataset": ld["ldda_id"], "library_dataset_multiple": [ld["ldda_id"], ld["ldda_id"]]}
             response = self._run("library_data", history_id, inputs, assert_ok=True)
             output = response["outputs"]
             output_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output[0])
             assert output_content == "TestData\n", output_content
             output_multiple_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output[1])
             assert output_multiple_content == "TestData\nTestData\n", output_multiple_content
 
     @skip_without_tool("multi_data_param")
     def test_multidata_param(self):
-        with self.dataset_populator.test_history() as history_id:
+        with self.dataset_populator.test_history(require_new=False) as history_id:
             hda1 = dataset_to_param(self.dataset_populator.new_dataset(history_id, content="1\t2\t3"))
             hda2 = dataset_to_param(self.dataset_populator.new_dataset(history_id, content="4\t5\t6"))
             inputs = {
                 "f1": {"batch": False, "values": [hda1, hda2]},
                 "f2": {"batch": False, "values": [hda2, hda1]},
             }
             response = self._run("multi_data_param", history_id, inputs, assert_ok=True)
@@ -862,145 +888,147 @@
             output2 = response["outputs"][1]
             output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
             output2_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output2)
             assert output1_content == "1\t2\t3\n4\t5\t6\n", output1_content
             assert output2_content == "4\t5\t6\n1\t2\t3\n", output2_content
 
     @skip_without_tool("cat1")
-    @uses_test_history(require_new=False)
-    def test_run_cat1(self, history_id):
-        # Run simple non-upload tool with an input data parameter.
-        new_dataset = self.dataset_populator.new_dataset(history_id, content="Cat1Test")
-        inputs = dict(
-            input1=dataset_to_param(new_dataset),
-        )
-        outputs = self._cat1_outputs(history_id, inputs=inputs)
-        self.assertEqual(len(outputs), 1)
-        output1 = outputs[0]
-        output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "Cat1Test")
+    def test_run_cat1(self):
+        with self.dataset_populator.test_history(require_new=False) as history_id:
+            # Run simple non-upload tool with an input data parameter.
+            new_dataset = self.dataset_populator.new_dataset(history_id, content="Cat1Test")
+            inputs = dict(
+                input1=dataset_to_param(new_dataset),
+            )
+            outputs = self._cat1_outputs(history_id, inputs=inputs)
+            assert len(outputs) == 1
+            output1 = outputs[0]
+            output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
+            assert output1_content.strip() == "Cat1Test"
 
     @skip_without_tool("cat1")
-    @uses_test_history(require_new=True)
-    def test_run_cat1_use_cached_job(self, history_id):
-        # Run simple non-upload tool with an input data parameter.
-        new_dataset = self.dataset_populator.new_dataset(history_id, content="Cat1Test")
-        inputs = dict(
-            input1=dataset_to_param(new_dataset),
-        )
-        outputs_one = self._run_cat1(history_id, inputs=inputs, assert_ok=True, wait_for_job=True)
-        outputs_two = self._run_cat1(history_id, inputs=inputs, use_cached_job=False, assert_ok=True, wait_for_job=True)
-        outputs_three = self._run_cat1(
-            history_id, inputs=inputs, use_cached_job=True, assert_ok=True, wait_for_job=True
-        )
-        dataset_details = []
-        for output in [outputs_one, outputs_two, outputs_three]:
-            output_id = output["outputs"][0]["id"]
-            dataset_details.append(self._get(f"datasets/{output_id}").json())
-        filenames = [dd["file_name"] for dd in dataset_details]
-        assert len(filenames) == 3, filenames
-        assert len(set(filenames)) <= 2, filenames
-
-    @skip_without_tool("cat1")
-    @uses_test_history(require_new=False)
-    def test_run_cat1_listified_param(self, history_id):
-        # Run simple non-upload tool with an input data parameter.
-        new_dataset = self.dataset_populator.new_dataset(history_id, content="Cat1Testlistified")
-        inputs = dict(
-            input1=[dataset_to_param(new_dataset)],
-        )
-        outputs = self._cat1_outputs(history_id, inputs=inputs)
-        self.assertEqual(len(outputs), 1)
-        output1 = outputs[0]
-        output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "Cat1Testlistified")
+    @requires_new_history
+    def test_run_cat1_use_cached_job(self):
+        with self.dataset_populator.test_history_for(self.test_run_cat1_use_cached_job) as history_id:
+            # Run simple non-upload tool with an input data parameter.
+            new_dataset = self.dataset_populator.new_dataset(history_id, content="Cat1Test")
+            inputs = dict(
+                input1=dataset_to_param(new_dataset),
+            )
+            outputs_one = self._run_cat1(history_id, inputs=inputs, assert_ok=True, wait_for_job=True)
+            outputs_two = self._run_cat1(
+                history_id, inputs=inputs, use_cached_job=False, assert_ok=True, wait_for_job=True
+            )
+            outputs_three = self._run_cat1(
+                history_id, inputs=inputs, use_cached_job=True, assert_ok=True, wait_for_job=True
+            )
+            dataset_details = []
+            for output in [outputs_one, outputs_two, outputs_three]:
+                output_id = output["outputs"][0]["id"]
+                dataset_details.append(self._get(f"datasets/{output_id}").json())
+            filenames = [dd["file_name"] for dd in dataset_details]
+            assert len(filenames) == 3, filenames
+            assert len(set(filenames)) <= 2, filenames
 
-    @skip_without_tool("multiple_versions")
-    @uses_test_history(require_new=False)
-    def test_run_by_versions(self, history_id):
-        for version in ["0.1", "0.2"]:
+    @skip_without_tool("cat1")
+    def test_run_cat1_listified_param(self):
+        with self.dataset_populator.test_history_for(self.test_run_cat1_listified_param) as history_id:
             # Run simple non-upload tool with an input data parameter.
-            outputs = self._run_and_get_outputs(
-                tool_id="multiple_versions", history_id=history_id, tool_version=version
+            new_dataset = self.dataset_populator.new_dataset(history_id, content="Cat1Testlistified")
+            inputs = dict(
+                input1=[dataset_to_param(new_dataset)],
             )
-            self.assertEqual(len(outputs), 1)
+            outputs = self._cat1_outputs(history_id, inputs=inputs)
+            assert len(outputs) == 1
             output1 = outputs[0]
             output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-            self.assertEqual(output1_content.strip(), f"Version {version}")
+            assert output1_content.strip() == "Cat1Testlistified"
+
+    @skip_without_tool("multiple_versions")
+    def test_run_by_versions(self):
+        with self.dataset_populator.test_history_for(self.test_run_by_versions) as history_id:
+            for version in ["0.1", "0.2"]:
+                # Run simple non-upload tool with an input data parameter.
+                outputs = self._run_and_get_outputs(
+                    tool_id="multiple_versions", history_id=history_id, tool_version=version
+                )
+                assert len(outputs) == 1
+                output1 = outputs[0]
+                output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
+                assert output1_content.strip() == f"Version {version}"
 
     @skip_without_tool("multiple_versions")
-    @uses_test_history(require_new=False)
-    def test_test_by_versions(self, history_id):
-        test_data_response = self._get(f"tools/{'multiple_versions'}/test_data")
+    def test_test_by_versions(self):
+        test_data_response = self._get("tools/multiple_versions/test_data")
         test_data_response.raise_for_status()
         test_data_dicts = test_data_response.json()
         assert len(test_data_dicts) == 1
         assert test_data_dicts[0]["tool_version"] == "0.2"
 
-        test_data_response = self._get(f"tools/{'multiple_versions'}/test_data?tool_version=*")
+        test_data_response = self._get("tools/multiple_versions/test_data?tool_version=*")
         test_data_response.raise_for_status()
         test_data_dicts = test_data_response.json()
         assert len(test_data_dicts) == 3
 
     @skip_without_tool("multiple_versions")
-    @uses_test_history(require_new=False)
-    def test_show_with_wrong_tool_version_in_tool_id(self, history_id):
+    def test_show_with_wrong_tool_version_in_tool_id(self):
         tool_info = self._show_valid_tool("multiple_versions", tool_version="0.01")
         # Return last version
         assert tool_info["version"] == "0.2"
 
     @skip_without_tool("cat1")
-    @uses_test_history(require_new=False)
-    def test_run_cat1_single_meta_wrapper(self, history_id):
-        # Wrap input in a no-op meta parameter wrapper like Sam is planning to
-        # use for all UI API submissions.
-        new_dataset = self.dataset_populator.new_dataset(history_id, content="123")
-        inputs = dict(
-            input1={"batch": False, "values": [dataset_to_param(new_dataset)]},
-        )
-        outputs = self._cat1_outputs(history_id, inputs=inputs)
-        self.assertEqual(len(outputs), 1)
-        output1 = outputs[0]
-        output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "123")
+    def test_run_cat1_single_meta_wrapper(self):
+        with self.dataset_populator.test_history_for(self.test_run_cat1_single_meta_wrapper) as history_id:
+            # Wrap input in a no-op meta parameter wrapper like Sam is planning to
+            # use for all UI API submissions.
+            new_dataset = self.dataset_populator.new_dataset(history_id, content="123")
+            inputs = dict(
+                input1={"batch": False, "values": [dataset_to_param(new_dataset)]},
+            )
+            outputs = self._cat1_outputs(history_id, inputs=inputs)
+            assert len(outputs) == 1
+            output1 = outputs[0]
+            output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
+            assert output1_content.strip() == "123"
 
     @skip_without_tool("cat1")
-    @uses_test_history(require_new=False)
-    def test_guess_derived_permissions(self, history_id):
-        def assert_inputs(inputs, can_be_used=True):
+    @requires_new_history
+    def test_guess_derived_permissions(self):
+        with self.dataset_populator.test_history_for(self.test_run_cat1_single_meta_wrapper) as history_id:
+
+            def assert_inputs(inputs, can_be_used=True):
+                # Until we make the dataset private, _different_user() can use it:
+                with self._different_user_and_history() as other_history_id:
+                    response = self._run("cat1", other_history_id, inputs)
+                    if can_be_used:
+                        assert response.status_code == 200
+                    else:
+                        self._assert_dataset_permission_denied_response(response)
+
+            new_dataset = self.dataset_populator.new_dataset(history_id, content="Cat1Test")
+            inputs = dict(
+                input1=dataset_to_param(new_dataset),
+            )
             # Until we make the dataset private, _different_user() can use it:
-            with self._different_user_and_history() as other_history_id:
-                response = self._run("cat1", other_history_id, inputs)
-                if can_be_used:
-                    assert response.status_code == 200
-                else:
-                    self._assert_dataset_permission_denied_response(response)
+            assert_inputs(inputs, can_be_used=True)
+            self.dataset_populator.make_private(history_id, new_dataset["id"])
+            # _different_user can no longer use the input dataset.
+            assert_inputs(inputs, can_be_used=False)
 
-        new_dataset = self.dataset_populator.new_dataset(history_id, content="Cat1Test")
-        inputs = dict(
-            input1=dataset_to_param(new_dataset),
-        )
-        # Until we make the dataset private, _different_user() can use it:
-        assert_inputs(inputs, can_be_used=True)
-        self.dataset_populator.make_private(history_id, new_dataset["id"])
-        # _different_user can no longer use the input dataset.
-        assert_inputs(inputs, can_be_used=False)
-
-        outputs = self._cat1_outputs(history_id, inputs=inputs)
-        self.assertEqual(len(outputs), 1)
-        output1 = outputs[0]
+            outputs = self._cat1_outputs(history_id, inputs=inputs)
+            assert len(outputs) == 1
+            output1 = outputs[0]
 
-        inputs_2 = dict(
-            input1=dataset_to_param(output1),
-        )
-        # _different_user cannot use datasets derived from the private input.
-        assert_inputs(inputs_2, can_be_used=False)
+            inputs_2 = dict(
+                input1=dataset_to_param(output1),
+            )
+            # _different_user cannot use datasets derived from the private input.
+            assert_inputs(inputs_2, can_be_used=False)
 
     @skip_without_tool("collection_creates_list")
-    @uses_test_history(require_new=False)
     def test_guess_derived_permissions_collections(self, history_id):
         def first_element_dataset_id(hdca):
             # Fetch full and updated details for HDCA
             print(hdca)
             full_hdca = self.dataset_populator.get_history_collection_details(history_id, hid=hdca["hid"])
             elements = full_hdca["elements"]
             element0 = elements[0]["object"]
@@ -1034,85 +1062,79 @@
             return "name" in contents_response
 
         with self._different_user():
             assert _dataset_accessible(public_element_id)
             assert not _dataset_accessible(private_element_id)
 
     @skip_without_tool("validation_default")
-    @uses_test_history(require_new=False)
     def test_validation(self, history_id):
         inputs = {
             "select_param": '" ; echo "moo',
         }
         response = self._run("validation_default", history_id, inputs)
         self._assert_status_code_is(response, 400)
 
     @skip_without_tool("validation_empty_dataset")
-    @uses_test_history(require_new=False)
     def test_validation_empty_dataset(self, history_id):
         outputs = self._run_and_get_outputs("empty_output", history_id)
         empty_dataset = outputs[0]
         inputs = {
             "input1": dataset_to_param(empty_dataset),
         }
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         response = self._run("validation_empty_dataset", history_id, inputs)
         self._assert_status_code_is(response, 400)
 
     @skip_without_tool("validation_repeat")
-    @uses_test_history(require_new=False)
     def test_validation_in_repeat(self, history_id):
         inputs = {
             "r1_0|text": "123",
             "r2_0|text": "",
         }
         response = self._run("validation_repeat", history_id, inputs)
         self._assert_status_code_is(response, 400)
 
     @skip_without_tool("multi_select")
-    @uses_test_history(require_new=False)
     def test_select_legal_values(self, history_id):
         inputs = {
             "select_ex": "not_option",
         }
         response = self._run("multi_select", history_id, inputs)
         self._assert_status_code_is(response, 400)
 
     @skip_without_tool("column_param")
-    @uses_test_history(require_new=False)
     def test_column_legal_values(self, history_id):
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="#col1\tcol2")
         inputs = {
             "input1": {"src": "hda", "id": new_dataset1["id"]},
             "col": "' ; echo 'moo",
         }
         response = self._run("column_param", history_id, inputs)
         # This needs to either fail at submit time or at job prepare time, but we have
         # to make sure the job doesn't run.
         if response.status_code == 200:
             job = response.json()["jobs"][0]
             final_job_state = self.dataset_populator.wait_for_job(job["id"])
             assert final_job_state == "error"
 
+    @requires_new_history
     @skip_without_tool("collection_paired_test")
-    @uses_test_history(require_new=True)
     def test_collection_parameter(self, history_id):
         hdca_id = self._build_pair(history_id, ["123\n", "456\n"])
         inputs = {
             "f1": {"src": "hdca", "id": hdca_id},
         }
         output = self._run("collection_paired_test", history_id, inputs, assert_ok=True)
         assert len(output["jobs"]) == 1
         assert len(output["implicit_collections"]) == 0
         assert len(output["outputs"]) == 1
         contents = self.dataset_populator.get_history_dataset_content(history_id, hid=4)
         assert contents.strip() == "123\n456", contents
 
     @skip_without_tool("collection_creates_pair")
-    @uses_test_history(require_new=False)
     def test_paired_collection_output(self, history_id):
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="123\n456\n789\n0ab")
         inputs = {
             "input1": {"src": "hda", "id": new_dataset1["id"]},
         }
         # TODO: shouldn't need this wait
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
@@ -1120,29 +1142,27 @@
         output_collection = self._assert_one_job_one_collection_run(create)
         element0, element1 = self._assert_elements_are(output_collection, "forward", "reverse")
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         self._verify_element(history_id, element0, contents="123\n789\n", file_ext="txt", visible=False)
         self._verify_element(history_id, element1, contents="456\n0ab\n", file_ext="txt", visible=False)
 
     @skip_without_tool("collection_creates_list")
-    @uses_test_history(require_new=False)
     def test_list_collection_output(self, history_id):
         create_response = self.dataset_collection_populator.create_list_in_history(
             history_id, contents=["a\nb\nc\nd", "e\nf\ng\nh"], wait=True
         )
         hdca_id = create_response.json()["outputs"][0]["id"]
         create = self.dataset_populator.run_collection_creates_list(history_id, hdca_id)
         output_collection = self._assert_one_job_one_collection_run(create)
         element0, element1 = self._assert_elements_are(output_collection, "data0", "data1")
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         self._verify_element(history_id, element0, contents="identifier is data0\n", file_ext="txt")
         self._verify_element(history_id, element1, contents="identifier is data1\n", file_ext="txt")
 
     @skip_without_tool("collection_creates_list_2")
-    @uses_test_history(require_new=False)
     def test_list_collection_output_format_source(self, history_id):
         # test using format_source with a tool
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="#col1\tcol2")
         create_response = self.dataset_collection_populator.create_list_in_history(
             history_id, contents=["a\tb\nc\td", "e\tf\ng\th"], wait=True
         )
         hdca_id = create_response.json()["outputs"][0]["id"]
@@ -1156,51 +1176,49 @@
         output_collection = self._assert_one_job_one_collection_run(create)
         element0, element1 = self._assert_elements_are(output_collection, "data0", "data1")
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         self._verify_element(history_id, element0, contents="#col1\tcol2\na\tb\nc\td\n", file_ext="txt")
         self._verify_element(history_id, element1, contents="#col1\tcol2\ne\tf\ng\th\n", file_ext="txt")
 
     @skip_without_tool("collection_split_on_column")
-    @uses_test_history(require_new=False)
     def test_dynamic_list_output(self, history_id):
         new_dataset1 = self.dataset_populator.new_dataset(
             history_id, content="samp1\t1\nsamp1\t3\nsamp2\t2\nsamp2\t4\n"
         )
         inputs = {
             "input1": dataset_to_param(new_dataset1),
         }
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         create = self._run("collection_split_on_column", history_id, inputs, assert_ok=True)
 
         output_collection = self._assert_one_job_one_collection_run(create)
         self._assert_has_keys(output_collection, "id", "name", "elements", "populated")
         assert not output_collection["populated"]
         assert len(output_collection["elements"]) == 0
-        self.assertEqual(output_collection["name"], "Table split on first column")
+        assert output_collection["name"] == "Table split on first column"
         self.dataset_populator.wait_for_job(create["jobs"][0]["id"], assert_ok=True)
 
         get_collection_response = self._get(
             f"dataset_collections/{output_collection['id']}", data={"instance_type": "history"}
         )
         self._assert_status_code_is(get_collection_response, 200)
 
         output_collection = get_collection_response.json()
         self._assert_has_keys(output_collection, "id", "name", "elements", "populated")
         assert output_collection["populated"]
-        self.assertEqual(output_collection["name"], "Table split on first column")
+        assert output_collection["name"] == "Table split on first column"
 
         assert len(output_collection["elements"]) == 2
         output_element_0 = output_collection["elements"][0]
         assert output_element_0["element_index"] == 0
         assert output_element_0["element_identifier"] == "samp1"
         output_element_hda_0 = output_element_0["object"]
         assert output_element_hda_0["metadata_column_types"] is not None
 
     @skip_without_tool("collection_creates_dynamic_nested")
-    @uses_test_history(require_new=False)
     def test_dynamic_list_output_datasets_in_failed_state(self, history_id):
         inputs = {"fail_bool": True}
         create = self._run("collection_creates_dynamic_nested", history_id, inputs, assert_ok=False, wait_for_job=True)
         self._assert_status_code_is(create, 200)
         collection = self._get(
             f"dataset_collections/{create.json()['output_collections'][0]['id']}", data={"instance_type": "history"}
         ).json()
@@ -1224,15 +1242,15 @@
 
         # Run tool.
         history_id = self.dataset_populator.new_history()
         self._run("minimal_tool", history_id)
 
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         output_content = self.dataset_populator.get_history_dataset_content(history_id)
-        self.assertEqual(output_content, "Hello World\n")
+        assert output_content == "Hello World\n"
 
     def test_dynamic_tool_from_path(self):
         # Create tool.
         dynamic_tool_path = os.path.join(
             galaxy_root_path, "lib", "galaxy_test", "base", "data", "minimal_tool_no_id.json"
         )
         tool_response = self.dataset_populator.create_tool_from_path(dynamic_tool_path)
@@ -1240,28 +1258,28 @@
 
         # Run tool.
         history_id = self.dataset_populator.new_history()
         self._run(history_id=history_id, tool_uuid=tool_response["uuid"])
 
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         output_content = self.dataset_populator.get_history_dataset_content(history_id)
-        self.assertEqual(output_content, "Hello World 2\n")
+        assert output_content == "Hello World 2\n"
 
     def test_dynamic_tool_no_id(self):
         # Create tool.
         tool_response = self.dataset_populator.create_tool(MINIMAL_TOOL_NO_ID)
         self._assert_has_keys(tool_response, "uuid")
 
         # Run tool.
         history_id = self.dataset_populator.new_history()
         self._run(history_id=history_id, tool_uuid=tool_response["uuid"])
 
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         output_content = self.dataset_populator.get_history_dataset_content(history_id)
-        self.assertEqual(output_content, "Hello World 2\n")
+        assert output_content == "Hello World 2\n"
 
     def test_show_dynamic_tools(self):
         # Create tool.
         original_list = self.dataset_populator.list_dynamic_tools()
         created_dynamic_tool_dict = self.dataset_populator.create_tool(MINIMAL_TOOL_NO_ID)
         self._assert_has_keys(created_dynamic_tool_dict, "id", "uuid", "active")
         created_id = created_dynamic_tool_dict["id"]
@@ -1305,28 +1323,26 @@
         # Run tool.
         history_id = self.dataset_populator.new_history()
         response = self._run(history_id=history_id, tool_uuid=tool_response["uuid"], assert_ok=False)
         # Get a 404 when trying to run a deactivated tool.
         self._assert_status_code_is(response, 404)
 
     @skip_without_tool("cat1")
-    @uses_test_history(require_new=False)
     def test_run_cat1_with_two_inputs(self, history_id):
         # Run tool with an multiple data parameter and grouping (repeat)
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="Cat1Test")
         new_dataset2 = self.dataset_populator.new_dataset(history_id, content="Cat2Test")
         inputs = {"input1": dataset_to_param(new_dataset1), "queries_0|input2": dataset_to_param(new_dataset2)}
         outputs = self._cat1_outputs(history_id, inputs=inputs)
-        self.assertEqual(len(outputs), 1)
+        assert len(outputs) == 1
         output1 = outputs[0]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "Cat1Test\nCat2Test")
+        assert output1_content.strip() == "Cat1Test\nCat2Test"
 
     @skip_without_tool("mapper_two")
-    @uses_test_history(require_new=False)
     def test_bam_state_regression(self, history_id):
         # Test regression of https://github.com/galaxyproject/galaxy/issues/6856. With changes
         # to metadata file flushing to optimize creating bam outputs and copying bam datasets
         # we observed very subtle problems with HDA state changes on other files being flushed at
         # the same time. This tests txt datasets finalized before and after the bam outputs as
         # well as other bam files all flush properly during job completion.
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="123\n456\n789")
@@ -1337,15 +1353,14 @@
         outputs = self._run_and_get_outputs("mapper_two", history_id, inputs)
         assert len(outputs) == 4
         for output in outputs:
             details = self.dataset_populator.get_history_dataset_details(history_id, dataset=output)
             assert details["state"] == "ok"
 
     @skip_without_tool("qc_stdout")
-    @uses_test_history(require_new=False)
     def test_qc_messages(self, history_id):
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="123\n456\n789")
         inputs = {
             "input1": dataset_to_param(new_dataset1),
             "quality": 3,
         }
         create = self._run("qc_stdout", history_id, inputs, wait_for_job=True, assert_ok=True)
@@ -1356,39 +1371,37 @@
         qc_message = details["job_messages"][0]
         # assert qc_message["code_desc"] == "QC Metrics for Tool", qc_message
         assert qc_message["desc"] == "QC: Matched on Quality of sample is 30%."
         assert qc_message["match"] == "Quality of sample is 30%."
         assert qc_message["error_level"] == 1.1
 
     @skip_without_tool("cat1")
-    @uses_test_history(require_new=False)
     def test_multirun_cat1(self, history_id):
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="123")
         new_dataset2 = self.dataset_populator.new_dataset(history_id, content="456")
         datasets = [dataset_to_param(new_dataset1), dataset_to_param(new_dataset2)]
         inputs = {
             "input1": {
                 "batch": True,
                 "values": datasets,
             },
         }
         self._check_cat1_multirun(history_id, inputs)
 
     def _check_cat1_multirun(self, history_id, inputs):
         outputs = self._cat1_outputs(history_id, inputs=inputs)
-        self.assertEqual(len(outputs), 2)
+        assert len(outputs) == 2
         output1 = outputs[0]
         output2 = outputs[1]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
         output2_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output2)
-        self.assertEqual(output1_content.strip(), "123")
-        self.assertEqual(output2_content.strip(), "456")
+        assert output1_content.strip() == "123"
+        assert output2_content.strip() == "456"
 
     @skip_without_tool("random_lines1")
-    @uses_test_history(require_new=False)
     def test_multirun_non_data_parameter(self, history_id):
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="123\n456\n789")
         inputs = {"input": dataset_to_param(new_dataset1), "num_lines": {"batch": True, "values": [1, 2, 3]}}
         outputs = self._run_and_get_outputs("random_lines1", history_id, inputs)
         # Assert we have three outputs with 1, 2, and 3 lines respectively.
         assert len(outputs) == 3
         outputs_contents = [
@@ -1418,15 +1431,15 @@
     def test_multirun_on_multiple_inputs(self):
         history_id, first_two, second_two = self._setup_two_multiruns()
         inputs = {
             "input1": {"batch": True, "values": first_two},
             "queries_0|input2": {"batch": True, "values": second_two},
         }
         outputs = self._cat1_outputs(history_id, inputs=inputs)
-        self.assertEqual(len(outputs), 2)
+        assert len(outputs) == 2
         outputs_contents = [
             self.dataset_populator.get_history_dataset_content(history_id, dataset=o).strip() for o in outputs
         ]
         assert "123\n789" in outputs_contents
         assert "456\n0ab" in outputs_contents
 
     @skip_without_tool("cat1")
@@ -1436,92 +1449,97 @@
             "input1": {"batch": True, "linked": False, "values": first_two},
             "queries_0|input2": {"batch": True, "linked": False, "values": second_two},
         }
         outputs = self._cat1_outputs(history_id, inputs=inputs)
         outputs_contents = [
             self.dataset_populator.get_history_dataset_content(history_id, dataset=o).strip() for o in outputs
         ]
-        self.assertEqual(len(outputs), 4)
+        assert len(outputs) == 4
         assert "123\n789" in outputs_contents
         assert "456\n0ab" in outputs_contents
         assert "123\n0ab" in outputs_contents
         assert "456\n789" in outputs_contents
 
     @skip_without_tool("dbkey_output_action")
     def test_dynamic_parameter_error_handling(self):
         # Run test with valid index once, then supply invalid dbkey and invalid table
         # entry to ensure dynamic param errors are register.
         job_data_list = []
 
         def register_job_data(job_data):
             job_data_list.append(job_data)
 
-        tool_test_dicts = [
+        def tool_test_case_list(inputs, required_files) -> List[ValidToolTestDict]:
+            return [
+                {
+                    "inputs": inputs,
+                    "outputs": {},
+                    "required_files": required_files,
+                    "output_collections": [],
+                    "test_index": 0,
+                    "tool_version": "0.1.0",
+                    "tool_id": "dbkey_output_action",
+                    "error": False,
+                }
+            ]
+
+        tool_test_dicts = tool_test_case_list(
             {
-                "inputs": {
-                    "input": ["simple_line.txt"],
-                    "index": ["hg18_value"],
-                },
-                "outputs": {},
-                "required_files": [["simple_line.txt", {"value": "simple_line.txt", "dbkey": "hg18"}]],
-            }
-        ]
+                "input": ["simple_line.txt"],
+                "index": ["hg18_value"],
+            },
+            [["simple_line.txt", {"value": "simple_line.txt", "dbkey": "hg18"}]],
+        )
         dynamic_param_error = None
         test_driver = self.driver_or_skip_test_if_remote()
         try:
-            test_driver.run_tool_test("dbkey_output_action", tool_test_dicts=tool_test_dicts)
+            test_driver.run_tool_test("dbkey_output_action", _tool_test_dicts=tool_test_dicts)
         except Exception as e:
             dynamic_param_error = getattr(e, "dynamic_param_error", False)
         assert dynamic_param_error is None
 
-        tool_test_dicts = [
+        tool_test_dicts = tool_test_case_list(
             {
-                "inputs": {
-                    "input": ["simple_line.txt"],
-                    "index": ["hg18_value"],
-                },
-                "outputs": {},
-                "required_files": [["simple_line.txt", {"value": "simple_line.txt", "dbkey": "hgnot18"}]],
-            }
-        ]
+                "input": ["simple_line.txt"],
+                "index": ["hg18_value"],
+            },
+            [["simple_line.txt", {"value": "simple_line.txt", "dbkey": "hgnot18"}]],
+        )
         dynamic_param_error = None
         try:
-            test_driver.run_tool_test("dbkey_output_action", tool_test_dicts=tool_test_dicts)
+            test_driver.run_tool_test("dbkey_output_action", _tool_test_dicts=tool_test_dicts)
         except Exception as e:
             dynamic_param_error = getattr(e, "dynamic_param_error", False)
         assert dynamic_param_error
 
-        tool_test_dicts = [
+        tool_test_dicts = tool_test_case_list(
             {
-                "inputs": {
-                    "input": ["simple_line.txt"],
-                    "index": ["hgnot18"],
-                },
-                "outputs": {},
-                "required_files": [["simple_line.txt", {"value": "simple_line.txt", "dbkey": "hg18"}]],
-            }
-        ]
+                "input": ["simple_line.txt"],
+                "index": ["hgnot18"],
+            },
+            [["simple_line.txt", {"value": "simple_line.txt", "dbkey": "hg18"}]],
+        )
         dynamic_param_error = None
         try:
             test_driver.run_tool_test(
-                "dbkey_output_action", tool_test_dicts=tool_test_dicts, register_job_data=register_job_data
+                "dbkey_output_action", _tool_test_dicts=tool_test_dicts, register_job_data=register_job_data
             )
         except Exception as e:
             dynamic_param_error = getattr(e, "dynamic_param_error", False)
         assert dynamic_param_error
         assert len(job_data_list) == 1
         job_data = job_data_list[0]
         assert job_data["status"] == "error"
         job_data_list.clear()
 
         dynamic_param_error = None
         try:
             test_driver.run_tool_test(
                 "dbkey_output_action",
-                tool_test_dicts=tool_test_dicts,
+                _tool_test_dicts=tool_test_dicts,
                 skip_on_dynamic_param_errors=True,
                 register_job_data=register_job_data,
             )
         except Exception as e:
             dynamic_param_error = getattr(e, "dynamic_param_error", False)
         assert dynamic_param_error
         assert len(job_data_list) == 1
@@ -1529,504 +1547,479 @@
         assert job_data["status"] == "skip"
 
     def _assert_one_job_one_collection_run(self, create):
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
         collections = create["output_collections"]
 
-        self.assertEqual(len(jobs), 1)
-        self.assertEqual(len(implicit_collections), 0)
-        self.assertEqual(len(collections), 1)
+        assert len(jobs) == 1
+        assert len(implicit_collections) == 0
+        assert len(collections) == 1
 
         output_collection = collections[0]
         return output_collection
 
     def _assert_elements_are(self, collection, *args):
         elements = collection["elements"]
-        self.assertEqual(len(elements), len(args))
+        assert len(elements) == len(args)
         for index, element in enumerate(elements):
             arg = args[index]
-            self.assertEqual(arg, element["element_identifier"])
+            assert arg == element["element_identifier"]
         return elements
 
     def _verify_element(self, history_id, element, **props):
         object_id = element["object"]["id"]
 
         if "contents" in props:
             expected_contents = props["contents"]
 
             contents = self.dataset_populator.get_history_dataset_content(history_id, dataset_id=object_id)
-            self.assertEqual(contents, expected_contents)
+            assert contents == expected_contents
 
             del props["contents"]
 
         if props:
             details = self.dataset_populator.get_history_dataset_details(history_id, dataset_id=object_id)
             for key, value in props.items():
-                self.assertEqual(details[key], value)
+                assert details[key] == value
 
     def _setup_repeat_multirun(self):
         history_id = self.dataset_populator.new_history()
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="123")
         new_dataset2 = self.dataset_populator.new_dataset(history_id, content="456")
         common_dataset = self.dataset_populator.new_dataset(history_id, content="Common")
         return (
             history_id,
             dataset_to_param(common_dataset),
             [dataset_to_param(new_dataset1), dataset_to_param(new_dataset2)],
         )
 
     def _check_repeat_multirun(self, history_id, inputs):
         outputs = self._cat1_outputs(history_id, inputs=inputs)
-        self.assertEqual(len(outputs), 2)
+        assert len(outputs) == 2
         output1 = outputs[0]
         output2 = outputs[1]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
         output2_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output2)
-        self.assertEqual(output1_content.strip(), "Common\n123")
-        self.assertEqual(output2_content.strip(), "Common\n456")
+        assert output1_content.strip() == "Common\n123"
+        assert output2_content.strip() == "Common\n456"
 
     def _setup_two_multiruns(self):
         history_id = self.dataset_populator.new_history()
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="123")
         new_dataset2 = self.dataset_populator.new_dataset(history_id, content="456")
         new_dataset3 = self.dataset_populator.new_dataset(history_id, content="789")
         new_dataset4 = self.dataset_populator.new_dataset(history_id, content="0ab")
         return (
             history_id,
             [dataset_to_param(new_dataset1), dataset_to_param(new_dataset2)],
             [dataset_to_param(new_dataset3), dataset_to_param(new_dataset4)],
         )
 
     @skip_without_tool("cat")
-    @uses_test_history(require_new=False)
     def test_map_over_collection(self, history_id):
         hdca_id = self._build_pair(history_id, ["123", "456"])
         inputs = {
             "input1": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
         }
         self._run_and_check_simple_collection_mapping(history_id, inputs)
 
     @skip_without_tool("cat1")
-    @uses_test_history(require_new=False)
     def test_map_over_empty_collection(self, history_id):
         hdca_id = self.dataset_collection_populator.create_list_in_history(history_id, contents=[]).json()["outputs"][
             0
         ]["id"]
         inputs = {
             "input1": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
         }
         create = self._run_cat1(history_id, inputs=inputs, assert_ok=True)
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 0)
-        self.assertEqual(len(outputs), 0)
-        self.assertEqual(len(implicit_collections), 1)
+        assert len(jobs) == 0
+        assert len(outputs) == 0
+        assert len(implicit_collections) == 1
 
         empty_output = implicit_collections[0]
         assert empty_output["name"] == "Concatenate datasets on collection 1", empty_output
 
     @skip_without_tool("output_action_change_format")
-    @uses_test_history(require_new=False)
     def test_map_over_with_output_format_actions(self, history_id):
         for use_action in ["do", "dont"]:
             hdca_id = self._build_pair(history_id, ["123", "456"])
             inputs = {
                 "input_cond|dispatch": use_action,
                 "input_cond|input": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
             }
             create = self._run("output_action_change_format", history_id, inputs).json()
             outputs = create["outputs"]
             jobs = create["jobs"]
             implicit_collections = create["implicit_collections"]
-            self.assertEqual(len(jobs), 2)
-            self.assertEqual(len(outputs), 2)
-            self.assertEqual(len(implicit_collections), 1)
+            assert len(jobs) == 2
+            assert len(outputs) == 2
+            assert len(implicit_collections) == 1
             output1 = outputs[0]
             output2 = outputs[1]
             output1_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=output1)
             output2_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=output2)
             assert output1_details["file_ext"] == "txt" if (use_action == "do") else "data"
             assert output2_details["file_ext"] == "txt" if (use_action == "do") else "data"
 
     @skip_without_tool("output_action_change_format_paired")
-    @uses_test_history(require_new=False)
     def test_map_over_with_nested_paired_output_format_actions(self, history_id):
         hdca_id = self.__build_nested_list(history_id)
         inputs = {"input": {"batch": True, "values": [dict(map_over_type="paired", src="hdca", id=hdca_id)]}}
         create = self._run("output_action_change_format_paired", history_id, inputs).json()
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 2)
-        self.assertEqual(len(outputs), 2)
-        self.assertEqual(len(implicit_collections), 1)
+        assert len(jobs) == 2
+        assert len(outputs) == 2
+        assert len(implicit_collections) == 1
         for output in outputs:
             assert output["file_ext"] == "txt", output
 
     @skip_without_tool("output_filter_with_input")
-    @uses_test_history(require_new=False)
     def test_map_over_with_output_filter_no_filtering(self, history_id):
         hdca_id = self.dataset_collection_populator.create_list_in_history(history_id, wait=True).json()["outputs"][0][
             "id"
         ]
         inputs = {
             "input_1": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
             "produce_out_1": "true",
             "filter_text_1": "foo",
         }
         create = self._run("output_filter_with_input", history_id, inputs).json()
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 3)
-        self.assertEqual(len(implicit_collections), 3)
+        assert len(jobs) == 3
+        assert len(implicit_collections) == 3
         self._check_implicit_collection_populated(create)
 
     @skip_without_tool("output_filter_with_input_optional")
-    @uses_test_history(require_new=False)
     def test_map_over_with_output_filter_on_optional_input(self, history_id):
         hdca_id = self.dataset_collection_populator.create_list_in_history(
             history_id, contents=["myinputs"], wait=True
         ).json()["outputs"][0]["id"]
         inputs = {
             "input_1": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
         }
         create = self._run("output_filter_with_input_optional", history_id, inputs).json()
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 1)
+        assert len(jobs) == 1
         self.dataset_populator.wait_for_job(jobs[0]["id"], assert_ok=True)
-        self.assertEqual(len(implicit_collections), 1)
+        assert len(implicit_collections) == 1
         self._check_implicit_collection_populated(create)
 
     @skip_without_tool("output_filter_with_input")
-    @uses_test_history(require_new=False)
     def test_map_over_with_output_filter_one_filtered(self, history_id):
         hdca_id = self.dataset_collection_populator.create_list_in_history(history_id, wait=True).json()["outputs"][0][
             "id"
         ]
         inputs = {
             "input_1": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
             "produce_out_1": "true",
             "filter_text_1": "bar",
         }
         create = self._run("output_filter_with_input", history_id, inputs).json()
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 3)
-        self.assertEqual(len(implicit_collections), 2)
+        assert len(jobs) == 3
+        assert len(implicit_collections) == 2
         self._check_implicit_collection_populated(create)
 
     @skip_without_tool("Cut1")
-    @uses_test_history(require_new=False)
     def test_map_over_with_complex_output_actions(self, history_id):
         hdca_id = self._bed_list(history_id)
         inputs = {
             "columnList": "c1,c2,c3,c4,c5",
             "delimiter": "T",
             "input": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
         }
         create = self._run("Cut1", history_id, inputs).json()
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 2)
-        self.assertEqual(len(outputs), 2)
-        self.assertEqual(len(implicit_collections), 1)
+        assert len(jobs) == 2
+        assert len(outputs) == 2
+        assert len(implicit_collections) == 1
         output1 = outputs[0]
         output2 = outputs[1]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
         output2_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output2)
         assert output1_content.startswith("chr1")
         assert output2_content.startswith("chr1")
 
     @skip_without_tool("collection_creates_dynamic_list_of_pairs")
-    @uses_test_history(require_new=False)
     def test_map_over_with_discovered_output_collection_elements(self, history_id):
         hdca_id = self.dataset_collection_populator.create_list_in_history(history_id, wait=True).json()["outputs"][0][
             "id"
         ]
         inputs = {"input": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]}}
         create = self._run("collection_creates_dynamic_list_of_pairs", history_id, inputs).json()
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(implicit_collections), 1)
-        self.assertEqual(implicit_collections[0]["collection_type"], "list:list:paired")
-        self.assertEqual(implicit_collections[0]["elements"][0]["object"]["element_count"], None)
+        assert len(implicit_collections) == 1
+        assert implicit_collections[0]["collection_type"] == "list:list:paired"
+        assert implicit_collections[0]["elements"][0]["object"]["element_count"] is None
         self.dataset_populator.wait_for_job(create["jobs"][0]["id"], assert_ok=True)
         hdca = self._get(f"histories/{history_id}/contents/dataset_collections/{implicit_collections[0]['id']}").json()
-        self.assertEqual(
-            hdca["elements"][0]["object"]["elements"][0]["object"]["elements"][0]["element_identifier"], "forward"
-        )
+        assert hdca["elements"][0]["object"]["elements"][0]["object"]["elements"][0]["element_identifier"] == "forward"
 
     def _bed_list(self, history_id):
         bed1_contents = open(self.get_filename("1.bed")).read()
         bed2_contents = open(self.get_filename("2.bed")).read()
         contents = [bed1_contents, bed2_contents]
         hdca = self.dataset_collection_populator.create_list_in_history(history_id, contents=contents, wait=True).json()
         return hdca["outputs"][0]["id"]
 
     @skip_without_tool("identifier_single")
-    @uses_test_history(require_new=False)
     def test_identifier_in_map(self, history_id):
         hdca_id = self._build_pair(history_id, ["123", "456"])
         inputs = {
             "input1": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
         }
         create_response = self._run("identifier_single", history_id, inputs)
         self._assert_status_code_is(create_response, 200)
         create = create_response.json()
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 2)
-        self.assertEqual(len(outputs), 2)
-        self.assertEqual(len(implicit_collections), 1)
+        assert len(jobs) == 2
+        assert len(outputs) == 2
+        assert len(implicit_collections) == 1
         output1 = outputs[0]
         output2 = outputs[1]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
         output2_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output2)
-        self.assertEqual(output1_content.strip(), "forward")
-        self.assertEqual(output2_content.strip(), "reverse")
+        assert output1_content.strip() == "forward"
+        assert output2_content.strip() == "reverse"
 
     @skip_without_tool("identifier_single")
-    @uses_test_history(require_new=False)
     def test_identifier_outside_map(self, history_id):
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="123", name="Plain HDA")
         inputs = {
             "input1": {"src": "hda", "id": new_dataset1["id"]},
         }
         create_response = self._run("identifier_single", history_id, inputs)
         self._assert_status_code_is(create_response, 200)
         create = create_response.json()
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 1)
-        self.assertEqual(len(outputs), 1)
-        self.assertEqual(len(implicit_collections), 0)
+        assert len(jobs) == 1
+        assert len(outputs) == 1
+        assert len(implicit_collections) == 0
         output1 = outputs[0]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "Plain HDA")
+        assert output1_content.strip() == "Plain HDA"
 
     @skip_without_tool("identifier_multiple")
-    @uses_test_history(require_new=False)
     def test_list_selectable_in_multidata_input(self, history_id):
         self.dataset_collection_populator.create_list_in_history(history_id, contents=["123", "456"], wait=True)
         build = self.dataset_populator.build_tool_state("identifier_multiple", history_id)
         assert len(build["inputs"][0]["options"]["hdca"]) == 1
 
     @skip_without_tool("identifier_multiple")
-    @uses_test_history(require_new=False)
     def test_identifier_in_multiple_reduce(self, history_id):
         hdca_id = self._build_pair(history_id, ["123", "456"])
         inputs = {
             "input1": {"src": "hdca", "id": hdca_id},
         }
         create_response = self._run("identifier_multiple", history_id, inputs)
         self._assert_status_code_is(create_response, 200)
         create = create_response.json()
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 1)
-        self.assertEqual(len(outputs), 1)
-        self.assertEqual(len(implicit_collections), 0)
+        assert len(jobs) == 1
+        assert len(outputs) == 1
+        assert len(implicit_collections) == 0
         output1 = outputs[0]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "forward\nreverse")
+        assert output1_content.strip() == "forward\nreverse"
 
     @skip_without_tool("identifier_in_conditional")
-    @uses_test_history(require_new=False)
     def test_identifier_map_over_multiple_input_in_conditional(self, history_id):
         hdca_id = self._build_pair(history_id, ["123", "456"])
         inputs = {
             "outer_cond|input1": {"src": "hdca", "id": hdca_id},
         }
         create_response = self._run("identifier_in_conditional", history_id, inputs)
         self._assert_status_code_is(create_response, 200)
         create = create_response.json()
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 1)
-        self.assertEqual(len(outputs), 1)
-        self.assertEqual(len(implicit_collections), 0)
+        assert len(jobs) == 1
+        assert len(outputs) == 1
+        assert len(implicit_collections) == 0
         output1 = outputs[0]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "forward\nreverse")
+        assert output1_content.strip() == "forward\nreverse"
 
     @skip_without_tool("identifier_in_conditional")
-    @uses_test_history(require_new=False)
     def test_identifier_map_over_multiple_input_in_conditional_new_payload_form(self, history_id):
         hdca_id = self._build_pair(history_id, ["123", "456"])
         inputs = {
             "outer_cond": {
                 "multi_input": True,
                 "input1": {"id": hdca_id, "src": "hdca"},
             },
         }
         create_response = self._run("identifier_in_conditional", history_id, inputs, input_format="21.01")
         self._assert_status_code_is(create_response, 200)
         create = create_response.json()
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 1)
-        self.assertEqual(len(outputs), 1)
-        self.assertEqual(len(implicit_collections), 0)
+        assert len(jobs) == 1
+        assert len(outputs) == 1
+        assert len(implicit_collections) == 0
         output1 = outputs[0]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "forward\nreverse")
+        assert output1_content.strip() == "forward\nreverse"
 
     @skip_without_tool("identifier_multiple_in_repeat")
-    @uses_test_history(require_new=False)
     def test_identifier_multiple_reduce_in_repeat_new_payload_form(self, history_id):
         hdca_id = self._build_pair(history_id, ["123", "456"])
         inputs = {
             "the_repeat": [{"the_data": {"input1": {"src": "hdca", "id": hdca_id}}}],
         }
         create_response = self._run("identifier_multiple_in_repeat", history_id, inputs, input_format="21.01")
         self._assert_status_code_is(create_response, 200)
         create = create_response.json()
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 1)
-        self.assertEqual(len(outputs), 1)
-        self.assertEqual(len(implicit_collections), 0)
+        assert len(jobs) == 1
+        assert len(outputs) == 1
+        assert len(implicit_collections) == 0
         output1 = outputs[0]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "forward\nreverse")
+        assert output1_content.strip() == "forward\nreverse"
 
     @skip_without_tool("identifier_in_conditional")
-    @uses_test_history(require_new=False)
     def test_identifier_map_over_input_in_conditional(self, history_id):
         # Run cat tool, so HDA names are different from element identifiers
         hdca_id = self._build_pair(history_id, ["123", "456"], run_cat=True)
         inputs = {
             "outer_cond|input1": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
             "outer_cond|multi_input": False,
         }
         create_response = self._run("identifier_in_conditional", history_id, inputs)
         self._assert_status_code_is(create_response, 200)
         create = create_response.json()
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 2)
-        self.assertEqual(len(outputs), 2)
-        self.assertEqual(len(implicit_collections), 1)
+        assert len(jobs) == 2
+        assert len(outputs) == 2
+        assert len(implicit_collections) == 1
         output1 = outputs[0]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "forward")
+        assert output1_content.strip() == "forward"
         output2 = outputs[1]
         output2_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output2)
-        self.assertEqual(output2_content.strip(), "reverse")
+        assert output2_content.strip() == "reverse"
 
     @skip_without_tool("identifier_multiple_in_conditional")
-    @uses_test_history(require_new=False)
     def test_identifier_multiple_reduce_in_conditional(self, history_id):
         hdca_id = self._build_pair(history_id, ["123", "456"])
         inputs = {
             "outer_cond|inner_cond|input1": {"src": "hdca", "id": hdca_id},
         }
         create_response = self._run("identifier_multiple_in_conditional", history_id, inputs)
         self._assert_status_code_is(create_response, 200)
         create = create_response.json()
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 1)
-        self.assertEqual(len(outputs), 1)
-        self.assertEqual(len(implicit_collections), 0)
+        assert len(jobs) == 1
+        assert len(outputs) == 1
+        assert len(implicit_collections) == 0
         output1 = outputs[0]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "forward\nreverse")
+        assert output1_content.strip() == "forward\nreverse"
 
     @skip_without_tool("identifier_multiple_in_repeat")
-    @uses_test_history(require_new=False)
     def test_identifier_multiple_reduce_in_repeat(self, history_id):
         hdca_id = self._build_pair(history_id, ["123", "456"])
         inputs = {
             "the_repeat_0|the_data|input1": {"src": "hdca", "id": hdca_id},
         }
         create_response = self._run("identifier_multiple_in_repeat", history_id, inputs)
         self._assert_status_code_is(create_response, 200)
         create = create_response.json()
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 1)
-        self.assertEqual(len(outputs), 1)
-        self.assertEqual(len(implicit_collections), 0)
+        assert len(jobs) == 1
+        assert len(outputs) == 1
+        assert len(implicit_collections) == 0
         output1 = outputs[0]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "forward\nreverse")
+        assert output1_content.strip() == "forward\nreverse"
 
     @skip_without_tool("identifier_single_in_repeat")
-    @uses_test_history(require_new=False)
     def test_identifier_single_in_repeat(self, history_id):
         hdca_id = self._build_pair(history_id, ["123", "456"])
         inputs = {"the_repeat_0|the_data|input1": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]}}
         create_response = self._run("identifier_single_in_repeat", history_id, inputs)
         self._assert_status_code_is(create_response, 200)
         create = create_response.json()
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 2)
-        self.assertEqual(len(implicit_collections), 1)
+        assert len(jobs) == 2
+        assert len(implicit_collections) == 1
         output_collection = implicit_collections[0]
         elements = output_collection["elements"]
         assert len(elements) == 2
         forward_output = elements[0]["object"]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=forward_output)
         assert output1_content.strip() == "forward", output1_content
 
     @skip_without_tool("identifier_multiple_in_conditional")
-    @uses_test_history(require_new=False)
     def test_identifier_multiple_in_conditional(self, history_id):
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="123", name="Normal HDA1")
         inputs = {
             "outer_cond|inner_cond|input1": {"src": "hda", "id": new_dataset1["id"]},
         }
         create_response = self._run("identifier_multiple_in_conditional", history_id, inputs)
         self._assert_status_code_is(create_response, 200)
         create = create_response.json()
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 1)
-        self.assertEqual(len(outputs), 1)
-        self.assertEqual(len(implicit_collections), 0)
+        assert len(jobs) == 1
+        assert len(outputs) == 1
+        assert len(implicit_collections) == 0
         output1 = outputs[0]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "Normal HDA1")
+        assert output1_content.strip() == "Normal HDA1"
 
     @skip_without_tool("identifier_multiple")
-    @uses_test_history(require_new=False)
     def test_identifier_with_multiple_normal_datasets(self, history_id):
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="123", name="Normal HDA1")
         new_dataset2 = self.dataset_populator.new_dataset(history_id, content="456", name="Normal HDA2")
         inputs = {"input1": [{"src": "hda", "id": new_dataset1["id"]}, {"src": "hda", "id": new_dataset2["id"]}]}
         create_response = self._run("identifier_multiple", history_id, inputs)
         self._assert_status_code_is(create_response, 200)
         create = create_response.json()
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 1)
-        self.assertEqual(len(outputs), 1)
-        self.assertEqual(len(implicit_collections), 0)
+        assert len(jobs) == 1
+        assert len(outputs) == 1
+        assert len(implicit_collections) == 0
         output1 = outputs[0]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "Normal HDA1\nNormal HDA2")
+        assert output1_content.strip() == "Normal HDA1\nNormal HDA2"
 
     @skip_without_tool("identifier_collection")
-    @uses_test_history(require_new=False)
     def test_identifier_with_data_collection(self, history_id):
         element_identifiers = self.dataset_collection_populator.list_identifiers(history_id)
 
         payload = dict(
             instance_type="history",
             history_id=history_id,
             element_identifiers=element_identifiers,
@@ -2042,22 +2035,21 @@
 
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         create_response = self._run("identifier_collection", history_id, inputs)
         self._assert_status_code_is(create_response, 200)
         create = create_response.json()
         outputs = create["outputs"]
         jobs = create["jobs"]
-        self.assertEqual(len(jobs), 1)
-        self.assertEqual(len(outputs), 1)
+        assert len(jobs) == 1
+        assert len(outputs) == 1
         output1 = outputs[0]
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
-        self.assertEqual(output1_content.strip(), "\n".join(d["name"] for d in element_identifiers))
+        assert output1_content.strip() == "\n".join(d["name"] for d in element_identifiers)
 
     @skip_without_tool("identifier_in_actions")
-    @uses_test_history(require_new=False)
     def test_identifier_in_actions(self, history_id):
         element_identifiers = self.dataset_collection_populator.list_identifiers(history_id, contents=["1\t2"])
 
         payload = dict(
             instance_type="history",
             history_id=history_id,
             element_identifiers=element_identifiers,
@@ -2078,129 +2070,124 @@
         outputs = create["outputs"]
         output1 = outputs[0]
 
         output_details = self.dataset_populator.get_history_dataset_details(history_id, dataset=output1)
         assert output_details["metadata_column_names"][1] == "data1", output_details
 
     @skip_without_tool("cat1")
-    @uses_test_history(require_new=False)
     def test_map_over_nested_collections(self, history_id):
         hdca_id = self.__build_nested_list(history_id)
         inputs = {
             "input1": {"batch": True, "values": [dict(src="hdca", id=hdca_id)]},
         }
         self._check_simple_cat1_over_nested_collections(history_id, inputs)
 
     @skip_without_tool("collection_paired_structured_like")
-    @uses_test_history(require_new=False)
     def test_paired_input_map_over_nested_collections(self, history_id):
         hdca_id = self.__build_nested_list(history_id)
         inputs = {
             "input1": {"batch": True, "values": [dict(map_over_type="paired", src="hdca", id=hdca_id)]},
         }
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         create = self._run("collection_paired_structured_like", history_id, inputs, assert_ok=True)
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 2)
-        self.assertEqual(len(implicit_collections), 1)
+        assert len(jobs) == 2
+        assert len(implicit_collections) == 1
         implicit_collection = implicit_collections[0]
         assert implicit_collection["collection_type"] == "list:paired", implicit_collection["collection_type"]
         outer_elements = implicit_collection["elements"]
         assert len(outer_elements) == 2
 
     @skip_without_tool("collection_paired_conditional_structured_like")
-    @uses_test_history(require_new=False)
     def test_paired_input_conditional_map_over_nested_collections(self, history_id):
         hdca_id = self.__build_nested_list(history_id)
         inputs = {
             "cond|cond_param": "paired",
             "cond|input1": {"batch": True, "values": [dict(map_over_type="paired", src="hdca", id=hdca_id)]},
         }
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         create = self._run("collection_paired_conditional_structured_like", history_id, inputs, assert_ok=True)
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 2)
-        self.assertEqual(len(implicit_collections), 1)
+        assert len(jobs) == 2
+        assert len(implicit_collections) == 1
         implicit_collection = implicit_collections[0]
         assert implicit_collection["collection_type"] == "list:paired", implicit_collection["collection_type"]
         outer_elements = implicit_collection["elements"]
         assert len(outer_elements) == 2
 
     def _check_simple_cat1_over_nested_collections(self, history_id, inputs):
         create = self._run_cat1(history_id, inputs=inputs, assert_ok=True)
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 4)
-        self.assertEqual(len(outputs), 4)
-        self.assertEqual(len(implicit_collections), 1)
+        assert len(jobs) == 4
+        assert len(outputs) == 4
+        assert len(implicit_collections) == 1
         implicit_collection = implicit_collections[0]
         self._assert_has_keys(implicit_collection, "collection_type", "elements")
         assert implicit_collection["collection_type"] == "list:paired"
         assert len(implicit_collection["elements"]) == 2
         first_element, second_element = implicit_collection["elements"]
         assert first_element["element_identifier"] == "test0", first_element
         assert second_element["element_identifier"] == "test1", second_element
 
         first_object = first_element["object"]
         assert first_object["collection_type"] == "paired"
         assert len(first_object["elements"]) == 2
         first_object_forward_element = first_object["elements"][0]
-        self.assertEqual(outputs[0]["id"], first_object_forward_element["object"]["id"])
+        assert outputs[0]["id"] == first_object_forward_element["object"]["id"]
 
     @skip_without_tool("cat1")
-    @uses_test_history(require_new=False)
     def test_map_over_two_collections(self, history_id):
         hdca1_id = self._build_pair(history_id, ["123\n", "456\n"])
         hdca2_id = self._build_pair(history_id, ["789\n", "0ab\n"])
         inputs = {
             "input1": {"batch": True, "values": [{"src": "hdca", "id": hdca1_id}]},
             "queries_0|input2": {"batch": True, "values": [{"src": "hdca", "id": hdca2_id}]},
         }
         self._check_map_cat1_over_two_collections(history_id, inputs)
 
     def _check_map_cat1_over_two_collections(self, history_id, inputs):
         response = self._run_cat1(history_id, inputs)
         self._assert_status_code_is(response, 200)
         response_object = response.json()
         outputs = response_object["outputs"]
-        self.assertEqual(len(outputs), 2)
+        assert len(outputs) == 2
         output1 = outputs[0]
         output2 = outputs[1]
         self.dataset_populator.wait_for_history(history_id)
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
         output2_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output2)
-        self.assertEqual(output1_content.strip(), "123\n789")
-        self.assertEqual(output2_content.strip(), "456\n0ab")
+        assert output1_content.strip() == "123\n789"
+        assert output2_content.strip() == "456\n0ab"
 
-        self.assertEqual(len(response_object["jobs"]), 2)
-        self.assertEqual(len(response_object["implicit_collections"]), 1)
+        assert len(response_object["jobs"]) == 2
+        assert len(response_object["implicit_collections"]) == 1
 
     @skip_without_tool("cat1")
-    @uses_test_history(require_new=False)
     def test_map_over_two_collections_unlinked(self, history_id):
         hdca1_id = self._build_pair(history_id, ["123\n", "456\n"])
         hdca2_id = self._build_pair(history_id, ["789\n", "0ab\n"])
         inputs = {
             "input1": {"batch": True, "linked": False, "values": [{"src": "hdca", "id": hdca1_id}]},
             "queries_0|input2": {"batch": True, "linked": False, "values": [{"src": "hdca", "id": hdca2_id}]},
         }
         response = self._run_cat1(history_id, inputs)
         self._assert_status_code_is(response, 200)
         response_object = response.json()
         outputs = response_object["outputs"]
-        self.assertEqual(len(outputs), 4)
+        assert len(outputs) == 4
 
-        self.assertEqual(len(response_object["jobs"]), 4)
+        assert len(response_object["jobs"]) == 4
         implicit_collections = response_object["implicit_collections"]
-        self.assertEqual(len(implicit_collections), 1)
+        assert len(implicit_collections) == 1
         implicit_collection = implicit_collections[0]
-        self.assertEqual(implicit_collection["collection_type"], "paired:paired")
+        assert implicit_collection["collection_type"] == "paired:paired"
 
         outer_elements = implicit_collection["elements"]
         assert len(outer_elements) == 2
         element0, element1 = outer_elements
         assert element0["element_identifier"] == "forward"
         assert element1["element_identifier"] == "reverse"
 
@@ -2220,21 +2207,20 @@
 
         expected_contents_list = [
             (element00, "123\n789\n"),
             (element01, "123\n0ab\n"),
             (element10, "456\n789\n"),
             (element11, "456\n0ab\n"),
         ]
-        for (element, expected_contents) in expected_contents_list:
+        for element, expected_contents in expected_contents_list:
             dataset_id = element["object"]["id"]
             contents = self.dataset_populator.get_history_dataset_content(history_id, dataset_id=dataset_id)
-            self.assertEqual(expected_contents, contents)
+            assert expected_contents == contents
 
     @skip_without_tool("cat1")
-    @uses_test_history(require_new=False)
     def test_map_over_collected_and_individual_datasets(self, history_id):
         hdca1_id = self._build_pair(history_id, ["123\n", "456\n"])
         new_dataset1 = self.dataset_populator.new_dataset(history_id, content="789")
         new_dataset2 = self.dataset_populator.new_dataset(history_id, content="0ab")
 
         inputs = {
             "input1": {"batch": True, "values": [{"src": "hdca", "id": hdca1_id}]},
@@ -2243,18 +2229,18 @@
                 "values": [dataset_to_param(new_dataset1), dataset_to_param(new_dataset2)],
             },
         }
         response = self._run_cat1(history_id, inputs)
         self._assert_status_code_is(response, 200)
         response_object = response.json()
         outputs = response_object["outputs"]
-        self.assertEqual(len(outputs), 2)
+        assert len(outputs) == 2
 
-        self.assertEqual(len(response_object["jobs"]), 2)
-        self.assertEqual(len(response_object["implicit_collections"]), 1)
+        assert len(response_object["jobs"]) == 2
+        assert len(response_object["implicit_collections"]) == 1
 
     @skip_without_tool("identifier_source")
     def test_default_identifier_source_map_over(self):
         with self.dataset_populator.test_history() as history_id:
             input_a_hdca_id = self.dataset_collection_populator.create_list_in_history(
                 history_id, contents=[("A", "A content")], wait=True
             ).json()["outputs"][0]["id"]
@@ -2283,16 +2269,16 @@
             inputs = {
                 "input1": {"batch": True, "values": [dict(src="hdca", id=hdca_id)]},
             }
             self.dataset_populator.wait_for_history(history_id, assert_ok=True)
             create = self._run("collection_creates_pair", history_id, inputs, assert_ok=True)
             jobs = create["jobs"]
             implicit_collections = create["implicit_collections"]
-            self.assertEqual(len(jobs), 2)
-            self.assertEqual(len(implicit_collections), 1)
+            assert len(jobs) == 2
+            assert len(implicit_collections) == 1
             implicit_collection = implicit_collections[0]
             assert implicit_collection["collection_type"] == "list:paired", implicit_collection
             outer_elements = implicit_collection["elements"]
             assert len(outer_elements) == 2
             element0, element1 = outer_elements
             assert element0["element_identifier"] == "data0"
             assert element1["element_identifier"] == "data1"
@@ -2315,15 +2301,15 @@
                 "a\nc\n",
                 "b\nd\n",
                 "e\ng\n",
                 "f\nh\n",
             ]
             for i in range(4):
                 contents = self.dataset_populator.get_history_dataset_content(history_id, dataset_id=pair_ids[i])
-                self.assertEqual(expected_contents[i], contents)
+                assert expected_contents[i] == contents
 
     @skip_without_tool("cat1")
     def test_cannot_map_over_incompatible_collections(self):
         with self.dataset_populator.test_history() as history_id:
             hdca1_id = self._build_pair(history_id, ["123\n", "456\n"])
             hdca2_id = self.dataset_collection_populator.create_list_in_history(history_id).json()["outputs"][0]["id"]
             inputs = {
@@ -2358,17 +2344,17 @@
             discarded_collection, filtered_collection = implicit_collections
             self.dataset_populator.wait_for_history(history_id, assert_ok=True)
             history_contents = self.dataset_populator._get_contents_request(history_id).json()
             # We should have a final collection count of 3 (2 nested collections, plus the input collection)
             new_collections = (
                 len([c for c in history_contents if c["history_content_type"] == "dataset_collection"]) - 1
             )
-            assert new_collections == 2, (
-                "Expected to generate 4 new, filtered collections, but got %d collections" % new_collections
-            )
+            assert (
+                new_collections == 2
+            ), f"Expected to generate 4 new, filtered collections, but got {new_collections} collections"
             assert (
                 filtered_collection["collection_type"] == discarded_collection["collection_type"] == "list:list"
             ), filtered_collection
             collection_details = self.dataset_populator.get_history_collection_details(
                 history_id, hid=filtered_collection["hid"]
             )
             assert collection_details["element_count"] == 2
@@ -2432,16 +2418,16 @@
                     "batch": True,
                     "values": [{"src": "hdca", "map_over_type": "list", "id": hdca2_id}],
                 },
             }
             create = self._run("multi_data_param", history_id, inputs, assert_ok=True)
             jobs = create["jobs"]
             implicit_collections = create["implicit_collections"]
-            self.assertEqual(len(jobs), 1)
-            self.assertEqual(len(implicit_collections), 2)
+            assert len(jobs) == 1
+            assert len(implicit_collections) == 2
             output_hdca = self.dataset_populator.get_history_collection_details(
                 history_id, hid=implicit_collections[0]["hid"]
             )
             assert output_hdca["collection_type"] == "list"
 
     @skip_without_tool("column_multi_param")
     def test_implicit_conversion_and_reduce(self):
@@ -2478,46 +2464,46 @@
             hdca_id = response.json()["outputs"][0]["id"]
             inputs = {
                 "input1": {"src": "hdca", "id": hdca_id},
                 "col": param,
             }
             create = self._run("column_multi_param", history_id, inputs, assert_ok=True)
             jobs = create["jobs"]
-            self.assertEqual(len(jobs), 1)
+            assert len(jobs) == 1
             content = self.dataset_populator.get_history_dataset_content(history_id, hid=3)
             assert content.strip() == "hg17", content
 
     @skip_without_tool("multi_data_repeat")
     def test_reduce_collections_in_repeat(self):
         with self.dataset_populator.test_history() as history_id:
             hdca1_id = self._build_pair(history_id, ["123\n", "456\n"])
             inputs = {
                 "outer_repeat_0|f1": {"src": "hdca", "id": hdca1_id},
             }
             create = self._run("multi_data_repeat", history_id, inputs, assert_ok=True)
             outputs = create["outputs"]
             jobs = create["jobs"]
-            self.assertEqual(len(jobs), 1)
-            self.assertEqual(len(outputs), 1)
+            assert len(jobs) == 1
+            assert len(outputs) == 1
             output1 = outputs[0]
             output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
             assert output1_content.strip() == "123\n456", output1_content
 
     @skip_without_tool("multi_data_repeat")
     def test_reduce_collections_in_repeat_legacy(self):
         with self.dataset_populator.test_history() as history_id:
             hdca1_id = self._build_pair(history_id, ["123\n", "456\n"])
             inputs = {
                 "outer_repeat_0|f1": f"__collection_reduce__|{hdca1_id}",
             }
             create = self._run("multi_data_repeat", history_id, inputs, assert_ok=True)
             outputs = create["outputs"]
             jobs = create["jobs"]
-            self.assertEqual(len(jobs), 1)
-            self.assertEqual(len(outputs), 1)
+            assert len(jobs) == 1
+            assert len(outputs) == 1
             output1 = outputs[0]
             output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
             assert output1_content.strip() == "123\n456", output1_content
 
     @skip_without_tool("multi_data_param")
     def test_reduce_multiple_lists_on_multi_data(self):
         with self.dataset_populator.test_history() as history_id:
@@ -2528,28 +2514,28 @@
             inputs = {
                 "f1": [{"src": "hdca", "id": hdca1_id}, {"src": "hdca", "id": hdca2_id}],
                 "f2": [{"src": "hdca", "id": hdca1_id}],
             }
             create = self._run("multi_data_param", history_id, inputs, assert_ok=True)
             outputs = create["outputs"]
             jobs = create["jobs"]
-            self.assertEqual(len(jobs), 1)
-            self.assertEqual(len(outputs), 2)
+            assert len(jobs) == 1
+            assert len(outputs) == 2
             output1, output2 = outputs
             output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
             output2_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output2)
-            self.assertEqual(output1_content.strip(), "123\n456\nTestData123\nTestData123\nTestData123")
-            self.assertEqual(output2_content.strip(), "123\n456")
+            assert output1_content.strip() == "123\n456\nTestData123\nTestData123\nTestData123"
+            assert output2_content.strip() == "123\n456"
 
     def _check_simple_reduce_job(self, history_id, inputs):
         create = self._run("multi_data_param", history_id, inputs, assert_ok=True)
         outputs = create["outputs"]
         jobs = create["jobs"]
-        self.assertEqual(len(jobs), 1)
-        self.assertEqual(len(outputs), 2)
+        assert len(jobs) == 1
+        assert len(outputs) == 2
         output1, output2 = outputs
         output1_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output1)
         output2_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output2)
         assert output1_content.strip() == "123\n456", output1_content
         assert len(output2_content.strip().split("\n")) == 3, output2_content
 
     @skip_without_tool("collection_paired_test")
@@ -2640,83 +2626,80 @@
             else:
                 tools.append(tool_or_section)
 
         tool_ids = [_["id"] for _ in tools]
         return tool_ids
 
     @skip_without_tool("collection_cat_group_tag_multiple")
-    @uses_test_history(require_new=False)
     def test_group_tag_selection(self, history_id):
         input_hdca_id = self.__build_group_list(history_id)
         inputs = {
             "input1": {"src": "hdca", "id": input_hdca_id},
             "group": "condition:treated",
         }
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         response = self._run("collection_cat_group_tag", history_id, inputs, assert_ok=True)
         outputs = response["outputs"]
-        self.assertEqual(len(outputs), 1)
+        assert len(outputs) == 1
         output = outputs[0]
         output_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output)
-        self.assertEqual(output_content.strip(), "123\n456")
+        assert output_content.strip() == "123\n456"
 
     @skip_without_tool("collection_cat_group_tag_multiple")
-    @uses_test_history(require_new=False)
     def test_group_tag_selection_multiple(self, history_id):
         input_hdca_id = self.__build_group_list(history_id)
         inputs = {
             "input1": {"src": "hdca", "id": input_hdca_id},
             "groups": "condition:treated,type:single",
         }
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         response = self._run("collection_cat_group_tag_multiple", history_id, inputs, assert_ok=True)
         outputs = response["outputs"]
-        self.assertEqual(len(outputs), 1)
+        assert len(outputs) == 1
         output = outputs[0]
         output_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output)
-        self.assertEqual(output_content.strip(), "123\n456\n456\n0ab")
+        assert output_content.strip() == "123\n456\n456\n0ab"
 
     @skip_without_tool("expression_forty_two")
     def test_galaxy_expression_tool_simplest(self):
         history_id = self.dataset_populator.new_history()
         run_response = self._run("expression_forty_two", history_id)
         self._assert_status_code_is(run_response, 200)
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         output_content = self.dataset_populator.get_history_dataset_content(history_id)
-        self.assertEqual(output_content, "42")
+        assert output_content == "42"
 
     @skip_without_tool("expression_parse_int")
     def test_galaxy_expression_tool_simple(self):
         history_id = self.dataset_populator.new_history()
         inputs = {
             "input1": "7",
         }
         run_response = self._run("expression_parse_int", history_id, inputs)
         self._assert_status_code_is(run_response, 200)
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         output_content = self.dataset_populator.get_history_dataset_content(history_id)
-        self.assertEqual(output_content, "7")
+        assert output_content == "7"
 
     @skip_without_tool("expression_log_line_count")
     def test_galaxy_expression_metadata(self):
         history_id = self.dataset_populator.new_history()
         new_dataset1 = self.dataset_populator.new_dataset(
             history_id, content="1\n2\n3\n4\n5\n6\n7\n8\n9\n10\n11\n12\n13\n14"
         )
         inputs = {
             "input1": dataset_to_param(new_dataset1),
         }
         run_response = self._run("expression_log_line_count", history_id, inputs)
         self._assert_status_code_is(run_response, 200)
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         output_content = self.dataset_populator.get_history_dataset_content(history_id)
-        self.assertEqual(output_content, "3")
+        assert output_content == "3"
 
     @skip_without_tool("cat1")
-    @uses_test_history(require_new=False)
     def test_run_deferred_dataset(self, history_id):
         details = self.dataset_populator.create_deferred_hda(
             history_id, "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/1.bed", ext="bed"
         )
         inputs = {
             "input1": dataset_to_param(details),
         }
@@ -2726,15 +2709,14 @@
             history_id, dataset=output, wait=True, assert_ok=True
         )
         assert details["state"] == "ok"
         output_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output)
         assert output_content.startswith("chr1	147962192	147962580	CCDS989.1_cds_0_0_chr1_147962193_r	0	-")
 
     @skip_without_tool("metadata_bam")
-    @uses_test_history(require_new=False)
     def test_run_deferred_dataset_with_metadata_options_filter(self, history_id):
         details = self.dataset_populator.create_deferred_hda(
             history_id, "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/1.bam", ext="bam"
         )
         inputs = {"input_bam": dataset_to_param(details), "ref_names": "chrM"}
         run_response = self.dataset_populator.run_tool(tool_id="metadata_bam", inputs=inputs, history_id=history_id)
         output = run_response["outputs"][0]
@@ -2742,28 +2724,26 @@
             history_id, dataset=output, wait=True, assert_ok=True
         )
         assert output_details["state"] == "ok"
         output_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output)
         assert output_content.startswith("chrM")
 
     @skip_without_tool("pileup")
-    @uses_test_history(require_new=False)
     def test_metadata_validator_on_deferred_input(self, history_id):
         deferred_bam_details = self.dataset_populator.create_deferred_hda(
             history_id, "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/1.bam", ext="bam"
         )
         fasta1_contents = open(self.get_filename("1.fasta")).read()
         fasta = self.dataset_populator.new_dataset(history_id, content=fasta1_contents)
         inputs = {"input1": dataset_to_param(deferred_bam_details), "reference": dataset_to_param(fasta)}
         run_response = self.dataset_populator.run_tool(tool_id="pileup", inputs=inputs, history_id=history_id)
         self.dataset_populator.wait_for_job(run_response["jobs"][0]["id"], assert_ok=True)
 
     @pytest.mark.xfail
     @skip_without_tool("pileup")
-    @uses_test_history(require_new=False)
     def test_metadata_validator_can_fail_on_deferred_input(self, history_id):
         # This test fails because we just skip the validator
         # Fixing this is a TODO
         deferred_bam_details = self.dataset_populator.create_deferred_hda(
             history_id,
             "https://github.com/galaxyproject/galaxy/blob/dev/test-data/3unsorted.bam?raw=true",
             ext="unsorted.bam",
@@ -2774,15 +2754,14 @@
         run_response = self.dataset_populator.run_tool(tool_id="pileup", inputs=inputs, history_id=history_id)
         self.dataset_populator.wait_for_job(run_response["jobs"][0]["id"], assert_ok=False)
         job_id = run_response["jobs"][0]["id"]
         job_details = self.dataset_populator.get_job_details(job_id=job_id).json()
         assert job_details["state"] == "failed"
 
     @skip_without_tool("cat1")
-    @uses_test_history(require_new=False)
     def test_run_deferred_mapping(self, history_id: str):
         elements = [
             {
                 "src": "url",
                 "url": "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/4.bed",
                 "info": "my cool bed",
                 "deferred": True,
@@ -2815,15 +2794,14 @@
         object_0 = elements[0]["object"]
         assert isinstance(object_0, dict)
         assert object_0["state"] == "ok"
         output_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=object_0)
         assert output_content.startswith("chr22	30128507	31828507	uc003bnx.1_cds_2_0_chr22_29227_f	0	+")
 
     @skip_without_tool("cat_list")
-    @uses_test_history(require_new=False)
     def test_run_deferred_list_multi_data_reduction(self, history_id: str):
         elements = [
             {
                 "src": "url",
                 "url": "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/4.bed",
                 "info": "my cool bed",
                 "deferred": True,
@@ -2850,15 +2828,14 @@
         }
         run_response = self._run("cat_list", history_id, inputs, assert_ok=True)
         output_dataset = run_response["outputs"][0]
         output_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output_dataset)
         assert output_content.startswith("chr22	30128507	31828507	uc003bnx.1_cds_2_0_chr22_29227_f	0	+")
 
     @skip_without_tool("cat_list")
-    @uses_test_history(require_new=False)
     def test_run_deferred_nested_list_input(self, history_id: str):
         elements = [
             {
                 "name": "outer",
                 "elements": [
                     {
                         "src": "url",
@@ -2909,15 +2886,14 @@
         }
         run_response = self._run("collection_nested_test", history_id, inputs, assert_ok=True, wait_for_job=True)
         output_dataset = run_response["outputs"][1]
         output_content = self.dataset_populator.get_history_dataset_content(history_id, dataset=output_dataset)
         assert output_content.startswith("chr22	30128507	31828507	uc003bnx.1_cds_2_0_chr22_29227_f	0	+")
 
     @skip_without_tool("collection_paired_structured_like")
-    @uses_test_history(require_new=False)
     def test_deferred_map_over_nested_collections(self, history_id):
         elements = [
             {
                 "name": "outer1",
                 "elements": [
                     {
                         "src": "url",
@@ -2977,17 +2953,17 @@
         inputs = {
             "input1": {"batch": True, "values": [dict(map_over_type="paired", src="hdca", id=hdca_id)]},
         }
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         create = self._run("collection_paired_structured_like", history_id, inputs, assert_ok=True)
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
-        self.assertEqual(len(jobs), 2)
+        assert len(jobs) == 2
         self.dataset_populator.wait_for_jobs(jobs, assert_ok=True)
-        self.assertEqual(len(implicit_collections), 1)
+        assert len(implicit_collections) == 1
         implicit_collection = implicit_collections[0]
         assert implicit_collection["collection_type"] == "list:paired", implicit_collection["collection_type"]
         outer_elements = implicit_collection["elements"]
         assert len(outer_elements) == 2
         element0 = outer_elements[0]
         pair1 = element0["object"]
         hda = pair1["elements"][0]["object"]
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_tools_upload.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_tools_upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,36 @@
 import os
 import urllib.parse
 
 import pytest
 from tusclient import client
 
 from galaxy.tool_util.verify.test_data import TestDataResolver
+from galaxy.util.unittest_utils import (
+    skip_if_github_down,
+    skip_if_site_down,
+)
 from galaxy_test.base.constants import (
     ONE_TO_SIX_ON_WINDOWS,
     ONE_TO_SIX_WITH_SPACES,
     ONE_TO_SIX_WITH_SPACES_ON_WINDOWS,
     ONE_TO_SIX_WITH_TABS,
     ONE_TO_SIX_WITH_TABS_NO_TRAILING_NEWLINE,
 )
 from galaxy_test.base.populators import (
     DatasetPopulator,
-    skip_if_github_down,
-    skip_if_site_down,
     skip_without_datatype,
     stage_inputs,
-    uses_test_history,
 )
 from ._framework import ApiTestCase
 
 
-class ToolsUploadTestCase(ApiTestCase):
+class TestToolsUpload(ApiTestCase):
+    dataset_populator: DatasetPopulator
+
     def setUp(self):
         super().setUp()
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
 
     def test_upload1_paste(self):
         with self.dataset_populator.test_history() as history_id:
             payload = self.dataset_populator.upload_payload(history_id, "Hello World")
@@ -47,79 +50,79 @@
     # upload1 rewrites content with posix lines by default but this can be disabled by setting
     # to_posix_lines=None in the request. Newer fetch API does not do this by default prefering
     # to keep content unaltered if possible but it can be enabled with a simple JSON boolean switch
     # of the same name (to_posix_lines).
     def test_upload_posix_newline_fixes_by_default(self):
         windows_content = ONE_TO_SIX_ON_WINDOWS
         result_content = self._upload_and_get_content(windows_content)
-        self.assertEqual(result_content, ONE_TO_SIX_WITH_TABS)
+        assert result_content == ONE_TO_SIX_WITH_TABS
 
     def test_fetch_posix_unaltered(self):
         windows_content = ONE_TO_SIX_ON_WINDOWS
         result_content = self._upload_and_get_content(windows_content, api="fetch")
-        self.assertEqual(result_content, ONE_TO_SIX_ON_WINDOWS)
+        assert result_content == ONE_TO_SIX_ON_WINDOWS
 
     def test_upload_disable_posix_fix(self):
         windows_content = ONE_TO_SIX_ON_WINDOWS
         result_content = self._upload_and_get_content(windows_content, to_posix_lines=None)
-        self.assertEqual(result_content, windows_content)
+        assert result_content == windows_content
 
     def test_fetch_post_lines_option(self):
         windows_content = ONE_TO_SIX_ON_WINDOWS
         result_content = self._upload_and_get_content(windows_content, api="fetch", to_posix_lines=True)
-        self.assertEqual(result_content, ONE_TO_SIX_WITH_TABS)
+        assert result_content == ONE_TO_SIX_WITH_TABS
 
     # Test how trailing new lines are added
     # - upload1 adds by default because to_posix_lines is on by default
     # - fetch doesn't add by default because to_posix_lines is off by default
     # - fetch does add trailing newline if to_posix_lines is enabled
     def test_post_lines_trailing(self):
         input_content = ONE_TO_SIX_WITH_TABS_NO_TRAILING_NEWLINE
         result_content = self._upload_and_get_content(input_content)
-        self.assertEqual(result_content, ONE_TO_SIX_WITH_TABS)
+        assert result_content == ONE_TO_SIX_WITH_TABS
 
     def test_post_lines_trailing_off(self):
         input_content = ONE_TO_SIX_WITH_TABS_NO_TRAILING_NEWLINE
         result_content = self._upload_and_get_content(input_content, to_posix_lines=False)
-        self.assertEqual(result_content, ONE_TO_SIX_WITH_TABS_NO_TRAILING_NEWLINE)
+        assert result_content == ONE_TO_SIX_WITH_TABS_NO_TRAILING_NEWLINE
 
     def test_fetch_post_lines_trailing_off_by_default(self):
         input_content = ONE_TO_SIX_WITH_TABS_NO_TRAILING_NEWLINE
         result_content = self._upload_and_get_content(input_content, api="fetch")
-        self.assertEqual(result_content, ONE_TO_SIX_WITH_TABS_NO_TRAILING_NEWLINE)
+        assert result_content == ONE_TO_SIX_WITH_TABS_NO_TRAILING_NEWLINE
 
     def test_fetch_post_lines_trailing_if_to_posix(self):
         input_content = ONE_TO_SIX_WITH_TABS_NO_TRAILING_NEWLINE
         result_content = self._upload_and_get_content(input_content, api="fetch", to_posix_lines=True)
-        self.assertEqual(result_content, ONE_TO_SIX_WITH_TABS)
+        assert result_content == ONE_TO_SIX_WITH_TABS
 
     def test_upload_tab_to_space_off_by_default(self):
         table = ONE_TO_SIX_WITH_SPACES
         result_content = self._upload_and_get_content(table)
-        self.assertEqual(result_content, table)
+        assert result_content == table
 
     def test_fetch_tab_to_space_off_by_default(self):
         table = ONE_TO_SIX_WITH_SPACES
         result_content = self._upload_and_get_content(table, api="fetch")
-        self.assertEqual(result_content, table)
+        assert result_content == table
 
     def test_upload_tab_to_space(self):
         table = ONE_TO_SIX_WITH_SPACES
         result_content = self._upload_and_get_content(table, space_to_tab="Yes")
-        self.assertEqual(result_content, ONE_TO_SIX_WITH_TABS)
+        assert result_content == ONE_TO_SIX_WITH_TABS
 
     def test_fetch_tab_to_space(self):
         table = ONE_TO_SIX_WITH_SPACES
         result_content = self._upload_and_get_content(table, api="fetch", space_to_tab=True)
-        self.assertEqual(result_content, ONE_TO_SIX_WITH_TABS)
+        assert result_content == ONE_TO_SIX_WITH_TABS
 
     def test_fetch_tab_to_space_doesnt_swap_newlines(self):
         table = ONE_TO_SIX_WITH_SPACES_ON_WINDOWS
         result_content = self._upload_and_get_content(table, api="fetch", space_to_tab=True)
-        self.assertEqual(result_content, ONE_TO_SIX_ON_WINDOWS)
+        assert result_content == ONE_TO_SIX_ON_WINDOWS
 
     def test_fetch_compressed_with_explicit_type(self):
         fastqgz_path = TestDataResolver().get_filename("1.fastqsanger.gz")
         with open(fastqgz_path, "rb") as fh:
             details = self._upload_and_get_details(fh, api="fetch", ext="fastqsanger.gz")
         assert details["state"] == "ok"
         assert details["file_ext"] == "fastqsanger.gz"
@@ -127,15 +130,15 @@
     def test_fetch_compressed_default(self):
         fastqgz_path = TestDataResolver().get_filename("1.fastqsanger.gz")
         with open(fastqgz_path, "rb") as fh:
             details = self._upload_and_get_details(fh, api="fetch", assert_ok=False)
         assert details["state"] == "ok"
         assert details["file_ext"] == "fastqsanger.gz", details
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_fetch_compressed_auto_decompress_target(self, history_id):
         # TODO: this should definitely be fixed to allow auto decompression via that API.
         fastqgz_path = TestDataResolver().get_filename("1.fastqsanger.gz")
         with open(fastqgz_path, "rb") as fh:
             details = self._upload_and_get_details(
                 fh, api="fetch", history_id=history_id, assert_ok=False, auto_decompress=True
             )
@@ -169,15 +172,15 @@
     def test_upload_auto_decompress_off(self):
         # UNSTABLE_FLAG: This might default to a bed.gz datatype in the future.
         bedgz_path = TestDataResolver().get_filename("4.bed.gz")
         with open(bedgz_path, "rb") as fh:
             details = self._upload_and_get_details(fh, file_type="auto", assert_ok=False, auto_decompress=False)
         assert details["file_ext"] == "binary", details
 
-    @uses_test_history(require_new=True)
+    @pytest.mark.require_new_history
     def test_fetch_compressed_with_auto(self, history_id):
         # UNSTABLE_FLAG: This might default to a bed.gz datatype in the future.
         # TODO: this should definitely be fixed to allow auto decompression via that API.
         bedgz_path = TestDataResolver().get_filename("4.bed.gz")
         with open(bedgz_path, "rb") as fh:
             details = self._upload_and_get_details(
                 fh, api="fetch", history_id=history_id, auto_decompress=True, assert_ok=False
@@ -187,105 +190,134 @@
 
     @skip_without_datatype("rdata")
     def test_rdata_not_decompressed(self):
         # Prevent regression of https://github.com/galaxyproject/galaxy/issues/753
         rdata_path = TestDataResolver().get_filename("1.RData")
         with open(rdata_path, "rb") as fh:
             rdata_metadata = self._upload_and_get_details(fh, file_type="auto")
-        self.assertEqual(rdata_metadata["file_ext"], "rdata")
+        assert rdata_metadata["file_ext"] == "rdata"
 
     @skip_without_datatype("csv")
     def test_csv_upload(self):
         csv_path = TestDataResolver().get_filename("1.csv")
         with open(csv_path, "rb") as fh:
             csv_metadata = self._upload_and_get_details(fh, file_type="csv")
-        self.assertEqual(csv_metadata["file_ext"], "csv")
+        assert csv_metadata["file_ext"] == "csv"
 
     @skip_without_datatype("csv")
     def test_csv_upload_auto(self):
         csv_path = TestDataResolver().get_filename("1.csv")
         with open(csv_path, "rb") as fh:
             csv_metadata = self._upload_and_get_details(fh, file_type="auto")
-        self.assertEqual(csv_metadata["file_ext"], "csv")
+        assert csv_metadata["file_ext"] == "csv"
 
     @skip_without_datatype("csv")
     def test_csv_fetch(self):
         csv_path = TestDataResolver().get_filename("1.csv")
         with open(csv_path, "rb") as fh:
             csv_metadata = self._upload_and_get_details(fh, api="fetch", ext="csv", to_posix_lines=True)
-        self.assertEqual(csv_metadata["file_ext"], "csv")
+        assert csv_metadata["file_ext"] == "csv"
 
     @skip_without_datatype("csv")
     def test_csv_sniff_fetch(self):
         csv_path = TestDataResolver().get_filename("1.csv")
         with open(csv_path, "rb") as fh:
             csv_metadata = self._upload_and_get_details(fh, api="fetch", ext="auto", to_posix_lines=True)
-        self.assertEqual(csv_metadata["file_ext"], "csv")
+        assert csv_metadata["file_ext"] == "csv"
 
     @skip_without_datatype("tiff")
     def test_image_upload_auto(self):
         tiff_path = TestDataResolver().get_filename("1.tiff")
         with open(tiff_path, "rb") as fh:
             tiff_metadata = self._upload_and_get_details(fh, file_type="auto")
-        self.assertEqual(tiff_metadata["file_ext"], "tiff")
+        assert tiff_metadata["file_ext"] == "tiff"
 
-    @uses_test_history(require_new=False)
-    def test_newlines_stage_fetch(self, history_id):
+    def test_newlines_stage_fetch(self, history_id: str) -> None:
         job = {
             "input1": {
                 "class": "File",
                 "format": "txt",
                 "path": "test-data/simple_line_no_newline.txt",
             }
         }
         inputs, datasets = stage_inputs(self.galaxy_interactor, history_id, job, use_path_paste=False)
-        dataset = datasets[0][0]
+        dataset = datasets[0]
         content = self.dataset_populator.get_history_dataset_content(history_id=history_id, dataset=dataset)
         # By default this appends the newline.
-        self.assertEqual(content, "This is a line of text.\n")
+        assert content == "This is a line of text.\n"
 
-    @uses_test_history(require_new=False)
-    def test_stage_object(self, history_id):
+    def test_stage_object(self, history_id: str) -> None:
         job = {"input1": "randomstr"}
         inputs, datasets = stage_inputs(
             self.galaxy_interactor, history_id, job, use_path_paste=False, use_fetch_api=False
         )
-        dataset = datasets[0][0]
+        dataset = datasets[0]
         content = self.dataset_populator.get_history_dataset_content(history_id=history_id, dataset=dataset)
-        self.assertEqual(content.strip(), '"randomstr"')
+        assert content.strip() == '"randomstr"'
 
-    @uses_test_history(require_new=False)
-    def test_stage_object_fetch(self, history_id):
+    def test_stage_object_fetch(self, history_id: str) -> None:
         job = {"input1": "randomstr"}
         inputs, datasets = stage_inputs(self.galaxy_interactor, history_id, job, use_path_paste=False)
-        dataset = datasets[0][0]
+        dataset = datasets[0]
         content = self.dataset_populator.get_history_dataset_content(history_id=history_id, dataset=dataset)
-        self.assertEqual(content, '"randomstr"')
+        assert content == '"randomstr"'
 
-    @uses_test_history(require_new=False)
-    def test_newlines_stage_fetch_configured(self, history_id):
+    def test_newlines_stage_fetch_configured(self, history_id: str) -> None:
         job = {
             "input1": {
                 "class": "File",
                 "format": "txt",
                 "path": "test-data/simple_line_no_newline.txt",
                 "dbkey": "hg19",
             }
         }
         inputs, datasets = stage_inputs(
             self.galaxy_interactor, history_id, job, use_path_paste=False, to_posix_lines=False
         )
-        dataset = datasets[0][0]
+        dataset = datasets[0]
         content = self.dataset_populator.get_history_dataset_content(history_id=history_id, dataset=dataset)
         # By default this appends the newline, but we disabled with 'to_posix_lines=False' above.
-        self.assertEqual(content, "This is a line of text.")
+        assert content == "This is a line of text."
         details = self.dataset_populator.get_history_dataset_details(history_id=history_id, dataset=dataset)
         assert details["genome_build"] == "hg19"
 
-    @uses_test_history(require_new=False)
+    @skip_if_github_down
+    def test_stage_fetch_decompress_true(self, history_id: str) -> None:
+        job = {
+            "input1": {
+                "class": "File",
+                "format": "fasta",
+                "location": "https://github.com/galaxyproject/galaxy/blob/dev/test-data/1.fasta.gz?raw=true",
+                "decompress": True,
+            }
+        }
+        inputs, datasets = stage_inputs(
+            self.galaxy_interactor, history_id, job, use_path_paste=False, to_posix_lines=False
+        )
+        dataset = datasets[0]
+        content = self.dataset_populator.get_history_dataset_content(history_id=history_id, dataset=dataset)
+        assert content.startswith(">hg17")
+
+    @skip_if_github_down
+    def test_stage_fetch_decompress_false(self, history_id: str) -> None:
+        job = {
+            "input1": {
+                "class": "File",
+                "format": "fasta",
+                "location": "https://github.com/galaxyproject/galaxy/blob/dev/test-data/1.fasta.gz?raw=true",
+                "decompress": False,
+            }
+        }
+        inputs, datasets = stage_inputs(
+            self.galaxy_interactor, history_id, job, use_path_paste=False, to_posix_lines=False
+        )
+        dataset = datasets[0]
+        content = self.dataset_populator.get_history_dataset_content(history_id=history_id, dataset=dataset)
+        assert not content.startswith(">hg17")
+
     @skip_if_github_down
     def test_upload_multiple_mixed_success(self, history_id):
         destination = {"type": "hdas"}
         targets = [
             {
                 "destination": destination,
                 "items": [
@@ -308,26 +340,24 @@
         output0 = outputs[0]
         output1 = outputs[1]
         output0 = self.dataset_populator.get_history_dataset_details(history_id, dataset=output0, assert_ok=False)
         output1 = self.dataset_populator.get_history_dataset_details(history_id, dataset=output1, assert_ok=False)
         assert output0["state"] == "ok"
         assert output1["state"] == "error"
 
-    @uses_test_history(require_new=False)
     @skip_if_github_down
     def test_fetch_bam_file_from_url_with_extension_set(self, history_id):
         item = {
             "src": "url",
             "url": "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/1.bam",
             "ext": "bam",
         }
         output = self.dataset_populator.fetch_hda(history_id, item)
         self.dataset_populator.get_history_dataset_details(history_id, dataset=output, assert_ok=True)
 
-    @uses_test_history(require_new=False)
     @skip_if_github_down
     def test_fetch_html_from_url(self, history_id):
         destination = {"type": "hdas"}
         targets = [
             {
                 "destination": destination,
                 "items": [
@@ -348,15 +378,14 @@
         output = response["outputs"][0]
         job = response["jobs"][0]
         self.dataset_populator.wait_for_job(job["id"])
         dataset = self.dataset_populator.get_history_dataset_details(history_id, dataset=output, assert_ok=False)
         assert dataset["state"] == "error"
         assert dataset["name"] == "html_file.txt"
 
-    @uses_test_history(require_new=False)
     def test_abort_fetch_job(self, history_id):
         # This should probably be an integration test that also verifies
         # that the celery chord is properly canceled.
         item = {
             "src": "url",
             "url": "https://httpstat.us/200?sleep=10000",
             "ext": "txt",
@@ -399,15 +428,14 @@
                 },
             )
 
             roadmaps_content = self._get_roadmaps_content(history_id, dataset)
             assert roadmaps_content.strip() == "roadmaps content", roadmaps_content
 
     @skip_without_datatype("velvet")
-    @uses_test_history(require_new=False)
     def test_composite_datatype_fetch(self, history_id):
         item = {
             "src": "composite",
             "ext": "velvet",
             "composite": {
                 "items": [
                     {"src": "pasted", "paste_content": "sequences content"},
@@ -417,68 +445,62 @@
             },
         }
         output = self.dataset_populator.fetch_hda(history_id, item)
         roadmaps_content = self._get_roadmaps_content(history_id, output)
         assert roadmaps_content.strip() == "roadmaps content", roadmaps_content
 
     @skip_without_datatype("velvet")
-    @uses_test_history(require_new=False)
-    def test_composite_datatype_stage_fetch(self, history_id):
+    def test_composite_datatype_stage_fetch(self, history_id: str) -> None:
         job = {
             "input1": {
                 "class": "File",
                 "format": "velvet",
                 "composite_data": [
                     "test-data/simple_line.txt",
                     "test-data/simple_line_alternative.txt",
                     "test-data/simple_line_x2.txt",
                 ],
             }
         }
-        inputs, datsets = stage_inputs(self.galaxy_interactor, history_id, job, use_path_paste=False)
+        stage_inputs(self.galaxy_interactor, history_id, job, use_path_paste=False)
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
 
     @skip_without_datatype("velvet")
-    @uses_test_history(require_new=False)
-    def test_composite_datatype_pbed_stage_fetch(self, history_id):
+    def test_composite_datatype_pbed_stage_fetch(self, history_id: str) -> None:
         job = {
             "input1": {
                 "class": "File",
                 "format": "pbed",
                 "composite_data": [
                     "test-data/rgenetics.bim",
                     "test-data/rgenetics.bed",
                     "test-data/rgenetics.fam",
                 ],
             }
         }
-        inputs, datsets = stage_inputs(self.galaxy_interactor, history_id, job, use_path_paste=False)
+        stage_inputs(self.galaxy_interactor, history_id, job, use_path_paste=False)
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
 
     @skip_without_datatype("velvet")
-    @uses_test_history(require_new=False)
-    def test_composite_datatype_stage_upload1(self, history_id):
+    def test_composite_datatype_stage_upload1(self, history_id: str) -> None:
         job = {
             "input1": {
                 "class": "File",
                 "format": "velvet",
                 "composite_data": [
                     "test-data/simple_line.txt",
                     "test-data/simple_line_alternative.txt",
                     "test-data/simple_line_x2.txt",
                 ],
             }
         }
-        inputs, datsets = stage_inputs(
-            self.galaxy_interactor, history_id, job, use_path_paste=False, use_fetch_api=False
-        )
+        stage_inputs(self.galaxy_interactor, history_id, job, use_path_paste=False, use_fetch_api=False)
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
 
     @skip_without_datatype("velvet")
-    @uses_test_history(require_new=False)
     def test_composite_datatype_space_to_tab(self, history_id):
         # Like previous test but set one upload with space_to_tab to True to
         # verify that works.
         dataset = self._velvet_upload(
             history_id,
             extra_inputs={
                 "files_1|url_paste": "roadmaps content",
@@ -515,15 +537,14 @@
     def test_composite_datatype_isatab(self):
         isatab_zip_path = TestDataResolver().get_filename("MTBLS6.zip")
         details = self._upload_and_get_details(open(isatab_zip_path, "rb"), file_type="isa-tab")
         assert details["state"] == "ok"
         assert details["file_ext"] == "isa-tab", details
         assert details["file_size"] == 85, details
 
-    @uses_test_history(require_new=False)
     def test_upload_composite_as_tar(self, history_id):
         tar_path = self.test_data_resolver.get_filename("testdir.tar")
         with open(tar_path, "rb") as tar_f:
             payload = self.dataset_populator.upload_payload(
                 history_id,
                 "Test123",
                 extra_inputs={
@@ -534,15 +555,14 @@
                 },
             )
             run_response = self.dataset_populator.tools_post(payload)
             self.dataset_populator.wait_for_tool_run(history_id, run_response)
             dataset = run_response.json()["outputs"][0]
             self._check_testdir_composite(dataset, history_id)
 
-    @uses_test_history(require_new=False)
     def test_upload_composite_as_tar_fetch(self, history_id):
         tar_path = self.test_data_resolver.get_filename("testdir.tar")
         with open(tar_path, "rb") as tar_f:
             destination = {"type": "hdas"}
             targets = [
                 {
                     "destination": destination,
@@ -591,15 +611,14 @@
             path = extra_file["path"]
             assert path in expected_contents
             assert extra_file["class"] == expected_contents[path]
             found_files.add(path)
 
         assert len(found_files) == 5, found_files
 
-    @uses_test_history(require_new=False)
     def test_upload_composite_from_bad_tar(self, history_id):
         tar_path = self.test_data_resolver.get_filename("unsafe.tar")
         with open(tar_path, "rb") as tar_f:
             payload = self.dataset_populator.upload_payload(
                 history_id,
                 "Test123",
                 extra_inputs={
@@ -619,15 +638,14 @@
         with self.dataset_populator.test_history() as history_id:
             payload = self.dataset_populator.upload_payload(history_id, "Test123", dbkey="hg19")
             run_response = self.dataset_populator.tools_post(payload)
             self.dataset_populator.wait_for_tool_run(history_id, run_response)
             datasets = run_response.json()["outputs"]
             assert datasets[0].get("genome_build") == "hg19", datasets[0]
 
-    @uses_test_history(require_new=False)
     def test_fetch_bam_file(self, history_id):
         bam_path = TestDataResolver().get_filename("1.bam")
         with open(bam_path, "rb") as fh:
             details = self._upload_and_get_details(fh, api="fetch", history_id=history_id, assert_ok=False)
         assert details["state"] == "ok"
         assert details["file_ext"] == "bam", details
 
@@ -986,14 +1004,13 @@
                 ext="fastqsanger.gz",
                 name="1.fastqsanger.gz",
             )
             assert hda["name"] == "1.fastqsanger.gz"
             assert hda["file_ext"] == "fastqsanger.gz"
             assert hda["state"] == "ok"
 
-    @uses_test_history(require_new=False)
     def test_upload_deferred(self, history_id):
         details = self.dataset_populator.create_deferred_hda(
             history_id, "https://raw.githubusercontent.com/galaxyproject/galaxy/dev/test-data/1.bam", ext="bam"
         )
         assert details["state"] == "deferred"
         assert details["file_ext"] == "bam"
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_tours.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_tours.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ._framework import ApiTestCase
 
 
-class TourApiTestCase(ApiTestCase):
+class TestToursApi(ApiTestCase):
     def test_index(self):
         response = self._get("tours")
         self._assert_status_code_is(response, 200)
         tours = response.json()
         tour_keys = map(lambda t: t["id"], tours)
         assert "core.history" in tour_keys
         for tour in tours:
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_users.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_users.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from requests import (
     delete,
     get,
     put,
 )
 
+from galaxy_test.api._framework import ApiTestCase
 from galaxy_test.base.api_asserts import assert_object_id_error
 from galaxy_test.base.populators import skip_without_tool
-from ._framework import ApiTestCase
 
 TEST_USER_EMAIL = "user_for_users_index_test@bx.psu.edu"
 TEST_USER_EMAIL_DELETE = "user_for_delete_test@bx.psu.edu"
 TEST_USER_EMAIL_PURGE = "user_for_purge_test@bx.psu.edu"
 TEST_USER_EMAIL_UNDELETE = "user_for_undelete_test@bx.psu.edu"
 
 
-class UsersApiTestCase(ApiTestCase):
+class TestUsersApi(ApiTestCase):
     def test_index(self):
         self._setup_user(TEST_USER_EMAIL)
         all_users_response = self._get("users", admin=True)
         self._assert_status_code_is(all_users_response, 200)
         all_users = all_users_response.json()
         # New user is in list
         assert len([u for u in all_users if u["email"] == TEST_USER_EMAIL]) == 1
@@ -43,43 +43,42 @@
             self.__assert_matches_user(user, show_response.json())
 
     def test_update(self):
         new_name = "linnaeus"
         user = self._setup_user(TEST_USER_EMAIL)
         not_the_user = self._setup_user("email@example.com")
         with self._different_user(email=TEST_USER_EMAIL):
-
             # working
             update_response = self.__update(user, username=new_name)
             self._assert_status_code_is(update_response, 200)
             update_json = update_response.json()
-            self.assertEqual(update_json["username"], new_name)
+            assert update_json["username"] == new_name
 
             # too short
             update_response = self.__update(user, username="")
             self._assert_status_code_is(update_response, 400)
 
             # not them
             update_response = self.__update(not_the_user, username=new_name)
-            self._assert_status_code_is(update_response, 403)
+            self._assert_status_code_is(update_response, 400)
 
             # non-existent
             no_user_id = "5d7db0757a2eb7ef"
             update_url = self._api_url(f"users/{no_user_id}", use_key=True)
             update_response = put(update_url, data=json.dumps(dict(username=new_name)))
             assert_object_id_error(update_response)
 
     def test_admin_update(self):
         new_name = "flexo"
         user = self._setup_user(TEST_USER_EMAIL)
         update_url = self._api_url(f"users/{user['id']}", params=dict(key=self.master_api_key))
         update_response = put(update_url, data=json.dumps(dict(username=new_name)))
         self._assert_status_code_is(update_response, 200)
         update_json = update_response.json()
-        self.assertEqual(update_json["username"], new_name)
+        assert update_json["username"] == new_name
 
     def test_delete_user(self):
         user = self._setup_user(TEST_USER_EMAIL_DELETE)
         self._delete(f"users/{user['id']}", admin=True)
         updated_user = self._get(f"users/deleted/{user['id']}", admin=True).json()
         assert updated_user["deleted"] is True, updated_user
 
@@ -107,53 +106,91 @@
         undeleted_user = self._get(f"users/{user['id']}", admin=True).json()
         assert undeleted_user["deleted"] is False, undeleted_user
 
     def test_information(self):
         user = self._setup_user(TEST_USER_EMAIL)
         url = self.__url("information/inputs", user)
         response = get(url).json()
-        self.assertEqual(response["username"], user["username"])
-        self.assertEqual(response["email"], TEST_USER_EMAIL)
+        assert response["username"] == user["username"]
+        assert response["email"] == TEST_USER_EMAIL
         put(url, data=json.dumps(dict(username="newname", email="new@email.email")))
         response = get(url).json()
-        self.assertEqual(response["username"], "newname")
-        self.assertEqual(response["email"], "new@email.email")
+        assert response["username"] == "newname"
+        assert response["email"] == "new@email.email"
         put(url, data=json.dumps(dict(username=user["username"], email=TEST_USER_EMAIL)))
         response = get(url).json()
-        self.assertEqual(response["username"], user["username"])
-        self.assertEqual(response["email"], TEST_USER_EMAIL)
+        assert response["username"] == user["username"]
+        assert response["email"] == TEST_USER_EMAIL
         put(url, data=json.dumps({"address_0|desc": "_desc"}))
         response = get(url).json()
-        self.assertEqual(len(response["addresses"]), 1)
-        self.assertEqual(response["addresses"][0]["desc"], "_desc")
+        assert len(response["addresses"]) == 1
+        assert response["addresses"][0]["desc"] == "_desc"
 
-    def test_create_api_key(self):
-        user = self._setup_user(TEST_USER_EMAIL)
-        user_id = user["id"]
-        response = self._put(f"users/{user_id}/api_key/inputs", admin=True)
+    def test_manage_api_key(self):
+        with self._different_user("manage-api-key-test@user.com"):
+            user_id = self._get_current_user_id()
+            # Initially we have an API key because it is bootstrapped for tests
+            response = self._get(f"users/{user_id}/api_key")
+            user_api_key = response.json()
+            assert user_api_key
+            # Test detailed endpoint
+            response = self._get(f"users/{user_id}/api_key/detailed")
+            api_key = response.json()
+            assert api_key["key"] == user_api_key
+            # Delete user API key
+            response = self._delete(f"users/{user_id}/api_key")
+            self._assert_status_code_is(response, 204)
+            # No API key anymore, so the detailed request returns no content 204
+            response = self._get(f"users/{user_id}/api_key/detailed")
+            self._assert_status_code_is(response, 204)
+            # create new as admin
+            response = self._post(f"users/{user_id}/api_key", admin=True)
+            self._assert_status_code_is_ok(response)
+            new_api_key = response.json()
+            assert new_api_key
+            assert new_api_key != user_api_key
+
+    def test_only_admin_can_manage_other_users_api_key(self):
+        with self._different_user():
+            other_user_id = self._get_current_user_id()
+        current_user_id = self._get_current_user_id()
+        # Users cannot access other users API keys
+        assert current_user_id != other_user_id
+        response = self._get(f"users/{other_user_id}/api_key")
+        self._assert_status_code_is(response, 403)
+        response = self._post(f"users/{other_user_id}/api_key")
+        self._assert_status_code_is(response, 403)
+        response = self._delete(f"users/{other_user_id}/api_key")
+        self._assert_status_code_is(response, 403)
+
+        # Admins can access other users API keys
+        response = self._get(f"users/{other_user_id}/api_key", admin=True)
+        self._assert_status_code_is_ok(response)
+        response = self._post(f"users/{other_user_id}/api_key", admin=True)
+        self._assert_status_code_is_ok(response)
+        response = self._delete(f"users/{other_user_id}/api_key", admin=True)
         self._assert_status_code_is_ok(response)
-        self.assertEqual(response.json()["inputs"][0]["name"], "api-key")
 
     @skip_without_tool("cat1")
     def test_favorites(self):
         user = self._setup_user(TEST_USER_EMAIL)
         # adding a tool to favorites
         url = self._api_url(f"users/{user['id']}/favorites/tools", params=dict(key=self.master_api_key))
         put_response = put(url, data=json.dumps({"object_id": "cat1"}))
         self._assert_status_code_is_ok(put_response)
-        self.assertEqual(put_response.json()["tools"][0], "cat1")
+        assert put_response.json()["tools"][0] == "cat1"
         # not implemented for workflows yet
         url = self._api_url(f"users/{user['id']}/favorites/workflows", params=dict(key=self.master_api_key))
         put_response = put(url, data=json.dumps({"object_id": "14ds68f4sda68gf46dsag4"}))
         self._assert_status_code_is(put_response, 400)
         # delete existing tool favorite
         url = self._api_url(f"users/{user['id']}/favorites/tools/cat1", params=dict(key=self.master_api_key))
         delete_response = delete(url)
         self._assert_status_code_is_ok(delete_response)
-        self.assertEqual(delete_response.json()["tools"], [])
+        assert delete_response.json()["tools"] == []
         # delete non-existing tool favorite
         url = self._api_url(
             f"users/{user['id']}/favorites/tools/madeuptoolthatdoes/not/exist/in/favs",
             params=dict(key=self.master_api_key),
         )
         delete_response = delete(url)
         self._assert_status_code_is(delete_response, 404)
@@ -185,7 +222,31 @@
         update_url = self._api_url(f"users/{user['id']}", use_key=True)
         return put(update_url, data=new_data)
 
     def __assert_matches_user(self, userA, userB):
         self._assert_has_keys(userB, "id", "username", "total_disk_usage")
         assert userA["id"] == userB["id"]
         assert userA["username"] == userB["username"]
+
+    def _get_current_user_id(self):
+        users_response = self._get("users")
+        users = users_response.json()
+        assert len(users) == 1
+        return users[0]["id"]
+
+    def test_manage_beacon_settings(self):
+        user_id = self._get_current_user_id()
+
+        # Assert that beacon sharing is initially disabled
+        response = self._get(f"users/{user_id}/beacon")
+        user_beacon_settings = response.json()
+        assert not user_beacon_settings["enabled"]
+
+        # Check if post request is successful
+        response = self._post(f"users/{user_id}/beacon", data={"enabled": True}, json=True)
+        user_beacon_settings = response.json()
+        assert user_beacon_settings["enabled"]
+
+        # Check if the setting has been persisted
+        response = self._get(f"users/{user_id}/beacon")
+        user_beacon_settings = response.json()
+        assert user_beacon_settings["enabled"]
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_visualizations.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_visualizations.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from ._framework import ApiTestCase
 
 INDEX_KEYS = ["id", "title", "type", "dbkey", "url"]
 SHOW_KEYS = INDEX_KEYS + ["user_id", "model_class", "revisions", "latest_revision", "annotation"]
 REVISION_KEYS = ["id", "title", "visualization_id", "dbkey", "model_class", "config"]
 
 
-class VisualizationsApiTestCase(ApiTestCase, SharingApiTests):
-
+class TestVisualizationsApi(ApiTestCase, SharingApiTests):
     api_name = "visualizations"
 
     def create(self, _: str) -> str:
         viz_id, _ = self._create_viz()
         return viz_id
 
     def test_index_and_show(self):
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_webhooks.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_webhooks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 from ._framework import ApiTestCase
 
 
-class WebhooksApiTestCase(ApiTestCase):
+class TestWebhooksApi(ApiTestCase):
     def setUp(self):
         super().setUp()
 
     def test_get_all(self):
         response = self._get("webhooks")
 
         self._assert_status_code_is(response, 200)
         webhook_objs = self._assert_are_webhooks(response)
         ids = self._get_webhook_ids(webhook_objs)
-        for expected_id in ["history_test1", "history_test2", "masthead_test", "phdcomics", "trans_object", "xkcd"]:
+        for expected_id in [
+            "history_test1",
+            "history_test2",
+            "masthead_test",
+            "phdcomics",
+            "trans_object",
+            "xkcd",
+            "gtn",
+        ]:
             assert expected_id in ids
 
     def test_get_data(self):
         response = self._get("webhooks/trans_object/data")
         self._assert_status_code_is(response, 200)
         self._assert_has_keys(response.json(), "username")
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_workflow_extraction.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_workflow_extraction.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,170 +9,171 @@
 from galaxy_test.base.populators import (
     skip_without_tool,
     summarize_instance_history_on_error,
 )
 from .test_workflows import BaseWorkflowsApiTestCase
 
 
-class WorkflowExtractionApiTestCase(BaseWorkflowsApiTestCase):
-    history_id: str
-
-    def setUp(self):
-        super().setUp()
-        self.history_id = self.dataset_populator.new_history()
-
+class TestWorkflowExtractionApi(BaseWorkflowsApiTestCase):
     @skip_without_tool("cat1")
     @summarize_instance_history_on_error
-    def test_extract_from_history(self):
+    def test_extract_from_history(self, history_id):
         # Run the simple test workflow and extract it back out from history
-        cat1_job_id = self.__setup_and_run_cat1_workflow(history_id=self.history_id)
-        contents = self._history_contents()
+        cat1_job_id = self.__setup_and_run_cat1_workflow(history_id=history_id)
+        contents = self._history_contents(history_id)
         input_hids = [c["hid"] for c in contents[0:2]]
         downloaded_workflow = self._extract_and_download_workflow(
+            history_id,
             reimport_as="extract_from_history_basic",
             dataset_ids=input_hids,
             job_ids=[cat1_job_id],
         )
-        self.assertEqual(downloaded_workflow["name"], "test import from history")
+        assert downloaded_workflow["name"] == "test import from history"
         self.__assert_looks_like_cat1_example_workflow(downloaded_workflow)
 
     @summarize_instance_history_on_error
-    def test_extract_with_copied_inputs(self):
+    def test_extract_with_copied_inputs(self, history_id):
         old_history_id = self.dataset_populator.new_history()
         # Run the simple test workflow and extract it back out from history
         self.__setup_and_run_cat1_workflow(history_id=old_history_id)
 
         # Bug cannot mess up hids or these don't extract correctly. See Trello card here:
         # https://trello.com/c/mKzLbM2P
         # # create dummy dataset to complicate hid mapping
         # self.dataset_populator.new_dataset( history_id, content="dummydataset" )
         # offset = 1
 
         offset = 0
         old_contents = self._history_contents(old_history_id)
         for old_dataset in old_contents:
-            self.__copy_content_to_history(self.history_id, old_dataset)
-        new_contents = self._history_contents()
+            self.__copy_content_to_history(history_id, old_dataset)
+        new_contents = self._history_contents(history_id)
         input_hids = [c["hid"] for c in new_contents[(offset + 0) : (offset + 2)]]
-        cat1_job_id = self.__job_id(self.history_id, new_contents[(offset + 2)]["id"])
+        cat1_job_id = self.__job_id(history_id, new_contents[(offset + 2)]["id"])
 
         def reimport_jobs_ids(new_history_id):
             return [j["id"] for j in self.dataset_populator.history_jobs(new_history_id) if j["tool_id"] == "cat1"]
 
         downloaded_workflow = self._extract_and_download_workflow(
+            history_id,
             dataset_ids=input_hids,
             job_ids=[cat1_job_id],
         )
         self.__assert_looks_like_cat1_example_workflow(downloaded_workflow)
 
     @summarize_instance_history_on_error
-    def test_extract_with_copied_inputs_reimported(self):
+    def test_extract_with_copied_inputs_reimported(self, history_id):
         old_history_id = self.dataset_populator.new_history()
         # Run the simple test workflow and extract it back out from history
         self.__setup_and_run_cat1_workflow(history_id=old_history_id)
 
         offset = 0
         old_contents = self._history_contents(old_history_id)
         for old_dataset in old_contents:
-            self.__copy_content_to_history(self.history_id, old_dataset)
-        new_contents = self._history_contents()
+            self.__copy_content_to_history(history_id, old_dataset)
+        new_contents = self._history_contents(history_id)
         input_hids = [c["hid"] for c in new_contents[(offset + 0) : (offset + 2)]]
 
         def reimport_jobs_ids(new_history_id):
             return [j["id"] for j in self.dataset_populator.history_jobs(new_history_id) if j["tool_id"] == "cat1"]
 
         downloaded_workflow = self._extract_and_download_workflow(
+            history_id,
             reimport_as="test_extract_with_copied_inputs",
             reimport_jobs_ids=reimport_jobs_ids,
             dataset_ids=input_hids,
         )
         self.__assert_looks_like_cat1_example_workflow(downloaded_workflow)
 
     @skip_without_tool("random_lines1")
     @summarize_instance_history_on_error
-    def test_extract_mapping_workflow_from_history(self):
-        hdca, job_id1, job_id2 = self.__run_random_lines_mapped_over_pair(self.history_id)
+    def test_extract_mapping_workflow_from_history(self, history_id):
+        hdca, job_id1, job_id2 = self.__run_random_lines_mapped_over_pair(history_id)
         downloaded_workflow = self._extract_and_download_workflow(
+            history_id,
             reimport_as="extract_from_history_with_mapping",
             dataset_collection_ids=[hdca["hid"]],
             job_ids=[job_id1, job_id2],
         )
         self.__assert_looks_like_randomlines_mapping_workflow(downloaded_workflow)
 
-    def test_extract_copied_mapping_from_history(self):
+    def test_extract_copied_mapping_from_history(self, history_id):
         old_history_id = self.dataset_populator.new_history()
         hdca, job_id1, job_id2 = self.__run_random_lines_mapped_over_pair(old_history_id)
 
         old_contents = self._history_contents(old_history_id)
         for old_content in old_contents:
-            self.__copy_content_to_history(self.history_id, old_content)
+            self.__copy_content_to_history(history_id, old_content)
         # API test is somewhat contrived since there is no good way
         # to retrieve job_id1, job_id2 like this for copied dataset
         # collections I don't think.
         downloaded_workflow = self._extract_and_download_workflow(
+            history_id,
             dataset_collection_ids=[hdca["hid"]],
             job_ids=[job_id1, job_id2],
         )
         self.__assert_looks_like_randomlines_mapping_workflow(downloaded_workflow)
 
-    def test_extract_copied_mapping_from_history_reimported(self):
+    def test_extract_copied_mapping_from_history_reimported(self, history_id):
         import unittest
 
         raise unittest.SkipTest(
             "Mapping connection for copied collections not yet implemented in history import/export"
         )
 
         old_history_id = self.dataset_populator.new_history()
         hdca, job_id1, job_id2 = self.__run_random_lines_mapped_over_singleton(old_history_id)
 
         old_contents = self._history_contents(old_history_id)
         for old_content in old_contents:
-            self.__copy_content_to_history(self.history_id, old_content)
+            self.__copy_content_to_history(history_id, old_content)
 
         def reimport_jobs_ids(new_history_id):
             rval = [
                 j["id"] for j in self.dataset_populator.history_jobs(new_history_id) if j["tool_id"] == "random_lines1"
             ]
             assert len(rval) == 2
             print(rval)
             return rval
 
         # API test is somewhat contrived since there is no good way
         # to retrieve job_id1, job_id2 like this for copied dataset
         # collections I don't think.
         downloaded_workflow = self._extract_and_download_workflow(
+            history_id,
             reimport_as="test_extract_from_history_with_mapped_collection_reimport",
             reimport_jobs_ids=reimport_jobs_ids,
             reimport_wait_on_history_length=9,  # see comments in _extract about eliminating this magic constant.
             dataset_collection_ids=[hdca["hid"]],
         )
         self.__assert_looks_like_randomlines_mapping_workflow(downloaded_workflow)
 
     @skip_without_tool("random_lines1")
     @skip_without_tool("multi_data_param")
-    def test_extract_reduction_from_history(self):
+    def test_extract_reduction_from_history(self, history_id):
         hdca = self.dataset_collection_populator.create_pair_in_history(
-            self.history_id, contents=["1 2 3\n4 5 6", "7 8 9\n10 11 10"], wait=True
+            history_id, contents=["1 2 3\n4 5 6", "7 8 9\n10 11 10"], wait=True
         ).json()["outputs"][0]
         hdca_id = hdca["id"]
         inputs1 = {"input": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]}, "num_lines": 2}
-        implicit_hdca1, job_id1 = self._run_tool_get_collection_and_job_id(self.history_id, "random_lines1", inputs1)
+        implicit_hdca1, job_id1 = self._run_tool_get_collection_and_job_id(history_id, "random_lines1", inputs1)
         inputs2 = {
             "f1": {"src": "hdca", "id": implicit_hdca1["id"]},
             "f2": {"src": "hdca", "id": implicit_hdca1["id"]},
         }
         reduction_run_output = self.dataset_populator.run_tool(
             tool_id="multi_data_param",
             inputs=inputs2,
-            history_id=self.history_id,
+            history_id=history_id,
         )
         job_id2 = reduction_run_output["jobs"][0]["id"]
         self.dataset_populator.wait_for_job(job_id2, assert_ok=True)
-        self.dataset_populator.wait_for_history(self.history_id, assert_ok=True)
+        self.dataset_populator.wait_for_history(history_id, assert_ok=True)
         downloaded_workflow = self._extract_and_download_workflow(
+            history_id,
             reimport_as="extract_from_history_with_reduction",
             dataset_collection_ids=[hdca["hid"]],
             job_ids=[job_id1, job_id2],
         )
         assert len(downloaded_workflow["steps"]) == 3
         collect_step_idx = self._assert_first_step_is_paired_input(downloaded_workflow)
         tool_steps = self._get_steps_of_type(downloaded_workflow, "tool", expected_len=2)
@@ -185,32 +186,34 @@
         assert "input" in random_lines_input_connections, random_lines_map_step
         random_lines_input = random_lines_input_connections["input"]
         assert random_lines_input["id"] == collect_step_idx
         reduction_step_input = reduction_step["input_connections"]["f1"]
         assert reduction_step_input["id"] == random_lines_map_step["id"]
 
     @skip_without_tool("collection_paired_test")
-    def test_extract_workflows_with_dataset_collections(self):
+    def test_extract_workflows_with_dataset_collections(self, history_id):
         jobs_summary = self._run_workflow(
             """
 class: GalaxyWorkflow
 steps:
   - label: text_input1
     type: input_collection
   - tool_id: collection_paired_test
     state:
       f1:
         $link: text_input1
 test_data:
   text_input1:
     collection_type: paired
-"""
+""",
+            history_id,
         )
         job_id = self._job_id_for_tool(jobs_summary.jobs, "collection_paired_test")
         downloaded_workflow = self._extract_and_download_workflow(
+            history_id,
             reimport_as="extract_from_history_with_basic_collections",
             dataset_collection_ids=["1"],
             job_ids=[job_id],
         )
         self.__check_workflow(
             downloaded_workflow,
             step_count=2,
@@ -218,18 +221,18 @@
             data_input_count=0,
             data_collection_input_count=1,
             tool_ids=["collection_paired_test"],
         )
 
         collection_step = self._get_steps_of_type(downloaded_workflow, "data_collection_input", expected_len=1)[0]
         collection_step_state = loads(collection_step["tool_state"])
-        self.assertEqual(collection_step_state["collection_type"], "paired")
+        assert collection_step_state["collection_type"] == "paired"
 
     @skip_without_tool("cat_collection")
-    def test_subcollection_mapping(self):
+    def test_subcollection_mapping(self, history_id):
         jobs_summary = self._run_workflow(
             """
 class: GalaxyWorkflow
 steps:
   - label: text_input1
     type: input_collection
   - label: noop
@@ -240,19 +243,21 @@
   - tool_id: cat_collection
     state:
       input1:
         $link: noop/out_file1
 test_data:
   text_input1:
     collection_type: "list:paired"
-        """
+        """,
+            history_id,
         )
         job1_id = self._job_id_for_tool(jobs_summary.jobs, "cat1")
         job2_id = self._job_id_for_tool(jobs_summary.jobs, "cat_collection")
         downloaded_workflow = self._extract_and_download_workflow(
+            history_id,
             reimport_as="test_extract_workflows_with_subcollection_mapping",
             dataset_collection_ids=["1"],
             job_ids=[job1_id, job2_id],
         )
         self.__check_workflow(
             downloaded_workflow,
             step_count=3,
@@ -260,43 +265,45 @@
             data_input_count=0,
             data_collection_input_count=1,
             tool_ids=["cat_collection", "cat1"],
         )
 
         collection_step = self._get_steps_of_type(downloaded_workflow, "data_collection_input", expected_len=1)[0]
         collection_step_state = loads(collection_step["tool_state"])
-        self.assertEqual(collection_step_state["collection_type"], "list:paired")
+        assert collection_step_state["collection_type"] == "list:paired"
 
     @skip_without_tool("cat_list")
     @skip_without_tool("collection_creates_dynamic_nested")
-    def test_subcollection_reduction(self):
+    def test_subcollection_reduction(self, history_id):
         jobs_summary = self._run_workflow(
             """
 class: GalaxyWorkflow
 steps:
   creates_nested_list:
     tool_id: collection_creates_dynamic_nested
   reduce_nested_list:
     tool_id: cat_list
     in:
       input1: creates_nested_list/list_output
-"""
+""",
+            history_id,
         )
         job1_id = self._job_id_for_tool(jobs_summary.jobs, "cat_list")
         job2_id = self._job_id_for_tool(jobs_summary.jobs, "collection_creates_dynamic_nested")
         self._extract_and_download_workflow(
+            history_id,
             reimport_as="test_extract_workflows_with_subcollection_reduction",
             dataset_collection_ids=["1"],
             job_ids=[job1_id, job2_id],
         )
         # TODO: refactor workflow extraction to not rely on HID, so we can actually properly connect
         # this workflow
 
     @skip_without_tool("collection_split_on_column")
-    def test_extract_workflow_with_output_collections(self):
+    def test_extract_workflow_with_output_collections(self, history_id):
         jobs_summary = self._run_workflow(
             """
 class: GalaxyWorkflow
 steps:
   - label: text_input1
     type: input
   - label: text_input2
@@ -317,19 +324,21 @@
   - tool_id: cat_list
     state:
       input1:
         $link: split_up/split_output
 test_data:
   text_input1: "samp1\t10.0\nsamp2\t20.0\n"
   text_input2: "samp1\t30.0\nsamp2\t40.0\n"
-"""
+""",
+            history_id,
         )
         tool_ids = ["cat1", "collection_split_on_column", "cat_list"]
         job_ids = [functools.partial(self._job_id_for_tool, jobs_summary.jobs)(_) for _ in tool_ids]
         downloaded_workflow = self._extract_and_download_workflow(
+            history_id,
             reimport_as="test_extract_workflows_with_output_collections",
             dataset_ids=["1", "2"],
             job_ids=job_ids,
         )
         self.__check_workflow(
             downloaded_workflow,
             step_count=5,
@@ -337,15 +346,15 @@
             data_input_count=2,
             data_collection_input_count=0,
             tool_ids=tool_ids,
         )
 
     @skip_without_tool("collection_creates_pair")
     @summarize_instance_history_on_error
-    def test_extract_with_mapped_output_collections(self):
+    def test_extract_with_mapped_output_collections(self, history_id):
         jobs_summary = self._run_workflow(
             """
 class: GalaxyWorkflow
 steps:
   - label: text_input1
     type: input_collection
   - label: cat_inputs
@@ -371,19 +380,21 @@
   text_input1:
     collection_type: list
     elements:
       - identifier: samp1
         content: "samp1\t10.0\nsamp2\t20.0\n"
       - identifier: samp2
         content: "samp1\t30.0\nsamp2\t40.0\n"
-"""
+""",
+            history_id,
         )
         tool_ids = ["cat1", "collection_creates_pair", "cat_collection", "cat_list"]
         job_ids = [functools.partial(self._job_id_for_tool, jobs_summary.jobs)(_) for _ in tool_ids]
         downloaded_workflow = self._extract_and_download_workflow(
+            history_id,
             reimport_as="test_extract_workflows_with_mapped_output_collections",
             dataset_collection_ids=["1"],
             job_ids=job_ids,
         )
         self.__check_workflow(
             downloaded_workflow,
             step_count=5,
@@ -446,20 +457,18 @@
         assert len(downloaded_workflow["steps"]) == 3
         input_steps = self._get_steps_of_type(downloaded_workflow, "data_input", expected_len=2)
         tool_step = self._get_steps_of_type(downloaded_workflow, "tool", expected_len=1)[0]
 
         input1 = tool_step["input_connections"]["input1"]
         input2 = tool_step["input_connections"]["queries_0|input2"]
 
-        self.assertEqual(input_steps[0]["id"], input1["id"])
-        self.assertEqual(input_steps[1]["id"], input2["id"])
+        assert input_steps[0]["id"] == input1["id"]
+        assert input_steps[1]["id"] == input2["id"]
 
-    def _history_contents(self, history_id=None):
-        if history_id is None:
-            history_id = self.history_id
+    def _history_contents(self, history_id: str):
         return self._get(f"histories/{history_id}/contents").json()
 
     def __copy_content_to_history(self, history_id, content):
         if content["history_content_type"] == "dataset":
             payload = dict(source="hda", content=content["id"])
             response = self._post(f"histories/{history_id}/contents/datasets", payload, json=True)
 
@@ -480,24 +489,23 @@
         )
         return self.__cat_job_id(history_id)
 
     def _assert_first_step_is_paired_input(self, downloaded_workflow):
         collection_steps = self._get_steps_of_type(downloaded_workflow, "data_collection_input", expected_len=1)
         collection_step = collection_steps[0]
         collection_step_state = loads(collection_step["tool_state"])
-        self.assertEqual(collection_step_state["collection_type"], "paired")
+        assert collection_step_state["collection_type"] == "paired"
         collect_step_idx = collection_step["id"]
         return collect_step_idx
 
-    def _extract_and_download_workflow(self, **extract_payload):
+    def _extract_and_download_workflow(self, history_id: str, **extract_payload):
         reimport_as = extract_payload.get("reimport_as")
 
         if reimport_as:
             history_name = reimport_as
-            history_id = self.history_id
             self.dataset_populator.wait_for_history(history_id)
             self.dataset_populator.rename_history(history_id, history_name)
 
             history_length = extract_payload.get("reimport_wait_on_history_length")
             if history_length is None:
                 # sometimes this won't be the same (i.e. datasets copied from outside the history
                 # that need to be included in target history for collections), but we can provide
@@ -541,18 +549,18 @@
                     job_ids = extract_payload["job_ids"]
                     new_job_ids = []
                     for job_id in job_ids:
                         new_job_ids.append(new_history_job_ids[history_job_ids.index(job_id)])
 
                     extract_payload["job_ids"] = new_job_ids
 
-            self.history_id = new_history_id
+            history_id = new_history_id
 
         if "from_history_id" not in extract_payload:
-            extract_payload["from_history_id"] = self.history_id
+            extract_payload["from_history_id"] = history_id
 
         if "workflow_name" not in extract_payload:
             extract_payload["workflow_name"] = "test import from history"
 
         for key in "job_ids", "dataset_ids", "dataset_collection_ids":
             if key in extract_payload:
                 value = extract_payload[key]
@@ -577,22 +585,22 @@
 
     def __job_id(self, history_id, dataset_id):
         url = f"histories/{history_id}/contents/{dataset_id}/provenance"
         prov_response = self._get(url, data=dict(follow=False))
         self._assert_status_code_is(prov_response, 200)
         return prov_response.json()["job_id"]
 
-    def __cat_job_id(self, history_id):
+    def __cat_job_id(self, history_id: str):
         data = dict(history_id=history_id, tool_id="cat1")
         jobs_response = self._get("jobs", data=data)
         self._assert_status_code_is(jobs_response, 200)
         cat1_job_id = jobs_response.json()[0]["id"]
         return cat1_job_id
 
-    def _run_tool_get_collection_and_job_id(self, history_id, tool_id, inputs):
+    def _run_tool_get_collection_and_job_id(self, history_id: str, tool_id, inputs):
         run_output1 = self.dataset_populator.run_tool(
             tool_id=tool_id,
             inputs=inputs,
             history_id=history_id,
         )
         implicit_hdca = run_output1["implicit_collections"][0]
         job_id = run_output1["jobs"][0]["id"]
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_workflows.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_workflows.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from uuid import uuid4
 
 import pytest
 import yaml
 from requests import (
     delete,
     get,
+    post,
     put,
 )
 
 from galaxy.exceptions import error_codes
 from galaxy_test.base import rules_test_data
 from galaxy_test.base.populators import (
     DatasetCollectionPopulator,
@@ -31,14 +32,15 @@
     RunJobsSummary,
     skip_without_tool,
     wait_on,
     workflow_str,
     WorkflowPopulator,
 )
 from galaxy_test.base.workflow_fixtures import (
+    NESTED_WORKFLOW_WITH_CONDITIONAL_SUBWORKFLOW_AND_DISCONNECTED_MAP_OVER_SOURCE,
     WORKFLOW_INPUTS_AS_OUTPUTS,
     WORKFLOW_NESTED_REPLACEMENT_PARAMETER,
     WORKFLOW_NESTED_RUNTIME_PARAMETER,
     WORKFLOW_NESTED_SIMPLE,
     WORKFLOW_ONE_STEP_DEFAULT,
     WORKFLOW_OPTIONAL_FALSE_INPUT_COLLECTION,
     WORKFLOW_OPTIONAL_FALSE_INPUT_DATA,
@@ -161,14 +163,15 @@
         usages = self.workflow_populator.workflow_invocations(workflow_id)
         assert len(usages) == 1
         return workflow_id, usages[0]
 
 
 class BaseWorkflowsApiTestCase(ApiTestCase, RunsWorkflowFixtures):
     # TODO: Find a new file for this class.
+    dataset_populator: DatasetPopulator
 
     def setUp(self):
         super().setUp()
         self.workflow_populator = WorkflowPopulator(self.galaxy_interactor)
         self.dataset_populator = DatasetPopulator(self.galaxy_interactor)
         self.dataset_collection_populator = DatasetCollectionPopulator(self.galaxy_interactor)
 
@@ -203,47 +206,42 @@
 
     def _invocation_details(self, workflow_id, invocation_id, **kwds):
         invocation_details_response = self._get(f"workflows/{workflow_id}/usage/{invocation_id}", data=kwds)
         self._assert_status_code_is(invocation_details_response, 200)
         invocation_details = invocation_details_response.json()
         return invocation_details
 
-    def _run_jobs(self, has_workflow, history_id=None, **kwds) -> Union[Dict[str, Any], RunJobsSummary]:
-        if history_id is None:
-            history_id = self.history_id
-
+    def _run_jobs(self, has_workflow, history_id: str, **kwds) -> Union[Dict[str, Any], RunJobsSummary]:
         return self.workflow_populator.run_workflow(has_workflow, history_id=history_id, **kwds)
 
-    def _run_workflow(self, has_workflow, history_id=None, **kwds) -> RunJobsSummary:
-        if history_id is None:
-            history_id = self.history_id
+    def _run_workflow(self, has_workflow, history_id: str, **kwds) -> RunJobsSummary:
         assert "expected_response" not in kwds
         run_summary = self.workflow_populator.run_workflow(has_workflow, history_id=history_id, **kwds)
         return cast(RunJobsSummary, run_summary)
 
     def _history_jobs(self, history_id):
         return self._get("jobs", {"history_id": history_id, "order_by": "create_time"}).json()
 
     def _assert_history_job_count(self, history_id, n):
         jobs = self._history_jobs(history_id)
-        self.assertEqual(len(jobs), n)
+        assert len(jobs) == n
 
     def _download_workflow(self, workflow_id, style=None, history_id=None):
         return self.workflow_populator.download_workflow(workflow_id, style=style, history_id=history_id)
 
     def _assert_is_runtime_input(self, tool_state_value):
         if not isinstance(tool_state_value, dict):
             tool_state_value = json.loads(tool_state_value)
 
         assert isinstance(tool_state_value, dict)
         assert "__class__" in tool_state_value
         assert tool_state_value["__class__"] == "RuntimeValue"
 
 
-class ChangeDatatypeTestCase:
+class ChangeDatatypeTests:
     dataset_populator: DatasetPopulator
     workflow_populator: WorkflowPopulator
 
     def test_assign_column_pja(self):
         with self.dataset_populator.test_history() as history_id:
             self.workflow_populator.run_workflow(
                 """
@@ -274,16 +272,15 @@
                 history_id, hid=2, wait=True, assert_ok=True
             )
             assert details_dataset_new_col["history_content_type"] == "dataset", details_dataset_new_col
             assert details_dataset_new_col["metadata_endCol"] == 2
             assert details_dataset_new_col["metadata_startCol"] == 3
 
 
-class WorkflowsSharingApiTestCase(ApiTestCase, SharingApiTests):
-
+class TestWorkflowSharingApi(ApiTestCase, SharingApiTests):
     api_name = "workflows"
 
     def create(self, name: str) -> str:
         """Creates a shareable resource with the given name and returns it's ID.
 
         :param name: The name of the shareable resource to create.
         :return: The ID of the resource.
@@ -304,31 +301,33 @@
 
 
 # Workflow API TODO:
 # - Allow history_id as param to workflow run action. (hist_id)
 # - Allow post to workflows/<workflow_id>/run in addition to posting to
 #    /workflows with id in payload.
 # - Much more testing obviously, always more testing.
-class WorkflowsApiTestCase(BaseWorkflowsApiTestCase, ChangeDatatypeTestCase):
+class TestWorkflowsApi(BaseWorkflowsApiTestCase, ChangeDatatypeTests):
+    dataset_populator: DatasetPopulator
+
     def test_show_valid(self):
         workflow_id = self.workflow_populator.simple_workflow("dummy")
         workflow_id = self.workflow_populator.simple_workflow("test_regular")
         show_response = self._get(f"workflows/{workflow_id}", {"style": "instance"})
         workflow = show_response.json()
         self._assert_looks_like_instance_workflow_representation(workflow)
         assert len(workflow["steps"]) == 3
-        self.assertEqual(sorted(step["id"] for step in workflow["steps"].values()), [0, 1, 2])
+        assert sorted(step["id"] for step in workflow["steps"].values()) == [0, 1, 2]
 
         show_response = self._get(f"workflows/{workflow_id}", {"legacy": True})
         workflow = show_response.json()
         self._assert_looks_like_instance_workflow_representation(workflow)
         assert len(workflow["steps"]) == 3
         # Can't reay say what the legacy IDs are but must be greater than 3 because dummy
         # workflow was created first in this instance.
-        self.assertNotEqual(sorted(step["id"] for step in workflow["steps"].values()), [0, 1, 2])
+        assert sorted(step["id"] for step in workflow["steps"].values()) != [0, 1, 2]
 
     def test_show_invalid_key_is_400(self):
         show_response = self._get(f"workflows/{self._random_key()}")
         self._assert_status_code_is(show_response, 400)
 
     def test_cannot_show_private_workflow(self):
         workflow_id = self.workflow_populator.simple_workflow("test_not_importable")
@@ -359,43 +358,70 @@
     def test_anon_can_download_public_workflow(self):
         workflow_id = self.workflow_populator.simple_workflow("test_downloadable", publish=True)
         workflows_url = self._api_url(f"workflows/{workflow_id}/download")
         response = get(workflows_url)
         response.raise_for_status()
         assert response.json()["a_galaxy_workflow"] == "true"
 
+    def test_anon_can_see_workflow_preview(self):
+        workflow_id = self.workflow_populator.simple_workflow(name="test_preview", importable=True)
+        workflows_url = self._api_url(f"workflows/{workflow_id}/download", params={"style": "preview"})
+        response = get(workflows_url)
+        response.raise_for_status()
+        assert response.json()["name"] == "test_preview"
+
     def test_delete(self):
         workflow_id = self.workflow_populator.simple_workflow("test_delete")
         workflow_name = "test_delete"
         self._assert_user_has_workflow_with_name(workflow_name)
         workflow_url = self._api_url(f"workflows/{workflow_id}", use_key=True)
         delete_response = delete(workflow_url)
-        self._assert_status_code_is(delete_response, 200)
+        self._assert_status_code_is(delete_response, 204)
         # Make sure workflow is no longer in index by default.
         assert workflow_name not in self._workflow_names()
 
     def test_other_cannot_delete(self):
         workflow_id = self.workflow_populator.simple_workflow("test_other_delete")
         with self._different_user():
             workflow_url = self._api_url(f"workflows/{workflow_id}", use_key=True)
             delete_response = delete(workflow_url)
             self._assert_status_code_is(delete_response, 403)
 
+    def test_undelete(self):
+        workflow_id = self.workflow_populator.simple_workflow("test_undelete")
+        workflow_name = "test_undelete"
+        self._assert_user_has_workflow_with_name(workflow_name)
+        workflow_delete_url = self._api_url(f"workflows/{workflow_id}", use_key=True)
+        delete(workflow_delete_url)
+        workflow_undelete_url = self._api_url(f"workflows/{workflow_id}/undelete", use_key=True)
+        undelete_response = post(workflow_undelete_url)
+        self._assert_status_code_is(undelete_response, 204)
+        assert workflow_name in self._workflow_names()
+
+    def test_other_cannot_undelete(self):
+        workflow_id = self.workflow_populator.simple_workflow("test_other_undelete")
+        workflow_delete_url = self._api_url(f"workflows/{workflow_id}", use_key=True)
+        delete(workflow_delete_url)
+        with self._different_user():
+            workflow_undelete_url = self._api_url(f"workflows/{workflow_id}/undelete", use_key=True)
+            undelete_response = post(workflow_undelete_url)
+            self._assert_status_code_is(undelete_response, 403)
+
     def test_index(self):
         index_response = self._get("workflows")
         self._assert_status_code_is(index_response, 200)
         assert isinstance(index_response.json(), list)
 
     def test_index_deleted(self):
         workflow_id = self.workflow_populator.simple_workflow("test_delete")
         workflow_index = self._get("workflows").json()
         assert [w for w in workflow_index if w["id"] == workflow_id]
         workflow_url = self._api_url(f"workflows/{workflow_id}", use_key=True)
         delete_response = delete(workflow_url)
-        self._assert_status_code_is(delete_response, 200)
+        self._assert_status_code_is(delete_response, 204)
         workflow_index = self._get("workflows").json()
         assert not [w for w in workflow_index if w["id"] == workflow_id]
         workflow_index = self._get("workflows?show_deleted=true").json()
         assert [w for w in workflow_index if w["id"] == workflow_id]
         workflow_index = self._get("workflows?show_deleted=false").json()
         assert not [w for w in workflow_index if w["id"] == workflow_id]
 
@@ -542,20 +568,21 @@
         assert workflow_id_1 in index_ids
         assert workflow_id_2 not in index_ids
 
     def test_index_search_tags(self):
         name1, name2 = self.dataset_populator.get_random_name(), self.dataset_populator.get_random_name()
         workflow_id_1 = self.workflow_populator.simple_workflow(name1)
         self.workflow_populator.simple_workflow(name2)
-        index_ids = self.workflow_populator.index_ids(search="moocowatag")
+        moocowtag = f"moocowatag {uuid4()}"
+        index_ids = self.workflow_populator.index_ids(search=moocowtag)
         assert len(index_ids) == 0
-        self.workflow_populator.set_tags(workflow_id_1, ["moocowatag", "moocowanothertag"])
-        index_ids = self.workflow_populator.index_ids(search="moocowatag")
+        self.workflow_populator.set_tags(workflow_id_1, [moocowtag, f"another{moocowtag}"])
+        index_ids = self.workflow_populator.index_ids(search=moocowtag)
         assert workflow_id_1 in index_ids
-        index_ids = self.workflow_populator.index_ids(search="tag:moocowatag")
+        index_ids = self.workflow_populator.index_ids(search=f"tag:{moocowtag}")
         assert workflow_id_1 in index_ids
 
     def test_index_search_tags_multiple(self):
         name1 = self.dataset_populator.get_random_name()
         name2 = self.dataset_populator.get_random_name()
         name3 = self.dataset_populator.get_random_name()
         workflow_id_1 = self.workflow_populator.simple_workflow(name1)
@@ -590,37 +617,39 @@
     def test_search_casing(self):
         name1, name2 = (
             self.dataset_populator.get_random_name().upper(),
             self.dataset_populator.get_random_name().upper(),
         )
         workflow_id_1 = self.workflow_populator.simple_workflow(name1)
         self.workflow_populator.simple_workflow(name2)
-        self.workflow_populator.set_tags(workflow_id_1, ["searchcasingtag", "searchcasinganothertag"])
+        searchcasingtag = f"searchcasingtag{uuid4()}"
+        self.workflow_populator.set_tags(workflow_id_1, [searchcasingtag, f"another{searchcasingtag}"])
         index_ids = self.workflow_populator.index_ids(search=name1.lower())
         assert len(index_ids) == 1
         assert workflow_id_1 in index_ids
-        index_ids = self.workflow_populator.index_ids(search="SEARCHCASINGTAG")
+        index_ids = self.workflow_populator.index_ids(search=searchcasingtag.upper())
         assert len(index_ids) == 1
         assert workflow_id_1 in index_ids
 
     def test_index_search_tags_exact(self):
         name1, name2 = self.dataset_populator.get_random_name(), self.dataset_populator.get_random_name()
         workflow_id_1 = self.workflow_populator.simple_workflow(name1)
         workflow_id_2 = self.workflow_populator.simple_workflow(name2)
-        index_ids = self.workflow_populator.index_ids(search="exacttagtosearch")
+        exact_tag_to_search = f"exacttagtosearch{uuid4()}"
+        index_ids = self.workflow_populator.index_ids(search=exact_tag_to_search)
         assert len(index_ids) == 0
-        self.workflow_populator.set_tags(workflow_id_1, ["exacttagtosearch"])
-        self.workflow_populator.set_tags(workflow_id_2, ["exacttagtosearchlonger"])
-        index_ids = self.workflow_populator.index_ids(search="exacttagtosearch")
+        self.workflow_populator.set_tags(workflow_id_1, [exact_tag_to_search])
+        self.workflow_populator.set_tags(workflow_id_2, [f"{exact_tag_to_search}longer"])
+        index_ids = self.workflow_populator.index_ids(search=exact_tag_to_search)
         assert workflow_id_1 in index_ids
         assert workflow_id_2 in index_ids
-        index_ids = self.workflow_populator.index_ids(search="tag:exacttagtosearch")
+        index_ids = self.workflow_populator.index_ids(search=f"tag:{exact_tag_to_search}")
         assert workflow_id_1 in index_ids
         assert workflow_id_2 in index_ids
-        index_ids = self.workflow_populator.index_ids(search="tag:'exacttagtosearch'")
+        index_ids = self.workflow_populator.index_ids(search=f"tag:'{exact_tag_to_search}'")
         assert workflow_id_1 in index_ids
         assert workflow_id_2 not in index_ids
 
     def test_index_published(self):
         # published workflows are also the default of what is displayed for anonymous API requests
         # this is tested in test_anonymous_published.
         uuid = str(uuid4())
@@ -723,40 +752,14 @@
             route = "workflows"
         upload_response = self._post(route, data=data)
         if assert_ok:
             self._assert_status_code_is(upload_response, 200)
             self._assert_user_has_workflow_with_name(name)
         return upload_response
 
-    def test_get_tool_predictions(self):
-        request = {
-            "tool_sequence": "Cut1",
-            "remote_model_url": "https://github.com/galaxyproject/galaxy-test-data/raw/master/tool_recommendation_model.hdf5",
-        }
-        actual_recommendations = ["Filter1", "cat1", "addValue", "comp1", "Grep1"]
-        route = "workflows/get_tool_predictions"
-        response = self._post(route, data=request)
-        recommendation_response = response.json()
-        is_empty = bool(recommendation_response["current_tool"])
-        if is_empty is False:
-            self._assert_status_code_is(response, 400)
-        else:
-            # check Ok response from the API
-            self._assert_status_code_is(response, 200)
-            recommendation_response = response.json()
-            # check the input tool sequence
-            assert recommendation_response["current_tool"] == request["tool_sequence"]
-            # check non-empty predictions list
-            predicted_tools = recommendation_response["predicted_data"]["children"]
-            assert len(predicted_tools) > 0
-            # check for the correct predictions
-            for tool in predicted_tools:
-                assert tool["tool_id"] in actual_recommendations
-                break
-
     def test_update(self):
         original_workflow = self.workflow_populator.load_workflow(name="test_import")
         uuids = {}
         labels = {}
 
         for order_index, step_dict in original_workflow["steps"].items():
             uuid = str(uuid4())
@@ -766,16 +769,16 @@
             step_dict["label"] = label
             labels[order_index] = label
 
         def check_label_and_uuid(order_index, step_dict):
             assert order_index in uuids
             assert order_index in labels
 
-            self.assertEqual(uuids[order_index], step_dict["uuid"])
-            self.assertEqual(labels[order_index], step_dict["label"])
+            assert uuids[order_index] == step_dict["uuid"]
+            assert labels[order_index] == step_dict["label"]
 
         upload_response = self.__test_upload(workflow=original_workflow)
         workflow_id = upload_response.json()["id"]
 
         def update(workflow_object):
             put_response = self._update_workflow(workflow_id, workflow_object)
             self._assert_status_code_is(put_response, 200)
@@ -1027,15 +1030,14 @@
         assert (
             workflow.get("source_metadata").get("url") == url
         )  # disappearance of source_metadata on modification is tested in test_trs_import
 
     def test_base64_import(self):
         base64_url = "base64://" + base64.b64encode(workflow_str.encode("utf-8")).decode("utf-8")
         response = self._post("workflows", data={"archive_source": base64_url})
-        print(response.content)
         response.raise_for_status()
         workflow_id = response.json()["id"]
         workflow = self._download_workflow(workflow_id)
         assert "TestWorkflow1" in workflow["name"]
 
     def test_trs_import(self):
         trs_payload = {
@@ -1045,14 +1047,79 @@
             "trs_version_id": "master",
         }
         workflow_id = self._post("workflows", data=trs_payload).json()["id"]
         original_workflow = self._download_workflow(workflow_id)
         assert "Test Workflow" in original_workflow["name"]
         assert original_workflow.get("source_metadata").get("trs_tool_id") == trs_payload["trs_tool_id"]
         assert original_workflow.get("source_metadata").get("trs_version_id") == trs_payload["trs_version_id"]
+        assert original_workflow.get("source_metadata").get("trs_server") == "dockstore"
+
+        # refactor workflow and check that the trs id is removed
+        actions = [
+            {"action_type": "update_step_label", "step": {"order_index": 0}, "label": "new_label"},
+        ]
+        self.workflow_populator.refactor_workflow(workflow_id, actions)
+        refactored_workflow = self._download_workflow(workflow_id)
+        assert refactored_workflow.get("source_metadata") is None
+
+        # reupload original_workflow and check that the trs id is removed
+        reuploaded_workflow_id = self.workflow_populator.create_workflow(original_workflow)
+        reuploaded_workflow = self._download_workflow(reuploaded_workflow_id)
+        assert reuploaded_workflow.get("source_metadata") is None
+
+    def test_trs_import_from_dockstore_trs_url(self):
+        trs_payload = {
+            "archive_source": "trs_tool",
+            "trs_url": "https://dockstore.org/api/ga4gh/trs/v2/tools/"
+            "%23workflow%2Fgithub.com%2Fjmchilton%2Fgalaxy-workflow-dockstore-example-1%2Fmycoolworkflow/"
+            "versions/master",
+        }
+        workflow_id = self._post("workflows", data=trs_payload).json()["id"]
+        original_workflow = self._download_workflow(workflow_id)
+        assert "Test Workflow" in original_workflow["name"]
+        assert (
+            original_workflow.get("source_metadata").get("trs_tool_id")
+            == "#workflow/github.com/jmchilton/galaxy-workflow-dockstore-example-1/mycoolworkflow"
+        )
+        assert original_workflow.get("source_metadata").get("trs_version_id") == "master"
+        assert original_workflow.get("source_metadata").get("trs_server") == ""
+        assert original_workflow.get("source_metadata").get("trs_url") == (
+            "https://dockstore.org/api/ga4gh/trs/v2/tools/"
+            "%23workflow%2Fgithub.com%2Fjmchilton%2Fgalaxy-workflow-dockstore-example-1%2Fmycoolworkflow/"
+            "versions/master"
+        )
+
+        # refactor workflow and check that the trs id is removed
+        actions = [
+            {"action_type": "update_step_label", "step": {"order_index": 0}, "label": "new_label"},
+        ]
+        self.workflow_populator.refactor_workflow(workflow_id, actions)
+        refactored_workflow = self._download_workflow(workflow_id)
+        assert refactored_workflow.get("source_metadata") is None
+
+        # reupload original_workflow and check that the trs id is removed
+        reuploaded_workflow_id = self.workflow_populator.create_workflow(original_workflow)
+        reuploaded_workflow = self._download_workflow(reuploaded_workflow_id)
+        assert reuploaded_workflow.get("source_metadata") is None
+
+    def test_trs_import_from_workflowhub_trs_url(self):
+        trs_payload = {
+            "archive_source": "trs_tool",
+            "trs_url": "https://workflowhub.eu/ga4gh/trs/v2/tools/109/versions/5",
+        }
+        workflow_id = self._post("workflows", data=trs_payload).json()["id"]
+        original_workflow = self._download_workflow(workflow_id)
+        assert "COVID-19: variation analysis reporting" in original_workflow["name"]
+        assert original_workflow.get("source_metadata").get("trs_tool_id") == "109"
+        assert original_workflow.get("source_metadata").get("trs_version_id") == "5"
+        assert original_workflow.get("source_metadata").get("trs_server") == ""
+        assert (
+            original_workflow.get("source_metadata").get("trs_url")
+            == "https://workflowhub.eu/ga4gh/trs/v2/tools/109/versions/5"
+        )
 
         # refactor workflow and check that the trs id is removed
         actions = [
             {"action_type": "update_step_label", "step": {"order_index": 0}, "label": "new_label"},
         ]
         self.workflow_populator.refactor_workflow(workflow_id, actions)
         refactored_workflow = self._download_workflow(workflow_id)
@@ -1070,22 +1137,23 @@
             else:
                 index_url = "workflows"
             workflows_url = self._api_url(index_url)
             response = get(workflows_url)
             response.raise_for_status()
             return response.json()
 
+        workflow_name = f"test published example {uuid4()}"
         names = [w["name"] for w in anonymous_published_workflows(True)]
-        assert "test published example" not in names
-        workflow_id = self.workflow_populator.simple_workflow("test published example", publish=True)
+        assert workflow_name not in names
+        workflow_id = self.workflow_populator.simple_workflow(workflow_name, publish=True)
 
         for explicit_query_parameter in [True, False]:
             workflow_index = anonymous_published_workflows(explicit_query_parameter)
             names = [w["name"] for w in workflow_index]
-            assert "test published example" in names
+            assert workflow_name in names
             ids = [w["id"] for w in workflow_index]
             assert workflow_id in ids
 
     def test_import_published(self):
         workflow_id = self.workflow_populator.simple_workflow("test_import_published", publish=True)
         with self._different_user():
             other_import_response = self.__import_workflow(workflow_id, deprecated_route=True)
@@ -1345,15 +1413,15 @@
         invocation = self._invocation_details(workflow_id, invocation_id)
         assert invocation["state"] == "scheduled", invocation
 
     @skip_without_tool("collection_creates_pair")
     def test_workflow_run_output_collections(self) -> None:
         with self.dataset_populator.test_history() as history_id:
             self._run_workflow(WORKFLOW_WITH_OUTPUT_COLLECTION, history_id=history_id)
-            self.assertEqual("a\nc\nb\nd\n", self.dataset_populator.get_history_dataset_content(history_id, hid=0))
+            assert "a\nc\nb\nd\n" == self.dataset_populator.get_history_dataset_content(history_id, hid=0)
 
     @skip_without_tool("job_properties")
     @skip_without_tool("identifier_multiple_in_conditional")
     def test_workflow_resume_from_failed_step(self):
         workflow_id = self._upload_yaml_workflow(
             """
 class: GalaxyWorkflow
@@ -1498,22 +1566,22 @@
         type: File
 """,
                 history_id=history_id,
                 assert_ok=False,
                 wait=True,
             )
             history_contents = self.dataset_populator._get_contents_request(history_id=history_id).json()
-            first_input = history_contents[1]
-            assert first_input["history_content_type"] == "dataset"
+            input_collection = self.dataset_populator.get_history_collection_details(history_id, hid=1, assert_ok=False)
+            first_input = input_collection["elements"][0]
             paused_dataset = history_contents[-1]
             failed_dataset = self.dataset_populator.get_history_dataset_details(history_id, hid=5, assert_ok=False)
             assert paused_dataset["state"] == "paused", paused_dataset
             assert failed_dataset["state"] == "error", failed_dataset
             inputs = {
-                "input1": {"values": [{"src": "hda", "id": first_input["id"]}]},
+                "input1": {"values": [{"src": "dce", "id": first_input["id"]}]},
                 "failbool": "false",
                 "rerun_remap_job_id": failed_dataset["creating_job"],
             }
             run_dict = self.dataset_populator.run_tool(
                 tool_id="fail_identifier",
                 inputs=inputs,
                 history_id=history_id,
@@ -1556,16 +1624,14 @@
     collection_type: "list:list:paired"
 """,
                 history_id=history_id,
                 assert_ok=False,
                 wait=True,
             )
             invocation = self.workflow_populator.get_invocation(job_summary.invocation_id, step_details=True)
-            # TODO: return steps sorted by order_index ? Why don't we do that ??
-            invocation["steps"].sort(key=lambda step: step["order_index"])
             failed_step = invocation["steps"][1]
             assert failed_step["jobs"][0]["state"] == "error"
             failed_hdca_id = failed_step["output_collections"]["list_output"]["id"]
             failed_hdca = self.dataset_populator.get_history_collection_details(
                 history_id=history_id, content_id=failed_hdca_id, assert_ok=False
             )
             assert (
@@ -1640,28 +1706,26 @@
             hdca1 = self.dataset_collection_populator.wait_for_fetched_collection(fetch_response)
             self.dataset_populator.wait_for_history(history_id, assert_ok=True)
             inputs = {
                 "0": self._ds_entry(hdca1),
             }
             invocation_id = self.__invoke_workflow(workflow_id, inputs=inputs, history_id=history_id)
             self.workflow_populator.wait_for_invocation_and_jobs(history_id, workflow_id, invocation_id)
-            self.assertEqual(
-                "a\nc\nb\nd\ne\ng\nf\nh\n", self.dataset_populator.get_history_dataset_content(history_id, hid=0)
-            )
+            assert "a\nc\nb\nd\ne\ng\nf\nh\n" == self.dataset_populator.get_history_dataset_content(history_id, hid=0)
 
     @skip_without_tool("cat_list")
     @skip_without_tool("collection_split_on_column")
     def test_workflow_run_dynamic_output_collections(self):
         with self.dataset_populator.test_history() as history_id:
             self._run_jobs(WORKFLOW_WITH_DYNAMIC_OUTPUT_COLLECTION, history_id=history_id, assert_ok=True, wait=True)
             details = self.dataset_populator.get_history_dataset_details(history_id, hid=0)
             last_item_hid = details["hid"]
             assert last_item_hid == 7, f"Expected 7 history items, got {last_item_hid}"
             content = self.dataset_populator.get_history_dataset_content(history_id, hid=0)
-            self.assertEqual("10.0\n30.0\n20.0\n40.0\n", content)
+            assert "10.0\n30.0\n20.0\n40.0\n" == content
 
     @skip_without_tool("collection_split_on_column")
     @skip_without_tool("min_repeat")
     def test_workflow_run_dynamic_output_collections_2(self):
         # A more advanced output collection workflow, testing regression of
         # https://github.com/galaxyproject/galaxy/issues/776
         with self.dataset_populator.test_history() as history_id:
@@ -1694,15 +1758,15 @@
                 "2": self._ds_entry(hda3),
             }
             invocation_id = self.__invoke_workflow(workflow_id, inputs=inputs, history_id=history_id)
             self.workflow_populator.wait_for_invocation_and_jobs(history_id, workflow_id, invocation_id)
             collection_details = self.dataset_populator.get_history_collection_details(history_id, hid=7)
             assert collection_details["populated_state"] == "ok"
             content = self.dataset_populator.get_history_dataset_content(history_id, hid=11)
-            self.assertEqual(content.strip(), "samp1\t10.0\nsamp2\t20.0")
+            assert content.strip() == "samp1\t10.0\nsamp2\t20.0"
 
     @skip_without_tool("cat")
     @skip_without_tool("collection_split_on_column")
     def test_workflow_run_dynamic_output_collections_3(self):
         # Test a workflow that create a list:list:list followed by a mapping step.
         with self.dataset_populator.test_history() as history_id:
             workflow_id = self._upload_yaml_workflow(
@@ -1869,47 +1933,468 @@
   reference:
     value: 1.fasta
     type: File
 """,
                 history_id=history_id,
             )
 
+    def test_run_workflow_simple_conditional_step(self):
+        with self.dataset_populator.test_history() as history_id:
+            summary = self._run_workflow(
+                """class: GalaxyWorkflow
+inputs:
+  should_run:
+    type: boolean
+  some_file:
+    type: data
+steps:
+  cat1:
+    tool_id: cat1
+    in:
+      input1: some_file
+      should_run: should_run
+    when: $(inputs.should_run)
+""",
+                test_data="""
+some_file:
+  value: 1.bed
+  type: File
+should_run:
+  value: false
+  type: raw
+""",
+                history_id=history_id,
+            )
+            invocation_details = self.workflow_populator.get_invocation(summary.invocation_id, step_details=True)
+            for step in invocation_details["steps"]:
+                if step["workflow_step_label"] == "cat1":
+                    assert sum(1 for j in step["jobs"] if j["state"] == "skipped") == 1
+
+    def test_run_workflow_invalid_when_expression(self):
+        with self.dataset_populator.test_history() as history_id:
+            summary = self._run_workflow(
+                """class: GalaxyWorkflow
+inputs:
+  should_run:
+    type: boolean
+  some_file:
+    type: data
+steps:
+  cat1:
+    tool_id: cat1
+    in:
+      input1: some_file
+      should_run: should_run
+    when: $(:syntaxError:)
+""",
+                test_data="""
+some_file:
+  value: 1.bed
+  type: File
+should_run:
+  value: false
+  type: raw
+""",
+                history_id=history_id,
+                wait=True,
+                assert_ok=False,
+            )
+            invocation_details = self.workflow_populator.get_invocation(summary.invocation_id, step_details=True)
+            assert invocation_details["state"] == "failed"
+            assert len(invocation_details["messages"]) == 1
+            message = invocation_details["messages"][0]
+            assert message["reason"] == "expression_evaluation_failed"
+
+    def test_run_workflow_fails_when_expression_not_boolean(self):
+        with self.dataset_populator.test_history() as history_id:
+            summary = self._run_workflow(
+                """class: GalaxyWorkflow
+inputs:
+  should_run:
+    type: boolean
+  some_file:
+    type: data
+steps:
+  cat1:
+    tool_id: cat1
+    in:
+      input1: some_file
+      should_run: should_run
+    when: $("false")
+""",
+                test_data="""
+some_file:
+  value: 1.bed
+  type: File
+should_run:
+  value: false
+  type: raw
+""",
+                history_id=history_id,
+                wait=True,
+                assert_ok=False,
+            )
+            invocation_details = self.workflow_populator.get_invocation(summary.invocation_id, step_details=True)
+            assert invocation_details["state"] == "failed"
+            assert len(invocation_details["messages"]) == 1
+            message = invocation_details["messages"][0]
+            assert message["reason"] == "when_not_boolean"
+            assert message["details"] == "Type is: str"
+            assert message["workflow_step_id"] == 2
+
+    def test_run_workflow_subworkflow_conditional_step(self):
+        with self.dataset_populator.test_history() as history_id:
+            summary = self._run_workflow(
+                """class: GalaxyWorkflow
+inputs:
+  should_run:
+    type: boolean
+  some_file:
+    type: data
+steps:
+  subworkflow:
+    run:
+      class: GalaxyWorkflow
+      inputs:
+        some_file:
+          type: data
+        should_run:
+          type: boolean
+      steps:
+        a_tool_step:
+          tool_id: cat1
+          in:
+            input1: some_file
+    in:
+      some_file: some_file
+      should_run: should_run
+    outputs:
+      inner_out: a_tool_step/out_file1
+    when: $(inputs.should_run)
+outputs:
+  outer_output:
+    outputSource: subworkflow/inner_out
+""",
+                test_data="""
+some_file:
+  value: 1.bed
+  type: File
+should_run:
+  value: false
+  type: raw
+""",
+                history_id=history_id,
+                wait=True,
+                assert_ok=True,
+            )
+            invocation_details = self.workflow_populator.get_invocation(summary.invocation_id, step_details=True)
+            subworkflow_invocation_id = invocation_details["steps"][-1]["subworkflow_invocation_id"]
+            self.workflow_populator.wait_for_invocation_and_jobs(
+                history_id=history_id, workflow_id="whatever", invocation_id=subworkflow_invocation_id
+            )
+            invocation_details = self.workflow_populator.get_invocation(subworkflow_invocation_id, step_details=True)
+            for step in invocation_details["steps"]:
+                if step["workflow_step_label"] == "a_tool_step":
+                    assert sum(1 for j in step["jobs"] if j["state"] == "skipped") == 1
+
+    def test_run_workflow_conditional_step_map_over_expression_tool(self):
+        with self.dataset_populator.test_history() as history_id:
+            summary = self._run_workflow(
+                """
+class: GalaxyWorkflow
+inputs:
+  boolean_input_files: collection
+steps:
+- label: param_out
+  tool_id: param_value_from_file
+  in:
+     input1: boolean_input_files
+  state:
+    param_type: boolean
+- label: consume_expression_parameter
+  tool_id: cat1
+  in:
+    input1: boolean_input_files
+    should_run: param_out/boolean_param
+  out:
+    out_file1:
+      change_datatype: txt
+  when: $(inputs.should_run)
+test_data:
+  boolean_input_files:
+    collection_type: list
+    elements:
+      - identifier: true
+        content: true
+      - identifier: false
+        content: false
+""",
+                history_id=history_id,
+            )
+            invocation_details = self.workflow_populator.get_invocation(summary.invocation_id, step_details=True)
+            for step in invocation_details["steps"]:
+                if step["workflow_step_label"] == "consume_expression_parameter":
+                    skipped_jobs = [j for j in step["jobs"] if j["state"] == "skipped"]
+                    assert len(skipped_jobs) == 1
+                    # also assert that change_datatype was ignored for null output
+                    job_details = self.dataset_populator.get_job_details(skipped_jobs[0]["id"], full=True).json()
+                    skipped_hda_id = job_details["outputs"]["out_file1"]["id"]
+                    dataset_details = self.dataset_populator.get_history_dataset_details(
+                        history_id=history_id, content_id=skipped_hda_id
+                    )
+                    assert dataset_details["file_ext"] == "expression.json", dataset_details
+
+    def test_run_workflow_conditional_subworkflow_step_map_over_expression_tool(self):
+        with self.dataset_populator.test_history() as history_id:
+            summary = self._run_workflow(
+                """
+class: GalaxyWorkflow
+inputs:
+  boolean_input_files: collection
+steps:
+  create_list_of_boolean:
+    tool_id: param_value_from_file
+    in:
+       input1: boolean_input_files
+    state:
+      param_type: boolean
+  subworkflow:
+    run:
+      class: GalaxyWorkflow
+      inputs:
+        boolean_input_file: data
+        should_run: boolean
+      steps:
+        consume_expression_parameter:
+          tool_id: cat1
+          in:
+            input1: boolean_input_file
+          out:
+            out_file1:
+              change_datatype: txt
+      outputs:
+        inner_output:
+          outputSource: consume_expression_parameter/out_file1
+    in:
+      boolean_input_file: boolean_input_files
+      should_run: create_list_of_boolean/boolean_param
+    when: $(inputs.should_run)
+outputs:
+  outer_output:
+    outputSource: subworkflow/inner_output
+test_data:
+  boolean_input_files:
+    collection_type: list
+    elements:
+      - identifier: true
+        content: true
+      - identifier: false
+        content: false
+""",
+                history_id=history_id,
+            )
+            invocation_details = self.workflow_populator.get_invocation(summary.invocation_id, step_details=True)
+            assert "outer_output" in invocation_details["output_collections"]
+            outer_output = invocation_details["output_collections"]["outer_output"]
+            outer_hdca = self.dataset_populator.get_history_collection_details(
+                history_id, content_id=outer_output["id"]
+            )
+            assert outer_hdca["job_state_summary"]["all_jobs"] == 2
+            assert outer_hdca["job_state_summary"]["ok"] == 1
+            assert outer_hdca["job_state_summary"]["skipped"] == 1
+
+    def test_run_workflow_conditional_subworkflow_step_map_over_expression_tool_with_extra_nesting(self):
+        with self.dataset_populator.test_history() as history_id:
+            summary = self._run_workflow(
+                NESTED_WORKFLOW_WITH_CONDITIONAL_SUBWORKFLOW_AND_DISCONNECTED_MAP_OVER_SOURCE,
+                test_data="""boolean_input_files:
+  collection_type: list
+  elements:
+    - identifier: true
+      content: true
+    - identifier: false
+      content: false
+""",
+                history_id=history_id,
+            )
+            invocation_details = self.workflow_populator.get_invocation(summary.invocation_id, step_details=True)
+            outer_create_nested_id = invocation_details["output_collections"]["outer_create_nested"]["id"]
+            outer_create_nested = self.dataset_populator.get_history_collection_details(
+                history_id, content_id=outer_create_nested_id
+            )
+            assert outer_create_nested["job_state_summary"]["all_jobs"] == 2
+            assert outer_create_nested["job_state_summary"]["ok"] == 1
+            assert outer_create_nested["job_state_summary"]["skipped"] == 1
+
+            for cat1_output in ["outer_output_1", "outer_output_2"]:
+                outer_output = invocation_details["output_collections"][cat1_output]
+                outer_hdca = self.dataset_populator.get_history_collection_details(
+                    history_id, content_id=outer_output["id"]
+                )
+                # You might expect 12 total jobs, 6 ok and 6 skipped,
+                # but because we're not actually running one branch of collection_creates_dynamic_nested
+                # there's no input to consume_expression_parameter.
+                # It's unclear if that's a problem or not ... probably not a major one,
+                # since we keep producing "empty" outer collections, which seems somewhat correct.
+                assert outer_hdca["job_state_summary"]["all_jobs"] == 6
+                assert outer_hdca["job_state_summary"]["ok"] == 6
+                assert outer_hdca["collection_type"] == "list:list:list"
+                elements = outer_hdca["elements"]
+                assert elements[0]["element_identifier"] == "True"
+                assert elements[0]["object"]["element_count"] == 3
+                assert elements[1]["element_identifier"] == "False"
+                assert elements[1]["object"]["element_count"] == 0
+
+    def test_run_workflow_conditional_subworkflow_step_map_over_expression_tool_with_extra_nesting_skip_all(self):
+        with self.dataset_populator.test_history() as history_id:
+            summary = self._run_workflow(
+                NESTED_WORKFLOW_WITH_CONDITIONAL_SUBWORKFLOW_AND_DISCONNECTED_MAP_OVER_SOURCE,
+                test_data="""boolean_input_files:
+  collection_type: list
+  elements:
+    - identifier: false
+      content: false
+    - identifier: also_false
+      content: false
+""",
+                history_id=history_id,
+            )
+            invocation_details = self.workflow_populator.get_invocation(summary.invocation_id, step_details=True)
+            outer_create_nested_id = invocation_details["output_collections"]["outer_create_nested"]["id"]
+            outer_create_nested = self.dataset_populator.get_history_collection_details(
+                history_id, content_id=outer_create_nested_id
+            )
+            assert outer_create_nested["job_state_summary"]["all_jobs"] == 2
+            assert outer_create_nested["job_state_summary"]["skipped"] == 2
+
+            for cat1_output in ["outer_output_1", "outer_output_2"]:
+                outer_output = invocation_details["output_collections"][cat1_output]
+                outer_hdca = self.dataset_populator.get_history_collection_details(
+                    history_id, content_id=outer_output["id"]
+                )
+                assert outer_hdca["job_state_summary"]["all_jobs"] == 0
+                assert outer_hdca["collection_type"] == "list:list:list"
+
+    def test_run_workflow_conditional_step_map_over_expression_tool_pick_value(self):
+        with self.dataset_populator.test_history() as history_id:
+            summary = self._run_workflow(
+                """
+class: GalaxyWorkflow
+inputs:
+  boolean_input_files_1: collection
+  boolean_input_files_2: collection
+outputs:
+  my_output:
+    outputSource: pick_value/data_param
+steps:
+- label: param_out_1
+  tool_id: param_value_from_file
+  in:
+     input1: boolean_input_files_1
+  state:
+    param_type: boolean
+- label: param_out_2
+  tool_id: param_value_from_file
+  in:
+     input1: boolean_input_files_2
+  state:
+    param_type: boolean
+- label: consume_expression_parameter_1
+  tool_id: cat1
+  in:
+    input1: boolean_input_files_1
+    should_run: param_out_1/boolean_param
+  when: $(inputs.should_run)
+- label: consume_expression_parameter_2
+  tool_id: cat1
+  in:
+    input1: boolean_input_files_2
+    should_run: param_out_2/boolean_param
+  when: $(inputs.should_run)
+- label: pick_value
+  tool_id: pick_value
+  tool_state:
+    style_cond:
+      __current_case__: 2
+      pick_style: first_or_error
+      type_cond:
+        __current_case__: 4
+        param_type: data
+        pick_from:
+        - __index__: 0
+          value:
+            __class__: RuntimeValue
+        - __index__: 1
+          value:
+            __class__: RuntimeValue
+  in:
+    style_cond|type_cond|pick_from_0|value:
+      source: consume_expression_parameter_1/out_file1
+    style_cond|type_cond|pick_from_1|value:
+      source: consume_expression_parameter_2/out_file1
+test_data:
+  boolean_input_files_1:
+    collection_type: list
+    elements:
+      - identifier: true
+        content: true
+      - identifier: false
+        content: false
+  boolean_input_files_2:
+    collection_type: list
+    elements:
+      - identifier: false
+        content: false
+      - identifier: true
+        content: true
+""",
+                history_id=history_id,
+            )
+            invocation_details = self.workflow_populator.get_invocation(summary.invocation_id, step_details=True)
+            output_collection_id = invocation_details["output_collections"]["my_output"]["id"]
+            hdca_details = self.dataset_populator.get_history_collection_details(
+                history_id=history_id, content_id=output_collection_id
+            )
+            elements = hdca_details["elements"]
+            assert len(elements) == 2
+            for element in elements:
+                content = self.dataset_populator.get_history_dataset_content(
+                    history_id, content_id=element["object"]["id"]
+                )
+                assert content == "True"
+            for step in invocation_details["steps"]:
+                if step["workflow_step_label"].startswith("consume_expression_parameter_"):
+                    assert sum(1 for j in step["jobs"] if j["state"] == "skipped") == 1
+
     def test_run_subworkflow_simple(self) -> None:
         with self.dataset_populator.test_history() as history_id:
             summary = self._run_workflow(
                 WORKFLOW_NESTED_SIMPLE,
                 test_data="""
 outer_input:
   value: 1.bed
   type: File
 """,
                 history_id=history_id,
             )
             invocation_id = summary.invocation_id
 
             content = self.dataset_populator.get_history_dataset_content(history_id)
-            self.assertEqual(
-                "chrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\nchrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n",
-                content,
+            assert (
+                content
+                == "chrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\nchrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n"
             )
             steps = self.workflow_populator.get_invocation(invocation_id)["steps"]
             assert sum(1 for step in steps if step["subworkflow_invocation_id"] is None) == 3
             subworkflow_invocation_id = [
                 step["subworkflow_invocation_id"] for step in steps if step["subworkflow_invocation_id"]
             ][0]
             subworkflow_invocation = self.workflow_populator.get_invocation(subworkflow_invocation_id)
-            assert [step for step in subworkflow_invocation["steps"] if step["order_index"] == 0][0][
-                "workflow_step_label"
-            ] == "inner_input"
-            assert [step for step in subworkflow_invocation["steps"] if step["order_index"] == 1][0][
-                "workflow_step_label"
-            ] == "random_lines"
-
-            bco = self.workflow_populator.get_biocompute_object(invocation_id)
-            self.workflow_populator.validate_biocompute_object(bco)
+            assert subworkflow_invocation["steps"][0]["workflow_step_label"] == "inner_input"
+            assert subworkflow_invocation["steps"][1]["workflow_step_label"] == "random_lines"
 
     @skip_without_tool("random_lines1")
     def test_run_subworkflow_runtime_parameters(self):
         with self.dataset_populator.test_history() as history_id:
             self._run_jobs(
                 WORKFLOW_NESTED_RUNTIME_PARAMETER,
                 test_data="""
@@ -2032,20 +2517,21 @@
                 test_data = """
         outer_input:
           value: 1.bed
           type: File
         """
                 summary = self._run_workflow(workflow_text, test_data=test_data, history_id=history_id)
                 jobs = summary.jobs
-                assert len(jobs) == 4, "4 jobs expected, got %d jobs" % len(jobs)
+                num_jobs = len(jobs)
+                assert num_jobs == 2, f"2 jobs expected, got {num_jobs} jobs"
 
                 content = self.dataset_populator.get_history_dataset_content(history_id)
-                self.assertEqual(
-                    "chrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\nchrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n",
-                    content,
+                assert (
+                    content
+                    == "chrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\nchrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n"
                 )
 
         run_test(NESTED_WORKFLOW_AUTO_LABELS_MODERN_SYNTAX)
 
     @skip_without_tool("cat1")
     @skip_without_tool("collection_paired_test")
     def test_workflow_run_zip_collections(self):
@@ -2078,15 +2564,15 @@
             inputs = {
                 "0": self._ds_entry(hda1),
                 "1": self._ds_entry(hda2),
             }
             invocation_id = self.__invoke_workflow(workflow_id, inputs=inputs, history_id=history_id)
             self.workflow_populator.wait_for_invocation_and_jobs(history_id, workflow_id, invocation_id)
             content = self.dataset_populator.get_history_dataset_content(history_id)
-            self.assertEqual(content.strip(), "samp1\t10.0\nsamp2\t20.0\nsamp1\t20.0\nsamp2\t40.0")
+            assert content.strip() == "samp1\t10.0\nsamp2\t20.0\nsamp1\t20.0\nsamp2\t40.0"
 
     @skip_without_tool("collection_paired_test")
     def test_workflow_flatten(self):
         with self.dataset_populator.test_history() as history_id:
             self._run_jobs(
                 """
 class: GalaxyWorkflow
@@ -2212,15 +2698,152 @@
     @skip_without_tool("cat1")
     def test_export_invocation_bco(self):
         with self.dataset_populator.test_history() as history_id:
             summary = self._run_workflow(WORKFLOW_SIMPLE, test_data={"input1": "hello world"}, history_id=history_id)
             invocation_id = summary.invocation_id
             bco = self.workflow_populator.get_biocompute_object(invocation_id)
             self.workflow_populator.validate_biocompute_object(bco)
-            self.assertEqual(bco["provenance_domain"]["name"], "Simple Workflow")
+            assert bco["provenance_domain"]["name"] == "Simple Workflow"
+
+    @skip_without_tool("cat1")
+    def test_export_invocation_ro_crate(self):
+        with self.dataset_populator.test_history() as history_id:
+            summary = self._run_workflow(WORKFLOW_SIMPLE, test_data={"input1": "hello world"}, history_id=history_id)
+            invocation_id = summary.invocation_id
+            crate = self.workflow_populator.get_ro_crate(invocation_id, include_files=True)
+            workflow = crate.mainEntity
+            assert workflow
+
+    @skip_without_tool("__MERGE_COLLECTION__")
+    @skip_without_tool("cat_collection")
+    @skip_without_tool("head")
+    def test_export_invocation_ro_crate_adv(self):
+        with self.dataset_populator.test_history() as history_id:
+            summary = self._run_workflow(
+                """
+class: GalaxyWorkflow
+inputs:
+  input collection 1:
+    type: collection
+    collection_type: list
+    optional: false
+  input collection 2:
+    type: collection
+    collection_type: list
+    optional: false
+  num_lines_param:
+    type: int
+    optional: false
+    default: 2
+outputs:
+  _anonymous_output_1:
+    outputSource: num_lines_param
+  output_collection:
+    outputSource: merge collections tool
+  concatenated_collection:
+    outputSource: concat collection/out_file1
+  output:
+    outputSource: select lines/out_file1
+steps:
+  merge collections tool:
+    tool_id: __MERGE_COLLECTION__
+    tool_version: 1.0.0
+    tool_state:
+      advanced:
+        conflict:
+          __current_case__: 0
+          duplicate_options: keep_first
+      inputs:
+      - __index__: 0
+        input:
+          __class__: ConnectedValue
+      - __index__: 1
+        input:
+          __class__: ConnectedValue
+    in:
+      inputs_1|input:
+        source: input collection 2
+      inputs_0|input:
+        source: input collection 1
+  concat collection:
+    tool_id: cat_collection
+    tool_state:
+      input1:
+        __class__: RuntimeValue
+    in:
+      input1:
+        source: merge collections tool
+  select lines:
+    tool_id: head
+    tool_state:
+      input:
+        __class__: RuntimeValue
+      lineNum:
+        __class__: ConnectedValue
+    in:
+      lineNum:
+        source: num_lines_param
+      input:
+        source: concat collection/out_file1
+""",
+                test_data="""
+num_lines_param:
+  type: int
+  value: 2
+input collection 1:
+  collection_type: list
+  elements:
+    - identifier: el1
+      value: 1.fastq
+      type: File
+    - identifier: el2
+      value: 1.fastq
+      type: File
+input collection 2:
+  collection_type: list
+  elements:
+    - identifier: el1
+      value: 1.fastq
+      type: File
+    - identifier: el2
+      value: 1.fastq
+      type: File
+""",
+                history_id=history_id,
+                wait=True,
+            )
+            invocation_id = summary.invocation_id
+            crate = self.workflow_populator.get_ro_crate(invocation_id, include_files=True)
+            workflow = crate.mainEntity
+            root = crate.root_dataset
+            assert len(root["mentions"]) == 4
+            actions = [_ for _ in crate.contextual_entities if "CreateAction" in _.type]
+            assert len(actions) == 1
+            wf_action = actions[0]
+            wf_objects = wf_action["object"]
+            assert len(workflow["input"]) == 3
+            assert len(workflow["output"]) == 3
+            collections = [_ for _ in crate.contextual_entities if "Collection" in _.type]
+            assert len(collections) == 3
+            collection = collections[0]
+            assert (
+                collection["additionalType"]
+                == "https://training.galaxyproject.org/training-material/faqs/galaxy/collections_build_list.html"
+            )
+            assert collection.type == "Collection"
+            assert len(collection["hasPart"]) == 2
+            assert collection in wf_objects
+
+            coll_dataset = collection["hasPart"][0].id
+            assert coll_dataset in [_.id for _ in collections[2]["hasPart"]]
+            property_values = [_ for _ in crate.contextual_entities if "PropertyValue" in _.type]
+            assert len(property_values) == 1
+            for pv in property_values:
+                assert pv in wf_objects
+                assert pv["exampleOfWork"] in workflow["input"]
 
     @skip_without_tool("__APPLY_RULES__")
     def test_workflow_run_apply_rules(self):
         with self.dataset_populator.test_history() as history_id:
             self._run_workflow(
                 WORKFLOW_WITH_RULES_1,
                 history_id=history_id,
@@ -2272,15 +2895,14 @@
                 assert_ok=False,
             )
             jobs = summary.jobs
 
             def filter_jobs_by_tool(tool_id):
                 return [j for j in summary.jobs if j["tool_id"] == tool_id]
 
-            assert len(filter_jobs_by_tool("__DATA_FETCH__")) == 1, jobs
             assert len(filter_jobs_by_tool("exit_code_from_file")) == 2, jobs
             assert len(filter_jobs_by_tool("__FILTER_FAILED_DATASETS__")) == 1, jobs
             # Follow proves one job was filtered out of the result of cat1
             assert len(filter_jobs_by_tool("cat1")) == 1, jobs
 
     def test_workflow_request(self):
         workflow = self.workflow_populator.load_workflow(name="test_for_queue")
@@ -2613,19 +3235,19 @@
     value: 1.bed
     type: File
 """,
                 history_id=history_id,
                 wait=True,
                 round_trip_format_conversion=True,
             )
-            self.assertEqual(
-                "chr6\t108722976\t108723115\tCCDS5067.1_cds_0_0_chr6_108722977_f\t0\t+\nchrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n",
-                self.dataset_populator.get_history_dataset_content(history_id),
+            assert (
+                self.dataset_populator.get_history_dataset_content(history_id)
+                == "chr6\t108722976\t108723115\tCCDS5067.1_cds_0_0_chr6_108722977_f\t0\t+\nchrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n"
             )
-            # self.assertEqual("chr16\t142908\t143003\tCCDS10397.1_cds_0_0_chr16_142909_f\t0\t+\nchrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n", self.dataset_populator.get_history_dataset_content(history_id))
+            # assert self.dataset_populator.get_history_dataset_content(history_id) == "chr16\t142908\t143003\tCCDS10397.1_cds_0_0_chr16_142909_f\t0\t+\nchrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n"
 
     @skip_without_tool("cat_list")
     @skip_without_tool("random_lines1")
     @skip_without_tool("split")
     def test_subworkflow_recover_mapping_2(self):
         # Like the above test case, this test case tests an outer workflow continues to
         # schedule and handle collection mapping properly after a subworkflow needs to be
@@ -2684,17 +3306,17 @@
   value: 1.bed
   type: File
 """,
                 history_id=history_id,
                 wait=True,
                 round_trip_format_conversion=True,
             )
-            self.assertEqual(
-                "chr6\t108722976\t108723115\tCCDS5067.1_cds_0_0_chr6_108722977_f\t0\t+\nchrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n",
-                self.dataset_populator.get_history_dataset_content(history_id),
+            assert (
+                self.dataset_populator.get_history_dataset_content(history_id)
+                == "chr6\t108722976\t108723115\tCCDS5067.1_cds_0_0_chr6_108722977_f\t0\t+\nchrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n"
             )
 
     @skip_without_tool("cat_list")
     @skip_without_tool("random_lines1")
     @skip_without_tool("split")
     def test_recover_mapping_in_subworkflow(self):
         with self.dataset_populator.test_history() as history_id:
@@ -2745,17 +3367,17 @@
   value: 1.bed
   type: File
 """,
                 history_id=history_id,
                 wait=True,
                 round_trip_format_conversion=True,
             )
-            self.assertEqual(
-                "chr6\t108722976\t108723115\tCCDS5067.1_cds_0_0_chr6_108722977_f\t0\t+\nchrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n",
-                self.dataset_populator.get_history_dataset_content(history_id),
+            assert (
+                self.dataset_populator.get_history_dataset_content(history_id)
+                == "chr6\t108722976\t108723115\tCCDS5067.1_cds_0_0_chr6_108722977_f\t0\t+\nchrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n"
             )
 
     @skip_without_tool("empty_list")
     @skip_without_tool("count_list")
     @skip_without_tool("random_lines1")
     def test_empty_list_mapping(self):
         with self.dataset_populator.test_history() as history_id:
@@ -2790,15 +3412,74 @@
 input1:
   value: 1.bed
   type: File
 """,
                 history_id=history_id,
                 wait=True,
             )
-            self.assertEqual("0\n", self.dataset_populator.get_history_dataset_content(history_id))
+            assert "0\n" == self.dataset_populator.get_history_dataset_content(history_id)
+
+    def test_subworkflow_map_over_data_column(self):
+        with self.dataset_populator.test_history() as history_id:
+            self._run_workflow(
+                """class: GalaxyWorkflow
+inputs:
+  input:
+    collection_type: list
+outputs:
+  reduced:
+    outputSource: list:list reduction/out_file1
+steps:
+  subworkflow:
+    in:
+      input collection:
+        source: input
+      input dataset:
+        source: input
+    run:
+      class: GalaxyWorkflow
+      inputs:
+        input dataset:
+          type: data
+        input collection:
+          collection_type: list
+      outputs:
+        subworkflow_out:
+          outputSource: join out/out_file1
+      steps:
+        join out:
+          tool_id: comp1
+          tool_state:
+            field1: '1'
+            field2: '1'
+          in:
+            input1:
+              source: input dataset
+            input2:
+              source: input collection
+  list:list reduction:
+    tool_id: cat_list
+    in:
+      input1:
+        source: subworkflow/subworkflow_out
+test_data:
+  input:
+    collection_type: list
+    elements:
+      - identifier: 1
+        content: A  1
+        ext: tabular
+      - identifier: 2
+        content: B  2
+        ext: tabular
+""",
+                history_id=history_id,
+                wait=True,
+                assert_ok=True,
+            )
 
     @skip_without_tool("random_lines1")
     def test_change_datatype_collection_map_over(self):
         with self.dataset_populator.test_history() as history_id:
             jobs_summary = self._run_workflow(
                 """
 class: GalaxyWorkflow
@@ -2887,15 +3568,15 @@
   value: 1.bed
   type: File
 """,
                 history_id=history_id,
                 wait=True,
                 round_trip_format_conversion=True,
             )
-            self.assertEqual("0\n", self.dataset_populator.get_history_dataset_content(history_id))
+            assert "0\n" == self.dataset_populator.get_history_dataset_content(history_id)
 
     @skip_without_tool("cat")
     def test_cancel_new_workflow_when_history_deleted(self):
         with self.dataset_populator.test_history() as history_id:
             # Invoke a workflow with a pause step.
             uploaded_workflow_id, invocation_id = self._invoke_paused_workflow(history_id)
 
@@ -2906,14 +3587,20 @@
             # Wait for all the datasets to complete, make sure the workflow invocation
             # is not complete.
             self._assert_invocation_non_terminal(uploaded_workflow_id, invocation_id)
 
             self._delete(f"histories/{history_id}")
 
             invocation_cancelled = self._wait_for_invocation_state(uploaded_workflow_id, invocation_id, "cancelled")
+            workflow_details = self._invocation_details(uploaded_workflow_id, invocation_id)
+            assert len(workflow_details["messages"]) == 1
+            message = workflow_details["messages"][0]
+            assert message["history_id"] == history_id
+            assert message["reason"] == "history_deleted"
+
             assert invocation_cancelled, "Workflow state is not cancelled..."
 
     @skip_without_tool("cat")
     def test_cancel_ready_workflow_when_history_deleted(self):
         # Same as previous test but make sure invocation isn't a new state before
         # cancelling.
         with self.dataset_populator.test_history() as history_id:
@@ -2927,14 +3614,19 @@
             # is not complete.
             self._assert_invocation_non_terminal(uploaded_workflow_id, invocation_id)
 
             self._delete(f"histories/{history_id}")
 
             invocation_cancelled = self._wait_for_invocation_state(uploaded_workflow_id, invocation_id, "cancelled")
             assert invocation_cancelled, "Workflow state is not cancelled..."
+            workflow_details = self._invocation_details(uploaded_workflow_id, invocation_id)
+            assert len(workflow_details["messages"]) == 1
+            message = workflow_details["messages"][0]
+            assert message["history_id"] == history_id
+            assert message["reason"] == "history_deleted"
 
     @skip_without_tool("cat")
     def test_workflow_pause(self):
         with self.dataset_populator.test_history() as history_id:
             # Invoke a workflow with a pause step.
             uploaded_workflow_id, invocation_id = self._invoke_paused_workflow(history_id)
 
@@ -2974,14 +3666,19 @@
             self._assert_invocation_non_terminal(uploaded_workflow_id, invocation_id)
 
             # Review the paused workflow and cancel it at the paused step.
             self.__review_paused_steps(uploaded_workflow_id, invocation_id, order_index=2, action=False)
 
             # Ensure the workflow eventually becomes cancelled.
             invocation_cancelled = self._wait_for_invocation_state(uploaded_workflow_id, invocation_id, "cancelled")
+            workflow_details = self._invocation_details(uploaded_workflow_id, invocation_id)
+            assert len(workflow_details["messages"]) == 1
+            message = workflow_details["messages"][0]
+            assert "workflow_step_id" in message
+            assert message["reason"] == "cancelled_on_review"
             assert invocation_cancelled, "Workflow state is not cancelled..."
 
     @skip_without_tool("head")
     def test_workflow_map_reduce_pause(self):
         with self.dataset_populator.test_history() as history_id:
             workflow = self.workflow_populator.load_workflow_from_resource("test_workflow_map_reduce_pause")
             uploaded_workflow_id = self.workflow_populator.create_workflow(workflow)
@@ -3006,17 +3703,15 @@
             # are at the pause step in this case then.
             self._assert_invocation_non_terminal(uploaded_workflow_id, invocation_id)
 
             self.__review_paused_steps(uploaded_workflow_id, invocation_id, order_index=4, action=True)
             self.workflow_populator.wait_for_invocation_and_jobs(history_id, uploaded_workflow_id, invocation_id)
             invocation = self._invocation_details(uploaded_workflow_id, invocation_id)
             assert invocation["state"] == "scheduled"
-            self.assertEqual(
-                "reviewed\n1\nreviewed\n4\n", self.dataset_populator.get_history_dataset_content(history_id)
-            )
+            assert "reviewed\n1\nreviewed\n4\n" == self.dataset_populator.get_history_dataset_content(history_id)
 
     @skip_without_tool("cat")
     def test_cancel_workflow_invocation(self):
         with self.dataset_populator.test_history() as history_id:
             # Invoke a workflow with a pause step.
             uploaded_workflow_id, invocation_id = self._invoke_paused_workflow(history_id)
 
@@ -3032,14 +3727,253 @@
 
             invocation_url = self._api_url(f"workflows/{uploaded_workflow_id}/usage/{invocation_id}", use_key=True)
             delete_response = delete(invocation_url)
             self._assert_status_code_is(delete_response, 200)
 
             invocation = self._invocation_details(uploaded_workflow_id, invocation_id)
             assert invocation["state"] == "cancelled"
+            message = invocation["messages"][0]
+            assert message["reason"] == "user_request"
+
+    def test_workflow_failed_output_not_found(self, history_id):
+        summary = self._run_workflow(
+            """
+class: GalaxyWorkflow
+inputs: []
+steps:
+  create_2:
+    tool_id: create_2
+    state:
+      sleep_time: 0
+    outputs:
+      out_file1:
+        rename: "my new name"
+      out_file2:
+        rename: "my other new name"
+  first_cat1:
+    tool_id: cat
+    in:
+      input1: create_2/does_not_exist
+ """,
+            history_id=history_id,
+            assert_ok=False,
+            wait=True,
+        )
+        invocation = self.workflow_populator.get_invocation(summary.invocation_id)
+        assert invocation["state"] == "failed"
+        assert len(invocation["messages"]) == 1
+        message = invocation["messages"][0]
+        assert message["reason"] == "output_not_found"
+        assert message["workflow_step_id"] == 1
+        assert message["dependent_workflow_step_id"] == 0
+
+    def test_workflow_warning_workflow_output_not_found(self, history_id):
+        summary = self._run_workflow(
+            """
+class: GalaxyWorkflow
+inputs: []
+steps:
+  create_2:
+    tool_id: create_2
+    state:
+      sleep_time: 0
+    outputs:
+      out_file1:
+        rename: "my new name"
+      out_file2:
+        rename: "my other new name"
+outputs:
+  main_out:
+    outputSource: create_2/does_not_exist
+ """,
+            history_id=history_id,
+            assert_ok=False,
+            wait=True,
+        )
+        invocation = self.workflow_populator.get_invocation(summary.invocation_id)
+        assert invocation["state"] == "scheduled"
+        assert len(invocation["messages"]) == 1
+        message = invocation["messages"][0]
+        assert message["reason"] == "workflow_output_not_found"
+        assert "workflow_step_id" in message
+        assert message["output_name"] == "does_not_exist"
+
+    @skip_without_tool("identifier_multiple")
+    def test_invocation_map_over(self, history_id):
+        summary = self._run_workflow(
+            """
+class: GalaxyWorkflow
+inputs:
+  input_collection:
+    collection_type: list
+    type: collection
+outputs:
+  main_out:
+    outputSource: subworkflow/sub_out
+steps:
+  subworkflow:
+    in:
+      data_input: input_collection
+    run:
+      class: GalaxyWorkflow
+      inputs:
+        data_input:
+          type: data
+      outputs:
+        sub_out:
+          outputSource: output_step/output1
+      steps:
+        intermediate_step:
+          tool_id: identifier_multiple
+          in:
+            input1: data_input
+        output_step:
+          tool_id: identifier_multiple
+          in:
+            input1: intermediate_step/output1
+test_data:
+  input_collection:
+    collection_type: list
+    elements:
+      - identifier: 1
+        content: A
+      - identifier: 2
+        content: B
+        """,
+            history_id=history_id,
+            assert_ok=True,
+            wait=True,
+        )
+        invocation = self.workflow_populator.get_invocation(summary.invocation_id)
+        # For consistency and conditional subworkflow steps this really needs to remain
+        # a collection and not get reduced.
+        assert "main_out" in invocation["output_collections"], invocation
+        hdca_details = self.dataset_populator.get_history_collection_details(history_id)
+        assert hdca_details["collection_type"] == "list"
+        elements = hdca_details["elements"]
+        assert len(elements) == 2
+        assert elements[0]["element_identifier"] == "1"
+        assert elements[0]["element_type"] == "hda"
+        hda_id = elements[0]["object"]["id"]
+        hda_content = self.dataset_populator.get_history_dataset_content(history_id, content_id=hda_id)
+        assert hda_content.strip() == "1"
+
+    @skip_without_tool("identifier_multiple")
+    def test_invocation_map_over_inner_collection(self, history_id):
+        summary = self._run_workflow(
+            """
+class: GalaxyWorkflow
+inputs:
+  input_collection:
+    collection_type: list:list
+    type: collection
+outputs:
+  main_out:
+    outputSource: subworkflow/sub_out
+steps:
+  subworkflow:
+    in:
+      list_input: input_collection
+    run:
+      class: GalaxyWorkflow
+      inputs:
+        list_input:
+          type: collection
+          collection_type: list
+      outputs:
+        sub_out:
+          outputSource: output_step/output1
+      steps:
+        intermediate_step:
+          tool_id: identifier_multiple
+          in:
+            input1: list_input
+        output_step:
+          tool_id: identifier_multiple
+          in:
+            input1: intermediate_step/output1
+test_data:
+  input_collection:
+    collection_type: list:list
+        """,
+            history_id=history_id,
+            assert_ok=True,
+            wait=True,
+        )
+        invocation = self.workflow_populator.get_invocation(summary.invocation_id)
+        assert "main_out" in invocation["output_collections"], invocation
+        input_hdca_details = self.dataset_populator.get_history_collection_details(
+            history_id, content_id=invocation["inputs"]["0"]["id"]
+        )
+        assert input_hdca_details["collection_type"] == "list:list"
+        assert len(input_hdca_details["elements"]) == 1
+        assert input_hdca_details["elements"][0]["element_identifier"] == "test_level_1"
+        hdca_details = self.dataset_populator.get_history_collection_details(
+            history_id, content_id=invocation["output_collections"]["main_out"]["id"]
+        )
+        assert hdca_details["collection_type"] == "list"
+        elements = hdca_details["elements"]
+        assert len(elements) == 1
+        assert elements[0]["element_identifier"] == "test_level_1"
+        assert elements[0]["element_type"] == "hda"
+
+    @skip_without_tool("identifier_multiple")
+    def test_invocation_map_over_inner_collection_with_tool_collection_input(self, history_id):
+        summary = self._run_workflow(
+            """
+class: GalaxyWorkflow
+inputs:
+  input_collection:
+    collection_type: list:list
+    type: collection
+outputs:
+  main_out:
+    outputSource: subworkflow/sub_out
+steps:
+  subworkflow:
+    in:
+      list_input: input_collection
+    run:
+      class: GalaxyWorkflow
+      inputs:
+        list_input:
+          type: collection
+          collection_type: list
+      outputs:
+        sub_out:
+          outputSource: output_step/output1
+      steps:
+        output_step:
+          tool_id: identifier_all_collection_types
+          in:
+            input1: list_input
+test_data:
+  input_collection:
+    collection_type: list:list
+        """,
+            history_id=history_id,
+            assert_ok=True,
+            wait=True,
+        )
+        invocation = self.workflow_populator.get_invocation(summary.invocation_id)
+        assert "main_out" in invocation["output_collections"], invocation
+        input_hdca_details = self.dataset_populator.get_history_collection_details(
+            history_id, content_id=invocation["inputs"]["0"]["id"]
+        )
+        assert input_hdca_details["collection_type"] == "list:list"
+        assert len(input_hdca_details["elements"]) == 1
+        assert input_hdca_details["elements"][0]["element_identifier"] == "test_level_1"
+        hdca_details = self.dataset_populator.get_history_collection_details(
+            history_id, content_id=invocation["output_collections"]["main_out"]["id"]
+        )
+        assert hdca_details["collection_type"] == "list"
+        elements = hdca_details["elements"]
+        assert len(elements) == 1
+        assert elements[0]["element_identifier"] == "test_level_1"
+        assert elements[0]["element_type"] == "hda"
 
     @skip_without_tool("cat")
     def test_pause_outputs_with_deleted_inputs(self):
         self._deleted_inputs_workflow(purge=False)
 
     @skip_without_tool("cat")
     def test_error_outputs_with_purged_inputs(self):
@@ -3084,15 +4018,15 @@
             )
             r = self.workflow_populator.invoke_workflow_raw(workflow_id, workflow_request)
             self._assert_status_code_is(r, 200)
             invocation_id = r.json()["id"]
             # If this starts failing we may have prevented running workflows on collections with deleted members,
             # in which case we can disable this test.
             self.workflow_populator.wait_for_invocation_and_jobs(
-                workflow_id, history_id, invocation_id, assert_ok=False
+                history_id=history_id, workflow_id=workflow_id, invocation_id=invocation_id, assert_ok=False
             )
             contents = self.__history_contents(history_id)
             datasets = [content for content in contents if content["history_content_type"] == "dataset"]
             assert datasets[DELETED]["deleted"]
             state = "error" if purge else "paused"
             assert datasets[PAUSED_1]["state"] == state
             assert datasets[PAUSED_2]["state"] == "paused"
@@ -3438,18 +4372,17 @@
   type: raw
 """,
                 history_id=history_id,
             )
 
             self.dataset_populator.wait_for_history(history_id, assert_ok=True)
             content = self.dataset_populator.get_history_dataset_content(history_id)
-            self.assertEqual("chrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n", content)
+            assert "chrX\t152691446\t152691471\tCCDS14735.1_cds_0_0_chrX_152691447_f\t0\t+\n" == content
 
-    def test_run_with_numeric_input_connection(self):
-        history_id = self.dataset_populator.new_history()
+    def test_run_with_numeric_input_connection(self, history_id):
         self._run_jobs(
             """
 class: GalaxyWorkflow
 steps:
 - label: forty_two
   tool_id: expression_forty_two
   state: {}
@@ -3471,16 +4404,15 @@
         str_43 = lines[0]
         str_4point14 = lines[2]
         assert lines[3] == ""
         assert int(str_43) == 43
         assert abs(float(str_4point14) - 4.14) < 0.0001
 
     @skip_without_tool("param_value_from_file")
-    def test_expression_tool_map_over(self):
-        history_id = self.dataset_populator.new_history()
+    def test_expression_tool_map_over(self, history_id):
         self._run_jobs(
             """
 class: GalaxyWorkflow
 inputs:
   text_input1: collection
 steps:
 - label: param_out
@@ -3644,18 +4576,16 @@
             # Now make sure that the HDAs in each history point to the same dataset instances
             history_one_contents = self.__history_contents(history_id_one)
             history_two_contents = self.__history_contents(history_id_two)
             assert len(history_one_contents) == len(history_two_contents)
             for i, (item_one, item_two) in enumerate(zip(history_one_contents, history_two_contents)):
                 assert (
                     item_one["dataset_id"] == item_two["dataset_id"]
-                ), 'Dataset ids should match, but "%s" and "%s" are not the same for History item %i.' % (
-                    item_one["dataset_id"],
-                    item_two["dataset_id"],
-                    i + 1,
+                ), 'Dataset ids should match, but "{}" and "{}" are not the same for History item {}.'.format(
+                    item_one["dataset_id"], item_two["dataset_id"], i + 1
                 )
 
     def test_cannot_run_inaccessible_workflow(self):
         workflow = self.workflow_populator.load_workflow(name="test_for_run_cannot_access")
         workflow_request, _, workflow_id = self._setup_workflow_run(workflow)
         with self._different_user():
             run_workflow_response = self._post(f"workflows/{workflow_id}/invocations", data=workflow_request)
@@ -3700,21 +4630,19 @@
             label_map = {"list1": self._ds_entry(hdca1), "list2": self._ds_entry(hdca2)}
             workflow_request = dict(
                 ds_map=self.workflow_populator.build_ds_map(workflow_id, label_map),
             )
             self.workflow_populator.invoke_workflow_and_wait(
                 workflow_id, history_id=history_id, request=workflow_request
             )
-            self.assertEqual(
-                "1 2 3\n4 5 6\n7 8 9\n0 a b\n", self.dataset_populator.get_history_dataset_content(history_id)
-            )
+            assert "1 2 3\n4 5 6\n7 8 9\n0 a b\n" == self.dataset_populator.get_history_dataset_content(history_id)
 
     def test_workflow_stability(self):
         # Run this index stability test with following command:
-        #   ./run_tests.sh test/api/test_workflows.py:WorkflowsApiTestCase.test_workflow_stability
+        #   ./run_tests.sh test/api/test_workflows.py:TestWorkflowsApi.test_workflow_stability
         num_tests = 1
         for workflow_file in ["test_workflow_topoambigouity", "test_workflow_topoambigouity_auto_laidout"]:
             workflow = self.workflow_populator.load_workflow_from_resource(workflow_file)
             last_step_map = self._step_map(workflow)
             for _ in range(num_tests):
                 uploaded_workflow_id = self.workflow_populator.create_workflow(workflow)
                 downloaded_workflow = self._download_workflow(uploaded_workflow_id)
@@ -4822,14 +5750,48 @@
         )
         with self.dataset_populator.test_history() as history_id:
             run_workflow = self._download_workflow(workflow_id, style="run", history_id=history_id)
         options = run_workflow["steps"][0]["inputs"][0]["options"]
         assert len(options) == 5
         assert options[0] == ["Ex1", "--ex1", False]
 
+    def test_value_restriction_with_select_from_subworkflow_input(self):
+        workflow_id = self.workflow_populator.upload_yaml_workflow(
+            """
+class: GalaxyWorkflow
+inputs:
+  Outer input parameter:
+    optional: false
+    restrictOnConnections: true
+    type: string
+steps:
+- in:
+    inner input parameter:
+      source: Outer input parameter
+  run:
+    class: GalaxyWorkflow
+    label: Restriction from subworkflow param
+    inputs:
+      inner input parameter:
+        optional: false
+        restrictOnConnections: true
+        type: string
+    steps:
+    - tool_id: multi_select
+      in:
+        select_ex:
+          source: inner input parameter
+"""
+        )
+        with self.dataset_populator.test_history() as history_id:
+            run_workflow = self._download_workflow(workflow_id, style="run", history_id=history_id)
+        options = run_workflow["steps"][0]["inputs"][0]["options"]
+        assert len(options) == 5
+        assert options[0] == ["Ex1", "--ex1", False]
+
     @skip_without_tool("random_lines1")
     def test_run_replace_params_by_tool(self):
         workflow_request, history_id, workflow_id = self._setup_random_x2_workflow("test_for_replace_tool_params")
         workflow_request["parameters"] = dumps(dict(random_lines1=dict(num_lines=5)))
         self.workflow_populator.invoke_workflow_and_wait(workflow_id, request=workflow_request)
         # Would be 8 and 6 without modification
         self.__assert_lines_hid_line_count_is(history_id, 2, 5)
@@ -4890,18 +5852,18 @@
             r2 = "4 5 6\t1\n1 2 3\t2\n"
             r3 = "7 8 9\t1\n1 2 3\t2\n"
             r4 = "10 11 12\t1\n1 2 3\t2\n"
             t1 = self.dataset_populator.get_history_dataset_content(history_id, hid=7)
             t2 = self.dataset_populator.get_history_dataset_content(history_id, hid=10)
             t3 = self.dataset_populator.get_history_dataset_content(history_id, hid=13)
             t4 = self.dataset_populator.get_history_dataset_content(history_id, hid=16)
-            self.assertEqual(r1, t1)
-            self.assertEqual(r2, t2)
-            self.assertEqual(r3, t3)
-            self.assertEqual(r4, t4)
+            assert r1 == t1
+            assert r2 == t2
+            assert r3 == t3
+            assert r4 == t4
 
     @skip_without_tool("cat1")
     @skip_without_tool("addValue")
     def test_run_batch_inputs(self):
         workflow = self.workflow_populator.load_workflow_from_resource("test_workflow_batch")
         workflow_id = self.workflow_populator.create_workflow(workflow)
         with self.dataset_populator.test_history() as history_id:
@@ -4942,28 +5904,26 @@
             r2 = "4 5 6\t1\n1 2 3\t2\n"
             r3 = "7 8 9\t1\n1 2 3\t2\n"
             r4 = "10 11 12\t1\n1 2 3\t2\n"
             t1 = self.dataset_populator.get_history_dataset_content(history_id, hid=7)
             t2 = self.dataset_populator.get_history_dataset_content(history_id, hid=10)
             t3 = self.dataset_populator.get_history_dataset_content(history_id, hid=13)
             t4 = self.dataset_populator.get_history_dataset_content(history_id, hid=16)
-            self.assertEqual(r1, t1)
-            self.assertEqual(r2, t2)
-            self.assertEqual(r3, t3)
-            self.assertEqual(r4, t4)
+            assert r1 == t1
+            assert r2 == t2
+            assert r3 == t3
+            assert r4 == t4
 
     @skip_without_tool("validation_default")
     def test_parameter_substitution_sanitization(self):
         substitions = dict(input1='" ; echo "moo')
         run_workflow_response, history_id = self._run_validation_workflow_with_substitions(substitions)
 
         self.dataset_populator.wait_for_history(history_id, assert_ok=True)
-        self.assertEqual(
-            "__dq__ X echo __dq__moo\n", self.dataset_populator.get_history_dataset_content(history_id, hid=1)
-        )
+        assert "__dq__ X echo __dq__moo\n" == self.dataset_populator.get_history_dataset_content(history_id, hid=1)
 
     @skip_without_tool("validation_repeat")
     def test_parameter_substitution_validation_value_errors_0(self):
         with self.dataset_populator.test_history() as history_id:
             workflow_id = self._upload_yaml_workflow(
                 """
 class: GalaxyWorkflow
@@ -5017,15 +5977,15 @@
             history=f"hist_id={history_id}",
             workflow_id=uploaded_workflow_id,
             parameters=dumps(dict(validation_default=substitions)),
         )
         run_workflow_response = self.workflow_populator.invoke_workflow_raw(uploaded_workflow_id, workflow_request)
         return run_workflow_response, history_id
 
-    def test_subworkflow_import_order_maintained(self):
+    def test_subworkflow_import_order_maintained(self, history_id):
         summary = self._run_workflow(
             """
 class: GalaxyWorkflow
 inputs:
   outer_input_1:
     type: int
     default: 1
@@ -5064,14 +6024,15 @@
           outputSource: inner_input_2/output
 outputs:
   - label: out_1
     outputSource: nested_workflow/nested_out_1
   - label: out_2
     outputSource: nested_workflow/nested_out_2
 """,
+            history_id=history_id,
             assert_ok=False,
             wait=False,
         )
         self.workflow_populator.wait_for_invocation(summary.workflow_id, summary.invocation_id)
         self.workflow_populator.wait_for_history_workflows(
             summary.history_id, assert_ok=False, expected_invocation_count=2
         )
@@ -5105,15 +6066,15 @@
             {
                 str(steps[0]["id"]): dict(num_lines=1, seed_source=seed_source),
                 str(steps[1]["id"]): dict(num_lines=1, seed_source=seed_source),
             }
         )
         workflow_request["parameters"] = params
         self.workflow_populator.invoke_workflow_and_wait(workflow_id, request=workflow_request)
-        self.assertEqual("2\n", self.dataset_populator.get_history_dataset_content(history_id))
+        assert "2\n" == self.dataset_populator.get_history_dataset_content(history_id)
 
     @skip_without_tool("random_lines1")
     def test_run_replace_params_nested_normalized(self):
         workflow_request, history_id, workflow_id, steps = self._setup_random_x2_workflow_steps(
             "test_for_replace_step_normalized_params_nested"
         )
         parameters = {
@@ -5121,15 +6082,15 @@
             "seed_source|seed_source_selector": "set_seed",
             "seed_source|seed": "moo",
         }
         params = dumps({str(steps[0]["id"]): parameters, str(steps[1]["id"]): parameters})
         workflow_request["parameters"] = params
         workflow_request["parameters_normalized"] = False
         self.workflow_populator.invoke_workflow_and_wait(workflow_id, request=workflow_request)
-        self.assertEqual("2\n", self.dataset_populator.get_history_dataset_content(history_id))
+        assert "2\n" == self.dataset_populator.get_history_dataset_content(history_id)
 
     @skip_without_tool("random_lines1")
     def test_run_replace_params_over_default(self):
         with self.dataset_populator.test_history() as history_id:
             self._run_jobs(
                 WORKFLOW_ONE_STEP_DEFAULT,
                 test_data="""
@@ -5151,14 +6112,52 @@
     @skip_without_tool("random_lines1")
     def test_defaults_editor(self):
         workflow_id = self._upload_yaml_workflow(WORKFLOW_ONE_STEP_DEFAULT, publish=True)
         workflow_object = self._download_workflow(workflow_id, style="editor")
         put_response = self._update_workflow(workflow_id, workflow_object)
         assert put_response.status_code == 200
 
+    def test_empty_collection_sort(self, history_id):
+        self._run_workflow(
+            """class: GalaxyWorkflow
+inputs:
+  input: collection
+  filter_file: data
+steps:
+  filter_collection:
+    tool_id: __FILTER_FROM_FILE__
+    in:
+       input: input
+       how|filter_source: filter_file
+  sort_collection_1:
+    tool_id: __SORTLIST__
+    in:
+      input: filter_collection/output_filtered
+  sort_collection_2:
+    tool_id: __SORTLIST__
+    in:
+      input: filter_collection/output_discarded
+  merge_collection:
+    tool_id: __MERGE_COLLECTION__
+    in:
+      inputs_0|input: sort_collection_1/output
+      inputs_1|input: sort_collection_2/output
+test_data:
+  input:
+    collection_type: list
+    elements:
+      - identifier: i1
+        content: "0"
+  filter_file: i1
+""",
+            history_id=history_id,
+            wait=True,
+            assert_ok=True,
+        )
+
     @skip_without_tool("random_lines1")
     def test_run_replace_params_over_default_delayed(self):
         with self.dataset_populator.test_history() as history_id:
             run_summary = self._run_workflow(
                 """
 class: GalaxyWorkflow
 inputs:
@@ -5210,25 +6209,27 @@
         pjas = list(downloaded_workflow["steps"]["2"]["post_job_actions"].values())
         assert len(pjas) == 1, len(pjas)
         pja = pjas[0]
         self._assert_has_keys(pja, "action_type", "output_name", "action_arguments")
 
     def test_invocation_filtering(self):
         with self._different_user(email=f"{uuid4()}@test.com"):
+            history_id = self.dataset_populator.new_history()
             # new user, start with no invocations
             assert not self._assert_invocation_for_url_is("invocations")
             self._run_jobs(
                 """
 class: GalaxyWorkflow
 inputs:
   input:
     type: data
     optional: true
 steps: []
 """,
+                history_id=history_id,
                 wait=False,
             )
             first_invocation = self._assert_invocation_for_url_is("invocations")
             new_history_id = self.dataset_populator.new_history()
             # new history has no invocations
             assert not self._assert_invocation_for_url_is(f"invocations?history_id={new_history_id}")
             self._run_jobs(
@@ -5343,53 +6344,35 @@
         workflow_id, invocation_id = self._run_mapping_workflow()
 
         usage_details = self._invocation_details(workflow_id, invocation_id)
         # Assert some high-level things about the structure of data returned.
         self._assert_has_keys(usage_details, "inputs", "steps", "workflow_id")
 
         invocation_steps = usage_details["steps"]
-        invocation_input_step, invocation_tool_step = None, None
-        for invocation_step in invocation_steps:
+        for step_index, invocation_step in enumerate(invocation_steps):
             self._assert_has_keys(invocation_step, "workflow_step_id", "order_index", "id")
-            order_index = invocation_step["order_index"]
-            assert order_index in [0, 1]
-            if invocation_step["order_index"] == 0:
-                assert invocation_input_step is None
-                invocation_input_step = invocation_step
-            else:
-                assert invocation_tool_step is None
-                invocation_tool_step = invocation_step
-
-        assert invocation_input_step
-        assert invocation_tool_step
+            assert step_index == invocation_step["order_index"]
+        invocation_input_step = invocation_steps[0]
+        invocation_tool_step = invocation_steps[1]
 
         # Tool steps have non-null job_ids (deprecated though they may be)
-        assert invocation_input_step.get("job_id", None) is None
-        assert invocation_tool_step.get("job_id", None) is None
+        assert invocation_input_step.get("job_id") is None
+        assert invocation_tool_step.get("job_id") is None
         assert invocation_tool_step["state"] == "scheduled"
 
         usage_details = self._invocation_details(workflow_id, invocation_id, legacy_job_state="true")
         # Assert some high-level things about the structure of data returned.
         self._assert_has_keys(usage_details, "inputs", "steps", "workflow_id")
 
         invocation_steps = usage_details["steps"]
-        invocation_input_step = None
-        invocation_tool_steps = []
+        assert len(invocation_steps) == 3
         for invocation_step in invocation_steps:
             self._assert_has_keys(invocation_step, "workflow_step_id", "order_index", "id")
-            order_index = invocation_step["order_index"]
-            assert order_index in [0, 1]
-            if invocation_step["order_index"] == 0:
-                assert invocation_input_step is None
-                invocation_input_step = invocation_step
-            else:
-                invocation_tool_steps.append(invocation_step)
 
-        assert len(invocation_tool_steps) == 2
-        assert invocation_tool_steps[0]["state"] == "ok"
+        assert invocation_steps[1]["state"] == "ok"
 
     def _run_mapping_workflow(self):
         history_id = self.dataset_populator.new_history()
         summary = self._run_workflow(
             """
 class: GalaxyWorkflow
 inputs:
@@ -5603,15 +6586,15 @@
 
     def __assert_lines_hid_line_count_is(self, history, hid, lines):
         contents_url = f"histories/{history}/contents"
         history_contents = self.__history_contents(history)
         hda_summary = next(hc for hc in history_contents if hc["hid"] == hid)
         hda_info_response = self._get(f"{contents_url}/{hda_summary['id']}")
         self._assert_status_code_is(hda_info_response, 200)
-        self.assertEqual(hda_info_response.json()["metadata_data_lines"], lines)
+        assert hda_info_response.json()["metadata_data_lines"] == lines
 
     def __history_contents(self, history_id):
         contents_url = f"histories/{history_id}/contents"
         history_contents_response = self._get(contents_url)
         self._assert_status_code_is(history_contents_response, 200)
         return history_contents_response.json()
 
@@ -5653,19 +6636,18 @@
     def _all_user_invocation_ids(self):
         all_invocations_for_user = self._get("invocations")
         self._assert_status_code_is(all_invocations_for_user, 200)
         invocation_ids = [i["id"] for i in all_invocations_for_user.json()]
         return invocation_ids
 
 
-class AdminWorkflowsApiTestCase(BaseWorkflowsApiTestCase):
-
+class TestAdminWorkflowsApi(BaseWorkflowsApiTestCase):
     require_admin_user = True
 
-    def test_import_export_dynamic_tools(self):
+    def test_import_export_dynamic_tools(self, history_id):
         workflow_id = self._upload_yaml_workflow(
             """
 class: GalaxyWorkflow
 steps:
   - type: input
     label: input1
   - tool_id: cat1
@@ -5690,18 +6672,14 @@
 test_data:
   input1: "hello world"
 """
         )
         downloaded_workflow = self._download_workflow(workflow_id)
         response = self.workflow_populator.create_workflow_response(downloaded_workflow)
         workflow_id = response.json()["id"]
-        history_id = self.dataset_populator.new_history()
         hda1 = self.dataset_populator.new_dataset(history_id, content="Hello World Second!")
         workflow_request = dict(
             inputs_by="name",
             inputs=json.dumps({"input1": self._ds_entry(hda1)}),
         )
         self.workflow_populator.invoke_workflow_and_wait(workflow_id, history_id=history_id, request=workflow_request)
-        self.assertEqual(
-            "Hello World Second!\nhello world 2\n",
-            self.dataset_populator.get_history_dataset_content(history_id),
-        )
+        assert self.dataset_populator.get_history_dataset_content(history_id) == "Hello World Second!\nhello world 2\n"
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test/api/test_workflows_from_yaml.py` & `galaxy-test-api-23.0.2/galaxy_test/api/test_workflows_from_yaml.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import json
 import os
 
-from galaxy_test.base.populators import uses_test_history
 from galaxy_test.base.workflow_fixtures import (
     WORKFLOW_PARAMETER_INPUT_INTEGER_DEFAULT,
     WORKFLOW_RUNTIME_PARAMETER_SIMPLE,
     WORKFLOW_SIMPLE_CAT_AND_RANDOM_LINES,
     WORKFLOW_SIMPLE_CAT_TWICE,
     WORKFLOW_WITH_OUTPUT_ACTIONS,
     WORKFLOW_WITH_OUTPUTS,
 )
 from .test_workflows import BaseWorkflowsApiTestCase
 
 WORKFLOWS_DIRECTORY = os.path.abspath(os.path.dirname(__file__))
 
 
-class WorkflowsFromYamlApiTestCase(BaseWorkflowsApiTestCase):
+class TestWorkflowsFromYamlApi(BaseWorkflowsApiTestCase):
     def setUp(self):
         super().setUp()
 
     def _upload_and_download(self, yaml_workflow, **kwds):
         style = None
         if "style" in kwds:
             style = kwds.pop("style")
@@ -74,21 +73,21 @@
         self._run_jobs(
             WORKFLOW_SIMPLE_CAT_TWICE,
             test_data={"input1": "hello world"},
             history_id=history_id,
             round_trip_format_conversion=True,
         )
         contents1 = self.dataset_populator.get_history_dataset_content(history_id)
-        self.assertEqual(contents1.strip(), "hello world\nhello world")
+        assert contents1.strip() == "hello world\nhello world"
 
     def test_outputs(self):
         workflow_id = self._upload_yaml_workflow(WORKFLOW_WITH_OUTPUTS, round_trip_format_conversion=True)
         workflow = self._get(f"workflows/{workflow_id}/download").json()
-        self.assertEqual(workflow["steps"]["1"]["workflow_outputs"][0]["output_name"], "out_file1")
-        self.assertEqual(workflow["steps"]["1"]["workflow_outputs"][0]["label"], "wf_output_1")
+        assert workflow["steps"]["1"]["workflow_outputs"][0]["output_name"] == "out_file1"
+        assert workflow["steps"]["1"]["workflow_outputs"][0]["label"] == "wf_output_1"
         workflow = self.workflow_populator.download_workflow(workflow_id, style="format2")
 
     def test_runtime_inputs(self):
         workflow = self._upload_and_download(WORKFLOW_RUNTIME_PARAMETER_SIMPLE)
         assert len(workflow["steps"]) == 2
         runtime_step = workflow["steps"]["1"]
         for runtime_input in runtime_step["inputs"]:
@@ -156,15 +155,15 @@
 
         subworkflow_connections = subworkflow_step["input_connections"]
         assert len(subworkflow_connections) == 1
         subworkflow_connection = subworkflow_connections["inner_input"]
         assert subworkflow_connection["input_subworkflow_step_id"] == 0
 
         # content = self.dataset_populator.get_history_dataset_content( history_id )
-        # self.assertEqual("chr5\t131424298\t131424460\tCCDS4149.1_cds_0_0_chr5_131424299_f\t0\t+\n", content)
+        # assert content == "chr5\t131424298\t131424460\tCCDS4149.1_cds_0_0_chr5_131424299_f\t0\t+\n"
 
     def test_subworkflow_duplicate(self):
         duplicate_subworkflow_invocate_wf = """
 format-version: "v2.0"
 $graph:
 - id: nested
   class: GalaxyWorkflow
@@ -258,15 +257,14 @@
     state:
       input1:
         $link: test_input
 """
         )
         self.workflow_populator.dump_workflow(workflow_id)
 
-    @uses_test_history()
     def test_conditional_ints(self, history_id):
         self._run_jobs(
             """
 class: GalaxyWorkflow
 steps:
   test_input:
     tool_id: disambiguate_cond
@@ -335,23 +333,23 @@
 test_data:
   input1: "hello world"
 """,
             history_id=history_id,
         )
 
         content = self.dataset_populator.get_history_dataset_content(history_id)
-        self.assertEqual(content, "hello world\nhello world 2\n")
+        assert content == "hello world\nhello world 2\n"
 
     def test_workflow_import_tool(self):
         history_id = self.dataset_populator.new_history()
         workflow_path = os.path.join(WORKFLOWS_DIRECTORY, "embed_test_1.gxwf.yml")
         jobs_descriptions = {"test_data": {"input1": "hello world"}}
         self._run_jobs(workflow_path, source_type="path", jobs_descriptions=jobs_descriptions, history_id=history_id)
         content = self.dataset_populator.get_history_dataset_content(history_id)
-        self.assertEqual(content, "hello world\nhello world 2\n")
+        assert content == "hello world\nhello world 2\n"
 
     def test_parameter_default_rep(self):
         workflow = self._upload_and_download(WORKFLOW_PARAMETER_INPUT_INTEGER_DEFAULT)
         int_input = self._steps_by_label(workflow)["int_input"]
         int_input_state = json.loads(int_input["tool_state"])
         assert int_input_state["default"] == 3
         assert int_input_state["optional"] is True
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test_api.egg-info/PKG-INFO` & `galaxy-test-api-23.0.2/galaxy_test_api.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-api
-Version: 22.5.0.dev0
+Version: 23.0.2
 Summary: Galaxy API tests
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: driver
 License-File: LICENSE
@@ -33,29 +34,49 @@
 
 
 Overview
 --------
 
 The Galaxy_ API tests.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.1.dev0
----------------------
+-------------------
+23.0.2 (2023-06-13)
+-------------------
 
+No recorded changes since last release
 
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
----------------------
+
+=========
+Bug fixes
+=========
+
+* Display DCE in job parameter component, allow rerunning with DCE input by `@mvdbeek <https://github.com/mvdbeek>`_ in `#15744 <https://github.com/galaxyproject/galaxy/pull/15744>`_
+* Fix folder listing via file browser by `@mvdbeek <https://github.com/mvdbeek>`_ in `#15950 <https://github.com/galaxyproject/galaxy/pull/15950>`_
+* Fix case sensitive filtering by name in histories by `@davelopez <https://github.com/davelopez>`_ in `#16036 <https://github.com/galaxyproject/galaxy/pull/16036>`_
+* Fix dataype_change not updating HDCA update_time by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16099 <https://github.com/galaxyproject/galaxy/pull/16099>`_
+* Extract HDA for code_file validate_input hook by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16120 <https://github.com/galaxyproject/galaxy/pull/16120>`_
+
+============
+Enhancements
+============
+
+* Add support for launching workflows via Tutorial Mode by `@hexylena <https://github.com/hexylena>`_ in `#15684 <https://github.com/galaxyproject/galaxy/pull/15684>`_
+* Allow setting auto_decompress property in staging interface by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16014 <https://github.com/galaxyproject/galaxy/pull/16014>`_
+
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * Initial import from dev branch of Galaxy during 20.09 branch of Galaxy.
-
```

### Comparing `galaxy-test-api-22.5.0.dev0/galaxy_test_api.egg-info/SOURCES.txt` & `galaxy-test-api-23.0.2/galaxy_test_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 MANIFEST.in
 README.rst
 dev-requirements.txt
 pyproject.toml
 setup.cfg
 test-requirements.txt
 galaxy_test/__init__.py
+galaxy_test/py.typed
 galaxy_test/api/__init__.py
 galaxy_test/api/_framework.py
 galaxy_test/api/embed_test_1.gxwf.yml
 galaxy_test/api/embed_test_1_tool.gxtool.yml
 galaxy_test/api/sharable.py
 galaxy_test/api/test_authenticate.py
 galaxy_test/api/test_configuration.py
 galaxy_test/api/test_container_resolution.py
 galaxy_test/api/test_dataset_collections.py
 galaxy_test/api/test_datasets.py
 galaxy_test/api/test_datatypes.py
 galaxy_test/api/test_display_applications.py
+galaxy_test/api/test_drs.py
 galaxy_test/api/test_folder_contents.py
 galaxy_test/api/test_folders.py
 galaxy_test/api/test_framework.py
 galaxy_test/api/test_group_roles.py
 galaxy_test/api/test_group_users.py
 galaxy_test/api/test_groups.py
 galaxy_test/api/test_histories.py
@@ -31,14 +33,15 @@
 galaxy_test/api/test_jobs.py
 galaxy_test/api/test_libraries.py
 galaxy_test/api/test_licenses.py
 galaxy_test/api/test_page_revisions.py
 galaxy_test/api/test_pages.py
 galaxy_test/api/test_roles.py
 galaxy_test/api/test_search.py
+galaxy_test/api/test_short_term_storage.py
 galaxy_test/api/test_tool_data.py
 galaxy_test/api/test_tools.py
 galaxy_test/api/test_tools_upload.py
 galaxy_test/api/test_tours.py
 galaxy_test/api/test_users.py
 galaxy_test/api/test_visualizations.py
 galaxy_test/api/test_webhooks.py
```

### Comparing `galaxy-test-api-22.5.0.dev0/setup.cfg` & `galaxy-test-api-23.0.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy API tests
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-test-api
 url = https://github.com/galaxyproject/galaxy
-version = 22.5.0.dev0
+version = 23.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-test-base
 	pytest
 	python-dateutil
```

