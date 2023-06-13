# Comparing `tmp/easy-config-py-0.0.1.tar.gz` & `tmp/easy-config-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\demoApps\python\EasyConfig\dist\.tmp-2l70brds\easy-config-py-0.0.1.tar", last modified: Tue Jun 13 05:40:18 2023, max compression
+gzip compressed data, was "E:\demoApps\python\EasyConfig\dist\.tmp-abx5tcz4\easy-config-py-0.0.2.tar", last modified: Tue Jun 13 06:04:26 2023, max compression
```

## Comparing `easy-config-py-0.0.1.tar` & `easy-config-py-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 05:40:18.000000 easy-config-py-0.0.1/
--rw-rw-rw-   0        0        0     1595 2023-06-13 05:40:18.000000 easy-config-py-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-06-13 05:30:26.000000 easy-config-py-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 05:40:18.000000 easy-config-py-0.0.1/easy_config/
--rw-rw-rw-   0        0        0     5208 2023-06-13 03:11:11.000000 easy-config-py-0.0.1/easy_config/Dict.py
--rw-rw-rw-   0        0        0      195 2023-06-13 03:00:47.000000 easy-config-py-0.0.1/easy_config/__init__.py
--rw-rw-rw-   0        0        0     1439 2023-06-13 03:17:04.000000 easy-config-py-0.0.1/easy_config/config.py
--rw-rw-rw-   0        0        0     1421 2023-06-12 06:27:45.000000 easy-config-py-0.0.1/easy_config/file_loader.py
-drwxrwxrwx   0        0        0        0 2023-06-13 05:40:18.000000 easy-config-py-0.0.1/easy_config_py.egg-info/
--rw-rw-rw-   0        0        0     1595 2023-06-13 05:40:18.000000 easy-config-py-0.0.1/easy_config_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-06-13 05:40:18.000000 easy-config-py-0.0.1/easy_config_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 05:40:18.000000 easy-config-py-0.0.1/easy_config_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 05:40:18.000000 easy-config-py-0.0.1/easy_config_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 05:40:18.000000 easy-config-py-0.0.1/easy_config_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 05:40:18.000000 easy-config-py-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-06-13 05:39:53.000000 easy-config-py-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:04:26.000000 easy-config-py-0.0.2/
+-rw-rw-rw-   0        0        0     1595 2023-06-13 06:04:26.000000 easy-config-py-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1248 2023-06-13 05:30:26.000000 easy-config-py-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 06:04:26.000000 easy-config-py-0.0.2/easy_config/
+-rw-rw-rw-   0        0        0      232 2023-06-13 05:59:46.000000 easy-config-py-0.0.2/easy_config/__init__.py
+-rw-rw-rw-   0        0        0     5208 2023-06-13 03:11:11.000000 easy-config-py-0.0.2/easy_config/addict.py
+-rw-rw-rw-   0        0        0     1427 2023-06-13 05:59:58.000000 easy-config-py-0.0.2/easy_config/config.py
+-rw-rw-rw-   0        0        0     1421 2023-06-12 06:27:45.000000 easy-config-py-0.0.2/easy_config/file_loader.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:04:26.000000 easy-config-py-0.0.2/easy_config_py.egg-info/
+-rw-rw-rw-   0        0        0     1595 2023-06-13 06:04:26.000000 easy-config-py-0.0.2/easy_config_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-13 06:04:26.000000 easy-config-py-0.0.2/easy_config_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 06:04:26.000000 easy-config-py-0.0.2/easy_config_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 06:04:26.000000 easy-config-py-0.0.2/easy_config_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 06:04:26.000000 easy-config-py-0.0.2/easy_config_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 06:04:26.000000 easy-config-py-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      748 2023-06-13 06:01:24.000000 easy-config-py-0.0.2/setup.py
```

### Comparing `easy-config-py-0.0.1/PKG-INFO` & `easy-config-py-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-config-py
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/cookieGeGe/py_easy_config
 Author: cookieGeGe
 Author-email: zhang1114570651@gmail.com
 License: MIT
 Keywords: easy,config,addict,anyconfig
 Platform: any
 Requires-Python: >=3.6
```

### Comparing `easy-config-py-0.0.1/README.md` & `easy-config-py-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `easy-config-py-0.0.1/easy_config/Dict.py` & `easy-config-py-0.0.2/easy_config/addict.py`

 * *Files identical despite different names*

### Comparing `easy-config-py-0.0.1/easy_config/config.py` & `easy-config-py-0.0.2/easy_config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @File    : config.py
 # @Software: PyCharm
 import os.path
 
 import anyconfig
 
 from easy_config import Dict
-from easy_config.file_loader import FileLoader
+from easy_config import FileLoader
 
 
 class EasyConfig(object):
 
     def __init__(self, data=None, path=None, default_filename='config.yml'):
         self._d_ = Dict(data)
         if os.path.isfile(path):
```

### Comparing `easy-config-py-0.0.1/easy_config/file_loader.py` & `easy-config-py-0.0.2/easy_config/file_loader.py`

 * *Files identical despite different names*

### Comparing `easy-config-py-0.0.1/easy_config_py.egg-info/PKG-INFO` & `easy-config-py-0.0.2/easy_config_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-config-py
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/cookieGeGe/py_easy_config
 Author: cookieGeGe
 Author-email: zhang1114570651@gmail.com
 License: MIT
 Keywords: easy,config,addict,anyconfig
 Platform: any
 Requires-Python: >=3.6
```

### Comparing `easy-config-py-0.0.1/setup.py` & `easy-config-py-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='easy-config-py',
-    version='0.0.1',
+    version='0.0.2',
     packages=['easy_config'],
     install_requires=['anyconfig'],
     license='MIT',
     description='',
     author='cookieGeGe',
     author_email='zhang1114570651@gmail.com',
     keywords=['easy', 'config', 'addict', 'anyconfig'],
```

