# Comparing `tmp/pm20_3-0.973.tar.gz` & `tmp/pm20_3-0.974.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm20_3-0.973.tar", last modified: Tue Jun 13 08:55:47 2023, max compression
+gzip compressed data, was "pm20_3-0.974.tar", last modified: Tue Jun 13 09:09:32 2023, max compression
```

## Comparing `pm20_3-0.973.tar` & `pm20_3-0.974.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 08:55:47.817014 pm20_3-0.973/
--rw-rw-rw-   0        0        0      995 2023-06-13 08:55:47.817014 pm20_3-0.973/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 08:55:47.804043 pm20_3-0.973/pm20_3/
-drwxrwxrwx   0        0        0        0 2023-06-13 08:55:47.806033 pm20_3-0.973/pm20_3/Hello/
--rw-rw-rw-   0        0        0        0 2023-06-13 08:40:36.741068 pm20_3-0.973/pm20_3/Hello/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:55:47.807035 pm20_3-0.973/pm20_3/Hello/__pycache__/
--rw-rw-rw-   0        0        0      133 2023-06-13 08:49:22.214079 pm20_3-0.973/pm20_3/Hello/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0       12 2023-06-13 08:42:18.688746 pm20_3-0.973/pm20_3/Hello/file_1
--rw-rw-rw-   0        0        0       46 2023-06-12 21:19:50.670481 pm20_3-0.973/pm20_3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:55:47.809030 pm20_3-0.973/pm20_3/__pycache__/
--rw-rw-rw-   0        0        0      192 2023-06-13 08:49:22.211086 pm20_3-0.973/pm20_3/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1416 2023-06-13 08:53:12.323845 pm20_3-0.973/pm20_3/__pycache__/questions.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-06-13 08:55:47.816012 pm20_3-0.973/pm20_3/q/
--rw-rw-rw-   0        0        0        0 2023-06-12 21:04:56.293147 pm20_3-0.973/pm20_3/q/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:55:47.817014 pm20_3-0.973/pm20_3/q/__pycache__/
--rw-rw-rw-   0        0        0      129 2023-06-13 08:54:40.937163 pm20_3-0.973/pm20_3/q/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    24796 2023-06-11 23:13:18.000000 pm20_3-0.973/pm20_3/q/task_1.png
--rw-rw-rw-   0        0        0    26421 2023-06-11 23:13:18.000000 pm20_3-0.973/pm20_3/q/task_2.png
--rw-rw-rw-   0        0        0    25932 2023-06-11 23:13:18.000000 pm20_3-0.973/pm20_3/q/task_3.png
--rw-rw-rw-   0        0        0    25398 2023-06-11 23:13:18.000000 pm20_3-0.973/pm20_3/q/task_4.png
--rw-rw-rw-   0        0        0    26943 2023-06-11 23:13:18.000000 pm20_3-0.973/pm20_3/q/task_5.png
--rw-rw-rw-   0        0        0    10322 2023-06-11 23:13:18.000000 pm20_3-0.973/pm20_3/q/task_6.png
--rw-rw-rw-   0        0        0     1740 2023-06-13 08:55:25.568668 pm20_3-0.973/pm20_3/questions.py
--rw-rw-rw-   0        0        0       63 2023-06-12 17:51:03.693651 pm20_3-0.973/setup.cfg
--rw-rw-rw-   0        0        0     1916 2023-06-13 08:55:47.608096 pm20_3-0.973/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:09:32.847952 pm20_3-0.974/
+-rw-rw-rw-   0        0        0       26 2023-06-12 18:43:23.000000 pm20_3-0.974/MANIFEST.in
+-rw-rw-rw-   0        0        0      995 2023-06-13 09:09:32.848950 pm20_3-0.974/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-06-12 17:52:57.000000 pm20_3-0.974/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 09:09:32.815207 pm20_3-0.974/pm20_3/
+drwxrwxrwx   0        0        0        0 2023-06-13 09:09:32.825153 pm20_3-0.974/pm20_3/Hello/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:40:36.000000 pm20_3-0.974/pm20_3/Hello/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:09:32.827147 pm20_3-0.974/pm20_3/Hello/__pycache__/
+-rw-rw-rw-   0        0        0      133 2023-06-13 08:49:22.000000 pm20_3-0.974/pm20_3/Hello/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0       12 2023-06-13 08:42:18.000000 pm20_3-0.974/pm20_3/Hello/file_1
+-rw-rw-rw-   0        0        0       46 2023-06-12 21:19:50.000000 pm20_3-0.974/pm20_3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:09:32.830139 pm20_3-0.974/pm20_3/__pycache__/
+-rw-rw-rw-   0        0        0      192 2023-06-13 08:49:22.000000 pm20_3-0.974/pm20_3/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1416 2023-06-13 08:53:12.000000 pm20_3-0.974/pm20_3/__pycache__/questions.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-13 09:09:32.844960 pm20_3-0.974/pm20_3/q/
+-rw-rw-rw-   0        0        0        0 2023-06-12 21:04:56.000000 pm20_3-0.974/pm20_3/q/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:09:32.846955 pm20_3-0.974/pm20_3/q/__pycache__/
+-rw-rw-rw-   0        0        0      129 2023-06-13 08:54:40.000000 pm20_3-0.974/pm20_3/q/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    24796 2023-06-11 23:13:18.000000 pm20_3-0.974/pm20_3/q/task_1.png
+-rw-rw-rw-   0        0        0    26421 2023-06-11 23:13:18.000000 pm20_3-0.974/pm20_3/q/task_2.png
+-rw-rw-rw-   0        0        0    25932 2023-06-11 23:13:18.000000 pm20_3-0.974/pm20_3/q/task_3.png
+-rw-rw-rw-   0        0        0    25398 2023-06-11 23:13:18.000000 pm20_3-0.974/pm20_3/q/task_4.png
+-rw-rw-rw-   0        0        0    26943 2023-06-11 23:13:18.000000 pm20_3-0.974/pm20_3/q/task_5.png
+-rw-rw-rw-   0        0        0    10322 2023-06-11 23:13:18.000000 pm20_3-0.974/pm20_3/q/task_6.png
+-rw-rw-rw-   0        0        0     1740 2023-06-13 08:55:25.000000 pm20_3-0.974/pm20_3/questions.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:09:32.822160 pm20_3-0.974/pm20_3.egg-info/
+-rw-rw-rw-   0        0        0      995 2023-06-13 09:09:32.000000 pm20_3-0.974/pm20_3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2023-06-13 09:09:32.000000 pm20_3-0.974/pm20_3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:09:32.000000 pm20_3-0.974/pm20_3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-13 09:09:32.000000 pm20_3-0.974/pm20_3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 09:09:32.000000 pm20_3-0.974/pm20_3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 09:09:32.848950 pm20_3-0.974/setup.cfg
+-rw-rw-rw-   0        0        0     1912 2023-06-13 09:09:32.000000 pm20_3-0.974/setup.py
```

### Comparing `pm20_3-0.973/PKG-INFO` & `pm20_3-0.974/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pm20_3
-Version: 0.973
+Version: 0.974
 Summary: For cheating again..
 Home-page: http://www.fa.ru/Pages/Home.aspx
 Author: Anatoliy Nesterov
 Author-email: your.email@domain.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `pm20_3-0.973/pm20_3/__pycache__/questions.cpython-39.pyc` & `pm20_3-0.974/pm20_3/__pycache__/questions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pm20_3-0.973/pm20_3/q/task_1.png` & `pm20_3-0.974/pm20_3/q/task_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-0.973/pm20_3/q/task_2.png` & `pm20_3-0.974/pm20_3/q/task_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-0.973/pm20_3/q/task_3.png` & `pm20_3-0.974/pm20_3/q/task_3.png`

 * *Files identical despite different names*

