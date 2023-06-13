# Comparing `tmp/milc-1.6.6.tar.gz` & `tmp/milc-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/milc-1.6.6.tar", last modified: Sun Mar 27 19:55:08 2022, max compression
+gzip compressed data, was "dist/milc-1.6.7.tar", last modified: Tue Jun 13 00:17:44 2023, max compression
```

## Comparing `milc-1.6.6.tar` & `milc-1.6.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 19:55:08.000000 milc-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2022-03-27 19:54:08.000000 milc-1.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9496 2022-03-27 19:55:08.000000 milc-1.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6885 2022-03-27 19:54:08.000000 milc-1.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 19:55:08.000000 milc-1.6.6/milc/
--rw-r--r--   0 runner    (1001) docker     (121)     2054 2022-03-27 19:55:05.000000 milc-1.6.6/milc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-03-27 19:54:08.000000 milc-1.6.6/milc/_in_argv.py
--rw-r--r--   0 runner    (1001) docker     (121)     4566 2022-03-27 19:54:08.000000 milc-1.6.6/milc/_sparkline.py
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-03-27 19:54:08.000000 milc-1.6.6/milc/ansi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-03-27 19:54:08.000000 milc-1.6.6/milc/attrdict.py
--rw-r--r--   0 runner    (1001) docker     (121)     4870 2022-03-27 19:54:08.000000 milc-1.6.6/milc/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-03-27 19:54:08.000000 milc-1.6.6/milc/emoji.py
--rw-r--r--   0 runner    (1001) docker     (121)    29886 2022-03-27 19:54:08.000000 milc-1.6.6/milc/milc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8015 2022-03-27 19:54:08.000000 milc-1.6.6/milc/questions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 19:55:08.000000 milc-1.6.6/milc/subcommand/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-27 19:54:08.000000 milc-1.6.6/milc/subcommand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4152 2022-03-27 19:54:08.000000 milc-1.6.6/milc/subcommand/config.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1334 2022-03-27 19:54:08.000000 milc-1.6.6/milc-color
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-27 19:55:08.000000 milc-1.6.6/milc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9496 2022-03-27 19:55:08.000000 milc-1.6.6/milc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-03-27 19:55:08.000000 milc-1.6.6/milc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-27 19:55:08.000000 milc-1.6.6/milc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-03-27 19:55:08.000000 milc-1.6.6/milc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-03-27 19:55:08.000000 milc-1.6.6/milc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-03-27 19:55:08.000000 milc-1.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-03-27 19:54:08.000000 milc-1.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:17:44.000000 milc-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-13 00:16:27.000000 milc-1.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-13 00:17:44.000000 milc-1.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-13 00:16:27.000000 milc-1.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:17:44.000000 milc-1.6.7/milc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-13 00:17:42.000000 milc-1.6.7/milc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-13 00:16:27.000000 milc-1.6.7/milc/_in_argv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-13 00:16:27.000000 milc-1.6.7/milc/_sparkline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-13 00:16:27.000000 milc-1.6.7/milc/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-13 00:16:27.000000 milc-1.6.7/milc/attrdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-13 00:16:27.000000 milc-1.6.7/milc/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-13 00:16:27.000000 milc-1.6.7/milc/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30285 2023-06-13 00:16:27.000000 milc-1.6.7/milc/milc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-06-13 00:16:27.000000 milc-1.6.7/milc/questions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:17:44.000000 milc-1.6.7/milc/subcommand/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:16:27.000000 milc-1.6.7/milc/subcommand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-13 00:16:27.000000 milc-1.6.7/milc/subcommand/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-06-13 00:16:27.000000 milc-1.6.7/milc-color
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:17:44.000000 milc-1.6.7/milc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-13 00:17:44.000000 milc-1.6.7/milc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 00:17:44.000000 milc-1.6.7/milc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:17:44.000000 milc-1.6.7/milc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 00:17:44.000000 milc-1.6.7/milc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 00:17:44.000000 milc-1.6.7/milc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-13 00:17:44.000000 milc-1.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-13 00:16:27.000000 milc-1.6.7/setup.py
```

### Comparing `milc-1.6.6/LICENSE` & `milc-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `milc-1.6.6/PKG-INFO` & `milc-1.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milc
-Version: 1.6.6
+Version: 1.6.7
 Summary: Opinionated Batteries-Included Python 3 CLI Framework.
 Home-page: https://milc.clueboard.co/
 Author: skullydazed
 Author-email: skullydazed@gmail.com
 Maintainer: skullydazed
 Maintainer-email: skullydazed@gmail.com
 License: MIT License
```

