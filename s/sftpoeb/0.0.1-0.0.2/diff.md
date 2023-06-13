# Comparing `tmp/sftpoeb-0.0.1.tar.gz` & `tmp/sftpoeb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.0.1.tar", last modified: Tue Jun 13 11:49:29 2023, max compression
+gzip compressed data, was "sftpoeb-0.0.2.tar", last modified: Tue Jun 13 11:50:18 2023, max compression
```

## Comparing `sftpoeb-0.0.1.tar` & `sftpoeb-0.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 11:49:29.865982 sftpoeb-0.0.1/
--rw-rw-rw-   0        0        0       81 2023-06-13 11:20:29.000000 sftpoeb-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      503 2023-06-13 11:49:29.864980 sftpoeb-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.0.1/README.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 11:49:29.865982 sftpoeb-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-06-13 11:49:19.000000 sftpoeb-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:49:29.784983 sftpoeb-0.0.1/sftpoeb/
--rw-rw-rw-   0        0        0      440 2023-06-13 11:20:13.000000 sftpoeb-0.0.1/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:49:29.833980 sftpoeb-0.0.1/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.0.1/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:49:29.835981 sftpoeb-0.0.1/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0     1489 2023-06-09 11:32:38.000000 sftpoeb-0.0.1/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:49:29.842980 sftpoeb-0.0.1/sftpoeb/method/
--rw-rw-rw-   0        0        0     4862 2023-06-09 11:32:38.000000 sftpoeb-0.0.1/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.0.1/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.0.1/sftpoeb/method/debug.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:49:29.767981 sftpoeb-0.0.1/sftpoeb/subclass/
-drwxrwxrwx   0        0        0        0 2023-06-13 11:49:29.847984 sftpoeb-0.0.1/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0     2889 2023-06-09 11:32:38.000000 sftpoeb-0.0.1/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.0.1/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:49:29.849982 sftpoeb-0.0.1/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0     1158 2023-06-09 11:32:38.000000 sftpoeb-0.0.1/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:49:29.851981 sftpoeb-0.0.1/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0     1167 2023-06-09 11:32:38.000000 sftpoeb-0.0.1/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:49:29.859981 sftpoeb-0.0.1/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0     4433 2023-06-09 11:32:38.000000 sftpoeb-0.0.1/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     3996 2023-06-09 11:32:38.000000 sftpoeb-0.0.1/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     1800 2023-06-09 11:32:38.000000 sftpoeb-0.0.1/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:49:29.862985 sftpoeb-0.0.1/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0    29074 2023-06-09 11:32:38.000000 sftpoeb-0.0.1/sftpoeb/subclass/process/s_c_process_package_1.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:49:29.831980 sftpoeb-0.0.1/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      503 2023-06-13 11:49:29.000000 sftpoeb-0.0.1/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      718 2023-06-13 11:49:29.000000 sftpoeb-0.0.1/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 11:49:29.000000 sftpoeb-0.0.1/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-13 11:49:29.000000 sftpoeb-0.0.1/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-13 11:49:29.000000 sftpoeb-0.0.1/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.300620 sftpoeb-0.0.2/
+-rw-rw-rw-   0        0        0       81 2023-06-13 11:20:29.000000 sftpoeb-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      503 2023-06-13 11:50:18.299619 sftpoeb-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.0.2/README.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 11:50:18.300620 sftpoeb-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-06-13 11:50:14.000000 sftpoeb-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.247623 sftpoeb-0.0.2/sftpoeb/
+-rw-rw-rw-   0        0        0      440 2023-06-13 11:20:13.000000 sftpoeb-0.0.2/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.269620 sftpoeb-0.0.2/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.271619 sftpoeb-0.0.2/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0     1489 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.278622 sftpoeb-0.0.2/sftpoeb/method/
+-rw-rw-rw-   0        0        0     4862 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      546 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/method/debug.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.231621 sftpoeb-0.0.2/sftpoeb/subclass/
+drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.282619 sftpoeb-0.0.2/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0     2889 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.285620 sftpoeb-0.0.2/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0     1158 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.287618 sftpoeb-0.0.2/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0     1167 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.294661 sftpoeb-0.0.2/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0     4433 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     3996 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     1800 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.297620 sftpoeb-0.0.2/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0    29074 2023-06-09 11:32:38.000000 sftpoeb-0.0.2/sftpoeb/subclass/process/s_c_process_package_1.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:50:18.267619 sftpoeb-0.0.2/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      503 2023-06-13 11:50:18.000000 sftpoeb-0.0.2/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      718 2023-06-13 11:50:18.000000 sftpoeb-0.0.2/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 11:50:18.000000 sftpoeb-0.0.2/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-13 11:50:18.000000 sftpoeb-0.0.2/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-13 11:50:18.000000 sftpoeb-0.0.2/sftpoeb.egg-info/top_level.txt
```

### Comparing `sftpoeb-0.0.1/LICENSE.txt` & `sftpoeb-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.1/setup.py` & `sftpoeb-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
         name='sftpoeb',
-        version='0.0.1',
+        version='0.0.2',
         url='',
         license='MIT',
         author='Natthawut Thawisombat',
         author_email='natthawut.th@inet.co.th',
         description='To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling',
         packages=find_packages(),
         long_description=open('README.txt').read() +  '\n\n' + open('CHANGELOG.txt').read(),
```

### Comparing `sftpoeb-0.0.1/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.0.2/sftpoeb/mainclass/c_sftp.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.1/sftpoeb/method/callservice.py` & `sftpoeb-0.0.2/sftpoeb/method/callservice.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.1/sftpoeb/method/checkpath.py` & `sftpoeb-0.0.2/sftpoeb/method/checkpath.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.1/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.0.2/sftpoeb/subclass/file/s_c_file.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.1/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.0.2/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.1/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.0.2/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.1/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.0.2/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.1/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.0.2/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.1/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.0.2/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.1/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.0.2/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.1/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.0.2/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.0.1/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.0.2/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

