# Comparing `tmp/cs.debug-20230610.tar.gz` & `tmp/cs.debug-20230613.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.debug-20230610.tar", last modified: Sat Jun 10 05:47:59 2023, max compression
+gzip compressed data, was "cs.debug-20230613.tar", last modified: Tue Jun 13 00:57:52 2023, max compression
```

## Comparing `cs.debug-20230610.tar` & `cs.debug-20230613.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-10 05:47:59.380517 cs.debug-20230610/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-10 05:47:37.000000 cs.debug-20230610/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     5601 2023-06-10 05:47:59.380653 cs.debug-20230610/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     5036 2023-06-10 05:47:40.000000 cs.debug-20230610/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-10 05:47:59.374218 cs.debug-20230610/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-10 05:47:59.374569 cs.debug-20230610/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-10 05:47:59.376742 cs.debug-20230610/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    17739 2023-06-10 05:47:28.000000 cs.debug-20230610/lib/python/cs/debug.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-10 05:47:59.380220 cs.debug-20230610/lib/python/cs.debug.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     5601 2023-06-10 05:47:59.000000 cs.debug-20230610/lib/python/cs.debug.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      292 2023-06-10 05:47:59.000000 cs.debug-20230610/lib/python/cs.debug.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-10 05:47:59.000000 cs.debug-20230610/lib/python/cs.debug.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      199 2023-06-10 05:47:59.000000 cs.debug-20230610/lib/python/cs.debug.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-10 05:47:59.000000 cs.debug-20230610/lib/python/cs.debug.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     6018 2023-06-10 05:47:49.000000 cs.debug-20230610/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1041 2023-06-10 05:47:59.381561 cs.debug-20230610/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-10 05:47:40.000000 cs.debug-20230610/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 00:57:52.497942 cs.debug-20230613/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-13 00:57:30.000000 cs.debug-20230613/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6035 2023-06-13 00:57:52.498073 cs.debug-20230613/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5470 2023-06-13 00:57:33.000000 cs.debug-20230613/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 00:57:52.493163 cs.debug-20230613/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 00:57:52.493519 cs.debug-20230613/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 00:57:52.495685 cs.debug-20230613/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    19453 2023-06-13 00:57:17.000000 cs.debug-20230613/lib/python/cs/debug.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 00:57:52.497660 cs.debug-20230613/lib/python/cs.debug.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6035 2023-06-13 00:57:52.000000 cs.debug-20230613/lib/python/cs.debug.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      292 2023-06-13 00:57:52.000000 cs.debug-20230613/lib/python/cs.debug.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-13 00:57:52.000000 cs.debug-20230613/lib/python/cs.debug.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      199 2023-06-13 00:57:52.000000 cs.debug-20230613/lib/python/cs.debug.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-13 00:57:52.000000 cs.debug-20230613/lib/python/cs.debug.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6452 2023-06-13 00:57:43.000000 cs.debug-20230613/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1041 2023-06-13 00:57:52.498685 cs.debug-20230613/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-13 00:57:33.000000 cs.debug-20230613/setup.py
```

### Comparing `cs.debug-20230610/PKG-INFO` & `cs.debug-20230613/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,23 @@
-Metadata-Version: 2.1
-Name: cs.debug
-Version: 20230610
-Summary: Assorted debugging facilities.
-Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
-Author: Cameron Simpson
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python2,python3
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
-
 Assorted debugging facilities.
 
-*Latest release 20230610*:
-* DebuggingRLock fixes.
-* Move @trace from cs.py.func to cs.debug.
-* Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
-* Rename threading.Thread to threading_Thread.
-* Simplify the debugging lock classes.
+*Latest release 20230613*:
+Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
+
+If the environment variable $CS_DEBUG_BUILTINS is set to a comma
+separated list of names then the `builtins` module will be monkey
+patched with those names, enabling trite debug use of those names
+anywhere in the code provided this module has been imported somewhere.
+The allowed names are the following:
+* `X`: `cs.x.X`
+* `pformat`: `pprint.pformat`
+* `pprint`: `pprint.pprint`
+* `r`: `cs.lex.r`
+* `s`: `cs.lex.s`
+* `trace`: `cs.debug.trace` (the `@trace` decorator)
 
 ## Function `DEBUG(f, force=False)`
 
 Decorator to wrap functions in timing and value debuggers.
 
 ## Function `debug_object_shell(o, prompt=None)`
 
