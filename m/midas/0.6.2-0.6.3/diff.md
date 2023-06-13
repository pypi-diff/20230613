# Comparing `tmp/midas-0.6.2.tar.gz` & `tmp/midas-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-0.6.2.tar", last modified: Mon Jun  5 20:56:39 2023, max compression
+gzip compressed data, was "midas-0.6.3.tar", last modified: Tue Jun 13 17:55:24 2023, max compression
```

## Comparing `midas-0.6.2.tar` & `midas-0.6.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 20:56:39.407750 midas-0.6.2/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-04-25 18:49:18.000000 midas-0.6.2/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-10 19:06:41.000000 midas-0.6.2/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3269 2023-06-05 20:56:39.407813 midas-0.6.2/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2376 2023-03-10 04:22:14.000000 midas-0.6.2/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 20:56:39.406760 midas-0.6.2/midas/
--rw-r--r--   0 a.ruddick   (502) staff       (20)      993 2023-06-02 19:43:38.000000 midas-0.6.2/midas/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5904 2023-05-01 20:34:55.000000 midas-0.6.2/midas/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     4028 2021-06-30 14:46:51.000000 midas-0.6.2/midas/faults.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1889 2023-06-05 20:43:02.000000 midas-0.6.2/midas/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-05-01 20:34:55.000000 midas-0.6.2/midas/py.typed
--rw-r--r--   0 a.ruddick   (502) staff       (20)     6137 2023-06-05 20:43:02.000000 midas-0.6.2/midas/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 20:56:39.407650 midas-0.6.2/midas.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3269 2023-06-05 20:56:39.000000 midas-0.6.2/midas.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      317 2023-06-05 20:56:39.000000 midas-0.6.2/midas.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-06-05 20:56:39.000000 midas-0.6.2/midas.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       45 2023-06-05 20:56:39.000000 midas-0.6.2/midas.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      207 2023-06-05 20:56:39.000000 midas-0.6.2/midas.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        6 2023-06-05 20:56:39.000000 midas-0.6.2/midas.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      252 2023-06-05 20:56:39.408040 midas-0.6.2/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1825 2023-06-05 20:56:20.000000 midas-0.6.2/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-13 17:55:24.282996 midas-0.6.3/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-04-25 18:49:18.000000 midas-0.6.3/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-10 19:06:41.000000 midas-0.6.3/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3269 2023-06-13 17:55:24.283079 midas-0.6.3/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2376 2023-03-10 04:22:14.000000 midas-0.6.3/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-13 17:55:24.281435 midas-0.6.3/midas/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      993 2023-06-02 19:43:38.000000 midas-0.6.3/midas/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5904 2023-05-01 20:34:55.000000 midas-0.6.3/midas/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     4028 2021-06-30 14:46:51.000000 midas-0.6.3/midas/faults.csv
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1889 2023-06-05 20:43:02.000000 midas-0.6.3/midas/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-05-01 20:34:55.000000 midas-0.6.3/midas/py.typed
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     6030 2023-06-13 17:47:50.000000 midas-0.6.3/midas/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-13 17:55:24.282826 midas-0.6.3/midas.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3269 2023-06-13 17:55:24.000000 midas-0.6.3/midas.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      317 2023-06-13 17:55:24.000000 midas-0.6.3/midas.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-06-13 17:55:24.000000 midas-0.6.3/midas.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       45 2023-06-13 17:55:24.000000 midas-0.6.3/midas.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      207 2023-06-13 17:55:24.000000 midas-0.6.3/midas.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        6 2023-06-13 17:55:24.000000 midas-0.6.3/midas.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      252 2023-06-13 17:55:24.283429 midas-0.6.3/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1825 2023-06-13 17:54:47.000000 midas-0.6.3/setup.py
```

### Comparing `midas-0.6.2/LICENSE` & `midas-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-0.6.2/PKG-INFO` & `midas-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python driver for Honeywell Midas gas detectors.
 Home-page: https://github.com/numat/midas/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 Maintainer: Alex Ruddick
 Maintainer-email: alex@numat-tech.com
 License: GPLv2
```

### Comparing `midas-0.6.2/README.md` & `midas-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `midas-0.6.2/midas/__init__.py` & `midas-0.6.3/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `midas-0.6.2/midas/driver.py` & `midas-0.6.3/midas/driver.py`

 * *Files identical despite different names*

### Comparing `midas-0.6.2/midas/faults.csv` & `midas-0.6.3/midas/faults.csv`

 * *Files identical despite different names*

### Comparing `midas-0.6.2/midas/mock.py` & `midas-0.6.3/midas/mock.py`

 * *Files identical despite different names*

### Comparing `midas-0.6.2/midas/util.py` & `midas-0.6.3/midas/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,16 +122,14 @@
         request sent while it's processing something). The driver handles this
         by assuming there is only one client instance. If other clients
         exist, other logic will have to be added to either prevent or manage
         race conditions.
         """
         await self.connectTask
         async with self.lock:
-            if not self.client.connected:
-                raise ConnectionError("Not connected to Midas.")
             try:
                 if self.pymodbus32plus:
                     future = getattr(self.client, method)
                 else:
                     future = getattr(self.client.protocol, method)  # type: ignore
                 return await future(*args, **kwargs)
             except (asyncio.TimeoutError, pymodbus.exceptions.ConnectionException) as e:
```

### Comparing `midas-0.6.2/midas.egg-info/PKG-INFO` & `midas-0.6.3/midas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python driver for Honeywell Midas gas detectors.
 Home-page: https://github.com/numat/midas/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 Maintainer: Alex Ruddick
 Maintainer-email: alex@numat-tech.com
 License: GPLv2
```

### Comparing `midas-0.6.2/setup.py` & `midas-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     raise ImportError("This module requires Python >=3.8.  Use 0.5.1 for Python3.7")
 
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="midas",
-    version="0.6.2",
+    version="0.6.3",
     description="Python driver for Honeywell Midas gas detectors.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/numat/midas/",
     author="Patrick Fuller",
     author_email="pat@numat-tech.com",
     maintainer="Alex Ruddick",
@@ -29,15 +29,15 @@
     ],
     extras_require={
         'test': [
             'mypy>=1.1.1',
             'pytest',
             'pytest-cov',
             'pytest-asyncio',
-            'ruff==0.0.270',
+            'ruff==0.0.272',
         ],
     },
     entry_points={
         'console_scripts': [('midas = midas:command_line')]
     },
     license='GPLv2',
     classifiers=[
```

