# Comparing `tmp/janis-pipelines.unix-0.9.1.tar.gz` & `tmp/janis-pipelines.unix-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/janis-pipelines.unix-0.9.1.tar", last modified: Wed Apr 22 09:18:12 2020, max compression
+gzip compressed data, was "dist/janis-pipelines.unix-0.9.2.tar", last modified: Fri Jun 19 03:05:54 2020, max compression
```

## Comparing `janis-pipelines.unix-0.9.1.tar` & `janis-pipelines.unix-0.9.2.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/janis_pipelines.unix.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2095 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/janis_pipelines.unix.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/janis_pipelines.unix.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/janis_pipelines.unix.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/janis_pipelines.unix.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      857 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/janis_pipelines.unix.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/janis_pipelines.unix.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/janis_pipelines.unix.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2095 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1289 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/janis_unix/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/janis_unix/data_types/
--rw-rw-r--   0 travis    (2000) travis    (2000)      293 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/data_types/text.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      531 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/data_types/tarfile.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      285 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/data_types/pdf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/data_types/tsv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      264 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/data_types/csv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      269 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/data_types/json.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/data_types/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      277 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/data_types/zipfile.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/__meta__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 09:18:12.000000 janis-pipelines.unix-0.9.1/janis_unix/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2961 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/tools/cat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      515 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/tools/greet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      706 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/tools/compile.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      524 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/tools/untar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1559 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/tools/echo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      246 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/tools/unixtool.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1018 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/tools/hello.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      177 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      852 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/tools/tar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      101 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/janis_unix/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1422 2020-04-22 09:17:58.000000 janis-pipelines.unix-0.9.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/janis_pipelines.unix.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2081 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/janis_pipelines.unix.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/janis_pipelines.unix.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/janis_pipelines.unix.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/janis_pipelines.unix.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      917 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/janis_pipelines.unix.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/janis_pipelines.unix.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/janis_pipelines.unix.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2081 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1275 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/janis_unix/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/janis_unix/data_types/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      293 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/data_types/text.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      324 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/data_types/tarfile.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      160 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/data_types/tsv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      162 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/data_types/csv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/data_types/json.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/data_types/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      175 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/data_types/zipfile.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/__meta__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-19 03:05:54.000000 janis-pipelines.unix-0.9.2/janis_unix/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2991 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/tools/cat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      706 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/tools/compile.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2654 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/tools/uncompressarchive.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      524 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/tools/untar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1559 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/tools/echo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      623 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/tools/awk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      246 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/tools/unixtool.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      566 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/tools/sleep.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1018 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/tools/hello.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      843 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/tools/md5sum.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      277 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/tools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      852 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/tools/tar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      101 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/janis_unix/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1422 2020-06-19 03:05:39.000000 janis-pipelines.unix-0.9.2/setup.py
```

### Comparing `janis-pipelines.unix-0.9.1/janis_pipelines.unix.egg-info/PKG-INFO` & `janis-pipelines.unix-0.9.2/janis_pipelines.unix.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: janis-pipelines.unix
-Version: 0.9.1
+Version: 0.9.2
 Summary: Unix tools and data types for Janis
 Home-page: UNKNOWN
 Author: Michael Franklin, Evan Thomas, Mohammad Bhuyan
 Author-email: michael.franklin@petermac.org
 License: GNU
