# Comparing `tmp/remote_ipykernel-1.0.tar.gz` & `tmp/remote_ipykernel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote_ipykernel-1.0.tar", last modified: Tue Jun 13 09:19:30 2023, max compression
+gzip compressed data, was "remote_ipykernel-1.0.1.tar", last modified: Tue Jun 13 09:39:37 2023, max compression
```

## Comparing `remote_ipykernel-1.0.tar` & `remote_ipykernel-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 09:19:30.455673 remote_ipykernel-1.0/
--rw-rw-rw-   0        0        0      243 2023-06-12 21:32:06.000000 remote_ipykernel-1.0/.gitignore
--rw-rw-rw-   0        0        0     1331 2023-06-12 21:39:03.000000 remote_ipykernel-1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 21:39:10.000000 remote_ipykernel-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6930 2023-06-13 09:19:30.455673 remote_ipykernel-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6426 2023-06-12 21:48:17.000000 remote_ipykernel-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 09:19:30.423665 remote_ipykernel-1.0/doc/
--rw-rw-rw-   0        0        0    13247 2023-06-12 15:25:19.000000 remote_ipykernel-1.0/doc/kernels.png
--rw-rw-rw-   0        0        0      745 2023-06-13 09:18:53.000000 remote_ipykernel-1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-13 09:19:30.430667 remote_ipykernel-1.0/remote_ipykernel/
--rw-rw-rw-   0        0        0      129 2023-06-12 15:25:19.000000 remote_ipykernel-1.0/remote_ipykernel/__init__.py
--rw-rw-rw-   0        0        0      482 2023-06-12 15:25:19.000000 remote_ipykernel-1.0/remote_ipykernel/__main__.py
--rw-rw-rw-   0        0        0      215 2023-06-12 22:00:10.000000 remote_ipykernel-1.0/remote_ipykernel/__version.py
--rw-rw-rw-   0        0        0      890 2023-06-12 15:25:19.000000 remote_ipykernel-1.0/remote_ipykernel/compat.py
--rw-rw-rw-   0        0        0    25045 2023-06-12 15:25:19.000000 remote_ipykernel-1.0/remote_ipykernel/kernel.py
--rw-rw-rw-   0        0        0    15608 2023-06-12 15:25:19.000000 remote_ipykernel-1.0/remote_ipykernel/manage.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:19:30.449671 remote_ipykernel-1.0/remote_ipykernel.egg-info/
--rw-rw-rw-   0        0        0     6930 2023-06-13 09:19:30.000000 remote_ipykernel-1.0/remote_ipykernel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      574 2023-06-13 09:19:30.000000 remote_ipykernel-1.0/remote_ipykernel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 09:19:30.000000 remote_ipykernel-1.0/remote_ipykernel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-13 09:19:30.000000 remote_ipykernel-1.0/remote_ipykernel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-13 09:19:30.000000 remote_ipykernel-1.0/remote_ipykernel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-13 09:19:30.000000 remote_ipykernel-1.0/remote_ipykernel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 09:19:30.455673 remote_ipykernel-1.0/setup.cfg
--rw-rw-rw-   0        0        0      191 2023-06-13 09:12:45.000000 remote_ipykernel-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:19:30.453672 remote_ipykernel-1.0/tests/
--rw-rw-rw-   0        0        0     3756 2023-06-13 09:14:04.000000 remote_ipykernel-1.0/tests/test_cli.py
--rw-rw-rw-   0        0        0     4176 2023-06-13 09:14:38.000000 remote_ipykernel-1.0/tests/test_command_fix.py
--rw-rw-rw-   0        0        0     1748 2023-06-13 09:14:55.000000 remote_ipykernel-1.0/tests/test_extract_uuid.py
--rw-rw-rw-   0        0        0      382 2023-06-12 15:25:19.000000 remote_ipykernel-1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-13 09:39:37.387745 remote_ipykernel-1.0.1/
+-rw-rw-rw-   0        0        0      243 2023-06-12 21:32:06.000000 remote_ipykernel-1.0.1/.gitignore
+-rw-rw-rw-   0        0        0     1331 2023-06-12 21:39:03.000000 remote_ipykernel-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       17 2023-06-12 21:39:10.000000 remote_ipykernel-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6877 2023-06-13 09:39:37.386745 remote_ipykernel-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6403 2023-06-13 09:31:41.000000 remote_ipykernel-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 09:39:37.350737 remote_ipykernel-1.0.1/doc/
+-rw-rw-rw-   0        0        0    13247 2023-06-12 15:25:19.000000 remote_ipykernel-1.0.1/doc/kernels.png
+-rw-rw-rw-   0        0        0      772 2023-06-13 09:38:58.000000 remote_ipykernel-1.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-13 09:39:37.356737 remote_ipykernel-1.0.1/remote_ipykernel/
+-rw-rw-rw-   0        0        0      129 2023-06-12 15:25:19.000000 remote_ipykernel-1.0.1/remote_ipykernel/__init__.py
+-rw-rw-rw-   0        0        0      215 2023-06-12 22:00:10.000000 remote_ipykernel-1.0.1/remote_ipykernel/__version.py
+-rw-rw-rw-   0        0        0      890 2023-06-12 15:25:19.000000 remote_ipykernel-1.0.1/remote_ipykernel/compat.py
+-rw-rw-rw-   0        0        0    25047 2023-06-13 09:25:32.000000 remote_ipykernel-1.0.1/remote_ipykernel/kernel.py
+-rw-rw-rw-   0        0        0    15527 2023-06-13 09:36:48.000000 remote_ipykernel-1.0.1/remote_ipykernel/manage.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:39:37.381743 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/
+-rw-rw-rw-   0        0        0     6877 2023-06-13 09:39:37.000000 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2023-06-13 09:39:37.000000 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:39:37.000000 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2023-06-13 09:39:37.000000 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-13 09:39:37.000000 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-13 09:39:37.000000 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 09:39:37.387745 remote_ipykernel-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      191 2023-06-13 09:12:45.000000 remote_ipykernel-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:39:37.385744 remote_ipykernel-1.0.1/tests/
+-rw-rw-rw-   0        0        0     3756 2023-06-13 09:14:04.000000 remote_ipykernel-1.0.1/tests/test_cli.py
+-rw-rw-rw-   0        0        0     4176 2023-06-13 09:14:38.000000 remote_ipykernel-1.0.1/tests/test_command_fix.py
+-rw-rw-rw-   0        0        0     1748 2023-06-13 09:14:55.000000 remote_ipykernel-1.0.1/tests/test_extract_uuid.py
+-rw-rw-rw-   0        0        0      382 2023-06-12 15:25:19.000000 remote_ipykernel-1.0.1/tox.ini
```

### Comparing `remote_ipykernel-1.0/LICENSE.txt` & `remote_ipykernel-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `remote_ipykernel-1.0/PKG-INFO` & `remote_ipykernel-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: remote_ipykernel
-Version: 1.0
-Summary: Running IPython kernels remotely and through batch queues
-Author: Conor Wills
-Author-email: Tom Daff <tdd20@cam.ac.uk>
-License: BSD
-Project-URL: Homepage, https://github.com/CWills96/remote_ipykernel
-Classifier: Programming Language :: Python :: 3
-Classifier: Framework :: IPython
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Remote IPyKernel
 
 All your Jupyter kernels, on all your machines, in one place.
 This is a fork of abandoned package `remote_ikernel` by Tom Daff <tdd20@cam.ac.uk>.
 
 Launch Jupyter kernels on remote systems and through batch queues so that
 they can be used within a local Jupyter noteboook.
@@ -56,55 +41,58 @@
 
    pip install remote_ipykernel
 ```
 
 ```bash
    # Set up the kernels you'd like to use
 
-   remote_ipykernel manage
+   remote_ipykernel
+
+   # Or
+   rkr
 ```
 
 ```bash
    # Add a new kernel running through GrideEngine
 
-   remote_ipykernel manage --add \
+   remote_ipykernel --add \
       --kernel_cmd="ipython kernel -f {connection_file}" \
       --name="Python 2.7" --cpus=2 --pe=smp --interface=sge
 ```
 
 ```bash
    # Add an SSH connection to a remote machine running IJulia
 
-   remote_ipykernel manage --add \
+   remote_ipykernel --add \
       --kernel_cmd="/home/me/julia-903644385b/bin/julia -i --startup-file=yes --color=yes /home/me/.julia/v0.6/IJulia/src/kernel.jl {connection_file}" \
       --name="IJulia 0.6.0" --interface=ssh \
       --host=me@remote.machine --workdir='/home/me/Workdir' --language=julia
 ```
 
 ```bash
    # Set up kernels for your local virtual environments that can be run
    # from a single notebook server.
 
-   remote_ipykernel manage --add \
+   remote_ipykernel --add \
       --kernel_cmd="/home/me/Virtualenvs/dev/bin/ipython kernel -f {connection_file}" \
       --name="Python 2 (venv:dev)" --interface=local
 ```
 
 ```bash
    # Connect to a SLURM cluster through a gateway machine (to get into a
    # local network) and cluster frontend machine (where the sqsub runs from).
 
-   remote_ipykernel manage --add \
+   remote_ipykernel --add \
       --kernel_cmd="ipython kernel -f {connection_file}" \
       --name="Python 2.7" --cpus=4 --interface=slurm \
       --tunnel-hosts gateway.machine cluster.frontend
 ```
 
 The kernel spec files will be installed so that the new kernel appears in
