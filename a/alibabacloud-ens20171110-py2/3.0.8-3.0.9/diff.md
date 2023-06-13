# Comparing `tmp/alibabacloud_ens20171110_py2-3.0.8.tar.gz` & `tmp/alibabacloud_ens20171110_py2-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ens20171110_py2-3.0.8.tar", last modified: Thu Sep 22 03:02:00 2022, max compression
+gzip compressed data, was "dist/alibabacloud_ens20171110_py2-3.0.9.tar", last modified: Thu Oct 13 08:56:56 2022, max compression
```

## Comparing `alibabacloud_ens20171110_py2-3.0.8.tar` & `alibabacloud_ens20171110_py2-3.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/
--rw-r--r--   0 root         (0) root         (0)      501 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2486 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/alibabacloud_ens20171110/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/alibabacloud_ens20171110/__init__.py
--rw-r--r--   0 root         (0) root         (0)   265849 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/alibabacloud_ens20171110/client.py
--rw-r--r--   0 root         (0) root         (0)  1153620 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/alibabacloud_ens20171110/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/alibabacloud_ens20171110_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2486 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/alibabacloud_ens20171110_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/alibabacloud_ens20171110_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/alibabacloud_ens20171110_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/alibabacloud_ens20171110_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/alibabacloud_ens20171110_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2917 2022-09-22 03:02:00.000000 alibabacloud_ens20171110_py2-3.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 08:56:56.000000 alibabacloud_ens20171110_py2-3.0.9/
+-rw-r--r--   0 root         (0) root         (0)      552 2022-10-13 08:56:55.000000 alibabacloud_ens20171110_py2-3.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2022-10-13 08:56:55.000000 alibabacloud_ens20171110_py2-3.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2022-10-13 08:56:55.000000 alibabacloud_ens20171110_py2-3.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2486 2022-10-13 08:56:56.000000 alibabacloud_ens20171110_py2-3.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2022-10-13 08:56:55.000000 alibabacloud_ens20171110_py2-3.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2022-10-13 08:56:55.000000 alibabacloud_ens20171110_py2-3.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 08:56:56.000000 alibabacloud_ens20171110_py2-3.0.9/alibabacloud_ens20171110/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-10-13 08:56:55.000000 alibabacloud_ens20171110_py2-3.0.9/alibabacloud_ens20171110/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   267992 2022-10-13 08:56:55.000000 alibabacloud_ens20171110_py2-3.0.9/alibabacloud_ens20171110/client.py
+-rw-r--r--   0 root         (0) root         (0)  1169660 2022-10-13 08:56:55.000000 alibabacloud_ens20171110_py2-3.0.9/alibabacloud_ens20171110/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-13 08:56:56.000000 alibabacloud_ens20171110_py2-3.0.9/alibabacloud_ens20171110_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2486 2022-10-13 08:56:56.000000 alibabacloud_ens20171110_py2-3.0.9/alibabacloud_ens20171110_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2022-10-13 08:56:56.000000 alibabacloud_ens20171110_py2-3.0.9/alibabacloud_ens20171110_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-13 08:56:56.000000 alibabacloud_ens20171110_py2-3.0.9/alibabacloud_ens20171110_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2022-10-13 08:56:56.000000 alibabacloud_ens20171110_py2-3.0.9/alibabacloud_ens20171110_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-10-13 08:56:56.000000 alibabacloud_ens20171110_py2-3.0.9/alibabacloud_ens20171110_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-10-13 08:56:56.000000 alibabacloud_ens20171110_py2-3.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2917 2022-10-13 08:56:55.000000 alibabacloud_ens20171110_py2-3.0.9/setup.py
```

### Comparing `alibabacloud_ens20171110_py2-3.0.8/LICENSE` & `alibabacloud_ens20171110_py2-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ens20171110_py2-3.0.8/PKG-INFO` & `alibabacloud_ens20171110_py2-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ens20171110_py2
-Version: 3.0.8
+Version: 3.0.9
 Summary: Alibaba Cloud edge node service (20171110) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ens20171110_py2-3.0.8/README-CN.md` & `alibabacloud_ens20171110_py2-3.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ens20171110_py2-3.0.8/README.md` & `alibabacloud_ens20171110_py2-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ens20171110_py2-3.0.8/alibabacloud_ens20171110/client.py` & `alibabacloud_ens20171110_py2-3.0.9/alibabacloud_ens20171110/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1912,14 +1912,48 @@
             self.call_api(params, req, runtime)
         )
 
     def delete_vswitch(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_vswitch_with_options(request, runtime)
 
+    def describe_aicimages_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.image_id):
+            query['ImageId'] = request.image_id
+        if not UtilClient.is_unset(request.image_url):
+            query['ImageUrl'] = request.image_url
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeAICImages',
+            version='2017-11-10',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ens_20171110_models.DescribeAICImagesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_aicimages(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_aicimages_with_options(request, runtime)
+
     def describe_armserver_instances_with_options(self, tmp_req, runtime):
         UtilClient.validate_model(tmp_req)
         request = ens_20171110_models.DescribeARMServerInstancesShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.ens_region_ids):
             request.ens_region_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.ens_region_ids, 'EnsRegionIds', 'json')
         if not UtilClient.is_unset(tmp_req.server_ids):
