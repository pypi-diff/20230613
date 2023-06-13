# Comparing `tmp/pm20_3-0.971.tar.gz` & `tmp/pm20_3-0.972.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm20_3-0.971.tar", last modified: Tue Jun 13 08:42:19 2023, max compression
+gzip compressed data, was "pm20_3-0.972.tar", last modified: Tue Jun 13 08:45:10 2023, max compression
```

## Comparing `pm20_3-0.971.tar` & `pm20_3-0.972.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 08:42:19.006896 pm20_3-0.971/
--rw-rw-rw-   0        0        0      995 2023-06-13 08:42:19.006896 pm20_3-0.971/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 08:42:18.993930 pm20_3-0.971/pm20_3/
-drwxrwxrwx   0        0        0        0 2023-06-13 08:42:18.995925 pm20_3-0.971/pm20_3/Hello/
--rw-rw-rw-   0        0        0        0 2023-06-13 08:40:36.741068 pm20_3-0.971/pm20_3/Hello/__init__.py
--rw-rw-rw-   0        0        0       12 2023-06-13 08:42:18.688746 pm20_3-0.971/pm20_3/Hello/file_1
--rw-rw-rw-   0        0        0       46 2023-06-12 21:19:50.670481 pm20_3-0.971/pm20_3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:42:18.998917 pm20_3-0.971/pm20_3/__pycache__/
--rw-rw-rw-   0        0        0      174 2023-06-12 16:52:57.741706 pm20_3-0.971/pm20_3/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      989 2023-06-12 16:52:56.543340 pm20_3-0.971/pm20_3/__pycache__/questions.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-06-13 08:42:19.006896 pm20_3-0.971/pm20_3/q/
--rw-rw-rw-   0        0        0        0 2023-06-12 21:04:56.293147 pm20_3-0.971/pm20_3/q/__init__.py
--rw-rw-rw-   0        0        0    24796 2023-06-11 23:13:18.000000 pm20_3-0.971/pm20_3/q/task_1.png
--rw-rw-rw-   0        0        0    26421 2023-06-11 23:13:18.000000 pm20_3-0.971/pm20_3/q/task_2.png
--rw-rw-rw-   0        0        0    25932 2023-06-11 23:13:18.000000 pm20_3-0.971/pm20_3/q/task_3.png
--rw-rw-rw-   0        0        0    25398 2023-06-11 23:13:18.000000 pm20_3-0.971/pm20_3/q/task_4.png
--rw-rw-rw-   0        0        0    26943 2023-06-11 23:13:18.000000 pm20_3-0.971/pm20_3/q/task_5.png
--rw-rw-rw-   0        0        0    10322 2023-06-11 23:13:18.000000 pm20_3-0.971/pm20_3/q/task_6.png
--rw-rw-rw-   0        0        0     1717 2023-06-13 08:42:18.693733 pm20_3-0.971/pm20_3/questions.py
--rw-rw-rw-   0        0        0       63 2023-06-12 17:51:03.693651 pm20_3-0.971/setup.cfg
--rw-rw-rw-   0        0        0     1916 2023-06-13 08:42:18.698719 pm20_3-0.971/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:45:10.960523 pm20_3-0.972/
+-rw-rw-rw-   0        0        0      995 2023-06-13 08:45:10.960523 pm20_3-0.972/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 08:45:10.948556 pm20_3-0.972/pm20_3/
+drwxrwxrwx   0        0        0        0 2023-06-13 08:45:10.950551 pm20_3-0.972/pm20_3/Hello/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:40:36.741068 pm20_3-0.972/pm20_3/Hello/__init__.py
+-rw-rw-rw-   0        0        0       12 2023-06-13 08:42:18.688746 pm20_3-0.972/pm20_3/Hello/file_1
+-rw-rw-rw-   0        0        0       46 2023-06-12 21:19:50.670481 pm20_3-0.972/pm20_3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:45:10.952569 pm20_3-0.972/pm20_3/__pycache__/
+-rw-rw-rw-   0        0        0      174 2023-06-12 16:52:57.741706 pm20_3-0.972/pm20_3/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      989 2023-06-12 16:52:56.543340 pm20_3-0.972/pm20_3/__pycache__/questions.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-13 08:45:10.959548 pm20_3-0.972/pm20_3/q/
+-rw-rw-rw-   0        0        0        0 2023-06-12 21:04:56.293147 pm20_3-0.972/pm20_3/q/__init__.py
+-rw-rw-rw-   0        0        0    24796 2023-06-11 23:13:18.000000 pm20_3-0.972/pm20_3/q/task_1.png
+-rw-rw-rw-   0        0        0    26421 2023-06-11 23:13:18.000000 pm20_3-0.972/pm20_3/q/task_2.png
+-rw-rw-rw-   0        0        0    25932 2023-06-11 23:13:18.000000 pm20_3-0.972/pm20_3/q/task_3.png
+-rw-rw-rw-   0        0        0    25398 2023-06-11 23:13:18.000000 pm20_3-0.972/pm20_3/q/task_4.png
+-rw-rw-rw-   0        0        0    26943 2023-06-11 23:13:18.000000 pm20_3-0.972/pm20_3/q/task_5.png
+-rw-rw-rw-   0        0        0    10322 2023-06-11 23:13:18.000000 pm20_3-0.972/pm20_3/q/task_6.png
+-rw-rw-rw-   0        0        0     1717 2023-06-13 08:42:18.693733 pm20_3-0.972/pm20_3/questions.py
+-rw-rw-rw-   0        0        0       63 2023-06-12 17:51:03.693651 pm20_3-0.972/setup.cfg
+-rw-rw-rw-   0        0        0     1916 2023-06-13 08:45:10.736864 pm20_3-0.972/setup.py
```

### Comparing `pm20_3-0.971/PKG-INFO` & `pm20_3-0.972/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pm20_3
-Version: 0.971
+Version: 0.972
 Summary: For cheating again..
 Home-page: http://www.fa.ru/Pages/Home.aspx
 Author: Anatoliy Nesterov
 Author-email: your.email@domain.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `pm20_3-0.971/pm20_3/__pycache__/questions.cpython-39.pyc` & `pm20_3-0.972/pm20_3/__pycache__/questions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pm20_3-0.971/pm20_3/q/task_1.png` & `pm20_3-0.972/pm20_3/q/task_1.png`

 * *Files identical despite different names*

