# Comparing `tmp/python-kacl-0.4.5.tar.gz` & `tmp/python-kacl-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-kacl-0.4.5.tar", last modified: Fri May 26 16:28:07 2023, max compression
+gzip compressed data, was "python-kacl-0.4.6.tar", last modified: Tue Jun 13 11:12:32 2023, max compression
```

## Comparing `python-kacl-0.4.5.tar` & `python-kacl-0.4.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:28:07.816015 python-kacl-0.4.5/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-26 16:27:59.000000 python-kacl-0.4.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-26 16:27:59.000000 python-kacl-0.4.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    19220 2023-05-26 16:28:07.816015 python-kacl-0.4.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    18571 2023-05-26 16:27:59.000000 python-kacl-0.4.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:28:07.814015 python-kacl-0.4.5/kacl/
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/changes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:28:07.814015 python-kacl-0.4.5/kacl/config/
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/config/kacl-default.yml
--rw-rw-rw-   0 root         (0) root         (0)     2792 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/config.py
--rw-rw-rw-   0 root         (0) root         (0)    20447 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/document.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/element.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/exception.py
--rwxrwxrwx   0 root         (0) root         (0)    16280 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/kacl_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/link_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     2338 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/validation.py
--rw-rw-rw-   0 root         (0) root         (0)     9533 2023-05-26 16:27:59.000000 python-kacl-0.4.5/kacl/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:28:07.815015 python-kacl-0.4.5/python_kacl.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19220 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-26 16:28:07.000000 python-kacl-0.4.5/python_kacl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 16:28:07.816015 python-kacl-0.4.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-26 16:27:59.000000 python-kacl-0.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:28:07.816015 python-kacl-0.4.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-26 16:27:59.000000 python-kacl-0.4.5/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1264 2023-05-26 16:27:59.000000 python-kacl-0.4.5/tests/snapshot_directory.py
--rw-rw-rw-   0 root         (0) root         (0)     7349 2023-05-26 16:27:59.000000 python-kacl-0.4.5/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    12545 2023-05-26 16:27:59.000000 python-kacl-0.4.5/tests/test_kacl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:12:32.075660 python-kacl-0.4.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-06-13 11:12:22.000000 python-kacl-0.4.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-13 11:12:22.000000 python-kacl-0.4.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    19220 2023-06-13 11:12:32.075660 python-kacl-0.4.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    18571 2023-06-13 11:12:22.000000 python-kacl-0.4.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:12:32.073660 python-kacl-0.4.6/kacl/
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/changes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:12:32.073660 python-kacl-0.4.6/kacl/config/
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/config/kacl-default.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2792 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    20447 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/document.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/element.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)    16276 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/kacl_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/link_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     2338 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9533 2023-06-13 11:12:22.000000 python-kacl-0.4.6/kacl/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:12:32.074660 python-kacl-0.4.6/python_kacl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19220 2023-06-13 11:12:32.000000 python-kacl-0.4.6/python_kacl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      620 2023-06-13 11:12:32.000000 python-kacl-0.4.6/python_kacl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 11:12:32.000000 python-kacl-0.4.6/python_kacl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-13 11:12:32.000000 python-kacl-0.4.6/python_kacl.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 11:12:32.000000 python-kacl-0.4.6/python_kacl.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-13 11:12:32.000000 python-kacl-0.4.6/python_kacl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-13 11:12:32.000000 python-kacl-0.4.6/python_kacl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 11:12:32.075660 python-kacl-0.4.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2023-06-13 11:12:22.000000 python-kacl-0.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:12:32.075660 python-kacl-0.4.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-06-13 11:12:22.000000 python-kacl-0.4.6/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2023-06-13 11:12:22.000000 python-kacl-0.4.6/tests/snapshot_directory.py
+-rw-rw-rw-   0 root         (0) root         (0)     7349 2023-06-13 11:12:22.000000 python-kacl-0.4.6/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    12545 2023-06-13 11:12:22.000000 python-kacl-0.4.6/tests/test_kacl.py
```

### Comparing `python-kacl-0.4.5/LICENSE` & `python-kacl-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/PKG-INFO` & `python-kacl-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kacl
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"
 Home-page: https://gitlab.com/schmieder.matthias/python-kacl.git
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-kacl-0.4.5/README.md` & `python-kacl-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/kacl/__init__.py` & `python-kacl-0.4.6/kacl/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version of the python-kacl package
-__version__ = "0.4.5"
+__version__ = "0.4.6"
 
 from kacl.document import KACLDocument
 from kacl.serializer import KACLMarkdownSerializer
 
 
 def load(file):
     """
```

### Comparing `python-kacl-0.4.5/kacl/changes.py` & `python-kacl-0.4.6/kacl/changes.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/kacl/config/kacl-default.yml` & `python-kacl-0.4.6/kacl/config/kacl-default.yml`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/kacl/config.py` & `python-kacl-0.4.6/kacl/config.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/kacl/document.py` & `python-kacl-0.4.6/kacl/document.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/kacl/kacl_cli.py` & `python-kacl-0.4.6/kacl/kacl_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,15 @@
 
     # check if we should modify the file
     if modify:
         with open(kacl_changelog.config.changelog_file_path, "w") as f:
             f.write(kacl_changelog_content)
         f.close()
 
-        if not no_commit:
+        if no_commit:
             return
 
         if commit or tag or kacl_config.git_create_commit or kacl_config.git_create_tag:
             vcs_context = {
                 "latest_version": latest_version,
                 "new_version": new_version,
             }
```

### Comparing `python-kacl-0.4.5/kacl/link_provider.py` & `python-kacl-0.4.6/kacl/link_provider.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/kacl/parser.py` & `python-kacl-0.4.6/kacl/parser.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/kacl/serializer.py` & `python-kacl-0.4.6/kacl/serializer.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/kacl/validation.py` & `python-kacl-0.4.6/kacl/validation.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/kacl/version.py` & `python-kacl-0.4.6/kacl/version.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/python_kacl.egg-info/PKG-INFO` & `python-kacl-0.4.6/python_kacl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-kacl
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python module and CLI tool for validating and modifying Changelogs in "keep-a-changelog" format"
 Home-page: https://gitlab.com/schmieder.matthias/python-kacl.git
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-kacl-0.4.5/python_kacl.egg-info/SOURCES.txt` & `python-kacl-0.4.6/python_kacl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/setup.py` & `python-kacl-0.4.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.4.5"
+version = "0.4.6"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [
```

### Comparing `python-kacl-0.4.5/tests/snapshot_directory.py` & `python-kacl-0.4.6/tests/snapshot_directory.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/tests/test_cli.py` & `python-kacl-0.4.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-kacl-0.4.5/tests/test_kacl.py` & `python-kacl-0.4.6/tests/test_kacl.py`

 * *Files identical despite different names*

