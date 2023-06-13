# Comparing `tmp/bkapi-plugins-py-0.612.tar.gz` & `tmp/bkapi-plugins-py-0.613.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkapi-plugins-py-0.612.tar", last modified: Mon Jun 12 01:39:23 2023, max compression
+gzip compressed data, was "bkapi-plugins-py-0.613.tar", last modified: Tue Jun 13 05:37:07 2023, max compression
```

## Comparing `bkapi-plugins-py-0.612.tar` & `bkapi-plugins-py-0.613.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 01:39:23.974073 bkapi-plugins-py-0.612/
--rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.612/MANIFEST.in
--rw-rw-rw-   0        0        0      257 2023-06-12 01:39:23.975069 bkapi-plugins-py-0.612/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 01:39:23.963109 bkapi-plugins-py-0.612/bkapi_plugins/
-drwxrwxrwx   0        0        0        0 2023-06-12 01:39:23.969089 bkapi-plugins-py-0.612/bkapi_plugins/files/
--rw-rw-rw-   0        0        0      683 2023-06-12 01:36:57.000000 bkapi-plugins-py-0.612/bkapi_plugins/files/io-monitor.sh
-drwxrwxrwx   0        0        0        0 2023-06-12 01:39:23.973077 bkapi-plugins-py-0.612/bkapi_plugins_py.egg-info/
--rw-rw-rw-   0        0        0      257 2023-06-12 01:39:23.000000 bkapi-plugins-py-0.612/bkapi_plugins_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-12 01:39:23.000000 bkapi-plugins-py-0.612/bkapi_plugins_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 01:39:23.000000 bkapi-plugins-py-0.612/bkapi_plugins_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 01:39:23.000000 bkapi-plugins-py-0.612/bkapi_plugins_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 01:39:23.977067 bkapi-plugins-py-0.612/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-06-12 01:37:24.000000 bkapi-plugins-py-0.612/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:37:07.841950 bkapi-plugins-py-0.613/
+-rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.613/MANIFEST.in
+-rw-rw-rw-   0        0        0      257 2023-06-13 05:37:07.841950 bkapi-plugins-py-0.613/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 05:37:07.827782 bkapi-plugins-py-0.613/bkapi_plugins/
+drwxrwxrwx   0        0        0        0 2023-06-13 05:37:07.833329 bkapi-plugins-py-0.613/bkapi_plugins/files/
+-rw-rw-rw-   0        0        0    22249 2023-06-13 05:30:17.000000 bkapi-plugins-py-0.613/bkapi_plugins/files/mongodb-7.3.0.tgz
+drwxrwxrwx   0        0        0        0 2023-06-13 05:37:07.839964 bkapi-plugins-py-0.613/bkapi_plugins_py.egg-info/
+-rw-rw-rw-   0        0        0      257 2023-06-13 05:37:07.000000 bkapi-plugins-py-0.613/bkapi_plugins_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-06-13 05:37:07.000000 bkapi-plugins-py-0.613/bkapi_plugins_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 05:37:07.000000 bkapi-plugins-py-0.613/bkapi_plugins_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 05:37:07.000000 bkapi-plugins-py-0.613/bkapi_plugins_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 05:37:07.844441 bkapi-plugins-py-0.613/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-06-13 05:35:49.000000 bkapi-plugins-py-0.613/setup.py
```

### Comparing `bkapi-plugins-py-0.612/setup.py` & `bkapi-plugins-py-0.613/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme = ''
 
 setup(
     description='',
     long_description=readme,
     name='bkapi-plugins-py', # 包的名字
-    version='0.612', # 版本号每次打包完要改一下
+    version='0.613', # 版本号每次打包完要改一下
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
     author='fadewalk',
     license='Apach License 2.0',
     # packages=find_packages(),
     # namespace_packages=['bkapi_plugins'],
     package_dir={'': '.'},
     include_package_data=True,
```

