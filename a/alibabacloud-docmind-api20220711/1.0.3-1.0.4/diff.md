# Comparing `tmp/alibabacloud_docmind-api20220711-1.0.3.tar.gz` & `tmp/alibabacloud_docmind-api20220711-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_docmind-api20220711-1.0.3.tar", last modified: Mon Mar 13 17:13:20 2023, max compression
+gzip compressed data, was "dist/alibabacloud_docmind-api20220711-1.0.4.tar", last modified: Tue Jun 13 06:54:19 2023, max compression
```

## Comparing `alibabacloud_docmind-api20220711-1.0.3.tar` & `alibabacloud_docmind-api20220711-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 17:13:20.000000 alibabacloud_docmind-api20220711-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      200 2023-03-13 17:13:19.000000 alibabacloud_docmind-api20220711-1.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-13 17:13:19.000000 alibabacloud_docmind-api20220711-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-13 17:13:19.000000 alibabacloud_docmind-api20220711-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2376 2023-03-13 17:13:20.000000 alibabacloud_docmind-api20220711-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2023-03-13 17:13:19.000000 alibabacloud_docmind-api20220711-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-03-13 17:13:19.000000 alibabacloud_docmind-api20220711-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 17:13:20.000000 alibabacloud_docmind-api20220711-1.0.3/alibabacloud_docmind_api20220711/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-13 17:13:19.000000 alibabacloud_docmind-api20220711-1.0.3/alibabacloud_docmind_api20220711/__init__.py
--rw-r--r--   0 root         (0) root         (0)   100838 2023-03-13 17:13:19.000000 alibabacloud_docmind-api20220711-1.0.3/alibabacloud_docmind_api20220711/client.py
--rw-r--r--   0 root         (0) root         (0)    78374 2023-03-13 17:13:19.000000 alibabacloud_docmind-api20220711-1.0.3/alibabacloud_docmind_api20220711/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 17:13:20.000000 alibabacloud_docmind-api20220711-1.0.3/alibabacloud_docmind_api20220711.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2376 2023-03-13 17:13:20.000000 alibabacloud_docmind-api20220711-1.0.3/alibabacloud_docmind_api20220711.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2023-03-13 17:13:20.000000 alibabacloud_docmind-api20220711-1.0.3/alibabacloud_docmind_api20220711.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 17:13:20.000000 alibabacloud_docmind-api20220711-1.0.3/alibabacloud_docmind_api20220711.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      315 2023-03-13 17:13:20.000000 alibabacloud_docmind-api20220711-1.0.3/alibabacloud_docmind_api20220711.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-03-13 17:13:20.000000 alibabacloud_docmind-api20220711-1.0.3/alibabacloud_docmind_api20220711.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-13 17:13:20.000000 alibabacloud_docmind-api20220711-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2843 2023-03-13 17:13:19.000000 alibabacloud_docmind-api20220711-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:54:19.000000 alibabacloud_docmind-api20220711-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-13 06:54:18.000000 alibabacloud_docmind-api20220711-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-13 06:54:18.000000 alibabacloud_docmind-api20220711-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-13 06:54:18.000000 alibabacloud_docmind-api20220711-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-06-13 06:54:19.000000 alibabacloud_docmind-api20220711-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-06-13 06:54:18.000000 alibabacloud_docmind-api20220711-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-13 06:54:18.000000 alibabacloud_docmind-api20220711-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:54:19.000000 alibabacloud_docmind-api20220711-1.0.4/alibabacloud_docmind_api20220711/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-13 06:54:18.000000 alibabacloud_docmind-api20220711-1.0.4/alibabacloud_docmind_api20220711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   101078 2023-06-13 06:54:18.000000 alibabacloud_docmind-api20220711-1.0.4/alibabacloud_docmind_api20220711/client.py
+-rw-r--r--   0 root         (0) root         (0)    78948 2023-06-13 06:54:18.000000 alibabacloud_docmind-api20220711-1.0.4/alibabacloud_docmind_api20220711/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:54:19.000000 alibabacloud_docmind-api20220711-1.0.4/alibabacloud_docmind_api20220711.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-06-13 06:54:19.000000 alibabacloud_docmind-api20220711-1.0.4/alibabacloud_docmind_api20220711.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-13 06:54:19.000000 alibabacloud_docmind-api20220711-1.0.4/alibabacloud_docmind_api20220711.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 06:54:19.000000 alibabacloud_docmind-api20220711-1.0.4/alibabacloud_docmind_api20220711.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      315 2023-06-13 06:54:19.000000 alibabacloud_docmind-api20220711-1.0.4/alibabacloud_docmind_api20220711.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-13 06:54:19.000000 alibabacloud_docmind-api20220711-1.0.4/alibabacloud_docmind_api20220711.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-13 06:54:19.000000 alibabacloud_docmind-api20220711-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-06-13 06:54:18.000000 alibabacloud_docmind-api20220711-1.0.4/setup.py
```

### Comparing `alibabacloud_docmind-api20220711-1.0.3/LICENSE` & `alibabacloud_docmind-api20220711-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_docmind-api20220711-1.0.3/PKG-INFO` & `alibabacloud_docmind-api20220711-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_docmind-api20220711
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud docmind-api (20220711) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_docmind-api20220711-1.0.3/README-CN.md` & `alibabacloud_docmind-api20220711-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_docmind-api20220711-1.0.3/README.md` & `alibabacloud_docmind-api20220711-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_docmind-api20220711-1.0.3/alibabacloud_docmind_api20220711/client.py` & `alibabacloud_docmind-api20220711-1.0.4/alibabacloud_docmind_api20220711/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1398,14 +1398,16 @@
         query = {}
         if not UtilClient.is_unset(request.file_name):
             query['FileName'] = request.file_name
         if not UtilClient.is_unset(request.file_name_extension):
             query['FileNameExtension'] = request.file_name_extension
         if not UtilClient.is_unset(request.file_url):
             query['FileUrl'] = request.file_url