@@ -38,25 +26,34 @@
 ## Class `DebuggingLock(DebugWrapper, types.SimpleNamespace)`
 
 Wrapper class for `threading.Lock` to trace creation and use.
 
 `cs.threads.Lock()` returns one of these in debug mode or a raw
 `threading.Lock` otherwise.
 
+*Method `DebuggingLock.acquire(self, *a)`*:
+Acquire the lock.
+
+*Method `DebuggingLock.release(self)`*:
+Release the lock.
+
 ## Class `DebuggingRLock(DebugWrapper, types.SimpleNamespace)`
 
 Wrapper class for threading.RLock to trace creation and use.
 
 `cs.threads.RLock()` returns on of these in debug mode or a raw
 `threading.RLock` otherwise.
 
 ## Class `DebugShell(cmd.Cmd)`
 
 An interactive prompt for python statements, attached to `/dev/tty` by default.
 
+*Method `DebugShell.default(self, line)`*:
+Default command action.
+
 ## Class `DebugWrapper(types.SimpleNamespace)`
 
 Base class for classes presenting debugging wrappers.
 
 ## Function `DF(func, *a, **kw)`
 
 Wrapper for a function call to debug its use.
@@ -67,14 +64,20 @@
 ## Class `Lock(DebugWrapper, types.SimpleNamespace)`
 
 Wrapper class for `threading.Lock` to trace creation and use.
 
 `cs.threads.Lock()` returns one of these in debug mode or a raw
 `threading.Lock` otherwise.
 
+*Method `Lock.acquire(self, *a)`*:
+Acquire the lock.
+
+*Method `Lock.release(self)`*:
+Release the lock.
+
 ## Function `openfiles(substr=None, pid=None)`
 
 Run lsof(8) against process `pid`
 returning paths of open files whose paths contain `substr`.
 
 Parameters:
 * `substr`: default substring to select by; default returns all paths.
@@ -129,14 +132,17 @@
 
 Context manager to trace start and end of a code suite.
 
 # Release Log
 
 
 
+*Release 20230613*:
+Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
+
 *Release 20230610*:
 * DebuggingRLock fixes.
 * Move @trace from cs.py.func to cs.debug.
 * Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
 * Rename threading.Thread to threading_Thread.
 * Simplify the debugging lock classes.
