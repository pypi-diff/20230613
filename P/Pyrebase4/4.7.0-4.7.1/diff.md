# Comparing `tmp/Pyrebase4-4.7.0.tar.gz` & `tmp/Pyrebase4-4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pyrebase4-4.7.0.tar", last modified: Sun May 14 14:18:54 2023, max compression
+gzip compressed data, was "Pyrebase4-4.7.1.tar", last modified: Tue Jun 13 18:20:27 2023, max compression
```

## Comparing `Pyrebase4-4.7.0.tar` & `Pyrebase4-4.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-05-14 14:18:54.042466 Pyrebase4-4.7.0/
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      412 2023-05-14 14:18:54.042466 Pyrebase4-4.7.0/PKG-INFO
-drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-05-14 14:18:54.042466 Pyrebase4-4.7.0/Pyrebase4.egg-info/
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      412 2023-05-14 14:18:54.000000 Pyrebase4-4.7.0/Pyrebase4.egg-info/PKG-INFO
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      294 2023-05-14 14:18:54.000000 Pyrebase4-4.7.0/Pyrebase4.egg-info/SOURCES.txt
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)        1 2023-05-14 14:18:54.000000 Pyrebase4-4.7.0/Pyrebase4.egg-info/dependency_links.txt
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      115 2023-05-14 14:18:54.000000 Pyrebase4-4.7.0/Pyrebase4.egg-info/requires.txt
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)        9 2023-05-14 14:18:54.000000 Pyrebase4-4.7.0/Pyrebase4.egg-info/top_level.txt
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)    13752 2023-05-14 14:05:14.000000 Pyrebase4-4.7.0/README.md
-drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-05-14 14:18:54.042466 Pyrebase4-4.7.0/pyrebase/
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       36 2022-11-30 18:49:25.000000 Pyrebase4-4.7.0/pyrebase/__init__.py
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)     5395 2022-11-30 18:49:25.000000 Pyrebase4-4.7.0/pyrebase/pyre_sseclient.py
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)    26616 2023-05-14 13:59:31.000000 Pyrebase4-4.7.0/pyrebase/pyrebase.py
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       38 2023-05-14 14:18:54.042466 Pyrebase4-4.7.0/setup.cfg
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      761 2023-05-14 14:18:28.000000 Pyrebase4-4.7.0/setup.py
-drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-05-14 14:18:54.042466 Pyrebase4-4.7.0/tests/
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)     5247 2022-11-30 18:49:25.000000 Pyrebase4-4.7.0/tests/test_database.py
--rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       95 2022-11-30 18:49:25.000000 Pyrebase4-4.7.0/tests/test_setup.py
+drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-06-13 18:20:27.215499 Pyrebase4-4.7.1/
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      412 2023-06-13 18:20:27.215499 Pyrebase4-4.7.1/PKG-INFO
+drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-06-13 18:20:27.215499 Pyrebase4-4.7.1/Pyrebase4.egg-info/
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      412 2023-06-13 18:20:27.000000 Pyrebase4-4.7.1/Pyrebase4.egg-info/PKG-INFO
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      294 2023-06-13 18:20:27.000000 Pyrebase4-4.7.1/Pyrebase4.egg-info/SOURCES.txt
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)        1 2023-06-13 18:20:27.000000 Pyrebase4-4.7.1/Pyrebase4.egg-info/dependency_links.txt
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      145 2023-06-13 18:20:27.000000 Pyrebase4-4.7.1/Pyrebase4.egg-info/requires.txt
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)        9 2023-06-13 18:20:27.000000 Pyrebase4-4.7.1/Pyrebase4.egg-info/top_level.txt
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)    13752 2023-05-14 14:05:14.000000 Pyrebase4-4.7.1/README.md
+drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-06-13 18:20:27.215499 Pyrebase4-4.7.1/pyrebase/
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       36 2022-11-30 18:49:25.000000 Pyrebase4-4.7.1/pyrebase/__init__.py
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)     5395 2022-11-30 18:49:25.000000 Pyrebase4-4.7.1/pyrebase/pyre_sseclient.py
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)    26616 2023-05-14 13:59:31.000000 Pyrebase4-4.7.1/pyrebase/pyrebase.py
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       38 2023-06-13 18:20:27.215499 Pyrebase4-4.7.1/setup.cfg
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)      802 2023-06-13 18:20:25.000000 Pyrebase4-4.7.1/setup.py
+drwxrwxr-x   0 nhorvath  (1001) nhorvath  (1001)        0 2023-06-13 18:20:27.215499 Pyrebase4-4.7.1/tests/
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)     5247 2022-11-30 18:49:25.000000 Pyrebase4-4.7.1/tests/test_database.py
+-rw-rw-r--   0 nhorvath  (1001) nhorvath  (1001)       95 2022-11-30 18:49:25.000000 Pyrebase4-4.7.1/tests/test_setup.py
```

### Comparing `Pyrebase4-4.7.0/README.md` & `Pyrebase4-4.7.1/README.md`

 * *Files identical despite different names*

### Comparing `Pyrebase4-4.7.0/pyrebase/pyre_sseclient.py` & `Pyrebase4-4.7.1/pyrebase/pyre_sseclient.py`

 * *Files identical despite different names*

### Comparing `Pyrebase4-4.7.0/pyrebase/pyrebase.py` & `Pyrebase4-4.7.1/pyrebase/pyrebase.py`

 * *Files identical despite different names*

### Comparing `Pyrebase4-4.7.0/setup.py` & `Pyrebase4-4.7.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Pyrebase4',
-    version='4.7.0',
+    version='4.7.1',
     url='https://github.com/nhorvath/Pyrebase4',
     description='A simple python wrapper for the Firebase API with current deps',
     author='nhorvath',
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.4',
     ],
     keywords='Firebase',
     packages=find_packages(exclude=['tests']),
     install_requires=[
-        'requests>=2.19.1',
-        'requests_toolbelt>=0.7.1',
+        'requests-toolbelt>=0.7.1,<1.0',
+        'requests>=2.19.1,<2.30',
+        'urllib3>=1.21.1,<2',
         'gcloud>=0.18.3',
         'oauth2client>=4.1.2',
         'python-jwt>=2.0.1',
         'pycryptodome>=3.6.4'
     ]
 )
```

### Comparing `Pyrebase4-4.7.0/tests/test_database.py` & `Pyrebase4-4.7.1/tests/test_database.py`

 * *Files identical despite different names*

