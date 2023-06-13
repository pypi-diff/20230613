# Comparing `tmp/bmw-lobster-core-0.9.3.tar.gz` & `tmp/bmw-lobster-core-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-core-0.9.3.tar", last modified: Tue May  9 09:58:19 2023, max compression
+gzip compressed data, was "bmw-lobster-core-0.9.4.tar", last modified: Tue Jun 13 09:18:56 2023, max compression
```

## Comparing `bmw-lobster-core-0.9.3.tar` & `bmw-lobster-core-0.9.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.812659 bmw-lobster-core-0.9.3/
--rw-r--r--   0 florian   (1000) florian   (1000)     2692 2023-05-09 09:58:19.812659 bmw-lobster-core-0.9.3/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1733 2023-05-08 15:03:18.000000 bmw-lobster-core-0.9.3/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.808659 bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2692 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      679 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      240 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.808659 bmw-lobster-core-0.9.3/lobster/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.808659 bmw-lobster-core-0.9.3/lobster/config/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/config/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4160 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/config/lexer.py
--rw-r--r--   0 florian   (1000) florian   (1000)     9086 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/config/parser.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2500 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/errors.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1243 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/exceptions.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.808659 bmw-lobster-core-0.9.3/lobster/html/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/html/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2682 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/html/assets.py
--rw-r--r--   0 florian   (1000) florian   (1000)     9667 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/html/htmldoc.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4401 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/io.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11204 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/items.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7161 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/location.py
--rw-r--r--   0 florian   (1000) florian   (1000)     8157 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/report.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.804659 bmw-lobster-core-0.9.3/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.812659 bmw-lobster-core-0.9.3/lobster/tools/core/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/tools/core/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     1917 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/tools/core/ci_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)    15949 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/tools/core/html_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     3707 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/tools/core/online_report.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     1817 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/tools/core/report.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1025 2023-05-09 09:58:19.000000 bmw-lobster-core-0.9.3/lobster/version.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-09 09:58:19.812659 bmw-lobster-core-0.9.3/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2513 2023-05-08 15:03:18.000000 bmw-lobster-core-0.9.3/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2695 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1735 2023-06-13 09:17:37.000000 bmw-lobster-core-0.9.4/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.185235 bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2695 2023-06-13 09:18:56.000000 bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      679 2023-06-13 09:18:56.000000 bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-13 09:18:56.000000 bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      240 2023-06-13 09:18:56.000000 bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-13 09:18:56.000000 bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/lobster/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/lobster/config/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/config/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4161 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/config/lexer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     9087 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/config/parser.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2501 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/errors.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1244 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/exceptions.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/lobster/html/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/html/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2682 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/html/assets.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     9667 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/html/htmldoc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4402 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/io.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11205 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/items.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7162 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/location.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     8158 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/report.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.185235 bmw-lobster-core-0.9.4/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/lobster/tools/core/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/tools/core/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     1917 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/tools/core/ci_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)    15951 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/tools/core/html_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     3707 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/tools/core/online_report.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     1818 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/tools/core/report.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1026 2023-06-13 09:18:55.000000 bmw-lobster-core-0.9.4/lobster/version.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-13 09:18:56.189235 bmw-lobster-core-0.9.4/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2514 2023-06-13 09:17:37.000000 bmw-lobster-core-0.9.4/setup.py
```

### Comparing `bmw-lobster-core-0.9.3/PKG-INFO` & `bmw-lobster-core-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-core
-Version: 0.9.3
-Summary: Lightweight Open BMW Software Tracability Evidence Report
+Version: 0.9.4
+Summary: Lightweight Open BMW Software Traceability Evidence Report
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
 Project-URL: Source Code, https://github.com/bmw-software-engineering/lobster
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
 
 This package contains the core LOBSTER tools: the basic API and tools
 for generating reports.
 
 ## Tools
```

### Comparing `bmw-lobster-core-0.9.3/README.md` & `bmw-lobster-core-0.9.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # LOBSTER
 
-The **L**ightweight **O**pen **B**MW **S**oftware **T**racability
-**E**vidence **R**eport allows you to demonstrate software tracability
+The **L**ightweight **O**pen **B**MW **S**oftware **T**raceability
+**E**vidence **R**eport allows you to demonstrate software traceability
 and requirements coverage, which is essential for meeting standards
 such as ISO 26262.
 
 This package contains the core LOBSTER tools: the basic API and tools
 for generating reports.
 
 ## Tools
```

### Comparing `bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/PKG-INFO` & `bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-core
-Version: 0.9.3
-Summary: Lightweight Open BMW Software Tracability Evidence Report
+Version: 0.9.4
+Summary: Lightweight Open BMW Software Traceability Evidence Report
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
 Project-URL: Source Code, https://github.com/bmw-software-engineering/lobster
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
 
 This package contains the core LOBSTER tools: the basic API and tools
 for generating reports.
 
 ## Tools
