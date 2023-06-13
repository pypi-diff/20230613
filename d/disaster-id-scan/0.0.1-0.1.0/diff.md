# Comparing `tmp/disaster_id_scan-0.0.1.tar.gz` & `tmp/disaster_id_scan-0.1.0.tar.gz`

## Comparing `disaster_id_scan-0.0.1.tar` & `disaster_id_scan-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 disaster_id_scan-0.0.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 disaster_id_scan-0.0.1/src/disaster_id_scan/__about__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 disaster_id_scan-0.0.1/src/disaster_id_scan/__init__.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 disaster_id_scan-0.0.1/src/disaster_id_scan/__main__.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 disaster_id_scan-0.0.1/src/disaster_id_scan/id_scanner.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 disaster_id_scan-0.0.1/src/disaster_id_scan/cli/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 disaster_id_scan-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 disaster_id_scan-0.0.1/.gitignore
--rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 disaster_id_scan-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 disaster_id_scan-0.0.1/README.md
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 disaster_id_scan-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 disaster_id_scan-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/src/disaster_id_scan/__about__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/src/disaster_id_scan/__init__.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/src/disaster_id_scan/__main__.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/src/disaster_id_scan/id_scanner.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/src/disaster_id_scan/mrz.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/src/disaster_id_scan/store.py
+-rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/src/disaster_id_scan/ui.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/src/disaster_id_scan/cli/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/.gitignore
+-rw-r--r--   0        0        0    13792 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/README.md
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 disaster_id_scan-0.1.0/PKG-INFO
```

### Comparing `disaster_id_scan-0.0.1/.github/workflows/pypi-publish.yml` & `disaster_id_scan-0.1.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `disaster_id_scan-0.0.1/src/disaster_id_scan/id_scanner.py` & `disaster_id_scan-0.1.0/src/disaster_id_scan/id_scanner.py`

 * *Files identical despite different names*

### Comparing `disaster_id_scan-0.0.1/src/disaster_id_scan/cli/__init__.py` & `disaster_id_scan-0.1.0/src/disaster_id_scan/cli/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # SPDX-FileCopyrightText: 2023-present anjomro <py@anjomro.de>
 #
 # SPDX-License-Identifier: EUPL-1.2
 import click
 
 from disaster_id_scan.__about__ import __version__
 from disaster_id_scan.id_scanner import id_scanner
+from disaster_id_scan.ui import start_gui
 
 
 @click.group(context_settings={"help_option_names": ["-h", "--help"]}, invoke_without_command=True)
 @click.version_option(version=__version__, prog_name="Disaster ID Scan")
 def disaster_id_scan():
-    click.echo("Hello world!")
+    start_gui()
 
 
 # Command to start id scanner as cli application
 @click.command()
 @click.option('--cam', '-c', default=0, help='Camera ID to use, default 0')
 def scan(cam):
     """Starts ID scanner"""
     id_scanner(cam)
 
 
 # Register commands
-disaster_id_scan.add_command(scan)
+disaster_id_scan.add_command(scan)
```

### Comparing `disaster_id_scan-0.0.1/LICENSE.txt` & `disaster_id_scan-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `disaster_id_scan-0.0.1/pyproject.toml` & `disaster_id_scan-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,18 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "click",
   "easyocr",
   "opencv-python",
+  "mrz",
+  "tk",
+  "tkcalendar",
+  "jsonpickle",
 ]
 
 [project.urls]
 Documentation = "https://github.com/unknown/disaster-id-scan#readme"
 Issues = "https://github.com/unknown/disaster-id-scan/issues"
 Source = "https://github.com/unknown/disaster-id-scan"
```

