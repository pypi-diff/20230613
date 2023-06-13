# Comparing `tmp/bmw-lobster-0.9.3.tar.gz` & `tmp/bmw-lobster-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-0.9.3.tar", last modified: Tue May  9 09:58:22 2023, max compression
+gzip compressed data, was "bmw-lobster-0.9.4.tar", last modified: Tue Jun 13 09:18:58 2023, max compression
```

## Comparing `bmw-lobster-0.9.3.tar` & `bmw-lobster-0.9.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:22.188671 bmw-lobster-0.9.3/
--rw-r--r--   0 florian   (1000) florian   (1000)     1504 2023-05-09 09:58:22.188671 bmw-lobster-0.9.3/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      567 2023-05-08 15:03:18.000000 bmw-lobster-0.9.3/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:22.188671 bmw-lobster-0.9.3/bmw_lobster.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     1504 2023-05-09 09:58:22.000000 bmw-lobster-0.9.3/bmw_lobster.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      192 2023-05-09 09:58:22.000000 bmw-lobster-0.9.3/bmw_lobster.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-09 09:58:22.000000 bmw-lobster-0.9.3/bmw_lobster.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      223 2023-05-09 09:58:22.000000 bmw-lobster-0.9.3/bmw_lobster.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-09 09:58:22.000000 bmw-lobster-0.9.3/bmw_lobster.egg-info/top_level.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-09 09:58:22.188671 bmw-lobster-0.9.3/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2334 2023-05-08 15:03:18.000000 bmw-lobster-0.9.3/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:58.397266 bmw-lobster-0.9.4/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2079 2023-06-13 09:18:58.397266 bmw-lobster-0.9.4/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1142 2023-06-13 09:17:37.000000 bmw-lobster-0.9.4/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:58.397266 bmw-lobster-0.9.4/bmw_lobster.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2079 2023-06-13 09:18:58.000000 bmw-lobster-0.9.4/bmw_lobster.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      192 2023-06-13 09:18:58.000000 bmw-lobster-0.9.4/bmw_lobster.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-13 09:18:58.000000 bmw-lobster-0.9.4/bmw_lobster.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      223 2023-06-13 09:18:58.000000 bmw-lobster-0.9.4/bmw_lobster.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-13 09:18:58.000000 bmw-lobster-0.9.4/bmw_lobster.egg-info/top_level.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-13 09:18:58.397266 bmw-lobster-0.9.4/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2334 2023-06-13 09:17:37.000000 bmw-lobster-0.9.4/setup.py
```

### Comparing `bmw-lobster-0.9.3/setup.py` & `bmw-lobster-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Source Code"   : "%s/%s"        % (gh_root, gh_project),
 }
 
 packages = ["bmw-lobster-core>=%s" % version.LOBSTER_VERSION]
 for dirname in glob.glob("../lobster-tool-*"):
     packages.append("bmw-%s>=%s" % (os.path.basename(dirname),
                                     version.LOBSTER_VERSION))
-packages.append("miss-hit>=0.9.38")
+packages.append("miss-hit>=0.9.41")
 
 setuptools.setup(
     name="bmw-lobster",
     version=version.LOBSTER_VERSION,
     author="Bayerische Motoren Werke Aktiengesellschaft (BMW AG)",
     author_email="florian.schanda@bmw.de",
     description="Metapackage to install all LOBSTER Tools",
```