```

### Comparing `bmw-lobster-core-0.9.3/bmw_lobster_core.egg-info/SOURCES.txt` & `bmw-lobster-core-0.9.4/bmw_lobster_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.3/lobster/config/lexer.py` & `bmw-lobster-core-0.9.4/lobster/config/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 #
-# LOBSTER - Lightweight Open BMW Software Tracability Evidence Report
+# LOBSTER - Lightweight Open BMW Software Traceability Evidence Report
 # Copyright (C) 2022 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `bmw-lobster-core-0.9.3/lobster/config/parser.py` & `bmw-lobster-core-0.9.4/lobster/config/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 #
-# LOBSTER - Lightweight Open BMW Software Tracability Evidence Report
+# LOBSTER - Lightweight Open BMW Software Traceability Evidence Report
 # Copyright (C) 2022 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `bmw-lobster-core-0.9.3/lobster/errors.py` & `bmw-lobster-core-0.9.4/lobster/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 #
-# LOBSTER - Lightweight Open BMW Software Tracability Evidence Report
+# LOBSTER - Lightweight Open BMW Software Traceability Evidence Report
 # Copyright (C) 2022-2023 Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
 #
```

### Comparing `bmw-lobster-core-0.9.3/lobster/exceptions.py` & `bmw-lobster-core-0.9.4/lobster/exceptions.py`

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

### Comparing `bmw-lobster-core-0.9.3/lobster/html/assets.py` & `bmw-lobster-core-0.9.4/lobster/html/assets.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.3/lobster/html/htmldoc.py` & `bmw-lobster-core-0.9.4/lobster/html/htmldoc.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.3/lobster/io.py` & `bmw-lobster-core-0.9.4/lobster/io.py`

 * *Files 2% similar despite different names*

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

### Comparing `bmw-lobster-core-0.9.3/lobster/items.py` & `bmw-lobster-core-0.9.4/lobster/items.py`

 * *Files 0% similar despite different names*

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

### Comparing `bmw-lobster-core-0.9.3/lobster/location.py` & `bmw-lobster-core-0.9.4/lobster/location.py`

 * *Files 0% similar despite different names*

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

### Comparing `bmw-lobster-core-0.9.3/lobster/report.py` & `bmw-lobster-core-0.9.4/lobster/report.py`

 * *Files 0% similar despite different names*

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

### Comparing `bmw-lobster-core-0.9.3/lobster/tools/core/ci_report.py` & `bmw-lobster-core-0.9.4/lobster/tools/core/ci_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.3/lobster/tools/core/html_report.py` & `bmw-lobster-core-0.9.4/lobster/tools/core/html_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
 
 
 def write_html(fd, report):
     assert isinstance(report, Report)
 
     doc = htmldoc.Document(
         "L.O.B.S.T.E.R.",
-        "Lightweight Open BMW Software Tracability Evidence Report"
+        "Lightweight Open BMW Software Traceability Evidence Report"
     )
 
     # Item styles
     doc.style[".item-ok, .item-partial, .item-missing, .item-justified"] = {
         "border"        : "1px solid black",
         "border-radius" : "0.5em",
         "margin-top"    : "0.4em",
@@ -396,15 +396,15 @@
                     doc.add_line("<ul>")
                 doc.add_line("<li>%s: %s</li>" %
                              (xref_item(item),
                               message))
     if has_issues:
         doc.add_line("</ul>")
     else:
-        doc.add_line("<div>No tracability issues found.</div>")
+        doc.add_line("<div>No traceability issues found.</div>")
 
     ### Report
     doc.add_heading(2, "Detailed report", "detailed-report")
     items_by_level = {}
     for level in report.config:
         items_by_level[level] = [item
                                  for item in report.items.values()
```

### Comparing `bmw-lobster-core-0.9.3/lobster/tools/core/online_report.py` & `bmw-lobster-core-0.9.4/lobster/tools/core/online_report.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-core-0.9.3/lobster/tools/core/report.py` & `bmw-lobster-core-0.9.4/lobster/tools/core/report.py`

 * *Files 3% similar despite different names*

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

### Comparing `bmw-lobster-core-0.9.3/lobster/version.py` & `bmw-lobster-core-0.9.4/lobster/version.py`

 * *Files 2% similar despite different names*

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
@@ -13,14 +13,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
 # Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public
 # License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-VERSION_TUPLE = (0, 9, 3)
+VERSION_TUPLE = (0, 9, 4)
 VERSION_SUFFIX = ""
 
 LOBSTER_VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
     ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "LOBSTER %s" % LOBSTER_VERSION
```

### Comparing `bmw-lobster-core-0.9.3/setup.py` & `bmw-lobster-core-0.9.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 }
 
 setuptools.setup(
     name="bmw-lobster-core",
     version=version.LOBSTER_VERSION,
     author="Bayerische Motoren Werke Aktiengesellschaft (BMW AG)",
     author_email="florian.schanda@bmw.de",
-    description="Lightweight Open BMW Software Tracability Evidence Report",
+    description="Lightweight Open BMW Software Traceability Evidence Report",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=project_urls["Source Code"],
     project_urls=project_urls,
     license="GNU Affero General Public License v3",
     packages=["lobster",
               "lobster.config",
```

