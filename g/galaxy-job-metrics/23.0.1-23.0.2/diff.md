# Comparing `tmp/galaxy-job-metrics-23.0.1.tar.gz` & `tmp/galaxy-job-metrics-23.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/job_metrics/dist/.tmp-k82uluf6/galaxy-job-metrics-23.0.1.tar", last modified: Thu Jun  8 17:39:12 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/job_metrics/dist/.tmp-e5z37yem/galaxy-job-metrics-23.0.2.tar", last modified: Tue Jun 13 17:06:54 2023, max compression
```

## Comparing `galaxy-job-metrics-23.0.1.tar` & `galaxy-job-metrics-23.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-job-metrics-23.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/cgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/cpuinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/meminfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/uname.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/safety.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:54.000000 galaxy-job-metrics-23.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-13 17:04:36.000000 galaxy-job-metrics-23.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-13 17:06:54.000000 galaxy-job-metrics-23.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:54.000000 galaxy-job-metrics-23.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:54.000000 galaxy-job-metrics-23.0.2/galaxy/job_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/galaxy/job_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/galaxy/job_metrics/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:54.000000 galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/cgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/cpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/meminfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/uname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/galaxy/job_metrics/safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:54.000000 galaxy-job-metrics-23.0.2/galaxy_job_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-13 17:06:54.000000 galaxy-job-metrics-23.0.2/galaxy_job_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-13 17:06:54.000000 galaxy-job-metrics-23.0.2/galaxy_job_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:06:54.000000 galaxy-job-metrics-23.0.2/galaxy_job_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 17:06:54.000000 galaxy-job-metrics-23.0.2/galaxy_job_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:06:54.000000 galaxy-job-metrics-23.0.2/galaxy_job_metrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-13 17:06:54.000000 galaxy-job-metrics-23.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:04:37.000000 galaxy-job-metrics-23.0.2/test-requirements.txt
```

### Comparing `galaxy-job-metrics-23.0.1/LICENSE` & `galaxy-job-metrics-23.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.0.1/PKG-INFO` & `galaxy-job-metrics-23.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-job-metrics
-Version: 23.0.1
+Version: 23.0.2
 Summary: Galaxy job metrics
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.2 (2023-06-13)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.1 (2023-06-08)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 20.9.0 (2020-10-15)
```

### Comparing `galaxy-job-metrics-23.0.1/galaxy/job_metrics/__init__.py` & `galaxy-job-metrics-23.0.2/galaxy/job_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.0.1/galaxy/job_metrics/formatting.py` & `galaxy-job-metrics-23.0.2/galaxy/job_metrics/formatting.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/__init__.py` & `galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/cgroup.py` & `galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/cgroup.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/core.py` & `galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/core.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/cpuinfo.py` & `galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/env.py` & `galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/env.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/hostname.py` & `galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/hostname.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/meminfo.py` & `galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/meminfo.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/uname.py` & `galaxy-job-metrics-23.0.2/galaxy/job_metrics/instrumenters/uname.py`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/PKG-INFO` & `galaxy-job-metrics-23.0.2/galaxy_job_metrics.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-job-metrics
-Version: 23.0.1
+Version: 23.0.2
 Summary: Galaxy job metrics
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.2 (2023-06-13)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.1 (2023-06-08)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 20.9.0 (2020-10-15)
```

### Comparing `galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/SOURCES.txt` & `galaxy-job-metrics-23.0.2/galaxy_job_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-job-metrics-23.0.1/setup.cfg` & `galaxy-job-metrics-23.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-job-metrics
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.1
+version = 23.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 packages = find:
 python_requires = >=3.7
```

