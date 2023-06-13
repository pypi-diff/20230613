# Comparing `tmp/dvc-task-0.2.1.tar.gz` & `tmp/dvc-task-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-task-0.2.1.tar", last modified: Thu Apr 27 09:22:22 2023, max compression
+gzip compressed data, was "dvc-task-0.3.0.tar", last modified: Tue Jun 13 09:21:10 2023, max compression
```

## Comparing `dvc-task-0.2.1.tar` & `dvc-task-0.3.0.tar`

### file list

```diff
@@ -1,71 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.138275 dvc-task-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.130275 dvc-task-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-27 09:21:37.000000 dvc-task-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-27 09:21:37.000000 dvc-task-0.2.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-27 09:21:37.000000 dvc-task-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-27 09:21:37.000000 dvc-task-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-27 09:22:22.138275 dvc-task-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-27 09:21:37.000000 dvc-task-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-27 09:21:37.000000 dvc-task-0.2.1/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-27 09:21:37.000000 dvc-task-0.2.1/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-27 09:21:37.000000 dvc-task-0.2.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-27 09:21:37.000000 dvc-task-0.2.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-27 09:21:37.000000 dvc-task-0.2.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-27 09:21:37.000000 dvc-task-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-27 09:22:22.138275 dvc-task-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.130275 dvc-task-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/src/dvc_task/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/src/dvc_task/app/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/app/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/src/dvc_task/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/contrib/kombu_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/src/dvc_task/proc/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/proc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/proc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/proc/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/proc/process.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/proc/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/src/dvc_task/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-27 09:21:37.000000 dvc-task-0.2.1/src/dvc_task/worker/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.134275 dvc-task-0.2.1/src/dvc_task.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-27 09:22:22.000000 dvc-task-0.2.1/src/dvc_task.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-27 09:22:22.000000 dvc-task-0.2.1/src/dvc_task.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:22:22.000000 dvc-task-0.2.1/src/dvc_task.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:22:21.000000 dvc-task-0.2.1/src/dvc_task.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 09:22:22.000000 dvc-task-0.2.1/src/dvc_task.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 09:22:22.000000 dvc-task-0.2.1/src/dvc_task.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.138275 dvc-task-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.138275 dvc-task-0.2.1/tests/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/app/test_filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.138275 dvc-task-0.2.1/tests/proc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/proc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/proc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/proc/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/proc/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/proc/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/test_dvc_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:22:22.138275 dvc-task-0.2.1/tests/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-27 09:21:37.000000 dvc-task-0.2.1/tests/worker/test_temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.813262 dvc-task-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-13 09:20:47.000000 dvc-task-0.3.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 09:20:47.000000 dvc-task-0.3.0/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 09:20:47.000000 dvc-task-0.3.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.809261 dvc-task-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-13 09:20:47.000000 dvc-task-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.809261 dvc-task-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-13 09:20:47.000000 dvc-task-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-13 09:20:47.000000 dvc-task-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-13 09:20:47.000000 dvc-task-0.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-13 09:20:47.000000 dvc-task-0.3.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-13 09:20:47.000000 dvc-task-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-13 09:20:47.000000 dvc-task-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-13 09:20:47.000000 dvc-task-0.3.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-13 09:20:47.000000 dvc-task-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-13 09:20:47.000000 dvc-task-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-06-13 09:21:10.813262 dvc-task-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-06-13 09:20:47.000000 dvc-task-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.809261 dvc-task-0.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.809261 dvc-task-0.3.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-13 09:20:47.000000 dvc-task-0.3.0/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 09:20:47.000000 dvc-task-0.3.0/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-13 09:20:47.000000 dvc-task-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 09:20:47.000000 dvc-task-0.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-13 09:20:47.000000 dvc-task-0.3.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-13 09:20:47.000000 dvc-task-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-13 09:21:10.817262 dvc-task-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.809261 dvc-task-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.813262 dvc-task-0.3.0/src/dvc_task/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 09:20:47.000000 dvc-task-0.3.0/src/dvc_task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.813262 dvc-task-0.3.0/src/dvc_task/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 09:20:47.000000 dvc-task-0.3.0/src/dvc_task/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-06-13 09:20:47.000000 dvc-task-0.3.0/src/dvc_task/app/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 09:20:47.000000 dvc-task-0.3.0/src/dvc_task/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.813262 dvc-task-0.3.0/src/dvc_task/proc/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 09:20:47.000000 dvc-task-0.3.0/src/dvc_task/proc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-13 09:20:47.000000 dvc-task-0.3.0/src/dvc_task/proc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-06-13 09:20:47.000000 dvc-task-0.3.0/src/dvc_task/proc/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-06-13 09:20:47.000000 dvc-task-0.3.0/src/dvc_task/proc/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-13 09:20:47.000000 dvc-task-0.3.0/src/dvc_task/proc/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:20:47.000000 dvc-task-0.3.0/src/dvc_task/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-13 09:20:47.000000 dvc-task-0.3.0/src/dvc_task/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.813262 dvc-task-0.3.0/src/dvc_task/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 09:20:47.000000 dvc-task-0.3.0/src/dvc_task/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-06-13 09:20:47.000000 dvc-task-0.3.0/src/dvc_task/worker/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.813262 dvc-task-0.3.0/src/dvc_task.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-06-13 09:21:10.000000 dvc-task-0.3.0/src/dvc_task.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-13 09:21:10.000000 dvc-task-0.3.0/src/dvc_task.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:21:10.000000 dvc-task-0.3.0/src/dvc_task.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:21:10.000000 dvc-task-0.3.0/src/dvc_task.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-13 09:21:10.000000 dvc-task-0.3.0/src/dvc_task.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 09:21:10.000000 dvc-task-0.3.0/src/dvc_task.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.813262 dvc-task-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 09:20:47.000000 dvc-task-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.813262 dvc-task-0.3.0/tests/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:20:47.000000 dvc-task-0.3.0/tests/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-06-13 09:20:47.000000 dvc-task-0.3.0/tests/app/test_filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.813262 dvc-task-0.3.0/tests/proc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:20:47.000000 dvc-task-0.3.0/tests/proc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-13 09:20:47.000000 dvc-task-0.3.0/tests/proc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-13 09:20:47.000000 dvc-task-0.3.0/tests/proc/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-13 09:20:47.000000 dvc-task-0.3.0/tests/proc/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-13 09:20:47.000000 dvc-task-0.3.0/tests/proc/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-13 09:20:47.000000 dvc-task-0.3.0/tests/test_dvc_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-13 09:20:47.000000 dvc-task-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:10.813262 dvc-task-0.3.0/tests/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:20:47.000000 dvc-task-0.3.0/tests/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-13 09:20:47.000000 dvc-task-0.3.0/tests/worker/test_temporary.py
```

### Comparing `dvc-task-0.2.1/.cruft.json` & `dvc-task-0.3.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/.github/dependabot.yml` & `dvc-task-0.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/.github/workflows/docs.yml` & `dvc-task-0.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/.github/workflows/release.yml` & `dvc-task-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/.github/workflows/tests.yml` & `dvc-task-0.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/.gitignore` & `dvc-task-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/.pre-commit-config.yaml` & `dvc-task-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/CODE_OF_CONDUCT.rst` & `dvc-task-0.3.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/CONTRIBUTING.rst` & `dvc-task-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/LICENSE` & `dvc-task-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/PKG-INFO` & `dvc-task-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-task
-Version: 0.2.1
+Version: 0.3.0
 Summary: Extensible task queue used in DVC.
 Home-page: https://github.com/iterative/dvc-task
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-task-0.2.1/README.rst` & `dvc-task-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/docs/assets/logo.svg` & `dvc-task-0.3.0/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/docs/gen_ref_pages.py` & `dvc-task-0.3.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/mkdocs.yml` & `dvc-task-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/noxfile.py` & `dvc-task-0.3.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/pyproject.toml` & `dvc-task-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 [tool.pytest.ini_options]
 addopts = "-ra"
 
 [tool.coverage.run]
 branch = true
 source = ["dvc_task", "tests"]
