# Comparing `tmp/quao-0.2.0.tar.gz` & `tmp/quao-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.2.0.tar", last modified: Fri Jun  2 11:42:27 2023, max compression
+gzip compressed data, was "quao-0.2.1.tar", last modified: Tue Jun 13 10:13:32 2023, max compression
```

## Comparing `quao-0.2.0.tar` & `quao-0.2.1.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:27.035174 quao-0.2.0/
--rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-06-02 11:42:27.034173 quao-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.2.0/README.md
--rw-rw-rw-   0        0        0      916 2023-06-02 11:41:53.000000 quao-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 11:42:27.035174 quao-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.929206 quao-0.2.0/src/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.932443 quao-0.2.0/src/quao/
--rw-rw-rw-   0        0        0      203 2023-06-02 11:41:53.000000 quao-0.2.0/src/quao/__init__.py
--rw-rw-rw-   0        0        0     5614 2023-06-02 09:50:49.000000 quao-0.2.0/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.964175 quao-0.2.0/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      190 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/config/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.965176 quao-0.2.0/src/quao/data/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.968175 quao-0.2.0/src/quao/data/job/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/data/job/__init__.py
--rw-rw-rw-   0        0        0      801 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/data/job/job_response.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.973176 quao-0.2.0/src/quao/data/request/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/data/request/__init__.py
--rw-rw-rw-   0        0        0      566 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/data/request/request_data.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.984176 quao-0.2.0/src/quao/enum/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/enum/__init__.py
--rw-rw-rw-   0        0        0      212 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/enum/http_status.py
--rw-rw-rw-   0        0        0      213 2023-06-01 11:44:52.000000 quao-0.2.0/src/quao/enum/job_status.py
--rw-rw-rw-   0        0        0      258 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/enum/media_type.py
--rw-rw-rw-   0        0        0      297 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/enum/provider_type.py
--rw-rw-rw-   0        0        0      179 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/enum/sdk.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.992206 quao-0.2.0/src/quao/factory/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/factory/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-06-01 11:39:48.000000 quao-0.2.0/src/quao/factory/device_factory.py
--rw-rw-rw-   0        0        0     1351 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/factory/provider_factory.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.994174 quao-0.2.0/src/quao/model/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:27.010205 quao-0.2.0/src/quao/model/device/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/model/device/__init__.py
--rw-rw-rw-   0        0        0     1538 2023-06-02 09:50:49.000000 quao-0.2.0/src/quao/model/device/aws_braket_device.py
--rw-rw-rw-   0        0        0     3062 2023-06-02 11:14:34.000000 quao-0.2.0/src/quao/model/device/device.py
--rw-rw-rw-   0        0        0     1012 2023-06-02 09:50:48.000000 quao-0.2.0/src/quao/model/device/ibm_cloud_device.py
--rw-rw-rw-   0        0        0      794 2023-06-02 09:50:49.000000 quao-0.2.0/src/quao/model/device/ibm_quantum_device.py
--rw-rw-rw-   0        0        0      776 2023-06-02 09:50:48.000000 quao-0.2.0/src/quao/model/device/qiskit_device.py
--rw-rw-rw-   0        0        0     2511 2023-06-02 09:52:05.000000 quao-0.2.0/src/quao/model/device/quao_device.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:27.013177 quao-0.2.0/src/quao/model/job/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/model/job/__init__.py
--rw-rw-rw-   0        0        0     2693 2023-06-02 10:03:39.000000 quao-0.2.0/src/quao/model/job/qiskit_status.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:27.026215 quao-0.2.0/src/quao/model/provider/
--rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/model/provider/__init__.py
--rw-rw-rw-   0        0        0     1255 2023-06-02 09:50:48.000000 quao-0.2.0/src/quao/model/provider/aws_braket_provider.py
--rw-rw-rw-   0        0        0     1008 2023-06-02 09:50:48.000000 quao-0.2.0/src/quao/model/provider/ibm_cloud_provider.py
--rw-rw-rw-   0        0        0      876 2023-06-02 09:50:48.000000 quao-0.2.0/src/quao/model/provider/ibm_quantum_provider.py
--rw-rw-rw-   0        0        0      589 2023-06-01 03:12:31.000000 quao-0.2.0/src/quao/model/provider/provider.py
--rw-rw-rw-   0        0        0     1372 2023-06-02 09:50:49.000000 quao-0.2.0/src/quao/model/provider/quao_provider.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:27.032173 quao-0.2.0/src/quao/util/
--rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/util/__init__.py
--rw-rw-rw-   0        0        0     2047 2023-06-02 09:11:35.000000 quao-0.2.0/src/quao/util/json_parser_util.py
--rw-rw-rw-   0        0        0     1288 2023-06-01 08:49:23.000000 quao-0.2.0/src/quao/util/response_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.960179 quao-0.2.0/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-06-02 11:42:26.000000 quao-0.2.0/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1447 2023-06-02 11:42:26.000000 quao-0.2.0/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 11:42:26.000000 quao-0.2.0/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      166 2023-06-02 11:42:26.000000 quao-0.2.0/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-02 11:42:26.000000 quao-0.2.0/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.807749 quao-0.2.1/
+-rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-06-13 10:13:32.806750 quao-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.2.1/README.md
+-rw-rw-rw-   0        0        0      916 2023-06-13 10:09:48.000000 quao-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 10:13:32.807749 quao-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.674815 quao-0.2.1/src/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.676769 quao-0.2.1/src/quao/
+-rw-rw-rw-   0        0        0      203 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/__init__.py
+-rw-rw-rw-   0        0        0     5614 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.712614 quao-0.2.1/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/config/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.714715 quao-0.2.1/src/quao/data/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.716603 quao-0.2.1/src/quao/data/job/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/data/job/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/data/job/job_response.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.726764 quao-0.2.1/src/quao/data/request/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/data/request/__init__.py
+-rw-rw-rw-   0        0        0      566 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/data/request/request_data.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.769379 quao-0.2.1/src/quao/enum/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/enum/__init__.py
+-rw-rw-rw-   0        0        0      212 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/enum/http_status.py
+-rw-rw-rw-   0        0        0      213 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/enum/job_status.py
+-rw-rw-rw-   0        0        0      258 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/enum/media_type.py
+-rw-rw-rw-   0        0        0      205 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/enum/processing_unit.py
+-rw-rw-rw-   0        0        0      297 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/enum/provider_type.py
+-rw-rw-rw-   0        0        0      179 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/enum/sdk.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.775210 quao-0.2.1/src/quao/factory/
+-rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/factory/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/factory/device_factory.py
+-rw-rw-rw-   0        0        0     1351 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.777226 quao-0.2.1/src/quao/model/
+-rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.789781 quao-0.2.1/src/quao/model/device/
+-rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/model/device/__init__.py
+-rw-rw-rw-   0        0        0     1540 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0        0        0     3144 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/device/device.py
+-rw-rw-rw-   0        0        0     1014 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      794 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0      778 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0        0        0     2513 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/device/quao_device.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.792457 quao-0.2.1/src/quao/model/job/
+-rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/model/job/__init__.py
+-rw-rw-rw-   0        0        0     2693 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/job/qiskit_status.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.801349 quao-0.2.1/src/quao/model/provider/
+-rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.1/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1257 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0        0        0     1010 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      880 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0      589 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/provider/provider.py
+-rw-rw-rw-   0        0        0     1519 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/model/provider/quao_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.805750 quao-0.2.1/src/quao/util/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.1/src/quao/util/__init__.py
+-rw-rw-rw-   0        0        0     2047 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/util/json_parser_util.py
+-rw-rw-rw-   0        0        0     1288 2023-06-13 10:09:48.000000 quao-0.2.1/src/quao/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:13:32.704082 quao-0.2.1/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-06-13 10:13:32.000000 quao-0.2.1/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1480 2023-06-13 10:13:32.000000 quao-0.2.1/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 10:13:32.000000 quao-0.2.1/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      166 2023-06-13 10:13:32.000000 quao-0.2.1/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 10:13:32.000000 quao-0.2.1/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.2.0/LICENSE` & `quao-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.2.0/PKG-INFO` & `quao-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.2.0
+Version: 0.2.1
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.2.0/README.md` & `quao-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.2.0/pyproject.toml` & `quao-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.2.0"
+version = "0.2.1"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `quao-0.2.0/src/quao/backend.py` & `quao-0.2.1/src/quao/backend.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.0/src/quao/data/job/job_response.py` & `quao-0.2.1/src/quao/data/job/job_response.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.0/src/quao/data/request/request_data.py` & `quao-0.2.1/src/quao/data/request/request_data.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.0/src/quao/factory/device_factory.py` & `quao-0.2.1/src/quao/factory/device_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.0/src/quao/factory/provider_factory.py` & `quao-0.2.1/src/quao/factory/provider_factory.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.0/src/quao/model/device/aws_braket_device.py` & `quao-0.2.1/src/quao/model/device/aws_braket_device.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 from ..device.device import Device
 from ..provider.provider import Provider
 from ...enum.job_status import JobStatus
 from ...util.json_parser_util import JsonParserUtils
 from ...config.logging_config import logging
 
+
 class AwsBraketDevice(Device):
 
     def __init__(self, provider: Provider,
                  device_specification: str,
                  s3_bucket_name: str,
                  s3_prefix: str):
         super().__init__(provider, device_specification)
```

