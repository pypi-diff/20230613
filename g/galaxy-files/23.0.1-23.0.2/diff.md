# Comparing `tmp/galaxy-files-23.0.1.tar.gz` & `tmp/galaxy-files-23.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/files/dist/.tmp-4kd67fqu/galaxy-files-23.0.1.tar", last modified: Thu Jun  8 17:38:42 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/files/dist/.tmp-5pgmdcpx/galaxy-files-23.0.2.tar", last modified: Tue Jun 13 17:06:22 2023, max compression
```

## Comparing `galaxy-files-23.0.1.tar` & `galaxy-files-23.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-files-23.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy/files/
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy/files/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/_pyfilesystem2.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/anvil.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/basespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/galaxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/googlecloudstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/onedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/posix.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/s3fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/sources/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy/files/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/files/uris.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/galaxy_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-08 17:38:42.000000 galaxy-files-23.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 17:37:04.000000 galaxy-files-23.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:22.000000 galaxy-files-23.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-13 17:04:36.000000 galaxy-files-23.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-13 17:06:22.000000 galaxy-files-23.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:22.000000 galaxy-files-23.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:22.000000 galaxy-files-23.0.2/galaxy/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:22.000000 galaxy-files-23.0.2/galaxy/files/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/_pyfilesystem2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/anvil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/basespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/googlecloudstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/onedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/s3fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/sources/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:22.000000 galaxy-files-23.0.2/galaxy/files/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/files/uris.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:06:22.000000 galaxy-files-23.0.2/galaxy_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-13 17:06:22.000000 galaxy-files-23.0.2/galaxy_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-13 17:06:22.000000 galaxy-files-23.0.2/galaxy_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:06:22.000000 galaxy-files-23.0.2/galaxy_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 17:06:22.000000 galaxy-files-23.0.2/galaxy_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:06:22.000000 galaxy-files-23.0.2/galaxy_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-13 17:06:22.000000 galaxy-files-23.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 17:04:37.000000 galaxy-files-23.0.2/test-requirements.txt
```

### Comparing `galaxy-files-23.0.1/LICENSE.txt` & `galaxy-files-23.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.1/PKG-INFO` & `galaxy-files-23.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-files
-Version: 23.0.1
+Version: 23.0.2
 Summary: Galaxy file source framework and default plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.2 (2023-06-13)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix dropbox import to support newer versions by `@nuwang <https://github.com/nuwang>`_ in `#16239 <https://github.com/galaxyproject/galaxy/pull/16239>`_
+
+-------------------
 23.0.1 (2023-06-08)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 22.1.1 (2022-08-22)
```

### Comparing `galaxy-files-23.0.1/galaxy/files/__init__.py` & `galaxy-files-23.0.2/galaxy/files/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.1/galaxy/files/sources/__init__.py` & `galaxy-files-23.0.2/galaxy/files/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.1/galaxy/files/sources/_pyfilesystem2.py` & `galaxy-files-23.0.2/galaxy/files/sources/_pyfilesystem2.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.1/galaxy/files/sources/galaxy.py` & `galaxy-files-23.0.2/galaxy/files/sources/galaxy.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.1/galaxy/files/sources/googlecloudstorage.py` & `galaxy-files-23.0.2/galaxy/files/sources/googlecloudstorage.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.1/galaxy/files/sources/googledrive.py` & `galaxy-files-23.0.2/galaxy/files/sources/googledrive.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.1/galaxy/files/sources/posix.py` & `galaxy-files-23.0.2/galaxy/files/sources/posix.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.1/galaxy/files/sources/s3fs.py` & `galaxy-files-23.0.2/galaxy/files/sources/s3fs.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.1/galaxy/files/sources/ssh.py` & `galaxy-files-23.0.2/galaxy/files/sources/ssh.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.1/galaxy/files/unittest_utils/__init__.py` & `galaxy-files-23.0.2/galaxy/files/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.1/galaxy/files/uris.py` & `galaxy-files-23.0.2/galaxy/files/uris.py`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.1/galaxy_files.egg-info/PKG-INFO` & `galaxy-files-23.0.2/galaxy_files.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-files
-Version: 23.0.1
+Version: 23.0.2
 Summary: Galaxy file source framework and default plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.2 (2023-06-13)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix dropbox import to support newer versions by `@nuwang <https://github.com/nuwang>`_ in `#16239 <https://github.com/galaxyproject/galaxy/pull/16239>`_
+
+-------------------
 23.0.1 (2023-06-08)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 22.1.1 (2022-08-22)
```

### Comparing `galaxy-files-23.0.1/galaxy_files.egg-info/SOURCES.txt` & `galaxy-files-23.0.2/galaxy_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-files-23.0.1/setup.cfg` & `galaxy-files-23.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-files
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.1
+version = 23.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	fs
 	typing-extensions
```

