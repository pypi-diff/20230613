# Comparing `tmp/datashuttle-0.1.0rc1.tar.gz` & `tmp/datashuttle-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datashuttle-0.1.0rc1.tar", last modified: Wed Jun  7 15:19:58 2023, max compression
+gzip compressed data, was "datashuttle-0.1.0rc2.tar", last modified: Wed Jun  7 15:43:19 2023, max compression
```

## Comparing `datashuttle-0.1.0rc1.tar` & `datashuttle-0.1.0rc2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.381699 datashuttle-0.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.369699 datashuttle-0.1.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.373699 datashuttle-0.1.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/.github/workflows/code_test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/.github/workflows/docs_build_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.373699 datashuttle-0.1.0rc1/datashuttle/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31473 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/command_line_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.373699 datashuttle-0.1.0rc1/datashuttle/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/configs/canonical_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/configs/canonical_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/configs/canonical_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/configs/config_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/configs/load_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43692 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/datashuttle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.373699 datashuttle-0.1.0rc1/datashuttle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/ds_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/folder_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    16658 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/rclone.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/datashuttle/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.373699 datashuttle-0.1.0rc1/datashuttle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-07 15:19:58.000000 datashuttle-0.1.0rc1/datashuttle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-07 15:19:58.000000 datashuttle-0.1.0rc1/datashuttle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:19:58.000000 datashuttle-0.1.0rc1/datashuttle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 15:19:58.000000 datashuttle-0.1.0rc1/datashuttle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-07 15:19:58.000000 datashuttle-0.1.0rc1/datashuttle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 15:19:58.000000 datashuttle-0.1.0rc1/datashuttle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/dark-logo-gatsby.png
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/dark-logo-swc.png
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/dark-logo-ucl.png
--rw-r--r--   0 runner    (1001) docker     (123)   171111 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/light-logo-gatsby.png
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/light-logo-swc.png
--rw-r--r--   0 runner    (1001) docker     (123)    39849 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/light-logo-ucl.png
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/logo_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_static/logo_light.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_templates/footer_end.html
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/_templates/footer_start.html
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/docs/source/pages/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/pages/api_index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/pages/cli_index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/pages/documentation.md
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/docs/source/pages/get_started.md
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:19:58.381699 datashuttle-0.1.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/ssh_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/tests/tests_integration/
--rw-r--r--   0 runner    (1001) docker     (123)    23408 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_command_line_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_file_conflicts_pathtable.py
--rw-r--r--   0 runner    (1001) docker     (123)    20185 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_filesystem_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    18319 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_make_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_ssh_file_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_integration/test_ssh_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:19:58.377699 datashuttle-0.1.0rc1/tests/tests_unit/
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tests/tests_unit/test_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-07 15:19:50.000000 datashuttle-0.1.0rc1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.729164 datashuttle-0.1.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.721164 datashuttle-0.1.0rc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.725164 datashuttle-0.1.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/.github/workflows/code_test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/.github/workflows/docs_build_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-07 15:43:19.729164 datashuttle-0.1.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.725164 datashuttle-0.1.0rc2/datashuttle/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31473 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/command_line_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.725164 datashuttle-0.1.0rc2/datashuttle/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/configs/canonical_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/configs/canonical_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/configs/canonical_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/configs/config_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/configs/load_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43692 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/datashuttle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.725164 datashuttle-0.1.0rc2/datashuttle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/utils/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/utils/ds_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/utils/folder_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16658 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/utils/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/utils/rclone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/utils/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/datashuttle/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.725164 datashuttle-0.1.0rc2/datashuttle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-07 15:43:19.000000 datashuttle-0.1.0rc2/datashuttle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-07 15:43:19.000000 datashuttle-0.1.0rc2/datashuttle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:43:19.000000 datashuttle-0.1.0rc2/datashuttle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 15:43:19.000000 datashuttle-0.1.0rc2/datashuttle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-07 15:43:19.000000 datashuttle-0.1.0rc2/datashuttle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 15:43:19.000000 datashuttle-0.1.0rc2/datashuttle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.725164 datashuttle-0.1.0rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.725164 datashuttle-0.1.0rc2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.729164 datashuttle-0.1.0rc2/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.729164 datashuttle-0.1.0rc2/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/_static/dark-logo-gatsby.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/_static/dark-logo-swc.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/_static/dark-logo-ucl.png
+-rw-r--r--   0 runner    (1001) docker     (123)   171111 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/_static/light-logo-gatsby.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/_static/light-logo-swc.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39849 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/_static/light-logo-ucl.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/_static/logo_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/_static/logo_light.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.729164 datashuttle-0.1.0rc2/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/_templates/footer_end.html
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/_templates/footer_start.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.729164 datashuttle-0.1.0rc2/docs/source/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/pages/api_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/pages/cli_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/pages/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/docs/source/pages/get_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:43:19.729164 datashuttle-0.1.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.729164 datashuttle-0.1.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tests/ssh_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.729164 datashuttle-0.1.0rc2/tests/tests_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)    23408 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tests/tests_integration/test_command_line_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tests/tests_integration/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tests/tests_integration/test_file_conflicts_pathtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20185 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tests/tests_integration/test_filesystem_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tests/tests_integration/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18319 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tests/tests_integration/test_make_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tests/tests_integration/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tests/tests_integration/test_ssh_file_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tests/tests_integration/test_ssh_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:43:19.729164 datashuttle-0.1.0rc2/tests/tests_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tests/tests_unit/test_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-07 15:43:10.000000 datashuttle-0.1.0rc2/tox.ini
```

### Comparing `datashuttle-0.1.0rc1/.flake8` & `datashuttle-0.1.0rc2/.flake8`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/.github/workflows/code_test_and_deploy.yml` & `datashuttle-0.1.0rc2/.github/workflows/code_test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/.github/workflows/docs_build_and_deploy.yml` & `datashuttle-0.1.0rc2/.github/workflows/docs_build_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/.gitignore` & `datashuttle-0.1.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/.pre-commit-config.yaml` & `datashuttle-0.1.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/LICENSE` & `datashuttle-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/PKG-INFO` & `datashuttle-0.1.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datashuttle
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: Organise and transfer scientific projects in BIDS format
 Author-email: Joe Ziminski <j.ziminski@ucl.ac.uk>, Adam Tyson <code@adamltyson.com>, Niko Sirmpilatze <niko.sirbiladze@gmail.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/neuroinformatics-unit/datashuttle
 Project-URL: bug_tracker, https://github.com/neuroinformatics-unit/datashuttle/issues
 Project-URL: documentation, https://github.com/neuroinformatics-unit/datashuttle
 Project-URL: source_code, https://github.com/neuroinformatics-unit/datashuttle
```

