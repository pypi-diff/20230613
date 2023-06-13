# Comparing `tmp/LambertProblem-0.4.tar.gz` & `tmp/LambertProblem-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LambertProblem-0.4.tar", last modified: Tue Jun 13 14:42:54 2023, max compression
+gzip compressed data, was "LambertProblem-0.5.tar", last modified: Tue Jun 13 15:54:01 2023, max compression
```

## Comparing `LambertProblem-0.4.tar` & `LambertProblem-0.5.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-13 14:42:54.254327 LambertProblem-0.4/
--rw-r--r--   0 juanita   (1000) juanita   (1000)     1134 2023-05-16 14:58:24.000000 LambertProblem-0.4/LICENSE
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-13 14:42:54.254327 LambertProblem-0.4/LambertProblem/
--rw-r--r--   0 juanita   (1000) juanita   (1000)     3349 2023-06-13 14:37:13.000000 LambertProblem-0.4/LambertProblem/__init__.py
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-13 14:42:54.254327 LambertProblem-0.4/LambertProblem.egg-info/
--rw-rw-r--   0 juanita   (1000) juanita   (1000)     2191 2023-06-13 14:42:54.000000 LambertProblem-0.4/LambertProblem.egg-info/PKG-INFO
--rw-rw-r--   0 juanita   (1000) juanita   (1000)      341 2023-06-13 14:42:54.000000 LambertProblem-0.4/LambertProblem.egg-info/SOURCES.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)        1 2023-06-13 14:42:54.000000 LambertProblem-0.4/LambertProblem.egg-info/dependency_links.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       51 2023-06-13 14:42:54.000000 LambertProblem-0.4/LambertProblem.egg-info/entry_points.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       12 2023-06-13 14:42:54.000000 LambertProblem-0.4/LambertProblem.egg-info/requires.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       23 2023-06-13 14:42:54.000000 LambertProblem-0.4/LambertProblem.egg-info/top_level.txt
--rw-rw-r--   0 juanita   (1000) juanita   (1000)     2191 2023-06-13 14:42:54.254327 LambertProblem-0.4/PKG-INFO
--rw-r--r--   0 juanita   (1000) juanita   (1000)     1675 2023-05-16 14:58:20.000000 LambertProblem-0.4/README.md
-drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-13 14:42:54.254327 LambertProblem-0.4/package/
--rw-r--r--   0 juanita   (1000) juanita   (1000)      500 2023-05-16 14:58:43.000000 LambertProblem-0.4/package/__init__.py
--rw-r--r--   0 juanita   (1000) juanita   (1000)     2174 2023-05-16 14:58:28.000000 LambertProblem-0.4/package/setup.py
--rw-r--r--   0 juanita   (1000) juanita   (1000)       96 2023-06-13 14:32:50.000000 LambertProblem-0.4/pyproject.toml
--rw-rw-r--   0 juanita   (1000) juanita   (1000)       38 2023-06-13 14:42:54.254327 LambertProblem-0.4/setup.cfg
--rw-r--r--   0 juanita   (1000) juanita   (1000)     2233 2023-06-13 14:32:17.000000 LambertProblem-0.4/setup.py
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-13 15:54:01.014512 LambertProblem-0.5/
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     1134 2023-05-16 14:58:24.000000 LambertProblem-0.5/LICENSE
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-13 15:54:01.014512 LambertProblem-0.5/LambertProblem/
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     7345 2023-06-13 15:43:44.000000 LambertProblem-0.5/LambertProblem/__init__.py
+drwxrwxr-x   0 juanita   (1000) juanita   (1000)        0 2023-06-13 15:54:01.014512 LambertProblem-0.5/LambertProblem.egg-info/
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)     2191 2023-06-13 15:54:00.000000 LambertProblem-0.5/LambertProblem.egg-info/PKG-INFO
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)      300 2023-06-13 15:54:00.000000 LambertProblem-0.5/LambertProblem.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)        1 2023-06-13 15:54:00.000000 LambertProblem-0.5/LambertProblem.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       51 2023-06-13 15:54:00.000000 LambertProblem-0.5/LambertProblem.egg-info/entry_points.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       12 2023-06-13 15:54:00.000000 LambertProblem-0.5/LambertProblem.egg-info/requires.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       15 2023-06-13 15:54:00.000000 LambertProblem-0.5/LambertProblem.egg-info/top_level.txt
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)     2191 2023-06-13 15:54:01.014512 LambertProblem-0.5/PKG-INFO
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     1675 2023-05-16 14:58:20.000000 LambertProblem-0.5/README.md
+-rw-r--r--   0 juanita   (1000) juanita   (1000)      115 2023-06-13 15:46:57.000000 LambertProblem-0.5/pyproject.toml
+-rw-rw-r--   0 juanita   (1000) juanita   (1000)       38 2023-06-13 15:54:01.014512 LambertProblem-0.5/setup.cfg
+-rw-r--r--   0 juanita   (1000) juanita   (1000)     2233 2023-06-13 15:46:33.000000 LambertProblem-0.5/setup.py
```

### Comparing `LambertProblem-0.4/LICENSE` & `LambertProblem-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `LambertProblem-0.4/LambertProblem.egg-info/PKG-INFO` & `LambertProblem-0.5/LambertProblem.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LambertProblem
-Version: 0.4
+Version: 0.5
 Summary: Solve the lambert problem for orbital mechanics
 Home-page: https://pypi.org/project/LambertProblem
 Author: juaniuwu
 Author-email: juanita.agudelo@udea.edu.co
 License: MIT
 Keywords: Lambert equation orbital mechanics solve
 Platform: UNKNOWN
```

### Comparing `LambertProblem-0.4/PKG-INFO` & `LambertProblem-0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LambertProblem
-Version: 0.4
+Version: 0.5
 Summary: Solve the lambert problem for orbital mechanics
 Home-page: https://pypi.org/project/LambertProblem
 Author: juaniuwu
 Author-email: juanita.agudelo@udea.edu.co
 License: MIT
 Keywords: Lambert equation orbital mechanics solve
 Platform: UNKNOWN
```

### Comparing `LambertProblem-0.4/README.md` & `LambertProblem-0.5/README.md`

 * *Files identical despite different names*

### Comparing `LambertProblem-0.4/package/setup.py` & `LambertProblem-0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # ######################################################################
     # BASIC DESCRIPTION
     # ######################################################################
-    name='pymiau',
-    author='Fulan@ de Tal',
-    author_email='fulano.de.tal@macondo.co',
-    description='Make a Miau',
+    name='LambertProblem',
+    author='juaniuwu',
+    author_email='juanita.agudelo@udea.edu.co',
+    description='Solve the lambert problem for orbital mechanics',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://pypi.org/project/pymiau',
-    keywords='Cats Dogs',
+    url='https://pypi.org/project/LambertProblem',
+    keywords='Lambert equation orbital mechanics solve',
     license='MIT',
 
     # ######################################################################
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.4',
+    version='0.5',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
     
@@ -45,15 +45,15 @@
     # ######################################################################
     test_suite='nose.collector',
     tests_require=['nose'],
 
     # ######################################################################
     # DEPENDENCIES
     # ######################################################################
-    install_requires=['scipy','ipython','matplotlib','tqdm'],
+    install_requires=['scipy','numpy'],
 
     # ######################################################################
     # OPTIONS
     # ######################################################################
     include_package_data=True,
     package_data={'': ['data/*.*', 'tests/*.*']},
 )
```

