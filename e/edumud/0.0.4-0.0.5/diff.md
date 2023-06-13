# Comparing `tmp/edumud-0.0.4.tar.gz` & `tmp/edumud-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edumud-0.0.4.tar", last modified: Tue Jun 13 12:17:26 2023, max compression
+gzip compressed data, was "edumud-0.0.5.tar", last modified: Tue Jun 13 12:33:48 2023, max compression
```

## Comparing `edumud-0.0.4.tar` & `edumud-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 12:17:26.882797 edumud-0.0.4/
--rw-rw-rw-   0        0        0    35823 2023-05-28 07:14:53.000000 edumud-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3211 2023-06-13 12:17:26.882797 edumud-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2713 2023-06-13 12:17:04.000000 edumud-0.0.4/README.rst
--rw-rw-rw-   0        0        0      584 2023-06-13 12:12:48.000000 edumud-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 12:17:26.883763 edumud-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      102 2023-05-26 11:39:59.000000 edumud-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 12:17:26.855232 edumud-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 12:17:26.873139 edumud-0.0.4/src/edumud/
--rw-rw-rw-   0        0        0        0 2023-05-14 17:00:29.000000 edumud-0.0.4/src/edumud/__init__.py
--rw-rw-rw-   0        0        0     1562 2023-06-08 11:32:09.000000 edumud-0.0.4/src/edumud/cells.py
--rw-rw-rw-   0        0        0     4365 2023-05-15 18:10:11.000000 edumud-0.0.4/src/edumud/colloids.py
--rw-rw-rw-   0        0        0      837 2023-06-09 06:10:09.000000 edumud-0.0.4/src/edumud/constants.py
--rw-rw-rw-   0        0        0     3095 2023-05-25 07:58:39.000000 edumud-0.0.4/src/edumud/electrolytes.py
--rw-rw-rw-   0        0        0      351 2023-05-25 06:25:39.000000 edumud-0.0.4/src/edumud/file_utils.py
--rw-rw-rw-   0        0        0     1766 2023-05-25 07:12:59.000000 edumud-0.0.4/src/edumud/particles.py
-drwxrwxrwx   0        0        0        0 2023-06-13 12:17:26.879761 edumud-0.0.4/src/edumud.egg-info/
--rw-rw-rw-   0        0        0     3211 2023-06-13 12:17:26.000000 edumud-0.0.4/src/edumud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-06-13 12:17:26.000000 edumud-0.0.4/src/edumud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 12:17:26.000000 edumud-0.0.4/src/edumud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-13 12:17:26.000000 edumud-0.0.4/src/edumud.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 12:17:26.880792 edumud-0.0.4/tests/
--rw-rw-rw-   0        0        0      100 2023-06-12 16:58:31.000000 edumud-0.0.4/tests/test_module_demo.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:33:48.022441 edumud-0.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-05-28 07:14:53.000000 edumud-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3237 2023-06-13 12:33:48.022441 edumud-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2737 2023-06-13 12:32:09.000000 edumud-0.0.5/README.rst
+-rw-rw-rw-   0        0        0      584 2023-06-13 12:32:33.000000 edumud-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 12:33:48.022441 edumud-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      102 2023-05-26 11:39:59.000000 edumud-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:33:47.991056 edumud-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 12:33:48.022441 edumud-0.0.5/src/edumud/
+-rw-rw-rw-   0        0        0        0 2023-05-14 17:00:29.000000 edumud-0.0.5/src/edumud/__init__.py
+-rw-rw-rw-   0        0        0     1562 2023-06-08 11:32:09.000000 edumud-0.0.5/src/edumud/cells.py
+-rw-rw-rw-   0        0        0     4365 2023-05-15 18:10:11.000000 edumud-0.0.5/src/edumud/colloids.py
+-rw-rw-rw-   0        0        0      837 2023-06-09 06:10:09.000000 edumud-0.0.5/src/edumud/constants.py
+-rw-rw-rw-   0        0        0     3095 2023-05-25 07:58:39.000000 edumud-0.0.5/src/edumud/electrolytes.py
+-rw-rw-rw-   0        0        0      351 2023-05-25 06:25:39.000000 edumud-0.0.5/src/edumud/file_utils.py
+-rw-rw-rw-   0        0        0     1766 2023-05-25 07:12:59.000000 edumud-0.0.5/src/edumud/particles.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:33:48.022441 edumud-0.0.5/src/edumud.egg-info/
+-rw-rw-rw-   0        0        0     3237 2023-06-13 12:33:47.000000 edumud-0.0.5/src/edumud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-06-13 12:33:47.000000 edumud-0.0.5/src/edumud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 12:33:47.000000 edumud-0.0.5/src/edumud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 12:33:47.000000 edumud-0.0.5/src/edumud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 12:33:48.022441 edumud-0.0.5/tests/
+-rw-rw-rw-   0        0        0      100 2023-06-12 16:58:31.000000 edumud-0.0.5/tests/test_module_demo.py
```

### Comparing `edumud-0.0.4/LICENSE` & `edumud-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edumud-0.0.4/PKG-INFO` & `edumud-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edumud
-Version: 0.0.4
+Version: 0.0.5
 Summary: Educational MUDNET software in Python
 Author-email: "Paul J.M. van Kan" <p.j.m.vankan@tudelft.nl>
 Project-URL: Homepage, https://bitbucket.org/deltares/edumud/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -108,8 +108,10 @@
    :alt: PyPI - Downloads
 
 .. |PyPi Status| image:: https://img.shields.io/pypi/status/edumud
    :alt: PyPI - Status
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/edumud/badge/?version=latest
    :target: https://edumud.readthedocs.io/en/latest/?badge=latest