### Comparing `quao-0.2.0/src/quao/model/device/device.py` & `quao-0.2.1/src/quao/model/device/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from ...data.job.job_response import JobResponse
 from ...enum.job_status import JobStatus
 from ...enum.media_type import MediaType
 from ...model.provider.provider import Provider
 from ...config.logging_config import logging
 
+
 class Device(ABC):
     def __init__(self, provider: Provider, device_specification: str):
         self.provider = provider
         self.device = provider.get_backend(device_specification)
 
     def run_circuit(self, circuit, shots: int) -> JobResponse:
         """
@@ -42,15 +43,16 @@
                 content_type = MediaType.APPLICATION_JSON.value
 
                 logging.info('Producing histogram ....')
                 job_histogram = self._produce_histogram_data(job_result)
                 logging.info('Producing histogram completed!')
 
         except Exception as exception:
-            logging.info('Exception when invoke job on device {0}: {1}'.format(self.device.shots, str(exception)))
+            logging.info('Exception when invoke job on device {0}: {1}'.format(self.device.shots,
+                                                                               str(exception)))
             job_result_dictionary = {
                 "error": "Exception when invoke job on device: " + self.device.name,
                 "exception": str(exception)
             }
             job_status = JobStatus.ERROR.value
 
         return JobResponse(
```

### Comparing `quao-0.2.0/src/quao/model/device/ibm_cloud_device.py` & `quao-0.2.1/src/quao/model/device/ibm_cloud_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 from qiskit_ibm_runtime import Options, Session, Sampler
 
 from ...model.device.qiskit_device import QiskitDevice
 from ...util.json_parser_util import JsonParserUtils
 from ...config.logging_config import logging
 
+
 class IbmCloudDevice(QiskitDevice):
     def _is_simulator(self) -> bool:
         return self.device.configuration().simulator
 
     def _parse_job_result(self, job_result) -> dict:
         return JsonParserUtils.parse(job_result.__dict__)
```

### Comparing `quao-0.2.0/src/quao/model/device/ibm_quantum_device.py` & `quao-0.2.1/src/quao/model/device/ibm_quantum_device.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 from qiskit import transpile
 
 from ...model.device.qiskit_device import QiskitDevice
 from ...util.json_parser_util import JsonParserUtils
 from ...config.logging_config import logging
 
+
 class IbmQuantumDevice(QiskitDevice):
 
     def _is_simulator(self) -> bool:
         return self.device.configuration().simulator
 
     def _parse_job_result(self, job_result) -> dict:
         return JsonParserUtils.parse(job_result.to_dict())
 
     def _create_job(self, circuit, shots):
         logging.info('Create Ibm Quantum job with {0} shots'.format(shots))
         transpile_circuit = transpile(circuit, self.device)
 
         return self.device.run(transpile_circuit, shots=shots)
-
```

### Comparing `quao-0.2.0/src/quao/model/device/qiskit_device.py` & `quao-0.2.1/src/quao/model/device/qiskit_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from abc import ABC
 
 from qiskit import QiskitError
 
 from ...model.device.device import Device
 from ...config.logging_config import logging
 
+
 class QiskitDevice(Device, ABC):
 
     def _produce_histogram_data(self, job_result) -> dict:
         try:
             histogram_data = job_result.get_counts()
         except QiskitError as qiskit_error:
             logging.info("Can't produce histogram with error: {0}".format(str(qiskit_error)))
```

### Comparing `quao-0.2.0/src/quao/model/device/quao_device.py` & `quao-0.2.1/src/quao/model/device/quao_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ...enum.job_status import JobStatus
 from ...util.json_parser_util import JsonParserUtils
 from ...enum.sdk import Sdk
 from ..device.device import Device
 from ..provider.provider import Provider
 from ...config.logging_config import logging
 
+
 class QuaoDevice(Device):
     def __init__(self, provider: Provider, device_specification: str, sdk: str):
         super().__init__(provider, device_specification)
         self.sdk = sdk
 
     def _create_job(self, circuit, shots):
         logging.info('Create Quao job with {0} shots'.format(shots))
```

### Comparing `quao-0.2.0/src/quao/model/job/qiskit_status.py` & `quao-0.2.1/src/quao/model/job/qiskit_status.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.0/src/quao/model/provider/aws_braket_provider.py` & `quao-0.2.1/src/quao/model/provider/aws_braket_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import boto3
 from braket.aws import AwsSession, AwsDevice
 
 from ...enum.provider_type import ProviderType
 from ...model.provider.provider import Provider
 from ...config.logging_config import logging
 
+
 class AwsBraketProvider(Provider):
 
     def __init__(self, aws_access_key, aws_secret_access_key, region_name):
         super().__init__(ProviderType.AWS_BRAKET)
         self.aws_access_key = aws_access_key
         self.aws_secret_access_key = aws_secret_access_key
         self.region_name = region_name
```

### Comparing `quao-0.2.0/src/quao/model/provider/ibm_cloud_provider.py` & `quao-0.2.1/src/quao/model/provider/ibm_cloud_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 from qiskit_ibm_runtime import QiskitRuntimeService
 
 from ...enum.provider_type import ProviderType
 from ...model.provider.provider import Provider
 from ...config.logging_config import logging
 
+
 class IbmCloudProvider(Provider):
 
     def __init__(self, api_key, crn):
         super().__init__(ProviderType.IBM_CLOUD)
         self.api_key = api_key
         self.crn = crn
         self.channel = 'ibm_cloud'
```

### Comparing `quao-0.2.0/src/quao/model/provider/ibm_quantum_provider.py` & `quao-0.2.1/src/quao/model/provider/ibm_quantum_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 from qiskit_ibm_provider import IBMProvider
 
 from ...enum.provider_type import ProviderType
 from ...model.provider.provider import Provider
 from ...config.logging_config import logging
 
+
 class IbmQuantumProvider(Provider):
     def __init__(self, api_token):
         super().__init__(ProviderType.IBM_QUANTUM)
         self.api_token = api_token
 
     def get_backend(self, device_specification: str):
         """
