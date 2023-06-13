# Comparing `tmp/consolidatewheels-0.3.tar.gz` & `tmp/consolidatewheels-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consolidatewheels-0.3.tar", last modified: Thu Apr  6 16:31:18 2023, max compression
+gzip compressed data, was "consolidatewheels-0.4.tar", last modified: Tue Jun 13 16:28:57 2023, max compression
```

## Comparing `consolidatewheels-0.3.tar` & `consolidatewheels-0.4.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:31:18.551715 consolidatewheels-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-06 16:31:11.000000 consolidatewheels-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-06 16:31:18.551715 consolidatewheels-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-06 16:31:11.000000 consolidatewheels-0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:31:18.547715 consolidatewheels-0.3/consolidatewheels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 16:31:11.000000 consolidatewheels-0.3/consolidatewheels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-06 16:31:11.000000 consolidatewheels-0.3/consolidatewheels/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-06 16:31:11.000000 consolidatewheels-0.3/consolidatewheels/consolidate_linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-04-06 16:31:11.000000 consolidatewheels-0.3/consolidatewheels/consolidate_osx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-06 16:31:11.000000 consolidatewheels-0.3/consolidatewheels/dedupe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-06 16:31:11.000000 consolidatewheels-0.3/consolidatewheels/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-06 16:31:11.000000 consolidatewheels-0.3/consolidatewheels/wheelsfunc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:31:18.547715 consolidatewheels-0.3/consolidatewheels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-06 16:31:18.000000 consolidatewheels-0.3/consolidatewheels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-06 16:31:18.000000 consolidatewheels-0.3/consolidatewheels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 16:31:18.000000 consolidatewheels-0.3/consolidatewheels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-06 16:31:18.000000 consolidatewheels-0.3/consolidatewheels.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-06 16:31:18.000000 consolidatewheels-0.3/consolidatewheels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-06 16:31:18.000000 consolidatewheels-0.3/consolidatewheels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-06 16:31:11.000000 consolidatewheels-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 16:31:18.551715 consolidatewheels-0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:31:18.547715 consolidatewheels-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-06 16:31:11.000000 consolidatewheels-0.3/tests/test_consolidate_linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-06 16:31:11.000000 consolidatewheels-0.3/tests/test_consolidate_osx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-06 16:31:11.000000 consolidatewheels-0.3/tests/test_dedupe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-06 16:31:11.000000 consolidatewheels-0.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-06 16:31:11.000000 consolidatewheels-0.3/tests/test_wheels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:28:57.839453 consolidatewheels-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 16:28:49.000000 consolidatewheels-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-13 16:28:57.839453 consolidatewheels-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-06-13 16:28:49.000000 consolidatewheels-0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:28:57.835453 consolidatewheels-0.4/consolidatewheels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:28:49.000000 consolidatewheels-0.4/consolidatewheels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-13 16:28:49.000000 consolidatewheels-0.4/consolidatewheels/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-13 16:28:49.000000 consolidatewheels-0.4/consolidatewheels/consolidate_linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-13 16:28:49.000000 consolidatewheels-0.4/consolidatewheels/consolidate_osx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-13 16:28:49.000000 consolidatewheels-0.4/consolidatewheels/consolidate_win.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-13 16:28:49.000000 consolidatewheels-0.4/consolidatewheels/dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-13 16:28:49.000000 consolidatewheels-0.4/consolidatewheels/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-13 16:28:49.000000 consolidatewheels-0.4/consolidatewheels/wheelsfunc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:28:57.839453 consolidatewheels-0.4/consolidatewheels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-13 16:28:57.000000 consolidatewheels-0.4/consolidatewheels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-13 16:28:57.000000 consolidatewheels-0.4/consolidatewheels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:28:57.000000 consolidatewheels-0.4/consolidatewheels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 16:28:57.000000 consolidatewheels-0.4/consolidatewheels.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 16:28:57.000000 consolidatewheels-0.4/consolidatewheels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 16:28:57.000000 consolidatewheels-0.4/consolidatewheels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-13 16:28:49.000000 consolidatewheels-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:28:57.839453 consolidatewheels-0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:28:57.839453 consolidatewheels-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-13 16:28:49.000000 consolidatewheels-0.4/tests/test_consolidate_linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-13 16:28:49.000000 consolidatewheels-0.4/tests/test_consolidate_osx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-13 16:28:49.000000 consolidatewheels-0.4/tests/test_consolidate_win.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-13 16:28:49.000000 consolidatewheels-0.4/tests/test_dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-13 16:28:49.000000 consolidatewheels-0.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-13 16:28:49.000000 consolidatewheels-0.4/tests/test_wheels.py
```

### Comparing `consolidatewheels-0.3/LICENSE` & `consolidatewheels-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `consolidatewheels-0.3/PKG-INFO` & `consolidatewheels-0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consolidatewheels
-Version: 0.3
+Version: 0.4
 Summary: Consolidates the shared object dependencies across multiple wheels
 Author-email: Alessandro Molina <amol@turbogears.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: testing
@@ -24,14 +24,21 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/consolidatewheels.svg
     :target: https://pypi.python.org/pypi/consolidatewheels
 
 .. image:: https://img.shields.io/pypi/l/consolidatewheels.svg
     :target: https://pypi.python.org/pypi/consolidatewheels
 
+Supported Platforms
+-------------------
+
+* Linux
+* OSX
+* Windows
+
 Introduction
 ------------
 
 When multiple wheels depend on each other and share some ``.so`` files,
 it is possible to rely on ``auditwheel --exclude`` to make sure the ``.so``
 is included in only one of the wheels to avoid duplicating the file in every package.
 
@@ -88,21 +95,35 @@
 
     $ ldd venv/lib/python3.10/site-packages/libtwo/_libtwo.cpython-310-aarch64-linux-gnu.so
 	libfoo-ef63151d.so => not found
 
 which would work correctly as far as ``libone`` is imported _before_ ``libtwo`` as they will
 both look for ``libfoo-ef63151d.so`` which was loaded already by ``libone``.
 
+Linux Support
+~~~~~~~~~~~~~
+
+``consolidatewheels`` works also in conjunction with ``auditwheel``, consolidating all libraries
+embedded by ``auditwheel``. But on Linux duplicates won't be removed automatically, so
+you need to make sure to use ``auditwheel --exclude`` to ensure libraries are not embedded twice.
+
 OSX Support
 ~~~~~~~~~~~
 
 ``consolidatewheels`` works also in conjunction with ``delocate``, consolidating all libraries
 embedded by ``delocate`` and removing duplicates of the embedded libraries when they are provided
 in multiple wheels.
 
+Windows Support
+~~~~~~~~~~~~~~~
+
+``consolidatewheels`` works also in conjunction with ``delvewheel``, consolidating all libraries
+embedded by ``delvewheel`` and removing duplicates of the embedded libraries when they are provided
+in multiple wheels.
+
 Install
 -------
 
 Install with::
 
     $ pip install consolidatewheels
```

