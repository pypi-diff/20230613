# Comparing `tmp/bpctl-test-1.3.2.tar.gz` & `tmp/bpctl-test-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpctl-test-1.3.2.tar", last modified: Tue Jun 13 04:57:48 2023, max compression
+gzip compressed data, was "bpctl-test-1.3.4.tar", last modified: Tue Jun 13 05:06:30 2023, max compression
```

## Comparing `bpctl-test-1.3.2.tar` & `bpctl-test-1.3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 04:57:48.596821 bpctl-test-1.3.2/
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)        0 2023-05-29 09:51:37.000000 bpctl-test-1.3.2/MANIFEST.in
--rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)      380 2023-06-13 04:57:48.596821 bpctl-test-1.3.2/PKG-INFO
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)       86 2023-05-29 09:51:37.000000 bpctl-test-1.3.2/README.md
-drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 04:57:48.592820 bpctl-test-1.3.2/bin/
--rwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)      122 2023-06-13 04:54:11.000000 bpctl-test-1.3.2/bin/bpctl
-drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 04:57:48.592820 bpctl-test-1.3.2/bpctl_test.egg-info/
--rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)      380 2023-06-13 04:57:48.000000 bpctl-test-1.3.2/bpctl_test.egg-info/PKG-INFO
--rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)      390 2023-06-13 04:57:48.000000 bpctl-test-1.3.2/bpctl_test.egg-info/SOURCES.txt
--rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)        1 2023-06-13 04:57:48.000000 bpctl-test-1.3.2/bpctl_test.egg-info/dependency_links.txt
--rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)        4 2023-06-13 04:57:48.000000 bpctl-test-1.3.2/bpctl_test.egg-info/top_level.txt
-drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 04:57:48.596821 bpctl-test-1.3.2/lib/
--rwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-12 07:35:49.000000 bpctl-test-1.3.2/lib/__init__.py
-drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 04:57:48.596821 bpctl-test-1.3.2/lib/bpctl/
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)        0 2023-05-29 09:51:37.000000 bpctl-test-1.3.2/lib/bpctl/__init__.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)      901 2023-05-29 10:05:57.000000 bpctl-test-1.3.2/lib/bpctl/authenticate.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     2777 2023-05-29 09:51:37.000000 bpctl-test-1.3.2/lib/bpctl/base.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     6909 2023-06-01 11:08:39.000000 bpctl-test-1.3.2/lib/bpctl/bp_manifest.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     1695 2023-05-30 12:33:17.000000 bpctl-test-1.3.2/lib/bpctl/bpctl.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)      457 2023-05-29 09:51:37.000000 bpctl-test-1.3.2/lib/bpctl/config.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     3341 2023-05-29 09:51:37.000000 bpctl-test-1.3.2/lib/bpctl/load_data.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)       51 2023-05-29 09:51:37.000000 bpctl-test-1.3.2/lib/bpctl/read_bp_yaml.py
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)        0 2023-05-29 09:51:37.000000 bpctl-test-1.3.2/lib/bpctl/utils.py
--rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)       38 2023-06-13 04:57:48.596821 bpctl-test-1.3.2/setup.cfg
--rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     1618 2023-06-13 04:57:45.000000 bpctl-test-1.3.2/setup.py
+drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 05:06:30.830433 bpctl-test-1.3.4/
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)        0 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/MANIFEST.in
+-rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)      380 2023-06-13 05:06:30.830433 bpctl-test-1.3.4/PKG-INFO
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)       86 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/README.md
+drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 05:06:30.826432 bpctl-test-1.3.4/bin/
+-rwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)      118 2023-06-13 05:06:03.000000 bpctl-test-1.3.4/bin/bpctl
+drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 05:06:30.830433 bpctl-test-1.3.4/bpctl_test.egg-info/
+-rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)      380 2023-06-13 05:06:30.000000 bpctl-test-1.3.4/bpctl_test.egg-info/PKG-INFO
+-rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)      390 2023-06-13 05:06:30.000000 bpctl-test-1.3.4/bpctl_test.egg-info/SOURCES.txt
+-rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)        1 2023-06-13 05:06:30.000000 bpctl-test-1.3.4/bpctl_test.egg-info/dependency_links.txt
+-rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)        4 2023-06-13 05:06:30.000000 bpctl-test-1.3.4/bpctl_test.egg-info/top_level.txt
+drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 05:06:30.830433 bpctl-test-1.3.4/lib/
+-rwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-12 07:35:49.000000 bpctl-test-1.3.4/lib/__init__.py
+drwxrwxr-x   0 vboxuser  (1000) vboxuser  (1000)        0 2023-06-13 05:06:30.830433 bpctl-test-1.3.4/lib/bpctl/
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)        0 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/lib/bpctl/__init__.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)      901 2023-05-29 10:05:57.000000 bpctl-test-1.3.4/lib/bpctl/authenticate.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     2777 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/lib/bpctl/base.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     6909 2023-06-01 11:08:39.000000 bpctl-test-1.3.4/lib/bpctl/bp_manifest.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     1695 2023-05-30 12:33:17.000000 bpctl-test-1.3.4/lib/bpctl/bpctl.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)      457 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/lib/bpctl/config.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     3341 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/lib/bpctl/load_data.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)       51 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/lib/bpctl/read_bp_yaml.py
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)        0 2023-05-29 09:51:37.000000 bpctl-test-1.3.4/lib/bpctl/utils.py
+-rw-rw-r--   0 vboxuser  (1000) vboxuser  (1000)       38 2023-06-13 05:06:30.830433 bpctl-test-1.3.4/setup.cfg
+-rwxrwxrwx   0 vboxuser  (1000) vboxuser  (1000)     1618 2023-06-13 05:05:57.000000 bpctl-test-1.3.4/setup.py
```

### Comparing `bpctl-test-1.3.2/lib/bpctl/authenticate.py` & `bpctl-test-1.3.4/lib/bpctl/authenticate.py`

 * *Files identical despite different names*

### Comparing `bpctl-test-1.3.2/lib/bpctl/base.py` & `bpctl-test-1.3.4/lib/bpctl/base.py`

 * *Files identical despite different names*

### Comparing `bpctl-test-1.3.2/lib/bpctl/bp_manifest.py` & `bpctl-test-1.3.4/lib/bpctl/bp_manifest.py`

 * *Files identical despite different names*

### Comparing `bpctl-test-1.3.2/lib/bpctl/bpctl.py` & `bpctl-test-1.3.4/lib/bpctl/bpctl.py`

 * *Files identical despite different names*

### Comparing `bpctl-test-1.3.2/lib/bpctl/load_data.py` & `bpctl-test-1.3.4/lib/bpctl/load_data.py`

 * *Files identical despite different names*

### Comparing `bpctl-test-1.3.2/setup.py` & `bpctl-test-1.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 
 setuptools.setup(
     name="bpctl-test",
-    version="1.3.2",
+    version="1.3.4",
     author="BP Team",
     author_email="shikhar.maheshwari@opstree.com",
     description="It is private package of bpctl",
     url="https://bitbucket.org/okts/bpctl/src/",
     packages=setuptools.find_packages(),
     include_package_data=True,
     scripts=['bin/bpctl'],
```

