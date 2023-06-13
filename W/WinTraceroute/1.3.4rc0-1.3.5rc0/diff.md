# Comparing `tmp/WinTraceroute-1.3.4rc0.tar.gz` & `tmp/WinTraceroute-1.3.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WinTraceroute-1.3.4rc0.tar", last modified: Fri May 19 16:35:47 2023, max compression
+gzip compressed data, was "WinTraceroute-1.3.5rc0.tar", last modified: Tue Jun 13 19:02:19 2023, max compression
```

## Comparing `WinTraceroute-1.3.4rc0.tar` & `WinTraceroute-1.3.5rc0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:35:47.803038 WinTraceroute-1.3.4rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-19 16:35:21.000000 WinTraceroute-1.3.4rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-05-19 16:35:47.803038 WinTraceroute-1.3.4rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-19 16:35:21.000000 WinTraceroute-1.3.4rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:35:47.803038 WinTraceroute-1.3.4rc0/WinTraceroute.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-05-19 16:35:47.000000 WinTraceroute-1.3.4rc0/WinTraceroute.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-19 16:35:47.000000 WinTraceroute-1.3.4rc0/WinTraceroute.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:35:47.000000 WinTraceroute-1.3.4rc0/WinTraceroute.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-19 16:35:47.000000 WinTraceroute-1.3.4rc0/WinTraceroute.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 16:35:47.000000 WinTraceroute-1.3.4rc0/WinTraceroute.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 16:35:47.000000 WinTraceroute-1.3.4rc0/WinTraceroute.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-19 16:35:21.000000 WinTraceroute-1.3.4rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:35:47.803038 WinTraceroute-1.3.4rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:35:47.803038 WinTraceroute-1.3.4rc0/traceroute/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:35:21.000000 WinTraceroute-1.3.4rc0/traceroute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-19 16:35:21.000000 WinTraceroute-1.3.4rc0/traceroute/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100486 2023-05-19 16:35:21.000000 WinTraceroute-1.3.4rc0/traceroute/lorem.py
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-05-19 16:35:21.000000 WinTraceroute-1.3.4rc0/traceroute/traceroute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:02:19.770067 WinTraceroute-1.3.5rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-13 19:01:47.000000 WinTraceroute-1.3.5rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-06-13 19:02:19.770067 WinTraceroute-1.3.5rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-13 19:01:47.000000 WinTraceroute-1.3.5rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:02:19.770067 WinTraceroute-1.3.5rc0/WinTraceroute.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-06-13 19:02:19.000000 WinTraceroute-1.3.5rc0/WinTraceroute.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 19:02:19.000000 WinTraceroute-1.3.5rc0/WinTraceroute.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:02:19.000000 WinTraceroute-1.3.5rc0/WinTraceroute.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 19:02:19.000000 WinTraceroute-1.3.5rc0/WinTraceroute.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 19:02:19.000000 WinTraceroute-1.3.5rc0/WinTraceroute.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 19:02:19.000000 WinTraceroute-1.3.5rc0/WinTraceroute.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-13 19:01:47.000000 WinTraceroute-1.3.5rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 19:02:19.770067 WinTraceroute-1.3.5rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:02:19.770067 WinTraceroute-1.3.5rc0/traceroute/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:01:47.000000 WinTraceroute-1.3.5rc0/traceroute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-13 19:01:47.000000 WinTraceroute-1.3.5rc0/traceroute/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100486 2023-06-13 19:01:47.000000 WinTraceroute-1.3.5rc0/traceroute/lorem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-06-13 19:01:47.000000 WinTraceroute-1.3.5rc0/traceroute/traceroute.py
```

### Comparing `WinTraceroute-1.3.4rc0/LICENSE` & `WinTraceroute-1.3.5rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `WinTraceroute-1.3.4rc0/PKG-INFO` & `WinTraceroute-1.3.5rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinTraceroute
-Version: 1.3.4rc0
+Version: 1.3.5rc0
 Summary: A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `WinTraceroute-1.3.4rc0/README.md` & `WinTraceroute-1.3.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `WinTraceroute-1.3.4rc0/WinTraceroute.egg-info/PKG-INFO` & `WinTraceroute-1.3.5rc0/WinTraceroute.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinTraceroute
-Version: 1.3.4rc0
+Version: 1.3.5rc0
 Summary: A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy.
 Author-email: Nico Rittinghaus <nico@ritti.ng>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `WinTraceroute-1.3.4rc0/pyproject.toml` & `WinTraceroute-1.3.5rc0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "bumpver", "scapy==2.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WinTraceroute"