@@ -2980,14 +3014,40 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_export_image_status(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_export_image_status_with_options(request, runtime)
 
+    def describe_file_systems_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = OpenApiUtilClient.query(UtilClient.to_map(request))
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeFileSystems',
+            version='2017-11-10',
+            protocol='HTTPS',
+            pathname='/',
+            method='GET',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ens_20171110_models.DescribeFileSystemsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_file_systems(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_file_systems_with_options(request, runtime)
+
     def describe_forward_table_entries_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.external_ip):
             query['ExternalIp'] = request.external_ip
         if not UtilClient.is_unset(request.forward_entry_id):
             query['ForwardEntryId'] = request.forward_entry_id
@@ -3299,14 +3359,16 @@
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.instance_ids):
             query['InstanceIds'] = request.instance_ids
         if not UtilClient.is_unset(request.instance_name):
             query['InstanceName'] = request.instance_name
         if not UtilClient.is_unset(request.instance_resource_type):
             query['InstanceResourceType'] = request.instance_resource_type
+        if not UtilClient.is_unset(request.intranet_ip):
+            query['IntranetIp'] = request.intranet_ip
         if not UtilClient.is_unset(request.network_id):
             query['NetworkId'] = request.network_id
         if not UtilClient.is_unset(request.order_by_params):
             query['OrderByParams'] = request.order_by_params
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -3805,16 +3867,14 @@
             query['DataDiskSize'] = request.data_disk_size
         if not UtilClient.is_unset(request.ens_region_id):
             query['EnsRegionId'] = request.ens_region_id
         if not UtilClient.is_unset(request.instance_spec):
             query['InstanceSpec'] = request.instance_spec
         if not UtilClient.is_unset(request.system_disk_size):
             query['SystemDiskSize'] = request.system_disk_size
-        if not UtilClient.is_unset(request.version):
-            query['Version'] = request.version
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePrePaidInstanceStock',
             version='2017-11-10',
             protocol='HTTPS',
@@ -4103,16 +4163,14 @@
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.isp):
             query['Isp'] = request.isp
         if not UtilClient.is_unset(request.period):
             query['Period'] = request.period
         if not UtilClient.is_unset(request.start_time):
             query['StartTime'] = request.start_time
-        if not UtilClient.is_unset(request.version):
-            query['Version'] = request.version
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeUserBandWidthData',
             version='2017-11-10',
             protocol='HTTPS',
