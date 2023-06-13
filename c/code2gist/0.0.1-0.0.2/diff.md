# Comparing `tmp/code2gist-0.0.1.tar.gz` & `tmp/code2gist-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code2gist-0.0.1.tar", last modified: Tue Jun 13 18:08:54 2023, max compression
+gzip compressed data, was "code2gist-0.0.2.tar", last modified: Tue Jun 13 18:37:04 2023, max compression
```

## Comparing `code2gist-0.0.1.tar` & `code2gist-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:08:54.439556 code2gist-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-06-13 15:23:13.000000 code2gist-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1367 2023-06-13 18:08:54.437550 code2gist-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      996 2023-06-13 16:04:03.000000 code2gist-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 18:08:54.388017 code2gist-0.0.1/code2gist/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:42:17.000000 code2gist-0.0.1/code2gist/__init__.py
--rw-rw-rw-   0        0        0     2053 2023-06-13 15:42:32.000000 code2gist-0.0.1/code2gist/main.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:08:54.435550 code2gist-0.0.1/code2gist.egg-info/
--rw-rw-rw-   0        0        0     1367 2023-06-13 18:08:54.000000 code2gist-0.0.1/code2gist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-13 18:08:54.000000 code2gist-0.0.1/code2gist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:08:54.000000 code2gist-0.0.1/code2gist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-13 18:08:54.000000 code2gist-0.0.1/code2gist.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-06-13 18:08:54.000000 code2gist-0.0.1/code2gist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 18:08:54.000000 code2gist-0.0.1/code2gist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      603 2023-06-13 18:07:51.000000 code2gist-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 18:08:54.439556 code2gist-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 18:37:04.241269 code2gist-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-06-13 15:23:13.000000 code2gist-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1367 2023-06-13 18:37:04.240270 code2gist-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      996 2023-06-13 16:04:03.000000 code2gist-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 18:37:04.193270 code2gist-0.0.2/code2gist/
+-rw-rw-rw-   0        0        0       22 2023-06-13 18:34:11.000000 code2gist-0.0.2/code2gist/__init__.py
+-rw-rw-rw-   0        0        0     2053 2023-06-13 18:34:48.000000 code2gist-0.0.2/code2gist/main.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:37:04.237269 code2gist-0.0.2/code2gist.egg-info/
+-rw-rw-rw-   0        0        0     1367 2023-06-13 18:37:03.000000 code2gist-0.0.2/code2gist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-13 18:37:04.000000 code2gist-0.0.2/code2gist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:37:03.000000 code2gist-0.0.2/code2gist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-13 18:37:03.000000 code2gist-0.0.2/code2gist.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-06-13 18:37:03.000000 code2gist-0.0.2/code2gist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 18:37:03.000000 code2gist-0.0.2/code2gist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      603 2023-06-13 18:35:23.000000 code2gist-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 18:37:04.241269 code2gist-0.0.2/setup.cfg
```

### Comparing `code2gist-0.0.1/LICENSE` & `code2gist-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `code2gist-0.0.1/PKG-INFO` & `code2gist-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code2gist
-Version: 0.0.1
+Version: 0.0.2
 Summary: Upload Python files in a directory to a GitHub Gist.
 Author-email: Cameron Spears <crspears@outlook.com>
 License: GPL-3.0
 Keywords: python,github,gist,upload
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
```

### Comparing `code2gist-0.0.1/README.md` & `code2gist-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `code2gist-0.0.1/code2gist/main.py` & `code2gist-0.0.2/code2gist/main.py`

 * *Files identical despite different names*

### Comparing `code2gist-0.0.1/code2gist.egg-info/PKG-INFO` & `code2gist-0.0.2/code2gist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code2gist
-Version: 0.0.1
+Version: 0.0.2
 Summary: Upload Python files in a directory to a GitHub Gist.
 Author-email: Cameron Spears <crspears@outlook.com>
 License: GPL-3.0
 Keywords: python,github,gist,upload
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
```

### Comparing `code2gist-0.0.1/pyproject.toml` & `code2gist-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "code2gist"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Cameron Spears", email = "crspears@outlook.com"},
 ]
 description = "Upload Python files in a directory to a GitHub Gist."
 readme = "README.md"
 requires-python = ">=3.11.4"
 keywords = ["python", "github", "gist", "upload"]
```