@@ -25,8 +26,8 @@
     def collect_providers(self):
         """
 
         @return:
         """
 
         logging.info('Connect to Ibm Quantum provider')
-        return IBMProvider(token=self.api_token)
+        return IBMProvider(token=self.api_token)
```

### Comparing `quao-0.2.0/src/quao/model/provider/provider.py` & `quao-0.2.1/src/quao/model/provider/provider.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.0/src/quao/model/provider/quao_provider.py` & `quao-0.2.1/src/quao/model/provider/quao_provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """
     QuaO Project quao_provider.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
 from qiskit_aer import Aer
 
+from ...enum.processing_unit import ProcessingUnit
 from ...enum.provider_type import ProviderType
 from ...model.provider.provider import Provider
 from braket.devices import LocalSimulator
 from ...config.logging_config import logging
 
+
 class QuaoProvider(Provider):
     def __init__(self):
         super().__init__(ProviderType.QUAO_QUANTUM_SIMULATOR)
 
     def get_backend(self, device_specification):
         """
 
         @param device_specification:
         @return:
         """
 
         providers = self.collect_providers()
-    
+
         aer_device_names = set(map(self.__map_aer_backend_name, providers[0].backends()))
         aws_device_names = providers[1].registered_backends()
 
         if aer_device_names.__contains__(device_specification):
-            return providers[0].get_backend(device_specification)
+            backend = providers[0].get_backend(device_specification)
+            backend.set_options(device=ProcessingUnit.GPU.value)
+            return backend
 
         if aws_device_names.__contains__(device_specification):
             return LocalSimulator(device_specification)
 
         raise Exception('Unsupported device')
 
     def collect_providers(self):
```

### Comparing `quao-0.2.0/src/quao/util/json_parser_util.py` & `quao-0.2.1/src/quao/util/json_parser_util.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.0/src/quao/util/response_utils.py` & `quao-0.2.1/src/quao/util/response_utils.py`

 * *Files identical despite different names*

### Comparing `quao-0.2.0/src/quao.egg-info/PKG-INFO` & `quao-0.2.1/src/quao.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.2.0
+Version: 0.2.1
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.2.0/src/quao.egg-info/SOURCES.txt` & `quao-0.2.1/src/quao.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 src/quao/data/job/job_response.py
 src/quao/data/request/__init__.py
 src/quao/data/request/request_data.py
 src/quao/enum/__init__.py
 src/quao/enum/http_status.py
 src/quao/enum/job_status.py
 src/quao/enum/media_type.py
+src/quao/enum/processing_unit.py
 src/quao/enum/provider_type.py
 src/quao/enum/sdk.py
 src/quao/factory/__init__.py
 src/quao/factory/device_factory.py
 src/quao/factory/provider_factory.py
 src/quao/model/__init__.py
 src/quao/model/device/__init__.py
```