```

### Comparing `alibabacloud_ens20171110_py2-3.0.8/alibabacloud_ens20171110/models.py` & `alibabacloud_ens20171110_py2-3.0.9/alibabacloud_ens20171110/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -6710,14 +6710,173 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteVSwitchResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeAICImagesRequest(TeaModel):
+    def __init__(self, image_id=None, image_url=None, page_number=None, page_size=None):
+        self.image_id = image_id  # type: str
+        self.image_url = image_url  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeAICImagesRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.image_id is not None:
+            result['ImageId'] = self.image_id
+        if self.image_url is not None:
+            result['ImageUrl'] = self.image_url
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ImageId') is not None:
+            self.image_id = m.get('ImageId')
+        if m.get('ImageUrl') is not None:
+            self.image_url = m.get('ImageUrl')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        return self
+
+
+class DescribeAICImagesResponseBodyImages(TeaModel):
+    def __init__(self, creation_time=None, image_id=None, image_url=None, status=None, user=None):
+        self.creation_time = creation_time  # type: str
+        self.image_id = image_id  # type: str
+        self.image_url = image_url  # type: str
+        self.status = status  # type: str
+        self.user = user  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeAICImagesResponseBodyImages, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.creation_time is not None:
+            result['CreationTime'] = self.creation_time
+        if self.image_id is not None:
+            result['ImageId'] = self.image_id
+        if self.image_url is not None:
+            result['ImageUrl'] = self.image_url
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.user is not None:
+            result['User'] = self.user
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CreationTime') is not None:
+            self.creation_time = m.get('CreationTime')
+        if m.get('ImageId') is not None:
+            self.image_id = m.get('ImageId')
+        if m.get('ImageUrl') is not None:
+            self.image_url = m.get('ImageUrl')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('User') is not None:
+            self.user = m.get('User')
+        return self
+
+
+class DescribeAICImagesResponseBody(TeaModel):
+    def __init__(self, images=None, request_id=None):
+        self.images = images  # type: list[DescribeAICImagesResponseBodyImages]
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.images:
+            for k in self.images:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeAICImagesResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Images'] = []
+        if self.images is not None:
+            for k in self.images:
+                result['Images'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.images = []
+        if m.get('Images') is not None:
+            for k in m.get('Images'):
+                temp_model = DescribeAICImagesResponseBodyImages()
+                self.images.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeAICImagesResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeAICImagesResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeAICImagesResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeAICImagesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeARMServerInstancesRequest(TeaModel):
     def __init__(self, ens_region_ids=None, page_number=None, page_size=None, server_ids=None):
         self.ens_region_ids = ens_region_ids  # type: list[str]
         self.page_number = page_number  # type: int
         self.page_size = page_size  # type: int
         self.server_ids = server_ids  # type: list[str]
 
@@ -13764,14 +13923,273 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeExportImageStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeFileSystemsRequest(TeaModel):
+    def __init__(self, ens_region_id=None, file_system_id=None, file_system_name=None, page_number=None,
+                 page_size=None):
+        self.ens_region_id = ens_region_id  # type: str
+        self.file_system_id = file_system_id  # type: str
+        self.file_system_name = file_system_name  # type: str
+        self.page_number = page_number  # type: int
+        self.page_size = page_size  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeFileSystemsRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ens_region_id is not None:
+            result['EnsRegionId'] = self.ens_region_id
+        if self.file_system_id is not None:
+            result['FileSystemId'] = self.file_system_id
+        if self.file_system_name is not None:
+            result['FileSystemName'] = self.file_system_name
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('EnsRegionId') is not None:
+            self.ens_region_id = m.get('EnsRegionId')
+        if m.get('FileSystemId') is not None:
+            self.file_system_id = m.get('FileSystemId')
+        if m.get('FileSystemName') is not None:
+            self.file_system_name = m.get('FileSystemName')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        return self
+
+
+class DescribeFileSystemsResponseBodyFileSystemsMountTargets(TeaModel):
+    def __init__(self, mount_target_domain=None, mount_target_name=None, net_work_id=None, status=None):
+        self.mount_target_domain = mount_target_domain  # type: str
+        self.mount_target_name = mount_target_name  # type: str
+        self.net_work_id = net_work_id  # type: str
+        self.status = status  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeFileSystemsResponseBodyFileSystemsMountTargets, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.mount_target_domain is not None:
+            result['MountTargetDomain'] = self.mount_target_domain
+        if self.mount_target_name is not None:
+            result['MountTargetName'] = self.mount_target_name
+        if self.net_work_id is not None:
+            result['NetWorkId'] = self.net_work_id
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('MountTargetDomain') is not None:
+            self.mount_target_domain = m.get('MountTargetDomain')
+        if m.get('MountTargetName') is not None:
+            self.mount_target_name = m.get('MountTargetName')
+        if m.get('NetWorkId') is not None:
+            self.net_work_id = m.get('NetWorkId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class DescribeFileSystemsResponseBodyFileSystems(TeaModel):
+    def __init__(self, capacity=None, creation_time=None, ens_region_id=None, file_system_id=None,
+                 file_system_name=None, metered_size=None, mount_targets=None, pay_type=None, protocol_type=None, status=None,
+                 storage_type=None):
+        self.capacity = capacity  # type: long
+        self.creation_time = creation_time  # type: str
+        self.ens_region_id = ens_region_id  # type: str
+        self.file_system_id = file_system_id  # type: str
+        self.file_system_name = file_system_name  # type: str
+        self.metered_size = metered_size  # type: long
+        self.mount_targets = mount_targets  # type: list[DescribeFileSystemsResponseBodyFileSystemsMountTargets]
+        self.pay_type = pay_type  # type: str
+        self.protocol_type = protocol_type  # type: str
+        self.status = status  # type: str
+        self.storage_type = storage_type  # type: str
+
+    def validate(self):
+        if self.mount_targets:
+            for k in self.mount_targets:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeFileSystemsResponseBodyFileSystems, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.capacity is not None:
+            result['Capacity'] = self.capacity
+        if self.creation_time is not None:
+            result['CreationTime'] = self.creation_time
+        if self.ens_region_id is not None:
+            result['EnsRegionId'] = self.ens_region_id
+        if self.file_system_id is not None:
+            result['FileSystemId'] = self.file_system_id
+        if self.file_system_name is not None:
+            result['FileSystemName'] = self.file_system_name
+        if self.metered_size is not None:
+            result['MeteredSize'] = self.metered_size
+        result['MountTargets'] = []
+        if self.mount_targets is not None:
+            for k in self.mount_targets:
+                result['MountTargets'].append(k.to_map() if k else None)
+        if self.pay_type is not None:
+            result['PayType'] = self.pay_type
+        if self.protocol_type is not None:
+            result['ProtocolType'] = self.protocol_type
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.storage_type is not None:
+            result['StorageType'] = self.storage_type
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Capacity') is not None:
+            self.capacity = m.get('Capacity')
+        if m.get('CreationTime') is not None:
+            self.creation_time = m.get('CreationTime')
+        if m.get('EnsRegionId') is not None:
+            self.ens_region_id = m.get('EnsRegionId')
+        if m.get('FileSystemId') is not None:
+            self.file_system_id = m.get('FileSystemId')
+        if m.get('FileSystemName') is not None:
+            self.file_system_name = m.get('FileSystemName')
+        if m.get('MeteredSize') is not None:
+            self.metered_size = m.get('MeteredSize')
+        self.mount_targets = []
+        if m.get('MountTargets') is not None:
+            for k in m.get('MountTargets'):
+                temp_model = DescribeFileSystemsResponseBodyFileSystemsMountTargets()
+                self.mount_targets.append(temp_model.from_map(k))
+        if m.get('PayType') is not None:
+            self.pay_type = m.get('PayType')
+        if m.get('ProtocolType') is not None:
+            self.protocol_type = m.get('ProtocolType')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('StorageType') is not None:
+            self.storage_type = m.get('StorageType')
+        return self
+
+
+class DescribeFileSystemsResponseBody(TeaModel):
+    def __init__(self, file_systems=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        self.file_systems = file_systems  # type: list[DescribeFileSystemsResponseBodyFileSystems]
+        self.page_number = page_number  # type: int
+        self.page_size = page_size  # type: int
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: int
+
+    def validate(self):
+        if self.file_systems:
+            for k in self.file_systems:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeFileSystemsResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['FileSystems'] = []
+        if self.file_systems is not None:
+            for k in self.file_systems:
+                result['FileSystems'].append(k.to_map() if k else None)
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.file_systems = []
+        if m.get('FileSystems') is not None:
+            for k in m.get('FileSystems'):
+                temp_model = DescribeFileSystemsResponseBodyFileSystems()
+                self.file_systems.append(temp_model.from_map(k))
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeFileSystemsResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeFileSystemsResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeFileSystemsResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeFileSystemsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeForwardTableEntriesRequest(TeaModel):
     def __init__(self, external_ip=None, forward_entry_id=None, forward_entry_name=None, internal_ip=None,
                  ip_protocol=None, nat_gateway_id=None, page_number=None, page_size=None):
         self.external_ip = external_ip  # type: str
         self.forward_entry_id = forward_entry_id  # type: str
         self.forward_entry_name = forward_entry_name  # type: str
         self.internal_ip = internal_ip  # type: str
@@ -15378,25 +15796,26 @@
             temp_model = DescribeInstanceVncUrlResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeInstancesRequest(TeaModel):
     def __init__(self, ens_region_id=None, ens_region_ids=None, ens_service_id=None, image_id=None,
-                 instance_id=None, instance_ids=None, instance_name=None, instance_resource_type=None, network_id=None,
-                 order_by_params=None, page_number=None, page_size=None, search_key=None, security_group_id=None, status=None,
-                 v_switch_id=None):
+                 instance_id=None, instance_ids=None, instance_name=None, instance_resource_type=None, intranet_ip=None,
+                 network_id=None, order_by_params=None, page_number=None, page_size=None, search_key=None,
+                 security_group_id=None, status=None, v_switch_id=None):
         self.ens_region_id = ens_region_id  # type: str
         self.ens_region_ids = ens_region_ids  # type: str
         self.ens_service_id = ens_service_id  # type: str
         self.image_id = image_id  # type: str
         self.instance_id = instance_id  # type: str
         self.instance_ids = instance_ids  # type: str
         self.instance_name = instance_name  # type: str
         self.instance_resource_type = instance_resource_type  # type: str
+        self.intranet_ip = intranet_ip  # type: str
         self.network_id = network_id  # type: str
         self.order_by_params = order_by_params  # type: str
         self.page_number = page_number  # type: int
         self.page_size = page_size  # type: str
         self.search_key = search_key  # type: str
         self.security_group_id = security_group_id  # type: str
         self.status = status  # type: str
@@ -15423,14 +15842,16 @@
             result['InstanceId'] = self.instance_id
         if self.instance_ids is not None:
             result['InstanceIds'] = self.instance_ids
         if self.instance_name is not None:
             result['InstanceName'] = self.instance_name
         if self.instance_resource_type is not None:
             result['InstanceResourceType'] = self.instance_resource_type
+        if self.intranet_ip is not None:
+            result['IntranetIp'] = self.intranet_ip
         if self.network_id is not None:
             result['NetworkId'] = self.network_id
         if self.order_by_params is not None:
             result['OrderByParams'] = self.order_by_params
         if self.page_number is not None:
             result['PageNumber'] = self.page_number
         if self.page_size is not None:
@@ -15459,14 +15880,16 @@
             self.instance_id = m.get('InstanceId')
         if m.get('InstanceIds') is not None:
             self.instance_ids = m.get('InstanceIds')
         if m.get('InstanceName') is not None:
             self.instance_name = m.get('InstanceName')
         if m.get('InstanceResourceType') is not None:
             self.instance_resource_type = m.get('InstanceResourceType')
+        if m.get('IntranetIp') is not None:
+            self.intranet_ip = m.get('IntranetIp')
         if m.get('NetworkId') is not None:
             self.network_id = m.get('NetworkId')
         if m.get('OrderByParams') is not None:
             self.order_by_params = m.get('OrderByParams')
         if m.get('PageNumber') is not None:
             self.page_number = m.get('PageNumber')
         if m.get('PageSize') is not None:
@@ -19761,21 +20184,19 @@
         if m.get('body') is not None:
             temp_model = DescribeNetworksResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribePrePaidInstanceStockRequest(TeaModel):
-    def __init__(self, data_disk_size=None, ens_region_id=None, instance_spec=None, system_disk_size=None,
-                 version=None):
+    def __init__(self, data_disk_size=None, ens_region_id=None, instance_spec=None, system_disk_size=None):
         self.data_disk_size = data_disk_size  # type: int
         self.ens_region_id = ens_region_id  # type: str
         self.instance_spec = instance_spec  # type: str
         self.system_disk_size = system_disk_size  # type: int
-        self.version = version  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribePrePaidInstanceStockRequest, self).to_map()
         if _map is not None:
@@ -19786,43 +20207,40 @@
             result['DataDiskSize'] = self.data_disk_size
         if self.ens_region_id is not None:
             result['EnsRegionId'] = self.ens_region_id
         if self.instance_spec is not None:
             result['InstanceSpec'] = self.instance_spec
         if self.system_disk_size is not None:
             result['SystemDiskSize'] = self.system_disk_size
-        if self.version is not None:
-            result['Version'] = self.version
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('DataDiskSize') is not None:
             self.data_disk_size = m.get('DataDiskSize')
         if m.get('EnsRegionId') is not None:
             self.ens_region_id = m.get('EnsRegionId')
         if m.get('InstanceSpec') is not None:
             self.instance_spec = m.get('InstanceSpec')
         if m.get('SystemDiskSize') is not None:
             self.system_disk_size = m.get('SystemDiskSize')
-        if m.get('Version') is not None:
-            self.version = m.get('Version')
         return self
 
 
 class DescribePrePaidInstanceStockResponseBody(TeaModel):
     def __init__(self, avaliable_count=None, cores=None, data_disk_size=None, ens_region_id=None,
-                 instance_spec=None, memory=None, request_id=None, system_disk_size=None):
+                 instance_spec=None, memory=None, request_id=None, resource_gap=None, system_disk_size=None):
         self.avaliable_count = avaliable_count  # type: int
         self.cores = cores  # type: int
         self.data_disk_size = data_disk_size  # type: int
         self.ens_region_id = ens_region_id  # type: str
         self.instance_spec = instance_spec  # type: str
         self.memory = memory  # type: int
         self.request_id = request_id  # type: str
