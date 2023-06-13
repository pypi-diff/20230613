# Comparing `tmp/galaxy-release-util-0.1.1.tar.gz` & `tmp/galaxy-release-util-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-release-util-0.1.1.tar", last modified: Tue Jun 13 13:18:45 2023, max compression
+gzip compressed data, was "galaxy-release-util-0.1.2.tar", last modified: Tue Jun 13 16:50:29 2023, max compression
```

## Comparing `galaxy-release-util-0.1.1.tar` & `galaxy-release-util-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:18:45.666021 galaxy-release-util-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-13 13:18:45.666021 galaxy-release-util-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:18:45.662021 galaxy-release-util-0.1.1/galaxy_release_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/galaxy_release_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22421 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/galaxy_release_util/bootstrap_history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:18:45.666021 galaxy-release-util-0.1.1/galaxy_release_util/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/galaxy_release_util/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/galaxy_release_util/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/galaxy_release_util/cli/release_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/galaxy_release_util/github_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/galaxy_release_util/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    26195 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/galaxy_release_util/point_release.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/galaxy_release_util/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:18:45.666021 galaxy-release-util-0.1.1/galaxy_release_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-13 13:18:45.000000 galaxy-release-util-0.1.1/galaxy_release_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-13 13:18:45.000000 galaxy-release-util-0.1.1/galaxy_release_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:18:45.000000 galaxy-release-util-0.1.1/galaxy_release_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 13:18:45.000000 galaxy-release-util-0.1.1/galaxy_release_util.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 13:18:45.000000 galaxy-release-util-0.1.1/galaxy_release_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 13:18:45.000000 galaxy-release-util-0.1.1/galaxy_release_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-13 13:18:45.666021 galaxy-release-util-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:18:45.666021 galaxy-release-util-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-13 13:18:35.000000 galaxy-release-util-0.1.1/tests/test_release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:28.999202 galaxy-release-util-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-13 16:50:28.999202 galaxy-release-util-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:28.995202 galaxy-release-util-0.1.2/galaxy_release_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/galaxy_release_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22421 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/galaxy_release_util/bootstrap_history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:28.999202 galaxy-release-util-0.1.2/galaxy_release_util/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/galaxy_release_util/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/galaxy_release_util/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/galaxy_release_util/cli/release_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/galaxy_release_util/github_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/galaxy_release_util/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26254 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/galaxy_release_util/point_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/galaxy_release_util/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:28.999202 galaxy-release-util-0.1.2/galaxy_release_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-13 16:50:28.000000 galaxy-release-util-0.1.2/galaxy_release_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-13 16:50:28.000000 galaxy-release-util-0.1.2/galaxy_release_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:50:28.000000 galaxy-release-util-0.1.2/galaxy_release_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 16:50:28.000000 galaxy-release-util-0.1.2/galaxy_release_util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 16:50:28.000000 galaxy-release-util-0.1.2/galaxy_release_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 16:50:28.000000 galaxy-release-util-0.1.2/galaxy_release_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-13 16:50:28.999202 galaxy-release-util-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:50:28.999202 galaxy-release-util-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-13 16:50:18.000000 galaxy-release-util-0.1.2/tests/test_release.py
```

### Comparing `galaxy-release-util-0.1.1/LICENSE.txt` & `galaxy-release-util-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.1/PKG-INFO` & `galaxy-release-util-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-release-util
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utlity for various tasks around creating Galaxy releases
 Home-page: https://github.com/galaxyproject/galaxy-release-util
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -55,14 +55,19 @@
 
 History
 -------
 
 .. to_doc
 
 ------------------
+0.1.2 (12-06-2023)
+------------------
+* Fix isinstance assertion
+
+------------------
 0.1.1 (12-06-2023)
 ------------------
 * Add simplified makefile, development instruction
 * Fix project description
 
 ------------------
 0.1.0 (12-06-2023)
```

### Comparing `galaxy-release-util-0.1.1/README.rst` & `galaxy-release-util-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.1/galaxy_release_util/bootstrap_history.py` & `galaxy-release-util-0.1.2/galaxy_release_util/bootstrap_history.py`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.1/galaxy_release_util/cli/options.py` & `galaxy-release-util-0.1.2/galaxy_release_util/cli/options.py`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.1/galaxy_release_util/github_client.py` & `galaxy-release-util-0.1.2/galaxy_release_util/github_client.py`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.1/galaxy_release_util/metadata.py` & `galaxy-release-util-0.1.2/galaxy_release_util/metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.1/galaxy_release_util/point_release.py` & `galaxy-release-util-0.1.2/galaxy_release_util/point_release.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     Parser().parse(package.history_rst.read_text(), document)
     changelog_items: List[ChangelogItem] = []
     root_section = document[0]
     assert isinstance(root_section, docutils.nodes.section)
     assert root_section.tagname == "section"
     for release in root_section.children:
         # ignore title and comment
-        assert isinstance(release, docutils.nodes.title)
+        assert isinstance(release, (docutils.nodes.title, docutils.nodes.comment, docutils.nodes.section)), release
         if release.tagname == "section":
             assert release[0].tagname == "title"
             release_version = release[0].astext()
             current_date = None
             if " (" in release_version:
                 version_str, current_date = release_version.split(" (")
                 current_date = current_date.split(")")[0]
```

### Comparing `galaxy-release-util-0.1.1/galaxy_release_util.egg-info/PKG-INFO` & `galaxy-release-util-0.1.2/galaxy_release_util.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-release-util
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utlity for various tasks around creating Galaxy releases
 Home-page: https://github.com/galaxyproject/galaxy-release-util
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -55,14 +55,19 @@
 
 History
 -------
 
 .. to_doc
 
 ------------------
+0.1.2 (12-06-2023)
+------------------
+* Fix isinstance assertion
+
+------------------
 0.1.1 (12-06-2023)
 ------------------
 * Add simplified makefile, development instruction
 * Fix project description
 
 ------------------
 0.1.0 (12-06-2023)
```

### Comparing `galaxy-release-util-0.1.1/galaxy_release_util.egg-info/SOURCES.txt` & `galaxy-release-util-0.1.2/galaxy_release_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-release-util-0.1.1/setup.cfg` & `galaxy-release-util-0.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-release-util
 url = https://github.com/galaxyproject/galaxy-release-util
-version = 0.1.1
+version = 0.1.2
 
 [options]
 include_package_data = True
 install_requires = 
 	build
 	click
 	docutils
```

### Comparing `galaxy-release-util-0.1.1/tests/test_release.py` & `galaxy-release-util-0.1.2/tests/test_release.py`

 * *Files identical despite different names*