```

### Comparing `cs.debug-20230610/README.md` & `cs.debug-20230613/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,66 @@
+[project]
+name = "cs.debug"
+description = "Assorted debugging facilities."
+authors = [
+    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
+]
+keywords = [
+    "python2",
+    "python3",
+]
+dependencies = [
+    "cs.deco>=20230331",
+    "cs.fs>=20230401",
+    "cs.lex>=20230401",
+    "cs.logutils>=20230212",
+    "cs.obj>=20220918",
+    "cs.pfx>=20230604",
+    "cs.py.func>=20230331",
+    "cs.py.stack>=20220918",
+    "cs.py3>=20220523",
+    "cs.seq>=20221118",
+    "cs.x>=20230331",
+]
+classifiers = [
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 2",
+    "Programming Language :: Python :: 3",
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+]
+version = "20230613"
+
+[project.license]
+text = "GNU General Public License v3 or later (GPLv3+)"
+
+[project.urls]
+URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
+
+[project.readme]
+text = """
 Assorted debugging facilities.
 
-*Latest release 20230610*:
-* DebuggingRLock fixes.
-* Move @trace from cs.py.func to cs.debug.
-* Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
-* Rename threading.Thread to threading_Thread.
-* Simplify the debugging lock classes.
+*Latest release 20230613*:
+Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
+
+If the environment variable $CS_DEBUG_BUILTINS is set to a comma
+separated list of names then the `builtins` module will be monkey
+patched with those names, enabling trite debug use of those names
+anywhere in the code provided this module has been imported somewhere.
+The allowed names are the following:
+* `X`: `cs.x.X`
+* `pformat`: `pprint.pformat`
+* `pprint`: `pprint.pprint`
+* `r`: `cs.lex.r`
+* `s`: `cs.lex.s`
+* `trace`: `cs.debug.trace` (the `@trace` decorator)
 
 ## Function `DEBUG(f, force=False)`
 
 Decorator to wrap functions in timing and value debuggers.
 
 ## Function `debug_object_shell(o, prompt=None)`
 
@@ -18,34 +69,25 @@
 ## Class `DebuggingLock(DebugWrapper, types.SimpleNamespace)`
 
 Wrapper class for `threading.Lock` to trace creation and use.
 
 `cs.threads.Lock()` returns one of these in debug mode or a raw
 `threading.Lock` otherwise.
 
-*Method `DebuggingLock.acquire(self, *a)`*:
-Acquire the lock.
-
-*Method `DebuggingLock.release(self)`*:
-Release the lock.
-
 ## Class `DebuggingRLock(DebugWrapper, types.SimpleNamespace)`
 
 Wrapper class for threading.RLock to trace creation and use.
 
 `cs.threads.RLock()` returns on of these in debug mode or a raw
 `threading.RLock` otherwise.
 
 ## Class `DebugShell(cmd.Cmd)`
 
 An interactive prompt for python statements, attached to `/dev/tty` by default.
 
-*Method `DebugShell.default(self, line)`*:
-Default command action.
-
 ## Class `DebugWrapper(types.SimpleNamespace)`
 
 Base class for classes presenting debugging wrappers.
 
 ## Function `DF(func, *a, **kw)`
 
 Wrapper for a function call to debug its use.
@@ -56,20 +98,14 @@
 ## Class `Lock(DebugWrapper, types.SimpleNamespace)`
 
 Wrapper class for `threading.Lock` to trace creation and use.
 
 `cs.threads.Lock()` returns one of these in debug mode or a raw
 `threading.Lock` otherwise.
 
-*Method `Lock.acquire(self, *a)`*:
-Acquire the lock.
-
-*Method `Lock.release(self)`*:
-Release the lock.
-
 ## Function `openfiles(substr=None, pid=None)`
 
 Run lsof(8) against process `pid`
 returning paths of open files whose paths contain `substr`.
 
 Parameters:
 * `substr`: default substring to select by; default returns all paths.
@@ -124,14 +160,17 @@
 
 Context manager to trace start and end of a code suite.
 
 # Release Log
 
 
 
+*Release 20230613*:
+Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
+
 *Release 20230610*:
 * DebuggingRLock fixes.
 * Move @trace from cs.py.func to cs.debug.
 * Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
 * Rename threading.Thread to threading_Thread.
 * Simplify the debugging lock classes.
 
@@ -152,17 +191,26 @@
 * Update imports for recentchanges.
 * New context manager TraceSuite to trace start and end of a code suite.
 
 *Release 20160918*:
 selftest(): fix parameter ordering to match unittest.
 
 *Release 20160828*:
-Update metadata with "install_requires" instead of "requires".
+Update metadata with \"install_requires\" instead of \"requires\".
 
 *Release 20160827*:
 * New openfiles() to return selected pathnames of open files via lsof(8).
 * New selftest() to invoke unittests with benefits.
 * DebugShell, a cmd.Cmd subclass for debugging - current use case calls this with self.__dict__ in a test case tearDwon.
 * debug_object_shell: convenience wrapper for DebugShell to call it on an object's attributes.
 
 *Release 20150116*:
-PyPI prep.
+PyPI prep."""
+content-type = "text/markdown"
+
+[build-system]
+requires = [
+    "setuptools >= 61.2",
+    "trove-classifiers",
+    "wheel",
+]
+build-backend = "setuptools.build_meta"
```

### Comparing `cs.debug-20230610/lib/python/cs/debug.py` & `cs.debug-20230613/lib/python/cs/debug.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,48 +2,60 @@
 #
 # Assorted debugging facilities.
 #       - Cameron Simpson <cs@cskk.id.au> 20apr2013
 #
 
 r'''
 Assorted debugging facilities.
+
+If the environment variable $CS_DEBUG_BUILTINS is set to a comma
+separated list of names then the `builtins` module will be monkey
+patched with those names, enabling trite debug use of those names
+anywhere in the code provided this module has been imported somewhere.
+The allowed names are the following:
+* `X`: `cs.x.X`
+* `pformat`: `pprint.pformat`
+* `pprint`: `pprint.pprint`
+* `r`: `cs.lex.r`
+* `s`: `cs.lex.s`
+* `trace`: `cs.debug.trace` (the `@trace` decorator)
 '''
 
 from __future__ import print_function
 from cmd import Cmd
 import inspect
 import logging
 import os
