# Comparing `tmp/portable-python-1.6.5.tar.gz` & `tmp/portable-python-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portable-python-1.6.5.tar", last modified: Fri May  5 19:48:31 2023, max compression
+gzip compressed data, was "portable-python-1.7.0.tar", last modified: Mon Jun 12 23:04:30 2023, max compression
```

## Comparing `portable-python-1.6.5.tar` & `portable-python-1.7.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:48:31.788893 portable-python-1.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-05 19:47:50.000000 portable-python-1.6.5/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 19:47:50.000000 portable-python-1.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 19:47:50.000000 portable-python-1.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-05 19:48:31.788893 portable-python-1.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-05-05 19:47:50.000000 portable-python-1.6.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-05 19:47:50.000000 portable-python-1.6.5/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 19:47:50.000000 portable-python-1.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:48:31.788893 portable-python-1.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-05 19:47:50.000000 portable-python-1.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:48:31.780893 portable-python-1.6.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:48:31.784893 portable-python-1.6.5/src/portable_python/
--rw-r--r--   0 runner    (1001) docker     (123)    26987 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/cpython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:48:31.788893 portable-python-1.6.5/src/portable_python/external/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/external/_inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/external/tkinter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/external/xcpython.py
--rw-r--r--   0 runner    (1001) docker     (123)    21099 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:48:31.788893 portable-python-1.6.5/src/portable_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-05 19:48:31.000000 portable-python-1.6.5/src/portable_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-05 19:48:31.000000 portable-python-1.6.5/src/portable_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:48:31.000000 portable-python-1.6.5/src/portable_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-05 19:48:31.000000 portable-python-1.6.5/src/portable_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 19:48:31.000000 portable-python-1.6.5/src/portable_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 19:48:31.000000 portable-python-1.6.5/src/portable_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:48:31.788893 portable-python-1.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_failed.py
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_invoker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_recompress.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:04:30.817541 portable-python-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-12 23:03:53.000000 portable-python-1.7.0/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 23:03:53.000000 portable-python-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-12 23:03:53.000000 portable-python-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-06-12 23:04:30.817541 portable-python-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-12 23:03:53.000000 portable-python-1.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 23:03:53.000000 portable-python-1.7.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 23:03:53.000000 portable-python-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 23:03:53.000000 portable-python-1.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 23:04:30.817541 portable-python-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-12 23:03:53.000000 portable-python-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:04:30.813541 portable-python-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:04:30.817541 portable-python-1.7.0/src/portable_python/
+-rw-r--r--   0 runner    (1001) docker     (123)    27141 2023-06-12 23:03:53.000000 portable-python-1.7.0/src/portable_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-12 23:03:53.000000 portable-python-1.7.0/src/portable_python/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-06-12 23:03:53.000000 portable-python-1.7.0/src/portable_python/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-06-12 23:03:53.000000 portable-python-1.7.0/src/portable_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-06-12 23:03:53.000000 portable-python-1.7.0/src/portable_python/cpython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:04:30.817541 portable-python-1.7.0/src/portable_python/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-12 23:03:53.000000 portable-python-1.7.0/src/portable_python/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-12 23:03:53.000000 portable-python-1.7.0/src/portable_python/external/_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-12 23:03:53.000000 portable-python-1.7.0/src/portable_python/external/tkinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-12 23:03:53.000000 portable-python-1.7.0/src/portable_python/external/xcpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21099 2023-06-12 23:03:53.000000 portable-python-1.7.0/src/portable_python/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-12 23:03:53.000000 portable-python-1.7.0/src/portable_python/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-06-12 23:03:53.000000 portable-python-1.7.0/src/portable_python/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:04:30.817541 portable-python-1.7.0/src/portable_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-06-12 23:04:30.000000 portable-python-1.7.0/src/portable_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-12 23:04:30.000000 portable-python-1.7.0/src/portable_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 23:04:30.000000 portable-python-1.7.0/src/portable_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-12 23:04:30.000000 portable-python-1.7.0/src/portable_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-12 23:04:30.000000 portable-python-1.7.0/src/portable_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 23:04:30.000000 portable-python-1.7.0/src/portable_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 23:04:30.817541 portable-python-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-12 23:03:53.000000 portable-python-1.7.0/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-12 23:03:53.000000 portable-python-1.7.0/tests/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-12 23:03:53.000000 portable-python-1.7.0/tests/test_failed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-06-12 23:03:53.000000 portable-python-1.7.0/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-12 23:03:53.000000 portable-python-1.7.0/tests/test_invoker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-12 23:03:53.000000 portable-python-1.7.0/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-12 23:03:53.000000 portable-python-1.7.0/tests/test_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-12 23:03:53.000000 portable-python-1.7.0/tests/test_recompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-12 23:03:53.000000 portable-python-1.7.0/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-12 23:03:53.000000 portable-python-1.7.0/tests/test_setup.py
```

### Comparing `portable-python-1.6.5/DEVELOP.md` & `portable-python-1.7.0/DEVELOP.md`

 * *Files 13% similar despite different names*

```diff
@@ -48,7 +48,28 @@
 You can easily run `portable-python` in a debugger.
 In PyCharm for example, you would simply browse to `.venv/bin/portable-python`
 then right-click and select "Debug portable-python".
 You can then edit the build/run configuration in PyCharm, add some "Parameters" to it,
 like for example `build-report 3.10.5`, and then set breakpoints wherever you like.
 
 There is a `--dryrun` mode that can come in very handy for rapid iterations.
+
+
+# Building a linux binary via docker
+
+Build a docker image, for example using the provided sample `Dockerfile`:
+
+```shell
+docker build -t portable-python-jammy .
+```
+
+Run the docker image, with a folder `/src/` mounted to point to:
+
+```shell
+docker run -it -v./:/src/ portable-python-jammy /bin/bash
+```
+
+Now inside docker, you run a build:
+
+```shell
+portable-python build 3.11.4
+```
```

### Comparing `portable-python-1.6.5/LICENSE` & `portable-python-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/PKG-INFO` & `portable-python-1.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portable-python
-Version: 1.6.5
+Version: 1.7.0
 Summary: Portable python binaries
 Home-page: https://github.com/codrsquad/portable-python
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/portable-python/wiki
 Project-URL: Release notes, https://github.com/codrsquad/portable-python/wiki/Release-notes
@@ -48,165 +48,93 @@
     :alt: Test coverage
 
 .. image:: https://img.shields.io/pypi/pyversions/portable-python.svg
     :target: https://github.com/codrsquad/portable-python
     :alt: Python versions tested (link to github project)
 
 