-the drop-down list in the notebook. ``remote_ipykernel manage`` also has options
+the drop-down list in the notebook. ``remote_ipykernel`` also has options
 to show and delete existing kernels.
 
 
 ## Connection multiplexing
 
 
 When working with remote machines, each kernel creates two ``ssh``
```

### Comparing `remote_ipykernel-1.0/README.md` & `remote_ipykernel-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: remote_ipykernel
+Version: 1.0.1
+Summary: Running IPython kernels remotely and through batch queues
+Author: Tom Daff, Conor Wills
+License: BSD
+Project-URL: Homepage, https://github.com/CWills96/remote_ipykernel
+Classifier: Programming Language :: Python :: 3
+Classifier: Framework :: IPython
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Remote IPyKernel
 
 All your Jupyter kernels, on all your machines, in one place.
 This is a fork of abandoned package `remote_ikernel` by Tom Daff <tdd20@cam.ac.uk>.
 
 Launch Jupyter kernels on remote systems and through batch queues so that
 they can be used within a local Jupyter noteboook.
@@ -41,55 +55,58 @@
 
    pip install remote_ipykernel
 ```
 
 ```bash
    # Set up the kernels you'd like to use
 
-   remote_ipykernel manage
+   remote_ipykernel
+
+   # Or
+   rkr
 ```
 
 ```bash
    # Add a new kernel running through GrideEngine
 
