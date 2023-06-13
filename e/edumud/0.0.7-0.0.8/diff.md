# Comparing `tmp/edumud-0.0.7.tar.gz` & `tmp/edumud-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edumud-0.0.7.tar", last modified: Tue Jun 13 12:50:38 2023, max compression
+gzip compressed data, was "edumud-0.0.8.tar", last modified: Tue Jun 13 12:54:17 2023, max compression
```

## Comparing `edumud-0.0.7.tar` & `edumud-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 12:50:38.045476 edumud-0.0.7/
--rw-rw-rw-   0        0        0    35823 2023-05-28 07:14:53.000000 edumud-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3366 2023-06-13 12:50:38.045476 edumud-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2866 2023-06-13 12:49:59.000000 edumud-0.0.7/README.rst
--rw-rw-rw-   0        0        0      584 2023-06-13 12:50:09.000000 edumud-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 12:50:38.045476 edumud-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      102 2023-05-26 11:39:59.000000 edumud-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 12:50:38.014226 edumud-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 12:50:38.029852 edumud-0.0.7/src/edumud/
--rw-rw-rw-   0        0        0        0 2023-05-14 17:00:29.000000 edumud-0.0.7/src/edumud/__init__.py
--rw-rw-rw-   0        0        0     1562 2023-06-08 11:32:09.000000 edumud-0.0.7/src/edumud/cells.py
--rw-rw-rw-   0        0        0     4365 2023-05-15 18:10:11.000000 edumud-0.0.7/src/edumud/colloids.py
--rw-rw-rw-   0        0        0      837 2023-06-09 06:10:09.000000 edumud-0.0.7/src/edumud/constants.py
--rw-rw-rw-   0        0        0     3095 2023-05-25 07:58:39.000000 edumud-0.0.7/src/edumud/electrolytes.py
--rw-rw-rw-   0        0        0      351 2023-05-25 06:25:39.000000 edumud-0.0.7/src/edumud/file_utils.py
--rw-rw-rw-   0        0        0     1766 2023-05-25 07:12:59.000000 edumud-0.0.7/src/edumud/particles.py
-drwxrwxrwx   0        0        0        0 2023-06-13 12:50:38.029852 edumud-0.0.7/src/edumud.egg-info/
--rw-rw-rw-   0        0        0     3366 2023-06-13 12:50:37.000000 edumud-0.0.7/src/edumud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-06-13 12:50:38.000000 edumud-0.0.7/src/edumud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 12:50:37.000000 edumud-0.0.7/src/edumud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-13 12:50:37.000000 edumud-0.0.7/src/edumud.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 12:50:38.045476 edumud-0.0.7/tests/
--rw-rw-rw-   0        0        0      100 2023-06-12 16:58:31.000000 edumud-0.0.7/tests/test_module_demo.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:17.047732 edumud-0.0.8/
+-rw-rw-rw-   0        0        0    35823 2023-05-28 07:14:53.000000 edumud-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3237 2023-06-13 12:54:17.047732 edumud-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2737 2023-06-13 12:53:43.000000 edumud-0.0.8/README.rst
+-rw-rw-rw-   0        0        0      584 2023-06-13 12:53:53.000000 edumud-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 12:54:17.047732 edumud-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      102 2023-05-26 11:39:59.000000 edumud-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:17.016675 edumud-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:17.035223 edumud-0.0.8/src/edumud/
+-rw-rw-rw-   0        0        0        0 2023-05-14 17:00:29.000000 edumud-0.0.8/src/edumud/__init__.py
+-rw-rw-rw-   0        0        0     1562 2023-06-08 11:32:09.000000 edumud-0.0.8/src/edumud/cells.py
+-rw-rw-rw-   0        0        0     4365 2023-05-15 18:10:11.000000 edumud-0.0.8/src/edumud/colloids.py
+-rw-rw-rw-   0        0        0      837 2023-06-09 06:10:09.000000 edumud-0.0.8/src/edumud/constants.py
+-rw-rw-rw-   0        0        0     3095 2023-05-25 07:58:39.000000 edumud-0.0.8/src/edumud/electrolytes.py
+-rw-rw-rw-   0        0        0      351 2023-05-25 06:25:39.000000 edumud-0.0.8/src/edumud/file_utils.py
+-rw-rw-rw-   0        0        0     1766 2023-05-25 07:12:59.000000 edumud-0.0.8/src/edumud/particles.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:17.035223 edumud-0.0.8/src/edumud.egg-info/
+-rw-rw-rw-   0        0        0     3237 2023-06-13 12:54:17.000000 edumud-0.0.8/src/edumud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-06-13 12:54:17.000000 edumud-0.0.8/src/edumud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 12:54:17.000000 edumud-0.0.8/src/edumud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 12:54:17.000000 edumud-0.0.8/src/edumud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 12:54:17.047732 edumud-0.0.8/tests/
+-rw-rw-rw-   0        0        0      100 2023-06-12 16:58:31.000000 edumud-0.0.8/tests/test_module_demo.py
```

### Comparing `edumud-0.0.7/LICENSE` & `edumud-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edumud-0.0.7/PKG-INFO` & `edumud-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: edumud
-Version: 0.0.7
+Version: 0.0.8
 Summary: Educational MUDNET software in Python
 Author-email: "Paul J.M. van Kan" <p.j.m.vankan@tudelft.nl>
 Project-URL: Homepage, https://bitbucket.org/deltares/edumud/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 EduMUD
 ======
 
