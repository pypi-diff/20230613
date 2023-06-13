# Comparing `tmp/remote_ipykernel-1.0.1.tar.gz` & `tmp/remote_ipykernel-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote_ipykernel-1.0.1.tar", last modified: Tue Jun 13 09:39:37 2023, max compression
+gzip compressed data, was "remote_ipykernel-1.0.2.tar", last modified: Tue Jun 13 16:44:11 2023, max compression
```

## Comparing `remote_ipykernel-1.0.1.tar` & `remote_ipykernel-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 09:39:37.387745 remote_ipykernel-1.0.1/
--rw-rw-rw-   0        0        0      243 2023-06-12 21:32:06.000000 remote_ipykernel-1.0.1/.gitignore
--rw-rw-rw-   0        0        0     1331 2023-06-12 21:39:03.000000 remote_ipykernel-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 21:39:10.000000 remote_ipykernel-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6877 2023-06-13 09:39:37.386745 remote_ipykernel-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6403 2023-06-13 09:31:41.000000 remote_ipykernel-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 09:39:37.350737 remote_ipykernel-1.0.1/doc/
--rw-rw-rw-   0        0        0    13247 2023-06-12 15:25:19.000000 remote_ipykernel-1.0.1/doc/kernels.png
--rw-rw-rw-   0        0        0      772 2023-06-13 09:38:58.000000 remote_ipykernel-1.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-13 09:39:37.356737 remote_ipykernel-1.0.1/remote_ipykernel/
--rw-rw-rw-   0        0        0      129 2023-06-12 15:25:19.000000 remote_ipykernel-1.0.1/remote_ipykernel/__init__.py
--rw-rw-rw-   0        0        0      215 2023-06-12 22:00:10.000000 remote_ipykernel-1.0.1/remote_ipykernel/__version.py
--rw-rw-rw-   0        0        0      890 2023-06-12 15:25:19.000000 remote_ipykernel-1.0.1/remote_ipykernel/compat.py
--rw-rw-rw-   0        0        0    25047 2023-06-13 09:25:32.000000 remote_ipykernel-1.0.1/remote_ipykernel/kernel.py
--rw-rw-rw-   0        0        0    15527 2023-06-13 09:36:48.000000 remote_ipykernel-1.0.1/remote_ipykernel/manage.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:39:37.381743 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/
--rw-rw-rw-   0        0        0     6877 2023-06-13 09:39:37.000000 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-06-13 09:39:37.000000 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 09:39:37.000000 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2023-06-13 09:39:37.000000 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-13 09:39:37.000000 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-13 09:39:37.000000 remote_ipykernel-1.0.1/remote_ipykernel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 09:39:37.387745 remote_ipykernel-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      191 2023-06-13 09:12:45.000000 remote_ipykernel-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:39:37.385744 remote_ipykernel-1.0.1/tests/
--rw-rw-rw-   0        0        0     3756 2023-06-13 09:14:04.000000 remote_ipykernel-1.0.1/tests/test_cli.py
--rw-rw-rw-   0        0        0     4176 2023-06-13 09:14:38.000000 remote_ipykernel-1.0.1/tests/test_command_fix.py
--rw-rw-rw-   0        0        0     1748 2023-06-13 09:14:55.000000 remote_ipykernel-1.0.1/tests/test_extract_uuid.py
--rw-rw-rw-   0        0        0      382 2023-06-12 15:25:19.000000 remote_ipykernel-1.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:44:11.680328 remote_ipykernel-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-13 16:44:11.680328 remote_ipykernel-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:44:11.680328 remote_ipykernel-1.0.2/remote_ipykernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/remote_ipykernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/remote_ipykernel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/remote_ipykernel/__version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/remote_ipykernel/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24321 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/remote_ipykernel/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/remote_ipykernel/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:44:11.680328 remote_ipykernel-1.0.2/remote_ipykernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-13 16:44:11.000000 remote_ipykernel-1.0.2/remote_ipykernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-13 16:44:11.000000 remote_ipykernel-1.0.2/remote_ipykernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:44:11.000000 remote_ipykernel-1.0.2/remote_ipykernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-13 16:44:11.000000 remote_ipykernel-1.0.2/remote_ipykernel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-13 16:44:11.000000 remote_ipykernel-1.0.2/remote_ipykernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 16:44:11.000000 remote_ipykernel-1.0.2/remote_ipykernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:44:11.680328 remote_ipykernel-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:44:11.680328 remote_ipykernel-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/tests/test_command_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-13 16:43:59.000000 remote_ipykernel-1.0.2/tests/test_extract_uuid.py
```

### Comparing `remote_ipykernel-1.0.1/LICENSE.txt` & `remote_ipykernel-1.0.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Copyright (c) 2015 Tom Daff, 2023 Conor Wills
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Copyright (c) 2015 Tom Daff, 2023 Conor Wills
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `remote_ipykernel-1.0.1/PKG-INFO` & `remote_ipykernel-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-Metadata-Version: 2.1
-Name: remote_ipykernel
-Version: 1.0.1
-Summary: Running IPython kernels remotely and through batch queues
-Author: Tom Daff, Conor Wills
-License: BSD
-Project-URL: Homepage, https://github.com/CWills96/remote_ipykernel
-Classifier: Programming Language :: Python :: 3
-Classifier: Framework :: IPython
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Remote IPyKernel
-
-All your Jupyter kernels, on all your machines, in one place.
-This is a fork of abandoned package `remote_ikernel` by Tom Daff <tdd20@cam.ac.uk>.
-
-Launch Jupyter kernels on remote systems and through batch queues so that
-they can be used within a local Jupyter noteboook.
-
-![kernel image](doc/kernels.png "Kernel Dropdown")
-
-Jupyter compatible Kernels start through interactive jobs in batch queue
-systems (SGE, SLURM, PBS...) or through SSH connections. Once the kernel is
-started, SSH tunnels are created for the communication ports are so the
-notebook can talk to the kernel as if it was local.
-
-Commands for managing the kernels are included. It is also possible to use
-`remote_ipykernel` to manage kernels from different virtual environments or
-different python implementations.
-
-Install with `pip install remote_ipykernel`. Requires `notebook` (as part
-of Jupyter), version 4.0 or greater and `pexpect`. Passwordless `ssh`
-to the all the remote machines is also recommended (e.g. nodes on a cluster).
-
-**Warning**
-
-   ``remote_ipykernel`` opens multiple connections across several machines
-   to tunnel communication ports. If you have concerns about security or
-   excessive use of resources, please consult your systems administrator
-   before using this software.
-
-**Note**
-
-   When running kernels on remote machines, the notebooks themselves will
-   be saved onto the local filesystem, but the kernel will only have access
-   to filesystem of the remote machine running the kernel. If you need shared
-   directories, set up ``sshfs`` between your machines.
-
-
-```bash
-   # Install the module ('python setup.py install' also works)
-
-   pip install remote_ipykernel
-```
-
-```bash
-   # Set up the kernels you'd like to use
-
-   remote_ipykernel
-
-   # Or
-   rkr
-```
-
-```bash
-   # Add a new kernel running through GrideEngine
-
-   remote_ipykernel --add \
-      --kernel_cmd="ipython kernel -f {connection_file}" \
-      --name="Python 2.7" --cpus=2 --pe=smp --interface=sge
-```
-
-```bash
-   # Add an SSH connection to a remote machine running IJulia
-
-   remote_ipykernel --add \
-      --kernel_cmd="/home/me/julia-903644385b/bin/julia -i --startup-file=yes --color=yes /home/me/.julia/v0.6/IJulia/src/kernel.jl {connection_file}" \
-      --name="IJulia 0.6.0" --interface=ssh \
-      --host=me@remote.machine --workdir='/home/me/Workdir' --language=julia
-```
-
-```bash
-   # Set up kernels for your local virtual environments that can be run
-   # from a single notebook server.
-
-   remote_ipykernel --add \
-      --kernel_cmd="/home/me/Virtualenvs/dev/bin/ipython kernel -f {connection_file}" \
-      --name="Python 2 (venv:dev)" --interface=local
-```
-
-```bash
-   # Connect to a SLURM cluster through a gateway machine (to get into a
-   # local network) and cluster frontend machine (where the sqsub runs from).
-
-   remote_ipykernel --add \
-      --kernel_cmd="ipython kernel -f {connection_file}" \
-      --name="Python 2.7" --cpus=4 --interface=slurm \
-      --tunnel-hosts gateway.machine cluster.frontend
-```
-
-The kernel spec files will be installed so that the new kernel appears in
-the drop-down list in the notebook. ``remote_ipykernel`` also has options
-to show and delete existing kernels.
-
-
-## Connection multiplexing
-
-
-When working with remote machines, each kernel creates two ``ssh``
-connections. If you would like to reduce that, you can set up automatic
-multiplexing of connections. For each machine, add a configuration to your
-``~/.ssh/config``:
-
-```shell
-   Host myhost.ac.uk
-       ControlMaster auto
-       ControlPath ~/.ssh/%r@%h:%p
-       ControlPersist 1
-```
-
-This will create a master connection that remains in the background when and
-multiplex everything through that. If you have multiple hops, this will need
-to be added for each hop. Note, for the security conscious, that idle kernels
-on multiplexed connections allow new ssh connections to be started without a
-password.
-
-Changes for v1.0
-================
-
-  * Setup updates and code usability tweaks
-
-Changes for v0.4
-================
-
-  * Option ``--tunnel-hosts``. When given, the software will try to create
-    an ssh tunnel through all the hosts before starting the final connection.
-    Allows using batch queues on remote systems.
-  * Preliminary support for dealing with passwords. If a program is defined
-    in the environment variable ``SSH_ASKPASS`` it will be used
-    to ask the user for a password.
-  * ``--launch-cmd`` can be used to override the command used to launch the
-    interactive jobs on the cluster, e.g. to replace ``qlogin`` with ``qrsh``.
-  * Platform LSF support.
-  * The kernel json files are given unique names.
-
-Changes for v0.3
-================
-
-  * Updated pip requirements to pull in the `notebook` package. Use an earlier
-    version if you need to use IPython 3.
-  * Remote process is polled for output which will show up when ``--verbose``
-    if used as a kernel option.
-
-Changes for v0.2
-================
-
-  * Version 0.2.11 is the last version to support IPython notebook version 3.
-    `pip` requirements enforce versions less than 4. Use a more recent version
-    to ensure compatibility with the Jupyter split.
-  * Support for PBS/Torque through ``qsub -I``.
-  * Tunnels are kept alive better, if something is not responding try waiting
-    20 seconds to see if a tunnel had dies. (Tunnels no longer depend on pyzmq,
-    instead they are launched through pexpect and monitored until they die.)
-  * ``--remote-launch-args`` can be used to set ``qlogin`` parameters or similar.
-  * ``--remote-precmd`` allows execution of an extra command on the remote host
-    before launching a kernel.
-  * Better compatibility with Python 3.
-  * Kernel output on terminals with ``--verbose`` option for debugging.
-  * Connect to a host with ssh, slurm, or local kernels.
-  * Changed prefix to ``rik_``.
-  * kernel_cmd now requires the ``{connection_file}`` argument.
-  * ``remote_ikernel manage --show`` command to show existing kernels.
-  * Specify the working directory on the remote machine with ``--workdir``.
-  * ``kernel-uuid.json`` is copied to the working director for systems where
-    there is no access to the frontend filesystem.
-  * Added compatibility layer to get rid of Jupyter warnings.
+Metadata-Version: 2.1
+Name: remote_ipykernel
+Version: 1.0.2
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
+# Remote IPyKernel
+
+All your Jupyter kernels, on all your machines, in one place.
+This is a fork of abandoned package `remote_ikernel` by Tom Daff <tdd20@cam.ac.uk>.
+
+Launch Jupyter kernels on remote systems and through batch queues so that
+they can be used within a local Jupyter noteboook.
+
+![kernel image](doc/kernels.png "Kernel Dropdown")
+
+Jupyter compatible Kernels start through interactive jobs in batch queue
+systems (SGE, SLURM, PBS...) or through SSH connections. Once the kernel is
+started, SSH tunnels are created for the communication ports are so the
+notebook can talk to the kernel as if it was local.
+
+Commands for managing the kernels are included. It is also possible to use
+`remote_ipykernel` to manage kernels from different virtual environments or
+different python implementations.
+
+Install with `pip install remote_ipykernel`. Requires `notebook` (as part
+of Jupyter), version 4.0 or greater and `pexpect`. Passwordless `ssh`
+to the all the remote machines is also recommended (e.g. nodes on a cluster).
+
+**Warning**
+
+   ``remote_ipykernel`` opens multiple connections across several machines
+   to tunnel communication ports. If you have concerns about security or
+   excessive use of resources, please consult your systems administrator
+   before using this software.
+
+**Note**
+
+   When running kernels on remote machines, the notebooks themselves will
+   be saved onto the local filesystem, but the kernel will only have access
+   to filesystem of the remote machine running the kernel. If you need shared
+   directories, set up ``sshfs`` between your machines.
+
+
+```bash
+   # Install the module ('python setup.py install' also works)
+
+   pip install remote_ipykernel
+```
+
+```bash
+   # Set up the kernels you'd like to use
+
+   remote_ipykernel
+
+   # Or
+   rkr
+```
+
+```bash
+   # Add a new kernel running through GrideEngine
+
+   remote_ipykernel --add \
+      --kernel_cmd="ipython kernel -f {connection_file}" \
+      --name="Python 2.7" --cpus=2 --pe=smp --interface=sge
+```
+
+```bash
+   # Add an SSH connection to a remote machine running IJulia
+
+   remote_ipykernel --add \
+      --kernel_cmd="/home/me/julia-903644385b/bin/julia -i --startup-file=yes --color=yes /home/me/.julia/v0.6/IJulia/src/kernel.jl {connection_file}" \
+      --name="IJulia 0.6.0" --interface=ssh \
+      --host=me@remote.machine --workdir='/home/me/Workdir' --language=julia
+```
+
+```bash
+   # Set up kernels for your local virtual environments that can be run
+   # from a single notebook server.
+
+   remote_ipykernel --add \
+      --kernel_cmd="/home/me/Virtualenvs/dev/bin/ipython kernel -f {connection_file}" \
+      --name="Python 2 (venv:dev)" --interface=local
+```
+
+```bash
+   # Connect to a SLURM cluster through a gateway machine (to get into a
+   # local network) and cluster frontend machine (where the sqsub runs from).
+
+   remote_ipykernel --add \
+      --kernel_cmd="ipython kernel -f {connection_file}" \
+      --name="Python 2.7" --cpus=4 --interface=slurm \
+      --tunnel-hosts gateway.machine cluster.frontend
+```
+
+The kernel spec files will be installed so that the new kernel appears in
+the drop-down list in the notebook. ``remote_ipykernel`` also has options
+to show and delete existing kernels.
+
+
+## Connection multiplexing
+
+
+When working with remote machines, each kernel creates two ``ssh``
+connections. If you would like to reduce that, you can set up automatic
+multiplexing of connections. For each machine, add a configuration to your
+``~/.ssh/config``:
+
+```shell
+   Host myhost.ac.uk
+       ControlMaster auto
+       ControlPath ~/.ssh/%r@%h:%p
+       ControlPersist 1
+```
+
+This will create a master connection that remains in the background when and
+multiplex everything through that. If you have multiple hops, this will need
+to be added for each hop. Note, for the security conscious, that idle kernels
+on multiplexed connections allow new ssh connections to be started without a
+password.
+
+Changes for v1.0
+================
+
+  * Setup updates and code usability tweaks
+
+Changes for v0.4
+================
+
+  * Option ``--tunnel-hosts``. When given, the software will try to create
+    an ssh tunnel through all the hosts before starting the final connection.
+    Allows using batch queues on remote systems.
+  * Preliminary support for dealing with passwords. If a program is defined
+    in the environment variable ``SSH_ASKPASS`` it will be used
+    to ask the user for a password.
+  * ``--launch-cmd`` can be used to override the command used to launch the
+    interactive jobs on the cluster, e.g. to replace ``qlogin`` with ``qrsh``.
+  * Platform LSF support.
+  * The kernel json files are given unique names.
+
+Changes for v0.3
+================
+
+  * Updated pip requirements to pull in the `notebook` package. Use an earlier
+    version if you need to use IPython 3.
+  * Remote process is polled for output which will show up when ``--verbose``
+    if used as a kernel option.
+
+Changes for v0.2
+================
+
+  * Version 0.2.11 is the last version to support IPython notebook version 3.
+    `pip` requirements enforce versions less than 4. Use a more recent version
+    to ensure compatibility with the Jupyter split.
+  * Support for PBS/Torque through ``qsub -I``.
+  * Tunnels are kept alive better, if something is not responding try waiting
+    20 seconds to see if a tunnel had dies. (Tunnels no longer depend on pyzmq,
+    instead they are launched through pexpect and monitored until they die.)
+  * ``--remote-launch-args`` can be used to set ``qlogin`` parameters or similar.
+  * ``--remote-precmd`` allows execution of an extra command on the remote host
+    before launching a kernel.
+  * Better compatibility with Python 3.
+  * Kernel output on terminals with ``--verbose`` option for debugging.
+  * Connect to a host with ssh, slurm, or local kernels.
+  * Changed prefix to ``rik_``.
+  * kernel_cmd now requires the ``{connection_file}`` argument.
+  * ``remote_ikernel manage --show`` command to show existing kernels.
+  * Specify the working directory on the remote machine with ``--workdir``.
+  * ``kernel-uuid.json`` is copied to the working director for systems where
+    there is no access to the frontend filesystem.
+  * Added compatibility layer to get rid of Jupyter warnings.
```

