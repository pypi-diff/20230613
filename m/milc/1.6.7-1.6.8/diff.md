# Comparing `tmp/milc-1.6.7.tar.gz` & `tmp/milc-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/milc-1.6.7.tar", last modified: Tue Jun 13 00:17:44 2023, max compression
+gzip compressed data, was "dist/milc-1.6.8.tar", last modified: Tue Jun 13 00:20:06 2023, max compression
```

## Comparing `milc-1.6.7.tar` & `milc-1.6.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:17:44.000000 milc-1.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-13 00:16:27.000000 milc-1.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-13 00:17:44.000000 milc-1.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-13 00:16:27.000000 milc-1.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:17:44.000000 milc-1.6.7/milc/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-13 00:17:42.000000 milc-1.6.7/milc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-13 00:16:27.000000 milc-1.6.7/milc/_in_argv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-13 00:16:27.000000 milc-1.6.7/milc/_sparkline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-13 00:16:27.000000 milc-1.6.7/milc/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-13 00:16:27.000000 milc-1.6.7/milc/attrdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-13 00:16:27.000000 milc-1.6.7/milc/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-13 00:16:27.000000 milc-1.6.7/milc/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    30285 2023-06-13 00:16:27.000000 milc-1.6.7/milc/milc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-06-13 00:16:27.000000 milc-1.6.7/milc/questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:17:44.000000 milc-1.6.7/milc/subcommand/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:16:27.000000 milc-1.6.7/milc/subcommand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-13 00:16:27.000000 milc-1.6.7/milc/subcommand/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-06-13 00:16:27.000000 milc-1.6.7/milc-color
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:17:44.000000 milc-1.6.7/milc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-13 00:17:44.000000 milc-1.6.7/milc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 00:17:44.000000 milc-1.6.7/milc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:17:44.000000 milc-1.6.7/milc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 00:17:44.000000 milc-1.6.7/milc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 00:17:44.000000 milc-1.6.7/milc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-13 00:17:44.000000 milc-1.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-13 00:16:27.000000 milc-1.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:20:06.000000 milc-1.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-13 00:19:06.000000 milc-1.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-13 00:20:06.000000 milc-1.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-13 00:19:06.000000 milc-1.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:20:06.000000 milc-1.6.8/milc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-13 00:20:04.000000 milc-1.6.8/milc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-13 00:19:06.000000 milc-1.6.8/milc/_in_argv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-13 00:19:06.000000 milc-1.6.8/milc/_sparkline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-13 00:19:06.000000 milc-1.6.8/milc/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-13 00:19:06.000000 milc-1.6.8/milc/attrdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-13 00:19:06.000000 milc-1.6.8/milc/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-13 00:19:06.000000 milc-1.6.8/milc/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30285 2023-06-13 00:19:06.000000 milc-1.6.8/milc/milc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-06-13 00:19:06.000000 milc-1.6.8/milc/questions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:20:06.000000 milc-1.6.8/milc/subcommand/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:19:06.000000 milc-1.6.8/milc/subcommand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-13 00:19:06.000000 milc-1.6.8/milc/subcommand/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-06-13 00:19:06.000000 milc-1.6.8/milc-color
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:20:06.000000 milc-1.6.8/milc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-13 00:20:06.000000 milc-1.6.8/milc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 00:20:06.000000 milc-1.6.8/milc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:20:06.000000 milc-1.6.8/milc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 00:20:06.000000 milc-1.6.8/milc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 00:20:06.000000 milc-1.6.8/milc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-13 00:20:06.000000 milc-1.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-13 00:19:06.000000 milc-1.6.8/setup.py
```

### Comparing `milc-1.6.7/LICENSE` & `milc-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `milc-1.6.7/PKG-INFO` & `milc-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milc
-Version: 1.6.7
+Version: 1.6.8
 Summary: Opinionated Batteries-Included Python 3 CLI Framework.
 Home-page: https://milc.clueboard.co/
 Author: skullydazed
 Author-email: skullydazed@gmail.com
 Maintainer: skullydazed
 Maintainer-email: skullydazed@gmail.com
 License: MIT License
```

### Comparing `milc-1.6.7/README.md` & `milc-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `milc-1.6.7/milc/__init__.py` & `milc-1.6.8/milc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 most common unix tool pattern- small tools that are run from the command
 line and generally do not feature any user interaction while they run.
 
 For more details see the MILC documentation:
 
     <https://github.com/clueboard/milc/tree/master/docs>
 """
-__VERSION__ = '1.6.7'
+__VERSION__ = '1.6.8'
 
 import logging
 import os
 import sys
 import warnings
 
 from .emoji import EMOJI_LOGLEVELS
```

### Comparing `milc-1.6.7/milc/_in_argv.py` & `milc-1.6.8/milc/_in_argv.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.7/milc/_sparkline.py` & `milc-1.6.8/milc/_sparkline.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.7/milc/ansi.py` & `milc-1.6.8/milc/ansi.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.7/milc/attrdict.py` & `milc-1.6.8/milc/attrdict.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.7/milc/configuration.py` & `milc-1.6.8/milc/configuration.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.7/milc/emoji.py` & `milc-1.6.8/milc/emoji.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.7/milc/milc.py` & `milc-1.6.8/milc/milc.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.7/milc/questions.py` & `milc-1.6.8/milc/questions.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.7/milc/subcommand/config.py` & `milc-1.6.8/milc/subcommand/config.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.7/milc-color` & `milc-1.6.8/milc-color`

 * *Files identical despite different names*

### Comparing `milc-1.6.7/milc.egg-info/PKG-INFO` & `milc-1.6.8/milc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milc
-Version: 1.6.7
+Version: 1.6.8
 Summary: Opinionated Batteries-Included Python 3 CLI Framework.
 Home-page: https://milc.clueboard.co/
 Author: skullydazed
 Author-email: skullydazed@gmail.com
 Maintainer: skullydazed
 Maintainer-email: skullydazed@gmail.com
 License: MIT License
```

### Comparing `milc-1.6.7/setup.cfg` & `milc-1.6.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.6.7
+current_version = 1.6.8
 commit = True
 tag = True
 tag_name = {new_version}
 message = New release: {current_version} → {new_version}
 
 [bumpversion:file:example]
```

### Comparing `milc-1.6.7/setup.py` & `milc-1.6.8/setup.py`

 * *Files identical despite different names*

