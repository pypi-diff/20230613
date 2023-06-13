# Comparing `tmp/cds-python-sdk-0.11.tar.gz` & `tmp/cds-python-sdk-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cds-python-sdk-0.11.tar", last modified: Wed May 31 09:03:33 2023, max compression
+gzip compressed data, was "cds-python-sdk-0.12.tar", last modified: Tue Jun 13 08:44:14 2023, max compression
```

## Comparing `cds-python-sdk-0.11.tar` & `cds-python-sdk-0.12.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.480455 cds-python-sdk-0.11/
--rw-rw-rw-   0        0        0    10313 2023-05-23 06:32:39.000000 cds-python-sdk-0.11/LICENSE
--rw-rw-rw-   0        0        0      221 2023-05-31 09:03:33.479530 cds-python-sdk-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     4500 2023-05-31 08:44:17.000000 cds-python-sdk-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.440857 cds-python-sdk-0.11/capitalonline/
--rw-rw-rw-   0        0        0       17 2023-05-10 08:44:21.000000 cds-python-sdk-0.11/capitalonline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.447510 cds-python-sdk-0.11/capitalonline/common/
--rw-rw-rw-   0        0        0        0 2023-05-08 10:10:30.000000 cds-python-sdk-0.11/capitalonline/common/__init__.py
--rw-rw-rw-   0        0        0    18497 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/common/abstract_client.py
--rw-rw-rw-   0        0        0     1127 2023-05-11 07:27:33.000000 cds-python-sdk-0.11/capitalonline/common/client.py
--rw-rw-rw-   0        0        0     1761 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/common/credential.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.449513 cds-python-sdk-0.11/capitalonline/common/exception/
--rw-rw-rw-   0        0        0      122 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/common/exception/__init__.py
--rw-rw-rw-   0        0        0      706 2023-05-10 08:44:21.000000 cds-python-sdk-0.11/capitalonline/common/exception/cds_sdk_exception.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.452505 cds-python-sdk-0.11/capitalonline/common/http/
--rw-rw-rw-   0        0        0        0 2023-05-10 08:44:21.000000 cds-python-sdk-0.11/capitalonline/common/http/__init__.py
--rw-rw-rw-   0        0        0     5211 2023-05-10 08:44:21.000000 cds-python-sdk-0.11/capitalonline/common/http/request.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.457467 cds-python-sdk-0.11/capitalonline/common/profile/
--rw-rw-rw-   0        0        0        0 2023-05-10 08:44:21.000000 cds-python-sdk-0.11/capitalonline/common/profile/__init__.py
--rw-rw-rw-   0        0        0     1048 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/common/profile/client_profile.py
--rw-rw-rw-   0        0        0     1300 2023-05-30 06:44:49.000000 cds-python-sdk-0.11/capitalonline/common/profile/http_profile.py
--rw-rw-rw-   0        0        0     2782 2023-05-10 08:44:21.000000 cds-python-sdk-0.11/capitalonline/common/sign.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.462449 cds-python-sdk-0.11/capitalonline/haproxy/
--rw-rw-rw-   0        0        0        0 2023-05-08 10:10:30.000000 cds-python-sdk-0.11/capitalonline/haproxy/__init__.py
--rw-rw-rw-   0        0        0    12947 2023-05-30 06:43:43.000000 cds-python-sdk-0.11/capitalonline/haproxy/client.py
--rw-rw-rw-   0        0        0     9175 2023-05-31 08:59:17.000000 cds-python-sdk-0.11/capitalonline/haproxy/client_test.py
--rw-rw-rw-   0        0        0     7938 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/haproxy/models.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.467425 cds-python-sdk-0.11/capitalonline/instance/
--rw-rw-rw-   0        0        0        0 2023-05-08 10:10:30.000000 cds-python-sdk-0.11/capitalonline/instance/__init__.py
--rw-rw-rw-   0        0        0    12078 2023-05-30 06:35:06.000000 cds-python-sdk-0.11/capitalonline/instance/client.py
--rw-rw-rw-   0        0        0    11436 2023-05-31 01:32:34.000000 cds-python-sdk-0.11/capitalonline/instance/client_test.py
--rw-rw-rw-   0        0        0     5795 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/instance/models.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.473541 cds-python-sdk-0.11/capitalonline/vdc/
--rw-rw-rw-   0        0        0        0 2023-05-08 10:10:30.000000 cds-python-sdk-0.11/capitalonline/vdc/__init__.py
--rw-rw-rw-   0        0        0     5518 2023-05-30 06:43:43.000000 cds-python-sdk-0.11/capitalonline/vdc/client.py
--rw-rw-rw-   0        0        0     6335 2023-05-31 08:48:52.000000 cds-python-sdk-0.11/capitalonline/vdc/client_test.py
--rw-rw-rw-   0        0        0     6908 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/vdc/model.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.478524 cds-python-sdk-0.11/cds_python_sdk.egg-info/
--rw-rw-rw-   0        0        0      221 2023-05-31 09:03:33.000000 cds-python-sdk-0.11/cds_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-05-31 09:03:33.000000 cds-python-sdk-0.11/cds_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 09:03:33.000000 cds-python-sdk-0.11/cds_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 09:03:33.000000 cds-python-sdk-0.11/cds_python_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 09:03:33.480455 cds-python-sdk-0.11/setup.cfg
--rw-rw-rw-   0        0        0      384 2023-05-31 09:03:01.000000 cds-python-sdk-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:44:14.181549 cds-python-sdk-0.12/
+-rw-rw-rw-   0        0        0    10313 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/LICENSE
+-rw-rw-rw-   0        0        0      221 2023-06-13 08:44:14.180419 cds-python-sdk-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     4500 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 08:44:14.138258 cds-python-sdk-0.12/capitalonline/
+-rw-rw-rw-   0        0        0       17 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:44:14.149823 cds-python-sdk-0.12/capitalonline/common/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/common/__init__.py
+-rw-rw-rw-   0        0        0    18497 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/common/abstract_client.py
+-rw-rw-rw-   0        0        0     1127 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/common/client.py
+-rw-rw-rw-   0        0        0     1761 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/common/credential.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:44:14.151835 cds-python-sdk-0.12/capitalonline/common/exception/
+-rw-rw-rw-   0        0        0      122 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/common/exception/__init__.py
+-rw-rw-rw-   0        0        0      706 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/common/exception/cds_sdk_exception.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:44:14.154832 cds-python-sdk-0.12/capitalonline/common/http/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/common/http/__init__.py
+-rw-rw-rw-   0        0        0     5211 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/common/http/request.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:44:14.157280 cds-python-sdk-0.12/capitalonline/common/profile/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/common/profile/__init__.py
+-rw-rw-rw-   0        0        0     1048 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/common/profile/client_profile.py
+-rw-rw-rw-   0        0        0     1300 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/common/profile/http_profile.py
+-rw-rw-rw-   0        0        0     2782 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/common/sign.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:44:14.164452 cds-python-sdk-0.12/capitalonline/haproxy/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/haproxy/__init__.py
+-rw-rw-rw-   0        0        0    12947 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/haproxy/client.py
+-rw-rw-rw-   0        0        0     9175 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/haproxy/client_test.py
+-rw-rw-rw-   0        0        0     7938 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/haproxy/models.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:44:14.169210 cds-python-sdk-0.12/capitalonline/instance/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/instance/__init__.py
+-rw-rw-rw-   0        0        0    12078 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/instance/client.py
+-rw-rw-rw-   0        0        0    11436 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/instance/client_test.py
+-rw-rw-rw-   0        0        0     5795 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/instance/models.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:44:14.174410 cds-python-sdk-0.12/capitalonline/vdc/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/vdc/__init__.py
+-rw-rw-rw-   0        0        0     5518 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/vdc/client.py
+-rw-rw-rw-   0        0        0     6335 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/vdc/client_test.py
+-rw-rw-rw-   0        0        0     6908 2023-06-13 08:29:06.000000 cds-python-sdk-0.12/capitalonline/vdc/model.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:44:14.179419 cds-python-sdk-0.12/cds_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-06-13 08:44:14.000000 cds-python-sdk-0.12/cds_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2023-06-13 08:44:14.000000 cds-python-sdk-0.12/cds_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 08:44:14.000000 cds-python-sdk-0.12/cds_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 08:44:14.000000 cds-python-sdk-0.12/cds_python_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 08:44:14.181549 cds-python-sdk-0.12/setup.cfg
+-rw-rw-rw-   0        0        0      384 2023-06-13 08:44:08.000000 cds-python-sdk-0.12/setup.py
```

### Comparing `cds-python-sdk-0.11/LICENSE` & `cds-python-sdk-0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/README.md` & `cds-python-sdk-0.12/README.md`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/abstract_client.py` & `cds-python-sdk-0.12/capitalonline/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/client.py` & `cds-python-sdk-0.12/capitalonline/common/client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/credential.py` & `cds-python-sdk-0.12/capitalonline/common/credential.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/exception/cds_sdk_exception.py` & `cds-python-sdk-0.12/capitalonline/common/exception/cds_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/http/request.py` & `cds-python-sdk-0.12/capitalonline/common/http/request.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/profile/client_profile.py` & `cds-python-sdk-0.12/capitalonline/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/profile/http_profile.py` & `cds-python-sdk-0.12/capitalonline/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/sign.py` & `cds-python-sdk-0.12/capitalonline/common/sign.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/haproxy/client.py` & `cds-python-sdk-0.12/capitalonline/haproxy/client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/haproxy/client_test.py` & `cds-python-sdk-0.12/capitalonline/haproxy/client_test.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/haproxy/models.py` & `cds-python-sdk-0.12/capitalonline/haproxy/models.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/instance/client.py` & `cds-python-sdk-0.12/capitalonline/instance/client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/instance/client_test.py` & `cds-python-sdk-0.12/capitalonline/instance/client_test.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/instance/models.py` & `cds-python-sdk-0.12/capitalonline/instance/models.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/vdc/client.py` & `cds-python-sdk-0.12/capitalonline/vdc/client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/vdc/client_test.py` & `cds-python-sdk-0.12/capitalonline/vdc/client_test.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/vdc/model.py` & `cds-python-sdk-0.12/capitalonline/vdc/model.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/cds_python_sdk.egg-info/SOURCES.txt` & `cds-python-sdk-0.12/cds_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