-omit = ["dvc_task/contrib/*"]
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 exclude_lines = [
@@ -59,29 +58,24 @@
 pretty = true
 check_untyped_defs = false
 # Warnings
 warn_no_return = true
 warn_redundant_casts = true
 warn_unreachable = true
 files = ["src", "tests"]
-exclude = ["^src/dvc_task/contrib"]
 
 [[tool.mypy.overrides]]
 module = [
     "celery.*",
     "funcy.*",
     "shortuuid",
-    "kombu.message.*",
-    "kombu.utils.*",
+    "kombu.*",
 ]
 ignore_missing_imports = true
 
-[tool.pylint.master]
-ignore-paths = ["src/dvc_task/contrib"]
-
 [tool.pylint.format]
 max-line-length = 88
 
 [tool.pylint.message_control]
 enable = ["c-extension-no-member", "no-else-return"]
 
 [tool.pylint.variables]
```

### Comparing `dvc-task-0.2.1/setup.cfg` & `dvc-task-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -20,38 +20,38 @@
 [options]
 python_requires = >=3.8
 zip_safe = False
 package_dir = 
 	=src
 packages = find:
 install_requires = 
-	celery>=5.2.0,<6
-	kombu>=5.2.0,<6
+	celery>=5.3.0,<6
+	kombu>=5.3.0,<6
 	funcy>=1.17
 	shortuuid>=1.0.8
 	pywin32>=225; sys_platform == 'win32'
 
 [options.extras_require]
 docs = 
 	mkdocs==1.3.1
 	mkdocs-gen-files==0.3.5
 	mkdocs-material==8.4.1
 	mkdocs-section-index==0.3.4
 	mkdocstrings-python==0.7.1
 tests = 
 	pytest==7.2.0
-	pytest-sugar==0.9.5
+	pytest-sugar==0.9.6
 	pytest-cov==3.0.0
 	pytest-mock==3.8.2
 	pylint==2.15.0
 	mypy==0.971
 	flaky==3.7.0
 	pytest-test-utils>=0.0.6
 	pytest-celery
-	celery-types>=0.11.0
+	celery-types==0.15.0
 dev = 
 	%(tests)s
 	%(docs)s
 
 [options.packages.find]
 exclude = 
 	tests
```

### Comparing `dvc-task-0.2.1/src/dvc_task/app/filesystem.py` & `dvc-task-0.3.0/src/dvc_task/app/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,31 +2,23 @@
 import logging
 import os
 from datetime import datetime
 from typing import Any, Dict, Iterable, Iterator, List, Optional, Set, cast
 
 from celery import Celery
 from kombu.message import Message
+from kombu.transport.filesystem import LOCK_SH, lock, unlock
 from kombu.utils.encoding import bytes_to_str
 from kombu.utils.json import loads
 
-from ..contrib.kombu_filesystem import (
-    LOCK_SH,
-    backport_filesystem_transport,
-    lock,
-    unlock,
-)
 from ..utils import makedirs, remove, unc_path
 
 logger = logging.getLogger(__name__)
 
 
-backport_filesystem_transport()
-
-
 def _get_fs_config(
     wdir: str,
     mkdir: bool = False,
     task_serializer: str = "json",
     result_serializer: str = "json",
 ) -> Dict[str, Any]:
     broker_path = os.path.join(wdir, "broker")
@@ -117,15 +109,15 @@
 
         Arguments:
             folder_name: the folder to iterate
             path_cache: cache of message path.
             queue: Optional name of queue.
         """
         with self.connection_for_read() as conn:  # type: ignore[attr-defined]
-            with conn.channel() as channel:
+            with conn.channel() as channel:  # type: ignore[attr-defined]
                 folder = getattr(channel, folder_name)
                 for filename in sorted(os.listdir(folder)):
                     path = os.path.join(folder, filename)
                     try:
                         with open(path, "rb") as fobj:
                             lock(fobj, LOCK_SH)
                             try:
```

### Comparing `dvc-task-0.2.1/src/dvc_task/proc/exceptions.py` & `dvc-task-0.3.0/src/dvc_task/proc/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/src/dvc_task/proc/manager.py` & `dvc-task-0.3.0/src/dvc_task/proc/manager.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/src/dvc_task/proc/process.py` & `dvc-task-0.3.0/src/dvc_task/proc/process.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/src/dvc_task/utils.py` & `dvc-task-0.3.0/src/dvc_task/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/src/dvc_task/worker/temporary.py` & `dvc-task-0.3.0/src/dvc_task/worker/temporary.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/src/dvc_task.egg-info/PKG-INFO` & `dvc-task-0.3.0/src/dvc_task.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-task
-Version: 0.2.1
+Version: 0.3.0
 Summary: Extensible task queue used in DVC.
 Home-page: https://github.com/iterative/dvc-task
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-task-0.2.1/src/dvc_task.egg-info/SOURCES.txt` & `dvc-task-0.3.0/src/dvc_task.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,16 +27,14 @@
 src/dvc_task.egg-info/SOURCES.txt
 src/dvc_task.egg-info/dependency_links.txt
 src/dvc_task.egg-info/not-zip-safe
 src/dvc_task.egg-info/requires.txt
 src/dvc_task.egg-info/top_level.txt
 src/dvc_task/app/__init__.py
 src/dvc_task/app/filesystem.py
-src/dvc_task/contrib/__init__.py
-src/dvc_task/contrib/kombu_filesystem.py
 src/dvc_task/proc/__init__.py
 src/dvc_task/proc/exceptions.py
 src/dvc_task/proc/manager.py
 src/dvc_task/proc/process.py
 src/dvc_task/proc/tasks.py
 src/dvc_task/worker/__init__.py
 src/dvc_task/worker/temporary.py
```

### Comparing `dvc-task-0.2.1/src/dvc_task.egg-info/requires.txt` & `dvc-task-0.3.0/src/dvc_task.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-celery<6,>=5.2.0
-kombu<6,>=5.2.0
+celery<6,>=5.3.0
+kombu<6,>=5.3.0
 funcy>=1.17
 shortuuid>=1.0.8
 
 [:sys_platform == "win32"]
 pywin32>=225
 
 [dev]
 pytest==7.2.0
-pytest-sugar==0.9.5
+pytest-sugar==0.9.6
 pytest-cov==3.0.0
 pytest-mock==3.8.2
 pylint==2.15.0
 mypy==0.971
 flaky==3.7.0
 pytest-test-utils>=0.0.6
 pytest-celery
-celery-types>=0.11.0
+celery-types==0.15.0
 mkdocs==1.3.1
 mkdocs-gen-files==0.3.5
 mkdocs-material==8.4.1
 mkdocs-section-index==0.3.4
 mkdocstrings-python==0.7.1
 
 [docs]
@@ -28,16 +28,16 @@
 mkdocs-gen-files==0.3.5
 mkdocs-material==8.4.1
 mkdocs-section-index==0.3.4
 mkdocstrings-python==0.7.1
 
 [tests]
 pytest==7.2.0
-pytest-sugar==0.9.5
+pytest-sugar==0.9.6
 pytest-cov==3.0.0
 pytest-mock==3.8.2
 pylint==2.15.0
 mypy==0.971
 flaky==3.7.0
 pytest-test-utils>=0.0.6
 pytest-celery
-celery-types>=0.11.0
+celery-types==0.15.0
```

### Comparing `dvc-task-0.2.1/tests/app/test_filesystem.py` & `dvc-task-0.3.0/tests/app/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/tests/proc/conftest.py` & `dvc-task-0.3.0/tests/proc/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/tests/proc/test_manager.py` & `dvc-task-0.3.0/tests/proc/test_manager.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/tests/proc/test_process.py` & `dvc-task-0.3.0/tests/proc/test_process.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/tests/proc/test_tasks.py` & `dvc-task-0.3.0/tests/proc/test_tasks.py`

 * *Files identical despite different names*

### Comparing `dvc-task-0.2.1/tests/worker/test_temporary.py` & `dvc-task-0.3.0/tests/worker/test_temporary.py`

 * *Files identical despite different names*

