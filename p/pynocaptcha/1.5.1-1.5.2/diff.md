# Comparing `tmp/pynocaptcha-1.5.1.tar.gz` & `tmp/pynocaptcha-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.5.1.tar", last modified: Tue Jun  6 02:58:09 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.5.2.tar", last modified: Tue Jun 13 04:04:43 2023, max compression
```

## Comparing `pynocaptcha-1.5.1.tar` & `pynocaptcha-1.5.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-06 02:58:09.000000 pynocaptcha-1.5.1/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-06-06 02:58:09.000000 pynocaptcha-1.5.1/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-06 02:58:09.000000 pynocaptcha-1.5.1/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      571 2023-05-15 07:30:18.000000 pynocaptcha-1.5.1/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-06 02:58:09.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)     1016 2023-06-06 02:53:27.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)     4715 2023-06-06 02:54:14.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2108 2023-05-15 07:32:09.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.5.1/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-06-06 02:43:43.000000 pynocaptcha-1.5.1/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-13 04:04:43.000000 pynocaptcha-1.5.2/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-06-13 04:04:43.000000 pynocaptcha-1.5.2/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-13 04:04:43.000000 pynocaptcha-1.5.2/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      571 2023-05-15 07:30:18.000000 pynocaptcha-1.5.2/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-06-13 04:04:43.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1016 2023-06-06 02:53:27.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     4715 2023-06-06 02:54:14.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5186 2023-04-23 09:01:32.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)   222114 2023-06-13 04:02:11.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2449 2023-04-23 08:59:52.000000 pynocaptcha-1.5.2/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-06-13 04:03:14.000000 pynocaptcha-1.5.2/setup.py
```

### Comparing `pynocaptcha-1.5.1/PKG-INFO` & `pynocaptcha-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.5.1
+Version: 1.5.2
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.5.1/pynocaptcha/__init__.py` & `pynocaptcha-1.5.2/pynocaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.1/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.5.2/pynocaptcha/crackers/akamai.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.1/pynocaptcha/crackers/base.py` & `pynocaptcha-1.5.2/pynocaptcha/crackers/base.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.1/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.5.2/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.1/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.5.2/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.1/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.5.2/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.5.1/setup.py` & `pynocaptcha-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.5.1',
+    version='1.5.2',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

