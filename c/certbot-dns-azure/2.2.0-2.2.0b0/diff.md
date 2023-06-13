# Comparing `tmp/certbot-dns-azure-2.2.0.tar.gz` & `tmp/certbot-dns-azure-2.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-azure-2.2.0.tar", last modified: Tue Jun 13 09:49:32 2023, max compression
+gzip compressed data, was "certbot-dns-azure-2.2.0b0.tar", last modified: Tue May 16 20:29:37 2023, max compression
```

## Comparing `certbot-dns-azure-2.2.0.tar` & `certbot-dns-azure-2.2.0b0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:49:32.681575 certbot-dns-azure-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-13 09:49:32.681575 certbot-dns-azure-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:49:32.677575 certbot-dns-azure-2.2.0/certbot_dns_azure/
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/certbot_dns_azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:49:32.677575 certbot-dns-azure-2.2.0/certbot_dns_azure/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/certbot_dns_azure/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15391 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/certbot_dns_azure/_internal/dns_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:49:32.677575 certbot-dns-azure-2.2.0/certbot_dns_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-13 09:49:32.000000 certbot-dns-azure-2.2.0/certbot_dns_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-13 09:49:32.000000 certbot-dns-azure-2.2.0/certbot_dns_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:49:32.000000 certbot-dns-azure-2.2.0/certbot_dns_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 09:49:32.000000 certbot-dns-azure-2.2.0/certbot_dns_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-13 09:49:32.000000 certbot-dns-azure-2.2.0/certbot_dns_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 09:49:32.000000 certbot-dns-azure-2.2.0/certbot_dns_azure.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:49:32.677575 certbot-dns-azure-2.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 09:49:32.681575 certbot-dns-azure-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:49:32.677575 certbot-dns-azure-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-06-13 09:49:27.000000 certbot-dns-azure-2.2.0/tests/dns_azure_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.536460 certbot-dns-azure-2.2.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-16 20:29:37.536460 certbot-dns-azure-2.2.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/certbot_dns_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/certbot_dns_azure/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15391 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure/_internal/dns_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 20:29:37.536460 certbot-dns-azure-2.2.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/tests/dns_azure_test.py
```

### Comparing `certbot-dns-azure-2.2.0/LICENSE.txt` & `certbot-dns-azure-2.2.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0/PKG-INFO` & `certbot-dns-azure-2.2.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-azure
-Version: 2.2.0
+Version: 2.2.0b0
 Summary: Azure DNS Authenticator plugin for Certbot
 Home-page: https://github.com/binkhq/certbot-dns-azure
 Author: Terry Cain
 Author-email: opensource@bink.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-azure-2.2.0/README.md` & `certbot-dns-azure-2.2.0b0/README.md`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0/certbot_dns_azure/__init__.py` & `certbot-dns-azure-2.2.0b0/certbot_dns_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0/certbot_dns_azure/_internal/dns_azure.py` & `certbot-dns-azure-2.2.0b0/certbot_dns_azure/_internal/dns_azure.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0/certbot_dns_azure.egg-info/PKG-INFO` & `certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-azure
-Version: 2.2.0
+Version: 2.2.0b0
 Summary: Azure DNS Authenticator plugin for Certbot
 Home-page: https://github.com/binkhq/certbot-dns-azure
 Author: Terry Cain
 Author-email: opensource@bink.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-azure-2.2.0/certbot_dns_azure.egg-info/SOURCES.txt` & `certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0/docs/Makefile` & `certbot-dns-azure-2.2.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0/docs/conf.py` & `certbot-dns-azure-2.2.0b0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0/docs/index.rst` & `certbot-dns-azure-2.2.0b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0/docs/make.bat` & `certbot-dns-azure-2.2.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0/setup.py` & `certbot-dns-azure-2.2.0b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages
 from setuptools import setup
 
-version = '2.2.0'
+version = '2.2.0b0'
 
 # azure-mgmt-dns is still the old style SDK, so will change dramatically
 # when they refactor, most notably the credential parts
 install_requires = [
     'azure-identity>=1.11.0',
     'azure-mgmt-dns>=8.0.0',
     'setuptools>=41.6.0',
```

### Comparing `certbot-dns-azure-2.2.0/tests/dns_azure_test.py` & `certbot-dns-azure-2.2.0b0/tests/dns_azure_test.py`

 * *Files identical despite different names*

