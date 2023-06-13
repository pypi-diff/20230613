# Comparing `tmp/exabyte-api-client-2023.5.18.post0.tar.gz` & `tmp/exabyte-api-client-2023.6.13.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exabyte-api-client-2023.5.18.post0.tar", last modified: Thu May 18 19:16:07 2023, max compression
+gzip compressed data, was "exabyte-api-client-2023.6.13.post0.tar", last modified: Tue Jun 13 00:36:19 2023, max compression
```

## Comparing `exabyte-api-client-2023.5.18.post0.tar` & `exabyte-api-client-2023.6.13.post0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.925072 exabyte-api-client-2023.5.18.post0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.917072 exabyte-api-client-2023.5.18.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-18 19:16:07.925072 exabyte-api-client-2023.5.18.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.917072 exabyte-api-client-2023.5.18.post0/exabyte_api_client/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-18 19:16:07.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/bank_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/bank_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/bank_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/charges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/mixins/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/mixins/set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/raw_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/refined_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/exabyte_api_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/utils/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client/utils/materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-18 19:16:07.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-18 19:16:07.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:16:07.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 19:16:07.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-18 19:16:07.000000 exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/requirements-dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-18 19:16:07.925072 exabyte-api-client-2023.5.18.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/data/login.json
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/data/logout.json
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/data/material.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.921072 exabyte-api-client-2023.5.18.post0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/integration/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/integration/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/integration/test_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:16:07.925072 exabyte-api-client-2023.5.18.post0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_bank_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_bank_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_httpBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_refined_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-18 19:15:28.000000 exabyte-api-client-2023.5.18.post0/tests/unit/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:36:19.679920 exabyte-api-client-2023.6.13.post0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:36:19.671920 exabyte-api-client-2023.6.13.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:36:19.675920 exabyte-api-client-2023.6.13.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-13 00:36:19.679920 exabyte-api-client-2023.6.13.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:36:19.675920 exabyte-api-client-2023.6.13.post0/exabyte_api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-13 00:36:19.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:36:19.675920 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/bank_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/bank_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/bank_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/charges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:36:19.675920 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/mixins/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/mixins/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/raw_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/refined_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:36:19.675920 exabyte-api-client-2023.6.13.post0/exabyte_api_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/utils/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client/utils/materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:36:19.679920 exabyte-api-client-2023.6.13.post0/exabyte_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-13 00:36:19.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-13 00:36:19.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:36:19.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 00:36:19.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 00:36:19.000000 exabyte-api-client-2023.6.13.post0/exabyte_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/requirements-dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-13 00:36:19.679920 exabyte-api-client-2023.6.13.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:36:19.679920 exabyte-api-client-2023.6.13.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:36:19.679920 exabyte-api-client-2023.6.13.post0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/data/login.json
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/data/logout.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/data/material.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:36:19.679920 exabyte-api-client-2023.6.13.post0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/integration/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/integration/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/integration/test_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:36:19.679920 exabyte-api-client-2023.6.13.post0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/unit/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/unit/test_bank_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/unit/test_bank_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/unit/test_httpBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/unit/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/unit/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/unit/test_logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/unit/test_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/unit/test_refined_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-13 00:35:42.000000 exabyte-api-client-2023.6.13.post0/tests/unit/test_workflows.py
```

### Comparing `exabyte-api-client-2023.5.18.post0/.github/workflows/cicd.yml` & `exabyte-api-client-2023.6.13.post0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/.gitignore` & `exabyte-api-client-2023.6.13.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/LICENSE.md` & `exabyte-api-client-2023.6.13.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/PKG-INFO` & `exabyte-api-client-2023.6.13.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exabyte-api-client
-Version: 2023.5.18.post0
+Version: 2023.6.13.post0
 Summary: Exabyte Python Client for RESTful API
 Home-page: https://github.com/Exabyte-io/api-client
 Author: Exabyte Inc.
 Author-email: info@mat3ra.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `exabyte-api-client-2023.5.18.post0/README.md` & `exabyte-api-client-2023.6.13.post0/README.md`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/__init__.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/__init__.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/bank_entity.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/bank_entity.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/bank_materials.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/bank_materials.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/bank_workflows.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/bank_workflows.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/charges.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/charges.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/entity.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/entity.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/jobs.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/jobs.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/login.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/login.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/logout.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/logout.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/materials.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/materials.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/mixins/set.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/mixins/set.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/projects.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/projects.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/raw_properties.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/raw_properties.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/refined_properties.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/refined_properties.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/endpoints/workflows.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/endpoints/workflows.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/utils/http.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/utils/http.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client/utils/materials.py` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client/utils/materials.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/PKG-INFO` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exabyte-api-client
-Version: 2023.5.18.post0
+Version: 2023.6.13.post0
 Summary: Exabyte Python Client for RESTful API
 Home-page: https://github.com/Exabyte-io/api-client
 Author: Exabyte Inc.
 Author-email: info@mat3ra.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `exabyte-api-client-2023.5.18.post0/exabyte_api_client.egg-info/SOURCES.txt` & `exabyte-api-client-2023.6.13.post0/exabyte_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/run-tests.sh` & `exabyte-api-client-2023.6.13.post0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/setup.cfg` & `exabyte-api-client-2023.6.13.post0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 [options]
 package_dir = 
 	= .
 packages = find:
 python_requires = >= 3.6
 install_requires = 
-	requests==2.26.0
+	requests>=2.26.0
 
 [options.extras_require]
 test = 
 	coverage[toml]>=5.3
 	mock>=1.3.0
 
 [options.packages.find]
```

### Comparing `exabyte-api-client-2023.5.18.post0/tests/__init__.py` & `exabyte-api-client-2023.6.13.post0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/data/material.json` & `exabyte-api-client-2023.6.13.post0/tests/data/material.json`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/integration/__init__.py` & `exabyte-api-client-2023.6.13.post0/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/integration/entity.py` & `exabyte-api-client-2023.6.13.post0/tests/integration/entity.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/integration/test_jobs.py` & `exabyte-api-client-2023.6.13.post0/tests/integration/test_jobs.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/integration/test_materials.py` & `exabyte-api-client-2023.6.13.post0/tests/integration/test_materials.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/unit/__init__.py` & `exabyte-api-client-2023.6.13.post0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/unit/entity.py` & `exabyte-api-client-2023.6.13.post0/tests/unit/entity.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/unit/test_bank_materials.py` & `exabyte-api-client-2023.6.13.post0/tests/unit/test_bank_materials.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/unit/test_bank_workflows.py` & `exabyte-api-client-2023.6.13.post0/tests/unit/test_bank_workflows.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/unit/test_httpBase.py` & `exabyte-api-client-2023.6.13.post0/tests/unit/test_httpBase.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/unit/test_jobs.py` & `exabyte-api-client-2023.6.13.post0/tests/unit/test_jobs.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/unit/test_login.py` & `exabyte-api-client-2023.6.13.post0/tests/unit/test_login.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/unit/test_logout.py` & `exabyte-api-client-2023.6.13.post0/tests/unit/test_logout.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/unit/test_materials.py` & `exabyte-api-client-2023.6.13.post0/tests/unit/test_materials.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/unit/test_refined_properties.py` & `exabyte-api-client-2023.6.13.post0/tests/unit/test_refined_properties.py`

 * *Files identical despite different names*

### Comparing `exabyte-api-client-2023.5.18.post0/tests/unit/test_workflows.py` & `exabyte-api-client-2023.6.13.post0/tests/unit/test_workflows.py`

 * *Files identical despite different names*