+        self.resource_gap = resource_gap  # type: str
         self.system_disk_size = system_disk_size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribePrePaidInstanceStockResponseBody, self).to_map()
@@ -19840,14 +20258,16 @@
             result['EnsRegionId'] = self.ens_region_id
         if self.instance_spec is not None:
             result['InstanceSpec'] = self.instance_spec
         if self.memory is not None:
             result['Memory'] = self.memory
         if self.request_id is not None:
             result['RequestId'] = self.request_id
+        if self.resource_gap is not None:
+            result['ResourceGap'] = self.resource_gap
         if self.system_disk_size is not None:
             result['SystemDiskSize'] = self.system_disk_size
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AvaliableCount') is not None:
@@ -19860,14 +20280,16 @@
             self.ens_region_id = m.get('EnsRegionId')
         if m.get('InstanceSpec') is not None:
             self.instance_spec = m.get('InstanceSpec')
         if m.get('Memory') is not None:
             self.memory = m.get('Memory')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
+        if m.get('ResourceGap') is not None:
+            self.resource_gap = m.get('ResourceGap')
         if m.get('SystemDiskSize') is not None:
             self.system_disk_size = m.get('SystemDiskSize')
         return self
 
 
 class DescribePrePaidInstanceStockResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
@@ -21832,23 +22254,21 @@
         if m.get('body') is not None:
             temp_model = DescribeSnatTableEntriesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeUserBandWidthDataRequest(TeaModel):
