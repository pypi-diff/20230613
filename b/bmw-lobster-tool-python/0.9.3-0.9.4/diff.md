# Comparing `tmp/bmw-lobster-tool-python-0.9.3.tar.gz` & `tmp/bmw-lobster-tool-python-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-python-0.9.3.tar", last modified: Tue May  9 09:58:21 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-python-0.9.4.tar", last modified: Tue Jun 13 09:18:58 2023, max compression
```

## Comparing `bmw-lobster-tool-python-0.9.3.tar` & `bmw-lobster-tool-python-0.9.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:21.836670 bmw-lobster-tool-python-0.9.3/
--rw-r--r--   0 florian   (1000) florian   (1000)     1542 2023-05-09 09:58:21.836670 bmw-lobster-tool-python-0.9.3/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      609 2023-05-08 15:03:18.000000 bmw-lobster-tool-python-0.9.3/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:21.836670 bmw-lobster-tool-python-0.9.3/bmw_lobster_tool_python.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     1542 2023-05-09 09:58:21.000000 bmw-lobster-tool-python-0.9.3/bmw_lobster_tool_python.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      366 2023-05-09 09:58:21.000000 bmw-lobster-tool-python-0.9.3/bmw_lobster_tool_python.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-09 09:58:21.000000 bmw-lobster-tool-python-0.9.3/bmw_lobster_tool_python.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       68 2023-05-09 09:58:21.000000 bmw-lobster-tool-python-0.9.3/bmw_lobster_tool_python.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-09 09:58:21.000000 bmw-lobster-tool-python-0.9.3/bmw_lobster_tool_python.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-09 09:58:21.000000 bmw-lobster-tool-python-0.9.3/bmw_lobster_tool_python.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:21.832669 bmw-lobster-tool-python-0.9.3/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:21.832669 bmw-lobster-tool-python-0.9.3/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:21.836670 bmw-lobster-tool-python-0.9.3/lobster/tools/python/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:21.000000 bmw-lobster-tool-python-0.9.3/lobster/tools/python/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)    12276 2023-05-09 09:58:21.000000 bmw-lobster-tool-python-0.9.3/lobster/tools/python/python.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-09 09:58:21.836670 bmw-lobster-tool-python-0.9.3/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2273 2023-05-08 15:03:18.000000 bmw-lobster-tool-python-0.9.3/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:58.097262 bmw-lobster-tool-python-0.9.4/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1544 2023-06-13 09:18:58.097262 bmw-lobster-tool-python-0.9.4/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      611 2023-06-13 09:17:37.000000 bmw-lobster-tool-python-0.9.4/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:58.097262 bmw-lobster-tool-python-0.9.4/bmw_lobster_tool_python.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1544 2023-06-13 09:18:58.000000 bmw-lobster-tool-python-0.9.4/bmw_lobster_tool_python.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      366 2023-06-13 09:18:58.000000 bmw-lobster-tool-python-0.9.4/bmw_lobster_tool_python.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-13 09:18:58.000000 bmw-lobster-tool-python-0.9.4/bmw_lobster_tool_python.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       68 2023-06-13 09:18:58.000000 bmw-lobster-tool-python-0.9.4/bmw_lobster_tool_python.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-13 09:18:58.000000 bmw-lobster-tool-python-0.9.4/bmw_lobster_tool_python.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-13 09:18:58.000000 bmw-lobster-tool-python-0.9.4/bmw_lobster_tool_python.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:58.097262 bmw-lobster-tool-python-0.9.4/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:58.097262 bmw-lobster-tool-python-0.9.4/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:58.097262 bmw-lobster-tool-python-0.9.4/lobster/tools/python/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:57.000000 bmw-lobster-tool-python-0.9.4/lobster/tools/python/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)    12276 2023-06-13 09:18:57.000000 bmw-lobster-tool-python-0.9.4/lobster/tools/python/python.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-13 09:18:58.097262 bmw-lobster-tool-python-0.9.4/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2273 2023-05-08 15:03:18.000000 bmw-lobster-tool-python-0.9.4/setup.py
```

### Comparing `bmw-lobster-tool-python-0.9.3/PKG-INFO` & `bmw-lobster-tool-python-0.9.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-python
-Version: 0.9.3
+Version: 0.9.4
 Summary: LOBSTER Tool for Python3
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
@@ -16,16 +16,16 @@
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 
 # LOBSTER
 
-The **L**ightweight **O**pen **B**MW **S**oftware **T**racability
-**E**vidence **R**eport allows you to demonstrate software tracability
+The **L**ightweight **O**pen **B**MW **S**oftware **T**raceability
+**E**vidence **R**eport allows you to demonstrate software traceability
 and requirements coverage, which is essential for meeting standards
 such as ISO 26262.
 
 This package contains a tool extract tracing tags from Python3 source
 code.
 
 ## Tools
```

### Comparing `bmw-lobster-tool-python-0.9.3/README.md` & `bmw-lobster-tool-python-0.9.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # LOBSTER
 
-The **L**ightweight **O**pen **B**MW **S**oftware **T**racability
-**E**vidence **R**eport allows you to demonstrate software tracability
+The **L**ightweight **O**pen **B**MW **S**oftware **T**raceability
+**E**vidence **R**eport allows you to demonstrate software traceability
 and requirements coverage, which is essential for meeting standards
 such as ISO 26262.
 
 This package contains a tool extract tracing tags from Python3 source
 code.
 
 ## Tools
```

### Comparing `bmw-lobster-tool-python-0.9.3/bmw_lobster_tool_python.egg-info/PKG-INFO` & `bmw-lobster-tool-python-0.9.4/bmw_lobster_tool_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-python
-Version: 0.9.3
+Version: 0.9.4
 Summary: LOBSTER Tool for Python3
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
@@ -16,16 +16,16 @@
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 
 # LOBSTER
 
-The **L**ightweight **O**pen **B**MW **S**oftware **T**racability
-**E**vidence **R**eport allows you to demonstrate software tracability
+The **L**ightweight **O**pen **B**MW **S**oftware **T**raceability
+**E**vidence **R**eport allows you to demonstrate software traceability
 and requirements coverage, which is essential for meeting standards
 such as ISO 26262.
 
 This package contains a tool extract tracing tags from Python3 source
 code.
 
 ## Tools
```

### Comparing `bmw-lobster-tool-python-0.9.3/lobster/tools/python/python.py` & `bmw-lobster-tool-python-0.9.4/lobster/tools/python/python.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-python-0.9.3/setup.py` & `bmw-lobster-tool-python-0.9.4/setup.py`

 * *Files identical despite different names*

