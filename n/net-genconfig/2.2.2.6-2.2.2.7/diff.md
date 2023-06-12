# Comparing `tmp/net-genconfig-2.2.2.6.tar.gz` & `tmp/net-genconfig-2.2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/net-genconfig-2.2.2.6.tar", last modified: Thu Feb  4 18:03:56 2021, max compression
+gzip compressed data, was "net-genconfig-2.2.2.7.tar", last modified: Mon Jun 12 22:35:25 2023, max compression
```

## Comparing `net-genconfig-2.2.2.6.tar` & `net-genconfig-2.2.2.7.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 rcf        (501) staff       (20)        0 2021-02-04 18:03:56.186770 net-genconfig-2.2.2.6/
--rw-r--r--   0 rcf        (501) staff       (20)     1323 2021-02-04 18:03:56.186395 net-genconfig-2.2.2.6/PKG-INFO
--rw-r--r--   0 rcf        (501) staff       (20)      707 2020-03-31 09:34:13.000000 net-genconfig-2.2.2.6/README.md
-drwxr-xr-x   0 rcf        (501) staff       (20)        0 2021-02-04 18:03:56.182664 net-genconfig-2.2.2.6/net_genconfig/
--rw-r--r--   0 rcf        (501) staff       (20)       51 2021-02-04 18:02:33.000000 net-genconfig-2.2.2.6/net_genconfig/__init__.py
--rw-r--r--   0 rcf        (501) staff       (20)    16882 2021-01-19 17:40:38.000000 net-genconfig-2.2.2.6/net_genconfig/__main__.py
--rw-r--r--   0 rcf        (501) staff       (20)    10016 2021-02-04 18:01:55.000000 net-genconfig-2.2.2.6/net_genconfig/helpers.py
--rw-r--r--   0 rcf        (501) staff       (20)    14643 2020-03-31 09:34:13.000000 net-genconfig-2.2.2.6/net_genconfig/netaddr_filter.py
-drwxr-xr-x   0 rcf        (501) staff       (20)        0 2021-02-04 18:03:56.185813 net-genconfig-2.2.2.6/net_genconfig.egg-info/
--rw-r--r--   0 rcf        (501) staff       (20)     1323 2021-02-04 18:03:55.000000 net-genconfig-2.2.2.6/net_genconfig.egg-info/PKG-INFO
--rw-r--r--   0 rcf        (501) staff       (20)      311 2021-02-04 18:03:55.000000 net-genconfig-2.2.2.6/net_genconfig.egg-info/SOURCES.txt
--rw-r--r--   0 rcf        (501) staff       (20)        1 2021-02-04 18:03:55.000000 net-genconfig-2.2.2.6/net_genconfig.egg-info/dependency_links.txt
--rw-r--r--   0 rcf        (501) staff       (20)       54 2021-02-04 18:03:55.000000 net-genconfig-2.2.2.6/net_genconfig.egg-info/requires.txt
--rw-r--r--   0 rcf        (501) staff       (20)       14 2021-02-04 18:03:55.000000 net-genconfig-2.2.2.6/net_genconfig.egg-info/top_level.txt
--rw-r--r--   0 rcf        (501) staff       (20)       38 2021-02-04 18:03:56.186892 net-genconfig-2.2.2.6/setup.cfg
--rwxr-xr-x   0 rcf        (501) staff       (20)      859 2020-08-15 15:12:56.000000 net-genconfig-2.2.2.6/setup.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-06-12 22:35:25.407025 net-genconfig-2.2.2.7/
+-rw-r--r--   0 rcf34      (503) staff       (20)     1315 2022-07-28 15:54:04.000000 net-genconfig-2.2.2.7/.gitignore
+-rw-r--r--   0 rcf34      (503) staff       (20)     1074 2022-07-28 15:54:04.000000 net-genconfig-2.2.2.7/LICENSE
+-rw-r--r--   0 rcf34      (503) staff       (20)      175 2022-07-28 15:54:04.000000 net-genconfig-2.2.2.7/Makefile
+-rw-r--r--   0 rcf34      (503) staff       (20)     1153 2023-06-12 22:35:25.406884 net-genconfig-2.2.2.7/PKG-INFO
+-rw-r--r--   0 rcf34      (503) staff       (20)      707 2022-07-28 15:54:04.000000 net-genconfig-2.2.2.7/README.md
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-06-12 22:35:25.405516 net-genconfig-2.2.2.7/bin/
+-rwxr-xr-x   0 rcf34      (503) staff       (20)       42 2022-07-28 15:54:04.000000 net-genconfig-2.2.2.7/bin/net-genconfig
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-06-12 22:35:25.406083 net-genconfig-2.2.2.7/net_genconfig/
+-rw-r--r--   0 rcf34      (503) staff       (20)       51 2023-06-12 22:32:24.000000 net-genconfig-2.2.2.7/net_genconfig/__init__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    19239 2023-06-12 22:32:18.000000 net-genconfig-2.2.2.7/net_genconfig/__main__.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    10016 2022-07-28 15:54:04.000000 net-genconfig-2.2.2.7/net_genconfig/helpers.py
+-rw-r--r--   0 rcf34      (503) staff       (20)    14643 2022-07-28 15:54:04.000000 net-genconfig-2.2.2.7/net_genconfig/netaddr_filter.py
+drwxr-xr-x   0 rcf34      (503) staff       (20)        0 2023-06-12 22:35:25.406686 net-genconfig-2.2.2.7/net_genconfig.egg-info/
+-rw-r--r--   0 rcf34      (503) staff       (20)     1153 2023-06-12 22:35:25.000000 net-genconfig-2.2.2.7/net_genconfig.egg-info/PKG-INFO
+-rw-r--r--   0 rcf34      (503) staff       (20)      357 2023-06-12 22:35:25.000000 net-genconfig-2.2.2.7/net_genconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)        1 2023-06-12 22:35:25.000000 net-genconfig-2.2.2.7/net_genconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)       54 2023-06-12 22:35:25.000000 net-genconfig-2.2.2.7/net_genconfig.egg-info/requires.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)       14 2023-06-12 22:35:25.000000 net-genconfig-2.2.2.7/net_genconfig.egg-info/top_level.txt
+-rw-r--r--   0 rcf34      (503) staff       (20)       38 2023-06-12 22:35:25.407069 net-genconfig-2.2.2.7/setup.cfg
+-rwxr-xr-x   0 rcf34      (503) staff       (20)      859 2022-07-28 15:54:04.000000 net-genconfig-2.2.2.7/setup.py
```

### Comparing `net-genconfig-2.2.2.6/PKG-INFO` & `net-genconfig-2.2.2.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: net-genconfig
-Version: 2.2.2.6
+Version: 2.2.2.7
 Summary: Network device configuration generator
 Home-page: https://gitlab.developers.cam.ac.uk/uis/netsys/udn/net-genconfig
 Author: Robert Franklin
 Author-email: rcf34@cam.ac.uk