-   remote_ipykernel manage --add \
+   remote_ipykernel --add \
       --kernel_cmd="ipython kernel -f {connection_file}" \
       --name="Python 2.7" --cpus=2 --pe=smp --interface=sge
 ```
 
 ```bash
    # Add an SSH connection to a remote machine running IJulia
 
-   remote_ipykernel manage --add \
+   remote_ipykernel --add \
       --kernel_cmd="/home/me/julia-903644385b/bin/julia -i --startup-file=yes --color=yes /home/me/.julia/v0.6/IJulia/src/kernel.jl {connection_file}" \
       --name="IJulia 0.6.0" --interface=ssh \
       --host=me@remote.machine --workdir='/home/me/Workdir' --language=julia
 ```
 
 ```bash
    # Set up kernels for your local virtual environments that can be run
    # from a single notebook server.
 
-   remote_ipykernel manage --add \
+   remote_ipykernel --add \
       --kernel_cmd="/home/me/Virtualenvs/dev/bin/ipython kernel -f {connection_file}" \
       --name="Python 2 (venv:dev)" --interface=local
 ```
 
 ```bash
    # Connect to a SLURM cluster through a gateway machine (to get into a
    # local network) and cluster frontend machine (where the sqsub runs from).
 
-   remote_ipykernel manage --add \
+   remote_ipykernel --add \
       --kernel_cmd="ipython kernel -f {connection_file}" \
       --name="Python 2.7" --cpus=4 --interface=slurm \
       --tunnel-hosts gateway.machine cluster.frontend
 ```
 
 The kernel spec files will be installed so that the new kernel appears in
-the drop-down list in the notebook. ``remote_ipykernel manage`` also has options
+the drop-down list in the notebook. ``remote_ipykernel`` also has options
 to show and delete existing kernels.
 
 
 ## Connection multiplexing
 
 
 When working with remote machines, each kernel creates two ``ssh``
```

