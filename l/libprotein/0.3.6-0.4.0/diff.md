# Comparing `tmp/libprotein-0.3.6.tar.gz` & `tmp/libprotein-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libprotein-0.3.6.tar", last modified: Mon Jun 12 13:33:31 2023, max compression
+gzip compressed data, was "libprotein-0.4.0.tar", last modified: Tue Jun 13 07:57:33 2023, max compression
```

## Comparing `libprotein-0.3.6.tar` & `libprotein-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 teletchea-s (115022) ufip      (2000)        0 2023-06-12 13:33:31.964892 libprotein-0.3.6/
--rw-r--r--   0 teletchea-s (115022) ufip      (2000)        0 2022-06-21 08:06:33.000000 libprotein-0.3.6/MANIFEST.in
--rw-r--r--   0 teletchea-s (115022) ufip      (2000)      727 2023-06-12 13:33:31.964892 libprotein-0.3.6/PKG-INFO
--rw-r--r--   0 teletchea-s (115022) ufip      (2000)        0 2022-06-21 08:06:33.000000 libprotein-0.3.6/README.md
-drwxr-xr-x   0 teletchea-s (115022) ufip      (2000)        0 2023-06-12 13:33:31.964892 libprotein-0.3.6/libprotein/
--rw-r--r--   0 teletchea-s (115022) ufip      (2000)    18324 2022-08-26 07:31:36.000000 libprotein-0.3.6/libprotein/__init__.py
-drwxr-xr-x   0 teletchea-s (115022) ufip      (2000)        0 2023-06-12 13:33:31.964892 libprotein-0.3.6/libprotein.egg-info/
--rw-r--r--   0 teletchea-s (115022) ufip      (2000)      727 2023-06-12 13:33:31.000000 libprotein-0.3.6/libprotein.egg-info/PKG-INFO
--rw-r--r--   0 teletchea-s (115022) ufip      (2000)      189 2023-06-12 13:33:31.000000 libprotein-0.3.6/libprotein.egg-info/SOURCES.txt
--rw-r--r--   0 teletchea-s (115022) ufip      (2000)        1 2023-06-12 13:33:31.000000 libprotein-0.3.6/libprotein.egg-info/dependency_links.txt
--rw-r--r--   0 teletchea-s (115022) ufip      (2000)       11 2023-06-12 13:33:31.000000 libprotein-0.3.6/libprotein.egg-info/top_level.txt
--rw-r--r--   0 teletchea-s (115022) ufip      (2000)       38 2023-06-12 13:33:31.964892 libprotein-0.3.6/setup.cfg
--rw-r--r--   0 teletchea-s (115022) ufip      (2000)     1889 2022-08-26 12:05:45.000000 libprotein-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:57:33.940424 libprotein-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-13 07:57:33.940424 libprotein-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-13 07:57:30.000000 libprotein-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:57:33.940424 libprotein-0.4.0/libprotein/
+-rw-r--r--   0 runner    (1001) docker     (123)    16405 2023-06-13 07:57:31.000000 libprotein-0.4.0/libprotein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   544800 2023-06-13 07:57:32.000000 libprotein-0.4.0/libprotein/_libprotein.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:57:33.940424 libprotein-0.4.0/libprotein.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-13 07:57:33.000000 libprotein-0.4.0/libprotein.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-13 07:57:33.000000 libprotein-0.4.0/libprotein.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:57:33.000000 libprotein-0.4.0/libprotein.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 07:57:33.000000 libprotein-0.4.0/libprotein.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:57:33.940424 libprotein-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-13 07:57:30.000000 libprotein-0.4.0/setup.py
```

### Comparing `libprotein-0.3.6/setup.py` & `libprotein-0.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+# -*- coding: utf-8 -*-
+
 from setuptools import setup, dist
 from setuptools.command.install import install
 import os
 
+version = os.environ.get("PACKAGE_VERSION", "0.0.0")
+
 class BinaryDistribution(dist.Distribution):
     def has_ext_modules(foo):
         return True
 
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
@@ -18,36 +22,39 @@
         target = os.path.join(self.install_scripts, binary)
         if os.path.isfile(target):
             os.remove(target)
         self.copy_file(source, target)
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md')) as f:
-    long_description = f.read()
+    README = f.read()
 
 setup(
     name='libprotein',
-    package_data={'libprotein': ['_libprotein.so']},
-    version='0.3.6',
+    package_data={
+        "libprotein": ["_libprotein.so", "_libprotein.dylib", "_libprotein.dll"]
+    },
+    version='0.4.0',
     description="This module allows to parse existing data for qualifying a protein sequence in order to assess the sequence knowledge available in various databases.",
-    long_description=long_description,
+    long_description=README,
     long_description_content_type="text/markdown",
-    url='https://gitlab.univ-nantes.fr/teletchea-s/libprotein',
-    author='Hamady BA',
-    author_email='bhamadydemba@gmail.com',
+    url='https://github.com/TeletcheaLab/libprotein',
+    author='Matthieu E :: Hamady BA :: Sébastien Téletchéa',
+    author_email='stephane.teletchea@univ-nantes.fr',
     include_package_data=True,
     distclass=BinaryDistribution,
     cmdclass={'install': PostInstallCommand},
+    download_url="https://github.com/TeletcheaLab/libprotein/archive/refs/tags/v0.4.0.tar.gz",
     packages=['libprotein'],
     classifiers=[
+        'Operating System :: MacOS :: MacOS X',
+        'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: C++',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     keywords='protein post-translational modification, protein domain',
     project_urls={
         'GitLab': 'https://gitlab.univ-nantes.fr/teletchea-s/libprotein',
-        
+        'Github': 'https://github.com/TeletcheaLab/libprotein'
     },
-)
-
-
+)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