+        if not UtilClient.is_unset(request.structure_type):
+            query['StructureType'] = request.structure_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SubmitDocStructureJob',
             version='2022-07-11',
             protocol='HTTPS',
@@ -1430,14 +1432,16 @@
         query = {}
         if not UtilClient.is_unset(request.file_name):
             query['FileName'] = request.file_name
         if not UtilClient.is_unset(request.file_name_extension):
             query['FileNameExtension'] = request.file_name_extension
         if not UtilClient.is_unset(request.file_url):
             query['FileUrl'] = request.file_url
+        if not UtilClient.is_unset(request.structure_type):
+            query['StructureType'] = request.structure_type
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SubmitDocStructureJob',
             version='2022-07-11',
             protocol='HTTPS',
```

### Comparing `alibabacloud_docmind-api20220711-1.0.3/alibabacloud_docmind_api20220711/models.py` & `alibabacloud_docmind-api20220711-1.0.4/alibabacloud_docmind_api20220711/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1887,18 +1887,20 @@
 
 class SubmitDocStructureJobRequest(TeaModel):
     def __init__(
         self,
         file_name: str = None,
         file_name_extension: str = None,
         file_url: str = None,
+        structure_type: str = None,
     ):
         self.file_name = file_name
         self.file_name_extension = file_name_extension
         self.file_url = file_url
+        self.structure_type = structure_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -1907,37 +1909,43 @@
         result = dict()
         if self.file_name is not None:
             result['FileName'] = self.file_name
         if self.file_name_extension is not None:
             result['FileNameExtension'] = self.file_name_extension
         if self.file_url is not None:
             result['FileUrl'] = self.file_url
+        if self.structure_type is not None:
+            result['StructureType'] = self.structure_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('FileName') is not None:
             self.file_name = m.get('FileName')
         if m.get('FileNameExtension') is not None:
             self.file_name_extension = m.get('FileNameExtension')
         if m.get('FileUrl') is not None:
             self.file_url = m.get('FileUrl')
+        if m.get('StructureType') is not None:
+            self.structure_type = m.get('StructureType')
         return self
 
 
 class SubmitDocStructureJobAdvanceRequest(TeaModel):
     def __init__(
         self,
         file_name: str = None,
         file_name_extension: str = None,
         file_url_object: BinaryIO = None,
+        structure_type: str = None,
     ):
         self.file_name = file_name
         self.file_name_extension = file_name_extension
         self.file_url_object = file_url_object
+        self.structure_type = structure_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -1946,24 +1954,28 @@
         result = dict()
         if self.file_name is not None:
             result['FileName'] = self.file_name
         if self.file_name_extension is not None:
             result['FileNameExtension'] = self.file_name_extension
         if self.file_url_object is not None:
             result['FileUrl'] = self.file_url_object
+        if self.structure_type is not None:
+            result['StructureType'] = self.structure_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('FileName') is not None:
             self.file_name = m.get('FileName')
         if m.get('FileNameExtension') is not None:
             self.file_name_extension = m.get('FileNameExtension')
         if m.get('FileUrl') is not None:
             self.file_url_object = m.get('FileUrl')
+        if m.get('StructureType') is not None:
+            self.structure_type = m.get('StructureType')
         return self
 
 
 class SubmitDocStructureJobResponseBodyData(TeaModel):
     def __init__(
         self,
         id: str = None,
```

### Comparing `alibabacloud_docmind-api20220711-1.0.3/alibabacloud_docmind_api20220711.egg-info/PKG-INFO` & `alibabacloud_docmind-api20220711-1.0.4/alibabacloud_docmind_api20220711.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-docmind-api20220711
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud docmind-api (20220711) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_docmind-api20220711-1.0.3/setup.py` & `alibabacloud_docmind-api20220711-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_docmind-api20220711.
 
-Created on 13/03/2023
+Created on 13/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_docmind_api20220711"
 NAME = "alibabacloud_docmind-api20220711" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud docmind-api (20220711) SDK Library for Python"
```

