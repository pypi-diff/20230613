# Comparing `tmp/dbfs_package_sync-0.1.1.tar.gz` & `tmp/dbfs_package_sync-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbfs_package_sync-0.1.1.tar", max compression
+gzip compressed data, was "dbfs_package_sync-0.2.0.tar", max compression
```

## Comparing `dbfs_package_sync-0.1.1.tar` & `dbfs_package_sync-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     3914 2023-05-18 16:46:24.211742 dbfs_package_sync-0.1.1/README.md
--rw-r--r--   0        0        0       96 2023-05-18 16:46:24.211742 dbfs_package_sync-0.1.1/dbfsps/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 16:46:24.211742 dbfs_package_sync-0.1.1/dbfsps/cli/__init__.py
--rw-r--r--   0        0        0     5429 2023-05-18 16:46:24.211742 dbfs_package_sync-0.1.1/dbfsps/cli/databricks_sync.py
--rw-r--r--   0        0        0      915 2023-05-18 16:46:24.211742 dbfs_package_sync-0.1.1/dbfsps/cli/utils.py
--rw-r--r--   0        0        0     5807 2023-05-18 16:46:24.211742 dbfs_package_sync-0.1.1/dbfsps/filestatus.py
--rw-r--r--   0        0        0        0 2023-05-18 16:46:24.211742 dbfs_package_sync-0.1.1/dbfsps/sdk/__init__.py
--rw-r--r--   0        0        0     3919 2023-05-18 16:46:24.211742 dbfs_package_sync-0.1.1/dbfsps/sdk/config.py
--rw-r--r--   0        0        0     4951 2023-05-18 16:46:24.211742 dbfs_package_sync-0.1.1/dbfsps/sdk/dbfs.py
--rw-r--r--   0        0        0     1800 2023-05-18 16:46:24.211742 dbfs_package_sync-0.1.1/dbfsps/sdk/errors.py
--rw-r--r--   0        0        0      781 2023-05-18 16:46:24.211742 dbfs_package_sync-0.1.1/dbfsps/setupnotebook.py
--rw-r--r--   0        0        0     1714 2023-05-18 16:46:24.211742 dbfs_package_sync-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4637 1970-01-01 00:00:00.000000 dbfs_package_sync-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3830 2023-06-13 15:39:34.516711 dbfs_package_sync-0.2.0/README.md
+-rw-r--r--   0        0        0       96 2023-06-13 15:39:34.516711 dbfs_package_sync-0.2.0/dbfsps/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:39:34.516711 dbfs_package_sync-0.2.0/dbfsps/cli/__init__.py
+-rw-r--r--   0        0        0     3145 2023-06-13 15:39:34.516711 dbfs_package_sync-0.2.0/dbfsps/cli/databricks_sync.py
+-rw-r--r--   0        0        0     2441 2023-06-13 15:39:34.516711 dbfs_package_sync-0.2.0/dbfsps/cli/utils.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:39:34.516711 dbfs_package_sync-0.2.0/dbfsps/sdk/__init__.py
+-rw-r--r--   0        0        0     3919 2023-06-13 15:39:34.520711 dbfs_package_sync-0.2.0/dbfsps/sdk/config.py
+-rw-r--r--   0        0        0     4951 2023-06-13 15:39:34.520711 dbfs_package_sync-0.2.0/dbfsps/sdk/dbfs.py
+-rw-r--r--   0        0        0     1800 2023-06-13 15:39:34.520711 dbfs_package_sync-0.2.0/dbfsps/sdk/errors.py
+-rw-r--r--   0        0        0      781 2023-06-13 15:39:34.520711 dbfs_package_sync-0.2.0/dbfsps/setupnotebook.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:39:34.520711 dbfs_package_sync-0.2.0/dbfsps/syncer/__init__.py
+-rw-r--r--   0        0        0     2385 2023-06-13 15:39:34.520711 dbfs_package_sync-0.2.0/dbfsps/syncer/file.py
+-rw-r--r--   0        0        0     6594 2023-06-13 15:39:34.520711 dbfs_package_sync-0.2.0/dbfsps/syncer/plan.py
+-rw-r--r--   0        0        0     1802 2023-06-13 15:39:34.520711 dbfs_package_sync-0.2.0/dbfsps/syncer/state.py
+-rw-r--r--   0        0        0     1698 2023-06-13 15:39:34.520711 dbfs_package_sync-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4518 1970-01-01 00:00:00.000000 dbfs_package_sync-0.2.0/PKG-INFO
```

### Comparing `dbfs_package_sync-0.1.1/README.md` & `dbfs_package_sync-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 to dbfs, no more, no less. Why all the fuss?
 
 So, that's what this CLI does. When I need to test the current state of my package in some Databricks notebook,
 I run `dbfsps` and I have my local state on DBFS.
 
 **Caveats:**
 