### Comparing `consolidatewheels-0.3/README.rst` & `consolidatewheels-0.4/consolidatewheels.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: consolidatewheels
+Version: 0.4
+Summary: Consolidates the shared object dependencies across multiple wheels
+Author-email: Alessandro Molina <amol@turbogears.org>
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: testing
+License-File: LICENSE
+
 consolidatewheels
 =================
 
 .. image:: https://github.com/amol-/consolidatewheels/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/amol-/consolidatewheels/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/amol-/consolidatewheels/badge.svg
@@ -12,14 +24,21 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/consolidatewheels.svg
     :target: https://pypi.python.org/pypi/consolidatewheels
 
 .. image:: https://img.shields.io/pypi/l/consolidatewheels.svg
     :target: https://pypi.python.org/pypi/consolidatewheels
 
+Supported Platforms
+-------------------
+
+* Linux
+* OSX
+* Windows
+
 Introduction
 ------------
 
 When multiple wheels depend on each other and share some ``.so`` files,
 it is possible to rely on ``auditwheel --exclude`` to make sure the ``.so``
 is included in only one of the wheels to avoid duplicating the file in every package.
 
@@ -76,21 +95,35 @@
 
     $ ldd venv/lib/python3.10/site-packages/libtwo/_libtwo.cpython-310-aarch64-linux-gnu.so
 	libfoo-ef63151d.so => not found
 
 which would work correctly as far as ``libone`` is imported _before_ ``libtwo`` as they will
 both look for ``libfoo-ef63151d.so`` which was loaded already by ``libone``.
 