-version = "1.3.4-rc"
+version = "1.3.5-rc"
 description = "A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy."
 authors = [{ name = "Nico Rittinghaus", email = "nico@ritti.ng" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta"
@@ -24,15 +24,15 @@
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "pyinstaller==5.10.1"]
 
 [project.urls]
 Homepage = "https://github.com/NiRit100/WinTraceroute"
 
 [tool.bumpver]
-current_version = "1.3.4-rc"
+current_version = "1.3.5-rc"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 # (BETA) tells setuptools you will be using a readme file for the long description field for your pypi profile.
```

### Comparing `WinTraceroute-1.3.4rc0/traceroute/__main__.py` & `WinTraceroute-1.3.5rc0/traceroute/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from signal import signal, SIGINT
 from sys import exit, \
                 version_info as py_version_info
+from os import environ
 import argparse
 from traceroute.traceroute import trace_udp, trace_icmp
 
 
 def main() -> int:
     import logging
     logging.getLogger("scapy").setLevel(logging.WARNING)
 
+    # parse args
     epilog = """See also RFC2151 section 3.4 for a quick
                 read-up on traceroute."""
     parser = argparse.ArgumentParser(
                     prog='traceroute',
                     description="""Provides a mostly *NIX-traceroute-
                     like -- but very basic -- tracert/traceroute IPv4
                     alternative built on scapy.""",
@@ -73,30 +75,18 @@
                         const=True, default=False, \
         help="""do *not* vary the IP segment 
                 'Identification' field.""")
     parser.add_argument('--no-legacy-python-notice', \
                         dest='show_legacy_py_notice', \
                         action='store_const', \
                         const=False, default=True, \
-        help="""disables the legacy python version notice.""")
+        help="""Obsolete -- stays for compatibility.""")
     args = parser.parse_args()
     
     # TODO: make id vary by default and add switch to turn it off
-    
-    if args.show_legacy_py_notice and py_version_info <= (3, 9):
-        print()
-        print()
-        print("NOTE: This software runs best under Python 3.9 and later.")
-        print("      It is currently running on Python " + \
-            str(py_version_info.major) + "." + str(py_version_info.minor) + ".")
-        print("      The program can still be executed, but it might show some" \
-            "\n      strange behaviour.")
-        input("  Press ENTER to continue.")
-        print("--- CONTINUING")
-        print()
 
     try:
         # this once was a match statement, but not any more 
         # since the language downgrade
         if args.module == 'UDP':
             print()
             trace_udp(args.remote_host,
@@ -126,19 +116,18 @@
         print("Error: Please run this program with higher privileges.")
         exit(1)
 
 def term_handler(signal_received, frame) -> None:
     print()
     print("-- Cancelled by signal " + str(signal_received) + ".")
     exit(-1)
-
-try:
-    # this sometimes makes problems on windows
+    
+def bind_term_sig():
     signal(SIGINT, term_handler)
     #signal(SIGKILL, term_handler)
     #signal(SIGABRT, term_handler)
     #signal(SIGTERM, term_handler)
-except ImportError:
-    pass
+
 
 if __name__ == '__main__':
+    bind_term_sig()
     main()
```

### Comparing `WinTraceroute-1.3.4rc0/traceroute/lorem.py` & `WinTraceroute-1.3.5rc0/traceroute/lorem.py`

 * *Files identical despite different names*

### Comparing `WinTraceroute-1.3.4rc0/traceroute/traceroute.py` & `WinTraceroute-1.3.5rc0/traceroute/traceroute.py`

 * *Files identical despite different names*