### Comparing `milc-1.6.6/README.md` & `milc-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `milc-1.6.6/milc/__init__.py` & `milc-1.6.7/milc/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 most common unix tool pattern- small tools that are run from the command
 line and generally do not feature any user interaction while they run.
 
 For more details see the MILC documentation:
 
     <https://github.com/clueboard/milc/tree/master/docs>
 """
-__VERSION__ = '1.6.6'
+__VERSION__ = '1.6.7'
 
 import logging
 import os
 import sys
 import warnings
 
 from .emoji import EMOJI_LOGLEVELS
@@ -35,15 +35,15 @@
 APP_AUTHOR = os.environ.get('MILC_APP_AUTHOR', APP_NAME.upper())
 
 if 'MILC_IGNORE_DEPRECATED' not in os.environ:
     for name in ('MILC_APP_NAME', 'MILC_APP_VERSION', 'MILC_APP_AUTHOR'):
         if name in os.environ:
             warnings.warn(f'Using {name} is deprecated and will not be supported in the future, please use set_metadata() instead.', stacklevel=2)
 
-logging.basicConfig(stream=os.devnull)  # Disable logging until we can configure it how the user wants
+logging.basicConfig(filename=os.devnull)  # Disable logging until we can configure it how the user wants
 
 cli = MILC(APP_NAME, APP_VERSION, APP_AUTHOR)
 
 
 def set_metadata(*, name=APP_NAME, author=APP_AUTHOR, version=APP_VERSION):
     """Set metadata about your program.
```

### Comparing `milc-1.6.6/milc/_in_argv.py` & `milc-1.6.7/milc/_in_argv.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.6/milc/_sparkline.py` & `milc-1.6.7/milc/_sparkline.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.6/milc/ansi.py` & `milc-1.6.7/milc/ansi.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.6/milc/attrdict.py` & `milc-1.6.7/milc/attrdict.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.6/milc/configuration.py` & `milc-1.6.7/milc/configuration.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.6/milc/emoji.py` & `milc-1.6.7/milc/emoji.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.6/milc/milc.py` & `milc-1.6.7/milc/milc.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,15 +286,26 @@
             self._lock.release()
 
     @lru_cache(maxsize=None)
     def find_config_file(self):
         """Locate the config file.
         """
         if _in_argv('--config-file'):
-            return Path(sys.argv[_index_argv('--config-file') + 1]).expanduser().resolve()
+            config_file_index = _index_argv('--config-file')
+            config_file_param = sys.argv[config_file_index]
+
+            if '=' in config_file_param:
+                # get the file name from the '=' assignment
+                opt, config_file = config_file_param.split('=')
+
+            else:
+                # assume the file name is next space-sep arg
+                config_file = sys.argv[config_file_index + 1]
+
+            return Path(config_file).expanduser().resolve()
 
         filedir = user_config_dir(appname=self.prog_name, appauthor=self.author)
         filename = '%s.ini' % self.prog_name
 
         return Path(filedir, filename).resolve()
 
     def argument(self, *args, **kwargs):
```

### Comparing `milc-1.6.6/milc/questions.py` & `milc-1.6.7/milc/questions.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.6/milc/subcommand/config.py` & `milc-1.6.7/milc/subcommand/config.py`

 * *Files identical despite different names*

### Comparing `milc-1.6.6/milc-color` & `milc-1.6.7/milc-color`

 * *Files identical despite different names*

### Comparing `milc-1.6.6/milc.egg-info/PKG-INFO` & `milc-1.6.7/milc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milc
-Version: 1.6.6
+Version: 1.6.7
 Summary: Opinionated Batteries-Included Python 3 CLI Framework.
 Home-page: https://milc.clueboard.co/
 Author: skullydazed
 Author-email: skullydazed@gmail.com
 Maintainer: skullydazed
 Maintainer-email: skullydazed@gmail.com
 License: MIT License
```

### Comparing `milc-1.6.6/setup.cfg` & `milc-1.6.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.6.6
+current_version = 1.6.7
 commit = True
 tag = True
 tag_name = {new_version}
 message = New release: {current_version} → {new_version}
 
 [bumpversion:file:example]
```

### Comparing `milc-1.6.6/setup.py` & `milc-1.6.7/setup.py`

 * *Files identical despite different names*

