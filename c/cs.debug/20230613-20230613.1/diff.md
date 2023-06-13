# Comparing `tmp/cs.debug-20230613.tar.gz` & `tmp/cs.debug-20230613.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.debug-20230613.tar", last modified: Tue Jun 13 00:57:52 2023, max compression
+gzip compressed data, was "cs.debug-20230613.1.tar", last modified: Tue Jun 13 01:11:26 2023, max compression
```

## Comparing `cs.debug-20230613.tar` & `cs.debug-20230613.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 00:57:52.497942 cs.debug-20230613/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-13 00:57:30.000000 cs.debug-20230613/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     6035 2023-06-13 00:57:52.498073 cs.debug-20230613/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     5470 2023-06-13 00:57:33.000000 cs.debug-20230613/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 00:57:52.493163 cs.debug-20230613/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 00:57:52.493519 cs.debug-20230613/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 00:57:52.495685 cs.debug-20230613/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    19453 2023-06-13 00:57:17.000000 cs.debug-20230613/lib/python/cs/debug.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 00:57:52.497660 cs.debug-20230613/lib/python/cs.debug.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     6035 2023-06-13 00:57:52.000000 cs.debug-20230613/lib/python/cs.debug.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      292 2023-06-13 00:57:52.000000 cs.debug-20230613/lib/python/cs.debug.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-13 00:57:52.000000 cs.debug-20230613/lib/python/cs.debug.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      199 2023-06-13 00:57:52.000000 cs.debug-20230613/lib/python/cs.debug.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-13 00:57:52.000000 cs.debug-20230613/lib/python/cs.debug.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     6452 2023-06-13 00:57:43.000000 cs.debug-20230613/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1041 2023-06-13 00:57:52.498685 cs.debug-20230613/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-13 00:57:33.000000 cs.debug-20230613/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 01:11:26.058406 cs.debug-20230613.1/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-13 01:11:02.000000 cs.debug-20230613.1/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6022 2023-06-13 01:11:26.058545 cs.debug-20230613.1/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5455 2023-06-13 01:11:06.000000 cs.debug-20230613.1/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 01:11:26.053857 cs.debug-20230613.1/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 01:11:26.054307 cs.debug-20230613.1/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 01:11:26.056394 cs.debug-20230613.1/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    19453 2023-06-13 01:10:53.000000 cs.debug-20230613.1/lib/python/cs/debug.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 01:11:26.058138 cs.debug-20230613.1/lib/python/cs.debug.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6022 2023-06-13 01:11:26.000000 cs.debug-20230613.1/lib/python/cs.debug.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      292 2023-06-13 01:11:26.000000 cs.debug-20230613.1/lib/python/cs.debug.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-13 01:11:26.000000 cs.debug-20230613.1/lib/python/cs.debug.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      199 2023-06-13 01:11:26.000000 cs.debug-20230613.1/lib/python/cs.debug.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-13 01:11:26.000000 cs.debug-20230613.1/lib/python/cs.debug.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6439 2023-06-13 01:11:17.000000 cs.debug-20230613.1/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1043 2023-06-13 01:11:26.059136 cs.debug-20230613.1/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-13 01:11:06.000000 cs.debug-20230613.1/setup.py
```

### Comparing `cs.debug-20230613/PKG-INFO` & `cs.debug-20230613.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.debug
-Version: 20230613
+Version: 20230613.1
 Summary: Assorted debugging facilities.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -16,16 +16,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted debugging facilities.
 
-*Latest release 20230613*:
-Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
+*Latest release 20230613.1*:
+Bugfix builtins monkey patch.
 
 If the environment variable $CS_DEBUG_BUILTINS is set to a comma
 separated list of names then the `builtins` module will be monkey
 patched with those names, enabling trite debug use of those names
 anywhere in the code provided this module has been imported somewhere.
 The allowed names are the following:
 * `X`: `cs.x.X`
@@ -137,14 +137,17 @@
 
 Context manager to trace start and end of a code suite.
 
 # Release Log
 
 
 
+*Release 20230613.1*:
+Bugfix builtins monkey patch.
+
 *Release 20230613*:
 Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
 
 *Release 20230610*:
 * DebuggingRLock fixes.
 * Move @trace from cs.py.func to cs.debug.
 * Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