-This project is a python CLI that aims to make compiling portable python binaries automatable.
+``Portable-Python`` is a CLI (and a python library) for compiling python binaries
+from source than can be decompressed in any folder, and used from there without
+further ado (ie: no need to run an "installer").
 
 
-Supported operating systems
----------------------------
-
-Currently Windows is not supported, contributions are welcome.
-
-Python binaries can be produced as "portable" (statically linked, can run from any folder
-where the binary is unpacked in), or with a ``--prefix`` (build targeted to live in a
-pre-determined folder, like ``/apps/pythonM.m``)
-
-================  ========  ========
-Operating system  Portable  --prefix
-================  ========  ========
-Linux                ✅        ✅
-Macos                ✅        ✅
-Windows              ❌        ❌
-================  ========  ========
-
-
-What is a "portable python"?
-----------------------------
-
-It's a binary python distribution (``.tar.gz`` or ``.zip``) that can be decompressed in any folder,
-and used from there without further ado (ie: no need to run an "installer" and things like that).
+Motivation
+----------
 
 The idea here is to allow for automated systems to:
 
 - Easily obtain a python binary, that can be used in sandboxes / workstations / laptops / instances...
 
-- Have an open source tool that can compile such portable pythons reliably,
-  without having to worry about the compilation part.
-
-- Be able to inspect any python installation, and point out how portable it is,
-  which shared or non-standard libraries it is using
-
-
-Guiding principles
-------------------
-
-- Focuses on just one thing: compile a portable python, and validate that it is indeed portable,
-  produce outcome in (configurable) ``./dist/`` folder and that's it
-
-- Only the last few non-EOL versions of python are supported (no historical stuff)
-
-- As time goes on, the code of this tool will evolve so that the latest pythons keep building
-  (but won't worry that older versions still keep building)
-
-- C compilation is done as simply as possible: no "patching" of any sort,
-  rely solely on the upstream make/configure scripts, typically via stuff like ``--enable-shared=no``
-
-- Builds are validated, an important part of the effort was to write up code that is able to
-  ``inspect`` a python installation and detect whether it is portable or not (and why not if so).
-
-- ``cpython`` is initially supported, but aiming to compile any python family in the future
-  (pypy, conda, ...)
-
-- Cross-compilation would be cool, but only if upstream supports it
-  (ie: only if doable via stuff like ``./configure --host=...`` - no on-the-fly patching allowed)
-
-
-For this repo itself:
-
-- Code is pure python, it is a CLI with one entry-point called ``portable-python``
-
-  - Can be ran in a debugger
-
-  - 100% test coverage, has a ``--dryrun`` mode to help with testing / debugging / seeing what would be done quickly
-
-  - No shell scripts (those are hard to maintain/test/debug)
-
-  - Can be ``pip install``-ed and reused
+- Inspect any python installation, and point out how portable it is, which
+  shared or non-standard libraries it is using
 
 
 Installation
 ------------
 
 ``portable-python`` is a regular python CLI, it can be installed with:
 
 pickley_::
 
     pickley install portable-python
     portable-python --help
-
+    portable-python inspect /usr/bin/python3
 
 Or pipx_::
 
     pipx install portable-python
-
-
-You can also run it directly (without explicit install) with pipx::
-
-    pipx run portable-python inspect /usr/bin/python3
-
+    portable-python inspect /usr/bin/python3
 
 Using ``pip install`` (a CI builder would probably do this)::
 
     /usr/bin/python3 -mvenv /tmp/pp
     /tmp/pp/bin/python -mpip install portable-python
     /tmp/pp/bin/portable-python --help
     /tmp/pp/bin/portable-python inspect /usr/bin/python3
 
 
-Invoke a build from python code::
-
-    from portable_python import BuildSetup
-
-    setup = BuildSetup("cpython:3.9.7")
-    setup.compile()
-
-
-Invoke an inspection from python code::
-
-    from portable_python.inspector import PythonInspector
-
-    inspector = PythonInspector("/usr/bin/python3")
-    print(inspector.represented())
-    problem = inspector.full_so_report.get_problem(portable=True)
-    if problem:
-        print("oops, it is not portable!: %s" % problem)
+Supported operating systems
+---------------------------
 
+Portable python binaries can be built for Linux and MacOS (Intel/M1/M2).
 
-From source, contributions welcome!::
+Currently **Windows is NOT supported**, contributions are welcome.
 
-    git clone https://github.com/codrsquad/portable-python.git
-    cd portable-python
-    tox -e venv
-    .venv/bin/portable-python --help
-    .venv/bin/portable-python inspect /usr/bin/python3
+Python binaries can be produced as "portable" (statically linked, can run from any folder
+where the binary is unpacked in), or with a ``--prefix`` (build targeted to live in a
+pre-determined folder, like ``/apps/pythonM.m``)
 
-    tox -e py39
-    tox -e style
+================  ========  ========
+Operating system  Portable  --prefix
+================  ========  ========
+Linux                ✅        ✅
+Macos                ✅        ✅
+Windows              ❌        ❌
+================  ========  ========
 
 
 Building a portable cpython
 ===========================
 
-Once you've installed ``portable-python``, you can get going like so::
+Once ``portable-python`` is installed:
+
+Build a binary::
 
-    # Build a binary
     cd some-temp-folder
     portable-python build 3.9.7
     ls -l dist/cpython-3.9.7-macos-arm64.tar.gz
 
-    # Unpack it somewhere
-    tar -C ~/.pyenv/versions/ -xf dist/cpython-3.9.7-macos-arm64.tar.gz
-    ls -l ~/.pyenv/versions/
+Unpack it somewhere::
 
-    # It's ready to be used
-    ~/.pyenv/versions/3.9.7/bin/python --version
+    tar -C ~/tmp/versions/ -xf dist/cpython-3.9.7-macos-arm64.tar.gz
+    ls -l ~/tmp/versions/
+
+It's ready to be used::
+
+    ~/tmp/versions/3.9.7/bin/python --version
 
 
 Note that you can use ``--dryrun`` mode to inspect what would be done without doing it::
 
     $ portable-python --dryrun build 3.9.7
 
     INFO selected: xz openssl gdbm (3 modules) xz:5.2.5 openssl:1.1.1k gdbm:1.18.1
@@ -230,14 +158,50 @@
     Would run: ./configure --prefix=/ppp-marker/3.9.7 --enable-optimizations ...
     Would run: /usr/bin/make
     Would run: /usr/bin/make install DESTDIR=build
     ...
     Would tar build/3.9.7 -> dist/cpython-3.9.7-macos-x86_64.tar.gz
 
 
+Library
+-------
+
+Portable Python can be used as a python library to invoke builds, or inspect an installation.
+
+Invoke a build from python code::
+
+    from portable_python import BuildSetup
+
+    setup = BuildSetup("cpython:3.9.7")
+    setup.compile()
+
+
+Invoke an inspection from python code::
+
+    from portable_python.inspector import PythonInspector
+
+    inspector = PythonInspector("/usr/bin/python3")
+    print(inspector.represented())
+    problem = inspector.full_so_report.get_problem(portable=True)
+    if problem:
+        print("oops, it is not portable!: %s" % problem)
+
+
+From source, contributions welcome!::
+
+    git clone https://github.com/codrsquad/portable-python.git
+    cd portable-python
+    tox -e venv
+    .venv/bin/portable-python --help
+    .venv/bin/portable-python inspect /usr/bin/python3
+
+    tox -e py39
+    tox -e style
+
+
 Build folder structure
 ----------------------
 
 ``portable-python`` uses this file structure (build/ and dist/ folders configurable)::
 
     build/
         ppp-marker/3.9.7/                   # Full installation (after build completes)
@@ -245,12 +209,41 @@
         deps/                               # --prefix=.../deps passed to all component ./configure scripts
         sources/
             openssl-1.1.1k.tar.gz           # Downloaded artifacts (downloaded only once)
     dist/
         cpython-3.9.7-macos-arm64.tar.gz    # Ready-to-go portable binary tarball
 
 
-.. _pyenv: https://github.com/pyenv/pyenv
+Guiding principles
+------------------
+
+- Focuses on just one thing: compile a portable python, and validate that it is indeed portable,
+  produce outcome in (configurable) ``./dist/`` folder and that's it
+
+- No patches: C compilation is done as simply as possible without modifying the upstream source code.
+  Rely solely on the make/configure scripts, typically via stuff like ``--enable-shared=no``
+
+- Builds are validated, an important part of the effort was to write up code that is able to
+  ``inspect`` a python installation and detect whether it is portable or not (and why not if so).
+
+- Only the last few non-EOL versions of python are supported (no historical stuff)
+
+- As time goes on, the code of this tool will evolve so that the latest pythons keep building
+  (but won't worry that older versions still keep building)
+
+
+For this repo itself:
+
+- Code is pure python, it is a CLI with one entry-point called ``portable-python``
+
+  - Can be ran in a debugger
+
+  - 100% test coverage, has a ``--dryrun`` mode to help with testing / debugging / seeing what would be done quickly
+
+  - No shell scripts (those are hard to maintain/test/debug)
+
+  - Can be ``pip install``-ed and reused
+
 
 .. _pickley: https://pypi.org/project/pickley/
 
 .. _pipx: https://pypi.org/project/pipx/
```

### Comparing `portable-python-1.6.5/README.rst` & `portable-python-1.7.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -14,165 +14,93 @@
     :alt: Test coverage
 
 .. image:: https://img.shields.io/pypi/pyversions/portable-python.svg
     :target: https://github.com/codrsquad/portable-python
     :alt: Python versions tested (link to github project)
 
 
-This project is a python CLI that aims to make compiling portable python binaries automatable.
+``Portable-Python`` is a CLI (and a python library) for compiling python binaries
+from source than can be decompressed in any folder, and used from there without
+further ado (ie: no need to run an "installer").
 
 
-Supported operating systems
----------------------------
-
-Currently Windows is not supported, contributions are welcome.
-
-Python binaries can be produced as "portable" (statically linked, can run from any folder
-where the binary is unpacked in), or with a ``--prefix`` (build targeted to live in a
-pre-determined folder, like ``/apps/pythonM.m``)
-
-================  ========  ========
-Operating system  Portable  --prefix
-================  ========  ========
-Linux                ✅        ✅
-Macos                ✅        ✅
-Windows              ❌        ❌
-================  ========  ========
-
-
-What is a "portable python"?
-----------------------------
-
-It's a binary python distribution (``.tar.gz`` or ``.zip``) that can be decompressed in any folder,
-and used from there without further ado (ie: no need to run an "installer" and things like that).
+Motivation
+----------
 
 The idea here is to allow for automated systems to:
 
 - Easily obtain a python binary, that can be used in sandboxes / workstations / laptops / instances...
 
-- Have an open source tool that can compile such portable pythons reliably,
-  without having to worry about the compilation part.
-
-- Be able to inspect any python installation, and point out how portable it is,
-  which shared or non-standard libraries it is using
-
-
-Guiding principles
-------------------
-
-- Focuses on just one thing: compile a portable python, and validate that it is indeed portable,
-  produce outcome in (configurable) ``./dist/`` folder and that's it
-
-- Only the last few non-EOL versions of python are supported (no historical stuff)
-
-- As time goes on, the code of this tool will evolve so that the latest pythons keep building
-  (but won't worry that older versions still keep building)
-
-- C compilation is done as simply as possible: no "patching" of any sort,
-  rely solely on the upstream make/configure scripts, typically via stuff like ``--enable-shared=no``
-
-- Builds are validated, an important part of the effort was to write up code that is able to
-  ``inspect`` a python installation and detect whether it is portable or not (and why not if so).
-
-- ``cpython`` is initially supported, but aiming to compile any python family in the future
-  (pypy, conda, ...)
-
-- Cross-compilation would be cool, but only if upstream supports it
-  (ie: only if doable via stuff like ``./configure --host=...`` - no on-the-fly patching allowed)
-
-
-For this repo itself:
-
-- Code is pure python, it is a CLI with one entry-point called ``portable-python``
-
-  - Can be ran in a debugger
-
-  - 100% test coverage, has a ``--dryrun`` mode to help with testing / debugging / seeing what would be done quickly
-
-  - No shell scripts (those are hard to maintain/test/debug)
-
-  - Can be ``pip install``-ed and reused
+- Inspect any python installation, and point out how portable it is, which
+  shared or non-standard libraries it is using
 
 
 Installation
 ------------
 
 ``portable-python`` is a regular python CLI, it can be installed with:
 
 pickley_::
 
     pickley install portable-python
     portable-python --help
-
+    portable-python inspect /usr/bin/python3
 
 Or pipx_::
 
     pipx install portable-python
-
-
-You can also run it directly (without explicit install) with pipx::
-
-    pipx run portable-python inspect /usr/bin/python3
-
+    portable-python inspect /usr/bin/python3
 
 Using ``pip install`` (a CI builder would probably do this)::
 
     /usr/bin/python3 -mvenv /tmp/pp
     /tmp/pp/bin/python -mpip install portable-python
     /tmp/pp/bin/portable-python --help
     /tmp/pp/bin/portable-python inspect /usr/bin/python3
 
 
-Invoke a build from python code::
-
-    from portable_python import BuildSetup
-
-    setup = BuildSetup("cpython:3.9.7")
-    setup.compile()
-
-
-Invoke an inspection from python code::
-
-    from portable_python.inspector import PythonInspector
-
-    inspector = PythonInspector("/usr/bin/python3")
-    print(inspector.represented())
-    problem = inspector.full_so_report.get_problem(portable=True)
-    if problem:
-        print("oops, it is not portable!: %s" % problem)
+Supported operating systems
+---------------------------
 
+Portable python binaries can be built for Linux and MacOS (Intel/M1/M2).
 
-From source, contributions welcome!::
+Currently **Windows is NOT supported**, contributions are welcome.
 
-    git clone https://github.com/codrsquad/portable-python.git
-    cd portable-python
-    tox -e venv
-    .venv/bin/portable-python --help
-    .venv/bin/portable-python inspect /usr/bin/python3
+Python binaries can be produced as "portable" (statically linked, can run from any folder
+where the binary is unpacked in), or with a ``--prefix`` (build targeted to live in a
+pre-determined folder, like ``/apps/pythonM.m``)
 
-    tox -e py39
-    tox -e style
+================  ========  ========
+Operating system  Portable  --prefix
+================  ========  ========
+Linux                ✅        ✅
+Macos                ✅        ✅
+Windows              ❌        ❌
+================  ========  ========
 
 
 Building a portable cpython
 ===========================
 
-Once you've installed ``portable-python``, you can get going like so::
+Once ``portable-python`` is installed:
+
+Build a binary::
 
-    # Build a binary
     cd some-temp-folder
     portable-python build 3.9.7
     ls -l dist/cpython-3.9.7-macos-arm64.tar.gz
 
-    # Unpack it somewhere
-    tar -C ~/.pyenv/versions/ -xf dist/cpython-3.9.7-macos-arm64.tar.gz
-    ls -l ~/.pyenv/versions/
+Unpack it somewhere::
 
-    # It's ready to be used
-    ~/.pyenv/versions/3.9.7/bin/python --version
+    tar -C ~/tmp/versions/ -xf dist/cpython-3.9.7-macos-arm64.tar.gz
+    ls -l ~/tmp/versions/
+
+It's ready to be used::
+
+    ~/tmp/versions/3.9.7/bin/python --version
 
 
 Note that you can use ``--dryrun`` mode to inspect what would be done without doing it::
 
     $ portable-python --dryrun build 3.9.7
 
     INFO selected: xz openssl gdbm (3 modules) xz:5.2.5 openssl:1.1.1k gdbm:1.18.1
@@ -196,14 +124,50 @@
     Would run: ./configure --prefix=/ppp-marker/3.9.7 --enable-optimizations ...
     Would run: /usr/bin/make
     Would run: /usr/bin/make install DESTDIR=build
     ...
     Would tar build/3.9.7 -> dist/cpython-3.9.7-macos-x86_64.tar.gz
 
 
+Library
+-------
+
+Portable Python can be used as a python library to invoke builds, or inspect an installation.
+
+Invoke a build from python code::
+
+    from portable_python import BuildSetup
+
+    setup = BuildSetup("cpython:3.9.7")
+    setup.compile()
+
+
+Invoke an inspection from python code::
+
+    from portable_python.inspector import PythonInspector
+
+    inspector = PythonInspector("/usr/bin/python3")
+    print(inspector.represented())
+    problem = inspector.full_so_report.get_problem(portable=True)
+    if problem:
+        print("oops, it is not portable!: %s" % problem)
+
+
+From source, contributions welcome!::
+
+    git clone https://github.com/codrsquad/portable-python.git
+    cd portable-python
+    tox -e venv
+    .venv/bin/portable-python --help
+    .venv/bin/portable-python inspect /usr/bin/python3
+
+    tox -e py39
+    tox -e style
+
+
 Build folder structure
 ----------------------
 
 ``portable-python`` uses this file structure (build/ and dist/ folders configurable)::
 
     build/
         ppp-marker/3.9.7/                   # Full installation (after build completes)
@@ -211,12 +175,41 @@
         deps/                               # --prefix=.../deps passed to all component ./configure scripts
         sources/
             openssl-1.1.1k.tar.gz           # Downloaded artifacts (downloaded only once)
     dist/
         cpython-3.9.7-macos-arm64.tar.gz    # Ready-to-go portable binary tarball
 
 
-.. _pyenv: https://github.com/pyenv/pyenv
+Guiding principles
+------------------
+
+- Focuses on just one thing: compile a portable python, and validate that it is indeed portable,
+  produce outcome in (configurable) ``./dist/`` folder and that's it
+
+- No patches: C compilation is done as simply as possible without modifying the upstream source code.
+  Rely solely on the make/configure scripts, typically via stuff like ``--enable-shared=no``
+
+- Builds are validated, an important part of the effort was to write up code that is able to
+  ``inspect`` a python installation and detect whether it is portable or not (and why not if so).
+
+- Only the last few non-EOL versions of python are supported (no historical stuff)
+
+- As time goes on, the code of this tool will evolve so that the latest pythons keep building
+  (but won't worry that older versions still keep building)
+
+
+For this repo itself:
+
+- Code is pure python, it is a CLI with one entry-point called ``portable-python``
+
+  - Can be ran in a debugger
+
+  - 100% test coverage, has a ``--dryrun`` mode to help with testing / debugging / seeing what would be done quickly
+
+  - No shell scripts (those are hard to maintain/test/debug)
+
+  - Can be ``pip install``-ed and reused
+
 
 .. _pickley: https://pypi.org/project/pickley/
 
 .. _pipx: https://pypi.org/project/pipx/
```

### Comparing `portable-python-1.6.5/setup.py` & `portable-python-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/src/portable_python/__init__.py` & `portable-python-1.7.0/src/portable_python/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,28 +193,30 @@
         """
         Args:
             python_spec (str | PythonSpec | None): Python to build (family and version)
             modules (str | None): Modules to build (default: from config)
             prefix (str | None): --prefix to use
         """
         if isinstance(python_spec, str):
-            v = Version.from_text(python_spec)
-            if v and not v.is_final:
+            v = Version(python_spec)
+            if v.is_valid and not v.is_final:
                 # Accept release candidates
                 family = python_spec.rpartition(":")[0] or "cpython"
-                python_spec = PythonSpec.to_spec(f"{family}:{v.main}")
+                python_spec = PythonSpec.from_text(f"{family}:{v.main}")
                 python_spec.version = v
 
         if not python_spec or python_spec == "latest":
             python_spec = "cpython:%s" % PPG.cpython.latest
 
-        python_spec = PythonSpec.to_spec(python_spec)
-        if not python_spec.version or not python_spec.version.is_valid:
-            runez.abort("Invalid python spec: %s" % runez.red(python_spec))
+        if not isinstance(python_spec, PythonSpec):
+            ps = PythonSpec.from_text(python_spec)
+            runez.abort_if(not ps, "Invalid python spec: %s" % runez.red(python_spec))
+            python_spec = ps
 
+        runez.abort_if(not python_spec.version or not python_spec.version.is_valid, "Invalid python spec: %s" % runez.red(python_spec))
         if len(python_spec.version.given_components) < 3:
             runez.abort("Please provide full desired version: %s is not good enough" % runez.red(python_spec))
 
         self.python_spec = python_spec
         self.folders = PPG.get_folders(base=os.getcwd(), family=python_spec.family, version=python_spec.version)
         self.desired_modules = modules
         prefix = self.folders.formatted(prefix)
```

### Comparing `portable-python-1.6.5/src/portable_python/cli.py` & `portable-python-1.7.0/src/portable_python/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 import click
 import runez
-from runez.pyenv import PythonDepot, PythonSpec
+from runez.pyenv import PythonSpec
 from runez.render import PrettyTable
 
 from portable_python import BuildSetup, PPG
 from portable_python.inspector import LibAutoCorrect, PythonInspector
 
 
 LOG = logging.getLogger(__name__)
@@ -56,23 +56,20 @@
     setup.validate_module_selection()
 
 
 @main.command()
 def diagnostics():
     """Show diagnostics info"""
     with runez.Anchored("."):
-        depot = PythonDepot(use_path=True)
-        depot.scan_path_env_var()
-
         def _diagnostics():
-            yield "invoker python", depot.invoker
+            yield "invoker python", runez.SYS_INFO.invoker_python
             yield from runez.SYS_INFO.diagnostics()
 
         config = PPG.config.represented()
-        print(PrettyTable.two_column_diagnostics(_diagnostics(), depot.representation(), config))
+        print(PrettyTable.two_column_diagnostics(_diagnostics(), config))
 
 
 @main.command()
 @click.option("--modules", "-m", help="Modules to inspect")
 @click.option("--verbose", "-v", is_flag=True, help="Show full so report")
 @click.option("--prefix", "-p", is_flag=True, help="Build was done with --prefix (not portable)")
 @click.option("--skip-so", "-s", is_flag=True, help="Don't check all .so-s")
@@ -159,15 +156,15 @@
     """
     Re-compress an existing binary tarball, or folder
 
     \b
     Mildly useful for comparing sizes from different compressions
     """
     extension = runez.SYS_INFO.platform_id.canonical_compress_extension(ext)
-    pspec = PythonSpec.to_spec(path)
+    pspec = PythonSpec.from_text(path)
     folders = PPG.get_folders(base=".", family=pspec and pspec.family, version=pspec and pspec.version)
     with runez.Anchored(folders.base_folder):
         actual_path = _find_recompress_source(folders, path)
         if not actual_path:
             runez.abort("'%s' does not exist" % runez.red(runez.short(path)))
 
         if actual_path.is_dir():
```

### Comparing `portable-python-1.6.5/src/portable_python/config.py` & `portable-python-1.7.0/src/portable_python/config.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/src/portable_python/cpython.py` & `portable-python-1.7.0/src/portable_python/cpython.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,41 +93,39 @@
             db_order = runez.joined(db_order, delimiter=":")
             if db_order:
                 yield f"--with-dbmliborder={db_order}"
 
         tkinter = self.active_module(TkInter)
         if tkinter:
             # TODO: this doesn't seem to be enough, on macos cpython's ./configure still picks up the shared macos tcl/tk libs
-            version = Version.from_text(tkinter.version)
+            version = Version(tkinter.version)
             yield f"--with-tcltk-includes=-I{self.deps}/include"
             yield f"--with-tcltk-libs=-L{self.deps_lib} -ltcl{version.mm} -ltk{version.mm}"
 
     @runez.cached_property
     def config_folder(self):
         for path in runez.ls_dir(self.install_folder / f"lib/python{self.version.mm}"):
             if path.name.startswith("config-"):
                 return path
 
     def _prepare(self):
         super()._prepare()
         if PPG.target.is_macos:
-            brew_path = os.path.join(self.setup.build_context.usr_local, "bin/brew")
-            if os.path.exists(brew_path):
-                # Avoid pollution of static builds via /usr/local on macos
-                rx = re.compile(r"^(Doc|Grammar|Lib|Misc|Modules|PC|Tools|msi|.*\.(md|html|man|pro|rst))$")
-                patch_folder(self.m_src_build, r"/usr/local\b", self.deps.as_posix(), ignore=rx)
-                setup_py = self.m_src_build / "setup.py"
-                if setup_py.exists():
-                    # Special edge case in macosx_sdk_specified() where /usr/local is fine...
-                    x = "startswith({q}/usr/{q}) and not path.startswith({q}{p}{q})"
-                    special_case = x.replace("(", r"\(").replace(")", r"\)").format(q="['\"]", p=self.deps)
-                    restored = x.format(q="'", p='/usr/local')
-                    patch_file(setup_py, special_case, restored)
+            # Avoid pollution of static builds via /usr/local on macOS
+            rx = re.compile(r"^(Doc|Grammar|Lib|Misc|Modules|PC|Tools|msi|.*\.(md|html|man|pro|rst))$")
+            patch_folder(self.m_src_build, r"/usr/local\b", self.deps.as_posix(), ignore=rx)
+            setup_py = self.m_src_build / "setup.py"
+            if setup_py.exists():
+                # Special edge case in macosx_sdk_specified() where /usr/local is fine...
+                x = "startswith({q}/usr/{q}) and not path.startswith({q}{p}{q})"
+                special_case = x.replace("(", r"\(").replace(")", r"\)").format(q="['\"]", p=self.deps)
+                restored = x.format(q="'", p='/usr/local')
+                patch_file(setup_py, special_case, restored)
 
-            # Only doable on macos: patch -install_name so produced exes/libs use a relative path
+            # Only doable on macOS: patch -install_name so produced exes/libs use a relative path
             install_name = "-Wl,-install_name,@executable_path/.."
             patch_folder(self.m_src_build, r"-Wl,-install_name,\$\(prefix\)", install_name)
 
     def _do_linux_compile(self):
         self.run_configure("./configure", self.c_configure_args(), prefix=self.c_configure_prefix)
         make_args = []
         if self.version < "3.8":
@@ -290,15 +288,15 @@
             LOG.info("Auto-corrected shebang for %s" % runez.short(path))
             with open(path, "wt") as fh:
                 for line in lines:
                     fh.write(line)
 
 
 class RelSysConf:
-    """Make _sysconfigdata report paths (prefix etc) relative to its current location"""
+    """Make _sysconfigdata report paths (eg: prefix) relative to its current location"""
 
     def __init__(self, path, prefix):
         self.path = path
         self.prefix = prefix
         self.rx_marker = re.compile(r"^build_time_vars\s*=.*")
         self.rx_strings = re.compile(r"(['\"])([^'\"]+)(['\"])")
         self.text = "\n".join(self._process_file())
```

### Comparing `portable-python-1.6.5/src/portable_python/external/__init__.py` & `portable-python-1.7.0/src/portable_python/external/__init__.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/src/portable_python/external/_inspect.py` & `portable-python-1.7.0/src/portable_python/external/_inspect.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/src/portable_python/external/tkinter.py` & `portable-python-1.7.0/src/portable_python/external/tkinter.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/src/portable_python/external/xcpython.py` & `portable-python-1.7.0/src/portable_python/external/xcpython.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
     @property
     def url(self):
         return f"https://www.openssl.org/source/openssl-{self.version}.tar.gz"
 
     @property
     def version(self):
-        return self.cfg_version("1.1.1t")
+        return self.cfg_version("1.1.1u")
 
     def c_configure_args(self):
         yield "--openssldir=/etc/ssl"
         yield "no-shared", "no-idea", "no-tests"
 
     def _do_linux_compile(self):
         self.run_configure("./config", "-v", self.c_configure_args())
@@ -166,16 +166,15 @@
 
     @property
     def url(self):
         return f"https://ftp.gnu.org/pub/gnu/ncurses/ncurses-{self.version}.tar.gz"
 
     @property
     def version(self):
-        # 6.3's configure fails with --enable-pc-files for some reason with py3.11 (looks like an internal error)
-        return self.cfg_version("6.2")
+        return self.cfg_version("6.4")
 
     def c_configure_args(self):
         yield "--disable-shared"
         yield "--enable-static"
         yield "--without-ada"
         yield "--disable-db-install"
         yield "--without-manpages"
@@ -220,22 +219,23 @@
 
     @property
     def url(self):
         return f"https://ftp.gnu.org/gnu/readline/readline-{self.version}.tar.gz"
 
     @property
     def version(self):
-        return self.cfg_version("8.1.2")
+        return self.cfg_version("8.2")
 
     def _do_linux_compile(self):
         self.run_configure(
-            "./configure", "--disable-shared", "--enable-static", "--with-curses", "--enable-multibyte", "--disable-install-examples"
+            "./configure", "--disable-shared", "--enable-static", "--with-curses", "--enable-multibyte",
+            "--disable-install-examples", "--disable-docs", "--enable-portable-binary",
         )
-        self.run_make()
-        self.run_make("install")
+        self.run_make(cpu_count=0)
+        self.run_make("install", cpu_count=0)
 
 
 class Sqlite(ModuleBuilder):
     """
     Known issues:
     - linux: libsqlite3-dev must be installed in order for static build to succeed
     """
@@ -253,15 +253,15 @@
 
     @property
     def url(self):
         return f"https://github.com/sqlite/sqlite/archive/refs/tags/version-{self.version}.tar.gz"
 
     @property
     def version(self):
-        return self.cfg_version("3.41.2")
+        return self.cfg_version("3.42.0")
 
     def _do_linux_compile(self):
         self.run_configure(
             "./configure", "--enable-shared=no", "--enable-static=yes", "--disable-tcl", "--disable-readline", "--with-pic=yes"
         )
         self.run_make()
         self.run_make("install")
@@ -303,16 +303,15 @@
 
     @property
     def url(self):
         return f"https://tukaani.org/xz/xz-{self.version}.tar.gz"
 
     @property
     def version(self):
-        # With 5.2.7 C compilation error on linux: version node not found for symbol lzma_get_progress@@XZ_5.2
-        return self.cfg_version("5.2.6")
+        return self.cfg_version("5.4.3")
 
     def _do_linux_compile(self):
         self.run_configure(
             "./configure",
             "--enable-shared=no", "--enable-static=yes", "--with-pic=yes", "--disable-rpath",
             "--disable-dependency-tracking", "--disable-doc", "--disable-nls", "--without-libintl-prefix",
         )
```

### Comparing `portable-python-1.6.5/src/portable_python/inspector.py` & `portable-python-1.7.0/src/portable_python/inspector.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/src/portable_python/tracking.py` & `portable-python-1.7.0/src/portable_python/tracking.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/src/portable_python/versions.py` & `portable-python-1.7.0/src/portable_python/versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def __repr__(self):
         return self.family_name
 
     def _fetch_versions(self):
         if self._versions is None:
             self._versions = {}
             versions = self.get_available_versions()
-            versions = versions and sorted((Version.from_text(x) for x in versions), reverse=True)
+            versions = versions and sorted(versions, reverse=True)
             if versions:
                 self._latest = versions[0]
                 for v in versions:
                     if v.mm not in self._versions:
                         self._versions[v.mm] = v
 
     @property
@@ -106,15 +106,15 @@
 
 class Folders:
 
     def __init__(self, config: Config, base=None, family=None, version=None):
         self.config = config
         self.base_folder = runez.resolved_path(base)
         self.family = family
-        self.version = Version.from_text(version, strict=True)
+        self.version = Version.from_object(version)
         self.mm = self.version and self.version.mm
         self.completions = config.completions(family=family, version=version, mm=self.mm)
         self.build_folder = self._get_path("build")
         self.completions["build"] = self.build_folder
         self.components = self.build_folder / "components"
         self.deps = self.build_folder / "deps"
         self.destdir = self._get_path("destdir")
@@ -186,15 +186,15 @@
             runez.abort(f"Python family '{family_name}' is not yet supported")
 
         return fam
 
     @classmethod
     def find_python(cls, spec):
         if cls._depot is None:
-            cls._depot = PythonDepot(use_path=False)
+            cls._depot = PythonDepot("PATH")
 
         return cls._depot.find_python(spec)
 
     @classmethod
     def find_telltale(cls, *telltales):
         for tt in runez.flattened(telltales):
             for sys_include in runez.flattened(cls.target.sys_include):
```

### Comparing `portable-python-1.6.5/src/portable_python.egg-info/PKG-INFO` & `portable-python-1.7.0/src/portable_python.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portable-python
-Version: 1.6.5
+Version: 1.7.0
 Summary: Portable python binaries
 Home-page: https://github.com/codrsquad/portable-python
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/portable-python/wiki
 Project-URL: Release notes, https://github.com/codrsquad/portable-python/wiki/Release-notes
@@ -48,165 +48,93 @@
     :alt: Test coverage
 
 .. image:: https://img.shields.io/pypi/pyversions/portable-python.svg
     :target: https://github.com/codrsquad/portable-python
     :alt: Python versions tested (link to github project)
 
 
-This project is a python CLI that aims to make compiling portable python binaries automatable.
+``Portable-Python`` is a CLI (and a python library) for compiling python binaries
+from source than can be decompressed in any folder, and used from there without
+further ado (ie: no need to run an "installer").
 
 
-Supported operating systems
----------------------------
-
-Currently Windows is not supported, contributions are welcome.
-
-Python binaries can be produced as "portable" (statically linked, can run from any folder
-where the binary is unpacked in), or with a ``--prefix`` (build targeted to live in a
-pre-determined folder, like ``/apps/pythonM.m``)
-
-================  ========  ========
-Operating system  Portable  --prefix
-================  ========  ========
-Linux                ✅        ✅
-Macos                ✅        ✅
-Windows              ❌        ❌
-================  ========  ========
-
-
-What is a "portable python"?
-----------------------------
-
-It's a binary python distribution (``.tar.gz`` or ``.zip``) that can be decompressed in any folder,
-and used from there without further ado (ie: no need to run an "installer" and things like that).
+Motivation
+----------
 
 The idea here is to allow for automated systems to:
 
 - Easily obtain a python binary, that can be used in sandboxes / workstations / laptops / instances...
 
-- Have an open source tool that can compile such portable pythons reliably,
-  without having to worry about the compilation part.
-
-- Be able to inspect any python installation, and point out how portable it is,
-  which shared or non-standard libraries it is using
-
-
-Guiding principles
-------------------
-
-- Focuses on just one thing: compile a portable python, and validate that it is indeed portable,
-  produce outcome in (configurable) ``./dist/`` folder and that's it
-
-- Only the last few non-EOL versions of python are supported (no historical stuff)
-
-- As time goes on, the code of this tool will evolve so that the latest pythons keep building
-  (but won't worry that older versions still keep building)
-
-- C compilation is done as simply as possible: no "patching" of any sort,
-  rely solely on the upstream make/configure scripts, typically via stuff like ``--enable-shared=no``
-
-- Builds are validated, an important part of the effort was to write up code that is able to
-  ``inspect`` a python installation and detect whether it is portable or not (and why not if so).
-
-- ``cpython`` is initially supported, but aiming to compile any python family in the future
-  (pypy, conda, ...)
-
-- Cross-compilation would be cool, but only if upstream supports it
-  (ie: only if doable via stuff like ``./configure --host=...`` - no on-the-fly patching allowed)
-
-
-For this repo itself:
-
-- Code is pure python, it is a CLI with one entry-point called ``portable-python``
-
-  - Can be ran in a debugger
-
-  - 100% test coverage, has a ``--dryrun`` mode to help with testing / debugging / seeing what would be done quickly
-
-  - No shell scripts (those are hard to maintain/test/debug)
-
-  - Can be ``pip install``-ed and reused
+- Inspect any python installation, and point out how portable it is, which
+  shared or non-standard libraries it is using
 
 
 Installation
 ------------
 
 ``portable-python`` is a regular python CLI, it can be installed with:
 
 pickley_::
 
     pickley install portable-python
     portable-python --help
-
+    portable-python inspect /usr/bin/python3
 
 Or pipx_::
 
     pipx install portable-python
-
-
-You can also run it directly (without explicit install) with pipx::
-
-    pipx run portable-python inspect /usr/bin/python3
-
+    portable-python inspect /usr/bin/python3
 
 Using ``pip install`` (a CI builder would probably do this)::
 
     /usr/bin/python3 -mvenv /tmp/pp
     /tmp/pp/bin/python -mpip install portable-python
     /tmp/pp/bin/portable-python --help
     /tmp/pp/bin/portable-python inspect /usr/bin/python3
 
 
-Invoke a build from python code::
-
-    from portable_python import BuildSetup
-
-    setup = BuildSetup("cpython:3.9.7")
-    setup.compile()
-
-
-Invoke an inspection from python code::
-
-    from portable_python.inspector import PythonInspector
-
-    inspector = PythonInspector("/usr/bin/python3")
-    print(inspector.represented())
-    problem = inspector.full_so_report.get_problem(portable=True)
-    if problem:
-        print("oops, it is not portable!: %s" % problem)
+Supported operating systems
+---------------------------
 
+Portable python binaries can be built for Linux and MacOS (Intel/M1/M2).
 
-From source, contributions welcome!::
+Currently **Windows is NOT supported**, contributions are welcome.
 
-    git clone https://github.com/codrsquad/portable-python.git
-    cd portable-python
-    tox -e venv
-    .venv/bin/portable-python --help
-    .venv/bin/portable-python inspect /usr/bin/python3
+Python binaries can be produced as "portable" (statically linked, can run from any folder
+where the binary is unpacked in), or with a ``--prefix`` (build targeted to live in a
+pre-determined folder, like ``/apps/pythonM.m``)
 
-    tox -e py39
-    tox -e style
+================  ========  ========
+Operating system  Portable  --prefix
+================  ========  ========
+Linux                ✅        ✅
+Macos                ✅        ✅
+Windows              ❌        ❌
+================  ========  ========
 
 
 Building a portable cpython
 ===========================
 
-Once you've installed ``portable-python``, you can get going like so::
+Once ``portable-python`` is installed:
+
+Build a binary::
 
-    # Build a binary
     cd some-temp-folder
     portable-python build 3.9.7
     ls -l dist/cpython-3.9.7-macos-arm64.tar.gz
 
-    # Unpack it somewhere
-    tar -C ~/.pyenv/versions/ -xf dist/cpython-3.9.7-macos-arm64.tar.gz
-    ls -l ~/.pyenv/versions/
+Unpack it somewhere::
 
-    # It's ready to be used
-    ~/.pyenv/versions/3.9.7/bin/python --version
+    tar -C ~/tmp/versions/ -xf dist/cpython-3.9.7-macos-arm64.tar.gz
+    ls -l ~/tmp/versions/
+
+It's ready to be used::
+
+    ~/tmp/versions/3.9.7/bin/python --version
 
 
 Note that you can use ``--dryrun`` mode to inspect what would be done without doing it::
 
     $ portable-python --dryrun build 3.9.7
 
     INFO selected: xz openssl gdbm (3 modules) xz:5.2.5 openssl:1.1.1k gdbm:1.18.1
@@ -230,14 +158,50 @@
     Would run: ./configure --prefix=/ppp-marker/3.9.7 --enable-optimizations ...
     Would run: /usr/bin/make
     Would run: /usr/bin/make install DESTDIR=build
     ...
     Would tar build/3.9.7 -> dist/cpython-3.9.7-macos-x86_64.tar.gz
 
 
+Library
+-------
+
+Portable Python can be used as a python library to invoke builds, or inspect an installation.
+
+Invoke a build from python code::
+
+    from portable_python import BuildSetup
+
+    setup = BuildSetup("cpython:3.9.7")
+    setup.compile()
+
+
+Invoke an inspection from python code::
+
+    from portable_python.inspector import PythonInspector
+
+    inspector = PythonInspector("/usr/bin/python3")
+    print(inspector.represented())
+    problem = inspector.full_so_report.get_problem(portable=True)
+    if problem:
+        print("oops, it is not portable!: %s" % problem)
+
+
+From source, contributions welcome!::
+
+    git clone https://github.com/codrsquad/portable-python.git
+    cd portable-python
+    tox -e venv
+    .venv/bin/portable-python --help
+    .venv/bin/portable-python inspect /usr/bin/python3
+
+    tox -e py39
+    tox -e style
+
+
 Build folder structure
 ----------------------
 
 ``portable-python`` uses this file structure (build/ and dist/ folders configurable)::
 
     build/
         ppp-marker/3.9.7/                   # Full installation (after build completes)
@@ -245,12 +209,41 @@
         deps/                               # --prefix=.../deps passed to all component ./configure scripts
         sources/
             openssl-1.1.1k.tar.gz           # Downloaded artifacts (downloaded only once)
     dist/
         cpython-3.9.7-macos-arm64.tar.gz    # Ready-to-go portable binary tarball
 
 
-.. _pyenv: https://github.com/pyenv/pyenv
+Guiding principles
+------------------
+
+- Focuses on just one thing: compile a portable python, and validate that it is indeed portable,
+  produce outcome in (configurable) ``./dist/`` folder and that's it
+
+- No patches: C compilation is done as simply as possible without modifying the upstream source code.
+  Rely solely on the make/configure scripts, typically via stuff like ``--enable-shared=no``
+
+- Builds are validated, an important part of the effort was to write up code that is able to
+  ``inspect`` a python installation and detect whether it is portable or not (and why not if so).
+
+- Only the last few non-EOL versions of python are supported (no historical stuff)
+
+- As time goes on, the code of this tool will evolve so that the latest pythons keep building
+  (but won't worry that older versions still keep building)
+
+
+For this repo itself:
+
+- Code is pure python, it is a CLI with one entry-point called ``portable-python``
+
+  - Can be ran in a debugger
+
+  - 100% test coverage, has a ``--dryrun`` mode to help with testing / debugging / seeing what would be done quickly
+
+  - No shell scripts (those are hard to maintain/test/debug)
+
+  - Can be ``pip install``-ed and reused
+
 
 .. _pickley: https://pypi.org/project/pickley/
 
 .. _pipx: https://pypi.org/project/pipx/
```

### Comparing `portable-python-1.6.5/src/portable_python.egg-info/SOURCES.txt` & `portable-python-1.7.0/src/portable_python.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 DEVELOP.md
 LICENSE
 MANIFEST.in
 README.rst
 SECURITY.md
 pyproject.toml
+requirements.txt
 setup.py
 src/portable_python/__init__.py
 src/portable_python/__main__.py
 src/portable_python/cli.py
 src/portable_python/config.py
 src/portable_python/cpython.py
 src/portable_python/inspector.py
```

### Comparing `portable-python-1.6.5/tests/test_build.py` & `portable-python-1.7.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/tests/test_cleanup.py` & `portable-python-1.7.0/tests/test_cleanup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def test_cleanup(cli, monkeypatch):
     f = PPG.get_folders(version="3.7.12")
     install_dir = f.resolved_destdir()
     lib = install_dir / "lib"
 
     # Simulate presence of some key files to verify code that is detecting them is hit
-    runez.write(f.components / "cpython/Mac/Makefile.in", "hmm\nmentions /usr/local", logger=None)
+    runez.write(f.components / "cpython/Mac/Makefile.in", "hmm\nmentions /usr/local\n", logger=None)
     runez.write(f.components / "cpython/Lib/trace.py", "hmm\nmentions /usr/local", logger=None)  # ignored because in Lib/ folder
     runez.write(f.components / "cpython/setup.py", "path.startswith('/usr/') and not path.startswith('/usr/local')", logger=None)
     runez.write(f.components / "cpython/foo", b"hello\xe4 /usr/local", logger=None)
     runez.touch(f.deps / "bin/bzcat", logger=None)
     runez.touch(f.deps / "include/readline/readline.h", logger=None)
     runez.touch(f.deps / "lib/libssl.a", logger=None)
     os.chmod(f.deps / "lib/libssl.a", 0o755)
@@ -28,14 +28,15 @@
     runez.write(lib / f"libpython{f.mm}.a", sample_content, logger=None)
     runez.write(lib / f"python{f.mm}/config-{f.mm}-darwin/libpython{f.mm}.a", sample_content, logger=None)
     runez.touch(lib / f"python{f.mm}/site-packages/setuptools", logger=None)
 
     cfg = cli.tests_path("sample-config1.yml")
     cli.run("-ntmacos-x86_64", f"-c{cfg}", "build", "-mopenssl,readline", f.version)
     assert cli.succeeded
+    assert "Patched '/usr/local\\b' in build/components/cpython/Mac/Makefile.in" in cli.logged
     assert "MACOSX_DEPLOYMENT_TARGET=10.25" in cli.logged
     assert "Cleaned 2 build artifacts" in cli.logged  # 1st pass
     assert "Cleaned 3 build artifacts" in cli.logged  # 2nd pass
     assert f"Corrected permissions for {f.deps}/lib/libssl.a" in cli.logged
     assert f" install DESTDIR={f.build_folder}\n" in cli.logged
     cli.match("Patched 'startswith(...)' in build/components/cpython/setup.py")
     assert "Exercising configured validation script" in cli.logged
@@ -50,11 +51,10 @@
     assert f"Would tar {install_dir} -> dist/cpython-{f.version}-linux-x86_64.tar.gz" in cli.logged
 
     runez.touch("bin/brew", logger=None)
     runez.touch("include/dbm.h", logger=None)
     monkeypatch.setattr(BuildContext, "usr_local", os.getcwd())
     cli.run("-ntmacos-arm64", f"-c{cfg}", "build", f.version)
     assert cli.succeeded
-    assert "Patched '/usr/local\\b' in build/components/cpython/Mac/Makefile.in" in cli.logged
     assert "Patched '/usr/local\\b' in build/components/cpython/setup.py" in cli.logged
     assert "Can't patch 'build/components/cpython/foo'" in cli.logged
     assert "isolate-usr-local: mount-shadow" in cli.logged
```

### Comparing `portable-python-1.6.5/tests/test_failed.py` & `portable-python-1.7.0/tests/test_failed.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/tests/test_inspector.py` & `portable-python-1.7.0/tests/test_inspector.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     runez.touch("foo/foo.so", logger=None)  # Folder not examined (looking only at known py subfolders)
     runez.touch("README.so.txt", logger=None)  # Not a dynamic lib
     runez.touch("lib-foo.a.1", logger=None)  # Not a lib
     x = sorted(str(x) for x in find_libs("."))
     assert x == ["lib-foo.a", "lp.dylib", "lp.so", "lp.so.1.0", "python3.9/config-3.9/libpython3.9.so"]
 
 
-def test_find_python(temp_folder):
+def test_inspect_python(temp_folder):
     PPG.grab_config("foo.yml")
     inspector = PythonInspector("invoker")
     assert str(inspector)
     assert str(inspector.module_info["_ctypes"])
     r = inspector.full_so_report
     assert r.ok
```

### Comparing `portable-python-1.6.5/tests/test_invoker.py` & `portable-python-1.7.0/tests/test_invoker.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/tests/test_list.py` & `portable-python-1.7.0/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/tests/test_prefix.py` & `portable-python-1.7.0/tests/test_prefix.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/tests/test_recompress.py` & `portable-python-1.7.0/tests/test_recompress.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.5/tests/test_setup.py` & `portable-python-1.7.0/tests/test_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,8 +61,8 @@
         _ = BuildSetup("3.9.6")
     assert "Invalid extension 'foo'" in logged.pop()
 
 
 def test_inspect(cli):
     cli.run("-n", "inspect", "foo", "-m+sys")
     assert cli.failed
-    assert "foo: not an executable" in cli.logged
+    assert "foo is not an executable" in cli.logged
```