-    def __init__(self, end_time=None, ens_region_id=None, instance_id=None, isp=None, period=None, start_time=None,
-                 version=None):
+    def __init__(self, end_time=None, ens_region_id=None, instance_id=None, isp=None, period=None, start_time=None):
         self.end_time = end_time  # type: str
         self.ens_region_id = ens_region_id  # type: str
         self.instance_id = instance_id  # type: str
         self.isp = isp  # type: str
         self.period = period  # type: str
         self.start_time = start_time  # type: str
-        self.version = version  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserBandWidthDataRequest, self).to_map()
         if _map is not None:
@@ -21863,16 +22283,14 @@
             result['InstanceId'] = self.instance_id
         if self.isp is not None:
             result['Isp'] = self.isp
         if self.period is not None:
             result['Period'] = self.period
         if self.start_time is not None:
             result['StartTime'] = self.start_time
-        if self.version is not None:
-            result['Version'] = self.version
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         if m.get('EnsRegionId') is not None:
@@ -21881,27 +22299,25 @@
             self.instance_id = m.get('InstanceId')
         if m.get('Isp') is not None:
             self.isp = m.get('Isp')
         if m.get('Period') is not None:
             self.period = m.get('Period')
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
-        if m.get('Version') is not None:
-            self.version = m.get('Version')
         return self
 
 
 class DescribeUserBandWidthDataResponseBodyMonitorDataBandWidthMonitorData(TeaModel):
     def __init__(self, down_band_width=None, internet_rx=None, internet_tx=None, time_stamp=None,
                  up_band_width=None):
