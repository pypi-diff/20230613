# Comparing `tmp/borg_space-2.1.tar.gz` & `tmp/borg_space-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "borg_space-2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "borg_space-2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `borg_space-2.1.tar` & `borg_space-2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2022-10-22 21:26:19.370225 borg_space-2.1/LICENSE
--rw-r--r--   0        0        0    11958 2023-06-09 22:55:49.182337 borg_space-2.1/README.rst
--rw-r--r--   0        0        0        0 2023-05-05 05:24:18.834041 borg_space-2.1/borg_space/__init__.py
--rw-r--r--   0        0        0     8694 2023-06-09 01:54:28.616901 borg_space-2.1/borg_space/config.py
--rw-r--r--   0        0        0    10733 2023-06-09 22:55:49.180337 borg_space-2.1/borg_space/main.py
--rw-r--r--   0        0        0     3089 2023-06-07 00:28:49.138158 borg_space-2.1/borg_space/trees.py
--rw-r--r--   0        0        0     1183 2023-06-09 22:55:49.179337 borg_space-2.1/pyproject.toml
--rw-r--r--   0        0        0    13015 1970-01-01 00:00:00.000000 borg_space-2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-22 21:26:19.370225 borg_space-2.2/LICENSE
+-rw-r--r--   0        0        0    11958 2023-06-13 03:12:03.558395 borg_space-2.2/README.rst
+-rw-r--r--   0        0        0        0 2023-05-05 05:24:18.834041 borg_space-2.2/borg_space/__init__.py
+-rw-r--r--   0        0        0     9536 2023-06-12 13:38:49.913154 borg_space-2.2/borg_space/config.py
+-rw-r--r--   0        0        0    10791 2023-06-13 03:12:03.557395 borg_space-2.2/borg_space/main.py
+-rw-r--r--   0        0        0     3089 2023-06-07 00:28:49.138158 borg_space-2.2/borg_space/trees.py
+-rw-r--r--   0        0        0     1183 2023-06-13 03:12:03.556395 borg_space-2.2/pyproject.toml
+-rw-r--r--   0        0        0    13015 1970-01-01 00:00:00.000000 borg_space-2.2/PKG-INFO
```

### Comparing `borg_space-2.1/LICENSE` & `borg_space-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `borg_space-2.1/README.rst` & `borg_space-2.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 .. image:: https://img.shields.io/pypi/v/borg-space.svg
     :target: https://pypi.python.org/pypi/borg-space
 
 .. image:: https://img.shields.io/pypi/pyversions/borg-space.svg
     :target: https://pypi.python.org/pypi/borg-space/
 
 :Author: Ken Kundert
-:Version: 2.1
-:Released: 2023-06-09
+:Version: 2.2
+:Released: 2023-06-12
 
 *Borg-Space* is an accessory for Emborg_.  It reports on the space consumed by 
 your *BorgBackup* repositories.  You can get this information using the
 ``emborg info`` command, but there are several reasons to prefer *Borg-Space*.
 
 #. *Borg-Space* is capable of reporting on many repositories at once.
 #. The *Emborg* *info* command gives a great deal of information,
```

### Comparing `borg_space-2.1/borg_space/config.py` & `borg_space-2.2/borg_space/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Process settings file
 
 # IMPORTS {{{1
 from appdirs import user_config_dir
 from inform import (
-    Error, conjoin, error, fatal, full_stop,
-    is_str, is_mapping, is_collection, plural, os_error, terminate
+    Error, conjoin, error, full_stop,
+    is_str, is_mapping, is_collection, plural, os_error, terminate_if_errors
 )
 from quantiphy import Quantity
 from shlib import to_path, Run, set_prefs
 from voluptuous import Schema, Invalid, MultipleInvalid
 import arrow
 import getpass
 import nestedtext as nt
@@ -33,14 +33,15 @@
 # GLOBALS {{{1
 set_prefs(use_inform=True)
 settings_file = to_path(user_config_dir('borg-space')) / 'settings.nt'
 voluptuous_error_msg_mappings = {
     "extra keys not allowed": ("unknown key", "key"),
     "expected a dictionary": ("expected key:value pair", "value"),
 }
+voluptuous_key_prefix = "key contains"
 hostname = socket.gethostname().split('.')[0]
     # version of the hostname (the hostname without any domain name)
 username = pwd.getpwuid(os.getuid()).pw_name
 
 
 # REPOSITORY {{{1
 # Repository class {{{2
@@ -163,29 +164,41 @@
     return to_snake_case(key.replace('_', ' '))
 
 # to_list() {{{2
 def to_list(args):
     if is_str(args):
         args = args.split()
     if is_mapping(args):
-        raise Invalid(f"{args}: expected list or string")
+        raise Invalid(f"expected a list or string")
     return args
 
 # a_name() {{{2
-def a_name(arg):
+def a_name(arg, is_key=False):
     # names are expected to be identifiers except that dashes are allowed
+    # also allow names starting with a digit
     if not arg:
         return arg
     if not is_str(arg):