### Comparing `datashuttle-0.1.0rc1/README.md` & `datashuttle-0.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/command_line_interface.py` & `datashuttle-0.1.0rc2/datashuttle/command_line_interface.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/configs/canonical_configs.py` & `datashuttle-0.1.0rc2/datashuttle/configs/canonical_configs.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/configs/canonical_folders.py` & `datashuttle-0.1.0rc2/datashuttle/configs/canonical_folders.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/configs/config_class.py` & `datashuttle-0.1.0rc2/datashuttle/configs/config_class.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/configs/load_configs.py` & `datashuttle-0.1.0rc2/datashuttle/configs/load_configs.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/datashuttle.py` & `datashuttle-0.1.0rc2/datashuttle/datashuttle.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/utils/data_transfer.py` & `datashuttle-0.1.0rc2/datashuttle/utils/data_transfer.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/utils/decorators.py` & `datashuttle-0.1.0rc2/datashuttle/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/utils/ds_logger.py` & `datashuttle-0.1.0rc2/datashuttle/utils/ds_logger.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/utils/folders.py` & `datashuttle-0.1.0rc2/datashuttle/utils/folders.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/utils/formatting.py` & `datashuttle-0.1.0rc2/datashuttle/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/utils/rclone.py` & `datashuttle-0.1.0rc2/datashuttle/utils/rclone.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/utils/ssh.py` & `datashuttle-0.1.0rc2/datashuttle/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle/utils/utils.py` & `datashuttle-0.1.0rc2/datashuttle/utils/utils.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/datashuttle.egg-info/PKG-INFO` & `datashuttle-0.1.0rc2/datashuttle.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datashuttle
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: Organise and transfer scientific projects in BIDS format
 Author-email: Joe Ziminski <j.ziminski@ucl.ac.uk>, Adam Tyson <code@adamltyson.com>, Niko Sirmpilatze <niko.sirbiladze@gmail.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/neuroinformatics-unit/datashuttle
 Project-URL: bug_tracker, https://github.com/neuroinformatics-unit/datashuttle/issues
 Project-URL: documentation, https://github.com/neuroinformatics-unit/datashuttle
 Project-URL: source_code, https://github.com/neuroinformatics-unit/datashuttle