+Linux Support
+~~~~~~~~~~~~~
+
+``consolidatewheels`` works also in conjunction with ``auditwheel``, consolidating all libraries
+embedded by ``auditwheel``. But on Linux duplicates won't be removed automatically, so
+you need to make sure to use ``auditwheel --exclude`` to ensure libraries are not embedded twice.
+
 OSX Support
 ~~~~~~~~~~~
 
 ``consolidatewheels`` works also in conjunction with ``delocate``, consolidating all libraries
 embedded by ``delocate`` and removing duplicates of the embedded libraries when they are provided
 in multiple wheels.
 
+Windows Support
+~~~~~~~~~~~~~~~
+
+``consolidatewheels`` works also in conjunction with ``delvewheel``, consolidating all libraries
+embedded by ``delvewheel`` and removing duplicates of the embedded libraries when they are provided
+in multiple wheels.
+
 Install
 -------
 
 Install with::
 
     $ pip install consolidatewheels
```

### Comparing `consolidatewheels-0.3/consolidatewheels/consolidate_linux.py` & `consolidatewheels-0.4/consolidatewheels/consolidate_linux.py`

 * *Files identical despite different names*

### Comparing `consolidatewheels-0.3/consolidatewheels/consolidate_osx.py` & `consolidatewheels-0.4/consolidatewheels/consolidate_osx.py`

 * *Files identical despite different names*

### Comparing `consolidatewheels-0.3/consolidatewheels/dedupe.py` & `consolidatewheels-0.4/consolidatewheels/dedupe.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 
 import pkg_resources
 import pkginfo
 
 from . import wheelsfunc
 
 
-def dedupe(wheels: list[str], destdir: str) -> list[str]:
+def dedupe(wheels: list[str], destdir: str, mangled: bool = False) -> list[str]:
     """Given a list of wheels remove duplicated libraries
 
     This searches .dylibs embedded by delocate for libraries
     that have been included multiple times across the wheels
     and will preserve only one of the copies.
     """
     wheels = [os.path.abspath(w) for w in wheels]
     distributions, dependency_tree = build_dependencies_tree(wheels)
     sorted_distributions = sort_dependencies(dependency_tree)
     wheels = [distributions[distname] for distname in sorted_distributions]
     print(wheels)
     with tempfile.TemporaryDirectory() as tmpcd:
         print(f"Dedupe, Working inside {tmpcd}")
         wheeldirs = wheelsfunc.unpackwheels(wheels, workdir=tmpcd)
-        delete_duplicate_libs(wheeldirs)
+        delete_duplicate_libs(wheeldirs, mangled)
         wheels = wheelsfunc.packwheels(wheeldirs, destdir)
     return wheels
 
 
 def build_dependencies_tree(
     wheels: list[str],
 ) -> tuple[dict[str, str], dict[str, list[str]]]:
@@ -92,34 +92,53 @@
                 # we can now insert this node
                 result.append(dname)
                 deptree.pop(dname)
                 continue
     return result
 
 
-def delete_duplicate_libs(wheeldirs: list[str]) -> None:
+def delete_duplicate_libs(wheeldirs: list[str], mangled: bool) -> None:
     """Given directories of unpacked wheels, preserve one copy of embedded libs.
 
     Deletes embedded libraries if they are provided by multiple wheels,
     only the first encountered lib is preserved.
 
-    This only works if embedded libraries are not marshalled or
-    they are marshalled with consistent naming.
+    mangled=True tries to make this work for mangled lib names.
+    This takes for granted that libraries have been mangled with
+    libname-HASH.ext, which is what auditwheel and dwelvewheel
+    currently do.
 
     Right now delocate on OSX doesn't apply any marshaling to file names,
     and thus this works correctly. Auditwheel currently seems to work
     because it retains the same marshaling hash across libraries,
     but usage of ``--exclude`` should be preferred over deduping the libs.
     """
     already_seen = set()
 
     for wheeldir in wheeldirs:
         print("Processing", wheeldir)
         for lib in itertools.chain(
             pathlib.Path(wheeldir).rglob(".dylibs/*"),
             pathlib.Path(wheeldir).rglob("*.libs/*.so"),
+            pathlib.Path(wheeldir).rglob("*.dll"),
         ):
-            libname = lib.name
+            if mangled:
+                libname = lib.name.split("-", 1)[0]
+            else:
+                libname = lib.name
             if libname in already_seen:
-                print(f"Removing {libname} as already provided by another wheel.")
+                print(
+                    f"Removing {lib.name} in {wheeldir} "
+                    "as already provided by another wheel."
+                )
                 lib.unlink()
+
+                # On Windows we also have to remove the entry from
+                # load-order generated by delvewheel
+                for load_order in pathlib.Path(lib.parent).rglob(".load-order-*"):
+                    with load_order.open() as load_order_f:
+                        embedded_libs = load_order_f.readlines()
+                    with load_order.open("w") as load_order_f:
+                        for embedded_lib in embedded_libs:
+                            if embedded_lib.strip() != lib.name:
+                                load_order_f.write(embedded_lib)
             already_seen.add(libname)
```

### Comparing `consolidatewheels-0.3/consolidatewheels/main.py` & `consolidatewheels-0.4/consolidatewheels/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 from __future__ import annotations
 
 import argparse
 import os
+import platform
 import shutil
 import subprocess
-import sys
 import tempfile
 
-from . import consolidate_linux, consolidate_osx, dedupe
+from . import consolidate_linux, consolidate_osx, consolidate_win, dedupe
 
 
 def main() -> int:
     """Main entry point of the command line tool.
 
     Executes consolidatewheels and returns the exit code.
     """
+    detected_system = platform.system().lower()
+
     if not requirements_satisfied():
         return 1
 
     opts = parse_options()
-    if sys.platform == "linux":
+    if detected_system == "linux":
         consolidate_linux.consolidate(opts.wheels, opts.dest)
-    elif sys.platform == "darwin":
+    elif detected_system == "windows":
+        # On Windows, we need to include all libraries
+        # so that they get mangled and reserve the right
+        # size in the IMPORTS section of the DLL to account for
+        # the mangling hash. That way we can then replace the hash
+        # without risk of overflowing.
+        # dedupe will take care that they don't appear twice.
+        with tempfile.TemporaryDirectory() as dedupedir:
+            wheels = dedupe.dedupe(opts.wheels, dedupedir, mangled=True)
+            consolidate_win.consolidate(wheels, opts.dest)
+    elif detected_system == "darwin":
         # On Mac, delocate does not mangle library names,
         # but there is no --exclude option,
         # so we just have to remove the extra lib.
         with tempfile.TemporaryDirectory() as dedupedir:
             wheels = dedupe.dedupe(opts.wheels, dedupedir)
             consolidate_osx.consolidate(wheels, opts.dest)
     return 0
@@ -66,32 +78,38 @@
     """Verifies that all system requirements are satisfied.
 
     Those can't be esily verified during install process,
     so it's easier to just check them when the tool starts.
 
     Returns ``False`` is the requirements are not satisfied.
     """
-    if sys.platform == "darwin":
+    detected_system = platform.system().lower()
+
+    if detected_system == "darwin":
         if not shutil.which("install_name_tool"):
             print("Cannot find required utility `install_name_tool` in PATH")
             return False
 
         if not shutil.which("codesign"):
             print("Cannot find required utility `codesign` in PATH")
             return False
-    elif sys.platform == "linux":
+    elif detected_system == "linux":
         # Ensure that patchelf exists and we can use it.
         if not shutil.which("patchelf"):
             print("Cannot find required utility `patchelf` in PATH")
             return False
 
         try:
             subprocess.check_output(["patchelf", "--version"]).decode("utf-8")
         except subprocess.CalledProcessError:
             print("Could not call `patchelf` binary")
             return False
+    elif detected_system == "windows":
+        # At the moment there are no system dependencies required.
+        pass
     else:
-        print("Error: This tool only supports Linux and MacOSX")
+        print("Error: This tool only supports Linux, MacOSX and Windows")
+        print("Detected System:", detected_system)
         return False
 
     # All requirements are in place, that's good!
     return True
```

### Comparing `consolidatewheels-0.3/consolidatewheels/wheelsfunc.py` & `consolidatewheels-0.4/consolidatewheels/wheelsfunc.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,10 +39,15 @@
     resulting_wheels = []
     for wheeldir in wheeldirs:
         if subprocess.call(["wheel", "pack", wheeldir, "--dest-dir", tmpdir]):
             raise RuntimeError(f"Unable to pack {wheeldir} into {tmpdir}")
 
         # This is a bit of an hack to preserve order of directories
         wheel = os.listdir(tmpdir)[0]