-License: UNKNOWN
-Description: net-genconfig
-        =============
-        
-        This package generates configurations for network devices based on three
-        sources of information:
-        
-        * roles -- these Jinja2 templates form the basis of an output
-          configuration file and exist for each platform and device role (e.g.
-          IOS as distribution router; IOS as core router, NX-OS as core router,
-          NX-OS as row switch)
-        
-        * include -- Jinja2 includes (some to be included 'as is' [.j2] and
-          some with macros that can be called [.j2m]); these are included by
-          the role templates and by each other
-        
-        * inventory -- this is a big database of device details (including the role for
-          a particular device) and associated information, such as VLANs, subnets,
-          interfaces, etc.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+net-genconfig
+=============
+
+This package generates configurations for network devices based on three
+sources of information:
+
+* roles -- these Jinja2 templates form the basis of an output
+  configuration file and exist for each platform and device role (e.g.
+  IOS as distribution router; IOS as core router, NX-OS as core router,
+  NX-OS as row switch)
+
+* include -- Jinja2 includes (some to be included 'as is' [.j2] and
+  some with macros that can be called [.j2m]); these are included by
+  the role templates and by each other
+
+* inventory -- this is a big database of device details (including the role for
+  a particular device) and associated information, such as VLANs, subnets,
+  interfaces, etc.
```

### Comparing `net-genconfig-2.2.2.6/README.md` & `net-genconfig-2.2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `net-genconfig-2.2.2.6/net_genconfig/__main__.py` & `net-genconfig-2.2.2.7/net_genconfig/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # net_genconfig.__main__
 
 
 
 import net_genconfig
 
 import argparse
-from copy import copy, deepcopy
-import datetime
+from copy import deepcopy
+from functools import reduce
 import jinja2
 import os
 import re
 import sys
 import yaml
 
-from deepops import deepmerge, deepremoveitems
+from deepops import deepget, deepmerge, deepremoveitems
 
 from net_genconfig import helpers, netaddr_filter
 
 from net_inventorylib import NetInventory
 
 
 
@@ -144,14 +144,45 @@
 
     # rendering succeeded
 
     return True
 
 
 
+def deepselect(d, *p):
+    """Return the specified portion of the nested structure d given by
+    the path p, as per deepops.deepget() but also prefix the path as a
+    leading path.
+
+    This has the effect of returning structure d with only the portion
+    given by p and nothing else and is useful for highlighting the path
+    into the structure.
+
+    If the path could not be found, None is returned, without the path
+    prefix, highlighting that it was not found (as opposed to being
+    empty).  This is useful in the context this is used.
+    """
+
+    # copy and reverse the path so we can use reduce() to fold right
+    r = list(p)
+    r.reverse()
+
+    # try to get the path into the structure, returning None if it was
+    # not found (not prefixing the path), to illustrate that the key
+    # could not be found
+    try:
+        d_sub = deepget(d, *p, default_error=True)
+    except KeyError:
+        return None
+
+    # build the path in with the final value as the deepget()
+    return reduce(lambda d, k: { k: d }, r, d_sub)
+
+
+
 def render_config(devicename, inventory, env, output_filename,
                   no_output=False, no_squash_blanklines=False,
                   comment_prefix=None, dump_device=False, debug=False, **vars):
 
     """Render the configuration for the specified device and write it
     to either standard output or a file, depending on the command line
     options specified.
@@ -295,97 +326,110 @@
     dest="inventory_dirname",
     default="inventory",
     help="directory containing inventory of devices, networks, etc.")
 
 parser.add_argument(
     "-o", "--output",
     dest="output_filename",
-    help="write configuration to named file instead of stdout; '%%' can be "
-             "used to substitute in the name of the device into the filename")
+    help="write configuration to named file instead of stdout; '%%' "
+         "can be used to substitute in the name of the device into the "
+         "filename")
 
 parser.add_argument(
     "-O", "--no-output",
     action="store_true",
-    help="generate the configuration but do not output it - useful to test "
-             "generation succeeds")
+    help="generate the configuration but do not output it - useful to "
+         "test generation succeeds")
 
 parser.add_argument(
-    "-S", "--no-squash-blanklines",
+    "-s", "--no-squash-blanklines",
     action="store_true",
     help="disable the squashing of leading and trailing, as well as "
-             "multiple, consecutive blank lines (prevent equivalent of '| "
-             "cat -s') in output")
+         "multiple, consecutive blank lines (prevent equivalent of '| "
+         "cat -s') in output")
 
 parser.add_argument(
     "-M", "--comment-prefix",
     default="##",
-    help="prefix for comments to strip from output (useful if the target "
-             "platform does not natively support comments but they are to be "
-             "used to provide a documented configuration; set to '-' to "
-             "disable stripping")
+    help="prefix for comments to strip from output (useful if the "
+         "target platform does not natively support comments but they "
+         "are to be used to provide a documented configuration; set to "
+         "'-' to disable stripping")
 
 parser.add_argument(
     "-E", "--list-env",
     action="store_true",
     help="list filter and global helper functions and stop (this will "
-             "include the standard Jinja2, as well as the netaddr module and "
-             "custom ones)")
+         "include the standard Jinja2, as well as the netaddr module "
+         "and custom ones)")
 
 parser.add_argument(
     "-I", "--dump-inventory",
     action="store_true",
-    help="dump complete read inventory in YAML to stdout and stop, without "
-             "generating any configurations")
+    help="dump complete read inventory in YAML to stdout and stop, "
+         "without generating any configurations")
 
 parser.add_argument(
     "-F", "--dump-filepaths",
     action="store_true",
-    help="dump paths of files which are the source of each entry in the "
-             "inventory")
+    help="dump paths of files which are the source of each entry in "
+         "the inventory")
 
 parser.add_argument(
     "-U", "--dump-device",
     action="store_true",
-    help="dump resulting device definition in YAML to stdout, after merging "
-             "profiles and stop, without generating any configurations")
+    help="dump resulting device definition in YAML to stdout, after "
+         "merging profiles and stop, without generating any "
+         "configurations")
+
+parser.add_argument(
+    "-S", "--subtree-dump-filter",
+    metavar="key",
+    nargs="*",
+    default=[],
+    help="limit dump options for the inventory and file paths to "
+         "subtree of configuration dictionary with a path specified as "
+         "list of keys; '-' can be used to represent None and values "
+         "that are parsable as integers will be converted to integers")
 
 parser.add_argument(
     "-d", "--define",
     action="append",
     nargs=2,
     default=[],
     help="define variable for use in the template",
     metavar=("VAR", "VALUE"))
 
 parser.add_argument(
     "-T", "--template",
     dest="template_filename",
-    help="read the inventory, set up the environment and then render the "
-             "specified template file (from the roles or include "
-             "directories) then stop - used to quickly test template "
-             "functions without needing to construct a device")
+    help="read the inventory, set up the environment and then render "
+         "the specified template file (from the roles or include "
+         "directories) then stop - used to quickly test template "
+         "functions without needing to construct a device")
 
 parser.add_argument(
     "-q", "--quiet",
     action="store_true",
     help="when generating configuration for multiple devices, don't "
-             "print the name of each device, as it's generated")
+         "print the name of each device, as it's generated")
 
 parser.add_argument(
     "-D", "--debug",
     action="store_true",
     help="enable debug mode")
 
 parser.add_argument(
     "-R", "--raise-exception",
     action="store_true",
-    help="when an exception is explicitly raised through a helper function, "
-            "raise the complete exception rather than catch it and just "
-            "print the message specific error message - this is useful if "
-            "the exception does not make it clear where it occurred")
+    help="when an exception is explicitly raised through a helper "
+         "function, raise the complete exception rather than catch it "
+         "and just print the message specific error message - this is "
+         "useful if the exception does not make it clear where it "
+         "occurred")
 
 parser.add_argument(
     "devicename",
     nargs="*",
     help="name(s) of the device(s) to generate the configuration for")
 
 parser.add_argument(
@@ -406,14 +450,15 @@
 no_output = args.no_output
 no_squash_blanklines = args.no_squash_blanklines
 comment_prefix = None if args.comment_prefix == "-" else args.comment_prefix
 list_env = args.list_env
 dump_inventory = args.dump_inventory
 dump_filepaths = args.dump_filepaths
 dump_device = args.dump_device
+subtree_dump_filter = args.subtree_dump_filter
 template_filename = args.template_filename
 quiet = args.quiet
 devicenames = args.devicename
 debug = args.debug
 raise_exception = args.raise_exception
 
 vars = {}
@@ -429,14 +474,43 @@
 debug: output filename: %s
 debug: device names: %s"""
               % (roles_dirname, include_dirname, inventory_dirname,
                  output_filename, devicenames),
           file=sys.stderr)
 
 
+# if a subtree was specified for debugging 'dump' options, handle some
+# special cases of the elements in the path:
+#
+# * a single dash ('-') is treated as None
+#
+# * if the element can be converted to an integer, do that, rather than
+#   treat it as a string
+#
+# these are to cope with limitations on the parsing available in the
+# ArgumentParser class compared with the flexibility and ambiguity of
+# the configuration dictionary
+
+if subtree_dump_filter:
+    def convert_path_item(s):
+        "Convert a single path element from a string into another type."
+
+        if s == "-":
+            return None
+
+        try:
+            return int(s)
+        except ValueError:
+            pass
+
+        return s
+
+    subtree_dump_filter = [ convert_path_item(s) for s in subtree_dump_filter]
+
+
 # check that the roles and include directories exist
 
 if not os.path.isdir(roles_dirname):
     print("error: roles directory does not exist: %s" % roles_dirname,
             file=sys.stderr)
 
     exit(1)
@@ -481,19 +555,22 @@
 
 # read in the inventory
 
 inventory = NetInventory(inventory_dirname, debug=debug)
 
 
 if dump_inventory:
-    print(yaml.dump(dict(inventory), default_flow_style=False))
+    print(yaml.dump(deepselect(dict(inventory), *subtree_dump_filter),
+          default_flow_style=False))
     exit(0)
 
 if dump_filepaths:
-    print(yaml.dump(inventory.get_filepaths(), default_flow_style=False))
+    print(yaml.dump(deepselect(inventory.get_filepaths(),
+                               *subtree_dump_filter),
+                    default_flow_style=False))
     exit(0)
 
 if "devices" not in inventory:
     print("error: no devices found in inventory", file=sys.stderr)
     exit(1)
 
 
@@ -509,15 +586,15 @@
 if debug:
     print("debug: creating environment with filesystem loader directories: "
           "%s" % jinja_fsloader_dirs)
 
 env = jinja2.Environment(
     loader=jinja2.FileSystemLoader(jinja_fsloader_dirs),
     extensions=[
-        "jinja2.ext.do", "jinja2.ext.loopcontrols", "jinja2.ext.with_"],
+        "jinja2.ext.do", "jinja2.ext.loopcontrols"],
     trim_blocks=True)
 
 
 # add in the special warn(), raise() and assert() functions, as well as
 # some other functions we need, into the Jinja2 environment
 
 for helpers_dict in [deep_helpers, helpers.helpers]:
```

