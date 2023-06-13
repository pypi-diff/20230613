# Comparing `tmp/alibabacloud_docmind-api20220711_py2-1.0.3.tar.gz` & `tmp/alibabacloud_docmind-api20220711_py2-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_docmind-api20220711_py2-1.0.3.tar", last modified: Mon Mar 13 17:12:41 2023, max compression
+gzip compressed data, was "dist/alibabacloud_docmind-api20220711_py2-1.0.4.tar", last modified: Tue Jun 13 06:53:54 2023, max compression
```

## Comparing `alibabacloud_docmind-api20220711_py2-1.0.3.tar` & `alibabacloud_docmind-api20220711_py2-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      200 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2520 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1057 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/alibabacloud_docmind_api20220711/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/alibabacloud_docmind_api20220711/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46702 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/alibabacloud_docmind_api20220711/client.py
--rw-r--r--   0 root         (0) root         (0)    79188 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/alibabacloud_docmind_api20220711/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/alibabacloud_docmind_api20220711_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2520 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/alibabacloud_docmind_api20220711_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      504 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/alibabacloud_docmind_api20220711_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/alibabacloud_docmind_api20220711_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      347 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/alibabacloud_docmind_api20220711_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/alibabacloud_docmind_api20220711_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3152 2023-03-13 17:12:41.000000 alibabacloud_docmind-api20220711_py2-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:53:54.000000 alibabacloud_docmind-api20220711_py2-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-13 06:53:53.000000 alibabacloud_docmind-api20220711_py2-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-13 06:53:53.000000 alibabacloud_docmind-api20220711_py2-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-13 06:53:53.000000 alibabacloud_docmind-api20220711_py2-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2023-06-13 06:53:54.000000 alibabacloud_docmind-api20220711_py2-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-06-13 06:53:53.000000 alibabacloud_docmind-api20220711_py2-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-06-13 06:53:53.000000 alibabacloud_docmind-api20220711_py2-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:53:54.000000 alibabacloud_docmind-api20220711_py2-1.0.4/alibabacloud_docmind_api20220711/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-13 06:53:53.000000 alibabacloud_docmind-api20220711_py2-1.0.4/alibabacloud_docmind_api20220711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46822 2023-06-13 06:53:53.000000 alibabacloud_docmind-api20220711_py2-1.0.4/alibabacloud_docmind_api20220711/client.py
+-rw-r--r--   0 root         (0) root         (0)    79758 2023-06-13 06:53:53.000000 alibabacloud_docmind-api20220711_py2-1.0.4/alibabacloud_docmind_api20220711/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 06:53:54.000000 alibabacloud_docmind-api20220711_py2-1.0.4/alibabacloud_docmind_api20220711_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2023-06-13 06:53:54.000000 alibabacloud_docmind-api20220711_py2-1.0.4/alibabacloud_docmind_api20220711_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      504 2023-06-13 06:53:54.000000 alibabacloud_docmind-api20220711_py2-1.0.4/alibabacloud_docmind_api20220711_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 06:53:54.000000 alibabacloud_docmind-api20220711_py2-1.0.4/alibabacloud_docmind_api20220711_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-13 06:53:54.000000 alibabacloud_docmind-api20220711_py2-1.0.4/alibabacloud_docmind_api20220711_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-13 06:53:54.000000 alibabacloud_docmind-api20220711_py2-1.0.4/alibabacloud_docmind_api20220711_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-13 06:53:54.000000 alibabacloud_docmind-api20220711_py2-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-06-13 06:53:53.000000 alibabacloud_docmind-api20220711_py2-1.0.4/setup.py
```

### Comparing `alibabacloud_docmind-api20220711_py2-1.0.3/LICENSE` & `alibabacloud_docmind-api20220711_py2-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_docmind-api20220711_py2-1.0.3/PKG-INFO` & `alibabacloud_docmind-api20220711_py2-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_docmind-api20220711_py2
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud docmind-api (20220711) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_docmind-api20220711_py2-1.0.3/README-CN.md` & `alibabacloud_docmind-api20220711_py2-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_docmind-api20220711_py2-1.0.3/README.md` & `alibabacloud_docmind-api20220711_py2-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_docmind-api20220711_py2-1.0.3/alibabacloud_docmind_api20220711/client.py` & `alibabacloud_docmind-api20220711_py2-1.0.4/alibabacloud_docmind_api20220711/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,14 +653,16 @@
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

### Comparing `alibabacloud_docmind-api20220711_py2-1.0.3/alibabacloud_docmind_api20220711/models.py` & `alibabacloud_docmind-api20220711_py2-1.0.4/alibabacloud_docmind_api20220711/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1650,18 +1650,19 @@
         if m.get('body') is not None:
             temp_model = SubmitConvertPdfToWordJobResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SubmitDocStructureJobRequest(TeaModel):
-    def __init__(self, file_name=None, file_name_extension=None, file_url=None):
+    def __init__(self, file_name=None, file_name_extension=None, file_url=None, structure_type=None):
         self.file_name = file_name  # type: str
         self.file_name_extension = file_name_extension  # type: str
         self.file_url = file_url  # type: str
+        self.structure_type = structure_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SubmitDocStructureJobRequest, self).to_map()
         if _map is not None:
@@ -1670,32 +1671,37 @@
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
 
     def from_map(self, m=None):
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
-    def __init__(self, file_name=None, file_name_extension=None, file_url_object=None):
+    def __init__(self, file_name=None, file_name_extension=None, file_url_object=None, structure_type=None):
         self.file_name = file_name  # type: str
         self.file_name_extension = file_name_extension  # type: str
         self.file_url_object = file_url_object  # type: READABLE
+        self.structure_type = structure_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SubmitDocStructureJobAdvanceRequest, self).to_map()
         if _map is not None:
@@ -1704,24 +1710,28 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, id=None):
         self.id = id  # type: str
```

### Comparing `alibabacloud_docmind-api20220711_py2-1.0.3/alibabacloud_docmind_api20220711_py2.egg-info/PKG-INFO` & `alibabacloud_docmind-api20220711_py2-1.0.4/alibabacloud_docmind_api20220711_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-docmind-api20220711-py2
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud docmind-api (20220711) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_docmind-api20220711_py2-1.0.3/setup.py` & `alibabacloud_docmind-api20220711_py2-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_docmind-api20220711_py2.
 
-Created on 13/03/2023
+Created on 13/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_docmind_api20220711"
 NAME = "alibabacloud_docmind-api20220711_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud docmind-api (20220711) SDK Library for Python2"
```