+        expected_dest_file = os.path.join(destdir, wheel)
+        if os.path.exists(expected_dest_file):
+            # This is required by windows as it is unable to
+            # overwrite the existing file.
+            os.unlink(expected_dest_file)
         shutil.move(os.path.join(tmpdir, wheel), destdir)
         resulting_wheels.append(os.path.join(destdir, wheel))
     return resulting_wheels
```

### Comparing `consolidatewheels-0.3/consolidatewheels.egg-info/PKG-INFO` & `consolidatewheels-0.4/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: consolidatewheels
-Version: 0.3
-Summary: Consolidates the shared object dependencies across multiple wheels
-Author-email: Alessandro Molina <amol@turbogears.org>
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: testing
-License-File: LICENSE
-
 consolidatewheels
 =================
 
 .. image:: https://github.com/amol-/consolidatewheels/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/amol-/consolidatewheels/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/amol-/consolidatewheels/badge.svg
@@ -24,14 +12,21 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/consolidatewheels.svg
     :target: https://pypi.python.org/pypi/consolidatewheels
 
 .. image:: https://img.shields.io/pypi/l/consolidatewheels.svg
     :target: https://pypi.python.org/pypi/consolidatewheels
 
+Supported Platforms
+-------------------
+
+* Linux
+* OSX
+* Windows
+
 Introduction
 ------------
 
 When multiple wheels depend on each other and share some ``.so`` files,
 it is possible to rely on ``auditwheel --exclude`` to make sure the ``.so``
 is included in only one of the wheels to avoid duplicating the file in every package.
 
@@ -88,21 +83,35 @@
 
     $ ldd venv/lib/python3.10/site-packages/libtwo/_libtwo.cpython-310-aarch64-linux-gnu.so
 	libfoo-ef63151d.so => not found
 
 which would work correctly as far as ``libone`` is imported _before_ ``libtwo`` as they will
 both look for ``libfoo-ef63151d.so`` which was loaded already by ``libone``.
 
+Linux Support
+~~~~~~~~~~~~~
+
+``consolidatewheels`` works also in conjunction with ``auditwheel``, consolidating all libraries
+embedded by ``auditwheel``. But on Linux duplicates won't be removed automatically, so
+you need to make sure to use ``auditwheel --exclude`` to ensure libraries are not embedded twice.
+
 OSX Support
 ~~~~~~~~~~~
 
 ``consolidatewheels`` works also in conjunction with ``delocate``, consolidating all libraries
 embedded by ``delocate`` and removing duplicates of the embedded libraries when they are provided
 in multiple wheels.
 
+Windows Support
+~~~~~~~~~~~~~~~
+
+``consolidatewheels`` works also in conjunction with ``delvewheel``, consolidating all libraries
+embedded by ``delvewheel`` and removing duplicates of the embedded libraries when they are provided
+in multiple wheels.
+
 Install
 -------
 
 Install with::
 
     $ pip install consolidatewheels
```

### Comparing `consolidatewheels-0.3/pyproject.toml` & `consolidatewheels-0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools>=45"]
 
 [project]
 name = "consolidatewheels"
-version = "0.3"
+version = "0.4"
 authors = [
     {name = "Alessandro Molina", email = "amol@turbogears.org"},
 ]
 license = {text = "MIT"}
 description = "Consolidates the shared object dependencies across multiple wheels"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "wheel",
-    "pkginfo"
+    "pkginfo",
+    "pefile"
 ]
 
 [project.optional-dependencies]
 testing = [
     "pytest >= 3.4",
     "pytest-cov"
 ]
```

### Comparing `consolidatewheels-0.3/tests/test_consolidate_linux.py` & `consolidatewheels-0.4/tests/test_consolidate_linux.py`

 * *Files identical despite different names*

### Comparing `consolidatewheels-0.3/tests/test_consolidate_osx.py` & `consolidatewheels-0.4/tests/test_consolidate_osx.py`

 * *Files identical despite different names*

### Comparing `consolidatewheels-0.3/tests/test_dedupe.py` & `consolidatewheels-0.4/tests/test_dedupe.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,17 +17,19 @@
         "files",
         "libfirst-0.0.0-cp310-cp310-manylinux1_x86_64.manylinux_2_5_x86_64.whl",
     ),
 }
 
 
 def test_dedupe(tmpdir):
