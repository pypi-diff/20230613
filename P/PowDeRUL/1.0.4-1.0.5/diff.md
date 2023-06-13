# Comparing `tmp/PowDeRUL-1.0.4.tar.gz` & `tmp/PowDeRUL-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PowDeRUL-1.0.4.tar", last modified: Fri Jun  2 09:28:46 2023, max compression
+gzip compressed data, was "PowDeRUL-1.0.5.tar", last modified: Fri Jun  2 09:35:31 2023, max compression
```

## Comparing `PowDeRUL-1.0.4.tar` & `PowDeRUL-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 09:28:46.380127 PowDeRUL-1.0.4/
--rw-------   0 runner    (1000) runner    (1000)     1060 2023-06-02 07:54:31.000000 PowDeRUL-1.0.4/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 09:28:46.380127 PowDeRUL-1.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 09:28:46.380127 PowDeRUL-1.0.4/PowDeRUL.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 09:28:46.000000 PowDeRUL-1.0.4/PowDeRUL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      200 2023-06-02 09:28:46.000000 PowDeRUL-1.0.4/PowDeRUL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 09:28:46.000000 PowDeRUL-1.0.4/PowDeRUL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      120 2023-06-02 09:28:46.000000 PowDeRUL-1.0.4/PowDeRUL.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 09:28:46.000000 PowDeRUL-1.0.4/PowDeRUL.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)     3909 2023-06-02 07:54:31.000000 PowDeRUL-1.0.4/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      429 2023-06-02 09:28:31.000000 PowDeRUL-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-02 09:28:46.380127 PowDeRUL-1.0.4/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      833 2023-06-02 09:28:18.000000 PowDeRUL-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 09:35:31.695715 PowDeRUL-1.0.5/
+-rw-------   0 runner    (1000) runner    (1000)     1060 2023-06-02 07:54:31.000000 PowDeRUL-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 09:35:31.695715 PowDeRUL-1.0.5/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)     3909 2023-06-02 07:54:31.000000 PowDeRUL-1.0.5/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 09:35:31.691715 PowDeRUL-1.0.5/function/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-02 09:35:31.695715 PowDeRUL-1.0.5/function/PowDeRUL.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      426 2023-06-02 09:35:31.000000 PowDeRUL-1.0.5/function/PowDeRUL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      245 2023-06-02 09:35:31.000000 PowDeRUL-1.0.5/function/PowDeRUL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 09:35:31.000000 PowDeRUL-1.0.5/function/PowDeRUL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      120 2023-06-02 09:35:31.000000 PowDeRUL-1.0.5/function/PowDeRUL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-02 09:35:31.000000 PowDeRUL-1.0.5/function/PowDeRUL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      429 2023-06-02 09:35:23.000000 PowDeRUL-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-02 09:35:31.695715 PowDeRUL-1.0.5/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      835 2023-06-02 09:35:17.000000 PowDeRUL-1.0.5/setup.py
```

### Comparing `PowDeRUL-1.0.4/LICENSE` & `PowDeRUL-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PowDeRUL-1.0.4/README.md` & `PowDeRUL-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `PowDeRUL-1.0.4/setup.py` & `PowDeRUL-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
+
 setup(
     name='PowDeRUL',
-    version='1.0.4',
+    version='1.0.5',
     description='Python package for calculating lifetime of components',
     author='PGarn',
     author_email='paul.garnier@ens-rennes.fr',
     url='https://github.com/PGarn/LifeTime',
-    packages=find_packages(),
-    package_data={
-        'PowDeRUL': ['function/*','example/*'],
-    },
+    packages=find_packages('function'),
+    package_dir={'': 'function'},
+    include_package_data=True,
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
     ],
     install_requires=[
```