```

### Comparing `datashuttle-0.1.0rc1/datashuttle.egg-info/SOURCES.txt` & `datashuttle-0.1.0rc2/datashuttle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/Makefile` & `datashuttle-0.1.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/make.bat` & `datashuttle-0.1.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/_static/css/custom.css` & `datashuttle-0.1.0rc2/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/_static/dark-logo-gatsby.png` & `datashuttle-0.1.0rc2/docs/source/_static/dark-logo-gatsby.png`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/_static/dark-logo-swc.png` & `datashuttle-0.1.0rc2/docs/source/_static/dark-logo-swc.png`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/_static/dark-logo-ucl.png` & `datashuttle-0.1.0rc2/docs/source/_static/dark-logo-ucl.png`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/_static/light-logo-gatsby.png` & `datashuttle-0.1.0rc2/docs/source/_static/light-logo-gatsby.png`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/_static/light-logo-swc.png` & `datashuttle-0.1.0rc2/docs/source/_static/light-logo-swc.png`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/_static/light-logo-ucl.png` & `datashuttle-0.1.0rc2/docs/source/_static/light-logo-ucl.png`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/_static/logo_dark.png` & `datashuttle-0.1.0rc2/docs/source/_static/logo_dark.png`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/_static/logo_light.png` & `datashuttle-0.1.0rc2/docs/source/_static/logo_light.png`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/_templates/footer_end.html` & `datashuttle-0.1.0rc2/docs/source/_templates/footer_end.html`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/conf.py` & `datashuttle-0.1.0rc2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/index.md` & `datashuttle-0.1.0rc2/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/pages/documentation.md` & `datashuttle-0.1.0rc2/docs/source/pages/documentation.md`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/docs/source/pages/get_started.md` & `datashuttle-0.1.0rc2/docs/source/pages/get_started.md`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/pyproject.toml` & `datashuttle-0.1.0rc2/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 dependencies = [
     "paramiko",
     "PyYAML",
     "requests",
     "rich",
     "fancylog[git]",
+    "simplejson",
 ]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
@@ -46,15 +47,14 @@
     "tox",
     "black",
     "isort",
     "mypy",
     "pre-commit",
     "flake8",
     "setuptools_scm",
-    "simplejson",
     "types-requests",
     "types-PyYAML",
     "types-appdirs",
     "types-paramiko",
     "types-simplejson",
 ]
```

### Comparing `datashuttle-0.1.0rc1/tests/conftest.py` & `datashuttle-0.1.0rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/tests/ssh_test_utils.py` & `datashuttle-0.1.0rc2/tests/ssh_test_utils.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/tests/test_utils.py` & `datashuttle-0.1.0rc2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/tests/tests_integration/test_command_line_interface.py` & `datashuttle-0.1.0rc2/tests/tests_integration/test_command_line_interface.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/tests/tests_integration/test_configs.py` & `datashuttle-0.1.0rc2/tests/tests_integration/test_configs.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/tests/tests_integration/test_file_conflicts_pathtable.py` & `datashuttle-0.1.0rc2/tests/tests_integration/test_file_conflicts_pathtable.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/tests/tests_integration/test_filesystem_transfer.py` & `datashuttle-0.1.0rc2/tests/tests_integration/test_filesystem_transfer.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/tests/tests_integration/test_logging.py` & `datashuttle-0.1.0rc2/tests/tests_integration/test_logging.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/tests/tests_integration/test_make_folders.py` & `datashuttle-0.1.0rc2/tests/tests_integration/test_make_folders.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/tests/tests_integration/test_settings.py` & `datashuttle-0.1.0rc2/tests/tests_integration/test_settings.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/tests/tests_integration/test_ssh_file_transfer.py` & `datashuttle-0.1.0rc2/tests/tests_integration/test_ssh_file_transfer.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/tests/tests_integration/test_ssh_setup.py` & `datashuttle-0.1.0rc2/tests/tests_integration/test_ssh_setup.py`

 * *Files identical despite different names*

### Comparing `datashuttle-0.1.0rc1/tests/tests_unit/test_unit.py` & `datashuttle-0.1.0rc2/tests/tests_unit/test_unit.py`

 * *Files identical despite different names*