-    # Integration test that actually does the dedupe workflow.
+    # Integration test that actually does the dedupe workflow on OSX.
     results = dedupe.dedupe(
-        [FIXTURE_FILES["libfirst.whl"], FIXTURE_FILES["libtwo.whl"]], destdir=tmpdir
+        [FIXTURE_FILES["libfirst.whl"], FIXTURE_FILES["libtwo.whl"]],
+        destdir=tmpdir,
+        mangled=False,
     )
     assert len(results) == 2
 
     os.makedirs(os.path.join(tmpdir, "wheeldirs"))
     wheeldirs = wheelsfunc.unpackwheels(
         results, workdir=os.path.join(tmpdir, "wheeldirs")
     )
@@ -43,14 +45,47 @@
             assert dylibs == ["libfoo.so"]
         elif "libtwo-0.0.0" in wheeldir:
             assert dylibs == ["libbar.so"]
         else:
             assert False, f"unexpected wheel {wheeldir}"
 
 
+def test_dedupe_mangled(tmpdir):
+    # Integration test that actually does the dedupe workflow on Windows.
+    results = dedupe.dedupe(
+        [FIXTURE_FILES["libfirst.whl"], FIXTURE_FILES["libtwo.whl"]],
+        destdir=tmpdir,
+        mangled=True,
+    )
+    assert len(results) == 2
+
+    os.makedirs(os.path.join(tmpdir, "wheeldirs"))
+    wheeldirs = wheelsfunc.unpackwheels(
+        results, workdir=os.path.join(tmpdir, "wheeldirs")
+    )
+    for wheeldir in wheeldirs:
+        dylibs = []
+        for p in pathlib.Path(wheeldir).rglob("*.dll"):
+            print(p)
+            if ".libs" in str(p):
+                dylibs.append(p.name)
+
+        # libfoo must have been removed from libtwo
+        # and only preserved in libone
+        if "libfirst-0.0.0" in wheeldir:
+            # foo should be mangled according to the libfirst mangling
+            assert dylibs == ["foo-93c7258ead29c23ea6ef9c0778a28c9a.dll"]
+        elif "libtwo-0.0.0" in wheeldir:
+            # bar should be mangled according to libtwo mangling
+            # and foo-1897da919eaed88c4c6f41b2487930e8.dll should have been deleted.
+            assert dylibs == ["bar-d7b39fe6bdc290ef3cdc9fb9c8ded0b9.dll"]
+        else:
+            assert False, f"unexpected wheel {wheeldir}"
+
+
 def test_build_dependencies_tree():
     name2files, deptree = dedupe.build_dependencies_tree(
         [FIXTURE_FILES["libfirst.whl"], FIXTURE_FILES["libtwo.whl"]]
     )
     assert deptree == {"libfirst": [], "libtwo": ["libfirst"]}
```

### Comparing `consolidatewheels-0.3/tests/test_wheels.py` & `consolidatewheels-0.4/tests/test_wheels.py`

 * *Files 21% similar despite different names*

```diff
@@ -36,16 +36,23 @@
 def test_packwheels(tmpdir):
     wheeldir = wheelsfunc.unpackwheels([FIXTURE_FILES["libtwo.whl"]], workdir=tmpdir)
     wheeldir = wheeldir[0]
 
     # Ensure that packing a wheel directory works
     destdir = os.path.join(tmpdir, "wheels")
     wheelsfunc.packwheels([wheeldir], destdir=destdir)
-    assert glob.glob(os.path.join(destdir, "libtwo-0.0.0-cp310-cp310-*.whl"))
+    generated_wheel = glob.glob(os.path.join(destdir, "libtwo-0.0.0-cp310-cp310-*.whl"))
+    assert generated_wheel
 
     # Ensure we trap errors
     with pytest.raises(RuntimeError) as err:
         wheelsfunc.packwheels(["non-existing-dir"], destdir=destdir)
     assert (
         str(err.value)
         == f"Unable to pack non-existing-dir into {os.path.join(destdir, 'tmp')}"
     )
+
+    # Ensure that replacing an existing wheel works.
+    existing_wheel = generated_wheel[0]
+    assert os.path.exists(existing_wheel)
+    result = wheelsfunc.packwheels([wheeldir], destdir=destdir)
+    assert result and result[0] == existing_wheel
```

