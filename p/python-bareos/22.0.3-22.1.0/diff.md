# Comparing `tmp/python-bareos-22.0.3.tar.gz` & `tmp/python-bareos-22.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-bareos-22.0.3.tar", last modified: Fri Mar 24 13:07:25 2023, max compression
+gzip compressed data, was "dist/python-bareos-22.1.0.tar", last modified: Tue Jun 13 10:17:09 2023, max compression
```

## Comparing `python-bareos-22.0.3.tar` & `python-bareos-22.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 13:07:25.000000 python-bareos-22.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-03-24 13:07:25.000000 python-bareos-22.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6890 2023-03-24 13:07:21.000000 python-bareos-22.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 13:07:25.000000 python-bareos-22.0.3/bareos/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-24 13:07:24.000000 python-bareos-22.0.3/bareos/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 13:07:25.000000 python-bareos-22.0.3/bareos/bsock/
--rw-r--r--   0 runner    (1001) docker     (122)     7997 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/bsock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/bsock/bsock.py
--rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/bsock/bsockjson.py
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/bsock/connectiontype.py
--rw-r--r--   0 runner    (1001) docker     (122)     5127 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/bsock/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     9765 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/bsock/directorconsole.py
--rw-r--r--   0 runner    (1001) docker     (122)     4457 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/bsock/directorconsolejson.py
--rw-r--r--   0 runner    (1001) docker     (122)     6048 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/bsock/filedaemon.py
--rw-r--r--   0 runner    (1001) docker     (122)    28846 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/bsock/lowlevel.py
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/bsock/protocolmessageids.py
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/bsock/protocolmessages.py
--rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/bsock/protocolversions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2817 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/bsock/tlsversionparser.py
--rw-r--r--   0 runner    (1001) docker     (122)     4071 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 13:07:25.000000 python-bareos-22.0.3/bareos/util/
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/util/bareosbase64.py
--rw-r--r--   0 runner    (1001) docker     (122)     2531 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/util/password.py
--rw-r--r--   0 runner    (1001) docker     (122)     3140 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bareos/util/path.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 13:07:25.000000 python-bareos-22.0.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (122)     2108 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bin/bareos-fd-connect.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1994 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bin/bconsole-json.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1968 2023-03-24 13:07:21.000000 python-bareos-22.0.3/bin/bconsole.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 13:07:25.000000 python-bareos-22.0.3/python_bareos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-03-24 13:07:25.000000 python-bareos-22.0.3/python_bareos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-03-24 13:07:25.000000 python-bareos-22.0.3/python_bareos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-24 13:07:25.000000 python-bareos-22.0.3/python_bareos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-03-24 13:07:25.000000 python-bareos-22.0.3/python_bareos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-24 13:07:25.000000 python-bareos-22.0.3/python_bareos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-24 13:07:25.000000 python-bareos-22.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-03-24 13:07:21.000000 python-bareos-22.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 10:17:09.000000 python-bareos-22.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-06-13 10:17:09.000000 python-bareos-22.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6890 2023-06-13 10:17:03.000000 python-bareos-22.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 10:17:09.000000 python-bareos-22.1.0/bareos/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-13 10:17:07.000000 python-bareos-22.1.0/bareos/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 10:17:09.000000 python-bareos-22.1.0/bareos/bsock/
+-rw-r--r--   0 runner    (1001) docker     (122)     7997 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/bsock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/bsock/bsock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/bsock/bsockjson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/bsock/connectiontype.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5127 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/bsock/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9765 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/bsock/directorconsole.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4457 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/bsock/directorconsolejson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6048 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/bsock/filedaemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28846 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/bsock/lowlevel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/bsock/protocolmessageids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/bsock/protocolmessages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/bsock/protocolversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2817 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/bsock/tlsversionparser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4071 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 10:17:09.000000 python-bareos-22.1.0/bareos/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/util/bareosbase64.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2531 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/util/password.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3140 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bareos/util/path.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 10:17:09.000000 python-bareos-22.1.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2108 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bin/bareos-fd-connect.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1994 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bin/bconsole-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1968 2023-06-13 10:17:03.000000 python-bareos-22.1.0/bin/bconsole.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 10:17:09.000000 python-bareos-22.1.0/python_bareos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-06-13 10:17:09.000000 python-bareos-22.1.0/python_bareos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-06-13 10:17:09.000000 python-bareos-22.1.0/python_bareos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 10:17:09.000000 python-bareos-22.1.0/python_bareos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-13 10:17:09.000000 python-bareos-22.1.0/python_bareos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-13 10:17:09.000000 python-bareos-22.1.0/python_bareos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 10:17:09.000000 python-bareos-22.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-06-13 10:17:03.000000 python-bareos-22.1.0/setup.py
```

### Comparing `python-bareos-22.0.3/PKG-INFO` & `python-bareos-22.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bareos
-Version: 22.0.3
+Version: 22.1.0
 Summary: Client library and tools for Bareos console access.
 Home-page: https://github.com/bareos/bareos/
 Author: Bareos Team
 Author-email: packager@bareos.com
 License: AGPLv3
 Description: python-bareos
         =============