### Comparing `remote_ipykernel-1.0/doc/kernels.png` & `remote_ipykernel-1.0.1/doc/kernels.png`

 * *Files identical despite different names*

### Comparing `remote_ipykernel-1.0/pyproject.toml` & `remote_ipykernel-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "remote_ipykernel"
-version = "1.0"
+version = "1.0.1"
 description = "Running IPython kernels remotely and through batch queues"
 authors = [
-    { name = "Tom Daff", email = "tdd20@cam.ac.uk" },
+    { name = "Tom Daff"},
     { name = "Conor Wills"}
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "BSD"}
 classifiers = [
     'Programming Language :: Python :: 3',
@@ -24,8 +24,9 @@
     'tornado>=4'
 ]
 
 [project.urls]
 Homepage = "https://github.com/CWills96/remote_ipykernel"
 
 [project.scripts]
-rkr = "remote_ipykernel.manage:manage"
+rkr = "remote_ipykernel.manage:manage"
+remote_ipykernel = "remote_ipykernel.manage:manage"
```

### Comparing `remote_ipykernel-1.0/remote_ipykernel/compat.py` & `remote_ipykernel-1.0.1/remote_ipykernel/compat.py`

 * *Files identical despite different names*

### Comparing `remote_ipykernel-1.0/remote_ipykernel/kernel.py` & `remote_ipykernel-1.0.1/remote_ipykernel/kernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     class pexpect_spawn(PopenSpawn):
         def isalive(self):
             return self.proc.poll() is None
 
 
 from tornado.log import LogFormatter
 