```

### Comparing `cs.debug-20230613/README.md` & `cs.debug-20230613.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Assorted debugging facilities.
 
-*Latest release 20230613*:
-Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
+*Latest release 20230613.1*:
+Bugfix builtins monkey patch.
 
 If the environment variable $CS_DEBUG_BUILTINS is set to a comma
 separated list of names then the `builtins` module will be monkey
 patched with those names, enabling trite debug use of those names
 anywhere in the code provided this module has been imported somewhere.
 The allowed names are the following:
 * `X`: `cs.x.X`
@@ -132,14 +132,17 @@
 
 Context manager to trace start and end of a code suite.
 
 # Release Log
 
 
 
+*Release 20230613.1*:
+Bugfix builtins monkey patch.
+
 *Release 20230613*:
 Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
 
 *Release 20230610*:
 * DebuggingRLock fixes.
 * Move @trace from cs.py.func to cs.debug.
 * Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
```

### Comparing `cs.debug-20230613/lib/python/cs/debug.py` & `cs.debug-20230613.1/lib/python/cs/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from cs.pfx import Pfx
 from cs.py.func import funccite, func_a_kw_fmt
 from cs.py.stack import caller
 from cs.py3 import Queue, Queue_Empty, exec_code
 from cs.seq import seq
 from cs.x import X
 
-__version__ = '20230613'
+__version__ = '20230613.1'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
@@ -685,8 +685,8 @@
       if not is_identifier(builtin_name):
         warning(
             "$%s: ignoring %r, not an identifier", CS_DEBUG_BUILTINS_ENVVAR,
             builtin_name
         )
         continue
       # pylint: disable=eval-used
-      eval('setattr(builtins,builtin_name,{%s})' % (builtin_name,))
+      eval('setattr(builtins,builtin_name,%s)' % (builtin_name,))
```

### Comparing `cs.debug-20230613/lib/python/cs.debug.egg-info/PKG-INFO` & `cs.debug-20230613.1/lib/python/cs.debug.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.debug
-Version: 20230613
+Version: 20230613.1
 Summary: Assorted debugging facilities.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -16,16 +16,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted debugging facilities.
 
-*Latest release 20230613*:
-Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
+*Latest release 20230613.1*:
+Bugfix builtins monkey patch.
 
 If the environment variable $CS_DEBUG_BUILTINS is set to a comma
 separated list of names then the `builtins` module will be monkey
 patched with those names, enabling trite debug use of those names
 anywhere in the code provided this module has been imported somewhere.
 The allowed names are the following:
 * `X`: `cs.x.X`
@@ -137,14 +137,17 @@
 
 Context manager to trace start and end of a code suite.
 
 # Release Log
 
 
 
+*Release 20230613.1*:
+Bugfix builtins monkey patch.
+
 *Release 20230613*:
 Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
 
 *Release 20230610*:
 * DebuggingRLock fixes.
 * Move @trace from cs.py.func to cs.debug.
 * Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
```

### Comparing `cs.debug-20230613/pyproject.toml` & `cs.debug-20230613.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,28 +27,28 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230613"
+version = "20230613.1"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Assorted debugging facilities.
 
-*Latest release 20230613*:
-Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
+*Latest release 20230613.1*:
+Bugfix builtins monkey patch.
 
 If the environment variable $CS_DEBUG_BUILTINS is set to a comma
 separated list of names then the `builtins` module will be monkey
 patched with those names, enabling trite debug use of those names
 anywhere in the code provided this module has been imported somewhere.
 The allowed names are the following:
 * `X`: `cs.x.X`
@@ -160,14 +160,17 @@
 
 Context manager to trace start and end of a code suite.
 
 # Release Log
 
 
 
+*Release 20230613.1*:
+Bugfix builtins monkey patch.
+
 *Release 20230613*:
 Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
 
 *Release 20230610*:
 * DebuggingRLock fixes.
 * Move @trace from cs.py.func to cs.debug.
 * Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
```

### Comparing `cs.debug-20230613/setup.cfg` & `cs.debug-20230613.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.debug
-version = 20230613
+version = 20230613.1
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Assorted debugging facilities.
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers =
```