-|PyPI| |PyPI - Downloads| |PyPI download total| |Documentation Status| |PyPI - License|
+|PyPI| |PyPI - Downloads| |Documentation Status| |PyPI - License|
 
 A Python package to assist in the study of sedimentation phenomena in
 colloidal suspensions. The code is being developed by `Paul J.M. van
 Kan <http://vankanscientific.nl>`__ for the MUDNET group at Delft
 Technical University and DELTARES, The Netherlands. The EduMUD package
 can be used under the conditions of the GPLv3 license.
 
@@ -100,17 +100,14 @@
 ----------
 
 -  ...
 
 .. |PyPi| image:: https://img.shields.io/pypi/v/edumud
    :alt: PyPI
 
-.. |PyPI download total| image:: https://img.shields.io/pypi/dt/edumud
-   :alt: PyPI - Total Downloads
-
 .. |PyPI - Downloads| image:: https://img.shields.io/pypi/dm/edumud
    :alt: PyPI - Downloads
 
 .. |PyPi Status| image:: https://img.shields.io/pypi/status/edumud
    :alt: PyPI - Status
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/edumud/badge/?version=latest
```

### Comparing `edumud-0.0.7/README.rst` & `edumud-0.0.8/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 EduMUD
 ======
 
-|PyPI| |PyPI - Downloads| |PyPI download total| |Documentation Status| |PyPI - License|
+|PyPI| |PyPI - Downloads| |Documentation Status| |PyPI - License|
 
 A Python package to assist in the study of sedimentation phenomena in
 colloidal suspensions. The code is being developed by `Paul J.M. van
 Kan <http://vankanscientific.nl>`__ for the MUDNET group at Delft
 Technical University and DELTARES, The Netherlands. The EduMUD package
 can be used under the conditions of the GPLv3 license.
 
@@ -87,17 +87,14 @@
 ----------
 
 -  ...
 
 .. |PyPi| image:: https://img.shields.io/pypi/v/edumud
    :alt: PyPI
 
-.. |PyPI download total| image:: https://img.shields.io/pypi/dt/edumud
-   :alt: PyPI - Total Downloads
-
 .. |PyPI - Downloads| image:: https://img.shields.io/pypi/dm/edumud
    :alt: PyPI - Downloads
 
 .. |PyPi Status| image:: https://img.shields.io/pypi/status/edumud
    :alt: PyPI - Status
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/edumud/badge/?version=latest
```

### Comparing `edumud-0.0.7/pyproject.toml` & `edumud-0.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edumud"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Paul J.M. van Kan", email="p.j.m.vankan@tudelft.nl" },
 ]
 description = "Educational MUDNET software in Python"
 readme = "README.rst"
 
 requires-python = ">=3.10"
```

### Comparing `edumud-0.0.7/src/edumud/cells.py` & `edumud-0.0.8/src/edumud/cells.py`

 * *Files identical despite different names*

### Comparing `edumud-0.0.7/src/edumud/colloids.py` & `edumud-0.0.8/src/edumud/colloids.py`

 * *Files identical despite different names*

### Comparing `edumud-0.0.7/src/edumud/constants.py` & `edumud-0.0.8/src/edumud/constants.py`

 * *Files identical despite different names*

### Comparing `edumud-0.0.7/src/edumud/electrolytes.py` & `edumud-0.0.8/src/edumud/electrolytes.py`

 * *Files identical despite different names*

### Comparing `edumud-0.0.7/src/edumud/particles.py` & `edumud-0.0.8/src/edumud/particles.py`

 * *Files identical despite different names*

### Comparing `edumud-0.0.7/src/edumud.egg-info/PKG-INFO` & `edumud-0.0.8/src/edumud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: edumud
-Version: 0.0.7
+Version: 0.0.8
 Summary: Educational MUDNET software in Python
 Author-email: "Paul J.M. van Kan" <p.j.m.vankan@tudelft.nl>
 Project-URL: Homepage, https://bitbucket.org/deltares/edumud/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 EduMUD
 ======
 
-|PyPI| |PyPI - Downloads| |PyPI download total| |Documentation Status| |PyPI - License|
+|PyPI| |PyPI - Downloads| |Documentation Status| |PyPI - License|
 
 A Python package to assist in the study of sedimentation phenomena in
 colloidal suspensions. The code is being developed by `Paul J.M. van
 Kan <http://vankanscientific.nl>`__ for the MUDNET group at Delft
 Technical University and DELTARES, The Netherlands. The EduMUD package
 can be used under the conditions of the GPLv3 license.
 
@@ -100,17 +100,14 @@
 ----------
 
 -  ...
 
 .. |PyPi| image:: https://img.shields.io/pypi/v/edumud
    :alt: PyPI
 
-.. |PyPI download total| image:: https://img.shields.io/pypi/dt/edumud
-   :alt: PyPI - Total Downloads
-
 .. |PyPI - Downloads| image:: https://img.shields.io/pypi/dm/edumud
    :alt: PyPI - Downloads
 
 .. |PyPi Status| image:: https://img.shields.io/pypi/status/edumud
    :alt: PyPI - Status
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/edumud/badge/?version=latest
```