-Description: # Janis - Unix Toolbox
+Description: # Janis - Unix
         
         [![Documentation Status](https://readthedocs.org/projects/janis/badge/?version=latest)](https://janis.readthedocs.io/en/latest/tools/unix/index.html)
         [![Build Status](https://travis-ci.org/PMCC-BioinformaticsCore/janis-unix.svg?branch=master)](https://travis-ci.org/PMCC-BioinformaticsCore/janis-unix)
         [![PyPI version](https://badge.fury.io/py/janis-pipelines.unix.svg)](https://badge.fury.io/py/janis-pipelines.unix)
         
-        This repository is the unix toolbox for [Janis](https://github.com/PMCC-BioinformaticsCore/janis). 
+        This repository contains common unix tools and data types for [Janis](https://github.com/PMCC-BioinformaticsCore/janis).
         
-        You can see a full list of tools in the [documentation](https://janis.readthedocs.io/en/latest/tools/bioinformatics/index.html).
+        Refer to the [documentation](https://janis.readthedocs.io/en/latest/tools/bioinformatics/index.html).
         
         
         ## Data types
         
         The data types are a way of encapsulating information about a particular input or output.
         Some common unix data types are `CSV`, `TSV` or `TarFile`. Visit the documentation for a full list.
```

### Comparing `janis-pipelines.unix-0.9.1/janis_pipelines.unix.egg-info/SOURCES.txt` & `janis-pipelines.unix-0.9.2/janis_pipelines.unix.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 janis_pipelines.unix.egg-info/requires.txt
 janis_pipelines.unix.egg-info/top_level.txt
 janis_unix/__init__.py
 janis_unix/__meta__.py
 janis_unix/data_types/__init__.py
 janis_unix/data_types/csv.py
 janis_unix/data_types/json.py
-janis_unix/data_types/pdf.py
 janis_unix/data_types/tarfile.py
 janis_unix/data_types/text.py
 janis_unix/data_types/tsv.py
 janis_unix/data_types/zipfile.py
 janis_unix/tools/__init__.py
+janis_unix/tools/awk.py
 janis_unix/tools/cat.py
 janis_unix/tools/compile.py
 janis_unix/tools/echo.py
-janis_unix/tools/greet.py
 janis_unix/tools/hello.py
+janis_unix/tools/md5sum.py
+janis_unix/tools/sleep.py
 janis_unix/tools/tar.py
+janis_unix/tools/uncompressarchive.py
 janis_unix/tools/unixtool.py
 janis_unix/tools/untar.py
```

### Comparing `janis-pipelines.unix-0.9.1/PKG-INFO` & `janis-pipelines.unix-0.9.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: janis-pipelines.unix
-Version: 0.9.1
+Version: 0.9.2
 Summary: Unix tools and data types for Janis
 Home-page: UNKNOWN
 Author: Michael Franklin, Evan Thomas, Mohammad Bhuyan
 Author-email: michael.franklin@petermac.org
 License: GNU
-Description: # Janis - Unix Toolbox
+Description: # Janis - Unix
         
         [![Documentation Status](https://readthedocs.org/projects/janis/badge/?version=latest)](https://janis.readthedocs.io/en/latest/tools/unix/index.html)
         [![Build Status](https://travis-ci.org/PMCC-BioinformaticsCore/janis-unix.svg?branch=master)](https://travis-ci.org/PMCC-BioinformaticsCore/janis-unix)
         [![PyPI version](https://badge.fury.io/py/janis-pipelines.unix.svg)](https://badge.fury.io/py/janis-pipelines.unix)
         
-        This repository is the unix toolbox for [Janis](https://github.com/PMCC-BioinformaticsCore/janis). 
+        This repository contains common unix tools and data types for [Janis](https://github.com/PMCC-BioinformaticsCore/janis).
         
-        You can see a full list of tools in the [documentation](https://janis.readthedocs.io/en/latest/tools/bioinformatics/index.html).
+        Refer to the [documentation](https://janis.readthedocs.io/en/latest/tools/bioinformatics/index.html).
         
         
         ## Data types
         
         The data types are a way of encapsulating information about a particular input or output.
         Some common unix data types are `CSV`, `TSV` or `TarFile`. Visit the documentation for a full list.
```

### Comparing `janis-pipelines.unix-0.9.1/README.md` & `janis-pipelines.unix-0.9.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Janis - Unix Toolbox
+# Janis - Unix
 
 [![Documentation Status](https://readthedocs.org/projects/janis/badge/?version=latest)](https://janis.readthedocs.io/en/latest/tools/unix/index.html)
 [![Build Status](https://travis-ci.org/PMCC-BioinformaticsCore/janis-unix.svg?branch=master)](https://travis-ci.org/PMCC-BioinformaticsCore/janis-unix)
 [![PyPI version](https://badge.fury.io/py/janis-pipelines.unix.svg)](https://badge.fury.io/py/janis-pipelines.unix)
 
-This repository is the unix toolbox for [Janis](https://github.com/PMCC-BioinformaticsCore/janis). 
+This repository contains common unix tools and data types for [Janis](https://github.com/PMCC-BioinformaticsCore/janis).
 
-You can see a full list of tools in the [documentation](https://janis.readthedocs.io/en/latest/tools/bioinformatics/index.html).
+Refer to the [documentation](https://janis.readthedocs.io/en/latest/tools/bioinformatics/index.html).
 
 
 ## Data types
 
 The data types are a way of encapsulating information about a particular input or output.
 Some common unix data types are `CSV`, `TSV` or `TarFile`. Visit the documentation for a full list.
```

### Comparing `janis-pipelines.unix-0.9.1/janis_unix/tools/cat.py` & `janis-pipelines.unix-0.9.2/janis_unix/tools/cat.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,28 +39,28 @@
             ToolInput(
                 "squeeze",
                 Boolean(optional=True),
                 prefix="-s",
                 doc="Squeeze multiple adjacent empty lines, causing the output to be single spaced.",
             ),
             ToolInput(
-                "display_nonprint_2",
+                "display_nonprint_and_eol_chars",
                 Boolean(optional=True),
                 prefix="-e",
                 doc="Display non-printing characters (see the -v option), and display "
                 "a dollar sign (`$') at the end of each line.",
             ),
             ToolInput(
-                "display_nonprint_1",
+                "display_nonprint_and_tab_chars",
                 Boolean(optional=True),
                 prefix="-t",
                 doc="Display non-printing characters (see the -v option), and display tab characters as `^I'.",
             ),
             ToolInput(
-                "display_nonprint",
+                "display_nonprint_chars",
                 Boolean(optional=True),
                 prefix="-v",
                 doc="Display non-printing characters so they are visible.  Control characters print as `^X' for "
                 "control-X; the delete character (octal 0177) prints as `^?'.  Non-ASCII characters (with the"
                 " high bit set) are printed as `M-' (for meta) followed by the character for the low 7 bits.",
             ),
         ]
```

### Comparing `janis-pipelines.unix-0.9.1/janis_unix/tools/compile.py` & `janis-pipelines.unix-0.9.2/janis_unix/tools/compile.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.unix-0.9.1/janis_unix/tools/untar.py` & `janis-pipelines.unix-0.9.2/janis_unix/tools/untar.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.unix-0.9.1/janis_unix/tools/echo.py` & `janis-pipelines.unix-0.9.2/janis_unix/tools/echo.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.unix-0.9.1/janis_unix/tools/hello.py` & `janis-pipelines.unix-0.9.2/janis_unix/tools/hello.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.unix-0.9.1/janis_unix/tools/tar.py` & `janis-pipelines.unix-0.9.2/janis_unix/tools/tar.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.unix-0.9.1/setup.py` & `janis-pipelines.unix-0.9.2/setup.py`

 * *Files identical despite different names*