-from pprint import pformat
+from pprint import pformat, pprint  # pylint: disable=unused-import
 from subprocess import Popen, PIPE
 import sys
 from threading import (
     enumerate as enumerate_threads,
     Lock as threading_Lock,
     RLock as threading_RLock,
     Thread as threading_Thread,
 )
 import time
 import traceback
 from types import SimpleNamespace as NS
 
 from cs.deco import decorator
 from cs.fs import shortpath
-from cs.lex import s
+from cs.lex import s, r, is_identifier  # pylint: disable=unused-import
 import cs.logutils
 from cs.logutils import debug, error, warning, D, ifdebug, loginfo
 from cs.obj import Proxy
 from cs.pfx import Pfx
 from cs.py.func import funccite, func_a_kw_fmt
 from cs.py.stack import caller
 from cs.py3 import Queue, Queue_Empty, exec_code
 from cs.seq import seq
 from cs.x import X
 
-__version__ = '20230610'
+__version__ = '20230613'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
@@ -59,14 +71,20 @@
         'cs.py.stack',
         'cs.py3',
         'cs.seq',
         'cs.x',
     ],
 }
 
+# environment variable specifying names to become built in
+CS_DEBUG_BUILTINS_ENVVAR = 'CS_DEBUG_BUILTINS'
+
+# white list of allowed builtin names
+CS_DEBUG_BUILTINS_NAMES = ('X', 'pformat', 'pprint', 's', 'r', 'trace')
+
 # @DEBUG dispatches a thread to monitor function elapsed time.
 # This is how often it polls for function completion.
 DEBUG_POLL_RATE = 0.25
 
 class TimingOutLock(object):
   ''' A `Lock` replacement which times out, used for locating deadlock points.
   '''
@@ -640,7 +658,35 @@
   import importlib
   importlib.import_module(module_name)
   import signal
   signal.signal(signal.SIGHUP, lambda sig, frame: thread_dump())
   signal.signal(signal.SIGINT, lambda sig, frame: sys.exit(thread_dump()))
   import unittest
   return unittest.main(module=module_name, defaultTest=defaultTest, argv=argv)
+
+builtin_names_s = os.environ.get(CS_DEBUG_BUILTINS_ENVVAR, '')
+if builtin_names_s:
+  try:
+    import builtins  # pylint: disable=unused-import
+  except ImportError:
+    warning(
+        "$%s=%r but connot import builtins for monkey patching",
+        CS_DEBUG_BUILTINS_ENVVAR, builtin_names_s
+    )
+  else:
+    for builtin_name in builtin_names_s.split(','):
+      if not builtin_name:
+        continue
+      if builtin_name not in CS_DEBUG_BUILTINS_NAMES:
+        warning(
+            "$%s: ignoring %r, not in CS_DEBUG_BUILTINS_NAMES:%r",
+            CS_DEBUG_BUILTINS_ENVVAR, builtin_name, CS_DEBUG_BUILTINS_NAMES
+        )
+        continue
+      if not is_identifier(builtin_name):
+        warning(
+            "$%s: ignoring %r, not an identifier", CS_DEBUG_BUILTINS_ENVVAR,
+            builtin_name
+        )
+        continue
+      # pylint: disable=eval-used
+      eval('setattr(builtins,builtin_name,{%s})' % (builtin_name,))
```

### Comparing `cs.debug-20230610/lib/python/cs.debug.egg-info/PKG-INFO` & `cs.debug-20230613/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.debug
-Version: 20230610
+Version: 20230613
 Summary: Assorted debugging facilities.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -16,20 +16,28 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted debugging facilities.
 
-*Latest release 20230610*:
-* DebuggingRLock fixes.
-* Move @trace from cs.py.func to cs.debug.
-* Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
-* Rename threading.Thread to threading_Thread.
-* Simplify the debugging lock classes.
+*Latest release 20230613*:
+Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
+
+If the environment variable $CS_DEBUG_BUILTINS is set to a comma
+separated list of names then the `builtins` module will be monkey
+patched with those names, enabling trite debug use of those names
+anywhere in the code provided this module has been imported somewhere.
+The allowed names are the following:
+* `X`: `cs.x.X`
+* `pformat`: `pprint.pformat`
+* `pprint`: `pprint.pprint`
+* `r`: `cs.lex.r`
+* `s`: `cs.lex.s`
+* `trace`: `cs.debug.trace` (the `@trace` decorator)
 
 ## Function `DEBUG(f, force=False)`
 
 Decorator to wrap functions in timing and value debuggers.
 
 ## Function `debug_object_shell(o, prompt=None)`
 
