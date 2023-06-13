# Comparing `tmp/buildrunner-3.0.753.tar.gz` & `tmp/buildrunner-3.0.756.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildrunner-3.0.753.tar", last modified: Thu Jun  8 22:28:55 2023, max compression
+gzip compressed data, was "buildrunner-3.0.756.tar", last modified: Tue Jun 13 01:31:25 2023, max compression
```

## Comparing `buildrunner-3.0.753.tar` & `buildrunner-3.0.756.tar`

### file list

```diff
@@ -1,56 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.680530 buildrunner-3.0.753/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-08 22:28:47.000000 buildrunner-3.0.753/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 22:28:47.000000 buildrunner-3.0.753/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    69064 2023-06-08 22:28:55.680530 buildrunner-3.0.753/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    57583 2023-06-08 22:28:47.000000 buildrunner-3.0.753/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.672530 buildrunner-3.0.753/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-06-08 22:28:47.000000 buildrunner-3.0.753/bin/buildrunner
--rwxr-xr-x   0 runner    (1001) docker     (123)      166 2023-06-08 22:28:47.000000 buildrunner-3.0.753/bin/buildrunner-cleanup
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/SourceDockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    27674 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/docker/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/docker/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/docker/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22485 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/docker/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/fetch/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/fetch/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/fetch/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/provisioners/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/provisioners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/provisioners/salt.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/provisioners/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/sshagent/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/sshagent/SSHAgentProxyImage/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)      212 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/sshagent/SSHAgentProxyImage/login.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      338 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/sshagent/SSHAgentProxyImage/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/sshagent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner/steprunner/
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.680530 buildrunner-3.0.753/buildrunner/steprunner/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/tasks/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/tasks/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/tasks/pypipush.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/tasks/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    43785 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/steprunner/tasks/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-08 22:28:47.000000 buildrunner-3.0.753/buildrunner/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 22:28:54.000000 buildrunner-3.0.753/buildrunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:28:55.676530 buildrunner-3.0.753/buildrunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    69064 2023-06-08 22:28:55.000000 buildrunner-3.0.753/buildrunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-08 22:28:55.000000 buildrunner-3.0.753/buildrunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:28:55.000000 buildrunner-3.0.753/buildrunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-08 22:28:55.000000 buildrunner-3.0.753/buildrunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 22:28:55.000000 buildrunner-3.0.753/buildrunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-08 22:28:47.000000 buildrunner-3.0.753/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 22:28:55.680530 buildrunner-3.0.753/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-08 22:28:47.000000 buildrunner-3.0.753/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-08 22:28:47.000000 buildrunner-3.0.753/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:31:25.819084 buildrunner-3.0.756/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-13 01:31:12.000000 buildrunner-3.0.756/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 01:31:12.000000 buildrunner-3.0.756/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    57840 2023-06-13 01:31:25.819084 buildrunner-3.0.756/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57583 2023-06-13 01:31:12.000000 buildrunner-3.0.756/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:31:25.807084 buildrunner-3.0.756/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-06-13 01:31:12.000000 buildrunner-3.0.756/bin/buildrunner
+-rwxr-xr-x   0 runner    (1001) docker     (123)      166 2023-06-13 01:31:12.000000 buildrunner-3.0.756/bin/buildrunner-cleanup
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:31:25.811084 buildrunner-3.0.756/buildrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/SourceDockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    27674 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15314 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:31:25.811084 buildrunner-3.0.756/buildrunner/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/docker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/docker/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/docker/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22485 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/docker/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:31:25.811084 buildrunner-3.0.756/buildrunner/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/fetch/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/fetch/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/fetch/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:31:25.815084 buildrunner-3.0.756/buildrunner/provisioners/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/provisioners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/provisioners/salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/provisioners/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:31:25.815084 buildrunner-3.0.756/buildrunner/sshagent/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:31:25.815084 buildrunner-3.0.756/buildrunner/sshagent/SSHAgentProxyImage/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)      212 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/sshagent/SSHAgentProxyImage/login.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      338 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/sshagent/SSHAgentProxyImage/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/sshagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:31:25.815084 buildrunner-3.0.756/buildrunner/steprunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/steprunner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:31:25.815084 buildrunner-3.0.756/buildrunner/steprunner/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/steprunner/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/steprunner/tasks/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/steprunner/tasks/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/steprunner/tasks/pypipush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/steprunner/tasks/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43785 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/steprunner/tasks/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-06-13 01:31:12.000000 buildrunner-3.0.756/buildrunner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 01:31:25.000000 buildrunner-3.0.756/buildrunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:31:25.811084 buildrunner-3.0.756/buildrunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    57840 2023-06-13 01:31:25.000000 buildrunner-3.0.756/buildrunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 01:31:25.000000 buildrunner-3.0.756/buildrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:31:25.000000 buildrunner-3.0.756/buildrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-13 01:31:25.000000 buildrunner-3.0.756/buildrunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 01:31:25.000000 buildrunner-3.0.756/buildrunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-13 01:31:12.000000 buildrunner-3.0.756/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-13 01:31:25.819084 buildrunner-3.0.756/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-13 01:31:12.000000 buildrunner-3.0.756/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-13 01:31:12.000000 buildrunner-3.0.756/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:31:25.819084 buildrunner-3.0.756/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-13 01:31:12.000000 buildrunner-3.0.756/tests/test_buildrunner_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-06-13 01:31:12.000000 buildrunner-3.0.756/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-13 01:31:12.000000 buildrunner-3.0.756/tests/test_console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-13 01:31:12.000000 buildrunner-3.0.756/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-13 01:31:12.000000 buildrunner-3.0.756/tests/test_push_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-13 01:31:12.000000 buildrunner-3.0.756/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-13 01:31:12.000000 buildrunner-3.0.756/tests/test_util_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-13 01:31:12.000000 buildrunner-3.0.756/tests/test_utils_flock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-13 01:31:12.000000 buildrunner-3.0.756/tests/test_version.py
```

### Comparing `buildrunner-3.0.753/LICENSE` & `buildrunner-3.0.756/LICENSE`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/README.rst` & `buildrunner-3.0.756/README.rst`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/__init__.py` & `buildrunner-3.0.756/buildrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/cli.py` & `buildrunner-3.0.756/buildrunner/cli.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/config.py` & `buildrunner-3.0.756/buildrunner/config.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/docker/__init__.py` & `buildrunner-3.0.756/buildrunner/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/docker/builder.py` & `buildrunner-3.0.756/buildrunner/docker/builder.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/docker/daemon.py` & `buildrunner-3.0.756/buildrunner/docker/daemon.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/docker/importer.py` & `buildrunner-3.0.756/buildrunner/docker/importer.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/docker/runner.py` & `buildrunner-3.0.756/buildrunner/docker/runner.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/errors.py` & `buildrunner-3.0.756/buildrunner/errors.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/fetch/__init__.py` & `buildrunner-3.0.756/buildrunner/fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/fetch/github.py` & `buildrunner-3.0.756/buildrunner/fetch/github.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/provisioners/__init__.py` & `buildrunner-3.0.756/buildrunner/provisioners/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/provisioners/salt.py` & `buildrunner-3.0.756/buildrunner/provisioners/salt.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/provisioners/shell.py` & `buildrunner-3.0.756/buildrunner/provisioners/shell.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile` & `buildrunner-3.0.756/buildrunner/sshagent/SSHAgentProxyImage/Dockerfile`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/sshagent/__init__.py` & `buildrunner-3.0.756/buildrunner/sshagent/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/steprunner/__init__.py` & `buildrunner-3.0.756/buildrunner/steprunner/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/steprunner/tasks/__init__.py` & `buildrunner-3.0.756/buildrunner/steprunner/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/steprunner/tasks/build.py` & `buildrunner-3.0.756/buildrunner/steprunner/tasks/build.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/steprunner/tasks/push.py` & `buildrunner-3.0.756/buildrunner/steprunner/tasks/push.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/steprunner/tasks/pypipush.py` & `buildrunner-3.0.756/buildrunner/steprunner/tasks/pypipush.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/steprunner/tasks/remote.py` & `buildrunner-3.0.756/buildrunner/steprunner/tasks/remote.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/steprunner/tasks/run.py` & `buildrunner-3.0.756/buildrunner/steprunner/tasks/run.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner/utils.py` & `buildrunner-3.0.756/buildrunner/utils.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/buildrunner.egg-info/requires.txt` & `buildrunner-3.0.756/buildrunner.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/requirements.txt` & `buildrunner-3.0.756/requirements.txt`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/setup.py` & `buildrunner-3.0.756/setup.py`

 * *Files identical despite different names*

### Comparing `buildrunner-3.0.753/test_requirements.txt` & `buildrunner-3.0.756/test_requirements.txt`

 * *Files identical despite different names*