```

### Comparing `python-bareos-22.0.3/README.rst` & `python-bareos-22.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/__init__.py` & `python-bareos-22.1.0/bareos/__init__.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/bsock/__init__.py` & `python-bareos-22.1.0/bareos/bsock/__init__.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/bsock/bsock.py` & `python-bareos-22.1.0/bareos/bsock/bsock.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/bsock/bsockjson.py` & `python-bareos-22.1.0/bareos/bsock/bsockjson.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/bsock/connectiontype.py` & `python-bareos-22.1.0/bareos/bsock/connectiontype.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/bsock/constants.py` & `python-bareos-22.1.0/bareos/bsock/constants.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/bsock/directorconsole.py` & `python-bareos-22.1.0/bareos/bsock/directorconsole.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/bsock/directorconsolejson.py` & `python-bareos-22.1.0/bareos/bsock/directorconsolejson.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/bsock/filedaemon.py` & `python-bareos-22.1.0/bareos/bsock/filedaemon.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/bsock/lowlevel.py` & `python-bareos-22.1.0/bareos/bsock/lowlevel.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/bsock/protocolmessageids.py` & `python-bareos-22.1.0/bareos/bsock/protocolmessageids.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/bsock/protocolmessages.py` & `python-bareos-22.1.0/bareos/bsock/protocolmessages.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/bsock/protocolversions.py` & `python-bareos-22.1.0/bareos/bsock/protocolversions.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/bsock/tlsversionparser.py` & `python-bareos-22.1.0/bareos/bsock/tlsversionparser.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/exceptions.py` & `python-bareos-22.1.0/bareos/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/util/__init__.py` & `python-bareos-22.1.0/bareos/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/util/bareosbase64.py` & `python-bareos-22.1.0/bareos/util/bareosbase64.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/util/password.py` & `python-bareos-22.1.0/bareos/util/password.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bareos/util/path.py` & `python-bareos-22.1.0/bareos/util/path.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bin/bareos-fd-connect.py` & `python-bareos-22.1.0/bin/bareos-fd-connect.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bin/bconsole-json.py` & `python-bareos-22.1.0/bin/bconsole-json.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/bin/bconsole.py` & `python-bareos-22.1.0/bin/bconsole.py`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/python_bareos.egg-info/PKG-INFO` & `python-bareos-22.1.0/python_bareos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bareos
-Version: 22.0.3
+Version: 22.1.0
 Summary: Client library and tools for Bareos console access.
 Home-page: https://github.com/bareos/bareos/
 Author: Bareos Team
 Author-email: packager@bareos.com
 License: AGPLv3
 Description: python-bareos
         =============
```

### Comparing `python-bareos-22.0.3/python_bareos.egg-info/SOURCES.txt` & `python-bareos-22.1.0/python_bareos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-bareos-22.0.3/setup.py` & `python-bareos-22.1.0/setup.py`

 * *Files identical despite different names*