@@ -129,14 +137,17 @@
 
 Context manager to trace start and end of a code suite.
 
 # Release Log
 
 
 
+*Release 20230613*:
+Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
+
 *Release 20230610*:
 * DebuggingRLock fixes.
 * Move @trace from cs.py.func to cs.debug.
 * Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
 * Rename threading.Thread to threading_Thread.
 * Simplify the debugging lock classes.
```

### Comparing `cs.debug-20230610/pyproject.toml` & `cs.debug-20230613/lib/python/cs.debug.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,43 @@
-[project]
-name = "cs.debug"
-description = "Assorted debugging facilities."
-authors = [
-    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
-]
-keywords = [
-    "python2",
-    "python3",
-]
-dependencies = [
-    "cs.deco>=20230331",
-    "cs.fs>=20230401",
-    "cs.lex>=20230401",
-    "cs.logutils>=20230212",
-    "cs.obj>=20220918",
-    "cs.pfx>=20230604",
-    "cs.py.func>=20230331",
-    "cs.py.stack>=20220918",
-    "cs.py3>=20220523",
-    "cs.seq>=20221118",
-    "cs.x>=20230331",
-]
-classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 2",
-    "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-]
-version = "20230610"
+Metadata-Version: 2.1
+Name: cs.debug
+Version: 20230613
+Summary: Assorted debugging facilities.
+Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
+Author: Cameron Simpson
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python2,python3
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
 
-[project.license]
-text = "GNU General Public License v3 or later (GPLv3+)"
-
-[project.urls]
-URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
-
-[project.readme]
-text = """
 Assorted debugging facilities.
 
-*Latest release 20230610*:
-* DebuggingRLock fixes.
-* Move @trace from cs.py.func to cs.debug.
-* Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
-* Rename threading.Thread to threading_Thread.
-* Simplify the debugging lock classes.
+*Latest release 20230613*:
+Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
+
+If the environment variable $CS_DEBUG_BUILTINS is set to a comma
+separated list of names then the `builtins` module will be monkey
+patched with those names, enabling trite debug use of those names
+anywhere in the code provided this module has been imported somewhere.
+The allowed names are the following:
+* `X`: `cs.x.X`
+* `pformat`: `pprint.pformat`
+* `pprint`: `pprint.pprint`
+* `r`: `cs.lex.r`
+* `s`: `cs.lex.s`
+* `trace`: `cs.debug.trace` (the `@trace` decorator)
 
 ## Function `DEBUG(f, force=False)`
 
 Decorator to wrap functions in timing and value debuggers.
 
 ## Function `debug_object_shell(o, prompt=None)`
 
@@ -152,14 +137,17 @@
 
 Context manager to trace start and end of a code suite.
 
 # Release Log
 
 
 
+*Release 20230613*:
+Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
+
 *Release 20230610*:
 * DebuggingRLock fixes.
 * Move @trace from cs.py.func to cs.debug.
 * Drop Lock and RLock alias factories - importers should just use the debugging lock classes directly.
 * Rename threading.Thread to threading_Thread.
 * Simplify the debugging lock classes.
 
@@ -180,26 +168,17 @@
 * Update imports for recentchanges.
 * New context manager TraceSuite to trace start and end of a code suite.
 
 *Release 20160918*:
 selftest(): fix parameter ordering to match unittest.
 
 *Release 20160828*:
-Update metadata with \"install_requires\" instead of \"requires\".
+Update metadata with "install_requires" instead of "requires".
 
 *Release 20160827*:
 * New openfiles() to return selected pathnames of open files via lsof(8).
 * New selftest() to invoke unittests with benefits.
 * DebugShell, a cmd.Cmd subclass for debugging - current use case calls this with self.__dict__ in a test case tearDwon.
 * debug_object_shell: convenience wrapper for DebugShell to call it on an object's attributes.
 
 *Release 20150116*:
-PyPI prep."""
-content-type = "text/markdown"
-
-[build-system]
-requires = [
-    "setuptools >= 61.2",
-    "trove-classifiers",
-    "wheel",
-]
-build-backend = "setuptools.build_meta"
+PyPI prep.
```

### Comparing `cs.debug-20230610/setup.cfg` & `cs.debug-20230613/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.debug
-version = 20230610
+version = 20230613
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = Assorted debugging facilities.
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers =
```