-from remote_ikernel import RIK_PREFIX, __version__
+from remote_ipykernel import RIK_PREFIX, __version__
 
 
 # All the ports that need to be forwarded
 PORT_NAMES = ["hb_port", "shell_port", "iopub_port", "stdin_port", "control_port"]
 
 # Blend in with the notebook logging
 _LOG_FMT = (
```

### Comparing `remote_ipykernel-1.0/remote_ipykernel/manage.py` & `remote_ipykernel-1.0.1/remote_ipykernel/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 import re
 import shlex
 import sys
 from os import path
 from subprocess import list2cmdline
 
 # How we identify kernels that rik will manage
-from remote_ikernel import RIK_PREFIX, __version__
+from remote_ipykernel import RIK_PREFIX, __version__
 
 # These go through a compatibility layer to work with IPython and Jupyter
-from remote_ikernel.compat import kernelspec as ks
-from remote_ikernel.compat import tempdir
+from remote_ipykernel.compat import kernelspec as ks
+from remote_ipykernel.compat import tempdir
 
 # When Python 2 pipes into something else, there is no encoding
 # set. Assume that it is utf-8 so that scripttest works as expected.
 # If LANG=C, unicode characters will break output, but
 # https://bugs.python.org/issue19846 says it should not be an issue
 # on modern systems. And you can't put unicode in with LANG=C so how can
 # you expect unicode out?
@@ -423,16 +423,14 @@
     raw_args = sys.argv[1:]
     # give argparse something unicode to deal with for PY2
     # otherwise, ignore if there is nothing to 'decode'
     try:
         raw_args = [x.decode("UTF-8") for x in sys.argv[1:]]
     except AttributeError:
         pass
-    # Remove 'manage' to parse manage specific options
-    raw_args.remove("manage")
     args = parser.parse_args(raw_args)
 
     if args.add:
         kernel_name, display_name = add_kernel(
             args.interface,
             args.name,
             args.kernel_cmd,
```

### Comparing `remote_ipykernel-1.0/remote_ipykernel.egg-info/PKG-INFO` & `remote_ipykernel-1.0.1/remote_ipykernel.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: remote-ipykernel
-Version: 1.0
+Version: 1.0.1
 Summary: Running IPython kernels remotely and through batch queues
-Author: Conor Wills
-Author-email: Tom Daff <tdd20@cam.ac.uk>
+Author: Tom Daff, Conor Wills
 License: BSD
 Project-URL: Homepage, https://github.com/CWills96/remote_ipykernel
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: IPython
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -56,55 +55,58 @@
 
    pip install remote_ipykernel
 ```
 
 ```bash
    # Set up the kernels you'd like to use
 
-   remote_ipykernel manage
+   remote_ipykernel
+
+   # Or
+   rkr
 ```
 
 ```bash
    # Add a new kernel running through GrideEngine
 
-   remote_ipykernel manage --add \
+   remote_ipykernel --add \
       --kernel_cmd="ipython kernel -f {connection_file}" \
       --name="Python 2.7" --cpus=2 --pe=smp --interface=sge
 ```
 
 ```bash
    # Add an SSH connection to a remote machine running IJulia
 
-   remote_ipykernel manage --add \
+   remote_ipykernel --add \
       --kernel_cmd="/home/me/julia-903644385b/bin/julia -i --startup-file=yes --color=yes /home/me/.julia/v0.6/IJulia/src/kernel.jl {connection_file}" \
       --name="IJulia 0.6.0" --interface=ssh \
       --host=me@remote.machine --workdir='/home/me/Workdir' --language=julia
 ```
 
 ```bash
    # Set up kernels for your local virtual environments that can be run
    # from a single notebook server.
 
-   remote_ipykernel manage --add \
+   remote_ipykernel --add \
       --kernel_cmd="/home/me/Virtualenvs/dev/bin/ipython kernel -f {connection_file}" \
       --name="Python 2 (venv:dev)" --interface=local
 ```
 
 ```bash
    # Connect to a SLURM cluster through a gateway machine (to get into a
    # local network) and cluster frontend machine (where the sqsub runs from).
 
-   remote_ipykernel manage --add \
+   remote_ipykernel --add \
       --kernel_cmd="ipython kernel -f {connection_file}" \
       --name="Python 2.7" --cpus=4 --interface=slurm \
       --tunnel-hosts gateway.machine cluster.frontend
 ```
 
 The kernel spec files will be installed so that the new kernel appears in
-the drop-down list in the notebook. ``remote_ipykernel manage`` also has options
+the drop-down list in the notebook. ``remote_ipykernel`` also has options
 to show and delete existing kernels.
 
 
 ## Connection multiplexing
 
 
 When working with remote machines, each kernel creates two ``ssh``
```

### Comparing `remote_ipykernel-1.0/tests/test_cli.py` & `remote_ipykernel-1.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `remote_ipykernel-1.0/tests/test_command_fix.py` & `remote_ipykernel-1.0.1/tests/test_command_fix.py`

 * *Files identical despite different names*

### Comparing `remote_ipykernel-1.0/tests/test_extract_uuid.py` & `remote_ipykernel-1.0.1/tests/test_extract_uuid.py`

 * *Files identical despite different names*

