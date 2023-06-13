# Comparing `tmp/bmw-lobster-tool-trlc-0.9.3.tar.gz` & `tmp/bmw-lobster-tool-trlc-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-trlc-0.9.3.tar", last modified: Tue May  9 09:58:20 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-trlc-0.9.4.tar", last modified: Tue Jun 13 09:18:56 2023, max compression
```

## Comparing `bmw-lobster-tool-trlc-0.9.3.tar` & `bmw-lobster-tool-trlc-0.9.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:20.156661 bmw-lobster-tool-trlc-0.9.3/
--rw-r--r--   0 florian   (1000) florian   (1000)     3208 2023-05-09 09:58:20.156661 bmw-lobster-tool-trlc-0.9.3/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     2280 2023-05-08 15:03:18.000000 bmw-lobster-tool-trlc-0.9.3/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:20.156661 bmw-lobster-tool-trlc-0.9.3/bmw_lobster_tool_trlc.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     3208 2023-05-09 09:58:20.000000 bmw-lobster-tool-trlc-0.9.3/bmw_lobster_tool_trlc.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      317 2023-05-09 09:58:20.000000 bmw-lobster-tool-trlc-0.9.3/bmw_lobster_tool_trlc.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-09 09:58:20.000000 bmw-lobster-tool-trlc-0.9.3/bmw_lobster_tool_trlc.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       62 2023-05-09 09:58:20.000000 bmw-lobster-tool-trlc-0.9.3/bmw_lobster_tool_trlc.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       36 2023-05-09 09:58:20.000000 bmw-lobster-tool-trlc-0.9.3/bmw_lobster_tool_trlc.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-09 09:58:20.000000 bmw-lobster-tool-trlc-0.9.3/bmw_lobster_tool_trlc.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:20.152661 bmw-lobster-tool-trlc-0.9.3/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:20.152661 bmw-lobster-tool-trlc-0.9.3/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:20.156661 bmw-lobster-tool-trlc-0.9.3/lobster/tools/trlc/
--rw-r--r--   0 florian   (1000) florian   (1000)    15532 2023-05-09 09:58:19.000000 bmw-lobster-tool-trlc-0.9.3/lobster/tools/trlc/trlc.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-09 09:58:20.156661 bmw-lobster-tool-trlc-0.9.3/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2257 2023-05-09 09:58:11.000000 bmw-lobster-tool-trlc-0.9.3/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/
+-rw-r--r--   0 florian   (1000) florian   (1000)     3210 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     2282 2023-06-13 09:17:37.000000 bmw-lobster-tool-trlc-0.9.4/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     3210 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      317 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       62 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       36 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/lobster/tools/trlc/
+-rw-r--r--   0 florian   (1000) florian   (1000)    15533 2023-06-13 09:18:56.000000 bmw-lobster-tool-trlc-0.9.4/lobster/tools/trlc/trlc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-13 09:18:56.525239 bmw-lobster-tool-trlc-0.9.4/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2257 2023-06-13 09:17:37.000000 bmw-lobster-tool-trlc-0.9.4/setup.py
```

### Comparing `bmw-lobster-tool-trlc-0.9.3/PKG-INFO` & `bmw-lobster-tool-trlc-0.9.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-trlc
-Version: 0.9.3
+Version: 0.9.4
 Summary: LOBSTER Tool for TRLC
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
 
 This package contains a tool to interface with the proprietary
 requirements management tool
 [Codebeamer](https://intland.com/codebeamer).
```

### Comparing `bmw-lobster-tool-trlc-0.9.3/README.md` & `bmw-lobster-tool-trlc-0.9.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # LOBSTER
 
-The **L**ightweight **O**pen **B**MW **S**oftware **T**racability
-**E**vidence **R**eport allows you to demonstrate software tracability
+The **L**ightweight **O**pen **B**MW **S**oftware **T**raceability
+**E**vidence **R**eport allows you to demonstrate software traceability
 and requirements coverage, which is essential for meeting standards
 such as ISO 26262.
 
 This package contains a tool to interface with the proprietary
 requirements management tool
 [Codebeamer](https://intland.com/codebeamer).
```

### Comparing `bmw-lobster-tool-trlc-0.9.3/bmw_lobster_tool_trlc.egg-info/PKG-INFO` & `bmw-lobster-tool-trlc-0.9.4/bmw_lobster_tool_trlc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-trlc
-Version: 0.9.3
+Version: 0.9.4
 Summary: LOBSTER Tool for TRLC
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
 
 This package contains a tool to interface with the proprietary
 requirements management tool
 [Codebeamer](https://intland.com/codebeamer).
```

### Comparing `bmw-lobster-tool-trlc-0.9.3/lobster/tools/trlc/trlc.py` & `bmw-lobster-tool-trlc-0.9.4/lobster/tools/trlc/trlc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 #
-# LOBSTER - Lightweight Open BMW Software Tracability Evidence Report
+# LOBSTER - Lightweight Open BMW Software Traceability Evidence Report
 # Copyright (C) 2023 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `bmw-lobster-tool-trlc-0.9.3/setup.py` & `bmw-lobster-tool-trlc-0.9.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     long_description_content_type="text/markdown",
     url=project_urls["Source Code"],
     project_urls=project_urls,
     license="GNU Affero General Public License v3",
     packages=["lobster.tools.trlc"],
     install_requires=[
         "bmw-lobster-core>=%s" % version.LOBSTER_VERSION,
-        "trlc>=1.1.4"
+        "trlc>=1.1.5"
     ],
     python_requires=">=3.7, <4",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
```