### Comparing `remote_ipykernel-1.0.1/README.md` & `remote_ipykernel-1.0.2/remote_ipykernel.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,165 +1,179 @@
-# Remote IPyKernel
-
-All your Jupyter kernels, on all your machines, in one place.
-This is a fork of abandoned package `remote_ikernel` by Tom Daff <tdd20@cam.ac.uk>.
-
-Launch Jupyter kernels on remote systems and through batch queues so that
-they can be used within a local Jupyter noteboook.
-
-![kernel image](doc/kernels.png "Kernel Dropdown")
-
-Jupyter compatible Kernels start through interactive jobs in batch queue
-systems (SGE, SLURM, PBS...) or through SSH connections. Once the kernel is
-started, SSH tunnels are created for the communication ports are so the
-notebook can talk to the kernel as if it was local.
-
-Commands for managing the kernels are included. It is also possible to use
-`remote_ipykernel` to manage kernels from different virtual environments or
-different python implementations.
-
-Install with `pip install remote_ipykernel`. Requires `notebook` (as part
-of Jupyter), version 4.0 or greater and `pexpect`. Passwordless `ssh`
-to the all the remote machines is also recommended (e.g. nodes on a cluster).
-
-**Warning**
-
-   ``remote_ipykernel`` opens multiple connections across several machines
-   to tunnel communication ports. If you have concerns about security or
-   excessive use of resources, please consult your systems administrator
-   before using this software.
-
-**Note**
-
-   When running kernels on remote machines, the notebooks themselves will
-   be saved onto the local filesystem, but the kernel will only have access
-   to filesystem of the remote machine running the kernel. If you need shared
-   directories, set up ``sshfs`` between your machines.
-
-
-```bash
-   # Install the module ('python setup.py install' also works)
-
-   pip install remote_ipykernel
-```
-
-```bash
-   # Set up the kernels you'd like to use
-
-   remote_ipykernel
-
-   # Or
-   rkr
-```
-
-```bash
-   # Add a new kernel running through GrideEngine
-
-   remote_ipykernel --add \
-      --kernel_cmd="ipython kernel -f {connection_file}" \
-      --name="Python 2.7" --cpus=2 --pe=smp --interface=sge
-```
-
-```bash
-   # Add an SSH connection to a remote machine running IJulia
-
-   remote_ipykernel --add \
-      --kernel_cmd="/home/me/julia-903644385b/bin/julia -i --startup-file=yes --color=yes /home/me/.julia/v0.6/IJulia/src/kernel.jl {connection_file}" \
-      --name="IJulia 0.6.0" --interface=ssh \
-      --host=me@remote.machine --workdir='/home/me/Workdir' --language=julia
-```
-
-```bash
-   # Set up kernels for your local virtual environments that can be run
-   # from a single notebook server.
-
-   remote_ipykernel --add \
-      --kernel_cmd="/home/me/Virtualenvs/dev/bin/ipython kernel -f {connection_file}" \
-      --name="Python 2 (venv:dev)" --interface=local
-```
-
-```bash
-   # Connect to a SLURM cluster through a gateway machine (to get into a
-   # local network) and cluster frontend machine (where the sqsub runs from).
-
-   remote_ipykernel --add \
-      --kernel_cmd="ipython kernel -f {connection_file}" \
-      --name="Python 2.7" --cpus=4 --interface=slurm \
-      --tunnel-hosts gateway.machine cluster.frontend
-```
-
-The kernel spec files will be installed so that the new kernel appears in
-the drop-down list in the notebook. ``remote_ipykernel`` also has options
-to show and delete existing kernels.
-
-
-## Connection multiplexing
-
-
-When working with remote machines, each kernel creates two ``ssh``
-connections. If you would like to reduce that, you can set up automatic
-multiplexing of connections. For each machine, add a configuration to your
-``~/.ssh/config``:
-
-```shell
-   Host myhost.ac.uk
-       ControlMaster auto
-       ControlPath ~/.ssh/%r@%h:%p
-       ControlPersist 1
-```
-
-This will create a master connection that remains in the background when and
-multiplex everything through that. If you have multiple hops, this will need
-to be added for each hop. Note, for the security conscious, that idle kernels
-on multiplexed connections allow new ssh connections to be started without a
-password.
-
-Changes for v1.0
-================
-
-  * Setup updates and code usability tweaks
-
-Changes for v0.4
-================
-
-  * Option ``--tunnel-hosts``. When given, the software will try to create
-    an ssh tunnel through all the hosts before starting the final connection.
-    Allows using batch queues on remote systems.
-  * Preliminary support for dealing with passwords. If a program is defined
-    in the environment variable ``SSH_ASKPASS`` it will be used
-    to ask the user for a password.
-  * ``--launch-cmd`` can be used to override the command used to launch the
-    interactive jobs on the cluster, e.g. to replace ``qlogin`` with ``qrsh``.
-  * Platform LSF support.
-  * The kernel json files are given unique names.
-
-Changes for v0.3
-================
-
-  * Updated pip requirements to pull in the `notebook` package. Use an earlier
-    version if you need to use IPython 3.
-  * Remote process is polled for output which will show up when ``--verbose``
-    if used as a kernel option.
-
-Changes for v0.2
-================
-
-  * Version 0.2.11 is the last version to support IPython notebook version 3.
-    `pip` requirements enforce versions less than 4. Use a more recent version
-    to ensure compatibility with the Jupyter split.
-  * Support for PBS/Torque through ``qsub -I``.
-  * Tunnels are kept alive better, if something is not responding try waiting
-    20 seconds to see if a tunnel had dies. (Tunnels no longer depend on pyzmq,
-    instead they are launched through pexpect and monitored until they die.)
-  * ``--remote-launch-args`` can be used to set ``qlogin`` parameters or similar.
-  * ``--remote-precmd`` allows execution of an extra command on the remote host
-    before launching a kernel.
-  * Better compatibility with Python 3.
-  * Kernel output on terminals with ``--verbose`` option for debugging.
-  * Connect to a host with ssh, slurm, or local kernels.
-  * Changed prefix to ``rik_``.
-  * kernel_cmd now requires the ``{connection_file}`` argument.
-  * ``remote_ikernel manage --show`` command to show existing kernels.
-  * Specify the working directory on the remote machine with ``--workdir``.
-  * ``kernel-uuid.json`` is copied to the working director for systems where
-    there is no access to the frontend filesystem.
-  * Added compatibility layer to get rid of Jupyter warnings.
+Metadata-Version: 2.1
+Name: remote-ipykernel
+Version: 1.0.2
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
+# Remote IPyKernel
+
+All your Jupyter kernels, on all your machines, in one place.
+This is a fork of abandoned package `remote_ikernel` by Tom Daff <tdd20@cam.ac.uk>.
+
+Launch Jupyter kernels on remote systems and through batch queues so that
+they can be used within a local Jupyter noteboook.
+
+![kernel image](doc/kernels.png "Kernel Dropdown")
+
+Jupyter compatible Kernels start through interactive jobs in batch queue
+systems (SGE, SLURM, PBS...) or through SSH connections. Once the kernel is
+started, SSH tunnels are created for the communication ports are so the
+notebook can talk to the kernel as if it was local.
+
+Commands for managing the kernels are included. It is also possible to use
+`remote_ipykernel` to manage kernels from different virtual environments or
+different python implementations.
+
+Install with `pip install remote_ipykernel`. Requires `notebook` (as part
+of Jupyter), version 4.0 or greater and `pexpect`. Passwordless `ssh`
+to the all the remote machines is also recommended (e.g. nodes on a cluster).
+
+**Warning**
+
+   ``remote_ipykernel`` opens multiple connections across several machines
+   to tunnel communication ports. If you have concerns about security or
+   excessive use of resources, please consult your systems administrator
+   before using this software.
+
+**Note**
+
+   When running kernels on remote machines, the notebooks themselves will
+   be saved onto the local filesystem, but the kernel will only have access
+   to filesystem of the remote machine running the kernel. If you need shared
+   directories, set up ``sshfs`` between your machines.
+
+
+```bash
+   # Install the module ('python setup.py install' also works)
+
+   pip install remote_ipykernel
+```
+
+```bash
+   # Set up the kernels you'd like to use
+
+   remote_ipykernel
+
+   # Or
+   rkr
+```
+
+```bash
+   # Add a new kernel running through GrideEngine
+
+   remote_ipykernel --add \
+      --kernel_cmd="ipython kernel -f {connection_file}" \
+      --name="Python 2.7" --cpus=2 --pe=smp --interface=sge
+```
+
+```bash
+   # Add an SSH connection to a remote machine running IJulia
+
+   remote_ipykernel --add \
+      --kernel_cmd="/home/me/julia-903644385b/bin/julia -i --startup-file=yes --color=yes /home/me/.julia/v0.6/IJulia/src/kernel.jl {connection_file}" \
+      --name="IJulia 0.6.0" --interface=ssh \
+      --host=me@remote.machine --workdir='/home/me/Workdir' --language=julia
+```
+
+```bash
+   # Set up kernels for your local virtual environments that can be run
+   # from a single notebook server.
+
+   remote_ipykernel --add \
+      --kernel_cmd="/home/me/Virtualenvs/dev/bin/ipython kernel -f {connection_file}" \
+      --name="Python 2 (venv:dev)" --interface=local
+```
+
+```bash
+   # Connect to a SLURM cluster through a gateway machine (to get into a
+   # local network) and cluster frontend machine (where the sqsub runs from).
+
+   remote_ipykernel --add \
+      --kernel_cmd="ipython kernel -f {connection_file}" \
+      --name="Python 2.7" --cpus=4 --interface=slurm \
+      --tunnel-hosts gateway.machine cluster.frontend
+```
+
+The kernel spec files will be installed so that the new kernel appears in
+the drop-down list in the notebook. ``remote_ipykernel`` also has options
+to show and delete existing kernels.
+
+
+## Connection multiplexing
+
+
+When working with remote machines, each kernel creates two ``ssh``
+connections. If you would like to reduce that, you can set up automatic
+multiplexing of connections. For each machine, add a configuration to your
+``~/.ssh/config``:
+
+```shell
+   Host myhost.ac.uk
+       ControlMaster auto
+       ControlPath ~/.ssh/%r@%h:%p
+       ControlPersist 1
+```
+
+This will create a master connection that remains in the background when and
+multiplex everything through that. If you have multiple hops, this will need
+to be added for each hop. Note, for the security conscious, that idle kernels
+on multiplexed connections allow new ssh connections to be started without a
+password.
+
+Changes for v1.0
+================
+
+  * Setup updates and code usability tweaks
+
+Changes for v0.4
+================
+
+  * Option ``--tunnel-hosts``. When given, the software will try to create
+    an ssh tunnel through all the hosts before starting the final connection.
+    Allows using batch queues on remote systems.
+  * Preliminary support for dealing with passwords. If a program is defined
+    in the environment variable ``SSH_ASKPASS`` it will be used
+    to ask the user for a password.
+  * ``--launch-cmd`` can be used to override the command used to launch the
+    interactive jobs on the cluster, e.g. to replace ``qlogin`` with ``qrsh``.
+  * Platform LSF support.
+  * The kernel json files are given unique names.
+
+Changes for v0.3
+================
+
+  * Updated pip requirements to pull in the `notebook` package. Use an earlier
+    version if you need to use IPython 3.
+  * Remote process is polled for output which will show up when ``--verbose``
+    if used as a kernel option.
+
+Changes for v0.2
+================
+
+  * Version 0.2.11 is the last version to support IPython notebook version 3.
+    `pip` requirements enforce versions less than 4. Use a more recent version
+    to ensure compatibility with the Jupyter split.
+  * Support for PBS/Torque through ``qsub -I``.
+  * Tunnels are kept alive better, if something is not responding try waiting
+    20 seconds to see if a tunnel had dies. (Tunnels no longer depend on pyzmq,
+    instead they are launched through pexpect and monitored until they die.)
+  * ``--remote-launch-args`` can be used to set ``qlogin`` parameters or similar.
+  * ``--remote-precmd`` allows execution of an extra command on the remote host
+    before launching a kernel.
+  * Better compatibility with Python 3.
+  * Kernel output on terminals with ``--verbose`` option for debugging.
+  * Connect to a host with ssh, slurm, or local kernels.
+  * Changed prefix to ``rik_``.
+  * kernel_cmd now requires the ``{connection_file}`` argument.
+  * ``remote_ikernel manage --show`` command to show existing kernels.
+  * Specify the working directory on the remote machine with ``--workdir``.
+  * ``kernel-uuid.json`` is copied to the working director for systems where
+    there is no access to the frontend filesystem.
+  * Added compatibility layer to get rid of Jupyter warnings.
```

### Comparing `remote_ipykernel-1.0.1/pyproject.toml` & `remote_ipykernel-1.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-[build-system]
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "remote_ipykernel"
-version = "1.0.1"
-description = "Running IPython kernels remotely and through batch queues"
-authors = [
-    { name = "Tom Daff"},
-    { name = "Conor Wills"}
-]
-readme = "README.md"
-requires-python = ">=3.7"
-license = {text = "BSD"}
-classifiers = [
-    'Programming Language :: Python :: 3',
-    'Framework :: IPython',
-    'License :: OSI Approved :: BSD License',
-]
-dependencies = [
-    'notebook>=6',
-    'pexpect>=4',
-    'tornado>=4'
-]
-
-[project.urls]
-Homepage = "https://github.com/CWills96/remote_ipykernel"
-
-[project.scripts]
-rkr = "remote_ipykernel.manage:manage"
-remote_ipykernel = "remote_ipykernel.manage:manage"
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "remote_ipykernel"
+version = "1.0.2"
+description = "Running IPython kernels remotely and through batch queues"
+authors = [
+    { name = "Tom Daff"},
+    { name = "Conor Wills"}
+]
+readme = "README.md"
+requires-python = ">=3.7"
+license = {text = "BSD"}
+classifiers = [
+    'Programming Language :: Python :: 3',
+    'Framework :: IPython',
+    'License :: OSI Approved :: BSD License',
+]
+dependencies = [
+    'notebook>=6',
+    'pexpect>=4',
+    'tornado>=4'
+]
+
+[project.urls]
+Homepage = "https://github.com/CWills96/remote_ipykernel"
+
+[project.scripts]
+rkr = "remote_ipykernel.manage:manage"
+remote_ipykernel = "remote_ipykernel.manage:manage"
```

### Comparing `remote_ipykernel-1.0.1/remote_ipykernel/compat.py` & `remote_ipykernel-1.0.2/remote_ipykernel/compat.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-"""
-compat.py
-
-Compatibility layer for transitions from IPython 3.0 to
-Jupyter structure. Will attempt to import Jupyter versions
-of modules, but will fall back to IPython if it is not
-available.
-
-Provides the following modules:
-    kernelspec -> {jupyter_client,IPython}.kernel.kernelspec
-    tempdir    -> {tempfile,IPython.utils.tempdir}
-
-"""
-# This is a module copied from Python 3.2, so will exist
-# in 3.2 onwards
-import tempfile as tempdir
-
-# kernelspec is moved in jupyter
-try:
-    from jupyter_client import kernelspec
-except ImportError:
-    from IPython.kernel import kernelspec
-
-# Otherwise it might be in genutils, but that will be dissolved
-if not hasattr(tempdir, "TemporaryDirectory"):
-    try:
-        from ipython_genutils import tempdir
-    except ImportError:
-        from IPython.utils import tempdir
-
-__all__ = ("kernelspec", "tempdir")
+"""
+compat.py
+
+Compatibility layer for transitions from IPython 3.0 to
+Jupyter structure. Will attempt to import Jupyter versions
+of modules, but will fall back to IPython if it is not
+available.
+
+Provides the following modules:
+    kernelspec -> {jupyter_client,IPython}.kernel.kernelspec
+    tempdir    -> {tempfile,IPython.utils.tempdir}
+
+"""
+# This is a module copied from Python 3.2, so will exist
+# in 3.2 onwards
+import tempfile as tempdir
+
+# kernelspec is moved in jupyter
+try:
+    from jupyter_client import kernelspec
+except ImportError:
+    from IPython.kernel import kernelspec
+
+# Otherwise it might be in genutils, but that will be dissolved
+if not hasattr(tempdir, "TemporaryDirectory"):
+    try:
+        from ipython_genutils import tempdir
+    except ImportError:
+        from IPython.utils import tempdir
+
+__all__ = ("kernelspec", "tempdir")
```

### Comparing `remote_ipykernel-1.0.1/remote_ipykernel/kernel.py` & `remote_ipykernel-1.0.2/remote_ipykernel/kernel.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,726 +1,726 @@
-#!/usr/bin/env python
-
-"""
-kernel.py
-
-Run standard IPython/Jupyter kernels on remote machines using
-job schedulers.
-
-"""
-
-import argparse
-import json
-import logging
-import os
-import re
-import subprocess
-import time
-import uuid
-
-import pexpect
-
-try:
-    from pexpect import spawn as pexpect_spawn
-except ImportError:
-    from pexpect.popen_spawn import PopenSpawn
-
-    class pexpect_spawn(PopenSpawn):
-        def isalive(self):
-            return self.proc.poll() is None
-
-
-from tornado.log import LogFormatter
-
-from remote_ipykernel import RIK_PREFIX, __version__
-
-
-# All the ports that need to be forwarded
-PORT_NAMES = ["hb_port", "shell_port", "iopub_port", "stdin_port", "control_port"]
-
-# Blend in with the notebook logging
-_LOG_FMT = (
-    "%(color)s[%(levelname)1.1s %(asctime)s.%(msecs).03d "
-    "%(name)s]%(end_color)s %(message)s"
-)
-_LOG_DATEFMT = "%H:%M:%S"
-
-
-def _setup_logging(verbose):
-    """
-    Create a logger using tornado coloured output to appear like
-    notebook messages. Will clear any existing handlers too.
-    """
-
-    log = logging.getLogger("remote_ikernel")
-    if verbose:
-        log.setLevel(logging.DEBUG)
-    else:
-        log.setLevel(logging.INFO)
-    # Logging on stderr
-    console = logging.StreamHandler()
-    console.setFormatter(LogFormatter(fmt=_LOG_FMT, datefmt=_LOG_DATEFMT))
-
-    log.handlers = []
-    log.addHandler(console)
-
-    # So that we can attach these to pexpect for debugging purposes
-    # we need to make them look like files
-    def _write(*args, **_):
-        """
-        Method to attach to a logger to allow it to act like a file object.
-
-        """
-        message = args[0]
-        # convert bytes from pexpect to something that prints better
-        if hasattr(message, "decode"):
-            message = message.decode("utf-8")
-
-        for line in message.splitlines():
-            if line.strip():
-                log.debug(line)
-
-    def _pass():
-        """pass"""
-        pass
-
-    log.write = _write
-    log.flush = _pass
-
-    return log
-
-
-def get_password(prompt):
-    """
-    Interact with the user and ask for a password.
-
-    Parameters
-    ----------
-    prompt : str
-        Text to show the user when asking for a password.
-
-    Returns
-    -------
-    password : str
-        The text input by the user.
-
-    """
-
-    if "SSH_ASKPASS" in os.environ:
-        password = subprocess.check_output([os.environ["SSH_ASKPASS"], prompt])
-    else:
-        raise RuntimeError("Unable to get password, try setting SSH_ASKPASS")
-
-    return password
-
-
-def check_password(connection):
-    """
-    Check to see if a newly spawned process requires a password and retrieve
-    it from the user if it does. Send the password to the process and
-    check repeatedly for more passwords.
-
-    Parameters
-    ----------
-    connection : pexpect.spawn
-        The connection to check. Requires an expect and sendline method.
-
-    """
-    # This will loop until no more passwords are encountered
-    while True:
-        try:
-            # Return all output as soon as anything arrives.
-            # Assume that immediate output includes the
-            # request for a password, or goes straight to
-            # a prompt.
-            text = connection.read_nonblocking(99999, timeout=-1)
-        except pexpect.TIMEOUT:
-            # Nothing more to read from the output
-            return
-
-        re_passphrase = re.search(b"Enter passphrase .*:", text)
-        re_password = re.search(b".*@.* password:", text)
-        if re_passphrase:
-            passphrase = get_password(re_passphrase.group())
-            connection.sendline(passphrase)
-        elif re_password:
-            password = get_password(re_password.group())
-            connection.sendline(password)
-        else:
-            # No more passwords or passphrases requested
-            return
-
-
-def extract_uuid(filename):
-    """
-    Given a filename containing a kernel, extract the uuid in
-    the kernel name.
-
-    Parameters
-    ----------
-    filename : str
-        The name of the kernel-...-json file with the connection info.
-
-    Returns
-    -------
-    uuid : str or None
-        The extracted uuid, or None if not found.
-    """
-
-    extracted = re.match(
-        ".*kernel-([0-9a-f]{8}-?[0-9a-f]{4}-?4[0-9a-f]{3}-"
-        "?[89ab][0-9a-f]{3}-?[0-9a-f]{12}).json",
-        filename,
-    )
-    if extracted is not None:
-        return uuid.UUID(extracted.group(1))
-    else:
-        return None
-
-
-class RemoteIKernel(object):
-    """
-    Configurable remote IPython kernel than runs on a node on a cluster
-    using the a job manager system.
-
-    """
-
-    def __init__(
-        self,
-        connection_info=None,
-        interface="sge",
-        cpus=1,
-        pe="smp",
-        kernel_cmd="ipython kernel",
-        workdir=None,
-        tunnel=True,
-        host=None,
-        precmd=None,
-        launch_args=None,
-        verbose=False,
-        tunnel_hosts=None,
-        launch_cmd=None,
-    ):
-        """
-        Initialise a kernel on a remote machine and start tunnels.
-
-        """
-
-        self.log = _setup_logging(verbose)
-        self.log.info("Remote kernel version: {0}.".format(__version__))
-        self.log.info("File location: {0}.".format(__file__))
-        # The connection info is provided by the notebook
-        try:
-            self.connection_info = json.load(open(connection_info))
-        except (OSError, IOError):
-            # file not found, allowed during testing
-            if interface != "test":
-                raise
-        self.interface = interface
-        self.cpus = cpus
-        self.pe = pe
-        self.kernel_cmd = kernel_cmd
-        self.host = host  # Name of node to be changed once connection is ready.
-        self.tunnel_hosts = tunnel_hosts
-        self.connection = None  # will usually be a spawned pexpect
-        self.workdir = workdir
-        self.tunnel = tunnel
-        self.tunnels = {}  # Processes running the SSH tunnels
-        self.precmd = precmd
-        self.launch_cmd = launch_cmd
-        self.launch_args = launch_args
-        self.cwd = os.getcwd()  # Launch directory may be needed if no workdir
-        # Assign the parent uuid, or generate a new one
-        self.uuid = extract_uuid(connection_info) or uuid.uuid4()
-
-        # Initiate an ssh tunnel through any tunnel hosts
-        # this will start a pexpect, so we must check if
-        # self.connection exists when launching the interface
-        if self.tunnel_hosts is not None:
-            self.launch_tunnel_hosts()
-
-        if self.interface == "local":
-            self.launch_local()
-        elif self.interface == "pbs":
-            self.launch_pbs()
-        elif self.interface == "sge":
-            self.launch_sge()
-        elif self.interface == "sge_qrsh":
-            self.launch_sge(qlogin="qrsh")
-        elif self.interface == "slurm":
-            self.launch_slurm()
-        elif self.interface == "lsf":
-            self.launch_lsf()
-        elif self.interface == "ssh":
-            self.launch_ssh()
-        elif self.interface == "test":
-            # don't start anything if testing
-            pass
-        else:
-            raise ValueError("Unknown interface {0}".format(interface))
-
-        # If we've established a connection, start the kernel!
-        if self.connection is not None:
-            self.start_kernel()
-            if self.tunnel:
-                self.tunnel_connection()
-
-    def get_cmd(self, default):
-        """
-        Check if cmd has been overridden and return that, otherwise use the
-        default.
-        """
-        if self.launch_cmd is not None:
-            self.log.info(
-                "Overriding default '{0}' with '{1}'.".format(default, self.launch_cmd)
-            )
-            return self.launch_cmd
-        else:
-            self.log.info("Default launch command: '{0}'.".format(default))
-            return default
-
-    def launch_tunnel_hosts(self):
-        """
-        Build a chain of hosts to tunnel through and start an ssh
-        chain with pexpect.
-        """
-        # TODO: does this need to be more than several ssh commands?
-        self._spawn(self.tunnel_hosts_cmd)
-        check_password(self.connection)
-
-    def launch_local(self):
-        """
-        Initialise a shell on the local machine that can be interacted with.
-        Stop tunneling if it is not needed.
-        """
-        self.log.info("Launching local kernel.")
-        if self.launch_args:
-            bash = "{bash} {args}".format(
-                bash=self.get_cmd("/bin/bash"), args=self.launch_args
-            )
-        else:
-            bash = self.get_cmd("/bin/bash")
-        self._spawn(bash)
-        # Don't try and start tunnels to the same machine. Causes issues.
-        self.tunnel = False
-
-    def launch_ssh(self):
-        """
-        Initialise a connection through ssh.
-
-        Launch an ssh connection using pexpect so it can be interacted with.
-        """
-        self.log.info("Launching kernel over SSH.")
-        if self.launch_args:
-            launch_args = self.launch_args
-        else:
-            launch_args = ""
-
-        if ":" in self.host:
-            host = self.host.replace(":", " -p ")
-        else:
-            host = self.host
-
-        login_cmd = "ssh -o StrictHostKeyChecking=no {args} {host}".format(
-            args=launch_args, host=host
-        )
-        self.log.info("Login command: '{0}'.".format(login_cmd))
-        self._spawn(login_cmd)
-        check_password(self.connection)
-
-    def launch_pbs(self):
-        """
-        Start a kernel through the torque 'qsub -I' command. The connection
-        will use the object's connection_info and kernel_command.
-        """
-        self.log.info("Launching kernel through PBS/Torque.")
-        job_name = "remote_ikernel"
-        if self.cpus > 1:
-            cpu_string = "-l ncpus={cpus}".format(cpus=self.cpus)
-        else:
-            cpu_string = ""
-        if self.launch_args:
-            args_string = self.launch_args
-        else:
-            args_string = ""
-        pbs_cmd = "{qsub} -I {cpus} -N {name} {args}".format(
-            cpus=cpu_string, name=job_name, args=args_string, qsub=self.get_cmd("qsub")
-        )
-        self.log.info("PBS command: '{0}'.".format(pbs_cmd))
-        # Will wait in the queue for up to 10 mins
-        qsub_i = self._spawn(pbs_cmd)
-        # Hopefully this text is universal? Job started...
-        qsub_i.expect("qsub: job (.*) ready")
-        # Now we have to ask for the hostname (any way for it to
-        # say automatically?)
-        qsub_i.sendline("echo Running on `hostname`")
-
-        # hostnames whould be alphanumeric with . and - permitted
-        # This way we also ignore the echoed echo command
-        qsub_i.expect(r"Running on ([\w.-]+)")
-        node = qsub_i.match.groups()[0]
-
-        self.log.info("Established session on node: {0}.".format(node))
-        self.host = node
-
-    def launch_sge(self, qlogin="qlogin"):
-        """
-        Start a kernel through the gridengine 'qlogin' command. The connection
-        will use the object's connection_info and kernel_command. 'qlogin' can
-        also be replaced with 'qrsh' on some systems.
-        """
-        self.log.info("Launching kernel through GridEngine.")
-        job_name = "remote_ikernel"
-        if self.cpus > 1:
-            pe_string = "-pe {pe} {cpus}".format(pe=self.pe, cpus=self.cpus)
-        else:
-            pe_string = ""
-        if self.launch_args:
-            args_string = self.launch_args
-        else:
-            args_string = ""
-        sge_cmd = "{qlogin} -verbose -now n {pe} -N {name} {args}".format(
-            qlogin=self.get_cmd(qlogin), pe=pe_string, name=job_name, args=args_string
-        )
-        self.log.info("Gridengine command: '{0}'.".format(sge_cmd))
-        # Will wait in the queue for up to 10 mins
-        qlogin = self._spawn(sge_cmd)
-        # Hopefully this text is universal?
-        qlogin.expect("Establishing .* session to host (.*) ...")
-
-        node = qlogin.match.groups()[0]
-        self.log.info("Established session on node: {0}.".format(node))
-        self.host = node
-
-    def launch_slurm(self):
-        """
-        Start a kernel through the slurm 'srun' command. Bind the spawned
-        pexpect to the class to interact with it.
-        """
-        self.log.info("Launching kernel through SLURM.")
-        job_name = "remote_ikernel"
-        if self.cpus > 1:
-            tasks = "--cpus-per-task {cpus}".format(cpus=self.cpus)
-        else:
-            tasks = ""
-        if self.launch_args:
-            launch_args = self.launch_args
-        else:
-            launch_args = ""
-        # -i is interactive, -v so we know the node, --pty needed for SIGINT
-        # tasks must be before the bash!
-        srun_cmd = "{srun} {tasks} -J {job_name} {args} -v --pty bash -i" "".format(
-            srun=self.get_cmd("srun"), tasks=tasks, job_name=job_name, args=launch_args
-        )
-        self.log.info("SLURM command: '{0}'.".format(srun_cmd))
-        srun = self._spawn(srun_cmd)
-        # Hopefully this text is universal?
-        srun.expect("srun: Node (.*), .* tasks started")
-
-        node = srun.match.groups()[0]
-        self.log.info("Established session on node: {0}.".format(node))
-        self.host = node
-
-    def launch_lsf(self):
-        """
-        Start a kernel through the Platform LSF 'bsub' command in interactive
-        mode. Bind the spawned pexpect to the class to interact with it.
-        """
-        self.log.info("Launching kernel through Platform LSF.")
-        job_name = "remote_ikernel"
-        if self.cpus > 1:
-            tasks = "-n {cpus}".format(cpus=self.cpus)
-        else:
-            tasks = ""
-        if self.launch_args:
-            launch_args = self.launch_args
-        else:
-            launch_args = ""
-        # -Is is interactive shell mode
-        bsub_cmd = "{bsub} {tasks} -J {job_name} {args} -Is /bin/bash".format(
-            bsub=self.get_cmd("bsub"), tasks=tasks, job_name=job_name, args=launch_args
-        )
-        self.log.info("LSF command: '{0}'.".format(bsub_cmd))
-        bsub = self._spawn(bsub_cmd)
-        # Hopefully this text is universal?
-        bsub.expect("<<Starting on (.*)>>")
-
-        node = bsub.match.groups()[0]
-        self.log.info("Established session on node: {0}.".format(node))
-        self.host = node
-
-    def start_kernel(self):
-        """
-        Start the kernel on the remote machine.
-        """
-        conn = self.connection
-        # If the remote system has a different filesystem, a temporary
-        # file is needed to hold the json.
-        kernel_name = "./{0}kernel-{1}.json".format(RIK_PREFIX, self.uuid)
-        self.log.info("Established connection; starting kernel.")
-
-        # Use the specified working directory or try to change to the same
-        # directory on the remote machine.
-        if self.workdir:
-            self.log.info("Remote working directory {0}.".format(self.workdir))
-            conn.sendline('cd "{0}"'.format(self.workdir))
-        else:
-            self.log.info("Current working directory {0}.".format(self.cwd))
-            conn.sendline('cd "{0}"'.format(self.cwd))
-
-        # Create a temporary file to store a copy of the connection information
-        # Delete the file if it already exists
-        conn.sendline("rm -f {0}".format(kernel_name))
-        file_contents = json.dumps(self.connection_info)
-        conn.sendline("echo '{0}' > {1}".format(file_contents, kernel_name))
-
-        # Is this the best place for a pre-command? I guess people will just
-        # have to deal with it. Pass it on as is.
-        if self.precmd:
-            conn.sendline(self.precmd)
-
-        # Init as a background process so we can delete the tempfile after
-        kernel_init = "{kernel_cmd}".format(kernel_cmd=self.kernel_cmd)
-        kernel_init = kernel_init.format(
-            host_connection_file=kernel_name, ci=self.connection_info
-        )
-        self.log.info("Running kernel command: '{0}'.".format(kernel_init))
-        conn.sendline(kernel_init)
-
-        # The kernel blocks further commands, so queue deletion of the
-        # transient file for once the process stops. Trying to do this
-        # whilst simultaneously starting the kernel ended up deleting
-        # the file before it was read.
-        conn.sendline("rm -f {0}".format(kernel_name))
-        conn.sendline("exit")
-
-        # Could check this for errors?
-        conn.expect("exit")
-
-    def tunnel_connection(self):
-        """
-        Set up tunnels to the node using the connection information.
-        """
-        # Auto accept ssh keys so tunnels work on previously unknown hosts.
-        # This might need to change, but the other option is to get user or
-        # admin to turn StrictHostKeyChecking off in .ssh/ssh_config for this
-        # to work seamlessly. (tunnels will have already done this)
-        pre = self.tunnel_hosts_cmd or ""
-
-        if ":" in self.host:
-            host = self.host.replace(":", " -p ")
-        else:
-            host = self.host
-
-        pexpect_spawn(
-            "{pre} ssh -o StrictHostKeyChecking=no "
-            "{host}".format(pre=pre, host=host).strip(),
-            logfile=self.log,
-        ).sendline("exit")
-
-        # connection info should have the ports being used
-        tunnel_command = self.tunnel_cmd.format(**self.connection_info)
-        tunnel = pexpect_spawn(tunnel_command, logfile=self.log)
-        check_password(tunnel)
-
-        self.log.info(
-            "Setting up tunnels on ports: {0}.".format(
-                ", ".join(
-                    [
-                        "{0}".format(self.connection_info[port_name])
-                        for port_name in PORT_NAMES
-                    ]
-                )
-            )
-        )
-        self.log.debug("Tunnel command: {0}.".format(tunnel_command))
-
-        # Store the tunnel
-        self.tunnels["tunnel"] = tunnel
-
-    def check_tunnels(self):
-        """
-        Check the PID of tunnels and restart any that have died.
-        """
-        if "tunnel" in self.tunnels:
-            if not self.tunnels["tunnel"].isalive():
-                self.log.debug("Restarting ssh tunnels.")
-                self.tunnel_connection()
-
-    def keep_alive(self, timeout=5):
-        """
-        Keep the script alive forever. KeyboardInterrupt will get passed on
-        to the kernel. The timeout determines how often the ssh tunnels are
-        checked.
-        """
-        # The timeout determines how long each loop will be,
-        # if an ssh tunnel dies, this is how long it will be
-        # before it is revived.
-        self.connection.timeout = timeout
-        time.sleep(timeout)
-
-        # There might be a more elegant way to do this, but since this
-        # process doesn't do anything and is managed by the notebook
-        # it really doesn't matter
-        while True:
-            # If the kernel dies, we should too, but try and
-            # give some error info
-            if not self.connection.isalive():
-                self.log.error("Kernel died.")
-                for line in self.connection.readlines():
-                    if line.strip():
-                        self.log.error(line)
-                break
-            # Kernel is still alive, ensure tunnels are too
-            self.check_tunnels()
-            try:
-                # read anything from the kernel output, pexpect
-                # logging will be set up to emit anything if
-                # required.
-                self.connection.readlines()
-            except pexpect.TIMEOUT:
-                # Raises timeout if there is no data, prevents blocking
-                # Moves on to the next loop.
-                pass
-            except KeyboardInterrupt:
-                self.log.info("Caught interrupt; sending SIGINT to kernel.")
-                self.connection.sendintr()
-
-    def _spawn(self, command, timeout=600):
-        """
-        Helper to start a pexpect.spawn as self.connection. If the session
-        has already been started, just pass the command to sendline. Return
-        the current spawn instance. The logfile is implicitly set to
-        self.log.
-
-        Parameters
-        ----------
-        command : str
-            Command to spawn or run in the current session.
-        timeout : int
-            Timeout for command to complete, passed to pexpect.
-
-        Returns
-        -------
-        connection : pexpect.spawn
-            The connection object. This is also attached to the class.
-        """
-        if self.connection is None:
-            self.connection = pexpect_spawn(command, timeout=timeout, logfile=self.log)
-        else:
-            self.connection.sendline(command)
-
-        return self.connection
-
-    @property
-    def tunnel_hosts_cmd(self):
-        """Return the ssh command to tunnel through the middle hosts."""
-        if self.tunnel_hosts is None:
-            return None
-
-        cmd = []
-        ssh = "ssh -o StrictHostKeyChecking=no"
-
-        for host in self.tunnel_hosts:
-            if ":" in host:
-                host = host.replace(":", " -p ")
-
-            cmd.extend([ssh, host])
-
-        return " ".join(cmd)
-
-    @property
-    def tunnel_cmd(self):
-        """Return a tunnelling command that just needs a port."""
-        # zmq needs str in Python 3, but pexpect gives bytes
-        if hasattr(self.host, "decode"):
-            self.host = self.host.decode("utf-8")
-
-        # One connection can tunnel all the ports
-        ports_str = " ".join(
-            [
-                "-L 127.0.0.1:{{{port}}}:127.0.0.1:{{{port}}}" "".format(port=port)
-                for port in PORT_NAMES
-            ]
-        )
-
-        ssh = "ssh"
-
-        # Add all the gateway machines as an ssh chain
-        pre_ssh = []
-        for pre_host in self.tunnel_hosts or []:
-            if ":" in pre_host:
-                pre_host = pre_host.replace(":", " -p ")
-
-            pre_ssh.append(
-                "{ssh} {ports_str} {pre_host}".format(
-                    ssh=ssh, pre_host=pre_host, ports_str=ports_str
-                )
-            )
-
-        if ":" in self.host:
-            host = self.host.replace(":", " -p ")
-        else:
-            host = self.host
-
-        # Timeout is specified here, this should be longer than the checking
-        # interval
-        # .strip() to prevent leading spaces
-        tunnel_cmd = (
-            " ".join(pre_ssh)
-            + " "
-            + "{ssh} {ports_str} {host} sleep 600".format(
-                ssh=ssh, host=host, ports_str=ports_str
-            )
-        ).strip()
-
-        self.log.debug("Tunnel command: {0}".format(tunnel_cmd))
-        return tunnel_cmd
-
-
-def start_remote_kernel():
-    """
-    Read command line arguments and initialise a kernel.
-    """
-    # These will not face a user since they are interpreting the command from
-    # kernel the kernel.json
-    description = "This is the kernel launcher! Try '%(prog)s manage'..."
-    parser = argparse.ArgumentParser(description=description)
-    parser.add_argument("connection_info")
-    parser.add_argument("--interface", default="local")
-    parser.add_argument("--cpus", type=int, default=1)
-    parser.add_argument("--pe", default="smp")
-    parser.add_argument(
-        "--kernel_cmd", default="ipython kernel -f {host_connection_file}"
-    )
-    parser.add_argument("--workdir")
-    parser.add_argument("--host")
-    parser.add_argument("--precmd")
-    parser.add_argument("--launch-args")
-    parser.add_argument("--verbose", action="store_true")
-    parser.add_argument("--tunnel-hosts", nargs="+")
-    parser.add_argument("--launch-cmd")
-    parser.add_argument(
-        "--version",
-        "-V",
-        action="version",
-        version="Remote Jupyter kernel launcher (version {0}).\n\n"
-        "Use the '%(prog)s manage' subcommand for managing "
-        "kernels.".format(__version__),
-    )
-    args = parser.parse_args()
-
-    kernel = RemoteIKernel(
-        connection_info=args.connection_info,
-        interface=args.interface,
-        cpus=args.cpus,
-        pe=args.pe,
-        kernel_cmd=args.kernel_cmd,
-        workdir=args.workdir,
-        host=args.host,
-        precmd=args.precmd,
-        launch_args=args.launch_args,
-        verbose=args.verbose,
-        tunnel_hosts=args.tunnel_hosts,
-        launch_cmd=args.launch_cmd,
-    )
-    kernel.keep_alive()
+#!/usr/bin/env python
+
+"""
+kernel.py
+
+Run standard IPython/Jupyter kernels on remote machines using
+job schedulers.
+
+"""
+
+import argparse
+import json
+import logging
+import os
+import re
+import subprocess
+import time
+import uuid
+
+import pexpect
+
+try:
+    from pexpect import spawn as pexpect_spawn
+except ImportError:
+    from pexpect.popen_spawn import PopenSpawn
+
+    class pexpect_spawn(PopenSpawn):
+        def isalive(self):
+            return self.proc.poll() is None
+
+
+from tornado.log import LogFormatter
+
+from remote_ipykernel import RIK_PREFIX, __version__
+
+
+# All the ports that need to be forwarded
+PORT_NAMES = ["hb_port", "shell_port", "iopub_port", "stdin_port", "control_port"]
+
+# Blend in with the notebook logging
+_LOG_FMT = (
+    "%(color)s[%(levelname)1.1s %(asctime)s.%(msecs).03d "
+    "%(name)s]%(end_color)s %(message)s"
+)
+_LOG_DATEFMT = "%H:%M:%S"
+
+
+def _setup_logging(verbose):
+    """
+    Create a logger using tornado coloured output to appear like
+    notebook messages. Will clear any existing handlers too.
+    """
+
+    log = logging.getLogger("remote_ikernel")
+    if verbose:
+        log.setLevel(logging.DEBUG)
+    else:
+        log.setLevel(logging.INFO)
+    # Logging on stderr
+    console = logging.StreamHandler()
+    console.setFormatter(LogFormatter(fmt=_LOG_FMT, datefmt=_LOG_DATEFMT))
+
+    log.handlers = []
+    log.addHandler(console)
+
+    # So that we can attach these to pexpect for debugging purposes
+    # we need to make them look like files
+    def _write(*args, **_):
+        """
+        Method to attach to a logger to allow it to act like a file object.
+
+        """
+        message = args[0]
+        # convert bytes from pexpect to something that prints better
+        if hasattr(message, "decode"):
+            message = message.decode("utf-8")
+
+        for line in message.splitlines():
+            if line.strip():
+                log.debug(line)
+
+    def _pass():
+        """pass"""
+        pass
+
+    log.write = _write
+    log.flush = _pass
+
+    return log
+
+
+def get_password(prompt):
+    """
+    Interact with the user and ask for a password.
+
+    Parameters
+    ----------
+    prompt : str
+        Text to show the user when asking for a password.
+
+    Returns
+    -------
+    password : str
+        The text input by the user.
+
+    """
+
+    if "SSH_ASKPASS" in os.environ:
+        password = subprocess.check_output([os.environ["SSH_ASKPASS"], prompt])
+    else:
+        raise RuntimeError("Unable to get password, try setting SSH_ASKPASS")
+
+    return password
+
+
+def check_password(connection):
+    """
+    Check to see if a newly spawned process requires a password and retrieve
+    it from the user if it does. Send the password to the process and
+    check repeatedly for more passwords.
+
+    Parameters
+    ----------
+    connection : pexpect.spawn
+        The connection to check. Requires an expect and sendline method.
+
+    """
+    # This will loop until no more passwords are encountered
+    while True:
+        try:
+            # Return all output as soon as anything arrives.
+            # Assume that immediate output includes the
+            # request for a password, or goes straight to
+            # a prompt.
+            text = connection.read_nonblocking(99999, timeout=-1)
+        except pexpect.TIMEOUT:
+            # Nothing more to read from the output
+            return
+
+        re_passphrase = re.search(b"Enter passphrase .*:", text)
+        re_password = re.search(b".*@.* password:", text)
+        if re_passphrase:
+            passphrase = get_password(re_passphrase.group())
+            connection.sendline(passphrase)
+        elif re_password:
+            password = get_password(re_password.group())
+            connection.sendline(password)
+        else:
+            # No more passwords or passphrases requested
+            return
+
+
+def extract_uuid(filename):
+    """
+    Given a filename containing a kernel, extract the uuid in
+    the kernel name.
+
+    Parameters
+    ----------
+    filename : str
+        The name of the kernel-...-json file with the connection info.
+
+    Returns
+    -------
+    uuid : str or None
+        The extracted uuid, or None if not found.
+    """
+
+    extracted = re.match(
+        ".*kernel-([0-9a-f]{8}-?[0-9a-f]{4}-?4[0-9a-f]{3}-"
+        "?[89ab][0-9a-f]{3}-?[0-9a-f]{12}).json",
+        filename,
+    )
+    if extracted is not None:
+        return uuid.UUID(extracted.group(1))
+    else:
+        return None
+
+
+class RemoteIKernel(object):
+    """
+    Configurable remote IPython kernel than runs on a node on a cluster
+    using the a job manager system.
+
+    """
+
+    def __init__(
+        self,
+        connection_info=None,
+        interface="sge",
+        cpus=1,
+        pe="smp",
+        kernel_cmd="ipython kernel",
+        workdir=None,
+        tunnel=True,
+        host=None,
+        precmd=None,
+        launch_args=None,
+        verbose=False,
+        tunnel_hosts=None,
+        launch_cmd=None,
+    ):
+        """
+        Initialise a kernel on a remote machine and start tunnels.
+
+        """
+
+        self.log = _setup_logging(verbose)
+        self.log.info("Remote kernel version: {0}.".format(__version__))
+        self.log.info("File location: {0}.".format(__file__))
+        # The connection info is provided by the notebook
+        try:
+            self.connection_info = json.load(open(connection_info))
+        except (OSError, IOError):
+            # file not found, allowed during testing
+            if interface != "test":
+                raise
+        self.interface = interface
+        self.cpus = cpus
+        self.pe = pe
+        self.kernel_cmd = kernel_cmd
+        self.host = host  # Name of node to be changed once connection is ready.
+        self.tunnel_hosts = tunnel_hosts
+        self.connection = None  # will usually be a spawned pexpect
+        self.workdir = workdir
+        self.tunnel = tunnel
+        self.tunnels = {}  # Processes running the SSH tunnels
+        self.precmd = precmd
+        self.launch_cmd = launch_cmd
+        self.launch_args = launch_args
+        self.cwd = os.getcwd()  # Launch directory may be needed if no workdir
+        # Assign the parent uuid, or generate a new one
+        self.uuid = extract_uuid(connection_info) or uuid.uuid4()
+
+        # Initiate an ssh tunnel through any tunnel hosts
+        # this will start a pexpect, so we must check if
+        # self.connection exists when launching the interface
+        if self.tunnel_hosts is not None:
+            self.launch_tunnel_hosts()
+
+        if self.interface == "local":
+            self.launch_local()
+        elif self.interface == "pbs":
+            self.launch_pbs()
+        elif self.interface == "sge":
+            self.launch_sge()
+        elif self.interface == "sge_qrsh":
+            self.launch_sge(qlogin="qrsh")
+        elif self.interface == "slurm":
+            self.launch_slurm()
+        elif self.interface == "lsf":
+            self.launch_lsf()
+        elif self.interface == "ssh":
+            self.launch_ssh()
+        elif self.interface == "test":
+            # don't start anything if testing
+            pass
+        else:
+            raise ValueError("Unknown interface {0}".format(interface))
+
+        # If we've established a connection, start the kernel!
+        if self.connection is not None:
+            self.start_kernel()
+            if self.tunnel:
+                self.tunnel_connection()
+
+    def get_cmd(self, default):
+        """
+        Check if cmd has been overridden and return that, otherwise use the
+        default.
+        """
+        if self.launch_cmd is not None:
+            self.log.info(
+                "Overriding default '{0}' with '{1}'.".format(default, self.launch_cmd)
+            )
+            return self.launch_cmd
+        else:
+            self.log.info("Default launch command: '{0}'.".format(default))
+            return default
+
+    def launch_tunnel_hosts(self):
+        """
+        Build a chain of hosts to tunnel through and start an ssh
+        chain with pexpect.
+        """
+        # TODO: does this need to be more than several ssh commands?
+        self._spawn(self.tunnel_hosts_cmd)
+        check_password(self.connection)
+
+    def launch_local(self):
+        """
+        Initialise a shell on the local machine that can be interacted with.
+        Stop tunneling if it is not needed.
+        """
+        self.log.info("Launching local kernel.")
+        if self.launch_args:
+            bash = "{bash} {args}".format(
+                bash=self.get_cmd("/bin/bash"), args=self.launch_args
+            )
+        else:
+            bash = self.get_cmd("/bin/bash")
+        self._spawn(bash)
+        # Don't try and start tunnels to the same machine. Causes issues.
+        self.tunnel = False
+
+    def launch_ssh(self):
+        """
+        Initialise a connection through ssh.
+
+        Launch an ssh connection using pexpect so it can be interacted with.
+        """
+        self.log.info("Launching kernel over SSH.")
+        if self.launch_args:
+            launch_args = self.launch_args
+        else:
+            launch_args = ""
+
+        if ":" in self.host:
+            host = self.host.replace(":", " -p ")
+        else:
+            host = self.host
+
+        login_cmd = "ssh -o StrictHostKeyChecking=no {args} {host}".format(
+            args=launch_args, host=host
+        )
+        self.log.info("Login command: '{0}'.".format(login_cmd))
+        self._spawn(login_cmd)
+        check_password(self.connection)
+
+    def launch_pbs(self):
+        """
+        Start a kernel through the torque 'qsub -I' command. The connection
+        will use the object's connection_info and kernel_command.
+        """
+        self.log.info("Launching kernel through PBS/Torque.")
+        job_name = "remote_ikernel"
+        if self.cpus > 1:
+            cpu_string = "-l ncpus={cpus}".format(cpus=self.cpus)
+        else:
+            cpu_string = ""
+        if self.launch_args:
+            args_string = self.launch_args
+        else:
+            args_string = ""
+        pbs_cmd = "{qsub} -I {cpus} -N {name} {args}".format(
+            cpus=cpu_string, name=job_name, args=args_string, qsub=self.get_cmd("qsub")
+        )
+        self.log.info("PBS command: '{0}'.".format(pbs_cmd))
+        # Will wait in the queue for up to 10 mins
+        qsub_i = self._spawn(pbs_cmd)
+        # Hopefully this text is universal? Job started...
+        qsub_i.expect("qsub: job (.*) ready")
+        # Now we have to ask for the hostname (any way for it to
+        # say automatically?)
+        qsub_i.sendline("echo Running on `hostname`")
+
+        # hostnames whould be alphanumeric with . and - permitted
+        # This way we also ignore the echoed echo command
+        qsub_i.expect(r"Running on ([\w.-]+)")
+        node = qsub_i.match.groups()[0]
+
+        self.log.info("Established session on node: {0}.".format(node))
+        self.host = node
+
+    def launch_sge(self, qlogin="qlogin"):
+        """
+        Start a kernel through the gridengine 'qlogin' command. The connection
+        will use the object's connection_info and kernel_command. 'qlogin' can
+        also be replaced with 'qrsh' on some systems.
+        """
+        self.log.info("Launching kernel through GridEngine.")
+        job_name = "remote_ikernel"
+        if self.cpus > 1:
+            pe_string = "-pe {pe} {cpus}".format(pe=self.pe, cpus=self.cpus)
+        else:
+            pe_string = ""
+        if self.launch_args:
+            args_string = self.launch_args
+        else:
+            args_string = ""
+        sge_cmd = "{qlogin} -verbose -now n {pe} -N {name} {args}".format(
+            qlogin=self.get_cmd(qlogin), pe=pe_string, name=job_name, args=args_string
+        )
+        self.log.info("Gridengine command: '{0}'.".format(sge_cmd))
+        # Will wait in the queue for up to 10 mins
+        qlogin = self._spawn(sge_cmd)
+        # Hopefully this text is universal?
+        qlogin.expect("Establishing .* session to host (.*) ...")
+
+        node = qlogin.match.groups()[0]
+        self.log.info("Established session on node: {0}.".format(node))
+        self.host = node
+
+    def launch_slurm(self):
+        """
+        Start a kernel through the slurm 'srun' command. Bind the spawned
+        pexpect to the class to interact with it.
+        """
+        self.log.info("Launching kernel through SLURM.")
+        job_name = "remote_ikernel"
+        if self.cpus > 1:
+            tasks = "--cpus-per-task {cpus}".format(cpus=self.cpus)
+        else:
+            tasks = ""
+        if self.launch_args:
+            launch_args = self.launch_args
+        else:
+            launch_args = ""
+        # -i is interactive, -v so we know the node, --pty needed for SIGINT
+        # tasks must be before the bash!
+        srun_cmd = "{srun} {tasks} -J {job_name} {args} -v --pty bash -i" "".format(
+            srun=self.get_cmd("srun"), tasks=tasks, job_name=job_name, args=launch_args
+        )
+        self.log.info("SLURM command: '{0}'.".format(srun_cmd))
+        srun = self._spawn(srun_cmd)
+        # Hopefully this text is universal?
+        srun.expect("srun: Node (.*), .* tasks started")
+
+        node = srun.match.groups()[0]
+        self.log.info("Established session on node: {0}.".format(node))
+        self.host = node
+
+    def launch_lsf(self):
+        """
+        Start a kernel through the Platform LSF 'bsub' command in interactive
+        mode. Bind the spawned pexpect to the class to interact with it.
+        """
+        self.log.info("Launching kernel through Platform LSF.")
+        job_name = "remote_ikernel"
+        if self.cpus > 1:
+            tasks = "-n {cpus}".format(cpus=self.cpus)
+        else:
+            tasks = ""
+        if self.launch_args:
+            launch_args = self.launch_args
+        else:
+            launch_args = ""
+        # -Is is interactive shell mode
+        bsub_cmd = "{bsub} {tasks} -J {job_name} {args} -Is /bin/bash".format(
+            bsub=self.get_cmd("bsub"), tasks=tasks, job_name=job_name, args=launch_args
+        )
+        self.log.info("LSF command: '{0}'.".format(bsub_cmd))
+        bsub = self._spawn(bsub_cmd)
+        # Hopefully this text is universal?
+        bsub.expect("<<Starting on (.*)>>")
+
+        node = bsub.match.groups()[0]
+        self.log.info("Established session on node: {0}.".format(node))
+        self.host = node
+
+    def start_kernel(self):
+        """
+        Start the kernel on the remote machine.
+        """
+        conn = self.connection
+        # If the remote system has a different filesystem, a temporary
+        # file is needed to hold the json.
+        kernel_name = "./{0}kernel-{1}.json".format(RIK_PREFIX, self.uuid)
+        self.log.info("Established connection; starting kernel.")
+
+        # Use the specified working directory or try to change to the same
+        # directory on the remote machine.
+        if self.workdir:
+            self.log.info("Remote working directory {0}.".format(self.workdir))
+            conn.sendline('cd "{0}"'.format(self.workdir))
+        else:
+            self.log.info("Current working directory {0}.".format(self.cwd))
+            conn.sendline('cd "{0}"'.format(self.cwd))
+
+        # Create a temporary file to store a copy of the connection information
+        # Delete the file if it already exists
+        conn.sendline("rm -f {0}".format(kernel_name))
+        file_contents = json.dumps(self.connection_info)
+        conn.sendline("echo '{0}' > {1}".format(file_contents, kernel_name))
+
+        # Is this the best place for a pre-command? I guess people will just
+        # have to deal with it. Pass it on as is.
+        if self.precmd:
+            conn.sendline(self.precmd)
+
+        # Init as a background process so we can delete the tempfile after
+        kernel_init = "{kernel_cmd}".format(kernel_cmd=self.kernel_cmd)
+        kernel_init = kernel_init.format(
+            host_connection_file=kernel_name, ci=self.connection_info
+        )
+        self.log.info("Running kernel command: '{0}'.".format(kernel_init))
+        conn.sendline(kernel_init)
+
+        # The kernel blocks further commands, so queue deletion of the
+        # transient file for once the process stops. Trying to do this
+        # whilst simultaneously starting the kernel ended up deleting
+        # the file before it was read.
+        conn.sendline("rm -f {0}".format(kernel_name))
+        conn.sendline("exit")
+
+        # Could check this for errors?
+        conn.expect("exit")
+
+    def tunnel_connection(self):
+        """
+        Set up tunnels to the node using the connection information.
+        """
+        # Auto accept ssh keys so tunnels work on previously unknown hosts.
+        # This might need to change, but the other option is to get user or
+        # admin to turn StrictHostKeyChecking off in .ssh/ssh_config for this
+        # to work seamlessly. (tunnels will have already done this)
+        pre = self.tunnel_hosts_cmd or ""
+
+        if ":" in self.host:
+            host = self.host.replace(":", " -p ")
+        else:
+            host = self.host
+
+        pexpect_spawn(
+            "{pre} ssh -o StrictHostKeyChecking=no "
+            "{host}".format(pre=pre, host=host).strip(),
+            logfile=self.log,
+        ).sendline("exit")
+
+        # connection info should have the ports being used
+        tunnel_command = self.tunnel_cmd.format(**self.connection_info)
+        tunnel = pexpect_spawn(tunnel_command, logfile=self.log)
+        check_password(tunnel)
+
+        self.log.info(
+            "Setting up tunnels on ports: {0}.".format(
+                ", ".join(
+                    [
+                        "{0}".format(self.connection_info[port_name])
+                        for port_name in PORT_NAMES
+                    ]
+                )
+            )
+        )
+        self.log.debug("Tunnel command: {0}.".format(tunnel_command))
+
+        # Store the tunnel
+        self.tunnels["tunnel"] = tunnel
+
+    def check_tunnels(self):
+        """
+        Check the PID of tunnels and restart any that have died.
+        """
+        if "tunnel" in self.tunnels:
+            if not self.tunnels["tunnel"].isalive():
+                self.log.debug("Restarting ssh tunnels.")
+                self.tunnel_connection()
+
+    def keep_alive(self, timeout=5):
+        """
+        Keep the script alive forever. KeyboardInterrupt will get passed on
+        to the kernel. The timeout determines how often the ssh tunnels are
+        checked.
+        """
+        # The timeout determines how long each loop will be,
+        # if an ssh tunnel dies, this is how long it will be
+        # before it is revived.
+        self.connection.timeout = timeout
+        time.sleep(timeout)
+
+        # There might be a more elegant way to do this, but since this
+        # process doesn't do anything and is managed by the notebook
+        # it really doesn't matter
+        while True:
+            # If the kernel dies, we should too, but try and
+            # give some error info
+            if not self.connection.isalive():
+                self.log.error("Kernel died.")
+                for line in self.connection.readlines():
+                    if line.strip():
+                        self.log.error(line)
+                break
+            # Kernel is still alive, ensure tunnels are too
+            self.check_tunnels()
+            try:
+                # read anything from the kernel output, pexpect
+                # logging will be set up to emit anything if
+                # required.
+                self.connection.readlines()
+            except pexpect.TIMEOUT:
+                # Raises timeout if there is no data, prevents blocking
+                # Moves on to the next loop.
+                pass
+            except KeyboardInterrupt:
+                self.log.info("Caught interrupt; sending SIGINT to kernel.")
+                self.connection.sendintr()
+
+    def _spawn(self, command, timeout=600):
+        """
+        Helper to start a pexpect.spawn as self.connection. If the session
+        has already been started, just pass the command to sendline. Return
+        the current spawn instance. The logfile is implicitly set to
+        self.log.
+
+        Parameters
+        ----------
+        command : str
+            Command to spawn or run in the current session.
+        timeout : int
+            Timeout for command to complete, passed to pexpect.
+
+        Returns
+        -------
+        connection : pexpect.spawn
+            The connection object. This is also attached to the class.
+        """
+        if self.connection is None:
+            self.connection = pexpect_spawn(command, timeout=timeout, logfile=self.log)
+        else:
+            self.connection.sendline(command)
+
+        return self.connection
+
+    @property
+    def tunnel_hosts_cmd(self):
+        """Return the ssh command to tunnel through the middle hosts."""
+        if self.tunnel_hosts is None:
+            return None
+
+        cmd = []
+        ssh = "ssh -o StrictHostKeyChecking=no"
+
+        for host in self.tunnel_hosts:
+            if ":" in host:
+                host = host.replace(":", " -p ")
+
+            cmd.extend([ssh, host])
+
+        return " ".join(cmd)
+
+    @property
+    def tunnel_cmd(self):
+        """Return a tunnelling command that just needs a port."""
+        # zmq needs str in Python 3, but pexpect gives bytes
+        if hasattr(self.host, "decode"):
+            self.host = self.host.decode("utf-8")
+
+        # One connection can tunnel all the ports
+        ports_str = " ".join(
+            [
+                "-L 127.0.0.1:{{{port}}}:127.0.0.1:{{{port}}}" "".format(port=port)
+                for port in PORT_NAMES
+            ]
+        )
+
+        ssh = "ssh"
+
+        # Add all the gateway machines as an ssh chain
+        pre_ssh = []
+        for pre_host in self.tunnel_hosts or []:
+            if ":" in pre_host:
+                pre_host = pre_host.replace(":", " -p ")
+
+            pre_ssh.append(
+                "{ssh} {ports_str} {pre_host}".format(
+                    ssh=ssh, pre_host=pre_host, ports_str=ports_str
+                )
+            )
+
+        if ":" in self.host:
+            host = self.host.replace(":", " -p ")
+        else:
+            host = self.host
+
+        # Timeout is specified here, this should be longer than the checking
+        # interval
+        # .strip() to prevent leading spaces
+        tunnel_cmd = (
+            " ".join(pre_ssh)
+            + " "
+            + "{ssh} {ports_str} {host} sleep 600".format(
+                ssh=ssh, host=host, ports_str=ports_str
+            )
+        ).strip()
+
+        self.log.debug("Tunnel command: {0}".format(tunnel_cmd))
+        return tunnel_cmd
+
+
+def start_remote_kernel():
+    """
+    Read command line arguments and initialise a kernel.
+    """
+    # These will not face a user since they are interpreting the command from
+    # kernel the kernel.json
+    description = "This is the kernel launcher! Try '%(prog)s manage'..."
+    parser = argparse.ArgumentParser(description=description)
+    parser.add_argument("connection_info")
+    parser.add_argument("--interface", default="local")
+    parser.add_argument("--cpus", type=int, default=1)
+    parser.add_argument("--pe", default="smp")
+    parser.add_argument(
+        "--kernel_cmd", default="ipython kernel -f {host_connection_file}"
+    )
+    parser.add_argument("--workdir")
+    parser.add_argument("--host")
+    parser.add_argument("--precmd")
+    parser.add_argument("--launch-args")
+    parser.add_argument("--verbose", action="store_true")
+    parser.add_argument("--tunnel-hosts", nargs="+")
+    parser.add_argument("--launch-cmd")
+    parser.add_argument(
+        "--version",
+        "-V",
+        action="version",
+        version="Remote Jupyter kernel launcher (version {0}).\n\n"
+        "Use the '%(prog)s manage' subcommand for managing "
+        "kernels.".format(__version__),
+    )
+    args = parser.parse_args()
+
+    kernel = RemoteIKernel(
+        connection_info=args.connection_info,
+        interface=args.interface,
+        cpus=args.cpus,
+        pe=args.pe,
+        kernel_cmd=args.kernel_cmd,
+        workdir=args.workdir,
+        host=args.host,
+        precmd=args.precmd,
+        launch_args=args.launch_args,
+        verbose=args.verbose,
+        tunnel_hosts=args.tunnel_hosts,
+        launch_cmd=args.launch_cmd,
+    )
+    kernel.keep_alive()
```

### Comparing `remote_ipykernel-1.0.1/remote_ipykernel/manage.py` & `remote_ipykernel-1.0.2/remote_ipykernel/manage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,479 +1,479 @@
-"""
-manage.py
-
-Manage the kernels available to remote_ikernel.
-Run ``remote_ikernel manage`` to see a list of commands.
-
-"""
-
-from __future__ import print_function
-from __future__ import unicode_literals
-
-import argparse
-import getpass
-import json
-import os
-import re
-import shlex
-import sys
-from os import path
-from subprocess import list2cmdline
-
-# How we identify kernels that rik will manage
-from remote_ipykernel import RIK_PREFIX, __version__
-
-# These go through a compatibility layer to work with IPython and Jupyter
-from remote_ipykernel.compat import kernelspec as ks
-from remote_ipykernel.compat import tempdir
-
-# When Python 2 pipes into something else, there is no encoding
-# set. Assume that it is utf-8 so that scripttest works as expected.
-# If LANG=C, unicode characters will break output, but
-# https://bugs.python.org/issue19846 says it should not be an issue
-# on modern systems. And you can't put unicode in with LANG=C so how can
-# you expect unicode out?
-if sys.stdout.encoding is None:
-    # no recursive
-    _print = print
-
-    def print(x):
-        _print(x.encode("UTF-8"))
-
-    # From http://bugs.python.org/issue9779
-    def _print_message(self, message, file=None):
-        """Output message to file, encoded as UTF-8 """
-        if message:
-            if file is None:
-                file = sys.stderr
-            file.write(message.encode("UTF-8"))
-
-    argparse.ArgumentParser._print_message = _print_message
-
-
-def delete_kernel(kernel_name):
-    """
-    Delete the kernel by removing the kernel.json and directory.
-
-    Parameters
-    ----------
-    kernel_name : str
-        The name of the kernel to delete
-
-    Raises
-    ------
-    KeyError
-        If the kernel is not found.
-    """
-    spec = ks.get_kernel_spec(kernel_name)
-    os.remove(path.join(spec.resource_dir, "kernel.json"))
-    try:
-        os.rmdir(spec.resource_dir)
-    except OSError:
-        # Non empty directory, just leave it
-        pass
-
-
-def command_fix(kernel_command):
-    """
-    Check the command for anything that might cause upset when it gets run
-    by bash.
-
-    Current checks are:
-        IRkernel:main() needs escaping.
-        Warn for any brackets
-        Warn for unpaired quotes
-
-    Parameters
-    ----------
-    kernel_command : str
-        The kernel command that is run by bash.
-
-    Returns
-    -------
-    fixed_kernel_command : srt
-        The kernel command with any fixes applied.
-
-    """
-    # IRKernel:main() fix
-    # if not escaped or quoted then bash trips up on the brackets
-    if " IRkernel::main()" in kernel_command:
-        kernel_command = kernel_command.replace(
-            " IRkernel::main()", " 'IRkernel::main()'"
-        )
-        print("Escaping IRkernel::main().")
-
-    # Unescaped brackets
-    if re.search(r"[^\\][()]", kernel_command) and not re.search(
-        r"[\'\"].*[^\\][()].*[\'\"]", kernel_command
-    ):
-        print("Warning: possibly unescaped brackets in the kernel command.")
-
-    try:
-        shlex.split(kernel_command)
-    except ValueError:
-        print("Kernel command may be missing quotation marks.")
-
-    return kernel_command
-
-
-def show_kernel(kernel_name):
-    """
-    Print the contents of the kernel.json to the terminal, plus some extra
-    information.
-
-    Parameters
-    ----------
-    kernel_name : str
-        The name of the kernel to show the information for.
-    """
-    # Load the raw json, since we store some unexpected data in there too
-    spec = ks.get_kernel_spec(kernel_name)
-    with open(path.join(spec.resource_dir, "kernel.json")) as kernel_file:
-        kernel_json = json.load(kernel_file)
-
-    # Manually format the json to put each key: value on a single line
-    print("['{}']".format(kernel_name))
-    print("|  * Kernel found in: {0}".format(spec.resource_dir))
-    print("|  * Name: {0}".format(spec.display_name))
-    print("|  * Kernel command: {0}".format(list2cmdline(spec.argv)))
-    print(
-        "|  * remote_ikernel command: {0}".format(
-            list2cmdline(kernel_json["remote_ikernel_argv"])
-        )
-    )
-    print("|  * Raw json: {0}".format(json.dumps(kernel_json, indent=2)))
-    print("")
-
-
-def add_kernel(
-    interface,
-    name,
-    kernel_cmd,
-    cpus=1,
-    pe=None,
-    language=None,
-    system=False,
-    workdir=None,
-    host=None,
-    precmd=None,
-    launch_args=None,
-    tunnel_hosts=None,
-    verbose=False,
-    launch_cmd=None,
-):
-    """
-    Add a kernel. Generates a kernel.json and installs it for the system or
-    user.
-    """
-    kernel_name = []
-    display_name = []
-    argv = [sys.executable, "-m", "remote_ikernel"]
-
-    # How to connect to kernel
-    if interface == "local":
-        argv.extend(["--interface", "local"])
-        kernel_name.append("local")
-        display_name.append("Local")
-    elif interface == "pbs":
-        argv.extend(["--interface", "pbs"])
-        display_name.append("PBS")
-    elif interface == "sge":
-        argv.extend(["--interface", "sge"])
-        kernel_name.append("sge")
-        display_name.append("GridEngine")
-    elif interface == "sge_qrsh":
-        argv.extend(["--interface", "sge_qrsh"])
-        kernel_name.append("sge_qrsh")
-        display_name.append("GridEngine (qrsh)")
-    elif interface == "slurm":
-        argv.extend(["--interface", "slurm"])
-        kernel_name.append("slurm")
-        display_name.append("SLURM")
-    elif interface == "lsf":
-        argv.extend(["--interface", "lsf"])
-        kernel_name.append("lsf")
-        display_name.append("Platform LSF")
-    elif interface == "ssh":
-        if host is None:
-            raise KeyError("A host is required for ssh.")
-        argv.extend(["--interface", "ssh"])
-        argv.extend(["--host", host])
-        kernel_name.append("ssh")
-        kernel_name.append(host)
-        display_name.append("SSH")
-        display_name.append(host)
-    elif interface is None:
-        raise ValueError("interface must be specified")
-    else:
-        raise ValueError("Unknown interface {0}".format(interface))
-
-    if name is None:
-        raise ValueError("name is required for kernel")
-    display_name.append(name)
-    kernel_name.append(re.sub(r"\W", "", name).lower())
-
-    if launch_cmd is not None:
-        argv.extend(["--launch-cmd", launch_cmd])
-        display_name.append("({0})".format(launch_cmd))
-        kernel_name.append(re.sub(r"\W", "", launch_cmd).lower())
-
-    if pe is not None:
-        argv.extend(["--pe", pe])
-        kernel_name.append(pe)
-        display_name.append(pe)
-
-    if cpus and cpus > 1:
-        argv.extend(["--cpus", "{0}".format(cpus)])
-        kernel_name.append("{0}".format(cpus))
-        display_name.append("{0} CPUs".format(cpus))
-
-    if workdir is not None:
-        argv.extend(["--workdir", workdir])
-
-    if precmd is not None:
-        argv.extend(["--precmd", precmd])
-
-    if launch_args is not None:
-        argv.extend(["--launch-args", launch_args])
-
-    if tunnel_hosts:
-        # This will be a list of hosts
-        kernel_name.append("via_{0}".format("_".join(tunnel_hosts)))
-        display_name.append("(via {0})".format(" ".join(tunnel_hosts)))
-        argv.extend(["--tunnel-hosts"] + tunnel_hosts)
-
-    if verbose:
-        argv.extend(["--verbose"])
-
-    # protect the {connection_file} part of the kernel command
-    if kernel_cmd is None:
-        raise ValueError("kernel_cmd is required")
-    kernel_cmd = command_fix(kernel_cmd)
-    kernel_cmd = kernel_cmd.replace("{connection_file}", "{host_connection_file}")
-    argv.extend(["--kernel_cmd", kernel_cmd])
-
-    # remote_ikernel needs the connection file too
-    argv.append("{connection_file}")
-
-    # Prefix all kernels with 'rik_' for management.
-    kernel_name = RIK_PREFIX + "_".join(kernel_name)
-    # Having an @ in the string messes up the javascript;
-    # so get rid of evrything just in case.
-    kernel_name = re.sub(r"\W", "_", kernel_name)
-    kernel_json = {
-        "display_name": " ".join(display_name),
-        "argv": argv,
-    }
-
-    if language is not None:
-        kernel_json["language"] = language
-
-    # Put the commandline in so that '--show' will show how to recreate
-    # the kernel
-    kernel_json["remote_ikernel_argv"] = sys.argv
-
-    # False attempts a system install, otherwise install as the current user
-    if system:
-        username = False
-    else:
-        username = getpass.getuser()
-
-    # kernel.json file installation
-    with tempdir.TemporaryDirectory() as temp_dir:
-        os.chmod(temp_dir, 0o755)  # Starts off as 700, not user readable
-
-        with open(path.join(temp_dir, "kernel.json"), "w") as kernel_file:
-            json.dump(kernel_json, kernel_file, sort_keys=True, indent=2)
-
-        ks.install_kernel_spec(temp_dir, kernel_name, user=username, replace=True)
-
-    return kernel_name, " ".join(display_name)
-
-
-def manage():
-    """
-    Manage the available remote_ikernels.
-
-    All the options are pulled from arguments so we take no
-    arguments here.
-    """
-
-    description = [
-        "Remote IKernel management utility",
-        "",
-        "Currently installed kernels:",
-    ]
-    existing_kernels = {}
-
-    # Sort so they are always in the same order
-    for kernel_name in sorted(ks.find_kernel_specs()):
-        if kernel_name.startswith(RIK_PREFIX):
-            spec = ks.get_kernel_spec(kernel_name)
-            display = "  ['{kernel_name}']: {desc}".format(
-                kernel_name=kernel_name, desc=spec.display_name
-            )
-            existing_kernels[kernel_name] = spec
-            description.append(display)
-
-    # The raw formatter stops lines wrapping
-    parser = argparse.ArgumentParser(
-        prog="%prog manage",
-        description="\n".join(description),
-        formatter_class=argparse.RawTextHelpFormatter,
-    )
-    parser.add_argument(
-        "--show",
-        "-s",
-        nargs="*",
-        help="Print the contents of the kernel. "
-        "Specify a list of kernels, or leave blank to list all.",
-    )
-    parser.add_argument(
-        "--add",
-        "-a",
-        action="store_true",
-        help="Add a new kernel according to other commandline options.",
-    )
-    parser.add_argument(
-        "--delete",
-        "-d",
-        nargs="+",
-        help="Remove the kernel and delete the associated kernel.json.",
-    )
-    parser.add_argument("--kernel_cmd", "-k", help="Kernel command " "to install.")
-    parser.add_argument(
-        "--name", "-n", help="Name to identify the kernel, e.g. 'Python 2.7'."
-    )
-    parser.add_argument(
-        "--language", "-l", help="Explicitly specify the language of the kernel."
-    )
-    parser.add_argument(
-        "--cpus",
-        "-c",
-        type=int,
-        help="Launch the kernel as a multi-core job with this many cores if > 1.",
-    )
-    parser.add_argument(
-        "--pe", help="Parallel environment to use on when running on gridengine."
-    )
-    parser.add_argument(
-        "--host",
-        "-x",
-        help="The hostname or ip address running through an SSH connection. "
-        "For non standard ports use host:port.",
-    )
-    parser.add_argument(
-        "--interface",
-        "-i",
-        choices=["local", "ssh", "pbs", "sge", "sge_qrsh", "slurm", "lsf"],
-        help="Specify how the remote kernel is launched.",
-    )
-    parser.add_argument(
-        "--system",
-        help="Install the kernel into the system directory so that it is available "
-        "for all users. Might need admin privileges.",
-        action="store_true",
-    )
-    parser.add_argument(
-        "--workdir",
-        help="Directory in which to start the kernel. If not specified it "
-        "will use the current directory. This is important if the local "
-        "and remote filesystems differ.",
-    )
-    parser.add_argument(
-        "--remote-precmd",
-        help="Command to execute on the remote host before launching the kernel, "
-        "but after changing to the working directory.",
-    )
-    parser.add_argument(
-        "--launch-cmd",
-        help="Override the command used to launch the remote session "
-        "(e.g. 'qrsh' to replace 'qlogin') or provide the full path for the "
-        "executable if it is not in $PATH.",
-    )
-    parser.add_argument(
-        "--remote-launch-args",
-        help="Arguments to add to the command that launches the remote session, "
-        "i.e. the ssh or qlogin command, such as '-l h_rt=24:00:00' to "
-        "limit job time on GridEngine jobs.",
-    )
-    parser.add_argument(
-        "--tunnel-hosts",
-        "-t",
-        nargs="+",
-        help="Tunnel the connection through the given ssh hosts before "
-        "starting the endpoint interface. Works with any "
-        "interface. For non standard ports use host:port.",
-    )
-    parser.add_argument(
-        "--verbose",
-        "-v",
-        action="store_true",
-        help="Running kernel will produce verbose debugging on the console.",
-    )
-    parser.add_argument(
-        "--version",
-        "-V",
-        action="version",
-        version="Remote Jupyter kernel manager (version {0}).".format(__version__),
-    )
-
-    # Work on a copy so we don't mangle sys.argv when it is copied into
-    # the kernel json
-    raw_args = sys.argv[1:]
-    # give argparse something unicode to deal with for PY2
-    # otherwise, ignore if there is nothing to 'decode'
-    try:
-        raw_args = [x.decode("UTF-8") for x in sys.argv[1:]]
-    except AttributeError:
-        pass
-    args = parser.parse_args(raw_args)
-
-    if args.add:
-        kernel_name, display_name = add_kernel(
-            args.interface,
-            args.name,
-            args.kernel_cmd,
-            args.cpus,
-            args.pe,
-            args.language,
-            args.system,
-            args.workdir,
-            args.host,
-            args.remote_precmd,
-            args.remote_launch_args,
-            args.tunnel_hosts,
-            args.verbose,
-            args.launch_cmd,
-        )
-        print("Added kernel ['{0}']: {1}.".format(kernel_name, display_name))
-    elif args.delete:
-        undeleted = []
-        for to_delete in args.delete:
-            if to_delete in existing_kernels:
-                delete_kernel(to_delete)
-                print(
-                    "Removed kernel ['{0}']: {1}.".format(
-                        to_delete, existing_kernels[to_delete].display_name
-                    )
-                )
-            else:
-                undeleted.append(to_delete)
-        if undeleted:
-            print("Can't delete: {0}.".format(", ".join(undeleted)))
-            print("\n".join(description[2:]))
-            raise SystemExit(1)
-    elif args.show is not None:
-        unshowable = []
-        # Show all if none are specified
-        for to_show in args.show or existing_kernels:
-            if to_show in existing_kernels:
-                show_kernel(to_show)
-            else:
-                unshowable.append(to_show)
-        if unshowable:
-            print("Could not find: {0}.".format(", ".join(unshowable)))
-            print("\n".join(description[2:]))
-            raise SystemExit(1)
-    else:
-        parser.print_help()
+"""
+manage.py
+
+Manage the kernels available to remote_ikernel.
+Run ``remote_ikernel manage`` to see a list of commands.
+
+"""
+
+from __future__ import print_function
+from __future__ import unicode_literals
+
+import argparse
+import getpass
+import json
+import os
+import re
+import shlex
+import sys
+from os import path
+from subprocess import list2cmdline
+
+# How we identify kernels that rik will manage
+from remote_ipykernel import RIK_PREFIX, __version__
+
+# These go through a compatibility layer to work with IPython and Jupyter
+from remote_ipykernel.compat import kernelspec as ks
+from remote_ipykernel.compat import tempdir
+
+# When Python 2 pipes into something else, there is no encoding
+# set. Assume that it is utf-8 so that scripttest works as expected.
+# If LANG=C, unicode characters will break output, but
+# https://bugs.python.org/issue19846 says it should not be an issue
+# on modern systems. And you can't put unicode in with LANG=C so how can
+# you expect unicode out?
+if sys.stdout.encoding is None:
+    # no recursive
+    _print = print
+
+    def print(x):
+        _print(x.encode("UTF-8"))
+
+    # From http://bugs.python.org/issue9779
+    def _print_message(self, message, file=None):
+        """Output message to file, encoded as UTF-8 """
+        if message:
+            if file is None:
+                file = sys.stderr
+            file.write(message.encode("UTF-8"))
+
+    argparse.ArgumentParser._print_message = _print_message
+
+
+def delete_kernel(kernel_name):
+    """
+    Delete the kernel by removing the kernel.json and directory.
+
+    Parameters
+    ----------
+    kernel_name : str
+        The name of the kernel to delete
+
+    Raises
+    ------
+    KeyError
+        If the kernel is not found.
+    """
+    spec = ks.get_kernel_spec(kernel_name)
+    os.remove(path.join(spec.resource_dir, "kernel.json"))
+    try:
+        os.rmdir(spec.resource_dir)
+    except OSError:
+        # Non empty directory, just leave it
+        pass
+
+
+def command_fix(kernel_command):
+    """
+    Check the command for anything that might cause upset when it gets run
+    by bash.
+
+    Current checks are:
+        IRkernel:main() needs escaping.
+        Warn for any brackets
+        Warn for unpaired quotes
+
+    Parameters
+    ----------
+    kernel_command : str
+        The kernel command that is run by bash.
+
+    Returns
+    -------
+    fixed_kernel_command : srt
+        The kernel command with any fixes applied.
+
+    """
+    # IRKernel:main() fix
+    # if not escaped or quoted then bash trips up on the brackets
+    if " IRkernel::main()" in kernel_command:
+        kernel_command = kernel_command.replace(
+            " IRkernel::main()", " 'IRkernel::main()'"
+        )
+        print("Escaping IRkernel::main().")
+
+    # Unescaped brackets
+    if re.search(r"[^\\][()]", kernel_command) and not re.search(
+        r"[\'\"].*[^\\][()].*[\'\"]", kernel_command
+    ):
+        print("Warning: possibly unescaped brackets in the kernel command.")
+
+    try:
+        shlex.split(kernel_command)
+    except ValueError:
+        print("Kernel command may be missing quotation marks.")
+
+    return kernel_command
+
+
+def show_kernel(kernel_name):
+    """
+    Print the contents of the kernel.json to the terminal, plus some extra
+    information.
+
+    Parameters
+    ----------
+    kernel_name : str
+        The name of the kernel to show the information for.
+    """
+    # Load the raw json, since we store some unexpected data in there too
+    spec = ks.get_kernel_spec(kernel_name)
+    with open(path.join(spec.resource_dir, "kernel.json")) as kernel_file:
+        kernel_json = json.load(kernel_file)
+
+    # Manually format the json to put each key: value on a single line
+    print("['{}']".format(kernel_name))
+    print("|  * Kernel found in: {0}".format(spec.resource_dir))
+    print("|  * Name: {0}".format(spec.display_name))
+    print("|  * Kernel command: {0}".format(list2cmdline(spec.argv)))
+    print(
+        "|  * remote_ikernel command: {0}".format(
+            list2cmdline(kernel_json["remote_ikernel_argv"])
+        )
+    )
+    print("|  * Raw json: {0}".format(json.dumps(kernel_json, indent=2)))
+    print("")
+
+
+def add_kernel(
+    interface,
+    name,
+    kernel_cmd,
+    cpus=1,
+    pe=None,
+    language=None,
+    system=False,
+    workdir=None,
+    host=None,
+    precmd=None,
+    launch_args=None,
+    tunnel_hosts=None,
+    verbose=False,
+    launch_cmd=None,
+):
+    """
+    Add a kernel. Generates a kernel.json and installs it for the system or
+    user.
+    """
+    kernel_name = []
+    display_name = []
+    argv = [sys.executable, "-m", "remote_ipykernel"]
+
+    # How to connect to kernel
+    if interface == "local":
+        argv.extend(["--interface", "local"])
+        kernel_name.append("local")
+        display_name.append("Local")
+    elif interface == "pbs":
+        argv.extend(["--interface", "pbs"])
+        display_name.append("PBS")
+    elif interface == "sge":
+        argv.extend(["--interface", "sge"])
+        kernel_name.append("sge")
+        display_name.append("GridEngine")
+    elif interface == "sge_qrsh":
+        argv.extend(["--interface", "sge_qrsh"])
+        kernel_name.append("sge_qrsh")
+        display_name.append("GridEngine (qrsh)")
+    elif interface == "slurm":
+        argv.extend(["--interface", "slurm"])
+        kernel_name.append("slurm")
+        display_name.append("SLURM")
+    elif interface == "lsf":
+        argv.extend(["--interface", "lsf"])
+        kernel_name.append("lsf")
+        display_name.append("Platform LSF")
+    elif interface == "ssh":
+        if host is None:
+            raise KeyError("A host is required for ssh.")
+        argv.extend(["--interface", "ssh"])
+        argv.extend(["--host", host])
+        kernel_name.append("ssh")
+        kernel_name.append(host)
+        display_name.append("SSH")
+        display_name.append(host)
+    elif interface is None:
+        raise ValueError("interface must be specified")
+    else:
+        raise ValueError("Unknown interface {0}".format(interface))
+
+    if name is None:
+        raise ValueError("name is required for kernel")
+    display_name.append(name)
+    kernel_name.append(re.sub(r"\W", "", name).lower())
+
+    if launch_cmd is not None:
+        argv.extend(["--launch-cmd", launch_cmd])
+        display_name.append("({0})".format(launch_cmd))
+        kernel_name.append(re.sub(r"\W", "", launch_cmd).lower())
+
+    if pe is not None:
+        argv.extend(["--pe", pe])
+        kernel_name.append(pe)
+        display_name.append(pe)
+
+    if cpus and cpus > 1:
+        argv.extend(["--cpus", "{0}".format(cpus)])
+        kernel_name.append("{0}".format(cpus))
+        display_name.append("{0} CPUs".format(cpus))
+
+    if workdir is not None:
+        argv.extend(["--workdir", workdir])
+
+    if precmd is not None:
+        argv.extend(["--precmd", precmd])
+
+    if launch_args is not None:
+        argv.extend(["--launch-args", launch_args])
+
+    if tunnel_hosts:
+        # This will be a list of hosts
+        kernel_name.append("via_{0}".format("_".join(tunnel_hosts)))
+        display_name.append("(via {0})".format(" ".join(tunnel_hosts)))
+        argv.extend(["--tunnel-hosts"] + tunnel_hosts)
+
+    if verbose:
+        argv.extend(["--verbose"])
+
+    # protect the {connection_file} part of the kernel command
+    if kernel_cmd is None:
+        raise ValueError("kernel_cmd is required")
+    kernel_cmd = command_fix(kernel_cmd)
+    kernel_cmd = kernel_cmd.replace("{connection_file}", "{host_connection_file}")
+    argv.extend(["--kernel_cmd", kernel_cmd])
+
+    # remote_ikernel needs the connection file too
+    argv.append("{connection_file}")
+
+    # Prefix all kernels with 'rik_' for management.
+    kernel_name = RIK_PREFIX + "_".join(kernel_name)
+    # Having an @ in the string messes up the javascript;
+    # so get rid of evrything just in case.
+    kernel_name = re.sub(r"\W", "_", kernel_name)
+    kernel_json = {
+        "display_name": " ".join(display_name),
+        "argv": argv,
+    }
+
+    if language is not None:
+        kernel_json["language"] = language
+
+    # Put the commandline in so that '--show' will show how to recreate
+    # the kernel
+    kernel_json["remote_ikernel_argv"] = sys.argv
+
+    # False attempts a system install, otherwise install as the current user
+    if system:
+        username = False
+    else:
+        username = getpass.getuser()
+
+    # kernel.json file installation
+    with tempdir.TemporaryDirectory() as temp_dir:
+        os.chmod(temp_dir, 0o755)  # Starts off as 700, not user readable
+
+        with open(path.join(temp_dir, "kernel.json"), "w") as kernel_file:
+            json.dump(kernel_json, kernel_file, sort_keys=True, indent=2)
+
+        ks.install_kernel_spec(temp_dir, kernel_name, user=username, replace=True)
+
+    return kernel_name, " ".join(display_name)
+
+
+def manage():
+    """
+    Manage the available remote_ikernels.
+
+    All the options are pulled from arguments so we take no
+    arguments here.
+    """
+
+    description = [
+        "Remote IKernel management utility",
+        "",
+        "Currently installed kernels:",
+    ]
+    existing_kernels = {}
+
+    # Sort so they are always in the same order
+    for kernel_name in sorted(ks.find_kernel_specs()):
+        if kernel_name.startswith(RIK_PREFIX):
+            spec = ks.get_kernel_spec(kernel_name)
+            display = "  ['{kernel_name}']: {desc}".format(
+                kernel_name=kernel_name, desc=spec.display_name
+            )
+            existing_kernels[kernel_name] = spec
+            description.append(display)
+
+    # The raw formatter stops lines wrapping
+    parser = argparse.ArgumentParser(
+        prog="%prog manage",
+        description="\n".join(description),
+        formatter_class=argparse.RawTextHelpFormatter,
+    )
+    parser.add_argument(
+        "--show",
+        "-s",
+        nargs="*",
+        help="Print the contents of the kernel. "
+        "Specify a list of kernels, or leave blank to list all.",
+    )
+    parser.add_argument(
+        "--add",
+        "-a",
+        action="store_true",
+        help="Add a new kernel according to other commandline options.",
+    )
+    parser.add_argument(
+        "--delete",
+        "-d",
+        nargs="+",
+        help="Remove the kernel and delete the associated kernel.json.",
+    )
+    parser.add_argument("--kernel_cmd", "-k", help="Kernel command " "to install.")
+    parser.add_argument(
+        "--name", "-n", help="Name to identify the kernel, e.g. 'Python 2.7'."
+    )
+    parser.add_argument(
+        "--language", "-l", help="Explicitly specify the language of the kernel."
+    )
+    parser.add_argument(
+        "--cpus",
+        "-c",
+        type=int,
+        help="Launch the kernel as a multi-core job with this many cores if > 1.",
+    )
+    parser.add_argument(
+        "--pe", help="Parallel environment to use on when running on gridengine."
+    )
+    parser.add_argument(
+        "--host",
+        "-x",
+        help="The hostname or ip address running through an SSH connection. "
+        "For non standard ports use host:port.",
+    )
+    parser.add_argument(
+        "--interface",
+        "-i",
+        choices=["local", "ssh", "pbs", "sge", "sge_qrsh", "slurm", "lsf"],
+        help="Specify how the remote kernel is launched.",
+    )
+    parser.add_argument(
+        "--system",
+        help="Install the kernel into the system directory so that it is available "
+        "for all users. Might need admin privileges.",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--workdir",
+        help="Directory in which to start the kernel. If not specified it "
+        "will use the current directory. This is important if the local "
+        "and remote filesystems differ.",
+    )
+    parser.add_argument(
+        "--remote-precmd",
+        help="Command to execute on the remote host before launching the kernel, "
+        "but after changing to the working directory.",
+    )
+    parser.add_argument(
+        "--launch-cmd",
+        help="Override the command used to launch the remote session "
+        "(e.g. 'qrsh' to replace 'qlogin') or provide the full path for the "
+        "executable if it is not in $PATH.",
+    )
+    parser.add_argument(
+        "--remote-launch-args",
+        help="Arguments to add to the command that launches the remote session, "
+        "i.e. the ssh or qlogin command, such as '-l h_rt=24:00:00' to "
+        "limit job time on GridEngine jobs.",
+    )
+    parser.add_argument(
+        "--tunnel-hosts",
+        "-t",
+        nargs="+",
+        help="Tunnel the connection through the given ssh hosts before "
+        "starting the endpoint interface. Works with any "
+        "interface. For non standard ports use host:port.",
+    )
+    parser.add_argument(
+        "--verbose",
+        "-v",
+        action="store_true",
+        help="Running kernel will produce verbose debugging on the console.",
+    )
+    parser.add_argument(
+        "--version",
+        "-V",
+        action="version",
+        version="Remote Jupyter kernel manager (version {0}).".format(__version__),
+    )
+
+    # Work on a copy so we don't mangle sys.argv when it is copied into
+    # the kernel json
+    raw_args = sys.argv[1:]
+    # give argparse something unicode to deal with for PY2
+    # otherwise, ignore if there is nothing to 'decode'
+    try:
+        raw_args = [x.decode("UTF-8") for x in sys.argv[1:]]
+    except AttributeError:
+        pass
+    args = parser.parse_args(raw_args)
+
+    if args.add:
+        kernel_name, display_name = add_kernel(
+            args.interface,
+            args.name,
+            args.kernel_cmd,
+            args.cpus,
+            args.pe,
+            args.language,
+            args.system,
+            args.workdir,
+            args.host,
+            args.remote_precmd,
+            args.remote_launch_args,
+            args.tunnel_hosts,
+            args.verbose,
+            args.launch_cmd,
+        )
+        print("Added kernel ['{0}']: {1}.".format(kernel_name, display_name))
+    elif args.delete:
+        undeleted = []
+        for to_delete in args.delete:
+            if to_delete in existing_kernels:
+                delete_kernel(to_delete)
+                print(
+                    "Removed kernel ['{0}']: {1}.".format(
+                        to_delete, existing_kernels[to_delete].display_name
+                    )
+                )
+            else:
+                undeleted.append(to_delete)
+        if undeleted:
+            print("Can't delete: {0}.".format(", ".join(undeleted)))
+            print("\n".join(description[2:]))
+            raise SystemExit(1)
+    elif args.show is not None:
+        unshowable = []
+        # Show all if none are specified
+        for to_show in args.show or existing_kernels:
+            if to_show in existing_kernels:
+                show_kernel(to_show)
+            else:
+                unshowable.append(to_show)
+        if unshowable:
+            print("Could not find: {0}.".format(", ".join(unshowable)))
+            print("\n".join(description[2:]))
+            raise SystemExit(1)
+    else:
+        parser.print_help()
```

### Comparing `remote_ipykernel-1.0.1/remote_ipykernel.egg-info/SOURCES.txt` & `remote_ipykernel-1.0.2/remote_ipykernel.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-.gitignore
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
-tox.ini
-doc/kernels.png
 remote_ipykernel/__init__.py