-        self.down_band_width = down_band_width  # type: int
-        self.internet_rx = internet_rx  # type: int
-        self.internet_tx = internet_tx  # type: int
+        self.down_band_width = down_band_width  # type: long
+        self.internet_rx = internet_rx  # type: long
+        self.internet_tx = internet_tx  # type: long
         self.time_stamp = time_stamp  # type: str
-        self.up_band_width = up_band_width  # type: int
+        self.up_band_width = up_band_width  # type: long
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeUserBandWidthDataResponseBodyMonitorDataBandWidthMonitorData, self).to_map()
         if _map is not None:
```

### Comparing `alibabacloud_ens20171110_py2-3.0.8/alibabacloud_ens20171110_py2.egg-info/PKG-INFO` & `alibabacloud_ens20171110_py2-3.0.9/alibabacloud_ens20171110_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ens20171110-py2
-Version: 3.0.8
+Version: 3.0.9
 Summary: Alibaba Cloud edge node service (20171110) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ens20171110_py2-3.0.8/setup.py` & `alibabacloud_ens20171110_py2-3.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ens20171110_py2.
 
-Created on 22/09/2022
+Created on 13/10/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ens20171110"
 NAME = "alibabacloud_ens20171110_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud edge node service (20171110) SDK Library for Python2"
```