-- Version 0.1.0 is not a very nice bit of code yet. I set it up in a bit of a rush.
 - Only works for poetry packages
 - At the top of the notebook you will of course need to install the dependencies once and set `autoreload`.
 The `dbfsps` command will send along a requirements file and create a helper notebook though, so you only need a single `%run`
 command at the top of your notebook.
 - I opted for running a single command every time you need to sync your code instead of a continuous syncing process
 running in the background. To keep track of which files need to be uploaded/removed, `dbfsps` creates a hidden 
 text file `.dbfsps_file_status`.
```

### Comparing `dbfs_package_sync-0.1.1/dbfsps/sdk/config.py` & `dbfs_package_sync-0.2.0/dbfsps/sdk/config.py`

 * *Files identical despite different names*

### Comparing `dbfs_package_sync-0.1.1/dbfsps/sdk/dbfs.py` & `dbfs_package_sync-0.2.0/dbfsps/sdk/dbfs.py`

 * *Files identical despite different names*

### Comparing `dbfs_package_sync-0.1.1/dbfsps/sdk/errors.py` & `dbfs_package_sync-0.2.0/dbfsps/sdk/errors.py`

 * *Files identical despite different names*

### Comparing `dbfs_package_sync-0.1.1/dbfsps/setupnotebook.py` & `dbfs_package_sync-0.2.0/dbfsps/setupnotebook.py`

 * *Files identical despite different names*

### Comparing `dbfs_package_sync-0.1.1/pyproject.toml` & `dbfs_package_sync-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "dbfs-package-sync"
-version = "0.1.1"
+version = "0.2.0"
 description = "Basic CLI tool that can sync a local Python package directory with a folder on dbfs"
 authors = ["Jeroen Meidam <j.meidam@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dbfsps"}]
 repository = "https://github.com/jmeidam/dbfs-package-sync"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.0"
-pandas = "^1.0"
 databricks-cli = "^0.17.7"
 
 
 [tool.poetry.group.dev.dependencies]
 coverage = {extras = ["toml"], version = "^6.4.4"}
 Sphinx = "^4.3.2"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `dbfs_package_sync-0.1.1/PKG-INFO` & `dbfs_package_sync-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: dbfs-package-sync
-Version: 0.1.1
+Version: 0.2.0
 Summary: Basic CLI tool that can sync a local Python package directory with a folder on dbfs
 Home-page: https://github.com/jmeidam/dbfs-package-sync
 Author: Jeroen Meidam
 Author-email: j.meidam@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0,<9.0)
 Requires-Dist: databricks-cli (>=0.17.7,<0.18.0)
-Requires-Dist: pandas (>=1.0,<2.0)
 Project-URL: Repository, https://github.com/jmeidam/dbfs-package-sync
 Description-Content-Type: text/markdown
 
 # dbfs-package-sync
 
 Scenario: You are developing a Python package that you need in a couple of notebooks. 
 You (of course) want to develop your package in an IDE. 
@@ -41,15 +40,14 @@
 to dbfs, no more, no less. Why all the fuss?
 
 So, that's what this CLI does. When I need to test the current state of my package in some Databricks notebook,
 I run `dbfsps` and I have my local state on DBFS.
 
 **Caveats:**
 
-- Version 0.1.0 is not a very nice bit of code yet. I set it up in a bit of a rush.
 - Only works for poetry packages
 - At the top of the notebook you will of course need to install the dependencies once and set `autoreload`.
 The `dbfsps` command will send along a requirements file and create a helper notebook though, so you only need a single `%run`
 command at the top of your notebook.
 - I opted for running a single command every time you need to sync your code instead of a continuous syncing process
 running in the background. To keep track of which files need to be uploaded/removed, `dbfsps` creates a hidden 
 text file `.dbfsps_file_status`.
```