### Comparing `pm20_3-0.971/pm20_3/q/task_2.png` & `pm20_3-0.972/pm20_3/q/task_2.png`

 * *Files identical despite different names*

### Comparing `pm20_3-0.971/pm20_3/q/task_3.png` & `pm20_3-0.972/pm20_3/q/task_3.png`

 * *Files identical despite different names*

### Comparing `pm20_3-0.971/pm20_3/q/task_4.png` & `pm20_3-0.972/pm20_3/q/task_4.png`

 * *Files identical despite different names*

### Comparing `pm20_3-0.971/pm20_3/q/task_5.png` & `pm20_3-0.972/pm20_3/q/task_5.png`

 * *Files identical despite different names*

### Comparing `pm20_3-0.971/pm20_3/q/task_6.png` & `pm20_3-0.972/pm20_3/q/task_6.png`

 * *Files identical despite different names*

### Comparing `pm20_3-0.971/pm20_3/questions.py` & `pm20_3-0.972/pm20_3/questions.py`

 * *Files identical despite different names*

### Comparing `pm20_3-0.971/setup.py` & `pm20_3-0.972/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='pm20_3',  # How you named your package folder (MyLib)
     packages=['pm20_3'],  # Chose the same as "name"
-    version='0.971',  # Start with a small number and increase it with every change you make
+    version='0.972',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='For cheating again..',  # Give a short description about your library
     author='Anatoliy Nesterov',  # Type in your name
     author_email='your.email@domain.com',  # Type in your E-Mail
     url='http://www.fa.ru/Pages/Home.aspx',  # Provide either the link to your github or to your website
     download_url='https://github.com/user/reponame/archive/v_01.tar.gz',  # I explain this later on
     keywords=['CHEATING'],  # Keywords that define your package best
```

