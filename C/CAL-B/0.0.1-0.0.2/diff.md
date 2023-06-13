# Comparing `tmp/CAL-B-0.0.1.tar.gz` & `tmp/CAL-B-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CAL-B-0.0.1.tar", last modified: Tue Jun 13 10:49:11 2023, max compression
+gzip compressed data, was "CAL-B-0.0.2.tar", last modified: Tue Jun 13 11:24:14 2023, max compression
```

## Comparing `CAL-B-0.0.1.tar` & `CAL-B-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 swastik   (1000) swastik   (1001)        0 2023-06-13 10:49:11.750112 CAL-B-0.0.1/
-drwxr-xr-x   0 swastik   (1000) swastik   (1001)        0 2023-06-13 10:49:11.750112 CAL-B-0.0.1/CAL-B/
--rw-r--r--   0 swastik   (1000) swastik   (1001)      218 2023-06-13 09:41:01.000000 CAL-B-0.0.1/CAL-B/__init__.py
-drwxr-xr-x   0 swastik   (1000) swastik   (1001)        0 2023-06-13 10:49:11.750112 CAL-B-0.0.1/CAL_B.egg-info/
--rw-r--r--   0 swastik   (1000) swastik   (1001)      589 2023-06-13 10:49:11.000000 CAL-B-0.0.1/CAL_B.egg-info/PKG-INFO
--rw-r--r--   0 swastik   (1000) swastik   (1001)      191 2023-06-13 10:49:11.000000 CAL-B-0.0.1/CAL_B.egg-info/SOURCES.txt
--rw-r--r--   0 swastik   (1000) swastik   (1001)        1 2023-06-13 10:49:11.000000 CAL-B-0.0.1/CAL_B.egg-info/dependency_links.txt
--rw-r--r--   0 swastik   (1000) swastik   (1001)        6 2023-06-13 10:49:11.000000 CAL-B-0.0.1/CAL_B.egg-info/top_level.txt
--rw-r--r--   0 swastik   (1000) swastik   (1001)       73 2023-06-13 09:44:38.000000 CAL-B-0.0.1/CHANGELOG.txt
--rw-r--r--   0 swastik   (1000) swastik   (1001)     1061 2023-06-13 09:47:23.000000 CAL-B-0.0.1/LICENCE.txt
--rw-r--r--   0 swastik   (1000) swastik   (1001)       25 2023-06-13 09:45:58.000000 CAL-B-0.0.1/MANIFEST.in
--rw-r--r--   0 swastik   (1000) swastik   (1001)      589 2023-06-13 10:49:11.750112 CAL-B-0.0.1/PKG-INFO
--rw-r--r--   0 swastik   (1000) swastik   (1001)      137 2023-06-13 09:42:52.000000 CAL-B-0.0.1/README.txt
--rw-r--r--   0 swastik   (1000) swastik   (1001)       38 2023-06-13 10:49:11.750112 CAL-B-0.0.1/setup.cfg
--rw-r--r--   0 swastik   (1000) swastik   (1001)      620 2023-06-13 10:48:01.000000 CAL-B-0.0.1/setup.py
+drwxr-xr-x   0 swastik   (1000) swastik   (1001)        0 2023-06-13 11:24:14.251507 CAL-B-0.0.2/
+drwxr-xr-x   0 swastik   (1000) swastik   (1001)        0 2023-06-13 11:24:14.251507 CAL-B-0.0.2/CAL-B/
+-rw-r--r--   0 swastik   (1000) swastik   (1001)      218 2023-06-13 09:41:01.000000 CAL-B-0.0.2/CAL-B/__init__.py
+drwxr-xr-x   0 swastik   (1000) swastik   (1001)        0 2023-06-13 11:24:14.251507 CAL-B-0.0.2/CAL_B.egg-info/
+-rw-r--r--   0 swastik   (1000) swastik   (1001)      683 2023-06-13 11:24:14.000000 CAL-B-0.0.2/CAL_B.egg-info/PKG-INFO
+-rw-r--r--   0 swastik   (1000) swastik   (1001)      191 2023-06-13 11:24:14.000000 CAL-B-0.0.2/CAL_B.egg-info/SOURCES.txt
+-rw-r--r--   0 swastik   (1000) swastik   (1001)        1 2023-06-13 11:24:14.000000 CAL-B-0.0.2/CAL_B.egg-info/dependency_links.txt
+-rw-r--r--   0 swastik   (1000) swastik   (1001)        6 2023-06-13 11:24:14.000000 CAL-B-0.0.2/CAL_B.egg-info/top_level.txt
+-rw-r--r--   0 swastik   (1000) swastik   (1001)       73 2023-06-13 09:44:38.000000 CAL-B-0.0.2/CHANGELOG.txt
+-rw-r--r--   0 swastik   (1000) swastik   (1001)     1061 2023-06-13 09:47:23.000000 CAL-B-0.0.2/LICENCE.txt
+-rw-r--r--   0 swastik   (1000) swastik   (1001)       25 2023-06-13 09:45:58.000000 CAL-B-0.0.2/MANIFEST.in
+-rw-r--r--   0 swastik   (1000) swastik   (1001)      683 2023-06-13 11:24:14.251507 CAL-B-0.0.2/PKG-INFO
+-rw-r--r--   0 swastik   (1000) swastik   (1001)      137 2023-06-13 09:42:52.000000 CAL-B-0.0.2/README.txt
+-rw-r--r--   0 swastik   (1000) swastik   (1001)       38 2023-06-13 11:24:14.251507 CAL-B-0.0.2/setup.cfg
+-rw-r--r--   0 swastik   (1000) swastik   (1001)      741 2023-06-13 11:23:55.000000 CAL-B-0.0.2/setup.py
```

### Comparing `CAL-B-0.0.1/LICENCE.txt` & `CAL-B-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `CAL-B-0.0.1/setup.py` & `CAL-B-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,21 +4,24 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
 ]
     
 setup(
     name= 'CAL-B',
-    version= '0.0.1',
-    description= 'basiCALC- A basic Calculator python package',
+    version= '0.0.2',
+    description= 'CAL-B A basic Calculator Python Package',
     long_description= open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
-    url='',
+    url='https://github.com/swastkk/CAL-B',
+    project_urls= {
+        "Bug Tracker": "https://github.com/swastkk/CAL-B/issues"
+    },
     author= 'Swastik Sharma',
     author_email= 'swastkk@gmail.com',
     license= 'MIT',
     classifiers= classifiers,
     keywords= 'calculators',
     packages= find_packages(),
     install_requires= ['']
 
 
-)
+)
```