### Comparing `pm20_3-0.973/pm20_3/q/task_4.png` & `pm20_3-0.974/pm20_3/q/task_4.png`

 * *Files identical despite different names*

### Comparing `pm20_3-0.973/pm20_3/q/task_5.png` & `pm20_3-0.974/pm20_3/q/task_5.png`

 * *Files identical despite different names*

### Comparing `pm20_3-0.973/pm20_3/q/task_6.png` & `pm20_3-0.974/pm20_3/q/task_6.png`

 * *Files identical despite different names*

### Comparing `pm20_3-0.973/pm20_3/questions.py` & `pm20_3-0.974/pm20_3/questions.py`

 * *Files identical despite different names*

### Comparing `pm20_3-0.973/setup.py` & `pm20_3-0.974/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from distutils.core import setup
+from setuptools import setup
 
 setup(
     name='pm20_3',  # How you named your package folder (MyLib)
     packages=['pm20_3'],  # Chose the same as "name"
-    version='0.973',  # Start with a small number and increase it with every change you make
+    version='0.974',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='For cheating again..',  # Give a short description about your library
     author='Anatoliy Nesterov',  # Type in your name
     author_email='your.email@domain.com',  # Type in your E-Mail
     url='http://www.fa.ru/Pages/Home.aspx',  # Provide either the link to your github or to your website
     download_url='https://github.com/user/reponame/archive/v_01.tar.gz',  # I explain this later on
     keywords=['CHEATING'],  # Keywords that define your package best
```