-.. |PyPI - License| image:: https://img.shields.io/pypi/l/edumud?
+
+.. |PyPI - License| image:: https://img.shields.io/pypi/l/edumud
+   :alt: PyPI - License
```

### Comparing `edumud-0.0.4/README.rst` & `edumud-0.0.5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -95,8 +95,10 @@
    :alt: PyPI - Downloads
 
 .. |PyPi Status| image:: https://img.shields.io/pypi/status/edumud
    :alt: PyPI - Status
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/edumud/badge/?version=latest
    :target: https://edumud.readthedocs.io/en/latest/?badge=latest
-.. |PyPI - License| image:: https://img.shields.io/pypi/l/edumud?
+
+.. |PyPI - License| image:: https://img.shields.io/pypi/l/edumud
+   :alt: PyPI - License
```

### Comparing `edumud-0.0.4/pyproject.toml` & `edumud-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edumud"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Paul J.M. van Kan", email="p.j.m.vankan@tudelft.nl" },
 ]
 description = "Educational MUDNET software in Python"
 readme = "README.rst"
 
 requires-python = ">=3.10"
```

### Comparing `edumud-0.0.4/src/edumud/cells.py` & `edumud-0.0.5/src/edumud/cells.py`

 * *Files identical despite different names*

### Comparing `edumud-0.0.4/src/edumud/colloids.py` & `edumud-0.0.5/src/edumud/colloids.py`

 * *Files identical despite different names*

### Comparing `edumud-0.0.4/src/edumud/constants.py` & `edumud-0.0.5/src/edumud/constants.py`

 * *Files identical despite different names*

### Comparing `edumud-0.0.4/src/edumud/electrolytes.py` & `edumud-0.0.5/src/edumud/electrolytes.py`

 * *Files identical despite different names*

### Comparing `edumud-0.0.4/src/edumud/particles.py` & `edumud-0.0.5/src/edumud/particles.py`

 * *Files identical despite different names*

### Comparing `edumud-0.0.4/src/edumud.egg-info/PKG-INFO` & `edumud-0.0.5/src/edumud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edumud
-Version: 0.0.4
+Version: 0.0.5
 Summary: Educational MUDNET software in Python
 Author-email: "Paul J.M. van Kan" <p.j.m.vankan@tudelft.nl>
 Project-URL: Homepage, https://bitbucket.org/deltares/edumud/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -108,8 +108,10 @@
    :alt: PyPI - Downloads
 
 .. |PyPi Status| image:: https://img.shields.io/pypi/status/edumud
    :alt: PyPI - Status
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/edumud/badge/?version=latest
    :target: https://edumud.readthedocs.io/en/latest/?badge=latest
-.. |PyPI - License| image:: https://img.shields.io/pypi/l/edumud?
+
+.. |PyPI - License| image:: https://img.shields.io/pypi/l/edumud
+   :alt: PyPI - License
```

