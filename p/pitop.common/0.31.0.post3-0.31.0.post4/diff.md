# Comparing `tmp/pitop.common-0.31.0.post3.tar.gz` & `tmp/pitop.common-0.31.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.common-0.31.0.post3.tar", last modified: Tue Jun 13 16:41:52 2023, max compression
+gzip compressed data, was "dist/pitop.common-0.31.0.post4.tar", last modified: Tue Jun 13 18:30:06 2023, max compression
```

## Comparing `pitop.common-0.31.0.post3.tar` & `pitop.common-0.31.0.post4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:52.000000 pitop.common-0.31.0.post3/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      945 2023-06-13 16:41:52.000000 pitop.common-0.31.0.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:52.000000 pitop.common-0.31.0.post3/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:52.000000 pitop.common-0.31.0.post3/pitop/common/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/bitwise_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     3618 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/common_ids.py
--rw-r--r--   0 runner    (1001) docker     (122)      649 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/common_names.py
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/configuration_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/counter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/current_session_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/file_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)     5477 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/firmware_device.py
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/formatting.py
--rw-r--r--   0 runner    (1001) docker     (122)     7212 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/i2c_device.py
--rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     3442 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     3050 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/notifications.py
--rw-r--r--   0 runner    (1001) docker     (122)     2659 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/pt_os.py
--rw-r--r--   0 runner    (1001) docker     (122)    19828 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/ptdm.py
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)     5539 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/smbus_device.py
--rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/switch_user.py
--rw-r--r--   0 runner    (1001) docker     (122)     8308 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/pitop/common/type_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:52.000000 pitop.common-0.31.0.post3/pitop.common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      945 2023-06-13 16:41:52.000000 pitop.common-0.31.0.post3/pitop.common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-06-13 16:41:52.000000 pitop.common-0.31.0.post3/pitop.common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 16:41:52.000000 pitop.common-0.31.0.post3/pitop.common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-06-13 16:41:52.000000 pitop.common-0.31.0.post3/pitop.common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 16:41:52.000000 pitop.common-0.31.0.post3/pitop.common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 16:41:52.000000 pitop.common-0.31.0.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2201 2023-06-13 16:41:37.000000 pitop.common-0.31.0.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:06.000000 pitop.common-0.31.0.post4/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      945 2023-06-13 18:30:06.000000 pitop.common-0.31.0.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:06.000000 pitop.common-0.31.0.post4/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:06.000000 pitop.common-0.31.0.post4/pitop/common/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/bitwise_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3618 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/common_ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/common_names.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/configuration_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/current_session_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/file_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5477 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/firmware_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7212 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/i2c_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3442 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3050 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2659 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/pt_os.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19828 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/ptdm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5539 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/smbus_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/switch_user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8308 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/pitop/common/type_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:06.000000 pitop.common-0.31.0.post4/pitop.common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      945 2023-06-13 18:30:06.000000 pitop.common-0.31.0.post4/pitop.common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-06-13 18:30:06.000000 pitop.common-0.31.0.post4/pitop.common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 18:30:06.000000 pitop.common-0.31.0.post4/pitop.common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-06-13 18:30:06.000000 pitop.common-0.31.0.post4/pitop.common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 18:30:06.000000 pitop.common-0.31.0.post4/pitop.common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 18:30:06.000000 pitop.common-0.31.0.post4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2218 2023-06-13 18:29:44.000000 pitop.common-0.31.0.post4/setup.py
```

### Comparing `pitop.common-0.31.0.post3/PKG-INFO` & `pitop.common-0.31.0.post4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.common
-Version: 0.31.0.post3
+Version: 0.31.0.post4
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Common
```

### Comparing `pitop.common-0.31.0.post3/pitop/common/bitwise_ops.py` & `pitop.common-0.31.0.post4/pitop/common/bitwise_ops.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/command_runner.py` & `pitop.common-0.31.0.post4/pitop/common/command_runner.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/common_ids.py` & `pitop.common-0.31.0.post4/pitop/common/common_ids.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/common_names.py` & `pitop.common-0.31.0.post4/pitop/common/common_names.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/configuration_file.py` & `pitop.common-0.31.0.post4/pitop/common/configuration_file.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/current_session_info.py` & `pitop.common-0.31.0.post4/pitop/common/current_session_info.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/file_ops.py` & `pitop.common-0.31.0.post4/pitop/common/file_ops.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/firmware_device.py` & `pitop.common-0.31.0.post4/pitop/common/firmware_device.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/formatting.py` & `pitop.common-0.31.0.post4/pitop/common/formatting.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/i2c_device.py` & `pitop.common-0.31.0.post4/pitop/common/i2c_device.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/lock.py` & `pitop.common-0.31.0.post4/pitop/common/lock.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/logger.py` & `pitop.common-0.31.0.post4/pitop/common/logger.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/notifications.py` & `pitop.common-0.31.0.post4/pitop/common/notifications.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/pt_os.py` & `pitop.common-0.31.0.post4/pitop/common/pt_os.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/ptdm.py` & `pitop.common-0.31.0.post4/pitop/common/ptdm.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/smbus_device.py` & `pitop.common-0.31.0.post4/pitop/common/smbus_device.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/switch_user.py` & `pitop.common-0.31.0.post4/pitop/common/switch_user.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop/common/sys_info.py` & `pitop.common-0.31.0.post4/pitop/common/sys_info.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/pitop.common.egg-info/PKG-INFO` & `pitop.common-0.31.0.post4/pitop.common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.common
-Version: 0.31.0.post3
+Version: 0.31.0.post4
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Common
```

### Comparing `pitop.common-0.31.0.post3/pitop.common.egg-info/SOURCES.txt` & `pitop.common-0.31.0.post4/pitop.common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.common-0.31.0.post3/setup.py` & `pitop.common-0.31.0.post4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 if not sys.version_info >= (3, 7):
     raise ValueError("This package requires Python 3.7 or above")
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
-__version__ = os.environ.get("PYTHON_PACKAGE_VERSION", "0.0.1.dev1")
+__version__ = os.environ.get("PYTHON_PACKAGE_VERSION", "0.0.1.dev1").replace('"', "")
 assert __version__ != ""
 
 __project__ = "pitop.common"
 __author__ = "pi-top"
 __author_email__ = "deb-maintainers@pi-top.com"
 
 __url__ = "https://github.com/pi-top/pi-top-Python-SDK"
```