+remote_ipykernel/__main__.py
 remote_ipykernel/__version.py
 remote_ipykernel/compat.py
 remote_ipykernel/kernel.py
 remote_ipykernel/manage.py
 remote_ipykernel.egg-info/PKG-INFO
 remote_ipykernel.egg-info/SOURCES.txt
 remote_ipykernel.egg-info/dependency_links.txt
```

### Comparing `remote_ipykernel-1.0.1/tests/test_cli.py` & `remote_ipykernel-1.0.2/tests/test_cli.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-# -*- coding: utf-8 -*-
-
-"""
-test_cli.py
-
-Check that the output of remote_ipykernel is as expected when run as a
-commandline script.
-
-"""
-
-import sys
-
-import pytest
-
-# pytest tries to include this if Test is kept in the name
-from scripttest import TestFileEnvironment as Env
-
-# Generic just for testing
-env = Env()
-
-
-def test_launcher_doing_nothing():
-    """Run without arguments."""
-    # This says error because there are no arguments -- that's fine.
-    result = env.run("remote_ipykernel", expect_error=True)
-    assert result.returncode != 0
-    # Help is useless, really
-    result = env.run("remote_ipykernel", "--help")
-    assert "usage: remote_ipykernel" in result.stdout
-
-
-def test_launcher_version():
-    """Launcher not manager."""
-    # version goes to stderr in PY2, stdout in PY3
-    result = env.run("remote_ipykernel", "-V", expect_stderr=True)
-    assert "Remote Jupyter kernel launcher" in result.stdout + result.stderr
-
-
-def test_manage_doing_nothing():
-    """Manage is different to the kernel itself."""
-    # Does not error. Gives help.
-    result = env.run("remote_ipykernel", "manage")
-    assert "usage" in result.stdout
-    result = env.run("remote_ipykernel", "manage", "--help")
-    assert "usage" in result.stdout
-
-
-def test_manage_basics():
-    result = env.run("remote_ipykernel", "manage", "-V", expect_stderr=True)
-    assert "Remote Jupyter kernel manager" in result.stdout + result.stderr
-    # Show will not error, even with no kernels
-    result = env.run("remote_ipykernel", "manage", "--show")
-
-
-def test_minimum_args():
-    # interface, kernel_cmd and name are required!
-    result = env.run(
-        "remote_ipykernel",
-        "manage",
-        "--add",
-        "--kernel_cmd=command",
-        "--name=name",
-        expect_error=True,
-    )
-    assert "interface must be specified" in result.stderr
-    result = env.run(
-        "remote_ipykernel",
-        "manage",
-        "--add",
-        "--interface=local",
-        "--name=name",
-        expect_error=True,
-    )
-    assert "kernel_cmd is required" in result.stderr
-    result = env.run(
-        "remote_ipykernel",
-        "manage",
-        "--add",
-        "--interface=local",
-        "--kernel_cmd=command",
-        expect_error=True,
-    )
-    assert "name is required for kernel" in result.stderr
-    result = env.run(
-        "remote_ipykernel",
-        "manage",
-        "--add",
-        "--interface=local",
-        "--kernel_cmd=command",
-        "--name=name",
-        expect_error=False,
-    )
-    assert "Added kernel" in result.stdout
-    result = env.run("remote_ipykernel", "manage", "--delete", "rik_local_name")
-    assert "Removed kernel" in result.stdout
-
-
-@pytest.mark.skipif(
-    sys.platform == "win32", reason="Unicode not working in windows terminal."
-)
-def test_unicode():
-    created = []
-    # Create a unicode containing kernel with unicode in every field possible
-    result = env.run(
-        "remote_ipykernel",
-        "manage",
-        "--add",
-        "--interface=local",
-        "--kernel_cmd=command ☂",
-        "--name=name ☂",
-        "--language=lang ☂",
-        "--pe=pe ☂",
-        "--host=host ☂",
-        "--workdir=dir ☂",
-        "--remote-precmd=pre ☂",
-        "--launch-cmd=launch ☂",
-        "--remote-launch-args=rla ☂",
-        "--tunnel-hosts=th ☂",
-    )
-    assert u"\u2602" in result.stdout
-    result = env.run("remote_ipykernel", "manage", "--show")
-    assert u"\u2602" in result.stdout
-    result = env.run(
-        "remote_ipykernel", "manage", "--delete", "rik_local_name_launch_pe___via_th__"
-    )
-    assert "Removed kernel" in result.stdout
+# -*- coding: utf-8 -*-
+
+"""
+test_cli.py
+
+Check that the output of remote_ipykernel is as expected when run as a
+commandline script.
+
+"""
+
+import sys
+
+import pytest
+
+# pytest tries to include this if Test is kept in the name
+from scripttest import TestFileEnvironment as Env
+
+# Generic just for testing
+env = Env()
+
+
+def test_launcher_doing_nothing():
+    """Run without arguments."""
+    # This says error because there are no arguments -- that's fine.
+    result = env.run("remote_ipykernel", expect_error=True)
+    assert result.returncode != 0
+    # Help is useless, really
+    result = env.run("remote_ipykernel", "--help")
+    assert "usage: remote_ipykernel" in result.stdout
+
+
+def test_launcher_version():
+    """Launcher not manager."""
+    # version goes to stderr in PY2, stdout in PY3
+    result = env.run("remote_ipykernel", "-V", expect_stderr=True)
+    assert "Remote Jupyter kernel launcher" in result.stdout + result.stderr
+
+
+def test_manage_doing_nothing():
+    """Manage is different to the kernel itself."""
+    # Does not error. Gives help.
+    result = env.run("remote_ipykernel", "manage")
+    assert "usage" in result.stdout
+    result = env.run("remote_ipykernel", "manage", "--help")
+    assert "usage" in result.stdout
+
+
+def test_manage_basics():
+    result = env.run("remote_ipykernel", "manage", "-V", expect_stderr=True)
+    assert "Remote Jupyter kernel manager" in result.stdout + result.stderr
+    # Show will not error, even with no kernels
+    result = env.run("remote_ipykernel", "manage", "--show")
+
+
+def test_minimum_args():
+    # interface, kernel_cmd and name are required!
+    result = env.run(
+        "remote_ipykernel",
+        "manage",
+        "--add",
+        "--kernel_cmd=command",
+        "--name=name",
+        expect_error=True,
+    )
+    assert "interface must be specified" in result.stderr
+    result = env.run(
+        "remote_ipykernel",
+        "manage",
+        "--add",
+        "--interface=local",
+        "--name=name",
+        expect_error=True,
+    )
+    assert "kernel_cmd is required" in result.stderr
+    result = env.run(
+        "remote_ipykernel",
+        "manage",
+        "--add",
+        "--interface=local",
+        "--kernel_cmd=command",
+        expect_error=True,
+    )
+    assert "name is required for kernel" in result.stderr
+    result = env.run(
+        "remote_ipykernel",
+        "manage",
+        "--add",
+        "--interface=local",
+        "--kernel_cmd=command",
+        "--name=name",
+        expect_error=False,
+    )
+    assert "Added kernel" in result.stdout
+    result = env.run("remote_ipykernel", "manage", "--delete", "rik_local_name")
+    assert "Removed kernel" in result.stdout
+
+
+@pytest.mark.skipif(
+    sys.platform == "win32", reason="Unicode not working in windows terminal."
+)
+def test_unicode():
+    created = []
+    # Create a unicode containing kernel with unicode in every field possible
+    result = env.run(
+        "remote_ipykernel",
+        "manage",
+        "--add",
+        "--interface=local",
+        "--kernel_cmd=command ☂",
+        "--name=name ☂",
+        "--language=lang ☂",
+        "--pe=pe ☂",
+        "--host=host ☂",
+        "--workdir=dir ☂",
+        "--remote-precmd=pre ☂",
+        "--launch-cmd=launch ☂",
+        "--remote-launch-args=rla ☂",
+        "--tunnel-hosts=th ☂",
+    )
+    assert u"\u2602" in result.stdout
+    result = env.run("remote_ipykernel", "manage", "--show")
+    assert u"\u2602" in result.stdout
+    result = env.run(
+        "remote_ipykernel", "manage", "--delete", "rik_local_name_launch_pe___via_th__"
+    )
+    assert "Removed kernel" in result.stdout
```

### Comparing `remote_ipykernel-1.0.1/tests/test_command_fix.py` & `remote_ipykernel-1.0.2/tests/test_command_fix.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-"""
-test_command_fix.py
-
-Check the special cases where the kernel command needs fixing up.
-
-"""
-
-from remote_ipykernel.manage import command_fix
-
-
-def test_irkernel_unescaped(capsys):
-    """Check that it gets escaped."""
-    kernel_command = (
-        "/usr/lib64/R/bin/R --slave -e IRkernel::main() --args {connection_file}"
-    )
-    fixed_kernel_command = (
-        "/usr/lib64/R/bin/R --slave -e 'IRkernel::main()' --args {connection_file}"
-    )
-    assert command_fix(kernel_command) != kernel_command
-    out, _err = capsys.readouterr()
-    assert "Escaping" in out
-    assert command_fix(kernel_command) == fixed_kernel_command
-
-
-def test_irkernel_already_escaped():
-    """Don't escape if it should already work."""
-    # single quotes
-    kernel_command = (
-        "/usr/lib64/R/bin/R --slave -e 'IRkernel::main()' --args {connection_file}"
-    )
-    assert command_fix(kernel_command) == kernel_command
-    # double quotes
-    kernel_command = (
-        '/usr/lib64/R/bin/R --slave -e "IRkernel::main()" --args {connection_file}'
-    )
-    assert command_fix(kernel_command) == kernel_command
-    # escaped
-    kernel_command = (
-        r"/usr/lib64/R/bin/R --slave -e IRkernel::main\(\) --args {connection_file}"
-    )
-    assert command_fix(kernel_command) == kernel_command
-
-
-def test_unescaped_brackets(capsys):
-    """Warn if there are brackets """
-    # unescaped cases
-    command_fix("one two three ( four five six")
-    out, _err = capsys.readouterr()
-    assert "unescaped brackets" in out
-
-    command_fix("one two three ) four five six")
-    out, _err = capsys.readouterr()
-    assert "unescaped brackets" in out
-
-    command_fix("one two three (\) four five six")
-    out, _err = capsys.readouterr()
-    assert "unescaped brackets" in out
-
-
-def test_escaped_brackets(capsys):
-    """Don't warn if it seems fine."""
-    # escaped cases
-    command_fix("one two three \(\) four five six")
-    out, _err = capsys.readouterr()
-    assert "unescaped brackets" not in out
-
-    command_fix("one two three '()' four five six")
-    out, _err = capsys.readouterr()
-    assert "unescaped brackets" not in out
-
-    command_fix('one two three "()" four five six')
-    out, _err = capsys.readouterr()
-    assert "unescaped brackets" not in out
-
-
-def test_missing_quotations(capsys):
-    """Warn if command seems broken."""
-    # Broken
-    command_fix("one two three ' four five six")
-    out, _err = capsys.readouterr()
-    assert "missing quotation marks" in out
-    command_fix('one two three " four five six')
-    out, _err = capsys.readouterr()
-    assert "missing quotation marks" in out
-    # Fine
-    command_fix("one two three ' four ' five six")
-    out, _err = capsys.readouterr()
-    assert "missing quotation marks" not in out
-    command_fix('one two three " four " five six')
-    out, _err = capsys.readouterr()
-    assert "missing quotation marks" not in out
-
-
-# Test when running from the commandline
-# pytest tries to include this if Test is kept in the name
-from scripttest import TestFileEnvironment as Env
-
-# Generic just for testing
-env = Env()
-
-
-def test_fix_in_manage():
-    # interface, kernel_cmd and name are required...
-    # Break kernel_cmd
-    result = env.run(
-        "remote_ipykernel",
-        "manage",
-        "--add",
-        "--interface=local",
-        "--kernel_cmd=something IRkernel::main()",
-        "--name=name",
-    )
-    assert "Escaping IRkernel" in result.stdout
-
-    result = env.run(
-        "remote_ipykernel",
-        "manage",
-        "--add",
-        "--interface=local",
-        "--kernel_cmd=something unescaped()",
-        "--name=name",
-    )
-    assert "unescaped brackets" in result.stdout
-
-    result = env.run(
-        "remote_ipykernel",
-        "manage",
-        "--add",
-        "--interface=local",
-        "--kernel_cmd=\"something badly quoted'",
-        "--name=name",
-    )
-    assert "missing quotation marks" in result.stdout
-
-    result = env.run("remote_ipykernel", "manage", "--delete", "rik_local_name")
-    assert "Removed kernel" in result.stdout
+"""
+test_command_fix.py
+
+Check the special cases where the kernel command needs fixing up.
+
+"""
+
+from remote_ipykernel.manage import command_fix
+
+
+def test_irkernel_unescaped(capsys):
+    """Check that it gets escaped."""
+    kernel_command = (
+        "/usr/lib64/R/bin/R --slave -e IRkernel::main() --args {connection_file}"
+    )
+    fixed_kernel_command = (
+        "/usr/lib64/R/bin/R --slave -e 'IRkernel::main()' --args {connection_file}"
+    )
+    assert command_fix(kernel_command) != kernel_command
+    out, _err = capsys.readouterr()
+    assert "Escaping" in out
+    assert command_fix(kernel_command) == fixed_kernel_command
+
+
+def test_irkernel_already_escaped():
+    """Don't escape if it should already work."""
+    # single quotes
+    kernel_command = (
+        "/usr/lib64/R/bin/R --slave -e 'IRkernel::main()' --args {connection_file}"
+    )
+    assert command_fix(kernel_command) == kernel_command
+    # double quotes
+    kernel_command = (
+        '/usr/lib64/R/bin/R --slave -e "IRkernel::main()" --args {connection_file}'
+    )
+    assert command_fix(kernel_command) == kernel_command
+    # escaped
+    kernel_command = (
+        r"/usr/lib64/R/bin/R --slave -e IRkernel::main\(\) --args {connection_file}"
+    )
+    assert command_fix(kernel_command) == kernel_command
+
+
+def test_unescaped_brackets(capsys):
+    """Warn if there are brackets """
+    # unescaped cases
+    command_fix("one two three ( four five six")
+    out, _err = capsys.readouterr()
+    assert "unescaped brackets" in out
+
+    command_fix("one two three ) four five six")
+    out, _err = capsys.readouterr()
+    assert "unescaped brackets" in out
+
+    command_fix("one two three (\) four five six")
+    out, _err = capsys.readouterr()
+    assert "unescaped brackets" in out
+
+
+def test_escaped_brackets(capsys):
+    """Don't warn if it seems fine."""
+    # escaped cases
+    command_fix("one two three \(\) four five six")
+    out, _err = capsys.readouterr()
+    assert "unescaped brackets" not in out
+
+    command_fix("one two three '()' four five six")
+    out, _err = capsys.readouterr()
+    assert "unescaped brackets" not in out
+
+    command_fix('one two three "()" four five six')
+    out, _err = capsys.readouterr()
+    assert "unescaped brackets" not in out
+
+
+def test_missing_quotations(capsys):
+    """Warn if command seems broken."""
+    # Broken
+    command_fix("one two three ' four five six")
+    out, _err = capsys.readouterr()
+    assert "missing quotation marks" in out
+    command_fix('one two three " four five six')
+    out, _err = capsys.readouterr()
+    assert "missing quotation marks" in out
+    # Fine
+    command_fix("one two three ' four ' five six")
+    out, _err = capsys.readouterr()
+    assert "missing quotation marks" not in out
+    command_fix('one two three " four " five six')
+    out, _err = capsys.readouterr()
+    assert "missing quotation marks" not in out
+
+
+# Test when running from the commandline
+# pytest tries to include this if Test is kept in the name
+from scripttest import TestFileEnvironment as Env
+
+# Generic just for testing
+env = Env()
+
+
+def test_fix_in_manage():
+    # interface, kernel_cmd and name are required...
+    # Break kernel_cmd
+    result = env.run(
+        "remote_ipykernel",
+        "manage",
+        "--add",
+        "--interface=local",
+        "--kernel_cmd=something IRkernel::main()",
+        "--name=name",
+    )
+    assert "Escaping IRkernel" in result.stdout
+
+    result = env.run(
+        "remote_ipykernel",
+        "manage",
+        "--add",
+        "--interface=local",
+        "--kernel_cmd=something unescaped()",
+        "--name=name",
+    )
+    assert "unescaped brackets" in result.stdout
+
+    result = env.run(
+        "remote_ipykernel",
+        "manage",
+        "--add",
+        "--interface=local",
+        "--kernel_cmd=\"something badly quoted'",
+        "--name=name",
+    )
+    assert "missing quotation marks" in result.stdout
+
+    result = env.run("remote_ipykernel", "manage", "--delete", "rik_local_name")
+    assert "Removed kernel" in result.stdout
```

### Comparing `remote_ipykernel-1.0.1/tests/test_extract_uuid.py` & `remote_ipykernel-1.0.2/tests/test_extract_uuid.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-"""
-test_extract_uuid.py
-
-Check that the uuid can be extracted from filenames when
-available.
-
-"""
-
-from uuid import UUID
-
-from remote_ipykernel.kernel import extract_uuid, RemoteIKernel
-
-
-def test_extract_uuid():
-    """Check that it gets the right one."""
-    this_uuid = UUID("fbbdec0f-1403-48c9-b2ae-b5b5e1572068")
-
-    full_path = (
-        "/home/user/.local/share/jupyter/runtime/"
-        "kernel-fbbdec0f-1403-48c9-b2ae-b5b5e1572068.json"
-    )
-    relative_path = (
-        "../../.local/share/jupyter/runtime/"
-        "kernel-fbbdec0f-1403-48c9-b2ae-b5b5e1572068.json"
-    )
-    no_path = "kernel-fbbdec0f-1403-48c9-b2ae-b5b5e1572068.json"
-
-    assert extract_uuid(full_path) == this_uuid
-    assert extract_uuid(relative_path) == this_uuid
-    assert extract_uuid(no_path) == this_uuid
-
-
-def test_no_uuid():
-    """Check that it gets nothing from these."""
-    full_path = "/home/user/.local/share/jupyter/runtime/" "kernel-not-a-uuid.json"
-    relative_path = "../../.local/share/jupyter/runtime/" "kernel-not-a-uuid.json"
-    no_path = "kernel-not-a-uuid.json"
-
-    assert extract_uuid(full_path) is None
-    assert extract_uuid(relative_path) is None
-    assert extract_uuid(no_path) is None
-
-
-def test_kernel_uuid():
-    """Check that any kernel gets a uuid."""
-    this_uuid = UUID("fbbdec0f-1403-48c9-b2ae-b5b5e1572068")
-    no_path = "kernel-fbbdec0f-1403-48c9-b2ae-b5b5e1572068.json"
-
-    test_kernel = RemoteIKernel(connection_info=no_path, interface="test")
-    assert test_kernel.uuid == this_uuid
-
-    test_kernel = RemoteIKernel(connection_info="not-a-uuid.json", interface="test")
-    assert test_kernel.uuid is not None
-    assert isinstance(test_kernel.uuid, UUID)
+"""
+test_extract_uuid.py
+
+Check that the uuid can be extracted from filenames when
+available.
+
+"""
+
+from uuid import UUID
+
+from remote_ipykernel.kernel import extract_uuid, RemoteIKernel
+
+
+def test_extract_uuid():
+    """Check that it gets the right one."""
+    this_uuid = UUID("fbbdec0f-1403-48c9-b2ae-b5b5e1572068")
+
+    full_path = (
+        "/home/user/.local/share/jupyter/runtime/"
+        "kernel-fbbdec0f-1403-48c9-b2ae-b5b5e1572068.json"
+    )
+    relative_path = (
+        "../../.local/share/jupyter/runtime/"
+        "kernel-fbbdec0f-1403-48c9-b2ae-b5b5e1572068.json"
+    )
+    no_path = "kernel-fbbdec0f-1403-48c9-b2ae-b5b5e1572068.json"
+
+    assert extract_uuid(full_path) == this_uuid
+    assert extract_uuid(relative_path) == this_uuid
+    assert extract_uuid(no_path) == this_uuid
+
+
+def test_no_uuid():
+    """Check that it gets nothing from these."""
+    full_path = "/home/user/.local/share/jupyter/runtime/" "kernel-not-a-uuid.json"
+    relative_path = "../../.local/share/jupyter/runtime/" "kernel-not-a-uuid.json"
+    no_path = "kernel-not-a-uuid.json"
+
+    assert extract_uuid(full_path) is None
+    assert extract_uuid(relative_path) is None
+    assert extract_uuid(no_path) is None
+
+
+def test_kernel_uuid():
+    """Check that any kernel gets a uuid."""
+    this_uuid = UUID("fbbdec0f-1403-48c9-b2ae-b5b5e1572068")
+    no_path = "kernel-fbbdec0f-1403-48c9-b2ae-b5b5e1572068.json"
+
+    test_kernel = RemoteIKernel(connection_info=no_path, interface="test")
+    assert test_kernel.uuid == this_uuid
+
+    test_kernel = RemoteIKernel(connection_info="not-a-uuid.json", interface="test")
+    assert test_kernel.uuid is not None
+    assert isinstance(test_kernel.uuid, UUID)
```