-        raise Invalid("expected string")
-    cleaned = arg.replace('-', '0')
+        raise Invalid("expected a string")
+    cleaned = '_' + arg.replace('-', '_')
+        # add prefix to allow leading digits, replace '-' to allow dashes
     if not cleaned.isidentifier():
-        raise Invalid(f"{arg}: expected a name")
+        from string import ascii_letters as letters, digits
+        invalid = ''.join(sorted(set(cleaned) - set(letters + digits + '-_')))
+        desc = f"{plural(invalid):/an invalid character/invalid characters}"
+        if is_key:
+            raise Invalid(f"key contains {desc}: ‘{invalid}’")
+        else:
+            raise Invalid(f"value contains {desc}: ‘{invalid}’")
     return arg
 
+# key_as_name() {{{2
+def key_as_name(arg):
+    return a_name(arg, is_key=True)
+
 # a_spec() {{{2
 def a_spec(arg):
     if is_str(arg):
         return arg
     if is_mapping(arg):
         unknown_keys = arg.keys() - set(['config', 'host', 'user'])
         if unknown_keys:
@@ -211,15 +224,15 @@
         return [a_spec(arg)]
     if is_collection(arg):
         return [a_spec(r) for r in arg]
     raise Invalid("expected a repository specification")
 
 # validate_settings {{{2
 validate_settings = Schema({
-    'repositories': {a_name: to_specs},
+    'repositories': {key_as_name: to_specs},
     'default_repository': str,
     'report_style': str,
     'compact_format': str,
     'table_format': str,
     'table_header': str,
     'report_fields': to_list,
     'tree_report_fields': to_list,
@@ -241,41 +254,48 @@
     )
 
     settings = validate_settings(settings)
     specifications = settings.get('repositories', {})
 
     # convert from specifications to Repository objects
     repositories = {}
-    for name, specs in specifications.items():
-        if specs:
-            repositories[name] = []
-            alias = name if len(specs) <= 1 else None
-            for spec in specs:
-                if spec in repositories and spec != name:
-                    # this is a known (previously defined) repository
-                    repositories[name].extend(repositories[spec])
-                else:
-                    repositories[name].append(Repository(spec, alias))
-        else:
-            repositories[name] = [Repository(name)]
+    try:
+        for name, specs in specifications.items():
+            if specs:
+                repositories[name] = []
+                alias = name if len(specs) <= 1 else None
+                for spec in specs:
+                    if spec in repositories and spec != name:
+                        # this is a known (previously defined) repository
+                        repositories[name].extend(repositories[spec])
+                    else:
+                        repositories[name].append(Repository(spec, alias))
+            else:
+                repositories[name] = [Repository(name)]
+    except Invalid as e:
+        raise Error(e, culprit=name)
 
 except nt.NestedTextError as e:
-    e.terminate()
+    e.report()
+except Error as e:
+    e.report(culprit=(settings_file,) + e.culprit)
 except FileNotFoundError:
     settings = {}
     repositories = {}
 except OSError as e:
-    fatal(os_error(e), culprit=settings_file)
+    error(os_error(e))
 except MultipleInvalid as e:  # report schema violations
     for err in e.errors:
         msg, flag = voluptuous_error_msg_mappings.get(
             err.msg, (err.msg, 'value')
         )
+        if msg.startswith(voluptuous_key_prefix):
+            flag = 'key'
         loc = keymap.get(tuple(err.path))
         codicil = loc.as_line(flag) if loc else None
         keys = nt.join_keys(err.path, keymap=keymap)
         error(
             full_stop(msg),
             culprit = (settings_file, keys),
             codicil = codicil
         )
-    terminate()
+terminate_if_errors()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `borg_space-2.1/borg_space/main.py` & `borg_space-2.2/borg_space/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,30 +32,30 @@
 
 # imports {{{1
 from .config import settings, get_repos
 from .trees import tree
 import arrow
 from appdirs import user_data_dir
 from docopt import docopt
-from inform import Error, display, error, os_error, warn
+from inform import Error, display, error, os_error, terminate, warn
 from pathlib import Path
 from quantiphy import Quantity
 import json
 import nestedtext as nt
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.dates import AutoDateFormatter, AutoDateLocator
 from matplotlib.ticker import FuncFormatter
 
 # globals {{{1
 data_dir = Path(user_data_dir('borg-space'))
 now = str(arrow.now())
 Quantity.set_prefs(prec='full')
-__version__ = "2.1"
-__released__ = "2023-06-09"
+__version__ = "2.2"
+__released__ = "2023-06-12"
 date_format = settings.get('date_format', 'D MMMM YYYY')
 size_format = settings.get('size_format', '.2b')
 nestedtext_size_format = settings.get('nestedtext_size_format', size_format)
 size_fields = ['size',]  # must contain only one value
 date_fields = ['last_create', 'last_prune', 'last_compact', 'last_squeeze']
 all_fields = size_fields + date_fields
 report_fields = settings.get('report_fields', size_fields)
@@ -147,27 +147,29 @@
         ax.set_yscale('log')
 
     # configure the axis labeling {{{3
     locator = AutoDateLocator()
     ax.xaxis.set_major_locator(locator)
     ax.xaxis.set_major_formatter(AutoDateFormatter(locator))
 
+    fig.autofmt_xdate()
+
     # add traces in order of last size, largest to smallest {{{3
     largest = 0
     smallest = 1e100
     for entry in sorted(traces, key=lambda d: d[1], reverse=True):
         name, last_size, dates, sizes = entry
         largest = max(largest, *sizes)
         smallest = min(smallest, *sizes)
         trace, = ax.plot_date(dates, sizes, "-")
         trace.set_label(f'{name} ({last_size:{size_format}})')
 
     # use SI scale factors on Y-axis
     def bytes(value, pos=None):
-        return Quantity(value, 'B').render()
+        return Quantity(value, 'B').render(prec=3)
     ax.yaxis.set_major_formatter(FuncFormatter(bytes))
     if largest / smallest > 10:
         ax.yaxis.set_minor_formatter("")
     else:
         ax.yaxis.set_minor_formatter(FuncFormatter(bytes))
 
     # draw the graph {{{3
@@ -337,7 +339,8 @@
                 print_report(repos, cmdline['--style'])
     except (Error, nt.NestedTextError) as e:
         e.report()
     except OSError as e:
         error(os_error(e))
     except KeyboardInterrupt:
         pass
+    terminate()
```

### Comparing `borg_space-2.1/borg_space/trees.py` & `borg_space-2.2/borg_space/trees.py`

 * *Files identical despite different names*

### Comparing `borg_space-2.1/pyproject.toml` & `borg_space-2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "borg_space"
 dist-name = "borg-space"
-version = "2.1"
+version = "2.2"
 description = "Accessory for Emborg used to report and track the size of your Borg repositories"
 readme = "README.rst"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 keywords = ["emborg", "borg", "backups"]
 authors = [{name = "Ken Kundert", email = "emborg@nurdletech.com"}]
 classifiers = [
```

### Comparing `borg_space-2.1/PKG-INFO` & `borg_space-2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: borg_space
-Version: 2.1
+Version: 2.2
 Summary: Accessory for Emborg used to report and track the size of your Borg repositories
 Keywords: emborg,borg,backups
 Author-email: Ken Kundert <emborg@nurdletech.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
@@ -34,16 +34,16 @@
 .. image:: https://img.shields.io/pypi/v/borg-space.svg
     :target: https://pypi.python.org/pypi/borg-space
 
 .. image:: https://img.shields.io/pypi/pyversions/borg-space.svg
     :target: https://pypi.python.org/pypi/borg-space/
 
 :Author: Ken Kundert
-:Version: 2.1
-:Released: 2023-06-09
+:Version: 2.2
+:Released: 2023-06-12
 
 *Borg-Space* is an accessory for Emborg_.  It reports on the space consumed by 
 your *BorgBackup* repositories.  You can get this information using the
 ``emborg info`` command, but there are several reasons to prefer *Borg-Space*.
 
 #. *Borg-Space* is capable of reporting on many repositories at once.
 #. The *Emborg* *info* command gives a great deal of information,
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_nwo9xrog_/tmprrvknbu4_TarContainer/0/7", line 352, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_nwo9xrog_/tmprrvknbu4_TarContainer/0/7", line 352, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: borg_space Version: 2.1 Summary: Accessory for
+Metadata-Version: 2.1 Name: borg_space Version: 2.2 Summary: Accessory for
 Emborg used to report and track the size of your Borg repositories Keywords:
 emborg,borg,backups Author-email: Ken Kundert
 nurdletech.com> Requires-Python: >=3.6 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later
 (GPLv3+) Classifier: Natural Language :: English Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Utilities Requires-Dist: appdirs Requires-Dist: arrow Requires-Dist:
@@ -14,15 +14,15 @@
 kenkundert/borg-space Project-URL: repository, https://github.com/kenkundert/
 borg-space Borg-Space â Report and track the size of your Emborg repositories
 ================================================================== .. image::
 https://pepy.tech/badge/borg-space/month :target: https://pepy.tech/project/
 borg-space .. image:: https://img.shields.io/pypi/v/borg-space.svg :target:
 https://pypi.python.org/pypi/borg-space .. image:: https://img.shields.io/pypi/
 pyversions/borg-space.svg :target: https://pypi.python.org/pypi/borg-space/ :
-Author: Ken Kundert :Version: 2.1 :Released: 2023-06-09 *Borg-Space* is an
+Author: Ken Kundert :Version: 2.2 :Released: 2023-06-12 *Borg-Space* is an
 accessory for Emborg_. It reports on the space consumed by your *BorgBackup*
 repositories. You can get this information using the ``emborg info`` command,
 but there are several reasons to prefer *Borg-Space*. #. *Borg-Space* is
 capable of reporting on many repositories at once. #. The *Emborg* *info*
 command gives a great deal of information, whereas *Borg-Space* only reports
 the space consumed by the repository, so is much more compact. #. The report is
 user customizable. #. *Borg-Space* can record the size of your repositories
```