### Comparing `net-genconfig-2.2.2.6/net_genconfig/helpers.py` & `net-genconfig-2.2.2.7/net_genconfig/helpers.py`

 * *Files identical despite different names*

### Comparing `net-genconfig-2.2.2.6/net_genconfig/netaddr_filter.py` & `net-genconfig-2.2.2.7/net_genconfig/netaddr_filter.py`

 * *Files identical despite different names*

### Comparing `net-genconfig-2.2.2.6/net_genconfig.egg-info/PKG-INFO` & `net-genconfig-2.2.2.7/net_genconfig.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: net-genconfig
-Version: 2.2.2.6
+Version: 2.2.2.7
 Summary: Network device configuration generator
 Home-page: https://gitlab.developers.cam.ac.uk/uis/netsys/udn/net-genconfig
 Author: Robert Franklin
 Author-email: rcf34@cam.ac.uk
-License: UNKNOWN
-Description: net-genconfig
-        =============
-        
-        This package generates configurations for network devices based on three
-        sources of information:
-        
-        * roles -- these Jinja2 templates form the basis of an output
-          configuration file and exist for each platform and device role (e.g.
-          IOS as distribution router; IOS as core router, NX-OS as core router,
-          NX-OS as row switch)
-        
-        * include -- Jinja2 includes (some to be included 'as is' [.j2] and
-          some with macros that can be called [.j2m]); these are included by
-          the role templates and by each other
-        
-        * inventory -- this is a big database of device details (including the role for
-          a particular device) and associated information, such as VLANs, subnets,
-          interfaces, etc.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+net-genconfig
+=============
+
+This package generates configurations for network devices based on three
+sources of information:
+
+* roles -- these Jinja2 templates form the basis of an output
+  configuration file and exist for each platform and device role (e.g.
+  IOS as distribution router; IOS as core router, NX-OS as core router,
+  NX-OS as row switch)
+
+* include -- Jinja2 includes (some to be included 'as is' [.j2] and
+  some with macros that can be called [.j2m]); these are included by
+  the role templates and by each other
+
+* inventory -- this is a big database of device details (including the role for
+  a particular device) and associated information, such as VLANs, subnets,
+  interfaces, etc.
```

### Comparing `net-genconfig-2.2.2.6/setup.py` & `net-genconfig-2.2.2.7/setup.py`

 * *Files identical despite different names*

